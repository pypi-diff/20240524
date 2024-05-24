# Comparing `tmp/elvia-vault-0.5.0.tar.gz` & `tmp/elvia_vault-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elvia-vault-0.5.0.tar", last modified: Mon Oct 30 08:03:35 2023, max compression
+gzip compressed data, was "elvia_vault-0.5.1.tar", last modified: Fri May 24 12:21:22 2024, max compression
```

## Comparing `elvia-vault-0.5.0.tar` & `elvia_vault-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-30 08:03:35.313272 elvia-vault-0.5.0/
--rw-r--r--   0 vsts      (1001) docker     (127)      292 2023-10-30 08:03:35.313272 elvia-vault-0.5.0/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-30 08:03:35.313272 elvia-vault-0.5.0/elvia_vault/
--rw-r--r--   0 vsts      (1001) docker     (127)      267 2023-10-30 08:03:26.000000 elvia-vault-0.5.0/elvia_vault/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14408 2023-10-30 08:03:10.000000 elvia-vault-0.5.0/elvia_vault/vault_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-30 08:03:35.313272 elvia-vault-0.5.0/elvia_vault.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      292 2023-10-30 08:03:35.000000 elvia-vault-0.5.0/elvia_vault.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      266 2023-10-30 08:03:35.000000 elvia-vault-0.5.0/elvia_vault.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-10-30 08:03:35.000000 elvia-vault-0.5.0/elvia_vault.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       83 2023-10-30 08:03:35.000000 elvia-vault-0.5.0/elvia_vault.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       12 2023-10-30 08:03:35.000000 elvia-vault-0.5.0/elvia_vault.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      103 2023-10-30 08:03:10.000000 elvia-vault-0.5.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2023-10-30 08:03:10.000000 elvia-vault-0.5.0/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2023-10-30 08:03:35.317272 elvia-vault-0.5.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1379 2023-10-30 08:03:10.000000 elvia-vault-0.5.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 12:21:22.652469 elvia_vault-0.5.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)      292 2024-05-24 12:21:22.652469 elvia_vault-0.5.1/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 12:21:22.648469 elvia_vault-0.5.1/elvia_vault/
+-rw-r--r--   0 vsts      (1001) docker     (127)      267 2024-05-24 12:21:19.000000 elvia_vault-0.5.1/elvia_vault/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14901 2024-05-24 12:21:09.000000 elvia_vault-0.5.1/elvia_vault/vault_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 12:21:22.652469 elvia_vault-0.5.1/elvia_vault.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      292 2024-05-24 12:21:22.000000 elvia_vault-0.5.1/elvia_vault.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      266 2024-05-24 12:21:22.000000 elvia_vault-0.5.1/elvia_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-24 12:21:22.000000 elvia_vault-0.5.1/elvia_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       83 2024-05-24 12:21:22.000000 elvia_vault-0.5.1/elvia_vault.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       12 2024-05-24 12:21:22.000000 elvia_vault-0.5.1/elvia_vault.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      103 2024-05-24 12:21:09.000000 elvia_vault-0.5.1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-24 12:21:09.000000 elvia_vault-0.5.1/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-24 12:21:22.652469 elvia_vault-0.5.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1379 2024-05-24 12:21:09.000000 elvia_vault-0.5.1/setup.py
```

### Comparing `elvia-vault-0.5.0/elvia_vault/vault_client.py` & `elvia_vault-0.5.1/elvia_vault/vault_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 from datetime import datetime, timedelta
 from http.server import BaseHTTPRequestHandler, HTTPServer
 import hvac
 import kubernetes
 import jwt
 
 
+# pylint: disable=C0115
+class ValidationError(Exception):
+    pass
+
 # pylint: disable=too-few-public-methods
 class EnvVarNames:
     """Reduce hardcoding by collecting env var names in this class."""
 
     VAULT_ADDR = 'VAULT_ADDR'
     GITHUB_TOKEN = 'GITHUB_TOKEN'
     ROLE_ID = 'ROLE_ID'
@@ -47,14 +51,18 @@
             vault_addr = self._get_vault_addr(vault_addr)
             self._client, self._authenticate_func = self._use_vaulttoken_auth(vault_addr)
         elif EnvVarNames.GITHUB_TOKEN in os.environ:
             vault_addr = self._get_vault_addr(vault_addr)
             self._client, self._authenticate_func = self._use_github_auth(
                 vault_addr, github_token)
         else:
+            print("No explicit login method found. Defaulting to using Azure AD.", flush=True)
+            if os.getenv("GITHUB_ACTIONS") == "true":
+                # pylint: disable=c0301
+                raise ValidationError("When running in Github Actions, interactive Azure AD login is not supported. See https://elvia.atlassian.net/wiki/spaces/Utviklerhandbok/pages/71813759342/Hente+Vault+secrets+fra+Github+Actions.")
             vault_addr = self._get_vault_addr(vault_addr)
             self._client, self._authenticate_func = self._use_azuread_auth(vault_addr)
         self._authenticate_func(self._client)
 
     def get_value(self, secret_path: str) -> str:
         """Retrieve a secret value for a given secret path.
```

### Comparing `elvia-vault-0.5.0/setup.py` & `elvia_vault-0.5.1/setup.py`

 * *Files identical despite different names*

