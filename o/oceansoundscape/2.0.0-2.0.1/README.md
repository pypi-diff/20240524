# Comparing `tmp/oceansoundscape-2.0.0.tar.gz` & `tmp/oceansoundscape-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceansoundscape-2.0.0.tar", max compression
+gzip compressed data, was "oceansoundscape-2.0.1.tar", max compression
```

## Comparing `oceansoundscape-2.0.0.tar` & `oceansoundscape-2.0.1.tar`

### file list

```diff
@@ -1,21 +1,96 @@
--rw-r--r--   0        0        0    35148 2023-01-24 00:19:42.587993 oceansoundscape-2.0.0/LICENSE
--rw-r--r--   0        0        0     1198 2023-01-24 00:19:42.752961 oceansoundscape-2.0.0/README.md
--rw-r--r--   0        0        0       44 2023-01-26 14:15:33.204289 oceansoundscape-2.0.0/oceansoundscape/__init__.py
--rw-r--r--   0        0        0       52 2023-01-24 00:19:42.603093 oceansoundscape-2.0.0/oceansoundscape/raven/__init__.py
--rw-r--r--   0        0        0     5687 2023-01-24 00:19:42.709524 oceansoundscape-2.0.0/oceansoundscape/raven/parser.py
--rw-r--r--   0        0        0       63 2023-01-24 00:19:42.603266 oceansoundscape-2.0.0/oceansoundscape/spectrogram/__init__.py
--rw-r--r--   0        0        0     3100 2023-01-24 00:19:42.709684 oceansoundscape-2.0.0/oceansoundscape/spectrogram/colormap.py
--rw-r--r--   0        0        0     1445 2023-01-24 02:53:49.667394 oceansoundscape-2.0.0/oceansoundscape/spectrogram/conf.py
--rw-r--r--   0        0        0     5623 2023-01-24 02:53:49.667560 oceansoundscape-2.0.0/oceansoundscape/spectrogram/denoise.py
--rw-r--r--   0        0        0     1423 2023-01-24 00:19:42.588694 oceansoundscape-2.0.0/oceansoundscape/spectrogram/signal.py
--rw-r--r--   0        0        0     2593 2023-01-24 21:18:53.385316 oceansoundscape-2.0.0/oceansoundscape/spectrogram/utils.py
--rw-r--r--   0        0        0      289 2023-01-24 00:19:45.205752 oceansoundscape-2.0.0/oceansoundscape/testdata/MARS-20150910T000000Z-2kHz.wav.Table01.txt
--rw-r--r--   0        0        0        0 2023-01-24 00:19:42.588975 oceansoundscape-2.0.0/oceansoundscape/testdata/__init__.py
--rw-r--r--   0        0        0       35 2023-01-24 02:08:28.927838 oceansoundscape-2.0.0/oceansoundscape/tests/__init__.py
--rw-r--r--   0        0        0     9061 2022-04-01 20:31:30.258132 oceansoundscape-2.0.0/oceansoundscape/tests/data/MARS-20150910T000000Z-2kHz.wav.Table01.txt
--rw-r--r--   0        0        0        0 2022-04-01 20:31:30.257965 oceansoundscape-2.0.0/oceansoundscape/tests/data/__init__.py
--rw-r--r--   0        0        0     1426 2023-01-24 02:46:37.347155 oceansoundscape-2.0.0/oceansoundscape/tests/test_raven.py
--rw-r--r--   0        0        0     2535 2023-01-24 02:46:37.347387 oceansoundscape-2.0.0/oceansoundscape/tests/test_spectrogram.py
--rw-r--r--   0        0        0     1171 2023-01-26 14:14:03.251320 oceansoundscape-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2249 2023-01-26 14:19:13.312308 oceansoundscape-2.0.0/setup.py
--rw-r--r--   0        0        0     2529 2023-01-26 14:19:13.312514 oceansoundscape-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-01-24 00:19:42.587993 oceansoundscape-2.0.1/LICENSE
+-rw-r--r--   0        0        0      818 2024-05-24 03:17:22.080055 oceansoundscape-2.0.1/README.md
+-rw-r--r--   0        0        0       44 2024-05-24 18:57:19.635249 oceansoundscape-2.0.1/oceansoundscape/__init__.py
+-rw-r--r--   0        0        0       52 2023-01-24 00:19:42.603093 oceansoundscape-2.0.1/oceansoundscape/raven/__init__.py
+-rw-r--r--   0        0        0     5687 2024-05-24 03:18:38.951125 oceansoundscape-2.0.1/oceansoundscape/raven/parser.py
+-rw-r--r--   0        0        0       63 2023-01-24 00:19:42.603266 oceansoundscape-2.0.1/oceansoundscape/spectrogram/__init__.py
+-rw-r--r--   0        0        0     3100 2024-05-24 03:18:38.953407 oceansoundscape-2.0.1/oceansoundscape/spectrogram/colormap.py
+-rw-r--r--   0        0        0     1410 2023-01-30 16:59:37.822521 oceansoundscape-2.0.1/oceansoundscape/spectrogram/conf.py
+-rw-r--r--   0        0        0     5622 2024-05-24 03:18:38.948866 oceansoundscape-2.0.1/oceansoundscape/spectrogram/denoise.py
+-rw-r--r--   0        0        0     1423 2023-01-24 00:19:42.588694 oceansoundscape-2.0.1/oceansoundscape/spectrogram/signal.py
+-rw-r--r--   0        0        0     2593 2023-01-24 21:18:53.385316 oceansoundscape-2.0.1/oceansoundscape/spectrogram/utils.py
+-rw-r--r--   0        0        0  3603978 2023-01-24 01:06:06.098445 oceansoundscape-2.0.1/oceansoundscape/testdata/MARS-20150910T000000Z-2kHz.wav
+-rw-r--r--   0        0        0      289 2023-01-24 00:19:45.205752 oceansoundscape-2.0.1/oceansoundscape/testdata/MARS-20150910T000000Z-2kHz.wav.Table01.txt
+-rw-r--r--   0        0        0    18060 2021-10-08 03:49:23.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/MARS-20160521T000000Z-2kHz.wav.Table01.txt
+-rw-r--r--   0        0        0     1274 2021-10-08 03:49:24.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/MARS-20160617T000000Z-2kHz.wav.Table01.txt
+-rw-r--r--   0        0        0     1704 2021-10-08 03:49:36.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/MARS-20170415T000000Z-2kHz.wav.Table01.txt
+-rw-r--r--   0        0        0    69605 2021-11-22 21:36:43.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/MARS-20190728T000000Z-2kHz.wav.Table01.txt
+-rwxr-xr-x   0        0        0   150938 2021-06-23 11:20:34.238929 oceansoundscape-2.0.1/oceansoundscape/testdata/MARS-20201109T000000Z-2kHz.wav.Table01.txt
+-rw-r--r--   0        0        0        0 2023-01-24 00:19:42.588975 oceansoundscape-2.0.1/oceansoundscape/testdata/__init__.py
+-rw-r--r--   0        0        0    18062 2021-10-08 03:49:12.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20150808T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     6785 2021-10-08 03:49:13.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20150809T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    17036 2021-10-08 03:49:13.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20150902T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     4217 2021-10-08 03:49:14.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20150903T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     9284 2021-10-08 03:49:15.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20151025T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     1945 2021-10-08 03:49:15.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20151026T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     7046 2021-10-08 03:49:16.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20151129T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     4435 2021-10-08 03:49:16.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20151130T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     6677 2021-10-08 03:49:17.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20151215T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     4251 2021-10-08 03:49:17.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20151216T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     5008 2021-10-08 03:49:18.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160101T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     1926 2021-10-08 03:49:19.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160102T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     3241 2021-10-08 03:49:19.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160215T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     3042 2021-10-08 03:49:20.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160216T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     4591 2021-10-08 03:49:20.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160306T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     1707 2021-10-08 03:49:21.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160307T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     2140 2021-10-08 03:49:22.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160409T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     1701 2021-10-08 03:49:22.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160410T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    18060 2021-10-08 03:49:23.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160521T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    10378 2021-10-08 03:49:23.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160522T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    19727 2021-10-08 03:49:24.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160616T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     1274 2021-10-08 03:49:24.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160617T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     6416 2021-10-08 03:49:25.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160703T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     4377 2021-10-08 03:49:26.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160704T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    45016 2021-10-08 03:49:26.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160805T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     6784 2021-10-08 03:49:27.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160806T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     9957 2021-10-08 03:49:27.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160917T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     3083 2021-10-08 03:49:28.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20160918T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     7285 2021-10-08 03:49:28.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20161003T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     7909 2021-10-08 03:49:29.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20161004T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    16115 2021-10-08 03:49:30.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20161104T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     5822 2021-10-08 03:49:30.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20161105T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    17004 2021-10-08 03:49:31.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20161201T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     6493 2021-10-08 03:49:31.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20161202T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     2578 2021-10-08 03:49:32.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170126T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0      359 2021-10-08 03:49:33.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170127T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     5490 2021-10-08 03:49:33.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170203T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     4222 2021-10-08 03:49:34.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170204T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     2811 2021-10-08 03:49:34.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170309T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     1251 2021-10-08 03:49:35.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170310T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     3482 2021-10-08 03:49:35.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170414T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     1704 2021-10-08 03:49:36.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170415T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     2595 2021-10-08 03:49:37.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170506T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     2845 2021-10-08 03:49:37.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170507T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    67614 2021-10-08 03:49:38.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170605T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    23607 2021-10-08 03:49:38.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170606T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    51416 2021-10-08 03:49:39.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170705T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    23009 2021-10-08 03:49:40.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170706T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    35791 2021-10-08 03:49:40.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170812T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    26825 2021-10-08 03:49:41.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170813T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    19258 2021-10-08 03:49:41.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170920T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     8338 2021-10-08 03:49:42.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20170921T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    30285 2021-10-08 03:49:43.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20171011T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     9224 2021-10-08 03:49:43.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20171012T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    49636 2021-10-08 03:49:44.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20171103T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    11925 2021-10-08 03:49:44.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20171104T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    31120 2021-10-08 03:49:45.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20171204T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    10337 2021-10-08 03:49:45.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20171205T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    16710 2021-10-08 03:49:46.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20180106T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     5858 2021-10-08 03:49:47.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20180107T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     3243 2021-10-08 03:49:47.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20180202T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0      803 2021-10-08 03:49:48.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20180203T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     2143 2021-10-08 03:49:48.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20180327T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     1245 2021-10-08 03:49:49.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20180328T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     1235 2021-10-08 03:49:49.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20180411T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     2155 2021-10-08 03:49:50.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20180412T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    17145 2021-10-08 03:49:51.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20180512T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     2834 2021-10-08 03:49:51.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20180513T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    10857 2021-10-08 03:49:52.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20180604T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0     3080 2021-10-08 03:49:53.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20180605T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0    69605 2021-11-22 21:36:43.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20190728T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0   149856 2021-11-23 02:12:24.000000 oceansoundscape-2.0.1/oceansoundscape/testdata/blueDBLEDval/MARS-20200725T000000Z-2kHz.Band.Limited.Energy.Detector.selections.txt
+-rw-r--r--   0        0        0       35 2023-01-24 02:08:28.927838 oceansoundscape-2.0.1/oceansoundscape/tests/__init__.py
+-rw-r--r--   0        0        0     1265 2024-05-24 03:17:22.080759 oceansoundscape-2.0.1/oceansoundscape/tests/test_raven.py
+-rw-r--r--   0        0        0     2361 2024-05-24 19:00:19.164492 oceansoundscape-2.0.1/oceansoundscape/tests/test_spectrogram.py
+-rw-r--r--   0        0        0     1947 2024-05-24 18:41:22.570377 oceansoundscape-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2176 1970-01-01 00:00:00.000000 oceansoundscape-2.0.1/PKG-INFO
```

### Comparing `oceansoundscape-2.0.0/LICENSE` & `oceansoundscape-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oceansoundscape-2.0.0/oceansoundscape/raven/parser.py` & `oceansoundscape-2.0.1/oceansoundscape/raven/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 __author__ = 'Danelle Cline'
-__copyright__ = '2022'
+__copyright__ = '2024'
 __license__ = 'GPL v3'
 __contact__ = 'dcline at mbari.org'
 __doc__ = '''
 
 Reads in a BLED annotation file created by the Raven software
 
 @var __date__: Date of last svn commit
```

### Comparing `oceansoundscape-2.0.0/oceansoundscape/spectrogram/colormap.py` & `oceansoundscape-2.0.1/oceansoundscape/spectrogram/colormap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 __author__ = 'Danelle Cline'
-__copyright__ = '2022'
+__copyright__ = '2024'
 __license__ = 'GPL v3'
 __contact__ = 'dcline at mbari.org'
 __doc__ = '''
 
 Parula colormap
 
 @var __date__: Date of last svn commit
```

### Comparing `oceansoundscape-2.0.0/oceansoundscape/spectrogram/conf.py` & `oceansoundscape-2.0.1/oceansoundscape/spectrogram/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     blur_axis='time',
     num_fft=512,
     center=True, # call should be centered during training
     # padding in seconds to add to beginning/ending of wav files
     padding_secs=2
 )
 BLUE_D = dict(
-    freq_range=[(25,250), (20,75)],
-    low_freq=25,
-    high_freq=75,
+    freq_range=[(25,200), (20,75)],
     duration_secs=7,
     blur_axis='',
     num_fft=1024,
     center=True, # call should be centered during training
     padding_secs=2,
     num_mels=30
 )
```

### Comparing `oceansoundscape-2.0.0/oceansoundscape/spectrogram/denoise.py` & `oceansoundscape-2.0.1/oceansoundscape/spectrogram/denoise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 __author__ = 'Danelle Cline'
-__copyright__ = '2022'
+__copyright__ = '2024'
 __license__ = 'GPL v3'
 __contact__ = 'dcline at mbari.org'
 __doc__ = '''
 
 PCEN denoise and cache
 
 @var __date__: Date of last svn commit
@@ -18,15 +18,14 @@
 import sklearn
 import numpy as np
 from pathlib import Path
 from oceansoundscape.raven import BLEDParser
 from oceansoundscape.spectrogram import conf as global_conf
 from oceansoundscape.spectrogram import utils
 
-
 class PCENSmooth(object):
 
     def __init__(self, hdf_path: Path, bled: BLEDParser, conf: dict(), x: np.array([]), sample_rate: int):
         """
         Denoises file with PCEN and caches in an HDF file; it if exists it will be overwritten
         :param hdf_path: absolute path to hdf file
         :param bled: RavenBLEDParser
```

### Comparing `oceansoundscape-2.0.0/oceansoundscape/spectrogram/signal.py` & `oceansoundscape-2.0.1/oceansoundscape/spectrogram/signal.py`

 * *Files identical despite different names*

### Comparing `oceansoundscape-2.0.0/oceansoundscape/spectrogram/utils.py` & `oceansoundscape-2.0.1/oceansoundscape/spectrogram/utils.py`

 * *Files identical despite different names*

### Comparing `oceansoundscape-2.0.0/oceansoundscape/tests/test_raven.py` & `oceansoundscape-2.0.1/oceansoundscape/tests/test_raven.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 import unittest
 import tempfile
 from pathlib import Path
+import oceansoundscape
 from oceansoundscape.raven import BLEDParser
 from oceansoundscape.spectrogram import conf
 from oceansoundscape import testdata
 
-from nose.tools import assert_dict_equal
-
-try:
-    import importlib.resources as pkg_resources
-except ImportError:
-    import importlib_resources as pkg_resources
+import importlib.resources as resources
 
 class TestRaven(unittest.TestCase):
     def test_bled_parser(self):
         max_samples = 10 * 60 * 2e3
-        with pkg_resources.path(testdata, "MARS-20150910T000000Z-2kHz.wav.Table01.txt") as bled_path:
-            print(f"bled_file: {bled_path}")
-            parser = BLEDParser(bled_path, conf.CONF_DICT['blueA'], max_samples=max_samples, sampling_rate=2e3)
-            df_subset = parser.data[0:1]
-            actual = df_subset.to_dict()
-            print(f"Actual {actual}")
-            expected = {'Selection': {0: 2},
-                        'Classification': {0: 'baf'},
-                        'Begin Time (s)': {0: 161.79},
-                        'End Time (s)': {0: 180.99},
-                        'call_start': {0: 317780.0},
-                        'call_end': {0: 367780.0},
-                        'image_filename': {0: '20150910T000241_baf.323580.361980.sel.02.ch01.spectrogram.jpg'},
-                        'has_label': {0: True}}
-            assert_dict_equal(expected, actual, "Error parsing BLED file")
+        bled_path = resources.files('oceansoundscape.testdata').joinpath("MARS-20150910T000000Z-2kHz.wav.Table01.txt")
+        print(f"bled_file: {bled_path}")
+        parser = BLEDParser(bled_path, conf.CONF_DICT['blueA'], max_samples=max_samples, sampling_rate=2e3)
+        df_subset = parser.data[0:1]
+        actual = df_subset.to_dict()
+        print(f"Actual {actual}")
+        expected = {'Selection': {0: 2},
+                    'Classification': {0: 'baf'},
+                    'Begin Time (s)': {0: 161.79},
+                    'End Time (s)': {0: 180.99},
+                    'call_start': {0: 317780.0},
+                    'call_end': {0: 367780.0},
+                    'image_filename': {0: '20150910T000241_baf.323580.361980.sel.02.ch01.spectrogram.jpg'},
+                    'has_label': {0: True}}
+
+        self.assertDictEqual(actual, expected)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `oceansoundscape-2.0.0/oceansoundscape/tests/test_spectrogram.py` & `oceansoundscape-2.0.1/oceansoundscape/tests/test_spectrogram.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 import unittest
 from pathlib import Path
+import oceansoundscape
 from oceansoundscape.raven import BLEDParser
 from oceansoundscape.spectrogram import conf, utils, denoise
 from oceansoundscape import testdata
 import soundfile as sf
 import tempfile
 
-try:
-    import importlib.resources as pkg_resources
-except ImportError:
-    import importlib_resources as pkg_resources
+import importlib.resources as resources
 
 class TestSpectrogram(unittest.TestCase):
 
     def test_blue_a(self):
         blue_conf = conf.CONF_DICT['blueA']
         with tempfile.TemporaryDirectory() as temp_dir:
             temp_path = Path(temp_dir)
-            with pkg_resources.path(testdata, "MARS-20150910T000000Z-2kHz.wav") as w:
-                with pkg_resources.path(testdata, "MARS-20150910T000000Z-2kHz.wav.Table01.txt") as b:
-                    x, sample_rate = sf.read(w, dtype='float32')
-                    print(f"Found {sample_rate} {len(x)} samples")
-                    self.assertEqual(len(x), 1201200)
-                    parser = BLEDParser(b, blue_conf, len(x), sample_rate)
-                    print(f'Denoising {b}')
-                    cache = denoise.PCENSmooth(temp_path / 'MARS-20150910T000000Z-2kHz.wav.Table01.txt.hdf', parser, blue_conf, x, sample_rate)
-                    call_width = int(blue_conf['duration_secs'] * sample_rate)
-                    num_fft = blue_conf['num_fft']
-                    hop_length = round(num_fft * (1 - conf.OVERLAP))
-                    num_processed = 1
-
-                    for row, item in sorted(parser.data.iterrows()):
-                        try:
-                            if item.has_label:
-                                data = cache.get_data(item.Selection)
-                                start = int(call_width / hop_length)
-                                end = int(2 * call_width / hop_length)
-
-                                # subset the call, leaving off the padding for PCEN
-                                subset_data = data[:, start:end]
-
-                                # save to a denoised color image
-                                utils.ImageUtils.colorizeDenoise(subset_data, temp_path / Path(item.image_filename))
-
-                                print(f'Processed row {row} total processed {num_processed} {item.image_filename} ')
-                                num_processed += 1
-                        except Exception as ex:
-                            print(ex)
-                            continue
-                    self.assertEqual(num_processed, 3)
+            package_name = 'oceansoundscape.testdata'
+            w = resources.files(package_name).joinpath("MARS-20150910T000000Z-2kHz.wav")
+            b = resources.files(package_name).joinpath("MARS-20150910T000000Z-2kHz.wav.Table01.txt")
+            x, sample_rate = sf.read(w, dtype='float32')
+            print(f"Found {sample_rate} {len(x)} samples")
+            self.assertEqual(len(x), 1201200)
+            parser = BLEDParser(Path(b), blue_conf, len(x), sample_rate)
+            print(f'Denoising {b}')
+            cache = denoise.PCENSmooth(temp_path / 'MARS-20150910T000000Z-2kHz.wav.Table01.txt.hdf', parser, blue_conf, x, sample_rate)
+            call_width = int(blue_conf['duration_secs'] * sample_rate)
+            num_fft = blue_conf['num_fft']
+            hop_length = round(num_fft * (1 - conf.OVERLAP))
+            num_processed = 1
+
+            for row, item in sorted(parser.data.iterrows()):
+                try:
+                    if item.has_label:
+                        data = cache.get_data(item.Selection)
+                        start = int(call_width / hop_length)
+                        end = int(2 * call_width / hop_length)
+
+                        # subset the call, leaving off the padding for PCEN
+                        subset_data = data[:, start:end]
+
+                        # save to a denoised color image
+                        utils.ImageUtils.colorizeDenoise(subset_data, temp_path / Path(item.image_filename))
+
+                        print(f'Processed row {row} total processed {num_processed} {item.image_filename} ')
+                        num_processed += 1
+                except Exception as ex:
+                    print(ex)
+                    continue
+            self.assertEqual(num_processed, 3)
+            temp_path.rmdir()
         print('Done')
 
 if __name__ == '__main__':
     unittest.main()
```

