# Comparing `tmp/mailtm_sdk-0.1.1.tar.gz` & `tmp/mailtm_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailtm_sdk-0.1.1.tar", last modified: Thu May 16 16:19:29 2024, max compression
+gzip compressed data, was "mailtm_sdk-0.1.2.tar", last modified: Fri May 24 16:34:44 2024, max compression
```

## Comparing `mailtm_sdk-0.1.1.tar` & `mailtm_sdk-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:19:29.530488 mailtm_sdk-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34823 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-05-16 16:19:29.530488 mailtm_sdk-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:19:29.526488 mailtm_sdk-0.1.1/mailtm/
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:19:29.526488 mailtm_sdk-0.1.1/mailtm/abc/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/abc/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/abc/modals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:19:29.526488 mailtm_sdk-0.1.1/mailtm/core/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/core/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:19:29.530488 mailtm_sdk-0.1.1/mailtm/impls/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/impls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/impls/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16153 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/impls/pullers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/impls/xclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:19:29.530488 mailtm_sdk-0.1.1/mailtm/server/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/server/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/server/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/server/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    13662 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/mailtm/server/srv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:19:29.530488 mailtm_sdk-0.1.1/mailtm_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-05-16 16:19:29.000000 mailtm_sdk-0.1.1/mailtm_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-16 16:19:29.000000 mailtm_sdk-0.1.1/mailtm_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:19:29.000000 mailtm_sdk-0.1.1/mailtm_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 16:19:29.000000 mailtm_sdk-0.1.1/mailtm_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 16:19:29.000000 mailtm_sdk-0.1.1/mailtm_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 16:19:29.000000 mailtm_sdk-0.1.1/mailtm_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 16:19:29.530488 mailtm_sdk-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-16 16:19:24.000000 mailtm_sdk-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:34:44.427040 mailtm_sdk-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    34823 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-05-24 16:34:44.427040 mailtm_sdk-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:34:44.423040 mailtm_sdk-0.1.2/mailtm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:34:44.423040 mailtm_sdk-0.1.2/mailtm/abc/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/abc/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/abc/modals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:34:44.423040 mailtm_sdk-0.1.2/mailtm/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/core/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:34:44.423040 mailtm_sdk-0.1.2/mailtm/impls/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/impls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12877 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/impls/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16183 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/impls/pullers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13801 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/impls/xclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:34:44.423040 mailtm_sdk-0.1.2/mailtm/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/server/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/server/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/server/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13662 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/mailtm/server/srv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:34:44.427040 mailtm_sdk-0.1.2/mailtm_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-05-24 16:34:44.000000 mailtm_sdk-0.1.2/mailtm_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-24 16:34:44.000000 mailtm_sdk-0.1.2/mailtm_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:34:44.000000 mailtm_sdk-0.1.2/mailtm_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-24 16:34:44.000000 mailtm_sdk-0.1.2/mailtm_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-24 16:34:44.000000 mailtm_sdk-0.1.2/mailtm_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 16:34:44.000000 mailtm_sdk-0.1.2/mailtm_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 16:34:44.427040 mailtm_sdk-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-24 16:34:40.000000 mailtm_sdk-0.1.2/setup.py
```

### Comparing `mailtm_sdk-0.1.1/LICENSE.md` & `mailtm_sdk-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mailtm_sdk-0.1.1/PKG-INFO` & `mailtm_sdk-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailtm-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Mail.tm Stack Development Kit, designed to enhance your experience with the renowned temporary email service, mail.tm
 Home-page: https://halfstackpgr.github.io/Mail.tm/
 Author: Parth Mishra
 Author-email: halfstackpgr@gmail.com
 Maintainer: Parth Mishra
 Maintainer-email: halfstackpgr@gmail.com
 Classifier: Environment :: Console
```

### Comparing `mailtm_sdk-0.1.1/README.md` & `mailtm_sdk-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mailtm_sdk-0.1.1/mailtm/__init__.py` & `mailtm_sdk-0.1.2/mailtm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ---
 ### Credits:
 Created by GitHub: [@halfstackpgr](https://github.com/halfstackpgr)
 For any query or bug: [Raise an Issues](https://github.com/halfstackpgr/mailtm/issues)
 For further updates visit: [GitHub](https://github.com/halfstackpgr/mailtm)
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.2"
 
 __all__ = [
     "MailServer",
     "ServerEvents",
     "GenericTypes",
     "ModalTypes",
     "AsyncMail",
```

### Comparing `mailtm_sdk-0.1.1/mailtm/abc/generic.py` & `mailtm_sdk-0.1.2/mailtm/abc/generic.py`

 * *Files identical despite different names*

### Comparing `mailtm_sdk-0.1.1/mailtm/abc/modals.py` & `mailtm_sdk-0.1.2/mailtm/abc/modals.py`

 * *Files identical despite different names*

### Comparing `mailtm_sdk-0.1.1/mailtm/cli.py` & `mailtm_sdk-0.1.2/mailtm/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 {mail}|  \/  |     (_) || |{reset}
 {mail}| \  / | __ _ _| || |_ _ __ ___{reset}    {info}Developed: halfstackpgr     Website: https://mail.tm{reset}
 {mail}| |\/| |/ _` | | || __| '_ ` _ \{reset}                        
 {mail}| |  | | (_| | | || |_| | | | | |{reset}  {info}Documentation: https://github.com/halfstackpgr/Mail.tm{reset}
 {mail}|_|  |_|\__,_|_|_(_)__|_| |_| |_|{reset}                       
         {sdk} ____  ____  _  __{reset}         {issues}Issues: https://github.com/halfstackpgr/Mail.tm/Issues{reset}
         {sdk}/ ___||  _ \| |/ /{reset}        
-        {sdk}\___ \| | | | ' /{reset}          {version}Version: 0.1.0                             Coverage: 98%{reset}  
+        {sdk}\___ \| | | | ' /{reset}          {version}Version: 0.1.2                            Coverage: 98%{reset}  
         {sdk} ___) | |_| | . \{reset}       
         {sdk}|____/|____/|_|\_\{reset}         {dateandtime}Time: {time}                             Date:{date}{reset}
 '''
 
 def version() -> None:
     """
     Version information and general banner for Mail.TM.
```

### Comparing `mailtm_sdk-0.1.1/mailtm/core/errors.py` & `mailtm_sdk-0.1.2/mailtm/core/errors.py`

 * *Files identical despite different names*

### Comparing `mailtm_sdk-0.1.1/mailtm/core/methods.py` & `mailtm_sdk-0.1.2/mailtm/core/methods.py`

 * *Files identical despite different names*

### Comparing `mailtm_sdk-0.1.1/mailtm/impls/client.py` & `mailtm_sdk-0.1.2/mailtm/impls/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             result = self._client.post(url=url, json=body)
         elif method == "DELETE":
             result = self._client.delete(url=url, params=params)
         elif method == "PATCH":
             result = self._client.patch(url=url, json=body)
         else:
             raise MethodNotAllowed("Report this as a bug on GitHub")
-        if result.status_code == 200:
+        if str(result.status_code).startswith("20"):
             return result.content
         elif result.status_code == 400:
             raise MissingArgument("Something in your payload is missing! Or, the payload isn't there at all.")
         elif result.status_code == 401:
             raise AccountTokenInvalid(
                 "Your token isn't correct (Or the headers hasn't a token at all!). Remember, every request (Except POST /accounts and POST /token) should be authenticated with a Bearer token!"
             )
```

### Comparing `mailtm_sdk-0.1.1/mailtm/impls/pullers.py` & `mailtm_sdk-0.1.2/mailtm/impls/pullers.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         elif method == "POST":
             resp = requests.post(url=url, params=params, json=body)
         elif method == "DELETE":
             resp = requests.delete(url=url, params=params, json=body)
         elif method == "PATCH":
             resp = requests.patch(url=url, params=params, json=body)
 
-        if resp.status_code == 200:
+        if str(resp.status_code).startswith("20"):
             return resp.content
         elif resp.status_code == 400:
             raise MissingArgument("Something in your payload is missing! Or, the payload isn't there at all.")
         elif resp.status_code == 401:
             raise AccountTokenInvalid(
                 "Your token isn't correct (Or the headers hasn't a token at all!). Remember, every request (Except POST /accounts and POST /token) should be authenticated with a Bearer token!"
             )
@@ -282,15 +282,15 @@
         params: t.Optional[t.Dict[str, str]] = None,
     ) -> t.Optional[bytes]:
         if method not in ["GET", "POST", "DELETE", "PATCH"]:
             raise ValueError("Invalid HTTP method")
         try:
             async with aiohttp.request(method, url, params=params, json=body) as resp:
                 result = resp
-                if result.status == 200:
+                if str(result.status).startswith("20"):
                     return await result.read()
                 elif result.status == 400:
                     raise MissingArgument("Something in your payload is missing! Or, the payload isn't there at all.")
                 elif result.status == 401:
                     raise AccountTokenInvalid(
                         "Your token isn't correct (Or the headers hasn't a token at all!). Remember, every request (Except POST /accounts and POST /token) should be authenticated with a Bearer token!"
                     )
```

### Comparing `mailtm_sdk-0.1.1/mailtm/impls/xclient.py` & `mailtm_sdk-0.1.2/mailtm/impls/xclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             result = await self._client.delete(url=url, params=params)
 
         elif method == "PATCH":
             result = await self._client.patch(url=url, json=body)
         else:
             raise MethodNotAllowed("Report this as a bug on GitHub")
 
-        if result.status == 200:
+        if str(result.status).startswith("20"):
             return await result.read()
         elif result.status == 400:
             raise MissingArgument("Something in your payload is missing! Or, the payload isn't there at all.")
         elif result.status == 401:
             raise AccountTokenInvalid(
                 "Your token isn't correct (Or the headers hasn't a token at all!). Remember, every request (Except POST /accounts and POST /token) should be authenticated with a Bearer token!"
             )
```

### Comparing `mailtm_sdk-0.1.1/mailtm/server/__init__.py` & `mailtm_sdk-0.1.2/mailtm/server/__init__.py`

 * *Files identical despite different names*

### Comparing `mailtm_sdk-0.1.1/mailtm/server/cache.py` & `mailtm_sdk-0.1.2/mailtm/server/cache.py`

 * *Files identical despite different names*

### Comparing `mailtm_sdk-0.1.1/mailtm/server/events.py` & `mailtm_sdk-0.1.2/mailtm/server/events.py`

 * *Files identical despite different names*

### Comparing `mailtm_sdk-0.1.1/mailtm/server/impl.py` & `mailtm_sdk-0.1.2/mailtm/server/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,22 +106,22 @@
 
         Returns
         -------
             None
         """
         try:
             if isinstance(new_account_token, Token):
-                self.mail_client._client.headers.update({"Authorization": f"Bearer {new_account_token.token}"})
+                self.mail_client._client.headers.update({"Authorization": f"Bearer {new_account_token.token}"}) #type: ignore
                 self.log(message=f"Switched to new account with ID: {new_account_token.id}", severity="WARNING")
             if isinstance(new_account_token, str):
-                self.mail_client._client.headers.update({"Authorization": f"Bearer {new_account_token}"})
-                self.log(message=f"Switched to new account with Token: {new_account_token}", severity="WARNING")
+                self.mail_client._client.headers.update({"Authorization": f"Bearer {new_account_token}"}) #type: ignore
+                self.log(message=f"Switched to new account with Token: {new_account_token}", severity="WARNING") 
 
             await self.dispatch(
-                AccountSwitched(event="Account switched", client=self.mail_client, _server=AttachServer(self))
+                AccountSwitched(event="Account switched", client=self.mail_client, _server=AttachServer(self), last_account_auth=self._server_auth)
             )
 
         except Exception as e:
             self.log(message="Could not switch account: " + str(e), severity="ERROR")
 
     async def delete_account(self, account_id: str) -> None:
         """
```

### Comparing `mailtm_sdk-0.1.1/mailtm/server/srv.py` & `mailtm_sdk-0.1.2/mailtm/server/srv.py`

 * *Files identical despite different names*

### Comparing `mailtm_sdk-0.1.1/mailtm_sdk.egg-info/PKG-INFO` & `mailtm_sdk-0.1.2/mailtm_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailtm-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Mail.tm Stack Development Kit, designed to enhance your experience with the renowned temporary email service, mail.tm
 Home-page: https://halfstackpgr.github.io/Mail.tm/
 Author: Parth Mishra
 Author-email: halfstackpgr@gmail.com
 Maintainer: Parth Mishra
 Maintainer-email: halfstackpgr@gmail.com
 Classifier: Environment :: Console
```

### Comparing `mailtm_sdk-0.1.1/mailtm_sdk.egg-info/SOURCES.txt` & `mailtm_sdk-0.1.2/mailtm_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mailtm_sdk-0.1.1/setup.py` & `mailtm_sdk-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open('README.md', "r", encoding="utf-8") as f:
     description = f.read()
 
 
 setup(
     name="mailtm-sdk",
-    version="0.1.1",
+    version="0.1.2",
     description="Mail.tm Stack Development Kit, designed to enhance your experience with the renowned temporary email service, mail.tm",
     long_description=description,
     long_description_content_type="text/markdown",
     author="Parth Mishra",
     author_email="halfstackpgr@gmail.com",
     maintainer="Parth Mishra", 
     maintainer_email="halfstackpgr@gmail.com",
```

