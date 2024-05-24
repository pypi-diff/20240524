# Comparing `tmp/polars_ta-0.2.6.tar.gz` & `tmp/polars_ta-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polars_ta-0.2.6.tar", last modified: Sun May 12 12:01:43 2024, max compression
+gzip compressed data, was "polars_ta-0.2.7.tar", last modified: Fri May 24 13:14:53 2024, max compression
```

## Comparing `polars_ta-0.2.6.tar` & `polars_ta-0.2.7.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:01:43.288202 polars_ta-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-12 12:01:39.000000 polars_ta-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-05-12 12:01:43.288202 polars_ta-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-05-12 12:01:39.000000 polars_ta-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:01:43.280202 polars_ta-0.2.6/polars_ta/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:01:43.280202 polars_ta-0.2.6/polars_ta/candles/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/candles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/candles/cdl1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/candles/cdl1_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/candles/cdl2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/noise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:01:43.280202 polars_ta-0.2.6/polars_ta/performance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/performance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/performance/drawdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/performance/returns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:01:43.280202 polars_ta-0.2.6/polars_ta/prefix/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/prefix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/prefix/cdl.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/prefix/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/prefix/ta.py
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/prefix/talib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/prefix/tdx.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/prefix/wq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:01:43.280202 polars_ta-0.2.6/polars_ta/reports/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/reports/cicc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:01:43.284202 polars_ta-0.2.6/polars_ta/ta/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/ta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/ta/momentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/ta/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/ta/overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/ta/price.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/ta/statistic.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/ta/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/ta/volatility.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/ta/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:01:43.284202 polars_ta-0.2.6/polars_ta/talib/
--rw-r--r--   0 runner    (1001) docker     (127)    34381 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/talib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:01:43.284202 polars_ta-0.2.6/polars_ta/tdx/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/tdx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/tdx/_nb.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/tdx/_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/tdx/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/tdx/choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/tdx/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/tdx/logical.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/tdx/moving_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/tdx/over_bought_over_sold.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/tdx/pressure_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/tdx/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/tdx/statistic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/tdx/trend.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/tdx/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:01:43.288202 polars_ta-0.2.6/polars_ta/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/utils/numba_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/utils/pandas_.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/utils/pit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/utils/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:01:43.288202 polars_ta-0.2.6/polars_ta/wq/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/wq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/wq/_nb.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/wq/_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/wq/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/wq/cross_sectional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/wq/logical.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/wq/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/wq/time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/wq/transformational.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-12 12:01:39.000000 polars_ta-0.2.6/polars_ta/wq/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:01:43.288202 polars_ta-0.2.6/polars_ta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-05-12 12:01:43.000000 polars_ta-0.2.6/polars_ta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-12 12:01:43.000000 polars_ta-0.2.6/polars_ta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 12:01:43.000000 polars_ta-0.2.6/polars_ta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-12 12:01:43.000000 polars_ta-0.2.6/polars_ta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-12 12:01:43.000000 polars_ta-0.2.6/polars_ta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-12 12:01:39.000000 polars_ta-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 12:01:43.288202 polars_ta-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 12:01:39.000000 polars_ta-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:14:53.980288 polars_ta-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-24 13:14:46.000000 polars_ta-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-05-24 13:14:53.980288 polars_ta-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-05-24 13:14:46.000000 polars_ta-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:14:53.972288 polars_ta-0.2.7/polars_ta/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:14:53.972288 polars_ta-0.2.7/polars_ta/candles/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/candles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/candles/cdl1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/candles/cdl1_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/candles/cdl2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/noise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:14:53.972288 polars_ta-0.2.7/polars_ta/performance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/performance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/performance/drawdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/performance/returns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:14:53.972288 polars_ta-0.2.7/polars_ta/prefix/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/prefix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/prefix/cdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/prefix/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/prefix/ta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/prefix/talib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/prefix/tdx.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/prefix/wq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:14:53.972288 polars_ta-0.2.7/polars_ta/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/reports/cicc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:14:53.976287 polars_ta-0.2.7/polars_ta/ta/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/ta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/ta/momentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/ta/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/ta/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/ta/price.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/ta/statistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/ta/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/ta/volatility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/ta/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:14:53.976287 polars_ta-0.2.7/polars_ta/talib/
+-rw-r--r--   0 runner    (1001) docker     (127)    34381 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/talib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:14:53.976287 polars_ta-0.2.7/polars_ta/tdx/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/tdx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/tdx/_nb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/tdx/_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/tdx/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/tdx/choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/tdx/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/tdx/logical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/tdx/moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/tdx/over_bought_over_sold.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/tdx/pressure_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/tdx/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/tdx/statistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/tdx/trend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/tdx/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:14:53.980288 polars_ta-0.2.7/polars_ta/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/utils/numba_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/utils/pandas_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/utils/pit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/utils/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:14:53.980288 polars_ta-0.2.7/polars_ta/wq/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/wq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/wq/_nb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/wq/_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/wq/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/wq/cross_sectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/wq/logical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/wq/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/wq/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/wq/transformational.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-24 13:14:46.000000 polars_ta-0.2.7/polars_ta/wq/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:14:53.980288 polars_ta-0.2.7/polars_ta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-05-24 13:14:53.000000 polars_ta-0.2.7/polars_ta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-24 13:14:53.000000 polars_ta-0.2.7/polars_ta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:14:53.000000 polars_ta-0.2.7/polars_ta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 13:14:53.000000 polars_ta-0.2.7/polars_ta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 13:14:53.000000 polars_ta-0.2.7/polars_ta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-24 13:14:46.000000 polars_ta-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 13:14:53.980288 polars_ta-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 13:14:46.000000 polars_ta-0.2.7/setup.py
```

### Comparing `polars_ta-0.2.6/LICENSE` & `polars_ta-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/PKG-INFO` & `polars_ta-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars_ta
-Version: 0.2.6
+Version: 0.2.7
 Summary: polars expressions
 Author-email: wukan <wu-kan@163.com>
 License: MIT License
         
         Copyright (c) 2023 wukan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polars_ta-0.2.6/README.md` & `polars_ta-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/candles/cdl1.py` & `polars_ta-0.2.7/polars_ta/candles/cdl1.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/candles/cdl1_limit.py` & `polars_ta-0.2.7/polars_ta/candles/cdl1_limit.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/candles/cdl2.py` & `polars_ta-0.2.7/polars_ta/candles/cdl2.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/noise.py` & `polars_ta-0.2.7/polars_ta/noise.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/performance/returns.py` & `polars_ta-0.2.7/polars_ta/performance/returns.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/prefix/ta.py` & `polars_ta-0.2.7/polars_ta/prefix/ta.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/prefix/talib.py` & `polars_ta-0.2.7/polars_ta/prefix/talib.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/prefix/tdx.py` & `polars_ta-0.2.7/polars_ta/prefix/tdx.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/reports/cicc.py` & `polars_ta-0.2.7/polars_ta/reports/cicc.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/ta/momentum.py` & `polars_ta-0.2.7/polars_ta/ta/momentum.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/ta/operators.py` & `polars_ta-0.2.7/polars_ta/ta/operators.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/ta/overlap.py` & `polars_ta-0.2.7/polars_ta/ta/overlap.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/ta/statistic.py` & `polars_ta-0.2.7/polars_ta/ta/statistic.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/ta/transform.py` & `polars_ta-0.2.7/polars_ta/ta/transform.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/ta/volatility.py` & `polars_ta-0.2.7/polars_ta/ta/volatility.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/ta/volume.py` & `polars_ta-0.2.7/polars_ta/ta/volume.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/talib/__init__.py` & `polars_ta-0.2.7/polars_ta/talib/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/tdx/__init__.py` & `polars_ta-0.2.7/polars_ta/tdx/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/tdx/_nb.py` & `polars_ta-0.2.7/polars_ta/tdx/_nb.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/tdx/arithmetic.py` & `polars_ta-0.2.7/polars_ta/tdx/arithmetic.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/tdx/choice.py` & `polars_ta-0.2.7/polars_ta/tdx/choice.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/tdx/energy.py` & `polars_ta-0.2.7/polars_ta/tdx/energy.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/tdx/logical.py` & `polars_ta-0.2.7/polars_ta/tdx/logical.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/tdx/over_bought_over_sold.py` & `polars_ta-0.2.7/polars_ta/tdx/over_bought_over_sold.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/tdx/pressure_support.py` & `polars_ta-0.2.7/polars_ta/tdx/pressure_support.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/tdx/reference.py` & `polars_ta-0.2.7/polars_ta/tdx/reference.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/tdx/statistic.py` & `polars_ta-0.2.7/polars_ta/tdx/statistic.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/tdx/trend.py` & `polars_ta-0.2.7/polars_ta/tdx/trend.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/tdx/volume.py` & `polars_ta-0.2.7/polars_ta/tdx/volume.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/utils/helper.py` & `polars_ta-0.2.7/polars_ta/utils/helper.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/utils/numba_.py` & `polars_ta-0.2.7/polars_ta/utils/numba_.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/utils/pandas_.py` & `polars_ta-0.2.7/polars_ta/utils/pandas_.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/utils/pit.py` & `polars_ta-0.2.7/polars_ta/utils/pit.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/utils/wrapper.py` & `polars_ta-0.2.7/polars_ta/utils/wrapper.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/wq/_nb.py` & `polars_ta-0.2.7/polars_ta/wq/_nb.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/wq/_slow.py` & `polars_ta-0.2.7/polars_ta/wq/_slow.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/wq/arithmetic.py` & `polars_ta-0.2.7/polars_ta/wq/arithmetic.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/wq/cross_sectional.py` & `polars_ta-0.2.7/polars_ta/wq/cross_sectional.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/wq/logical.py` & `polars_ta-0.2.7/polars_ta/wq/logical.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from polars import when
 
 
 # TODO 本文件返回bool时是否有必要转换成 0/1 ?
 
 def and_(a: Expr, b: Expr, *args) -> Expr:
     """Logical AND operator, returns true if both operands are true and returns false otherwise"""
-    _args = [a, b] + list(args)
-    return all_horizontal(*args)
+    return all_horizontal(a, b, *args)
 
 
 def equal(input1: Expr, input2: Expr) -> Expr:
     """Returns true if both inputs are same and returns false otherwise"""
     return input1 == input2
 
 
@@ -48,9 +47,8 @@
 def negate(input1: Expr) -> Expr:
     """The result is true if the converted operand is false; the result is false if the converted operand is true"""
     return ~input1
 
 
 def or_(a: Expr, b: Expr, *args) -> Expr:
     """Logical OR operator returns true if either or both inputs are true and returns false otherwise"""
-    _args = [a, b] + list(args)
-    return any_horizontal(*args)
+    return any_horizontal(a, b, *args)
```

### Comparing `polars_ta-0.2.6/polars_ta/wq/preprocess.py` & `polars_ta-0.2.7/polars_ta/wq/preprocess.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/wq/time_series.py` & `polars_ta-0.2.7/polars_ta/wq/time_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,19 @@
 
 
 def ts_kurtosis(x: Expr, d: int = 5) -> Expr:
     # TODO 等待polars官方出rolling_kurt
     return x.map_batches(lambda a: roll_kurt(a, d))
 
 
+def ts_l2_norm(x: Expr, d: int = 5) -> Expr:
+    """Euclidean norm"""
+    return x.pow(2).rolling_sum(d).sqrt()
+
+
 def ts_log_diff(x: Expr, d: int = 1) -> Expr:
     """Returns log(current value of input or x[t] ) - log(previous value of input or x[t-1])."""
     return x.log().diff(d)
 
 
 def ts_max(x: Expr, d: int = 30) -> Expr:
     return x.rolling_max(d)
```

### Comparing `polars_ta-0.2.6/polars_ta/wq/transformational.py` & `polars_ta-0.2.7/polars_ta/wq/transformational.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/polars_ta/wq/vector.py` & `polars_ta-0.2.7/polars_ta/wq/vector.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 
 
 def vec_kurtosis(x: Expr) -> Expr:
     """Kurtosis of vector field x"""
     return x.kurtosis()
 
 
+def vec_l2_norm(x: Expr) -> Expr:
+    """Euclidean norm"""
+    return x.pow(2).sum().sqrt()
+
+
 def vec_max(x: Expr) -> Expr:
     """Maximum value form vector field x"""
     return x.max()
 
 
 def vec_min(x: Expr) -> Expr:
     """Minimum value form vector field x"""
```

### Comparing `polars_ta-0.2.6/polars_ta.egg-info/PKG-INFO` & `polars_ta-0.2.7/polars_ta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars_ta
-Version: 0.2.6
+Version: 0.2.7
 Summary: polars expressions
 Author-email: wukan <wu-kan@163.com>
 License: MIT License
         
         Copyright (c) 2023 wukan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polars_ta-0.2.6/polars_ta.egg-info/SOURCES.txt` & `polars_ta-0.2.7/polars_ta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.6/pyproject.toml` & `polars_ta-0.2.7/pyproject.toml`

 * *Files identical despite different names*

