# Comparing `tmp/coactive-1.0.8.tar.gz` & `tmp/coactive-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coactive-1.0.8.tar", max compression
+gzip compressed data, was "coactive-1.0.9.tar", max compression
```

## Comparing `coactive-1.0.8.tar` & `coactive-1.0.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     4126 2024-04-08 18:42:18.773704 coactive-1.0.8/README.md
--rw-r--r--   0        0        0      402 2024-04-08 18:42:18.777704 coactive-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     2782 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/__init__.py
--rw-r--r--   0        0        0     3229 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/client.py
--rw-r--r--   0        0        0      519 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/core/api_error.py
--rw-r--r--   0        0        0     1382 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      157 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/environment.py
--rw-r--r--   0        0        0      296 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/errors/__init__.py
--rw-r--r--   0        0        0      285 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/errors/bad_request_error.py
--rw-r--r--   0        0        0      246 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/errors/not_found_error.py
--rw-r--r--   0        0        0      313 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/py.typed
--rw-r--r--   0        0        0      308 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/__init__.py
--rw-r--r--   0        0        0      143 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/asset/__init__.py
--rw-r--r--   0        0        0     9326 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/asset/client.py
--rw-r--r--   0        0        0      162 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/asset/types/__init__.py
--rw-r--r--   0        0        0      209 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/asset/types/image_or_keyframe_detail.py
--rw-r--r--   0        0        0       65 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/classification/__init__.py
--rw-r--r--   0        0        0     5995 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/classification/client.py
--rw-r--r--   0        0        0       65 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/concept/__init__.py
--rw-r--r--   0        0        0    31777 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/concept/client.py
--rw-r--r--   0        0        0       65 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/credentials/__init__.py
--rw-r--r--   0        0        0    10437 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/credentials/client.py
--rw-r--r--   0        0        0       65 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/dataset/__init__.py
--rw-r--r--   0        0        0    38568 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/dataset/client.py
--rw-r--r--   0        0        0       65 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/query/__init__.py
--rw-r--r--   0        0        0    20726 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/query/client.py
--rw-r--r--   0        0        0       65 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/search/__init__.py
--rw-r--r--   0        0        0    10133 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/resources/search/client.py
--rw-r--r--   0        0        0     3554 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/__init__.py
--rw-r--r--   0        0        0     1408 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/add_assets_confirmation.py
--rw-r--r--   0        0        0     1220 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/add_image_request.py
--rw-r--r--   0        0        0     1129 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/add_video_request.py
--rw-r--r--   0        0        0     2096 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/added_image.py
--rw-r--r--   0        0        0     2027 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/added_video.py
--rw-r--r--   0        0        0     1419 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/audio_segment.py
--rw-r--r--   0        0        0     1156 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/candidates_to_label.py
--rw-r--r--   0        0        0     1131 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/classification.py
--rw-r--r--   0        0        0     1454 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/classification_score.py
--rw-r--r--   0        0        0     1968 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/concept.py
--rw-r--r--   0        0        0     1572 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/concept_label.py
--rw-r--r--   0        0        0      534 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/concept_label_enum.py
--rw-r--r--   0        0        0     1659 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/concept_label_request.py
--rw-r--r--   0        0        0     1237 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/credentials.py
--rw-r--r--   0        0        0     1537 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/credentials_validation.py
--rw-r--r--   0        0        0     2305 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/dataset.py
--rw-r--r--   0        0        0     1888 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/dataset_status_enum.py
--rw-r--r--   0        0        0      998 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/error_response.py
--rw-r--r--   0        0        0      966 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/http_validation_error.py
--rw-r--r--   0        0        0     1819 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/image.py
--rw-r--r--   0        0        0      185 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/image_or_keyframe.py
--rw-r--r--   0        0        0      194 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/image_or_keyframe_candidate.py
--rw-r--r--   0        0        0      471 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/key_type_enum.py
--rw-r--r--   0        0        0     1627 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/keyframe.py
--rw-r--r--   0        0        0     1185 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_concept_labels.py
--rw-r--r--   0        0        0     1174 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_concepts.py
--rw-r--r--   0        0        0     1170 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_datasets.py
--rw-r--r--   0        0        0     1173 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_images.py
--rw-r--r--   0        0        0     1251 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_links_response.py
--rw-r--r--   0        0        0     1429 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_meta_response.py
--rw-r--r--   0        0        0     1438 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_page_details_response.py
--rw-r--r--   0        0        0     1163 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_queries.py
--rw-r--r--   0        0        0     1173 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/paged_videos.py
--rw-r--r--   0        0        0     2255 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/query.py
--rw-r--r--   0        0        0     1327 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/query_result.py
--rw-r--r--   0        0        0     1131 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/query_results_download_url.py
--rw-r--r--   0        0        0     1033 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/query_row.py
--rw-r--r--   0        0        0     1139 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/query_status_enum.py
--rw-r--r--   0        0        0     2400 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/query_with_result.py
--rw-r--r--   0        0        0     1200 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/search_result.py
--rw-r--r--   0        0        0     1326 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/shot.py
--rw-r--r--   0        0        0      528 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/sort_direction_enum.py
--rw-r--r--   0        0        0     1119 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/sort_item.py
--rw-r--r--   0        0        0      724 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/storage_type_enum.py
--rw-r--r--   0        0        0     1353 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/update_assets_metadata_confirmation.py
--rw-r--r--   0        0        0     1383 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/update_image_metadata_request.py
--rw-r--r--   0        0        0     1382 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/update_video_metadata_request.py
--rw-r--r--   0        0        0     2096 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/updated_image.py
--rw-r--r--   0        0        0     2028 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/updated_video.py
--rw-r--r--   0        0        0      992 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     1750 2024-04-08 18:42:18.777704 coactive-1.0.8/src/coactive/types/video.py
--rw-r--r--   0        0        0     4631 1970-01-01 00:00:00.000000 coactive-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     4126 2024-04-08 20:58:38.849863 coactive-1.0.9/README.md
+-rw-r--r--   0        0        0      402 2024-04-08 20:58:38.849863 coactive-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2782 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/__init__.py
+-rw-r--r--   0        0        0     3229 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/client.py
+-rw-r--r--   0        0        0      519 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/core/api_error.py
+-rw-r--r--   0        0        0     1382 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      157 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/environment.py
+-rw-r--r--   0        0        0      296 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/errors/__init__.py
+-rw-r--r--   0        0        0      285 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/errors/bad_request_error.py
+-rw-r--r--   0        0        0      246 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/errors/not_found_error.py
+-rw-r--r--   0        0        0      313 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/py.typed
+-rw-r--r--   0        0        0      308 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/resources/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/resources/asset/__init__.py
+-rw-r--r--   0        0        0     9326 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/resources/asset/client.py
+-rw-r--r--   0        0        0      162 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/resources/asset/types/__init__.py
+-rw-r--r--   0        0        0      209 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/resources/asset/types/image_or_keyframe_detail.py
+-rw-r--r--   0        0        0       65 2024-04-08 20:58:38.849863 coactive-1.0.9/src/coactive/resources/classification/__init__.py
+-rw-r--r--   0        0        0     5869 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/resources/classification/client.py
+-rw-r--r--   0        0        0       65 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/resources/concept/__init__.py
+-rw-r--r--   0        0        0    31541 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/resources/concept/client.py
+-rw-r--r--   0        0        0       65 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/resources/credentials/__init__.py
+-rw-r--r--   0        0        0    11039 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/resources/credentials/client.py
+-rw-r--r--   0        0        0       65 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/resources/dataset/__init__.py
+-rw-r--r--   0        0        0    37982 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/resources/dataset/client.py
+-rw-r--r--   0        0        0       65 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/resources/query/__init__.py
+-rw-r--r--   0        0        0    20742 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/resources/query/client.py
+-rw-r--r--   0        0        0       65 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/resources/search/__init__.py
+-rw-r--r--   0        0        0    10503 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/resources/search/client.py
+-rw-r--r--   0        0        0     3554 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/__init__.py
+-rw-r--r--   0        0        0     1408 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/add_assets_confirmation.py
+-rw-r--r--   0        0        0     1220 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/add_image_request.py
+-rw-r--r--   0        0        0     1129 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/add_video_request.py
+-rw-r--r--   0        0        0     2096 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/added_image.py
+-rw-r--r--   0        0        0     2027 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/added_video.py
+-rw-r--r--   0        0        0     1419 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/audio_segment.py
+-rw-r--r--   0        0        0     1156 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/candidates_to_label.py
+-rw-r--r--   0        0        0     1131 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/classification.py
+-rw-r--r--   0        0        0     1454 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/classification_score.py
+-rw-r--r--   0        0        0     1968 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/concept.py
+-rw-r--r--   0        0        0     1572 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/concept_label.py
+-rw-r--r--   0        0        0      534 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/concept_label_enum.py
+-rw-r--r--   0        0        0     1659 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/concept_label_request.py
+-rw-r--r--   0        0        0     1237 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/credentials.py
+-rw-r--r--   0        0        0     1537 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/credentials_validation.py
+-rw-r--r--   0        0        0     2305 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/dataset.py
+-rw-r--r--   0        0        0     1888 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/dataset_status_enum.py
+-rw-r--r--   0        0        0      998 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/error_response.py
+-rw-r--r--   0        0        0      966 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/http_validation_error.py
+-rw-r--r--   0        0        0     1819 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/image.py
+-rw-r--r--   0        0        0      185 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/image_or_keyframe.py
+-rw-r--r--   0        0        0      194 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/image_or_keyframe_candidate.py
+-rw-r--r--   0        0        0      471 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/key_type_enum.py
+-rw-r--r--   0        0        0     1627 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/keyframe.py
+-rw-r--r--   0        0        0     1185 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/paged_concept_labels.py
+-rw-r--r--   0        0        0     1174 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/paged_concepts.py
+-rw-r--r--   0        0        0     1170 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/paged_datasets.py
+-rw-r--r--   0        0        0     1173 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/paged_images.py
+-rw-r--r--   0        0        0     1251 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/paged_links_response.py
+-rw-r--r--   0        0        0     1429 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/paged_meta_response.py
+-rw-r--r--   0        0        0     1438 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/paged_page_details_response.py
+-rw-r--r--   0        0        0     1163 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/paged_queries.py
+-rw-r--r--   0        0        0     1173 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/paged_videos.py
+-rw-r--r--   0        0        0     2255 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/query.py
+-rw-r--r--   0        0        0     1327 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/query_result.py
+-rw-r--r--   0        0        0     1131 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/query_results_download_url.py
+-rw-r--r--   0        0        0     1033 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/query_row.py
+-rw-r--r--   0        0        0     1139 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/query_status_enum.py
+-rw-r--r--   0        0        0     2400 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/query_with_result.py
+-rw-r--r--   0        0        0     1200 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/search_result.py
+-rw-r--r--   0        0        0     1326 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/shot.py
+-rw-r--r--   0        0        0      528 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/sort_direction_enum.py
+-rw-r--r--   0        0        0     1119 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/sort_item.py
+-rw-r--r--   0        0        0      724 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/storage_type_enum.py
+-rw-r--r--   0        0        0     1353 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/update_assets_metadata_confirmation.py
+-rw-r--r--   0        0        0     1383 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/update_image_metadata_request.py
+-rw-r--r--   0        0        0     1382 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/update_video_metadata_request.py
+-rw-r--r--   0        0        0     2096 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/updated_image.py
+-rw-r--r--   0        0        0     2028 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/updated_video.py
+-rw-r--r--   0        0        0      992 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     1750 2024-04-08 20:58:38.853863 coactive-1.0.9/src/coactive/types/video.py
+-rw-r--r--   0        0        0     4631 1970-01-01 00:00:00.000000 coactive-1.0.9/PKG-INFO
```

### Comparing `coactive-1.0.8/README.md` & `coactive-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/__init__.py` & `coactive-1.0.9/src/coactive/__init__.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/client.py` & `coactive-1.0.9/src/coactive/client.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/core/__init__.py` & `coactive-1.0.9/src/coactive/core/__init__.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/core/client_wrapper.py` & `coactive-1.0.9/src/coactive/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self._token = token
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "coactive",
-            "X-Fern-SDK-Version": "1.0.8",
+            "X-Fern-SDK-Version": "1.0.9",
         }
         headers["Authorization"] = f"Bearer {self._get_token()}"
         return headers
 
     def _get_token(self) -> str:
         if isinstance(self._token, str):
             return self._token
```

### Comparing `coactive-1.0.8/src/coactive/core/datetime_utils.py` & `coactive-1.0.9/src/coactive/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/core/jsonable_encoder.py` & `coactive-1.0.9/src/coactive/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/resources/asset/client.py` & `coactive-1.0.9/src/coactive/resources/asset/client.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/resources/classification/client.py` & `coactive-1.0.9/src/coactive/resources/classification/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.classification.classify_image_at_url(
             url="s3://coactive-public/logo.png",
-            dataset_id="c40276f0-024b-4a3f-b3e6-dcf0d304843e",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"url": url}
         if concept_ids is not OMIT:
             _request["conceptIds"] = concept_ids
         if dataset_id is not OMIT:
             _request["datasetId"] = dataset_id
@@ -109,15 +108,14 @@
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.classification.classify_image_at_url(
             url="s3://coactive-public/logo.png",
-            dataset_id="c40276f0-024b-4a3f-b3e6-dcf0d304843e",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"url": url}
         if concept_ids is not OMIT:
             _request["conceptIds"] = concept_ids
         if dataset_id is not OMIT:
             _request["datasetId"] = dataset_id
```

### Comparing `coactive-1.0.8/src/coactive/resources/concept/client.py` & `coactive-1.0.9/src/coactive/resources/concept/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.concept.get(
-            concept_id="string",
+            concept_id="concept_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/concepts/{concept_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -177,15 +177,15 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.concept.delete(
-            concept_id="string",
+            concept_id="concept_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/concepts/{concept_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -224,15 +224,15 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.concept.update(
-            concept_id="string",
+            concept_id="concept_id",
             name="TheNorth",
             description="Screenshots and clips from Game of Thrones that take place in the North",
             threshold=0.8,
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if name is not OMIT:
@@ -282,15 +282,15 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.concept.get_labels(
-            concept_id="string",
+            concept_id="concept_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/concepts/{concept_id}/labels"),
             params=remove_none_from_dict({"offset": offset, "limit": limit, "labels_to_include": labels_to_include}),
             headers=self._client_wrapper.get_headers(),
@@ -320,19 +320,17 @@
         from coactive import ConceptLabelEnum, ConceptLabelRequest
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.concept.update_labels(
-            concept_id="string",
+            concept_id="concept_id",
             labels=[
                 ConceptLabelRequest(
-                    coactive_image_id="a6894d72-612d-4c20-b4d0-8f3f21c2bb10",
-                    image_path="s3://coactive-public/logo.png",
                     label=ConceptLabelEnum.POSITIVE,
                 )
             ],
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
@@ -362,15 +360,15 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.concept.get_label_candidates(
-            concept_id="string",
+            concept_id="concept_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/concepts/{concept_id}/candidates"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -502,15 +500,15 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.concept.get(
-            concept_id="string",
+            concept_id="concept_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/concepts/{concept_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -536,15 +534,15 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.concept.delete(
-            concept_id="string",
+            concept_id="concept_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/concepts/{concept_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -583,15 +581,15 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.concept.update(
-            concept_id="string",
+            concept_id="concept_id",
             name="TheNorth",
             description="Screenshots and clips from Game of Thrones that take place in the North",
             threshold=0.8,
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if name is not OMIT:
@@ -641,15 +639,15 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.concept.get_labels(
-            concept_id="string",
+            concept_id="concept_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/concepts/{concept_id}/labels"),
             params=remove_none_from_dict({"offset": offset, "limit": limit, "labels_to_include": labels_to_include}),
             headers=self._client_wrapper.get_headers(),
@@ -679,19 +677,17 @@
         from coactive import ConceptLabelEnum, ConceptLabelRequest
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.concept.update_labels(
-            concept_id="string",
+            concept_id="concept_id",
             labels=[
                 ConceptLabelRequest(
-                    coactive_image_id="a6894d72-612d-4c20-b4d0-8f3f21c2bb10",
-                    image_path="s3://coactive-public/logo.png",
                     label=ConceptLabelEnum.POSITIVE,
                 )
             ],
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
@@ -721,15 +717,15 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.concept.get_label_candidates(
-            concept_id="string",
+            concept_id="concept_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/concepts/{concept_id}/candidates"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
```

### Comparing `coactive-1.0.8/src/coactive/resources/credentials/client.py` & `coactive-1.0.9/src/coactive/resources/credentials/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,21 @@
 
     def add_aws_credentials(self, *, file: typing.IO) -> Credentials:
         """
         Add credentials to access data in your Amazon Web Services account
 
         Parameters:
             - file: typing.IO.
+        ---
+        from coactive.client import Coactive
+
+        client = Coactive(
+            token="YOUR_TOKEN",
+        )
+        client.credentials.add_aws_credentials()
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/credentials/aws"),
             data=jsonable_encoder({}),
             files={"file": file},
             headers=self._client_wrapper.get_headers(),
@@ -57,14 +64,21 @@
 
     def add_gcp_credentials(self, *, file: typing.IO) -> Credentials:
         """
         Add credentials to access data in your Google Cloud Platform account
 
         Parameters:
             - file: typing.IO.
+        ---
+        from coactive.client import Coactive
+
+        client = Coactive(
+            token="YOUR_TOKEN",
+        )
+        client.credentials.add_gcp_credentials()
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/credentials/gcp"),
             data=jsonable_encoder({}),
             files={"file": file},
             headers=self._client_wrapper.get_headers(),
@@ -93,15 +107,14 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.credentials.test(
-            credentials_id="382cc760-8e8e-4b97-abab-84438282cb9a",
             data_path="s3://your-s3-bucket/prefix/to/use/",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"dataPath": data_path}
         if credentials_id is not OMIT:
             _request["credentialsId"] = credentials_id
         _response = self._client_wrapper.httpx_client.request(
@@ -132,14 +145,21 @@
 
     async def add_aws_credentials(self, *, file: typing.IO) -> Credentials:
         """
         Add credentials to access data in your Amazon Web Services account
 
         Parameters:
             - file: typing.IO.
+        ---
+        from coactive.client import AsyncCoactive
+
+        client = AsyncCoactive(
+            token="YOUR_TOKEN",
+        )
+        await client.credentials.add_aws_credentials()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/credentials/aws"),
             data=jsonable_encoder({}),
             files={"file": file},
             headers=self._client_wrapper.get_headers(),
@@ -159,14 +179,21 @@
 
     async def add_gcp_credentials(self, *, file: typing.IO) -> Credentials:
         """
         Add credentials to access data in your Google Cloud Platform account
 
         Parameters:
             - file: typing.IO.
+        ---
+        from coactive.client import AsyncCoactive
+
+        client = AsyncCoactive(
+            token="YOUR_TOKEN",
+        )
+        await client.credentials.add_gcp_credentials()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/credentials/gcp"),
             data=jsonable_encoder({}),
             files={"file": file},
             headers=self._client_wrapper.get_headers(),
@@ -195,15 +222,14 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.credentials.test(
-            credentials_id="382cc760-8e8e-4b97-abab-84438282cb9a",
             data_path="s3://your-s3-bucket/prefix/to/use/",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"dataPath": data_path}
         if credentials_id is not OMIT:
             _request["credentialsId"] = credentials_id
         _response = await self._client_wrapper.httpx_client.request(
```

### Comparing `coactive-1.0.8/src/coactive/resources/dataset/client.py` & `coactive-1.0.9/src/coactive/resources/dataset/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,15 +89,14 @@
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.dataset.create(
             name="GameOfThrones",
             description="A dataset containing screenshots and clips from the tv show Game of Thrones",
-            credentials_id="382cc760-8e8e-4b97-abab-84438282cb9a",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if description is not OMIT:
             _request["description"] = description
         if credentials_id is not OMIT:
             _request["credentialsId"] = credentials_id
@@ -131,15 +130,15 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.dataset.get(
-            dataset_id="string",
+            dataset_id="dataset_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/datasets/{dataset_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -165,15 +164,15 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.dataset.delete(
-            dataset_id="string",
+            dataset_id="dataset_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/datasets/{dataset_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -205,15 +204,15 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.dataset.update(
-            dataset_id="string",
+            dataset_id="dataset_id",
             name="GameOfThrones",
             description="A dataset containing screenshots and clips from the tv show Game of Thrones",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if name is not OMIT:
             _request["name"] = name
@@ -255,15 +254,15 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.dataset.get_images(
-            dataset_id="string",
+            dataset_id="dataset_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/datasets/{dataset_id}/images"),
             params=remove_none_from_dict({"offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
@@ -296,15 +295,15 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.dataset.get_videos(
-            dataset_id="string",
+            dataset_id="dataset_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/datasets/{dataset_id}/videos"),
             params=remove_none_from_dict({"offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
@@ -348,15 +347,15 @@
         from coactive import AddImageRequest, AddVideoRequest
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.dataset.add_assets(
-            dataset_id="string",
+            dataset_id="dataset_id",
             images=[
                 AddImageRequest(
                     path="s3://coactive-public/logo.png",
                     id="kingslanding_041711",
                     metadata={"artist": "Marc Simonetti"},
                 )
             ],
@@ -367,16 +366,14 @@
                         "show": "The Boys",
                         "season": 1,
                         "episode": 1,
                         "title": "The Name of the Game",
                     },
                 )
             ],
-            data_path="s3://your-s3-bucket/path/prefix",
-            csv_path="path/to/file.csv",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if images is not OMIT:
             _request["images"] = images
         if videos is not OMIT:
             _request["videos"] = videos
@@ -423,26 +420,24 @@
         from coactive import UpdateImageMetadataRequest, UpdateVideoMetadataRequest
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.dataset.update_asset_metadata(
-            dataset_id="string",
+            dataset_id="dataset_id",
             images=[
                 UpdateImageMetadataRequest(
                     path="s3://coactive-public/logo.png",
-                    coactive_image_id="a6894d72-612d-4c20-b4d0-8f3f21c2bb10",
                     metadata={"artist": "Marc Simonetti"},
                 )
             ],
             videos=[
                 UpdateVideoMetadataRequest(
                     path="s3://your-s3-bucket/path/to/video.mp4",
-                    coactive_video_id="5cf18348-8336-4db7-bb35-db7fbfe8951d",
                     metadata={"artist": "Marc Simonetti"},
                 )
             ],
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if images is not OMIT:
@@ -527,15 +522,14 @@
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.dataset.create(
             name="GameOfThrones",
             description="A dataset containing screenshots and clips from the tv show Game of Thrones",
-            credentials_id="382cc760-8e8e-4b97-abab-84438282cb9a",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if description is not OMIT:
             _request["description"] = description
         if credentials_id is not OMIT:
             _request["credentialsId"] = credentials_id
@@ -569,15 +563,15 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.dataset.get(
-            dataset_id="string",
+            dataset_id="dataset_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/datasets/{dataset_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -603,15 +597,15 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.dataset.delete(
-            dataset_id="string",
+            dataset_id="dataset_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/datasets/{dataset_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -643,15 +637,15 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.dataset.update(
-            dataset_id="string",
+            dataset_id="dataset_id",
             name="GameOfThrones",
             description="A dataset containing screenshots and clips from the tv show Game of Thrones",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if name is not OMIT:
             _request["name"] = name
@@ -693,15 +687,15 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.dataset.get_images(
-            dataset_id="string",
+            dataset_id="dataset_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/datasets/{dataset_id}/images"),
             params=remove_none_from_dict({"offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
@@ -734,15 +728,15 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.dataset.get_videos(
-            dataset_id="string",
+            dataset_id="dataset_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/datasets/{dataset_id}/videos"),
             params=remove_none_from_dict({"offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
@@ -786,15 +780,15 @@
         from coactive import AddImageRequest, AddVideoRequest
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.dataset.add_assets(
-            dataset_id="string",
+            dataset_id="dataset_id",
             images=[
                 AddImageRequest(
                     path="s3://coactive-public/logo.png",
                     id="kingslanding_041711",
                     metadata={"artist": "Marc Simonetti"},
                 )
             ],
@@ -805,16 +799,14 @@
                         "show": "The Boys",
                         "season": 1,
                         "episode": 1,
                         "title": "The Name of the Game",
                     },
                 )
             ],
-            data_path="s3://your-s3-bucket/path/prefix",
-            csv_path="path/to/file.csv",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if images is not OMIT:
             _request["images"] = images
         if videos is not OMIT:
             _request["videos"] = videos
@@ -861,26 +853,24 @@
         from coactive import UpdateImageMetadataRequest, UpdateVideoMetadataRequest
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.dataset.update_asset_metadata(
-            dataset_id="string",
+            dataset_id="dataset_id",
             images=[
                 UpdateImageMetadataRequest(
                     path="s3://coactive-public/logo.png",
-                    coactive_image_id="a6894d72-612d-4c20-b4d0-8f3f21c2bb10",
                     metadata={"artist": "Marc Simonetti"},
                 )
             ],
             videos=[
                 UpdateVideoMetadataRequest(
                     path="s3://your-s3-bucket/path/to/video.mp4",
-                    coactive_video_id="5cf18348-8336-4db7-bb35-db7fbfe8951d",
                     metadata={"artist": "Marc Simonetti"},
                 )
             ],
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if images is not OMIT:
```

### Comparing `coactive-1.0.8/src/coactive/resources/query/client.py` & `coactive-1.0.9/src/coactive/resources/query/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.query.get(
-            query_id="string",
+            query_id="query_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/queries/{query_id}"),
             params=remove_none_from_dict({"offset": offset, "limit": limit, "exclude_results": exclude_results}),
             headers=self._client_wrapper.get_headers(),
@@ -167,15 +167,15 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.query.delete(
-            query_id="string",
+            query_id="query_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/queries/{query_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -201,15 +201,15 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.query.stop(
-            query_id="string",
+            query_id="query_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/queries/{query_id}/stop"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -235,15 +235,15 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.query.get_results_download_url(
-            query_id="string",
+            query_id="query_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/queries/{query_id}/csv/url"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -368,15 +368,15 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.query.get(
-            query_id="string",
+            query_id="query_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/queries/{query_id}"),
             params=remove_none_from_dict({"offset": offset, "limit": limit, "exclude_results": exclude_results}),
             headers=self._client_wrapper.get_headers(),
@@ -403,15 +403,15 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.query.delete(
-            query_id="string",
+            query_id="query_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/queries/{query_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -437,15 +437,15 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.query.stop(
-            query_id="string",
+            query_id="query_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/queries/{query_id}/stop"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -471,15 +471,15 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.query.get_results_download_url(
-            query_id="string",
+            query_id="query_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/queries/{query_id}/csv/url"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
```

### Comparing `coactive-1.0.8/src/coactive/resources/search/client.py` & `coactive-1.0.9/src/coactive/resources/search/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         *,
         query: typing.Optional[str] = None,
         dataset_id: str,
         offset: typing.Optional[int] = None,
         limit: typing.Optional[int] = None,
     ) -> SearchResult:
         """
-        Perform a visual and audio search of a dataset using a natural language (text) query
+        Perform a visual and audio search of a dataset using a natural language (text) query. Please note that the meta.page.total value in the response is set to "null" as Coactive allows for paginating through the entire dataset using the similarity search relevance.
 
         Parameters:
             - query: typing.Optional[str]. The search query
 
             - dataset_id: str. The id of the dataset to search
 
             - offset: typing.Optional[int]. Starting index to return
@@ -44,15 +44,15 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.search.search_dataset(
-            dataset_id="string",
+            dataset_id="dataset_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/search"),
             params=remove_none_from_dict({"query": query, "dataset_id": dataset_id, "offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
@@ -98,15 +98,15 @@
         ---
         from coactive.client import Coactive
 
         client = Coactive(
             token="YOUR_TOKEN",
         )
         client.search.search_for_similar_images_in_dataset(
-            dataset_id="string",
+            dataset_id="dataset_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/search/similar-images"),
             params=remove_none_from_dict(
                 {
@@ -143,15 +143,15 @@
         *,
         query: typing.Optional[str] = None,
         dataset_id: str,
         offset: typing.Optional[int] = None,
         limit: typing.Optional[int] = None,
     ) -> SearchResult:
         """
-        Perform a visual and audio search of a dataset using a natural language (text) query
+        Perform a visual and audio search of a dataset using a natural language (text) query. Please note that the meta.page.total value in the response is set to "null" as Coactive allows for paginating through the entire dataset using the similarity search relevance.
 
         Parameters:
             - query: typing.Optional[str]. The search query
 
             - dataset_id: str. The id of the dataset to search
 
             - offset: typing.Optional[int]. Starting index to return
@@ -160,15 +160,15 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.search.search_dataset(
-            dataset_id="string",
+            dataset_id="dataset_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/search"),
             params=remove_none_from_dict({"query": query, "dataset_id": dataset_id, "offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
@@ -214,15 +214,15 @@
         ---
         from coactive.client import AsyncCoactive
 
         client = AsyncCoactive(
             token="YOUR_TOKEN",
         )
         await client.search.search_for_similar_images_in_dataset(
-            dataset_id="string",
+            dataset_id="dataset_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/search/similar-images"),
             params=remove_none_from_dict(
                 {
```

### Comparing `coactive-1.0.8/src/coactive/types/__init__.py` & `coactive-1.0.9/src/coactive/types/__init__.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/add_assets_confirmation.py` & `coactive-1.0.9/src/coactive/types/add_assets_confirmation.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/add_image_request.py` & `coactive-1.0.9/src/coactive/types/add_image_request.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/add_video_request.py` & `coactive-1.0.9/src/coactive/types/add_video_request.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/added_image.py` & `coactive-1.0.9/src/coactive/types/added_image.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/added_video.py` & `coactive-1.0.9/src/coactive/types/added_video.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/audio_segment.py` & `coactive-1.0.9/src/coactive/types/audio_segment.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/candidates_to_label.py` & `coactive-1.0.9/src/coactive/types/candidates_to_label.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/classification.py` & `coactive-1.0.9/src/coactive/types/classification.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/classification_score.py` & `coactive-1.0.9/src/coactive/types/classification_score.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/concept.py` & `coactive-1.0.9/src/coactive/types/concept.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/concept_label.py` & `coactive-1.0.9/src/coactive/types/concept_label.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/concept_label_enum.py` & `coactive-1.0.9/src/coactive/types/concept_label_enum.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/concept_label_request.py` & `coactive-1.0.9/src/coactive/types/concept_label_request.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/credentials.py` & `coactive-1.0.9/src/coactive/types/credentials.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/credentials_validation.py` & `coactive-1.0.9/src/coactive/types/credentials_validation.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/dataset.py` & `coactive-1.0.9/src/coactive/types/dataset.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/dataset_status_enum.py` & `coactive-1.0.9/src/coactive/types/dataset_status_enum.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/error_response.py` & `coactive-1.0.9/src/coactive/types/error_response.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/http_validation_error.py` & `coactive-1.0.9/src/coactive/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/image.py` & `coactive-1.0.9/src/coactive/types/image.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/keyframe.py` & `coactive-1.0.9/src/coactive/types/keyframe.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/paged_concept_labels.py` & `coactive-1.0.9/src/coactive/types/paged_concept_labels.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/paged_concepts.py` & `coactive-1.0.9/src/coactive/types/paged_concepts.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/paged_datasets.py` & `coactive-1.0.9/src/coactive/types/paged_datasets.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/paged_images.py` & `coactive-1.0.9/src/coactive/types/paged_images.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/paged_links_response.py` & `coactive-1.0.9/src/coactive/types/paged_links_response.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/paged_meta_response.py` & `coactive-1.0.9/src/coactive/types/paged_meta_response.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/paged_page_details_response.py` & `coactive-1.0.9/src/coactive/types/paged_page_details_response.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/paged_queries.py` & `coactive-1.0.9/src/coactive/types/paged_queries.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/paged_videos.py` & `coactive-1.0.9/src/coactive/types/paged_videos.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/query.py` & `coactive-1.0.9/src/coactive/types/query.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/query_result.py` & `coactive-1.0.9/src/coactive/types/query_result.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/query_results_download_url.py` & `coactive-1.0.9/src/coactive/types/query_results_download_url.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/query_row.py` & `coactive-1.0.9/src/coactive/types/query_row.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/query_status_enum.py` & `coactive-1.0.9/src/coactive/types/query_status_enum.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/query_with_result.py` & `coactive-1.0.9/src/coactive/types/query_with_result.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/search_result.py` & `coactive-1.0.9/src/coactive/types/search_result.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/shot.py` & `coactive-1.0.9/src/coactive/types/shot.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/sort_direction_enum.py` & `coactive-1.0.9/src/coactive/types/sort_direction_enum.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/sort_item.py` & `coactive-1.0.9/src/coactive/types/sort_item.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/storage_type_enum.py` & `coactive-1.0.9/src/coactive/types/storage_type_enum.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/update_assets_metadata_confirmation.py` & `coactive-1.0.9/src/coactive/types/update_assets_metadata_confirmation.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/update_image_metadata_request.py` & `coactive-1.0.9/src/coactive/types/update_image_metadata_request.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/update_video_metadata_request.py` & `coactive-1.0.9/src/coactive/types/update_video_metadata_request.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/updated_image.py` & `coactive-1.0.9/src/coactive/types/updated_image.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/updated_video.py` & `coactive-1.0.9/src/coactive/types/updated_video.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/validation_error.py` & `coactive-1.0.9/src/coactive/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/src/coactive/types/video.py` & `coactive-1.0.9/src/coactive/types/video.py`

 * *Files identical despite different names*

### Comparing `coactive-1.0.8/PKG-INFO` & `coactive-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coactive
-Version: 1.0.8
+Version: 1.0.9
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

