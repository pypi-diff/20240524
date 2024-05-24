# Comparing `tmp/rucio-34.4.0.tar.gz` & `tmp/rucio-34.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-34.4.0.tar", last modified: Tue May 21 14:54:21 2024, max compression
+gzip compressed data, was "rucio-34.4.1.tar", last modified: Fri May 24 12:25:31 2024, max compression
```

## Comparing `rucio-34.4.0.tar` & `rucio-34.4.1.tar`

### file list

```diff
@@ -1,646 +1,646 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.782573 rucio-34.4.0/
--rwxr-xr-x   0 root         (0) root         (0)     4487 2024-05-16 07:28:57.000000 rucio-34.4.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio-34.4.0/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio-34.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      934 2024-05-21 14:54:17.000000 rucio-34.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2799 2024-05-21 14:54:21.781573 rucio-34.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1982 2024-05-21 09:35:26.000000 rucio-34.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.675572 rucio-34.4.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)   127119 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio
--rwxr-xr-x   0 root         (0) root         (0)     2820 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-abacus-account
--rwxr-xr-x   0 root         (0) root         (0)     1823 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-abacus-collection-replica
--rwxr-xr-x   0 root         (0) root         (0)     2567 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-abacus-rse
--rwxr-xr-x   0 root         (0) root         (0)   133582 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-admin
--rwxr-xr-x   0 root         (0) root         (0)     3185 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-atropos
--rwxr-xr-x   0 root         (0) root         (0)     5850 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-auditor
--rwxr-xr-x   0 root         (0) root         (0)     2010 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-automatix
--rwxr-xr-x   0 root         (0) root         (0)     3103 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-bb8
--rwxr-xr-x   0 root         (0) root         (0)     6100 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-c3po
--rwxr-xr-x   0 root         (0) root         (0)     5060 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-cache-client
--rwxr-xr-x   0 root         (0) root         (0)     1362 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-cache-consumer
--rwxr-xr-x   0 root         (0) root         (0)     2347 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-conveyor-finisher
--rwxr-xr-x   0 root         (0) root         (0)     2839 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-conveyor-poller
--rwxr-xr-x   0 root         (0) root         (0)     1759 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-conveyor-preparer
--rwxr-xr-x   0 root         (0) root         (0)     1682 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-conveyor-receiver
--rwxr-xr-x   0 root         (0) root         (0)     3385 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-conveyor-stager
--rwxr-xr-x   0 root         (0) root         (0)     6752 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-conveyor-submitter
--rwxr-xr-x   0 root         (0) root         (0)     3859 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-conveyor-throttler
--rwxr-xr-x   0 root         (0) root         (0)     2546 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-dark-reaper
--rwxr-xr-x   0 root         (0) root         (0)     6463 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-dumper
--rwxr-xr-x   0 root         (0) root         (0)     1414 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-follower
--rwxr-xr-x   0 root         (0) root         (0)     1987 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-hermes
--rwxr-xr-x   0 root         (0) root         (0)     4649 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-judge-cleaner
--rwxr-xr-x   0 root         (0) root         (0)     7472 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-judge-evaluator
--rwxr-xr-x   0 root         (0) root         (0)     1671 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-judge-injector
--rwxr-xr-x   0 root         (0) root         (0)     1675 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-judge-repairer
--rwxr-xr-x   0 root         (0) root         (0)     1782 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-kronos
--rwxr-xr-x   0 root         (0) root         (0)     2260 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-minos
--rwxr-xr-x   0 root         (0) root         (0)     1997 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-minos-temporary-expiration
--rwxr-xr-x   0 root         (0) root         (0)     5626 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-necromancer
--rwxr-xr-x   0 root         (0) root         (0)     2790 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-oauth-manager
--rwxr-xr-x   0 root         (0) root         (0)     4070 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-reaper
--rwxr-xr-x   0 root         (0) root         (0)    18988 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-replica-recoverer
--rwxr-xr-x   0 root         (0) root         (0)     2351 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-rse-decommissioner
--rwxr-xr-x   0 root         (0) root         (0)     3920 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-storage-consistency-actions
--rwxr-xr-x   0 root         (0) root         (0)     3364 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-transmogrifier
--rwxr-xr-x   0 root         (0) root         (0)     2720 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-undertaker
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.677572 rucio-34.4.0/etc/
--rw-r--r--   0 root         (0) root         (0)     1764 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/alembic.ini.template
--rw-r--r--   0 root         (0) root         (0)     1922 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/alembic_offline.ini.template
--rw-r--r--   0 root         (0) root         (0)       96 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/globus-config.yml.template
--rw-r--r--   0 root         (0) root         (0)      806 2024-05-16 07:28:57.000000 rucio-34.4.0/etc/ldap.cfg.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.678572 rucio-34.4.0/etc/mail_templates/
--rw-r--r--   0 root         (0) root         (0)     1210 2024-05-06 09:19:47.000000 rucio-34.4.0/etc/mail_templates/rule_approval_request.tmpl
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/mail_templates/rule_approved_admin.tmpl
--rw-r--r--   0 root         (0) root         (0)      499 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/mail_templates/rule_approved_user.tmpl
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/mail_templates/rule_denied_admin.tmpl
--rw-r--r--   0 root         (0) root         (0)      493 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/mail_templates/rule_denied_user.tmpl
--rw-r--r--   0 root         (0) root         (0)      546 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/mail_templates/rule_ok_notification.tmpl
--rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/rse-accounts.cfg.template
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/rucio.cfg.atlas.client.template
--rw-r--r--   0 root         (0) root         (0)     8534 2024-05-06 09:19:47.000000 rucio-34.4.0/etc/rucio.cfg.template
--rw-r--r--   0 root         (0) root         (0)     7477 2024-05-06 09:19:47.000000 rucio-34.4.0/etc/rucio_multi_vo.cfg.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.662572 rucio-34.4.0/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.678572 rucio-34.4.0/lib/rucio/
--rw-r--r--   0 root         (0) root         (0)      660 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      690 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/alembicrevision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.683572 rucio-34.4.0/lib/rucio/api/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9396 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/account.py
--rw-r--r--   0 root         (0) root         (0)    11394 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/account_limit.py
--rw-r--r--   0 root         (0) root         (0)    12890 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/authentication.py
--rw-r--r--   0 root         (0) root         (0)     9085 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/config.py
--rw-r--r--   0 root         (0) root         (0)     2908 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/credential.py
--rw-r--r--   0 root         (0) root         (0)    29418 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/did.py
--rw-r--r--   0 root         (0) root         (0)     3206 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/dirac.py
--rw-r--r--   0 root         (0) root         (0)     2148 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/exporter.py
--rw-r--r--   0 root         (0) root         (0)     2885 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/heartbeat.py
--rw-r--r--   0 root         (0) root         (0)     6830 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/identity.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/importer.py
--rw-r--r--   0 root         (0) root         (0)     3685 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/lifetime_exception.py
--rw-r--r--   0 root         (0) root         (0)     4628 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/lock.py
--rw-r--r--   0 root         (0) root         (0)     3615 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     2727 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/permission.py
--rw-r--r--   0 root         (0) root         (0)     2495 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    22565 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/replica.py
--rw-r--r--   0 root         (0) root         (0)    10550 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/request.py
--rw-r--r--   0 root         (0) root         (0)    23637 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/rse.py
--rw-r--r--   0 root         (0) root         (0)    16037 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/rule.py
--rw-r--r--   0 root         (0) root         (0)     3055 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/scope.py
--rw-r--r--   0 root         (0) root         (0)    10537 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/subscription.py
--rw-r--r--   0 root         (0) root         (0)     4817 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/vo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.688572 rucio-34.4.0/lib/rucio/client/
--rw-r--r--   0 root         (0) root         (0)      660 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16352 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/accountclient.py
--rw-r--r--   0 root         (0) root         (0)     5961 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/accountlimitclient.py
--rw-r--r--   0 root         (0) root         (0)    48035 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/client/baseclient.py
--rw-r--r--   0 root         (0) root         (0)     3079 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/client.py
--rw-r--r--   0 root         (0) root         (0)     4401 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/configclient.py
--rw-r--r--   0 root         (0) root         (0)     1989 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/credentialclient.py
--rw-r--r--   0 root         (0) root         (0)    28378 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/didclient.py
--rw-r--r--   0 root         (0) root         (0)     2114 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/diracclient.py
--rw-r--r--   0 root         (0) root         (0)    87520 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/downloadclient.py
--rw-r--r--   0 root         (0) root         (0)     1575 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/exportclient.py
--rw-r--r--   0 root         (0) root         (0)     1610 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/fileclient.py
--rw-r--r--   0 root         (0) root         (0)     1469 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/importclient.py
--rw-r--r--   0 root         (0) root         (0)     2822 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/lifetimeclient.py
--rw-r--r--   0 root         (0) root         (0)     3914 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/lockclient.py
--rw-r--r--   0 root         (0) root         (0)     5195 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/metaconventionsclient.py
--rw-r--r--   0 root         (0) root         (0)     1390 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/pingclient.py
--rw-r--r--   0 root         (0) root         (0)    19518 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/replicaclient.py
--rw-r--r--   0 root         (0) root         (0)     4197 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/requestclient.py
--rw-r--r--   0 root         (0) root         (0)    27121 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/rseclient.py
--rw-r--r--   0 root         (0) root         (0)    12734 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/ruleclient.py
--rw-r--r--   0 root         (0) root         (0)     3147 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/scopeclient.py
--rw-r--r--   0 root         (0) root         (0)     7971 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/subscriptionclient.py
--rw-r--r--   0 root         (0) root         (0)     2642 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/touchclient.py
--rw-r--r--   0 root         (0) root         (0)    46627 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/uploadclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.691572 rucio-34.4.0/lib/rucio/common/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2301 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/cache.py
--rw-r--r--   0 root         (0) root         (0)    24636 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/config.py
--rw-r--r--   0 root         (0) root         (0)     5507 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/constants.py
--rw-r--r--   0 root         (0) root         (0)      726 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/constraints.py
--rwxr-xr-x   0 root         (0) root         (0)     6545 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/didtype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.692572 rucio-34.4.0/lib/rucio/common/dumper/
--rw-r--r--   0 root         (0) root         (0)    10796 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/dumper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15985 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/dumper/consistency.py
--rw-r--r--   0 root         (0) root         (0)     9693 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/dumper/data_models.py
--rw-r--r--   0 root         (0) root         (0)     1923 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/dumper/path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    32345 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/exception.py
--rw-r--r--   0 root         (0) root         (0)     1398 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/extra.py
--rw-r--r--   0 root         (0) root         (0)    15046 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/logging.py
--rw-r--r--   0 root         (0) root         (0)    45338 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/common/pcache.py
--rw-r--r--   0 root         (0) root         (0)     6071 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/plugins.py
--rw-r--r--   0 root         (0) root         (0)     3085 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.694572 rucio-34.4.0/lib/rucio/common/schema/
--rw-r--r--   0 root         (0) root         (0)     5384 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15589 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/schema/atlas.py
--rw-r--r--   0 root         (0) root         (0)    15406 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/schema/belleii.py
--rw-r--r--   0 root         (0) root         (0)    14987 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/schema/domatpc.py
--rw-r--r--   0 root         (0) root         (0)    15926 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/schema/escape.py
--rw-r--r--   0 root         (0) root         (0)    16241 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/schema/generic.py
--rw-r--r--   0 root         (0) root         (0)    15468 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/schema/generic_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)    15277 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/schema/icecube.py
--rw-r--r--   0 root         (0) root         (0)     5414 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/stomp_utils.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/stopwatch.py
--rw-r--r--   0 root         (0) root         (0)     4935 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)     5716 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/types.py
--rw-r--r--   0 root         (0) root         (0)    79163 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.702572 rucio-34.4.0/lib/rucio/core/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14952 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/account.py
--rw-r--r--   0 root         (0) root         (0)     6289 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/account_counter.py
--rw-r--r--   0 root         (0) root         (0)    14274 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/account_limit.py
--rw-r--r--   0 root         (0) root         (0)    21045 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/authentication.py
--rw-r--r--   0 root         (0) root         (0)    13462 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/config.py
--rw-r--r--   0 root         (0) root         (0)     8211 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/credential.py
--rw-r--r--   0 root         (0) root         (0)   129547 2024-05-21 09:34:41.000000 rucio-34.4.0/lib/rucio/core/did.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.704573 rucio-34.4.0/lib/rucio/core/did_meta_plugins/
--rw-r--r--   0 root         (0) root         (0)    11733 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/did_meta_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17445 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/did_meta_plugins/did_column_meta.py
--rw-r--r--   0 root         (0) root         (0)     4932 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py
--rw-r--r--   0 root         (0) root         (0)    30038 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/did_meta_plugins/filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     9215 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/did_meta_plugins/json_meta.py
--rw-r--r--   0 root         (0) root         (0)     7431 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/did_meta_plugins/mongo_meta.py
--rw-r--r--   0 root         (0) root         (0)    13727 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/did_meta_plugins/postgres_meta.py
--rw-r--r--   0 root         (0) root         (0)     9402 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/dirac.py
--rw-r--r--   0 root         (0) root         (0)     5735 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/distance.py
--rw-r--r--   0 root         (0) root         (0)     1875 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/exporter.py
--rw-r--r--   0 root         (0) root         (0)    10986 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    12099 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/identity.py
--rw-r--r--   0 root         (0) root         (0)    14169 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/importer.py
--rw-r--r--   0 root         (0) root         (0)    15254 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/lifetime_exception.py
--rw-r--r--   0 root         (0) root         (0)    22857 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/lock.py
--rw-r--r--   0 root         (0) root         (0)     9693 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/message.py
--rw-r--r--   0 root         (0) root         (0)     8691 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)    15984 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/monitor.py
--rw-r--r--   0 root         (0) root         (0)     6054 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/naming_convention.py
--rw-r--r--   0 root         (0) root         (0)     4890 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/nongrid_trace.py
--rw-r--r--   0 root         (0) root         (0)    69833 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/core/oidc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.705572 rucio-34.4.0/lib/rucio/core/permission/
--rw-r--r--   0 root         (0) root         (0)     4070 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/permission/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55734 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/permission/atlas.py
--rw-r--r--   0 root         (0) root         (0)    46969 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/permission/belleii.py
--rw-r--r--   0 root         (0) root         (0)    43171 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/permission/escape.py
--rw-r--r--   0 root         (0) root         (0)    48439 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/permission/generic.py
--rw-r--r--   0 root         (0) root         (0)    45926 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/permission/generic_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     8030 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)   178001 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/replica.py
--rw-r--r--   0 root         (0) root         (0)    15434 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/core/replica_sorter.py
--rw-r--r--   0 root         (0) root         (0)   116306 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/request.py
--rw-r--r--   0 root         (0) root         (0)    68107 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/rse.py
--rw-r--r--   0 root         (0) root         (0)     5506 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/rse_counter.py
--rw-r--r--   0 root         (0) root         (0)    15368 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)    14577 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/rse_selector.py
--rw-r--r--   0 root         (0) root         (0)   208876 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/rule.py
--rw-r--r--   0 root         (0) root         (0)    94279 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/rule_grouping.py
--rw-r--r--   0 root         (0) root         (0)     5450 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/scope.py
--rw-r--r--   0 root         (0) root         (0)    15235 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/subscription.py
--rw-r--r--   0 root         (0) root         (0)    18930 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/topology.py
--rw-r--r--   0 root         (0) root         (0)    13107 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/trace.py
--rw-r--r--   0 root         (0) root         (0)    64200 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/transfer.py
--rw-r--r--   0 root         (0) root         (0)     5599 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/core/vo.py
--rw-r--r--   0 root         (0) root         (0)     5066 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/volatile_replica.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.705572 rucio-34.4.0/lib/rucio/daemons/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.706573 rucio-34.4.0/lib/rucio/daemons/abacus/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/abacus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3736 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/abacus/account.py
--rw-r--r--   0 root         (0) root         (0)     3856 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/abacus/collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3596 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/abacus/rse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.706573 rucio-34.4.0/lib/rucio/daemons/atropos/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/atropos/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10574 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/atropos/atropos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.707573 rucio-34.4.0/lib/rucio/daemons/auditor/
--rw-r--r--   0 root         (0) root         (0)    10003 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/auditor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2865 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/auditor/hdfs.py
--rw-r--r--   0 root         (0) root         (0)    10409 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/auditor/srmdumps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.707573 rucio-34.4.0/lib/rucio/daemons/automatix/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/automatix/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9974 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/automatix/automatix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.708572 rucio-34.4.0/lib/rucio/daemons/badreplicas/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/badreplicas/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15769 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/badreplicas/minos.py
--rw-r--r--   0 root         (0) root         (0)     8626 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py
--rw-r--r--   0 root         (0) root         (0)     9892 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/badreplicas/necromancer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.709573 rucio-34.4.0/lib/rucio/daemons/bb8/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/bb8/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13071 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/bb8/bb8.py
--rw-r--r--   0 root         (0) root         (0)    26778 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/bb8/common.py
--rw-r--r--   0 root         (0) root         (0)     6693 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/bb8/nuclei_background_rebalance.py
--rw-r--r--   0 root         (0) root         (0)     6571 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/bb8/t2_background_rebalance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.709573 rucio-34.4.0/lib/rucio/daemons/c3po/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.710573 rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4571 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/simple.py
--rw-r--r--   0 root         (0) root         (0)     4651 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/t2_free_space.py
--rw-r--r--   0 root         (0) root         (0)     4774 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py
--rw-r--r--   0 root         (0) root         (0)    12212 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py
--rw-r--r--   0 root         (0) root         (0)    15009 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/c3po.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.711573 rucio-34.4.0/lib/rucio/daemons/c3po/collectors/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/collectors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3261 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/collectors/agis.py
--rw-r--r--   0 root         (0) root         (0)     2094 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/collectors/free_space.py
--rw-r--r--   0 root         (0) root         (0)     1648 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/collectors/jedi_did.py
--rw-r--r--   0 root         (0) root         (0)     1339 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/collectors/mock_did.py
--rw-r--r--   0 root         (0) root         (0)     2068 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/collectors/network_metrics.py
--rw-r--r--   0 root         (0) root         (0)     3818 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/collectors/workload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.712573 rucio-34.4.0/lib/rucio/daemons/c3po/utils/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1386 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/utils/dataset_cache.py
--rw-r--r--   0 root         (0) root         (0)     1523 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py
--rw-r--r--   0 root         (0) root         (0)     1596 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/utils/expiring_list.py
--rw-r--r--   0 root         (0) root         (0)     2440 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/utils/popularity.py
--rw-r--r--   0 root         (0) root         (0)     2087 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/utils/timeseries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.713573 rucio-34.4.0/lib/rucio/daemons/cache/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-34.4.0/lib/rucio/daemons/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6744 2024-05-06 09:19:47.000000 rucio-34.4.0/lib/rucio/daemons/cache/consumer.py
--rw-r--r--   0 root         (0) root         (0)    14947 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.714573 rucio-34.4.0/lib/rucio/daemons/conveyor/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25817 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/common.py
--rw-r--r--   0 root         (0) root         (0)    23645 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/finisher.py
--rw-r--r--   0 root         (0) root         (0)    16241 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/poller.py
--rw-r--r--   0 root         (0) root         (0)     7462 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/preparer.py
--rw-r--r--   0 root         (0) root         (0)     8289 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/receiver.py
--rw-r--r--   0 root         (0) root         (0)     3986 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/stager.py
--rw-r--r--   0 root         (0) root         (0)    16333 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/submitter.py
--rw-r--r--   0 root         (0) root         (0)    20351 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/throttler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.715573 rucio-34.4.0/lib/rucio/daemons/follower/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/follower/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3355 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/follower/follower.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.715573 rucio-34.4.0/lib/rucio/daemons/hermes/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/hermes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26475 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/hermes/hermes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.716573 rucio-34.4.0/lib/rucio/daemons/judge/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/judge/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5772 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/judge/cleaner.py
--rw-r--r--   0 root         (0) root         (0)     7170 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/judge/evaluator.py
--rw-r--r--   0 root         (0) root         (0)     6394 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/judge/injector.py
--rw-r--r--   0 root         (0) root         (0)     5310 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/judge/repairer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.716573 rucio-34.4.0/lib/rucio/daemons/oauthmanager/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/oauthmanager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8817 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/oauthmanager/oauthmanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.717573 rucio-34.4.0/lib/rucio/daemons/reaper/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/reaper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11431 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/reaper/dark_reaper.py
--rw-r--r--   0 root         (0) root         (0)    35602 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/reaper/reaper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.717573 rucio-34.4.0/lib/rucio/daemons/replicarecoverer/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/replicarecoverer/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    35895 2024-05-21 07:16:09.000000 rucio-34.4.0/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.718573 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.719573 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/
--rw-r--r--   0 root         (0) root         (0)      863 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2221 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/atlas.py
--rw-r--r--   0 root         (0) root         (0)    16280 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/generic.py
--rw-r--r--   0 root         (0) root         (0)     2927 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/types.py
--rw-r--r--   0 root         (0) root         (0)    10413 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/rse_decommissioner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.719573 rucio-34.4.0/lib/rucio/daemons/storage/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.719573 rucio-34.4.0/lib/rucio/daemons/storage/consistency/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/storage/consistency/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29562 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/storage/consistency/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.720573 rucio-34.4.0/lib/rucio/daemons/tracer/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/tracer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23764 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/tracer/kronos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.720573 rucio-34.4.0/lib/rucio/daemons/transmogrifier/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/transmogrifier/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30581 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/transmogrifier/transmogrifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.720573 rucio-34.4.0/lib/rucio/daemons/undertaker/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/undertaker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5230 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/undertaker/undertaker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.721573 rucio-34.4.0/lib/rucio/db/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.722573 rucio-34.4.0/lib/rucio/db/sqla/
--rw-r--r--   0 root         (0) root         (0)     2506 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4151 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.722573 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3545 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.745573 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/
--rw-r--r--   0 root         (0) root         (0)     3340 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py
--rw-r--r--   0 root         (0) root         (0)     1821 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py
--rw-r--r--   0 root         (0) root         (0)     2640 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py
--rw-r--r--   0 root         (0) root         (0)     1533 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     5272 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py
--rw-r--r--   0 root         (0) root         (0)     3659 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py
--rw-r--r--   0 root         (0) root         (0)     1548 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py
--rw-r--r--   0 root         (0) root         (0)     2291 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py
--rw-r--r--   0 root         (0) root         (0)     2816 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py
--rw-r--r--   0 root         (0) root         (0)     1260 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py
--rw-r--r--   0 root         (0) root         (0)     1678 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py
--rw-r--r--   0 root         (0) root         (0)     2675 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py
--rw-r--r--   0 root         (0) root         (0)     1314 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py
--rw-r--r--   0 root         (0) root         (0)     8494 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py
--rw-r--r--   0 root         (0) root         (0)     3277 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py
--rw-r--r--   0 root         (0) root         (0)     3782 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py
--rw-r--r--   0 root         (0) root         (0)     1546 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py
--rw-r--r--   0 root         (0) root         (0)     1692 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py
--rw-r--r--   0 root         (0) root         (0)     4360 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py
--rw-r--r--   0 root         (0) root         (0)     3014 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py
--rw-r--r--   0 root         (0) root         (0)     1497 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py
--rw-r--r--   0 root         (0) root         (0)     2781 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py
--rw-r--r--   0 root         (0) root         (0)     2297 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py
--rw-r--r--   0 root         (0) root         (0)     1400 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1535 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     2274 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py
--rw-r--r--   0 root         (0) root         (0)     1219 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py
--rw-r--r--   0 root         (0) root         (0)     1710 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py
--rw-r--r--   0 root         (0) root         (0)     1723 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py
--rw-r--r--   0 root         (0) root         (0)     2206 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py
--rw-r--r--   0 root         (0) root         (0)     1787 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py
--rw-r--r--   0 root         (0) root         (0)     2837 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py
--rw-r--r--   0 root         (0) root         (0)     1554 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py
--rw-r--r--   0 root         (0) root         (0)     1571 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py
--rw-r--r--   0 root         (0) root         (0)     1758 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py
--rw-r--r--   0 root         (0) root         (0)     1308 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py
--rw-r--r--   0 root         (0) root         (0)     2019 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py
--rw-r--r--   0 root         (0) root         (0)     3882 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py
--rw-r--r--   0 root         (0) root         (0)     2513 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py
--rw-r--r--   0 root         (0) root         (0)     3997 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py
--rw-r--r--   0 root         (0) root         (0)     1470 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py
--rw-r--r--   0 root         (0) root         (0)     2817 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py
--rw-r--r--   0 root         (0) root         (0)     7527 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py
--rw-r--r--   0 root         (0) root         (0)     2396 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py
--rw-r--r--   0 root         (0) root         (0)     3592 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py
--rw-r--r--   0 root         (0) root         (0)     2687 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py
--rw-r--r--   0 root         (0) root         (0)     2777 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1287 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py
--rw-r--r--   0 root         (0) root         (0)     1644 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py
--rw-r--r--   0 root         (0) root         (0)     3682 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py
--rw-r--r--   0 root         (0) root         (0)     1420 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py
--rw-r--r--   0 root         (0) root         (0)     2424 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py
--rw-r--r--   0 root         (0) root         (0)     1666 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py
--rw-r--r--   0 root         (0) root         (0)     1585 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py
--rw-r--r--   0 root         (0) root         (0)     2008 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py
--rw-r--r--   0 root         (0) root         (0)     1272 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py
--rw-r--r--   0 root         (0) root         (0)     2757 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py
--rw-r--r--   0 root         (0) root         (0)     1598 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py
--rw-r--r--   0 root         (0) root         (0)     2476 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4df2c5ddabc0_remove_temporary_dids.py
--rw-r--r--   0 root         (0) root         (0)     1542 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py
--rw-r--r--   0 root         (0) root         (0)     1417 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py
--rw-r--r--   0 root         (0) root         (0)     1526 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py
--rw-r--r--   0 root         (0) root         (0)     1829 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py
--rw-r--r--   0 root         (0) root         (0)     2363 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py
--rw-r--r--   0 root         (0) root         (0)     1701 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py
--rw-r--r--   0 root         (0) root         (0)     6101 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py
--rw-r--r--   0 root         (0) root         (0)     2266 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py
--rw-r--r--   0 root         (0) root         (0)     1666 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py
--rw-r--r--   0 root         (0) root         (0)     1969 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1559 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py
--rw-r--r--   0 root         (0) root         (0)     1363 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py
--rw-r--r--   0 root         (0) root         (0)     5023 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py
--rw-r--r--   0 root         (0) root         (0)     3568 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py
--rw-r--r--   0 root         (0) root         (0)     1893 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py
--rw-r--r--   0 root         (0) root         (0)     1889 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py
--rw-r--r--   0 root         (0) root         (0)     1661 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py
--rw-r--r--   0 root         (0) root         (0)     1715 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py
--rw-r--r--   0 root         (0) root         (0)     3118 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1749 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py
--rw-r--r--   0 root         (0) root         (0)     5038 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py
--rw-r--r--   0 root         (0) root         (0)     1938 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py
--rw-r--r--   0 root         (0) root         (0)     3689 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py
--rw-r--r--   0 root         (0) root         (0)     2614 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a08fa8de1545_transfer_stats_table.py
--rw-r--r--   0 root         (0) root         (0)     3117 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py
--rw-r--r--   0 root         (0) root         (0)     5836 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py
--rw-r--r--   0 root         (0) root         (0)     2595 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py
--rw-r--r--   0 root         (0) root         (0)     2195 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py
--rw-r--r--   0 root         (0) root         (0)     2173 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py
--rw-r--r--   0 root         (0) root         (0)     1883 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1546 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py
--rw-r--r--   0 root         (0) root         (0)     5407 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py
--rw-r--r--   0 root         (0) root         (0)     1348 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py
--rw-r--r--   0 root         (0) root         (0)     1585 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py
--rw-r--r--   0 root         (0) root         (0)     7344 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py
--rw-r--r--   0 root         (0) root         (0)     3704 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py
--rw-r--r--   0 root         (0) root         (0)     2091 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py
--rw-r--r--   0 root         (0) root         (0)     2934 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py
--rw-r--r--   0 root         (0) root         (0)     2784 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py
--rw-r--r--   0 root         (0) root         (0)     1747 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py
--rw-r--r--   0 root         (0) root         (0)     9561 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py
--rw-r--r--   0 root         (0) root         (0)     4748 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py
--rw-r--r--   0 root         (0) root         (0)     1736 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1594 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py
--rw-r--r--   0 root         (0) root         (0)     5263 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py
--rw-r--r--   0 root         (0) root         (0)     2429 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py
--rw-r--r--   0 root         (0) root         (0)     4865 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py
--rw-r--r--   0 root         (0) root         (0)      897 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py
--rw-r--r--   0 root         (0) root         (0)     2947 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py
--rw-r--r--   0 root         (0) root         (0)     1949 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py
--rw-r--r--   0 root         (0) root         (0)     1110 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py
--rw-r--r--   0 root         (0) root         (0)     1896 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py
--rw-r--r--   0 root         (0) root         (0)     1599 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py
--rw-r--r--   0 root         (0) root         (0)   112134 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/db/sqla/models.py
--rw-r--r--   0 root         (0) root         (0)     1658 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/sautils.py
--rw-r--r--   0 root         (0) root         (0)    17773 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/session.py
--rw-r--r--   0 root         (0) root         (0)     6088 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/types.py
--rw-r--r--   0 root         (0) root         (0)    22230 2024-05-21 09:34:41.000000 rucio-34.4.0/lib/rucio/db/sqla/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.746573 rucio-34.4.0/lib/rucio/rse/
--rw-r--r--   0 root         (0) root         (0)     3303 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.749573 rucio-34.4.0/lib/rucio/rse/protocols/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7199 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/bittorrent.py
--rw-r--r--   0 root         (0) root         (0)     4603 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/cache.py
--rw-r--r--   0 root         (0) root         (0)     4225 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/dummy.py
--rw-r--r--   0 root         (0) root         (0)    29100 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/gfal.py
--rw-r--r--   0 root         (0) root         (0)     9730 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/globus.py
--rw-r--r--   0 root         (0) root         (0)     3411 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/gsiftp.py
--rw-r--r--   0 root         (0) root         (0)     2975 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/http_cache.py
--rw-r--r--   0 root         (0) root         (0)     4495 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/mock.py
--rw-r--r--   0 root         (0) root         (0)     7224 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/ngarc.py
--rw-r--r--   0 root         (0) root         (0)    10414 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/rse/protocols/posix.py
--rw-r--r--   0 root         (0) root         (0)    21937 2024-05-21 07:56:16.000000 rucio-34.4.0/lib/rucio/rse/protocols/protocol.py
--rw-r--r--   0 root         (0) root         (0)    15260 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/rclone.py
--rw-r--r--   0 root         (0) root         (0)     5501 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/rfio.py
--rw-r--r--   0 root         (0) root         (0)    14689 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/rse/protocols/srm.py
--rw-r--r--   0 root         (0) root         (0)    17473 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/ssh.py
--rw-r--r--   0 root         (0) root         (0)     8141 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/rse/protocols/storm.py
--rw-r--r--   0 root         (0) root         (0)    22448 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/rse/protocols/webdav.py
--rw-r--r--   0 root         (0) root         (0)    12571 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/xrootd.py
--rw-r--r--   0 root         (0) root         (0)    37238 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/rsemanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.749573 rucio-34.4.0/lib/rucio/tests/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8907 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     5045 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/tests/common_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.751573 rucio-34.4.0/lib/rucio/transfertool/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8342 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/bittorrent.py
--rw-r--r--   0 root         (0) root         (0)     1705 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/bittorrent_driver.py
--rw-r--r--   0 root         (0) root         (0)     4966 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/bittorrent_driver_qbittorrent.py
--rw-r--r--   0 root         (0) root         (0)    72157 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/fts3.py
--rw-r--r--   0 root         (0) root         (0)     6156 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/fts3_plugins.py
--rw-r--r--   0 root         (0) root         (0)     7716 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/globus.py
--rw-r--r--   0 root         (0) root         (0)     8411 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/globus_library.py
--rw-r--r--   0 root         (0) root         (0)     2859 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/mock.py
--rw-r--r--   0 root         (0) root         (0)     7752 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/transfertool.py
--rw-r--r--   0 root         (0) root         (0)      244 2024-05-21 12:45:12.000000 rucio-34.4.0/lib/rucio/vcsversion.py
--rw-r--r--   0 root         (0) root         (0)     1577 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.751573 rucio-34.4.0/lib/rucio/web/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.752573 rucio-34.4.0/lib/rucio/web/rest/
--rwxr-xr-x   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.752573 rucio-34.4.0/lib/rucio/web/rest/flaskapi/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)      999 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/authenticated_bp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.758573 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7791 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/accountlimits.py
--rw-r--r--   0 root         (0) root         (0)    36983 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/accounts.py
--rw-r--r--   0 root         (0) root         (0)     3344 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/archives.py
--rw-r--r--   0 root         (0) root         (0)    61047 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/auth.py
--rw-r--r--   0 root         (0) root         (0)    16148 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/common.py
--rw-r--r--   0 root         (0) root         (0)    10143 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/config.py
--rw-r--r--   0 root         (0) root         (0)     7714 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/credentials.py
--rw-r--r--   0 root         (0) root         (0)    80867 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/dids.py
--rw-r--r--   0 root         (0) root         (0)     4706 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/dirac.py
--rw-r--r--   0 root         (0) root         (0)     2656 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/export.py
--rw-r--r--   0 root         (0) root         (0)     4620 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/heartbeats.py
--rw-r--r--   0 root         (0) root         (0)     7894 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/identities.py
--rw-r--r--   0 root         (0) root         (0)     5259 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/import.py
--rw-r--r--   0 root         (0) root         (0)    12009 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py
--rw-r--r--   0 root         (0) root         (0)    12990 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/locks.py
--rw-r--r--   0 root         (0) root         (0)     2860 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/main.py
--rw-r--r--   0 root         (0) root         (0)     7785 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     1250 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/metrics.py
--rw-r--r--   0 root         (0) root         (0)     3131 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py
--rw-r--r--   0 root         (0) root         (0)     3096 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/ping.py
--rw-r--r--   0 root         (0) root         (0)    13331 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/redirect.py
--rw-r--r--   0 root         (0) root         (0)    72711 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/replicas.py
--rw-r--r--   0 root         (0) root         (0)    41622 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/requests.py
--rw-r--r--   0 root         (0) root         (0)    81948 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/rses.py
--rw-r--r--   0 root         (0) root         (0)    32189 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/rules.py
--rw-r--r--   0 root         (0) root         (0)     5068 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/scopes.py
--rw-r--r--   0 root         (0) root         (0)    24151 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/subscriptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.758573 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/templates/
--rw-r--r--   0 root         (0) root         (0)     2254 2023-07-27 12:40:37.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html
--rw-r--r--   0 root         (0) root         (0)     2139 2023-07-27 12:40:37.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html
--rw-r--r--   0 root         (0) root         (0)     3213 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/traces.py
--rw-r--r--   0 root         (0) root         (0)     9154 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/vos.py
--rw-r--r--   0 root         (0) root         (0)      725 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/main.py
--rw-r--r--   0 root         (0) root         (0)     1016 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/metrics.py
--rw-r--r--   0 root         (0) root         (0)     1010 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/ping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.777573 rucio-34.4.0/lib/rucio.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25876 2024-05-21 14:54:21.000000 rucio-34.4.0/lib/rucio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    16384 2024-05-06 09:19:47.000000 rucio-34.4.0/pylintrc
--rw-r--r--   0 root         (0) root         (0)     5763 2024-05-21 07:56:54.000000 rucio-34.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5235 2024-05-21 09:35:26.000000 rucio-34.4.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      206 2024-05-21 14:54:21.783573 rucio-34.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2932 2024-05-21 14:54:17.000000 rucio-34.4.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     4778 2024-05-16 07:28:57.000000 rucio-34.4.0/setuputil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.776573 rucio-34.4.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3682 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_abacus_account.py
--rw-r--r--   0 root         (0) root         (0)    10677 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_abacus_collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3229 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_abacus_rse.py
--rw-r--r--   0 root         (0) root         (0)    15923 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_account.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_account_limits.py
--rw-r--r--   0 root         (0) root         (0)    20523 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_api_external_representation.py
--rw-r--r--   0 root         (0) root         (0)    13352 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_archive.py
--rw-r--r--   0 root         (0) root         (0)     4074 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_auditor.py
--rw-r--r--   0 root         (0) root         (0)     2181 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_auditor_hdfs.py
--rw-r--r--   0 root         (0) root         (0)     4201 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_auditor_srmdumps.py
--rw-r--r--   0 root         (0) root         (0)    14964 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_authentication.py
--rw-r--r--   0 root         (0) root         (0)     3464 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_automatix.py
--rw-r--r--   0 root         (0) root         (0)    23265 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_bad_replica.py
--rw-r--r--   0 root         (0) root         (0)    12425 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_bb8.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_belleii.py
--rwxr-xr-x   0 root         (0) root         (0)   107450 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_bin_rucio.py
--rw-r--r--   0 root         (0) root         (0)     2065 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)     8398 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_clients.py
--rw-r--r--   0 root         (0) root         (0)     1865 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_common_types.py
--rw-r--r--   0 root         (0) root         (0)     6942 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    96724 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_conveyor.py
--rw-r--r--   0 root         (0) root         (0)    23870 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_conveyor_submitter.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_counter.py
--rw-r--r--   0 root         (0) root         (0)     7728 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_credential.py
--rw-r--r--   0 root         (0) root         (0)     7337 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_curl.py
--rw-r--r--   0 root         (0) root         (0)     2618 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_daemons.py
--rw-r--r--   0 root         (0) root         (0)    28183 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_dataset_replicas.py
--rw-r--r--   0 root         (0) root         (0)     2736 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_db.py
--rw-r--r--   0 root         (0) root         (0)    58823 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_did.py
--rw-r--r--   0 root         (0) root         (0)    29517 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_did_meta_plugins.py
--rw-r--r--   0 root         (0) root         (0)     4185 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_didtype.py
--rw-r--r--   0 root         (0) root         (0)    35315 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)     7118 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_dumper.py
--rw-r--r--   0 root         (0) root         (0)    16419 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_dumper_consistency.py
--rw-r--r--   0 root         (0) root         (0)    10869 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_dumper_data_model.py
--rw-r--r--   0 root         (0) root         (0)     3082 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_dumper_path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    38301 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     7953 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    10106 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_hermes.py
--rw-r--r--   0 root         (0) root         (0)     5821 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_identity.py
--rw-r--r--   0 root         (0) root         (0)    18584 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_impl_upload_download.py
--rw-r--r--   0 root         (0) root         (0)    57290 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_import_export.py
--rw-r--r--   0 root         (0) root         (0)     5258 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_judge_cleaner.py
--rw-r--r--   0 root         (0) root         (0)    22277 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_judge_evaluator.py
--rw-r--r--   0 root         (0) root         (0)    11050 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_judge_injector.py
--rw-r--r--   0 root         (0) root         (0)    20429 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_judge_repairer.py
--rw-r--r--   0 root         (0) root         (0)    12180 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_lifetime.py
--rw-r--r--   0 root         (0) root         (0)     5855 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_message.py
--rw-r--r--   0 root         (0) root         (0)     6299 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_meta_did.py
--rw-r--r--   0 root         (0) root         (0)      957 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_module_import.py
--rw-r--r--   0 root         (0) root         (0)     2034 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_monitor.py
--rw-r--r--   0 root         (0) root         (0)    54332 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     2759 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_naming_convention.py
--rw-r--r--   0 root         (0) root         (0)    11582 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_oauthmanager.py
--rw-r--r--   0 root         (0) root         (0)   108359 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_oidc.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_permission.py
--rw-r--r--   0 root         (0) root         (0)     4123 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_pfns.py
--rw-r--r--   0 root         (0) root         (0)     1141 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_ping.py
--rw-r--r--   0 root         (0) root         (0)     7662 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_preparer.py
--rw-r--r--   0 root         (0) root         (0)     2741 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_qos.py
--rw-r--r--   0 root         (0) root         (0)     2023 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    27487 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_reaper.py
--rw-r--r--   0 root         (0) root         (0)     6440 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_redirect.py
--rw-r--r--   0 root         (0) root         (0)    62467 2024-05-21 07:56:54.000000 rucio-34.4.0/tests/test_replica.py
--rw-r--r--   0 root         (0) root         (0)    42098 2024-05-21 07:16:09.000000 rucio-34.4.0/tests/test_replica_recoverer.py
--rw-r--r--   0 root         (0) root         (0)    22796 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_replica_sorting.py
--rw-r--r--   0 root         (0) root         (0)    17257 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_request.py
--rw-r--r--   0 root         (0) root         (0)    13033 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_root_proxy.py
--rw-r--r--   0 root         (0) root         (0)    75080 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse.py
--rw-r--r--   0 root         (0) root         (0)    13184 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)     8940 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_lfn2path.py
--rw-r--r--   0 root         (0) root         (0)     4277 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_gfal2.py
--rw-r--r--   0 root         (0) root         (0)     3822 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_gfal2_impl.py
--rw-r--r--   0 root         (0) root         (0)     3267 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_posix.py
--rw-r--r--   0 root         (0) root         (0)     3690 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_rclone.py
--rw-r--r--   0 root         (0) root         (0)     4799 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_rsync.py
--rw-r--r--   0 root         (0) root         (0)     3979 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_srm.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_ssh.py
--rw-r--r--   0 root         (0) root         (0)     3015 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_webdav.py
--rw-r--r--   0 root         (0) root         (0)     3780 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_xrootd.py
--rw-r--r--   0 root         (0) root         (0)     7746 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_selector.py
--rw-r--r--   0 root         (0) root         (0)      867 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)    91949 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_rule.py
--rw-r--r--   0 root         (0) root         (0)     7486 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_scope.py
--rw-r--r--   0 root         (0) root         (0)    48389 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_subscription.py
--rw-r--r--   0 root         (0) root         (0)    55587 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_throttler.py
--rw-r--r--   0 root         (0) root         (0)     5011 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_tpc.py
--rw-r--r--   0 root         (0) root         (0)     3181 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_trace.py
--rw-r--r--   0 root         (0) root         (0)    25254 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_transfer.py
--rw-r--r--   0 root         (0) root         (0)     8924 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_transfer_plugins.py
--rw-r--r--   0 root         (0) root         (0)     8412 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_undertaker.py
--rw-r--r--   0 root         (0) root         (0)    15575 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_upload.py
--rw-r--r--   0 root         (0) root         (0)     7427 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.777573 rucio-34.4.0/tools/
--rwxr-xr-x   0 root         (0) root         (0)     1259 2024-05-16 07:28:57.000000 rucio-34.4.0/tools/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     6163 2024-05-16 07:28:57.000000 rucio-34.4.0/tools/merge_rucio_configs.py
--rwxr-xr-x   0 root         (0) root         (0)     1351 2024-05-16 07:28:57.000000 rucio-34.4.0/tools/reset_database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:31.013405 rucio-34.4.1/
+-rwxr-xr-x   0 root         (0) root         (0)     4487 2024-05-23 08:12:33.000000 rucio-34.4.1/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio-34.4.1/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio-34.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      934 2024-05-24 12:25:27.000000 rucio-34.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2790 2024-05-24 12:25:31.013405 rucio-34.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-05-24 11:15:54.000000 rucio-34.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.919404 rucio-34.4.1/bin/
+-rwxr-xr-x   0 root         (0) root         (0)   127119 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio
+-rwxr-xr-x   0 root         (0) root         (0)     2820 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-abacus-account
+-rwxr-xr-x   0 root         (0) root         (0)     1823 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-abacus-collection-replica
+-rwxr-xr-x   0 root         (0) root         (0)     2567 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-abacus-rse
+-rwxr-xr-x   0 root         (0) root         (0)   133582 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-admin
+-rwxr-xr-x   0 root         (0) root         (0)     3185 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-atropos
+-rwxr-xr-x   0 root         (0) root         (0)     5850 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-auditor
+-rwxr-xr-x   0 root         (0) root         (0)     2010 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-automatix
+-rwxr-xr-x   0 root         (0) root         (0)     3103 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-bb8
+-rwxr-xr-x   0 root         (0) root         (0)     6100 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-c3po
+-rwxr-xr-x   0 root         (0) root         (0)     5060 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-cache-client
+-rwxr-xr-x   0 root         (0) root         (0)     1362 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-cache-consumer
+-rwxr-xr-x   0 root         (0) root         (0)     2347 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-conveyor-finisher
+-rwxr-xr-x   0 root         (0) root         (0)     2839 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-conveyor-poller
+-rwxr-xr-x   0 root         (0) root         (0)     1759 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-conveyor-preparer
+-rwxr-xr-x   0 root         (0) root         (0)     1682 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-conveyor-receiver
+-rwxr-xr-x   0 root         (0) root         (0)     3385 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-conveyor-stager
+-rwxr-xr-x   0 root         (0) root         (0)     6752 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-conveyor-submitter
+-rwxr-xr-x   0 root         (0) root         (0)     3859 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-conveyor-throttler
+-rwxr-xr-x   0 root         (0) root         (0)     2546 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-dark-reaper
+-rwxr-xr-x   0 root         (0) root         (0)     6463 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-dumper
+-rwxr-xr-x   0 root         (0) root         (0)     1414 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-follower
+-rwxr-xr-x   0 root         (0) root         (0)     1987 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-hermes
+-rwxr-xr-x   0 root         (0) root         (0)     4649 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-judge-cleaner
+-rwxr-xr-x   0 root         (0) root         (0)     7472 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-judge-evaluator
+-rwxr-xr-x   0 root         (0) root         (0)     1671 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-judge-injector
+-rwxr-xr-x   0 root         (0) root         (0)     1675 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-judge-repairer
+-rwxr-xr-x   0 root         (0) root         (0)     1782 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-kronos
+-rwxr-xr-x   0 root         (0) root         (0)     2260 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-minos
+-rwxr-xr-x   0 root         (0) root         (0)     1997 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-minos-temporary-expiration
+-rwxr-xr-x   0 root         (0) root         (0)     5626 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-necromancer
+-rwxr-xr-x   0 root         (0) root         (0)     2790 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-oauth-manager
+-rwxr-xr-x   0 root         (0) root         (0)     4070 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-reaper
+-rwxr-xr-x   0 root         (0) root         (0)    18988 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-replica-recoverer
+-rwxr-xr-x   0 root         (0) root         (0)     2351 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-rse-decommissioner
+-rwxr-xr-x   0 root         (0) root         (0)     3920 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-storage-consistency-actions
+-rwxr-xr-x   0 root         (0) root         (0)     3364 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-transmogrifier
+-rwxr-xr-x   0 root         (0) root         (0)     2720 2024-05-23 08:12:33.000000 rucio-34.4.1/bin/rucio-undertaker
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.920404 rucio-34.4.1/etc/
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-07-27 12:40:37.000000 rucio-34.4.1/etc/alembic.ini.template
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-07-27 12:40:37.000000 rucio-34.4.1/etc/alembic_offline.ini.template
+-rw-r--r--   0 root         (0) root         (0)       96 2023-07-27 12:40:37.000000 rucio-34.4.1/etc/globus-config.yml.template
+-rw-r--r--   0 root         (0) root         (0)      806 2024-05-23 08:12:33.000000 rucio-34.4.1/etc/ldap.cfg.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.921404 rucio-34.4.1/etc/mail_templates/
+-rw-r--r--   0 root         (0) root         (0)     1210 2024-05-06 09:19:47.000000 rucio-34.4.1/etc/mail_templates/rule_approval_request.tmpl
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-27 12:40:37.000000 rucio-34.4.1/etc/mail_templates/rule_approved_admin.tmpl
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-27 12:40:37.000000 rucio-34.4.1/etc/mail_templates/rule_approved_user.tmpl
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-27 12:40:37.000000 rucio-34.4.1/etc/mail_templates/rule_denied_admin.tmpl
+-rw-r--r--   0 root         (0) root         (0)      493 2023-07-27 12:40:37.000000 rucio-34.4.1/etc/mail_templates/rule_denied_user.tmpl
+-rw-r--r--   0 root         (0) root         (0)      546 2023-07-27 12:40:37.000000 rucio-34.4.1/etc/mail_templates/rule_ok_notification.tmpl
+-rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio-34.4.1/etc/rse-accounts.cfg.template
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio-34.4.1/etc/rucio.cfg.atlas.client.template
+-rw-r--r--   0 root         (0) root         (0)     8534 2024-05-06 09:19:47.000000 rucio-34.4.1/etc/rucio.cfg.template
+-rw-r--r--   0 root         (0) root         (0)     7477 2024-05-06 09:19:47.000000 rucio-34.4.1/etc/rucio_multi_vo.cfg.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.906404 rucio-34.4.1/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.922404 rucio-34.4.1/lib/rucio/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      690 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/alembicrevision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.926405 rucio-34.4.1/lib/rucio/api/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9396 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/account.py
+-rw-r--r--   0 root         (0) root         (0)    11394 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/account_limit.py
+-rw-r--r--   0 root         (0) root         (0)    12890 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/authentication.py
+-rw-r--r--   0 root         (0) root         (0)     9085 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/config.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/credential.py
+-rw-r--r--   0 root         (0) root         (0)    29418 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/did.py
+-rw-r--r--   0 root         (0) root         (0)     3206 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/dirac.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/exporter.py
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)     6830 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/identity.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/importer.py
+-rw-r--r--   0 root         (0) root         (0)     3685 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/lifetime_exception.py
+-rw-r--r--   0 root         (0) root         (0)     4628 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/lock.py
+-rw-r--r--   0 root         (0) root         (0)     3615 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/permission.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    22565 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/replica.py
+-rw-r--r--   0 root         (0) root         (0)    10550 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/request.py
+-rw-r--r--   0 root         (0) root         (0)    23637 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/rse.py
+-rw-r--r--   0 root         (0) root         (0)    16037 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/rule.py
+-rw-r--r--   0 root         (0) root         (0)     3055 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/scope.py
+-rw-r--r--   0 root         (0) root         (0)    10537 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     4817 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/api/vo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.930405 rucio-34.4.1/lib/rucio/client/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16352 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/accountclient.py
+-rw-r--r--   0 root         (0) root         (0)     5961 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/accountlimitclient.py
+-rw-r--r--   0 root         (0) root         (0)    48035 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/baseclient.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     4401 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/configclient.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/credentialclient.py
+-rw-r--r--   0 root         (0) root         (0)    28378 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/didclient.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/diracclient.py
+-rw-r--r--   0 root         (0) root         (0)    87520 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/downloadclient.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/exportclient.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/fileclient.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/importclient.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/lifetimeclient.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/lockclient.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/metaconventionsclient.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/pingclient.py
+-rw-r--r--   0 root         (0) root         (0)    19518 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/replicaclient.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/requestclient.py
+-rw-r--r--   0 root         (0) root         (0)    27121 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/rseclient.py
+-rw-r--r--   0 root         (0) root         (0)    12734 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/ruleclient.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/scopeclient.py
+-rw-r--r--   0 root         (0) root         (0)     7971 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/subscriptionclient.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/touchclient.py
+-rw-r--r--   0 root         (0) root         (0)    46920 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/client/uploadclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.932405 rucio-34.4.1/lib/rucio/common/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/cache.py
+-rw-r--r--   0 root         (0) root         (0)    24636 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/config.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/constants.py
+-rw-r--r--   0 root         (0) root         (0)      726 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/constraints.py
+-rwxr-xr-x   0 root         (0) root         (0)     6545 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/didtype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.933405 rucio-34.4.1/lib/rucio/common/dumper/
+-rw-r--r--   0 root         (0) root         (0)    10796 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/dumper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15985 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/dumper/consistency.py
+-rw-r--r--   0 root         (0) root         (0)     9693 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/dumper/data_models.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/dumper/path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    32345 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/exception.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/extra.py
+-rw-r--r--   0 root         (0) root         (0)    15046 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/logging.py
+-rw-r--r--   0 root         (0) root         (0)    45338 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/pcache.py
+-rw-r--r--   0 root         (0) root         (0)     6071 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.935405 rucio-34.4.1/lib/rucio/common/schema/
+-rw-r--r--   0 root         (0) root         (0)     5384 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15589 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/schema/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    15406 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/schema/belleii.py
+-rw-r--r--   0 root         (0) root         (0)    14987 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/schema/domatpc.py
+-rw-r--r--   0 root         (0) root         (0)    15926 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/schema/escape.py
+-rw-r--r--   0 root         (0) root         (0)    16241 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/schema/generic.py
+-rw-r--r--   0 root         (0) root         (0)    15468 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/schema/generic_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)    15277 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/schema/icecube.py
+-rw-r--r--   0 root         (0) root         (0)     5414 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/stomp_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/stopwatch.py
+-rw-r--r--   0 root         (0) root         (0)     4935 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)     5716 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/common/types.py
+-rw-r--r--   0 root         (0) root         (0)    79163 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.942405 rucio-34.4.1/lib/rucio/core/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14952 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/account.py
+-rw-r--r--   0 root         (0) root         (0)     6289 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/account_counter.py
+-rw-r--r--   0 root         (0) root         (0)    14274 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/account_limit.py
+-rw-r--r--   0 root         (0) root         (0)    21045 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/authentication.py
+-rw-r--r--   0 root         (0) root         (0)    13462 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/config.py
+-rw-r--r--   0 root         (0) root         (0)     8211 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/credential.py
+-rw-r--r--   0 root         (0) root         (0)   129547 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/did.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.943405 rucio-34.4.1/lib/rucio/core/did_meta_plugins/
+-rw-r--r--   0 root         (0) root         (0)    11733 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/did_meta_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17445 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/did_meta_plugins/did_column_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4932 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py
+-rw-r--r--   0 root         (0) root         (0)    30038 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/did_meta_plugins/filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     9215 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/did_meta_plugins/json_meta.py
+-rw-r--r--   0 root         (0) root         (0)     7431 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/did_meta_plugins/mongo_meta.py
+-rw-r--r--   0 root         (0) root         (0)    13727 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/did_meta_plugins/postgres_meta.py
+-rw-r--r--   0 root         (0) root         (0)     9402 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/dirac.py
+-rw-r--r--   0 root         (0) root         (0)     5735 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/distance.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/exporter.py
+-rw-r--r--   0 root         (0) root         (0)    10986 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    12099 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/identity.py
+-rw-r--r--   0 root         (0) root         (0)    14169 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/importer.py
+-rw-r--r--   0 root         (0) root         (0)    15254 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/lifetime_exception.py
+-rw-r--r--   0 root         (0) root         (0)    22857 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/lock.py
+-rw-r--r--   0 root         (0) root         (0)     9693 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/message.py
+-rw-r--r--   0 root         (0) root         (0)     8691 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)    15984 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/monitor.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)     4890 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/nongrid_trace.py
+-rw-r--r--   0 root         (0) root         (0)    69833 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/oidc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.944405 rucio-34.4.1/lib/rucio/core/permission/
+-rw-r--r--   0 root         (0) root         (0)     4070 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/permission/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55734 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/permission/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    46969 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/permission/belleii.py
+-rw-r--r--   0 root         (0) root         (0)    43171 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/permission/escape.py
+-rw-r--r--   0 root         (0) root         (0)    48439 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/permission/generic.py
+-rw-r--r--   0 root         (0) root         (0)    45926 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/permission/generic_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     8030 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)   177082 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/replica.py
+-rw-r--r--   0 root         (0) root         (0)    15434 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/replica_sorter.py
+-rw-r--r--   0 root         (0) root         (0)   116306 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/request.py
+-rw-r--r--   0 root         (0) root         (0)    68107 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/rse.py
+-rw-r--r--   0 root         (0) root         (0)     5506 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/rse_counter.py
+-rw-r--r--   0 root         (0) root         (0)    15368 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)    14577 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)   208876 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/rule.py
+-rw-r--r--   0 root         (0) root         (0)    94279 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/rule_grouping.py
+-rw-r--r--   0 root         (0) root         (0)     5450 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/scope.py
+-rw-r--r--   0 root         (0) root         (0)    15235 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/subscription.py
+-rw-r--r--   0 root         (0) root         (0)    18930 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/topology.py
+-rw-r--r--   0 root         (0) root         (0)    13107 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/trace.py
+-rw-r--r--   0 root         (0) root         (0)    64200 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/transfer.py
+-rw-r--r--   0 root         (0) root         (0)     5599 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/vo.py
+-rw-r--r--   0 root         (0) root         (0)     5066 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/core/volatile_replica.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.944405 rucio-34.4.1/lib/rucio/daemons/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.945405 rucio-34.4.1/lib/rucio/daemons/abacus/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/abacus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3736 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/abacus/account.py
+-rw-r--r--   0 root         (0) root         (0)     3856 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/abacus/collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/abacus/rse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.945405 rucio-34.4.1/lib/rucio/daemons/atropos/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/atropos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10574 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/atropos/atropos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.946405 rucio-34.4.1/lib/rucio/daemons/auditor/
+-rw-r--r--   0 root         (0) root         (0)    10003 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/auditor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2865 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/auditor/hdfs.py
+-rw-r--r--   0 root         (0) root         (0)    10409 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/auditor/srmdumps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.946405 rucio-34.4.1/lib/rucio/daemons/automatix/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/automatix/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9974 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/automatix/automatix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.947405 rucio-34.4.1/lib/rucio/daemons/badreplicas/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/badreplicas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15769 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/badreplicas/minos.py
+-rw-r--r--   0 root         (0) root         (0)     8626 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py
+-rw-r--r--   0 root         (0) root         (0)     9892 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/badreplicas/necromancer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.948405 rucio-34.4.1/lib/rucio/daemons/bb8/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/bb8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13071 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/bb8/bb8.py
+-rw-r--r--   0 root         (0) root         (0)    26778 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/bb8/common.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/bb8/nuclei_background_rebalance.py
+-rw-r--r--   0 root         (0) root         (0)     6571 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/bb8/t2_background_rebalance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.948405 rucio-34.4.1/lib/rucio/daemons/c3po/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.949405 rucio-34.4.1/lib/rucio/daemons/c3po/algorithms/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/algorithms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4571 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/algorithms/simple.py
+-rw-r--r--   0 root         (0) root         (0)     4651 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/algorithms/t2_free_space.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py
+-rw-r--r--   0 root         (0) root         (0)    12212 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py
+-rw-r--r--   0 root         (0) root         (0)    15009 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/c3po.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.950405 rucio-34.4.1/lib/rucio/daemons/c3po/collectors/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/collectors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3261 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/collectors/agis.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/collectors/free_space.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/collectors/jedi_did.py
+-rw-r--r--   0 root         (0) root         (0)     1339 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/collectors/mock_did.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/collectors/network_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     3818 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/collectors/workload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.951405 rucio-34.4.1/lib/rucio/daemons/c3po/utils/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/utils/dataset_cache.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/utils/expiring_list.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/utils/popularity.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/c3po/utils/timeseries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.951405 rucio-34.4.1/lib/rucio/daemons/cache/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-34.4.1/lib/rucio/daemons/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6744 2024-05-06 09:19:47.000000 rucio-34.4.1/lib/rucio/daemons/cache/consumer.py
+-rw-r--r--   0 root         (0) root         (0)    14947 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.953405 rucio-34.4.1/lib/rucio/daemons/conveyor/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/conveyor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25817 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/conveyor/common.py
+-rw-r--r--   0 root         (0) root         (0)    23645 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/conveyor/finisher.py
+-rw-r--r--   0 root         (0) root         (0)    16241 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/conveyor/poller.py
+-rw-r--r--   0 root         (0) root         (0)     7462 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/conveyor/preparer.py
+-rw-r--r--   0 root         (0) root         (0)     8289 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/conveyor/receiver.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/conveyor/stager.py
+-rw-r--r--   0 root         (0) root         (0)    16333 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/conveyor/submitter.py
+-rw-r--r--   0 root         (0) root         (0)    20351 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/conveyor/throttler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.953405 rucio-34.4.1/lib/rucio/daemons/follower/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/follower/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/follower/follower.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.953405 rucio-34.4.1/lib/rucio/daemons/hermes/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/hermes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26475 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/hermes/hermes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.954405 rucio-34.4.1/lib/rucio/daemons/judge/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/judge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5772 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/judge/cleaner.py
+-rw-r--r--   0 root         (0) root         (0)     7170 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/judge/evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     6394 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/judge/injector.py
+-rw-r--r--   0 root         (0) root         (0)     5310 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/judge/repairer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.954405 rucio-34.4.1/lib/rucio/daemons/oauthmanager/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/oauthmanager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8817 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/oauthmanager/oauthmanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.955405 rucio-34.4.1/lib/rucio/daemons/reaper/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/reaper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11431 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/reaper/dark_reaper.py
+-rw-r--r--   0 root         (0) root         (0)    35602 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/reaper/reaper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.955405 rucio-34.4.1/lib/rucio/daemons/replicarecoverer/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/replicarecoverer/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    35895 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.956405 rucio-34.4.1/lib/rucio/daemons/rsedecommissioner/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/rsedecommissioner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/rsedecommissioner/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.956405 rucio-34.4.1/lib/rucio/daemons/rsedecommissioner/profiles/
+-rw-r--r--   0 root         (0) root         (0)      863 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/rsedecommissioner/profiles/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2221 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/rsedecommissioner/profiles/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    16280 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/rsedecommissioner/profiles/generic.py
+-rw-r--r--   0 root         (0) root         (0)     2927 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/rsedecommissioner/profiles/types.py
+-rw-r--r--   0 root         (0) root         (0)    10413 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/rsedecommissioner/rse_decommissioner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.956405 rucio-34.4.1/lib/rucio/daemons/storage/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.957405 rucio-34.4.1/lib/rucio/daemons/storage/consistency/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/storage/consistency/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29562 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/storage/consistency/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.957405 rucio-34.4.1/lib/rucio/daemons/tracer/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/tracer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23764 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/tracer/kronos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.957405 rucio-34.4.1/lib/rucio/daemons/transmogrifier/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/transmogrifier/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30581 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/transmogrifier/transmogrifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.958405 rucio-34.4.1/lib/rucio/daemons/undertaker/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/undertaker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5230 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/daemons/undertaker/undertaker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.958405 rucio-34.4.1/lib/rucio/db/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.959405 rucio-34.4.1/lib/rucio/db/sqla/
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4151 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.959405 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3545 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.980405 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/
+-rw-r--r--   0 root         (0) root         (0)     3340 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py
+-rw-r--r--   0 root         (0) root         (0)     2640 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     5272 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py
+-rw-r--r--   0 root         (0) root         (0)     1260 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py
+-rw-r--r--   0 root         (0) root         (0)     1678 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py
+-rw-r--r--   0 root         (0) root         (0)     8494 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py
+-rw-r--r--   0 root         (0) root         (0)     3277 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py
+-rw-r--r--   0 root         (0) root         (0)     3782 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py
+-rw-r--r--   0 root         (0) root         (0)     4360 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py
+-rw-r--r--   0 root         (0) root         (0)     2781 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py
+-rw-r--r--   0 root         (0) root         (0)     1219 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py
+-rw-r--r--   0 root         (0) root         (0)     2206 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py
+-rw-r--r--   0 root         (0) root         (0)     2837 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py
+-rw-r--r--   0 root         (0) root         (0)     3882 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py
+-rw-r--r--   0 root         (0) root         (0)     3997 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2817 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)     7527 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py
+-rw-r--r--   0 root         (0) root         (0)     3592 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py
+-rw-r--r--   0 root         (0) root         (0)     2777 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/4df2c5ddabc0_remove_temporary_dids.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py
+-rw-r--r--   0 root         (0) root         (0)     2363 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py
+-rw-r--r--   0 root         (0) root         (0)     6101 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py
+-rw-r--r--   0 root         (0) root         (0)     5023 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py
+-rw-r--r--   0 root         (0) root         (0)     3568 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py
+-rw-r--r--   0 root         (0) root         (0)     1715 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3118 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py
+-rw-r--r--   0 root         (0) root         (0)     5038 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py
+-rw-r--r--   0 root         (0) root         (0)     3689 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py
+-rw-r--r--   0 root         (0) root         (0)     2614 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/a08fa8de1545_transfer_stats_table.py
+-rw-r--r--   0 root         (0) root         (0)     3117 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py
+-rw-r--r--   0 root         (0) root         (0)     5836 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     5407 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py
+-rw-r--r--   0 root         (0) root         (0)     7344 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py
+-rw-r--r--   0 root         (0) root         (0)     3704 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py
+-rw-r--r--   0 root         (0) root         (0)     2934 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py
+-rw-r--r--   0 root         (0) root         (0)     2784 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py
+-rw-r--r--   0 root         (0) root         (0)     9561 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py
+-rw-r--r--   0 root         (0) root         (0)     4748 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1594 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py
+-rw-r--r--   0 root         (0) root         (0)     5263 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py
+-rw-r--r--   0 root         (0) root         (0)     4865 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py
+-rw-r--r--   0 root         (0) root         (0)      897 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py
+-rw-r--r--   0 root         (0) root         (0)     2947 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py
+-rw-r--r--   0 root         (0) root         (0)     1949 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py
+-rw-r--r--   0 root         (0) root         (0)   112134 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/db/sqla/models.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/sautils.py
+-rw-r--r--   0 root         (0) root         (0)    17773 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/session.py
+-rw-r--r--   0 root         (0) root         (0)     6088 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/types.py
+-rw-r--r--   0 root         (0) root         (0)    22230 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/db/sqla/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.980405 rucio-34.4.1/lib/rucio/rse/
+-rw-r--r--   0 root         (0) root         (0)     3303 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.983405 rucio-34.4.1/lib/rucio/rse/protocols/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7199 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/bittorrent.py
+-rw-r--r--   0 root         (0) root         (0)     4603 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/dummy.py
+-rw-r--r--   0 root         (0) root         (0)    29100 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/gfal.py
+-rw-r--r--   0 root         (0) root         (0)     9730 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/globus.py
+-rw-r--r--   0 root         (0) root         (0)     3411 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/gsiftp.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/http_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/mock.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/ngarc.py
+-rw-r--r--   0 root         (0) root         (0)    10414 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/posix.py
+-rw-r--r--   0 root         (0) root         (0)    23933 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/protocol.py
+-rw-r--r--   0 root         (0) root         (0)    15260 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/rclone.py
+-rw-r--r--   0 root         (0) root         (0)     5501 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/rfio.py
+-rw-r--r--   0 root         (0) root         (0)    14689 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/srm.py
+-rw-r--r--   0 root         (0) root         (0)    17473 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     8141 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/storm.py
+-rw-r--r--   0 root         (0) root         (0)    22448 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/webdav.py
+-rw-r--r--   0 root         (0) root         (0)    12571 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/protocols/xrootd.py
+-rw-r--r--   0 root         (0) root         (0)    37647 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/rse/rsemanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.984405 rucio-34.4.1/lib/rucio/tests/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8907 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     5045 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/tests/common_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.985405 rucio-34.4.1/lib/rucio/transfertool/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/transfertool/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8342 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/transfertool/bittorrent.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/transfertool/bittorrent_driver.py
+-rw-r--r--   0 root         (0) root         (0)     4966 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/transfertool/bittorrent_driver_qbittorrent.py
+-rw-r--r--   0 root         (0) root         (0)    72157 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/transfertool/fts3.py
+-rw-r--r--   0 root         (0) root         (0)     6156 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/transfertool/fts3_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     7716 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/transfertool/globus.py
+-rw-r--r--   0 root         (0) root         (0)     8411 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/transfertool/globus_library.py
+-rw-r--r--   0 root         (0) root         (0)     2859 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/transfertool/mock.py
+-rw-r--r--   0 root         (0) root         (0)     7752 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/transfertool/transfertool.py
+-rw-r--r--   0 root         (0) root         (0)      244 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/vcsversion.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.986405 rucio-34.4.1/lib/rucio/web/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/web/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.986405 rucio-34.4.1/lib/rucio/web/rest/
+-rwxr-xr-x   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/web/rest/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.986405 rucio-34.4.1/lib/rucio/web/rest/flaskapi/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      999 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/authenticated_bp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.992405 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7791 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/accountlimits.py
+-rw-r--r--   0 root         (0) root         (0)    36983 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/accounts.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/archives.py
+-rw-r--r--   0 root         (0) root         (0)    61047 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/auth.py
+-rw-r--r--   0 root         (0) root         (0)    16148 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/common.py
+-rw-r--r--   0 root         (0) root         (0)    10143 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/config.py
+-rw-r--r--   0 root         (0) root         (0)     7714 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/credentials.py
+-rw-r--r--   0 root         (0) root         (0)    80867 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/dids.py
+-rw-r--r--   0 root         (0) root         (0)     4706 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/dirac.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/export.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/heartbeats.py
+-rw-r--r--   0 root         (0) root         (0)     7894 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/identities.py
+-rw-r--r--   0 root         (0) root         (0)     5259 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/import.py
+-rw-r--r--   0 root         (0) root         (0)    12009 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    12990 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/locks.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/main.py
+-rw-r--r--   0 root         (0) root         (0)     7785 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     3131 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/ping.py
+-rw-r--r--   0 root         (0) root         (0)    13331 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/redirect.py
+-rw-r--r--   0 root         (0) root         (0)    72711 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/replicas.py
+-rw-r--r--   0 root         (0) root         (0)    41622 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/requests.py
+-rw-r--r--   0 root         (0) root         (0)    81948 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/rses.py
+-rw-r--r--   0 root         (0) root         (0)    32189 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/rules.py
+-rw-r--r--   0 root         (0) root         (0)     5068 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/scopes.py
+-rw-r--r--   0 root         (0) root         (0)    24151 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:30.992405 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/templates/
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-07-27 12:40:37.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-07-27 12:40:37.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/traces.py
+-rw-r--r--   0 root         (0) root         (0)     9154 2024-05-24 11:15:54.000000 rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/vos.py
+-rw-r--r--   0 root         (0) root         (0)      725 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/web/rest/main.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/web/rest/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2024-05-23 08:12:33.000000 rucio-34.4.1/lib/rucio/web/rest/ping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:31.008405 rucio-34.4.1/lib/rucio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25876 2024-05-24 12:25:30.000000 rucio-34.4.1/lib/rucio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    16384 2024-05-06 09:19:47.000000 rucio-34.4.1/pylintrc
+-rw-r--r--   0 root         (0) root         (0)     5763 2024-05-24 12:25:23.000000 rucio-34.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     5235 2024-05-24 11:15:54.000000 rucio-34.4.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-24 12:25:31.015406 rucio-34.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2932 2024-05-24 12:25:27.000000 rucio-34.4.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2024-05-23 08:12:33.000000 rucio-34.4.1/setuputil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:31.008405 rucio-34.4.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_abacus_account.py
+-rw-r--r--   0 root         (0) root         (0)    10677 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_abacus_collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_abacus_rse.py
+-rw-r--r--   0 root         (0) root         (0)    15923 2024-05-24 11:15:54.000000 rucio-34.4.1/tests/test_account.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_account_limits.py
+-rw-r--r--   0 root         (0) root         (0)    20523 2024-05-24 11:15:54.000000 rucio-34.4.1/tests/test_api_external_representation.py
+-rw-r--r--   0 root         (0) root         (0)    13352 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_archive.py
+-rw-r--r--   0 root         (0) root         (0)     4074 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_auditor.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_auditor_hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_auditor_srmdumps.py
+-rw-r--r--   0 root         (0) root         (0)    14964 2024-05-24 11:15:54.000000 rucio-34.4.1/tests/test_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_automatix.py
+-rw-r--r--   0 root         (0) root         (0)    23265 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_bad_replica.py
+-rw-r--r--   0 root         (0) root         (0)    12425 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_bb8.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_belleii.py
+-rwxr-xr-x   0 root         (0) root         (0)   107450 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_bin_rucio.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_boolean.py
+-rw-r--r--   0 root         (0) root         (0)     8398 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_clients.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_common_types.py
+-rw-r--r--   0 root         (0) root         (0)     6942 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    96724 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_conveyor.py
+-rw-r--r--   0 root         (0) root         (0)    23870 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_conveyor_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_counter.py
+-rw-r--r--   0 root         (0) root         (0)     7728 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_credential.py
+-rw-r--r--   0 root         (0) root         (0)     7337 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_curl.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_daemons.py
+-rw-r--r--   0 root         (0) root         (0)    28183 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_dataset_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_db.py
+-rw-r--r--   0 root         (0) root         (0)    58823 2024-05-24 11:15:54.000000 rucio-34.4.1/tests/test_did.py
+-rw-r--r--   0 root         (0) root         (0)    29517 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_did_meta_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     4185 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_didtype.py
+-rw-r--r--   0 root         (0) root         (0)    35315 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     7118 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_dumper.py
+-rw-r--r--   0 root         (0) root         (0)    16419 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_dumper_consistency.py
+-rw-r--r--   0 root         (0) root         (0)    10869 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_dumper_data_model.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_dumper_path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    38301 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    10106 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_hermes.py
+-rw-r--r--   0 root         (0) root         (0)     5821 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)    18584 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_impl_upload_download.py
+-rw-r--r--   0 root         (0) root         (0)    57290 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_import_export.py
+-rw-r--r--   0 root         (0) root         (0)     5258 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_judge_cleaner.py
+-rw-r--r--   0 root         (0) root         (0)    22277 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_judge_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_judge_injector.py
+-rw-r--r--   0 root         (0) root         (0)    20429 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_judge_repairer.py
+-rw-r--r--   0 root         (0) root         (0)    12180 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_lifetime.py
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_meta_did.py
+-rw-r--r--   0 root         (0) root         (0)      957 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_module_import.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    54332 2024-05-24 11:15:54.000000 rucio-34.4.1/tests/test_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)    11582 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_oauthmanager.py
+-rw-r--r--   0 root         (0) root         (0)   108359 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-05-24 11:15:54.000000 rucio-34.4.1/tests/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_pfns.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_ping.py
+-rw-r--r--   0 root         (0) root         (0)     7662 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_qos.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    27487 2024-05-24 11:15:54.000000 rucio-34.4.1/tests/test_reaper.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_redirect.py
+-rw-r--r--   0 root         (0) root         (0)    62467 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_replica.py
+-rw-r--r--   0 root         (0) root         (0)    42098 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_replica_recoverer.py
+-rw-r--r--   0 root         (0) root         (0)    22796 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_replica_sorting.py
+-rw-r--r--   0 root         (0) root         (0)    17257 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_request.py
+-rw-r--r--   0 root         (0) root         (0)    13033 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_root_proxy.py
+-rw-r--r--   0 root         (0) root         (0)    75080 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_rse.py
+-rw-r--r--   0 root         (0) root         (0)    13184 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)     8940 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_rse_lfn2path.py
+-rw-r--r--   0 root         (0) root         (0)     4277 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_rse_protocol_gfal2.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_rse_protocol_gfal2_impl.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_rse_protocol_posix.py
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_rse_protocol_rclone.py
+-rw-r--r--   0 root         (0) root         (0)     4799 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_rse_protocol_rsync.py
+-rw-r--r--   0 root         (0) root         (0)     3979 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_rse_protocol_srm.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_rse_protocol_ssh.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_rse_protocol_webdav.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_rse_protocol_xrootd.py
+-rw-r--r--   0 root         (0) root         (0)     7746 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)      867 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)    91949 2024-05-24 11:15:54.000000 rucio-34.4.1/tests/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)     7486 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_scope.py
+-rw-r--r--   0 root         (0) root         (0)    48389 2024-05-24 11:15:54.000000 rucio-34.4.1/tests/test_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    55587 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_throttler.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_tpc.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)    25254 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     8924 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_transfer_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8412 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_undertaker.py
+-rw-r--r--   0 root         (0) root         (0)    16778 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2024-05-23 08:12:33.000000 rucio-34.4.1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:25:31.008405 rucio-34.4.1/tools/
+-rwxr-xr-x   0 root         (0) root         (0)     1259 2024-05-23 08:12:33.000000 rucio-34.4.1/tools/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     6163 2024-05-23 08:12:33.000000 rucio-34.4.1/tools/merge_rucio_configs.py
+-rwxr-xr-x   0 root         (0) root         (0)     1351 2024-05-23 08:12:33.000000 rucio-34.4.1/tools/reset_database.py
```

### Comparing `rucio-34.4.0/AUTHORS.rst` & `rucio-34.4.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/LICENSE` & `rucio-34.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/MANIFEST.in` & `rucio-34.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/PKG-INFO` & `rucio-34.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rucio
-Version: 34.4.0
+Version: 34.4.1
 Summary: Rucio Package
 Home-page: https://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Environment :: No Input/Output (Daemon)
 Requires-Python: >=3.9, <4
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: requests<=2.31.0,>=2.25.1
+Requires-Dist: requests~=2.32.0
 Requires-Dist: urllib3~=1.26.18
 Requires-Dist: dogpile.cache~=1.2.2
 Requires-Dist: tabulate~=0.9.0
 Requires-Dist: jsonschema~=4.20.0
 Requires-Dist: paramiko~=3.4.0
 Requires-Dist: argcomplete~=3.1.6
 Requires-Dist: python-magic~=0.4.27
```

### Comparing `rucio-34.4.0/README.rst` & `rucio-34.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio` & `rucio-34.4.1/bin/rucio`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-abacus-account` & `rucio-34.4.1/bin/rucio-abacus-account`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-abacus-collection-replica` & `rucio-34.4.1/bin/rucio-abacus-collection-replica`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-abacus-rse` & `rucio-34.4.1/bin/rucio-abacus-rse`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-admin` & `rucio-34.4.1/bin/rucio-admin`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-atropos` & `rucio-34.4.1/bin/rucio-atropos`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-auditor` & `rucio-34.4.1/bin/rucio-auditor`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-automatix` & `rucio-34.4.1/bin/rucio-automatix`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-bb8` & `rucio-34.4.1/bin/rucio-bb8`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-c3po` & `rucio-34.4.1/bin/rucio-c3po`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-cache-client` & `rucio-34.4.1/bin/rucio-cache-client`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-cache-consumer` & `rucio-34.4.1/bin/rucio-cache-consumer`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-conveyor-finisher` & `rucio-34.4.1/bin/rucio-conveyor-finisher`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-conveyor-poller` & `rucio-34.4.1/bin/rucio-conveyor-poller`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-conveyor-preparer` & `rucio-34.4.1/bin/rucio-conveyor-preparer`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-conveyor-receiver` & `rucio-34.4.1/bin/rucio-conveyor-receiver`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-conveyor-stager` & `rucio-34.4.1/bin/rucio-conveyor-stager`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-conveyor-submitter` & `rucio-34.4.1/bin/rucio-conveyor-submitter`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-conveyor-throttler` & `rucio-34.4.1/bin/rucio-conveyor-throttler`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-dark-reaper` & `rucio-34.4.1/bin/rucio-dark-reaper`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-dumper` & `rucio-34.4.1/bin/rucio-dumper`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-follower` & `rucio-34.4.1/bin/rucio-follower`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-hermes` & `rucio-34.4.1/bin/rucio-hermes`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-judge-cleaner` & `rucio-34.4.1/bin/rucio-judge-cleaner`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-judge-evaluator` & `rucio-34.4.1/bin/rucio-judge-evaluator`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-judge-injector` & `rucio-34.4.1/bin/rucio-judge-injector`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-judge-repairer` & `rucio-34.4.1/bin/rucio-judge-repairer`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-kronos` & `rucio-34.4.1/bin/rucio-kronos`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-minos` & `rucio-34.4.1/bin/rucio-minos`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-minos-temporary-expiration` & `rucio-34.4.1/bin/rucio-minos-temporary-expiration`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-necromancer` & `rucio-34.4.1/bin/rucio-necromancer`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-oauth-manager` & `rucio-34.4.1/bin/rucio-oauth-manager`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-reaper` & `rucio-34.4.1/bin/rucio-reaper`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-replica-recoverer` & `rucio-34.4.1/bin/rucio-replica-recoverer`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-rse-decommissioner` & `rucio-34.4.1/bin/rucio-rse-decommissioner`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-storage-consistency-actions` & `rucio-34.4.1/bin/rucio-storage-consistency-actions`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-transmogrifier` & `rucio-34.4.1/bin/rucio-transmogrifier`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/bin/rucio-undertaker` & `rucio-34.4.1/bin/rucio-undertaker`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/etc/alembic.ini.template` & `rucio-34.4.1/etc/alembic.ini.template`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/etc/alembic_offline.ini.template` & `rucio-34.4.1/etc/alembic_offline.ini.template`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/etc/ldap.cfg.template` & `rucio-34.4.1/etc/ldap.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/etc/mail_templates/rule_approval_request.tmpl` & `rucio-34.4.1/etc/mail_templates/rule_approval_request.tmpl`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/etc/mail_templates/rule_ok_notification.tmpl` & `rucio-34.4.1/etc/mail_templates/rule_ok_notification.tmpl`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/etc/rse-accounts.cfg.template` & `rucio-34.4.1/etc/rse-accounts.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/etc/rucio.cfg.atlas.client.template` & `rucio-34.4.1/etc/rucio.cfg.atlas.client.template`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/etc/rucio.cfg.template` & `rucio-34.4.1/etc/rucio.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/etc/rucio_multi_vo.cfg.template` & `rucio-34.4.1/etc/rucio_multi_vo.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/__init__.py` & `rucio-34.4.1/lib/rucio/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/alembicrevision.py` & `rucio-34.4.1/lib/rucio/alembicrevision.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/__init__.py` & `rucio-34.4.1/lib/rucio/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/account.py` & `rucio-34.4.1/lib/rucio/api/account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/account_limit.py` & `rucio-34.4.1/lib/rucio/api/account_limit.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/authentication.py` & `rucio-34.4.1/lib/rucio/api/authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/config.py` & `rucio-34.4.1/lib/rucio/api/config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/credential.py` & `rucio-34.4.1/lib/rucio/api/credential.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/did.py` & `rucio-34.4.1/lib/rucio/api/did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/dirac.py` & `rucio-34.4.1/lib/rucio/api/dirac.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/exporter.py` & `rucio-34.4.1/lib/rucio/api/exporter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/heartbeat.py` & `rucio-34.4.1/lib/rucio/api/heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/identity.py` & `rucio-34.4.1/lib/rucio/api/identity.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/importer.py` & `rucio-34.4.1/lib/rucio/api/importer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/lifetime_exception.py` & `rucio-34.4.1/lib/rucio/api/lifetime_exception.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/lock.py` & `rucio-34.4.1/lib/rucio/api/lock.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/meta_conventions.py` & `rucio-34.4.1/lib/rucio/api/meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/permission.py` & `rucio-34.4.1/lib/rucio/api/permission.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/quarantined_replica.py` & `rucio-34.4.1/lib/rucio/api/quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/replica.py` & `rucio-34.4.1/lib/rucio/api/replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/request.py` & `rucio-34.4.1/lib/rucio/api/request.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/rse.py` & `rucio-34.4.1/lib/rucio/api/rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/rule.py` & `rucio-34.4.1/lib/rucio/api/rule.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/scope.py` & `rucio-34.4.1/lib/rucio/api/scope.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/subscription.py` & `rucio-34.4.1/lib/rucio/api/subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/api/vo.py` & `rucio-34.4.1/lib/rucio/api/vo.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/__init__.py` & `rucio-34.4.1/lib/rucio/client/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/accountclient.py` & `rucio-34.4.1/lib/rucio/client/accountclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/accountlimitclient.py` & `rucio-34.4.1/lib/rucio/client/accountlimitclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/baseclient.py` & `rucio-34.4.1/lib/rucio/client/baseclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/client.py` & `rucio-34.4.1/lib/rucio/client/client.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/configclient.py` & `rucio-34.4.1/lib/rucio/client/configclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/credentialclient.py` & `rucio-34.4.1/lib/rucio/client/credentialclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/didclient.py` & `rucio-34.4.1/lib/rucio/client/didclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/diracclient.py` & `rucio-34.4.1/lib/rucio/client/diracclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/downloadclient.py` & `rucio-34.4.1/lib/rucio/client/downloadclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/exportclient.py` & `rucio-34.4.1/lib/rucio/client/exportclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/fileclient.py` & `rucio-34.4.1/lib/rucio/client/fileclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/importclient.py` & `rucio-34.4.1/lib/rucio/client/importclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/lifetimeclient.py` & `rucio-34.4.1/lib/rucio/client/lifetimeclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/lockclient.py` & `rucio-34.4.1/lib/rucio/client/lockclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/metaconventionsclient.py` & `rucio-34.4.1/lib/rucio/client/metaconventionsclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/pingclient.py` & `rucio-34.4.1/lib/rucio/client/pingclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/replicaclient.py` & `rucio-34.4.1/lib/rucio/client/replicaclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/requestclient.py` & `rucio-34.4.1/lib/rucio/client/requestclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/rseclient.py` & `rucio-34.4.1/lib/rucio/client/rseclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/ruleclient.py` & `rucio-34.4.1/lib/rucio/client/ruleclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/scopeclient.py` & `rucio-34.4.1/lib/rucio/client/scopeclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/subscriptionclient.py` & `rucio-34.4.1/lib/rucio/client/subscriptionclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/touchclient.py` & `rucio-34.4.1/lib/rucio/client/touchclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/client/uploadclient.py` & `rucio-34.4.1/lib/rucio/client/uploadclient.py`

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

### Comparing `rucio-34.4.0/lib/rucio/common/__init__.py` & `rucio-34.4.1/lib/rucio/common/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/cache.py` & `rucio-34.4.1/lib/rucio/common/cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/config.py` & `rucio-34.4.1/lib/rucio/common/config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/constants.py` & `rucio-34.4.1/lib/rucio/common/constants.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/constraints.py` & `rucio-34.4.1/lib/rucio/common/constraints.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/didtype.py` & `rucio-34.4.1/lib/rucio/common/didtype.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/dumper/__init__.py` & `rucio-34.4.1/lib/rucio/common/dumper/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/dumper/consistency.py` & `rucio-34.4.1/lib/rucio/common/dumper/consistency.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/dumper/data_models.py` & `rucio-34.4.1/lib/rucio/common/dumper/data_models.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/dumper/path_parsing.py` & `rucio-34.4.1/lib/rucio/common/dumper/path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/exception.py` & `rucio-34.4.1/lib/rucio/common/exception.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/extra.py` & `rucio-34.4.1/lib/rucio/common/extra.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/logging.py` & `rucio-34.4.1/lib/rucio/common/logging.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/pcache.py` & `rucio-34.4.1/lib/rucio/common/pcache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/plugins.py` & `rucio-34.4.1/lib/rucio/common/plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/policy.py` & `rucio-34.4.1/lib/rucio/common/policy.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/schema/__init__.py` & `rucio-34.4.1/lib/rucio/common/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/schema/atlas.py` & `rucio-34.4.1/lib/rucio/common/schema/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/schema/belleii.py` & `rucio-34.4.1/lib/rucio/common/schema/belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/schema/domatpc.py` & `rucio-34.4.1/lib/rucio/common/schema/domatpc.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/schema/escape.py` & `rucio-34.4.1/lib/rucio/common/schema/escape.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/schema/generic.py` & `rucio-34.4.1/lib/rucio/common/schema/generic.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/schema/generic_multi_vo.py` & `rucio-34.4.1/lib/rucio/common/schema/generic_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/schema/icecube.py` & `rucio-34.4.1/lib/rucio/common/schema/icecube.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/stomp_utils.py` & `rucio-34.4.1/lib/rucio/common/stomp_utils.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/stopwatch.py` & `rucio-34.4.1/lib/rucio/common/stopwatch.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/test_rucio_server.py` & `rucio-34.4.1/lib/rucio/common/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/types.py` & `rucio-34.4.1/lib/rucio/common/types.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/common/utils.py` & `rucio-34.4.1/lib/rucio/common/utils.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/__init__.py` & `rucio-34.4.1/lib/rucio/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/account.py` & `rucio-34.4.1/lib/rucio/core/account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/account_counter.py` & `rucio-34.4.1/lib/rucio/core/account_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/account_limit.py` & `rucio-34.4.1/lib/rucio/core/account_limit.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/authentication.py` & `rucio-34.4.1/lib/rucio/core/authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/config.py` & `rucio-34.4.1/lib/rucio/core/config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/credential.py` & `rucio-34.4.1/lib/rucio/core/credential.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/did.py` & `rucio-34.4.1/lib/rucio/core/did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/did_meta_plugins/__init__.py` & `rucio-34.4.1/lib/rucio/core/did_meta_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/did_meta_plugins/did_column_meta.py` & `rucio-34.4.1/lib/rucio/core/did_meta_plugins/did_column_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py` & `rucio-34.4.1/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/did_meta_plugins/filter_engine.py` & `rucio-34.4.1/lib/rucio/core/did_meta_plugins/filter_engine.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/did_meta_plugins/json_meta.py` & `rucio-34.4.1/lib/rucio/core/did_meta_plugins/json_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/did_meta_plugins/mongo_meta.py` & `rucio-34.4.1/lib/rucio/core/did_meta_plugins/mongo_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/did_meta_plugins/postgres_meta.py` & `rucio-34.4.1/lib/rucio/core/did_meta_plugins/postgres_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/dirac.py` & `rucio-34.4.1/lib/rucio/core/dirac.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/distance.py` & `rucio-34.4.1/lib/rucio/core/distance.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/exporter.py` & `rucio-34.4.1/lib/rucio/core/exporter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/heartbeat.py` & `rucio-34.4.1/lib/rucio/core/heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/identity.py` & `rucio-34.4.1/lib/rucio/core/identity.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/importer.py` & `rucio-34.4.1/lib/rucio/core/importer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/lifetime_exception.py` & `rucio-34.4.1/lib/rucio/core/lifetime_exception.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/lock.py` & `rucio-34.4.1/lib/rucio/core/lock.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/message.py` & `rucio-34.4.1/lib/rucio/core/message.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/meta_conventions.py` & `rucio-34.4.1/lib/rucio/core/meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/monitor.py` & `rucio-34.4.1/lib/rucio/core/monitor.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/naming_convention.py` & `rucio-34.4.1/lib/rucio/core/naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/nongrid_trace.py` & `rucio-34.4.1/lib/rucio/core/nongrid_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/oidc.py` & `rucio-34.4.1/lib/rucio/core/oidc.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/permission/__init__.py` & `rucio-34.4.1/lib/rucio/core/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/permission/atlas.py` & `rucio-34.4.1/lib/rucio/core/permission/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/permission/belleii.py` & `rucio-34.4.1/lib/rucio/core/permission/belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/permission/escape.py` & `rucio-34.4.1/lib/rucio/core/permission/escape.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/permission/generic.py` & `rucio-34.4.1/lib/rucio/core/permission/generic.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/permission/generic_multi_vo.py` & `rucio-34.4.1/lib/rucio/core/permission/generic_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/quarantined_replica.py` & `rucio-34.4.1/lib/rucio/core/quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/replica.py` & `rucio-34.4.1/lib/rucio/core/replica.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,28 +264,19 @@
     path_pfn_dict = {}
 
     if len(pfns) > 0 and type(pfns[0]) is str:
         # If pfns is a list of PFNs, the scope and names need to be extracted from the path
         rse_info = rsemgr.get_rse_info(rse_id=rse_id, session=session)
         proto = rsemgr.create_protocol(rse_info, 'read', scheme=scheme)
         if rse_info['deterministic']:
-            # TBD : In case of deterministic RSE, call the extract_scope_from_path method
+            scope_proto = rsemgr.get_scope_protocol(vo=issuer.vo)
             parsed_pfn = proto.parse_pfns(pfns=pfns)
             for pfn in parsed_pfn:
-                # WARNING : this part is ATLAS specific and must be changed
-                path = parsed_pfn[pfn]['path']
-                if path.startswith('/user') or path.startswith('/group'):
-                    scope = '%s.%s' % (path.split('/')[1], path.split('/')[2])
-                    name = parsed_pfn[pfn]['name']
-                elif path.startswith('/'):
-                    scope = path.split('/')[1]
-                    name = parsed_pfn[pfn]['name']
-                else:
-                    scope = path.split('/')[0]
-                    name = parsed_pfn[pfn]['name']
+                # Translate into a scope and name
+                name, scope = scope_proto(parsed_pfn[pfn])
 
                 scope = InternalScope(scope, vo=issuer.vo)
                 replicas.append({'scope': scope, 'name': name, 'rse_id': rse_id, 'state': status})
                 path = '%s%s' % (parsed_pfn[pfn]['path'], parsed_pfn[pfn]['name'])
                 path_pfn_dict[path] = pfn
 
         else:
@@ -596,28 +587,20 @@
         dict_rse[rse_id] = pfns
     for rse_id in dict_rse:
         pfns = dict_rse[rse_id]
         rse_info = rsemgr.get_rse_info(rse_id=rse_id, session=session)
         pfndict = {}
         proto = rsemgr.create_protocol(rse_info, 'read', scheme=scheme)
         if rse_info['deterministic']:
+            scope_proto = rsemgr.get_scope_protocol(vo=vo)
             parsed_pfn = proto.parse_pfns(pfns=pfns)
 
-            # WARNING : this part is ATLAS specific and must be changed
             for pfn in parsed_pfn:
-                path = parsed_pfn[pfn]['path']
-                if path.startswith('/user') or path.startswith('/group'):
-                    scope = '%s.%s' % (path.split('/')[1], path.split('/')[2])
-                    name = parsed_pfn[pfn]['name']
-                elif path.startswith('/'):
-                    scope = path.split('/')[1]
-                    name = parsed_pfn[pfn]['name']
-                else:
-                    scope = path.split('/')[0]
-                    name = parsed_pfn[pfn]['name']
+                # Translate into a scope and name
+                name, scope = scope_proto(parsed_pfn[pfn])
                 scope = InternalScope(scope, vo)
                 yield {pfn: {'scope': scope, 'name': name}}
         else:
             condition = []
             parsed_pfn = proto.parse_pfns(pfns=pfns)
             for pfn in parsed_pfn:
                 path = '%s%s' % (parsed_pfn[pfn]['path'], parsed_pfn[pfn]['name'])
```

### Comparing `rucio-34.4.0/lib/rucio/core/replica_sorter.py` & `rucio-34.4.1/lib/rucio/core/replica_sorter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/request.py` & `rucio-34.4.1/lib/rucio/core/request.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/rse.py` & `rucio-34.4.1/lib/rucio/core/rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/rse_counter.py` & `rucio-34.4.1/lib/rucio/core/rse_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/rse_expression_parser.py` & `rucio-34.4.1/lib/rucio/core/rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/rse_selector.py` & `rucio-34.4.1/lib/rucio/core/rse_selector.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/rule.py` & `rucio-34.4.1/lib/rucio/core/rule.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/rule_grouping.py` & `rucio-34.4.1/lib/rucio/core/rule_grouping.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/scope.py` & `rucio-34.4.1/lib/rucio/core/scope.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/subscription.py` & `rucio-34.4.1/lib/rucio/core/subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/topology.py` & `rucio-34.4.1/lib/rucio/core/topology.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/trace.py` & `rucio-34.4.1/lib/rucio/core/trace.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/transfer.py` & `rucio-34.4.1/lib/rucio/core/transfer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/vo.py` & `rucio-34.4.1/lib/rucio/core/vo.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/core/volatile_replica.py` & `rucio-34.4.1/lib/rucio/core/volatile_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/abacus/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/abacus/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/abacus/account.py` & `rucio-34.4.1/lib/rucio/daemons/abacus/account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/abacus/collection_replica.py` & `rucio-34.4.1/lib/rucio/daemons/abacus/collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/abacus/rse.py` & `rucio-34.4.1/lib/rucio/daemons/abacus/rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/atropos/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/atropos/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/atropos/atropos.py` & `rucio-34.4.1/lib/rucio/daemons/atropos/atropos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/auditor/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/auditor/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/auditor/hdfs.py` & `rucio-34.4.1/lib/rucio/daemons/auditor/hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/auditor/srmdumps.py` & `rucio-34.4.1/lib/rucio/daemons/auditor/srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/automatix/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/automatix/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/automatix/automatix.py` & `rucio-34.4.1/lib/rucio/daemons/automatix/automatix.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/badreplicas/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/badreplicas/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/badreplicas/minos.py` & `rucio-34.4.1/lib/rucio/daemons/badreplicas/minos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py` & `rucio-34.4.1/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/badreplicas/necromancer.py` & `rucio-34.4.1/lib/rucio/daemons/badreplicas/necromancer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/bb8/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/bb8/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/bb8/bb8.py` & `rucio-34.4.1/lib/rucio/daemons/bb8/bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/bb8/common.py` & `rucio-34.4.1/lib/rucio/daemons/bb8/common.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/bb8/nuclei_background_rebalance.py` & `rucio-34.4.1/lib/rucio/daemons/bb8/nuclei_background_rebalance.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/bb8/t2_background_rebalance.py` & `rucio-34.4.1/lib/rucio/daemons/bb8/t2_background_rebalance.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/simple.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/algorithms/simple.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/t2_free_space.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/algorithms/t2_free_space.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/c3po.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/c3po.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/collectors/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/collectors/agis.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/collectors/agis.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/collectors/free_space.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/collectors/free_space.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/collectors/jedi_did.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/collectors/jedi_did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/collectors/mock_did.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/collectors/mock_did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/collectors/network_metrics.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/collectors/network_metrics.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/collectors/workload.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/collectors/workload.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/utils/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/utils/dataset_cache.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/utils/dataset_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/utils/expiring_list.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/utils/expiring_list.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/utils/popularity.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/utils/popularity.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/c3po/utils/timeseries.py` & `rucio-34.4.1/lib/rucio/daemons/c3po/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/cache/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/cache/consumer.py` & `rucio-34.4.1/lib/rucio/daemons/cache/consumer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/common.py` & `rucio-34.4.1/lib/rucio/daemons/common.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/conveyor/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/conveyor/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/conveyor/common.py` & `rucio-34.4.1/lib/rucio/daemons/conveyor/common.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/conveyor/finisher.py` & `rucio-34.4.1/lib/rucio/daemons/conveyor/finisher.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/conveyor/poller.py` & `rucio-34.4.1/lib/rucio/daemons/conveyor/poller.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/conveyor/preparer.py` & `rucio-34.4.1/lib/rucio/daemons/conveyor/preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/conveyor/receiver.py` & `rucio-34.4.1/lib/rucio/daemons/conveyor/receiver.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/conveyor/stager.py` & `rucio-34.4.1/lib/rucio/daemons/conveyor/stager.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/conveyor/submitter.py` & `rucio-34.4.1/lib/rucio/daemons/conveyor/submitter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/conveyor/throttler.py` & `rucio-34.4.1/lib/rucio/daemons/conveyor/throttler.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/follower/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/follower/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/follower/follower.py` & `rucio-34.4.1/lib/rucio/daemons/follower/follower.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/hermes/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/hermes/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/hermes/hermes.py` & `rucio-34.4.1/lib/rucio/daemons/hermes/hermes.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/judge/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/judge/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/judge/cleaner.py` & `rucio-34.4.1/lib/rucio/daemons/judge/cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/judge/evaluator.py` & `rucio-34.4.1/lib/rucio/daemons/judge/evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/judge/injector.py` & `rucio-34.4.1/lib/rucio/daemons/judge/injector.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/judge/repairer.py` & `rucio-34.4.1/lib/rucio/daemons/judge/repairer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/oauthmanager/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/oauthmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/oauthmanager/oauthmanager.py` & `rucio-34.4.1/lib/rucio/daemons/oauthmanager/oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/reaper/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/reaper/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/reaper/dark_reaper.py` & `rucio-34.4.1/lib/rucio/daemons/reaper/dark_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/reaper/reaper.py` & `rucio-34.4.1/lib/rucio/daemons/reaper/reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/replicarecoverer/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/replicarecoverer/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py` & `rucio-34.4.1/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/rsedecommissioner/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/config.py` & `rucio-34.4.1/lib/rucio/daemons/rsedecommissioner/config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/rsedecommissioner/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/atlas.py` & `rucio-34.4.1/lib/rucio/daemons/rsedecommissioner/profiles/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/generic.py` & `rucio-34.4.1/lib/rucio/daemons/rsedecommissioner/profiles/generic.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/types.py` & `rucio-34.4.1/lib/rucio/daemons/rsedecommissioner/profiles/types.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/rse_decommissioner.py` & `rucio-34.4.1/lib/rucio/daemons/rsedecommissioner/rse_decommissioner.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/storage/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/storage/consistency/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/storage/consistency/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/storage/consistency/actions.py` & `rucio-34.4.1/lib/rucio/daemons/storage/consistency/actions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/tracer/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/tracer/kronos.py` & `rucio-34.4.1/lib/rucio/daemons/tracer/kronos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/transmogrifier/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/transmogrifier/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/transmogrifier/transmogrifier.py` & `rucio-34.4.1/lib/rucio/daemons/transmogrifier/transmogrifier.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/undertaker/__init__.py` & `rucio-34.4.1/lib/rucio/daemons/undertaker/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/daemons/undertaker/undertaker.py` & `rucio-34.4.1/lib/rucio/daemons/undertaker/undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/__init__.py` & `rucio-34.4.1/lib/rucio/db/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/__init__.py` & `rucio-34.4.1/lib/rucio/db/sqla/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/constants.py` & `rucio-34.4.1/lib/rucio/db/sqla/constants.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/__init__.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/env.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/env.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4df2c5ddabc0_remove_temporary_dids.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/4df2c5ddabc0_remove_temporary_dids.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a08fa8de1545_transfer_stats_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/a08fa8de1545_transfer_stats_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py` & `rucio-34.4.1/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/models.py` & `rucio-34.4.1/lib/rucio/db/sqla/models.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/sautils.py` & `rucio-34.4.1/lib/rucio/db/sqla/sautils.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/session.py` & `rucio-34.4.1/lib/rucio/db/sqla/session.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/types.py` & `rucio-34.4.1/lib/rucio/db/sqla/types.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/db/sqla/util.py` & `rucio-34.4.1/lib/rucio/db/sqla/util.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/__init__.py` & `rucio-34.4.1/lib/rucio/rse/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/__init__.py` & `rucio-34.4.1/lib/rucio/rse/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/bittorrent.py` & `rucio-34.4.1/lib/rucio/rse/protocols/bittorrent.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/cache.py` & `rucio-34.4.1/lib/rucio/rse/protocols/cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/dummy.py` & `rucio-34.4.1/lib/rucio/rse/protocols/dummy.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/gfal.py` & `rucio-34.4.1/lib/rucio/rse/protocols/gfal.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/globus.py` & `rucio-34.4.1/lib/rucio/rse/protocols/globus.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/gsiftp.py` & `rucio-34.4.1/lib/rucio/rse/protocols/gsiftp.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/http_cache.py` & `rucio-34.4.1/lib/rucio/rse/protocols/http_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/mock.py` & `rucio-34.4.1/lib/rucio/rse/protocols/mock.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/ngarc.py` & `rucio-34.4.1/lib/rucio/rse/protocols/ngarc.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/posix.py` & `rucio-34.4.1/lib/rucio/rse/protocols/posix.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/protocol.py` & `rucio-34.4.1/lib/rucio/rse/protocols/protocol.py`

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

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/rclone.py` & `rucio-34.4.1/lib/rucio/rse/protocols/rclone.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/rfio.py` & `rucio-34.4.1/lib/rucio/rse/protocols/rfio.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/srm.py` & `rucio-34.4.1/lib/rucio/rse/protocols/srm.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/ssh.py` & `rucio-34.4.1/lib/rucio/rse/protocols/ssh.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/storm.py` & `rucio-34.4.1/lib/rucio/rse/protocols/storm.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/webdav.py` & `rucio-34.4.1/lib/rucio/rse/protocols/webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/protocols/xrootd.py` & `rucio-34.4.1/lib/rucio/rse/protocols/xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/rse/rsemanager.py` & `rucio-34.4.1/lib/rucio/rse/rsemanager.py`

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

### Comparing `rucio-34.4.0/lib/rucio/tests/__init__.py` & `rucio-34.4.1/lib/rucio/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/tests/common.py` & `rucio-34.4.1/lib/rucio/tests/common.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/tests/common_server.py` & `rucio-34.4.1/lib/rucio/tests/common_server.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/transfertool/__init__.py` & `rucio-34.4.1/lib/rucio/transfertool/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/transfertool/bittorrent.py` & `rucio-34.4.1/lib/rucio/transfertool/bittorrent.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/transfertool/bittorrent_driver.py` & `rucio-34.4.1/lib/rucio/transfertool/bittorrent_driver.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/transfertool/bittorrent_driver_qbittorrent.py` & `rucio-34.4.1/lib/rucio/transfertool/bittorrent_driver_qbittorrent.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/transfertool/fts3.py` & `rucio-34.4.1/lib/rucio/transfertool/fts3.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/transfertool/fts3_plugins.py` & `rucio-34.4.1/lib/rucio/transfertool/fts3_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/transfertool/globus.py` & `rucio-34.4.1/lib/rucio/transfertool/globus.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/transfertool/globus_library.py` & `rucio-34.4.1/lib/rucio/transfertool/globus_library.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/transfertool/mock.py` & `rucio-34.4.1/lib/rucio/transfertool/mock.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/transfertool/transfertool.py` & `rucio-34.4.1/lib/rucio/transfertool/transfertool.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/version.py` & `rucio-34.4.1/lib/rucio/version.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/__init__.py` & `rucio-34.4.1/lib/rucio/web/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/__init__.py` & `rucio-34.4.1/lib/rucio/web/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/__init__.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/authenticated_bp.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/authenticated_bp.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/__init__.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/accountlimits.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/accountlimits.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/accounts.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/accounts.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/archives.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/archives.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/auth.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/auth.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/common.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/common.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/config.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/credentials.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/credentials.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/dids.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/dids.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/dirac.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/dirac.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/export.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/export.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/heartbeats.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/heartbeats.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/identities.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/identities.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/import.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/import.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/locks.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/locks.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/main.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/main.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/meta_conventions.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/metrics.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/metrics.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/ping.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/ping.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/redirect.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/replicas.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/requests.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/rses.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/rses.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/rules.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/scopes.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/scopes.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/subscriptions.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/subscriptions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/traces.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/traces.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/vos.py` & `rucio-34.4.1/lib/rucio/web/rest/flaskapi/v1/vos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/main.py` & `rucio-34.4.1/lib/rucio/web/rest/main.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/metrics.py` & `rucio-34.4.1/lib/rucio/web/rest/metrics.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio/web/rest/ping.py` & `rucio-34.4.1/lib/rucio/web/rest/ping.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/lib/rucio.egg-info/SOURCES.txt` & `rucio-34.4.1/lib/rucio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/pylintrc` & `rucio-34.4.1/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/pyproject.toml` & `rucio-34.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/requirements.txt` & `rucio-34.4.1/requirements.txt`

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

### Comparing `rucio-34.4.0/setup.py` & `rucio-34.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/setuputil.py` & `rucio-34.4.1/setuputil.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_abacus_account.py` & `rucio-34.4.1/tests/test_abacus_account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_abacus_collection_replica.py` & `rucio-34.4.1/tests/test_abacus_collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_abacus_rse.py` & `rucio-34.4.1/tests/test_abacus_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_account.py` & `rucio-34.4.1/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_account_limits.py` & `rucio-34.4.1/tests/test_account_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_api_external_representation.py` & `rucio-34.4.1/tests/test_api_external_representation.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_archive.py` & `rucio-34.4.1/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_auditor.py` & `rucio-34.4.1/tests/test_auditor.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_auditor_hdfs.py` & `rucio-34.4.1/tests/test_auditor_hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_auditor_srmdumps.py` & `rucio-34.4.1/tests/test_auditor_srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_authentication.py` & `rucio-34.4.1/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_automatix.py` & `rucio-34.4.1/tests/test_automatix.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_bad_replica.py` & `rucio-34.4.1/tests/test_bad_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_bb8.py` & `rucio-34.4.1/tests/test_bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_belleii.py` & `rucio-34.4.1/tests/test_belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_bin_rucio.py` & `rucio-34.4.1/tests/test_bin_rucio.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_boolean.py` & `rucio-34.4.1/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_clients.py` & `rucio-34.4.1/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_common_types.py` & `rucio-34.4.1/tests/test_common_types.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_config.py` & `rucio-34.4.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_conveyor.py` & `rucio-34.4.1/tests/test_conveyor.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_conveyor_submitter.py` & `rucio-34.4.1/tests/test_conveyor_submitter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_counter.py` & `rucio-34.4.1/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_credential.py` & `rucio-34.4.1/tests/test_credential.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_curl.py` & `rucio-34.4.1/tests/test_curl.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_daemons.py` & `rucio-34.4.1/tests/test_daemons.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_dataset_replicas.py` & `rucio-34.4.1/tests/test_dataset_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_db.py` & `rucio-34.4.1/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_did.py` & `rucio-34.4.1/tests/test_did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_did_meta_plugins.py` & `rucio-34.4.1/tests/test_did_meta_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_didtype.py` & `rucio-34.4.1/tests/test_didtype.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_download.py` & `rucio-34.4.1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_dumper.py` & `rucio-34.4.1/tests/test_dumper.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_dumper_consistency.py` & `rucio-34.4.1/tests/test_dumper_consistency.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_dumper_data_model.py` & `rucio-34.4.1/tests/test_dumper_data_model.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_dumper_path_parsing.py` & `rucio-34.4.1/tests/test_dumper_path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_filter_engine.py` & `rucio-34.4.1/tests/test_filter_engine.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_heartbeat.py` & `rucio-34.4.1/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_hermes.py` & `rucio-34.4.1/tests/test_hermes.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_identity.py` & `rucio-34.4.1/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_impl_upload_download.py` & `rucio-34.4.1/tests/test_impl_upload_download.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_import_export.py` & `rucio-34.4.1/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_judge_cleaner.py` & `rucio-34.4.1/tests/test_judge_cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_judge_evaluator.py` & `rucio-34.4.1/tests/test_judge_evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_judge_injector.py` & `rucio-34.4.1/tests/test_judge_injector.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_judge_repairer.py` & `rucio-34.4.1/tests/test_judge_repairer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_lifetime.py` & `rucio-34.4.1/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_message.py` & `rucio-34.4.1/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_meta_conventions.py` & `rucio-34.4.1/tests/test_meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_meta_did.py` & `rucio-34.4.1/tests/test_meta_did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_module_import.py` & `rucio-34.4.1/tests/test_module_import.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_monitor.py` & `rucio-34.4.1/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_multi_vo.py` & `rucio-34.4.1/tests/test_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_naming_convention.py` & `rucio-34.4.1/tests/test_naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_oauthmanager.py` & `rucio-34.4.1/tests/test_oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_oidc.py` & `rucio-34.4.1/tests/test_oidc.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_permission.py` & `rucio-34.4.1/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_pfns.py` & `rucio-34.4.1/tests/test_pfns.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_ping.py` & `rucio-34.4.1/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_preparer.py` & `rucio-34.4.1/tests/test_preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_qos.py` & `rucio-34.4.1/tests/test_qos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_quarantined_replica.py` & `rucio-34.4.1/tests/test_quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_reaper.py` & `rucio-34.4.1/tests/test_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_redirect.py` & `rucio-34.4.1/tests/test_redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_replica.py` & `rucio-34.4.1/tests/test_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_replica_recoverer.py` & `rucio-34.4.1/tests/test_replica_recoverer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_replica_sorting.py` & `rucio-34.4.1/tests/test_replica_sorting.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_request.py` & `rucio-34.4.1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_root_proxy.py` & `rucio-34.4.1/tests/test_root_proxy.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_rse.py` & `rucio-34.4.1/tests/test_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_rse_expression_parser.py` & `rucio-34.4.1/tests/test_rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_rse_lfn2path.py` & `rucio-34.4.1/tests/test_rse_lfn2path.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_rse_protocol_gfal2.py` & `rucio-34.4.1/tests/test_rse_protocol_gfal2.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_rse_protocol_gfal2_impl.py` & `rucio-34.4.1/tests/test_rse_protocol_gfal2_impl.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_rse_protocol_posix.py` & `rucio-34.4.1/tests/test_rse_protocol_posix.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_rse_protocol_rclone.py` & `rucio-34.4.1/tests/test_rse_protocol_rclone.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_rse_protocol_rsync.py` & `rucio-34.4.1/tests/test_rse_protocol_rsync.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_rse_protocol_srm.py` & `rucio-34.4.1/tests/test_rse_protocol_srm.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_rse_protocol_ssh.py` & `rucio-34.4.1/tests/test_rse_protocol_ssh.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_rse_protocol_webdav.py` & `rucio-34.4.1/tests/test_rse_protocol_webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_rse_protocol_xrootd.py` & `rucio-34.4.1/tests/test_rse_protocol_xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_rse_selector.py` & `rucio-34.4.1/tests/test_rse_selector.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_rucio_server.py` & `rucio-34.4.1/tests/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_rule.py` & `rucio-34.4.1/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_scope.py` & `rucio-34.4.1/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_subscription.py` & `rucio-34.4.1/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_throttler.py` & `rucio-34.4.1/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_tpc.py` & `rucio-34.4.1/tests/test_tpc.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_trace.py` & `rucio-34.4.1/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_transfer.py` & `rucio-34.4.1/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_transfer_plugins.py` & `rucio-34.4.1/tests/test_transfer_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_undertaker.py` & `rucio-34.4.1/tests/test_undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tests/test_upload.py` & `rucio-34.4.1/tests/test_upload.py`

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

### Comparing `rucio-34.4.0/tests/test_utils.py` & `rucio-34.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tools/bootstrap.py` & `rucio-34.4.1/tools/bootstrap.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tools/merge_rucio_configs.py` & `rucio-34.4.1/tools/merge_rucio_configs.py`

 * *Files identical despite different names*

### Comparing `rucio-34.4.0/tools/reset_database.py` & `rucio-34.4.1/tools/reset_database.py`

 * *Files identical despite different names*

