# Comparing `tmp/netbox-vlan-manager-0.1.2.tar.gz` & `tmp/netbox_vlan_manager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-vlan-manager-0.1.2.tar", last modified: Wed Jul 12 14:29:54 2023, max compression
+gzip compressed data, was "netbox_vlan_manager-0.2.0.tar", last modified: Fri May 24 11:16:28 2024, max compression
```

## Comparing `netbox-vlan-manager-0.1.2.tar` & `netbox_vlan_manager-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:29:54.268277 netbox-vlan-manager-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-12 14:29:54.268277 netbox-vlan-manager-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:29:54.264277 netbox-vlan-manager-0.1.2/netbox_vlan_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:29:54.264277 netbox-vlan-manager-0.1.2/netbox_vlan_manager/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:29:54.268277 netbox-vlan-manager-0.1.2/netbox_vlan_manager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:29:54.264277 netbox-vlan-manager-0.1.2/netbox_vlan_manager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:29:54.268277 netbox-vlan-manager-0.1.2/netbox_vlan_manager/templates/netbox_vlan_manager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:29:54.268277 netbox-vlan-manager-0.1.2/netbox_vlan_manager/templates/netbox_vlan_manager/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/templates/netbox_vlan_manager/inc/toggle_available.html
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/templates/netbox_vlan_manager/vlangroupset.html
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/templates/netbox_vlan_manager/vlangroupset_vlans.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:29:54.268277 netbox-vlan-manager-0.1.2/netbox_vlan_manager/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/templatetags/view_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:29:54.264277 netbox-vlan-manager-0.1.2/netbox_vlan_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-12 14:29:54.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-12 14:29:54.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:29:54.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:29:54.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 14:29:54.000000 netbox-vlan-manager-0.1.2/netbox_vlan_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:29:54.268277 netbox-vlan-manager-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-12 14:29:44.000000 netbox-vlan-manager-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:16:28.884600 netbox_vlan_manager-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-24 11:16:28.884600 netbox_vlan_manager-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:16:28.880600 netbox_vlan_manager-0.2.0/netbox_vlan_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:16:28.884600 netbox_vlan_manager-0.2.0/netbox_vlan_manager/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:16:28.884600 netbox_vlan_manager-0.2.0/netbox_vlan_manager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:16:28.880600 netbox_vlan_manager-0.2.0/netbox_vlan_manager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:16:28.884600 netbox_vlan_manager-0.2.0/netbox_vlan_manager/templates/netbox_vlan_manager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:16:28.884600 netbox_vlan_manager-0.2.0/netbox_vlan_manager/templates/netbox_vlan_manager/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/templates/netbox_vlan_manager/inc/toggle_available.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/templates/netbox_vlan_manager/vlangroupset.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/templates/netbox_vlan_manager/vlangroupset_vlans.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:16:28.884600 netbox_vlan_manager-0.2.0/netbox_vlan_manager/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/templatetags/view_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:16:28.884600 netbox_vlan_manager-0.2.0/netbox_vlan_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-24 11:16:28.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-24 11:16:28.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 11:16:28.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 11:16:28.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 11:16:28.000000 netbox_vlan_manager-0.2.0/netbox_vlan_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 11:16:28.884600 netbox_vlan_manager-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-24 11:16:24.000000 netbox_vlan_manager-0.2.0/setup.py
```

### Comparing `netbox-vlan-manager-0.1.2/LICENSE` & `netbox_vlan_manager-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.2/PKG-INFO` & `netbox_vlan_manager-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-vlan-manager
-Version: 0.1.2
+Version: 0.2.0
 Summary: VLAN Manager for multiple VLAN Groups
 Home-page: https://github.com/miyuk/netbox-vlan-manager/
 Author: miyuk
 Author-email: miyuk@miyuk.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
@@ -54,14 +54,21 @@
 - Available VLAN
   - Extract none used VID searching all VLAN Groups
 
 ## Compatibility
 
 This plugin requires NetBox `v3.4.0` or later because has migration scripts compatibility.
 
+The compatibility table between plugin versions and netbox is as follows.
+
+|NetBox version|Plugin version|
+|---|---|
+|3.x.x|0.1.x|
+|4.x.x|0.2.x|
+
 ## Installation
 
 The plugin is available as a Python package in PyPI and can be installed with pip:
 
 ```bash
 pip install netbox-vlan-manager
 ```
```

### Comparing `netbox-vlan-manager-0.1.2/README.md` & `netbox_vlan_manager-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -41,14 +41,21 @@
 - Available VLAN
   - Extract none used VID searching all VLAN Groups
 
 ## Compatibility
 
 This plugin requires NetBox `v3.4.0` or later because has migration scripts compatibility.
 
+The compatibility table between plugin versions and netbox is as follows.
+
+|NetBox version|Plugin version|
+|---|---|
+|3.x.x|0.1.x|
+|4.x.x|0.2.x|
+
 ## Installation
 
 The plugin is available as a Python package in PyPI and can be installed with pip:
 
 ```bash
 pip install netbox-vlan-manager
 ```
```

### Comparing `netbox-vlan-manager-0.1.2/netbox_vlan_manager/api/serializers.py` & `netbox_vlan_manager-0.2.0/netbox_vlan_manager/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.2/netbox_vlan_manager/api/views.py` & `netbox_vlan_manager-0.2.0/netbox_vlan_manager/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.2/netbox_vlan_manager/forms.py` & `netbox_vlan_manager-0.2.0/netbox_vlan_manager/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.2/netbox_vlan_manager/migrations/0001_initial.py` & `netbox_vlan_manager-0.2.0/netbox_vlan_manager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.2/netbox_vlan_manager/models.py` & `netbox_vlan_manager-0.2.0/netbox_vlan_manager/models.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.2/netbox_vlan_manager/navigation.py` & `netbox_vlan_manager-0.2.0/netbox_vlan_manager/navigation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from extras.plugins import PluginMenuItem, PluginMenuButton, PluginMenuItem
-from utilities.choices import ButtonColorChoices
+from netbox.plugins import PluginMenuItem, PluginMenuButton, PluginMenuItem
+from netbox.choices import ButtonColorChoices
 
 vlan_group_manager_buttons = [
     PluginMenuButton(
         link=f'plugins:netbox_vlan_manager:vlangroupset_add',
         title='Add',
         icon_class='mdi mdi-plus-thick',
         color=ButtonColorChoices.GREEN
```

### Comparing `netbox-vlan-manager-0.1.2/netbox_vlan_manager/tables.py` & `netbox_vlan_manager-0.2.0/netbox_vlan_manager/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.2/netbox_vlan_manager/templates/netbox_vlan_manager/inc/toggle_available.html` & `netbox_vlan_manager-0.2.0/netbox_vlan_manager/templates/netbox_vlan_manager/inc/toggle_available.html`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.2/netbox_vlan_manager/templates/netbox_vlan_manager/vlangroupset.html` & `netbox_vlan_manager-0.2.0/netbox_vlan_manager/templates/netbox_vlan_manager/vlangroupset.html`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.2/netbox_vlan_manager/templates/netbox_vlan_manager/vlangroupset_vlans.html` & `netbox_vlan_manager-0.2.0/netbox_vlan_manager/templates/netbox_vlan_manager/vlangroupset_vlans.html`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.2/netbox_vlan_manager/urls.py` & `netbox_vlan_manager-0.2.0/netbox_vlan_manager/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.2/netbox_vlan_manager/views.py` & `netbox_vlan_manager-0.2.0/netbox_vlan_manager/views.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.2/netbox_vlan_manager.egg-info/PKG-INFO` & `netbox_vlan_manager-0.2.0/netbox_vlan_manager.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-vlan-manager
-Version: 0.1.2
+Version: 0.2.0
 Summary: VLAN Manager for multiple VLAN Groups
 Home-page: https://github.com/miyuk/netbox-vlan-manager/
 Author: miyuk
 Author-email: miyuk@miyuk.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
@@ -54,14 +54,21 @@
 - Available VLAN
   - Extract none used VID searching all VLAN Groups
 
 ## Compatibility
 
 This plugin requires NetBox `v3.4.0` or later because has migration scripts compatibility.
 
+The compatibility table between plugin versions and netbox is as follows.
+
+|NetBox version|Plugin version|
+|---|---|
+|3.x.x|0.1.x|
+|4.x.x|0.2.x|
+
 ## Installation
 
 The plugin is available as a Python package in PyPI and can be installed with pip:
 
 ```bash
 pip install netbox-vlan-manager
 ```
```

### Comparing `netbox-vlan-manager-0.1.2/netbox_vlan_manager.egg-info/SOURCES.txt` & `netbox_vlan_manager-0.2.0/netbox_vlan_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.2/setup.py` & `netbox_vlan_manager-0.2.0/setup.py`

 * *Files identical despite different names*

