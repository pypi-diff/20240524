# Comparing `tmp/data_prep_toolkit-0.1.0.tar.gz` & `tmp/data_prep_toolkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_prep_toolkit-0.1.0.tar", last modified: Wed May 15 16:26:42 2024, max compression
+gzip compressed data, was "data_prep_toolkit-0.1.1.tar", last modified: Fri May 24 10:09:18 2024, max compression
```

## Comparing `data_prep_toolkit-0.1.0.tar` & `data_prep_toolkit-0.1.1.tar`

### file list

```diff
@@ -1,140 +1,122 @@
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.529639 data_prep_toolkit-0.1.0/
--rw-r--r--   0 dawood     (501) staff       (20)      357 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/.gitignore
--rw-r--r--   0 dawood     (501) staff       (20)     2572 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/Makefile
--rw-r--r--   0 dawood     (501) staff       (20)     1880 2024-05-15 16:26:42.529334 data_prep_toolkit-0.1.0/PKG-INFO
--rw-r--r--   0 dawood     (501) staff       (20)      963 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/README.md
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.501759 data_prep_toolkit-0.1.0/doc/
--rw-r--r--   0 dawood     (501) staff       (20)    13397 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/doc/advanced-transform-tutorial.md
--rw-r--r--   0 dawood     (501) staff       (20)     7687 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/doc/architecture.md
--rw-r--r--   0 dawood     (501) staff       (20)     1418 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/doc/overview.md
--rw-r--r--   0 dawood     (501) staff       (20)   137580 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/doc/processing-architecture.jpg
--rw-r--r--   0 dawood     (501) staff       (20)     3659 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/doc/python-launcher-options.md
--rw-r--r--   0 dawood     (501) staff       (20)      531 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/doc/python-runtime.md
--rw-r--r--   0 dawood     (501) staff       (20)     5221 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/doc/ray-launcher-options.md
--rw-r--r--   0 dawood     (501) staff       (20)     7567 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/doc/ray-runtime.md
--rw-r--r--   0 dawood     (501) staff       (20)     9369 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/doc/simplest-transform-tutorial.md
--rw-r--r--   0 dawood     (501) staff       (20)      195 2024-05-14 11:51:27.000000 data_prep_toolkit-0.1.0/doc/testing-e2e-transform.md
--rw-r--r--   0 dawood     (501) staff       (20)    12176 2024-05-14 11:51:27.000000 data_prep_toolkit-0.1.0/doc/transform-external-resources.md
--rw-r--r--   0 dawood     (501) staff       (20)      436 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/doc/transform-runtimes.md
--rw-r--r--   0 dawood     (501) staff       (20)     3614 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/doc/transform-s3-testing.md
--rw-r--r--   0 dawood     (501) staff       (20)     5889 2024-05-14 11:51:27.000000 data_prep_toolkit-0.1.0/doc/transform-standalone-testing.md
--rw-r--r--   0 dawood     (501) staff       (20)      472 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/doc/transform-testing.md
--rw-r--r--   0 dawood     (501) staff       (20)      674 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/doc/transform-tutorial-examples.md
--rw-r--r--   0 dawood     (501) staff       (20)     4595 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/doc/transform-tutorials.md
--rw-r--r--   0 dawood     (501) staff       (20)     1418 2024-05-14 11:51:27.000000 data_prep_toolkit-0.1.0/doc/transformer-utilities.md
--rw-r--r--   0 dawood     (501) staff       (20)     1329 2024-05-15 16:26:12.000000 data_prep_toolkit-0.1.0/pyproject.toml
--rw-r--r--   0 dawood     (501) staff       (20)       38 2024-05-15 16:26:42.529696 data_prep_toolkit-0.1.0/setup.cfg
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.489934 data_prep_toolkit-0.1.0/src/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.528162 data_prep_toolkit-0.1.0/src/data_prep_toolkit.egg-info/
--rw-r--r--   0 dawood     (501) staff       (20)     1880 2024-05-15 16:26:42.000000 data_prep_toolkit-0.1.0/src/data_prep_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 dawood     (501) staff       (20)     4693 2024-05-15 16:26:42.000000 data_prep_toolkit-0.1.0/src/data_prep_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 dawood     (501) staff       (20)        1 2024-05-15 16:26:42.000000 data_prep_toolkit-0.1.0/src/data_prep_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 dawood     (501) staff       (20)      249 2024-05-15 16:26:42.000000 data_prep_toolkit-0.1.0/src/data_prep_toolkit.egg-info/requires.txt
--rw-r--r--   0 dawood     (501) staff       (20)       16 2024-05-15 16:26:42.000000 data_prep_toolkit-0.1.0/src/data_prep_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.503249 data_prep_toolkit-0.1.0/src/data_processing/
--rw-r--r--   0 dawood     (501) staff       (20)        0 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/__init__.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.505781 data_prep_toolkit-0.1.0/src/data_processing/data_access/
--rw-r--r--   0 dawood     (501) staff       (20)      427 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/data_access/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     8339 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/src/data_processing/data_access/arrow_s3.py
--rw-r--r--   0 dawood     (501) staff       (20)     8484 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access.py
--rw-r--r--   0 dawood     (501) staff       (20)    11466 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access_factory.py
--rw-r--r--   0 dawood     (501) staff       (20)     5647 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access_factory_base.py
--rw-r--r--   0 dawood     (501) staff       (20)    15061 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access_local.py
--rw-r--r--   0 dawood     (501) staff       (20)    13499 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access_s3.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.507122 data_prep_toolkit-0.1.0/src/data_processing/runtime/
--rw-r--r--   0 dawood     (501) staff       (20)      370 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     3067 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/execution_configuration.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.508141 data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/
--rw-r--r--   0 dawood     (501) staff       (20)      378 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     1143 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/runtime_configuration.py
--rw-r--r--   0 dawood     (501) staff       (20)     3719 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/transform_launcher.py
--rw-r--r--   0 dawood     (501) staff       (20)     4301 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/transform_orchestrator.py
--rw-r--r--   0 dawood     (501) staff       (20)     2107 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/transform_table_processor.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.510679 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/
--rw-r--r--   0 dawood     (501) staff       (20)      763 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     4572 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/execution_configuration.py
--rw-r--r--   0 dawood     (501) staff       (20)     7404 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/ray_utils.py
--rw-r--r--   0 dawood     (501) staff       (20)     1788 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/runtime_configuration.py
--rw-r--r--   0 dawood     (501) staff       (20)     4801 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_launcher.py
--rw-r--r--   0 dawood     (501) staff       (20)     6354 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_orchestrator.py
--rw-r--r--   0 dawood     (501) staff       (20)     2536 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_runtime.py
--rw-r--r--   0 dawood     (501) staff       (20)     2883 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_statistics.py
--rw-r--r--   0 dawood     (501) staff       (20)     2012 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_table_processor.py
--rw-r--r--   0 dawood     (501) staff       (20)     2777 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/runtime_configuration.py
--rw-r--r--   0 dawood     (501) staff       (20)     2889 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/transform_launcher.py
--rw-r--r--   0 dawood     (501) staff       (20)     8328 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/src/data_processing/runtime/transform_table_processor.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.511274 data_prep_toolkit-0.1.0/src/data_processing/test_support/
--rw-r--r--   0 dawood     (501) staff       (20)       62 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     8234 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/abstract_test.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.511870 data_prep_toolkit-0.1.0/src/data_processing/test_support/data_access/
--rw-r--r--   0 dawood     (501) staff       (20)       69 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/data_access/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     2666 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/data_access/data_access_factory_test.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.512803 data_prep_toolkit-0.1.0/src/data_processing/test_support/launch/
--rw-r--r--   0 dawood     (501) staff       (20)        0 2024-05-10 14:02:13.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/launch/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     4821 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/launch/transform_test.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.513825 data_prep_toolkit-0.1.0/src/data_processing/test_support/transform/
--rw-r--r--   0 dawood     (501) staff       (20)      174 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/transform/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     6140 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/transform/noop_transform.py
--rw-r--r--   0 dawood     (501) staff       (20)     4476 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/test_support/transform/transform_test.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.514667 data_prep_toolkit-0.1.0/src/data_processing/transform/
--rw-r--r--   0 dawood     (501) staff       (20)      263 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/src/data_processing/transform/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     2298 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/transform/table_transform.py
--rw-r--r--   0 dawood     (501) staff       (20)     4394 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/src/data_processing/transform/transform_configuration.py
--rw-r--r--   0 dawood     (501) staff       (20)     1465 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/transform/transform_statistics.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.515940 data_prep_toolkit-0.1.0/src/data_processing/utils/
--rw-r--r--   0 dawood     (501) staff       (20)      354 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/utils/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     3135 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/utils/cli_utils.py
--rw-r--r--   0 dawood     (501) staff       (20)     1695 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/utils/config.py
--rw-r--r--   0 dawood     (501) staff       (20)     2052 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/utils/log.py
--rw-r--r--   0 dawood     (501) staff       (20)     6029 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/src/data_processing/utils/params_utils.py
--rw-r--r--   0 dawood     (501) staff       (20)     7916 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/src/data_processing/utils/transform_utils.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.493074 data_prep_toolkit-0.1.0/test/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.493712 data_prep_toolkit-0.1.0/test/data_processing_tests/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.524283 data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/
--rw-r--r--   0 dawood     (501) staff       (20)     1256 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/daf_local_test.py
--rw-r--r--   0 dawood     (501) staff       (20)    24597 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/data_access_local_test.py
--rw-r--r--   0 dawood     (501) staff       (20)     5734 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/data_access_s3_test.py
--rw-r--r--   0 dawood     (501) staff       (20)     1545 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/sample_input_data_test.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.493505 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.524796 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/pure_python/
--rw-r--r--   0 dawood     (501) staff       (20)     6443 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/pure_python/launcher_test.py
--rw-r--r--   0 dawood     (501) staff       (20)     2717 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/pure_python/multi_launcher_test.py
--rw-r--r--   0 dawood     (501) staff       (20)     1852 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/pure_python/test_noop_launch.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.525407 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/ray/
--rw-r--r--   0 dawood     (501) staff       (20)     7229 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/ray/launcher_test.py
--rw-r--r--   0 dawood     (501) staff       (20)     2825 2024-05-15 16:22:24.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/ray/multi_launcher_test.py
--rw-r--r--   0 dawood     (501) staff       (20)     3296 2024-05-13 13:07:17.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/ray/ray_util_test.py
--rw-r--r--   0 dawood     (501) staff       (20)     1856 2024-05-14 17:53:57.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/launch/ray/test_noop_launch.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.525555 data_prep_toolkit-0.1.0/test/data_processing_tests/transform/
--rw-r--r--   0 dawood     (501) staff       (20)     1678 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/transform/test_noop.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.525773 data_prep_toolkit-0.1.0/test/data_processing_tests/util/
--rw-r--r--   0 dawood     (501) staff       (20)     1386 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test/data_processing_tests/util/transform_utils_test.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.491391 data_prep_toolkit-0.1.0/test-data/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.492327 data_prep_toolkit-0.1.0/test-data/data_processing/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.491812 data_prep_toolkit-0.1.0/test-data/data_processing/daf/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.491712 data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.516960 data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/ds1/
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/ds1/sample1.parquet
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/ds1/sample2.parquet
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.517853 data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/ds2/
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/ds2/sample3.parquet
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.491904 data_prep_toolkit-0.1.0/test-data/data_processing/daf/output/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.518578 data_prep_toolkit-0.1.0/test-data/data_processing/daf/output/ds1/
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/daf/output/ds1/sample1.parquet
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.519300 data_prep_toolkit-0.1.0/test-data/data_processing/input/
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/input/sample1.parquet
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.520896 data_prep_toolkit-0.1.0/test-data/data_processing/input_multiple/
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/input_multiple/sample1.parquet
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/input_multiple/sample2.parquet
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/input_multiple/sample3.parquet
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.492474 data_prep_toolkit-0.1.0/test-data/data_processing/ray/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.492756 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.521548 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/expected/
--rw-r--r--   0 dawood     (501) staff       (20)     1128 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/expected/metadata.json
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/expected/sample1.parquet
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.522163 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/expected/subdir/
--rw-r--r--   0 dawood     (501) staff       (20)      753 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/expected/subdir/test1.parquet
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.522365 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/input/
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/input/sample1.parquet
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-15 16:26:42.522594 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/input/subdir/
--rw-r--r--   0 dawood     (501) staff       (20)      753 2024-05-09 14:24:06.000000 data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/input/subdir/test1.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.046186 data_prep_toolkit-0.1.1/
+-rw-r--r--   0 boris      (501) staff       (20)      357 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/.gitignore
+-rw-r--r--   0 boris      (501) staff       (20)     2826 2024-05-22 13:03:48.000000 data_prep_toolkit-0.1.1/Makefile
+-rw-r--r--   0 boris      (501) staff       (20)     1887 2024-05-24 10:09:18.045567 data_prep_toolkit-0.1.1/PKG-INFO
+-rw-r--r--   0 boris      (501) staff       (20)      970 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/README.md
+-rw-r--r--   0 boris      (501) staff       (20)     1329 2024-05-24 10:07:32.000000 data_prep_toolkit-0.1.1/pyproject.toml
+-rw-r--r--   0 boris      (501) staff       (20)       38 2024-05-24 10:09:18.046311 data_prep_toolkit-0.1.1/setup.cfg
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:17.966858 data_prep_toolkit-0.1.1/src/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.043136 data_prep_toolkit-0.1.1/src/data_prep_toolkit.egg-info/
+-rw-r--r--   0 boris      (501) staff       (20)     1887 2024-05-24 10:09:17.000000 data_prep_toolkit-0.1.1/src/data_prep_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 boris      (501) staff       (20)     4231 2024-05-24 10:09:17.000000 data_prep_toolkit-0.1.1/src/data_prep_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 boris      (501) staff       (20)        1 2024-05-24 10:09:17.000000 data_prep_toolkit-0.1.1/src/data_prep_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 boris      (501) staff       (20)      249 2024-05-24 10:09:17.000000 data_prep_toolkit-0.1.1/src/data_prep_toolkit.egg-info/requires.txt
+-rw-r--r--   0 boris      (501) staff       (20)       16 2024-05-24 10:09:17.000000 data_prep_toolkit-0.1.1/src/data_prep_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:17.984405 data_prep_toolkit-0.1.1/src/data_processing/
+-rw-r--r--   0 boris      (501) staff       (20)        0 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/__init__.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:17.990193 data_prep_toolkit-0.1.1/src/data_processing/data_access/
+-rw-r--r--   0 boris      (501) staff       (20)      427 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/data_access/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     8339 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/data_access/arrow_s3.py
+-rw-r--r--   0 boris      (501) staff       (20)     8484 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/data_access/data_access.py
+-rw-r--r--   0 boris      (501) staff       (20)    11511 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/data_access/data_access_factory.py
+-rw-r--r--   0 boris      (501) staff       (20)     5647 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/data_access/data_access_factory_base.py
+-rw-r--r--   0 boris      (501) staff       (20)    14967 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/data_access/data_access_local.py
+-rw-r--r--   0 boris      (501) staff       (20)    13499 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/data_access/data_access_s3.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:17.994484 data_prep_toolkit-0.1.1/src/data_processing/runtime/
+-rw-r--r--   0 boris      (501) staff       (20)      369 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     3178 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/execution_configuration.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:17.998366 data_prep_toolkit-0.1.1/src/data_processing/runtime/pure_python/
+-rw-r--r--   0 boris      (501) staff       (20)      382 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/pure_python/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     1143 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/pure_python/runtime_configuration.py
+-rw-r--r--   0 boris      (501) staff       (20)     2217 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/pure_python/transform_file_processor.py
+-rw-r--r--   0 boris      (501) staff       (20)     3719 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/pure_python/transform_launcher.py
+-rw-r--r--   0 boris      (501) staff       (20)     4326 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/pure_python/transform_orchestrator.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.005635 data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/
+-rw-r--r--   0 boris      (501) staff       (20)      668 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     4435 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/execution_configuration.py
+-rw-r--r--   0 boris      (501) staff       (20)     7404 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/ray_utils.py
+-rw-r--r--   0 boris      (501) staff       (20)     1768 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/runtime_configuration.py
+-rw-r--r--   0 boris      (501) staff       (20)     2001 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/transform_file_processor.py
+-rw-r--r--   0 boris      (501) staff       (20)     4801 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/transform_launcher.py
+-rw-r--r--   0 boris      (501) staff       (20)     6352 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/transform_orchestrator.py
+-rw-r--r--   0 boris      (501) staff       (20)     2531 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/transform_runtime.py
+-rw-r--r--   0 boris      (501) staff       (20)     3297 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/transform_statistics.py
+-rw-r--r--   0 boris      (501) staff       (20)     2769 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/runtime_configuration.py
+-rw-r--r--   0 boris      (501) staff       (20)     7917 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/transform_file_processor.py
+-rw-r--r--   0 boris      (501) staff       (20)     2804 2024-05-20 13:38:14.000000 data_prep_toolkit-0.1.1/src/data_processing/runtime/transform_launcher.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.006792 data_prep_toolkit-0.1.1/src/data_processing/test_support/
+-rw-r--r--   0 boris      (501) staff       (20)       62 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/test_support/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     8234 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/test_support/abstract_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.008353 data_prep_toolkit-0.1.1/src/data_processing/test_support/data_access/
+-rw-r--r--   0 boris      (501) staff       (20)       69 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/test_support/data_access/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     2666 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/test_support/data_access/data_access_factory_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.009205 data_prep_toolkit-0.1.1/src/data_processing/test_support/launch/
+-rw-r--r--   0 boris      (501) staff       (20)        0 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/test_support/launch/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     4821 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/test_support/launch/transform_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.011543 data_prep_toolkit-0.1.1/src/data_processing/test_support/transform/
+-rw-r--r--   0 boris      (501) staff       (20)      174 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/test_support/transform/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     6140 2024-05-18 09:49:39.000000 data_prep_toolkit-0.1.1/src/data_processing/test_support/transform/noop_transform.py
+-rw-r--r--   0 boris      (501) staff       (20)     4476 2024-05-21 07:23:07.000000 data_prep_toolkit-0.1.1/src/data_processing/test_support/transform/transform_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.015288 data_prep_toolkit-0.1.1/src/data_processing/transform/
+-rw-r--r--   0 boris      (501) staff       (20)      342 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/transform/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     2905 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/transform/binary_transform.py
+-rw-r--r--   0 boris      (501) staff       (20)     5758 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/transform/table_transform.py
+-rw-r--r--   0 boris      (501) staff       (20)     4387 2024-05-22 07:01:10.000000 data_prep_toolkit-0.1.1/src/data_processing/transform/transform_configuration.py
+-rw-r--r--   0 boris      (501) staff       (20)     1465 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/transform/transform_statistics.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.019267 data_prep_toolkit-0.1.1/src/data_processing/utils/
+-rw-r--r--   0 boris      (501) staff       (20)      354 2024-05-20 13:38:14.000000 data_prep_toolkit-0.1.1/src/data_processing/utils/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     3135 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/utils/cli_utils.py
+-rw-r--r--   0 boris      (501) staff       (20)     1695 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/utils/config.py
+-rw-r--r--   0 boris      (501) staff       (20)     2052 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/utils/log.py
+-rw-r--r--   0 boris      (501) staff       (20)     6554 2024-05-20 13:38:14.000000 data_prep_toolkit-0.1.1/src/data_processing/utils/params_utils.py
+-rw-r--r--   0 boris      (501) staff       (20)     7869 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/src/data_processing/utils/transform_utils.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:17.975911 data_prep_toolkit-0.1.1/test/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:17.977597 data_prep_toolkit-0.1.1/test/data_processing_tests/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.035936 data_prep_toolkit-0.1.1/test/data_processing_tests/data_access/
+-rw-r--r--   0 boris      (501) staff       (20)     1256 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test/data_processing_tests/data_access/daf_local_test.py
+-rw-r--r--   0 boris      (501) staff       (20)    24597 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test/data_processing_tests/data_access/data_access_local_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     5734 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test/data_processing_tests/data_access/data_access_s3_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     1545 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test/data_processing_tests/data_access/sample_input_data_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:17.976906 data_prep_toolkit-0.1.1/test/data_processing_tests/launch/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.038014 data_prep_toolkit-0.1.1/test/data_processing_tests/launch/pure_python/
+-rw-r--r--   0 boris      (501) staff       (20)     6443 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test/data_processing_tests/launch/pure_python/launcher_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     2719 2024-05-20 13:38:14.000000 data_prep_toolkit-0.1.1/test/data_processing_tests/launch/pure_python/multi_launcher_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     1852 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test/data_processing_tests/launch/pure_python/test_noop_launch.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.040833 data_prep_toolkit-0.1.1/test/data_processing_tests/launch/ray/
+-rw-r--r--   0 boris      (501) staff       (20)     7229 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test/data_processing_tests/launch/ray/launcher_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     2828 2024-05-20 13:38:14.000000 data_prep_toolkit-0.1.1/test/data_processing_tests/launch/ray/multi_launcher_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     3296 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test/data_processing_tests/launch/ray/ray_util_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     1856 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test/data_processing_tests/launch/ray/test_noop_launch.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.041522 data_prep_toolkit-0.1.1/test/data_processing_tests/transform/
+-rw-r--r--   0 boris      (501) staff       (20)     1678 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test/data_processing_tests/transform/test_noop.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.042232 data_prep_toolkit-0.1.1/test/data_processing_tests/util/
+-rw-r--r--   0 boris      (501) staff       (20)     1386 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test/data_processing_tests/util/transform_utils_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:17.970307 data_prep_toolkit-0.1.1/test-data/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:17.973582 data_prep_toolkit-0.1.1/test-data/data_processing/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:17.972191 data_prep_toolkit-0.1.1/test-data/data_processing/daf/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:17.971726 data_prep_toolkit-0.1.1/test-data/data_processing/daf/input/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.021571 data_prep_toolkit-0.1.1/test-data/data_processing/daf/input/ds1/
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test-data/data_processing/daf/input/ds1/sample1.parquet
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test-data/data_processing/daf/input/ds1/sample2.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.022858 data_prep_toolkit-0.1.1/test-data/data_processing/daf/input/ds2/
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test-data/data_processing/daf/input/ds2/sample3.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:17.972474 data_prep_toolkit-0.1.1/test-data/data_processing/daf/output/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.023744 data_prep_toolkit-0.1.1/test-data/data_processing/daf/output/ds1/
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test-data/data_processing/daf/output/ds1/sample1.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.024940 data_prep_toolkit-0.1.1/test-data/data_processing/input/
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test-data/data_processing/input/sample1.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.028216 data_prep_toolkit-0.1.1/test-data/data_processing/input_multiple/
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test-data/data_processing/input_multiple/sample1.parquet
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test-data/data_processing/input_multiple/sample2.parquet
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test-data/data_processing/input_multiple/sample3.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:17.973852 data_prep_toolkit-0.1.1/test-data/data_processing/ray/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:17.974916 data_prep_toolkit-0.1.1/test-data/data_processing/ray/noop/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.030039 data_prep_toolkit-0.1.1/test-data/data_processing/ray/noop/expected/
+-rw-r--r--   0 boris      (501) staff       (20)     1128 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test-data/data_processing/ray/noop/expected/metadata.json
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test-data/data_processing/ray/noop/expected/sample1.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.031183 data_prep_toolkit-0.1.1/test-data/data_processing/ray/noop/expected/subdir/
+-rw-r--r--   0 boris      (501) staff       (20)      753 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test-data/data_processing/ray/noop/expected/subdir/test1.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.031717 data_prep_toolkit-0.1.1/test-data/data_processing/ray/noop/input/
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test-data/data_processing/ray/noop/input/sample1.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:09:18.032690 data_prep_toolkit-0.1.1/test-data/data_processing/ray/noop/input/subdir/
+-rw-r--r--   0 boris      (501) staff       (20)      753 2024-05-17 14:49:26.000000 data_prep_toolkit-0.1.1/test-data/data_processing/ray/noop/input/subdir/test1.parquet
```

### Comparing `data_prep_toolkit-0.1.0/Makefile` & `data_prep_toolkit-0.1.1/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Use make help, to see the available rules
-REPOROOT=../
-include ../.make.defaults
-include ../.make.versions
+REPOROOT=../..
+include $(REPOROOT)/.make.defaults
 
 TAG := "v${DPK_LIB_VERSION}"
 
 
 clean::
 	@# Help: Clean up the distribution build and the venv 
 	rm -rf dist venv
@@ -52,12 +51,14 @@
 # it seems when running multiple ray launch tests in a single pytest run there is some sort of ray.init() duplication.
 # pytest-forked was tried, but then we get SIGABRT in pytest when running the s3 tests, some of which are skipped.. 
 test::  
 	@# Help: Use the already-built virtual environment to run pytest on the test directory. 
 	source venv/bin/activate; export PYTHONPATH=../src; cd test; $(PYTEST)  data_processing_tests/data_access;
 	source venv/bin/activate; export PYTHONPATH=../src;  cd test; $(PYTEST)  data_processing_tests/transform;
 	source venv/bin/activate; export PYTHONPATH=../src;  cd test; $(PYTEST)  data_processing_tests/launch/pure_python/launcher_test.py;
+	source venv/bin/activate; export PYTHONPATH=../src;  cd test; $(PYTEST)  data_processing_tests/launch/pure_python/multi_launcher_test.py;
 	source venv/bin/activate; export PYTHONPATH=../src;  cd test; $(PYTEST)  data_processing_tests/launch/pure_python/test_noop_launch.py;
 	source venv/bin/activate; export PYTHONPATH=../src; cd test; $(PYTEST)  data_processing_tests/launch/ray/ray_util_test.py;
+	source venv/bin/activate; export PYTHONPATH=../src; cd test; $(PYTEST)  data_processing_tests/launch/ray/multi_launcher_test.py;
 	source venv/bin/activate; export PYTHONPATH=../src; cd test; $(PYTEST)  data_processing_tests/launch/ray/launcher_test.py;
 	source venv/bin/activate; export PYTHONPATH=../src; cd test; $(PYTEST)  data_processing_tests/launch/ray/test_noop_launch.py;
```

### Comparing `data_prep_toolkit-0.1.0/PKG-INFO` & `data_prep_toolkit-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_prep_toolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Data Preparation Toolkit Library
 Author-email: David Wood <dawood@us.ibm.com>, Boris Lublinsky <blublinsky@ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ray[default]==2.9.3
 Requires-Dist: pyarrow==15.0.2
@@ -23,17 +23,17 @@
 Requires-Dist: pytest-mock>=3.10.0; extra == "dev"
 Requires-Dist: moto==5.0.5; extra == "dev"
 Requires-Dist: markupsafe==2.0.1; extra == "dev"
 
 # Data Processing Library
 This provides a python framework for developing _transforms_
 on data stored in files - currently parquet files are supported -
-and running them in a [ray](https://ray.com) cluster.
+and running them in a [ray](https://www.ray.io/) cluster.
 Data files may be stored in the local file system or  COS/S3.
-For more details see the [documentation](doc/overview.md).
+For more details see the [documentation](../doc/overview.md).
 
 ### Virtual Environment
 The project uses `pyproject.toml` and a Makefile for operations.
 To do development you should establish the virtual environment
 ```shell
 make venv
 ```
```

### Comparing `data_prep_toolkit-0.1.0/README.md` & `data_prep_toolkit-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Data Processing Library
 This provides a python framework for developing _transforms_
 on data stored in files - currently parquet files are supported -
-and running them in a [ray](https://ray.com) cluster.
+and running them in a [ray](https://www.ray.io/) cluster.
 Data files may be stored in the local file system or  COS/S3.
-For more details see the [documentation](doc/overview.md).
+For more details see the [documentation](../doc/overview.md).
 
 ### Virtual Environment
 The project uses `pyproject.toml` and a Makefile for operations.
 To do development you should establish the virtual environment
 ```shell
 make venv
 ```
```

### Comparing `data_prep_toolkit-0.1.0/pyproject.toml` & `data_prep_toolkit-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "data_prep_toolkit"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.10"
 description = "Data Preparation Toolkit Library"
 license = {text = "Apache-2.0"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     { name = "David Wood", email = "dawood@us.ibm.com" },
     { name = "Boris Lublinsky", email = "blublinsky@ibm.com" },
```

### Comparing `data_prep_toolkit-0.1.0/src/data_prep_toolkit.egg-info/PKG-INFO` & `data_prep_toolkit-0.1.1/src/data_prep_toolkit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_prep_toolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Data Preparation Toolkit Library
 Author-email: David Wood <dawood@us.ibm.com>, Boris Lublinsky <blublinsky@ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ray[default]==2.9.3
 Requires-Dist: pyarrow==15.0.2
@@ -23,17 +23,17 @@
 Requires-Dist: pytest-mock>=3.10.0; extra == "dev"
 Requires-Dist: moto==5.0.5; extra == "dev"
 Requires-Dist: markupsafe==2.0.1; extra == "dev"
 
 # Data Processing Library
 This provides a python framework for developing _transforms_
 on data stored in files - currently parquet files are supported -
-and running them in a [ray](https://ray.com) cluster.
+and running them in a [ray](https://www.ray.io/) cluster.
 Data files may be stored in the local file system or  COS/S3.
-For more details see the [documentation](doc/overview.md).
+For more details see the [documentation](../doc/overview.md).
 
 ### Virtual Environment
 The project uses `pyproject.toml` and a Makefile for operations.
 To do development you should establish the virtual environment
 ```shell
 make venv
 ```
```

### Comparing `data_prep_toolkit-0.1.0/src/data_prep_toolkit.egg-info/SOURCES.txt` & `data_prep_toolkit-0.1.1/src/data_prep_toolkit.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,11 @@
 .gitignore
 Makefile
 README.md
 pyproject.toml
-doc/advanced-transform-tutorial.md
-doc/architecture.md
-doc/overview.md
-doc/processing-architecture.jpg
-doc/python-launcher-options.md
-doc/python-runtime.md
-doc/ray-launcher-options.md
-doc/ray-runtime.md
-doc/simplest-transform-tutorial.md
-doc/testing-e2e-transform.md
-doc/transform-external-resources.md
-doc/transform-runtimes.md
-doc/transform-s3-testing.md
-doc/transform-standalone-testing.md
-doc/transform-testing.md
-doc/transform-tutorial-examples.md
-doc/transform-tutorials.md
-doc/transformer-utilities.md
 src/data_prep_toolkit.egg-info/PKG-INFO
 src/data_prep_toolkit.egg-info/SOURCES.txt
 src/data_prep_toolkit.egg-info/dependency_links.txt
 src/data_prep_toolkit.egg-info/requires.txt
 src/data_prep_toolkit.egg-info/top_level.txt
 src/data_processing/__init__.py
 src/data_processing/data_access/__init__.py
@@ -32,40 +14,41 @@
 src/data_processing/data_access/data_access_factory.py
 src/data_processing/data_access/data_access_factory_base.py
 src/data_processing/data_access/data_access_local.py
 src/data_processing/data_access/data_access_s3.py
 src/data_processing/runtime/__init__.py
 src/data_processing/runtime/execution_configuration.py
 src/data_processing/runtime/runtime_configuration.py
+src/data_processing/runtime/transform_file_processor.py
 src/data_processing/runtime/transform_launcher.py
-src/data_processing/runtime/transform_table_processor.py
 src/data_processing/runtime/pure_python/__init__.py
 src/data_processing/runtime/pure_python/runtime_configuration.py
+src/data_processing/runtime/pure_python/transform_file_processor.py
 src/data_processing/runtime/pure_python/transform_launcher.py
 src/data_processing/runtime/pure_python/transform_orchestrator.py
-src/data_processing/runtime/pure_python/transform_table_processor.py
 src/data_processing/runtime/ray/__init__.py
 src/data_processing/runtime/ray/execution_configuration.py
 src/data_processing/runtime/ray/ray_utils.py
 src/data_processing/runtime/ray/runtime_configuration.py
+src/data_processing/runtime/ray/transform_file_processor.py
 src/data_processing/runtime/ray/transform_launcher.py
 src/data_processing/runtime/ray/transform_orchestrator.py
 src/data_processing/runtime/ray/transform_runtime.py
 src/data_processing/runtime/ray/transform_statistics.py
-src/data_processing/runtime/ray/transform_table_processor.py
 src/data_processing/test_support/__init__.py
 src/data_processing/test_support/abstract_test.py
 src/data_processing/test_support/data_access/__init__.py
 src/data_processing/test_support/data_access/data_access_factory_test.py
 src/data_processing/test_support/launch/__init__.py
 src/data_processing/test_support/launch/transform_test.py
 src/data_processing/test_support/transform/__init__.py
 src/data_processing/test_support/transform/noop_transform.py
 src/data_processing/test_support/transform/transform_test.py
 src/data_processing/transform/__init__.py
+src/data_processing/transform/binary_transform.py
 src/data_processing/transform/table_transform.py
 src/data_processing/transform/transform_configuration.py
 src/data_processing/transform/transform_statistics.py
 src/data_processing/utils/__init__.py
 src/data_processing/utils/cli_utils.py
 src/data_processing/utils/config.py
 src/data_processing/utils/log.py
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/data_access/arrow_s3.py` & `data_prep_toolkit-0.1.1/src/data_processing/data_access/arrow_s3.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access.py` & `data_prep_toolkit-0.1.1/src/data_processing/data_access/data_access.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access_factory.py` & `data_prep_toolkit-0.1.1/src/data_processing/data_access/data_access_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,22 +138,22 @@
         """
         if isinstance(args, argparse.Namespace):
             arg_dict = vars(args)
         elif isinstance(args, dict):
             arg_dict = args
         else:
             raise ValueError("args must be Namespace or dictionary")
-        s3_cred = arg_dict.get(f"{self.cli_arg_prefix}s3_cred")
-        s3_config = arg_dict.get(f"{self.cli_arg_prefix}s3_config")
-        local_config = arg_dict.get(f"{self.cli_arg_prefix}local_config")
-        checkpointing = arg_dict.get(f"{self.cli_arg_prefix}checkpointing")
+        s3_cred = arg_dict.get(f"{self.cli_arg_prefix}s3_cred", None)
+        s3_config = arg_dict.get(f"{self.cli_arg_prefix}s3_config", None)
+        local_config = arg_dict.get(f"{self.cli_arg_prefix}local_config", None)
+        checkpointing = arg_dict.get(f"{self.cli_arg_prefix}checkpointing", False)
         max_files = arg_dict.get(f"{self.cli_arg_prefix}max_files", -1)
-        data_sets = arg_dict.get(f"{self.cli_arg_prefix}data_sets")
+        data_sets = arg_dict.get(f"{self.cli_arg_prefix}data_sets", None)
         n_samples = arg_dict.get(f"{self.cli_arg_prefix}num_samples", -1)
-        files_to_use = arg_dict.get(f"{self.cli_arg_prefix}files_to_use")
+        files_to_use = arg_dict.get(f"{self.cli_arg_prefix}files_to_use", [".parquet"])
         # check which configuration (S3, LakeHouse, or Local) is specified
         s3_config_specified = 1 if s3_config is not None else 0
         local_config_specified = 1 if local_config is not None else 0
 
         # check that only one (S3, LakeHouse, or Local) configuration is specified
         if s3_config_specified + local_config_specified > 1:
             self.logger.error(
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access_factory_base.py` & `data_prep_toolkit-0.1.1/src/data_processing/data_access/data_access_factory_base.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access_local.py` & `data_prep_toolkit-0.1.1/src/data_processing/data_access/data_access_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,40 +314,40 @@
         """
         if self.output_folder is None:
             logger.error("local configuration is not defined, can't save metadata")
             return None
         metadata["source"] = {"name": self.input_folder, "type": "path"}
         metadata["target"] = {"name": self.output_folder, "type": "path"}
         return self.save_file(
-            file_path=os.path.join(self.output_folder, "metadata.json"),
-            bytes_data=json.dumps(metadata, indent=2).encode(),
+            path=os.path.join(self.output_folder, "metadata.json"),
+            data=json.dumps(metadata, indent=2).encode(),
         )
 
-    def get_file(self, file_path: str) -> bytes:
+    def get_file(self, path: str) -> bytes:
         """
         Gets the contents of a file as a byte array, decompressing gz files if needed.
 
         Args:
-            file_path (str): The path to the file.
+            path (str): The path to the file.
 
         Returns:
             bytes: The contents of the file as a byte array, or None if an error occurs.
         """
 
         try:
-            if file_path.endswith(".gz"):
-                with gzip.open(file_path, "rb") as f:
+            if path.endswith(".gz"):
+                with gzip.open(path, "rb") as f:
                     data = f.read()
             else:
-                with open(file_path, "rb") as f:
+                with open(path, "rb") as f:
                     data = f.read()
             return data
 
         except (FileNotFoundError, gzip.BadGzipFile) as e:
-            logger.error(f"Error reading file {file_path}: {e}")
+            logger.error(f"Error reading file {path}: {e}")
             raise e
 
     def get_folder_files(self, path: str, extensions: list[str] = None, return_data: bool = True) -> dict[str, bytes]:
         """
         Get a list of byte content of files. The path here is an absolute path and can be anywhere.
         The current limitation for S3 and Lakehouse is that it has to be in the same bucket
         :param path: file path
@@ -370,30 +370,30 @@
             return None
 
         matching_files = {}
         for filename in sorted(self._get_all_files_ext(path=path, extensions=extensions)):
             matching_files[filename] = _get_file_content(filename, return_data)
         return matching_files
 
-    def save_file(self, file_path: str, bytes_data: bytes) -> dict[str, Any]:
+    def save_file(self, path: str, data: bytes) -> dict[str, Any]:
         """
         Saves bytes to a file and returns a dictionary with file information.
 
         Args:
-            bytes_data (bytes): The bytes data to save.
-            file_path (str): The full name of the file to save.
+            data (bytes): The bytes data to save.
+            path (str): The full name of the file to save.
 
         Returns:
             dict or None: A dictionary with "name" and "size" keys if successful,
                         or None if saving fails.
         """
 
         try:
-            os.makedirs(os.path.dirname(file_path), exist_ok=True)
-            with open(file_path, "wb") as f:
-                f.write(bytes_data)
-            file_info = {"name": file_path, "size": os.path.getsize(file_path)}
+            os.makedirs(os.path.dirname(path), exist_ok=True)
+            with open(path, "wb") as f:
+                f.write(data)
+            file_info = {"name": path, "size": os.path.getsize(path)}
             return file_info
 
         except Exception as e:
-            logger.error(f"Error saving bytes to file {file_path}: {e}")
+            logger.error(f"Error saving bytes to file {path}: {e}")
             return None
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/data_access/data_access_s3.py` & `data_prep_toolkit-0.1.1/src/data_processing/data_access/data_access_s3.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/execution_configuration.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/execution_configuration.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,23 +23,25 @@
 
 
 class TransformExecutionConfiguration(CLIArgumentProvider):
     """
     A class specifying and validating transform execution configuration
     """
 
-    def __init__(self, name: str, pp: bool = True):
+    def __init__(self, name: str, print_params: bool = True):
         """
         Initialization
+        :param name: job name
+        :param print_params: flag to print parameters
         """
         self.pipeline_id = ""
         self.job_details = {}
         self.code_location = {}
         self.name = name
-        self.pp = pp
+        self.print_params = print_params
 
     def add_input_params(self, parser: argparse.ArgumentParser) -> None:
         """
         This method adds transformer specific parameter to parser
         :param parser: parser
         :return:
         """
@@ -70,14 +72,13 @@
         self.job_details = {
             "job category": "preprocessing",
             "job name": self.name,
             "job type": "pure python",
             "job id": captured["job_id"],
         }
         self.code_location = captured["code_location"]
-
-        if self.pp:
-            # print parameters
-            logger.info(f"pipeline id {self.pipeline_id}")
+        # print parameters
+        logger.info(f"pipeline id {self.pipeline_id}")
+        if self.print_params:
             logger.info(f"job details {self.job_details}")
-            logger.info(f"code location {self.code_location}")
+        logger.info(f"code location {self.code_location}")
         return True
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/runtime_configuration.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/pure_python/runtime_configuration.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/transform_launcher.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/pure_python/transform_launcher.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/transform_orchestrator.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/pure_python/transform_orchestrator.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from datetime import datetime
 
 from data_processing.data_access import DataAccessFactoryBase
 from data_processing.runtime import (
     TransformExecutionConfiguration,
     TransformRuntimeConfiguration,
 )
-from data_processing.runtime.pure_python import TransformTableProcessor
+from data_processing.runtime.pure_python import PythonTransformFileProcessor
 from data_processing.transform import TransformStatistics
 from data_processing.utils import get_logger
 
 
 logger = get_logger(__name__)
 
 
@@ -56,23 +56,23 @@
         # Print interval
         print_interval = int(len(files) / 100)
         if print_interval == 0:
             print_interval = 1
         # create statistics
         statistics = TransformStatistics()
         # create executor
-        executor = TransformTableProcessor(
-            data_access_factory=data_access_factory, statistics=statistics, params=runtime_config
+        executor = PythonTransformFileProcessor(
+            data_access_factory=data_access_factory, statistics=statistics, runtime_configuration=runtime_config
         )
         # process data
         logger.debug(f"{runtime_config.get_name()} Begin processing files")
         t_start = time.time()
         completed = 0
         for path in files:
-            executor.process_data(path)
+            executor.process_file(path)
             completed += 1
             if completed % print_interval == 0:
                 logger.info(f"Completed {completed} files in {(time.time() - t_start)/60} min")
         logger.debug("Done processing files, waiting for flush() completion.")
         # invoke flush to ensure that all results are returned
         start = time.time()
         executor.flush()
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/pure_python/transform_table_processor.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/transform_file_processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,46 +8,39 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 from typing import Any
 
-from data_processing.data_access import DataAccessFactoryBase
-from data_processing.runtime import (
-    AbstractTransformTableProcessor,
-    TransformRuntimeConfiguration,
-)
-from data_processing.transform import TransformStatistics
+import ray
+from data_processing.runtime import AbstractTransformFileProcessor
 
 
-class TransformTableProcessor(AbstractTransformTableProcessor):
+@ray.remote(scheduling_strategy="SPREAD")
+class RayTransformFileProcessor(AbstractTransformFileProcessor):
     """
-    This is the class implementing the worker class processing of a single pyarrow file
+    This is the class implementing the actual work/actor processing of a single file
     """
 
-    def __init__(
-        self,
-        data_access_factory: DataAccessFactoryBase,
-        statistics: TransformStatistics,
-        params: TransformRuntimeConfiguration,
-    ):
+    def __init__(self, params: dict[str, Any]):
         """
         Init method
-        :param data_access_factory - data access factory
-        :param statistics - reference to statistics class
-        :param params: transform configuration class
+        :param params: dictionary that has the following key
+            data_access_factory: data access factory
+            transform_class: local transform class
+            transform_params: dictionary of parameters for local transform creation
+            statistics: object reference to statistics
         """
-        # Create data access
         super().__init__()
-        self.data_access = data_access_factory.create_data_access()
-        # Add data access and statistics to the processor parameters
-        transform_params = dict(params.get_transform_params())
+        # Create data access
+        self.data_access = params.get("data_access_factory", None).create_data_access()
+        # Add data access ant statistics to the processor parameters
+        transform_params = params.get("transform_params", None)
         transform_params["data_access"] = self.data_access
-        transform_params["statistics"] = statistics
         # Create local processor
-        self.transform = params.get_transform_class()(transform_params)
+        self.transform = params.get("transform_class", None)(transform_params)
         # Create statistics
-        self.stats = statistics
+        self.stats = params.get("statistics", None)
 
     def _publish_stats(self, stats: dict[str, Any]) -> None:
-        self.stats.add_stats(stats)
+        self.stats.add_stats.remote(stats)
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/__init__.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from data_processing.runtime.ray.ray_utils import RayUtils
 from data_processing.runtime.ray.transform_statistics import TransformStatisticsRay
-from data_processing.runtime.ray.transform_runtime import DefaultTableTransformRuntimeRay
+from data_processing.runtime.ray.transform_runtime import DefaultRayTransformRuntime
 from data_processing.runtime.ray.runtime_configuration import RayTransformRuntimeConfiguration
-from data_processing.runtime.ray.transform_table_processor import TransformTableProcessorRay
+from data_processing.runtime.ray.transform_file_processor import RayTransformFileProcessor
 from data_processing.runtime.ray.execution_configuration import RayTransformExecutionConfiguration
 from data_processing.runtime.ray.transform_orchestrator import orchestrate
 from data_processing.runtime.ray.transform_launcher import RayTransformLauncher
-from data_processing.runtime.runtime_configuration import TransformRuntimeConfiguration
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/execution_configuration.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/execution_configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     A class specifying and validating Ray orchestrator configuration
     """
 
     def __init__(self, name: str):
         """
         Initialization
         """
-        super().__init__(name=name, pp=False)
+        super().__init__(name=name, print_params=False)
         self.worker_options = {}
         self.n_workers = 1
         self.creation_delay = 0
 
     def add_input_params(self, parser: argparse.ArgumentParser) -> None:
         """
         This method adds transformer specific parameter to parser
@@ -87,18 +87,16 @@
             "job name": self.name,
             "job type": "ray",
             "job id": captured["job_id"],
         }
 
         # print them
         logger.info(f"number of workers {self.n_workers} worker options {self.worker_options}")
-        logger.info(f"pipeline id {self.pipeline_id}; number workers {self.n_workers}")
-        logger.info(f"job details {self.job_details}")
-        logger.info(f"code location {self.code_location}")
         logger.info(f"actor creation delay {self.creation_delay}")
+        logger.info(f"job details {self.job_details}")
         return True
 
     def get_input_params(self) -> dict[str, Any]:
         """
         get input parameters for job_input_params in metadata
         :return: dictionary of parameters
         """
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/ray_utils.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/ray_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,20 +128,20 @@
             object_memory_gauge=object_memory_gauge,
         )
         running = 0
         t_start = time.time()
         completed = 0
         for path in files:
             if executors.has_free():  # still have room
-                executors.submit(lambda a, v: a.process_data.remote(v), path)
+                executors.submit(lambda a, v: a.process_file.remote(v), path)
                 running = running + 1
                 files_in_progress_gauge.set(running)
             else:  # need to wait for some actors
                 executors.get_next_unordered()
-                executors.submit(lambda a, v: a.process_data.remote(v), path)
+                executors.submit(lambda a, v: a.process_file.remote(v), path)
                 completed = completed + 1
                 files_completed_gauge.set(completed)
                 RayUtils.get_available_resources(
                     available_cpus_gauge=available_cpus_gauge,
                     available_gpus_gauge=available_gpus_gauge,
                     available_memory_gauge=available_memory_gauge,
                     object_memory_gauge=object_memory_gauge,
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/runtime_configuration.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/runtime_configuration.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 from data_processing.runtime import TransformRuntimeConfiguration
-from data_processing.runtime.ray import DefaultTableTransformRuntimeRay
+from data_processing.runtime.ray import DefaultRayTransformRuntime
 from data_processing.transform import TransformConfiguration
 
 
 class RayTransformRuntimeConfiguration(TransformRuntimeConfiguration):
     def __init__(
         self,
         transform_config: TransformConfiguration,
-        runtime_class: type[DefaultTableTransformRuntimeRay] = DefaultTableTransformRuntimeRay,
+        runtime_class: type[DefaultRayTransformRuntime] = DefaultRayTransformRuntime,
     ):
         """
         Initialization
         :param transform_config - base configuration class
         :param runtime_class: implementation of the transform runtime
         :param remove_from_metadata - list of parameters to remove from metadata
         """
         super().__init__(transform_config=transform_config)
         self.runtime_class = runtime_class
 
-    def create_transform_runtime(self) -> DefaultTableTransformRuntimeRay:
+    def create_transform_runtime(self) -> DefaultRayTransformRuntime:
         """
         Create transform runtime with the parameters captured during apply_input_params()
         :return: transform runtime object
         """
         return self.runtime_class(self.transform_config.get_transform_params())
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_launcher.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/transform_launcher.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_orchestrator.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/transform_orchestrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 import traceback
 from datetime import datetime
 
 import ray
 from data_processing.data_access import DataAccessFactoryBase
 from data_processing.runtime.ray import (
     RayTransformExecutionConfiguration,
+    RayTransformFileProcessor,
     RayTransformRuntimeConfiguration,
     RayUtils,
     TransformStatisticsRay,
-    TransformTableProcessorRay,
 )
 from data_processing.utils import get_logger
 from ray.util import ActorPool
 from ray.util.metrics import Gauge
 
 
 logger = get_logger(__name__)
@@ -80,15 +80,15 @@
             "transform_params": runtime.get_transform_config(
                 data_access_factory=data_access_factory, statistics=statistics, files=files
             ),
             "statistics": statistics,
         }
         logger.debug("Creating actors")
         processors = RayUtils.create_actors(
-            clazz=TransformTableProcessorRay,
+            clazz=RayTransformFileProcessor,
             params=processor_params,
             actor_options=preprocessing_params.worker_options,
             n_actors=preprocessing_params.n_workers,
             creation_delay=preprocessing_params.creation_delay,
         )
         processors_pool = ActorPool(processors)
         # create gauges
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_runtime.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/transform_runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from typing import Any
 
 from data_processing.data_access import DataAccessFactoryBase
 from ray.actor import ActorHandle
 
 
-class DefaultTableTransformRuntimeRay:
+class DefaultRayTransformRuntime:
     """
     Transformer runtime used by processor to to create Transform specific environment
     """
 
     def __init__(self, params: dict[str, Any]):
         """
         Create/config this runtime.
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_statistics.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/ray/transform_statistics.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,16 +24,18 @@
     It can be extended for specific processors
     """
 
     def __init__(self, params: dict[str, Any]):
         super().__init__()
         self.data_write_counter = Counter("data_written", "Total data written bytes")
         self.data_read_counter = Counter("data_read", "Total data read bytes")
-        self.source_document_counter = Counter("source_files_processed", "Total source document processed")
-        self.result_document_counter = Counter("result_files_written", "Total result documents written")
+        self.source_files_counter = Counter("source_files_processed", "Total source files processed")
+        self.result_files_counter = Counter("result_files_written", "Total result files written")
+        self.source_documents_counter = Counter("source_documents_processed", "Total source document processed")
+        self.result_documents_counter = Counter("result_documents_written", "Total result documents written")
         self.empty_table_counter = Counter("empty_tables", "Total empty tables read")
         self.failed_read_counter = Counter("failed_read_files", "Total read failed files")
         self.failed_write_counter = Counter("failed_write_files", "Total write failed files")
         self.transform_exceptions_counter = Counter("transform_exceptions", "Transform exception occurred")
 
     def add_stats(self, stats=dict[str, Any]) -> None:
         """
@@ -41,19 +43,23 @@
         :param stats - dictionary creating new statistics
         :return: None
         """
         for key, val in stats.items():
             if val > 0:
                 self.stats[key] = self.stats.get(key, 0) + val
                 if key == "source_files":
-                    self.source_document_counter.inc(val)
+                    self.source_files_counter.inc(val)
                 if key == "source_size":
                     self.data_read_counter.inc(val)
                 if key == "result_files":
-                    self.result_document_counter.inc(val)
+                    self.result_files_counter.inc(val)
+                if key == "source_doc_count":
+                    self.source_documents_counter.inc(val)
+                if key == "result_doc_count":
+                    self.result_documents_counter.inc(val)
                 if key == "skipped empty tables":
                     self.empty_table_counter.inc(val)
                 if key == "failed_reads":
                     self.failed_read_counter.inc(val)
                 if key == "failed_writes":
                     self.failed_write_counter.inc(val)
                 if key == "transform execution exception":
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/ray/transform_table_processor.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/pure_python/transform_file_processor.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,39 +8,46 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 from typing import Any
 
-import ray
-from data_processing.runtime import AbstractTransformTableProcessor
+from data_processing.data_access import DataAccessFactoryBase
+from data_processing.runtime import (
+    AbstractTransformFileProcessor,
+)
+from data_processing.transform import TransformStatistics
+from data_processing.runtime.pure_python import PythonTransformRuntimeConfiguration
 
 
-@ray.remote(scheduling_strategy="SPREAD")
-class TransformTableProcessorRay(AbstractTransformTableProcessor):
+class PythonTransformFileProcessor(AbstractTransformFileProcessor):
     """
-    This is the class implementing the actual work/actor processing of a single pyarrow file
+    This is the class implementing the worker class processing of a single file
     """
 
-    def __init__(self, params: dict[str, Any]):
+    def __init__(
+        self,
+        data_access_factory: DataAccessFactoryBase,
+        statistics: TransformStatistics,
+        runtime_configuration: PythonTransformRuntimeConfiguration,
+    ):
         """
         Init method
-        :param params: dictionary that has the following key
-            data_access_factory: data access factory
-            transform_class: local transform class
-            transform_params: dictionary of parameters for local transform creation
-            statistics: object reference to statistics
+        :param data_access_factory - data access factory
+        :param statistics - reference to statistics class
+        :param runtime_configuration: transform configuration class
         """
-        super().__init__()
         # Create data access
-        self.data_access = params.get("data_access_factory", None).create_data_access()
-        # Add data access ant statistics to the processor parameters
-        transform_params = params.get("transform_params", None)
+        super().__init__()
+        self.data_access = data_access_factory.create_data_access()
+        # Add data access and statistics to the processor parameters
+        transform_params = dict(runtime_configuration.get_transform_params())
         transform_params["data_access"] = self.data_access
+        transform_params["statistics"] = statistics
         # Create local processor
-        self.transform = params.get("transform_class", None)(transform_params)
+        self.transform = runtime_configuration.get_transform_class()(transform_params)
         # Create statistics
-        self.stats = params.get("statistics", None)
+        self.stats = statistics
 
     def _publish_stats(self, stats: dict[str, Any]) -> None:
-        self.stats.add_stats.remote(stats)
+        self.stats.add_stats(stats)
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/runtime_configuration.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/runtime_configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 from argparse import ArgumentParser, Namespace
 from typing import Any
 
-from data_processing.transform import AbstractTableTransform, TransformConfiguration
+from data_processing.transform import AbstractBinaryTransform, TransformConfiguration
 from data_processing.utils import CLIArgumentProvider
 
 
 class TransformRuntimeConfiguration(CLIArgumentProvider):
     def __init__(self, transform_config: TransformConfiguration):
         """
         Initialization
@@ -30,20 +30,20 @@
 
     def apply_input_params(self, args: Namespace) -> bool:
         return self.transform_config.apply_input_params(args)
 
     def get_input_params(self) -> dict[str, Any]:
         return self.transform_config.get_input_params()
 
-    def get_transform_class(self) -> type[AbstractTableTransform]:
+    def get_transform_class(self) -> type[AbstractBinaryTransform]:
         """
-        Get the class extending AbstractTableTransform which implements a specific transformation.
+        Get the class extending AbstractTransform which implements a specific transformation.
         The class will generally be instantiated with a dictionary of configuration produced by
         the associated TransformRuntime get_transform_config() method.
-        :return: class extending AbstractTableTransform
+        :return: class extending AbstractTransform
         """
         return self.transform_config.get_transform_class()
 
     def get_name(self):
         return self.transform_config.get_name()
 
     def get_transform_metadata(self) -> dict[str, Any]:
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/transform_launcher.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/transform_launcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,37 +39,34 @@
     def launch(self):
         raise ValueError("must be implemented by subclass")
 
     def get_transform_name(self) -> str:
         return self.name
 
 
-def multi_luncher(params: dict[str, Any], launcher: AbstractTransformLauncher) -> int:
+def multi_launcher(params: dict[str, Any], launcher: AbstractTransformLauncher) -> int:
     """
     Multi launcher. A function orchestrating multiple launcher executions
     :param params: A set of parameters containing an array of configs (s3, local, etc)
     :param launcher: An actual launcher for a specific runtime
     :return: number of launches
     """
     # find config parameter
-    config = None
-    for key in params.keys():
-        if key.startswith("data") and key.endswith("config"):
-            config = key
-            break
+    config = ParamsUtils.get_config_parameter(params)
     if config is None:
-        logger.warning("Could no find config parameter")
         return 1
+    # get and validate config value
     config_value = params[config]
     if type(config_value) is not list:
         logger.warning("config value is not a list")
         return 1
     # remove config key from the dictionary
     launch_params = dict(params)
     del launch_params[config]
+    # Loop through all parameters
     n_launches = 0
     for conf in config_value:
         # populate individual config and launch
         launch_params[config] = conf
         sys.argv = ParamsUtils.dict_to_req(d=launch_params)
         res = launcher.launch()
         if res > 0:
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/runtime/transform_table_processor.py` & `data_prep_toolkit-0.1.1/src/data_processing/runtime/transform_file_processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,161 +10,158 @@
 # limitations under the License.
 ################################################################################
 
 import time
 import traceback
 from typing import Any
 
-import pyarrow as pa
 from data_processing.utils import TransformUtils, get_logger
 
 
-class AbstractTransformTableProcessor:
+class AbstractTransformFileProcessor:
     """
-    This is the the base class implementing processing of a single pyarrow file
+    This is the the base class implementing processing of a single binary file
     """
 
     def __init__(self):
         """
         Init method
         """
         self.data_access = None
         self.transform = None
         self.stats = None
         self.last_file_name = None
+        self.last_extension = None
         self.last_file_name_next_index = None
         self.logger = get_logger(__name__)
 
-    def process_data(self, f_name: str) -> None:
+    def process_file(self, f_name: str) -> None:
         """
-        Method processing an individual table
+        Method processing an individual file
         :param f_name: file name
         :return: None
         """
         self.logger.debug(f"Begin processing file {f_name}")
         if self.data_access is None:
             self.logger.warning("No data_access found. Returning.")
             return
         t_start = time.time()
-        # Read source table
-        table = self.data_access.get_table(path=f_name)
-        if table is None:
-            self.logger.warning("File read resulted in None. Returning.")
+        # Read source file
+        filedata = self.data_access.get_file(path=f_name)
+        if filedata is None:
+            self.logger.warning(f"File read resulted in None for {f_name}. Returning.")
             self._publish_stats({"failed_reads": 1})
             return
-        self._publish_stats({"source_files": 1, "source_size": table.nbytes})
-        # Process input table
+        self._publish_stats({"source_files": 1, "source_size": len(filedata)})
+        # Process input file
         try:
-            if table.num_rows > 0:
-                # execute local processing
-                self.logger.debug(f"Begin transforming table from {f_name}")
-                out_tables, stats = self.transform.transform(table=table)
-                self.logger.debug(f"Done transforming table from {f_name}")
-                self.last_file_name = TransformUtils.get_file_extension(f_name)[0]
-                self.last_file_name_next_index = None
-            else:
-                self.logger.info(f"table: {f_name} is empty, skipping processing")
-                self._publish_stats({"skipped empty tables": 1})
-                return
+            # execute local processing
+            name_extension = TransformUtils.get_file_extension(f_name)
+            self.logger.debug(f"Begin transforming file {f_name}")
+            out_files, stats = self.transform.transform_binary(byte_array=filedata, ext=name_extension[1])
+            self.logger.debug(f"Done transforming file {f_name}")
+            self.last_file_name = name_extension[0]
+            self.last_file_name_next_index = None
+            self.last_extension = name_extension[1]
             # save results
-            self._submit_table(t_start=t_start, out_tables=out_tables, stats=stats)
+            self._submit_file(t_start=t_start, out_files=out_files, stats=stats)
         except Exception as e:
             self.logger.warning(f"Exception {e} processing file {f_name}: {traceback.format_exc()}")
             self._publish_stats({"transform execution exception": 1})
 
     def flush(self) -> None:
         """
-        This is supporting method for transformers, that implement buffering of tables, for example coalesce.
-        These transformers can have buffers containing tables that were not written to the output. Flush is
-        the hook for them to return back locally stored tables and their statistics.
+        This is supporting method for transformers, that implement buffering of data, for example resize.
+        These transformers can have buffers containing data that were not written to the output. Flush is
+        the hook for them to return back locally stored data and their statistics.
         :return: None
         """
-        t_start = time.time()
         if self.last_file_name is None:
             # for some reason a given worker never processed anything. Happens in testing
             # when the amount of workers is greater then the amount of files
             self.logger.debug("skipping flush, no name for file is defined")
             return
         try:
+            t_start = time.time()
             # get flush results
             self.logger.debug(f"Begin flushing transform")
-            out_tables, stats = self.transform.flush()
-            self.logger.debug(f"Done flushing transform, got {len(out_tables)} tables")
-            # Here we are using the name of the last table, that we were processing
-            self._submit_table(t_start=t_start, out_tables=out_tables, stats=stats)
+            out_files, stats = self.transform.flush_binary()
+            self.logger.debug(f"Done flushing transform, got {len(out_files)} files")
+            # Here we are using the name of the last file, that we were processing
+            self._submit_file(t_start=t_start, out_files=out_files, stats=stats)
         except Exception as e:
             self.logger.warning(f"Exception {e} flushing: {traceback.format_exc()}")
             self._publish_stats({"transform execution exception": 1})
 
-    def _submit_table(self, t_start: float, out_tables: list[pa.Table], stats: dict[str, Any]) -> None:
+    def _submit_file(self, t_start: float, out_files: list[tuple[bytes, str]], stats: dict[str, Any]) -> None:
         """
-        This is a helper method writing output tables and statistics
+        This is a helper method writing output files and statistics
         :param t_start: execution start time
-        :param out_tables: list of tables to write
+        :param out_files: list of files to write
         :param stats: execution statistics to populate
         :return: None
         """
         self.logger.debug(
-            f"submitting tables under file named {self.last_file_name}.parquet, " f"number of tables {len(out_tables)}"
+            f"submitting files under file named {self.last_file_name}{self.last_extension} "
+            f"number of files {len(out_files)}"
         )
-        # Compute output file location. Preserve sub folders for Wisdom
-        match len(out_tables):
+        match len(out_files):
             case 0:
-                # no tables - save input file name for flushing
+                # no output file - save input file name for flushing
                 self.logger.debug(
-                    f"Transform did not produce a transformed table for " f"file {self.last_file_name}.parquet"
+                    f"Transform did not produce a transformed file for " f"file {self.last_file_name}.parquet"
                 )
             case 1:
-                # we have exactly 1 table
-                output_name = self.data_access.get_output_location(path=f"{self.last_file_name}.parquet")
-                self.logger.debug(f"Writing transformed file {self.last_file_name}.parquet to {output_name}")
-                if TransformUtils.verify_no_duplicate_columns(table=out_tables[0], file=output_name):
-                    output_file_size, save_res = self.data_access.save_table(path=output_name, table=out_tables[0])
-                    if save_res is not None:
-                        # Store execution statistics. Doing this async
-                        self._publish_stats(
-                            {
-                                "result_files": 1,
-                                "result_size": out_tables[0].nbytes,
-                                "table_processing": time.time() - t_start,
-                            }
-                        )
-                    else:
-                        self.logger.warning(f"Failed to write file {output_name}")
-                        self._publish_stats({"failed_writes": 1})
+                # we have exactly 1 output file
+                file_ext = out_files[0]
+                output_name = self.data_access.get_output_location(path=f"{self.last_file_name}{file_ext[1]}")
+                self.logger.debug(
+                    f"Writing transformed file {self.last_file_name}{self.last_extension} " f"to {output_name}"
+                )
+                save_res = self.data_access.save_file(path=output_name, data=file_ext[0])
+                if save_res is not None:
+                    # Store execution statistics. Doing this async
+                    self._publish_stats(
+                        {
+                            "result_files": 1,
+                            "result_size": len(file_ext[0]),
+                            "processing_time": time.time() - t_start,
+                        }
+                    )
+                else:
+                    self.logger.warning(f"Failed to write file {output_name}")
+                    self._publish_stats({"failed_writes": 1})
                 self.last_file_name_next_index = 0
             case _:
-                # we have more then 1 table
-                table_sizes = 0
+                # we have more then 1 file
+                file_sizes = 0
                 output_file_name = self.data_access.get_output_location(path=self.last_file_name)
                 start_index = self.last_file_name_next_index
                 if start_index is None:
                     start_index = 0
-                count = len(out_tables)
+                count = len(out_files)
                 for index in range(count):
-                    output_name_indexed = f"{output_file_name}_{start_index + index}.parquet"
-                    if TransformUtils.verify_no_duplicate_columns(table=out_tables[index], file=output_name_indexed):
-                        table_sizes += out_tables[index].nbytes
-                        self.logger.debug(
-                            f"Writing transformed file {self.last_file_name}.parquet, {index + 1} "
-                            f"of {count}  to {output_name_indexed}"
-                        )
-                        output_file_size, save_res = self.data_access.save_table(
-                            path=output_name_indexed, table=out_tables[index]
-                        )
-                        if save_res is None:
-                            self.logger.warning(f"Failed to write file {output_name_indexed}")
-                            self._publish_stats({"failed_writes": 1})
-                            break
+                    file_ext = out_files[index]
+                    output_name_indexed = f"{output_file_name}_{start_index + index}{file_ext[1]}"
+                    file_sizes += len(file_ext[0])
+                    self.logger.debug(
+                        f"Writing transformed file {self.last_file_name}{self.last_extension}, {index + 1} "
+                        f"of {count}  to {output_name_indexed}"
+                    )
+                    save_res = self.data_access.save_file(path=output_name_indexed, data=file_ext[0])
+                    if save_res is None:
+                        self.logger.warning(f"Failed to write file {output_name_indexed}")
+                        self._publish_stats({"failed_writes": 1})
+                        break
                 self.last_file_name_next_index = start_index + count
                 self._publish_stats(
                     {
-                        "result_files": len(out_tables),
-                        "result_size": table_sizes,
-                        "table_processing": time.time() - t_start,
+                        "result_files": len(out_files),
+                        "result_size": file_sizes,
+                        "processing_time": time.time() - t_start,
                     }
                 )
         # save transformer's statistics
         if len(stats) > 0:
             self._publish_stats(stats)
 
     def _publish_stats(self, stats: dict[str, Any]) -> None:
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/test_support/abstract_test.py` & `data_prep_toolkit-0.1.1/src/data_processing/test_support/abstract_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/test_support/data_access/data_access_factory_test.py` & `data_prep_toolkit-0.1.1/src/data_processing/test_support/data_access/data_access_factory_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/test_support/launch/transform_test.py` & `data_prep_toolkit-0.1.1/src/data_processing/test_support/launch/transform_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/test_support/transform/noop_transform.py` & `data_prep_toolkit-0.1.1/src/data_processing/test_support/transform/noop_transform.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/test_support/transform/transform_test.py` & `data_prep_toolkit-0.1.1/src/data_processing/test_support/transform/transform_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/transform/table_transform.py` & `data_prep_toolkit-0.1.1/src/data_processing/transform/binary_transform.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,43 +8,46 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 from typing import Any
 
-import pyarrow as pa
 
-
-class AbstractTableTransform:
+class AbstractBinaryTransform:
     """
-    Converts input to output table
-    Sub-classes must provide the transform() method to provide the conversion of one table to 0 or more new tables.
+    Converts input binary file to output file(s) (binary)
+    Sub-classes must provide the transform() method to provide the conversion of one binary files to 0 or
+    more new binary files.
     """
 
     def __init__(self, config: dict[str, Any]):
         """
         Initialize based on the dictionary of configuration information.
+        This simply stores the given instance in this instance for later use.
         """
         self.config = config
 
-    def transform(self, table: pa.Table) -> tuple[list[pa.Table], dict[str, Any]]:
+    def transform_binary(self, byte_array: bytes, ext: str) -> tuple[list[tuple[bytes, str]], dict[str, Any]]:
         """
-        Converts input table into an output table.
-        If there is an error, an exception must be raised - exit()ing is not generally allowed when running in Ray.
-        :param table: input table
-        :return: a tuple of a list of 0 or more converted tables and a dictionary of statistics that will be
-        propagated to metadata
+        Converts input file into o or more output files.
+        If there is an error, an exception must be raised - exit()ing is not generally allowed.
+        :param byte_array: contents of the input file to be transformed.
+        :param ext: the file extension of the file containing the given byte_array.
+        :return: a tuple of a list of 0 or more tuples and a dictionary of statistics that will be propagated
+                to metadata.  Each element of the return list, is a tuple of the transformed bytes and a string
+                holding the extension to be used when writing out the new bytes.
         """
         raise NotImplemented()
 
-    def flush(self) -> tuple[list[pa.Table], dict[str, Any]]:
+    def flush_binary(self) -> tuple[list[tuple[bytes, str]], dict[str, Any]]:
         """
-        This is supporting method for transformers, that implement buffering of tables, for example coalesce.
-        These transformers can have buffers containing tables that were not written to the output. Flush is
-        the hook for them to return back locally stored tables and their statistics. The majority of transformers
-        should use default implementation.
-        If there is an error, an exception must be raised - exit()ing is not generally allowed when running in Ray.
-        :return: a tuple of a list of 0 or more converted tables and a dictionary of statistics that will be
-        propagated to metadata
+        This is supporting method for transformers, that implement buffering of data, for example coalesce.
+        These transformers can have buffers containing data that were not written to the output immediately.
+        Flush is the hook for them to return back locally stored data and their statistics.
+        The majority of transformers are expected not to use such buffering and can use this default implementation.
+        If there is an error, an exception must be raised - exit()ing is not generally allowed.
+        :return: a tuple of a list of 0 or more tuples and a dictionary of statistics that will be propagated
+                to metadata.  Each element of the return list, is a tuple of the transformed bytes and a string
+                holding the extension to be used when writing out the new bytes.
         """
         return [], {}
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/transform/transform_configuration.py` & `data_prep_toolkit-0.1.1/src/data_processing/transform/transform_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,41 +9,41 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 from argparse import ArgumentParser
 from typing import Any
 
-from data_processing.transform import AbstractTableTransform
+from data_processing.transform import AbstractBinaryTransform
 from data_processing.utils import CLIArgumentProvider
 
 
 class TransformConfiguration(CLIArgumentProvider):
     """
     This is a base transform configuration class defining transform's input/output parameter
     """
 
-    def __init__(self, name: str, transform_class: type[AbstractTableTransform], remove_from_metadata: list[str] = []):
+    def __init__(self, name: str, transform_class: type[AbstractBinaryTransform], remove_from_metadata: list[str] = []):
         """
         Initialization
         :param name: transformer name
         :param transform_class: transform implementation class
         :param remove_from_metadata - list of parameters to remove from metadata
         """
         self.name = name
         self.transform_class = transform_class
         self.remove_from_metadata = remove_from_metadata
         self.params = {}
 
-    def get_transform_class(self) -> type[AbstractTableTransform]:
+    def get_transform_class(self) -> type[AbstractBinaryTransform]:
         """
-        Get the class extending AbstractTableTransform which implements a specific transformation.
+        Get the class extending AbstractTransform which implements a specific transformation.
         The class will generally be instantiated with a dictionary of configuration produced by
         the associated TransformRuntime get_transform_config() method.
-        :return: class extending AbstractTableTransform
+        :return: class extending AbstractTransform
         """
         return self.transform_class
 
     def get_name(self):
         return self.name
 
     def get_transform_metadata(self) -> dict[str, Any]:
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/transform/transform_statistics.py` & `data_prep_toolkit-0.1.1/src/data_processing/transform/transform_statistics.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/utils/cli_utils.py` & `data_prep_toolkit-0.1.1/src/data_processing/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/utils/config.py` & `data_prep_toolkit-0.1.1/src/data_processing/utils/config.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/utils/log.py` & `data_prep_toolkit-0.1.1/src/data_processing/utils/log.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/utils/params_utils.py` & `data_prep_toolkit-0.1.1/src/data_processing/utils/params_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,14 +88,29 @@
             first = False
         all_text = all_text.strip()
         if as_value:
             all_text = all_text + " }"
         return all_text
 
     @staticmethod
+    def get_config_parameter(params: dict[str, Any]) -> str:
+        """
+        Get parameters for multi launch
+        :param params: original parameters
+        :return: tuple of name of repeated parameter, list of repeated parameters, and dict of non changing ones
+        """
+        # find config parameter
+        config = None
+        for key in params.keys():
+            if key.startswith("data") and key.endswith("config"):
+                config = key
+                break
+        return config
+
+    @staticmethod
     def get_ast_help_and_example_text(help_dict: dict[str, str], examples: list[dict[str, Any]]):
         initial_indent = ""
         indent_per_level = "   "
         help_txt = ParamsUtils.__dict_to_str(help_dict, initial_indent, indent_per_level, False)
         if examples is not None:
             example_txt = "\n" + initial_indent
             if len(examples) == 1:
@@ -131,15 +146,15 @@
             parser.add_argument(
                 "--s3_cred",
                 type=ast.literal_eval,
                 default=None,
                 help="ast string of options for s3 credentials\n" +
                      ParamsUtils.get_ast_help_text(help_example_dict)
             )
-        :return:  a string to be included in help text, usually concantentated with the general
+        :return:  a string to be included in help text, usually concatenated with the general
         parameter help text.
         """
 
         help_dict = {}
         example_dict = {}
         for key, value in help_example_dict.items():
             if not isinstance(value, list):
```

### Comparing `data_prep_toolkit-0.1.0/src/data_processing/utils/transform_utils.py` & `data_prep_toolkit-0.1.1/src/data_processing/utils/transform_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,15 @@
         :param encoding:The encoding to use while decoding the content. Default is 'utf-8'
         :return: str: The decoded content as a string if successful,
                       otherwise empty string if an error occurs during decoding.
         """
         try:
             content_string = content_bytes.decode(encoding)
             return content_string
-        except Exception as e:
-            logger.error(f"Error -> {e}")
+        except Exception:
             return ""
 
     @staticmethod
     def get_file_extension(file_path) -> list[str]:
         """
         Get the file's root and extension from the given file path.
         :param file_path : The path of the file.
```

### Comparing `data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/daf_local_test.py` & `data_prep_toolkit-0.1.1/test/data_processing_tests/data_access/daf_local_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/data_access_local_test.py` & `data_prep_toolkit-0.1.1/test/data_processing_tests/data_access/data_access_local_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/data_access_s3_test.py` & `data_prep_toolkit-0.1.1/test/data_processing_tests/data_access/data_access_s3_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test/data_processing_tests/data_access/sample_input_data_test.py` & `data_prep_toolkit-0.1.1/test/data_processing_tests/data_access/sample_input_data_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test/data_processing_tests/launch/pure_python/launcher_test.py` & `data_prep_toolkit-0.1.1/test/data_processing_tests/launch/pure_python/launcher_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test/data_processing_tests/launch/pure_python/multi_launcher_test.py` & `data_prep_toolkit-0.1.1/test/data_processing_tests/launch/pure_python/multi_launcher_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 import os
 
-from data_processing.runtime import multi_luncher
+from data_processing.runtime import multi_launcher
 from data_processing.runtime.pure_python import PythonTransformLauncher
 from data_processing.test_support.transform import NOOPPythonTransformConfiguration
-
 from data_processing.utils import ParamsUtils
 
 
 s3_cred = {
     "access_key": "access",
     "secret_key": "secret",
     "url": "https://s3.us-east.cloud-object-storage.appdomain.cloud",
@@ -59,20 +58,20 @@
         "data_s3_cred": ParamsUtils.convert_to_ast(s3_cred),
         "data_s3_config": [ParamsUtils.convert_to_ast(s3_conf)],
         "runtime_pipeline_id": "pipeline_id",
         "runtime_job_id": "job_id",
         "runtime_code_location": ParamsUtils.convert_to_ast(code_location),
     }
     # s3 configuration
-    res = multi_luncher(params=params, launcher=TestLauncherPython())
+    res = multi_launcher(params=params, launcher=TestLauncherPython())
     assert 1 == res
     params = {
         "data_max_files": -1,
         "data_checkpointing": False,
         "data_local_config": [ParamsUtils.convert_to_ast(local_conf)],
         "runtime_pipeline_id": "pipeline_id",
         "runtime_job_id": "job_id",
         "runtime_code_location": ParamsUtils.convert_to_ast(code_location),
     }
     # local configuration
-    res = multi_luncher(params=params, launcher=TestLauncherPython())
+    res = multi_launcher(params=params, launcher=TestLauncherPython())
     assert 1 == res
```

### Comparing `data_prep_toolkit-0.1.0/test/data_processing_tests/launch/pure_python/test_noop_launch.py` & `data_prep_toolkit-0.1.1/test/data_processing_tests/launch/pure_python/test_noop_launch.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test/data_processing_tests/launch/ray/launcher_test.py` & `data_prep_toolkit-0.1.1/test/data_processing_tests/launch/ray/launcher_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test/data_processing_tests/launch/ray/multi_launcher_test.py` & `data_prep_toolkit-0.1.1/test/data_processing_tests/launch/ray/multi_launcher_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 import os
 
-from data_processing.runtime import multi_luncher
+from data_processing.runtime import multi_launcher
 from data_processing.runtime.ray import RayTransformLauncher
-from data_processing.utils import ParamsUtils
 from data_processing.test_support.transform import NOOPRayTransformConfiguration
+from data_processing.utils import ParamsUtils
 
 
 s3_cred = {
     "access_key": "access",
     "secret_key": "secret",
     "url": "https://s3.us-east.cloud-object-storage.appdomain.cloud",
 }
@@ -61,20 +61,20 @@
         "data_s3_cred": ParamsUtils.convert_to_ast(s3_cred),
         "data_s3_config": [ParamsUtils.convert_to_ast(s3_conf)],
         "runtime_pipeline_id": "pipeline_id",
         "runtime_job_id": "job_id",
         "runtime_code_location": ParamsUtils.convert_to_ast(code_location),
     }
     # s3 configuration
-    res = multi_luncher(params=params, launcher=TestLauncherRay())
+    res = multi_launcher(params=params, launcher=TestLauncherRay())
     assert 1 == res
     params = {
         "data_max_files": -1,
         "data_checkpointing": False,
         "data_local_config": [ParamsUtils.convert_to_ast(local_conf)],
         "runtime_pipeline_id": "pipeline_id",
         "runtime_job_id": "job_id",
         "runtime_code_location": ParamsUtils.convert_to_ast(code_location),
     }
     # local configuration
-    res = multi_luncher(params=params, launcher=TestLauncherRay())
+    res = multi_launcher(params=params, launcher=TestLauncherRay())
     assert 1 == res
```

### Comparing `data_prep_toolkit-0.1.0/test/data_processing_tests/launch/ray/ray_util_test.py` & `data_prep_toolkit-0.1.1/test/data_processing_tests/launch/ray/ray_util_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test/data_processing_tests/launch/ray/test_noop_launch.py` & `data_prep_toolkit-0.1.1/test/data_processing_tests/launch/ray/test_noop_launch.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test/data_processing_tests/transform/test_noop.py` & `data_prep_toolkit-0.1.1/test/data_processing_tests/transform/test_noop.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test/data_processing_tests/util/transform_utils_test.py` & `data_prep_toolkit-0.1.1/test/data_processing_tests/util/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/ds1/sample1.parquet` & `data_prep_toolkit-0.1.1/test-data/data_processing/daf/input/ds1/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/ds1/sample2.parquet` & `data_prep_toolkit-0.1.1/test-data/data_processing/daf/input/ds1/sample2.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test-data/data_processing/daf/input/ds2/sample3.parquet` & `data_prep_toolkit-0.1.1/test-data/data_processing/daf/input/ds2/sample3.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test-data/data_processing/daf/output/ds1/sample1.parquet` & `data_prep_toolkit-0.1.1/test-data/data_processing/daf/output/ds1/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test-data/data_processing/input/sample1.parquet` & `data_prep_toolkit-0.1.1/test-data/data_processing/input/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test-data/data_processing/input_multiple/sample1.parquet` & `data_prep_toolkit-0.1.1/test-data/data_processing/input_multiple/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test-data/data_processing/input_multiple/sample2.parquet` & `data_prep_toolkit-0.1.1/test-data/data_processing/input_multiple/sample2.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test-data/data_processing/input_multiple/sample3.parquet` & `data_prep_toolkit-0.1.1/test-data/data_processing/input_multiple/sample3.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/expected/metadata.json` & `data_prep_toolkit-0.1.1/test-data/data_processing/ray/noop/expected/metadata.json`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/expected/sample1.parquet` & `data_prep_toolkit-0.1.1/test-data/data_processing/ray/noop/expected/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/expected/subdir/test1.parquet` & `data_prep_toolkit-0.1.1/test-data/data_processing/ray/noop/expected/subdir/test1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/input/sample1.parquet` & `data_prep_toolkit-0.1.1/test-data/data_processing/ray/noop/input/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.1.0/test-data/data_processing/ray/noop/input/subdir/test1.parquet` & `data_prep_toolkit-0.1.1/test-data/data_processing/ray/noop/input/subdir/test1.parquet`

 * *Files identical despite different names*

