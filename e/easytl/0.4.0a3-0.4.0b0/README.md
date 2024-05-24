# Comparing `tmp/easytl-0.4.0a3.tar.gz` & `tmp/easytl-0.4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytl-0.4.0a3.tar", last modified: Thu May 23 01:24:54 2024, max compression
+gzip compressed data, was "easytl-0.4.0b0.tar", last modified: Fri May 24 01:30:57 2024, max compression
```

## Comparing `easytl-0.4.0a3.tar` & `easytl-0.4.0b0.tar`

### file list

```diff
@@ -1,35 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:24:54.253780 easytl-0.4.0a3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:24:54.249780 easytl-0.4.0a3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:24:54.249780 easytl-0.4.0a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-23 01:23:17.000000 easytl-0.4.0a3/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-23 01:23:17.000000 easytl-0.4.0a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-23 01:23:17.000000 easytl-0.4.0a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-05-23 01:24:54.253780 easytl-0.4.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-05-23 01:23:17.000000 easytl-0.4.0a3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-23 01:23:17.000000 easytl-0.4.0a3/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-23 01:23:17.000000 easytl-0.4.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 01:24:54.253780 easytl-0.4.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:24:54.249780 easytl-0.4.0a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:24:54.253780 easytl-0.4.0a3/src/easytl/
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17912 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/anthropic_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/deepl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    96843 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/easytl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16117 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/gemini_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/googletl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    17576 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/openai_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    39556 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:24:54.253780 easytl-0.4.0a3/src/easytl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-05-23 01:24:54.000000 easytl-0.4.0a3/src/easytl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-23 01:24:54.000000 easytl-0.4.0a3/src/easytl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:24:54.000000 easytl-0.4.0a3/src/easytl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-23 01:24:54.000000 easytl-0.4.0a3/src/easytl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 01:24:54.000000 easytl-0.4.0a3/src/easytl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:24:54.253780 easytl-0.4.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-23 01:23:17.000000 easytl-0.4.0a3/tests/issue_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-05-23 01:23:17.000000 easytl-0.4.0a3/tests/passing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-23 01:23:17.000000 easytl-0.4.0a3/tests/simple_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.744840 easytl-0.4.0b0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.740841 easytl-0.4.0b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.740841 easytl-0.4.0b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-24 01:28:55.000000 easytl-0.4.0b0/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-24 01:28:55.000000 easytl-0.4.0b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-24 01:28:55.000000 easytl-0.4.0b0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-24 01:30:57.744840 easytl-0.4.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-05-24 01:28:55.000000 easytl-0.4.0b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-24 01:28:55.000000 easytl-0.4.0b0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-24 01:28:55.000000 easytl-0.4.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-24 01:28:55.000000 easytl-0.4.0b0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 01:30:57.744840 easytl-0.4.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.740841 easytl-0.4.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.740841 easytl-0.4.0b0/src/easytl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105332 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/easytl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.744840 easytl-0.4.0b0/src/easytl/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/services/anthropic_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/services/azure_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/services/deepl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/services/gemini_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/services/googletl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17689 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/services/openai_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.744840 easytl-0.4.0b0/src/easytl/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14452 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/util/llm_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18474 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.744840 easytl-0.4.0b0/src/easytl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-24 01:30:57.000000 easytl-0.4.0b0/src/easytl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-24 01:30:57.000000 easytl-0.4.0b0/src/easytl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:30:57.000000 easytl-0.4.0b0/src/easytl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-24 01:30:57.000000 easytl-0.4.0b0/src/easytl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 01:30:57.000000 easytl-0.4.0b0/src/easytl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.744840 easytl-0.4.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-24 01:28:55.000000 easytl-0.4.0b0/tests/issue_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19390 2024-05-24 01:28:55.000000 easytl-0.4.0b0/tests/passing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-05-24 01:28:55.000000 easytl-0.4.0b0/tests/simple_test.py
```

### Comparing `easytl-0.4.0a3/.github/workflows/workflow.yml` & `easytl-0.4.0b0/.github/workflows/workflow.yml`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,16 @@
       - name: Set Environment Variables and Run Tests
         env:
           DEEPL_API_KEY: ${{ secrets.DEEPL_API_KEY }}
           GEMINI_API_KEY: ${{ secrets.GEMINI_API_KEY }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
           ANTHROPIC_API_KEY: ${{ secrets.ANTHROPIC_API_KEY }}
           GOOGLE_TRANSLATE_SERVICE_KEY_VALUE: ${{ secrets.GOOGLE_TRANSLATE_SERVICE_KEY_VALUE }}
+          AZURE_API_KEY: ${{ secrets.AZURE_API_KEY }}
+          AZURE_REGION: ${{ secrets.AZURE_REGION }}
           LOGGING_DIRECTORY: /tmp/
         run: |
           python tests/passing.py
 
       - name: Build the package
         run: |
           python -m build
@@ -66,14 +68,16 @@
       - name: Set Environment Variables and Run Tests
         env:
           DEEPL_API_KEY: ${{ secrets.DEEPL_API_KEY }}
           GEMINI_API_KEY: ${{ secrets.GEMINI_API_KEY }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
           ANTHROPIC_API_KEY: ${{ secrets.ANTHROPIC_API_KEY }}
           GOOGLE_TRANSLATE_SERVICE_KEY_VALUE: ${{ secrets.GOOGLE_TRANSLATE_SERVICE_KEY_VALUE }}
+          AZURE_API_KEY: ${{ secrets.AZURE_API_KEY }}
+          AZURE_REGION: ${{ secrets.AZURE_REGION }}
           LOGGING_DIRECTORY: /tmp/
         run: |
           python tests/passing.py
 
       - name: Build the package
         run: |
           python -m build
@@ -103,14 +107,16 @@
       - name: Set Environment Variables and Run Tests
         env:
           DEEPL_API_KEY: ${{ secrets.DEEPL_API_KEY }}
           GEMINI_API_KEY: ${{ secrets.GEMINI_API_KEY }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
           ANTHROPIC_API_KEY: ${{ secrets.ANTHROPIC_API_KEY }}
           GOOGLE_TRANSLATE_SERVICE_KEY_VALUE: ${{ secrets.GOOGLE_TRANSLATE_SERVICE_KEY_VALUE }}
+          AZURE_API_KEY: ${{ secrets.AZURE_API_KEY }}
+          AZURE_REGION: ${{ secrets.AZURE_REGION }}
           LOGGING_DIRECTORY: /tmp/
         run: |
           python tests/passing.py
 
       - name: Install twine
         run: |
           python -m pip install twine
```

### Comparing `easytl-0.4.0a3/.gitignore` & `easytl-0.4.0b0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -163,7 +163,12 @@
 ## test files
 tests/gemini.txt
 tests/openai.txt
 tests/deepl.txt
 tests/easytl-log.txt
 tests/google_translate_key.json
 tests/anthropic.txt
+tests/azure.txt
+tests/azure_region.txt
+
+# For MacOS
+.DS_Store
```

### Comparing `easytl-0.4.0a3/LICENSE.md` & `easytl-0.4.0b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a3/PKG-INFO` & `easytl-0.4.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.4.0a3
-Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
-Author-email: Bikatr7 <Bikatr7@proton.me>
+Version: 0.4.0b0
+Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini, Google Translate and More.
+Author-email: "Kaden Bilyeu (Bikatr7)" <Bikatr7@proton.me>, Alejandro Mata <alemalvarez@icloud.com>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,15 @@
 Requires-Dist: google-generativeai==0.5.4
 Requires-Dist: deepl==1.16.1
 Requires-Dist: openai==1.29.0
 Requires-Dist: backoff==2.2.1
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: google-cloud-translate==3.15.3
 Requires-Dist: anthropic==0.26.0
+Requires-Dist: requests>=2.31.0
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Table of Contents**
 
 - [Quick Start](#quick-start)
 - [Installation](#installation)
 - [Features](#features)
```

### Comparing `easytl-0.4.0a3/README.md` & `easytl-0.4.0b0/README.md`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a3/SECURITY.md` & `easytl-0.4.0b0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a3/pyproject.toml` & `easytl-0.4.0b0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -12,23 +12,25 @@
 dependencies = [
     "google-generativeai==0.5.4",
     "deepl==1.16.1",
     "openai==1.29.0",
     "backoff==2.2.1",
     "tiktoken==0.6.0",
     "google-cloud-translate==3.15.3",
-    "anthropic==0.26.0"
+    "anthropic==0.26.0",
+    "requests>=2.31.0",
 ]
 
 name = "easytl"
-version = "v0.4.0-alpha-3"
+version = "v0.4.0-beta"
 authors = [
-  { name="Bikatr7", email="Bikatr7@proton.me" },
-]
-description = "Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate."
+  { name="Kaden Bilyeu (Bikatr7)", email="Bikatr7@proton.me"},
+  { name="Alejandro Mata", email="alemalvarez@icloud.com"},
+] 
+description = "Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini, Google Translate and More."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
```

### Comparing `easytl-0.4.0a3/src/easytl/__init__.py` & `easytl-0.4.0b0/src/easytl/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-## Copyright Bikatr7 (https://github.com/Bikatr7)
-## Use of this source code is governed by a GNU Lesser General Public License v2.1
+## Copyright (C) 2024 Kaden Bilyeu (Bikatr7) (https://github.com/Bikatr7), Alejandro Mata (https://github.com/alemalvarez)
+## Use of this source code is governed by an GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 from .version import VERSION as __version__  # noqa
 
 __author__ = "Bikatr7 <Tetralon07@gmail.com>"
 
 from .easytl import EasyTL
@@ -11,28 +11,31 @@
 from .classes import Language, SplitSentences, Formality, GlossaryInfo, TextResult
 from .classes import Message, SystemTranslationMessage, ModelTranslationMessage
 from .classes import ChatCompletion
 from .classes import GenerateContentResponse, AsyncGenerateContentResponse, GenerationConfig
 from .classes import AnthropicMessage, AnthropicTextBlock, AnthropicToolsBetaMessage, AnthropicToolUseBlock
 from .classes import NOT_GIVEN, NotGiven
 
-from .util import MODEL_COSTS, ALLOWED_GEMINI_MODELS, ALLOWED_OPENAI_MODELS, ALLOWED_ANTHROPIC_MODELS, VALID_JSON_OPENAI_MODELS, VALID_JSON_GEMINI_MODELS, VALID_JSON_ANTHROPIC_MODELS, MODEL_MAX_TOKENS
+from .util.constants import MODEL_COSTS, ALLOWED_GEMINI_MODELS, ALLOWED_OPENAI_MODELS, ALLOWED_ANTHROPIC_MODELS, VALID_JSON_OPENAI_MODELS, VALID_JSON_GEMINI_MODELS, VALID_JSON_ANTHROPIC_MODELS, MODEL_MAX_TOKENS
 
 ## deepL generic exception
 from .exceptions import DeepLException
 
 ## google generic exception
 from .exceptions import GoogleAPIError
 
 ## openai generic exception
 from .exceptions import OpenAIError
 
 ## anthropic generic exception
 from .exceptions import AnthropicError
 
+## azure generic exception
+from .exceptions import RequestException
+
 ## service specific exceptions
 from .exceptions import OpenAIAPIError, OpenAIConflictError, OpenAINotFoundError, OpenAIAPIStatusError, OpenAIRateLimitError, OpenAIAPITimeoutError, OpenAIBadRequestError, OpenAIAPIConnectionError, OpenAIAuthenticationError, OpenAIInternalServerError, OpenAIPermissionDeniedError, OpenAIUnprocessableEntityError, OpenAIAPIResponseValidationError
 from .exceptions import DeepLAuthorizationException, DeepLQuotaExceededException, DeepLConnectionException, DeepLTooManyRequestsException, DeepLDocumentNotReadyException, DeepLGlossaryNotFoundException, DeepLDocumentTranslationException
 from .exceptions import GoogleAuthError, GoogleDefaultCredentialsError
 from .exceptions import AnthropicAPIError, AnthropicConflictError, AnthropicNotFoundError, AnthropicAPIStatusError, AnthropicRateLimitError, AnthropicAPITimeoutError, AnthropicBadRequestError, AnthropicAPIConnectionError, AnthropicAuthenticationError, AnthropicInternalServerError, AnthropicPermissionDeniedError, AnthropicUnprocessableEntityError, AnthropicAPIResponseValidationError
 
 __all__ = [
@@ -44,12 +47,13 @@
     "AnthropicMessage","AnthropicTextBlock", "AnthropicToolsBetaMessage", "AnthropicToolUseBlock",
     "NOT_GIVEN","NotGiven",
     "MODEL_COSTS", "ALLOWED_GEMINI_MODELS", "ALLOWED_OPENAI_MODELS", "ALLOWED_ANTHROPIC_MODELS", "VALID_JSON_OPENAI_MODELS", "VALID_JSON_GEMINI_MODELS", "VALID_JSON_ANTHROPIC_MODELS", "MODEL_MAX_TOKENS",
     "DeepLException",
     "GoogleAPIError",
     "OpenAIError",
     "AnthropicError",
+    "RequestException",
     "OpenAIAPIError", "OpenAIConflictError", "OpenAINotFoundError", "OpenAIAPIStatusError", "OpenAIRateLimitError", "OpenAIAPITimeoutError", "OpenAIBadRequestError", "OpenAIAPIConnectionError", "OpenAIAuthenticationError", "OpenAIInternalServerError", "OpenAIPermissionDeniedError", "OpenAIUnprocessableEntityError", "OpenAIAPIResponseValidationError",
     "DeepLAuthorizationException", "DeepLQuotaExceededException", "DeepLConnectionException", "DeepLTooManyRequestsException", "DeepLDocumentNotReadyException", "DeepLGlossaryNotFoundException", "DeepLDocumentTranslationException",
     "GoogleAuthError", "GoogleDefaultCredentialsError",
     "AnthropicAPIError", "AnthropicConflictError", "AnthropicNotFoundError", "AnthropicAPIStatusError", "AnthropicRateLimitError", "AnthropicAPITimeoutError", "AnthropicBadRequestError", "AnthropicAPIConnectionError", "AnthropicAuthenticationError", "AnthropicInternalServerError", "AnthropicPermissionDeniedError", "AnthropicUnprocessableEntityError", "AnthropicAPIResponseValidationError"
 ]
```

### Comparing `easytl-0.4.0a3/src/easytl/anthropic_service.py` & `easytl-0.4.0b0/src/easytl/services/anthropic_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-## Copyright Bikatr7 (https://github.com/Bikatr7)
-## Use of this source code is governed by a GNU Lesser General Public License v2.1
+## Copyright (C) 2024 Kaden Bilyeu (Bikatr7) (https://github.com/Bikatr7), Alejandro Mata (https://github.com/alemalvarez)
+## Use of this source code is governed by an GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 ## built-in libraries
 import typing
 import asyncio
 
 ## third-party imports
 from anthropic import Anthropic, AsyncAnthropic
 
 ## custom modules
-from .exceptions import EasyTLException
-from .classes import ModelTranslationMessage, NotGiven, NOT_GIVEN, AnthropicMessage, AnthropicToolsBetaMessage
-from .util import VALID_JSON_ANTHROPIC_MODELS, _is_iterable_of_strings, _convert_iterable_to_str, _estimate_cost
-from .decorators import _sync_logging_decorator, _async_logging_decorator
+from ..exceptions import EasyTLException
+from ..classes import ModelTranslationMessage, NotGiven, NOT_GIVEN, AnthropicMessage, AnthropicToolsBetaMessage
+from ..decorators import _sync_logging_decorator, _async_logging_decorator
+
+from ..util.util import _is_iterable_of_strings, _convert_iterable_to_str, _estimate_cost
+from ..util.constants import VALID_JSON_ANTHROPIC_MODELS
+
 
 class AnthropicService:
 
     _default_model:str = "claude-3-haiku-20240307"
     _default_translation_instructions:str = "Please translate the following text into English."
 
     _system:str | None   = _default_translation_instructions
```

### Comparing `easytl-0.4.0a3/src/easytl/classes.py` & `easytl-0.4.0b0/src/easytl/classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## Copyright Bikatr7 (https://github.com/Bikatr7)
+## Copyright (C) 2024 Kaden Bilyeu (Bikatr7) (https://github.com/Bikatr7), Alejandro Mata (https://github.com/alemalvarez)
 ## Use of this source code is governed by an GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 ## built-in libraries
 from typing_extensions import override
 
 import typing
```

### Comparing `easytl-0.4.0a3/src/easytl/decorators.py` & `easytl-0.4.0b0/src/easytl/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-## Copyright Bikatr7 (https://github.com/Bikatr7)
-## Use of this source code is governed by a GNU Lesser General Public License v2.1
+## Copyright (C) 2024 Kaden Bilyeu (Bikatr7) (https://github.com/Bikatr7), Alejandro Mata (https://github.com/alemalvarez)
+## Use of this source code is governed by an GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 ## built-in libraries
 from functools import wraps
 
 import datetime
 import os
@@ -167,9 +167,12 @@
     'OpenAIService': [[('choices', None), ('0', None), ('message', None), ('content', None)],
                       [('choices', None), ('0', None), ('message', None), ('content', None)],
                       ],
     'GoogleTLService': [('translatedText', None)],
     'AnthropicService': [
         [('content', None), ('0', None), ('text', AnthropicTextBlock)],
         [('content', None), ('0', None), ('input', AnthropicToolUseBlock)]
+    ],
+    'AzureService': [
+        [('0', None), ('translations', None), ('0', None), ('text', None)]
     ]
 }
```

### Comparing `easytl-0.4.0a3/src/easytl/deepl_service.py` & `easytl-0.4.0b0/src/easytl/services/deepl_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## Copyright Bikatr7 (https://github.com/Bikatr7)
+## Copyright (C) 2024 Kaden Bilyeu (Bikatr7) (https://github.com/Bikatr7), Alejandro Mata (https://github.com/alemalvarez)
 ## Use of this source code is governed by an GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 ## built-in libraries
 import typing
 import asyncio
 import time
@@ -10,18 +10,18 @@
 
 ## third-party libraries
 from deepl.translator import Translator
 
 import deepl
 
 ## custom modules
-from .version import VERSION
-from .util import _convert_iterable_to_str
-from .decorators import _async_logging_decorator, _sync_logging_decorator
-from .classes import Language, SplitSentences, Formality, GlossaryInfo, TextResult
+from ..version import VERSION
+from ..util.util import _convert_iterable_to_str
+from ..decorators import _async_logging_decorator, _sync_logging_decorator
+from ..classes import Language, SplitSentences, Formality, GlossaryInfo, TextResult
 
 class DeepLService:
 
     _api_key:str = ""
     
     _translator:Translator
 
@@ -34,15 +34,15 @@
     _glossary:str | GlossaryInfo | None = None
     _tag_handling:typing.Literal["xml", "html"] | None = None
     _outline_detection:bool | None = None
     _non_splitting_tags:str | typing.List[str] | None = None
     _splitting_tags:str | typing.List[str] | None = None
     _ignore_tags:str | typing.List[str] | None = None
 
-    _semaphore_value:int = 30
+    _semaphore_value:int = 15
     _semaphore:asyncio.Semaphore = asyncio.Semaphore(_semaphore_value)
 
     _rate_limit_delay:float | None = None 
 
     _decorator_to_use:typing.Union[typing.Callable, None] = None
 
     _log_directory:str | None = None
```

### Comparing `easytl-0.4.0a3/src/easytl/easytl.py` & `easytl-0.4.0b0/src/easytl/easytl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-## Copyright Bikatr7 (https://github.com/Bikatr7)
-## Use of this source code is governed by a GNU Lesser General Public License v2.1
+## Copyright (C) 2024 Kaden Bilyeu (Bikatr7) (https://github.com/Bikatr7), Alejandro Mata (https://github.com/alemalvarez)
+## Use of this source code is governed by an GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 ## built-in libraries
 import typing
 import asyncio
 
 import warnings
 
 ## third-party libraries
 from .classes import Language, SplitSentences, Formality, GlossaryInfo, NOT_GIVEN, NotGiven
 
 ## custom modules
-from .deepl_service import DeepLService
-from .gemini_service import GeminiService
-from .openai_service import OpenAIService
-from .googletl_service import GoogleTLService
-from .anthropic_service import AnthropicService
+from .services.deepl_service import DeepLService
+from .services.gemini_service import GeminiService
+from .services.openai_service import OpenAIService
+from .services.googletl_service import GoogleTLService
+from .services.anthropic_service import AnthropicService
+from .services.azure_service import AzureService
 
 from. classes import ModelTranslationMessage, SystemTranslationMessage, TextResult, GenerateContentResponse, AsyncGenerateContentResponse, ChatCompletion, AnthropicMessage, AnthropicToolsBetaMessage, AnthropicTextBlock, AnthropicToolUseBlock
-from .exceptions import DeepLException, GoogleAPIError, OpenAIError, InvalidAPITypeException, InvalidResponseFormatException, InvalidTextInputException, EasyTLException, AnthropicError
+from .exceptions import DeepLException, GoogleAPIError, OpenAIError, InvalidAPITypeException, InvalidResponseFormatException, InvalidTextInputException, EasyTLException, AnthropicError, RequestException
 
-from .util import _validate_easytl_translation_settings, _is_iterable_of_strings, _return_curated_gemini_settings, _return_curated_openai_settings, _validate_stop_sequences, _validate_response_schema,  _return_curated_anthropic_settings, _validate_text_length
+from .util.util import _is_iterable_of_strings
+from .util.llm_util import _validate_easytl_llm_translation_settings, _return_curated_gemini_settings, _return_curated_openai_settings, _validate_stop_sequences, _validate_response_schema,  _return_curated_anthropic_settings, _validate_text_length 
 
 class EasyTL:
 
     """
     
     EasyTL global client, used to interact with Translation APIs.
 
@@ -37,49 +39,18 @@
 
     Use calculate_cost() to calculate the cost of translating text using the specified service. (Optional)
 
     See the documentation for each function for more information.
 
     """
 
-##-------------------start-of-set_api_key()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-    @staticmethod
-    def set_api_key(api_type:typing.Literal["deepl", "gemini", "openai"], api_key:str) -> None:
-        
-        """
-
-        Sets the API key for the specified API type.
-        For Google Translate, use set_credentials() instead.
-
-        Deprecated: This function is deprecated and will be removed in a future version.
-        Use set_credentials(auth_info) instead.
-
-        Parameters:
-        api_type (literal["deepl", "gemini", "openai"]) : The API type to set the key for.
-        api_key (string) : The API key to set.
-
-        """
-
-        warnings.warn("set_api_key is deprecated and will be removed in a future version. Use set_credentials instead.", DeprecationWarning, stacklevel=2)
-
-        service_map = {
-            "deepl": DeepLService,
-            "gemini": GeminiService,
-            "openai": OpenAIService,
-        }
-
-        assert api_type in service_map, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini' and 'openai'.")
-
-        service_map[api_type]._set_api_key(api_key)
-
 ##-------------------start-of-set_credentials()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
-    def set_credentials(api_type:typing.Literal["deepl", "gemini", "openai", "google translate", "anthropic"], credentials:str) -> None:
+    def set_credentials(api_type:typing.Literal["deepl", "gemini", "openai", "google translate", "anthropic", "azure"], credentials:str) -> None:
 
         """
 
         Sets the credentials for the specified API type.
 
         Parameters:
         api_type (literal["deepl", "gemini", "openai", "google translate", "anthropic"]) : The API type to set the credentials for.
@@ -88,66 +59,27 @@
         """
 
         service_map = {
             "deepl": DeepLService._set_api_key,
             "gemini": GeminiService._set_api_key,
             "openai": OpenAIService._set_api_key,
             "google translate": GoogleTLService._set_credentials,
-            "anthropic": AnthropicService._set_api_key
+            "anthropic": AnthropicService._set_api_key,
+            "azure": AzureService._set_api_key
 
         }
 
-        assert api_type in service_map, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini', 'openai', 'google translate', and 'anthropic'.")
+        assert api_type in service_map, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini', 'openai', 'google translate', 'anthropic' and 'azure'.")
 
         service_map[api_type](credentials)
 
-##-------------------start-of-test_api_key_validity()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-            
-    @staticmethod
-    def test_api_key_validity(api_type:typing.Literal["deepl", "gemini", "openai"]) -> typing.Tuple[bool, typing.Optional[Exception]]:
-        
-        """
-
-        Tests the validity of the API key for the specified API type.
-        
-        Deprecated: This function is deprecated and will be removed in a future version.
-        Use test_credentials() instead.
-
-        Parameters:
-        api_type (literal["deepl", "gemini", "openai"]) : The API type to test the key for.
-
-        Returns:
-        (bool) : Whether the API key is valid.
-        (Exception) : The exception that was raised, if any. None otherwise.
-
-        """
-
-        warnings.warn("test_api_key_validity is deprecated and will be removed in a future version. Use test_credentials instead.", DeprecationWarning, stacklevel=2)
-        
-        api_services = {
-            "deepl": {"service": DeepLService, "exception": DeepLException},
-            "gemini": {"service": GeminiService, "exception": GoogleAPIError},
-            "openai": {"service": OpenAIService, "exception": OpenAIError}
-        }
-
-        assert api_type in api_services, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini' and 'openai'.")
-
-        _is_valid, _e = api_services[api_type]["service"]._test_api_key_validity()
-
-        if(not _is_valid):
-            ## Done to make sure the exception is due to the specified API type and not the fault of EasyTL
-            assert isinstance(_e, api_services[api_type]["exception"]), _e
-            return False, _e
-
-        return True, None
-    
 ##-------------------start-of-test_credentials()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
-    def test_credentials(api_type:typing.Literal["deepl", "gemini", "openai", "google translate", "anthropic"]) -> typing.Tuple[bool, typing.Optional[Exception]]:
+    def test_credentials(api_type:typing.Literal["deepl", "gemini", "openai", "google translate", "anthropic", "azure"]) -> typing.Tuple[bool, typing.Optional[Exception]]:
 
         """
 
         Tests the validity of the credentials for the specified API type.
 
         Parameters:
         api_type (literal["deepl", "gemini", "openai", "google translate", "anthropic"]) : The API type to test the credentials for.
@@ -159,18 +91,19 @@
         """
 
         api_services = {
             "deepl": {"service": DeepLService, "exception": DeepLException, "test_func": DeepLService._test_api_key_validity},
             "gemini": {"service": GeminiService, "exception": GoogleAPIError, "test_func": GeminiService._test_api_key_validity},
             "openai": {"service": OpenAIService, "exception": OpenAIError, "test_func": OpenAIService._test_api_key_validity},
             "google translate": {"service": GoogleTLService, "exception": GoogleAPIError, "test_func": GoogleTLService._test_credentials},
-            "anthropic": {"service": AnthropicService, "exception": AnthropicError, "test_func": AnthropicService._test_api_key_validity}
+            "anthropic": {"service": AnthropicService, "exception": AnthropicError, "test_func": AnthropicService._test_api_key_validity},
+            "azure": {"service": AzureService, "exception": RequestException, "test_func": AzureService._test_credentials}
         }
 
-        assert api_type in api_services, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini', 'openai', 'google translate', and 'anthropic'.")
+        assert api_type in api_services, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini', 'openai', 'google translate', 'anthropic' and 'azure'.")
 
         _is_valid, _e = api_services[api_type]["test_func"]()
 
         if(not _is_valid):
             ## Done to make sure the exception is due to the specified API type and not the fault of EasyTL
             assert isinstance(_e, api_services[api_type]["exception"]), _e
             return False, _e
@@ -194,16 +127,14 @@
 
         Translates the given text to the target language using Google Translate.
 
         This function assumes that the credentials have already been set.
 
         It is unknown whether Google Translate has backoff retrying implemented. Assume it does not exist.
 
-        Due to how Google Translate's API works, the translation delay and semaphore are not as important as they are for other services. As they process iterables directly.
-
         Google Translate v2 API is poorly documented and type hints are near non-existent. typing.Any return types are used for the raw response type.
 
         Parameters:
         text (string or iterable) : The text to translate.
         target_lang (string) : The target language to translate to.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a Google Translate function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
@@ -271,15 +202,15 @@
     @staticmethod
     async def googletl_translate_async(text:typing.Union[str, typing.Iterable[str]],
                                        target_lang:str = "en",
                                        override_previous_settings:bool = True,
                                        decorator:typing.Callable | None = None,
                                        logging_directory:str | None = None,
                                        response_type:typing.Literal["text", "raw"] | None = "text",
-                                       semaphore:int | None = None,
+                                       semaphore:int | None = 15,
                                        translation_delay:float | None = None,
                                        format:typing.Literal["text", "html"] = "text",
                                        source_lang:str | None = None) -> typing.Union[typing.List[str], str, typing.List[typing.Any], typing.Any]:
         
         """
 
         Asynchronous version of googletl_translate().
@@ -287,16 +218,14 @@
         Translates the given text to the target language using Google Translate.
         Will generally be faster for iterables. Order is preserved.
 
         This function assumes that the credentials have already been set.
 
         It is unknown whether Google Translate has backoff retrying implemented. Assume it does not exist.
 
-        Due to how Google Translate's API works, the translation delay and semaphore are not as important as they are for other services. As they process iterables directly.
-
         Google Translate v2 API is poorly documented and type hints are near non-existent. typing.Any return types are used for the raw response type.
 
         Parameters:
         text (string or iterable) : The text to translate.
         target_lang (string) : The target language to translate to.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a Google Translate function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
@@ -383,16 +312,14 @@
         
         """
 
         Translates the given text to the target language using DeepL.
 
         This function assumes that the API key has already been set.
 
-        Due to how DeepL's API works, the translation delay and semaphore are not as important as they are for other services. As they process iterables directly.
-
         Parameters:
         text (string or iterable) : The text to translate.
         target_lang (string or Language) : The target language to translate to.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a DeepL translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying. If this parameter is None, DeepL will retry your request 5 times before failing. Otherwise, the given decorator will be used.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
         response_type (literal["text", "raw"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a TextResult object.
@@ -472,15 +399,15 @@
     @staticmethod
     async def deepl_translate_async(text:typing.Union[str, typing.Iterable[str]],
                             target_lang:str | Language = "EN-US",
                             override_previous_settings:bool = True,
                             decorator:typing.Callable | None = None,
                             logging_directory:str | None = None,
                             response_type:typing.Literal["text", "raw"] | None = "text",
-                            semaphore:int | None = None,
+                            semaphore:int | None = 15,
                             translation_delay:float | None = None,
                             source_lang:str | Language | None = None,
                             context:str | None = None,
                             split_sentences:typing.Literal["OFF", "ALL", "NO_NEWLINES"] |  SplitSentences | None = "ALL",
                             preserve_formatting:bool | None = None,
                             formality:typing.Literal["default", "more", "less", "prefer_more", "prefer_less"] | Formality | None = None,
                             glossary:str | GlossaryInfo | None = None,
@@ -491,28 +418,27 @@
                             ignore_tags:str | typing.List[str] | None = None) -> typing.Union[typing.List[str], str, typing.List[TextResult], TextResult]:
         
         """
 
         Asynchronous version of deepl_translate().
         
         Translates the given text to the target language using DeepL.
+
         Will generally be faster for iterables. Order is preserved.
 
         This function assumes that the API key has already been set.
-
-        Due to how DeepL's API works, the translation delay and semaphore are not as important as they are for other services. As they process iterables directly.
         
         Parameters:
         text (string or iterable) : The text to translate.
         target_lang (string or Language) : The target language to translate to.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a DeepL translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying. If this parameter is None, DeepL will retry your request 5 times before failing. Otherwise, the given decorator will be used.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
         response_type (literal["text", "raw"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a TextResult object.
-        semaphore (int) : The number of concurrent requests to make. Default is 30.
+        semaphore (int) : The number of concurrent requests to make. Default is 15.
         translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
         source_lang (string or Language or None) : The source language to translate from.
         context (string or None) : Additional information for the translator to be considered when translating. Not translated itself. This is a DeepL alpha feature and may be removed at any time.
         split_sentences (literal or SplitSentences or None) : How to split sentences.
         preserve_formatting (bool or None) : Whether to preserve formatting.
         formality (literal or Formality or None) : The formality level to use.
         glossary (string or GlossaryInfo or None) : The glossary to use.
@@ -631,15 +557,15 @@
 
         """
 
         assert response_type in ["text", "raw", "json", "raw_json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw', 'json' or 'raw_json'.")
 
         _settings = _return_curated_gemini_settings(locals())
 
-        _validate_easytl_translation_settings(_settings, "gemini")
+        _validate_easytl_llm_translation_settings(_settings, "gemini")
 
         _validate_stop_sequences(stop_sequences)
 
         _validate_text_length(text, model, service="gemini")
 
         response_schema = _validate_response_schema(response_schema)
 
@@ -693,15 +619,15 @@
     @staticmethod
     async def gemini_translate_async(text:typing.Union[str, typing.Iterable[str]],
                                     override_previous_settings:bool = True,
                                     decorator:typing.Callable | None = None,
                                     logging_directory:str | None = None,
                                     response_type:typing.Literal["text", "raw", "json", "raw_json"] | None = "text",
                                     response_schema:str | typing.Mapping[str, typing.Any] | None = None,
-                                    semaphore:int | None = None,
+                                    semaphore:int | None = 5,
                                     translation_delay:float | None = None,
                                     translation_instructions:str | None = None,
                                     model:str="gemini-pro",
                                     temperature:float=0.5,
                                     top_p:float=0.9,
                                     top_k:int=40,
                                     stop_sequences:typing.List[str] | None=None,
@@ -725,15 +651,15 @@
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a Gemini translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
         response_type (literal["text", "raw", "json", "raw_json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, an AsyncGenerateContentResponse object, 'json' returns a json-parseable string. 'raw_json' returns the raw response, an AsyncGenerateContentResponse object, but with the content as a json-parseable string.
         response_schema (string or mapping or None) : The schema to use for the response. If None, no schema is used. This is only used if the response type is 'json' or 'json_raw'. EasyTL only validates the schema to the extend that it is None or a valid json. It does not validate the contents of the json.
-        semaphore (int) : The number of concurrent requests to make. Default is 15 for 1.0 and 2 for 1.5 gemini models. For Gemini, it is recommend to use translation_delay along with the semaphore to prevent rate limiting.
+        semaphore (int) : The number of concurrent requests to make. Default is 5 for 1.0 and 2 for 1.5 gemini models. For Gemini, it is recommend to use translation_delay along with the semaphore to prevent rate limiting.
         translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
         translation_instructions (string or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
         model (string) : The model to use. (E.g. 'gemini-pro' or 'gemini-pro-1.5-latest')
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
         top_k (int) : The top k tokens to consider. Generally, alter this or temperature or top_p, not all three.
         stop_sequences (list or None) : String sequences that will cause the model to stop translating if encountered, generally useless.
@@ -744,15 +670,15 @@
 
         """
 
         assert response_type in ["text", "raw", "json", "raw_json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw', 'json' or 'raw_json'.")
 
         _settings = _return_curated_gemini_settings(locals())
 
-        _validate_easytl_translation_settings(_settings, "gemini")
+        _validate_easytl_llm_translation_settings(_settings, "gemini")
 
         _validate_stop_sequences(stop_sequences)
 
         _validate_text_length(text, model, service="gemini")
 
         response_schema = _validate_response_schema(response_schema)
 
@@ -847,15 +773,15 @@
 
         """
 
         assert response_type in ["text", "raw", "json", "raw_json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw', 'json' or 'raw_json'.")
 
         _settings = _return_curated_openai_settings(locals())
 
-        _validate_easytl_translation_settings(_settings, "openai")
+        _validate_easytl_llm_translation_settings(_settings, "openai")
 
         _validate_stop_sequences(stop)
 
         _validate_text_length(text, model, service="openai")
 
         ## Should be done after validating the settings to reduce cost to the user
         EasyTL.test_credentials("openai")
@@ -909,15 +835,15 @@
 
     @staticmethod
     async def openai_translate_async(text:typing.Union[str, typing.Iterable[str], ModelTranslationMessage, typing.Iterable[ModelTranslationMessage]],
                                     override_previous_settings:bool = True,
                                     decorator:typing.Callable | None = None,
                                     logging_directory:str | None = None,
                                     response_type:typing.Literal["text", "raw", "json", "raw_json"] | None = "text",
-                                    semaphore:int | None = None,
+                                    semaphore:int | None = 5,
                                     translation_delay:float | None = None,
                                     translation_instructions:str | SystemTranslationMessage | None = None,
                                     model:str="gpt-4",
                                     temperature:float=0.3,
                                     top_p:float=1.0,
                                     stop:typing.List[str] | None=None,
                                     max_tokens:int | None=None,
@@ -926,14 +852,16 @@
                                     ) -> typing.Union[typing.List[str], str, typing.List[ChatCompletion], ChatCompletion]:
         
         """
 
         Asynchronous version of openai_translate().
         Will generally be faster for iterables. Order is preserved.
 
+        Translates the given text using OpenAI.
+
         This function assumes that the API key has already been set.
 
         Translation instructions default to translating the text to English. To change this, specify the instructions.
 
         This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
 
         Parameters:
@@ -958,15 +886,15 @@
         
         """
 
         assert response_type in ["text", "raw", "json", "raw_json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw', 'json' or 'raw_json'.")
 
         _settings = _return_curated_openai_settings(locals())
 
-        _validate_easytl_translation_settings(_settings, "openai")
+        _validate_easytl_llm_translation_settings(_settings, "openai")
 
         _validate_stop_sequences(stop)
 
         _validate_text_length(text, model, service="openai")
 
         ## Should be done after validating the settings to reduce cost to the user
         EasyTL.test_credentials("openai")
@@ -1072,15 +1000,15 @@
 
         """
 
         assert response_type in ["text", "raw", "json", "raw_json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw', 'json' or 'raw_json'.")
 
         _settings = _return_curated_anthropic_settings(locals())
 
-        _validate_easytl_translation_settings(_settings, "anthropic")
+        _validate_easytl_llm_translation_settings(_settings, "anthropic")
 
         _validate_stop_sequences(stop_sequences)
 
         _validate_text_length(text, model, service="anthropic")
 
         response_schema = _validate_response_schema(response_schema)
 
@@ -1148,32 +1076,33 @@
     @staticmethod
     async def anthropic_translate_async(text:typing.Union[str, typing.Iterable[str], ModelTranslationMessage, typing.Iterable[ModelTranslationMessage]],
                                         override_previous_settings:bool = True,
                                         decorator:typing.Callable | None = None,
                                         logging_directory:str | None = None,
                                         response_type:typing.Literal["text", "raw", "json", "raw_json"] | None = "text",
                                         response_schema:str | typing.Mapping[str, typing.Any] | None = None,
-                                        semaphore:int | None = None,
+                                        semaphore:int | None = 5,
                                         translation_delay:float | None = None,
                                         translation_instructions:str | None = None,
                                         model:str="claude-3-haiku-20240307",
                                         temperature:float | NotGiven = NOT_GIVEN,
                                         top_p:float | NotGiven = NOT_GIVEN,
                                         top_k:int | NotGiven = NOT_GIVEN,
                                         stop_sequences:typing.List[str] | NotGiven = NOT_GIVEN,
                                         max_output_tokens:int | NotGiven = NOT_GIVEN) -> typing.Union[typing.List[str], str, 
                                                                                                     AnthropicMessage, typing.List[AnthropicMessage],
                                                                                                     AnthropicToolsBetaMessage, typing.List[AnthropicToolsBetaMessage]]:
         
         """
 
         Asynchronous version of anthropic_translate().
-
         Will generally be faster for iterables. Order is preserved.
 
+        Translates the given text using Anthropic.
+
         This function assumes that the API key has already been set.
 
         Translation instructions default to translating the text to English. To change this, specify the instructions.
 
         This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
 
         Due to how Anthropic's API works, NOT_GIVEN is treated differently than None. If a parameter is set to NOT_GIVEN, it is not passed to the API.
@@ -1202,15 +1131,15 @@
 
         """
 
         assert response_type in ["text", "raw", "json", "raw_json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw', 'json' or 'raw_json'.")
 
         _settings = _return_curated_anthropic_settings(locals())
 
-        _validate_easytl_translation_settings(_settings, "anthropic")
+        _validate_easytl_llm_translation_settings(_settings, "anthropic")
 
         _validate_stop_sequences(stop_sequences)
 
         _validate_text_length(text, model, service="anthropic")
 
         response_schema = _validate_response_schema(response_schema)
 
@@ -1263,20 +1192,207 @@
         
         elif(isinstance(_results[0], AnthropicMessage)):
             translations = [result.content[0].text for result in _results if isinstance(result.content[0], AnthropicTextBlock)]
                 
         result = translations if isinstance(text, typing.Iterable) and not isinstance(text, str) else translations[0]
 
         return result # type: ignore
+    
+##-------------------start-of-azure_translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+    @staticmethod
+    def azure_translate(text: typing.Union[str, typing.Iterable[str]],
+                        target_lang:str = 'en',
+                        override_previous_settings:bool = True,
+                        decorator:typing.Callable | None = None,
+                        logging_directory:str | None = None,
+                        response_type:typing.Literal["text", "json"] | None = "text",
+                        translation_delay:float | None = None,
+                        api_version:str = '3.0',
+                        azure_region:str = "global",
+                        azure_endpoint:str = "https://api.cognitive.microsofttranslator.com/",
+                        source_lang:str | None = None) -> typing.Union[typing.List[str], str]:
         
+        """
+
+        Translates the given text to the target language using Azure.
+
+        This function assumes that the API key has already been set.
+
+        It is unknown whether Azure Translate has backoff retrying implemented. Assume it does not  exist
+
+        Default api_version, azure_region, and azure_endpoint values should be fine for most users.
+        
+        Parameters:
+        text (string or iterable) : The text to translate.
+        target_lang (string) : The target language for translation. Default is 'en'. These are ISO 639-1 language codes
+        override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to an Azure translation function.
+        decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying. 
+        logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
+        response_type (literal["text", "json"]) : The type of response to return. 'text' returns the translated text, 'json' returns the original response in json format.
+        translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
+        api_version (string) : The version of the Azure Translator API. Default is '3.0'.
+        azure_region (string) : The Azure region to use for translation. Default is 'global'.
+        azure_endpoint (string) : The Azure Translator API endpoint. Default is 'https://api.cognitive.microsofttranslator.com/'.
+        source_lang (string or None) : The source language of the text. If None, the service will attempt to detect the language.
+
+        Returns:
+        result (string or list - string) : The translation result. A list of strings if the input was an iterable, a string otherwise.
+
+        """
+
+        assert response_type in ["text", "json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text' or 'json'.")
+
+        EasyTL.test_credentials("azure")
+
+        if(override_previous_settings == True):
+            AzureService._set_attributes(target_language=target_lang,
+                                        api_version=api_version,
+                                        azure_region=azure_region,
+                                        azure_endpoint=azure_endpoint,
+                                        source_language=source_lang,
+                                        decorator=decorator,
+                                        log_directory=logging_directory,
+                                        semaphore=None,
+                                        rate_limit_delay=translation_delay)
+            
+        ## This section may seem overly complex, but it is necessary to apply the decorator outside of the function call to avoid infinite recursion.
+        ## Attempting to dynamically apply the decorator within the function leads to unexpected behavior, where this function's arguments are passed to the function instead of the intended translation function.
+
+        def translate(text):
+            return AzureService._translate_text(text)
+        
+        if(decorator is not None):
+            translate = AzureService._decorator_to_use(AzureService._translate_text) # type: ignore
+
+        else:
+            translate = AzureService._translate_text
+
+        if(isinstance(text, str)):
+
+            result = translate(text)[0]
+
+            assert not isinstance(result, list), EasyTLException("Malformed response received. Please try again.")
+
+            result = result if response_type == "json" else result['translations'][0]['text']
+        
+        elif(_is_iterable_of_strings(text)):
+
+            _results = [translate(_t) for _t in text]
+
+            assert isinstance(_results, list), EasyTLException("Malformed response received. Please try again.")
+
+            result = _results if response_type == "json" else [result[0]['translations'][0]['text'] for result in _results]
+
+        else:
+            raise InvalidTextInputException("text must be a string or an iterable of strings.")
+
+        return result # type: ignore
+
+##-------------------start-of-azure_translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+    @staticmethod
+    async def azure_translate_async(text: typing.Union[str, typing.Iterable[str]],
+                                    target_lang:str = 'en',
+                                    override_previous_settings:bool = True,
+                                    decorator:typing.Callable | None = None,
+                                    logging_directory:str | None = None,
+                                    response_type:typing.Literal["text", "json"] | None = "text",
+                                    semaphore:int | None = 15,
+                                    translation_delay:float | None = None,
+                                    api_version:str = '3.0',
+                                    azure_region:str = "global",
+                                    azure_endpoint:str = "https://api.cognitive.microsofttranslator.com/",
+                                    source_lang:str | None = None) -> typing.Union[typing.List[str], str]:
+        """
+
+        Asynchronous version of azure_translate().
+        Will generally be faster for iterables. Order is preserved.
+
+        Translates the given text to the target language using Azure.
+
+        This function assumes that the API key has already been set.
+
+        It is unknown whether Azure Translate has backoff retrying implemented. Assume it does not  exist
+
+        Default api_version, azure_region, and azure_endpoint values should be fine for most users.
+
+        Parameters:
+        text (string or iterable) : The text to translate.
+        target_lang (string) : The target language for translation. Default is 'en'. These are ISO 639-1 language codes
+        override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to an Azure translation function.
+        decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
+        logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
+        response_type (literal["text", "json"]) : The type of response to return. 'text' returns the translated text, 'json' returns the original response in json format.
+        semaphore (int) : The number of concurrent requests to make. Default is 15.
+        translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
+        api_version (string) : The version of the Azure Translator API. Default is '3.0'.
+        azure_region (string) : The Azure region to use for translation. Default is 'global'.
+        azure_endpoint (string) : The Azure Translator API endpoint. Default is 'https://api.cognitive.microsofttranslator.com/'.
+        source_lang (string or None) : The source language of the text. If None, the service will attempt to detect the language.
+
+        Returns:
+        result (string or list - string) : The translation result. A list of strings if the input was an iterable, a string otherwise.
+        
+        """
+
+        assert response_type in ["text", "json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text' or 'json'.")
+
+        EasyTL.test_credentials("azure")
+
+        if(override_previous_settings == True):
+            AzureService._set_attributes(target_language=target_lang,
+                                        api_version=api_version,
+                                        azure_region=azure_region,
+                                        azure_endpoint=azure_endpoint,
+                                        source_language=source_lang,
+                                        decorator=decorator,
+                                        log_directory=logging_directory,
+                                        semaphore=semaphore,
+                                        rate_limit_delay=translation_delay)
+            
+        ## This section may seem overly complex, but it is necessary to apply the decorator outside of the function call to avoid infinite recursion.
+        ## Attempting to dynamically apply the decorator within the function leads to unexpected behavior, where this function's arguments are passed to the function instead of the intended translation function.
+
+        async def translate(text):
+            return await AzureService._translate_text_async(text)
+        
+        if(decorator is not None):
+            translate = AzureService._decorator_to_use(AzureService._translate_text_async) # type: ignore
+
+        else:
+            translate = AzureService._translate_text_async
+
+        if(isinstance(text, str)):
+
+            result = (await translate(text))[0]
+
+            assert not isinstance(result, list), EasyTLException("Malformed response received. Please try again.")
+
+            result = result if response_type == "json" else result['translations'][0]['text']
+
+        elif(_is_iterable_of_strings(text)):
+
+            _tasks = [translate(_t) for _t in text]
+            _results = await asyncio.gather(*_tasks)
+
+            assert isinstance(_results, list), EasyTLException("Malformed response received. Please try again.")
+
+            result = _results if response_type == "json" else [result[0]['translations'][0]['text'] for result in _results]
+
+        else:
+            raise InvalidTextInputException("text must be a string or an iterable of strings.")
+        
+        return result # type: ignore
+
 ##-------------------start-of-translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
     def translate(text:str | typing.Iterable[str],
-                  service:typing.Optional[typing.Literal["deepl", "openai", "gemini", "google translate", "anthropic"]] = "deepl",
+                  service:typing.Optional[typing.Literal["deepl", "openai", "gemini", "google translate", "anthropic", "azure"]] = "deepl",
                   **kwargs) -> typing.Union[typing.List[str], str, 
                                             typing.List[TextResult], TextResult, 
                                             typing.List[ChatCompletion], ChatCompletion,
                                             typing.List[GenerateContentResponse], GenerateContentResponse, 
                                             typing.List[typing.Any], typing.Any,
                                             typing.List[AnthropicMessage], AnthropicMessage]:
         
@@ -1287,33 +1403,35 @@
         Please see the documentation for the specific translation function for the service you want to use.
 
         DeepL: deepl_translate() 
         OpenAI: openai_translate() 
         Gemini: gemini_translate() 
         Google Translate: googletl_translate() 
         Anthropic: anthropic_translate()
+        Azure: azure_translate()
 
         All functions can return a list of strings or a string, depending on the input. The response type can be specified to return the raw response instead:
         DeepL: TextResult
         OpenAI: ChatCompletion
         Gemini: GenerateContentResponse
         Google Translate: any
         Anthropic: AnthropicMessage or AnthropicToolsBetaMessage
+        Azure: str
 
         Parameters:
         service (string) : The service to use for translation.
         text (string) : The text to translate.
         **kwargs : The keyword arguments to pass to the translation function.
 
         Returns:
         result (string or list - string or TextResult or list - TextResult or GenerateContentResponse or list - GenerateContentResponse or ChatCompletion or list - ChatCompletion or any or list - any or AnthropicMessage or list - AnthropicMessage or AnthropicToolsBetaMessage or list - AnthropicToolsBetaMessage) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of TextResult objects if the response type is 'raw' and input was an iterable, a TextResult object otherwise. A list of GenerateContentResponse objects if the response type is 'raw' and input was an iterable, a GenerateContentResponse object otherwise. A list of ChatCompletion objects if the response type is 'raw' and input was an iterable, a ChatCompletion object otherwise. A list of any objects if the response type is 'raw' and input was an iterable, an any object otherwise. A list of AnthropicMessage objects if the response type is 'raw' and input was an iterable, an AnthropicMessage object otherwise. A list of AnthropicToolsBetaMessage objects if the response type is 'raw' and input was an iterable, an AnthropicToolsBetaMessage object otherwise.
 
         """
 
-        assert service in ["deepl", "openai", "gemini", "google translate", "anthropic"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini', 'google translate' or 'anthropic'.")
+        assert service in ["deepl", "openai", "gemini", "google translate", "anthropic", "azure"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini', 'google translate', 'anthropic' or 'azure'.")
 
         if(service == "deepl"):
             return EasyTL.deepl_translate(text, **kwargs)
 
         elif(service == "openai"):
             return EasyTL.openai_translate(text, **kwargs)
 
@@ -1322,19 +1440,22 @@
         
         elif(service == "google translate"):
             return EasyTL.googletl_translate(text, **kwargs)
         
         elif(service == "anthropic"):
             return EasyTL.anthropic_translate(text, **kwargs)
         
+        elif(service == "azure"):
+            return EasyTL.azure_translate(text, **kwargs)
+        
 ##-------------------start-of-translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
     async def translate_async(text:str | typing.Iterable[str],
-                              service:typing.Optional[typing.Literal["deepl", "openai", "gemini", "google translate", "anthropic"]] = "deepl",
+                              service:typing.Optional[typing.Literal["deepl", "openai", "gemini", "google translate", "anthropic", "azure"]] = "deepl",
                               **kwargs) -> typing.Union[typing.List[str], str, 
                                                         typing.List[TextResult], TextResult,  
                                                         typing.List[ChatCompletion], ChatCompletion,
                                                         typing.List[AsyncGenerateContentResponse], AsyncGenerateContentResponse,
                                                         typing.List[typing.Any], typing.Any,
                                                         typing.List[AnthropicMessage], AnthropicMessage]:
 
@@ -1350,33 +1471,35 @@
         Please see the documentation for the specific translation function for the service you want to use.
 
         DeepL: deepl_translate_async()
         OpenAI: openai_translate_async() 
         Gemini: gemini_translate_async() 
         Google Translate: googletl_translate_async()
         Anthropic: anthropic_translate_async()
+        Azure: azure_translate_async()
 
         All functions can return a list of strings or a string, depending on the input. The response type can be specified to return the raw response instead:
         DeepL: TextResult
         OpenAI: ChatCompletion
         Gemini: AsyncGenerateContentResponse
         Google Translate: any
         Anthropic: AnthropicMessage or AnthropicToolsBetaMessage
+        Azure: str
 
         Parameters:
         service (string) : The service to use for translation.
         text (string) : The text to translate.
         **kwargs : The keyword arguments to pass to the translation function.
 
         Returns:
         result (string or list - string or TextResult or list - TextResult or AsyncGenerateContentResponse or list - AsyncGenerateContentResponse or ChatCompletion or list - ChatCompletion or any or list - any or AnthropicMessage or list - AnthropicMessage or AnthropicToolsBetaMessage or list - AnthropicToolsBetaMessage) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of TextResult objects if the response type is 'raw' and input was an iterable, a TextResult object otherwise. A list of AsyncGenerateContentResponse objects if the response type is 'raw' and input was an iterable, an AsyncGenerateContentResponse object otherwise. A list of ChatCompletion objects if the response type is 'raw' and input was an iterable, a ChatCompletion object otherwise. A list of any objects if the response type is 'raw' and input was an iterable, an any object otherwise. A list of AnthropicMessage objects if the response type is 'raw' and input was an iterable, an AnthropicMessage object otherwise. A list of AnthropicToolsBetaMessage objects if the response type is 'raw' and input was an iterable, an AnthropicToolsBetaMessage object otherwise.
 
         """
 
-        assert service in ["deepl", "openai", "gemini", "google translate", "anthropic"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini', 'google translate' or 'anthropic'.")
+        assert service in ["deepl", "openai", "gemini", "google translate", "anthropic", "azure"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini', 'google translate', 'anthropic' or 'azure'.")
 
         if(service == "deepl"):
             return await EasyTL.deepl_translate_async(text, **kwargs)
 
         elif(service == "openai"):
             return await EasyTL.openai_translate_async(text, **kwargs)
 
@@ -1384,20 +1507,23 @@
             return await EasyTL.gemini_translate_async(text, **kwargs)
         
         elif(service == "google translate"):
             return await EasyTL.googletl_translate_async(text, **kwargs)
         
         elif(service == "anthropic"):
             return await EasyTL.anthropic_translate_async(text, **kwargs)
+        
+        elif(service == "azure"):
+            return await EasyTL.azure_translate_async(text, **kwargs)
 
 ##-------------------start-of-calculate_cost()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
     def calculate_cost(text:str | typing.Iterable[str],
-                       service:typing.Optional[typing.Literal["deepl", "openai", "gemini", "google translate", "anthropic"]] = "deepl",
+                       service:typing.Optional[typing.Literal["deepl", "openai", "gemini", "google translate", "anthropic", "azure"]] = "deepl",
                        model:typing.Optional[str] = None,
                        translation_instructions:typing.Optional[str] = None
                        ) -> typing.Tuple[int, float, str]:
         
         """
 
         Calculates the cost of translating the given text using the specified service.
@@ -1420,23 +1546,26 @@
         Returns:
         num_tokens (int) : The number of tokens/characters in the text.
         cost (float) : The cost of translating the text.
         model (string) : The model used for translation.
 
         """
 
-        assert service in ["deepl", "openai", "gemini", "google translate", "anthropic"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini', 'google translate' or 'anthropic'.")
+        assert service in ["deepl", "openai", "gemini", "google translate", "anthropic", "azure"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini', 'google translate' or 'anthropic'.")
 
         if(service == "deepl"):
             return DeepLService._calculate_cost(text)
         
         elif(service == "openai"):
             return OpenAIService._calculate_cost(text, translation_instructions, model)
 
         elif(service == "gemini"):
             return GeminiService._calculate_cost(text, translation_instructions, model)
         
         elif(service == "google translate"):
             return GoogleTLService._calculate_cost(text)
         
         elif(service == "anthropic"):
-            return AnthropicService._calculate_cost(text, translation_instructions, model)
+            return AnthropicService._calculate_cost(text, translation_instructions, model)
+        
+        elif(service == "azure"):
+            return AzureService._calculate_cost(text)
```

### Comparing `easytl-0.4.0a3/src/easytl/exceptions.py` & `easytl-0.4.0b0/src/easytl/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-## Copyright Bikatr7 (https://github.com/Bikatr7)
-## Use of this source code is governed by a GNU Lesser General Public License v2.1
+## Copyright (C) 2024 Kaden Bilyeu (Bikatr7) (https://github.com/Bikatr7), Alejandro Mata (https://github.com/alemalvarez)
+## Use of this source code is governed by an GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 ## deepL generic exception
 from deepl.exceptions import DeepLException
 
 ## google generic exception
 from google.api_core.exceptions import GoogleAPIError
 
 ## openai generic exception
 from openai import OpenAIError
 
 ## anthropic generic exception
 from anthropic import AnthropicError
 
+## azure generic exception
+from requests import RequestException
+
 ## service specific exceptions
 from openai import APIError as OpenAIAPIError, ConflictError as OpenAIConflictError, NotFoundError as OpenAINotFoundError, APIStatusError as OpenAIAPIStatusError, RateLimitError as OpenAIRateLimitError, APITimeoutError as OpenAIAPITimeoutError, BadRequestError as OpenAIBadRequestError, APIConnectionError as OpenAIAPIConnectionError, AuthenticationError as OpenAIAuthenticationError, InternalServerError as OpenAIInternalServerError, PermissionDeniedError as OpenAIPermissionDeniedError, UnprocessableEntityError as OpenAIUnprocessableEntityError, APIResponseValidationError as OpenAIAPIResponseValidationError
 from deepl.exceptions import AuthorizationException as DeepLAuthorizationException, QuotaExceededException as DeepLQuotaExceededException, ConnectionException as DeepLConnectionException, TooManyRequestsException as DeepLTooManyRequestsException, DocumentNotReadyException as DeepLDocumentNotReadyException, GlossaryNotFoundException as DeepLGlossaryNotFoundException, DocumentTranslationException as DeepLDocumentTranslationException
 from google.auth.exceptions import GoogleAuthError, DefaultCredentialsError as GoogleDefaultCredentialsError
 from anthropic import APIError as AnthropicAPIError, ConflictError as AnthropicConflictError, NotFoundError as AnthropicNotFoundError, APIStatusError as AnthropicAPIStatusError, RateLimitError as AnthropicRateLimitError, APITimeoutError as AnthropicAPITimeoutError, BadRequestError as AnthropicBadRequestError, APIConnectionError as AnthropicAPIConnectionError, AuthenticationError as AnthropicAuthenticationError, InternalServerError as AnthropicInternalServerError, PermissionDeniedError as AnthropicPermissionDeniedError, UnprocessableEntityError as AnthropicUnprocessableEntityError, APIResponseValidationError as AnthropicAPIResponseValidationError
 
 class EasyTLException(Exception):
@@ -131,14 +134,16 @@
         Parameters:
         message (string) : The message to display when the exception is raised.
 
         """
 
         self.message = message
 
+##-------------------start-of-TooManyInputTokensException--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
 class TooManyInputTokensException(EasyTLException):
 
     """
 
     TooManyInputTokensException is an exception that is raised when the input text contains too many tokens to be accepted by the API
 
     """
```

### Comparing `easytl-0.4.0a3/src/easytl/gemini_service.py` & `easytl-0.4.0b0/src/easytl/services/gemini_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-## Copyright Bikatr7 (https://github.com/Bikatr7)
-## Use of this source code is governed by a GNU Lesser General Public License v2.1
+## Copyright (C) 2024 Kaden Bilyeu (Bikatr7) (https://github.com/Bikatr7), Alejandro Mata (https://github.com/alemalvarez)
+## Use of this source code is governed by an GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 ## built-in libraries
 import typing
 import asyncio
 
 import google.generativeai as genai
 
 ## custom modules
-from .util import _estimate_cost, _convert_iterable_to_str, _is_iterable_of_strings, VALID_JSON_GEMINI_MODELS
-from .util import VALID_JSON_GEMINI_MODELS as VALID_SYSTEM_MESSAGE_MODELS
-from .decorators import _async_logging_decorator, _sync_logging_decorator
+from ..util.util import _estimate_cost, _convert_iterable_to_str, _is_iterable_of_strings
+from ..util.constants import VALID_JSON_GEMINI_MODELS as VALID_SYSTEM_MESSAGE_MODELS, VALID_JSON_GEMINI_MODELS
 
-from .classes import GenerationConfig, GenerateContentResponse, AsyncGenerateContentResponse
-from .exceptions import EasyTLException, InvalidTextInputException
+from ..decorators import _async_logging_decorator, _sync_logging_decorator
+from ..classes import GenerationConfig, GenerateContentResponse, AsyncGenerateContentResponse
+from ..exceptions import EasyTLException, InvalidTextInputException
 
 class GeminiService:
 
     _default_translation_instructions:str = "Please translate the following text into English."
     _default_model:str = "gemini-pro"
 
     _system_message = _default_translation_instructions
@@ -31,15 +31,15 @@
     _stream:bool = False
     _stop_sequences:typing.List[str] | None = None
     _max_output_tokens:int | None = None
 
     _client:genai.GenerativeModel
     _generation_config:GenerationConfig
 
-    _semaphore_value:int = 15
+    _semaphore_value:int = 5
     _semaphore:asyncio.Semaphore = asyncio.Semaphore(_semaphore_value)
 
     _rate_limit_delay:float | None = None
 
     _decorator_to_use:typing.Union[typing.Callable, None] = None
 
     _log_directory:str | None = None
@@ -137,15 +137,15 @@
         ## rate limits for 1.0B models are 15 requests per second
         semaphore_values = {"gemini-1.5-pro": 2,
                             "gemini-1.5-flash": 2,
                             "gemini-1.5-pro-latest": 2,
                             "gemini-1.5-flash-latest": 2,
                             }
         
-        GeminiService._semaphore_value = semaphore or semaphore_values.get(GeminiService._model, 15)
+        GeminiService._semaphore_value = semaphore or semaphore_values.get(GeminiService._model, 5)
         GeminiService._semaphore = asyncio.Semaphore(GeminiService._semaphore_value)
 
         if(GeminiService._json_mode and GeminiService._model in VALID_JSON_GEMINI_MODELS and response_schema is not None):
             GeminiService._default_translation_instructions = "Please translate the following text into English. Make sure to return the translated text in JSON format. The JSON should be in the format specified in the response schema."
 
         elif(GeminiService._json_mode and GeminiService._model in VALID_JSON_GEMINI_MODELS):
             GeminiService._default_translation_instructions = "Please translate the following text into English. Make sure to return the translated text in JSON format."
```

### Comparing `easytl-0.4.0a3/src/easytl/googletl_service.py` & `easytl-0.4.0b0/src/easytl/services/googletl_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## Copyright Bikatr7 (https://github.com/Bikatr7)
+## Copyright (C) 2024 Kaden Bilyeu (Bikatr7) (https://github.com/Bikatr7), Alejandro Mata (https://github.com/alemalvarez)
 ## Use of this source code is governed by an GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 ## built-in libraries
 import asyncio
 import typing
 import time
@@ -11,22 +11,20 @@
 from google.cloud import translate_v2 as translate
 from google.cloud.translate_v2 import Client
 
 from google.oauth2 import service_account
 from google.oauth2.service_account import Credentials
 
 ## custom modules
-from .version import VERSION
-from .util import _convert_iterable_to_str
-from .decorators import _sync_logging_decorator, _async_logging_decorator
+from ..version import VERSION
+from ..util.util import _convert_iterable_to_str
+from ..decorators import _sync_logging_decorator, _async_logging_decorator
 
 class GoogleTLService:
 
-    
-    
     _translator:Client
     _credentials:Credentials
 
     ## ISO 639-1 language codes
     _target_lang:str = 'en'
     _source_lang:str | None = None
```

### Comparing `easytl-0.4.0a3/src/easytl/openai_service.py` & `easytl-0.4.0b0/src/easytl/services/openai_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-## Copyright Bikatr7 (https://github.com/Bikatr7)
-## Use of this source code is governed by a GNU Lesser General Public License v2.1
+## Copyright (C) 2024 Kaden Bilyeu (Bikatr7) (https://github.com/Bikatr7), Alejandro Mata (https://github.com/alemalvarez)
+## Use of this source code is governed by an GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 ## built-in libraries
 import typing
 import asyncio
 
 ## third-party libraries
 from openai import AsyncOpenAI, OpenAI
 
 ## custom modules
-from .classes import SystemTranslationMessage, ModelTranslationMessage, ChatCompletion
-from .util import _convert_iterable_to_str, _estimate_cost, _is_iterable_of_strings, VALID_JSON_OPENAI_MODELS
-from .decorators import _async_logging_decorator, _sync_logging_decorator
-from .exceptions import EasyTLException
+from ..classes import SystemTranslationMessage, ModelTranslationMessage, ChatCompletion
+from ..decorators import _async_logging_decorator, _sync_logging_decorator
+from ..exceptions import EasyTLException
+
+from ..util.util import _convert_iterable_to_str, _estimate_cost, _is_iterable_of_strings
+from ..util.constants import VALID_JSON_OPENAI_MODELS
+
 
 class OpenAIService:
 
     _default_model:str = "gpt-4"
     _default_translation_instructions:SystemTranslationMessage = SystemTranslationMessage("Please translate the following text into English.")
 
     _system_message:typing.Optional[typing.Union[SystemTranslationMessage, str]] = _default_translation_instructions
```

### Comparing `easytl-0.4.0a3/src/easytl.egg-info/PKG-INFO` & `easytl-0.4.0b0/src/easytl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.4.0a3
-Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
-Author-email: Bikatr7 <Bikatr7@proton.me>
+Version: 0.4.0b0
+Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini, Google Translate and More.
+Author-email: "Kaden Bilyeu (Bikatr7)" <Bikatr7@proton.me>, Alejandro Mata <alemalvarez@icloud.com>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,15 @@
 Requires-Dist: google-generativeai==0.5.4
 Requires-Dist: deepl==1.16.1
 Requires-Dist: openai==1.29.0
 Requires-Dist: backoff==2.2.1
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: google-cloud-translate==3.15.3
 Requires-Dist: anthropic==0.26.0
+Requires-Dist: requests>=2.31.0
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Table of Contents**
 
 - [Quick Start](#quick-start)
 - [Installation](#installation)
 - [Features](#features)
```

### Comparing `easytl-0.4.0a3/src/easytl.egg-info/SOURCES.txt` & `easytl-0.4.0b0/src/easytl.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 .gitignore
 LICENSE.md
 README.md
 SECURITY.md
 pyproject.toml
+requirements.txt
 .github/workflows/workflow.yml
 src/easytl/__init__.py
-src/easytl/anthropic_service.py
 src/easytl/classes.py
 src/easytl/decorators.py
-src/easytl/deepl_service.py
 src/easytl/easytl.py
 src/easytl/exceptions.py
-src/easytl/gemini_service.py
-src/easytl/googletl_service.py
-src/easytl/openai_service.py
-src/easytl/util.py
 src/easytl/version.py
 src/easytl.egg-info/PKG-INFO
 src/easytl.egg-info/SOURCES.txt
 src/easytl.egg-info/dependency_links.txt
 src/easytl.egg-info/requires.txt
 src/easytl.egg-info/top_level.txt
+src/easytl/services/__init__.py
+src/easytl/services/anthropic_service.py
+src/easytl/services/azure_service.py
+src/easytl/services/deepl_service.py
+src/easytl/services/gemini_service.py
+src/easytl/services/googletl_service.py
+src/easytl/services/openai_service.py
+src/easytl/util/__init__.py
+src/easytl/util/constants.py
+src/easytl/util/llm_util.py
+src/easytl/util/util.py
 tests/issue_template.py
 tests/passing.py
 tests/simple_test.py
```

### Comparing `easytl-0.4.0a3/tests/issue_template.py` & `easytl-0.4.0b0/tests/issue_template.py`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a3/tests/passing.py` & `easytl-0.4.0b0/tests/passing.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,23 +15,27 @@
     try:
         with open(filename, 'r') as file:
             return file.read().strip()
         
     except:
         pass
 
+##-------------------start-of-setup_preconditions()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
 def setup_preconditions():
 
     gemini_time_delay = 30
 
     deepl_api_key = os.environ.get('DEEPL_API_KEY')
     gemini_api_key = os.environ.get('GEMINI_API_KEY')
     openai_api_key = os.environ.get('OPENAI_API_KEY')
     anthropic_api_key = os.environ.get('ANTHROPIC_API_KEY')
     json_value = os.environ.get('GOOGLE_TRANSLATE_SERVICE_KEY_VALUE')
+    azure_api_key = os.environ.get('AZURE_API_KEY')
+    azure_region = os.environ.get('AZURE_REGION')
 
     if(json_value is not None):
 
         with open("json_value.txt", "w") as file:
             file.write(json_value)
 
         google_tl_key_path = "json_value.txt"
@@ -42,32 +46,39 @@
         deepl_api_key = read_api_key("tests/deepl.txt")
     if(gemini_api_key is None):
         gemini_api_key = read_api_key("tests/gemini.txt")
     if(openai_api_key is None):
         openai_api_key = read_api_key("tests/openai.txt")
     if(anthropic_api_key is None):
         anthropic_api_key = read_api_key("tests/anthropic.txt")
+    if(azure_api_key is None):
+        azure_api_key = read_api_key("tests/azure.txt")
+    if(azure_region is None):
+        azure_region = read_api_key("tests/azure_region.txt")
 
     if(json_value is None):
         google_tl_key_path = "tests/google_translate_key.json"
         
         logging_directory = "tests/"
         gemini_time_delay = 5
 
     assert deepl_api_key is not None, "DEEPL_API_KEY environment variable must be set"
     assert gemini_api_key is not None, "GEMINI_API_KEY environment variable must be set"
     assert openai_api_key is not None, "OPENAI_API_KEY environment variable must be set"
     assert anthropic_api_key is not None, "ANTHROPIC_API_KEY environment variable must be set"
+    assert azure_api_key is not None, "AZURE_API_KEY environment variable must be set"
+    assert azure_region is not None, "AZURE_REGION environment variable must be set"
     assert google_tl_key_path is not None, "GOOGLE_TRANSLATE_SERVICE_KEY_VALUE environment variable must be set"
 
     EasyTL.set_credentials("deepl", deepl_api_key)
     EasyTL.set_credentials("gemini", gemini_api_key)
     EasyTL.set_credentials("openai", openai_api_key)
     EasyTL.set_credentials("anthropic", anthropic_api_key)
     EasyTL.set_credentials("google translate", google_tl_key_path)
+    EasyTL.set_credentials("azure", azure_api_key)
 
     schema = {
         "type": "object",
         "properties": {
             "input": {
                 "type": "string",
                 "description": "The text you were given to translate"
@@ -76,21 +87,21 @@
                 "type": "string",
                 "description": "The translated text"
             }
         },
         "required": ["input", "output"]
     }
 
-    return gemini_time_delay, logging_directory, schema
+    return gemini_time_delay, logging_directory, schema, azure_region
 
 ##-------------------start-of-main()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 async def main():
 
-    gemini_time_delay, logging_directory, schema = setup_preconditions()
+    gemini_time_delay, logging_directory, schema, azure_region = setup_preconditions()
 
     decorator = backoff.on_exception(backoff.expo, exception=(DeepLException, GoogleAPIError, OpenAIError, AnthropicAPIError), logger=logging.getLogger())
 
     print("------------------------------------------------Deepl------------------------------------------------")
 
     print("------------------------------------------------Text response------------------------------------------------")
 
@@ -248,14 +259,32 @@
 
     print("------------------------------------------------Cost calculation------------------------------------------------")
 
     tokens, cost, model = EasyTL.calculate_cost(text="Hello, world!", service="anthropic", model="claude-3-haiku-20240307", translation_instructions="Translate this to German.")
 
     print(f"Tokens: {tokens}, Cost: {cost}, Model: {model}")
 
+    print("------------------------------------------------Azure------------------------------------------------")
+    
+    print("-----------------------------------------------Text response-----------------------------------------------")
+
+    print(EasyTL.azure_translate("Hello, world!", target_lang="de", logging_directory=logging_directory, decorator=decorator, azure_region=azure_region))
+    print(await EasyTL.azure_translate_async("Hello, world!", target_lang="de", logging_directory=logging_directory, decorator=decorator, azure_region=azure_region))
+
+    print("-----------------------------------------------JSON response-----------------------------------------------")
+
+    print(EasyTL.azure_translate("Hello, world!", target_lang="de", response_type="json", logging_directory=logging_directory,decorator=decorator, azure_region=azure_region))
+    print(await EasyTL.azure_translate_async("Hello, world!", target_lang="de", response_type="json", logging_directory=logging_directory,decorator=decorator, azure_region=azure_region))
+
+    print("------------------------------------------------Cost calculation------------------------------------------------")
+
+    characters, cost, model = EasyTL.calculate_cost(text="Hello, world!", service="azure", model=None, translation_instructions=None)
+
+    print(f"Characters: {characters}, Cost: {cost}, Model: {model}")   
+
 ##-------------------end-of-main()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 
 
 if(__name__ == "__main__"):
     ## setup logging
     logging.basicConfig(level=logging.DEBUG,
```

