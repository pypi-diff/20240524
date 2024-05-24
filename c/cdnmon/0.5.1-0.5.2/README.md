# Comparing `tmp/cdnmon-0.5.1.tar.gz` & `tmp/cdnmon-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdnmon-0.5.1.tar", max compression
+gzip compressed data, was "cdnmon-0.5.2.tar", max compression
```

## Comparing `cdnmon-0.5.1.tar` & `cdnmon-0.5.2.tar`

### file list

```diff
@@ -1,57 +1,59 @@
--rw-r--r--   0        0        0      636 2024-05-16 01:19:02.151957 cdnmon-0.5.1/README.md
--rw-r--r--   0        0        0      536 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/__init__.py
--rw-r--r--   0        0        0     6863 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/__init__.py
--rw-r--r--   0        0        0      338 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/advancedhosting.py
--rw-r--r--   0        0        0     1766 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/akamai.py
--rw-r--r--   0        0        0    13674 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/alibaba_cdn.py
--rw-r--r--   0        0        0     1502 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/alibaba_dcdn.py
--rw-r--r--   0        0        0      728 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/alibaba_waf.py
--rw-r--r--   0        0        0      335 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/asia_isp.py
--rw-r--r--   0        0        0      498 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/baidu.py
--rw-r--r--   0        0        0      406 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/baishan.py
--rw-r--r--   0        0        0      205 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/beluga.py
--rw-r--r--   0        0        0      292 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/bunny.py
--rw-r--r--   0        0        0      211 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/cachefly.py
--rw-r--r--   0        0        0      202 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/cdn77.py
--rw-r--r--   0        0        0      217 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/cdnetworks.py
--rw-r--r--   0        0        0      211 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/cdnvideo.py
--rw-r--r--   0        0        0      217 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/chinacache.py
--rw-r--r--   0        0        0      365 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/chinanet.py
--rw-r--r--   0        0        0     1128 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/cloudflare.py
--rw-r--r--   0        0        0     1283 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/cloudfront.py
--rw-r--r--   0        0        0      423 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/ctyun.py
--rw-r--r--   0        0        0      202 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/dnion.py
--rw-r--r--   0        0        0      359 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/douyin.py
--rw-r--r--   0        0        0      307 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/edgecast.py
--rw-r--r--   0        0        0      211 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/edgenext.py
--rw-r--r--   0        0        0      202 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/edgio.py
--rw-r--r--   0        0        0     1936 2024-05-16 01:19:02.151957 cdnmon-0.5.1/cdnmon/model/cdn/fastly.py
--rw-r--r--   0        0        0      309 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/fastly_edge_compute.py
--rw-r--r--   0        0        0      382 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/frontdoor.py
--rw-r--r--   0        0        0     1481 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/gcore.py
--rw-r--r--   0        0        0     1620 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/google.py
--rw-r--r--   0        0        0    11778 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/huawei.py
--rw-r--r--   0        0        0      208 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/imperva.py
--rw-r--r--   0        0        0      307 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/incapsula.py
--rw-r--r--   0        0        0      804 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/jingdong.py
--rw-r--r--   0        0        0      295 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/keycdn.py
--rw-r--r--   0        0        0      417 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/kingsoft.py
--rw-r--r--   0        0        0      227 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/leaseweb.py
--rw-r--r--   0        0        0      218 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/lumen.py
--rw-r--r--   0        0        0     1438 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/maxcdn.py
--rw-r--r--   0        0        0      230 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/medianova.py
--rw-r--r--   0        0        0      887 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/qihoo.py
--rw-r--r--   0        0        0      369 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/qiniu.py
--rw-r--r--   0        0        0      230 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/tata_communications.py
--rw-r--r--   0        0        0     1352 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/tencent.py
--rw-r--r--   0        0        0      604 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/ucloud.py
--rw-r--r--   0        0        0      366 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/upyun.py
--rw-r--r--   0        0        0      224 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/verizon.py
--rw-r--r--   0        0        0      353 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/volc.py
--rw-r--r--   0        0        0     1043 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/model/cdn/wangsu.py
--rw-r--r--   0        0        0      691 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/util/aws.py
--rw-r--r--   0        0        0     1076 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/util/bgpview.py
--rw-r--r--   0        0        0      389 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/util/cidr.py
--rw-r--r--   0        0        0      258 2024-05-16 01:19:02.155957 cdnmon-0.5.1/cdnmon/util/db.py
--rw-r--r--   0        0        0      513 2024-05-16 01:19:02.155957 cdnmon-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 cdnmon-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      636 2024-05-24 04:57:58.921685 cdnmon-0.5.2/README.md
+-rw-r--r--   0        0        0      536 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/__init__.py
+-rw-r--r--   0        0        0     7852 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/__init__.py
+-rw-r--r--   0        0        0      338 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/advancedhosting.py
+-rw-r--r--   0        0        0     1766 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/akamai.py
+-rw-r--r--   0        0        0    14006 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/alibaba_cdn.py
+-rw-r--r--   0        0        0     1502 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/alibaba_dcdn.py
+-rw-r--r--   0        0        0      728 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/alibaba_waf.py
+-rw-r--r--   0        0        0      335 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/asia_isp.py
+-rw-r--r--   0        0        0      498 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/baidu.py
+-rw-r--r--   0        0        0      406 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/baishan.py
+-rw-r--r--   0        0        0      205 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/beluga.py
+-rw-r--r--   0        0        0      292 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/bunny.py
+-rw-r--r--   0        0        0      211 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/cachefly.py
+-rw-r--r--   0        0        0      202 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/cdn77.py
+-rw-r--r--   0        0        0      217 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/cdnetworks.py
+-rw-r--r--   0        0        0      211 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/cdnvideo.py
+-rw-r--r--   0        0        0      217 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/chinacache.py
+-rw-r--r--   0        0        0      365 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/chinanet.py
+-rw-r--r--   0        0        0     1128 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/cloudflare.py
+-rw-r--r--   0        0        0     1283 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/cloudfront.py
+-rw-r--r--   0        0        0      498 2024-05-24 04:57:58.921685 cdnmon-0.5.2/cdnmon/model/cdn/ctyun.py
+-rw-r--r--   0        0        0      202 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/dnion.py
+-rw-r--r--   0        0        0      515 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/douyin.py
+-rw-r--r--   0        0        0      307 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/edgecast.py
+-rw-r--r--   0        0        0      211 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/edgenext.py
+-rw-r--r--   0        0        0      202 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/edgio.py
+-rw-r--r--   0        0        0     2031 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/fastly.py
+-rw-r--r--   0        0        0      309 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/fastly_edge_compute.py
+-rw-r--r--   0        0        0      382 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/frontdoor.py
+-rw-r--r--   0        0        0     1481 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/gcore.py
+-rw-r--r--   0        0        0     1620 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/google.py
+-rw-r--r--   0        0        0    11778 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/huawei.py
+-rw-r--r--   0        0        0      208 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/imperva.py
+-rw-r--r--   0        0        0      307 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/incapsula.py
+-rw-r--r--   0        0        0      804 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/jingdong.py
+-rw-r--r--   0        0        0      295 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/keycdn.py
+-rw-r--r--   0        0        0      417 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/kingsoft.py
+-rw-r--r--   0        0        0      538 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/leaseweb.py
+-rw-r--r--   0        0        0      218 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/lumen.py
+-rw-r--r--   0        0        0     1438 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/maxcdn.py
+-rw-r--r--   0        0        0      230 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/medianova.py
+-rw-r--r--   0        0        0      323 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/mi.py
+-rw-r--r--   0        0        0      352 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/netease.py
+-rw-r--r--   0        0        0      887 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/qihoo.py
+-rw-r--r--   0        0        0      369 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/qiniu.py
+-rw-r--r--   0        0        0      230 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/tata_communications.py
+-rw-r--r--   0        0        0     1352 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/tencent.py
+-rw-r--r--   0        0        0      604 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/ucloud.py
+-rw-r--r--   0        0        0      366 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/upyun.py
+-rw-r--r--   0        0        0      224 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/verizon.py
+-rw-r--r--   0        0        0      432 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/volc.py
+-rw-r--r--   0        0        0     1043 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/model/cdn/wangsu.py
+-rw-r--r--   0        0        0      691 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/util/aws.py
+-rw-r--r--   0        0        0     1051 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/util/bgpview.py
+-rw-r--r--   0        0        0      389 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/util/cidr.py
+-rw-r--r--   0        0        0      258 2024-05-24 04:57:58.925685 cdnmon-0.5.2/cdnmon/util/db.py
+-rw-r--r--   0        0        0      531 2024-05-24 04:57:58.925685 cdnmon-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 cdnmon-0.5.2/PKG-INFO
```

### Comparing `cdnmon-0.5.1/README.md` & `cdnmon-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/__init__.py` & `cdnmon-0.5.2/cdnmon/__init__.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/__init__.py` & `cdnmon-0.5.2/cdnmon/model/cdn/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import functools
+import glob
 import ipaddress
 import os
 import sys
 import tempfile
 from dataclasses import dataclass
 from dataclasses import field
 from typing import List
@@ -59,23 +60,23 @@
 
     def ipv4_prefixes(self) -> List[str]:
         ipv4_networks = []
         for query_term in self.query_term_list:
             data = self.bgpview_client.search(query_term)
             for item in data["data"]["ipv4_prefixes"]:
                 ipv4_networks.append(str(ipaddress.IPv4Network(item["prefix"], strict=False)))
-        return deduplicate_networks(ipv4_networks)
+        return deduplicate_networks(ipv4_networks, filter_version=4)
 
     def ipv6_prefixes(self) -> List[str]:
         ipv6_networks = []
         for query_term in self.query_term_list:
             data = self.bgpview_client.search(query_term)
             for item in data["data"]["ipv6_prefixes"]:
                 ipv6_networks.append(str(ipaddress.IPv6Network(item["prefix"], strict=False)))
-        return deduplicate_networks(ipv6_networks)
+        return deduplicate_networks(ipv6_networks, filter_version=6)
 
 
 @dataclass
 class CNAMEPattern:
     suffix: str = ""
     pattern: str = ""
     source: str = ""
@@ -98,44 +99,79 @@
         if not os.getenv("MONGODB_URI"):
             logger.warning("MONGODB_URI is not set")
             return []
 
         suffix = self.suffix if self.suffix.endswith(".") else self.suffix + "."
         pattern = f'^{suffix[::-1].replace(".", chr(92)+".")}'
         filter = {
-            "task.qtype": "A",
             "task.dns.response.answers.cname_reverse": {"$regex": pattern},
-            "task.dns.response.answers.a": {"$exists": True, "$ne": []},
         }
         collection = db.get_mongo_collection("kepler", "dns")
         domain_set = set()
         for item in collection.find(filter).limit(1):
             qname = item["task"]["qname"]
             logger.warning("{} | {}", qname, self.suffix)
             domain_set.add(qname)
         return list(domain_set)
 
 
 @dataclass
+class DomainOwnershipVerification:
+    supported: bool = field(default=False)
+    suffix: str = field(default_factory=str)
+    pattern: str = field(default_factory=str)
+    is_brutable: bool = field(default=False)
+
+    def __dict__(self) -> dict:
+        return {
+            "supported": self.supported,
+            "suffix": self.suffix,
+            "pattern": self.pattern,
+            "is_brutable": self.is_brutable,
+        }
+
+
+@dataclass
+class HTTPOwnershipVerification:
+    supported: bool = field(default=False)
+    path: str = field(default_factory=str)
+    pattern: str = field(default_factory=str)
+    is_brutable: bool = field(default=False)
+
+    def __dict__(self) -> dict:
+        return {
+            "supported": self.supported,
+            "path": self.path,
+            "pattern": self.pattern,
+            "is_brutable": self.is_brutable,
+        }
+
+
+@dataclass
+class OwnershipVerification:
+    txt: DomainOwnershipVerification = field(default_factory=DomainOwnershipVerification)
+    http: HTTPOwnershipVerification = field(default_factory=HTTPOwnershipVerification)
+
+    def __dict__(self) -> dict:
+        result = {}
+        if self.txt.supported:
+            result["txt"] = self.txt.__dict__()
+        if self.http.supported:
+            result["http"] = self.http.__dict__()
+        return result
+
+
+@dataclass
 class CommonCDN:
-    name: str
+    name: str = field(default_factory=str)
     asn_patterns: list[str] = field(default_factory=list)
     cname_suffixes: list[CNAMEPattern] = field(default_factory=list)
-
-    def __init__(
-        self,
-        name: str,
-        asn_patterns: List[str],
-        cname_suffixes: List[CNAMEPattern],
-        cidr: CIDR,
-    ):
-        self.name = name
-        self.asn_patterns = asn_patterns
-        self.cname_suffixes = cname_suffixes
-        self.cidr = cidr
+    cidr: CIDR = field(default_factory=CIDR)
+    frontend_ownership_verification: OwnershipVerification = field(default_factory=OwnershipVerification)
+    backend_ownership_verification: OwnershipVerification = field(default_factory=OwnershipVerification)
 
     def ipv4_prefixes(self) -> List[str]:
         return self.cidr.ipv4_prefixes()
 
     def ipv6_prefixes(self) -> List[str]:
         return self.cidr.ipv6_prefixes()
 
@@ -161,26 +197,31 @@
                     ),
                 ),
             ),
             "assets",
             "cdn",
             f"{self.name}.yaml",
         )
-        with open(path, mode="r", encoding="utf-8") as f:
-            old_content = f.read()
+
+        old_content = ""
+        if os.path.exists(path):
+            with open(path, mode="r", encoding="utf-8") as f:
+                old_content = f.read()
 
         with tempfile.NamedTemporaryFile(mode="w", encoding="utf-8", delete=False) as f:
             temporary_filename = f.name
             yaml.dump(
                 {
                     "name": self.name,
                     "asn_patterns": self.asn_patterns,
                     "cname_suffixes": [i.marshal() for i in self.cname_suffixes],
                     "ipv4_prefixes": self.ipv4_prefixes(),
                     "ipv6_prefixes": self.ipv6_prefixes(),
+                    "frontend_ownership_verification": self.frontend_ownership_verification.__dict__(),
+                    "backend_ownership_verification": self.backend_ownership_verification.__dict__(),
                     "updated_at": datetime.datetime.now().isoformat(),
                 },
                 f,
             )
 
         with open(temporary_filename, mode="r", encoding="utf-8") as f:
             new_content = f.read()
@@ -194,55 +235,12 @@
             return True
         else:
             # remove temporary file
             os.remove(temporary_filename)
             return False
 
 
-__all__ = [
-    "advancedhosting",
-    "akamai",
-    "alibaba_cdn",
-    "alibaba_dcdn",
-    "alibaba_waf",
-    "asia_isp",
-    "baidu",
-    "baishan",
-    "beluga",
-    "bunny",
-    "cachefly",
-    "cdn77",
-    "cdnetworks",
-    "cdnvideo",
-    "chinacache",
-    "cloudflare",
-    "cloudfront",
-    "ctyun",
-    "dnion",
-    "douyin",
-    "edgecast",
-    "edgenext",
-    "edgio",
-    "fastly_edge_compute",
-    "fastly",
-    "frontdoor",
-    "gcore",
-    "google",
-    "huawei",
-    "imperva",
-    "incapsula",
-    "jingdong",
-    "keycdn",
-    "kingsoft",
-    "leaseweb",
-    "lumen",
-    "maxcdn",
-    "medianova",
-    "qiniu",
-    "tata_communications",
-    "tencent",
-    "ucloud",
-    "upyun",
-    "verizon",
-    "volc",
-    "wangsu",
-]
+__all__ = []
+for path in glob.glob(f"{os.path.dirname(__file__)}/*.py"):
+    name, _ = os.path.splitext(os.path.basename(path))
+    if name != "__init__":
+        __all__.append(name)
```

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/akamai.py` & `cdnmon-0.5.2/cdnmon/model/cdn/akamai.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/alibaba_cdn.py` & `cdnmon-0.5.2/cdnmon/model/cdn/alibaba_cdn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from cdnmon.model.cdn import BGPViewCIDR
 from cdnmon.model.cdn import CNAMEPattern
 from cdnmon.model.cdn import CommonCDN
+from cdnmon.model.cdn import DomainOwnershipVerification
+from cdnmon.model.cdn import OwnershipVerification
 
 CDN = CommonCDN(
     name="alibaba-cdn",
     asn_patterns=["alibaba", "taobao", "alicloud"],
     cname_suffixes=[
         CNAMEPattern(suffix=".cdngslb.com", pattern=r"${domain}.cdngslb.com"),
         CNAMEPattern(suffix=".queniuaa.com", pattern=r"${domain}.queniuaa.com"),
@@ -169,8 +171,15 @@
         CNAMEPattern(suffix=".queniuzl.com", pattern=r"${domain}.queniuzl.com"),
         CNAMEPattern(suffix=".queniuzp.com", pattern=r"${domain}.queniuzp.com"),
         CNAMEPattern(suffix=".queniuzv.com", pattern=r"${domain}.queniuzv.com"),
         CNAMEPattern(suffix=".queniuzy.com", pattern=r"${domain}.queniuzy.com"),
         CNAMEPattern(suffix=".queniuzz.com", pattern=r"${domain}.queniuzz.com"),
     ],
     cidr=BGPViewCIDR(["alibaba", "taobao", "alicloud"]),
+    frontend_ownership_verification=OwnershipVerification(
+        txt=DomainOwnershipVerification(
+            supported=True,
+            suffix="verification",
+            pattern=r"verify_[0-9a-f]{32}",
+        )
+    ),
 )
```

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/alibaba_dcdn.py` & `cdnmon-0.5.2/cdnmon/model/cdn/alibaba_dcdn.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/alibaba_waf.py` & `cdnmon-0.5.2/cdnmon/model/cdn/alibaba_waf.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/cloudflare.py` & `cdnmon-0.5.2/cdnmon/model/cdn/cloudflare.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/cloudfront.py` & `cdnmon-0.5.2/cdnmon/model/cdn/cloudfront.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/fastly.py` & `cdnmon-0.5.2/cdnmon/model/cdn/fastly.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,10 +43,12 @@
     asn_patterns=["fastly"],
     cname_suffixes=[
         CNAMEPattern(suffix=".global.ssl.fastly.net", pattern=r"${name}.global.ssl.fastly.net"),
         CNAMEPattern(suffix=".freetls.fastly.net", pattern=r"${name}.freetls.fastly.net"),
         CNAMEPattern(suffix=".global.prod.fastly.net", pattern=r"${domain}.global.prod.fastly.net"),
         CNAMEPattern(suffix=".nonssl.global.fastly.net", pattern=r"nonssl.global.fastly.net"),
         CNAMEPattern(suffix=".nonssl.us-eu.fastly.net", pattern=r"nonssl.us-eu.fastly.net"),
+        CNAMEPattern(suffix=".global.fastly.net"),
+        CNAMEPattern(suffix=".fastly.net"),
     ],
     cidr=FastlyCIDR(),
 )
```

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/gcore.py` & `cdnmon-0.5.2/cdnmon/model/cdn/gcore.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/google.py` & `cdnmon-0.5.2/cdnmon/model/cdn/google.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/huawei.py` & `cdnmon-0.5.2/cdnmon/model/cdn/huawei.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/jingdong.py` & `cdnmon-0.5.2/cdnmon/model/cdn/jingdong.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/maxcdn.py` & `cdnmon-0.5.2/cdnmon/model/cdn/maxcdn.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/qihoo.py` & `cdnmon-0.5.2/cdnmon/model/cdn/qihoo.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/tencent.py` & `cdnmon-0.5.2/cdnmon/model/cdn/tencent.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/ucloud.py` & `cdnmon-0.5.2/cdnmon/model/cdn/ucloud.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/model/cdn/wangsu.py` & `cdnmon-0.5.2/cdnmon/model/cdn/wangsu.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/util/aws.py` & `cdnmon-0.5.2/cdnmon/util/aws.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.1/cdnmon/util/bgpview.py` & `cdnmon-0.5.2/cdnmon/util/bgpview.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,12 +26,12 @@
         logger.info(
             f"{response.status_code} {response.reason} | GET {url}  ({humanize.naturalsize(len(response.content))} Bytes)"
         )
         return response.json()
 
 
 def main():
-    BGPViewClient.transform(BGPViewClient.search("alicloud"))
+    BGPViewClient.search("alicloud")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cdnmon-0.5.1/pyproject.toml` & `cdnmon-0.5.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "cdnmon"
-version = "0.5.1"
+version = "0.5.2"
 description = ""
 authors = ["Yihang Wang <wangyihanger@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
 coloredlogs = "^15.0.1"
 pyyaml = "^6.0.1"
 ipy = "^1.1"
 pymongo = "^4.7.2"
 dynaconf = "^3.2.5"
 loguru = "^0.7.2"
 humanize = "^4.9.0"
+jinja2 = "^3.1.4"
 
 
 [tool.poetry.group.dev.dependencies]
 build = "^0.10.0"
 twine = "^4.0.2"
 deptry = "^0.16.1"
```

### Comparing `cdnmon-0.5.1/PKG-INFO` & `cdnmon-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: cdnmon
-Version: 0.5.1
+Version: 0.5.2
 Summary: 
 Author: Yihang Wang
 Author-email: wangyihanger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: dynaconf (>=3.2.5,<4.0.0)
 Requires-Dist: humanize (>=4.9.0,<5.0.0)
 Requires-Dist: ipy (>=1.1,<2.0)
+Requires-Dist: jinja2 (>=3.1.4,<4.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pymongo (>=4.7.2,<5.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 ## Introduction
```

