# Comparing `tmp/otpme-0.3.0a65.tar.gz` & `tmp/otpme-0.3.0a66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otpme-0.3.0a65.tar", last modified: Thu May 23 17:55:31 2024, max compression
+gzip compressed data, was "otpme-0.3.0a66.tar", last modified: Thu May 23 17:58:10 2024, max compression
```

## Comparing `otpme-0.3.0a65.tar` & `otpme-0.3.0a66.tar`

### file list

```diff
@@ -1,509 +1,509 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.401572 otpme-0.3.0a65/
--rw-r--r--   0 root         (0) root         (0)    35121 2024-05-23 17:55:31.000000 otpme-0.3.0a65/LICENSE
--rw-r--r--   0 root         (0) root         (0)      665 2024-05-23 17:55:31.000000 otpme-0.3.0a65/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      680 2024-05-23 17:55:31.401572 otpme-0.3.0a65/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3821 2024-05-23 17:55:31.000000 otpme-0.3.0a65/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.353571 otpme-0.3.0a65/bash_completion/
--rw-r--r--   0 root         (0) root         (0)     1937 2024-05-23 17:55:31.000000 otpme-0.3.0a65/bash_completion/otpme
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.353571 otpme-0.3.0a65/deploy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.357571 otpme-0.3.0a65/deploy/dicts/
--rw-r--r--   0 root         (0) root         (0)     2535 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/dicts/abbreviations-it.gz
--rw-r--r--   0 root         (0) root         (0)    18683 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/dicts/at-surnames.gz
--rw-r--r--   0 root         (0) root         (0)   197269 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/dicts/common-passwords.gz
--rwxr-xr-x   0 root         (0) root         (0)      532 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/dicts/convert_dict.sh
--rw-r--r--   0 root         (0) root         (0)     3286 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/dicts/de-female.gz
--rw-r--r--   0 root         (0) root         (0)     3070 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/dicts/de-male.gz
--rw-r--r--   0 root         (0) root         (0)    11343 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/dicts/de-surnames.gz
--rw-r--r--   0 root         (0) root         (0)    34845 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/dicts/de-top10000.gz
--rw-r--r--   0 root         (0) root         (0)    30600 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/dicts/en-top10000.gz
--rw-r--r--   0 root         (0) root         (0)   127983 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/dicts/english-guessing.gz
--rw-r--r--   0 root         (0) root         (0)  1041710 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/dicts/english.gz
--rw-r--r--   0 root         (0) root         (0)   547291 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/dicts/german-guessing.gz
--rw-r--r--   0 root         (0) root         (0)   544600 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/dicts/german.gz
--rw-r--r--   0 root         (0) root         (0)    13539 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/dicts/us-female.gz
--rw-r--r--   0 root         (0) root         (0)     4089 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/dicts/us-male.gz
--rw-r--r--   0 root         (0) root         (0)    35682 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/dicts/us-surnames.gz
--rw-r--r--   0 root         (0) root         (0)    13331 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/otpme.conf.dist
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.357571 otpme-0.3.0a65/deploy/pam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.357571 otpme-0.3.0a65/deploy/pam/pam-python/
--rw-r--r--   0 root         (0) root         (0)      511 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/pam/pam-python/README
--rw-r--r--   0 root         (0) root         (0)     2436 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/pam/pam_otpme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.357571 otpme-0.3.0a65/deploy/radius/
--rw-r--r--   0 root         (0) root         (0)    13085 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/radius/dictionary
--rw-r--r--   0 root         (0) root         (0)     3851 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/radius/dictionary.freeradius
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.357571 otpme-0.3.0a65/deploy/schema/
--rw-r--r--   0 root         (0) root         (0)    21610 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/schema/core.schema
--rw-r--r--   0 root         (0) root         (0)    73993 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/schema/cosine.schema
--rw-r--r--   0 root         (0) root         (0)     6267 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/schema/inetorgperson.schema
--rw-r--r--   0 root         (0) root         (0)     7632 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/schema/nis.schema
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.357571 otpme-0.3.0a65/deploy/scripts/
--rw-r--r--   0 root         (0) root         (0)     8600 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/scripts/agent_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/scripts/auth_script.sh
--rw-r--r--   0 root         (0) root         (0)    21045 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/scripts/key_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/scripts/login_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/scripts/node_vote_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 17:55:31.000000 otpme-0.3.0a65/deploy/scripts/push_script.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.361571 otpme-0.3.0a65/otpme/
--rw-r--r--   0 root         (0) root         (0)     1535 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    12650 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.365571 otpme-0.3.0a65/otpme/lib/
--rw-r--r--   0 root         (0) root         (0)    10420 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1970 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/arp.py
--rw-r--r--   0 root         (0) root         (0)     3502 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/auth_script.py
--rw-r--r--   0 root         (0) root         (0)    48043 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.365571 otpme-0.3.0a65/otpme/lib/backends/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/backends/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.365571 otpme-0.3.0a65/otpme/lib/backends/file/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/backends/file/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90185 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/backends/file/file.py
--rw-r--r--   0 root         (0) root         (0)    12946 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/backends/file/index.py
--rw-r--r--   0 root         (0) root         (0)     5831 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/backends/file/models.py
--rw-r--r--   0 root         (0) root         (0)    67194 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/backends/file/transaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.365571 otpme-0.3.0a65/otpme/lib/cache/
--rw-r--r--   0 root         (0) root         (0)    27567 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3159 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cache/dogpile.py
--rw-r--r--   0 root         (0) root         (0)    19444 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cache/funccache.py
--rw-r--r--   0 root         (0) root         (0)     3448 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cache/lru.py
--rw-r--r--   0 root         (0) root         (0)    14349 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cache/memcache.py
--rw-r--r--   0 root         (0) root         (0)     6433 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cache/memcached.py
--rw-r--r--   0 root         (0) root         (0)     7277 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cache/memcachedb.py
--rw-r--r--   0 root         (0) root         (0)    27128 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cache/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.369571 otpme-0.3.0a65/otpme/lib/classes/
--rw-r--r--   0 root         (0) root         (0)      890 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86180 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/accessgroup.py
--rw-r--r--   0 root         (0) root         (0)    14807 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/agent_conn.py
--rw-r--r--   0 root         (0) root         (0)   126036 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/auth_handler.py
--rw-r--r--   0 root         (0) root         (0)    56607 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/ca.py
--rw-r--r--   0 root         (0) root         (0)    40741 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/client.py
--rw-r--r--   0 root         (0) root         (0)   230501 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/command_handler.py
--rw-r--r--   0 root         (0) root         (0)     8663 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/conn_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.373571 otpme-0.3.0a65/otpme/lib/classes/data_objects/
--rw-r--r--   0 root         (0) root         (0)      813 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/data_objects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2319 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/data_objects/cert.py
--rw-r--r--   0 root         (0) root         (0)     6798 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/data_objects/data_revision.py
--rw-r--r--   0 root         (0) root         (0)     6813 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/data_objects/failed_pass.py
--rw-r--r--   0 root         (0) root         (0)     8058 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/data_objects/last_assigned_id.py
--rw-r--r--   0 root         (0) root         (0)    10512 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/data_objects/revoked_signature.py
--rw-r--r--   0 root         (0) root         (0)     2503 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/data_objects/rsa_key.py
--rw-r--r--   0 root         (0) root         (0)     6953 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/data_objects/skip_sync.py
--rw-r--r--   0 root         (0) root         (0)     5744 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/data_objects/token_counter.py
--rw-r--r--   0 root         (0) root         (0)     5579 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/data_objects/used_hash.py
--rw-r--r--   0 root         (0) root         (0)     5922 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/data_objects/used_otp.py
--rw-r--r--   0 root         (0) root         (0)     5930 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/data_objects/used_slp.py
--rw-r--r--   0 root         (0) root         (0)     5925 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/data_objects/used_sotp.py
--rw-r--r--   0 root         (0) root         (0)    28615 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/dictionary.py
--rw-r--r--   0 root         (0) root         (0)    39118 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/group.py
--rw-r--r--   0 root         (0) root         (0)    51998 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/host.py
--rw-r--r--   0 root         (0) root         (0)    12229 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/login_handler.py
--rw-r--r--   0 root         (0) root         (0)     5303 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/mgmt_client.py
--rw-r--r--   0 root         (0) root         (0)    38791 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/node.py
--rw-r--r--   0 root         (0) root         (0)    24374 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/object_config.py
--rw-r--r--   0 root         (0) root         (0)    77062 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/otpme_agent.py
--rw-r--r--   0 root         (0) root         (0)    49637 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/otpme_host.py
--rw-r--r--   0 root         (0) root         (0)   318795 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/otpme_object.py
--rw-r--r--   0 root         (0) root         (0)    23290 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/policy.py
--rw-r--r--   0 root         (0) root         (0)    62426 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/realm.py
--rw-r--r--   0 root         (0) root         (0)    74411 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/resolver.py
--rw-r--r--   0 root         (0) root         (0)    45000 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/role.py
--rw-r--r--   0 root         (0) root         (0)    34173 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/script.py
--rw-r--r--   0 root         (0) root         (0)    52920 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/session.py
--rw-r--r--   0 root         (0) root         (0)    31418 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/signing.py
--rw-r--r--   0 root         (0) root         (0)   107184 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/site.py
--rw-r--r--   0 root         (0) root         (0)     6987 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/ssh_agent.py
--rw-r--r--   0 root         (0) root         (0)   134850 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/token.py
--rw-r--r--   0 root         (0) root         (0)    49395 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/unit.py
--rw-r--r--   0 root         (0) root         (0)   182171 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/classes/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.373571 otpme-0.3.0a65/otpme/lib/cli/
--rw-r--r--   0 root         (0) root         (0)    64574 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12885 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/accessgroup.py
--rw-r--r--   0 root         (0) root         (0)     7119 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/ca.py
--rw-r--r--   0 root         (0) root         (0)    13242 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/client.py
--rw-r--r--   0 root         (0) root         (0)     5643 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/dictionary.py
--rw-r--r--   0 root         (0) root         (0)    12993 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/group.py
--rw-r--r--   0 root         (0) root         (0)    13057 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/host.py
--rw-r--r--   0 root         (0) root         (0)    10974 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/node.py
--rw-r--r--   0 root         (0) root         (0)     6165 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/policy.py
--rw-r--r--   0 root         (0) root         (0)     6174 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/realm.py
--rw-r--r--   0 root         (0) root         (0)     6600 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/resolver.py
--rw-r--r--   0 root         (0) root         (0)    20248 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/role.py
--rw-r--r--   0 root         (0) root         (0)     7383 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/script.py
--rw-r--r--   0 root         (0) root         (0)     7524 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/site.py
--rw-r--r--   0 root         (0) root         (0)    17354 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/token.py
--rw-r--r--   0 root         (0) root         (0)     5423 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/unit.py
--rw-r--r--   0 root         (0) root         (0)     7596 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/cli/user.py
--rw-r--r--   0 root         (0) root         (0)    24867 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/compgen.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.373571 otpme-0.3.0a65/otpme/lib/compression/
--rw-r--r--   0 root         (0) root         (0)      447 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/compression/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4082 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/compression/base.py
--rw-r--r--   0 root         (0) root         (0)    14277 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/connections.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.377571 otpme-0.3.0a65/otpme/lib/daemon/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3785 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/daemon/authd.py
--rw-r--r--   0 root         (0) root         (0)   108965 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/daemon/clusterd.py
--rw-r--r--   0 root         (0) root         (0)    47551 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/daemon/controld.py
--rw-r--r--   0 root         (0) root         (0)    76763 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/daemon/hostd.py
--rw-r--r--   0 root         (0) root         (0)     3074 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/daemon/joind.py
--rw-r--r--   0 root         (0) root         (0)     6713 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/daemon/ldapd.py
--rw-r--r--   0 root         (0) root         (0)     3003 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/daemon/mgmtd.py
--rw-r--r--   0 root         (0) root         (0)    15876 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/daemon/otpme_daemon.py
--rw-r--r--   0 root         (0) root         (0)    11391 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/daemon/scriptd.py
--rw-r--r--   0 root         (0) root         (0)     3017 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/daemon/syncd.py
--rw-r--r--   0 root         (0) root         (0)     6941 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/daemon/unix_daemon.py
--rw-r--r--   0 root         (0) root         (0)    19005 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/debug.py
--rw-r--r--   0 root         (0) root         (0)     2090 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/doc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.377571 otpme-0.3.0a65/otpme/lib/encoding/
--rw-r--r--   0 root         (0) root         (0)      429 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/encoding/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/encoding/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.377571 otpme-0.3.0a65/otpme/lib/encryption/
--rw-r--r--   0 root         (0) root         (0)     3953 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/encryption/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3296 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/encryption/aes.py
--rw-r--r--   0 root         (0) root         (0)     1479 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/encryption/aes_cfb.py
--rw-r--r--   0 root         (0) root         (0)     7900 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/encryption/argon2.py
--rw-r--r--   0 root         (0) root         (0)    10240 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/encryption/asymmetric_key_handler.py
--rw-r--r--   0 root         (0) root         (0)     4251 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/encryption/ec.py
--rw-r--r--   0 root         (0) root         (0)     2912 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/encryption/fernet.py
--rw-r--r--   0 root         (0) root         (0)     3237 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/encryption/hkdf.py
--rw-r--r--   0 root         (0) root         (0)     3727 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/encryption/pbkdf2.py
--rw-r--r--   0 root         (0) root         (0)     7824 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/encryption/rsa.py
--rw-r--r--   0 root         (0) root         (0)     4324 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.377571 otpme-0.3.0a65/otpme/lib/extensions/
--rw-r--r--   0 root         (0) root         (0)      329 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/extensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.377571 otpme-0.3.0a65/otpme/lib/extensions/base/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/extensions/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12278 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/extensions/base/base.py
--rw-r--r--   0 root         (0) root         (0)    40152 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/extensions/ldif_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.377571 otpme-0.3.0a65/otpme/lib/extensions/posix/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/extensions/posix/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14286 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/extensions/posix/posix.py
--rw-r--r--   0 root         (0) root         (0)     3640 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/extensions/utils.py
--rw-r--r--   0 root         (0) root         (0)    34081 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/filetools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.377571 otpme-0.3.0a65/otpme/lib/freeradius/
--rw-r--r--   0 root         (0) root         (0)     9119 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/freeradius/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18685 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/freeradius/otpme.py
--rw-r--r--   0 root         (0) root         (0)     1297 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/freeradius/radiusd.py
--rw-r--r--   0 root         (0) root         (0)     1203 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/freeradius/radiusd_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.377571 otpme-0.3.0a65/otpme/lib/gpg/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/gpg/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    28498 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/gpg/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.381571 otpme-0.3.0a65/otpme/lib/help/
--rwxr-xr-x   0 root         (0) root         (0)    26529 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22986 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/accessgroup.py
--rw-r--r--   0 root         (0) root         (0)     5485 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/agent.py
--rw-r--r--   0 root         (0) root         (0)     1857 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/auth.py
--rw-r--r--   0 root         (0) root         (0)    15707 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/ca.py
--rw-r--r--   0 root         (0) root         (0)    16924 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/client.py
--rw-r--r--   0 root         (0) root         (0)     1568 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/cluster.py
--rw-r--r--   0 root         (0) root         (0)     5785 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/controld.py
--rw-r--r--   0 root         (0) root         (0)    11388 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/dictionary.py
--rw-r--r--   0 root         (0) root         (0)      522 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/get_authorized_keys.py
--rw-r--r--   0 root         (0) root         (0)    19872 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/group.py
--rw-r--r--   0 root         (0) root         (0)    24436 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/host.py
--rw-r--r--   0 root         (0) root         (0)    21309 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/node.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/pinentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.381571 otpme-0.3.0a65/otpme/lib/help/policy/
--rw-r--r--   0 root         (0) root         (0)     8739 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/policy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3710 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/policy/authonaction.py
--rw-r--r--   0 root         (0) root         (0)     1247 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/policy/autodisable.py
--rw-r--r--   0 root         (0) root         (0)     1751 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/policy/defaultgroups.py
--rw-r--r--   0 root         (0) root         (0)     1559 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/policy/defaultpolicies.py
--rw-r--r--   0 root         (0) root         (0)     1421 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/policy/defaultroles.py
--rw-r--r--   0 root         (0) root         (0)     1836 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/policy/defaultunits.py
--rw-r--r--   0 root         (0) root         (0)     1492 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/policy/forcetoken.py
--rw-r--r--   0 root         (0) root         (0)     2230 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/policy/idrange.py
--rw-r--r--   0 root         (0) root         (0)     3225 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/policy/logintimes.py
--rw-r--r--   0 root         (0) root         (0)     1098 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/policy/objecttemplates.py
--rw-r--r--   0 root         (0) root         (0)     2918 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/policy/password.py
--rw-r--r--   0 root         (0) root         (0)     2779 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/policy/tokenacls.py
--rw-r--r--   0 root         (0) root         (0)    20037 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/realm.py
--rw-r--r--   0 root         (0) root         (0)     1441 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/register.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.381571 otpme-0.3.0a65/otpme/lib/help/resolver/
--rw-r--r--   0 root         (0) root         (0)    12522 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4465 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/resolver/ldap.py
--rw-r--r--   0 root         (0) root         (0)    18198 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/role.py
--rw-r--r--   0 root         (0) root         (0)    15111 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/script.py
--rw-r--r--   0 root         (0) root         (0)     2844 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/session.py
--rw-r--r--   0 root         (0) root         (0)    22488 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.381571 otpme-0.3.0a65/otpme/lib/help/token/
--rw-r--r--   0 root         (0) root         (0)    20503 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/token/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1385 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/token/fido2.py
--rw-r--r--   0 root         (0) root         (0)     5619 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/token/hotp.py
--rw-r--r--   0 root         (0) root         (0)     6339 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/token/motp.py
--rw-r--r--   0 root         (0) root         (0)     1991 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/token/otp_push.py
--rw-r--r--   0 root         (0) root         (0)     4951 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/token/otpme.py
--rw-r--r--   0 root         (0) root         (0)     3880 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/token/password.py
--rw-r--r--   0 root         (0) root         (0)     7251 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/token/ssh.py
--rw-r--r--   0 root         (0) root         (0)     5977 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/token/totp.py
--rw-r--r--   0 root         (0) root         (0)     5803 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/token/yubikey_hmac.py
--rw-r--r--   0 root         (0) root         (0)     1252 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/token/yubikey_hotp.py
--rw-r--r--   0 root         (0) root         (0)    24935 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/tool.py
--rw-r--r--   0 root         (0) root         (0)    15168 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/unit.py
--rw-r--r--   0 root         (0) root         (0)    29409 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/help/user.py
--rw-r--r--   0 root         (0) root         (0)    16341 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/host.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.385572 otpme-0.3.0a65/otpme/lib/humanize/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/humanize/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4191 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/humanize/units.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.385572 otpme-0.3.0a65/otpme/lib/index/
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23948 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/index/mysql.py
--rw-r--r--   0 root         (0) root         (0)    24542 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/index/postgres.py
--rw-r--r--   0 root         (0) root         (0)     8336 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/index/sqlite3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.385572 otpme-0.3.0a65/otpme/lib/job/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20681 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/job/callback.py
--rw-r--r--   0 root         (0) root         (0)    12849 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/job/otpme_job.py
--rw-r--r--   0 root         (0) root         (0)    37097 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/join.py
--rw-r--r--   0 root         (0) root         (0)     4857 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/json.py
--rw-r--r--   0 root         (0) root         (0)     1942 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/jwt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.385572 otpme-0.3.0a65/otpme/lib/ldap/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/ldap/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1354 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/ldap/client.py
--rw-r--r--   0 root         (0) root         (0)    11062 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/ldap/schema.py
--rw-r--r--   0 root         (0) root         (0)    50483 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/ldap/server.py
--rw-r--r--   0 root         (0) root         (0)    19709 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/locking.py
--rw-r--r--   0 root         (0) root         (0)     9430 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/log.py
--rw-r--r--   0 root         (0) root         (0)     1529 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/messages.py
--rw-r--r--   0 root         (0) root         (0)     5981 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/mschap.py
--rw-r--r--   0 root         (0) root         (0)     2366 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/mschap_util.py
--rw-r--r--   0 root         (0) root         (0)    35744 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/multiprocessing.py
--rw-r--r--   0 root         (0) root         (0)    10250 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/net.py
--rw-r--r--   0 root         (0) root         (0)    27144 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/nsscache.py
--rw-r--r--   0 root         (0) root         (0)    63328 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/offline_token.py
--rw-r--r--   0 root         (0) root         (0)    23778 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/oid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.385572 otpme-0.3.0a65/otpme/lib/otp/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/otp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.385572 otpme-0.3.0a65/otpme/lib/otp/oath/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/otp/oath/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1727 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/otp/oath/hotp.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/otp/oath/totp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.385572 otpme-0.3.0a65/otpme/lib/otp/otpme/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/otp/otpme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3087 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/otp/otpme/otpme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.385572 otpme-0.3.0a65/otpme/lib/otp/yubico/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/otp/yubico/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3026 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/otp/yubico/yubiotp.py
--rw-r--r--   0 root         (0) root         (0)    19837 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/otpme_acl.py
--rw-r--r--   0 root         (0) root         (0)   115772 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/otpme_config.py
--rw-r--r--   0 root         (0) root         (0)     3519 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/otpme_pass.py
--rw-r--r--   0 root         (0) root         (0)    70359 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/pam.py
--rw-r--r--   0 root         (0) root         (0)     1975 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/pickle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.385572 otpme-0.3.0a65/otpme/lib/pinentry/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/pinentry/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27465 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/pinentry/pinentry.py
--rwxr-xr-x   0 root         (0) root         (0)     7880 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/pinentry/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.385572 otpme-0.3.0a65/otpme/lib/pki/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/pki/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9797 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/pki/cert.py
--rw-r--r--   0 root         (0) root         (0)    23150 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/pki/utils.py
--rw-r--r--   0 root         (0) root         (0)    16890 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/pki/utils_openssl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.385572 otpme-0.3.0a65/otpme/lib/policy/
--rw-r--r--   0 root         (0) root         (0)     2099 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.385572 otpme-0.3.0a65/otpme/lib/policy/authonaction/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/authonaction/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32663 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/authonaction/authonaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.385572 otpme-0.3.0a65/otpme/lib/policy/autodisable/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/autodisable/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15718 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/autodisable/autodisable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.385572 otpme-0.3.0a65/otpme/lib/policy/defaultgroups/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/defaultgroups/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17570 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/defaultgroups/defaultgroups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.385572 otpme-0.3.0a65/otpme/lib/policy/defaultpolicies/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/defaultpolicies/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14510 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/defaultpolicies/defaultpolicies.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.389572 otpme-0.3.0a65/otpme/lib/policy/defaultroles/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/defaultroles/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14217 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/defaultroles/defaultroles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.389572 otpme-0.3.0a65/otpme/lib/policy/defaultunits/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/defaultunits/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15637 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/defaultunits/defaultunits.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.389572 otpme-0.3.0a65/otpme/lib/policy/forcetoken/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/forcetoken/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14202 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/forcetoken/forcetoken.py
--rw-r--r--   0 root         (0) root         (0)     1176 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/get_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.389572 otpme-0.3.0a65/otpme/lib/policy/idrange/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/idrange/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27256 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/idrange/idrange.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.389572 otpme-0.3.0a65/otpme/lib/policy/logintimes/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/logintimes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23017 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/logintimes/logintimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.389572 otpme-0.3.0a65/otpme/lib/policy/objecttemplates/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/objecttemplates/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14954 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/objecttemplates/objecttemplates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.389572 otpme-0.3.0a65/otpme/lib/policy/password/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/password/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28981 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/password/password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.389572 otpme-0.3.0a65/otpme/lib/policy/tokenacls/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/tokenacls/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24897 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/tokenacls/tokenacls.py
--rw-r--r--   0 root         (0) root         (0)      491 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/policy/utils.py
--rw-r--r--   0 root         (0) root         (0)     9332 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/preload.py
--rw-r--r--   0 root         (0) root         (0)     2466 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.389572 otpme-0.3.0a65/otpme/lib/protocols/
--rw-r--r--   0 root         (0) root         (0)      304 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.389572 otpme-0.3.0a65/otpme/lib/protocols/client/
--rw-r--r--   0 root         (0) root         (0)      655 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1887 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/client/agent1.py
--rw-r--r--   0 root         (0) root         (0)      832 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/client/auth1.py
--rw-r--r--   0 root         (0) root         (0)    14301 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/client/cluster1.py
--rw-r--r--   0 root         (0) root         (0)     1046 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/client/get_class.py
--rw-r--r--   0 root         (0) root         (0)     4645 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/client/host1.py
--rw-r--r--   0 root         (0) root         (0)      832 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/client/join1.py
--rwxr-xr-x   0 root         (0) root         (0)    11305 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/client/mgmt1.py
--rw-r--r--   0 root         (0) root         (0)    67975 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/client/sync1.py
--rw-r--r--   0 root         (0) root         (0)   160693 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/otpme_client.py
--rw-r--r--   0 root         (0) root         (0)    81420 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/otpme_server.py
--rw-r--r--   0 root         (0) root         (0)     1601 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/request.py
--rw-r--r--   0 root         (0) root         (0)     1770 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.393572 otpme-0.3.0a65/otpme/lib/protocols/server/
--rw-r--r--   0 root         (0) root         (0)      827 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40219 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/server/agent1.py
--rw-r--r--   0 root         (0) root         (0)    12842 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/server/auth1.py
--rw-r--r--   0 root         (0) root         (0)    32302 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/server/cluster1.py
--rw-r--r--   0 root         (0) root         (0)     1912 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/server/get_class.py
--rw-r--r--   0 root         (0) root         (0)    26608 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/server/host1.py
--rw-r--r--   0 root         (0) root         (0)    52562 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/server/join1.py
--rw-r--r--   0 root         (0) root         (0)    70866 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/server/mgmt1.py
--rw-r--r--   0 root         (0) root         (0)    45433 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/server/sync1.py
--rw-r--r--   0 root         (0) root         (0)      527 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/status_codes.py
--rw-r--r--   0 root         (0) root         (0)     6937 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/protocols/utils.py
--rw-r--r--   0 root         (0) root         (0)     2157 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/push_script.py
--rw-r--r--   0 root         (0) root         (0)     1139 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/qrcode.py
--rw-r--r--   0 root         (0) root         (0)      478 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/re.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.393572 otpme-0.3.0a65/otpme/lib/register/
--rw-r--r--   0 root         (0) root         (0)     9716 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/register/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.393572 otpme-0.3.0a65/otpme/lib/resolver/
--rw-r--r--   0 root         (0) root         (0)      485 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1158 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/resolver/get_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.393572 otpme-0.3.0a65/otpme/lib/resolver/ldap/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/resolver/ldap/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39438 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/resolver/ldap/ldap.py
--rw-r--r--   0 root         (0) root         (0)      451 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/resolver/utils.py
--rw-r--r--   0 root         (0) root         (0)    10019 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/script.py
--rw-r--r--   0 root         (0) root         (0)     3005 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/sign_key_cache.py
--rw-r--r--   0 root         (0) root         (0)      537 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/slp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.393572 otpme-0.3.0a65/otpme/lib/smartcard/
--rw-r--r--   0 root         (0) root         (0)      623 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/smartcard/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.393572 otpme-0.3.0a65/otpme/lib/smartcard/fido2/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/smartcard/fido2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10161 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/smartcard/fido2/fido2.py
--rw-r--r--   0 root         (0) root         (0)      858 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/smartcard/get_class.py
--rw-r--r--   0 root         (0) root         (0)     1666 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/smartcard/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.393572 otpme-0.3.0a65/otpme/lib/smartcard/yubikey/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/smartcard/yubikey/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11951 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/smartcard/yubikey/deploy.py
--rw-r--r--   0 root         (0) root         (0)     1982 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/smartcard/yubikey/usb.py
--rw-r--r--   0 root         (0) root         (0)     8075 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/smartcard/yubikey/yubikey.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.393572 otpme-0.3.0a65/otpme/lib/smartcard/yubikey_gpg/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/smartcard/yubikey_gpg/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6364 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.393572 otpme-0.3.0a65/otpme/lib/smartcard/yubikey_hmac/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/smartcard/yubikey_hmac/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11955 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.393572 otpme-0.3.0a65/otpme/lib/smartcard/yubikey_hotp/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/smartcard/yubikey_hotp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5032 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.393572 otpme-0.3.0a65/otpme/lib/socket/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/socket/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13152 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/socket/connect.py
--rw-r--r--   0 root         (0) root         (0)     8450 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/socket/handler.py
--rw-r--r--   0 root         (0) root         (0)    30962 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/socket/listen.py
--rw-r--r--   0 root         (0) root         (0)     2830 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/socket/send_recv1.py
--rw-r--r--   0 root         (0) root         (0)     4408 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/sotp.py
--rwxr-xr-x   0 root         (0) root         (0)    37113 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/spsc.py
--rw-r--r--   0 root         (0) root         (0)      544 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/srp.py
--rw-r--r--   0 root         (0) root         (0)    23454 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/ssh.py
--rw-r--r--   0 root         (0) root         (0)    63673 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/stuff.py
--rw-r--r--   0 root         (0) root         (0)    12338 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/sync_cache.py
--rw-r--r--   0 root         (0) root         (0)     4636 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/system_command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.393572 otpme-0.3.0a65/otpme/lib/third_party/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.397572 otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/
--rw-r--r--   0 root         (0) root         (0)     1981 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/advanced.py
--rw-r--r--   0 root         (0) root         (0)     9859 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/caching_query.py
--rw-r--r--   0 root         (0) root         (0)     2250 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/environment.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/fixture_data.py
--rw-r--r--   0 root         (0) root         (0)     2248 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/helloworld.py
--rw-r--r--   0 root         (0) root         (0)     3310 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/local_session_caching.py
--rw-r--r--   0 root         (0) root         (0)     3033 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/model.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/relationship_caching.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.397572 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/
--rw-r--r--   0 root         (0) root         (0)     1140 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.397572 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/caches/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/caches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9083 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/caches/caches.py
--rw-r--r--   0 root         (0) root         (0)    14341 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/caches/files.py
--rw-r--r--   0 root         (0) root         (0)     1044 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/config.py
--rw-r--r--   0 root         (0) root         (0)     1959 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/error.py
--rw-r--r--   0 root         (0) root         (0)     7963 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.397572 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/maps/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/maps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2389 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/maps/group.py
--rw-r--r--   0 root         (0) root         (0)    11745 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/maps/maps.py
--rw-r--r--   0 root         (0) root         (0)     2554 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/maps/passwd.py
--rw-r--r--   0 root         (0) root         (0)     2387 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/maps/shadow.py
--rw-r--r--   0 root         (0) root         (0)     4140 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/nss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.397572 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/update/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/update/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5487 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/update/files_updater.py
--rw-r--r--   0 root         (0) root         (0)     5826 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/update/map_updater.py
--rw-r--r--   0 root         (0) root         (0)    10980 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/update/updater.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.397572 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/util/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4117 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/nss_cache/util/file_formats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.397572 otpme-0.3.0a65/otpme/lib/third_party/oath_toolkit/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/oath_toolkit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1592 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/oath_toolkit/_compat.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/third_party/oath_toolkit/uri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.397572 otpme-0.3.0a65/otpme/lib/token/
--rw-r--r--   0 root         (0) root         (0)      953 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.397572 otpme-0.3.0a65/otpme/lib/token/fido2/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/fido2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14939 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/fido2/fido2.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/get_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.397572 otpme-0.3.0a65/otpme/lib/token/hotp/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/hotp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39346 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/hotp/hotp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.397572 otpme-0.3.0a65/otpme/lib/token/link/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/link/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9656 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/link/link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.397572 otpme-0.3.0a65/otpme/lib/token/motp/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/motp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27770 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/motp/motp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.397572 otpme-0.3.0a65/otpme/lib/token/oath/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/oath/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19667 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/oath/oath.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.397572 otpme-0.3.0a65/otpme/lib/token/otp_push/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/otp_push/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23393 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/otp_push/otp_push.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.401572 otpme-0.3.0a65/otpme/lib/token/otpme/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/otpme/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24704 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/otpme/otpme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.401572 otpme-0.3.0a65/otpme/lib/token/password/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/password/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26068 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/password/password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.401572 otpme-0.3.0a65/otpme/lib/token/script_otp/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/script_otp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9677 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/script_otp/script_otp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.401572 otpme-0.3.0a65/otpme/lib/token/script_static/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/script_static/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9677 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/script_static/script_static.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.401572 otpme-0.3.0a65/otpme/lib/token/ssh/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/ssh/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39547 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/ssh/ssh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.401572 otpme-0.3.0a65/otpme/lib/token/totp/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/totp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35398 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/totp/totp.py
--rw-r--r--   0 root         (0) root         (0)      480 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.401572 otpme-0.3.0a65/otpme/lib/token/yubikey_hmac/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/yubikey_hmac/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25111 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme/lib/token/yubikey_hmac/yubikey_hmac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:55:31.361571 otpme-0.3.0a65/otpme.egg-info/
--rw-r--r--   0 root         (0) root         (0)      680 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13359 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1080 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      973 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-23 17:55:31.000000 otpme-0.3.0a65/otpme.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 17:55:31.401572 otpme-0.3.0a65/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8833 2024-05-23 17:55:31.000000 otpme-0.3.0a65/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.776894 otpme-0.3.0a66/
+-rw-r--r--   0 root         (0) root         (0)    35121 2024-05-23 17:58:10.000000 otpme-0.3.0a66/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      665 2024-05-23 17:58:10.000000 otpme-0.3.0a66/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      680 2024-05-23 17:58:10.776894 otpme-0.3.0a66/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3821 2024-05-23 17:58:10.000000 otpme-0.3.0a66/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.728893 otpme-0.3.0a66/bash_completion/
+-rw-r--r--   0 root         (0) root         (0)     1937 2024-05-23 17:58:10.000000 otpme-0.3.0a66/bash_completion/otpme
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.728893 otpme-0.3.0a66/deploy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.732893 otpme-0.3.0a66/deploy/dicts/
+-rw-r--r--   0 root         (0) root         (0)     2535 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/dicts/abbreviations-it.gz
+-rw-r--r--   0 root         (0) root         (0)    18683 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/dicts/at-surnames.gz
+-rw-r--r--   0 root         (0) root         (0)   197269 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/dicts/common-passwords.gz
+-rwxr-xr-x   0 root         (0) root         (0)      532 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/dicts/convert_dict.sh
+-rw-r--r--   0 root         (0) root         (0)     3286 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/dicts/de-female.gz
+-rw-r--r--   0 root         (0) root         (0)     3070 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/dicts/de-male.gz
+-rw-r--r--   0 root         (0) root         (0)    11343 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/dicts/de-surnames.gz
+-rw-r--r--   0 root         (0) root         (0)    34845 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/dicts/de-top10000.gz
+-rw-r--r--   0 root         (0) root         (0)    30600 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/dicts/en-top10000.gz
+-rw-r--r--   0 root         (0) root         (0)   127983 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/dicts/english-guessing.gz
+-rw-r--r--   0 root         (0) root         (0)  1041710 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/dicts/english.gz
+-rw-r--r--   0 root         (0) root         (0)   547291 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/dicts/german-guessing.gz
+-rw-r--r--   0 root         (0) root         (0)   544600 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/dicts/german.gz
+-rw-r--r--   0 root         (0) root         (0)    13539 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/dicts/us-female.gz
+-rw-r--r--   0 root         (0) root         (0)     4089 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/dicts/us-male.gz
+-rw-r--r--   0 root         (0) root         (0)    35682 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/dicts/us-surnames.gz
+-rw-r--r--   0 root         (0) root         (0)    13331 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/otpme.conf.dist
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.732893 otpme-0.3.0a66/deploy/pam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.732893 otpme-0.3.0a66/deploy/pam/pam-python/
+-rw-r--r--   0 root         (0) root         (0)      511 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/pam/pam-python/README
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/pam/pam_otpme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.732893 otpme-0.3.0a66/deploy/radius/
+-rw-r--r--   0 root         (0) root         (0)    13085 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/radius/dictionary
+-rw-r--r--   0 root         (0) root         (0)     3851 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/radius/dictionary.freeradius
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.732893 otpme-0.3.0a66/deploy/schema/
+-rw-r--r--   0 root         (0) root         (0)    21610 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/schema/core.schema
+-rw-r--r--   0 root         (0) root         (0)    73993 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/schema/cosine.schema
+-rw-r--r--   0 root         (0) root         (0)     6267 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/schema/inetorgperson.schema
+-rw-r--r--   0 root         (0) root         (0)     7632 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/schema/nis.schema
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.732893 otpme-0.3.0a66/deploy/scripts/
+-rw-r--r--   0 root         (0) root         (0)     8600 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/scripts/agent_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/scripts/auth_script.sh
+-rw-r--r--   0 root         (0) root         (0)    21045 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/scripts/key_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/scripts/login_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/scripts/node_vote_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 17:58:10.000000 otpme-0.3.0a66/deploy/scripts/push_script.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.732893 otpme-0.3.0a66/otpme/
+-rw-r--r--   0 root         (0) root         (0)     1535 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    12650 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.740893 otpme-0.3.0a66/otpme/lib/
+-rw-r--r--   0 root         (0) root         (0)    10420 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/arp.py
+-rw-r--r--   0 root         (0) root         (0)     3502 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/auth_script.py
+-rw-r--r--   0 root         (0) root         (0)    48043 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.740893 otpme-0.3.0a66/otpme/lib/backends/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/backends/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.740893 otpme-0.3.0a66/otpme/lib/backends/file/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/backends/file/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90185 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/backends/file/file.py
+-rw-r--r--   0 root         (0) root         (0)    12946 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/backends/file/index.py
+-rw-r--r--   0 root         (0) root         (0)     5831 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/backends/file/models.py
+-rw-r--r--   0 root         (0) root         (0)    67194 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/backends/file/transaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.740893 otpme-0.3.0a66/otpme/lib/cache/
+-rw-r--r--   0 root         (0) root         (0)    27567 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cache/dogpile.py
+-rw-r--r--   0 root         (0) root         (0)    19444 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cache/funccache.py
+-rw-r--r--   0 root         (0) root         (0)     3448 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cache/lru.py
+-rw-r--r--   0 root         (0) root         (0)    14349 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cache/memcache.py
+-rw-r--r--   0 root         (0) root         (0)     6433 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cache/memcached.py
+-rw-r--r--   0 root         (0) root         (0)     7277 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cache/memcachedb.py
+-rw-r--r--   0 root         (0) root         (0)    27128 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cache/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.744893 otpme-0.3.0a66/otpme/lib/classes/
+-rw-r--r--   0 root         (0) root         (0)      890 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86180 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/accessgroup.py
+-rw-r--r--   0 root         (0) root         (0)    14807 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/agent_conn.py
+-rw-r--r--   0 root         (0) root         (0)   126036 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/auth_handler.py
+-rw-r--r--   0 root         (0) root         (0)    56607 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/ca.py
+-rw-r--r--   0 root         (0) root         (0)    40741 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/client.py
+-rw-r--r--   0 root         (0) root         (0)   230501 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/command_handler.py
+-rw-r--r--   0 root         (0) root         (0)     8663 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/conn_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.748893 otpme-0.3.0a66/otpme/lib/classes/data_objects/
+-rw-r--r--   0 root         (0) root         (0)      813 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/data_objects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/data_objects/cert.py
+-rw-r--r--   0 root         (0) root         (0)     6798 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/data_objects/data_revision.py
+-rw-r--r--   0 root         (0) root         (0)     6813 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/data_objects/failed_pass.py
+-rw-r--r--   0 root         (0) root         (0)     8058 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/data_objects/last_assigned_id.py
+-rw-r--r--   0 root         (0) root         (0)    10512 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/data_objects/revoked_signature.py
+-rw-r--r--   0 root         (0) root         (0)     2503 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/data_objects/rsa_key.py
+-rw-r--r--   0 root         (0) root         (0)     6953 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/data_objects/skip_sync.py
+-rw-r--r--   0 root         (0) root         (0)     5744 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/data_objects/token_counter.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/data_objects/used_hash.py
+-rw-r--r--   0 root         (0) root         (0)     5922 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/data_objects/used_otp.py
+-rw-r--r--   0 root         (0) root         (0)     5930 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/data_objects/used_slp.py
+-rw-r--r--   0 root         (0) root         (0)     5925 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/data_objects/used_sotp.py
+-rw-r--r--   0 root         (0) root         (0)    28615 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)    39118 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/group.py
+-rw-r--r--   0 root         (0) root         (0)    51998 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/host.py
+-rw-r--r--   0 root         (0) root         (0)    12229 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/login_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5303 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/mgmt_client.py
+-rw-r--r--   0 root         (0) root         (0)    38791 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/node.py
+-rw-r--r--   0 root         (0) root         (0)    24374 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/object_config.py
+-rw-r--r--   0 root         (0) root         (0)    77062 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/otpme_agent.py
+-rw-r--r--   0 root         (0) root         (0)    49637 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/otpme_host.py
+-rw-r--r--   0 root         (0) root         (0)   318795 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/otpme_object.py
+-rw-r--r--   0 root         (0) root         (0)    23290 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/policy.py
+-rw-r--r--   0 root         (0) root         (0)    62426 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/realm.py
+-rw-r--r--   0 root         (0) root         (0)    74411 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    45000 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/role.py
+-rw-r--r--   0 root         (0) root         (0)    34173 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/script.py
+-rw-r--r--   0 root         (0) root         (0)    52920 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/session.py
+-rw-r--r--   0 root         (0) root         (0)    31418 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/signing.py
+-rw-r--r--   0 root         (0) root         (0)   107184 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/site.py
+-rw-r--r--   0 root         (0) root         (0)     6987 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/ssh_agent.py
+-rw-r--r--   0 root         (0) root         (0)   134850 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/token.py
+-rw-r--r--   0 root         (0) root         (0)    49395 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/unit.py
+-rw-r--r--   0 root         (0) root         (0)   182171 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/classes/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.748893 otpme-0.3.0a66/otpme/lib/cli/
+-rw-r--r--   0 root         (0) root         (0)    64574 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12885 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/accessgroup.py
+-rw-r--r--   0 root         (0) root         (0)     7119 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/ca.py
+-rw-r--r--   0 root         (0) root         (0)    13242 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/client.py
+-rw-r--r--   0 root         (0) root         (0)     5643 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)    12993 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/group.py
+-rw-r--r--   0 root         (0) root         (0)    13057 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/host.py
+-rw-r--r--   0 root         (0) root         (0)    10974 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/node.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/policy.py
+-rw-r--r--   0 root         (0) root         (0)     6174 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/realm.py
+-rw-r--r--   0 root         (0) root         (0)     6600 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    20248 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/role.py
+-rw-r--r--   0 root         (0) root         (0)     7383 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/script.py
+-rw-r--r--   0 root         (0) root         (0)     7524 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/site.py
+-rw-r--r--   0 root         (0) root         (0)    17354 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/token.py
+-rw-r--r--   0 root         (0) root         (0)     5423 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/unit.py
+-rw-r--r--   0 root         (0) root         (0)     7596 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/cli/user.py
+-rw-r--r--   0 root         (0) root         (0)    24867 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/compgen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.748893 otpme-0.3.0a66/otpme/lib/compression/
+-rw-r--r--   0 root         (0) root         (0)      447 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/compression/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4082 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/compression/base.py
+-rw-r--r--   0 root         (0) root         (0)    14277 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/connections.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.752893 otpme-0.3.0a66/otpme/lib/daemon/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3785 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/daemon/authd.py
+-rw-r--r--   0 root         (0) root         (0)   108965 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/daemon/clusterd.py
+-rw-r--r--   0 root         (0) root         (0)    47551 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/daemon/controld.py
+-rw-r--r--   0 root         (0) root         (0)    76763 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/daemon/hostd.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/daemon/joind.py
+-rw-r--r--   0 root         (0) root         (0)     6713 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/daemon/ldapd.py
+-rw-r--r--   0 root         (0) root         (0)     3003 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/daemon/mgmtd.py
+-rw-r--r--   0 root         (0) root         (0)    15876 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/daemon/otpme_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    11391 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/daemon/scriptd.py
+-rw-r--r--   0 root         (0) root         (0)     3017 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/daemon/syncd.py
+-rw-r--r--   0 root         (0) root         (0)     6941 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/daemon/unix_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    19005 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/debug.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/doc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.752893 otpme-0.3.0a66/otpme/lib/encoding/
+-rw-r--r--   0 root         (0) root         (0)      429 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/encoding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/encoding/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.752893 otpme-0.3.0a66/otpme/lib/encryption/
+-rw-r--r--   0 root         (0) root         (0)     3953 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/encryption/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3296 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/encryption/aes.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/encryption/aes_cfb.py
+-rw-r--r--   0 root         (0) root         (0)     7900 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/encryption/argon2.py
+-rw-r--r--   0 root         (0) root         (0)    10240 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/encryption/asymmetric_key_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4251 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/encryption/ec.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/encryption/fernet.py
+-rw-r--r--   0 root         (0) root         (0)     3237 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/encryption/hkdf.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/encryption/pbkdf2.py
+-rw-r--r--   0 root         (0) root         (0)     7824 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/encryption/rsa.py
+-rw-r--r--   0 root         (0) root         (0)     4324 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.752893 otpme-0.3.0a66/otpme/lib/extensions/
+-rw-r--r--   0 root         (0) root         (0)      329 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/extensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.752893 otpme-0.3.0a66/otpme/lib/extensions/base/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/extensions/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12278 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/extensions/base/base.py
+-rw-r--r--   0 root         (0) root         (0)    40152 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/extensions/ldif_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.752893 otpme-0.3.0a66/otpme/lib/extensions/posix/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/extensions/posix/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14286 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/extensions/posix/posix.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/extensions/utils.py
+-rw-r--r--   0 root         (0) root         (0)    34081 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/filetools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.752893 otpme-0.3.0a66/otpme/lib/freeradius/
+-rw-r--r--   0 root         (0) root         (0)     9119 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/freeradius/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18685 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/freeradius/otpme.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/freeradius/radiusd.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/freeradius/radiusd_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.752893 otpme-0.3.0a66/otpme/lib/gpg/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/gpg/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    28498 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/gpg/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.756893 otpme-0.3.0a66/otpme/lib/help/
+-rwxr-xr-x   0 root         (0) root         (0)    26529 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22986 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/accessgroup.py
+-rw-r--r--   0 root         (0) root         (0)     5485 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/agent.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/auth.py
+-rw-r--r--   0 root         (0) root         (0)    15707 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/ca.py
+-rw-r--r--   0 root         (0) root         (0)    16924 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/client.py
+-rw-r--r--   0 root         (0) root         (0)     1568 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5785 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/controld.py
+-rw-r--r--   0 root         (0) root         (0)    11388 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)      522 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/get_authorized_keys.py
+-rw-r--r--   0 root         (0) root         (0)    19872 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/group.py
+-rw-r--r--   0 root         (0) root         (0)    24436 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/host.py
+-rw-r--r--   0 root         (0) root         (0)    21309 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/node.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/pinentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.756893 otpme-0.3.0a66/otpme/lib/help/policy/
+-rw-r--r--   0 root         (0) root         (0)     8739 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/policy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/policy/authonaction.py
+-rw-r--r--   0 root         (0) root         (0)     1247 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/policy/autodisable.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/policy/defaultgroups.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/policy/defaultpolicies.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/policy/defaultroles.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/policy/defaultunits.py
+-rw-r--r--   0 root         (0) root         (0)     1492 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/policy/forcetoken.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/policy/idrange.py
+-rw-r--r--   0 root         (0) root         (0)     3225 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/policy/logintimes.py
+-rw-r--r--   0 root         (0) root         (0)     1098 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/policy/objecttemplates.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/policy/password.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/policy/tokenacls.py
+-rw-r--r--   0 root         (0) root         (0)    20037 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/realm.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/register.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.756893 otpme-0.3.0a66/otpme/lib/help/resolver/
+-rw-r--r--   0 root         (0) root         (0)    12522 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/resolver/ldap.py
+-rw-r--r--   0 root         (0) root         (0)    18198 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/role.py
+-rw-r--r--   0 root         (0) root         (0)    15111 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/script.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/session.py
+-rw-r--r--   0 root         (0) root         (0)    22488 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.760893 otpme-0.3.0a66/otpme/lib/help/token/
+-rw-r--r--   0 root         (0) root         (0)    20503 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/token/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/token/fido2.py
+-rw-r--r--   0 root         (0) root         (0)     5619 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/token/hotp.py
+-rw-r--r--   0 root         (0) root         (0)     6339 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/token/motp.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/token/otp_push.py
+-rw-r--r--   0 root         (0) root         (0)     4951 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/token/otpme.py
+-rw-r--r--   0 root         (0) root         (0)     3880 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/token/password.py
+-rw-r--r--   0 root         (0) root         (0)     7251 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/token/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     5977 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/token/totp.py
+-rw-r--r--   0 root         (0) root         (0)     5803 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/token/yubikey_hmac.py
+-rw-r--r--   0 root         (0) root         (0)     1252 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/token/yubikey_hotp.py
+-rw-r--r--   0 root         (0) root         (0)    24935 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/tool.py
+-rw-r--r--   0 root         (0) root         (0)    15168 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/unit.py
+-rw-r--r--   0 root         (0) root         (0)    29409 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/help/user.py
+-rw-r--r--   0 root         (0) root         (0)    16341 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/host.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.760893 otpme-0.3.0a66/otpme/lib/humanize/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/humanize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4191 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/humanize/units.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.760893 otpme-0.3.0a66/otpme/lib/index/
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23948 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/index/mysql.py
+-rw-r--r--   0 root         (0) root         (0)    24542 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/index/postgres.py
+-rw-r--r--   0 root         (0) root         (0)     8336 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/index/sqlite3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.760893 otpme-0.3.0a66/otpme/lib/job/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20681 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/job/callback.py
+-rw-r--r--   0 root         (0) root         (0)    12849 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/job/otpme_job.py
+-rw-r--r--   0 root         (0) root         (0)    37097 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/join.py
+-rw-r--r--   0 root         (0) root         (0)     4857 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/json.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.760893 otpme-0.3.0a66/otpme/lib/ldap/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/ldap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1354 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/ldap/client.py
+-rw-r--r--   0 root         (0) root         (0)    11062 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/ldap/schema.py
+-rw-r--r--   0 root         (0) root         (0)    50483 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/ldap/server.py
+-rw-r--r--   0 root         (0) root         (0)    19709 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/locking.py
+-rw-r--r--   0 root         (0) root         (0)     9430 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/log.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/messages.py
+-rw-r--r--   0 root         (0) root         (0)     5981 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/mschap.py
+-rw-r--r--   0 root         (0) root         (0)     2366 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/mschap_util.py
+-rw-r--r--   0 root         (0) root         (0)    35744 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/multiprocessing.py
+-rw-r--r--   0 root         (0) root         (0)    10250 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/net.py
+-rw-r--r--   0 root         (0) root         (0)    27144 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/nsscache.py
+-rw-r--r--   0 root         (0) root         (0)    63328 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/offline_token.py
+-rw-r--r--   0 root         (0) root         (0)    23778 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/oid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.760893 otpme-0.3.0a66/otpme/lib/otp/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/otp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.760893 otpme-0.3.0a66/otpme/lib/otp/oath/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/otp/oath/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/otp/oath/hotp.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/otp/oath/totp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.760893 otpme-0.3.0a66/otpme/lib/otp/otpme/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/otp/otpme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/otp/otpme/otpme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.760893 otpme-0.3.0a66/otpme/lib/otp/yubico/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/otp/yubico/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3026 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/otp/yubico/yubiotp.py
+-rw-r--r--   0 root         (0) root         (0)    19837 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/otpme_acl.py
+-rw-r--r--   0 root         (0) root         (0)   115772 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/otpme_config.py
+-rw-r--r--   0 root         (0) root         (0)     3519 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/otpme_pass.py
+-rw-r--r--   0 root         (0) root         (0)    70359 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/pam.py
+-rw-r--r--   0 root         (0) root         (0)     1975 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/pickle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.760893 otpme-0.3.0a66/otpme/lib/pinentry/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/pinentry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27465 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/pinentry/pinentry.py
+-rwxr-xr-x   0 root         (0) root         (0)     7880 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/pinentry/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.764893 otpme-0.3.0a66/otpme/lib/pki/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/pki/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9797 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/pki/cert.py
+-rw-r--r--   0 root         (0) root         (0)    23150 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/pki/utils.py
+-rw-r--r--   0 root         (0) root         (0)    16890 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/pki/utils_openssl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.764893 otpme-0.3.0a66/otpme/lib/policy/
+-rw-r--r--   0 root         (0) root         (0)     2099 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.764893 otpme-0.3.0a66/otpme/lib/policy/authonaction/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/authonaction/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32663 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/authonaction/authonaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.764893 otpme-0.3.0a66/otpme/lib/policy/autodisable/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/autodisable/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15718 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/autodisable/autodisable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.764893 otpme-0.3.0a66/otpme/lib/policy/defaultgroups/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/defaultgroups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17570 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/defaultgroups/defaultgroups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.764893 otpme-0.3.0a66/otpme/lib/policy/defaultpolicies/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/defaultpolicies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14510 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/defaultpolicies/defaultpolicies.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.764893 otpme-0.3.0a66/otpme/lib/policy/defaultroles/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/defaultroles/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14217 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/defaultroles/defaultroles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.764893 otpme-0.3.0a66/otpme/lib/policy/defaultunits/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/defaultunits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15637 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/defaultunits/defaultunits.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.764893 otpme-0.3.0a66/otpme/lib/policy/forcetoken/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/forcetoken/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14202 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/forcetoken/forcetoken.py
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/get_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.764893 otpme-0.3.0a66/otpme/lib/policy/idrange/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/idrange/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27256 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/idrange/idrange.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.764893 otpme-0.3.0a66/otpme/lib/policy/logintimes/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/logintimes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23017 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/logintimes/logintimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.764893 otpme-0.3.0a66/otpme/lib/policy/objecttemplates/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/objecttemplates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14954 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/objecttemplates/objecttemplates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.764893 otpme-0.3.0a66/otpme/lib/policy/password/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/password/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28981 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/password/password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.764893 otpme-0.3.0a66/otpme/lib/policy/tokenacls/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/tokenacls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24897 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/tokenacls/tokenacls.py
+-rw-r--r--   0 root         (0) root         (0)      491 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/policy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9332 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/preload.py
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.768893 otpme-0.3.0a66/otpme/lib/protocols/
+-rw-r--r--   0 root         (0) root         (0)      304 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.768893 otpme-0.3.0a66/otpme/lib/protocols/client/
+-rw-r--r--   0 root         (0) root         (0)      655 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1887 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/client/agent1.py
+-rw-r--r--   0 root         (0) root         (0)      832 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/client/auth1.py
+-rw-r--r--   0 root         (0) root         (0)    14301 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/client/cluster1.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/client/get_class.py
+-rw-r--r--   0 root         (0) root         (0)     4645 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/client/host1.py
+-rw-r--r--   0 root         (0) root         (0)      832 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/client/join1.py
+-rwxr-xr-x   0 root         (0) root         (0)    11305 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/client/mgmt1.py
+-rw-r--r--   0 root         (0) root         (0)    67975 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/client/sync1.py
+-rw-r--r--   0 root         (0) root         (0)   160693 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/otpme_client.py
+-rw-r--r--   0 root         (0) root         (0)    81420 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/otpme_server.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/request.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.768893 otpme-0.3.0a66/otpme/lib/protocols/server/
+-rw-r--r--   0 root         (0) root         (0)      827 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40219 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/server/agent1.py
+-rw-r--r--   0 root         (0) root         (0)    12842 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/server/auth1.py
+-rw-r--r--   0 root         (0) root         (0)    32302 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/server/cluster1.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/server/get_class.py
+-rw-r--r--   0 root         (0) root         (0)    26608 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/server/host1.py
+-rw-r--r--   0 root         (0) root         (0)    52562 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/server/join1.py
+-rw-r--r--   0 root         (0) root         (0)    70866 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/server/mgmt1.py
+-rw-r--r--   0 root         (0) root         (0)    45433 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/server/sync1.py
+-rw-r--r--   0 root         (0) root         (0)      527 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/status_codes.py
+-rw-r--r--   0 root         (0) root         (0)     6937 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/protocols/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/push_script.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/qrcode.py
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/re.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.768893 otpme-0.3.0a66/otpme/lib/register/
+-rw-r--r--   0 root         (0) root         (0)     9716 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/register/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.768893 otpme-0.3.0a66/otpme/lib/resolver/
+-rw-r--r--   0 root         (0) root         (0)      485 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1158 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/resolver/get_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.768893 otpme-0.3.0a66/otpme/lib/resolver/ldap/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/resolver/ldap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39438 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/resolver/ldap/ldap.py
+-rw-r--r--   0 root         (0) root         (0)      451 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/resolver/utils.py
+-rw-r--r--   0 root         (0) root         (0)    10019 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/script.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/sign_key_cache.py
+-rw-r--r--   0 root         (0) root         (0)      537 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/slp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.768893 otpme-0.3.0a66/otpme/lib/smartcard/
+-rw-r--r--   0 root         (0) root         (0)      623 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/smartcard/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.768893 otpme-0.3.0a66/otpme/lib/smartcard/fido2/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/smartcard/fido2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10161 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/smartcard/fido2/fido2.py
+-rw-r--r--   0 root         (0) root         (0)      858 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/smartcard/get_class.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/smartcard/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.768893 otpme-0.3.0a66/otpme/lib/smartcard/yubikey/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/smartcard/yubikey/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11951 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/smartcard/yubikey/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/smartcard/yubikey/usb.py
+-rw-r--r--   0 root         (0) root         (0)     8075 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/smartcard/yubikey/yubikey.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.772894 otpme-0.3.0a66/otpme/lib/smartcard/yubikey_gpg/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/smartcard/yubikey_gpg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6364 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.772894 otpme-0.3.0a66/otpme/lib/smartcard/yubikey_hmac/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/smartcard/yubikey_hmac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11955 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.772894 otpme-0.3.0a66/otpme/lib/smartcard/yubikey_hotp/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/smartcard/yubikey_hotp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5032 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.772894 otpme-0.3.0a66/otpme/lib/socket/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/socket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13152 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/socket/connect.py
+-rw-r--r--   0 root         (0) root         (0)     8450 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/socket/handler.py
+-rw-r--r--   0 root         (0) root         (0)    30962 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/socket/listen.py
+-rw-r--r--   0 root         (0) root         (0)     2830 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/socket/send_recv1.py
+-rw-r--r--   0 root         (0) root         (0)     4408 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/sotp.py
+-rwxr-xr-x   0 root         (0) root         (0)    37113 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/spsc.py
+-rw-r--r--   0 root         (0) root         (0)      544 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/srp.py
+-rw-r--r--   0 root         (0) root         (0)    23454 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/ssh.py
+-rw-r--r--   0 root         (0) root         (0)    63673 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/stuff.py
+-rw-r--r--   0 root         (0) root         (0)    12338 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/sync_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/system_command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.772894 otpme-0.3.0a66/otpme/lib/third_party/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.772894 otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/advanced.py
+-rw-r--r--   0 root         (0) root         (0)     9859 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/caching_query.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/environment.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/fixture_data.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/helloworld.py
+-rw-r--r--   0 root         (0) root         (0)     3310 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/local_session_caching.py
+-rw-r--r--   0 root         (0) root         (0)     3033 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/model.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/relationship_caching.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.772894 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.772894 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/caches/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/caches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9083 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/caches/caches.py
+-rw-r--r--   0 root         (0) root         (0)    14341 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/caches/files.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/config.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/error.py
+-rw-r--r--   0 root         (0) root         (0)     7963 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.772894 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/maps/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/maps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/maps/group.py
+-rw-r--r--   0 root         (0) root         (0)    11745 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/maps/maps.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/maps/passwd.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/maps/shadow.py
+-rw-r--r--   0 root         (0) root         (0)     4140 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/nss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.772894 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/update/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/update/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5487 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/update/files_updater.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/update/map_updater.py
+-rw-r--r--   0 root         (0) root         (0)    10980 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/update/updater.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.772894 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4117 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/nss_cache/util/file_formats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.776894 otpme-0.3.0a66/otpme/lib/third_party/oath_toolkit/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/oath_toolkit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/oath_toolkit/_compat.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/third_party/oath_toolkit/uri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.776894 otpme-0.3.0a66/otpme/lib/token/
+-rw-r--r--   0 root         (0) root         (0)      953 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.776894 otpme-0.3.0a66/otpme/lib/token/fido2/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/fido2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14939 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/fido2/fido2.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/get_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.776894 otpme-0.3.0a66/otpme/lib/token/hotp/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/hotp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39346 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/hotp/hotp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.776894 otpme-0.3.0a66/otpme/lib/token/link/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/link/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9656 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/link/link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.776894 otpme-0.3.0a66/otpme/lib/token/motp/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/motp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27770 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/motp/motp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.776894 otpme-0.3.0a66/otpme/lib/token/oath/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/oath/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19667 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/oath/oath.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.776894 otpme-0.3.0a66/otpme/lib/token/otp_push/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/otp_push/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23393 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/otp_push/otp_push.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.776894 otpme-0.3.0a66/otpme/lib/token/otpme/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/otpme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24704 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/otpme/otpme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.776894 otpme-0.3.0a66/otpme/lib/token/password/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/password/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26068 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/password/password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.776894 otpme-0.3.0a66/otpme/lib/token/script_otp/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/script_otp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9677 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/script_otp/script_otp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.776894 otpme-0.3.0a66/otpme/lib/token/script_static/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/script_static/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9677 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/script_static/script_static.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.776894 otpme-0.3.0a66/otpme/lib/token/ssh/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/ssh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39547 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/ssh/ssh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.776894 otpme-0.3.0a66/otpme/lib/token/totp/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/totp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35398 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/totp/totp.py
+-rw-r--r--   0 root         (0) root         (0)      480 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.776894 otpme-0.3.0a66/otpme/lib/token/yubikey_hmac/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/yubikey_hmac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25111 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme/lib/token/yubikey_hmac/yubikey_hmac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:58:10.736893 otpme-0.3.0a66/otpme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      680 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13359 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      973 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-23 17:58:10.000000 otpme-0.3.0a66/otpme.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 17:58:10.776894 otpme-0.3.0a66/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8833 2024-05-23 17:58:10.000000 otpme-0.3.0a66/setup.py
```

### Comparing `otpme-0.3.0a65/LICENSE` & `otpme-0.3.0a66/LICENSE`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/MANIFEST.in` & `otpme-0.3.0a66/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/PKG-INFO` & `otpme-0.3.0a66/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otpme
-Version: 0.3.0a65
+Version: 0.3.0a66
 Summary: OTPme: A flexible One-Time-Password system.
 Home-page: http://www.otpme.org
 Author: the2nd
 Author-email: the2nd@otpme.org
 Maintainer: the2nd
 Maintainer-email: the2nd@otpme.org
 License: GPLv2
```

### Comparing `otpme-0.3.0a65/README` & `otpme-0.3.0a66/README`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/bash_completion/otpme` & `otpme-0.3.0a66/bash_completion/otpme`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/dicts/abbreviations-it.gz` & `otpme-0.3.0a66/deploy/dicts/abbreviations-it.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/dicts/at-surnames.gz` & `otpme-0.3.0a66/deploy/dicts/at-surnames.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/dicts/common-passwords.gz` & `otpme-0.3.0a66/deploy/dicts/common-passwords.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/dicts/convert_dict.sh` & `otpme-0.3.0a66/deploy/dicts/convert_dict.sh`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/dicts/de-female.gz` & `otpme-0.3.0a66/deploy/dicts/de-female.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/dicts/de-male.gz` & `otpme-0.3.0a66/deploy/dicts/de-male.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/dicts/de-surnames.gz` & `otpme-0.3.0a66/deploy/dicts/de-surnames.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/dicts/de-top10000.gz` & `otpme-0.3.0a66/deploy/dicts/de-top10000.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/dicts/en-top10000.gz` & `otpme-0.3.0a66/deploy/dicts/en-top10000.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/dicts/english-guessing.gz` & `otpme-0.3.0a66/deploy/dicts/english-guessing.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/dicts/english.gz` & `otpme-0.3.0a66/deploy/dicts/english.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/dicts/german-guessing.gz` & `otpme-0.3.0a66/deploy/dicts/german-guessing.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/dicts/german.gz` & `otpme-0.3.0a66/deploy/dicts/german.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/dicts/us-female.gz` & `otpme-0.3.0a66/deploy/dicts/us-female.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/dicts/us-male.gz` & `otpme-0.3.0a66/deploy/dicts/us-male.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/dicts/us-surnames.gz` & `otpme-0.3.0a66/deploy/dicts/us-surnames.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/otpme.conf.dist` & `otpme-0.3.0a66/deploy/otpme.conf.dist`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # OTPme config file
 
 # Path to otpme commands.
-BIN_DIR="/usr/local/bin/"
+BIN_DIR="/opt/otpme/bin/"
 # Timezone to use (e.g. certificates).
 TIMEZONE="Europe/Berlin"
 
 # Start freeradius.
 START_FREERADIUS="True"
 # Path to freeradius binary.
 FREERADIUS_BIN="/usr/sbin/freeradius"
```

### Comparing `otpme-0.3.0a65/deploy/pam/pam_otpme.py` & `otpme-0.3.0a66/deploy/pam/pam_otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/radius/dictionary` & `otpme-0.3.0a66/deploy/radius/dictionary`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/radius/dictionary.freeradius` & `otpme-0.3.0a66/deploy/radius/dictionary.freeradius`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/schema/core.schema` & `otpme-0.3.0a66/deploy/schema/core.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/schema/cosine.schema` & `otpme-0.3.0a66/deploy/schema/cosine.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/schema/inetorgperson.schema` & `otpme-0.3.0a66/deploy/schema/inetorgperson.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/schema/nis.schema` & `otpme-0.3.0a66/deploy/schema/nis.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/scripts/agent_script.sh` & `otpme-0.3.0a66/deploy/scripts/agent_script.sh`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/deploy/scripts/key_script.sh` & `otpme-0.3.0a66/deploy/scripts/key_script.sh`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/__init__.py` & `otpme-0.3.0a66/otpme/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 __project_url__ = "http://www.otpme.org"
 __copyright__ = "Copyright 2014-2024 the2nd <the2nd@otpme.org>"
 __project_description__ = "OTPme: A flexible One-Time-Password system."
 __author__ = "the2nd"
 __email__ = "the2nd@otpme.org"
 __credits__ = []
 __license__ = "GPLv2"
-__version__ = "0.3.0a65"
+__version__ = "0.3.0a66"
 __status__ = "Development Status :: 3 - Alpha"
 # In future versions :D
 #__status__ = "Development Status :: 4 - Beta"
 #__status__ = "Development Status :: 5 - Production/Stable"
 __pkg_name__ = __project_name__
 __maintainer__ = __author__
 __author_email__  = __email__
```

### Comparing `otpme-0.3.0a65/otpme/command.py` & `otpme-0.3.0a66/otpme/command.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/__init__.py` & `otpme-0.3.0a66/otpme/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/arp.py` & `otpme-0.3.0a66/otpme/lib/arp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/auth_script.py` & `otpme-0.3.0a66/otpme/lib/auth_script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/backend.py` & `otpme-0.3.0a66/otpme/lib/backend.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/backends/file/file.py` & `otpme-0.3.0a66/otpme/lib/backends/file/file.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/backends/file/index.py` & `otpme-0.3.0a66/otpme/lib/backends/file/index.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/backends/file/models.py` & `otpme-0.3.0a66/otpme/lib/backends/file/models.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/backends/file/transaction.py` & `otpme-0.3.0a66/otpme/lib/backends/file/transaction.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cache/__init__.py` & `otpme-0.3.0a66/otpme/lib/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cache/dogpile.py` & `otpme-0.3.0a66/otpme/lib/cache/dogpile.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cache/funccache.py` & `otpme-0.3.0a66/otpme/lib/cache/funccache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cache/lru.py` & `otpme-0.3.0a66/otpme/lib/cache/lru.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cache/memcache.py` & `otpme-0.3.0a66/otpme/lib/cache/memcache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cache/memcached.py` & `otpme-0.3.0a66/otpme/lib/cache/memcached.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cache/memcachedb.py` & `otpme-0.3.0a66/otpme/lib/cache/memcachedb.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cache/redis.py` & `otpme-0.3.0a66/otpme/lib/cache/redis.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/__init__.py` & `otpme-0.3.0a66/otpme/lib/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/accessgroup.py` & `otpme-0.3.0a66/otpme/lib/classes/accessgroup.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/agent_conn.py` & `otpme-0.3.0a66/otpme/lib/classes/agent_conn.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/auth_handler.py` & `otpme-0.3.0a66/otpme/lib/classes/auth_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/ca.py` & `otpme-0.3.0a66/otpme/lib/classes/ca.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/client.py` & `otpme-0.3.0a66/otpme/lib/classes/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/command_handler.py` & `otpme-0.3.0a66/otpme/lib/classes/command_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/conn_handler.py` & `otpme-0.3.0a66/otpme/lib/classes/conn_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/data_objects/__init__.py` & `otpme-0.3.0a66/otpme/lib/classes/data_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/data_objects/cert.py` & `otpme-0.3.0a66/otpme/lib/classes/data_objects/cert.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/data_objects/data_revision.py` & `otpme-0.3.0a66/otpme/lib/classes/data_objects/data_revision.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/data_objects/failed_pass.py` & `otpme-0.3.0a66/otpme/lib/classes/data_objects/failed_pass.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/data_objects/last_assigned_id.py` & `otpme-0.3.0a66/otpme/lib/classes/data_objects/last_assigned_id.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/data_objects/revoked_signature.py` & `otpme-0.3.0a66/otpme/lib/classes/data_objects/revoked_signature.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/data_objects/rsa_key.py` & `otpme-0.3.0a66/otpme/lib/classes/data_objects/rsa_key.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/data_objects/skip_sync.py` & `otpme-0.3.0a66/otpme/lib/classes/data_objects/skip_sync.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/data_objects/token_counter.py` & `otpme-0.3.0a66/otpme/lib/classes/data_objects/token_counter.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/data_objects/used_hash.py` & `otpme-0.3.0a66/otpme/lib/classes/data_objects/used_hash.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/data_objects/used_otp.py` & `otpme-0.3.0a66/otpme/lib/classes/data_objects/used_otp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/data_objects/used_slp.py` & `otpme-0.3.0a66/otpme/lib/classes/data_objects/used_slp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/data_objects/used_sotp.py` & `otpme-0.3.0a66/otpme/lib/classes/data_objects/used_sotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/dictionary.py` & `otpme-0.3.0a66/otpme/lib/classes/dictionary.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/group.py` & `otpme-0.3.0a66/otpme/lib/classes/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/host.py` & `otpme-0.3.0a66/otpme/lib/classes/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/login_handler.py` & `otpme-0.3.0a66/otpme/lib/classes/login_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/mgmt_client.py` & `otpme-0.3.0a66/otpme/lib/classes/mgmt_client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/node.py` & `otpme-0.3.0a66/otpme/lib/classes/node.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/object_config.py` & `otpme-0.3.0a66/otpme/lib/classes/object_config.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/otpme_agent.py` & `otpme-0.3.0a66/otpme/lib/classes/otpme_agent.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/otpme_host.py` & `otpme-0.3.0a66/otpme/lib/classes/otpme_host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/otpme_object.py` & `otpme-0.3.0a66/otpme/lib/classes/otpme_object.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/policy.py` & `otpme-0.3.0a66/otpme/lib/classes/policy.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/realm.py` & `otpme-0.3.0a66/otpme/lib/classes/realm.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/resolver.py` & `otpme-0.3.0a66/otpme/lib/classes/resolver.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/role.py` & `otpme-0.3.0a66/otpme/lib/classes/role.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/script.py` & `otpme-0.3.0a66/otpme/lib/classes/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/session.py` & `otpme-0.3.0a66/otpme/lib/classes/session.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/signing.py` & `otpme-0.3.0a66/otpme/lib/classes/signing.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/site.py` & `otpme-0.3.0a66/otpme/lib/classes/site.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/ssh_agent.py` & `otpme-0.3.0a66/otpme/lib/classes/ssh_agent.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/token.py` & `otpme-0.3.0a66/otpme/lib/classes/token.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/unit.py` & `otpme-0.3.0a66/otpme/lib/classes/unit.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/classes/user.py` & `otpme-0.3.0a66/otpme/lib/classes/user.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/__init__.py` & `otpme-0.3.0a66/otpme/lib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/accessgroup.py` & `otpme-0.3.0a66/otpme/lib/cli/accessgroup.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/ca.py` & `otpme-0.3.0a66/otpme/lib/cli/ca.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/client.py` & `otpme-0.3.0a66/otpme/lib/cli/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/dictionary.py` & `otpme-0.3.0a66/otpme/lib/cli/dictionary.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/group.py` & `otpme-0.3.0a66/otpme/lib/cli/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/host.py` & `otpme-0.3.0a66/otpme/lib/cli/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/node.py` & `otpme-0.3.0a66/otpme/lib/cli/node.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/policy.py` & `otpme-0.3.0a66/otpme/lib/cli/policy.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/realm.py` & `otpme-0.3.0a66/otpme/lib/cli/realm.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/resolver.py` & `otpme-0.3.0a66/otpme/lib/cli/resolver.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/role.py` & `otpme-0.3.0a66/otpme/lib/cli/role.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/script.py` & `otpme-0.3.0a66/otpme/lib/cli/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/site.py` & `otpme-0.3.0a66/otpme/lib/cli/site.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/token.py` & `otpme-0.3.0a66/otpme/lib/cli/token.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/unit.py` & `otpme-0.3.0a66/otpme/lib/cli/unit.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/cli/user.py` & `otpme-0.3.0a66/otpme/lib/cli/user.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/compgen.py` & `otpme-0.3.0a66/otpme/lib/compgen.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/compression/base.py` & `otpme-0.3.0a66/otpme/lib/compression/base.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/connections.py` & `otpme-0.3.0a66/otpme/lib/connections.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/daemon/__init__.py` & `otpme-0.3.0a66/otpme/lib/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/daemon/authd.py` & `otpme-0.3.0a66/otpme/lib/daemon/authd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/daemon/clusterd.py` & `otpme-0.3.0a66/otpme/lib/daemon/clusterd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/daemon/controld.py` & `otpme-0.3.0a66/otpme/lib/daemon/controld.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/daemon/hostd.py` & `otpme-0.3.0a66/otpme/lib/daemon/hostd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/daemon/joind.py` & `otpme-0.3.0a66/otpme/lib/daemon/joind.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/daemon/ldapd.py` & `otpme-0.3.0a66/otpme/lib/daemon/ldapd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/daemon/mgmtd.py` & `otpme-0.3.0a66/otpme/lib/daemon/mgmtd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/daemon/otpme_daemon.py` & `otpme-0.3.0a66/otpme/lib/daemon/otpme_daemon.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/daemon/scriptd.py` & `otpme-0.3.0a66/otpme/lib/daemon/scriptd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/daemon/syncd.py` & `otpme-0.3.0a66/otpme/lib/daemon/syncd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/daemon/unix_daemon.py` & `otpme-0.3.0a66/otpme/lib/daemon/unix_daemon.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/debug.py` & `otpme-0.3.0a66/otpme/lib/debug.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/doc.py` & `otpme-0.3.0a66/otpme/lib/doc.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/encoding/base.py` & `otpme-0.3.0a66/otpme/lib/encoding/base.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/encryption/__init__.py` & `otpme-0.3.0a66/otpme/lib/encryption/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/encryption/aes.py` & `otpme-0.3.0a66/otpme/lib/encryption/aes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/encryption/aes_cfb.py` & `otpme-0.3.0a66/otpme/lib/encryption/aes_cfb.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/encryption/argon2.py` & `otpme-0.3.0a66/otpme/lib/encryption/argon2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/encryption/asymmetric_key_handler.py` & `otpme-0.3.0a66/otpme/lib/encryption/asymmetric_key_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/encryption/ec.py` & `otpme-0.3.0a66/otpme/lib/encryption/ec.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/encryption/fernet.py` & `otpme-0.3.0a66/otpme/lib/encryption/fernet.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/encryption/hkdf.py` & `otpme-0.3.0a66/otpme/lib/encryption/hkdf.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/encryption/pbkdf2.py` & `otpme-0.3.0a66/otpme/lib/encryption/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/encryption/rsa.py` & `otpme-0.3.0a66/otpme/lib/encryption/rsa.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/exceptions.py` & `otpme-0.3.0a66/otpme/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/extensions/base/base.py` & `otpme-0.3.0a66/otpme/lib/extensions/base/base.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/extensions/ldif_handler.py` & `otpme-0.3.0a66/otpme/lib/extensions/ldif_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/extensions/posix/posix.py` & `otpme-0.3.0a66/otpme/lib/extensions/posix/posix.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/extensions/utils.py` & `otpme-0.3.0a66/otpme/lib/extensions/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/filetools.py` & `otpme-0.3.0a66/otpme/lib/filetools.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/freeradius/__init__.py` & `otpme-0.3.0a66/otpme/lib/freeradius/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/freeradius/otpme.py` & `otpme-0.3.0a66/otpme/lib/freeradius/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/freeradius/radiusd.py` & `otpme-0.3.0a66/otpme/lib/freeradius/radiusd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/freeradius/radiusd_test.py` & `otpme-0.3.0a66/otpme/lib/freeradius/radiusd_test.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/gpg/utils.py` & `otpme-0.3.0a66/otpme/lib/gpg/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/__init__.py` & `otpme-0.3.0a66/otpme/lib/help/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/accessgroup.py` & `otpme-0.3.0a66/otpme/lib/help/accessgroup.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/agent.py` & `otpme-0.3.0a66/otpme/lib/help/agent.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/auth.py` & `otpme-0.3.0a66/otpme/lib/help/auth.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/ca.py` & `otpme-0.3.0a66/otpme/lib/help/ca.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/client.py` & `otpme-0.3.0a66/otpme/lib/help/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/cluster.py` & `otpme-0.3.0a66/otpme/lib/help/cluster.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/controld.py` & `otpme-0.3.0a66/otpme/lib/help/controld.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/dictionary.py` & `otpme-0.3.0a66/otpme/lib/help/dictionary.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/get_authorized_keys.py` & `otpme-0.3.0a66/otpme/lib/help/get_authorized_keys.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/group.py` & `otpme-0.3.0a66/otpme/lib/help/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/host.py` & `otpme-0.3.0a66/otpme/lib/help/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/node.py` & `otpme-0.3.0a66/otpme/lib/help/node.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/policy/__init__.py` & `otpme-0.3.0a66/otpme/lib/help/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/policy/authonaction.py` & `otpme-0.3.0a66/otpme/lib/help/policy/authonaction.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/policy/autodisable.py` & `otpme-0.3.0a66/otpme/lib/help/policy/autodisable.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/policy/defaultgroups.py` & `otpme-0.3.0a66/otpme/lib/help/policy/defaultgroups.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/policy/defaultpolicies.py` & `otpme-0.3.0a66/otpme/lib/help/policy/defaultpolicies.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/policy/defaultroles.py` & `otpme-0.3.0a66/otpme/lib/help/policy/defaultroles.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/policy/defaultunits.py` & `otpme-0.3.0a66/otpme/lib/help/policy/defaultunits.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/policy/forcetoken.py` & `otpme-0.3.0a66/otpme/lib/help/policy/forcetoken.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/policy/idrange.py` & `otpme-0.3.0a66/otpme/lib/help/policy/idrange.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/policy/logintimes.py` & `otpme-0.3.0a66/otpme/lib/help/policy/logintimes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/policy/objecttemplates.py` & `otpme-0.3.0a66/otpme/lib/help/policy/objecttemplates.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/policy/password.py` & `otpme-0.3.0a66/otpme/lib/help/policy/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/policy/tokenacls.py` & `otpme-0.3.0a66/otpme/lib/help/policy/tokenacls.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/realm.py` & `otpme-0.3.0a66/otpme/lib/help/realm.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/register.py` & `otpme-0.3.0a66/otpme/lib/help/register.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/resolver/__init__.py` & `otpme-0.3.0a66/otpme/lib/help/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/resolver/ldap.py` & `otpme-0.3.0a66/otpme/lib/help/resolver/ldap.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/role.py` & `otpme-0.3.0a66/otpme/lib/help/role.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/script.py` & `otpme-0.3.0a66/otpme/lib/help/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/session.py` & `otpme-0.3.0a66/otpme/lib/help/session.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/site.py` & `otpme-0.3.0a66/otpme/lib/help/site.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/token/__init__.py` & `otpme-0.3.0a66/otpme/lib/help/token/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/token/fido2.py` & `otpme-0.3.0a66/otpme/lib/help/token/fido2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/token/hotp.py` & `otpme-0.3.0a66/otpme/lib/help/token/hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/token/motp.py` & `otpme-0.3.0a66/otpme/lib/help/token/motp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/token/otp_push.py` & `otpme-0.3.0a66/otpme/lib/help/token/otp_push.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/token/otpme.py` & `otpme-0.3.0a66/otpme/lib/help/token/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/token/password.py` & `otpme-0.3.0a66/otpme/lib/help/token/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/token/ssh.py` & `otpme-0.3.0a66/otpme/lib/help/token/ssh.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/token/totp.py` & `otpme-0.3.0a66/otpme/lib/help/token/totp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/token/yubikey_hmac.py` & `otpme-0.3.0a66/otpme/lib/help/token/yubikey_hmac.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/token/yubikey_hotp.py` & `otpme-0.3.0a66/otpme/lib/help/token/yubikey_hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/tool.py` & `otpme-0.3.0a66/otpme/lib/help/tool.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/unit.py` & `otpme-0.3.0a66/otpme/lib/help/unit.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/help/user.py` & `otpme-0.3.0a66/otpme/lib/help/user.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/host.py` & `otpme-0.3.0a66/otpme/lib/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/humanize/units.py` & `otpme-0.3.0a66/otpme/lib/humanize/units.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/index/mysql.py` & `otpme-0.3.0a66/otpme/lib/index/mysql.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/index/postgres.py` & `otpme-0.3.0a66/otpme/lib/index/postgres.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/index/sqlite3.py` & `otpme-0.3.0a66/otpme/lib/index/sqlite3.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/job/callback.py` & `otpme-0.3.0a66/otpme/lib/job/callback.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/job/otpme_job.py` & `otpme-0.3.0a66/otpme/lib/job/otpme_job.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/join.py` & `otpme-0.3.0a66/otpme/lib/join.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/json.py` & `otpme-0.3.0a66/otpme/lib/json.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/jwt.py` & `otpme-0.3.0a66/otpme/lib/jwt.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/ldap/client.py` & `otpme-0.3.0a66/otpme/lib/ldap/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/ldap/schema.py` & `otpme-0.3.0a66/otpme/lib/ldap/schema.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/ldap/server.py` & `otpme-0.3.0a66/otpme/lib/ldap/server.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/locking.py` & `otpme-0.3.0a66/otpme/lib/locking.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/log.py` & `otpme-0.3.0a66/otpme/lib/log.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/messages.py` & `otpme-0.3.0a66/otpme/lib/messages.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/mschap.py` & `otpme-0.3.0a66/otpme/lib/mschap.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/mschap_util.py` & `otpme-0.3.0a66/otpme/lib/mschap_util.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/multiprocessing.py` & `otpme-0.3.0a66/otpme/lib/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/net.py` & `otpme-0.3.0a66/otpme/lib/net.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/nsscache.py` & `otpme-0.3.0a66/otpme/lib/nsscache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/offline_token.py` & `otpme-0.3.0a66/otpme/lib/offline_token.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/oid.py` & `otpme-0.3.0a66/otpme/lib/oid.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/otp/oath/hotp.py` & `otpme-0.3.0a66/otpme/lib/otp/oath/hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/otp/oath/totp.py` & `otpme-0.3.0a66/otpme/lib/otp/oath/totp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/otp/otpme/otpme.py` & `otpme-0.3.0a66/otpme/lib/otp/otpme/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/otp/yubico/yubiotp.py` & `otpme-0.3.0a66/otpme/lib/otp/yubico/yubiotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/otpme_acl.py` & `otpme-0.3.0a66/otpme/lib/otpme_acl.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/otpme_config.py` & `otpme-0.3.0a66/otpme/lib/otpme_config.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/otpme_pass.py` & `otpme-0.3.0a66/otpme/lib/otpme_pass.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/pam.py` & `otpme-0.3.0a66/otpme/lib/pam.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/pickle.py` & `otpme-0.3.0a66/otpme/lib/pickle.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/pinentry/pinentry.py` & `otpme-0.3.0a66/otpme/lib/pinentry/pinentry.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/pinentry/wrapper.py` & `otpme-0.3.0a66/otpme/lib/pinentry/wrapper.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/pki/cert.py` & `otpme-0.3.0a66/otpme/lib/pki/cert.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/pki/utils.py` & `otpme-0.3.0a66/otpme/lib/pki/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/pki/utils_openssl.py` & `otpme-0.3.0a66/otpme/lib/pki/utils_openssl.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/policy/__init__.py` & `otpme-0.3.0a66/otpme/lib/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/policy/authonaction/authonaction.py` & `otpme-0.3.0a66/otpme/lib/policy/authonaction/authonaction.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/policy/autodisable/autodisable.py` & `otpme-0.3.0a66/otpme/lib/policy/autodisable/autodisable.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/policy/defaultgroups/defaultgroups.py` & `otpme-0.3.0a66/otpme/lib/policy/defaultgroups/defaultgroups.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/policy/defaultpolicies/defaultpolicies.py` & `otpme-0.3.0a66/otpme/lib/policy/defaultpolicies/defaultpolicies.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/policy/defaultroles/defaultroles.py` & `otpme-0.3.0a66/otpme/lib/policy/defaultroles/defaultroles.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/policy/defaultunits/defaultunits.py` & `otpme-0.3.0a66/otpme/lib/policy/defaultunits/defaultunits.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/policy/forcetoken/forcetoken.py` & `otpme-0.3.0a66/otpme/lib/policy/forcetoken/forcetoken.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/policy/get_class.py` & `otpme-0.3.0a66/otpme/lib/policy/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/policy/idrange/idrange.py` & `otpme-0.3.0a66/otpme/lib/policy/idrange/idrange.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/policy/logintimes/logintimes.py` & `otpme-0.3.0a66/otpme/lib/policy/logintimes/logintimes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/policy/objecttemplates/objecttemplates.py` & `otpme-0.3.0a66/otpme/lib/policy/objecttemplates/objecttemplates.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/policy/password/password.py` & `otpme-0.3.0a66/otpme/lib/policy/password/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/policy/tokenacls/tokenacls.py` & `otpme-0.3.0a66/otpme/lib/policy/tokenacls/tokenacls.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/preload.py` & `otpme-0.3.0a66/otpme/lib/preload.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/progress.py` & `otpme-0.3.0a66/otpme/lib/progress.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/client/__init__.py` & `otpme-0.3.0a66/otpme/lib/protocols/client/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/client/agent1.py` & `otpme-0.3.0a66/otpme/lib/protocols/client/agent1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/client/auth1.py` & `otpme-0.3.0a66/otpme/lib/protocols/client/auth1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/client/cluster1.py` & `otpme-0.3.0a66/otpme/lib/protocols/client/cluster1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/client/get_class.py` & `otpme-0.3.0a66/otpme/lib/protocols/client/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/client/host1.py` & `otpme-0.3.0a66/otpme/lib/protocols/client/host1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/client/join1.py` & `otpme-0.3.0a66/otpme/lib/protocols/client/join1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/client/mgmt1.py` & `otpme-0.3.0a66/otpme/lib/protocols/client/mgmt1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/client/sync1.py` & `otpme-0.3.0a66/otpme/lib/protocols/client/sync1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/otpme_client.py` & `otpme-0.3.0a66/otpme/lib/protocols/otpme_client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/otpme_server.py` & `otpme-0.3.0a66/otpme/lib/protocols/otpme_server.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/request.py` & `otpme-0.3.0a66/otpme/lib/protocols/request.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/response.py` & `otpme-0.3.0a66/otpme/lib/protocols/response.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/server/__init__.py` & `otpme-0.3.0a66/otpme/lib/protocols/server/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/server/agent1.py` & `otpme-0.3.0a66/otpme/lib/protocols/server/agent1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/server/auth1.py` & `otpme-0.3.0a66/otpme/lib/protocols/server/auth1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/server/cluster1.py` & `otpme-0.3.0a66/otpme/lib/protocols/server/cluster1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/server/get_class.py` & `otpme-0.3.0a66/otpme/lib/protocols/server/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/server/host1.py` & `otpme-0.3.0a66/otpme/lib/protocols/server/host1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/server/join1.py` & `otpme-0.3.0a66/otpme/lib/protocols/server/join1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/server/mgmt1.py` & `otpme-0.3.0a66/otpme/lib/protocols/server/mgmt1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/server/sync1.py` & `otpme-0.3.0a66/otpme/lib/protocols/server/sync1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/status_codes.py` & `otpme-0.3.0a66/otpme/lib/protocols/status_codes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/protocols/utils.py` & `otpme-0.3.0a66/otpme/lib/protocols/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/push_script.py` & `otpme-0.3.0a66/otpme/lib/push_script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/qrcode.py` & `otpme-0.3.0a66/otpme/lib/qrcode.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/register/__init__.py` & `otpme-0.3.0a66/otpme/lib/register/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/resolver/get_class.py` & `otpme-0.3.0a66/otpme/lib/resolver/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/resolver/ldap/ldap.py` & `otpme-0.3.0a66/otpme/lib/resolver/ldap/ldap.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/script.py` & `otpme-0.3.0a66/otpme/lib/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/sign_key_cache.py` & `otpme-0.3.0a66/otpme/lib/sign_key_cache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/slp.py` & `otpme-0.3.0a66/otpme/lib/slp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/smartcard/__init__.py` & `otpme-0.3.0a66/otpme/lib/smartcard/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/smartcard/fido2/fido2.py` & `otpme-0.3.0a66/otpme/lib/smartcard/fido2/fido2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/smartcard/get_class.py` & `otpme-0.3.0a66/otpme/lib/smartcard/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/smartcard/utils.py` & `otpme-0.3.0a66/otpme/lib/smartcard/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/smartcard/yubikey/deploy.py` & `otpme-0.3.0a66/otpme/lib/smartcard/yubikey/deploy.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/smartcard/yubikey/usb.py` & `otpme-0.3.0a66/otpme/lib/smartcard/yubikey/usb.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/smartcard/yubikey/yubikey.py` & `otpme-0.3.0a66/otpme/lib/smartcard/yubikey/yubikey.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py` & `otpme-0.3.0a66/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py` & `otpme-0.3.0a66/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py` & `otpme-0.3.0a66/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/socket/connect.py` & `otpme-0.3.0a66/otpme/lib/socket/connect.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/socket/handler.py` & `otpme-0.3.0a66/otpme/lib/socket/handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/socket/listen.py` & `otpme-0.3.0a66/otpme/lib/socket/listen.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/socket/send_recv1.py` & `otpme-0.3.0a66/otpme/lib/socket/send_recv1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/sotp.py` & `otpme-0.3.0a66/otpme/lib/sotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/spsc.py` & `otpme-0.3.0a66/otpme/lib/spsc.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/srp.py` & `otpme-0.3.0a66/otpme/lib/srp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/ssh.py` & `otpme-0.3.0a66/otpme/lib/ssh.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/stuff.py` & `otpme-0.3.0a66/otpme/lib/stuff.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/sync_cache.py` & `otpme-0.3.0a66/otpme/lib/sync_cache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/system_command.py` & `otpme-0.3.0a66/otpme/lib/system_command.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/__init__.py` & `otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/advanced.py` & `otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/advanced.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/caching_query.py` & `otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/caching_query.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/environment.py` & `otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/environment.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/fixture_data.py` & `otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/fixture_data.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/helloworld.py` & `otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/helloworld.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/local_session_caching.py` & `otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/local_session_caching.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/model.py` & `otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/model.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/dogpile_caching/relationship_caching.py` & `otpme-0.3.0a66/otpme/lib/third_party/dogpile_caching/relationship_caching.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/nss_cache/__init__.py` & `otpme-0.3.0a66/otpme/lib/third_party/nss_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/nss_cache/caches/caches.py` & `otpme-0.3.0a66/otpme/lib/third_party/nss_cache/caches/caches.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/nss_cache/caches/files.py` & `otpme-0.3.0a66/otpme/lib/third_party/nss_cache/caches/files.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/nss_cache/config.py` & `otpme-0.3.0a66/otpme/lib/third_party/nss_cache/config.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/nss_cache/error.py` & `otpme-0.3.0a66/otpme/lib/third_party/nss_cache/error.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/nss_cache/lock.py` & `otpme-0.3.0a66/otpme/lib/third_party/nss_cache/lock.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/nss_cache/maps/group.py` & `otpme-0.3.0a66/otpme/lib/third_party/nss_cache/maps/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/nss_cache/maps/maps.py` & `otpme-0.3.0a66/otpme/lib/third_party/nss_cache/maps/maps.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/nss_cache/maps/passwd.py` & `otpme-0.3.0a66/otpme/lib/third_party/nss_cache/maps/passwd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/nss_cache/maps/shadow.py` & `otpme-0.3.0a66/otpme/lib/third_party/nss_cache/maps/shadow.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/nss_cache/nss.py` & `otpme-0.3.0a66/otpme/lib/third_party/nss_cache/nss.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/nss_cache/update/files_updater.py` & `otpme-0.3.0a66/otpme/lib/third_party/nss_cache/update/files_updater.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/nss_cache/update/map_updater.py` & `otpme-0.3.0a66/otpme/lib/third_party/nss_cache/update/map_updater.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/nss_cache/update/updater.py` & `otpme-0.3.0a66/otpme/lib/third_party/nss_cache/update/updater.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/nss_cache/util/file_formats.py` & `otpme-0.3.0a66/otpme/lib/third_party/nss_cache/util/file_formats.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/oath_toolkit/_compat.py` & `otpme-0.3.0a66/otpme/lib/third_party/oath_toolkit/_compat.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/third_party/oath_toolkit/uri.py` & `otpme-0.3.0a66/otpme/lib/third_party/oath_toolkit/uri.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/token/__init__.py` & `otpme-0.3.0a66/otpme/lib/token/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/token/fido2/fido2.py` & `otpme-0.3.0a66/otpme/lib/token/fido2/fido2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/token/get_class.py` & `otpme-0.3.0a66/otpme/lib/token/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/token/hotp/hotp.py` & `otpme-0.3.0a66/otpme/lib/token/hotp/hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/token/link/link.py` & `otpme-0.3.0a66/otpme/lib/token/link/link.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/token/motp/motp.py` & `otpme-0.3.0a66/otpme/lib/token/motp/motp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/token/oath/oath.py` & `otpme-0.3.0a66/otpme/lib/token/oath/oath.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/token/otp_push/otp_push.py` & `otpme-0.3.0a66/otpme/lib/token/otp_push/otp_push.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/token/otpme/otpme.py` & `otpme-0.3.0a66/otpme/lib/token/otpme/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/token/password/password.py` & `otpme-0.3.0a66/otpme/lib/token/password/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/token/script_otp/script_otp.py` & `otpme-0.3.0a66/otpme/lib/token/script_otp/script_otp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/token/script_static/script_static.py` & `otpme-0.3.0a66/otpme/lib/token/script_static/script_static.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/token/ssh/ssh.py` & `otpme-0.3.0a66/otpme/lib/token/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/token/totp/totp.py` & `otpme-0.3.0a66/otpme/lib/token/totp/totp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme/lib/token/yubikey_hmac/yubikey_hmac.py` & `otpme-0.3.0a66/otpme/lib/token/yubikey_hmac/yubikey_hmac.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme.egg-info/PKG-INFO` & `otpme-0.3.0a66/otpme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otpme
-Version: 0.3.0a65
+Version: 0.3.0a66
 Summary: OTPme: A flexible One-Time-Password system.
 Home-page: http://www.otpme.org
 Author: the2nd
 Author-email: the2nd@otpme.org
 Maintainer: the2nd
 Maintainer-email: the2nd@otpme.org
 License: GPLv2
```

### Comparing `otpme-0.3.0a65/otpme.egg-info/SOURCES.txt` & `otpme-0.3.0a66/otpme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme.egg-info/entry_points.txt` & `otpme-0.3.0a66/otpme.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/otpme.egg-info/requires.txt` & `otpme-0.3.0a66/otpme.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a65/setup.py` & `otpme-0.3.0a66/setup.py`

 * *Files identical despite different names*

