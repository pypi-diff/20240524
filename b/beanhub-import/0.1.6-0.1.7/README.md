# Comparing `tmp/beanhub_import-0.1.6.tar.gz` & `tmp/beanhub_import-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_import-0.1.6.tar", max compression
+gzip compressed data, was "beanhub_import-0.1.7.tar", max compression
```

## Comparing `beanhub_import-0.1.6.tar` & `beanhub_import-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-05-11 07:46:53.301742 beanhub_import-0.1.6/LICENSE
--rw-r--r--   0        0        0    24362 2024-05-11 07:46:53.301742 beanhub_import-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-05-11 07:46:53.309742 beanhub_import-0.1.6/beanhub_import/__init__.py
--rw-r--r--   0        0        0      231 2024-05-11 07:46:53.309742 beanhub_import-0.1.6/beanhub_import/constants.py
--rw-r--r--   0        0        0     4617 2024-05-11 07:46:53.309742 beanhub_import-0.1.6/beanhub_import/data_types.py
--rw-r--r--   0        0        0     7958 2024-05-11 07:46:53.309742 beanhub_import-0.1.6/beanhub_import/post_processor.py
--rw-r--r--   0        0        0    10490 2024-05-11 07:46:53.309742 beanhub_import-0.1.6/beanhub_import/processor.py
--rw-r--r--   0        0        0      276 2024-05-11 07:46:53.309742 beanhub_import-0.1.6/beanhub_import/templates.py
--rw-r--r--   0        0        0      774 2024-05-11 07:46:53.309742 beanhub_import-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    25283 1970-01-01 00:00:00.000000 beanhub_import-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-24 00:31:40.438308 beanhub_import-0.1.7/LICENSE
+-rw-r--r--   0        0        0    24362 2024-05-24 00:31:40.438308 beanhub_import-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 00:31:40.446308 beanhub_import-0.1.7/beanhub_import/__init__.py
+-rw-r--r--   0        0        0      231 2024-05-24 00:31:40.446308 beanhub_import-0.1.7/beanhub_import/constants.py
+-rw-r--r--   0        0        0     4617 2024-05-24 00:31:40.446308 beanhub_import-0.1.7/beanhub_import/data_types.py
+-rw-r--r--   0        0        0     7958 2024-05-24 00:31:40.446308 beanhub_import-0.1.7/beanhub_import/post_processor.py
+-rw-r--r--   0        0        0    10800 2024-05-24 00:31:40.446308 beanhub_import-0.1.7/beanhub_import/processor.py
+-rw-r--r--   0        0        0      276 2024-05-24 00:31:40.446308 beanhub_import-0.1.7/beanhub_import/templates.py
+-rw-r--r--   0        0        0      774 2024-05-24 00:31:40.446308 beanhub_import-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    25283 1970-01-01 00:00:00.000000 beanhub_import-0.1.7/PKG-INFO
```

### Comparing `beanhub_import-0.1.6/LICENSE` & `beanhub_import-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.1.6/README.md` & `beanhub_import-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.1.6/beanhub_import/data_types.py` & `beanhub_import-0.1.7/beanhub_import/data_types.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.1.6/beanhub_import/post_processor.py` & `beanhub_import-0.1.7/beanhub_import/post_processor.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.1.6/beanhub_import/processor.py` & `beanhub_import-0.1.7/beanhub_import/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import pathlib
 import re
 import typing
 
 from beanhub_extract.data_types import Transaction
 from beanhub_extract.extractors import ALL_EXTRACTORS
+from beanhub_extract.extractors import detect_extractor
 from beanhub_extract.utils import strip_txn_base_path
 from jinja2.sandbox import SandboxedEnvironment
 
 from . import constants
 from .data_types import ActionType
 from .data_types import Amount
 from .data_types import GeneratedPosting
@@ -228,16 +229,20 @@
     for filepath in walk_dir_files(input_dir):
         for input_config in import_doc.inputs:
             if not match_file(input_config.match, filepath):
                 continue
             rel_filepath = filepath.relative_to(input_dir)
             extractor_name = input_config.config.extractor
             if extractor_name is None:
-                # TODO: identify input file automatically
-                pass
+                with filepath.open("rt") as fo:
+                    extractor_cls = detect_extractor(fo)
+                if extractor_cls is None:
+                    raise ValueError(
+                        f"Extractor not specified for {rel_filepath} and the extractor type cannot be automatically detected"
+                    )
             else:
                 extractor_cls = ALL_EXTRACTORS.get(extractor_name)
                 if extractor_cls is None:
                     logger.warning(
                         "Extractor %s not found for file %s, skip",
                         extractor_name,
                         rel_filepath,
```

### Comparing `beanhub_import-0.1.6/pyproject.toml` & `beanhub_import-0.1.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "beanhub-import"
-version = "0.1.6"
+version = "0.1.7"
 description = "The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pytz = ">=2023.1,<2025"
 pydantic = ">= 2.0.0, <3.0.0"
 pyyaml = "^6.0.1"
 jinja2 = "^3.1.3"
-beanhub-extract = ">= 0.0.7, <0.1.0"
+beanhub-extract = ">= 0.1.0, <0.2.0"
 beancount-black = ">= 1.0.2, < 1.1.0"
 beancount-parser = ">= 1.2.3, < 1.3.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.1"
```

### Comparing `beanhub_import-0.1.6/PKG-INFO` & `beanhub_import-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: beanhub-import
-Version: 0.1.6
+Version: 0.1.7
 Summary: The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beancount-black (>=1.0.2,<1.1.0)
 Requires-Dist: beancount-parser (>=1.2.3,<1.3.0)
-Requires-Dist: beanhub-extract (>=0.0.7,<0.1.0)
+Requires-Dist: beanhub-extract (>=0.1.0,<0.2.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: pydantic (>=2.0.0,<3.0.0)
 Requires-Dist: pytz (>=2023.1,<2025)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
 
 # beanhub-import [![CircleCI](https://dl.circleci.com/status-badge/img/gh/LaunchPlatform/beanhub-import/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/LaunchPlatform/beanhub-import/tree/master)
```

