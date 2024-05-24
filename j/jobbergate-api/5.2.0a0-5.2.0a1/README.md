# Comparing `tmp/jobbergate_api-5.2.0a0.tar.gz` & `tmp/jobbergate_api-5.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_api-5.2.0a0.tar", max compression
+gzip compressed data, was "jobbergate_api-5.2.0a1.tar", max compression
```

## Comparing `jobbergate_api-5.2.0a0.tar` & `jobbergate_api-5.2.0a1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1082 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/LICENSE
--rw-r--r--   0        0        0      683 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/README.md
--rw-r--r--   0        0        0      169 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/__init__.py
--rw-r--r--   0        0        0       30 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/__init__.py
--rw-r--r--   0        0        0       54 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/clusters/__init__.py
--rw-r--r--   0        0        0      944 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/clusters/models.py
--rw-r--r--   0        0        0     2114 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/clusters/routers.py
--rw-r--r--   0        0        0     1582 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/clusters/schemas.py
--rw-r--r--   0        0        0      177 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/constants.py
--rw-r--r--   0        0        0     5251 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/dependencies.py
--rw-r--r--   0        0        0     3620 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/file_validation.py
--rw-r--r--   0        0        0     1955 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/garbage_collector.py
--rw-r--r--   0        0        0       43 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/__init__.py
--rw-r--r--   0        0        0      100 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/constants.py
--rw-r--r--   0        0        0     4098 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/models.py
--rw-r--r--   0        0        0    15897 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/routers.py
--rw-r--r--   0        0        0     7060 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/schemas.py
--rw-r--r--   0        0        0     3749 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/services.py
--rw-r--r--   0        0        0       40 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0     2984 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/models.py
--rw-r--r--   0        0        0    13925 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/routers.py
--rw-r--r--   0        0        0     4759 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/schemas.py
--rw-r--r--   0        0        0     6390 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/services.py
--rw-r--r--   0        0        0     1295 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/tools.py
--rw-r--r--   0        0        0       44 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0     6561 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/constants.py
--rw-r--r--   0        0        0     3575 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/models.py
--rw-r--r--   0        0        0    14577 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/routers.py
--rw-r--r--   0        0        0     8208 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/schemas.py
--rw-r--r--   0        0        0     1285 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/services.py
--rw-r--r--   0        0        0     5986 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/models.py
--rw-r--r--   0        0        0     1065 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/permissions.py
--rw-r--r--   0        0        0     2254 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/schemas.py
--rw-r--r--   0        0        0    23693 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/services.py
--rw-r--r--   0        0        0     4589 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/config.py
--rw-r--r--   0        0        0     2467 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/email_notification.py
--rw-r--r--   0        0        0     1627 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/logging.py
--rw-r--r--   0        0        0     3622 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/main.py
--rw-r--r--   0        0        0     3436 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/meta_mapper.py
--rw-r--r--   0        0        0     2781 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/rabbitmq_notification.py
--rw-r--r--   0        0        0     1082 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/safe_types.py
--rw-r--r--   0        0        0     4598 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/security.py
--rw-r--r--   0        0        0    10874 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/storage.py
--rw-r--r--   0        0        0     1146 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/version.py
--rw-r--r--   0        0        0     3982 2024-04-29 20:17:27.680660 jobbergate_api-5.2.0a0/pyproject.toml
--rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 jobbergate_api-5.2.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/LICENSE
+-rw-r--r--   0        0        0      683 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/README.md
+-rw-r--r--   0        0        0      169 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/__init__.py
+-rw-r--r--   0        0        0       54 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/clusters/__init__.py
+-rw-r--r--   0        0        0      944 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/clusters/models.py
+-rw-r--r--   0        0        0     2114 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/clusters/routers.py
+-rw-r--r--   0        0        0     1582 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/clusters/schemas.py
+-rw-r--r--   0        0        0      177 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/constants.py
+-rw-r--r--   0        0        0     5251 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/dependencies.py
+-rw-r--r--   0        0        0     3620 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/file_validation.py
+-rw-r--r--   0        0        0     1955 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/garbage_collector.py
+-rw-r--r--   0        0        0       43 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/__init__.py
+-rw-r--r--   0        0        0      100 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/constants.py
+-rw-r--r--   0        0        0     4098 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/models.py
+-rw-r--r--   0        0        0    16611 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/routers.py
+-rw-r--r--   0        0        0     7060 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/schemas.py
+-rw-r--r--   0        0        0     3749 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/services.py
+-rw-r--r--   0        0        0       40 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0     2984 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/models.py
+-rw-r--r--   0        0        0    14649 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/routers.py
+-rw-r--r--   0        0        0     4759 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/schemas.py
+-rw-r--r--   0        0        0     6483 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/services.py
+-rw-r--r--   0        0        0     1295 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/tools.py
+-rw-r--r--   0        0        0       44 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0     6561 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/constants.py
+-rw-r--r--   0        0        0     3575 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/models.py
+-rw-r--r--   0        0        0    14577 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/routers.py
+-rw-r--r--   0        0        0     8208 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/schemas.py
+-rw-r--r--   0        0        0     1285 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/services.py
+-rw-r--r--   0        0        0     5986 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/models.py
+-rw-r--r--   0        0        0     1065 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/permissions.py
+-rw-r--r--   0        0        0     2254 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/schemas.py
+-rw-r--r--   0        0        0    25232 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/apps/services.py
+-rw-r--r--   0        0        0     4589 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/config.py
+-rw-r--r--   0        0        0     2467 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/email_notification.py
+-rw-r--r--   0        0        0     1627 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/logging.py
+-rw-r--r--   0        0        0     3622 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/main.py
+-rw-r--r--   0        0        0     3436 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/meta_mapper.py
+-rw-r--r--   0        0        0     2781 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/rabbitmq_notification.py
+-rw-r--r--   0        0        0     1082 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/safe_types.py
+-rw-r--r--   0        0        0     4598 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/security.py
+-rw-r--r--   0        0        0    10874 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/storage.py
+-rw-r--r--   0        0        0     1146 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/version.py
+-rw-r--r--   0        0        0     4007 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 jobbergate_api-5.2.0a1/PKG-INFO
```

### Comparing `jobbergate_api-5.2.0a0/LICENSE` & `jobbergate_api-5.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/README.md` & `jobbergate_api-5.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/clusters/models.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/clusters/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/clusters/routers.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/clusters/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/clusters/schemas.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/clusters/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/dependencies.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/dependencies.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/file_validation.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/garbage_collector.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/models.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/routers.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/routers.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,43 +210,57 @@
         headers={"filename": job_script_template_file.filename},
     )
 
 
 @router.put(
     "/{id_or_identifier}/upload/template/{file_type}",
     status_code=status.HTTP_200_OK,
-    description="Endpoint to upload a file to a job script template by id or identifier",
+    description=(
+        "Endpoint to upload a file to a job script template by id or identifier. "
+        "If a previous filename is provided, the file will be renamed from that. "
+        "Upload file is optional in this scenario since the file content can be copied from previous file."
+    ),
     response_model=TemplateFileDetailedView,
 )
 async def job_script_template_upload_file(
     id_or_identifier: int | str = Path(),
     file_type: FileType = Path(),
-    upload_file: UploadFile = File(..., description="File to upload"),
+    filename: str | None = Query(None, max_length=255),
+    upload_file: UploadFile | None = File(None, description="File to upload"),
+    previous_filename: str | None = Query(
+        None, description="Previous name of the file in case a rename is needed", max_length=255
+    ),
     secure_services: SecureService = Depends(
         secure_services(Permissions.JOB_TEMPLATES_CREATE, ensure_email=True)
     ),
 ):
     """Upload a file to a job script template by id or identifier."""
-    if upload_file.filename is None:
+    # This is included for backwards compatibility with the previous implementation
+    # where filename was recovered from the upload_file object
+    filename = filename or getattr(upload_file, "filename")
+    if not filename:
         raise HTTPException(
-            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-            detail="The upload file has no filename",
+            status_code=status.HTTP_400_BAD_REQUEST,
+            detail="Filename must be provided either as a query parameter or as part of the file upload",
         )
 
-    logger.debug(f"Uploading file {upload_file.filename} to job script template {id_or_identifier=}")
+    logger.debug(
+        f"Uploading {filename=} to job template {id_or_identifier=}; {file_type=}; {previous_filename=}"
+    )
     job_script_template = await secure_services.crud.template.get(id_or_identifier)
     if Permissions.ADMIN not in secure_services.identity_payload.permissions:
         secure_services.crud.template.ensure_attribute(
             job_script_template, owner_email=secure_services.identity_payload.email
         )
 
     return await secure_services.file.template.upsert(
         parent_id=job_script_template.id,
-        filename=upload_file.filename,
+        filename=filename,
         upload_content=upload_file,
+        previous_filename=previous_filename,
         file_type=file_type,
     )
 
 
 @router.delete(
     "/{id_or_identifier}/upload/template/{file_name:path}",
     status_code=status.HTTP_200_OK,
```

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/schemas.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/services.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/models.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/routers.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/routers.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from jobbergate_api.apps.garbage_collector import garbage_collect
 from jobbergate_api.apps.job_script_templates.models import JobScriptTemplate
 from jobbergate_api.apps.job_scripts.models import JobScriptFile
 from jobbergate_api.apps.job_scripts.schemas import (
     JobScriptCloneRequest,
     JobScriptCreateRequest,
     JobScriptDetailedView,
+    JobScriptFileDetailedView,
     JobScriptListView,
     JobScriptUpdateRequest,
     RenderFromTemplateRequest,
 )
 from jobbergate_api.apps.job_scripts.tools import inject_sbatch_params
 from jobbergate_api.apps.permissions import Permissions
 from jobbergate_api.apps.schemas import ListParams
@@ -278,55 +279,67 @@
 ):
     """
     Get a job script file.
 
     Note:
         See https://fastapi.tiangolo.com/advanced/custom-response/#streamingresponse
     """
-    job_script = await secure_services.crud.job_script.get(id)
-    job_script_file = await secure_services.file.job_script.get(job_script.id, file_name)
+    job_script_file = await secure_services.file.job_script.get(id, file_name)
     return StreamingResponse(
         content=await secure_services.file.job_script.stream_file_content(job_script_file),
         media_type="text/plain",
         headers={"filename": job_script_file.filename},
     )
 
 
 @router.put(
     "/{id}/upload/{file_type}",
     status_code=status.HTTP_200_OK,
-    description="Endpoint to upload a file to a job script file",
+    description=(
+        "Endpoint to upload a file to a job script. "
+        "If a previous filename is provided, the file will be renamed from that. "
+        "Upload file is optional in this scenario since the file content can be copied from previous file."
+    ),
+    response_model=JobScriptFileDetailedView,
 )
 async def job_script_upload_file(
     id: int = Path(...),
     file_type: FileType = Path(...),
-    upload_file: UploadFile = File(..., description="File to upload"),
+    filename: str | None = Query(None, max_length=255),
+    upload_file: UploadFile | None = File(None, description="File to upload"),
+    previous_filename: str | None = Query(
+        None, description="Previous name of the file in case a rename is needed", max_length=255
+    ),
     secure_services: SecureService = Depends(
         secure_services(Permissions.JOB_SCRIPTS_CREATE, ensure_email=True)
     ),
 ):
     """Upload a file to a job script."""
-    if upload_file.filename is None:
+    # This is included for backwards compatibility with the previous implementation
+    # where filename was recovered from the upload_file object
+    filename = filename or getattr(upload_file, "filename")
+    if not filename:
         raise HTTPException(
-            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-            detail="The upload file has no filename",
+            status_code=status.HTTP_400_BAD_REQUEST,
+            detail="Filename must be provided either as a query parameter or as part of the file upload",
         )
 
-    logger.debug(f"Uploading file {upload_file.filename} to job script {id=}")
+    logger.debug(f"Uploading file {filename=} to job script {id=} with {file_type=} and {previous_filename=}")
 
     job_script = await secure_services.crud.job_script.get(id)
     if Permissions.ADMIN not in secure_services.identity_payload.permissions:
         secure_services.crud.job_script.ensure_attribute(
             job_script, owner_email=secure_services.identity_payload.email
         )
 
-    await secure_services.file.job_script.upsert(
+    return await secure_services.file.job_script.upsert(
         parent_id=job_script.id,
-        filename=upload_file.filename,
+        filename=filename,
         upload_content=upload_file,
+        previous_filename=previous_filename,
         file_type=file_type,
     )
 
 
 @router.delete(
     "/{id}/upload/{file_name}",
     status_code=status.HTTP_200_OK,
```

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/schemas.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/services.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,29 +119,30 @@
         error: Value of type variable "FileModel" of "FileService" cannot be "JobScriptFile"
     """
 
     async def upsert(
         self,
         parent_id: int,
         filename: str,
-        upload_content: str | bytes | UploadFile,
+        upload_content: str | bytes | UploadFile | None,
+        previous_filename: str | None = None,
         **upsert_kwargs,
     ) -> FileModel:
         """
         Upsert a file instance.
         """
         file_type: str = enforce_defined(
             upsert_kwargs.get("file_type", None),
             "File type must be defined when upserting a file.",
             raise_exc_class=ServiceError,
             raise_kwargs=dict(status_code=status.HTTP_422_UNPROCESSABLE_ENTITY),
         )
         if file_type == FileType.ENTRYPOINT:
-            await self.validate_entrypoint_file(parent_id, filename)
-        return await super().upsert(parent_id, filename, upload_content, **upsert_kwargs)
+            await self.validate_entrypoint_file(parent_id, previous_filename or filename)
+        return await super().upsert(parent_id, filename, upload_content, previous_filename, **upsert_kwargs)
 
     async def validate_entrypoint_file(self, parent_id: int, filename: str):
         """
         Validate that the entrypoint file is unique.
         """
         file_list = await self.find_children(parent_id)
```

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/tools.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/constants.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/models.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/routers.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/schemas.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/services.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/models.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/permissions.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/permissions.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/schemas.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/apps/services.py` & `jobbergate_api-5.2.0a1/jobbergate_api/apps/services.py`

 * *Files 5% similar despite different names*

```diff
@@ -520,22 +520,52 @@
         data: bytes = await stream.read()  # type: ignore
         return data
 
     async def upsert(
         self,
         parent_id: int,
         filename: str,
-        upload_content: str | bytes | UploadFile,
+        upload_content: str | bytes | UploadFile | None,
+        previous_filename: str | None = None,
         **upsert_kwargs,
     ) -> FileModel:
         """
         Upsert a file instance.
+
+        This method will either create a new file instance or update an existing one.
+
+        If a 'previous_filename' is provided, it is replaced by the new one, being deleted in the process.
+        In this case, the 'upload_content' is optional, as the content can be copied from the previous file.
         """
-        instance = await self.add_instance(parent_id, filename, upsert_kwargs)
+        upsert_instance = await self.add_instance(parent_id, filename, upsert_kwargs)
 
+        if previous_filename == filename:
+            previous_filename = None
+
+        if upload_content:
+            await self.upload_file_content(upsert_instance, upload_content)
+            if not previous_filename:
+                return upsert_instance
+        if previous_filename:
+            previous_instance = await self.get(parent_id, previous_filename)
+            if not upload_content:
+                await self.copy_file_content(previous_instance, upsert_instance)
+            await self.delete(previous_instance)
+            return upsert_instance
+
+        raise ServiceError(
+            "Either a file or a previous filename must be provided", status_code=status.HTTP_400_BAD_REQUEST
+        )
+
+    async def upload_file_content(
+        self, instance: FileModel, upload_content: str | bytes | UploadFile
+    ) -> None:
+        """
+        Upload the content of a file to s3.
+        """
         if isinstance(upload_content, str):
             file_obj: Any = io.BytesIO(upload_content.encode())
             size = file_obj.getbuffer().nbytes
         elif isinstance(upload_content, bytes):
             file_obj = io.BytesIO(upload_content)
             size = file_obj.getbuffer().nbytes
         elif hasattr(upload_content, "file") and hasattr(upload_content, "size"):
@@ -553,23 +583,22 @@
             size <= settings.MAX_UPLOAD_FILE_SIZE,
             f"Uploaded files cannot exceed {settings.MAX_UPLOAD_FILE_SIZE} bytes, got {size} bytes",
             raise_exc_class=ServiceError,
             raise_kwargs=dict(status_code=status.HTTP_413_REQUEST_ENTITY_TOO_LARGE),
         )
 
         require_condition(
-            check_uploaded_file_syntax(file_obj, filename),
-            f"File {filename=} did not pass the syntax check for its extension",
+            check_uploaded_file_syntax(file_obj, instance.filename),
+            f"File {instance.filename} did not pass the syntax check for its extension",
             raise_exc_class=ServiceError,
             raise_kwargs=dict(status_code=status.HTTP_400_BAD_REQUEST),
         )
 
         # Mypy doesn't like aioboto3 much
         await self.bucket.upload_fileobj(Fileobj=file_obj, Key=instance.file_key)  # type: ignore
-        return instance
 
     async def add_instance(self, parent_id, filename, upsert_kwargs) -> FileModel:
         """
         Add a file instance to the database.
         """
         instance: FileModel = self.model_type(
             parent_id=parent_id,
@@ -588,22 +617,28 @@
         logger.info(f"Cloning file={original_instance.file_key} to {new_parent_id=}")
         table = self.model_type.__table__  # type: ignore
         non_primary_key_columns = [c.name for c in table.columns if not c.primary_key]
         data = {c: getattr(original_instance, c) for c in non_primary_key_columns}
 
         cloned_instance = await self.add_instance(new_parent_id, original_instance.filename, data)
 
-        copy_source = {"Bucket": self.bucket.name, "Key": original_instance.file_key}
+        await self.copy_file_content(original_instance, cloned_instance)
+        return cloned_instance
+
+    async def copy_file_content(self, source_instance: FileModel, destination_instance: FileModel) -> None:
+        """
+        Copy the content of a file from one instance to another.
+        """
+        copy_source = {"Bucket": self.bucket.name, "Key": source_instance.file_key}
         with handle_errors(
-            f"{self.model_type.__tablename__} file={original_instance.file_key} could not be copied",
+            f"{self.model_type.__tablename__} file={source_instance.file_key} could not be copied",
             raise_exc_class=ServiceError,
             raise_kwargs=dict(status_code=status.HTTP_500_INTERNAL_SERVER_ERROR),
         ):
-            await self.bucket.copy(copy_source, cloned_instance.file_key)
-        return cloned_instance
+            await self.bucket.copy(copy_source, destination_instance.file_key)
 
     async def delete(self, instance: FileModel) -> None:
         """
         Delete a file from s3 and from the corresponding table.
         """
         await self.session.delete(instance)
         # Mypy doesn't like aioboto3 much
```

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/config.py` & `jobbergate_api-5.2.0a1/jobbergate_api/config.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/email_notification.py` & `jobbergate_api-5.2.0a1/jobbergate_api/email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/logging.py` & `jobbergate_api-5.2.0a1/jobbergate_api/logging.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/main.py` & `jobbergate_api-5.2.0a1/jobbergate_api/main.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/meta_mapper.py` & `jobbergate_api-5.2.0a1/jobbergate_api/meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/rabbitmq_notification.py` & `jobbergate_api-5.2.0a1/jobbergate_api/rabbitmq_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/safe_types.py` & `jobbergate_api-5.2.0a1/jobbergate_api/safe_types.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/security.py` & `jobbergate_api-5.2.0a1/jobbergate_api/security.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/storage.py` & `jobbergate_api-5.2.0a1/jobbergate_api/storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/jobbergate_api/version.py` & `jobbergate_api-5.2.0a1/jobbergate_api/version.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a0/pyproject.toml` & `jobbergate_api-5.2.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-api"
-version = "5.2.0a0"
+version = "5.2.0a1"
 description = "Jobbergate API"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -94,14 +94,15 @@
 
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = [
     "--random-order",
     "--cov=jobbergate_api",
+    "--cov-report=term",
     "--cov-report=xml:tests/coverage.xml",
     "--no-flaky-report",
 ]
 testpaths = ["tests"]
 asyncio_mode = "auto"
 
 [tool.pytest_env]
```

### Comparing `jobbergate_api-5.2.0a0/PKG-INFO` & `jobbergate_api-5.2.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-api
-Version: 5.2.0a0
+Version: 5.2.0a1
 Summary: Jobbergate API
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

