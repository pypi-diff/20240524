# Comparing `tmp/ooresults-0.2.8.tar.gz` & `tmp/ooresults-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooresults-0.2.8.tar", last modified: Fri Jan  5 17:17:39 2024, max compression
+gzip compressed data, was "ooresults-0.2.9.tar", last modified: Tue Feb 13 11:44:49 2024, max compression
```

## Comparing `ooresults-0.2.8.tar` & `ooresults-0.2.9.tar`

### file list

```diff
@@ -1,181 +1,187 @@
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.319736 ooresults-0.2.8/
--rw-r--r--   0 rainer    (1000) users      (100)    34523 2023-03-01 18:09:04.000000 ooresults-0.2.8/LICENSE
--rw-r--r--   0 rainer    (1000) users      (100)      260 2023-03-01 18:09:04.000000 ooresults-0.2.8/MANIFEST.in
--rw-r--r--   0 rainer    (1000) users      (100)    43344 2024-01-05 17:17:39.319736 ooresults-0.2.8/PKG-INFO
--rw-r--r--   0 rainer    (1000) users      (100)     2278 2023-03-01 18:09:04.000000 ooresults-0.2.8/README.rst
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.287736 ooresults-0.2.8/ooresults/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)    15992 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/_reader.py
--rw-r--r--   0 rainer    (1000) users      (100)    11491 2023-12-26 10:38:40.000000 ooresults-0.2.8/ooresults/_server.py
--rw-r--r--   0 rainer    (1000) users      (100)     4363 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/configuration.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.291736 ooresults-0.2.8/ooresults/handler/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/handler/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     9424 2023-12-26 10:38:40.000000 ooresults-0.2.8/ooresults/handler/build_results.py
--rw-r--r--   0 rainer    (1000) users      (100)     7573 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/handler/classes.py
--rw-r--r--   0 rainer    (1000) users      (100)     2710 2023-09-11 17:41:10.000000 ooresults-0.2.8/ooresults/handler/clubs.py
--rw-r--r--   0 rainer    (1000) users      (100)     4259 2023-12-29 10:46:54.000000 ooresults-0.2.8/ooresults/handler/competitors.py
--rw-r--r--   0 rainer    (1000) users      (100)     5527 2023-08-22 18:32:58.000000 ooresults-0.2.8/ooresults/handler/courses.py
--rw-r--r--   0 rainer    (1000) users      (100)     1110 2023-04-23 07:29:14.000000 ooresults-0.2.8/ooresults/handler/demo_reader.py
--rw-r--r--   0 rainer    (1000) users      (100)    11612 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/handler/entries.py
--rw-r--r--   0 rainer    (1000) users      (100)     3253 2023-08-22 18:32:58.000000 ooresults-0.2.8/ooresults/handler/events.py
--rw-r--r--   0 rainer    (1000) users      (100)     4504 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/handler/handicap.py
--rw-r--r--   0 rainer    (1000) users      (100)    32689 2023-12-31 14:40:12.000000 ooresults-0.2.8/ooresults/handler/model.py
--rw-r--r--   0 rainer    (1000) users      (100)     3888 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/handler/results.py
--rw-r--r--   0 rainer    (1000) users      (100)     5021 2023-12-26 10:38:40.000000 ooresults-0.2.8/ooresults/handler/series.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.291736 ooresults-0.2.8/ooresults/pdf/
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.295736 ooresults-0.2.8/ooresults/pdf/fonts/
--rw-r--r--   0 rainer    (1000) users      (100)   690516 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/pdf/fonts/Carlito-Bold.ttf
--rw-r--r--   0 rainer    (1000) users      (100)   816716 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/pdf/fonts/Carlito-BoldItalic.ttf
--rw-r--r--   0 rainer    (1000) users      (100)   623416 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/pdf/fonts/Carlito-Italic.ttf
--rw-r--r--   0 rainer    (1000) users      (100)   635996 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/pdf/fonts/Carlito-Regular.ttf
--rw-r--r--   0 rainer    (1000) users      (100)     3706 2023-10-04 17:38:38.000000 ooresults-0.2.8/ooresults/pdf/pdf.py
--rw-r--r--   0 rainer    (1000) users      (100)    11061 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/pdf/result.py
--rw-r--r--   0 rainer    (1000) users      (100)     5552 2023-12-26 10:38:40.000000 ooresults-0.2.8/ooresults/pdf/series.py
--rw-r--r--   0 rainer    (1000) users      (100)    11350 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/pdf/splittimes.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.295736 ooresults-0.2.8/ooresults/plugins/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/plugins/__init__.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.283736 ooresults-0.2.8/ooresults/plugins/imports/
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.299736 ooresults-0.2.8/ooresults/plugins/imports/entries/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/plugins/imports/entries/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     2948 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/plugins/imports/entries/text.py
--rw-r--r--   0 rainer    (1000) users      (100)     2807 2023-10-04 17:38:38.000000 ooresults-0.2.8/ooresults/plugins/iof_class_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     4091 2023-09-25 15:59:56.000000 ooresults-0.2.8/ooresults/plugins/iof_competitor_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     5991 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/plugins/iof_course_data.py
--rw-r--r--   0 rainer    (1000) users      (100)     5105 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/plugins/iof_entry_list.py
--rw-r--r--   0 rainer    (1000) users      (100)    11062 2023-12-31 14:40:12.000000 ooresults-0.2.8/ooresults/plugins/iof_result_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     7352 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/plugins/oe12.py
--rw-r--r--   0 rainer    (1000) users      (100)    14486 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/plugins/oe2003.py
--rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/reader.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.299736 ooresults-0.2.8/ooresults/repo/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/repo/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     1944 2023-10-04 17:38:38.000000 ooresults-0.2.8/ooresults/repo/class_params.py
--rw-r--r--   0 rainer    (1000) users      (100)     1363 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/repo/class_type.py
--rw-r--r--   0 rainer    (1000) users      (100)      891 2023-09-11 17:41:10.000000 ooresults-0.2.8/ooresults/repo/club_type.py
--rw-r--r--   0 rainer    (1000) users      (100)     1080 2023-09-25 15:59:56.000000 ooresults-0.2.8/ooresults/repo/competitor_type.py
--rw-r--r--   0 rainer    (1000) users      (100)     1098 2023-08-22 18:32:58.000000 ooresults-0.2.8/ooresults/repo/course_type.py
--rw-r--r--   0 rainer    (1000) users      (100)     1810 2024-01-05 17:15:47.000000 ooresults-0.2.8/ooresults/repo/entry_type.py
--rw-r--r--   0 rainer    (1000) users      (100)     1087 2023-08-22 18:32:58.000000 ooresults-0.2.8/ooresults/repo/event_type.py
--rw-r--r--   0 rainer    (1000) users      (100)     7412 2023-08-22 18:32:58.000000 ooresults-0.2.8/ooresults/repo/repo.py
--rw-r--r--   0 rainer    (1000) users      (100)    16334 2023-10-17 16:33:01.000000 ooresults-0.2.8/ooresults/repo/result_type.py
--rw-r--r--   0 rainer    (1000) users      (100)     1403 2023-12-26 10:38:40.000000 ooresults-0.2.8/ooresults/repo/series_type.py
--rw-r--r--   0 rainer    (1000) users      (100)    42806 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/repo/sqlite_repo.py
--rw-r--r--   0 rainer    (1000) users      (100)      972 2023-10-17 16:33:01.000000 ooresults-0.2.8/ooresults/repo/start_type.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.299736 ooresults-0.2.8/ooresults/repo/update/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/repo/update/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     4728 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/repo/update/update_008.py
--rw-r--r--   0 rainer    (1000) users      (100)     1549 2023-09-25 15:59:56.000000 ooresults-0.2.8/ooresults/repo/update/update_008a.py
--rw-r--r--   0 rainer    (1000) users      (100)     1975 2023-09-25 15:59:56.000000 ooresults-0.2.8/ooresults/repo/update/update_tables.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.303736 ooresults-0.2.8/ooresults/schema/
--rw-r--r--   0 rainer    (1000) users      (100)   177863 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/schema/IOF.xsd
--rwxr-xr-x   0 rainer    (1000) users      (100)     2117 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/schema/cardreader_log.json
--rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/server.py
--rw-r--r--   0 rainer    (1000) users      (100)     2257 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/set_legacy_mode.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.303736 ooresults-0.2.8/ooresults/static/
--rw-r--r--   0 rainer    (1000) users      (100)      643 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/static/style-tab.css
--rw-r--r--   0 rainer    (1000) users      (100)     1267 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/static/style.css
--rw-r--r--   0 rainer    (1000) users      (100)    12106 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/static/w3.js
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.307736 ooresults-0.2.8/ooresults/templates/
--rw-r--r--   0 rainer    (1000) users      (100)     6102 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/templates/add_class.html
--rw-r--r--   0 rainer    (1000) users      (100)      969 2023-09-11 17:41:10.000000 ooresults-0.2.8/ooresults/templates/add_club.html
--rw-r--r--   0 rainer    (1000) users      (100)     3568 2023-12-29 10:46:54.000000 ooresults-0.2.8/ooresults/templates/add_competitor.html
--rw-r--r--   0 rainer    (1000) users      (100)     2006 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/templates/add_course.html
--rw-r--r--   0 rainer    (1000) users      (100)     7107 2023-12-29 10:46:54.000000 ooresults-0.2.8/ooresults/templates/add_entry.html
--rw-r--r--   0 rainer    (1000) users      (100)     1811 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/templates/add_entry_competitors.html
--rw-r--r--   0 rainer    (1000) users      (100)     7197 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/templates/add_entry_result.html
--rw-r--r--   0 rainer    (1000) users      (100)     2600 2023-08-22 18:32:58.000000 ooresults-0.2.8/ooresults/templates/add_event.html
--rw-r--r--   0 rainer    (1000) users      (100)      466 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/templates/base.html
--rw-r--r--   0 rainer    (1000) users      (100)    12298 2023-12-28 11:05:24.000000 ooresults-0.2.8/ooresults/templates/classes_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     2917 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/templates/classes_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     7144 2023-12-28 11:05:24.000000 ooresults-0.2.8/ooresults/templates/clubs_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)      453 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/templates/clubs_table.html
--rwxr-xr-x   0 rainer    (1000) users      (100)    12166 2023-12-28 11:05:24.000000 ooresults-0.2.8/ooresults/templates/competitors_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1093 2023-09-25 15:59:56.000000 ooresults-0.2.8/ooresults/templates/competitors_table.html
--rw-r--r--   0 rainer    (1000) users      (100)    12312 2023-12-28 11:05:24.000000 ooresults-0.2.8/ooresults/templates/courses_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1388 2023-08-22 18:32:58.000000 ooresults-0.2.8/ooresults/templates/courses_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     6529 2023-04-23 07:11:17.000000 ooresults-0.2.8/ooresults/templates/demo_reader.html
--rwxr-xr-x   0 rainer    (1000) users      (100)    19708 2023-12-28 11:05:24.000000 ooresults-0.2.8/ooresults/templates/entries_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     2816 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/templates/entries_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     9731 2023-12-28 11:05:24.000000 ooresults-0.2.8/ooresults/templates/events_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/templates/events_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     5943 2023-08-22 18:32:58.000000 ooresults-0.2.8/ooresults/templates/main.html
--rw-r--r--   0 rainer    (1000) users      (100)     5711 2023-12-28 11:05:24.000000 ooresults-0.2.8/ooresults/templates/results_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     5379 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/templates/results_table.html
--rw-r--r--   0 rainer    (1000) users      (100)      528 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/templates/root.html
--rw-r--r--   0 rainer    (1000) users      (100)     1084 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/templates/select_event.html
--rw-r--r--   0 rainer    (1000) users      (100)     2498 2023-12-29 10:46:54.000000 ooresults-0.2.8/ooresults/templates/series_settings.html
--rw-r--r--   0 rainer    (1000) users      (100)     7523 2023-12-28 11:05:24.000000 ooresults-0.2.8/ooresults/templates/series_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1654 2023-12-26 10:38:40.000000 ooresults-0.2.8/ooresults/templates/series_table.html
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.307736 ooresults-0.2.8/ooresults/templates/si/
--rw-r--r--   0 rainer    (1000) users      (100)      902 2023-04-23 07:29:14.000000 ooresults-0.2.8/ooresults/templates/si/si1_data.html
--rw-r--r--   0 rainer    (1000) users      (100)      396 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/templates/si/si1_error.html
--rw-r--r--   0 rainer    (1000) users      (100)     6992 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/templates/si/si1_page.html
--rw-r--r--   0 rainer    (1000) users      (100)     4105 2023-08-22 18:32:58.000000 ooresults-0.2.8/ooresults/templates/si/si2_data.html
--rw-r--r--   0 rainer    (1000) users      (100)     3589 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/templates/si/si2_page.html
--rw-r--r--   0 rainer    (1000) users      (100)      383 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/templates/unauthorized.html
--rw-r--r--   0 rainer    (1000) users      (100)     2407 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/user.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.311736 ooresults-0.2.8/ooresults/utils/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/utils/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     2025 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/utils/globals.py
--rw-r--r--   0 rainer    (1000) users      (100)     1411 2023-07-17 16:30:29.000000 ooresults-0.2.8/ooresults/utils/rental_cards.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.311736 ooresults-0.2.8/ooresults/websocket_server/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/websocket_server/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     1719 2023-11-26 23:16:20.000000 ooresults-0.2.8/ooresults/websocket_server/si.py
--rw-r--r--   0 rainer    (1000) users      (100)    14645 2023-10-16 16:51:43.000000 ooresults-0.2.8/ooresults/websocket_server/websocket_handler.py
--rw-r--r--   0 rainer    (1000) users      (100)     2143 2023-03-01 18:09:04.000000 ooresults-0.2.8/ooresults/websocket_server/websocket_server.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.319736 ooresults-0.2.8/ooresults.egg-info/
--rw-r--r--   0 rainer    (1000) users      (100)    43344 2024-01-05 17:17:39.000000 ooresults-0.2.8/ooresults.egg-info/PKG-INFO
--rw-r--r--   0 rainer    (1000) users      (100)     5190 2024-01-05 17:17:39.000000 ooresults-0.2.8/ooresults.egg-info/SOURCES.txt
--rw-r--r--   0 rainer    (1000) users      (100)        1 2024-01-05 17:17:39.000000 ooresults-0.2.8/ooresults.egg-info/dependency_links.txt
--rw-r--r--   0 rainer    (1000) users      (100)      102 2024-01-05 17:17:39.000000 ooresults-0.2.8/ooresults.egg-info/entry_points.txt
--rw-r--r--   0 rainer    (1000) users      (100)      152 2024-01-05 17:17:39.000000 ooresults-0.2.8/ooresults.egg-info/requires.txt
--rw-r--r--   0 rainer    (1000) users      (100)       10 2024-01-05 17:17:39.000000 ooresults-0.2.8/ooresults.egg-info/top_level.txt
--rwxr-xr-x   0 rainer    (1000) users      (100)     1772 2024-01-05 17:15:47.000000 ooresults-0.2.8/pyproject.toml
--rw-r--r--   0 rainer    (1000) users      (100)       38 2024-01-05 17:17:39.319736 ooresults-0.2.8/setup.cfg
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.311736 ooresults-0.2.8/tests/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.8/tests/__init__.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.315736 ooresults-0.2.8/tests/model/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.8/tests/model/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     8827 2023-12-26 10:38:40.000000 ooresults-0.2.8/tests/model/test_build_series_result.py
--rw-r--r--   0 rainer    (1000) users      (100)     8896 2023-11-26 23:16:20.000000 ooresults-0.2.8/tests/model/test_classes.py
--rw-r--r--   0 rainer    (1000) users      (100)    15079 2023-11-26 23:16:20.000000 ooresults-0.2.8/tests/model/test_courses.py
--rw-r--r--   0 rainer    (1000) users      (100)     7752 2023-11-26 23:16:20.000000 ooresults-0.2.8/tests/model/test_event_class_results.py
--rw-r--r--   0 rainer    (1000) users      (100)    17315 2023-10-16 16:51:43.000000 ooresults-0.2.8/tests/model/test_parse_cardreader_log.py
--rw-r--r--   0 rainer    (1000) users      (100)    32198 2023-11-26 23:16:20.000000 ooresults-0.2.8/tests/model/test_store_cardreader_result.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.315736 ooresults-0.2.8/tests/plugins/
--rw-r--r--   0 rainer    (1000) users      (100)    23172 2023-11-26 23:16:20.000000 ooresults-0.2.8/tests/plugins/test_export_competitors_oe12.py
--rw-r--r--   0 rainer    (1000) users      (100)    20280 2023-11-26 23:16:20.000000 ooresults-0.2.8/tests/plugins/test_export_competitors_oe2003.py
--rw-r--r--   0 rainer    (1000) users      (100)    29297 2023-04-23 07:29:14.000000 ooresults-0.2.8/tests/plugins/test_import_competitors_oe2003.py
--rw-r--r--   0 rainer    (1000) users      (100)     3886 2023-11-26 23:16:20.000000 ooresults-0.2.8/tests/plugins/test_plugin_iof_class_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     4289 2023-10-04 17:38:38.000000 ooresults-0.2.8/tests/plugins/test_plugin_iof_competitor_list.py
--rw-r--r--   0 rainer    (1000) users      (100)    11600 2023-11-26 23:16:20.000000 ooresults-0.2.8/tests/plugins/test_plugin_iof_course_data.py
--rw-r--r--   0 rainer    (1000) users      (100)     9683 2023-11-26 23:16:20.000000 ooresults-0.2.8/tests/plugins/test_plugin_iof_entry_list.py
--rw-r--r--   0 rainer    (1000) users      (100)    38969 2023-12-31 14:40:12.000000 ooresults-0.2.8/tests/plugins/test_plugin_iof_result_list.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.319736 ooresults-0.2.8/tests/repo/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.8/tests/repo/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)    11441 2023-11-26 23:16:20.000000 ooresults-0.2.8/tests/repo/test_classes.py
--rw-r--r--   0 rainer    (1000) users      (100)     5177 2023-09-11 17:41:10.000000 ooresults-0.2.8/tests/repo/test_clubs.py
--rw-r--r--   0 rainer    (1000) users      (100)    15015 2023-09-25 15:59:56.000000 ooresults-0.2.8/tests/repo/test_competitors.py
--rw-r--r--   0 rainer    (1000) users      (100)     7481 2023-11-26 23:16:20.000000 ooresults-0.2.8/tests/repo/test_courses.py
--rw-r--r--   0 rainer    (1000) users      (100)    35875 2023-11-26 23:16:20.000000 ooresults-0.2.8/tests/repo/test_entries.py
--rw-r--r--   0 rainer    (1000) users      (100)     7821 2023-08-22 18:32:58.000000 ooresults-0.2.8/tests/repo/test_events.py
--rw-r--r--   0 rainer    (1000) users      (100)     2353 2023-03-01 18:09:04.000000 ooresults-0.2.8/tests/repo/test_settings.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-01-05 17:17:39.319736 ooresults-0.2.8/tests/templates/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-12-29 10:46:54.000000 ooresults-0.2.8/tests/templates/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     7839 2023-12-29 10:46:54.000000 ooresults-0.2.8/tests/templates/test_add_class.py
--rw-r--r--   0 rainer    (1000) users      (100)     1808 2023-12-29 10:46:54.000000 ooresults-0.2.8/tests/templates/test_add_club.py
--rw-r--r--   0 rainer    (1000) users      (100)     4580 2023-12-29 10:46:54.000000 ooresults-0.2.8/tests/templates/test_add_competitor.py
--rw-r--r--   0 rainer    (1000) users      (100)     2555 2023-12-29 10:46:54.000000 ooresults-0.2.8/tests/templates/test_add_course.py
--rw-r--r--   0 rainer    (1000) users      (100)    19545 2023-12-29 10:46:54.000000 ooresults-0.2.8/tests/templates/test_add_entry.py
--rw-r--r--   0 rainer    (1000) users      (100)     2828 2023-12-29 10:46:54.000000 ooresults-0.2.8/tests/templates/test_add_entry_competitors.py
--rw-r--r--   0 rainer    (1000) users      (100)     3372 2023-12-29 10:46:54.000000 ooresults-0.2.8/tests/templates/test_add_event.py
--rw-r--r--   0 rainer    (1000) users      (100)     3192 2023-12-29 10:46:54.000000 ooresults-0.2.8/tests/templates/test_series_settings.py
--rw-r--r--   0 rainer    (1000) users      (100)     9467 2023-03-01 18:09:04.000000 ooresults-0.2.8/tests/test_compute_result_net.py
--rw-r--r--   0 rainer    (1000) users      (100)    15440 2023-03-01 18:09:04.000000 ooresults-0.2.8/tests/test_compute_result_score.py
--rw-r--r--   0 rainer    (1000) users      (100)    38250 2023-04-23 07:29:14.000000 ooresults-0.2.8/tests/test_compute_result_standard.py
--rw-r--r--   0 rainer    (1000) users      (100)     7257 2023-03-01 18:09:04.000000 ooresults-0.2.8/tests/test_configuration.py
--rw-r--r--   0 rainer    (1000) users      (100)     1973 2023-04-23 07:29:14.000000 ooresults-0.2.8/tests/test_globals.py
--rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.8/tests/test_handicap.py
--rw-r--r--   0 rainer    (1000) users      (100)    20521 2023-11-26 23:16:20.000000 ooresults-0.2.8/tests/test_ranking.py
--rw-r--r--   0 rainer    (1000) users      (100)     3671 2023-07-17 16:30:29.000000 ooresults-0.2.8/tests/test_rental_cards.py
--rw-r--r--   0 rainer    (1000) users      (100)    40600 2023-12-26 10:38:40.000000 ooresults-0.2.8/tests/test_series.py
--rw-r--r--   0 rainer    (1000) users      (100)     2326 2023-03-01 18:09:04.000000 ooresults-0.2.8/tests/test_user.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.299342 ooresults-0.2.9/
+-rw-r--r--   0 rainer    (1000) users      (100)    34523 2023-03-01 18:09:04.000000 ooresults-0.2.9/LICENSE
+-rw-r--r--   0 rainer    (1000) users      (100)      260 2023-03-01 18:09:04.000000 ooresults-0.2.9/MANIFEST.in
+-rw-r--r--   0 rainer    (1000) users      (100)    43391 2024-02-13 11:44:49.299342 ooresults-0.2.9/PKG-INFO
+-rw-r--r--   0 rainer    (1000) users      (100)     2278 2023-03-01 18:09:04.000000 ooresults-0.2.9/README.rst
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.259342 ooresults-0.2.9/ooresults/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)    15992 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/_reader.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11491 2023-12-26 10:38:40.000000 ooresults-0.2.9/ooresults/_server.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4363 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/configuration.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.267342 ooresults-0.2.9/ooresults/handler/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/handler/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     9424 2023-12-26 10:38:40.000000 ooresults-0.2.9/ooresults/handler/build_results.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7573 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/handler/classes.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2710 2023-09-11 17:41:10.000000 ooresults-0.2.9/ooresults/handler/clubs.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4259 2023-12-29 10:46:54.000000 ooresults-0.2.9/ooresults/handler/competitors.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5527 2023-08-22 18:32:58.000000 ooresults-0.2.9/ooresults/handler/courses.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1110 2023-04-23 07:29:14.000000 ooresults-0.2.9/ooresults/handler/demo_reader.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11612 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/handler/entries.py
+-rw-r--r--   0 rainer    (1000) users      (100)     3253 2023-08-22 18:32:58.000000 ooresults-0.2.9/ooresults/handler/events.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4504 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/handler/handicap.py
+-rw-r--r--   0 rainer    (1000) users      (100)    32689 2023-12-31 14:40:12.000000 ooresults-0.2.9/ooresults/handler/model.py
+-rw-r--r--   0 rainer    (1000) users      (100)     3888 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/handler/results.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5021 2023-12-26 10:38:40.000000 ooresults-0.2.9/ooresults/handler/series.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.267342 ooresults-0.2.9/ooresults/pdf/
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.271342 ooresults-0.2.9/ooresults/pdf/fonts/
+-rw-r--r--   0 rainer    (1000) users      (100)   690516 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/pdf/fonts/Carlito-Bold.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)   816716 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/pdf/fonts/Carlito-BoldItalic.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)   623416 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/pdf/fonts/Carlito-Italic.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)   635996 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/pdf/fonts/Carlito-Regular.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)     3669 2024-02-13 11:39:54.000000 ooresults-0.2.9/ooresults/pdf/pdf.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11060 2024-02-13 11:39:54.000000 ooresults-0.2.9/ooresults/pdf/result.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5552 2023-12-26 10:38:40.000000 ooresults-0.2.9/ooresults/pdf/series.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11349 2024-02-13 11:39:54.000000 ooresults-0.2.9/ooresults/pdf/splittimes.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.271342 ooresults-0.2.9/ooresults/plugins/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/plugins/__init__.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.255342 ooresults-0.2.9/ooresults/plugins/imports/
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.275342 ooresults-0.2.9/ooresults/plugins/imports/entries/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/plugins/imports/entries/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2948 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/plugins/imports/entries/text.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2807 2023-10-04 17:38:38.000000 ooresults-0.2.9/ooresults/plugins/iof_class_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4091 2023-09-25 15:59:56.000000 ooresults-0.2.9/ooresults/plugins/iof_competitor_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5991 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/plugins/iof_course_data.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5105 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/plugins/iof_entry_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11062 2023-12-31 14:40:12.000000 ooresults-0.2.9/ooresults/plugins/iof_result_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7352 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/plugins/oe12.py
+-rw-r--r--   0 rainer    (1000) users      (100)    14486 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/plugins/oe2003.py
+-rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/reader.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.275342 ooresults-0.2.9/ooresults/repo/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/repo/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1944 2023-10-04 17:38:38.000000 ooresults-0.2.9/ooresults/repo/class_params.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1363 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/repo/class_type.py
+-rw-r--r--   0 rainer    (1000) users      (100)      891 2023-09-11 17:41:10.000000 ooresults-0.2.9/ooresults/repo/club_type.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1080 2023-09-25 15:59:56.000000 ooresults-0.2.9/ooresults/repo/competitor_type.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1098 2023-08-22 18:32:58.000000 ooresults-0.2.9/ooresults/repo/course_type.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1810 2024-01-05 17:15:47.000000 ooresults-0.2.9/ooresults/repo/entry_type.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1087 2023-08-22 18:32:58.000000 ooresults-0.2.9/ooresults/repo/event_type.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7412 2023-08-22 18:32:58.000000 ooresults-0.2.9/ooresults/repo/repo.py
+-rw-r--r--   0 rainer    (1000) users      (100)    16334 2023-10-17 16:33:01.000000 ooresults-0.2.9/ooresults/repo/result_type.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1403 2023-12-26 10:38:40.000000 ooresults-0.2.9/ooresults/repo/series_type.py
+-rw-r--r--   0 rainer    (1000) users      (100)    42806 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/repo/sqlite_repo.py
+-rw-r--r--   0 rainer    (1000) users      (100)      972 2023-10-17 16:33:01.000000 ooresults-0.2.9/ooresults/repo/start_type.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.275342 ooresults-0.2.9/ooresults/repo/update/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/repo/update/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4728 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/repo/update/update_008.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1549 2023-09-25 15:59:56.000000 ooresults-0.2.9/ooresults/repo/update/update_008a.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1975 2023-09-25 15:59:56.000000 ooresults-0.2.9/ooresults/repo/update/update_tables.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.279342 ooresults-0.2.9/ooresults/schema/
+-rw-r--r--   0 rainer    (1000) users      (100)   177863 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/schema/IOF.xsd
+-rwxr-xr-x   0 rainer    (1000) users      (100)     2117 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/schema/cardreader_log.json
+-rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/server.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2257 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/set_legacy_mode.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.279342 ooresults-0.2.9/ooresults/static/
+-rw-r--r--   0 rainer    (1000) users      (100)      643 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/static/style-tab.css
+-rw-r--r--   0 rainer    (1000) users      (100)     1267 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/static/style.css
+-rw-r--r--   0 rainer    (1000) users      (100)    12106 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/static/w3.js
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.287342 ooresults-0.2.9/ooresults/templates/
+-rw-r--r--   0 rainer    (1000) users      (100)     6102 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/templates/add_class.html
+-rw-r--r--   0 rainer    (1000) users      (100)      969 2023-09-11 17:41:10.000000 ooresults-0.2.9/ooresults/templates/add_club.html
+-rw-r--r--   0 rainer    (1000) users      (100)     3568 2023-12-29 10:46:54.000000 ooresults-0.2.9/ooresults/templates/add_competitor.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2006 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/templates/add_course.html
+-rw-r--r--   0 rainer    (1000) users      (100)     7107 2023-12-29 10:46:54.000000 ooresults-0.2.9/ooresults/templates/add_entry.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1811 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/templates/add_entry_competitors.html
+-rw-r--r--   0 rainer    (1000) users      (100)     7197 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/templates/add_entry_result.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2600 2023-08-22 18:32:58.000000 ooresults-0.2.9/ooresults/templates/add_event.html
+-rw-r--r--   0 rainer    (1000) users      (100)      466 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/templates/base.html
+-rw-r--r--   0 rainer    (1000) users      (100)    12298 2023-12-28 11:05:24.000000 ooresults-0.2.9/ooresults/templates/classes_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2917 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/templates/classes_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     7144 2023-12-28 11:05:24.000000 ooresults-0.2.9/ooresults/templates/clubs_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)      453 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/templates/clubs_table.html
+-rwxr-xr-x   0 rainer    (1000) users      (100)    12166 2023-12-28 11:05:24.000000 ooresults-0.2.9/ooresults/templates/competitors_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1093 2023-09-25 15:59:56.000000 ooresults-0.2.9/ooresults/templates/competitors_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)    12312 2023-12-28 11:05:24.000000 ooresults-0.2.9/ooresults/templates/courses_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1388 2023-08-22 18:32:58.000000 ooresults-0.2.9/ooresults/templates/courses_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6529 2023-04-23 07:11:17.000000 ooresults-0.2.9/ooresults/templates/demo_reader.html
+-rwxr-xr-x   0 rainer    (1000) users      (100)    19708 2023-12-28 11:05:24.000000 ooresults-0.2.9/ooresults/templates/entries_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2816 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/templates/entries_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     9731 2023-12-28 11:05:24.000000 ooresults-0.2.9/ooresults/templates/events_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/templates/events_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     5943 2023-08-22 18:32:58.000000 ooresults-0.2.9/ooresults/templates/main.html
+-rw-r--r--   0 rainer    (1000) users      (100)     5711 2023-12-28 11:05:24.000000 ooresults-0.2.9/ooresults/templates/results_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     5379 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/templates/results_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)      528 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/templates/root.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1084 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/templates/select_event.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2498 2023-12-29 10:46:54.000000 ooresults-0.2.9/ooresults/templates/series_settings.html
+-rw-r--r--   0 rainer    (1000) users      (100)     7523 2023-12-28 11:05:24.000000 ooresults-0.2.9/ooresults/templates/series_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1654 2023-12-26 10:38:40.000000 ooresults-0.2.9/ooresults/templates/series_table.html
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.287342 ooresults-0.2.9/ooresults/templates/si/
+-rw-r--r--   0 rainer    (1000) users      (100)      902 2023-04-23 07:29:14.000000 ooresults-0.2.9/ooresults/templates/si/si1_data.html
+-rw-r--r--   0 rainer    (1000) users      (100)      396 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/templates/si/si1_error.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6992 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/templates/si/si1_page.html
+-rw-r--r--   0 rainer    (1000) users      (100)     4105 2023-08-22 18:32:58.000000 ooresults-0.2.9/ooresults/templates/si/si2_data.html
+-rw-r--r--   0 rainer    (1000) users      (100)     3589 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/templates/si/si2_page.html
+-rw-r--r--   0 rainer    (1000) users      (100)      383 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/templates/unauthorized.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2407 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/user.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.287342 ooresults-0.2.9/ooresults/utils/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/utils/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2025 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/utils/globals.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1411 2023-07-17 16:30:29.000000 ooresults-0.2.9/ooresults/utils/rental_cards.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.287342 ooresults-0.2.9/ooresults/websocket_server/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/websocket_server/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1719 2023-11-26 23:16:20.000000 ooresults-0.2.9/ooresults/websocket_server/si.py
+-rw-r--r--   0 rainer    (1000) users      (100)    14165 2024-02-07 21:11:25.000000 ooresults-0.2.9/ooresults/websocket_server/websocket_handler.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2143 2023-03-01 18:09:04.000000 ooresults-0.2.9/ooresults/websocket_server/websocket_server.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.299342 ooresults-0.2.9/ooresults.egg-info/
+-rw-r--r--   0 rainer    (1000) users      (100)    43391 2024-02-13 11:44:49.000000 ooresults-0.2.9/ooresults.egg-info/PKG-INFO
+-rw-r--r--   0 rainer    (1000) users      (100)     5304 2024-02-13 11:44:49.000000 ooresults-0.2.9/ooresults.egg-info/SOURCES.txt
+-rw-r--r--   0 rainer    (1000) users      (100)        1 2024-02-13 11:44:49.000000 ooresults-0.2.9/ooresults.egg-info/dependency_links.txt
+-rw-r--r--   0 rainer    (1000) users      (100)      102 2024-02-13 11:44:49.000000 ooresults-0.2.9/ooresults.egg-info/entry_points.txt
+-rw-r--r--   0 rainer    (1000) users      (100)      167 2024-02-13 11:44:49.000000 ooresults-0.2.9/ooresults.egg-info/requires.txt
+-rw-r--r--   0 rainer    (1000) users      (100)       10 2024-02-13 11:44:49.000000 ooresults-0.2.9/ooresults.egg-info/top_level.txt
+-rwxr-xr-x   0 rainer    (1000) users      (100)     1794 2024-02-13 11:39:54.000000 ooresults-0.2.9/pyproject.toml
+-rw-r--r--   0 rainer    (1000) users      (100)       38 2024-02-13 11:44:49.299342 ooresults-0.2.9/setup.cfg
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.291342 ooresults-0.2.9/tests/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.9/tests/__init__.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.291342 ooresults-0.2.9/tests/model/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.9/tests/model/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     8827 2023-12-26 10:38:40.000000 ooresults-0.2.9/tests/model/test_build_series_result.py
+-rw-r--r--   0 rainer    (1000) users      (100)     8896 2023-11-26 23:16:20.000000 ooresults-0.2.9/tests/model/test_classes.py
+-rw-r--r--   0 rainer    (1000) users      (100)    15079 2023-11-26 23:16:20.000000 ooresults-0.2.9/tests/model/test_courses.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7752 2023-11-26 23:16:20.000000 ooresults-0.2.9/tests/model/test_event_class_results.py
+-rw-r--r--   0 rainer    (1000) users      (100)    17315 2023-10-16 16:51:43.000000 ooresults-0.2.9/tests/model/test_parse_cardreader_log.py
+-rw-r--r--   0 rainer    (1000) users      (100)    32198 2023-11-26 23:16:20.000000 ooresults-0.2.9/tests/model/test_store_cardreader_result.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.291342 ooresults-0.2.9/tests/pdf/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2024-02-13 11:39:54.000000 ooresults-0.2.9/tests/pdf/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1943 2024-02-13 11:39:54.000000 ooresults-0.2.9/tests/pdf/test_pdf.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.295342 ooresults-0.2.9/tests/plugins/
+-rw-r--r--   0 rainer    (1000) users      (100)    23172 2023-11-26 23:16:20.000000 ooresults-0.2.9/tests/plugins/test_export_competitors_oe12.py
+-rw-r--r--   0 rainer    (1000) users      (100)    20280 2023-11-26 23:16:20.000000 ooresults-0.2.9/tests/plugins/test_export_competitors_oe2003.py
+-rw-r--r--   0 rainer    (1000) users      (100)    29297 2023-04-23 07:29:14.000000 ooresults-0.2.9/tests/plugins/test_import_competitors_oe2003.py
+-rw-r--r--   0 rainer    (1000) users      (100)     3886 2023-11-26 23:16:20.000000 ooresults-0.2.9/tests/plugins/test_plugin_iof_class_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4289 2023-10-04 17:38:38.000000 ooresults-0.2.9/tests/plugins/test_plugin_iof_competitor_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11600 2023-11-26 23:16:20.000000 ooresults-0.2.9/tests/plugins/test_plugin_iof_course_data.py
+-rw-r--r--   0 rainer    (1000) users      (100)     9683 2023-11-26 23:16:20.000000 ooresults-0.2.9/tests/plugins/test_plugin_iof_entry_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)    38969 2023-12-31 14:40:12.000000 ooresults-0.2.9/tests/plugins/test_plugin_iof_result_list.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.295342 ooresults-0.2.9/tests/repo/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.9/tests/repo/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11441 2023-11-26 23:16:20.000000 ooresults-0.2.9/tests/repo/test_classes.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5177 2023-09-11 17:41:10.000000 ooresults-0.2.9/tests/repo/test_clubs.py
+-rw-r--r--   0 rainer    (1000) users      (100)    15015 2023-09-25 15:59:56.000000 ooresults-0.2.9/tests/repo/test_competitors.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7481 2023-11-26 23:16:20.000000 ooresults-0.2.9/tests/repo/test_courses.py
+-rw-r--r--   0 rainer    (1000) users      (100)    35875 2023-11-26 23:16:20.000000 ooresults-0.2.9/tests/repo/test_entries.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7821 2023-08-22 18:32:58.000000 ooresults-0.2.9/tests/repo/test_events.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2353 2023-03-01 18:09:04.000000 ooresults-0.2.9/tests/repo/test_settings.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.299342 ooresults-0.2.9/tests/templates/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-12-29 10:46:54.000000 ooresults-0.2.9/tests/templates/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7839 2023-12-29 10:46:54.000000 ooresults-0.2.9/tests/templates/test_add_class.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1808 2023-12-29 10:46:54.000000 ooresults-0.2.9/tests/templates/test_add_club.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4580 2023-12-29 10:46:54.000000 ooresults-0.2.9/tests/templates/test_add_competitor.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2555 2023-12-29 10:46:54.000000 ooresults-0.2.9/tests/templates/test_add_course.py
+-rw-r--r--   0 rainer    (1000) users      (100)    19545 2023-12-29 10:46:54.000000 ooresults-0.2.9/tests/templates/test_add_entry.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2828 2023-12-29 10:46:54.000000 ooresults-0.2.9/tests/templates/test_add_entry_competitors.py
+-rw-r--r--   0 rainer    (1000) users      (100)     3372 2023-12-29 10:46:54.000000 ooresults-0.2.9/tests/templates/test_add_event.py
+-rw-r--r--   0 rainer    (1000) users      (100)     3192 2023-12-29 10:46:54.000000 ooresults-0.2.9/tests/templates/test_series_settings.py
+-rw-r--r--   0 rainer    (1000) users      (100)     9467 2023-03-01 18:09:04.000000 ooresults-0.2.9/tests/test_compute_result_net.py
+-rw-r--r--   0 rainer    (1000) users      (100)    15440 2023-03-01 18:09:04.000000 ooresults-0.2.9/tests/test_compute_result_score.py
+-rw-r--r--   0 rainer    (1000) users      (100)    38250 2023-04-23 07:29:14.000000 ooresults-0.2.9/tests/test_compute_result_standard.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7257 2023-03-01 18:09:04.000000 ooresults-0.2.9/tests/test_configuration.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1973 2023-04-23 07:29:14.000000 ooresults-0.2.9/tests/test_globals.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.9/tests/test_handicap.py
+-rw-r--r--   0 rainer    (1000) users      (100)    20521 2023-11-26 23:16:20.000000 ooresults-0.2.9/tests/test_ranking.py
+-rw-r--r--   0 rainer    (1000) users      (100)     3671 2023-07-17 16:30:29.000000 ooresults-0.2.9/tests/test_rental_cards.py
+-rw-r--r--   0 rainer    (1000) users      (100)    40600 2023-12-26 10:38:40.000000 ooresults-0.2.9/tests/test_series.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2326 2023-03-01 18:09:04.000000 ooresults-0.2.9/tests/test_user.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2024-02-13 11:44:49.299342 ooresults-0.2.9/tests/websocket/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2024-02-07 21:11:25.000000 ooresults-0.2.9/tests/websocket/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)    12669 2024-02-07 21:11:25.000000 ooresults-0.2.9/tests/websocket/test_websocket_handler.py
```

### Comparing `ooresults-0.2.8/LICENSE` & `ooresults-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/PKG-INFO` & `ooresults-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooresults
-Version: 0.2.8
+Version: 0.2.9
 Summary: A software for the evaluation of the results of orienteering events
 Author: Rainer Garus
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -691,14 +691,15 @@
 Requires-Dist: fpdf2!=2.5.7
 Requires-Dist: pyserial
 Requires-Dist: tzlocal
 Requires-Dist: unidecode
 Requires-Dist: pyOpenSSL
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-asyncio; extra == "test"
 
 .. image:: https://img.shields.io/pypi/v/ooresults
     :target: https://pypi.org/project/ooresults/
 
 .. image:: https://img.shields.io/pypi/pyversions/ooresults
     :target: https://pypi.org/project/ooresults/
```

### Comparing `ooresults-0.2.8/README.rst` & `ooresults-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/__init__.py` & `ooresults-0.2.9/ooresults/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/_reader.py` & `ooresults-0.2.9/ooresults/_reader.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/_server.py` & `ooresults-0.2.9/ooresults/_server.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/configuration.py` & `ooresults-0.2.9/ooresults/configuration.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/handler/__init__.py` & `ooresults-0.2.9/ooresults/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/handler/build_results.py` & `ooresults-0.2.9/ooresults/handler/build_results.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/handler/classes.py` & `ooresults-0.2.9/ooresults/handler/classes.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/handler/clubs.py` & `ooresults-0.2.9/ooresults/handler/clubs.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/handler/competitors.py` & `ooresults-0.2.9/ooresults/handler/competitors.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/handler/courses.py` & `ooresults-0.2.9/ooresults/handler/courses.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/handler/demo_reader.py` & `ooresults-0.2.9/ooresults/handler/demo_reader.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/handler/entries.py` & `ooresults-0.2.9/ooresults/handler/entries.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/handler/events.py` & `ooresults-0.2.9/ooresults/handler/events.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/handler/handicap.py` & `ooresults-0.2.9/ooresults/handler/handicap.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/handler/model.py` & `ooresults-0.2.9/ooresults/handler/model.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/handler/results.py` & `ooresults-0.2.9/ooresults/handler/results.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/handler/series.py` & `ooresults-0.2.9/ooresults/handler/series.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/pdf/fonts/Carlito-Bold.ttf` & `ooresults-0.2.9/ooresults/pdf/fonts/Carlito-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/pdf/fonts/Carlito-BoldItalic.ttf` & `ooresults-0.2.9/ooresults/pdf/fonts/Carlito-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/pdf/fonts/Carlito-Italic.ttf` & `ooresults-0.2.9/ooresults/pdf/fonts/Carlito-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/pdf/fonts/Carlito-Regular.ttf` & `ooresults-0.2.9/ooresults/pdf/fonts/Carlito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/pdf/pdf.py` & `ooresults-0.2.9/ooresults/pdf/pdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,43 +36,39 @@
         ResultStatus.DID_NOT_FINISH: "DNF",
         ResultStatus.OVER_TIME: "OTL",
         ResultStatus.DISQUALIFIED: "DSQ",
     }
 
     def __init__(self, name: str, landscape: bool = False):
         orientation = "landscape" if landscape else "portrait"
-        super().__init__(font_cache_dir=None, orientation=orientation)
+        super().__init__(orientation=orientation)
         self.name = name
         self.creation_time = datetime.now()
         self.set_creator(creator="https://pypi.org/project/ooresults")
         self.set_producer(producer="https://pypi.org/project/ooresults")
 
         self.fonts_dir = pathlib.Path(__file__).parent / "fonts"
         self.add_font(
             family="Carlito",
             fname=str(self.fonts_dir / "Carlito-Regular.ttf"),
-            uni=True,
         )
         self.add_font(
             family="Carlito",
             style="B",
             fname=str(self.fonts_dir / "Carlito-Bold.ttf"),
-            uni=True,
         )
         self.add_font(
             family="Carlito",
             style="I",
             fname=str(self.fonts_dir / "Carlito-Italic.ttf"),
-            uni=True,
         )
         self.add_font(
             family="Carlito",
             style="BI",
             fname=str(self.fonts_dir / "Carlito-BoldItalic.ttf"),
-            uni=True,
         )
 
     def header(self):
         self.set_font(family="Carlito", size=12)
         self.cell(w=0, h=10, txt=self.name, border=1, align="C")
         self.ln(20)
 
@@ -82,26 +78,29 @@
         self.set_font(family="Carlito", size=12)
         # Printing page number
         self.cell(
             w=0, h=10, txt=self.creation_time.strftime("%Y-%m-%d %H:%M:%S"), align="L"
         )
         self.cell(w=0, h=10, txt=f"Page {self.page_no()}/{{nb}}", align="R")
 
-    def course_data(self, class_: ClassInfoType) -> str:
+    def course_data(self, class_info: ClassInfoType) -> str:
         #
         # compute course data string:
         # course length - course climb - number of controls
         #
         s = ""
-        if class_.course_length is not None:
+        if class_info.course_length is not None:
             if s != "":
                 s += " - "
-            s += str(round(class_.course_length)) + " m"
-        if class_.course_climb is not None:
+            s += str(round(class_info.course_length)) + " m"
+        if class_info.course_climb is not None:
             if s != "":
                 s += " - "
-            s += str(round(class_.course_id)) + " m"
-        if class_.number_of_controls is not None and class_.number_of_controls > 0:
+            s += str(round(class_info.course_climb)) + " Hm"
+        if (
+            class_info.number_of_controls is not None
+            and class_info.number_of_controls > 0
+        ):
             if s != "":
                 s += " - "
-            s += str(class_.number_of_controls) + " Posten"
+            s += str(class_info.number_of_controls) + " Posten"
         return s
```

### Comparing `ooresults-0.2.8/ooresults/pdf/result.py` & `ooresults-0.2.9/ooresults/pdf/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         pdf.ln()
 
         ranked = False
         for ranked_result in ranked_results:
             entry = ranked_result.entry
             result = entry.result
 
-            def f(value: Union[Optional[int] | Optional[str]]) -> str:
+            def f(value: Union[Optional[int], Optional[str]]) -> str:
                 return str(value) if value is not None else ""
 
             pdf.set_font(family="Carlito", size=12)
             if ranked_result.rank is not None:
                 ranked = True
             elif ranked:
                 ranked = False
```

### Comparing `ooresults-0.2.8/ooresults/pdf/series.py` & `ooresults-0.2.9/ooresults/pdf/series.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/pdf/splittimes.py` & `ooresults-0.2.9/ooresults/pdf/splittimes.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             entry = ranked_result.entry
             result = entry.result
 
             def get(d: Dict, key: str) -> str:
                 s = d.get(key, "")
                 return s if s is not None else ""
 
-            def f(value: Union[Optional[int] | Optional[str]]) -> str:
+            def f(value: Union[Optional[int], Optional[str]]) -> str:
                 return str(value) if value is not None else ""
 
             class Result:
                 def __init__(self, result: PersonRaceResult):
                     self.result = result
 
                 def t(
```

### Comparing `ooresults-0.2.8/ooresults/plugins/__init__.py` & `ooresults-0.2.9/ooresults/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/plugins/imports/entries/__init__.py` & `ooresults-0.2.9/ooresults/plugins/imports/entries/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/plugins/imports/entries/text.py` & `ooresults-0.2.9/ooresults/plugins/imports/entries/text.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/plugins/iof_class_list.py` & `ooresults-0.2.9/ooresults/plugins/iof_class_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/plugins/iof_competitor_list.py` & `ooresults-0.2.9/ooresults/plugins/iof_competitor_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/plugins/iof_course_data.py` & `ooresults-0.2.9/ooresults/plugins/iof_course_data.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/plugins/iof_entry_list.py` & `ooresults-0.2.9/ooresults/plugins/iof_entry_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/plugins/iof_result_list.py` & `ooresults-0.2.9/ooresults/plugins/iof_result_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/plugins/oe12.py` & `ooresults-0.2.9/ooresults/plugins/oe12.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/plugins/oe2003.py` & `ooresults-0.2.9/ooresults/plugins/oe2003.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/reader.py` & `ooresults-0.2.9/ooresults/reader.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/__init__.py` & `ooresults-0.2.9/ooresults/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/class_params.py` & `ooresults-0.2.9/ooresults/repo/class_params.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/class_type.py` & `ooresults-0.2.9/ooresults/repo/class_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/club_type.py` & `ooresults-0.2.9/ooresults/repo/club_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/competitor_type.py` & `ooresults-0.2.9/ooresults/repo/competitor_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/course_type.py` & `ooresults-0.2.9/ooresults/repo/course_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/entry_type.py` & `ooresults-0.2.9/ooresults/repo/entry_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/event_type.py` & `ooresults-0.2.9/ooresults/repo/event_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/repo.py` & `ooresults-0.2.9/ooresults/repo/repo.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/result_type.py` & `ooresults-0.2.9/ooresults/repo/result_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/series_type.py` & `ooresults-0.2.9/ooresults/repo/series_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/sqlite_repo.py` & `ooresults-0.2.9/ooresults/repo/sqlite_repo.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/start_type.py` & `ooresults-0.2.9/ooresults/repo/start_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/update/__init__.py` & `ooresults-0.2.9/ooresults/repo/update/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/update/update_008.py` & `ooresults-0.2.9/ooresults/repo/update/update_008.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/update/update_008a.py` & `ooresults-0.2.9/ooresults/repo/update/update_008a.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/repo/update/update_tables.py` & `ooresults-0.2.9/ooresults/repo/update/update_tables.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/schema/IOF.xsd` & `ooresults-0.2.9/ooresults/schema/IOF.xsd`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/schema/cardreader_log.json` & `ooresults-0.2.9/ooresults/schema/cardreader_log.json`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/server.py` & `ooresults-0.2.9/ooresults/server.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/set_legacy_mode.py` & `ooresults-0.2.9/ooresults/set_legacy_mode.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/static/style-tab.css` & `ooresults-0.2.9/ooresults/static/style-tab.css`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/static/style.css` & `ooresults-0.2.9/ooresults/static/style.css`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/static/w3.js` & `ooresults-0.2.9/ooresults/static/w3.js`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/add_class.html` & `ooresults-0.2.9/ooresults/templates/add_class.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/add_club.html` & `ooresults-0.2.9/ooresults/templates/add_club.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/add_competitor.html` & `ooresults-0.2.9/ooresults/templates/add_competitor.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/add_course.html` & `ooresults-0.2.9/ooresults/templates/add_course.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/add_entry.html` & `ooresults-0.2.9/ooresults/templates/add_entry.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/add_entry_competitors.html` & `ooresults-0.2.9/ooresults/templates/add_entry_competitors.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/add_entry_result.html` & `ooresults-0.2.9/ooresults/templates/add_entry_result.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/add_event.html` & `ooresults-0.2.9/ooresults/templates/add_event.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/classes_tab_content.html` & `ooresults-0.2.9/ooresults/templates/classes_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/classes_table.html` & `ooresults-0.2.9/ooresults/templates/classes_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/clubs_tab_content.html` & `ooresults-0.2.9/ooresults/templates/clubs_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/competitors_tab_content.html` & `ooresults-0.2.9/ooresults/templates/competitors_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/competitors_table.html` & `ooresults-0.2.9/ooresults/templates/competitors_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/courses_tab_content.html` & `ooresults-0.2.9/ooresults/templates/courses_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/courses_table.html` & `ooresults-0.2.9/ooresults/templates/courses_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/demo_reader.html` & `ooresults-0.2.9/ooresults/templates/demo_reader.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/entries_tab_content.html` & `ooresults-0.2.9/ooresults/templates/entries_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/entries_table.html` & `ooresults-0.2.9/ooresults/templates/entries_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/events_tab_content.html` & `ooresults-0.2.9/ooresults/templates/events_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/events_table.html` & `ooresults-0.2.9/ooresults/templates/events_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/main.html` & `ooresults-0.2.9/ooresults/templates/main.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/results_tab_content.html` & `ooresults-0.2.9/ooresults/templates/results_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/results_table.html` & `ooresults-0.2.9/ooresults/templates/results_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/root.html` & `ooresults-0.2.9/ooresults/templates/root.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/select_event.html` & `ooresults-0.2.9/ooresults/templates/select_event.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/series_settings.html` & `ooresults-0.2.9/ooresults/templates/series_settings.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/series_tab_content.html` & `ooresults-0.2.9/ooresults/templates/series_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/series_table.html` & `ooresults-0.2.9/ooresults/templates/series_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/si/si1_data.html` & `ooresults-0.2.9/ooresults/templates/si/si1_data.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/si/si1_page.html` & `ooresults-0.2.9/ooresults/templates/si/si1_page.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/si/si2_data.html` & `ooresults-0.2.9/ooresults/templates/si/si2_data.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/templates/si/si2_page.html` & `ooresults-0.2.9/ooresults/templates/si/si2_page.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/user.py` & `ooresults-0.2.9/ooresults/user.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/utils/__init__.py` & `ooresults-0.2.9/ooresults/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/utils/globals.py` & `ooresults-0.2.9/ooresults/utils/globals.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/utils/rental_cards.py` & `ooresults-0.2.9/ooresults/utils/rental_cards.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/websocket_server/__init__.py` & `ooresults-0.2.9/ooresults/websocket_server/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/websocket_server/si.py` & `ooresults-0.2.9/ooresults/websocket_server/si.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults/websocket_server/websocket_handler.py` & `ooresults-0.2.9/ooresults/websocket_server/websocket_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 
 import asyncio
 import copy
 import json
 import pathlib
 import datetime
+import logging
 import bz2
 import functools
-import traceback
 from concurrent.futures import ThreadPoolExecutor
 from typing import Dict
 
 import tzlocal
 import websockets
 from websockets.legacy.server import WebSocketServerProtocol
 import web
@@ -67,39 +67,27 @@
     async def update_event(self, event: EventType) -> None:
         if event:
             connections = {
                 k: v
                 for k, v in self.connections.items()
                 if v[0] == "/si2" and str(event.id) == v[1]
             }
-            if connections:
-                await asyncio.wait(
-                    [
-                        self.send(conn=conn, event=copy.deepcopy(event), message={})
-                        for conn in connections
-                    ]
-                )
+            for conn in connections:
+                await self.send(conn=conn, event=copy.deepcopy(event), message={})
 
-    async def send_to_all(self, event: EventType, message: Dict = {}) -> None:
+    async def send_to_all(self, event: EventType, message: Dict) -> None:
         if event:
             connections = {
                 k: v for k, v in self.connections.items() if str(event.id) == v[1]
             }
-            if connections:
-                await asyncio.wait(
-                    [
-                        self.send(
-                            conn=conn, event=copy.deepcopy(event), message=message
-                        )
-                        for conn in connections
-                    ]
-                )
+            for conn in connections:
+                await self.send(conn=conn, event=copy.deepcopy(event), message=message)
 
     async def send(
-        self, conn: WebSocketServerProtocol, event: EventType, message: Dict = {}
+        self, conn: WebSocketServerProtocol, event: EventType, message: Dict
     ) -> None:
         status = (
             self.cardreader_status[event.id]
             if event and event.id in self.cardreader_status
             else "offline"
         )
         path, event_id, event_key = self.connections[conn]
@@ -111,22 +99,23 @@
             elif message.get("error", None) is not None:
                 data = render.si.si1_error(message)
             elif message.get("lastName", None) is not None:
                 data = render.si.si1_data(message)
             else:
                 return
             data = json.dumps({"status": status, "data": str(data)})
-        print("WEBSOCKET SEND ...", conn)
-        await conn.send(str(data))
+        try:
+            await conn.send(str(data))
+        except websockets.ConnectionClosed:
+            pass
 
     async def handler(self, websocket: WebSocketServerProtocol, path: str) -> None:
-        print("WEBSOCKET CONNECTED")
-        print("websocket:", websocket)
+        addr = f"addr: {websocket.remote_address}, path: {path}"
+        print(f"WEBSOCKET CONNECTED, {addr}")
         print("websocket.request_headers:", websocket.request_headers)
-        print("path:", path)
 
         if path == "/demo":
             event = None
             try:
                 if self.demo_reader:
                     async for message in websocket:
                         # workaround to detect lost websocket connection in the browser
@@ -208,17 +197,14 @@
                                         model.store_cardreader_result,
                                         event_key=item["key"],
                                         item=d,
                                     ),
                                 )
                             except EventNotFoundError as e:
                                 raise RuntimeError(str(e))
-                            except Exception as e:
-                                traceback.print_exc()
-                                raise RuntimeError(str(e))
 
                             self.cardreader_status[event.id] = status
 
                             if "entryTime" in res:
                                 res["entryTime"] = res["entryTime"].strftime("%H:%M:%S")
 
                             if status == "cardRead":
@@ -229,18 +215,21 @@
 
                             res["readerStatus"] = status
                             res["event"] = event.name
                             if "status" in res:
                                 res["status"] = res["status"].name
                             print(res)
 
-            except websockets.exceptions.ConnectionClosed:
+            except websockets.ConnectionClosed:
                 pass
+            except Exception as e:
+                logging.exception(e)
+                await websocket.close()
             finally:
-                print("WEBSOCKET CONNECTION CLOSED", websocket)
+                print(f"WEBSOCKET CLOSED, {addr}")
                 if event:
                     if event.id in self.cardreader_status:
                         del self.cardreader_status[event.id]
                     await self.send_to_all(event=copy.deepcopy(event), message={})
 
         elif path == "/cardreader":
             event = None
@@ -274,17 +263,14 @@
                                 model.store_cardreader_result,
                                 event_key=event_key,
                                 item=item,
                             ),
                         )
                     except EventNotFoundError as e:
                         raise RuntimeError(str(e))
-                    except Exception as e:
-                        traceback.print_exc()
-                        raise RuntimeError(str(e))
 
                     self.cardreader_status[event.id] = status
 
                     if "entryTime" in res:
                         res["entryTime"] = res["entryTime"].strftime("%H:%M:%S")
 
                     if status == "cardRead":
@@ -296,21 +282,22 @@
                     res["readerStatus"] = status
                     res["event"] = event.name
                     if "status" in res:
                         res["status"] = res["status"].name
                     print(res)
                     await websocket.send(json.dumps(res))
 
-            except websockets.exceptions.ConnectionClosed:
+            except websockets.ConnectionClosed:
                 pass
             except Exception as e:
+                logging.exception(e)
                 await websocket.send(str(e))
-                print(str(e))
+                await websocket.close()
             finally:
-                print("CARDREADER CONNECTION CLOSED", websocket)
+                print(f"WEBSOCKET CLOSED, {addr}")
                 if event:
                     if event.id in self.cardreader_status:
                         del self.cardreader_status[event.id]
                     await self.send_to_all(event=copy.deepcopy(event), message={})
 
         else:
             try:
@@ -328,17 +315,18 @@
                             await self.send(conn=websocket, event=e, message={})
                             async for message in websocket:
                                 # workaround to detect lost websocket connection in the browser
                                 # see https://stackoverflow.com/questions/26971026/handling-connection-loss-with-websockets
                                 if message == "__ping__":
                                     await websocket.send("__pong__")
                                 else:
-                                    print("WEBSOCKET RECEIVED", websocket, message)
+                                    print(f"WEBSOCKET RECEIVED, {addr}, {message}")
                                     break
                     else:
                         await websocket.send("__no_access__")
-            except websockets.exceptions.ConnectionClosed:
+            except websockets.ConnectionClosed:
                 pass
             finally:
                 if websocket in self.connections:
                     del self.connections[websocket]
-                print("WEBSOCKET CONNECTION CLOSED", websocket)
+                await websocket.close()
+                print(f"WEBSOCKET CLOSED, {addr}")
```

### Comparing `ooresults-0.2.8/ooresults/websocket_server/websocket_server.py` & `ooresults-0.2.9/ooresults/websocket_server/websocket_server.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/ooresults.egg-info/PKG-INFO` & `ooresults-0.2.9/ooresults.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooresults
-Version: 0.2.8
+Version: 0.2.9
 Summary: A software for the evaluation of the results of orienteering events
 Author: Rainer Garus
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -691,14 +691,15 @@
 Requires-Dist: fpdf2!=2.5.7
 Requires-Dist: pyserial
 Requires-Dist: tzlocal
 Requires-Dist: unidecode
 Requires-Dist: pyOpenSSL
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-asyncio; extra == "test"
 
 .. image:: https://img.shields.io/pypi/v/ooresults
     :target: https://pypi.org/project/ooresults/
 
 .. image:: https://img.shields.io/pypi/pyversions/ooresults
     :target: https://pypi.org/project/ooresults/
```

### Comparing `ooresults-0.2.8/ooresults.egg-info/SOURCES.txt` & `ooresults-0.2.9/ooresults.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,16 @@
 tests/model/__init__.py
 tests/model/test_build_series_result.py
 tests/model/test_classes.py
 tests/model/test_courses.py
 tests/model/test_event_class_results.py
 tests/model/test_parse_cardreader_log.py
 tests/model/test_store_cardreader_result.py
+tests/pdf/__init__.py
+tests/pdf/test_pdf.py
 tests/plugins/test_export_competitors_oe12.py
 tests/plugins/test_export_competitors_oe2003.py
 tests/plugins/test_import_competitors_oe2003.py
 tests/plugins/test_plugin_iof_class_list.py
 tests/plugins/test_plugin_iof_competitor_list.py
 tests/plugins/test_plugin_iof_course_data.py
 tests/plugins/test_plugin_iof_entry_list.py
@@ -150,8 +152,10 @@
 tests/templates/test_add_class.py
 tests/templates/test_add_club.py
 tests/templates/test_add_competitor.py
 tests/templates/test_add_course.py
 tests/templates/test_add_entry.py
 tests/templates/test_add_entry_competitors.py
 tests/templates/test_add_event.py
-tests/templates/test_series_settings.py
+tests/templates/test_series_settings.py
+tests/websocket/__init__.py
+tests/websocket/test_websocket_handler.py
```

### Comparing `ooresults-0.2.8/pyproject.toml` & `ooresults-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ooresults"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   {name="Rainer Garus"},
 ]
 description = "A software for the evaluation of the results of orienteering events"
 readme = "README.rst"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
@@ -39,14 +39,15 @@
     "unidecode",
     "pyOpenSSL",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest",
+    "pytest-asyncio",
 ]
 
 [project.scripts]
 ooresults-server = "ooresults._server:main"
 ooresults-reader = "ooresults._reader:main"
 
 [project.urls]
```

### Comparing `ooresults-0.2.8/tests/__init__.py` & `ooresults-0.2.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/model/__init__.py` & `ooresults-0.2.9/tests/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/model/test_build_series_result.py` & `ooresults-0.2.9/tests/model/test_build_series_result.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/model/test_classes.py` & `ooresults-0.2.9/tests/model/test_classes.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/model/test_courses.py` & `ooresults-0.2.9/tests/model/test_courses.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/model/test_event_class_results.py` & `ooresults-0.2.9/tests/model/test_event_class_results.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/model/test_parse_cardreader_log.py` & `ooresults-0.2.9/tests/model/test_parse_cardreader_log.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/model/test_store_cardreader_result.py` & `ooresults-0.2.9/tests/model/test_store_cardreader_result.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/plugins/test_export_competitors_oe12.py` & `ooresults-0.2.9/tests/plugins/test_export_competitors_oe12.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/plugins/test_export_competitors_oe2003.py` & `ooresults-0.2.9/tests/plugins/test_export_competitors_oe2003.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/plugins/test_import_competitors_oe2003.py` & `ooresults-0.2.9/tests/plugins/test_import_competitors_oe2003.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/plugins/test_plugin_iof_class_list.py` & `ooresults-0.2.9/tests/plugins/test_plugin_iof_class_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/plugins/test_plugin_iof_competitor_list.py` & `ooresults-0.2.9/tests/plugins/test_plugin_iof_competitor_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/plugins/test_plugin_iof_course_data.py` & `ooresults-0.2.9/tests/plugins/test_plugin_iof_course_data.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/plugins/test_plugin_iof_entry_list.py` & `ooresults-0.2.9/tests/plugins/test_plugin_iof_entry_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/plugins/test_plugin_iof_result_list.py` & `ooresults-0.2.9/tests/plugins/test_plugin_iof_result_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/repo/__init__.py` & `ooresults-0.2.9/tests/pdf/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/repo/test_classes.py` & `ooresults-0.2.9/tests/repo/test_classes.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/repo/test_clubs.py` & `ooresults-0.2.9/tests/repo/test_clubs.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/repo/test_competitors.py` & `ooresults-0.2.9/tests/repo/test_competitors.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/repo/test_courses.py` & `ooresults-0.2.9/tests/repo/test_courses.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/repo/test_entries.py` & `ooresults-0.2.9/tests/repo/test_entries.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/repo/test_events.py` & `ooresults-0.2.9/tests/repo/test_events.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/repo/test_settings.py` & `ooresults-0.2.9/tests/repo/test_settings.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/templates/__init__.py` & `ooresults-0.2.9/tests/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/templates/test_add_class.py` & `ooresults-0.2.9/tests/templates/test_add_class.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/templates/test_add_club.py` & `ooresults-0.2.9/tests/templates/test_add_club.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/templates/test_add_competitor.py` & `ooresults-0.2.9/tests/templates/test_add_competitor.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/templates/test_add_course.py` & `ooresults-0.2.9/tests/templates/test_add_course.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/templates/test_add_entry.py` & `ooresults-0.2.9/tests/templates/test_add_entry.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/templates/test_add_entry_competitors.py` & `ooresults-0.2.9/tests/templates/test_add_entry_competitors.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/templates/test_add_event.py` & `ooresults-0.2.9/tests/templates/test_add_event.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/templates/test_series_settings.py` & `ooresults-0.2.9/tests/templates/test_series_settings.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/test_compute_result_net.py` & `ooresults-0.2.9/tests/test_compute_result_net.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/test_compute_result_score.py` & `ooresults-0.2.9/tests/test_compute_result_score.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/test_compute_result_standard.py` & `ooresults-0.2.9/tests/test_compute_result_standard.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/test_configuration.py` & `ooresults-0.2.9/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/test_globals.py` & `ooresults-0.2.9/tests/test_globals.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/test_handicap.py` & `ooresults-0.2.9/tests/test_handicap.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/test_ranking.py` & `ooresults-0.2.9/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/test_rental_cards.py` & `ooresults-0.2.9/tests/test_rental_cards.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/test_series.py` & `ooresults-0.2.9/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.8/tests/test_user.py` & `ooresults-0.2.9/tests/test_user.py`

 * *Files identical despite different names*

