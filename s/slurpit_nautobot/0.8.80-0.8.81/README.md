# Comparing `tmp/slurpit_nautobot-0.8.80.tar.gz` & `tmp/slurpit_nautobot-0.8.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurpit_nautobot-0.8.80.tar", max compression
+gzip compressed data, was "slurpit_nautobot-0.8.81.tar", max compression
```

## Comparing `slurpit_nautobot-0.8.80.tar` & `slurpit_nautobot-0.8.81.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1064 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.80/LICENSE
--rw-r--r--   0        0        0     1220 2024-04-18 00:21:17.300831 slurpit_nautobot-0.8.80/README.md
--rw-r--r--   0        0        0      559 2024-04-18 10:06:41.716558 slurpit_nautobot-0.8.80/pyproject.toml
--rw-r--r--   0        0        0     1262 2024-04-18 10:06:41.716558 slurpit_nautobot-0.8.80/src/slurpit_nautobot/__init__.py
--rw-r--r--   0        0        0       46 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/api/__init__.py
--rw-r--r--   0        0        0     1993 2024-04-18 00:21:17.304831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/api/serializers.py
--rw-r--r--   0        0        0      484 2024-03-17 21:19:15.970312 slurpit_nautobot-0.8.80/src/slurpit_nautobot/api/urls.py
--rw-r--r--   0        0        0     9406 2024-04-18 00:21:17.304831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/api/views.py
--rw-r--r--   0        0        0     2547 2024-04-18 00:21:17.304831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/decorators.py
--rw-r--r--   0        0        0     2040 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/filtersets.py
--rw-r--r--   0        0        0     7715 2024-04-18 00:21:17.304831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/forms.py
--rw-r--r--   0        0        0    10767 2024-04-18 00:21:17.308831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/importer.py
--rw-r--r--   0        0        0        0 2024-04-18 10:06:41.812558 slurpit_nautobot-0.8.80/src/slurpit_nautobot/management/__init__.py
--rw-r--r--   0        0        0     1159 2024-04-18 00:21:17.308831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/management/choices.py
--rw-r--r--   0        0        0     9517 2024-04-18 00:21:17.308831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-18 10:06:41.812558 slurpit_nautobot-0.8.80/src/slurpit_nautobot/migrations/__init__.py
--rw-r--r--   0        0        0     5071 2024-04-18 00:21:17.312831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/models/__init__.py
--rw-r--r--   0        0        0     3069 2024-04-18 00:21:17.312831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/models/device.py
--rw-r--r--   0        0        0     1409 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/models/logs.py
--rw-r--r--   0        0        0      411 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/models/mapping.py
--rw-r--r--   0        0        0      844 2024-04-18 00:21:17.312831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/models/planning.py
--rw-r--r--   0        0        0     1146 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/models/setting.py
--rw-r--r--   0        0        0     1975 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/navigation.py
--rw-r--r--   0        0        0      101 2024-04-18 00:21:17.316831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/references/__init__.py
--rw-r--r--   0        0        0     1888 2024-04-18 00:21:17.316831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/references/generic.py
--rw-r--r--   0        0        0      648 2024-04-18 00:21:17.316831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/references/imports.py
--rw-r--r--   0        0        0      286 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/search.py
--rw-r--r--   0        0        0      528 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/slurpitch.py
--rw-r--r--   0        0        0     7586 2024-04-18 00:21:17.320831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/tables.py
--rw-r--r--   0        0        0     1506 2024-04-18 00:21:17.320831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/template_content.py
--rw-r--r--   0        0        0     3832 2024-04-18 00:21:17.320831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html
--rw-r--r--   0        0        0     1623 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html
--rw-r--r--   0        0        0     3425 2024-04-18 00:21:17.320831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html
--rw-r--r--   0        0        0    22100 2024-04-18 00:21:17.324832 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html
--rw-r--r--   0        0        0      352 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/commingsoon.html
--rw-r--r--   0        0        0    17659 2024-04-18 00:21:17.324832 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html
--rw-r--r--   0        0        0     3637 2024-04-18 00:21:17.324832 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html
--rw-r--r--   0        0        0     3623 2024-04-18 00:21:17.324832 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html
--rw-r--r--   0        0        0     6638 2024-04-18 00:21:17.328832 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html
--rw-r--r--   0        0        0      475 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/onboarded_device_list.html
--rw-r--r--   0        0        0     3628 2024-04-18 00:21:17.328832 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html
--rw-r--r--   0        0        0     4553 2024-04-18 00:21:17.328832 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html
--rw-r--r--   0        0        0     3177 2024-04-18 00:21:17.328832 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html
--rw-r--r--   0        0        0     9331 2024-04-18 00:21:17.328832 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html
--rw-r--r--   0        0        0     2368 2024-04-18 00:21:17.328832 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html
--rw-r--r--   0        0        0     2841 2024-04-18 00:21:17.328832 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html
--rw-r--r--   0        0        0     2915 2024-04-18 00:21:17.332831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/table.html
--rw-r--r--   0        0        0      350 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/table1.html
--rw-r--r--   0        0        0     1162 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/urls.py
--rw-r--r--   0        0        0      459 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/utilities.py
--rw-r--r--   0        0        0     1490 2024-04-18 00:21:17.332831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/validator.py
--rw-r--r--   0        0        0      298 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/views/__init__.py
--rw-r--r--   0        0        0    10493 2024-04-18 00:21:17.332831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/views/datamapping.py
--rw-r--r--   0        0        0     1073 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/views/logging.py
--rw-r--r--   0        0        0    14365 2024-04-18 00:21:17.332831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/views/onboarding.py
--rw-r--r--   0        0        0      520 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.80/src/slurpit_nautobot/views/reconcile.py
--rw-r--r--   0        0        0    18895 2024-04-18 00:21:17.332831 slurpit_nautobot-0.8.80/src/slurpit_nautobot/views/setting.py
--rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 slurpit_nautobot-0.8.80/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.81/LICENSE
+-rw-r--r--   0        0        0     1220 2024-05-24 06:48:01.996611 slurpit_nautobot-0.8.81/README.md
+-rw-r--r--   0        0        0      559 2024-05-24 06:48:02.008611 slurpit_nautobot-0.8.81/pyproject.toml
+-rw-r--r--   0        0        0     1262 2024-05-24 06:48:02.008611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/__init__.py
+-rw-r--r--   0        0        0       46 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/api/__init__.py
+-rw-r--r--   0        0        0     1993 2024-05-24 06:48:02.012611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/api/serializers.py
+-rw-r--r--   0        0        0      484 2024-03-17 21:19:15.970312 slurpit_nautobot-0.8.81/src/slurpit_nautobot/api/urls.py
+-rw-r--r--   0        0        0     9406 2024-05-24 06:48:02.012611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/api/views.py
+-rw-r--r--   0        0        0     2547 2024-05-24 06:48:02.012611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/decorators.py
+-rw-r--r--   0        0        0     2040 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/filtersets.py
+-rw-r--r--   0        0        0     7883 2024-05-24 06:48:02.012611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/forms.py
+-rw-r--r--   0        0        0    11707 2024-05-24 06:48:02.012611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/importer.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:48:02.204612 slurpit_nautobot-0.8.81/src/slurpit_nautobot/management/__init__.py
+-rw-r--r--   0        0        0     1159 2024-05-24 06:48:02.012611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/management/choices.py
+-rw-r--r--   0        0        0     9517 2024-05-24 06:48:02.016611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:48:02.220613 slurpit_nautobot-0.8.81/src/slurpit_nautobot/migrations/__init__.py
+-rw-r--r--   0        0        0     5071 2024-05-24 06:48:02.016611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/models/__init__.py
+-rw-r--r--   0        0        0     3069 2024-05-24 06:48:02.016611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/models/device.py
+-rw-r--r--   0        0        0     1409 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/models/logs.py
+-rw-r--r--   0        0        0      411 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/models/mapping.py
+-rw-r--r--   0        0        0      844 2024-05-24 06:48:02.020611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/models/planning.py
+-rw-r--r--   0        0        0     1146 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/models/setting.py
+-rw-r--r--   0        0        0     1975 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/navigation.py
+-rw-r--r--   0        0        0      101 2024-05-24 06:48:02.020611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/references/__init__.py
+-rw-r--r--   0        0        0     2200 2024-05-24 06:48:02.024611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/references/generic.py
+-rw-r--r--   0        0        0      742 2024-05-24 06:48:02.024611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/references/imports.py
+-rw-r--r--   0        0        0      286 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/search.py
+-rw-r--r--   0        0        0      528 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/slurpitch.py
+-rw-r--r--   0        0        0     7586 2024-05-24 06:48:02.024611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/tables.py
+-rw-r--r--   0        0        0     1506 2024-05-24 06:48:02.024611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/template_content.py
+-rw-r--r--   0        0        0     3832 2024-05-24 06:48:02.028611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html
+-rw-r--r--   0        0        0     1623 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html
+-rw-r--r--   0        0        0     3425 2024-05-24 06:48:02.028611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html
+-rw-r--r--   0        0        0    22100 2024-05-24 06:48:02.028611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html
+-rw-r--r--   0        0        0      352 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/commingsoon.html
+-rw-r--r--   0        0        0    17659 2024-05-24 06:48:02.032611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html
+-rw-r--r--   0        0        0     3637 2024-05-24 06:48:02.032611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html
+-rw-r--r--   0        0        0     3623 2024-05-24 06:48:02.036611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html
+-rw-r--r--   0        0        0     6638 2024-05-24 06:48:02.036611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html
+-rw-r--r--   0        0        0      475 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/onboarded_device_list.html
+-rw-r--r--   0        0        0     3628 2024-05-24 06:48:02.040611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html
+-rw-r--r--   0        0        0     4553 2024-05-24 06:48:02.040611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html
+-rw-r--r--   0        0        0     3177 2024-05-24 06:48:02.040611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html
+-rw-r--r--   0        0        0     9331 2024-05-24 06:48:02.044611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html
+-rw-r--r--   0        0        0     2368 2024-05-24 06:48:02.040611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html
+-rw-r--r--   0        0        0     2841 2024-05-24 06:48:02.044611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html
+-rw-r--r--   0        0        0     2915 2024-05-24 06:48:02.048611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/table.html
+-rw-r--r--   0        0        0      350 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/table1.html
+-rw-r--r--   0        0        0     1162 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/urls.py
+-rw-r--r--   0        0        0      459 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/utilities.py
+-rw-r--r--   0        0        0     1490 2024-05-24 06:48:02.048611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/validator.py
+-rw-r--r--   0        0        0      298 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/views/__init__.py
+-rw-r--r--   0        0        0    10493 2024-05-24 06:48:02.048611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/views/datamapping.py
+-rw-r--r--   0        0        0     1073 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/views/logging.py
+-rw-r--r--   0        0        0    16665 2024-05-24 06:48:02.048611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/views/onboarding.py
+-rw-r--r--   0        0        0      520 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.81/src/slurpit_nautobot/views/reconcile.py
+-rw-r--r--   0        0        0    18895 2024-05-24 06:48:02.052611 slurpit_nautobot-0.8.81/src/slurpit_nautobot/views/setting.py
+-rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 slurpit_nautobot-0.8.81/PKG-INFO
```

### Comparing `slurpit_nautobot-0.8.80/LICENSE` & `slurpit_nautobot-0.8.81/LICENSE`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/README.md` & `slurpit_nautobot-0.8.81/README.md`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/pyproject.toml` & `slurpit_nautobot-0.8.81/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slurpit_nautobot"
-version = "0.8.80"
+version = "0.8.81"
 description = ""
 authors = ["Pieter <pieter@slurpit.io>"]
 readme = "README.md"
 packages = [{include = "slurpit_nautobot", from = "src"}]
 
 
 [tool.poetry.dependencies]
```

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/__init__.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nautobot.apps import NautobotAppConfig
 from nautobot.apps import config as app_config
 
 class SlurpitConfig(NautobotAppConfig):
     name = "slurpit_nautobot"
     verbose_name = "Slurp'it Plugin"
     description = "Sync Slurp'it into Nautobot"
-    version = '0.8.80'
+    version = '0.8.81'
     base_url = "slurpit"   
     default_settings = {
         'DeviceType': {'model': "Slurp'it"},
         'Role': {'name': "Slurp'it"},
         'Location': {'name': 'Slurp\'it'},
         'LocationType': {'name': 'Slurp\'it'},
         'Region': {'name': 'Slurp\'it'},
```

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/api/serializers.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/api/serializers.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/api/views.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/api/views.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/decorators.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/decorators.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/filtersets.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/filtersets.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/forms.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,22 @@
 from django.contrib.contenttypes.models import ContentType
 # from nautobot.ipam.models import IPRange
 from nautobot.extras.models.tags import Tag
 
 
 class OnboardingForm(NautobotBulkEditForm):
     pk = forms.ModelMultipleChoiceField(queryset=SlurpitImportedDevice.objects.all(), widget=forms.MultipleHiddenInput())
+    
+    interface_name = forms.CharField(
+        label=_('Management Interface'),
+        initial='Management1',
+        max_length=200,
+        required=True
+    )
+
     device_type = forms.ChoiceField(
         choices=[],
         label=_('Device type'),
         required=True
     )
     location = DynamicModelChoiceField(
         label=_('Location'),
```

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/importer.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/importer.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,20 @@
 from django.utils import timezone
 from django.db.models.expressions import RawSQL
 
 from . import get_config
 from .models import SlurpitImportedDevice, SlurpitStagedDevice, ensure_slurpit_tags, SlurpitLog, SlurpitSetting, SlurpitPlanning, SlurpitSnapshot
 from .management.choices import *
 from .references import base_name, plugin_type, custom_field_data_name
-from .references.generic import get_default_objects, status_inventory, status_offline, get_create_dcim_objects, set_device_custom_fields
+from .references.generic import get_default_objects, status_inventory, status_offline, get_create_dcim_objects, set_device_custom_fields, status_active_for_ipaddress, status_active_for_interface, status_active_for_prefix
 from .references.imports import *
 
+from nautobot.dcim.models import Interface
+from nautobot.ipam.models import IPAddress
+
 BATCH_SIZE = 256
 columns = ('slurpit_id', 'disabled', 'hostname', 'fqdn', 'ipv4', 'device_os', 'device_type', 'brand', 'createddate', 'changeddate')
 
 
 def get_devices(offset):
     try:
         setting = SlurpitSetting.objects.get()
@@ -176,14 +179,16 @@
             to_import.append(device)
         SlurpitImportedDevice.objects.bulk_update(to_import, fields={'mapped_device_id'})
         offset += BATCH_SIZE
 
 def get_dcim_device(staged: SlurpitStagedDevice | SlurpitImportedDevice, **extra) -> Device:
     kw = get_default_objects()
     cf = extra.pop(custom_field_data_name, {})
+    interface_name = extra.pop('interface_name', 'management1')
+
     cf.update({
         'slurpit_hostname': staged.hostname,
         'slurpit_fqdn': staged.fqdn,
         'slurpit_platform': staged.device_os,
         'slurpit_manufacturer': staged.brand,
         'slurpit_devicetype': staged.device_type,
         'slurpit_ipv4': staged.ipv4
@@ -197,14 +202,31 @@
         # 'primary_ip4_id': int(ip_address(staged.fqdn)),
     })
     if 'device_type' not in extra and staged.mapped_devicetype is not None:
         kw['device_type'] = staged.mapped_devicetype
     kw.setdefault('status', status_inventory())
     device = Device.objects.create(**kw)
     ensure_slurpit_tags(device)
+
+    # Interface for new device.
+    if staged.ipv4:
+        interface = Interface.objects.create(name=interface_name, device=device, type='other', status=status_active_for_interface())
+        
+        address = f'{staged.ipv4}/32'
+        ipaddress = IPAddress.objects.filter(address=address)
+        if ipaddress:
+            ipaddress = ipaddress.first()
+        else:
+            prefix = Prefix.objects.create(prefix=address, status=status_active_for_prefix())
+            ipaddress = IPAddress.objects.create(address=address, status=status_active_for_ipaddress())
+        ipaddress.assigned_object = interface
+        ipaddress.save()
+        device.primary_ip4 = ipaddress
+        device.save()
+
     return device
 
 def get_from_staged(
         staged: SlurpitStagedDevice,
         add_dcim: bool
 ) -> SlurpitImportedDevice:
     device = SlurpitImportedDevice()
```

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/management/choices.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/management/choices.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/migrations/0001_initial.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/models/__init__.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/models/device.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/models/device.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/models/logs.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/models/logs.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/models/planning.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/models/planning.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/models/setting.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/models/setting.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/navigation.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/navigation.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/references/generic.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/references/generic.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,14 +27,23 @@
 
 def status_inventory():
     return Status.objects.get_for_model(Device).get(name="Inventory")
 
 def status_offline():
     return Status.objects.get_for_model(Device).get(name="Offline")
 
+def status_active_for_interface():
+    return Status.objects.get_for_model(Interface).get(name="Active")
+
+def status_active_for_ipaddress():
+    return Status.objects.get_for_model(IPAddress).get(name="Active")
+
+def status_active_for_prefix():
+    return Status.objects.get_for_model(Prefix).get(name="Active")
+
 def get_create_dcim_objects(staged: SlurpitStagedDevice):
     manu, new = Manufacturer.objects.get_or_create(name=staged.brand)
     platform, new = Platform.objects.get_or_create(name=staged.device_os)
     dtype, new = DeviceType.objects.get_or_create(model=staged.device_type, manufacturer=manu)
     if new:
         ensure_slurpit_tags(dtype)
     return dtype
```

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/references/imports.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/references/imports.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,7 +5,9 @@
 from nautobot.dcim.choices import DeviceStatusChoices
 from nautobot.dcim.filters import DeviceFilterSet
 from nautobot.dcim.models import  Manufacturer, Platform, DeviceType, Device, Location, LocationType
 from nautobot.extras.api.views import ConfigContextQuerySetMixin, NautobotModelViewSet
 from nautobot.extras.models import CustomField, Status, Role
 from nautobot.extras.models.tags import Tag
 from nautobot.tenancy.models import Tenant
+from nautobot.dcim.models import Interface
+from nautobot.ipam.models import IPAddress, Prefix
```

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/slurpitch.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/slurpitch.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/tables.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/tables.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/template_content.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/template_content.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/templates/slurpit_nautobot/table.html` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/templates/slurpit_nautobot/table.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/urls.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/urls.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/validator.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/validator.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/views/datamapping.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/views/datamapping.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/views/logging.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/views/logging.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/views/onboarding.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/views/onboarding.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from .. import get_config, forms, importer, models, tables
 from ..models import SlurpitImportedDevice, SlurpitLog, SlurpitSetting
 from ..management.choices import *
 from ..importer import get_dcim_device, import_from_queryset, run_import, get_devices, BATCH_SIZE, import_devices, process_import, start_device_import
 from ..decorators import slurpit_plugin_registered
 from ..references import base_name, custom_field_data_name
-from ..references.generic import create_form, get_form_device_data, SlurpitViewMixim, get_default_objects, set_device_custom_fields, status_inventory
+from ..references.generic import create_form, get_form_device_data, SlurpitViewMixim, get_default_objects, set_device_custom_fields, status_inventory, status_active_for_interface, status_active_for_ipaddress, status_active_for_prefix
 from ..references.imports import * 
 
 from django.http import HttpResponse, HttpResponseRedirect, JsonResponse
 
 @method_decorator(slurpit_plugin_registered, name='dispatch')
 class SlurpitImportedDeviceListView(SlurpitViewMixim, generic.ObjectListView):
     conflicted_queryset = models.SlurpitImportedDevice.objects.filter(mapped_device_id__isnull=True, hostname__in=Device.objects.values('name'))
@@ -167,14 +167,35 @@
 
                     manu = Manufacturer.objects.get(name=obj.brand)
                     device.device_type = DeviceType.objects.get(model=obj.device_type, manufacturer=manu)
                     device.platform = Platform.objects.get(name=obj.device_os)
                     device.save()
                     obj.save()
 
+                    # Interface
+                    if obj.ipv4:
+                        interface = Interface.objects.filter(device=device)
+                        if interface:
+                            interface = interface.first()
+                        else:
+                            interface = Interface.objects.create(name='management1', device=device, type='other', status=status_active_for_interface())
+
+                        address = f'{obj.ipv4}/32'
+                        ipaddress = IPAddress.objects.filter(address=address)
+                        if ipaddress:
+                            ipaddress = ipaddress.first()
+                        else:
+                            prefix = Prefix.objects.create(prefix=address, status=status_active_for_prefix())
+                            ipaddress = IPAddress.objects.create(address=address, status=status_active_for_ipaddress())
+                        
+                        ipaddress.assigned_object = interface
+                        ipaddress.save()
+                        device.primary_ip4 = ipaddress
+                        device.save()
+
                     log_message = f"Migration of onboarded device - {obj.hostname} successfully updated."
                     SlurpitLog.success(category=LogCategoryChoices.ONBOARD, message=log_message)
                 
                 msg = f'Migration is done successfully.'
                 messages.success(self.request, msg)
 
                 return redirect(self.get_return_url(request))
@@ -199,14 +220,35 @@
 
                     manu = Manufacturer.objects.get(name=obj.brand)
                     device.device_type = DeviceType.objects.get(model=obj.device_type, manufacturer=manu)
                     device.platform = Platform.objects.get(name=obj.device_os)
                     device.save()
                     obj.save()
 
+                    # Interface
+                    if obj.ipv4:
+                        interface = Interface.objects.filter(device=device)
+                        if interface:
+                            interface = interface.first()
+                        else:
+                            interface = Interface.objects.create(name='management1', device=device, type='other')
+
+                        address = f'{obj.ipv4}/32'
+                        ipaddress = IPAddress.objects.filter(address=address)
+                        if ipaddress:
+                            ipaddress = ipaddress.first()
+                        else:
+                            prefix = Prefix.objects.create(prefix=address, status=status_active_for_prefix())
+                            ipaddress = IPAddress.objects.create(address=address, status=status_active_for_ipaddress())
+                        
+                        ipaddress.assigned_object = interface
+                        ipaddress.save()
+                        device.primary_ip4 = ipaddress
+                        device.save()
+
                     log_message = f"Conflicted device resolved - {obj.hostname} successfully updated."
                     SlurpitLog.success(category=LogCategoryChoices.ONBOARD, message=log_message)
                 
                 msg = f'Conflicts successfully resolved.'
                 messages.success(self.request, msg)
 
                 return redirect(self.get_return_url(request))
```

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/views/reconcile.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/views/reconcile.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/src/slurpit_nautobot/views/setting.py` & `slurpit_nautobot-0.8.81/src/slurpit_nautobot/views/setting.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.80/PKG-INFO` & `slurpit_nautobot-0.8.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurpit_nautobot
-Version: 0.8.80
+Version: 0.8.81
 Summary: 
 Author: Pieter
 Author-email: pieter@slurpit.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

