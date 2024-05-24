# Comparing `tmp/ml_pipeline_engine-1.6.0.tar.gz` & `tmp/ml_pipeline_engine-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_pipeline_engine-1.6.0.tar", max compression
+gzip compressed data, was "ml_pipeline_engine-2.0.0a0.tar", max compression
```

## Comparing `ml_pipeline_engine-1.6.0.tar` & `ml_pipeline_engine-2.0.0a0.tar`

### file list

```diff
@@ -1,69 +1,67 @@
--rw-r--r--   0        0        0      410 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/AUTHORS
--rw-r--r--   0        0        0     2570 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/LICENSE
--rw-r--r--   0        0        0     7578 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/README.md
--rw-r--r--   0        0        0        0 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/__init__.py
--rw-r--r--   0        0        0       93 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/enums.py
--rw-r--r--   0        0        0      165 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/errors.py
--rw-r--r--   0        0        0     1726 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/serializers.py
--rw-r--r--   0        0        0        0 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/store/__init__.py
--rw-r--r--   0        0        0      808 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/store/base.py
--rw-r--r--   0        0        0     2394 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/store/filesystem.py
--rw-r--r--   0        0        0      437 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/store/no_op.py
--rw-r--r--   0        0        0        0 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/base_nodes/__init__.py
--rw-r--r--   0        0        0      400 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/base_nodes/datasources.py
--rw-r--r--   0        0        0      359 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/base_nodes/feature.py
--rw-r--r--   0        0        0      354 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/base_nodes/ml_model.py
--rw-r--r--   0        0        0      779 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/base_nodes/processors.py
--rw-r--r--   0        0        0      381 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/base_nodes/vectorizer.py
--rw-r--r--   0        0        0      585 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/cache.py
--rw-r--r--   0        0        0     2781 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/chart.py
--rw-r--r--   0        0        0     1403 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/cli.py
--rw-r--r--   0        0        0       34 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/const.py
--rw-r--r--   0        0        0        0 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/context/__init__.py
--rw-r--r--   0        0        0     2212 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/context/dag.py
--rw-r--r--   0        0        0      207 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/__init__.py
--rw-r--r--   0        0        0     2378 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/dag.py
--rw-r--r--   0        0        0      444 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/enums.py
--rw-r--r--   0        0        0      325 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/graph.py
--rw-r--r--   0        0        0    22393 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/manager.py
--rw-r--r--   0        0        0      588 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/retrying.py
--rw-r--r--   0        0        0     3063 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/storage.py
--rw-r--r--   0        0        0      623 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/utils.py
--rw-r--r--   0        0        0        0 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag_builders/__init__.py
--rw-r--r--   0        0        0       31 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag_builders/annotation/__init__.py
--rw-r--r--   0        0        0    14609 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag_builders/annotation/builder.py
--rw-r--r--   0        0        0      531 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag_builders/annotation/errors.py
--rw-r--r--   0        0        0     5765 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag_builders/annotation/marks.py
--rw-r--r--   0        0        0     1796 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/decorators.py
--rw-r--r--   0        0        0     1439 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/events.py
--rw-r--r--   0        0        0      513 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/exceptions.py
--rw-r--r--   0        0        0      290 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/logs.py
--rw-r--r--   0        0        0     1124 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/module_loading.py
--rw-r--r--   0        0        0      156 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/node/__init__.py
--rw-r--r--   0        0        0      774 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/node/enums.py
--rw-r--r--   0        0        0      149 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/node/errors.py
--rw-r--r--   0        0        0     5943 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/node/node.py
--rw-r--r--   0        0        0      124 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/parallelism/__init__.py
--rw-r--r--   0        0        0     1883 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/parallelism/basic.py
--rw-r--r--   0        0        0     1945 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/parallelism/processes.py
--rw-r--r--   0        0        0      619 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/parallelism/threads.py
--rw-r--r--   0        0        0    11573 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/types.py
--rw-r--r--   0        0        0        0 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/__init__.py
--rw-r--r--   0        0        0     5385 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/dag.py
--rw-r--r--   0        0        0     2651 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/sample.py
--rw-r--r--   0        0        0     1214 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/schema.py
--rw-r--r--   0        0        0      597 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/utils.py
--rw-r--r--   0        0        0      524 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/asset-manifest.json
--rw-r--r--   0        0        0     3870 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/favicon.ico
--rw-r--r--   0        0        0      571 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/index.html
--rw-r--r--   0        0        0      366 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/manifest.json
--rw-r--r--   0        0        0   693682 2024-03-28 14:15:00.408856 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/css/main.fdcc84c5.css
--rw-r--r--   0        0        0  1073488 2024-03-28 14:15:00.412856 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/css/main.fdcc84c5.css.map
--rw-r--r--   0        0        0     4531 2024-03-28 14:15:00.412856 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/453.ae999f12.chunk.js
--rw-r--r--   0        0        0    10597 2024-03-28 14:15:00.412856 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/453.ae999f12.chunk.js.map
--rw-r--r--   0        0        0   750045 2024-03-28 14:15:00.416856 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js
--rw-r--r--   0        0        0     1629 2024-03-28 14:15:00.416856 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js.LICENSE.txt
--rw-r--r--   0        0        0  3506105 2024-03-28 14:15:00.428856 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js.map
--rw-r--r--   0        0        0     1247 2024-03-28 14:15:00.432856 ml_pipeline_engine-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     8640 1970-01-01 00:00:00.000000 ml_pipeline_engine-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0      410 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/AUTHORS
+-rw-r--r--   0        0        0     2570 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/LICENSE
+-rw-r--r--   0        0        0     1865 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/artifact_store/__init__.py
+-rw-r--r--   0        0        0       93 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/artifact_store/enums.py
+-rw-r--r--   0        0        0      165 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/artifact_store/errors.py
+-rw-r--r--   0        0        0     1751 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/artifact_store/serializers.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/artifact_store/store/__init__.py
+-rw-r--r--   0        0        0      910 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/artifact_store/store/base.py
+-rw-r--r--   0        0        0     2619 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/artifact_store/store/filesystem.py
+-rw-r--r--   0        0        0      437 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/artifact_store/store/no_op.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/base_nodes/__init__.py
+-rw-r--r--   0        0        0      414 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/base_nodes/datasources.py
+-rw-r--r--   0        0        0      402 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/base_nodes/feature.py
+-rw-r--r--   0        0        0      397 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/base_nodes/ml_model.py
+-rw-r--r--   0        0        0      909 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/base_nodes/processors.py
+-rw-r--r--   0        0        0      424 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/base_nodes/vectorizer.py
+-rw-r--r--   0        0        0      657 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/cache.py
+-rw-r--r--   0        0        0     2999 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/chart.py
+-rw-r--r--   0        0        0     1508 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/cli.py
+-rw-r--r--   0        0        0       34 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/const.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/context/__init__.py
+-rw-r--r--   0        0        0     2356 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/context/dag.py
+-rw-r--r--   0        0        0      153 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag/__init__.py
+-rw-r--r--   0        0        0     2486 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag/dag.py
+-rw-r--r--   0        0        0      409 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag/enums.py
+-rw-r--r--   0        0        0      226 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag/errors.py
+-rw-r--r--   0        0        0     1049 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag/graph.py
+-rw-r--r--   0        0        0    26337 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag/manager.py
+-rw-r--r--   0        0        0     3433 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag/storage.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag_builders/__init__.py
+-rw-r--r--   0        0        0       31 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag_builders/annotation/__init__.py
+-rw-r--r--   0        0        0    14240 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag_builders/annotation/builder.py
+-rw-r--r--   0        0        0      531 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag_builders/annotation/errors.py
+-rw-r--r--   0        0        0     5904 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag_builders/annotation/marks.py
+-rw-r--r--   0        0        0     1573 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/events.py
+-rw-r--r--   0        0        0      419 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/logs.py
+-rw-r--r--   0        0        0     1145 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/module_loading.py
+-rw-r--r--   0        0        0      156 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/node/__init__.py
+-rw-r--r--   0        0        0      774 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/node/enums.py
+-rw-r--r--   0        0        0      149 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/node/errors.py
+-rw-r--r--   0        0        0     5457 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/node/node.py
+-rw-r--r--   0        0        0      556 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/node/retrying.py
+-rw-r--r--   0        0        0      124 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/parallelism/__init__.py
+-rw-r--r--   0        0        0     2030 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/parallelism/basic.py
+-rw-r--r--   0        0        0     1963 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/parallelism/processes.py
+-rw-r--r--   0        0        0      610 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/parallelism/threads.py
+-rw-r--r--   0        0        0     8795 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/types.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/__init__.py
+-rw-r--r--   0        0        0     5484 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/dag.py
+-rw-r--r--   0        0        0     2779 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/sample.py
+-rw-r--r--   0        0        0     1322 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/schema.py
+-rw-r--r--   0        0        0      597 2024-05-24 08:37:05.284208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/utils.py
+-rw-r--r--   0        0        0      524 2024-05-24 08:37:05.288208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2024-05-24 08:37:05.288208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/favicon.ico
+-rw-r--r--   0        0        0      571 2024-05-24 08:37:05.288208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/index.html
+-rw-r--r--   0        0        0      366 2024-05-24 08:37:05.288208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/manifest.json
+-rw-r--r--   0        0        0   693682 2024-05-24 08:37:05.288208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/static/css/main.fdcc84c5.css
+-rw-r--r--   0        0        0  1073488 2024-05-24 08:37:05.292208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/static/css/main.fdcc84c5.css.map
+-rw-r--r--   0        0        0     4531 2024-05-24 08:37:05.292208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/static/js/453.ae999f12.chunk.js
+-rw-r--r--   0        0        0    10597 2024-05-24 08:37:05.292208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/static/js/453.ae999f12.chunk.js.map
+-rw-r--r--   0        0        0   750045 2024-05-24 08:37:05.296208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js
+-rw-r--r--   0        0        0     1629 2024-05-24 08:37:05.296208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js.LICENSE.txt
+-rw-r--r--   0        0        0  3506105 2024-05-24 08:37:05.312208 ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js.map
+-rw-r--r--   0        0        0     3698 2024-05-24 08:37:05.316208 ml_pipeline_engine-2.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0     2929 1970-01-01 00:00:00.000000 ml_pipeline_engine-2.0.0a0/PKG-INFO
```

### Comparing `ml_pipeline_engine-1.6.0/LICENSE` & `ml_pipeline_engine-2.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/serializers.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/artifact_store/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import io
 import json
 import pickle
 import typing as t
-from abc import ABC, abstractmethod
+from abc import ABC
+from abc import abstractmethod
 
 from ml_pipeline_engine.artifact_store.enums import DataFormat
 
 SerializableObjectT = t.Any
 
 
 class SerializerInitializationError(Exception):
@@ -61,13 +62,13 @@
 
         return JSONSerializer()
 
     def from_extension(self, extension: str) -> Serializer:
         try:
             fmt = DataFormat(extension)
         except ValueError:
-            raise SerializerInitializationError(f'No suitable serializer for {extension} extension')
+            raise SerializerInitializationError(f'No suitable serializer for {extension} extension') from None
 
         return self.from_data_format(fmt)
 
 
 serializer_factory = SerializerFactory()
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/store/base.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/artifact_store/store/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import typing as t
-from abc import ABCMeta, abstractmethod
+from abc import ABCMeta
+from abc import abstractmethod
 
 from ml_pipeline_engine.artifact_store.enums import DataFormat
-from ml_pipeline_engine.types import NodeId, PipelineContextLike
+from ml_pipeline_engine.types import NodeId
+from ml_pipeline_engine.types import PipelineContextLike
 
 
 class ArtifactStore(metaclass=ABCMeta):
-    def __init__(self, ctx: PipelineContextLike, *args, **kwargs):
+    def __init__(self, ctx: PipelineContextLike, *_: t.Any, **__: t.Any) -> None:
         self.ctx = ctx
 
     @abstractmethod
     async def save(self, node_id: NodeId, data: t.Any) -> None:
         ...
 
     @abstractmethod
     async def load(self, node_id: NodeId) -> t.Any:
         ...
 
 
 class SerializedArtifactStore(ArtifactStore, metaclass=ABCMeta):
-    def __init__(self, ctx: PipelineContextLike, *args, **kwargs):
-        super().__init__(ctx=ctx, *args, **kwargs)
+    def __init__(self, ctx: PipelineContextLike, *args: t.Any, **kwargs: t.Any) -> None:
+        super().__init__(ctx=ctx, *args, **kwargs)  # noqa: B026
 
     @abstractmethod
     async def save(self, node_id: NodeId, data: t.Any, fmt: DataFormat = None) -> None:
         ...
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/store/filesystem.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/artifact_store/store/filesystem.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,69 @@
 import functools
-import os
 import typing as t
 import warnings
 from enum import Enum
 from pathlib import Path
 
 from ml_pipeline_engine.artifact_store.enums import DataFormat
-from ml_pipeline_engine.artifact_store.errors import (
-    ArtifactAlreadyExists,
-    ArtifactDoesNotExist,
-)
+from ml_pipeline_engine.artifact_store.errors import ArtifactAlreadyExists
+from ml_pipeline_engine.artifact_store.errors import ArtifactDoesNotExist
 from ml_pipeline_engine.artifact_store.serializers import serializer_factory
 from ml_pipeline_engine.artifact_store.store.base import SerializedArtifactStore
-from ml_pipeline_engine.types import NodeId, NodeResultT, PipelineContextLike
+from ml_pipeline_engine.types import NodeId
+from ml_pipeline_engine.types import NodeResultT
+from ml_pipeline_engine.types import PipelineContextLike
 
 
 class ArtifactFileAlreadyExists(ArtifactAlreadyExists):
     pass
 
 
 class ArtifactFileDoesNotExist(ArtifactDoesNotExist):
     pass
 
 
-def dont_use_for_prod(func: t.Callable):
+def dont_use_for_prod(func: t.Callable) -> t.Callable[..., t.Any]:
 
     @functools.wraps(func)
-    async def wrap(*args, **kwargs):
-        warnings.warn(f'Функция {func.__name__} предназначена для локального использования')
+    async def wrap(*args: t.Any, **kwargs: t.Any) -> t.Any:
+        warnings.warn(f'Функция {func.__name__} предназначена для локального использования', stacklevel=1)
         return await func(*args, **kwargs)
 
     return wrap
 
 
 class FileSystemArtifactStore(SerializedArtifactStore):
-    def __init__(self, ctx: PipelineContextLike, artifact_dir: t.Union[Path, str]):
+    def __init__(self, ctx: PipelineContextLike, artifact_dir: t.Union[Path, str]) -> None:
         super().__init__(ctx)
 
         self.artifact_dir = Path(artifact_dir)
 
     def _ensure_dir(self) -> Path:
         model_name = self.ctx.model_name.value if isinstance(self.ctx.model_name, Enum) else self.ctx.model_name
         path = Path(self.artifact_dir / model_name / str(self.ctx.pipeline_id))
 
         if not path.exists():
-            os.makedirs(path)
+            path.mkdir(parents=True)
 
         return path
 
     def _get_glob(self, node_id: NodeId) -> t.List[Path]:
         return list(Path(self._ensure_dir()).glob(f'{node_id}.*'))
 
     @dont_use_for_prod
     async def save(self, node_id: NodeId, data: NodeResultT, fmt: DataFormat = DataFormat.PICKLE) -> None:
         if len(self._get_glob(node_id)):
             raise ArtifactFileAlreadyExists(f'Artifact file for {node_id} already exists')
 
-        with open(self._ensure_dir() / f'{node_id}.{fmt.value}', 'wb') as file:
+        with Path(self._ensure_dir() / f'{node_id}.{fmt.value}').open('wb') as file:  # noqa: ASYNC101
             serializer_factory.from_data_format(fmt).dump(data, file)
 
     @dont_use_for_prod
     async def load(self, node_id: NodeId) -> NodeResultT:
         glob = self._get_glob(node_id)
 
         if not len(glob):
             raise ArtifactFileDoesNotExist(f'Artifact file for {node_id} does not exist')
 
-        with open(glob[0], 'rb') as file:
+        with Path(glob[0]).open('rb') as file:  # noqa: ASYNC101
             return serializer_factory.from_extension(glob[0].suffix[1:]).load(file)
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/chart.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/chart.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import typing as t
-from dataclasses import dataclass, field
+from dataclasses import dataclass
+from dataclasses import field
 
 from ml_pipeline_engine.context import dag as dag_ctx
 from ml_pipeline_engine.node import generate_pipeline_id
-from ml_pipeline_engine.types import (
-    ArtifactStoreLike,
-    DAGLike,
-    EventManagerLike,
-    ModelName,
-    NodeLike,
-    PipelineId,
-    PipelineResult,
-)
+from ml_pipeline_engine.types import ArtifactStoreLike
+from ml_pipeline_engine.types import DAGLike
+from ml_pipeline_engine.types import EventManagerLike
+from ml_pipeline_engine.types import ModelName
+from ml_pipeline_engine.types import NodeLike
+from ml_pipeline_engine.types import PipelineId
+from ml_pipeline_engine.types import PipelineResult
 
 NodeResultT = t.TypeVar('NodeResultT')
 
 Entrypoint = t.Optional[t.Union[NodeLike[NodeResultT], DAGLike[NodeResultT]]]
 
 
 @dataclass(frozen=True, repr=False)
@@ -81,10 +80,10 @@
 
     entrypoint: Entrypoint = None
 
     def run(
         self,
         pipeline_id: t.Optional[PipelineId] = None,
         input_kwargs: t.Optional[t.Dict[str, t.Any]] = None,
-        meta: t.Dict[str, t.Any] = None,
+        meta: t.Optional[t.Dict[str, t.Any]] = None,
     ) -> NodeResultT:
         raise NotImplementedError('Unable to run this kind of pipeline')
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/cli.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import pathlib
-from typing import Optional, List, Tuple
+from typing import List
+from typing import Optional
+from typing import Tuple
 
 import click
 
 from ml_pipeline_engine.node.enums import NodeType
 
 
 @click.group()
-def main():
+def main() -> None:
     """Cli"""
 
 
 @main.command()
 @click.option('--dag_path', help='Dotted path to a dag', required=True)
 @click.option('--dag_name', default='Dag', help='Tech name for the dag')
 @click.option('--dag_verbose_name', default='Dag', help='Title for the dag')
@@ -21,19 +23,21 @@
 def build_static(
     dag_path: str,
     dag_name: str,
     dag_verbose_name: str,
     target_dir: pathlib.Path,
     repo_link: Optional[str] = None,
     color: Optional[List[Tuple[NodeType, str]]] = None,
-):
+) -> None:
     """Build static for a dag by path"""
 
     import importlib
-    from ml_pipeline_engine.visualization.dag import build_static, GraphConfigImpl
+
+    from ml_pipeline_engine.visualization.dag import GraphConfigImpl
+    from ml_pipeline_engine.visualization.dag import build_static
 
     module, dag_object_name = dag_path.rsplit(':', 1)
     module = importlib.import_module(module)
 
     config = GraphConfigImpl(getattr(module, dag_object_name)).generate(
         node_colors=dict(color),
         repo_link=repo_link,
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/context/dag.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/context/dag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,62 @@
 import typing as t
 
 from ml_pipeline_engine.artifact_store.store.no_op import NoOpArtifactStore
-from ml_pipeline_engine.cache import Cache
 from ml_pipeline_engine.events import EventSourceMixin
 from ml_pipeline_engine.module_loading import get_instance
 from ml_pipeline_engine.node import generate_pipeline_id
-from ml_pipeline_engine.types import (
-    ArtifactStoreLike,
-    CaseResult,
-    EventManagerLike,
-    ModelName,
-    NodeId,
-    PipelineChartLike,
-    PipelineId,
-)
+from ml_pipeline_engine.types import ArtifactStoreLike
+from ml_pipeline_engine.types import EventManagerLike
+from ml_pipeline_engine.types import ModelName
+from ml_pipeline_engine.types import NodeId
+from ml_pipeline_engine.types import PipelineChartLike
+from ml_pipeline_engine.types import PipelineId
 
 
 class DAGPipelineContext(EventSourceMixin):
     """
     Контекст выполнения пайплайна ML-модели
     """
 
     def __init__(
         self,
         chart: PipelineChartLike,
         pipeline_id: PipelineId = None,
-        input_kwargs: t.Dict[str, t.Any] = None,
-        meta: t.Dict[str, t.Any] = None,
-    ):
+        input_kwargs: t.Optional[t.Dict[str, t.Any]] = None,
+        meta: t.Optional[t.Dict[str, t.Any]] = None,
+    ) -> None:
         self.chart = chart
         self.pipeline_id = pipeline_id if pipeline_id is not None else generate_pipeline_id()
         self.input_kwargs = input_kwargs if input_kwargs is not None else {}
         self.meta = meta if meta is not None else {}
         self.artifact_store: ArtifactStoreLike = get_instance(
-            cls=self.chart.artifact_store or NoOpArtifactStore, ctx=self
+            cls=self.chart.artifact_store or NoOpArtifactStore, ctx=self,
         )
 
         self._event_managers = [get_instance(cls) for cls in self.chart.event_managers]
 
     async def save_node_result(self, node_id: NodeId, data: t.Any) -> None:
         await self.artifact_store.save(node_id=node_id, data=data)
 
     @property
     def model_name(self) -> ModelName:
         return self.chart.model_name
 
     def _get_event_managers(self) -> t.List[EventManagerLike]:
         return self._event_managers
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'<{self.__class__.__name__} model_name="{self.chart.model_name}" pipeline_id="{self.pipeline_id}">'
 
 
 def create_context_from_chart(
     chart: PipelineChartLike,
     input_kwargs: t.Dict[str, t.Any],
     pipeline_id: PipelineId = None,
-    meta: t.Dict[str, t.Any] = None,
+    meta: t.Optional[t.Dict[str, t.Any]] = None,
 ) -> DAGPipelineContext:
     """
     Создать контекст выполнения пайплайна ML-модели
     """
 
     return DAGPipelineContext(
         pipeline_id=pipeline_id, chart=chart, input_kwargs=input_kwargs, meta=meta,
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/dag.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag/dag.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,71 @@
 import pathlib
+import typing as t
 from dataclasses import dataclass
-from typing import Dict, Type, Optional, Union
 
 from ml_pipeline_engine.dag.graph import DiGraph
-from ml_pipeline_engine.dag.manager import DAGRunConcurrentManager, DAGConcurrentManagerLock
-from ml_pipeline_engine.dag.retrying import DagRetryPolicy
-from ml_pipeline_engine.parallelism import (
-    process_pool_registry,
-    threads_pool_registry,
-)
-from ml_pipeline_engine.types import (
-    DAGLike,
-    DAGRunManagerLike,
-    NodeId,
-    NodeResultT,
-    NodeLike,
-    PipelineContextLike,
-    RetryPolicyLike,
-)
+from ml_pipeline_engine.dag.manager import DAGRunConcurrentManager
+from ml_pipeline_engine.node.retrying import NodeRetryPolicy
+from ml_pipeline_engine.parallelism import process_pool_registry
+from ml_pipeline_engine.parallelism import threads_pool_registry
+from ml_pipeline_engine.types import DAGLike
+from ml_pipeline_engine.types import DAGRunManagerLike
+from ml_pipeline_engine.types import NodeId
+from ml_pipeline_engine.types import NodeLike
+from ml_pipeline_engine.types import NodeResultT
+from ml_pipeline_engine.types import PipelineContextLike
+from ml_pipeline_engine.types import RetryPolicyLike
 
 
 @dataclass()
 class DAG(DAGLike):
     graph: DiGraph
     input_node: NodeId
     output_node: NodeId
     is_process_pool_needed: bool
     is_thread_pool_needed: bool
-    node_map: Dict[NodeId, NodeLike]
-    retry_policy: Type[RetryPolicyLike] = DagRetryPolicy
-    run_manager: Type[DAGRunManagerLike] = DAGRunConcurrentManager
+    node_map: t.Dict[NodeId, NodeLike]
+    retry_policy: t.Type[RetryPolicyLike] = NodeRetryPolicy
+    run_manager: t.Type[DAGRunManagerLike] = DAGRunConcurrentManager
 
     def _start_runtime_validation(self) -> None:
         self._validate_pool_executors()
 
     def _validate_pool_executors(self) -> None:
         if self.is_thread_pool_needed:
             threads_pool_registry.is_ready()
 
         if self.is_process_pool_needed:
             process_pool_registry.is_ready()
 
     async def run(self, ctx: PipelineContextLike) -> NodeResultT:
         self._start_runtime_validation()
 
-        run_manager = self.run_manager(
-            lock_manager=DAGConcurrentManagerLock(
-                self.node_map.keys(),
-            ),
-            dag=self,
-            ctx=ctx,
-        )
-
+        run_manager = self.run_manager(dag=self, ctx=ctx)
         return await run_manager.run()
 
-    def visualize(  # noqa
+    def visualize(  # type: ignore
         self,
         name: str,
-        verbose_name: Optional[str] = None,
-        target_dir: Optional[Union[pathlib.Path, str]] = None,
-        **kwargs,
+        verbose_name: t.Optional[str] = None,
+        target_dir: t.Optional[t.Union[pathlib.Path, str]] = None,
+        **kwargs: t.Any,
     ) -> None:
         """
-        Create a static for graph visualization
+        Create static files for graph visualization
 
         Args:
             name: Tech name for the dag
             verbose_name: Dag title
             target_dir: Target dir for static
             **kwargs: Graph config kwargs
         """
 
-        from ml_pipeline_engine.visualization.dag import GraphConfigImpl, build_static
+        from ml_pipeline_engine.visualization.dag import GraphConfigImpl
+        from ml_pipeline_engine.visualization.dag import build_static
 
         config = GraphConfigImpl(self).generate(
             name=name or 'Dag',
             verbose_name=verbose_name,
             **kwargs,
         )
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/storage.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag/storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import typing as t
 from collections import UserDict
-from dataclasses import dataclass, field
+from dataclasses import dataclass
+from dataclasses import field
 
-from ml_pipeline_engine.types import HiddenDictLike, DAGNodeStorageLike, NodeId
+from ml_pipeline_engine.types import NodeId
 
 
-class HiddenDict(UserDict, HiddenDictLike):
+class HiddenDict(UserDict):
+    """
+    Dict object that can hide some keys until they are set again
+    """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
         super().__init__(*args, **kwargs)
         self._hidden_keys: set = set()
 
     def get(self, key: t.Any, with_hidden: bool = True) -> t.Any:
         if with_hidden is False and key in self._hidden_keys:
             return None
 
         return super().get(key)
 
-    def exists(self, key, with_hidden: bool = True) -> bool:
+    def exists(self, key: t.Any, with_hidden: bool = True) -> bool:
         if with_hidden is False and key in self._hidden_keys:
             return False
 
         return key in self
 
     def set(self, key: t.Any, value: t.Any) -> None:
 
@@ -34,32 +38,40 @@
         self._hidden_keys.add(key)
 
     def delete(self, key: t.Any) -> None:
         self.pop(key)
 
 
 @dataclass
-class DAGNodeStorage(DAGNodeStorageLike):
+class DAGNodeStorage:
+    """
+    A container for all information about node results
+    """
+
     node_results: HiddenDict = field(default_factory=HiddenDict)
     processed_nodes: HiddenDict = field(default_factory=HiddenDict)
     switch_results: HiddenDict = field(default_factory=HiddenDict)
     recurrent_subgraph: HiddenDict = field(default_factory=HiddenDict)
+    waiting_list: HiddenDict = field(default_factory=HiddenDict)
 
     def set_node_result(self, node_id: NodeId, data: t.Any) -> None:
         self.node_results.set(node_id, data)
 
     def get_node_result(self, node_id: NodeId, with_hidden: bool = False) -> t.Any:
         return self.node_results.get(node_id, with_hidden)
 
     def hide_node_result(self, node_id: NodeId) -> None:
         self.node_results.hide(node_id)
 
     def exists_node_result(self, node_id: NodeId, with_hidden: bool = False) -> bool:
         return self.node_results.exists(node_id, with_hidden)
 
+    def exists_node_error(self, node_id: NodeId, with_hidden: bool = False) -> bool:
+        return isinstance(self.node_results.get(node_id, with_hidden), BaseException)
+
     def set_switch_result(self, node_id: NodeId, data: t.Any) -> t.Any:
         self.switch_results.set(node_id, data)
 
     def get_switch_result(self, node_id: NodeId, with_hidden: bool = False) -> t.Any:
         return self.switch_results.get(node_id, with_hidden)
 
     def set_node_as_processed(self, node_id: NodeId) -> None:
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag_builders/annotation/builder.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag_builders/annotation/builder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,49 @@
 import copy
 import inspect
 import typing as t
 from collections import deque
 
-from ml_pipeline_engine.dag import DAG, EdgeField, NodeField
+from ml_pipeline_engine.dag import DAG
+from ml_pipeline_engine.dag import EdgeField
+from ml_pipeline_engine.dag import NodeField
 from ml_pipeline_engine.dag.graph import DiGraph
-from ml_pipeline_engine.dag.utils import get_connected_subgraph
+from ml_pipeline_engine.dag.graph import get_connected_subgraph
 from ml_pipeline_engine.dag_builders.annotation import errors
-from ml_pipeline_engine.dag_builders.annotation.marks import (
-    InputGenericMark,
-    InputMark,
-    InputOneOfMark,
-    RecurrentSubGraphMark,
-    SwitchCaseMark,
-)
-from ml_pipeline_engine.node import (
-    NodeTag,
-    NodeType,
-    generate_node_id,
-    get_callable_run_method,
-    get_node_id,
-)
-from ml_pipeline_engine.types import (
-    DAGLike,
-    NodeBase,
-    NodeId,
-    NodeLike,
-    RecurrentProtocol,
-)
+from ml_pipeline_engine.dag_builders.annotation.marks import InputGenericMark
+from ml_pipeline_engine.dag_builders.annotation.marks import InputMark
+from ml_pipeline_engine.dag_builders.annotation.marks import InputOneOfMark
+from ml_pipeline_engine.dag_builders.annotation.marks import RecurrentSubGraphMark
+from ml_pipeline_engine.dag_builders.annotation.marks import SwitchCaseMark
+from ml_pipeline_engine.node import NodeTag
+from ml_pipeline_engine.node import NodeType
+from ml_pipeline_engine.node import generate_node_id
+from ml_pipeline_engine.node import get_callable_run_method
+from ml_pipeline_engine.node import get_node_id
+from ml_pipeline_engine.types import DAGLike
+from ml_pipeline_engine.types import NodeBase
+from ml_pipeline_engine.types import NodeId
+from ml_pipeline_engine.types import NodeLike
+from ml_pipeline_engine.types import RecurrentProtocol
 
 __all__ = [
     'build_dag',
     'build_dag_single',
 ]
 
 KwargName = str
 
 NodeInputSpec = t.Tuple[KwargName, t.Union[InputMark, SwitchCaseMark]]
 
 NodeResultT = t.TypeVar('NodeResultT')
 
 
 class AnnotationDAGBuilder:
-    def __init__(self):
-        self._dag = DiGraph()
+    def __init__(self) -> None:
+        self._dag = DiGraph(name='main-graph')
         self._node_map: t.Dict[NodeId, NodeLike] = dict()
         self._recurrent_sub_graphs: t.List[t.Tuple[NodeId, NodeId]] = []
         self._synthetic_nodes: t.List[NodeId] = []
 
     @staticmethod
     def _check_annotations(obj: t.Any) -> None:
         """
@@ -98,15 +94,15 @@
         """
         Получение меток зависимостей для входных kwarg-ов узла
         """
 
         node = get_callable_run_method(node)
 
         inputs = []
-        for name, annotation in node.__annotations__.items():  # noqa
+        for name, annotation in node.__annotations__.items():
 
             if isinstance(annotation, InputGenericMark):
                 raise errors.NonRedefinedGenericTypeError(
                     f'Для использования узлов общего назначения необходимо их переопределение для целевого графа. '
                     f'param_name={name}, node={node}, ',
                 )
 
@@ -120,15 +116,15 @@
     def _add_node_to_map(self, node: NodeLike) -> None:
         """
         Добавление узла в мэппинг "Имя узла -> Класс/функция узла"
         """
 
         self._node_map[get_node_id(node)] = node
 
-    def _add_node_pair_to_dag(self, source_node_id: NodeId, dest_node_id: NodeId, **edge_data) -> None:
+    def _add_node_pair_to_dag(self, source_node_id: NodeId, dest_node_id: NodeId, **edge_data: t.Any) -> None:
         """
         Добавить в граф пару узлов, связанных ребром
         """
 
         self._dag.add_node(source_node_id)
         self._dag.add_node(dest_node_id)
 
@@ -192,61 +188,54 @@
                         ),
                     )
                     _set_visited(input_mark.dest_node)
 
                 if isinstance(input_mark, InputOneOfMark):
                     first_node_in_pool = input_mark.nodes[0]
                     synthetic_node_id = generate_node_id(NodeType.input_one_of.value, get_node_id(first_node_in_pool))
-                    self._dag.add_node(synthetic_node_id, **{NodeField.is_first_success: True})
+
+                    node_id_list = [get_node_id(node) for node in input_mark.nodes]
+
+                    self._dag.add_node(
+                        synthetic_node_id, **{NodeField.is_oneof_head: True, NodeField.oneof_nodes: node_id_list},
+                    )
                     self._dag.add_edge(get_node_id(input_node), synthetic_node_id)
 
-                    node_list = input_mark.nodes
-                    for idx, node in enumerate(node_list):
-                        self._add_node_to_map(node)
-                        self._dag.add_node(get_node_id(node), **{NodeField.is_first_success_pool: True})
-
-                        if idx + 1 < len(node_list):
-                            self._dag.add_edge(
-                                get_node_id(node),
-                                get_node_id(node_list[idx + 1]),
-                                **{EdgeField.is_first_success: get_node_id(first_node_in_pool)},
-                            )
-                        else:
-                            self._dag.add_edge(
-                                get_node_id(node),
-                                synthetic_node_id,
-                                **{EdgeField.is_first_success: get_node_id(first_node_in_pool)},
-                            )
+                    for idx, node_id in enumerate(node_id_list):
 
-                        _set_visited(node)
+                        self._add_node_to_map(input_mark.nodes[idx])
+                        self._dag.add_node(node_id, **{NodeField.is_oneof_child: True})
+                        self._dag.add_edge(node_id, synthetic_node_id)
+
+                        _set_visited(input_mark.nodes[idx])
 
                     self._synthetic_nodes.append(synthetic_node_id)
                     self._dag.add_edge(
-                        synthetic_node_id, get_node_id(current_node), **{EdgeField.kwarg_name: kwarg_name}
+                        synthetic_node_id, get_node_id(current_node), **{EdgeField.kwarg_name: kwarg_name},
                     )
 
                 if isinstance(input_mark, InputMark):
                     self._add_node_to_map(input_mark.node)
                     self._add_node_pair_to_dag(
-                        get_node_id(input_mark.node), get_node_id(current_node), **{EdgeField.kwarg_name: kwarg_name}
+                        get_node_id(input_mark.node), get_node_id(current_node), **{EdgeField.kwarg_name: kwarg_name},
                     )
                     _set_visited(input_mark.node)
 
                 if isinstance(input_mark, SwitchCaseMark):
 
                     switch_node_id = generate_node_id(NodeType.switch.value, input_mark.name)
 
                     self._add_node_to_map(input_mark.switch)
                     self._add_switch_node(switch_node_id, get_node_id(input_mark.switch))
                     _set_visited(input_mark.switch)
 
                     for case_branch, case_node in input_mark.cases:
                         self._add_node_to_map(case_node)
                         self._dag.add_edge(
-                            get_node_id(case_node), switch_node_id, **{EdgeField.case_branch: case_branch}
+                            get_node_id(case_node), switch_node_id, **{EdgeField.case_branch: case_branch},
                         )
                         _set_visited(case_node)
 
                     self._dag.add_edge(switch_node_id, get_node_id(current_node), **{EdgeField.kwarg_name: kwarg_name})
                     self._synthetic_nodes.append(switch_node_id)
 
     def _validate_recurrent_node_base_classes(self) -> None:
@@ -275,27 +264,20 @@
 
         for source, dest in self._recurrent_sub_graphs:
             if source in self._synthetic_nodes or dest in self._synthetic_nodes:
                 continue
 
             method = get_callable_run_method(self._node_map[source])
 
-            if 'additional_data' not in method.__annotations__:  # noqa
+            if 'additional_data' not in method.__annotations__:
                 raise errors.IncorrectParamsRecurrentNode(
                     f'В {method} отсутствует системный параметр "additional_data" для получения данных от узла, '
                     'который может перезапустить подграф',
                 )
 
-            dest_node = self._node_map[dest]
-            if not dest_node.use_default:
-                raise errors.IncorrectParamsRecurrentNode(
-                    f'Для участия в рекуррентном подграфе {dest_node} должен устанавливать параметр use_default=True. '
-                    'Дополнительно должен быть переопределен метод get_default()'
-                )
-
     def _validate_graph(self) -> None:
         """
         Метод для валидации построенного графа
         """
 
         self._validate_recurrent_node_base_classes()
         self._validate_recurrent_nodes_params()
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag_builders/annotation/errors.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag_builders/annotation/errors.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag_builders/annotation/marks.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/dag_builders/annotation/marks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import typing as t
 from dataclasses import dataclass
 
-from ml_pipeline_engine.types import CaseLabel, NodeLike
+from ml_pipeline_engine.types import CaseLabel
+from ml_pipeline_engine.types import NodeLike
 
 NodeResultT = t.TypeVar('NodeResultT')
 
 
 @dataclass(frozen=True)
 class InputGenericMark:
     node: NodeLike[t.Any]
@@ -17,61 +18,61 @@
 
 
 @dataclass(frozen=True)
 class InputOneOfMark:
     nodes: t.List[NodeLike[t.Any]]
 
 
-def InputOneOf(nodes: t.List[NodeLike[NodeResultT]]) -> t.Type[NodeResultT]:  # noqa
+def InputOneOf(nodes: t.List[NodeLike[NodeResultT]]) -> t.Type[NodeResultT]:  # noqa:  N802,RUF100
     """
     Принимает список нод, возвращает результат первой успешно выполненной ноды
     """
     return t.cast(t.Any, InputOneOfMark(nodes))
 
 
-def InputGeneric(node: NodeLike[NodeResultT]) -> t.Type[NodeResultT]:  # noqa
+def InputGeneric(node: NodeLike[NodeResultT]) -> t.Type[NodeResultT]:  # noqa:  N802,RUF100
     return t.cast(t.Any, InputGenericMark(node))
 
 
-def Input(node: NodeLike[NodeResultT]) -> t.Type[NodeResultT]:  # noqa
+def Input(node: NodeLike[NodeResultT]) -> t.Type[NodeResultT]:  # noqa:  N802,RUF100
     return t.cast(t.Any, InputMark(node))
 
 
 @dataclass(frozen=True)
 class GenericInputMark:
     node: NodeLike[t.Any]
 
 
-def GenericInput(node: NodeLike[NodeResultT]) -> t.Type[NodeResultT]:  # noqa
+def GenericInput(node: NodeLike[NodeResultT]) -> t.Type[NodeResultT]:  # noqa:  N802,RUF100
     return t.cast(t.Any, GenericInputMark(node))
 
 
 @dataclass(frozen=True)
 class SwitchCaseMark:
     switch: NodeLike[t.Any]
     cases: t.List[t.Tuple[str, NodeLike]]
     name: str
 
 
-def SwitchCase(  # noqa
+def SwitchCase(  # noqa:  N802,RUF100
     switch: NodeLike[t.Any],
     cases: t.List[t.Tuple[CaseLabel, NodeLike[NodeResultT]]],
-    name=None,
+    name: t.Optional[str] = None,
 ) -> t.Type[NodeResultT]:
     return t.cast(t.Any, SwitchCaseMark(switch, cases, name))
 
 
 @dataclass(frozen=True)
 class RecurrentSubGraphMark:
     start_node: NodeLike[NodeResultT]
     dest_node: NodeLike[NodeResultT]
     max_iterations: int
 
 
-def RecurrentSubGraph(  # noqa
+def RecurrentSubGraph(  # noqa:  N802,RUF100
     start_node: t.Type[NodeLike[NodeResultT]],
     dest_node: t.Type[NodeLike[NodeResultT]],
     max_iterations: int,
 ) -> t.Type[NodeResultT]:
     """
     Указание рекуррентного подграфа.
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/events.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/events.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import typing as t
 
-from ml_pipeline_engine.types import (
-    EventManagerLike,
-    NodeId,
-    PipelineContextLike,
-    PipelineResult,
-)
+from ml_pipeline_engine.types import EventManagerLike
+from ml_pipeline_engine.types import NodeId
+from ml_pipeline_engine.types import PipelineContextLike
+from ml_pipeline_engine.types import PipelineResult
 
 
 class EventManagerBase:
     async def on_pipeline_start(self, ctx: PipelineContextLike) -> None:
         ...
 
     async def on_pipeline_complete(self, ctx: PipelineContextLike, result: PipelineResult) -> None:
@@ -21,25 +19,25 @@
     async def on_node_complete(self, ctx: PipelineContextLike, node_id: NodeId, error: t.Optional[Exception]) -> None:
         ...
 
 
 class EventSourceMixin:
     _get_event_managers: t.Callable[..., t.List[t.Type[EventManagerLike]]]
 
-    async def _emit(self, event_name: str, **kwargs):
+    async def _emit(self, event_name: str, **kwargs: t.Any) -> None:
         for mgr in self._get_event_managers():
             callback = getattr(mgr, event_name, None)
 
             if callback:
                 await callback(ctx=self, **kwargs)
 
-    async def emit_on_node_start(self, node_id: NodeId):
+    async def emit_on_node_start(self, node_id: NodeId) -> None:
         await self._emit('on_node_start', node_id=node_id)
 
-    async def emit_on_node_complete(self, node_id: NodeId, error: t.Optional[Exception]):
+    async def emit_on_node_complete(self, node_id: NodeId, error: t.Optional[Exception]) -> None:
         await self._emit('on_node_complete', node_id=node_id, error=error)
 
-    async def emit_on_pipeline_start(self):
+    async def emit_on_pipeline_start(self) -> None:
         await self._emit('on_pipeline_start')
 
-    async def emit_on_pipeline_complete(self, result: PipelineResult):
+    async def emit_on_pipeline_complete(self, result: PipelineResult) -> None:
         await self._emit('on_pipeline_complete', result=result)
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/module_loading.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/module_loading.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 
 __all__ = [
     'import_string',
     'get_instance',
 ]
 
 
-def _cached_import(module_path, class_name) -> t.Type:
+def _cached_import(module_path: str, class_name: str) -> t.Type:
     if not (
         (module := sys.modules.get(module_path))
         and (spec := getattr(module, '__spec__', None))
-        and getattr(spec, '_initializing', False) is False  # noqa
+        and getattr(spec, '_initializing', False) is False
     ):
         module = import_module(module_path)
     return getattr(module, class_name)
 
 
-def import_string(dotted_path) -> t.Type:
+def import_string(dotted_path: str) -> t.Type:
     try:
         module_path, class_name = dotted_path.rsplit('.', 1)
     except ValueError as err:
         raise ImportError(f"{dotted_path} doesn't look like a module path") from err
 
     try:
         return _cached_import(module_path, class_name)
     except AttributeError as err:
         raise ImportError(f'Module "{module_path}" does not define a "{class_name}" attribute/class') from err
 
 
-def get_instance(cls: t.Type, *args, **kwargs) -> t.Any:
+def get_instance(cls: t.Type, *args: t.Any, **kwargs: t.Any) -> t.Any:
     default_factory = getattr(cls, 'default_factory', None)
     if default_factory is None:
         return cls(*args, **kwargs)
     return default_factory(*args, **kwargs)
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/node/enums.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/node/enums.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/parallelism/basic.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/parallelism/basic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import abc
-from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
-from typing import Optional, Union
+import typing as t
+from concurrent.futures import ProcessPoolExecutor
+from concurrent.futures import ThreadPoolExecutor
 
 from ml_pipeline_engine.logs import logger_parallelism as logger
 
+SingletonMetaT = t.TypeVar('SingletonMetaT', bound='SingletonMeta')
+
 
 class SingletonMeta(type):
     """
     The Singleton class can be implemented in different ways in Python. Some
     possible methods include: base class, decorator, metaclass. We will use the
     metaclass because it is best suited for this purpose.
     """
 
-    _instances = {}
+    _instances: t.ClassVar[t.Dict] = {}
 
-    def __call__(cls, *args, **kwargs):
+    def __call__(cls, *args: t.Any, **kwargs: t.Any) -> SingletonMetaT:
         """
         Possible changes to the value of the `__init__` argument do not affect
         the returned instance.
         """
         if cls not in cls._instances:
             instance = super().__call__(*args, **kwargs)
             cls._instances[cls] = instance
         return cls._instances[cls]
 
 
-PoolExecutorT = Union[ProcessPoolExecutor, ThreadPoolExecutor]
+PoolExecutorT = t.Union[ProcessPoolExecutor, ThreadPoolExecutor]
 
 
 class PoolExecutorRegistry(metaclass=SingletonMeta):
 
-    def __init__(self):
-        self._pool_executor: Optional[PoolExecutorT] = None
+    def __init__(self) -> None:
+        self._pool_executor: t.Optional[PoolExecutorT] = None
 
     @abc.abstractmethod
     def is_ready(self) -> None:
         ...
 
     def register_pool_executor(self, pool_executor: PoolExecutorT) -> None:
         if self._pool_executor:
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/parallelism/processes.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/parallelism/processes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from concurrent.futures import ProcessPoolExecutor
-from multiprocessing import Manager, get_context
+from multiprocessing import Manager
+from multiprocessing import get_context
 from typing import Optional
 
 from ml_pipeline_engine.logs import logger_parallelism as logger
-from ml_pipeline_engine.parallelism.basic import (
-    PoolExecutorRegistry as BasePoolExecutorRegistry,
-)
+from ml_pipeline_engine.parallelism.basic import PoolExecutorRegistry as BasePoolExecutorRegistry
 
 __all__ = ('process_pool_registry', )
 
 
 class PoolExecutorRegistry(BasePoolExecutorRegistry):
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self._process_manager: Optional[Manager] = None
 
     def is_ready(self) -> None:
 
-        if not self._pool_executor or self._pool_executor._shutdown_thread:  # noqa
+        if not self._pool_executor or self._pool_executor._shutdown_thread:
             raise RuntimeError('Исполнение невозможно без указания пула процессов')
 
         if not self._process_manager:
             raise RuntimeError('Исполнение невозможно без указания менеджера данных для процессов')
 
     def register_manager(self, manager: Manager) -> None:
         if self._process_manager:
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/parallelism/threads.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/parallelism/threads.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from concurrent.futures import ThreadPoolExecutor
 
-from ml_pipeline_engine.parallelism.basic import (
-    PoolExecutorRegistry as BasePoolExecutorRegistry,
-)
+from ml_pipeline_engine.parallelism.basic import PoolExecutorRegistry as BasePoolExecutorRegistry
 
 __all__ = ('threads_pool_registry',)
 
 
 class PoolExecutorRegistry(BasePoolExecutorRegistry):
 
     def is_ready(self) -> None:
-        if not self._pool_executor or self._pool_executor._shutdown:  # noqa
+        if not self._pool_executor or self._pool_executor._shutdown:
             raise RuntimeError('Исполнение невозможно без указания пула потоков')
 
-    def auto_init(self):
+    def auto_init(self) -> None:
         self.register_pool_executor(ThreadPoolExecutor())
 
 
 threads_pool_registry = PoolExecutorRegistry()
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/dag.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/dag.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 import inspect
+import json
 import pathlib
+import typing as t
 import warnings
-import json
-from typing import Type, List, Dict, TypeVar, Optional, Union
 
+from ml_pipeline_engine import const
 from ml_pipeline_engine.node import get_callable_run_method
 from ml_pipeline_engine.node.enums import NodeType
-from ml_pipeline_engine.types import DAGLike, NodeId, NodeLike
+from ml_pipeline_engine.types import DAGLike
+from ml_pipeline_engine.types import NodeId
+from ml_pipeline_engine.types import NodeLike
 from ml_pipeline_engine.visualization import schema
 from ml_pipeline_engine.visualization.utils import copy_resources
-from ml_pipeline_engine import const
 
-_HexColorT = TypeVar('_HexColorT', bound=str)
-_NodeTypeT = TypeVar('_NodeTypeT', bound=Union[str, NodeType])
-_NodeColorsT = Dict[_NodeTypeT, _HexColorT]
+_HexColorT = t.TypeVar('_HexColorT', bound=str)
+_NodeTypeT = t.TypeVar('_NodeTypeT', bound=t.Union[str, NodeType])
+_NodeColorsT = t.Dict[_NodeTypeT, _HexColorT]
 
 
 class GraphConfigImpl:
 
-    def __init__(self, dag: DAGLike):
+    def __init__(self, dag: DAGLike) -> None:
         self._dag = dag
 
-    def _get_node(self, node_id: NodeId) -> Type[NodeLike]:
+    def _get_node(self, node_id: NodeId) -> t.Type[NodeLike]:
         """
         Get a node object. Sometimes it can be None if we work with an artificial node
         """
         return self._dag.node_map.get(node_id)
 
     @staticmethod
-    def _get_node_relative_path(node: Type[NodeLike]) -> str:
+    def _get_node_relative_path(node: t.Type[NodeLike]) -> str:
         """
         Generate relative path for a node
         """
 
         generic_class = getattr(node, '__generic_class__', None)
 
         if generic_class is None:
@@ -41,15 +43,15 @@
         else:
             file_path = '/'.join(generic_class.__module__.split('.'))
             node = generic_class
 
         line_number = inspect.getsourcelines(node)[-1]
         return f'{file_path}.py#L{line_number}'
 
-    def _generate_nodes(self) -> List[schema.Node]:
+    def _generate_nodes(self) -> t.List[schema.Node]:
         """
         Generate physical and artificial nodes
         """
 
         nodes = []
 
         for node_id in self._dag.graph.nodes:
@@ -81,24 +83,24 @@
                             code_source=self._get_node_relative_path(node),
                         ),
                     ),
                 )
 
         return nodes
 
-    def _generate_edges(self) -> List[schema.Edge]:
+    def _generate_edges(self) -> t.List[schema.Edge]:
         """
         Generate edges between physical and artificial nodes
         """
         return [
             schema.Edge(source=source, target=target)
             for source, target in self._dag.graph.edges
         ]
 
-    def _generate_node_types(self, node_colors: Optional[_NodeColorsT] = None) -> Dict[str, schema.NodeType]:
+    def _generate_node_types(self, node_colors: t.Optional[_NodeColorsT] = None) -> t.Dict[str, schema.NodeType]:
         """
         Generate all node types.
         Will skip nodes without type.
         """
         node_colors = node_colors or {}
         node_types = {}
 
@@ -106,36 +108,36 @@
             node = self._get_node(node_id)
 
             if node is None:
                 node_type = NodeType.by_prefix(node_id)
 
             elif node.node_type is None:
                 node_type = None
-                warnings.warn(f'Node {node_id} without node type.')
+                warnings.warn(f'Node {node_id} without node type.', stacklevel=1)
 
             else:
                 node_type = NodeType(node.node_type)
 
             if node_type in node_types or node_type is None:
                 continue
 
             node_types[node_type.value] = schema.NodeType(
                 name=node_type.value,
-                hex_bgr_color=node_colors.get(node_type.value)
+                hex_bgr_color=node_colors.get(node_type.value),
             )
 
         return node_types
 
     def generate(
         self,
         name: str,
-        verbose_name: Optional[str] = None,
-        repo_link: Optional[str] = None,
-        node_colors: Optional[_NodeColorsT] = None,
-        **kwargs,
+        verbose_name: t.Optional[str] = None,
+        repo_link: t.Optional[str] = None,
+        node_colors: t.Optional[_NodeColorsT] = None,
+        **kwargs: t.Any,
     ) -> schema.GraphConfig:
         """
         Generate a config for graph visualizer
 
         Args:
             name: Tech name for the graph
             verbose_name: Name for the graph
@@ -149,15 +151,15 @@
             edges=self._generate_edges(),
             node_types=self._generate_node_types(node_colors),
             attributes=schema.GraphAttributes(
                 verbose_name=verbose_name or name,
                 repo_link=repo_link,
                 name=name,
                 **kwargs,
-            )
+            ),
         )
 
 
 def build_static(config: schema.GraphConfig, target_dir: pathlib.Path) -> None:
     """
     Generate static using config and place it in the target dir
     """
@@ -165,9 +167,9 @@
     copy_resources(
         const.LIB_ANCHOR, 'visualization', 'viewer',
         target_dir=str(target_dir),
     )
 
     config = json.dumps(config.as_dict(), ensure_ascii=False, indent=2)
 
-    with open(target_dir / 'data.js', 'w', encoding="utf-8") as file:
+    with pathlib.Path(target_dir / 'data.js').open('w', encoding='utf-8') as file:
         file.write(f'window.__GRAPH_DATA__ = {config}')
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/sample.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,80 @@
 from ml_pipeline_engine.base_nodes.processors import ProcessorBase
 from ml_pipeline_engine.dag_builders.annotation import build_dag
-from ml_pipeline_engine.dag_builders.annotation.marks import Input, SwitchCase
+from ml_pipeline_engine.dag_builders.annotation.marks import Input
+from ml_pipeline_engine.dag_builders.annotation.marks import SwitchCase
 
 
 class Ident(ProcessorBase):
     """
     Возвращает входное значение таким, каким оно было
     """
     name = 'ident'
     verbose_name = 'Identity'
 
-    def process(self, num: float):
+    def process(self, num: float) -> float:
         return num
 
 
 class SwitchStmt(ProcessorBase):
     """
     Вычисляет условие для switch
     """
     name = 'switch_stmt'
     verbose_name = 'Условие для switch'
 
-    def process(self, num: Input(Ident)):
+    def process(self, num: Input(Ident)) -> str:
         if num < 0.0:
             return 'invert'
         return 'nested_switch'
 
 
 class Invert(ProcessorBase):
     """
     Инвертирует число
     """
     name = 'invert'
     verbose_name = 'Инвертор'
 
-    def process(self, num: Input(Ident)):
+    def process(self, num: Input(Ident)) -> float:
         return -num
 
 
 class NestedSwitchStmt(ProcessorBase):
     """
     Вычисляет условие для switch
     """
     name = 'nested_switch_stmt'
     verbose_name = 'Условие для вложенного switch'
 
-    def process(self, num: Input(Ident)):
+    def process(self, num: Input(Ident)) -> str:
         if num == 1.0:
             return 'double'
         return 'triple'
 
 
 class DoubleNumber(ProcessorBase):
     """
     Умножает число на 2
     """
     name = 'double_number'
     verbose_name = 'Удвоение числа'
 
-    def process(self, num: Input(Ident)):
+    def process(self, num: Input(Ident)) -> float:
         return num * 2
 
 
 class TripleNumber(ProcessorBase):
     """
     Умножает число на 3
     """
     name = 'triple_number'
     verbose_name = 'Умножение числа на 3'
 
-    def process(self, num: Input(Ident)):
+    def process(self, num: Input(Ident)) -> float:
         return num * 3
 
 
 NestedSwitchCase = SwitchCase(
     name='nested_switch',
     switch=NestedSwitchStmt,
     cases=[
@@ -86,15 +87,15 @@
 class Add3Node(ProcessorBase):
     """
     Прибавляет число 3
     """
     name = 'add_3'
     verbose_name = 'Прибавление числа 3'
 
-    def process(self, num: NestedSwitchCase):
+    def process(self, num: NestedSwitchCase) -> float:
         return num + 3
 
 
 SomeSwitchCase = SwitchCase(
     name='main_switch',
     switch=SwitchStmt,
     cases=[
@@ -107,12 +108,12 @@
 class Result(ProcessorBase):
     """
     Возвращает результат
     """
     name = 'result'
     verbose_name = 'Результат'
 
-    def process(self, num: SomeSwitchCase, num2: Input(Ident)):
+    def process(self, num: SomeSwitchCase, num2: Input(Ident)) -> float:
         return num + num2
 
 
 sample_dag = build_dag(input_node=Ident, output_node=Result)
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/schema.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-from dataclasses import dataclass, field, asdict
-from typing import List, Optional, Dict, Any
+from dataclasses import asdict
+from dataclasses import dataclass
+from dataclasses import field
+from typing import Any
+from typing import Dict
+from typing import List
+from typing import Optional
 
 
 @dataclass
 class GraphAttributes:
     verbose_name: str
     name: str  # Tech name
     repo_link: Optional[str] = None
@@ -30,15 +35,15 @@
 
 @dataclass
 class Edge:
     id: str = field(init=False)
     source: str
     target: str
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         self.id = f'{self.source}->{self.target}'
 
 
 @dataclass
 class NodeType:
     name: str  # Tech name
     hex_bgr_color: Optional[str] = None
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/utils.py` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/asset-manifest.json` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/favicon.ico` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/favicon.ico`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/index.html` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/index.html`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/css/main.fdcc84c5.css` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/static/css/main.fdcc84c5.css`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/css/main.fdcc84c5.css.map` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/static/css/main.fdcc84c5.css.map`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/453.ae999f12.chunk.js` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/static/js/453.ae999f12.chunk.js`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/453.ae999f12.chunk.js.map` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/static/js/453.ae999f12.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js.LICENSE.txt` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js.map` & `ml_pipeline_engine-2.0.0a0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js.map`

 * *Files identical despite different names*

