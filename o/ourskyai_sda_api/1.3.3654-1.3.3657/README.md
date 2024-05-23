# Comparing `tmp/ourskyai_sda_api-1.3.3654.tar.gz` & `tmp/ourskyai_sda_api-1.3.3657.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_sda_api-1.3.3654.tar", max compression
+gzip compressed data, was "ourskyai_sda_api-1.3.3657.tar", max compression
```

## Comparing `ourskyai_sda_api-1.3.3654.tar` & `ourskyai_sda_api-1.3.3657.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    10151 2024-05-23 19:26:18.742591 ourskyai_sda_api-1.3.3654/README.md
--rw-r--r--   0        0        0     5222 2024-05-23 19:26:21.398336 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/__init__.py
--rw-r--r--   0        0        0      104 2024-05-23 19:26:21.430333 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/api/__init__.py
--rw-r--r--   0        0        0   220784 2024-05-23 19:26:21.522324 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/api/default_api.py
--rw-r--r--   0        0        0    30830 2024-05-23 19:26:21.570320 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-23 19:26:21.626314 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/api_response.py
--rw-r--r--   0        0        0    15175 2024-05-23 19:26:21.670310 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/configuration.py
--rw-r--r--   0        0        0     5923 2024-05-23 19:26:21.738303 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/exceptions.py
--rw-r--r--   0        0        0     4601 2024-05-23 19:26:21.786299 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/__init__.py
--rw-r--r--   0        0        0     4311 2024-05-23 19:26:21.830294 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/astrometric_offsets.py
--rw-r--r--   0        0        0     2394 2024-05-23 19:26:21.882290 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/empty_success.py
--rw-r--r--   0        0        0     1676 2024-05-23 19:26:21.938284 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/filter_type.py
--rw-r--r--   0        0        0     2420 2024-05-23 19:26:21.990279 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/fits_header.py
--rw-r--r--   0        0        0     2645 2024-05-23 19:26:22.058273 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/location.py
--rw-r--r--   0        0        0     1237 2024-05-23 19:26:22.138265 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/mount_type.py
--rw-r--r--   0        0        0     2756 2024-05-23 19:26:22.170262 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/observation_bounding_box.py
--rw-r--r--   0        0        0     3713 2024-05-23 19:26:22.226256 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/observation_quality.py
--rw-r--r--   0        0        0     6381 2024-05-23 19:26:22.278252 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/observation_result.py
--rw-r--r--   0        0        0     1320 2024-05-23 19:26:22.334246 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/observation_state.py
--rw-r--r--   0        0        0     1529 2024-05-23 19:26:22.390241 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/orbit_type.py
--rw-r--r--   0        0        0     1361 2024-05-23 19:26:22.434236 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/satellite_target_tracking_status.py
--rw-r--r--   0        0        0     1241 2024-05-23 19:26:22.486231 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/shutter_type.py
--rw-r--r--   0        0        0     2382 2024-05-23 19:26:22.530227 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/successful_create.py
--rw-r--r--   0        0        0     1258 2024-05-23 19:26:22.606220 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/tracking_type.py
--rw-r--r--   0        0        0     2534 2024-05-23 19:26:22.678213 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2605 2024-05-23 19:26:22.726209 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     3169 2024-05-23 19:26:22.806201 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2609 2024-05-23 19:26:22.854196 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_create_organization_target_request.py
--rw-r--r--   0        0        0     2761 2024-05-23 19:26:22.898192 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_create_satellite_target_request.py
--rw-r--r--   0        0        0     3373 2024-05-23 19:26:22.946187 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_create_search_instruction_request.py
--rw-r--r--   0        0        0     3353 2024-05-23 19:26:22.998182 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_create_survey_instruction_request.py
--rw-r--r--   0        0        0     3017 2024-05-23 19:26:23.054177 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_get_satellite_targets_response.py
--rw-r--r--   0        0        0     4457 2024-05-23 19:26:23.106172 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_ground_station_participant.py
--rw-r--r--   0        0        0     3922 2024-05-23 19:26:23.162166 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_image_set.py
--rw-r--r--   0        0        0     6285 2024-05-23 19:26:23.222161 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0     4676 2024-05-23 19:26:23.274156 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_observation_feature.py
--rw-r--r--   0        0        0     3748 2024-05-23 19:26:23.358148 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_observation_sequence_result.py
--rw-r--r--   0        0        0     4306 2024-05-23 19:26:23.390145 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py
--rw-r--r--   0        0        0     4637 2024-05-23 19:26:23.438140 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_observation_status.py
--rw-r--r--   0        0        0     3192 2024-05-23 19:26:23.490135 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_organization_target.py
--rw-r--r--   0        0        0     3644 2024-05-23 19:26:23.530131 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_satellite_potential.py
--rw-r--r--   0        0        0     3528 2024-05-23 19:26:23.578127 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_satellite_target.py
--rw-r--r--   0        0        0     3733 2024-05-23 19:26:23.622122 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_search_instruction.py
--rw-r--r--   0        0        0     3407 2024-05-23 19:26:23.666118 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_search_instruction_step.py
--rw-r--r--   0        0        0     3634 2024-05-23 19:26:23.714114 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_survey_instruction.py
--rw-r--r--   0        0        0     2799 2024-05-23 19:26:23.766108 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_survey_instruction_step.py
--rw-r--r--   0        0        0     3716 2024-05-23 19:26:23.818103 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_target_correlation.py
--rw-r--r--   0        0        0     3185 2024-05-23 19:26:23.910095 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_tdm.py
--rw-r--r--   0        0        0     2575 2024-05-23 19:26:23.978088 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_update_email_configuration_request.py
--rw-r--r--   0        0        0     2913 2024-05-23 19:26:24.074079 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_update_satellite_target_request.py
--rw-r--r--   0        0        0     3146 2024-05-23 19:26:24.122074 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py
--rw-r--r--   0        0        0     2963 2024-05-23 19:26:24.178069 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_webhook_configuration.py
--rw-r--r--   0        0        0     1386 2024-05-23 19:26:24.226064 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/weather_condition.py
--rw-r--r--   0        0        0     1350 2024-05-23 19:26:24.278059 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/webhook_auth_type.py
--rw-r--r--   0        0        0     1734 2024-05-23 19:26:24.314056 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/webhook_event.py
--rw-r--r--   0        0        0        0 2024-05-23 19:26:24.346053 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/py.typed
--rw-r--r--   0        0        0    13423 2024-05-23 19:26:24.402047 ourskyai_sda_api-1.3.3654/ourskyai_sda_api/rest.py
--rw-r--r--   0        0        0      731 2024-05-23 19:26:24.454042 ourskyai_sda_api-1.3.3654/pyproject.toml
--rw-r--r--   0        0        0    11113 1970-01-01 00:00:00.000000 ourskyai_sda_api-1.3.3654/PKG-INFO
+-rw-r--r--   0        0        0    10151 2024-05-23 23:15:12.505301 ourskyai_sda_api-1.3.3657/README.md
+-rw-r--r--   0        0        0     5222 2024-05-23 23:15:15.016862 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/__init__.py
+-rw-r--r--   0        0        0      104 2024-05-23 23:15:15.044857 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/api/__init__.py
+-rw-r--r--   0        0        0   220784 2024-05-23 23:15:15.156838 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/api/default_api.py
+-rw-r--r--   0        0        0    30830 2024-05-23 23:15:15.196831 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-23 23:15:15.256820 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/api_response.py
+-rw-r--r--   0        0        0    15175 2024-05-23 23:15:15.300812 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/configuration.py
+-rw-r--r--   0        0        0     5923 2024-05-23 23:15:15.352803 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/exceptions.py
+-rw-r--r--   0        0        0     4601 2024-05-23 23:15:15.392796 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/__init__.py
+-rw-r--r--   0        0        0     4311 2024-05-23 23:15:15.452786 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/astrometric_offsets.py
+-rw-r--r--   0        0        0     2394 2024-05-23 23:15:15.504777 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/empty_success.py
+-rw-r--r--   0        0        0     1676 2024-05-23 23:15:15.548769 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/filter_type.py
+-rw-r--r--   0        0        0     2420 2024-05-23 23:15:15.600760 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/fits_header.py
+-rw-r--r--   0        0        0     2645 2024-05-23 23:15:15.652751 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/location.py
+-rw-r--r--   0        0        0     1237 2024-05-23 23:15:15.700743 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/mount_type.py
+-rw-r--r--   0        0        0     2756 2024-05-23 23:15:15.752733 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/observation_bounding_box.py
+-rw-r--r--   0        0        0     3713 2024-05-23 23:15:15.816722 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/observation_quality.py
+-rw-r--r--   0        0        0     6381 2024-05-23 23:15:15.864714 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/observation_result.py
+-rw-r--r--   0        0        0     1320 2024-05-23 23:15:15.924703 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/observation_state.py
+-rw-r--r--   0        0        0     1529 2024-05-23 23:15:15.952698 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/orbit_type.py
+-rw-r--r--   0        0        0     1361 2024-05-23 23:15:16.012688 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/satellite_target_tracking_status.py
+-rw-r--r--   0        0        0     1241 2024-05-23 23:15:16.068678 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/shutter_type.py
+-rw-r--r--   0        0        0     2382 2024-05-23 23:15:16.108671 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/successful_create.py
+-rw-r--r--   0        0        0     1258 2024-05-23 23:15:16.168661 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/tracking_type.py
+-rw-r--r--   0        0        0     2534 2024-05-23 23:15:16.224651 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2605 2024-05-23 23:15:16.272642 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     3169 2024-05-23 23:15:16.320634 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2609 2024-05-23 23:15:16.368626 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_create_organization_target_request.py
+-rw-r--r--   0        0        0     2761 2024-05-23 23:15:16.412618 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_create_satellite_target_request.py
+-rw-r--r--   0        0        0     3373 2024-05-23 23:15:16.460610 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_create_search_instruction_request.py
+-rw-r--r--   0        0        0     3353 2024-05-23 23:15:16.516600 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_create_survey_instruction_request.py
+-rw-r--r--   0        0        0     3017 2024-05-23 23:15:16.564592 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_get_satellite_targets_response.py
+-rw-r--r--   0        0        0     4457 2024-05-23 23:15:16.628580 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_ground_station_participant.py
+-rw-r--r--   0        0        0     3922 2024-05-23 23:15:16.676572 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     6285 2024-05-23 23:15:16.720564 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0     4676 2024-05-23 23:15:16.776554 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_observation_feature.py
+-rw-r--r--   0        0        0     3748 2024-05-23 23:15:16.820547 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_observation_sequence_result.py
+-rw-r--r--   0        0        0     4306 2024-05-23 23:15:16.864539 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py
+-rw-r--r--   0        0        0     4637 2024-05-23 23:15:16.908531 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_observation_status.py
+-rw-r--r--   0        0        0     3192 2024-05-23 23:15:16.956523 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_organization_target.py
+-rw-r--r--   0        0        0     3644 2024-05-23 23:15:17.064504 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_satellite_potential.py
+-rw-r--r--   0        0        0     3528 2024-05-23 23:15:17.112496 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_satellite_target.py
+-rw-r--r--   0        0        0     3733 2024-05-23 23:15:17.156488 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_search_instruction.py
+-rw-r--r--   0        0        0     3407 2024-05-23 23:15:17.232475 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_search_instruction_step.py
+-rw-r--r--   0        0        0     3634 2024-05-23 23:15:17.288465 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_survey_instruction.py
+-rw-r--r--   0        0        0     2799 2024-05-23 23:15:17.328458 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_survey_instruction_step.py
+-rw-r--r--   0        0        0     3716 2024-05-23 23:15:17.376449 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_target_correlation.py
+-rw-r--r--   0        0        0     3185 2024-05-23 23:15:17.440438 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_tdm.py
+-rw-r--r--   0        0        0     2575 2024-05-23 23:15:17.488430 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_update_email_configuration_request.py
+-rw-r--r--   0        0        0     2913 2024-05-23 23:15:17.560417 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_update_satellite_target_request.py
+-rw-r--r--   0        0        0     3146 2024-05-23 23:15:17.608409 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py
+-rw-r--r--   0        0        0     2963 2024-05-23 23:15:17.664399 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_webhook_configuration.py
+-rw-r--r--   0        0        0     1386 2024-05-23 23:15:17.712391 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/weather_condition.py
+-rw-r--r--   0        0        0     1350 2024-05-23 23:15:17.756383 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/webhook_auth_type.py
+-rw-r--r--   0        0        0     1734 2024-05-23 23:15:17.820372 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/webhook_event.py
+-rw-r--r--   0        0        0        0 2024-05-23 23:15:17.852366 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/py.typed
+-rw-r--r--   0        0        0    13423 2024-05-23 23:15:17.892359 ourskyai_sda_api-1.3.3657/ourskyai_sda_api/rest.py
+-rw-r--r--   0        0        0      731 2024-05-23 23:15:17.940351 ourskyai_sda_api-1.3.3657/pyproject.toml
+-rw-r--r--   0        0        0    11113 1970-01-01 00:00:00.000000 ourskyai_sda_api-1.3.3657/PKG-INFO
```

### Comparing `ourskyai_sda_api-1.3.3654/README.md` & `ourskyai_sda_api-1.3.3657/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 The basic flow for a new organization is as follows:
 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe.
 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above.
 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
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

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/__init__.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3654"
+__version__ = "1.3.3657"
 
 # import apis into sdk package
 from ourskyai_sda_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_sda_api.api_response import ApiResponse
 from ourskyai_sda_api.api_client import ApiClient
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/api/default_api.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/api_client.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
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

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/api_response.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/configuration.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
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

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/exceptions.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/__init__.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/astrometric_offsets.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/astrometric_offsets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/empty_success.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/empty_success.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/filter_type.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/filter_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/fits_header.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/fits_header.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/location.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/location.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/mount_type.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/mount_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/observation_bounding_box.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/observation_bounding_box.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/observation_quality.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/observation_quality.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/observation_result.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/observation_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/observation_state.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/observation_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/orbit_type.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/orbit_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/satellite_target_tracking_status.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/satellite_target_tracking_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/shutter_type.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/shutter_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/successful_create.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/successful_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/tracking_type.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/tracking_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_create_image_set_image_request.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_create_image_set_image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_create_image_set_image_response.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_create_image_set_image_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_create_image_set_request.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_create_image_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_create_organization_target_request.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_create_organization_target_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_create_satellite_target_request.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_create_satellite_target_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_create_search_instruction_request.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_create_search_instruction_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_create_survey_instruction_request.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_create_survey_instruction_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_get_satellite_targets_response.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_get_satellite_targets_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_ground_station_participant.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_ground_station_participant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_image_set.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_image_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_image_set_image.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_image_set_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_observation_feature.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_observation_feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_observation_sequence_result.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_observation_sequence_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_observation_status.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_observation_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_organization_target.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_organization_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_satellite_potential.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_satellite_potential.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_satellite_target.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_satellite_target.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_search_instruction.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_search_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_search_instruction_step.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_search_instruction_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_survey_instruction.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_survey_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_survey_instruction_step.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_survey_instruction_step.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_target_correlation.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_target_correlation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_tdm.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_tdm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_update_email_configuration_request.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_update_email_configuration_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_update_satellite_target_request.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_update_satellite_target_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/v1_webhook_configuration.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/v1_webhook_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/weather_condition.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/weather_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/webhook_auth_type.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/webhook_auth_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/models/webhook_event.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/models/webhook_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3654/ourskyai_sda_api/rest.py` & `ourskyai_sda_api-1.3.3657/ourskyai_sda_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3654
+    The version of the OpenAPI document: 1.3.3657
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_sda_api-1.3.3654/pyproject.toml` & `ourskyai_sda_api-1.3.3657/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_sda_api"
-version = "1.3.3654"
+version = "1.3.3657"
 description = "OurSky SDA"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky SDA"]
 include = ["ourskyai_sda_api/py.typed"]
```

### Comparing `ourskyai_sda_api-1.3.3654/PKG-INFO` & `ourskyai_sda_api-1.3.3657/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_sda_api
-Version: 1.3.3654
+Version: 1.3.3657
 Summary: OurSky SDA
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky SDA
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -27,16 +27,16 @@
 The basic flow for a new organization is as follows:
 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe.
 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above.
 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
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

