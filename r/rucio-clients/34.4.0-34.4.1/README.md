# Comparing `tmp/rucio_clients-34.4.0.tar.gz` & `tmp/rucio_clients-34.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio_clients-34.4.0.tar", last modified: Tue May 21 14:54:26 2024, max compression
+gzip compressed data, was "rucio_clients-34.4.1.tar", last modified: Fri May 24 12:25:35 2024, max compression
```

## Comparing `rucio_clients-34.4.0.tar` & `rucio_clients-34.4.1.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.463628 rucio_clients-34.4.0/
--rwxr-xr-x   0 root         (0) root         (0)     4487 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio_clients-34.4.0/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio_clients-34.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      598 2024-05-21 14:54:22.000000 rucio_clients-34.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2024-05-21 14:54:26.463628 rucio_clients-34.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1982 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.425627 rucio_clients-34.4.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)   127119 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/bin/rucio
--rwxr-xr-x   0 root         (0) root         (0)   133582 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/bin/rucio-admin
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.426627 rucio_clients-34.4.0/etc/
--rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio_clients-34.4.0/etc/rse-accounts.cfg.template
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio_clients-34.4.0/etc/rucio.cfg.atlas.client.template
--rw-r--r--   0 root         (0) root         (0)     8534 2024-05-06 09:19:47.000000 rucio_clients-34.4.0/etc/rucio.cfg.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.422627 rucio_clients-34.4.0/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.426627 rucio_clients-34.4.0/lib/rucio/
--rw-r--r--   0 root         (0) root         (0)      660 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      690 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/alembicrevision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.431627 rucio_clients-34.4.0/lib/rucio/client/
--rw-r--r--   0 root         (0) root         (0)      660 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16352 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/accountclient.py
--rw-r--r--   0 root         (0) root         (0)     5961 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/accountlimitclient.py
--rw-r--r--   0 root         (0) root         (0)    48035 2024-05-21 07:56:54.000000 rucio_clients-34.4.0/lib/rucio/client/baseclient.py
--rw-r--r--   0 root         (0) root         (0)     3079 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/client.py
--rw-r--r--   0 root         (0) root         (0)     4401 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/configclient.py
--rw-r--r--   0 root         (0) root         (0)     1989 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/credentialclient.py
--rw-r--r--   0 root         (0) root         (0)    28378 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/didclient.py
--rw-r--r--   0 root         (0) root         (0)     2114 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/diracclient.py
--rw-r--r--   0 root         (0) root         (0)    87520 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/downloadclient.py
--rw-r--r--   0 root         (0) root         (0)     1575 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/exportclient.py
--rw-r--r--   0 root         (0) root         (0)     1610 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/fileclient.py
--rw-r--r--   0 root         (0) root         (0)     1469 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/importclient.py
--rw-r--r--   0 root         (0) root         (0)     2822 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/lifetimeclient.py
--rw-r--r--   0 root         (0) root         (0)     3914 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/lockclient.py
--rw-r--r--   0 root         (0) root         (0)     5195 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/metaconventionsclient.py
--rw-r--r--   0 root         (0) root         (0)     1390 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/pingclient.py
--rw-r--r--   0 root         (0) root         (0)    19518 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/replicaclient.py
--rw-r--r--   0 root         (0) root         (0)     4197 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/requestclient.py
--rw-r--r--   0 root         (0) root         (0)    27121 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/rseclient.py
--rw-r--r--   0 root         (0) root         (0)    12734 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/ruleclient.py
--rw-r--r--   0 root         (0) root         (0)     3147 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/scopeclient.py
--rw-r--r--   0 root         (0) root         (0)     7971 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/subscriptionclient.py
--rw-r--r--   0 root         (0) root         (0)     2642 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/touchclient.py
--rw-r--r--   0 root         (0) root         (0)    46627 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/uploadclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.435627 rucio_clients-34.4.0/lib/rucio/common/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2301 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/cache.py
--rw-r--r--   0 root         (0) root         (0)    24636 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/config.py
--rw-r--r--   0 root         (0) root         (0)     5507 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/constants.py
--rw-r--r--   0 root         (0) root         (0)      726 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/constraints.py
--rwxr-xr-x   0 root         (0) root         (0)     6545 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/didtype.py
--rw-r--r--   0 root         (0) root         (0)    32345 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/exception.py
--rw-r--r--   0 root         (0) root         (0)     1398 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/extra.py
--rw-r--r--   0 root         (0) root         (0)    15046 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/logging.py
--rw-r--r--   0 root         (0) root         (0)    45338 2024-05-21 07:56:54.000000 rucio_clients-34.4.0/lib/rucio/common/pcache.py
--rw-r--r--   0 root         (0) root         (0)     6071 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/plugins.py
--rw-r--r--   0 root         (0) root         (0)     3085 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.437627 rucio_clients-34.4.0/lib/rucio/common/schema/
--rw-r--r--   0 root         (0) root         (0)     5384 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15589 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/schema/atlas.py
--rw-r--r--   0 root         (0) root         (0)    15406 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/schema/belleii.py
--rw-r--r--   0 root         (0) root         (0)    14987 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/schema/domatpc.py
--rw-r--r--   0 root         (0) root         (0)    15926 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/schema/escape.py
--rw-r--r--   0 root         (0) root         (0)    16241 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/schema/generic.py
--rw-r--r--   0 root         (0) root         (0)    15468 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/schema/generic_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)    15277 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/schema/icecube.py
--rw-r--r--   0 root         (0) root         (0)     5414 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/stomp_utils.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/stopwatch.py
--rw-r--r--   0 root         (0) root         (0)     4935 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)     5716 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/types.py
--rw-r--r--   0 root         (0) root         (0)    79163 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/lib/rucio/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.437627 rucio_clients-34.4.0/lib/rucio/rse/
--rw-r--r--   0 root         (0) root         (0)     3303 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.441627 rucio_clients-34.4.0/lib/rucio/rse/protocols/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7199 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/bittorrent.py
--rw-r--r--   0 root         (0) root         (0)     4603 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/cache.py
--rw-r--r--   0 root         (0) root         (0)     4225 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/dummy.py
--rw-r--r--   0 root         (0) root         (0)    29100 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/gfal.py
--rw-r--r--   0 root         (0) root         (0)     9730 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/globus.py
--rw-r--r--   0 root         (0) root         (0)     3411 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/gsiftp.py
--rw-r--r--   0 root         (0) root         (0)     2975 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/http_cache.py
--rw-r--r--   0 root         (0) root         (0)     4495 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/mock.py
--rw-r--r--   0 root         (0) root         (0)     7224 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/ngarc.py
--rw-r--r--   0 root         (0) root         (0)    10414 2024-05-21 07:56:54.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/posix.py
--rw-r--r--   0 root         (0) root         (0)    21937 2024-05-21 07:56:16.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/protocol.py
--rw-r--r--   0 root         (0) root         (0)    15260 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/rclone.py
--rw-r--r--   0 root         (0) root         (0)     5501 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/rfio.py
--rw-r--r--   0 root         (0) root         (0)    14689 2024-05-21 07:56:54.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/srm.py
--rw-r--r--   0 root         (0) root         (0)    17473 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/ssh.py
--rw-r--r--   0 root         (0) root         (0)     8141 2024-05-21 07:56:54.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/storm.py
--rw-r--r--   0 root         (0) root         (0)    22448 2024-05-21 07:56:54.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/webdav.py
--rw-r--r--   0 root         (0) root         (0)    12571 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/xrootd.py
--rw-r--r--   0 root         (0) root         (0)    37238 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/rsemanager.py
--rw-r--r--   0 root         (0) root         (0)      244 2024-05-21 12:45:12.000000 rucio_clients-34.4.0/lib/rucio/vcsversion.py
--rw-r--r--   0 root         (0) root         (0)     1577 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.461628 rucio_clients-34.4.0/lib/rucio_clients.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5117 2024-05-21 14:54:26.000000 rucio_clients-34.4.0/lib/rucio_clients.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    16384 2024-05-06 09:19:47.000000 rucio_clients-34.4.0/pylintrc
--rw-r--r--   0 root         (0) root         (0)     5763 2024-05-21 07:56:54.000000 rucio_clients-34.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5235 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      206 2024-05-21 14:54:26.464628 rucio_clients-34.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3050 2024-05-21 14:54:22.000000 rucio_clients-34.4.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     4778 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/setuputil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.461628 rucio_clients-34.4.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3682 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_abacus_account.py
--rw-r--r--   0 root         (0) root         (0)    10677 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_abacus_collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3229 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_abacus_rse.py
--rw-r--r--   0 root         (0) root         (0)    15923 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_account.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_account_limits.py
--rw-r--r--   0 root         (0) root         (0)    20523 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_api_external_representation.py
--rw-r--r--   0 root         (0) root         (0)    13352 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_archive.py
--rw-r--r--   0 root         (0) root         (0)     4074 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_auditor.py
--rw-r--r--   0 root         (0) root         (0)     2181 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_auditor_hdfs.py
--rw-r--r--   0 root         (0) root         (0)     4201 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_auditor_srmdumps.py
--rw-r--r--   0 root         (0) root         (0)    14964 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_authentication.py
--rw-r--r--   0 root         (0) root         (0)     3464 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_automatix.py
--rw-r--r--   0 root         (0) root         (0)    23265 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_bad_replica.py
--rw-r--r--   0 root         (0) root         (0)    12425 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_bb8.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_belleii.py
--rwxr-xr-x   0 root         (0) root         (0)   107450 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_bin_rucio.py
--rw-r--r--   0 root         (0) root         (0)     2065 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)     8398 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_clients.py
--rw-r--r--   0 root         (0) root         (0)     1865 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_common_types.py
--rw-r--r--   0 root         (0) root         (0)     6942 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    96724 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_conveyor.py
--rw-r--r--   0 root         (0) root         (0)    23870 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_conveyor_submitter.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_counter.py
--rw-r--r--   0 root         (0) root         (0)     7728 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_credential.py
--rw-r--r--   0 root         (0) root         (0)     7337 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_curl.py
--rw-r--r--   0 root         (0) root         (0)     2618 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_daemons.py
--rw-r--r--   0 root         (0) root         (0)    28183 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_dataset_replicas.py
--rw-r--r--   0 root         (0) root         (0)     2736 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_db.py
--rw-r--r--   0 root         (0) root         (0)    58823 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_did.py
--rw-r--r--   0 root         (0) root         (0)    29517 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_did_meta_plugins.py
--rw-r--r--   0 root         (0) root         (0)     4185 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_didtype.py
--rw-r--r--   0 root         (0) root         (0)    35315 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)     7118 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_dumper.py
--rw-r--r--   0 root         (0) root         (0)    16419 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_dumper_consistency.py
--rw-r--r--   0 root         (0) root         (0)    10869 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_dumper_data_model.py
--rw-r--r--   0 root         (0) root         (0)     3082 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_dumper_path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    38301 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     7953 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    10106 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_hermes.py
--rw-r--r--   0 root         (0) root         (0)     5821 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_identity.py
--rw-r--r--   0 root         (0) root         (0)    18584 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_impl_upload_download.py
--rw-r--r--   0 root         (0) root         (0)    57290 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_import_export.py
--rw-r--r--   0 root         (0) root         (0)     5258 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_judge_cleaner.py
--rw-r--r--   0 root         (0) root         (0)    22277 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_judge_evaluator.py
--rw-r--r--   0 root         (0) root         (0)    11050 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_judge_injector.py
--rw-r--r--   0 root         (0) root         (0)    20429 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_judge_repairer.py
--rw-r--r--   0 root         (0) root         (0)    12180 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_lifetime.py
--rw-r--r--   0 root         (0) root         (0)     5855 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_message.py
--rw-r--r--   0 root         (0) root         (0)     6299 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_meta_did.py
--rw-r--r--   0 root         (0) root         (0)      957 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_module_import.py
--rw-r--r--   0 root         (0) root         (0)     2034 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_monitor.py
--rw-r--r--   0 root         (0) root         (0)    54332 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     2759 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_naming_convention.py
--rw-r--r--   0 root         (0) root         (0)    11582 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_oauthmanager.py
--rw-r--r--   0 root         (0) root         (0)   108359 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_oidc.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_permission.py
--rw-r--r--   0 root         (0) root         (0)     4123 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_pfns.py
--rw-r--r--   0 root         (0) root         (0)     1141 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_ping.py
--rw-r--r--   0 root         (0) root         (0)     7662 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_preparer.py
--rw-r--r--   0 root         (0) root         (0)     2741 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_qos.py
--rw-r--r--   0 root         (0) root         (0)     2023 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    27487 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_reaper.py
--rw-r--r--   0 root         (0) root         (0)     6440 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_redirect.py
--rw-r--r--   0 root         (0) root         (0)    62467 2024-05-21 07:56:54.000000 rucio_clients-34.4.0/tests/test_replica.py
--rw-r--r--   0 root         (0) root         (0)    42098 2024-05-21 07:16:09.000000 rucio_clients-34.4.0/tests/test_replica_recoverer.py
--rw-r--r--   0 root         (0) root         (0)    22796 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_replica_sorting.py
--rw-r--r--   0 root         (0) root         (0)    17257 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_request.py
--rw-r--r--   0 root         (0) root         (0)    13033 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_root_proxy.py
--rw-r--r--   0 root         (0) root         (0)    75080 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse.py
--rw-r--r--   0 root         (0) root         (0)    13184 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)     8940 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_lfn2path.py
--rw-r--r--   0 root         (0) root         (0)     4277 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_gfal2.py
--rw-r--r--   0 root         (0) root         (0)     3822 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_gfal2_impl.py
--rw-r--r--   0 root         (0) root         (0)     3267 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_posix.py
--rw-r--r--   0 root         (0) root         (0)     3690 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_rclone.py
--rw-r--r--   0 root         (0) root         (0)     4799 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_rsync.py
--rw-r--r--   0 root         (0) root         (0)     3979 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_srm.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_ssh.py
--rw-r--r--   0 root         (0) root         (0)     3015 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_webdav.py
--rw-r--r--   0 root         (0) root         (0)     3780 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_xrootd.py
--rw-r--r--   0 root         (0) root         (0)     7746 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_selector.py
--rw-r--r--   0 root         (0) root         (0)      867 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)    91949 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_rule.py
--rw-r--r--   0 root         (0) root         (0)     7486 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_scope.py
--rw-r--r--   0 root         (0) root         (0)    48389 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_subscription.py
--rw-r--r--   0 root         (0) root         (0)    55587 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_throttler.py
--rw-r--r--   0 root         (0) root         (0)     5011 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_tpc.py
--rw-r--r--   0 root         (0) root         (0)     3181 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_trace.py
--rw-r--r--   0 root         (0) root         (0)    25254 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_transfer.py
--rw-r--r--   0 root         (0) root         (0)     8924 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_transfer_plugins.py
--rw-r--r--   0 root         (0) root         (0)     8412 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_undertaker.py
--rw-r--r--   0 root         (0) root         (0)    15575 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_upload.py
--rw-r--r--   0 root         (0) root         (0)     7427 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.461628 rucio_clients-34.4.0/tools/
--rw-r--r--   0 root         (0) root         (0)     6163 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tools/merge_rucio_configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:35.518458 rucio_clients-34.4.1/
+-rwxr-xr-x   0 root         (0) root         (0)     4487 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio_clients-34.4.1/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio_clients-34.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      598 2024-05-24 12:25:32.000000 rucio_clients-34.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1533 2024-05-24 12:25:35.518458 rucio_clients-34.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-05-24 11:15:54.000000 rucio_clients-34.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:35.484457 rucio_clients-34.4.1/bin/
+-rwxr-xr-x   0 root         (0) root         (0)   127119 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/bin/rucio
+-rwxr-xr-x   0 root         (0) root         (0)   133582 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/bin/rucio-admin
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:35.485457 rucio_clients-34.4.1/etc/
+-rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio_clients-34.4.1/etc/rse-accounts.cfg.template
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio_clients-34.4.1/etc/rucio.cfg.atlas.client.template
+-rw-r--r--   0 root         (0) root         (0)     8534 2024-05-06 09:19:47.000000 rucio_clients-34.4.1/etc/rucio.cfg.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:35.481457 rucio_clients-34.4.1/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:35.486457 rucio_clients-34.4.1/lib/rucio/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      690 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/alembicrevision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:35.490457 rucio_clients-34.4.1/lib/rucio/client/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16352 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/accountclient.py
+-rw-r--r--   0 root         (0) root         (0)     5961 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/accountlimitclient.py
+-rw-r--r--   0 root         (0) root         (0)    48035 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/baseclient.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     4401 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/configclient.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/credentialclient.py
+-rw-r--r--   0 root         (0) root         (0)    28378 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/didclient.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/diracclient.py
+-rw-r--r--   0 root         (0) root         (0)    87520 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/downloadclient.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/exportclient.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/fileclient.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/importclient.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/lifetimeclient.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/lockclient.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/metaconventionsclient.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/pingclient.py
+-rw-r--r--   0 root         (0) root         (0)    19518 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/replicaclient.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/requestclient.py
+-rw-r--r--   0 root         (0) root         (0)    27121 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/rseclient.py
+-rw-r--r--   0 root         (0) root         (0)    12734 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/ruleclient.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/scopeclient.py
+-rw-r--r--   0 root         (0) root         (0)     7971 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/subscriptionclient.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/touchclient.py
+-rw-r--r--   0 root         (0) root         (0)    46920 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/client/uploadclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:35.493457 rucio_clients-34.4.1/lib/rucio/common/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/cache.py
+-rw-r--r--   0 root         (0) root         (0)    24636 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/config.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/constants.py
+-rw-r--r--   0 root         (0) root         (0)      726 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/constraints.py
+-rwxr-xr-x   0 root         (0) root         (0)     6545 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/didtype.py
+-rw-r--r--   0 root         (0) root         (0)    32345 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/exception.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/extra.py
+-rw-r--r--   0 root         (0) root         (0)    15046 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/logging.py
+-rw-r--r--   0 root         (0) root         (0)    45338 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/pcache.py
+-rw-r--r--   0 root         (0) root         (0)     6071 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:35.494457 rucio_clients-34.4.1/lib/rucio/common/schema/
+-rw-r--r--   0 root         (0) root         (0)     5384 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15589 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/schema/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    15406 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/schema/belleii.py
+-rw-r--r--   0 root         (0) root         (0)    14987 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/schema/domatpc.py
+-rw-r--r--   0 root         (0) root         (0)    15926 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/schema/escape.py
+-rw-r--r--   0 root         (0) root         (0)    16241 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/schema/generic.py
+-rw-r--r--   0 root         (0) root         (0)    15468 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/schema/generic_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)    15277 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/schema/icecube.py
+-rw-r--r--   0 root         (0) root         (0)     5414 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/stomp_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/stopwatch.py
+-rw-r--r--   0 root         (0) root         (0)     4935 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)     5716 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/common/types.py
+-rw-r--r--   0 root         (0) root         (0)    79163 2024-05-24 11:15:54.000000 rucio_clients-34.4.1/lib/rucio/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:35.495457 rucio_clients-34.4.1/lib/rucio/rse/
+-rw-r--r--   0 root         (0) root         (0)     3303 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:35.498457 rucio_clients-34.4.1/lib/rucio/rse/protocols/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7199 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/bittorrent.py
+-rw-r--r--   0 root         (0) root         (0)     4603 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/dummy.py
+-rw-r--r--   0 root         (0) root         (0)    29100 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/gfal.py
+-rw-r--r--   0 root         (0) root         (0)     9730 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/globus.py
+-rw-r--r--   0 root         (0) root         (0)     3411 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/gsiftp.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/http_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/mock.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/ngarc.py
+-rw-r--r--   0 root         (0) root         (0)    10414 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/posix.py
+-rw-r--r--   0 root         (0) root         (0)    23933 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/protocol.py
+-rw-r--r--   0 root         (0) root         (0)    15260 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/rclone.py
+-rw-r--r--   0 root         (0) root         (0)     5501 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/rfio.py
+-rw-r--r--   0 root         (0) root         (0)    14689 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/srm.py
+-rw-r--r--   0 root         (0) root         (0)    17473 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     8141 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/storm.py
+-rw-r--r--   0 root         (0) root         (0)    22448 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/webdav.py
+-rw-r--r--   0 root         (0) root         (0)    12571 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/protocols/xrootd.py
+-rw-r--r--   0 root         (0) root         (0)    37647 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/rse/rsemanager.py
+-rw-r--r--   0 root         (0) root         (0)      244 2024-05-24 11:15:54.000000 rucio_clients-34.4.1/lib/rucio/vcsversion.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/lib/rucio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:35.516458 rucio_clients-34.4.1/lib/rucio_clients.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5117 2024-05-24 12:25:35.000000 rucio_clients-34.4.1/lib/rucio_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    16384 2024-05-06 09:19:47.000000 rucio_clients-34.4.1/pylintrc
+-rw-r--r--   0 root         (0) root         (0)     5763 2024-05-24 12:25:23.000000 rucio_clients-34.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     5235 2024-05-24 11:15:54.000000 rucio_clients-34.4.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-24 12:25:35.520458 rucio_clients-34.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-05-24 12:25:32.000000 rucio_clients-34.4.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/setuputil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:35.516458 rucio_clients-34.4.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_abacus_account.py
+-rw-r--r--   0 root         (0) root         (0)    10677 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_abacus_collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_abacus_rse.py
+-rw-r--r--   0 root         (0) root         (0)    15923 2024-05-24 11:15:54.000000 rucio_clients-34.4.1/tests/test_account.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_account_limits.py
+-rw-r--r--   0 root         (0) root         (0)    20523 2024-05-24 11:15:54.000000 rucio_clients-34.4.1/tests/test_api_external_representation.py
+-rw-r--r--   0 root         (0) root         (0)    13352 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_archive.py
+-rw-r--r--   0 root         (0) root         (0)     4074 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_auditor.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_auditor_hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_auditor_srmdumps.py
+-rw-r--r--   0 root         (0) root         (0)    14964 2024-05-24 11:15:54.000000 rucio_clients-34.4.1/tests/test_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_automatix.py
+-rw-r--r--   0 root         (0) root         (0)    23265 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_bad_replica.py
+-rw-r--r--   0 root         (0) root         (0)    12425 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_bb8.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_belleii.py
+-rwxr-xr-x   0 root         (0) root         (0)   107450 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_bin_rucio.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_boolean.py
+-rw-r--r--   0 root         (0) root         (0)     8398 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_clients.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_common_types.py
+-rw-r--r--   0 root         (0) root         (0)     6942 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    96724 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_conveyor.py
+-rw-r--r--   0 root         (0) root         (0)    23870 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_conveyor_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_counter.py
+-rw-r--r--   0 root         (0) root         (0)     7728 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_credential.py
+-rw-r--r--   0 root         (0) root         (0)     7337 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_curl.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_daemons.py
+-rw-r--r--   0 root         (0) root         (0)    28183 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_dataset_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_db.py
+-rw-r--r--   0 root         (0) root         (0)    58823 2024-05-24 11:15:54.000000 rucio_clients-34.4.1/tests/test_did.py
+-rw-r--r--   0 root         (0) root         (0)    29517 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_did_meta_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     4185 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_didtype.py
+-rw-r--r--   0 root         (0) root         (0)    35315 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     7118 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_dumper.py
+-rw-r--r--   0 root         (0) root         (0)    16419 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_dumper_consistency.py
+-rw-r--r--   0 root         (0) root         (0)    10869 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_dumper_data_model.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_dumper_path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    38301 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    10106 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_hermes.py
+-rw-r--r--   0 root         (0) root         (0)     5821 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)    18584 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_impl_upload_download.py
+-rw-r--r--   0 root         (0) root         (0)    57290 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_import_export.py
+-rw-r--r--   0 root         (0) root         (0)     5258 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_judge_cleaner.py
+-rw-r--r--   0 root         (0) root         (0)    22277 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_judge_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_judge_injector.py
+-rw-r--r--   0 root         (0) root         (0)    20429 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_judge_repairer.py
+-rw-r--r--   0 root         (0) root         (0)    12180 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_lifetime.py
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_meta_did.py
+-rw-r--r--   0 root         (0) root         (0)      957 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_module_import.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    54332 2024-05-24 11:15:54.000000 rucio_clients-34.4.1/tests/test_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)    11582 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_oauthmanager.py
+-rw-r--r--   0 root         (0) root         (0)   108359 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-05-24 11:15:54.000000 rucio_clients-34.4.1/tests/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_pfns.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_ping.py
+-rw-r--r--   0 root         (0) root         (0)     7662 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_qos.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    27487 2024-05-24 11:15:54.000000 rucio_clients-34.4.1/tests/test_reaper.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_redirect.py
+-rw-r--r--   0 root         (0) root         (0)    62467 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_replica.py
+-rw-r--r--   0 root         (0) root         (0)    42098 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_replica_recoverer.py
+-rw-r--r--   0 root         (0) root         (0)    22796 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_replica_sorting.py
+-rw-r--r--   0 root         (0) root         (0)    17257 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_request.py
+-rw-r--r--   0 root         (0) root         (0)    13033 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_root_proxy.py
+-rw-r--r--   0 root         (0) root         (0)    75080 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_rse.py
+-rw-r--r--   0 root         (0) root         (0)    13184 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)     8940 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_rse_lfn2path.py
+-rw-r--r--   0 root         (0) root         (0)     4277 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_rse_protocol_gfal2.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_rse_protocol_gfal2_impl.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_rse_protocol_posix.py
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_rse_protocol_rclone.py
+-rw-r--r--   0 root         (0) root         (0)     4799 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_rse_protocol_rsync.py
+-rw-r--r--   0 root         (0) root         (0)     3979 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_rse_protocol_srm.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_rse_protocol_ssh.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_rse_protocol_webdav.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_rse_protocol_xrootd.py
+-rw-r--r--   0 root         (0) root         (0)     7746 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)      867 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)    91949 2024-05-24 11:15:54.000000 rucio_clients-34.4.1/tests/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)     7486 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_scope.py
+-rw-r--r--   0 root         (0) root         (0)    48389 2024-05-24 11:15:54.000000 rucio_clients-34.4.1/tests/test_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    55587 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_throttler.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_tpc.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)    25254 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     8924 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_transfer_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8412 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_undertaker.py
+-rw-r--r--   0 root         (0) root         (0)    16778 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:35.516458 rucio_clients-34.4.1/tools/
+-rw-r--r--   0 root         (0) root         (0)     6163 2024-05-23 08:12:33.000000 rucio_clients-34.4.1/tools/merge_rucio_configs.py
```

### Comparing `rucio_clients-34.4.0/AUTHORS.rst` & `rucio_clients-34.4.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/LICENSE` & `rucio_clients-34.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/MANIFEST.in` & `rucio_clients-34.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/PKG-INFO` & `rucio_clients-34.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rucio-clients
-Version: 34.4.0
+Version: 34.4.1
 Summary: Rucio Client Lite Package
 Home-page: https://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9, <4
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: requests<=2.31.0,>=2.25.1
+Requires-Dist: requests~=2.32.0
 Requires-Dist: urllib3~=1.26.18
 Requires-Dist: dogpile.cache~=1.2.2
 Requires-Dist: tabulate~=0.9.0
 Requires-Dist: jsonschema~=4.20.0
 Provides-Extra: ssh
 Requires-Dist: paramiko~=3.4.0; extra == "ssh"
 Provides-Extra: kerberos
```

### Comparing `rucio_clients-34.4.0/README.rst` & `rucio_clients-34.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/bin/rucio` & `rucio_clients-34.4.1/bin/rucio`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/bin/rucio-admin` & `rucio_clients-34.4.1/bin/rucio-admin`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/etc/rse-accounts.cfg.template` & `rucio_clients-34.4.1/etc/rse-accounts.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/etc/rucio.cfg.atlas.client.template` & `rucio_clients-34.4.1/etc/rucio.cfg.atlas.client.template`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/etc/rucio.cfg.template` & `rucio_clients-34.4.1/etc/rucio.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/__init__.py` & `rucio_clients-34.4.1/lib/rucio/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/alembicrevision.py` & `rucio_clients-34.4.1/lib/rucio/alembicrevision.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/__init__.py` & `rucio_clients-34.4.1/lib/rucio/client/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/accountclient.py` & `rucio_clients-34.4.1/lib/rucio/client/accountclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/accountlimitclient.py` & `rucio_clients-34.4.1/lib/rucio/client/accountlimitclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/baseclient.py` & `rucio_clients-34.4.1/lib/rucio/client/baseclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/client.py` & `rucio_clients-34.4.1/lib/rucio/client/client.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/configclient.py` & `rucio_clients-34.4.1/lib/rucio/client/configclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/credentialclient.py` & `rucio_clients-34.4.1/lib/rucio/client/credentialclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/didclient.py` & `rucio_clients-34.4.1/lib/rucio/client/didclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/diracclient.py` & `rucio_clients-34.4.1/lib/rucio/client/diracclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/downloadclient.py` & `rucio_clients-34.4.1/lib/rucio/client/downloadclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/exportclient.py` & `rucio_clients-34.4.1/lib/rucio/client/exportclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/fileclient.py` & `rucio_clients-34.4.1/lib/rucio/client/fileclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/importclient.py` & `rucio_clients-34.4.1/lib/rucio/client/importclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/lifetimeclient.py` & `rucio_clients-34.4.1/lib/rucio/client/lifetimeclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/lockclient.py` & `rucio_clients-34.4.1/lib/rucio/client/lockclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/metaconventionsclient.py` & `rucio_clients-34.4.1/lib/rucio/client/metaconventionsclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/pingclient.py` & `rucio_clients-34.4.1/lib/rucio/client/pingclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/replicaclient.py` & `rucio_clients-34.4.1/lib/rucio/client/replicaclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/requestclient.py` & `rucio_clients-34.4.1/lib/rucio/client/requestclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/rseclient.py` & `rucio_clients-34.4.1/lib/rucio/client/rseclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/ruleclient.py` & `rucio_clients-34.4.1/lib/rucio/client/ruleclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/scopeclient.py` & `rucio_clients-34.4.1/lib/rucio/client/scopeclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/subscriptionclient.py` & `rucio_clients-34.4.1/lib/rucio/client/subscriptionclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/touchclient.py` & `rucio_clients-34.4.1/lib/rucio/client/touchclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/client/uploadclient.py` & `rucio_clients-34.4.1/lib/rucio/client/uploadclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,42 +282,48 @@
                     file['upload_result'] = {0: True, 1: None, 'success': True, 'pfn': pfn}  # needs to be removed
                 except (ServiceUnavailable, ResourceTemporaryUnavailable, RSEOperationNotSupported, RucioException) as error:
                     logger(logging.WARNING, 'Upload attempt failed')
                     logger(logging.INFO, 'Exception: %s' % str(error), exc_info=True)
                     state_reason = str(error)
 
             if success:
-                num_succeeded += 1
                 trace['transferEnd'] = time.time()
                 trace['clientState'] = 'DONE'
                 file['state'] = 'A'
                 logger(logging.INFO, 'Successfully uploaded file %s' % basename)
                 self._send_trace(trace)
 
                 if summary_file_path:
                     summary.append(copy.deepcopy(file))
 
+                registration_succeeded = True
                 if not no_register:
                     if register_after_upload:
                         self._register_file(file, registered_dataset_dids, ignore_availability=ignore_availability, activity=activity)
                     else:
                         replica_for_api = self._convert_file_for_api(file)
                         try:
                             self.client.update_replicas_states(rse, files=[replica_for_api])
                         except Exception as error:
+                            registration_succeeded = False
                             logger(logging.ERROR, 'Failed to update replica state for file {}'.format(basename))
                             logger(logging.DEBUG, 'Details: {}'.format(str(error)))
 
                 # add file to dataset if needed
                 if dataset_did_str and not no_register:
                     try:
                         self.client.attach_dids(file['dataset_scope'], file['dataset_name'], [file_did])
                     except Exception as error:
-                        logger(logging.WARNING, 'Failed to attach file to the dataset')
+                        registration_succeeded = False
+                        logger(logging.ERROR, 'Failed to attach file to the dataset')
                         logger(logging.DEBUG, 'Attaching to dataset {}'.format(str(error)))
+
+                # only report success if the registration operations succeeded as well
+                if registration_succeeded:
+                    num_succeeded += 1
             else:
                 trace['clientState'] = 'FAILED'
                 trace['stateReason'] = state_reason
                 self._send_trace(trace)
                 logger(logging.ERROR, 'Failed to upload file %s' % basename)
 
         if summary_file_path:
```

### Comparing `rucio_clients-34.4.0/lib/rucio/common/__init__.py` & `rucio_clients-34.4.1/lib/rucio/common/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/cache.py` & `rucio_clients-34.4.1/lib/rucio/common/cache.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/config.py` & `rucio_clients-34.4.1/lib/rucio/common/config.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/constants.py` & `rucio_clients-34.4.1/lib/rucio/common/constants.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/constraints.py` & `rucio_clients-34.4.1/lib/rucio/common/constraints.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/didtype.py` & `rucio_clients-34.4.1/lib/rucio/common/didtype.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/exception.py` & `rucio_clients-34.4.1/lib/rucio/common/exception.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/extra.py` & `rucio_clients-34.4.1/lib/rucio/common/extra.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/logging.py` & `rucio_clients-34.4.1/lib/rucio/common/logging.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/pcache.py` & `rucio_clients-34.4.1/lib/rucio/common/pcache.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/plugins.py` & `rucio_clients-34.4.1/lib/rucio/common/plugins.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/policy.py` & `rucio_clients-34.4.1/lib/rucio/common/policy.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/schema/__init__.py` & `rucio_clients-34.4.1/lib/rucio/common/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/schema/atlas.py` & `rucio_clients-34.4.1/lib/rucio/common/schema/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/schema/belleii.py` & `rucio_clients-34.4.1/lib/rucio/common/schema/belleii.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/schema/domatpc.py` & `rucio_clients-34.4.1/lib/rucio/common/schema/domatpc.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/schema/escape.py` & `rucio_clients-34.4.1/lib/rucio/common/schema/escape.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/schema/generic.py` & `rucio_clients-34.4.1/lib/rucio/common/schema/generic.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/schema/generic_multi_vo.py` & `rucio_clients-34.4.1/lib/rucio/common/schema/generic_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/schema/icecube.py` & `rucio_clients-34.4.1/lib/rucio/common/schema/icecube.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/stomp_utils.py` & `rucio_clients-34.4.1/lib/rucio/common/stomp_utils.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/stopwatch.py` & `rucio_clients-34.4.1/lib/rucio/common/stopwatch.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/test_rucio_server.py` & `rucio_clients-34.4.1/lib/rucio/common/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/types.py` & `rucio_clients-34.4.1/lib/rucio/common/types.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/common/utils.py` & `rucio_clients-34.4.1/lib/rucio/common/utils.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/__init__.py` & `rucio_clients-34.4.1/lib/rucio/rse/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/__init__.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/bittorrent.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/bittorrent.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/cache.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/cache.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/dummy.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/dummy.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/gfal.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/gfal.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/globus.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/globus.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/gsiftp.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/gsiftp.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/http_cache.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/http_cache.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/mock.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/mock.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/ngarc.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/ngarc.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/posix.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/posix.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/protocol.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 This module defines the base class for implementing a transfer protocol,
 along with some of the default methods for LFN2PFN translations.
 """
-
 import hashlib
 import logging
+from collections.abc import Callable, Mapping
 from configparser import NoOptionError, NoSectionError
 from typing import TypeVar
 from urllib.parse import urlparse
 
 from rucio.common import config, exception
 from rucio.common.constants import RseAttr
 from rucio.common.plugins import PolicyPackageAlgorithms
@@ -33,14 +33,69 @@
 
 if getattr(rsemanager, 'SERVER_MODE', None):
     from rucio.common.types import InternalScope
     from rucio.core import replica
     from rucio.core.rse import get_rse_vo
 
 
+class RSEDeterministicScopeTranslation(PolicyPackageAlgorithms):
+    """
+        Translates a pfn dictionary into a scope and name
+    """
+    def __init__(self, vo: str = 'def'):
+        super().__init__()
+        self.register("def", RSEDeterministicScopeTranslation._default)
+        self.register("atlas", RSEDeterministicScopeTranslation._atlas)
+        policy_module = vo
+        # Uses the same policy as the DeterministicTranslation
+        if super()._supports(self.__class__.__name__, policy_module):
+            self.parser = self._get_one_algorithm(self.__class__.__name__, policy_module)
+        else:
+            self.parser = self._get_one_algorithm(self.__class__.__name__, "def")
+
+    @classmethod
+    def register(cls, name: str, func: Callable) -> None:
+        super()._register(cls.__name__, {name: func})
+
+    @staticmethod
+    def _default(parsed_pfn: Mapping[str, str]) -> tuple[str, str]:
+        """ Translate pfn to name/scope pair
+
+        :param parsed_pfn: dictionary representing pfn containing:
+            - path: str,
+            - name: str
+        :return: tuple containing name, scope
+        """
+        path = parsed_pfn['path']
+        scope = path.lstrip('/').split('/')[0]
+        name = parsed_pfn['name']
+        return name, scope
+
+    @staticmethod
+    def _atlas(parsed_pfn: Mapping[str, str]) -> tuple[str, str]:
+        """ Translate pfn to name/scope pair
+
+        :param parsed_pfn: dictionary representing pfn containing:
+            - path: str,
+            - name: str
+        :return: tuple containing name, scope
+        """
+        path = parsed_pfn['path']
+        if path.startswith('/user') or path.startswith('/group'):
+            scope = '%s.%s' % (path.split('/')[1], path.split('/')[2])
+            name = parsed_pfn['name']
+        else:
+            name, scope = RSEDeterministicScopeTranslation._default(parsed_pfn)
+
+        return name, scope
+
+
+RSEDeterministicScopeTranslation()
+
+
 RSEDeterministicTranslationT = TypeVar('RSEDeterministicTranslationT', bound='RSEDeterministicTranslation')
 
 
 class RSEDeterministicTranslation(PolicyPackageAlgorithms):
     """
     Execute the logic for translating a LFN to a path.
     """
```

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/rclone.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/rclone.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/rfio.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/rfio.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/srm.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/srm.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/ssh.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/ssh.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/storm.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/storm.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/webdav.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/webdav.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/protocols/xrootd.py` & `rucio_clients-34.4.1/lib/rucio/rse/protocols/xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio/rse/rsemanager.py` & `rucio_clients-34.4.1/lib/rucio/rse/rsemanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,37 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 import logging
 import random
+from collections.abc import Callable
 from time import sleep
 from urllib.parse import urlparse
 
 from rucio.common import constants, exception, types, utils
 from rucio.common.config import config_get_int
 from rucio.common.constraints import STRING_TYPES
 from rucio.common.logging import formatted_logger
 from rucio.common.utils import GLOBALLY_SUPPORTED_CHECKSUMS, make_valid_did
 
 
+def get_scope_protocol(vo: str = 'def') -> Callable:
+    """
+        Returns the callable protocol to translate the pfn to a name/scope pair
+
+    :returns:
+        Callable: Scope Parser function
+    """
+    from rucio.rse.protocols.protocol import RSEDeterministicScopeTranslation
+    translation = RSEDeterministicScopeTranslation(vo=vo)
+    return translation.parser
+
+
 def get_rse_info(rse=None, vo='def', rse_id=None, session=None) -> types.RSESettingsDict:
     """
         Returns all protocol related RSE attributes.
         Call with either rse and vo, or (in server mode) rse_id
 
         :param rse: Name of the requested RSE
         :param vo: The VO for the RSE.
```

### Comparing `rucio_clients-34.4.0/lib/rucio/version.py` & `rucio_clients-34.4.1/lib/rucio/version.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/lib/rucio_clients.egg-info/SOURCES.txt` & `rucio_clients-34.4.1/lib/rucio_clients.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/pylintrc` & `rucio_clients-34.4.1/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/pyproject.toml` & `rucio_clients-34.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/requirements.txt` & `rucio_clients-34.4.1/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # All dependencies needed to run rucio client (and server/daemons) should be defined here
-requests>=2.25.1,<=2.31.0                                   # Python HTTP for Humans.
+requests~=2.32.0                                            # Python HTTP for Humans.
 urllib3~=1.26.18                                            # HTTP library with thread-safe connection pooling, file post, etc.
 dogpile.cache~=1.2.2                                        # Caching API plugins (1.1.2 is the first version to support pymemcache)
 tabulate~=0.9.0                                             # Pretty-print tabular data
 jsonschema~=4.20.0                                          # For JSON schema validation (Policy modules)
 
 # All dependencies needed in extras for rucio client (and server/daemons) should be defined here
 paramiko~=3.4.0                                             # ssh_extras; SSH2 protocol library (also needed in the server)
```

### Comparing `rucio_clients-34.4.0/setup.py` & `rucio_clients-34.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/setuputil.py` & `rucio_clients-34.4.1/setuputil.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_abacus_account.py` & `rucio_clients-34.4.1/tests/test_abacus_account.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_abacus_collection_replica.py` & `rucio_clients-34.4.1/tests/test_abacus_collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_abacus_rse.py` & `rucio_clients-34.4.1/tests/test_abacus_rse.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_account.py` & `rucio_clients-34.4.1/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_account_limits.py` & `rucio_clients-34.4.1/tests/test_account_limits.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_api_external_representation.py` & `rucio_clients-34.4.1/tests/test_api_external_representation.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_archive.py` & `rucio_clients-34.4.1/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_auditor.py` & `rucio_clients-34.4.1/tests/test_auditor.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_auditor_hdfs.py` & `rucio_clients-34.4.1/tests/test_auditor_hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_auditor_srmdumps.py` & `rucio_clients-34.4.1/tests/test_auditor_srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_authentication.py` & `rucio_clients-34.4.1/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_automatix.py` & `rucio_clients-34.4.1/tests/test_automatix.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_bad_replica.py` & `rucio_clients-34.4.1/tests/test_bad_replica.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_bb8.py` & `rucio_clients-34.4.1/tests/test_bb8.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_belleii.py` & `rucio_clients-34.4.1/tests/test_belleii.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_bin_rucio.py` & `rucio_clients-34.4.1/tests/test_bin_rucio.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_boolean.py` & `rucio_clients-34.4.1/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_clients.py` & `rucio_clients-34.4.1/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_common_types.py` & `rucio_clients-34.4.1/tests/test_common_types.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_config.py` & `rucio_clients-34.4.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_conveyor.py` & `rucio_clients-34.4.1/tests/test_conveyor.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_conveyor_submitter.py` & `rucio_clients-34.4.1/tests/test_conveyor_submitter.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_counter.py` & `rucio_clients-34.4.1/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_credential.py` & `rucio_clients-34.4.1/tests/test_credential.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_curl.py` & `rucio_clients-34.4.1/tests/test_curl.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_daemons.py` & `rucio_clients-34.4.1/tests/test_daemons.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_dataset_replicas.py` & `rucio_clients-34.4.1/tests/test_dataset_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_db.py` & `rucio_clients-34.4.1/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_did.py` & `rucio_clients-34.4.1/tests/test_did.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_did_meta_plugins.py` & `rucio_clients-34.4.1/tests/test_did_meta_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_didtype.py` & `rucio_clients-34.4.1/tests/test_didtype.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_download.py` & `rucio_clients-34.4.1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_dumper.py` & `rucio_clients-34.4.1/tests/test_dumper.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_dumper_consistency.py` & `rucio_clients-34.4.1/tests/test_dumper_consistency.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_dumper_data_model.py` & `rucio_clients-34.4.1/tests/test_dumper_data_model.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_dumper_path_parsing.py` & `rucio_clients-34.4.1/tests/test_dumper_path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_filter_engine.py` & `rucio_clients-34.4.1/tests/test_filter_engine.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_heartbeat.py` & `rucio_clients-34.4.1/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_hermes.py` & `rucio_clients-34.4.1/tests/test_hermes.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_identity.py` & `rucio_clients-34.4.1/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_impl_upload_download.py` & `rucio_clients-34.4.1/tests/test_impl_upload_download.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_import_export.py` & `rucio_clients-34.4.1/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_judge_cleaner.py` & `rucio_clients-34.4.1/tests/test_judge_cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_judge_evaluator.py` & `rucio_clients-34.4.1/tests/test_judge_evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_judge_injector.py` & `rucio_clients-34.4.1/tests/test_judge_injector.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_judge_repairer.py` & `rucio_clients-34.4.1/tests/test_judge_repairer.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_lifetime.py` & `rucio_clients-34.4.1/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_message.py` & `rucio_clients-34.4.1/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_meta_conventions.py` & `rucio_clients-34.4.1/tests/test_meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_meta_did.py` & `rucio_clients-34.4.1/tests/test_meta_did.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_module_import.py` & `rucio_clients-34.4.1/tests/test_module_import.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_monitor.py` & `rucio_clients-34.4.1/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_multi_vo.py` & `rucio_clients-34.4.1/tests/test_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_naming_convention.py` & `rucio_clients-34.4.1/tests/test_naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_oauthmanager.py` & `rucio_clients-34.4.1/tests/test_oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_oidc.py` & `rucio_clients-34.4.1/tests/test_oidc.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_permission.py` & `rucio_clients-34.4.1/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_pfns.py` & `rucio_clients-34.4.1/tests/test_pfns.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_ping.py` & `rucio_clients-34.4.1/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_preparer.py` & `rucio_clients-34.4.1/tests/test_preparer.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_qos.py` & `rucio_clients-34.4.1/tests/test_qos.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_quarantined_replica.py` & `rucio_clients-34.4.1/tests/test_quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_reaper.py` & `rucio_clients-34.4.1/tests/test_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_redirect.py` & `rucio_clients-34.4.1/tests/test_redirect.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_replica.py` & `rucio_clients-34.4.1/tests/test_replica.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_replica_recoverer.py` & `rucio_clients-34.4.1/tests/test_replica_recoverer.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_replica_sorting.py` & `rucio_clients-34.4.1/tests/test_replica_sorting.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_request.py` & `rucio_clients-34.4.1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_root_proxy.py` & `rucio_clients-34.4.1/tests/test_root_proxy.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_rse.py` & `rucio_clients-34.4.1/tests/test_rse.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_rse_expression_parser.py` & `rucio_clients-34.4.1/tests/test_rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_rse_lfn2path.py` & `rucio_clients-34.4.1/tests/test_rse_lfn2path.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_rse_protocol_gfal2.py` & `rucio_clients-34.4.1/tests/test_rse_protocol_gfal2.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_rse_protocol_gfal2_impl.py` & `rucio_clients-34.4.1/tests/test_rse_protocol_gfal2_impl.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_rse_protocol_posix.py` & `rucio_clients-34.4.1/tests/test_rse_protocol_posix.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_rse_protocol_rclone.py` & `rucio_clients-34.4.1/tests/test_rse_protocol_rclone.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_rse_protocol_rsync.py` & `rucio_clients-34.4.1/tests/test_rse_protocol_rsync.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_rse_protocol_srm.py` & `rucio_clients-34.4.1/tests/test_rse_protocol_srm.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_rse_protocol_ssh.py` & `rucio_clients-34.4.1/tests/test_rse_protocol_ssh.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_rse_protocol_webdav.py` & `rucio_clients-34.4.1/tests/test_rse_protocol_webdav.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_rse_protocol_xrootd.py` & `rucio_clients-34.4.1/tests/test_rse_protocol_xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_rse_selector.py` & `rucio_clients-34.4.1/tests/test_rse_selector.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_rucio_server.py` & `rucio_clients-34.4.1/tests/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_rule.py` & `rucio_clients-34.4.1/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_scope.py` & `rucio_clients-34.4.1/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_subscription.py` & `rucio_clients-34.4.1/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_throttler.py` & `rucio_clients-34.4.1/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_tpc.py` & `rucio_clients-34.4.1/tests/test_tpc.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_trace.py` & `rucio_clients-34.4.1/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_transfer.py` & `rucio_clients-34.4.1/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_transfer_plugins.py` & `rucio_clients-34.4.1/tests/test_transfer_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_undertaker.py` & `rucio_clients-34.4.1/tests/test_undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tests/test_upload.py` & `rucio_clients-34.4.1/tests/test_upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 import os
 import shutil
 from tempfile import TemporaryDirectory
 from unittest.mock import patch
 
 import pytest
 
+from rucio.client.client import Client
 from rucio.client.uploadclient import UploadClient
 from rucio.common.config import config_add_section, config_set
 from rucio.common.constants import RseAttr
-from rucio.common.exception import InputValidationError, NoFilesUploaded, NotAllFilesUploaded
+from rucio.common.exception import InputValidationError, NoFilesUploaded, NotAllFilesUploaded, ResourceTemporaryUnavailable
 from rucio.common.utils import adler32, generate_uuid
 from rucio.core.rse import add_protocol, add_rse_attribute
 
 
 @pytest.fixture
 def upload_client():
     logger = logging.getLogger('upload_client')
@@ -394,7 +395,37 @@
             'rse': rse,
             'did_scope': scope,
         }
     ]
 
     status = upload_client.upload(item, ignore_availability=True)
     assert status == 0
+
+
+@pytest.fixture
+def upload_client_registration_fail():
+    logger = logging.getLogger('upload_client')
+    logger.addHandler(logging.StreamHandler())
+    logger.setLevel(logging.DEBUG)
+    # modify the client object used by upload_client so that replica registration fails
+    class RegistrationFailureClient(Client):
+        def __init__(self, **args):
+            super(RegistrationFailureClient, self).__init__(**args)
+        def update_replicas_states(self, rse, files):
+            # simulate server timing out
+            raise ResourceTemporaryUnavailable
+    return UploadClient(logger=logger, _client=RegistrationFailureClient())
+
+
+def test_upload_registration_fail(rse, scope, upload_client_registration_fail, file_factory):
+    local_file = file_factory.file_generator()
+    fn = os.path.basename(local_file)
+
+    # upload a file and check that exception is raised
+    with pytest.raises(NoFilesUploaded):
+        upload_client_registration_fail.upload([{
+            'path': local_file,
+            'rse': rse,
+            'did_scope': scope,
+            'did_name': fn,
+            'guid': generate_uuid()
+        }])
```

### Comparing `rucio_clients-34.4.0/tests/test_utils.py` & `rucio_clients-34.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.4.0/tools/merge_rucio_configs.py` & `rucio_clients-34.4.1/tools/merge_rucio_configs.py`

 * *Files identical despite different names*

