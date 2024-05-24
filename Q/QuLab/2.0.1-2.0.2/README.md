# Comparing `tmp/QuLab-2.0.1.tar.gz` & `tmp/qulab-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuLab-2.0.1.tar", last modified: Tue Mar 12 07:04:04 2024, max compression
+gzip compressed data, was "qulab-2.0.2.tar", last modified: Fri May 24 02:30:50 2024, max compression
```

## Comparing `QuLab-2.0.1.tar` & `qulab-2.0.2.tar`

### file list

```diff
@@ -1,106 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:04:04.399675 QuLab-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-12 07:03:24.000000 QuLab-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-12 07:03:24.000000 QuLab-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-03-12 07:04:04.399675 QuLab-2.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:04:04.399675 QuLab-2.0.1/QuLab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-03-12 07:04:04.000000 QuLab-2.0.1/QuLab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-03-12 07:04:04.000000 QuLab-2.0.1/QuLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 07:04:04.000000 QuLab-2.0.1/QuLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-12 07:04:04.000000 QuLab-2.0.1/QuLab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-12 07:04:04.000000 QuLab-2.0.1/QuLab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-12 07:04:04.000000 QuLab-2.0.1/QuLab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-12 07:03:24.000000 QuLab-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-12 07:03:24.000000 QuLab-2.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:04:04.383675 QuLab-2.0.1/qulab/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:04:04.387675 QuLab-2.0.1/qulab/monitor/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/monitor/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      744 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/monitor/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2455 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/monitor/dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1823 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/monitor/event_queue.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7799 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/monitor/mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/monitor/monitor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3601 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/monitor/ploter.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/monitor/qt_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7948 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/monitor/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:04:04.387675 QuLab-2.0.1/qulab/scan/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17143 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/scan/base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/scan/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    14781 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/scan/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/scan/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     7802 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/scan/scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/scan/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/scan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:04:04.391675 QuLab-2.0.1/qulab/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:04:04.391675 QuLab-2.0.1/qulab/storage/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/backend/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8343 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:04:04.391675 QuLab-2.0.1/qulab/storage/models/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/models/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/models/ipy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/models/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/models/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/storage/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:04:04.391675 QuLab-2.0.1/qulab/sys/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22449 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:04:04.391675 QuLab-2.0.1/qulab/sys/device/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/device/basedevice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/device/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/device/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:04:04.391675 QuLab-2.0.1/qulab/sys/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/drivers/FakeInstrument.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/ipy_events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:04:04.395675 QuLab-2.0.1/qulab/sys/net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/net/bencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/net/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    23509 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/net/dhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/net/dhcpd.py
--rw-r--r--   0 runner    (1001) docker     (127)    38981 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/net/kad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/net/kcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/net/nginx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:04:04.395675 QuLab-2.0.1/qulab/sys/rpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/rpc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/rpc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    35327 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/rpc/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/rpc/msgpack.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/rpc/rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/rpc/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/rpc/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/rpc/socket.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/rpc/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/sys/rpc/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:04:04.395675 QuLab-2.0.1/qulab/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/visualization/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13777 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/visualization/_autoplot.py
--rw-r--r--   0 runner    (1001) docker     (127)    13533 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/visualization/plot_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/visualization/plot_seq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/visualization/qdat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-03-12 07:03:24.000000 QuLab-2.0.1/qulab/visualization/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 07:04:04.399675 QuLab-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-12 07:03:24.000000 QuLab-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:04:04.395675 QuLab-2.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-12 07:03:24.000000 QuLab-2.0.1/src/qulab.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:04:04.395675 QuLab-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-03-12 07:03:24.000000 QuLab-2.0.1/tests/test_scan_iter.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.797087 qulab-2.0.2/
+-rw-r--r--   0 runner     (501) staff       (20)     1065 2024-05-24 02:30:21.000000 qulab-2.0.2/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-24 02:30:21.000000 qulab-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     3464 2024-05-24 02:30:50.796704 qulab-2.0.2/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.796382 qulab-2.0.2/QuLab.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3464 2024-05-24 02:30:50.000000 qulab-2.0.2/QuLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2256 2024-05-24 02:30:50.000000 qulab-2.0.2/QuLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-24 02:30:50.000000 qulab-2.0.2/QuLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-24 02:30:50.000000 qulab-2.0.2/QuLab.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)      188 2024-05-24 02:30:50.000000 qulab-2.0.2/QuLab.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2024-05-24 02:30:50.000000 qulab-2.0.2/QuLab.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1953 2024-05-24 02:30:21.000000 qulab-2.0.2/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     1772 2024-05-24 02:30:21.000000 qulab-2.0.2/pyproject.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.784091 qulab-2.0.2/qulab/
+-rw-r--r--   0 runner     (501) staff       (20)       32 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      430 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.785620 qulab-2.0.2/qulab/monitor/
+-rw-r--r--   0 runner     (501) staff       (20)       42 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       97 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/__main__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      744 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/config.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2455 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/dataset.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1823 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/event_queue.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7799 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/mainwindow.py
+-rw-r--r--   0 runner     (501) staff       (20)     2305 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/monitor.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3601 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/ploter.py
+-rw-r--r--   0 runner     (501) staff       (20)      788 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/qt_compat.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7948 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/toolbar.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.787476 qulab-2.0.2/qulab/scan/
+-rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4518 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/curd.py
+-rw-r--r--   0 runner     (501) staff       (20)    15694 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/expression.py
+-rw-r--r--   0 runner     (501) staff       (20)    17117 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/models.py
+-rw-r--r--   0 runner     (501) staff       (20)     2287 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/optimize.py
+-rw-r--r--   0 runner     (501) staff       (20)    11521 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/query_record.py
+-rw-r--r--   0 runner     (501) staff       (20)    15402 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/recorder.py
+-rw-r--r--   0 runner     (501) staff       (20)    23030 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/scan.py
+-rw-r--r--   0 runner     (501) staff       (20)     1024 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.788409 qulab-2.0.2/qulab/storage/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1692 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.788628 qulab-2.0.2/qulab/storage/backend/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/backend/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5202 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/backend/redis.py
+-rw-r--r--   0 runner     (501) staff       (20)    11865 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/base_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     1701 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/chunk.py
+-rw-r--r--   0 runner     (501) staff       (20)     4655 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     8343 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/file.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.789978 qulab-2.0.2/qulab/storage/models/
+-rw-r--r--   0 runner     (501) staff       (20)      586 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/base.py
+-rw-r--r--   0 runner     (501) staff       (20)      689 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/config.py
+-rw-r--r--   0 runner     (501) staff       (20)     2716 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/file.py
+-rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/ipy.py
+-rw-r--r--   0 runner     (501) staff       (20)     2879 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/models.py
+-rw-r--r--   0 runner     (501) staff       (20)     4970 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/record.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/report.py
+-rw-r--r--   0 runner     (501) staff       (20)     2339 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/tag.py
+-rw-r--r--   0 runner     (501) staff       (20)     2561 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/storage.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.790658 qulab-2.0.2/qulab/sys/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    22449 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/chat.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.791253 qulab-2.0.2/qulab/sys/device/
+-rw-r--r--   0 runner     (501) staff       (20)      149 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/device/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6423 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/device/basedevice.py
+-rw-r--r--   0 runner     (501) staff       (20)     2501 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/device/loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     1564 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/device/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.791573 qulab-2.0.2/qulab/sys/drivers/
+-rw-r--r--   0 runner     (501) staff       (20)     1867 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/drivers/FakeInstrument.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/drivers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2889 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/ipy_events.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.792922 qulab-2.0.2/qulab/sys/net/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/net/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4959 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/net/bencoder.py
+-rw-r--r--   0 runner     (501) staff       (20)     5690 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/net/cli.py
+-rw-r--r--   0 runner     (501) staff       (20)    23509 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/net/dhcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     5322 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/net/dhcpd.py
+-rw-r--r--   0 runner     (501) staff       (20)    38981 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/net/kad.py
+-rw-r--r--   0 runner     (501) staff       (20)     5761 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/net/kcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     4964 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/net/nginx.py
+-rw-r--r--   0 runner     (501) staff       (20)     5350 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/progress.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.794783 qulab-2.0.2/qulab/sys/rpc/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2567 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/exceptions.py
+-rw-r--r--   0 runner     (501) staff       (20)    35327 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/msgpack.py
+-rw-r--r--   0 runner     (501) staff       (20)     1274 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/msgpack.pyi
+-rw-r--r--   0 runner     (501) staff       (20)    11979 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/rpc.py
+-rw-r--r--   0 runner     (501) staff       (20)     3355 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/serialize.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/socket.py
+-rw-r--r--   0 runner     (501) staff       (20)      594 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     7926 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/zmq_socket.py
+-rw-r--r--   0 runner     (501) staff       (20)       21 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.795771 qulab-2.0.2/qulab/visualization/
+-rw-r--r--   0 runner     (501) staff       (20)     6129 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/visualization/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1639 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/visualization/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)    14099 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/visualization/_autoplot.py
+-rw-r--r--   0 runner     (501) staff       (20)    13533 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/visualization/plot_layout.py
+-rw-r--r--   0 runner     (501) staff       (20)     2693 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/visualization/plot_seq.py
+-rw-r--r--   0 runner     (501) staff       (20)     5735 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/visualization/qdat.py
+-rw-r--r--   0 runner     (501) staff       (20)     3180 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/visualization/widgets.py
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-24 02:30:50.797126 qulab-2.0.2/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      833 2024-05-24 02:30:21.000000 qulab-2.0.2/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.796000 qulab-2.0.2/src/
+-rw-r--r--   0 runner     (501) staff       (20)       63 2024-05-24 02:30:21.000000 qulab-2.0.2/src/qulab.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.796189 qulab-2.0.2/tests/
+-rw-r--r--   0 runner     (501) staff       (20)       30 2024-05-24 02:30:21.000000 qulab-2.0.2/tests/test_scan.py
```

### Comparing `QuLab-2.0.1/LICENSE` & `qulab-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/PKG-INFO` & `qulab-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuLab
-Version: 2.0.1
+Version: 2.0.2
 Summary: contral instruments and manage data
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/feihoo87/QuLab
 Project-URL: Bug Reports, https://github.com/feihoo87/QuLab/issues
 Project-URL: Source, https://github.com/feihoo87/QuLab/
@@ -26,18 +26,21 @@
 License-File: LICENSE
 Requires-Dist: blinker>=1.4
 Requires-Dist: click>=7.1.2
 Requires-Dist: dill>=0.3.6
 Requires-Dist: GitPython>=3.1.14
 Requires-Dist: ipython>=7.4.0
 Requires-Dist: ipywidgets>=7.4.2
+Requires-Dist: loguru>=0.7.2
 Requires-Dist: matplotlib>=3.7.2
 Requires-Dist: numpy>=1.13.3
 Requires-Dist: ply>=3.11
+Requires-Dist: pyzmq>=25.1.0
 Requires-Dist: scipy>=1.0.0
+Requires-Dist: watchdog>=4.0.0
 
 # QuLab
 [![View build status](https://travis-ci.org/feihoo87/QuLab.svg?branch=master)](https://travis-ci.org/feihoo87/QuLab)
 [![Coverage Status](https://coveralls.io/repos/github/feihoo87/QuLab/badge.svg)](https://coveralls.io/github/feihoo87/QuLab)
 [![Updates](https://pyup.io/repos/github/feihoo87/QuLab/shield.svg)](https://pyup.io/repos/github/feihoo87/QuLab/)
 [![Docs Status](https://readthedocs.org/projects/qulab/badge/?version=latest)](http://qulab.readthedocs.org)
 [![PyPI version](https://badge.fury.io/py/QuLab.svg)](https://badge.fury.io/py/QuLab)
```

### Comparing `QuLab-2.0.1/QuLab.egg-info/PKG-INFO` & `qulab-2.0.2/QuLab.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuLab
-Version: 2.0.1
+Version: 2.0.2
 Summary: contral instruments and manage data
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/feihoo87/QuLab
 Project-URL: Bug Reports, https://github.com/feihoo87/QuLab/issues
 Project-URL: Source, https://github.com/feihoo87/QuLab/
@@ -26,18 +26,21 @@
 License-File: LICENSE
 Requires-Dist: blinker>=1.4
 Requires-Dist: click>=7.1.2
 Requires-Dist: dill>=0.3.6
 Requires-Dist: GitPython>=3.1.14
 Requires-Dist: ipython>=7.4.0
 Requires-Dist: ipywidgets>=7.4.2
+Requires-Dist: loguru>=0.7.2
 Requires-Dist: matplotlib>=3.7.2
 Requires-Dist: numpy>=1.13.3
 Requires-Dist: ply>=3.11
+Requires-Dist: pyzmq>=25.1.0
 Requires-Dist: scipy>=1.0.0
+Requires-Dist: watchdog>=4.0.0
 
 # QuLab
 [![View build status](https://travis-ci.org/feihoo87/QuLab.svg?branch=master)](https://travis-ci.org/feihoo87/QuLab)
 [![Coverage Status](https://coveralls.io/repos/github/feihoo87/QuLab/badge.svg)](https://coveralls.io/github/feihoo87/QuLab)
 [![Updates](https://pyup.io/repos/github/feihoo87/QuLab/shield.svg)](https://pyup.io/repos/github/feihoo87/QuLab/)
 [![Docs Status](https://readthedocs.org/projects/qulab/badge/?version=latest)](http://qulab.readthedocs.org)
 [![PyPI version](https://badge.fury.io/py/QuLab.svg)](https://badge.fury.io/py/QuLab)
```

### Comparing `QuLab-2.0.1/QuLab.egg-info/SOURCES.txt` & `qulab-2.0.2/QuLab.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -19,20 +19,21 @@
 qulab/monitor/event_queue.py
 qulab/monitor/mainwindow.py
 qulab/monitor/monitor.py
 qulab/monitor/ploter.py
 qulab/monitor/qt_compat.py
 qulab/monitor/toolbar.py
 qulab/scan/__init__.py
-qulab/scan/base.py
-qulab/scan/dataset.py
+qulab/scan/curd.py
 qulab/scan/expression.py
+qulab/scan/models.py
 qulab/scan/optimize.py
-qulab/scan/scanner.py
-qulab/scan/transforms.py
+qulab/scan/query_record.py
+qulab/scan/recorder.py
+qulab/scan/scan.py
 qulab/scan/utils.py
 qulab/storage/__init__.py
 qulab/storage/__main__.py
 qulab/storage/base_dataset.py
 qulab/storage/chunk.py
 qulab/storage/dataset.py
 qulab/storage/file.py
@@ -73,16 +74,17 @@
 qulab/sys/rpc/msgpack.pyi
 qulab/sys/rpc/rpc.py
 qulab/sys/rpc/serialize.py
 qulab/sys/rpc/server.py
 qulab/sys/rpc/socket.py
 qulab/sys/rpc/utils.py
 qulab/sys/rpc/worker.py
+qulab/sys/rpc/zmq_socket.py
 qulab/visualization/__init__.py
 qulab/visualization/__main__.py
 qulab/visualization/_autoplot.py
 qulab/visualization/plot_layout.py
 qulab/visualization/plot_seq.py
 qulab/visualization/qdat.py
 qulab/visualization/widgets.py
 src/qulab.h
-tests/test_scan_iter.py
+tests/test_scan.py
```

### Comparing `QuLab-2.0.1/README.md` & `qulab-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/pyproject.toml` & `qulab-2.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -30,18 +30,21 @@
 dependencies = [
     "blinker>=1.4",
     "click>=7.1.2",
     "dill>=0.3.6",
     "GitPython>=3.1.14",
     "ipython>=7.4.0",
     "ipywidgets>=7.4.2",
+    "loguru>=0.7.2",
     "matplotlib>=3.7.2",
     "numpy>=1.13.3",
     "ply>=3.11",
-    "scipy>=1.0.0"
+    "pyzmq>=25.1.0",
+    "scipy>=1.0.0",
+    "watchdog>=4.0.0"
 ]
 dynamic = ["version"]
 
 [project.scripts]
 "qulab" = "qulab.__main__:main"
 
 [project.urls]
```

### Comparing `QuLab-2.0.1/qulab/monitor/config.py` & `qulab-2.0.2/qulab/monitor/config.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/monitor/dataset.py` & `qulab-2.0.2/qulab/monitor/dataset.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/monitor/event_queue.py` & `qulab-2.0.2/qulab/monitor/event_queue.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/monitor/mainwindow.py` & `qulab-2.0.2/qulab/monitor/mainwindow.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/monitor/monitor.py` & `qulab-2.0.2/qulab/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/monitor/ploter.py` & `qulab-2.0.2/qulab/monitor/ploter.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/monitor/qt_compat.py` & `qulab-2.0.2/qulab/monitor/qt_compat.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/monitor/toolbar.py` & `qulab-2.0.2/qulab/monitor/toolbar.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/scan/expression.py` & `qulab-2.0.2/qulab/scan/expression.py`

 * *Files 6% similar despite different names*

```diff
@@ -319,14 +319,22 @@
 class UnaryExpression(Expression):
 
     def __init__(self, a, op):
         super().__init__()
         self.a = a
         self.op = op
 
+    def __getstate__(self) -> dict:
+        return {'a': self.a, 'op': self.op}
+
+    def __setstate__(self, state: dict):
+        self.a = state['a']
+        self.op = state['op']
+        self.cache = _empty
+
     def symbols(self) -> list[str]:
         if isinstance(self.a, Expression):
             return self.a.symbols()
         else:
             return []
 
     def changed(self, env) -> bool:
@@ -358,14 +366,23 @@
 
     def __init__(self, a, b, op):
         super().__init__()
         self.a = a
         self.b = b
         self.op = op
 
+    def __getstate__(self) -> dict:
+        return {'a': self.a, 'b': self.b, 'op': self.op}
+
+    def __setstate__(self, state: dict):
+        self.a = state['a']
+        self.b = state['b']
+        self.op = state['op']
+        self.cache = _empty
+
     def symbols(self) -> list[str]:
         symbs = set()
         if isinstance(self.a, Expression):
             symbs.update(self.a.symbols())
         if isinstance(self.b, Expression):
             symbs.update(self.b.symbols())
         return list(symbs)
@@ -415,14 +432,23 @@
 
     def __init__(self, obj, method: str, *args):
         super().__init__()
         self.obj = obj
         self.method = method
         self.args = args
 
+    def __getstate__(self) -> dict:
+        return {'obj': self.obj, 'method': self.method, 'args': self.args}
+
+    def __setstate__(self, state: dict):
+        self.obj = state['obj']
+        self.method = state['method']
+        self.args = state['args']
+        self.cache = _empty
+
     def symbols(self) -> list[str]:
         symbs = set()
         if isinstance(self.obj, Expression):
             symbs.update(self.obj.symbols())
         for a in self.args:
             if isinstance(a, Expression):
                 symbs.update(a.symbols())
@@ -435,28 +461,35 @@
             a.value(env) if isinstance(a, Expression) else a for a in self.args
         ]
         if isinstance(obj, Expression) or any(
                 isinstance(x, Expression) for x in args):
             return ObjectMethod(obj, self.method, *args)
         else:
             return getattr(obj, self.method)(*args)
-        
+
     def __repr__(self):
         if self.method == '__call__':
             return f"{self.obj!r}({', '.join(map(repr, self.args))})"
         else:
             return f"{self.obj!r}.{self.method}({', '.join(map(repr, self.args))})"
 
 
 class Symbol(Expression):
 
     def __init__(self, name):
         super().__init__()
         self.name = name
 
+    def __getstate__(self) -> dict:
+        return {'name': self.name}
+
+    def __setstate__(self, state: dict):
+        self.name = state['name']
+        self.cache = _empty
+
     def symbols(self) -> list[str]:
         return [self.name]
 
     def eval(self, env):
         if self.name in env:
             return env[self.name]
         else:
```

### Comparing `QuLab-2.0.1/qulab/scan/utils.py` & `qulab-2.0.2/qulab/scan/utils.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/storage/__main__.py` & `qulab-2.0.2/qulab/storage/__main__.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/storage/backend/redis.py` & `qulab-2.0.2/qulab/storage/backend/redis.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/storage/base_dataset.py` & `qulab-2.0.2/qulab/storage/base_dataset.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/storage/chunk.py` & `qulab-2.0.2/qulab/storage/chunk.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/storage/dataset.py` & `qulab-2.0.2/qulab/storage/dataset.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/storage/file.py` & `qulab-2.0.2/qulab/storage/file.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/storage/models/__init__.py` & `qulab-2.0.2/qulab/storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/storage/models/config.py` & `qulab-2.0.2/qulab/storage/models/config.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/storage/models/file.py` & `qulab-2.0.2/qulab/storage/models/file.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/storage/models/ipy.py` & `qulab-2.0.2/qulab/storage/models/ipy.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/storage/models/models.py` & `qulab-2.0.2/qulab/storage/models/models.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/storage/models/record.py` & `qulab-2.0.2/qulab/storage/models/record.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/storage/models/report.py` & `qulab-2.0.2/qulab/storage/models/report.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/storage/models/tag.py` & `qulab-2.0.2/qulab/storage/models/tag.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/storage/storage.py` & `qulab-2.0.2/qulab/storage/storage.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/chat.py` & `qulab-2.0.2/qulab/sys/chat.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/device/basedevice.py` & `qulab-2.0.2/qulab/sys/device/basedevice.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/device/loader.py` & `qulab-2.0.2/qulab/sys/device/loader.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/device/utils.py` & `qulab-2.0.2/qulab/sys/device/utils.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/drivers/FakeInstrument.py` & `qulab-2.0.2/qulab/sys/drivers/FakeInstrument.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/ipy_events.py` & `qulab-2.0.2/qulab/sys/ipy_events.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/net/bencoder.py` & `qulab-2.0.2/qulab/sys/net/bencoder.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/net/cli.py` & `qulab-2.0.2/qulab/sys/net/cli.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/net/dhcp.py` & `qulab-2.0.2/qulab/sys/net/dhcp.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/net/dhcpd.py` & `qulab-2.0.2/qulab/sys/net/dhcpd.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/net/kad.py` & `qulab-2.0.2/qulab/sys/net/kad.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/net/kcp.py` & `qulab-2.0.2/qulab/sys/net/kcp.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/net/nginx.py` & `qulab-2.0.2/qulab/sys/net/nginx.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/progress.py` & `qulab-2.0.2/qulab/sys/progress.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/rpc/exceptions.py` & `qulab-2.0.2/qulab/sys/rpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/rpc/msgpack.py` & `qulab-2.0.2/qulab/sys/rpc/msgpack.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/rpc/msgpack.pyi` & `qulab-2.0.2/qulab/sys/rpc/msgpack.pyi`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/rpc/rpc.py` & `qulab-2.0.2/qulab/sys/rpc/rpc.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/rpc/serialize.py` & `qulab-2.0.2/qulab/sys/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/rpc/server.py` & `qulab-2.0.2/qulab/sys/rpc/server.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/rpc/socket.py` & `qulab-2.0.2/qulab/sys/rpc/socket.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/sys/rpc/utils.py` & `qulab-2.0.2/qulab/sys/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/visualization/__init__.py` & `qulab-2.0.2/qulab/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/visualization/__main__.py` & `qulab-2.0.2/qulab/visualization/__main__.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/visualization/_autoplot.py` & `qulab-2.0.2/qulab/visualization/_autoplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 
 import matplotlib.pyplot as plt
 import numpy as np
-from matplotlib.colors import LogNorm
+from matplotlib.colors import LogNorm, Normalize, SymLogNorm
 from matplotlib.ticker import EngFormatter, LogFormatterSciNotation
 from scipy.interpolate import griddata
 
 
 def good_for_logscale(x, threshold=4):
     if np.any(x <= 0):
         return False
@@ -235,18 +235,24 @@
              zscale='linear',
              resolution=None,
              **kwds):
     kwds.setdefault('origin', 'lower')
     kwds.setdefault('aspect', 'auto')
     kwds.setdefault('interpolation', 'nearest')
 
+    vmin = kwds.get('vmin', np.nanmin(z))
+    vmax = kwds.get('vmax', np.nanmax(z))
     if zscale == 'log':
-        vmim = kwds.get('vmin', np.min(z))
-        vmax = kwds.get('vmax', np.max(z))
-        kwds.setdefault('norm', LogNorm(vmax=vmax, vmin=vmim))
+        kwds.setdefault('norm', LogNorm(vmax=vmax, vmin=vmin))
+    elif zscale == 'symlog':
+        kwds.setdefault('norm', SymLogNorm(vmax=vmax,
+                                           vmin=vmin,
+                                           linthresh=1e-5))
+    else:
+        kwds.setdefault('norm', Normalize(vmin=vmin, vmax=vmax))
     zlabel = f"{zlabel} [{z_unit}]" if z_unit else zlabel
 
     band_area = False
     if x.ndim == 1 and y.ndim == 2 and y.shape[1] == x.shape[0]:
         x = np.asarray([x] * y.shape[0])
         band_area = True
     elif x.ndim == 2 and y.ndim == 1 and x.shape[0] == y.shape[0]:
@@ -299,15 +305,15 @@
         img = imshow_logy(x, y, z, y_unit, ax, **kwds)
     elif (xscale, yscale) == ('log', 'log'):
         img = imshow_loglog(x, y, z, x_unit, y_unit, ax, **kwds)
     else:
         pass
     ax.set_xlabel(xlabel)
     ax.set_ylabel(ylabel)
-    cb = fig.colorbar(img, ax=ax)
+    cb = fig.colorbar(img, ax=ax, norm=kwds.get('norm', None))
     cb.set_label(zlabel)
 
 
 def plot_scatter(x,
                  y,
                  z,
                  xlabel,
```

### Comparing `QuLab-2.0.1/qulab/visualization/plot_layout.py` & `qulab-2.0.2/qulab/visualization/plot_layout.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/visualization/plot_seq.py` & `qulab-2.0.2/qulab/visualization/plot_seq.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/visualization/qdat.py` & `qulab-2.0.2/qulab/visualization/qdat.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/qulab/visualization/widgets.py` & `qulab-2.0.2/qulab/visualization/widgets.py`

 * *Files identical despite different names*

### Comparing `QuLab-2.0.1/setup.py` & `qulab-2.0.2/setup.py`

 * *Files identical despite different names*

