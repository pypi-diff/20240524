# Comparing `tmp/ourskyai_platform_api-1.3.3654.tar.gz` & `tmp/ourskyai_platform_api-1.3.3657.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_platform_api-1.3.3654.tar", max compression
+gzip compressed data, was "ourskyai_platform_api-1.3.3657.tar", max compression
```

## Comparing `ourskyai_platform_api-1.3.3654.tar` & `ourskyai_platform_api-1.3.3657.tar`

### file list

```diff
@@ -1,76 +1,78 @@
--rw-r--r--   0        0        0     9661 2024-05-23 19:26:18.742591 ourskyai_platform_api-1.3.3654/README.md
--rw-r--r--   0        0        0     6336 2024-05-23 19:26:22.214258 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/__init__.py
--rw-r--r--   0        0        0      109 2024-05-23 19:26:22.238255 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/api/__init__.py
--rw-r--r--   0        0        0   199259 2024-05-23 19:26:22.338246 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/api/default_api.py
--rw-r--r--   0        0        0    30373 2024-05-23 19:26:22.390241 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-23 19:26:22.430237 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/api_response.py
--rw-r--r--   0        0        0    14693 2024-05-23 19:26:22.470233 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/configuration.py
--rw-r--r--   0        0        0     5436 2024-05-23 19:26:22.514229 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/exceptions.py
--rw-r--r--   0        0        0     5665 2024-05-23 19:26:22.558225 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/__init__.py
--rw-r--r--   0        0        0      745 2024-05-23 19:26:22.626218 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/camera_mode.py
--rw-r--r--   0        0        0     1907 2024-05-23 19:26:22.682213 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/empty_success.py
--rw-r--r--   0        0        0     1189 2024-05-23 19:26:22.726209 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/filter_type.py
--rw-r--r--   0        0        0     1933 2024-05-23 19:26:22.778203 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/fits_header.py
--rw-r--r--   0        0        0     2158 2024-05-23 19:26:22.814200 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/location.py
--rw-r--r--   0        0        0      777 2024-05-23 19:26:22.850196 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/metric_type.py
--rw-r--r--   0        0        0      750 2024-05-23 19:26:22.886193 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/mount_type.py
--rw-r--r--   0        0        0      890 2024-05-23 19:26:22.930189 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/node_state.py
--rw-r--r--   0        0        0      830 2024-05-23 19:26:22.974185 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/optical_tube_type.py
--rw-r--r--   0        0        0     2407 2024-05-23 19:26:23.034179 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/plate_solve_parameters.py
--rw-r--r--   0        0        0      754 2024-05-23 19:26:23.086174 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/shutter_type.py
--rw-r--r--   0        0        0     1895 2024-05-23 19:26:23.170166 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/successful_create.py
--rw-r--r--   0        0        0      771 2024-05-23 19:26:23.206162 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/tracking_type.py
--rw-r--r--   0        0        0     2622 2024-05-23 19:26:23.254158 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_auto_focus_instruction.py
--rw-r--r--   0        0        0     2366 2024-05-23 19:26:23.298153 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py
--rw-r--r--   0        0        0     4920 2024-05-23 19:26:23.342149 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_camera.py
--rw-r--r--   0        0        0     2115 2024-05-23 19:26:23.378146 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_client_token.py
--rw-r--r--   0        0        0     2047 2024-05-23 19:26:23.426141 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_complete_observation_request.py
--rw-r--r--   0        0        0     2047 2024-05-23 19:26:23.470137 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2118 2024-05-23 19:26:23.518132 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2692 2024-05-23 19:26:23.554129 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2302 2024-05-23 19:26:23.622122 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     2710 2024-05-23 19:26:23.670118 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_create_node_diagnostic.py
--rw-r--r--   0        0        0     2715 2024-05-23 19:26:23.742111 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
--rw-r--r--   0        0        0     3152 2024-05-23 19:26:23.806105 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2453 2024-05-23 19:26:23.842101 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2124 2024-05-23 19:26:23.922093 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_diagnostic_instruction.py
--rw-r--r--   0        0        0     2444 2024-05-23 19:26:23.998086 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0      719 2024-05-23 19:26:24.050081 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_file_type.py
--rw-r--r--   0        0        0     3298 2024-05-23 19:26:24.098077 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2054 2024-05-23 19:26:24.158071 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2570 2024-05-23 19:26:24.238063 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_get_instruction_request.py
--rw-r--r--   0        0        0     2370 2024-05-23 19:26:24.282059 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7081 2024-05-23 19:26:24.330054 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2330 2024-05-23 19:26:24.386049 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2519 2024-05-23 19:26:24.438044 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     2675 2024-05-23 19:26:24.490039 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
--rw-r--r--   0        0        0     3985 2024-05-23 19:26:24.534035 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_ground_station_participant.py
--rw-r--r--   0        0        0     3445 2024-05-23 19:26:24.602028 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5803 2024-05-23 19:26:24.646024 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0     3763 2024-05-23 19:26:24.694019 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_instruction.py
--rw-r--r--   0        0        0     2400 2024-05-23 19:26:24.758013 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_metric.py
--rw-r--r--   0        0        0     1917 2024-05-23 19:26:24.806008 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_mount.py
--rw-r--r--   0        0        0     4470 2024-05-23 19:26:24.854004 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_node.py
--rw-r--r--   0        0        0      850 2024-05-23 19:26:24.909999 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_node_component_type.py
--rw-r--r--   0        0        0     1669 2024-05-23 19:26:24.953994 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_node_diagnostic_type.py
--rw-r--r--   0        0        0     2573 2024-05-23 19:26:25.021988 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     5537 2024-05-23 19:26:25.073983 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_observation_instruction.py
--rw-r--r--   0        0        0     2242 2024-05-23 19:26:25.141976 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     2135 2024-05-23 19:26:25.189972 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
--rw-r--r--   0        0        0     2648 2024-05-23 19:26:25.229968 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
--rw-r--r--   0        0        0     2054 2024-05-23 19:26:25.269964 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2401 2024-05-23 19:26:25.325959 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_release.py
--rw-r--r--   0        0        0     2053 2024-05-23 19:26:25.385953 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2946 2024-05-23 19:26:25.437948 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2243 2024-05-23 19:26:25.485943 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     3601 2024-05-23 19:26:25.533939 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_update_node_components_request.py
--rw-r--r--   0        0        0     6269 2024-05-23 19:26:25.589933 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
--rw-r--r--   0        0        0     2402 2024-05-23 19:26:25.693923 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
--rw-r--r--   0        0        0     2591 2024-05-23 19:26:25.761917 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
--rw-r--r--   0        0        0     4620 2024-05-23 19:26:25.817911 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2525 2024-05-23 19:26:25.865907 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0     2224 2024-05-23 19:26:25.925901 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v2_complete_observation_request.py
--rw-r--r--   0        0        0        0 2024-05-23 19:26:25.957898 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/py.typed
--rw-r--r--   0        0        0    12941 2024-05-23 19:26:25.997894 ourskyai_platform_api-1.3.3654/ourskyai_platform_api/rest.py
--rw-r--r--   0        0        0      751 2024-05-23 19:26:26.045889 ourskyai_platform_api-1.3.3654/pyproject.toml
--rw-r--r--   0        0        0    10638 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3654/PKG-INFO
+-rw-r--r--   0        0        0     9968 2024-05-23 23:15:12.461309 ourskyai_platform_api-1.3.3657/README.md
+-rw-r--r--   0        0        0     6552 2024-05-23 23:15:16.024686 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/__init__.py
+-rw-r--r--   0        0        0      109 2024-05-23 23:15:16.056680 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/api/__init__.py
+-rw-r--r--   0        0        0   206365 2024-05-23 23:15:16.132667 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/api/default_api.py
+-rw-r--r--   0        0        0    30373 2024-05-23 23:15:16.180659 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-23 23:15:16.232649 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/api_response.py
+-rw-r--r--   0        0        0    14693 2024-05-23 23:15:16.276642 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/configuration.py
+-rw-r--r--   0        0        0     5436 2024-05-23 23:15:16.320634 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/exceptions.py
+-rw-r--r--   0        0        0     5881 2024-05-23 23:15:16.360627 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-23 23:15:16.428615 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/camera_mode.py
+-rw-r--r--   0        0        0     1907 2024-05-23 23:15:16.540596 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/empty_success.py
+-rw-r--r--   0        0        0     1189 2024-05-23 23:15:16.572590 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/filter_type.py
+-rw-r--r--   0        0        0     1933 2024-05-23 23:15:16.624581 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/fits_header.py
+-rw-r--r--   0        0        0     2158 2024-05-23 23:15:16.708566 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/location.py
+-rw-r--r--   0        0        0      777 2024-05-23 23:15:16.780554 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/metric_type.py
+-rw-r--r--   0        0        0      750 2024-05-23 23:15:16.856541 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/mount_type.py
+-rw-r--r--   0        0        0      890 2024-05-23 23:15:16.908531 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/node_state.py
+-rw-r--r--   0        0        0      830 2024-05-23 23:15:16.952524 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0     2407 2024-05-23 23:15:17.032510 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/plate_solve_parameters.py
+-rw-r--r--   0        0        0      754 2024-05-23 23:15:17.080501 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1895 2024-05-23 23:15:17.120494 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/successful_create.py
+-rw-r--r--   0        0        0      771 2024-05-23 23:15:17.168486 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/tracking_type.py
+-rw-r--r--   0        0        0     2622 2024-05-23 23:15:17.204480 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_auto_focus_instruction.py
+-rw-r--r--   0        0        0     2366 2024-05-23 23:15:17.248472 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py
+-rw-r--r--   0        0        0     4920 2024-05-23 23:15:17.288465 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2115 2024-05-23 23:15:17.388447 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_client_token.py
+-rw-r--r--   0        0        0     2047 2024-05-23 23:15:17.424441 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_complete_observation_request.py
+-rw-r--r--   0        0        0     2047 2024-05-23 23:15:17.476432 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2118 2024-05-23 23:15:17.512426 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2692 2024-05-23 23:15:17.560417 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2302 2024-05-23 23:15:17.604410 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     2071 2024-05-23 23:15:17.664399 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py
+-rw-r--r--   0        0        0     2710 2024-05-23 23:15:17.728388 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_node_diagnostic.py
+-rw-r--r--   0        0        0     2715 2024-05-23 23:15:17.788378 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
+-rw-r--r--   0        0        0     3152 2024-05-23 23:15:17.828371 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2453 2024-05-23 23:15:17.860365 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2124 2024-05-23 23:15:17.924354 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_diagnostic_instruction.py
+-rw-r--r--   0        0        0     2444 2024-05-23 23:15:17.968346 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0      719 2024-05-23 23:15:18.036334 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_file_type.py
+-rw-r--r--   0        0        0     3298 2024-05-23 23:15:18.116320 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2054 2024-05-23 23:15:18.148315 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2570 2024-05-23 23:15:18.204305 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_instruction_request.py
+-rw-r--r--   0        0        0     2370 2024-05-23 23:15:18.248297 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7081 2024-05-23 23:15:18.296289 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2330 2024-05-23 23:15:18.344280 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2519 2024-05-23 23:15:18.396271 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2675 2024-05-23 23:15:18.456261 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
+-rw-r--r--   0        0        0     3985 2024-05-23 23:15:18.540246 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_ground_station_participant.py
+-rw-r--r--   0        0        0     3445 2024-05-23 23:15:18.604235 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5803 2024-05-23 23:15:18.644228 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0     3763 2024-05-23 23:15:18.676222 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_instruction.py
+-rw-r--r--   0        0        0     2400 2024-05-23 23:15:18.724214 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_metric.py
+-rw-r--r--   0        0        0     1917 2024-05-23 23:15:18.800201 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4470 2024-05-23 23:15:18.848192 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node.py
+-rw-r--r--   0        0        0      850 2024-05-23 23:15:18.880187 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node_component_type.py
+-rw-r--r--   0        0        0     1963 2024-05-23 23:15:18.924179 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node_controller_artifact.py
+-rw-r--r--   0        0        0     1669 2024-05-23 23:15:18.972171 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node_diagnostic_type.py
+-rw-r--r--   0        0        0     2573 2024-05-23 23:15:19.020162 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     5537 2024-05-23 23:15:19.076152 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_observation_instruction.py
+-rw-r--r--   0        0        0     2242 2024-05-23 23:15:19.152139 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     2135 2024-05-23 23:15:19.200131 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
+-rw-r--r--   0        0        0     2648 2024-05-23 23:15:19.240124 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
+-rw-r--r--   0        0        0     2054 2024-05-23 23:15:19.288115 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2401 2024-05-23 23:15:19.352104 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_release.py
+-rw-r--r--   0        0        0     2053 2024-05-23 23:15:19.400096 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2946 2024-05-23 23:15:19.444088 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2243 2024-05-23 23:15:19.516075 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     3601 2024-05-23 23:15:19.568066 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_components_request.py
+-rw-r--r--   0        0        0     6269 2024-05-23 23:15:19.612059 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
+-rw-r--r--   0        0        0     2402 2024-05-23 23:15:19.656051 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
+-rw-r--r--   0        0        0     2591 2024-05-23 23:15:19.708042 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
+-rw-r--r--   0        0        0     4620 2024-05-23 23:15:19.760033 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2525 2024-05-23 23:15:19.812024 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0     2224 2024-05-23 23:15:19.872013 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v2_complete_observation_request.py
+-rw-r--r--   0        0        0        0 2024-05-23 23:15:19.904008 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/py.typed
+-rw-r--r--   0        0        0    12941 2024-05-23 23:15:19.955999 ourskyai_platform_api-1.3.3657/ourskyai_platform_api/rest.py
+-rw-r--r--   0        0        0      751 2024-05-23 23:15:19.995992 ourskyai_platform_api-1.3.3657/pyproject.toml
+-rw-r--r--   0        0        0    10945 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3657/PKG-INFO
```

### Comparing `ourskyai_platform_api-1.3.3654/README.md` & `ourskyai_platform_api-1.3.3657/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-platform-api
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
@@ -85,14 +85,15 @@
 *DefaultApi* | [**v1_camera_match**](docs/DefaultApi.md#v1_camera_match) | **GET** /v1/camera-match | 
 *DefaultApi* | [**v1_complete_observation**](docs/DefaultApi.md#v1_complete_observation) | **PUT** /v1/observation-complete | 
 *DefaultApi* | [**v1_create_image_set**](docs/DefaultApi.md#v1_create_image_set) | **POST** /v1/image-set | 
 *DefaultApi* | [**v1_create_image_set_image**](docs/DefaultApi.md#v1_create_image_set_image) | **POST** /v1/image-set-image | 
 *DefaultApi* | [**v1_create_metrics**](docs/DefaultApi.md#v1_create_metrics) | **POST** /v1/metrics | 
 *DefaultApi* | [**v1_create_mount**](docs/DefaultApi.md#v1_create_mount) | **POST** /v1/mount | 
 *DefaultApi* | [**v1_create_node**](docs/DefaultApi.md#v1_create_node) | **POST** /v1/node | 
+*DefaultApi* | [**v1_create_node_controller_artifact**](docs/DefaultApi.md#v1_create_node_controller_artifact) | **PUT** /v1/node-controller-artifact | 
 *DefaultApi* | [**v1_create_node_diagnostics**](docs/DefaultApi.md#v1_create_node_diagnostics) | **POST** /v1/node-diagnostics | 
 *DefaultApi* | [**v1_create_optical_tube**](docs/DefaultApi.md#v1_create_optical_tube) | **POST** /v1/optical-tube | 
 *DefaultApi* | [**v1_delete_image_set**](docs/DefaultApi.md#v1_delete_image_set) | **DELETE** /v1/image-set | 
 *DefaultApi* | [**v1_delete_image_set_image**](docs/DefaultApi.md#v1_delete_image_set_image) | **DELETE** /v1/image-set-image | 
 *DefaultApi* | [**v1_get_cameras**](docs/DefaultApi.md#v1_get_cameras) | **GET** /v1/cameras | 
 *DefaultApi* | [**v1_get_image_set**](docs/DefaultApi.md#v1_get_image_set) | **GET** /v1/image-set | 
 *DefaultApi* | [**v1_get_image_set_image**](docs/DefaultApi.md#v1_get_image_set_image) | **GET** /v1/image-set-image | 
@@ -134,14 +135,15 @@
  - [V1Camera](docs/V1Camera.md)
  - [V1ClientToken](docs/V1ClientToken.md)
  - [V1CompleteObservationRequest](docs/V1CompleteObservationRequest.md)
  - [V1CreateImageSetImageRequest](docs/V1CreateImageSetImageRequest.md)
  - [V1CreateImageSetImageResponse](docs/V1CreateImageSetImageResponse.md)
  - [V1CreateImageSetRequest](docs/V1CreateImageSetRequest.md)
  - [V1CreateMountRequest](docs/V1CreateMountRequest.md)
+ - [V1CreateNodeControllerArtifactRequest](docs/V1CreateNodeControllerArtifactRequest.md)
  - [V1CreateNodeDiagnostic](docs/V1CreateNodeDiagnostic.md)
  - [V1CreateNodeDiagnosticsRequest](docs/V1CreateNodeDiagnosticsRequest.md)
  - [V1CreateNodeRequest](docs/V1CreateNodeRequest.md)
  - [V1CreateOpticalTubeRequest](docs/V1CreateOpticalTubeRequest.md)
  - [V1DiagnosticInstruction](docs/V1DiagnosticInstruction.md)
  - [V1ElevationMaskPoint](docs/V1ElevationMaskPoint.md)
  - [V1FileType](docs/V1FileType.md)
@@ -157,14 +159,15 @@
  - [V1ImageSet](docs/V1ImageSet.md)
  - [V1ImageSetImage](docs/V1ImageSetImage.md)
  - [V1Instruction](docs/V1Instruction.md)
  - [V1Metric](docs/V1Metric.md)
  - [V1Mount](docs/V1Mount.md)
  - [V1Node](docs/V1Node.md)
  - [V1NodeComponentType](docs/V1NodeComponentType.md)
+ - [V1NodeControllerArtifact](docs/V1NodeControllerArtifact.md)
  - [V1NodeDiagnosticType](docs/V1NodeDiagnosticType.md)
  - [V1NodeWithLocation](docs/V1NodeWithLocation.md)
  - [V1ObservationInstruction](docs/V1ObservationInstruction.md)
  - [V1OpticalTube](docs/V1OpticalTube.md)
  - [V1PlateSolveCatalogFile](docs/V1PlateSolveCatalogFile.md)
  - [V1PlateSolveCatalogFileDownload](docs/V1PlateSolveCatalogFileDownload.md)
  - [V1ReadNoisePoint](docs/V1ReadNoisePoint.md)
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/__init__.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3654"
+__version__ = "1.3.3657"
 
 # import apis into sdk package
 from ourskyai_platform_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_platform_api.api_response import ApiResponse
 from ourskyai_platform_api.api_client import ApiClient
@@ -49,14 +49,15 @@
 from ourskyai_platform_api.models.v1_camera import V1Camera
 from ourskyai_platform_api.models.v1_client_token import V1ClientToken
 from ourskyai_platform_api.models.v1_complete_observation_request import V1CompleteObservationRequest
 from ourskyai_platform_api.models.v1_create_image_set_image_request import V1CreateImageSetImageRequest
 from ourskyai_platform_api.models.v1_create_image_set_image_response import V1CreateImageSetImageResponse
 from ourskyai_platform_api.models.v1_create_image_set_request import V1CreateImageSetRequest
 from ourskyai_platform_api.models.v1_create_mount_request import V1CreateMountRequest
+from ourskyai_platform_api.models.v1_create_node_controller_artifact_request import V1CreateNodeControllerArtifactRequest
 from ourskyai_platform_api.models.v1_create_node_diagnostic import V1CreateNodeDiagnostic
 from ourskyai_platform_api.models.v1_create_node_diagnostics_request import V1CreateNodeDiagnosticsRequest
 from ourskyai_platform_api.models.v1_create_node_request import V1CreateNodeRequest
 from ourskyai_platform_api.models.v1_create_optical_tube_request import V1CreateOpticalTubeRequest
 from ourskyai_platform_api.models.v1_diagnostic_instruction import V1DiagnosticInstruction
 from ourskyai_platform_api.models.v1_elevation_mask_point import V1ElevationMaskPoint
 from ourskyai_platform_api.models.v1_file_type import V1FileType
@@ -72,14 +73,15 @@
 from ourskyai_platform_api.models.v1_image_set import V1ImageSet
 from ourskyai_platform_api.models.v1_image_set_image import V1ImageSetImage
 from ourskyai_platform_api.models.v1_instruction import V1Instruction
 from ourskyai_platform_api.models.v1_metric import V1Metric
 from ourskyai_platform_api.models.v1_mount import V1Mount
 from ourskyai_platform_api.models.v1_node import V1Node
 from ourskyai_platform_api.models.v1_node_component_type import V1NodeComponentType
+from ourskyai_platform_api.models.v1_node_controller_artifact import V1NodeControllerArtifact
 from ourskyai_platform_api.models.v1_node_diagnostic_type import V1NodeDiagnosticType
 from ourskyai_platform_api.models.v1_node_with_location import V1NodeWithLocation
 from ourskyai_platform_api.models.v1_observation_instruction import V1ObservationInstruction
 from ourskyai_platform_api.models.v1_optical_tube import V1OpticalTube
 from ourskyai_platform_api.models.v1_plate_solve_catalog_file import V1PlateSolveCatalogFile
 from ourskyai_platform_api.models.v1_plate_solve_catalog_file_download import V1PlateSolveCatalogFileDownload
 from ourskyai_platform_api.models.v1_read_noise_point import V1ReadNoisePoint
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/api/default_api.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
@@ -28,14 +28,15 @@
 from ourskyai_platform_api.models.v1_camera import V1Camera
 from ourskyai_platform_api.models.v1_client_token import V1ClientToken
 from ourskyai_platform_api.models.v1_complete_observation_request import V1CompleteObservationRequest
 from ourskyai_platform_api.models.v1_create_image_set_image_request import V1CreateImageSetImageRequest
 from ourskyai_platform_api.models.v1_create_image_set_image_response import V1CreateImageSetImageResponse
 from ourskyai_platform_api.models.v1_create_image_set_request import V1CreateImageSetRequest
 from ourskyai_platform_api.models.v1_create_mount_request import V1CreateMountRequest
+from ourskyai_platform_api.models.v1_create_node_controller_artifact_request import V1CreateNodeControllerArtifactRequest
 from ourskyai_platform_api.models.v1_create_node_diagnostics_request import V1CreateNodeDiagnosticsRequest
 from ourskyai_platform_api.models.v1_create_node_request import V1CreateNodeRequest
 from ourskyai_platform_api.models.v1_create_optical_tube_request import V1CreateOpticalTubeRequest
 from ourskyai_platform_api.models.v1_get_instruction_request import V1GetInstructionRequest
 from ourskyai_platform_api.models.v1_get_nodes import V1GetNodes
 from ourskyai_platform_api.models.v1_get_or_create_camera_request import V1GetOrCreateCameraRequest
 from ourskyai_platform_api.models.v1_get_or_create_mount_request import V1GetOrCreateMountRequest
@@ -44,14 +45,15 @@
 from ourskyai_platform_api.models.v1_ground_station_participant import V1GroundStationParticipant
 from ourskyai_platform_api.models.v1_image_set import V1ImageSet
 from ourskyai_platform_api.models.v1_image_set_image import V1ImageSetImage
 from ourskyai_platform_api.models.v1_instruction import V1Instruction
 from ourskyai_platform_api.models.v1_metric import V1Metric
 from ourskyai_platform_api.models.v1_mount import V1Mount
 from ourskyai_platform_api.models.v1_node import V1Node
+from ourskyai_platform_api.models.v1_node_controller_artifact import V1NodeControllerArtifact
 from ourskyai_platform_api.models.v1_node_diagnostic_type import V1NodeDiagnosticType
 from ourskyai_platform_api.models.v1_optical_tube import V1OpticalTube
 from ourskyai_platform_api.models.v1_plate_solve_catalog_file_download import V1PlateSolveCatalogFileDownload
 from ourskyai_platform_api.models.v1_release import V1Release
 from ourskyai_platform_api.models.v1_update_node_components_request import V1UpdateNodeComponentsRequest
 from ourskyai_platform_api.models.v1_update_node_request import V1UpdateNodeRequest
 from ourskyai_platform_api.models.v2_complete_observation_request import V2CompleteObservationRequest
@@ -1274,14 +1276,161 @@
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
+    def v1_create_node_controller_artifact(self, v1_create_node_controller_artifact_request : V1CreateNodeControllerArtifactRequest, **kwargs) -> V1NodeControllerArtifact:  # noqa: E501
+        """v1_create_node_controller_artifact  # noqa: E501
+
+        Create a node controller artifact.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_create_node_controller_artifact(v1_create_node_controller_artifact_request, async_req=True)
+        >>> result = thread.get()
+
+        :param v1_create_node_controller_artifact_request: (required)
+        :type v1_create_node_controller_artifact_request: V1CreateNodeControllerArtifactRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: V1NodeControllerArtifact
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the v1_create_node_controller_artifact_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+        return self.v1_create_node_controller_artifact_with_http_info(v1_create_node_controller_artifact_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def v1_create_node_controller_artifact_with_http_info(self, v1_create_node_controller_artifact_request : V1CreateNodeControllerArtifactRequest, **kwargs) -> ApiResponse:  # noqa: E501
+        """v1_create_node_controller_artifact  # noqa: E501
+
+        Create a node controller artifact.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_create_node_controller_artifact_with_http_info(v1_create_node_controller_artifact_request, async_req=True)
+        >>> result = thread.get()
+
+        :param v1_create_node_controller_artifact_request: (required)
+        :type v1_create_node_controller_artifact_request: V1CreateNodeControllerArtifactRequest
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
+        :rtype: tuple(V1NodeControllerArtifact, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'v1_create_node_controller_artifact_request'
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
+                    " to method v1_create_node_controller_artifact" % _key
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
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        if _params['v1_create_node_controller_artifact_request'] is not None:
+            _body_params = _params['v1_create_node_controller_artifact_request']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['Roles', 'BearerToken']  # noqa: E501
+
+        _response_types_map = {
+            '200': "V1NodeControllerArtifact",
+        }
+
+        return self.api_client.call_api(
+            '/v1/node-controller-artifact', 'PUT',
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

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/api_client.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
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

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/api_response.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/configuration.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
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

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/exceptions.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/__init__.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
@@ -32,14 +32,15 @@
 from ourskyai_platform_api.models.v1_camera import V1Camera
 from ourskyai_platform_api.models.v1_client_token import V1ClientToken
 from ourskyai_platform_api.models.v1_complete_observation_request import V1CompleteObservationRequest
 from ourskyai_platform_api.models.v1_create_image_set_image_request import V1CreateImageSetImageRequest
 from ourskyai_platform_api.models.v1_create_image_set_image_response import V1CreateImageSetImageResponse
 from ourskyai_platform_api.models.v1_create_image_set_request import V1CreateImageSetRequest
 from ourskyai_platform_api.models.v1_create_mount_request import V1CreateMountRequest
+from ourskyai_platform_api.models.v1_create_node_controller_artifact_request import V1CreateNodeControllerArtifactRequest
 from ourskyai_platform_api.models.v1_create_node_diagnostic import V1CreateNodeDiagnostic
 from ourskyai_platform_api.models.v1_create_node_diagnostics_request import V1CreateNodeDiagnosticsRequest
 from ourskyai_platform_api.models.v1_create_node_request import V1CreateNodeRequest
 from ourskyai_platform_api.models.v1_create_optical_tube_request import V1CreateOpticalTubeRequest
 from ourskyai_platform_api.models.v1_diagnostic_instruction import V1DiagnosticInstruction
 from ourskyai_platform_api.models.v1_elevation_mask_point import V1ElevationMaskPoint
 from ourskyai_platform_api.models.v1_file_type import V1FileType
@@ -55,14 +56,15 @@
 from ourskyai_platform_api.models.v1_image_set import V1ImageSet
 from ourskyai_platform_api.models.v1_image_set_image import V1ImageSetImage
 from ourskyai_platform_api.models.v1_instruction import V1Instruction
 from ourskyai_platform_api.models.v1_metric import V1Metric
 from ourskyai_platform_api.models.v1_mount import V1Mount
 from ourskyai_platform_api.models.v1_node import V1Node
 from ourskyai_platform_api.models.v1_node_component_type import V1NodeComponentType
+from ourskyai_platform_api.models.v1_node_controller_artifact import V1NodeControllerArtifact
 from ourskyai_platform_api.models.v1_node_diagnostic_type import V1NodeDiagnosticType
 from ourskyai_platform_api.models.v1_node_with_location import V1NodeWithLocation
 from ourskyai_platform_api.models.v1_observation_instruction import V1ObservationInstruction
 from ourskyai_platform_api.models.v1_optical_tube import V1OpticalTube
 from ourskyai_platform_api.models.v1_plate_solve_catalog_file import V1PlateSolveCatalogFile
 from ourskyai_platform_api.models.v1_plate_solve_catalog_file_download import V1PlateSolveCatalogFileDownload
 from ourskyai_platform_api.models.v1_read_noise_point import V1ReadNoisePoint
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/camera_mode.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/camera_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/empty_success.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/empty_success.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/filter_type.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/filter_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/fits_header.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/fits_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/location.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/metric_type.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/metric_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/mount_type.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/shutter_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,24 +17,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class MountType(str, Enum):
+class ShutterType(str, Enum):
     """
-    MountType
+    ShutterType
     """
 
     """
     allowed enum values
     """
-    ALT_AZ = 'ALT_AZ'
-    EQUITORIAL = 'EQUITORIAL'
+    ROLLING = 'ROLLING'
+    GLOBAL = 'GLOBAL'
 
     @classmethod
-    def from_json(cls, json_str: str) -> MountType:
-        """Create an instance of MountType from a JSON string"""
-        return MountType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> ShutterType:
+        """Create an instance of ShutterType from a JSON string"""
+        return ShutterType(json.loads(json_str))
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/node_state.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/node_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/optical_tube_type.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/optical_tube_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/plate_solve_parameters.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/plate_solve_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/shutter_type.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_file_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,24 +17,23 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class ShutterType(str, Enum):
+class V1FileType(str, Enum):
     """
-    ShutterType
+    V1FileType
     """
 
     """
     allowed enum values
     """
-    ROLLING = 'ROLLING'
-    GLOBAL = 'GLOBAL'
+    ZIP = 'ZIP'
 
     @classmethod
-    def from_json(cls, json_str: str) -> ShutterType:
-        """Create an instance of ShutterType from a JSON string"""
-        return ShutterType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1FileType:
+        """Create an instance of V1FileType from a JSON string"""
+        return V1FileType(json.loads(json_str))
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/successful_create.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/successful_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/tracking_type.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/tracking_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_auto_focus_instruction.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_auto_focus_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_camera.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_client_token.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_client_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_complete_observation_request.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_complete_observation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_create_image_set_image_request.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_image_set_image_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_create_image_set_image_response.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_image_set_image_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_create_image_set_request.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_image_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_create_mount_request.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_mount_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_create_node_diagnostic.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_node_diagnostic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_create_node_request.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_create_optical_tube_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_diagnostic_instruction.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_diagnostic_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_elevation_mask_point.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_elevation_mask_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_file_type.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/mount_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,23 +17,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1FileType(str, Enum):
+class MountType(str, Enum):
     """
-    V1FileType
+    MountType
     """
 
     """
     allowed enum values
     """
-    ZIP = 'ZIP'
+    ALT_AZ = 'ALT_AZ'
+    EQUITORIAL = 'EQUITORIAL'
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1FileType:
-        """Create an instance of V1FileType from a JSON string"""
-        return V1FileType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> MountType:
+        """Create an instance of MountType from a JSON string"""
+        return MountType(json.loads(json_str))
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_gain_curve.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_gain_curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_gain_curve_point.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_gain_curve_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_get_instruction_request.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_instruction_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_get_nodes.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_get_or_create_camera_request.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_or_create_camera_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_get_or_create_mount_request.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_or_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_ground_station_participant.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_ground_station_participant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_image_set.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_image_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_image_set_image.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_image_set_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_instruction.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_metric.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_mount.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_mount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_node.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_node_component_type.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node_component_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_node_diagnostic_type.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node_diagnostic_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_node_with_location.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_node_with_location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_observation_instruction.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_observation_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_optical_tube.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_optical_tube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_read_noise_point.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_read_noise_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_release.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_release.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_setup_action.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_setup_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_slew_timing.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_slew_timing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_slew_timing_interval.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_slew_timing_interval.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_update_node_components_request.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_components_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_update_node_components_request_camera.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_components_request_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_update_node_components_request_mount.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_components_request_mount.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_update_node_request.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_update_node_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v1_video_mode_framerate_property.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v1_video_mode_framerate_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/models/v2_complete_observation_request.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/models/v2_complete_observation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3654/ourskyai_platform_api/rest.py` & `ourskyai_platform_api-1.3.3657/ourskyai_platform_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_platform_api-1.3.3654/pyproject.toml` & `ourskyai_platform_api-1.3.3657/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_platform_api"
-version = "1.3.3654"
+version = "1.3.3657"
 description = "OurSky Platform"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Platform"]
 include = ["ourskyai_platform_api/py.typed"]
```

### Comparing `ourskyai_platform_api-1.3.3654/PKG-INFO` & `ourskyai_platform_api-1.3.3657/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_platform_api
-Version: 1.3.3654
+Version: 1.3.3657
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
 
-- API version: 1.3.3654
-- Package version: 1.3.3654
+- API version: 1.3.3657
+- Package version: 1.3.3657
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -110,14 +110,15 @@
 *DefaultApi* | [**v1_camera_match**](docs/DefaultApi.md#v1_camera_match) | **GET** /v1/camera-match | 
 *DefaultApi* | [**v1_complete_observation**](docs/DefaultApi.md#v1_complete_observation) | **PUT** /v1/observation-complete | 
 *DefaultApi* | [**v1_create_image_set**](docs/DefaultApi.md#v1_create_image_set) | **POST** /v1/image-set | 
 *DefaultApi* | [**v1_create_image_set_image**](docs/DefaultApi.md#v1_create_image_set_image) | **POST** /v1/image-set-image | 
 *DefaultApi* | [**v1_create_metrics**](docs/DefaultApi.md#v1_create_metrics) | **POST** /v1/metrics | 
 *DefaultApi* | [**v1_create_mount**](docs/DefaultApi.md#v1_create_mount) | **POST** /v1/mount | 
 *DefaultApi* | [**v1_create_node**](docs/DefaultApi.md#v1_create_node) | **POST** /v1/node | 
+*DefaultApi* | [**v1_create_node_controller_artifact**](docs/DefaultApi.md#v1_create_node_controller_artifact) | **PUT** /v1/node-controller-artifact | 
 *DefaultApi* | [**v1_create_node_diagnostics**](docs/DefaultApi.md#v1_create_node_diagnostics) | **POST** /v1/node-diagnostics | 
 *DefaultApi* | [**v1_create_optical_tube**](docs/DefaultApi.md#v1_create_optical_tube) | **POST** /v1/optical-tube | 
 *DefaultApi* | [**v1_delete_image_set**](docs/DefaultApi.md#v1_delete_image_set) | **DELETE** /v1/image-set | 
 *DefaultApi* | [**v1_delete_image_set_image**](docs/DefaultApi.md#v1_delete_image_set_image) | **DELETE** /v1/image-set-image | 
 *DefaultApi* | [**v1_get_cameras**](docs/DefaultApi.md#v1_get_cameras) | **GET** /v1/cameras | 
 *DefaultApi* | [**v1_get_image_set**](docs/DefaultApi.md#v1_get_image_set) | **GET** /v1/image-set | 
 *DefaultApi* | [**v1_get_image_set_image**](docs/DefaultApi.md#v1_get_image_set_image) | **GET** /v1/image-set-image | 
@@ -159,14 +160,15 @@
  - [V1Camera](docs/V1Camera.md)
  - [V1ClientToken](docs/V1ClientToken.md)
  - [V1CompleteObservationRequest](docs/V1CompleteObservationRequest.md)
  - [V1CreateImageSetImageRequest](docs/V1CreateImageSetImageRequest.md)
  - [V1CreateImageSetImageResponse](docs/V1CreateImageSetImageResponse.md)
  - [V1CreateImageSetRequest](docs/V1CreateImageSetRequest.md)
  - [V1CreateMountRequest](docs/V1CreateMountRequest.md)
+ - [V1CreateNodeControllerArtifactRequest](docs/V1CreateNodeControllerArtifactRequest.md)
  - [V1CreateNodeDiagnostic](docs/V1CreateNodeDiagnostic.md)
  - [V1CreateNodeDiagnosticsRequest](docs/V1CreateNodeDiagnosticsRequest.md)
  - [V1CreateNodeRequest](docs/V1CreateNodeRequest.md)
  - [V1CreateOpticalTubeRequest](docs/V1CreateOpticalTubeRequest.md)
  - [V1DiagnosticInstruction](docs/V1DiagnosticInstruction.md)
  - [V1ElevationMaskPoint](docs/V1ElevationMaskPoint.md)
  - [V1FileType](docs/V1FileType.md)
@@ -182,14 +184,15 @@
  - [V1ImageSet](docs/V1ImageSet.md)
  - [V1ImageSetImage](docs/V1ImageSetImage.md)
  - [V1Instruction](docs/V1Instruction.md)
  - [V1Metric](docs/V1Metric.md)
  - [V1Mount](docs/V1Mount.md)
  - [V1Node](docs/V1Node.md)
  - [V1NodeComponentType](docs/V1NodeComponentType.md)
+ - [V1NodeControllerArtifact](docs/V1NodeControllerArtifact.md)
  - [V1NodeDiagnosticType](docs/V1NodeDiagnosticType.md)
  - [V1NodeWithLocation](docs/V1NodeWithLocation.md)
  - [V1ObservationInstruction](docs/V1ObservationInstruction.md)
  - [V1OpticalTube](docs/V1OpticalTube.md)
  - [V1PlateSolveCatalogFile](docs/V1PlateSolveCatalogFile.md)
  - [V1PlateSolveCatalogFileDownload](docs/V1PlateSolveCatalogFileDownload.md)
  - [V1ReadNoisePoint](docs/V1ReadNoisePoint.md)
```

