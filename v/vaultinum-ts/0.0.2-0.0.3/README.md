# Comparing `tmp/vaultinum_ts-0.0.2.tar.gz` & `tmp/vaultinum_ts-0.0.3.tar.gz`

## Comparing `vaultinum_ts-0.0.2.tar` & `vaultinum_ts-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.2/2023-12-08-195515_Readme.md.tsq
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.2/2023-12-08-195515_Readme.md.tsr
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.2/2023-12-11-192549_Readme.md.tsq
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.2/2023-12-11-192549_Readme.md.tsr
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.2/2023-12-11-192943_Readme.md.tsq
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.2/2023-12-11-192943_Readme.md.tsr
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.2/requirements.txt
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.2/src/vaultinum_ts/__init__.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.2/src/vaultinum_ts/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.2/src/vaultinum_ts/__version__.py
--rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.2/src/vaultinum_ts/vaultinum_ts.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.2/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.2/LICENSE
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.2/Readme.md
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/2023-12-08-195515_Readme.md.tsq
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/2023-12-08-195515_Readme.md.tsr
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/2023-12-11-192549_Readme.md.tsq
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/2023-12-11-192549_Readme.md.tsr
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/2023-12-11-192943_Readme.md.tsq
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/2023-12-11-192943_Readme.md.tsr
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/requirements.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/src/2024-05-24-154013_Readme.md.tsq
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/src/2024-05-24-154013_Readme.md.tsr
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/src/vaultinum_ts/__init__.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/src/vaultinum_ts/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/src/vaultinum_ts/__version__.py
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/src/vaultinum_ts/vaultinum_ts.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/LICENSE
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/Readme.md
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 vaultinum_ts-0.0.3/PKG-INFO
```

### Comparing `vaultinum_ts-0.0.2/2023-12-08-195515_Readme.md.tsr` & `vaultinum_ts-0.0.3/2023-12-08-195515_Readme.md.tsr`

 * *Files identical despite different names*

### Comparing `vaultinum_ts-0.0.2/2023-12-11-192549_Readme.md.tsr` & `vaultinum_ts-0.0.3/2023-12-11-192549_Readme.md.tsr`

 * *Files identical despite different names*

### Comparing `vaultinum_ts-0.0.2/2023-12-11-192943_Readme.md.tsr` & `vaultinum_ts-0.0.3/2023-12-11-192943_Readme.md.tsr`

 * *Files identical despite different names*

### Comparing `vaultinum_ts-0.0.2/src/vaultinum_ts/vaultinum_ts.py` & `vaultinum_ts-0.0.3/src/vaultinum_ts/vaultinum_ts.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     with open(ts_req_filename, mode="wb") as output_file:
         output_file.write(encoded_tsq)
         output_file.close()
 
     TS_URL = TS_ENVIRONMENTS[environment]
     print(f'Sending request to the timestamp service: {TS_URL}')
     TS_HEADERS = {
-        'Bearer': f'Bearer {apikey}',
+        'Authorization': f'Bearer {apikey}',
         'Content-Type': 'application/timestamp-query'
     }
     r = requests.post(TS_URL, headers=TS_HEADERS, data=encoded_tsq)
 
     # Save the timestamp response to disk
     ts_res_filename = 'tmp_req_output_file'
     if r.status_code != 200:
```

### Comparing `vaultinum_ts-0.0.2/LICENSE` & `vaultinum_ts-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vaultinum_ts-0.0.2/Readme.md` & `vaultinum_ts-0.0.3/Readme.md`

 * *Files identical despite different names*

### Comparing `vaultinum_ts-0.0.2/pyproject.toml` & `vaultinum_ts-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vaultinum_ts-0.0.2/PKG-INFO` & `vaultinum_ts-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: vaultinum_ts
-Version: 0.0.2
+Version: 0.0.3
 Summary: Client for Vaultinum's timestamping service.
 Project-URL: Homepage, https://github.com/vaultinum/vaultinum-timestamping-sdk
 Project-URL: Documentation, https://docs.vaultinum.com
 Project-URL: Issues, https://github.com/vaultinum/vaultinum-timestamping-sdk/issues
 Author-email: Vaultinum <contact@vaultinum.com>
 License: MIT License
```

