# Comparing `tmp/affliction-0.7.tar.gz` & `tmp/affliction-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "affliction-0.7.tar", last modified: Wed Feb 14 22:40:10 2024, max compression
+gzip compressed data, was "affliction-0.8.tar", last modified: Fri May 24 04:50:53 2024, max compression
```

## Comparing `affliction-0.7.tar` & `affliction-0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-02-14 22:40:10.872452 affliction-0.7/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       85 2023-10-27 01:45:33.000000 affliction-0.7/MANIFEST.in
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4099 2024-02-14 22:40:10.872452 affliction-0.7/PKG-INFO
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2377 2023-10-27 23:05:55.000000 affliction-0.7/README.md
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-02-14 22:40:10.872452 affliction-0.7/affliction/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-22 06:26:46.000000 affliction-0.7/affliction/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4744 2023-12-07 02:42:30.000000 affliction-0.7/affliction/base.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      902 2023-10-27 02:54:51.000000 affliction-0.7/affliction/exchange_client.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)    17617 2024-02-02 03:16:18.000000 affliction-0.7/affliction/graph_client.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       37 2024-02-14 22:40:08.000000 affliction-0.7/affliction/version_info.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-02-14 22:40:10.872452 affliction-0.7/affliction.egg-info/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4099 2024-02-14 22:40:10.000000 affliction-0.7/affliction.egg-info/PKG-INFO
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      333 2024-02-14 22:40:10.000000 affliction-0.7/affliction.egg-info/SOURCES.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2024-02-14 22:40:10.000000 affliction-0.7/affliction.egg-info/dependency_links.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      143 2024-02-14 22:40:10.000000 affliction-0.7/affliction.egg-info/requires.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       11 2024-02-14 22:40:10.000000 affliction-0.7/affliction.egg-info/top_level.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      105 2023-10-27 01:48:10.000000 affliction-0.7/dev.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       38 2024-02-14 22:40:10.872452 affliction-0.7/setup.cfg
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2380 2024-02-14 22:40:08.000000 affliction-0.7/setup.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-05-24 04:50:53.162835 affliction-0.8/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       85 2024-05-24 04:04:14.000000 affliction-0.8/MANIFEST.in
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4099 2024-05-24 04:50:53.162835 affliction-0.8/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2377 2024-05-24 04:04:14.000000 affliction-0.8/README.md
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-05-24 04:50:53.152835 affliction-0.8/affliction/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2024-05-24 04:04:14.000000 affliction-0.8/affliction/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4984 2024-05-24 04:43:51.000000 affliction-0.8/affliction/base.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      902 2024-05-24 04:04:14.000000 affliction-0.8/affliction/exchange_client.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)    19626 2024-05-24 04:34:21.000000 affliction-0.8/affliction/graph_client.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       37 2024-05-24 04:50:51.000000 affliction-0.8/affliction/version_info.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-05-24 04:50:53.152835 affliction-0.8/affliction.egg-info/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4099 2024-05-24 04:50:53.000000 affliction-0.8/affliction.egg-info/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      333 2024-05-24 04:50:53.000000 affliction-0.8/affliction.egg-info/SOURCES.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2024-05-24 04:50:53.000000 affliction-0.8/affliction.egg-info/dependency_links.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      143 2024-05-24 04:50:53.000000 affliction-0.8/affliction.egg-info/requires.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       11 2024-05-24 04:50:53.000000 affliction-0.8/affliction.egg-info/top_level.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      105 2024-05-24 04:04:14.000000 affliction-0.8/dev.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       38 2024-05-24 04:50:53.162835 affliction-0.8/setup.cfg
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2380 2024-05-24 04:50:51.000000 affliction-0.8/setup.py
```

### Comparing `affliction-0.7/PKG-INFO` & `affliction-0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affliction
-Version: 0.7
+Version: 0.8
 Summary: affliction
 Home-page: https://bitbucket.org/dbuy/affliction
 Author: dev
 Author-email: unknown@yahoo.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `affliction-0.7/README.md` & `affliction-0.8/README.md`

 * *Files identical despite different names*

### Comparing `affliction-0.7/affliction/base.py` & `affliction-0.8/affliction/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from time import time
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 
+class MicrosoftApiException(Exception):
+    def __init__(self, json_data, *args) -> None:
+        super().__init__(*args)
+        self.data = json_data
+
+
 class SynchronousMicrosoftApiClient:
     def __init__(
             self,
             tenant_id,
             client_id=None,
             client_secret=None,
             creds=None,
@@ -69,29 +75,29 @@
         if response.status_code == 200:
             if raw:
                 return response
             return response.json()
         if response.status_code == 401 and not token_retry:  # pragma: no cover
             self.fetch_access_token()
             return self.get(url, params, token_retry=True)
-        raise Exception("request failure: " + response.text)  # pragma: no cover
+        raise MicrosoftApiException(response.json(), "request failure: " + response.text)  # pragma: no cover
 
     def post(self, url, params=None, headers=None, token_retry=False, **kwargs):
         raw = kwargs.pop('raw', False)
         if self.token.expires_on - time() < 5:  # pragma: no cover
             self.fetch_access_token()
         response = self.session.post(url, params=params, headers=headers, **kwargs)
         if 200 <= response.status_code < 300:
             if raw:
                 return response
             return response.json()
         if response.status_code == 401 and not token_retry:  # pragma: no cover
             self.fetch_access_token()
             return self.get(url, params, token_retry=True)
-        raise Exception("request failure: " + response.text)  # pragma: no cover
+        raise MicrosoftApiException(response.json(), "request failure: " + response.text)  # pragma: no cover
 
     def delete(self, url, params=None, headers=None, token_retry=False, **kwargs):
         raw = kwargs.pop('raw', False)
         if self.token.expires_on - time() < 5:  # pragma: no cover
             self.fetch_access_token()
         response = self.session.delete(url, params=params, headers=headers, **kwargs)
         if 200 <= response.status_code < 300:
@@ -99,17 +105,16 @@
                 return response
             if response.text:  # pragma: no cover
                 return response.json()
             return None  # pragma: no cover
         if response.status_code == 401 and not token_retry:  # pragma: no cover
             self.fetch_access_token()
             return self.get(url, params, token_retry=True)
-        raise Exception("request failure: " + response.text)  # pragma: no cover
+        raise MicrosoftApiException(response.json(), "request failure: " + response.text)  # pragma: no cover
 
     def yield_result(self, url, params=None, **kwargs):
         endpoint = url
         while endpoint:
             result = self.get(endpoint, params=params, **kwargs)
             yield from result.get('value', [])
             endpoint = result.get('@odata.nextLink')
             params = None
-
```

### Comparing `affliction-0.7/affliction/exchange_client.py` & `affliction-0.8/affliction/exchange_client.py`

 * *Files identical despite different names*

### Comparing `affliction-0.7/affliction/graph_client.py` & `affliction-0.8/affliction/graph_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,30 @@
     m365_e5 = 'SPE_E5'
     m365_f1 = 'M365_F1'
     o365_e1 = 'STANDARDPACK'
     o365_e2 = 'STANDARDWOFFPACK'
     o365_storage = 'SHAREPOINTSTORAGE'
     o365_e3 = 'ENTERPRISEPACK'
     o365_e5 = 'ENTERPRISEPREMIUM'
+    values_map = {
+        'AAD_PREMIUM_P2': 'entra_id_p2',
+        'EXCHANGESTANDARD': 'exchange_plan_1',
+        'EXCHANGEENTERPRISE': 'exchange_plan_2',
+        'O365_BUSINESS': 'm365_apps',
+        'OFFICESUBSCRIPTION': 'm365_apps_enterprise',
+        'O365_BUSINESS_PREMIUM': 'm365_business_standard',
+        'SPE_E3': 'm365_e3',
+        'SPE_E5': 'm365_e5',
+        'M365_F1': 'm365_f1',
+        'STANDARDPACK': 'o365_e1',
+        'STANDARDWOFFPACK': 'o365_e2',
+        'SHAREPOINTSTORAGE': 'o365_storage',
+        'ENTERPRISEPACK': 'o365_e3',
+        'ENTERPRISEPREMIUM': 'o365_e5',
+    }
 
 
 class SynchronousGraphClient(SynchronousMicrosoftApiClient):
     def __init__(
             self,
             tenant_id,
             client_id=None,
@@ -132,15 +148,15 @@
     @classmethod
     def escape_upn(cls, upn):
         return upn.replace('#', '%23')
 
     def get_user(self, n_id=None, select=None):
         """
         returns the specified user, select should be a list of strings
-        that include one or more properties from https://docs.microsoft.com/en-us/graph/api/user-list?view=graph-rest-1.0
+        that include 1+ properties from https://docs.microsoft.com/en-us/graph/api/user-list?view=graph-rest-1.0
         """
         n_id = self.escape_upn(n_id)
         endpoint = f"{self.base_url}/users('{n_id}')"
         select = select or [
             'id',
             'userPrincipalName',
             'displayName',
@@ -183,15 +199,15 @@
         https://learn.microsoft.com/en-us/entra/identity/users/licensing-service-plan-reference
         """
         params = {
             '$select': 'skuId,skuPartNumber',
         }
         rg = self.subscribed_skus(params=params)
         rg = list(rg)
-        rg.sort(key = lambda lx: lx['skuPartNumber'].lower())
+        rg.sort(key=lambda lx: lx['skuPartNumber'].lower())
         return {
             x['skuPartNumber']: x['skuId']
             for x in rg
         }
 
     def resolve_skus(self, user, sku_map=None):
         if not sku_map:
@@ -234,15 +250,14 @@
                 remove_licenses.append(sku_id)
         json_data = {}
         json_data['addLicenses'] = add_licenses
         json_data['removeLicenses'] = remove_licenses
         url = f"{self.base_url}/users('{user_id}')/assignLicense"
         return self.post(url, json_data=json_data)
 
-
     def get_groups(self, params=None, **kwargs):
         """
         https://learn.microsoft.com/en-us/graph/api/group-list?view=graph-rest-1.0&tabs=http
         """
         url = f'{self.base_url}/groups'
         return list(self.yield_result(url, params=params, **kwargs))
 
@@ -337,14 +352,39 @@
             group_id=None):
         """
         deletes group using the microsoft graph api
         """
         url = f'{self.base_url}/groups/{group_id}'
         return self.delete(url, raw=True)
 
+    def add_group_member(
+            self,
+            group_id,
+            user_id):
+        """
+        adds a user to a group
+        """
+        url = f'{self.base_url}/groups/{group_id}/members/$ref'
+        data = {
+            '@odata.id': f'https://graph.microsoft.com/v1.0/directoryObjects/{user_id}',
+        }
+        response = self.post(url, json_data=data, raw=True)
+        return response.status_code == 204
+
+    def remove_group_member(
+            self,
+            group_id,
+            user_id):
+        """
+        removes a user from a group
+        """
+        url = f'{self.base_url}/groups/{group_id}/members/{user_id}/$ref'
+        response = self.delete(url, raw=True)
+        return response.status_code == 204
+
     def get_app(self, object_id=None, app_id=None):
         if object_id:
             url = f'{self.base_url}/applications/{object_id}'
         else:
             url = f"{self.base_url}/applications(appId='{app_id}')"
         return self.get(url)
 
@@ -426,15 +466,15 @@
             self.base_url,
             'servicePrincipals', service_principal_id,
             'synchronization', 'jobs', job_id,
             'schema',
         )
         return self.get(url)
 
-    def provision_group_on_demand(self, group_id, app_name, rule_name=None, **kwargs):
+    def provision_on_demand(self, subjects, app_name, rule_name=None, **kwargs):
         service_principal = self.get_service_principal(name=app_name)
         service_principal_id = service_principal['id']
         jobs = self.get_app_jobs(service_principal_id=service_principal_id)
         job = jobs[0]
         job_id = job['id']
         schema = self.get_app_job_schema(job_id, service_principal_id)
         rules = schema['synchronizationRules']
@@ -442,24 +482,41 @@
         if rule_name:
             for rule in rules:
                 if rule['name'] == rule_name:
                     rule_id = rule['id']
                     break
         else:
             rule_id = rules[0]['id']
-        subjects = [{
-            'objectId': group_id,
-            'objectTypeName': 'Group',
-        }]
         data = {
             'parameters': [{
                 'subjects': subjects,
                 'ruleId': rule_id,
             }],
         }
         url = posixpath.join(
             self.base_url,
             'servicePrincipals', service_principal_id,
             'synchronization', 'jobs', job_id,
             'provisionOnDemand'
         )
         return self.post(url, json_data=data, **kwargs)
+
+    def provision_group_on_demand(self, group_id, app_name, rule_name=None, **kwargs):
+        subjects = [{
+            'objectId': group_id,
+            'objectTypeName': 'Group',
+        }]
+        return self.provision_on_demand(subjects, app_name, rule_name, **kwargs)
+
+    def provision_group_members_on_demand(self, group_id, user_ids, app_name, rule_name=None, **kwargs):
+        subject = {
+            'objectId': group_id,
+            'objectTypeName': 'Group',
+            'links': {
+                'members': [{
+                    'objectId': user_id,
+                    'objectTypeName': 'User',
+                } for user_id in user_ids]
+            },
+        }
+        subjects = [ subject ]
+        return self.provision_on_demand(subjects, app_name, rule_name, **kwargs)
```

### Comparing `affliction-0.7/affliction.egg-info/PKG-INFO` & `affliction-0.8/affliction.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affliction
-Version: 0.7
+Version: 0.8
 Summary: affliction
 Home-page: https://bitbucket.org/dbuy/affliction
 Author: dev
 Author-email: unknown@yahoo.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `affliction-0.7/setup.py` & `affliction-0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     all_extras = list(all_extras)
     all_extras.sort()
     extras['all'] = all_extras
 
 
 setup(
     name='affliction',
-    version='0.7',
+    version='0.8',
     description='affliction',
     license='BSD',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='dev',
     author_email='unknown@yahoo.com',
     url='https://bitbucket.org/dbuy/affliction',
```

