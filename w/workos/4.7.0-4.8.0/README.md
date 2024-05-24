# Comparing `tmp/workos-4.7.0.tar.gz` & `tmp/workos-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workos-4.7.0.tar", last modified: Fri May 17 14:02:34 2024, max compression
+gzip compressed data, was "workos-4.8.0.tar", last modified: Fri May 24 13:23:03 2024, max compression
```

## Comparing `workos-4.7.0.tar` & `workos-4.8.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:02:34.688580 workos-4.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-17 14:02:27.000000 workos-4.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-17 14:02:34.688580 workos-4.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-17 14:02:27.000000 workos-4.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:02:34.688580 workos-4.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-17 14:02:27.000000 workos-4.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:02:34.684580 workos-4.7.0/workos/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-17 14:02:27.000000 workos-4.7.0/workos/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-17 14:02:27.000000 workos-4.7.0/workos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-17 14:02:27.000000 workos-4.7.0/workos/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-17 14:02:27.000000 workos-4.7.0/workos/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-05-17 14:02:27.000000 workos-4.7.0/workos/directory_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-17 14:02:27.000000 workos-4.7.0/workos/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-17 14:02:27.000000 workos-4.7.0/workos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-17 14:02:27.000000 workos-4.7.0/workos/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-17 14:02:27.000000 workos-4.7.0/workos/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-17 14:02:27.000000 workos-4.7.0/workos/passwordless.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-17 14:02:27.000000 workos-4.7.0/workos/portal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:02:34.684580 workos-4.7.0/workos/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/audit_logs_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/directory_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/event_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/passwordless.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-17 14:02:27.000000 workos-4.7.0/workos/resources/user_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-05-17 14:02:27.000000 workos-4.7.0/workos/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)    43591 2024-05-17 14:02:27.000000 workos-4.7.0/workos/user_management.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:02:34.684580 workos-4.7.0/workos/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:02:27.000000 workos-4.7.0/workos/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-17 14:02:27.000000 workos-4.7.0/workos/utils/connection_types.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-17 14:02:27.000000 workos-4.7.0/workos/utils/pagination_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-17 14:02:27.000000 workos-4.7.0/workos/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-17 14:02:27.000000 workos-4.7.0/workos/utils/sso_provider_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-17 14:02:27.000000 workos-4.7.0/workos/utils/um_provider_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-17 14:02:27.000000 workos-4.7.0/workos/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-17 14:02:27.000000 workos-4.7.0/workos/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:02:34.684580 workos-4.7.0/workos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-17 14:02:34.000000 workos-4.7.0/workos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-17 14:02:34.000000 workos-4.7.0/workos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:02:34.000000 workos-4.7.0/workos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:02:32.000000 workos-4.7.0/workos.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-17 14:02:34.000000 workos-4.7.0/workos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 14:02:34.000000 workos-4.7.0/workos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:23:02.998345 workos-4.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-24 13:22:52.000000 workos-4.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-24 13:23:02.998345 workos-4.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-24 13:22:52.000000 workos-4.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 13:23:02.998345 workos-4.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-24 13:22:52.000000 workos-4.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:23:02.994345 workos-4.8.0/workos/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-24 13:22:52.000000 workos-4.8.0/workos/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-24 13:22:52.000000 workos-4.8.0/workos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-24 13:22:52.000000 workos-4.8.0/workos/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-24 13:22:52.000000 workos-4.8.0/workos/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-05-24 13:22:52.000000 workos-4.8.0/workos/directory_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-24 13:22:52.000000 workos-4.8.0/workos/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-24 13:22:52.000000 workos-4.8.0/workos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-24 13:22:52.000000 workos-4.8.0/workos/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-24 13:22:52.000000 workos-4.8.0/workos/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-24 13:22:52.000000 workos-4.8.0/workos/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-24 13:22:52.000000 workos-4.8.0/workos/portal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:23:02.998345 workos-4.8.0/workos/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:52.000000 workos-4.8.0/workos/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-24 13:22:52.000000 workos-4.8.0/workos/resources/audit_logs_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-24 13:22:52.000000 workos-4.8.0/workos/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-24 13:22:52.000000 workos-4.8.0/workos/resources/directory_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-24 13:22:52.000000 workos-4.8.0/workos/resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-24 13:22:52.000000 workos-4.8.0/workos/resources/event_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-24 13:22:52.000000 workos-4.8.0/workos/resources/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-24 13:22:52.000000 workos-4.8.0/workos/resources/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-24 13:22:52.000000 workos-4.8.0/workos/resources/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-24 13:22:52.000000 workos-4.8.0/workos/resources/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-24 13:22:52.000000 workos-4.8.0/workos/resources/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-24 13:22:52.000000 workos-4.8.0/workos/resources/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-05-24 13:22:52.000000 workos-4.8.0/workos/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46146 2024-05-24 13:22:52.000000 workos-4.8.0/workos/user_management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:23:02.998345 workos-4.8.0/workos/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:22:52.000000 workos-4.8.0/workos/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-24 13:22:52.000000 workos-4.8.0/workos/utils/connection_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-24 13:22:52.000000 workos-4.8.0/workos/utils/pagination_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-24 13:22:52.000000 workos-4.8.0/workos/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-24 13:22:52.000000 workos-4.8.0/workos/utils/sso_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-24 13:22:52.000000 workos-4.8.0/workos/utils/um_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-24 13:22:52.000000 workos-4.8.0/workos/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-24 13:22:52.000000 workos-4.8.0/workos/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:23:02.998345 workos-4.8.0/workos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-24 13:23:02.000000 workos-4.8.0/workos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-24 13:23:02.000000 workos-4.8.0/workos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:23:02.000000 workos-4.8.0/workos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:23:00.000000 workos-4.8.0/workos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-24 13:23:02.000000 workos-4.8.0/workos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 13:23:02.000000 workos-4.8.0/workos.egg-info/top_level.txt
```

### Comparing `workos-4.7.0/LICENSE` & `workos-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/PKG-INFO` & `workos-4.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 4.7.0
+Version: 4.8.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `workos-4.7.0/README.md` & `workos-4.8.0/README.md`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/setup.py` & `workos-4.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/audit_logs.py` & `workos-4.8.0/workos/audit_logs.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/client.py` & `workos-4.8.0/workos/client.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/directory_sync.py` & `workos-4.8.0/workos/directory_sync.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/events.py` & `workos-4.8.0/workos/events.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/exceptions.py` & `workos-4.8.0/workos/exceptions.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/mfa.py` & `workos-4.8.0/workos/mfa.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/organizations.py` & `workos-4.8.0/workos/organizations.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/passwordless.py` & `workos-4.8.0/workos/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/portal.py` & `workos-4.8.0/workos/portal.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/resources/audit_logs_export.py` & `workos-4.8.0/workos/resources/audit_logs_export.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/resources/base.py` & `workos-4.8.0/workos/resources/base.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/resources/directory_sync.py` & `workos-4.8.0/workos/resources/directory_sync.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/resources/event.py` & `workos-4.8.0/workos/resources/event.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/resources/list.py` & `workos-4.8.0/workos/resources/list.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/resources/mfa.py` & `workos-4.8.0/workos/resources/mfa.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/resources/organizations.py` & `workos-4.8.0/workos/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/resources/passwordless.py` & `workos-4.8.0/workos/resources/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/resources/sso.py` & `workos-4.8.0/workos/resources/sso.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/resources/user_management.py` & `workos-4.8.0/workos/resources/user_management.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,14 +71,32 @@
         authentication_response_dict = super(
             WorkOSRefreshTokenAuthenticationResponse, self
         ).to_dict()
 
         return authentication_response_dict
 
 
+class WorkOSEmailVerification(WorkOSBaseResource):
+    """Representation of a EmailVerification object as returned by WorkOS through User Management features.
+
+    Attributes:
+        OBJECT_FIELDS (list): List of fields a WorkOSEmailVerification comprises.
+    """
+
+    OBJECT_FIELDS = [
+        "id",
+        "user_id",
+        "email",
+        "expires_at",
+        "code",
+        "created_at",
+        "updated_at",
+    ]
+
+
 class WorkOSInvitation(WorkOSBaseResource):
     """Representation of an Invitation as returned by WorkOS through User Management features.
 
     Attributes:
         OBJECT_FIELDS (list): List of fields a WorkOSInvitation comprises.
     """
 
@@ -88,14 +106,15 @@
         "state",
         "accepted_at",
         "revoked_at",
         "expires_at",
         "token",
         "accept_invitation_url",
         "organization_id",
+        "inviter_user_id",
         "created_at",
         "updated_at",
     ]
 
 
 class WorkOSMagicAuth(WorkOSBaseResource):
     """Representation of a MagicAuth object as returned by WorkOS through User Management features.
@@ -111,14 +130,32 @@
         "expires_at",
         "code",
         "created_at",
         "updated_at",
     ]
 
 
+class WorkOSPasswordReset(WorkOSBaseResource):
+    """Representation of a PasswordReset object as returned by WorkOS through User Management features.
+
+    Attributes:
+        OBJECT_FIELDS (list): List of fields a WorkOSPasswordReset comprises.
+    """
+
+    OBJECT_FIELDS = [
+        "id",
+        "user_id",
+        "email",
+        "password_reset_token",
+        "password_reset_url",
+        "expires_at",
+        "created_at",
+    ]
+
+
 class WorkOSOrganizationMembership(WorkOSBaseResource):
     """Representation of an Organization Membership as returned by WorkOS through User Management features.
 
     Attributes:
         OBJECT_FIELDS (list): List of fields a WorkOSOrganizationMembership comprises.
     """
```

### Comparing `workos-4.7.0/workos/sso.py` & `workos-4.8.0/workos/sso.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/user_management.py` & `workos-4.8.0/workos/user_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 from warnings import warn
 import workos
 from workos.resources.list import WorkOSListResource
 from workos.resources.mfa import WorkOSAuthenticationFactorTotp, WorkOSChallenge
 from workos.resources.user_management import (
     WorkOSAuthenticationResponse,
     WorkOSRefreshTokenAuthenticationResponse,
+    WorkOSEmailVerification,
     WorkOSInvitation,
     WorkOSMagicAuth,
+    WorkOSPasswordReset,
     WorkOSOrganizationMembership,
     WorkOSPasswordChallengeResponse,
     WorkOSUser,
 )
 from workos.utils.pagination_order import Order
 from workos.utils.um_provider_types import UserManagementProviderType
 from workos.utils.request import (
@@ -40,17 +42,20 @@
 USER_RESET_PASSWORD_PATH = "user_management/password_reset/confirm"
 USER_SEND_VERIFICATION_EMAIL_PATH = "user_management/users/{0}/email_verification/send"
 USER_VERIFY_EMAIL_CODE_PATH = "user_management/users/{0}/email_verification/confirm"
 MAGIC_AUTH_DETAIL_PATH = "user_management/magic_auth/{0}"
 MAGIC_AUTH_PATH = "user_management/magic_auth"
 USER_SEND_MAGIC_AUTH_PATH = "user_management/magic_auth/send"
 USER_AUTH_FACTORS_PATH = "user_management/users/{0}/auth_factors"
+EMAIL_VERIFICATION_DETAIL_PATH = "user_management/email_verification/{0}"
 INVITATION_PATH = "user_management/invitations"
 INVITATION_DETAIL_PATH = "user_management/invitations/{0}"
 INVITATION_REVOKE_PATH = "user_management/invitations/{0}/revoke"
+PASSWORD_RESET_PATH = "user_management/password_reset"
+PASSWORD_RESET_DETAIL_PATH = "user_management/password_reset/{0}"
 
 RESPONSE_LIMIT = 10
 
 
 class UserManagement(WorkOSListResource):
     """Offers methods for using the WorkOS User Management API."""
 
@@ -808,43 +813,98 @@
     def get_jwks_url(self):
         """Get the public key that is used for verifying access tokens.
 
         Returns:
             (str): The public JWKS URL.
         """
 
-        return "%s/sso/jwks/%s" % (workos.base_api_url, workos.client_id)
+        return "%ssso/jwks/%s" % (workos.base_api_url, workos.client_id)
 
     def get_logout_url(self, session_id):
         """Get the URL for ending the session and redirecting the user
 
         Kwargs:
             session_id (str): The ID of the user's session
 
         Returns:
             (str): URL to redirect the user to to end the session.
         """
 
-        return "%s/user_management/sessions/logout?session_id=%s" % (
+        return "%suser_management/sessions/logout?session_id=%s" % (
             workos.base_api_url,
             session_id,
         )
 
+    def get_password_reset(self, password_reset_id):
+        """Get the details of a password reset object.
+
+        Args:
+            password_reset_id (str) -  The unique ID of the password reset object.
+
+        Returns:
+            dict: PasswordReset response from WorkOS.
+        """
+        headers = {}
+
+        response = self.request_helper.request(
+            PASSWORD_RESET_DETAIL_PATH.format(password_reset_id),
+            method=REQUEST_METHOD_GET,
+            headers=headers,
+            token=workos.api_key,
+        )
+
+        return WorkOSPasswordReset.construct_from_response(response).to_dict()
+
+    def create_password_reset(
+        self,
+        email,
+    ):
+        """Creates a password reset token that can be sent to a user's email to reset the password.
+
+        Args:
+            email: The email address of the user.
+
+        Returns:
+            dict: PasswordReset response from WorkOS.
+        """
+        headers = {}
+
+        params = {
+            "email": email,
+        }
+
+        response = self.request_helper.request(
+            PASSWORD_RESET_PATH,
+            method=REQUEST_METHOD_POST,
+            params=params,
+            headers=headers,
+            token=workos.api_key,
+        )
+
+        return WorkOSPasswordReset.construct_from_response(response).to_dict()
+
     def send_password_reset_email(
         self,
         email,
         password_reset_url,
     ):
         """Sends a password reset email to a user.
 
+        Deprecated: Please use `create_password_reset` instead. This method will be removed in a future major version.
+
         Kwargs:
             email (str): The email of the user that wishes to reset their password.
             password_reset_url (str): The URL that will be linked to in the email.
         """
 
+        warn(
+            "'send_password_reset_email' is deprecated. Please use 'create_password_reset' instead. This method will be removed in a future major version.",
+            DeprecationWarning,
+        )
+
         headers = {}
 
         payload = {
             "email": email,
             "password_reset_url": password_reset_url,
         }
 
@@ -884,14 +944,34 @@
             headers=headers,
             params=payload,
             token=workos.api_key,
         )
 
         return WorkOSUser.construct_from_response(response["user"]).to_dict()
 
+    def get_email_verification(self, email_verification_id):
+        """Get the details of an email verification object.
+
+        Args:
+            email_verificationh_id (str) -  The unique ID of the email verification object.
+
+        Returns:
+            dict: EmailVerification response from WorkOS.
+        """
+        headers = {}
+
+        response = self.request_helper.request(
+            EMAIL_VERIFICATION_DETAIL_PATH.format(email_verification_id),
+            method=REQUEST_METHOD_GET,
+            headers=headers,
+            token=workos.api_key,
+        )
+
+        return WorkOSEmailVerification.construct_from_response(response).to_dict()
+
     def send_verification_email(
         self,
         user_id,
     ):
         """Sends a verification email to the provided user.
 
         Kwargs:
```

### Comparing `workos-4.7.0/workos/utils/connection_types.py` & `workos-4.8.0/workos/utils/connection_types.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/utils/request.py` & `workos-4.8.0/workos/utils/request.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/utils/validation.py` & `workos-4.8.0/workos/utils/validation.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos/webhooks.py` & `workos-4.8.0/workos/webhooks.py`

 * *Files identical despite different names*

### Comparing `workos-4.7.0/workos.egg-info/PKG-INFO` & `workos-4.8.0/workos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 4.7.0
+Version: 4.8.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `workos-4.7.0/workos.egg-info/SOURCES.txt` & `workos-4.8.0/workos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

