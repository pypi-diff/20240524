# Comparing `tmp/fal-1.0.2.tar.gz` & `tmp/fal-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal-1.0.2.tar", last modified: Fri May 10 23:18:26 2024, max compression
+gzip compressed data, was "fal-1.0.3.tar", last modified: Fri May 24 12:42:37 2024, max compression
```

## Comparing `fal-1.0.2.tar` & `fal-1.0.3.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.490856 fal-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 23:18:20.000000 fal-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-10 23:18:26.490856 fal-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-10 23:18:20.000000 fal-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.486856 fal-1.0.2/fal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-10 23:18:26.000000 fal-1.0.2/fal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-10 23:18:26.000000 fal-1.0.2/fal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:18:26.000000 fal-1.0.2/fal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 23:18:26.000000 fal-1.0.2/fal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-10 23:18:26.000000 fal-1.0.2/fal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 23:18:26.000000 fal-1.0.2/fal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.466856 fal-1.0.2/openapi-fal-rest/
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.466856 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.466856 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.466856 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/applications/app_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.466856 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/billing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/billing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/billing/get_user_details.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.470856 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/files/check_dir_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/files/upload_local_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.470856 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/workflows/create_or_update_workflow_workflows_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/workflows/delete_workflow_workflows_user_id_workflow_name_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/workflows/execute_workflow_workflows_user_id_workflow_name_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflow_workflows_user_id_workflow_name_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflows_workflows_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.474856 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/app_metadata_response_app_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/body_upload_local_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/customer_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_json_body_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_response_200_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/hash_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/lock_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/page_workflow_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/typed_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_detail_contents_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_node_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_output.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/openapi_fal_rest/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-10 23:18:20.000000 fal-1.0.2/openapi-fal-rest/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 23:18:20.000000 fal-1.0.2/openapi_rest.config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-10 23:18:20.000000 fal-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 23:18:26.490856 fal-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.462856 fal-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.478856 fal-1.0.2/src/fal/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 23:18:26.000000 fal-1.0.2/src/fal/_fal_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7655 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    36287 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13826 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.478856 fal-1.0.2/src/fal/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/auth/auth0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/auth/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.478856 fal-1.0.2/src/fal/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/cli/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/cli/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/cli/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.478856 fal-1.0.2/src/fal/console/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/console/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/console/ux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.482856 fal-1.0.2/src/fal/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/exceptions/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/exceptions/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.482856 fal-1.0.2/src/fal/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/logging/isolate.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/logging/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/logging/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/logging/user.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/rest_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19976 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.482856 fal-1.0.2/src/fal/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/toolkit/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.482856 fal-1.0.2/src/fal/toolkit/file/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/toolkit/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/toolkit/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.482856 fal-1.0.2/src/fal/toolkit/file/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/toolkit/file/providers/fal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/toolkit/file/providers/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/toolkit/file/providers/r2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/toolkit/file/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.482856 fal-1.0.2/src/fal/toolkit/image/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/toolkit/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/toolkit/image/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/toolkit/optimize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.482856 fal-1.0.2/src/fal/toolkit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/toolkit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/toolkit/utils/download_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14682 2024-05-10 23:18:20.000000 fal-1.0.2/src/fal/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.486856 fal-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:20.000000 fal-1.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.486856 fal-1.0.2/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:20.000000 fal-1.0.2/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-10 23:18:20.000000 fal-1.0.2/tests/cli/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-10 23:18:20.000000 fal-1.0.2/tests/cli/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-10 23:18:20.000000 fal-1.0.2/tests/cli/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-10 23:18:20.000000 fal-1.0.2/tests/cli/test_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-10 23:18:20.000000 fal-1.0.2/tests/cli/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-10 23:18:20.000000 fal-1.0.2/tests/cli/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-10 23:18:20.000000 fal-1.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-10 23:18:20.000000 fal-1.0.2/tests/integration_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.486856 fal-1.0.2/tests/mainify_package/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 23:18:20.000000 fal-1.0.2/tests/mainify_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-10 23:18:20.000000 fal-1.0.2/tests/mainify_package/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 23:18:20.000000 fal-1.0.2/tests/mainify_package/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-10 23:18:20.000000 fal-1.0.2/tests/mainify_target.py
--rw-r--r--   0 runner    (1001) docker     (127)    17322 2024-05-10 23:18:20.000000 fal-1.0.2/tests/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    16943 2024-05-10 23:18:20.000000 fal-1.0.2/tests/test_stability.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.486856 fal-1.0.2/tests/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-10 23:18:20.000000 fal-1.0.2/tests/toolkit/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-10 23:18:20.000000 fal-1.0.2/tests/toolkit/image_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:18:26.486856 fal-1.0.2/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-10 23:18:20.000000 fal-1.0.2/tools/demo_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.370914 fal-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 12:42:27.000000 fal-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-24 12:42:37.370914 fal-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-24 12:42:27.000000 fal-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.366914 fal-1.0.3/fal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-24 12:42:37.000000 fal-1.0.3/fal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-24 12:42:37.000000 fal-1.0.3/fal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:42:37.000000 fal-1.0.3/fal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-24 12:42:37.000000 fal-1.0.3/fal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-24 12:42:37.000000 fal-1.0.3/fal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 12:42:37.000000 fal-1.0.3/fal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.346914 fal-1.0.3/openapi-fal-rest/
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.346914 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.346914 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.346914 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/applications/app_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.346914 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/billing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/billing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/billing/get_user_details.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.346914 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/files/check_dir_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/files/upload_local_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.350914 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/workflows/create_or_update_workflow_workflows_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/workflows/delete_workflow_workflows_user_id_workflow_name_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/workflows/execute_workflow_workflows_user_id_workflow_name_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflow_workflows_user_id_workflow_name_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflows_workflows_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.354914 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/app_metadata_response_app_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/body_upload_local_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/customer_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_json_body_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_response_200_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/hash_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/lock_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/page_workflow_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/typed_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_detail_contents_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_node_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/openapi_fal_rest/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-24 12:42:27.000000 fal-1.0.3/openapi-fal-rest/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 12:42:27.000000 fal-1.0.3/openapi_rest.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-24 12:42:27.000000 fal-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 12:42:37.370914 fal-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.342913 fal-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.354914 fal-1.0.3/src/fal/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 12:42:37.000000 fal-1.0.3/src/fal/_fal_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7655 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36286 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13826 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.358914 fal-1.0.3/src/fal/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/auth/auth0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/auth/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.358914 fal-1.0.3/src/fal/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/cli/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/cli/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/cli/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.358914 fal-1.0.3/src/fal/console/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/console/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/console/ux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.358914 fal-1.0.3/src/fal/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/exceptions/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/exceptions/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.362914 fal-1.0.3/src/fal/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/logging/isolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/logging/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/logging/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/logging/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19976 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.362914 fal-1.0.3/src/fal/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/toolkit/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.362914 fal-1.0.3/src/fal/toolkit/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/toolkit/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/toolkit/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.362914 fal-1.0.3/src/fal/toolkit/file/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/toolkit/file/providers/fal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/toolkit/file/providers/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/toolkit/file/providers/r2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/toolkit/file/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.362914 fal-1.0.3/src/fal/toolkit/image/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/toolkit/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/toolkit/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/toolkit/optimize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.362914 fal-1.0.3/src/fal/toolkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/toolkit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17006 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/toolkit/utils/download_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14682 2024-05-24 12:42:27.000000 fal-1.0.3/src/fal/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.366914 fal-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:27.000000 fal-1.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.366914 fal-1.0.3/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:27.000000 fal-1.0.3/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-24 12:42:27.000000 fal-1.0.3/tests/cli/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-24 12:42:27.000000 fal-1.0.3/tests/cli/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-24 12:42:27.000000 fal-1.0.3/tests/cli/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-24 12:42:27.000000 fal-1.0.3/tests/cli/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-24 12:42:27.000000 fal-1.0.3/tests/cli/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-24 12:42:27.000000 fal-1.0.3/tests/cli/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-24 12:42:27.000000 fal-1.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-24 12:42:27.000000 fal-1.0.3/tests/integration_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.366914 fal-1.0.3/tests/mainify_package/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-24 12:42:27.000000 fal-1.0.3/tests/mainify_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-24 12:42:27.000000 fal-1.0.3/tests/mainify_package/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 12:42:27.000000 fal-1.0.3/tests/mainify_package/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-24 12:42:27.000000 fal-1.0.3/tests/mainify_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-05-24 12:42:27.000000 fal-1.0.3/tests/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16591 2024-05-24 12:42:27.000000 fal-1.0.3/tests/test_stability.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.366914 fal-1.0.3/tests/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-24 12:42:27.000000 fal-1.0.3/tests/toolkit/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-24 12:42:27.000000 fal-1.0.3/tests/toolkit/image_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:42:37.366914 fal-1.0.3/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-24 12:42:27.000000 fal-1.0.3/tools/demo_script.py
```

### Comparing `fal-1.0.2/PKG-INFO` & `fal-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fal
-Version: 1.0.2
+Version: 1.0.3
 Summary: fal is an easy-to-use Serverless Python Framework
-Author: Features & Labels <hello@fal.ai>
+Author: Features & Labels <support@fal.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: isolate[build]<1.0,>=0.12.3
 Requires-Dist: isolate-proto==0.4.0
 Requires-Dist: grpcio<2,>=1.50.0
 Requires-Dist: dill==0.3.7
 Requires-Dist: cloudpickle==3.0.0
@@ -16,15 +16,15 @@
 Requires-Dist: opentelemetry-api<2,>=1.15.0
 Requires-Dist: opentelemetry-sdk<2,>=1.15.0
 Requires-Dist: grpc-interceptor<1,>=0.15.0
 Requires-Dist: colorama<1,>=0.4.6
 Requires-Dist: portalocker<3,>=2.7.0
 Requires-Dist: rich<14,>=13.3.2
 Requires-Dist: rich_argparse
-Requires-Dist: packaging<22,>=21.3
+Requires-Dist: packaging>=21.3
 Requires-Dist: pathspec<1,>=0.11.1
 Requires-Dist: pydantic!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,<3
 Requires-Dist: fastapi<1,>=0.99.1
 Requires-Dist: starlette-exporter>=0.21.0
 Requires-Dist: httpx>=0.15.4
 Requires-Dist: attrs>=21.3.0
 Requires-Dist: python-dateutil<3,>=2.8.0
```

### Comparing `fal-1.0.2/README.md` & `fal-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/fal.egg-info/PKG-INFO` & `fal-1.0.3/fal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fal
-Version: 1.0.2
+Version: 1.0.3
 Summary: fal is an easy-to-use Serverless Python Framework
-Author: Features & Labels <hello@fal.ai>
+Author: Features & Labels <support@fal.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: isolate[build]<1.0,>=0.12.3
 Requires-Dist: isolate-proto==0.4.0
 Requires-Dist: grpcio<2,>=1.50.0
 Requires-Dist: dill==0.3.7
 Requires-Dist: cloudpickle==3.0.0
@@ -16,15 +16,15 @@
 Requires-Dist: opentelemetry-api<2,>=1.15.0
 Requires-Dist: opentelemetry-sdk<2,>=1.15.0
 Requires-Dist: grpc-interceptor<1,>=0.15.0
 Requires-Dist: colorama<1,>=0.4.6
 Requires-Dist: portalocker<3,>=2.7.0
 Requires-Dist: rich<14,>=13.3.2
 Requires-Dist: rich_argparse
-Requires-Dist: packaging<22,>=21.3
+Requires-Dist: packaging>=21.3
 Requires-Dist: pathspec<1,>=0.11.1
 Requires-Dist: pydantic!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,<3
 Requires-Dist: fastapi<1,>=0.99.1
 Requires-Dist: starlette-exporter>=0.21.0
 Requires-Dist: httpx>=0.15.4
 Requires-Dist: attrs>=21.3.0
 Requires-Dist: python-dateutil<3,>=2.8.0
```

### Comparing `fal-1.0.2/fal.egg-info/SOURCES.txt` & `fal-1.0.3/fal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/fal.egg-info/requires.txt` & `fal-1.0.3/fal.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 opentelemetry-api<2,>=1.15.0
 opentelemetry-sdk<2,>=1.15.0
 grpc-interceptor<1,>=0.15.0
 colorama<1,>=0.4.6
 portalocker<3,>=2.7.0
 rich<14,>=13.3.2
 rich_argparse
-packaging<22,>=21.3
+packaging>=21.3
 pathspec<1,>=0.11.1
 pydantic!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,<3
 fastapi<1,>=0.99.1
 starlette-exporter>=0.21.0
 httpx>=0.15.4
 attrs>=21.3.0
 python-dateutil<3,>=2.8.0
```

### Comparing `fal-1.0.2/openapi-fal-rest/README.md` & `fal-1.0.3/openapi-fal-rest/README.md`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/applications/app_metadata.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/applications/app_metadata.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/billing/get_user_details.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/billing/get_user_details.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/files/check_dir_hash.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/files/check_dir_hash.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/files/upload_local_file.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/files/upload_local_file.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/workflows/create_or_update_workflow_workflows_post.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/workflows/create_or_update_workflow_workflows_post.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/workflows/delete_workflow_workflows_user_id_workflow_name_delete.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/workflows/delete_workflow_workflows_user_id_workflow_name_delete.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/workflows/execute_workflow_workflows_user_id_workflow_name_post.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/workflows/execute_workflow_workflows_user_id_workflow_name_post.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflow_workflows_user_id_workflow_name_get.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflow_workflows_user_id_workflow_name_get.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflows_workflows_get.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflows_workflows_get.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/client.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/client.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/__init__.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/app_metadata_response_app_metadata.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/app_metadata_response_app_metadata.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/body_upload_local_file.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/body_upload_local_file.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/customer_details.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/customer_details.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_json_body_type_0.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_json_body_type_0.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_response_200_type_0.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_response_200_type_0.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/hash_check.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/hash_check.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/http_validation_error.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/lock_reason.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/lock_reason.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/page_workflow_item.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/page_workflow_item.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/typed_workflow.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/typed_workflow.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/validation_error.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_contents.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_contents.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_nodes.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_nodes.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_output.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_output.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_detail.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_detail.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_detail_contents_type_0.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_detail_contents_type_0.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_item.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_item.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_node.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_node.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_schema.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_schema.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_input.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_input.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_output.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_output.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/openapi_fal_rest/types.py` & `fal-1.0.3/openapi-fal-rest/openapi_fal_rest/types.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/openapi-fal-rest/pyproject.toml` & `fal-1.0.3/openapi-fal-rest/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/pyproject.toml` & `fal-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 include = ["fal", "openapi_fal_rest"]
 namespaces = false
 
 [project]
 name = "fal"
 dynamic = ["version"]
 description = "fal is an easy-to-use Serverless Python Framework"
-authors = [{ name = "Features & Labels <hello@fal.ai>"}]
+authors = [{ name = "Features & Labels <support@fal.ai>"}]
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "isolate[build]>=0.12.3,<1.0",
     "isolate-proto==0.4.0",
     "grpcio>=1.50.0,<2",
     "dill==0.3.7",
@@ -33,15 +33,15 @@
     "opentelemetry-api>=1.15.0,<2",
     "opentelemetry-sdk>=1.15.0,<2",
     "grpc-interceptor>=0.15.0,<1",
     "colorama>=0.4.6,<1",
     "portalocker>=2.7.0,<3",
     "rich>=13.3.2,<14",
     "rich_argparse",
-    "packaging>=21.3,<22",
+    "packaging>=21.3",
     "pathspec>=0.11.1,<1",
     "pydantic!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,<3",
     # serve=True dependencies
     "fastapi>=0.99.1,<1",
     "starlette-exporter>=0.21.0",
     # rest-api-client dependencies
     "httpx>=0.15.4",
```

### Comparing `fal-1.0.2/src/fal/__init__.py` & `fal-1.0.3/src/fal/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/_serialization.py` & `fal-1.0.3/src/fal/_serialization.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/api.py` & `fal-1.0.3/src/fal/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,14 @@
                     )
                 elif e.details().endswith("died with <Signals.SIGKILL: 9>.`."):
                     raise FalServerlessError(
                         "Isolated function crashed. "
                         "This is likely due to resource overflow. "
                         "You can try again by setting a bigger `machine_type`"
                     )
-
                 elif e.code() == grpc.StatusCode.INVALID_ARGUMENT and (
                     "The function function could not be deserialized" in e.details()
                 ):
                     raise FalMissingDependencyError(e.details()) from None
                 else:
                     raise FalServerlessError(e.details())
```

### Comparing `fal-1.0.2/src/fal/app.py` & `fal-1.0.3/src/fal/app.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/apps.py` & `fal-1.0.3/src/fal/apps.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/auth/__init__.py` & `fal-1.0.3/src/fal/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/auth/auth0.py` & `fal-1.0.3/src/fal/auth/auth0.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/auth/local.py` & `fal-1.0.3/src/fal/auth/local.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/cli/apps.py` & `fal-1.0.3/src/fal/cli/apps.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/cli/auth.py` & `fal-1.0.3/src/fal/cli/auth.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/cli/debug.py` & `fal-1.0.3/src/fal/cli/debug.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/cli/deploy.py` & `fal-1.0.3/src/fal/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/cli/keys.py` & `fal-1.0.3/src/fal/cli/keys.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/cli/main.py` & `fal-1.0.3/src/fal/cli/main.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/cli/parser.py` & `fal-1.0.3/src/fal/cli/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,24 +47,47 @@
                 )
             key, value = parts
             d[key] = value
 
         setattr(args, self.dest, d)
 
 
+def _find_parser(parser, func):
+    defaults = parser._defaults
+    if not func or func == defaults.get("func"):
+        return parser
+
+    actions = parser._actions
+    for action in actions:
+        if not isinstance(action.choices, dict):
+            continue
+        for subparser in action.choices.values():
+            par = _find_parser(subparser, func)
+            if par:
+                return par
+    return None
+
+
 class FalParser(argparse.ArgumentParser):
     def __init__(self, *args, **kwargs):
         kwargs.setdefault("formatter_class", rich_argparse.RawTextRichHelpFormatter)
         super().__init__(*args, **kwargs)
 
     def exit(self, status=0, message=None):
         if message:
             self._print_message(message, sys.stderr)
         raise FalParserExit(status)
 
+    def parse_args(self, args=None, namespace=None):
+        args, argv = self.parse_known_args(args, namespace)
+        if argv:
+            parser = _find_parser(self, getattr(args, "func", None)) or self
+            parser.error("unrecognized arguments: %s" % " ".join(argv))
+        return args
+
 
 class FalClientParser(FalParser):
     def __init__(self, *args, **kwargs):
         from fal.flags import GRPC_HOST
 
         super().__init__(*args, **kwargs)
         self.add_argument(
```

### Comparing `fal-1.0.2/src/fal/cli/run.py` & `fal-1.0.3/src/fal/cli/run.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/cli/secrets.py` & `fal-1.0.3/src/fal/cli/secrets.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/flags.py` & `fal-1.0.3/src/fal/flags.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/logging/__init__.py` & `fal-1.0.3/src/fal/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/logging/isolate.py` & `fal-1.0.3/src/fal/logging/isolate.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/logging/trace.py` & `fal-1.0.3/src/fal/logging/trace.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/logging/user.py` & `fal-1.0.3/src/fal/logging/user.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/rest_client.py` & `fal-1.0.3/src/fal/rest_client.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/sdk.py` & `fal-1.0.3/src/fal/sdk.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/sync.py` & `fal-1.0.3/src/fal/sync.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/toolkit/__init__.py` & `fal-1.0.3/src/fal/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/toolkit/file/file.py` & `fal-1.0.3/src/fal/toolkit/file/file.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/toolkit/file/providers/fal.py` & `fal-1.0.3/src/fal/toolkit/file/providers/fal.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/toolkit/file/providers/gcp.py` & `fal-1.0.3/src/fal/toolkit/file/providers/gcp.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/toolkit/file/providers/r2.py` & `fal-1.0.3/src/fal/toolkit/file/providers/r2.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/toolkit/file/types.py` & `fal-1.0.3/src/fal/toolkit/file/types.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/toolkit/image/image.py` & `fal-1.0.3/src/fal/toolkit/image/image.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/toolkit/optimize.py` & `fal-1.0.3/src/fal/toolkit/optimize.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/src/fal/toolkit/utils/download_utils.py` & `fal-1.0.3/src/fal/toolkit/utils/download_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import hashlib
 import shutil
 import subprocess
 import sys
-from functools import lru_cache
 from pathlib import Path, PurePath
 from tempfile import TemporaryDirectory
 from urllib.parse import urlparse
 from urllib.request import Request, urlopen
 
 FAL_PERSISTENT_DIR = PurePath("/data")
 FAL_REPOSITORY_DIR = FAL_PERSISTENT_DIR / ".fal" / "repos"
@@ -36,16 +35,18 @@
 
     Returns:
         A string representing the hashed URL.
     """
     return hashlib.sha256(url.encode("utf-8")).hexdigest()
 
 
-@lru_cache
-def _get_remote_file_properties(url: str) -> tuple[str, int]:
+def _get_remote_file_properties(
+    url: str,
+    request_headers: dict[str, str] | None = None,
+) -> tuple[str, int]:
     """Retrieves the file name and content length of a remote file.
 
     This function sends an HTTP request to the remote URL and retrieves the
     "Content-Disposition" header and the "Content-Length" header from the response.
     The "Content-Disposition" header contains the file name of the remote file, while
     the "Content-Length" header contains the expected content length of the remote
     file.
@@ -56,19 +57,23 @@
     uses it as the file name.
 
     If the "Content-Length" header is not available, the function returns -1 as the
     content length.
 
     Args:
         url: The URL of the remote file.
+        request_headers: A dictionary containing additional headers to be included in
+            the HTTP request.
 
     Returns:
         A tuple containing the file name and the content length of the remote file.
     """
-    request = Request(url, headers=TEMP_HEADERS)
+    headers = {**TEMP_HEADERS, **(request_headers or {})}
+    request = Request(url, headers=headers)
+
     with urlopen(request) as response:
         file_name = response.headers.get_filename()
         content_length = int(response.headers.get("Content-Length", -1))
 
     if not file_name:
         parsed_url = urlparse(url)
 
@@ -77,44 +82,49 @@
         else:
             url_path = parsed_url.path
             file_name = Path(url_path).name or _hash_url(url)
 
     return file_name, content_length
 
 
-def _file_content_length_matches(url: str, file_path: Path) -> bool:
+def _file_content_length_matches(
+    url: str, file_path: Path, request_headers: dict[str, str] | None = None
+) -> bool:
     """Check if the local file's content length matches the expected remote
     file's content length.
 
     This function compares the content length of a local file to the expected content
     length of a remote file, which is determined by sending an HTTP request to the
     remote URL. If the content lengths match, the function returns `True`, indicating
     that the local file's content matches the expected remote content. If the content
     lengths do not match or information about the content length is unavailable, the
     function returns `False`.
 
     Args:
         url: The URL of the remote file.
         file_path: The local path to the file being compared.
+        request_headers: A dictionary containing additional headers to be included in
+            the HTTP request.
 
     Returns:
         bool: `True` if the local file's content length matches the remote file's
             content length, `False` otherwise.
     """
     local_file_content_length = file_path.stat().st_size
-    remote_file_content_length = _get_remote_file_properties(url)[1]
+    remote_file_content_length = _get_remote_file_properties(url, request_headers)[1]
 
     return local_file_content_length == remote_file_content_length
 
 
 def download_file(
     url: str,
     target_dir: str | Path,
     *,
     force: bool = False,
+    request_headers: dict[str, str] | None = None,
 ) -> Path:
     """Downloads a file from the specified URL to the target directory.
 
     The function downloads the file from the given URL and saves it in the specified
     target directory.
 
     It also checks whether the local file already exists and whether its content length
@@ -130,84 +140,100 @@
     Parameters:
         url: The URL of the file to be downloaded.
         target_dir: The directory where the downloaded file will be saved. If it's not
             an absolute path, it's treated as a relative directory to "/data".
         force: If `True`, the file is downloaded even if it already exists locally and
             its content length matches the expected content length from the remote file.
             Defaults to `False`.
+        request_headers: A dictionary containing additional headers to be included in
+            the HTTP request. Defaults to `None`.
+
 
     Returns:
         A Path object representing the full path to the downloaded file.
 
     Raises:
         ValueError: If the provided `file_name` contains a forward slash ('/').
         DownloadError: If an error occurs during the download process.
     """
-    file_name = _get_remote_file_properties(url)[0]
+    try:
+        file_name = _get_remote_file_properties(url, request_headers)[0]
+    except Exception as e:
+        raise DownloadError(f"Failed to get remote file properties for {url}") from e
+
     if "/" in file_name:
         raise ValueError(f"File name '{file_name}' cannot contain a slash.")
 
     target_dir_path = Path(target_dir)
 
     # If target_dir is not an absolute path, use "/data" as the relative directory
     if not target_dir_path.is_absolute():
         target_dir_path = Path(FAL_PERSISTENT_DIR / target_dir_path)  # type: ignore[assignment]
 
     target_path = target_dir_path.resolve() / file_name
 
     if (
         target_path.exists()
-        and _file_content_length_matches(url, target_path)
+        and _file_content_length_matches(url, target_path, request_headers)
         and not force
     ):
         return target_path
 
     if force:
         print(f"File already exists. Forcing download of {url} to {target_path}")
     else:
         print(f"Downloading {url} to {target_path}")
 
     # Make sure the directory exists
     target_path.parent.mkdir(parents=True, exist_ok=True)
 
     try:
-        _download_file_python(url=url, target_path=target_path)
+        _download_file_python(
+            url=url, target_path=target_path, request_headers=request_headers
+        )
     except Exception as e:
         msg = f"Failed to download {url} to {target_path}"
 
         target_path.unlink(missing_ok=True)
 
         raise DownloadError(msg) from e
 
     return target_path
 
 
-def _download_file_python(url: str, target_path: Path | str) -> Path:
+def _download_file_python(
+    url: str, target_path: Path | str, request_headers: dict[str, str] | None = None
+) -> Path:
     """Download a file from a given URL and save it to a specified path using a
     Python interface.
 
     Args:
         url: The URL of the file to be downloaded.
         target_path: The path where the downloaded file will be saved.
+        request_headers: A dictionary containing additional headers to be included in
+            the HTTP request. Defaults to `None`.
 
     Returns:
         The path where the downloaded file has been saved.
     """
     import shutil
     import tempfile
 
     with tempfile.NamedTemporaryFile(delete=False) as temp_file:
         try:
             file_path = temp_file.name
 
-            for (progress, total_size) in _stream_url_data_to_file(url, temp_file.name):
+            for progress, total_size in _stream_url_data_to_file(
+                url, temp_file.name, request_headers=request_headers
+            ):
                 if total_size:
                     progress_msg = f"Downloading {url} ... {progress:.2%}"
                 else:
                     progress_msg = f"Downloading {url} ... {progress:.2f} MB"
+
                 print(progress_msg, end="\r\n")
 
             # Move the file when the file is downloaded completely. Since the
             # file used is temporary, in a case of an interruption, the downloaded
             # content will be lost. So, it is safe to redownload the file in such cases.
             shutil.move(file_path, target_path)
 
@@ -215,40 +241,48 @@
             raise error
         finally:
             Path(temp_file.name).unlink(missing_ok=True)
 
     return Path(target_path)
 
 
-def _stream_url_data_to_file(url: str, file_path: str, chunk_size_in_mb: int = 64):
+def _stream_url_data_to_file(
+    url: str,
+    file_path: str,
+    chunk_size_in_mb: int = 64,
+    request_headers: dict[str, str] | None = None,
+):
     """Download data from a URL and stream it to a file.
 
     Note:
         - This function sets a User-Agent header to mimic a web browser to
             prevent issues with some websites.
         - It downloads the file in chunks to save memory and ensures the file
             is only moved when the download is complete.
 
     Args:
         request: The Request object representing the URL to download from.
         file_path: The path to the file where the downloaded data will be saved.
         chunk_size_in_mb: The size of each download chunk in megabytes.
             Defaults to 64.
+        request_headers: A dictionary containing additional headers to be included in
+            the HTTP request. Defaults to `None`.
 
     Yields:
         A tuple containing two elements:
         - float: The progress of the download as a percentage (0.0 to 1.0) if
             the total size is known. Else, equals to the downloaded size in MB.
         - int: The total size of the downloaded content in bytes. If the total
             size is not known (e.g., the server doesn't provide a
             'content-length' header), the second element is 0.
     """
     ONE_MB = 1024**2
 
-    request = Request(url, headers=TEMP_HEADERS)
+    headers = {**TEMP_HEADERS, **(request_headers or {})}
+    request = Request(url, headers=headers)
 
     received_size = 0
     total_size = 0
 
     with urlopen(request) as response, open(file_path, "wb") as f_stream:
         total_size = int(response.headers.get("content-length", total_size))
         while data := response.read(chunk_size_in_mb * ONE_MB):
@@ -263,15 +297,17 @@
             yield progress, total_size
 
     # Check if received size matches the expected total size
     if total_size and received_size < total_size:
         raise DownloadError("Received less data than expected from the server.")
 
 
-def download_model_weights(url: str, force: bool = False):
+def download_model_weights(
+    url: str, force: bool = False, request_headers: dict[str, str] | None = None
+) -> Path:
     """Downloads model weights from the specified URL and saves them to a
     predefined directory.
 
     This function is specifically designed for downloading model weights and stores
     them in a predefined directory.
 
     It calls the `download_file` function with the provided
@@ -280,14 +316,16 @@
     the full path to the downloaded weights file.
 
     Args:
         url: The URL from which the model weights will be downloaded.
         force: If `True`, the model weights are downloaded even if they already exist
             locally and their content length matches the expected content length from
             the remote file. Defaults to `False`.
+        request_headers: A dictionary containing additional headers to be included in
+            the HTTP request. Defaults to `None`.
 
     Returns:
         A Path object representing the full path to the downloaded model weights.
     """
     # This is not a protected path, so the user may change stuff internally
     weights_dir = Path(FAL_MODEL_WEIGHTS_DIR / _hash_url(url))
 
@@ -299,14 +337,15 @@
         except StopIteration:
             pass
 
     return download_file(
         url,
         target_dir=weights_dir,
         force=force,
+        request_headers=request_headers,
     )
 
 
 def clone_repository(
     https_url: str,
     *,
     commit_hash: str | None = None,
```

### Comparing `fal-1.0.2/src/fal/utils.py` & `fal-1.0.3/src/fal/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
                 "Please specify the name of the app."
             )
 
         [(app_name, function_name)] = fal_objects.items()
     else:
         app_name = None
 
-    module = runpy.run_path(file_path)
     if function_name not in module:
         raise FalServerlessError(f"Function '{function_name}' not found in module")
 
     # The module for the function is set to <run_path> when runpy is used, in which
     # case we want to manually include the package it is defined in.
     fal._serialization.include_package_from_path(file_path)
```

### Comparing `fal-1.0.2/src/fal/workflows.py` & `fal-1.0.3/src/fal/workflows.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/tests/cli/test_apps.py` & `fal-1.0.3/tests/cli/test_apps.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/tests/cli/test_keys.py` & `fal-1.0.3/tests/cli/test_keys.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/tests/integration_test.py` & `fal-1.0.3/tests/integration_test.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/tests/test_apps.py` & `fal-1.0.3/tests/test_apps.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,14 @@
         print("sleeping...")
         time.sleep(1)
 
     return Output(result=input.lhs + input.rhs)
 
 
 nomad_addition_app = addition_app.on(_scheduler="nomad")
-kubernetes_addition_app = addition_app.on(_scheduler="kubernetes")
-
 
 @fal.function(
     keep_alive=300,
     requirements=["fastapi", "uvicorn", "pydantic==1.10.12"],
     machine_type="S",
     max_concurrency=1,
     max_multiplexing=30,
@@ -200,28 +198,14 @@
         options=nomad_addition_app.options,
     )
     user_id = _get_user_id()
     yield f"{user_id}/{app_revision}"
 
 
 @pytest.fixture(scope="module")
-def test_kubernetes_app():
-    # Create a temporary app, register it, and return the ID of it.
-
-    from fal.cli.deploy import _get_user_id
-
-    app_revision = kubernetes_addition_app.host.register(
-        func=nomad_addition_app.func,
-        options=kubernetes_addition_app.options,
-    )
-    user_id = _get_user_id()
-    yield f"{user_id}/{app_revision}"
-
-
-@pytest.fixture(scope="module")
 def test_fastapi_app():
     # Create a temporary app, register it, and return the ID of it.
 
     from fal.cli.deploy import _get_user_id
 
     app_revision = calculator_app.host.register(
         func=calculator_app.func,
@@ -422,15 +406,15 @@
         )
         assert res.alias == app_alias
         assert res.keep_alive == new_keep_alive
         assert res.max_concurrency == new_max_concurrency
         assert res.max_multiplexing == new_max_multiplexing
 
     with host._connection as client:
-        new_max_concurrency = new_max_concurrency + 1
+        new_max_concurrency = new_max_concurrency - 1
         res = client.update_application(
             application_name=app_alias,
             max_concurrency=new_max_concurrency,
         )
         assert res.alias == app_alias
         assert res.keep_alive == new_keep_alive
         assert res.max_concurrency == new_max_concurrency
```

### Comparing `fal-1.0.2/tests/test_stability.py` & `fal-1.0.3/tests/test_stability.py`

 * *Files 4% similar despite different names*

```diff
@@ -371,30 +371,14 @@
     # (no mix and match between arguments and the returned
     # future).
     assert future_2.result() == 4
     assert future_3.result() == 6
     assert future_4.result() == 8
 
 
-def test_conda_environment(isolated_client):
-    @isolated_client(
-        "conda",
-        packages=["pyjokes=0.6.0"],
-        machine_type="L",
-        # conda is only supported on Kubernetes
-        _scheduler="kubernetes",
-    )
-    def regular_function():
-        import pyjokes
-
-        return pyjokes.__version__
-
-    assert regular_function() == "0.6.0"
-
-
 @pytest.mark.xfail(reason="Nomad does not support conda")
 def test_conda_environment_on_nomad(isolated_client):
     @isolated_client(
         "conda",
         packages=["pyjokes=0.6.0"],
         machine_type="L",
         # conda is only supported on Kubernetes
@@ -404,14 +388,15 @@
         import pyjokes
 
         return pyjokes.__version__
 
     assert regular_function() == "0.6.0"
 
 
+@pytest.mark.xfail(reason="Broken on nomad")
 def test_cached_function(isolated_client, capsys, monkeypatch):
     import inspect
     import time
 
     test_stamp = time.time()
     real_getsource = inspect.getsource
 
@@ -440,15 +425,14 @@
         return math.factorial(n)
 
     # make sure this machine is not shared with others by using a unique requirements
     @isolated_client(
         "virtualenv",
         keep_alive=30,
         requirements=["pyjokes     "],
-        _scheduler="kubernetes",
     )
     def regular_function(n):
         if get_pipe() == "pipe":
             return factorial(n)
 
     assert regular_function(4) == 24
     out, err = capsys.readouterr()
```

### Comparing `fal-1.0.2/tests/toolkit/file_test.py` & `fal-1.0.3/tests/toolkit/file_test.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.2/tests/toolkit/image_test.py` & `fal-1.0.3/tests/toolkit/image_test.py`

 * *Files identical despite different names*

