# Comparing `tmp/ourskyai_platform_api-1.3.3657.tar.gz` & `tmp/ourskyai_platform_api-1.3.3661.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_platform_api-1.3.3657.tar", max compression
+gzip compressed data, was "ourskyai_platform_api-1.3.3661.tar", max compression
```

## Comparing `ourskyai_platform_api-1.3.3657.tar` & `ourskyai_platform_api-1.3.3661.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     9968 2024-05-23 23:15:12.461309 ourskyai_platform_api-1.3.3657/README.md
--rw-r--r--   0        0        0     6552 2024-05-23 23:15:16.024686 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/__init__.py
--rw-r--r--   0        0        0      109 2024-05-23 23:15:16.056680 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/api/__init__.py
--rw-r--r--   0        0        0   206365 2024-05-23 23:15:16.132667 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/api/default_api.py
--rw-r--r--   0        0        0    30373 2024-05-23 23:15:16.180659 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-23 23:15:16.232649 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/api_response.py
--rw-r--r--   0        0        0    14693 2024-05-23 23:15:16.276642 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/configuration.py
--rw-r--r--   0        0        0     5436 2024-05-23 23:15:16.320634 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/exceptions.py
--rw-r--r--   0        0        0     5881 2024-05-23 23:15:16.360627 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/__init__.py
--rw-r--r--   0        0        0      745 2024-05-23 23:15:16.428615 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/camera_mode.py
--rw-r--r--   0        0        0     1907 2024-05-23 23:15:16.540596 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/empty_success.py
--rw-r--r--   0        0        0     1189 2024-05-23 23:15:16.572590 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/filter_type.py
--rw-r--r--   0        0        0     1933 2024-05-23 23:15:16.624581 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/fits_header.py
--rw-r--r--   0        0        0     2158 2024-05-23 23:15:16.708566 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/location.py
--rw-r--r--   0        0        0      777 2024-05-23 23:15:16.780554 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/metric_type.py
--rw-r--r--   0        0        0      750 2024-05-23 23:15:16.856541 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/mount_type.py
--rw-r--r--   0        0        0      890 2024-05-23 23:15:16.908531 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/node_state.py
--rw-r--r--   0        0        0      830 2024-05-23 23:15:16.952524 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/optical_tube_type.py
--rw-r--r--   0        0        0     2407 2024-05-23 23:15:17.032510 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/plate_solve_parameters.py
--rw-r--r--   0        0        0      754 2024-05-23 23:15:17.080501 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/shutter_type.py
--rw-r--r--   0        0        0     1895 2024-05-23 23:15:17.120494 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/successful_create.py
--rw-r--r--   0        0        0      771 2024-05-23 23:15:17.168486 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/tracking_type.py
--rw-r--r--   0        0        0     2622 2024-05-23 23:15:17.204480 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_auto_focus_instruction.py
--rw-r--r--   0        0        0     2366 2024-05-23 23:15:17.248472 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py
--rw-r--r--   0        0        0     4920 2024-05-23 23:15:17.288465 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_camera.py
--rw-r--r--   0        0        0     2115 2024-05-23 23:15:17.388447 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_client_token.py
--rw-r--r--   0        0        0     2047 2024-05-23 23:15:17.424441 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_complete_observation_request.py
--rw-r--r--   0        0        0     2047 2024-05-23 23:15:17.476432 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2118 2024-05-23 23:15:17.512426 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2692 2024-05-23 23:15:17.560417 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2302 2024-05-23 23:15:17.604410 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     2071 2024-05-23 23:15:17.664399 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py
--rw-r--r--   0        0        0     2710 2024-05-23 23:15:17.728388 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_node_diagnostic.py
--rw-r--r--   0        0        0     2715 2024-05-23 23:15:17.788378 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
--rw-r--r--   0        0        0     3152 2024-05-23 23:15:17.828371 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2453 2024-05-23 23:15:17.860365 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2124 2024-05-23 23:15:17.924354 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_diagnostic_instruction.py
--rw-r--r--   0        0        0     2444 2024-05-23 23:15:17.968346 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0      719 2024-05-23 23:15:18.036334 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_file_type.py
--rw-r--r--   0        0        0     3298 2024-05-23 23:15:18.116320 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2054 2024-05-23 23:15:18.148315 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2570 2024-05-23 23:15:18.204305 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_instruction_request.py
--rw-r--r--   0        0        0     2370 2024-05-23 23:15:18.248297 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7081 2024-05-23 23:15:18.296289 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2330 2024-05-23 23:15:18.344280 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2519 2024-05-23 23:15:18.396271 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     2675 2024-05-23 23:15:18.456261 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
--rw-r--r--   0        0        0     3985 2024-05-23 23:15:18.540246 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_ground_station_participant.py
--rw-r--r--   0        0        0     3445 2024-05-23 23:15:18.604235 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5803 2024-05-23 23:15:18.644228 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0     3763 2024-05-23 23:15:18.676222 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_instruction.py
--rw-r--r--   0        0        0     2400 2024-05-23 23:15:18.724214 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_metric.py
--rw-r--r--   0        0        0     1917 2024-05-23 23:15:18.800201 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_mount.py
--rw-r--r--   0        0        0     4470 2024-05-23 23:15:18.848192 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node.py
--rw-r--r--   0        0        0      850 2024-05-23 23:15:18.880187 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node_component_type.py
--rw-r--r--   0        0        0     1963 2024-05-23 23:15:18.924179 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node_controller_artifact.py
--rw-r--r--   0        0        0     1669 2024-05-23 23:15:18.972171 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node_diagnostic_type.py
--rw-r--r--   0        0        0     2573 2024-05-23 23:15:19.020162 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     5537 2024-05-23 23:15:19.076152 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_observation_instruction.py
--rw-r--r--   0        0        0     2242 2024-05-23 23:15:19.152139 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     2135 2024-05-23 23:15:19.200131 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
--rw-r--r--   0        0        0     2648 2024-05-23 23:15:19.240124 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
--rw-r--r--   0        0        0     2054 2024-05-23 23:15:19.288115 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2401 2024-05-23 23:15:19.352104 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_release.py
--rw-r--r--   0        0        0     2053 2024-05-23 23:15:19.400096 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2946 2024-05-23 23:15:19.444088 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2243 2024-05-23 23:15:19.516075 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     3601 2024-05-23 23:15:19.568066 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_components_request.py
--rw-r--r--   0        0        0     6269 2024-05-23 23:15:19.612059 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
--rw-r--r--   0        0        0     2402 2024-05-23 23:15:19.656051 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
--rw-r--r--   0        0        0     2591 2024-05-23 23:15:19.708042 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
--rw-r--r--   0        0        0     4620 2024-05-23 23:15:19.760033 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2525 2024-05-23 23:15:19.812024 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0     2224 2024-05-23 23:15:19.872013 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v2_complete_observation_request.py
--rw-r--r--   0        0        0        0 2024-05-23 23:15:19.904008 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/py.typed
--rw-r--r--   0        0        0    12941 2024-05-23 23:15:19.955999 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/rest.py
--rw-r--r--   0        0        0      751 2024-05-23 23:15:19.995992 ourskyai_platform_api-1.3.3657/pyproject.toml
--rw-r--r--   0        0        0    10945 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3657/PKG-INFO
+-rw-r--r--   0        0        0     9968 2024-05-24 01:28:40.901336 ourskyai_platform_api-1.3.3661/README.md
+-rw-r--r--   0        0        0     6552 2024-05-24 01:28:44.541375 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/__init__.py
+-rw-r--r--   0        0        0      109 2024-05-24 01:28:44.573375 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/api/__init__.py
+-rw-r--r--   0        0        0   206365 2024-05-24 01:28:44.681376 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/api/default_api.py
+-rw-r--r--   0        0        0    30373 2024-05-24 01:28:44.753377 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-24 01:28:44.793377 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/api_response.py
+-rw-r--r--   0        0        0    14693 2024-05-24 01:28:44.833378 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/configuration.py
+-rw-r--r--   0        0        0     5436 2024-05-24 01:28:44.877378 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/exceptions.py
+-rw-r--r--   0        0        0     5881 2024-05-24 01:28:44.917379 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-24 01:28:44.961379 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/camera_mode.py
+-rw-r--r--   0        0        0     1907 2024-05-24 01:28:45.001379 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/empty_success.py
+-rw-r--r--   0        0        0     1189 2024-05-24 01:28:45.057380 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/filter_type.py
+-rw-r--r--   0        0        0     1933 2024-05-24 01:28:45.113381 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/fits_header.py
+-rw-r--r--   0        0        0     2158 2024-05-24 01:28:45.173381 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/location.py
+-rw-r--r--   0        0        0      777 2024-05-24 01:28:45.213382 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/metric_type.py
+-rw-r--r--   0        0        0      750 2024-05-24 01:28:45.265382 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/mount_type.py
+-rw-r--r--   0        0        0      890 2024-05-24 01:28:45.337383 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/node_state.py
+-rw-r--r--   0        0        0      830 2024-05-24 01:28:45.377383 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0     2407 2024-05-24 01:28:45.417384 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/plate_solve_parameters.py
+-rw-r--r--   0        0        0      754 2024-05-24 01:28:45.493384 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1895 2024-05-24 01:28:45.561385 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/successful_create.py
+-rw-r--r--   0        0        0      771 2024-05-24 01:28:45.649386 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/tracking_type.py
+-rw-r--r--   0        0        0     2622 2024-05-24 01:28:45.701387 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_auto_focus_instruction.py
+-rw-r--r--   0        0        0     2366 2024-05-24 01:28:45.745387 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py
+-rw-r--r--   0        0        0     4920 2024-05-24 01:28:45.793388 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2115 2024-05-24 01:28:45.877388 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_client_token.py
+-rw-r--r--   0        0        0     2047 2024-05-24 01:28:45.909389 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_complete_observation_request.py
+-rw-r--r--   0        0        0     2047 2024-05-24 01:28:46.017390 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2118 2024-05-24 01:28:46.065390 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2692 2024-05-24 01:28:46.117391 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2302 2024-05-24 01:28:46.173391 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     2071 2024-05-24 01:28:46.221392 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py
+-rw-r--r--   0        0        0     2710 2024-05-24 01:28:46.277392 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_node_diagnostic.py
+-rw-r--r--   0        0        0     2715 2024-05-24 01:28:46.321393 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
+-rw-r--r--   0        0        0     3152 2024-05-24 01:28:46.365393 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2453 2024-05-24 01:28:46.417394 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2124 2024-05-24 01:28:46.469394 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_diagnostic_instruction.py
+-rw-r--r--   0        0        0     2444 2024-05-24 01:28:46.537395 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0      719 2024-05-24 01:28:46.613396 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_file_type.py
+-rw-r--r--   0        0        0     3298 2024-05-24 01:28:46.661396 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2054 2024-05-24 01:28:46.721397 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2570 2024-05-24 01:28:46.761397 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_get_instruction_request.py
+-rw-r--r--   0        0        0     2370 2024-05-24 01:28:46.809398 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7081 2024-05-24 01:28:46.873398 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2330 2024-05-24 01:28:46.913399 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2519 2024-05-24 01:28:46.961399 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2675 2024-05-24 01:28:47.017400 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
+-rw-r--r--   0        0        0     3985 2024-05-24 01:28:47.125401 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_ground_station_participant.py
+-rw-r--r--   0        0        0     3445 2024-05-24 01:28:47.177401 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5803 2024-05-24 01:28:47.229402 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0     3763 2024-05-24 01:28:47.273403 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_instruction.py
+-rw-r--r--   0        0        0     2400 2024-05-24 01:28:47.329403 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_metric.py
+-rw-r--r--   0        0        0     1917 2024-05-24 01:28:47.389404 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4470 2024-05-24 01:28:47.429404 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_node.py
+-rw-r--r--   0        0        0      850 2024-05-24 01:28:47.493405 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_node_component_type.py
+-rw-r--r--   0        0        0     1963 2024-05-24 01:28:47.545405 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_node_controller_artifact.py
+-rw-r--r--   0        0        0     1669 2024-05-24 01:28:47.629406 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_node_diagnostic_type.py
+-rw-r--r--   0        0        0     2573 2024-05-24 01:28:47.725407 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     5537 2024-05-24 01:28:47.773408 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_observation_instruction.py
+-rw-r--r--   0        0        0     2242 2024-05-24 01:28:47.817408 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     2135 2024-05-24 01:28:47.885409 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
+-rw-r--r--   0        0        0     2648 2024-05-24 01:28:47.929409 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
+-rw-r--r--   0        0        0     2054 2024-05-24 01:28:47.989410 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2401 2024-05-24 01:28:48.029410 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_release.py
+-rw-r--r--   0        0        0     2053 2024-05-24 01:28:48.085411 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2946 2024-05-24 01:28:48.125411 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2243 2024-05-24 01:28:48.169412 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     3601 2024-05-24 01:28:48.205412 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_update_node_components_request.py
+-rw-r--r--   0        0        0     6269 2024-05-24 01:28:48.269413 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
+-rw-r--r--   0        0        0     2402 2024-05-24 01:28:48.313413 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
+-rw-r--r--   0        0        0     2591 2024-05-24 01:28:48.357413 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
+-rw-r--r--   0        0        0     4620 2024-05-24 01:28:48.409414 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2525 2024-05-24 01:28:48.453415 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0     2224 2024-05-24 01:28:48.497415 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v2_complete_observation_request.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:28:48.525415 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/py.typed
+-rw-r--r--   0        0        0    12941 2024-05-24 01:28:48.605416 ourskyai_platform_api-1.3.3661/ourskyai_platform_api/rest.py
+-rw-r--r--   0        0        0      751 2024-05-24 01:28:48.637416 ourskyai_platform_api-1.3.3661/pyproject.toml
+-rw-r--r--   0        0        0    10945 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3661/PKG-INFO
```

### Comparing `ourskyai_platform_api-1.3.3657/README.md` & `ourskyai_platform_api-1.3.3661/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-platform-api
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
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/__init__.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3657"
+__version__ = "1.3.3661"
 
 # import apis into sdk package
 from ourskyai_platform_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_platform_api.api_response import ApiResponse
 from ourskyai_platform_api.api_client import ApiClient
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/api/default_api.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/api_client.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
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

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/api_response.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/configuration.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
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

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/exceptions.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/__init__.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/camera_mode.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/camera_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/empty_success.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/empty_success.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/filter_type.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/filter_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/fits_header.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/fits_header.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/location.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/metric_type.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/metric_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/mount_type.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_file_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,24 +17,23 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class MountType(str, Enum):
+class V1FileType(str, Enum):
     """
-    MountType
+    V1FileType
     """
 
     """
     allowed enum values
     """
-    ALT_AZ = 'ALT_AZ'
-    EQUITORIAL = 'EQUITORIAL'
+    ZIP = 'ZIP'
 
     @classmethod
-    def from_json(cls, json_str: str) -> MountType:
-        """Create an instance of MountType from a JSON string"""
-        return MountType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1FileType:
+        """Create an instance of V1FileType from a JSON string"""
+        return V1FileType(json.loads(json_str))
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/node_state.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/node_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/optical_tube_type.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/optical_tube_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/plate_solve_parameters.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/plate_solve_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/shutter_type.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/shutter_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/successful_create.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/successful_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/tracking_type.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/tracking_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_auto_focus_instruction.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_auto_focus_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_camera.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_client_token.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_client_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_complete_observation_request.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_complete_observation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_image_set_image_request.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_image_set_image_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_image_set_image_response.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_image_set_image_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_image_set_request.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_image_set_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_mount_request.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_mount_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_node_diagnostic.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_node_diagnostic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_node_request.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_create_optical_tube_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_diagnostic_instruction.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_diagnostic_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_elevation_mask_point.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_elevation_mask_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_gain_curve.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_gain_curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_gain_curve_point.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_gain_curve_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_instruction_request.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_get_instruction_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_nodes.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_get_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_or_create_camera_request.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_get_or_create_camera_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_or_create_mount_request.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_get_or_create_mount_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_ground_station_participant.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_ground_station_participant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_image_set.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_image_set.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_image_set_image.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_image_set_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_instruction.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_metric.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_mount.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_mount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node_component_type.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_node_component_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node_controller_artifact.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_node_controller_artifact.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node_diagnostic_type.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_node_diagnostic_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node_with_location.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_node_with_location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_observation_instruction.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_observation_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_optical_tube.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_optical_tube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_read_noise_point.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_read_noise_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_release.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_release.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_setup_action.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_setup_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_slew_timing.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_slew_timing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_slew_timing_interval.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_slew_timing_interval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_components_request.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_update_node_components_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_components_request_camera.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_update_node_components_request_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_components_request_mount.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_update_node_components_request_mount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_request.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_update_node_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_video_mode_framerate_property.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v1_video_mode_framerate_property.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v2_complete_observation_request.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/models/v2_complete_observation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/rest.py` & `ourskyai_platform_api-1.3.3661/ourskyai_platform_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_platform_api-1.3.3657/pyproject.toml` & `ourskyai_platform_api-1.3.3661/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_platform_api"
-version = "1.3.3657"
+version = "1.3.3661"
 description = "OurSky Platform"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Platform"]
 include = ["ourskyai_platform_api/py.typed"]
```

### Comparing `ourskyai_platform_api-1.3.3657/PKG-INFO` & `ourskyai_platform_api-1.3.3661/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_platform_api
-Version: 1.3.3657
+Version: 1.3.3661
 Summary: OurSky Platform
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky Platform
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # ourskyai-platform-api
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
```

