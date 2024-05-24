# Comparing `tmp/masterfile-0.6.0.tar.gz` & `tmp/masterfile-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masterfile-0.6.0.tar", last modified: Wed Jun 30 22:21:41 2021, max compression
+gzip compressed data, was "masterfile-0.6.1.tar", last modified: Fri May 24 16:39:24 2024, max compression
```

## Comparing `masterfile-0.6.0.tar` & `masterfile-0.6.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2021-06-30 22:21:41.097642 masterfile-0.6.0/
--rw-r--r--   0 njvack     (501) staff       (20)     1113 2017-08-11 20:55:06.000000 masterfile-0.6.0/LICENSE
--rw-r--r--   0 njvack     (501) staff       (20)      196 2017-08-11 20:55:06.000000 masterfile-0.6.0/MANIFEST.in
--rw-r--r--   0 njvack     (501) staff       (20)     5399 2021-06-30 22:21:41.097861 masterfile-0.6.0/PKG-INFO
--rw-r--r--   0 njvack     (501) staff       (20)     3499 2020-09-24 15:48:33.000000 masterfile-0.6.0/README.md
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2021-06-30 22:21:41.085877 masterfile-0.6.0/masterfile/
--rw-r--r--   0 njvack     (501) staff       (20)      286 2020-09-24 15:48:33.000000 masterfile-0.6.0/masterfile/__init__.py
--rw-r--r--   0 njvack     (501) staff       (20)      332 2021-06-30 22:18:17.000000 masterfile-0.6.0/masterfile/_metadata.py
--rw-r--r--   0 njvack     (501) staff       (20)     2512 2020-09-24 15:48:33.000000 masterfile-0.6.0/masterfile/annotator.py
--rw-r--r--   0 njvack     (501) staff       (20)     4865 2020-09-24 15:48:33.000000 masterfile-0.6.0/masterfile/dictionary.py
--rw-r--r--   0 njvack     (501) staff       (20)     3965 2021-06-28 19:01:31.000000 masterfile-0.6.0/masterfile/errors.py
--rw-r--r--   0 njvack     (501) staff       (20)     1385 2020-09-24 15:48:33.000000 masterfile-0.6.0/masterfile/formatters.py
--rw-r--r--   0 njvack     (501) staff       (20)    10284 2021-06-30 19:33:59.000000 masterfile-0.6.0/masterfile/masterfile.py
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2021-06-30 22:21:41.088163 masterfile-0.6.0/masterfile/scripts/
--rw-r--r--   0 njvack     (501) staff       (20)        0 2020-09-24 15:48:33.000000 masterfile-0.6.0/masterfile/scripts/__init__.py
--rw-r--r--   0 njvack     (501) staff       (20)     2055 2020-09-24 15:48:33.000000 masterfile-0.6.0/masterfile/scripts/create.py
--rw-r--r--   0 njvack     (501) staff       (20)     3853 2021-06-25 21:42:54.000000 masterfile-0.6.0/masterfile/scripts/extract.py
--rw-r--r--   0 njvack     (501) staff       (20)     1299 2021-06-30 20:14:20.000000 masterfile-0.6.0/masterfile/scripts/join.py
--rw-r--r--   0 njvack     (501) staff       (20)     4151 2021-06-30 20:46:13.000000 masterfile-0.6.0/masterfile/scripts/masterfile.py
--rw-r--r--   0 njvack     (501) staff       (20)     3030 2021-06-30 21:34:48.000000 masterfile-0.6.0/masterfile/scripts/pretty.py
--rw-r--r--   0 njvack     (501) staff       (20)     1511 2020-09-24 15:48:33.000000 masterfile-0.6.0/masterfile/scripts/text_to_dos.py
--rw-r--r--   0 njvack     (501) staff       (20)     1887 2020-09-24 15:48:33.000000 masterfile-0.6.0/masterfile/scripts/validate.py
--rw-r--r--   0 njvack     (501) staff       (20)     1341 2020-09-24 15:48:33.000000 masterfile-0.6.0/masterfile/validator.py
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2021-06-30 22:21:41.091194 masterfile-0.6.0/masterfile/validators/
--rw-r--r--   0 njvack     (501) staff       (20)      192 2020-09-24 15:48:33.000000 masterfile-0.6.0/masterfile/validators/__init__.py
--rw-r--r--   0 njvack     (501) staff       (20)     2183 2020-09-24 15:48:33.000000 masterfile-0.6.0/masterfile/validators/column_format.py
--rw-r--r--   0 njvack     (501) staff       (20)     1763 2020-09-24 15:48:33.000000 masterfile-0.6.0/masterfile/validators/components_in_dictionary.py
--rw-r--r--   0 njvack     (501) staff       (20)      947 2020-09-24 15:48:33.000000 masterfile-0.6.0/masterfile/validators/dictionary_format.py
--rw-r--r--   0 njvack     (501) staff       (20)     2227 2020-09-24 15:48:33.000000 masterfile-0.6.0/masterfile/validators/duplicate_column.py
--rw-r--r--   0 njvack     (501) staff       (20)     2788 2020-09-24 15:48:33.000000 masterfile-0.6.0/masterfile/validators/index_column.py
--rw-r--r--   0 njvack     (501) staff       (20)      754 2020-09-24 15:48:33.000000 masterfile-0.6.0/masterfile/validators/io.py
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2021-06-30 22:21:41.086709 masterfile-0.6.0/masterfile.egg-info/
--rw-rw-r--   0 njvack     (501) staff       (20)     5399 2021-06-30 22:21:41.000000 masterfile-0.6.0/masterfile.egg-info/PKG-INFO
--rw-rw-r--   0 njvack     (501) staff       (20)     2242 2021-06-30 22:21:41.000000 masterfile-0.6.0/masterfile.egg-info/SOURCES.txt
--rw-rw-r--   0 njvack     (501) staff       (20)        1 2021-06-30 22:21:41.000000 masterfile-0.6.0/masterfile.egg-info/dependency_links.txt
--rw-rw-r--   0 njvack     (501) staff       (20)       67 2021-06-30 22:21:41.000000 masterfile-0.6.0/masterfile.egg-info/entry_points.txt
--rw-rw-r--   0 njvack     (501) staff       (20)        1 2020-05-21 12:40:13.000000 masterfile-0.6.0/masterfile.egg-info/not-zip-safe
--rw-rw-r--   0 njvack     (501) staff       (20)       36 2021-06-30 22:21:41.000000 masterfile-0.6.0/masterfile.egg-info/requires.txt
--rw-rw-r--   0 njvack     (501) staff       (20)       17 2021-06-30 22:21:41.000000 masterfile-0.6.0/masterfile.egg-info/top_level.txt
--rw-r--r--   0 njvack     (501) staff       (20)     1150 2021-06-30 22:21:41.098344 masterfile-0.6.0/setup.cfg
--rwxr-xr-x   0 njvack     (501) staff       (20)      595 2020-09-24 15:48:33.000000 masterfile-0.6.0/setup.py
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2021-06-30 22:21:41.092659 masterfile-0.6.0/tests/
--rw-r--r--   0 njvack     (501) staff       (20)       24 2017-08-11 20:55:06.000000 masterfile-0.6.0/tests/__init__.py
--rw-r--r--   0 njvack     (501) staff       (20)     1762 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/conftest.py
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2021-06-30 22:21:41.093112 masterfile-0.6.0/tests/examples/
--rw-r--r--   0 njvack     (501) staff       (20)     6148 2017-08-30 18:11:47.000000 masterfile-0.6.0/tests/examples/.DS_Store
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2021-06-30 22:21:41.093494 masterfile-0.6.0/tests/examples/baddict/
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2021-06-30 22:21:41.093723 masterfile-0.6.0/tests/examples/baddict/dictionary/
--rw-rw-r--   0 njvack     (501) staff       (20)      105 2020-01-22 15:10:43.000000 masterfile-0.6.0/tests/examples/baddict/dictionary/dictionary.csv
--rw-rw-r--   0 njvack     (501) staff       (20)      160 2020-01-22 15:10:43.000000 masterfile-0.6.0/tests/examples/baddict/foo.csv
--rw-r--r--   0 njvack     (501) staff       (20)       74 2021-06-28 19:18:08.000000 masterfile-0.6.0/tests/examples/baddict/settings.yml
--rw-r--r--   0 njvack     (501) staff       (20)      273 2017-09-01 20:42:57.000000 masterfile-0.6.0/tests/examples/foo_input.csv
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2021-06-30 22:21:41.094327 masterfile-0.6.0/tests/examples/good/
--rw-r--r--   0 njvack     (501) staff       (20)      160 2021-06-30 19:00:55.000000 masterfile-0.6.0/tests/examples/good/bar.csv
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2021-06-30 22:21:41.094693 masterfile-0.6.0/tests/examples/good/dictionary/
--rw-r--r--   0 njvack     (501) staff       (20)       93 2018-03-14 17:14:31.000000 masterfile-0.6.0/tests/examples/good/dictionary/dictionary.csv
--rw-r--r--   0 njvack     (501) staff       (20)      101 2018-03-14 17:14:31.000000 masterfile-0.6.0/tests/examples/good/dictionary/measure_contacts.csv
--rw-r--r--   0 njvack     (501) staff       (20)      160 2021-06-30 19:00:57.000000 masterfile-0.6.0/tests/examples/good/foo.csv
--rw-r--r--   0 njvack     (501) staff       (20)      117 2021-06-28 19:13:45.000000 masterfile-0.6.0/tests/examples/good/settings.yml
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2021-06-30 22:21:41.095108 masterfile-0.6.0/tests/examples/problems/
--rw-r--r--   0 njvack     (501) staff       (20)      119 2018-03-14 17:14:31.000000 masterfile-0.6.0/tests/examples/problems/bar.csv
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2021-06-30 22:21:41.095473 masterfile-0.6.0/tests/examples/problems/dictionary/
--rw-r--r--   0 njvack     (501) staff       (20)      119 2018-03-14 17:14:31.000000 masterfile-0.6.0/tests/examples/problems/dictionary/dictionary.csv
--rw-r--r--   0 njvack     (501) staff       (20)       28 2018-03-14 17:14:31.000000 masterfile-0.6.0/tests/examples/problems/dictionary/noindex.csv
--rw-r--r--   0 njvack     (501) staff       (20)      252 2018-03-14 17:14:31.000000 masterfile-0.6.0/tests/examples/problems/foo.csv
--rw-r--r--   0 njvack     (501) staff       (20)       74 2021-06-28 19:18:04.000000 masterfile-0.6.0/tests/examples/problems/settings.yml
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2021-06-30 22:21:41.096444 masterfile-0.6.0/tests/scripts/
--rw-r--r--   0 njvack     (501) staff       (20)        0 2018-03-14 17:14:31.000000 masterfile-0.6.0/tests/scripts/__init__.py
--rw-r--r--   0 njvack     (501) staff       (20)     2668 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/scripts/test_extract_masterfile_data.py
--rw-r--r--   0 njvack     (501) staff       (20)      927 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/scripts/test_make_blank_dictionary.py
--rw-r--r--   0 njvack     (501) staff       (20)      954 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/scripts/test_make_joined_data.py
--rw-r--r--   0 njvack     (501) staff       (20)      740 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/scripts/test_make_pretty_dictionary.py
--rw-r--r--   0 njvack     (501) staff       (20)     1658 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/scripts/test_validate_masterfile.py
--rw-r--r--   0 njvack     (501) staff       (20)     1667 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/test_annotator.py
--rw-r--r--   0 njvack     (501) staff       (20)     2412 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/test_dictionary.py
--rw-r--r--   0 njvack     (501) staff       (20)     1552 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/test_errors.py
--rw-r--r--   0 njvack     (501) staff       (20)     1338 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/test_formatters.py
--rw-r--r--   0 njvack     (501) staff       (20)     3235 2021-06-24 21:58:06.000000 masterfile-0.6.0/tests/test_masterfile.py
--rw-r--r--   0 njvack     (501) staff       (20)     2359 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/test_validator.py
-drwxr-xr-x   0 njvack     (501) staff       (20)        0 2021-06-30 22:21:41.097518 masterfile-0.6.0/tests/validators/
--rw-r--r--   0 njvack     (501) staff       (20)        0 2018-03-14 17:14:31.000000 masterfile-0.6.0/tests/validators/__init__.py
--rw-r--r--   0 njvack     (501) staff       (20)      947 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/validators/test_column_format.py
--rw-r--r--   0 njvack     (501) staff       (20)      873 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/validators/test_components_in_dictionary.py
--rw-r--r--   0 njvack     (501) staff       (20)      788 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/validators/test_dictionary_format.py
--rw-r--r--   0 njvack     (501) staff       (20)     1748 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/validators/test_duplicate_column.py
--rw-r--r--   0 njvack     (501) staff       (20)     1330 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/validators/test_index_column.py
--rw-r--r--   0 njvack     (501) staff       (20)      934 2020-09-24 15:48:33.000000 masterfile-0.6.0/tests/validators/test_io.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-24 16:39:24.180053 masterfile-0.6.1/
+-rw-r--r--   0 njvack     (501) staff       (20)     1113 2017-08-11 20:55:06.000000 masterfile-0.6.1/LICENSE
+-rw-r--r--   0 njvack     (501) staff       (20)      196 2017-08-11 20:55:06.000000 masterfile-0.6.1/MANIFEST.in
+-rw-r--r--   0 njvack     (501) staff       (20)     4521 2024-05-24 16:39:24.179986 masterfile-0.6.1/PKG-INFO
+-rw-r--r--   0 njvack     (501) staff       (20)     3499 2020-09-24 15:48:33.000000 masterfile-0.6.1/README.md
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-24 16:39:24.168462 masterfile-0.6.1/masterfile/
+-rw-r--r--   0 njvack     (501) staff       (20)      286 2020-09-24 15:48:33.000000 masterfile-0.6.1/masterfile/__init__.py
+-rw-r--r--   0 njvack     (501) staff       (20)      332 2024-05-24 16:38:18.000000 masterfile-0.6.1/masterfile/_metadata.py
+-rw-r--r--   0 njvack     (501) staff       (20)     2512 2020-09-24 15:48:33.000000 masterfile-0.6.1/masterfile/annotator.py
+-rw-r--r--   0 njvack     (501) staff       (20)     4865 2020-09-24 15:48:33.000000 masterfile-0.6.1/masterfile/dictionary.py
+-rw-r--r--   0 njvack     (501) staff       (20)     3965 2021-06-28 19:01:31.000000 masterfile-0.6.1/masterfile/errors.py
+-rw-r--r--   0 njvack     (501) staff       (20)     1385 2020-09-24 15:48:33.000000 masterfile-0.6.1/masterfile/formatters.py
+-rw-r--r--   0 njvack     (501) staff       (20)    10284 2021-06-30 19:33:59.000000 masterfile-0.6.1/masterfile/masterfile.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-24 16:39:24.172381 masterfile-0.6.1/masterfile/scripts/
+-rw-r--r--   0 njvack     (501) staff       (20)        0 2020-09-24 15:48:33.000000 masterfile-0.6.1/masterfile/scripts/__init__.py
+-rw-r--r--   0 njvack     (501) staff       (20)     2055 2020-09-24 15:48:33.000000 masterfile-0.6.1/masterfile/scripts/create.py
+-rw-r--r--   0 njvack     (501) staff       (20)     3827 2024-05-24 16:38:35.000000 masterfile-0.6.1/masterfile/scripts/extract.py
+-rw-r--r--   0 njvack     (501) staff       (20)     1269 2024-05-24 16:38:40.000000 masterfile-0.6.1/masterfile/scripts/join.py
+-rw-r--r--   0 njvack     (501) staff       (20)     4151 2021-06-30 20:46:13.000000 masterfile-0.6.1/masterfile/scripts/masterfile.py
+-rw-r--r--   0 njvack     (501) staff       (20)     3030 2021-06-30 21:34:48.000000 masterfile-0.6.1/masterfile/scripts/pretty.py
+-rw-r--r--   0 njvack     (501) staff       (20)     1511 2020-09-24 15:48:33.000000 masterfile-0.6.1/masterfile/scripts/text_to_dos.py
+-rw-r--r--   0 njvack     (501) staff       (20)     1887 2020-09-24 15:48:33.000000 masterfile-0.6.1/masterfile/scripts/validate.py
+-rw-r--r--   0 njvack     (501) staff       (20)     1341 2020-09-24 15:48:33.000000 masterfile-0.6.1/masterfile/validator.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-24 16:39:24.173717 masterfile-0.6.1/masterfile/validators/
+-rw-r--r--   0 njvack     (501) staff       (20)      192 2020-09-24 15:48:33.000000 masterfile-0.6.1/masterfile/validators/__init__.py
+-rw-r--r--   0 njvack     (501) staff       (20)     2183 2020-09-24 15:48:33.000000 masterfile-0.6.1/masterfile/validators/column_format.py
+-rw-r--r--   0 njvack     (501) staff       (20)     1763 2020-09-24 15:48:33.000000 masterfile-0.6.1/masterfile/validators/components_in_dictionary.py
+-rw-r--r--   0 njvack     (501) staff       (20)      947 2020-09-24 15:48:33.000000 masterfile-0.6.1/masterfile/validators/dictionary_format.py
+-rw-r--r--   0 njvack     (501) staff       (20)     2227 2020-09-24 15:48:33.000000 masterfile-0.6.1/masterfile/validators/duplicate_column.py
+-rw-r--r--   0 njvack     (501) staff       (20)     2788 2020-09-24 15:48:33.000000 masterfile-0.6.1/masterfile/validators/index_column.py
+-rw-r--r--   0 njvack     (501) staff       (20)      754 2020-09-24 15:48:33.000000 masterfile-0.6.1/masterfile/validators/io.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-24 16:39:24.179716 masterfile-0.6.1/masterfile.egg-info/
+-rw-r--r--   0 njvack     (501) staff       (20)     4521 2024-05-24 16:39:24.000000 masterfile-0.6.1/masterfile.egg-info/PKG-INFO
+-rw-rw-r--   0 njvack     (501) staff       (20)     2242 2024-05-24 16:39:24.000000 masterfile-0.6.1/masterfile.egg-info/SOURCES.txt
+-rw-rw-r--   0 njvack     (501) staff       (20)        1 2024-05-24 16:39:24.000000 masterfile-0.6.1/masterfile.egg-info/dependency_links.txt
+-rw-rw-r--   0 njvack     (501) staff       (20)       66 2024-05-24 16:39:24.000000 masterfile-0.6.1/masterfile.egg-info/entry_points.txt
+-rw-rw-r--   0 njvack     (501) staff       (20)        1 2020-05-21 12:40:13.000000 masterfile-0.6.1/masterfile.egg-info/not-zip-safe
+-rw-rw-r--   0 njvack     (501) staff       (20)       36 2024-05-24 16:39:24.000000 masterfile-0.6.1/masterfile.egg-info/requires.txt
+-rw-rw-r--   0 njvack     (501) staff       (20)       17 2024-05-24 16:39:24.000000 masterfile-0.6.1/masterfile.egg-info/top_level.txt
+-rw-r--r--   0 njvack     (501) staff       (20)     1150 2024-05-24 16:39:24.180428 masterfile-0.6.1/setup.cfg
+-rwxr-xr-x   0 njvack     (501) staff       (20)      595 2020-09-24 15:48:33.000000 masterfile-0.6.1/setup.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-24 16:39:24.175458 masterfile-0.6.1/tests/
+-rw-r--r--   0 njvack     (501) staff       (20)       24 2017-08-11 20:55:06.000000 masterfile-0.6.1/tests/__init__.py
+-rw-r--r--   0 njvack     (501) staff       (20)     1762 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/conftest.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-24 16:39:24.175973 masterfile-0.6.1/tests/examples/
+-rw-r--r--   0 njvack     (501) staff       (20)     6148 2017-08-30 18:11:47.000000 masterfile-0.6.1/tests/examples/.DS_Store
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-24 16:39:24.176262 masterfile-0.6.1/tests/examples/baddict/
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-24 16:39:24.176402 masterfile-0.6.1/tests/examples/baddict/dictionary/
+-rw-rw-r--   0 njvack     (501) staff       (20)      105 2020-01-22 15:10:43.000000 masterfile-0.6.1/tests/examples/baddict/dictionary/dictionary.csv
+-rw-rw-r--   0 njvack     (501) staff       (20)      160 2020-01-22 15:10:43.000000 masterfile-0.6.1/tests/examples/baddict/foo.csv
+-rw-r--r--   0 njvack     (501) staff       (20)       74 2021-06-28 19:18:08.000000 masterfile-0.6.1/tests/examples/baddict/settings.yml
+-rw-r--r--   0 njvack     (501) staff       (20)      273 2017-09-01 20:42:57.000000 masterfile-0.6.1/tests/examples/foo_input.csv
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-24 16:39:24.176832 masterfile-0.6.1/tests/examples/good/
+-rw-r--r--   0 njvack     (501) staff       (20)      160 2021-06-30 19:00:55.000000 masterfile-0.6.1/tests/examples/good/bar.csv
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-24 16:39:24.177110 masterfile-0.6.1/tests/examples/good/dictionary/
+-rw-r--r--   0 njvack     (501) staff       (20)      108 2021-07-02 01:41:02.000000 masterfile-0.6.1/tests/examples/good/dictionary/dictionary.csv
+-rw-r--r--   0 njvack     (501) staff       (20)      101 2018-03-14 17:14:31.000000 masterfile-0.6.1/tests/examples/good/dictionary/measure_contacts.csv
+-rw-r--r--   0 njvack     (501) staff       (20)      193 2021-07-02 01:40:58.000000 masterfile-0.6.1/tests/examples/good/foo.csv
+-rw-r--r--   0 njvack     (501) staff       (20)      143 2021-07-02 01:41:31.000000 masterfile-0.6.1/tests/examples/good/settings.yml
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-24 16:39:24.177518 masterfile-0.6.1/tests/examples/problems/
+-rw-r--r--   0 njvack     (501) staff       (20)      119 2018-03-14 17:14:31.000000 masterfile-0.6.1/tests/examples/problems/bar.csv
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-24 16:39:24.177789 masterfile-0.6.1/tests/examples/problems/dictionary/
+-rw-r--r--   0 njvack     (501) staff       (20)      119 2018-03-14 17:14:31.000000 masterfile-0.6.1/tests/examples/problems/dictionary/dictionary.csv
+-rw-r--r--   0 njvack     (501) staff       (20)       28 2018-03-14 17:14:31.000000 masterfile-0.6.1/tests/examples/problems/dictionary/noindex.csv
+-rw-r--r--   0 njvack     (501) staff       (20)      252 2018-03-14 17:14:31.000000 masterfile-0.6.1/tests/examples/problems/foo.csv
+-rw-r--r--   0 njvack     (501) staff       (20)       74 2021-06-28 19:18:04.000000 masterfile-0.6.1/tests/examples/problems/settings.yml
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-24 16:39:24.178552 masterfile-0.6.1/tests/scripts/
+-rw-r--r--   0 njvack     (501) staff       (20)        0 2018-03-14 17:14:31.000000 masterfile-0.6.1/tests/scripts/__init__.py
+-rw-r--r--   0 njvack     (501) staff       (20)     2668 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/scripts/test_extract_masterfile_data.py
+-rw-r--r--   0 njvack     (501) staff       (20)      927 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/scripts/test_make_blank_dictionary.py
+-rw-r--r--   0 njvack     (501) staff       (20)      954 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/scripts/test_make_joined_data.py
+-rw-r--r--   0 njvack     (501) staff       (20)      740 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/scripts/test_make_pretty_dictionary.py
+-rw-r--r--   0 njvack     (501) staff       (20)     1658 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/scripts/test_validate_masterfile.py
+-rw-r--r--   0 njvack     (501) staff       (20)     1667 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/test_annotator.py
+-rw-r--r--   0 njvack     (501) staff       (20)     2412 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/test_dictionary.py
+-rw-r--r--   0 njvack     (501) staff       (20)     1552 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/test_errors.py
+-rw-r--r--   0 njvack     (501) staff       (20)     1338 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/test_formatters.py
+-rw-r--r--   0 njvack     (501) staff       (20)     3235 2021-06-24 21:58:06.000000 masterfile-0.6.1/tests/test_masterfile.py
+-rw-r--r--   0 njvack     (501) staff       (20)     2359 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/test_validator.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-24 16:39:24.179543 masterfile-0.6.1/tests/validators/
+-rw-r--r--   0 njvack     (501) staff       (20)        0 2018-03-14 17:14:31.000000 masterfile-0.6.1/tests/validators/__init__.py
+-rw-r--r--   0 njvack     (501) staff       (20)      947 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/validators/test_column_format.py
+-rw-r--r--   0 njvack     (501) staff       (20)      873 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/validators/test_components_in_dictionary.py
+-rw-r--r--   0 njvack     (501) staff       (20)      788 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/validators/test_dictionary_format.py
+-rw-r--r--   0 njvack     (501) staff       (20)     1748 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/validators/test_duplicate_column.py
+-rw-r--r--   0 njvack     (501) staff       (20)     1330 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/validators/test_index_column.py
+-rw-r--r--   0 njvack     (501) staff       (20)      934 2020-09-24 15:48:33.000000 masterfile-0.6.1/tests/validators/test_io.py
```

### Comparing `masterfile-0.6.0/LICENSE` & `masterfile-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/PKG-INFO` & `masterfile-0.6.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,145 +1,149 @@
 Metadata-Version: 2.1
 Name: masterfile
-Version: 0.6.0
+Version: 0.6.1
 Summary: Tools to organize, document, and validate the variables of interest in scientific studies
 Home-page: https://github.com/uwmadison-chm/masterfile
+Download-URL: https://github.com/uwmadison-chm/masterfile/releases
 Author: Nate Vack
 Author-email: njvack@wisc.edu
 Maintainer: Nate Vack
 Maintainer-email: njvack@wisc.edu
 License: MIT License
-Download-URL: https://github.com/uwmadison-chm/masterfile/releases
-Description: # masterfile
-        
-        [![DOI](https://zenodo.org/badge/100069618.svg)](https://zenodo.org/badge/latestdoi/100069618)
-        
-        ## Tools to organize, document, and validate the variables of interest in scientific studies
-        
-        ## Command line usage
-        
-        `masterfile --help` will list all the subcommands.
-        
-        ### Create
-        
-            masterfile create masterfile_path out_file
-        
-        ### Join
-        
-            masterfile join masterfile_path out_file
-        
-        ### Extract
-        
-            masterfile extract [-s|--skip ROWS] [--index_column COL]
-                                  masterfile_path csv_file out_file
-        
-        ### Validate
-        
-            asterfile validate masterfile_path [file [file ...]]
-        
-        
-        ## Draft API usage example
-        
-        ```python
-        import masterfile
-        # Load all of the .csv files from /path, and the dictionary files in
-        # /path/dictionaries. Takes settings info from a 'settings.json' file in
-        # /path.
-        # joins the .csv files on 'participant_id', which will be used as the index
-        # There will be warnings if the data look bad in some way
-        mf = masterfile.load('/path')
-        # Get the pandas dataframe associated
-        df = mf.dataframe  # aliased as mf.df
-        
-        # All the variable stuff is less important, people can go look in data dicts
-        # So we'll write that stuff later.
-        v = mf.lookup('sr_t1_panas_pa')
-        v.contacts # list_of_names
-        v.measure.contact  # Someone
-        v.modality # Component("self-report")
-        ```
-        
-        ## CSV file format
-        
-        CSV files should be comma-separated (no surprise there) and have DOS line endings (CRLF). They should not have the stupid UTF-8 signature at the start. UTF-8 characters are fine. Missing data is indicated by an empty cell. Quoting should be like Excel does.
-        
-        Basically, you want Excel-for-Windows-style CSV files with no UTF-8 signature.
-        
-        ## Dictionaries
-        
-        * CSV format
-        * Has AT LEAST two columns: component, short_name
-        * Those are the indexes
-        * There shouldn't be any repeats in the index
-        * The settings.json file should contain a "components" thing that says what should exist in the component column
-        * Things with blank component are ignored (TODO: Maybe?)
-        
-        
-        ## Exclusion files
-        
-        * CSV format
-        * Live in exclusions/
-        * One row per ppt, one column per value
-        * Has index column, same as data file
-        * Blanks mean "Use this value," nonblanks mean "exclude this value"
-        * Things in the cells may be codes; these codes may be defined in settings.json
-        * If data is excluded for more than one reason, separate codes with ","
-        * Not all rows / columns in masterfiles need to be included in exclusion files. Missing rows / columns are treated like blank values.
-        
-        
-        ## Data checks
-        
-        Here are some (all?) of the things to do to verify you have semantically reasonable data:
-        
-        * Variable parts not in dictionaries
-        * Missing participant_id column
-        * Repeated paticipant_id column
-        * Blanks in participant_id column
-        * Duplicate columns
-        * Column names not matching format
-        
-        ## Getting started for development
-        
-        Create a virtualenv:
-        
-            virtualenv ~/env/masterfile
-            source ~/env/masterfile/bin/activate
-        
-        Install the requirements and this module for development:
-        
-            pip install -r requirements_dev.txt
-            pip install -e .
-        
-        Run tests:
-        
-            pytest
-        
-        Run tests across all supported Python versions:
-        
-            tox
-        
-        To run in a specific python version:
-        
-            tox -e py37
-        
-        ## Credits
-        
-        Written by Nate Vack <njvack@wisc.edu> with help from Dan Fitch <dfitch@wisc.edu>
-        
-        masterfile packages some wonderful tools: [schema](https://github.com/halst/schema) and [attrs](https://github.com/python-attrs/attrs).
-        
-        schema is copyright (c) 2012 Vladimir Keleshev, vladimir@keleshev.com
-        
-        attrs is copyright (c) 2015 Hynek Schlawack
-        
 Keywords: science research data library
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Provides: masterfile
 Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+Requires-Dist: pandas>=0.9
+Requires-Dist: attrs>=17.0
+Requires-Dist: schema>=0.2
+
+# masterfile
+
+[![DOI](https://zenodo.org/badge/100069618.svg)](https://zenodo.org/badge/latestdoi/100069618)
+
+## Tools to organize, document, and validate the variables of interest in scientific studies
+
+## Command line usage
+
+`masterfile --help` will list all the subcommands.
+
+### Create
+
+    masterfile create masterfile_path out_file
+
+### Join
+
+    masterfile join masterfile_path out_file
+
+### Extract
+
+    masterfile extract [-s|--skip ROWS] [--index_column COL]
+                          masterfile_path csv_file out_file
+
+### Validate
+
+    asterfile validate masterfile_path [file [file ...]]
+
+
+## Draft API usage example
+
+```python
+import masterfile
+# Load all of the .csv files from /path, and the dictionary files in
+# /path/dictionaries. Takes settings info from a 'settings.json' file in
+# /path.
+# joins the .csv files on 'participant_id', which will be used as the index
+# There will be warnings if the data look bad in some way
+mf = masterfile.load('/path')
+# Get the pandas dataframe associated
+df = mf.dataframe  # aliased as mf.df
+
+# All the variable stuff is less important, people can go look in data dicts
+# So we'll write that stuff later.
+v = mf.lookup('sr_t1_panas_pa')
+v.contacts # list_of_names
+v.measure.contact  # Someone
+v.modality # Component("self-report")
+```
+
+## CSV file format
+
+CSV files should be comma-separated (no surprise there) and have DOS line endings (CRLF). They should not have the stupid UTF-8 signature at the start. UTF-8 characters are fine. Missing data is indicated by an empty cell. Quoting should be like Excel does.
+
+Basically, you want Excel-for-Windows-style CSV files with no UTF-8 signature.
+
+## Dictionaries
+
+* CSV format
+* Has AT LEAST two columns: component, short_name
+* Those are the indexes
+* There shouldn't be any repeats in the index
+* The settings.json file should contain a "components" thing that says what should exist in the component column
+* Things with blank component are ignored (TODO: Maybe?)
+
+
+## Exclusion files
+
+* CSV format
+* Live in exclusions/
+* One row per ppt, one column per value
+* Has index column, same as data file
+* Blanks mean "Use this value," nonblanks mean "exclude this value"
+* Things in the cells may be codes; these codes may be defined in settings.json
+* If data is excluded for more than one reason, separate codes with ","
+* Not all rows / columns in masterfiles need to be included in exclusion files. Missing rows / columns are treated like blank values.
+
+
+## Data checks
+
+Here are some (all?) of the things to do to verify you have semantically reasonable data:
+
+* Variable parts not in dictionaries
+* Missing participant_id column
+* Repeated paticipant_id column
+* Blanks in participant_id column
+* Duplicate columns
+* Column names not matching format
+
+## Getting started for development
+
+Create a virtualenv:
+
+    virtualenv ~/env/masterfile
+    source ~/env/masterfile/bin/activate
+
+Install the requirements and this module for development:
+
+    pip install -r requirements_dev.txt
+    pip install -e .
+
+Run tests:
+
+    pytest
+
+Run tests across all supported Python versions:
+
+    tox
+
+To run in a specific python version:
+
+    tox -e py37
+
+## Credits
+
+Written by Nate Vack <njvack@wisc.edu> with help from Dan Fitch <dfitch@wisc.edu>
+
+masterfile packages some wonderful tools: [schema](https://github.com/halst/schema) and [attrs](https://github.com/python-attrs/attrs).
+
+schema is copyright (c) 2012 Vladimir Keleshev, vladimir@keleshev.com
+
+attrs is copyright (c) 2015 Hynek Schlawack
```

### Comparing `masterfile-0.6.0/README.md` & `masterfile-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/annotator.py` & `masterfile-0.6.1/masterfile/annotator.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/dictionary.py` & `masterfile-0.6.1/masterfile/dictionary.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/errors.py` & `masterfile-0.6.1/masterfile/errors.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/formatters.py` & `masterfile-0.6.1/masterfile/formatters.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/masterfile.py` & `masterfile-0.6.1/masterfile/masterfile.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/scripts/create.py` & `masterfile-0.6.1/masterfile/scripts/create.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/scripts/extract.py` & `masterfile-0.6.1/masterfile/scripts/extract.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,87 +30,85 @@
 from contextlib import contextmanager
 
 import pandas as pd
 
 from masterfile.masterfile import LINE_ENDING
 from masterfile.masterfile import Masterfile
 
-logging.basicConfig(level=logging.DEBUG, format='%(message)s')
+logging.basicConfig(level=logging.DEBUG, format="%(message)s")
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 
 
 def main(args):
     import os
+
     os.linesep = "\r\n"
     if args.verbose:
         logger.setLevel(logging.DEBUG)
     logger.debug(args)
     df = pd.read_csv(args.csv_file, dtype=str, na_filter=False)
     mf = Masterfile.find_settings_file_and_construct(args.masterfile_path)
     extract_index_col = args.index_column
     if extract_index_col is None or extract_index_col.strip() == "":
         extract_index_col = mf.index_column
 
-    formatted = format_dataframe_for_masterfile(
-        df, mf, extract_index_col, args.skip)
+    formatted = format_dataframe_for_masterfile(df, mf, extract_index_col, args.skip)
     with file_or_stdout(args.out_file) as output:
-        formatted.to_csv(output, line_terminator=LINE_ENDING)
+        formatted.to_csv(output, lineterminator=LINE_ENDING)
 
 
 @contextmanager
 def file_or_stdout(filename):
-    if filename == '-':
-        logger.info('Writing to stdout')
+    if filename == "-":
+        logger.info("Writing to stdout")
         yield sys.stdout
     else:
-        with open(filename, 'w') as f:
-            logger.info('Writing to {}'.format(filename))
+        with open(filename, "w") as f:
+            logger.info("Writing to {}".format(filename))
             yield f
 
 
 def format_dataframe_for_masterfile(df, mf, input_index_col, skip_rows):
     """
     Return a copy of df, with:
     * input_index_col renamed to mf.index_col
     * index_col as the first column
     * only the columns that match the format (c1_c2_..._cN) included
     * rows with index_col as blank excluded
     """
     index_col = mf.index_column
-    logger.debug('Original columns: {}'.format(df.columns))
-    logger.debug('Original has {} rows'.format(len(df)))
+    logger.debug("Original columns: {}".format(df.columns))
+    logger.debug("Original has {} rows".format(len(df)))
     col_rx = col_match_regex(mf, input_index_col)
-    logger.debug('Column regex: {}'.format(col_rx))
+    logger.debug("Column regex: {}".format(col_rx))
     col_filtered = df.filter(regex=col_rx)
     row_filtered = _filter_rows(col_filtered, input_index_col, skip_rows)
-    logger.debug('Now has {} rows'.format(len(row_filtered)))
+    logger.debug("Now has {} rows".format(len(row_filtered)))
     renamed = row_filtered.rename(columns={input_index_col: index_col})
     renamed.set_index(index_col, inplace=True)
-    logger.debug('New columns: {}'.format(renamed.columns))
+    logger.debug("New columns: {}".format(renamed.columns))
     return renamed
 
 
 def _filter_rows(df, index_col, skip_rows):
     skipped = df[skip_rows:]
-    has_data = ~(
-        (skipped[index_col].str.strip() == '') |
-        (skipped[index_col].isnull())
-    )
+    has_data = ~((skipped[index_col].str.strip() == "") | (skipped[index_col].isnull()))
     return skipped[has_data]
 
 
 def col_match_regex(mf, input_index_col):
     index_col = input_index_col or mf.index_column
-    return '(^{}$)|(^{}$)'.format(
-        re.escape(index_col), component_col_regex(len(mf.components)))
+    return "(^{}$)|(^{}$)".format(
+        re.escape(index_col), component_col_regex(len(mf.components))
+    )
 
 
 def component_col_regex(component_count):
     """
     Match things like 'foo_bar_baz_corge'
     """
-    return '_'.join(([r'[^_\s]+'] * component_count))
+    return "_".join(([r"[^_\s]+"] * component_count))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `masterfile-0.6.0/masterfile/scripts/join.py` & `masterfile-0.6.1/masterfile/scripts/join.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,31 +17,31 @@
 
 import sys
 
 import masterfile
 from masterfile.masterfile import LINE_ENDING
 
 import logging
-logging.basicConfig(level=logging.DEBUG, format='%(message)s')
+
+logging.basicConfig(level=logging.DEBUG, format="%(message)s")
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 
 
 def make_joined_data(masterfile_path, output_file):
     mf = masterfile.load(masterfile_path)
-    mf.dataframe.to_csv(output_file, line_terminator=LINE_ENDING)
+    mf.dataframe.to_csv(output_file, lineterminator=LINE_ENDING)
     return 0
 
 
 def main(args):
     if args.verbose:
         logger.setLevel(logging.DEBUG)
     logger.debug(args)
     output = args.out_file
-    if output == '-':
-        logger.info("stdout")
+    if output == "-":
         output = sys.stdout
     return make_joined_data(args.masterfile_path, output)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `masterfile-0.6.0/masterfile/scripts/masterfile.py` & `masterfile-0.6.1/masterfile/scripts/masterfile.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/scripts/pretty.py` & `masterfile-0.6.1/masterfile/scripts/pretty.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/scripts/text_to_dos.py` & `masterfile-0.6.1/masterfile/scripts/text_to_dos.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/scripts/validate.py` & `masterfile-0.6.1/masterfile/scripts/validate.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/validator.py` & `masterfile-0.6.1/masterfile/validator.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/validators/column_format.py` & `masterfile-0.6.1/masterfile/validators/column_format.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/validators/components_in_dictionary.py` & `masterfile-0.6.1/masterfile/validators/components_in_dictionary.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/validators/dictionary_format.py` & `masterfile-0.6.1/masterfile/validators/dictionary_format.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/validators/duplicate_column.py` & `masterfile-0.6.1/masterfile/validators/duplicate_column.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/validators/index_column.py` & `masterfile-0.6.1/masterfile/validators/index_column.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile/validators/io.py` & `masterfile-0.6.1/masterfile/validators/io.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/masterfile.egg-info/PKG-INFO` & `masterfile-0.6.1/masterfile.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,145 +1,149 @@
 Metadata-Version: 2.1
 Name: masterfile
-Version: 0.6.0
+Version: 0.6.1
 Summary: Tools to organize, document, and validate the variables of interest in scientific studies
 Home-page: https://github.com/uwmadison-chm/masterfile
+Download-URL: https://github.com/uwmadison-chm/masterfile/releases
 Author: Nate Vack
 Author-email: njvack@wisc.edu
 Maintainer: Nate Vack
 Maintainer-email: njvack@wisc.edu
 License: MIT License
-Download-URL: https://github.com/uwmadison-chm/masterfile/releases
-Description: # masterfile
-        
-        [![DOI](https://zenodo.org/badge/100069618.svg)](https://zenodo.org/badge/latestdoi/100069618)
-        
-        ## Tools to organize, document, and validate the variables of interest in scientific studies
-        
-        ## Command line usage
-        
-        `masterfile --help` will list all the subcommands.
-        
-        ### Create
-        
-            masterfile create masterfile_path out_file
-        
-        ### Join
-        
-            masterfile join masterfile_path out_file
-        
-        ### Extract
-        
-            masterfile extract [-s|--skip ROWS] [--index_column COL]
-                                  masterfile_path csv_file out_file
-        
-        ### Validate
-        
-            asterfile validate masterfile_path [file [file ...]]
-        
-        
-        ## Draft API usage example
-        
-        ```python
-        import masterfile
-        # Load all of the .csv files from /path, and the dictionary files in
-        # /path/dictionaries. Takes settings info from a 'settings.json' file in
-        # /path.
-        # joins the .csv files on 'participant_id', which will be used as the index
-        # There will be warnings if the data look bad in some way
-        mf = masterfile.load('/path')
-        # Get the pandas dataframe associated
-        df = mf.dataframe  # aliased as mf.df
-        
-        # All the variable stuff is less important, people can go look in data dicts
-        # So we'll write that stuff later.
-        v = mf.lookup('sr_t1_panas_pa')
-        v.contacts # list_of_names
-        v.measure.contact  # Someone
-        v.modality # Component("self-report")
-        ```
-        
-        ## CSV file format
-        
-        CSV files should be comma-separated (no surprise there) and have DOS line endings (CRLF). They should not have the stupid UTF-8 signature at the start. UTF-8 characters are fine. Missing data is indicated by an empty cell. Quoting should be like Excel does.
-        
-        Basically, you want Excel-for-Windows-style CSV files with no UTF-8 signature.
-        
-        ## Dictionaries
-        
-        * CSV format
-        * Has AT LEAST two columns: component, short_name
-        * Those are the indexes
-        * There shouldn't be any repeats in the index
-        * The settings.json file should contain a "components" thing that says what should exist in the component column
-        * Things with blank component are ignored (TODO: Maybe?)
-        
-        
-        ## Exclusion files
-        
-        * CSV format
-        * Live in exclusions/
-        * One row per ppt, one column per value
-        * Has index column, same as data file
-        * Blanks mean "Use this value," nonblanks mean "exclude this value"
-        * Things in the cells may be codes; these codes may be defined in settings.json
-        * If data is excluded for more than one reason, separate codes with ","
-        * Not all rows / columns in masterfiles need to be included in exclusion files. Missing rows / columns are treated like blank values.
-        
-        
-        ## Data checks
-        
-        Here are some (all?) of the things to do to verify you have semantically reasonable data:
-        
-        * Variable parts not in dictionaries
-        * Missing participant_id column
-        * Repeated paticipant_id column
-        * Blanks in participant_id column
-        * Duplicate columns
-        * Column names not matching format
-        
-        ## Getting started for development
-        
-        Create a virtualenv:
-        
-            virtualenv ~/env/masterfile
-            source ~/env/masterfile/bin/activate
-        
-        Install the requirements and this module for development:
-        
-            pip install -r requirements_dev.txt
-            pip install -e .
-        
-        Run tests:
-        
-            pytest
-        
-        Run tests across all supported Python versions:
-        
-            tox
-        
-        To run in a specific python version:
-        
-            tox -e py37
-        
-        ## Credits
-        
-        Written by Nate Vack <njvack@wisc.edu> with help from Dan Fitch <dfitch@wisc.edu>
-        
-        masterfile packages some wonderful tools: [schema](https://github.com/halst/schema) and [attrs](https://github.com/python-attrs/attrs).
-        
-        schema is copyright (c) 2012 Vladimir Keleshev, vladimir@keleshev.com
-        
-        attrs is copyright (c) 2015 Hynek Schlawack
-        
 Keywords: science research data library
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Provides: masterfile
 Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+Requires-Dist: pandas>=0.9
+Requires-Dist: attrs>=17.0
+Requires-Dist: schema>=0.2
+
+# masterfile
+
+[![DOI](https://zenodo.org/badge/100069618.svg)](https://zenodo.org/badge/latestdoi/100069618)
+
+## Tools to organize, document, and validate the variables of interest in scientific studies
+
+## Command line usage
+
+`masterfile --help` will list all the subcommands.
+
+### Create
+
+    masterfile create masterfile_path out_file
+
+### Join
+
+    masterfile join masterfile_path out_file
+
+### Extract
+
+    masterfile extract [-s|--skip ROWS] [--index_column COL]
+                          masterfile_path csv_file out_file
+
+### Validate
+
+    asterfile validate masterfile_path [file [file ...]]
+
+
+## Draft API usage example
+
+```python
+import masterfile
+# Load all of the .csv files from /path, and the dictionary files in
+# /path/dictionaries. Takes settings info from a 'settings.json' file in
+# /path.
+# joins the .csv files on 'participant_id', which will be used as the index
+# There will be warnings if the data look bad in some way
+mf = masterfile.load('/path')
+# Get the pandas dataframe associated
+df = mf.dataframe  # aliased as mf.df
+
+# All the variable stuff is less important, people can go look in data dicts
+# So we'll write that stuff later.
+v = mf.lookup('sr_t1_panas_pa')
+v.contacts # list_of_names
+v.measure.contact  # Someone
+v.modality # Component("self-report")
+```
+
+## CSV file format
+
+CSV files should be comma-separated (no surprise there) and have DOS line endings (CRLF). They should not have the stupid UTF-8 signature at the start. UTF-8 characters are fine. Missing data is indicated by an empty cell. Quoting should be like Excel does.
+
+Basically, you want Excel-for-Windows-style CSV files with no UTF-8 signature.
+
+## Dictionaries
+
+* CSV format
+* Has AT LEAST two columns: component, short_name
+* Those are the indexes
+* There shouldn't be any repeats in the index
+* The settings.json file should contain a "components" thing that says what should exist in the component column
+* Things with blank component are ignored (TODO: Maybe?)
+
+
+## Exclusion files
+
+* CSV format
+* Live in exclusions/
+* One row per ppt, one column per value
+* Has index column, same as data file
+* Blanks mean "Use this value," nonblanks mean "exclude this value"
+* Things in the cells may be codes; these codes may be defined in settings.json
+* If data is excluded for more than one reason, separate codes with ","
+* Not all rows / columns in masterfiles need to be included in exclusion files. Missing rows / columns are treated like blank values.
+
+
+## Data checks
+
+Here are some (all?) of the things to do to verify you have semantically reasonable data:
+
+* Variable parts not in dictionaries
+* Missing participant_id column
+* Repeated paticipant_id column
+* Blanks in participant_id column
+* Duplicate columns
+* Column names not matching format
+
+## Getting started for development
+
+Create a virtualenv:
+
+    virtualenv ~/env/masterfile
+    source ~/env/masterfile/bin/activate
+
+Install the requirements and this module for development:
+
+    pip install -r requirements_dev.txt
+    pip install -e .
+
+Run tests:
+
+    pytest
+
+Run tests across all supported Python versions:
+
+    tox
+
+To run in a specific python version:
+
+    tox -e py37
+
+## Credits
+
+Written by Nate Vack <njvack@wisc.edu> with help from Dan Fitch <dfitch@wisc.edu>
+
+masterfile packages some wonderful tools: [schema](https://github.com/halst/schema) and [attrs](https://github.com/python-attrs/attrs).
+
+schema is copyright (c) 2012 Vladimir Keleshev, vladimir@keleshev.com
+
+attrs is copyright (c) 2015 Hynek Schlawack
```

### Comparing `masterfile-0.6.0/masterfile.egg-info/SOURCES.txt` & `masterfile-0.6.1/masterfile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/setup.cfg` & `masterfile-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/setup.py` & `masterfile-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/conftest.py` & `masterfile-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/examples/.DS_Store` & `masterfile-0.6.1/tests/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/scripts/test_extract_masterfile_data.py` & `masterfile-0.6.1/tests/scripts/test_extract_masterfile_data.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/scripts/test_make_blank_dictionary.py` & `masterfile-0.6.1/tests/scripts/test_make_blank_dictionary.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/scripts/test_make_joined_data.py` & `masterfile-0.6.1/tests/scripts/test_make_joined_data.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/scripts/test_make_pretty_dictionary.py` & `masterfile-0.6.1/tests/scripts/test_make_pretty_dictionary.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/scripts/test_validate_masterfile.py` & `masterfile-0.6.1/tests/scripts/test_validate_masterfile.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/test_annotator.py` & `masterfile-0.6.1/tests/test_annotator.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/test_dictionary.py` & `masterfile-0.6.1/tests/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/test_errors.py` & `masterfile-0.6.1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/test_formatters.py` & `masterfile-0.6.1/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/test_masterfile.py` & `masterfile-0.6.1/tests/test_masterfile.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/test_validator.py` & `masterfile-0.6.1/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/validators/test_column_format.py` & `masterfile-0.6.1/tests/validators/test_column_format.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/validators/test_components_in_dictionary.py` & `masterfile-0.6.1/tests/validators/test_components_in_dictionary.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/validators/test_dictionary_format.py` & `masterfile-0.6.1/tests/validators/test_dictionary_format.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/validators/test_duplicate_column.py` & `masterfile-0.6.1/tests/validators/test_duplicate_column.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/validators/test_index_column.py` & `masterfile-0.6.1/tests/validators/test_index_column.py`

 * *Files identical despite different names*

### Comparing `masterfile-0.6.0/tests/validators/test_io.py` & `masterfile-0.6.1/tests/validators/test_io.py`

 * *Files identical despite different names*

