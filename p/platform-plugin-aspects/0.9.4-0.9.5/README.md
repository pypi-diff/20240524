# Comparing `tmp/platform_plugin_aspects-0.9.4.tar.gz` & `tmp/platform_plugin_aspects-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform_plugin_aspects-0.9.4.tar", last modified: Wed May 22 17:00:25 2024, max compression
+gzip compressed data, was "platform_plugin_aspects-0.9.5.tar", last modified: Fri May 24 16:21:06 2024, max compression
```

## Comparing `platform_plugin_aspects-0.9.4.tar` & `platform_plugin_aspects-0.9.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.387469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.387469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/extensions/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.387469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.387469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/commands/load_test_tracking_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    14312 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/base_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/course_overview_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/external_id_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/user_profile_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/user_retire_sink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.383469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/css/superset.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/html/superset.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/html/superset_student.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/js/embed_dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/js/install_required.js
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/js/superset.js
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.383469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/templates/instructor_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/waffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-05-22 17:00:25.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-22 17:00:25.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:00:25.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-22 17:00:25.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:00:25.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-22 17:00:25.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 17:00:25.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6997 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:21:06.051670 platform_plugin_aspects-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-05-24 16:21:06.051670 platform_plugin_aspects-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:21:06.043670 platform_plugin_aspects-0.9.5/platform_plugin_aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:21:06.047670 platform_plugin_aspects-0.9.5/platform_plugin_aspects/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/extensions/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:21:06.047670 platform_plugin_aspects-0.9.5/platform_plugin_aspects/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:21:06.047670 platform_plugin_aspects-0.9.5/platform_plugin_aspects/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/management/commands/load_test_tracking_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14312 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:21:06.047670 platform_plugin_aspects-0.9.5/platform_plugin_aspects/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:21:06.047670 platform_plugin_aspects-0.9.5/platform_plugin_aspects/sinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/sinks/base_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/sinks/course_overview_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/sinks/external_id_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/sinks/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/sinks/user_profile_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/sinks/user_retire_sink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:21:06.043670 platform_plugin_aspects-0.9.5/platform_plugin_aspects/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:21:06.047670 platform_plugin_aspects-0.9.5/platform_plugin_aspects/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/static/css/superset.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:21:06.051670 platform_plugin_aspects-0.9.5/platform_plugin_aspects/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/static/html/superset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/static/html/superset_student.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:21:06.051670 platform_plugin_aspects-0.9.5/platform_plugin_aspects/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/static/js/embed_dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/static/js/install_required.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/static/js/superset.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:21:06.043670 platform_plugin_aspects-0.9.5/platform_plugin_aspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:21:06.051670 platform_plugin_aspects-0.9.5/platform_plugin_aspects/templates/instructor_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects/xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:21:06.051670 platform_plugin_aspects-0.9.5/platform_plugin_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-05-24 16:21:06.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-24 16:21:06.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:21:06.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-24 16:21:06.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:21:06.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-24 16:21:06.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-24 16:21:06.000000 platform_plugin_aspects-0.9.5/platform_plugin_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:21:06.051670 platform_plugin_aspects-0.9.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-24 16:21:06.051670 platform_plugin_aspects-0.9.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6997 2024-05-24 16:20:58.000000 platform_plugin_aspects-0.9.5/setup.py
```

### Comparing `platform_plugin_aspects-0.9.4/CHANGELOG.rst` & `platform_plugin_aspects-0.9.5/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+0.9.5 - 2024-05-24
+******************
+
+Fixes
+=====
+
+* UserProfile sink now runs after the transaction is committed, preventing UserProfileNotFound errors and creation of rows in ClickHouse that don't exist in MySQL in the case of a rollback.
+
+
 0.9.4 - 2024-05-16
 ******************
 
 Fixes
 =====
 
 * Allow to serialize dates as strings in JSON.
```

### Comparing `platform_plugin_aspects-0.9.4/LICENSE` & `platform_plugin_aspects-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/PKG-INFO` & `platform_plugin_aspects-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.9.4
+Version: 0.9.5
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -272,14 +272,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+0.9.5 - 2024-05-24
+******************
+
+Fixes
+=====
+
+* UserProfile sink now runs after the transaction is committed, preventing UserProfileNotFound errors and creation of rows in ClickHouse that don't exist in MySQL in the case of a rollback.
+
+
 0.9.4 - 2024-05-16
 ******************
 
 Fixes
 =====
 
 * Allow to serialize dates as strings in JSON.
```

### Comparing `platform_plugin_aspects-0.9.4/README.rst` & `platform_plugin_aspects-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/apps.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/apps.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/extensions/filters.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/extensions/filters.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/commands/load_test_tracking_events.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/management/commands/load_test_tracking_events.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/settings/common.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/settings/common.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/settings/production.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/settings/production.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/signals.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/signals.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Signal handler functions, mapped to specific signals in apps.py.
 """
 
+from django.db import transaction
 from django.db.models.signals import post_save
 from django.dispatch import Signal, receiver
 
 from platform_plugin_aspects.sinks import (
     ExternalIdSink,
     UserProfileSink,
     UserRetirementSink,
@@ -29,38 +30,51 @@
     from platform_plugin_aspects.tasks import (  # pylint: disable=import-outside-toplevel
         dump_course_to_clickhouse,
     )
 
     dump_course_to_clickhouse.delay(str(course_key))
 
 
-def on_user_profile_updated(  # pylint: disable=unused-argument  # pragma: no cover
-    sender, instance, **kwargs
-):
+def on_user_profile_updated(instance):
     """
-    Receives post save signal and queues the dump job.
+    Queues the UserProfile dump job when the parent transaction is committed.
     """
     # import here, because signal is registered at startup, but items in tasks are not yet able to be loaded
     from platform_plugin_aspects.tasks import (  # pylint: disable=import-outside-toplevel
         dump_data_to_clickhouse,
     )
 
     sink = UserProfileSink(None, None)
     dump_data_to_clickhouse.delay(
         sink_module=sink.__module__,
         sink_name=sink.__class__.__name__,
         object_id=str(instance.id),
     )
 
 
+def on_user_profile_updated_txn(**kwargs):
+    """
+    Handle user_profile saves in the middle of a transaction.
+
+    If this gets fired before the transaction commits, the task may try to
+    query an id that doesn't exist yet and throw an error. This should postpone
+    queuing the Celery task until after the transaction is committed.
+    """
+    transaction.on_commit(
+        lambda: on_user_profile_updated(kwargs["instance"])
+    )  # pragma: no cover
+
+
 # Connect the UserProfile.post_save signal handler only if we have a model to attach to.
 # (prevents celery errors during tests)
 _user_profile = get_model("user_profile")
 if _user_profile:
-    post_save.connect(on_user_profile_updated, sender=_user_profile)  # pragma: no cover
+    post_save.connect(
+        on_user_profile_updated_txn, sender=_user_profile
+    )  # pragma: no cover
 
 
 def on_externalid_saved(  # pylint: disable=unused-argument  # pragma: no cover
     sender, instance, **kwargs
 ):
     """
     Receives post save signal and queues the dump job.
```

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/base_sink.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/sinks/base_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/course_overview_sink.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/sinks/course_overview_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/external_id_sink.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/sinks/external_id_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/serializers.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/sinks/serializers.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/user_profile_sink.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/sinks/user_profile_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/user_retire_sink.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/sinks/user_retire_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/css/superset.css` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/static/css/superset.css`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/html/superset.html` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/static/html/superset.html`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/js/embed_dashboard.js` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/static/js/embed_dashboard.js`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/js/superset.js` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/static/js/superset.js`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/tasks.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/tasks.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/templates/instructor_dashboard/aspects.html` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/templates/instructor_dashboard/aspects.html`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/urls.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/urls.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/utils.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/utils.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/views.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/views.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects/xblock.py` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects/xblock.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 from webob import Response
 from xblock.core import XBlock
 from xblock.exceptions import JsonHandlerError
 from xblock.fields import List, Scope, String
 
 # These moved from xblockutils to xblock in Quince, these can be removed
 # when we stop supporting earlier versions.
-try:  # pragma: no-cover
+try:  # pragma: no cover
     from xblock.utils.resources import ResourceLoader
     from xblock.utils.studio_editable import StudioEditableXBlockMixin
-except ImportError:
+except ImportError:  # pragma: no cover
     from xblockutils.resources import ResourceLoader
     from xblockutils.studio_editable import StudioEditableXBlockMixin
 
 from .utils import (
     DEFAULT_FILTERS_FORMAT,
     _,
     generate_guest_token,
```

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/PKG-INFO` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.9.4
+Version: 0.9.5
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -272,14 +272,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+0.9.5 - 2024-05-24
+******************
+
+Fixes
+=====
+
+* UserProfile sink now runs after the transaction is committed, preventing UserProfileNotFound errors and creation of rows in ClickHouse that don't exist in MySQL in the case of a rollback.
+
+
 0.9.4 - 2024-05-16
 ******************
 
 Fixes
 =====
 
 * Allow to serialize dates as strings in JSON.
```

### Comparing `platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/SOURCES.txt` & `platform_plugin_aspects-0.9.5/platform_plugin_aspects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/requirements/constraints.txt` & `platform_plugin_aspects-0.9.5/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.4/setup.py` & `platform_plugin_aspects-0.9.5/setup.py`

 * *Files identical despite different names*

