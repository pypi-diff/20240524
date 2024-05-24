# Comparing `tmp/msal_bearer-0.2.1.tar.gz` & `tmp/msal_bearer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msal_bearer-0.2.1.tar", max compression
+gzip compressed data, was "msal_bearer-1.0.0.tar", max compression
```

## Comparing `msal_bearer-0.2.1.tar` & `msal_bearer-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2024-01-19 10:25:24.717267 msal_bearer-0.2.1/LICENSE.md
--rw-r--r--   0        0        0      894 2024-03-11 14:42:32.418562 msal_bearer-0.2.1/README.md
--rw-r--r--   0        0        0     5848 2024-03-12 18:38:33.040551 msal_bearer-0.2.1/msal_bearer/BearerAuth.py
--rw-r--r--   0        0        0      522 2024-03-12 18:38:33.045686 msal_bearer-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1663 1970-01-01 00:00:00.000000 msal_bearer-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-01-19 10:25:24.717267 msal_bearer-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0      894 2024-03-11 14:42:32.418562 msal_bearer-1.0.0/README.md
+-rw-r--r--   0        0        0     6259 2024-05-24 13:45:28.990987 msal_bearer-1.0.0/msal_bearer/BearerAuth.py
+-rw-r--r--   0        0        0      653 2024-05-23 12:25:15.658364 msal_bearer-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 msal_bearer-1.0.0/PKG-INFO
```

### Comparing `msal_bearer-0.2.1/LICENSE.md` & `msal_bearer-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `msal_bearer-0.2.1/README.md` & `msal_bearer-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `msal_bearer-0.2.1/msal_bearer/BearerAuth.py` & `msal_bearer-1.0.0/msal_bearer/BearerAuth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,49 @@
 import os
 from typing import List, Union
 
 import msal
 from msal_extensions import (
     build_encrypted_persistence,
     PersistedTokenCache,
-    # PersistenceDecryptionError
 )
 
 _token_location = "token_cache.bin"
 
 
 def set_token_location(location: str):
+    """Setter for token location
+
+    Args:
+        location (str): Where to set
+
+    Raises:
+        ValueError: If input location is not a valid path.
+        TypeError: If input location is not string.
+    """
     global _token_location
 
     if isinstance(location, str):
-        if len(location) > 5:
+        if len(location) > 4 and "." in location:
             _token_location = location
         else:
             raise ValueError(f"Invalid location string {location}")
     else:
         raise TypeError("Input location shall be a string.")
 
 
+def get_token_location() -> str:
+    """Getter for token location.
+
+    Returns:
+        str: Token location (pathlike)
+    """
+    return _token_location
+
+
 def get_login_name() -> Union[str, None]:
     """Get login name of current user.
 
     Returns:
         Union[str, None]: Login name or None
     """
     env_names = ["LOGNAME", "USER", "LNAME", "USERNAME"]
@@ -51,15 +68,15 @@
     if isinstance(token_location, str) and len(token_location) > 0:
         set_token_location(token_location)
     else:
         # if verbose:
         # Uses default token location
         pass
 
-    persistence = build_encrypted_persistence(_token_location)
+    persistence = build_encrypted_persistence(get_token_location())
 
     cache = PersistedTokenCache(persistence)
     return msal.PublicClientApplication(
         client_id=client_id, authority=authority, token_cache=cache
     )
 
 
@@ -120,21 +137,23 @@
         if authority is None or (isinstance(authority, str) and len(authority) == 0):
             authority = get_tenant_authority(tenant_id=tenantID)
 
         result = None
         accounts = None
 
         try:
+            if not token_location:
+                token_location = get_token_location()
+
             # Try to get Access Token silently from cache
             app = get_app_with_cache(
                 client_id=clientID, authority=authority, token_location=token_location
             )
             accounts = app.get_accounts(username=username)
         except Exception as ex:
-            # PersistenceDecryptionError
             if os.path.isfile(_token_location):
                 if verbose:
                     print(
                         f"Failed getting accounts from app with cache. Attempts to delete cache-file at {_token_location}"
                     )
                 os.remove(_token_location)
             app = get_app_with_cache(
```

### Comparing `msal_bearer-0.2.1/pyproject.toml` & `msal_bearer-1.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [tool.poetry]
 name = "msal-bearer"
-version = "0.2.1"
+version = "1.0.0"
 description = "Python package to get auth token interactively for a public client application using msal and msal-extension for caching."
 authors = [
     "Åsmund Våge Fannemel <asmf@equinor.com>",
 ]
 license = "MIT"
 readme = "README.md"
+repository = "https://github.com/Equinor/msal-bearer"
+classifiers = ["Operating System :: OS Independent"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-msal = "^1.26.0"
+msal = "^1.28.0"
 msal-extensions = "^1.1.0"
+cryptography = "^42.0.6"
 
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.12.1"
+black = "^24.4.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `msal_bearer-0.2.1/PKG-INFO` & `msal_bearer-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: msal-bearer
-Version: 0.2.1
+Version: 1.0.0
 Summary: Python package to get auth token interactively for a public client application using msal and msal-extension for caching.
+Home-page: https://github.com/Equinor/msal-bearer
 License: MIT
 Author: Åsmund Våge Fannemel
 Author-email: asmf@equinor.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: msal (>=1.26.0,<2.0.0)
+Requires-Dist: cryptography (>=42.0.6,<43.0.0)
+Requires-Dist: msal (>=1.28.0,<2.0.0)
 Requires-Dist: msal-extensions (>=1.1.0,<2.0.0)
+Project-URL: Repository, https://github.com/Equinor/msal-bearer
 Description-Content-Type: text/markdown
 
 # msal-bearer
 Python package to get auth token interactively for a msal public client application and cache it locally.
 
 ## Usage
```

