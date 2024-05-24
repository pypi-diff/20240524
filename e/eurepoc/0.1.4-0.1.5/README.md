# Comparing `tmp/eurepoc-0.1.4.tar.gz` & `tmp/eurepoc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurepoc-0.1.4.tar", last modified: Sun May 19 11:33:13 2024, max compression
+gzip compressed data, was "eurepoc-0.1.5.tar", last modified: Fri May 24 09:28:13 2024, max compression
```

## Comparing `eurepoc-0.1.4.tar` & `eurepoc-0.1.5.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-19 11:33:13.803586 eurepoc-0.1.4/
--rw-r--r--   0 camille    (501) staff       (20)     1068 2024-05-18 11:49:09.000000 eurepoc-0.1.4/LICENSE
--rw-r--r--   0 camille    (501) staff       (20)      310 2024-05-18 11:42:32.000000 eurepoc-0.1.4/MANIFEST.in
--rw-r--r--   0 camille    (501) staff       (20)     1951 2024-05-19 11:33:13.802293 eurepoc-0.1.4/PKG-INFO
--rw-r--r--   0 camille    (501) staff       (20)     1333 2024-05-19 11:00:11.000000 eurepoc-0.1.4/README.md
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-19 11:33:13.593963 eurepoc-0.1.4/docs/
--rw-r--r--   0 camille    (501) staff       (20)      638 2024-05-17 13:41:39.000000 eurepoc-0.1.4/docs/Makefile
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-19 11:33:13.630110 eurepoc-0.1.4/docs/build/
--rw-r--r--   0 camille    (501) staff       (20)      230 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/.buildinfo
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-19 11:33:13.655497 eurepoc-0.1.4/docs/build/.doctrees/
--rw-r--r--   0 camille    (501) staff       (20)    26530 2024-05-19 11:20:40.000000 eurepoc-0.1.4/docs/build/.doctrees/DatabaseQuery.doctree
--rw-r--r--   0 camille    (501) staff       (20)    53689 2024-05-19 11:20:40.000000 eurepoc-0.1.4/docs/build/.doctrees/IncidentDataFrameGenerator.doctree
--rw-r--r--   0 camille    (501) staff       (20)     4978 2024-05-19 11:20:40.000000 eurepoc-0.1.4/docs/build/.doctrees/date_type.doctree
--rw-r--r--   0 camille    (501) staff       (20)   363639 2024-05-19 11:20:40.000000 eurepoc-0.1.4/docs/build/.doctrees/environment.pickle
--rw-r--r--   0 camille    (501) staff       (20)     2438 2024-05-19 11:20:40.000000 eurepoc-0.1.4/docs/build/.doctrees/flag_type.doctree
--rw-r--r--   0 camille    (501) staff       (20)     8544 2024-05-19 11:20:40.000000 eurepoc-0.1.4/docs/build/.doctrees/index.doctree
--rw-r--r--   0 camille    (501) staff       (20)    52464 2024-05-19 11:20:40.000000 eurepoc-0.1.4/docs/build/.doctrees/initiator_country.doctree
--rw-r--r--   0 camille    (501) staff       (20)     9218 2024-05-19 11:20:40.000000 eurepoc-0.1.4/docs/build/.doctrees/read_token.doctree
--rw-r--r--   0 camille    (501) staff       (20)     6564 2024-05-19 11:20:40.000000 eurepoc-0.1.4/docs/build/.doctrees/receiver_category.doctree
--rw-r--r--   0 camille    (501) staff       (20)    52411 2024-05-19 11:20:40.000000 eurepoc-0.1.4/docs/build/.doctrees/receiver_country.doctree
--rw-r--r--   0 camille    (501) staff       (20)    13421 2024-05-19 11:20:40.000000 eurepoc-0.1.4/docs/build/.doctrees/receiver_region.doctree
--rw-r--r--   0 camille    (501) staff       (20)    18434 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/DatabaseQuery.html
--rw-r--r--   0 camille    (501) staff       (20)    42047 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/IncidentDataFrameGenerator.html
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-19 11:33:13.657389 eurepoc-0.1.4/docs/build/_modules/
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-19 11:33:13.660954 eurepoc-0.1.4/docs/build/_modules/eurepoc/
--rw-r--r--   0 camille    (501) staff       (20)    19498 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/_modules/eurepoc/database_query.html
--rw-r--r--   0 camille    (501) staff       (20)    47913 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/_modules/eurepoc/incident_dataframes.html
--rw-r--r--   0 camille    (501) staff       (20)    12207 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/_modules/eurepoc/read_token.html
--rw-r--r--   0 camille    (501) staff       (20)     9226 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/_modules/index.html
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-19 11:33:13.688542 eurepoc-0.1.4/docs/build/_sources/
--rw-r--r--   0 camille    (501) staff       (20)      592 2024-05-19 11:13:05.000000 eurepoc-0.1.4/docs/build/_sources/DatabaseQuery.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)      307 2024-05-19 11:20:25.000000 eurepoc-0.1.4/docs/build/_sources/IncidentDataFrameGenerator.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)      580 2024-05-18 11:23:56.000000 eurepoc-0.1.4/docs/build/_sources/date_type.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)       19 2024-05-18 10:46:49.000000 eurepoc-0.1.4/docs/build/_sources/flag_type.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)     1843 2024-05-19 11:01:08.000000 eurepoc-0.1.4/docs/build/_sources/index.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)     4085 2024-05-18 11:09:52.000000 eurepoc-0.1.4/docs/build/_sources/initiator_country.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)      112 2024-05-18 13:45:23.000000 eurepoc-0.1.4/docs/build/_sources/read_token.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)      708 2024-05-18 11:23:56.000000 eurepoc-0.1.4/docs/build/_sources/receiver_category.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)     4059 2024-05-18 11:09:52.000000 eurepoc-0.1.4/docs/build/_sources/receiver_country.rst.txt
--rw-r--r--   0 camille    (501) staff       (20)      980 2024-05-18 11:23:56.000000 eurepoc-0.1.4/docs/build/_sources/receiver_region.rst.txt
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-19 11:33:13.746363 eurepoc-0.1.4/docs/build/_static/
--rw-r--r--   0 camille    (501) staff       (20)    15094 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/_static/basic.css
--rw-r--r--   0 camille    (501) staff       (20)     4913 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/_static/classic.css
--rw-r--r--   0 camille    (501) staff       (20)     3508 2024-05-17 15:45:22.000000 eurepoc-0.1.4/docs/build/_static/copybutton.js
--rw-r--r--   0 camille    (501) staff       (20)       28 2024-05-17 13:40:31.000000 eurepoc-0.1.4/docs/build/_static/default.css
--rw-r--r--   0 camille    (501) staff       (20)     4472 2024-05-17 13:40:31.000000 eurepoc-0.1.4/docs/build/_static/doctools.js
--rw-r--r--   0 camille    (501) staff       (20)      328 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/_static/documentation_options.js
--rw-r--r--   0 camille    (501) staff       (20)      286 2024-05-17 13:40:31.000000 eurepoc-0.1.4/docs/build/_static/file.png
--rw-r--r--   0 camille    (501) staff       (20)     4758 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/_static/language_data.js
--rw-r--r--   0 camille    (501) staff       (20)     2137 2024-05-17 15:45:22.000000 eurepoc-0.1.4/docs/build/_static/menu.js
--rw-r--r--   0 camille    (501) staff       (20)       90 2024-05-17 13:40:31.000000 eurepoc-0.1.4/docs/build/_static/minus.png
--rw-r--r--   0 camille    (501) staff       (20)       90 2024-05-17 13:40:31.000000 eurepoc-0.1.4/docs/build/_static/plus.png
--rw-r--r--   0 camille    (501) staff       (20)      695 2024-05-17 15:45:22.000000 eurepoc-0.1.4/docs/build/_static/py.png
--rw-r--r--   0 camille    (501) staff       (20)     2041 2024-05-17 15:45:22.000000 eurepoc-0.1.4/docs/build/_static/py.svg
--rw-r--r--   0 camille    (501) staff       (20)    13101 2024-05-17 15:45:22.000000 eurepoc-0.1.4/docs/build/_static/pydoctheme.css
--rw-r--r--   0 camille    (501) staff       (20)     2371 2024-05-17 15:45:22.000000 eurepoc-0.1.4/docs/build/_static/pydoctheme_dark.css
--rw-r--r--   0 camille    (501) staff       (20)     4902 2024-05-19 11:20:40.000000 eurepoc-0.1.4/docs/build/_static/pygments.css
--rw-r--r--   0 camille    (501) staff       (20)     5055 2024-05-19 11:20:40.000000 eurepoc-0.1.4/docs/build/_static/pygments_dark.css
--rw-r--r--   0 camille    (501) staff       (20)      559 2024-05-17 15:45:22.000000 eurepoc-0.1.4/docs/build/_static/search-focus.js
--rw-r--r--   0 camille    (501) staff       (20)    20731 2024-05-17 13:40:31.000000 eurepoc-0.1.4/docs/build/_static/searchtools.js
--rw-r--r--   0 camille    (501) staff       (20)     2617 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/_static/sidebar.js
--rw-r--r--   0 camille    (501) staff       (20)     5123 2024-05-17 13:40:31.000000 eurepoc-0.1.4/docs/build/_static/sphinx_highlight.js
--rw-r--r--   0 camille    (501) staff       (20)      779 2024-05-17 15:45:22.000000 eurepoc-0.1.4/docs/build/_static/themetoggle.js
--rw-r--r--   0 camille    (501) staff       (20)    11699 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/date_type.html
--rw-r--r--   0 camille    (501) staff       (20)    11079 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/flag_type.html
--rw-r--r--   0 camille    (501) staff       (20)    16596 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/genindex.html
--rw-r--r--   0 camille    (501) staff       (20)    15261 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/index.html
--rw-r--r--   0 camille    (501) staff       (20)    18852 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/initiator_country.html
--rw-r--r--   0 camille    (501) staff       (20)      683 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/objects.inv
--rw-r--r--   0 camille    (501) staff       (20)    10062 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/py-modindex.html
--rw-r--r--   0 camille    (501) staff       (20)    13325 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/read_token.html
--rw-r--r--   0 camille    (501) staff       (20)    12144 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/receiver_category.html
--rw-r--r--   0 camille    (501) staff       (20)    18880 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/receiver_country.html
--rw-r--r--   0 camille    (501) staff       (20)    12935 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/receiver_region.html
--rw-r--r--   0 camille    (501) staff       (20)     7117 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/search.html
--rw-r--r--   0 camille    (501) staff       (20)    21668 2024-05-19 11:20:41.000000 eurepoc-0.1.4/docs/build/searchindex.js
--rw-r--r--   0 camille    (501) staff       (20)      804 2024-05-17 13:41:39.000000 eurepoc-0.1.4/docs/make.bat
--rw-r--r--   0 camille    (501) staff       (20)       66 2024-05-19 11:05:40.000000 eurepoc-0.1.4/docs/requirements.txt
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-19 11:33:13.772828 eurepoc-0.1.4/docs/source/
--rw-r--r--   0 camille    (501) staff       (20)      592 2024-05-19 11:13:05.000000 eurepoc-0.1.4/docs/source/DatabaseQuery.rst
--rw-r--r--   0 camille    (501) staff       (20)      307 2024-05-19 11:20:25.000000 eurepoc-0.1.4/docs/source/IncidentDataFrameGenerator.rst
--rw-r--r--   0 camille    (501) staff       (20)      917 2024-05-19 11:10:24.000000 eurepoc-0.1.4/docs/source/conf.py
--rw-r--r--   0 camille    (501) staff       (20)      580 2024-05-18 11:23:56.000000 eurepoc-0.1.4/docs/source/date_type.rst
--rw-r--r--   0 camille    (501) staff       (20)       19 2024-05-18 10:46:49.000000 eurepoc-0.1.4/docs/source/flag_type.rst
--rw-r--r--   0 camille    (501) staff       (20)     1843 2024-05-19 11:01:08.000000 eurepoc-0.1.4/docs/source/index.rst
--rw-r--r--   0 camille    (501) staff       (20)     4085 2024-05-18 11:09:52.000000 eurepoc-0.1.4/docs/source/initiator_country.rst
--rw-r--r--   0 camille    (501) staff       (20)      112 2024-05-18 13:45:23.000000 eurepoc-0.1.4/docs/source/read_token.rst
--rw-r--r--   0 camille    (501) staff       (20)      708 2024-05-18 11:23:56.000000 eurepoc-0.1.4/docs/source/receiver_category.rst
--rw-r--r--   0 camille    (501) staff       (20)     4059 2024-05-18 11:09:52.000000 eurepoc-0.1.4/docs/source/receiver_country.rst
--rw-r--r--   0 camille    (501) staff       (20)      980 2024-05-18 11:23:56.000000 eurepoc-0.1.4/docs/source/receiver_region.rst
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-19 11:33:13.788345 eurepoc-0.1.4/eurepoc/
--rw-r--r--   0 camille    (501) staff       (20)      254 2024-05-19 11:00:11.000000 eurepoc-0.1.4/eurepoc/__init__.py
--rw-r--r--   0 camille    (501) staff       (20)    36013 2024-05-18 10:16:25.000000 eurepoc-0.1.4/eurepoc/data_cleaning_utils.py
--rw-r--r--   0 camille    (501) staff       (20)     9265 2024-05-17 12:10:59.000000 eurepoc-0.1.4/eurepoc/data_query_utils.py
--rw-r--r--   0 camille    (501) staff       (20)     3289 2024-05-19 11:00:11.000000 eurepoc-0.1.4/eurepoc/database_query.py
--rw-r--r--   0 camille    (501) staff       (20)    10816 2024-05-19 11:00:11.000000 eurepoc-0.1.4/eurepoc/incident_dataframes.py
--rw-r--r--   0 camille    (501) staff       (20)      924 2024-05-18 10:24:49.000000 eurepoc-0.1.4/eurepoc/read_token.py
--rw-r--r--   0 camille    (501) staff       (20)     8832 2024-05-17 09:56:40.000000 eurepoc-0.1.4/eurepoc/table_models.py
--rw-r--r--   0 camille    (501) staff       (20)    31942 2024-05-19 11:00:11.000000 eurepoc-0.1.4/eurepoc/tables.py
-drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-19 11:33:13.797402 eurepoc-0.1.4/eurepoc.egg-info/
--rw-r--r--   0 camille    (501) staff       (20)     1951 2024-05-19 11:33:13.000000 eurepoc-0.1.4/eurepoc.egg-info/PKG-INFO
--rw-r--r--   0 camille    (501) staff       (20)     3016 2024-05-19 11:33:13.000000 eurepoc-0.1.4/eurepoc.egg-info/SOURCES.txt
--rw-r--r--   0 camille    (501) staff       (20)        1 2024-05-19 11:33:13.000000 eurepoc-0.1.4/eurepoc.egg-info/dependency_links.txt
--rw-r--r--   0 camille    (501) staff       (20)      102 2024-05-19 11:33:13.000000 eurepoc-0.1.4/eurepoc.egg-info/requires.txt
--rw-r--r--   0 camille    (501) staff       (20)        8 2024-05-19 11:33:13.000000 eurepoc-0.1.4/eurepoc.egg-info/top_level.txt
--rw-r--r--   0 camille    (501) staff       (20)       38 2024-05-19 11:33:13.803829 eurepoc-0.1.4/setup.cfg
--rw-r--r--   0 camille    (501) staff       (20)      792 2024-05-19 11:31:49.000000 eurepoc-0.1.4/setup.py
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-24 09:28:13.347275 eurepoc-0.1.5/
+-rw-r--r--   0 camille    (501) staff       (20)     1068 2024-05-18 11:49:09.000000 eurepoc-0.1.5/LICENSE
+-rw-r--r--   0 camille    (501) staff       (20)      310 2024-05-18 11:42:32.000000 eurepoc-0.1.5/MANIFEST.in
+-rw-r--r--   0 camille    (501) staff       (20)     1951 2024-05-24 09:28:13.344706 eurepoc-0.1.5/PKG-INFO
+-rw-r--r--   0 camille    (501) staff       (20)     1333 2024-05-19 11:00:11.000000 eurepoc-0.1.5/README.md
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-24 09:28:13.082260 eurepoc-0.1.5/docs/
+-rw-r--r--   0 camille    (501) staff       (20)      638 2024-05-17 13:41:39.000000 eurepoc-0.1.5/docs/Makefile
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-24 09:28:13.106437 eurepoc-0.1.5/docs/build/
+-rw-r--r--   0 camille    (501) staff       (20)      230 2024-05-24 09:25:46.000000 eurepoc-0.1.5/docs/build/.buildinfo
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-24 09:28:13.134120 eurepoc-0.1.5/docs/build/.doctrees/
+-rw-r--r--   0 camille    (501) staff       (20)    26530 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/.doctrees/DatabaseQuery.doctree
+-rw-r--r--   0 camille    (501) staff       (20)    53689 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/.doctrees/IncidentDataFrameGenerator.doctree
+-rw-r--r--   0 camille    (501) staff       (20)     4978 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/.doctrees/date_type.doctree
+-rw-r--r--   0 camille    (501) staff       (20)   363639 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/.doctrees/environment.pickle
+-rw-r--r--   0 camille    (501) staff       (20)     2438 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/.doctrees/flag_type.doctree
+-rw-r--r--   0 camille    (501) staff       (20)     8544 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/.doctrees/index.doctree
+-rw-r--r--   0 camille    (501) staff       (20)    52464 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/.doctrees/initiator_country.doctree
+-rw-r--r--   0 camille    (501) staff       (20)     9218 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/.doctrees/read_token.doctree
+-rw-r--r--   0 camille    (501) staff       (20)     6564 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/.doctrees/receiver_category.doctree
+-rw-r--r--   0 camille    (501) staff       (20)    52411 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/.doctrees/receiver_country.doctree
+-rw-r--r--   0 camille    (501) staff       (20)    13421 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/.doctrees/receiver_region.doctree
+-rw-r--r--   0 camille    (501) staff       (20)    18434 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/DatabaseQuery.html
+-rw-r--r--   0 camille    (501) staff       (20)    42047 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/IncidentDataFrameGenerator.html
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-24 09:28:13.135441 eurepoc-0.1.5/docs/build/_modules/
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-24 09:28:13.139548 eurepoc-0.1.5/docs/build/_modules/eurepoc/
+-rw-r--r--   0 camille    (501) staff       (20)    19498 2024-05-24 09:25:46.000000 eurepoc-0.1.5/docs/build/_modules/eurepoc/database_query.html
+-rw-r--r--   0 camille    (501) staff       (20)    47913 2024-05-24 09:25:46.000000 eurepoc-0.1.5/docs/build/_modules/eurepoc/incident_dataframes.html
+-rw-r--r--   0 camille    (501) staff       (20)    12207 2024-05-24 09:25:46.000000 eurepoc-0.1.5/docs/build/_modules/eurepoc/read_token.html
+-rw-r--r--   0 camille    (501) staff       (20)     9226 2024-05-24 09:25:46.000000 eurepoc-0.1.5/docs/build/_modules/index.html
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-24 09:28:13.223635 eurepoc-0.1.5/docs/build/_sources/
+-rw-r--r--   0 camille    (501) staff       (20)      592 2024-05-24 09:19:42.000000 eurepoc-0.1.5/docs/build/_sources/DatabaseQuery.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)      307 2024-05-24 09:19:39.000000 eurepoc-0.1.5/docs/build/_sources/IncidentDataFrameGenerator.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)      580 2024-05-18 11:23:56.000000 eurepoc-0.1.5/docs/build/_sources/date_type.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)       19 2024-05-18 10:46:49.000000 eurepoc-0.1.5/docs/build/_sources/flag_type.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)     1843 2024-05-19 11:01:08.000000 eurepoc-0.1.5/docs/build/_sources/index.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)     4085 2024-05-18 11:09:52.000000 eurepoc-0.1.5/docs/build/_sources/initiator_country.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)      112 2024-05-24 09:19:35.000000 eurepoc-0.1.5/docs/build/_sources/read_token.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)      708 2024-05-18 11:23:56.000000 eurepoc-0.1.5/docs/build/_sources/receiver_category.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)     4059 2024-05-18 11:09:52.000000 eurepoc-0.1.5/docs/build/_sources/receiver_country.rst.txt
+-rw-r--r--   0 camille    (501) staff       (20)      980 2024-05-18 11:23:56.000000 eurepoc-0.1.5/docs/build/_sources/receiver_region.rst.txt
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-24 09:28:13.300145 eurepoc-0.1.5/docs/build/_static/
+-rw-r--r--   0 camille    (501) staff       (20)    15094 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/_static/basic.css
+-rw-r--r--   0 camille    (501) staff       (20)     4913 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/_static/classic.css
+-rw-r--r--   0 camille    (501) staff       (20)     3508 2024-05-17 15:45:22.000000 eurepoc-0.1.5/docs/build/_static/copybutton.js
+-rw-r--r--   0 camille    (501) staff       (20)       28 2024-05-17 13:40:31.000000 eurepoc-0.1.5/docs/build/_static/default.css
+-rw-r--r--   0 camille    (501) staff       (20)     4472 2024-05-17 13:40:31.000000 eurepoc-0.1.5/docs/build/_static/doctools.js
+-rw-r--r--   0 camille    (501) staff       (20)      328 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/_static/documentation_options.js
+-rw-r--r--   0 camille    (501) staff       (20)      286 2024-05-17 13:40:31.000000 eurepoc-0.1.5/docs/build/_static/file.png
+-rw-r--r--   0 camille    (501) staff       (20)     4758 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/_static/language_data.js
+-rw-r--r--   0 camille    (501) staff       (20)     2137 2024-05-17 15:45:22.000000 eurepoc-0.1.5/docs/build/_static/menu.js
+-rw-r--r--   0 camille    (501) staff       (20)       90 2024-05-17 13:40:31.000000 eurepoc-0.1.5/docs/build/_static/minus.png
+-rw-r--r--   0 camille    (501) staff       (20)       90 2024-05-17 13:40:31.000000 eurepoc-0.1.5/docs/build/_static/plus.png
+-rw-r--r--   0 camille    (501) staff       (20)      695 2024-05-17 15:45:22.000000 eurepoc-0.1.5/docs/build/_static/py.png
+-rw-r--r--   0 camille    (501) staff       (20)     2041 2024-05-17 15:45:22.000000 eurepoc-0.1.5/docs/build/_static/py.svg
+-rw-r--r--   0 camille    (501) staff       (20)    13101 2024-05-17 15:45:22.000000 eurepoc-0.1.5/docs/build/_static/pydoctheme.css
+-rw-r--r--   0 camille    (501) staff       (20)     2371 2024-05-17 15:45:22.000000 eurepoc-0.1.5/docs/build/_static/pydoctheme_dark.css
+-rw-r--r--   0 camille    (501) staff       (20)     4902 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/_static/pygments.css
+-rw-r--r--   0 camille    (501) staff       (20)     5055 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/_static/pygments_dark.css
+-rw-r--r--   0 camille    (501) staff       (20)      559 2024-05-17 15:45:22.000000 eurepoc-0.1.5/docs/build/_static/search-focus.js
+-rw-r--r--   0 camille    (501) staff       (20)    20731 2024-05-17 13:40:31.000000 eurepoc-0.1.5/docs/build/_static/searchtools.js
+-rw-r--r--   0 camille    (501) staff       (20)     2617 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/_static/sidebar.js
+-rw-r--r--   0 camille    (501) staff       (20)     5123 2024-05-17 13:40:31.000000 eurepoc-0.1.5/docs/build/_static/sphinx_highlight.js
+-rw-r--r--   0 camille    (501) staff       (20)      779 2024-05-17 15:45:22.000000 eurepoc-0.1.5/docs/build/_static/themetoggle.js
+-rw-r--r--   0 camille    (501) staff       (20)    11699 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/date_type.html
+-rw-r--r--   0 camille    (501) staff       (20)    11079 2024-05-24 09:25:45.000000 eurepoc-0.1.5/docs/build/flag_type.html
+-rw-r--r--   0 camille    (501) staff       (20)    16596 2024-05-24 09:25:46.000000 eurepoc-0.1.5/docs/build/genindex.html
+-rw-r--r--   0 camille    (501) staff       (20)    15261 2024-05-24 09:25:46.000000 eurepoc-0.1.5/docs/build/index.html
+-rw-r--r--   0 camille    (501) staff       (20)    18852 2024-05-24 09:25:46.000000 eurepoc-0.1.5/docs/build/initiator_country.html
+-rw-r--r--   0 camille    (501) staff       (20)      683 2024-05-24 09:25:46.000000 eurepoc-0.1.5/docs/build/objects.inv
+-rw-r--r--   0 camille    (501) staff       (20)    10062 2024-05-24 09:25:46.000000 eurepoc-0.1.5/docs/build/py-modindex.html
+-rw-r--r--   0 camille    (501) staff       (20)    13325 2024-05-24 09:25:46.000000 eurepoc-0.1.5/docs/build/read_token.html
+-rw-r--r--   0 camille    (501) staff       (20)    12144 2024-05-24 09:25:46.000000 eurepoc-0.1.5/docs/build/receiver_category.html
+-rw-r--r--   0 camille    (501) staff       (20)    18880 2024-05-24 09:25:46.000000 eurepoc-0.1.5/docs/build/receiver_country.html
+-rw-r--r--   0 camille    (501) staff       (20)    12935 2024-05-24 09:25:46.000000 eurepoc-0.1.5/docs/build/receiver_region.html
+-rw-r--r--   0 camille    (501) staff       (20)     7117 2024-05-24 09:25:46.000000 eurepoc-0.1.5/docs/build/search.html
+-rw-r--r--   0 camille    (501) staff       (20)    21668 2024-05-24 09:25:46.000000 eurepoc-0.1.5/docs/build/searchindex.js
+-rw-r--r--   0 camille    (501) staff       (20)      804 2024-05-17 13:41:39.000000 eurepoc-0.1.5/docs/make.bat
+-rw-r--r--   0 camille    (501) staff       (20)       66 2024-05-19 11:05:40.000000 eurepoc-0.1.5/docs/requirements.txt
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-24 09:28:13.321899 eurepoc-0.1.5/docs/source/
+-rw-r--r--   0 camille    (501) staff       (20)      592 2024-05-24 09:19:42.000000 eurepoc-0.1.5/docs/source/DatabaseQuery.rst
+-rw-r--r--   0 camille    (501) staff       (20)      307 2024-05-24 09:19:39.000000 eurepoc-0.1.5/docs/source/IncidentDataFrameGenerator.rst
+-rw-r--r--   0 camille    (501) staff       (20)     1057 2024-05-24 09:25:42.000000 eurepoc-0.1.5/docs/source/conf.py
+-rw-r--r--   0 camille    (501) staff       (20)      580 2024-05-18 11:23:56.000000 eurepoc-0.1.5/docs/source/date_type.rst
+-rw-r--r--   0 camille    (501) staff       (20)       19 2024-05-18 10:46:49.000000 eurepoc-0.1.5/docs/source/flag_type.rst
+-rw-r--r--   0 camille    (501) staff       (20)     1843 2024-05-19 11:01:08.000000 eurepoc-0.1.5/docs/source/index.rst
+-rw-r--r--   0 camille    (501) staff       (20)     4085 2024-05-18 11:09:52.000000 eurepoc-0.1.5/docs/source/initiator_country.rst
+-rw-r--r--   0 camille    (501) staff       (20)      112 2024-05-24 09:19:35.000000 eurepoc-0.1.5/docs/source/read_token.rst
+-rw-r--r--   0 camille    (501) staff       (20)      708 2024-05-18 11:23:56.000000 eurepoc-0.1.5/docs/source/receiver_category.rst
+-rw-r--r--   0 camille    (501) staff       (20)     4059 2024-05-18 11:09:52.000000 eurepoc-0.1.5/docs/source/receiver_country.rst
+-rw-r--r--   0 camille    (501) staff       (20)      980 2024-05-18 11:23:56.000000 eurepoc-0.1.5/docs/source/receiver_region.rst
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-24 09:28:13.332029 eurepoc-0.1.5/eurepoc/
+-rw-r--r--   0 camille    (501) staff       (20)      254 2024-05-19 11:00:11.000000 eurepoc-0.1.5/eurepoc/__init__.py
+-rw-r--r--   0 camille    (501) staff       (20)    36013 2024-05-18 10:16:25.000000 eurepoc-0.1.5/eurepoc/data_cleaning_utils.py
+-rw-r--r--   0 camille    (501) staff       (20)     9265 2024-05-17 12:10:59.000000 eurepoc-0.1.5/eurepoc/data_query_utils.py
+-rw-r--r--   0 camille    (501) staff       (20)     3289 2024-05-19 11:00:11.000000 eurepoc-0.1.5/eurepoc/database_query.py
+-rw-r--r--   0 camille    (501) staff       (20)    10816 2024-05-19 11:00:11.000000 eurepoc-0.1.5/eurepoc/incident_dataframes.py
+-rw-r--r--   0 camille    (501) staff       (20)      924 2024-05-18 10:24:49.000000 eurepoc-0.1.5/eurepoc/read_token.py
+-rw-r--r--   0 camille    (501) staff       (20)     8832 2024-05-17 09:56:40.000000 eurepoc-0.1.5/eurepoc/table_models.py
+-rw-r--r--   0 camille    (501) staff       (20)    33473 2024-05-24 09:03:15.000000 eurepoc-0.1.5/eurepoc/tables.py
+drwxr-xr-x   0 camille    (501) staff       (20)        0 2024-05-24 09:28:13.343108 eurepoc-0.1.5/eurepoc.egg-info/
+-rw-r--r--   0 camille    (501) staff       (20)     1951 2024-05-24 09:28:12.000000 eurepoc-0.1.5/eurepoc.egg-info/PKG-INFO
+-rw-r--r--   0 camille    (501) staff       (20)     3016 2024-05-24 09:28:12.000000 eurepoc-0.1.5/eurepoc.egg-info/SOURCES.txt
+-rw-r--r--   0 camille    (501) staff       (20)        1 2024-05-24 09:28:12.000000 eurepoc-0.1.5/eurepoc.egg-info/dependency_links.txt
+-rw-r--r--   0 camille    (501) staff       (20)      102 2024-05-24 09:28:12.000000 eurepoc-0.1.5/eurepoc.egg-info/requires.txt
+-rw-r--r--   0 camille    (501) staff       (20)        8 2024-05-24 09:28:12.000000 eurepoc-0.1.5/eurepoc.egg-info/top_level.txt
+-rw-r--r--   0 camille    (501) staff       (20)       38 2024-05-24 09:28:13.347622 eurepoc-0.1.5/setup.cfg
+-rw-r--r--   0 camille    (501) staff       (20)      792 2024-05-24 09:27:21.000000 eurepoc-0.1.5/setup.py
```

### Comparing `eurepoc-0.1.4/LICENSE` & `eurepoc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/PKG-INFO` & `eurepoc-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eurepoc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Wrapper for the EuRepoC API
 Author: Camille Borrett
 License: MIT
 Project-URL: Documentation, https://eurepoc.readthedocs.io/
 Project-URL: Source, https://github.com/camilleborrett/eurepoc
 Project-URL: Tracker, https://github.com/camilleborrett/eurepoc/issues
 Project-URL: EuRepoC Project, https://eurepoc.eu/
```

### Comparing `eurepoc-0.1.4/README.md` & `eurepoc-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/Makefile` & `eurepoc-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/.doctrees/DatabaseQuery.doctree` & `eurepoc-0.1.5/docs/build/.doctrees/DatabaseQuery.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/.doctrees/IncidentDataFrameGenerator.doctree` & `eurepoc-0.1.5/docs/build/.doctrees/IncidentDataFrameGenerator.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/.doctrees/date_type.doctree` & `eurepoc-0.1.5/docs/build/.doctrees/date_type.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/.doctrees/environment.pickle` & `eurepoc-0.1.5/docs/build/.doctrees/environment.pickle`

 * *Files 0% similar despite different names*

```diff
@@ -704,50 +704,50 @@
 00002bf0: 7374 6174 7573 5f65 7874 7261 9468 2f8c  status_extra.h/.
 00002c00: 0665 7665 6e74 7394 4e68 2a8c 0e73 7068  .events.Nh*..sph
 00002c10: 696e 782e 7072 6f6a 6563 7494 8c07 5072  inx.project...Pr
 00002c20: 6f6a 6563 7494 9394 2981 947d 9428 6815  oject...)..}.(h.
 00002c30: 6818 683e 6840 8594 8c14 5f66 6972 7374  h.h>h@...._first
 00002c40: 5f73 6f75 7263 655f 7375 6666 6978 9468  _source_suffix.h
 00002c50: 408c 0864 6f63 6e61 6d65 7394 8f94 288c  @..docnames...(.
-00002c60: 0a72 6561 645f 746f 6b65 6e94 8c0d 4461  .read_token...Da
-00002c70: 7461 6261 7365 5175 6572 7994 8c0f 7265  tabaseQuery...re
-00002c80: 6365 6976 6572 5f72 6567 696f 6e94 8c09  ceiver_region...
-00002c90: 666c 6167 5f74 7970 6594 8c05 696e 6465  flag_type...inde
-00002ca0: 7894 8c10 7265 6365 6976 6572 5f63 6f75  x...receiver_cou
-00002cb0: 6e74 7279 948c 1172 6563 6569 7665 725f  ntry...receiver_
-00002cc0: 6361 7465 676f 7279 948c 0964 6174 655f  category...date_
-00002cd0: 7479 7065 948c 1169 6e69 7469 6174 6f72  type...initiator
-00002ce0: 5f63 6f75 6e74 7279 948c 1a49 6e63 6964  _country...Incid
-00002cf0: 656e 7444 6174 6146 7261 6d65 4765 6e65  entDataFrameGene
-00002d00: 7261 746f 7294 908c 105f 7061 7468 5f74  rator...._path_t
+00002c60: 1172 6563 6569 7665 725f 6361 7465 676f  .receiver_catego
+00002c70: 7279 948c 0d44 6174 6162 6173 6551 7565  ry...DatabaseQue
+00002c80: 7279 948c 0569 6e64 6578 948c 0964 6174  ry...index...dat
+00002c90: 655f 7479 7065 948c 1169 6e69 7469 6174  e_type...initiat
+00002ca0: 6f72 5f63 6f75 6e74 7279 948c 0f72 6563  or_country...rec
+00002cb0: 6569 7665 725f 7265 6769 6f6e 948c 1072  eiver_region...r
+00002cc0: 6563 6569 7665 725f 636f 756e 7472 7994  eceiver_country.
+00002cd0: 8c09 666c 6167 5f74 7970 6594 8c1a 496e  ..flag_type...In
+00002ce0: 6369 6465 6e74 4461 7461 4672 616d 6547  cidentDataFrameG
+00002cf0: 656e 6572 6174 6f72 948c 0a72 6561 645f  enerator...read_
+00002d00: 746f 6b65 6e94 908c 105f 7061 7468 5f74  token...._path_t
 00002d10: 6f5f 646f 636e 616d 6594 7d94 288c 1144  o_docname.}.(..D
 00002d20: 6174 6162 6173 6551 7565 7279 2e72 7374  atabaseQuery.rst
 00002d30: 946a 1203 0000 8c1e 496e 6369 6465 6e74  .j......Incident
 00002d40: 4461 7461 4672 616d 6547 656e 6572 6174  DataFrameGenerat
-00002d50: 6f72 2e72 7374 946a 1a03 0000 8c0d 6461  or.rst.j......da
-00002d60: 7465 5f74 7970 652e 7273 7494 6a18 0300  te_type.rst.j...
+00002d50: 6f72 2e72 7374 946a 1903 0000 8c0d 6461  or.rst.j......da
+00002d60: 7465 5f74 7970 652e 7273 7494 6a14 0300  te_type.rst.j...
 00002d70: 008c 0d66 6c61 675f 7479 7065 2e72 7374  ...flag_type.rst
-00002d80: 946a 1403 0000 8c09 696e 6465 782e 7273  .j......index.rs
-00002d90: 7494 6a15 0300 008c 1569 6e69 7469 6174  t.j......initiat
+00002d80: 946a 1803 0000 8c09 696e 6465 782e 7273  .j......index.rs
+00002d90: 7494 6a13 0300 008c 1569 6e69 7469 6174  t.j......initiat
 00002da0: 6f72 5f63 6f75 6e74 7279 2e72 7374 946a  or_country.rst.j
-00002db0: 1903 0000 8c0e 7265 6164 5f74 6f6b 656e  ......read_token
-00002dc0: 2e72 7374 946a 1103 0000 8c15 7265 6365  .rst.j......rece
+00002db0: 1503 0000 8c0e 7265 6164 5f74 6f6b 656e  ......read_token
+00002dc0: 2e72 7374 946a 1a03 0000 8c15 7265 6365  .rst.j......rece
 00002dd0: 6976 6572 5f63 6174 6567 6f72 792e 7273  iver_category.rs
-00002de0: 7494 6a17 0300 008c 1472 6563 6569 7665  t.j......receive
-00002df0: 725f 636f 756e 7472 792e 7273 7494 6a16  r_country.rst.j.
+00002de0: 7494 6a11 0300 008c 1472 6563 6569 7665  t.j......receive
+00002df0: 725f 636f 756e 7472 792e 7273 7494 6a17  r_country.rst.j.
 00002e00: 0300 008c 1372 6563 6569 7665 725f 7265  .....receiver_re
-00002e10: 6769 6f6e 2e72 7374 946a 1303 0000 758c  gion.rst.j....u.
+00002e10: 6769 6f6e 2e72 7374 946a 1603 0000 758c  gion.rst.j....u.
 00002e20: 105f 646f 636e 616d 655f 746f 5f70 6174  ._docname_to_pat
 00002e30: 6894 7d94 286a 1203 0000 6a1d 0300 006a  h.}.(j....j....j
-00002e40: 1a03 0000 6a1e 0300 006a 1803 0000 6a1f  ....j....j....j.
-00002e50: 0300 006a 1403 0000 6a20 0300 006a 1503  ...j....j ...j..
-00002e60: 0000 6a21 0300 006a 1903 0000 6a22 0300  ..j!...j....j"..
-00002e70: 006a 1103 0000 6a23 0300 006a 1703 0000  .j....j#...j....
-00002e80: 6a24 0300 006a 1603 0000 6a25 0300 006a  j$...j....j%...j
-00002e90: 1303 0000 6a26 0300 0075 7562 6830 7d94  ....j&...uubh0}.
+00002e40: 1903 0000 6a1e 0300 006a 1403 0000 6a1f  ....j....j....j.
+00002e50: 0300 006a 1803 0000 6a20 0300 006a 1303  ...j....j ...j..
+00002e60: 0000 6a21 0300 006a 1503 0000 6a22 0300  ..j!...j....j"..
+00002e70: 006a 1a03 0000 6a23 0300 006a 1103 0000  .j....j#...j....
+00002e80: 6a24 0300 006a 1703 0000 6a25 0300 006a  j$...j....j%...j
+00002e90: 1603 0000 6a26 0300 0075 7562 6830 7d94  ....j&...uubh0}.
 00002ea0: 288c 1073 7068 696e 782e 646f 6d61 696e  (..sphinx.domain
 00002eb0: 732e 6394 4b03 8c18 7370 6869 6e78 2e64  s.c.K...sphinx.d
 00002ec0: 6f6d 6169 6e73 2e63 6861 6e67 6573 6574  omains.changeset
 00002ed0: 944b 018c 1773 7068 696e 782e 646f 6d61  .K...sphinx.doma
 00002ee0: 696e 732e 6369 7461 7469 6f6e 944b 018c  ins.citation.K..
 00002ef0: 1273 7068 696e 782e 646f 6d61 696e 732e  .sphinx.domains.
 00002f00: 6370 7094 4b09 8c14 7370 6869 6e78 2e64  cpp.K...sphinx.d
@@ -788,40 +788,40 @@
 00003130: 6c94 4b05 8c16 6669 6c65 5f69 6e73 6572  l.K...file_inser
 00003140: 7469 6f6e 5f65 6e61 626c 6564 9488 8c13  tion_enabled....
 00003150: 736d 6172 7471 756f 7465 735f 6c6f 6361  smartquotes_loca
 00003160: 6c65 7394 5d94 6ab3 0100 0068 0368 4f89  les.].j....h.hO.
 00003170: 8c0d 6c61 6e67 7561 6765 5f63 6f64 6594  ..language_code.
 00003180: 6828 8c0c 736d 6172 745f 7175 6f74 6573  h(..smart_quotes
 00003190: 9488 758c 0861 6c6c 5f64 6f63 7394 7d94  ..u..all_docs.}.
-000031a0: 286a 1203 0000 8a07 8a85 5cc6 cc18 066a  (j........\....j
-000031b0: 1a03 0000 8a07 854f 5ec6 cc18 066a 1803  .......O^....j..
-000031c0: 0000 8a07 bc6c 5ec6 cc18 066a 1403 0000  .....l^....j....
-000031d0: 8a07 5179 5ec6 cc18 066a 1503 0000 8a07  ..Qy^....j......
-000031e0: 3aa3 5ec6 cc18 066a 1903 0000 8a07 aca6  :.^....j........
-000031f0: 5fc6 cc18 066a 1103 0000 8a07 e7a0 60c6  _....j........`.
-00003200: cc18 066a 1703 0000 8a07 1fc1 60c6 cc18  ...j........`...
-00003210: 066a 1603 0000 8a07 85d3 61c6 cc18 066a  .j........a....j
-00003220: 1303 0000 8a07 a022 62c6 cc18 0675 8c0c  ......."b....u..
+000031a0: 286a 1203 0000 8a07 89a3 94c0 2f19 066a  (j........../..j
+000031b0: 1903 0000 8a07 5e30 96c0 2f19 066a 1403  ......^0../..j..
+000031c0: 0000 8a07 6b4e 96c0 2f19 066a 1803 0000  ....kN../..j....
+000031d0: 8a07 1359 96c0 2f19 066a 1303 0000 8a07  ...Y../..j......
+000031e0: 6f7b 96c0 2f19 066a 1503 0000 8a07 d34e  o{../..j.......N
+000031f0: 97c0 2f19 066a 1a03 0000 8a07 ca2b 98c0  ../..j.......+..
+00003200: 2f19 066a 1103 0000 8a07 3449 98c0 2f19  /..j......4I../.
+00003210: 066a 1703 0000 8a07 af36 99c0 2f19 066a  .j.......6../..j
+00003220: 1603 0000 8a07 2c70 99c0 2f19 0675 8c0c  ......,p../..u..
 00003230: 6465 7065 6e64 656e 6369 6573 948c 0b63  dependencies...c
 00003240: 6f6c 6c65 6374 696f 6e73 948c 0b64 6566  ollections...def
 00003250: 6175 6c74 6469 6374 9493 948c 0862 7569  aultdict.....bui
 00003260: 6c74 696e 7394 8c03 7365 7494 9394 8594  ltins...set.....
-00003270: 5294 286a 1203 0000 8f94 288c 1f2e 2e2f  R.(j......(..../
-00003280: 2e2e 2f65 7572 6570 6f63 2f64 6174 6162  ../eurepoc/datab
-00003290: 6173 655f 7175 6572 792e 7079 948c 212e  ase_query.py..!.
-000032a0: 2e2f 2e2e 2f65 7572 6570 6f63 2f64 6174  ./../eurepoc/dat
-000032b0: 615f 7175 6572 795f 7574 696c 732e 7079  a_query_utils.py
-000032c0: 948c 242e 2e2f 2e2e 2f65 7572 6570 6f63  ..$../../eurepoc
-000032d0: 2f64 6174 615f 636c 6561 6e69 6e67 5f75  /data_cleaning_u
-000032e0: 7469 6c73 2e70 7994 906a 1a03 0000 8f94  tils.py..j......
-000032f0: 288c 242e 2e2f 2e2e 2f65 7572 6570 6f63  (.$../../eurepoc
-00003300: 2f69 6e63 6964 656e 745f 6461 7461 6672  /incident_datafr
-00003310: 616d 6573 2e70 7994 8c17 2e2e 2f2e 2e2f  ames.py...../../
-00003320: 6575 7265 706f 632f 7461 626c 6573 2e70  eurepoc/tables.p
-00003330: 7994 906a 1103 0000 8f94 288c 1b2e 2e2f  y..j......(..../
+00003270: 5294 286a 1203 0000 8f94 288c 212e 2e2f  R.(j......(.!../
+00003280: 2e2e 2f65 7572 6570 6f63 2f64 6174 615f  ../eurepoc/data_
+00003290: 7175 6572 795f 7574 696c 732e 7079 948c  query_utils.py..
+000032a0: 242e 2e2f 2e2e 2f65 7572 6570 6f63 2f64  $../../eurepoc/d
+000032b0: 6174 615f 636c 6561 6e69 6e67 5f75 7469  ata_cleaning_uti
+000032c0: 6c73 2e70 7994 8c1f 2e2e 2f2e 2e2f 6575  ls.py...../../eu
+000032d0: 7265 706f 632f 6461 7461 6261 7365 5f71  repoc/database_q
+000032e0: 7565 7279 2e70 7994 906a 1903 0000 8f94  uery.py..j......
+000032f0: 288c 172e 2e2f 2e2e 2f65 7572 6570 6f63  (..../../eurepoc
+00003300: 2f74 6162 6c65 732e 7079 948c 242e 2e2f  /tables.py..$../
+00003310: 2e2e 2f65 7572 6570 6f63 2f69 6e63 6964  ../eurepoc/incid
+00003320: 656e 745f 6461 7461 6672 616d 6573 2e70  ent_dataframes.p
+00003330: 7994 906a 1a03 0000 8f94 288c 1b2e 2e2f  y..j......(..../
 00003340: 2e2e 2f65 7572 6570 6f63 2f72 6561 645f  ../eurepoc/read_
 00003350: 746f 6b65 6e2e 7079 9490 758c 0869 6e63  token.py..u..inc
 00003360: 6c75 6465 6494 6a56 0300 006a 5903 0000  luded.jV...jY...
 00003370: 8594 5294 8c0d 7265 7265 6164 5f61 6c77  ..R...reread_alw
 00003380: 6179 7394 8f94 8c16 5f70 6963 6b6c 6564  ays....._pickled
 00003390: 5f64 6f63 7472 6565 5f63 6163 6865 947d  _doctree_cache.}
 000033a0: 948c 185f 7772 6974 655f 646f 635f 646f  ..._write_doc_do
@@ -2947,15 +2947,15 @@
 0000b820: 656c 944b 018c 0474 7970 6594 8c04 494e  el.K...type...IN
 0000b830: 464f 948c 0673 6f75 7263 6594 6a22 0400  FO...source.j"..
 0000b840: 008c 046c 696e 6594 4b01 756a 9603 0000  ...line.K.uj....
 0000b850: 6a5a 0d00 0075 6261 8c0b 7472 616e 7366  jZ...uba..transf
 0000b860: 6f72 6d65 7294 4e8c 0b69 6e63 6c75 6465  ormer.N..include
 0000b870: 5f6c 6f67 945d 948c 0a64 6563 6f72 6174  _log.]...decorat
 0000b880: 696f 6e94 4e6a 8803 0000 6a71 0300 0075  ion.Nj....jq...u
-0000b890: 626a 1a03 0000 6a70 0300 0029 8194 7d94  bj....jp...)..}.
+0000b890: 626a 1903 0000 6a70 0300 0029 8194 7d94  bj....jp...)..}.
 0000b8a0: 286a 7303 0000 682f 6a74 0300 005d 946a  (js...h/jt...].j
 0000b8b0: 7703 0000 2981 947d 9428 6a73 0300 0068  w...)..}.(js...h
 0000b8c0: 2f6a 7403 0000 5d94 286a 7c03 0000 2981  /jt...].(j|...).
 0000b8d0: 947d 9428 6a73 0300 008c 1a49 6e63 6964  .}.(js.....Incid
 0000b8e0: 656e 7444 6174 6146 7261 6d65 4765 6e65  entDataFrameGene
 0000b8f0: 7261 746f 7294 6a74 0300 005d 946a 8203  rator.jt...].j..
 0000b900: 0000 8c1a 496e 6369 6465 6e74 4461 7461  ....IncidentData
@@ -3182,15 +3182,15 @@
 0000c6d0: 0000 5d94 6a8a 0300 007d 9428 6a8c 0300  ..].j....}.(j...
 0000c6e0: 005d 946a 8e03 0000 5d94 6a90 0300 005d  .].j....].j....]
 0000c6f0: 946a 9203 0000 5d94 6a94 0300 005d 948c  .j....].j....]..
 0000c700: 0972 6566 7461 7267 6574 948c 245f 6d6f  .reftarget..$_mo
 0000c710: 6475 6c65 732f 6575 7265 706f 632f 696e  dules/eurepoc/in
 0000c720: 6369 6465 6e74 5f64 6174 6166 7261 6d65  cident_dataframe
 0000c730: 7394 8c05 7265 6669 6494 6a0a 0e00 008c  s...refid.j.....
-0000c740: 0672 6566 646f 6394 6a1a 0300 0075 6a96  .refdoc.j....uj.
+0000c740: 0672 6566 646f 6394 6a19 0300 0075 6a96  .refdoc.j....uj.
 0000c750: 0300 006a 8206 0000 6a87 0300 006a d90d  ...j....j....j..
 0000c760: 0000 6a88 0300 006a 7b0d 0000 6816 4e6a  ..j....j{...h.Nj
 0000c770: 8903 0000 4e75 6265 6a8a 0300 007d 9428  ....Nubej....}.(
 0000c780: 6a8c 0300 005d 946a c90d 0000 616a 8e03  j....].j....aj..
 0000c790: 0000 5d94 286a 9406 0000 6a95 0600 0065  ..].(j....j....e
 0000c7a0: 6a90 0300 005d 946a 9203 0000 5d94 6a94  j....].j....].j.
 0000c7b0: 0300 005d 946a 9906 0000 8c1b 6575 7265  ...].j......eure
@@ -3222,15 +3222,15 @@
 0000c950: 0270 7994 8c08 7079 2d63 6c61 7373 9465  .py...py-class.e
 0000c960: 6a90 0300 005d 946a 9203 0000 5d94 6a94  j....].j....].j.
 0000c970: 0300 005d 9475 6a96 0300 006a b206 0000  ...].uj....j....
 0000c980: 6a87 0300 006a 750e 0000 7562 616a 8a03  j....ju...ubaj..
 0000c990: 0000 7d94 286a 8c03 0000 5d94 6a8e 0300  ..}.(j....].j...
 0000c9a0: 005d 946a 9003 0000 5d94 6a92 0300 005d  .].j....].j....]
 0000c9b0: 946a 9403 0000 5d94 8c06 7265 6664 6f63  .j....]...refdoc
-0000c9c0: 946a 1a03 0000 8c09 7265 6664 6f6d 6169  .j......refdomai
+0000c9c0: 946a 1903 0000 8c09 7265 6664 6f6d 6169  .j......refdomai
 0000c9d0: 6e94 6a83 0e00 008c 0772 6566 7479 7065  n.j......reftype
 0000c9e0: 948c 0563 6c61 7373 948c 0b72 6566 6578  ...class...refex
 0000c9f0: 706c 6963 6974 9489 8c07 7265 6677 6172  plicit....refwar
 0000ca00: 6e94 896a d006 0000 6a68 0e00 006a d106  n..j....jh...j..
 0000ca10: 0000 6a0a 0e00 006a d206 0000 8c06 6f62  ..j....j......ob
 0000ca20: 6a65 6374 9475 6a96 0300 006a ac06 0000  ject.uj....j....
 0000ca30: 6816 8c8e 2f55 7365 7273 2f63 616d 696c  h.../Users/camil
@@ -3653,15 +3653,15 @@
 0000e440: 6566 7461 7267 6574 948c 245f 6d6f 6475  eftarget..$_modu
 0000e450: 6c65 732f 6575 7265 706f 632f 696e 6369  les/eurepoc/inci
 0000e460: 6465 6e74 5f64 6174 6166 7261 6d65 7394  dent_dataframes.
 0000e470: 8c05 7265 6669 6494 8c32 496e 6369 6465  ..refid..2Incide
 0000e480: 6e74 4461 7461 4672 616d 6547 656e 6572  ntDataFrameGener
 0000e490: 6174 6f72 2e67 6574 5f61 7474 7269 6275  ator.get_attribu
 0000e4a0: 7469 6f6e 5f73 6f75 7263 6573 948c 0672  tion_sources...r
-0000e4b0: 6566 646f 6394 6a1a 0300 0075 6a96 0300  efdoc.j....uj...
+0000e4b0: 6566 646f 6394 6a19 0300 0075 6a96 0300  efdoc.j....uj...
 0000e4c0: 006a 8206 0000 6a87 0300 006a e40f 0000  .j....j....j....
 0000e4d0: 6a88 0300 006a 7b0d 0000 6816 4e6a 8903  j....j{...h.Nj..
 0000e4e0: 0000 4e75 6265 6a8a 0300 007d 9428 6a8c  ..Nubej....}.(j.
 0000e4f0: 0300 005d 946a de0f 0000 616a 8e03 0000  ...].j....aj....
 0000e500: 5d94 286a 9406 0000 6a95 0600 0065 6a90  ].(j....j....ej.
 0000e510: 0300 005d 946a 9203 0000 5d94 6a94 0300  ...].j....].j...
 0000e520: 005d 946a 9906 0000 8c1b 6575 7265 706f  .].j......eurepo
@@ -3785,15 +3785,15 @@
 0000ec80: 0300 005d 948c 0972 6566 7461 7267 6574  ...]...reftarget
 0000ec90: 948c 245f 6d6f 6475 6c65 732f 6575 7265  ..$_modules/eure
 0000eca0: 706f 632f 696e 6369 6465 6e74 5f64 6174  poc/incident_dat
 0000ecb0: 6166 7261 6d65 7394 8c05 7265 6669 6494  aframes...refid.
 0000ecc0: 8c2b 496e 6369 6465 6e74 4461 7461 4672  .+IncidentDataFr
 0000ecd0: 616d 6547 656e 6572 6174 6f72 2e67 6574  ameGenerator.get
 0000ece0: 5f61 7474 7269 6275 7469 6f6e 7394 8c06  _attributions...
-0000ecf0: 7265 6664 6f63 946a 1a03 0000 756a 9603  refdoc.j....uj..
+0000ecf0: 7265 6664 6f63 946a 1903 0000 756a 9603  refdoc.j....uj..
 0000ed00: 0000 6a82 0600 006a 8703 0000 6a4b 1000  ..j....j....jK..
 0000ed10: 006a 8803 0000 6a7b 0d00 0068 164e 6a89  .j....j{...h.Nj.
 0000ed20: 0300 004e 7562 656a 8a03 0000 7d94 286a  ...Nubej....}.(j
 0000ed30: 8c03 0000 5d94 6a45 1000 0061 6a8e 0300  ....].jE...aj...
 0000ed40: 005d 9428 6a94 0600 006a 9506 0000 656a  .].(j....j....ej
 0000ed50: 9003 0000 5d94 6a92 0300 005d 946a 9403  ....].j....].j..
 0000ed60: 0000 5d94 6a99 0600 008c 1b65 7572 6570  ..].j......eurep
@@ -3966,15 +3966,15 @@
 0000f7d0: 948c 245f 6d6f 6475 6c65 732f 6575 7265  ..$_modules/eure
 0000f7e0: 706f 632f 696e 6369 6465 6e74 5f64 6174  poc/incident_dat
 0000f7f0: 6166 7261 6d65 7394 8c05 7265 6669 6494  aframes...refid.
 0000f800: 8c34 496e 6369 6465 6e74 4461 7461 4672  .4IncidentDataFr
 0000f810: 616d 6547 656e 6572 6174 6f72 2e67 6574  ameGenerator.get
 0000f820: 5f63 7962 6572 5f63 6f6e 666c 6963 745f  _cyber_conflict_
 0000f830: 6973 7375 6573 948c 0672 6566 646f 6394  issues...refdoc.
-0000f840: 6a1a 0300 0075 6a96 0300 006a 8206 0000  j....uj....j....
+0000f840: 6a19 0300 0075 6a96 0300 006a 8206 0000  j....uj....j....
 0000f850: 6a87 0300 006a b210 0000 6a88 0300 006a  j....j....j....j
 0000f860: 7b0d 0000 6816 4e6a 8903 0000 4e75 6265  {...h.Nj....Nube
 0000f870: 6a8a 0300 007d 9428 6a8c 0300 005d 946a  j....}.(j....].j
 0000f880: ac10 0000 616a 8e03 0000 5d94 286a 9406  ....aj....].(j..
 0000f890: 0000 6a95 0600 0065 6a90 0300 005d 946a  ..j....ej....].j
 0000f8a0: 9203 0000 5d94 6a94 0300 005d 946a 9906  ....].j....].j..
 0000f8b0: 0000 8c1b 6575 7265 706f 632e 696e 6369  ....eurepoc.inci
@@ -4105,15 +4105,15 @@
 00010080: 245f 6d6f 6475 6c65 732f 6575 7265 706f  $_modules/eurepo
 00010090: 632f 696e 6369 6465 6e74 5f64 6174 6166  c/incident_dataf
 000100a0: 7261 6d65 7394 8c05 7265 6669 6494 8c38  rames...refid..8
 000100b0: 496e 6369 6465 6e74 4461 7461 4672 616d  IncidentDataFram
 000100c0: 6547 656e 6572 6174 6f72 2e67 6574 5f63  eGenerator.get_c
 000100d0: 7962 6572 5f69 6e74 656e 7369 7479 5f76  yber_intensity_v
 000100e0: 6172 6961 626c 6573 948c 0672 6566 646f  ariables...refdo
-000100f0: 6394 6a1a 0300 0075 6a96 0300 006a 8206  c.j....uj....j..
+000100f0: 6394 6a19 0300 0075 6a96 0300 006a 8206  c.j....uj....j..
 00010100: 0000 6a87 0300 006a 1911 0000 6a88 0300  ..j....j....j...
 00010110: 006a 7b0d 0000 6816 4e6a 8903 0000 4e75  .j{...h.Nj....Nu
 00010120: 6265 6a8a 0300 007d 9428 6a8c 0300 005d  bej....}.(j....]
 00010130: 946a 1311 0000 616a 8e03 0000 5d94 286a  .j....aj....].(j
 00010140: 9406 0000 6a95 0600 0065 6a90 0300 005d  ....j....ej....]
 00010150: 946a 9203 0000 5d94 6a94 0300 005d 946a  .j....].j....].j
 00010160: 9906 0000 8c1b 6575 7265 706f 632e 696e  ......eurepoc.in
@@ -4257,15 +4257,15 @@
 00010a00: 6765 7494 8c24 5f6d 6f64 756c 6573 2f65  get..$_modules/e
 00010a10: 7572 6570 6f63 2f69 6e63 6964 656e 745f  urepoc/incident_
 00010a20: 6461 7461 6672 616d 6573 948c 0572 6566  dataframes...ref
 00010a30: 6964 948c 3249 6e63 6964 656e 7444 6174  id..2IncidentDat
 00010a40: 6146 7261 6d65 4765 6e65 7261 746f 722e  aFrameGenerator.
 00010a50: 6765 745f 696c 5f62 7265 6163 685f 696e  get_il_breach_in
 00010a60: 6469 6361 746f 7294 8c06 7265 6664 6f63  dicator...refdoc
-00010a70: 946a 1a03 0000 756a 9603 0000 6a82 0600  .j....uj....j...
+00010a70: 946a 1903 0000 756a 9603 0000 6a82 0600  .j....uj....j...
 00010a80: 006a 8703 0000 6a80 1100 006a 8803 0000  .j....j....j....
 00010a90: 6a7b 0d00 0068 164e 6a89 0300 004e 7562  j{...h.Nj....Nub
 00010aa0: 656a 8a03 0000 7d94 286a 8c03 0000 5d94  ej....}.(j....].
 00010ab0: 6a7a 1100 0061 6a8e 0300 005d 9428 6a94  jz...aj....].(j.
 00010ac0: 0600 006a 9506 0000 656a 9003 0000 5d94  ...j....ej....].
 00010ad0: 6a92 0300 005d 946a 9403 0000 5d94 6a99  j....].j....].j.
 00010ae0: 0600 008c 1b65 7572 6570 6f63 2e69 6e63  .....eurepoc.inc
@@ -4399,15 +4399,15 @@
 000112e0: 7494 8c24 5f6d 6f64 756c 6573 2f65 7572  t..$_modules/eur
 000112f0: 6570 6f63 2f69 6e63 6964 656e 745f 6461  epoc/incident_da
 00011300: 7461 6672 616d 6573 948c 0572 6566 6964  taframes...refid
 00011310: 948c 3949 6e63 6964 656e 7444 6174 6146  ..9IncidentDataF
 00011320: 7261 6d65 4765 6e65 7261 746f 722e 6765  rameGenerator.ge
 00011330: 745f 696d 7061 6374 5f69 6e64 6963 6174  t_impact_indicat
 00011340: 6f72 5f76 6172 6961 626c 6573 948c 0672  or_variables...r
-00011350: 6566 646f 6394 6a1a 0300 0075 6a96 0300  efdoc.j....uj...
+00011350: 6566 646f 6394 6a19 0300 0075 6a96 0300  efdoc.j....uj...
 00011360: 006a 8206 0000 6a87 0300 006a e711 0000  .j....j....j....
 00011370: 6a88 0300 006a 7b0d 0000 6816 4e6a 8903  j....j{...h.Nj..
 00011380: 0000 4e75 6265 6a8a 0300 007d 9428 6a8c  ..Nubej....}.(j.
 00011390: 0300 005d 946a e111 0000 616a 8e03 0000  ...].j....aj....
 000113a0: 5d94 286a 9406 0000 6a95 0600 0065 6a90  ].(j....j....ej.
 000113b0: 0300 005d 946a 9203 0000 5d94 6a94 0300  ...].j....].j...
 000113c0: 005d 946a 9906 0000 8c1b 6575 7265 706f  .].j......eurepo
@@ -4569,15 +4569,15 @@
 00011d80: 0972 6566 7461 7267 6574 948c 245f 6d6f  .reftarget..$_mo
 00011d90: 6475 6c65 732f 6575 7265 706f 632f 696e  dules/eurepoc/in
 00011da0: 6369 6465 6e74 5f64 6174 6166 7261 6d65  cident_dataframe
 00011db0: 7394 8c05 7265 6669 6494 8c2d 496e 6369  s...refid..-Inci
 00011dc0: 6465 6e74 4461 7461 4672 616d 6547 656e  dentDataFrameGen
 00011dd0: 6572 6174 6f72 2e67 6574 5f69 6e63 6964  erator.get_incid
 00011de0: 656e 745f 7479 7065 7394 8c06 7265 6664  ent_types...refd
-00011df0: 6f63 946a 1a03 0000 756a 9603 0000 6a82  oc.j....uj....j.
+00011df0: 6f63 946a 1903 0000 756a 9603 0000 6a82  oc.j....uj....j.
 00011e00: 0600 006a 8703 0000 6a4e 1200 006a 8803  ...j....jN...j..
 00011e10: 0000 6a7b 0d00 0068 164e 6a89 0300 004e  ..j{...h.Nj....N
 00011e20: 7562 656a 8a03 0000 7d94 286a 8c03 0000  ubej....}.(j....
 00011e30: 5d94 6a48 1200 0061 6a8e 0300 005d 9428  ].jH...aj....].(
 00011e40: 6a94 0600 006a 9506 0000 656a 9003 0000  j....j....ej....
 00011e50: 5d94 6a92 0300 005d 946a 9403 0000 5d94  ].j....].j....].
 00011e60: 6a99 0600 008c 1b65 7572 6570 6f63 2e69  j......eurepoc.i
@@ -4702,15 +4702,15 @@
 000125d0: 8c09 7265 6674 6172 6765 7494 8c24 5f6d  ..reftarget..$_m
 000125e0: 6f64 756c 6573 2f65 7572 6570 6f63 2f69  odules/eurepoc/i
 000125f0: 6e63 6964 656e 745f 6461 7461 6672 616d  ncident_datafram
 00012600: 6573 948c 0572 6566 6964 948c 3149 6e63  es...refid..1Inc
 00012610: 6964 656e 7444 6174 6146 7261 6d65 4765  identDataFrameGe
 00012620: 6e65 7261 746f 722e 6765 745f 696e 636c  nerator.get_incl
 00012630: 7573 696f 6e5f 6372 6974 6572 6961 948c  usion_criteria..
-00012640: 0672 6566 646f 6394 6a1a 0300 0075 6a96  .refdoc.j....uj.
+00012640: 0672 6566 646f 6394 6a19 0300 0075 6a96  .refdoc.j....uj.
 00012650: 0300 006a 8206 0000 6a87 0300 006a b512  ...j....j....j..
 00012660: 0000 6a88 0300 006a 7b0d 0000 6816 4e6a  ..j....j{...h.Nj
 00012670: 8903 0000 4e75 6265 6a8a 0300 007d 9428  ....Nubej....}.(
 00012680: 6a8c 0300 005d 946a af12 0000 616a 8e03  j....].j....aj..
 00012690: 0000 5d94 286a 9406 0000 6a95 0600 0065  ..].(j....j....e
 000126a0: 6a90 0300 005d 946a 9203 0000 5d94 6a94  j....].j....].j.
 000126b0: 0300 005d 946a 9906 0000 8c1b 6575 7265  ...].j......eure
@@ -4875,15 +4875,15 @@
 000130a0: 0000 5d94 6a94 0300 005d 948c 0972 6566  ..].j....]...ref
 000130b0: 7461 7267 6574 948c 245f 6d6f 6475 6c65  target..$_module
 000130c0: 732f 6575 7265 706f 632f 696e 6369 6465  s/eurepoc/incide
 000130d0: 6e74 5f64 6174 6166 7261 6d65 7394 8c05  nt_dataframes...
 000130e0: 7265 6669 6494 8c29 496e 6369 6465 6e74  refid..)Incident
 000130f0: 4461 7461 4672 616d 6547 656e 6572 6174  DataFrameGenerat
 00013100: 6f72 2e67 6574 5f69 6e69 7469 6174 6f72  or.get_initiator
-00013110: 7394 8c06 7265 6664 6f63 946a 1a03 0000  s...refdoc.j....
+00013110: 7394 8c06 7265 6664 6f63 946a 1903 0000  s...refdoc.j....
 00013120: 756a 9603 0000 6a82 0600 006a 8703 0000  uj....j....j....
 00013130: 6a1c 1300 006a 8803 0000 6a7b 0d00 0068  j....j....j{...h
 00013140: 164e 6a89 0300 004e 7562 656a 8a03 0000  .Nj....Nubej....
 00013150: 7d94 286a 8c03 0000 5d94 6a16 1300 0061  }.(j....].j....a
 00013160: 6a8e 0300 005d 9428 6a94 0600 006a 9506  j....].(j....j..
 00013170: 0000 656a 9003 0000 5d94 6a92 0300 005d  ..ej....].j....]
 00013180: 946a 9403 0000 5d94 6a99 0600 008c 1b65  .j....].j......e
@@ -5021,15 +5021,15 @@
 000139c0: 7461 7267 6574 948c 245f 6d6f 6475 6c65  target..$_module
 000139d0: 732f 6575 7265 706f 632f 696e 6369 6465  s/eurepoc/incide
 000139e0: 6e74 5f64 6174 6166 7261 6d65 7394 8c05  nt_dataframes...
 000139f0: 7265 6669 6494 8c2e 496e 6369 6465 6e74  refid...Incident
 00013a00: 4461 7461 4672 616d 6547 656e 6572 6174  DataFrameGenerat
 00013a10: 6f72 2e67 6574 5f6c 6567 616c 5f72 6573  or.get_legal_res
 00013a20: 706f 6e73 6573 948c 0672 6566 646f 6394  ponses...refdoc.
-00013a30: 6a1a 0300 0075 6a96 0300 006a 8206 0000  j....uj....j....
+00013a30: 6a19 0300 0075 6a96 0300 006a 8206 0000  j....uj....j....
 00013a40: 6a87 0300 006a b813 0000 6a88 0300 006a  j....j....j....j
 00013a50: 7b0d 0000 6816 4e6a 8903 0000 4e75 6265  {...h.Nj....Nube
 00013a60: 6a8a 0300 007d 9428 6a8c 0300 005d 946a  j....}.(j....].j
 00013a70: b213 0000 616a 8e03 0000 5d94 286a 9406  ....aj....].(j..
 00013a80: 0000 6a95 0600 0065 6a90 0300 005d 946a  ..j....ej....].j
 00013a90: 9203 0000 5d94 6a94 0300 005d 946a 9906  ....].j....].j..
 00013aa0: 0000 8c1b 6575 7265 706f 632e 696e 6369  ....eurepoc.inci
@@ -5170,15 +5170,15 @@
 00014310: 7265 6674 6172 6765 7494 8c24 5f6d 6f64  reftarget..$_mod
 00014320: 756c 6573 2f65 7572 6570 6f63 2f69 6e63  ules/eurepoc/inc
 00014330: 6964 656e 745f 6461 7461 6672 616d 6573  ident_dataframes
 00014340: 948c 0572 6566 6964 948c 2e49 6e63 6964  ...refid...Incid
 00014350: 656e 7444 6174 6146 7261 6d65 4765 6e65  entDataFrameGene
 00014360: 7261 746f 722e 6765 745f 6c65 6761 6c5f  rator.get_legal_
 00014370: 7661 7269 6162 6c65 7394 8c06 7265 6664  variables...refd
-00014380: 6f63 946a 1a03 0000 756a 9603 0000 6a82  oc.j....uj....j.
+00014380: 6f63 946a 1903 0000 756a 9603 0000 6a82  oc.j....uj....j.
 00014390: 0600 006a 8703 0000 6a1f 1400 006a 8803  ...j....j....j..
 000143a0: 0000 6a7b 0d00 0068 164e 6a89 0300 004e  ..j{...h.Nj....N
 000143b0: 7562 656a 8a03 0000 7d94 286a 8c03 0000  ubej....}.(j....
 000143c0: 5d94 6a19 1400 0061 6a8e 0300 005d 9428  ].j....aj....].(
 000143d0: 6a94 0600 006a 9506 0000 656a 9003 0000  j....j....ej....
 000143e0: 5d94 6a92 0300 005d 946a 9403 0000 5d94  ].j....].j....].
 000143f0: 6a99 0600 008c 1b65 7572 6570 6f63 2e69  j......eurepoc.i
@@ -5307,15 +5307,15 @@
 00014ba0: 5d94 6a94 0300 005d 948c 0972 6566 7461  ].j....]...refta
 00014bb0: 7267 6574 948c 245f 6d6f 6475 6c65 732f  rget..$_modules/
 00014bc0: 6575 7265 706f 632f 696e 6369 6465 6e74  eurepoc/incident
 00014bd0: 5f64 6174 6166 7261 6d65 7394 8c05 7265  _dataframes...re
 00014be0: 6669 6494 8c28 496e 6369 6465 6e74 4461  fid..(IncidentDa
 00014bf0: 7461 4672 616d 6547 656e 6572 6174 6f72  taFrameGenerator
 00014c00: 2e67 6574 5f6d 6169 6e5f 6461 7461 948c  .get_main_data..
-00014c10: 0672 6566 646f 6394 6a1a 0300 0075 6a96  .refdoc.j....uj.
+00014c10: 0672 6566 646f 6394 6a19 0300 0075 6a96  .refdoc.j....uj.
 00014c20: 0300 006a 8206 0000 6a87 0300 006a 8614  ...j....j....j..
 00014c30: 0000 6a88 0300 006a 7b0d 0000 6816 4e6a  ..j....j{...h.Nj
 00014c40: 8903 0000 4e75 6265 6a8a 0300 007d 9428  ....Nubej....}.(
 00014c50: 6a8c 0300 005d 946a 8014 0000 616a 8e03  j....].j....aj..
 00014c60: 0000 5d94 286a 9406 0000 6a95 0600 0065  ..].(j....j....e
 00014c70: 6a90 0300 005d 946a 9203 0000 5d94 6a94  j....].j....].j.
 00014c80: 0300 005d 946a 9906 0000 8c1b 6575 7265  ...].j......eure
@@ -5457,15 +5457,15 @@
 00015500: 948c 0972 6566 7461 7267 6574 948c 245f  ...reftarget..$_
 00015510: 6d6f 6475 6c65 732f 6575 7265 706f 632f  modules/eurepoc/
 00015520: 696e 6369 6465 6e74 5f64 6174 6166 7261  incident_datafra
 00015530: 6d65 7394 8c05 7265 6669 6494 8c2b 496e  mes...refid..+In
 00015540: 6369 6465 6e74 4461 7461 4672 616d 6547  cidentDataFrameG
 00015550: 656e 6572 6174 6f72 2e67 6574 5f6d 6974  enerator.get_mit
 00015560: 7265 5f69 6d70 6163 7494 8c06 7265 6664  re_impact...refd
-00015570: 6f63 946a 1a03 0000 756a 9603 0000 6a82  oc.j....uj....j.
+00015570: 6f63 946a 1903 0000 756a 9603 0000 6a82  oc.j....uj....j.
 00015580: 0600 006a 8703 0000 6aed 1400 006a 8803  ...j....j....j..
 00015590: 0000 6a7b 0d00 0068 164e 6a89 0300 004e  ..j{...h.Nj....N
 000155a0: 7562 656a 8a03 0000 7d94 286a 8c03 0000  ubej....}.(j....
 000155b0: 5d94 6ae7 1400 0061 6a8e 0300 005d 9428  ].j....aj....].(
 000155c0: 6a94 0600 006a 9506 0000 656a 9003 0000  j....j....ej....
 000155d0: 5d94 6a92 0300 005d 946a 9403 0000 5d94  ].j....].j....].
 000155e0: 6a99 0600 008c 1b65 7572 6570 6f63 2e69  j......eurepoc.i
@@ -5591,15 +5591,15 @@
 00015d60: 6765 7494 8c24 5f6d 6f64 756c 6573 2f65  get..$_modules/e
 00015d70: 7572 6570 6f63 2f69 6e63 6964 656e 745f  urepoc/incident_
 00015d80: 6461 7461 6672 616d 6573 948c 0572 6566  dataframes...ref
 00015d90: 6964 948c 3349 6e63 6964 656e 7444 6174  id..3IncidentDat
 00015da0: 6146 7261 6d65 4765 6e65 7261 746f 722e  aFrameGenerator.
 00015db0: 6765 745f 6d69 7472 655f 696e 6974 6961  get_mitre_initia
 00015dc0: 6c5f 6163 6365 7373 948c 0672 6566 646f  l_access...refdo
-00015dd0: 6394 6a1a 0300 0075 6a96 0300 006a 8206  c.j....uj....j..
+00015dd0: 6394 6a19 0300 0075 6a96 0300 006a 8206  c.j....uj....j..
 00015de0: 0000 6a87 0300 006a 5415 0000 6a88 0300  ..j....jT...j...
 00015df0: 006a 7b0d 0000 6816 4e6a 8903 0000 4e75  .j{...h.Nj....Nu
 00015e00: 6265 6a8a 0300 007d 9428 6a8c 0300 005d  bej....}.(j....]
 00015e10: 946a 4e15 0000 616a 8e03 0000 5d94 286a  .jN...aj....].(j
 00015e20: 9406 0000 6a95 0600 0065 6a90 0300 005d  ....j....ej....]
 00015e30: 946a 9203 0000 5d94 6a94 0300 005d 946a  .j....].j....].j
 00015e40: 9906 0000 8c1b 6575 7265 706f 632e 696e  ......eurepoc.in
@@ -5725,15 +5725,15 @@
 000165c0: 5d94 8c09 7265 6674 6172 6765 7494 8c24  ]...reftarget..$
 000165d0: 5f6d 6f64 756c 6573 2f65 7572 6570 6f63  _modules/eurepoc
 000165e0: 2f69 6e63 6964 656e 745f 6461 7461 6672  /incident_datafr
 000165f0: 616d 6573 948c 0572 6566 6964 948c 3049  ames...refid..0I
 00016600: 6e63 6964 656e 7444 6174 6146 7261 6d65  ncidentDataFrame
 00016610: 4765 6e65 7261 746f 722e 6765 745f 6f66  Generator.get_of
 00016620: 666c 696e 655f 636f 6e66 6c69 6374 7394  fline_conflicts.
-00016630: 8c06 7265 6664 6f63 946a 1a03 0000 756a  ..refdoc.j....uj
+00016630: 8c06 7265 6664 6f63 946a 1903 0000 756a  ..refdoc.j....uj
 00016640: 9603 0000 6a82 0600 006a 8703 0000 6abb  ....j....j....j.
 00016650: 1500 006a 8803 0000 6a7b 0d00 0068 164e  ...j....j{...h.N
 00016660: 6a89 0300 004e 7562 656a 8a03 0000 7d94  j....Nubej....}.
 00016670: 286a 8c03 0000 5d94 6ab5 1500 0061 6a8e  (j....].j....aj.
 00016680: 0300 005d 9428 6a94 0600 006a 9506 0000  ...].(j....j....
 00016690: 656a 9003 0000 5d94 6a92 0300 005d 946a  ej....].j....].j
 000166a0: 9403 0000 5d94 6a99 0600 008c 1b65 7572  ....].j......eur
@@ -5869,15 +5869,15 @@
 00016ec0: 6a94 0300 005d 948c 0972 6566 7461 7267  j....]...reftarg
 00016ed0: 6574 948c 245f 6d6f 6475 6c65 732f 6575  et..$_modules/eu
 00016ee0: 7265 706f 632f 696e 6369 6465 6e74 5f64  repoc/incident_d
 00016ef0: 6174 6166 7261 6d65 7394 8c05 7265 6669  ataframes...refi
 00016f00: 6494 8c2e 496e 6369 6465 6e74 4461 7461  d...IncidentData
 00016f10: 4672 616d 6547 656e 6572 6174 6f72 2e67  FrameGenerator.g
 00016f20: 6574 5f6f 7065 7261 7469 6f6e 5f74 7970  et_operation_typ
-00016f30: 6573 948c 0672 6566 646f 6394 6a1a 0300  es...refdoc.j...
+00016f30: 6573 948c 0672 6566 646f 6394 6a19 0300  es...refdoc.j...
 00016f40: 0075 6a96 0300 006a 8206 0000 6a87 0300  .uj....j....j...
 00016f50: 006a 2216 0000 6a88 0300 006a 7b0d 0000  .j"...j....j{...
 00016f60: 6816 4e6a 8903 0000 4e75 6265 6a8a 0300  h.Nj....Nubej...
 00016f70: 007d 9428 6a8c 0300 005d 946a 1c16 0000  .}.(j....].j....
 00016f80: 616a 8e03 0000 5d94 286a 9406 0000 6a95  aj....].(j....j.
 00016f90: 0600 0065 6a90 0300 005d 946a 9203 0000  ...ej....].j....
 00016fa0: 5d94 6a94 0300 005d 946a 9906 0000 8c1b  ].j....].j......
@@ -6003,15 +6003,15 @@
 00017720: 0000 5d94 8c09 7265 6674 6172 6765 7494  ..]...reftarget.
 00017730: 8c24 5f6d 6f64 756c 6573 2f65 7572 6570  .$_modules/eurep
 00017740: 6f63 2f69 6e63 6964 656e 745f 6461 7461  oc/incident_data
 00017750: 6672 616d 6573 948c 0572 6566 6964 948c  frames...refid..
 00017760: 3249 6e63 6964 656e 7444 6174 6146 7261  2IncidentDataFra
 00017770: 6d65 4765 6e65 7261 746f 722e 6765 745f  meGenerator.get_
 00017780: 706f 6c69 7469 6361 6c5f 7265 7370 6f6e  political_respon
-00017790: 7365 7394 8c06 7265 6664 6f63 946a 1a03  ses...refdoc.j..
+00017790: 7365 7394 8c06 7265 6664 6f63 946a 1903  ses...refdoc.j..
 000177a0: 0000 756a 9603 0000 6a82 0600 006a 8703  ..uj....j....j..
 000177b0: 0000 6a89 1600 006a 8803 0000 6a7b 0d00  ..j....j....j{..
 000177c0: 0068 164e 6a89 0300 004e 7562 656a 8a03  .h.Nj....Nubej..
 000177d0: 0000 7d94 286a 8c03 0000 5d94 6a83 1600  ..}.(j....].j...
 000177e0: 0061 6a8e 0300 005d 9428 6a94 0600 006a  .aj....].(j....j
 000177f0: 9506 0000 656a 9003 0000 5d94 6a92 0300  ....ej....].j...
 00017800: 005d 946a 9403 0000 5d94 6a99 0600 008c  .].j....].j.....
@@ -6153,15 +6153,15 @@
 00018080: 5d94 6a94 0300 005d 948c 0972 6566 7461  ].j....]...refta
 00018090: 7267 6574 948c 245f 6d6f 6475 6c65 732f  rget..$_modules/
 000180a0: 6575 7265 706f 632f 696e 6369 6465 6e74  eurepoc/incident
 000180b0: 5f64 6174 6166 7261 6d65 7394 8c05 7265  _dataframes...re
 000180c0: 6669 6494 8c28 496e 6369 6465 6e74 4461  fid..(IncidentDa
 000180d0: 7461 4672 616d 6547 656e 6572 6174 6f72  taFrameGenerator
 000180e0: 2e67 6574 5f72 6563 6569 7665 7273 948c  .get_receivers..
-000180f0: 0672 6566 646f 6394 6a1a 0300 0075 6a96  .refdoc.j....uj.
+000180f0: 0672 6566 646f 6394 6a19 0300 0075 6a96  .refdoc.j....uj.
 00018100: 0300 006a 8206 0000 6a87 0300 006a f016  ...j....j....j..
 00018110: 0000 6a88 0300 006a 7b0d 0000 6816 4e6a  ..j....j{...h.Nj
 00018120: 8903 0000 4e75 6265 6a8a 0300 007d 9428  ....Nubej....}.(
 00018130: 6a8c 0300 005d 946a ea16 0000 616a 8e03  j....].j....aj..
 00018140: 0000 5d94 286a 9406 0000 6a95 0600 0065  ..].(j....j....e
 00018150: 6a90 0300 005d 946a 9203 0000 5d94 6a94  j....].j....].j.
 00018160: 0300 005d 946a 9906 0000 8c1b 6575 7265  ...].j......eure
@@ -6304,15 +6304,15 @@
 000189f0: 005d 948c 0972 6566 7461 7267 6574 948c  .]...reftarget..
 00018a00: 245f 6d6f 6475 6c65 732f 6575 7265 706f  $_modules/eurepo
 00018a10: 632f 696e 6369 6465 6e74 5f64 6174 6166  c/incident_dataf
 00018a20: 7261 6d65 7394 8c05 7265 6669 6494 8c2b  rames...refid..+
 00018a30: 496e 6369 6465 6e74 4461 7461 4672 616d  IncidentDataFram
 00018a40: 6547 656e 6572 6174 6f72 2e67 6574 5f73  eGenerator.get_s
 00018a50: 6f75 7263 655f 6e61 6d65 7394 8c06 7265  ource_names...re
-00018a60: 6664 6f63 946a 1a03 0000 756a 9603 0000  fdoc.j....uj....
+00018a60: 6664 6f63 946a 1903 0000 756a 9603 0000  fdoc.j....uj....
 00018a70: 6a82 0600 006a 8703 0000 6a57 1700 006a  j....j....jW...j
 00018a80: 8803 0000 6a7b 0d00 0068 164e 6a89 0300  ....j{...h.Nj...
 00018a90: 004e 7562 656a 8a03 0000 7d94 286a 8c03  .Nubej....}.(j..
 00018aa0: 0000 5d94 6a51 1700 0061 6a8e 0300 005d  ..].jQ...aj....]
 00018ab0: 9428 6a94 0600 006a 9506 0000 656a 9003  .(j....j....ej..
 00018ac0: 0000 5d94 6a92 0300 005d 946a 9403 0000  ..].j....].j....
 00018ad0: 5d94 6a99 0600 008c 1b65 7572 6570 6f63  ].j......eurepoc
@@ -6440,15 +6440,15 @@
 00019270: 6566 7461 7267 6574 948c 245f 6d6f 6475  eftarget..$_modu
 00019280: 6c65 732f 6575 7265 706f 632f 696e 6369  les/eurepoc/inci
 00019290: 6465 6e74 5f64 6174 6166 7261 6d65 7394  dent_dataframes.
 000192a0: 8c05 7265 6669 6494 8c34 496e 6369 6465  ..refid..4Incide
 000192b0: 6e74 4461 7461 4672 616d 6547 656e 6572  ntDataFrameGener
 000192c0: 6174 6f72 2e67 6574 5f73 6f75 7263 6573  ator.get_sources
 000192d0: 5f6f 665f 6469 7363 6c6f 7375 7265 948c  _of_disclosure..
-000192e0: 0672 6566 646f 6394 6a1a 0300 0075 6a96  .refdoc.j....uj.
+000192e0: 0672 6566 646f 6394 6a19 0300 0075 6a96  .refdoc.j....uj.
 000192f0: 0300 006a 8206 0000 6a87 0300 006a be17  ...j....j....j..
 00019300: 0000 6a88 0300 006a 7b0d 0000 6816 4e6a  ..j....j{...h.Nj
 00019310: 8903 0000 4e75 6265 6a8a 0300 007d 9428  ....Nubej....}.(
 00019320: 6a8c 0300 005d 946a b817 0000 616a 8e03  j....].j....aj..
 00019330: 0000 5d94 286a 9406 0000 6a95 0600 0065  ..].(j....j....e
 00019340: 6a90 0300 005d 946a 9203 0000 5d94 6a94  j....].j....].j.
 00019350: 0300 005d 946a 9906 0000 8c1b 6575 7265  ...].j......eure
@@ -6572,15 +6572,15 @@
 00019ab0: 948c 0972 6566 7461 7267 6574 948c 245f  ...reftarget..$_
 00019ac0: 6d6f 6475 6c65 732f 6575 7265 706f 632f  modules/eurepoc/
 00019ad0: 696e 6369 6465 6e74 5f64 6174 6166 7261  incident_datafra
 00019ae0: 6d65 7394 8c05 7265 6669 6494 8c2b 496e  mes...refid..+In
 00019af0: 6369 6465 6e74 4461 7461 4672 616d 6547  cidentDataFrameG
 00019b00: 656e 6572 6174 6f72 2e67 6574 5f73 6f75  enerator.get_sou
 00019b10: 7263 6573 5f75 726c 7394 8c06 7265 6664  rces_urls...refd
-00019b20: 6f63 946a 1a03 0000 756a 9603 0000 6a82  oc.j....uj....j.
+00019b20: 6f63 946a 1903 0000 756a 9603 0000 6a82  oc.j....uj....j.
 00019b30: 0600 006a 8703 0000 6a25 1800 006a 8803  ...j....j%...j..
 00019b40: 0000 6a7b 0d00 0068 164e 6a89 0300 004e  ..j{...h.Nj....N
 00019b50: 7562 656a 8a03 0000 7d94 286a 8c03 0000  ubej....}.(j....
 00019b60: 5d94 6a1f 1800 0061 6a8e 0300 005d 9428  ].j....aj....].(
 00019b70: 6a94 0600 006a 9506 0000 656a 9003 0000  j....j....ej....
 00019b80: 5d94 6a92 0300 005d 946a 9403 0000 5d94  ].j....].j....].
 00019b90: 6a99 0600 008c 1b65 7572 6570 6f63 2e69  j......eurepoc.i
@@ -6707,15 +6707,15 @@
 0001a320: 6566 7461 7267 6574 948c 245f 6d6f 6475  eftarget..$_modu
 0001a330: 6c65 732f 6575 7265 706f 632f 696e 6369  les/eurepoc/inci
 0001a340: 6465 6e74 5f64 6174 6166 7261 6d65 7394  dent_dataframes.
 0001a350: 8c05 7265 6669 6494 8c32 496e 6369 6465  ..refid..2Incide
 0001a360: 6e74 4461 7461 4672 616d 6547 656e 6572  ntDataFrameGener
 0001a370: 6174 6f72 2e67 6574 5f74 6563 686e 6963  ator.get_technic
 0001a380: 616c 5f76 6172 6961 626c 6573 948c 0672  al_variables...r
-0001a390: 6566 646f 6394 6a1a 0300 0075 6a96 0300  efdoc.j....uj...
+0001a390: 6566 646f 6394 6a19 0300 0075 6a96 0300  efdoc.j....uj...
 0001a3a0: 006a 8206 0000 6a87 0300 006a 8c18 0000  .j....j....j....
 0001a3b0: 6a88 0300 006a 7b0d 0000 6816 4e6a 8903  j....j{...h.Nj..
 0001a3c0: 0000 4e75 6265 6a8a 0300 007d 9428 6a8c  ..Nubej....}.(j.
 0001a3d0: 0300 005d 946a 8618 0000 616a 8e03 0000  ...].j....aj....
 0001a3e0: 5d94 286a 9406 0000 6a95 0600 0065 6a90  ].(j....j....ej.
 0001a3f0: 0300 005d 946a 9203 0000 5d94 6a94 0300  ...].j....].j...
 0001a400: 005d 946a 9906 0000 8c1b 6575 7265 706f  .].j......eurepo
@@ -6879,15 +6879,15 @@
 0001ade0: 0300 005d 946a 9003 0000 5d94 6a92 0300  ...].j....].j...
 0001adf0: 005d 946a 9403 0000 5d94 8c05 6c65 7665  .].j....]...leve
 0001ae00: 6c94 4b01 8c04 7479 7065 946a 740d 0000  l.K...type.jt...
 0001ae10: 8c06 736f 7572 6365 946a d50d 0000 8c04  ..source.j......
 0001ae20: 6c69 6e65 944b 0175 6a96 0300 006a 5a0d  line.K.uj....jZ.
 0001ae30: 0000 7562 616a 770d 0000 4e6a 780d 0000  ..ubajw...Njx...
 0001ae40: 5d94 6a7a 0d00 004e 6a88 0300 006a 7b0d  ].jz...Nj....j{.
-0001ae50: 0000 7562 6a18 0300 006a 7003 0000 2981  ..ubj....jp...).
+0001ae50: 0000 7562 6a14 0300 006a 7003 0000 2981  ..ubj....jp...).
 0001ae60: 947d 9428 6a73 0300 0068 2f6a 7403 0000  .}.(js...h/jt...
 0001ae70: 5d94 6a77 0300 0029 8194 7d94 286a 7303  ].jw...)..}.(js.
 0001ae80: 0000 682f 6a74 0300 005d 9428 6a7c 0300  ..h/jt...].(j|..
 0001ae90: 0029 8194 7d94 286a 7303 0000 8c09 6461  .)..}.(js.....da
 0001aea0: 7465 5f74 7970 6594 6a74 0300 005d 946a  te_type.jt...].j
 0001aeb0: 8203 0000 8c09 6461 7465 5f74 7970 6594  ......date_type.
 0001aec0: 8594 8194 7d94 286a 8703 0000 6a39 1900  ....}.(j....j9..
@@ -7159,15 +7159,15 @@
 0001bf60: 6a42 0d00 005d 946a 440d 0000 5d94 6a46  jB...].jD...].jF
 0001bf70: 0d00 005d 946a 480d 0000 5d94 6a4a 0d00  ...].jH...].jJ..
 0001bf80: 005d 946a 4c0d 0000 5d94 6a4e 0d00 004b  .].jL...].jN...K
 0001bf90: 016a 4f0d 0000 4b00 6a50 0d00 006a 520d  .jO...K.jP...jR.
 0001bfa0: 0000 7d94 8594 5294 6a56 0d00 005d 946a  ..}...R.jV...].j
 0001bfb0: 580d 0000 5d94 6a77 0d00 004e 6a78 0d00  X...].jw...Njx..
 0001bfc0: 005d 946a 7a0d 0000 4e6a 8803 0000 6a33  .].jz...Nj....j3
-0001bfd0: 1900 0075 626a 1403 0000 6a70 0300 0029  ...ubj....jp...)
+0001bfd0: 1900 0075 626a 1803 0000 6a70 0300 0029  ...ubj....jp...)
 0001bfe0: 8194 7d94 286a 7303 0000 682f 6a74 0300  ..}.(js...h/jt..
 0001bff0: 005d 946a 7703 0000 2981 947d 9428 6a73  .].jw...)..}.(js
 0001c000: 0300 0068 2f6a 7403 0000 5d94 6a7c 0300  ...h/jt...].j|..
 0001c010: 0029 8194 7d94 286a 7303 0000 8c09 666c  .)..}.(js.....fl
 0001c020: 6167 5f74 7970 6594 6a74 0300 005d 946a  ag_type.jt...].j
 0001c030: 8203 0000 8c09 666c 6167 5f74 7970 6594  ......flag_type.
 0001c040: 8594 8194 7d94 286a 8703 0000 6a2a 1a00  ....}.(j....j*..
@@ -7234,15 +7234,15 @@
 0001c410: 946a 440d 0000 5d94 6a46 0d00 005d 946a  .jD...].jF...].j
 0001c420: 480d 0000 5d94 6a4a 0d00 005d 946a 4c0d  H...].jJ...].jL.
 0001c430: 0000 5d94 6a4e 0d00 004b 016a 4f0d 0000  ..].jN...K.jO...
 0001c440: 4b00 6a50 0d00 006a 520d 0000 7d94 8594  K.jP...jR...}...
 0001c450: 5294 6a56 0d00 005d 946a 580d 0000 5d94  R.jV...].jX...].
 0001c460: 6a77 0d00 004e 6a78 0d00 005d 946a 7a0d  jw...Njx...].jz.
 0001c470: 0000 4e6a 8803 0000 6a24 1a00 0075 626a  ..Nj....j$...ubj
-0001c480: 1503 0000 6a70 0300 0029 8194 7d94 286a  ....jp...)..}.(j
+0001c480: 1303 0000 6a70 0300 0029 8194 7d94 286a  ....jp...)..}.(j
 0001c490: 7303 0000 682f 6a74 0300 005d 9428 6a76  s...h/jt...].(jv
 0001c4a0: 0300 008c 0763 6f6d 6d65 6e74 9493 9429  .....comment...)
 0001c4b0: 8194 7d94 286a 7303 0000 8ccc 6575 7265  ..}.(js.....eure
 0001c4c0: 706f 6320 646f 6375 6d65 6e74 6174 696f  poc documentatio
 0001c4d0: 6e20 6d61 7374 6572 2066 696c 652c 2063  n master file, c
 0001c4e0: 7265 6174 6564 2062 790a 7370 6869 6e78  reated by.sphinx
 0001c4f0: 2d71 7569 636b 7374 6172 7420 6f6e 2046  -quickstart on F
@@ -7615,15 +7615,15 @@
 0001dbe0: 6a61 1a00 0068 166a 741a 0000 6a89 0300  ja...h.jt...j...
 0001dbf0: 004b 3375 626a c703 0000 2981 947d 9428  .K3ubj....)..}.(
 0001dc00: 6a73 0300 0068 2f6a 7403 0000 5d94 6acc  js...h/jt...].j.
 0001dc10: 0300 0029 8194 7d94 286a 7303 0000 682f  ...)..}.(js...h/
 0001dc20: 6a74 0300 005d 946a 8a03 0000 7d94 286a  jt...].j....}.(j
 0001dc30: 8c03 0000 5d94 6a8e 0300 005d 946a 9003  ....].j....].j..
 0001dc40: 0000 5d94 6a92 0300 005d 946a 9403 0000  ..].j....].j....
-0001dc50: 5d94 6a87 0300 006a 1503 0000 6ad6 0300  ].j....j....j...
+0001dc50: 5d94 6a87 0300 006a 1303 0000 6ad6 0300  ].j....j....j...
 0001dc60: 005d 9428 4e8c 0a72 6561 645f 746f 6b65  .].(N..read_toke
 0001dc70: 6e94 8694 4e8c 0d44 6174 6162 6173 6551  n...N..DatabaseQ
 0001dc80: 7565 7279 9486 944e 8c1a 496e 6369 6465  uery...N..Incide
 0001dc90: 6e74 4461 7461 4672 616d 6547 656e 6572  ntDataFrameGener
 0001dca0: 6174 6f72 9486 9465 6ae4 0300 005d 9428  ator...ej....].(
 0001dcb0: 6a6b 1b00 006a 6d1b 0000 6a6f 1b00 0065  jk...jm...jo...e
 0001dcc0: 6ae6 0300 004b 016a e703 0000 8c09 436f  j....K.j......Co
@@ -7677,15 +7677,15 @@
 0001dfc0: 0300 005d 9428 6abe 0600 008c 0373 7464  ...].(j......std
 0001dfd0: 948c 0773 7464 2d72 6566 9465 6a90 0300  ...std-ref.ej...
 0001dfe0: 005d 946a 9203 0000 5d94 6a94 0300 005d  .].j....].j....]
 0001dff0: 9475 6a96 0300 0068 a66a 8703 0000 6a9e  .uj....h.j....j.
 0001e000: 1b00 0075 6261 6a8a 0300 007d 9428 6a8c  ...ubaj....}.(j.
 0001e010: 0300 005d 946a 8e03 0000 5d94 6a90 0300  ...].j....].j...
 0001e020: 005d 946a 9203 0000 5d94 6a94 0300 005d  .].j....].j....]
-0001e030: 948c 0672 6566 646f 6394 6a15 0300 008c  ...refdoc.j.....
+0001e030: 948c 0672 6566 646f 6394 6a13 0300 008c  ...refdoc.j.....
 0001e040: 0972 6566 646f 6d61 696e 946a ab1b 0000  .refdomain.j....
 0001e050: 8c07 7265 6674 7970 6594 8c03 7265 6694  ..reftype...ref.
 0001e060: 8c0b 7265 6665 7870 6c69 6369 7494 898c  ..refexplicit...
 0001e070: 0772 6566 7761 726e 9488 6ad2 0600 008c  .refwarn..j.....
 0001e080: 0673 6561 7263 6894 756a 9603 0000 6aac  .search.uj....j.
 0001e090: 0600 0068 166a 741a 0000 6a89 0300 004b  ...h.jt...j....K
 0001e0a0: 406a 8703 0000 6a9b 1b00 0075 6261 6a8a  @j....j....ubaj.
@@ -7763,15 +7763,15 @@
 0001e520: 0d00 007d 946a 420d 0000 5d94 6a44 0d00  ...}.jB...].jD..
 0001e530: 005d 946a 460d 0000 5d94 6a48 0d00 005d  .].jF...].jH...]
 0001e540: 946a 4a0d 0000 5d94 6a4c 0d00 005d 946a  .jJ...].jL...].j
 0001e550: 4e0d 0000 4b01 6a4f 0d00 004b 006a 500d  N...K.jO...K.jP.
 0001e560: 0000 6a52 0d00 007d 9485 9452 946a 560d  ..jR...}...R.jV.
 0001e570: 0000 5d94 6a58 0d00 005d 946a 770d 0000  ..].jX...].jw...
 0001e580: 4e6a 780d 0000 5d94 6a7a 0d00 004e 6a88  Njx...].jz...Nj.
-0001e590: 0300 006a 611a 0000 7562 6a19 0300 006a  ...ja...ubj....j
+0001e590: 0300 006a 611a 0000 7562 6a15 0300 006a  ...ja...ubj....j
 0001e5a0: 7003 0000 2981 947d 9428 6a73 0300 0068  p...)..}.(js...h
 0001e5b0: 2f6a 7403 0000 5d94 6a77 0300 0029 8194  /jt...].jw...)..
 0001e5c0: 7d94 286a 7303 0000 682f 6a74 0300 005d  }.(js...h/jt...]
 0001e5d0: 9428 6a7c 0300 0029 8194 7d94 286a 7303  .(j|...)..}.(js.
 0001e5e0: 0000 8c11 696e 6974 6961 746f 725f 636f  ....initiator_co
 0001e5f0: 756e 7472 7994 6a74 0300 005d 946a 8203  untry.jt...].j..
 0001e600: 0000 8c11 696e 6974 6961 746f 725f 636f  ....initiator_co
@@ -12763,15 +12763,15 @@
 00031da0: 7d94 6a40 0d00 007d 946a 420d 0000 5d94  }.j@...}.jB...].
 00031db0: 6a44 0d00 005d 946a 460d 0000 5d94 6a48  jD...].jF...].jH
 00031dc0: 0d00 005d 946a 4a0d 0000 5d94 6a4c 0d00  ...].jJ...].jL..
 00031dd0: 005d 946a 4e0d 0000 4b01 6a4f 0d00 004b  .].jN...K.jO...K
 00031de0: 006a 500d 0000 6a52 0d00 007d 9485 9452  .jP...jR...}...R
 00031df0: 946a 560d 0000 5d94 6a58 0d00 005d 946a  .jV...].jX...].j
 00031e00: 770d 0000 4e6a 780d 0000 5d94 6a7a 0d00  w...Njx...].jz..
-00031e10: 004e 6a88 0300 006a f81b 0000 7562 6a11  .Nj....j....ubj.
+00031e10: 004e 6a88 0300 006a f81b 0000 7562 6a1a  .Nj....j....ubj.
 00031e20: 0300 006a 7003 0000 2981 947d 9428 6a73  ...jp...)..}.(js
 00031e30: 0300 0068 2f6a 7403 0000 5d94 6a77 0300  ...h/jt...].jw..
 00031e40: 0029 8194 7d94 286a 7303 0000 682f 6a74  .)..}.(js...h/jt
 00031e50: 0300 005d 9428 6a7c 0300 0029 8194 7d94  ...].(j|...)..}.
 00031e60: 286a 7303 0000 8c0a 7265 6164 5f74 6f6b  (js.....read_tok
 00031e70: 656e 946a 7403 0000 5d94 6a82 0300 008c  en.jt...].j.....
 00031e80: 0a72 6561 645f 746f 6b65 6e94 8594 8194  .read_token.....
@@ -12904,15 +12904,15 @@
 00032670: 286a 7303 0000 682f 6a74 0300 005d 946a  (js...h/jt...].j
 00032680: 8a03 0000 7d94 286a 8c03 0000 5d94 6a8e  ....}.(j....].j.
 00032690: 0300 005d 946a 9003 0000 5d94 6a92 0300  ...].j....].j...
 000326a0: 005d 946a 9403 0000 5d94 8c09 7265 6674  .].j....]...reft
 000326b0: 6172 6765 7494 8c1b 5f6d 6f64 756c 6573  arget..._modules
 000326c0: 2f65 7572 6570 6f63 2f72 6561 645f 746f  /eurepoc/read_to
 000326d0: 6b65 6e94 8c05 7265 6669 6494 6a6d 3400  ken...refid.jm4.
-000326e0: 008c 0672 6566 646f 6394 6a11 0300 0075  ...refdoc.j....u
+000326e0: 008c 0672 6566 646f 6394 6a1a 0300 0075  ...refdoc.j....u
 000326f0: 6a96 0300 006a 8206 0000 6a87 0300 006a  j....j....j....j
 00032700: 5834 0000 6a88 0300 006a 2434 0000 6816  X4..j....j$4..h.
 00032710: 4e6a 8903 0000 4e75 6265 6a8a 0300 007d  Nj....Nubej....}
 00032720: 9428 6a8c 0300 005d 946a 5334 0000 616a  .(j....].jS4..aj
 00032730: 8e03 0000 5d94 286a 9406 0000 6a95 0600  ....].(j....j...
 00032740: 0065 6a90 0300 005d 946a 9203 0000 5d94  .ej....].j....].
 00032750: 6a94 0300 005d 946a 9906 0000 8c12 6575  j....].j......eu
@@ -13363,15 +13363,15 @@
 00034320: 0d00 007d 946a 420d 0000 5d94 6a44 0d00  ...}.jB...].jD..
 00034330: 005d 946a 460d 0000 5d94 6a48 0d00 005d  .].jF...].jH...]
 00034340: 946a 4a0d 0000 5d94 6a4c 0d00 005d 946a  .jJ...].jL...].j
 00034350: 4e0d 0000 4b01 6a4f 0d00 004b 006a 500d  N...K.jO...K.jP.
 00034360: 0000 6a52 0d00 007d 9485 9452 946a 560d  ..jR...}...R.jV.
 00034370: 0000 5d94 6a58 0d00 005d 946a 770d 0000  ..].jX...].jw...
 00034380: 4e6a 780d 0000 5d94 6a7a 0d00 004e 6a88  Njx...].jz...Nj.
-00034390: 0300 006a 2434 0000 7562 6a17 0300 006a  ...j$4..ubj....j
+00034390: 0300 006a 2434 0000 7562 6a11 0300 006a  ...j$4..ubj....j
 000343a0: 7003 0000 2981 947d 9428 6a73 0300 0068  p...)..}.(js...h
 000343b0: 2f6a 7403 0000 5d94 6a77 0300 0029 8194  /jt...].jw...)..
 000343c0: 7d94 286a 7303 0000 682f 6a74 0300 005d  }.(js...h/jt...]
 000343d0: 9428 6a7c 0300 0029 8194 7d94 286a 7303  .(j|...)..}.(js.
 000343e0: 0000 8c11 7265 6365 6976 6572 5f63 6174  ....receiver_cat
 000343f0: 6567 6f72 7994 6a74 0300 005d 946a 8203  egory.jt...].j..
 00034400: 0000 8c11 7265 6365 6976 6572 5f63 6174  ....receiver_cat
@@ -13811,15 +13811,15 @@
 00035f20: 6a40 0d00 007d 946a 420d 0000 5d94 6a44  j@...}.jB...].jD
 00035f30: 0d00 005d 946a 460d 0000 5d94 6a48 0d00  ...].jF...].jH..
 00035f40: 005d 946a 4a0d 0000 5d94 6a4c 0d00 005d  .].jJ...].jL...]
 00035f50: 946a 4e0d 0000 4b01 6a4f 0d00 004b 006a  .jN...K.jO...K.j
 00035f60: 500d 0000 6a52 0d00 007d 9485 9452 946a  P...jR...}...R.j
 00035f70: 560d 0000 5d94 6a58 0d00 005d 946a 770d  V...].jX...].jw.
 00035f80: 0000 4e6a 780d 0000 5d94 6a7a 0d00 004e  ..Njx...].jz...N
-00035f90: 6a88 0300 006a c236 0000 7562 6a16 0300  j....j.6..ubj...
+00035f90: 6a88 0300 006a c236 0000 7562 6a17 0300  j....j.6..ubj...
 00035fa0: 006a 7003 0000 2981 947d 9428 6a73 0300  .jp...)..}.(js..
 00035fb0: 0068 2f6a 7403 0000 5d94 6a77 0300 0029  .h/jt...].jw...)
 00035fc0: 8194 7d94 286a 7303 0000 682f 6a74 0300  ..}.(js...h/jt..
 00035fd0: 005d 9428 6a7c 0300 0029 8194 7d94 286a  .].(j|...)..}.(j
 00035fe0: 7303 0000 8c10 7265 6365 6976 6572 5f63  s.....receiver_c
 00035ff0: 6f75 6e74 7279 946a 7403 0000 5d94 6a82  ountry.jt...].j.
 00036000: 0300 008c 1072 6563 6569 7665 725f 636f  .....receiver_co
@@ -18808,15 +18808,15 @@
 00049770: 0000 5d94 6a44 0d00 005d 946a 460d 0000  ..].jD...].jF...
 00049780: 5d94 6a48 0d00 005d 946a 4a0d 0000 5d94  ].jH...].jJ...].
 00049790: 6a4c 0d00 005d 946a 4e0d 0000 4b01 6a4f  jL...].jN...K.jO
 000497a0: 0d00 004b 006a 500d 0000 6a52 0d00 007d  ...K.jP...jR...}
 000497b0: 9485 9452 946a 560d 0000 5d94 6a58 0d00  ...R.jV...].jX..
 000497c0: 005d 946a 770d 0000 4e6a 780d 0000 5d94  .].jw...Njx...].
 000497d0: 6a7a 0d00 004e 6a88 0300 006a 9638 0000  jz...Nj....j.8..
-000497e0: 7562 6a13 0300 006a 7003 0000 2981 947d  ubj....jp...)..}
+000497e0: 7562 6a16 0300 006a 7003 0000 2981 947d  ubj....jp...)..}
 000497f0: 9428 6a73 0300 0068 2f6a 7403 0000 5d94  .(js...h/jt...].
 00049800: 6a77 0300 0029 8194 7d94 286a 7303 0000  jw...)..}.(js...
 00049810: 682f 6a74 0300 005d 9428 6a7c 0300 0029  h/jt...].(j|...)
 00049820: 8194 7d94 286a 7303 0000 8c0f 7265 6365  ..}.(js.....rece
 00049830: 6976 6572 5f72 6567 696f 6e94 6a74 0300  iver_region.jt..
 00049840: 005d 946a 8203 0000 8c0f 7265 6365 6976  .].j......receiv
 00049850: 6572 5f72 6567 696f 6e94 8594 8194 7d94  er_region.....}.
@@ -19922,95 +19922,95 @@
 0004dd10: 7c03 0000 2981 947d 9428 6a73 0300 0068  |...)..}.(js...h
 0004dd20: 2f6a 7403 0000 5d94 6a82 0300 008c 0d44  /jt...].j......D
 0004dd30: 6174 6162 6173 6551 7565 7279 9485 9481  atabaseQuery....
 0004dd40: 947d 946a 8703 0000 6a20 5600 0073 6261  .}.j....j V..sba
 0004dd50: 6a8a 0300 007d 9428 6a8c 0300 005d 946a  j....}.(j....].j
 0004dd60: 8e03 0000 5d94 6a90 0300 005d 946a 9203  ....].j....].j..
 0004dd70: 0000 5d94 6a94 0300 005d 9475 6a96 0300  ..].j....].uj...
-0004dd80: 006a 7b03 0000 7562 6a1a 0300 006a 7c03  .j{...ubj....j|.
+0004dd80: 006a 7b03 0000 7562 6a19 0300 006a 7c03  .j{...ubj....j|.
 0004dd90: 0000 2981 947d 9428 6a73 0300 0068 2f6a  ..)..}.(js...h/j
 0004dda0: 7403 0000 5d94 6a82 0300 008c 1a49 6e63  t...].j......Inc
 0004ddb0: 6964 656e 7444 6174 6146 7261 6d65 4765  identDataFrameGe
 0004ddc0: 6e65 7261 746f 7294 8594 8194 7d94 6a87  nerator.....}.j.
 0004ddd0: 0300 006a 2d56 0000 7362 616a 8a03 0000  ...j-V..sbaj....
 0004dde0: 7d94 286a 8c03 0000 5d94 6a8e 0300 005d  }.(j....].j....]
 0004ddf0: 946a 9003 0000 5d94 6a92 0300 005d 946a  .j....].j....].j
 0004de00: 9403 0000 5d94 756a 9603 0000 6a7b 0300  ....].uj....j{..
-0004de10: 0075 626a 1803 0000 6a7c 0300 0029 8194  .ubj....j|...)..
+0004de10: 0075 626a 1403 0000 6a7c 0300 0029 8194  .ubj....j|...)..
 0004de20: 7d94 286a 7303 0000 682f 6a74 0300 005d  }.(js...h/jt...]
 0004de30: 946a 8203 0000 8c09 6461 7465 5f74 7970  .j......date_typ
 0004de40: 6594 8594 8194 7d94 6a87 0300 006a 3a56  e.....}.j....j:V
 0004de50: 0000 7362 616a 8a03 0000 7d94 286a 8c03  ..sbaj....}.(j..
 0004de60: 0000 5d94 6a8e 0300 005d 946a 9003 0000  ..].j....].j....
 0004de70: 5d94 6a92 0300 005d 946a 9403 0000 5d94  ].j....].j....].
-0004de80: 756a 9603 0000 6a7b 0300 0075 626a 1403  uj....j{...ubj..
+0004de80: 756a 9603 0000 6a7b 0300 0075 626a 1803  uj....j{...ubj..
 0004de90: 0000 6a7c 0300 0029 8194 7d94 286a 7303  ..j|...)..}.(js.
 0004dea0: 0000 682f 6a74 0300 005d 946a 8203 0000  ..h/jt...].j....
 0004deb0: 8c09 666c 6167 5f74 7970 6594 8594 8194  ..flag_type.....
 0004dec0: 7d94 6a87 0300 006a 4756 0000 7362 616a  }.j....jGV..sbaj
 0004ded0: 8a03 0000 7d94 286a 8c03 0000 5d94 6a8e  ....}.(j....].j.
 0004dee0: 0300 005d 946a 9003 0000 5d94 6a92 0300  ...].j....].j...
 0004def0: 005d 946a 9403 0000 5d94 756a 9603 0000  .].j....].uj....
-0004df00: 6a7b 0300 0075 626a 1503 0000 6a7c 0300  j{...ubj....j|..
+0004df00: 6a7b 0300 0075 626a 1303 0000 6a7c 0300  j{...ubj....j|..
 0004df10: 0029 8194 7d94 286a 7303 0000 682f 6a74  .)..}.(js...h/jt
 0004df20: 0300 005d 946a 8203 0000 8c1d 4575 5265  ...].j......EuRe
 0004df30: 706f 4320 5061 636b 6167 6520 446f 6375  poC Package Docu
 0004df40: 6d65 6e74 6174 696f 6e94 8594 8194 7d94  mentation.....}.
 0004df50: 6a87 0300 006a 5456 0000 7362 616a 8a03  j....jTV..sbaj..
 0004df60: 0000 7d94 286a 8c03 0000 5d94 6a8e 0300  ..}.(j....].j...
 0004df70: 005d 946a 9003 0000 5d94 6a92 0300 005d  .].j....].j....]
 0004df80: 946a 9403 0000 5d94 756a 9603 0000 6a7b  .j....].uj....j{
-0004df90: 0300 0075 626a 1903 0000 6a7c 0300 0029  ...ubj....j|...)
+0004df90: 0300 0075 626a 1503 0000 6a7c 0300 0029  ...ubj....j|...)
 0004dfa0: 8194 7d94 286a 7303 0000 682f 6a74 0300  ..}.(js...h/jt..
 0004dfb0: 005d 946a 8203 0000 8c11 696e 6974 6961  .].j......initia
 0004dfc0: 746f 725f 636f 756e 7472 7994 8594 8194  tor_country.....
 0004dfd0: 7d94 6a87 0300 006a 6156 0000 7362 616a  }.j....jaV..sbaj
 0004dfe0: 8a03 0000 7d94 286a 8c03 0000 5d94 6a8e  ....}.(j....].j.
 0004dff0: 0300 005d 946a 9003 0000 5d94 6a92 0300  ...].j....].j...
 0004e000: 005d 946a 9403 0000 5d94 756a 9603 0000  .].j....].uj....
-0004e010: 6a7b 0300 0075 626a 1103 0000 6a7c 0300  j{...ubj....j|..
+0004e010: 6a7b 0300 0075 626a 1a03 0000 6a7c 0300  j{...ubj....j|..
 0004e020: 0029 8194 7d94 286a 7303 0000 682f 6a74  .)..}.(js...h/jt
 0004e030: 0300 005d 946a 8203 0000 8c0a 7265 6164  ...].j......read
 0004e040: 5f74 6f6b 656e 9485 9481 947d 946a 8703  _token.....}.j..
 0004e050: 0000 6a6e 5600 0073 6261 6a8a 0300 007d  ..jnV..sbaj....}
 0004e060: 9428 6a8c 0300 005d 946a 8e03 0000 5d94  .(j....].j....].
 0004e070: 6a90 0300 005d 946a 9203 0000 5d94 6a94  j....].j....].j.
 0004e080: 0300 005d 9475 6a96 0300 006a 7b03 0000  ...].uj....j{...
-0004e090: 7562 6a17 0300 006a 7c03 0000 2981 947d  ubj....j|...)..}
+0004e090: 7562 6a11 0300 006a 7c03 0000 2981 947d  ubj....j|...)..}
 0004e0a0: 9428 6a73 0300 0068 2f6a 7403 0000 5d94  .(js...h/jt...].
 0004e0b0: 6a82 0300 008c 1172 6563 6569 7665 725f  j......receiver_
 0004e0c0: 6361 7465 676f 7279 9485 9481 947d 946a  category.....}.j
 0004e0d0: 8703 0000 6a7b 5600 0073 6261 6a8a 0300  ....j{V..sbaj...
 0004e0e0: 007d 9428 6a8c 0300 005d 946a 8e03 0000  .}.(j....].j....
 0004e0f0: 5d94 6a90 0300 005d 946a 9203 0000 5d94  ].j....].j....].
 0004e100: 6a94 0300 005d 9475 6a96 0300 006a 7b03  j....].uj....j{.
-0004e110: 0000 7562 6a16 0300 006a 7c03 0000 2981  ..ubj....j|...).
+0004e110: 0000 7562 6a17 0300 006a 7c03 0000 2981  ..ubj....j|...).
 0004e120: 947d 9428 6a73 0300 0068 2f6a 7403 0000  .}.(js...h/jt...
 0004e130: 5d94 6a82 0300 008c 1072 6563 6569 7665  ].j......receive
 0004e140: 725f 636f 756e 7472 7994 8594 8194 7d94  r_country.....}.
 0004e150: 6a87 0300 006a 8856 0000 7362 616a 8a03  j....j.V..sbaj..
 0004e160: 0000 7d94 286a 8c03 0000 5d94 6a8e 0300  ..}.(j....].j...
 0004e170: 005d 946a 9003 0000 5d94 6a92 0300 005d  .].j....].j....]
 0004e180: 946a 9403 0000 5d94 756a 9603 0000 6a7b  .j....].uj....j{
-0004e190: 0300 0075 626a 1303 0000 6a7c 0300 0029  ...ubj....j|...)
+0004e190: 0300 0075 626a 1603 0000 6a7c 0300 0029  ...ubj....j|...)
 0004e1a0: 8194 7d94 286a 7303 0000 682f 6a74 0300  ..}.(js...h/jt..
 0004e1b0: 005d 946a 8203 0000 8c0f 7265 6365 6976  .].j......receiv
 0004e1c0: 6572 5f72 6567 696f 6e94 8594 8194 7d94  er_region.....}.
 0004e1d0: 6a87 0300 006a 9556 0000 7362 616a 8a03  j....j.V..sbaj..
 0004e1e0: 0000 7d94 286a 8c03 0000 5d94 6a8e 0300  ..}.(j....].j...
 0004e1f0: 005d 946a 9003 0000 5d94 6a92 0300 005d  .].j....].j....]
 0004e200: 946a 9403 0000 5d94 756a 9603 0000 6a7b  .j....].uj....j{
 0004e210: 0300 0075 6275 8c0a 6c6f 6e67 7469 746c  ...ubu..longtitl
 0004e220: 6573 947d 9428 6a12 0300 006a 2056 0000  es.}.(j....j V..
-0004e230: 6a1a 0300 006a 2d56 0000 6a18 0300 006a  j....j-V..j....j
-0004e240: 3a56 0000 6a14 0300 006a 4756 0000 6a15  :V..j....jGV..j.
-0004e250: 0300 006a 5456 0000 6a19 0300 006a 6156  ...jTV..j....jaV
-0004e260: 0000 6a11 0300 006a 6e56 0000 6a17 0300  ..j....jnV..j...
-0004e270: 006a 7b56 0000 6a16 0300 006a 8856 0000  .j{V..j....j.V..
-0004e280: 6a13 0300 006a 9556 0000 758c 0474 6f63  j....j.V..u..toc
+0004e230: 6a19 0300 006a 2d56 0000 6a14 0300 006a  j....j-V..j....j
+0004e240: 3a56 0000 6a18 0300 006a 4756 0000 6a13  :V..j....jGV..j.
+0004e250: 0300 006a 5456 0000 6a15 0300 006a 6156  ...jTV..j....jaV
+0004e260: 0000 6a1a 0300 006a 6e56 0000 6a11 0300  ..j....jnV..j...
+0004e270: 006a 7b56 0000 6a17 0300 006a 8856 0000  .j{V..j....j.V..
+0004e280: 6a16 0300 006a 9556 0000 758c 0474 6f63  j....j.V..u..toc
 0004e290: 7394 7d94 286a 1203 0000 6a0a 0700 0029  s.}.(j....j....)
 0004e2a0: 8194 7d94 286a 7303 0000 682f 6a74 0300  ..}.(js...h/jt..
 0004e2b0: 005d 946a 0f07 0000 2981 947d 9428 6a73  .].j....)..}.(js
 0004e2c0: 0300 0068 2f6a 7403 0000 5d94 286a 6e03  ...h/jt...].(jn.
 0004e2d0: 0000 8c11 636f 6d70 6163 745f 7061 7261  ....compact_para
 0004e2e0: 6772 6170 6894 9394 2981 947d 9428 6a73  graph...)..}.(js
 0004e2f0: 0300 0068 2f6a 7403 0000 5d94 6a99 0d00  ...h/jt...].j...
@@ -20121,29 +20121,29 @@
 0004e980: 7d94 286a 8c03 0000 5d94 6a8e 0300 005d  }.(j....].j....]
 0004e990: 946a 9003 0000 5d94 6a92 0300 005d 946a  .j....].j....].j
 0004e9a0: 9403 0000 5d94 756a 9603 0000 6a0e 0700  ....].uj....j...
 0004e9b0: 006a 8703 0000 6aa6 5600 0075 6261 6a8a  .j....j.V..ubaj.
 0004e9c0: 0300 007d 9428 6a8c 0300 005d 946a 8e03  ...}.(j....].j..
 0004e9d0: 0000 5d94 6a90 0300 005d 946a 9203 0000  ..].j....].j....
 0004e9e0: 5d94 6a94 0300 005d 9475 6a96 0300 006a  ].j....].uj....j
-0004e9f0: 0907 0000 7562 6a1a 0300 006a 0a07 0000  ....ubj....j....
+0004e9f0: 0907 0000 7562 6a19 0300 006a 0a07 0000  ....ubj....j....
 0004ea00: 2981 947d 9428 6a73 0300 0068 2f6a 7403  )..}.(js...h/jt.
 0004ea10: 0000 5d94 6a0f 0700 0029 8194 7d94 286a  ..].j....)..}.(j
 0004ea20: 7303 0000 682f 6a74 0300 005d 9428 6aad  s...h/jt...].(j.
 0004ea30: 5600 0029 8194 7d94 286a 7303 0000 682f  V..)..}.(js...h/
 0004ea40: 6a74 0300 005d 946a 990d 0000 2981 947d  jt...].j....)..}
 0004ea50: 9428 6a73 0300 0068 2f6a 7403 0000 5d94  .(js...h/jt...].
 0004ea60: 6a82 0300 008c 1a49 6e63 6964 656e 7444  j......IncidentD
 0004ea70: 6174 6146 7261 6d65 4765 6e65 7261 746f  ataFrameGenerato
 0004ea80: 7294 8594 8194 7d94 6a87 0300 006a 5157  r.....}.j....jQW
 0004ea90: 0000 7362 616a 8a03 0000 7d94 286a 8c03  ..sbaj....}.(j..
 0004eaa0: 0000 5d94 6a8e 0300 005d 946a 9003 0000  ..].j....].j....
 0004eab0: 5d94 6a92 0300 005d 946a 9403 0000 5d94  ].j....].j....].
 0004eac0: 8c08 696e 7465 726e 616c 9488 8c06 7265  ..internal....re
-0004ead0: 6675 7269 946a 1a03 0000 8c0a 616e 6368  furi.j......anch
+0004ead0: 6675 7269 946a 1903 0000 8c0a 616e 6368  furi.j......anch
 0004eae0: 6f72 6e61 6d65 9468 2f75 6a96 0300 006a  orname.h/uj....j
 0004eaf0: 980d 0000 6a87 0300 006a 4e57 0000 7562  ....j....jNW..ub
 0004eb00: 616a 8a03 0000 7d94 286a 8c03 0000 5d94  aj....}.(j....].
 0004eb10: 6a8e 0300 005d 946a 9003 0000 5d94 6a92  j....].j....].j.
 0004eb20: 0300 005d 946a 9403 0000 5d94 756a 9603  ...].j....].uj..
 0004eb30: 0000 6aac 5600 006a 8703 0000 6a4b 5700  ..j.V..j....jKW.
 0004eb40: 0075 626a 0a07 0000 2981 947d 9428 6a73  .ubj....)..}.(js
@@ -20161,15 +20161,15 @@
 0004ec00: 0300 005d 946a 8e03 0000 5d94 6a90 0300  ...].j....].j...
 0004ec10: 005d 946a 9203 0000 5d94 6a94 0300 005d  .].j....].j....]
 0004ec20: 9475 6a96 0300 006a b206 0000 6a87 0300  .uj....j....j...
 0004ec30: 006a 7057 0000 7562 616a 8a03 0000 7d94  .jpW..ubaj....}.
 0004ec40: 286a 8c03 0000 5d94 6a8e 0300 005d 946a  (j....].j....].j
 0004ec50: 9003 0000 5d94 6a92 0300 005d 946a 9403  ....].j....].j..
 0004ec60: 0000 5d94 8c08 696e 7465 726e 616c 9488  ..]...internal..
-0004ec70: 8c06 7265 6675 7269 946a 1a03 0000 8c0a  ..refuri.j......
+0004ec70: 8c06 7265 6675 7269 946a 1903 0000 8c0a  ..refuri.j......
 0004ec80: 616e 6368 6f72 6e61 6d65 948c 3723 6575  anchorname..7#eu
 0004ec90: 7265 706f 632e 696e 6369 6465 6e74 5f64  repoc.incident_d
 0004eca0: 6174 6166 7261 6d65 732e 496e 6369 6465  ataframes.Incide
 0004ecb0: 6e74 4461 7461 4672 616d 6547 656e 6572  ntDataFrameGener
 0004ecc0: 6174 6f72 9475 6a96 0300 006a 980d 0000  ator.uj....j....
 0004ecd0: 6a87 0300 006a 6d57 0000 7562 616a 8a03  j....jmW..ubaj..
 0004ece0: 0000 7d94 286a 8c03 0000 5d94 6a8e 0300  ..}.(j....].j...
@@ -20194,15 +20194,15 @@
 0004ee10: 5d94 6a8e 0300 005d 946a 9003 0000 5d94  ].j....].j....].
 0004ee20: 6a92 0300 005d 946a 9403 0000 5d94 756a  j....].j....].uj
 0004ee30: 9603 0000 6ab2 0600 006a 8703 0000 6a9a  ....j....j....j.
 0004ee40: 5700 0075 6261 6a8a 0300 007d 9428 6a8c  W..ubaj....}.(j.
 0004ee50: 0300 005d 946a 8e03 0000 5d94 6a90 0300  ...].j....].j...
 0004ee60: 005d 946a 9203 0000 5d94 6a94 0300 005d  .].j....].j....]
 0004ee70: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
-0004ee80: 6566 7572 6994 6a1a 0300 008c 0a61 6e63  efuri.j......anc
+0004ee80: 6566 7572 6994 6a19 0300 008c 0a61 6e63  efuri.j......anc
 0004ee90: 686f 726e 616d 6594 8c4f 2365 7572 6570  horname..O#eurep
 0004eea0: 6f63 2e69 6e63 6964 656e 745f 6461 7461  oc.incident_data
 0004eeb0: 6672 616d 6573 2e49 6e63 6964 656e 7444  frames.IncidentD
 0004eec0: 6174 6146 7261 6d65 4765 6e65 7261 746f  ataFrameGenerato
 0004eed0: 722e 6765 745f 6174 7472 6962 7574 696f  r.get_attributio
 0004eee0: 6e5f 736f 7572 6365 7394 756a 9603 0000  n_sources.uj....
 0004eef0: 6a98 0d00 006a 8703 0000 6a97 5700 0075  j....j....j.W..u
@@ -20230,15 +20230,15 @@
 0004f050: 9428 6a8c 0300 005d 946a 8e03 0000 5d94  .(j....].j....].
 0004f060: 6a90 0300 005d 946a 9203 0000 5d94 6a94  j....].j....].j.
 0004f070: 0300 005d 9475 6a96 0300 006a b206 0000  ...].uj....j....
 0004f080: 6a87 0300 006a c757 0000 7562 616a 8a03  j....j.W..ubaj..
 0004f090: 0000 7d94 286a 8c03 0000 5d94 6a8e 0300  ..}.(j....].j...
 0004f0a0: 005d 946a 9003 0000 5d94 6a92 0300 005d  .].j....].j....]
 0004f0b0: 946a 9403 0000 5d94 8c08 696e 7465 726e  .j....]...intern
-0004f0c0: 616c 9488 8c06 7265 6675 7269 946a 1a03  al....refuri.j..
+0004f0c0: 616c 9488 8c06 7265 6675 7269 946a 1903  al....refuri.j..
 0004f0d0: 0000 8c0a 616e 6368 6f72 6e61 6d65 948c  ....anchorname..
 0004f0e0: 4823 6575 7265 706f 632e 696e 6369 6465  H#eurepoc.incide
 0004f0f0: 6e74 5f64 6174 6166 7261 6d65 732e 496e  nt_dataframes.In
 0004f100: 6369 6465 6e74 4461 7461 4672 616d 6547  cidentDataFrameG
 0004f110: 656e 6572 6174 6f72 2e67 6574 5f61 7474  enerator.get_att
 0004f120: 7269 6275 7469 6f6e 7394 756a 9603 0000  ributions.uj....
 0004f130: 6a98 0d00 006a 8703 0000 6ac4 5700 0075  j....j....j.W..u
@@ -20267,15 +20267,15 @@
 0004f2a0: 5d94 6a8e 0300 005d 946a 9003 0000 5d94  ].j....].j....].
 0004f2b0: 6a92 0300 005d 946a 9403 0000 5d94 756a  j....].j....].uj
 0004f2c0: 9603 0000 6ab2 0600 006a 8703 0000 6af4  ....j....j....j.
 0004f2d0: 5700 0075 6261 6a8a 0300 007d 9428 6a8c  W..ubaj....}.(j.
 0004f2e0: 0300 005d 946a 8e03 0000 5d94 6a90 0300  ...].j....].j...
 0004f2f0: 005d 946a 9203 0000 5d94 6a94 0300 005d  .].j....].j....]
 0004f300: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
-0004f310: 6566 7572 6994 6a1a 0300 008c 0a61 6e63  efuri.j......anc
+0004f310: 6566 7572 6994 6a19 0300 008c 0a61 6e63  efuri.j......anc
 0004f320: 686f 726e 616d 6594 8c51 2365 7572 6570  horname..Q#eurep
 0004f330: 6f63 2e69 6e63 6964 656e 745f 6461 7461  oc.incident_data
 0004f340: 6672 616d 6573 2e49 6e63 6964 656e 7444  frames.IncidentD
 0004f350: 6174 6146 7261 6d65 4765 6e65 7261 746f  ataFrameGenerato
 0004f360: 722e 6765 745f 6379 6265 725f 636f 6e66  r.get_cyber_conf
 0004f370: 6c69 6374 5f69 7373 7565 7394 756a 9603  lict_issues.uj..
 0004f380: 0000 6a98 0d00 006a 8703 0000 6af1 5700  ..j....j....j.W.
@@ -20304,15 +20304,15 @@
 0004f4f0: 286a 8c03 0000 5d94 6a8e 0300 005d 946a  (j....].j....].j
 0004f500: 9003 0000 5d94 6a92 0300 005d 946a 9403  ....].j....].j..
 0004f510: 0000 5d94 756a 9603 0000 6ab2 0600 006a  ..].uj....j....j
 0004f520: 8703 0000 6a21 5800 0075 6261 6a8a 0300  ....j!X..ubaj...
 0004f530: 007d 9428 6a8c 0300 005d 946a 8e03 0000  .}.(j....].j....
 0004f540: 5d94 6a90 0300 005d 946a 9203 0000 5d94  ].j....].j....].
 0004f550: 6a94 0300 005d 948c 0869 6e74 6572 6e61  j....]...interna
-0004f560: 6c94 888c 0672 6566 7572 6994 6a1a 0300  l....refuri.j...
+0004f560: 6c94 888c 0672 6566 7572 6994 6a19 0300  l....refuri.j...
 0004f570: 008c 0a61 6e63 686f 726e 616d 6594 8c55  ...anchorname..U
 0004f580: 2365 7572 6570 6f63 2e69 6e63 6964 656e  #eurepoc.inciden
 0004f590: 745f 6461 7461 6672 616d 6573 2e49 6e63  t_dataframes.Inc
 0004f5a0: 6964 656e 7444 6174 6146 7261 6d65 4765  identDataFrameGe
 0004f5b0: 6e65 7261 746f 722e 6765 745f 6379 6265  nerator.get_cybe
 0004f5c0: 725f 696e 7465 6e73 6974 795f 7661 7269  r_intensity_vari
 0004f5d0: 6162 6c65 7394 756a 9603 0000 6a98 0d00  ables.uj....j...
@@ -20342,15 +20342,15 @@
 0004f750: 005d 946a 9003 0000 5d94 6a92 0300 005d  .].j....].j....]
 0004f760: 946a 9403 0000 5d94 756a 9603 0000 6ab2  .j....].uj....j.
 0004f770: 0600 006a 8703 0000 6a4e 5800 0075 6261  ...j....jNX..uba
 0004f780: 6a8a 0300 007d 9428 6a8c 0300 005d 946a  j....}.(j....].j
 0004f790: 8e03 0000 5d94 6a90 0300 005d 946a 9203  ....].j....].j..
 0004f7a0: 0000 5d94 6a94 0300 005d 948c 0869 6e74  ..].j....]...int
 0004f7b0: 6572 6e61 6c94 888c 0672 6566 7572 6994  ernal....refuri.
-0004f7c0: 6a1a 0300 008c 0a61 6e63 686f 726e 616d  j......anchornam
+0004f7c0: 6a19 0300 008c 0a61 6e63 686f 726e 616d  j......anchornam
 0004f7d0: 6594 8c4f 2365 7572 6570 6f63 2e69 6e63  e..O#eurepoc.inc
 0004f7e0: 6964 656e 745f 6461 7461 6672 616d 6573  ident_dataframes
 0004f7f0: 2e49 6e63 6964 656e 7444 6174 6146 7261  .IncidentDataFra
 0004f800: 6d65 4765 6e65 7261 746f 722e 6765 745f  meGenerator.get_
 0004f810: 696c 5f62 7265 6163 685f 696e 6469 6361  il_breach_indica
 0004f820: 746f 7294 756a 9603 0000 6a98 0d00 006a  tor.uj....j....j
 0004f830: 8703 0000 6a4b 5800 0075 6261 6a8a 0300  ....jKX..ubaj...
@@ -20379,15 +20379,15 @@
 0004f9a0: 946a 8e03 0000 5d94 6a90 0300 005d 946a  .j....].j....].j
 0004f9b0: 9203 0000 5d94 6a94 0300 005d 9475 6a96  ....].j....].uj.
 0004f9c0: 0300 006a b206 0000 6a87 0300 006a 7b58  ...j....j....j{X
 0004f9d0: 0000 7562 616a 8a03 0000 7d94 286a 8c03  ..ubaj....}.(j..
 0004f9e0: 0000 5d94 6a8e 0300 005d 946a 9003 0000  ..].j....].j....
 0004f9f0: 5d94 6a92 0300 005d 946a 9403 0000 5d94  ].j....].j....].
 0004fa00: 8c08 696e 7465 726e 616c 9488 8c06 7265  ..internal....re
-0004fa10: 6675 7269 946a 1a03 0000 8c0a 616e 6368  furi.j......anch
+0004fa10: 6675 7269 946a 1903 0000 8c0a 616e 6368  furi.j......anch
 0004fa20: 6f72 6e61 6d65 948c 5623 6575 7265 706f  orname..V#eurepo
 0004fa30: 632e 696e 6369 6465 6e74 5f64 6174 6166  c.incident_dataf
 0004fa40: 7261 6d65 732e 496e 6369 6465 6e74 4461  rames.IncidentDa
 0004fa50: 7461 4672 616d 6547 656e 6572 6174 6f72  taFrameGenerator
 0004fa60: 2e67 6574 5f69 6d70 6163 745f 696e 6469  .get_impact_indi
 0004fa70: 6361 746f 725f 7661 7269 6162 6c65 7394  cator_variables.
 0004fa80: 756a 9603 0000 6a98 0d00 006a 8703 0000  uj....j....j....
@@ -20416,15 +20416,15 @@
 0004fbf0: 946a 8e03 0000 5d94 6a90 0300 005d 946a  .j....].j....].j
 0004fc00: 9203 0000 5d94 6a94 0300 005d 9475 6a96  ....].j....].uj.
 0004fc10: 0300 006a b206 0000 6a87 0300 006a a858  ...j....j....j.X
 0004fc20: 0000 7562 616a 8a03 0000 7d94 286a 8c03  ..ubaj....}.(j..
 0004fc30: 0000 5d94 6a8e 0300 005d 946a 9003 0000  ..].j....].j....
 0004fc40: 5d94 6a92 0300 005d 946a 9403 0000 5d94  ].j....].j....].
 0004fc50: 8c08 696e 7465 726e 616c 9488 8c06 7265  ..internal....re
-0004fc60: 6675 7269 946a 1a03 0000 8c0a 616e 6368  furi.j......anch
+0004fc60: 6675 7269 946a 1903 0000 8c0a 616e 6368  furi.j......anch
 0004fc70: 6f72 6e61 6d65 948c 4a23 6575 7265 706f  orname..J#eurepo
 0004fc80: 632e 696e 6369 6465 6e74 5f64 6174 6166  c.incident_dataf
 0004fc90: 7261 6d65 732e 496e 6369 6465 6e74 4461  rames.IncidentDa
 0004fca0: 7461 4672 616d 6547 656e 6572 6174 6f72  taFrameGenerator
 0004fcb0: 2e67 6574 5f69 6e63 6964 656e 745f 7479  .get_incident_ty
 0004fcc0: 7065 7394 756a 9603 0000 6a98 0d00 006a  pes.uj....j....j
 0004fcd0: 8703 0000 6aa5 5800 0075 6261 6a8a 0300  ....j.X..ubaj...
@@ -20452,15 +20452,15 @@
 0004fe30: 9428 6a8c 0300 005d 946a 8e03 0000 5d94  .(j....].j....].
 0004fe40: 6a90 0300 005d 946a 9203 0000 5d94 6a94  j....].j....].j.
 0004fe50: 0300 005d 9475 6a96 0300 006a b206 0000  ...].uj....j....
 0004fe60: 6a87 0300 006a d558 0000 7562 616a 8a03  j....j.X..ubaj..
 0004fe70: 0000 7d94 286a 8c03 0000 5d94 6a8e 0300  ..}.(j....].j...
 0004fe80: 005d 946a 9003 0000 5d94 6a92 0300 005d  .].j....].j....]
 0004fe90: 946a 9403 0000 5d94 8c08 696e 7465 726e  .j....]...intern
-0004fea0: 616c 9488 8c06 7265 6675 7269 946a 1a03  al....refuri.j..
+0004fea0: 616c 9488 8c06 7265 6675 7269 946a 1903  al....refuri.j..
 0004feb0: 0000 8c0a 616e 6368 6f72 6e61 6d65 948c  ....anchorname..
 0004fec0: 4e23 6575 7265 706f 632e 696e 6369 6465  N#eurepoc.incide
 0004fed0: 6e74 5f64 6174 6166 7261 6d65 732e 496e  nt_dataframes.In
 0004fee0: 6369 6465 6e74 4461 7461 4672 616d 6547  cidentDataFrameG
 0004fef0: 656e 6572 6174 6f72 2e67 6574 5f69 6e63  enerator.get_inc
 0004ff00: 6c75 7369 6f6e 5f63 7269 7465 7269 6194  lusion_criteria.
 0004ff10: 756a 9603 0000 6a98 0d00 006a 8703 0000  uj....j....j....
@@ -20489,15 +20489,15 @@
 00050080: 8c03 0000 5d94 6a8e 0300 005d 946a 9003  ....].j....].j..
 00050090: 0000 5d94 6a92 0300 005d 946a 9403 0000  ..].j....].j....
 000500a0: 5d94 756a 9603 0000 6ab2 0600 006a 8703  ].uj....j....j..
 000500b0: 0000 6a02 5900 0075 6261 6a8a 0300 007d  ..j.Y..ubaj....}
 000500c0: 9428 6a8c 0300 005d 946a 8e03 0000 5d94  .(j....].j....].
 000500d0: 6a90 0300 005d 946a 9203 0000 5d94 6a94  j....].j....].j.
 000500e0: 0300 005d 948c 0869 6e74 6572 6e61 6c94  ...]...internal.
-000500f0: 888c 0672 6566 7572 6994 6a1a 0300 008c  ...refuri.j.....
+000500f0: 888c 0672 6566 7572 6994 6a19 0300 008c  ...refuri.j.....
 00050100: 0a61 6e63 686f 726e 616d 6594 8c46 2365  .anchorname..F#e
 00050110: 7572 6570 6f63 2e69 6e63 6964 656e 745f  urepoc.incident_
 00050120: 6461 7461 6672 616d 6573 2e49 6e63 6964  dataframes.Incid
 00050130: 656e 7444 6174 6146 7261 6d65 4765 6e65  entDataFrameGene
 00050140: 7261 746f 722e 6765 745f 696e 6974 6961  rator.get_initia
 00050150: 746f 7273 9475 6a96 0300 006a 980d 0000  tors.uj....j....
 00050160: 6a87 0300 006a ff58 0000 7562 616a 8a03  j....j.X..ubaj..
@@ -20525,15 +20525,15 @@
 000502c0: 6a8c 0300 005d 946a 8e03 0000 5d94 6a90  j....].j....].j.
 000502d0: 0300 005d 946a 9203 0000 5d94 6a94 0300  ...].j....].j...
 000502e0: 005d 9475 6a96 0300 006a b206 0000 6a87  .].uj....j....j.
 000502f0: 0300 006a 2f59 0000 7562 616a 8a03 0000  ...j/Y..ubaj....
 00050300: 7d94 286a 8c03 0000 5d94 6a8e 0300 005d  }.(j....].j....]
 00050310: 946a 9003 0000 5d94 6a92 0300 005d 946a  .j....].j....].j
 00050320: 9403 0000 5d94 8c08 696e 7465 726e 616c  ....]...internal
-00050330: 9488 8c06 7265 6675 7269 946a 1a03 0000  ....refuri.j....
+00050330: 9488 8c06 7265 6675 7269 946a 1903 0000  ....refuri.j....
 00050340: 8c0a 616e 6368 6f72 6e61 6d65 948c 4b23  ..anchorname..K#
 00050350: 6575 7265 706f 632e 696e 6369 6465 6e74  eurepoc.incident
 00050360: 5f64 6174 6166 7261 6d65 732e 496e 6369  _dataframes.Inci
 00050370: 6465 6e74 4461 7461 4672 616d 6547 656e  dentDataFrameGen
 00050380: 6572 6174 6f72 2e67 6574 5f6c 6567 616c  erator.get_legal
 00050390: 5f72 6573 706f 6e73 6573 9475 6a96 0300  _responses.uj...
 000503a0: 006a 980d 0000 6a87 0300 006a 2c59 0000  .j....j....j,Y..
@@ -20562,15 +20562,15 @@
 00050510: 0000 5d94 6a90 0300 005d 946a 9203 0000  ..].j....].j....
 00050520: 5d94 6a94 0300 005d 9475 6a96 0300 006a  ].j....].uj....j
 00050530: b206 0000 6a87 0300 006a 5c59 0000 7562  ....j....j\Y..ub
 00050540: 616a 8a03 0000 7d94 286a 8c03 0000 5d94  aj....}.(j....].
 00050550: 6a8e 0300 005d 946a 9003 0000 5d94 6a92  j....].j....].j.
 00050560: 0300 005d 946a 9403 0000 5d94 8c08 696e  ...].j....]...in
 00050570: 7465 726e 616c 9488 8c06 7265 6675 7269  ternal....refuri
-00050580: 946a 1a03 0000 8c0a 616e 6368 6f72 6e61  .j......anchorna
+00050580: 946a 1903 0000 8c0a 616e 6368 6f72 6e61  .j......anchorna
 00050590: 6d65 948c 4b23 6575 7265 706f 632e 696e  me..K#eurepoc.in
 000505a0: 6369 6465 6e74 5f64 6174 6166 7261 6d65  cident_dataframe
 000505b0: 732e 496e 6369 6465 6e74 4461 7461 4672  s.IncidentDataFr
 000505c0: 616d 6547 656e 6572 6174 6f72 2e67 6574  ameGenerator.get
 000505d0: 5f6c 6567 616c 5f76 6172 6961 626c 6573  _legal_variables
 000505e0: 9475 6a96 0300 006a 980d 0000 6a87 0300  .uj....j....j...
 000505f0: 006a 5959 0000 7562 616a 8a03 0000 7d94  .jYY..ubaj....}.
@@ -20598,15 +20598,15 @@
 00050750: 0000 5d94 6a90 0300 005d 946a 9203 0000  ..].j....].j....
 00050760: 5d94 6a94 0300 005d 9475 6a96 0300 006a  ].j....].uj....j
 00050770: b206 0000 6a87 0300 006a 8959 0000 7562  ....j....j.Y..ub
 00050780: 616a 8a03 0000 7d94 286a 8c03 0000 5d94  aj....}.(j....].
 00050790: 6a8e 0300 005d 946a 9003 0000 5d94 6a92  j....].j....].j.
 000507a0: 0300 005d 946a 9403 0000 5d94 8c08 696e  ...].j....]...in
 000507b0: 7465 726e 616c 9488 8c06 7265 6675 7269  ternal....refuri
-000507c0: 946a 1a03 0000 8c0a 616e 6368 6f72 6e61  .j......anchorna
+000507c0: 946a 1903 0000 8c0a 616e 6368 6f72 6e61  .j......anchorna
 000507d0: 6d65 948c 4523 6575 7265 706f 632e 696e  me..E#eurepoc.in
 000507e0: 6369 6465 6e74 5f64 6174 6166 7261 6d65  cident_dataframe
 000507f0: 732e 496e 6369 6465 6e74 4461 7461 4672  s.IncidentDataFr
 00050800: 616d 6547 656e 6572 6174 6f72 2e67 6574  ameGenerator.get
 00050810: 5f6d 6169 6e5f 6461 7461 9475 6a96 0300  _main_data.uj...
 00050820: 006a 980d 0000 6a87 0300 006a 8659 0000  .j....j....j.Y..
 00050830: 7562 616a 8a03 0000 7d94 286a 8c03 0000  ubaj....}.(j....
@@ -20633,15 +20633,15 @@
 00050980: 7d94 286a 8c03 0000 5d94 6a8e 0300 005d  }.(j....].j....]
 00050990: 946a 9003 0000 5d94 6a92 0300 005d 946a  .j....].j....].j
 000509a0: 9403 0000 5d94 756a 9603 0000 6ab2 0600  ....].uj....j...
 000509b0: 006a 8703 0000 6ab6 5900 0075 6261 6a8a  .j....j.Y..ubaj.
 000509c0: 0300 007d 9428 6a8c 0300 005d 946a 8e03  ...}.(j....].j..
 000509d0: 0000 5d94 6a90 0300 005d 946a 9203 0000  ..].j....].j....
 000509e0: 5d94 6a94 0300 005d 948c 0869 6e74 6572  ].j....]...inter
-000509f0: 6e61 6c94 888c 0672 6566 7572 6994 6a1a  nal....refuri.j.
+000509f0: 6e61 6c94 888c 0672 6566 7572 6994 6a19  nal....refuri.j.
 00050a00: 0300 008c 0a61 6e63 686f 726e 616d 6594  .....anchorname.
 00050a10: 8c48 2365 7572 6570 6f63 2e69 6e63 6964  .H#eurepoc.incid
 00050a20: 656e 745f 6461 7461 6672 616d 6573 2e49  ent_dataframes.I
 00050a30: 6e63 6964 656e 7444 6174 6146 7261 6d65  ncidentDataFrame
 00050a40: 4765 6e65 7261 746f 722e 6765 745f 6d69  Generator.get_mi
 00050a50: 7472 655f 696d 7061 6374 9475 6a96 0300  tre_impact.uj...
 00050a60: 006a 980d 0000 6a87 0300 006a b359 0000  .j....j....j.Y..
@@ -20670,15 +20670,15 @@
 00050bd0: 5d94 6a8e 0300 005d 946a 9003 0000 5d94  ].j....].j....].
 00050be0: 6a92 0300 005d 946a 9403 0000 5d94 756a  j....].j....].uj
 00050bf0: 9603 0000 6ab2 0600 006a 8703 0000 6ae3  ....j....j....j.
 00050c00: 5900 0075 6261 6a8a 0300 007d 9428 6a8c  Y..ubaj....}.(j.
 00050c10: 0300 005d 946a 8e03 0000 5d94 6a90 0300  ...].j....].j...
 00050c20: 005d 946a 9203 0000 5d94 6a94 0300 005d  .].j....].j....]
 00050c30: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
-00050c40: 6566 7572 6994 6a1a 0300 008c 0a61 6e63  efuri.j......anc
+00050c40: 6566 7572 6994 6a19 0300 008c 0a61 6e63  efuri.j......anc
 00050c50: 686f 726e 616d 6594 8c50 2365 7572 6570  horname..P#eurep
 00050c60: 6f63 2e69 6e63 6964 656e 745f 6461 7461  oc.incident_data
 00050c70: 6672 616d 6573 2e49 6e63 6964 656e 7444  frames.IncidentD
 00050c80: 6174 6146 7261 6d65 4765 6e65 7261 746f  ataFrameGenerato
 00050c90: 722e 6765 745f 6d69 7472 655f 696e 6974  r.get_mitre_init
 00050ca0: 6961 6c5f 6163 6365 7373 9475 6a96 0300  ial_access.uj...
 00050cb0: 006a 980d 0000 6a87 0300 006a e059 0000  .j....j....j.Y..
@@ -20707,15 +20707,15 @@
 00050e20: 8e03 0000 5d94 6a90 0300 005d 946a 9203  ....].j....].j..
 00050e30: 0000 5d94 6a94 0300 005d 9475 6a96 0300  ..].j....].uj...
 00050e40: 006a b206 0000 6a87 0300 006a 105a 0000  .j....j....j.Z..
 00050e50: 7562 616a 8a03 0000 7d94 286a 8c03 0000  ubaj....}.(j....
 00050e60: 5d94 6a8e 0300 005d 946a 9003 0000 5d94  ].j....].j....].
 00050e70: 6a92 0300 005d 946a 9403 0000 5d94 8c08  j....].j....]...
 00050e80: 696e 7465 726e 616c 9488 8c06 7265 6675  internal....refu
-00050e90: 7269 946a 1a03 0000 8c0a 616e 6368 6f72  ri.j......anchor
+00050e90: 7269 946a 1903 0000 8c0a 616e 6368 6f72  ri.j......anchor
 00050ea0: 6e61 6d65 948c 4d23 6575 7265 706f 632e  name..M#eurepoc.
 00050eb0: 696e 6369 6465 6e74 5f64 6174 6166 7261  incident_datafra
 00050ec0: 6d65 732e 496e 6369 6465 6e74 4461 7461  mes.IncidentData
 00050ed0: 4672 616d 6547 656e 6572 6174 6f72 2e67  FrameGenerator.g
 00050ee0: 6574 5f6f 6666 6c69 6e65 5f63 6f6e 666c  et_offline_confl
 00050ef0: 6963 7473 9475 6a96 0300 006a 980d 0000  icts.uj....j....
 00050f00: 6a87 0300 006a 0d5a 0000 7562 616a 8a03  j....j.Z..ubaj..
@@ -20743,15 +20743,15 @@
 00051060: 6a8c 0300 005d 946a 8e03 0000 5d94 6a90  j....].j....].j.
 00051070: 0300 005d 946a 9203 0000 5d94 6a94 0300  ...].j....].j...
 00051080: 005d 9475 6a96 0300 006a b206 0000 6a87  .].uj....j....j.
 00051090: 0300 006a 3d5a 0000 7562 616a 8a03 0000  ...j=Z..ubaj....
 000510a0: 7d94 286a 8c03 0000 5d94 6a8e 0300 005d  }.(j....].j....]
 000510b0: 946a 9003 0000 5d94 6a92 0300 005d 946a  .j....].j....].j
 000510c0: 9403 0000 5d94 8c08 696e 7465 726e 616c  ....]...internal
-000510d0: 9488 8c06 7265 6675 7269 946a 1a03 0000  ....refuri.j....
+000510d0: 9488 8c06 7265 6675 7269 946a 1903 0000  ....refuri.j....
 000510e0: 8c0a 616e 6368 6f72 6e61 6d65 948c 4b23  ..anchorname..K#
 000510f0: 6575 7265 706f 632e 696e 6369 6465 6e74  eurepoc.incident
 00051100: 5f64 6174 6166 7261 6d65 732e 496e 6369  _dataframes.Inci
 00051110: 6465 6e74 4461 7461 4672 616d 6547 656e  dentDataFrameGen
 00051120: 6572 6174 6f72 2e67 6574 5f6f 7065 7261  erator.get_opera
 00051130: 7469 6f6e 5f74 7970 6573 9475 6a96 0300  tion_types.uj...
 00051140: 006a 980d 0000 6a87 0300 006a 3a5a 0000  .j....j....j:Z..
@@ -20780,15 +20780,15 @@
 000512b0: 946a 8e03 0000 5d94 6a90 0300 005d 946a  .j....].j....].j
 000512c0: 9203 0000 5d94 6a94 0300 005d 9475 6a96  ....].j....].uj.
 000512d0: 0300 006a b206 0000 6a87 0300 006a 6a5a  ...j....j....jjZ
 000512e0: 0000 7562 616a 8a03 0000 7d94 286a 8c03  ..ubaj....}.(j..
 000512f0: 0000 5d94 6a8e 0300 005d 946a 9003 0000  ..].j....].j....
 00051300: 5d94 6a92 0300 005d 946a 9403 0000 5d94  ].j....].j....].
 00051310: 8c08 696e 7465 726e 616c 9488 8c06 7265  ..internal....re
-00051320: 6675 7269 946a 1a03 0000 8c0a 616e 6368  furi.j......anch
+00051320: 6675 7269 946a 1903 0000 8c0a 616e 6368  furi.j......anch
 00051330: 6f72 6e61 6d65 948c 4f23 6575 7265 706f  orname..O#eurepo
 00051340: 632e 696e 6369 6465 6e74 5f64 6174 6166  c.incident_dataf
 00051350: 7261 6d65 732e 496e 6369 6465 6e74 4461  rames.IncidentDa
 00051360: 7461 4672 616d 6547 656e 6572 6174 6f72  taFrameGenerator
 00051370: 2e67 6574 5f70 6f6c 6974 6963 616c 5f72  .get_political_r
 00051380: 6573 706f 6e73 6573 9475 6a96 0300 006a  esponses.uj....j
 00051390: 980d 0000 6a87 0300 006a 675a 0000 7562  ....j....jgZ..ub
@@ -20816,15 +20816,15 @@
 000514f0: 0300 005d 946a 8e03 0000 5d94 6a90 0300  ...].j....].j...
 00051500: 005d 946a 9203 0000 5d94 6a94 0300 005d  .].j....].j....]
 00051510: 9475 6a96 0300 006a b206 0000 6a87 0300  .uj....j....j...
 00051520: 006a 975a 0000 7562 616a 8a03 0000 7d94  .j.Z..ubaj....}.
 00051530: 286a 8c03 0000 5d94 6a8e 0300 005d 946a  (j....].j....].j
 00051540: 9003 0000 5d94 6a92 0300 005d 946a 9403  ....].j....].j..
 00051550: 0000 5d94 8c08 696e 7465 726e 616c 9488  ..]...internal..
-00051560: 8c06 7265 6675 7269 946a 1a03 0000 8c0a  ..refuri.j......
+00051560: 8c06 7265 6675 7269 946a 1903 0000 8c0a  ..refuri.j......
 00051570: 616e 6368 6f72 6e61 6d65 948c 4523 6575  anchorname..E#eu
 00051580: 7265 706f 632e 696e 6369 6465 6e74 5f64  repoc.incident_d
 00051590: 6174 6166 7261 6d65 732e 496e 6369 6465  ataframes.Incide
 000515a0: 6e74 4461 7461 4672 616d 6547 656e 6572  ntDataFrameGener
 000515b0: 6174 6f72 2e67 6574 5f72 6563 6569 7665  ator.get_receive
 000515c0: 7273 9475 6a96 0300 006a 980d 0000 6a87  rs.uj....j....j.
 000515d0: 0300 006a 945a 0000 7562 616a 8a03 0000  ...j.Z..ubaj....
@@ -20852,15 +20852,15 @@
 00051730: 5d94 6a8e 0300 005d 946a 9003 0000 5d94  ].j....].j....].
 00051740: 6a92 0300 005d 946a 9403 0000 5d94 756a  j....].j....].uj
 00051750: 9603 0000 6ab2 0600 006a 8703 0000 6ac4  ....j....j....j.
 00051760: 5a00 0075 6261 6a8a 0300 007d 9428 6a8c  Z..ubaj....}.(j.
 00051770: 0300 005d 946a 8e03 0000 5d94 6a90 0300  ...].j....].j...
 00051780: 005d 946a 9203 0000 5d94 6a94 0300 005d  .].j....].j....]
 00051790: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
-000517a0: 6566 7572 6994 6a1a 0300 008c 0a61 6e63  efuri.j......anc
+000517a0: 6566 7572 6994 6a19 0300 008c 0a61 6e63  efuri.j......anc
 000517b0: 686f 726e 616d 6594 8c48 2365 7572 6570  horname..H#eurep
 000517c0: 6f63 2e69 6e63 6964 656e 745f 6461 7461  oc.incident_data
 000517d0: 6672 616d 6573 2e49 6e63 6964 656e 7444  frames.IncidentD
 000517e0: 6174 6146 7261 6d65 4765 6e65 7261 746f  ataFrameGenerato
 000517f0: 722e 6765 745f 736f 7572 6365 5f6e 616d  r.get_source_nam
 00051800: 6573 9475 6a96 0300 006a 980d 0000 6a87  es.uj....j....j.
 00051810: 0300 006a c15a 0000 7562 616a 8a03 0000  ...j.Z..ubaj....
@@ -20889,15 +20889,15 @@
 00051980: 5d94 6a90 0300 005d 946a 9203 0000 5d94  ].j....].j....].
 00051990: 6a94 0300 005d 9475 6a96 0300 006a b206  j....].uj....j..
 000519a0: 0000 6a87 0300 006a f15a 0000 7562 616a  ..j....j.Z..ubaj
 000519b0: 8a03 0000 7d94 286a 8c03 0000 5d94 6a8e  ....}.(j....].j.
 000519c0: 0300 005d 946a 9003 0000 5d94 6a92 0300  ...].j....].j...
 000519d0: 005d 946a 9403 0000 5d94 8c08 696e 7465  .].j....]...inte
 000519e0: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
-000519f0: 1a03 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
+000519f0: 1903 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
 00051a00: 948c 5123 6575 7265 706f 632e 696e 6369  ..Q#eurepoc.inci
 00051a10: 6465 6e74 5f64 6174 6166 7261 6d65 732e  dent_dataframes.
 00051a20: 496e 6369 6465 6e74 4461 7461 4672 616d  IncidentDataFram
 00051a30: 6547 656e 6572 6174 6f72 2e67 6574 5f73  eGenerator.get_s
 00051a40: 6f75 7263 6573 5f6f 665f 6469 7363 6c6f  ources_of_disclo
 00051a50: 7375 7265 9475 6a96 0300 006a 980d 0000  sure.uj....j....
 00051a60: 6a87 0300 006a ee5a 0000 7562 616a 8a03  j....j.Z..ubaj..
@@ -20925,15 +20925,15 @@
 00051bc0: 0000 5d94 6a8e 0300 005d 946a 9003 0000  ..].j....].j....
 00051bd0: 5d94 6a92 0300 005d 946a 9403 0000 5d94  ].j....].j....].
 00051be0: 756a 9603 0000 6ab2 0600 006a 8703 0000  uj....j....j....
 00051bf0: 6a1e 5b00 0075 6261 6a8a 0300 007d 9428  j.[..ubaj....}.(
 00051c00: 6a8c 0300 005d 946a 8e03 0000 5d94 6a90  j....].j....].j.
 00051c10: 0300 005d 946a 9203 0000 5d94 6a94 0300  ...].j....].j...
 00051c20: 005d 948c 0869 6e74 6572 6e61 6c94 888c  .]...internal...
-00051c30: 0672 6566 7572 6994 6a1a 0300 008c 0a61  .refuri.j......a
+00051c30: 0672 6566 7572 6994 6a19 0300 008c 0a61  .refuri.j......a
 00051c40: 6e63 686f 726e 616d 6594 8c48 2365 7572  nchorname..H#eur
 00051c50: 6570 6f63 2e69 6e63 6964 656e 745f 6461  epoc.incident_da
 00051c60: 7461 6672 616d 6573 2e49 6e63 6964 656e  taframes.Inciden
 00051c70: 7444 6174 6146 7261 6d65 4765 6e65 7261  tDataFrameGenera
 00051c80: 746f 722e 6765 745f 736f 7572 6365 735f  tor.get_sources_
 00051c90: 7572 6c73 9475 6a96 0300 006a 980d 0000  urls.uj....j....
 00051ca0: 6a87 0300 006a 1b5b 0000 7562 616a 8a03  j....j.[..ubaj..
@@ -20962,15 +20962,15 @@
 00051e10: 5d94 6a90 0300 005d 946a 9203 0000 5d94  ].j....].j....].
 00051e20: 6a94 0300 005d 9475 6a96 0300 006a b206  j....].uj....j..
 00051e30: 0000 6a87 0300 006a 4b5b 0000 7562 616a  ..j....jK[..ubaj
 00051e40: 8a03 0000 7d94 286a 8c03 0000 5d94 6a8e  ....}.(j....].j.
 00051e50: 0300 005d 946a 9003 0000 5d94 6a92 0300  ...].j....].j...
 00051e60: 005d 946a 9403 0000 5d94 8c08 696e 7465  .].j....]...inte
 00051e70: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
-00051e80: 1a03 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
+00051e80: 1903 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
 00051e90: 948c 4f23 6575 7265 706f 632e 696e 6369  ..O#eurepoc.inci
 00051ea0: 6465 6e74 5f64 6174 6166 7261 6d65 732e  dent_dataframes.
 00051eb0: 496e 6369 6465 6e74 4461 7461 4672 616d  IncidentDataFram
 00051ec0: 6547 656e 6572 6174 6f72 2e67 6574 5f74  eGenerator.get_t
 00051ed0: 6563 686e 6963 616c 5f76 6172 6961 626c  echnical_variabl
 00051ee0: 6573 9475 6a96 0300 006a 980d 0000 6a87  es.uj....j....j.
 00051ef0: 0300 006a 485b 0000 7562 616a 8a03 0000  ...jH[..ubaj....
@@ -20999,84 +20999,84 @@
 00052060: 656a 8a03 0000 7d94 286a 8c03 0000 5d94  ej....}.(j....].
 00052070: 6a8e 0300 005d 946a 9003 0000 5d94 6a92  j....].j....].j.
 00052080: 0300 005d 946a 9403 0000 5d94 756a 9603  ...].j....].uj..
 00052090: 0000 6a0e 0700 006a 8703 0000 6a48 5700  ..j....j....jHW.
 000520a0: 0075 6261 6a8a 0300 007d 9428 6a8c 0300  .ubaj....}.(j...
 000520b0: 005d 946a 8e03 0000 5d94 6a90 0300 005d  .].j....].j....]
 000520c0: 946a 9203 0000 5d94 6a94 0300 005d 9475  .j....].j....].u
-000520d0: 6a96 0300 006a 0907 0000 7562 6a18 0300  j....j....ubj...
+000520d0: 6a96 0300 006a 0907 0000 7562 6a14 0300  j....j....ubj...
 000520e0: 006a 0a07 0000 2981 947d 9428 6a73 0300  .j....)..}.(js..
 000520f0: 0068 2f6a 7403 0000 5d94 6a0f 0700 0029  .h/jt...].j....)
 00052100: 8194 7d94 286a 7303 0000 682f 6a74 0300  ..}.(js...h/jt..
 00052110: 005d 946a ad56 0000 2981 947d 9428 6a73  .].j.V..)..}.(js
 00052120: 0300 0068 2f6a 7403 0000 5d94 6a99 0d00  ...h/jt...].j...
 00052130: 0029 8194 7d94 286a 7303 0000 682f 6a74  .)..}.(js...h/jt
 00052140: 0300 005d 946a 8203 0000 8c09 6461 7465  ...].j......date
 00052150: 5f74 7970 6594 8594 8194 7d94 6a87 0300  _type.....}.j...
 00052160: 006a 995b 0000 7362 616a 8a03 0000 7d94  .j.[..sbaj....}.
 00052170: 286a 8c03 0000 5d94 6a8e 0300 005d 946a  (j....].j....].j
 00052180: 9003 0000 5d94 6a92 0300 005d 946a 9403  ....].j....].j..
 00052190: 0000 5d94 8c08 696e 7465 726e 616c 9488  ..]...internal..
-000521a0: 8c06 7265 6675 7269 946a 1803 0000 8c0a  ..refuri.j......
+000521a0: 8c06 7265 6675 7269 946a 1403 0000 8c0a  ..refuri.j......
 000521b0: 616e 6368 6f72 6e61 6d65 9468 2f75 6a96  anchorname.h/uj.
 000521c0: 0300 006a 980d 0000 6a87 0300 006a 965b  ...j....j....j.[
 000521d0: 0000 7562 616a 8a03 0000 7d94 286a 8c03  ..ubaj....}.(j..
 000521e0: 0000 5d94 6a8e 0300 005d 946a 9003 0000  ..].j....].j....
 000521f0: 5d94 6a92 0300 005d 946a 9403 0000 5d94  ].j....].j....].
 00052200: 756a 9603 0000 6aac 5600 006a 8703 0000  uj....j.V..j....
 00052210: 6a93 5b00 0075 6261 6a8a 0300 007d 9428  j.[..ubaj....}.(
 00052220: 6a8c 0300 005d 946a 8e03 0000 5d94 6a90  j....].j....].j.
 00052230: 0300 005d 946a 9203 0000 5d94 6a94 0300  ...].j....].j...
 00052240: 005d 9475 6a96 0300 006a 0e07 0000 6a87  .].uj....j....j.
 00052250: 0300 006a 905b 0000 7562 616a 8a03 0000  ...j.[..ubaj....
 00052260: 7d94 286a 8c03 0000 5d94 6a8e 0300 005d  }.(j....].j....]
 00052270: 946a 9003 0000 5d94 6a92 0300 005d 946a  .j....].j....].j
 00052280: 9403 0000 5d94 756a 9603 0000 6a09 0700  ....].uj....j...
-00052290: 0075 626a 1403 0000 6a0a 0700 0029 8194  .ubj....j....)..
+00052290: 0075 626a 1803 0000 6a0a 0700 0029 8194  .ubj....j....)..
 000522a0: 7d94 286a 7303 0000 682f 6a74 0300 005d  }.(js...h/jt...]
 000522b0: 946a 0f07 0000 2981 947d 9428 6a73 0300  .j....)..}.(js..
 000522c0: 0068 2f6a 7403 0000 5d94 6aad 5600 0029  .h/jt...].j.V..)
 000522d0: 8194 7d94 286a 7303 0000 682f 6a74 0300  ..}.(js...h/jt..
 000522e0: 005d 946a 990d 0000 2981 947d 9428 6a73  .].j....)..}.(js
 000522f0: 0300 0068 2f6a 7403 0000 5d94 6a82 0300  ...h/jt...].j...
 00052300: 008c 0966 6c61 675f 7479 7065 9485 9481  ...flag_type....
 00052310: 947d 946a 8703 0000 6ac4 5b00 0073 6261  .}.j....j.[..sba
 00052320: 6a8a 0300 007d 9428 6a8c 0300 005d 946a  j....}.(j....].j
 00052330: 8e03 0000 5d94 6a90 0300 005d 946a 9203  ....].j....].j..
 00052340: 0000 5d94 6a94 0300 005d 948c 0869 6e74  ..].j....]...int
 00052350: 6572 6e61 6c94 888c 0672 6566 7572 6994  ernal....refuri.
-00052360: 6a14 0300 008c 0a61 6e63 686f 726e 616d  j......anchornam
+00052360: 6a18 0300 008c 0a61 6e63 686f 726e 616d  j......anchornam
 00052370: 6594 682f 756a 9603 0000 6a98 0d00 006a  e.h/uj....j....j
 00052380: 8703 0000 6ac1 5b00 0075 6261 6a8a 0300  ....j.[..ubaj...
 00052390: 007d 9428 6a8c 0300 005d 946a 8e03 0000  .}.(j....].j....
 000523a0: 5d94 6a90 0300 005d 946a 9203 0000 5d94  ].j....].j....].
 000523b0: 6a94 0300 005d 9475 6a96 0300 006a ac56  j....].uj....j.V
 000523c0: 0000 6a87 0300 006a be5b 0000 7562 616a  ..j....j.[..ubaj
 000523d0: 8a03 0000 7d94 286a 8c03 0000 5d94 6a8e  ....}.(j....].j.
 000523e0: 0300 005d 946a 9003 0000 5d94 6a92 0300  ...].j....].j...
 000523f0: 005d 946a 9403 0000 5d94 756a 9603 0000  .].j....].uj....
 00052400: 6a0e 0700 006a 8703 0000 6abb 5b00 0075  j....j....j.[..u
 00052410: 6261 6a8a 0300 007d 9428 6a8c 0300 005d  baj....}.(j....]
 00052420: 946a 8e03 0000 5d94 6a90 0300 005d 946a  .j....].j....].j
 00052430: 9203 0000 5d94 6a94 0300 005d 9475 6a96  ....].j....].uj.
-00052440: 0300 006a 0907 0000 7562 6a15 0300 006a  ...j....ubj....j
+00052440: 0300 006a 0907 0000 7562 6a13 0300 006a  ...j....ubj....j
 00052450: 0a07 0000 2981 947d 9428 6a73 0300 0068  ....)..}.(js...h
 00052460: 2f6a 7403 0000 5d94 286a 0f07 0000 2981  /jt...].(j....).
 00052470: 947d 9428 6a73 0300 0068 2f6a 7403 0000  .}.(js...h/jt...
 00052480: 5d94 6aad 5600 0029 8194 7d94 286a 7303  ].j.V..)..}.(js.
 00052490: 0000 682f 6a74 0300 005d 946a 990d 0000  ..h/jt...].j....
 000524a0: 2981 947d 9428 6a73 0300 0068 2f6a 7403  )..}.(js...h/jt.
 000524b0: 0000 5d94 6a82 0300 008c 1d45 7552 6570  ..].j......EuRep
 000524c0: 6f43 2050 6163 6b61 6765 2044 6f63 756d  oC Package Docum
 000524d0: 656e 7461 7469 6f6e 9485 9481 947d 946a  entation.....}.j
 000524e0: 8703 0000 6aef 5b00 0073 6261 6a8a 0300  ....j.[..sbaj...
 000524f0: 007d 9428 6a8c 0300 005d 946a 8e03 0000  .}.(j....].j....
 00052500: 5d94 6a90 0300 005d 946a 9203 0000 5d94  ].j....].j....].
 00052510: 6a94 0300 005d 948c 0869 6e74 6572 6e61  j....]...interna
-00052520: 6c94 888c 0672 6566 7572 6994 6a15 0300  l....refuri.j...
+00052520: 6c94 888c 0672 6566 7572 6994 6a13 0300  l....refuri.j...
 00052530: 008c 0a61 6e63 686f 726e 616d 6594 682f  ...anchorname.h/
 00052540: 756a 9603 0000 6a98 0d00 006a 8703 0000  uj....j....j....
 00052550: 6aec 5b00 0075 6261 6a8a 0300 007d 9428  j.[..ubaj....}.(
 00052560: 6a8c 0300 005d 946a 8e03 0000 5d94 6a90  j....].j....].j.
 00052570: 0300 005d 946a 9203 0000 5d94 6a94 0300  ...].j....].j...
 00052580: 005d 9475 6a96 0300 006a ac56 0000 6a87  .].uj....j.V..j.
 00052590: 0300 006a e95b 0000 7562 616a 8a03 0000  ...j.[..ubaj....
@@ -21090,15 +21090,15 @@
 00052610: 990d 0000 2981 947d 9428 6a73 0300 0068  ....)..}.(js...h
 00052620: 2f6a 7403 0000 5d94 6a82 0300 008c 0a51  /jt...].j......Q
 00052630: 7569 636b 7374 6172 7494 8594 8194 7d94  uickstart.....}.
 00052640: 6a87 0300 006a 115c 0000 7362 616a 8a03  j....j.\..sbaj..
 00052650: 0000 7d94 286a 8c03 0000 5d94 6a8e 0300  ..}.(j....].j...
 00052660: 005d 946a 9003 0000 5d94 6a92 0300 005d  .].j....].j....]
 00052670: 946a 9403 0000 5d94 8c08 696e 7465 726e  .j....]...intern
-00052680: 616c 9488 8c06 7265 6675 7269 946a 1503  al....refuri.j..
+00052680: 616c 9488 8c06 7265 6675 7269 946a 1303  al....refuri.j..
 00052690: 0000 8c0a 616e 6368 6f72 6e61 6d65 948c  ....anchorname..
 000526a0: 0b23 7175 6963 6b73 7461 7274 9475 6a96  .#quickstart.uj.
 000526b0: 0300 006a 980d 0000 6a87 0300 006a 0e5c  ...j....j....j.\
 000526c0: 0000 7562 616a 8a03 0000 7d94 286a 8c03  ..ubaj....}.(j..
 000526d0: 0000 5d94 6a8e 0300 005d 946a 9003 0000  ..].j....].j....
 000526e0: 5d94 6a92 0300 005d 946a 9403 0000 5d94  ].j....].j....].
 000526f0: 756a 9603 0000 6aac 5600 006a 8703 0000  uj....j.V..j....
@@ -21113,29 +21113,29 @@
 00052780: 0000 2981 947d 9428 6a73 0300 0068 2f6a  ..)..}.(js...h/j
 00052790: 7403 0000 5d94 6a82 0300 008c 0843 6f6e  t...].j......Con
 000527a0: 7465 6e74 7394 8594 8194 7d94 6a87 0300  tents.....}.j...
 000527b0: 006a 345c 0000 7362 616a 8a03 0000 7d94  .j4\..sbaj....}.
 000527c0: 286a 8c03 0000 5d94 6a8e 0300 005d 946a  (j....].j....].j
 000527d0: 9003 0000 5d94 6a92 0300 005d 946a 9403  ....].j....].j..
 000527e0: 0000 5d94 8c08 696e 7465 726e 616c 9488  ..]...internal..
-000527f0: 8c06 7265 6675 7269 946a 1503 0000 8c0a  ..refuri.j......
+000527f0: 8c06 7265 6675 7269 946a 1303 0000 8c0a  ..refuri.j......
 00052800: 616e 6368 6f72 6e61 6d65 948c 0923 636f  anchorname...#co
 00052810: 6e74 656e 7473 9475 6a96 0300 006a 980d  ntents.uj....j..
 00052820: 0000 6a87 0300 006a 315c 0000 7562 616a  ..j....j1\..ubaj
 00052830: 8a03 0000 7d94 286a 8c03 0000 5d94 6a8e  ....}.(j....].j.
 00052840: 0300 005d 946a 9003 0000 5d94 6a92 0300  ...].j....].j...
 00052850: 005d 946a 9403 0000 5d94 756a 9603 0000  .].j....].uj....
 00052860: 6aac 5600 006a 8703 0000 6a2e 5c00 0075  j.V..j....j.\..u
 00052870: 626a 0a07 0000 2981 947d 9428 6a73 0300  bj....)..}.(js..
 00052880: 0068 2f6a 7403 0000 5d94 6acc 0300 0029  .h/jt...].j....)
 00052890: 8194 7d94 286a 7403 0000 5d94 6a73 0300  ..}.(jt...].js..
 000528a0: 0068 2f6a 9603 0000 6acb 0300 006a 8a03  .h/j....j....j..
 000528b0: 0000 7d94 286a 8c03 0000 5d94 6a8e 0300  ..}.(j....].j...
 000528c0: 005d 946a 9003 0000 5d94 6a92 0300 005d  .].j....].j....]
-000528d0: 946a 9403 0000 5d94 6a87 0300 006a 1503  .j....].j....j..
+000528d0: 946a 9403 0000 5d94 6a87 0300 006a 1303  .j....].j....j..
 000528e0: 0000 6ad6 0300 006a 6a1b 0000 6ae4 0300  ..j....jj...j...
 000528f0: 006a 711b 0000 6ae6 0300 004b 016a e703  .jq...j....K.j..
 00052900: 0000 6a72 1b00 006a e803 0000 896a e903  ..jr...j.....j..
 00052910: 0000 896a ea03 0000 896a eb03 0000 4b00  ...j.....j....K.
 00052920: 6aec 0300 0089 6aed 0300 006a 731b 0000  j.....j....js...
 00052930: 6a74 1b00 006a 721b 0000 756a 8903 0000  jt...jr...uj....
 00052940: 4b35 6816 6a74 1a00 006a 8703 0000 6a4b  K5h.jt...j....jK
@@ -21155,15 +21155,15 @@
 00052a20: 7403 0000 5d94 6a82 0300 008c 1249 6e64  t...].j......Ind
 00052a30: 6963 6573 2061 6e64 2074 6162 6c65 7394  ices and tables.
 00052a40: 8594 8194 7d94 6a87 0300 006a 695c 0000  ....}.j....ji\..
 00052a50: 7362 616a 8a03 0000 7d94 286a 8c03 0000  sbaj....}.(j....
 00052a60: 5d94 6a8e 0300 005d 946a 9003 0000 5d94  ].j....].j....].
 00052a70: 6a92 0300 005d 946a 9403 0000 5d94 8c08  j....].j....]...
 00052a80: 696e 7465 726e 616c 9488 8c06 7265 6675  internal....refu
-00052a90: 7269 946a 1503 0000 8c0a 616e 6368 6f72  ri.j......anchor
+00052a90: 7269 946a 1303 0000 8c0a 616e 6368 6f72  ri.j......anchor
 00052aa0: 6e61 6d65 948c 1323 696e 6469 6365 732d  name...#indices-
 00052ab0: 616e 642d 7461 626c 6573 9475 6a96 0300  and-tables.uj...
 00052ac0: 006a 980d 0000 6a87 0300 006a 665c 0000  .j....j....jf\..
 00052ad0: 7562 616a 8a03 0000 7d94 286a 8c03 0000  ubaj....}.(j....
 00052ae0: 5d94 6a8e 0300 005d 946a 9003 0000 5d94  ].j....].j....].
 00052af0: 6a92 0300 005d 946a 9403 0000 5d94 756a  j....].j....].uj
 00052b00: 9603 0000 6aac 5600 006a 8703 0000 6a63  ....j.V..j....jc
@@ -21171,56 +21171,56 @@
 00052b20: 0300 005d 946a 8e03 0000 5d94 6a90 0300  ...].j....].j...
 00052b30: 005d 946a 9203 0000 5d94 6a94 0300 005d  .].j....].j....]
 00052b40: 9475 6a96 0300 006a 0e07 0000 6a87 0300  .uj....j....j...
 00052b50: 006a e65b 0000 7562 656a 8a03 0000 7d94  .j.[..ubej....}.
 00052b60: 286a 8c03 0000 5d94 6a8e 0300 005d 946a  (j....].j....].j
 00052b70: 9003 0000 5d94 6a92 0300 005d 946a 9403  ....].j....].j..
 00052b80: 0000 5d94 756a 9603 0000 6a09 0700 0075  ..].uj....j....u
-00052b90: 626a 1903 0000 6a0a 0700 0029 8194 7d94  bj....j....)..}.
+00052b90: 626a 1503 0000 6a0a 0700 0029 8194 7d94  bj....j....)..}.
 00052ba0: 286a 7303 0000 682f 6a74 0300 005d 946a  (js...h/jt...].j
 00052bb0: 0f07 0000 2981 947d 9428 6a73 0300 0068  ....)..}.(js...h
 00052bc0: 2f6a 7403 0000 5d94 6aad 5600 0029 8194  /jt...].j.V..)..
 00052bd0: 7d94 286a 7303 0000 682f 6a74 0300 005d  }.(js...h/jt...]
 00052be0: 946a 990d 0000 2981 947d 9428 6a73 0300  .j....)..}.(js..
 00052bf0: 0068 2f6a 7403 0000 5d94 6a82 0300 008c  .h/jt...].j.....
 00052c00: 1169 6e69 7469 6174 6f72 5f63 6f75 6e74  .initiator_count
 00052c10: 7279 9485 9481 947d 946a 8703 0000 6a95  ry.....}.j....j.
 00052c20: 5c00 0073 6261 6a8a 0300 007d 9428 6a8c  \..sbaj....}.(j.
 00052c30: 0300 005d 946a 8e03 0000 5d94 6a90 0300  ...].j....].j...
 00052c40: 005d 946a 9203 0000 5d94 6a94 0300 005d  .].j....].j....]
 00052c50: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
-00052c60: 6566 7572 6994 6a19 0300 008c 0a61 6e63  efuri.j......anc
+00052c60: 6566 7572 6994 6a15 0300 008c 0a61 6e63  efuri.j......anc
 00052c70: 686f 726e 616d 6594 682f 756a 9603 0000  horname.h/uj....
 00052c80: 6a98 0d00 006a 8703 0000 6a92 5c00 0075  j....j....j.\..u
 00052c90: 6261 6a8a 0300 007d 9428 6a8c 0300 005d  baj....}.(j....]
 00052ca0: 946a 8e03 0000 5d94 6a90 0300 005d 946a  .j....].j....].j
 00052cb0: 9203 0000 5d94 6a94 0300 005d 9475 6a96  ....].j....].uj.
 00052cc0: 0300 006a ac56 0000 6a87 0300 006a 8f5c  ...j.V..j....j.\
 00052cd0: 0000 7562 616a 8a03 0000 7d94 286a 8c03  ..ubaj....}.(j..
 00052ce0: 0000 5d94 6a8e 0300 005d 946a 9003 0000  ..].j....].j....
 00052cf0: 5d94 6a92 0300 005d 946a 9403 0000 5d94  ].j....].j....].
 00052d00: 756a 9603 0000 6a0e 0700 006a 8703 0000  uj....j....j....
 00052d10: 6a8c 5c00 0075 6261 6a8a 0300 007d 9428  j.\..ubaj....}.(
 00052d20: 6a8c 0300 005d 946a 8e03 0000 5d94 6a90  j....].j....].j.
 00052d30: 0300 005d 946a 9203 0000 5d94 6a94 0300  ...].j....].j...
 00052d40: 005d 9475 6a96 0300 006a 0907 0000 7562  .].uj....j....ub
-00052d50: 6a11 0300 006a 0a07 0000 2981 947d 9428  j....j....)..}.(
+00052d50: 6a1a 0300 006a 0a07 0000 2981 947d 9428  j....j....)..}.(
 00052d60: 6a73 0300 0068 2f6a 7403 0000 5d94 6a0f  js...h/jt...].j.
 00052d70: 0700 0029 8194 7d94 286a 7303 0000 682f  ...)..}.(js...h/
 00052d80: 6a74 0300 005d 9428 6aad 5600 0029 8194  jt...].(j.V..)..
 00052d90: 7d94 286a 7303 0000 682f 6a74 0300 005d  }.(js...h/jt...]
 00052da0: 946a 990d 0000 2981 947d 9428 6a73 0300  .j....)..}.(js..
 00052db0: 0068 2f6a 7403 0000 5d94 6a82 0300 008c  .h/jt...].j.....
 00052dc0: 0a72 6561 645f 746f 6b65 6e94 8594 8194  .read_token.....
 00052dd0: 7d94 6a87 0300 006a c05c 0000 7362 616a  }.j....j.\..sbaj
 00052de0: 8a03 0000 7d94 286a 8c03 0000 5d94 6a8e  ....}.(j....].j.
 00052df0: 0300 005d 946a 9003 0000 5d94 6a92 0300  ...].j....].j...
 00052e00: 005d 946a 9403 0000 5d94 8c08 696e 7465  .].j....]...inte
 00052e10: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
-00052e20: 1103 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
+00052e20: 1a03 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
 00052e30: 9468 2f75 6a96 0300 006a 980d 0000 6a87  .h/uj....j....j.
 00052e40: 0300 006a bd5c 0000 7562 616a 8a03 0000  ...j.\..ubaj....
 00052e50: 7d94 286a 8c03 0000 5d94 6a8e 0300 005d  }.(j....].j....]
 00052e60: 946a 9003 0000 5d94 6a92 0300 005d 946a  .j....].j....].j
 00052e70: 9403 0000 5d94 756a 9603 0000 6aac 5600  ....].uj....j.V.
 00052e80: 006a 8703 0000 6aba 5c00 0075 626a 0a07  .j....j.\..ubj..
 00052e90: 0000 2981 947d 9428 6a73 0300 0068 2f6a  ..)..}.(js...h/j
@@ -21237,15 +21237,15 @@
 00052f40: 6a8e 0300 005d 946a 9003 0000 5d94 6a92  j....].j....].j.
 00052f50: 0300 005d 946a 9403 0000 5d94 756a 9603  ...].j....].uj..
 00052f60: 0000 6ab2 0600 006a 8703 0000 6adf 5c00  ..j....j....j.\.
 00052f70: 0075 6261 6a8a 0300 007d 9428 6a8c 0300  .ubaj....}.(j...
 00052f80: 005d 946a 8e03 0000 5d94 6a90 0300 005d  .].j....].j....]
 00052f90: 946a 9203 0000 5d94 6a94 0300 005d 948c  .j....].j....]..
 00052fa0: 0869 6e74 6572 6e61 6c94 888c 0672 6566  .internal....ref
-00052fb0: 7572 6994 6a11 0300 008c 0a61 6e63 686f  uri.j......ancho
+00052fb0: 7572 6994 6a1a 0300 008c 0a61 6e63 686f  uri.j......ancho
 00052fc0: 726e 616d 6594 8c1e 2365 7572 6570 6f63  rname...#eurepoc
 00052fd0: 2e72 6561 645f 746f 6b65 6e2e 7265 6164  .read_token.read
 00052fe0: 5f74 6f6b 656e 9475 6a96 0300 006a 980d  _token.uj....j..
 00052ff0: 0000 6a87 0300 006a dc5c 0000 7562 616a  ..j....j.\..ubaj
 00053000: 8a03 0000 7d94 286a 8c03 0000 5d94 6a8e  ....}.(j....].j.
 00053010: 0300 005d 946a 9003 0000 5d94 6a92 0300  ...].j....].j...
 00053020: 005d 946a 9403 0000 5d94 8c13 736b 6970  .].j....]...skip
@@ -21263,84 +21263,84 @@
 000530e0: 8a03 0000 7d94 286a 8c03 0000 5d94 6a8e  ....}.(j....].j.
 000530f0: 0300 005d 946a 9003 0000 5d94 6a92 0300  ...].j....].j...
 00053100: 005d 946a 9403 0000 5d94 756a 9603 0000  .].j....].uj....
 00053110: 6a0e 0700 006a 8703 0000 6ab7 5c00 0075  j....j....j.\..u
 00053120: 6261 6a8a 0300 007d 9428 6a8c 0300 005d  baj....}.(j....]
 00053130: 946a 8e03 0000 5d94 6a90 0300 005d 946a  .j....].j....].j
 00053140: 9203 0000 5d94 6a94 0300 005d 9475 6a96  ....].j....].uj.
-00053150: 0300 006a 0907 0000 7562 6a17 0300 006a  ...j....ubj....j
+00053150: 0300 006a 0907 0000 7562 6a11 0300 006a  ...j....ubj....j
 00053160: 0a07 0000 2981 947d 9428 6a73 0300 0068  ....)..}.(js...h
 00053170: 2f6a 7403 0000 5d94 6a0f 0700 0029 8194  /jt...].j....)..
 00053180: 7d94 286a 7303 0000 682f 6a74 0300 005d  }.(js...h/jt...]
 00053190: 946a ad56 0000 2981 947d 9428 6a73 0300  .j.V..)..}.(js..
 000531a0: 0068 2f6a 7403 0000 5d94 6a99 0d00 0029  .h/jt...].j....)
 000531b0: 8194 7d94 286a 7303 0000 682f 6a74 0300  ..}.(js...h/jt..
 000531c0: 005d 946a 8203 0000 8c11 7265 6365 6976  .].j......receiv
 000531d0: 6572 5f63 6174 6567 6f72 7994 8594 8194  er_category.....
 000531e0: 7d94 6a87 0300 006a 215d 0000 7362 616a  }.j....j!]..sbaj
 000531f0: 8a03 0000 7d94 286a 8c03 0000 5d94 6a8e  ....}.(j....].j.
 00053200: 0300 005d 946a 9003 0000 5d94 6a92 0300  ...].j....].j...
 00053210: 005d 946a 9403 0000 5d94 8c08 696e 7465  .].j....]...inte
 00053220: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
-00053230: 1703 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
+00053230: 1103 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
 00053240: 9468 2f75 6a96 0300 006a 980d 0000 6a87  .h/uj....j....j.
 00053250: 0300 006a 1e5d 0000 7562 616a 8a03 0000  ...j.]..ubaj....
 00053260: 7d94 286a 8c03 0000 5d94 6a8e 0300 005d  }.(j....].j....]
 00053270: 946a 9003 0000 5d94 6a92 0300 005d 946a  .j....].j....].j
 00053280: 9403 0000 5d94 756a 9603 0000 6aac 5600  ....].uj....j.V.
 00053290: 006a 8703 0000 6a1b 5d00 0075 6261 6a8a  .j....j.]..ubaj.
 000532a0: 0300 007d 9428 6a8c 0300 005d 946a 8e03  ...}.(j....].j..
 000532b0: 0000 5d94 6a90 0300 005d 946a 9203 0000  ..].j....].j....
 000532c0: 5d94 6a94 0300 005d 9475 6a96 0300 006a  ].j....].uj....j
 000532d0: 0e07 0000 6a87 0300 006a 185d 0000 7562  ....j....j.]..ub
 000532e0: 616a 8a03 0000 7d94 286a 8c03 0000 5d94  aj....}.(j....].
 000532f0: 6a8e 0300 005d 946a 9003 0000 5d94 6a92  j....].j....].j.
 00053300: 0300 005d 946a 9403 0000 5d94 756a 9603  ...].j....].uj..
-00053310: 0000 6a09 0700 0075 626a 1603 0000 6a0a  ..j....ubj....j.
+00053310: 0000 6a09 0700 0075 626a 1703 0000 6a0a  ..j....ubj....j.
 00053320: 0700 0029 8194 7d94 286a 7303 0000 682f  ...)..}.(js...h/
 00053330: 6a74 0300 005d 946a 0f07 0000 2981 947d  jt...].j....)..}
 00053340: 9428 6a73 0300 0068 2f6a 7403 0000 5d94  .(js...h/jt...].
 00053350: 6aad 5600 0029 8194 7d94 286a 7303 0000  j.V..)..}.(js...
 00053360: 682f 6a74 0300 005d 946a 990d 0000 2981  h/jt...].j....).
 00053370: 947d 9428 6a73 0300 0068 2f6a 7403 0000  .}.(js...h/jt...
 00053380: 5d94 6a82 0300 008c 1072 6563 6569 7665  ].j......receive
 00053390: 725f 636f 756e 7472 7994 8594 8194 7d94  r_country.....}.
 000533a0: 6a87 0300 006a 4c5d 0000 7362 616a 8a03  j....jL]..sbaj..
 000533b0: 0000 7d94 286a 8c03 0000 5d94 6a8e 0300  ..}.(j....].j...
 000533c0: 005d 946a 9003 0000 5d94 6a92 0300 005d  .].j....].j....]
 000533d0: 946a 9403 0000 5d94 8c08 696e 7465 726e  .j....]...intern
-000533e0: 616c 9488 8c06 7265 6675 7269 946a 1603  al....refuri.j..
+000533e0: 616c 9488 8c06 7265 6675 7269 946a 1703  al....refuri.j..
 000533f0: 0000 8c0a 616e 6368 6f72 6e61 6d65 9468  ....anchorname.h
 00053400: 2f75 6a96 0300 006a 980d 0000 6a87 0300  /uj....j....j...
 00053410: 006a 495d 0000 7562 616a 8a03 0000 7d94  .jI]..ubaj....}.
 00053420: 286a 8c03 0000 5d94 6a8e 0300 005d 946a  (j....].j....].j
 00053430: 9003 0000 5d94 6a92 0300 005d 946a 9403  ....].j....].j..
 00053440: 0000 5d94 756a 9603 0000 6aac 5600 006a  ..].uj....j.V..j
 00053450: 8703 0000 6a46 5d00 0075 6261 6a8a 0300  ....jF]..ubaj...
 00053460: 007d 9428 6a8c 0300 005d 946a 8e03 0000  .}.(j....].j....
 00053470: 5d94 6a90 0300 005d 946a 9203 0000 5d94  ].j....].j....].
 00053480: 6a94 0300 005d 9475 6a96 0300 006a 0e07  j....].uj....j..
 00053490: 0000 6a87 0300 006a 435d 0000 7562 616a  ..j....jC]..ubaj
 000534a0: 8a03 0000 7d94 286a 8c03 0000 5d94 6a8e  ....}.(j....].j.
 000534b0: 0300 005d 946a 9003 0000 5d94 6a92 0300  ...].j....].j...
 000534c0: 005d 946a 9403 0000 5d94 756a 9603 0000  .].j....].uj....
-000534d0: 6a09 0700 0075 626a 1303 0000 6a0a 0700  j....ubj....j...
+000534d0: 6a09 0700 0075 626a 1603 0000 6a0a 0700  j....ubj....j...
 000534e0: 0029 8194 7d94 286a 7303 0000 682f 6a74  .)..}.(js...h/jt
 000534f0: 0300 005d 946a 0f07 0000 2981 947d 9428  ...].j....)..}.(
 00053500: 6a73 0300 0068 2f6a 7403 0000 5d94 6aad  js...h/jt...].j.
 00053510: 5600 0029 8194 7d94 286a 7303 0000 682f  V..)..}.(js...h/
 00053520: 6a74 0300 005d 946a 990d 0000 2981 947d  jt...].j....)..}
 00053530: 9428 6a73 0300 0068 2f6a 7403 0000 5d94  .(js...h/jt...].
 00053540: 6a82 0300 008c 0f72 6563 6569 7665 725f  j......receiver_
 00053550: 7265 6769 6f6e 9485 9481 947d 946a 8703  region.....}.j..
 00053560: 0000 6a77 5d00 0073 6261 6a8a 0300 007d  ..jw]..sbaj....}
 00053570: 9428 6a8c 0300 005d 946a 8e03 0000 5d94  .(j....].j....].
 00053580: 6a90 0300 005d 946a 9203 0000 5d94 6a94  j....].j....].j.
 00053590: 0300 005d 948c 0869 6e74 6572 6e61 6c94  ...]...internal.
-000535a0: 888c 0672 6566 7572 6994 6a13 0300 008c  ...refuri.j.....
+000535a0: 888c 0672 6566 7572 6994 6a16 0300 008c  ...refuri.j.....
 000535b0: 0a61 6e63 686f 726e 616d 6594 682f 756a  .anchorname.h/uj
 000535c0: 9603 0000 6a98 0d00 006a 8703 0000 6a74  ....j....j....jt
 000535d0: 5d00 0075 6261 6a8a 0300 007d 9428 6a8c  ]..ubaj....}.(j.
 000535e0: 0300 005d 946a 8e03 0000 5d94 6a90 0300  ...].j....].j...
 000535f0: 005d 946a 9203 0000 5d94 6a94 0300 005d  .].j....].j....]
 00053600: 9475 6a96 0300 006a ac56 0000 6a87 0300  .uj....j.V..j...
 00053610: 006a 715d 0000 7562 616a 8a03 0000 7d94  .jq]..ubaj....}.
@@ -21349,35 +21349,35 @@
 00053640: 0000 5d94 756a 9603 0000 6a0e 0700 006a  ..].uj....j....j
 00053650: 8703 0000 6a6e 5d00 0075 6261 6a8a 0300  ....jn]..ubaj...
 00053660: 007d 9428 6a8c 0300 005d 946a 8e03 0000  .}.(j....].j....
 00053670: 5d94 6a90 0300 005d 946a 9203 0000 5d94  ].j....].j....].
 00053680: 6a94 0300 005d 9475 6a96 0300 006a 0907  j....].uj....j..
 00053690: 0000 7562 758c 0f74 6f63 5f6e 756d 5f65  ..ubu..toc_num_e
 000536a0: 6e74 7269 6573 947d 9428 6a12 0300 004b  ntries.}.(j....K
-000536b0: 036a 1a03 0000 4b18 6a18 0300 004b 016a  .j....K.j....K.j
-000536c0: 1403 0000 4b01 6a15 0300 004b 046a 1903  ....K.j....K.j..
-000536d0: 0000 4b01 6a11 0300 004b 026a 1703 0000  ..K.j....K.j....
-000536e0: 4b01 6a16 0300 004b 016a 1303 0000 4b01  K.j....K.j....K.
+000536b0: 036a 1903 0000 4b18 6a14 0300 004b 016a  .j....K.j....K.j
+000536c0: 1803 0000 4b01 6a13 0300 004b 046a 1503  ....K.j....K.j..
+000536d0: 0000 4b01 6a1a 0300 004b 026a 1103 0000  ..K.j....K.j....
+000536e0: 4b01 6a17 0300 004b 016a 1603 0000 4b01  K.j....K.j....K.
 000536f0: 758c 0e74 6f63 5f73 6563 6e75 6d62 6572  u..toc_secnumber
 00053700: 7394 7d94 8c0e 746f 635f 6669 676e 756d  s.}...toc_fignum
 00053710: 6265 7273 947d 948c 1074 6f63 7472 6565  bers.}...toctree
 00053720: 5f69 6e63 6c75 6465 7394 7d94 286a 1203  _includes.}.(j..
 00053730: 0000 5d94 286a d803 0000 6ada 0300 006a  ..].(j....j....j
 00053740: dc03 0000 6ade 0300 006a e003 0000 6ae2  ....j....j....j.
-00053750: 0300 0065 6a15 0300 005d 9428 6a6b 1b00  ...ej....].(jk..
+00053750: 0300 0065 6a13 0300 005d 9428 6a6b 1b00  ...ej....].(jk..
 00053760: 006a 6d1b 0000 6a6f 1b00 0065 758c 1066  .jm...jo...eu..f
 00053770: 696c 6573 5f74 6f5f 7265 6275 696c 6494  iles_to_rebuild.
 00053780: 7d94 286a d803 0000 8f94 286a 1203 0000  }.(j......(j....
 00053790: 906a da03 0000 8f94 286a 1203 0000 906a  .j......(j.....j
 000537a0: dc03 0000 8f94 286a 1203 0000 906a de03  ......(j.....j..
 000537b0: 0000 8f94 286a 1203 0000 906a e003 0000  ....(j.....j....
 000537c0: 8f94 286a 1203 0000 906a e203 0000 8f94  ..(j.....j......
 000537d0: 286a 1203 0000 906a 6b1b 0000 8f94 286a  (j.....jk.....(j
-000537e0: 1503 0000 906a 6d1b 0000 8f94 286a 1503  .....jm.....(j..
-000537f0: 0000 906a 6f1b 0000 8f94 286a 1503 0000  ...jo.....(j....
+000537e0: 1303 0000 906a 6d1b 0000 8f94 286a 1303  .....jm.....(j..
+000537f0: 0000 906a 6f1b 0000 8f94 286a 1303 0000  ...jo.....(j....
 00053800: 9075 8c0d 676c 6f62 5f74 6f63 7472 6565  .u..glob_toctree
 00053810: 7394 8f94 8c11 6e75 6d62 6572 6564 5f74  s.....numbered_t
 00053820: 6f63 7472 6565 7394 8f94 8c0a 646f 6d61  octrees.....doma
 00053830: 696e 6461 7461 947d 9428 8c01 6394 7d94  indata.}.(..c.}.
 00053840: 288c 0b72 6f6f 745f 7379 6d62 6f6c 948c  (..root_symbol..
 00053850: 1873 7068 696e 782e 646f 6d61 696e 732e  .sphinx.domains.
 00053860: 632e 5f73 796d 626f 6c94 8c06 5379 6d62  c._symbol...Symb
@@ -21404,35 +21404,35 @@
 000539b0: 7465 5061 7261 6d73 944e 8c0c 7465 6d70  teParams.N..temp
 000539c0: 6c61 7465 4172 6773 944e 6abf 5d00 004e  lateArgs.Nj.]..N
 000539d0: 6ac0 5d00 004e 6a89 0300 004e 6ac1 5d00  j.]..Nj....Nj.].
 000539e0: 0089 6ac2 5d00 005d 946a c45d 0000 5d94  ..j.]..].j.]..].
 000539f0: 7562 6a90 0300 007d 9468 304b 0075 683d  ubj....}.h0K.uh=
 00053a00: 7d94 2868 304b 006a d603 0000 7d94 286a  }.(h0K.j....}.(j
 00053a10: 1203 0000 5d94 286a 0504 0000 6a14 0400  ....].(j....j...
-00053a20: 006a f40b 0000 656a 1a03 0000 5d94 286a  .j....ej....].(j
+00053a20: 006a f40b 0000 656a 1903 0000 5d94 286a  .j....ej....].(j
 00053a30: bc0d 0000 6aca 0d00 006a df0f 0000 6a46  ....j....j....jF
 00053a40: 1000 006a ad10 0000 6a14 1100 006a 7b11  ...j....j....j{.
 00053a50: 0000 6ae2 1100 006a 4912 0000 6ab0 1200  ..j....jI...j...
 00053a60: 006a 1713 0000 6ab3 1300 006a 1a14 0000  .j....j....j....
 00053a70: 6a81 1400 006a e814 0000 6a4f 1500 006a  j....j....jO...j
 00053a80: b615 0000 6a1d 1600 006a 8416 0000 6aeb  ....j....j....j.
 00053a90: 1600 006a 5217 0000 6ab9 1700 006a 2018  ...jR...j....j .
-00053aa0: 0000 6a87 1800 0065 6a18 0300 005d 946a  ..j....ej....].j
-00053ab0: 1403 0000 5d94 6a15 0300 005d 946a 1903  ....].j....].j..
-00053ac0: 0000 5d94 6a11 0300 005d 9428 6a46 3400  ..].j....].(jF4.
-00053ad0: 006a 5434 0000 656a 1703 0000 5d94 6a16  .jT4..ej....].j.
-00053ae0: 0300 005d 946a 1303 0000 5d94 7575 8c02  ...].j....].uu..
+00053aa0: 0000 6a87 1800 0065 6a14 0300 005d 946a  ..j....ej....].j
+00053ab0: 1803 0000 5d94 6a13 0300 005d 946a 1503  ....].j....].j..
+00053ac0: 0000 5d94 6a1a 0300 005d 9428 6a46 3400  ..].j....].(jF4.
+00053ad0: 006a 5434 0000 656a 1103 0000 5d94 6a17  .jT4..ej....].j.
+00053ae0: 0300 005d 946a 1603 0000 5d94 7575 8c02  ...].j....].uu..
 00053af0: 6a73 947d 9428 6ac6 5d00 007d 948c 076d  js.}.(j.]..}...m
 00053b00: 6f64 756c 6573 947d 9468 304b 0075 8c04  odules.}.h0K.u..
 00053b10: 6d61 7468 947d 9428 6ac6 5d00 007d 948c  math.}.(j.]..}..
 00053b20: 0d68 6173 5f65 7175 6174 696f 6e73 947d  .has_equations.}
-00053b30: 9428 6a12 0300 0089 6a1a 0300 0089 6a18  .(j.....j.....j.
-00053b40: 0300 0089 6a14 0300 0089 6a15 0300 0089  ....j.....j.....
-00053b50: 6a19 0300 0089 6a11 0300 0089 6a17 0300  j.....j.....j...
-00053b60: 0089 6a16 0300 0089 6a13 0300 0089 7568  ..j.....j.....uh
+00053b30: 9428 6a12 0300 0089 6a19 0300 0089 6a14  .(j.....j.....j.
+00053b40: 0300 0089 6a18 0300 0089 6a13 0300 0089  ....j.....j.....
+00053b50: 6a15 0300 0089 6a1a 0300 0089 6a11 0300  j.....j.....j...
+00053b60: 0089 6a17 0300 0089 6a16 0300 0089 7568  ..j.....j.....uh
 00053b70: 304b 0075 6864 7d94 286a c65d 0000 7d94  0K.uhd}.(j.]..}.
 00053b80: 288c 1665 7572 6570 6f63 2e64 6174 6162  (..eurepoc.datab
 00053b90: 6173 655f 7175 6572 7994 8c15 7370 6869  ase_query...sphi
 00053ba0: 6e78 2e64 6f6d 6169 6e73 2e70 7974 686f  nx.domains.pytho
 00053bb0: 6e94 8c0b 4f62 6a65 6374 456e 7472 7994  n...ObjectEntry.
 00053bc0: 9394 286a 1203 0000 6a04 0400 006a 9906  ..(j....j....j..
 00053bd0: 0000 8974 9481 948c 2465 7572 6570 6f63  ...t....$eurepoc
@@ -21442,178 +21442,178 @@
 00053c10: 0c00 0089 7494 8194 8c32 6575 7265 706f  ....t....2eurepo
 00053c20: 632e 6461 7461 6261 7365 5f71 7565 7279  c.database_query
 00053c30: 2e44 6174 6162 6173 6551 7565 7279 2e65  .DatabaseQuery.e
 00053c40: 7865 6375 7465 5f71 7565 7279 946a f75d  xecute_query.j.]
 00053c50: 0000 286a 1203 0000 6af3 0b00 006a c50c  ..(j....j....j..
 00053c60: 0000 8974 9481 948c 1b65 7572 6570 6f63  ...t.....eurepoc
 00053c70: 2e69 6e63 6964 656e 745f 6461 7461 6672  .incident_datafr
-00053c80: 616d 6573 946a f75d 0000 286a 1a03 0000  ames.j.]..(j....
+00053c80: 616d 6573 946a f75d 0000 286a 1903 0000  ames.j.]..(j....
 00053c90: 6abb 0d00 006a 9906 0000 8974 9481 948c  j....j.....t....
 00053ca0: 3665 7572 6570 6f63 2e69 6e63 6964 656e  6eurepoc.inciden
 00053cb0: 745f 6461 7461 6672 616d 6573 2e49 6e63  t_dataframes.Inc
 00053cc0: 6964 656e 7444 6174 6146 7261 6d65 4765  identDataFrameGe
-00053cd0: 6e65 7261 746f 7294 6af7 5d00 0028 6a1a  nerator.j.]..(j.
+00053cd0: 6e65 7261 746f 7294 6af7 5d00 0028 6a19  nerator.j.]..(j.
 00053ce0: 0300 006a c90d 0000 6aea 1800 0089 7494  ...j....j.....t.
 00053cf0: 8194 8c4e 6575 7265 706f 632e 696e 6369  ...Neurepoc.inci
 00053d00: 6465 6e74 5f64 6174 6166 7261 6d65 732e  dent_dataframes.
 00053d10: 496e 6369 6465 6e74 4461 7461 4672 616d  IncidentDataFram
 00053d20: 6547 656e 6572 6174 6f72 2e67 6574 5f61  eGenerator.get_a
 00053d30: 7474 7269 6275 7469 6f6e 5f73 6f75 7263  ttribution_sourc
-00053d40: 6573 946a f75d 0000 286a 1a03 0000 6ade  es.j.]..(j....j.
+00053d40: 6573 946a f75d 0000 286a 1903 0000 6ade  es.j.]..(j....j.
 00053d50: 0f00 006a 3510 0000 8974 9481 948c 4765  ...j5....t....Ge
 00053d60: 7572 6570 6f63 2e69 6e63 6964 656e 745f  urepoc.incident_
 00053d70: 6461 7461 6672 616d 6573 2e49 6e63 6964  dataframes.Incid
 00053d80: 656e 7444 6174 6146 7261 6d65 4765 6e65  entDataFrameGene
 00053d90: 7261 746f 722e 6765 745f 6174 7472 6962  rator.get_attrib
-00053da0: 7574 696f 6e73 946a f75d 0000 286a 1a03  utions.j.]..(j..
+00053da0: 7574 696f 6e73 946a f75d 0000 286a 1903  utions.j.]..(j..
 00053db0: 0000 6a45 1000 006a 9c10 0000 8974 9481  ..jE...j.....t..
 00053dc0: 948c 5065 7572 6570 6f63 2e69 6e63 6964  ..Peurepoc.incid
 00053dd0: 656e 745f 6461 7461 6672 616d 6573 2e49  ent_dataframes.I
 00053de0: 6e63 6964 656e 7444 6174 6146 7261 6d65  ncidentDataFrame
 00053df0: 4765 6e65 7261 746f 722e 6765 745f 6379  Generator.get_cy
 00053e00: 6265 725f 636f 6e66 6c69 6374 5f69 7373  ber_conflict_iss
-00053e10: 7565 7394 6af7 5d00 0028 6a1a 0300 006a  ues.j.]..(j....j
+00053e10: 7565 7394 6af7 5d00 0028 6a19 0300 006a  ues.j.]..(j....j
 00053e20: ac10 0000 6a03 1100 0089 7494 8194 8c54  ....j.....t....T
 00053e30: 6575 7265 706f 632e 696e 6369 6465 6e74  eurepoc.incident
 00053e40: 5f64 6174 6166 7261 6d65 732e 496e 6369  _dataframes.Inci
 00053e50: 6465 6e74 4461 7461 4672 616d 6547 656e  dentDataFrameGen
 00053e60: 6572 6174 6f72 2e67 6574 5f63 7962 6572  erator.get_cyber
 00053e70: 5f69 6e74 656e 7369 7479 5f76 6172 6961  _intensity_varia
-00053e80: 626c 6573 946a f75d 0000 286a 1a03 0000  bles.j.]..(j....
+00053e80: 626c 6573 946a f75d 0000 286a 1903 0000  bles.j.]..(j....
 00053e90: 6a13 1100 006a 6a11 0000 8974 9481 948c  j....jj....t....
 00053ea0: 4e65 7572 6570 6f63 2e69 6e63 6964 656e  Neurepoc.inciden
 00053eb0: 745f 6461 7461 6672 616d 6573 2e49 6e63  t_dataframes.Inc
 00053ec0: 6964 656e 7444 6174 6146 7261 6d65 4765  identDataFrameGe
 00053ed0: 6e65 7261 746f 722e 6765 745f 696c 5f62  nerator.get_il_b
 00053ee0: 7265 6163 685f 696e 6469 6361 746f 7294  reach_indicator.
-00053ef0: 6af7 5d00 0028 6a1a 0300 006a 7a11 0000  j.]..(j....jz...
+00053ef0: 6af7 5d00 0028 6a19 0300 006a 7a11 0000  j.]..(j....jz...
 00053f00: 6ad1 1100 0089 7494 8194 8c55 6575 7265  j.....t....Ueure
 00053f10: 706f 632e 696e 6369 6465 6e74 5f64 6174  poc.incident_dat
 00053f20: 6166 7261 6d65 732e 496e 6369 6465 6e74  aframes.Incident
 00053f30: 4461 7461 4672 616d 6547 656e 6572 6174  DataFrameGenerat
 00053f40: 6f72 2e67 6574 5f69 6d70 6163 745f 696e  or.get_impact_in
 00053f50: 6469 6361 746f 725f 7661 7269 6162 6c65  dicator_variable
-00053f60: 7394 6af7 5d00 0028 6a1a 0300 006a e111  s.j.]..(j....j..
+00053f60: 7394 6af7 5d00 0028 6a19 0300 006a e111  s.j.]..(j....j..
 00053f70: 0000 6a38 1200 0089 7494 8194 8c49 6575  ..j8....t....Ieu
 00053f80: 7265 706f 632e 696e 6369 6465 6e74 5f64  repoc.incident_d
 00053f90: 6174 6166 7261 6d65 732e 496e 6369 6465  ataframes.Incide
 00053fa0: 6e74 4461 7461 4672 616d 6547 656e 6572  ntDataFrameGener
 00053fb0: 6174 6f72 2e67 6574 5f69 6e63 6964 656e  ator.get_inciden
-00053fc0: 745f 7479 7065 7394 6af7 5d00 0028 6a1a  t_types.j.]..(j.
+00053fc0: 745f 7479 7065 7394 6af7 5d00 0028 6a19  t_types.j.]..(j.
 00053fd0: 0300 006a 4812 0000 6a9f 1200 0089 7494  ...jH...j.....t.
 00053fe0: 8194 8c4d 6575 7265 706f 632e 696e 6369  ...Meurepoc.inci
 00053ff0: 6465 6e74 5f64 6174 6166 7261 6d65 732e  dent_dataframes.
 00054000: 496e 6369 6465 6e74 4461 7461 4672 616d  IncidentDataFram
 00054010: 6547 656e 6572 6174 6f72 2e67 6574 5f69  eGenerator.get_i
 00054020: 6e63 6c75 7369 6f6e 5f63 7269 7465 7269  nclusion_criteri
-00054030: 6194 6af7 5d00 0028 6a1a 0300 006a af12  a.j.]..(j....j..
+00054030: 6194 6af7 5d00 0028 6a19 0300 006a af12  a.j.]..(j....j..
 00054040: 0000 6a06 1300 0089 7494 8194 8c45 6575  ..j.....t....Eeu
 00054050: 7265 706f 632e 696e 6369 6465 6e74 5f64  repoc.incident_d
 00054060: 6174 6166 7261 6d65 732e 496e 6369 6465  ataframes.Incide
 00054070: 6e74 4461 7461 4672 616d 6547 656e 6572  ntDataFrameGener
 00054080: 6174 6f72 2e67 6574 5f69 6e69 7469 6174  ator.get_initiat
-00054090: 6f72 7394 6af7 5d00 0028 6a1a 0300 006a  ors.j.]..(j....j
+00054090: 6f72 7394 6af7 5d00 0028 6a19 0300 006a  ors.j.]..(j....j
 000540a0: 1613 0000 6aa2 1300 0089 7494 8194 8c4a  ....j.....t....J
 000540b0: 6575 7265 706f 632e 696e 6369 6465 6e74  eurepoc.incident
 000540c0: 5f64 6174 6166 7261 6d65 732e 496e 6369  _dataframes.Inci
 000540d0: 6465 6e74 4461 7461 4672 616d 6547 656e  dentDataFrameGen
 000540e0: 6572 6174 6f72 2e67 6574 5f6c 6567 616c  erator.get_legal
 000540f0: 5f72 6573 706f 6e73 6573 946a f75d 0000  _responses.j.]..
-00054100: 286a 1a03 0000 6ab2 1300 006a 0914 0000  (j....j....j....
+00054100: 286a 1903 0000 6ab2 1300 006a 0914 0000  (j....j....j....
 00054110: 8974 9481 948c 4a65 7572 6570 6f63 2e69  .t....Jeurepoc.i
 00054120: 6e63 6964 656e 745f 6461 7461 6672 616d  ncident_datafram
 00054130: 6573 2e49 6e63 6964 656e 7444 6174 6146  es.IncidentDataF
 00054140: 7261 6d65 4765 6e65 7261 746f 722e 6765  rameGenerator.ge
 00054150: 745f 6c65 6761 6c5f 7661 7269 6162 6c65  t_legal_variable
-00054160: 7394 6af7 5d00 0028 6a1a 0300 006a 1914  s.j.]..(j....j..
+00054160: 7394 6af7 5d00 0028 6a19 0300 006a 1914  s.j.]..(j....j..
 00054170: 0000 6a70 1400 0089 7494 8194 8c44 6575  ..jp....t....Deu
 00054180: 7265 706f 632e 696e 6369 6465 6e74 5f64  repoc.incident_d
 00054190: 6174 6166 7261 6d65 732e 496e 6369 6465  ataframes.Incide
 000541a0: 6e74 4461 7461 4672 616d 6547 656e 6572  ntDataFrameGener
 000541b0: 6174 6f72 2e67 6574 5f6d 6169 6e5f 6461  ator.get_main_da
-000541c0: 7461 946a f75d 0000 286a 1a03 0000 6a80  ta.j.]..(j....j.
+000541c0: 7461 946a f75d 0000 286a 1903 0000 6a80  ta.j.]..(j....j.
 000541d0: 1400 006a d714 0000 8974 9481 948c 4765  ...j.....t....Ge
 000541e0: 7572 6570 6f63 2e69 6e63 6964 656e 745f  urepoc.incident_
 000541f0: 6461 7461 6672 616d 6573 2e49 6e63 6964  dataframes.Incid
 00054200: 656e 7444 6174 6146 7261 6d65 4765 6e65  entDataFrameGene
 00054210: 7261 746f 722e 6765 745f 6d69 7472 655f  rator.get_mitre_
-00054220: 696d 7061 6374 946a f75d 0000 286a 1a03  impact.j.]..(j..
+00054220: 696d 7061 6374 946a f75d 0000 286a 1903  impact.j.]..(j..
 00054230: 0000 6ae7 1400 006a 3e15 0000 8974 9481  ..j....j>....t..
 00054240: 948c 4f65 7572 6570 6f63 2e69 6e63 6964  ..Oeurepoc.incid
 00054250: 656e 745f 6461 7461 6672 616d 6573 2e49  ent_dataframes.I
 00054260: 6e63 6964 656e 7444 6174 6146 7261 6d65  ncidentDataFrame
 00054270: 4765 6e65 7261 746f 722e 6765 745f 6d69  Generator.get_mi
 00054280: 7472 655f 696e 6974 6961 6c5f 6163 6365  tre_initial_acce
-00054290: 7373 946a f75d 0000 286a 1a03 0000 6a4e  ss.j.]..(j....jN
+00054290: 7373 946a f75d 0000 286a 1903 0000 6a4e  ss.j.]..(j....jN
 000542a0: 1500 006a a515 0000 8974 9481 948c 4c65  ...j.....t....Le
 000542b0: 7572 6570 6f63 2e69 6e63 6964 656e 745f  urepoc.incident_
 000542c0: 6461 7461 6672 616d 6573 2e49 6e63 6964  dataframes.Incid
 000542d0: 656e 7444 6174 6146 7261 6d65 4765 6e65  entDataFrameGene
 000542e0: 7261 746f 722e 6765 745f 6f66 666c 696e  rator.get_offlin
 000542f0: 655f 636f 6e66 6c69 6374 7394 6af7 5d00  e_conflicts.j.].
-00054300: 0028 6a1a 0300 006a b515 0000 6a0c 1600  .(j....j....j...
+00054300: 0028 6a19 0300 006a b515 0000 6a0c 1600  .(j....j....j...
 00054310: 0089 7494 8194 8c4a 6575 7265 706f 632e  ..t....Jeurepoc.
 00054320: 696e 6369 6465 6e74 5f64 6174 6166 7261  incident_datafra
 00054330: 6d65 732e 496e 6369 6465 6e74 4461 7461  mes.IncidentData
 00054340: 4672 616d 6547 656e 6572 6174 6f72 2e67  FrameGenerator.g
 00054350: 6574 5f6f 7065 7261 7469 6f6e 5f74 7970  et_operation_typ
-00054360: 6573 946a f75d 0000 286a 1a03 0000 6a1c  es.j.]..(j....j.
+00054360: 6573 946a f75d 0000 286a 1903 0000 6a1c  es.j.]..(j....j.
 00054370: 1600 006a 7316 0000 8974 9481 948c 4e65  ...js....t....Ne
 00054380: 7572 6570 6f63 2e69 6e63 6964 656e 745f  urepoc.incident_
 00054390: 6461 7461 6672 616d 6573 2e49 6e63 6964  dataframes.Incid
 000543a0: 656e 7444 6174 6146 7261 6d65 4765 6e65  entDataFrameGene
 000543b0: 7261 746f 722e 6765 745f 706f 6c69 7469  rator.get_politi
 000543c0: 6361 6c5f 7265 7370 6f6e 7365 7394 6af7  cal_responses.j.
-000543d0: 5d00 0028 6a1a 0300 006a 8316 0000 6ada  ]..(j....j....j.
+000543d0: 5d00 0028 6a19 0300 006a 8316 0000 6ada  ]..(j....j....j.
 000543e0: 1600 0089 7494 8194 8c44 6575 7265 706f  ....t....Deurepo
 000543f0: 632e 696e 6369 6465 6e74 5f64 6174 6166  c.incident_dataf
 00054400: 7261 6d65 732e 496e 6369 6465 6e74 4461  rames.IncidentDa
 00054410: 7461 4672 616d 6547 656e 6572 6174 6f72  taFrameGenerator
 00054420: 2e67 6574 5f72 6563 6569 7665 7273 946a  .get_receivers.j
-00054430: f75d 0000 286a 1a03 0000 6aea 1600 006a  .]..(j....j....j
+00054430: f75d 0000 286a 1903 0000 6aea 1600 006a  .]..(j....j....j
 00054440: 4117 0000 8974 9481 948c 4765 7572 6570  A....t....Geurep
 00054450: 6f63 2e69 6e63 6964 656e 745f 6461 7461  oc.incident_data
 00054460: 6672 616d 6573 2e49 6e63 6964 656e 7444  frames.IncidentD
 00054470: 6174 6146 7261 6d65 4765 6e65 7261 746f  ataFrameGenerato
 00054480: 722e 6765 745f 736f 7572 6365 5f6e 616d  r.get_source_nam
-00054490: 6573 946a f75d 0000 286a 1a03 0000 6a51  es.j.]..(j....jQ
+00054490: 6573 946a f75d 0000 286a 1903 0000 6a51  es.j.]..(j....jQ
 000544a0: 1700 006a a817 0000 8974 9481 948c 5065  ...j.....t....Pe
 000544b0: 7572 6570 6f63 2e69 6e63 6964 656e 745f  urepoc.incident_
 000544c0: 6461 7461 6672 616d 6573 2e49 6e63 6964  dataframes.Incid
 000544d0: 656e 7444 6174 6146 7261 6d65 4765 6e65  entDataFrameGene
 000544e0: 7261 746f 722e 6765 745f 736f 7572 6365  rator.get_source
 000544f0: 735f 6f66 5f64 6973 636c 6f73 7572 6594  s_of_disclosure.
-00054500: 6af7 5d00 0028 6a1a 0300 006a b817 0000  j.]..(j....j....
+00054500: 6af7 5d00 0028 6a19 0300 006a b817 0000  j.]..(j....j....
 00054510: 6a0f 1800 0089 7494 8194 8c47 6575 7265  j.....t....Geure
 00054520: 706f 632e 696e 6369 6465 6e74 5f64 6174  poc.incident_dat
 00054530: 6166 7261 6d65 732e 496e 6369 6465 6e74  aframes.Incident
 00054540: 4461 7461 4672 616d 6547 656e 6572 6174  DataFrameGenerat
 00054550: 6f72 2e67 6574 5f73 6f75 7263 6573 5f75  or.get_sources_u
-00054560: 726c 7394 6af7 5d00 0028 6a1a 0300 006a  rls.j.]..(j....j
+00054560: 726c 7394 6af7 5d00 0028 6a19 0300 006a  rls.j.]..(j....j
 00054570: 1f18 0000 6a76 1800 0089 7494 8194 8c4e  ....jv....t....N
 00054580: 6575 7265 706f 632e 696e 6369 6465 6e74  eurepoc.incident
 00054590: 5f64 6174 6166 7261 6d65 732e 496e 6369  _dataframes.Inci
 000545a0: 6465 6e74 4461 7461 4672 616d 6547 656e  dentDataFrameGen
 000545b0: 6572 6174 6f72 2e67 6574 5f74 6563 686e  erator.get_techn
 000545c0: 6963 616c 5f76 6172 6961 626c 6573 946a  ical_variables.j
-000545d0: f75d 0000 286a 1a03 0000 6a86 1800 006a  .]..(j....j....j
+000545d0: f75d 0000 286a 1903 0000 6a86 1800 006a  .]..(j....j....j
 000545e0: dd18 0000 8974 9481 948c 1265 7572 6570  .....t.....eurep
 000545f0: 6f63 2e72 6561 645f 746f 6b65 6e94 6af7  oc.read_token.j.
-00054600: 5d00 0028 6a11 0300 006a 4534 0000 6a99  ]..(j....jE4..j.
+00054600: 5d00 0028 6a1a 0300 006a 4534 0000 6a99  ]..(j....jE4..j.
 00054610: 0600 0089 7494 8194 8c1d 6575 7265 706f  ....t.....eurepo
 00054620: 632e 7265 6164 5f74 6f6b 656e 2e72 6561  c.read_token.rea
-00054630: 645f 746f 6b65 6e94 6af7 5d00 0028 6a11  d_token.j.]..(j.
+00054630: 645f 746f 6b65 6e94 6af7 5d00 0028 6a1a  d_token.j.]..(j.
 00054640: 0300 006a 5334 0000 6a8b 3600 0089 7494  ...jS4..j.6...t.
 00054650: 8194 756a eb5d 0000 7d94 286a f45d 0000  ..uj.]..}.(j.]..
 00054660: 6af5 5d00 008c 0b4d 6f64 756c 6545 6e74  j.]....ModuleEnt
 00054670: 7279 9493 9428 6a12 0300 006a 0404 0000  ry...(j....j....
 00054680: 682f 682f 8974 9481 946a 005e 0000 6a50  h/h/.t...j.^..jP
-00054690: 5e00 0028 6a1a 0300 006a bb0d 0000 682f  ^..(j....j....h/
+00054690: 5e00 0028 6a19 0300 006a bb0d 0000 682f  ^..(j....j....h/
 000546a0: 682f 8974 9481 946a 485e 0000 6a50 5e00  h/.t...jH^..jP^.
-000546b0: 0028 6a11 0300 006a 4534 0000 682f 682f  .(j....jE4..h/h/
+000546b0: 0028 6a1a 0300 006a 4534 0000 682f 682f  .(j....jE4..h/h/
 000546c0: 8974 9481 9475 6830 4b00 758c 0372 7374  .t...uh0K.u..rst
 000546d0: 947d 9428 6ac6 5d00 007d 9468 304b 0075  .}.(j.]..}.h0K.u
 000546e0: 8c03 7374 6494 7d94 288c 0b70 726f 676f  ..std.}.(..progo
 000546f0: 7074 696f 6e73 947d 946a c65d 0000 7d94  ptions.}.j.]..}.
 00054700: 8c06 6c61 6265 6c73 947d 9428 8c08 6765  ..labels.}.(..ge
 00054710: 6e69 6e64 6578 946a 615e 0000 682f 8c0d  nindex.ja^..h/..
 00054720: 7370 6869 6e78 2e6c 6f63 616c 6594 8c11  sphinx.locale...
@@ -22644,29 +22644,29 @@
 00058730: 8794 8c32 496e 6369 6465 6e74 4461 7461  ...2IncidentData
 00058740: 4672 616d 6547 656e 6572 6174 6f72 2e67  FrameGenerator.g
 00058750: 6574 5f61 7474 7269 6275 7469 6f6e 5f73  et_attribution_s
 00058760: 6f75 7263 6573 946a a65e 0000 4bb2 4bb4  ources.j.^..K.K.
 00058770: 8794 8c1a 496e 6369 6465 6e74 4461 7461  ....IncidentData
 00058780: 4672 616d 6547 656e 6572 6174 6f72 946a  FrameGenerator.j
 00058790: 6b01 0000 4b10 4bb4 8794 757d 9428 6a0a  k...K.K...u}.(j.
-000587a0: 0e00 006a 1a03 0000 6a0d 1000 006a 1a03  ...j....j....j..
-000587b0: 0000 6a74 1000 006a 1a03 0000 6adb 1000  ..jt...j....j...
-000587c0: 006a 1a03 0000 6a42 1100 006a 1a03 0000  .j....jB...j....
-000587d0: 6aa9 1100 006a 1a03 0000 6a10 1200 006a  j....j....j....j
-000587e0: 1a03 0000 6a77 1200 006a 1a03 0000 6ade  ....jw...j....j.
-000587f0: 1200 006a 1a03 0000 6a7a 1300 006a 1a03  ...j....jz...j..
-00058800: 0000 6ae1 1300 006a 1a03 0000 6a48 1400  ..j....j....jH..
-00058810: 006a 1a03 0000 6aaf 1400 006a 1a03 0000  .j....j....j....
-00058820: 6a16 1500 006a 1a03 0000 6a7d 1500 006a  j....j....j}...j
-00058830: 1a03 0000 6ae4 1500 006a 1a03 0000 6a4b  ....j....j....jK
-00058840: 1600 006a 1a03 0000 6ab2 1600 006a 1a03  ...j....j....j..
-00058850: 0000 6a19 1700 006a 1a03 0000 6a80 1700  ..j....j....j...
-00058860: 006a 1a03 0000 6ae7 1700 006a 1a03 0000  .j....j....j....
-00058870: 6a4e 1800 006a 1a03 0000 6ab5 1800 006a  jN...j....j....j
-00058880: 1a03 0000 756a 680e 0000 7494 8c12 6575  ....ujh...t...eu
+000587a0: 0e00 006a 1903 0000 6a0d 1000 006a 1903  ...j....j....j..
+000587b0: 0000 6a74 1000 006a 1903 0000 6adb 1000  ..jt...j....j...
+000587c0: 006a 1903 0000 6a42 1100 006a 1903 0000  .j....jB...j....
+000587d0: 6aa9 1100 006a 1903 0000 6a10 1200 006a  j....j....j....j
+000587e0: 1903 0000 6a77 1200 006a 1903 0000 6ade  ....jw...j....j.
+000587f0: 1200 006a 1903 0000 6a7a 1300 006a 1903  ...j....jz...j..
+00058800: 0000 6ae1 1300 006a 1903 0000 6a48 1400  ..j....j....jH..
+00058810: 006a 1903 0000 6aaf 1400 006a 1903 0000  .j....j....j....
+00058820: 6a16 1500 006a 1903 0000 6a7d 1500 006a  j....j....j}...j
+00058830: 1903 0000 6ae4 1500 006a 1903 0000 6a4b  ....j....j....jK
+00058840: 1600 006a 1903 0000 6ab2 1600 006a 1903  ...j....j....j..
+00058850: 0000 6a19 1700 006a 1903 0000 6a80 1700  ..j....j....j...
+00058860: 006a 1903 0000 6ae7 1700 006a 1903 0000  .j....j....j....
+00058870: 6a4e 1800 006a 1903 0000 6ab5 1800 006a  jN...j....j....j
+00058880: 1903 0000 756a 680e 0000 7494 8c12 6575  ....ujh...t...eu
 00058890: 7265 706f 632e 7265 6164 5f74 6f6b 656e  repoc.read_token
 000588a0: 9428 589c 0300 0064 6566 2072 6561 645f  .(X....def read_
 000588b0: 746f 6b65 6e28 7465 7874 5f66 696c 653d  token(text_file=
 000588c0: 2741 5049 5f74 6f6b 656e 2e74 7874 2729  'API_token.txt')
 000588d0: 3a0a 2020 2020 2222 220a 2020 2020 2020  :.    """.      
 000588e0: 2020 5265 7472 6965 7665 7320 7468 6520    Retrieves the 
 000588f0: 4150 4920 746f 6b65 6e20 6672 6f6d 2061  API token from a
@@ -22720,9 +22720,9 @@
 00058bf0: 6e64 2229 0a20 2020 2065 7863 6570 7420  nd").    except 
 00058c00: 4578 6365 7074 696f 6e20 6173 2065 3a0a  Exception as e:.
 00058c10: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
 00058c20: 6365 7074 696f 6e28 6622 416e 2065 7272  ception(f"An err
 00058c30: 6f72 206f 6363 7572 7265 643a 207b 657d  or occurred: {e}
 00058c40: 2229 0a94 7d94 8c0a 7265 6164 5f74 6f6b  ")..}...read_tok
 00058c50: 656e 946a a65e 0000 4b01 4b19 8794 737d  en.j.^..K.K...s}
-00058c60: 946a 6d34 0000 6a11 0300 0073 6acb 3400  .jm4..j....sj.4.
+00058c60: 946a 6d34 0000 6a1a 0300 0073 6acb 3400  .jm4..j....sj.4.
 00058c70: 0074 9475 7562 2e                        .t.uub.
```

### Comparing `eurepoc-0.1.4/docs/build/.doctrees/flag_type.doctree` & `eurepoc-0.1.5/docs/build/.doctrees/flag_type.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/.doctrees/index.doctree` & `eurepoc-0.1.5/docs/build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/.doctrees/initiator_country.doctree` & `eurepoc-0.1.5/docs/build/.doctrees/initiator_country.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/.doctrees/read_token.doctree` & `eurepoc-0.1.5/docs/build/.doctrees/read_token.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/.doctrees/receiver_category.doctree` & `eurepoc-0.1.5/docs/build/.doctrees/receiver_category.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/.doctrees/receiver_country.doctree` & `eurepoc-0.1.5/docs/build/.doctrees/receiver_country.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/.doctrees/receiver_region.doctree` & `eurepoc-0.1.5/docs/build/.doctrees/receiver_region.doctree`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/DatabaseQuery.html` & `eurepoc-0.1.5/docs/build/DatabaseQuery.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/IncidentDataFrameGenerator.html` & `eurepoc-0.1.5/docs/build/IncidentDataFrameGenerator.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_modules/eurepoc/database_query.html` & `eurepoc-0.1.5/docs/build/_modules/eurepoc/database_query.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_modules/eurepoc/incident_dataframes.html` & `eurepoc-0.1.5/docs/build/_modules/eurepoc/incident_dataframes.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_modules/eurepoc/read_token.html` & `eurepoc-0.1.5/docs/build/_modules/eurepoc/read_token.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_modules/index.html` & `eurepoc-0.1.5/docs/build/_modules/index.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_sources/DatabaseQuery.rst.txt` & `eurepoc-0.1.5/docs/build/_sources/DatabaseQuery.rst.txt`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_sources/date_type.rst.txt` & `eurepoc-0.1.5/docs/build/_sources/date_type.rst.txt`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_sources/index.rst.txt` & `eurepoc-0.1.5/docs/build/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_sources/initiator_country.rst.txt` & `eurepoc-0.1.5/docs/build/_sources/initiator_country.rst.txt`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_sources/receiver_category.rst.txt` & `eurepoc-0.1.5/docs/build/_sources/receiver_category.rst.txt`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_sources/receiver_country.rst.txt` & `eurepoc-0.1.5/docs/build/_sources/receiver_country.rst.txt`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_sources/receiver_region.rst.txt` & `eurepoc-0.1.5/docs/build/_sources/receiver_region.rst.txt`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/basic.css` & `eurepoc-0.1.5/docs/build/_static/basic.css`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/classic.css` & `eurepoc-0.1.5/docs/build/_static/classic.css`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/copybutton.js` & `eurepoc-0.1.5/docs/build/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/doctools.js` & `eurepoc-0.1.5/docs/build/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/language_data.js` & `eurepoc-0.1.5/docs/build/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/menu.js` & `eurepoc-0.1.5/docs/build/_static/menu.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/py.png` & `eurepoc-0.1.5/docs/build/_static/py.png`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/py.svg` & `eurepoc-0.1.5/docs/build/_static/py.svg`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/pydoctheme.css` & `eurepoc-0.1.5/docs/build/_static/pydoctheme.css`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/pydoctheme_dark.css` & `eurepoc-0.1.5/docs/build/_static/pydoctheme_dark.css`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/pygments.css` & `eurepoc-0.1.5/docs/build/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/pygments_dark.css` & `eurepoc-0.1.5/docs/build/_static/pygments_dark.css`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/search-focus.js` & `eurepoc-0.1.5/docs/build/_static/search-focus.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/searchtools.js` & `eurepoc-0.1.5/docs/build/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/sidebar.js` & `eurepoc-0.1.5/docs/build/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/sphinx_highlight.js` & `eurepoc-0.1.5/docs/build/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/_static/themetoggle.js` & `eurepoc-0.1.5/docs/build/_static/themetoggle.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/date_type.html` & `eurepoc-0.1.5/docs/build/date_type.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/flag_type.html` & `eurepoc-0.1.5/docs/build/flag_type.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/genindex.html` & `eurepoc-0.1.5/docs/build/genindex.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/index.html` & `eurepoc-0.1.5/docs/build/index.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/initiator_country.html` & `eurepoc-0.1.5/docs/build/initiator_country.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/objects.inv` & `eurepoc-0.1.5/docs/build/objects.inv`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/py-modindex.html` & `eurepoc-0.1.5/docs/build/py-modindex.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/read_token.html` & `eurepoc-0.1.5/docs/build/read_token.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/receiver_category.html` & `eurepoc-0.1.5/docs/build/receiver_category.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/receiver_country.html` & `eurepoc-0.1.5/docs/build/receiver_country.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/receiver_region.html` & `eurepoc-0.1.5/docs/build/receiver_region.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/search.html` & `eurepoc-0.1.5/docs/build/search.html`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/build/searchindex.js` & `eurepoc-0.1.5/docs/build/searchindex.js`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/make.bat` & `eurepoc-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/source/DatabaseQuery.rst` & `eurepoc-0.1.5/docs/source/DatabaseQuery.rst`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/source/conf.py` & `eurepoc-0.1.5/docs/source/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 import os
 import sys
+import logging
 
 # Add the project root directory to the PYTHONPATH
 sys.path.insert(0, os.path.abspath('../..'))
 
 # Verify the added path (optional for debugging)
 print("Project root added to PYTHONPATH:", os.path.abspath('../..'))
 
+logging.basicConfig(level=logging.DEBUG)
+logger = logging.getLogger(__name__)
+logger.debug("Debugging enabled for Sphinx")
+
+
 # Project information
 project = 'EuRepoC'
 author = 'Camille Borrett'
 release = '0.1.2'
 
 # General configuration
 extensions = [
```

### Comparing `eurepoc-0.1.4/docs/source/date_type.rst` & `eurepoc-0.1.5/docs/source/date_type.rst`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/source/index.rst` & `eurepoc-0.1.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/source/initiator_country.rst` & `eurepoc-0.1.5/docs/source/initiator_country.rst`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/source/receiver_category.rst` & `eurepoc-0.1.5/docs/source/receiver_category.rst`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/source/receiver_country.rst` & `eurepoc-0.1.5/docs/source/receiver_country.rst`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/docs/source/receiver_region.rst` & `eurepoc-0.1.5/docs/source/receiver_region.rst`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/eurepoc/data_cleaning_utils.py` & `eurepoc-0.1.5/eurepoc/data_cleaning_utils.py`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/eurepoc/data_query_utils.py` & `eurepoc-0.1.5/eurepoc/data_query_utils.py`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/eurepoc/database_query.py` & `eurepoc-0.1.5/eurepoc/database_query.py`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/eurepoc/incident_dataframes.py` & `eurepoc-0.1.5/eurepoc/incident_dataframes.py`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/eurepoc/read_token.py` & `eurepoc-0.1.5/eurepoc/read_token.py`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/eurepoc/table_models.py` & `eurepoc-0.1.5/eurepoc/table_models.py`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/eurepoc/tables.py` & `eurepoc-0.1.5/eurepoc/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,24 +284,36 @@
 
 
 def process_initiators_data(full_data):
     initiators_data = []
     for incident in full_data:
         for i in range(len(incident["attributions"])):
             if isinstance(incident["attributions"][i], dict):
-                initiators_data.append(
-                    Initiators(
-                        initiator_id="init_" + str(incident["id"]) + "_" + str(i),
-                        incident_id=int(incident["id"]),
-                        attribution_id=str(incident["attributions"][i]['attribution_id']),
-                        settled_initiator=incident["attributions"][i]['settled'],
-                        initiator_name=incident["attributions"][i]['attributed_initiator_name'][0],
-                        initiator_country=incident["attributions"][i]['attributed_initiator_country'][0],
+                names_length = len(incident["attributions"][i].get('attributed_initiator_name', []))
+                countries_length = len(incident["attributions"][i].get('attributed_initiator_country', []))
+                max_length = max(names_length, countries_length)
+                for j in range(max_length):
+                    if j < names_length:
+                        initiator_name = incident["attributions"][i]['attributed_initiator_name'][j]
+                    else:
+                        initiator_name = "Not available"
+                    if j < countries_length:
+                        initiator_country = incident["attributions"][i]['attributed_initiator_country'][j]
+                    else:
+                        initiator_country = "Not available"
+                    initiators_data.append(
+                        Initiators(
+                            initiator_id="init_" + str(incident["id"]) + "_" + str(j),
+                            incident_id=int(incident["id"]),
+                            attribution_id=str(incident["attributions"][i]['attribution_id']),
+                            settled_initiator=incident["attributions"][i]['settled'],
+                            initiator_name=initiator_name,
+                            initiator_country=initiator_country
+                        )
                     )
-                )
             else:
                 initiators_data.append(
                     Initiators(
                         initiator_id="init_" + str(incident["id"]) + "_" + str(i),
                         incident_id=int(incident["id"]),
                         attribution_id=str(incident["id"]) + "_attr",
                         settled_initiator=None,
@@ -313,22 +325,32 @@
 
 
 def process_initiators_categories_data(full_data):
     initiators_categories_data = []
     for incident in full_data:
         for i in range(len(incident["attributions"])):
             if isinstance(incident["attributions"][i], dict):
-                for j in range(len(incident["attributions"][i]['attributed_initiator_category'])):
-                    initiators_categories_data.append(
-                        InitiatorsCategories(
-                            initiator_id="init_" + str(incident["id"]) + "_" + str(i),
-                            initiator_category=incident["attributions"][i]['attributed_initiator_category'][j],
-                            initiator_subcategory=incident["attributions"][i]['attributed_initiator_category_subcode'][j]
+                if len(incident["attributions"][i]['attributed_initiator_category']) > len(incident["attributions"][i]['attributed_initiator_name']):
+                    for y in range(len(incident["attributions"][i]['attributed_initiator_category'])):
+                        initiators_categories_data.append(
+                            InitiatorsCategories(
+                                initiator_id="init_" + str(incident["id"]) + "_" + str(y),
+                                initiator_category=incident["attributions"][i]['attributed_initiator_category'][y],
+                                initiator_subcategory=incident["attributions"][i]['attributed_initiator_category_subcode'][y]
+                            )
+                        )
+                else:
+                    for y in range(len(incident["attributions"][i]['attributed_initiator_name'])):
+                        initiators_categories_data.append(
+                            InitiatorsCategories(
+                                initiator_id="init_" + str(incident["id"]) + "_" + str(y),
+                                initiator_category=incident["attributions"][i]['attributed_initiator_category'][y],
+                                initiator_subcategory=incident["attributions"][i]['attributed_initiator_category_subcode'][y]
+                            )
                         )
-                    )
             else:
                 initiators_categories_data.append(
                     InitiatorsCategories(
                         initiator_id="init_" + str(incident["id"]) + "_" + str(i),
                         initiator_category=None,
                         initiator_subcategory=None
                     )
```

### Comparing `eurepoc-0.1.4/eurepoc.egg-info/PKG-INFO` & `eurepoc-0.1.5/eurepoc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eurepoc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Wrapper for the EuRepoC API
 Author: Camille Borrett
 License: MIT
 Project-URL: Documentation, https://eurepoc.readthedocs.io/
 Project-URL: Source, https://github.com/camilleborrett/eurepoc
 Project-URL: Tracker, https://github.com/camilleborrett/eurepoc/issues
 Project-URL: EuRepoC Project, https://eurepoc.eu/
```

### Comparing `eurepoc-0.1.4/eurepoc.egg-info/SOURCES.txt` & `eurepoc-0.1.5/eurepoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eurepoc-0.1.4/setup.py` & `eurepoc-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurepoc',
-    version='0.1.4',
+    version='0.1.5',
     author='Camille Borrett',
     description='Wrapper for the EuRepoC API',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     project_urls={
         'Documentation': 'https://eurepoc.readthedocs.io/',
         'Source': 'https://github.com/camilleborrett/eurepoc',
```

