# Comparing `tmp/resc_backend-3.2.2.tar.gz` & `tmp/resc_backend-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_backend-3.2.2.tar", last modified: Fri May 17 12:04:39 2024, max compression
+gzip compressed data, was "resc_backend-3.3.0.tar", last modified: Fri May 24 15:29:42 2024, max compression
```

## Comparing `resc_backend-3.2.2.tar` & `resc_backend-3.3.0.tar`

### file list

```diff
@@ -1,118 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:39.440496 resc_backend-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-17 12:04:35.000000 resc_backend-3.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-17 12:04:39.440496 resc_backend-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-17 12:04:35.000000 resc_backend-3.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-17 12:04:35.000000 resc_backend-3.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-17 12:04:35.000000 resc_backend-3.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-17 12:04:39.444496 resc_backend-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-17 12:04:35.000000 resc_backend-3.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:39.424496 resc_backend-3.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:39.428496 resc_backend-3.2.2/src/resc_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:39.428496 resc_backend-3.2.2/src/resc_backend/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/bin/rabbitmq_bootup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:39.428496 resc_backend-3.2.2/src/resc_backend/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/db/engine_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:39.432496 resc_backend-3.2.2/src/resc_backend/db/model/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/db/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/db/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/db/model/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/db/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/db/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/db/model/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/db/model/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/db/model/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/db/model/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/db/model/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/db/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/db/model/vcs_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:39.432496 resc_backend-3.2.2/src/resc_backend/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/helpers/dict_remapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/helpers/environment_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:39.432496 resc_backend-3.2.2/src/resc_backend/helpers/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/helpers/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/helpers/rabbitmq/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:39.432496 resc_backend-3.2.2/src/resc_backend/resc_web_service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:39.436496 resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)    32592 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:39.436496 resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
--rw-r--r--   0 runner    (1001) docker     (127)    17792 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/health.py
--rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    20445 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    17302 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    14911 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:39.436496 resc_backend-3.2.2/src/resc_backend/resc_web_service/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/helpers/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/helpers/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/helpers/toml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:39.440496 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/audit_count_over_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/date_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/date_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/finding_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/finding_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/pagination_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/personal_audit_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/repository_enriched.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/rule_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/status_count.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/time_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/vcs_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:39.440496 resc_backend-3.2.2/src/resc_backend/resc_web_service_interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service_interface/findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service_interface/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service_interface/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service_interface/scans.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-17 12:04:35.000000 resc_backend-3.2.2/src/resc_backend/resc_web_service_interface/vcs_instances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:04:39.440496 resc_backend-3.2.2/src/resc_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-17 12:04:39.000000 resc_backend-3.2.2/src/resc_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-17 12:04:39.000000 resc_backend-3.2.2/src/resc_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:04:39.000000 resc_backend-3.2.2/src/resc_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-17 12:04:39.000000 resc_backend-3.2.2/src/resc_backend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:04:39.000000 resc_backend-3.2.2/src/resc_backend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-17 12:04:39.000000 resc_backend-3.2.2/src/resc_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 12:04:39.000000 resc_backend-3.2.2/src/resc_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.221480 resc_backend-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-24 15:29:36.000000 resc_backend-3.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-24 15:29:42.221480 resc_backend-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-24 15:29:36.000000 resc_backend-3.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-24 15:29:36.000000 resc_backend-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-24 15:29:36.000000 resc_backend-3.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-24 15:29:42.221480 resc_backend-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-24 15:29:36.000000 resc_backend-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.189479 resc_backend-3.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.193479 resc_backend-3.3.0/src/resc_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.197480 resc_backend-3.3.0/src/resc_backend/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/bin/rabbitmq_bootup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.197480 resc_backend-3.3.0/src/resc_backend/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/engine_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.197480 resc_backend-3.3.0/src/resc_backend/db/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/db/model/vcs_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.197480 resc_backend-3.3.0/src/resc_backend/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/helpers/dict_remapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/helpers/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/helpers/list_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.197480 resc_backend-3.3.0/src/resc_backend/helpers/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/helpers/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/helpers/rabbitmq/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.201480 resc_backend-3.3.0/src/resc_backend/resc_web_service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.201480 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36235 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.205479 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17780 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20433 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17302 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16686 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.205479 resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/toml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.217480 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/audit_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/date_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/date_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/finding_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/finding_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/pagination_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/personal_audit_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/repository_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/rule_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/status_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/time_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/vcs_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.217480 resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-24 15:29:36.000000 resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/vcs_instances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:29:42.217480 resc_backend-3.3.0/src/resc_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-24 15:29:42.000000 resc_backend-3.3.0/src/resc_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-24 15:29:42.000000 resc_backend-3.3.0/src/resc_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:29:42.000000 resc_backend-3.3.0/src/resc_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-24 15:29:42.000000 resc_backend-3.3.0/src/resc_backend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:29:42.000000 resc_backend-3.3.0/src/resc_backend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-24 15:29:42.000000 resc_backend-3.3.0/src/resc_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 15:29:42.000000 resc_backend-3.3.0/src/resc_backend.egg-info/top_level.txt
```

### Comparing `resc_backend-3.2.2/LICENSE.md` & `resc_backend-3.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/PKG-INFO` & `resc_backend-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_backend
-Version: 3.2.2
+Version: 3.3.0
 Summary: Repository Scanner - Backend
 Home-page: https://github.com/abnamro/resc-backend
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `resc_backend-3.2.2/README.md` & `resc_backend-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/pyproject.toml` & `resc_backend-3.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/setup.cfg` & `resc_backend-3.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_backend
 description = Repository Scanner - Backend
-version = 3.2.2
+version = 3.3.0
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/abnamro/resc-backend
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE.md
```

### Comparing `resc_backend-3.2.2/src/resc_backend/bin/rabbitmq_bootup.py` & `resc_backend-3.3.0/src/resc_backend/bin/rabbitmq_bootup.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/constants.py` & `resc_backend-3.3.0/src/resc_backend/constants.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/db/connection.py` & `resc_backend-3.3.0/src/resc_backend/db/connection.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/db/engine_azure.py` & `resc_backend-3.3.0/src/resc_backend/db/engine_azure.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/db/model/__init__.py` & `resc_backend-3.3.0/src/resc_backend/db/model/__init__.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/db/model/audit.py` & `resc_backend-3.3.0/src/resc_backend/db/model/audit.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,7 +58,22 @@
             auditor=auditor,
             status=status,
             comment=sanitized_comment,
             timestamp=timestamp,
             is_latest=is_latest,
         )
         return db_audit
+
+    @staticmethod
+    def create_automated(
+        finding_id: int,
+        status: str,
+    ):
+        db_audit = DBaudit(
+            finding_id=finding_id,
+            status=status,
+            comment="automated",
+            auditor="resc",
+            timestamp=datetime.now(UTC),
+            is_latest=True,
+        )
+        return db_audit
```

### Comparing `resc_backend-3.2.2/src/resc_backend/db/model/finding.py` & `resc_backend-3.3.0/src/resc_backend/db/model/finding.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 # Standard Library
 from datetime import datetime, UTC
 
 # Third Party
-from sqlalchemy import (
-    Column,
-    DateTime,
-    ForeignKey,
-    Integer,
-    String,
-    Text,
-    UniqueConstraint,
-)
+from sqlalchemy import Column, DateTime, ForeignKey, Integer, String, Text, UniqueConstraint, Boolean
 
 # First Party
 from resc_backend.db.model import Base
 
 
 class DBfinding(Base):
     __tablename__ = "finding"
@@ -27,14 +19,15 @@
     column_end = Column(Integer, nullable=False, default=0)
     commit_id = Column(String(120))
     commit_message = Column(Text)
     commit_timestamp = Column(DateTime, default=datetime.now(UTC).isoformat())
     author = Column(String(200))
     email = Column(String(100))
     event_sent_on = Column(DateTime, nullable=True)
+    is_dir_scan = Column(Boolean, nullable=False, default=False)
 
     __table_args__ = (
         UniqueConstraint(
             "commit_id",
             "repository_id",
             "rule_name",
             "file_path",
@@ -43,50 +36,53 @@
             "column_end",
             name="uc_finding_per_repository",
         ),
     )
 
     def __init__(
         self,
-        rule_name,
-        file_path,
-        line_number,
-        commit_id,
-        commit_message,
-        commit_timestamp,
-        author,
-        email,
-        event_sent_on,
-        repository_id,
-        column_start,
-        column_end,
+        rule_name: str,
+        file_path: str,
+        line_number: int,
+        commit_id: str,
+        commit_message: str,
+        commit_timestamp: datetime,
+        author: str,
+        email: str,
+        event_sent_on: datetime,
+        repository_id: int,
+        column_start: int,
+        column_end: int,
+        is_dir_scan: bool = False,
     ):
         self.email = email
         self.author = author
         self.commit_timestamp = commit_timestamp
         self.commit_message = commit_message
         self.commit_id = commit_id
         self.line_number = line_number
         self.file_path = file_path
         self.rule_name = rule_name
         self.event_sent_on = event_sent_on
         self.repository_id = repository_id
         self.column_start = column_start
         self.column_end = column_end
+        self.is_dir_scan = is_dir_scan
 
     @staticmethod
-    def create_from_finding(finding):
+    def create_from_finding(finding, is_dir_scan: bool = False):
         db_finding = DBfinding(
             rule_name=finding.rule_name,
             file_path=finding.file_path,
             line_number=finding.line_number,
             email=finding.email,
             commit_id=finding.commit_id,
             commit_message=finding.commit_message,
             commit_timestamp=finding.commit_timestamp,
             author=finding.author,
             event_sent_on=finding.event_sent_on,
             repository_id=finding.repository_id,
             column_start=finding.column_start,
             column_end=finding.column_end,
+            is_dir_scan=is_dir_scan,
         )
         return db_finding
```

### Comparing `resc_backend-3.2.2/src/resc_backend/db/model/repository.py` & `resc_backend-3.3.0/src/resc_backend/db/model/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/db/model/rule.py` & `resc_backend-3.3.0/src/resc_backend/db/model/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/db/model/rule_allow_list.py` & `resc_backend-3.3.0/src/resc_backend/db/model/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/db/model/rule_pack.py` & `resc_backend-3.3.0/src/resc_backend/db/model/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/db/model/scan.py` & `resc_backend-3.3.0/src/resc_backend/db/model/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/db/model/vcs_instance.py` & `resc_backend-3.3.0/src/resc_backend/db/model/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/helpers/dict_remapper.py` & `resc_backend-3.3.0/src/resc_backend/helpers/dict_remapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 # Standard Library
 from functools import reduce
 
 
+def _remapper0(val):
+    return val[0]
+
+
+def _remapper1(val):
+    return val[1]
+
+
 def remap_dict_keys(input_dict: dict, transformation_map: list):
-    new_keys = [val[1] for val in transformation_map]
+    new_keys = list(map(_remapper1, transformation_map))
     for old_key, new_key in transformation_map:
         create_nested_dictionary(input_dict, new_key, get_value_from_nested_dictionary(input_dict, *old_key))
 
-    output_dict = {k: v for k, v in input_dict.items() if k in [key[0] for key in new_keys]}
+    new_keys_mapped = list(map(_remapper0, new_keys))
+    output_dict = {k: v for k, v in input_dict.items() if k in new_keys_mapped}
 
     return output_dict
 
 
 def create_nested_dictionary(dictionary, keys, value):
     for key in keys[:-1]:
         dictionary = dictionary.setdefault(key, {})
     if not isinstance(dictionary, dict):
         dictionary = {}
         dictionary = dictionary.setdefault(keys[-1], {})
     dictionary[keys[-1]] = value
 
 
+def _reducer(d, key):
+    return d.get(key) if d else None
+
+
 def get_value_from_nested_dictionary(dictionary, *keys):
-    return reduce(lambda d, key: d.get(key) if d else None, keys, dictionary)
+    return reduce(_reducer, keys, dictionary)
 
 
 def delete_keys_from_nested_dict(dict_del, lst_keys):
     if not lst_keys:
         return
     if len(lst_keys) == 1:
         del dict_del[lst_keys[0]]
```

### Comparing `resc_backend-3.2.2/src/resc_backend/helpers/environment_wrapper.py` & `resc_backend-3.3.0/src/resc_backend/helpers/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/helpers/rabbitmq/configuration.py` & `resc_backend-3.3.0/src/resc_backend/helpers/rabbitmq/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py` & `resc_backend-3.3.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/api.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Standard Library
 import logging.config
+from contextlib import asynccontextmanager
 
 # Third Party
 from fastapi import Depends, FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 from starlette.responses import RedirectResponse
 from starlette.status import HTTP_302_FOUND
 from tenacity import RetryError
 
 # First Party
-from resc_backend.common import get_package_version
 from resc_backend.constants import RWS_VERSION_PREFIX
 from resc_backend.db.connection import Session, engine
 from resc_backend.helpers.environment_wrapper import validate_environment
 from resc_backend.resc_web_service.configuration import (
     AUTHENTICATION_REQUIRED,
     CORS_ALLOWED_DOMAINS,
     ENABLE_CORS,
@@ -107,20 +107,28 @@
     {"name": "resc-metrics", "description": "Retrieve metrics"},
 ]
 
 # Check if authentication is required for api endpoints
 auth_disabled = env_variables[AUTHENTICATION_REQUIRED].lower() in ["false"]
 AUTH = [Depends(requires_no_auth)] if auth_disabled else [Depends(requires_auth)]
 
+
+@asynccontextmanager
+async def lifespan(_: FastAPI):
+    app_startup()
+    yield
+    await app_shutdown()
+
+
 app = FastAPI(
     title="Repository Scanner (RESC)",
     description="RESC API helps you to perform several operations upon findings "
     "obtained from multiple source code repositories.",
-    version=get_package_version(),
     openapi_tags=tags_metadata,
+    lifespan=lifespan,
 )
 
 if env_variables[ENABLE_CORS].lower() in ["true"]:
     origins = env_variables[CORS_ALLOWED_DOMAINS].split(", ")
     app.add_middleware(
         CORSMiddleware,
         allow_origins=origins,
@@ -143,27 +151,25 @@
 # Apply the security headers to the app in the form of middleware
 app.middleware("http")(add_security_headers)
 
 # Add exception handlers
 add_exception_handlers(app=app)
 
 
-@app.on_event("startup")
 def app_startup():
     CacheManager.initialize_cache(env_variables=env_variables)
     try:
         _ = Session(bind=engine)
         check_db_initialized()
 
         logger.info("Database is connected, expected table(s) found")
     except RetryError as exc:
         raise SystemExit("Error while connecting to the database, retry timed out") from exc
 
 
-@app.on_event("shutdown")
 async def app_shutdown():
     await CacheManager.clear_all_cache()
 
 
 @app.get("/")
 def view_docs():
     return RedirectResponse(url="/docs", status_code=HTTP_302_FOUND)
```

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/cache_manager.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/cache_manager.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/configuration.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/audit.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/audit.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,14 +61,35 @@
     db_connection.add(db_audit)
     db_connection.commit()
     db_connection.refresh(db_audit)
 
     return db_audit
 
 
+def create_automated_audit(db_connection: Session, findings_ids: list[int], status: FindingStatus) -> list[DBaudit]:
+    """
+        Create automated audit for a list of findings.
+
+    Args:
+        db_connection (Session): Session of the database connection
+        findings_ids (list[int]): list of id to audit
+        status (FindingStatus): status to apply
+
+    Returns:
+        list[DBaudit]: newly created audits
+    """
+    db_audits = [DBaudit.create_automated(finding_id, status) for finding_id in findings_ids]
+    db_connection.add_all(db_audits)
+    db_connection.commit()
+
+    logger.debug(f"Automated audit of {len(db_audits)} findings.")
+
+    return db_audits
+
+
 def get_finding_audits(
     db_connection: Session,
     finding_id: int,
     skip: int = 0,
     limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT,
 ) -> list[DBaudit]:
     """
```

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/detailed_finding.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/detailed_finding.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,14 +198,15 @@
         DBfinding.column_start,
         DBfinding.column_end,
         DBfinding.commit_id,
         DBfinding.commit_message,
         DBfinding.commit_timestamp,
         DBfinding.author,
         DBfinding.email,
+        DBfinding.is_dir_scan,
         DBaudit.status,
         DBaudit.comment,
         DBfinding.rule_name,
         DBscan.rule_pack,
         DBfinding.event_sent_on,
         DBscan.timestamp,
         DBscan.id_.label("scan_id"),
@@ -290,14 +291,15 @@
             DBfinding.column_start,
             DBfinding.column_end,
             DBfinding.commit_id,
             DBfinding.commit_message,
             DBfinding.commit_timestamp,
             DBfinding.author,
             DBfinding.email,
+            DBfinding.is_dir_scan,
             DBaudit.status,
             DBaudit.comment,
             DBfinding.rule_name,
             DBscan.rule_pack,
             DBscan.timestamp,
             DBscan.id_.label("scan_id"),
             DBscan.last_scanned_commit,
```

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/finding.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/finding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Standard Library
 import logging
 from datetime import datetime, timedelta, UTC
 
 # Third Party
-from sqlalchemy import extract, func, union
+from sqlalchemy import extract, func, select, union
 from sqlalchemy.engine import Row
 from sqlalchemy.orm import Session
 from sqlalchemy.orm.query import Query
 from sqlalchemy.sql.expression import literal_column
 
 # First Party
 from resc_backend.constants import (
@@ -21,14 +21,15 @@
     DBrule,
     DBruleTag,
     DBscan,
     DBscanFinding,
     DBtag,
     DBVcsInstance,
 )
+from resc_backend.helpers.list_mapper import dict_of_list
 from resc_backend.resc_web_service.crud import scan_finding as scan_finding_crud
 from resc_backend.resc_web_service.filters import FindingsFilter
 from resc_backend.resc_web_service.schema import finding as finding_schema
 from resc_backend.resc_web_service.schema.date_filter import DateFilter
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
@@ -44,47 +45,45 @@
         setattr(db_finding, key, finding_update_dict[key])
 
     db_connection.commit()
     db_connection.refresh(db_finding)
     return db_finding
 
 
+def _long_key(finding: DBfinding | finding_schema.FindingCreate) -> str:
+    key = (
+        f"{finding.commit_id}|{finding.rule_name}|{finding.file_path}"
+        + f"|{finding.line_number}|{finding.column_start}|{finding.column_end}"
+    )
+    return key
+
+
 def create_findings(db_connection: Session, findings: list[finding_schema.FindingCreate]) -> list[DBfinding]:
     if len(findings) < 1:
         # Function is called with an empty list of findings
         return []
 
     repository_id = findings[0].repository_id
 
     # get a list of known / registered findings for this repository
     query = db_connection.query(DBfinding)
     query = query.where(DBfinding.repository_id == repository_id)
     db_repository_findings = query.all()
 
-    # Compare new findings list with findings in the db
-    new_findings = findings[:]
-    db_findings = []
-    for finding in findings:
-        for repository_finding in db_repository_findings:
-            # Compare based on the unique key in the findings table
-            if (
-                repository_finding.commit_id == finding.commit_id
-                and repository_finding.rule_name == finding.rule_name
-                and repository_finding.file_path == finding.file_path
-                and repository_finding.line_number == finding.line_number
-                and repository_finding.column_start == finding.column_start
-                and repository_finding.column_end == finding.column_end
-            ):
-                # Store the already known finding
-                db_findings.append(repository_finding)
-                # Remove from the db_repository_findings to increase performance for the next loop
-                db_repository_findings.remove(repository_finding)
-                # Remove from the to be created findings
-                new_findings.remove(finding)
-                break
+    map_repository_finding: dict[str, DBfinding] = dict_of_list(_long_key, db_repository_findings)
+    map_findings: dict[str, finding_schema.FindingCreate] = dict_of_list(_long_key, findings)
+
+    intersection = map_findings.keys() & map_repository_finding.keys()
+
+    db_findings: list[DBfinding] = []
+    for key in intersection:
+        db_findings.append(map_repository_finding.get(key))
+        del map_findings[key]
+
+    new_findings: list[finding_schema.FindingCreate] = map_findings.values()
     logger.info(
         f"create_findings repository {repository_id}, Requested: {len(findings)}. "
         f"New findings: {len(new_findings)}. Already in db: {len(db_findings)}"
     )
 
     db_create_findings = []
     # Map the to be created findings to the DBfinding type object
@@ -97,14 +96,86 @@
         db_connection.flush()
         db_connection.commit()
         db_findings.extend(db_create_findings)
     # Return the known findings that are part of the request and the newly created findings
     return db_findings
 
 
+def _short_key(finding: DBfinding | finding_schema.FindingCreate) -> str:
+    return f"{finding.rule_name}|{finding.file_path}|{finding.line_number}|{finding.column_start}|{finding.column_end}"
+
+
+def create_or_update_findings(db_connection: Session, findings: list[finding_schema.FindingCreate]) -> list[DBfinding]:
+    """
+    Create or update findings.
+    This is used in the case of rules which are applied to directories.
+
+    Args:
+        db_connection (Session): connection to DB
+        findings (list[finding_schema.FindingCreate]): list of findings to create or update
+        db_scan (DBscan): current scan (used for the new commit ID)
+
+    Returns:
+        list[DBfinding]: list of created findings
+    """
+    if len(findings) < 1:
+        # Function is called with an empty list of findings
+        return []
+
+    repository_id = findings[0].repository_id
+
+    # get a list of known / registered findings for this repository
+    query = db_connection.query(DBfinding)
+    query = query.where(DBfinding.repository_id == repository_id)
+    db_repository_findings = query.all()
+
+    map_repository_finding: dict[str, DBfinding] = dict_of_list(_short_key, db_repository_findings)
+    map_findings: dict[str, finding_schema.FindingCreate] = dict_of_list(_short_key, findings)
+
+    intersection = map_findings.keys() & map_repository_finding.keys()
+
+    db_findings: list[DBfinding] = []
+    for key in intersection:
+        repository_finding = map_repository_finding.get(key)
+        finding = map_findings.get(key)
+        repository_finding.commit_id = finding.commit_id
+        repository_finding.commit_message = finding.commit_message
+        repository_finding.commit_timestamp = finding.commit_timestamp
+        repository_finding.author = finding.author
+        repository_finding.is_dir_scan = True
+        db_findings.append(repository_finding)
+        del map_findings[key]
+
+    new_findings: list[finding_schema.FindingCreate] = map_findings.values()
+
+    logger.info(
+        f"create_or_update_findings repository {repository_id}, Requested: {len(findings)}. "
+        f"New findings: {len(new_findings)}. Already in db: {len(db_findings)}"
+    )
+
+    db_create_findings = []
+    # Map the to be created findings to the DBfinding type object
+    for new_finding in new_findings:
+        db_create_finding = DBfinding.create_from_finding(new_finding, is_dir_scan=True)
+        db_create_findings.append(db_create_finding)
+
+    # Store all the to be created findings in the database
+    if len(db_create_findings) >= 1:
+        db_connection.add_all(db_create_findings)
+
+    if len(db_findings) > 0 or len(db_create_findings) > 0:
+        db_connection.flush()
+        db_connection.commit()
+
+    db_findings.extend(db_create_findings)
+
+    # Return the known findings that are part of the request and the newly created findings
+    return db_findings
+
+
 def get_finding(db_connection: Session, finding_id: int):
     finding = db_connection.query(DBfinding)
     finding = finding.where(DBfinding.id_ == finding_id).first()
     return finding
 
 
 def get_findings(db_connection: Session, skip: int = 0, limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT):
@@ -169,14 +240,43 @@
 
     query = query.order_by(DBfinding.id_)
     query = query.offset(skip).limit(limit_val)
     findings = query.all()
     return findings
 
 
+def get_findings_from_repo_of_scan_as_dir(db_connection: Session, scan: DBscan) -> list[int]:
+    """
+    Retrieve all the findings which are:
+     - tied to the repository of the scan
+     - for the rule pack of the scan
+     - which are not tied to the scan (in other words out-dated)
+
+    Args:
+        db_connection (Session): session
+        scan (DBscan): scan to restrict with
+
+    Returns:
+        list[int]: list of ids of findings which are to be audited
+    """
+
+    query = select(DBfinding.id_)
+    query = query.join(DBrule, DBrule.rule_name == DBfinding.rule_name)
+    query = query.where(DBrule.rule_pack == scan.rule_pack)
+    query = query.where(DBfinding.repository_id == scan.repository_id)
+    query = query.where(DBfinding.is_dir_scan == True)  # noqa: E712
+
+    sub_query: Query = select(DBscanFinding.finding_id)
+    sub_query = sub_query.where(DBscanFinding.scan_id == scan.id_)
+    sub_query = sub_query.subquery()
+    query = query.where(DBfinding.id_.not_in(sub_query))
+
+    return db_connection.execute(query).scalars().all()
+
+
 def get_total_findings_count(db_connection: Session, findings_filter: FindingsFilter = None) -> int:
     """
         Retrieve count of finding records of a given scan
     :param findings_filter:
     :param db_connection:
         Session of the database connection
     :return: total_count
```

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/repository.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/rule.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/rule.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,14 +30,36 @@
     rule_query = db_connection.query(DBrule)
     rule_query = rule_query.join(DBscan, DBscan.rule_pack == DBrule.rule_pack)
     rule_query = rule_query.where(DBscan.id_ == scan_id)
     rules: list[RuleRead] = rule_query.all()
     return rules
 
 
+def get_scan_as_dir_rules_by_scan_id(db_connection: Session, scan_id: int) -> list[str]:
+    """
+        Fetch rules applied as directory by rule pack version
+    :param db_connection:
+        Session of the database connection
+    :param rule_pack_version:
+        rule pack version
+    :return: List[str]
+        The output contains list of strings of rules which are applied as directory
+    """
+    query: Query = select(DBrule.rule_name)
+    query = query.join(DBscan, DBscan.rule_pack == DBrule.rule_pack)
+    query = query.join(DBruleTag, DBruleTag.rule_id == DBrule.id_)
+    query = query.join(DBtag, DBtag.id_ == DBruleTag.tag_id)
+    query = query.where(DBscan.id_ == scan_id)
+    # We could make this a parameter later, but for now it is simpler. KISS
+    query = query.where(DBtag.name == RULE_TAG_SCAN_AS_DIR)
+    db_rules = db_connection.execute(query).scalars().all()
+
+    return db_rules
+
+
 def create_rule_allow_list(db_connection: Session, rule_allow_list: rule_allow_list_schema.RuleAllowList):
     """
         Create rule allow list in database
     :param db_connection:
         Session of the database connection
     :param rule_allow_list:
         RuleAllowList object to be created
```

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/rule_pack.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/rule_tag.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/rule_tag.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/scan.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/scan_finding.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/scan_finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/crud/vcs_instance.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/crud/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/dependencies.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/dependencies.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/common.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/common.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/detailed_findings.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 import json
 import logging
 import urllib.parse
 
 # Third Party
 from fastapi import APIRouter, Depends, HTTPException, Query, status
 from fastapi_cache.decorator import cache
+from sqlalchemy.orm import Session
 
 # First Party
 from resc_backend.constants import (
     CACHE_NAMESPACE_FINDING,
     DEFAULT_RECORDS_PER_PAGE_LIMIT,
     ERROR_MESSAGE_500,
     ERROR_MESSAGE_503,
     FINDINGS_TAG,
     REDIS_CACHE_EXPIRE,
     RWS_ROUTE_DETAILED_FINDINGS,
 )
-from resc_backend.db.connection import Session
 from resc_backend.resc_web_service.crud import detailed_finding as detailed_finding_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
 from resc_backend.resc_web_service.filters import FindingsFilter
 from resc_backend.resc_web_service.helpers.resc_swagger_models import Model404
 from resc_backend.resc_web_service.schema import (
     detailed_finding as detailed_finding_schema,
 )
```

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/findings.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/findings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Standard Library
 from datetime import datetime
 
 # Third Party
 from fastapi import APIRouter, Depends, HTTPException, Query, Request, status
 from fastapi_cache.decorator import cache
+from sqlalchemy.orm import Session
 
 # First Party
 from resc_backend.constants import (
     CACHE_NAMESPACE_FINDING,
     CACHE_NAMESPACE_FINDING_STATUS,
     CACHE_NAMESPACE_RULE,
     DEFAULT_RECORDS_PER_PAGE_LIMIT,
@@ -18,15 +19,14 @@
     RWS_ROUTE_AUDIT,
     RWS_ROUTE_BY_RULE,
     RWS_ROUTE_COUNT_BY_TIME,
     RWS_ROUTE_FINDINGS,
     RWS_ROUTE_SUPPORTED_STATUSES,
     RWS_ROUTE_TOTAL_COUNT_BY_RULE,
 )
-from resc_backend.db.connection import Session
 from resc_backend.resc_web_service.cache_manager import CacheManager
 from resc_backend.resc_web_service.crud import audit as audit_crud
 from resc_backend.resc_web_service.crud import finding as finding_crud
 from resc_backend.resc_web_service.crud import scan_finding as scan_finding_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
 from resc_backend.resc_web_service.filters import FindingsFilter
 from resc_backend.resc_web_service.helpers.resc_swagger_models import Model400, Model404
```

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/health.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/metrics.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/metrics.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/repositories.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/repositories.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Standard Library
 
 # Third Party
 from fastapi import APIRouter, Depends, HTTPException, Query, status
 from fastapi_cache.decorator import cache
+from sqlalchemy.orm import Session
 
 # First Party
 from resc_backend.constants import (
     CACHE_NAMESPACE_FINDING,
     CACHE_NAMESPACE_REPOSITORY,
     DEFAULT_RECORDS_PER_PAGE_LIMIT,
     ERROR_MESSAGE_500,
@@ -16,15 +17,14 @@
     RWS_ROUTE_DISTINCT_PROJECTS,
     RWS_ROUTE_DISTINCT_REPOSITORIES,
     RWS_ROUTE_FINDINGS_METADATA,
     RWS_ROUTE_LAST_SCAN,
     RWS_ROUTE_REPOSITORIES,
     RWS_ROUTE_SCANS,
 )
-from resc_backend.db.connection import Session
 from resc_backend.resc_web_service.cache_manager import CacheManager
 from resc_backend.resc_web_service.crud import repository as repository_crud
 from resc_backend.resc_web_service.crud import scan as scan_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
 from resc_backend.resc_web_service.helpers.resc_swagger_models import Model404
 from resc_backend.resc_web_service.schema import repository as repository_schema
 from resc_backend.resc_web_service.schema import (
```

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/rule_packs.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/rules.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Standard Library
 import logging
 from datetime import datetime
 
 # Third Party
 from fastapi import APIRouter, Depends, Query, status
 from fastapi_cache.decorator import cache
+from sqlalchemy.orm import Session
 
 # First Party
 from resc_backend.constants import (
     CACHE_NAMESPACE_FINDING,
     CACHE_NAMESPACE_RULE,
     ERROR_MESSAGE_500,
     ERROR_MESSAGE_503,
     REDIS_CACHE_EXPIRE,
     RULES_TAG,
     RWS_ROUTE_DETECTED_RULES,
     RWS_ROUTE_FINDING_STATUS_COUNT,
     RWS_ROUTE_RULES,
 )
-from resc_backend.db.connection import Session
 from resc_backend.resc_web_service.crud import finding as finding_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
 from resc_backend.resc_web_service.schema.rule_count_model import RuleFindingCountModel
 from resc_backend.resc_web_service.schema.status_count import StatusCount
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
```

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/scans.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/scans.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # Standard Library
 import logging
 
 # Third Party
 from fastapi import APIRouter, Depends, HTTPException, Query, status
 from sqlalchemy.exc import IntegrityError
+from sqlalchemy.orm import Session
 
 # First Party
 from resc_backend.constants import (
     CACHE_NAMESPACE_FINDING,
     CACHE_NAMESPACE_RULE,
     DEFAULT_RECORDS_PER_PAGE_LIMIT,
     ERROR_MESSAGE_500,
     ERROR_MESSAGE_503,
     RWS_ROUTE_DETECTED_RULES,
     RWS_ROUTE_FINDINGS,
     RWS_ROUTE_SCANS,
     SCANS_TAG,
 )
-from resc_backend.db.connection import Session
-from resc_backend.db.model import DBscanFinding
+from resc_backend.db.model import DBscanFinding, DBfinding, DBscan
 from resc_backend.resc_web_service.cache_manager import CacheManager
+from resc_backend.resc_web_service.crud import audit as audit_crud
 from resc_backend.resc_web_service.crud import finding as finding_crud
 from resc_backend.resc_web_service.crud import scan as scan_crud
+from resc_backend.resc_web_service.crud import rule as rule_crud
 from resc_backend.resc_web_service.crud import scan_finding as scan_finding_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
 from resc_backend.resc_web_service.filters import FindingsFilter
 from resc_backend.resc_web_service.helpers.resc_swagger_models import Model400, Model404
 from resc_backend.resc_web_service.schema import finding as finding_schema
 from resc_backend.resc_web_service.schema import scan as scan_schema
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
@@ -91,15 +93,17 @@
     - **timestamp**: creation timestamp
     - **increment_number**: scan increment number
     - **rule_pack**: rule pack version
     - **repository_id**: repository id
     """
     # Determine the increment number if needed and not supplied
     if scan.scan_type == ScanType.INCREMENTAL and (not scan.increment_number or scan.increment_number <= 0):
-        last_scan = scan_crud.get_latest_scan_for_repository(db_connection, repository_id=scan.repository_id)
+        last_scan = scan_crud.get_latest_scan_for_repository(
+            db_connection=db_connection, repository_id=scan.repository_id
+        )
         new_increment = last_scan.increment_number + 1
         scan.increment_number = new_increment
 
     try:
         created_scan = scan_crud.create_scan(db_connection=db_connection, scan=scan)
     except IntegrityError as err:
         logger.debug(f"Error creating new scan object: {err}")
@@ -235,22 +239,60 @@
     - **rule_name**: rule name
     - **repository_id**: repository id of the finding
     - **return**: [FindingRead]
         The output will contain a PaginationModel containing the list of FindingRead type objects,
         or an empty list if no scan was found
     """
 
-    created_findings = finding_crud.create_findings(db_connection=db_connection, findings=findings)
-    scan_findings = []
+    db_scan: DBscan = scan_crud.get_scan(db_connection, scan_id=scan_id)
+    if db_scan is None:
+        raise HTTPException(status_code=404, detail="Scan not found")
+    # return db_scan
+
+    # 1. Fetch rules with scan_as_dir
+    rules_scan_as_dir: list[str] = rule_crud.get_scan_as_dir_rules_by_scan_id(
+        db_connection=db_connection, scan_id=scan_id
+    )
+    logger.debug(f"rules as directory: {", ".join(rules_scan_as_dir)}")
+
+    # 2. split findings into 2 category: scan_as_dir and normal.
+    findings_as_repo = []
+    findings_as_dir = []
+    for finding in findings:
+        (findings_as_dir if finding.rule_name in rules_scan_as_dir else findings_as_repo).append(finding)
+    logger.debug(f"number of findings scan as directory: {len(findings_as_dir)}")
+    logger.debug(f"number of findings scan as repo: {len(findings_as_repo)}")
+
+    # 3. Process normal as previously done.
+    created_findings: list[DBfinding] = finding_crud.create_findings(
+        db_connection=db_connection, findings=findings_as_repo
+    )
+    # 4. Process scan_as_dir with updates.
+    created_dir_findings: list[DBfinding] = finding_crud.create_or_update_findings(
+        db_connection=db_connection, findings=findings_as_dir
+    )
+
+    created_findings.extend(created_dir_findings)
+    # 5. Add link between findings and scan
+    scan_findings: list[DBscanFinding] = []
     for finding in created_findings:
         scan_finding = DBscanFinding(finding_id=finding.id_, scan_id=scan_id)
         scan_findings.append(scan_finding)
 
+    # 6. merge.
     _ = scan_finding_crud.create_scan_findings(db_connection=db_connection, scan_findings=scan_findings)
 
+    # 7. Mark old scan_as_dir findings as outdated.
+    findings_to_audit: list[int] = finding_crud.get_findings_from_repo_of_scan_as_dir(
+        db_connection=db_connection, scan=db_scan
+    )
+    audit_crud.create_automated_audit(
+        db_connection=db_connection, findings_ids=findings_to_audit, status=FindingStatus.OUTDATED
+    )
+
     # Clear cache related to findings
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_FINDING)
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_RULE)
 
     return len(created_findings)
```

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/endpoints/vcs_instances.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Standard Library
 import logging
 
 # Third Party
 from fastapi import APIRouter, Depends, HTTPException, Query, status
 from sqlalchemy.exc import IntegrityError
+from sqlalchemy.orm import Session
 
 # First Party
 from resc_backend.constants import (
     CACHE_NAMESPACE_VCS_INSTANCE,
     DEFAULT_RECORDS_PER_PAGE_LIMIT,
     ERROR_MESSAGE_500,
     ERROR_MESSAGE_503,
     RWS_ROUTE_VCS,
     VCS_TAG,
 )
-from resc_backend.db.connection import Session
 from resc_backend.resc_web_service.cache_manager import CacheManager
 from resc_backend.resc_web_service.crud import vcs_instance as vcs_instance_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
 from resc_backend.resc_web_service.helpers.resc_swagger_models import Model400, Model404
 from resc_backend.resc_web_service.schema import vcs_instance as vcs_instance_schema
 from resc_backend.resc_web_service.schema.pagination_model import PaginationModel
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
```

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/filters.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/filters.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/helpers/exception_handler.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/exception_handler.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/helpers/rule.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/helpers/toml.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/helpers/toml.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/audit.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/detailed_finding.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/detailed_finding.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     repository_name: constr(min_length=1, max_length=100)
     repository_url: HttpUrl
     timestamp: datetime.datetime
     vcs_provider: VCSProviders
     last_scanned_commit: constr(min_length=1, max_length=100)
     scan_id: conint(gt=0)
     event_sent_on: datetime.datetime | None
+    is_dir_scan: bool
 
 
 class DetailedFinding(DetailedFindingBase):
     pass
 
 
 class DetailedFindingRead(DetailedFinding):
@@ -44,30 +45,45 @@
     @staticmethod
     def build_bitbucket_commit_url(
         repository_url: str,
         repository_name: str,
         project_key: str,
         file_path: str,
         commit_id: str,
+        line_number: int,
     ) -> str:
         arr = repository_url.split("/")
         if len(arr) >= 3:
             repo_base_url = arr[0] + "//" + arr[2]
         else:
             repo_base_url = repository_url
-        bitbucket_commit_url = (
-            f"{repo_base_url}/projects/{project_key}/repos/" f"{repository_name}/browse/{file_path}?at={commit_id}"
+
+        return (
+            f"{repo_base_url}/projects/{project_key}/repos/"
+            f"{repository_name}/commits/{commit_id}#{file_path}?t={line_number}"
         )
-        commit_url = bitbucket_commit_url
-        return commit_url
 
     @staticmethod
-    def build_ado_commit_url(repository_url: str, file_path: str, commit_id: str) -> str:
-        ado_commit_url = f"{repository_url}/commit/{commit_id}?path=/{file_path}"
-        return ado_commit_url
+    def build_ado_commit_url(
+        repository_url: str,
+        file_path: str,
+        commit_id: str,
+        line_number: int,
+        is_dir_scan: bool,
+    ) -> str:
+        if is_dir_scan:
+            return (
+                f"{repository_url}?version=GC{commit_id}&path=/{file_path}&line={line_number}&lineEnd={line_number + 1}"
+                "&lineStartColumn=1&lineEndColumn=1&type=2&lineStyle=plain"
+            )
+
+        return (
+            f"{repository_url}/commit/{commit_id}?path=/{file_path}&line={line_number}&lineEnd={line_number + 1}"
+            "&lineStartColumn=1&lineEndColumn=1&type=2&lineStyle=plain"
+        )
 
     @staticmethod
     def build_github_commit_url(repository_url: str, file_path: str, commit_id: str) -> str:
         github_commit_url = f"{repository_url}/commit/{commit_id}?path=/{file_path}"
         return github_commit_url
 
     @root_validator
@@ -79,20 +95,23 @@
         if values["vcs_provider"] == VCSProviders.BITBUCKET:
             values["commit_url"] = cls.build_bitbucket_commit_url(
                 repository_url=values["repository_url"],
                 repository_name=values["repository_name"],
                 project_key=values["project_key"],
                 file_path=values["file_path"],
                 commit_id=values["commit_id"],
+                line_number=values["line_number"],
             )
         elif values["vcs_provider"] == VCSProviders.AZURE_DEVOPS:
             values["commit_url"] = cls.build_ado_commit_url(
                 repository_url=values["repository_url"],
                 file_path=values["file_path"],
                 commit_id=values["commit_id"],
+                line_number=values["line_number"],
+                is_dir_scan=values["is_dir_scan"],
             )
 
         elif values["vcs_provider"] == VCSProviders.GITHUB_PUBLIC:
             values["commit_url"] = cls.build_github_commit_url(
                 repository_url=values["repository_url"],
                 file_path=values["file_path"],
                 commit_id=values["commit_id"],
```

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/finding.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/finding_count_model.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/finding_count_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/finding_status.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/finding_status.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/pagination_model.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/pagination_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/repository.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/repository_enriched.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/repository_enriched.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/rule.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/rule_allow_list.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/rule_pack.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/scan.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service/schema/vcs_instance.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service/schema/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service_interface/findings.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service_interface/repositories.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/repositories.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service_interface/rule_packs.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/rule_packs.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend/resc_web_service_interface/vcs_instances.py` & `resc_backend-3.3.0/src/resc_backend/resc_web_service_interface/vcs_instances.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.2.2/src/resc_backend.egg-info/PKG-INFO` & `resc_backend-3.3.0/src/resc_backend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_backend
-Version: 3.2.2
+Version: 3.3.0
 Summary: Repository Scanner - Backend
 Home-page: https://github.com/abnamro/resc-backend
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `resc_backend-3.2.2/src/resc_backend.egg-info/SOURCES.txt` & `resc_backend-3.3.0/src/resc_backend.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 src/resc_backend/db/model/scan.py
 src/resc_backend/db/model/scan_finding.py
 src/resc_backend/db/model/tag.py
 src/resc_backend/db/model/vcs_instance.py
 src/resc_backend/helpers/__init__.py
 src/resc_backend/helpers/dict_remapper.py
 src/resc_backend/helpers/environment_wrapper.py
+src/resc_backend/helpers/list_mapper.py
 src/resc_backend/helpers/rabbitmq/__init__.py
 src/resc_backend/helpers/rabbitmq/configuration.py
 src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
 src/resc_backend/resc_web_service/__init__.py
 src/resc_backend/resc_web_service/api.py
 src/resc_backend/resc_web_service/cache_manager.py
 src/resc_backend/resc_web_service/configuration.py
```

