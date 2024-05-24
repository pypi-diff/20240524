# Comparing `tmp/netbox_interface_synchronization-4.0.1.tar.gz` & `tmp/netbox_interface_synchronization-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_interface_synchronization-4.0.1.tar", last modified: Sun May 19 19:31:57 2024, max compression
+gzip compressed data, was "netbox_interface_synchronization-4.0.3.tar", last modified: Fri May 24 03:54:51 2024, max compression
```

## Comparing `netbox_interface_synchronization-4.0.1.tar` & `netbox_interface_synchronization-4.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2024-05-19 19:31:57.647681 netbox_interface_synchronization-4.0.1/
--rw-r--r--   0 keith     (1000) keith     (1000)    35803 2024-05-19 09:59:29.000000 netbox_interface_synchronization-4.0.1/LICENSE
--rw-r--r--   0 keith     (1000) keith     (1000)     1999 2024-05-19 19:31:57.647681 netbox_interface_synchronization-4.0.1/PKG-INFO
--rw-r--r--   0 keith     (1000) keith     (1000)     1350 2024-05-19 10:03:46.000000 netbox_interface_synchronization-4.0.1/README.md
--rw-r--r--   0 keith     (1000) keith     (1000)      817 2024-05-19 19:26:49.000000 netbox_interface_synchronization-4.0.1/pyproject.toml
--rw-rw-r--   0 keith     (1000) keith     (1000)       38 2024-05-19 19:31:57.647681 netbox_interface_synchronization-4.0.1/setup.cfg
-drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2024-05-19 19:31:57.643681 netbox_interface_synchronization-4.0.1/src/
-drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2024-05-19 19:31:57.647681 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization/
--rw-rw-r--   0 keith     (1000) keith     (1000)      473 2024-05-19 18:15:00.000000 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization/__init__.py
--rw-rw-r--   0 keith     (1000) keith     (1000)      191 2024-05-19 09:37:36.000000 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization/forms.py
--rw-rw-r--   0 keith     (1000) keith     (1000)     1188 2024-05-19 09:37:36.000000 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization/template_content.py
-drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2024-05-19 19:31:57.643681 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization/templates/
-drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2024-05-19 19:31:57.647681 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization/templates/netbox_interface_synchronization/
--rw-rw-r--   0 keith     (1000) keith     (1000)      203 2024-05-19 09:39:15.000000 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization/templates/netbox_interface_synchronization/compare_interfaces_button.html
--rw-rw-r--   0 keith     (1000) keith     (1000)     5394 2024-05-19 18:45:47.000000 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization/templates/netbox_interface_synchronization/interface_comparison.html
--rw-rw-r--   0 keith     (1000) keith     (1000)      394 2024-05-19 18:15:00.000000 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization/templates/netbox_interface_synchronization/number_of_interfaces_panel.html
--rw-rw-r--   0 keith     (1000) keith     (1000)      341 2024-05-19 09:37:36.000000 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization/urls.py
--rw-rw-r--   0 keith     (1000) keith     (1000)      991 2024-05-19 09:37:36.000000 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization/utils.py
--rw-rw-r--   0 keith     (1000) keith     (1000)     5916 2024-05-19 09:38:23.000000 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization/views.py
-drwxrwxr-x   0 keith     (1000) keith     (1000)        0 2024-05-19 19:31:57.647681 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization.egg-info/
--rw-r--r--   0 keith     (1000) keith     (1000)     1999 2024-05-19 19:31:57.000000 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization.egg-info/PKG-INFO
--rw-rw-r--   0 keith     (1000) keith     (1000)      890 2024-05-19 19:31:57.000000 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization.egg-info/SOURCES.txt
--rw-rw-r--   0 keith     (1000) keith     (1000)        1 2024-05-19 19:31:57.000000 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization.egg-info/dependency_links.txt
--rw-rw-r--   0 keith     (1000) keith     (1000)       38 2024-05-19 19:31:57.000000 netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:54:51.468502 netbox_interface_synchronization-4.0.3/
+-rw-r--r--   0 root         (0) root         (0)    35803 2024-05-19 09:59:29.000000 netbox_interface_synchronization-4.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2052 2024-05-24 03:54:51.468502 netbox_interface_synchronization-4.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1388 2024-05-24 03:10:14.000000 netbox_interface_synchronization-4.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      832 2024-05-24 03:52:36.000000 netbox_interface_synchronization-4.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 03:54:51.468502 netbox_interface_synchronization-4.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:54:51.464502 netbox_interface_synchronization-4.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:54:51.464502 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization/
+-rw-rw-r--   0 root         (0) root         (0)      463 2024-05-24 03:53:31.000000 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      191 2024-05-19 09:37:36.000000 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization/forms.py
+-rw-rw-r--   0 root         (0) root         (0)     1188 2024-05-19 09:37:36.000000 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization/template_content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:54:51.464502 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:54:51.468502 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization/templates/netbox_interface_synchronization/
+-rw-rw-r--   0 root         (0) root         (0)      203 2024-05-19 09:39:15.000000 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization/templates/netbox_interface_synchronization/compare_interfaces_button.html
+-rw-rw-r--   0 root         (0) root         (0)     5422 2024-05-23 05:03:41.000000 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization/templates/netbox_interface_synchronization/interface_comparison.html
+-rw-rw-r--   0 root         (0) root         (0)      394 2024-05-19 18:15:00.000000 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization/templates/netbox_interface_synchronization/number_of_interfaces_panel.html
+-rw-rw-r--   0 root         (0) root         (0)      341 2024-05-19 09:37:36.000000 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization/urls.py
+-rw-rw-r--   0 root         (0) root         (0)     1020 2024-05-24 02:55:26.000000 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     5985 2024-05-24 02:55:39.000000 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:54:51.468502 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2052 2024-05-24 03:54:51.000000 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      890 2024-05-24 03:54:51.000000 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-05-24 03:54:51.000000 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       38 2024-05-24 03:54:51.000000 netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization.egg-info/top_level.txt
```

### Comparing `netbox_interface_synchronization-4.0.1/LICENSE` & `netbox_interface_synchronization-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_interface_synchronization-4.0.1/PKG-INFO` & `netbox_interface_synchronization-4.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: netbox_interface_synchronization
-Version: 4.0.1
-Summary: Syncing Device Interfaces with the Interfaces from Device Type for NetBox
+Version: 4.0.3
+Summary: Syncing existing interfaces with the interfaces from a device type template in NetBox 4+
 Author-email: Keith Knowles <mkknowles@outlook.com>
 Project-URL: Homepage, https://github.com/NetTech2001/netbox-interface-synchronization
 Project-URL: Issues, https://github.com/NetTech2001/netbox-interface-synchronization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # netbox-interface-synchronization
 ## Overview
-This plugin allows you to compare and synchronize interfaces between devices and device types in NetBox . It can be useful for finding and correcting inconsistencies between interfaces.
+This plugin allows you to compare and synchronize interface names and types between devices and device types in NetBox. It can be useful for finding and correcting inconsistencies between interfaces when changing the device type.
 ## Compatibility
-Tested with NetBox versions 4.0.0, 4.0.1, 4.0.2.  This plugin is not compatible with Netbox 2 or 3
+Tested with NetBox versions 4.0.0 - 4.0.3.  This plugin is not compatible with Netbox 2 or 3
 ## Installation
 If your NetBox 4 installation uses virtualenv, activate it like this:
 ```
 source /opt/netbox/venv/bin/activate
 ```
 Install the plugin from PyPI:
 ```
```

### Comparing `netbox_interface_synchronization-4.0.1/README.md` & `netbox_interface_synchronization-4.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # netbox-interface-synchronization
 ## Overview
-This plugin allows you to compare and synchronize interfaces between devices and device types in NetBox . It can be useful for finding and correcting inconsistencies between interfaces.
+This plugin allows you to compare and synchronize interface names and types between devices and device types in NetBox. It can be useful for finding and correcting inconsistencies between interfaces when changing the device type.
 ## Compatibility
-Tested with NetBox versions 4.0.0, 4.0.1, 4.0.2.  This plugin is not compatible with Netbox 2 or 3
+Tested with NetBox versions 4.0.0 - 4.0.3.  This plugin is not compatible with Netbox 2 or 3
 ## Installation
 If your NetBox 4 installation uses virtualenv, activate it like this:
 ```
 source /opt/netbox/venv/bin/activate
 ```
 Install the plugin from PyPI:
 ```
```

### Comparing `netbox_interface_synchronization-4.0.1/pyproject.toml` & `netbox_interface_synchronization-4.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox_interface_synchronization"
-version = "4.0.1"
+version = "4.0.3"
 authors = [
   { name="Keith Knowles", email="mkknowles@outlook.com" },
 ]
-description = "Syncing Device Interfaces with the Interfaces from Device Type for NetBox"
+description = "Syncing existing interfaces with the interfaces from a device type template in NetBox 4+"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization/template_content.py` & `netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization/templates/netbox_interface_synchronization/interface_comparison.html` & `netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization/templates/netbox_interface_synchronization/interface_comparison.html`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     document.getElementById(src.name).checked = false;
   }
 }
 </script>
 
 <p>
 {% if templates_count == interfaces_count %}
-    The Device Type and Device have the same Interfaces.
+    The Device Type and Device have the same number of Interfaces.
 {% else %}
-    The Device Type and Device have different Interfaces.<br>
+    The Device Type and Device have a different number of Interfaces.<br>
     Device Type: {{ templates_count }}<br>
     Device: {{ interfaces_count }}
 {% endif %}
 </p>
 
 <form method="post">
     <!-- Interface templates -->
@@ -150,12 +150,12 @@
             <td>&nbsp;</td>
             <td>&nbsp;</td>
         </tr>
         {% endif %}
         {% endfor %}
     </table>
     <div class="text-right">
-        <input type="submit" value="Apply" class="btn btn-primary">
+        <input type="submit" value="Apply Changes" class="btn btn-green">
     </div>
 </form>
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
 {% extends 'base/layout.html' %} {% block title %}{{ device }} - Interface
 comparison{% endblock %} {% block header %}
    1. _D_e_v_i_c_e
    2. _{_{_ _d_e_v_i_c_e_._s_i_t_e_ _}_}
    3. _{_{_ _d_e_v_i_c_e_ _}_}
 {{ block.super }} {% endblock %} {% block content %}
 {% if templates_count == interfaces_count %} The Device Type and Device have
-the same Interfaces. {% else %} The Device Type and Device have different
-Interfaces.
+the same number of Interfaces. {% else %} The Device Type and Device have a
+different number of Interfaces.
 Device Type: {{ templates_count }}
 Device: {{ interfaces_count }} {% endif %}
 {% csrf_token %}
 DDeevviiccee TTyyppee AAccttiioonnss
 NNaammee TTyyppee   ???AAdddd
              
 DDeevviiccee    AAccttiioonnss
 NNaammee TTyyppee ???RReemmoovvee ???FFiixx NNaammee
                    
-[Apply]
+[Apply Changes]
 {% endblock %}
```

### Comparing `netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization/utils.py` & `netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 @dataclass(frozen=True)
 class UnifiedInterface:
     """A unified way to represent the interface and interface template"""
     id: int
     name: str
     type: str
     type_display: str
+    mgmt_only: bool = False
     is_template: bool = False
 
     def __eq__(self, other):
         # Ignore some fields when comparing; ignore interface name case and whitespaces
         return (self.name.lower().replace(' ', '') == other.name.lower().replace(' ', '')) and (self.type == other.type)
 
     def __hash__(self):
```

### Comparing `netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization/views.py` & `netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         interfaces = device.vc_interfaces()
         if config["exclude_virtual_interfaces"]:
             interfaces = list(filter(lambda i: not i.is_virtual, interfaces))
         interface_templates = InterfaceTemplate.objects.filter(device_type=device.device_type)
 
         unified_interfaces = [UnifiedInterface(i.id, i.name, i.type, i.get_type_display()) for i in interfaces]
         unified_interface_templates = [
-            UnifiedInterface(i.id, i.name, i.type, i.get_type_display(), is_template=True) for i in interface_templates]
+            UnifiedInterface(i.id, i.name, i.type, i.get_type_display(), i.mgmt_only, is_template=True) for i in interface_templates]
 
         # List of interfaces and interface templates presented in the unified format
         overall_interfaces = list(set(unified_interface_templates + unified_interfaces))
         overall_interfaces.sort(key=lambda o: natural_keys(o.name))
 
         comparison_templates = []
         comparison_interfaces = []
@@ -75,27 +75,27 @@
 
             # Remove selected interfaces from the device and count them
             interfaces_deleted = Interface.objects.filter(id__in=remove_from_device).delete()[0]
 
             # Add selected interfaces to the device and count them
             add_to_device_interfaces = InterfaceTemplate.objects.filter(id__in=add_to_device)
             interfaces_created = len(Interface.objects.bulk_create([
-                Interface(device=device, name=i.name, type=i.type) for i in add_to_device_interfaces
+                Interface(device=device, name=i.name, type=i.type, mgmt_only=i.mgmt_only) for i in add_to_device_interfaces
             ]))
 
             # Getting and validating a list of interfaces to rename
             fix_name_interfaces = filter(lambda i: str(i.id) in request.POST.getlist("fix_name"), interfaces)
             # Casting interface templates into UnifiedInterface objects for proper comparison with interfaces for renaming
             unified_interface_templates = [
-                UnifiedInterface(i.id, i.name, i.type, i.get_type_display()) for i in interface_templates]
+                UnifiedInterface(i.id, i.name, i.type,i.mgmt_only, i.get_type_display()) for i in interface_templates]
 
             # Rename selected interfaces
             interfaces_fixed = 0
             for interface in fix_name_interfaces:
-                unified_interface = UnifiedInterface(interface.id, interface.name, interface.type, interface.get_type_display())
+                unified_interface = UnifiedInterface(interface.id, interface.name, interface.type, interface.mgmt_only, interface.get_type_display())
                 try:
                     # Try to extract an interface template with the corresponding name
                     corresponding_template = unified_interface_templates[unified_interface_templates.index(unified_interface)]
                     interface.name = corresponding_template.name
                     interface.save()
                     interfaces_fixed += 1
                 except ValueError:
```

### Comparing `netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization.egg-info/PKG-INFO` & `netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: netbox_interface_synchronization
-Version: 4.0.1
-Summary: Syncing Device Interfaces with the Interfaces from Device Type for NetBox
+Version: 4.0.3
+Summary: Syncing existing interfaces with the interfaces from a device type template in NetBox 4+
 Author-email: Keith Knowles <mkknowles@outlook.com>
 Project-URL: Homepage, https://github.com/NetTech2001/netbox-interface-synchronization
 Project-URL: Issues, https://github.com/NetTech2001/netbox-interface-synchronization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # netbox-interface-synchronization
 ## Overview
-This plugin allows you to compare and synchronize interfaces between devices and device types in NetBox . It can be useful for finding and correcting inconsistencies between interfaces.
+This plugin allows you to compare and synchronize interface names and types between devices and device types in NetBox. It can be useful for finding and correcting inconsistencies between interfaces when changing the device type.
 ## Compatibility
-Tested with NetBox versions 4.0.0, 4.0.1, 4.0.2.  This plugin is not compatible with Netbox 2 or 3
+Tested with NetBox versions 4.0.0 - 4.0.3.  This plugin is not compatible with Netbox 2 or 3
 ## Installation
 If your NetBox 4 installation uses virtualenv, activate it like this:
 ```
 source /opt/netbox/venv/bin/activate
 ```
 Install the plugin from PyPI:
 ```
```

### Comparing `netbox_interface_synchronization-4.0.1/src/netbox_interface_synchronization.egg-info/SOURCES.txt` & `netbox_interface_synchronization-4.0.3/src/netbox_interface_synchronization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

