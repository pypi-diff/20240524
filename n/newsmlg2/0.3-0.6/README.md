# Comparing `tmp/newsmlg2-0.3.tar.gz` & `tmp/newsmlg2-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newsmlg2-0.3.tar", last modified: Tue Oct 12 10:35:59 2021, max compression
+gzip compressed data, was "newsmlg2-0.6.tar", last modified: Fri May 24 13:52:15 2024, max compression
```

## Comparing `newsmlg2-0.3.tar` & `newsmlg2-0.6.tar`

### file list

```diff
@@ -1,46 +1,54 @@
-drwxr-xr-x   0 brendan    (501) staff       (20)        0 2021-10-12 10:35:59.178388 newsmlg2-0.3/
--rw-r--r--   0 brendan    (501) staff       (20)     1114 2021-10-12 10:20:31.000000 newsmlg2-0.3/LICENSE
-drwxr-xr-x   0 brendan    (501) staff       (20)        0 2021-10-12 10:35:59.176101 newsmlg2-0.3/NewsMLG2/
--rw-r--r--   0 brendan    (501) staff       (20)      709 2021-10-12 10:12:28.000000 newsmlg2-0.3/NewsMLG2/__init__.py
--rw-r--r--   0 brendan    (501) staff       (20)    10728 2021-10-12 09:29:52.000000 newsmlg2-0.3/NewsMLG2/anyitem.py
--rw-r--r--   0 brendan    (501) staff       (20)    32143 2021-07-08 09:04:54.000000 newsmlg2-0.3/NewsMLG2/attributegroups.py
--rw-r--r--   0 brendan    (501) staff       (20)     9339 2021-10-12 09:21:06.000000 newsmlg2-0.3/NewsMLG2/catalog.py
--rw-r--r--   0 brendan    (501) staff       (20)     1043 2021-08-04 13:15:53.000000 newsmlg2-0.3/NewsMLG2/catalogitem.py
--rw-r--r--   0 brendan    (501) staff       (20)     1613 2021-05-26 12:04:01.000000 newsmlg2-0.3/NewsMLG2/catalogstore.py
--rw-r--r--   0 brendan    (501) staff       (20)     5299 2021-07-09 09:49:54.000000 newsmlg2-0.3/NewsMLG2/complextypes.py
--rw-r--r--   0 brendan    (501) staff       (20)     1307 2021-07-16 09:36:53.000000 newsmlg2-0.3/NewsMLG2/conceptitem.py
--rw-r--r--   0 brendan    (501) staff       (20)     9057 2021-07-16 12:45:14.000000 newsmlg2-0.3/NewsMLG2/conceptrelationships.py
--rw-r--r--   0 brendan    (501) staff       (20)    18220 2021-07-16 12:44:46.000000 newsmlg2-0.3/NewsMLG2/concepts.py
--rw-r--r--   0 brendan    (501) staff       (20)    17764 2021-07-16 12:48:57.000000 newsmlg2-0.3/NewsMLG2/contentmeta.py
--rw-r--r--   0 brendan    (501) staff       (20)    14208 2021-10-12 10:14:36.000000 newsmlg2-0.3/NewsMLG2/core.py
--rwxr-xr-x   0 brendan    (501) staff       (20)     2815 2021-07-24 13:55:24.000000 newsmlg2-0.3/NewsMLG2/document.py
--rw-r--r--   0 brendan    (501) staff       (20)    12440 2021-07-16 09:33:37.000000 newsmlg2-0.3/NewsMLG2/entities.py
--rw-r--r--   0 brendan    (501) staff       (20)     1315 2021-07-09 09:52:30.000000 newsmlg2-0.3/NewsMLG2/extensionproperties.py
--rw-r--r--   0 brendan    (501) staff       (20)     3771 2021-07-09 09:13:37.000000 newsmlg2-0.3/NewsMLG2/ids.py
--rw-r--r--   0 brendan    (501) staff       (20)     9595 2021-07-16 12:53:58.000000 newsmlg2-0.3/NewsMLG2/itemmanagement.py
--rw-r--r--   0 brendan    (501) staff       (20)     5245 2021-07-16 09:32:34.000000 newsmlg2-0.3/NewsMLG2/knowledgeitem.py
--rw-r--r--   0 brendan    (501) staff       (20)     5699 2021-07-16 09:32:11.000000 newsmlg2-0.3/NewsMLG2/labeltypes.py
--rw-r--r--   0 brendan    (501) staff       (20)     6478 2021-07-09 08:59:34.000000 newsmlg2-0.3/NewsMLG2/link.py
--rw-r--r--   0 brendan    (501) staff       (20)     7730 2021-07-16 09:30:42.000000 newsmlg2-0.3/NewsMLG2/newsitem.py
--rw-r--r--   0 brendan    (501) staff       (20)     5296 2021-07-16 09:31:37.000000 newsmlg2-0.3/NewsMLG2/packageitem.py
--rw-r--r--   0 brendan    (501) staff       (20)     8641 2021-07-16 12:50:40.000000 newsmlg2-0.3/NewsMLG2/partmeta.py
--rw-r--r--   0 brendan    (501) staff       (20)     6075 2021-07-16 09:30:59.000000 newsmlg2-0.3/NewsMLG2/rights.py
--rw-r--r--   0 brendan    (501) staff       (20)     3874 2021-07-09 09:50:23.000000 newsmlg2-0.3/NewsMLG2/simpletypes.py
--rw-r--r--   0 brendan    (501) staff       (20)     1685 2021-10-12 10:03:55.000000 newsmlg2-0.3/NewsMLG2/utils.py
--rw-r--r--   0 brendan    (501) staff       (20)     6094 2021-10-12 10:35:59.178474 newsmlg2-0.3/PKG-INFO
--rw-r--r--   0 brendan    (501) staff       (20)     4361 2021-10-12 10:32:06.000000 newsmlg2-0.3/README.md
-drwxr-xr-x   0 brendan    (501) staff       (20)        0 2021-10-12 10:35:59.176816 newsmlg2-0.3/newsmlg2.egg-info/
--rw-r--r--   0 brendan    (501) staff       (20)     6094 2021-10-12 10:35:59.000000 newsmlg2-0.3/newsmlg2.egg-info/PKG-INFO
--rw-r--r--   0 brendan    (501) staff       (20)      939 2021-10-12 10:35:59.000000 newsmlg2-0.3/newsmlg2.egg-info/SOURCES.txt
--rw-r--r--   0 brendan    (501) staff       (20)        1 2021-10-12 10:35:59.000000 newsmlg2-0.3/newsmlg2.egg-info/dependency_links.txt
--rw-r--r--   0 brendan    (501) staff       (20)        5 2021-10-12 10:35:59.000000 newsmlg2-0.3/newsmlg2.egg-info/requires.txt
--rw-r--r--   0 brendan    (501) staff       (20)       15 2021-10-12 10:35:59.000000 newsmlg2-0.3/newsmlg2.egg-info/top_level.txt
--rw-r--r--   0 brendan    (501) staff       (20)      108 2021-10-12 10:35:59.178674 newsmlg2-0.3/setup.cfg
--rw-r--r--   0 brendan    (501) staff       (20)     1218 2021-10-12 10:35:43.000000 newsmlg2-0.3/setup.py
-drwxr-xr-x   0 brendan    (501) staff       (20)        0 2021-10-12 10:35:59.178162 newsmlg2-0.3/tests/
--rw-r--r--   0 brendan    (501) staff       (20)        0 2021-05-24 19:10:25.000000 newsmlg2-0.3/tests/__init__.py
--rwxr-xr-x   0 brendan    (501) staff       (20)     7243 2021-10-12 10:20:49.000000 newsmlg2-0.3/tests/test_catalogitems.py
--rwxr-xr-x   0 brendan    (501) staff       (20)     6177 2021-10-12 10:20:54.000000 newsmlg2-0.3/tests/test_conceptitems.py
--rwxr-xr-x   0 brendan    (501) staff       (20)     9066 2021-10-12 10:21:01.000000 newsmlg2-0.3/tests/test_knowledgeitems.py
--rwxr-xr-x   0 brendan    (501) staff       (20)    18409 2021-10-12 10:21:05.000000 newsmlg2-0.3/tests/test_newsitems.py
--rwxr-xr-x   0 brendan    (501) staff       (20)    14227 2021-10-12 10:21:10.000000 newsmlg2-0.3/tests/test_packageitems.py
+drwxr-xr-x   0 brendan    (501) staff       (20)        0 2024-05-24 13:52:15.310228 newsmlg2-0.6/
+-rw-r--r--   0 brendan    (501) staff       (20)     1114 2021-10-12 10:20:31.000000 newsmlg2-0.6/LICENSE
+drwxr-xr-x   0 brendan    (501) staff       (20)        0 2024-05-24 13:52:15.306502 newsmlg2-0.6/NewsMLG2/
+-rw-r--r--   0 brendan    (501) staff       (20)     1149 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/__init__.py
+-rw-r--r--   0 brendan    (501) staff       (20)    10195 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/anyitem.py
+-rw-r--r--   0 brendan    (501) staff       (20)    32903 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/attributegroups.py
+-rw-r--r--   0 brendan    (501) staff       (20)     9295 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/catalog.py
+-rw-r--r--   0 brendan    (501) staff       (20)     1043 2021-08-04 13:15:53.000000 newsmlg2-0.6/NewsMLG2/catalogitem.py
+-rw-r--r--   0 brendan    (501) staff       (20)     1641 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/catalogstore.py
+-rw-r--r--   0 brendan    (501) staff       (20)     5044 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/complextypes.py
+-rw-r--r--   0 brendan    (501) staff       (20)     1307 2023-07-17 07:44:32.000000 newsmlg2-0.6/NewsMLG2/conceptitem.py
+-rw-r--r--   0 brendan    (501) staff       (20)     9056 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/conceptrelationships.py
+-rw-r--r--   0 brendan    (501) staff       (20)    17718 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/concepts.py
+-rw-r--r--   0 brendan    (501) staff       (20)    18196 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/contentmeta.py
+-rw-r--r--   0 brendan    (501) staff       (20)    14206 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/core.py
+-rwxr-xr-x   0 brendan    (501) staff       (20)     3237 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/document.py
+-rw-r--r--   0 brendan    (501) staff       (20)    12670 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/entities.py
+-rw-r--r--   0 brendan    (501) staff       (20)    19034 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/events.py
+-rw-r--r--   0 brendan    (501) staff       (20)     1315 2021-07-09 09:52:30.000000 newsmlg2-0.6/NewsMLG2/extensionproperties.py
+-rw-r--r--   0 brendan    (501) staff       (20)     3771 2021-07-09 09:13:37.000000 newsmlg2-0.6/NewsMLG2/ids.py
+-rw-r--r--   0 brendan    (501) staff       (20)     9595 2021-07-16 12:53:58.000000 newsmlg2-0.6/NewsMLG2/itemmanagement.py
+-rw-r--r--   0 brendan    (501) staff       (20)     5235 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/knowledgeitem.py
+-rw-r--r--   0 brendan    (501) staff       (20)     5699 2021-07-16 09:32:11.000000 newsmlg2-0.6/NewsMLG2/labeltypes.py
+-rw-r--r--   0 brendan    (501) staff       (20)     5462 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/link.py
+-rw-r--r--   0 brendan    (501) staff       (20)     7730 2021-07-16 09:30:42.000000 newsmlg2-0.6/NewsMLG2/newsitem.py
+-rw-r--r--   0 brendan    (501) staff       (20)     4857 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/newsmessage.py
+-rw-r--r--   0 brendan    (501) staff       (20)     5296 2021-07-16 09:31:37.000000 newsmlg2-0.6/NewsMLG2/packageitem.py
+-rw-r--r--   0 brendan    (501) staff       (20)     8641 2021-07-16 12:50:40.000000 newsmlg2-0.6/NewsMLG2/partmeta.py
+-rw-r--r--   0 brendan    (501) staff       (20)    10871 2023-07-17 07:44:32.000000 newsmlg2-0.6/NewsMLG2/planningitem.py
+-rw-r--r--   0 brendan    (501) staff       (20)     6376 2024-05-24 13:00:37.000000 newsmlg2-0.6/NewsMLG2/rights.py
+-rw-r--r--   0 brendan    (501) staff       (20)     3874 2021-07-09 09:50:23.000000 newsmlg2-0.6/NewsMLG2/simpletypes.py
+-rw-r--r--   0 brendan    (501) staff       (20)     1554 2023-07-19 08:05:27.000000 newsmlg2-0.6/NewsMLG2/utils.py
+-rw-r--r--   0 brendan    (501) staff       (20)     8429 2024-05-24 13:52:15.310348 newsmlg2-0.6/PKG-INFO
+-rw-r--r--   0 brendan    (501) staff       (20)     6321 2024-05-24 13:00:37.000000 newsmlg2-0.6/README.md
+drwxr-xr-x   0 brendan    (501) staff       (20)        0 2024-05-24 13:52:15.307078 newsmlg2-0.6/newsmlg2.egg-info/
+-rw-r--r--   0 brendan    (501) staff       (20)     8429 2024-05-24 13:52:15.000000 newsmlg2-0.6/newsmlg2.egg-info/PKG-INFO
+-rw-r--r--   0 brendan    (501) staff       (20)     1126 2024-05-24 13:52:15.000000 newsmlg2-0.6/newsmlg2.egg-info/SOURCES.txt
+-rw-r--r--   0 brendan    (501) staff       (20)        1 2024-05-24 13:52:15.000000 newsmlg2-0.6/newsmlg2.egg-info/dependency_links.txt
+-rw-r--r--   0 brendan    (501) staff       (20)        5 2024-05-24 13:52:15.000000 newsmlg2-0.6/newsmlg2.egg-info/requires.txt
+-rw-r--r--   0 brendan    (501) staff       (20)       15 2024-05-24 13:52:15.000000 newsmlg2-0.6/newsmlg2.egg-info/top_level.txt
+-rw-r--r--   0 brendan    (501) staff       (20)      108 2024-05-24 13:52:15.310576 newsmlg2-0.6/setup.cfg
+-rw-r--r--   0 brendan    (501) staff       (20)     1217 2024-05-24 13:50:42.000000 newsmlg2-0.6/setup.py
+drwxr-xr-x   0 brendan    (501) staff       (20)        0 2024-05-24 13:52:15.309983 newsmlg2-0.6/tests/
+-rw-r--r--   0 brendan    (501) staff       (20)        0 2021-05-24 19:10:25.000000 newsmlg2-0.6/tests/__init__.py
+-rw-r--r--   0 brendan    (501) staff       (20)     1793 2023-07-19 08:05:27.000000 newsmlg2-0.6/tests/test_autoloader.py
+-rwxr-xr-x   0 brendan    (501) staff       (20)     7159 2024-05-24 13:00:37.000000 newsmlg2-0.6/tests/test_catalogitems.py
+-rwxr-xr-x   0 brendan    (501) staff       (20)    11657 2024-05-24 13:00:37.000000 newsmlg2-0.6/tests/test_conceptitems.py
+-rw-r--r--   0 brendan    (501) staff       (20)     1875 2024-05-24 13:00:37.000000 newsmlg2-0.6/tests/test_core.py
+-rwxr-xr-x   0 brendan    (501) staff       (20)     7423 2024-05-24 13:00:37.000000 newsmlg2-0.6/tests/test_events.py
+-rwxr-xr-x   0 brendan    (501) staff       (20)     9202 2024-05-24 13:00:37.000000 newsmlg2-0.6/tests/test_knowledgeitems.py
+-rwxr-xr-x   0 brendan    (501) staff       (20)    30763 2024-05-24 13:00:37.000000 newsmlg2-0.6/tests/test_newsitems.py
+-rw-r--r--   0 brendan    (501) staff       (20)     7061 2024-05-24 13:00:37.000000 newsmlg2-0.6/tests/test_newsmessage.py
+-rwxr-xr-x   0 brendan    (501) staff       (20)    14227 2024-05-24 13:00:37.000000 newsmlg2-0.6/tests/test_packageitems.py
+-rwxr-xr-x   0 brendan    (501) staff       (20)    10061 2024-05-24 13:00:37.000000 newsmlg2-0.6/tests/test_planningitems.py
```

### Comparing `newsmlg2-0.3/LICENSE` & `newsmlg2-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `newsmlg2-0.3/NewsMLG2/anyitem.py` & `newsmlg2-0.6/NewsMLG2/anyitem.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
 AnyItemType definitions
 """
 
 from lxml import etree
 
-from .core import BaseObject, QCodeURIMixin
+from .core import BaseObject, NEWSMLG2_VERSION, QCodeURIMixin
 from .attributegroups import (
     CommonPowerAttributes, I18NAttributes, QuantifyAttributes
 )
 from .catalog import build_catalog, get_catalogs, CatalogRef, Catalog
 from .complextypes import Name, TruncatedDateTimePropType
 from .concepts import Flex1PropType
 from .extensionproperties import Flex2ExtPropType
@@ -177,26 +177,14 @@
     """
     def __init__(self,  **kwargs):
         super().__init__(**kwargs)
         assert self.itemclass is not None, "itemClass is required in any NewsML-G2 Item"
         assert self.provider is not None, "provider is required in any NewsML-G2 Item"
         assert self.versioncreated is not None, "versionCreated is required in any NewsML-G2 Item"
 
-    def get_service_uri(self):
-        """Return URI for first service in services array."""
-        return self.get_element_value('service')[0].get_uri()
-
-    def get_signal(self):
-        """Return QCode for first signal in signals array."""
-        return self.get_element_value('signal')[0].get_qcode()
-
-    def get_signal_uri(self):
-        """Return URI for first signal in signals array."""
-        return self.get_element_value('signal')[0].get_uri()
-
 
 class AnyItem(I18NAttributes):
     """
     An abstract class. All G2 items are inherited from this class.
     """
 
     attributes = {
@@ -207,16 +195,16 @@
             # we do, for ease of use reasons
             'default': 'NewsML-G2'
         },
         # The major-minor version of the IPTC standard with which the Item is conformant.
         'standardversion': {
             'xml_name': 'standardversion',
             # NOTE: the XML Schema doesn't define a default but
-            # we do, for ease of use reasons
-            'default': '2.29'
+            # we default to the most recent version, for ease of use
+            'default': NEWSMLG2_VERSION
         },
         # The conformance level with which the Item is conformant.
         'conformance': {
             'xml_name': 'conformance',
             # NOTE: the XML Schema defines default "core" but from 2.27+ the
             # Specification recommends only using "power"
             'default': 'power'
@@ -231,16 +219,14 @@
             'xml_name': 'version',
             'xml_type': 'positive integer',
             'default': '1'
         }
     }
 
     elements = [
-        # TODO implement xs:choice either "catalogRef" or "catalog"
-        # (but unlimited number of whichever one exists)
         ('catalogref', { 'type': 'array', 'xml_name': 'catalogRef', 'element_class': CatalogRef }),
         ('catalog', { 'type': 'array', 'xml_name': 'catalog', 'element_class': Catalog }),
         ('hophistory', { 'type': 'single', 'xml_name': 'hopHistory', 'element_class': HopHistory }),
         ('pubhistory', { 'type': 'single', 'xml_name': 'pubHistory', 'element_class': PubHistory }),
         ('rightsinfo', { 'type': 'array', 'xml_name': 'rightsInfo', 'element_class': RightsInfo }),
         ('itemmeta', { 'type': 'single', 'xml_name': 'itemMeta', 'element_class': ItemMeta })
     ]
```

### Comparing `newsmlg2-0.3/NewsMLG2/attributegroups.py` & `newsmlg2-0.6/NewsMLG2/attributegroups.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,21 +84,46 @@
         # Specifies the language of this property and potentially all
         # descendant properties. xml:lang values of descendant properties
         # override this value. Values are determined by Internet BCP 47.
         'xml_lang': {
             'xml_name': XMLNSPREFIX+'lang'
         },
         # The directionality of textual content
-        # (enumeration: ltr, rtl)
+        # (TODO enumeration: ltr, rtl)
         'dir': {
             'xml_name': 'dir'
         }
     }
 
 
+class AuthorityAttributes(BaseObject):
+    """
+    A group of attributes for defining the authority that manages/maintains
+    a catalog or scheme
+
+    Added in NewsML-G2 2.32
+    """
+    attributes = {
+        # Defines the authority controlling this catalog
+        'authority': {
+            'xml_name': 'authority'
+        },
+        # The status of the Authority associated with the Scheme - expressed as a QCode.
+        'authoritystatus': {
+            'xml_name': 'authoritystatus',
+            'xml_type': 'QCodeType'
+        },
+        # The status of the Authority associated with the Scheme - expressed as a URI.
+        'authoritystatusuri': {
+            'xml_name': 'authoritystatusuri',
+            'xml_type': 'IRIType'
+        }
+    }
+
+
 class QuantifyAttributes(BaseObject):
     """
     A group of attriubutes quantifying the property value
     """
     attributes = {
         # The confidence with which the metadata has been assigned.
         'confidence': {
```

### Comparing `newsmlg2-0.3/NewsMLG2/catalog.py` & `newsmlg2-0.6/NewsMLG2/catalog.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 aliases and locations)
 """
 
 import os
 from lxml import etree
 
 from .core import NEWSMLG2NSPREFIX, BaseObject
-from .attributegroups import CommonPowerAttributes, I18NAttributes
+from .attributegroups import (
+    AuthorityAttributes, CommonPowerAttributes, I18NAttributes
+)
 from .complextypes import Name
 from .concepts import Definition, Note
 from .conceptrelationships import SameAs
 from .contentmeta import ContentMetadataCatType
 from .labeltypes import Label1Type
 from .simpletypes import IRIType
 from .catalogstore import CATALOG_STORE
@@ -34,45 +36,51 @@
     'http://www.iptc.org/std/catalog/catalog.IPTC-G2-Standards_33.xml':
         'catalogs/catalog.IPTC-G2-Standards_33.xml',
     'http://www.iptc.org/std/catalog/catalog.IPTC-G2-Standards_34.xml':
         'catalogs/catalog.IPTC-G2-Standards_34.xml',
     'http://www.iptc.org/std/catalog/catalog.IPTC-G2-Standards_35.xml':
         'catalogs/catalog.IPTC-G2-Standards_35.xml',
     'http://www.iptc.org/std/catalog/catalog.IPTC-G2-Standards_36.xml':
-        'catalogs/catalog.IPTC-G2-Standards_36.xml'
+        'catalogs/catalog.IPTC-G2-Standards_36.xml',
+    'http://www.iptc.org/std/catalog/catalog.IPTC-G2-Standards_37.xml':
+        'catalogs/catalog.IPTC-G2-Standards_37.xml',
+    'http://www.iptc.org/std/catalog/catalog.IPTC-G2-Standards_38.xml':
+        'catalogs/catalog.IPTC-G2-Standards_38.xml'
 }
 
+
 def build_catalog(xmlelement):
     """
     Load all CVs referenced in local and remote catalogs.
     TODO:
-    - inline catalogs are not yet tested
-    - load and cache catalog from catalogRef href
+    - load and cache catalog from remote catalogRef href
     """
+    CATALOG_STORE.__init__([])
     catalogs = xmlelement.findall(NEWSMLG2NSPREFIX+'catalog')
-    catalog_refs = xmlelement.findall(NEWSMLG2NSPREFIX+'catalogRef')
     for catalog in catalogs:
         add_catalog(xmlelement=catalog)
+    catalog_refs = xmlelement.findall(NEWSMLG2NSPREFIX+'catalogRef')
     for catalog_ref in catalog_refs:
         href = catalog_ref.get('href')
 
         if href in CATALOG_CACHE:
-            # IPTC standard catalogs are built in, to avoid network traffic
-            # (and load on IPTC servers)
+            # IPTC standard catalogs are built in to this module
+            # to avoid network traffic (and load on IPTC servers)
             file = CATALOG_CACHE[href]
             add_catalog(uri=href, file=file)
         else:
             # TODO convert to a logged warning
             print("WARNING: Remote catalog {} declared. Remote "
                   "loading of catalogs is not yet supported.".format(href))
 
 
 def add_catalog(**kwargs):
     """
-    Load an individual catalog from a local file.
+    Load an individual catalog from a local file
+    or directly from an XML element.
     """
     if 'file' in kwargs:
         dirname = os.path.dirname(os.path.realpath(__file__))
         filename = os.path.join(dirname, kwargs['file'])
         xmltree = etree.parse(filename)
         catalog_element = xmltree.getroot()
         catalog = Catalog(xmlelement=catalog_element)
@@ -98,15 +106,15 @@
 class SameAsScheme(IRIType, CommonPowerAttributes):
     """
     A URI which identifies another scheme with concepts that use the
     same codes and are semantically equivalent to the concepts of this scheme
     """
 
 
-class Scheme(CommonPowerAttributes):
+class Scheme(AuthorityAttributes, CommonPowerAttributes):
     """
     A scheme alias-to-URI mapping.
     """
 
     elements = [
         ('sameasscheme', {
             'type': 'array', 'xml_name': 'sameAsScheme', 'element_class': SameAsScheme
@@ -134,19 +142,14 @@
         },
         # The URI which identifies the scheme.
         'uri': {
             'xml_name': 'uri',
             'xml_type': 'IRIType',
             'use': 'required'
         },
-        # Defines the authority controlling this scheme
-        'authority': {
-            'xml_name': 'authority',
-            'xml_type': 'IRIType'
-        },
         # The date (and, optionally, the time) when the scheme was created.
         # This must not be later than the creation timestamp of any concepts in the scheme.
         'schemecreated': {
             'xml_name': 'schemecreated',
             'xml_type': 'DateOptTimeType',
             'use': 'optional'
         },
@@ -167,15 +170,15 @@
         }
     }
 
     def __str__(self):
         return "{} ({}, {})".format(self.name, self.alias, self.uri)
 
 
-class Catalog(CommonPowerAttributes):
+class Catalog(AuthorityAttributes, CommonPowerAttributes):
     """
     A local or remote catalog.
     """
 
     _catalog = []
     elements = [
         ('title', {
@@ -196,19 +199,14 @@
         # Defines the location of the catalog as remote resource.
         # (Should be the same as the URL which is used with the href
         # attribute of a catalogRef in an item.)
         'url': {
             'xml_name': 'url',
             'xml_type': 'IRIType'
         },
-        # Defines the authority controlling this catalog
-        'authority': {
-            'xml_name': 'authority',
-            'xml_type': 'IRIType'
-        },
         # Globally Unique Identifier for this kind of catalog as
         # managed by a provider. A version attribute should be used with it.
         'guid': {
             'xml_name': 'guid',
             'xml_type': 'xs:anyURI'
         },
         # Version corresponding to the guid of the catalog.
@@ -243,30 +241,25 @@
             return self._catalog_alias_lookup[alias]
         return None
 
     def get_scheme_for_uri(self, uri):
         """Return the scheme matching a given URI"""
         if uri in self._catalog_uri_lookup.keys():
             return self._catalog_uri_lookup[uri]
-        return None
-
-    def __iter__(self):
-        for key in self._catalog:
-            yield key
 
     def __getitem__(self,index):
         return self._catalog[index]
 
     def __len__(self):
         return len(self._catalog)
 
-    def str(self):
+    def __str__(self):
         """String representation of the catalog object."""
         if self.title:
-            return '<Catalog '+self.title[0]+'>'
+            return '<Catalog "'+str(self.title[0])+'">'
         return '<Catalog>'
 
 
 class CatalogRef(BaseObject):
     """
     A reference to a remote catalog. A hyperlink to a set of scheme alias
     declarations.
```

### Comparing `newsmlg2-0.3/NewsMLG2/catalogitem.py` & `newsmlg2-0.6/NewsMLG2/catalogitem.py`

 * *Files identical despite different names*

### Comparing `newsmlg2-0.3/NewsMLG2/catalogstore.py` & `newsmlg2-0.6/NewsMLG2/catalogstore.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,50 +10,54 @@
     """Alias prefix not found in any catalogs"""
 
 
 class URINotFoundInCatalogs(Exception):
     """Catalog URI not found in any catalogs"""
 
 
-class CatalogStore(list):
+class CatalogStore():
     """
     Singleton class to handle all catalogs used
     in this NewsMLG2 processor.
     """
-    def __add__(self, rhs):
-        return CatalogStore(list.__add__(self, rhs))
+    _list = []
+    def __init__(self, val = []):
+        self._list = val
+
+    def append(self, rhs):
+        self._list.append(rhs)
+        return self
 
     def __getitem__(self, item):
         """
         Return a given catalog in our list.
         """
-        result = list.__getitem__(self, item)
-        try:
-            return CatalogStore(result)
-        except TypeError:
-            return result
+        return self._list.__getitem__(item)
+
+    def __len__(self):
+        return len(self._list)
 
     def get_scheme_for_alias(self, alias):
         """
         Return the catalog scheme matching a given alias.
         e.g. 'nrol' would return the Scheme for 'name role'.
         """
-        for catalog in self:
+        for catalog in self._list:
             scheme = catalog.get_scheme_for_alias(alias)
             if scheme is not None:
                 return scheme
         raise AliasNotFoundInCatalogs()
 
     def get_scheme_for_uri(self, uri):
         """
         Return the catalog scheme matching a given URI.
         e.g. 'https://cv.iptc.org/newscodes/scene' would return the Scheme for
         'scene'.
         """
-        for catalog in self:
+        for catalog in self._list:
             scheme = catalog.get_scheme_for_uri(uri)
             if scheme is not None:
                 return scheme
         raise URINotFoundInCatalogs()
 
 
 CATALOG_STORE = CatalogStore([])
```

### Comparing `newsmlg2-0.3/NewsMLG2/complextypes.py` & `newsmlg2-0.6/NewsMLG2/complextypes.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     """
     The type of a property with date and time
     In XML Schema, extends xsd:dateTime
 
     TODO add helper methods for date/time manipulation, timezone conversion etc
     """
 
-
 class DateOptTimePropType(DateOptTimeType, CommonPowerAttributes):
     """
     The type of a property with date and time
     In XML Schema, extends xsd:dateTime
     """
 
 
@@ -94,15 +93,14 @@
 
 class ConceptNameType(TimeValidityAttributes, IntlStringType):
     """
     The type of a natural language name for the concept (Type defined in this
     XML Schema only)
     """
     xml_element_name = 'name'
-    name = None
     attributes = {
         # A refinement of the semantics of the name - expressed by a QCode
         'role': {
             'xml_name': 'role'
         },
         # A refinement of the semantics of the name - expressed by a URI
         'roleuri': {
@@ -116,20 +114,15 @@
         # Specifies which part of a full name this property provides - expressed
         # by a URI
         'parturi': {
             'xml_name': 'parturi'
         }
     }
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        xmlelement = kwargs.get('xmlelement')
-        if isinstance(xmlelement, etree._Element):
-            self._name = xmlelement.text and xmlelement.text.strip()
-
+    # TODO this lookup is currently not used...
     _name_role_mappings = {
         # http://cv.iptc.org/newscodes/namerole/
         # http://cv.iptc.org/newscodes/namerole/adjectival
         'nrol:adjectival': 'adjectival',
         # http://cv.iptc.org/newscodes/namerole/alternate
         'nrol:alternate': 'alternate',
         # http://cv.iptc.org/newscodes/namerole/display
@@ -158,15 +151,12 @@
         # these are incorrect but found in SportsML sample files
         'nprt:first': 'given',
         'nrol:first': 'given',
         'nprt:last': 'family',
         'nrol:last': 'family'
     }
 
-    def __str__(self):
-        return self._name
-
 
 class Name(ConceptNameType):
     """
     Instance of ConceptNameType.
     """
```

### Comparing `newsmlg2-0.3/NewsMLG2/conceptitem.py` & `newsmlg2-0.6/NewsMLG2/conceptitem.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class ConceptItemContentMeta(ContentMetadataAcDType):
     """
     Content Metadata for a Concept Item
     User Note: For multiple concepts use a Knowledge Item
     """
-    xml_element_name = 'conceptItem'
+    xml_element_name = 'contentMeta'
 
 
 class ConceptItem(AnyItem):
     """
     An Item containing information about a concept.
     """
     elements = [
```

### Comparing `newsmlg2-0.3/NewsMLG2/conceptrelationships.py` & `newsmlg2-0.6/NewsMLG2/conceptrelationships.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
 
     elements = [
         ('name', { 'type': 'array', 'xml_name': 'name', 'element_class': Name }),
         ('hierarchyinfo', {
             'type': 'array', 'xml_name': 'hierarchyInfo',
             'element_class': HierarchyInfo
         }),
-        ('sameAs', {
+        ('sameas', {
             'type': 'array', 'xml_name': 'sameAs', 'element_class': SameAs
         })
     ]
 
 
 class FlexRelatedPropType(FlexProp2Type):
     """
@@ -285,15 +285,15 @@
             'xml_type': 'IRIType',
             'use': 'optional'
         }
     }
 
 
 ConceptRelationshipsGroup = [
-    ('same_as', {
+    ('sameas', {
         'type': 'array', 'xml_name': 'sameAs', 'element_class': SameAs
     }),
     ('broader', {
         'type': 'array', 'xml_name': 'broader', 'element_class': Broader
     }),
     ('narrower', {
         'type': 'array', 'xml_name': 'narrower', 'element_class': Narrower
```

### Comparing `newsmlg2-0.3/NewsMLG2/concepts.py` & `newsmlg2-0.6/NewsMLG2/concepts.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,64 +91,64 @@
     optional attributes
     """
 
     elements = [
         ('bag', {
             'type': 'single', 'xml_name': 'bag', 'element_class': Bag
         }),
-        ('main_concept', {
+        ('mainconcept', {
             'type': 'single', 'xml_name': 'mainConcept',
             'element_class': MainConcept
         }),
-        ('facet_concept', {
+        ('facetconcept', {
             'type': 'array', 'xml_name': 'facetConcept',
             'element_class': FacetConcept
         })
     ]
 
 
 class FlexPersonPropType(CommonPowerAttributes, FlexAttributes, I18NAttributes):
     """
     Flexible person data type for both controlled and uncontrolled values
     """
 
     elements = ConceptDefinitionGroup + ConceptRelationshipsGroup + [
-        ('person_details', {
+        ('persondetails', {
             'type': 'single', 'xml_name': 'personDetails',
             'element_class': 'entities.PersonDetails'
         })
     ]
 
 
 class FlexOrganisationPropType(CommonPowerAttributes, QualifyingAttributes,
     I18NAttributes):
     """
     Flexible organisation data type for both controlled and uncontrolled values
     """
 
     elements = ConceptDefinitionGroup + ConceptRelationshipsGroup + [
-        ('organisation_details', {
+        ('organisationdetails', {
             'type': 'single', 'xml_name': 'organisationDetails',
             'element_class': 'entities.OrganisationDetails'
         })
     ]
 
 
 class FlexPartyPropType(CommonPowerAttributes, FlexAttributes, I18NAttributes,
     QCodeURIMixin):
     """
     Flexible party (person or organisation) PCL-type for both controlled and
     uncontrolled values
     """
     elements = ConceptDefinitionGroup + ConceptRelationshipsGroup + [
-        ('person_details', {
+        ('persondetails', {
             'type': 'single', 'xml_name': 'personDetails',
             'element_class': 'entities.PersonDetails'
         }),
-        ('organisation_details', {
+        ('organisationdetails', {
             'type': 'single', 'xml_name': 'organisationDetails',
             'element_class': 'entities.OrganisationDetails'
         })
     ]
 
 
 class Party(FlexPartyPropType):
@@ -214,15 +214,15 @@
         },
         # The job title of the person who created or enhanced the content in
         # the news provider organisation - expressed by a URI
         'jobtitleuri': {
             'xml_name': 'jobtitleuri',
             'xml_type': 'IRIType',
             'use': 'optional'
-        },
+        }
     }
 
 
 class GeoCoordinatesType(CommonPowerAttributes):
     """
     The type for geographic coordinates (Type defined in this XML Schema only)
     """
@@ -354,38 +354,35 @@
     I18NAttributes):
     """
     Flexible location (geopolitical area of point-of-interest)
     data type for both controlled and uncontrolled values
     """
 
     elements = ConceptDefinitionGroup + ConceptRelationshipsGroup + [
-        ('geo_area_details', {
+        ('geoareadetails', {
             'type': 'single',
             'xml_name': 'geoAreaDetails',
             'element_class': GeoAreaDetails
         }),
-        ('poi_details', {
+        ('poidetails', {
             'type': 'single',
             'xml_name': 'POIDetails',
             'element_class': 'concepts.POIDetails'
         })
     ]
 
-    def __bool__(self):
-        return self.geo_area_details is not None or self.poi_details is not None
-
 
 class FlexPOIPropType(CommonPowerAttributes, FlexAttributes, I18NAttributes):
     """
     Flexible point-of-intrerest data type for both controlled and uncontrolled
     values
     """
 
     elements = ConceptDefinitionGroup + ConceptRelationshipsGroup + [
-        ('poi_details', {
+        ('poidetails', {
             'type': 'single',
             'xml_name': 'POIDetails',
             'element_class': 'concepts.POIDetails'
         })
     ]
 
 
@@ -431,15 +428,15 @@
     I18NAttributes):
     """
     Flexible geopolitical area data type for both controlled and uncontrolled
     values
     """
 
     elements = ConceptDefinitionGroup + ConceptRelationshipsGroup + [
-        ('geo_area_details', {
+        ('geoareadetails', {
             'type': 'single',
             'xml_name': 'geoAreaDetails',
             'element_class': GeoAreaDetails
         })
     ]
 
 
@@ -532,39 +529,42 @@
     """
 
 
 """
 A group of properties to define the details of specific entities
 """
 EntityDetailsGroup = [
+    ('hasinstrument', {
+        'type': 'array', 'xml_name': 'hasInstrument',
+        'element_class': 'entities.HasInstrument'
+    }),
     ('persondetails', {
         'type': 'single', 'xml_name': 'personDetails',
         'element_class': 'entities.PersonDetails'
     }),
-    ('organisationDetails', {
+    ('organisationdetails', {
         'type': 'single', 'xml_name': 'organisationDetails',
         'element_class': 'entities.OrganisationDetails'
     }),
     ('geoareadetails', {
         'type': 'single', 'xml_name': 'geoAreaDetails',
         'element_class': GeoAreaDetails
     }),
     ('poidetails', {
         'type': 'single', 'xml_name': 'POIDetails',
         'element_class': POIDetails
     }),
     ('objectdetails', {
         'type': 'single', 'xml_name': 'objectDetails',
         'element_class': 'entities.ObjectDetails'
+    }),
+    ('eventdetails', {
+        'type': 'single', 'xml_name': 'eventDetails',
+        'element_class': 'events.EventDetails'
     })
-    # TODO
-    # ('eventdetails': {
-    #     'type': 'single', 'xml_name': 'eventDetails',
-    #     'element_class': EventDetails
-    # })
 ]
 
 
 class Concept(CommonPowerAttributes, I18NAttributes):
     """
     A set of properties defining a concept
     """
@@ -592,23 +592,7 @@
         })
     ] + ConceptRelationshipsGroup + EntityDetailsGroup + [
         ('conceptextproperty', {
             'type': 'single', 'xml_name': 'conceptExtProperty',
             'element_class': 'extensionproperties.ConceptExtProperty'
         })
     ]
-
-    def get_conceptid(self):
-        """Return QCode for conceptid."""
-        return self.get_element_value('conceptid').get_qcode()
-
-    def get_conceptid_uri(self):
-        """Return URI for conceptid."""
-        return self.get_element_value('conceptid').get_uri()
-
-    def get_type(self):
-        """Return QCode for type."""
-        return self.get_element_value('type').get_qcode()
-
-    def get_type_uri(self):
-        """Return URI for type."""
-        return self.get_element_value('type').get_uri()
```

### Comparing `newsmlg2-0.3/NewsMLG2/contentmeta.py` & `newsmlg2-0.6/NewsMLG2/contentmeta.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     CommonPowerAttributes, I18NAttributes, MediaContentCharacteristics1,
     RankingAttributes, QuantifyAttributes
 )
 from .concepts import (
     FlexAuthorPropType, FlexLocationPropType, Flex1ConceptPropType,
     Flex1PartyPropType, Flex1PropType
 )
+from .conceptrelationships import FlexPropType
 from .complextypes import IntlStringType, TruncatedDateTimePropType
 from .extensionproperties import Flex2ExtPropType
 from .ids import AltId
 from .labeltypes import BlockType, Label1Type
 from .link import TargetResourceAttributes
 from .simpletypes import Int1to9Type
 
@@ -34,14 +35,19 @@
 
 class ContentModified(TruncatedDateTimePropType):
     """
     The date (and optionally the time) on which the content was last modified.
     """
 
 
+class DigitalSourceType(FlexPropType):
+    """
+    Indicates the source type from which the content was created. The recommended vocabulary is the IPTC Digital Source Type NewsCodes http://cv.iptc.org/newscodes/digitalsourcetype/
+    """
+
 class Icon(TargetResourceAttributes, CommonPowerAttributes,
     MediaContentCharacteristics1):
     """
     An iconic visual identification of the content
     """
     attributes = {
          # Identifies the rendition of the target resource - expressed by
@@ -459,14 +465,19 @@
         'element_class': ContentCreated
     }),
     ('contentmodified', {
         'type': 'single',
         'xml_name': 'contentModified',
         'element_class': ContentModified
     }),
+    ('digitalsourcetype', {
+        'type': 'single',
+        'xml_name': 'digitalSourceType',
+        'element_class': DigitalSourceType
+    }),
     ('located', {
         'type': 'array',
         'xml_name': 'located',
         'element_class': Located
     }),
     ('infosource', {
         'type': 'array',
```

### Comparing `newsmlg2-0.3/NewsMLG2/core.py` & `newsmlg2-0.6/NewsMLG2/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,72 +1,56 @@
+#!/usr/bin/env python
+
 """
-Core functions for NewsMLG2 library.
+Core functions for NewsMLG2 library: base objects for most
+of our XML-based elements. Use magic methods to handle
+property accessors to make processing easier.
 """
 
 import re
 from lxml import etree
 
 from .catalogstore import CATALOG_STORE
 from .utils import import_string
 
+NEWSMLG2_VERSION = '2.34'
 NEWSMLG2_NS = 'http://iptc.org/std/nar/2006-10-01/'
 NEWSMLG2NSPREFIX = '{%s}' % NEWSMLG2_NS
 NITF_NS = 'http://iptc.org/std/NITF/2006-10-18/'
 NITFNSPREFIX= '{%s}' % NITF_NS
 XML_NS = 'http://www.w3.org/XML/1998/namespace'
 XMLNSPREFIX = '{%s}' % XML_NS
 NSMAP = {None : NEWSMLG2_NS, 'xml': XML_NS, 'nitf': NITF_NS}
 
 
 class BaseObject():
     """
     Implements `attributes` and `elements` handlers.
     """
     _attribute_definitions = None
-    _element_definitions = None
     _attribute_values = {}
-    _attribute_types = {}
     _element_values = {}
 
     def get_attribute_definitions(self):
         """
         Load all 'attributes' from any class in the MRO inheritance chain
         """
         if self._attribute_definitions:
             return self._attribute_definitions
         self._attribute_definitions = {}
         for otherclass in reversed(self.__class__.__mro__):
             attrs = vars(otherclass).get('attributes', {})
             self._attribute_definitions.update(attrs)
         return self._attribute_definitions
 
-    def get_attribute_types(self):
-        """
-        Load all 'attribute_types' declared in  any class in the MRO
-        inheritance chain
-        """
-        all_attr_types = {}
-        for otherclass in reversed(self.__class__.__mro__):
-            attr_types = vars(otherclass).get('attribute_types', {})
-            all_attr_types.update(attr_types)
-        return all_attr_types
-
-    def get_attr(self, attr):
-        """
-        Get value of the given XML attribute.
-        """
-        return self._attribute_values.get(attr, None)
-
     def get_element_definitions(self):
         """
         Load all element definitions declared in any class in the MRO
         inheritance chain
         """
-        if self._element_definitions:
-            return self._element_definitions
         self._element_definitions = []
         for otherclass in reversed(self.__class__.__mro__):
             elements = vars(otherclass).get('elements', ())
             self._element_definitions += elements
         return self._element_definitions
 
     def get_element_class(self, element_class):
@@ -89,15 +73,15 @@
         attr_defns = self.get_attribute_definitions()
         element_defns = self.get_element_definitions()
         if 'text' in kwargs:
             self._text = kwargs.get('text')
         if xmlelement is None:
             return
         if not isinstance(xmlelement, etree._Element):
-            raise AttributeError("xmlelement should be an instance of _Element")
+            raise AttributeError("xmlelement should be an instance of _Element. Currently it is a "+str(type(xmlelement)))
         for attribute_id, attribute_definition in attr_defns.items():
             attribute_xmlname = attribute_definition['xml_name']
             xmlattr_value = xmlelement.get(attribute_xmlname)
             if xmlattr_value is not None:
                 self._attribute_values[attribute_id] = xmlattr_value
         for (element_id, element_definition) in element_defns:
             element_class = self.get_element_class(element_definition['element_class'])
@@ -121,50 +105,43 @@
         """
         Return value of the element as read from the XML.
         """
         return self._element_values[item]
 
     def __getattr__(self, name):
         """
-        Default getter for all methods where we don't have a defined method
+        Default getter for all property access operations that don't have a defined method
         """
         if name in self._element_values:
-            return self._element_values[name]
+            return self.get_element_value(name)
         # convert our list of tuples to a dict so we can look up keys
         elemdefndict = dict(self._element_definitions)
         if name in elemdefndict:
-            # no value, but the element exists - create it on the fly!
+            # no value, but the element definition exists - so create an empty object on the fly
             element_definition = elemdefndict[name]
-            # TODO refactor this out - repeated code
             element_class = self.get_element_class(element_definition['element_class'])
-            if element_definition['type'] == 'array':
-                self._element_values[name] = GenericArray(
-                    element_class = element_definition['element_class']
-                )
-            else:
-                self._element_values[name] = element_class()
+            self._element_values[name] = element_class()
             return self._element_values[name]
+
         if name in self._attribute_definitions:
             if name in self._attribute_values:
                 return self._attribute_values[name]
             if 'default' in self._attribute_definitions[name]:
                 return self._attribute_definitions[name]['default']
-            raise AttributeError(
-                "'" + name + "' is a defined attribute of " +
-                "'" + self.__class__.__name__ + "' " +
-                "but has no defined value or default"
-            )
+            # <name> is a defined attribute of the class but
+            # has no defined value or default: return None
+            return None
         raise AttributeError(
             "'" + self.__class__.__name__ +
             "' has no element or attribute '" + name + "'"
         )
 
     def __setattr__(self, name, value):
         """
-        Object setter: this should let us set all NewsMLg2 properties (elements
+        Object setter: this should let us set all NewsML-G2 properties (elements
         and attributes) using Python dot syntax, e.g. "newsitem.version" or
         "newsitem.contentmeta".
         The type of "value" could be anything so we can't validate it unless we
         have defined it in the attribute definition.
         Note that __setattr__ is called for *all* property sets, not just
         when there is no other method, so we need to look for our own properties
         before handling other property names.
@@ -172,41 +149,54 @@
         if name.startswith('_'):
             # it's a property internal to this module, handle it normally
             super().__setattr__(name, value)
             return
         # convert our list of tuples to a dict so we can look up keys
         elemdefndict = dict(self._element_definitions)
         if name in elemdefndict:
+            element_class_name = elemdefndict[name]['element_class']
+            element_class = self.get_element_class(element_class_name)
             if isinstance(value, str):
-                element_class_name = elemdefndict[name]['element_class']
-                element_class = self.get_element_class(element_class_name)
                 self._element_values[name] = element_class(text = value)
+            elif isinstance(value, list):
+                if elemdefndict[name]['type'] == 'array':
+                    self._element_values[name] = GenericArray(
+                        xmlarray = value,
+                        element_class = element_class
+                    )
+                else:
+                    raise AttributeError(
+                            "Trying to assign a list to a non-array element"
+                          )
             else:
                 self._element_values[name] = value
         elif name in self._attribute_definitions:
             self._attribute_values[name] = value
         else:
             raise AttributeError(
                 "'" + self.__class__.__name__ +
                 "' has no element or attribute '" + name + "'"
                   )
 
-
     def __bool__(self):
         if any(self._attribute_values.values()):
             return True
         if [bool(elem) for elem in self._element_values.values()]:
             return True
         if getattr(self, '_text', None):
             return True
         return False
 
     def __str__(self):
-        if hasattr(self, '_text') and self._text is not None:
+        if hasattr(self, '_text') and self._text != '':
             return self._text
+        elif hasattr(self, 'qcode') and self.qcode:
+            return '<'+self.__class__.__name__+' qcode="'+str(self.qcode)+'">'
+        elif hasattr(self, 'uri') and self.uri:
+            return '<'+self.__class__.__name__+' uri="'+str(self.uri)+'">'
         return '<'+self.__class__.__name__+'>'
 
     def to_xml(self):
         """
         Convert the current object to XML representation.
         Any XML generated should conform to the NewsML-G2 schema.
         """
@@ -217,37 +207,32 @@
             xml_element_name = (xml_element_name[0].lower()
                 + xml_element_name[1:])
         elem = etree.Element(NEWSMLG2NSPREFIX+xml_element_name, nsmap=NSMAP)
         if hasattr(self, '_text') and self._text != '':
             elem.text = self._text
         for attr_id, attr_defn in self.get_attribute_definitions().items():
             if attr_id in self._attribute_values:
-                if isinstance(attr_defn, str):
-                    # old style - TODO remove after all attr defns are updated
-                    xml_attr = attr_defn
-                else:
-                    xml_attr = attr_defn['xml_name']
+                xml_attr = attr_defn['xml_name']
                 elem.set(xml_attr, self._attribute_values[attr_id])
-            # only check for new-style attribute definitions
             elif not isinstance(attr_defn, str):
                 if 'default' in attr_defn:
                     attr_xml_name = attr_defn['xml_name']
                     attr_default_value = attr_defn['default']
                     elem.set(attr_xml_name, attr_default_value)
                 elif 'use' in attr_defn and attr_defn['use'] == 'required':
                     raise AttributeError(
                         "Attribute '" + attr_id + "' is required but has no value"
                     )
         for child_element_id, child_element_value in self._element_values.items():
             if child_element_value:
-                child_elem_xml = child_element_value.to_xml()
-                if isinstance(child_elem_xml, list):
-                    for child in child_elem_xml:
-                        elem.append(child)
+                if isinstance(child_element_value, GenericArray):
+                    for arrayelem in child_element_value:
+                        elem.append(arrayelem.to_xml())
                 else:
+                    child_elem_xml = child_element_value.to_xml()
                     elem.append(child_elem_xml)
         return elem
 
 
 class GenericArray():
     """
     Handle arrays of objects.
@@ -257,26 +242,34 @@
     """
     _array_contents = []
     _element_module_name = None
     _element_class_name = None
     _element_class = None
 
     def __init__(self, **kwargs):
-        # super().__init__(**kwargs)
         self._array_contents = []
+        self._iterindex = -1
+
+        # Populate array based on initial args
         xmlarray = kwargs.get('xmlarray')
         if isinstance(xmlarray, (list, etree._Element)):
             if 'element_class' in kwargs:
                 self._element_class = kwargs['element_class']
             else:
                 raise AttributeError("'element_class' is required")
-            for xmlelement in xmlarray:
-                array_elem = self._element_class(xmlelement = xmlelement)
-                self._array_contents.append(array_elem)
-        self._iterindex = -1
+            if isinstance(xmlarray, list):
+                for element in xmlarray:
+                    if isinstance(element, etree._Element):
+                        array_elem = self._element_class(xmlelement = element)
+                        self._array_contents.append(array_elem)
+                    else:
+                        self._array_contents.append(element)
+        else:
+            raise AttributeError("'xmlarray' must be an etree _Element "
+                                 "or a list of objects")
 
     def __iter__(self):
         return self
 
     def __next__(self):
         self._iterindex += 1
         if (self._iterindex >= len(self._array_contents)):
@@ -301,17 +294,17 @@
         Hack / "syntactic sugar": if an array has only one element,
         then requesting str() on the array returns the str() of the
         first element.
         """
         if len(self._array_contents) == 1:
             return str(self._array_contents[0])
         return (
-            '<' + self.__class__.__name__ + 'of ' +
-            len(self._array_contents) + ' ' +
-            self._element_class_name +' objects>'
+            '<' + self.__class__.__name__ + ' of ' +
+            str(len(self._array_contents)) + ' ' +
+            self._element_class.__name__ +' objects>'
         )
 
     def __getattr__(self, name):
         """
         More "syntactic sugar": If a user tries to get a property or call a
         method on the array, and the array only contains one element, then pass
         the call on to the first element in the array.
@@ -324,35 +317,31 @@
         )
 
     def __bool__(self):
         if self._array_contents != []:
             return any(bool(item) for item in self._array_contents)
         return False
 
-    def to_xml(self):
-        xml_array = []
-        for elem in self._array_contents:
-            xml_array.append(elem.to_xml())
-        return xml_array
-
     def get_languages(self):
         """
         For repeating elements with xml:lang attributes,
         this helper function returns all available language codes.
         """
         return [elem.xml_lang for elem in self._array_contents]
 
-    def get_language(self, language):
+    def get_for_language(self, language):
         """
         For repeating elements with xml:lang attributes,
         this helper function finds the correct language version.
         """
         for elem in self._array_contents:
             if elem.xml_lang == language:
-                return str(elem)
+                return elem
+        # If language is not found, returns None - should we
+        # raise an exception?
         return None
 
 
 class QCodeURIMixin(BaseObject):
     """
     Used for any class that has "qcode" and "uri" attributes.
     Up to version 0.2, provided helper methods. Now users should
```

### Comparing `newsmlg2-0.3/NewsMLG2/document.py` & `newsmlg2-0.6/NewsMLG2/document.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 
 from .anyitem import AnyItem
 from .core import NEWSMLG2NSPREFIX
 from .catalogitem import CatalogItem
 from .conceptitem import ConceptItem
 from .knowledgeitem import KnowledgeItem
 from .newsitem import NewsItem
+from .newsmessage import NewsMessage
 from .packageitem import PackageItem
+from .planningitem import PlanningItem
 
 
 class NewsMLG2Document():
     """
-    Parent class to paarse a NewsMLG2 document.
+    Parent class to parse a NewsMLG2 document.
     """
     _root_element = None
     item = None
 
     def __init__(self, filename=None, string=None):
         if isinstance(filename, str):
             tree = etree.parse(filename)
@@ -45,19 +47,25 @@
                 self.item = NewsItem(
                     xmlelement = self._root_element
                 )
             elif self._root_element.tag == NEWSMLG2NSPREFIX+'packageItem':
                 self.item = PackageItem(
                     xmlelement = self._root_element
                 )
+            elif self._root_element.tag == NEWSMLG2NSPREFIX+'planningItem':
+                self.item = PlanningItem(
+                    xmlelement = self._root_element
+                )
+            elif self._root_element.tag == NEWSMLG2NSPREFIX+'newsMessage':
+                self.item = NewsMessage(
+                    xmlelement = self._root_element
+                )
             else:
                 raise Exception(
-                    "Item types other than CatalogItem, ConceptItem, "
-                    "KnowledgeItem, NewsItem and PackageItem are not yet "
-                    "supported."
+                    "Root element is not a NewsML-G2 specified document root."
                 )
 
     def get_item(self):
         """
         Return the main Item object (NewsItem, KnowledgeItem, ConceptItem etc)
         for this document.
         """
@@ -66,15 +74,16 @@
     def set_item(self, item):
         """
         Set the main Item object (NewsItem, KnowledgeItem, ConceptItem etc)
         for this document.
         """
         if not isinstance(item, AnyItem):
             raise Exception(
-                "Item must be an instance of NewsItem or KnowledgeItem"
+                "Item must be an instance of AnyItem (i.e. NewsItem, CatalogItem, "
+                "ConceptItem, KnowledgeItem or PackageItem)"
             )
         self.item = item
 
     def to_xml(self):
         """Return this document in XML form."""
         elem = self.item.to_xml()
         return etree.tostring(
```

### Comparing `newsmlg2-0.3/NewsMLG2/entities.py` & `newsmlg2-0.6/NewsMLG2/entities.py`

 * *Files 3% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         }),
         ('area', {
             'type': 'array', 'xml_name': 'area', 'element_class': Area
         }),
         ('country', {
             'type': 'single', 'xml_name': 'country', 'element_class': Country
         }),
-        ('postal_code', {
+        ('postalcode', {
             'type': 'single', 'xml_name': 'postalCode',
             'element_class': PostalCode
         })
     ]
     attributes = {
         # A refinement of the semantics of the postal address - expressed by
         # a QCode
@@ -266,50 +266,54 @@
     elements = [
         ('born', { 'type': 'single', 'xml_name': 'born', 'element_class': Born }),
         ('died', { 'type': 'single', 'xml_name': 'died', 'element_class': Died }),
         ('affiliation', {
             'type': 'array', 'xml_name': 'affiliation',
             'element_class': PersonAffiliation
         }),
-        ('contact_info', {
+        ('contactinfo', {
             'type': 'array', 'xml_name': 'contactInfo',
             'element_class': ContactInfo
         })
     ]
 
 
 class OrganisationFounded(TruncatedDateTimePropType):
     """
     The date the organisation was founded/established.
     """
+    xml_element_name = 'founded'
 
 
 class OrganisationDissolved(TruncatedDateTimePropType):
     """
     The date the organisation was dissolved.
     """
+    xml_element_name = 'dissolved'
 
 
 class OrganisationLocation(FlexLocationPropType):
     """
     A place where the organisation is located.
     """
+    xml_element_name = 'location'
 
 
 class OrganisationAffiliationType(FlexOrganisationPropType, TimeValidityAttributes):
     """
     The type for an affliation of an organisation to another organisation
     (Type defined in this XML Schema only)
     """
 
 
 class OrganisationAffiliation(OrganisationAffiliationType):
     """
     An affiliation of the organisation with another organisation.
     """
+    xml_element_name = 'affiliation'
 
 
 class HasInstrument(CommonPowerAttributes):
     """
     Defines a financial instrument which is related to a company
     """
     attributes = {
@@ -393,17 +397,19 @@
             'type': 'array', 'xml_name': 'affiliation',
             'element_class': OrganisationAffiliation
         }),
         ('contactinfo', {
             'type': 'array', 'xml_name': 'contactInfo',
             'element_class': ContactInfo
         }),
+        # deprecated in NewsML-G2 2.31 but still allowed
         ('hasinstrument', {
             'type': 'array', 'xml_name': 'hasInstrument',
-            'element_class': HasInstrument
+            'element_class': HasInstrument,
+            'status': 'deprecated'
         })
     ]
 
 
 class ObjectCreated(TruncatedDateTimePropType):
     """
     The date (and optionally the time) on which this object was created
```

### Comparing `newsmlg2-0.3/NewsMLG2/extensionproperties.py` & `newsmlg2-0.6/NewsMLG2/extensionproperties.py`

 * *Files identical despite different names*

### Comparing `newsmlg2-0.3/NewsMLG2/ids.py` & `newsmlg2-0.6/NewsMLG2/ids.py`

 * *Files identical despite different names*

### Comparing `newsmlg2-0.3/NewsMLG2/itemmanagement.py` & `newsmlg2-0.6/NewsMLG2/itemmanagement.py`

 * *Files identical despite different names*

### Comparing `newsmlg2-0.3/NewsMLG2/knowledgeitem.py` & `newsmlg2-0.6/NewsMLG2/knowledgeitem.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 KnowledgeItem - one of the main Item classes in NewsML-G2
 """
 
 from .anyitem import (
     AnyItem, Assert, DerivedFrom, DerivedFromValue, InlineRef
 )
 from .attributegroups import (
-    CommonPowerAttributes
+    AuthorityAttributes, CommonPowerAttributes
 )
 from .catalog import SameAsScheme
 from .complextypes import Name
 from .concepts import Concept, Definition, Note
 from .extensionproperties import Flex2ExtPropType
 from .conceptrelationships import Related
 from .contentmeta import ContentMetadataAcDType
@@ -21,15 +21,18 @@
 
 class ConceptSet(CommonPowerAttributes):
     """
     An unordered set of concepts
     """
 
     elements = [
-        ('concept', { 'type': 'array', 'xml_name': 'concept', 'element_class': Concept })
+        ('concept', {
+            'type': 'array', 'xml_name': 'concept',
+            'element_class': Concept
+        })
     ]
 
 
 class SchemeMetaExtPropertyElement(Flex2ExtPropType):
     """
     Extension Property; the semantics are defined by the concept referenced by
     the rel attribute. The semantics of the Extension Property must have the
@@ -40,32 +43,39 @@
 class SchemeMetaExtProperty(Flex2ExtPropType):
     """
     Array of SchemeMetaExtProperty objects.
     """
     element_class = SchemeMetaExtPropertyElement
 
 
-class SchemeMeta(CommonPowerAttributes):
+class SchemeMeta(AuthorityAttributes, CommonPowerAttributes):
     """
     Metadata about a scheme conveyed by a Knowledge Item
     """
 
     elements = [
         ('sameasscheme', {
             'type': 'array', 'xml_name': 'sameAsScheme',
             'element_class': SameAsScheme
         }),
-        ('name', { 'type': 'array', 'xml_name': 'name', 'element_class': Name }),
+        ('name', {
+            'type': 'array', 'xml_name': 'name',
+            'element_class': Name
+        }),
         ('definition', {
             'type': 'array', 'xml_name': 'definition',
             'element_class': Definition
         }),
-        ('note', { 'type': 'array', 'xml_name': 'note', 'element_class': Note }),
+        ('note', {
+            'type': 'array', 'xml_name': 'note',
+            'element_class': Note
+        }),
         ('related', {
-            'type': 'array', 'xml_name': 'related', 'element_class': Related
+            'type': 'array', 'xml_name': 'related',
+            'element_class': Related
         }),
         ('schememetaextproperty', {
             'type': 'array', 'xml_name': 'schemeMetaExtProperty',
             'element_class': SchemeMetaExtProperty
         })
     ]
     attributes = {
@@ -75,19 +85,14 @@
             'xml_type': 'IRIType',
             'use': 'required'
         },
         # The alias preferred by the schema authority
         'preferredalias': {
             'xml_name': 'preferredalias'
         },
-        # Defines the authority controlling the scheme
-        'authority': {
-            'xml_name': 'authority',
-            'xml_type': 'IRIType'
-        },
         # List of all concept types used within this Knowledge Item
         'concepttype': {
             'xml_name': 'concepttype',
             'xml_type': 'QCodeListType'
         },
         # The date (and, optionally, the time) when the scheme was created.
         # This must not be later than the creation timestamp of any concepts in
```

### Comparing `newsmlg2-0.3/NewsMLG2/labeltypes.py` & `newsmlg2-0.6/NewsMLG2/labeltypes.py`

 * *Files identical despite different names*

### Comparing `newsmlg2-0.3/NewsMLG2/link.py` & `newsmlg2-0.6/NewsMLG2/link.py`

 * *Files 13% similar despite different names*

```diff
@@ -153,47 +153,14 @@
         'rank': {
             'xml_name': 'rank',
             'xml_type': 'xs:nonNegativeInteger',
             'use': 'optional'
         }
     }
 
-    def get_rel(self):
-        """
-        Return the value of this property as a qcode
-        TODO - make this generic in BaseObject
-        """
-        qcode = self.get_attr('rel')
-        if qcode is not None:
-            return qcode
-        # convert URI to qcode:
-        uri = self.get_attr('reluri')
-        urimainpart, code = uri.rsplit('/', 1)
-        # get catalog
-        scheme = CATALOG_STORE.get_scheme_for_uri(urimainpart)
-        # look up catalog for URI, get prefix
-        alias = scheme.alias
-        return alias + ':' + code
-
-    def get_rel_uri(self):
-        """
-        Return the value of this property as a URI
-        """
-        uri = self.get_attr('reluri')
-        if uri:
-            return uri
-        # convert qcode to URI:
-        qcode = self.get_attr('rel')
-        alias, code = qcode.split(':')
-        # get catalog
-        scheme = CATALOG_STORE.get_scheme_for_alias(alias)
-        # look up catalog for alias, get URI
-        uri = scheme.uri
-        return uri + code
-
 
 class Link(Link1Type):
     """
     A link from the current Item to a target Item or Web resource
     """
```

### Comparing `newsmlg2-0.3/NewsMLG2/newsitem.py` & `newsmlg2-0.6/NewsMLG2/newsitem.py`

 * *Files identical despite different names*

### Comparing `newsmlg2-0.3/NewsMLG2/packageitem.py` & `newsmlg2-0.6/NewsMLG2/packageitem.py`

 * *Files identical despite different names*

### Comparing `newsmlg2-0.3/NewsMLG2/partmeta.py` & `newsmlg2-0.6/NewsMLG2/partmeta.py`

 * *Files identical despite different names*

### Comparing `newsmlg2-0.3/NewsMLG2/rights.py` & `newsmlg2-0.6/NewsMLG2/rights.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Elements for handling rights management
 """
 
 from .attributegroups import (
     CommonPowerAttributes, I18NAttributes, TimeValidityAttributes
 )
 from .concepts import FlexPartyPropType, FlexPersonPropType
+from .conceptrelationships import FlexPropType
 from .extensionproperties import Flex2ExtPropType
 from .labeltypes import BlockType
 from .link import Link
 
 
 class RightsBlockType(BlockType):
     """
@@ -90,14 +91,20 @@
             'xml_name': 'enctype',
             'xml_type': 'xs:string',
             'use': 'required'
         }
     }
 
 
+class DataMining(FlexPropType):
+    """
+    Data mining prohibition or permission, optionally with constraints
+    """
+
+
 class RightsInfo(CommonPowerAttributes, I18NAttributes, TimeValidityAttributes):
     """
     A set of properties representing the rights associated with the Item
     """
     attributes = {
         # Reference(s) to the part(s) of an Item to which the rightsInfo element
         # applies. When referencing part(s) of the content of an Item, idrefs
@@ -176,9 +183,13 @@
         ('rightsexpressionxml', {
             'type': 'array', 'xml_name': 'rightsExpressionXML',
             'element_class': RightsExpressionXML
         }),
         ('rightsexpressiondata', {
             'type': 'array', 'xml_name': 'rightsExpressionData',
             'element_class': RightsExpressionData
+        }),
+        ('datamining', {
+            'type': 'single', 'xml_name': 'dataMining',
+            'element_class': DataMining
         })
     ]
```

### Comparing `newsmlg2-0.3/NewsMLG2/simpletypes.py` & `newsmlg2-0.6/NewsMLG2/simpletypes.py`

 * *Files identical despite different names*

### Comparing `newsmlg2-0.3/NewsMLG2/utils.py` & `newsmlg2-0.6/NewsMLG2/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,19 +11,15 @@
     Import a dotted module path and return the attribute/class designated by the
     last name in the path. Raise ImportError if the import failed.
 
     Copied from Django source code:
     https://github.com/django/django/blob/main/django/utils/module_loading.py
     """
     dotted_path = "NewsMLG2." + dotted_path
-    try:
-        module_path, class_name = dotted_path.rsplit('.', 1)
-    except ValueError as err:
-        raise ImportError("%s doesn't look like a module path" % dotted_path) from err
-
+    module_path, class_name = dotted_path.rsplit('.', 1)
     module = import_module(module_path)
 
     try:
         return getattr(module, class_name)
     except AttributeError as err:
         raise ImportError('Module "%s" does not define a "%s" attribute/class' % (
             module_path, class_name)
```

### Comparing `newsmlg2-0.3/newsmlg2.egg-info/SOURCES.txt` & `newsmlg2-0.6/newsmlg2.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -12,30 +12,38 @@
 NewsMLG2/conceptitem.py
 NewsMLG2/conceptrelationships.py
 NewsMLG2/concepts.py
 NewsMLG2/contentmeta.py
 NewsMLG2/core.py
 NewsMLG2/document.py
 NewsMLG2/entities.py
+NewsMLG2/events.py
 NewsMLG2/extensionproperties.py
 NewsMLG2/ids.py
 NewsMLG2/itemmanagement.py
 NewsMLG2/knowledgeitem.py
 NewsMLG2/labeltypes.py
 NewsMLG2/link.py
 NewsMLG2/newsitem.py
+NewsMLG2/newsmessage.py
 NewsMLG2/packageitem.py
 NewsMLG2/partmeta.py
+NewsMLG2/planningitem.py
 NewsMLG2/rights.py
 NewsMLG2/simpletypes.py
 NewsMLG2/utils.py
 newsmlg2.egg-info/PKG-INFO
 newsmlg2.egg-info/SOURCES.txt
 newsmlg2.egg-info/dependency_links.txt
 newsmlg2.egg-info/requires.txt
 newsmlg2.egg-info/top_level.txt
 tests/__init__.py
+tests/test_autoloader.py
 tests/test_catalogitems.py
 tests/test_conceptitems.py
+tests/test_core.py
+tests/test_events.py
 tests/test_knowledgeitems.py
 tests/test_newsitems.py
-tests/test_packageitems.py
+tests/test_newsmessage.py
+tests/test_packageitems.py
+tests/test_planningitems.py
```

### Comparing `newsmlg2-0.3/setup.py` & `newsmlg2-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-VERSION = '0.3'
+VERSION = '0.6'
 
 setup(
   name = 'newsmlg2',
   packages = find_packages(exclude=['contrib', 'docs']),
   version = VERSION,
   description = 'Python implementation of the NewsML-G2 standard (https://iptc.org/standards/newsml-g2/)',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'Brendan Quinn',
   author_email = 'office@iptc.org',
   url = 'https://github.com/iptc/python-newsmlg2',
   download_url = 'https://github.com/iptc/python-newsmlg2/archive/v'+VERSION+'.tar.gz',
   keywords = ['api', 'media', 'publishing', 'news', 'syndication'],
   classifiers = [
-    'Development Status :: 3 - Alpha',
+    'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
   ],
   install_requires=[
     'lxml',
   ],
```

### Comparing `newsmlg2-0.3/tests/test_catalogitems.py` & `newsmlg2-0.6/tests/test_catalogitems.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,19 +43,19 @@
     def test_parse_from_string(self):
         # LISTING_13 example
         test_newsmlg2_string = b"""<?xml version="1.0" encoding="UTF-8"?>
 <catalogItem
     xmlns="http://iptc.org/std/nar/2006-10-01/"
     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
     xsi:schemaLocation="http://iptc.org/std/nar/2006-10-01/
-        ./NewsML-G2_2.29-spec-All-Power.xsd"
+        ./NewsML-G2_2.34-spec-All-Power.xsd"
     guid="urn:newsml:iptc.org:20130517:catalog"
     version="31"
     standard="NewsML-G2"
-    standardversion="2.29"
+    standardversion="2.34"
     conformance="power"
     xml:lang="en-GB">
     <catalogRef
         href="http://www.iptc.org/std/catalog/catalog.IPTC-G2-Standards_36.xml" />
     <rightsInfo>
         <copyrightHolder uri="http://www.iptc.org">
             <name>IPTC</name>
@@ -87,15 +87,15 @@
 </catalogItem>
 """
         g2doc = NewsMLG2.NewsMLG2Document(string=test_newsmlg2_string)
 
         catitem = g2doc.get_item()
         assert catitem.guid == 'urn:newsml:iptc.org:20130517:catalog'
         assert catitem.standard == 'NewsML-G2'
-        assert catitem.standardversion == '2.29'
+        assert catitem.standardversion == '2.34'
         assert catitem.conformance == 'power'
         assert catitem.version == '31'
 
         catalogs = catitem.get_catalogs()
         # catalogs should work the same as for news items.
         test_scheme = catalogs.get_scheme_for_alias('prov')
         assert test_scheme.uri == 'http://cv.iptc.org/newscodes/provider/'
@@ -124,24 +124,23 @@
 class TestNewsMLG2CatalogItemFiles(unittest.TestCase):
     def test_from_file(self):
         test_newsmlg2_file = os.path.join('tests', 'test_files', 'LISTING_13_Complete_Catalog_Item.xml')
         g2doc = NewsMLG2.NewsMLG2Document(filename=test_newsmlg2_file)
         catitem = g2doc.get_item()
         assert catitem.guid == 'urn:newsml:iptc.org:20130517:catalog'
         assert catitem.standard == 'NewsML-G2'
-        assert catitem.standardversion == '2.29'
+        assert catitem.standardversion == '2.34'
         assert catitem.conformance == 'power'
         assert catitem.version == '31'
 
         catalogs = catitem.get_catalogs()
         # catalogs should work the same as for news items.
         test_scheme = catalogs.get_scheme_for_alias('prov')
         assert test_scheme.uri == 'http://cv.iptc.org/newscodes/provider/'
-        # the listing refers to catalog v32 which doesn't have authority elements
-        # assert test_scheme.authority == 'https://iptc.org/'
+        assert test_scheme.authority == 'https://iptc.org/'
         assert test_scheme.modified == '2019-09-13T12:00:00+00:00'
         assert str(test_scheme.definition) == 'Indicates a company, publication or service provider.'
 
         itemmeta = catitem.itemmeta
         assert itemmeta.itemclass.qcode == 'catinat:catalog'
         assert NewsMLG2.qcode_to_uri(itemmeta.itemclass.qcode) == 'http://cv.iptc.org/newscodes/catinature/catalog'
         assert itemmeta.provider.qcode == 'nprov:IPTC'
```

### Comparing `newsmlg2-0.3/tests/test_knowledgeitems.py` & `newsmlg2-0.6/tests/test_knowledgeitems.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 XML_NS = '{http://www.w3.org/XML/1998/namespace}'
 
 class TestNewsMLG2KnowledgeItems(unittest.TestCase):
 
     def test_parse_from_string(self):
         test_newsmlg2_string = b"""<?xml version="1.0" encoding="UTF-8"?>
-<knowledgeItem xmlns="http://iptc.org/std/nar/2006-10-01/" standard="NewsML-G2" standardversion="2.29" conformance="power" guid="urn:newsml:iptc.org:20080229:srcncdki-medtop-TS201901110952144" version="1">
+<knowledgeItem xmlns="http://iptc.org/std/nar/2006-10-01/" standard="NewsML-G2" standardversion="2.34" conformance="power" guid="urn:newsml:iptc.org:20080229:srcncdki-medtop-TS201901110952144" version="1">
   <catalogRef href="http://www.iptc.org/std/catalog/catalog.IPTC-G2-Standards_36.xml"/>
   <rightsInfo>
     <copyrightHolder uri="http://cv.iptc.org/newscodes/newsprovider/IPTC">
       <name>IPTC - International Press Telecommunications Council</name>
     </copyrightHolder>
     <copyrightNotice>Copyright 2021, IPTC, www.iptc.org, Rights Reserved</copyrightNotice>
     <usageTerms href="http://creativecommons.org/licenses/by/4.0/">the Creative Commons Attribution (CC BY) 4.0 licence applies to all NewsCodes</usageTerms>
@@ -100,15 +100,15 @@
 </knowledgeItem>
 """
         g2doc = NewsMLG2.NewsMLG2Document(string=test_newsmlg2_string)
 
         knowlitem = g2doc.get_item()
         assert knowlitem.guid == 'urn:newsml:iptc.org:20080229:srcncdki-medtop-TS201901110952144'
         assert knowlitem.standard == 'NewsML-G2'
-        assert knowlitem.standardversion == '2.29'
+        assert knowlitem.standardversion == '2.34'
         assert knowlitem.conformance == 'power'
         assert knowlitem.version == '1'
 
         catalogs = knowlitem.get_catalogs()
         # catalogs should work the same as for news items.
         test_scheme = catalogs.get_scheme_for_alias('prov')
         assert test_scheme.uri == 'http://cv.iptc.org/newscodes/provider/'
@@ -123,42 +123,42 @@
         assert NewsMLG2.uri_to_qcode(itemmeta.provider.uri) == 'nprov:IPTC'
         assert str(itemmeta.versioncreated) == '2021-05-05T12:00:00+00:00'
 
         conceptset = knowlitem.conceptset
         assert conceptset.concept[0].id == 'nprovACCESSWIRE'
         assert conceptset.concept[0].modified == '2021-02-09T12:00:00+00:00'
         assert conceptset.concept[0].conceptid.qcode == 'nprov:ACCESSWIRE'
-        assert conceptset.concept[0].get_conceptid() == 'nprov:ACCESSWIRE'
-        assert conceptset.concept[0].get_conceptid_uri() == 'http://cv.iptc.org/newscodes/newsprovider/ACCESSWIRE'
+        assert NewsMLG2.qcode_to_uri(conceptset.concept[0].conceptid.qcode) == 'http://cv.iptc.org/newscodes/newsprovider/ACCESSWIRE'
         assert conceptset.concept[0].conceptid.created == '2021-02-09T12:00:00+00:00'
         assert conceptset.concept[0].type.qcode == 'cpnat:abstract'
-        assert conceptset.concept[0].get_type() == 'cpnat:abstract'
-        assert conceptset.concept[0].get_type_uri() == 'http://cv.iptc.org/newscodes/cpnature/abstract'
+        assert NewsMLG2.qcode_to_uri(conceptset.concept[0].type.qcode) == 'http://cv.iptc.org/newscodes/cpnature/abstract'
         assert str(conceptset.concept[0].name) == 'ACCESSWIRE'
-        assert conceptset.concept[0].name[0].get_attr('xml_lang') == 'en-GB'
+        assert conceptset.concept[0].name[0].xml_lang == 'en-GB'
         assert conceptset.concept[0].related.uri == 'http://cv.iptc.org/newscodes/newsprovider/'
         assert conceptset.concept[0].related.rel == 'skos:inScheme'
 
-        """ TODO concept[1]:
-        <concept id="nprovAFP" modified="2008-07-02T12:00:00+00:00">
-          <conceptId qcode="nprov:AFP" created="2008-07-02T12:00:00+00:00"/>
-          <type qcode="cpnat:abstract"/>
-          <name xml:lang="en-GB">Agence France-Presse</name>
-          <related uri="http://cv.iptc.org/newscodes/newsprovider/" rel="skos:inScheme"/>
-        </concept>
-        """
+        assert conceptset.concept[1].id == 'nprovAFP'
+        assert conceptset.concept[1].modified == '2008-07-02T12:00:00+00:00'
+        assert conceptset.concept[1].conceptid.qcode == 'nprov:AFP'
+        assert conceptset.concept[1].modified == '2008-07-02T12:00:00+00:00'
+        assert conceptset.concept[1].type.qcode == 'cpnat:abstract'
+        assert conceptset.concept[1].name[0].xml_lang == 'en-GB'
+        assert str(conceptset.concept[1].name[0]) == 'Agence France-Presse'
+        assert conceptset.concept[1].related.uri == 'http://cv.iptc.org/newscodes/newsprovider/'
+        assert conceptset.concept[1].related.rel == 'skos:inScheme'
+
 
 class TestNewsMLG2Files(unittest.TestCase):
     def test_from_file(self):
         test_newsmlg2_file = os.path.join('tests', 'test_files', '002_knowledgeitem.xml')
         g2doc = NewsMLG2.NewsMLG2Document(filename=test_newsmlg2_file)
         knowledgeitem = g2doc.get_item()
         assert knowledgeitem.guid == 'urn:newsml:iptc.org:20080229:srcncdki-nprov-TS202102091406532'
         assert knowledgeitem.standard == 'NewsML-G2'
-        assert knowledgeitem.standardversion == '2.29'
+        assert knowledgeitem.standardversion == '2.34'
         assert knowledgeitem.conformance == 'power'
 
         # catalog tests
         catalogs = knowledgeitem.get_catalogs()
         test_scheme = catalogs.get_scheme_for_alias('nprov')
 
         assert test_scheme.uri == 'http://cv.iptc.org/newscodes/newsprovider/'
```

### Comparing `newsmlg2-0.3/tests/test_packageitems.py` & `newsmlg2-0.6/tests/test_packageitems.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 
     def test_parse_from_string(self):
         test_newsmlg2_string = """<?xml version="1.0" encoding="UTF-8"?>
 <packageItem
     xmlns="http://iptc.org/std/nar/2006-10-01/"
     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
     xsi:schemaLocation="http://iptc.org/std/nar/2006-10-01/
-        ./NewsML-G2_2.29-spec-All-Power.xsd"
+        ./NewsML-G2_2.34-spec-All-Power.xsd"
      standard="NewsML-G2"
-    standardversion="2.29"
+    standardversion="2.34"
     conformance="power"
     guid="tag:example.com,2008:UK-NEWS-TOPTEN:UK20081220098658" version="11">
     <catalogRef
         href="http://www.iptc.org/std/catalog/catalog.IPTC-G2-Standards_36.xml" />
     <catalogRef
         href="http:/www.example.com/customer/cv/catalog4customers-1.xml" />
     <itemMeta>
@@ -113,15 +113,15 @@
 </packageItem>""".encode('utf-8')
 
         g2doc = NewsMLG2.NewsMLG2Document(string=test_newsmlg2_string)
 
         packageitem = g2doc.get_item()
         assert packageitem.guid == 'tag:example.com,2008:UK-NEWS-TOPTEN:UK20081220098658'
         assert packageitem.standard == 'NewsML-G2'
-        assert packageitem.standardversion == '2.29'
+        assert packageitem.standardversion == '2.34'
         assert packageitem.conformance == 'power'
         assert packageitem.version == '11'
 
         catalogs = packageitem.get_catalogs()
         # catalogs should work the same as for news items.
         test_scheme = catalogs.get_scheme_for_alias('prov')
         assert test_scheme.uri == 'http://cv.iptc.org/newscodes/provider/'
@@ -190,15 +190,15 @@
 class TestNewsMLG2Files(unittest.TestCase):
     def test_from_file(self):
         test_newsmlg2_file = os.path.join('tests', 'test_files', 'LISTING_6_Simple_NewsML-G2_Package.xml')
         g2doc = NewsMLG2.NewsMLG2Document(filename=test_newsmlg2_file)
         packageitem = g2doc.get_item()
         assert packageitem.guid == 'tag:example.com,2008:UK-NEWS-TOPTEN:UK20081220098658'
         assert packageitem.standard == 'NewsML-G2'
-        assert packageitem.standardversion == '2.29'
+        assert packageitem.standardversion == '2.34'
         assert packageitem.conformance == 'power'
         assert packageitem.version == '11'
 
         catalogs = packageitem.get_catalogs()
         # catalogs should work the same as for news items.
         test_scheme = catalogs.get_scheme_for_alias('prov')
         assert test_scheme.uri == 'http://cv.iptc.org/newscodes/provider/'
```

