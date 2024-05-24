# Comparing `tmp/aioli_sdk-0.2.4.dev6.tar.gz` & `tmp/aioli_sdk-0.2.4.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioli_sdk-0.2.4.dev6.tar", last modified: Wed May 22 22:44:25 2024, max compression
+gzip compressed data, was "aioli_sdk-0.2.4.dev7.tar", last modified: Thu May 23 07:13:15 2024, max compression
```

## Comparing `aioli_sdk-0.2.4.dev6.tar` & `aioli_sdk-0.2.4.dev7.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 22:44:25.269115 aioli_sdk-0.2.4.dev6/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-05-22 22:44:25.269115 aioli_sdk-0.2.4.dev6/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 22:44:25.265115 aioli_sdk-0.2.4.dev6/aioli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/__version__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 22:44:25.265115 aioli_sdk-0.2.4.dev6/aioli/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/cli/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/cli/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8497 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/cli/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13159 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/cli/deployment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/cli/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14935 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/cli/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8210 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/cli/registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7221 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/cli/render.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/cli/role.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5304 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/cli/sso.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 22:44:25.265115 aioli_sdk-0.2.4.dev6/aioli/cli/test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/cli/test/conftest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31029 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/cli/test/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6629 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/cli/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3103 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/cli/version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 22:44:25.265115 aioli_sdk-0.2.4.dev6/aioli/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/common/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 22:44:25.265115 aioli_sdk-0.2.4.dev6/aioli/common/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/common/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/common/api/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18000 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/common/api/authentication.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8098 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/common/api/certs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3671 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/common/api/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10969 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/common/api/request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8655 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/common/check.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/common/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8480 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/common/declarative_argparse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/common/requests.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4706 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/common/util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/aioli/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 22:44:25.269115 aioli_sdk-0.2.4.dev6/aioli_sdk.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-05-22 22:44:25.000000 aioli_sdk-0.2.4.dev6/aioli_sdk.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2482 2024-05-22 22:44:25.000000 aioli_sdk-0.2.4.dev6/aioli_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-22 22:44:25.000000 aioli_sdk-0.2.4.dev6/aioli_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-05-22 22:44:25.000000 aioli_sdk-0.2.4.dev6/aioli_sdk.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-22 22:44:23.000000 aioli_sdk-0.2.4.dev6/aioli_sdk.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-05-22 22:44:25.000000 aioli_sdk-0.2.4.dev6/aioli_sdk.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-05-22 22:44:25.000000 aioli_sdk-0.2.4.dev6/aioli_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 22:44:25.265115 aioli_sdk-0.2.4.dev6/aiolirest/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3218 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 22:44:25.269115 aioli_sdk-0.2.4.dev6/aiolirest/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22813 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/api/authentication_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    84659 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/api/deployments_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10515 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/api/information_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    91193 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/api/packaged_models_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    66586 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/api/registries_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43082 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/api/roles_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   105944 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/api/templates_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    61885 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/api/users_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25050 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/api_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14926 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/configuration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5597 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/exceptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 22:44:25.269115 aioli_sdk-0.2.4.dev6/aiolirest/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2280 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3384 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/auto_scaling_template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3986 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/autoscaling.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3662 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/configuration_resources.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7356 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/deployment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4309 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/deployment_model_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5068 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/deployment_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5091 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/deployment_state.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/error_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3775 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/event_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3261 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/failure_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2642 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/login_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/login_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2820 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/model_auth_token.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4130 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/model_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2970 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/observability.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6263 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/packaged_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5740 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/packaged_model_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2940 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/resource_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3366 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/resources_template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2747 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/role.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2836 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/role_assignment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3296 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/role_assignments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/security.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2649 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/success_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5468 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/trained_model_registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5294 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/trained_model_registry_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2663 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/user_patch_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3387 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/models/user_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/py.typed
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8440 2024-05-22 22:44:21.000000 aioli_sdk-0.2.4.dev6/aiolirest/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-22 22:44:25.269115 aioli_sdk-0.2.4.dev6/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2024-05-22 22:39:07.000000 aioli_sdk-0.2.4.dev6/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 07:13:15.466131 aioli_sdk-0.2.4.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-05-23 07:13:15.466131 aioli_sdk-0.2.4.dev7/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 07:13:15.458131 aioli_sdk-0.2.4.dev7/aioli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/__version__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 07:13:15.458131 aioli_sdk-0.2.4.dev7/aioli/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/cli/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/cli/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8497 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/cli/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13159 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/cli/deployment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/cli/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14935 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/cli/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8210 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/cli/registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7221 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/cli/render.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/cli/role.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5304 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/cli/sso.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 07:13:15.458131 aioli_sdk-0.2.4.dev7/aioli/cli/test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/cli/test/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31029 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/cli/test/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6629 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/cli/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3103 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/cli/version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 07:13:15.458131 aioli_sdk-0.2.4.dev7/aioli/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/common/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 07:13:15.458131 aioli_sdk-0.2.4.dev7/aioli/common/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/common/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/common/api/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18000 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/common/api/authentication.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8098 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/common/api/certs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3671 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/common/api/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10969 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/common/api/request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8655 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/common/check.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/common/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8480 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/common/declarative_argparse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/common/requests.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4706 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/common/util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/aioli/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 07:13:15.466131 aioli_sdk-0.2.4.dev7/aioli_sdk.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-05-23 07:13:15.000000 aioli_sdk-0.2.4.dev7/aioli_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2482 2024-05-23 07:13:15.000000 aioli_sdk-0.2.4.dev7/aioli_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-23 07:13:15.000000 aioli_sdk-0.2.4.dev7/aioli_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-05-23 07:13:15.000000 aioli_sdk-0.2.4.dev7/aioli_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-23 07:13:13.000000 aioli_sdk-0.2.4.dev7/aioli_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-05-23 07:13:15.000000 aioli_sdk-0.2.4.dev7/aioli_sdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-05-23 07:13:15.000000 aioli_sdk-0.2.4.dev7/aioli_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 07:13:15.462131 aioli_sdk-0.2.4.dev7/aiolirest/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3218 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 07:13:15.462131 aioli_sdk-0.2.4.dev7/aiolirest/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22813 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/api/authentication_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    84659 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/api/deployments_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10515 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/api/information_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    91193 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/api/packaged_models_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    66586 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/api/registries_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43082 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/api/roles_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   105944 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/api/templates_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    61885 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/api/users_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25050 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/api_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14926 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/configuration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5597 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/exceptions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 07:13:15.462131 aioli_sdk-0.2.4.dev7/aiolirest/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2280 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3384 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/auto_scaling_template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3986 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/autoscaling.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3662 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/configuration_resources.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7356 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/deployment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4309 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/deployment_model_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5068 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/deployment_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5091 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/deployment_state.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/error_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3775 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/event_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3261 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/failure_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2642 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/login_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/login_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2820 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/model_auth_token.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4130 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/model_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2970 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/observability.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6263 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/packaged_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5740 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/packaged_model_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2940 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/resource_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3366 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/resources_template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2747 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/role.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2836 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/role_assignment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3296 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/role_assignments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/security.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2649 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/success_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5468 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/trained_model_registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5294 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/trained_model_registry_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2663 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/user_patch_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3387 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/models/user_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/py.typed
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8440 2024-05-23 07:13:11.000000 aioli_sdk-0.2.4.dev7/aiolirest/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-23 07:13:15.466131 aioli_sdk-0.2.4.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2024-05-23 07:07:51.000000 aioli_sdk-0.2.4.dev7/setup.py
```

### Comparing `aioli_sdk-0.2.4.dev6/PKG-INFO` & `aioli_sdk-0.2.4.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.2.4.dev6
+Version: 0.2.4.dev7
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli_sdk-0.2.4.dev6/aioli/cli/_util.py` & `aioli_sdk-0.2.4.dev7/aioli/cli/_util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/cli/cli.py` & `aioli_sdk-0.2.4.dev7/aioli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/cli/deployment.py` & `aioli_sdk-0.2.4.dev7/aioli/cli/deployment.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/cli/errors.py` & `aioli_sdk-0.2.4.dev7/aioli/cli/errors.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/cli/model.py` & `aioli_sdk-0.2.4.dev7/aioli/cli/model.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/cli/registry.py` & `aioli_sdk-0.2.4.dev7/aioli/cli/registry.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/cli/render.py` & `aioli_sdk-0.2.4.dev7/aioli/cli/render.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/cli/role.py` & `aioli_sdk-0.2.4.dev7/aioli/cli/role.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/cli/sso.py` & `aioli_sdk-0.2.4.dev7/aioli/cli/sso.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/cli/test/conftest.py` & `aioli_sdk-0.2.4.dev7/aioli/cli/test/conftest.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/cli/test/test_cli.py` & `aioli_sdk-0.2.4.dev7/aioli/cli/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/cli/user.py` & `aioli_sdk-0.2.4.dev7/aioli/cli/user.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/cli/version.py` & `aioli_sdk-0.2.4.dev7/aioli/cli/version.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/common/api/authentication.py` & `aioli_sdk-0.2.4.dev7/aioli/common/api/authentication.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/common/api/certs.py` & `aioli_sdk-0.2.4.dev7/aioli/common/api/certs.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/common/api/errors.py` & `aioli_sdk-0.2.4.dev7/aioli/common/api/errors.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/common/api/request.py` & `aioli_sdk-0.2.4.dev7/aioli/common/api/request.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/common/check.py` & `aioli_sdk-0.2.4.dev7/aioli/common/check.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/common/constants.py` & `aioli_sdk-0.2.4.dev7/aioli/common/constants.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/common/declarative_argparse.py` & `aioli_sdk-0.2.4.dev7/aioli/common/declarative_argparse.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/common/requests.py` & `aioli_sdk-0.2.4.dev7/aioli/common/requests.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/common/util.py` & `aioli_sdk-0.2.4.dev7/aioli/common/util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli/util.py` & `aioli_sdk-0.2.4.dev7/aioli/util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aioli_sdk.egg-info/PKG-INFO` & `aioli_sdk-0.2.4.dev7/aioli_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.2.4.dev6
+Version: 0.2.4.dev7
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli_sdk-0.2.4.dev6/aioli_sdk.egg-info/SOURCES.txt` & `aioli_sdk-0.2.4.dev7/aioli_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/__init__.py` & `aioli_sdk-0.2.4.dev7/aiolirest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/api/authentication_api.py` & `aioli_sdk-0.2.4.dev7/aiolirest/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/api/deployments_api.py` & `aioli_sdk-0.2.4.dev7/aiolirest/api/deployments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/api/information_api.py` & `aioli_sdk-0.2.4.dev7/aiolirest/api/information_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/api/packaged_models_api.py` & `aioli_sdk-0.2.4.dev7/aiolirest/api/packaged_models_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/api/registries_api.py` & `aioli_sdk-0.2.4.dev7/aiolirest/api/registries_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/api/roles_api.py` & `aioli_sdk-0.2.4.dev7/aiolirest/api/roles_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/api/templates_api.py` & `aioli_sdk-0.2.4.dev7/aiolirest/api/templates_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/api/users_api.py` & `aioli_sdk-0.2.4.dev7/aiolirest/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/api_client.py` & `aioli_sdk-0.2.4.dev7/aiolirest/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/api_response.py` & `aioli_sdk-0.2.4.dev7/aiolirest/api_response.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/configuration.py` & `aioli_sdk-0.2.4.dev7/aiolirest/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -385,15 +385,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.2.4-dev6\n"\
+               "Version of the API: 0.2.4-dev7\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/exceptions.py` & `aioli_sdk-0.2.4.dev7/aiolirest/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/__init__.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/auto_scaling_template.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/auto_scaling_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/autoscaling.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/autoscaling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/configuration_resources.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/configuration_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/deployment.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/deployment_model_version.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/deployment_model_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/deployment_request.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/deployment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/deployment_state.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/deployment_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/error_response.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/error_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/event_info.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/event_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/failure_info.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/failure_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/login_request.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/login_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/login_response.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/login_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/model_auth_token.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/model_auth_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/model_response.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/model_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/observability.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/observability.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/packaged_model.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/packaged_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/packaged_model_request.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/packaged_model_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/resource_profile.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/resource_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/resources_template.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/resources_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/role.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/role_assignment.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/role_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/role_assignments.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/role_assignments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/security.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/security.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/success_response.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/success_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/trained_model_registry.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/trained_model_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/trained_model_registry_request.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/trained_model_registry_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/user.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/user_patch_request.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/user_patch_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/models/user_request.py` & `aioli_sdk-0.2.4.dev7/aiolirest/models/user_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/aiolirest/rest.py` & `aioli_sdk-0.2.4.dev7/aiolirest/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev6
+    The version of the OpenAPI document: 0.2.4-dev7
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev6/setup.py` & `aioli_sdk-0.2.4.dev7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as readme:
     markdown_description = "".join(readme.readlines())
 
 setuptools.setup(
     name="aioli-sdk",
-    version="0.2.4-dev6",
+    version="0.2.4-dev7",
     author="HPE AI Solutions",
     # author_email="hello@determined.ai",
     url="https://github.com/determined-ai/aioli",
     description="Aioli (AI OnLine Inference), a platform for deploying AI models at scale.",
     long_description = markdown_description,
     long_description_content_type = "text/markdown",
     license="Apache License 2.0",
```

