# Comparing `tmp/seismic-zfp-0.3.1.tar.gz` & `tmp/seismic_zfp-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seismic-zfp-0.3.1.tar", last modified: Wed Aug  3 11:32:42 2022, max compression
+gzip compressed data, was "seismic_zfp-0.3.3.tar", last modified: Fri May 24 07:58:41 2024, max compression
```

## Comparing `seismic-zfp-0.3.1.tar` & `seismic_zfp-0.3.3.tar`

### file list

```diff
@@ -1,173 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 11:32:42.806642 seismic-zfp-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 11:32:42.766641 seismic-zfp-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 11:32:42.770641 seismic-zfp-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      747 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/.github/workflows/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (116)      955 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1056 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (116)      206 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      517 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/CITATION
--rw-r--r--   0 runner    (1001) docker     (116)     2629 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     7652 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (116)     8537 2022-08-03 11:32:42.806642 seismic-zfp-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     8205 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 11:32:42.774641 seismic-zfp-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (116)   712502 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/docs/EAGE_extended-abstract.pdf
--rw-r--r--   0 runner    (1001) docker     (116)     3317 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/docs/file-specification.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 11:32:42.774641 seismic-zfp-0.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (116)      680 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     1056 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/example_accessors.py
--rw-r--r--   0 runner    (1001) docker     (116)      944 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/example_open.py
--rw-r--r--   0 runner    (1001) docker     (116)     5519 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/example_powerspectrum.py
--rw-r--r--   0 runner    (1001) docker     (116)     1122 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/example_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 11:32:42.778642 seismic-zfp-0.3.1/examples/sgz_reading/
--rw-r--r--   0 runner    (1001) docker     (116)     1090 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-2d-sgz-subplane.py
--rw-r--r--   0 runner    (1001) docker     (116)     1074 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-2d-sgz-traces.py
--rw-r--r--   0 runner    (1001) docker     (116)      615 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-all-inlines.py
--rw-r--r--   0 runner    (1001) docker     (116)     1666 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-anticorrelated-diagonal.py
--rw-r--r--   0 runner    (1001) docker     (116)     1085 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-as-xarray.py
--rw-r--r--   0 runner    (1001) docker     (116)     1528 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-correlated-diagonal.py
--rw-r--r--   0 runner    (1001) docker     (116)     1100 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-cropped-diagonals.py
--rw-r--r--   0 runner    (1001) docker     (116)     1496 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-crossline-unstructured.py
--rw-r--r--   0 runner    (1001) docker     (116)     1080 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-crossline.py
--rw-r--r--   0 runner    (1001) docker     (116)      991 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-cube.py
--rw-r--r--   0 runner    (1001) docker     (116)      317 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-file-header.py
--rw-r--r--   0 runner    (1001) docker     (116)      748 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-from-azure.py
--rw-r--r--   0 runner    (1001) docker     (116)      839 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-headerarrays.py
--rw-r--r--   0 runner    (1001) docker     (116)      277 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-headers.py
--rw-r--r--   0 runner    (1001) docker     (116)     1605 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-inline-unstructured.py
--rw-r--r--   0 runner    (1001) docker     (116)     1068 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-inline.py
--rw-r--r--   0 runner    (1001) docker     (116)     1190 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-subvolume.py
--rw-r--r--   0 runner    (1001) docker     (116)      427 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-traces.py
--rw-r--r--   0 runner    (1001) docker     (116)     1057 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_reading/read-zslice.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 11:32:42.778642 seismic-zfp-0.3.1/examples/sgz_writing/
--rw-r--r--   0 runner    (1001) docker     (116)      589 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_writing/numpy2sgz.py
--rw-r--r--   0 runner    (1001) docker     (116)      366 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_writing/sgy2sgz-adv.py
--rw-r--r--   0 runner    (1001) docker     (116)      361 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_writing/sgy2sgz.py
--rw-r--r--   0 runner    (1001) docker     (116)      361 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_writing/sgy2sgz_2d.py
--rw-r--r--   0 runner    (1001) docker     (116)      551 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_writing/sgy2sgz_crop.py
--rw-r--r--   0 runner    (1001) docker     (116)      334 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_writing/sgz2sgy.py
--rw-r--r--   0 runner    (1001) docker     (116)      337 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_writing/sgz2sgz_adv.py
--rw-r--r--   0 runner    (1001) docker     (116)     1579 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_writing/sgz_cropping.py
--rw-r--r--   0 runner    (1001) docker     (116)      359 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/examples/sgz_writing/zgy2sgz_.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 11:32:42.778642 seismic-zfp-0.3.1/gui/
--rw-r--r--   0 runner    (1001) docker     (116)      723 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/gui/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      155 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/gui/hook-seismic_zfp.py
--rw-r--r--   0 runner    (1001) docker     (116)       32 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/gui/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)     8607 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/gui/seismic-zfp-desktop.py
--rw-r--r--   0 runner    (1001) docker     (116)       30 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)       83 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 11:32:42.782642 seismic-zfp-0.3.1/seismic_zfp/
--rw-r--r--   0 runner    (1001) docker     (116)       47 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5582 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/accessors.py
--rw-r--r--   0 runner    (1001) docker     (116)     5253 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)    22259 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/conversion.py
--rw-r--r--   0 runner    (1001) docker     (116)    21138 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/conversion_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     9019 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/cropping.py
--rw-r--r--   0 runner    (1001) docker     (116)    10981 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/headers.py
--rw-r--r--   0 runner    (1001) docker     (116)    12842 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/loader.py
--rw-r--r--   0 runner    (1001) docker     (116)      277 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/open.py
--rw-r--r--   0 runner    (1001) docker     (116)    44363 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/read.py
--rw-r--r--   0 runner    (1001) docker     (116)     1786 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/segyio_emulator.py
--rw-r--r--   0 runner    (1001) docker     (116)     2464 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/seismicfile.py
--rw-r--r--   0 runner    (1001) docker     (116)     2594 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/sgz_xarray.py
--rw-r--r--   0 runner    (1001) docker     (116)      203 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/sgzconstants.py
--rw-r--r--   0 runner    (1001) docker     (116)      692 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/tools.py
--rw-r--r--   0 runner    (1001) docker     (116)     7175 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1754 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/seismic_zfp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 11:32:42.782642 seismic-zfp-0.3.1/seismic_zfp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8537 2022-08-03 11:32:42.000000 seismic-zfp-0.3.1/seismic_zfp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4698 2022-08-03 11:32:42.000000 seismic-zfp-0.3.1/seismic_zfp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-03 11:32:42.000000 seismic-zfp-0.3.1/seismic_zfp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      135 2022-08-03 11:32:42.000000 seismic-zfp-0.3.1/seismic_zfp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      112 2022-08-03 11:32:42.000000 seismic-zfp-0.3.1/seismic_zfp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2022-08-03 11:32:42.000000 seismic-zfp-0.3.1/seismic_zfp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-08-03 11:32:42.806642 seismic-zfp-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1600 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 11:32:42.790641 seismic-zfp-0.3.1/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 11:32:42.798642 seismic-zfp-0.3.1/test_data/padding/
--rw-r--r--   0 runner    (1001) docker     (116)    22400 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_5x5.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    25476 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_5x5.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    26160 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_5x6.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    25656 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_5x6.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    29920 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_5x7.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    25836 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_5x7.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    33680 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_5x8.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    26016 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_5x8.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    26160 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_6x5.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    25656 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_6x5.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    30672 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_6x6.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    25872 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_6x6.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    35184 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_6x7.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    26088 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_6x7.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    39696 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_6x8.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    26304 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_6x8.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    29920 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_7x5.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    25836 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_7x5.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    35184 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_7x6.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    26088 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_7x6.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    40448 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_7x7.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    26340 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_7x7.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    45712 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_7x8.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    26592 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_7x8.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    33680 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_8x5.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    26016 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_8x5.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    39696 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_8x6.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    26304 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_8x6.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    45712 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_8x7.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    26592 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_8x7.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    51728 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_8x8.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    26880 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/padding/padding_8x8.sgz
--rw-r--r--   0 runner    (1001) docker     (116)     5800 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small-2d-CROSSLINE_3D.sgy
--rw-r--r--   0 runner    (1001) docker     (116)     5800 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small-2d-INLINE_3D.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    14600 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small-2d.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    17408 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small-2d.sgz
--rw-r--r--   0 runner    (1001) docker     (116)     7560 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small-dec.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    12360 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small-dec_8bit.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    14600 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small-duplicate-traceheaders.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    14600 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small-ieee.sgy
--rw-r--r--   0 runner    (1001) docker     (116)     7120 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small-irreg-dec.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    14160 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small-irregular.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    25600 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small-irregular.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    11600 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small-negative-samples.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    14600 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small-traceheader-samplerate.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    14600 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    24776 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small_025bit.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    24776 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small_05bit.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    24776 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small_1bit.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    61640 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small_2bit-64x64.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    24776 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small_2bit.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    24776 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small_4bit.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    12488 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small_8bit-8x8.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    25600 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small_8bit.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    14160 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small_hole.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    25600 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small_hole.sgz
--rw-r--r--   0 runner    (1001) docker     (116)    14600 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small_negative_il_xl.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    14600 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small_reverse_il.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    14600 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small_us.sgy
--rw-r--r--   0 runner    (1001) docker     (116)    20480 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/small_v0.0.1.sgz
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 11:32:42.798642 seismic-zfp-0.3.1/test_data/vds/
--rw-r--r--   0 runner    (1001) docker     (116)   102751 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/vds/small.vds
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 11:32:42.802641 seismic-zfp-0.3.1/test_data/zgy/
--rwxr-xr-x   0 runner    (1001) docker     (116)    14600 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/zgy/small-16bit.sgy
--rwxr-xr-x   0 runner    (1001) docker     (116)  1048576 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/zgy/small-16bit.zgy
--rwxr-xr-x   0 runner    (1001) docker     (116)    14600 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/zgy/small-32bit.sgy
--rwxr-xr-x   0 runner    (1001) docker     (116)  2097152 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/zgy/small-32bit.zgy
--rwxr-xr-x   0 runner    (1001) docker     (116)    14600 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/zgy/small-8bit.sgy
--rwxr-xr-x   0 runner    (1001) docker     (116)   524288 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/test_data/zgy/small-8bit.zgy
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-03 11:32:42.806642 seismic-zfp-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5484 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)    20216 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/tests/test_compress.py
--rw-r--r--   0 runner    (1001) docker     (116)     4658 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/tests/test_cropping.py
--rw-r--r--   0 runner    (1001) docker     (116)     3345 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/tests/test_decompress.py
--rw-r--r--   0 runner    (1001) docker     (116)     1416 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/tests/test_header-accessors.py
--rw-r--r--   0 runner    (1001) docker     (116)     1298 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/tests/test_minimal_inline_reader.py
--rw-r--r--   0 runner    (1001) docker     (116)      979 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (116)    24908 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (116)     1628 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/tests/test_read_blob.py
--rw-r--r--   0 runner    (1001) docker     (116)    11235 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/tests/test_segyio-emulator.py
--rw-r--r--   0 runner    (1001) docker     (116)     1964 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/tests/test_seismicfile.py
--rw-r--r--   0 runner    (1001) docker     (116)      492 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/tests/test_trace-accessor.py
--rw-r--r--   0 runner    (1001) docker     (116)     4418 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     2078 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (116)      320 2022-08-03 11:31:49.000000 seismic-zfp-0.3.1/tests/test_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:58:41.867932 seismic_zfp-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:58:41.831932 seismic_zfp-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:58:41.835932 seismic_zfp-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/.github/workflows/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/CITATION
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-05-24 07:58:41.867932 seismic_zfp-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:58:41.835932 seismic_zfp-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)   712502 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/docs/EAGE_extended-abstract.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/docs/file-specification.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:58:41.835932 seismic_zfp-0.3.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/example_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/example_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/example_powerspectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/example_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:58:41.839932 seismic_zfp-0.3.3/examples/sgz_reading/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-2d-sgz-subplane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-2d-sgz-traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-all-inlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-anticorrelated-diagonal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-as-xarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-correlated-diagonal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-cropped-diagonals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-crossline-unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-crossline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-file-header.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-from-azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-headerarrays.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-inline-unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-inline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-subvolume.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_reading/read-zslice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:58:41.839932 seismic_zfp-0.3.3/examples/sgz_writing/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_writing/numpy2sgz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_writing/sgy2sgz-adv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_writing/sgy2sgz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_writing/sgy2sgz_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_writing/sgy2sgz_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_writing/sgz2sgy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_writing/sgz2sgz_adv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_writing/sgz_cropping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/examples/sgz_writing/zgy2sgz_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:58:41.843932 seismic_zfp-0.3.3/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/gui/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/gui/hook-seismic_zfp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/gui/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/gui/seismic-zfp-desktop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:58:41.843932 seismic_zfp-0.3.3/seismic_zfp/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22259 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21138 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/conversion_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/cropping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11024 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12842 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/open.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44363 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/segyio_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/seismicfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/sgz_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/sgzconstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/seismic_zfp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:58:41.867932 seismic_zfp-0.3.3/seismic_zfp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-05-24 07:58:41.000000 seismic_zfp-0.3.3/seismic_zfp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-05-24 07:58:41.000000 seismic_zfp-0.3.3/seismic_zfp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 07:58:41.000000 seismic_zfp-0.3.3/seismic_zfp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-24 07:58:41.000000 seismic_zfp-0.3.3/seismic_zfp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-24 07:58:41.000000 seismic_zfp-0.3.3/seismic_zfp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 07:58:41.000000 seismic_zfp-0.3.3/seismic_zfp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 07:58:41.867932 seismic_zfp-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:58:41.851932 seismic_zfp-0.3.3/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:58:41.859932 seismic_zfp-0.3.3/test_data/padding/
+-rw-r--r--   0 runner    (1001) docker     (127)    22400 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_5x5.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    25476 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_5x5.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    26160 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_5x6.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_5x6.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    29920 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_5x7.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    25836 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_5x7.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    33680 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_5x8.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    26016 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_5x8.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    26160 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_6x5.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_6x5.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    30672 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_6x6.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    25872 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_6x6.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_6x7.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    26088 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_6x7.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    39696 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_6x8.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    26304 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_6x8.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    29920 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_7x5.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    25836 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_7x5.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_7x6.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    26088 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_7x6.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    40448 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_7x7.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    26340 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_7x7.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    45712 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_7x8.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    26592 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_7x8.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    33680 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_8x5.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    26016 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_8x5.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    39696 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_8x6.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    26304 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_8x6.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    45712 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_8x7.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    26592 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_8x7.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    51728 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_8x8.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    26880 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/padding/padding_8x8.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small-2d-CROSSLINE_3D.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small-2d-INLINE_3D.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    14600 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small-2d.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    17408 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small-2d.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small-dec.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    12360 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small-dec_8bit.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    14600 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small-duplicate-traceheaders.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    14600 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small-ieee.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small-irreg-dec.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    14160 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small-irregular.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    25600 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small-irregular.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small-negative-samples.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    14600 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small-traceheader-samplerate.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    14600 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    24776 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small_025bit.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    24776 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small_05bit.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    24776 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small_1bit.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    61640 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small_2bit-64x64.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    24776 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small_2bit.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    24776 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small_4bit.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small_8bit-8x8.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    25600 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small_8bit.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    14160 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small_hole.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    25600 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small_hole.sgz
+-rw-r--r--   0 runner    (1001) docker     (127)    14600 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small_negative_il_xl.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    14600 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small_reverse_il.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    14600 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small_us.sgy
+-rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/small_v0.0.1.sgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:58:41.859932 seismic_zfp-0.3.3/test_data/vds/
+-rw-r--r--   0 runner    (1001) docker     (127)   102751 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/vds/small.vds
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:58:41.863932 seismic_zfp-0.3.3/test_data/zgy/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14600 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/zgy/small-16bit.sgy
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1048576 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/zgy/small-16bit.zgy
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14600 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/zgy/small-32bit.sgy
+-rwxr-xr-x   0 runner    (1001) docker     (127)  2097152 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/zgy/small-32bit.zgy
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14600 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/zgy/small-8bit.sgy
+-rwxr-xr-x   0 runner    (1001) docker     (127)   524288 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/test_data/zgy/small-8bit.zgy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:58:41.867932 seismic_zfp-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/tests/test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/tests/test_cropping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/tests/test_decompress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/tests/test_header-accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/tests/test_minimal_inline_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24908 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/tests/test_read_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11235 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/tests/test_segyio-emulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/tests/test_seismicfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/tests/test_trace-accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-24 07:58:06.000000 seismic_zfp-0.3.3/tests/test_xarray.py
```

### Comparing `seismic-zfp-0.3.1/.github/workflows/publish-to-pypi.yml` & `seismic_zfp-0.3.3/.github/workflows/publish-to-pypi.yml`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 on:
   release:
     types: [published]
 
 jobs:
   build-n-publish:
     name: Build and publish
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Set up Python 3.9
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: 3.9
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install pytest mock
           pip install .[zgy,vds,xr,azure]
@@ -29,8 +29,8 @@
           python -m pip install build --user
       - name: Build a binary wheel and a source tarball
         run: |
           python -m build --sdist --wheel --outdir dist/ .
       - name: Publish to Test PyPI
         uses: pypa/gh-action-pypi-publish@master
         with:
-          password: ${{ secrets.PYPI_API_TOKEN  }}
+          password: ${{ secrets.PYPI_API_TOKEN  }}
```

### Comparing `seismic-zfp-0.3.1/.github/workflows/run_tests.yml` & `seismic_zfp-0.3.3/.github/workflows/run_tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -10,38 +10,42 @@
   test:
 
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: ["windows-latest", "ubuntu-latest", "macos-latest"]
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
         exclude:
           - os: "macos-latest"
             python-version: "3.7"
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install testing dependencies
       run: |
         python -m pip install --upgrade pip
         pip install pytest mock
 
     - name: Install seismic-zfp dependencies with VDS
-      if: matrix.os != 'macos-latest'
+      if: matrix.os != 'macos-latest' && matrix.python-version != '3.7'
       run: pip install .[zgy,vds,xr,azure]
 
     - name: Install seismic-zfp dependencies without VDS
       if: matrix.os == 'macos-latest'
       run: pip install .[zgy,xr,azure]
 
+    - name: Install seismic-zfp dependencies without VDS or XR
+      if: matrix.python-version == '3.7'
+      run: pip install .[zgy,azure]
+
     - name: Test with pytest
       run: |
         pytest
```

### Comparing `seismic-zfp-0.3.1/CITATION` & `seismic_zfp-0.3.3/CITATION`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/CODE_OF_CONDUCT.md` & `seismic_zfp-0.3.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/LICENSE.md` & `seismic_zfp-0.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/PKG-INFO` & `seismic_zfp-0.3.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,13 @@
-Metadata-Version: 2.1
-Name: seismic-zfp
-Version: 0.3.1
-Summary: Compress and decompress seismic data
-Home-page: https://github.com/equinor/seismic-zfp
-Author: equinor
-License: LGPL-3.0
-Description-Content-Type: text/markdown
-Provides-Extra: zgy
-Provides-Extra: vds
-Provides-Extra: xr
-Provides-Extra: azure
-License-File: LICENSE.md
-
 # seismic-zfp #
 
 [![LGPLv3 License](https://img.shields.io/badge/License-LGPL%20v3-green.svg)](https://opensource.org/licenses/)
-[![Travis](https://travis-ci.org/equinor/seismic-zfp.svg?branch=master)](https://travis-ci.org/equinor/seismic-zfp)
+[![Run Tests](https://github.com/equinor/seismic-zfp/actions/workflows/run_tests.yml/badge.svg)](https://github.com/equinor/seismic-zfp/actions/workflows/run_tests.yml)
 [![codecov](https://codecov.io/gh/equinor/seismic-zfp/branch/master/graph/badge.svg)](https://codecov.io/gh/equinor/seismic-zfp)
+[![SCM Compliance](https://scm-compliance-api.radix.equinor.com/repos/equinor/seismic-zfp/badge)](https://scm-compliance-api.radix.equinor.com/repos/equinor/seismic-zfp/badge)
 [![PyPi Version](https://img.shields.io/pypi/v/seismic-zfp.svg)](https://pypi.org/project/seismic-zfp/)
 
 Python library to convert SEG-Y files to compressed cubes and retrieve arbitrary sub-volumes from these, fast.
 
 ## Motivation ##
 
 Reading whole SEG-Y volumes to retrieve, for example, a single time-slice is wasteful.
```

### Comparing `seismic-zfp-0.3.1/README.md` & `seismic_zfp-0.3.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,36 @@
+Metadata-Version: 2.1
+Name: seismic-zfp
+Version: 0.3.3
+Summary: Compress and decompress seismic data
+Home-page: https://github.com/equinor/seismic-zfp
+Author: equinor
+License: LGPL-3.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: numpy>=1.20
+Requires-Dist: segyio
+Requires-Dist: zfpy
+Requires-Dist: psutil
+Requires-Dist: click
+Provides-Extra: zgy
+Requires-Dist: pyzgy; extra == "zgy"
+Provides-Extra: vds
+Requires-Dist: pyvds; extra == "vds"
+Provides-Extra: xr
+Requires-Dist: xarray>=0.20.2; extra == "xr"
+Provides-Extra: azure
+Requires-Dist: azure-storage-blob; extra == "azure"
+
 # seismic-zfp #
 
 [![LGPLv3 License](https://img.shields.io/badge/License-LGPL%20v3-green.svg)](https://opensource.org/licenses/)
-[![Travis](https://travis-ci.org/equinor/seismic-zfp.svg?branch=master)](https://travis-ci.org/equinor/seismic-zfp)
+[![Run Tests](https://github.com/equinor/seismic-zfp/actions/workflows/run_tests.yml/badge.svg)](https://github.com/equinor/seismic-zfp/actions/workflows/run_tests.yml)
 [![codecov](https://codecov.io/gh/equinor/seismic-zfp/branch/master/graph/badge.svg)](https://codecov.io/gh/equinor/seismic-zfp)
+[![SCM Compliance](https://scm-compliance-api.radix.equinor.com/repos/equinor/seismic-zfp/badge)](https://scm-compliance-api.radix.equinor.com/repos/equinor/seismic-zfp/badge)
 [![PyPi Version](https://img.shields.io/pypi/v/seismic-zfp.svg)](https://pypi.org/project/seismic-zfp/)
 
 Python library to convert SEG-Y files to compressed cubes and retrieve arbitrary sub-volumes from these, fast.
 
 ## Motivation ##
 
 Reading whole SEG-Y volumes to retrieve, for example, a single time-slice is wasteful.
```

### Comparing `seismic-zfp-0.3.1/docs/EAGE_extended-abstract.pdf` & `seismic_zfp-0.3.3/docs/EAGE_extended-abstract.pdf`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/docs/file-specification.md` & `seismic_zfp-0.3.3/docs/file-specification.md`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/README.md` & `seismic_zfp-0.3.3/examples/README.md`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/example_accessors.py` & `seismic_zfp-0.3.3/examples/example_accessors.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/example_open.py` & `seismic_zfp-0.3.3/examples/example_open.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/example_powerspectrum.py` & `seismic_zfp-0.3.3/examples/example_powerspectrum.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/example_tools.py` & `seismic_zfp-0.3.3/examples/example_tools.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_reading/read-2d-sgz-subplane.py` & `seismic_zfp-0.3.3/examples/sgz_reading/read-2d-sgz-subplane.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_reading/read-2d-sgz-traces.py` & `seismic_zfp-0.3.3/examples/sgz_reading/read-2d-sgz-traces.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_reading/read-all-inlines.py` & `seismic_zfp-0.3.3/examples/sgz_reading/read-all-inlines.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_reading/read-anticorrelated-diagonal.py` & `seismic_zfp-0.3.3/examples/sgz_reading/read-anticorrelated-diagonal.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_reading/read-as-xarray.py` & `seismic_zfp-0.3.3/examples/sgz_reading/read-as-xarray.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_reading/read-correlated-diagonal.py` & `seismic_zfp-0.3.3/examples/sgz_reading/read-correlated-diagonal.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_reading/read-cropped-diagonals.py` & `seismic_zfp-0.3.3/examples/sgz_reading/read-cropped-diagonals.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_reading/read-crossline-unstructured.py` & `seismic_zfp-0.3.3/examples/sgz_reading/read-crossline-unstructured.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_reading/read-crossline.py` & `seismic_zfp-0.3.3/examples/sgz_reading/read-crossline.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_reading/read-cube.py` & `seismic_zfp-0.3.3/examples/sgz_reading/read-cube.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_reading/read-from-azure.py` & `seismic_zfp-0.3.3/examples/sgz_reading/read-from-azure.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_reading/read-headerarrays.py` & `seismic_zfp-0.3.3/examples/sgz_reading/read-headerarrays.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_reading/read-inline-unstructured.py` & `seismic_zfp-0.3.3/examples/sgz_reading/read-inline-unstructured.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_reading/read-inline.py` & `seismic_zfp-0.3.3/examples/sgz_reading/read-inline.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_reading/read-subvolume.py` & `seismic_zfp-0.3.3/examples/sgz_reading/read-subvolume.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_reading/read-zslice.py` & `seismic_zfp-0.3.3/examples/sgz_reading/read-zslice.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_writing/numpy2sgz.py` & `seismic_zfp-0.3.3/examples/sgz_writing/numpy2sgz.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_writing/sgy2sgz_crop.py` & `seismic_zfp-0.3.3/examples/sgz_writing/sgy2sgz_crop.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/examples/sgz_writing/sgz_cropping.py` & `seismic_zfp-0.3.3/examples/sgz_writing/sgz_cropping.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/gui/README.md` & `seismic_zfp-0.3.3/gui/README.md`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/gui/seismic-zfp-desktop.py` & `seismic_zfp-0.3.3/gui/seismic-zfp-desktop.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/seismic_zfp/accessors.py` & `seismic_zfp-0.3.3/seismic_zfp/accessors.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,17 +116,17 @@
         self.values_function = self.read_zslice
 
 
 class HeaderAccessor(Accessor):
     def __init__(self, file):
         super(Accessor, self).__init__(file)
         self.len_object = self.tracecount
-        self.keys_object = list(range(self.tracecount))
+        self.keys_object = range(self.tracecount)
         self.values_function = self.gen_trace_header
 
 
 class TraceAccessor(Accessor):
     def __init__(self, file):
         super(Accessor, self).__init__(file)
         self.len_object = self.tracecount
-        self.keys_object = list(range(self.tracecount))
+        self.keys_object = range(self.tracecount)
         self.values_function = self.get_trace
```

### Comparing `seismic-zfp-0.3.1/seismic_zfp/cli.py` & `seismic_zfp-0.3.3/seismic_zfp/cli.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/seismic_zfp/conversion.py` & `seismic_zfp-0.3.3/seismic_zfp/conversion.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/seismic_zfp/conversion_utils.py` & `seismic_zfp-0.3.3/seismic_zfp/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/seismic_zfp/cropping.py` & `seismic_zfp-0.3.3/seismic_zfp/cropping.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/seismic_zfp/headers.py` & `seismic_zfp-0.3.3/seismic_zfp/headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
                 for k in self.unique_variant_nonzero_header_words:
                     self.headers_dict[k] = np.zeros(n_traces, dtype=np.int32)
 
             elif seismicfile.filetype == Filetype.ZGY:
                 # Set up hw table with entries possible to scrape out of ZGY
                 self.table[115] = (int(seismicfile.n_samples), 0)
                 self.table[117] = (int(1000*seismicfile.zinc), 0)
+                self.table[71] = (-100, 0)
                 for hw_code in [181, 185, 189, 193]:
                     self.table[hw_code] = (0, hw_code)
 
                 # Create required numpy int arrays
                 cdp_x, cdp_y, iline_headers, xline_headers = self.get_zgy_header_arrays()
 
                 # Keep them in memory until file is ready for them to be written
```

### Comparing `seismic-zfp-0.3.1/seismic_zfp/loader.py` & `seismic_zfp-0.3.3/seismic_zfp/loader.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/seismic_zfp/read.py` & `seismic_zfp-0.3.3/seismic_zfp/read.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/seismic_zfp/segyio_emulator.py` & `seismic_zfp-0.3.3/seismic_zfp/segyio_emulator.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/seismic_zfp/seismicfile.py` & `seismic_zfp-0.3.3/seismic_zfp/seismicfile.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/seismic_zfp/sgz_xarray.py` & `seismic_zfp-0.3.3/seismic_zfp/sgz_xarray.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/seismic_zfp/tools.py` & `seismic_zfp-0.3.3/seismic_zfp/tools.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/seismic_zfp/utils.py` & `seismic_zfp-0.3.3/seismic_zfp/utils.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/seismic_zfp/version.py` & `seismic_zfp-0.3.3/seismic_zfp/version.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/seismic_zfp.egg-info/PKG-INFO` & `seismic_zfp-0.3.3/seismic_zfp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 Metadata-Version: 2.1
 Name: seismic-zfp
-Version: 0.3.1
+Version: 0.3.3
 Summary: Compress and decompress seismic data
 Home-page: https://github.com/equinor/seismic-zfp
 Author: equinor
 License: LGPL-3.0
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: numpy>=1.20
+Requires-Dist: segyio
+Requires-Dist: zfpy
+Requires-Dist: psutil
+Requires-Dist: click
 Provides-Extra: zgy
+Requires-Dist: pyzgy; extra == "zgy"
 Provides-Extra: vds
+Requires-Dist: pyvds; extra == "vds"
 Provides-Extra: xr
+Requires-Dist: xarray>=0.20.2; extra == "xr"
 Provides-Extra: azure
-License-File: LICENSE.md
+Requires-Dist: azure-storage-blob; extra == "azure"
 
 # seismic-zfp #
 
 [![LGPLv3 License](https://img.shields.io/badge/License-LGPL%20v3-green.svg)](https://opensource.org/licenses/)
-[![Travis](https://travis-ci.org/equinor/seismic-zfp.svg?branch=master)](https://travis-ci.org/equinor/seismic-zfp)
+[![Run Tests](https://github.com/equinor/seismic-zfp/actions/workflows/run_tests.yml/badge.svg)](https://github.com/equinor/seismic-zfp/actions/workflows/run_tests.yml)
 [![codecov](https://codecov.io/gh/equinor/seismic-zfp/branch/master/graph/badge.svg)](https://codecov.io/gh/equinor/seismic-zfp)
+[![SCM Compliance](https://scm-compliance-api.radix.equinor.com/repos/equinor/seismic-zfp/badge)](https://scm-compliance-api.radix.equinor.com/repos/equinor/seismic-zfp/badge)
 [![PyPi Version](https://img.shields.io/pypi/v/seismic-zfp.svg)](https://pypi.org/project/seismic-zfp/)
 
 Python library to convert SEG-Y files to compressed cubes and retrieve arbitrary sub-volumes from these, fast.
 
 ## Motivation ##
 
 Reading whole SEG-Y volumes to retrieve, for example, a single time-slice is wasteful.
```

### Comparing `seismic-zfp-0.3.1/seismic_zfp.egg-info/SOURCES.txt` & `seismic_zfp-0.3.3/seismic_zfp.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 CITATION
 CODE_OF_CONDUCT.md
 LICENSE.md
 README.md
+SECURITY.md
 requirements-dev.txt
 requirements.txt
 setup.py
 .github/workflows/codecov.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/run_tests.yml
 docs/EAGE_extended-abstract.pdf
```

### Comparing `seismic-zfp-0.3.1/setup.py` & `seismic_zfp-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_5x5.sgy` & `seismic_zfp-0.3.3/test_data/padding/padding_5x5.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_5x5.sgz` & `seismic_zfp-0.3.3/test_data/padding/padding_5x5.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_5x6.sgy` & `seismic_zfp-0.3.3/test_data/padding/padding_5x6.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_5x6.sgz` & `seismic_zfp-0.3.3/test_data/padding/padding_5x6.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_5x7.sgy` & `seismic_zfp-0.3.3/test_data/padding/padding_5x7.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_5x7.sgz` & `seismic_zfp-0.3.3/test_data/padding/padding_5x7.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_5x8.sgy` & `seismic_zfp-0.3.3/test_data/padding/padding_5x8.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_5x8.sgz` & `seismic_zfp-0.3.3/test_data/padding/padding_5x8.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_6x5.sgy` & `seismic_zfp-0.3.3/test_data/padding/padding_6x5.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_6x5.sgz` & `seismic_zfp-0.3.3/test_data/padding/padding_6x5.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_6x6.sgy` & `seismic_zfp-0.3.3/test_data/padding/padding_6x6.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_6x6.sgz` & `seismic_zfp-0.3.3/test_data/padding/padding_6x6.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_6x7.sgy` & `seismic_zfp-0.3.3/test_data/padding/padding_6x7.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_6x7.sgz` & `seismic_zfp-0.3.3/test_data/padding/padding_6x7.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_6x8.sgy` & `seismic_zfp-0.3.3/test_data/padding/padding_6x8.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_6x8.sgz` & `seismic_zfp-0.3.3/test_data/padding/padding_6x8.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_7x5.sgy` & `seismic_zfp-0.3.3/test_data/padding/padding_7x5.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_7x5.sgz` & `seismic_zfp-0.3.3/test_data/padding/padding_7x5.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_7x6.sgy` & `seismic_zfp-0.3.3/test_data/padding/padding_7x6.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_7x6.sgz` & `seismic_zfp-0.3.3/test_data/padding/padding_7x6.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_7x7.sgy` & `seismic_zfp-0.3.3/test_data/padding/padding_7x7.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_7x7.sgz` & `seismic_zfp-0.3.3/test_data/padding/padding_7x7.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_7x8.sgy` & `seismic_zfp-0.3.3/test_data/padding/padding_7x8.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_7x8.sgz` & `seismic_zfp-0.3.3/test_data/padding/padding_7x8.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_8x5.sgy` & `seismic_zfp-0.3.3/test_data/padding/padding_8x5.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_8x5.sgz` & `seismic_zfp-0.3.3/test_data/padding/padding_8x5.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_8x6.sgy` & `seismic_zfp-0.3.3/test_data/padding/padding_8x6.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_8x6.sgz` & `seismic_zfp-0.3.3/test_data/padding/padding_8x6.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_8x7.sgy` & `seismic_zfp-0.3.3/test_data/padding/padding_8x7.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_8x7.sgz` & `seismic_zfp-0.3.3/test_data/padding/padding_8x7.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_8x8.sgy` & `seismic_zfp-0.3.3/test_data/padding/padding_8x8.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/padding/padding_8x8.sgz` & `seismic_zfp-0.3.3/test_data/padding/padding_8x8.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small-2d-CROSSLINE_3D.sgy` & `seismic_zfp-0.3.3/test_data/small-2d-CROSSLINE_3D.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small-2d-INLINE_3D.sgy` & `seismic_zfp-0.3.3/test_data/small-2d-INLINE_3D.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small-2d.sgy` & `seismic_zfp-0.3.3/test_data/small-2d.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small-2d.sgz` & `seismic_zfp-0.3.3/test_data/small-2d.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small-dec.sgy` & `seismic_zfp-0.3.3/test_data/small-dec.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small-dec_8bit.sgz` & `seismic_zfp-0.3.3/test_data/small-dec_8bit.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small-duplicate-traceheaders.sgy` & `seismic_zfp-0.3.3/test_data/small-duplicate-traceheaders.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small-ieee.sgy` & `seismic_zfp-0.3.3/test_data/small-ieee.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small-irreg-dec.sgy` & `seismic_zfp-0.3.3/test_data/small-irreg-dec.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small-irregular.sgy` & `seismic_zfp-0.3.3/test_data/small-irregular.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small-irregular.sgz` & `seismic_zfp-0.3.3/test_data/small-irregular.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small-negative-samples.sgy` & `seismic_zfp-0.3.3/test_data/small-negative-samples.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small-traceheader-samplerate.sgy` & `seismic_zfp-0.3.3/test_data/small-traceheader-samplerate.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small.sgy` & `seismic_zfp-0.3.3/test_data/small.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small_025bit.sgz` & `seismic_zfp-0.3.3/test_data/small_025bit.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small_05bit.sgz` & `seismic_zfp-0.3.3/test_data/small_05bit.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small_1bit.sgz` & `seismic_zfp-0.3.3/test_data/small_1bit.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small_2bit-64x64.sgz` & `seismic_zfp-0.3.3/test_data/small_2bit-64x64.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small_2bit.sgz` & `seismic_zfp-0.3.3/test_data/small_2bit.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small_4bit.sgz` & `seismic_zfp-0.3.3/test_data/small_4bit.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small_8bit-8x8.sgz` & `seismic_zfp-0.3.3/test_data/small_8bit-8x8.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small_8bit.sgz` & `seismic_zfp-0.3.3/test_data/small_8bit.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small_hole.sgy` & `seismic_zfp-0.3.3/test_data/small_hole.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small_hole.sgz` & `seismic_zfp-0.3.3/test_data/small_hole.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small_negative_il_xl.sgy` & `seismic_zfp-0.3.3/test_data/small_negative_il_xl.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small_reverse_il.sgy` & `seismic_zfp-0.3.3/test_data/small_reverse_il.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small_us.sgy` & `seismic_zfp-0.3.3/test_data/small_us.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/small_v0.0.1.sgz` & `seismic_zfp-0.3.3/test_data/small_v0.0.1.sgz`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/vds/small.vds` & `seismic_zfp-0.3.3/test_data/vds/small.vds`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/zgy/small-16bit.sgy` & `seismic_zfp-0.3.3/test_data/zgy/small-16bit.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/zgy/small-16bit.zgy` & `seismic_zfp-0.3.3/test_data/zgy/small-16bit.zgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/zgy/small-32bit.sgy` & `seismic_zfp-0.3.3/test_data/zgy/small-32bit.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/zgy/small-32bit.zgy` & `seismic_zfp-0.3.3/test_data/zgy/small-32bit.zgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/zgy/small-8bit.sgy` & `seismic_zfp-0.3.3/test_data/zgy/small-8bit.sgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/test_data/zgy/small-8bit.zgy` & `seismic_zfp-0.3.3/test_data/zgy/small-8bit.zgy`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/tests/test_cli.py` & `seismic_zfp-0.3.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/tests/test_compress.py` & `seismic_zfp-0.3.3/tests/test_compress.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             sgz_ilines = sgzfile.ilines
             sgz_samples = sgzfile.zslices
             assert sgzfile.structured
 
             for trace_number in range(25):
                 sgz_header = sgzfile.header[trace_number]
                 zgy_header = zgyfile.header[trace_number]
-                for header_pos in [115, 117, 181, 185, 189, 193]:
+                for header_pos in [71, 115, 117, 181, 185, 189, 193]:
                     assert sgz_header[header_pos] == zgy_header[header_pos]
 
     assert np.allclose(sgz_data, segyio.tools.cube(sgy_file), rtol=rtol)
     assert all([a == b for a, b in zip(sgz_ilines, ref_ilines)])
     assert all(ref_samples == sgz_samples)
     assert 10 == SgzReader(out_filepath).get_file_source_code()
```

### Comparing `seismic-zfp-0.3.1/tests/test_cropping.py` & `seismic_zfp-0.3.3/tests/test_cropping.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/tests/test_decompress.py` & `seismic_zfp-0.3.3/tests/test_decompress.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/tests/test_header-accessors.py` & `seismic_zfp-0.3.3/tests/test_header-accessors.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/tests/test_minimal_inline_reader.py` & `seismic_zfp-0.3.3/tests/test_minimal_inline_reader.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/tests/test_open.py` & `seismic_zfp-0.3.3/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/tests/test_read.py` & `seismic_zfp-0.3.3/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/tests/test_read_blob.py` & `seismic_zfp-0.3.3/tests/test_read_blob.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/tests/test_segyio-emulator.py` & `seismic_zfp-0.3.3/tests/test_segyio-emulator.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/tests/test_seismicfile.py` & `seismic_zfp-0.3.3/tests/test_seismicfile.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/tests/test_utils.py` & `seismic_zfp-0.3.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `seismic-zfp-0.3.1/tests/test_version.py` & `seismic_zfp-0.3.3/tests/test_version.py`

 * *Files identical despite different names*

