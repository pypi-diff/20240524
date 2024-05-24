# Comparing `tmp/meerschaum-2.2.0rc2.tar.gz` & `tmp/meerschaum-2.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meerschaum-2.2.0rc2.tar", last modified: Wed May 22 22:01:38 2024, max compression
+gzip compressed data, was "meerschaum-2.2.0rc3.tar", last modified: Fri May 24 03:17:02 2024, max compression
```

## Comparing `meerschaum-2.2.0rc2.tar` & `meerschaum-2.2.0rc3.tar`

### file list

```diff
@@ -1,301 +1,301 @@
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.944576 meerschaum-2.2.0rc2/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-2.2.0rc2/LICENSE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-2.2.0rc2/NOTICE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23441 2024-05-22 22:01:38.944576 meerschaum-2.2.0rc2/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9183 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/README.md
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.887577 meerschaum-2.2.0rc2/meerschaum/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1487 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2763 2024-05-17 16:18:37.000000 meerschaum-2.2.0rc2/meerschaum/__main__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.888577 meerschaum-2.2.0rc2/meerschaum/_internal/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-2.2.0rc2/meerschaum/_internal/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.888577 meerschaum-2.2.0rc2/meerschaum/_internal/arguments/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-2.2.0rc2/meerschaum/_internal/arguments/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10249 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/_internal/arguments/_parse_arguments.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13719 2024-05-07 20:25:34.000000 meerschaum-2.2.0rc2/meerschaum/_internal/arguments/_parser.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.889577 meerschaum-2.2.0rc2/meerschaum/_internal/docs/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/_internal/docs/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7076 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/_internal/docs/index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4806 2024-05-15 15:21:26.000000 meerschaum-2.2.0rc2/meerschaum/_internal/entry.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.889577 meerschaum-2.2.0rc2/meerschaum/_internal/gui/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1313 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/_internal/gui/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.889577 meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/_windows.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      935 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1596 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.890576 meerschaum-2.2.0rc2/meerschaum/_internal/shell/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32826 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/_internal/shell/Shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3114 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/_internal/shell/ShellCompleter.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-2.2.0rc2/meerschaum/_internal/shell/ValidAutoSuggest.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc2/meerschaum/_internal/shell/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.890576 meerschaum-2.2.0rc2/meerschaum/_internal/shell/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc2/meerschaum/_internal/shell/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.891577 meerschaum-2.2.0rc2/meerschaum/_internal/term/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      520 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/_internal/term/TermPageHandler.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1594 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/_internal/term/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      716 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/_internal/term/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.894577 meerschaum-2.2.0rc2/meerschaum/actions/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11360 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/actions/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12756 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/actions/api.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13396 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/actions/bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4851 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6213 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/copy.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1167 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15528 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/actions/delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2453 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9487 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7431 2024-05-07 20:26:48.000000 meerschaum-2.2.0rc2/meerschaum/actions/install.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2023-09-21 17:52:19.000000 meerschaum-2.2.0rc2/meerschaum/actions/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-2.2.0rc2/meerschaum/actions/os.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-13 21:37:33.000000 meerschaum-2.2.0rc2/meerschaum/actions/pause.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc2/meerschaum/actions/python.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11326 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/actions/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      508 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/actions/reload.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3205 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/setup.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-2.2.0rc2/meerschaum/actions/sh.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    29016 2024-05-22 21:36:42.000000 meerschaum-2.2.0rc2/meerschaum/actions/show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-10-27 06:03:46.000000 meerschaum-2.2.0rc2/meerschaum/actions/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5886 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc2/meerschaum/actions/stack.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18384 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/actions/start.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/stop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    17518 2024-03-26 19:47:08.000000 meerschaum-2.2.0rc2/meerschaum/actions/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3053 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/actions/tag.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6068 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/uninstall.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6302 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/upgrade.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4885 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.895577 meerschaum-2.2.0rc2/meerschaum/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7694 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc2/meerschaum/api/_chain.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1603 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/_events.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      961 2023-08-24 00:13:16.000000 meerschaum-2.2.0rc2/meerschaum/api/_oauth2.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1609 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/api/_websockets.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.897576 meerschaum-2.2.0rc2/meerschaum/api/dash/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2252 2024-03-20 22:38:46.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9418 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/actions.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.898577 meerschaum-2.2.0rc2/meerschaum/api/dash/assets/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/assets/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/assets/ansi_up.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/assets/banner_1920x320.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/assets/favicon.ico
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/assets/logo_48x48.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/assets/logo_500x500.png
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.899577 meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      325 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32283 2024-05-22 21:31:12.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7689 2024-05-10 01:45:18.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2613 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3600 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6364 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/components.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2046 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/graphs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7529 2024-05-10 02:30:25.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12591 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/keys.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.899577 meerschaum-2.2.0rc2/meerschaum/api/dash/pages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-07-21 01:07:38.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/pages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3930 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/pages/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      595 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/pages/error.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4600 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/pages/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1549 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/pages/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2364 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/pages/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19233 2024-05-17 02:49:16.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3662 2024-05-16 15:25:17.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/websockets.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3298 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/webterm.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.900576 meerschaum-2.2.0rc2/meerschaum/api/models/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/models/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/models/_interfaces.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/models/_locations.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/models/_metrics.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-2.2.0rc2/meerschaum/api/models/_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.900576 meerschaum-2.2.0rc2/meerschaum/api/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.900576 meerschaum-2.2.0rc2/meerschaum/api/resources/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.901576 meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/bootstrap.min.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1714 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/dash.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/dbc_dark.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/styles.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5383 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/xterm.css
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.901576 meerschaum-2.2.0rc2/meerschaum/api/resources/static/ico/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/ico/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/ico/logo.ico
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.902577 meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/action_button.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/main.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1729 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/terminado.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   289441 2024-04-05 14:30:27.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/xterm.js
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.902577 meerschaum-2.2.0rc2/meerschaum/api/resources/static/png/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/png/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.903576 meerschaum-2.2.0rc2/meerschaum/api/resources/templates/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/templates/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/templates/index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/templates/old_index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/templates/secret.html
--rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     4527 2024-05-22 21:27:22.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/templates/termpage.html
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.904576 meerschaum-2.2.0rc2/meerschaum/api/routes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      564 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1849 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1933 2024-05-22 19:54:14.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2469 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21677 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6216 2024-05-16 15:09:58.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7204 2023-08-24 00:13:16.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_version.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_webterm.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.904576 meerschaum-2.2.0rc2/meerschaum/api/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      482 2023-10-26 06:22:59.000000 meerschaum-2.2.0rc2/meerschaum/api/tables/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.906576 meerschaum-2.2.0rc2/meerschaum/config/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11517 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/config/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2024-05-16 15:33:56.000000 meerschaum-2.2.0rc2/meerschaum/config/_dash.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5251 2024-05-16 15:31:32.000000 meerschaum-2.2.0rc2/meerschaum/config/_default.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8218 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/config/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4419 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/config/_environment.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6635 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/config/_formatting.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1228 2024-05-17 21:01:54.000000 meerschaum-2.2.0rc2/meerschaum/config/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1526 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/config/_patch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8064 2024-05-22 16:51:21.000000 meerschaum-2.2.0rc2/meerschaum/config/_paths.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc2/meerschaum/config/_preprocess.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14720 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/config/_read_config.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3551 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/config/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4155 2024-05-22 20:00:09.000000 meerschaum-2.2.0rc2/meerschaum/config/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       74 2024-05-22 16:51:34.000000 meerschaum-2.2.0rc2/meerschaum/config/_version.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.906576 meerschaum-2.2.0rc2/meerschaum/config/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/config/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.906576 meerschaum-2.2.0rc2/meerschaum/config/stack/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9007 2024-05-22 20:05:40.000000 meerschaum-2.2.0rc2/meerschaum/config/stack/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.906576 meerschaum-2.2.0rc2/meerschaum/config/stack/grafana/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2024-05-22 20:11:13.000000 meerschaum-2.2.0rc2/meerschaum/config/stack/grafana/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.906576 meerschaum-2.2.0rc2/meerschaum/config/stack/mosquitto/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/config/stack/mosquitto/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.907576 meerschaum-2.2.0rc2/meerschaum/config/stack/mosquitto/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/config/stack/mosquitto/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.907576 meerschaum-2.2.0rc2/meerschaum/config/stack/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/config/stack/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.907576 meerschaum-2.2.0rc2/meerschaum/config/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4435 2024-05-22 19:41:39.000000 meerschaum-2.2.0rc2/meerschaum/config/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.907576 meerschaum-2.2.0rc2/meerschaum/connectors/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc2/meerschaum/connectors/Connector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12023 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc2/meerschaum/connectors/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.909577 meerschaum-2.2.0rc2/meerschaum/connectors/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4355 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/APIConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2755 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2050 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1093 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20962 2023-11-10 05:44:22.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5217 2024-05-07 20:27:04.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6922 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_request.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5275 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4044 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc2/meerschaum/connectors/parse.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.909577 meerschaum-2.2.0rc2/meerschaum/connectors/plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-2.2.0rc2/meerschaum/connectors/plugin/PluginConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/connectors/plugin/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7363 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/connectors/poll.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.911576 meerschaum-2.2.0rc2/meerschaum/connectors/sql/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11522 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/SQLConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4123 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_cli.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10375 2024-03-26 20:20:31.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_create_engine.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13086 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6447 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_instance.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   100925 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8321 2024-05-16 15:18:16.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34262 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3460 2023-10-26 06:22:59.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10100 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_users.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.911576 meerschaum-2.2.0rc2/meerschaum/connectors/sql/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9001 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/tables/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/tables/types.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.911576 meerschaum-2.2.0rc2/meerschaum/core/
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.913576 meerschaum-2.2.0rc2/meerschaum/core/Pipe/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16230 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_attributes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2261 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20880 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_data.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10267 2023-11-13 06:20:00.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2118 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3694 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5234 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    28038 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14262 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.913576 meerschaum-2.2.0rc2/meerschaum/core/Plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc2/meerschaum/core/Plugin/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.914576 meerschaum-2.2.0rc2/meerschaum/core/User/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6456 2024-05-22 21:15:28.000000 meerschaum-2.2.0rc2/meerschaum/core/User/_User.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      193 2024-05-22 19:53:09.000000 meerschaum-2.2.0rc2/meerschaum/core/User/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc2/meerschaum/core/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.914576 meerschaum-2.2.0rc2/meerschaum/plugins/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34039 2024-05-16 15:06:05.000000 meerschaum-2.2.0rc2/meerschaum/plugins/_Plugin.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20760 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/plugins/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.916576 meerschaum-2.2.0rc2/meerschaum/utils/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/utils/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11460 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/utils/_get_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.917576 meerschaum-2.2.0rc2/meerschaum/utils/daemon/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    33728 2024-05-22 21:57:49.000000 meerschaum-2.2.0rc2/meerschaum/utils/daemon/Daemon.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3180 2024-05-22 17:22:17.000000 meerschaum-2.2.0rc2/meerschaum/utils/daemon/FileDescriptorInterceptor.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23376 2024-05-22 21:47:46.000000 meerschaum-2.2.0rc2/meerschaum/utils/daemon/RotatingFile.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8262 2024-05-16 15:03:42.000000 meerschaum-2.2.0rc2/meerschaum/utils/daemon/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4330 2023-09-26 04:28:45.000000 meerschaum-2.2.0rc2/meerschaum/utils/daemon/_names.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31955 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/utils/dataframe.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-2.2.0rc2/meerschaum/utils/debug.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.917576 meerschaum-2.2.0rc2/meerschaum/utils/dtypes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6261 2024-03-26 20:33:15.000000 meerschaum-2.2.0rc2/meerschaum/utils/dtypes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14638 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/utils/dtypes/sql.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.918576 meerschaum-2.2.0rc2/meerschaum/utils/formatting/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13778 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/utils/formatting/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3294 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/utils/formatting/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19492 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/utils/formatting/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3096 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/utils/formatting/_pprint.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3677 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/utils/formatting/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3196 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/utils/interactive.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    43296 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/utils/misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc2/meerschaum/utils/networking.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.918576 meerschaum-2.2.0rc2/meerschaum/utils/packages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    57032 2024-05-15 15:40:39.000000 meerschaum-2.2.0rc2/meerschaum/utils/packages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7968 2024-05-16 05:34:17.000000 meerschaum-2.2.0rc2/meerschaum/utils/packages/_packages.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-2.2.0rc2/meerschaum/utils/packages/lazy_loader.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2655 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/utils/pool.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-10-04 03:17:38.000000 meerschaum-2.2.0rc2/meerschaum/utils/process.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16490 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/utils/prompt.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10020 2024-05-16 04:42:13.000000 meerschaum-2.2.0rc2/meerschaum/utils/schedule.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    46656 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc2/meerschaum/utils/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2489 2024-05-17 21:02:01.000000 meerschaum-2.2.0rc2/meerschaum/utils/threading.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2807 2024-03-20 22:41:20.000000 meerschaum-2.2.0rc2/meerschaum/utils/typing.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.918576 meerschaum-2.2.0rc2/meerschaum/utils/venv/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3553 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc2/meerschaum/utils/venv/_Venv.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23183 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/utils/venv/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6535 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/utils/warnings.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-2.2.0rc2/meerschaum/utils/yaml.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.920576 meerschaum-2.2.0rc2/meerschaum.egg-info/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23441 2024-05-22 22:01:38.000000 meerschaum-2.2.0rc2/meerschaum.egg-info/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8485 2024-05-22 22:01:38.000000 meerschaum-2.2.0rc2/meerschaum.egg-info/SOURCES.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-22 22:01:38.000000 meerschaum-2.2.0rc2/meerschaum.egg-info/dependency_links.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2024-05-22 22:01:38.000000 meerschaum-2.2.0rc2/meerschaum.egg-info/entry_points.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4726 2024-05-22 22:01:38.000000 meerschaum-2.2.0rc2/meerschaum.egg-info/requires.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2024-05-22 22:01:38.000000 meerschaum-2.2.0rc2/meerschaum.egg-info/top_level.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-22 22:01:38.000000 meerschaum-2.2.0rc2/meerschaum.egg-info/zip-safe
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2024-05-22 22:01:38.944576 meerschaum-2.2.0rc2/setup.cfg
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3254 2024-05-15 14:36:58.000000 meerschaum-2.2.0rc2/setup.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.920576 meerschaum-2.2.0rc2/tests/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3139 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/tests/test_deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15351 2023-11-13 21:37:33.000000 meerschaum-2.2.0rc2/tests/test_pipes_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3646 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/tests/test_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21818 2024-05-10 21:08:07.000000 meerschaum-2.2.0rc2/tests/test_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      744 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/tests/test_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3090 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/tests/test_verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.438446 meerschaum-2.2.0rc3/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-2.2.0rc3/LICENSE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-2.2.0rc3/NOTICE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23384 2024-05-24 03:17:02.437446 meerschaum-2.2.0rc3/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9183 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/README.md
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.379446 meerschaum-2.2.0rc3/meerschaum/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1487 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2763 2024-05-17 16:18:37.000000 meerschaum-2.2.0rc3/meerschaum/__main__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.381446 meerschaum-2.2.0rc3/meerschaum/_internal/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-2.2.0rc3/meerschaum/_internal/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.382446 meerschaum-2.2.0rc3/meerschaum/_internal/arguments/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-2.2.0rc3/meerschaum/_internal/arguments/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10249 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/_internal/arguments/_parse_arguments.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13719 2024-05-07 20:25:34.000000 meerschaum-2.2.0rc3/meerschaum/_internal/arguments/_parser.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.382446 meerschaum-2.2.0rc3/meerschaum/_internal/docs/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/_internal/docs/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7076 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/_internal/docs/index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4806 2024-05-15 15:21:26.000000 meerschaum-2.2.0rc3/meerschaum/_internal/entry.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.382446 meerschaum-2.2.0rc3/meerschaum/_internal/gui/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1313 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/_internal/gui/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.383446 meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/_windows.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      935 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1596 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.383446 meerschaum-2.2.0rc3/meerschaum/_internal/shell/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32826 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc3/meerschaum/_internal/shell/Shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3114 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/_internal/shell/ShellCompleter.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-2.2.0rc3/meerschaum/_internal/shell/ValidAutoSuggest.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc3/meerschaum/_internal/shell/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.383446 meerschaum-2.2.0rc3/meerschaum/_internal/shell/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc3/meerschaum/_internal/shell/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.384446 meerschaum-2.2.0rc3/meerschaum/_internal/term/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      520 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/_internal/term/TermPageHandler.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1594 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/_internal/term/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      716 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/_internal/term/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.388446 meerschaum-2.2.0rc3/meerschaum/actions/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11360 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/actions/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12756 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc3/meerschaum/actions/api.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13396 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/actions/bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4851 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6213 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/copy.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1167 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15528 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/actions/delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2453 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9487 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7431 2024-05-07 20:26:48.000000 meerschaum-2.2.0rc3/meerschaum/actions/install.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2023-09-21 17:52:19.000000 meerschaum-2.2.0rc3/meerschaum/actions/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-2.2.0rc3/meerschaum/actions/os.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-13 21:37:33.000000 meerschaum-2.2.0rc3/meerschaum/actions/pause.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc3/meerschaum/actions/python.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11326 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/actions/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      508 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/actions/reload.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3205 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/setup.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-2.2.0rc3/meerschaum/actions/sh.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    29016 2024-05-22 21:36:42.000000 meerschaum-2.2.0rc3/meerschaum/actions/show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-10-27 06:03:46.000000 meerschaum-2.2.0rc3/meerschaum/actions/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5886 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc3/meerschaum/actions/stack.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18384 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/actions/start.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/stop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    17518 2024-03-26 19:47:08.000000 meerschaum-2.2.0rc3/meerschaum/actions/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3053 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/actions/tag.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6068 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/uninstall.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6302 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/upgrade.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4885 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/actions/verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.389446 meerschaum-2.2.0rc3/meerschaum/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7410 2024-05-23 05:45:25.000000 meerschaum-2.2.0rc3/meerschaum/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc3/meerschaum/api/_chain.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1603 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/_events.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      961 2023-08-24 00:13:16.000000 meerschaum-2.2.0rc3/meerschaum/api/_oauth2.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1609 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/api/_websockets.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.391446 meerschaum-2.2.0rc3/meerschaum/api/dash/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2252 2024-03-20 22:38:46.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9418 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/actions.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.392446 meerschaum-2.2.0rc3/meerschaum/api/dash/assets/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/assets/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/assets/ansi_up.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/assets/banner_1920x320.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/assets/favicon.ico
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/assets/logo_48x48.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/assets/logo_500x500.png
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.393446 meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      325 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32283 2024-05-22 21:31:12.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7689 2024-05-10 01:45:18.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2613 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3600 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6364 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/components.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2046 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/graphs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7529 2024-05-10 02:30:25.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12591 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/keys.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.394446 meerschaum-2.2.0rc3/meerschaum/api/dash/pages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-07-21 01:07:38.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/pages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3930 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/pages/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      595 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/pages/error.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4600 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/pages/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1549 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/pages/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2364 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/pages/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19233 2024-05-17 02:49:16.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3662 2024-05-16 15:25:17.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/websockets.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3298 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/api/dash/webterm.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.395446 meerschaum-2.2.0rc3/meerschaum/api/models/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/models/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/models/_interfaces.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/models/_locations.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/models/_metrics.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-2.2.0rc3/meerschaum/api/models/_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.395446 meerschaum-2.2.0rc3/meerschaum/api/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.395446 meerschaum-2.2.0rc3/meerschaum/api/resources/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.396446 meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/bootstrap.min.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1714 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/dash.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/dbc_dark.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/styles.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5383 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/xterm.css
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.396446 meerschaum-2.2.0rc3/meerschaum/api/resources/static/ico/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/ico/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/ico/logo.ico
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.397446 meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/action_button.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/main.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1729 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/terminado.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   289441 2024-04-05 14:30:27.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/xterm.js
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.397446 meerschaum-2.2.0rc3/meerschaum/api/resources/static/png/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/static/png/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.398446 meerschaum-2.2.0rc3/meerschaum/api/resources/templates/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/templates/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/templates/index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/templates/old_index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/templates/secret.html
+-rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     4527 2024-05-22 21:27:22.000000 meerschaum-2.2.0rc3/meerschaum/api/resources/templates/termpage.html
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.400446 meerschaum-2.2.0rc3/meerschaum/api/routes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      564 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1849 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1933 2024-05-22 19:54:14.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2469 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21677 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6216 2024-05-16 15:09:58.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7204 2023-08-24 00:13:16.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_version.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/api/routes/_webterm.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.400446 meerschaum-2.2.0rc3/meerschaum/api/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      482 2023-10-26 06:22:59.000000 meerschaum-2.2.0rc3/meerschaum/api/tables/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.401446 meerschaum-2.2.0rc3/meerschaum/config/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11517 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/config/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2024-05-16 15:33:56.000000 meerschaum-2.2.0rc3/meerschaum/config/_dash.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5251 2024-05-16 15:31:32.000000 meerschaum-2.2.0rc3/meerschaum/config/_default.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8218 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/config/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4419 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/config/_environment.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6635 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/config/_formatting.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1227 2024-05-23 04:18:10.000000 meerschaum-2.2.0rc3/meerschaum/config/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1526 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc3/meerschaum/config/_patch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8154 2024-05-23 00:55:12.000000 meerschaum-2.2.0rc3/meerschaum/config/_paths.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc3/meerschaum/config/_preprocess.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14720 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/config/_read_config.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3551 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc3/meerschaum/config/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4155 2024-05-22 20:00:09.000000 meerschaum-2.2.0rc3/meerschaum/config/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       74 2024-05-24 02:32:37.000000 meerschaum-2.2.0rc3/meerschaum/config/_version.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.401446 meerschaum-2.2.0rc3/meerschaum/config/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/config/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.402446 meerschaum-2.2.0rc3/meerschaum/config/stack/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9007 2024-05-22 20:05:40.000000 meerschaum-2.2.0rc3/meerschaum/config/stack/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.402446 meerschaum-2.2.0rc3/meerschaum/config/stack/grafana/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2024-05-22 20:11:13.000000 meerschaum-2.2.0rc3/meerschaum/config/stack/grafana/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.402446 meerschaum-2.2.0rc3/meerschaum/config/stack/mosquitto/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/config/stack/mosquitto/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.402446 meerschaum-2.2.0rc3/meerschaum/config/stack/mosquitto/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/config/stack/mosquitto/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.402446 meerschaum-2.2.0rc3/meerschaum/config/stack/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/config/stack/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.402446 meerschaum-2.2.0rc3/meerschaum/config/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4474 2024-05-23 05:41:27.000000 meerschaum-2.2.0rc3/meerschaum/config/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.402446 meerschaum-2.2.0rc3/meerschaum/connectors/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc3/meerschaum/connectors/Connector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12071 2024-05-23 02:54:44.000000 meerschaum-2.2.0rc3/meerschaum/connectors/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.403446 meerschaum-2.2.0rc3/meerschaum/connectors/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4355 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/APIConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2755 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2050 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1093 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20962 2023-11-10 05:44:22.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5217 2024-05-07 20:27:04.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6922 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_request.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5275 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc3/meerschaum/connectors/api/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4044 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc3/meerschaum/connectors/parse.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.404446 meerschaum-2.2.0rc3/meerschaum/connectors/plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-2.2.0rc3/meerschaum/connectors/plugin/PluginConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/connectors/plugin/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7363 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/connectors/poll.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.405446 meerschaum-2.2.0rc3/meerschaum/connectors/sql/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11709 2024-05-23 02:46:39.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/SQLConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4123 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_cli.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10396 2024-05-23 03:26:48.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_create_engine.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13086 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6509 2024-05-24 02:32:37.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_instance.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   101357 2024-05-24 02:52:48.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8321 2024-05-16 15:18:16.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34199 2024-05-24 02:32:37.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3460 2023-10-26 06:22:59.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10100 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/_users.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.405446 meerschaum-2.2.0rc3/meerschaum/connectors/sql/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9001 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/tables/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/tables/types.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc3/meerschaum/connectors/sql/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.405446 meerschaum-2.2.0rc3/meerschaum/core/
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.407446 meerschaum-2.2.0rc3/meerschaum/core/Pipe/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16230 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_attributes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2261 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20880 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_data.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10267 2023-11-13 06:20:00.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2118 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3694 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5234 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    28038 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14262 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/core/Pipe/_verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.407446 meerschaum-2.2.0rc3/meerschaum/core/Plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc3/meerschaum/core/Plugin/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.407446 meerschaum-2.2.0rc3/meerschaum/core/User/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6527 2024-05-23 06:00:16.000000 meerschaum-2.2.0rc3/meerschaum/core/User/_User.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      193 2024-05-22 19:53:09.000000 meerschaum-2.2.0rc3/meerschaum/core/User/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc3/meerschaum/core/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.407446 meerschaum-2.2.0rc3/meerschaum/plugins/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34039 2024-05-16 15:06:05.000000 meerschaum-2.2.0rc3/meerschaum/plugins/_Plugin.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21866 2024-05-23 03:07:17.000000 meerschaum-2.2.0rc3/meerschaum/plugins/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.409446 meerschaum-2.2.0rc3/meerschaum/utils/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/utils/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11460 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/utils/_get_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.409446 meerschaum-2.2.0rc3/meerschaum/utils/daemon/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34414 2024-05-23 05:42:59.000000 meerschaum-2.2.0rc3/meerschaum/utils/daemon/Daemon.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4544 2024-05-23 04:51:08.000000 meerschaum-2.2.0rc3/meerschaum/utils/daemon/FileDescriptorInterceptor.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23499 2024-05-22 23:55:35.000000 meerschaum-2.2.0rc3/meerschaum/utils/daemon/RotatingFile.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8375 2024-05-22 22:31:49.000000 meerschaum-2.2.0rc3/meerschaum/utils/daemon/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4330 2023-09-26 04:28:45.000000 meerschaum-2.2.0rc3/meerschaum/utils/daemon/_names.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31955 2024-05-24 03:15:14.000000 meerschaum-2.2.0rc3/meerschaum/utils/dataframe.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-2.2.0rc3/meerschaum/utils/debug.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.410446 meerschaum-2.2.0rc3/meerschaum/utils/dtypes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6261 2024-03-26 20:33:15.000000 meerschaum-2.2.0rc3/meerschaum/utils/dtypes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14638 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/meerschaum/utils/dtypes/sql.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.410446 meerschaum-2.2.0rc3/meerschaum/utils/formatting/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13778 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc3/meerschaum/utils/formatting/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3294 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/utils/formatting/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19492 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc3/meerschaum/utils/formatting/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3096 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/utils/formatting/_pprint.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3677 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/utils/formatting/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3196 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/utils/interactive.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    43296 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc3/meerschaum/utils/misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc3/meerschaum/utils/networking.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.411446 meerschaum-2.2.0rc3/meerschaum/utils/packages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    57185 2024-05-23 05:06:05.000000 meerschaum-2.2.0rc3/meerschaum/utils/packages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7923 2024-05-24 02:32:37.000000 meerschaum-2.2.0rc3/meerschaum/utils/packages/_packages.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-2.2.0rc3/meerschaum/utils/packages/lazy_loader.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2655 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/utils/pool.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7192 2024-05-23 05:42:16.000000 meerschaum-2.2.0rc3/meerschaum/utils/process.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16490 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/meerschaum/utils/prompt.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10654 2024-05-24 02:36:46.000000 meerschaum-2.2.0rc3/meerschaum/utils/schedule.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    46656 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc3/meerschaum/utils/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2489 2024-05-17 21:02:01.000000 meerschaum-2.2.0rc3/meerschaum/utils/threading.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2807 2024-03-20 22:41:20.000000 meerschaum-2.2.0rc3/meerschaum/utils/typing.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.411446 meerschaum-2.2.0rc3/meerschaum/utils/venv/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3553 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc3/meerschaum/utils/venv/_Venv.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23183 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc3/meerschaum/utils/venv/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6535 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc3/meerschaum/utils/warnings.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-2.2.0rc3/meerschaum/utils/yaml.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.411446 meerschaum-2.2.0rc3/meerschaum.egg-info/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23384 2024-05-24 03:17:02.000000 meerschaum-2.2.0rc3/meerschaum.egg-info/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8485 2024-05-24 03:17:02.000000 meerschaum-2.2.0rc3/meerschaum.egg-info/SOURCES.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-24 03:17:02.000000 meerschaum-2.2.0rc3/meerschaum.egg-info/dependency_links.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2024-05-24 03:17:02.000000 meerschaum-2.2.0rc3/meerschaum.egg-info/entry_points.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4732 2024-05-24 03:17:02.000000 meerschaum-2.2.0rc3/meerschaum.egg-info/requires.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2024-05-24 03:17:02.000000 meerschaum-2.2.0rc3/meerschaum.egg-info/top_level.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-24 03:17:02.000000 meerschaum-2.2.0rc3/meerschaum.egg-info/zip-safe
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2024-05-24 03:17:02.438446 meerschaum-2.2.0rc3/setup.cfg
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3254 2024-05-15 14:36:58.000000 meerschaum-2.2.0rc3/setup.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-24 03:17:02.411446 meerschaum-2.2.0rc3/tests/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3139 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc3/tests/test_deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15351 2023-11-13 21:37:33.000000 meerschaum-2.2.0rc3/tests/test_pipes_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3646 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/tests/test_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21905 2024-05-24 02:32:37.000000 meerschaum-2.2.0rc3/tests/test_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      744 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/tests/test_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3090 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc3/tests/test_verify.py
```

### Comparing `meerschaum-2.2.0rc2/LICENSE` & `meerschaum-2.2.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/PKG-INFO` & `meerschaum-2.2.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 2.2.0rc2
+Version: 2.2.0rc3
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
@@ -67,15 +67,15 @@
 Requires-Dist: APScheduler>=4.0.0a5; extra == "required"
 Provides-Extra: drivers
 Requires-Dist: cryptography>=38.0.1; extra == "drivers"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "drivers"
 Requires-Dist: PyMySQL>=0.9.0; extra == "drivers"
 Requires-Dist: aiomysql>=0.0.21; extra == "drivers"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "drivers"
-Requires-Dist: duckdb>=0.9.0; extra == "drivers"
+Requires-Dist: duckdb<0.10.0; extra == "drivers"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "drivers"
 Provides-Extra: drivers
 Requires-Dist: pyodbc>=4.0.30; extra == "drivers"
 Requires-Dist: cx_Oracle>=8.3.0; extra == "drivers"
 Provides-Extra: cli
 Requires-Dist: pgcli>=3.1.0; extra == "cli"
 Requires-Dist: mycli>=1.23.2; extra == "cli"
@@ -116,28 +116,28 @@
 Requires-Dist: ruamel.yaml>=0.16.12; extra == "extras"
 Requires-Dist: modin[ray]>=0.8.3; extra == "extras"
 Requires-Dist: nanoid>=2.0.0; extra == "extras"
 Requires-Dist: importlib-metadata>=4.12.0; extra == "extras"
 Provides-Extra: sql
 Requires-Dist: numpy>=1.18.5; extra == "sql"
 Requires-Dist: pandas[parquet]>=2.0.1; extra == "sql"
-Requires-Dist: pyarrow>=7.0.0; extra == "sql"
-Requires-Dist: dask>=2023.5.0; extra == "sql"
+Requires-Dist: pyarrow>=16.1.0; extra == "sql"
+Requires-Dist: dask[dataframe]>=2024.5.1; extra == "sql"
 Requires-Dist: pytz; extra == "sql"
 Requires-Dist: joblib>=0.17.0; extra == "sql"
 Requires-Dist: SQLAlchemy>=2.0.5; extra == "sql"
 Requires-Dist: databases>=0.4.0; extra == "sql"
 Requires-Dist: aiosqlite>=0.16.0; extra == "sql"
 Requires-Dist: asyncpg>=0.21.0; extra == "sql"
 Requires-Dist: cryptography>=38.0.1; extra == "sql"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "sql"
 Requires-Dist: PyMySQL>=0.9.0; extra == "sql"
 Requires-Dist: aiomysql>=0.0.21; extra == "sql"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "sql"
-Requires-Dist: duckdb>=0.9.0; extra == "sql"
+Requires-Dist: duckdb<0.10.0; extra == "sql"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "sql"
 Requires-Dist: wheel>=0.34.2; extra == "sql"
 Requires-Dist: setuptools>=63.3.0; extra == "sql"
 Requires-Dist: PyYAML>=5.3.1; extra == "sql"
 Requires-Dist: pip>=22.0.4; extra == "sql"
 Requires-Dist: update-checker>=0.18.0; extra == "sql"
 Requires-Dist: semver>=3.0.0; extra == "sql"
@@ -163,39 +163,38 @@
 Requires-Dist: dash-bootstrap-components>=1.2.1; extra == "dash"
 Requires-Dist: dash-ace>=0.2.1; extra == "dash"
 Requires-Dist: dash-extensions>=1.0.4; extra == "dash"
 Requires-Dist: dash-daq>=0.5.0; extra == "dash"
 Requires-Dist: terminado>=0.12.1; extra == "dash"
 Requires-Dist: tornado>=6.1.0; extra == "dash"
 Provides-Extra: api
-Requires-Dist: uvicorn[standard]>=0.22.0; extra == "api"
-Requires-Dist: gunicorn>=20.1.0; extra == "api"
+Requires-Dist: uvicorn[standard]>=0.29.0; extra == "api"
+Requires-Dist: gunicorn>=22.0.0; extra == "api"
 Requires-Dist: python-dotenv>=0.20.0; extra == "api"
 Requires-Dist: websockets>=11.0.3; extra == "api"
-Requires-Dist: fastapi>=0.100.0; extra == "api"
-Requires-Dist: passlib>=1.7.4; extra == "api"
+Requires-Dist: fastapi>=0.111.0; extra == "api"
 Requires-Dist: fastapi-login>=1.7.2; extra == "api"
-Requires-Dist: python-multipart>=0.0.5; extra == "api"
+Requires-Dist: python-multipart>=0.0.9; extra == "api"
 Requires-Dist: httpx>=0.24.1; extra == "api"
 Requires-Dist: numpy>=1.18.5; extra == "api"
 Requires-Dist: pandas[parquet]>=2.0.1; extra == "api"
-Requires-Dist: pyarrow>=7.0.0; extra == "api"
-Requires-Dist: dask>=2023.5.0; extra == "api"
+Requires-Dist: pyarrow>=16.1.0; extra == "api"
+Requires-Dist: dask[dataframe]>=2024.5.1; extra == "api"
 Requires-Dist: pytz; extra == "api"
 Requires-Dist: joblib>=0.17.0; extra == "api"
 Requires-Dist: SQLAlchemy>=2.0.5; extra == "api"
 Requires-Dist: databases>=0.4.0; extra == "api"
 Requires-Dist: aiosqlite>=0.16.0; extra == "api"
 Requires-Dist: asyncpg>=0.21.0; extra == "api"
 Requires-Dist: cryptography>=38.0.1; extra == "api"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "api"
 Requires-Dist: PyMySQL>=0.9.0; extra == "api"
 Requires-Dist: aiomysql>=0.0.21; extra == "api"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "api"
-Requires-Dist: duckdb>=0.9.0; extra == "api"
+Requires-Dist: duckdb<0.10.0; extra == "api"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "api"
 Requires-Dist: wheel>=0.34.2; extra == "api"
 Requires-Dist: setuptools>=63.3.0; extra == "api"
 Requires-Dist: PyYAML>=5.3.1; extra == "api"
 Requires-Dist: pip>=22.0.4; extra == "api"
 Requires-Dist: update-checker>=0.18.0; extra == "api"
 Requires-Dist: semver>=3.0.0; extra == "api"
@@ -263,45 +262,44 @@
 Requires-Dist: virtualenv>=20.1.0; extra == "full"
 Requires-Dist: APScheduler>=4.0.0a5; extra == "full"
 Requires-Dist: cryptography>=38.0.1; extra == "full"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "full"
 Requires-Dist: PyMySQL>=0.9.0; extra == "full"
 Requires-Dist: aiomysql>=0.0.21; extra == "full"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "full"
-Requires-Dist: duckdb>=0.9.0; extra == "full"
+Requires-Dist: duckdb<0.10.0; extra == "full"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "full"
 Requires-Dist: toga>=0.3.0-dev29; extra == "full"
 Requires-Dist: pywebview>=3.6.3; extra == "full"
 Requires-Dist: pycparser>=2.21.0; extra == "full"
 Requires-Dist: numpy>=1.18.5; extra == "full"
 Requires-Dist: pandas[parquet]>=2.0.1; extra == "full"
-Requires-Dist: pyarrow>=7.0.0; extra == "full"
-Requires-Dist: dask>=2023.5.0; extra == "full"
+Requires-Dist: pyarrow>=16.1.0; extra == "full"
+Requires-Dist: dask[dataframe]>=2024.5.1; extra == "full"
 Requires-Dist: pytz; extra == "full"
 Requires-Dist: joblib>=0.17.0; extra == "full"
 Requires-Dist: SQLAlchemy>=2.0.5; extra == "full"
 Requires-Dist: databases>=0.4.0; extra == "full"
 Requires-Dist: aiosqlite>=0.16.0; extra == "full"
 Requires-Dist: asyncpg>=0.21.0; extra == "full"
 Requires-Dist: Flask-Compress>=1.10.1; extra == "full"
 Requires-Dist: dash>=2.6.2; extra == "full"
 Requires-Dist: dash-bootstrap-components>=1.2.1; extra == "full"
 Requires-Dist: dash-ace>=0.2.1; extra == "full"
 Requires-Dist: dash-extensions>=1.0.4; extra == "full"
 Requires-Dist: dash-daq>=0.5.0; extra == "full"
 Requires-Dist: terminado>=0.12.1; extra == "full"
 Requires-Dist: tornado>=6.1.0; extra == "full"
-Requires-Dist: uvicorn[standard]>=0.22.0; extra == "full"
-Requires-Dist: gunicorn>=20.1.0; extra == "full"
+Requires-Dist: uvicorn[standard]>=0.29.0; extra == "full"
+Requires-Dist: gunicorn>=22.0.0; extra == "full"
 Requires-Dist: python-dotenv>=0.20.0; extra == "full"
 Requires-Dist: websockets>=11.0.3; extra == "full"
-Requires-Dist: fastapi>=0.100.0; extra == "full"
-Requires-Dist: passlib>=1.7.4; extra == "full"
+Requires-Dist: fastapi>=0.111.0; extra == "full"
 Requires-Dist: fastapi-login>=1.7.2; extra == "full"
-Requires-Dist: python-multipart>=0.0.5; extra == "full"
+Requires-Dist: python-multipart>=0.0.9; extra == "full"
 Requires-Dist: httpx>=0.24.1; extra == "full"
 
 <img src="https://meerschaum.io/assets/banner_1920x320.png" alt="Meerschaum banner" style="width: 100%"/>
 
 | PyPI | GitHub | Info | Stats |
 |---|---|---|---|
 | ![PyPI]( https://img.shields.io/pypi/v/meerschaum?color=%2300cc66&label=Version ) | ![GitHub Repo stars](https://img.shields.io/github/stars/bmeares/Meerschaum?style=social) | ![License](https://img.shields.io/github/license/bmeares/Meerschaum?label=License) | ![Number of plugins]( https://img.shields.io/badge/dynamic/json?color=3098c1&label=Public%20Plugins&query=num_plugins&url=https%3A%2F%2Fapi.mrsm.io%2Finfo ) |
```

### Comparing `meerschaum-2.2.0rc2/README.md` & `meerschaum-2.2.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/__main__.py` & `meerschaum-2.2.0rc3/meerschaum/__main__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/_internal/arguments/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/_internal/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/_internal/arguments/_parse_arguments.py` & `meerschaum-2.2.0rc3/meerschaum/_internal/arguments/_parse_arguments.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/_internal/arguments/_parser.py` & `meerschaum-2.2.0rc3/meerschaum/_internal/arguments/_parser.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/_internal/docs/index.py` & `meerschaum-2.2.0rc3/meerschaum/_internal/docs/index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/_internal/entry.py` & `meerschaum-2.2.0rc3/meerschaum/_internal/entry.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/_internal/gui/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/_internal/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/_windows.py` & `meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/_windows.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/actions.py` & `meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/pipes.py` & `meerschaum-2.2.0rc3/meerschaum/_internal/gui/app/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/_internal/shell/Shell.py` & `meerschaum-2.2.0rc3/meerschaum/_internal/shell/Shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/_internal/shell/ShellCompleter.py` & `meerschaum-2.2.0rc3/meerschaum/_internal/shell/ShellCompleter.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/_internal/shell/ValidAutoSuggest.py` & `meerschaum-2.2.0rc3/meerschaum/_internal/shell/ValidAutoSuggest.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/_internal/term/TermPageHandler.py` & `meerschaum-2.2.0rc3/meerschaum/_internal/term/TermPageHandler.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/_internal/term/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/_internal/term/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/_internal/term/tools.py` & `meerschaum-2.2.0rc3/meerschaum/_internal/term/tools.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/api.py` & `meerschaum-2.2.0rc3/meerschaum/actions/api.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/bootstrap.py` & `meerschaum-2.2.0rc3/meerschaum/actions/bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/clear.py` & `meerschaum-2.2.0rc3/meerschaum/actions/clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/copy.py` & `meerschaum-2.2.0rc3/meerschaum/actions/copy.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/deduplicate.py` & `meerschaum-2.2.0rc3/meerschaum/actions/deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/delete.py` & `meerschaum-2.2.0rc3/meerschaum/actions/delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/drop.py` & `meerschaum-2.2.0rc3/meerschaum/actions/drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/edit.py` & `meerschaum-2.2.0rc3/meerschaum/actions/edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/install.py` & `meerschaum-2.2.0rc3/meerschaum/actions/install.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/login.py` & `meerschaum-2.2.0rc3/meerschaum/actions/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/os.py` & `meerschaum-2.2.0rc3/meerschaum/actions/os.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/pause.py` & `meerschaum-2.2.0rc3/meerschaum/actions/pause.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/python.py` & `meerschaum-2.2.0rc3/meerschaum/actions/python.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/register.py` & `meerschaum-2.2.0rc3/meerschaum/actions/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/setup.py` & `meerschaum-2.2.0rc3/meerschaum/actions/setup.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/sh.py` & `meerschaum-2.2.0rc3/meerschaum/actions/sh.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/show.py` & `meerschaum-2.2.0rc3/meerschaum/actions/show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/sql.py` & `meerschaum-2.2.0rc3/meerschaum/actions/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/stack.py` & `meerschaum-2.2.0rc3/meerschaum/actions/stack.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/start.py` & `meerschaum-2.2.0rc3/meerschaum/actions/start.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/stop.py` & `meerschaum-2.2.0rc3/meerschaum/actions/stop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/sync.py` & `meerschaum-2.2.0rc3/meerschaum/actions/sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/tag.py` & `meerschaum-2.2.0rc3/meerschaum/actions/tag.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/uninstall.py` & `meerschaum-2.2.0rc3/meerschaum/actions/uninstall.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/upgrade.py` & `meerschaum-2.2.0rc3/meerschaum/actions/upgrade.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/actions/verify.py` & `meerschaum-2.2.0rc3/meerschaum/actions/verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,29 +26,34 @@
 
 _locks = {'pipes': RLock(), 'connector': RLock(), 'uvicorn_config': RLock()}
 
 ### Skip verifying packages in the docker image.
 CHECK_UPDATE = os.environ.get(STATIC_CONFIG['environment']['runtime'], None) != 'docker'
 
 endpoints = STATIC_CONFIG['api']['endpoints']
-aiofiles = attempt_import('aiofiles', lazy=False, check_update=CHECK_UPDATE)
+
+(
+    fastapi,
+    aiofiles,
+    starlette_responses,
+    multipart,
+    packaging_version,
+) = attempt_import(
+    'fastapi',
+    'aiofiles',
+    'starlette.responses',
+    'multipart',
+    'packaging.version',
+    lazy = False,
+    check_update = CHECK_UPDATE,
+)
 typing_extensions = attempt_import(
     'typing_extensions', lazy=False, check_update=CHECK_UPDATE,
     venv = None,
 )
-pydantic_dataclasses = attempt_import(
-    'pydantic.dataclasses', lazy=False, check_update=CHECK_UPDATE,
-)
-fastapi = attempt_import('fastapi', lazy=False, check_update=CHECK_UPDATE)
-starlette_reponses = attempt_import(
-    'starlette.responses', warn=False, lazy=False,
-    check_update=CHECK_UPDATE,
-)
-python_multipart = attempt_import('multipart', lazy=False, check_update=CHECK_UPDATE)
-packaging_version = attempt_import('packaging.version', check_update=CHECK_UPDATE)
 from meerschaum.api._chain import check_allow_chaining, DISALLOW_CHAINING_MESSAGE
 uvicorn_config_path = API_UVICORN_RESOURCES_PATH / SERVER_ID / 'config.json'
 
 uvicorn_workers = attempt_import('uvicorn.workers', venv=None, check_update=CHECK_UPDATE)
 uvicorn_config = None
 sys_config = get_config('system', 'api')
 permissions_config = get_config('system', 'api', 'permissions')
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/_chain.py` & `meerschaum-2.2.0rc3/meerschaum/api/_chain.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/_events.py` & `meerschaum-2.2.0rc3/meerschaum/api/_events.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/_oauth2.py` & `meerschaum-2.2.0rc3/meerschaum/api/_oauth2.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/_websockets.py` & `meerschaum-2.2.0rc3/meerschaum/api/_websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/actions.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/assets/ansi_up.js` & `meerschaum-2.2.0rc3/meerschaum/api/dash/assets/ansi_up.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/assets/banner_1920x320.png` & `meerschaum-2.2.0rc3/meerschaum/api/dash/assets/banner_1920x320.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/assets/favicon.ico` & `meerschaum-2.2.0rc3/meerschaum/api/dash/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/assets/logo_48x48.png` & `meerschaum-2.2.0rc3/meerschaum/api/dash/assets/logo_48x48.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/assets/logo_500x500.png` & `meerschaum-2.2.0rc3/meerschaum/api/dash/assets/logo_500x500.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/dashboard.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/dashboard.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/jobs.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/login.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/plugins.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/register.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/components.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/components.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/connectors.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/graphs.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/graphs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/jobs.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/keys.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/keys.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/pages/dashboard.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/pages/dashboard.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/pages/error.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/pages/error.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/pages/login.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/pages/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/pages/plugins.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/pages/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/pages/register.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/pages/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/pipes.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/plugins.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/users.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/websockets.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/dash/webterm.py` & `meerschaum-2.2.0rc3/meerschaum/api/dash/webterm.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/bootstrap.min.css` & `meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/dash.css` & `meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/dash.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/dbc_dark.css` & `meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/dbc_dark.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/xterm.css` & `meerschaum-2.2.0rc3/meerschaum/api/resources/static/css/xterm.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/resources/static/ico/logo.ico` & `meerschaum-2.2.0rc3/meerschaum/api/resources/static/ico/logo.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/action_button.js` & `meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/action_button.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/terminado.js` & `meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/terminado.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/xterm.js` & `meerschaum-2.2.0rc3/meerschaum/api/resources/static/js/xterm.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/resources/templates/index.html` & `meerschaum-2.2.0rc3/meerschaum/api/resources/templates/index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/resources/templates/old_index.html` & `meerschaum-2.2.0rc3/meerschaum/api/resources/templates/old_index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/resources/templates/termpage.html` & `meerschaum-2.2.0rc3/meerschaum/api/resources/templates/termpage.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/routes/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/api/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/routes/_actions.py` & `meerschaum-2.2.0rc3/meerschaum/api/routes/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/routes/_connectors.py` & `meerschaum-2.2.0rc3/meerschaum/api/routes/_connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/routes/_index.py` & `meerschaum-2.2.0rc3/meerschaum/api/routes/_index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/routes/_login.py` & `meerschaum-2.2.0rc3/meerschaum/api/routes/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/routes/_misc.py` & `meerschaum-2.2.0rc3/meerschaum/api/routes/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/routes/_pipes.py` & `meerschaum-2.2.0rc3/meerschaum/api/routes/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/routes/_plugins.py` & `meerschaum-2.2.0rc3/meerschaum/api/routes/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/routes/_users.py` & `meerschaum-2.2.0rc3/meerschaum/api/routes/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/routes/_version.py` & `meerschaum-2.2.0rc3/meerschaum/api/routes/_version.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/api/routes/_webterm.py` & `meerschaum-2.2.0rc3/meerschaum/api/routes/_webterm.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/config/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/config/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/config/_default.py` & `meerschaum-2.2.0rc3/meerschaum/config/_default.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/config/_edit.py` & `meerschaum-2.2.0rc3/meerschaum/config/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/config/_environment.py` & `meerschaum-2.2.0rc3/meerschaum/config/_environment.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/config/_formatting.py` & `meerschaum-2.2.0rc3/meerschaum/config/_formatting.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/config/_jobs.py` & `meerschaum-2.2.0rc3/meerschaum/config/_jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         'columns': 70,
     },
     'logs': {
         'num_files_to_keep': 5,
         'max_file_size': 100_000,
         'lines_to_show': 30,
         'refresh_files_seconds': 5,
-        'min_buffer_len': 10,
+        'min_buffer_len': 5,
         'timestamp_format': '%Y-%m-%d %H:%M',
         'follow_timestamp_format': '%H:%M',
         'colors': [
             'cyan',
             'magenta',
             'orange3',
             'green',
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/config/_patch.py` & `meerschaum-2.2.0rc3/meerschaum/config/_patch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/config/_paths.py` & `meerschaum-2.2.0rc3/meerschaum/config/_paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 
     'CACHE_RESOURCES_PATH'           : ('{ROOT_DIR_PATH}', '.cache'),
     'PIPES_CACHE_RESOURCES_PATH'     : ('{CACHE_RESOURCES_PATH}', 'pipes'),
     'USERS_CACHE_RESOURCES_PATH'     : ('{CACHE_RESOURCES_PATH}', 'users'),
 
     'PLUGINS_RESOURCES_PATH'         : ('{INTERNAL_RESOURCES_PATH}', 'plugins'),
     'PLUGINS_INTERNAL_LOCK_PATH'     : ('{INTERNAL_RESOURCES_PATH}', 'plugins.lock'),
+    'PLUGINS_PACKAGES_INTERNAL_PATH' : ('{INTERNAL_RESOURCES_PATH}', 'packaged_plugins'),
     'PLUGINS_ARCHIVES_RESOURCES_PATH': ('{PLUGINS_RESOURCES_PATH}', '.archives'),
     'PLUGINS_TEMP_RESOURCES_PATH'    : ('{PLUGINS_RESOURCES_PATH}', '.tmp'),
     'PLUGINS_INIT_PATH'              : ('{PLUGINS_RESOURCES_PATH}', '__init__.py'),
 
     'SQLITE_RESOURCES_PATH'          : ('{ROOT_DIR_PATH}', 'sqlite'),
     'SQLITE_DB_PATH'                 : ('{SQLITE_RESOURCES_PATH}', 'mrsm_local.db'),
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/config/_preprocess.py` & `meerschaum-2.2.0rc3/meerschaum/config/_preprocess.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/config/_read_config.py` & `meerschaum-2.2.0rc3/meerschaum/config/_read_config.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/config/_shell.py` & `meerschaum-2.2.0rc3/meerschaum/config/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/config/_sync.py` & `meerschaum-2.2.0rc3/meerschaum/config/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/config/stack/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/config/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/config/stack/grafana/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/config/stack/grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/config/static/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/config/static/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         'dep_group': 'MRSM_DEP_GROUP',
         'home': 'MRSM_HOME',
         'src': 'MRSM_SRC',
         'uid': 'MRSM_UID',
         'gid': 'MRSM_GID',
         'noask': 'MRSM_NOASK',
         'id': 'MRSM_SERVER_ID',
+        'daemon_id': 'MRSM_DAEMON_ID',
         'uri_regex': r'MRSM_([a-zA-Z0-9]*)_(\d*[a-zA-Z][a-zA-Z0-9-_+]*$)',
         'prefix': 'MRSM_',
     },
     'config': {
         'default_filetype': 'json',
         'symlinks_key': '_symlinks',
     },
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/Connector.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/Connector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,14 +313,16 @@
     """
     If a plugin makes use of the `make_connector` decorator,
     load its module.
     """
     from meerschaum.plugins import get_plugins, import_plugins
     to_import = []
     for plugin in get_plugins():
+        if plugin is None:
+            continue
         with open(plugin.__file__, encoding='utf-8') as f:
             text = f.read()
         if 'make_connector' in text:
             to_import.append(plugin.name)
     if not to_import:
         return
     import_plugins(*to_import)
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/api/APIConnector.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/api/APIConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/api/_actions.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/api/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/api/_fetch.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/api/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/api/_login.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/api/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/api/_misc.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/api/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/api/_pipes.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/api/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/api/_plugins.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/api/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/api/_request.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/api/_request.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/api/_uri.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/api/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/api/_users.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/api/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/parse.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/parse.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/plugin/PluginConnector.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/plugin/PluginConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/poll.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/poll.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/sql/SQLConnector.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/sql/SQLConnector.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,16 +124,18 @@
         kw: Any
             All other arguments will be passed to the connector's attributes.
             Therefore, a connector may be made without being registered,
             as long enough parameters are supplied to the constructor.
         """
         if 'uri' in kw:
             uri = kw['uri']
-            if uri.startswith('postgres://'):
-                uri = uri.replace('postgres://', 'postgresql://', 1)
+            if uri.startswith('postgres') and not uri.startswith('postgresql'):
+                uri = uri.replace('postgres', 'postgresql', 1)
+            if uri.startswith('postgresql') and not uri.startswith('postgresql+'):
+                uri = uri.replace('postgresql://', 'postgresql+psycopg', 1)
             if uri.startswith('timescaledb://'):
                 uri = uri.replace('timescaledb://', 'postgresql://', 1)
                 flavor = 'timescaledb'
             kw['uri'] = uri
             from_uri_params = self.from_uri(kw['uri'], as_dict=True)
             label = label or from_uri_params.get('label', None)
             _ = from_uri_params.pop('label', None)
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_cli.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_cli.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_create_engine.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_create_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,35 +24,35 @@
     'pool_size': 5,
     'max_overflow': 10,
     'pool_recycle': 3600,
     'connect_args': {},
 }
 flavor_configs = {
     'timescaledb'      : {
-        'engine'       : 'postgresql',
+        'engine'       : 'postgresql+psycopg',
         'create_engine' : default_create_engine_args,
         'omit_create_engine': {'method',},
         'to_sql' : {},
         'requirements' : default_requirements,
         'defaults'     : {
             'port'     : 5432,
         },
     },
     'postgresql'         : {
-        'engine'       : 'postgresql',
+        'engine'       : 'postgresql+psycopg',
         'create_engine' : default_create_engine_args,
         'omit_create_engine': {'method',},
         'to_sql' : {},
         'requirements' : default_requirements,
         'defaults'     : {
             'port'     : 5432,
         },
     },
     'citus'            : {
-        'engine'       : 'postgresql',
+        'engine'       : 'postgresql+psycopg',
         'create_engine' : default_create_engine_args,
         'omit_create_engine': {'method',},
         'to_sql' : {},
         'requirements' : default_requirements,
         'defaults'     : {
             'port'     : 5432,
         },
@@ -238,15 +238,15 @@
             "@" + _host + ((":" + str(_port)) if _port is not None else '') +
             (("/" + _database) if _database is not None else '')
             + (("?" + urllib.parse.urlencode(_options)) if _options else '')
         ) if not _uri else _uri
 
         ### Sometimes the timescaledb:// flavor can slip in.
         if _uri and self.flavor in ('timescaledb',) and self.flavor in _uri:
-            engine_str = engine_str.replace(f'{self.flavor}://', 'postgresql://')
+            engine_str = engine_str.replace(f'{self.flavor}', 'postgresql', 1)
 
     if debug:
         dprint(
             (
                 (engine_str.replace(':' + _password, ':' + ('*' * len(_password))))
                     if _password is not None else engine_str
             ) + '\n' + f"{self._sys_config.get('create_engine', {}).get('connect_args', {})}"
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_fetch.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_instance.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,17 @@
     from meerschaum.config import get_config
     from meerschaum.connectors.sql.tables import get_tables
     from meerschaum.utils.misc import items_str
     sqlalchemy = mrsm.attempt_import('sqlalchemy')
     temp_tables_table = get_tables(mrsm_instance=self, create=False, debug=debug)['temp_tables']
     last_check = getattr(self, '_stale_temporary_tables_check_timestamp', 0)
     now_ts = time.perf_counter()
-    if refresh or not last_check or (now_ts - last_check) > 60:
+    if not last_check:
+        self._stale_temporary_tables_check_timestamp = 0
+    if refresh or (now_ts - last_check) < 60:
         self._stale_temporary_tables_check_timestamp = now_ts
         return self._drop_temporary_tables(debug=debug)
 
     stale_temporary_tables_minutes = get_config(
         'system', 'connectors', 'sql', 'instance', 'stale_temporary_tables_minutes'
     )
     now = datetime.now(timezone.utc).replace(tzinfo=None)
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_pipes.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_pipes.py`

 * *Files 0% similar despite different names*

```diff
@@ -748,15 +748,15 @@
         order = order,
         limit = limit,
         begin_add_minutes = begin_add_minutes,
         end_add_minutes = end_add_minutes,
         debug = debug,
         **kw
     )
-
+    
     if is_dask:
         index_col = pipe.columns.get('datetime', None)
         kw['index_col'] = index_col
 
     numeric_columns = [
         col
         for col, typ in pipe.dtypes.items()
@@ -1474,77 +1474,86 @@
     )
     from meerschaum.utils.dtypes.sql import (
         get_pd_type_from_db_type,
     )
     from meerschaum.utils.misc import generate_password
     from meerschaum.utils.debug import dprint
 
-    sqlalchemy, sqlalchemy_orm = mrsm.attempt_import('sqlalchemy', 'sqlalchemy.orm')
-    metadef = self.get_pipe_metadef(
-        pipe,
-        params = params,
-        begin = begin,
-        end = end,
-        check_existing = check_existing,
-        debug = debug,
-    )
-    pipe_name = sql_item_name(pipe.target, self.flavor, self.get_pipe_schema(pipe))
-    upsert = pipe.parameters.get('upsert', False) and f'{self.flavor}-upsert' in update_queries
-    internal_schema = self.internal_schema
-    database = getattr(self, 'database', self.parse_uri(self.URI).get('database', None))
-
-    if not pipe.exists(debug=debug):
-        create_pipe_query = get_create_table_query(
-            metadef,
-            pipe.target,
-            self.flavor,
-            schema = self.get_pipe_schema(pipe),
-        )
-        result = self.exec(create_pipe_query, debug=debug)
-        if result is None:
-            return False, f"Could not insert new data into {pipe} from its SQL query definition."
-        if not self.create_indices(pipe, debug=debug):
-            warn(f"Failed to create indices for {pipe}. Continuing...")
-
-        rowcount = pipe.get_rowcount(debug=debug)
-        return True, f"Inserted {rowcount}, updated 0 rows."
-
-    session = sqlalchemy_orm.Session(self.engine)
-    connectable = session if self.flavor != 'duckdb' else self
-
     transact_id = generate_password(3)
     def get_temp_table_name(label: str) -> str:
         return '-' + transact_id + '_' + label + '_' + pipe.target
 
+    internal_schema = self.internal_schema
     temp_table_roots = ['backtrack', 'new', 'delta', 'joined', 'unseen', 'update']
     temp_tables = {
         table_root: get_temp_table_name(table_root)
         for table_root in temp_table_roots
     }
     temp_table_names = {
         table_root: sql_item_name(
             table_name_raw,
             self.flavor,
             internal_schema,
         )
         for table_root, table_name_raw in temp_tables.items()
     }
+    metadef = self.get_pipe_metadef(
+        pipe,
+        params = params,
+        begin = begin,
+        end = end,
+        check_existing = check_existing,
+        debug = debug,
+    )
+    pipe_name = sql_item_name(pipe.target, self.flavor, self.get_pipe_schema(pipe))
+    upsert = pipe.parameters.get('upsert', False) and f'{self.flavor}-upsert' in update_queries
+    database = getattr(self, 'database', self.parse_uri(self.URI).get('database', None))
 
     def clean_up_temp_tables(ready_to_drop: bool = False):
         log_success, log_msg = self._log_temporary_tables_creation(
             [
                 table
                 for table in temp_tables.values()
             ] if not upsert else [temp_tables['update']],
             ready_to_drop = ready_to_drop,
             create = (not pipe.temporary),
             debug = debug,
         )
         if not log_success:
             warn(log_msg)
+        drop_stale_success, drop_stale_msg = self._drop_old_temporary_tables(
+            refresh = False,
+            debug = debug,
+        )
+        if not drop_stale_success:
+            warn(drop_stale_msg)
+        return drop_stale_success, drop_stale_msg
+
+    sqlalchemy, sqlalchemy_orm = mrsm.attempt_import('sqlalchemy', 'sqlalchemy.orm')
+    if not pipe.exists(debug=debug):
+        create_pipe_query = get_create_table_query(
+            metadef,
+            pipe.target,
+            self.flavor,
+            schema = self.get_pipe_schema(pipe),
+        )
+        result = self.exec(create_pipe_query, debug=debug)
+        if result is None:
+            _ = clean_up_temp_tables()
+            return False, f"Could not insert new data into {pipe} from its SQL query definition."
+
+        if not self.create_indices(pipe, debug=debug):
+            warn(f"Failed to create indices for {pipe}. Continuing...")
+
+        rowcount = pipe.get_rowcount(debug=debug)
+        _ = clean_up_temp_tables()
+        return True, f"Inserted {rowcount}, updated 0 rows."
+
+    session = sqlalchemy_orm.Session(self.engine)
+    connectable = session if self.flavor != 'duckdb' else self
 
     create_new_query = get_create_table_query(
         metadef,
         temp_tables[('new') if not upsert else 'update'],
         self.flavor,
         schema = internal_schema,
     )
@@ -1904,18 +1913,14 @@
     msg = (
         f"Inserted {unseen_count}, updated {update_count} rows."
         if not upsert
         else f"Upserted {update_count} row" + ('s' if update_count != 1 else '') + "."
     )
     _ = clean_up_temp_tables(ready_to_drop=True)
 
-    drop_stale_success, drop_stale_msg = self._drop_old_temporary_tables(refresh=False, debug=debug)
-    if not drop_stale_success:
-        warn(drop_stale_msg)
-
     return True, msg
 
 
 def get_sync_time(
         self,
         pipe: 'mrsm.Pipe',
         params: Optional[Dict[str, Any]] = None,
@@ -2368,14 +2373,24 @@
       'id': 'BIGINT',
       'val': 'DOUBLE PRECISION',
     }
     >>> 
     """
     if not pipe.exists(debug=debug):
         return {}
+
+    if self.flavor == 'duckdb':
+        from meerschaum.utils.sql import get_table_cols_types
+        return get_table_cols_types(
+            pipe.target,
+            self,
+            flavor = self.flavor,
+            schema = self.schema,
+        )
+
     table_columns = {}
     try:
         pipe_table = self.get_pipe_table(pipe, debug=debug)
         if pipe_table is None:
             return {}
         for col in pipe_table.columns:
             table_columns[str(col.name)] = str(col.type)
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_plugins.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_sql.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -939,25 +939,23 @@
                 )
             ) if item is not None
             else r'\N'
             for item in row
         ) for row in data_iter
     )
 
+    table_name = sql_item_name(table.name, 'postgresql', table.schema)
+    columns = ', '.join(f'"{k}"' for k in keys)
+    sql = f"COPY {table_name} ({columns}) FROM STDIN WITH CSV NULL '\\N'"
+
     dbapi_conn = conn.connection
     with dbapi_conn.cursor() as cur:
-        s_buf = StringIO()
-        writer = csv.writer(s_buf)
-        writer.writerows(data_iter)
-        s_buf.seek(0)
-
-        columns = ', '.join(f'"{k}"' for k in keys)
-        table_name = sql_item_name(table.name, 'postgresql', table.schema)
-        sql = f"COPY {table_name} ({columns}) FROM STDIN WITH CSV NULL '\\N'"
-        cur.copy_expert(sql=sql, file=s_buf)
+        with cur.copy(sql) as copy:
+            writer = csv.writer(copy)
+            writer.writerows(data_iter)
 
 
 def format_sql_query_for_dask(query: str) -> 'sqlalchemy.sql.selectable.Select':
     """
     Given a `SELECT` query, return a `sqlalchemy` query for Dask to use.
     This may only work with specific database flavors like PostgreSQL.
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_uri.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_users.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/sql/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/sql/tables/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/sql/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/connectors/sql/tables/types.py` & `meerschaum-2.2.0rc3/meerschaum/connectors/sql/tables/types.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/core/Pipe/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/core/Pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_attributes.py` & `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_attributes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_bootstrap.py` & `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_clear.py` & `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_data.py` & `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_data.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_deduplicate.py` & `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_delete.py` & `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_drop.py` & `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_dtypes.py` & `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_dtypes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_edit.py` & `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_fetch.py` & `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_register.py` & `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_show.py` & `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_sync.py` & `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_verify.py` & `meerschaum-2.2.0rc3/meerschaum/core/Pipe/_verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/core/User/_User.py` & `meerschaum-2.2.0rc3/meerschaum/core/User/_User.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,16 @@
     password_hash: str
         The encoded hash string as generated from `hash_password()`.
 
     Returns
     -------
     A `bool` indicating whether `password` matches `password_hash`.
     """
+    if password is None or password_hash is None:
+        return False
     hash_config = STATIC_CONFIG['users']['password_hash']
     try:
         digest, rounds_str, encoded_salt, encoded_checksum = password_hash.split('$')[1:]
         algorithm_name = digest.split('-')[-1]
         salt = ab64_decode(encoded_salt)
         checksum = ab64_decode(encoded_checksum)
         rounds = int(rounds_str)
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/plugins/_Plugin.py` & `meerschaum-2.2.0rc3/meerschaum/plugins/_Plugin.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/plugins/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/plugins/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,23 +243,42 @@
         try:
             PLUGINS_INTERNAL_LOCK_PATH.touch()
         except Exception as e:
             if warn:
                 _warn(f"Unable to create lockfile {PLUGINS_INTERNAL_LOCK_PATH}:\n{e}")
 
     with _locks['internal_plugins']:
+
+        try:
+            from importlib.metadata import entry_points
+        except ImportError:
+            importlib_metadata = attempt_import('importlib_metadata', lazy=False)
+            entry_points = importlib_metadata.entry_points
+
+        ### NOTE: Allow plugins to be installed via `pip`.
+        packaged_plugin_paths = []
+        discovered_packaged_plugins_eps = entry_points(group='meerschaum.plugins')
+        for ep in discovered_packaged_plugins_eps:
+            module_name = ep.name
+            for package_file_path in ep.dist.files:
+                if package_file_path.suffix != '.py':
+                    continue
+                if str(package_file_path) == f'{module_name}.py':
+                    packaged_plugin_paths.append(package_file_path.locate())
+                elif str(package_file_path) == f'{module_name}/__init__.py':
+                    packaged_plugin_paths.append(package_file_path.locate().parent)
+
         if is_symlink(PLUGINS_RESOURCES_PATH) or not PLUGINS_RESOURCES_PATH.exists():
             try:
                 PLUGINS_RESOURCES_PATH.unlink()
             except Exception as e:
                 pass
 
         PLUGINS_RESOURCES_PATH.mkdir(exist_ok=True)
 
-
         existing_symlinked_paths = [
             (PLUGINS_RESOURCES_PATH / item) 
             for item in os.listdir(PLUGINS_RESOURCES_PATH)
         ]
         for plugins_path in PLUGINS_DIR_PATHS:
             if not plugins_path.exists():
                 plugins_path.mkdir(exist_ok=True, parents=True)
@@ -271,14 +290,15 @@
                     if (
                         not item.startswith('.')
                     ) and (item not in ('__pycache__', '__init__.py'))
                 ]
                 for plugins_path in PLUGINS_DIR_PATHS
             ]
         ))
+        plugins_to_be_symlinked.extend(packaged_plugin_paths)
 
         ### Check for duplicates.
         seen_plugins = defaultdict(lambda: 0)
         for plugin_path in plugins_to_be_symlinked:
             plugin_name = plugin_path.stem
             seen_plugins[plugin_name] += 1
         for plugin_name, plugin_count in seen_plugins.items():
@@ -534,14 +554,16 @@
                     else name[:-3]
                 ) for name in os.listdir(PLUGINS_RESOURCES_PATH) if name != '__init__.py'
             ]
         )
     ]
     plugins = tuple(plugin for plugin in _plugins if plugin.is_installed(try_import=try_import))
     if len(to_load) == 1:
+        if len(plugins) == 0:
+            raise ValueError(f"Plugin '{to_load[0]}' is not installed.")
         return plugins[0]
     return plugins
 
 
 def get_plugins_names(*to_load, **kw) -> List[str]:
     """
     Return a list of installed plugins.
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/_get_pipes.py` & `meerschaum-2.2.0rc3/meerschaum/utils/_get_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/daemon/Daemon.py` & `meerschaum-2.2.0rc3/meerschaum/utils/daemon/Daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import sys
 import time
 import traceback
 from functools import partial
 from datetime import datetime, timezone
 from meerschaum.utils.typing import Optional, Dict, Any, SuccessTuple, Callable, List, Union
 from meerschaum.config import get_config
+from meerschaum.config.static import STATIC_CONFIG
 from meerschaum.config._paths import DAEMON_RESOURCES_PATH, LOGS_RESOURCES_PATH
 from meerschaum.config._patch import apply_patch_to_config
 from meerschaum.utils.warnings import warn, error
 from meerschaum.utils.packages import attempt_import
 from meerschaum.utils.venv import venv_exec
 from meerschaum.utils.daemon._names import get_new_daemon_name
 from meerschaum.utils.daemon.RotatingFile import RotatingFile
@@ -166,17 +167,19 @@
         )
 
         log_refresh_seconds = get_config('jobs', 'logs', 'refresh_files_seconds')
         self._log_refresh_timer = RepeatTimer(
             log_refresh_seconds,
             partial(self.rotating_log.refresh_files, start_interception=True),
         )
+
         try:
             os.environ['LINES'], os.environ['COLUMNS'] = str(int(lines)), str(int(columns))
             with self._daemon_context:
+                os.environ[STATIC_CONFIG['environment']['daemon_id']] = self.daemon_id
                 self.rotating_log.refresh_files(start_interception=True)
                 try:
                     with open(self.pid_path, 'w+', encoding='utf-8') as f:
                         f.write(str(os.getpid()))
 
                     self._log_refresh_timer.start()
                     result = self.target(*self.target_args, **self.target_kw)
@@ -458,24 +461,36 @@
 
 
     def _handle_interrupt(self, signal_number: int, stack_frame: 'frame') -> None:
         """
         Handle `SIGINT` within the Daemon context.
         This method is injected into the `DaemonContext`.
         """
+        #  from meerschaum.utils.daemon.FileDescriptorInterceptor import STOP_READING_FD_EVENT
+        #  STOP_READING_FD_EVENT.set()
+        self.rotating_log.stop_log_fd_interception(unused_only=False)
         timer = self.__dict__.get('_log_refresh_timer', None)
         if timer is not None:
             timer.cancel()
 
         daemon_context = self.__dict__.get('_daemon_context', None)
         if daemon_context is not None:
             daemon_context.close()
 
         _close_pools()
-        self.rotating_log.stop_log_fd_interception()
+        import threading
+        for thread in threading.enumerate():
+            if thread.name == 'MainThread':
+                continue
+            try:
+                if thread.is_alive():
+                    stack = traceback.format_stack(sys._current_frames()[thread.ident])
+                    thread.join()
+            except Exception as e:
+                warn(traceback.format_exc())
         raise KeyboardInterrupt()
 
 
     def _handle_sigterm(self, signal_number: int, stack_frame: 'frame') -> None:
         """
         Handle `SIGTERM` within the `Daemon` context.
         This method is injected into the `DaemonContext`.
@@ -485,15 +500,15 @@
             timer.cancel()
 
         daemon_context = self.__dict__.get('_daemon_context', None)
         if daemon_context is not None:
             daemon_context.close()
 
         _close_pools()
-        raise SystemExit(1)
+        raise SystemExit(0)
 
  
     def _send_signal(
             self,
             signal_to_send,
             timeout: Union[float, int, None] = None,
             check_timeout_interval: Union[float, int, None] = None,
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/daemon/RotatingFile.py` & `meerschaum-2.2.0rc3/meerschaum/utils/daemon/RotatingFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -617,14 +617,18 @@
             self._interceptor_threads = []
         if '_interceptors' not in self.__dict__:
             self._interceptors = []
         self._interceptor_threads.extend([
             self._stdout_interceptor_thread,
             self._stderr_interceptor_thread,
         ])
+        self._interceptors.extend([
+            self._stdout_interceptor,
+            self._stderr_interceptor,
+        ])
         self.stop_log_fd_interception(unused_only=True)
 
     def stop_log_fd_interception(self, unused_only: bool = False):
         """
         Stop the file descriptor monitoring threads.
         """
         interceptors = self.__dict__.get('_interceptors', [])
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/daemon/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/utils/daemon/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,14 +60,16 @@
         _ = existing_kwargs.pop('sysargs', None)
         _ = existing_kwargs.pop('filtered_sysargs', None)
         _ = existing_kwargs.pop('debug', None)
         existing_kwargs['sub_args'] = sorted(existing_kwargs.get('sub_args', []))
 
         ### Only run if the kwargs equal or no actions are provided.
         if existing_kwargs == _args or not _args.get('action', []):
+            if daemon.status == 'running':
+                return True, f"Daemon '{daemon}' is already running."
             return daemon.run(
                 debug = debug,
                 allow_dirty_run = True,
             )
 
     success_tuple = run_daemon(
         entry,
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/daemon/_names.py` & `meerschaum-2.2.0rc3/meerschaum/utils/daemon/_names.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/dataframe.py` & `meerschaum-2.2.0rc3/meerschaum/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/debug.py` & `meerschaum-2.2.0rc3/meerschaum/utils/debug.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/dtypes/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/utils/dtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/dtypes/sql.py` & `meerschaum-2.2.0rc3/meerschaum/utils/dtypes/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/formatting/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/utils/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/formatting/_jobs.py` & `meerschaum-2.2.0rc3/meerschaum/utils/formatting/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/formatting/_pipes.py` & `meerschaum-2.2.0rc3/meerschaum/utils/formatting/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/formatting/_pprint.py` & `meerschaum-2.2.0rc3/meerschaum/utils/formatting/_pprint.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/formatting/_shell.py` & `meerschaum-2.2.0rc3/meerschaum/utils/formatting/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/interactive.py` & `meerschaum-2.2.0rc3/meerschaum/utils/interactive.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/misc.py` & `meerschaum-2.2.0rc3/meerschaum/utils/misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/networking.py` & `meerschaum-2.2.0rc3/meerschaum/utils/networking.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/packages/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/utils/packages/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -825,16 +825,19 @@
                 if not pip_install(
                     'setuptools', 'wheel',
                     venv = venv,
                     check_update = False, check_pypi = False,
                     check_wheel = False, debug = debug,
                 ):
                     warn(
-                        f"Failed to install `setuptools` and `wheel` for virtual environment '{venv}'.",
-                        color=False,
+                        (
+                            "Failed to install `setuptools` and `wheel` for virtual "
+                            + f"environment '{venv}'."
+                        ),
+                        color = False,
                     )
 
         if requirements_file_path is not None:
             _args.append('-r')
             _args.append(str(pathlib.Path(requirements_file_path).resolve()))
 
         if not ANSI and '--no-color' not in _args:
@@ -889,21 +892,24 @@
                     _install_no_version,
                     venv=venv, debug=debug,
                 ):
                     warn(
                         f"Failed to clean up package '{_install_no_version}'.",
                     )
 
-        success = run_python_package(
+        rc = run_python_package(
             'pip',
             _args + _packages,
             venv = venv,
             env = _get_pip_os_env(),
             debug = debug,
-        ) == 0
+        )
+        if debug:
+            print(f"{rc=}")
+        success = rc == 0
 
     msg = (
         "Successfully " + ('un' if _uninstall else '') + "installed packages." if success 
         else "Failed to " + ('un' if _uninstall else '') + "install packages."
     )
     if not silent:
         print(msg)
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/packages/_packages.py` & `meerschaum-2.2.0rc3/meerschaum/utils/packages/_packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     },
     'drivers': {
         'cryptography'               : 'cryptography>=38.0.1',
         'psycopg'                    : 'psycopg[binary]>=3.1.18',
         'pymysql'                    : 'PyMySQL>=0.9.0',
         'aiomysql'                   : 'aiomysql>=0.0.21',
         'sqlalchemy_cockroachdb'     : 'sqlalchemy-cockroachdb>=2.0.0',
-        'duckdb'                     : 'duckdb>=0.9.0',
+        'duckdb'                     : 'duckdb<0.10.0',
         'duckdb_engine'              : 'duckdb-engine>=0.9.2',
     },
     '_drivers': {
         'pyodbc'                     : 'pyodbc>=4.0.30',
         'cx_Oracle'                  : 'cx_Oracle>=8.3.0',
     },
     'cli': {
@@ -116,16 +116,16 @@
         'nanoid'                     : 'nanoid>=2.0.0',
         'importlib_metadata'         : 'importlib-metadata>=4.12.0',
     },
 }
 packages['sql'] = {
     'numpy'                          : 'numpy>=1.18.5',
     'pandas'                         : 'pandas[parquet]>=2.0.1',
-    'pyarrow'                        : 'pyarrow>=7.0.0',
-    'dask'                           : 'dask>=2023.5.0',
+    'pyarrow'                        : 'pyarrow>=16.1.0',
+    'dask'                           : 'dask[dataframe]>=2024.5.1',
     'pytz'                           : 'pytz',
     'joblib'                         : 'joblib>=0.17.0',
     'sqlalchemy'                     : 'SQLAlchemy>=2.0.5',
     'databases'                      : 'databases>=0.4.0',
     'aiosqlite'                      : 'aiosqlite>=0.16.0',
     'asyncpg'                        : 'asyncpg>=0.21.0',
 }
@@ -138,22 +138,21 @@
     'dash_ace'                       : 'dash-ace>=0.2.1',
     'dash_extensions'                : 'dash-extensions>=1.0.4',
     'dash_daq'                       : 'dash-daq>=0.5.0',
     'terminado'                      : 'terminado>=0.12.1',
     'tornado'                        : 'tornado>=6.1.0',
 }
 packages['api'] = {
-    'uvicorn'                        : 'uvicorn[standard]>=0.22.0',
-    'gunicorn'                       : 'gunicorn>=20.1.0',
+    'uvicorn'                        : 'uvicorn[standard]>=0.29.0',
+    'gunicorn'                       : 'gunicorn>=22.0.0',
     'dotenv'                         : 'python-dotenv>=0.20.0',
     'websockets'                     : 'websockets>=11.0.3',
-    'fastapi'                        : 'fastapi>=0.100.0',
-    'passlib'                        : 'passlib>=1.7.4',
+    'fastapi'                        : 'fastapi>=0.111.0',
     'fastapi_login'                  : 'fastapi-login>=1.7.2',
-    'multipart'                      : 'python-multipart>=0.0.5',
+    'multipart'                      : 'python-multipart>=0.0.9',
     'httpx'                          : 'httpx>=0.24.1',
     'websockets'                     : 'websockets>=11.0.3',
 }
 packages['api'].update(packages['sql'])
 packages['api'].update(packages['formatting'])
 packages['api'].update(packages['dash'])
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/packages/lazy_loader.py` & `meerschaum-2.2.0rc3/meerschaum/utils/packages/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/pool.py` & `meerschaum-2.2.0rc3/meerschaum/utils/pool.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/process.py` & `meerschaum-2.2.0rc3/meerschaum/utils/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 See `meerschaum.utils.pool` for multiprocessing and
 `meerschaum.utils.threading` for threads.
 """
 
 from __future__ import annotations
 import os, signal, subprocess, sys, platform
 from meerschaum.utils.typing import Union, Optional, Any, Callable, Dict, Tuple
+from meerschaum.config.static import STATIC_CONFIG
 
 def run_process(
         *args,
         foreground: bool = False,
         as_proc: bool = False,
         line_callback: Optional[Callable[[bytes], Any]] = None,
         store_proc_dict: Optional[Dict[str, Any]] = None,
@@ -64,17 +65,26 @@
         import termios
     except ImportError:
         termios = None
 
     if platform.system() == 'Windows':
         foreground = False
 
-    if line_callback is not None:
+    def print_line(line):
+        sys.stdout.write(line.decode('utf-8'))
+        sys.stdout.flush()
+
+    if capture_output or line_callback is not None:
+        kw['stdout'] = subprocess.PIPE
+        kw['stderr'] = subprocess.STDOUT
+    elif os.environ.get(STATIC_CONFIG['environment']['daemon_id']):
         kw['stdout'] = subprocess.PIPE
         kw['stderr'] = subprocess.STDOUT
+        if line_callback is None:
+            line_callback = print_line
 
     if 'env' not in kw:
         kw['env'] = os.environ
 
     user_preexec_fn = kw.get("preexec_fn", None)
 
     if foreground:
@@ -108,23 +118,14 @@
         # terminate then.
         # `os.kill(os.getpid(), signal.SIGSTOP)`
 
     if foreground:
         kw['preexec_fn'] = new_pgid
 
     try:
-        # fork the child
-        #  stdout, stderr = (
-            #  (sys.stdout, sys.stderr) if not capture_output
-            #  else (subprocess.PIPE, subprocess.PIPE)
-        #  )
-        if capture_output:
-            kw['stdout'] = subprocess.PIPE
-            kw['stderr'] = subprocess.PIPE
-
         child = subprocess.Popen(*args, **kw)
 
         # we can't set the process group id from the parent since the child
         # will already have exec'd. and we can't SIGSTOP it before exec,
         # see above.
         # `os.setpgid(child.pid, child.pid)`
 
@@ -193,10 +194,12 @@
         watchdog_thread = Timer(timeout_seconds, timeout_handler)
         watchdog_thread.daemon = True
         watchdog_thread.start()
 
     while proc.poll() is None:
         line = proc.stdout.readline()
         line_callback(line)
+
     if timeout_seconds is not None:
         watchdog_thread.cancel()
+
     return proc.poll()
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/prompt.py` & `meerschaum-2.2.0rc3/meerschaum/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/schedule.py` & `meerschaum-2.2.0rc3/meerschaum/utils/schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -274,15 +274,29 @@
     from meerschaum.utils.misc import round_time
     from meerschaum.utils.warnings import error, warn
     dateutil_parser = mrsm.attempt_import('dateutil.parser')
     starting_parts = schedule.split(STARTING_KEYWORD)
     starting_str = ('now' if len(starting_parts) == 1 else starting_parts[-1]).strip()
     now = now or round_time(datetime.now(timezone.utc), timedelta(minutes=1))
     try:
-        starting_ts = now if starting_str == 'now' else dateutil_parser.parse(starting_str)
+        if starting_str == 'now':
+            starting_ts = now
+        elif 'tomorrow' in starting_str or 'today' in starting_str:
+            today = round_time(now, timedelta(days=1))
+            tomorrow = today + timedelta(days=1)
+            is_tomorrow = 'tomorrow' in starting_str
+            time_str = starting_str.replace('tomorrow', '').replace('today', '').strip()
+            time_ts = dateutil_parser.parse(time_str) if time_str else today
+            starting_ts = (
+                (tomorrow if is_tomorrow else today)
+                + timedelta(hours=time_ts.hour)
+                + timedelta(minutes=time_ts.minute)
+            )
+        else:
+            starting_ts = dateutil_parser.parse(starting_str)
         schedule_parse_error = None
     except Exception as e:
         warn(f"Unable to parse starting time from '{starting_str}'.", stack=False)
         schedule_parse_error = str(e)
     if schedule_parse_error:
         error(schedule_parse_error, ValueError, stack=False)
     if not starting_ts.tzinfo:
```

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/sql.py` & `meerschaum-2.2.0rc3/meerschaum/utils/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/threading.py` & `meerschaum-2.2.0rc3/meerschaum/utils/threading.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/typing.py` & `meerschaum-2.2.0rc3/meerschaum/utils/typing.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/venv/_Venv.py` & `meerschaum-2.2.0rc3/meerschaum/utils/venv/_Venv.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/venv/__init__.py` & `meerschaum-2.2.0rc3/meerschaum/utils/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/warnings.py` & `meerschaum-2.2.0rc3/meerschaum/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum/utils/yaml.py` & `meerschaum-2.2.0rc3/meerschaum/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum.egg-info/PKG-INFO` & `meerschaum-2.2.0rc3/meerschaum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 2.2.0rc2
+Version: 2.2.0rc3
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
@@ -67,15 +67,15 @@
 Requires-Dist: APScheduler>=4.0.0a5; extra == "required"
 Provides-Extra: drivers
 Requires-Dist: cryptography>=38.0.1; extra == "drivers"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "drivers"
 Requires-Dist: PyMySQL>=0.9.0; extra == "drivers"
 Requires-Dist: aiomysql>=0.0.21; extra == "drivers"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "drivers"
-Requires-Dist: duckdb>=0.9.0; extra == "drivers"
+Requires-Dist: duckdb<0.10.0; extra == "drivers"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "drivers"
 Provides-Extra: drivers
 Requires-Dist: pyodbc>=4.0.30; extra == "drivers"
 Requires-Dist: cx_Oracle>=8.3.0; extra == "drivers"
 Provides-Extra: cli
 Requires-Dist: pgcli>=3.1.0; extra == "cli"
 Requires-Dist: mycli>=1.23.2; extra == "cli"
@@ -116,28 +116,28 @@
 Requires-Dist: ruamel.yaml>=0.16.12; extra == "extras"
 Requires-Dist: modin[ray]>=0.8.3; extra == "extras"
 Requires-Dist: nanoid>=2.0.0; extra == "extras"
 Requires-Dist: importlib-metadata>=4.12.0; extra == "extras"
 Provides-Extra: sql
 Requires-Dist: numpy>=1.18.5; extra == "sql"
 Requires-Dist: pandas[parquet]>=2.0.1; extra == "sql"
-Requires-Dist: pyarrow>=7.0.0; extra == "sql"
-Requires-Dist: dask>=2023.5.0; extra == "sql"
+Requires-Dist: pyarrow>=16.1.0; extra == "sql"
+Requires-Dist: dask[dataframe]>=2024.5.1; extra == "sql"
 Requires-Dist: pytz; extra == "sql"
 Requires-Dist: joblib>=0.17.0; extra == "sql"
 Requires-Dist: SQLAlchemy>=2.0.5; extra == "sql"
 Requires-Dist: databases>=0.4.0; extra == "sql"
 Requires-Dist: aiosqlite>=0.16.0; extra == "sql"
 Requires-Dist: asyncpg>=0.21.0; extra == "sql"
 Requires-Dist: cryptography>=38.0.1; extra == "sql"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "sql"
 Requires-Dist: PyMySQL>=0.9.0; extra == "sql"
 Requires-Dist: aiomysql>=0.0.21; extra == "sql"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "sql"
-Requires-Dist: duckdb>=0.9.0; extra == "sql"
+Requires-Dist: duckdb<0.10.0; extra == "sql"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "sql"
 Requires-Dist: wheel>=0.34.2; extra == "sql"
 Requires-Dist: setuptools>=63.3.0; extra == "sql"
 Requires-Dist: PyYAML>=5.3.1; extra == "sql"
 Requires-Dist: pip>=22.0.4; extra == "sql"
 Requires-Dist: update-checker>=0.18.0; extra == "sql"
 Requires-Dist: semver>=3.0.0; extra == "sql"
@@ -163,39 +163,38 @@
 Requires-Dist: dash-bootstrap-components>=1.2.1; extra == "dash"
 Requires-Dist: dash-ace>=0.2.1; extra == "dash"
 Requires-Dist: dash-extensions>=1.0.4; extra == "dash"
 Requires-Dist: dash-daq>=0.5.0; extra == "dash"
 Requires-Dist: terminado>=0.12.1; extra == "dash"
 Requires-Dist: tornado>=6.1.0; extra == "dash"
 Provides-Extra: api
-Requires-Dist: uvicorn[standard]>=0.22.0; extra == "api"
-Requires-Dist: gunicorn>=20.1.0; extra == "api"
+Requires-Dist: uvicorn[standard]>=0.29.0; extra == "api"
+Requires-Dist: gunicorn>=22.0.0; extra == "api"
 Requires-Dist: python-dotenv>=0.20.0; extra == "api"
 Requires-Dist: websockets>=11.0.3; extra == "api"
-Requires-Dist: fastapi>=0.100.0; extra == "api"
-Requires-Dist: passlib>=1.7.4; extra == "api"
+Requires-Dist: fastapi>=0.111.0; extra == "api"
 Requires-Dist: fastapi-login>=1.7.2; extra == "api"
-Requires-Dist: python-multipart>=0.0.5; extra == "api"
+Requires-Dist: python-multipart>=0.0.9; extra == "api"
 Requires-Dist: httpx>=0.24.1; extra == "api"
 Requires-Dist: numpy>=1.18.5; extra == "api"
 Requires-Dist: pandas[parquet]>=2.0.1; extra == "api"
-Requires-Dist: pyarrow>=7.0.0; extra == "api"
-Requires-Dist: dask>=2023.5.0; extra == "api"
+Requires-Dist: pyarrow>=16.1.0; extra == "api"
+Requires-Dist: dask[dataframe]>=2024.5.1; extra == "api"
 Requires-Dist: pytz; extra == "api"
 Requires-Dist: joblib>=0.17.0; extra == "api"
 Requires-Dist: SQLAlchemy>=2.0.5; extra == "api"
 Requires-Dist: databases>=0.4.0; extra == "api"
 Requires-Dist: aiosqlite>=0.16.0; extra == "api"
 Requires-Dist: asyncpg>=0.21.0; extra == "api"
 Requires-Dist: cryptography>=38.0.1; extra == "api"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "api"
 Requires-Dist: PyMySQL>=0.9.0; extra == "api"
 Requires-Dist: aiomysql>=0.0.21; extra == "api"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "api"
-Requires-Dist: duckdb>=0.9.0; extra == "api"
+Requires-Dist: duckdb<0.10.0; extra == "api"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "api"
 Requires-Dist: wheel>=0.34.2; extra == "api"
 Requires-Dist: setuptools>=63.3.0; extra == "api"
 Requires-Dist: PyYAML>=5.3.1; extra == "api"
 Requires-Dist: pip>=22.0.4; extra == "api"
 Requires-Dist: update-checker>=0.18.0; extra == "api"
 Requires-Dist: semver>=3.0.0; extra == "api"
@@ -263,45 +262,44 @@
 Requires-Dist: virtualenv>=20.1.0; extra == "full"
 Requires-Dist: APScheduler>=4.0.0a5; extra == "full"
 Requires-Dist: cryptography>=38.0.1; extra == "full"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "full"
 Requires-Dist: PyMySQL>=0.9.0; extra == "full"
 Requires-Dist: aiomysql>=0.0.21; extra == "full"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "full"
-Requires-Dist: duckdb>=0.9.0; extra == "full"
+Requires-Dist: duckdb<0.10.0; extra == "full"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "full"
 Requires-Dist: toga>=0.3.0-dev29; extra == "full"
 Requires-Dist: pywebview>=3.6.3; extra == "full"
 Requires-Dist: pycparser>=2.21.0; extra == "full"
 Requires-Dist: numpy>=1.18.5; extra == "full"
 Requires-Dist: pandas[parquet]>=2.0.1; extra == "full"
-Requires-Dist: pyarrow>=7.0.0; extra == "full"
-Requires-Dist: dask>=2023.5.0; extra == "full"
+Requires-Dist: pyarrow>=16.1.0; extra == "full"
+Requires-Dist: dask[dataframe]>=2024.5.1; extra == "full"
 Requires-Dist: pytz; extra == "full"
 Requires-Dist: joblib>=0.17.0; extra == "full"
 Requires-Dist: SQLAlchemy>=2.0.5; extra == "full"
 Requires-Dist: databases>=0.4.0; extra == "full"
 Requires-Dist: aiosqlite>=0.16.0; extra == "full"
 Requires-Dist: asyncpg>=0.21.0; extra == "full"
 Requires-Dist: Flask-Compress>=1.10.1; extra == "full"
 Requires-Dist: dash>=2.6.2; extra == "full"
 Requires-Dist: dash-bootstrap-components>=1.2.1; extra == "full"
 Requires-Dist: dash-ace>=0.2.1; extra == "full"
 Requires-Dist: dash-extensions>=1.0.4; extra == "full"
 Requires-Dist: dash-daq>=0.5.0; extra == "full"
 Requires-Dist: terminado>=0.12.1; extra == "full"
 Requires-Dist: tornado>=6.1.0; extra == "full"
-Requires-Dist: uvicorn[standard]>=0.22.0; extra == "full"
-Requires-Dist: gunicorn>=20.1.0; extra == "full"
+Requires-Dist: uvicorn[standard]>=0.29.0; extra == "full"
+Requires-Dist: gunicorn>=22.0.0; extra == "full"
 Requires-Dist: python-dotenv>=0.20.0; extra == "full"
 Requires-Dist: websockets>=11.0.3; extra == "full"
-Requires-Dist: fastapi>=0.100.0; extra == "full"
-Requires-Dist: passlib>=1.7.4; extra == "full"
+Requires-Dist: fastapi>=0.111.0; extra == "full"
 Requires-Dist: fastapi-login>=1.7.2; extra == "full"
-Requires-Dist: python-multipart>=0.0.5; extra == "full"
+Requires-Dist: python-multipart>=0.0.9; extra == "full"
 Requires-Dist: httpx>=0.24.1; extra == "full"
 
 <img src="https://meerschaum.io/assets/banner_1920x320.png" alt="Meerschaum banner" style="width: 100%"/>
 
 | PyPI | GitHub | Info | Stats |
 |---|---|---|---|
 | ![PyPI]( https://img.shields.io/pypi/v/meerschaum?color=%2300cc66&label=Version ) | ![GitHub Repo stars](https://img.shields.io/github/stars/bmeares/Meerschaum?style=social) | ![License](https://img.shields.io/github/license/bmeares/Meerschaum?label=License) | ![Number of plugins]( https://img.shields.io/badge/dynamic/json?color=3098c1&label=Public%20Plugins&query=num_plugins&url=https%3A%2F%2Fapi.mrsm.io%2Finfo ) |
```

### Comparing `meerschaum-2.2.0rc2/meerschaum.egg-info/SOURCES.txt` & `meerschaum-2.2.0rc3/meerschaum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/meerschaum.egg-info/requires.txt` & `meerschaum-2.2.0rc3/meerschaum.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -24,39 +24,38 @@
 psutil>=5.8.0
 watchfiles>=0.21.0
 dill>=0.3.3
 virtualenv>=20.1.0
 APScheduler>=4.0.0a5
 
 [api]
-uvicorn[standard]>=0.22.0
-gunicorn>=20.1.0
+uvicorn[standard]>=0.29.0
+gunicorn>=22.0.0
 python-dotenv>=0.20.0
 websockets>=11.0.3
-fastapi>=0.100.0
-passlib>=1.7.4
+fastapi>=0.111.0
 fastapi-login>=1.7.2
-python-multipart>=0.0.5
+python-multipart>=0.0.9
 httpx>=0.24.1
 numpy>=1.18.5
 pandas[parquet]>=2.0.1
-pyarrow>=7.0.0
-dask>=2023.5.0
+pyarrow>=16.1.0
+dask[dataframe]>=2024.5.1
 pytz
 joblib>=0.17.0
 SQLAlchemy>=2.0.5
 databases>=0.4.0
 aiosqlite>=0.16.0
 asyncpg>=0.21.0
 cryptography>=38.0.1
 psycopg[binary]>=3.1.18
 PyMySQL>=0.9.0
 aiomysql>=0.0.21
 sqlalchemy-cockroachdb>=2.0.0
-duckdb>=0.9.0
+duckdb<0.10.0
 duckdb-engine>=0.9.2
 wheel>=0.34.2
 setuptools>=63.3.0
 PyYAML>=5.3.1
 pip>=22.0.4
 update-checker>=0.18.0
 semver>=3.0.0
@@ -137,15 +136,15 @@
 
 [drivers]
 cryptography>=38.0.1
 psycopg[binary]>=3.1.18
 PyMySQL>=0.9.0
 aiomysql>=0.0.21
 sqlalchemy-cockroachdb>=2.0.0
-duckdb>=0.9.0
+duckdb<0.10.0
 duckdb-engine>=0.9.2
 
 [extras]
 cmd2>=1.4.0
 ruamel.yaml>=0.16.12
 modin[ray]>=0.8.3
 nanoid>=2.0.0
@@ -193,45 +192,44 @@
 virtualenv>=20.1.0
 APScheduler>=4.0.0a5
 cryptography>=38.0.1
 psycopg[binary]>=3.1.18
 PyMySQL>=0.9.0
 aiomysql>=0.0.21
 sqlalchemy-cockroachdb>=2.0.0
-duckdb>=0.9.0
+duckdb<0.10.0
 duckdb-engine>=0.9.2
 toga>=0.3.0-dev29
 pywebview>=3.6.3
 pycparser>=2.21.0
 numpy>=1.18.5
 pandas[parquet]>=2.0.1
-pyarrow>=7.0.0
-dask>=2023.5.0
+pyarrow>=16.1.0
+dask[dataframe]>=2024.5.1
 pytz
 joblib>=0.17.0
 SQLAlchemy>=2.0.5
 databases>=0.4.0
 aiosqlite>=0.16.0
 asyncpg>=0.21.0
 Flask-Compress>=1.10.1
 dash>=2.6.2
 dash-bootstrap-components>=1.2.1
 dash-ace>=0.2.1
 dash-extensions>=1.0.4
 dash-daq>=0.5.0
 terminado>=0.12.1
 tornado>=6.1.0
-uvicorn[standard]>=0.22.0
-gunicorn>=20.1.0
+uvicorn[standard]>=0.29.0
+gunicorn>=22.0.0
 python-dotenv>=0.20.0
 websockets>=11.0.3
-fastapi>=0.100.0
-passlib>=1.7.4
+fastapi>=0.111.0
 fastapi-login>=1.7.2
-python-multipart>=0.0.5
+python-multipart>=0.0.9
 httpx>=0.24.1
 
 [gui]
 toga>=0.3.0-dev29
 pywebview>=3.6.3
 pycparser>=2.21.0
 
@@ -240,28 +238,28 @@
 [required]
 
 [setup]
 
 [sql]
 numpy>=1.18.5
 pandas[parquet]>=2.0.1
-pyarrow>=7.0.0
-dask>=2023.5.0
+pyarrow>=16.1.0
+dask[dataframe]>=2024.5.1
 pytz
 joblib>=0.17.0
 SQLAlchemy>=2.0.5
 databases>=0.4.0
 aiosqlite>=0.16.0
 asyncpg>=0.21.0
 cryptography>=38.0.1
 psycopg[binary]>=3.1.18
 PyMySQL>=0.9.0
 aiomysql>=0.0.21
 sqlalchemy-cockroachdb>=2.0.0
-duckdb>=0.9.0
+duckdb<0.10.0
 duckdb-engine>=0.9.2
 wheel>=0.34.2
 setuptools>=63.3.0
 PyYAML>=5.3.1
 pip>=22.0.4
 update-checker>=0.18.0
 semver>=3.0.0
```

### Comparing `meerschaum-2.2.0rc2/setup.py` & `meerschaum-2.2.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/tests/test_deduplicate.py` & `meerschaum-2.2.0rc3/tests/test_deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/tests/test_pipes_dtypes.py` & `meerschaum-2.2.0rc3/tests/test_pipes_dtypes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/tests/test_sql.py` & `meerschaum-2.2.0rc3/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/tests/test_sync.py` & `meerschaum-2.2.0rc3/tests/test_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,16 @@
 @pytest.mark.parametrize("flavor", get_flavors())
 def test_sync_new_columns(flavor: str):
     """
     Test that new columns are added.
     """
     conn = conns[flavor]
     pipe = Pipe('foo', 'bar', columns={'datetime': 'dt', 'id': 'id'}, instance=conn)
-    pipe.drop(debug=debug)
+    pipe.delete(debug=debug)
+    pipe = Pipe('foo', 'bar', columns={'datetime': 'dt', 'id': 'id'}, instance=conn)
     docs = [
         {'dt': '2022-01-01', 'id': 1, 'a': 10},
     ]
     pipe.sync(docs, debug=debug)
     assert len(pipe.get_data().columns) == 3
 
     docs = [
```

### Comparing `meerschaum-2.2.0rc2/tests/test_users.py` & `meerschaum-2.2.0rc3/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc2/tests/test_verify.py` & `meerschaum-2.2.0rc3/tests/test_verify.py`

 * *Files identical despite different names*

