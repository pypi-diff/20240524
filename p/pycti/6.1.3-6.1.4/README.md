# Comparing `tmp/pycti-6.1.3.tar.gz` & `tmp/pycti-6.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-6.1.3.tar", last modified: Mon May 20 23:00:26 2024, max compression
+gzip compressed data, was "pycti-6.1.4.tar", last modified: Thu May 23 22:27:40 2024, max compression
```

## Comparing `pycti-6.1.3.tar` & `pycti-6.1.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:26.435885 pycti-6.1.3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-20 23:00:12.000000 pycti-6.1.3/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-20 23:00:26.435885 pycti-6.1.3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3156 2024-05-20 23:00:12.000000 pycti-6.1.3/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:26.423885 pycti-6.1.3/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5035 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:26.423885 pycti-6.1.3/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29575 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3549 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/api/opencti_api_playbook.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7615 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:26.427885 pycti-6.1.3/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2449 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    60311 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/connector/opencti_connector_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/connector/opencti_metric_handler.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:26.431885 pycti-6.1.3/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21471 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17107 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33699 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31876 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32760 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18001 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18582 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17470 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16706 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13216 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29320 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22879 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18553 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27581 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19353 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18957 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8062 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8800 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16176 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16970 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20411 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21480 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_malware_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16468 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29938 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30550 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21837 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33580 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2275 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    49559 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42895 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106785 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    78504 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12330 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17696 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27584 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18996 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_threat_actor_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19238 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_threat_actor_individual.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14661 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20094 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:26.435885 pycti-6.1.3/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10601 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2199 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/utils/opencti_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   112457 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14658 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4138 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:26.435885 pycti-6.1.3/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-20 23:00:26.000000 pycti-6.1.3/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-20 23:00:26.000000 pycti-6.1.3/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-20 23:00:26.000000 pycti-6.1.3/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-20 23:00:26.000000 pycti-6.1.3/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-20 23:00:26.000000 pycti-6.1.3/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-20 23:00:12.000000 pycti-6.1.3/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-05-20 23:00:26.435885 pycti-6.1.3/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:40.827206 pycti-6.1.4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-23 22:27:27.000000 pycti-6.1.4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-23 22:27:40.827206 pycti-6.1.4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3156 2024-05-23 22:27:27.000000 pycti-6.1.4/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:40.815206 pycti-6.1.4/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5035 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:40.815206 pycti-6.1.4/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29575 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3549 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/api/opencti_api_playbook.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7615 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:40.815206 pycti-6.1.4/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2449 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    60311 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/connector/opencti_connector_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/connector/opencti_metric_handler.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:40.823206 pycti-6.1.4/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21471 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17107 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33699 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31876 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32760 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18001 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18582 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17470 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16706 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13216 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29320 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22879 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18553 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27581 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19353 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18957 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8062 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8800 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16176 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16970 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20411 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21480 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_malware_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16468 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29938 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30550 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21837 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33580 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2275 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    49559 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43249 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   106785 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    78504 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12330 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17696 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27584 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18996 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_threat_actor_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19238 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_threat_actor_individual.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14661 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20094 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:40.823206 pycti-6.1.4/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10601 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2199 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/utils/opencti_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   112457 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14658 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4138 2024-05-23 22:27:28.000000 pycti-6.1.4/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 22:27:40.823206 pycti-6.1.4/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-23 22:27:40.000000 pycti-6.1.4/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-23 22:27:40.000000 pycti-6.1.4/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-23 22:27:40.000000 pycti-6.1.4/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-23 22:27:40.000000 pycti-6.1.4/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-23 22:27:40.000000 pycti-6.1.4/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-23 22:27:28.000000 pycti-6.1.4/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-05-23 22:27:40.827206 pycti-6.1.4/setup.cfg
```

### Comparing `pycti-6.1.3/LICENSE` & `pycti-6.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/PKG-INFO` & `pycti-6.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 6.1.3
+Version: 6.1.4
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycti-6.1.3/README.md` & `pycti-6.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/__init__.py` & `pycti-6.1.4/pycti/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "6.1.3"
+__version__ = "6.1.4"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
```

### Comparing `pycti-6.1.3/pycti/api/opencti_api_client.py` & `pycti-6.1.4/pycti/api/opencti_api_client.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/api/opencti_api_connector.py` & `pycti-6.1.4/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/api/opencti_api_playbook.py` & `pycti-6.1.4/pycti/api/opencti_api_playbook.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/api/opencti_api_work.py` & `pycti-6.1.4/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/connector/opencti_connector.py` & `pycti-6.1.4/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/connector/opencti_connector_helper.py` & `pycti-6.1.4/pycti/connector/opencti_connector_helper.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/connector/opencti_metric_handler.py` & `pycti-6.1.4/pycti/connector/opencti_metric_handler.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_attack_pattern.py` & `pycti-6.1.4/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_campaign.py` & `pycti-6.1.4/pycti/entities/opencti_campaign.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_case_incident.py` & `pycti-6.1.4/pycti/entities/opencti_case_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_case_rfi.py` & `pycti-6.1.4/pycti/entities/opencti_case_rfi.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_case_rft.py` & `pycti-6.1.4/pycti/entities/opencti_case_rft.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_channel.py` & `pycti-6.1.4/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_course_of_action.py` & `pycti-6.1.4/pycti/entities/opencti_course_of_action.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_data_component.py` & `pycti-6.1.4/pycti/entities/opencti_data_component.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_data_source.py` & `pycti-6.1.4/pycti/entities/opencti_data_source.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_event.py` & `pycti-6.1.4/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_external_reference.py` & `pycti-6.1.4/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_feedback.py` & `pycti-6.1.4/pycti/entities/opencti_feedback.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_grouping.py` & `pycti-6.1.4/pycti/entities/opencti_grouping.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_identity.py` & `pycti-6.1.4/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_incident.py` & `pycti-6.1.4/pycti/entities/opencti_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_indicator.py` & `pycti-6.1.4/pycti/entities/opencti_indicator.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_infrastructure.py` & `pycti-6.1.4/pycti/entities/opencti_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_intrusion_set.py` & `pycti-6.1.4/pycti/entities/opencti_intrusion_set.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_kill_chain_phase.py` & `pycti-6.1.4/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_label.py` & `pycti-6.1.4/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_language.py` & `pycti-6.1.4/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_location.py` & `pycti-6.1.4/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_malware.py` & `pycti-6.1.4/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_malware_analysis.py` & `pycti-6.1.4/pycti/entities/opencti_malware_analysis.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_marking_definition.py` & `pycti-6.1.4/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_narrative.py` & `pycti-6.1.4/pycti/entities/opencti_narrative.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_note.py` & `pycti-6.1.4/pycti/entities/opencti_note.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_observed_data.py` & `pycti-6.1.4/pycti/entities/opencti_observed_data.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_opinion.py` & `pycti-6.1.4/pycti/entities/opencti_opinion.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_report.py` & `pycti-6.1.4/pycti/entities/opencti_report.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_stix.py` & `pycti-6.1.4/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_stix_core_object.py` & `pycti-6.1.4/pycti/entities/opencti_stix_core_object.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_stix_core_relationship.py` & `pycti-6.1.4/pycti/entities/opencti_stix_core_relationship.py`

 * *Files 2% similar despite different names*

```diff
@@ -584,14 +584,15 @@
         modified = kwargs.get("modified", None)
         created_by = kwargs.get("createdBy", None)
         object_marking = kwargs.get("objectMarking", None)
         object_label = kwargs.get("objectLabel", None)
         external_references = kwargs.get("externalReferences", None)
         kill_chain_phases = kwargs.get("killChainPhases", None)
         granted_refs = kwargs.get("objectOrganization", None)
+        x_opencti_workflow_id = kwargs.get("x_opencti_workflow_id", None)
         update = kwargs.get("update", False)
 
         self.opencti.app_logger.info(
             "Creating stix_core_relationship",
             {
                 "relationship_type": relationship_type,
                 "from_id": from_id,
@@ -626,14 +627,15 @@
                     "modified": modified,
                     "createdBy": created_by,
                     "objectMarking": object_marking,
                     "objectLabel": object_label,
                     "objectOrganization": granted_refs,
                     "externalReferences": external_references,
                     "killChainPhases": kill_chain_phases,
+                    "x_opencti_workflow_id": x_opencti_workflow_id,
                     "update": update,
                 }
             },
         )
         return self.opencti.process_multiple_fields(
             result["data"]["stixCoreRelationshipAdd"]
         )
@@ -1186,13 +1188,18 @@
                     else None
                 ),
                 objectOrganization=(
                     stix_relation["x_opencti_granted_refs"]
                     if "x_opencti_granted_refs" in stix_relation
                     else None
                 ),
+                x_opencti_workflow_id=(
+                    stix_relation["x_opencti_workflow_id"]
+                    if "x_opencti_workflow_id" in stix_relation
+                    else None
+                ),
                 update=update,
             )
         else:
             self.opencti.app_logger.error(
                 "[opencti_stix_core_relationship] Missing parameters: stixObject"
             )
```

### Comparing `pycti-6.1.3/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-6.1.4/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_stix_domain_object.py` & `pycti-6.1.4/pycti/entities/opencti_stix_domain_object.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-6.1.4/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-6.1.4/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-6.1.4/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_task.py` & `pycti-6.1.4/pycti/entities/opencti_task.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_threat_actor.py` & `pycti-6.1.4/pycti/entities/opencti_threat_actor.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_threat_actor_group.py` & `pycti-6.1.4/pycti/entities/opencti_threat_actor_group.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_threat_actor_individual.py` & `pycti-6.1.4/pycti/entities/opencti_threat_actor_individual.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_tool.py` & `pycti-6.1.4/pycti/entities/opencti_tool.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_vocabulary.py` & `pycti-6.1.4/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/entities/opencti_vulnerability.py` & `pycti-6.1.4/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/utils/constants.py` & `pycti-6.1.4/pycti/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/utils/opencti_logger.py` & `pycti-6.1.4/pycti/utils/opencti_logger.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/utils/opencti_stix2.py` & `pycti-6.1.4/pycti/utils/opencti_stix2.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/utils/opencti_stix2_splitter.py` & `pycti-6.1.4/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/utils/opencti_stix2_update.py` & `pycti-6.1.4/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti/utils/opencti_stix2_utils.py` & `pycti-6.1.4/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti.egg-info/PKG-INFO` & `pycti-6.1.4/pycti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 6.1.3
+Version: 6.1.4
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycti-6.1.3/pycti.egg-info/SOURCES.txt` & `pycti-6.1.4/pycti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pycti.egg-info/requires.txt` & `pycti-6.1.4/pycti.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/pyproject.toml` & `pycti-6.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-6.1.3/setup.cfg` & `pycti-6.1.4/setup.cfg`

 * *Files identical despite different names*

