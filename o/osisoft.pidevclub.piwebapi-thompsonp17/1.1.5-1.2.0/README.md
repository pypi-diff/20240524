# Comparing `tmp/osisoft.pidevclub.piwebapi-thompsonp17-1.1.5.tar.gz` & `tmp/osisoft_pidevclub_piwebapi_thompsonp17-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osisoft.pidevclub.piwebapi-thompsonp17-1.1.5.tar", last modified: Wed Sep 27 16:06:33 2023, max compression
+gzip compressed data, was "osisoft_pidevclub_piwebapi_thompsonp17-1.2.0.tar", last modified: Fri May 24 19:13:38 2024, max compression
```

## Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5.tar` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0.tar`

### file list

```diff
@@ -1,229 +1,229 @@
-drwxrwxrwx   0        0        0        0 2023-09-27 16:06:33.159584 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/
--rw-rw-rw-   0        0        0    11558 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/LICENSE.md
--rw-rw-rw-   0        0        0      656 2023-09-27 16:06:33.157570 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     9726 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-09-27 16:06:31.529119 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/credentials/
--rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/credentials/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-27 16:06:31.530123 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/mockers/
--rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/mockers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-27 16:06:31.531124 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/mockers/pidevclub/
--rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/mockers/pidevclub/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-27 16:06:31.542568 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/mockers/pidevclub/piwebapi/
--rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/mockers/pidevclub/piwebapi/__init__.py
--rw-rw-rw-   0        0        0     2570 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/mockers/pidevclub/piwebapi/pi_web_api_client.py
-drwxrwxrwx   0        0        0        0 2023-09-27 16:06:31.543577 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/
--rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-27 16:06:31.559092 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/
--rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-27 16:06:31.581092 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/
--rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-27 16:06:31.968255 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/
--rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/__init__.py
--rw-rw-rw-   0        0        0    32521 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/analysis_api.py
--rw-rw-rw-   0        0        0    27198 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/analysis_category_api.py
--rw-rw-rw-   0        0        0    16298 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/analysis_rule_api.py
--rw-rw-rw-   0        0        0     5632 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/analysis_rule_plug_in_api.py
--rw-rw-rw-   0        0        0    35214 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/analysis_template_api.py
--rw-rw-rw-   0        0        0   120410 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/asset_database_api.py
--rw-rw-rw-   0        0        0    59529 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/asset_server_api.py
--rw-rw-rw-   0        0        0    32332 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/attribute_api.py
--rw-rw-rw-   0        0        0    27211 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/attribute_category_api.py
--rw-rw-rw-   0        0        0    17520 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/attribute_template_api.py
--rw-rw-rw-   0        0        0     5297 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/attribute_trait_api.py
--rw-rw-rw-   0        0        0     2677 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/batch_api.py
--rw-rw-rw-   0        0        0    13170 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/calculation_api.py
--rw-rw-rw-   0        0        0     2447 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/channel_api.py
--rw-rw-rw-   0        0        0     6276 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/configuration_api.py
--rw-rw-rw-   0        0        0     8960 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/data_api.py
--rw-rw-rw-   0        0        0    23660 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/data_server_api.py
--rw-rw-rw-   0        0        0    86574 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/element_api.py
--rw-rw-rw-   0        0        0    27265 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/element_category_api.py
--rw-rw-rw-   0        0        0    37862 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/element_template_api.py
--rw-rw-rw-   0        0        0    32316 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/enumeration_set_api.py
--rw-rw-rw-   0        0        0    10167 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/enumeration_value_api.py
--rw-rw-rw-   0        0        0    89019 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/event_frame_api.py
--rw-rw-rw-   0        0        0     2383 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/home_api.py
--rw-rw-rw-   0        0        0    19551 2023-09-27 13:12:00.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/point_api.py
--rw-rw-rw-   0        0        0    21272 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/security_identity_api.py
--rw-rw-rw-   0        0        0    18701 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/security_mapping_api.py
--rw-rw-rw-   0        0        0    40882 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/stream_api.py
--rw-rw-rw-   0        0        0    99737 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/stream_set_api.py
--rw-rw-rw-   0        0        0     9115 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/system_api.py
--rw-rw-rw-   0        0        0    33961 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/table_api.py
--rw-rw-rw-   0        0        0    27219 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/table_category_api.py
--rw-rw-rw-   0        0        0     9797 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/time_rule_api.py
--rw-rw-rw-   0        0        0     5612 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/time_rule_plug_in_api.py
--rw-rw-rw-   0        0        0     9779 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/unit_api.py
--rw-rw-rw-   0        0        0    17330 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/unit_class_api.py
--rw-rw-rw-   0        0        0    18484 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api_client.py
-drwxrwxrwx   0        0        0        0 2023-09-27 16:06:33.038847 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/
--rw-rw-rw-   0        0        0    12528 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/__init__.py
--rw-rw-rw-   0        0        0    10107 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis.py
--rw-rw-rw-   0        0        0     3537 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_category.py
--rw-rw-rw-   0        0        0     2646 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_category_links.py
--rw-rw-rw-   0        0        0     5065 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_links.py
--rw-rw-rw-   0        0        0     6920 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_rule.py
--rw-rw-rw-   0        0        0     3274 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_rule_links.py
--rw-rw-rw-   0        0        0     7671 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_rule_plug_in.py
--rw-rw-rw-   0        0        0     2012 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_rule_plug_in_links.py
--rw-rw-rw-   0        0        0     7166 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_template.py
--rw-rw-rw-   0        0        0     4792 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_template_links.py
--rw-rw-rw-   0        0        0     4538 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_annotation.py
--rw-rw-rw-   0        0        0     1892 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_annotation_links.py
--rw-rw-rw-   0        0        0     3996 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_asset_database.py
--rw-rw-rw-   0        0        0     6631 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_asset_database_links.py
--rw-rw-rw-   0        0        0     4717 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_asset_server.py
--rw-rw-rw-   0        0        0     4807 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_asset_server_links.py
--rw-rw-rw-   0        0        0     8288 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_attribute.py
--rw-rw-rw-   0        0        0     3540 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_attribute_category.py
--rw-rw-rw-   0        0        0     2648 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_attribute_category_links.py
--rw-rw-rw-   0        0        0     6742 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_attribute_links.py
--rw-rw-rw-   0        0        0     8448 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_attribute_template.py
--rw-rw-rw-   0        0        0     3345 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_attribute_template_links.py
--rw-rw-rw-   0        0        0     5985 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_attribute_trait.py
--rw-rw-rw-   0        0        0     1632 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_attribute_trait_links.py
--rw-rw-rw-   0        0        0     3847 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_cache_instance.py
--rw-rw-rw-   0        0        0     3472 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_channel_instance.py
--rw-rw-rw-   0        0        0     3912 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_data_server.py
--rw-rw-rw-   0        0        0     3534 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_data_server_license.py
--rw-rw-rw-   0        0        0     1921 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_data_server_license_links.py
--rw-rw-rw-   0        0        0     2315 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_data_server_links.py
--rw-rw-rw-   0        0        0     5074 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_element.py
--rw-rw-rw-   0        0        0     3534 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_element_category.py
--rw-rw-rw-   0        0        0     2644 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_element_category_links.py
--rw-rw-rw-   0        0        0     7147 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_element_links.py
--rw-rw-rw-   0        0        0     6744 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_element_template.py
--rw-rw-rw-   0        0        0     4640 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_element_template_links.py
--rw-rw-rw-   0        0        0     4015 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_enumeration_set.py
--rw-rw-rw-   0        0        0     3234 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_enumeration_set_links.py
--rw-rw-rw-   0        0        0     6054 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_enumeration_value.py
--rw-rw-rw-   0        0        0     2312 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_enumeration_value_links.py
--rw-rw-rw-   0        0        0     1895 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_errors.py
--rw-rw-rw-   0        0        0     9500 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_event_frame.py
--rw-rw-rw-   0        0        0     7919 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_event_frame_links.py
--rw-rw-rw-   0        0        0     2932 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_item_attribute.py
--rw-rw-rw-   0        0        0     2926 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_item_element.py
--rw-rw-rw-   0        0        0     2935 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_item_event_frame.py
--rw-rw-rw-   0        0        0     2920 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_item_point.py
--rw-rw-rw-   0        0        0     2159 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_analysis.py
--rw-rw-rw-   0        0        0     2183 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_analysis_category.py
--rw-rw-rw-   0        0        0     2171 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_analysis_rule.py
--rw-rw-rw-   0        0        0     2189 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_analysis_rule_plug_in.py
--rw-rw-rw-   0        0        0     2183 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_analysis_template.py
--rw-rw-rw-   0        0        0     2165 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_annotation.py
--rw-rw-rw-   0        0        0     2174 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_asset_database.py
--rw-rw-rw-   0        0        0     2168 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_asset_server.py
--rw-rw-rw-   0        0        0     2162 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_attribute.py
--rw-rw-rw-   0        0        0     2186 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_attribute_category.py
--rw-rw-rw-   0        0        0     2186 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_attribute_template.py
--rw-rw-rw-   0        0        0     2177 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_attribute_trait.py
--rw-rw-rw-   0        0        0     2174 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_cache_instance.py
--rw-rw-rw-   0        0        0     2180 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_channel_instance.py
--rw-rw-rw-   0        0        0     2165 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_data_server.py
--rw-rw-rw-   0        0        0     2156 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_element.py
--rw-rw-rw-   0        0        0     2180 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_element_category.py
--rw-rw-rw-   0        0        0     2180 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_element_template.py
--rw-rw-rw-   0        0        0     2177 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_enumeration_set.py
--rw-rw-rw-   0        0        0     2183 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_enumeration_value.py
--rw-rw-rw-   0        0        0     2165 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_event_frame.py
--rw-rw-rw-   0        0        0     2174 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_item_attribute.py
--rw-rw-rw-   0        0        0     2168 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_item_element.py
--rw-rw-rw-   0        0        0     2177 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_item_event_frame.py
--rw-rw-rw-   0        0        0     2162 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_item_point.py
--rw-rw-rw-   0        0        0     2177 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_items_substatus.py
--rw-rw-rw-   0        0        0     2150 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_point.py
--rw-rw-rw-   0        0        0     2177 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_point_attribute.py
--rw-rw-rw-   0        0        0     2174 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_security_entry.py
--rw-rw-rw-   0        0        0     2183 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_security_identity.py
--rw-rw-rw-   0        0        0     2180 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_security_mapping.py
--rw-rw-rw-   0        0        0     2177 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_security_rights.py
--rw-rw-rw-   0        0        0     2180 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_stream_summaries.py
--rw-rw-rw-   0        0        0     2168 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_stream_value.py
--rw-rw-rw-   0        0        0     2171 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_stream_values.py
--rw-rw-rw-   0        0        0     2162 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_substatus.py
--rw-rw-rw-   0        0        0     2171 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_summary_value.py
--rw-rw-rw-   0        0        0     2150 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_table.py
--rw-rw-rw-   0        0        0     2174 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_table_category.py
--rw-rw-rw-   0        0        0     2177 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_time_rule_plug_in.py
--rw-rw-rw-   0        0        0     2162 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_unit_class.py
--rw-rw-rw-   0        0        0     2261 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_landing.py
--rw-rw-rw-   0        0        0     2871 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_landing_links.py
--rw-rw-rw-   0        0        0     2639 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_pagination_links.py
--rw-rw-rw-   0        0        0     5460 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_point.py
--rw-rw-rw-   0        0        0     2758 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_point_attribute.py
--rw-rw-rw-   0        0        0     1900 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_point_attribute_links.py
--rw-rw-rw-   0        0        0     4274 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_point_links.py
--rw-rw-rw-   0        0        0     2242 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_property_error.py
--rw-rw-rw-   0        0        0     3810 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_request.py
--rw-rw-rw-   0        0        0     1937 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_request_template.py
--rw-rw-rw-   0        0        0     2455 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_response.py
--rw-rw-rw-   0        0        0     3026 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_search_by_attribute.py
--rw-rw-rw-   0        0        0     5745 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security.py
--rw-rw-rw-   0        0        0     3698 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security_entry.py
--rw-rw-rw-   0        0        0     2485 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security_entry_links.py
--rw-rw-rw-   0        0        0     3856 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security_identity.py
--rw-rw-rw-   0        0        0     3128 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security_identity_links.py
--rw-rw-rw-   0        0        0     4334 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security_mapping.py
--rw-rw-rw-   0        0        0     3126 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security_mapping_links.py
--rw-rw-rw-   0        0        0     7092 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security_rights.py
--rw-rw-rw-   0        0        0     1900 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security_rights_links.py
--rw-rw-rw-   0        0        0     3262 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_stream_summaries.py
--rw-rw-rw-   0        0        0     1917 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_stream_summaries_links.py
--rw-rw-rw-   0        0        0     3242 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_stream_value.py
--rw-rw-rw-   0        0        0     1909 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_stream_value_links.py
--rw-rw-rw-   0        0        0     3689 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_stream_values.py
--rw-rw-rw-   0        0        0     1911 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_stream_values_links.py
--rw-rw-rw-   0        0        0     2588 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_substatus.py
--rw-rw-rw-   0        0        0     2498 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_summary_value.py
--rw-rw-rw-   0        0        0     3035 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_system_landing.py
--rw-rw-rw-   0        0        0     3262 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_system_landing_links.py
--rw-rw-rw-   0        0        0     3091 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_system_status.py
--rw-rw-rw-   0        0        0     4673 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_table.py
--rw-rw-rw-   0        0        0     3528 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_table_category.py
--rw-rw-rw-   0        0        0     2640 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_table_category_links.py
--rw-rw-rw-   0        0        0     2544 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_table_data.py
--rw-rw-rw-   0        0        0     3172 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_table_links.py
--rw-rw-rw-   0        0        0     6657 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_time_rule.py
--rw-rw-rw-   0        0        0     2629 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_time_rule_links.py
--rw-rw-rw-   0        0        0     7659 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_time_rule_plug_in.py
--rw-rw-rw-   0        0        0     2004 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_time_rule_plug_in_links.py
--rw-rw-rw-   0        0        0     4193 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_timed_value.py
--rw-rw-rw-   0        0        0     2711 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_timed_values.py
--rw-rw-rw-   0        0        0     5764 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_unit.py
--rw-rw-rw-   0        0        0     4540 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_unit_class.py
--rw-rw-rw-   0        0        0     2616 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_unit_class_links.py
--rw-rw-rw-   0        0        0     2014 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_unit_links.py
--rw-rw-rw-   0        0        0     3704 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_user_info.py
--rw-rw-rw-   0        0        0     2558 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_value.py
--rw-rw-rw-   0        0        0     3570 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_value_query.py
--rw-rw-rw-   0        0        0     3065 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_version.py
--rw-rw-rw-   0        0        0     2240 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_web_exception.py
--rw-rw-rw-   0        0        0    10218 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/pi_web_api_client.py
--rw-rw-rw-   0        0        0     3643 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/rest.py
-drwxrwxrwx   0        0        0        0 2023-09-27 16:06:33.080168 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/web_id/
--rw-rw-rw-   0        0        0      745 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/web_id/__init__.py
--rw-rw-rw-   0        0        0      687 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/web_id/web_id_exception.py
--rw-rw-rw-   0        0        0     5701 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/web_id/web_id_helper.py
--rw-rw-rw-   0        0        0    14929 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/web_id/web_id_info.py
--rw-rw-rw-   0        0        0      719 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/web_id/web_id_string_type.py
--rw-rw-rw-   0        0        0      795 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/web_id/web_id_type.py
-drwxrwxrwx   0        0        0        0 2023-09-27 16:06:31.558143 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft.pidevclub.piwebapi_thompsonp17.egg-info/
--rw-rw-rw-   0        0        0      656 2023-09-27 16:06:31.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft.pidevclub.piwebapi_thompsonp17.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11137 2023-09-27 16:06:31.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft.pidevclub.piwebapi_thompsonp17.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-27 16:06:31.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft.pidevclub.piwebapi_thompsonp17.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-09-27 16:06:31.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft.pidevclub.piwebapi_thompsonp17.egg-info/requires.txt
--rw-rw-rw-   0        0        0       39 2023-09-27 16:06:31.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft.pidevclub.piwebapi_thompsonp17.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-09-27 16:06:33.159584 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1578 2023-09-27 16:06:09.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-27 16:06:33.125061 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/test/
--rw-rw-rw-   0        0        0       45 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-27 16:06:33.126069 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/test/mocks/
--rw-rw-rw-   0        0        0       45 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/test/mocks/__init__.py
--rw-rw-rw-   0        0        0     8525 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/test/test_data.py
--rw-rw-rw-   0        0        0     7761 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/test/test_main.py
--rw-rw-rw-   0        0        0     3371 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/test/test_webids.py
-drwxrwxrwx   0        0        0        0 2023-09-27 16:06:33.156638 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/utils/
--rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/utils/__init__.py
--rw-rw-rw-   0        0        0     1251 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/utils/arg_hash_functions.py
--rw-rw-rw-   0        0        0     2246 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/utils/mock_generators.py
--rw-rw-rw-   0        0        0      278 2023-09-27 12:05:15.000000 osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/utils/os_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:13:38.095108 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/
+-rw-rw-rw-   0        0        0    11558 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/LICENSE.md
+-rw-rw-rw-   0        0        0      656 2024-05-24 19:13:38.092090 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9726 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 19:13:34.657155 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/credentials/
+-rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/credentials/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:13:34.659180 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/mockers/
+-rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/mockers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:13:34.662163 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/mockers/pidevclub/
+-rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/mockers/pidevclub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:13:34.744419 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/mockers/pidevclub/piwebapi/
+-rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/mockers/pidevclub/piwebapi/__init__.py
+-rw-rw-rw-   0        0        0     2570 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/mockers/pidevclub/piwebapi/pi_web_api_client.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:13:34.744419 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/
+-rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:13:34.802723 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/
+-rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:13:34.860643 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/
+-rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:13:34.979012 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/
+-rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/__init__.py
+-rw-rw-rw-   0        0        0    32521 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/analysis_api.py
+-rw-rw-rw-   0        0        0    27198 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/analysis_category_api.py
+-rw-rw-rw-   0        0        0    16298 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/analysis_rule_api.py
+-rw-rw-rw-   0        0        0     5632 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/analysis_rule_plug_in_api.py
+-rw-rw-rw-   0        0        0    35214 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/analysis_template_api.py
+-rw-rw-rw-   0        0        0   120410 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/asset_database_api.py
+-rw-rw-rw-   0        0        0    59529 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/asset_server_api.py
+-rw-rw-rw-   0        0        0    32332 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/attribute_api.py
+-rw-rw-rw-   0        0        0    27211 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/attribute_category_api.py
+-rw-rw-rw-   0        0        0    17520 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/attribute_template_api.py
+-rw-rw-rw-   0        0        0     5297 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/attribute_trait_api.py
+-rw-rw-rw-   0        0        0     2677 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/batch_api.py
+-rw-rw-rw-   0        0        0    13170 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/calculation_api.py
+-rw-rw-rw-   0        0        0     2447 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/channel_api.py
+-rw-rw-rw-   0        0        0     6276 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/configuration_api.py
+-rw-rw-rw-   0        0        0     8960 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/data_api.py
+-rw-rw-rw-   0        0        0    23660 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/data_server_api.py
+-rw-rw-rw-   0        0        0    86574 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/element_api.py
+-rw-rw-rw-   0        0        0    27265 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/element_category_api.py
+-rw-rw-rw-   0        0        0    37862 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/element_template_api.py
+-rw-rw-rw-   0        0        0    32316 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/enumeration_set_api.py
+-rw-rw-rw-   0        0        0    10167 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/enumeration_value_api.py
+-rw-rw-rw-   0        0        0    89019 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/event_frame_api.py
+-rw-rw-rw-   0        0        0     2383 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/home_api.py
+-rw-rw-rw-   0        0        0    19551 2023-09-27 13:12:00.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/point_api.py
+-rw-rw-rw-   0        0        0    21272 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/security_identity_api.py
+-rw-rw-rw-   0        0        0    18701 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/security_mapping_api.py
+-rw-rw-rw-   0        0        0    40882 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/stream_api.py
+-rw-rw-rw-   0        0        0    99737 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/stream_set_api.py
+-rw-rw-rw-   0        0        0     9115 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/system_api.py
+-rw-rw-rw-   0        0        0    33961 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/table_api.py
+-rw-rw-rw-   0        0        0    27219 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/table_category_api.py
+-rw-rw-rw-   0        0        0     9797 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/time_rule_api.py
+-rw-rw-rw-   0        0        0     5612 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/time_rule_plug_in_api.py
+-rw-rw-rw-   0        0        0     9779 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/unit_api.py
+-rw-rw-rw-   0        0        0    17330 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/unit_class_api.py
+-rw-rw-rw-   0        0        0    18484 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api_client.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:13:37.832404 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/
+-rw-rw-rw-   0        0        0    12528 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/__init__.py
+-rw-rw-rw-   0        0        0    10107 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis.py
+-rw-rw-rw-   0        0        0     3537 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_category.py
+-rw-rw-rw-   0        0        0     2646 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_category_links.py
+-rw-rw-rw-   0        0        0     5065 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_links.py
+-rw-rw-rw-   0        0        0     6920 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_rule.py
+-rw-rw-rw-   0        0        0     3274 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_rule_links.py
+-rw-rw-rw-   0        0        0     7671 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_rule_plug_in.py
+-rw-rw-rw-   0        0        0     2012 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_rule_plug_in_links.py
+-rw-rw-rw-   0        0        0     7166 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_template.py
+-rw-rw-rw-   0        0        0     4792 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_template_links.py
+-rw-rw-rw-   0        0        0     4538 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_annotation.py
+-rw-rw-rw-   0        0        0     1892 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_annotation_links.py
+-rw-rw-rw-   0        0        0     3996 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_asset_database.py
+-rw-rw-rw-   0        0        0     6631 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_asset_database_links.py
+-rw-rw-rw-   0        0        0     4717 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_asset_server.py
+-rw-rw-rw-   0        0        0     4807 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_asset_server_links.py
+-rw-rw-rw-   0        0        0     8288 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_attribute.py
+-rw-rw-rw-   0        0        0     3540 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_attribute_category.py
+-rw-rw-rw-   0        0        0     2648 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_attribute_category_links.py
+-rw-rw-rw-   0        0        0     6742 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_attribute_links.py
+-rw-rw-rw-   0        0        0     8448 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_attribute_template.py
+-rw-rw-rw-   0        0        0     3345 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_attribute_template_links.py
+-rw-rw-rw-   0        0        0     5985 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_attribute_trait.py
+-rw-rw-rw-   0        0        0     1632 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_attribute_trait_links.py
+-rw-rw-rw-   0        0        0     3847 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_cache_instance.py
+-rw-rw-rw-   0        0        0     3472 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_channel_instance.py
+-rw-rw-rw-   0        0        0     3912 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_data_server.py
+-rw-rw-rw-   0        0        0     3534 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_data_server_license.py
+-rw-rw-rw-   0        0        0     1921 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_data_server_license_links.py
+-rw-rw-rw-   0        0        0     2315 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_data_server_links.py
+-rw-rw-rw-   0        0        0     5074 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_element.py
+-rw-rw-rw-   0        0        0     3534 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_element_category.py
+-rw-rw-rw-   0        0        0     2644 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_element_category_links.py
+-rw-rw-rw-   0        0        0     7147 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_element_links.py
+-rw-rw-rw-   0        0        0     6744 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_element_template.py
+-rw-rw-rw-   0        0        0     4640 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_element_template_links.py
+-rw-rw-rw-   0        0        0     4015 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_enumeration_set.py
+-rw-rw-rw-   0        0        0     3234 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_enumeration_set_links.py
+-rw-rw-rw-   0        0        0     6054 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_enumeration_value.py
+-rw-rw-rw-   0        0        0     2312 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_enumeration_value_links.py
+-rw-rw-rw-   0        0        0     1895 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_errors.py
+-rw-rw-rw-   0        0        0     9500 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_event_frame.py
+-rw-rw-rw-   0        0        0     7919 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_event_frame_links.py
+-rw-rw-rw-   0        0        0     2932 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_item_attribute.py
+-rw-rw-rw-   0        0        0     2926 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_item_element.py
+-rw-rw-rw-   0        0        0     2935 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_item_event_frame.py
+-rw-rw-rw-   0        0        0     2920 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_item_point.py
+-rw-rw-rw-   0        0        0     2159 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_analysis.py
+-rw-rw-rw-   0        0        0     2183 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_analysis_category.py
+-rw-rw-rw-   0        0        0     2171 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_analysis_rule.py
+-rw-rw-rw-   0        0        0     2189 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_analysis_rule_plug_in.py
+-rw-rw-rw-   0        0        0     2183 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_analysis_template.py
+-rw-rw-rw-   0        0        0     2165 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_annotation.py
+-rw-rw-rw-   0        0        0     2174 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_asset_database.py
+-rw-rw-rw-   0        0        0     2168 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_asset_server.py
+-rw-rw-rw-   0        0        0     2162 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_attribute.py
+-rw-rw-rw-   0        0        0     2186 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_attribute_category.py
+-rw-rw-rw-   0        0        0     2186 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_attribute_template.py
+-rw-rw-rw-   0        0        0     2177 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_attribute_trait.py
+-rw-rw-rw-   0        0        0     2174 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_cache_instance.py
+-rw-rw-rw-   0        0        0     2180 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_channel_instance.py
+-rw-rw-rw-   0        0        0     2165 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_data_server.py
+-rw-rw-rw-   0        0        0     2156 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_element.py
+-rw-rw-rw-   0        0        0     2180 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_element_category.py
+-rw-rw-rw-   0        0        0     2180 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_element_template.py
+-rw-rw-rw-   0        0        0     2177 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_enumeration_set.py
+-rw-rw-rw-   0        0        0     2183 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_enumeration_value.py
+-rw-rw-rw-   0        0        0     2165 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_event_frame.py
+-rw-rw-rw-   0        0        0     2174 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_item_attribute.py
+-rw-rw-rw-   0        0        0     2168 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_item_element.py
+-rw-rw-rw-   0        0        0     2177 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_item_event_frame.py
+-rw-rw-rw-   0        0        0     2162 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_item_point.py
+-rw-rw-rw-   0        0        0     2177 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_items_substatus.py
+-rw-rw-rw-   0        0        0     2150 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_point.py
+-rw-rw-rw-   0        0        0     2177 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_point_attribute.py
+-rw-rw-rw-   0        0        0     2174 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_security_entry.py
+-rw-rw-rw-   0        0        0     2183 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_security_identity.py
+-rw-rw-rw-   0        0        0     2180 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_security_mapping.py
+-rw-rw-rw-   0        0        0     2177 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_security_rights.py
+-rw-rw-rw-   0        0        0     2180 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_stream_summaries.py
+-rw-rw-rw-   0        0        0     2168 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_stream_value.py
+-rw-rw-rw-   0        0        0     2171 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_stream_values.py
+-rw-rw-rw-   0        0        0     2162 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_substatus.py
+-rw-rw-rw-   0        0        0     2171 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_summary_value.py
+-rw-rw-rw-   0        0        0     2150 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_table.py
+-rw-rw-rw-   0        0        0     2174 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_table_category.py
+-rw-rw-rw-   0        0        0     2177 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_time_rule_plug_in.py
+-rw-rw-rw-   0        0        0     2162 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_unit_class.py
+-rw-rw-rw-   0        0        0     2261 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_landing.py
+-rw-rw-rw-   0        0        0     2871 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_landing_links.py
+-rw-rw-rw-   0        0        0     2639 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_pagination_links.py
+-rw-rw-rw-   0        0        0     5460 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_point.py
+-rw-rw-rw-   0        0        0     2758 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_point_attribute.py
+-rw-rw-rw-   0        0        0     1900 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_point_attribute_links.py
+-rw-rw-rw-   0        0        0     4274 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_point_links.py
+-rw-rw-rw-   0        0        0     2242 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_property_error.py
+-rw-rw-rw-   0        0        0     3810 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_request.py
+-rw-rw-rw-   0        0        0     1937 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_request_template.py
+-rw-rw-rw-   0        0        0     2455 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_response.py
+-rw-rw-rw-   0        0        0     3026 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_search_by_attribute.py
+-rw-rw-rw-   0        0        0     5745 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security.py
+-rw-rw-rw-   0        0        0     3698 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security_entry.py
+-rw-rw-rw-   0        0        0     2485 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security_entry_links.py
+-rw-rw-rw-   0        0        0     3856 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security_identity.py
+-rw-rw-rw-   0        0        0     3128 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security_identity_links.py
+-rw-rw-rw-   0        0        0     4334 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security_mapping.py
+-rw-rw-rw-   0        0        0     3126 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security_mapping_links.py
+-rw-rw-rw-   0        0        0     7092 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security_rights.py
+-rw-rw-rw-   0        0        0     1900 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security_rights_links.py
+-rw-rw-rw-   0        0        0     3262 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_stream_summaries.py
+-rw-rw-rw-   0        0        0     1917 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_stream_summaries_links.py
+-rw-rw-rw-   0        0        0     3242 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_stream_value.py
+-rw-rw-rw-   0        0        0     1909 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_stream_value_links.py
+-rw-rw-rw-   0        0        0     3689 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_stream_values.py
+-rw-rw-rw-   0        0        0     1911 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_stream_values_links.py
+-rw-rw-rw-   0        0        0     2588 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_substatus.py
+-rw-rw-rw-   0        0        0     2498 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_summary_value.py
+-rw-rw-rw-   0        0        0     3035 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_system_landing.py
+-rw-rw-rw-   0        0        0     3262 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_system_landing_links.py
+-rw-rw-rw-   0        0        0     3091 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_system_status.py
+-rw-rw-rw-   0        0        0     4673 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_table.py
+-rw-rw-rw-   0        0        0     3528 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_table_category.py
+-rw-rw-rw-   0        0        0     2640 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_table_category_links.py
+-rw-rw-rw-   0        0        0     2544 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_table_data.py
+-rw-rw-rw-   0        0        0     3172 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_table_links.py
+-rw-rw-rw-   0        0        0     6657 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_time_rule.py
+-rw-rw-rw-   0        0        0     2629 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_time_rule_links.py
+-rw-rw-rw-   0        0        0     7659 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_time_rule_plug_in.py
+-rw-rw-rw-   0        0        0     2004 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_time_rule_plug_in_links.py
+-rw-rw-rw-   0        0        0     4193 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_timed_value.py
+-rw-rw-rw-   0        0        0     2711 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_timed_values.py
+-rw-rw-rw-   0        0        0     5764 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_unit.py
+-rw-rw-rw-   0        0        0     4540 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_unit_class.py
+-rw-rw-rw-   0        0        0     2616 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_unit_class_links.py
+-rw-rw-rw-   0        0        0     2014 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_unit_links.py
+-rw-rw-rw-   0        0        0     3704 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_user_info.py
+-rw-rw-rw-   0        0        0     2558 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_value.py
+-rw-rw-rw-   0        0        0     3570 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_value_query.py
+-rw-rw-rw-   0        0        0     3065 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_version.py
+-rw-rw-rw-   0        0        0     2240 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_web_exception.py
+-rw-rw-rw-   0        0        0    10218 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/pi_web_api_client.py
+-rw-rw-rw-   0        0        0     3643 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/rest.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:13:37.932623 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/web_id/
+-rw-rw-rw-   0        0        0      745 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/web_id/__init__.py
+-rw-rw-rw-   0        0        0      687 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/web_id/web_id_exception.py
+-rw-rw-rw-   0        0        0     5701 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/web_id/web_id_helper.py
+-rw-rw-rw-   0        0        0    14929 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/web_id/web_id_info.py
+-rw-rw-rw-   0        0        0      719 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/web_id/web_id_string_type.py
+-rw-rw-rw-   0        0        0      795 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/web_id/web_id_type.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:13:38.090089 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft.pidevclub.piwebapi_thompsonp17.egg-info/
+-rw-rw-rw-   0        0        0      656 2024-05-24 19:13:34.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft.pidevclub.piwebapi_thompsonp17.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11137 2024-05-24 19:13:34.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft.pidevclub.piwebapi_thompsonp17.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 19:13:34.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft.pidevclub.piwebapi_thompsonp17.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-05-24 19:13:34.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft.pidevclub.piwebapi_thompsonp17.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       39 2024-05-24 19:13:34.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft.pidevclub.piwebapi_thompsonp17.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 19:13:38.096116 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1578 2024-05-24 19:10:05.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:13:38.014195 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/test/
+-rw-rw-rw-   0        0        0       45 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:13:38.020368 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/test/mocks/
+-rw-rw-rw-   0        0        0       45 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/test/mocks/__init__.py
+-rw-rw-rw-   0        0        0     8525 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/test/test_data.py
+-rw-rw-rw-   0        0        0     7761 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/test/test_main.py
+-rw-rw-rw-   0        0        0     3371 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/test/test_webids.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:13:38.084007 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/utils/
+-rw-rw-rw-   0        0        0        0 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/utils/__init__.py
+-rw-rw-rw-   0        0        0     1251 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/utils/arg_hash_functions.py
+-rw-rw-rw-   0        0        0     2246 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/utils/mock_generators.py
+-rw-rw-rw-   0        0        0      278 2023-09-27 12:05:15.000000 osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/utils/os_utils.py
```

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/LICENSE.md` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/PKG-INFO` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osisoft.pidevclub.piwebapi-thompsonp17
-Version: 1.1.5
+Version: 1.2.0
 Summary: PI Web API client library for Python (2017 R2)
 Home-page: https://github.com/osimloeff/PI-Web-API-Client-Python
 Author: Marcos Vainer Loeff
 Author-email: mloeff@osisoft.com
 License: MIT
 Keywords: PI Web API
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/README.md` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/mockers/pidevclub/piwebapi/pi_web_api_client.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/mockers/pidevclub/piwebapi/pi_web_api_client.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/analysis_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/analysis_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/analysis_category_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/analysis_category_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/analysis_rule_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/analysis_rule_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/analysis_rule_plug_in_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/analysis_rule_plug_in_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/analysis_template_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/analysis_template_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/asset_database_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/asset_database_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/asset_server_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/asset_server_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/attribute_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/attribute_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/attribute_category_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/attribute_category_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/attribute_template_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/attribute_template_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/attribute_trait_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/attribute_trait_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/batch_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/batch_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/calculation_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/calculation_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/channel_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/channel_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/configuration_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/configuration_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/data_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/data_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/data_server_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/data_server_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/element_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/element_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/element_category_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/element_category_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/element_template_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/element_template_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/enumeration_set_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/enumeration_set_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/enumeration_value_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/enumeration_value_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/event_frame_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/event_frame_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/home_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/home_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/point_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/point_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/security_identity_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/security_identity_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/security_mapping_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/security_mapping_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/stream_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/stream_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/stream_set_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/stream_set_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/system_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/system_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/table_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/table_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/table_category_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/table_category_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/time_rule_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/time_rule_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/time_rule_plug_in_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/time_rule_plug_in_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/unit_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/unit_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api/unit_class_api.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api/unit_class_api.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/api_client.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/api_client.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/__init__.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_category.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_category.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_category_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_category_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_rule.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_rule.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_rule_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_rule_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_rule_plug_in.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_rule_plug_in.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_rule_plug_in_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_rule_plug_in_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_template.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_template.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_analysis_template_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_analysis_template_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_annotation.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_annotation.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_annotation_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_annotation_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_asset_database.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_asset_database.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_asset_database_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_asset_database_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_asset_server.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_asset_server.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_asset_server_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_asset_server_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_attribute.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_attribute.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_attribute_category.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_attribute_category.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_attribute_category_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_attribute_category_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_attribute_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_attribute_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_attribute_template.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_attribute_template.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_attribute_template_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_attribute_template_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_attribute_trait.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_attribute_trait.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_attribute_trait_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_attribute_trait_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_cache_instance.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_cache_instance.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_channel_instance.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_channel_instance.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_data_server.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_data_server.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_data_server_license.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_data_server_license.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_data_server_license_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_data_server_license_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_data_server_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_data_server_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_element.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_element.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_element_category.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_element_category.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_element_category_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_element_category_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_element_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_element_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_element_template.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_element_template.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_element_template_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_element_template_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_enumeration_set.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_enumeration_set.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_enumeration_set_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_enumeration_set_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_enumeration_value.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_enumeration_value.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_enumeration_value_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_enumeration_value_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_errors.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_errors.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_event_frame.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_event_frame.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_event_frame_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_event_frame_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_item_attribute.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_item_attribute.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_item_element.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_item_element.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_item_event_frame.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_item_event_frame.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_item_point.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_item_point.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_analysis.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_analysis.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_analysis_category.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_analysis_category.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_analysis_rule.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_analysis_rule.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_analysis_rule_plug_in.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_analysis_rule_plug_in.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_analysis_template.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_analysis_template.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_annotation.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_annotation.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_asset_database.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_asset_database.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_asset_server.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_asset_server.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_attribute.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_attribute.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_attribute_category.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_attribute_category.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_attribute_template.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_attribute_template.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_attribute_trait.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_attribute_trait.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_cache_instance.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_cache_instance.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_channel_instance.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_channel_instance.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_data_server.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_data_server.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_element.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_element.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_element_category.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_element_category.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_element_template.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_element_template.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_enumeration_set.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_enumeration_set.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_enumeration_value.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_enumeration_value.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_event_frame.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_event_frame.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_item_attribute.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_item_attribute.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_item_element.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_item_element.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_item_event_frame.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_item_event_frame.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_item_point.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_item_point.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_items_substatus.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_items_substatus.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_point.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_point.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_point_attribute.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_point_attribute.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_security_entry.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_security_entry.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_security_identity.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_security_identity.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_security_mapping.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_security_mapping.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_security_rights.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_security_rights.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_stream_summaries.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_stream_summaries.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_stream_value.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_stream_value.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_stream_values.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_stream_values.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_substatus.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_substatus.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_summary_value.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_summary_value.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_table.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_table.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_table_category.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_table_category.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_time_rule_plug_in.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_time_rule_plug_in.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_items_unit_class.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_items_unit_class.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_landing.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_landing.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_landing_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_landing_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_pagination_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_pagination_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_point.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_point.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_point_attribute.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_point_attribute.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_point_attribute_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_point_attribute_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_point_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_point_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_property_error.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_property_error.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_request.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_request.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_request_template.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_request_template.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_response.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_response.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_search_by_attribute.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_search_by_attribute.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security_entry.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security_entry.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security_entry_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security_entry_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security_identity.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security_identity.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security_identity_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security_identity_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security_mapping.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security_mapping.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security_mapping_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security_mapping_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security_rights.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security_rights.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_security_rights_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_security_rights_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_stream_summaries.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_stream_summaries.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_stream_summaries_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_stream_summaries_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_stream_value.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_stream_value.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_stream_value_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_stream_value_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_stream_values.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_stream_values.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_stream_values_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_stream_values_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_substatus.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_substatus.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_summary_value.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_summary_value.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_system_landing.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_system_landing.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_system_landing_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_system_landing_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_system_status.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_system_status.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_table.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_table.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_table_category.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_table_category.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_table_category_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_table_category_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_table_data.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_table_data.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_table_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_table_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_time_rule.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_time_rule.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_time_rule_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_time_rule_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_time_rule_plug_in.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_time_rule_plug_in.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_time_rule_plug_in_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_time_rule_plug_in_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_timed_value.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_timed_value.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_timed_values.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_timed_values.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_unit.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_unit.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_unit_class.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_unit_class.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_unit_class_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_unit_class_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_unit_links.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_unit_links.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_user_info.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_user_info.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_value.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_value.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_value_query.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_value_query.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_version.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_version.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/models/pi_web_exception.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/models/pi_web_exception.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/pi_web_api_client.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/pi_web_api_client.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/rest.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/rest.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/web_id/__init__.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/web_id/__init__.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/web_id/web_id_exception.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/web_id/web_id_exception.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/web_id/web_id_helper.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/web_id/web_id_helper.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/web_id/web_id_info.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/web_id/web_id_info.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/web_id/web_id_string_type.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/web_id/web_id_string_type.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft/pidevclub/piwebapi/web_id/web_id_type.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft/pidevclub/piwebapi/web_id/web_id_type.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft.pidevclub.piwebapi_thompsonp17.egg-info/PKG-INFO` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft.pidevclub.piwebapi_thompsonp17.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osisoft.pidevclub.piwebapi-thompsonp17
-Version: 1.1.5
+Version: 1.2.0
 Summary: PI Web API client library for Python (2017 R2)
 Home-page: https://github.com/osimloeff/PI-Web-API-Client-Python
 Author: Marcos Vainer Loeff
 Author-email: mloeff@osisoft.com
 License: MIT
 Keywords: PI Web API
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/osisoft.pidevclub.piwebapi_thompsonp17.egg-info/SOURCES.txt` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/osisoft.pidevclub.piwebapi_thompsonp17.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/setup.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	See the License for the specific language governing permissions and
 	limitations under the License.
 """
 
 from setuptools import setup, find_packages
 
 NAME = "osisoft.pidevclub.piwebapi-thompsonp17"
-VERSION = "1.1.5"
+VERSION = "1.2.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/test/test_data.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/test/test_data.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/test/test_main.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/test/test_webids.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/test/test_webids.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/utils/arg_hash_functions.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/utils/arg_hash_functions.py`

 * *Files identical despite different names*

### Comparing `osisoft.pidevclub.piwebapi-thompsonp17-1.1.5/utils/mock_generators.py` & `osisoft_pidevclub_piwebapi_thompsonp17-1.2.0/utils/mock_generators.py`

 * *Files identical despite different names*

