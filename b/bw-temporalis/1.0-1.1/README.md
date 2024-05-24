# Comparing `tmp/bw_temporalis-1.0.tar.gz` & `tmp/bw_temporalis-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_temporalis-1.0.tar", last modified: Thu May 23 19:01:18 2024, max compression
+gzip compressed data, was "bw_temporalis-1.1.tar", last modified: Fri May 24 02:18:39 2024, max compression
```

## Comparing `bw_temporalis-1.0.tar` & `bw_temporalis-1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-23 19:01:18.746003 bw_temporalis-1.0/
--rw-r--r--   0 cmutel     (501) staff       (20)     1456 2024-05-23 18:50:52.000000 bw_temporalis-1.0/LICENSE
--rw-r--r--   0 cmutel     (501) staff       (20)       30 2024-05-23 18:50:52.000000 bw_temporalis-1.0/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     4650 2024-05-23 19:01:18.745933 bw_temporalis-1.0/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     3063 2024-05-23 18:50:52.000000 bw_temporalis-1.0/README.md
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-23 19:01:18.740279 bw_temporalis-1.0/bw_temporalis/
--rw-r--r--   0 cmutel     (501) staff       (20)        4 2024-05-23 18:59:19.000000 bw_temporalis-1.0/bw_temporalis/VERSION
--rw-r--r--   0 cmutel     (501) staff       (20)      902 2024-05-23 18:50:52.000000 bw_temporalis-1.0/bw_temporalis/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3287 2024-05-23 18:50:52.000000 bw_temporalis-1.0/bw_temporalis/convolution.py
--rw-r--r--   0 cmutel     (501) staff       (20)    12579 2024-05-23 18:50:52.000000 bw_temporalis-1.0/bw_temporalis/lca.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-23 19:01:18.739104 bw_temporalis-1.0/bw_temporalis/lcia/
--rw-r--r--   0 cmutel     (501) staff       (20)       60 2024-05-23 18:50:52.000000 bw_temporalis-1.0/bw_temporalis/lcia/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4752 2024-05-23 18:50:52.000000 bw_temporalis-1.0/bw_temporalis/lcia/climate.py
--rw-r--r--   0 cmutel     (501) staff       (20)    16890 2024-05-23 18:51:42.000000 bw_temporalis-1.0/bw_temporalis/temporal_distribution.py
--rw-r--r--   0 cmutel     (501) staff       (20)    10634 2024-05-23 18:50:52.000000 bw_temporalis-1.0/bw_temporalis/timeline.py
--rw-r--r--   0 cmutel     (501) staff       (20)     9398 2024-05-23 18:50:52.000000 bw_temporalis-1.0/bw_temporalis/utils.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-23 19:01:18.743225 bw_temporalis-1.0/bw_temporalis.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)     4650 2024-05-23 19:01:18.000000 bw_temporalis-1.0/bw_temporalis.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)      876 2024-05-23 19:01:18.000000 bw_temporalis-1.0/bw_temporalis.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2024-05-23 19:01:18.000000 bw_temporalis-1.0/bw_temporalis.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2024-05-23 18:51:54.000000 bw_temporalis-1.0/bw_temporalis.egg-info/not-zip-safe
--rw-r--r--   0 cmutel     (501) staff       (20)      174 2024-05-23 19:01:18.000000 bw_temporalis-1.0/bw_temporalis.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       37 2024-05-23 19:01:18.000000 bw_temporalis-1.0/bw_temporalis.egg-info/top_level.txt
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-23 19:01:18.739353 bw_temporalis-1.0/docs/
--rw-r--r--   0 cmutel     (501) staff       (20)     2872 2024-05-23 18:50:52.000000 bw_temporalis-1.0/docs/conf.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-23 19:01:18.739915 bw_temporalis-1.0/examples/
--rw-r--r--   0 cmutel     (501) staff       (20)     1500 2024-05-23 18:50:52.000000 bw_temporalis-1.0/examples/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4350 2024-05-23 18:50:52.000000 bw_temporalis-1.0/examples/ia.py
--rw-r--r--   0 cmutel     (501) staff       (20)     6149 2024-05-23 18:50:52.000000 bw_temporalis-1.0/examples/inv.py
--rw-r--r--   0 cmutel     (501) staff       (20)       87 2024-05-23 18:50:52.000000 bw_temporalis-1.0/pyproject.toml
--rw-r--r--   0 cmutel     (501) staff       (20)     1754 2024-05-23 19:01:18.746322 bw_temporalis-1.0/setup.cfg
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-23 19:01:18.742972 bw_temporalis-1.0/tests/
--rw-r--r--   0 cmutel     (501) staff       (20)     8786 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_convolution.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3247 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_fixed_td.py
--rw-r--r--   0 cmutel     (501) staff       (20)     6094 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_fixed_time_of_year.py
--rw-r--r--   0 cmutel     (501) staff       (20)     8567 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_fixtures.py
--rw-r--r--   0 cmutel     (501) staff       (20)    13408 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_lca.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4104 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_patched_matrix_lca.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4074 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_serialization.py
--rw-r--r--   0 cmutel     (501) staff       (20)     5976 2024-05-23 18:55:54.000000 bw_temporalis-1.0/tests/test_td.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2948 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_tdaware.py
--rw-r--r--   0 cmutel     (501) staff       (20)     8635 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_timeline.py
--rw-r--r--   0 cmutel     (501) staff       (20)    13941 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_utils.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-24 02:18:39.693283 bw_temporalis-1.1/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1456 2024-05-23 18:50:52.000000 bw_temporalis-1.1/LICENSE
+-rw-r--r--   0 cmutel     (501) staff       (20)       30 2024-05-23 18:50:52.000000 bw_temporalis-1.1/MANIFEST.in
+-rw-r--r--   0 cmutel     (501) staff       (20)     4650 2024-05-24 02:18:39.693227 bw_temporalis-1.1/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     3063 2024-05-23 18:50:52.000000 bw_temporalis-1.1/README.md
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-24 02:18:39.688609 bw_temporalis-1.1/bw_temporalis/
+-rw-r--r--   0 cmutel     (501) staff       (20)        4 2024-05-24 01:57:04.000000 bw_temporalis-1.1/bw_temporalis/VERSION
+-rw-r--r--   0 cmutel     (501) staff       (20)      902 2024-05-23 18:50:52.000000 bw_temporalis-1.1/bw_temporalis/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3287 2024-05-23 18:50:52.000000 bw_temporalis-1.1/bw_temporalis/convolution.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    12804 2024-05-24 01:52:52.000000 bw_temporalis-1.1/bw_temporalis/lca.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-24 02:18:39.687487 bw_temporalis-1.1/bw_temporalis/lcia/
+-rw-r--r--   0 cmutel     (501) staff       (20)       60 2024-05-23 18:50:52.000000 bw_temporalis-1.1/bw_temporalis/lcia/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4752 2024-05-23 18:50:52.000000 bw_temporalis-1.1/bw_temporalis/lcia/climate.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    16890 2024-05-23 18:51:42.000000 bw_temporalis-1.1/bw_temporalis/temporal_distribution.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    10634 2024-05-23 18:50:52.000000 bw_temporalis-1.1/bw_temporalis/timeline.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     9398 2024-05-23 18:50:52.000000 bw_temporalis-1.1/bw_temporalis/utils.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-24 02:18:39.692646 bw_temporalis-1.1/bw_temporalis.egg-info/
+-rw-r--r--   0 cmutel     (501) staff       (20)     4650 2024-05-24 02:18:39.000000 bw_temporalis-1.1/bw_temporalis.egg-info/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)      876 2024-05-24 02:18:39.000000 bw_temporalis-1.1/bw_temporalis.egg-info/SOURCES.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2024-05-24 02:18:39.000000 bw_temporalis-1.1/bw_temporalis.egg-info/dependency_links.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2024-05-23 18:51:54.000000 bw_temporalis-1.1/bw_temporalis.egg-info/not-zip-safe
+-rw-r--r--   0 cmutel     (501) staff       (20)      174 2024-05-24 02:18:39.000000 bw_temporalis-1.1/bw_temporalis.egg-info/requires.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       37 2024-05-24 02:18:39.000000 bw_temporalis-1.1/bw_temporalis.egg-info/top_level.txt
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-24 02:18:39.687747 bw_temporalis-1.1/docs/
+-rw-r--r--   0 cmutel     (501) staff       (20)     2872 2024-05-23 18:50:52.000000 bw_temporalis-1.1/docs/conf.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-24 02:18:39.688351 bw_temporalis-1.1/examples/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1522 2024-05-24 01:41:50.000000 bw_temporalis-1.1/examples/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4402 2024-05-24 01:41:50.000000 bw_temporalis-1.1/examples/ia.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     6125 2024-05-24 01:41:50.000000 bw_temporalis-1.1/examples/inv.py
+-rw-r--r--   0 cmutel     (501) staff       (20)       87 2024-05-23 18:50:52.000000 bw_temporalis-1.1/pyproject.toml
+-rw-r--r--   0 cmutel     (501) staff       (20)     1754 2024-05-24 02:18:39.693602 bw_temporalis-1.1/setup.cfg
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-24 02:18:39.692247 bw_temporalis-1.1/tests/
+-rw-r--r--   0 cmutel     (501) staff       (20)     8786 2024-05-23 18:50:52.000000 bw_temporalis-1.1/tests/test_convolution.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3247 2024-05-23 18:50:52.000000 bw_temporalis-1.1/tests/test_fixed_td.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     6094 2024-05-23 18:50:52.000000 bw_temporalis-1.1/tests/test_fixed_time_of_year.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     8567 2024-05-23 18:50:52.000000 bw_temporalis-1.1/tests/test_fixtures.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    16743 2024-05-24 01:52:04.000000 bw_temporalis-1.1/tests/test_lca.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4104 2024-05-23 18:50:52.000000 bw_temporalis-1.1/tests/test_patched_matrix_lca.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4074 2024-05-23 18:50:52.000000 bw_temporalis-1.1/tests/test_serialization.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     5976 2024-05-23 18:55:54.000000 bw_temporalis-1.1/tests/test_td.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2948 2024-05-23 18:50:52.000000 bw_temporalis-1.1/tests/test_tdaware.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     8635 2024-05-23 18:50:52.000000 bw_temporalis-1.1/tests/test_timeline.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    13941 2024-05-23 18:50:52.000000 bw_temporalis-1.1/tests/test_utils.py
```

### Comparing `bw_temporalis-1.0/LICENSE` & `bw_temporalis-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/PKG-INFO` & `bw_temporalis-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_temporalis
-Version: 1.0
+Version: 1.1
 Summary: Revision of bw2temporalis for modern Brightway
 Home-page: https://github.com/brightway-lca/bw_temporalis
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
```

### Comparing `bw_temporalis-1.0/README.md` & `bw_temporalis-1.1/README.md`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/bw_temporalis/__init__.py` & `bw_temporalis-1.1/bw_temporalis/__init__.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/bw_temporalis/convolution.py` & `bw_temporalis-1.1/bw_temporalis/convolution.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/bw_temporalis/lca.py` & `bw_temporalis-1.1/bw_temporalis/lca.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     cutoff : float
         The fraction of the total score below which graph traversal should stop. In range `(0, 1)`.
     biosphere_cutoff : float
         The fraction of the total score below which we don't include separate biosphere nodes to be characterized in the `Timeline`. In range `(0, 1)`.
     max_calc : int
         Total number of LCA inventory calculations to perform during graph traversal
     static_activity_indices : set[int]
-        Activity `id` values where graph traversal will stop
+        Activity database node `id` values where graph traversal will stop
     skip_coproducts : bool
         Should we also traverse edges for the other products in multioutput activities?
     functional_unit_unique_id : int
         The unique id of the functional unit. Strongly recommended to leave as default.
     graph_traversal : bw_graph_tools.NewNodeEachVisitGraphTraversal
         Optional subclass of `NewNodeEachVisitGraphTraversal` for advanced usage
 
@@ -77,37 +77,43 @@
 
     def __init__(
         self,
         lca_object: LCA,
         starting_datetime: datetime | str = "now",
         cutoff: float | None = 5e-4,
         biosphere_cutoff: float | None = 1e-6,
-        max_calc: int | None = 2e3,
-        static_activity_indices: set[int] | None = set(),
+        max_calc: int | None = 2000,
+        static_activity_indices: set[int] | None = None,
         skip_coproducts: bool | None = False,
         functional_unit_unique_id: int | None = -1,
         graph_traversal: (
             NewNodeEachVisitGraphTraversal | None
         ) = NewNodeEachVisitGraphTraversal,
     ):
         self.lca_object = lca_object
         self.unique_id = functional_unit_unique_id
         self.t0 = TemporalDistribution(
             np.array([np.datetime64(starting_datetime)]),
             np.array([1]),
         )
+
+        if static_activity_indices is None:
+            static_activity_indices = set()
+
         for db in bd.databases:
             if bd.databases[db].get("static"):
-                static_activity_indices.add(
-                    {
-                        obj[0]
-                        for obj in AD.select(AD.id).where(AD.database == db).tuples()
-                    }
+                static_activity_indices.update(
+                    obj[0] for obj in AD.select(AD.id).where(AD.database == db).tuples()
                 )
 
+        # Translate database indices to matrix indices which `graph_traversal` expects
+        static_activity_indices = {
+            self.lca_object.dicts.activity[x] for x in static_activity_indices
+        }
+
         print("Starting graph traversal")
         gt = graph_traversal.calculate(
             lca_object=lca_object,
             static_activity_indices=static_activity_indices,
             max_calc=max_calc,
             cutoff=cutoff,
             biosphere_cutoff=biosphere_cutoff,
@@ -302,23 +308,22 @@
         elif len(exchanges) == 1:
             yield from exchanges
         else:
             yield NoExchange
 
     def get_technosphere_exchange(self, input_id: int, output_id: int) -> ED:
         def printer(x):
-            return "({}|{}|{})".format(x['database'], x['code'], x['name'])
+            return "({}|{}|{})".format(x["database"], x["code"], x["name"])
 
         exchanges = self._exchange_iterator(input_id, output_id)
         if len(exchanges) > 1:
             _exchange = Exchange(exchanges[0])
             raise MultipleTechnosphereExchanges(
                 "Found {} exchanges for link between {} and {}".format(
-                    len(exchanges),
-                    printer(_exchange.input),
-                    printer(_exchange.output))
+                    len(exchanges), printer(_exchange.input), printer(_exchange.output)
+                )
             )
         elif not exchanges:
             # Edge injected via datapackage, no exchange in dataset
             return NoExchange
         else:
             return exchanges[0]
```

### Comparing `bw_temporalis-1.0/bw_temporalis/lcia/climate.py` & `bw_temporalis-1.1/bw_temporalis/lcia/climate.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/bw_temporalis/temporal_distribution.py` & `bw_temporalis-1.1/bw_temporalis/temporal_distribution.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/bw_temporalis/timeline.py` & `bw_temporalis-1.1/bw_temporalis/timeline.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/bw_temporalis/utils.py` & `bw_temporalis-1.1/bw_temporalis/utils.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/bw_temporalis.egg-info/PKG-INFO` & `bw_temporalis-1.1/bw_temporalis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_temporalis
-Version: 1.0
+Version: 1.1
 Summary: Revision of bw2temporalis for modern Brightway
 Home-page: https://github.com/brightway-lca/bw_temporalis
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
```

### Comparing `bw_temporalis-1.0/bw_temporalis.egg-info/SOURCES.txt` & `bw_temporalis-1.1/bw_temporalis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/docs/conf.py` & `bw_temporalis-1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/examples/__init__.py` & `bw_temporalis-1.1/examples/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 # -*- coding: utf-8 -*-
 from __future__ import print_function, unicode_literals
-from eight import *
 
+from brightway2 import Database, Method, databases, methods
+from eight import *
 
-from brightway2 import Database, databases, Method, methods
-from .. import dynamic_methods, DynamicIAMethod
+from .. import DynamicIAMethod, dynamic_methods
+from .ia import (
+    cumulative_CH4,
+    cumulative_CO2,
+    dynamic_cfs,
+    dynamic_discounted_cfs,
+    linear_decrease_weight,
+    marginal_CH4,
+    marginal_CO2,
+    static_cfs,
+)
 from .inv import db_data
-from .ia import static_cfs, dynamic_cfs, dynamic_discounted_cfs
-from .ia import cumulative_CO2, marginal_CO2, cumulative_CH4, marginal_CH4, linear_decrease_weight
 
 
 def import_example_data():
     db = Database("temp-example-db")
     if db.name not in databases:
         db.register()
     db.write(db_data)
```

### Comparing `bw_temporalis-1.0/examples/ia.py` & `bw_temporalis-1.1/examples/ia.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 # -*- coding: utf-8 -*-
 from __future__ import print_function, unicode_literals
-from eight import *
 
-import numpy as np
 import datetime
 
+import numpy as np
+from eight import *
+
+
 def cumulative_CO2(year):
     """Gives total radiative forcing from year zero to year *year* in watts/square meter/kilogram of CO2. From:
 
-        Joos, F., Roth, R., Fuglestvedt, J. S., Peters, G. P., Enting, I. G., Bloh, W. V.,
-        & Weaver, A. J. (2013). Carbon dioxide and climate impulse response functions for the
-        computation of greenhouse gas metrics: a multi-model analysis. Atmospheric Chemistry
-        and Physics, 13(5), 2793-2825.
+    Joos, F., Roth, R., Fuglestvedt, J. S., Peters, G. P., Enting, I. G., Bloh, W. V.,
+    & Weaver, A. J. (2013). Carbon dioxide and climate impulse response functions for the
+    computation of greenhouse gas metrics: a multi-model analysis. Atmospheric Chemistry
+    and Physics, 13(5), 2793-2825.
 
     """
     decay_term = lambda year, alpha, tau: alpha * tau * (1 - np.exp(-year / tau))
 
     RE = 1.76e-15  # Radiative forcing (W/m2/kg)
     alpha_0, alpha_1, alpha_2, alpha_3 = 0.2173, 0.2240, 0.2824, 0.2763
     tau_1, tau_2, tau_3 = 394.4, 36.54, 4.304
     return RE * (
-        alpha_0 * year +
-        decay_term(year, alpha_1, tau_1) +
-        decay_term(year, alpha_2, tau_2) +
-        decay_term(year, alpha_3, tau_3)
+        alpha_0 * year
+        + decay_term(year, alpha_1, tau_1)
+        + decay_term(year, alpha_2, tau_2)
+        + decay_term(year, alpha_3, tau_3)
     )
 
+
 def marginal_CO2(year, delta=1):
     """Get the marginal difference in radiative forcing for one year."""
     year = np.array(year)
     diff = cumulative_CO2(year) - cumulative_CO2(year - delta)
     diff[year < 0] = 0
     return diff
 
+
 def cumulative_CH4(year):
     """Gives total radiative forcing from year zero to year *year* in watts/square meter/kilogram of CH4.
 
     Values from fifth assessment report, chapter 8: Anthropogenic and Natural Radiative Forcing, and supplementary material.
 
     """
-    f1 = 0.5          # Unitless
-    f2 = 0.15         # Unitless
+    f1 = 0.5  # Unitless
+    f2 = 0.15  # Unitless
     alpha = 1.27e-13  # Radiative forcing (W/m2/kg)
-    tau = 12.4        # Lifetime (years)
+    tau = 12.4  # Lifetime (years)
     return (1 + f1 + f2) * alpha * tau * (1 - np.exp(-year / tau))
 
+
 def marginal_CH4(year, delta=1):
     """Get the marginal difference in radiation forcing for one year for methane."""
     year = np.array(year)
     diff = cumulative_CH4(year) - cumulative_CH4(year - delta)
     diff[year < 0] = 0
     return diff
 
 
 Y2000 = datetime.datetime(2000, 1, 1)
 Y2100 = datetime.datetime(1000, 1, 1)
-SLOPE = -1. / (Y2100 - Y2000).days
+SLOPE = -1.0 / (Y2100 - Y2000).days
 
 
 def linear_decrease_weight(dt):
     """Linear decrease from *start_year* to *end_year*, from 1 to 0."""
     # Convert from datetime if needed
     if hasattr(dt, "datetime"):
         dt = dt.datetime
@@ -67,59 +72,68 @@
         return 1
     elif dt > Y2100:
         return 0
     else:
         return 1 + SLOPE * (dt - Y2000).days
 
 
-static_cfs = [
-    [("temp-example-db", "CO2"), 1],
-    [("temp-example-db", "CH4"), 28]
-]
+static_cfs = [[("temp-example-db", "CO2"), 1], [("temp-example-db", "CH4"), 28]]
 
-dynamic_cfs  = {
-    ("temp-example-db", "CO2"): """def marginal_CO2_function(dt):
+dynamic_cfs = {
+    (
+        "temp-example-db",
+        "CO2",
+    ): """def marginal_CO2_function(dt):
     from bw2temporalis.examples import marginal_CO2
     from datetime import timedelta
     import collections
 
     return_tuple = collections.namedtuple('return_tuple', ['dt', 'amount'])
     xs = range(250)
     cfs = marginal_CO2(xs)
     return [return_tuple(dt + timedelta(days=365.24 * x), float(cfs[x])) for x in xs]
     """,
-    ("temp-example-db", "CH4"): """def marginal_CH4_function(dt):
+    (
+        "temp-example-db",
+        "CH4",
+    ): """def marginal_CH4_function(dt):
     from bw2temporalis.examples import marginal_CH4
     from datetime import timedelta
     import collections
 
     return_tuple = collections.namedtuple('return_tuple', ['dt', 'amount'])
     xs = range(250)
     cfs = marginal_CH4(xs)
     return [return_tuple(dt + timedelta(days=365.24 * x), float(cfs[x])) for x in xs]
-    """
+    """,
 }
 
 dynamic_discounted_cfs = {
-    ("temp-example-db", "CO2"): """def discounted_CO2_function(dt):
+    (
+        "temp-example-db",
+        "CO2",
+    ): """def discounted_CO2_function(dt):
     from bw2temporalis.examples import marginal_CO2, linear_decrease_weight
     from datetime import timedelta
     import collections
 
     return_tuple = collections.namedtuple('return_tuple', ['dt', 'amount'])
     xs = range(100)
     cfs = marginal_CO2(xs)
     data = [(dt + timedelta(days=365.24 * x), float(cfs[x])) for x in xs]
     return [return_tuple(x, y * linear_decrease_weight(x)) for x, y in data]
     """,
-    ("temp-example-db", "CH4"): """def discounted_CH4_function(dt):
+    (
+        "temp-example-db",
+        "CH4",
+    ): """def discounted_CH4_function(dt):
     from bw2temporalis.examples import marginal_CH4, linear_decrease_weight
     from datetime import timedelta
     import collections
 
     return_tuple = collections.namedtuple('return_tuple', ['dt', 'amount'])
     xs = range(100)
     cfs = marginal_CH4(xs)
     data = [(dt + timedelta(days=365.24 * x), float(cfs[x])) for x in xs]
     return [return_tuple(x, y * linear_decrease_weight(x)) for x, y in data]
-    """
+    """,
 }
```

### Comparing `bw_temporalis-1.0/setup.cfg` & `bw_temporalis-1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/tests/test_convolution.py` & `bw_temporalis-1.1/tests/test_convolution.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/tests/test_fixed_td.py` & `bw_temporalis-1.1/tests/test_fixed_td.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/tests/test_fixed_time_of_year.py` & `bw_temporalis-1.1/tests/test_fixed_time_of_year.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/tests/test_fixtures.py` & `bw_temporalis-1.1/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/tests/test_lca.py` & `bw_temporalis-1.1/tests/test_lca.py`

 * *Files 10% similar despite different names*

```diff
@@ -250,14 +250,107 @@
     )
     expected_df.sort_values(by="date", ascending=True, inplace=True)
     expected_df.reset_index(drop=True, inplace=True)
 
     pd.testing.assert_frame_equal(given_df, expected_df)
 
 
+@bw2test
+def test_temporalis_static_indices_correct_lookup():
+    bd.projects.set_current("__test_fixture__")
+
+    db = bd.Database("db")
+    # Push indices forward
+    bd.Database("fake").write(
+        {
+            ("fake", str(x)): {"type": "process", "exchanges": [], "name": "foo"}
+            for x in range(1000)
+        }
+    )
+    db.write(
+        {
+            ("db", "CO2"): {
+                "type": "emission",
+                "name": "carbon dioxide",
+            },
+            ("db", "CH4"): {
+                "type": "emission",
+                "name": "methane",
+            },
+            ("db", "A"): {
+                "name": "Functional Unit",
+                "exchanges": [
+                    {
+                        "amount": 5,
+                        "input": ("db", "B"),
+                        "temporal_distribution": easy_timedelta_distribution(
+                            0, 4, resolution="Y", steps=5
+                        ),
+                        "type": "technosphere",
+                    },
+                ],
+            },
+            ("db", "B"): {
+                "exchanges": [
+                    {"amount": 2, "input": ("db", "C"), "type": "technosphere"},
+                    {"amount": 4, "input": ("db", "D"), "type": "technosphere"},
+                    {
+                        "amount": 8,
+                        "input": ("db", "CO2"),
+                        "type": "biosphere",
+                        "temporal_distribution": easy_timedelta_distribution(
+                            10, 17, steps=4, resolution="Y"
+                        ),
+                    },
+                ],
+                "name": "B",
+            },
+            ("db", "C"): {
+                "exchanges": [
+                    {
+                        "amount": 0.5,
+                        "input": ("db", "CH4"),
+                        "type": "biosphere",
+                    },
+                ]
+            },
+            ("db", "D"): {
+                "exchanges": [
+                    {
+                        "amount": 2,
+                        "input": ("db", "CO2"),
+                        "type": "biosphere",
+                        "temporal_distribution": easy_timedelta_distribution(
+                            -8, -5, steps=4, resolution="Y"
+                        ),
+                    },
+                ]
+            },
+        }
+    )
+    bd.Method(("m",)).write([(("db", "CO2"), 1), (("db", "CH4"), 25)])
+
+    lca = LCA({("db", "A"): 2}, ("m",))
+    lca.lci()
+    lca.lcia()
+
+    assert lca.score == 410
+
+    static_indices = {x.id for x in db if x.get("type", "process") == "process"}
+    assert min(static_indices) > 500
+
+    tlca = TemporalisLCA(
+        lca_object=lca,
+        starting_datetime="2023-01-01",
+        static_activity_indices=static_indices,
+    )
+    # No timeline because everything is static
+    assert not tlca.build_timeline()
+
+
 @pytest.mark.xfail
 def test_temporalis_lca_node_timeline(basic_db):
     lca = LCA({("db", "A"): 2}, ("m",))
     lca.lci()
     lca.lcia()
 
     assert lca.score == 410
@@ -437,7 +530,22 @@
             "cumulative_score": 160,
             "direct_emissions_score": 160,
         },
     ]
 
     for a in expected_nodes:
         node_equal_dict(tlca.nodes[a["unique_id"]], a)
+
+
+def test_lca_provide_static_activity_indices(basic_db):
+    lca = LCA({("db", "A"): 2}, ("m",))
+    lca.lci()
+    lca.lcia()
+
+    TemporalisLCA(
+        lca_object=lca,
+        static_activity_indices=[
+            x.id for x in basic_db if x.get("type", "process") == "process"
+        ][:2],
+    )
+    with pytest.raises(TypeError):
+        TemporalisLCA(lca_object=lca, static_activity_indices=1001)
```

### Comparing `bw_temporalis-1.0/tests/test_patched_matrix_lca.py` & `bw_temporalis-1.1/tests/test_patched_matrix_lca.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/tests/test_serialization.py` & `bw_temporalis-1.1/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/tests/test_td.py` & `bw_temporalis-1.1/tests/test_td.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/tests/test_tdaware.py` & `bw_temporalis-1.1/tests/test_tdaware.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/tests/test_timeline.py` & `bw_temporalis-1.1/tests/test_timeline.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-1.0/tests/test_utils.py` & `bw_temporalis-1.1/tests/test_utils.py`

 * *Files identical despite different names*

