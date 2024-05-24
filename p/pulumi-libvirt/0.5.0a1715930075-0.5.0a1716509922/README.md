# Comparing `tmp/pulumi_libvirt-0.5.0a1715930075.tar.gz` & `tmp/pulumi_libvirt-0.5.0a1716509922.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_libvirt-0.5.0a1715930075.tar", last modified: Fri May 17 07:18:29 2024, max compression
+gzip compressed data, was "pulumi_libvirt-0.5.0a1716509922.tar", last modified: Fri May 24 00:26:34 2024, max compression
```

## Comparing `pulumi_libvirt-0.5.0a1715930075.tar` & `pulumi_libvirt-0.5.0a1716509922.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:18:29.921335 pulumi_libvirt-0.5.0a1715930075/
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-17 07:18:29.921335 pulumi_libvirt-0.5.0a1715930075/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:18:29.921335 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42947 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/cloud_init_disk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:18:29.921335 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    70503 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/get_network_dns_host_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/get_network_dns_srv_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/get_network_dnsmasq_options_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/ignition.py
--rw-r--r--   0 runner    (1001) docker     (127)    40872 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    36652 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    28830 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:18:29.921335 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-17 07:18:29.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-17 07:18:29.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 07:18:29.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 07:18:29.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 07:18:29.000000 pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-17 07:18:23.000000 pulumi_libvirt-0.5.0a1715930075/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 07:18:29.921335 pulumi_libvirt-0.5.0a1715930075/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:26:34.692214 pulumi_libvirt-0.5.0a1716509922/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-24 00:26:34.692214 pulumi_libvirt-0.5.0a1716509922/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:26:34.692214 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44081 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/cloud_init_disk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:26:34.692214 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70503 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/get_network_dns_host_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/get_network_dns_srv_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/get_network_dnsmasq_options_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/ignition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40872 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37730 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    28830 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:26:34.692214 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-24 00:26:34.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-24 00:26:34.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 00:26:34.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 00:26:34.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-24 00:26:34.000000 pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-24 00:26:28.000000 pulumi_libvirt-0.5.0a1716509922/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 00:26:34.692214 pulumi_libvirt-0.5.0a1716509922/setup.cfg
```

### Comparing `pulumi_libvirt-0.5.0a1715930075/PKG-INFO` & `pulumi_libvirt-0.5.0a1716509922/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_libvirt
-Version: 0.5.0a1715930075
+Version: 0.5.0a1716509922
 Summary: A Pulumi package for creating and managing libvirt cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-libvirt
 Keywords: pulumi,libvirt
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_libvirt-0.5.0a1715930075/README.md` & `pulumi_libvirt-0.5.0a1716509922/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/__init__.py` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/_inputs.py` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,51 +375,79 @@
 @pulumi.input_type
 class DomainFilesystemArgs:
     def __init__(__self__, *,
                  source: pulumi.Input[str],
                  target: pulumi.Input[str],
                  accessmode: Optional[pulumi.Input[str]] = None,
                  readonly: Optional[pulumi.Input[bool]] = None):
+        """
+        :param pulumi.Input[str] source: the directory of the host to be shared with the guest.
+        :param pulumi.Input[str] target: an arbitrary string tag that is exported to the guest as a hint for
+               where to mount the source.
+        :param pulumi.Input[str] accessmode: specifies the security mode for accessing the source. By default
+               the `mapped` mode is chosen.
+        :param pulumi.Input[bool] readonly: enables exporting filesystem as a readonly mount for guest, by
+               default read-only access is given.
+               
+               Example:
+        """
         pulumi.set(__self__, "source", source)
         pulumi.set(__self__, "target", target)
         if accessmode is not None:
             pulumi.set(__self__, "accessmode", accessmode)
         if readonly is not None:
             pulumi.set(__self__, "readonly", readonly)
 
     @property
     @pulumi.getter
     def source(self) -> pulumi.Input[str]:
+        """
+        the directory of the host to be shared with the guest.
+        """
         return pulumi.get(self, "source")
 
     @source.setter
     def source(self, value: pulumi.Input[str]):
         pulumi.set(self, "source", value)
 
     @property
     @pulumi.getter
     def target(self) -> pulumi.Input[str]:
+        """
+        an arbitrary string tag that is exported to the guest as a hint for
+        where to mount the source.
+        """
         return pulumi.get(self, "target")
 
     @target.setter
     def target(self, value: pulumi.Input[str]):
         pulumi.set(self, "target", value)
 
     @property
     @pulumi.getter
     def accessmode(self) -> Optional[pulumi.Input[str]]:
+        """
+        specifies the security mode for accessing the source. By default
+        the `mapped` mode is chosen.
+        """
         return pulumi.get(self, "accessmode")
 
     @accessmode.setter
     def accessmode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "accessmode", value)
 
     @property
     @pulumi.getter
     def readonly(self) -> Optional[pulumi.Input[bool]]:
+        """
+        enables exporting filesystem as a readonly mount for guest, by
+        default read-only access is given.
+
+        Example:
+        """
         return pulumi.get(self, "readonly")
 
     @readonly.setter
     def readonly(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "readonly", value)
```

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/_utilities.py` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/cloud_init_disk.py` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/cloud_init_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/config/vars.py` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/domain.py` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/get_network_dns_host_template.py` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/get_network_dns_host_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/get_network_dns_srv_template.py` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/get_network_dns_srv_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/get_network_dnsmasq_options_template.py` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/get_network_dnsmasq_options_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/ignition.py` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/ignition.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/network.py` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/outputs.py` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,39 +364,67 @@
 @pulumi.output_type
 class DomainFilesystem(dict):
     def __init__(__self__, *,
                  source: str,
                  target: str,
                  accessmode: Optional[str] = None,
                  readonly: Optional[bool] = None):
+        """
+        :param str source: the directory of the host to be shared with the guest.
+        :param str target: an arbitrary string tag that is exported to the guest as a hint for
+               where to mount the source.
+        :param str accessmode: specifies the security mode for accessing the source. By default
+               the `mapped` mode is chosen.
+        :param bool readonly: enables exporting filesystem as a readonly mount for guest, by
+               default read-only access is given.
+               
+               Example:
+        """
         pulumi.set(__self__, "source", source)
         pulumi.set(__self__, "target", target)
         if accessmode is not None:
             pulumi.set(__self__, "accessmode", accessmode)
         if readonly is not None:
             pulumi.set(__self__, "readonly", readonly)
 
     @property
     @pulumi.getter
     def source(self) -> str:
+        """
+        the directory of the host to be shared with the guest.
+        """
         return pulumi.get(self, "source")
 
     @property
     @pulumi.getter
     def target(self) -> str:
+        """
+        an arbitrary string tag that is exported to the guest as a hint for
+        where to mount the source.
+        """
         return pulumi.get(self, "target")
 
     @property
     @pulumi.getter
     def accessmode(self) -> Optional[str]:
+        """
+        specifies the security mode for accessing the source. By default
+        the `mapped` mode is chosen.
+        """
         return pulumi.get(self, "accessmode")
 
     @property
     @pulumi.getter
     def readonly(self) -> Optional[bool]:
+        """
+        enables exporting filesystem as a readonly mount for guest, by
+        default read-only access is given.
+
+        Example:
+        """
         return pulumi.get(self, "readonly")
 
 
 @pulumi.output_type
 class DomainGraphics(dict):
     @staticmethod
     def __key_warning(key: str):
```

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/pool.py` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/provider.py` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt/volume.py` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt.egg-info/PKG-INFO` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_libvirt
-Version: 0.5.0a1715930075
+Version: 0.5.0a1716509922
 Summary: A Pulumi package for creating and managing libvirt cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-libvirt
 Keywords: pulumi,libvirt
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_libvirt-0.5.0a1715930075/pulumi_libvirt.egg-info/SOURCES.txt` & `pulumi_libvirt-0.5.0a1716509922/pulumi_libvirt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715930075/pyproject.toml` & `pulumi_libvirt-0.5.0a1716509922/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_libvirt"
   description = "A Pulumi package for creating and managing libvirt cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "libvirt"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.5.0a1715930075"
+  version = "0.5.0a1716509922"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-libvirt"
 
 [build-system]
```

