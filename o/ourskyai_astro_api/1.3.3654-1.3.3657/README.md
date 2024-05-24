# Comparing `tmp/ourskyai_astro_api-1.3.3654.tar.gz` & `tmp/ourskyai_astro_api-1.3.3657.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_astro_api-1.3.3654.tar", max compression
+gzip compressed data, was "ourskyai_astro_api-1.3.3657.tar", max compression
```

## Comparing `ourskyai_astro_api-1.3.3654.tar` & `ourskyai_astro_api-1.3.3657.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0    11493 2024-05-23 19:26:18.682597 ourskyai_astro_api-1.3.3654/README.md
--rw-r--r--   0        0        0     6218 2024-05-23 19:26:22.446235 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/__init__.py
--rw-r--r--   0        0        0      106 2024-05-23 19:26:22.482232 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/api/__init__.py
--rw-r--r--   0        0        0   260295 2024-05-23 19:26:22.582222 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/api/default_api.py
--rw-r--r--   0        0        0    30352 2024-05-23 19:26:22.630218 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-23 19:26:22.718209 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/api_response.py
--rw-r--r--   0        0        0    14687 2024-05-23 19:26:22.826199 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/configuration.py
--rw-r--r--   0        0        0     5433 2024-05-23 19:26:22.874194 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/exceptions.py
--rw-r--r--   0        0        0     5577 2024-05-23 19:26:22.918190 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/__init__.py
--rw-r--r--   0        0        0      819 2024-05-23 19:26:22.962186 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/asset_file_type.py
--rw-r--r--   0        0        0      931 2024-05-23 19:26:23.010181 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/asset_type.py
--rw-r--r--   0        0        0      809 2024-05-23 19:26:23.066176 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/calibration_master_type.py
--rw-r--r--   0        0        0     4308 2024-05-23 19:26:23.126170 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/daily_weather_forecast_item.py
--rw-r--r--   0        0        0     2527 2024-05-23 19:26:23.210162 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py
--rw-r--r--   0        0        0     2551 2024-05-23 19:26:23.246158 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py
--rw-r--r--   0        0        0     2562 2024-05-23 19:26:23.290154 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/daily_weather_forecast_list_response.py
--rw-r--r--   0        0        0     1904 2024-05-23 19:26:23.350149 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/empty_success.py
--rw-r--r--   0        0        0     1186 2024-05-23 19:26:23.386145 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/filter_type.py
--rw-r--r--   0        0        0     1930 2024-05-23 19:26:23.430141 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/fits_header.py
--rw-r--r--   0        0        0     2155 2024-05-23 19:26:23.490135 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/location.py
--rw-r--r--   0        0        0      747 2024-05-23 19:26:23.530131 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/mount_type.py
--rw-r--r--   0        0        0      887 2024-05-23 19:26:23.642120 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/node_state.py
--rw-r--r--   0        0        0      827 2024-05-23 19:26:23.678117 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/optical_tube_type.py
--rw-r--r--   0        0        0      751 2024-05-23 19:26:23.738111 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/shutter_type.py
--rw-r--r--   0        0        0     1892 2024-05-23 19:26:23.798105 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/successful_create.py
--rw-r--r--   0        0        0      768 2024-05-23 19:26:23.886097 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/tracking_type.py
--rw-r--r--   0        0        0     3258 2024-05-23 19:26:23.970089 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_project.py
--rw-r--r--   0        0        0     3969 2024-05-23 19:26:24.014085 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_project_asset.py
--rw-r--r--   0        0        0     2569 2024-05-23 19:26:24.066080 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
--rw-r--r--   0        0        0     2399 2024-05-23 19:26:24.122074 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
--rw-r--r--   0        0        0     2381 2024-05-23 19:26:24.186068 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_target.py
--rw-r--r--   0        0        0     3640 2024-05-23 19:26:24.238063 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_calibration_master.py
--rw-r--r--   0        0        0     4908 2024-05-23 19:26:24.290058 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_camera.py
--rw-r--r--   0        0        0     2421 2024-05-23 19:26:24.330054 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
--rw-r--r--   0        0        0     2668 2024-05-23 19:26:24.398048 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_astro_project_request.py
--rw-r--r--   0        0        0     2121 2024-05-23 19:26:24.434044 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_astro_project_response.py
--rw-r--r--   0        0        0     3777 2024-05-23 19:26:24.474040 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_calibration_master_request.py
--rw-r--r--   0        0        0     2147 2024-05-23 19:26:24.518036 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_calibration_master_response.py
--rw-r--r--   0        0        0     7059 2024-05-23 19:26:24.582030 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_camera_request.py
--rw-r--r--   0        0        0     2044 2024-05-23 19:26:24.638025 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2115 2024-05-23 19:26:24.690020 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2683 2024-05-23 19:26:24.738015 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2296 2024-05-23 19:26:24.798009 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     3146 2024-05-23 19:26:24.854004 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2447 2024-05-23 19:26:24.917998 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2441 2024-05-23 19:26:24.973992 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0     3289 2024-05-23 19:26:25.013989 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2051 2024-05-23 19:26:25.061984 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2096 2024-05-23 19:26:25.133977 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
--rw-r--r--   0        0        0     2364 2024-05-23 19:26:25.181972 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7066 2024-05-23 19:26:25.209970 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2324 2024-05-23 19:26:25.289962 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2513 2024-05-23 19:26:25.321959 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     3436 2024-05-23 19:26:25.365955 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5797 2024-05-23 19:26:25.409951 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0      795 2024-05-23 19:26:25.441947 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_job_kind.py
--rw-r--r--   0        0        0     2632 2024-05-23 19:26:25.485943 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_job_log.py
--rw-r--r--   0        0        0      803 2024-05-23 19:26:25.573935 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_job_status.py
--rw-r--r--   0        0        0     1914 2024-05-23 19:26:25.621930 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_mount.py
--rw-r--r--   0        0        0     4458 2024-05-23 19:26:25.701923 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_node.py
--rw-r--r--   0        0        0     2564 2024-05-23 19:26:25.753917 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     2239 2024-05-23 19:26:25.805912 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     3057 2024-05-23 19:26:25.889904 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_platform_credit.py
--rw-r--r--   0        0        0      870 2024-05-23 19:26:25.949899 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_platform_credit_source.py
--rw-r--r--   0        0        0      800 2024-05-23 19:26:25.985895 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_platform_credit_type.py
--rw-r--r--   0        0        0      776 2024-05-23 19:26:26.065888 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_platform_credit_unit.py
--rw-r--r--   0        0        0     2045 2024-05-23 19:26:26.121882 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
--rw-r--r--   0        0        0     2051 2024-05-23 19:26:26.157878 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2050 2024-05-23 19:26:26.221872 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2940 2024-05-23 19:26:26.269868 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2240 2024-05-23 19:26:26.313864 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     4605 2024-05-23 19:26:26.373858 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2522 2024-05-23 19:26:26.437852 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0        0 2024-05-23 19:26:26.469848 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/py.typed
--rw-r--r--   0        0        0    12935 2024-05-23 19:26:26.513844 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/rest.py
--rw-r--r--   0        0        0      739 2024-05-23 19:26:26.573839 ourskyai_astro_api-1.3.3654/pyproject.toml
--rw-r--r--   0        0        0    12461 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3654/PKG-INFO
+-rw-r--r--   0        0        0    11493 2024-05-23 23:15:12.509300 ourskyai_astro_api-1.3.3657/README.md
+-rw-r--r--   0        0        0     6218 2024-05-23 23:15:15.948699 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-23 23:15:15.976694 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/api/__init__.py
+-rw-r--r--   0        0        0   260295 2024-05-23 23:15:16.052681 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/api/default_api.py
+-rw-r--r--   0        0        0    30352 2024-05-23 23:15:16.096673 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-23 23:15:16.136666 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/api_response.py
+-rw-r--r--   0        0        0    14687 2024-05-23 23:15:16.172660 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/configuration.py
+-rw-r--r--   0        0        0     5433 2024-05-23 23:15:16.208654 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/exceptions.py
+-rw-r--r--   0        0        0     5577 2024-05-23 23:15:16.252646 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/__init__.py
+-rw-r--r--   0        0        0      819 2024-05-23 23:15:16.292639 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/asset_file_type.py
+-rw-r--r--   0        0        0      931 2024-05-23 23:15:16.320634 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/asset_type.py
+-rw-r--r--   0        0        0      809 2024-05-23 23:15:16.388622 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/calibration_master_type.py
+-rw-r--r--   0        0        0     4308 2024-05-23 23:15:16.440613 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/daily_weather_forecast_item.py
+-rw-r--r--   0        0        0     2527 2024-05-23 23:15:16.488605 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py
+-rw-r--r--   0        0        0     2551 2024-05-23 23:15:16.548594 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py
+-rw-r--r--   0        0        0     2562 2024-05-23 23:15:16.600585 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/daily_weather_forecast_list_response.py
+-rw-r--r--   0        0        0     1904 2024-05-23 23:15:16.652576 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/empty_success.py
+-rw-r--r--   0        0        0     1186 2024-05-23 23:15:16.704567 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/filter_type.py
+-rw-r--r--   0        0        0     1930 2024-05-23 23:15:16.768556 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/fits_header.py
+-rw-r--r--   0        0        0     2155 2024-05-23 23:15:16.824546 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/location.py
+-rw-r--r--   0        0        0      747 2024-05-23 23:15:16.864539 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/mount_type.py
+-rw-r--r--   0        0        0      887 2024-05-23 23:15:16.932527 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/node_state.py
+-rw-r--r--   0        0        0      827 2024-05-23 23:15:16.972520 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0      751 2024-05-23 23:15:17.056506 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1892 2024-05-23 23:15:17.104497 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/successful_create.py
+-rw-r--r--   0        0        0      768 2024-05-23 23:15:17.148489 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/tracking_type.py
+-rw-r--r--   0        0        0     3258 2024-05-23 23:15:17.240473 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_project.py
+-rw-r--r--   0        0        0     3969 2024-05-23 23:15:17.284466 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_project_asset.py
+-rw-r--r--   0        0        0     2569 2024-05-23 23:15:17.348454 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
+-rw-r--r--   0        0        0     2399 2024-05-23 23:15:17.392447 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
+-rw-r--r--   0        0        0     2381 2024-05-23 23:15:17.452436 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_target.py
+-rw-r--r--   0        0        0     3640 2024-05-23 23:15:17.540421 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_calibration_master.py
+-rw-r--r--   0        0        0     4908 2024-05-23 23:15:17.596411 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2421 2024-05-23 23:15:17.644403 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
+-rw-r--r--   0        0        0     2668 2024-05-23 23:15:17.692394 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_astro_project_request.py
+-rw-r--r--   0        0        0     2121 2024-05-23 23:15:17.740386 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_astro_project_response.py
+-rw-r--r--   0        0        0     3777 2024-05-23 23:15:17.792377 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_calibration_master_request.py
+-rw-r--r--   0        0        0     2147 2024-05-23 23:15:17.832370 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_calibration_master_response.py
+-rw-r--r--   0        0        0     7059 2024-05-23 23:15:17.892359 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_camera_request.py
+-rw-r--r--   0        0        0     2044 2024-05-23 23:15:17.936352 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2115 2024-05-23 23:15:17.988343 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2683 2024-05-23 23:15:18.044333 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2296 2024-05-23 23:15:18.100323 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     3146 2024-05-23 23:15:18.156313 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2447 2024-05-23 23:15:18.204305 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2441 2024-05-23 23:15:18.256296 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0     3289 2024-05-23 23:15:18.312286 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2051 2024-05-23 23:15:18.380274 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2096 2024-05-23 23:15:18.464259 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
+-rw-r--r--   0        0        0     2364 2024-05-23 23:15:18.520250 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7066 2024-05-23 23:15:18.576240 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2324 2024-05-23 23:15:18.608234 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2513 2024-05-23 23:15:18.656226 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     3436 2024-05-23 23:15:18.720215 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5797 2024-05-23 23:15:18.764207 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0      795 2024-05-23 23:15:18.812198 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_job_kind.py
+-rw-r--r--   0        0        0     2632 2024-05-23 23:15:18.860190 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_job_log.py
+-rw-r--r--   0        0        0      803 2024-05-23 23:15:18.928178 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_job_status.py
+-rw-r--r--   0        0        0     1914 2024-05-23 23:15:18.972171 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4458 2024-05-23 23:15:19.020162 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_node.py
+-rw-r--r--   0        0        0     2564 2024-05-23 23:15:19.088150 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     2239 2024-05-23 23:15:19.128143 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     3057 2024-05-23 23:15:19.176135 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_platform_credit.py
+-rw-r--r--   0        0        0      870 2024-05-23 23:15:19.232125 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_platform_credit_source.py
+-rw-r--r--   0        0        0      800 2024-05-23 23:15:19.272118 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_platform_credit_type.py
+-rw-r--r--   0        0        0      776 2024-05-23 23:15:19.324109 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_platform_credit_unit.py
+-rw-r--r--   0        0        0     2045 2024-05-23 23:15:19.368101 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
+-rw-r--r--   0        0        0     2051 2024-05-23 23:15:19.444088 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2050 2024-05-23 23:15:19.496079 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2940 2024-05-23 23:15:19.548070 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2240 2024-05-23 23:15:19.592062 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     4605 2024-05-23 23:15:19.652052 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2522 2024-05-23 23:15:19.700043 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0        0 2024-05-23 23:15:19.732038 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/py.typed
+-rw-r--r--   0        0        0    12935 2024-05-23 23:15:19.780029 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/rest.py
+-rw-r--r--   0        0        0      739 2024-05-23 23:15:19.812024 ourskyai_astro_api-1.3.3657/pyproject.toml
+-rw-r--r--   0        0        0    12461 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3657/PKG-INFO
```

### Comparing `ourskyai_astro_api-1.3.3654/README.md` & `ourskyai_astro_api-1.3.3657/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-astro-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3654
-- Package version: 1.3.3654
+- API version: 1.3.3657
+- Package version: 1.3.3657
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/__init__.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3654"
+__version__ = "1.3.3657"
 
 # import apis into sdk package
 from ourskyai_astro_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_astro_api.api_response import ApiResponse
 from ourskyai_astro_api.api_client import ApiClient
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/api/default_api.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/api_client.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
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
-        self.user_agent = 'OpenAPI-Generator/1.3.3654/python'
+        self.user_agent = 'OpenAPI-Generator/1.3.3657/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/api_response.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/configuration.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
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
-               "Version of the API: 1.3.3654\n"\
-               "SDK Package Version: 1.3.3654".\
+               "Version of the API: 1.3.3657\n"\
+               "SDK Package Version: 1.3.3657".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/exceptions.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/__init__.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/asset_file_type.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/asset_file_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/asset_type.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/asset_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/calibration_master_type.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/calibration_master_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/daily_weather_forecast_item.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/daily_weather_forecast_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/daily_weather_forecast_list_response.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/daily_weather_forecast_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/empty_success.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/empty_success.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/filter_type.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/filter_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/fits_header.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/fits_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/location.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/mount_type.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/mount_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/node_state.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/node_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/optical_tube_type.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/optical_tube_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/shutter_type.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/shutter_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/successful_create.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/successful_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/tracking_type.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/tracking_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_project.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_project_asset.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_project_asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_target.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_calibration_master.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_calibration_master.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_camera.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_astro_project_request.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_astro_project_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_astro_project_response.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_astro_project_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_calibration_master_request.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_calibration_master_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_calibration_master_response.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_calibration_master_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_camera_request.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_camera_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_image_set_image_request.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_image_set_image_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_image_set_image_response.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_image_set_image_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_image_set_request.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_image_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_mount_request.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_node_request.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_optical_tube_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_elevation_mask_point.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_elevation_mask_point.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_gain_curve.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_gain_curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_gain_curve_point.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_gain_curve_point.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_nodes.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_or_create_camera_request.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_or_create_camera_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_or_create_mount_request.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_or_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_image_set.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_image_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_image_set_image.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_image_set_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_job_kind.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_job_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_job_log.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_job_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_mount.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_mount.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_node.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_node_with_location.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_node_with_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_optical_tube.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_optical_tube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_platform_credit.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_platform_credit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_platform_credit_source.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_platform_credit_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_platform_credit_type.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_platform_credit_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_platform_credit_unit.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_platform_credit_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_read_noise_point.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_read_noise_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_setup_action.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_setup_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_slew_timing.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_slew_timing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_slew_timing_interval.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_slew_timing_interval.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_update_node_request.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_update_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_video_mode_framerate_property.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_video_mode_framerate_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/rest.py` & `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_astro_api-1.3.3654/pyproject.toml` & `ourskyai_astro_api-1.3.3657/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_astro_api"
-version = "1.3.3654"
+version = "1.3.3657"
 description = "OurSky Astro"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Astro"]
 include = ["ourskyai_astro_api/py.typed"]
```

### Comparing `ourskyai_astro_api-1.3.3654/PKG-INFO` & `ourskyai_astro_api-1.3.3657/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_astro_api
-Version: 1.3.3654
+Version: 1.3.3657
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
 
-- API version: 1.3.3654
-- Package version: 1.3.3654
+- API version: 1.3.3657
+- Package version: 1.3.3657
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

