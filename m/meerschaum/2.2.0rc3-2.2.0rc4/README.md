# Comparing `tmp/meerschaum-2.2.0rc3.tar.gz` & `tmp/meerschaum-2.2.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meerschaum-2.2.0rc3.tar", last modified: Fri May 24 03:17:02 2024, max compression
+gzip compressed data, was "meerschaum-2.2.0rc4.tar", last modified: Fri May 24 06:35:22 2024, max compression
```

## Comparing `meerschaum-2.2.0rc3.tar` & `meerschaum-2.2.0rc4.tar`

### file list

```diff
@@ -1,301 +1,301 @@
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.438446 meerschaum-2.2.0rc3/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-2.2.0rc3/LICENSE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-2.2.0rc3/NOTICE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23384 2024-05-24 03:17:02.437446 meerschaum-2.2.0rc3/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9183 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/README.md
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.379446 meerschaum-2.2.0rc3/meerschaum/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1487 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2763 2024-05-17 16:18:37.000000 meerschaum-2.2.0rc3/meerschaum/__main__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.381446 meerschaum-2.2.0rc3/meerschaum/_internal/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-2.2.0rc3/meerschaum/_internal/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.382446 meerschaum-2.2.0rc3/meerschaum/_internal/arguments/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-2.2.0rc3/meerschaum/_internal/arguments/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10249 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/_internal/arguments/_parse_arguments.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13719 2024-05-07 20:25:34.000000 meerschaum-2.2.0rc3/meerschaum/_internal/arguments/_parser.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.382446 meerschaum-2.2.0rc3/meerschaum/_internal/docs/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/_internal/docs/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7076 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/_internal/docs/index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4806 2024-05-15 15:21:26.000000 meerschaum-2.2.0rc3/meerschaum/_internal/entry.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.382446 meerschaum-2.2.0rc3/meerschaum/_internal/gui/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1313 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/_internal/gui/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.383446 meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/_windows.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      935 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1596 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.383446 meerschaum-2.2.0rc3/meerschaum/_internal/shell/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32826 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc3/meerschaum/_internal/shell/Shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3114 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/_internal/shell/ShellCompleter.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-2.2.0rc3/meerschaum/_internal/shell/ValidAutoSuggest.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc3/meerschaum/_internal/shell/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.383446 meerschaum-2.2.0rc3/meerschaum/_internal/shell/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc3/meerschaum/_internal/shell/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.384446 meerschaum-2.2.0rc3/meerschaum/_internal/term/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      520 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/_internal/term/TermPageHandler.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1594 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/_internal/term/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      716 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/_internal/term/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.388446 meerschaum-2.2.0rc3/meerschaum/actions/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11360 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/actions/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12756 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc3/meerschaum/actions/api.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13396 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/actions/bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4851 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6213 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/copy.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1167 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15528 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/actions/delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2453 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9487 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7431 2024-05-07 20:26:48.000000 meerschaum-2.2.0rc3/meerschaum/actions/install.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2023-09-21 17:52:19.000000 meerschaum-2.2.0rc3/meerschaum/actions/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-2.2.0rc3/meerschaum/actions/os.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-13 21:37:33.000000 meerschaum-2.2.0rc3/meerschaum/actions/pause.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc3/meerschaum/actions/python.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11326 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/actions/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      508 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/actions/reload.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3205 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/setup.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-2.2.0rc3/meerschaum/actions/sh.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    29016 2024-05-22 21:36:42.000000 meerschaum-2.2.0rc3/meerschaum/actions/show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-10-27 06:03:46.000000 meerschaum-2.2.0rc3/meerschaum/actions/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5886 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc3/meerschaum/actions/stack.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18384 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/actions/start.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/stop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    17518 2024-03-26 19:47:08.000000 meerschaum-2.2.0rc3/meerschaum/actions/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3053 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/actions/tag.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6068 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/uninstall.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6302 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/upgrade.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4885 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.389446 meerschaum-2.2.0rc3/meerschaum/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7410 2024-05-23 05:45:25.000000 meerschaum-2.2.0rc3/meerschaum/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc3/meerschaum/api/_chain.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1603 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/_events.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      961 2023-08-24 00:13:16.000000 meerschaum-2.2.0rc3/meerschaum/api/_oauth2.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1609 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/api/_websockets.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.391446 meerschaum-2.2.0rc3/meerschaum/api/dash/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2252 2024-03-20 22:38:46.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9418 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/actions.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.392446 meerschaum-2.2.0rc3/meerschaum/api/dash/assets/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/assets/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/assets/ansi_up.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/assets/banner_1920x320.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/assets/favicon.ico
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/assets/logo_48x48.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/assets/logo_500x500.png
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.393446 meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      325 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32283 2024-05-22 21:31:12.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7689 2024-05-10 01:45:18.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2613 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3600 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6364 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/components.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2046 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/graphs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7529 2024-05-10 02:30:25.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12591 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/keys.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.394446 meerschaum-2.2.0rc3/meerschaum/api/dash/pages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-07-21 01:07:38.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/pages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3930 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/pages/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      595 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/pages/error.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4600 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/pages/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1549 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/pages/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2364 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/pages/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19233 2024-05-17 02:49:16.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3662 2024-05-16 15:25:17.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/websockets.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3298 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/webterm.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.395446 meerschaum-2.2.0rc3/meerschaum/api/models/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/models/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/models/_interfaces.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/models/_locations.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/models/_metrics.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-2.2.0rc3/meerschaum/api/models/_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.395446 meerschaum-2.2.0rc3/meerschaum/api/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.395446 meerschaum-2.2.0rc3/meerschaum/api/resources/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.396446 meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/bootstrap.min.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1714 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/dash.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/dbc_dark.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/styles.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5383 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/xterm.css
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.396446 meerschaum-2.2.0rc3/meerschaum/api/resources/static/ico/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/ico/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/ico/logo.ico
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.397446 meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/action_button.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/main.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1729 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/terminado.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   289441 2024-04-05 14:30:27.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/xterm.js
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.397446 meerschaum-2.2.0rc3/meerschaum/api/resources/static/png/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/png/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.398446 meerschaum-2.2.0rc3/meerschaum/api/resources/templates/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/templates/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/templates/index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/templates/old_index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/templates/secret.html
--rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     4527 2024-05-22 21:27:22.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/templates/termpage.html
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.400446 meerschaum-2.2.0rc3/meerschaum/api/routes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      564 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1849 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1933 2024-05-22 19:54:14.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2469 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21677 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6216 2024-05-16 15:09:58.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7204 2023-08-24 00:13:16.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_version.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_webterm.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.400446 meerschaum-2.2.0rc3/meerschaum/api/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      482 2023-10-26 06:22:59.000000 meerschaum-2.2.0rc3/meerschaum/api/tables/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.401446 meerschaum-2.2.0rc3/meerschaum/config/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11517 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/config/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2024-05-16 15:33:56.000000 meerschaum-2.2.0rc3/meerschaum/config/_dash.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5251 2024-05-16 15:31:32.000000 meerschaum-2.2.0rc3/meerschaum/config/_default.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8218 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/config/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4419 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/config/_environment.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6635 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/config/_formatting.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1227 2024-05-23 04:18:10.000000 meerschaum-2.2.0rc3/meerschaum/config/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1526 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/config/_patch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8154 2024-05-23 00:55:12.000000 meerschaum-2.2.0rc3/meerschaum/config/_paths.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc3/meerschaum/config/_preprocess.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14720 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/config/_read_config.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3551 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc3/meerschaum/config/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4155 2024-05-22 20:00:09.000000 meerschaum-2.2.0rc3/meerschaum/config/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       74 2024-05-24 02:32:37.000000 meerschaum-2.2.0rc3/meerschaum/config/_version.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.401446 meerschaum-2.2.0rc3/meerschaum/config/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/config/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.402446 meerschaum-2.2.0rc3/meerschaum/config/stack/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9007 2024-05-22 20:05:40.000000 meerschaum-2.2.0rc3/meerschaum/config/stack/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.402446 meerschaum-2.2.0rc3/meerschaum/config/stack/grafana/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2024-05-22 20:11:13.000000 meerschaum-2.2.0rc3/meerschaum/config/stack/grafana/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.402446 meerschaum-2.2.0rc3/meerschaum/config/stack/mosquitto/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/config/stack/mosquitto/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.402446 meerschaum-2.2.0rc3/meerschaum/config/stack/mosquitto/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/config/stack/mosquitto/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.402446 meerschaum-2.2.0rc3/meerschaum/config/stack/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/config/stack/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.402446 meerschaum-2.2.0rc3/meerschaum/config/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4474 2024-05-23 05:41:27.000000 meerschaum-2.2.0rc3/meerschaum/config/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.402446 meerschaum-2.2.0rc3/meerschaum/connectors/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc3/meerschaum/connectors/Connector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12071 2024-05-23 02:54:44.000000 meerschaum-2.2.0rc3/meerschaum/connectors/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.403446 meerschaum-2.2.0rc3/meerschaum/connectors/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4355 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/APIConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2755 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2050 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1093 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20962 2023-11-10 05:44:22.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5217 2024-05-07 20:27:04.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6922 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_request.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5275 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4044 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc3/meerschaum/connectors/parse.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.404446 meerschaum-2.2.0rc3/meerschaum/connectors/plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-2.2.0rc3/meerschaum/connectors/plugin/PluginConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/connectors/plugin/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7363 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/connectors/poll.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.405446 meerschaum-2.2.0rc3/meerschaum/connectors/sql/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11709 2024-05-23 02:46:39.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/SQLConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4123 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_cli.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10396 2024-05-23 03:26:48.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_create_engine.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13086 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6509 2024-05-24 02:32:37.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_instance.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   101357 2024-05-24 02:52:48.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8321 2024-05-16 15:18:16.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34199 2024-05-24 02:32:37.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3460 2023-10-26 06:22:59.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10100 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_users.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.405446 meerschaum-2.2.0rc3/meerschaum/connectors/sql/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9001 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/tables/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/tables/types.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.405446 meerschaum-2.2.0rc3/meerschaum/core/
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.407446 meerschaum-2.2.0rc3/meerschaum/core/Pipe/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16230 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_attributes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2261 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20880 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_data.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10267 2023-11-13 06:20:00.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2118 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3694 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5234 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    28038 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14262 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.407446 meerschaum-2.2.0rc3/meerschaum/core/Plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc3/meerschaum/core/Plugin/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.407446 meerschaum-2.2.0rc3/meerschaum/core/User/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6527 2024-05-23 06:00:16.000000 meerschaum-2.2.0rc3/meerschaum/core/User/_User.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      193 2024-05-22 19:53:09.000000 meerschaum-2.2.0rc3/meerschaum/core/User/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc3/meerschaum/core/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.407446 meerschaum-2.2.0rc3/meerschaum/plugins/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34039 2024-05-16 15:06:05.000000 meerschaum-2.2.0rc3/meerschaum/plugins/_Plugin.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21866 2024-05-23 03:07:17.000000 meerschaum-2.2.0rc3/meerschaum/plugins/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.409446 meerschaum-2.2.0rc3/meerschaum/utils/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/utils/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11460 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/utils/_get_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.409446 meerschaum-2.2.0rc3/meerschaum/utils/daemon/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34414 2024-05-23 05:42:59.000000 meerschaum-2.2.0rc3/meerschaum/utils/daemon/Daemon.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4544 2024-05-23 04:51:08.000000 meerschaum-2.2.0rc3/meerschaum/utils/daemon/FileDescriptorInterceptor.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23499 2024-05-22 23:55:35.000000 meerschaum-2.2.0rc3/meerschaum/utils/daemon/RotatingFile.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8375 2024-05-22 22:31:49.000000 meerschaum-2.2.0rc3/meerschaum/utils/daemon/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4330 2023-09-26 04:28:45.000000 meerschaum-2.2.0rc3/meerschaum/utils/daemon/_names.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31955 2024-05-24 03:15:14.000000 meerschaum-2.2.0rc3/meerschaum/utils/dataframe.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-2.2.0rc3/meerschaum/utils/debug.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.410446 meerschaum-2.2.0rc3/meerschaum/utils/dtypes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6261 2024-03-26 20:33:15.000000 meerschaum-2.2.0rc3/meerschaum/utils/dtypes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14638 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/utils/dtypes/sql.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.410446 meerschaum-2.2.0rc3/meerschaum/utils/formatting/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13778 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/utils/formatting/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3294 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/utils/formatting/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19492 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc3/meerschaum/utils/formatting/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3096 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/utils/formatting/_pprint.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3677 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/utils/formatting/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3196 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/utils/interactive.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    43296 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc3/meerschaum/utils/misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc3/meerschaum/utils/networking.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.411446 meerschaum-2.2.0rc3/meerschaum/utils/packages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    57185 2024-05-23 05:06:05.000000 meerschaum-2.2.0rc3/meerschaum/utils/packages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7923 2024-05-24 02:32:37.000000 meerschaum-2.2.0rc3/meerschaum/utils/packages/_packages.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-2.2.0rc3/meerschaum/utils/packages/lazy_loader.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2655 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/utils/pool.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7192 2024-05-23 05:42:16.000000 meerschaum-2.2.0rc3/meerschaum/utils/process.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16490 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/utils/prompt.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10654 2024-05-24 02:36:46.000000 meerschaum-2.2.0rc3/meerschaum/utils/schedule.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    46656 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc3/meerschaum/utils/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2489 2024-05-17 21:02:01.000000 meerschaum-2.2.0rc3/meerschaum/utils/threading.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2807 2024-03-20 22:41:20.000000 meerschaum-2.2.0rc3/meerschaum/utils/typing.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.411446 meerschaum-2.2.0rc3/meerschaum/utils/venv/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3553 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc3/meerschaum/utils/venv/_Venv.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23183 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/utils/venv/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6535 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/utils/warnings.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-2.2.0rc3/meerschaum/utils/yaml.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.411446 meerschaum-2.2.0rc3/meerschaum.egg-info/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23384 2024-05-24 03:17:02.000000 meerschaum-2.2.0rc3/meerschaum.egg-info/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8485 2024-05-24 03:17:02.000000 meerschaum-2.2.0rc3/meerschaum.egg-info/SOURCES.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-24 03:17:02.000000 meerschaum-2.2.0rc3/meerschaum.egg-info/dependency_links.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2024-05-24 03:17:02.000000 meerschaum-2.2.0rc3/meerschaum.egg-info/entry_points.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4732 2024-05-24 03:17:02.000000 meerschaum-2.2.0rc3/meerschaum.egg-info/requires.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2024-05-24 03:17:02.000000 meerschaum-2.2.0rc3/meerschaum.egg-info/top_level.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-24 03:17:02.000000 meerschaum-2.2.0rc3/meerschaum.egg-info/zip-safe
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2024-05-24 03:17:02.438446 meerschaum-2.2.0rc3/setup.cfg
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3254 2024-05-15 14:36:58.000000 meerschaum-2.2.0rc3/setup.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.411446 meerschaum-2.2.0rc3/tests/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3139 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/tests/test_deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15351 2023-11-13 21:37:33.000000 meerschaum-2.2.0rc3/tests/test_pipes_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3646 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/tests/test_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21905 2024-05-24 02:32:37.000000 meerschaum-2.2.0rc3/tests/test_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      744 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/tests/test_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3090 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/tests/test_verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.895734 meerschaum-2.2.0rc4/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-2.2.0rc4/LICENSE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-2.2.0rc4/NOTICE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23313 2024-05-24 06:35:22.894734 meerschaum-2.2.0rc4/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9183 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc4/README.md
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.844735 meerschaum-2.2.0rc4/meerschaum/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1487 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc4/meerschaum/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2763 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/__main__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.845735 meerschaum-2.2.0rc4/meerschaum/_internal/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-2.2.0rc4/meerschaum/_internal/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.846735 meerschaum-2.2.0rc4/meerschaum/_internal/arguments/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-2.2.0rc4/meerschaum/_internal/arguments/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10249 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/_internal/arguments/_parse_arguments.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13719 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/_internal/arguments/_parser.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.846735 meerschaum-2.2.0rc4/meerschaum/_internal/docs/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/_internal/docs/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7076 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc4/meerschaum/_internal/docs/index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4806 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/_internal/entry.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.846735 meerschaum-2.2.0rc4/meerschaum/_internal/gui/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1313 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc4/meerschaum/_internal/gui/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.847735 meerschaum-2.2.0rc4/meerschaum/_internal/gui/app/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc4/meerschaum/_internal/gui/app/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-2.2.0rc4/meerschaum/_internal/gui/app/_windows.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      935 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc4/meerschaum/_internal/gui/app/actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1596 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc4/meerschaum/_internal/gui/app/pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.847735 meerschaum-2.2.0rc4/meerschaum/_internal/shell/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32826 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc4/meerschaum/_internal/shell/Shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3114 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc4/meerschaum/_internal/shell/ShellCompleter.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-2.2.0rc4/meerschaum/_internal/shell/ValidAutoSuggest.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc4/meerschaum/_internal/shell/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.847735 meerschaum-2.2.0rc4/meerschaum/_internal/shell/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc4/meerschaum/_internal/shell/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.848734 meerschaum-2.2.0rc4/meerschaum/_internal/term/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      520 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc4/meerschaum/_internal/term/TermPageHandler.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1594 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc4/meerschaum/_internal/term/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      716 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc4/meerschaum/_internal/term/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.851734 meerschaum-2.2.0rc4/meerschaum/actions/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11360 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc4/meerschaum/actions/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12756 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc4/meerschaum/actions/api.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13396 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc4/meerschaum/actions/bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4851 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/actions/clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6213 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/actions/copy.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1167 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/actions/deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15528 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc4/meerschaum/actions/delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2453 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/actions/drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9487 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/actions/edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7431 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/actions/install.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2023-09-21 17:52:19.000000 meerschaum-2.2.0rc4/meerschaum/actions/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-2.2.0rc4/meerschaum/actions/os.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-13 21:37:33.000000 meerschaum-2.2.0rc4/meerschaum/actions/pause.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc4/meerschaum/actions/python.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11326 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc4/meerschaum/actions/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      508 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc4/meerschaum/actions/reload.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3205 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/actions/setup.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-2.2.0rc4/meerschaum/actions/sh.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    29024 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/actions/show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-10-27 06:03:46.000000 meerschaum-2.2.0rc4/meerschaum/actions/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5886 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc4/meerschaum/actions/stack.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18384 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc4/meerschaum/actions/start.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/actions/stop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    17518 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/actions/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3053 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc4/meerschaum/actions/tag.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6068 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/actions/uninstall.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6302 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/actions/upgrade.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4885 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/actions/verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.851734 meerschaum-2.2.0rc4/meerschaum/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7385 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc4/meerschaum/api/_chain.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1603 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc4/meerschaum/api/_events.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1056 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/api/_oauth2.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1609 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc4/meerschaum/api/_websockets.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.853735 meerschaum-2.2.0rc4/meerschaum/api/dash/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2252 2024-03-20 22:38:46.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9418 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/actions.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.853735 meerschaum-2.2.0rc4/meerschaum/api/dash/assets/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/assets/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/assets/ansi_up.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/assets/banner_1920x320.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/assets/favicon.ico
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/assets/logo_48x48.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/assets/logo_500x500.png
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.854735 meerschaum-2.2.0rc4/meerschaum/api/dash/callbacks/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      325 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/callbacks/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32301 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/callbacks/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7689 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/callbacks/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2613 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/callbacks/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/callbacks/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3600 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/callbacks/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6364 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/components.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2046 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/graphs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7529 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12598 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/keys.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.855734 meerschaum-2.2.0rc4/meerschaum/api/dash/pages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-07-21 01:07:38.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/pages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3835 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/pages/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      595 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/pages/error.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4600 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/pages/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1549 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/pages/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2364 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/pages/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19233 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3662 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/websockets.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3298 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc4/meerschaum/api/dash/webterm.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.855734 meerschaum-2.2.0rc4/meerschaum/api/models/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/models/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/models/_interfaces.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/models/_locations.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/models/_metrics.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-2.2.0rc4/meerschaum/api/models/_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.855734 meerschaum-2.2.0rc4/meerschaum/api/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.855734 meerschaum-2.2.0rc4/meerschaum/api/resources/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.856735 meerschaum-2.2.0rc4/meerschaum/api/resources/static/css/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/static/css/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/static/css/bootstrap.min.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1714 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/static/css/dash.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/static/css/dbc_dark.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/static/css/styles.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5383 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/static/css/xterm.css
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.856735 meerschaum-2.2.0rc4/meerschaum/api/resources/static/ico/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/static/ico/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/static/ico/logo.ico
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.856735 meerschaum-2.2.0rc4/meerschaum/api/resources/static/js/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/static/js/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/static/js/action_button.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/static/js/main.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1729 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/static/js/terminado.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   289441 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/static/js/xterm.js
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.857735 meerschaum-2.2.0rc4/meerschaum/api/resources/static/png/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/static/png/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.857735 meerschaum-2.2.0rc4/meerschaum/api/resources/templates/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/templates/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/templates/index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/templates/old_index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/templates/secret.html
+-rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     4527 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/api/resources/templates/termpage.html
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.858734 meerschaum-2.2.0rc4/meerschaum/api/routes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      564 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc4/meerschaum/api/routes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-2.2.0rc4/meerschaum/api/routes/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1849 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc4/meerschaum/api/routes/_connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc4/meerschaum/api/routes/_index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1933 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/api/routes/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2469 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc4/meerschaum/api/routes/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21677 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc4/meerschaum/api/routes/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6216 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/api/routes/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7204 2023-08-24 00:13:16.000000 meerschaum-2.2.0rc4/meerschaum/api/routes/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-2.2.0rc4/meerschaum/api/routes/_version.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc4/meerschaum/api/routes/_webterm.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.858734 meerschaum-2.2.0rc4/meerschaum/api/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      482 2023-10-26 06:22:59.000000 meerschaum-2.2.0rc4/meerschaum/api/tables/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.860735 meerschaum-2.2.0rc4/meerschaum/config/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11517 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc4/meerschaum/config/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/config/_dash.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5251 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/config/_default.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8218 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc4/meerschaum/config/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4419 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc4/meerschaum/config/_environment.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6635 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc4/meerschaum/config/_formatting.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1279 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/config/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1526 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc4/meerschaum/config/_patch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8154 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/config/_paths.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc4/meerschaum/config/_preprocess.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14720 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/config/_read_config.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3551 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc4/meerschaum/config/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4155 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/config/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       74 2024-05-24 06:35:06.000000 meerschaum-2.2.0rc4/meerschaum/config/_version.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.860735 meerschaum-2.2.0rc4/meerschaum/config/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/config/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.860735 meerschaum-2.2.0rc4/meerschaum/config/stack/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9007 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/config/stack/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.860735 meerschaum-2.2.0rc4/meerschaum/config/stack/grafana/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/config/stack/grafana/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.860735 meerschaum-2.2.0rc4/meerschaum/config/stack/mosquitto/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/config/stack/mosquitto/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.860735 meerschaum-2.2.0rc4/meerschaum/config/stack/mosquitto/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/config/stack/mosquitto/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.860735 meerschaum-2.2.0rc4/meerschaum/config/stack/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/config/stack/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.860735 meerschaum-2.2.0rc4/meerschaum/config/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4474 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/config/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.861734 meerschaum-2.2.0rc4/meerschaum/connectors/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc4/meerschaum/connectors/Connector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12071 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/connectors/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.862734 meerschaum-2.2.0rc4/meerschaum/connectors/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4355 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc4/meerschaum/connectors/api/APIConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/connectors/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2755 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc4/meerschaum/connectors/api/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/connectors/api/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2050 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc4/meerschaum/connectors/api/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1093 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc4/meerschaum/connectors/api/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20962 2023-11-10 05:44:22.000000 meerschaum-2.2.0rc4/meerschaum/connectors/api/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5217 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/connectors/api/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6922 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc4/meerschaum/connectors/api/_request.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-2.2.0rc4/meerschaum/connectors/api/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5275 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc4/meerschaum/connectors/api/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4044 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc4/meerschaum/connectors/parse.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.862734 meerschaum-2.2.0rc4/meerschaum/connectors/plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-2.2.0rc4/meerschaum/connectors/plugin/PluginConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/connectors/plugin/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7363 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc4/meerschaum/connectors/poll.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.864735 meerschaum-2.2.0rc4/meerschaum/connectors/sql/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11709 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/connectors/sql/SQLConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc4/meerschaum/connectors/sql/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4123 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc4/meerschaum/connectors/sql/_cli.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10396 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/connectors/sql/_create_engine.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13086 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc4/meerschaum/connectors/sql/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6509 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/connectors/sql/_instance.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   101362 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/connectors/sql/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8321 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/connectors/sql/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34199 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/connectors/sql/_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3460 2023-10-26 06:22:59.000000 meerschaum-2.2.0rc4/meerschaum/connectors/sql/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10100 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc4/meerschaum/connectors/sql/_users.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.864735 meerschaum-2.2.0rc4/meerschaum/connectors/sql/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9001 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc4/meerschaum/connectors/sql/tables/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc4/meerschaum/connectors/sql/tables/types.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc4/meerschaum/connectors/sql/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.864735 meerschaum-2.2.0rc4/meerschaum/core/
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.865734 meerschaum-2.2.0rc4/meerschaum/core/Pipe/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16230 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc4/meerschaum/core/Pipe/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-2.2.0rc4/meerschaum/core/Pipe/_attributes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc4/meerschaum/core/Pipe/_bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2261 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/core/Pipe/_clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20880 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc4/meerschaum/core/Pipe/_data.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10267 2023-11-13 06:20:00.000000 meerschaum-2.2.0rc4/meerschaum/core/Pipe/_deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2118 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc4/meerschaum/core/Pipe/_delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/core/Pipe/_drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3694 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc4/meerschaum/core/Pipe/_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-2.2.0rc4/meerschaum/core/Pipe/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5234 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc4/meerschaum/core/Pipe/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-2.2.0rc4/meerschaum/core/Pipe/_register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc4/meerschaum/core/Pipe/_show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    28038 2024-05-24 04:09:22.000000 meerschaum-2.2.0rc4/meerschaum/core/Pipe/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14262 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc4/meerschaum/core/Pipe/_verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.865734 meerschaum-2.2.0rc4/meerschaum/core/Plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc4/meerschaum/core/Plugin/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.865734 meerschaum-2.2.0rc4/meerschaum/core/User/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6527 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/core/User/_User.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      193 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/core/User/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc4/meerschaum/core/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.866734 meerschaum-2.2.0rc4/meerschaum/plugins/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34039 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/plugins/_Plugin.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21866 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/plugins/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.867735 meerschaum-2.2.0rc4/meerschaum/utils/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc4/meerschaum/utils/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11460 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc4/meerschaum/utils/_get_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.868734 meerschaum-2.2.0rc4/meerschaum/utils/daemon/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34595 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/utils/daemon/Daemon.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4544 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/utils/daemon/FileDescriptorInterceptor.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23658 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/utils/daemon/RotatingFile.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8375 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/utils/daemon/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4330 2023-09-26 04:28:45.000000 meerschaum-2.2.0rc4/meerschaum/utils/daemon/_names.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31955 2024-05-24 03:15:14.000000 meerschaum-2.2.0rc4/meerschaum/utils/dataframe.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-2.2.0rc4/meerschaum/utils/debug.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.868734 meerschaum-2.2.0rc4/meerschaum/utils/dtypes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6261 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/utils/dtypes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14638 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc4/meerschaum/utils/dtypes/sql.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.868734 meerschaum-2.2.0rc4/meerschaum/utils/formatting/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13778 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc4/meerschaum/utils/formatting/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3294 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/utils/formatting/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19492 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc4/meerschaum/utils/formatting/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3096 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/utils/formatting/_pprint.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3677 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc4/meerschaum/utils/formatting/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3196 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc4/meerschaum/utils/interactive.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    43296 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc4/meerschaum/utils/misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc4/meerschaum/utils/networking.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.869734 meerschaum-2.2.0rc4/meerschaum/utils/packages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    57185 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/utils/packages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7864 2024-05-24 06:34:18.000000 meerschaum-2.2.0rc4/meerschaum/utils/packages/_packages.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-2.2.0rc4/meerschaum/utils/packages/lazy_loader.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2655 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc4/meerschaum/utils/pool.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7192 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/utils/process.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16490 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/meerschaum/utils/prompt.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10654 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/utils/schedule.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    46656 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc4/meerschaum/utils/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2489 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/utils/threading.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2807 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/meerschaum/utils/typing.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.869734 meerschaum-2.2.0rc4/meerschaum/utils/venv/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3553 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc4/meerschaum/utils/venv/_Venv.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23183 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc4/meerschaum/utils/venv/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6535 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc4/meerschaum/utils/warnings.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-2.2.0rc4/meerschaum/utils/yaml.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.870735 meerschaum-2.2.0rc4/meerschaum.egg-info/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23313 2024-05-24 06:35:22.000000 meerschaum-2.2.0rc4/meerschaum.egg-info/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8485 2024-05-24 06:35:22.000000 meerschaum-2.2.0rc4/meerschaum.egg-info/SOURCES.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-24 06:35:22.000000 meerschaum-2.2.0rc4/meerschaum.egg-info/dependency_links.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2024-05-24 06:35:22.000000 meerschaum-2.2.0rc4/meerschaum.egg-info/entry_points.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4733 2024-05-24 06:35:22.000000 meerschaum-2.2.0rc4/meerschaum.egg-info/requires.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2024-05-24 06:35:22.000000 meerschaum-2.2.0rc4/meerschaum.egg-info/top_level.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-24 06:35:22.000000 meerschaum-2.2.0rc4/meerschaum.egg-info/zip-safe
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2024-05-24 06:35:22.895734 meerschaum-2.2.0rc4/setup.cfg
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3254 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/setup.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 06:35:22.869734 meerschaum-2.2.0rc4/tests/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3139 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc4/tests/test_deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15351 2023-11-13 21:37:33.000000 meerschaum-2.2.0rc4/tests/test_pipes_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3646 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/tests/test_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21905 2024-05-24 06:27:39.000000 meerschaum-2.2.0rc4/tests/test_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      744 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/tests/test_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3090 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc4/tests/test_verify.py
```

### Comparing `meerschaum-2.2.0rc3/LICENSE` & `meerschaum-2.2.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/PKG-INFO` & `meerschaum-2.2.0rc4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 2.2.0rc3
+Version: 2.2.0rc4
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
@@ -38,48 +38,48 @@
 Requires-Dist: asciitree>=0.3.3; extra == "formatting"
 Requires-Dist: typing-extensions>=4.7.1; extra == "formatting"
 Requires-Dist: pygments>=2.7.2; extra == "formatting"
 Requires-Dist: colorama>=0.4.3; extra == "formatting"
 Requires-Dist: rich>=13.4.2; extra == "formatting"
 Requires-Dist: more-termcolor>=1.1.3; extra == "formatting"
 Requires-Dist: humanfriendly>=10.0.0; extra == "formatting"
-Provides-Extra: required
-Requires-Dist: wheel>=0.34.2; extra == "required"
-Requires-Dist: setuptools>=63.3.0; extra == "required"
-Requires-Dist: PyYAML>=5.3.1; extra == "required"
-Requires-Dist: pip>=22.0.4; extra == "required"
-Requires-Dist: update-checker>=0.18.0; extra == "required"
-Requires-Dist: semver>=3.0.0; extra == "required"
-Requires-Dist: pathspec>=0.9.0; extra == "required"
-Requires-Dist: python-dateutil>=2.7.5; extra == "required"
-Requires-Dist: requests>=2.23.0; extra == "required"
-Requires-Dist: binaryornot>=0.4.4; extra == "required"
-Requires-Dist: pyvim>=3.0.2; extra == "required"
-Requires-Dist: aiofiles>=0.6.0; extra == "required"
-Requires-Dist: packaging>=21.3.0; extra == "required"
-Requires-Dist: prompt-toolkit>=3.0.39; extra == "required"
-Requires-Dist: more-itertools>=8.7.0; extra == "required"
-Requires-Dist: python-daemon>=0.2.3; extra == "required"
-Requires-Dist: fasteners>=0.18.0; extra == "required"
-Requires-Dist: psutil>=5.8.0; extra == "required"
-Requires-Dist: watchfiles>=0.21.0; extra == "required"
-Requires-Dist: dill>=0.3.3; extra == "required"
-Requires-Dist: virtualenv>=20.1.0; extra == "required"
-Requires-Dist: APScheduler>=4.0.0a5; extra == "required"
+Provides-Extra: core
+Requires-Dist: wheel>=0.34.2; extra == "core"
+Requires-Dist: setuptools>=63.3.0; extra == "core"
+Requires-Dist: PyYAML>=5.3.1; extra == "core"
+Requires-Dist: pip>=22.0.4; extra == "core"
+Requires-Dist: update-checker>=0.18.0; extra == "core"
+Requires-Dist: semver>=3.0.0; extra == "core"
+Requires-Dist: pathspec>=0.9.0; extra == "core"
+Requires-Dist: python-dateutil>=2.7.5; extra == "core"
+Requires-Dist: requests>=2.23.0; extra == "core"
+Requires-Dist: binaryornot>=0.4.4; extra == "core"
+Requires-Dist: pyvim>=3.0.2; extra == "core"
+Requires-Dist: aiofiles>=0.6.0; extra == "core"
+Requires-Dist: packaging>=21.3.0; extra == "core"
+Requires-Dist: prompt-toolkit>=3.0.39; extra == "core"
+Requires-Dist: more-itertools>=8.7.0; extra == "core"
+Requires-Dist: python-daemon>=0.2.3; extra == "core"
+Requires-Dist: fasteners>=0.18.0; extra == "core"
+Requires-Dist: psutil>=5.8.0; extra == "core"
+Requires-Dist: watchfiles>=0.21.0; extra == "core"
+Requires-Dist: dill>=0.3.3; extra == "core"
+Requires-Dist: virtualenv>=20.1.0; extra == "core"
+Requires-Dist: APScheduler>=4.0.0a5; extra == "core"
 Provides-Extra: drivers
 Requires-Dist: cryptography>=38.0.1; extra == "drivers"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "drivers"
 Requires-Dist: PyMySQL>=0.9.0; extra == "drivers"
 Requires-Dist: aiomysql>=0.0.21; extra == "drivers"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "drivers"
-Requires-Dist: duckdb<0.10.0; extra == "drivers"
+Requires-Dist: duckdb<0.10.3; extra == "drivers"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "drivers"
-Provides-Extra: drivers
-Requires-Dist: pyodbc>=4.0.30; extra == "drivers"
-Requires-Dist: cx_Oracle>=8.3.0; extra == "drivers"
+Provides-Extra: drivers-extras
+Requires-Dist: pyodbc>=4.0.30; extra == "drivers-extras"
+Requires-Dist: cx_Oracle>=8.3.0; extra == "drivers-extras"
 Provides-Extra: cli
 Requires-Dist: pgcli>=3.1.0; extra == "cli"
 Requires-Dist: mycli>=1.23.2; extra == "cli"
 Requires-Dist: litecli>=1.5.0; extra == "cli"
 Requires-Dist: mssql-cli>=1.0.0; extra == "cli"
 Requires-Dist: gadwall>=0.2.0; extra == "cli"
 Provides-Extra: stack
@@ -129,15 +129,15 @@
 Requires-Dist: aiosqlite>=0.16.0; extra == "sql"
 Requires-Dist: asyncpg>=0.21.0; extra == "sql"
 Requires-Dist: cryptography>=38.0.1; extra == "sql"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "sql"
 Requires-Dist: PyMySQL>=0.9.0; extra == "sql"
 Requires-Dist: aiomysql>=0.0.21; extra == "sql"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "sql"
-Requires-Dist: duckdb<0.10.0; extra == "sql"
+Requires-Dist: duckdb<0.10.3; extra == "sql"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "sql"
 Requires-Dist: wheel>=0.34.2; extra == "sql"
 Requires-Dist: setuptools>=63.3.0; extra == "sql"
 Requires-Dist: PyYAML>=5.3.1; extra == "sql"
 Requires-Dist: pip>=22.0.4; extra == "sql"
 Requires-Dist: update-checker>=0.18.0; extra == "sql"
 Requires-Dist: semver>=3.0.0; extra == "sql"
@@ -186,15 +186,15 @@
 Requires-Dist: aiosqlite>=0.16.0; extra == "api"
 Requires-Dist: asyncpg>=0.21.0; extra == "api"
 Requires-Dist: cryptography>=38.0.1; extra == "api"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "api"
 Requires-Dist: PyMySQL>=0.9.0; extra == "api"
 Requires-Dist: aiomysql>=0.0.21; extra == "api"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "api"
-Requires-Dist: duckdb<0.10.0; extra == "api"
+Requires-Dist: duckdb<0.10.3; extra == "api"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "api"
 Requires-Dist: wheel>=0.34.2; extra == "api"
 Requires-Dist: setuptools>=63.3.0; extra == "api"
 Requires-Dist: PyYAML>=5.3.1; extra == "api"
 Requires-Dist: pip>=22.0.4; extra == "api"
 Requires-Dist: update-checker>=0.18.0; extra == "api"
 Requires-Dist: semver>=3.0.0; extra == "api"
@@ -262,15 +262,15 @@
 Requires-Dist: virtualenv>=20.1.0; extra == "full"
 Requires-Dist: APScheduler>=4.0.0a5; extra == "full"
 Requires-Dist: cryptography>=38.0.1; extra == "full"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "full"
 Requires-Dist: PyMySQL>=0.9.0; extra == "full"
 Requires-Dist: aiomysql>=0.0.21; extra == "full"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "full"
-Requires-Dist: duckdb<0.10.0; extra == "full"
+Requires-Dist: duckdb<0.10.3; extra == "full"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "full"
 Requires-Dist: toga>=0.3.0-dev29; extra == "full"
 Requires-Dist: pywebview>=3.6.3; extra == "full"
 Requires-Dist: pycparser>=2.21.0; extra == "full"
 Requires-Dist: numpy>=1.18.5; extra == "full"
 Requires-Dist: pandas[parquet]>=2.0.1; extra == "full"
 Requires-Dist: pyarrow>=16.1.0; extra == "full"
```

### Comparing `meerschaum-2.2.0rc3/README.md` & `meerschaum-2.2.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/__main__.py` & `meerschaum-2.2.0rc4/meerschaum/__main__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/_internal/arguments/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/_internal/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/_internal/arguments/_parse_arguments.py` & `meerschaum-2.2.0rc4/meerschaum/_internal/arguments/_parse_arguments.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/_internal/arguments/_parser.py` & `meerschaum-2.2.0rc4/meerschaum/_internal/arguments/_parser.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/_internal/docs/index.py` & `meerschaum-2.2.0rc4/meerschaum/_internal/docs/index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/_internal/entry.py` & `meerschaum-2.2.0rc4/meerschaum/_internal/entry.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/_internal/gui/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/_internal/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/_internal/gui/app/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/_windows.py` & `meerschaum-2.2.0rc4/meerschaum/_internal/gui/app/_windows.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/actions.py` & `meerschaum-2.2.0rc4/meerschaum/_internal/gui/app/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/pipes.py` & `meerschaum-2.2.0rc4/meerschaum/_internal/gui/app/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/_internal/shell/Shell.py` & `meerschaum-2.2.0rc4/meerschaum/_internal/shell/Shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/_internal/shell/ShellCompleter.py` & `meerschaum-2.2.0rc4/meerschaum/_internal/shell/ShellCompleter.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/_internal/shell/ValidAutoSuggest.py` & `meerschaum-2.2.0rc4/meerschaum/_internal/shell/ValidAutoSuggest.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/_internal/term/TermPageHandler.py` & `meerschaum-2.2.0rc4/meerschaum/_internal/term/TermPageHandler.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/_internal/term/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/_internal/term/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/_internal/term/tools.py` & `meerschaum-2.2.0rc4/meerschaum/_internal/term/tools.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/api.py` & `meerschaum-2.2.0rc4/meerschaum/actions/api.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/bootstrap.py` & `meerschaum-2.2.0rc4/meerschaum/actions/bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/clear.py` & `meerschaum-2.2.0rc4/meerschaum/actions/clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/copy.py` & `meerschaum-2.2.0rc4/meerschaum/actions/copy.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/deduplicate.py` & `meerschaum-2.2.0rc4/meerschaum/actions/deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/delete.py` & `meerschaum-2.2.0rc4/meerschaum/actions/delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/drop.py` & `meerschaum-2.2.0rc4/meerschaum/actions/drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/edit.py` & `meerschaum-2.2.0rc4/meerschaum/actions/edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/install.py` & `meerschaum-2.2.0rc4/meerschaum/actions/install.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/login.py` & `meerschaum-2.2.0rc4/meerschaum/actions/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/os.py` & `meerschaum-2.2.0rc4/meerschaum/actions/os.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/pause.py` & `meerschaum-2.2.0rc4/meerschaum/actions/pause.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/python.py` & `meerschaum-2.2.0rc4/meerschaum/actions/python.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/register.py` & `meerschaum-2.2.0rc4/meerschaum/actions/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/setup.py` & `meerschaum-2.2.0rc4/meerschaum/actions/setup.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/sh.py` & `meerschaum-2.2.0rc4/meerschaum/actions/sh.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/show.py` & `meerschaum-2.2.0rc4/meerschaum/actions/show.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,16 +585,16 @@
     from meerschaum.utils.formatting import get_console, ANSI, UNICODE
     from meerschaum.utils.misc import tail
     from meerschaum.config._paths import LOGS_RESOURCES_PATH
     from meerschaum.config import get_config
     if not ANSI:
         info = print
     colors = get_config('jobs', 'logs', 'colors')
-    timestamp_format = get_config('jobs', 'logs', 'timestamp_format')
-    follow_timestamp_format = get_config('jobs', 'logs', 'follow_timestamp_format')
+    timestamp_format = get_config('jobs', 'logs', 'timestamps', 'format')
+    follow_timestamp_format = get_config('jobs', 'logs', 'timestamps', 'follow_format')
     daemons = get_filtered_daemons(action)
     now = datetime.now(timezone.utc)
     now_str = now.strftime(timestamp_format)
     now_follow_str = now.strftime(follow_timestamp_format)
 
     def build_buffer_spaces(daemons) -> Dict[str, str]:
         max_len_id = max(len(d.daemon_id) for d in daemons) if daemons else 0
```

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/sql.py` & `meerschaum-2.2.0rc4/meerschaum/actions/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/stack.py` & `meerschaum-2.2.0rc4/meerschaum/actions/stack.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/start.py` & `meerschaum-2.2.0rc4/meerschaum/actions/start.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/stop.py` & `meerschaum-2.2.0rc4/meerschaum/actions/stop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/sync.py` & `meerschaum-2.2.0rc4/meerschaum/actions/sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/tag.py` & `meerschaum-2.2.0rc4/meerschaum/actions/tag.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/uninstall.py` & `meerschaum-2.2.0rc4/meerschaum/actions/uninstall.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/upgrade.py` & `meerschaum-2.2.0rc4/meerschaum/actions/upgrade.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/actions/verify.py` & `meerschaum-2.2.0rc4/meerschaum/actions/verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,22 +42,27 @@
     'aiofiles',
     'starlette.responses',
     'multipart',
     'packaging.version',
     lazy = False,
     check_update = CHECK_UPDATE,
 )
-typing_extensions = attempt_import(
-    'typing_extensions', lazy=False, check_update=CHECK_UPDATE,
+(
+    typing_extensions,
+    uvicorn_workers,
+) = attempt_import(
+    'typing_extensions',
+    'uvicorn.workers',
+    lazy = False,
+    check_update = CHECK_UPDATE,
     venv = None,
 )
 from meerschaum.api._chain import check_allow_chaining, DISALLOW_CHAINING_MESSAGE
 uvicorn_config_path = API_UVICORN_RESOURCES_PATH / SERVER_ID / 'config.json'
 
-uvicorn_workers = attempt_import('uvicorn.workers', venv=None, check_update=CHECK_UPDATE)
 uvicorn_config = None
 sys_config = get_config('system', 'api')
 permissions_config = get_config('system', 'api', 'permissions')
 
 def get_uvicorn_config() -> Dict[str, Any]:
     """Read the Uvicorn configuration JSON and return a dictionary."""
     global uvicorn_config
```

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/_chain.py` & `meerschaum-2.2.0rc4/meerschaum/api/_chain.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/_events.py` & `meerschaum-2.2.0rc4/meerschaum/api/_events.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/_websockets.py` & `meerschaum-2.2.0rc4/meerschaum/api/_websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/actions.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/assets/ansi_up.js` & `meerschaum-2.2.0rc4/meerschaum/api/dash/assets/ansi_up.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/assets/banner_1920x320.png` & `meerschaum-2.2.0rc4/meerschaum/api/dash/assets/banner_1920x320.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/assets/favicon.ico` & `meerschaum-2.2.0rc4/meerschaum/api/dash/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/assets/logo_48x48.png` & `meerschaum-2.2.0rc4/meerschaum/api/dash/assets/logo_48x48.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/assets/logo_500x500.png` & `meerschaum-2.2.0rc4/meerschaum/api/dash/assets/logo_500x500.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/dashboard.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/callbacks/dashboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -709,19 +709,19 @@
         raise PreventUpdate
     ctx = dash.callback_context.triggered
     if ctx[0]['value'] is None:
         raise PreventUpdate
     pipe = pipe_from_ctx(ctx, 'n_clicks')
     if pipe is None:
         raise PreventUpdate
-    filename = str(pipe.target) + '.csv'
     bounds = pipe.get_chunk_bounds(bounded=True, debug=debug)
-    begin, _ = bounds[-1]
+    begin, end = bounds[-1]
+    filename = str(pipe.target) + f" {begin} - {end}.csv"
     try:
-        df = pipe.get_data(begin=begin, end=None, debug=debug)
+        df = pipe.get_data(begin=begin, end=end, debug=debug)
     except Exception as e:
         df = None
     if df is not None:
         return dcc.send_data_frame(df.to_csv, filename, index=False)
     raise PreventUpdate
```

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/jobs.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/callbacks/jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/login.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/callbacks/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/plugins.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/callbacks/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/register.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/components.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/components.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/connectors.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/graphs.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/graphs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/jobs.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/keys.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             children = [
                 dbc.Col(
                     html.Div(
                         dcc.Dropdown(
                             id = 'flags-dropdown',
                             multi = True,
                             placeholder = 'Boolean flags',
-                            options = [],
+                            options = ['--yes'],
                             value = ['--yes'],
                         ),
                         id = 'flags-dropdown-div',
                         className = 'dbc_dark input-text',
                     ),
                     width = widths['flags'],
                 ),
```

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/pages/dashboard.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/pages/dashboard.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,30 @@
 """
 
 import uuid
 from meerschaum.config import __doc__ as doc, get_config
 from meerschaum.utils.misc import get_connector_labels
 from meerschaum.utils.packages import attempt_import, import_html, import_dcc, import_pandas
 from meerschaum.api import endpoints, CHECK_UPDATE
-dex = attempt_import('dash_extensions', lazy=False, check_update=CHECK_UPDATE)
-dbc = attempt_import('dash_bootstrap_components', lazy=False, check_update=CHECK_UPDATE)
+(
+    dex,
+    px,
+    daq,
+    dbc,
+) = attempt_import(
+    'dash_extensions',
+    'plotly.express',
+    'dash_daq',
+    'dash_bootstrap_components',
+    lazy = False,
+    warn = False,
+    check_update = CHECK_UPDATE,
+)
 html, dcc = import_html(check_update=CHECK_UPDATE), import_dcc(check_update=CHECK_UPDATE)
 pd = import_pandas(check_update=CHECK_UPDATE)
-px = attempt_import('plotly.express', warn=False, check_update=CHECK_UPDATE)
-daq = attempt_import('dash_daq', warn=False, check_update=CHECK_UPDATE)
 
 from meerschaum.api.dash.components import (
     go_button,
     search_parameters_editor,
     test_button,
     get_items_menu,
     bottom_buttons_content,
```

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/pages/error.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/pages/error.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/pages/login.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/pages/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/pages/plugins.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/pages/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/pages/register.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/pages/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/pipes.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/plugins.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/users.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/websockets.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/dash/webterm.py` & `meerschaum-2.2.0rc4/meerschaum/api/dash/webterm.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/bootstrap.min.css` & `meerschaum-2.2.0rc4/meerschaum/api/resources/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/dash.css` & `meerschaum-2.2.0rc4/meerschaum/api/resources/static/css/dash.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/dbc_dark.css` & `meerschaum-2.2.0rc4/meerschaum/api/resources/static/css/dbc_dark.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/xterm.css` & `meerschaum-2.2.0rc4/meerschaum/api/resources/static/css/xterm.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/resources/static/ico/logo.ico` & `meerschaum-2.2.0rc4/meerschaum/api/resources/static/ico/logo.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/action_button.js` & `meerschaum-2.2.0rc4/meerschaum/api/resources/static/js/action_button.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/terminado.js` & `meerschaum-2.2.0rc4/meerschaum/api/resources/static/js/terminado.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/xterm.js` & `meerschaum-2.2.0rc4/meerschaum/api/resources/static/js/xterm.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/resources/templates/index.html` & `meerschaum-2.2.0rc4/meerschaum/api/resources/templates/index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/resources/templates/old_index.html` & `meerschaum-2.2.0rc4/meerschaum/api/resources/templates/old_index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/resources/templates/termpage.html` & `meerschaum-2.2.0rc4/meerschaum/api/resources/templates/termpage.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/routes/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/api/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/routes/_actions.py` & `meerschaum-2.2.0rc4/meerschaum/api/routes/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/routes/_connectors.py` & `meerschaum-2.2.0rc4/meerschaum/api/routes/_connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/routes/_index.py` & `meerschaum-2.2.0rc4/meerschaum/api/routes/_index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/routes/_login.py` & `meerschaum-2.2.0rc4/meerschaum/api/routes/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/routes/_misc.py` & `meerschaum-2.2.0rc4/meerschaum/api/routes/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/routes/_pipes.py` & `meerschaum-2.2.0rc4/meerschaum/api/routes/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/routes/_plugins.py` & `meerschaum-2.2.0rc4/meerschaum/api/routes/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/routes/_users.py` & `meerschaum-2.2.0rc4/meerschaum/api/routes/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/routes/_version.py` & `meerschaum-2.2.0rc4/meerschaum/api/routes/_version.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/api/routes/_webterm.py` & `meerschaum-2.2.0rc4/meerschaum/api/routes/_webterm.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/config/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/config/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/config/_default.py` & `meerschaum-2.2.0rc4/meerschaum/config/_default.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/config/_edit.py` & `meerschaum-2.2.0rc4/meerschaum/config/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/config/_environment.py` & `meerschaum-2.2.0rc4/meerschaum/config/_environment.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/config/_formatting.py` & `meerschaum-2.2.0rc4/meerschaum/config/_formatting.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/config/_jobs.py` & `meerschaum-2.2.0rc4/meerschaum/config/_jobs.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,21 +10,24 @@
     'timeout_seconds': 8,
     'check_timeout_interval_seconds': 0.1,
     'terminal': {
         'lines': 40,
         'columns': 70,
     },
     'logs': {
+        'timestamps': {
+            'enabled': True,
+            'format': '%Y-%m-%d %H:%M',
+            'follow_format': '%H:%M',
+        },
         'num_files_to_keep': 5,
         'max_file_size': 100_000,
         'lines_to_show': 30,
         'refresh_files_seconds': 5,
         'min_buffer_len': 5,
-        'timestamp_format': '%Y-%m-%d %H:%M',
-        'follow_timestamp_format': '%H:%M',
         'colors': [
             'cyan',
             'magenta',
             'orange3',
             'green',
             'blue',
             'red',
```

### Comparing `meerschaum-2.2.0rc3/meerschaum/config/_patch.py` & `meerschaum-2.2.0rc4/meerschaum/config/_patch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/config/_paths.py` & `meerschaum-2.2.0rc4/meerschaum/config/_paths.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/config/_preprocess.py` & `meerschaum-2.2.0rc4/meerschaum/config/_preprocess.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/config/_read_config.py` & `meerschaum-2.2.0rc4/meerschaum/config/_read_config.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/config/_shell.py` & `meerschaum-2.2.0rc4/meerschaum/config/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/config/_sync.py` & `meerschaum-2.2.0rc4/meerschaum/config/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/config/stack/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/config/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/config/stack/grafana/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/config/stack/grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/config/static/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/config/static/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/Connector.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/Connector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/api/APIConnector.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/api/APIConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/api/_actions.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/api/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/api/_fetch.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/api/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/api/_login.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/api/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/api/_misc.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/api/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/api/_pipes.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/api/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/api/_plugins.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/api/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/api/_request.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/api/_request.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/api/_uri.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/api/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/api/_users.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/api/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/parse.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/parse.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/plugin/PluginConnector.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/plugin/PluginConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/poll.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/poll.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/sql/SQLConnector.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/sql/SQLConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_cli.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/sql/_cli.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_create_engine.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/sql/_create_engine.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_fetch.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/sql/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_instance.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/sql/_instance.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_pipes.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/sql/_pipes.py`

 * *Files 0% similar despite different names*

```diff
@@ -759,14 +759,15 @@
 
     numeric_columns = [
         col
         for col, typ in pipe.dtypes.items()
         if typ == 'numeric' and col in dtypes
     ]
     kw['coerce_float'] = kw.get('coerce_float', (len(numeric_columns) == 0))
+    
     df = self.read(
         query,
         dtype = dtypes,
         debug = debug,
         **kw
     )
     for col in numeric_columns:
```

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_plugins.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/sql/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_sql.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/sql/_sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_uri.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/sql/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_users.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/sql/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/sql/tables/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/sql/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/connectors/sql/tables/types.py` & `meerschaum-2.2.0rc4/meerschaum/connectors/sql/tables/types.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/core/Pipe/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/core/Pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_attributes.py` & `meerschaum-2.2.0rc4/meerschaum/core/Pipe/_attributes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_bootstrap.py` & `meerschaum-2.2.0rc4/meerschaum/core/Pipe/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_clear.py` & `meerschaum-2.2.0rc4/meerschaum/core/Pipe/_clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_data.py` & `meerschaum-2.2.0rc4/meerschaum/core/Pipe/_data.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_deduplicate.py` & `meerschaum-2.2.0rc4/meerschaum/core/Pipe/_deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_delete.py` & `meerschaum-2.2.0rc4/meerschaum/core/Pipe/_delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_drop.py` & `meerschaum-2.2.0rc4/meerschaum/core/Pipe/_drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_dtypes.py` & `meerschaum-2.2.0rc4/meerschaum/core/Pipe/_dtypes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_edit.py` & `meerschaum-2.2.0rc4/meerschaum/core/Pipe/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_fetch.py` & `meerschaum-2.2.0rc4/meerschaum/core/Pipe/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_register.py` & `meerschaum-2.2.0rc4/meerschaum/core/Pipe/_register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_show.py` & `meerschaum-2.2.0rc4/meerschaum/core/Pipe/_show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_sync.py` & `meerschaum-2.2.0rc4/meerschaum/core/Pipe/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_verify.py` & `meerschaum-2.2.0rc4/meerschaum/core/Pipe/_verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/core/User/_User.py` & `meerschaum-2.2.0rc4/meerschaum/core/User/_User.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/plugins/_Plugin.py` & `meerschaum-2.2.0rc4/meerschaum/plugins/_Plugin.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/plugins/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/_get_pipes.py` & `meerschaum-2.2.0rc4/meerschaum/utils/_get_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/daemon/Daemon.py` & `meerschaum-2.2.0rc4/meerschaum/utils/daemon/Daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -680,30 +680,31 @@
     def rotating_log(self) -> RotatingFile:
         if '_rotating_log' in self.__dict__:
             return self._rotating_log
 
         self._rotating_log = RotatingFile(
             self.log_path,
             redirect_streams = True,
-            write_timestamps = True,
-            timestamp_format = get_config('jobs', 'logs', 'timestamp_format'),
+            write_timestamps = get_config('jobs', 'logs', 'timestamps', 'enabled'),
+            timestamp_format = get_config('jobs', 'logs', 'timestamps', 'format'),
         )
         return self._rotating_log
 
 
     @property
     def log_text(self) -> Optional[str]:
         """Read the log files and return their contents.
         Returns `None` if the log file does not exist.
         """
         new_rotating_log = RotatingFile(
             self.rotating_log.file_path,
             num_files_to_keep = self.rotating_log.num_files_to_keep,
             max_file_size = self.rotating_log.max_file_size,
-            write_timestamps = True,
+            write_timestamps = get_config('jobs', 'logs', 'timestamps', 'enabled'),
+            timestamp_format = get_config('jobs', 'logs', 'timestamps', 'format'),
         )
         return new_rotating_log.read()
 
 
     def readlines(self) -> List[str]:
         """
         Read the next log lines, persisting the cursor for later use.
```

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/daemon/FileDescriptorInterceptor.py` & `meerschaum-2.2.0rc4/meerschaum/utils/daemon/FileDescriptorInterceptor.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/daemon/RotatingFile.py` & `meerschaum-2.2.0rc4/meerschaum/utils/daemon/RotatingFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,15 @@
                 try:
                     daemon.daemon.redirect_stream(sys.stdout, self._current_file_obj)
                     daemon.daemon.redirect_stream(sys.stderr, self._current_file_obj)
                 except OSError as e:
                     warn(
                         f"Encountered an issue when redirecting streams:\n{traceback.format_exc()}"
                     )
-                if start_interception:
+                if start_interception and self.write_timestamps:
                     self.start_log_fd_interception()
 
         create_new_file = (
             (latest_subfile_index == -1)
             or
             self._current_file_obj is None
             or
@@ -359,15 +359,15 @@
         if isinstance(data, bytes):
             data = data.decode('utf-8')
 
         prefix_str = self.get_timestamp_prefix_str() if self.write_timestamps else ""
         suffix_str = "\n" if self.write_timestamps else ""
         self.refresh_files(
             potential_new_len = len(prefix_str + data + suffix_str),
-            start_interception = True,
+            start_interception = self.write_timestamps,
         )
         try:
             if prefix_str:
                 self._current_file_obj.write(prefix_str)
             self._current_file_obj.write(data)
             if suffix_str:
                 self._current_file_obj.write(suffix_str)
@@ -587,14 +587,17 @@
                 warn(f"Failed to flush STDERR:\n{traceback.format_exc()}")
 
 
     def start_log_fd_interception(self):
         """
         Start the file descriptor monitoring threads.
         """
+        if not self.write_timestamps:
+            return
+
         threads = self.__dict__.get('_interceptor_threads', [])
         self._stdout_interceptor = FileDescriptorInterceptor(
             sys.stdout.fileno(),
             self.get_timestamp_prefix_str,
         )
         self._stderr_interceptor = FileDescriptorInterceptor(
             sys.stderr.fileno(),
@@ -623,18 +626,21 @@
         ])
         self._interceptors.extend([
             self._stdout_interceptor,
             self._stderr_interceptor,
         ])
         self.stop_log_fd_interception(unused_only=True)
 
+
     def stop_log_fd_interception(self, unused_only: bool = False):
         """
         Stop the file descriptor monitoring threads.
         """
+        if not self.write_timestamps:
+            return
         interceptors = self.__dict__.get('_interceptors', [])
         interceptor_threads = self.__dict__.get('_interceptor_threads', [])
 
         end_ix = len(interceptors) if not unused_only else -2
 
         for interceptor in interceptors[:end_ix]:
             interceptor.stop_interception()
```

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/daemon/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/utils/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/daemon/_names.py` & `meerschaum-2.2.0rc4/meerschaum/utils/daemon/_names.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/dataframe.py` & `meerschaum-2.2.0rc4/meerschaum/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/debug.py` & `meerschaum-2.2.0rc4/meerschaum/utils/debug.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/dtypes/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/utils/dtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/dtypes/sql.py` & `meerschaum-2.2.0rc4/meerschaum/utils/dtypes/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/formatting/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/utils/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/formatting/_jobs.py` & `meerschaum-2.2.0rc4/meerschaum/utils/formatting/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/formatting/_pipes.py` & `meerschaum-2.2.0rc4/meerschaum/utils/formatting/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/formatting/_pprint.py` & `meerschaum-2.2.0rc4/meerschaum/utils/formatting/_pprint.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/formatting/_shell.py` & `meerschaum-2.2.0rc4/meerschaum/utils/formatting/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/interactive.py` & `meerschaum-2.2.0rc4/meerschaum/utils/interactive.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/misc.py` & `meerschaum-2.2.0rc4/meerschaum/utils/misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/networking.py` & `meerschaum-2.2.0rc4/meerschaum/utils/networking.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/packages/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/utils/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/packages/_packages.py` & `meerschaum-2.2.0rc4/meerschaum/utils/packages/_packages.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         'typing_extensions'          : 'typing-extensions>=4.7.1',
         'pygments'                   : 'pygments>=2.7.2',
         'colorama'                   : 'colorama>=0.4.3',
         'rich'                       : 'rich>=13.4.2',
         'more_termcolor'             : 'more-termcolor>=1.1.3',
         'humanfriendly'              : 'humanfriendly>=10.0.0',
     },
-    '_required': {
+    'core': {
         'wheel'                      : 'wheel>=0.34.2',
         'setuptools'                 : 'setuptools>=63.3.0',
         'yaml'                       : 'PyYAML>=5.3.1',
         'pip'                        : 'pip>=22.0.4',
         'update_checker'             : 'update-checker>=0.18.0',
         'semver'                     : 'semver>=3.0.0',
         'pathspec'                   : 'pathspec>=0.9.0',
@@ -56,18 +56,18 @@
     },
     'drivers': {
         'cryptography'               : 'cryptography>=38.0.1',
         'psycopg'                    : 'psycopg[binary]>=3.1.18',
         'pymysql'                    : 'PyMySQL>=0.9.0',
         'aiomysql'                   : 'aiomysql>=0.0.21',
         'sqlalchemy_cockroachdb'     : 'sqlalchemy-cockroachdb>=2.0.0',
-        'duckdb'                     : 'duckdb<0.10.0',
+        'duckdb'                     : 'duckdb<0.10.3',
         'duckdb_engine'              : 'duckdb-engine>=0.9.2',
     },
-    '_drivers': {
+    'drivers-extras': {
         'pyodbc'                     : 'pyodbc>=4.0.30',
         'cx_Oracle'                  : 'cx_Oracle>=8.3.0',
     },
     'cli': {
         'pgcli'                      : 'pgcli>=3.1.0',
         'mycli'                      : 'mycli>=1.23.2',
         'litecli'                    : 'litecli>=1.5.0',
@@ -126,15 +126,15 @@
     'joblib'                         : 'joblib>=0.17.0',
     'sqlalchemy'                     : 'SQLAlchemy>=2.0.5',
     'databases'                      : 'databases>=0.4.0',
     'aiosqlite'                      : 'aiosqlite>=0.16.0',
     'asyncpg'                        : 'asyncpg>=0.21.0',
 }
 packages['sql'].update(packages['drivers'])
-packages['sql'].update(packages['_required'])
+packages['sql'].update(packages['core'])
 packages['dash'] = {
     'flask_compress'                 : 'Flask-Compress>=1.10.1',
     'dash'                           : 'dash>=2.6.2',
     'dash_bootstrap_components'      : 'dash-bootstrap-components>=1.2.1',
     'dash_ace'                       : 'dash-ace>=0.2.1',
     'dash_extensions'                : 'dash-extensions>=1.0.4',
     'dash_daq'                       : 'dash-daq>=0.5.0',
@@ -146,15 +146,14 @@
     'gunicorn'                       : 'gunicorn>=22.0.0',
     'dotenv'                         : 'python-dotenv>=0.20.0',
     'websockets'                     : 'websockets>=11.0.3',
     'fastapi'                        : 'fastapi>=0.111.0',
     'fastapi_login'                  : 'fastapi-login>=1.7.2',
     'multipart'                      : 'python-multipart>=0.0.9',
     'httpx'                          : 'httpx>=0.24.1',
-    'websockets'                     : 'websockets>=11.0.3',
 }
 packages['api'].update(packages['sql'])
 packages['api'].update(packages['formatting'])
 packages['api'].update(packages['dash'])
 
 all_packages = {}
 for group, import_names in packages.items():
@@ -166,15 +165,15 @@
     """
     if not install_names:
         from meerschaum.utils.packages import get_install_no_version
         for _import_name, _install_name in all_packages.items():
             install_names[get_install_no_version(_install_name)] = _import_name
     return install_names
 
-skip_groups = {'docs', 'build', 'cli', 'dev-tools', 'portable', 'extras', 'stack', '_drivers'}
+skip_groups = {'docs', 'build', 'cli', 'dev-tools', 'portable', 'extras', 'stack', 'drivers-extras'}
 full = []
 _full = {}
 for group, import_names in packages.items():
     ### omit 'cli' and 'docs' from 'full'
     if group in skip_groups:
         continue
     full += [ install_name for import_name, install_name in import_names.items() ]
```

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/packages/lazy_loader.py` & `meerschaum-2.2.0rc4/meerschaum/utils/packages/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/pool.py` & `meerschaum-2.2.0rc4/meerschaum/utils/pool.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/process.py` & `meerschaum-2.2.0rc4/meerschaum/utils/process.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/prompt.py` & `meerschaum-2.2.0rc4/meerschaum/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/schedule.py` & `meerschaum-2.2.0rc4/meerschaum/utils/schedule.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/sql.py` & `meerschaum-2.2.0rc4/meerschaum/utils/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/threading.py` & `meerschaum-2.2.0rc4/meerschaum/utils/threading.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/typing.py` & `meerschaum-2.2.0rc4/meerschaum/utils/typing.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/venv/_Venv.py` & `meerschaum-2.2.0rc4/meerschaum/utils/venv/_Venv.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/venv/__init__.py` & `meerschaum-2.2.0rc4/meerschaum/utils/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/warnings.py` & `meerschaum-2.2.0rc4/meerschaum/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum/utils/yaml.py` & `meerschaum-2.2.0rc4/meerschaum/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum.egg-info/PKG-INFO` & `meerschaum-2.2.0rc4/meerschaum.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 2.2.0rc3
+Version: 2.2.0rc4
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
@@ -38,48 +38,48 @@
 Requires-Dist: asciitree>=0.3.3; extra == "formatting"
 Requires-Dist: typing-extensions>=4.7.1; extra == "formatting"
 Requires-Dist: pygments>=2.7.2; extra == "formatting"
 Requires-Dist: colorama>=0.4.3; extra == "formatting"
 Requires-Dist: rich>=13.4.2; extra == "formatting"
 Requires-Dist: more-termcolor>=1.1.3; extra == "formatting"
 Requires-Dist: humanfriendly>=10.0.0; extra == "formatting"
-Provides-Extra: required
-Requires-Dist: wheel>=0.34.2; extra == "required"
-Requires-Dist: setuptools>=63.3.0; extra == "required"
-Requires-Dist: PyYAML>=5.3.1; extra == "required"
-Requires-Dist: pip>=22.0.4; extra == "required"
-Requires-Dist: update-checker>=0.18.0; extra == "required"
-Requires-Dist: semver>=3.0.0; extra == "required"
-Requires-Dist: pathspec>=0.9.0; extra == "required"
-Requires-Dist: python-dateutil>=2.7.5; extra == "required"
-Requires-Dist: requests>=2.23.0; extra == "required"
-Requires-Dist: binaryornot>=0.4.4; extra == "required"
-Requires-Dist: pyvim>=3.0.2; extra == "required"
-Requires-Dist: aiofiles>=0.6.0; extra == "required"
-Requires-Dist: packaging>=21.3.0; extra == "required"
-Requires-Dist: prompt-toolkit>=3.0.39; extra == "required"
-Requires-Dist: more-itertools>=8.7.0; extra == "required"
-Requires-Dist: python-daemon>=0.2.3; extra == "required"
-Requires-Dist: fasteners>=0.18.0; extra == "required"
-Requires-Dist: psutil>=5.8.0; extra == "required"
-Requires-Dist: watchfiles>=0.21.0; extra == "required"
-Requires-Dist: dill>=0.3.3; extra == "required"
-Requires-Dist: virtualenv>=20.1.0; extra == "required"
-Requires-Dist: APScheduler>=4.0.0a5; extra == "required"
+Provides-Extra: core
+Requires-Dist: wheel>=0.34.2; extra == "core"
+Requires-Dist: setuptools>=63.3.0; extra == "core"
+Requires-Dist: PyYAML>=5.3.1; extra == "core"
+Requires-Dist: pip>=22.0.4; extra == "core"
+Requires-Dist: update-checker>=0.18.0; extra == "core"
+Requires-Dist: semver>=3.0.0; extra == "core"
+Requires-Dist: pathspec>=0.9.0; extra == "core"
+Requires-Dist: python-dateutil>=2.7.5; extra == "core"
+Requires-Dist: requests>=2.23.0; extra == "core"
+Requires-Dist: binaryornot>=0.4.4; extra == "core"
+Requires-Dist: pyvim>=3.0.2; extra == "core"
+Requires-Dist: aiofiles>=0.6.0; extra == "core"
+Requires-Dist: packaging>=21.3.0; extra == "core"
+Requires-Dist: prompt-toolkit>=3.0.39; extra == "core"
+Requires-Dist: more-itertools>=8.7.0; extra == "core"
+Requires-Dist: python-daemon>=0.2.3; extra == "core"
+Requires-Dist: fasteners>=0.18.0; extra == "core"
+Requires-Dist: psutil>=5.8.0; extra == "core"
+Requires-Dist: watchfiles>=0.21.0; extra == "core"
+Requires-Dist: dill>=0.3.3; extra == "core"
+Requires-Dist: virtualenv>=20.1.0; extra == "core"
+Requires-Dist: APScheduler>=4.0.0a5; extra == "core"
 Provides-Extra: drivers
 Requires-Dist: cryptography>=38.0.1; extra == "drivers"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "drivers"
 Requires-Dist: PyMySQL>=0.9.0; extra == "drivers"
 Requires-Dist: aiomysql>=0.0.21; extra == "drivers"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "drivers"
-Requires-Dist: duckdb<0.10.0; extra == "drivers"
+Requires-Dist: duckdb<0.10.3; extra == "drivers"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "drivers"
-Provides-Extra: drivers
-Requires-Dist: pyodbc>=4.0.30; extra == "drivers"
-Requires-Dist: cx_Oracle>=8.3.0; extra == "drivers"
+Provides-Extra: drivers-extras
+Requires-Dist: pyodbc>=4.0.30; extra == "drivers-extras"
+Requires-Dist: cx_Oracle>=8.3.0; extra == "drivers-extras"
 Provides-Extra: cli
 Requires-Dist: pgcli>=3.1.0; extra == "cli"
 Requires-Dist: mycli>=1.23.2; extra == "cli"
 Requires-Dist: litecli>=1.5.0; extra == "cli"
 Requires-Dist: mssql-cli>=1.0.0; extra == "cli"
 Requires-Dist: gadwall>=0.2.0; extra == "cli"
 Provides-Extra: stack
@@ -129,15 +129,15 @@
 Requires-Dist: aiosqlite>=0.16.0; extra == "sql"
 Requires-Dist: asyncpg>=0.21.0; extra == "sql"
 Requires-Dist: cryptography>=38.0.1; extra == "sql"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "sql"
 Requires-Dist: PyMySQL>=0.9.0; extra == "sql"
 Requires-Dist: aiomysql>=0.0.21; extra == "sql"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "sql"
-Requires-Dist: duckdb<0.10.0; extra == "sql"
+Requires-Dist: duckdb<0.10.3; extra == "sql"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "sql"
 Requires-Dist: wheel>=0.34.2; extra == "sql"
 Requires-Dist: setuptools>=63.3.0; extra == "sql"
 Requires-Dist: PyYAML>=5.3.1; extra == "sql"
 Requires-Dist: pip>=22.0.4; extra == "sql"
 Requires-Dist: update-checker>=0.18.0; extra == "sql"
 Requires-Dist: semver>=3.0.0; extra == "sql"
@@ -186,15 +186,15 @@
 Requires-Dist: aiosqlite>=0.16.0; extra == "api"
 Requires-Dist: asyncpg>=0.21.0; extra == "api"
 Requires-Dist: cryptography>=38.0.1; extra == "api"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "api"
 Requires-Dist: PyMySQL>=0.9.0; extra == "api"
 Requires-Dist: aiomysql>=0.0.21; extra == "api"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "api"
-Requires-Dist: duckdb<0.10.0; extra == "api"
+Requires-Dist: duckdb<0.10.3; extra == "api"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "api"
 Requires-Dist: wheel>=0.34.2; extra == "api"
 Requires-Dist: setuptools>=63.3.0; extra == "api"
 Requires-Dist: PyYAML>=5.3.1; extra == "api"
 Requires-Dist: pip>=22.0.4; extra == "api"
 Requires-Dist: update-checker>=0.18.0; extra == "api"
 Requires-Dist: semver>=3.0.0; extra == "api"
@@ -262,15 +262,15 @@
 Requires-Dist: virtualenv>=20.1.0; extra == "full"
 Requires-Dist: APScheduler>=4.0.0a5; extra == "full"
 Requires-Dist: cryptography>=38.0.1; extra == "full"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "full"
 Requires-Dist: PyMySQL>=0.9.0; extra == "full"
 Requires-Dist: aiomysql>=0.0.21; extra == "full"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "full"
-Requires-Dist: duckdb<0.10.0; extra == "full"
+Requires-Dist: duckdb<0.10.3; extra == "full"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "full"
 Requires-Dist: toga>=0.3.0-dev29; extra == "full"
 Requires-Dist: pywebview>=3.6.3; extra == "full"
 Requires-Dist: pycparser>=2.21.0; extra == "full"
 Requires-Dist: numpy>=1.18.5; extra == "full"
 Requires-Dist: pandas[parquet]>=2.0.1; extra == "full"
 Requires-Dist: pyarrow>=16.1.0; extra == "full"
```

### Comparing `meerschaum-2.2.0rc3/meerschaum.egg-info/SOURCES.txt` & `meerschaum-2.2.0rc4/meerschaum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/meerschaum.egg-info/requires.txt` & `meerschaum-2.2.0rc4/meerschaum.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,8 @@
 
-[_drivers]
-pyodbc>=4.0.30
-cx_Oracle>=8.3.0
-
-[_required]
-wheel>=0.34.2
-setuptools>=63.3.0
-PyYAML>=5.3.1
-pip>=22.0.4
-update-checker>=0.18.0
-semver>=3.0.0
-pathspec>=0.9.0
-python-dateutil>=2.7.5
-requests>=2.23.0
-binaryornot>=0.4.4
-pyvim>=3.0.2
-aiofiles>=0.6.0
-packaging>=21.3.0
-prompt-toolkit>=3.0.39
-more-itertools>=8.7.0
-python-daemon>=0.2.3
-fasteners>=0.18.0
-psutil>=5.8.0
-watchfiles>=0.21.0
-dill>=0.3.3
-virtualenv>=20.1.0
-APScheduler>=4.0.0a5
-
 [api]
 uvicorn[standard]>=0.29.0
 gunicorn>=22.0.0
 python-dotenv>=0.20.0
 websockets>=11.0.3
 fastapi>=0.111.0
 fastapi-login>=1.7.2
@@ -47,15 +19,15 @@
 aiosqlite>=0.16.0
 asyncpg>=0.21.0
 cryptography>=38.0.1
 psycopg[binary]>=3.1.18
 PyMySQL>=0.9.0
 aiomysql>=0.0.21
 sqlalchemy-cockroachdb>=2.0.0
-duckdb<0.10.0
+duckdb<0.10.3
 duckdb-engine>=0.9.2
 wheel>=0.34.2
 setuptools>=63.3.0
 PyYAML>=5.3.1
 pip>=22.0.4
 update-checker>=0.18.0
 semver>=3.0.0
@@ -99,14 +71,38 @@
 [cli]
 pgcli>=3.1.0
 mycli>=1.23.2
 litecli>=1.5.0
 mssql-cli>=1.0.0
 gadwall>=0.2.0
 
+[core]
+wheel>=0.34.2
+setuptools>=63.3.0
+PyYAML>=5.3.1
+pip>=22.0.4
+update-checker>=0.18.0
+semver>=3.0.0
+pathspec>=0.9.0
+python-dateutil>=2.7.5
+requests>=2.23.0
+binaryornot>=0.4.4
+pyvim>=3.0.2
+aiofiles>=0.6.0
+packaging>=21.3.0
+prompt-toolkit>=3.0.39
+more-itertools>=8.7.0
+python-daemon>=0.2.3
+fasteners>=0.18.0
+psutil>=5.8.0
+watchfiles>=0.21.0
+dill>=0.3.3
+virtualenv>=20.1.0
+APScheduler>=4.0.0a5
+
 [dash]
 Flask-Compress>=1.10.1
 dash>=2.6.2
 dash-bootstrap-components>=1.2.1
 dash-ace>=0.2.1
 dash-extensions>=1.0.4
 dash-daq>=0.5.0
@@ -136,17 +132,21 @@
 
 [drivers]
 cryptography>=38.0.1
 psycopg[binary]>=3.1.18
 PyMySQL>=0.9.0
 aiomysql>=0.0.21
 sqlalchemy-cockroachdb>=2.0.0
-duckdb<0.10.0
+duckdb<0.10.3
 duckdb-engine>=0.9.2
 
+[drivers-extras]
+pyodbc>=4.0.30
+cx_Oracle>=8.3.0
+
 [extras]
 cmd2>=1.4.0
 ruamel.yaml>=0.16.12
 modin[ray]>=0.8.3
 nanoid>=2.0.0
 importlib-metadata>=4.12.0
 
@@ -192,15 +192,15 @@
 virtualenv>=20.1.0
 APScheduler>=4.0.0a5
 cryptography>=38.0.1
 psycopg[binary]>=3.1.18
 PyMySQL>=0.9.0
 aiomysql>=0.0.21
 sqlalchemy-cockroachdb>=2.0.0
-duckdb<0.10.0
+duckdb<0.10.3
 duckdb-engine>=0.9.2
 toga>=0.3.0-dev29
 pywebview>=3.6.3
 pycparser>=2.21.0
 numpy>=1.18.5
 pandas[parquet]>=2.0.1
 pyarrow>=16.1.0
@@ -251,15 +251,15 @@
 aiosqlite>=0.16.0
 asyncpg>=0.21.0
 cryptography>=38.0.1
 psycopg[binary]>=3.1.18
 PyMySQL>=0.9.0
 aiomysql>=0.0.21
 sqlalchemy-cockroachdb>=2.0.0
-duckdb<0.10.0
+duckdb<0.10.3
 duckdb-engine>=0.9.2
 wheel>=0.34.2
 setuptools>=63.3.0
 PyYAML>=5.3.1
 pip>=22.0.4
 update-checker>=0.18.0
 semver>=3.0.0
```

### Comparing `meerschaum-2.2.0rc3/setup.py` & `meerschaum-2.2.0rc4/setup.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/tests/test_deduplicate.py` & `meerschaum-2.2.0rc4/tests/test_deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/tests/test_pipes_dtypes.py` & `meerschaum-2.2.0rc4/tests/test_pipes_dtypes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/tests/test_sql.py` & `meerschaum-2.2.0rc4/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/tests/test_sync.py` & `meerschaum-2.2.0rc4/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/tests/test_users.py` & `meerschaum-2.2.0rc4/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc3/tests/test_verify.py` & `meerschaum-2.2.0rc4/tests/test_verify.py`

 * *Files identical despite different names*

