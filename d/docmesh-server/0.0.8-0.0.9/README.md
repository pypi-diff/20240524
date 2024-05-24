# Comparing `tmp/docmesh_server-0.0.8.tar.gz` & `tmp/docmesh_server-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_server-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_server-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_server-0.0.8.tar` & `docmesh_server-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       16 2024-05-14 04:58:32.409536 docmesh_server-0.0.8/README.md
--rw-r--r--   0        0        0       64 2024-05-23 05:41:01.598019 docmesh_server-0.0.8/docmesh_server/__init__.py
--rw-r--r--   0        0        0      707 2024-05-23 04:52:30.791699 docmesh_server-0.0.8/docmesh_server/database.py
--rw-r--r--   0        0        0     1220 2024-05-23 05:21:51.231797 docmesh_server-0.0.8/docmesh_server/dependencies.py
--rw-r--r--   0        0        0        0 2024-05-23 04:41:13.676269 docmesh_server-0.0.8/docmesh_server/internals/__init__.py
--rw-r--r--   0        0        0     1361 2024-05-23 04:53:44.441375 docmesh_server-0.0.8/docmesh_server/internals/admin.py
--rw-r--r--   0        0        0     2131 2024-05-23 05:16:56.945092 docmesh_server-0.0.8/docmesh_server/internals/collections.py
--rw-r--r--   0        0        0      960 2024-05-23 04:55:33.875867 docmesh_server-0.0.8/docmesh_server/internals/embeddings.py
--rw-r--r--   0        0        0     1604 2024-05-23 05:17:04.393262 docmesh_server-0.0.8/docmesh_server/internals/venues.py
--rw-r--r--   0        0        0     1090 2024-05-23 05:38:43.318860 docmesh_server-0.0.8/docmesh_server/main.py
--rw-r--r--   0        0        0        0 2024-05-23 03:27:04.878936 docmesh_server-0.0.8/docmesh_server/routers/__init__.py
--rw-r--r--   0        0        0     1138 2024-05-23 05:16:42.528764 docmesh_server-0.0.8/docmesh_server/routers/agents.py
--rw-r--r--   0        0        0     2466 2024-05-23 05:16:34.096572 docmesh_server-0.0.8/docmesh_server/routers/papers.py
--rw-r--r--   0        0        0      674 2024-05-22 08:55:49.532998 docmesh_server-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 docmesh_server-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-05-14 04:58:32.409536 docmesh_server-0.0.9/README.md
+-rw-r--r--   0        0        0       64 2024-05-24 02:20:55.436725 docmesh_server-0.0.9/docmesh_server/__init__.py
+-rw-r--r--   0        0        0      707 2024-05-23 05:55:08.341423 docmesh_server-0.0.9/docmesh_server/database.py
+-rw-r--r--   0        0        0     1220 2024-05-23 05:55:08.341423 docmesh_server-0.0.9/docmesh_server/dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-23 05:55:08.341423 docmesh_server-0.0.9/docmesh_server/internals/__init__.py
+-rw-r--r--   0        0        0     1368 2024-05-23 11:53:05.613620 docmesh_server-0.0.9/docmesh_server/internals/admin.py
+-rw-r--r--   0        0        0     2177 2024-05-23 11:52:26.448725 docmesh_server-0.0.9/docmesh_server/internals/collections.py
+-rw-r--r--   0        0        0      960 2024-05-23 05:55:08.341423 docmesh_server-0.0.9/docmesh_server/internals/embeddings.py
+-rw-r--r--   0        0        0     1610 2024-05-23 11:51:33.135505 docmesh_server-0.0.9/docmesh_server/internals/venues.py
+-rw-r--r--   0        0        0     1090 2024-05-23 05:55:08.345423 docmesh_server-0.0.9/docmesh_server/main.py
+-rw-r--r--   0        0        0        0 2024-05-23 05:55:08.345423 docmesh_server-0.0.9/docmesh_server/routers/__init__.py
+-rw-r--r--   0        0        0     1138 2024-05-23 05:55:08.345423 docmesh_server-0.0.9/docmesh_server/routers/agents.py
+-rw-r--r--   0        0        0     2507 2024-05-24 02:06:06.400381 docmesh_server-0.0.9/docmesh_server/routers/papers.py
+-rw-r--r--   0        0        0      674 2024-05-24 02:20:50.692617 docmesh_server-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 docmesh_server-0.0.9/PKG-INFO
```

### Comparing `docmesh_server-0.0.8/docmesh_server/database.py` & `docmesh_server-0.0.9/docmesh_server/database.py`

 * *Files identical despite different names*

### Comparing `docmesh_server-0.0.8/docmesh_server/dependencies.py` & `docmesh_server-0.0.9/docmesh_server/dependencies.py`

 * *Files identical despite different names*

### Comparing `docmesh_server-0.0.8/docmesh_server/internals/admin.py` & `docmesh_server-0.0.9/docmesh_server/internals/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any
 from pydantic import BaseModel
 
 from fastapi import status, APIRouter, Response, Depends
 
-from docmesh_core.db.neo import add_entity, DuplicateEntity
 from docmesh_core.db.auth import add_auth_for_entity
+from docmesh_core.db.neo.entity import add_entity, DuplicateEntity
 from docmesh_server.database import engine
 from docmesh_server.dependencies import check_admin_access_token
 
 router = APIRouter(prefix="/admin", dependencies=[Depends(check_admin_access_token)])
 
 
 class EntityBody(BaseModel):
```

### Comparing `docmesh_server-0.0.8/docmesh_server/internals/collections.py` & `docmesh_server-0.0.9/docmesh_server/internals/collections.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any
 from pydantic import BaseModel
 
 from fastapi import status, APIRouter, Response, Depends
 
+from docmesh_core.db.neo.paper import add_paper
+from docmesh_core.db.neo.collection import add_collection, add_paper_to_collection
 from docmesh_core.utils.semantic_scholar import get_paper_id
-from docmesh_core.db.neo import _add_paper, add_collection, add_paper_to_collection
 from docmesh_server.dependencies import check_admin_access_token
 
 router = APIRouter(prefix="/collections", dependencies=[Depends(check_admin_access_token)])
 
 
 class CollectionBody(BaseModel):
     collection_name: str
@@ -48,15 +49,15 @@
     if semantic_scholar_paper_id is None:
         response.status_code = status.HTTP_404_NOT_FOUND
         data = {
             "msg": f"Failed to add {body.paper} to collection, cannot find semantic scholar paper id.",
         }
     else:
         try:
-            paper_id = _add_paper(paper_id=semantic_scholar_paper_id).paper_id
+            paper_id = add_paper(paper_id=semantic_scholar_paper_id).paper_id
             add_paper_to_collection(paper_id=paper_id, collection_name=body.collection_name)
             data = {
                 "msg": f"Successfully add paper {body.paper} to collection {body.collection_name}.",
             }
         except Exception as e:
             response.status_code = status.HTTP_500_INTERNAL_SERVER_ERROR
             data = {
```

### Comparing `docmesh_server-0.0.8/docmesh_server/internals/embeddings.py` & `docmesh_server-0.0.9/docmesh_server/internals/embeddings.py`

 * *Files identical despite different names*

### Comparing `docmesh_server-0.0.8/docmesh_server/internals/venues.py` & `docmesh_server-0.0.9/docmesh_server/internals/venues.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any
 from pydantic import BaseModel
 
 from fastapi import status, APIRouter, Response, Depends
 
-from docmesh_core.db.neo import add_venue, add_collection_to_venue
+from docmesh_core.db.neo.venue import add_venue, add_collection_to_venue
 from docmesh_server.dependencies import check_admin_access_token
 
 router = APIRouter(prefix="/venues", dependencies=[Depends(check_admin_access_token)])
 
 
 class VenueBody(BaseModel):
     venue_name: str
```

### Comparing `docmesh_server-0.0.8/docmesh_server/main.py` & `docmesh_server-0.0.9/docmesh_server/main.py`

 * *Files identical despite different names*

### Comparing `docmesh_server-0.0.8/docmesh_server/routers/agents.py` & `docmesh_server-0.0.9/docmesh_server/routers/agents.py`

 * *Files identical despite different names*

### Comparing `docmesh_server-0.0.8/docmesh_server/routers/papers.py` & `docmesh_server-0.0.9/docmesh_server/routers/papers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any
 from pydantic import BaseModel
 
 from fastapi import status, APIRouter, Response, Depends
 
+from docmesh_core.db.neo.paper import add_paper
+from docmesh_core.db.neo.entity import mark_paper_read
 from docmesh_core.utils.semantic_scholar import get_paper_id
-from docmesh_core.db.neo import _add_paper, mark_paper_read
 from docmesh_server.dependencies import check_access_token, EntityInfo
 
 router = APIRouter(prefix="/papers")
 
 
 class PaperBody(BaseModel):
     paper: str
@@ -25,15 +26,15 @@
     if semantic_scholar_paper_id is None:
         response.status_code = status.HTTP_404_NOT_FOUND
         data = {
             "msg": f"Failed to add a new paper {body.paper}, cannot find semantic scholar paper id.",
         }
     else:
         try:
-            paper_id = _add_paper(paper_id=semantic_scholar_paper_id).paper_id
+            paper_id = add_paper(paper_id=semantic_scholar_paper_id).paper_id
             data = {
                 "msg": f"Successfully add a new paper {body.paper} with paper id {paper_id}.",
             }
         except Exception as e:
             response.status_code = status.HTTP_500_INTERNAL_SERVER_ERROR
             data = {
                 "msg": f"Failed to add a new paper {body.paper}, with error: {e}.",
@@ -54,15 +55,15 @@
     if semantic_scholar_paper_id is None:
         response.status_code = status.HTTP_404_NOT_FOUND
         data = {
             "msg": f"Failed to add and mark paper {body.paper}, cannot find semantic scholar paper id.",
         }
     else:
         try:
-            paper_id = _add_paper(paper_id=semantic_scholar_paper_id).paper_id
+            paper_id = add_paper(paper_id=semantic_scholar_paper_id).paper_id
             mark_paper_read(entity_name=entity_name, paper_id=paper_id)
             data = {
                 "msg": (
                     f"Successfully add and mark paper {body.paper} read with paper id {paper_id} for {entity_name}."
                 ),
             }
         except Exception as e:
```

### Comparing `docmesh_server-0.0.8/pyproject.toml` & `docmesh_server-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent"
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "docmesh-core>=0.0.8",
-    "docmesh-agent>=0.0.10",
+    "docmesh-core>=0.0.9",
+    "docmesh-agent>=0.0.11",
     "fastapi==0.111.0",
     "uvicorn==0.29.0",
     "gunicorn==19.3.0",
 ]
 
 [tool.flake8]
 max-line-length = 120
```

### Comparing `docmesh_server-0.0.8/PKG-INFO` & `docmesh_server-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: docmesh_server
-Version: 0.0.8
+Version: 0.0.9
 Summary: Server of docmesh.
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Dist: docmesh-core>=0.0.8
-Requires-Dist: docmesh-agent>=0.0.10
+Requires-Dist: docmesh-core>=0.0.9
+Requires-Dist: docmesh-agent>=0.0.11
 Requires-Dist: fastapi==0.111.0
 Requires-Dist: uvicorn==0.29.0
 Requires-Dist: gunicorn==19.3.0
 
 # docemsh server
```

