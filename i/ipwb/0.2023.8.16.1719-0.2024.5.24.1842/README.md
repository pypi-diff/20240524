# Comparing `tmp/ipwb-0.2023.8.16.1719.tar.gz` & `tmp/ipwb-0.2024.5.24.1842.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipwb-0.2023.8.16.1719.tar", last modified: Wed Aug 16 17:20:13 2023, max compression
+gzip compressed data, was "ipwb-0.2024.5.24.1842.tar", last modified: Fri May 24 18:56:52 2024, max compression
```

## Comparing `ipwb-0.2023.8.16.1719.tar` & `ipwb-0.2024.5.24.1842.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-16 17:20:13.529383 ipwb-0.2023.8.16.1719/
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    14967 2023-08-16 17:20:13.529383 ipwb-0.2023.8.16.1719/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13810 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-16 17:20:13.525383 ipwb-0.2023.8.16.1719/ipwb/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6739 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-16 17:20:13.529383 ipwb-0.2023.8.16.1719/ipwb/assets/
--rw-r--r--   0 runner    (1001) docker     (122)      871 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/admin.css
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/daemonController.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-16 17:20:13.529383 ipwb-0.2023.8.16.1719/ipwb/assets/favicons/
--rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/favicons/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/favicons/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (122)      231 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/favicons/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (122)      418 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/favicons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/favicons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)    15086 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/favicons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/favicons/manifest.json
--rw-r--r--   0 runner    (1001) docker     (122)     1718 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/favicons/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (122)     7019 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/favicons/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (122)    19972 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (122)    15933 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/reconstructive-banner.js
--rw-r--r--   0 runner    (1001) docker     (122)     7965 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/reconstructive.js
--rw-r--r--   0 runner    (1001) docker     (122)     1695 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/serviceWorker.js
--rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/webui.css
--rw-r--r--   0 runner    (1001) docker     (122)     9489 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/assets/webui.js
--rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13291 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/indexer.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    38846 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/replay.py
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-16 17:20:13.529383 ipwb-0.2023.8.16.1719/ipwb/templates/
--rw-r--r--   0 runner    (1001) docker     (122)     2476 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/templates/admin.html
--rw-r--r--   0 runner    (1001) docker     (122)     3071 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     9385 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/ipwb/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-16 17:20:13.525383 ipwb-0.2023.8.16.1719/ipwb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14967 2023-08-16 17:20:13.000000 ipwb-0.2023.8.16.1719/ipwb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-08-16 17:20:13.000000 ipwb-0.2023.8.16.1719/ipwb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-16 17:20:13.000000 ipwb-0.2023.8.16.1719/ipwb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-08-16 17:20:13.000000 ipwb-0.2023.8.16.1719/ipwb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-16 17:20:13.000000 ipwb-0.2023.8.16.1719/ipwb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-08-16 17:20:13.000000 ipwb-0.2023.8.16.1719/ipwb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-08-16 17:20:13.000000 ipwb-0.2023.8.16.1719/ipwb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-08-16 17:20:13.529383 ipwb-0.2023.8.16.1719/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2158 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-16 17:20:13.529383 ipwb-0.2023.8.16.1719/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/tests/testUtil.py
--rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)      340 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/tests/test_compile_target_uri.py
--rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/tests/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/tests/test_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      965 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1559 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/tests/test_ipfs_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    12932 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/tests/test_memento.py
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/tests/test_nodeToNode.py
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/tests/test_randomized_add.py
--rw-r--r--   0 runner    (1001) docker     (122)     6793 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/tests/test_replay.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-08-16 17:20:09.000000 ipwb-0.2023.8.16.1719/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:56:52.415657 ipwb-0.2024.5.24.1842/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-05-24 18:56:52.415657 ipwb-0.2024.5.24.1842/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:56:52.411656 ipwb-0.2024.5.24.1842/ipwb/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:56:52.411656 ipwb-0.2024.5.24.1842/ipwb/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/admin.css
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/daemonController.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:56:52.415657 ipwb-0.2024.5.24.1842/ipwb/assets/favicons/
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/favicons/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/favicons/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/favicons/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/favicons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/favicons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/favicons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/favicons/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/favicons/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/favicons/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    19972 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15933 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/reconstructive-banner.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/reconstructive.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/serviceWorker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/webui.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9493 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/assets/webui.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13201 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/indexer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38836 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:56:52.415657 ipwb-0.2024.5.24.1842/ipwb/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/templates/admin.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9385 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/ipwb/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:56:52.415657 ipwb-0.2024.5.24.1842/ipwb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-05-24 18:56:52.000000 ipwb-0.2024.5.24.1842/ipwb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-24 18:56:52.000000 ipwb-0.2024.5.24.1842/ipwb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:56:52.000000 ipwb-0.2024.5.24.1842/ipwb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-24 18:56:52.000000 ipwb-0.2024.5.24.1842/ipwb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:56:52.000000 ipwb-0.2024.5.24.1842/ipwb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-24 18:56:52.000000 ipwb-0.2024.5.24.1842/ipwb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-24 18:56:52.000000 ipwb-0.2024.5.24.1842/ipwb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-24 18:56:52.419657 ipwb-0.2024.5.24.1842/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:56:52.415657 ipwb-0.2024.5.24.1842/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/tests/testUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/tests/test_compile_target_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/tests/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/tests/test_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/tests/test_ipfs_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12932 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/tests/test_memento.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/tests/test_nodeToNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/tests/test_randomized_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/tests/test_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-24 18:56:50.000000 ipwb-0.2024.5.24.1842/tests/test_util.py
```

### Comparing `ipwb-0.2023.8.16.1719/LICENSE` & `ipwb-0.2024.5.24.1842/LICENSE`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/PKG-INFO` & `ipwb-0.2024.5.24.1842/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipwb
-Version: 0.2023.8.16.1719
+Version: 0.2024.5.24.1842
 Summary: InterPlanetary Wayback (ipwb): Web Archive integration with IPFS
 Home-page: https://github.com/oduwsdl/ipwb
 Download-URL: https://github.com/oduwsdl/ipwb
 Author: Mat Kelly
 Author-email: me@matkelly.com
 License: MIT
 Keywords: http web archives ipfs distributed odu wayback memento
@@ -23,22 +23,29 @@
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Archiving :: Mirroring
 Classifier: Topic :: Utilities
 Provides: ipwb
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: warcio>=1.5.3
+Requires-Dist: ipfshttpclient>=0.8.0a
+Requires-Dist: Flask>=3.0
+Requires-Dist: pycryptodome>=3.4.11
+Requires-Dist: requests>=2.19.1
+Requires-Dist: beautifulsoup4>=4.6.3
+Requires-Dist: surt>=0.3.0
 
 [![image](https://github.com/oduwsdl/ipwb/raw/master/docs/logo_stroked_400px.png)](https://pypi.python.org/pypi/ipwb)
 
 # InterPlanetary Wayback (ipwb)
 
 **Peer-To-Peer Permanence of Web Archives**
 
-[![Build Status](https://travis-ci.org/oduwsdl/ipwb.svg?branch=master)](https://travis-ci.org/oduwsdl/ipwb) [![pypi](https://img.shields.io/pypi/v/ipwb.svg)](https://pypi.org/project/ipwb) [![codecov](https://codecov.io/gh/oduwsdl/ipwb/branch/master/graph/badge.svg)](https://codecov.io/gh/oduwsdl/ipwb)
+[![pypi](https://img.shields.io/pypi/v/ipwb.svg)](https://pypi.org/project/ipwb) [![codecov](https://codecov.io/gh/oduwsdl/ipwb/branch/master/graph/badge.svg)](https://codecov.io/gh/oduwsdl/ipwb)
 
 InterPlanetary Wayback (ipwb) facilitates permanence and collaboration in web archives by disseminating the contents of [WARC](http://www.iso.org/iso/catalogue_detail.htm?csnumber=44717) files into the IPFS network. [IPFS](https://ipfs.io/) is a peer-to-peer content-addressable file system that inherently allows deduplication and facilitates opt-in replication. ipwb splits the header and payload of WARC response records before disseminating into IPFS to leverage the deduplication, builds a [CDXJ index](https://github.com/oduwsdl/ORS/wiki/CDXJ) with references to the IPFS hashes returned, and combines the header and payload from IPFS at the time of replay.
 
 InterPlanetary Wayback primarily consists of two scripts:
 
 - **ipwb/indexer.py** - archival indexing script that takes the path to a WARC input, extracts the HTTP headers, HTTP payload (response body), and relevant parts of the WARC-response record header from the WARC specified and creates byte string representations. The indexer then pushes the byte strings into IPFS using a locally running IPFS daemon then creates a [CDXJ](https://github.com/oduwsdl/ORS/wiki/CDXJ) file with this metadata for replay.py.
 - **ipwb/replay.py** - rudimentary replay script to resolve requests for archival content contained in IPFS for replay in the browser.
```

### Comparing `ipwb-0.2023.8.16.1719/README.md` & `ipwb-0.2024.5.24.1842/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [![image](https://github.com/oduwsdl/ipwb/raw/master/docs/logo_stroked_400px.png)](https://pypi.python.org/pypi/ipwb)
 
 # InterPlanetary Wayback (ipwb)
 
 **Peer-To-Peer Permanence of Web Archives**
 
-[![Build Status](https://travis-ci.org/oduwsdl/ipwb.svg?branch=master)](https://travis-ci.org/oduwsdl/ipwb) [![pypi](https://img.shields.io/pypi/v/ipwb.svg)](https://pypi.org/project/ipwb) [![codecov](https://codecov.io/gh/oduwsdl/ipwb/branch/master/graph/badge.svg)](https://codecov.io/gh/oduwsdl/ipwb)
+[![pypi](https://img.shields.io/pypi/v/ipwb.svg)](https://pypi.org/project/ipwb) [![codecov](https://codecov.io/gh/oduwsdl/ipwb/branch/master/graph/badge.svg)](https://codecov.io/gh/oduwsdl/ipwb)
 
 InterPlanetary Wayback (ipwb) facilitates permanence and collaboration in web archives by disseminating the contents of [WARC](http://www.iso.org/iso/catalogue_detail.htm?csnumber=44717) files into the IPFS network. [IPFS](https://ipfs.io/) is a peer-to-peer content-addressable file system that inherently allows deduplication and facilitates opt-in replication. ipwb splits the header and payload of WARC response records before disseminating into IPFS to leverage the deduplication, builds a [CDXJ index](https://github.com/oduwsdl/ORS/wiki/CDXJ) with references to the IPFS hashes returned, and combines the header and payload from IPFS at the time of replay.
 
 InterPlanetary Wayback primarily consists of two scripts:
 
 - **ipwb/indexer.py** - archival indexing script that takes the path to a WARC input, extracts the HTTP headers, HTTP payload (response body), and relevant parts of the WARC-response record header from the WARC specified and creates byte string representations. The indexer then pushes the byte strings into IPFS using a locally running IPFS daemon then creates a [CDXJ](https://github.com/oduwsdl/ORS/wiki/CDXJ) file with this metadata for replay.py.
 - **ipwb/replay.py** - rudimentary replay script to resolve requests for archival content contained in IPFS for replay in the browser.
```

### Comparing `ipwb-0.2023.8.16.1719/ipwb/__main__.py` & `ipwb-0.2024.5.24.1842/ipwb/__main__.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/assets/admin.css` & `ipwb-0.2024.5.24.1842/ipwb/assets/admin.css`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/assets/daemonController.js` & `ipwb-0.2024.5.24.1842/ipwb/assets/daemonController.js`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/assets/favicons/android-chrome-192x192.png` & `ipwb-0.2024.5.24.1842/ipwb/assets/favicons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/assets/favicons/apple-touch-icon.png` & `ipwb-0.2024.5.24.1842/ipwb/assets/favicons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/assets/favicons/favicon-32x32.png` & `ipwb-0.2024.5.24.1842/ipwb/assets/favicons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/assets/favicons/favicon.ico` & `ipwb-0.2024.5.24.1842/ipwb/assets/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/assets/favicons/mstile-150x150.png` & `ipwb-0.2024.5.24.1842/ipwb/assets/favicons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/assets/favicons/safari-pinned-tab.svg` & `ipwb-0.2024.5.24.1842/ipwb/assets/favicons/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/assets/logo.png` & `ipwb-0.2024.5.24.1842/ipwb/assets/logo.png`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/assets/reconstructive-banner.js` & `ipwb-0.2024.5.24.1842/ipwb/assets/reconstructive-banner.js`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/assets/reconstructive.js` & `ipwb-0.2024.5.24.1842/ipwb/assets/reconstructive.js`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/assets/serviceWorker.js` & `ipwb-0.2024.5.24.1842/ipwb/assets/serviceWorker.js`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/assets/webui.css` & `ipwb-0.2024.5.24.1842/ipwb/assets/webui.css`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/assets/webui.js` & `ipwb-0.2024.5.24.1842/ipwb/assets/webui.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -238,15 +238,15 @@
 function injectIPWBJS() { // eslint-disable-line no-unused-vars
     registerServiceWorker()
 }
 
 function getServiceWorkerVersion() {
     return window.fetch(document.location.href)
         .then(function(resp) {
-            return Promise.resolve(resp.headers.get('Server').split('/')[1])
+            return Promise.resolve(resp.headers.get('Server').split('/').at(-1))
         })
 }
 
 function reinstallServiceWorker() {
     console.log('Deleting old serviceWorker')
     deleteServiceWorker()
     document.getElementById('serviceWorkerVersion').innerHTML = 'Updating...'
```

### Comparing `ipwb-0.2023.8.16.1719/ipwb/backends.py` & `ipwb-0.2024.5.24.1842/ipwb/backends.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/error_handler.py` & `ipwb-0.2024.5.24.1842/ipwb/error_handler.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/indexer.py` & `ipwb-0.2024.5.24.1842/ipwb/indexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,14 @@
 from warcio.archiveiterator import ArchiveIterator
 from warcio.recordloader import ArchiveLoadFailed
 
 from requests.packages.urllib3.exceptions import NewConnectionError
 from ipfshttpclient.exceptions import ConnectionError
 # from requests.exceptions import ConnectionError
 
-from six.moves import input
-from six import PY2
-from six import PY3
-
 from ipwb.util import iso8601_to_digits14, ipfs_client
 
 import requests
 import datetime
 
 from bs4 import BeautifulSoup
 
@@ -45,15 +41,15 @@
 
 from .__init__ import __version__ as ipwb_version
 
 DEBUG = False
 
 
 def s2b(s):  # Convert str to bytes, cross-py
-    return bytes(s) if PY2 else bytes(s, 'utf-8')
+    return bytes(s, 'utf-8')
 
 
 # TODO: put this method definition below index_file_at()
 def push_to_ipfs(hstr, payload):
     ipfs_retry_count = 5  # WARC->IPFS attempts before giving up
     retry_count = 0
     while retry_count < ipfs_retry_count:
```

### Comparing `ipwb-0.2023.8.16.1719/ipwb/replay.py` & `ipwb-0.2024.5.24.1842/ipwb/replay.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Flask, Response, request, redirect, render_template,
 )
 
 from bisect import bisect_left
 from socket import gaierror
 from socket import error as socketerror
 
-from six.moves.urllib_parse import urlsplit, urlunsplit
+from urllib.parse import urlsplit, urlunsplit
 
 
 from requests.exceptions import HTTPError
 from ipfshttpclient.exceptions import ConnectionError
 
 from . import util as ipwb_utils
 from .backends import get_web_archive_index
```

### Comparing `ipwb-0.2023.8.16.1719/ipwb/settings.py` & `ipwb-0.2024.5.24.1842/ipwb/settings.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/templates/admin.html` & `ipwb-0.2024.5.24.1842/ipwb/templates/admin.html`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/templates/index.html` & `ipwb-0.2024.5.24.1842/ipwb/templates/index.html`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb/util.py` & `ipwb-0.2024.5.24.1842/ipwb/util.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/ipwb.egg-info/PKG-INFO` & `ipwb-0.2024.5.24.1842/ipwb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipwb
-Version: 0.2023.8.16.1719
+Version: 0.2024.5.24.1842
 Summary: InterPlanetary Wayback (ipwb): Web Archive integration with IPFS
 Home-page: https://github.com/oduwsdl/ipwb
 Download-URL: https://github.com/oduwsdl/ipwb
 Author: Mat Kelly
 Author-email: me@matkelly.com
 License: MIT
 Keywords: http web archives ipfs distributed odu wayback memento
@@ -23,22 +23,29 @@
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Archiving :: Mirroring
 Classifier: Topic :: Utilities
 Provides: ipwb
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: warcio>=1.5.3
+Requires-Dist: ipfshttpclient>=0.8.0a
+Requires-Dist: Flask>=3.0
+Requires-Dist: pycryptodome>=3.4.11
+Requires-Dist: requests>=2.19.1
+Requires-Dist: beautifulsoup4>=4.6.3
+Requires-Dist: surt>=0.3.0
 
 [![image](https://github.com/oduwsdl/ipwb/raw/master/docs/logo_stroked_400px.png)](https://pypi.python.org/pypi/ipwb)
 
 # InterPlanetary Wayback (ipwb)
 
 **Peer-To-Peer Permanence of Web Archives**
 
-[![Build Status](https://travis-ci.org/oduwsdl/ipwb.svg?branch=master)](https://travis-ci.org/oduwsdl/ipwb) [![pypi](https://img.shields.io/pypi/v/ipwb.svg)](https://pypi.org/project/ipwb) [![codecov](https://codecov.io/gh/oduwsdl/ipwb/branch/master/graph/badge.svg)](https://codecov.io/gh/oduwsdl/ipwb)
+[![pypi](https://img.shields.io/pypi/v/ipwb.svg)](https://pypi.org/project/ipwb) [![codecov](https://codecov.io/gh/oduwsdl/ipwb/branch/master/graph/badge.svg)](https://codecov.io/gh/oduwsdl/ipwb)
 
 InterPlanetary Wayback (ipwb) facilitates permanence and collaboration in web archives by disseminating the contents of [WARC](http://www.iso.org/iso/catalogue_detail.htm?csnumber=44717) files into the IPFS network. [IPFS](https://ipfs.io/) is a peer-to-peer content-addressable file system that inherently allows deduplication and facilitates opt-in replication. ipwb splits the header and payload of WARC response records before disseminating into IPFS to leverage the deduplication, builds a [CDXJ index](https://github.com/oduwsdl/ORS/wiki/CDXJ) with references to the IPFS hashes returned, and combines the header and payload from IPFS at the time of replay.
 
 InterPlanetary Wayback primarily consists of two scripts:
 
 - **ipwb/indexer.py** - archival indexing script that takes the path to a WARC input, extracts the HTTP headers, HTTP payload (response body), and relevant parts of the WARC-response record header from the WARC specified and creates byte string representations. The indexer then pushes the byte strings into IPFS using a locally running IPFS daemon then creates a [CDXJ](https://github.com/oduwsdl/ORS/wiki/CDXJ) file with this metadata for replay.py.
 - **ipwb/replay.py** - rudimentary replay script to resolve requests for archival content contained in IPFS for replay in the browser.
```

### Comparing `ipwb-0.2023.8.16.1719/ipwb.egg-info/SOURCES.txt` & `ipwb-0.2024.5.24.1842/ipwb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/setup.py` & `ipwb-0.2024.5.24.1842/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,19 +22,18 @@
     long_description_content_type="text/markdown",
     provides=[
         'ipwb'
     ],
     install_requires=[
         'warcio>=1.5.3',
         'ipfshttpclient>=0.8.0a',
-        'Flask==2.3.2',
+        'Flask>=3.0',
         'pycryptodome>=3.4.11',
         'requests>=2.19.1',
         'beautifulsoup4>=4.6.3',
-        'six==1.11.0',
         'surt>=0.3.0'
     ],
     tests_require=[
         'flake8>=3.4',
         'pytest>=3.6',
         'pytest-cov',
         'pytest-flake8'
```

### Comparing `ipwb-0.2023.8.16.1719/tests/testUtil.py` & `ipwb-0.2024.5.24.1842/tests/testUtil.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/tests/test_backends.py` & `ipwb-0.2024.5.24.1842/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/tests/test_daemon.py` & `ipwb-0.2024.5.24.1842/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/tests/test_error_handler.py` & `ipwb-0.2024.5.24.1842/tests/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/tests/test_indexing.py` & `ipwb-0.2024.5.24.1842/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/tests/test_ipfs_client.py` & `ipwb-0.2024.5.24.1842/tests/test_ipfs_client.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/tests/test_memento.py` & `ipwb-0.2024.5.24.1842/tests/test_memento.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/tests/test_randomized_add.py` & `ipwb-0.2024.5.24.1842/tests/test_randomized_add.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/tests/test_replay.py` & `ipwb-0.2024.5.24.1842/tests/test_replay.py`

 * *Files identical despite different names*

### Comparing `ipwb-0.2023.8.16.1719/tests/test_util.py` & `ipwb-0.2024.5.24.1842/tests/test_util.py`

 * *Files identical despite different names*

