# Comparing `tmp/docketalarm_api-1.0.1.tar.gz` & `tmp/docketalarm_api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docketalarm_api-1.0.1.tar", max compression
+gzip compressed data, was "docketalarm_api-1.0.2.tar", max compression
```

## Comparing `docketalarm_api-1.0.1.tar` & `docketalarm_api-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    11417 2024-04-30 01:00:40.795751 docketalarm_api-1.0.1/README.md
--rw-r--r--   0        0        0       53 2024-04-29 16:31:02.638318 docketalarm_api-1.0.1/docketalarm_api/__init__.py
--rw-r--r--   0        0        0    14054 2024-04-29 22:46:47.247110 docketalarm_api-1.0.1/docketalarm_api/api_client.py
--rw-r--r--   0        0        0      454 2024-04-30 01:14:41.349219 docketalarm_api-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    12357 2024-04-30 01:14:59.041008 docketalarm_api-1.0.1/setup.py
--rw-r--r--   0        0        0    12012 2024-04-30 01:14:59.042458 docketalarm_api-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    12011 2024-05-24 13:39:31.526227 docketalarm_api-1.0.2/README.md
+-rw-r--r--   0        0        0       53 2024-04-29 16:31:02.638318 docketalarm_api-1.0.2/docketalarm_api/__init__.py
+-rw-r--r--   0        0        0    14584 2024-05-24 13:36:31.152948 docketalarm_api-1.0.2/docketalarm_api/api_client.py
+-rw-r--r--   0        0        0      454 2024-05-24 13:45:43.038939 docketalarm_api-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    12708 1970-01-01 00:00:00.000000 docketalarm_api-1.0.2/PKG-INFO
```

### Comparing `docketalarm_api-1.0.1/README.md` & `docketalarm_api-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,58 +39,60 @@
 ```
 
 ## search
 Perform a search on DocketAlarm API's search endpoint.  
 
 | Parameter    | Description                                         |
 |--------------|-----------------------------------------------------|
-| query        | The DocketAlarm query to use.                      |
-| order        | The order to get the results by.                   |
-| limit        | The search limit, must be 50 or less.              |
+| query        | The DocketAlarm query to use.                       |
+| order        | The order to get the results by.                    |
+| limit        | The search limit, must be 50 or less.               |
 | offset       | Offset for the search, useful for pagination.       |
-| login_token  | Will be created if not provided.                   |
+| login_token  | Will be created if not provided.                    |
 | return       | Dictionary with JSON response.                      |
 
 **Example**:
 
 ```
     response = da_client.search("is:docket AND is:state", "random", limit=10)
     search_results = response["search_results"]
 ```
 
 ## get_docket
 Interact with getdocket endpoint, fetching a docket by court and docket number.  
 
-| Parameter       | Description                                       |
-|-----------------|---------------------------------------------------|
-| docket          | The docket number obtained from search.           |
-| court           | The court of the docket obtained from search.     |
-| timeout         | Timeout for the GET request.                      |
-| client_matter   | The client matter for the API call.               |
-| normalize       | Normalize option for getdocket endpoint.          |
-| cached          | Defaults to True, gets cached version of the docket. |
-| login_token     | If not provided it's auto-generated.             |
-| return          | Dictionary with JSON response.                    |
+| Parameter               | Description                                                |
+|-------------------------|------------------------------------------------------------|
+| docket                  | The docket number obtained from search.                    |
+| court                   | The court of the docket obtained from search.              |
+| timeout                 | Timeout for the GET request.                               |
+| client_matter           | The client matter for the API call.                        |
+| normalize               | Normalize option for getdocket endpoint.                   |
+| cached                  | Defaults to True, gets cached version of the docket.       |
+| login_token             | If not provided it's auto-generated.                       |
+| check_is_pacer          | Include a boolean stating if the case is from a PACER court|
+| add_documents_by_entries| Include a list of all documents per entry on the response  |
+| return                  | Dictionary with JSON response.                             |
 
 **Example**:
 
 ```
     docket_data = da_client.get_docket(docket="JC205-106", court="Texas State, Grayson County, Justice of the Peace 2")
 ```
 
 ## get_document_binary
 Fetches the binary content of a pdf stored in DocketAlarm or directly from the court.  
 
-| Parameter    | Description                                           |
-|--------------|-------------------------------------------------------|
-| doc_url      | URL for the document.                                 |
-| login_token  | Token for OpenAI authentication.                      |
-| client_matter| The matter or client for the API call.                |
+| Parameter    | Description                                                              |
+|--------------|--------------------------------------------------------------------------|
+| doc_url      | URL for the document.                                                    |
+| login_token  | Token for OpenAI authentication.                                         |
+| client_matter| The matter or client for the API call.                                   |
 | cached       | Boolean stating if desired to use cached version of the document or not. |
-| return       | Document binary (bytes).                              |
+| return       | Document binary (bytes).                                                 |
 
 **Example**:
 
 ```
     document_bytes = da_client.get_document_binary(
         'https://www.docketalarm.com/cases/Arkansas_State_Faulkner_County_Circuit_Court/23DR-98-821/OCSE_V_JOHN_TAYLOR/docs/28082014_OTHER_0.pdf'
     )
@@ -100,44 +102,44 @@
 
 These methods require the use of an OpenAI API key, suplied when initializing the instance.  
 You can check if an OpenAI API key is valid using the `DocketAlarmClient.is_openai_valid_api_key` method.
 
 ## ask_docket
 Interact with DocketAlarm's ask_docket OpenAI endpoint.  
 
-| Parameter       | Description                                                      |
-|-----------------|------------------------------------------------------------------|
-| docket          | The docket number as extracted from search.                      |
-| court           | The court of the docket as extracted from search.                |
-| question        | The question to ask to the docket data.                          |
-| output_format   | The output format of the desired response in natural language.   |
-| target          | The target for ask_docket, "dockets", "documents" or "both".     |
+| Parameter       | Description                                                              |
+|-----------------|--------------------------------------------------------------------------|
+| docket          | The docket number as extracted from search.                              |
+| court           | The court of the docket as extracted from search.                        |
+| question        | The question to ask to the docket data.                                  |
+| output_format   | The output format of the desired response in natural language.           |
+| target          | The target for ask_docket, "docket", "documents" or "both".              |
 | openai_model    | Model to be used on OpenAI interactions, defaults to gpt-3.5-turbo-1106. |
 | cached          | Gets cached version of the docket on the interaction, defaults to False. |
-| show_relevant   | Gets relevant data used by ask_docket.                           |
-| login_token     | If not provided, it is autogenerated.                           |
-| return          | Dictionary with JSON response.                                   |
+| show_relevant   | Gets relevant data used by ask_docket.                                   |
+| login_token     | If not provided, it is autogenerated.                                    |
+| return          | Dictionary with JSON response.                                           |
 
 **Example**:
 
 ```
     response = da_client.ask_docket(docket='JC205-106', court='Texas State, Grayson County, Justice of the Peace 2',
                                     question='is the case pre or post discovery stages?',
                                     output_format='Enum["pre" or "post" or "unknown"]',
-                                    target="dockets", cached = True)
+                                    target="docket", cached = True)
 
     openai_answer = response["from_dockets"]["openai_answer"]
 ```
 
 ## case_matcher
 Match a case from any input provided using DocketAlarm's OpenAI powered case_matcher endpoint.  
 
-| Parameter       | Description                                                      |
-|-----------------|------------------------------------------------------------------|
-| openai_model    | The OpenAI model to use during case matching.                    |
+| Parameter       | Description                                                         |
+|-----------------|---------------------------------------------------------------------|
+| openai_model    | The OpenAI model to use during case matching.                       |
 | kwargs          | Provide any argument and it will be used as inputs in case matcher. |
 | return          | Dictionary with result from case matcher and OpenAI costs incurred. |
 
 **Example**:
 
 ```
     response = da_client.case_matcher(openai_model="gpt-4-1106-preview",
@@ -163,22 +165,22 @@
     )
     query = response["query"]
 ```
 
 ## attorney_billing_rates
 Extract attorney billing rates by name and state.  
 
-| Parameter       | Description                                                     |
-|-----------------|-----------------------------------------------------------------|
+| Parameter       | Description                                                           |
+|-----------------|-----------------------------------------------------------------------|
 | attorney_name   | The name of the attorney for which billing rates are to be extracted. |
-| state           | The state of the attorney.                                      |
-| openai_model    | OpenAI model to be used on the API call.                         |
-| login_token     | Auto-generated by default.                                      |
-| client_matter   | Empty by default.                                                |
-| return          | Dictionary with result and OpenAI costs incurred.               |
+| state           | The state of the attorney.                                            |
+| openai_model    | OpenAI model to be used on the API call.                              |
+| login_token     | Auto-generated by default.                                            |
+| client_matter   | Empty by default.                                                     |
+| return          | Dictionary with result and OpenAI costs incurred.                     |
 
 **Example**
 
 ```
     response = da_client.attorney_billing_rates(attorney_name="ashley marshal",
                                                 state="connecticut")
     attorney_data = response["result"]
@@ -227,15 +229,15 @@
 
 ## entity_normalizer
 Get a DocketAlarm query for the entity normalized  
 
 | Parameter           | Description                                                            |
 |---------------------|------------------------------------------------------------------------|
 | entity              | The entity to normalize.                                               |
-| include_corp_group | Boolean stating if desired to include corporation group matches.       |
+| include_corp_group  | Boolean stating if desired to include corporation group matches.       |
 | search_limit        | The internal search limit when optimizing. Must be between 10 and 50.  |
 | login_token         | If not provided, it is autogenerated.                                  |
 
 **Example**:
 
 ```
     response = da_client.entity_normalizer(entity="Apple", search_limit=20,
```

### Comparing `docketalarm_api-1.0.1/docketalarm_api/api_client.py` & `docketalarm_api-1.0.2/docketalarm_api/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,19 +121,23 @@
         :param docket: The docket number obtained from search.
         :param court: The court of the docket obtained from search
         :kwarg timeout: Timout for the GET request.
         :kwarg client_matter: The client matter for the API call.
         :kwarg normalize: normalize option for getdocket endpoint.
         :kwarg cached: Defaults to True, gets cached version of the docket
         :kwarg login_token: If not provided it's auto generated
+        :kwarg check_is_pacer: Includes a boolean showing whether the
+                               case is from a PACER court or not.
+        :kwarg add_documents_by_entries: Includes a list of all documents for
+                                     each entry in the main response body 
         :return: dictionary with json response
         """
         timeout = kwargs.get("timeout")
         client_matter = kwargs.get("client_matter", "")
-        extra_keys = ["normalize", "cached", "login_token", "check_is_pacer"]
+        extra_keys = ["normalize", "cached", "login_token", "check_is_pacer", "add_documents_by_entries"]
         basic_params = [("docket", docket), ("client_matter", client_matter), ("court", court)]
         params = dict(basic_params+[(key, kwargs.get(key)) for key in extra_keys if key in kwargs])
 
         if not "cached" in params:
             params["cached"] = True
         
         self.logger.info("Fetching docket using cached=%s" % params["cached"])
@@ -144,15 +148,15 @@
         return self._make_get_request("getdocket/", params=params, timeout=timeout)
     
 
     def get_document_binary(self, doc_url:str, login_token:str="", client_matter:str="", cached:bool=True) -> bytes:
         """
         Fetches the binary content of a pdf stored in DocketAlarm or directly from the court.
         :param doc_url: Url for the document.
-        :param login_token: Token for OpenAI authentication.
+        :param login_token: Token for DocketAlarm authentication.
         :param client_matter: The matter or client for the API call.
         :param cached: Boolean stating if desired to use cached version of the document or not.
         :return: document binarty (bytes)
         """
         if not doc_url.endswith(".pdf") or not doc_url.startswith("https://www.docketalarm.com"):
             raise BadRequest("A DocketAlarm document URL must be provided")
         
@@ -247,15 +251,15 @@
         :param state: The state of the attorney.
         :kwarg openai_model: OpenAI model to be used on the API call.
         :kwarg login_token: Auto generated by default.
         :kwarg client_matter: Empty by default.
         :return: dictionary with result and OpenAI costs incurred
         """
         extra_keys = ["openai_model", "login_token", "client_matter"]
-        basic_params = [("attorney_name", attorney_name), ("state", state)]
+        basic_params = [("attorney_name", attorney_name), ("state", state), ("openai_key", self._openai_api_key)]
         params = dict(basic_params+[(key, kwargs.get(key)) for key in extra_keys if key in kwargs])
 
         if not params.get("login_token"):
             params["login_token"] = self.get_login_token()
     
         if not params.get("client_matter"):
             params["client_matter"] = ""
@@ -272,15 +276,15 @@
         :kwarg openai_model: The OpenAI model to be used on the API call.
         :kwarg login_token: Auto generated by default.
         :kwarg cached: Bool stating if desired to use cached version of the docket.
         :kwarg short: Extract a short complaint summary
         :return: dictionary with complaint summary and OpenAI costs incurred
         """
         extra_keys = ["openai_model", "login_token", "cached", "short"]
-        basic_params = [("docket", docket), ("court", court)]
+        basic_params = [("docket", docket), ("court", court), ("openai_key", self._openai_api_key)]
         params = dict(basic_params+[(key, kwargs.get(key)) for key in extra_keys if key in kwargs])
 
         if not params.get("login_token"):
             params["login_token"] = self.get_login_token()
         
         return self._make_get_request("get_complaint_summary/", params)
 
@@ -293,15 +297,15 @@
         :param court: The court of the docket.
         :kwarg openai_model: The OpenAI model to be used on the API call.
         :kwarg login_token: Auto generated by default.
         :kwarg cached: Bool stating if desired to use cached version of the docket.
         :return: Dictionary with cause of action and OpenAI costs incurred
         """
         extra_keys = ["openai_model", "login_token", "cached"]
-        basic_params = [("docket", docket), ("court", court)]
+        basic_params = [("docket", docket), ("court", court), ("openai_key", self._openai_api_key)]
         params = dict(basic_params+[(key, kwargs.get(key)) for key in extra_keys if key in kwargs])
 
         if not params.get("login_token"):
             params["login_token"] = self.get_login_token()
         
         return self._make_get_request("get_cause_of_action/", params)
 
@@ -312,15 +316,20 @@
         """
         Get a DocketAlarm query for the entity normalized
         :param entity: The entity to normalize.
         :param include_corp_group: Boolean stating if desired to include corporation group matches.
         :param search_limit: The internal search limit when optimizing. Must be between 10 and 50.
         :param login_token: If not provided is autogenerated.
         """
-        params = {"entity": entity, "login_token": login_token or self.get_login_token(), "search_limit": search_limit}
+        params = {
+            "entity": entity,
+            "login_token": login_token or self.get_login_token(),
+            "search_limit": search_limit,
+            "openai_key": self._openai_api_key
+        }
         if include_corp_group:
             params["include_corporate_group"] = True
         
         return self._make_get_request("entity_normalizer/", params)
 
 
     @staticmethod
```

### Comparing `docketalarm_api-1.0.1/setup.py` & `docketalarm_api-1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,264 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: docketalarm_api
+Version: 1.0.2
+Summary: Wrapper to interact with DocketAlarm API
+Home-page: https://www.docketalarm.com/dockets/
+Author: Ezequiel Ghiena
+Author-email: ezequiel.ghiena@vlex.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: requests (>=2.26.0,<3.0.0)
+Project-URL: Documentation, https://www.docketalarm.com/api/v1/
+Description-Content-Type: text/markdown
 
-packages = \
-['docketalarm_api']
+# DocketAlarmAPI
+API Wrapper for DocketAlarm.
+# Table of Contents
+1. [Instalation and usage](#usage)
+2. [Get Login Token](#get_login_token)
+3. [Search](#search)
+4. [Get Docket](#get_docket)
+5. [Get Document](#get_document_binary)
+6. [Ask Docket](#ask_docket)
+7. [Case Matcher](#case_matcher)
+8. [Smart Search](#smart_search)
+9. [Attorney Billing Rates](#attorney_billing_rates)
+10. [Get Complaint Summary](#get_complaint_summary)
+11. [Get Cause of Action](#get_cause_of_action)
 
-package_data = \
-{'': ['*']}
+# usage
+Use `pip install docketalarm_api` to install this library.  
+To use the DocketAlarmClient you'll need your DocketAlarm user and password, and if desired to interact with OpenAI powered endpoints, an OpenAI API Key.  
+Import and initialize the client as follows:
+```
+from docketalarm_api import DocketAlarmClient
 
-install_requires = \
-['requests>=2.26.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'docketalarm-api',
-    'version': '1.0.1',
-    'description': 'Wrapper to interact with DocketAlarm API',
-    'long_description': '# DocketAlarmAPI\nAPI Wrapper for DocketAlarm.\n# Table of Contents\n1. [Instalation and usage](#usage)\n2. [Get Login Token](#get_login_token)\n3. [Search](#search)\n4. [Get Docket](#get_docket)\n5. [Get Document](#get_document_binary)\n6. [Ask Docket](#ask_docket)\n7. [Case Matcher](#case_matcher)\n8. [Smart Search](#smart_search)\n9. [Attorney Billing Rates](#attorney_billing_rates)\n10. [Get Complaint Summary](#get_complaint_summary)\n11. [Get Cause of Action](#get_cause_of_action)\n\n# usage\nUse `pip install docketalarm_api` to install this library.  \nTo use the DocketAlarmClient you\'ll need your DocketAlarm user and password, and if desired to interact with OpenAI powered endpoints, an OpenAI API Key.  \nImport and initialize the client as follows:\n```\nfrom docketalarm_api import DocketAlarmClient\n\nda_client = DocketAlarmClient(<your-docketalarm-user>, <your-docketalarm-password>, <your-openai-api-key>)\n```\n\n# General Endpoints\nThese are methods available directly to your DocketAlarm user through a `DocketAlarmClient` instance.\n\n## get_login_token\nGet authentication token from docketalarm.  \n\n**Example**:\n\n```\n    from docketalarm_api import DocketAlarmClient\n\n    da_client = DocketAlarmClient(<your-docketalarm-user>, <your-docketalarm-password>, <your-openai-api-key>)\n    login_token = da_client.get_login_token()\n```\n\n## search\nPerform a search on DocketAlarm API\'s search endpoint.  \n\n| Parameter    | Description                                         |\n|--------------|-----------------------------------------------------|\n| query        | The DocketAlarm query to use.                      |\n| order        | The order to get the results by.                   |\n| limit        | The search limit, must be 50 or less.              |\n| offset       | Offset for the search, useful for pagination.       |\n| login_token  | Will be created if not provided.                   |\n| return       | Dictionary with JSON response.                      |\n\n**Example**:\n\n```\n    response = da_client.search("is:docket AND is:state", "random", limit=10)\n    search_results = response["search_results"]\n```\n\n## get_docket\nInteract with getdocket endpoint, fetching a docket by court and docket number.  \n\n| Parameter       | Description                                       |\n|-----------------|---------------------------------------------------|\n| docket          | The docket number obtained from search.           |\n| court           | The court of the docket obtained from search.     |\n| timeout         | Timeout for the GET request.                      |\n| client_matter   | The client matter for the API call.               |\n| normalize       | Normalize option for getdocket endpoint.          |\n| cached          | Defaults to True, gets cached version of the docket. |\n| login_token     | If not provided it\'s auto-generated.             |\n| return          | Dictionary with JSON response.                    |\n\n**Example**:\n\n```\n    docket_data = da_client.get_docket(docket="JC205-106", court="Texas State, Grayson County, Justice of the Peace 2")\n```\n\n## get_document_binary\nFetches the binary content of a pdf stored in DocketAlarm or directly from the court.  \n\n| Parameter    | Description                                           |\n|--------------|-------------------------------------------------------|\n| doc_url      | URL for the document.                                 |\n| login_token  | Token for OpenAI authentication.                      |\n| client_matter| The matter or client for the API call.                |\n| cached       | Boolean stating if desired to use cached version of the document or not. |\n| return       | Document binary (bytes).                              |\n\n**Example**:\n\n```\n    document_bytes = da_client.get_document_binary(\n        \'https://www.docketalarm.com/cases/Arkansas_State_Faulkner_County_Circuit_Court/23DR-98-821/OCSE_V_JOHN_TAYLOR/docs/28082014_OTHER_0.pdf\'\n    )\n```\n\n# OpenAI Endpoints\n\nThese methods require the use of an OpenAI API key, suplied when initializing the instance.  \nYou can check if an OpenAI API key is valid using the `DocketAlarmClient.is_openai_valid_api_key` method.\n\n## ask_docket\nInteract with DocketAlarm\'s ask_docket OpenAI endpoint.  \n\n| Parameter       | Description                                                      |\n|-----------------|------------------------------------------------------------------|\n| docket          | The docket number as extracted from search.                      |\n| court           | The court of the docket as extracted from search.                |\n| question        | The question to ask to the docket data.                          |\n| output_format   | The output format of the desired response in natural language.   |\n| target          | The target for ask_docket, "dockets", "documents" or "both".     |\n| openai_model    | Model to be used on OpenAI interactions, defaults to gpt-3.5-turbo-1106. |\n| cached          | Gets cached version of the docket on the interaction, defaults to False. |\n| show_relevant   | Gets relevant data used by ask_docket.                           |\n| login_token     | If not provided, it is autogenerated.                           |\n| return          | Dictionary with JSON response.                                   |\n\n**Example**:\n\n```\n    response = da_client.ask_docket(docket=\'JC205-106\', court=\'Texas State, Grayson County, Justice of the Peace 2\',\n                                    question=\'is the case pre or post discovery stages?\',\n                                    output_format=\'Enum["pre" or "post" or "unknown"]\',\n                                    target="dockets", cached = True)\n\n    openai_answer = response["from_dockets"]["openai_answer"]\n```\n\n## case_matcher\nMatch a case from any input provided using DocketAlarm\'s OpenAI powered case_matcher endpoint.  \n\n| Parameter       | Description                                                      |\n|-----------------|------------------------------------------------------------------|\n| openai_model    | The OpenAI model to use during case matching.                    |\n| kwargs          | Provide any argument and it will be used as inputs in case matcher. |\n| return          | Dictionary with result from case matcher and OpenAI costs incurred. |\n\n**Example**:\n\n```\n    response = da_client.case_matcher(openai_model="gpt-4-1106-preview",\n                                    description="A PACER case involving Cloud Systems HoldCo in California")\n    case_link = response["result"]["Link"]\n```\n\n## smart_search\nReturn a query for DocketAlarm search based on instructions in natural language  \n\n| Parameter       | Description                                                     |\n|-----------------|-----------------------------------------------------------------|\n| instructions    | Instructions to build a query by.                               |\n| openai_model    | OpenAI model to be used when generating the query.              |\n| login_token     | If not provided, it will be auto-generated.                     |\n| return          | Dictionary with query and OpenAI costs incurred.                |\n\n**Example**:\n\n```\n    response = da_client.smart_search(\n        instructions="Cases involving Ford Motor in New York, that span from December 2014 to june 2019"\n    )\n    query = response["query"]\n```\n\n## attorney_billing_rates\nExtract attorney billing rates by name and state.  \n\n| Parameter       | Description                                                     |\n|-----------------|-----------------------------------------------------------------|\n| attorney_name   | The name of the attorney for which billing rates are to be extracted. |\n| state           | The state of the attorney.                                      |\n| openai_model    | OpenAI model to be used on the API call.                         |\n| login_token     | Auto-generated by default.                                      |\n| client_matter   | Empty by default.                                                |\n| return          | Dictionary with result and OpenAI costs incurred.               |\n\n**Example**\n\n```\n    response = da_client.attorney_billing_rates(attorney_name="ashley marshal",\n                                                state="connecticut")\n    attorney_data = response["result"]\n```\n\n## get_complaint_summary\nGet a summary of the legal complaint in the docket.  \n\n| Parameter       | Description                                                     |\n|-----------------|-----------------------------------------------------------------|\n| docket          | Docket number.                                                  |\n| court           | The court of the docket.                                        |\n| openai_model    | The OpenAI model to be used on the API call.                    |\n| login_token     | Auto-generated by default.                                      |\n| cached          | Bool stating if desired to use cached version of the docket.    |\n| short           | Extract a short complaint summary.                              |\n| return          | Dictionary with complaint summary and OpenAI costs incurred.    |\n\n**Example**:\n\n```\n    response = da_client.get_complaint_summary(docket="JC205-106", court="Texas State, Grayson County, Justice of the Peace 2",\n                                            short=True, openai_model="gpt-4-1106-preview", cached=True)\n    openai_answer = response["openai_answer"]\n```\n\n## get_cause_of_action\nGet the causes of action from a legal complaint.  \n\n| Parameter       | Description                                                     |\n|-----------------|-----------------------------------------------------------------|\n| docket          | Docket number.                                                  |\n| court           | The court of the docket.                                        |\n| openai_model    | The OpenAI model to be used on the API call.                    |\n| login_token     | Auto-generated by default.                                      |\n| cached          | Bool stating if desired to use cached version of the docket.    |\n| return          | Dictionary with cause of action and OpenAI costs incurred.      |\n\n**Example**:\n\n```\n    response = da_client.get_cause_of_action(docket="JC205-106", court="Texas State, Grayson County, Justice of the Peace 2",\n                                            openai_model="gpt-4-1106-preview", cached=True)\n    openai_answer = response["openai_answer"]\n```\n\n## entity_normalizer\nGet a DocketAlarm query for the entity normalized  \n\n| Parameter           | Description                                                            |\n|---------------------|------------------------------------------------------------------------|\n| entity              | The entity to normalize.                                               |\n| include_corp_group | Boolean stating if desired to include corporation group matches.       |\n| search_limit        | The internal search limit when optimizing. Must be between 10 and 50.  |\n| login_token         | If not provided, it is autogenerated.                                  |\n\n**Example**:\n\n```\n    response = da_client.entity_normalizer(entity="Apple", search_limit=20,\n                                           include_corp_group=True)\n    query = response["query"]\n```',
-    'author': 'Ezequiel Ghiena',
-    'author_email': 'ezequiel.ghiena@vlex.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://www.docketalarm.com/dockets/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+da_client = DocketAlarmClient(<your-docketalarm-user>, <your-docketalarm-password>, <your-openai-api-key>)
+```
 
+# General Endpoints
+These are methods available directly to your DocketAlarm user through a `DocketAlarmClient` instance.
 
-setup(**setup_kwargs)
+## get_login_token
+Get authentication token from docketalarm.  
+
+**Example**:
+
+```
+    from docketalarm_api import DocketAlarmClient
+
+    da_client = DocketAlarmClient(<your-docketalarm-user>, <your-docketalarm-password>, <your-openai-api-key>)
+    login_token = da_client.get_login_token()
+```
+
+## search
+Perform a search on DocketAlarm API's search endpoint.  
+
+| Parameter    | Description                                         |
+|--------------|-----------------------------------------------------|
+| query        | The DocketAlarm query to use.                       |
+| order        | The order to get the results by.                    |
+| limit        | The search limit, must be 50 or less.               |
+| offset       | Offset for the search, useful for pagination.       |
+| login_token  | Will be created if not provided.                    |
+| return       | Dictionary with JSON response.                      |
+
+**Example**:
+
+```
+    response = da_client.search("is:docket AND is:state", "random", limit=10)
+    search_results = response["search_results"]
+```
+
+## get_docket
+Interact with getdocket endpoint, fetching a docket by court and docket number.  
+
+| Parameter               | Description                                                |
+|-------------------------|------------------------------------------------------------|
+| docket                  | The docket number obtained from search.                    |
+| court                   | The court of the docket obtained from search.              |
+| timeout                 | Timeout for the GET request.                               |
+| client_matter           | The client matter for the API call.                        |
+| normalize               | Normalize option for getdocket endpoint.                   |
+| cached                  | Defaults to True, gets cached version of the docket.       |
+| login_token             | If not provided it's auto-generated.                       |
+| check_is_pacer          | Include a boolean stating if the case is from a PACER court|
+| add_documents_by_entries| Include a list of all documents per entry on the response  |
+| return                  | Dictionary with JSON response.                             |
+
+**Example**:
+
+```
+    docket_data = da_client.get_docket(docket="JC205-106", court="Texas State, Grayson County, Justice of the Peace 2")
+```
+
+## get_document_binary
+Fetches the binary content of a pdf stored in DocketAlarm or directly from the court.  
+
+| Parameter    | Description                                                              |
+|--------------|--------------------------------------------------------------------------|
+| doc_url      | URL for the document.                                                    |
+| login_token  | Token for OpenAI authentication.                                         |
+| client_matter| The matter or client for the API call.                                   |
+| cached       | Boolean stating if desired to use cached version of the document or not. |
+| return       | Document binary (bytes).                                                 |
+
+**Example**:
+
+```
+    document_bytes = da_client.get_document_binary(
+        'https://www.docketalarm.com/cases/Arkansas_State_Faulkner_County_Circuit_Court/23DR-98-821/OCSE_V_JOHN_TAYLOR/docs/28082014_OTHER_0.pdf'
+    )
+```
+
+# OpenAI Endpoints
+
+These methods require the use of an OpenAI API key, suplied when initializing the instance.  
+You can check if an OpenAI API key is valid using the `DocketAlarmClient.is_openai_valid_api_key` method.
+
+## ask_docket
+Interact with DocketAlarm's ask_docket OpenAI endpoint.  
+
+| Parameter       | Description                                                              |
+|-----------------|--------------------------------------------------------------------------|
+| docket          | The docket number as extracted from search.                              |
+| court           | The court of the docket as extracted from search.                        |
+| question        | The question to ask to the docket data.                                  |
+| output_format   | The output format of the desired response in natural language.           |
+| target          | The target for ask_docket, "docket", "documents" or "both".              |
+| openai_model    | Model to be used on OpenAI interactions, defaults to gpt-3.5-turbo-1106. |
+| cached          | Gets cached version of the docket on the interaction, defaults to False. |
+| show_relevant   | Gets relevant data used by ask_docket.                                   |
+| login_token     | If not provided, it is autogenerated.                                    |
+| return          | Dictionary with JSON response.                                           |
+
+**Example**:
+
+```
+    response = da_client.ask_docket(docket='JC205-106', court='Texas State, Grayson County, Justice of the Peace 2',
+                                    question='is the case pre or post discovery stages?',
+                                    output_format='Enum["pre" or "post" or "unknown"]',
+                                    target="docket", cached = True)
+
+    openai_answer = response["from_dockets"]["openai_answer"]
+```
+
+## case_matcher
+Match a case from any input provided using DocketAlarm's OpenAI powered case_matcher endpoint.  
+
+| Parameter       | Description                                                         |
+|-----------------|---------------------------------------------------------------------|
+| openai_model    | The OpenAI model to use during case matching.                       |
+| kwargs          | Provide any argument and it will be used as inputs in case matcher. |
+| return          | Dictionary with result from case matcher and OpenAI costs incurred. |
+
+**Example**:
+
+```
+    response = da_client.case_matcher(openai_model="gpt-4-1106-preview",
+                                    description="A PACER case involving Cloud Systems HoldCo in California")
+    case_link = response["result"]["Link"]
+```
+
+## smart_search
+Return a query for DocketAlarm search based on instructions in natural language  
+
+| Parameter       | Description                                                     |
+|-----------------|-----------------------------------------------------------------|
+| instructions    | Instructions to build a query by.                               |
+| openai_model    | OpenAI model to be used when generating the query.              |
+| login_token     | If not provided, it will be auto-generated.                     |
+| return          | Dictionary with query and OpenAI costs incurred.                |
+
+**Example**:
+
+```
+    response = da_client.smart_search(
+        instructions="Cases involving Ford Motor in New York, that span from December 2014 to june 2019"
+    )
+    query = response["query"]
+```
+
+## attorney_billing_rates
+Extract attorney billing rates by name and state.  
+
+| Parameter       | Description                                                           |
+|-----------------|-----------------------------------------------------------------------|
+| attorney_name   | The name of the attorney for which billing rates are to be extracted. |
+| state           | The state of the attorney.                                            |
+| openai_model    | OpenAI model to be used on the API call.                              |
+| login_token     | Auto-generated by default.                                            |
+| client_matter   | Empty by default.                                                     |
+| return          | Dictionary with result and OpenAI costs incurred.                     |
+
+**Example**
+
+```
+    response = da_client.attorney_billing_rates(attorney_name="ashley marshal",
+                                                state="connecticut")
+    attorney_data = response["result"]
+```
+
+## get_complaint_summary
+Get a summary of the legal complaint in the docket.  
+
+| Parameter       | Description                                                     |
+|-----------------|-----------------------------------------------------------------|
+| docket          | Docket number.                                                  |
+| court           | The court of the docket.                                        |
+| openai_model    | The OpenAI model to be used on the API call.                    |
+| login_token     | Auto-generated by default.                                      |
+| cached          | Bool stating if desired to use cached version of the docket.    |
+| short           | Extract a short complaint summary.                              |
+| return          | Dictionary with complaint summary and OpenAI costs incurred.    |
+
+**Example**:
+
+```
+    response = da_client.get_complaint_summary(docket="JC205-106", court="Texas State, Grayson County, Justice of the Peace 2",
+                                            short=True, openai_model="gpt-4-1106-preview", cached=True)
+    openai_answer = response["openai_answer"]
+```
+
+## get_cause_of_action
+Get the causes of action from a legal complaint.  
+
+| Parameter       | Description                                                     |
+|-----------------|-----------------------------------------------------------------|
+| docket          | Docket number.                                                  |
+| court           | The court of the docket.                                        |
+| openai_model    | The OpenAI model to be used on the API call.                    |
+| login_token     | Auto-generated by default.                                      |
+| cached          | Bool stating if desired to use cached version of the docket.    |
+| return          | Dictionary with cause of action and OpenAI costs incurred.      |
+
+**Example**:
+
+```
+    response = da_client.get_cause_of_action(docket="JC205-106", court="Texas State, Grayson County, Justice of the Peace 2",
+                                            openai_model="gpt-4-1106-preview", cached=True)
+    openai_answer = response["openai_answer"]
+```
+
+## entity_normalizer
+Get a DocketAlarm query for the entity normalized  
+
+| Parameter           | Description                                                            |
+|---------------------|------------------------------------------------------------------------|
+| entity              | The entity to normalize.                                               |
+| include_corp_group  | Boolean stating if desired to include corporation group matches.       |
+| search_limit        | The internal search limit when optimizing. Must be between 10 and 50.  |
+| login_token         | If not provided, it is autogenerated.                                  |
+
+**Example**:
+
+```
+    response = da_client.entity_normalizer(entity="Apple", search_limit=20,
+                                           include_corp_group=True)
+    query = response["query"]
+```
```

