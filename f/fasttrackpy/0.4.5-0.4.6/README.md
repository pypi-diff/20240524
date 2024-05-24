# Comparing `tmp/fasttrackpy-0.4.5.tar.gz` & `tmp/fasttrackpy-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttrackpy-0.4.5.tar", max compression
+gzip compressed data, was "fasttrackpy-0.4.6.tar", max compression
```

## Comparing `fasttrackpy-0.4.5.tar` & `fasttrackpy-0.4.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1072 2023-11-15 22:25:59.747254 fasttrackpy-0.4.5/LICENSE
--rw-r--r--   0        0        0     1617 2024-05-21 16:47:49.547057 fasttrackpy-0.4.5/README.md
--rw-r--r--   0        0        0     1746 2024-05-21 16:47:49.548166 fasttrackpy-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      629 2023-11-28 04:58:49.197727 fasttrackpy-0.4.5/src/fasttrackpy/__init__.py
--rw-r--r--   0        0        0    17458 2024-04-25 20:32:54.436009 fasttrackpy-0.4.5/src/fasttrackpy/cli.py
--rw-r--r--   0        0        0        0 2023-11-15 22:25:59.749448 fasttrackpy-0.4.5/src/fasttrackpy/patterns/__init__.py
--rw-r--r--   0        0        0     6455 2024-05-21 16:47:49.548507 fasttrackpy-0.4.5/src/fasttrackpy/patterns/audio_textgrid.py
--rw-r--r--   0        0        0     8109 2024-05-21 16:47:49.548720 fasttrackpy-0.4.5/src/fasttrackpy/patterns/corpus.py
--rw-r--r--   0        0        0     7464 2024-05-21 16:47:49.548926 fasttrackpy-0.4.5/src/fasttrackpy/patterns/just_audio.py
--rw-r--r--   0        0        0        0 2023-11-15 22:11:10.457070 fasttrackpy-0.4.5/src/fasttrackpy/processors/__init__.py
--rw-r--r--   0        0        0      844 2023-11-15 22:25:59.749799 fasttrackpy-0.4.5/src/fasttrackpy/processors/aggs.py
--rw-r--r--   0        0        0     1753 2023-11-15 22:25:59.749908 fasttrackpy-0.4.5/src/fasttrackpy/processors/losses.py
--rw-r--r--   0        0        0    13195 2024-05-21 16:47:49.549143 fasttrackpy-0.4.5/src/fasttrackpy/processors/outputs.py
--rw-r--r--   0        0        0     3285 2024-05-13 16:24:10.932141 fasttrackpy-0.4.5/src/fasttrackpy/processors/smoothers.py
--rw-r--r--   0        0        0        0 2023-11-27 01:47:20.549781 fasttrackpy-0.4.5/src/fasttrackpy/resources/config.yml
--rw-r--r--   0        0        0    20530 2024-05-21 15:07:51.285028 fasttrackpy-0.4.5/src/fasttrackpy/tracks.py
--rw-r--r--   0        0        0        0 2024-05-21 16:47:49.549179 fasttrackpy-0.4.5/src/fasttrackpy/utils/__init__.py
--rw-r--r--   0        0        0     1751 2024-05-21 16:47:49.549349 fasttrackpy-0.4.5/src/fasttrackpy/utils/safely.py
--rw-r--r--   0        0        0     3252 1970-01-01 00:00:00.000000 fasttrackpy-0.4.5/setup.py
--rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 fasttrackpy-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-11-15 22:25:59.747254 fasttrackpy-0.4.6/LICENSE
+-rw-r--r--   0        0        0     1771 2024-05-24 14:01:21.514666 fasttrackpy-0.4.6/README.md
+-rw-r--r--   0        0        0     1746 2024-05-24 14:01:21.515068 fasttrackpy-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      629 2023-11-28 04:58:49.197727 fasttrackpy-0.4.6/src/fasttrackpy/__init__.py
+-rw-r--r--   0        0        0    17458 2024-04-25 20:32:54.436009 fasttrackpy-0.4.6/src/fasttrackpy/cli.py
+-rw-r--r--   0        0        0        0 2023-11-15 22:25:59.749448 fasttrackpy-0.4.6/src/fasttrackpy/patterns/__init__.py
+-rw-r--r--   0        0        0     7270 2024-05-24 14:01:21.515331 fasttrackpy-0.4.6/src/fasttrackpy/patterns/audio_textgrid.py
+-rw-r--r--   0        0        0     8931 2024-05-24 14:01:21.515535 fasttrackpy-0.4.6/src/fasttrackpy/patterns/corpus.py
+-rw-r--r--   0        0        0     8131 2024-05-24 14:01:21.515720 fasttrackpy-0.4.6/src/fasttrackpy/patterns/just_audio.py
+-rw-r--r--   0        0        0        0 2023-11-15 22:11:10.457070 fasttrackpy-0.4.6/src/fasttrackpy/processors/__init__.py
+-rw-r--r--   0        0        0      844 2023-11-15 22:25:59.749799 fasttrackpy-0.4.6/src/fasttrackpy/processors/aggs.py
+-rw-r--r--   0        0        0     1753 2023-11-15 22:25:59.749908 fasttrackpy-0.4.6/src/fasttrackpy/processors/losses.py
+-rw-r--r--   0        0        0    13195 2024-05-21 16:47:49.549143 fasttrackpy-0.4.6/src/fasttrackpy/processors/outputs.py
+-rw-r--r--   0        0        0     3285 2024-05-13 16:24:10.932141 fasttrackpy-0.4.6/src/fasttrackpy/processors/smoothers.py
+-rw-r--r--   0        0        0        0 2023-11-27 01:47:20.549781 fasttrackpy-0.4.6/src/fasttrackpy/resources/config.yml
+-rw-r--r--   0        0        0    20530 2024-05-21 15:07:51.285028 fasttrackpy-0.4.6/src/fasttrackpy/tracks.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:47:49.549179 fasttrackpy-0.4.6/src/fasttrackpy/utils/__init__.py
+-rw-r--r--   0        0        0     1751 2024-05-24 13:47:41.304285 fasttrackpy-0.4.6/src/fasttrackpy/utils/safely.py
+-rw-r--r--   0        0        0     3405 1970-01-01 00:00:00.000000 fasttrackpy-0.4.6/setup.py
+-rw-r--r--   0        0        0     3132 1970-01-01 00:00:00.000000 fasttrackpy-0.4.6/PKG-INFO
```

### Comparing `fasttrackpy-0.4.5/LICENSE` & `fasttrackpy-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.5/README.md` & `fasttrackpy-0.4.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # FastTrackPy
-[![PyPI](https://img.shields.io/pypi/v/fasttrackpy)](https://pypi.org/project/fasttrackpy/)
-[![Python CI](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [![codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy) <a href="https://codeclimate.com/github/JoFrhwld/fasttrackpy/maintainability"><img src="https://api.codeclimate.com/v1/badges/6725fded174b21a3c59f/maintainability" /></a> [![DOI](https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/latestdoi/580169086)
+[![PyPI](https://img.shields.io/pypi/v/fasttrackpy)](https://pypi.org/project/fasttrackpy/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fasttrackpy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fasttrackpy) [![Python CI](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [![codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy) <a href="https://codeclimate.com/github/JoFrhwld/fasttrackpy/maintainability"><img src="https://api.codeclimate.com/v1/badges/6725fded174b21a3c59f/maintainability" /></a> [![DOI](https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/latestdoi/580169086)
 
 
 A python implementation of the FastTrack method
 
 ## Installation
 
 ```bash
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
 # FastTrackPy [![PyPI](https://img.shields.io/pypi/v/fasttrackpy)](https://
-pypi.org/project/fasttrackpy/) [![Python CI](https://github.com/JoFrhwld/
+pypi.org/project/fasttrackpy/) ![PyPI - Python Version](https://img.shields.io/
+pypi/pyversions/fasttrackpy) ![PyPI - Python Version](https://img.shields.io/
+pypi/pyversions/fasttrackpy) [![Python CI](https://github.com/JoFrhwld/
 fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/
 JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [![codecov](https://
 codecov.io/gh/FastTrackiverse/fasttrackpy/graph/badge.svg?token=GOAWY4B5C8)]
 (https://codecov.io/gh/FastTrackiverse/fasttrackpy) _[_h_t_t_p_s_:_/_/
 _a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_6_7_2_5_f_d_e_d_1_7_4_b_2_1_a_3_c_5_9_f_/_m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_][![DOI]
 (https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/latestdoi/
 580169086) A python implementation of the FastTrack method ## Installation
```

### Comparing `fasttrackpy-0.4.5/pyproject.toml` & `fasttrackpy-0.4.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fasttrackpy"
-version = "0.4.5"
+version = "0.4.6"
 description = "A python implementation of FastTrack"
 authors = [
     "JoFrhwld <JoFrhwld@gmail.com>",
     "santiagobarreda <sbarreda@ucdavis.edu>"
 ]
 license = "MIT"
 readme = "README.md"
@@ -14,18 +14,18 @@
     "examples/",
     "docs/"
 ]
 homepage = "https://fasttrackiverse.github.io/fasttrackpy/"
 repository = "https://github.com/FastTrackiverse/fasttrackpy"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
+python = ">=3.10,<3.13"
 praat-parselmouth = "^0.4.3"
-scipy = {version = "^1.11.3", python = ">=3.10,<3.12"}
-numpy = {version = "^1.26.1", python = ">=3.10,<3.12"}
+scipy = {version = "^1.11.3", python = ">=3.10,<3.13"}
+numpy = {version = "^1.26.1", python = ">=3.10,<3.13"}
 polars = "^0.20.18"
 pytest-cov = "^4.1.0"
 pytest = "^7.4.3"
 python-magic = {version = "^0.4.27", markers = "sys_platform != 'win32'"}
 python-magic-bin = {version = "^0.4.14", markers = "sys_platform == 'win32'"}
 click = "^8.1.7"
 cloup = "^3.0.3"
```

### Comparing `fasttrackpy-0.4.5/src/fasttrackpy/__init__.py` & `fasttrackpy-0.4.6/src/fasttrackpy/__init__.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.5/src/fasttrackpy/cli.py` & `fasttrackpy-0.4.6/src/fasttrackpy/cli.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.5/src/fasttrackpy/patterns/audio_textgrid.py` & `fasttrackpy-0.4.6/src/fasttrackpy/patterns/audio_textgrid.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import parselmouth as pm
 from aligned_textgrid import AlignedTextGrid, Word, Phone, SequenceInterval, SequenceTier
 import aligned_textgrid
 from fasttrackpy import CandidateTracks, Smoother, Loss, Agg
 from fasttrackpy.patterns.just_audio import create_audio_checker
 from fasttrackpy.utils.safely import safely, filter_nones
 import re
+import os
+import sys
 
 from pathlib import Path
 from tqdm import tqdm
 from joblib import Parallel, cpu_count, delayed
 import warnings
 
 try:
@@ -61,24 +63,44 @@
         for interval in tier
         if re.match(target_labels, interval.label) and
         (interval.end - interval.start) > min_duration
     ]
 
     return intervals
 
-@delayed
 @safely(message="There was a problem getting some candidate tracks.")
 def get_candidates(args_dict):
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         candidates =  CandidateTracks(**args_dict)
     if candidates.winner.formants.shape[1] == 1:
         warnings.warn("formant tracking error")
     return candidates
 
+@delayed
+@safely(message="There was a problem getting some candidate tracks.")
+def get_candidates_delayed(args_dict):
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore")
+        candidates =  CandidateTracks(**args_dict)
+    if candidates.winner.formants.shape[1] == 1:
+        warnings.warn("formant tracking error")
+    return candidates
+
+def run_candidates(arg_list, parallel:bool):
+    if parallel:
+        n_jobs = cpu_count()
+        all_candidates = Parallel(n_jobs=n_jobs)(
+            get_candidates_delayed(args_dict=arg) for arg in tqdm(arg_list)
+            )
+        return all_candidates
+    
+    all_candidates = [get_candidates(args_dict=arg) for arg in tqdm(arg_list)]
+    return all_candidates
+
 def process_audio_textgrid(
         audio_path: str|Path,
         textgrid_path: str|Path,
         entry_classes: list = ["Word", "Phone"],
         target_tier: str = "Phone",
         target_labels: str = "[AEIOU]",
         min_duration: float = 0.05,
@@ -164,18 +186,22 @@
             "pre_emphasis_from": pre_emphasis_from,
             "smoother": smoother,
             "loss_fun":loss_fun,
             "agg_fun": agg_fun
         } for x, interval in zip(sound_parts, target_intervals)
     ]
     
-    n_jobs = cpu_count()
-    candidate_list = Parallel(n_jobs=n_jobs)(
-        get_candidates(args_dict=arg) for arg in tqdm(arg_list)
-        )
+    windows_3_12 = os.name != "posix" and \
+            sys.version_info.major == 3 and \
+            sys.version_info.minor == 12
+
+    candidate_list = run_candidates(
+        arg_list, not windows_3_12
+    )
+
     candidate_list, target_intervals = filter_nones(candidate_list, [candidate_list, target_intervals])
     for cand, interval in zip(candidate_list, target_intervals):
         cand.interval = interval
         cand.file_name = Path(str(audio_path)).stem
 
     return candidate_list
```

### Comparing `fasttrackpy-0.4.5/src/fasttrackpy/patterns/corpus.py` & `fasttrackpy-0.4.6/src/fasttrackpy/patterns/corpus.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from collections import namedtuple
 from pathlib import Path
 from tqdm import tqdm
 from functools import reduce
 from operator import add
 from joblib import Parallel, cpu_count, delayed
 import warnings
-
+import os
+import sys
 
 
 try:
     import magic
     no_magic = False
 except:
     warnings.warn("libmagic not found. "\
@@ -111,22 +112,41 @@
         for interval in intervals
     ]
 
     return sound_parts
 
 @delayed
 @safely(message = "There was a problem getting some candidate tracks.")
+def get_candidates_delayed(args_dict):
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore")
+        candidates =  CandidateTracks(**args_dict)
+    if candidates.winner.formants.shape[1] == 1:
+        warnings.warn("formant tracking error")
+    return candidates
+
+@safely(message = "There was a problem getting some candidate tracks.")
 def get_candidates(args_dict):
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         candidates =  CandidateTracks(**args_dict)
     if candidates.winner.formants.shape[1] == 1:
         warnings.warn("formant tracking error")
     return candidates
 
+def run_candidates(arg_list, parallel:bool):
+    if parallel:
+        n_jobs = cpu_count()
+        all_candidates = Parallel(n_jobs=n_jobs)(
+            get_candidates_delayed(args_dict=arg) for arg in tqdm(arg_list)
+            )
+        return all_candidates
+    
+    all_candidates = [get_candidates(args_dict=arg) for arg in tqdm(arg_list)]
+    return all_candidates
 
 def process_corpus(
         corpus_path: str|Path,
         entry_classes: list = ["Word", "Phone"],
         target_tier: str = "Phone",
         target_labels: str = "[AEIOU]",
         min_duration: float = 0.05,
@@ -210,18 +230,21 @@
                 "pre_emphasis_from": pre_emphasis_from,
                 "smoother": smoother,
                 "loss_fun":loss_fun,
                 "agg_fun": agg_fun
             } for x, interval in zip(sound_parts, intervals)
         ]
 
-        n_jobs = cpu_count()
-        candidate_list = Parallel(n_jobs=n_jobs)(
-            get_candidates(args_dict=arg) for arg in tqdm(arg_list)
-            )
+        windows_3_12 = os.name != "posix" and \
+                sys.version_info.major == 3 and \
+                sys.version_info.minor == 12
+
+        candidate_list = run_candidates(
+            arg_list, not windows_3_12
+        )
 
         candidate_list, intervals = filter_nones(candidate_list, [candidate_list, intervals])
         for cand, interval in zip(candidate_list, intervals):
             cand.interval = interval
             cand.file_name = Path(str(interval.wav)).stem
         all_candidates += candidate_list
```

### Comparing `fasttrackpy-0.4.5/src/fasttrackpy/patterns/just_audio.py` & `fasttrackpy-0.4.6/src/fasttrackpy/patterns/just_audio.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,18 @@
                         Smoother,\
                         Loss,\
                         Agg
 from fasttrackpy.utils.safely import safely, filter_nones
 
 from tqdm import tqdm
 from joblib import Parallel, cpu_count, delayed
+import os
+import sys
+import logging
+logging.basicConfig(level=logging.INFO)
 
 try:
     import magic
     no_magic = False
 except:
     warnings.warn("libmagic not found. "\
                 "Some audio file types won't be discovered by fasttrack. "\
@@ -134,17 +138,32 @@
         agg_fun=agg_fun
     )
     candidates.file_name = Path(str(path)).name
     return candidates
 
 @delayed
 @safely(message = "There was a problem processing an audio file.")
-def wrapped_audio(args_dict):
+def get_candidates_delayed(args_dict):
     return process_audio_file(**args_dict)
 
+@safely(message = "There was a problem processing an audio file.")
+def get_candidates(args_dict):
+    return process_audio_file(**args_dict)
+
+def run_candidates(arg_list, parallel:bool):
+    if parallel:
+        n_jobs = cpu_count()
+        all_candidates = Parallel(n_jobs=n_jobs)(
+            get_candidates_delayed(args_dict=arg) for arg in tqdm(arg_list)
+            )
+        return all_candidates
+    
+    all_candidates = [get_candidates(args_dict=arg) for arg in tqdm(arg_list)]
+    return all_candidates
+
 def process_directory(
         path: str|Path,
         min_max_formant:float = 4000,
         max_max_formant:float = 7000,
         nstep:int = 20,
         n_formants: int = 4,
         window_length: float = 0.05,
@@ -198,18 +217,23 @@
             "pre_emphasis_from":pre_emphasis_from,
             "smoother":smoother,
             "loss_fun":loss_fun,
             "agg_fun":agg_fun
             }
             for x in all_audio
     ]
-    n_jobs = cpu_count()
 
-    all_candidates = Parallel(n_jobs=n_jobs)(
-        wrapped_audio(args_dict=arg) for arg in tqdm(arg_list)
-        )
+    windows_3_12 = os.name != "posix" and \
+            sys.version_info.major == 3 and \
+            sys.version_info.minor == 12
+
+    all_candidates = run_candidates(
+        arg_list, not windows_3_12
+    )
+
     all_candidates, all_audio = filter_nones(all_candidates, [all_candidates, all_audio])
+
     for x, path in zip(all_candidates, all_audio):
         x.file_name = Path(str(path)).name
 
     return all_candidates
```

### Comparing `fasttrackpy-0.4.5/src/fasttrackpy/processors/aggs.py` & `fasttrackpy-0.4.6/src/fasttrackpy/processors/aggs.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.5/src/fasttrackpy/processors/losses.py` & `fasttrackpy-0.4.6/src/fasttrackpy/processors/losses.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.5/src/fasttrackpy/processors/outputs.py` & `fasttrackpy-0.4.6/src/fasttrackpy/processors/outputs.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.5/src/fasttrackpy/processors/smoothers.py` & `fasttrackpy-0.4.6/src/fasttrackpy/processors/smoothers.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.5/src/fasttrackpy/tracks.py` & `fasttrackpy-0.4.6/src/fasttrackpy/tracks.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.5/src/fasttrackpy/utils/safely.py` & `fasttrackpy-0.4.6/src/fasttrackpy/utils/safely.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.5/setup.py` & `fasttrackpy-0.4.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,36 +23,36 @@
  'praat-parselmouth>=0.4.3,<0.5.0',
  'pytest-cov>=4.1.0,<5.0.0',
  'pytest>=7.4.3,<8.0.0',
  'pyyaml>=6.0.1,<7.0.0',
  'tqdm>=4.66.1,<5.0.0']
 
 extras_require = \
-{':python_version >= "3.10" and python_version < "3.12"': ['scipy>=1.11.3,<2.0.0',
+{':python_version >= "3.10" and python_version < "3.13"': ['scipy>=1.11.3,<2.0.0',
                                                            'numpy>=1.26.1,<2.0.0'],
  ':sys_platform != "win32"': ['python-magic>=0.4.27,<0.5.0'],
  ':sys_platform == "win32"': ['python-magic-bin>=0.4.14,<0.5.0']}
 
 entry_points = \
 {'console_scripts': ['fasttrack = fasttrackpy.cli:fasttrack']}
 
 setup_kwargs = {
     'name': 'fasttrackpy',
-    'version': '0.4.5',
+    'version': '0.4.6',
     'description': 'A python implementation of FastTrack',
-    'long_description': '# FastTrackPy\n[![PyPI](https://img.shields.io/pypi/v/fasttrackpy)](https://pypi.org/project/fasttrackpy/)\n[![Python CI](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [![codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy) <a href="https://codeclimate.com/github/JoFrhwld/fasttrackpy/maintainability"><img src="https://api.codeclimate.com/v1/badges/6725fded174b21a3c59f/maintainability" /></a> [![DOI](https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/latestdoi/580169086)\n\n\nA python implementation of the FastTrack method\n\n## Installation\n\n```bash\npip install fasttrackpy\n```\n\nThis will make the command line executable `fasttrack` available, along with its subcommands:\n\n- `audio`\n- `audio-textgrid`\n- `corpus`\n\n## Getting help\n\nFor any of the fasttrack subcommands, add the `--help` flag to\nprint the help info. You can also visit [the docs](https://fasttrackiverse.github.io/fasttrackpy/usage/getting_started.html).\n\n## Usage\n\nFor a single audio file containing a vowel-like sound:\n\n```bash\nfasttrack audio --file audio.wav \\\n    --output formants.csv\n```\n\nFor a paired audio file and textgrid with intervals defining\ntarget audio to process:\n\n```bash\nfasttrack audio-textgrid --audio audio.wav \\\n    --textgrid audio.TextGrid \\\n    --output formants.csv\n```\n\nFor a corpus directory of paired audio files and textgrid\n\n```bash\nfasttrack corpus --corpus dir/ \\\n    --output formants.csv\n```',
+    'long_description': '# FastTrackPy\n[![PyPI](https://img.shields.io/pypi/v/fasttrackpy)](https://pypi.org/project/fasttrackpy/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fasttrackpy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fasttrackpy) [![Python CI](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [![codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy) <a href="https://codeclimate.com/github/JoFrhwld/fasttrackpy/maintainability"><img src="https://api.codeclimate.com/v1/badges/6725fded174b21a3c59f/maintainability" /></a> [![DOI](https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/latestdoi/580169086)\n\n\nA python implementation of the FastTrack method\n\n## Installation\n\n```bash\npip install fasttrackpy\n```\n\nThis will make the command line executable `fasttrack` available, along with its subcommands:\n\n- `audio`\n- `audio-textgrid`\n- `corpus`\n\n## Getting help\n\nFor any of the fasttrack subcommands, add the `--help` flag to\nprint the help info. You can also visit [the docs](https://fasttrackiverse.github.io/fasttrackpy/usage/getting_started.html).\n\n## Usage\n\nFor a single audio file containing a vowel-like sound:\n\n```bash\nfasttrack audio --file audio.wav \\\n    --output formants.csv\n```\n\nFor a paired audio file and textgrid with intervals defining\ntarget audio to process:\n\n```bash\nfasttrack audio-textgrid --audio audio.wav \\\n    --textgrid audio.TextGrid \\\n    --output formants.csv\n```\n\nFor a corpus directory of paired audio files and textgrid\n\n```bash\nfasttrack corpus --corpus dir/ \\\n    --output formants.csv\n```',
     'author': 'JoFrhwld',
     'author_email': 'JoFrhwld@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://fasttrackiverse.github.io/fasttrackpy/',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.10,<3.12',
+    'python_requires': '>=3.10,<3.13',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -2,22 +2,24 @@
 'src'} packages = \ ['fasttrackpy', 'fasttrackpy.patterns',
 'fasttrackpy.processors', 'fasttrackpy.utils'] package_data = \ {'': ['*'],
 'fasttrackpy': ['resources/*']} install_requires = \ ['aligned-
 textgrid>=0.6.2,<0.7.0', 'click>=8.1.7,<9.0.0', 'cloup>=3.0.3,<4.0.0',
 'joblib>=1.3.2,<2.0.0', 'matplotlib>=3.8.2,<4.0.0', 'polars>=0.20.18,<0.21.0',
 'praat-parselmouth>=0.4.3,<0.5.0', 'pytest-cov>=4.1.0,<5.0.0',
 'pytest>=7.4.3,<8.0.0', 'pyyaml>=6.0.1,<7.0.0', 'tqdm>=4.66.1,<5.0.0']
-extras_require = \ {':python_version >= "3.10" and python_version < "3.12"':
+extras_require = \ {':python_version >= "3.10" and python_version < "3.13"':
 ['scipy>=1.11.3,<2.0.0', 'numpy>=1.26.1,<2.0.0'], ':sys_platform != "win32"':
 ['python-magic>=0.4.27,<0.5.0'], ':sys_platform == "win32"': ['python-magic-
 bin>=0.4.14,<0.5.0']} entry_points = \ {'console_scripts': ['fasttrack =
 fasttrackpy.cli:fasttrack']} setup_kwargs = { 'name': 'fasttrackpy', 'version':
-'0.4.5', 'description': 'A python implementation of FastTrack',
+'0.4.6', 'description': 'A python implementation of FastTrack',
 'long_description': '# FastTrackPy\n[![PyPI](https://img.shields.io/pypi/v/
-fasttrackpy)](https://pypi.org/project/fasttrackpy/)\n[![Python CI](https://
+fasttrackpy)](https://pypi.org/project/fasttrackpy/) ![PyPI - Python Version]
+(https://img.shields.io/pypi/pyversions/fasttrackpy) ![PyPI - Python Version]
+(https://img.shields.io/pypi/pyversions/fasttrackpy) [![Python CI](https://
 github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)]
 (https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [!
 [codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/
 badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy)
 _[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_6_7_2_5_f_d_e_d_1_7_4_b_2_1_a_3_c_5_9_f_/_m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_][!
 [DOI](https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/
 latestdoi/580169086)\n\n\nA python implementation of the FastTrack method\n\n##
@@ -33,9 +35,9 @@
 audio.wav \\\n --textgrid audio.TextGrid \\\n --output formants.csv\n```\n\nFor
 a corpus directory of paired audio files and textgrid\n\n```bash\nfasttrack
 corpus --corpus dir/ \\\n --output formants.csv\n```', 'author': 'JoFrhwld',
 'author_email': 'JoFrhwld@gmail.com', 'maintainer': 'None', 'maintainer_email':
 'None', 'url': 'https://fasttrackiverse.github.io/fasttrackpy/', 'package_dir':
 package_dir, 'packages': packages, 'package_data': package_data,
 'install_requires': install_requires, 'extras_require': extras_require,
-'entry_points': entry_points, 'python_requires': '>=3.10,<3.12', } setup
+'entry_points': entry_points, 'python_requires': '>=3.10,<3.13', } setup
 (**setup_kwargs)
```

### Comparing `fasttrackpy-0.4.5/PKG-INFO` & `fasttrackpy-0.4.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: fasttrackpy
-Version: 0.4.5
+Version: 0.4.6
 Summary: A python implementation of FastTrack
 Home-page: https://fasttrackiverse.github.io/fasttrackpy/
 License: MIT
 Author: JoFrhwld
 Author-email: JoFrhwld@gmail.com
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aligned-textgrid (>=0.6.2,<0.7.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cloup (>=3.0.3,<4.0.0)
 Requires-Dist: joblib (>=1.3.2,<2.0.0)
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
-Requires-Dist: numpy (>=1.26.1,<2.0.0) ; python_version >= "3.10" and python_version < "3.12"
+Requires-Dist: numpy (>=1.26.1,<2.0.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: polars (>=0.20.18,<0.21.0)
 Requires-Dist: praat-parselmouth (>=0.4.3,<0.5.0)
 Requires-Dist: pytest (>=7.4.3,<8.0.0)
 Requires-Dist: pytest-cov (>=4.1.0,<5.0.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0) ; sys_platform != "win32"
 Requires-Dist: python-magic-bin (>=0.4.14,<0.5.0) ; sys_platform == "win32"
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: scipy (>=1.11.3,<2.0.0) ; python_version >= "3.10" and python_version < "3.12"
+Requires-Dist: scipy (>=1.11.3,<2.0.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Project-URL: Repository, https://github.com/FastTrackiverse/fasttrackpy
 Description-Content-Type: text/markdown
 
 # FastTrackPy
-[![PyPI](https://img.shields.io/pypi/v/fasttrackpy)](https://pypi.org/project/fasttrackpy/)
-[![Python CI](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [![codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy) <a href="https://codeclimate.com/github/JoFrhwld/fasttrackpy/maintainability"><img src="https://api.codeclimate.com/v1/badges/6725fded174b21a3c59f/maintainability" /></a> [![DOI](https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/latestdoi/580169086)
+[![PyPI](https://img.shields.io/pypi/v/fasttrackpy)](https://pypi.org/project/fasttrackpy/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fasttrackpy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fasttrackpy) [![Python CI](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [![codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy) <a href="https://codeclimate.com/github/JoFrhwld/fasttrackpy/maintainability"><img src="https://api.codeclimate.com/v1/badges/6725fded174b21a3c59f/maintainability" /></a> [![DOI](https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/latestdoi/580169086)
 
 
 A python implementation of the FastTrack method
 
 ## Installation
 
 ```bash
```

#### html2text {}

```diff
@@ -1,27 +1,29 @@
-Metadata-Version: 2.1 Name: fasttrackpy Version: 0.4.5 Summary: A python
+Metadata-Version: 2.1 Name: fasttrackpy Version: 0.4.6 Summary: A python
 implementation of FastTrack Home-page: https://fasttrackiverse.github.io/
 fasttrackpy/ License: MIT Author: JoFrhwld Author-email: JoFrhwld@gmail.com
-Requires-Python: >=3.10,<3.12 Classifier: License :: OSI Approved :: MIT
+Requires-Python: >=3.10,<3.13 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aligned-textgrid (>=0.6.2,<0.7.0) Requires-Dist: click
 (>=8.1.7,<9.0.0) Requires-Dist: cloup (>=3.0.3,<4.0.0) Requires-Dist: joblib
 (>=1.3.2,<2.0.0) Requires-Dist: matplotlib (>=3.8.2,<4.0.0) Requires-Dist:
-numpy (>=1.26.1,<2.0.0) ; python_version >= "3.10" and python_version < "3.12"
+numpy (>=1.26.1,<2.0.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: polars (>=0.20.18,<0.21.0) Requires-Dist: praat-parselmouth
 (>=0.4.3,<0.5.0) Requires-Dist: pytest (>=7.4.3,<8.0.0) Requires-Dist: pytest-
 cov (>=4.1.0,<5.0.0) Requires-Dist: python-magic (>=0.4.27,<0.5.0) ;
 sys_platform != "win32" Requires-Dist: python-magic-bin (>=0.4.14,<0.5.0) ;
 sys_platform == "win32" Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist:
-scipy (>=1.11.3,<2.0.0) ; python_version >= "3.10" and python_version < "3.12"
+scipy (>=1.11.3,<2.0.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: tqdm (>=4.66.1,<5.0.0) Project-URL: Repository, https://
 github.com/FastTrackiverse/fasttrackpy Description-Content-Type: text/markdown
 # FastTrackPy [![PyPI](https://img.shields.io/pypi/v/fasttrackpy)](https://
-pypi.org/project/fasttrackpy/) [![Python CI](https://github.com/JoFrhwld/
+pypi.org/project/fasttrackpy/) ![PyPI - Python Version](https://img.shields.io/
+pypi/pyversions/fasttrackpy) ![PyPI - Python Version](https://img.shields.io/
+pypi/pyversions/fasttrackpy) [![Python CI](https://github.com/JoFrhwld/
 fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/
 JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [![codecov](https://
 codecov.io/gh/FastTrackiverse/fasttrackpy/graph/badge.svg?token=GOAWY4B5C8)]
 (https://codecov.io/gh/FastTrackiverse/fasttrackpy) _[_h_t_t_p_s_:_/_/
 _a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_6_7_2_5_f_d_e_d_1_7_4_b_2_1_a_3_c_5_9_f_/_m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_][![DOI]
 (https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/latestdoi/
 580169086) A python implementation of the FastTrack method ## Installation
```

