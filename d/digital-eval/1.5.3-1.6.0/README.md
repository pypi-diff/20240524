# Comparing `tmp/digital-eval-1.5.3.tar.gz` & `tmp/digital_eval-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital-eval-1.5.3.tar", last modified: Wed Jun 14 12:47:35 2023, max compression
+gzip compressed data, was "digital_eval-1.6.0.tar", last modified: Fri May 24 17:42:51 2024, max compression
```

## Comparing `digital-eval-1.5.3.tar` & `digital_eval-1.6.0.tar`

### file list

```diff
@@ -1,27 +1,36 @@
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-06-14 12:47:35.945068 digital-eval-1.5.3/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1107 2022-07-13 13:34:42.000000 digital-eval-1.5.3/LICENSE
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       11 2022-11-16 10:06:15.000000 digital-eval-1.5.3/MANIFEST.in
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5798 2023-06-14 12:47:35.945068 digital-eval-1.5.3/PKG-INFO
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5206 2023-04-17 10:19:40.000000 digital-eval-1.5.3/README.md
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       87 2022-11-15 13:27:11.000000 digital-eval-1.5.3/pyproject.toml
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      942 2023-06-14 12:47:35.945068 digital-eval-1.5.3/setup.cfg
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-06-14 12:47:35.941068 digital-eval-1.5.3/src/
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-06-14 12:47:35.945068 digital-eval-1.5.3/src/digital_eval/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        6 2023-06-14 12:18:33.000000 digital-eval-1.5.3/src/digital_eval/VERSION
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      617 2023-06-07 13:56:39.000000 digital-eval-1.5.3/src/digital_eval/__init__.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     8595 2023-06-14 12:21:18.000000 digital-eval-1.5.3/src/digital_eval/cli.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    28651 2023-06-14 11:00:54.000000 digital-eval-1.5.3/src/digital_eval/evaluation.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    17660 2023-06-07 14:05:05.000000 digital-eval-1.5.3/src/digital_eval/metrics.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    26728 2023-06-14 12:27:00.000000 digital-eval-1.5.3/src/digital_eval/model.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    14939 2022-11-15 13:27:11.000000 digital-eval-1.5.3/src/digital_eval/model_legacy.py
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-06-14 12:47:35.945068 digital-eval-1.5.3/src/digital_eval.egg-info/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5798 2023-06-14 12:47:35.000000 digital-eval-1.5.3/src/digital_eval.egg-info/PKG-INFO
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      559 2023-06-14 12:47:35.000000 digital-eval-1.5.3/src/digital_eval.egg-info/SOURCES.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        1 2023-06-14 12:47:35.000000 digital-eval-1.5.3/src/digital_eval.egg-info/dependency_links.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       86 2023-06-14 12:47:35.000000 digital-eval-1.5.3/src/digital_eval.egg-info/entry_points.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       31 2023-06-14 12:47:35.000000 digital-eval-1.5.3/src/digital_eval.egg-info/requires.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       22 2023-06-14 12:47:35.000000 digital-eval-1.5.3/src/digital_eval.egg-info/top_level.txt
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-06-14 12:47:35.945068 digital-eval-1.5.3/src/ocr_util/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       21 2023-03-28 09:38:32.000000 digital-eval-1.5.3/src/ocr_util/__init__.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     2690 2023-04-17 08:33:00.000000 digital-eval-1.5.3/src/ocr_util/cli.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     4120 2023-04-17 08:29:20.000000 digital-eval-1.5.3/src/ocr_util/frame.py
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-05-24 17:42:51.308904 digital_eval-1.6.0/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1107 2022-07-13 16:50:10.000000 digital_eval-1.6.0/LICENSE
+-rw-r--r--   0 hartwig   (1000) hartwig   (1000)     5988 2024-05-24 17:42:51.308904 digital_eval-1.6.0/PKG-INFO
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5381 2024-05-24 17:32:10.000000 digital_eval-1.6.0/README.md
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      869 2024-05-24 17:32:10.000000 digital_eval-1.6.0/pyproject.toml
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       38 2024-05-24 17:42:51.308904 digital_eval-1.6.0/setup.cfg
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-05-24 17:42:51.304904 digital_eval-1.6.0/src/
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-05-24 17:42:51.304904 digital_eval-1.6.0/src/digital_eval/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      331 2024-05-24 17:32:10.000000 digital_eval-1.6.0/src/digital_eval/__init__.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     8447 2024-05-24 17:32:10.000000 digital_eval-1.6.0/src/digital_eval/cli.py
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-05-24 17:42:51.308904 digital_eval-1.6.0/src/digital_eval/dictionary_metrics/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        0 2024-05-16 19:04:39.000000 digital_eval-1.6.0/src/digital_eval/dictionary_metrics/__init__.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1902 2024-05-16 19:04:39.000000 digital_eval-1.6.0/src/digital_eval/dictionary_metrics/common.py
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-05-24 17:42:51.308904 digital_eval-1.6.0/src/digital_eval/dictionary_metrics/language_tool/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     3711 2024-05-16 19:04:39.000000 digital_eval-1.6.0/src/digital_eval/dictionary_metrics/language_tool/LanguageTool.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     2923 2024-05-16 19:04:39.000000 digital_eval-1.6.0/src/digital_eval/dictionary_metrics/language_tool/Util.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        0 2024-05-16 19:04:39.000000 digital_eval-1.6.0/src/digital_eval/dictionary_metrics/language_tool/__init__.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1285 2024-05-16 19:04:39.000000 digital_eval-1.6.0/src/digital_eval/dictionary_metrics/language_tool/common.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    25488 2024-05-24 17:32:10.000000 digital_eval-1.6.0/src/digital_eval/evaluation.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    20767 2024-05-24 17:32:10.000000 digital_eval-1.6.0/src/digital_eval/metrics.py
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-05-24 17:42:51.308904 digital_eval-1.6.0/src/digital_eval.egg-info/
+-rw-r--r--   0 hartwig   (1000) hartwig   (1000)     5988 2024-05-24 17:42:51.000000 digital_eval-1.6.0/src/digital_eval.egg-info/PKG-INFO
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      912 2024-05-24 17:42:51.000000 digital_eval-1.6.0/src/digital_eval.egg-info/SOURCES.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        1 2024-05-24 17:42:51.000000 digital_eval-1.6.0/src/digital_eval.egg-info/dependency_links.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       86 2024-05-24 17:42:51.000000 digital_eval-1.6.0/src/digital_eval.egg-info/entry_points.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       61 2024-05-24 17:42:51.000000 digital_eval-1.6.0/src/digital_eval.egg-info/requires.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       22 2024-05-24 17:42:51.000000 digital_eval-1.6.0/src/digital_eval.egg-info/top_level.txt
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-05-24 17:42:51.308904 digital_eval-1.6.0/src/ocr_util/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        1 2024-05-16 19:04:39.000000 digital_eval-1.6.0/src/ocr_util/__init__.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     2615 2024-05-24 17:32:10.000000 digital_eval-1.6.0/src/ocr_util/cli.py
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-05-24 17:42:51.308904 digital_eval-1.6.0/tests/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     3533 2024-05-24 17:32:10.000000 digital_eval-1.6.0/tests/test_dict_metric.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1896 2024-05-24 17:32:10.000000 digital_eval-1.6.0/tests/test_digital_eval_cli.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    13488 2024-05-24 17:32:10.000000 digital_eval-1.6.0/tests/test_ocr_evaluate.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    11847 2024-05-24 17:32:10.000000 digital_eval-1.6.0/tests/test_ocr_metrics.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     4743 2024-05-24 17:32:10.000000 digital_eval-1.6.0/tests/test_ocr_metrics_base.py
```

### Comparing `digital-eval-1.5.3/LICENSE` & `digital_eval-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `digital-eval-1.5.3/PKG-INFO` & `digital_eval-1.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 Metadata-Version: 2.1
 Name: digital-eval
-Version: 1.5.3
-Summary: Evaluate Mass Digitalization Data
-Author: Universitäts- und Landesbibliothek Sachsen-Anhalt
-Author-email: development@bibliothek.uni-halle.de
-Maintainer: Uwe Hartwig
-Maintainer-email: uwe.hartwig@bibliothek.uni-halle.de
+Version: 1.6.0
+Summary: Evaluate Digitalization Data
+Author-email: Universitäts- und Landesbibliothek Sachsen-Anhalt <development@bibliothek.uni-halle.de>
 Project-URL: Homepage, https://github.com/ulb-sachsen-anhalt/digital-eval
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: rapidfuzz>3
+Requires-Dist: nltk
+Requires-Dist: requests
+Requires-Dist: docker
+Requires-Dist: numpy
+Requires-Dist: digital-object==0.2.0
 
 # digital eval
 
 ![example workflow](https://github.com/ulb-sachsen-anhalt/digital-eval/actions/workflows/python-app.yml/badge.svg)
 [![PyPi version](https://badgen.net/pypi/v/digital-eval/)](https://pypi.org/project/digital-eval) ![PyPI - Downloads](https://img.shields.io/pypi/dm/digital-eval) ![PyPI - License](https://img.shields.io/pypi/l/digital-eval) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/digital-eval)
 
 Python3 Tool to report evaluation outcomes from mass digitalization workflows.
 
 ## Features
 
-* match automatically groundtruth (i.e. reference data) and candidates by filename
+* [OCR-D compliant](https://ocr-d.de/en/spec/ocrd_eval#character-error-rate-cer) normalized similarity for edit-distance based metrics based on characters, letters and words
+* choose from textual metrics based on characters or words plus common Information Retrieval
+* choose from different UTF-8 Python norms
+* match groundtruth (i.e. reference data) and candidates by filename start
 * use geometric information to evaluate only specific frame (i.e. specific column or region from large page) of
   candidates (requires ALTO or PAGE format)
-* aggregate evaluation outcome on domain range (with multiple subdomains)
-* choose from textual metrics based on characters or words plus common Information Retrieval
-* choose between accuracy / error rate and different UTF-8 Python norms
+* aggregate evaluation outcomes on domain range (with multiple subdomains) according to folder layout
 * formats: ALTO, PAGE or plain text for both groundtruth and candidates
 * speedup with parallel execution
 * additional OCR util:
-  * filter custom areas of single OCR files
+  * filter custom areas of single OCR files of ALTO files
 
 ## Installation
 
 ```bash
 pip install digital-eval
 ```
 
 ## Usage
 
 ### Metrics
 
-Calculate similarity (`acc`) or difference (`err`) ratios between single reference/groundtruth and test/candidate item.
-
-#### Edit-Distance based
+#### Edit-Distance based Strin Similarity
 
-Character-based text string minus whitechars (`Cs`, `Characters`) or Letter-based (`Ls`, `Letters`) minus whites,
-punctuation and digits.
-Word/Token-based edit-distance of single tokens identified by whitespaces.
+Calculate similarity for each single reference/groundtruth and test/candidate item.
+Complete haracter-based text string (`Cs`, `Characters`) or Letter-based (`Ls`, `Letters`) minus whitespaces,
+punctuation and common digits (arabic, persian). 
+Word/Token-based edit-distance of single tokens identified by Word or String elements or whitespaces, depending on data.
 
 #### Set based
 
 Calculate union of sets of tokens/words (`BoW`, `BagOfWords`).
 Operate on sets of tokens/words with respect to language specific stopwords using [nltk](https://www.nltk.org/)
 -framework for:
 
@@ -130,35 +132,32 @@
 Plattform: Intel(R) Core(TM) i5-6500 CPU@3.20GHz, 16GB RAM, Ubuntu 20.04 LTS, Python 3.8.
 
 ```bash
 # clone local
 git clone <repository-url> <local-dir>
 cd <local-dir>
 
-# enable virtual python environment (linux)
-# and install libraries
+# enable virtual python 3 environment (linux)
+# and update pip itself
 python3 -m venv venv
 . venv/bin/activate
 python -m pip install -U pip
-python -m pip install -r requirements.txt
 
 # install
-pip install .
+python -m pip install -e .
 
-# optional:
 # install additional development dependencies
-pip install -r tests/test_requirements.txt
-pytest -v
+python -m pip install -r tests/test_requirements.txt
 
-# run
-digital-eval --help
+# run tests
+python -m pytest -v
 ```
 
 ## Contribute
 
 Contributions, suggestions and proposals welcome!
 
-## Licence
+## License
 
 Under terms of the [MIT license](https://opensource.org/licenses/MIT).
 
-**NOTE**: This software depends on other packages that _may_ be licensed under different open source licenses.
+**NOTE**: This software depends on packages that _might_ be licensed under different terms.
```

### Comparing `digital-eval-1.5.3/README.md` & `digital_eval-1.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,42 +3,42 @@
 ![example workflow](https://github.com/ulb-sachsen-anhalt/digital-eval/actions/workflows/python-app.yml/badge.svg)
 [![PyPi version](https://badgen.net/pypi/v/digital-eval/)](https://pypi.org/project/digital-eval) ![PyPI - Downloads](https://img.shields.io/pypi/dm/digital-eval) ![PyPI - License](https://img.shields.io/pypi/l/digital-eval) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/digital-eval)
 
 Python3 Tool to report evaluation outcomes from mass digitalization workflows.
 
 ## Features
 
-* match automatically groundtruth (i.e. reference data) and candidates by filename
+* [OCR-D compliant](https://ocr-d.de/en/spec/ocrd_eval#character-error-rate-cer) normalized similarity for edit-distance based metrics based on characters, letters and words
+* choose from textual metrics based on characters or words plus common Information Retrieval
+* choose from different UTF-8 Python norms
+* match groundtruth (i.e. reference data) and candidates by filename start
 * use geometric information to evaluate only specific frame (i.e. specific column or region from large page) of
   candidates (requires ALTO or PAGE format)
-* aggregate evaluation outcome on domain range (with multiple subdomains)
-* choose from textual metrics based on characters or words plus common Information Retrieval
-* choose between accuracy / error rate and different UTF-8 Python norms
+* aggregate evaluation outcomes on domain range (with multiple subdomains) according to folder layout
 * formats: ALTO, PAGE or plain text for both groundtruth and candidates
 * speedup with parallel execution
 * additional OCR util:
-  * filter custom areas of single OCR files
+  * filter custom areas of single OCR files of ALTO files
 
 ## Installation
 
 ```bash
 pip install digital-eval
 ```
 
 ## Usage
 
 ### Metrics
 
-Calculate similarity (`acc`) or difference (`err`) ratios between single reference/groundtruth and test/candidate item.
-
-#### Edit-Distance based
+#### Edit-Distance based Strin Similarity
 
-Character-based text string minus whitechars (`Cs`, `Characters`) or Letter-based (`Ls`, `Letters`) minus whites,
-punctuation and digits.
-Word/Token-based edit-distance of single tokens identified by whitespaces.
+Calculate similarity for each single reference/groundtruth and test/candidate item.
+Complete haracter-based text string (`Cs`, `Characters`) or Letter-based (`Ls`, `Letters`) minus whitespaces,
+punctuation and common digits (arabic, persian). 
+Word/Token-based edit-distance of single tokens identified by Word or String elements or whitespaces, depending on data.
 
 #### Set based
 
 Calculate union of sets of tokens/words (`BoW`, `BagOfWords`).
 Operate on sets of tokens/words with respect to language specific stopwords using [nltk](https://www.nltk.org/)
 -framework for:
 
@@ -114,35 +114,32 @@
 Plattform: Intel(R) Core(TM) i5-6500 CPU@3.20GHz, 16GB RAM, Ubuntu 20.04 LTS, Python 3.8.
 
 ```bash
 # clone local
 git clone <repository-url> <local-dir>
 cd <local-dir>
 
-# enable virtual python environment (linux)
-# and install libraries
+# enable virtual python 3 environment (linux)
+# and update pip itself
 python3 -m venv venv
 . venv/bin/activate
 python -m pip install -U pip
-python -m pip install -r requirements.txt
 
 # install
-pip install .
+python -m pip install -e .
 
-# optional:
 # install additional development dependencies
-pip install -r tests/test_requirements.txt
-pytest -v
+python -m pip install -r tests/test_requirements.txt
 
-# run
-digital-eval --help
+# run tests
+python -m pytest -v
 ```
 
 ## Contribute
 
 Contributions, suggestions and proposals welcome!
 
-## Licence
+## License
 
 Under terms of the [MIT license](https://opensource.org/licenses/MIT).
 
-**NOTE**: This software depends on other packages that _may_ be licensed under different open source licenses.
+**NOTE**: This software depends on packages that _might_ be licensed under different terms.
```

### Comparing `digital-eval-1.5.3/src/digital_eval/cli.py` & `digital_eval-1.6.0/src/digital_eval/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,258 +1,224 @@
 # -*- coding: utf-8 -*-
 """OCR QA Evaluation CLI"""
 
 import argparse
 import os
 import sys
+import typing
 
-import datetime as dt
+import digital_eval as digev
+import digital_eval.dictionary_metrics.common as digev_cm
+import digital_eval.metrics as digem
+from digital_eval.dictionary_metrics.language_tool.LanguageTool import LanguageTool
 
-from typing import (
-    List, Type
-)
-
-from digital_eval import (
-    find_groundtruth,
-    gather_candidates,
-    Evaluator,
-    report_stdout,
-    ocr_to_text,
-    UC_NORMALIZATION_DEFAULT,
-    accuracy_for,
-    error_for,
-    MetricChars,
-    MetricLetters,
-    MetricWords,
-    MetricBoW,
-    MetricIRPre,
-    MetricIRRec,
-    MetricIRFM
-)
-from digital_eval.metrics import OCRDifferenceMetric, accuracy_for_bow, error_for_bow
 
 # script constants
 DEFAULT_VERBOSITY = 0
 VERBOSITY = DEFAULT_VERBOSITY
 EVAL_VERBOSITY = DEFAULT_VERBOSITY
-
-# calculations
-DEFAULT_CALCULCATION = 'acc'
-CALC_DICT = {
-    'acc': accuracy_for,
-    'accuracy': accuracy_for,
-    'err': error_for,
-    'error': error_for,
-}
-
-CALC_DICT_BOW = {
-    'acc': accuracy_for_bow,
-    'accuracy': accuracy_for_bow,
-    'err': error_for_bow,
-    'error': error_for_bow,
-}
-
-DEFAULT_UTF8_NORM = UC_NORMALIZATION_DEFAULT
+DEFAULT_UTF8_NORM = digev.UC_NORMALIZATION_DEFAULT
 
 # metrics
 DEFAULT_OCR_METRICS = 'Cs,Ls'
 DEFAULT_OCR_METRIC_PREPROCESSINGS = ''
 DEFAULT_OCR_METRIC_POSTPROCESSINGS = ''
 METRIC_DICT = {
-    'Cs': MetricChars,
-    'Characters': MetricChars,
-    'Ls': MetricLetters,
-    'Letters': MetricLetters,
-    'Ws': MetricWords,
-    'Words': MetricWords,
-    'BoWs': MetricBoW,
-    'BagOfWords': MetricBoW,
-    'IRPre': MetricIRPre,
-    'Pre': MetricIRPre,
-    'Precision': MetricIRPre,
-    'IRRec': MetricIRRec,
-    'Rec': MetricIRRec,
-    'IRFMeasure': MetricIRFM,
-    'FM': MetricIRFM,
+    'Cs': digev.MetricChars,
+    'Characters': digev.MetricChars,
+    'Ls': digev.MetricLetters,
+    'Letters': digev.MetricLetters,
+    'Ws': digev.MetricWords,
+    'Words': digev.MetricWords,
+    'BoWs': digev.MetricBoW,
+    'BagOfWords': digev.MetricBoW,
+    'IRPre': digev.MetricIRPre,
+    'Pre': digev.MetricIRPre,
+    'Precision': digev.MetricIRPre,
+    'IRRec': digev.MetricIRRec,
+    'Rec': digev.MetricIRRec,
+    'IRFMeasure': digev.MetricIRFM,
+    'FM': digev.MetricIRFM,
+    'DictLT': digem.MetricDictionaryLangTool,
+    'DictionaryLangTool': digem.MetricDictionaryLangTool,
 }
 
 
-def _get_info():
-    here = os.path.abspath(os.path.dirname(__file__))
-    _v = ''
-    _t = ''
-    _fp = os.path.join(here, 'VERSION')
-    with open(_fp) as fp:
-        _v = fp.read()
-    _t = dt.datetime.fromtimestamp(os.stat(_fp).st_mtime).strftime("%Y-%m-%d")
-    return f'v{_v}/{_t}'
-
-
-def _initialize_metrics(the_metrics, norm, calc) -> List[OCRDifferenceMetric]:
+def _initialize_metrics(
+        the_metrics,
+        norm,
+) -> typing.List[digem.SimilarityMetric]:
     _tokens = the_metrics.split(',')
     try:
-        metric_objects: List[OCRDifferenceMetric] = []
+        metric_objects: typing.List[digem.SimilarityMetric] = []
         for m in _tokens:
-            clazz: Type[OCRDifferenceMetric] = METRIC_DICT[m]
-            calc_func = CALC_DICT[calc]
-            if m == 'BoWs' or m == 'BagOfWords':
-                calc_func = CALC_DICT_BOW[calc]
-            metric_inst: OCRDifferenceMetric = clazz(normalization=norm, calc_func=calc_func)
+            clazz: typing.Type[digem.SimilarityMetric] = METRIC_DICT[m]
+            if 'Dict' in m:
+                norm = digem.UC_NORMALIZATION_NFKD
+            metric_inst: digem.SimilarityMetric = clazz(normalization=norm)
             metric_objects.append(metric_inst)
         return metric_objects
     except KeyError as _err:
-        _keys = ','.join(METRIC_DICT.keys()) + ','.join(CALC_DICT.keys())
+        _keys = ','.join(METRIC_DICT.keys())
         _msg = f"Unknown: '{_err.args[0]}'.\nPlease use one of the following keys: '{_keys}'."
         print(_msg)
         sys.exit(1)
 
 
-########
-# MAIN #
-########
-def _main(path_candidates, path_reference, metrics, utf8norm, calc, xtra, is_legacy=False, is_sequential=False):
+#########
+# START #
+#########
+def start_evaluation(parse_args: typing.Dict):
+    """Main workflow"""
+
+    path_candidates = parse_args["candidates"]
+    path_reference = parse_args["reference"]
+    metrics: str = parse_args["metrics"]
+    utf8norm = parse_args["utf8"]
+    verbosity = parse_args["verbosity"]
+    is_seq = parse_args["sequential"] if "sequential" in parse_args else False
+    xtra = parse_args["extra"] if "extra" in parse_args else None
+
+    if "language" in parse_args:
+        digem.MetricDictionary.LANGUAGE = parse_args["language"]
+    uses_lang_tool: bool = 'DictLT' in metrics or "DictionaryLangTool" in metrics
+    if uses_lang_tool:
+        lt_url: str = parse_args["lt_api_url"] if "lp_api_url" in parse_args else LanguageTool.DEFAULT_URL
+        LanguageTool.initialize(lt_url)
+
+    # go on with basic validation
+    if not os.path.isdir(path_candidates):
+        print(f'[ERROR] input "{path_candidates}": invalid directory! exit!')
+        sys.exit(1)
+    if path_reference and not os.path.isdir(path_reference):
+        print(f'[ERROR] reference "{path_reference}": invalid directory! exit!')
+        sys.exit(1)
+
+    # sanitize trailing slash
+    if not isinstance(path_candidates, str):
+        path_candidates = str(path_candidates)
+    if not isinstance(path_reference, str):
+        path_reference = str(path_reference)
+    path_candidates = path_candidates[:-1] if path_candidates.endswith('/') else path_candidates
+    path_reference = path_reference[:-1] if path_reference.endswith('/') else path_reference
+
+    # if candidates and both reference provided: do domains match?
+    if path_candidates and path_reference:
+        _base_can = os.path.basename(path_candidates)
+        _base_ref = os.path.basename(path_reference)
+        if _base_can != _base_ref:
+            print(f"[WARN ] start domains '{_base_can}' and '{_base_ref}' mismatch, summary might be inaccurate!")
+
+    # some diagnostics
+    if verbosity >= 2:
+        args = f"{path_candidates}, {path_reference}, {verbosity}, {xtra}"
+        print(f'[DEBUG] called with {args}')
 
     # create basic evaluator instance
-    evaluator = Evaluator(path_candidates, VERBOSITY, xtra)
-    evaluator.metrics = _initialize_metrics(metrics, norm=utf8norm, calc=calc)
-    evaluator.calc = calc
-    if VERBOSITY >= 1:
-        print(f"[DEBUG] text normalized using '{utf8norm}' calculate '{calc}' metric values for '{metrics}'")
-
-    if is_legacy:
-        evaluator.to_text_func = ocr_to_text
-    evaluator.is_sequential = is_sequential
+    evaluator = digev.Evaluator(
+        path_candidates,
+        verbosity=verbosity,
+        extras=xtra,
+    )
+    evaluator.metrics = _initialize_metrics(metrics, norm=utf8norm)#, calc=calc)
+    if verbosity >= 1:
+        print(f"[DEBUG] text normalized using '{utf8norm}' code points for '{metrics}'")
+
+    evaluator.is_sequential = is_seq
     evaluator.domain_reference = path_reference
 
     # gather structure information
-    candidates = gather_candidates(path_candidates)
+    candidates = digev.gather_candidates(path_candidates)
     if not candidates:
         print(f"[WARN ] no ocr data (.*xml) in any dir starting from '{path_candidates}'! exit.")
         sys.exit(0)
 
     # match groundtruth
     for entry in candidates:
-        gt = find_groundtruth(entry.path_c, path_candidates, path_reference)
+        gt = digev.find_groundtruth(entry.path_c, path_candidates, path_reference)
         if gt:
             entry.path_g = gt
 
     # remove all paths where no groundtruth exists
     gt_entries = [c for c in candidates if c.path_g]
     n_entries = len(candidates)
     n_diff = n_entries - len(gt_entries)
     gt_missing = set(gt_entries) ^ set(candidates)
     rnd_str = f" ({gt_missing})" if gt_missing else ""
-    if VERBOSITY >= 1:
+    if verbosity >= 1:
         print(f'[DEBUG] from "{n_entries}" filtered "{n_diff}" candidates missing groundtruth{rnd_str}')
 
     # trigger actual evaluation
     evaluator.eval_all(gt_entries)
 
     # aggregate
     evaluator.aggregate(by_type=True)
 
     # evaluator.evaluate()
     evaluator.eval_map()
 
-    # get results
-    # results = evaluator.get_results()
-
     # serialize stdout report
-    if VERBOSITY >= 0:
-        report_stdout(evaluator, VERBOSITY)
+    if verbosity >= 0:
+        digev.report_stdout(evaluator, verbosity)
+
+    # for testing purposes
+    eval_results =  evaluator.get_results()
+
+    # final clean-up
+    if uses_lang_tool:
+        LanguageTool.deinitialize()
+
+    return eval_results
 
 
 def start():
-    PARSER = argparse.ArgumentParser(description=f"""
-        Evaluate Mass Digital Data. ({_get_info()})
-        """)
-    PARSER.add_argument(
-        "candidates",
-        help="Root Directory for evaluation candidates"
-    )
-    PARSER.add_argument("-ref", "--reference",
+    """Wrap argparsing"""
+    parser = argparse.ArgumentParser(description=f"Evaluate Mass Digitalization Data {digev.__version__}")
+    parser.add_argument("candidates",
+                        help="Root Directory for evaluation candidates"
+                        )
+    parser.add_argument("-ref", "--reference",
                         required=False,
                         help="Root directory for Reference/Groundtruth data (optional, but necessary for most metrics)"
                         )
-    PARSER.add_argument("-v", "--VERBOSITY",
+    parser.add_argument("-v", "--verbosity",
                         action='count',
                         default=DEFAULT_VERBOSITY,
                         required=False,
                         help=f"Verbosity flag. To increase, append multiple 'v's (optional; default: '{DEFAULT_VERBOSITY}')"
                         )
-    PARSER.add_argument("--calc",
-                        default=DEFAULT_CALCULCATION,
-                        required=False,
-                        help=f"Calculation to perform (optional; default: '{DEFAULT_CALCULCATION}'; available: '{','.join(CALC_DICT.keys())}')"
-                        )
-    # metrics
-    PARSER.add_argument("--metrics",
+    parser.add_argument("--metrics",
                         default=DEFAULT_OCR_METRICS,
                         required=False,
                         help=f"List of metrics to use (optional, default: '{DEFAULT_OCR_METRICS}'; available: '{','.join(METRIC_DICT.keys())}')"
                         )
-    PARSER.add_argument("--legacy",
-                        action='store_true',
-                        required=False,
-                        help="legacy evaluation with naive rectangular geometry (optional; default: 'False')",
-                        )
-    PARSER.add_argument("--utf8",
+    parser.add_argument("--utf8",
                         default=DEFAULT_UTF8_NORM,
                         required=False,
                         help=f"UTF-8 Unicode Python Normalization (optional; default: '{DEFAULT_UTF8_NORM}'; available: 'NFC','NFKC','NFD','NFKD')",
                         )
-    PARSER.add_argument("--sequential",
+    parser.add_argument("-s", "--sequential",
                         action='store_true',
                         required=False,
                         help="Execute calculations sequentially (optional; default: 'False')",
                         )
-    PARSER.add_argument("-x", "--extra",
+    parser.add_argument("-x", "--extra",
                         required=False,
                         help="pass additional information to evaluation, like 'ignore_geometry' (compare only text, ignore coords)"
                         )
-    PARSER.set_defaults(legacy=False)
-    PARSER.set_defaults(sequential=False)
-
-    ARGS = vars(PARSER.parse_args())
-    path_candidates = ARGS["candidates"]
-    path_reference = ARGS["reference"]
-    global VERBOSITY
-    VERBOSITY = ARGS["VERBOSITY"]
-    IS_LEGACY = ARGS["legacy"]
-    IS_SEQUENTIAL = ARGS["sequential"]
-    xtra = ARGS["extra"]
-    metrics = ARGS["metrics"]
-    calc = ARGS["calc"]
-    utf8norm = ARGS["utf8"]
-
-    # go on
-    # basic validation
-    if not os.path.isdir(path_candidates):
-        print(f'[ERROR] input "{path_candidates}": invalid directory! exit!')
-        sys.exit(1)
-    if path_reference and not os.path.isdir(path_reference):
-        print(f'[ERROR] reference "{path_reference}": invalid directory! exit!')
-        sys.exit(1)
-
-    # sanitize trailing slash
-    path_candidates = path_candidates[:-1] if path_candidates.endswith('/') else path_candidates
-    path_reference = path_reference[:-1] if path_reference.endswith('/') else path_reference
-
-    # if candidates and both reference provided: do domains match?
-    if path_candidates and path_reference:
-        _base_can = os.path.basename(path_candidates)
-        _base_ref = os.path.basename(path_reference)
-        if _base_can != _base_ref:
-            print(f"[WARN ] start domains '{_base_can}' and '{_base_ref}' mismatch, summary might be inaccurate!")
-
-    # some diagnostics
-    if VERBOSITY >= 2:
-        args = f"{path_candidates}, {path_reference}, {VERBOSITY}, {xtra}"
-        print(f'[DEBUG] called with {args}')
-
-    # here we go
-    _main(path_candidates, path_reference, metrics, utf8norm, calc, xtra, is_legacy=IS_LEGACY,
-          is_sequential=IS_SEQUENTIAL)
+    parser.add_argument('-l', "--language",
+                        default=digev_cm.LANGUAGE_KEY_DEFAULT,
+                        choices=digev_cm.LANGUAGE_KEYS,
+                        required=False,
+                        help=f"Language code for LanguagTool according to ISO 639-2 (optional; default: '{digev_cm.LANGUAGE_KEY_DEFAULT}')",
+                        )
+    parser.add_argument('-u', "--lt-api-url",
+                        default=LanguageTool.DEFAULT_URL,
+                        required=False,
+                        help=f"Language Tool Api URL (optional; default: '{LanguageTool.DEFAULT_URL}')",
+                        )
+    main_args = vars(parser.parse_args())
+    start_evaluation(main_args)
 
 
 if __name__ == "__main__":
     start()
```

### Comparing `digital-eval-1.5.3/src/digital_eval/evaluation.py` & `digital_eval-1.6.0/src/digital_eval/evaluation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,30 @@
 # -*- coding: utf-8 -*-
 """OCR Evaluation Module"""
+from __future__ import annotations
 
 import concurrent.futures
 import copy
+import datetime
+import math
+import multiprocessing
 import os
 import re
 import sys
+import typing
 import xml.dom.minidom
 import xml.etree.ElementTree as ET
-from datetime import (
-    date
-)
-from math import (
-    floor
-)
-from multiprocessing import (
-    cpu_count
-)
+
 from pathlib import (
     Path
 )
-from typing import (
-    List,
-    Tuple,
-)
 
 import numpy as np
 
-from digital_eval.model import (
-    Piece,
-    PieceLevel,
-    to_pieces,
-)
-from digital_eval.model_legacy import (
-    OCRData,
-)
+import digital_eval.metrics as digem
 
 PAGE_2013 = 'http://schema.primaresearch.org/PAGE/gts/pagecontent/2013-07-15'
 XML_NS = {'alto': 'http://www.loc.gov/standards/alto/ns-v3#',
           'pg2013': PAGE_2013}
 
 # just use textual information for evaluation
 # do *not* respect any geometrics
@@ -75,15 +61,15 @@
 
     the_mean = np.mean(data_points)
     the_deviation = np.std(data_points)
     the_median = np.median(data_points)
     return (the_mean, the_deviation, the_median)
 
 
-def gather_candidates(start_path) -> List:
+def gather_candidates(start_path) -> typing.List[EvalEntry]:
     candidates = []
     if os.path.isdir(start_path):
         for curr_dir, _, files in os.walk(start_path):
             xml_files = [f for f in files if str(f).endswith('.xml')]
             if xml_files:
                 for xml_file in xml_files:
                     rel_path = os.path.join(curr_dir, xml_file)
@@ -93,41 +79,40 @@
         candidates.append(EvalEntry(start_path))
 
     candidates.sort(key=lambda e: e.path_c)
     return candidates
 
 
 def find_groundtruth(path_candidate, root_candidates, root_groundtruth):
-    file_name = os.path.basename(path_candidate)
-    file_dir = os.path.dirname(path_candidate)
-    path_segmts = file_dir.split(os.sep)
+    candidate_name = os.path.basename(path_candidate)
+    candidate_dir = os.path.dirname(path_candidate)
+    cand_path_segmts = candidate_dir.split(os.sep)
     candidate_root_dir = os.path.basename(root_candidates) if os.path.isdir(
         root_candidates) else os.path.dirname(root_candidates)
-    _segm_cand = path_segmts.pop()
-    _segm_gt = [os.path.splitext(file_name)[0]]
+    _segm_cand = cand_path_segmts.pop()
+    _segm_gt = [os.path.splitext(candidate_name)[0]]
     while candidate_root_dir != _segm_cand:
         _segm_gt.append(_segm_cand)
-        _segm_cand = path_segmts.pop()
+        _segm_cand = cand_path_segmts.pop()
     _segm_gt.reverse()
     _gt_path = str(os.sep).join(_segm_gt)
     groundtruth_filepath = os.path.join(root_groundtruth, _gt_path)
     groundtruth_filepath_parent = os.path.dirname(groundtruth_filepath)
     if os.path.exists(groundtruth_filepath_parent):
         path_groundtruth = match_candidate(groundtruth_filepath)
         return path_groundtruth
 
 
 def match_candidates(path_candidates, path_gt_file):
     '''Find candidates that match groundtruth'''
 
     if not os.path.isdir(path_candidates):
-        raise IOError('invalid ocr result path "{}"'.format(path_candidates))
+        raise IOError(f'invalid ocr result path "{path_candidates}"')
     if not os.path.exists(path_gt_file):
-        raise IOError(
-            'invalid groundtruth data path "{}"'.format(path_gt_file))
+        raise IOError(f'invalid groundtruth data path "{path_gt_file}"')
 
     gt_filename = os.path.basename(path_gt_file)
 
     # 0: assume groundtruth is xml data
     cleared_name = ''
     if gt_filename.endswith('.xml'):
         # 1: get image name from metadata
@@ -203,15 +188,15 @@
     return False
 
 
 def get_bbox_data(file_path):
     '''Get Bounding Box Data from given resource, if any exists'''
 
     if not os.path.exists(file_path):
-        raise IOError('{} not existing!'.format(file_path))
+        raise IOError(f'{file_path} not existing!')
 
     # 1: inspect filename
     file_name = os.path.basename(file_path)
     result = re.match(r'.*_(\d{2,})x(\d{2,})_(\d{2,})x(\d{2,})', file_name)
     if result:
         groups = result.groups()
         x0 = int(groups[0])
@@ -264,162 +249,53 @@
             if _frame_points:
                 return _frame_points
             else:
                 raise RuntimeError(f"{file_path} missing page/line coords!")
     return None
 
 
-def _map_alto(e: ET.Element) -> Tuple[str, int, int, int, int]:
+def _map_alto(e: ET.Element) -> typing.Tuple[str, int, int, int, int]:
     i = e.attrib['ID']
     x0 = int(e.attrib['HPOS'])
     y0 = int(e.attrib['VPOS'])
     x1 = x0 + int(e.attrib['WIDTH'])
     y1 = y0 + int(e.attrib['HEIGHT'])
     return (i, x0, y0, x1, y1)
 
 
-def _map_page2013(elem: ET.Element) -> Tuple[str, int, int, int, int]:
+def _map_page2013(elem: ET.Element) -> typing.Tuple[str, int, int, int, int]:
     points = elem.attrib['points'].strip().split(' ')
     _xs = [int(p.split(',')[0]) for p in points]
     _ys = [int(p.split(',')[1]) for p in points]
     return (NOT_SET, min(_xs), min(_ys), max(_xs), max(_ys))
 
 
-def calculate_bounding_box(elements: List[ET.Element], map_func) -> Tuple[int, int, int, int]:
+def calculate_bounding_box(elements: typing.List[ET.Element], map_func) -> typing.Tuple[int, int, int, int]:
     """Review element's points to get points for
     minimum (top-left) and maximum (bottom-right)"""
 
     all_points = [map_func(e) for e in elements]
     all_x1 = [p[1] for p in all_points]
     all_y1 = [p[2] for p in all_points]
     all_x2 = [p[3] for p in all_points]
     all_y2 = [p[4] for p in all_points]
     return ((min(all_x1), min(all_y1)), (max(all_x2), max(all_y2)))
 
 
-def ocr_to_text(file_path, coords=None, oneliner=False) -> Tuple:
-    """Create representation which contains
-    * groundtruth type (if annotated)
-    * groundtruth text (as string or list of lines)
-    * number of text lines
-
-    DEPRECATED
-
-    """
-
-    gt_type = NOT_SET
-    try:
-        ocr_data = OCRData(file_path)
-
-        # optional groundtruth type
-        _type = ocr_data.get_type_groundtruth()
-        if _type:
-            gt_type = _type
-
-        # optional filter frame
-        if coords:
-            (coords_start, coords_end) = coords
-            lines = ocr_data.filter_all(coords_start, coords_end)
-        else:
-            lines = ocr_data.get_lines()
-
-        if oneliner:
-            return (gt_type, ' '.join([c.get_text() for c in lines]), len(lines))
-        else:
-            return (gt_type, lines, len(lines))
-    except xml.parsers.expat.ExpatError as _:
-        with open(file_path, mode='r', encoding='utf-8') as fhandle:
-            text_lines = fhandle.readlines()
-            if oneliner:
-                text_lines = ' '.join([l.strip() for l in text_lines])
-            return (gt_type, text_lines, len(text_lines))
-    except RuntimeError as exc:
-        raise RuntimeError(f"{file_path}: {exc}") from exc
-
-
-def piece_to_text(file_path, frame=None, oneliner=True) -> Tuple:
-    '''Wrap OCR-Data Comparison'''
-
-    _gt_type = NOT_SET
-    try:
-        top_piece = to_pieces(file_path)
-        # optional groundtruth type
-        _gt_type = _get_groundtruth_from_filename(file_path)
-        if not _gt_type:
-            _level = top_piece.subject
-            if _level:
-                _gt_type = _level
-        # explicit filter frame?
-        if not frame:
-            frame = top_piece.dimensions
-        elif len(frame) == 2:
-            frame = [[frame[0][0], frame[0][1]],
-                     [frame[1][0], frame[0][1]],
-                     [frame[1][0], frame[1][1]],
-                     [frame[0][0], frame[1][1]]]
-        frame_piece = Piece()
-        frame_piece.dimensions = frame
-        filter_word_pieces(frame_piece, top_piece)
-        the_lines = [l
-                     for r in top_piece.pieces
-                     for l in r.pieces
-                     if l.transcription and l.level == PieceLevel.LINE]
-        if oneliner:
-            return (_gt_type, top_piece.transcription, len(the_lines))
-        else:
-            return (_gt_type, [l.transcription for l in the_lines], len(the_lines))
-    except xml.parsers.expat.ExpatError as _:
-        with open(file_path, mode='r', encoding='utf-8') as fhandle:
-            text_lines = fhandle.readlines()
-            if oneliner:
-                text_lines = ' '.join([l.strip() for l in text_lines])
-            return (_gt_type, text_lines, len(text_lines))
-    except RuntimeError as exc:
-        raise RuntimeError(f"{file_path}: {exc}") from exc
-
-
-def _get_groundtruth_from_filename(file_path):
+def _get_groundtruth_from_filename(file_path) -> str:
     _file_name = os.path.basename(file_path)
     result = re.match(r'.*gt.(\w{3,}).xml$', _file_name)
     if result:
         return result[1]
     else:
         alternative = re.match(r'.*\.(\w{3,})\.gt\.xml$', _file_name)
         if alternative:
             return alternative[1]
-
-
-def filter_word_pieces(frame, current) -> int:
-    _filtered = 0
-    _tmp_stack = []
-    _total_stack = []
-    # stack all items
-    _total_stack.append(current)
-    _tmp_stack.append(current)
-    while _tmp_stack:
-        _current = _tmp_stack.pop()
-        if _current.pieces:
-            _tmp_stack += _current.pieces
-            _total_stack += _current.pieces
-    # now pick words
-    _words = [_p for _p in _total_stack if _p.level == PieceLevel.WORD]
-
-    # check for each word piece
-    for _word in _words:
-        if _word not in frame:
-            _filtered += 1
-            _uplete(_word)
-    return _filtered
-
-
-def _uplete(curr):
-    if len(curr.pieces) == 0:
-        _pa = curr.parent
-        _pa.remove_pieces(curr)
-        _uplete(_pa)
+        else:
+            return NOT_SET
 
 
 def _normalize_gt_type(label) -> str:
     if label.startswith('art'):
         return 'article'
     elif label.startswith('ann'):
         return 'announcement'
@@ -478,39 +354,45 @@
         _accs = [1, 3]
         _raws = []
         _pre_v = None
         for i, m in enumerate(self.metrics):
             _val = m.value
             _ref = m.n_ref
             if _ref > 10000:
-                _ref_fmt = f'{(floor(float(m.n_ref) / 1000)):>2}K+'
+                _ref_fmt = f'{(math.floor(float(m.n_ref) / 1000)):>2}K+'
             else:
                 _ref_fmt = f'{m.n_ref:>4}'
             _raw = f'{m.label}:{_val:>5.2f}({_ref_fmt})'
             if i in _pres:
                 _pre_v = _val
             if i in _accs and _pre_v is not None:
                 diff = round(_val, 3) - round(_pre_v, 3)
                 _raw += f'(+{diff:>5.2f})' if diff > 0 else f'(-{abs(diff):>5.2f})'
                 _pre_v = None
             _raws.append(_raw)
         return ', '.join(_raws)
 
     def __repr__(self) -> str:
-        return '{} {}'.format(self.gt_type, self.path_c)
+        return f'{self.gt_type} {self.path_c}'
 
 
 class Evaluator:
     """Wrapper for Evaluation given candidates versus reference data
 
     Raises:
         RuntimeError: if candidates or reference data missing
     """
 
-    def __init__(self, root_candidates, verbosity=0, extras=None, to_text_func=piece_to_text):
+    def __init__(
+            self,
+            root_candidates,
+            verbosity=0,
+            extras=None,
+
+    ):
         """initiate new Evaluator
 
         Args:
             root_candidates (string|Path): Root domain/path to search for candidates
             verbosity (int, optional): Level of verbosity Defaults to 0.
             extras (_type_, optional): Implementation dependend. Defaults to None.
         """
@@ -518,34 +400,33 @@
         self.domain_reference = None
         self.evaluation_entries = []
         self.verbosity = verbosity
         self.evaluation_data = {}
         self.evaluation_results = []
         self.evaluation_map = {}
         self.text_mode = extras == EVAL_EXTRA_IGNORE_GEOMETRY
-        self.to_text_func = to_text_func
         self.is_sequential = False
-        self.metrics = []
+        self.metrics: typing.List[digem.SimilarityMetric] = []
         self.evaluation_report = {}
 
-    def eval_all(self, entries: List[EvalEntry], sequential=False) -> None:
+    def eval_all(self, entries: typing.List[EvalEntry], sequential=False) -> None:
         """evaluate all pairs groundtruth-candidate"""
 
         _entries = []
         if sequential or self.is_sequential:
             _entries = [self._wrap_eval_entry(e) for e in entries]
         else:
-            cpus = cpu_count()
-            n_executors = cpus - 1 if cpus > 3 else 1
+            cpus = multiprocessing.cpu_count()
+            n_executors = cpus // 2 if cpus > 3 else 1
             if self.verbosity == 1:
                 print(f"[DEBUG] use {n_executors} executors ({cpus}) to create evaluation data")
-
             with concurrent.futures.ProcessPoolExecutor(max_workers=n_executors) as executor:
                 try:
-                    _entries = list(executor.map(self._wrap_eval_entry, entries, timeout=EVAL_TIMEOUT))
+                    _entries = list(
+                        executor.map(self._wrap_eval_entry, entries, timeout=EVAL_TIMEOUT))
                 except concurrent.futures.TimeoutError:
                     print(f"[ERROR] takes longer than {EVAL_TIMEOUT}s to evaluate {len(entries)} entries!")
                     sys.exit(1)
                 except Exception as err:
                     print(f"[ERROR] '{err}' creating evaluation data!")
                     sys.exit(1)
 
@@ -571,59 +452,68 @@
             except Exception as exc:
                 print(f"[WARN ][{entry.path_g}] _wrap {exc}")
 
     def eval_entry(self, entry: EvalEntry) -> EvalEntry:
         """Create evaluation entry for matching pair of 
         groundtruth and candidate data"""
 
-        path_g = entry.path_g
-        path_c = entry.path_c
-
-        # read coordinate information (if any provided)
-        # to create frame for candidate data
-        coords = get_bbox_data(path_g)
-        if coords is not None and self.verbosity >= 2:
-            print(f"[TRACE] token coordinates {coords[0]}, {coords[1]}")
-
-        # load ground-thruth text
-        (gt_type, txt_gt, _) = self.to_text_func(path_g, oneliner=True)
-        if not txt_gt:
-            print(f"[WARN ] {path_g} contains no text")
-
-        # if text mode is enforced
-        # forget groundtruth coordinates
-        coords = None if self.text_mode else coords
-
-        # read candidate data as text
-        (_, txt_c, _) = self.to_text_func(path_c, coords, oneliner=True)
-        if self.verbosity >= 2:
-            _label_ref = os.path.basename(path_g)
-            _label_can = os.path.basename(path_c)
-            print(f'[TRACE][{_label_ref}] RAW GROUNDTRUTH :: "{txt_gt}"')
-            print(f'[TRACE][{_label_can}] RAW CANDIDATE   :: "{txt_c}"')
-
         # evaluate metric copies
         _current_metrics = []
+
         for _m in self.metrics:
+
+            path_g = entry.path_g
+            path_c = entry.path_c
+
+            # read coordinate information (if any provided)
+            # to create frame for candidate data
+            coords = get_bbox_data(path_g)
+            if coords is not None and self.verbosity >= 2:
+                print(f"[TRACE] token coordinates {coords[0]}, {coords[1]}")
+
+            to_text_func = _m.to_text_func
+
+            # load ground-thruth text
+            (txt_gt, _) = to_text_func(path_g, oneliner=True)
+
+            if not txt_gt:
+                print(f"[WARN ] groundtrooth '{path_g}' contains no text")
+
+            # if text mode is enforced
+            # forget groundtruth coordinates
+            coords = None if self.text_mode else coords
+
+            # read candidate data as text
+            (txt_c, _) = to_text_func(path_c, coords, oneliner=True)
+
+            if not txt_c:
+                print(f"[WARN ] candidate '{path_c}' contains no text")
+
+            if self.verbosity >= 2:
+                _label_ref = os.path.basename(path_g)
+                _label_can = os.path.basename(path_c)
+                print(f'[TRACE][{_label_ref}] RAW GROUNDTRUTH :: "{txt_gt}"')
+                print(f'[TRACE][{_label_can}] RAW CANDIDATE   :: "{txt_c}"')
+
             _curr = copy.copy(_m)
             _curr.reference = txt_gt
             _curr.candidate = txt_c
-            # ATTENZIONE! inital access to this attribute 
+            # ATTENZIONE! inital access to this attribute
             # triggers preprocessing and calculation!
             _curr.value
             _current_metrics.append(_curr)
             if self.verbosity >= 2:
                 _label_ref = os.path.basename(path_g)
                 _label_can = os.path.basename(path_c)
                 print(f'[TRACE][{_label_ref}][{_curr.label}] REFERENCE :: "{_curr._data_reference}"')
                 print(f'[TRACE][{_label_can}][{_curr.label}] CANDIDATE :: "{_curr._data_candidate}"')
 
         # enrich entry with metrics and
         # normalize data type (i.e., art or ann or ...)
-        _normed_gt_type = _normalize_gt_type(str(gt_type))
+        _normed_gt_type = _normalize_gt_type(_get_groundtruth_from_filename(entry.path_g))
         entry.gt_type = _normed_gt_type
         entry.metrics = _current_metrics
         return entry
 
     def _generate_report_candidate(self, the_entry):
         try:
             image_name = os.path.basename(the_entry.path_c)
@@ -650,15 +540,15 @@
             # set initial result level values
             evaluation_result = EvaluationResult(k, n_total, n_chars=n_chars)
             evaluation_result.mean = data_points[0]
             evaluation_result.median = data_points[0]
 
             # if more than one single evaluation item
             # calculate additional statistics to reflect
-            # impact of outlying data sets 
+            # impact of outlying data sets
             # take CA and number of GT into account
             # also calculate statistics (mean, std)
             if len(data_points) > 1:
                 (mean, std, median) = get_statistics(data_points)
                 evaluation_result.mean = mean
                 evaluation_result.median = median
                 evaluation_result.std = std
@@ -673,31 +563,35 @@
                     clear_result.n_chars = sum([e[2] for e in regulars])
                     # set as child component
                     evaluation_result.cleared_result = clear_result
             self._add(evaluation_result)
             # re-order
             self.evaluation_results = sorted(self.evaluation_results, key=lambda e: e.eval_key)
 
-    def aggregate(self, by_type=False, by_metrics=[0, 1, 2, 3]):
+    def aggregate(self, by_type=False, by_metrics=None):
+        """Aggregate item's metrics for domain/directory
+        and/or annotated type (if present)"""
 
         # precheck - having root dir
         self._check_aggregate_preconditions()
+        if by_metrics is None:
+            by_metrics = [0, 1, 2, 3]
 
         root_base = Path(self.domain_reference).parts[-1]
 
         # aggregate on each directory
         for _metrics_index in by_metrics:
             for ee in self.evaluation_entries:
-                # if we do not have all these different metrics set, 
+                # if we do not have all these different metrics set,
                 # do of course not aggregate by non-existing index!
                 if _metrics_index >= len(self.evaluation_entries[0].metrics):
                     continue
                 path_key = f"{ee.metrics[_metrics_index].label}@{root_base}"
                 # ATTENZIONE! works only when forehand
-                # the *real* attribute has been accessed 
+                # the *real* attribute has been accessed
                 # *at least one time*
                 # kept this way for testing reasons
                 metric_value = ee.metrics[_metrics_index].value
                 metric_gt_refs = ee.metrics[_metrics_index].n_ref
                 dir_o = os.path.dirname(ee.path_c)
                 ocr_parts = Path(dir_o).parts
                 if root_base in ocr_parts:
@@ -739,20 +633,20 @@
     if verbosity >= 1:
         if 'candidates' in evaluator.evaluation_report:
             for _c in evaluator.evaluation_report['candidates']:
                 print(f'[DEBUG] {_c}')
     results = evaluator.get_results()
     _path_can = evaluator.domain_candidate
     _path_ref = evaluator.domain_reference
-    evaluation_date = date.today().isoformat()
+    evaluation_date = datetime.date.today().isoformat()
     print(f'[INFO ] Evaluation Summary (candidates: "{_path_can}" vs. reference: "{_path_ref}" ({evaluation_date})')
     for result in results:
         (gt_type, n_total, mean_total, med, _n_refs) = result.get_defaults()
-        add_stats = f', std: {result.std:.2f}, median: {med:.2f}' if n_total > 1 else ''
-        print(f'[INFO ] "{gt_type}"\t∅: {mean_total:.2f}\t{n_total} items, {_n_refs} refs{add_stats}')
+        add_stats = f', std: {result.std:5.2f}, median: {med:5.2f}' if n_total > 1 else ''
+        print(f'[INFO ] "{gt_type}"\t∅: {mean_total:5.2f}\t{n_total: 3d} items, {_n_refs:_} refs{add_stats}')
         if result.cleared_result:
             (_, n_t2, mean2, med2, n_c2) = result.cleared_result.get_defaults()
             ccr_std = result.cleared_result.std
             drops = n_total - n_t2
             if drops > 0:
                 print(
-                    f'[INFO ] "{gt_type}"\t∅: {mean2:.2f}\t{n_t2} items (-{drops}), {n_c2} refs, std: {ccr_std:.2f}, median: {med2:.2f}')
+                    f'[INFO ] "{gt_type}(-{drops})"\t∅: {mean2:5.2f}\t{n_t2: 3d} items, {n_c2:_} refs, std: {ccr_std:5.2f}, median: {med2:5.2f}')
```

### Comparing `digital-eval-1.5.3/src/digital_eval/metrics.py` & `digital_eval-1.6.0/src/digital_eval/metrics.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,44 @@
 # -*- coding: utf-8 -*-
 """Metrics Module"""
 
 from __future__ import annotations
 
-from collections import (
-    Counter
-)
-from functools import partial
-
+import collections
+import functools
 import string
-
-from typing import (
-    List,
-    Set, Callable,
-)
-
+import typing
 import unicodedata
+import xml.dom.minidom
 
-from nltk import (
-    download,
-)
-from nltk.corpus import (
-    stopwords
-)
-from nltk.metrics import (
-    recall,
-    f_measure
-)
+import nltk
+import nltk.corpus as nltk_corp
 from nltk.metrics import precision as nltk_precision
+from nltk.metrics import (
+     recall,
+     f_measure
+ )
+import rapidfuzz.distance.Levenshtein as rfls
+
+import digital_object as do
 
-from rapidfuzz.distance import (
-    Levenshtein
-)
+from digital_eval.dictionary_metrics.common import LANGUAGE_KEY_DEFAULT
+from digital_eval.dictionary_metrics.language_tool.LanguageTool import LanguageTool
 
 # Python3 standard Unicode Normalization
 #
 UC_NORMALIZATION_DEFAULT = 'NFC'
 UC_NORMALIZATION_NFKD = 'NFKD'
 
 # whitespaces
 #
 # usual spatium and special control sequences
 WHITESPACES = string.whitespace
 
-WHITESPACES_EXCLUDING_BLANK_CHARS = WHITESPACES[1:]
+WHITESPACES_EXCL_BLANK_CHARS = WHITESPACES[1:]
 
 # punctuations
 #
 #   * regular ASCII-punctuations
 #   * Dashes        \u2012-2017
 #   * Quotations    \u2018-201F
 PUNCTUATIONS = string.punctuation + '\u2012' + '\u2013' + '\u2014' + '\u2015' + '\u2016' + \
@@ -71,41 +62,41 @@
 # persian indic digits
 DIGITS = DIGITS + '\u06f0' + '\u06f1' + '\u06f2' + '\u06f3' + \
          '\u06f4' + '\u06f5' + '\u06f6' + '\u06f7' + '\u06f8' + '\u06f9'
 
 # filter mechanics
 #
 # via Python3 string translation maps
-WHITESPACE_TRANSLATOR = str.maketrans('', '', WHITESPACES)
-WHITESPACE_EXCLUDING_BLANK_CHARS_TRANSLATOR = str.maketrans('', '', WHITESPACES_EXCLUDING_BLANK_CHARS)
-PUNCT_TRANLATOR = str.maketrans('', '', PUNCTUATIONS)
-DIGIT_TRANSLATOR = str.maketrans('', '', DIGITS)
+WHITESPACE_TRNSL = str.maketrans('', '', WHITESPACES)
+WHITESPACE_EXCL_BLANK_CHARS_TRNSL = str.maketrans('', '', WHITESPACES_EXCL_BLANK_CHARS)
+PUNCT_TRNSL = str.maketrans('', '', PUNCTUATIONS)
+DIGIT_TRNSL = str.maketrans('', '', DIGITS)
 
 
 def _filter_whitespaces(a_str) -> str:
-    return a_str.translate(WHITESPACE_TRANSLATOR)
+    return a_str.translate(WHITESPACE_TRNSL)
 
 
 def _filter_whitespaces_excluding_blank_chars(a_str) -> str:
-    return a_str.translate(WHITESPACE_EXCLUDING_BLANK_CHARS_TRANSLATOR)
+    return a_str.translate(WHITESPACE_EXCL_BLANK_CHARS_TRNSL)
 
 
 def _filter_puncts(a_str) -> str:
-    return a_str.translate(PUNCT_TRANLATOR)
+    return a_str.translate(PUNCT_TRNSL)
 
 
 def _filter_digits(a_str) -> str:
-    return a_str.translate(DIGIT_TRANSLATOR)
+    return a_str.translate(DIGIT_TRNSL)
 
 
-def _tokenize(a_str) -> List[str]:
+def _tokenize(a_str) -> typing.List[str]:
     return a_str.split() if isinstance(a_str, str) else a_str
 
 
-def _tokenize_to_sorted_set(a_str) -> Set[str]:
+def _tokenize_to_sorted_set(a_str) -> typing.Set[str]:
     return set(sorted(_tokenize(a_str)))
 
 
 #
 # information retrieval (nltk)
 #
 NLTK_STOPWORDS = [
@@ -116,39 +107,41 @@
     'greek',
     'arabic',
     'turkish',
     'italian']
 STOPWORDS_DEFAULT = ['german', 'english', 'arabic', 'russian']
 
 
-def get_stopwords(nltk_mappings=NLTK_STOPWORDS, languages=None) -> Set[str]:
+def get_stopwords(nltk_mappings=None, languages=None) -> typing.Set[str]:
     """Helper Function to gather NLTK stopword data
     * ensure stopwords files are locally available
     * extract them as set
     """
+    if nltk_mappings is None:
+        nltk_mappings = NLTK_STOPWORDS
     try:
         for mapping in nltk_mappings:
-            stopwords.words(mapping)
+            nltk_corp.stopwords.words(mapping)
     except LookupError:
-        download('stopwords')
+        nltk.download('stopwords')
     if languages is None:
         languages = STOPWORDS_DEFAULT
     _stopwords = {_all_words
                   for _lang in languages
-                  for _all_words in stopwords.words(_lang)
+                  for _all_words in nltk_corp.stopwords.words(_lang)
                   }
     return _stopwords
 
 
 def _strip_languages_stopwords(tokens, languages):
     return tokens - get_stopwords(languages=languages)
 
 
 def _strip_stopwords_for(languages):
-    return partial(_strip_languages_stopwords, languages=languages)
+    return functools.partial(_strip_languages_stopwords, languages=languages)
 
 
 def normalize_unicode(input_str: str, uc_norm_by=UC_NORMALIZATION_DEFAULT) -> str:
     """Apply basic unicode normalization
     """
 
     if uc_norm_by is not None:
@@ -162,171 +155,201 @@
     punct_translator = str.maketrans('', '', PUNCTUATIONS)
     digit_translator = str.maketrans('', '', DIGITS)
     the_content = the_content.translate(punct_translator)
     the_content = the_content.translate(digit_translator)
     return the_content
 
 
-class DigitalEvalMetricException(Exception):
-    """Mark Exception during validation/calculating metrics"""
+def digital_object_to_dict_text(file_path: str, frame=None, oneliner=False) -> typing.Tuple:
+    line_texts: typing.List[str]
+    len_lines: int
+    line_texts, len_lines = digital_object_to_text(file_path=file_path, frame=frame, oneliner=False)
+    non_empty_lines: typing.List[str] = [line_text for line_text in line_texts if len(line_text) > 0]
+    lines_sanitized_wraps: typing.List[str] = _sanitize_wraps(non_empty_lines)
+    lines_sanitized_chars: typing.List[str] = _sanitize_chars(lines_sanitized_wraps)
+    text = ' '.join(lines_sanitized_chars) if oneliner else lines_sanitized_chars
+    return text, len_lines
 
-    def __init__(self, *args: object) -> None:
-        super().__init__(*args)
 
+def digital_object_to_text(file_path, frame=None, oneliner=True) -> typing.Tuple:
+    """Wrap OCR-Data Comparison"""
 
-def _inspect_calculation_object(an_object):
-    if not isinstance(an_object, OCRDifferenceMetric):
-        _msg = f"{an_object} is no instance of {OCRDifferenceMetric}!"
-        raise DigitalEvalMetricException(_msg)
     try:
-        _diff = an_object.diff
-        _ref = an_object.n_ref
-        if _diff is None or _diff < 0:
-            raise DigitalEvalMetricException(f"invalid diff: {_diff}!")
-        if _ref is None or _ref < 0:
-            raise DigitalEvalMetricException(f"invalid ref: {_ref}!")
-    except AttributeError as _ae:
-        raise DigitalEvalMetricException(_ae.args[0]) from _ae
-
-
-def accuracy_for(metric_obj: OCRDifferenceMetric) -> float:
-    """Calculate accuracy as ratio of
-    correct items, with correct items
-    being expected items minus
-    number of differences.
-
-    Respect following corner cases:
-    * if less correct items than differences => 0
-    * if both correct items and differences eq zero => 1
-      means: nothing to find and it did detect nothing
-      (i.e. no false-positives)
-
-    Args:
-        metric_obj (OCRDifferenceMetric): object containing information
-        about reference data and difference
-
-    Returns:
-        float: accuracy in range 0.0 - 1.0
-    """
-
-    _inspect_calculation_object(metric_obj)
-    diffs = metric_obj.diff
-    n_refs = len(metric_obj._data_reference)
-    return _calculate(lambda d, n: (n - d) / n, diffs, n_refs)
-
-
-def error_for_bow(metric_obj: OCRDifferenceMetric) -> float:
-    _inspect_calculation_object(metric_obj)
-    diffs = metric_obj.diff
-    n_refs = len(metric_obj._data_reference) + len(metric_obj._data_candidate)
-    return _calculate(lambda d, n: d / n, diffs, n_refs)
-
-
-def accuracy_for_bow(metric_obj: OCRDifferenceMetric) -> float:
-    _inspect_calculation_object(metric_obj)
-    diffs = metric_obj.diff
-    n_refs = len(metric_obj._data_reference) + len(metric_obj._data_candidate)
-    return _calculate(lambda d, n: 1 - (d / n), diffs, n_refs)
-
-
-def error_for(metric_obj: OCRDifferenceMetric) -> float:
-    """Calculate error as ratio of
-    difference and number of
-    expected items.
-
-    Respect following corner cases:
-    * if less expected items than differences => 0
-    * if both expected items and differences eq zero => 1
-      means: nothing to find and detected nothing
-      (i.e. no false-positives)
-
-    Args:
-        metric_obj (OCRDifferenceMetric): object containing information
-        about reference data and difference
-
-    Returns:
-        float: error in range 0.0 - 1.0
+        top_digo: do.DigitalObjectTree = do.to_digital_object(file_path)
+        # explicit filter frame?
+        if not frame:
+            frame = top_digo.dimensions
+        elif len(frame) == 2:
+            frame = [[frame[0][0], frame[0][1]],
+                     [frame[1][0], frame[0][1]],
+                     [frame[1][0], frame[1][1]],
+                     [frame[0][0], frame[1][1]]]
+        frame_digo = do.DigitalObjectTree()
+        frame_digo.dimensions = frame
+        filter_word_pieces(frame_digo, top_digo)
+        the_lines = _get_line_digos_from_digo(top_digo)
+        if oneliner:
+            return top_digo.transcription, len(the_lines)
+        else:
+            return [line.transcription for line in the_lines], len(the_lines)
+    except xml.parsers.expat.ExpatError as _:
+        with open(file_path, mode='r', encoding='utf-8') as fhandle:
+            text_lines = fhandle.readlines()
+            if oneliner:
+                text_lines = ' '.join([l.strip() for l in text_lines])
+            return text_lines, len(text_lines)
+    except RuntimeError as exc:
+        raise RuntimeError(f"{file_path}: {exc}") from exc
+
+
+def filter_word_pieces(frame, current) -> int:
+    _filtered = 0
+    _tmp_stack = []
+    _total_stack = []
+    # stack all items
+    _total_stack.append(current)
+    _tmp_stack.append(current)
+    while _tmp_stack:
+        _current: do.DigitalObjectTree = _tmp_stack.pop()
+        if _current.children:
+            _tmp_stack += _current.children
+            _total_stack += _current.children
+    # now pick words
+    _words = [_p for _p in _total_stack if _p.level == do.DigitalObjectLevel.WORD]
+
+    # check for each word piece
+    for _word in _words:
+        if _word not in frame:
+            _filtered += 1
+            _uplete(_word)
+    return _filtered
+
+
+def _uplete(curr: do.DigitalObjectTree):
+    if len(curr.children) == 0 and curr.level < do.DigitalObjectLevel.PAGE:
+        _pa: do.DigitalObjectTree = curr.parent
+        _pa.remove_children(curr)
+        _uplete(_pa)
+
+
+def _get_line_digos_from_digo(digo: do.DigitalObjectTree, lines: typing.List = None) -> typing.List[do.DigitalObjectTree]:
+    if lines is None:
+        lines = []
+    if digo.level == do.DigitalObjectLevel.LINE and digo.transcription:
+        lines.append(digo)
+        return lines
+    for child in digo.children:
+        _get_line_digos_from_digo(child, lines)
+    return lines
+
+
+_HYPHENS: typing.List[str] = [
+    "⸗",
+    "-",
+    "—",
+]
+
+
+def _sanitize_wraps(lines: typing.List[str]) -> typing.List[str]:
+    """Sanitize word wraps if
+    * last word token ends with '-', "⸗" or "—"
+    * another line following
+    * following line not empty
     """
-    _inspect_calculation_object(metric_obj)
-    diffs = metric_obj.diff
-    n_refs = len(metric_obj._data_reference)
-    return _calculate(lambda d, n: d / n, diffs, n_refs)
-
 
-def _calculate(calculate: Callable[[int, int], float], diffs: int, n_refs: int) -> float:
-    if (n_refs - diffs) < 0:
-        return 0.0
-    if n_refs == 0 and diffs == 0:
-        return 1.0
-    elif n_refs > 0:
-        return calculate(diffs, n_refs)
-    else:
-        return 0.0
+    normalized_lines: typing.List[str] = []
+    for i, line in enumerate(lines):
+        if i < len(lines) - 1:
+            for hyphen in _HYPHENS:
+                if line.endswith(hyphen):
+                    next_line = lines[i + 1]
+                    if len(next_line.strip()) == 0:
+                        # encountered empty next line, no merge possible
+                        continue
+                    next_line_tokens = next_line.split()
+                    nextline_first_token = next_line_tokens.pop(0)
+                    # join the rest of valid next line
+                    lines[i + 1] = ' '.join(next_line_tokens)
+                    line = line[:-1] + nextline_first_token
+                    break
+        normalized_lines.append(line)
+    return normalized_lines
+
+
+def _sanitize_chars(lines: typing.List[str]) -> typing.List[str]:
+    """Replace or remove nonrelevant chars for current german word error rate"""
+
+    sanitized: typing.List[str] = []
+    for line in lines:
+        text = line.strip()
+        bad_chars = '0123456789“„"\'?!*.;:-=[]()|'
+        text = ''.join([c for c in text if c not in bad_chars])
+        if '..' in text:
+            text = text.replace('..', '')
+        if '  ' in text:
+            text = text.replace('  ', ' ')
+        text = ' '.join([t for t in text.split() if len(t) > 1])
+        sanitized.append(text)
 
+    return sanitized
 
-def norm_to_scale(value, scale_by) -> float:
-    """Normalize outcome in range 0 - scale_by"""
-    return value * scale_by
 
+class DigitalEvalMetricException(Exception):
+    """Mark Exception during validation/calculating metrics"""
 
-def norm_percentual(value):
-    """Normalize value in between 0 - 100"""
-    return partial(norm_to_scale, scale_by=100)(value)
+    def __init__(self, *args: object) -> None:
+        super().__init__(*args)
 
 
-class OCRDifferenceMetric:
-    """Basic definition of a OCRDifferenceMetric"""
+class SimilarityMetric:
+    """Basic definition of OCR Similarity Metric,
+    expressed in percent (0 - 100)
+    """
 
     def __init__(
             self,
             precision=2,
             normalization=UC_NORMALIZATION_DEFAULT,
-            calc_func=accuracy_for,
             preprocessings=None,
-            postprocessings=None
+            to_text_func=digital_object_to_text,
     ) -> None:
+        self.to_text_func: typing.Optional[typing.Callable] = to_text_func
         self.precision = precision
         self._value = None
-        self.diff = None
         self._label = None
         self.unicode_normalization = normalization
         self.preprocessings = []
         if isinstance(preprocessings, list):
             self.preprocessings = preprocessings
-        self.calc_func = calc_func
-        self.postprocessings = [norm_percentual]
-        if isinstance(postprocessings, list):
-            self.postprocessings = postprocessings
         self.input_reference = None
         self.input_candidate = None
         self._data_reference = None
         self._data_candidate = None
         self.languages = None
 
     @property
     def reference(self):
         """Reference/Groundtruth data"""
         return self._data_reference
 
     @reference.setter
     def reference(self, value):
         self.input_reference = value
-        self._data_reference = normalize_unicode(
-            value, self.unicode_normalization)
+        self._data_reference = normalize_unicode(value, self.unicode_normalization)
         self._value = None
 
     @property
     def candidate(self):
         """Candidate data"""
         return self._data_candidate
 
     @candidate.setter
     def candidate(self, value):
         self.input_candidate = value
-        self._data_candidate = normalize_unicode(value)
+        self._data_candidate = normalize_unicode(value, self.unicode_normalization)
         self._value = None
 
     @property
     def label(self):
         """Metric's label"""
         return self._label
 
@@ -344,220 +367,227 @@
 
         self._data_reference = 't' * value
 
     @property
     def value(self):
         """Evaluate each time and round
         with desired precision afterwards"""
-
         if self._value is None:
             if self.preprocessings:
                 for _pre in self.preprocessings:
                     self._data_reference = _pre(self._data_reference)
                     self._data_candidate = _pre(self._data_candidate)
             self._forward()
-            if self.calc_func:
-                self._value = self.calc_func(self)
-            else:
-                self._value = self.diff
-            if self.postprocessings:
-                for _post in self.postprocessings:
-                    self._value = _post(self._value)
+            self._value *= 100
         return round(self._value, self.precision)
 
     def _forward(self):
-        """Calculate metric's value
-        remember this needs further refinement"""
-        raise NotImplementedError
+        self._value = levenshtein_norm(self._data_reference, self._data_candidate)
 
 
-class MetricChars(OCRDifferenceMetric):
+class MetricChars(SimilarityMetric):
     """Calculate plain sequent character based metric"""
 
-    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT, calc_func=accuracy_for,
-                 preprocessings=None, postprocessings=None):
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT,
+                 preprocessings=None):
         super().__init__(
             precision,
             normalization,
-            calc_func,
-            preprocessings,
-            postprocessings)
+            preprocessings)
         self._label = 'Cs'
         self.name = 'Characters'
         self.preprocessings = [_filter_whitespaces_excluding_blank_chars]
-        self.postprocessings = [norm_percentual]
-
-    def _forward(self):
-        self.diff = edit_distance(self._data_reference, self._data_candidate)
 
 
-class MetricLetters(OCRDifferenceMetric):
+class MetricLetters(SimilarityMetric):
     """Calculate metric for only a certain sub-set of
     character sequence"""
 
-    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT, calc_func=accuracy_for,
-                 preprocessings=None, postprocessings=None):
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT,
+                 preprocessings=None):
         super().__init__(
             precision,
             normalization,
-            calc_func,
-            preprocessings,
-            postprocessings)
+            preprocessings)
         self._label = 'Ls'
         self.preprocessings = [
             _filter_whitespaces,
             _filter_puncts,
             _filter_digits]
 
-    def _forward(self):
-        self.diff = edit_distance(self._data_reference, self._data_candidate)
-
 
-class MetricWords(OCRDifferenceMetric):
+class MetricWords(SimilarityMetric):
     """Calculate metric for a sequence of word tokens"""
 
-    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT, calc_func=accuracy_for,
-                 preprocessings=None, postprocessings=None):
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT,
+                 preprocessings=None):
         super().__init__(
             precision,
             normalization,
-            calc_func,
-            preprocessings,
-            postprocessings)
+            preprocessings)
         self._label = 'Ws'
         self.preprocessings = [_tokenize]
 
+
+class MetricDictionary(SimilarityMetric):
+    """Calculate metric for a multiset of word tokens"""
+
+    LANGUAGE: str = LANGUAGE_KEY_DEFAULT
+
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT,
+                 preprocessings=None, to_text_func=digital_object_to_dict_text):
+        super().__init__(
+            precision=precision,
+            normalization=normalization,
+            preprocessings=preprocessings,
+            to_text_func=to_text_func,
+        )
+
+
+class MetricDictionaryLangTool(MetricDictionary):
+    """Calculate metric for a multiset of word tokens"""
+
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_NFKD,
+                 preprocessings=None):
+        if not isinstance(preprocessings, list):
+            preprocessings = [_normalize_vocal_ligatures]
+        super().__init__(
+            precision=precision,
+            normalization=normalization,
+            preprocessings=preprocessings,
+        )
+        self._label = 'DictLT'
+        self.diff = 0
+
     def _forward(self):
-        self.diff = edit_distance(self._data_reference, self._data_candidate)
+        text: str = self._data_candidate
+        text_list: typing.List[str] = self._data_candidate.split()
+        self._data_reference = text_list
+        num_words: int = len(text_list)
+        lt_response_data: typing.Dict = LanguageTool.check(text, MetricDictionary.LANGUAGE)
+        total_matches = lt_response_data['matches'] if 'matches' in lt_response_data else 0
+        typo_errors = len(total_matches)
+        self.diff = typo_errors if typo_errors <= num_words else num_words
 
 
-class MetricBoW(OCRDifferenceMetric):
+class MetricBoW(SimilarityMetric):
     """Calculate metric for a multiset of word tokens"""
 
-    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT, calc_func=accuracy_for,
-                 preprocessings=None, postprocessings=None):
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT,
+                 preprocessings=None):
         super().__init__(
             precision,
             normalization,
-            calc_func,
-            preprocessings,
-            postprocessings)
+            preprocessings)
         self._label = 'BoWs'
         self.preprocessings = [_tokenize]
 
     def _forward(self):
-        self.diff = bag_of_tokens(self._data_reference, self._data_candidate)
+        self._value = bag_of_tokens(self._data_reference, self._data_candidate)
 
 
-class MetricIR(OCRDifferenceMetric):
+class MetricIR(SimilarityMetric):
     """Calculate information retrival metrics"""
 
-    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT, calc_func=accuracy_for,
-                 preprocessings=None, postprocessings=None, languages=None):
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT,
+                 preprocessings=None, languages=None):
         super().__init__(
             precision,
             normalization,
-            calc_func,
-            preprocessings,
-            postprocessings)
+            preprocessings)
         self.languages = languages
         self.preprocessings = [_tokenize_to_sorted_set,
                                _strip_stopwords_for(self.languages)
                                ]
         # no aligning required, we rely on nltk
         self.calc_func = None
-        # no percentual value
-        self.postprocessings = []
 
     def _forward(self):
         """to remind that this class needs further refinement"""
         raise NotImplementedError
 
 
 class MetricIRPre(MetricIR):
     """Calculate precision"""
 
-    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT, calc_func=accuracy_for,
-                 preprocessings=None, postprocessings=None, languages=None):
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT,
+                 preprocessings=None, languages=None):
         super().__init__(
             precision,
             normalization,
-            calc_func,
             preprocessings,
-            postprocessings,
             languages)
         self._label = 'Pre'
 
     def _forward(self):
-        self.diff = ir_precision(self._data_reference, self._data_candidate)
+        self._value = ir_precision(self._data_reference, self._data_candidate)
 
 
 class MetricIRRec(MetricIR):
     "Calculate recall"
 
-    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT, calc_func=accuracy_for,
-                 preprocessings=None, postprocessings=None, languages=None):
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT,
+                 preprocessings=None, languages=None):
         super().__init__(
             precision,
             normalization,
-            calc_func,
             preprocessings,
-            postprocessings,
             languages)
         self._label = 'Rec'
 
     def _forward(self):
-        self.diff = ir_recall(self._data_reference, self._data_candidate)
+        self._value = ir_recall(self._data_reference, self._data_candidate)
 
 
 class MetricIRFM(MetricIR):
     """Calculate harmonic mean for precision/recall"""
 
-    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT, calc_func=accuracy_for,
-                 preprocessings=None, postprocessings=None, languages=None):
+    def __init__(self, precision=2, normalization=UC_NORMALIZATION_DEFAULT,
+                 preprocessings=None, languages=None):
         super().__init__(
             precision,
             normalization,
-            calc_func,
             preprocessings,
-            postprocessings,
             languages)
         self._label = 'FM'
 
     def _forward(self):
-        self.diff = ir_fmeasure(self._data_reference, self._data_candidate)
+        self._value = ir_fmeasure(self._data_reference, self._data_candidate)
 
 
-def edit_distance(reference_data, candidate_data) -> int:
-    """Calculate edit distance with levenshtein-distance.
-    as sum of edit operations required to get from
-    candidate to reference string / token_list
+def levenshtein_norm(reference_data, candidate_data, inverse=False) -> int:
+    """Calculate levenshtein metric as ration of sum of edit operations 
+    normalized to sum of edit and equal operations.
 
     Works with characters and word-like tokens, where
     tokens correspond also to:
     * abbreviations  (like "Nr." or "Etg.")
     * numbers/years  (like "1899")
     * split-up words (line endings/beginnings)
     """
+    if inverse:
+        return rfls.normalized_distance(reference_data, candidate_data)
+    return rfls.normalized_similarity(reference_data, candidate_data)
 
-    return Levenshtein.distance(reference_data, candidate_data)
 
-
-def bag_of_tokens(reference_tokens: List[str],
-                  candidate_tokens: List[str]) -> int:
-    """Calculate intersection/difference
-    between reference and candidate token list
+def bag_of_tokens(reference_tokens: typing.List[str],
+                  candidate_tokens: typing.List[str]) -> int:
+    """Calculate difference between reference and candidate token list
     """
-    false_negatives: List[str] = _diff(reference_tokens, candidate_tokens)
-    false_positives: List[str] = _diff(candidate_tokens, reference_tokens)
-    return len(false_negatives) + len(false_positives)
+    false_negatives: typing.List[str] = _diff(reference_tokens, candidate_tokens)
+    false_positives: typing.List[str] = _diff(candidate_tokens, reference_tokens)
+    delta = len(false_negatives) + len(false_positives)
+    total = len(reference_tokens) + len(candidate_tokens)
+    subtrahend = (delta / total) if total > 0 else 0
+    ratio = 1 - subtrahend
+    return ratio
 
 
-def _diff(gt_tokens, cd_tokens) -> List[str]:
-    return list((Counter(gt_tokens) - Counter(cd_tokens)).elements())
+def _diff(gt_tokens, cd_tokens) -> typing.List[str]:
+    return list((collections.Counter(gt_tokens) - collections.Counter(cd_tokens)).elements())
 
 
 def ir_precision(reference_data, candidate_data) -> float:
     """Calculate Precision for given languages"""
 
     _prec = nltk_precision(reference_data, candidate_data)
     # nltk actually handles this inconsistently ...
@@ -577,7 +607,40 @@
     """Calculate F-Measure for given languages"""
 
     _fm = f_measure(reference_data, candidate_data)
     # required since nltk actually handles this inconsistently ...
     if _fm is None:
         _fm = 0.0
     return _fm
+
+
+# diacritica to take care of
+_COMBINING_SMALL_E = '\u0364'
+
+def _normalize_vocal_ligatures(a_string) -> str:
+    """Replace vocal ligatures, which otherwise
+    may confuse the index component workflow,
+    especially COMBINING SMALL LETTER E : \u0364
+
+    a^e, o^e, u^e => (u0364) => ä, ö, ü
+    """
+
+    _out = []
+    for i, _c in enumerate(a_string):
+        if _c == _COMBINING_SMALL_E:
+            _preceeding_vocal = _out[i - 1]
+            _vocal_name = unicodedata.name(_preceeding_vocal)
+            _replacement = ''
+            if 'LETTER A' in _vocal_name:
+                _replacement = 'ä'
+            elif 'LETTER O' in _vocal_name:
+                _replacement = 'ö'
+            elif 'LETTER U' in _vocal_name:
+                _replacement = 'ü'
+            else:
+                _msg = f"No conversion for {_preceeding_vocal} ('{a_string}')!"
+                raise DigitalEvalMetricException(f"normalize vocal ligatures: {_msg}")
+            _out[i - 1] = _replacement
+        _out.append(_c)
+
+    # strip all combining e's anyway
+    return ''.join(_out).replace(_COMBINING_SMALL_E, '')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `digital-eval-1.5.3/src/digital_eval.egg-info/PKG-INFO` & `digital_eval-1.6.0/src/digital_eval.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 Metadata-Version: 2.1
 Name: digital-eval
-Version: 1.5.3
-Summary: Evaluate Mass Digitalization Data
-Author: Universitäts- und Landesbibliothek Sachsen-Anhalt
-Author-email: development@bibliothek.uni-halle.de
-Maintainer: Uwe Hartwig
-Maintainer-email: uwe.hartwig@bibliothek.uni-halle.de
+Version: 1.6.0
+Summary: Evaluate Digitalization Data
+Author-email: Universitäts- und Landesbibliothek Sachsen-Anhalt <development@bibliothek.uni-halle.de>
 Project-URL: Homepage, https://github.com/ulb-sachsen-anhalt/digital-eval
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: rapidfuzz>3
+Requires-Dist: nltk
+Requires-Dist: requests
+Requires-Dist: docker
+Requires-Dist: numpy
+Requires-Dist: digital-object==0.2.0
 
 # digital eval
 
 ![example workflow](https://github.com/ulb-sachsen-anhalt/digital-eval/actions/workflows/python-app.yml/badge.svg)
 [![PyPi version](https://badgen.net/pypi/v/digital-eval/)](https://pypi.org/project/digital-eval) ![PyPI - Downloads](https://img.shields.io/pypi/dm/digital-eval) ![PyPI - License](https://img.shields.io/pypi/l/digital-eval) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/digital-eval)
 
 Python3 Tool to report evaluation outcomes from mass digitalization workflows.
 
 ## Features
 
-* match automatically groundtruth (i.e. reference data) and candidates by filename
+* [OCR-D compliant](https://ocr-d.de/en/spec/ocrd_eval#character-error-rate-cer) normalized similarity for edit-distance based metrics based on characters, letters and words
+* choose from textual metrics based on characters or words plus common Information Retrieval
+* choose from different UTF-8 Python norms
+* match groundtruth (i.e. reference data) and candidates by filename start
 * use geometric information to evaluate only specific frame (i.e. specific column or region from large page) of
   candidates (requires ALTO or PAGE format)
-* aggregate evaluation outcome on domain range (with multiple subdomains)
-* choose from textual metrics based on characters or words plus common Information Retrieval
-* choose between accuracy / error rate and different UTF-8 Python norms
+* aggregate evaluation outcomes on domain range (with multiple subdomains) according to folder layout
 * formats: ALTO, PAGE or plain text for both groundtruth and candidates
 * speedup with parallel execution
 * additional OCR util:
-  * filter custom areas of single OCR files
+  * filter custom areas of single OCR files of ALTO files
 
 ## Installation
 
 ```bash
 pip install digital-eval
 ```
 
 ## Usage
 
 ### Metrics
 
-Calculate similarity (`acc`) or difference (`err`) ratios between single reference/groundtruth and test/candidate item.
-
-#### Edit-Distance based
+#### Edit-Distance based Strin Similarity
 
-Character-based text string minus whitechars (`Cs`, `Characters`) or Letter-based (`Ls`, `Letters`) minus whites,
-punctuation and digits.
-Word/Token-based edit-distance of single tokens identified by whitespaces.
+Calculate similarity for each single reference/groundtruth and test/candidate item.
+Complete haracter-based text string (`Cs`, `Characters`) or Letter-based (`Ls`, `Letters`) minus whitespaces,
+punctuation and common digits (arabic, persian). 
+Word/Token-based edit-distance of single tokens identified by Word or String elements or whitespaces, depending on data.
 
 #### Set based
 
 Calculate union of sets of tokens/words (`BoW`, `BagOfWords`).
 Operate on sets of tokens/words with respect to language specific stopwords using [nltk](https://www.nltk.org/)
 -framework for:
 
@@ -130,35 +132,32 @@
 Plattform: Intel(R) Core(TM) i5-6500 CPU@3.20GHz, 16GB RAM, Ubuntu 20.04 LTS, Python 3.8.
 
 ```bash
 # clone local
 git clone <repository-url> <local-dir>
 cd <local-dir>
 
-# enable virtual python environment (linux)
-# and install libraries
+# enable virtual python 3 environment (linux)
+# and update pip itself
 python3 -m venv venv
 . venv/bin/activate
 python -m pip install -U pip
-python -m pip install -r requirements.txt
 
 # install
-pip install .
+python -m pip install -e .
 
-# optional:
 # install additional development dependencies
-pip install -r tests/test_requirements.txt
-pytest -v
+python -m pip install -r tests/test_requirements.txt
 
-# run
-digital-eval --help
+# run tests
+python -m pytest -v
 ```
 
 ## Contribute
 
 Contributions, suggestions and proposals welcome!
 
-## Licence
+## License
 
 Under terms of the [MIT license](https://opensource.org/licenses/MIT).
 
-**NOTE**: This software depends on other packages that _may_ be licensed under different open source licenses.
+**NOTE**: This software depends on packages that _might_ be licensed under different terms.
```

### Comparing `digital-eval-1.5.3/src/ocr_util/cli.py` & `digital_eval-1.6.0/src/ocr_util/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # -*- coding: utf-8 -*-
 """OCR Utils"""
 
 import argparse
 import re
 from pathlib import PurePath
-from typing import Final
 
-from digital_eval import Piece
-from digital_eval.model import from_pieces
-from ocr_util import PolygonFrameFilterUtil, PolygonFrameFilter
+import digital_object as do
+import digital_object.filter as dofi
 
 # script constants
-
-DEFAULT_VERBOSITY: int = 0
-SUB_CMD_FRAME: Final[str] = 'frame'
+DEFAULT_VERBOSITY = 0
+SUB_CMD_FRAME = 'frame'
 
 
 def points_type(points: str) -> str:
-    match: re.Match = re.match(PolygonFrameFilterUtil.POINT_LIST_PATTERN, points)
+    match: re.Match = re.match(dofi.PolygonFrameFilterUtil.POINT_LIST_PATTERN, points)
     if not match:
         raise argparse.ArgumentTypeError(f"Invalid point coordinates: '{points}'")
     return points
 
 
 def start() -> None:
     arg_parser: argparse.ArgumentParser = argparse.ArgumentParser(
@@ -69,20 +66,20 @@
     verbosity: int = args.verbosity
     if args.subcommand == SUB_CMD_FRAME:
         input_ocr_file: str = args.input_ocr_file
         output_ocr_file: str = args.output_ocr_file
         points: str = args.points
         if verbosity > 1:
             print(f"[DEBUG] args: {input_ocr_file}, {output_ocr_file}, {points}, {verbosity}")
-        polygon_frame_filter: PolygonFrameFilter = PolygonFrameFilter(
+        polygon_frame_filter: dofi.PolygonFrameFilter = dofi.PolygonFrameFilter(
             input_ocr_file,
             points,
             verbosity
         )
-        piece_result: Piece = polygon_frame_filter.process()
-        file_result: PurePath = from_pieces(piece_result, output_ocr_file)
+        piece_result: do.DigitalObjectTree = polygon_frame_filter.process()
+        file_result: PurePath = do.from_digital_object(piece_result, output_ocr_file)
         if verbosity > 0:
             print('[INFO ] file_result', file_result)
 
 
 if __name__ == "__main__":
     start()
```

