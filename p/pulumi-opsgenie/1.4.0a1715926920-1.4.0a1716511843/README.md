# Comparing `tmp/pulumi_opsgenie-1.4.0a1715926920.tar.gz` & `tmp/pulumi_opsgenie-1.4.0a1716511843.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_opsgenie-1.4.0a1715926920.tar", last modified: Fri May 17 06:36:33 2024, max compression
+gzip compressed data, was "pulumi_opsgenie-1.4.0a1716511843.tar", last modified: Fri May 24 00:56:21 2024, max compression
```

## Comparing `pulumi_opsgenie-1.4.0a1715926920.tar` & `pulumi_opsgenie-1.4.0a1716511843.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:36:33.331712 pulumi_opsgenie-1.4.0a1715926920/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-17 06:36:33.331712 pulumi_opsgenie-1.4.0a1715926920/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:36:33.331712 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   170966 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    58178 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/alert_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    30384 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/api_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:36:33.331712 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/custom_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    19644 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/email_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/escalation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/get_escalation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/get_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/get_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/get_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/get_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    23914 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)    23476 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/incident_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    28366 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/integration_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (127)    36085 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/notification_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    29962 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/notification_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)   152017 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13728 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    25325 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/schedule_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13174 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13102 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/service_incident_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    19589 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    28124 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/team_routing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    26255 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/user_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:36:33.331712 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-17 06:36:33.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-17 06:36:33.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:36:33.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 06:36:33.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 06:36:33.000000 pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-17 06:36:25.000000 pulumi_opsgenie-1.4.0a1715926920/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:36:33.331712 pulumi_opsgenie-1.4.0a1715926920/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:56:21.333025 pulumi_opsgenie-1.4.0a1716511843/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-24 00:56:21.333025 pulumi_opsgenie-1.4.0a1716511843/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:56:21.333025 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   174024 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58178 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/alert_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30384 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/api_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:56:21.333025 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/custom_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19644 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/email_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/escalation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/get_escalation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/get_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/get_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23914 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24688 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/incident_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28366 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/integration_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36085 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/notification_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29962 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/notification_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154935 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13728 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25325 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/schedule_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13174 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13102 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/service_incident_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19589 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28124 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/team_routing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26255 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/user_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:56:21.333025 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-24 00:56:21.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-24 00:56:21.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 00:56:21.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 00:56:21.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 00:56:21.000000 pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-24 00:56:15.000000 pulumi_opsgenie-1.4.0a1716511843/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 00:56:21.333025 pulumi_opsgenie-1.4.0a1716511843/setup.cfg
```

### Comparing `pulumi_opsgenie-1.4.0a1715926920/PKG-INFO` & `pulumi_opsgenie-1.4.0a1716511843/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_opsgenie
-Version: 1.4.0a1715926920
+Version: 1.4.0a1716511843
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi,opsgenie
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_opsgenie-1.4.0a1715926920/README.md` & `pulumi_opsgenie-1.4.0a1716511843/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/__init__.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/_inputs.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3424,49 +3424,67 @@
 @pulumi.input_type
 class ScheduleRotationTimeRestrictionRestrictionArgs:
     def __init__(__self__, *,
                  end_hour: pulumi.Input[int],
                  end_min: pulumi.Input[int],
                  start_hour: pulumi.Input[int],
                  start_min: pulumi.Input[int]):
+        """
+        :param pulumi.Input[int] end_hour: Value of the hour that frame will end.
+        :param pulumi.Input[int] end_min: Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+        :param pulumi.Input[int] start_hour: Value of the hour that frame will start.
+        :param pulumi.Input[int] start_min: Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+        """
         pulumi.set(__self__, "end_hour", end_hour)
         pulumi.set(__self__, "end_min", end_min)
         pulumi.set(__self__, "start_hour", start_hour)
         pulumi.set(__self__, "start_min", start_min)
 
     @property
     @pulumi.getter(name="endHour")
     def end_hour(self) -> pulumi.Input[int]:
+        """
+        Value of the hour that frame will end.
+        """
         return pulumi.get(self, "end_hour")
 
     @end_hour.setter
     def end_hour(self, value: pulumi.Input[int]):
         pulumi.set(self, "end_hour", value)
 
     @property
     @pulumi.getter(name="endMin")
     def end_min(self) -> pulumi.Input[int]:
+        """
+        Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+        """
         return pulumi.get(self, "end_min")
 
     @end_min.setter
     def end_min(self, value: pulumi.Input[int]):
         pulumi.set(self, "end_min", value)
 
     @property
     @pulumi.getter(name="startHour")
     def start_hour(self) -> pulumi.Input[int]:
+        """
+        Value of the hour that frame will start.
+        """
         return pulumi.get(self, "start_hour")
 
     @start_hour.setter
     def start_hour(self, value: pulumi.Input[int]):
         pulumi.set(self, "start_hour", value)
 
     @property
     @pulumi.getter(name="startMin")
     def start_min(self) -> pulumi.Input[int]:
+        """
+        Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+        """
         return pulumi.get(self, "start_min")
 
     @start_min.setter
     def start_min(self, value: pulumi.Input[int]):
         pulumi.set(self, "start_min", value)
 
 
@@ -3475,69 +3493,99 @@
     def __init__(__self__, *,
                  end_day: pulumi.Input[str],
                  end_hour: pulumi.Input[int],
                  end_min: pulumi.Input[int],
                  start_day: pulumi.Input[str],
                  start_hour: pulumi.Input[int],
                  start_min: pulumi.Input[int]):
+        """
+        :param pulumi.Input[str] end_day: Value of the day that frame will end.
+        :param pulumi.Input[int] end_hour: Value of the hour that frame will end.
+        :param pulumi.Input[int] end_min: Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+               
+               Both `start_day` and `end_day` can assume only `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, or `sunday` values.
+        :param pulumi.Input[str] start_day: Value of the day that frame will start.
+        :param pulumi.Input[int] start_hour: Value of the hour that frame will start
+        :param pulumi.Input[int] start_min: Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+        """
         pulumi.set(__self__, "end_day", end_day)
         pulumi.set(__self__, "end_hour", end_hour)
         pulumi.set(__self__, "end_min", end_min)
         pulumi.set(__self__, "start_day", start_day)
         pulumi.set(__self__, "start_hour", start_hour)
         pulumi.set(__self__, "start_min", start_min)
 
     @property
     @pulumi.getter(name="endDay")
     def end_day(self) -> pulumi.Input[str]:
+        """
+        Value of the day that frame will end.
+        """
         return pulumi.get(self, "end_day")
 
     @end_day.setter
     def end_day(self, value: pulumi.Input[str]):
         pulumi.set(self, "end_day", value)
 
     @property
     @pulumi.getter(name="endHour")
     def end_hour(self) -> pulumi.Input[int]:
+        """
+        Value of the hour that frame will end.
+        """
         return pulumi.get(self, "end_hour")
 
     @end_hour.setter
     def end_hour(self, value: pulumi.Input[int]):
         pulumi.set(self, "end_hour", value)
 
     @property
     @pulumi.getter(name="endMin")
     def end_min(self) -> pulumi.Input[int]:
+        """
+        Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+
+        Both `start_day` and `end_day` can assume only `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, or `sunday` values.
+        """
         return pulumi.get(self, "end_min")
 
     @end_min.setter
     def end_min(self, value: pulumi.Input[int]):
         pulumi.set(self, "end_min", value)
 
     @property
     @pulumi.getter(name="startDay")
     def start_day(self) -> pulumi.Input[str]:
+        """
+        Value of the day that frame will start.
+        """
         return pulumi.get(self, "start_day")
 
     @start_day.setter
     def start_day(self, value: pulumi.Input[str]):
         pulumi.set(self, "start_day", value)
 
     @property
     @pulumi.getter(name="startHour")
     def start_hour(self) -> pulumi.Input[int]:
+        """
+        Value of the hour that frame will start
+        """
         return pulumi.get(self, "start_hour")
 
     @start_hour.setter
     def start_hour(self, value: pulumi.Input[int]):
         pulumi.set(self, "start_hour", value)
 
     @property
     @pulumi.getter(name="startMin")
     def start_min(self) -> pulumi.Input[int]:
+        """
+        Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+        """
         return pulumi.get(self, "start_min")
 
     @start_min.setter
     def start_min(self, value: pulumi.Input[int]):
         pulumi.set(self, "start_min", value)
 
 
@@ -3930,14 +3978,16 @@
                  expected_value: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  not_: Optional[pulumi.Input[bool]] = None,
                  order: Optional[pulumi.Input[int]] = None):
         """
         :param pulumi.Input[str] field: Specifies which alert field will be used in condition. Possible values are `message`, `alias`, `description`, `source`, `entity`, `tags`, `actions`, `extra-properties`, `recipients`, `teams` or `priority`.
         :param pulumi.Input[str] operation: It is the operation that will be executed for the given field and key. Possible operations are `matches`, `contains`, `starts-with`, `ends-with`, `equals`, `contains-key`, `contains-value`, `greater-than`, `less-than`, `is-empty` and `equals-ignore-whitespace`.
+               
+               * `expectedValue` - (Optional) User defined value that will be compared with alert field according to the operation. Default: empty string.
         :param pulumi.Input[str] key: If field is set as extra-properties, key could be used for key-value pair.
         :param pulumi.Input[bool] not_: Indicates behaviour of the given operation. Default value is false.
         :param pulumi.Input[int] order: Order of the condition in conditions list.
         """
         pulumi.set(__self__, "field", field)
         pulumi.set(__self__, "operation", operation)
         if expected_value is not None:
@@ -3962,14 +4012,16 @@
         pulumi.set(self, "field", value)
 
     @property
     @pulumi.getter
     def operation(self) -> pulumi.Input[str]:
         """
         It is the operation that will be executed for the given field and key. Possible operations are `matches`, `contains`, `starts-with`, `ends-with`, `equals`, `contains-key`, `contains-value`, `greater-than`, `less-than`, `is-empty` and `equals-ignore-whitespace`.
+
+        * `expectedValue` - (Optional) User defined value that will be compared with alert field according to the operation. Default: empty string.
         """
         return pulumi.get(self, "operation")
 
     @operation.setter
     def operation(self, value: pulumi.Input[str]):
         pulumi.set(self, "operation", value)
```

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/_utilities.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/alert_policy.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/alert_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/api_integration.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/api_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/config/vars.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/custom_role.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/custom_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/email_integration.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/email_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/escalation.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/escalation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/get_escalation.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/get_escalation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/get_heartbeat.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/get_heartbeat.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/get_schedule.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/get_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/get_service.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/get_team.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/get_user.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/heartbeat.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/incident_template.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/incident_template.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,18 @@
                  impacted_services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a IncidentTemplate resource.
         :param pulumi.Input[str] message: Message of the related incident template. This field must not be longer than 130 characters.
         :param pulumi.Input[str] priority: Priority level of the incident. Possible values are `P1`, `P2`, `P3`, `P4` and `P5`.
+               
+               * `impactedServices` (Optional) Impacted services of incident template. Maximum 20 services.
+               
+               * `stakeholderProperties` (Required)
         :param pulumi.Input[str] description: Description field of the incident template. This field must not be longer than 10000 characters.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] details: Map of key-value pairs to use as custom properties of the incident template. This field must not be longer than 8000 characters.
         :param pulumi.Input[str] name: Name of the incident template.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags of the incident template.
         """
         pulumi.set(__self__, "message", message)
         pulumi.set(__self__, "priority", priority)
@@ -60,14 +64,18 @@
         pulumi.set(self, "message", value)
 
     @property
     @pulumi.getter
     def priority(self) -> pulumi.Input[str]:
         """
         Priority level of the incident. Possible values are `P1`, `P2`, `P3`, `P4` and `P5`.
+
+        * `impactedServices` (Optional) Impacted services of incident template. Maximum 20 services.
+
+        * `stakeholderProperties` (Required)
         """
         return pulumi.get(self, "priority")
 
     @priority.setter
     def priority(self, value: pulumi.Input[str]):
         pulumi.set(self, "priority", value)
 
@@ -152,14 +160,18 @@
         """
         Input properties used for looking up and filtering IncidentTemplate resources.
         :param pulumi.Input[str] description: Description field of the incident template. This field must not be longer than 10000 characters.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] details: Map of key-value pairs to use as custom properties of the incident template. This field must not be longer than 8000 characters.
         :param pulumi.Input[str] message: Message of the related incident template. This field must not be longer than 130 characters.
         :param pulumi.Input[str] name: Name of the incident template.
         :param pulumi.Input[str] priority: Priority level of the incident. Possible values are `P1`, `P2`, `P3`, `P4` and `P5`.
+               
+               * `impactedServices` (Optional) Impacted services of incident template. Maximum 20 services.
+               
+               * `stakeholderProperties` (Required)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags of the incident template.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if details is not None:
             pulumi.set(__self__, "details", details)
         if impacted_services is not None:
@@ -233,14 +245,18 @@
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def priority(self) -> Optional[pulumi.Input[str]]:
         """
         Priority level of the incident. Possible values are `P1`, `P2`, `P3`, `P4` and `P5`.
+
+        * `impactedServices` (Optional) Impacted services of incident template. Maximum 20 services.
+
+        * `stakeholderProperties` (Required)
         """
         return pulumi.get(self, "priority")
 
     @priority.setter
     def priority(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "priority", value)
 
@@ -327,14 +343,18 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description field of the incident template. This field must not be longer than 10000 characters.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] details: Map of key-value pairs to use as custom properties of the incident template. This field must not be longer than 8000 characters.
         :param pulumi.Input[str] message: Message of the related incident template. This field must not be longer than 130 characters.
         :param pulumi.Input[str] name: Name of the incident template.
         :param pulumi.Input[str] priority: Priority level of the incident. Possible values are `P1`, `P2`, `P3`, `P4` and `P5`.
+               
+               * `impactedServices` (Optional) Impacted services of incident template. Maximum 20 services.
+               
+               * `stakeholderProperties` (Required)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags of the incident template.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: IncidentTemplateArgs,
@@ -455,14 +475,18 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description field of the incident template. This field must not be longer than 10000 characters.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] details: Map of key-value pairs to use as custom properties of the incident template. This field must not be longer than 8000 characters.
         :param pulumi.Input[str] message: Message of the related incident template. This field must not be longer than 130 characters.
         :param pulumi.Input[str] name: Name of the incident template.
         :param pulumi.Input[str] priority: Priority level of the incident. Possible values are `P1`, `P2`, `P3`, `P4` and `P5`.
+               
+               * `impactedServices` (Optional) Impacted services of incident template. Maximum 20 services.
+               
+               * `stakeholderProperties` (Required)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags of the incident template.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _IncidentTemplateState.__new__(_IncidentTemplateState)
 
         __props__.__dict__["description"] = description
@@ -513,14 +537,18 @@
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def priority(self) -> pulumi.Output[str]:
         """
         Priority level of the incident. Possible values are `P1`, `P2`, `P3`, `P4` and `P5`.
+
+        * `impactedServices` (Optional) Impacted services of incident template. Maximum 20 services.
+
+        * `stakeholderProperties` (Required)
         """
         return pulumi.get(self, "priority")
 
     @property
     @pulumi.getter(name="stakeholderProperties")
     def stakeholder_properties(self) -> pulumi.Output[Sequence['outputs.IncidentTemplateStakeholderProperty']]:
         return pulumi.get(self, "stakeholder_properties")
```

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/integration_action.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/integration_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/maintenance.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/maintenance.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/notification_policy.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/notification_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/notification_rule.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/notification_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/outputs.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3197,37 +3197,55 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  end_hour: int,
                  end_min: int,
                  start_hour: int,
                  start_min: int):
+        """
+        :param int end_hour: Value of the hour that frame will end.
+        :param int end_min: Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+        :param int start_hour: Value of the hour that frame will start.
+        :param int start_min: Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+        """
         pulumi.set(__self__, "end_hour", end_hour)
         pulumi.set(__self__, "end_min", end_min)
         pulumi.set(__self__, "start_hour", start_hour)
         pulumi.set(__self__, "start_min", start_min)
 
     @property
     @pulumi.getter(name="endHour")
     def end_hour(self) -> int:
+        """
+        Value of the hour that frame will end.
+        """
         return pulumi.get(self, "end_hour")
 
     @property
     @pulumi.getter(name="endMin")
     def end_min(self) -> int:
+        """
+        Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+        """
         return pulumi.get(self, "end_min")
 
     @property
     @pulumi.getter(name="startHour")
     def start_hour(self) -> int:
+        """
+        Value of the hour that frame will start.
+        """
         return pulumi.get(self, "start_hour")
 
     @property
     @pulumi.getter(name="startMin")
     def start_min(self) -> int:
+        """
+        Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+        """
         return pulumi.get(self, "start_min")
 
 
 @pulumi.output_type
 class ScheduleRotationTimeRestrictionRestrictionList(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3259,49 +3277,79 @@
     def __init__(__self__, *,
                  end_day: str,
                  end_hour: int,
                  end_min: int,
                  start_day: str,
                  start_hour: int,
                  start_min: int):
+        """
+        :param str end_day: Value of the day that frame will end.
+        :param int end_hour: Value of the hour that frame will end.
+        :param int end_min: Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+               
+               Both `start_day` and `end_day` can assume only `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, or `sunday` values.
+        :param str start_day: Value of the day that frame will start.
+        :param int start_hour: Value of the hour that frame will start
+        :param int start_min: Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+        """
         pulumi.set(__self__, "end_day", end_day)
         pulumi.set(__self__, "end_hour", end_hour)
         pulumi.set(__self__, "end_min", end_min)
         pulumi.set(__self__, "start_day", start_day)
         pulumi.set(__self__, "start_hour", start_hour)
         pulumi.set(__self__, "start_min", start_min)
 
     @property
     @pulumi.getter(name="endDay")
     def end_day(self) -> str:
+        """
+        Value of the day that frame will end.
+        """
         return pulumi.get(self, "end_day")
 
     @property
     @pulumi.getter(name="endHour")
     def end_hour(self) -> int:
+        """
+        Value of the hour that frame will end.
+        """
         return pulumi.get(self, "end_hour")
 
     @property
     @pulumi.getter(name="endMin")
     def end_min(self) -> int:
+        """
+        Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+
+        Both `start_day` and `end_day` can assume only `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, or `sunday` values.
+        """
         return pulumi.get(self, "end_min")
 
     @property
     @pulumi.getter(name="startDay")
     def start_day(self) -> str:
+        """
+        Value of the day that frame will start.
+        """
         return pulumi.get(self, "start_day")
 
     @property
     @pulumi.getter(name="startHour")
     def start_hour(self) -> int:
+        """
+        Value of the hour that frame will start
+        """
         return pulumi.get(self, "start_hour")
 
     @property
     @pulumi.getter(name="startMin")
     def start_min(self) -> int:
+        """
+        Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+        """
         return pulumi.get(self, "start_min")
 
 
 @pulumi.output_type
 class ServiceIncidentRuleIncidentRule(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3676,14 +3724,16 @@
                  expected_value: Optional[str] = None,
                  key: Optional[str] = None,
                  not_: Optional[bool] = None,
                  order: Optional[int] = None):
         """
         :param str field: Specifies which alert field will be used in condition. Possible values are `message`, `alias`, `description`, `source`, `entity`, `tags`, `actions`, `extra-properties`, `recipients`, `teams` or `priority`.
         :param str operation: It is the operation that will be executed for the given field and key. Possible operations are `matches`, `contains`, `starts-with`, `ends-with`, `equals`, `contains-key`, `contains-value`, `greater-than`, `less-than`, `is-empty` and `equals-ignore-whitespace`.
+               
+               * `expectedValue` - (Optional) User defined value that will be compared with alert field according to the operation. Default: empty string.
         :param str key: If field is set as extra-properties, key could be used for key-value pair.
         :param bool not_: Indicates behaviour of the given operation. Default value is false.
         :param int order: Order of the condition in conditions list.
         """
         pulumi.set(__self__, "field", field)
         pulumi.set(__self__, "operation", operation)
         if expected_value is not None:
@@ -3704,14 +3754,16 @@
         return pulumi.get(self, "field")
 
     @property
     @pulumi.getter
     def operation(self) -> str:
         """
         It is the operation that will be executed for the given field and key. Possible operations are `matches`, `contains`, `starts-with`, `ends-with`, `equals`, `contains-key`, `contains-value`, `greater-than`, `less-than`, `is-empty` and `equals-ignore-whitespace`.
+
+        * `expectedValue` - (Optional) User defined value that will be compared with alert field according to the operation. Default: empty string.
         """
         return pulumi.get(self, "operation")
 
     @property
     @pulumi.getter(name="expectedValue")
     def expected_value(self) -> Optional[str]:
         return pulumi.get(self, "expected_value")
```

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/provider.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/schedule.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/schedule_rotation.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/schedule_rotation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/service.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/service_incident_rule.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/service_incident_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/team.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/team_routing_rule.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/team_routing_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/user.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie/user_contact.py` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie/user_contact.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie.egg-info/PKG-INFO` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_opsgenie
-Version: 1.4.0a1715926920
+Version: 1.4.0a1716511843
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi,opsgenie
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pulumi_opsgenie.egg-info/SOURCES.txt` & `pulumi_opsgenie-1.4.0a1716511843/pulumi_opsgenie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1715926920/pyproject.toml` & `pulumi_opsgenie-1.4.0a1716511843/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_opsgenie"
   description = "A Pulumi package for creating and managing opsgenie cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "opsgenie"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "1.4.0a1715926920"
+  version = "1.4.0a1716511843"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-opsgenie"
 
 [build-system]
```

