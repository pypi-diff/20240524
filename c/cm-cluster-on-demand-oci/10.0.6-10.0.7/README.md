# Comparing `tmp/cm-cluster-on-demand-oci-10.0.6.tar.gz` & `tmp/cm-cluster-on-demand-oci-10.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cm-cluster-on-demand-oci-10.0.6.tar", last modified: Thu Mar 28 15:00:03 2024, max compression
+gzip compressed data, was "cm-cluster-on-demand-oci-10.0.7.tar", last modified: Fri May 24 18:43:15 2024, max compression
```

## Comparing `cm-cluster-on-demand-oci-10.0.6.tar` & `cm-cluster-on-demand-oci-10.0.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:00:03.613506 cm-cluster-on-demand-oci-10.0.6/
--rw-r--r--   0 root         (0) root         (0)    11358 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      133 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1751 2024-03-28 15:00:03.613506 cm-cluster-on-demand-oci-10.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      833 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:00:03.613506 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/
--rw-r--r--   0 root         (0) root         (0)      596 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/__init__.py
--rw-r--r--   0 root         (0) root         (0)      413 2024-03-28 15:00:02.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/_version.py
--rw-r--r--   0 root         (0) root         (0)    12654 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/base.py
--rw-r--r--   0 root         (0) root         (0)     5491 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/brightsetup.py
--rw-r--r--   0 root         (0) root         (0)     3414 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/cli.py
--rw-r--r--   0 root         (0) root         (0)     4210 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/client.py
--rw-r--r--   0 root         (0) root         (0)     2927 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/client_base.py
--rw-r--r--   0 root         (0) root         (0)     7555 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/cluster.py
--rw-r--r--   0 root         (0) root         (0)    38913 2024-03-28 14:59:47.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/clustercreate.py
--rw-r--r--   0 root         (0) root         (0)    27231 2024-03-28 14:59:47.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/clusterdelete.py
--rw-r--r--   0 root         (0) root         (0)     9702 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/clusterlist.py
--rw-r--r--   0 root         (0) root         (0)     3876 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/clusterstart.py
--rw-r--r--   0 root         (0) root         (0)     7634 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/clusterstop.py
--rw-r--r--   0 root         (0) root         (0)     4284 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/configuration.py
--rw-r--r--   0 root         (0) root         (0)      738 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/const.py
--rw-r--r--   0 root         (0) root         (0)     2552 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/imagelist.py
--rw-r--r--   0 root         (0) root         (0)    12583 2024-03-28 14:59:47.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/images.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:00:03.613506 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/
--rw-r--r--   0 root         (0) root         (0)      596 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5106 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/blockstorage.py
--rw-r--r--   0 root         (0) root         (0)    14544 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/compute.py
--rw-r--r--   0 root         (0) root         (0)     2969 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/filestorage.py
--rw-r--r--   0 root         (0) root         (0)     5319 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/identity.py
--rw-r--r--   0 root         (0) root         (0)     3068 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/marketplace.py
--rw-r--r--   0 root         (0) root         (0)     3228 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/search.py
--rw-r--r--   0 root         (0) root         (0)    13220 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/virtual_network.py
--rw-r--r--   0 root         (0) root         (0)     4416 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/workrequest.py
--rw-r--r--   0 root         (0) root         (0)     3463 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/summary.py
--rw-r--r--   0 root         (0) root         (0)     6223 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:00:03.613506 cm-cluster-on-demand-oci-10.0.6/cm_cluster_on_demand_oci.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1751 2024-03-28 15:00:03.000000 cm-cluster-on-demand-oci-10.0.6/cm_cluster_on_demand_oci.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1358 2024-03-28 15:00:03.000000 cm-cluster-on-demand-oci-10.0.6/cm_cluster_on_demand_oci.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 15:00:03.000000 cm-cluster-on-demand-oci-10.0.6/cm_cluster_on_demand_oci.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-03-28 15:00:03.000000 cm-cluster-on-demand-oci-10.0.6/cm_cluster_on_demand_oci.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      100 2024-03-28 15:00:03.000000 cm-cluster-on-demand-oci-10.0.6/cm_cluster_on_demand_oci.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-03-28 15:00:03.000000 cm-cluster-on-demand-oci-10.0.6/cm_cluster_on_demand_oci.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       34 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/external_requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-28 15:00:03.613506 cm-cluster-on-demand-oci-10.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2498 2024-03-28 14:59:26.000000 cm-cluster-on-demand-oci-10.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 18:43:15.709066 cm-cluster-on-demand-oci-10.0.7/
+-rw-r--r--   0 root         (0) root         (0)    11358 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      133 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-05-24 18:43:15.709066 cm-cluster-on-demand-oci-10.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      833 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 18:43:15.709066 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/
+-rw-r--r--   0 root         (0) root         (0)      596 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      413 2024-05-24 18:43:14.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/_version.py
+-rw-r--r--   0 root         (0) root         (0)    15091 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/base.py
+-rw-r--r--   0 root         (0) root         (0)     5491 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/brightsetup.py
+-rw-r--r--   0 root         (0) root         (0)     3414 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/cli.py
+-rw-r--r--   0 root         (0) root         (0)     4210 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/client.py
+-rw-r--r--   0 root         (0) root         (0)     2927 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/client_base.py
+-rw-r--r--   0 root         (0) root         (0)     7555 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/cluster.py
+-rw-r--r--   0 root         (0) root         (0)    39611 2024-05-24 18:42:53.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/clustercreate.py
+-rw-r--r--   0 root         (0) root         (0)    27841 2024-05-24 18:42:53.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/clusterdelete.py
+-rw-r--r--   0 root         (0) root         (0)     9702 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/clusterlist.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/clusterstart.py
+-rw-r--r--   0 root         (0) root         (0)     7634 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/clusterstop.py
+-rw-r--r--   0 root         (0) root         (0)     4284 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/configuration.py
+-rw-r--r--   0 root         (0) root         (0)      738 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/const.py
+-rw-r--r--   0 root         (0) root         (0)     2552 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/imagelist.py
+-rw-r--r--   0 root         (0) root         (0)    12583 2024-05-24 18:42:53.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/images.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 18:43:15.709066 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/
+-rw-r--r--   0 root         (0) root         (0)      596 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5106 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/blockstorage.py
+-rw-r--r--   0 root         (0) root         (0)    14544 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/compute.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/filestorage.py
+-rw-r--r--   0 root         (0) root         (0)     6607 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/identity.py
+-rw-r--r--   0 root         (0) root         (0)     3068 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/marketplace.py
+-rw-r--r--   0 root         (0) root         (0)     3228 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/search.py
+-rw-r--r--   0 root         (0) root         (0)    13220 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/virtual_network.py
+-rw-r--r--   0 root         (0) root         (0)     4416 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/workrequest.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/summary.py
+-rw-r--r--   0 root         (0) root         (0)     6808 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 18:43:15.709066 cm-cluster-on-demand-oci-10.0.7/cm_cluster_on_demand_oci.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-05-24 18:43:15.000000 cm-cluster-on-demand-oci-10.0.7/cm_cluster_on_demand_oci.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-05-24 18:43:15.000000 cm-cluster-on-demand-oci-10.0.7/cm_cluster_on_demand_oci.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 18:43:15.000000 cm-cluster-on-demand-oci-10.0.7/cm_cluster_on_demand_oci.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-24 18:43:15.000000 cm-cluster-on-demand-oci-10.0.7/cm_cluster_on_demand_oci.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-24 18:43:15.000000 cm-cluster-on-demand-oci-10.0.7/cm_cluster_on_demand_oci.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-24 18:43:15.000000 cm-cluster-on-demand-oci-10.0.7/cm_cluster_on_demand_oci.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/external_requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 18:43:15.709066 cm-cluster-on-demand-oci-10.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-05-24 18:42:30.000000 cm-cluster-on-demand-oci-10.0.7/setup.py
```

### Comparing `cm-cluster-on-demand-oci-10.0.6/LICENSE` & `cm-cluster-on-demand-oci-10.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/PKG-INFO` & `cm-cluster-on-demand-oci-10.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm-cluster-on-demand-oci
-Version: 10.0.6
+Version: 10.0.7
 Summary: Bright Cluster on Demand Utility OCI
 Home-page: https://www.brightcomputing.com/
 Author: Cloudteam
 Author-email: cloudteam@brightcomputing.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cm-cluster-on-demand-oci-10.0.6/README.md` & `cm-cluster-on-demand-oci-10.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/__init__.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/__init__.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/base.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from __future__ import annotations
 
 import logging
+from collections import defaultdict
 from collections.abc import Collection
 from datetime import datetime
 from functools import cached_property, lru_cache
 
 import netaddr
 from oci import wait_until
 from oci.core.models import CreatePublicIpDetails, Instance, PrivateIp, PublicIp, Subnet, Vcn
@@ -74,14 +75,54 @@
     def _validate_availability_domain(self):
         if all(domain.name != self.availability_domain_name for domain in self.availability_domains):
             raise UserReportableException(
                 f"Availability domain {self.availability_domain_name} is not valid"
                 " for the provided compartment, please provide an availability domain"
                 " or skip parameter to use a random availability domain")
 
+    def _validate_defined_tags(self):
+        if not config.get("head_node_defined_tags"):
+            return
+
+        try:
+            # OCI allows compartments to nest up to six levels. Resources can have defined tags from their own, parent,
+            # or peer compartments. This code fetches tag namespaces from all compartments under the root
+            # (tenant ID matches root compartment ID).
+            available_namespaces = {
+                namespace.name: namespace.id for namespace in self.client.identity.list_tag_namespaces(
+                    compartment_id=config["oci_tenancy"], include_subcompartments=True)
+            }
+
+            # Validate each tag namespace and defined tag provided by the user
+            for namespace, tag_key, tag_value in config["head_node_defined_tags"]:
+                if namespace not in available_namespaces:
+                    available_namespaces = ', '.join(available_namespaces.keys())
+                    raise UserReportableException(f"Provided tag namespace '{namespace}' not found. "
+                                                  f"Available tag namespaces are: {available_namespaces}")
+
+                # Fetch tags for the requested namespaces only
+                available_tag_keys = {
+                    tag.name for tag in self.client.identity.list_tags(
+                        tag_namespace_id=available_namespaces[namespace]
+                    )
+                }
+
+                if tag_key not in available_tag_keys:
+                    raise UserReportableException(
+                        f"Provided tag '{tag_key}' from '{namespace}' namespace not found. "
+                        f"Available tags in '{namespace}' namespace are: {', '.join(available_tag_keys)}"
+                    )
+
+        except ServiceError as se:
+            raise UserReportableException(f"OCI Service error: {se.message}")
+        except UserReportableException as ure:
+            raise ure
+        except Exception as e:
+            raise UserReportableException(f"Unexpected error: {str(e)}")
+
     def _generate_freeform_tags_for(self, object_type: str, cluster_name=None) -> dict[str, str]:
         if not cluster_name:
             cluster_name = config["name"]
         cur_time_str = datetime.utcnow().isoformat(timespec="milliseconds") + "Z"  # same as oci portal
         self._default_freeform_tags = {
             "BCM_Type": None,
             "BCM_Resource": "True",
@@ -103,14 +144,25 @@
             "Shared Public IP",
         ]
         if object_type not in valid_object_types:
             raise CODException(f"Unsupported object type '{object_type}'")
 
         return {**self._default_freeform_tags, "BCM_Type": object_type}
 
+    @classmethod
+    def _generate_defined_tags(cls):
+        if not config["head_node_defined_tags"]:
+            return {}
+
+        merged_dict = defaultdict(dict)
+        for namespace, tag_key, tag_value in config["head_node_defined_tags"]:
+            merged_dict[namespace].update({tag_key: tag_value})
+
+        return merged_dict
+
     def _validate_shape(self):
         # Wrong shape raises UserReportableException from get_shape()
         head_shape = self.client.compute.get_shape(config["head_node_shape"],
                                                    self.availability_domain_name, self.compute_cid)
         node_shape = self.client.compute.get_shape(config["node_shape"],
                                                    self.availability_domain_name, self.compute_cid)
         if config["node_use_cluster_network"] and not node_shape.rdma_ports:
```

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/brightsetup.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/brightsetup.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/cli.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/cli.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/client.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/client.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/client_base.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/client_base.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/cluster.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/cluster.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/clustercreate.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/clustercreate.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 from clusterondemandconfig.configuration_validation import requires_other_parameters_to_be_set
 from clusterondemandoci.base import ClusterCommand
 from clusterondemandoci.brightsetup import build_cloud_config, generate_bright_setup
 from clusterondemandoci.cluster import Cluster
 from clusterondemandoci.clusterdelete import ClusterDelete
 from clusterondemandoci.const import CLUSTER_NAME_TAG, IMAGE_CREATED_TIME_TAG, IMAGE_NAME_TAG
 from clusterondemandoci.summary import OCISummaryGenerator
-from clusterondemandoci.utils import get_head_node_list, get_oci_key_content
+from clusterondemandoci.utils import get_head_node_list, get_oci_key_content, parse_defined_tags
 
 from .configuration import ociclustercommon_ns, ocicommon_ns
 from .images import CommunityAppImage, OCIImageSource, findimages_ns, make_cod_image_from_ocid
 
 log = logging.getLogger("cluster-on-demand")
 
 config_ns = ConfigNamespace("oci.cluster.create", "cluster creation parameters")
@@ -293,21 +293,32 @@
     help="Number of Volume Peformance Units (VPUs) per GB to apply to the head node's boot volume.",
     help_varname="HEADNODE_ROOT_VOLUME_VPUS",
     validation=[number_must_be_between(10, 120), must_be_multiple_of(10)],
     advanced=True,
     type=int
 )
 headnodecreate_ns.add_enumeration_parameter(
-    "head_node_tags",
+    "head_node_freeform_tags",
     default=[],
     help=("List of tags to be added to the head node "
           "(e.g. --head-node-tags tag1=value tag2=value)"),
     parser=utils.parse_assignment,
     serializer=lambda val: "{}={}".format(*val)
 )
+headnodecreate_ns.add_enumeration_parameter(
+    "head_node_defined_tags",
+    help=(
+        "List of defined tags to be added to the head node. Defined tags in OCI exist under tag namespaces, so the "
+        "user should supply tag namespace name along with tag's key and value. "
+        "Defined tag format is: namespace.tag_key.tag_value. For example: "
+        "--head-node-defined-tags namespace1.key1.value namespace1.key2.value namespace2.key1.value"
+    ),
+    parser=parse_defined_tags,
+    advanced=True,
+)
 config_ns.import_namespace(headnodecreate_ns)
 
 
 def run_command():
     ClusterCreate().run()
 
 
@@ -319,14 +330,15 @@
 
     def _validate_params(self):
         self._validate_cluster_name()
         self._validate_access_credentials()
         self._validate_availability_domain()
         self._validate_shape()
         self._validate_head_node_ip()
+        self._validate_defined_tags()
 
     def _generate_cloud_config(self, subnet_id: str, private_subnet_id: str, node_nsg_id: str) -> str:
         node_instance_configuration_id = ""
         if config["instance_configuration_id"]:
             node_instance_configuration_id = config["instance_configuration_id"]
             log.info(f"Using supplied instance configuration ID '{node_instance_configuration_id}'")
 
@@ -607,18 +619,18 @@
         instance_metadata = {
             "user_data": cloud_init_script,
         }
 
         if config["ssh_pub_key_path"]:
             instance_metadata["ssh_authorized_keys"] = self._readfile(config["ssh_pub_key_path"])
 
-        head_node_tags = dict(config["head_node_tags"])
-        head_node_tags[IMAGE_NAME_TAG] = self.head_node_image.name
+        head_node_freeform_tags = dict(config["head_node_freeform_tags"])
+        head_node_freeform_tags[IMAGE_NAME_TAG] = self.head_node_image.name
         # timeformat same as oci portal, 2023-07-03T09:04:52.555Z (Z for UTC)
-        head_node_tags[IMAGE_CREATED_TIME_TAG] = \
+        head_node_freeform_tags[IMAGE_CREATED_TIME_TAG] = \
             self.head_node_image.created_at.isoformat(timespec="milliseconds") + "Z"
 
         instance_source_via_image_details = oci.core.models.InstanceSourceViaImageDetails(
             image_id=self.head_node_image_id,
             boot_volume_size_in_gbs=config["head_node_root_volume_size"],
             boot_volume_vpus_per_gb=config["head_node_root_volume_vpus"],
         )
@@ -638,15 +650,16 @@
             display_name=head_node_name,
             instance_options=instance_options,
             metadata=instance_metadata,
             shape=shape.shape,
             shape_config=shape_config,
             # extended_metadata=instance_extended_metadata,
             source_details=instance_source_via_image_details,
-            freeform_tags=head_node_tags | self._generate_freeform_tags_for("Head Node"),
+            defined_tags=ClusterCommand._generate_defined_tags(),
+            freeform_tags=head_node_freeform_tags | self._generate_freeform_tags_for("Head Node"),
         )
 
         launched_instance = self.client.compute.launch_instance(
             head_node_details
         )
         return launched_instance
```

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/clusterdelete.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/clusterdelete.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,15 +86,14 @@
             cluster_names = [c.cluster_name for c in clusters]
         else:
             log.error("Need to specify cluster name to be deleted")
             return
 
         if config["dry_run"]:
             log.info("--dry-run passed; no delete operations will be performed")
-            return
 
         tag_values = ", ".join(cluster_names)
         if not confirm(f"This will delete all OCI resources tagged as '{tag_values}'; continue?"):
             return
 
         log.debug("Cluster deletion starting")
         multithread_run(self.delete_cluster,
@@ -249,14 +248,17 @@
             log.info("Cluster %s: No cluster networks '%s=%s'; skipping", tag_value,
                      CLUSTER_NAME_TAG, tag_value)
             return
 
         num_cluster_networks_to_delete = len(cluster_network_summary_list)
         log.info("Cluster %s: Deleting %d cluster network(s)", tag_value, num_cluster_networks_to_delete)
 
+        if config["dry_run"]:
+            return
+
         for cluster_network_summary in cluster_network_summary_list:
             self.client.compute.delete_cluster_network(cluster_network_summary.identifier)
 
         cluster_network_delete_elapsed_time = time.time() - start_time
         log.info(
             "Cluster %s: Terminated %d cluster network(s) in %0.2f seconds",
             tag_value,
@@ -283,14 +285,17 @@
             log.info("Cluster %s: No instance pools found matching '%s=%s'; skipping", tag_value,
                      CLUSTER_NAME_TAG, tag_value)
             return
 
         num_instance_pools_to_delete = len(instance_pool_summary_list)
         log.info("Cluster %s: Deleting %d instance pool(s)", tag_value, num_instance_pools_to_delete)
 
+        if config["dry_run"]:
+            return
+
         for instance_pool_summary in instance_pool_summary_list:
             self.client.compute.delete_instance_pool(instance_pool_summary.identifier)
 
         instance_pool_delete_elapsed_time = time.time() - start_time
         log.info(
             "Cluster %s: Terminated %d instance pool(s) in %0.2f seconds",
             tag_value,
@@ -318,25 +323,29 @@
         if not instances_to_delete_summary_list:
             log.info("Cluster %s: No instances found matching '%s=%s'", tag_value, CLUSTER_NAME_TAG, tag_value)
             return
 
         if num_instances_to_terminate == 0:
             num_instances_to_terminate = len(instances_to_delete_summary_list)
 
-        #
-        # If there's only one instance, terminate it the easy way. This is sometimes faster than
-        # using bulk delete on a single node; reductions of up to 20 seconds were seen in testing.
-        if num_instances_to_terminate == 1:
-            instance_to_delete_summary = instances_to_delete_summary_list[0]
+        for instance_to_delete_summary in instances_to_delete_summary_list:
             log.info(
                 "Cluster %s: Terminating %s (instance state: %s)...",
                 tag_value,
                 instance_to_delete_summary.display_name,
                 instance_to_delete_summary.lifecycle_state,
             )
+
+        if config["dry_run"]:
+            return
+
+        #
+        # If there's only one instance, terminate it the easy way. This is sometimes faster than
+        # using bulk delete on a single node; reductions of up to 20 seconds were seen in testing.
+        if num_instances_to_terminate == 1:
             self.client.compute.terminate_instance(instance_to_delete_summary.identifier)
             instance_delete_elapsed_time = time.time() - start_time
             log.info(
                 "Cluster %s: Terminated 1 instance in %0.2f seconds",
                 tag_value,
                 instance_delete_elapsed_time
             )
@@ -379,15 +388,16 @@
 
         try:
             # Shared public IP is optional and will not exist unless cluster is HA. Hence, its absense is a valid case.
             shared_public_ip = next(
                 ip for ip in shared_public_ip_summary_list if ip.freeform_tags["BCM_Type"] == "Shared Public IP"
             )
             log.info(f"Cluster {tag_value}: Deleting shared public IP: {shared_public_ip.display_name}")
-            self.client.network.delete_public_ip(shared_public_ip.identifier)
+            if not config["dry_run"]:
+                self.client.network.delete_public_ip(shared_public_ip.identifier)
         except StopIteration:
             log.debug(f"no shared public IP found for the cluster {tag_value}")
 
     def delete_file_system(self, compartment_id: str, tag_value: str) -> None:
         where_clause = (
             f"compartmentId = '{compartment_id}'"
             f" && lifeCycleState != '{FileSystem.LIFECYCLE_STATE_DELETED}'"
@@ -406,15 +416,16 @@
                      tag_value,
                      CLUSTER_NAME_TAG,
                      tag_value)
             return
 
         for file_system_summary in file_system_summary_list:
             log.info(f"Cluster {tag_value}: Deleting File System {file_system_summary.display_name}")
-            self.client.file_storage.delete_file_system_and_wait_for_state(file_system_summary.identifier)
+            if not config["dry_run"]:
+                self.client.file_storage.delete_file_system_and_wait_for_state(file_system_summary.identifier)
 
     def delete_mount_target(self, compartment_id: str, tag_value: str) -> None:
         where_clause = (
             f"compartmentId = '{compartment_id}'"
             f" && lifeCycleState != '{MountTarget.LIFECYCLE_STATE_DELETED}'"
             f" && lifeCycleState != '{MountTarget.LIFECYCLE_STATE_DELETING}'"
         )
@@ -429,15 +440,16 @@
         if not mount_target_summary_list:
             log.info(f"Cluster {tag_value}: No Mount Targets found matching "
                      f"'{CLUSTER_NAME_TAG}={tag_value}'; skipping")
             return
 
         for mount_target_summary in mount_target_summary_list:
             log.info("Cluster %s: Deleting Mount Target %r", tag_value, mount_target_summary.display_name)
-            self.client.file_storage.delete_mount_target_and_wait_for_state(mount_target_summary.identifier)
+            if not config["dry_run"]:
+                self.client.file_storage.delete_mount_target_and_wait_for_state(mount_target_summary.identifier)
 
     def delete_volumes(self, compartment_id: str, tag_value: str) -> None:
         where_clause = (
             f"compartmentId = '{compartment_id}'"
             f" && lifeCycleState != '{Volume.LIFECYCLE_STATE_TERMINATED}'"
             f" && lifeCycleState != '{Volume.LIFECYCLE_STATE_TERMINATING}'"
         )
@@ -457,15 +469,16 @@
         num_volumes = len(volumes_summary_list)
         log.info("Cluster %s: Deleting %d volume(s)", tag_value, num_volumes)
 
         block_storage = self.client.block_storage
 
         for i, volumes_summary in enumerate(volumes_summary_list):
             log.info("Cluster %s: Deleting %d of %d", CLUSTER_NAME_TAG, i + 1, num_volumes)
-            block_storage.delete_volume(volumes_summary.identifier)
+            if not config["dry_run"]:
+                block_storage.delete_volume(volumes_summary.identifier)
 
         # FIXME: Optional, may be useful to be sure, all data was deleted.
         # for i, volumes_summary in enumerate(volumes_summary_list):
         #     log.info("Confirming deletion of %d of %d", i + 1, num_volumes)
         #     wait_until(
         #         block_storage,
         #         block_storage.get_volume(volumes_summary.identifier),
@@ -493,15 +506,16 @@
                 CLUSTER_NAME_TAG,
                 tag_value
             )
             return
 
         for subnet_resource_summary in subnet_resource_summary_list:
             log.info("Cluster %s: Deleting subnet %r", tag_value, subnet_resource_summary.display_name)
-            self.client.network.delete_subnet(subnet_resource_summary.identifier)
+            if not config["dry_run"]:
+                self.client.network.delete_subnet(subnet_resource_summary.identifier)
 
     def delete_internet_gateways(self, compartment_id: str, tag_value: str) -> None:
         where_clause = (
             f"compartmentId = '{compartment_id}'"
             f" && lifeCycleState != '{InternetGateway.LIFECYCLE_STATE_TERMINATED}'"
             f" && lifeCycleState != '{InternetGateway.LIFECYCLE_STATE_TERMINATING}'"
         )
@@ -519,15 +533,16 @@
                 CLUSTER_NAME_TAG,
                 tag_value
             )
             return
 
         for internet_gateway_summary in internet_gateway_summary_list:
             log.info("Cluster %s: Deleting internet gateway %r", tag_value, internet_gateway_summary.display_name)
-            self.client.network.delete_internet_gateway(internet_gateway_summary.identifier)
+            if not config["dry_run"]:
+                self.client.network.delete_internet_gateway(internet_gateway_summary.identifier)
 
     def delete_nat_gateways(self, compartment_id: str, tag_value: str) -> None:
         where_clause = (
             f"compartmentId = '{compartment_id}'"
             f" && lifeCycleState != '{NatGateway.LIFECYCLE_STATE_TERMINATED}'"
             f" && lifeCycleState != '{NatGateway.LIFECYCLE_STATE_TERMINATING}'"
         )
@@ -545,15 +560,16 @@
                 CLUSTER_NAME_TAG,
                 tag_value
             )
             return
 
         for nat_gateway_summary in nat_gateway_summary_list:
             log.info("Cluster %s: Deleting NAT gateway %r", tag_value, nat_gateway_summary.display_name)
-            self.client.network.delete_nat_gateway(nat_gateway_summary.identifier)
+            if not config["dry_run"]:
+                self.client.network.delete_nat_gateway(nat_gateway_summary.identifier)
 
     def delete_route_tables(self, compartment_id: str, tag_value: str) -> None:
         """
         Deletes all route tables in supplied compartment which have the supplied tag. For the default route
         table, all rules are deleted; for all other route tables, the entire table is deleted.
         """
         where_clause = (
@@ -576,15 +592,16 @@
                 tag_value
             )
             return
 
         for route_table_summary in route_table_summary_list:
             try:
                 log.info("Cluster %s: Deleting route table %r", tag_value, route_table_summary.display_name)
-                self.client.network.delete_route_table(route_table_summary.identifier)
+                if not config["dry_run"]:
+                    self.client.network.delete_route_table(route_table_summary.identifier)
             except TransientServiceError as error:
                 #
                 # Attempting to the delete the default route table for a VCN throws an exception; it's safe
                 # to ignore because as long as the table has no rules, the VCN can still be deleted.
                 if error.code == 'IncorrectState' and 'is the default for VCN' in error.message:
                     self.client.network.delete_all_route_table_rules(route_table_summary.identifier)
                 else:
@@ -613,17 +630,19 @@
             return
 
         for vcn_summary in vcn_summary_list:
             log.info("Cluster %s: Deleting VCN %r", tag_value, vcn_summary.display_name)
             nsg_list = self.client.network.get_nsgs_in_vcn(vcn_summary.identifier, vcn_summary.compartment_id)
             for nsg in nsg_list:
                 log.debug("Cluster %s: Deleting NSG %r", tag_value, nsg.display_name)
-                self.client.network.delete_nsg(nsg.id)
+                if not config["dry_run"]:
+                    self.client.network.delete_nsg(nsg.id)
 
-            self.client.network.delete_vcn(vcn_summary.identifier)
+            if not config["dry_run"]:
+                self.client.network.delete_vcn(vcn_summary.identifier)
 
     def delete_instance_configurations(self, compartment_id: str, tag_value: str) -> None:
         where_clause = (
             f"compartmentId = '{compartment_id}'"
         )
 
         instance_configuration_summary_list = self.client.search.query_items_by_freeform_tag(
@@ -644,13 +663,17 @@
 
         num_instance_configurations_to_delete = len(instance_configuration_summary_list)
         log.info(
             "Cluster %s: Deleting %s instance configuration(s)",
             tag_value,
             num_instance_configurations_to_delete,
         )
+
+        if config["dry_run"]:
+            return
+
         for instance_configuration_summary in instance_configuration_summary_list:
             self.client.compute.delete_instance_configuration(instance_configuration_summary.identifier)
 
     # =============  helpers  ================
     def _validate_params(self):
         self._validate_access_credentials()
```

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/clusterlist.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/clusterlist.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/clusterstart.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/clusterstart.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/clusterstop.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/clusterstop.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/configuration.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/configuration.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/const.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/const.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/imagelist.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/imagelist.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/images.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/images.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/__init__.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/__init__.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/blockstorage.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/blockstorage.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/compute.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/compute.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/filestorage.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/filestorage.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/identity.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/identity.py`

 * *Files 17% similar despite different names*

```diff
@@ -47,14 +47,48 @@
         """
         region_subscriptions = oci.pagination.list_call_get_all_results(
             self._identity.list_region_subscriptions,
             self._config["tenancy"],
         ).data
         return region_subscriptions
 
+    def list_tag_namespaces(
+            self, compartment_id: str, include_subcompartments: bool
+    ) -> list[oci.identity.models.TagNamespace]:
+        """
+        Lists tag namespaces for the given compartment.
+
+        :param compartment_id:
+            OCID of the compartment in which to search for the availability domain
+        :param include_subcompartments:
+            Whether list tag namespaces of the sub-compartments of a given compartment id.
+        :return:
+            TagNamespace list
+        """
+        tag_namespaces = oci.pagination.list_call_get_all_results(
+            self._identity.list_tag_namespaces,
+            compartment_id=compartment_id, include_subcompartments=include_subcompartments
+        ).data
+        return tag_namespaces
+
+    def list_tags(self, tag_namespace_id: str) -> list[oci.identity.models.TagNamespaceSummary]:
+        """
+        Lists defined tags in a specified namespace.
+
+        :param tag_namespace_id:
+            OCI ID of the tag namespace in which we're listing defined tags.
+        :return:
+            TagNamespaceSummary list
+        """
+        tags = oci.pagination.list_call_get_all_results(
+            self._identity.list_tags,
+            tag_namespace_id=tag_namespace_id
+        ).data
+        return tags
+
     def get_availability_domains(self, compartment_id: str) -> list[oci.identity.models.AvailabilityDomain]:
         """
         Fetches all availability domains available in a given compartment
 
         :param compartment_id:
             OCID of the compartment in which to search for the availability domain
         :return:
```

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/marketplace.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/marketplace.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/search.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/search.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/virtual_network.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/virtual_network.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/oci_actions/workrequest.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/oci_actions/workrequest.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/summary.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/summary.py`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/clusterondemandoci/utils.py` & `cm-cluster-on-demand-oci-10.0.7/clusterondemandoci/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -156,7 +156,23 @@
         regexes = [fnmatch.translate(ensure_cod_prefix(pattern)) for pattern in config["filters"]]
         head_node_list = [
             node for node in head_node_list
             if any(re.match(regex, node.freeform_tags.get(CLUSTER_NAME_TAG)) for regex in regexes)
         ]
 
     return head_node_list
+
+
+def parse_defined_tags(s: str) -> tuple[str, str, str]:
+    # Convert user input string to a dictionary early, to build configuration.
+    # Postponing detailed tag validation to subsequent stages.
+    expected_tag_format = "namespace.tag_key.tag_value"
+    try:
+        namespace, tag_key, tag_value = s.split(".", maxsplit=2)
+    except Exception as e:
+        raise CODException(
+            f"Unable to parse provided tag.\n"
+            f"Expected format: {expected_tag_format!r}, received {s!r}.\n"
+            f"Error: {e}"
+        )
+
+    return namespace, tag_key, tag_value
```

### Comparing `cm-cluster-on-demand-oci-10.0.6/cm_cluster_on_demand_oci.egg-info/PKG-INFO` & `cm-cluster-on-demand-oci-10.0.7/cm_cluster_on_demand_oci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm-cluster-on-demand-oci
-Version: 10.0.6
+Version: 10.0.7
 Summary: Bright Cluster on Demand Utility OCI
 Home-page: https://www.brightcomputing.com/
 Author: Cloudteam
 Author-email: cloudteam@brightcomputing.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cm-cluster-on-demand-oci-10.0.6/cm_cluster_on_demand_oci.egg-info/SOURCES.txt` & `cm-cluster-on-demand-oci-10.0.7/cm_cluster_on_demand_oci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-oci-10.0.6/setup.py` & `cm-cluster-on-demand-oci-10.0.7/setup.py`

 * *Files identical despite different names*

