# Comparing `tmp/crawlee-0.0.4b1.tar.gz` & `tmp/crawlee-0.0.4b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlee-0.0.4b1.tar", max compression
+gzip compressed data, was "crawlee-0.0.4b2.tar", max compression
```

## Comparing `crawlee-0.0.4b1.tar` & `crawlee-0.0.4b2.tar`

### file list

```diff
@@ -1,93 +1,94 @@
--rw-r--r--   0        0        0    11355 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/LICENSE
--rw-r--r--   0        0        0    16623 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/README.md
--rw-r--r--   0        0        0     6603 2024-05-21 10:42:58.843917 crawlee-0.0.4b1/pyproject.toml
--rw-r--r--   0        0        0       31 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/__init__.py
--rw-r--r--   0        0        0        0 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/__init__.py
--rw-r--r--   0        0        0      774 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/blocked.py
--rw-r--r--   0        0        0     3341 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/byte_size.py
--rw-r--r--   0        0        0      759 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/crypto.py
--rw-r--r--   0        0        0     3365 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/data_processing.py
--rw-r--r--   0        0        0     1683 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/env_vars.py
--rw-r--r--   0        0        0     3503 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/file.py
--rw-r--r--   0        0        0     5262 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/globs.py
--rw-r--r--   0        0        0     2056 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/lru_cache.py
--rw-r--r--   0        0        0      918 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/math.py
--rw-r--r--   0        0        0      715 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/measure_time.py
--rw-r--r--   0        0        0      790 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/models.py
--rw-r--r--   0        0        0     1585 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/recurring_task.py
--rw-r--r--   0        0        0     4765 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/requests.py
--rw-r--r--   0        0        0     2414 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/system.py
--rw-r--r--   0        0        0     1429 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/_utils/wait.py
--rw-r--r--   0        0        0      142 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/autoscaling/__init__.py
--rw-r--r--   0        0        0    14883 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/autoscaling/autoscaled_pool.py
--rw-r--r--   0        0        0        0 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/autoscaling/py.typed
--rw-r--r--   0        0        0    15793 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/autoscaling/snapshotter.py
--rw-r--r--   0        0        0     9293 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/autoscaling/system_status.py
--rw-r--r--   0        0        0     5140 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/autoscaling/types.py
--rw-r--r--   0        0        0      470 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/base_storage_client/__init__.py
--rw-r--r--   0        0        0     9143 2024-05-21 10:42:40.827903 crawlee-0.0.4b1/src/crawlee/base_storage_client/base_dataset_client.py
--rw-r--r--   0        0        0     1883 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/base_storage_client/base_dataset_collection_client.py
--rw-r--r--   0        0        0     3486 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/base_storage_client/base_key_value_store_client.py
--rw-r--r--   0        0        0     2025 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/base_storage_client/base_key_value_store_collection_client.py
--rw-r--r--   0        0        0     5622 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/base_storage_client/base_request_queue_client.py
--rw-r--r--   0        0        0     1992 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/base_storage_client/base_request_queue_collection_client.py
--rw-r--r--   0        0        0     2229 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/base_storage_client/base_storage_client.py
--rw-r--r--   0        0        0        0 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/base_storage_client/py.typed
--rw-r--r--   0        0        0      735 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/base_storage_client/types.py
--rw-r--r--   0        0        0      186 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/basic_crawler/__init__.py
--rw-r--r--   0        0        0    27235 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/basic_crawler/basic_crawler.py
--rw-r--r--   0        0        0     4696 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/basic_crawler/context_pipeline.py
--rw-r--r--   0        0        0     2145 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/basic_crawler/errors.py
--rw-r--r--   0        0        0     2279 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/basic_crawler/router.py
--rw-r--r--   0        0        0     2706 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/basic_crawler/types.py
--rw-r--r--   0        0        0       86 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/beautifulsoup_crawler/__init__.py
--rw-r--r--   0        0        0     5409 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
--rw-r--r--   0        0        0      524 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/beautifulsoup_crawler/types.py
--rw-r--r--   0        0        0     1310 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/configuration.py
--rw-r--r--   0        0        0      146 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/consts.py
--rw-r--r--   0        0        0      272 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/enqueue_strategy.py
--rw-r--r--   0        0        0       91 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/events/__init__.py
--rw-r--r--   0        0        0     7211 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/events/event_manager.py
--rw-r--r--   0        0        0     2682 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/events/local_event_manager.py
--rw-r--r--   0        0        0        0 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/events/py.typed
--rw-r--r--   0        0        0     1303 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/events/types.py
--rw-r--r--   0        0        0        0 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/http_clients/__init__.py
--rw-r--r--   0        0        0     1976 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/http_clients/base_http_client.py
--rw-r--r--   0        0        0     4426 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/http_clients/httpx_client.py
--rw-r--r--   0        0        0       59 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/http_crawler/__init__.py
--rw-r--r--   0        0        0     2852 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/http_crawler/http_crawler.py
--rw-r--r--   0        0        0      329 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/http_crawler/types.py
--rw-r--r--   0        0        0     4719 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/log_config.py
--rw-r--r--   0        0        0       55 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/__init__.py
--rw-r--r--   0        0        0    15666 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/_creation_management.py
--rw-r--r--   0        0        0    15684 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/dataset_client.py
--rw-r--r--   0        0        0     2243 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/dataset_collection_client.py
--rw-r--r--   0        0        0    15914 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/key_value_store_client.py
--rw-r--r--   0        0        0     2333 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/key_value_store_collection_client.py
--rw-r--r--   0        0        0    11113 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/memory_storage_client.py
--rw-r--r--   0        0        0        0 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/py.typed
--rw-r--r--   0        0        0    20944 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/request_queue_client.py
--rw-r--r--   0        0        0     2316 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/memory_storage_client/request_queue_collection_client.py
--rw-r--r--   0        0        0    12997 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/models.py
--rw-r--r--   0        0        0        0 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/py.typed
--rw-r--r--   0        0        0       67 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/sessions/__init__.py
--rw-r--r--   0        0        0     2430 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/sessions/models.py
--rw-r--r--   0        0        0        0 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/sessions/py.typed
--rw-r--r--   0        0        0     8084 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/sessions/session.py
--rw-r--r--   0        0        0    11695 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/sessions/session_pool.py
--rw-r--r--   0        0        0        0 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/statistics/__init__.py
--rw-r--r--   0        0        0      980 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/statistics/error_tracker.py
--rw-r--r--   0        0        0     3646 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/statistics/models.py
--rw-r--r--   0        0        0    10880 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/statistics/statistics.py
--rw-r--r--   0        0        0     1520 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storage_client_manager.py
--rw-r--r--   0        0        0      150 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/__init__.py
--rw-r--r--   0        0        0     8804 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/_creation_management.py
--rw-r--r--   0        0        0     1090 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/base_storage.py
--rw-r--r--   0        0        0    15956 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/dataset.py
--rw-r--r--   0        0        0     4994 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/key_value_store.py
--rw-r--r--   0        0        0        0 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/py.typed
--rw-r--r--   0        0        0     2841 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/request_list.py
--rw-r--r--   0        0        0     2755 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/request_provider.py
--rw-r--r--   0        0        0    25708 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/storages/request_queue.py
--rw-r--r--   0        0        0      630 2024-05-21 10:42:40.831903 crawlee-0.0.4b1/src/crawlee/types.py
--rw-r--r--   0        0        0    18689 1970-01-01 00:00:00.000000 crawlee-0.0.4b1/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/LICENSE
+-rw-r--r--   0        0        0    16623 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/README.md
+-rw-r--r--   0        0        0     6623 2024-05-24 18:44:17.299330 crawlee-0.0.4b2/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/__init__.py
+-rw-r--r--   0        0        0      774 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/blocked.py
+-rw-r--r--   0        0        0     3341 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/byte_size.py
+-rw-r--r--   0        0        0      759 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/crypto.py
+-rw-r--r--   0        0        0     3365 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/data_processing.py
+-rw-r--r--   0        0        0     1683 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/env_vars.py
+-rw-r--r--   0        0        0     3503 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/file.py
+-rw-r--r--   0        0        0     5262 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/globs.py
+-rw-r--r--   0        0        0     2056 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/lru_cache.py
+-rw-r--r--   0        0        0      918 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/math.py
+-rw-r--r--   0        0        0      715 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/measure_time.py
+-rw-r--r--   0        0        0      790 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/models.py
+-rw-r--r--   0        0        0     1585 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/recurring_task.py
+-rw-r--r--   0        0        0     4765 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/requests.py
+-rw-r--r--   0        0        0     2414 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/system.py
+-rw-r--r--   0        0        0     1429 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/wait.py
+-rw-r--r--   0        0        0      142 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/autoscaling/__init__.py
+-rw-r--r--   0        0        0    14883 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/autoscaling/autoscaled_pool.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/autoscaling/py.typed
+-rw-r--r--   0        0        0    15793 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/autoscaling/snapshotter.py
+-rw-r--r--   0        0        0     9293 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/autoscaling/system_status.py
+-rw-r--r--   0        0        0     5140 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/autoscaling/types.py
+-rw-r--r--   0        0        0      470 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/__init__.py
+-rw-r--r--   0        0        0     9143 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/base_dataset_client.py
+-rw-r--r--   0        0        0     1883 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/base_dataset_collection_client.py
+-rw-r--r--   0        0        0     3486 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/base_key_value_store_client.py
+-rw-r--r--   0        0        0     2025 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/base_key_value_store_collection_client.py
+-rw-r--r--   0        0        0     5622 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/base_request_queue_client.py
+-rw-r--r--   0        0        0     1992 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/base_request_queue_collection_client.py
+-rw-r--r--   0        0        0     2229 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/base_storage_client.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/py.typed
+-rw-r--r--   0        0        0      735 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/types.py
+-rw-r--r--   0        0        0      186 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/basic_crawler/__init__.py
+-rw-r--r--   0        0        0    28317 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/basic_crawler/basic_crawler.py
+-rw-r--r--   0        0        0     4696 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/basic_crawler/context_pipeline.py
+-rw-r--r--   0        0        0     2145 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/basic_crawler/errors.py
+-rw-r--r--   0        0        0     2279 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/basic_crawler/router.py
+-rw-r--r--   0        0        0     2820 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/basic_crawler/types.py
+-rw-r--r--   0        0        0       86 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/beautifulsoup_crawler/__init__.py
+-rw-r--r--   0        0        0     5574 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
+-rw-r--r--   0        0        0      524 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/beautifulsoup_crawler/types.py
+-rw-r--r--   0        0        0     1310 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/configuration.py
+-rw-r--r--   0        0        0      146 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/consts.py
+-rw-r--r--   0        0        0      272 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/enqueue_strategy.py
+-rw-r--r--   0        0        0       91 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/events/__init__.py
+-rw-r--r--   0        0        0     7211 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/events/event_manager.py
+-rw-r--r--   0        0        0     2682 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/events/local_event_manager.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/events/py.typed
+-rw-r--r--   0        0        0     1303 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/events/types.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/http_clients/__init__.py
+-rw-r--r--   0        0        0     2140 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/http_clients/base_http_client.py
+-rw-r--r--   0        0        0     5085 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/http_clients/httpx_client.py
+-rw-r--r--   0        0        0       59 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/http_crawler/__init__.py
+-rw-r--r--   0        0        0     2992 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/http_crawler/http_crawler.py
+-rw-r--r--   0        0        0      329 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/http_crawler/types.py
+-rw-r--r--   0        0        0     4719 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/log_config.py
+-rw-r--r--   0        0        0       55 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/__init__.py
+-rw-r--r--   0        0        0    15666 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/_creation_management.py
+-rw-r--r--   0        0        0    15684 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/dataset_client.py
+-rw-r--r--   0        0        0     2243 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/dataset_collection_client.py
+-rw-r--r--   0        0        0    15914 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/key_value_store_client.py
+-rw-r--r--   0        0        0     2333 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/key_value_store_collection_client.py
+-rw-r--r--   0        0        0    11113 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/memory_storage_client.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/py.typed
+-rw-r--r--   0        0        0    20944 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/request_queue_client.py
+-rw-r--r--   0        0        0     2316 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/request_queue_collection_client.py
+-rw-r--r--   0        0        0    13847 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/models.py
+-rw-r--r--   0        0        0     7393 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/proxy_configuration.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/py.typed
+-rw-r--r--   0        0        0       67 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/sessions/__init__.py
+-rw-r--r--   0        0        0     2430 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/sessions/models.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/sessions/py.typed
+-rw-r--r--   0        0        0     8084 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/sessions/session.py
+-rw-r--r--   0        0        0    11695 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/sessions/session_pool.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/statistics/__init__.py
+-rw-r--r--   0        0        0      980 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/statistics/error_tracker.py
+-rw-r--r--   0        0        0     3646 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/statistics/models.py
+-rw-r--r--   0        0        0    10880 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/statistics/statistics.py
+-rw-r--r--   0        0        0     1520 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storage_client_manager.py
+-rw-r--r--   0        0        0      150 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/__init__.py
+-rw-r--r--   0        0        0     8804 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/_creation_management.py
+-rw-r--r--   0        0        0     1090 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/base_storage.py
+-rw-r--r--   0        0        0    15956 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/dataset.py
+-rw-r--r--   0        0        0     4994 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/key_value_store.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/py.typed
+-rw-r--r--   0        0        0     2841 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/request_list.py
+-rw-r--r--   0        0        0     2755 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/request_provider.py
+-rw-r--r--   0        0        0    25708 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/request_queue.py
+-rw-r--r--   0        0        0      630 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/types.py
+-rw-r--r--   0        0        0    18689 1970-01-01 00:00:00.000000 crawlee-0.0.4b2/PKG-INFO
```

### Comparing `crawlee-0.0.4b1/LICENSE` & `crawlee-0.0.4b2/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/README.md` & `crawlee-0.0.4b2/README.md`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/pyproject.toml` & `crawlee-0.0.4b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "crawlee"
-version = "0.0.4b1"
+version = "0.0.4b2"
 description = "Crawlee for Python"
 authors = ["Apify Technologies s.r.o. <support@apify.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "crawlee", from = "src" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -79,14 +79,15 @@
 respx = "~0.21.0"
 ruff = "~0.4.0"
 types-aiofiles = "^23.2.0.20240106"
 types-beautifulsoup4 = "^4.12.0.20240229"
 types-colorama = "~0.4.15.20240106"
 types-psutil = "~5.9.5.20240205"
 types-python-dateutil = "^2.9.0.20240316"
+proxy-py = "^2.4.4"
 
 [tool.poetry.extras]
 beautifulsoup = ["beautifulsoup4", "lxml", "html5lib"]
 
 [tool.ruff]
 line-length = 120
```

### Comparing `crawlee-0.0.4b1/src/crawlee/_utils/blocked.py` & `crawlee-0.0.4b2/src/crawlee/_utils/blocked.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/_utils/byte_size.py` & `crawlee-0.0.4b2/src/crawlee/_utils/byte_size.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/_utils/crypto.py` & `crawlee-0.0.4b2/src/crawlee/_utils/crypto.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/_utils/data_processing.py` & `crawlee-0.0.4b2/src/crawlee/_utils/data_processing.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/_utils/env_vars.py` & `crawlee-0.0.4b2/src/crawlee/_utils/env_vars.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/_utils/file.py` & `crawlee-0.0.4b2/src/crawlee/_utils/file.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/_utils/globs.py` & `crawlee-0.0.4b2/src/crawlee/_utils/globs.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/_utils/lru_cache.py` & `crawlee-0.0.4b2/src/crawlee/_utils/lru_cache.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/_utils/math.py` & `crawlee-0.0.4b2/src/crawlee/_utils/math.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/_utils/measure_time.py` & `crawlee-0.0.4b2/src/crawlee/_utils/measure_time.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/_utils/models.py` & `crawlee-0.0.4b2/src/crawlee/_utils/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/_utils/recurring_task.py` & `crawlee-0.0.4b2/src/crawlee/_utils/recurring_task.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/_utils/requests.py` & `crawlee-0.0.4b2/src/crawlee/_utils/requests.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/_utils/system.py` & `crawlee-0.0.4b2/src/crawlee/_utils/system.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/_utils/wait.py` & `crawlee-0.0.4b2/src/crawlee/_utils/wait.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/autoscaling/autoscaled_pool.py` & `crawlee-0.0.4b2/src/crawlee/autoscaling/autoscaled_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/autoscaling/snapshotter.py` & `crawlee-0.0.4b2/src/crawlee/autoscaling/snapshotter.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/autoscaling/system_status.py` & `crawlee-0.0.4b2/src/crawlee/autoscaling/system_status.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/autoscaling/types.py` & `crawlee-0.0.4b2/src/crawlee/autoscaling/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/base_storage_client/base_dataset_client.py` & `crawlee-0.0.4b2/src/crawlee/base_storage_client/base_dataset_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/base_storage_client/base_dataset_collection_client.py` & `crawlee-0.0.4b2/src/crawlee/base_storage_client/base_dataset_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/base_storage_client/base_key_value_store_client.py` & `crawlee-0.0.4b2/src/crawlee/base_storage_client/base_key_value_store_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/base_storage_client/base_key_value_store_collection_client.py` & `crawlee-0.0.4b2/src/crawlee/base_storage_client/base_key_value_store_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/base_storage_client/base_request_queue_client.py` & `crawlee-0.0.4b2/src/crawlee/base_storage_client/base_request_queue_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/base_storage_client/base_request_queue_collection_client.py` & `crawlee-0.0.4b2/src/crawlee/base_storage_client/base_request_queue_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/base_storage_client/base_storage_client.py` & `crawlee-0.0.4b2/src/crawlee/base_storage_client/base_storage_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/base_storage_client/types.py` & `crawlee-0.0.4b2/src/crawlee/base_storage_client/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/basic_crawler/basic_crawler.py` & `crawlee-0.0.4b2/src/crawlee/basic_crawler/basic_crawler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Inspiration: https://github.com/apify/crawlee/blob/v3.7.3/packages/basic-crawler/src/internals/basic-crawler.ts
 from __future__ import annotations
 
 import tempfile
+from collections.abc import AsyncGenerator, Awaitable, Sequence
 from contextlib import AsyncExitStack
 from datetime import timedelta
 from functools import partial
 from logging import getLogger
-from typing import TYPE_CHECKING, Any, AsyncGenerator, Awaitable, Callable, Generic, Sequence, Union, cast
+from typing import TYPE_CHECKING, Any, Callable, Generic, Union, cast
 
 import httpx
 from tldextract import TLDExtract
 from typing_extensions import NotRequired, TypedDict, TypeVar, assert_never
 
 from crawlee import Glob
 from crawlee._utils.wait import wait_for
@@ -42,14 +43,15 @@
 from crawlee.statistics.statistics import Statistics
 from crawlee.storages.request_queue import RequestQueue
 
 if TYPE_CHECKING:
     import re
 
     from crawlee.http_clients.base_http_client import BaseHttpClient, HttpResponse
+    from crawlee.proxy_configuration import ProxyConfiguration, ProxyInfo
     from crawlee.sessions.session import Session
     from crawlee.statistics.models import FinalStatistics, StatisticsState
     from crawlee.storages.request_provider import RequestProvider
 
 TCrawlingContext = TypeVar('TCrawlingContext', bound=BasicCrawlingContext, default=BasicCrawlingContext)
 ErrorHandler = Callable[[TCrawlingContext, Exception], Awaitable[Union[Request, None]]]
 FailedRequestHandler = Callable[[TCrawlingContext, Exception], Awaitable[None]]
@@ -67,14 +69,15 @@
     max_request_retries: NotRequired[int]
     max_session_rotations: NotRequired[int]
     configuration: NotRequired[Configuration]
     request_handler_timeout: NotRequired[timedelta]
     session_pool: NotRequired[SessionPool]
     use_session_pool: NotRequired[bool]
     retry_on_blocked: NotRequired[bool]
+    proxy_configuration: NotRequired[ProxyConfiguration]
     statistics: NotRequired[Statistics[StatisticsState]]
     _context_pipeline: NotRequired[ContextPipeline[TCrawlingContext]]
 
 
 class BasicCrawler(Generic[TCrawlingContext]):
     """Provides a simple framework for parallel crawling of web pages.
 
@@ -96,14 +99,15 @@
         max_request_retries: int = 3,
         max_session_rotations: int = 10,
         configuration: Configuration | None = None,
         request_handler_timeout: timedelta = timedelta(minutes=1),
         session_pool: SessionPool | None = None,
         use_session_pool: bool = True,
         retry_on_blocked: bool = True,
+        proxy_configuration: ProxyConfiguration | None = None,
         statistics: Statistics | None = None,
         _context_pipeline: ContextPipeline[TCrawlingContext] | None = None,
     ) -> None:
         """Initialize the BasicCrawler.
 
         Args:
             request_provider: Provides requests to be processed
@@ -115,14 +119,15 @@
                 The crawler will automatically rotate the session in case of a proxy error or if it gets blocked by
                 the website.
             configuration: Crawler configuration
             request_handler_timeout: How long is a single request handler allowed to run
             use_session_pool: Enables using the session pool for crawling
             session_pool: A preconfigured `SessionPool` instance if you wish to use non-default configuration
             retry_on_blocked: If set to True, the crawler will try to automatically bypass any detected bot protection
+            proxy_configuration: A HTTP proxy configuration to be used for making requests
             statistics: A preconfigured `Statistics` instance if you wish to use non-default configuration
             _context_pipeline: Allows extending the request lifecycle and modifying the crawling context.
                 This parameter is meant to be used by child classes, not when BasicCrawler is instantiated directly.
         """
         self._router: Router[TCrawlingContext] | None = None
 
         if isinstance(cast(Router, request_handler), Router):
@@ -165,14 +170,15 @@
         )
 
         self._use_session_pool = use_session_pool
         self._session_pool = session_pool or SessionPool()
 
         self._retry_on_blocked = retry_on_blocked
 
+        self._proxy_configuration = proxy_configuration
         self._statistics = statistics or Statistics(
             event_manager=self._event_manager,
             log_message=f'{logger.name} request statistics',
         )
 
         self._running = False
         self._has_finished_before = False
@@ -207,14 +213,25 @@
             timeout=self._internal_timeout,
             timeout_message='Fetching a session from the pool timed out after '
             f'{self._internal_timeout.total_seconds()} seconds',
             max_retries=3,
             logger=logger,
         )
 
+    async def _get_proxy_info(self, request: Request, session: Session | None) -> ProxyInfo | None:
+        """Retrieve a new ProxyInfo object based on crawler configuration and the current request and session."""
+        if not self._proxy_configuration:
+            return None
+
+        return await self._proxy_configuration.new_proxy_info(
+            session_id=session.id if session else None,
+            request=request,
+            proxy_tier=None,
+        )
+
     async def get_request_provider(self) -> RequestProvider:
         """Return the configured request provider. If none is configured, open and return the default request queue."""
         if not self._request_provider:
             self._request_provider = await RequestQueue.open()
 
         return self._request_provider
 
@@ -407,23 +424,31 @@
 
         if self._failed_request_handler:
             try:
                 await self._failed_request_handler(crawling_context, error)
             except Exception as e:
                 raise UserDefinedErrorHandlerError('Exception thrown in user-defined failed request handler') from e
 
-    def _prepare_send_request_function(self, session: Session | None) -> SendRequestFunction:
+    def _prepare_send_request_function(
+        self,
+        session: Session | None,
+        proxy_info: ProxyInfo | None,
+    ) -> SendRequestFunction:
         async def send_request(
             url: str,
             *,
             method: str = 'get',
             headers: dict[str, str] | None = None,
         ) -> HttpResponse:
             return await self._http_client.send_request(
-                url, method=method, headers=httpx.Headers(headers), session=session
+                url,
+                method=method,
+                headers=httpx.Headers(headers),
+                session=session,
+                proxy_info=proxy_info,
             )
 
         return send_request
 
     async def _commit_request_handler_result(
         self, context: BasicCrawlingContext, result: RequestHandlerRunResult
     ) -> None:
@@ -457,35 +482,37 @@
         request_provider = await self.get_request_provider()
         return await request_provider.is_finished()
 
     async def __is_task_ready_function(self) -> bool:
         request_provider = await self.get_request_provider()
         return not await request_provider.is_empty()
 
-    async def __run_task_function(self) -> None:  # noqa: PLR0912
+    async def __run_task_function(self) -> None:
         request_provider = await self.get_request_provider()
 
         request = await wait_for(
             lambda: request_provider.fetch_next_request(),
             timeout=self._internal_timeout,
             timeout_message=f'Fetching next request failed after {self._internal_timeout.total_seconds()} seconds',
             logger=logger,
             max_retries=3,
         )
 
         if request is None:
             return
 
         session = await self._get_session()
+        proxy_info = await self._get_proxy_info(request, session)
         result = RequestHandlerRunResult()
 
         crawling_context = BasicCrawlingContext(
             request=request,
             session=session,
-            send_request=self._prepare_send_request_function(session),
+            proxy_info=proxy_info,
+            send_request=self._prepare_send_request_function(session, proxy_info),
             add_requests=result.add_requests,
         )
 
         statistics_id = request.id or request.unique_key
         self._statistics.record_request_processing_start(statistics_id)
 
         try:
```

### Comparing `crawlee-0.0.4b1/src/crawlee/basic_crawler/context_pipeline.py` & `crawlee-0.0.4b2/src/crawlee/basic_crawler/context_pipeline.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/basic_crawler/errors.py` & `crawlee-0.0.4b2/src/crawlee/basic_crawler/errors.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/basic_crawler/router.py` & `crawlee-0.0.4b2/src/crawlee/basic_crawler/router.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/basic_crawler/types.py` & `crawlee-0.0.4b2/src/crawlee/basic_crawler/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # ruff: noqa: TCH003
 from __future__ import annotations
 
 import re
+from collections.abc import Coroutine, Sequence
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any, Coroutine, Protocol, Sequence
+from typing import TYPE_CHECKING, Any, Protocol
 
 from typing_extensions import NotRequired, TypedDict, Unpack
 
 if TYPE_CHECKING:
     from crawlee import Glob
     from crawlee.enqueue_strategy import EnqueueStrategy
     from crawlee.http_clients.base_http_client import HttpResponse
     from crawlee.models import BaseRequestData, Request
+    from crawlee.proxy_configuration import ProxyInfo
     from crawlee.sessions.session import Session
 
 
 class AddRequestsFunctionKwargs(TypedDict):
     """Keyword arguments type for AddRequestsFunction."""
 
     limit: NotRequired[int]
@@ -60,14 +62,15 @@
 
 @dataclass(frozen=True)
 class BasicCrawlingContext:
     """Basic crawling context intended to be extended by crawlers."""
 
     request: Request
     session: Session | None
+    proxy_info: ProxyInfo | None
     send_request: SendRequestFunction
     add_requests: AddRequestsFunction
 
 
 class AddRequestsFunctionCall(AddRequestsFunctionKwargs):
     """Record of a call to `add_requests`."""
```

### Comparing `crawlee-0.0.4b1/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py` & `crawlee-0.0.4b2/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,19 +58,25 @@
                 ignore_http_error_status_codes=ignore_http_error_status_codes,
             ),
         )
 
         super().__init__(**kwargs)
 
     async def _make_http_request(self, context: BasicCrawlingContext) -> AsyncGenerator[HttpCrawlingContext, None]:
-        result = await self._http_client.crawl(context.request, context.session, self._statistics)
+        result = await self._http_client.crawl(
+            context.request,
+            context.session,
+            context.proxy_info,
+            self._statistics,
+        )
 
         yield HttpCrawlingContext(
             request=context.request,
             session=context.session,
+            proxy_info=context.proxy_info,
             send_request=context.send_request,
             add_requests=context.add_requests,
             http_response=result.http_response,
         )
 
     async def _handle_blocked_request(
         self, crawling_context: BeautifulSoupCrawlingContext
@@ -124,13 +130,14 @@
             kwargs.setdefault('strategy', EnqueueStrategy.SAME_HOSTNAME if uses_patterns else EnqueueStrategy.ALL)
 
             await context.add_requests(requests, **kwargs)
 
         yield BeautifulSoupCrawlingContext(
             request=context.request,
             session=context.session,
+            proxy_info=context.proxy_info,
             send_request=context.send_request,
             add_requests=context.add_requests,
             enqueue_links=enqueue_links,
             http_response=context.http_response,
             soup=soup,
         )
```

### Comparing `crawlee-0.0.4b1/src/crawlee/beautifulsoup_crawler/types.py` & `crawlee-0.0.4b2/src/crawlee/beautifulsoup_crawler/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/configuration.py` & `crawlee-0.0.4b2/src/crawlee/configuration.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/events/event_manager.py` & `crawlee-0.0.4b2/src/crawlee/events/event_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/events/local_event_manager.py` & `crawlee-0.0.4b2/src/crawlee/events/local_event_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/events/types.py` & `crawlee-0.0.4b2/src/crawlee/events/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/http_clients/base_http_client.py` & `crawlee-0.0.4b2/src/crawlee/http_clients/base_http_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Iterable, Protocol
 
 if TYPE_CHECKING:
     from httpx import Headers  # Type from `httpx` is used here because it is lightweight and convenient
 
     from crawlee.models import Request
+    from crawlee.proxy_configuration import ProxyInfo
     from crawlee.sessions.session import Session
     from crawlee.statistics.statistics import Statistics
 
 
 class HttpResponse(Protocol):
     """Response to an HTTP call."""
 
@@ -49,16 +50,23 @@
         self._ignore_http_error_status_codes = set(ignore_http_error_status_codes)
 
     @abstractmethod
     async def crawl(
         self,
         request: Request,
         session: Session | None,
+        proxy_info: ProxyInfo | None,
         statistics: Statistics,
     ) -> HttpCrawlingResult:
         """Perform a crawl of an URL."""
 
     @abstractmethod
     async def send_request(
-        self, url: str, *, method: str, headers: Headers | dict[str, str], session: Session | None = None
+        self,
+        url: str,
+        *,
+        method: str,
+        headers: Headers | dict[str, str],
+        session: Session | None,
+        proxy_info: ProxyInfo | None,
     ) -> HttpResponse:
         """Perform an HTTP request."""
```

### Comparing `crawlee-0.0.4b1/src/crawlee/http_clients/httpx_client.py` & `crawlee-0.0.4b2/src/crawlee/http_clients/httpx_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Iterable, cast
+from typing import TYPE_CHECKING, Optional, cast
 
 import httpx
 from typing_extensions import override
 
 from crawlee._utils.blocked import ROTATE_PROXY_ERRORS
 from crawlee.basic_crawler.errors import ProxyError
 from crawlee.http_clients.base_http_client import BaseHttpClient, HttpCrawlingResult, HttpResponse
 from crawlee.sessions.session import Session
 
 if TYPE_CHECKING:
+    from collections.abc import Iterable
+
     from crawlee.models import Request
+    from crawlee.proxy_configuration import ProxyInfo
     from crawlee.statistics.statistics import Statistics
 
+__all__ = ['HttpxClient']
+
 
 class HttpTransport(httpx.AsyncHTTPTransport):
     """A modified HTTP transport adapter that stores response cookies in a `Session` instead of the httpx client."""
 
     @override
     async def handle_async_request(
         self,
@@ -58,28 +63,42 @@
         ignore_http_error_status_codes: Iterable[int] = (),
     ) -> None:
         super().__init__(
             persist_cookies_per_session=persist_cookies_per_session,
             additional_http_error_status_codes=additional_http_error_status_codes,
             ignore_http_error_status_codes=ignore_http_error_status_codes,
         )
-        self._client = httpx.AsyncClient(transport=HttpTransport())
+
+        self._client_by_proxy_url = dict[Optional[str], httpx.AsyncClient]()
+
+    def _get_client(self, proxy_url: str | None) -> httpx.AsyncClient:
+        if proxy_url not in self._client_by_proxy_url:
+            self._client_by_proxy_url[proxy_url] = httpx.AsyncClient(transport=HttpTransport(), proxy=proxy_url)
+
+        return self._client_by_proxy_url[proxy_url]
 
     @override
-    async def crawl(self, request: Request, session: Session | None, statistics: Statistics) -> HttpCrawlingResult:
-        http_request = self._client.build_request(
+    async def crawl(
+        self,
+        request: Request,
+        session: Session | None,
+        proxy_info: ProxyInfo | None,
+        statistics: Statistics,
+    ) -> HttpCrawlingResult:
+        client = self._get_client(proxy_info.url if proxy_info else None)
+        http_request = client.build_request(
             method=request.method,
             url=request.url,
             headers=request.headers,
             cookies=session.cookies if session else None,
             extensions={'crawlee_session': session if self._persist_cookies_per_session else None},
         )
 
         try:
-            response = await self._client.send(http_request, follow_redirects=True)
+            response = await client.send(http_request, follow_redirects=True)
         except httpx.TransportError as e:
             if _is_proxy_error(e):
                 raise ProxyError from e
 
             raise
 
         statistics.register_status_code(response.status_code)
@@ -106,25 +125,28 @@
     @override
     async def send_request(
         self,
         url: str,
         *,
         method: str,
         headers: httpx.Headers | dict[str, str],
-        session: Session | None = None,
+        session: Session | None,
+        proxy_info: ProxyInfo | None,
     ) -> HttpResponse:
-        http_request = self._client.build_request(
+        client = self._get_client(proxy_info.url if proxy_info else None)
+
+        http_request = client.build_request(
             url=url,
             method=method,
             headers=headers,
             extensions={'crawlee_session': session if self._persist_cookies_per_session else None},
         )
 
         try:
-            response = await self._client.send(http_request)
+            response = await client.send(http_request)
         except httpx.TransportError as e:
             if _is_proxy_error(e):
                 raise ProxyError from e
 
             raise
 
         return response
```

### Comparing `crawlee-0.0.4b1/src/crawlee/http_crawler/http_crawler.py` & `crawlee-0.0.4b2/src/crawlee/http_crawler/http_crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,19 +47,25 @@
         )
 
         super().__init__(**kwargs)
 
     async def _make_http_request(
         self, crawling_context: BasicCrawlingContext
     ) -> AsyncGenerator[HttpCrawlingContext, None]:
-        result = await self._http_client.crawl(crawling_context.request, crawling_context.session, self._statistics)
+        result = await self._http_client.crawl(
+            crawling_context.request,
+            crawling_context.session,
+            crawling_context.proxy_info,
+            self._statistics,
+        )
 
         yield HttpCrawlingContext(
             request=crawling_context.request,
             session=crawling_context.session,
+            proxy_info=crawling_context.proxy_info,
             send_request=crawling_context.send_request,
             add_requests=crawling_context.add_requests,
             http_response=result.http_response,
         )
 
     async def _handle_blocked_request(
         self, crawling_context: HttpCrawlingContext
```

### Comparing `crawlee-0.0.4b1/src/crawlee/log_config.py` & `crawlee-0.0.4b2/src/crawlee/log_config.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/memory_storage_client/_creation_management.py` & `crawlee-0.0.4b2/src/crawlee/memory_storage_client/_creation_management.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/memory_storage_client/dataset_client.py` & `crawlee-0.0.4b2/src/crawlee/memory_storage_client/dataset_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/memory_storage_client/dataset_collection_client.py` & `crawlee-0.0.4b2/src/crawlee/memory_storage_client/dataset_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/memory_storage_client/key_value_store_client.py` & `crawlee-0.0.4b2/src/crawlee/memory_storage_client/key_value_store_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/memory_storage_client/key_value_store_collection_client.py` & `crawlee-0.0.4b2/src/crawlee/memory_storage_client/key_value_store_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/memory_storage_client/memory_storage_client.py` & `crawlee-0.0.4b2/src/crawlee/memory_storage_client/memory_storage_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/memory_storage_client/request_queue_client.py` & `crawlee-0.0.4b2/src/crawlee/memory_storage_client/request_queue_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/memory_storage_client/request_queue_collection_client.py` & `crawlee-0.0.4b2/src/crawlee/memory_storage_client/request_queue_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/models.py` & `crawlee-0.0.4b2/src/crawlee/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,14 +163,34 @@
         )
 
     @enqueue_strategy.setter
     def enqueue_strategy(self, new_enqueue_strategy: EnqueueStrategy) -> None:
         self.user_data.setdefault('__crawlee', {})
         self.user_data['__crawlee']['enqueueStrategy'] = str(new_enqueue_strategy)
 
+    @property
+    def last_proxy_tier(self) -> int | None:
+        """The last proxy tier used to process the request."""
+        return self.crawlee_data.last_proxy_tier
+
+    @last_proxy_tier.setter
+    def last_proxy_tier(self, new_value: int) -> None:
+        self.user_data.setdefault('__crawlee', {})
+        self.user_data['__crawlee']['lastProxyTier'] = new_value
+
+    @property
+    def forefront(self) -> bool:
+        """Should the request be enqueued at the start of the queue?"""
+        return self.crawlee_data.forefront
+
+    @forefront.setter
+    def forefront(self, new_value: bool) -> None:
+        self.user_data.setdefault('__crawlee', {})
+        self.user_data['__crawlee']['forefront'] = new_value
+
 
 class RequestState(Enum):
     """Crawlee-specific request handling state."""
 
     UNPROCESSED = 0
     BEFORE_NAV = 1
     AFTER_NAV = 2
@@ -193,14 +213,18 @@
     state: RequestState | None = None
     """Describes the request's current lifecycle state."""
 
     session_rotation_count: Annotated[int | None, Field(alias='sessionRotationCount')] = None
 
     skip_navigation: Annotated[bool, Field(alias='skipNavigation')] = False
 
+    last_proxy_tier: Annotated[int | None, Field(alias='lastProxyTier')] = None
+
+    forefront: Annotated[bool, Field()] = False
+
 
 class BaseStorageMetadata(BaseModel):
     """Base model for storage metadata."""
 
     model_config = ConfigDict(populate_by_name=True)
 
     id: Annotated[str, Field(alias='id')]
```

### Comparing `crawlee-0.0.4b1/src/crawlee/sessions/models.py` & `crawlee-0.0.4b2/src/crawlee/sessions/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/sessions/session.py` & `crawlee-0.0.4b2/src/crawlee/sessions/session.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/sessions/session_pool.py` & `crawlee-0.0.4b2/src/crawlee/sessions/session_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/statistics/error_tracker.py` & `crawlee-0.0.4b2/src/crawlee/statistics/error_tracker.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/statistics/models.py` & `crawlee-0.0.4b2/src/crawlee/statistics/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/statistics/statistics.py` & `crawlee-0.0.4b2/src/crawlee/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/storage_client_manager.py` & `crawlee-0.0.4b2/src/crawlee/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/storages/_creation_management.py` & `crawlee-0.0.4b2/src/crawlee/storages/_creation_management.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/storages/base_storage.py` & `crawlee-0.0.4b2/src/crawlee/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/storages/dataset.py` & `crawlee-0.0.4b2/src/crawlee/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/storages/key_value_store.py` & `crawlee-0.0.4b2/src/crawlee/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/storages/request_list.py` & `crawlee-0.0.4b2/src/crawlee/storages/request_list.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/storages/request_provider.py` & `crawlee-0.0.4b2/src/crawlee/storages/request_provider.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/storages/request_queue.py` & `crawlee-0.0.4b2/src/crawlee/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/src/crawlee/types.py` & `crawlee-0.0.4b2/src/crawlee/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b1/PKG-INFO` & `crawlee-0.0.4b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlee
-Version: 0.0.4b1
+Version: 0.0.4b2
 Summary: Crawlee for Python
 License: Apache-2.0
 Keywords: apify,automation,chrome,crawlee,crawler,headless,scraper,scraping
 Author: Apify Technologies s.r.o.
 Author-email: support@apify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crawlee Version: 0.0.4b1 Summary: Crawlee for
+Metadata-Version: 2.1 Name: crawlee Version: 0.0.4b2 Summary: Crawlee for
 Python License: Apache-2.0 Keywords:
 apify,automation,chrome,crawlee,crawler,headless,scraper,scraping Author: Apify
 Technologies s.r.o. Author-email: support@apify.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

