# Comparing `tmp/vss-cli-2024.5.0.dev4.tar.gz` & `tmp/vss-cli-2024.5.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vss-cli-2024.5.0.dev4.tar", last modified: Wed May 22 20:25:40 2024, max compression
+gzip compressed data, was "vss-cli-2024.5.0.dev5.tar", last modified: Thu May 23 18:20:38 2024, max compression
```

## Comparing `vss-cli-2024.5.0.dev4.tar` & `vss-cli-2024.5.0.dev5.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:25:40.177055 vss-cli-2024.5.0.dev4/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13867 2024-05-22 20:25:40.177055 vss-cli-2024.5.0.dev4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10991 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/README.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1257 2024-05-22 20:25:40.177055 vss-cli-2024.5.0.dev4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3827 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:25:40.157055 vss-cli-2024.5.0.dev4/tests/
--rw-rw-rw-   0 root         (0) root         (0)     5569 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/tests/test_vss_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:25:40.161055 vss-cli-2024.5.0.dev4/vss_cli/
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19671 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/autocompletion.py
--rw-rw-rw-   0 root         (0) root         (0)     7453 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    64867 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/config.py
--rw-rw-rw-   0 root         (0) root         (0)    15476 2024-05-22 20:21:22.000000 vss-cli-2024.5.0.dev4/vss_cli/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:25:40.165055 vss-cli-2024.5.0.dev4/vss_cli/data/
--rw-rw-rw-   0 root         (0) root         (0)     4500 2024-05-22 20:21:22.000000 vss-cli-2024.5.0.dev4/vss_cli/data/clib.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4288 2024-05-22 20:21:22.000000 vss-cli-2024.5.0.dev4/vss_cli/data/clone.yaml
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/data/config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2892 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/data/image.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2926 2024-05-22 20:21:22.000000 vss-cli-2024.5.0.dev4/vss_cli/data/shell.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4198 2024-05-22 20:21:22.000000 vss-cli-2024.5.0.dev4/vss_cli/data/template.yaml
--rw-rw-rw-   0 root         (0) root         (0)    25848 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/data_types.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/hcio.py
--rw-rw-rw-   0 root         (0) root         (0)    12512 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:25:40.169055 vss-cli-2024.5.0.dev4/vss_cli/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 20:25:36.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15976 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/account.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/completion.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:25:40.173055 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8906 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/callbacks.py
--rw-rw-rw-   0 root         (0) root         (0)     4015 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/contentlib.py
--rw-rw-rw-   0 root         (0) root         (0)     2813 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/domain.py
--rw-rw-rw-   0 root         (0) root         (0)     3133 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/floppy.py
--rw-rw-rw-   0 root         (0) root         (0)     8680 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/helper.py
--rw-rw-rw-   0 root         (0) root         (0)     3287 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/image.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     3046 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/iso.py
--rw-rw-rw-   0 root         (0) root         (0)     3477 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/net.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/os.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/rel_args.py
--rw-rw-rw-   0 root         (0) root         (0)     9604 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/rel_opts.py
--rw-rw-rw-   0 root         (0) root         (0)     3790 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/template.py
--rw-rw-rw-   0 root         (0) root         (0)   150499 2024-05-22 20:21:22.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/vm.py
--rw-rw-rw-   0 root         (0) root         (0)     1907 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/vmdks.py
--rw-rw-rw-   0 root         (0) root         (0)    10871 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/configure.py
--rw-rw-rw-   0 root         (0) root         (0)     3481 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/key.py
--rw-rw-rw-   0 root         (0) root         (0)     3010 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/message.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     4310 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/ovf.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/plugins.py
--rw-rw-rw-   0 root         (0) root         (0)     1362 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/raw.py
--rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:25:40.173055 vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5330 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/change.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/export.py
--rw-rw-rw-   0 root         (0) root         (0)     2372 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     2362 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/image.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     2860 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/new.py
--rw-rw-rw-   0 root         (0) root         (0)     2366 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/restore.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/retirement.py
--rw-rw-rw-   0 root         (0) root         (0)     3307 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/snapshot.py
--rw-rw-rw-   0 root         (0) root         (0)     2246 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/vmdk.py
--rw-rw-rw-   0 root         (0) root         (0)     1614 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/service.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/shell.py
--rw-rw-rw-   0 root         (0) root         (0)     2325 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/status.py
--rw-rw-rw-   0 root         (0) root         (0)     6761 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/stor.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/token.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/plugins/upgrade.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/rel_opts.py
--rw-rw-rw-   0 root         (0) root         (0)     2864 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/sstatus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:25:40.173055 vss-cli-2024.5.0.dev4/vss_cli/utils/
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    75203 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/utils/emoji.py
--rw-rw-rw-   0 root         (0) root         (0)     2929 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/utils/threading.py
--rw-rw-rw-   0 root         (0) root         (0)     4734 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/vss.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/vssconst.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev4/vss_cli/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:25:40.173055 vss-cli-2024.5.0.dev4/vss_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13867 2024-05-22 20:25:40.000000 vss-cli-2024.5.0.dev4/vss_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2453 2024-05-22 20:25:40.000000 vss-cli-2024.5.0.dev4/vss_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 20:25:40.000000 vss-cli-2024.5.0.dev4/vss_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-22 20:25:40.000000 vss-cli-2024.5.0.dev4/vss_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 20:25:40.000000 vss-cli-2024.5.0.dev4/vss_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      679 2024-05-22 20:25:40.000000 vss-cli-2024.5.0.dev4/vss_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-22 20:25:40.000000 vss-cli-2024.5.0.dev4/vss_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 18:20:38.338788 vss-cli-2024.5.0.dev5/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13909 2024-05-23 18:20:38.338788 vss-cli-2024.5.0.dev5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10991 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2024-05-23 18:20:38.338788 vss-cli-2024.5.0.dev5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3827 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 18:20:38.322788 vss-cli-2024.5.0.dev5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5569 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/tests/test_vss_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 18:20:38.322788 vss-cli-2024.5.0.dev5/vss_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19671 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/autocompletion.py
+-rw-rw-rw-   0 root         (0) root         (0)     7449 2024-05-23 18:19:57.000000 vss-cli-2024.5.0.dev5/vss_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    64867 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15466 2024-05-23 18:19:57.000000 vss-cli-2024.5.0.dev5/vss_cli/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 18:20:38.326788 vss-cli-2024.5.0.dev5/vss_cli/data/
+-rw-rw-rw-   0 root         (0) root         (0)     4500 2024-05-23 18:19:57.000000 vss-cli-2024.5.0.dev5/vss_cli/data/clib.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4288 2024-05-23 18:19:57.000000 vss-cli-2024.5.0.dev5/vss_cli/data/clone.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/data/config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/data/image.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2926 2024-05-23 18:19:57.000000 vss-cli-2024.5.0.dev5/vss_cli/data/shell.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2024-05-23 18:19:57.000000 vss-cli-2024.5.0.dev5/vss_cli/data/template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    25848 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/hcio.py
+-rw-rw-rw-   0 root         (0) root         (0)    12512 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 18:20:38.330788 vss-cli-2024.5.0.dev5/vss_cli/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 18:20:33.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15976 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/completion.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 18:20:38.330788 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8906 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/callbacks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/contentlib.py
+-rw-rw-rw-   0 root         (0) root         (0)     2813 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3133 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/floppy.py
+-rw-rw-rw-   0 root         (0) root         (0)     8680 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3287 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/iso.py
+-rw-rw-rw-   0 root         (0) root         (0)     3477 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/net.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/os.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/rel_args.py
+-rw-rw-rw-   0 root         (0) root         (0)     9604 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/rel_opts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3790 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/template.py
+-rw-rw-rw-   0 root         (0) root         (0)   150499 2024-05-22 20:21:22.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/vm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1907 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/vmdks.py
+-rw-rw-rw-   0 root         (0) root         (0)    10871 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/key.py
+-rw-rw-rw-   0 root         (0) root         (0)     3010 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4310 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/ovf.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/raw.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 18:20:38.334788 vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/change.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/export.py
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2362 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/new.py
+-rw-rw-rw-   0 root         (0) root         (0)     2366 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/restore.py
+-rw-rw-rw-   0 root         (0) root         (0)     3924 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/retirement.py
+-rw-rw-rw-   0 root         (0) root         (0)     3307 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/snapshot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2246 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/vmdk.py
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)     2325 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/status.py
+-rw-rw-rw-   0 root         (0) root         (0)     6761 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/stor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/token.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/plugins/upgrade.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/rel_opts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2864 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/sstatus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 18:20:38.334788 vss-cli-2024.5.0.dev5/vss_cli/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    75203 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/utils/emoji.py
+-rw-rw-rw-   0 root         (0) root         (0)     2929 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/utils/threading.py
+-rw-rw-rw-   0 root         (0) root         (0)     4734 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/vss.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/vssconst.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev5/vss_cli/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 18:20:38.334788 vss-cli-2024.5.0.dev5/vss_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13909 2024-05-23 18:20:38.000000 vss-cli-2024.5.0.dev5/vss_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2453 2024-05-23 18:20:38.000000 vss-cli-2024.5.0.dev5/vss_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 18:20:38.000000 vss-cli-2024.5.0.dev5/vss_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-23 18:20:38.000000 vss-cli-2024.5.0.dev5/vss_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 18:20:38.000000 vss-cli-2024.5.0.dev5/vss_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      706 2024-05-23 18:20:38.000000 vss-cli-2024.5.0.dev5/vss_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-23 18:20:38.000000 vss-cli-2024.5.0.dev5/vss_cli.egg-info/top_level.txt
```

### Comparing `vss-cli-2024.5.0.dev4/LICENSE` & `vss-cli-2024.5.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/PKG-INFO` & `vss-cli-2024.5.0.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vss-cli
-Version: 2024.5.0.dev4
+Version: 2024.5.0.dev5
 Summary: ITS Private Cloud Command Line Interface
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.5.0-dev4.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.5.0-dev5.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/issues
 Project-URL: Documentation, https://eis.utoronto.ca/~vss/vss-cli/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
@@ -42,14 +42,15 @@
 Requires-Dist: validators==0.20.0
 Requires-Dist: click-spinner==0.1.10
 Requires-Dist: ruamel.yaml==0.17.21
 Requires-Dist: qrcode==7.3.1
 Requires-Dist: pyjwt==2.6.0
 Requires-Dist: xmltodict==0.13.0
 Requires-Dist: setuptools==68.2.2
+Requires-Dist: importlib-resources==6.4.0
 Provides-Extra: test
 Requires-Dist: flake8==6.0.0; extra == "test"
 Requires-Dist: nose==1.3.7; extra == "test"
 Requires-Dist: coverage==6.5.0; extra == "test"
 Requires-Dist: pytz==2022.6; extra == "test"
 Requires-Dist: wheel==0.38.4; extra == "test"
 Requires-Dist: minio==7.2.7; extra == "test"
```

### Comparing `vss-cli-2024.5.0.dev4/README.md` & `vss-cli-2024.5.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/setup.cfg` & `vss-cli-2024.5.0.dev5/setup.cfg`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/setup.py` & `vss-cli-2024.5.0.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/tests/test_vss_cli.py` & `vss-cli-2024.5.0.dev5/tests/test_vss_cli.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/autocompletion.py` & `vss-cli-2024.5.0.dev5/vss_cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/cli.py` & `vss-cli-2024.5.0.dev5/vss_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import logging
 import os
 import platform
 import sys
 from typing import List, Optional, Union, cast
 
 import click
-from click.core import Command, Context, Group
 import click_log
+from click.core import Command, Context, Group
 from pyvss.const import __version__ as pyvss_version
 
 import vss_cli.autocompletion as autocompletion
-from vss_cli.config import Configuration
 import vss_cli.const as const
+from vss_cli.config import Configuration
 from vss_cli.helper import to_tuples
 
 click_log.basic_config()
 
 _LOGGER = logging.getLogger(__name__)
 
 CONTEXT_SETTINGS = dict(auto_envvar_prefix='VSS')
@@ -140,15 +140,15 @@
     help='The API password for VSS API.',
     envvar='VSS_USER_PASS',
 )
 @click.option(
     '--totp',
     default=_default_token,
     help='Timed One Time Password.',
-    envvar='VSS_API_USER_OTP',
+    envvar='VSS_USER_OTP',
 )
 @click.option(
     '--timeout',
     help='Timeout for network operations.',
     type=click.INT,
     envvar='VSS_TIMEOUT',
     show_default=True,
```

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/config.py` & `vss-cli-2024.5.0.dev5/vss_cli/config.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/const.py` & `vss-cli-2024.5.0.dev5/vss_cli/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Constants used by VSS CLI (vss-cli)."""
 import os
-
-import pkg_resources
+from importlib import resources
 
 PACKAGE_NAME = "vss_cli"
 
-__version__ = "2024.5.0-dev4"
+__version__ = "2024.5.0-dev5"
 
 
 DEFAULT_TIMEOUT = 30
 DEFAULT_ENDPOINT = "https://cloud-api.eis.utoronto.ca"
 DEFAULT_ENDPOINT_NAME = "cloud-api"
 DEFAULT_S3_SERVER = "https://vskey-stor.eis.utoronto.ca"
 _LEGACY_CONFIG = ("~", ".vss-cli", "config.json")
@@ -19,16 +18,16 @@
 
 COLUMNS_WIDTH_DEFAULT = -1
 COLUMNS_WIDTH_STR = "\u2026"
 
 LEGACY_CONFIG = os.path.expanduser(os.path.join(*_LEGACY_CONFIG))
 DEFAULT_CONFIG = os.path.expanduser(os.path.join(*_DEFAULT_CONFIG))
 DEFAULT_HISTORY = os.path.expanduser(os.path.join(*_DEFAULT_HISTORY))
-DEFAULT_DATA_PATH = pkg_resources.resource_filename(PACKAGE_NAME, "data")
-DEFAULT_CONFIG_TMPL = os.path.join(DEFAULT_DATA_PATH, "config.yaml")
+DEFAULT_DATA_PATH = resources.files(PACKAGE_NAME) / "data"
+DEFAULT_CONFIG_TMPL = DEFAULT_DATA_PATH.joinpath("config.yaml")
 DEFAULT_CHECK_UPDATES = True
 DEFAULT_CHECK_MESSAGES = True
 DEFAULT_TOTP = False
 
 DEFAULT_TABLE_FORMAT = "simple"
 DEFAULT_DATA_OUTPUT = "table"
 DEFAULT_RAW_OUTPUT = "json"
```

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/data/clib.yaml` & `vss-cli-2024.5.0.dev5/vss_cli/data/clib.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from CLib 2024.5.0-dev4             #
+#     VSS-CLI Spec from CLib 2024.5.0-dev5             #
 ####################################################
 built: clib               # Required: Do not remove.
 machine:
   item: ubuntu-22.04      # Required: Source content library id OVF.
   cpu: 1                  # Optional: CPU count (Default: 1).
   memory: 1               # Optional: Memory in GB (Default: 1GB).
   name: &name Vm-Name     # Required: Target virtual machine name.
```

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/data/clone.yaml` & `vss-cli-2024.5.0.dev5/vss_cli/data/clone.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from Clone 2024.5.0-dev4             #
+#     VSS-CLI Spec from Clone 2024.5.0-dev5             #
 ####################################################
 built: clone              # Required: Do not remove.
 machine:
   source: SourceVM        # Required: Can be a vm name or a vm id.
   name: &name Vm-Name     # Required: Target virtual machine name
   disks:                  # Optional: Disks (Default: source vm disk layout)
     - capacity_gb: 40     # Optional: Disk capacity in GB (Default: source vm disk capacity)
```

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/data/config.yaml` & `vss-cli-2024.5.0.dev5/vss_cli/data/config.yaml`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/data/image.yaml` & `vss-cli-2024.5.0.dev5/vss_cli/data/image.yaml`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/data/shell.yaml` & `vss-cli-2024.5.0.dev5/vss_cli/data/shell.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec shell VM 2024.5.0-dev4             #
+#     VSS-CLI Spec shell VM 2024.5.0-dev5             #
 ####################################################
 built: os_install         # Required: Do not remove.
 machine:
   name: Vm-Name            # Required: Target virtual machine name.
   os: ubuntu64Guest              # Required: Guest Operating System name or Id.
   cpu: 1                   # Optional: CPU count (Default: 1).
   memory: 1                # Optional: Memory in GB (Default: 1GB).
```

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/data/template.yaml` & `vss-cli-2024.5.0.dev5/vss_cli/data/template.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from Template 2024.5.0-dev4        #
+#     VSS-CLI Spec from Template 2024.5.0-dev5        #
 ####################################################
 built: template           # Required: Do not remove.
 machine:
   source: NixSource                # Required: Can be a vm name or a vm id.
   name: &name Vm-Name     # Required: Target virtual machine name
   folder: MyFolder       # Optional: Folder name, path or ID (Default: source vm folder)
   disks:                  # Optional: Disks (Default: source vm disk layout)
```

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/data_types.py` & `vss-cli-2024.5.0.dev5/vss_cli/data_types.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/hcio.py` & `vss-cli-2024.5.0.dev5/vss_cli/hcio.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/helper.py` & `vss-cli-2024.5.0.dev5/vss_cli/helper.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/account.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/account.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/completion.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/completion.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/callbacks.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/callbacks.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/contentlib.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/contentlib.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/domain.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/domain.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/floppy.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/floppy.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/folder.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/folder.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/helper.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/helper.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/image.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/image.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/inventory.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/inventory.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/iso.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/iso.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/net.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/net.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/os.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/os.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/rel_args.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/rel_args.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/rel_opts.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/rel_opts.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/template.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/template.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/vm.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/vm.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/compute_plugins/vmdks.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/compute_plugins/vmdks.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/configure.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/configure.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/key.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/key.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/message.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/message.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/misc.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/misc.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/ovf.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/ovf.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/plugins.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/raw.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/raw.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/request.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/request.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/change.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/change.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/export.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/export.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/folder.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/folder.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/image.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/image.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/inventory.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/inventory.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/new.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/new.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/restore.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/restore.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/retirement.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/retirement.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/snapshot.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/snapshot.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/request_plugins/vmdk.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/request_plugins/vmdk.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/service.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/service.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/shell.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/status.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/status.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/stor.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/stor.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/token.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/token.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/plugins/upgrade.py` & `vss-cli-2024.5.0.dev5/vss_cli/plugins/upgrade.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/rel_opts.py` & `vss-cli-2024.5.0.dev5/vss_cli/rel_opts.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/sstatus.py` & `vss-cli-2024.5.0.dev5/vss_cli/sstatus.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/utils/emoji.py` & `vss-cli-2024.5.0.dev5/vss_cli/utils/emoji.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/utils/threading.py` & `vss-cli-2024.5.0.dev5/vss_cli/utils/threading.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/validators.py` & `vss-cli-2024.5.0.dev5/vss_cli/validators.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/vss.py` & `vss-cli-2024.5.0.dev5/vss_cli/vss.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli/yaml.py` & `vss-cli-2024.5.0.dev5/vss_cli/yaml.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli.egg-info/PKG-INFO` & `vss-cli-2024.5.0.dev5/vss_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vss-cli
-Version: 2024.5.0.dev4
+Version: 2024.5.0.dev5
 Summary: ITS Private Cloud Command Line Interface
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.5.0-dev4.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.5.0-dev5.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/issues
 Project-URL: Documentation, https://eis.utoronto.ca/~vss/vss-cli/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
@@ -42,14 +42,15 @@
 Requires-Dist: validators==0.20.0
 Requires-Dist: click-spinner==0.1.10
 Requires-Dist: ruamel.yaml==0.17.21
 Requires-Dist: qrcode==7.3.1
 Requires-Dist: pyjwt==2.6.0
 Requires-Dist: xmltodict==0.13.0
 Requires-Dist: setuptools==68.2.2
+Requires-Dist: importlib-resources==6.4.0
 Provides-Extra: test
 Requires-Dist: flake8==6.0.0; extra == "test"
 Requires-Dist: nose==1.3.7; extra == "test"
 Requires-Dist: coverage==6.5.0; extra == "test"
 Requires-Dist: pytz==2022.6; extra == "test"
 Requires-Dist: wheel==0.38.4; extra == "test"
 Requires-Dist: minio==7.2.7; extra == "test"
```

### Comparing `vss-cli-2024.5.0.dev4/vss_cli.egg-info/SOURCES.txt` & `vss-cli-2024.5.0.dev5/vss_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev4/vss_cli.egg-info/requires.txt` & `vss-cli-2024.5.0.dev5/vss_cli.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 validators==0.20.0
 click-spinner==0.1.10
 ruamel.yaml==0.17.21
 qrcode==7.3.1
 pyjwt==2.6.0
 xmltodict==0.13.0
 setuptools==68.2.2
+importlib-resources==6.4.0
 
 [dev]
 flake8==6.0.0
 nose==1.3.7
 coverage==6.5.0
 pytz==2022.6
 wheel==0.38.4
```

