# Comparing `tmp/fastapi_oidc_backend-0.4.0.tar.gz` & `tmp/fastapi_oidc_backend-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_oidc_backend-0.4.0.tar", max compression
+gzip compressed data, was "fastapi_oidc_backend-0.4.1.tar", max compression
```

## Comparing `fastapi_oidc_backend-0.4.0.tar` & `fastapi_oidc_backend-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1106 2024-05-17 11:42:33.371825 fastapi_oidc_backend-0.4.0/LICENSE
--rwxr-xr-x   0        0        0     1371 2024-05-17 11:42:33.371825 fastapi_oidc_backend-0.4.0/README.md
--rwxr-xr-x   0        0        0     1422 2024-05-17 11:42:33.371825 fastapi_oidc_backend-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 11:42:33.371825 fastapi_oidc_backend-0.4.0/src/fastapi_oidc_backend/__init__.py
--rw-r--r--   0        0        0      105 2024-05-17 11:42:33.371825 fastapi_oidc_backend-0.4.0/src/fastapi_oidc_backend/exceptions.py
--rw-r--r--   0        0        0     1521 2024-05-17 11:42:33.371825 fastapi_oidc_backend-0.4.0/src/fastapi_oidc_backend/models.py
--rwxr-xr-x   0        0        0     4665 2024-05-17 11:42:33.371825 fastapi_oidc_backend-0.4.0/src/fastapi_oidc_backend/security.py
--rw-r--r--   0        0        0     2705 1970-01-01 00:00:00.000000 fastapi_oidc_backend-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1106 2024-05-23 11:45:11.588076 fastapi_oidc_backend-0.4.1/LICENSE
+-rwxr-xr-x   0        0        0     1414 2024-05-23 11:45:11.588076 fastapi_oidc_backend-0.4.1/README.md
+-rwxr-xr-x   0        0        0     1422 2024-05-23 11:45:11.588076 fastapi_oidc_backend-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 11:45:11.592076 fastapi_oidc_backend-0.4.1/src/fastapi_oidc_backend/__init__.py
+-rw-r--r--   0        0        0      105 2024-05-23 11:45:11.592076 fastapi_oidc_backend-0.4.1/src/fastapi_oidc_backend/exceptions.py
+-rw-r--r--   0        0        0     1521 2024-05-23 11:45:11.592076 fastapi_oidc_backend-0.4.1/src/fastapi_oidc_backend/models.py
+-rwxr-xr-x   0        0        0     4581 2024-05-23 11:45:11.592076 fastapi_oidc_backend-0.4.1/src/fastapi_oidc_backend/security.py
+-rw-r--r--   0        0        0     2748 1970-01-01 00:00:00.000000 fastapi_oidc_backend-0.4.1/PKG-INFO
```

### Comparing `fastapi_oidc_backend-0.4.0/LICENSE` & `fastapi_oidc_backend-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_oidc_backend-0.4.0/README.md` & `fastapi_oidc_backend-0.4.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from pydantic import BaseModel
 
 from fastapi_oidc_backend.security import OidcResourceServer
 from fastapi_oidc_backend.models import JwtKwargs
 
 oidc_config = JwtKwargs(audience="myclient", issuer="http://localhost:8888/realms/myrealm")
 
-app = FastAPI(swagger_ui_init_oauth={"clientId": oidc_config.audience})
+app = FastAPI(swagger_ui_init_oauth={"clientId": oidc_config.audience, "usePkceWithAuthorizationCodeGrant": True})
 
 auth_scheme = OidcResourceServer(
     oidc_config,
     scheme_name="Keycloak",
 )
```

### Comparing `fastapi_oidc_backend-0.4.0/pyproject.toml` & `fastapi_oidc_backend-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-oidc-backend"
-version = "0.4.0"
+version = "0.4.1"
 description = "Build resource servers with FastAPI"
 authors = ["Felix Gustavsson <felix@0b1.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/BlackVoid/fastapi-oidc-backend"
 keywords = [ "fastapi", "authentication", "oidc", "openidconnect" ]
 classifiers = [
```

### Comparing `fastapi_oidc_backend-0.4.0/src/fastapi_oidc_backend/models.py` & `fastapi_oidc_backend-0.4.1/src/fastapi_oidc_backend/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_oidc_backend-0.4.0/src/fastapi_oidc_backend/security.py` & `fastapi_oidc_backend-0.4.1/src/fastapi_oidc_backend/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 from typing import List, Optional
 
 import httpx
 from fastapi import Request
 from fastapi.exceptions import HTTPException
 from fastapi.openapi.models import (
     OAuthFlowAuthorizationCode,
@@ -48,15 +47,14 @@
 
     async def load_configuration(self):
         """
         Required to run before it's fully initialized, can be run again to refresh endpoints and keys.
         If fetching fails on start a runtime error will be thrown, otherwse a regular Exception
         :return:
         """
-        logging.log(logging.WARN, "Hello")
         try:
             async with httpx.AsyncClient() as client:
                 self.well_known = await self.fetch_well_known(client)
                 self.jwks = await self.fetch_jwks(client, self.well_known)
         except Exception as e:
             if self.well_known and self.jwks:
                 raise OidcInitException("Failed to refresh OIDC configuration") from e
@@ -81,15 +79,14 @@
 
         if GrantType.PASSWORD in grant_types:
             self.flows.password = OAuthFlowPassword(tokenUrl=token_url)
 
         if GrantType.IMPLICIT in grant_types:
             self.flows.implicit = OAuthFlowImplicit(authorizationUrl=authz_url)
 
-        print(self.flows)
         self.model = OAuth2Model(flows=self.flows)
 
     async def fetch_well_known(self, client: "httpx.AsyncClient") -> dict:
         url = f"{self.oidc_config.issuer}/.well-known/openid-configuration"
 
         response = await client.get(url)
         response.raise_for_status()
```

### Comparing `fastapi_oidc_backend-0.4.0/PKG-INFO` & `fastapi_oidc_backend-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-oidc-backend
-Version: 0.4.0
+Version: 0.4.1
 Summary: Build resource servers with FastAPI
 Home-page: https://github.com/BlackVoid/fastapi-oidc-backend
 License: MIT
 Keywords: fastapi,authentication,oidc,openidconnect
 Author: Felix Gustavsson
 Author-email: felix@0b1.se
 Requires-Python: >=3.11.2,<4.0.0
@@ -60,15 +60,15 @@
 from pydantic import BaseModel
 
 from fastapi_oidc_backend.security import OidcResourceServer
 from fastapi_oidc_backend.models import JwtKwargs
 
 oidc_config = JwtKwargs(audience="myclient", issuer="http://localhost:8888/realms/myrealm")
 
-app = FastAPI(swagger_ui_init_oauth={"clientId": oidc_config.audience})
+app = FastAPI(swagger_ui_init_oauth={"clientId": oidc_config.audience, "usePkceWithAuthorizationCodeGrant": True})
 
 auth_scheme = OidcResourceServer(
     oidc_config,
     scheme_name="Keycloak",
 )
```

