# Comparing `tmp/taegis_magic-2024.3.29.tar.gz` & `tmp/taegis_magic-2024.5.24.tar.gz`

## Comparing `taegis_magic-2024.3.29.tar` & `taegis_magic-2024.5.24.tar`

### file list

```diff
@@ -1,44 +1,43 @@
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/_version.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/cli.py
--rw-r--r--   0        0        0     6903 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/magics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/__init__.py
--rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/alerts.py
--rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/audits.py
--rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/clients.py
--rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/configure.py
--rw-r--r--   0        0        0     8404 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/events.py
--rw-r--r--   0        0        0    24637 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/investigations.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/preferences.py
--rw-r--r--   0        0        0    16102 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/rules.py
--rw-r--r--   0        0        0    24939 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/tenant_profiles.py
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/tenants.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/threat.py
--rw-r--r--   0        0        0     7336 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/utils/__init__.py
--rw-r--r--   0        0        0    14693 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/commands/utils/investigations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/core/__init__.py
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/core/cache.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/core/callbacks.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/core/log.py
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/core/normalizer.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/core/queries.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/core/service.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/core/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/__init__.py
--rw-r--r--   0        0        0    12891 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/alerts.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/assets.py
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/audits.py
--rw-r--r--   0        0        0    20558 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/context.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/events.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/rules.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/tenants.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/pandas/utils.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/templates/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/templates/taegis_results.md.jinja
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/taegis_magic/templates/taegis_search_results.md.jinja
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/.gitignore
--rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/LICENSE
--rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/README.md
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/pyproject.toml
--rw-r--r--   0        0        0    19302 2020-02-02 00:00:00.000000 taegis_magic-2024.3.29/PKG-INFO
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/_version.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/cli.py
+-rw-r--r--   0        0        0     6903 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/magics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/commands/__init__.py
+-rw-r--r--   0        0        0    10292 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/commands/alerts.py
+-rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/commands/audits.py
+-rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/commands/clients.py
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/commands/configure.py
+-rw-r--r--   0        0        0     7361 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/commands/events.py
+-rw-r--r--   0        0        0    24575 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/commands/investigations.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/commands/preferences.py
+-rw-r--r--   0        0        0    16102 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/commands/rules.py
+-rw-r--r--   0        0        0    24939 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/commands/tenant_profiles.py
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/commands/tenants.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/commands/threat.py
+-rw-r--r--   0        0        0     7336 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/commands/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/commands/utils/__init__.py
+-rw-r--r--   0        0        0    14693 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/commands/utils/investigations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/core/__init__.py
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/core/cache.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/core/callbacks.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/core/log.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/core/normalizer.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/core/service.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/core/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/pandas/__init__.py
+-rw-r--r--   0        0        0    12891 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/pandas/alerts.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/pandas/assets.py
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/pandas/audits.py
+-rw-r--r--   0        0        0    20558 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/pandas/context.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/pandas/events.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/pandas/rules.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/pandas/tenants.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/pandas/utils.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/templates/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/templates/taegis_results.md.jinja
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/taegis_magic/templates/taegis_search_results.md.jinja
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/.gitignore
+-rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/LICENSE
+-rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/README.md
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/pyproject.toml
+-rw-r--r--   0        0        0    19302 2020-02-02 00:00:00.000000 taegis_magic-2024.5.24/PKG-INFO
```

### Comparing `taegis_magic-2024.3.29/taegis_magic/cli.py` & `taegis_magic-2024.5.24/taegis_magic/cli.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/magics.py` & `taegis_magic-2024.5.24/taegis_magic/magics.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/commands/alerts.py` & `taegis_magic-2024.5.24/taegis_magic/commands/alerts.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 import typer
 from dataclasses_json import config, dataclass_json
 from taegis_magic.commands.configure import QUERIES_SECTION
 from taegis_magic.core.log import tracing
 from taegis_magic.core.normalizer import TaegisResultsNormalizer
 
-from taegis_magic.core.queries import create_query
 from taegis_magic.core.service import get_service
 from taegis_sdk_python import (
     GraphQLNoRowsInResultSetError,
     GraphQLService,
     build_output_string,
     prepare_input,
 )
@@ -135,49 +134,18 @@
     @property
     def query_identifier(self) -> Optional[str]:
         """Alerts Service Query Identifier."""
         log.debug("Calling AlertsResultsNormalizer.query_identifier...")
         if not self.raw_results:
             return None
 
-        if self._query_id:
-            return self._query_id
-
         if self.raw_results[0].query_id:
-            self._query_id = self.raw_results[0].query_id
-            return self._query_id
-
-        if not self.query:
-            raise ValueError("No query found to generate query id")
-
-        query_name = "Taegis Query Magic" if self.is_saved else "alert"
-        data = {
-            "query": None,
-            "name": query_name,
-            "description": self.query,
-            "query_source": "alert",
-            "metadata": [
-                {"id": "start"},
-                {"id": "dateOption", "value": "custom"},
-                {"id": "timeDescription"},
-                {"id": "searchTerms"},
-                {"id": "isSaved", "value": str(self.is_saved).lower()},
-                {"id": "isRedql", "value": "true"},
-                {"id": "isAlerts2", "value": "true"},
-            ],
-        }
-        service = get_service(environment=self.region, tenant_id=self.tenant_id)
-        query_id = create_query(service, data).get("id")
-
-        if not query_id:
-            log.error("No query id returned from Query API")
-
-        self._query_id = query_id
+            return self.raw_results[0].query_id
 
-        return self._query_id
+        return None
 
     @property
     def shareable_url(self) -> str:
         """Alerts Service Sharelinks URL."""
         log.debug("Calling AlertsResultsNormalizer.shareable_url...")
         if not self.raw_results:
             return "Unable to create shareable link"
```

### Comparing `taegis_magic-2024.3.29/taegis_magic/commands/audits.py` & `taegis_magic-2024.5.24/taegis_magic/commands/audits.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/commands/clients.py` & `taegis_magic-2024.5.24/taegis_magic/commands/clients.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/commands/configure.py` & `taegis_magic-2024.5.24/taegis_magic/commands/configure.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/commands/events.py` & `taegis_magic-2024.5.24/taegis_magic/commands/events.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import typer
 from dataclasses_json import dataclass_json
 from taegis_magic.commands.configure import QUERIES_SECTION
 from taegis_magic.commands.utils.investigations import insert_search_query
 from taegis_magic.core.log import tracing
 from taegis_magic.core.normalizer import TaegisResultsNormalizer
 
-from taegis_magic.core.queries import create_query
 from taegis_magic.core.service import get_service
 from taegis_sdk_python.config import get_config
 from taegis_sdk_python.services.events.types import (
     Event,
     EventQueryOptions,
     EventQueryResults,
 )
@@ -142,48 +141,18 @@
             No query found to generate query id
         ValueError
             No query id returned from Query API
         """
         if not self.raw_results:
             return None
 
-        if self._query_id:
-            return self._query_id
-
         if self.raw_results[0].query_id:
-            self._query_id = self.raw_results[0].query_id
-            return self._query_id
-
-        if not self.query:
-            raise None
-
-        query_name = self.query if self.is_saved else "cql"
-        data = {
-            "query": None,
-            "name": query_name,
-            "description": self.query,
-            "query_source": "cql",
-            "metadata": [
-                {"id": "start"},
-                {"id": "dateOption", "value": "custom"},
-                {"id": "timeDescription"},
-                {"id": "searchTerms"},
-                {"id": "isSaved", "value": str(self.is_saved).lower()},
-                {"id": "isRedql", "value": "true"},
-            ],
-        }
-        service = get_service(environment=self.region, tenant_id=self.tenant_id)
-        query_id = create_query(service, data).get("id")
-
-        if not query_id:
-            raise ValueError("No query id returned from Query API")
-
-        self._query_id = query_id
+            return self.raw_results[0].query_id
 
-        return self._query_id
+        return None
 
     @property
     def shareable_url(self) -> str:
         """Generate a shareable url for Taegis XDR.
 
         Returns
         -------
```

### Comparing `taegis_magic-2024.3.29/taegis_magic/commands/investigations.py` & `taegis_magic-2024.5.24/taegis_magic/commands/investigations.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 from taegis_magic.core.log import tracing
 from taegis_magic.core.normalizer import (
     DataFrameNormalizer,
     TaegisResult,
     TaegisResults,
     TaegisResultsNormalizer,
 )
-from taegis_magic.core.queries import get_query, update_query
 from taegis_magic.core.service import get_service
 from taegis_magic.core.utils import remove_output_node
 from taegis_magic.core.callbacks import verify_file
 from taegis_sdk_python import build_output_string
 from taegis_sdk_python.services.investigations2.types import (
     CreateInvestigationInput,
     InvestigationStatus,
```

### Comparing `taegis_magic-2024.3.29/taegis_magic/commands/preferences.py` & `taegis_magic-2024.5.24/taegis_magic/commands/preferences.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/commands/rules.py` & `taegis_magic-2024.5.24/taegis_magic/commands/rules.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/commands/tenant_profiles.py` & `taegis_magic-2024.5.24/taegis_magic/commands/tenant_profiles.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/commands/tenants.py` & `taegis_magic-2024.5.24/taegis_magic/commands/tenants.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/commands/threat.py` & `taegis_magic-2024.5.24/taegis_magic/commands/threat.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/commands/users.py` & `taegis_magic-2024.5.24/taegis_magic/commands/users.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/commands/utils/investigations.py` & `taegis_magic-2024.5.24/taegis_magic/commands/utils/investigations.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/core/cache.py` & `taegis_magic-2024.5.24/taegis_magic/core/cache.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/core/log.py` & `taegis_magic-2024.5.24/taegis_magic/core/log.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/core/normalizer.py` & `taegis_magic-2024.5.24/taegis_magic/core/normalizer.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/core/service.py` & `taegis_magic-2024.5.24/taegis_magic/core/service.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/core/utils.py` & `taegis_magic-2024.5.24/taegis_magic/core/utils.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/pandas/alerts.py` & `taegis_magic-2024.5.24/taegis_magic/pandas/alerts.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/pandas/assets.py` & `taegis_magic-2024.5.24/taegis_magic/pandas/assets.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/pandas/audits.py` & `taegis_magic-2024.5.24/taegis_magic/pandas/audits.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/pandas/context.py` & `taegis_magic-2024.5.24/taegis_magic/pandas/context.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/pandas/events.py` & `taegis_magic-2024.5.24/taegis_magic/pandas/events.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/pandas/rules.py` & `taegis_magic-2024.5.24/taegis_magic/pandas/rules.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/pandas/tenants.py` & `taegis_magic-2024.5.24/taegis_magic/pandas/tenants.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/pandas/utils.py` & `taegis_magic-2024.5.24/taegis_magic/pandas/utils.py`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/taegis_magic/templates/taegis_search_results.md.jinja` & `taegis_magic-2024.5.24/taegis_magic/templates/taegis_search_results.md.jinja`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/.gitignore` & `taegis_magic-2024.5.24/.gitignore`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/LICENSE` & `taegis_magic-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/README.md` & `taegis_magic-2024.5.24/README.md`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/pyproject.toml` & `taegis_magic-2024.5.24/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taegis_magic-2024.3.29/PKG-INFO` & `taegis_magic-2024.5.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: taegis-magic
-Version: 2024.3.29
+Version: 2024.5.24
 Summary: Taegis IPython Magics
 Project-URL: Homepage, https://github.com/secureworks/taegis-magic
 Project-URL: Bug Reports, https://github.com/secureworks/taegis-magic/issues
 Project-URL: Source, https://github.com/secureworks/taegis-magic
 Project-URL: Package, https://pypi.org/project/taegis-magic/
 Author-email: Micah Pegman <sdks@secureworks.com>
 License:                                  Apache License
```

