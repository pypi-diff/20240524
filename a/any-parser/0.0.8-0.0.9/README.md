# Comparing `tmp/any_parser-0.0.8.tar.gz` & `tmp/any_parser-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "any_parser-0.0.8.tar", max compression
+gzip compressed data, was "any_parser-0.0.9.tar", max compression
```

## Comparing `any_parser-0.0.8.tar` & `any_parser-0.0.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1882 2024-05-06 06:10:36.107663 any_parser-0.0.8/README.md
--rw-r--r--   0        0        0       86 2024-05-06 06:10:36.107818 any_parser-0.0.8/any_parser/__init__.py
--rw-r--r--   0        0        0     3481 2024-05-06 06:10:36.107942 any_parser-0.0.8/any_parser/base.py
--rw-r--r--   0        0        0      388 2024-05-06 06:10:36.116825 any_parser-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 any_parser-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1882 2024-05-06 06:10:36.107663 any_parser-0.0.9/README.md
+-rw-r--r--   0        0        0       86 2024-05-07 07:53:27.937223 any_parser-0.0.9/any_parser/__init__.py
+-rw-r--r--   0        0        0     3490 2024-05-07 07:53:27.937625 any_parser-0.0.9/any_parser/base.py
+-rw-r--r--   0        0        0      388 2024-05-07 07:53:27.941749 any_parser-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 any_parser-0.0.9/PKG-INFO
```

### Comparing `any_parser-0.0.8/README.md` & `any_parser-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `any_parser-0.0.8/any_parser/base.py` & `any_parser-0.0.9/any_parser/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self._request_header = {"x-api-key": apiKey}
 
     def extract(self, file_path):
         user_id, job_id, s3_key = self._request_and_upload_by_apiKey(file_path)
         result = self._request_file_extraction(user_id, job_id, s3_key)
         return json.loads(result)["result"]
 
-    def parse(self, file_path, prompt, mode="advanced"):
+    def parse(self, file_path, prompt="", mode="advanced"):
         user_id, job_id, s3_key = self._request_and_upload_by_apiKey(file_path)
         result = self._request_info_extraction(user_id, job_id, s3_key, mode, prompt)
         return json.loads(result)["result"]
 
     def _error_handler(self, response):
         if response.status_code == 403:
             raise Exception("Invalid API Key")
@@ -52,15 +52,15 @@
             uid = response.json()["userId"]
             jid = response.json()["jobId"]
             with open(file_path, "rb") as file_to_upload:
                 files = {"file": (file_path, file_to_upload)}
                 upload_response = requests.post(
                     url_info["url"], data=url_info["fields"], files=files
                 )
-            print(f"Upload response: {upload_response.status_code}")
+            # print(f"Upload response: {upload_response.status_code}")
             return uid, jid, url_info["fields"]["key"]
 
         self._error_handler(response)
 
     def _request_file_extraction(self, user_id, job_id, s3_key):
         payload = {
             "userId": user_id,
@@ -68,15 +68,15 @@
             "fileKey": s3_key,
         }
         response = requests.post(
             self._extracturl, headers=self._request_header, json=payload
         )
 
         if response.status_code == 200:
-            print("Extraction success.")
+            # print("Extraction success.")
             return response.text
 
         self._error_handler(response)
 
     def _request_info_extraction(self, user_id, job_id, s3_key, mode, prompt=""):
         if mode not in ["advanced", "basic"]:
             raise ValueError("Invalid mode. Choose either 'advanced' or 'basic'.")
@@ -88,11 +88,11 @@
             "use_textract": "True" if mode == "advanced" else "False",
         }
         response = requests.post(
             self._parseurl, headers=self._request_header, json=payload
         )
 
         if response.status_code == 200:
-            print("Extraction success.")
+            # print("Extraction success.")
             return response.text
 
         self._error_handler(response)
```

### Comparing `any_parser-0.0.8/PKG-INFO` & `any_parser-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: any-parser
-Version: 0.0.8
+Version: 0.0.9
 Summary: Parser for all.
 Author: CambioML
 Author-email: wanwanaiai45@gmail.com
 Maintainer: Rachel Hu
 Maintainer-email: goldpiggy@berkeley.edu
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
```

