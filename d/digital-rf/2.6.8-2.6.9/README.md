# Comparing `tmp/digital_rf-2.6.8.tar.gz` & `tmp/digital_rf-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital_rf-2.6.8.tar", last modified: Wed Dec  7 18:20:32 2022, max compression
+gzip compressed data, was "digital_rf-2.6.9.tar", last modified: Thu May 23 20:30:40 2024, max compression
```

## Comparing `digital_rf-2.6.8.tar` & `digital_rf-2.6.9.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.960725 digital_rf-2.6.8/
--rw-rw-r--   0 root         (0) root         (0)      625 2022-12-07 18:20:26.000000 digital_rf-2.6.8/AUTHORS
--rw-rw-r--   0 root         (0) root         (0)    14893 2022-12-07 18:20:26.000000 digital_rf-2.6.8/CHANGELOG.rst
--rw-rw-r--   0 root         (0) root         (0)     1602 2022-12-07 18:20:26.000000 digital_rf-2.6.8/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      684 2022-12-07 18:20:27.000000 digital_rf-2.6.8/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)      759 2022-12-07 18:20:27.000000 digital_rf-2.6.8/MANIFEST.md
--rw-r--r--   0 root         (0) root         (0)     3627 2022-12-07 18:20:32.960725 digital_rf-2.6.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2058 2022-12-07 18:20:27.000000 digital_rf-2.6.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.916725 digital_rf-2.6.8/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.916725 digital_rf-2.6.8/data/example/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.924724 digital_rf-2.6.8/data/example/ch0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.924724 digital_rf-2.6.8/data/example/ch0/2019-08-29T19-00-00/
--rw-rw-r--   0 root         (0) root         (0)    47608 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/example/ch0/2019-08-29T19-00-00/rf@1567105700.000.h5
--rw-rw-r--   0 root         (0) root         (0)     2232 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/example/ch0/drf_properties.h5
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.924724 digital_rf-2.6.8/data/example/ch0/metadata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.924724 digital_rf-2.6.8/data/example/ch0/metadata/2019-08-29T19-00-00/
--rw-rw-r--   0 root         (0) root         (0)    22944 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/example/ch0/metadata/2019-08-29T19-00-00/metadata@1567105700.h5
--rw-rw-r--   0 root         (0) root         (0)     4192 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/example/ch0/metadata/dmd_properties.h5
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.920724 digital_rf-2.6.8/data/synthetic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.924724 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.924724 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/
--rw-rw-r--   0 root         (0) root         (0)    11912 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368230.000.h5
--rw-rw-r--   0 root         (0) root         (0)    11912 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368231.000.h5
--rw-rw-r--   0 root         (0) root         (0)    11848 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368232.000.h5
--rw-rw-r--   0 root         (0) root         (0)    11912 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368233.000.h5
--rw-rw-r--   0 root         (0) root         (0)    11912 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368234.000.h5
--rw-rw-r--   0 root         (0) root         (0)    11912 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368236.000.h5
--rw-rw-r--   0 root         (0) root         (0)    11912 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368237.000.h5
--rw-rw-r--   0 root         (0) root         (0)    11848 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368238.000.h5
--rw-rw-r--   0 root         (0) root         (0)    11912 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368239.000.h5
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.928725 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/
--rw-rw-r--   0 root         (0) root         (0)    11912 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368240.000.h5
--rw-rw-r--   0 root         (0) root         (0)    11848 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368241.000.h5
--rw-rw-r--   0 root         (0) root         (0)    11912 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368242.000.h5
--rw-rw-r--   0 root         (0) root         (0)    11912 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368243.000.h5
--rw-rw-r--   0 root         (0) root         (0)    11848 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368244.000.h5
--rw-rw-r--   0 root         (0) root         (0)     2232 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/drf_properties.h5
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.928725 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.928725 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/
--rw-rw-r--   0 root         (0) root         (0)    10744 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368230.000.h5
--rw-rw-r--   0 root         (0) root         (0)    10744 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368231.000.h5
--rw-rw-r--   0 root         (0) root         (0)    10480 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368232.000.h5
--rw-rw-r--   0 root         (0) root         (0)    10480 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368233.000.h5
--rw-rw-r--   0 root         (0) root         (0)    10480 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368234.000.h5
--rw-rw-r--   0 root         (0) root         (0)    10480 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368236.000.h5
--rw-rw-r--   0 root         (0) root         (0)    10744 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368237.000.h5
--rw-rw-r--   0 root         (0) root         (0)    10480 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368238.000.h5
--rw-rw-r--   0 root         (0) root         (0)    10744 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368239.000.h5
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.928725 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/
--rw-rw-r--   0 root         (0) root         (0)    10744 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368240.000.h5
--rw-rw-r--   0 root         (0) root         (0)    10480 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368241.000.h5
--rw-rw-r--   0 root         (0) root         (0)    10744 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368242.000.h5
--rw-rw-r--   0 root         (0) root         (0)    10744 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368243.000.h5
--rw-rw-r--   0 root         (0) root         (0)    10480 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368244.000.h5
--rw-rw-r--   0 root         (0) root         (0)     2232 2022-12-07 18:20:26.000000 digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/drf_properties.h5
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.964725 digital_rf-2.6.8/digital_rf/
--rw-rw-r--   0 root         (0) root         (0)     1143 2022-12-07 18:20:27.000000 digital_rf-2.6.8/digital_rf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-12-07 18:20:32.964725 digital_rf-2.6.8/digital_rf/_version.py
--rw-rw-r--   0 root         (0) root         (0)    47645 2022-12-07 18:20:27.000000 digital_rf-2.6.8/digital_rf/digital_metadata.py
--rw-rw-r--   0 root         (0) root         (0)    99813 2022-12-07 18:20:27.000000 digital_rf-2.6.8/digital_rf/digital_rf_deprecated_hdf5.py
--rw-rw-r--   0 root         (0) root         (0)    82937 2022-12-07 18:20:27.000000 digital_rf-2.6.8/digital_rf/digital_rf_hdf5.py
--rw-rw-r--   0 root         (0) root         (0)     1820 2022-12-07 18:20:27.000000 digital_rf-2.6.8/digital_rf/drf_command.py
--rw-rw-r--   0 root         (0) root         (0)    23797 2022-12-07 18:20:27.000000 digital_rf-2.6.8/digital_rf/list_drf.py
--rw-rw-r--   0 root         (0) root         (0)    15110 2022-12-07 18:20:27.000000 digital_rf-2.6.8/digital_rf/mirror.py
--rw-rw-r--   0 root         (0) root         (0)    35796 2022-12-07 18:20:27.000000 digital_rf-2.6.8/digital_rf/ringbuffer.py
--rw-rw-r--   0 root         (0) root         (0)     9616 2022-12-07 18:20:27.000000 digital_rf-2.6.8/digital_rf/util.py
--rw-rw-r--   0 root         (0) root         (0)    20471 2022-12-07 18:20:27.000000 digital_rf-2.6.8/digital_rf/watchdog_drf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.936725 digital_rf-2.6.8/digital_rf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3627 2022-12-07 18:20:32.000000 digital_rf-2.6.8/digital_rf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5492 2022-12-07 18:20:32.000000 digital_rf-2.6.8/digital_rf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-07 18:20:32.000000 digital_rf-2.6.8/digital_rf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2022-12-07 18:20:32.000000 digital_rf-2.6.8/digital_rf.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      164 2022-12-07 18:20:32.000000 digital_rf-2.6.8/digital_rf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-12-07 18:20:32.000000 digital_rf-2.6.8/digital_rf.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.936725 digital_rf-2.6.8/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.936725 digital_rf-2.6.8/examples/beacon/
--rw-rw-r--   0 root         (0) root         (0)    43744 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/beacon/beacon_analysis.py
--rw-rw-r--   0 root         (0) root         (0)    34895 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/beacon/beacon_record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.936725 digital_rf-2.6.8/examples/beacon/config/
--rw-rw-r--   0 root         (0) root         (0)     1347 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/beacon/config/beacons.ini
--rw-rw-r--   0 root         (0) root         (0)      733 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/beacon/config/site.ini
--rw-rw-r--   0 root         (0) root         (0)     2889 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/benchmark_rf_read_hdf5.py
--rw-rw-r--   0 root         (0) root         (0)     4244 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/benchmark_rf_write_hdf5.py
--rw-rw-r--   0 root         (0) root         (0)     1888 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/example_read_digital_metadata.py
--rw-rw-r--   0 root         (0) root         (0)     2016 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/example_read_digital_rf.py
--rw-rw-r--   0 root         (0) root         (0)     3093 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/example_write_digital_metadata.py
--rw-rw-r--   0 root         (0) root         (0)     2798 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/example_write_digital_rf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.936725 digital_rf-2.6.8/examples/sounder/
--rw-rw-r--   0 root         (0) root         (0)      615 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/sounder/README.txt
--rwxrwxr-x   0 root         (0) root         (0)     7631 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/sounder/prc_analyze.py
--rwxrwxr-x   0 root         (0) root         (0)    37588 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/sounder/tx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.948725 digital_rf-2.6.8/examples/sounder/waveforms/
--rw-rw-r--   0 root         (0) root         (0)   800000 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/sounder/waveforms/code-l1000-b100-000000f.bin
--rw-rw-r--   0 root         (0) root         (0)   800000 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/sounder/waveforms/code-l10000-b10-000000.bin
--rw-rw-r--   0 root         (0) root         (0)  8000000 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/sounder/waveforms/const.bin
--rw-rw-r--   0 root         (0) root         (0)     3379 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/sounder/waveforms/create_waveform.py
--rw-rw-r--   0 root         (0) root         (0)   800000 2022-12-07 18:20:27.000000 digital_rf-2.6.8/examples/sounder/waveforms/pulse_2us.bin
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.952725 digital_rf-2.6.8/gr_digital_rf/
--rw-rw-r--   0 root         (0) root         (0)      334 2022-12-07 18:20:27.000000 digital_rf-2.6.8/gr_digital_rf/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    37844 2022-12-07 18:20:27.000000 digital_rf-2.6.8/gr_digital_rf/digital_rf_sink.py
--rw-rw-r--   0 root         (0) root         (0)    29369 2022-12-07 18:20:27.000000 digital_rf-2.6.8/gr_digital_rf/digital_rf_source.py
--rw-rw-r--   0 root         (0) root         (0)    22728 2022-12-07 18:20:27.000000 digital_rf-2.6.8/gr_digital_rf/raster.py
--rw-rw-r--   0 root         (0) root         (0)     4485 2022-12-07 18:20:27.000000 digital_rf-2.6.8/gr_digital_rf/vector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.956725 digital_rf-2.6.8/grc/
--rw-rw-r--   0 root         (0) root         (0)      388 2022-12-07 18:20:27.000000 digital_rf-2.6.8/grc/gr_digital_rf.tree.yml
--rw-rw-r--   0 root         (0) root         (0)    11581 2022-12-07 18:20:27.000000 digital_rf-2.6.8/grc/gr_digital_rf_digital_rf_channel_sink.block.yml
--rw-rw-r--   0 root         (0) root         (0)    14560 2022-12-07 18:20:27.000000 digital_rf-2.6.8/grc/gr_digital_rf_digital_rf_channel_sink.xml
--rw-rw-r--   0 root         (0) root         (0)     5564 2022-12-07 18:20:27.000000 digital_rf-2.6.8/grc/gr_digital_rf_digital_rf_channel_source.block.yml
--rw-rw-r--   0 root         (0) root         (0)     6212 2022-12-07 18:20:27.000000 digital_rf-2.6.8/grc/gr_digital_rf_digital_rf_channel_source.xml
--rw-r--r--   0 root         (0) root         (0)    16032 2022-12-07 18:20:28.000000 digital_rf-2.6.8/grc/gr_digital_rf_digital_rf_sink.block.yml
--rw-r--r--   0 root         (0) root         (0)    24761 2022-12-07 18:20:28.000000 digital_rf-2.6.8/grc/gr_digital_rf_digital_rf_sink.xml
--rw-r--r--   0 root         (0) root         (0)    16944 2022-12-07 18:20:29.000000 digital_rf-2.6.8/grc/gr_digital_rf_digital_rf_source.block.yml
--rw-r--r--   0 root         (0) root         (0)    29936 2022-12-07 18:20:28.000000 digital_rf-2.6.8/grc/gr_digital_rf_digital_rf_source.xml
--rw-rw-r--   0 root         (0) root         (0)     5714 2022-12-07 18:20:27.000000 digital_rf-2.6.8/grc/gr_digital_rf_raster_aggregate.block.yml
--rw-rw-r--   0 root         (0) root         (0)     7905 2022-12-07 18:20:27.000000 digital_rf-2.6.8/grc/gr_digital_rf_raster_aggregate.xml
--rw-rw-r--   0 root         (0) root         (0)     4545 2022-12-07 18:20:27.000000 digital_rf-2.6.8/grc/gr_digital_rf_raster_chunk.block.yml
--rw-rw-r--   0 root         (0) root         (0)     5862 2022-12-07 18:20:27.000000 digital_rf-2.6.8/grc/gr_digital_rf_raster_chunk.xml
--rw-rw-r--   0 root         (0) root         (0)     7583 2022-12-07 18:20:27.000000 digital_rf-2.6.8/grc/gr_digital_rf_raster_select.block.yml
--rw-rw-r--   0 root         (0) root         (0)    10079 2022-12-07 18:20:27.000000 digital_rf-2.6.8/grc/gr_digital_rf_raster_select.xml
--rw-rw-r--   0 root         (0) root         (0)     3912 2022-12-07 18:20:27.000000 digital_rf-2.6.8/grc/gr_digital_rf_raster_tag.block.yml
--rw-rw-r--   0 root         (0) root         (0)     5123 2022-12-07 18:20:27.000000 digital_rf-2.6.8/grc/gr_digital_rf_raster_tag.xml
--rw-rw-r--   0 root         (0) root         (0)     4186 2022-12-07 18:20:27.000000 digital_rf-2.6.8/grc/gr_digital_rf_vector_aggregate.block.yml
--rw-rw-r--   0 root         (0) root         (0)     6189 2022-12-07 18:20:27.000000 digital_rf-2.6.8/grc/gr_digital_rf_vector_aggregate.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.956725 digital_rf-2.6.8/include/
--rw-rw-r--   0 root         (0) root         (0)    11900 2022-12-07 18:20:26.000000 digital_rf-2.6.8/include/digital_rf.h
--rw-rw-r--   0 root         (0) root         (0)      115 2022-12-07 18:20:26.000000 digital_rf-2.6.8/include/digital_rf_version.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.956725 digital_rf-2.6.8/include/windows/
--rw-rw-r--   0 root         (0) root         (0)     8051 2022-12-07 18:20:26.000000 digital_rf-2.6.8/include/windows/inttypes.h
--rw-rw-r--   0 root         (0) root         (0)     7287 2022-12-07 18:20:26.000000 digital_rf-2.6.8/include/windows/stdint.h
--rw-rw-r--   0 root         (0) root         (0)     1696 2022-12-07 18:20:26.000000 digital_rf-2.6.8/include/windows/wincompat.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.956725 digital_rf-2.6.8/lib/
--rw-rw-r--   0 root         (0) root         (0)    18469 2022-12-07 18:20:27.000000 digital_rf-2.6.8/lib/py_rf_write_hdf5.c
--rw-rw-r--   0 root         (0) root         (0)    93680 2022-12-07 18:20:26.000000 digital_rf-2.6.8/lib/rf_write_hdf5.c
--rw-rw-r--   0 root         (0) root         (0)      108 2022-12-07 18:20:27.000000 digital_rf-2.6.8/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)      278 2022-12-07 18:20:32.964725 digital_rf-2.6.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)    11598 2022-12-07 18:20:27.000000 digital_rf-2.6.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.956725 digital_rf-2.6.8/tests/
--rw-rw-r--   0 root         (0) root         (0)     1388 2022-12-07 18:20:27.000000 digital_rf-2.6.8/tests/conftest.py
--rw-rw-r--   0 root         (0) root         (0)    51802 2022-12-07 18:20:27.000000 digital_rf-2.6.8/tests/test_digital_rf_hdf5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 18:20:32.960725 digital_rf-2.6.8/tools/
--rw-rw-r--   0 root         (0) root         (0)    10332 2022-12-07 18:20:27.000000 digital_rf-2.6.8/tools/digital_metadata_archive.py
--rw-rw-r--   0 root         (0) root         (0)    33006 2022-12-07 18:20:27.000000 digital_rf-2.6.8/tools/digital_rf_archive.py
--rw-rw-r--   0 root         (0) root         (0)     7544 2022-12-07 18:20:27.000000 digital_rf-2.6.8/tools/digital_rf_upconvert.py
--rw-rw-r--   0 root         (0) root         (0)     3987 2022-12-07 18:20:27.000000 digital_rf-2.6.8/tools/digital_rf_update_properties.py
--rw-rw-r--   0 root         (0) root         (0)    18043 2022-12-07 18:20:27.000000 digital_rf-2.6.8/tools/drf_cross_sti.py
--rw-rw-r--   0 root         (0) root         (0)    40473 2022-12-07 18:20:27.000000 digital_rf-2.6.8/tools/drf_plot.py
--rw-rw-r--   0 root         (0) root         (0)     8156 2022-12-07 18:20:27.000000 digital_rf-2.6.8/tools/drf_sound.py
--rw-rw-r--   0 root         (0) root         (0)    19978 2022-12-07 18:20:27.000000 digital_rf-2.6.8/tools/drf_sti.py
--rw-rw-r--   0 root         (0) root         (0)    71729 2022-12-07 18:20:27.000000 digital_rf-2.6.8/tools/thor.py
--rw-rw-r--   0 root         (0) root         (0)    60428 2022-12-07 18:20:27.000000 digital_rf-2.6.8/tools/thorosmo.py
--rwxrwxr-x   0 root         (0) root         (0)    54821 2022-12-07 18:20:27.000000 digital_rf-2.6.8/tools/thorpluto.py
--rw-rw-r--   0 root         (0) root         (0)    80011 2022-12-07 18:20:27.000000 digital_rf-2.6.8/tools/uhdtodrf.py
--rw-rw-r--   0 root         (0) root         (0)     2719 2022-12-07 18:20:27.000000 digital_rf-2.6.8/tools/verify_digital_rf_upconvert.py
--rw-rw-r--   0 root         (0) root         (0)    68751 2022-12-07 18:20:27.000000 digital_rf-2.6.8/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.851878 digital_rf-2.6.9/
+-rw-rw-r--   0 root         (0) root         (0)      625 2024-05-23 20:30:29.000000 digital_rf-2.6.9/AUTHORS
+-rw-rw-r--   0 root         (0) root         (0)    15833 2024-05-23 20:30:29.000000 digital_rf-2.6.9/CHANGELOG.rst
+-rw-rw-r--   0 root         (0) root         (0)     1602 2024-05-23 20:30:29.000000 digital_rf-2.6.9/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      684 2024-05-23 20:30:30.000000 digital_rf-2.6.9/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)      759 2024-05-23 20:30:30.000000 digital_rf-2.6.9/MANIFEST.md
+-rw-r--r--   0 root         (0) root         (0)     3627 2024-05-23 20:30:40.851878 digital_rf-2.6.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2058 2024-05-23 20:30:30.000000 digital_rf-2.6.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.787878 digital_rf-2.6.9/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.787878 digital_rf-2.6.9/data/example/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.791879 digital_rf-2.6.9/data/example/ch0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.791879 digital_rf-2.6.9/data/example/ch0/2019-08-29T19-00-00/
+-rw-rw-r--   0 root         (0) root         (0)    47608 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/example/ch0/2019-08-29T19-00-00/rf@1567105700.000.h5
+-rw-rw-r--   0 root         (0) root         (0)     2232 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/example/ch0/drf_properties.h5
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.791879 digital_rf-2.6.9/data/example/ch0/metadata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.791879 digital_rf-2.6.9/data/example/ch0/metadata/2019-08-29T19-00-00/
+-rw-rw-r--   0 root         (0) root         (0)    22944 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/example/ch0/metadata/2019-08-29T19-00-00/metadata@1567105700.h5
+-rw-rw-r--   0 root         (0) root         (0)     4192 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/example/ch0/metadata/dmd_properties.h5
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.787878 digital_rf-2.6.9/data/synthetic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.795879 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.795879 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/
+-rw-rw-r--   0 root         (0) root         (0)    11912 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368230.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    11912 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368231.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    11848 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368232.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    11912 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368233.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    11912 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368234.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    11912 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368236.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    11912 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368237.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    11848 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368238.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    11912 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368239.000.h5
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.795879 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/
+-rw-rw-r--   0 root         (0) root         (0)    11912 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368240.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    11848 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368241.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    11912 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368242.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    11912 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368243.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    11848 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368244.000.h5
+-rw-rw-r--   0 root         (0) root         (0)     2232 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/drf_properties.h5
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.795879 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.799878 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/
+-rw-rw-r--   0 root         (0) root         (0)    10744 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368230.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    10744 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368231.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    10480 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368232.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    10480 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368233.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    10480 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368234.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    10480 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368236.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    10744 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368237.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    10480 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368238.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    10744 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368239.000.h5
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.807878 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/
+-rw-rw-r--   0 root         (0) root         (0)    10744 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368240.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    10480 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368241.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    10744 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368242.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    10744 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368243.000.h5
+-rw-rw-r--   0 root         (0) root         (0)    10480 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368244.000.h5
+-rw-rw-r--   0 root         (0) root         (0)     2232 2024-05-23 20:30:29.000000 digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/drf_properties.h5
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.811878 digital_rf-2.6.9/digital_rf/
+-rw-rw-r--   0 root         (0) root         (0)     1123 2024-05-23 20:30:30.000000 digital_rf-2.6.9/digital_rf/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      497 2024-05-23 20:30:40.855878 digital_rf-2.6.9/digital_rf/_version.py
+-rw-rw-r--   0 root         (0) root         (0)    47645 2024-05-23 20:30:30.000000 digital_rf-2.6.9/digital_rf/digital_metadata.py
+-rw-rw-r--   0 root         (0) root         (0)    99813 2024-05-23 20:30:30.000000 digital_rf-2.6.9/digital_rf/digital_rf_deprecated_hdf5.py
+-rw-rw-r--   0 root         (0) root         (0)    83760 2024-05-23 20:30:30.000000 digital_rf-2.6.9/digital_rf/digital_rf_hdf5.py
+-rw-rw-r--   0 root         (0) root         (0)     1909 2024-05-23 20:30:30.000000 digital_rf-2.6.9/digital_rf/drf_command.py
+-rw-rw-r--   0 root         (0) root         (0)    24745 2024-05-23 20:30:30.000000 digital_rf-2.6.9/digital_rf/list_drf.py
+-rw-rw-r--   0 root         (0) root         (0)    17274 2024-05-23 20:30:30.000000 digital_rf-2.6.9/digital_rf/mirror.py
+-rw-rw-r--   0 root         (0) root         (0)    35796 2024-05-23 20:30:30.000000 digital_rf-2.6.9/digital_rf/ringbuffer.py
+-rw-rw-r--   0 root         (0) root         (0)     9616 2024-05-23 20:30:30.000000 digital_rf-2.6.9/digital_rf/util.py
+-rw-rw-r--   0 root         (0) root         (0)    20471 2024-05-23 20:30:30.000000 digital_rf-2.6.9/digital_rf/watchdog_drf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.811878 digital_rf-2.6.9/digital_rf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3627 2024-05-23 20:30:40.000000 digital_rf-2.6.9/digital_rf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5492 2024-05-23 20:30:40.000000 digital_rf-2.6.9/digital_rf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:30:40.000000 digital_rf-2.6.9/digital_rf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-05-23 20:30:40.000000 digital_rf-2.6.9/digital_rf.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2024-05-23 20:30:40.000000 digital_rf-2.6.9/digital_rf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-23 20:30:40.000000 digital_rf-2.6.9/digital_rf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.815878 digital_rf-2.6.9/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.815878 digital_rf-2.6.9/examples/beacon/
+-rw-rw-r--   0 root         (0) root         (0)    43746 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/beacon/beacon_analysis.py
+-rw-rw-r--   0 root         (0) root         (0)    34890 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/beacon/beacon_record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.815878 digital_rf-2.6.9/examples/beacon/config/
+-rw-rw-r--   0 root         (0) root         (0)     1347 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/beacon/config/beacons.ini
+-rw-rw-r--   0 root         (0) root         (0)      733 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/beacon/config/site.ini
+-rw-rw-r--   0 root         (0) root         (0)     2889 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/benchmark_rf_read_hdf5.py
+-rw-rw-r--   0 root         (0) root         (0)     4244 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/benchmark_rf_write_hdf5.py
+-rw-rw-r--   0 root         (0) root         (0)     1888 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/example_read_digital_metadata.py
+-rw-rw-r--   0 root         (0) root         (0)     2016 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/example_read_digital_rf.py
+-rw-rw-r--   0 root         (0) root         (0)     3097 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/example_write_digital_metadata.py
+-rw-rw-r--   0 root         (0) root         (0)     2798 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/example_write_digital_rf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.815878 digital_rf-2.6.9/examples/sounder/
+-rw-rw-r--   0 root         (0) root         (0)      615 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/sounder/README.txt
+-rwxrwxr-x   0 root         (0) root         (0)     7631 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/sounder/prc_analyze.py
+-rwxrwxr-x   0 root         (0) root         (0)    38601 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/sounder/tx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.835878 digital_rf-2.6.9/examples/sounder/waveforms/
+-rw-rw-r--   0 root         (0) root         (0)   800000 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/sounder/waveforms/code-l1000-b100-000000f.bin
+-rw-rw-r--   0 root         (0) root         (0)   800000 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/sounder/waveforms/code-l10000-b10-000000.bin
+-rw-rw-r--   0 root         (0) root         (0)  8000000 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/sounder/waveforms/const.bin
+-rw-rw-r--   0 root         (0) root         (0)     3379 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/sounder/waveforms/create_waveform.py
+-rw-rw-r--   0 root         (0) root         (0)   800000 2024-05-23 20:30:30.000000 digital_rf-2.6.9/examples/sounder/waveforms/pulse_2us.bin
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.839878 digital_rf-2.6.9/gr_digital_rf/
+-rw-rw-r--   0 root         (0) root         (0)      334 2024-05-23 20:30:30.000000 digital_rf-2.6.9/gr_digital_rf/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    37844 2024-05-23 20:30:30.000000 digital_rf-2.6.9/gr_digital_rf/digital_rf_sink.py
+-rw-rw-r--   0 root         (0) root         (0)    29369 2024-05-23 20:30:30.000000 digital_rf-2.6.9/gr_digital_rf/digital_rf_source.py
+-rw-rw-r--   0 root         (0) root         (0)    22728 2024-05-23 20:30:30.000000 digital_rf-2.6.9/gr_digital_rf/raster.py
+-rw-rw-r--   0 root         (0) root         (0)     4485 2024-05-23 20:30:30.000000 digital_rf-2.6.9/gr_digital_rf/vector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.843878 digital_rf-2.6.9/grc/
+-rw-rw-r--   0 root         (0) root         (0)      388 2024-05-23 20:30:30.000000 digital_rf-2.6.9/grc/gr_digital_rf.tree.yml
+-rw-rw-r--   0 root         (0) root         (0)    11581 2024-05-23 20:30:30.000000 digital_rf-2.6.9/grc/gr_digital_rf_digital_rf_channel_sink.block.yml
+-rw-rw-r--   0 root         (0) root         (0)    14560 2024-05-23 20:30:30.000000 digital_rf-2.6.9/grc/gr_digital_rf_digital_rf_channel_sink.xml
+-rw-rw-r--   0 root         (0) root         (0)     5564 2024-05-23 20:30:30.000000 digital_rf-2.6.9/grc/gr_digital_rf_digital_rf_channel_source.block.yml
+-rw-rw-r--   0 root         (0) root         (0)     6212 2024-05-23 20:30:30.000000 digital_rf-2.6.9/grc/gr_digital_rf_digital_rf_channel_source.xml
+-rw-r--r--   0 root         (0) root         (0)    16032 2024-05-23 20:30:33.000000 digital_rf-2.6.9/grc/gr_digital_rf_digital_rf_sink.block.yml
+-rw-r--r--   0 root         (0) root         (0)    24761 2024-05-23 20:30:33.000000 digital_rf-2.6.9/grc/gr_digital_rf_digital_rf_sink.xml
+-rw-r--r--   0 root         (0) root         (0)    16944 2024-05-23 20:30:34.000000 digital_rf-2.6.9/grc/gr_digital_rf_digital_rf_source.block.yml
+-rw-r--r--   0 root         (0) root         (0)    29936 2024-05-23 20:30:33.000000 digital_rf-2.6.9/grc/gr_digital_rf_digital_rf_source.xml
+-rw-rw-r--   0 root         (0) root         (0)     5714 2024-05-23 20:30:30.000000 digital_rf-2.6.9/grc/gr_digital_rf_raster_aggregate.block.yml
+-rw-rw-r--   0 root         (0) root         (0)     7905 2024-05-23 20:30:30.000000 digital_rf-2.6.9/grc/gr_digital_rf_raster_aggregate.xml
+-rw-rw-r--   0 root         (0) root         (0)     4545 2024-05-23 20:30:30.000000 digital_rf-2.6.9/grc/gr_digital_rf_raster_chunk.block.yml
+-rw-rw-r--   0 root         (0) root         (0)     5862 2024-05-23 20:30:30.000000 digital_rf-2.6.9/grc/gr_digital_rf_raster_chunk.xml
+-rw-rw-r--   0 root         (0) root         (0)     7583 2024-05-23 20:30:30.000000 digital_rf-2.6.9/grc/gr_digital_rf_raster_select.block.yml
+-rw-rw-r--   0 root         (0) root         (0)    10079 2024-05-23 20:30:30.000000 digital_rf-2.6.9/grc/gr_digital_rf_raster_select.xml
+-rw-rw-r--   0 root         (0) root         (0)     3912 2024-05-23 20:30:30.000000 digital_rf-2.6.9/grc/gr_digital_rf_raster_tag.block.yml
+-rw-rw-r--   0 root         (0) root         (0)     5123 2024-05-23 20:30:30.000000 digital_rf-2.6.9/grc/gr_digital_rf_raster_tag.xml
+-rw-rw-r--   0 root         (0) root         (0)     4186 2024-05-23 20:30:30.000000 digital_rf-2.6.9/grc/gr_digital_rf_vector_aggregate.block.yml
+-rw-rw-r--   0 root         (0) root         (0)     6189 2024-05-23 20:30:30.000000 digital_rf-2.6.9/grc/gr_digital_rf_vector_aggregate.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.847878 digital_rf-2.6.9/include/
+-rw-rw-r--   0 root         (0) root         (0)    11900 2024-05-23 20:30:29.000000 digital_rf-2.6.9/include/digital_rf.h
+-rw-rw-r--   0 root         (0) root         (0)      115 2024-05-23 20:30:29.000000 digital_rf-2.6.9/include/digital_rf_version.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.847878 digital_rf-2.6.9/include/windows/
+-rw-rw-r--   0 root         (0) root         (0)     8051 2024-05-23 20:30:29.000000 digital_rf-2.6.9/include/windows/inttypes.h
+-rw-rw-r--   0 root         (0) root         (0)     7287 2024-05-23 20:30:29.000000 digital_rf-2.6.9/include/windows/stdint.h
+-rw-rw-r--   0 root         (0) root         (0)     1696 2024-05-23 20:30:29.000000 digital_rf-2.6.9/include/windows/wincompat.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.847878 digital_rf-2.6.9/lib/
+-rw-rw-r--   0 root         (0) root         (0)    18469 2024-05-23 20:30:30.000000 digital_rf-2.6.9/lib/py_rf_write_hdf5.c
+-rw-rw-r--   0 root         (0) root         (0)    93680 2024-05-23 20:30:29.000000 digital_rf-2.6.9/lib/rf_write_hdf5.c
+-rw-rw-r--   0 root         (0) root         (0)      108 2024-05-23 20:30:30.000000 digital_rf-2.6.9/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)      278 2024-05-23 20:30:40.855878 digital_rf-2.6.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)    11599 2024-05-23 20:30:30.000000 digital_rf-2.6.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.847878 digital_rf-2.6.9/tests/
+-rw-rw-r--   0 root         (0) root         (0)     1388 2024-05-23 20:30:30.000000 digital_rf-2.6.9/tests/conftest.py
+-rw-rw-r--   0 root         (0) root         (0)    51800 2024-05-23 20:30:30.000000 digital_rf-2.6.9/tests/test_digital_rf_hdf5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:30:40.851878 digital_rf-2.6.9/tools/
+-rw-rw-r--   0 root         (0) root         (0)    10331 2024-05-23 20:30:30.000000 digital_rf-2.6.9/tools/digital_metadata_archive.py
+-rw-rw-r--   0 root         (0) root         (0)    33005 2024-05-23 20:30:30.000000 digital_rf-2.6.9/tools/digital_rf_archive.py
+-rw-rw-r--   0 root         (0) root         (0)     7544 2024-05-23 20:30:30.000000 digital_rf-2.6.9/tools/digital_rf_upconvert.py
+-rw-rw-r--   0 root         (0) root         (0)     3987 2024-05-23 20:30:30.000000 digital_rf-2.6.9/tools/digital_rf_update_properties.py
+-rw-rw-r--   0 root         (0) root         (0)    18038 2024-05-23 20:30:30.000000 digital_rf-2.6.9/tools/drf_cross_sti.py
+-rw-rw-r--   0 root         (0) root         (0)    40459 2024-05-23 20:30:30.000000 digital_rf-2.6.9/tools/drf_plot.py
+-rw-rw-r--   0 root         (0) root         (0)     8153 2024-05-23 20:30:30.000000 digital_rf-2.6.9/tools/drf_sound.py
+-rw-rw-r--   0 root         (0) root         (0)    19975 2024-05-23 20:30:30.000000 digital_rf-2.6.9/tools/drf_sti.py
+-rw-rw-r--   0 root         (0) root         (0)    71729 2024-05-23 20:30:30.000000 digital_rf-2.6.9/tools/thor.py
+-rw-rw-r--   0 root         (0) root         (0)    60426 2024-05-23 20:30:30.000000 digital_rf-2.6.9/tools/thorosmo.py
+-rwxrwxr-x   0 root         (0) root         (0)    54386 2024-05-23 20:30:30.000000 digital_rf-2.6.9/tools/thorpluto.py
+-rw-rw-r--   0 root         (0) root         (0)    80005 2024-05-23 20:30:30.000000 digital_rf-2.6.9/tools/uhdtodrf.py
+-rw-rw-r--   0 root         (0) root         (0)     2718 2024-05-23 20:30:30.000000 digital_rf-2.6.9/tools/verify_digital_rf_upconvert.py
+-rw-rw-r--   0 root         (0) root         (0)    86854 2024-05-23 20:30:30.000000 digital_rf-2.6.9/versioneer.py
```

### Comparing `digital_rf-2.6.8/AUTHORS` & `digital_rf-2.6.9/AUTHORS`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/CHANGELOG.rst` & `digital_rf-2.6.9/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,35 @@
 =====================
 digital_rf Change Log
 =====================
 
 .. current developments
 
+v2.6.9
+====================
+
+**Added:**
+
+* Add "link" method to mirror module and "ln" to `drf mirror`, to hard link files instead of copying. When hard linking is not possible (e.g. across different partitions), it will fall back to copying.
+* Add `drf ln` command to link files (hard or symbolic).
+* Added option `rdcc_nbytes` to `DigitalRFReader` to allow specification of HDF5 chunk cache size (see HDF5 documentation for details). This also increases the default chunk cache size from 1 MB to 4 MB to speed up reading of compressed or checksummed data in a typical use case.
+* The sounder/tx.py example script has been updated to accept waveform files in complex int16 format through use of the new `--type int16` argument.
+
+**Fixed:**
+
+* Fixed thorpluto.py, changed the iio.pluto_source to iio.fmcomms2_source_fc32 as the pluto_source was removed in newer versions of iio.
+
+**Authors:**
+
+* Ryan Volz
+* John Swoboda
+* Juha Vierinen
+
+
+
 v2.6.8
 ====================
 
 **Changed:**
 
 * drf_sti: Updated to have better arguments (consistent with more recent tools), handle data gaps, and add simple channel sum beamforming.
 * thor: Swap order of setting USRP clock and time sources, time first. This should reduce the number of re-syncs necessary with modern USRPs (N3xx, X4xx) in the absence of being able to do a set_sync_source call.
```

### Comparing `digital_rf-2.6.8/LICENSE` & `digital_rf-2.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/MANIFEST.in` & `digital_rf-2.6.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/MANIFEST.md` & `digital_rf-2.6.9/MANIFEST.md`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/PKG-INFO` & `digital_rf-2.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital_rf
-Version: 2.6.8
+Version: 2.6.9
 Summary: Python tools to read/write Digital RF data in HDF5 format
 Home-page: https://github.com/MITHaystack/digital_rf
 Author: MIT Haystack Observatory
 Author-email: openradar-developers@openradar.org
 License: BSD-3-Clause
 Description: The Digital RF project encompasses a standardized HDF5 format for reading and writing of radio frequency data and the software for doing so. The format is designed to be self-documenting for data archive and to allow rapid random access for data processing.
```

### Comparing `digital_rf-2.6.8/README.rst` & `digital_rf-2.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/example/ch0/2019-08-29T19-00-00/rf@1567105700.000.h5` & `digital_rf-2.6.9/data/example/ch0/2019-08-29T19-00-00/rf@1567105700.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/example/ch0/drf_properties.h5` & `digital_rf-2.6.9/data/example/ch0/drf_properties.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/example/ch0/metadata/2019-08-29T19-00-00/metadata@1567105700.h5` & `digital_rf-2.6.9/data/example/ch0/metadata/2019-08-29T19-00-00/metadata@1567105700.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/example/ch0/metadata/dmd_properties.h5` & `digital_rf-2.6.9/data/example/ch0/metadata/dmd_properties.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368230.000.h5` & `digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368230.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368231.000.h5` & `digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368231.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368232.000.h5` & `digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368232.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368233.000.h5` & `digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368233.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368234.000.h5` & `digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368234.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368236.000.h5` & `digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368236.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368237.000.h5` & `digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368237.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368238.000.h5` & `digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368238.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368239.000.h5` & `digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-30/rf@1394368239.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368240.000.h5` & `digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368240.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368241.000.h5` & `digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368241.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368242.000.h5` & `digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368242.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368243.000.h5` & `digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368243.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368244.000.h5` & `digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/2014-03-09T12-30-40/rf@1394368244.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/drf_properties.h5` & `digital_rf-2.6.9/data/synthetic/fc32_x8_n200_d3_10s_1000ms_c1/drf_properties.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368230.000.h5` & `digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368230.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368231.000.h5` & `digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368231.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368232.000.h5` & `digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368232.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368233.000.h5` & `digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368233.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368234.000.h5` & `digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368234.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368236.000.h5` & `digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368236.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368237.000.h5` & `digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368237.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368238.000.h5` & `digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368238.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368239.000.h5` & `digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-30/rf@1394368239.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368240.000.h5` & `digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368240.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368241.000.h5` & `digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368241.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368242.000.h5` & `digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368242.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368243.000.h5` & `digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368243.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368244.000.h5` & `digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/2014-03-09T12-30-40/rf@1394368244.000.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/drf_properties.h5` & `digital_rf-2.6.9/data/synthetic/sc16_x1_n200_d3_10s_1000ms_c0/drf_properties.h5`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/digital_rf/__init__.py` & `digital_rf-2.6.9/digital_rf/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os as _os
 
 from .digital_metadata import *  # noqa: F401,F403
 from .digital_rf_hdf5 import *  # noqa: F401,F403
 from . import list_drf  # noqa: F401
 from .list_drf import ilsdrf, lsdrf  # noqa: F401
 from . import util  # noqa: F401
-from ._version import get_versions
+from . import _version
 
 _logging.basicConfig(
     level=_os.environ.get(
         "DRF_LOGLEVEL", _os.environ.get("LOGLEVEL", "WARNING")
     ).upper()
 )
 _logger = _logging.getLogger(__name__)
@@ -27,9 +27,8 @@
         "Failed to import the `mirror`, `ringbuffer`, and/or `watchdog_drf` modules,"
         " likely because the `watchdog` package is not installed or is incompatible."
         " You can safely ignore this if you do not need the functionality of any of"
         " those modules."
     )
     _logger.info(watchdog_msg, exc_info=True)
 
-__version__ = get_versions()["version"]
-del get_versions
+__version__ = _version.get_versions()["version"]
```

### Comparing `digital_rf-2.6.8/digital_rf/digital_metadata.py` & `digital_rf-2.6.9/digital_rf/digital_metadata.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/digital_rf/digital_rf_deprecated_hdf5.py` & `digital_rf-2.6.9/digital_rf/digital_rf_deprecated_hdf5.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/digital_rf/digital_rf_hdf5.py` & `digital_rf-2.6.9/digital_rf/digital_rf_hdf5.py`

 * *Files 1% similar despite different names*

```diff
@@ -788,26 +788,30 @@
 class DigitalRFReader(object):
     """Read data in Digital RF HDF5 format.
 
     This class allows random access to the rf data.
 
     """
 
-    def __init__(self, top_level_directory_arg):
+    def __init__(self, top_level_directory_arg, rdcc_nbytes=4000000):
         """Initialize reader to directory containing Digital RF channels.
 
         Parameters
         ----------
         top_level_directory_arg : string
             Either a single top level directory containing Digital RF channel
             directories, or a list of such. A directory can be a file system
             path or a url, where the url points to a top level directory. Each
             must be a local path, or start with 'http://'', 'file://'', or
             'ftp://''.
 
+        rdcc_nbytes : int, optional
+            HDF5 chunk cache size. Needs to be at least file size
+            for efficient access of compressed or checksummed files to
+            avoid serious performance penalties with sparse data access.
 
         Notes
         -----
         A top level directory must contain files in the format:
             [channel]/[YYYY-MM-DDTHH-MM-SS]/rf@[seconds].[%03i milliseconds].h5
 
         If more than one top level directory contains the same channel_name
@@ -858,15 +862,18 @@
                     channel_dict[channel_name] = [top_level_dir]
 
         # update all channels
         for channel_name in channel_dict.keys():
             top_level_dir_properties_list = []
             for top_level_dir in channel_dict[channel_name]:
                 new_top_level_metadata = _top_level_dir_properties(
-                    top_level_dir, channel_name, self._top_level_dir_dict[top_level_dir]
+                    top_level_dir,
+                    channel_name,
+                    self._top_level_dir_dict[top_level_dir],
+                    rdcc_nbytes=rdcc_nbytes,
                 )
                 top_level_dir_properties_list.append(new_top_level_metadata)
             new_channel_properties = _channel_properties(
                 channel_name, top_level_dir_meta_list=top_level_dir_properties_list
             )
             self._channel_dict[channel_name] = new_channel_properties
 
@@ -1851,33 +1858,39 @@
     """A Digital RF channel in a specific top-level directory."""
 
     _min_version = packaging.version.parse("2.0")
     _max_version = packaging.version.parse(
         packaging.version.parse(__version__).base_version
     )
 
-    def __init__(self, top_level_dir, channel_name, access_mode):
+    def __init__(self, top_level_dir, channel_name, access_mode, rdcc_nbytes=4000000):
         """Create a new _top_level_dir_properties object.
 
         Parameters
         ----------
         top_level_dir : string
             Full path the top-level directory that contains the parent
             `channel_name`.
 
         channel_name : string
             The subdirectory name for the channel.
 
         access_mode : string
             String giving the access mode ('local', 'file', or 'http').
 
+        rdcc_nbytes : int, optional
+            HDF5 chunk cache size. Needs to be at least file size
+            for efficient access of compressed or checksummed files to
+            avoid serious performance penalties with sparse data access.
+
         """
         self.top_level_dir = top_level_dir
         self.channel_name = channel_name
         self.access_mode = access_mode
+        self.rdcc_nbytes = rdcc_nbytes
         self._cachedFilename = None  # full name of last file opened
         self._cachedFile = None  # h5py.File object of last file opened
         # expect that _read_properties() will not raise error since we
         # already checked for existence of drf_properties.h5 before init
         self.properties = self._read_properties()
         try:
             version = self.properties["digital_rf_version"]
@@ -2025,29 +2038,32 @@
                 if fullfile != self._cachedFilename:
                     if self._cachedFile is not None:
                         try:
                             self._cachedFile.close()
                         except ValueError:
                             # already closed
                             pass
-                    self._cachedFile = h5py.File(fullfile, "r")
+                    self._cachedFile = h5py.File(
+                        fullfile, "r", rdcc_nbytes=self.rdcc_nbytes
+                    )
                     self._cachedFilename = fullfile
-                rf_data = self._cachedFile["rf_data"]
-                rf_data_len = rf_data.shape[0]
+                    self.rf_data = self._cachedFile["rf_data"]
+                    self.rf_data_len = self.rf_data.shape[0]
+
+                    self.rf_index = self._cachedFile["rf_data_index"][...]
+                    self.rf_index_len = self.rf_index.shape[0]
 
-                rf_index = self._cachedFile["rf_data_index"][...]
-                rf_index_len = rf_index.shape[0]
                 # loop through each row in rf_index
-                for row in range(rf_index_len):
-                    block_start_sample = int(rf_index[row, 0])
-                    block_start_index = int(rf_index[row, 1])
-                    if row + 1 == rf_index_len:
-                        block_stop_index = rf_data_len
+                for row in range(self.rf_index_len):
+                    block_start_sample = int(self.rf_index[row, 0])
+                    block_start_index = int(self.rf_index[row, 1])
+                    if row + 1 == self.rf_index_len:
+                        block_stop_index = self.rf_data_len
                     else:
-                        block_stop_index = int(rf_index[row + 1, 1])
+                        block_stop_index = int(self.rf_index[row + 1, 1])
                     block_stop_sample = block_start_sample + (
                         block_stop_index - block_start_index
                     )
 
                     if start_sample <= block_start_sample:
                         read_start_index = block_start_index
                         read_start_sample = block_start_sample
@@ -2068,17 +2084,17 @@
                         )
 
                     # skip if no data found
                     if read_start_index >= read_stop_index:
                         continue
                     if not len_only:
                         if sub_channel is None:
-                            data = rf_data[read_start_index:read_stop_index]
+                            data = self.rf_data[read_start_index:read_stop_index]
                         else:
-                            data = rf_data[
+                            data = self.rf_data[
                                 read_start_index:read_stop_index, sub_channel
                             ]
                         cont_data_dict[read_start_sample] = data
                     else:
                         cont_data_dict[read_start_sample] = (
                             read_stop_index - read_start_index
                         )
```

### Comparing `digital_rf-2.6.8/digital_rf/drf_command.py` & `digital_rf-2.6.9/digital_rf/drf_command.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 #
 # The full license is in the LICENSE file, distributed with this software.
 # ----------------------------------------------------------------------------
 from __future__ import absolute_import, division, print_function
 
 from argparse import ArgumentParser
 
-from .list_drf import _build_cp_parser, _build_ls_parser, _build_mv_parser
+from .list_drf import (
+    _build_cp_parser,
+    _build_ln_parser,
+    _build_ls_parser,
+    _build_mv_parser,
+)
 
 try:
     from .mirror import _build_mirror_parser
     from .ringbuffer import _build_ringbuffer_parser
     from .watchdog_drf import _build_watch_parser
 except ImportError:
     _WATCHDOG = False
@@ -30,14 +35,15 @@
             " commands.)"
         )
         epi = epi + " " + s
     parser = ArgumentParser(description="Digital RF command line tools.", epilog=epi)
     subparsers = parser.add_subparsers(title="Available commands")
 
     _build_cp_parser(subparsers.add_parser, "cp")
+    _build_ln_parser(subparsers.add_parser, "ln")
     _build_ls_parser(subparsers.add_parser, "ls")
     _build_mv_parser(subparsers.add_parser, "mv")
     if _WATCHDOG:
         _build_mirror_parser(subparsers.add_parser, "mirror")
         _build_ringbuffer_parser(subparsers.add_parser, "ringbuffer")
         _build_watch_parser(subparsers.add_parser, "watch")
```

### Comparing `digital_rf-2.6.8/digital_rf/list_drf.py` & `digital_rf-2.6.9/digital_rf/list_drf.py`

 * *Files 4% similar despite different names*

```diff
@@ -684,34 +684,65 @@
     parser = _add_srcdest_arguments(parser)
     parser.set_defaults(func=_run_cp)
     return parser
 
 
 def _run_cp(args):
     args, kwargs = _parse_srcdest_args(args)
-    for (src, dest) in args.srcdests:
+    for src, dest in args.srcdests:
         for srcpath in ilsdrf(src, **kwargs):
             destpath = os.path.join(dest, os.path.relpath(srcpath, src))
             destdir = os.path.dirname(destpath)
             if not os.path.exists(destdir):
                 os.makedirs(destdir)
             shutil.copy2(srcpath, destpath)
 
 
+def _build_ln_parser(Parser, *args):
+    desc = "Link Digital RF/Metadata files from source to destination."
+    parser = Parser(*args, description=desc)
+    parser = _add_srcdest_arguments(parser)
+    parser.add_argument(
+        "--symbolic",
+        "--sym",
+        action="store_true",
+        help="""Make symbolic links instead of hard links.
+                (default: False)""",
+    )
+    parser.set_defaults(func=_run_ln)
+    return parser
+
+
+def _run_ln(args):
+    if args.symbolic:
+        link_fun = os.symlink
+    else:
+        link_fun = os.link
+    del args.symbolic
+    args, kwargs = _parse_srcdest_args(args)
+    for src, dest in args.srcdests:
+        for srcpath in ilsdrf(src, **kwargs):
+            destpath = os.path.join(dest, os.path.relpath(srcpath, src))
+            destdir = os.path.dirname(destpath)
+            if not os.path.exists(destdir):
+                os.makedirs(destdir)
+            link_fun(srcpath, destpath)
+
+
 def _build_mv_parser(Parser, *args):
     desc = "Move Digital RF/Metadata files from source to destination."
     parser = Parser(*args, description=desc)
     parser = _add_srcdest_arguments(parser)
     parser.set_defaults(func=_run_mv)
     return parser
 
 
 def _run_mv(args):
     args, kwargs = _parse_srcdest_args(args)
-    for (src, dest) in args.srcdests:
+    for src, dest in args.srcdests:
         for srcpath in ilsdrf(src, **kwargs):
             destpath = os.path.join(dest, os.path.relpath(srcpath, src))
             destdir = os.path.dirname(destpath)
             if not os.path.exists(destdir):
                 os.makedirs(destdir)
             shutil.move(srcpath, destpath)
```

### Comparing `digital_rf-2.6.8/digital_rf/mirror.py` & `digital_rf-2.6.9/digital_rf/mirror.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,15 @@
 
     def __init__(
         self,
         src,
         dest,
         method="move",
         ignore_existing=False,
+        link=False,
         verbose=False,
         starttime=None,
         endtime=None,
         include_drf=True,
         include_dmd=True,
         force_polling=False,
     ):
@@ -164,28 +165,36 @@
         ----------
         src : str
             Source directory to monitor.
 
         dest : str
             Destination directory.
 
-        method : 'move' | 'copy'
+        method : 'move' | 'copy' | 'link'
             Mirroring method. New Digital RF files in the source directory will
-            be moved or copied to the destination directory depending on this
-            parameter. Metadata is always copied regardless of this parameter.
+            be moved or copied/hardlinked to the destination directory depending
+            on this parameter. Metadata is always copied/hardlinked regardless
+            of this parameter.
 
 
         Other Parameters
         ----------------
         ignore_existing : bool
             If True, existing Digital RF and Digital Metadata files will not be
             mirrored. Otherwise, they will be mirrored to the destination
             directory along with any existing channel metadata files
             when mirroring starts.
 
+        link : bool
+            If True, files that would be copied (because `method` is copy or
+            because the files are Digital Metadata) are instead hard linked.
+            When hard linking is not possible, files will be copied instead.
+            Linking is enabled regardless of this value when the `method` is
+            'link'.
+
         verbose : bool
             If True, print the name of mirrored files.
 
         starttime : datetime.datetime
             Data covering this time or after will be included. This has no
             effect on property files.
 
@@ -204,40 +213,75 @@
         force_polling : bool
             If True, force the watchdog to use polling instead of the default
             observer.
 
         """
         self.src = os.path.abspath(src)
         self.dest = os.path.abspath(dest)
-        if method not in ("move", "copy"):
-            raise ValueError('Mirror method must be either "move" or "copy".')
+        if method not in ("move", "copy", "link"):
+            raise ValueError('Mirror method must be either "move", "copy", or "link"')
         self.method = method
         self.ignore_existing = ignore_existing
+        self.link = link
         self.verbose = verbose
         self.starttime = starttime
         self.endtime = endtime
         self.include_drf = include_drf
         self.include_dmd = include_dmd
         self.force_polling = force_polling
 
         if not self.include_drf and not self.include_dmd:
             errstr = "One of `include_drf` or `include_dmd` must be True."
             raise ValueError(errstr)
 
+        if self.method == "link":
+            self.link = True
+        elif self.method == "copy" and self.link:
+            self.method = "link"
+
+        if self.link:
+            # set up a hard linking function that falls back to copying
+            class LinkWithFallback(object):
+                def __init__(self):
+                    self.unlinkable_path_pairs = set()
+
+                def __call__(self, src, dst):
+                    src_dir = os.path.dirname(src)
+                    dst_dir = os.path.dirname(dst)
+                    if (src_dir, dst_dir) not in self.unlinkable_path_pairs:
+                        try:
+                            os.link(src, dst)
+                        except FileExistsError:
+                            # assume we've already linked this file
+                            # (e.g. a Digital Metadata file has been newly written to,
+                            #  but we've already hard linked it)
+                            pass
+                        except OSError:
+                            print((src_dir, dst_dir))
+                            self.unlinkable_path_pairs.add((src_dir, dst_dir))
+                            # fall back to copying
+                            shutil.copy2(src, dst)
+                    else:
+                        shutil.copy2(src, dst)
+
+            copylike_mirror_fun = LinkWithFallback()
+        else:
+            copylike_mirror_fun = shutil.copy2
+
         self.event_handlers = []
         # have to copy properties files because static,
         # have to copy metadata because can be modified
         copy_handler = DigitalRFMirrorHandler(
             self.src,
             self.dest,
             verbose=verbose,
-            mirror_fun=shutil.copy2,
+            mirror_fun=copylike_mirror_fun,
             starttime=self.starttime,
             endtime=self.endtime,
-            include_drf=(self.include_drf and self.method == "copy"),
+            include_drf=(self.include_drf and self.method in ("copy", "link")),
             include_dmd=self.include_dmd,
             include_drf_properties=self.include_drf,
             include_dmd_properties=self.include_dmd,
         )
         self.event_handlers.append(copy_handler)
 
         if self.include_drf and self.method == "move":
@@ -360,25 +404,31 @@
         self.observer.stop()
 
 
 def _build_mirror_parser(Parser, *args):
     desc = "Mirror Digital RF files from one directory to another."
     parser = Parser(*args, description=desc)
 
-    parser.add_argument("method", choices=["mv", "cp"], help="Mirroring method.")
+    parser.add_argument("method", choices=["mv", "cp", "ln"], help="Mirroring method.")
     parser.add_argument("src", help="Source directory to monitor.")
     parser.add_argument("dest", help="Destination directory.")
     parser.add_argument(
         "-v", "--verbose", action="store_true", help="Print the name of mirrored files."
     )
     parser.add_argument(
         "--ignore_existing",
         action="store_true",
         help="Ignore existing files in source directory.",
     )
+    parser.add_argument(
+        "--link",
+        action="store_true",
+        help="""Use hardlinking in place of copying when possible. This is always
+                enabled when the `method` is 'ln'. (default: False)""",
+    )
 
     parser = list_drf._add_time_group(parser)
 
     includegroup = parser.add_argument_group(title="include")
     includegroup.add_argument(
         "--nodrf",
         dest="include_drf",
@@ -400,15 +450,15 @@
 
     return parser
 
 
 def _run_mirror(args):
     import signal
 
-    methods = {"mv": "move", "cp": "copy"}
+    methods = {"mv": "move", "cp": "copy", "ln": "link"}
     args.method = methods[args.method]
 
     if args.starttime is not None:
         args.starttime = util.parse_identifier_to_time(args.starttime)
     if args.endtime is not None:
         args.endtime = util.parse_identifier_to_time(
             args.endtime, ref_datetime=args.starttime
```

### Comparing `digital_rf-2.6.8/digital_rf/ringbuffer.py` & `digital_rf-2.6.9/digital_rf/ringbuffer.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/digital_rf/util.py` & `digital_rf-2.6.9/digital_rf/util.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/digital_rf/watchdog_drf.py` & `digital_rf-2.6.9/digital_rf/watchdog_drf.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/digital_rf.egg-info/PKG-INFO` & `digital_rf-2.6.9/digital_rf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-rf
-Version: 2.6.8
+Version: 2.6.9
 Summary: Python tools to read/write Digital RF data in HDF5 format
 Home-page: https://github.com/MITHaystack/digital_rf
 Author: MIT Haystack Observatory
 Author-email: openradar-developers@openradar.org
 License: BSD-3-Clause
 Description: The Digital RF project encompasses a standardized HDF5 format for reading and writing of radio frequency data and the software for doing so. The format is designed to be self-documenting for data archive and to allow rapid random access for data processing.
```

### Comparing `digital_rf-2.6.8/digital_rf.egg-info/SOURCES.txt` & `digital_rf-2.6.9/digital_rf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/examples/beacon/beacon_analysis.py` & `digital_rf-2.6.9/examples/beacon/beacon_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 TLE_def = (
     "CASSIOPE",
     "1 39265U 13055A   17015.93102647 +.00001768 +00000-0 +52149-4 0  9992",
     "2 39265 080.9701 172.4450 0693099 333.2926 023.4045 14.21489964169876",
 )
 debug_plot = False
 
+
 # update_progress() : Displays or updates a console progress bar
 ## Accepts a float between 0 and 1. Any int will be converted to a float.
 ## A value under 0 represents a 'halt'.
 ## A value at 1 or bigger represents 100%
 def update_progress(progress):
     barLength = 100  # Modify this to change the length of the progress bar
     status = ""
@@ -86,15 +87,15 @@
             {
                     't': Time in posix,
                     'dop1': Doppler frequency of 150 MHz channel from TLE ,
                     'dop2': Doppler frequency of 400 MHz channel from TLE ,
             }
     """
 
-    #%% Get Ephem info
+    # %% Get Ephem info
     # Assuming this will stay the same
     ut0 = 25567.5
     e2p = 3600.0 * 24  # ephem day to utc seconds
 
     sitepath = os.path.expanduser(os.path.join(maindir, "metadata/config/site"))
     sitemeta = drf.DigitalMetadataReader(sitepath)
     sdict = sitemeta.read_latest()
@@ -562,15 +563,14 @@
     std1 = sp.zeros(len(start_vec))
     fi = window // 2
     subchan = 0
     outspec0 = sp.zeros((len(tvec), window))
     outspec1 = sp.zeros((len(tvec), window))
     print("Start Beacon Processing")
     for i_t, c_st in enumerate(start_vec):
-
         update_progress(float(i_t) / float(len(start_vec)))
         t_cur = tvec[i_t]
 
         z00 = drfObj.read_vector(c_st, Nr, chans[0], subchan)[Msamp]
         z01 = drfObj.read_vector(c_st + soff, Nr, chans[0], subchan)[Msamp]
         z10 = drfObj.read_vector(c_st, Nr, chans[1], subchan)[Msamp]
         z11 = drfObj.read_vector(c_st + soff, Nr, chans[1], subchan)[Msamp]
@@ -677,15 +677,15 @@
         "phasestd": stdcurve,
         "outspec0": outspec0,
         "outspec1": outspec1,
     }
     return outdict
 
 
-#%% Plotting
+# %% Plotting
 def plotsti_vel(
     maindir,
     savename="chancomp.png",
     timewin=[0, 0],
     offset=0,
     window=512,
     sfactor=2,
@@ -741,15 +741,14 @@
 
     wfun = sig.get_window("hann", window)
     wmat = sp.tile(wfun[sp.newaxis, :], (incoh_int, 1))
 
     sti0 = sp.zeros((Nt, window), float)
     sti1 = sp.zeros_like(sti0)
     for i_t, c_st in enumerate(start_vec):
-
         z0 = drfObj.read_vector(c_st, Nr, chans[0], subchan)
         z1 = drfObj.read_vector(c_st, Nr, chans[1], subchan)
         for idec in dec_vec:
             z0 = sig.decimate(z0, idec)
             z1 = sig.decimate(z1, idec)
 
         z0 = z0[Msamp]
@@ -1051,15 +1050,15 @@
     # plt.tight_layout()
     figpath, name = os.path.split(savename)
     savename = os.path.join(figpath, "amp" + name)
     fig1.savefig(savename, dpi=300)
     plt.close(fig1)
 
 
-#%% I/O for measurements
+# %% I/O for measurements
 def save_output(maindirmeta, outdict, e):
     """
     This function saves the output of the relative TEC measurement processing.
 
     Args:
         maindir (:obj:`str`): Path for data.
         outdict (dict[str, obj]): Output data dictionary::
@@ -1118,15 +1117,15 @@
         return None
     metadict = dmeta.read_latest()
     outdict = list(metadict.values())[0]
 
     return outdict
 
 
-#%% Run from commandline material
+# %% Run from commandline material
 def analyzebeacons(input_args):
     """
     This function will run the analysis code and save the data. Plots will be
     made as well if desired.
     """
     # makes sure theres no trailing / for the path
     mainpath = os.path.expanduser(os.path.dirname(os.path.join(input_args.path, "")))
@@ -1156,15 +1155,14 @@
         if outdict is None:
             print("No ouptut data exists")
         else:
             plot_resid(outdict["resid"], os.path.join(figspath, "resid.png"))
             plot_measurements(outdict, savename)
             plot_map(outdict, e, os.path.join(figspath, "mapdata.png"))
     else:
-
         outdict = calc_TEC(
             mainpath,
             window=input_args.window,
             incoh_int=input_args.incoh,
             sfactor=input_args.overlap,
             offset=tleoff,
             timewin=[input_args.begoff, input_args.endoff],
```

### Comparing `digital_rf-2.6.8/examples/beacon/beacon_record.py` & `digital_rf-2.6.9/examples/beacon/beacon_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -495,15 +495,14 @@
 
     ctime = st0
     etime = et0
 
     last_sat_rise = ctime
 
     while ctime < etime:
-
         obj = get_next_object(opt, site, objects, ctime)
 
         obj_id = obj
         obj_info = objects[obj]
 
         if opt.debug:
             print("# object ", obj_id, " @ ", ctime)
@@ -662,15 +661,14 @@
                         site["recorder"]["channels"][1:-1], ","
                     )
                     radio_sample_rate = site["radio"]["sample_rate"]
 
                     cmd_line0 = "%s " % (site["recorder"]["command"])
 
                     if site["radio"]["type"] == "b210":
-
                         # just record a fixed frequency, needs a dual radio Thor3 script. This can be done!
                         idx = 0
                         freq = obj_freqs[1]
 
                         cmd_line1 = '-r %s -d "%s" -s %s -e %s -c %s -f %4.3f ' % (
                             radio_sample_rate,
                             radio_channel[idx],
@@ -723,15 +721,14 @@
                                 obj_info,
                             )
                         )
 
                         print("\n")
 
                     elif site["radio"]["type"] == "n200_tvrx2":
-
                         cmd_line1 = (
                             ' -r %s -d "%s %s" -s %s -e %s -c %s,%s -f %4.3f,%4.3f '
                             % (
                                 radio_sample_rate,
                                 radio_channel[0],
                                 radio_channel[1],
                                 offset_rise_time,
@@ -800,15 +797,14 @@
 
                     while time.time() < start0 - 30:
                         time.sleep(op.interval)
                         if opt.verbose:
                             print("#    %d sec" % (start0 - time.time()))
 
                     for cmd_tuple in cmd_lines:
-
                         cmd, cmd_fname, pass_md, info_md = cmd_tuple
 
                         print("# Executing command %s " % (cmd))
 
                         # write the digital metadata
                         start_idx = int(start0)
                         mdata_dir = (
@@ -819,15 +815,14 @@
                         )
 
                         # site metadata
                         # note we use directory structure for the dictionary here
                         # eventually we will add this feature to digital metadata
 
                         for k in site:
-
                             try:
                                 os.makedirs(mdata_dir + "/config/%s" % (k))
                             except:
                                 pass
 
                             md_site_obj = DigitalMetadataWriter(
                                 mdata_dir + "/config/%s" % (k), 3600, 60, 1, 1, k
```

### Comparing `digital_rf-2.6.8/examples/beacon/config/beacons.ini` & `digital_rf-2.6.9/examples/beacon/config/beacons.ini`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/examples/beacon/config/site.ini` & `digital_rf-2.6.9/examples/beacon/config/site.ini`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/examples/benchmark_rf_read_hdf5.py` & `digital_rf-2.6.9/examples/benchmark_rf_read_hdf5.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/examples/benchmark_rf_write_hdf5.py` & `digital_rf-2.6.9/examples/benchmark_rf_write_hdf5.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/examples/example_read_digital_metadata.py` & `digital_rf-2.6.9/examples/example_read_digital_metadata.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/examples/example_read_digital_rf.py` & `digital_rf-2.6.9/examples/example_read_digital_rf.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/examples/example_write_digital_metadata.py` & `digital_rf-2.6.9/examples/example_write_digital_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,21 +60,21 @@
 complex_data = np.arange(70, dtype=np.complex64)
 data_dict["complex_data"] = complex_data
 single_int = 5
 data_dict["single_int"] = np.int32(single_int)
 single_float = 6.0
 data_dict["single_float"] = np.float64(single_float)
 single_complex = 7.0 + 8.0j
-data_dict["single_complex"] = np.complex(single_complex)
+data_dict["single_complex"] = np.complex64(single_complex)
 
 # now create subdirectories
 sub_dict = {}
 sub_dict["single_int"] = np.int32(single_int)
 sub_dict["single_float"] = np.float64(single_float)
-sub_dict["single_complex"] = np.complex(single_complex)
+sub_dict["single_complex"] = np.complex64(single_complex)
 level2_dict = {}  # embed yey another level
 level2_dict["single_float"] = np.float64(single_float)
 sub_dict["level2"] = level2_dict
 
 
 data_dict["sub_system"] = sub_dict
```

### Comparing `digital_rf-2.6.8/examples/example_write_digital_rf.py` & `digital_rf-2.6.9/examples/example_write_digital_rf.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/examples/sounder/README.txt` & `digital_rf-2.6.9/examples/sounder/README.txt`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/examples/sounder/prc_analyze.py` & `digital_rf-2.6.9/examples/sounder/prc_analyze.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/examples/sounder/tx.py` & `digital_rf-2.6.9/examples/sounder/tx.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     """
     # make sure mode_ini exists as named, or add extension
     mode_ini = os.path.abspath(mode_ini)
     if not os.path.isfile(mode_ini):
         mode_ini = mode_ini + ".iq.ini"
 
     # parse mode INI file (so we can fail early if it's bad)
-    cparser = configparser.SafeConfigParser()
+    cparser = configparser.ConfigParser()
     try:
         cparser.read(mode_ini)
     except configparser.MissingSectionHeaderError:
         raise ValueError("Cannot read timing mode INI file.")
     if not cparser.has_section("mode"):
         raise ValueError("Cannot read timing mode INI file.")
 
@@ -234,14 +234,26 @@
             del u
 
     @staticmethod
     def _parse_options(**kwargs):
         """Put all keyword options in a namespace and normalize them."""
         op = Namespace(**kwargs)
 
+        if op.waveform is not None:
+            if op.waveform.dtype == np.complex64:
+                op.cpu_format = "fc32"
+            elif op.waveform.dtype == np.int16:
+                op.cpu_format = "sc16"
+                wrn = "Waveform dtype is int16, amplitudes and phases will be ignored!"
+                print(f"\033[93m{wrn}\033[00m")
+            else:
+                raise ValueError(
+                    f"Waveform dtype {op.waveform.dtype} must be complex64 or int16"
+                )
+
         # determine mboard and subdev per channel, get number of channels
         op.mboards_bychan = []
         op.subdevs_bychan = []
         op.mboardnum_bychan = []
         mboards = op.mboards if op.mboards else ["default"]
         for mbnum, (mb, sd) in enumerate(zip(mboards, op.subdevs)):
             sds = sd.split()
@@ -335,15 +347,15 @@
     def _usrp_setup(self):
         """Create, set up, and return USRP sink object."""
         op = self.op
         # create usrp sink block
         u = uhd.usrp_sink(
             device_addr=",".join(chain(op.mboard_strs, op.dev_args)),
             stream_args=uhd.stream_args(
-                cpu_format="fc32",
+                cpu_format=op.cpu_format,
                 otw_format="sc16",
                 channels=list(range(op.nchs)),
                 args=",".join(op.stream_args),
             ),
         )
 
         # set clock and time source if synced
@@ -632,16 +644,21 @@
         u.set_start_time(uhd.time_spec(ct_secs) + uhd.time_spec(ct_frac))
 
         # populate flowgraph one channel at a time
         fg = gr.top_block()
         for k in range(op.nchs):
             mult_k = op.amplitudes[k] * np.exp(1j * op.phases[k])
             if op.waveform is not None:
-                waveform_k = mult_k * op.waveform
-                src_k = blocks.vector_source_c(waveform_k.tolist(), repeat=True)
+                if op.waveform.dtype == np.complex64:
+                    waveform_k = mult_k * op.waveform
+                    src_k = blocks.vector_source_c(waveform_k.tolist(), repeat=True)
+                else:
+                    src_k = blocks.vector_source_s(
+                        op.waveform.tolist(), repeat=True, vlen=2
+                    )
             else:
                 src_k = analog.sig_source_c(0, analog.GR_CONST_WAVE, 0, 0, mult_k)
             fg.connect(src_k, (u, k))
 
         # start the flowgraph once we are near the launch time
         # (start too soon and device buffers might not yet be flushed)
         # (start too late and device might not be able to start in time)
@@ -770,18 +787,26 @@
     )
 
     wavgroup = parser.add_argument_group(title="waveform")
     wavgroup.add_argument(
         "file",
         nargs="?",
         default=None,
-        help="""INI file specifying the waveform timing mode or complex64
+        help="""INI file specifying the waveform timing mode or --type
                 binary file giving the waveform directly.""",
     )
     wavgroup.add_argument(
+        "--type",
+        dest="dtype",
+        default=np.complex64,
+        type=np.dtype,
+        help="""String giving numpy dtype for the waveform binary file,
+                either `complex64` (default) or `int16`.""",
+    )
+    wavgroup.add_argument(
         "--iq_dir",
         default=None,
         help='''Directory with int16 binary IQ sweep files corresponding to the
                 mode INIT given with `file`. If None, defaults to
                 "`os.path.dirname(file)`/../iq"''',
     )
     wavgroup.add_argument(
@@ -1017,14 +1042,15 @@
 
     # ignore test_settings option if no starttime is set (starting right now)
     if op.starttime is None:
         op.test_settings = False
 
     options = {k: v for k, v in op._get_kwargs() if v is not None}
     fpath = options.pop("file")
+    dtype = options.pop("dtype")
     iq_dir = options.pop("iq_dir", None)
     tone = options.pop("tone", False)
     runopts = {
         k: options.pop(k)
         for k in list(options.keys())
         if k in ("starttime", "endtime", "duration", "period")
     }
@@ -1036,11 +1062,11 @@
         try:
             tm_dict = read_timing_mode_waveform(fpath, iq_dir=iq_dir)
             # use tm_dict as default options, overriding with command line
             options["waveform"] = tm_dict["waveform"]
             options.setdefault("samplerate", tm_dict["samplerate"])
             options.setdefault("centerfreqs", [tm_dict["center_freq"]])
         except ValueError:
-            options["waveform"] = np.fromfile(op.file, dtype=np.complex64)
+            options["waveform"] = np.fromfile(op.file, dtype=dtype)
 
     tx = Tx(**options)
     tx.run(**runopts)
```

### Comparing `digital_rf-2.6.8/examples/sounder/waveforms/code-l1000-b100-000000f.bin` & `digital_rf-2.6.9/examples/sounder/waveforms/code-l1000-b100-000000f.bin`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/examples/sounder/waveforms/code-l10000-b10-000000.bin` & `digital_rf-2.6.9/examples/sounder/waveforms/code-l10000-b10-000000.bin`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/examples/sounder/waveforms/create_waveform.py` & `digital_rf-2.6.9/examples/sounder/waveforms/create_waveform.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/gr_digital_rf/digital_rf_sink.py` & `digital_rf-2.6.9/gr_digital_rf/digital_rf_sink.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/gr_digital_rf/digital_rf_source.py` & `digital_rf-2.6.9/gr_digital_rf/digital_rf_source.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/gr_digital_rf/raster.py` & `digital_rf-2.6.9/gr_digital_rf/raster.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/gr_digital_rf/vector.py` & `digital_rf-2.6.9/gr_digital_rf/vector.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_digital_rf_channel_sink.block.yml` & `digital_rf-2.6.9/grc/gr_digital_rf_digital_rf_channel_sink.block.yml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_digital_rf_channel_sink.xml` & `digital_rf-2.6.9/grc/gr_digital_rf_digital_rf_channel_sink.xml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_digital_rf_channel_source.block.yml` & `digital_rf-2.6.9/grc/gr_digital_rf_digital_rf_channel_source.block.yml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_digital_rf_channel_source.xml` & `digital_rf-2.6.9/grc/gr_digital_rf_digital_rf_channel_source.xml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_digital_rf_sink.block.yml` & `digital_rf-2.6.9/grc/gr_digital_rf_digital_rf_sink.block.yml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_digital_rf_sink.xml` & `digital_rf-2.6.9/grc/gr_digital_rf_digital_rf_sink.xml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_digital_rf_source.block.yml` & `digital_rf-2.6.9/grc/gr_digital_rf_digital_rf_source.block.yml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_digital_rf_source.xml` & `digital_rf-2.6.9/grc/gr_digital_rf_digital_rf_source.xml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_raster_aggregate.block.yml` & `digital_rf-2.6.9/grc/gr_digital_rf_raster_aggregate.block.yml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_raster_aggregate.xml` & `digital_rf-2.6.9/grc/gr_digital_rf_raster_aggregate.xml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_raster_chunk.block.yml` & `digital_rf-2.6.9/grc/gr_digital_rf_raster_chunk.block.yml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_raster_chunk.xml` & `digital_rf-2.6.9/grc/gr_digital_rf_raster_chunk.xml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_raster_select.block.yml` & `digital_rf-2.6.9/grc/gr_digital_rf_raster_select.block.yml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_raster_select.xml` & `digital_rf-2.6.9/grc/gr_digital_rf_raster_select.xml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_raster_tag.block.yml` & `digital_rf-2.6.9/grc/gr_digital_rf_raster_tag.block.yml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_raster_tag.xml` & `digital_rf-2.6.9/grc/gr_digital_rf_raster_tag.xml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_vector_aggregate.block.yml` & `digital_rf-2.6.9/grc/gr_digital_rf_vector_aggregate.block.yml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/grc/gr_digital_rf_vector_aggregate.xml` & `digital_rf-2.6.9/grc/gr_digital_rf_vector_aggregate.xml`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/include/digital_rf.h` & `digital_rf-2.6.9/include/digital_rf.h`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/include/windows/inttypes.h` & `digital_rf-2.6.9/include/windows/inttypes.h`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/include/windows/stdint.h` & `digital_rf-2.6.9/include/windows/stdint.h`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/include/windows/wincompat.h` & `digital_rf-2.6.9/include/windows/wincompat.h`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/lib/py_rf_write_hdf5.c` & `digital_rf-2.6.9/lib/py_rf_write_hdf5.c`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/lib/rf_write_hdf5.c` & `digital_rf-2.6.9/lib/rf_write_hdf5.c`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/setup.py` & `digital_rf-2.6.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,15 @@
             libname_re = re.compile("(?P<libname>.*)")
         else:
             libname_re = re.compile("^lib(?P<libname>.*)")
         for k, lib in enumerate(self.libraries):
             if os.path.isabs(lib):
                 libdir, libfile = os.path.split(lib)
                 libfilename, _ = os.path.splitext(libfile)
-                libname = libname_re.sub("\g<libname>", libfilename)
+                libname = libname_re.sub(r"\g<libname>", libfilename)
                 # replace library entry with its name and add dir to path
                 self.libraries[k] = libname
                 if libdir not in self.library_dirs:
                     self.library_dirs.append(libdir)
 
     def run(self):
         self._add_build_settings()
```

### Comparing `digital_rf-2.6.8/tests/conftest.py` & `digital_rf-2.6.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/tests/test_digital_rf_hdf5.py` & `digital_rf-2.6.9/tests/test_digital_rf_hdf5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1097,15 +1097,15 @@
             with np.errstate(invalid="ignore"):
                 np.testing.assert_equal(
                     rdata, data.reshape((-1, num_subchannels))[bstart:bstop, 0]
                 )
 
         # check that we get all of the data if we read entire bounds
         data_dict = drf_reader.read(bounds[0], bounds[1], channel)
-        for (sstart, rdata) in data_dict.items():
+        for sstart, rdata in data_dict.items():
             bstart = sstart - bounds[0]
             bstop = sstart + len(rdata) - bounds[0]
             with np.errstate(invalid="ignore"):
                 np.testing.assert_equal(
                     rdata, data.reshape((-1, num_subchannels))[bstart:bstop, :]
                 )
```

### Comparing `digital_rf-2.6.8/tools/digital_metadata_archive.py` & `digital_rf-2.6.9/tools/digital_metadata_archive.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,14 @@
             shutil.rmtree(os.path.dirname(dest_archive), True)
 
         return count
 
 
 ### main begins here ###
 if __name__ == "__main__":
-
     # command line interface
     parser = argparse.ArgumentParser(
         description="digital_metadata_archive.py is a tool for archiving Digital Metadata.."
     )
     parser.add_argument(
         "--startDT",
         metavar="start datetime string",
```

### Comparing `digital_rf-2.6.8/tools/digital_rf_archive.py` & `digital_rf-2.6.9/tools/digital_rf_archive.py`

 * *Files 0% similar despite different names*

```diff
@@ -807,15 +807,14 @@
         subdirectory basenames, 2: list of metadata files in channel directory
         """
         return "nyi"
 
 
 ### main begins here ###
 if __name__ == "__main__":
-
     # command line interface
     parser = argparse.ArgumentParser(
         description="digital_rf_archive.py is a tool for archiving Digital RF data.."
     )
     parser.add_argument(
         "--startDT",
         metavar="start datetime string",
```

### Comparing `digital_rf-2.6.8/tools/digital_rf_upconvert.py` & `digital_rf-2.6.9/tools/digital_rf_upconvert.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/tools/digital_rf_update_properties.py` & `digital_rf-2.6.9/tools/digital_rf_update_properties.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/tools/drf_cross_sti.py` & `digital_rf-2.6.9/tools/drf_cross_sti.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         self.dio = []
         self.dmd = []
         self.channel = []
         self.sub_channel = []
         self.bounds = []
 
         for idx, p in enumerate(self.control.path):
-
             ch = self.control.channel[idx].split(":")
             self.channel.append(ch[0])
             self.sub_channel.append(int(ch[1]))
 
             # open digital RF path
             self.dio.append(drf.DigitalRFReader(p))
 
@@ -122,15 +121,14 @@
         """
 
         # initial plotting scales
         vmin = 0
         vmax = 0
 
         for fidx, xpair in enumerate(self.xlist):
-
             xidx, yidx = xpair
 
             if self.control.verbose:
                 print(("pair is : ", xidx, yidx))
 
             # sample rate
             xsr = self.dio[xidx].get_properties(self.channel[xidx])[
@@ -173,15 +171,14 @@
                     dtst0 - datetime.datetime(1970, 1, 1, tzinfo=pytz.utc)
                 ).total_seconds()
                 et0 = int(et0 * sr)
             else:
                 et0 = int(b[1])
 
             if self.control.verbose:
-
                 print(("start sample st0: ", st0))
                 print(("end sample et0: ", et0))
 
             blocks = self.control.bins * self.control.frames
 
             samples_per_stripe = (
                 self.control.num_fft
@@ -230,26 +227,24 @@
                     self.control.frames,
                     self.control.bins,
                     samples_per_stripe,
                     bin_stride,
                 )
 
             for p in np.arange(0, self.control.frames * 2, 2):
-
                 sti_csd_data_coherence = np.zeros(
                     [self.control.num_fft, self.control.bins], np.float
                 )
                 sti_csd_data_phase = np.zeros(
                     [self.control.num_fft, self.control.bins], np.float
                 )
 
                 sti_times = np.zeros([self.control.bins], np.complex128)
 
                 for b in np.arange(self.control.bins, dtype=np.int_):
-
                     if self.control.verbose:
                         print(
                             "read vector :",
                             self.channel,
                             start_sample,
                             samples_per_stripe,
                         )
```

### Comparing `digital_rf-2.6.8/tools/drf_plot.py` & `digital_rf-2.6.9/tools/drf_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,21 +108,19 @@
     as a pure average on the power level data.
     """
     if modulus:
         block = 0
         block_size = integration * modulus
         block_toffset = toffset
         while block < len(data) / block_size:
-
             vblock = data[block * block_size : block * block_size + modulus]
             pblock = (vblock * np.conjugate(vblock)).real
 
             # complete integration
             for idx in range(1, integration):
-
                 vblock = data[
                     block * block_size
                     + idx * modulus : block * block_size
                     + idx * modulus
                     + modulus
                 ]
                 pblock += (vblock * np.conjugate(vblock)).real
@@ -312,28 +310,26 @@
     win = np.blackman(bins)
 
     if modulus:
         block = 0
         block_size = integration * modulus
         block_toffset = toffset
         while block < len(data) / block_size:
-
             vblock = data[block * block_size : block * block_size + modulus]
             pblock, freq = matplotlib.mlab.psd(
                 vblock,
                 NFFT=bins,
                 Fs=sfreq,
                 detrend=dfn,
                 window=win,
                 scale_by_freq=False,
             )
 
             # complete integration
             for idx in range(1, integration):
-
                 vblock = data[
                     block * block_size
                     + idx * modulus : block * block_size
                     + idx * modulus
                     + modulus
                 ]
                 pblock_n, freq = matplotlib.mlab.psd(
@@ -473,29 +469,27 @@
     noverlap = int(bins * 0.9)
 
     if modulus:
         block = 0
         block_size = integration * modulus
         block_toffset = toffset
         while block < len(data) / block_size:
-
             vblock = data[(block * block_size) : (block * block_size + modulus)]
             pblock, freq, tm = matplotlib.mlab.specgram(
                 vblock,
                 NFFT=bins,
                 Fs=sfreq,
                 noverlap=noverlap,
                 detrend=dfn,
                 window=matplotlib.mlab.window_hanning,
                 scale_by_freq=False,
             )
 
             # complete integration
             for idx in range(1, integration):
-
                 vblock = data[
                     (block * block_size + idx * modulus) : (
                         block * block_size + idx * modulus + modulus
                     )
                 ]
                 pblock_n, freq, tm = matplotlib.mlab.specgram(
                     vblock,
@@ -607,21 +601,19 @@
 
         rti_bins = len(data) // block_size
 
         RTIdata = np.zeros([modulus, rti_bins], np.complex64)
         RTItimes = np.zeros([rti_bins])
 
         while block < rti_bins:
-
             vblock = data[block * block_size : block * block_size + modulus]
             pblock = vblock * np.conjugate(vblock)
 
             # complete integration
             for idx in range(1, integration):
-
                 vblock = data[
                     block * block_size
                     + idx * modulus : block * block_size
                     + idx * modulus
                     + modulus
                 ]
                 pblock += vblock * np.conjugate(vblock)
@@ -669,15 +661,14 @@
 
     yield rti_plot(
         RTIdata.real, extent, tick_locs, tick_labels, log_scale, zscale, title
     )
 
 
 def rti_plot(data, extent, tick_locs, tick_labels, log_scale, zscale, title):
-
     # set to log scaling
     if log_scale:
         RTId = 10.0 * np.log10(data + 1e-12)
     else:
         RTId = data
 
     zscale_low, zscale_high = zscale
@@ -746,28 +737,26 @@
 
         sti_bins = len(data) // block_size
 
         STIdata = np.zeros([bins, sti_bins], np.complex64)
         STItimes = np.zeros([sti_bins])
 
         while block < sti_bins:
-
             vblock = data[block * block_size : block * block_size + modulus]
             pblock, freq = matplotlib.mlab.psd(
                 vblock,
                 NFFT=bins,
                 Fs=sfreq,
                 detrend=dfn,
                 window=matplotlib.mlab.window_hanning,
                 scale_by_freq=False,
             )
 
             # complete integration
             for idx in range(1, integration):
-
                 vblock = data[
                     block * block_size
                     + idx * modulus : block * block_size
                     + idx * modulus
                     + modulus
                 ]
                 pblock_n, freq = matplotlib.mlab.psd(
@@ -818,15 +807,14 @@
 
     yield sti_plot(
         STIdata.real, freq, extent, tick_locs, tick_labels, log_scale, zscale, title
     )
 
 
 def sti_plot(data, freq, extent, tick_locs, tick_labels, log_scale, zscale, title):
-
     pss = data
 
     # set to log scaling
     if log_scale:
         STId = 10.0 * np.log10(pss + 1e-12)
     else:
         STId = pss
@@ -905,15 +893,14 @@
 
     if len(vec) < ell:
         raise ValueError("hex string too short")
     return vec[len(vec) - ell :]
 
 
 def apply_msl_filter(data, msl_code_length, msl_baud_length):
-
     code_table = {
         2: [0, 1],  # barker codes
         3: [0, 0, 1],
         4: [0, 1, 0, 0],
         5: [0, 0, 0, 1, 0],
         7: [0, 0, 0, 1, 1, 0, 1],
         11: [0, 0, 0, 1, 1, 1, 0, 1, 1, 0, 1],
@@ -1099,15 +1086,14 @@
     try:
         opts, args = getopt.getopt(sys.argv[1:], "hi:p:c:o:r:b:z:m:t:a:ld:s:")
     except:
         usage()
         sys.exit()
 
     for opt, val in opts:
-
         if opt in ("-h"):
             usage()
             sys.exit()
         elif opt in ("-i"):
             input_files.append(val)
         elif opt in ("-s"):
             plot_file = val
```

### Comparing `digital_rf-2.6.8/tools/drf_sound.py` & `digital_rf-2.6.9/tools/drf_sound.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
                 dtst0 - datetime.datetime(1970, 1, 1, tzinfo=pytz.utc)
             ).total_seconds()
             et0 = int(et0 * sr)
         else:
             et0 = int(bound[1])
 
         if self.control.verbose:
-
             print("start sample st0: ", st0)
             print("end sample et0: ", et0)
 
         decimate = int(self.control.timedilation * sr / self.control.audiosampling)
         blocks = self.control.blocks
 
         dsamps = int(2**15)
@@ -119,17 +118,15 @@
                 blocks,
                 reads_per_block,
                 samples_per_stripe,
                 end=" ",
             )
 
         for iblock in range(blocks):
-
             for iread in range(reads_per_block):
-
                 if self.control.verbose:
                     print(
                         "read vector :", self.channel, start_sample, samples_per_stripe
                     )
 
                 data = self.dio.read_vector(
                     start_sample, samples_per_stripe, self.channel, self.sub_channel
```

### Comparing `digital_rf-2.6.8/tools/drf_sti.py` & `digital_rf-2.6.9/tools/drf_sti.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,14 @@
                 dtst0 - datetime.datetime(1970, 1, 1, tzinfo=pytz.utc)
             ).total_seconds()
             et0 = int(et0 * self.sr)
         else:
             et0 = int(b[1])
 
         if self.opt.verbose:
-
             print("start sample st0: {0}".format(st0))
             print("end sample et0: {0}".format(et0))
 
         blocks = self.opt.length * self.opt.frames
 
         samples_per_stripe = (
             self.opt.fft_bins * self.opt.integration * self.opt.decimation
@@ -210,15 +209,14 @@
             )
 
         for p in np.arange(self.opt.frames):
             sti_psd_data = np.zeros([self.opt.fft_bins, self.opt.length], np.float64)
             sti_times = np.zeros([self.opt.length], np.complex128)
 
             for b in np.arange(self.opt.length, dtype=np.int_):
-
                 if self.opt.verbose:
                     print(
                         "read vector : {0} {1} {2}".format(
                             self.channels, start_sample, samples_per_stripe
                         )
                     )
 
@@ -445,15 +443,14 @@
             matplotlib.pyplot.savefig(fname + ext)
         if self.opt.appear or not self.opt.outname:
             print("Show plot")
             matplotlib.pyplot.show()
 
 
 def parse_command_line():
-
     scriptname = os.path.basename(sys.argv[0])
 
     formatter = argparse.RawDescriptionHelpFormatter(scriptname)
     width = formatter._width
 
     title = "drf_sti"
     copyright = "Copyright (c) 2022 Massachusetts Institute of Technology"
```

### Comparing `digital_rf-2.6.8/tools/thor.py` & `digital_rf-2.6.9/tools/thor.py`

 * *Files identical despite different names*

### Comparing `digital_rf-2.6.8/tools/thorosmo.py` & `digital_rf-2.6.9/tools/thorosmo.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,15 +610,14 @@
         if op.time_sync:
             # wait until time 0.2 to 0.5 past full second, then latch
             # we have to trust NTP to be 0.2 s accurate
             while tt - math.floor(tt) < 0.2 or tt - math.floor(tt) > 0.3:
                 time.sleep(0.01)
                 tt = time.time()
             if op.verbose:
-
                 print("Latching at " + str(tt))
             # waits for the next pps to happen
             # (at time math.ceil(tt))
             # then sets the time for the subsequent pps
             # (at time math.ceil(tt) + 1.0)
             for ichan in osmo_dict.keys():
                 rtl_chan = osmo_dict[ichan]
@@ -1334,15 +1333,14 @@
                 (after any scaling) to the maximum integer value.
                 (default: None)""",
     )
     return parser
 
 
 def _add_drf_group(parser):
-
     drfgroup = parser.add_argument_group(title="digital_rf")
     drfgroup.add_argument(
         "-n",
         "--file_cadence_ms",
         dest="file_cadence_ms",
         type=evalint,
         help="""Number of milliseconds of data per file.
```

### Comparing `digital_rf-2.6.8/tools/thorpluto.py` & `digital_rf-2.6.9/tools/thorpluto.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,15 +152,15 @@
             realtime=False,
             test_settings=True,
             # receiver ch. group (num: matching channels from mboards)
             centerfreqs=[2.4e9],
             quad_track=[False],
             rfdc_track=[False],
             bbdc_track=[False],
-            gains=[73],
+            gains=[62],
             bandwidths=[20e6],
             # output channel group (num: len of channel_names)
             channel_names=["ch0"],
             channels=[None],
             ch_samplerates=[None],
             ch_centerfreqs=[False],
             ch_scalings=[1.0],
@@ -268,15 +268,15 @@
             setattr(op, mb_arg, mbval)
 
         # get number of receiver channels by total number of subdevices over
         # all mainboards
         op.mboards_bychan = []
         op.mboardnum_bychan = []
         # add a default mboard if the argument was empty
-        op.mboards = op.mboards if op.mboards else [""]
+        op.mboards = op.mboards if op.mboards else [iio.get_pluto_uri()]
         for mbnum, mb in enumerate(op.mboards):
             op.mboards_bychan.extend([mb])
             op.mboardnum_bychan.extend([mbnum])
         op.nrchs = op.nmboards
         # repeat receiver channel arguments as necessary
         for rch_arg in (
             "bandwidths",
@@ -409,38 +409,27 @@
         # sup_gs = [0.0, 0.9, 1.4, 2.7, 3.7, 7.7, 8.7, 12.5, 14.4, 15.7, 16.6, 19.7,
         #           20.7, 22.9, 25.4, 28.0, 29.7, 32.8, 33.8, 36.4, 37.2, 38.6, 40.2,
         #           42.1, 43.4, 43.9, 44.5, 48.0, 49.6]
         # List of possible sample rates for RTL dongle. Here for reference for now.
         # sup_sr = [1.024e6, 1.4e6, 1.8e6, 1.92e6, 2.048e6, 2.4e6, 2.56e6]
 
         for mnum in range(op.nmboards):
-            # HACK two questions
-            # 1 Do I need to use the pluto source or you use the iio device source?
-            # ans: Can use fmcomms2_source
-            """make(std::string const & uri, unsigned long long frequency,
-            unsigned long samplerate, unsigned long bandwidth, bool ch1_en,
-            bool ch2_en, bool ch3_en, bool ch4_en, unsigned long buffer_size,
-            bool quadrature, bool rfdc, bool bbdc, char const * gain1,
-            double gain1_value, char const * gain2, double gain2_value,
-            char const * rf_port_select, char const * filter, bool auto_filter=True)
-            """
-            pluto_sources[mnum] = iio.pluto_source(
-                uri=op.mboard_strs[mnum],
-                frequency=int(op.centerfreqs[mnum]),
-                samplerate=int(op.samplerate),
-                bandwidth=int(op.bandwidths[mnum]),
-                buffer_size=0x8000,
-                quadrature=op.quad_track[mnum],
-                rfdc=op.rfdc_track[mnum],
-                bbdc=op.bbdc_track[mnum],
-                gain="manual" if op.gains[mnum] >= 0 else "fast_attack",
-                gain_value=op.gains[mnum],
-                filter="",
-                auto_filter=True,
+            # Use the fmcomms 2 source does only fc32 over the wire data.
+            pluto_sources[mnum] = iio.fmcomms2_source_fc32(
+                op.mboard_strs[mnum], [True, True], 32768
             )
+            pluto_sources[mnum].set_len_tag_key("packet_len")
+            pluto_sources[mnum].set_frequency(int(op.centerfreqs[mnum]))
+            pluto_sources[mnum].set_samplerate(int(op.samplerate))
+            pluto_sources[mnum].set_gain_mode(0, "manual")
+            pluto_sources[mnum].set_gain(0, op.gains[mnum])
+            pluto_sources[mnum].set_quadrature(op.quad_track[mnum])
+            pluto_sources[mnum].set_rfdc(op.rfdc_track[mnum])
+            pluto_sources[mnum].set_bbdc(op.bbdc_track[mnum])
+            pluto_sources[mnum].set_filter_params("Auto", "", 0, 0)
 
             # set master clock rate
             # HACK can you set clock rates
             # clock_rate = op.clock_rates[mnum]
             # if clock_rate is not None:
             #     osmo_sources[mnum].set_clock_rate(clock_rate, 0)
             # op.clock_rates[mnum] = osmo_sources[mnum].get_clock_rate()
@@ -1243,15 +1232,14 @@
                 (after any scaling) to the maximum integer value.
                 (default: None)""",
     )
     return parser
 
 
 def _add_drf_group(parser):
-
     drfgroup = parser.add_argument_group(title="digital_rf")
     drfgroup.add_argument(
         "-n",
         "--file_cadence_ms",
         dest="file_cadence_ms",
         type=evalint,
         help="""Number of milliseconds of data per file.
```

### Comparing `digital_rf-2.6.8/tools/uhdtodrf.py` & `digital_rf-2.6.9/tools/uhdtodrf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1091,15 +1091,14 @@
                 target=self.buff_func, args=(stream, radfifo, end_rec, start_sample)
             )
             read_th.start()
             read_th.setName("Read Thread")
             # now that we're ready to accept samples, send the start streaming command
             stream.issue_stream_cmd(stream_cmd)
             while not end_rec.is_set():
-
                 if et is not None:
                     stop_bool = pytz.utc.localize(datetime.utcnow()) >= et - timedelta(
                         seconds=1
                     )
                     if stop_bool:
                         end_rec.set()
 
@@ -1134,15 +1133,14 @@
         # Handle the error codes
 
         except KeyboardInterrupt:
             end_rec.set()
             time.sleep(1)
 
         finally:
-
             while write_threads or proc_threads or (not radfifo.empty()):
                 if not radfifo.empty():
                     d1 = radfifo.get()
                     tmp = self.bufflist[d1[0]][:, : self.pntlist[d1[0]]]
                     cur_pt = threading.Thread(
                         target=self.procsamples, args=(write_fifo, tmp, d1[1])
                     )
@@ -1273,15 +1271,14 @@
                     samp_num += bpnt
                     self.pntlist[b] = m_overlap
                     self.act_buff = b
                     a = self.act_buff
                     bpnt = self.pntlist[a]
 
                 if num_rx_dropped:
-
                     end_pnt = min(self.bufflen, bpnt + num_rx_dropped)
                     self.bufflist[a][:, bpnt:end_pnt] = np.nan
                     self.pntlist[a] += num_rx_dropped
                     num_rx_dropped = 0
 
                 beg_samp = max(0, start_sample - rec_samp)
                 a = self.act_buff
@@ -1398,15 +1395,14 @@
         List of digital rf writers for each channel.
 
     data_samples : array, shape (nchan, nsample)
         Array that will be saved.
 
     """
     try:
-
         for i_num, iobj in enumerate(drfObj):
             iobj.rf_write(data_samples[i_num])
     except Exception as error:
         print("write function caught this error: " + repr(error))
 
 
 def evalint(s):
@@ -2021,15 +2017,14 @@
 
     # parser.set_defaults(func=_run_thor)
 
     return parser
 
 
 def _ops_setup(args):
-
     if args.datadir is None:
         args.datadir = args.outdir
     del args.outdir
 
     # handle deprecated decimation argument, converting it to sample rate
     if args.decimations is not None:
         if args.samplerate is None:
@@ -2101,15 +2096,14 @@
         for k in list(options.keys())
         if k in ("starttime", "endtime", "duration", "period")
     }
     return options, runopts
 
 
 if __name__ == "__main__":
-
     parser = _build_parser(argparse.ArgumentParser)
     args = parser.parse_args()
     options, runopts = _ops_setup(args)
     import signal
 
     # handle SIGTERM (getting killed) gracefully by calling sys.exit
     def sigterm_handler(signal, frame):
```

### Comparing `digital_rf-2.6.8/tools/verify_digital_rf_upconvert.py` & `digital_rf-2.6.9/tools/verify_digital_rf_upconvert.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from digital_rf import digital_rf_deprecated_hdf5  # for reading old formatter
 
 read_len = 1000000  # default read len
 
 
 ### main begins here ###
 if __name__ == "__main__":
-
     # command line interface
     parser = argparse.ArgumentParser(
         description="verify_digital_rf_upconvert will test if a digital rf 2 subdirectory matches sample for sample a digital rf 1 subdirectory. Prints True or False"
     )
     parser.add_argument(
         "--drf2",
         metavar="drf2Dir",
```

### Comparing `digital_rf-2.6.8/versioneer.py` & `digital_rf-2.6.9/versioneer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,63 @@
-# Version: 0.18
+# Version: 0.29
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
-* https://github.com/warner/python-versioneer
+* https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain
-* Compatible With: python2.6, 2.7, 3.2, 3.3, 3.4, 3.5, 3.6, and pypy
-* [![Latest Version]
-(https://pypip.in/version/versioneer/badge.svg?style=flat)
-](https://pypi.python.org/pypi/versioneer/)
-* [![Build Status]
-(https://travis-ci.org/warner/python-versioneer.png?branch=master)
-](https://travis-ci.org/warner/python-versioneer)
+* License: Public Domain (Unlicense)
+* Compatible with: Python 3.7, 3.8, 3.9, 3.10, 3.11 and pypy3
+* [![Latest Version][pypi-image]][pypi-url]
+* [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in distutils-based
+This is a tool for managing a recorded version number in setuptools-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
-* `pip install versioneer` to somewhere to your $PATH
-* add a `[versioneer]` section to your setup.cfg (see below)
-* run `versioneer install` in your source tree, commit the results
+Versioneer provides two installation modes. The "classic" vendored mode installs
+a copy of versioneer into your repository. The experimental build-time dependency mode
+is intended to allow you to skip this step and simplify the process of upgrading.
+
+### Vendored mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+   * Note that you will need to add `tomli; python_version < "3.11"` to your
+     build-time dependencies if you use `pyproject.toml`
+* run `versioneer install --vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
+
+### Build-time dependency mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
+  to the `requires` key of the `build-system` table in `pyproject.toml`:
+  ```toml
+  [build-system]
+  requires = ["setuptools", "versioneer[toml]"]
+  build-backend = "setuptools.build_meta"
+  ```
+* run `versioneer install --no-vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -56,15 +81,15 @@
 unreleased software (between tags), the version identifier should provide
 enough information to help developers recreate the same tree, while also
 giving them an idea of roughly how old the tree is (after version 1.2, before
 version 1.3). Many VCS systems can report a description that captures this,
 for example `git describe --tags --dirty --always` reports things like
 "0.7-1-g574ab98-dirty" to indicate that the checkout is one revision past the
 0.7 tag, has a unique revision id of "574ab98", and is "dirty" (it has
-uncommitted changes.
+uncommitted changes).
 
 The version identifier is used for multiple purposes:
 
 * to allow the module to self-identify its version: `myproject.__version__`
 * to choose a name and prefix for a 'setup.py sdist' tarball
 
 ## Theory of Operation
@@ -161,45 +186,45 @@
 display the full contents of `get_versions()` (including the `error` string,
 which may help identify what went wrong).
 
 ## Known Limitations
 
 Some situations are known to cause problems for Versioneer. This details the
 most significant ones. More can be found on Github
-[issues page](https://github.com/warner/python-versioneer/issues).
+[issues page](https://github.com/python-versioneer/python-versioneer/issues).
 
 ### Subprojects
 
 Versioneer has limited support for source trees in which `setup.py` is not in
 the root directory (e.g. `setup.py` and `.git/` are *not* siblings). The are
 two common reasons why `setup.py` might not be in the root:
 
 * Source trees which contain multiple subprojects, such as
   [Buildbot](https://github.com/buildbot/buildbot), which contains both
   "master" and "slave" subprojects, each with their own `setup.py`,
   `setup.cfg`, and `tox.ini`. Projects like these produce multiple PyPI
   distributions (and upload multiple independently-installable tarballs).
 * Source trees whose main purpose is to contain a C library, but which also
-  provide bindings to Python (and perhaps other langauges) in subdirectories.
+  provide bindings to Python (and perhaps other languages) in subdirectories.
 
 Versioneer will look for `.git` in parent directories, and most operations
 should get the right version string. However `pip` and `setuptools` have bugs
 and implementation details which frequently cause `pip install .` from a
 subproject directory to fail to find a correct version string (so it usually
 defaults to `0+unknown`).
 
 `pip install --editable .` should work correctly. `setup.py install` might
 work too.
 
 Pip-8.1.1 is known to have this problem, but hopefully it will get fixed in
 some later version.
 
-[Bug #38](https://github.com/warner/python-versioneer/issues/38) is tracking
+[Bug #38](https://github.com/python-versioneer/python-versioneer/issues/38) is tracking
 this issue. The discussion in
-[PR #61](https://github.com/warner/python-versioneer/pull/61) describes the
+[PR #61](https://github.com/python-versioneer/python-versioneer/pull/61) describes the
 issue from the Versioneer side in more detail.
 [pip PR#3176](https://github.com/pypa/pip/pull/3176) and
 [pip PR#3615](https://github.com/pypa/pip/pull/3615) contain work to improve
 pip to let Versioneer work correctly.
 
 Versioneer-0.16 and earlier only looked for a `.git` directory next to the
 `setup.cfg`, so subprojects were completely unsupported with those releases.
@@ -219,39 +244,28 @@
 `pkg_resources.DistributionNotFound` errors when running the entrypoint
 script, which must be resolved by re-installing the package. This happens
 when the install happens with one version, then the egg_info data is
 regenerated while a different version is checked out. Many setup.py commands
 cause egg_info to be rebuilt (including `sdist`, `wheel`, and installing into
 a different virtualenv), so this can be surprising.
 
-[Bug #83](https://github.com/warner/python-versioneer/issues/83) describes
+[Bug #83](https://github.com/python-versioneer/python-versioneer/issues/83) describes
 this one, but upgrading to a newer version of setuptools should probably
 resolve it.
 
-### Unicode version strings
-
-While Versioneer works (and is continually tested) with both Python 2 and
-Python 3, it is not entirely consistent with bytes-vs-unicode distinctions.
-Newer releases probably generate unicode version strings on py2. It's not
-clear that this is wrong, but it may be surprising for applications when then
-write these strings to a network connection or include them in bytes-oriented
-APIs like cryptographic checksums.
-
-[Bug #71](https://github.com/warner/python-versioneer/issues/71) investigates
-this question.
-
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install` in your source tree, to replace
+* edit `setup.cfg` and `pyproject.toml`, if necessary,
+  to include any new configuration settings indicated by the release notes.
+  See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install --[no-]vendor` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -260,58 +274,102 @@
 will take a VCS name as an argument, and will construct a version of
 `versioneer.py` that is specific to the given VCS. It might also take the
 configuration arguments that are currently provided manually during
 installation by editing setup.py . Alternatively, it might go the other
 direction and include code from all supported VCS systems, reducing the
 number of intermediate scripts.
 
+## Similar projects
+
+* [setuptools_scm](https://github.com/pypa/setuptools_scm/) - a non-vendored build-time
+  dependency
+* [minver](https://github.com/jbweston/miniver) - a lightweight reimplementation of
+  versioneer
+* [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
+  plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
+Specifically, both are released under the "Unlicense", as described in
+https://unlicense.org/.
 
-"""
+[pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
+[pypi-url]: https://pypi.python.org/pypi/versioneer/
+[travis-image]:
+https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
+[travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
-from __future__ import print_function
+"""
+# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
+# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
+# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
+# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
+# pylint:disable=attribute-defined-outside-init,too-many-arguments
 
-try:
-    import configparser
-except ImportError:
-    import ConfigParser as configparser
+import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
+from pathlib import Path
+from typing import Any, Callable, cast, Dict, List, Optional, Tuple, Union
+from typing import NoReturn
+import functools
+
+have_tomllib = True
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    try:
+        import tomli as tomllib
+    except ImportError:
+        have_tomllib = False
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    versionfile_source: str
+    versionfile_build: Optional[str]
+    parentdir_prefix: Optional[str]
+    verbose: Optional[bool]
+
 
-def get_root():
+def get_root() -> str:
     """Get the project root directory.
 
     We require that all commands are run from the project root, i.e. the
     directory that contains setup.py, setup.cfg, and versioneer.py .
     """
     root = os.path.realpath(os.path.abspath(os.getcwd()))
     setup_py = os.path.join(root, "setup.py")
+    pyproject_toml = os.path.join(root, "pyproject.toml")
     versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py)
+        or os.path.exists(pyproject_toml)
+        or os.path.exists(versioneer_py)
+    ):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
+        pyproject_toml = os.path.join(root, "pyproject.toml")
         versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py)
+        or os.path.exists(pyproject_toml)
+        or os.path.exists(versioneer_py)
+    ):
         err = (
             "Versioneer was unable to run the project root directory. "
             "Versioneer requires setup.py to be executed from "
             "its immediate directory (like 'python setup.py COMMAND'), "
             "or in a way that lets it use sys.argv[0] to find the root "
             "(like 'python path/to/setup.py COMMAND')."
         )
@@ -319,140 +377,172 @@
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
-        me = os.path.realpath(os.path.abspath(__file__))
-        me_dir = os.path.normcase(os.path.splitext(me)[0])
+        my_path = os.path.realpath(os.path.abspath(__file__))
+        me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir:
+        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
             print(
                 "Warning: build in %s is using versioneer.py from %s"
-                % (os.path.dirname(me), versioneer_py)
+                % (os.path.dirname(my_path), versioneer_py)
             )
     except NameError:
         pass
     return root
 
 
-def get_config_from_root(root):
+def get_config_from_root(root: str) -> VersioneerConfig:
     """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise EnvironmentError (if setup.cfg is missing), or
+    # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
-    with open(setup_cfg, "r") as f:
-        parser.readfp(f)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
-
-    def get(parser, name):
-        if parser.has_option("versioneer", name):
-            return parser.get("versioneer", name)
-        return None
+    root_pth = Path(root)
+    pyproject_toml = root_pth / "pyproject.toml"
+    setup_cfg = root_pth / "setup.cfg"
+    section: Union[Dict[str, Any], configparser.SectionProxy, None] = None
+    if pyproject_toml.exists() and have_tomllib:
+        try:
+            with open(pyproject_toml, "rb") as fobj:
+                pp = tomllib.load(fobj)
+            section = pp["tool"]["versioneer"]
+        except (tomllib.TOMLDecodeError, KeyError) as e:
+            print(f"Failed to load config from {pyproject_toml}: {e}")
+            print("Try to load it from setup.cfg")
+    if not section:
+        parser = configparser.ConfigParser()
+        with open(setup_cfg) as cfg_file:
+            parser.read_file(cfg_file)
+        parser.get("versioneer", "VCS")  # raise error if missing
+
+        section = parser["versioneer"]
+
+    # `cast`` really shouldn't be used, but its simplest for the
+    # common VersioneerConfig users at the moment. We verify against
+    # `None` values elsewhere where it matters
 
     cfg = VersioneerConfig()
-    cfg.VCS = VCS
-    cfg.style = get(parser, "style") or ""
-    cfg.versionfile_source = get(parser, "versionfile_source")
-    cfg.versionfile_build = get(parser, "versionfile_build")
-    cfg.tag_prefix = get(parser, "tag_prefix")
-    if cfg.tag_prefix in ("''", '""'):
+    cfg.VCS = section["VCS"]
+    cfg.style = section.get("style", "")
+    cfg.versionfile_source = cast(str, section.get("versionfile_source"))
+    cfg.versionfile_build = section.get("versionfile_build")
+    cfg.tag_prefix = cast(str, section.get("tag_prefix"))
+    if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
-    cfg.parentdir_prefix = get(parser, "parentdir_prefix")
-    cfg.verbose = get(parser, "verbose")
+    cfg.parentdir_prefix = section.get("parentdir_prefix")
+    if isinstance(section, configparser.SectionProxy):
+        # Make sure configparser translates to bool
+        cfg.verbose = section.getboolean("verbose")
+    else:
+        cfg.verbose = section.get("verbose")
+
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
+    """Create decorator to mark a method as the handler of a VCS."""
 
-    def decorate(f):
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
-        if vcs not in HANDLERS:
-            HANDLERS[vcs] = {}
-        HANDLERS[vcs][method] = f
+        HANDLERS.setdefault(vcs, {})[method] = f
         return f
 
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen(
-                [c] + args,
+            process = subprocess.Popen(
+                [command] + args,
                 cwd=cwd,
                 env=env,
                 stdout=subprocess.PIPE,
                 stderr=(subprocess.PIPE if hide_stderr else None),
+                **popen_kwargs,
             )
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %s" % (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
 LONG_VERSION_PY[
     "git"
-] = '''
+] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.18 (https://github.com/warner/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.29
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
+from typing import Any, Callable, Dict, List, Optional, Tuple
+import functools
 
 
-def get_keywords():
+def get_keywords() -> Dict[str, str]:
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
     # get_keywords().
     git_refnames = "%(DOLLAR)sFormat:%%d%(DOLLAR)s"
     git_full = "%(DOLLAR)sFormat:%%H%(DOLLAR)s"
@@ -460,16 +550,23 @@
     keywords = {"refnames": git_refnames, "full": git_full, "date": git_date}
     return keywords
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    parentdir_prefix: str
+    versionfile_source: str
+    verbose: bool
 
-def get_config():
+
+def get_config() -> VersioneerConfig:
     """Create, populate and return the VersioneerConfig() object."""
     # these strings are filled in when 'setup.py versioneer' creates
     # _version.py
     cfg = VersioneerConfig()
     cfg.VCS = "git"
     cfg.style = "%(STYLE)s"
     cfg.tag_prefix = "%(TAG_PREFIX)s"
@@ -479,161 +576,187 @@
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
-    def decorate(f):
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
+    """Create decorator to mark a method as the handler of a VCS."""
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %%s" %% (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %%s (error)" %% dispcmd)
             print("stdout was %%s" %% stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %%s but none started with prefix %%s" %%
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %%d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%%s', no digits" %% ",".join(refs - tags))
     if verbose:
         print("likely tags: %%s" %% ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %%s" %% r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -641,52 +764,97 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str,
+    root: str,
+    verbose: bool,
+    runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%%s*" %% tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -695,15 +863,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -720,34 +888,35 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -764,31 +933,79 @@
         rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%%d" %% pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%%d" %% (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%%d" %% pieces["distance"]
+        rendered = "0.post0.dev%%d" %% pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -807,20 +1024,49 @@
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%%d" %% pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%%s" %% pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%%d" %% pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%%s" %% pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%%d" %% pieces["distance"]
             if pieces["dirty"]:
@@ -829,15 +1075,15 @@
         # exception #1
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -849,15 +1095,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -869,47 +1115,51 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
                 "error": pieces["error"],
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%%s'" %% style)
 
     return {"version": rendered, "full-revisionid": pieces["long"],
             "dirty": pieces["dirty"], "error": None,
             "date": pieces.get("date")}
 
 
-def get_versions():
+def get_versions() -> Dict[str, Any]:
     """Get version information or return default if unable to do so."""
     # I am in _version.py, which lives at ROOT/VERSIONFILE_SOURCE. If we have
     # __file__, we can work backwards from there to the root. Some
     # py2exe/bbfreeze/non-CPython implementations don't do __file__, in which
     # case we can only use expanded keywords.
 
     cfg = get_config()
@@ -922,15 +1172,15 @@
         pass
 
     try:
         root = os.path.realpath(__file__)
         # versionfile_source is the relative path from the top of the source
         # tree (where the .git directory might live) to this file. Invert
         # this to find the root from __file__.
-        for i in cfg.versionfile_source.split('/'):
+        for _ in cfg.versionfile_source.split('/'):
             root = os.path.dirname(root)
     except NameError:
         return {"version": "0+unknown", "full-revisionid": None,
                 "dirty": None,
                 "error": "unable to find root of source tree",
                 "date": None}
 
@@ -949,83 +1199,95 @@
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None,
             "error": "unable to compute version", "date": None}
 '''
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG) :] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG) :] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r"\d", r)])
+        tags = {r for r in refs if re.search(r"\d", r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix) :]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r"\d", r):
+                continue
             if verbose:
                 print("picking %s" % r)
             return {
                 "version": r,
                 "full-revisionid": keywords["full"].strip(),
                 "dirty": False,
                 "error": None,
@@ -1040,60 +1302,101 @@
         "dirty": False,
         "error": "no suitable tags",
         "date": None,
     }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str, root: str, verbose: bool, runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(
+    describe_out, rc = runner(
         GITS,
         [
             "describe",
             "--tags",
             "--dirty",
             "--always",
             "--long",
             "--match",
-            "%s*" % tag_prefix,
+            f"{tag_prefix}[[:digit:]]*",
         ],
         cwd=root,
     )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"], cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -1102,15 +1405,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
@@ -1128,97 +1431,101 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[
-        0
-    ].strip()
+    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(manifest_in, versionfile_source, ipy):
+def do_vcs_install(versionfile_source: str, ipy: Optional[str]) -> None:
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [manifest_in, versionfile_source]
+    files = [versionfile_source]
     if ipy:
         files.append(ipy)
-    try:
-        me = __file__
-        if me.endswith(".pyc") or me.endswith(".pyo"):
-            me = os.path.splitext(me)[0] + ".py"
-        versioneer_file = os.path.relpath(me)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
+    if "VERSIONEER_PEP518" not in globals():
+        try:
+            my_path = __file__
+            if my_path.endswith((".pyc", ".pyo")):
+                my_path = os.path.splitext(my_path)[0] + ".py"
+            versioneer_file = os.path.relpath(my_path)
+        except NameError:
+            versioneer_file = "versioneer.py"
+        files.append(versioneer_file)
     present = False
     try:
-        f = open(".gitattributes", "r")
-        for line in f.readlines():
-            if line.strip().startswith(versionfile_source):
-                if "export-subst" in line.strip().split()[1:]:
-                    present = True
-        f.close()
-    except EnvironmentError:
+        with open(".gitattributes", "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith(versionfile_source):
+                    if "export-subst" in line.strip().split()[1:]:
+                        present = True
+                        break
+    except OSError:
         pass
     if not present:
-        f = open(".gitattributes", "a+")
-        f.write("%s export-subst\n" % versionfile_source)
-        f.close()
+        with open(".gitattributes", "a+") as fobj:
+            fobj.write(f"{versionfile_source} export-subst\n")
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {
                 "version": dirname[len(parentdir_prefix) :],
                 "full-revisionid": None,
                 "dirty": False,
                 "error": None,
                 "date": None,
             }
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print(
             "Tried directories %s but none started with prefix %s"
             % (str(rootdirs), parentdir_prefix)
         )
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.18) from
+# This file was generated by 'versioneer.py' (0.29) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1227,51 +1534,50 @@
 
 
 def get_versions():
     return json.loads(version_json)
 """
 
 
-def versions_from_file(filename):
+def versions_from_file(filename: str) -> Dict[str, Any]:
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except EnvironmentError:
+    except OSError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(
         r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
     )
     if not mo:
         mo = re.search(
             r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
         )
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
-def write_to_version_file(filename, versions):
+def write_to_version_file(filename: str, versions: Dict[str, Any]) -> None:
     """Write the given version number to the given _version.py file."""
-    os.unlink(filename)
     contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -1287,31 +1593,78 @@
         # exception #1
         rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%d" % pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%d" % (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%d" % pieces["distance"]
+        rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -1330,20 +1683,49 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%d" % pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%s" % pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%d" % pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%s" % pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%d" % pieces["distance"]
             if pieces["dirty"]:
@@ -1352,15 +1734,15 @@
         # exception #1
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -1372,15 +1754,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -1392,15 +1774,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {
             "version": "unknown",
             "full-revisionid": pieces.get("long"),
             "dirty": None,
             "error": pieces["error"],
@@ -1408,18 +1790,22 @@
         }
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
@@ -1434,30 +1820,30 @@
     }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
-def get_versions(verbose=False):
+def get_versions(verbose: bool = False) -> Dict[str, Any]:
     """Get the project version from whatever source is available.
 
     Returns dict with two keys: 'version' and 'full'.
     """
     if "versioneer" in sys.modules:
         # see the discussion in cmdclass.py:get_cmdclass()
         del sys.modules["versioneer"]
 
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
-    verbose = verbose or cfg.verbose
+    verbose = verbose or bool(cfg.verbose)  # `bool()` used to avoid `None`
     assert (
         cfg.versionfile_source is not None
     ), "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
@@ -1515,111 +1901,156 @@
         "full-revisionid": None,
         "dirty": None,
         "error": "unable to compute version",
         "date": None,
     }
 
 
-def get_version():
+def get_version() -> str:
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
-def get_cmdclass():
-    """Get the custom setuptools/distutils subclasses used by Versioneer."""
+def get_cmdclass(cmdclass: Optional[Dict[str, Any]] = None):
+    """Get the custom setuptools subclasses used by Versioneer.
+
+    If the package uses a different cmdclass (e.g. one from numpy), it
+    should be provide as an argument.
+    """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
         # 'easy_install .'), in which subdependencies of the main project are
         # built (using setup.py bdist_egg) in the same python process. Assume
         # a main project A and a dependency B, which use different versions
         # of Versioneer. A's setup.py imports A's Versioneer, leaving it in
         # sys.modules by the time B's setup.py is executed, causing B to run
         # with the wrong versioneer. Setuptools wraps the sub-dep builds in a
         # sandbox that restores sys.modules to it's pre-build state, so the
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
-        # Also see https://github.com/warner/python-versioneer/issues/52
+        # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
-    cmds = {}
+    cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to both distutils and setuptools
-    from distutils.core import Command
+    # we add "version" to setuptools
+    from setuptools import Command
 
     class cmd_version(Command):
         description = "report generated version string"
-        user_options = []
-        boolean_options = []
+        user_options: List[Tuple[str, str, str]] = []
+        boolean_options: List[str] = []
 
-        def initialize_options(self):
+        def initialize_options(self) -> None:
             pass
 
-        def finalize_options(self):
+        def finalize_options(self) -> None:
             pass
 
-        def run(self):
+        def run(self) -> None:
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
 
     cmds["version"] = cmd_version
 
-    # we override "build_py" in both distutils and setuptools
+    # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
+    # pip install -e . and setuptool/editable_wheel will invoke build_py
+    # but the build_py command is not expected to copy any files.
+
     # we override different "build_py" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.build_py import build_py as _build_py
+    if "build_py" in cmds:
+        _build_py: Any = cmds["build_py"]
     else:
-        from distutils.command.build_py import build_py as _build_py
+        from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
-        def run(self):
+        def run(self) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
+            if getattr(self, "editable_mode", False):
+                # During editable installs `.py` and data files are
+                # not copied to build_lib
+                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
     cmds["build_py"] = cmd_build_py
 
+    if "build_ext" in cmds:
+        _build_ext: Any = cmds["build_ext"]
+    else:
+        from setuptools.command.build_ext import build_ext as _build_ext
+
+    class cmd_build_ext(_build_ext):
+        def run(self) -> None:
+            root = get_root()
+            cfg = get_config_from_root(root)
+            versions = get_versions()
+            _build_ext.run(self)
+            if self.inplace:
+                # build_ext --inplace will only build extensions in
+                # build/lib<..> dir with no _version.py to write to.
+                # As in place builds will already have a _version.py
+                # in the module dir, we do not need to write one.
+                return
+            # now locate _version.py in the new build/ directory and replace
+            # it with an updated value
+            if not cfg.versionfile_build:
+                return
+            target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
+            if not os.path.exists(target_versionfile):
+                print(
+                    f"Warning: {target_versionfile} does not exist, skipping "
+                    "version update. This can happen if you are running build_ext "
+                    "without first running build_py."
+                )
+                return
+            print("UPDATING %s" % target_versionfile)
+            write_to_version_file(target_versionfile, versions)
+
+    cmds["build_ext"] = cmd_build_ext
+
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
-        from cx_Freeze.dist import build_exe as _build_exe
+        from cx_Freeze.dist import build_exe as _build_exe  # type: ignore
 
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
         class cmd_build_exe(_build_exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -1639,20 +2070,20 @@
                     )
 
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if "py2exe" in sys.modules:  # py2exe enabled?
         try:
-            from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
+            from py2exe.setuptools_buildexe import py2exe as _py2exe  # type: ignore
         except ImportError:
-            from py2exe.build_exe import py2exe as _py2exe  # py2
+            from py2exe.distutils_buildexe import py2exe as _py2exe  # type: ignore
 
         class cmd_py2exe(_py2exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -1669,30 +2100,70 @@
                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
                         }
                     )
 
         cmds["py2exe"] = cmd_py2exe
 
+    # sdist farms its file list building out to egg_info
+    if "egg_info" in cmds:
+        _egg_info: Any = cmds["egg_info"]
+    else:
+        from setuptools.command.egg_info import egg_info as _egg_info
+
+    class cmd_egg_info(_egg_info):
+        def find_sources(self) -> None:
+            # egg_info.find_sources builds the manifest list and writes it
+            # in one shot
+            super().find_sources()
+
+            # Modify the filelist and normalize it
+            root = get_root()
+            cfg = get_config_from_root(root)
+            self.filelist.append("versioneer.py")
+            if cfg.versionfile_source:
+                # There are rare cases where versionfile_source might not be
+                # included by default, so we must be explicit
+                self.filelist.append(cfg.versionfile_source)
+            self.filelist.sort()
+            self.filelist.remove_duplicates()
+
+            # The write method is hidden in the manifest_maker instance that
+            # generated the filelist and was thrown away
+            # We will instead replicate their final normalization (to unicode,
+            # and POSIX-style paths)
+            from setuptools import unicode_utils
+
+            normalized = [
+                unicode_utils.filesys_decode(f).replace(os.sep, "/")
+                for f in self.filelist.files
+            ]
+
+            manifest_filename = os.path.join(self.egg_info, "SOURCES.txt")
+            with open(manifest_filename, "w") as fobj:
+                fobj.write("\n".join(normalized))
+
+    cmds["egg_info"] = cmd_egg_info
+
     # we override different "sdist" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.sdist import sdist as _sdist
+    if "sdist" in cmds:
+        _sdist: Any = cmds["sdist"]
     else:
-        from distutils.command.sdist import sdist as _sdist
+        from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
-        def run(self):
+        def run(self) -> None:
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
             self.distribution.metadata.version = versions["version"]
             return _sdist.run(self)
 
-        def make_release_tree(self, base_dir, files):
+        def make_release_tree(self, base_dir: str, files: List[str]) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
@@ -1739,32 +2210,33 @@
 #versionfile_source =
 #versionfile_build =
 #tag_prefix =
 #parentdir_prefix =
 
 """
 
-INIT_PY_SNIPPET = """
+OLD_SNIPPET = """
 from ._version import get_versions
 __version__ = get_versions()['version']
 del get_versions
 """
 
+INIT_PY_SNIPPET = """
+from . import {0}
+__version__ = {0}.get_versions()['version']
+"""
 
-def do_setup():
-    """Main VCS-independent setup function for installing Versioneer."""
+
+def do_setup() -> int:
+    """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (
-        EnvironmentError,
-        configparser.NoSectionError,
-        configparser.NoOptionError,
-    ) as e:
-        if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
+    except (OSError, configparser.NoSectionError, configparser.NoOptionError) as e:
+        if isinstance(e, (OSError, configparser.NoSectionError)):
             print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
@@ -1778,72 +2250,45 @@
                 "TAG_PREFIX": cfg.tag_prefix,
                 "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                 "VERSIONFILE_SOURCE": cfg.versionfile_source,
             }
         )
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
+    maybe_ipy: Optional[str] = ipy
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
-        except EnvironmentError:
+        except OSError:
             old = ""
-        if INIT_PY_SNIPPET not in old:
+        module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
+        snippet = INIT_PY_SNIPPET.format(module)
+        if OLD_SNIPPET in old:
+            print(" replacing boilerplate in %s" % ipy)
+            with open(ipy, "w") as f:
+                f.write(old.replace(OLD_SNIPPET, snippet))
+        elif snippet not in old:
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
-                f.write(INIT_PY_SNIPPET)
+                f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
-        ipy = None
-
-    # Make sure both the top-level "versioneer.py" and versionfile_source
-    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
-    # they'll be copied into source distributions. Pip won't be able to
-    # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
-    simple_includes = set()
-    try:
-        with open(manifest_in, "r") as f:
-            for line in f:
-                if line.startswith("include "):
-                    for include in line.split()[1:]:
-                        simple_includes.add(include)
-    except EnvironmentError:
-        pass
-    # That doesn't cover everything MANIFEST.in can do
-    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
-    # it might give some false negatives. Appending redundant 'include'
-    # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
-        print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
-    else:
-        print(" 'versioneer.py' already in MANIFEST.in")
-    if cfg.versionfile_source not in simple_includes:
-        print(
-            " appending versionfile_source ('%s') to MANIFEST.in"
-            % cfg.versionfile_source
-        )
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
-    else:
-        print(" versionfile_source already in MANIFEST.in")
+        maybe_ipy = None
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
+    do_vcs_install(cfg.versionfile_source, maybe_ipy)
     return 0
 
 
-def scan_setup_py():
+def scan_setup_py() -> int:
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
     errors = 0
     with open("setup.py", "r") as f:
         for line in f.readlines():
             if "import versioneer" in line:
@@ -1872,14 +2317,18 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
+def setup_command() -> NoReturn:
+    """Set up Versioneer and exit with appropriate error code."""
+    errors = do_setup()
+    errors += scan_setup_py()
+    sys.exit(1 if errors else 0)
+
+
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
+        setup_command()
```

