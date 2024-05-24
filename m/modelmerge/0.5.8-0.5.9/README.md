# Comparing `tmp/modelmerge-0.5.8.tar.gz` & `tmp/modelmerge-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.5.8.tar", last modified: Wed May 22 20:37:02 2024, max compression
+gzip compressed data, was "modelmerge-0.5.9.tar", last modified: Fri May 24 07:34:59 2024, max compression
```

## Comparing `modelmerge-0.5.8.tar` & `modelmerge-0.5.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:37:02.269773 modelmerge-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-22 20:36:54.000000 modelmerge-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-22 20:37:02.269773 modelmerge-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-22 20:36:54.000000 modelmerge-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:37:02.269773 modelmerge-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-22 20:36:54.000000 modelmerge-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:37:02.257773 modelmerge-0.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:37:02.257773 modelmerge-0.5.8/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:37:02.257773 modelmerge-0.5.8/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    25436 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    16024 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:37:02.261773 modelmerge-0.5.8/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/plugins/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/plugins/run_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:37:02.261773 modelmerge-0.5.8/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/tools/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/tools/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/tools/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:37:02.261773 modelmerge-0.5.8/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-22 20:36:54.000000 modelmerge-0.5.8/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:37:02.265773 modelmerge-0.5.8/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-22 20:37:02.000000 modelmerge-0.5.8/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-22 20:37:02.000000 modelmerge-0.5.8/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:37:02.000000 modelmerge-0.5.8/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-22 20:37:02.000000 modelmerge-0.5.8/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 20:37:02.000000 modelmerge-0.5.8/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:37:02.265773 modelmerge-0.5.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_API.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_Web_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_claude_zh_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_get_token_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_langchain_search_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_py_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_tikitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-22 20:36:54.000000 modelmerge-0.5.8/test/test_whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:34:59.442255 modelmerge-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-24 07:34:51.000000 modelmerge-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-24 07:34:59.442255 modelmerge-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-24 07:34:51.000000 modelmerge-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 07:34:59.442255 modelmerge-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-24 07:34:51.000000 modelmerge-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:34:59.430255 modelmerge-0.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:34:59.434255 modelmerge-0.5.9/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:34:59.434255 modelmerge-0.5.9/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25449 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16024 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:34:59.434255 modelmerge-0.5.9/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/plugins/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/plugins/run_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:34:59.434255 modelmerge-0.5.9/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/tools/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/tools/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/tools/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:34:59.438255 modelmerge-0.5.9/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-24 07:34:51.000000 modelmerge-0.5.9/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:34:59.442255 modelmerge-0.5.9/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-24 07:34:59.000000 modelmerge-0.5.9/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-24 07:34:59.000000 modelmerge-0.5.9/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 07:34:59.000000 modelmerge-0.5.9/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-24 07:34:59.000000 modelmerge-0.5.9/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 07:34:59.000000 modelmerge-0.5.9/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:34:59.442255 modelmerge-0.5.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_get_token_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_py_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-24 07:34:51.000000 modelmerge-0.5.9/test/test_whisper.py
```

### Comparing `modelmerge-0.5.8/LICENSE` & `modelmerge-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/PKG-INFO` & `modelmerge-0.5.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.5.8
+Version: 0.5.9
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.5.8/README.md` & `modelmerge-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/src/ModelMerge/models/base.py` & `modelmerge-0.5.9/src/ModelMerge/models/base.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.5.9/src/ModelMerge/models/chatgpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,15 +427,15 @@
             else:
                 self.function_calls_counter[function_call_name] += 1
             if self.function_calls_counter[function_call_name] <= self.function_call_max_loop:
                 function_call_max_tokens = self.truncate_limit - message_token["total"] - 1000
                 if function_call_max_tokens <= 0:
                     function_call_max_tokens = int(self.truncate_limit / 2)
                 print("\033[32m function_call", function_call_name, "max token:", function_call_max_tokens, "\033[0m")
-                function_response = yield from get_tools_result(function_call_name, function_full_response, function_call_max_tokens, self.engine, chatgpt, self.api_key, self.api_url, use_plugins=False)
+                function_response = yield from get_tools_result(function_call_name, function_full_response, function_call_max_tokens, self.engine, chatgpt, self.api_key, self.api_url, use_plugins=False, model=model)
             else:
                 function_response = "无法找到相关信息，停止使用 tools"
             response_role = "function"
             # print(self.conversation[convo_id][-1])
             if self.conversation[convo_id][-1]["role"] == "function" and self.conversation[convo_id][-1]["name"] == "get_search_results":
                 mess = self.conversation[convo_id].pop(-1)
                 # print("Truncate message:", mess)
```

### Comparing `modelmerge-0.5.8/src/ModelMerge/models/claude.py` & `modelmerge-0.5.9/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/src/ModelMerge/models/genimi.py` & `modelmerge-0.5.9/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/src/ModelMerge/models/groq.py` & `modelmerge-0.5.9/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/src/ModelMerge/plugins/config.py` & `modelmerge-0.5.9/src/ModelMerge/plugins/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/src/ModelMerge/plugins/image.py` & `modelmerge-0.5.9/src/ModelMerge/plugins/image.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.5.9/src/ModelMerge/plugins/tarvel.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.5.9/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/src/ModelMerge/tools/chatgpt.py` & `modelmerge-0.5.9/src/ModelMerge/tools/chatgpt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/src/ModelMerge/tools/claude.py` & `modelmerge-0.5.9/src/ModelMerge/tools/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/src/ModelMerge/tools/run.py` & `modelmerge-0.5.9/src/ModelMerge/tools/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from ..utils.prompt import search_key_word_prompt
 
 from ..plugins import *
 
 LANGUAGE = os.environ.get('LANGUAGE', 'Simplified Chinese')
 
 
-def get_tools_result(function_call_name, function_full_response, function_call_max_tokens, engine, robot, api_key, api_url, use_plugins):
+def get_tools_result(function_call_name, function_full_response, function_call_max_tokens, engine, robot, api_key, api_url, use_plugins, model):
     if function_call_name == "get_search_results":
         prompt = json.loads(function_full_response)["prompt"]
         yield "🌐 正在搜索您的问题，提取关键词..."
         llm = robot(api_key=api_key, api_url=api_url.source_api_url, engine=engine, use_plugins=use_plugins)
-        keywords = llm.ask(search_key_word_prompt.format(source=prompt)).split("\n")
+        keywords = llm.ask(search_key_word_prompt.format(source=prompt), model=model).split("\n")
         function_response = yield from eval(function_call_name)(prompt, keywords)
         function_call_max_tokens = 32000
         function_response, text_len = cut_message(function_response, function_call_max_tokens, engine)
         if function_response:
             function_response = (
                 f"You need to response the following question: {prompt}. Search results is provided inside <Search_results></Search_results> XML tags. Your task is to think about the question step by step and then answer the above question in {LANGUAGE} based on the Search results provided. Please response in {LANGUAGE} and adopt a style that is logical, in-depth, and detailed. Note: In order to make the answer appear highly professional, you should be an expert in textual analysis, aiming to make the answer precise and comprehensive. Directly response markdown format, without using markdown code blocks"
                 "Here is the Search results, inside <Search_results></Search_results> XML tags:"
```

### Comparing `modelmerge-0.5.8/src/ModelMerge/utils/prompt.py` & `modelmerge-0.5.9/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/src/ModelMerge/utils/scripts.py` & `modelmerge-0.5.9/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.5.9/src/modelmerge.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.5.8
+Version: 0.5.9
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.5.8/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.5.9/src/modelmerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/test/test_Web_crawler.py` & `modelmerge-0.5.9/test/test_Web_crawler.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/test/test_claude_zh_char.py` & `modelmerge-0.5.9/test/test_claude_zh_char.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/test/test_ddg_search.py` & `modelmerge-0.5.9/test/test_ddg_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/test/test_download_pdf.py` & `modelmerge-0.5.9/test/test_download_pdf.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/test/test_get_token_dict.py` & `modelmerge-0.5.9/test/test_get_token_dict.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/test/test_google_search.py` & `modelmerge-0.5.9/test/test_google_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/test/test_jieba.py` & `modelmerge-0.5.9/test/test_jieba.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/test/test_json.py` & `modelmerge-0.5.9/test/test_json.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/test/test_langchain_search_old.py` & `modelmerge-0.5.9/test/test_langchain_search_old.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/test/test_logging.py` & `modelmerge-0.5.9/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/test/test_ollama.py` & `modelmerge-0.5.9/test/test_ollama.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/test/test_py_run.py` & `modelmerge-0.5.9/test/test_py_run.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/test/test_requests.py` & `modelmerge-0.5.9/test/test_requests.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/test/test_tikitoken.py` & `modelmerge-0.5.9/test/test_tikitoken.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/test/test_token.py` & `modelmerge-0.5.9/test/test_token.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.8/test/test_url.py` & `modelmerge-0.5.9/test/test_url.py`

 * *Files identical despite different names*

