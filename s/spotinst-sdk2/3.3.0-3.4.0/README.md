# Comparing `tmp/spotinst-sdk2-3.3.0.tar.gz` & `tmp/spotinst-sdk2-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-sdk2-3.3.0.tar", last modified: Thu May 23 05:19:17 2024, max compression
+gzip compressed data, was "spotinst-sdk2-3.4.0.tar", last modified: Fri May 24 06:19:07 2024, max compression
```

## Comparing `spotinst-sdk2-3.3.0.tar` & `spotinst-sdk2-3.4.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.686983 spotinst-sdk2-3.3.0/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    11356 2023-02-24 13:45:28.000000 spotinst-sdk2-3.3.0/LICENSE
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       43 2023-02-24 13:45:28.000000 spotinst-sdk2-3.3.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      751 2023-02-24 13:45:28.000000 spotinst-sdk2-3.3.0/NOTICE.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8093 2024-05-23 05:19:17.686983 spotinst-sdk2-3.3.0/PKG-INFO
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     7177 2023-02-24 13:45:28.000000 spotinst-sdk2-3.3.0/README.md
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       63 2024-05-23 05:19:17.686983 spotinst-sdk2-3.3.0/setup.cfg
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     3535 2024-04-24 11:51:28.000000 spotinst-sdk2-3.3.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.678983 spotinst-sdk2-3.3.0/spotinst_sdk2/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     5098 2024-04-24 11:51:28.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15928 2023-11-20 13:07:49.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.678983 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.678983 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/admin/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12645 2024-02-01 18:22:35.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/admin/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/elastigroup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    78320 2024-04-19 16:12:01.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/elastigroup/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/functions/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3184 2023-11-08 04:20:46.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/functions/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/hpc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3376 2023-11-08 04:20:46.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/hpc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/managed_instance/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11698 2023-11-08 04:20:46.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/managed_instance/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/mcs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      916 2023-11-08 04:20:46.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/mcs/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/mrscaler/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6286 2024-02-25 21:58:42.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/mrscaler/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/ocean/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    80602 2024-04-24 11:51:28.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/ocean/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/ocean_cd/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30586 2023-11-08 04:20:46.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/ocean_cd/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/setup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5562 2023-11-08 04:20:46.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/setup/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/stateful_node/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16650 2023-11-25 09:32:13.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/stateful_node/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/subscription/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3859 2024-01-27 17:33:52.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/clients/subscription/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/admin/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/admin/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      548 2023-02-24 13:45:28.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/admin/user_mapping.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/aws/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    40959 2024-04-19 15:27:36.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/aws/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-11-08 04:20:46.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/aws/asg.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1278 2023-11-08 04:20:46.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/aws/deployment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      931 2023-11-08 04:20:46.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/aws/deployment_action.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-11-08 04:20:46.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/aws/stateful.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/azure_v3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21715 2023-11-08 04:20:46.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/azure_v3/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/gcp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17709 2023-08-16 14:46:57.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/gcp/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/functions/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3685 2023-11-08 04:25:02.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/functions/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/hpc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 14:21:47.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/hpc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/hpc/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4954 2023-11-08 04:25:02.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/hpc/aws/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/managed_instance/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/managed_instance/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/managed_instance/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15583 2024-04-19 15:27:36.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/managed_instance/aws/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/mrscaler/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/mrscaler/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/mrscaler/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18653 2024-02-25 21:58:42.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/mrscaler/aws/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36517 2024-02-25 21:58:42.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean/aws/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean/azure/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22048 2024-05-22 17:35:17.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean/azure/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean/gcp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24001 2024-04-24 11:51:28.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean/gcp/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean_cd/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      806 2023-04-11 10:16:17.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean_cd/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2988 2023-11-08 04:23:08.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean_cd/rollout.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8887 2023-04-11 10:16:17.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean_cd/rollout_spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4154 2023-04-11 10:16:17.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean_cd/strategy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2652 2023-11-08 04:23:37.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean_cd/verification_provider.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9061 2023-11-08 04:23:47.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean_cd/verification_template.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/setup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/setup/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/setup/azure/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1082 2023-02-24 13:45:28.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/setup/azure/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/setup/gcp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1656 2023-02-24 13:45:28.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/setup/gcp/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.682983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/stateful_node/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27588 2024-02-25 21:58:42.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/stateful_node/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.686983 spotinst-sdk2-3.3.0/spotinst_sdk2/models/subscription/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      856 2023-11-08 04:24:10.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/models/subscription/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2615 2023-11-08 04:24:57.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/session.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-05-23 05:18:35.000000 spotinst-sdk2-3.3.0/spotinst_sdk2/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 05:19:17.678983 spotinst-sdk2-3.3.0/spotinst_sdk2.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8093 2024-05-23 05:19:17.000000 spotinst-sdk2-3.3.0/spotinst_sdk2.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2392 2024-05-23 05:19:17.000000 spotinst-sdk2-3.3.0/spotinst_sdk2.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 05:19:17.000000 spotinst-sdk2-3.3.0/spotinst_sdk2.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-23 05:19:17.000000 spotinst-sdk2-3.3.0/spotinst_sdk2.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-05-23 05:19:17.000000 spotinst-sdk2-3.3.0/spotinst_sdk2.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.971996 spotinst-sdk2-3.4.0/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    11356 2023-02-24 13:45:28.000000 spotinst-sdk2-3.4.0/LICENSE
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       43 2023-02-24 13:45:28.000000 spotinst-sdk2-3.4.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      751 2023-02-24 13:45:28.000000 spotinst-sdk2-3.4.0/NOTICE.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8093 2024-05-24 06:19:07.971996 spotinst-sdk2-3.4.0/PKG-INFO
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     7177 2023-02-24 13:45:28.000000 spotinst-sdk2-3.4.0/README.md
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       63 2024-05-24 06:19:07.971996 spotinst-sdk2-3.4.0/setup.cfg
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     3535 2024-04-24 11:51:28.000000 spotinst-sdk2-3.4.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.963996 spotinst-sdk2-3.4.0/spotinst_sdk2/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     5098 2024-04-24 11:51:28.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15928 2023-11-20 13:07:49.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.963996 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.963996 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/admin/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12645 2024-02-01 18:22:35.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/admin/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.963996 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/elastigroup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    78320 2024-04-19 16:12:01.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/elastigroup/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.963996 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/functions/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3184 2023-11-08 04:20:46.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/functions/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.963996 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/hpc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3376 2023-11-08 04:20:46.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/hpc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.963996 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/managed_instance/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11698 2023-11-08 04:20:46.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/managed_instance/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.963996 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/mcs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      916 2023-11-08 04:20:46.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/mcs/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.963996 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/mrscaler/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6286 2024-02-25 21:58:42.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/mrscaler/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/ocean/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    80602 2024-04-24 11:51:28.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/ocean/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/ocean_cd/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30586 2023-11-08 04:20:46.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/ocean_cd/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/setup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5562 2023-11-08 04:20:46.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/setup/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/stateful_node/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16650 2023-11-25 09:32:13.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/stateful_node/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/subscription/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3859 2024-01-27 17:33:52.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/clients/subscription/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/admin/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/admin/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      548 2023-02-24 13:45:28.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/admin/user_mapping.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/aws/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    40959 2024-04-19 15:27:36.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/aws/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-11-08 04:20:46.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/aws/asg.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1278 2023-11-08 04:20:46.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/aws/deployment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      931 2023-11-08 04:20:46.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/aws/deployment_action.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-11-08 04:20:46.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/aws/stateful.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/azure_v3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21715 2023-11-08 04:20:46.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/azure_v3/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/gcp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17709 2023-08-16 14:46:57.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/gcp/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/functions/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3685 2023-11-08 04:25:02.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/functions/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/hpc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 14:21:47.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/hpc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/hpc/aws/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4954 2023-11-08 04:25:02.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/hpc/aws/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/managed_instance/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/managed_instance/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/managed_instance/aws/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15583 2024-04-19 15:27:36.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/managed_instance/aws/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/mrscaler/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/mrscaler/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/mrscaler/aws/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18653 2024-02-25 21:58:42.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/mrscaler/aws/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean/aws/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36517 2024-02-25 21:58:42.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean/aws/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean/azure/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22048 2024-05-22 17:35:17.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean/azure/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.967996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean/gcp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24001 2024-04-24 11:51:28.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean/gcp/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.971996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean_cd/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      806 2023-04-11 10:16:17.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean_cd/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2988 2023-11-08 04:23:08.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean_cd/rollout.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8887 2023-04-11 10:16:17.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean_cd/rollout_spec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4154 2023-04-11 10:16:17.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean_cd/strategy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2652 2023-11-08 04:23:37.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean_cd/verification_provider.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9061 2023-11-08 04:23:47.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean_cd/verification_template.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.971996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/setup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/setup/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.971996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/setup/azure/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1082 2023-02-24 13:45:28.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/setup/azure/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.971996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/setup/gcp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1656 2023-02-24 13:45:28.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/setup/gcp/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.971996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/stateful_node/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27712 2024-05-24 06:18:57.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/stateful_node/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.971996 spotinst-sdk2-3.4.0/spotinst_sdk2/models/subscription/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      856 2023-11-08 04:24:10.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/models/subscription/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2615 2023-11-08 04:24:57.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/session.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-05-24 06:18:57.000000 spotinst-sdk2-3.4.0/spotinst_sdk2/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 06:19:07.963996 spotinst-sdk2-3.4.0/spotinst_sdk2.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8093 2024-05-24 06:19:07.000000 spotinst-sdk2-3.4.0/spotinst_sdk2.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2392 2024-05-24 06:19:07.000000 spotinst-sdk2-3.4.0/spotinst_sdk2.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-24 06:19:07.000000 spotinst-sdk2-3.4.0/spotinst_sdk2.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-24 06:19:07.000000 spotinst-sdk2-3.4.0/spotinst_sdk2.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-05-24 06:19:07.000000 spotinst-sdk2-3.4.0/spotinst_sdk2.egg-info/top_level.txt
```

### Comparing `spotinst-sdk2-3.3.0/LICENSE` & `spotinst-sdk2-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/NOTICE.md` & `spotinst-sdk2-3.4.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/PKG-INFO` & `spotinst-sdk2-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-sdk2
-Version: 3.3.0
+Version: 3.4.0
 Summary: A Python SDK for Spotinst
 Home-page: https://github.com/spotinst/spotinst-sdk-python
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst spot instances aws azure ec2 cloud infrastructure development elastigroup
 Platform: UNKNOWN
```

### Comparing `spotinst-sdk2-3.3.0/README.md` & `spotinst-sdk2-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/setup.py` & `spotinst-sdk2-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/client.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/client.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/clients/admin/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/clients/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/clients/elastigroup/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/clients/elastigroup/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/clients/functions/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/clients/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/clients/hpc/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/clients/hpc/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/clients/managed_instance/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/clients/managed_instance/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/clients/mcs/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/clients/mcs/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/clients/mrscaler/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/clients/mrscaler/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/clients/ocean/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/clients/ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/clients/ocean_cd/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/clients/ocean_cd/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/clients/setup/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/clients/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/clients/stateful_node/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/clients/stateful_node/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/clients/subscription/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/clients/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/admin/user_mapping.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/admin/user_mapping.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/aws/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/aws/asg.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/aws/asg.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/aws/deployment.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/aws/deployment.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/aws/deployment_action.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/aws/deployment_action.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/aws/stateful.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/aws/stateful.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/azure_v3/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/azure_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/elastigroup/gcp/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/elastigroup/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/functions/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/hpc/aws/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/hpc/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/managed_instance/aws/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/managed_instance/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/mrscaler/aws/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/mrscaler/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean/aws/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean/azure/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean/gcp/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean_cd/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean_cd/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean_cd/rollout.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean_cd/rollout.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean_cd/rollout_spec.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean_cd/rollout_spec.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean_cd/strategy.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean_cd/strategy.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean_cd/verification_provider.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean_cd/verification_provider.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/ocean_cd/verification_template.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/ocean_cd/verification_template.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/setup/azure/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/setup/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/setup/gcp/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/setup/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/stateful_node/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/stateful_node/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -892,20 +892,22 @@
 
 class DeallocationConfig:
     def __init__(self,
                  disk_deallocation_config: Deallocate = none,
                  network_deallocation_config: Deallocate = none,
                  public_ip_deallocation_config: Deallocate = none,
                  snapshot_deallocation_config: Deallocate = none,
-                 should_terminate_vm: bool = none):
+                 should_terminate_vm: bool = none,
+                 should_deregister_from_lb: bool = none):
         self.disk_deallocation_config = disk_deallocation_config
         self.network_deallocation_config = network_deallocation_config
         self.public_ip_deallocation_config = public_ip_deallocation_config
         self.snapshot_deallocation_config = snapshot_deallocation_config
         self.should_terminate_vm = should_terminate_vm
+        self.should_deregister_from_lb = should_deregister_from_lb
 
     def toJSON(self):
         return json.dumps(self, default=lambda o: o.__dict__,
                           sort_keys=True, indent=4)
 
 
 class DeleteStatefulNodeRequest:
```

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/models/subscription/__init__.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/models/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2/session.py` & `spotinst-sdk2-3.4.0/spotinst_sdk2/session.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2.egg-info/PKG-INFO` & `spotinst-sdk2-3.4.0/spotinst_sdk2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-sdk2
-Version: 3.3.0
+Version: 3.4.0
 Summary: A Python SDK for Spotinst
 Home-page: https://github.com/spotinst/spotinst-sdk-python
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst spot instances aws azure ec2 cloud infrastructure development elastigroup
 Platform: UNKNOWN
```

### Comparing `spotinst-sdk2-3.3.0/spotinst_sdk2.egg-info/SOURCES.txt` & `spotinst-sdk2-3.4.0/spotinst_sdk2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

