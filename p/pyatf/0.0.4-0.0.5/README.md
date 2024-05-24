# Comparing `tmp/pyatf-0.0.4.tar.gz` & `tmp/pyatf-0.0.5.tar.gz`

## Comparing `pyatf-0.0.4.tar` & `pyatf-0.0.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    15623 2020-02-02 00:00:00.000000 pyatf-0.0.4/README.md
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/feature_demonstration/program_guided_tuning/program_guided_tuning.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/feature_demonstration/result_check/result_check.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/bash__gcc_flags/bash__gcc_flags.py
--rwxr-xr-x   0        0        0      151 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/bash__gcc_flags/raytracer/compile_raytracer.sh
--rw-r--r--   0        0        0    10585 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/bash__gcc_flags/raytracer/raytracer.cpp
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/bash__opentuner_matmul/bash__opentuner_matmul.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/bash__opentuner_matmul/mmm_block.cpp
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/cuda__saxpy/cuda__saxpy.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/opencl__saxpy/opencl__saxpy.py
--rw-r--r--   0        0        0    19051 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/opencl__sgemm/cltune_gemm.cl
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 pyatf-0.0.4/examples/full_examples/opencl__sgemm/opencl__sgemm.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/__init__.py
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/range.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/result_check.py
--rw-r--r--   0        0        0    26798 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_space.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/tp.py
--rw-r--r--   0        0        0    13289 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/tuner.py
--rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/tuning_data.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/abort_conditions/__init__.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/abort_conditions/abort_condition.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/abort_conditions/cost.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/abort_conditions/duration.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/abort_conditions/evaluations.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/abort_conditions/fraction.py
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/abort_conditions/speedup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/cost_functions/__init__.py
--rw-r--r--   0        0        0    20784 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/cost_functions/cuda.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/cost_functions/generic.py
--rw-r--r--   0        0        0    16487 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/cost_functions/opencl.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/cost_functions/python.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/__init__.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/auc_bandit.py
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/differential_evolution.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/exhaustive.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/opentuner.py
--rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/pattern_search.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/random.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/round_robin.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/search_technique.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/search_technique_1d.py
--rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/simulated_annealing.py
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 pyatf-0.0.4/src/pyatf/search_techniques/torczon.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyatf-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 pyatf-0.0.4/tests/test_range.py
--rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 pyatf-0.0.4/tests/test_search_space.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyatf-0.0.4/tests/test_tp.py
--rw-r--r--   0        0        0    14546 2020-02-02 00:00:00.000000 pyatf-0.0.4/tests/test_tuning_data.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pyatf-0.0.4/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 pyatf-0.0.4/LICENSE
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pyatf-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pyatf-0.0.4/PyPI/README.md
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 pyatf-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    15623 2020-02-02 00:00:00.000000 pyatf-0.0.5/README.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 pyatf-0.0.5/examples/feature_demonstration/program_guided_tuning/program_guided_tuning.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 pyatf-0.0.5/examples/feature_demonstration/result_check/result_check.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyatf-0.0.5/examples/full_examples/bash__gcc_flags/bash__gcc_flags.py
+-rwxr-xr-x   0        0        0      151 2020-02-02 00:00:00.000000 pyatf-0.0.5/examples/full_examples/bash__gcc_flags/raytracer/compile_raytracer.sh
+-rw-r--r--   0        0        0    10585 2020-02-02 00:00:00.000000 pyatf-0.0.5/examples/full_examples/bash__gcc_flags/raytracer/raytracer.cpp
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pyatf-0.0.5/examples/full_examples/bash__opentuner_matmul/bash__opentuner_matmul.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pyatf-0.0.5/examples/full_examples/bash__opentuner_matmul/mmm_block.cpp
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 pyatf-0.0.5/examples/full_examples/cuda__saxpy/cuda__saxpy.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pyatf-0.0.5/examples/full_examples/opencl__saxpy/opencl__saxpy.py
+-rw-r--r--   0        0        0    19051 2020-02-02 00:00:00.000000 pyatf-0.0.5/examples/full_examples/opencl__sgemm/cltune_gemm.cl
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 pyatf-0.0.5/examples/full_examples/opencl__sgemm/opencl__sgemm.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/__init__.py
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/range.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/result_check.py
+-rw-r--r--   0        0        0    26798 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/search_space.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/tp.py
+-rw-r--r--   0        0        0    13456 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/tuner.py
+-rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/tuning_data.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/abort_conditions/__init__.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/abort_conditions/abort_condition.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/abort_conditions/cost.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/abort_conditions/duration.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/abort_conditions/evaluations.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/abort_conditions/fraction.py
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/abort_conditions/speedup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/cost_functions/__init__.py
+-rw-r--r--   0        0        0    20784 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/cost_functions/cuda.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/cost_functions/generic.py
+-rw-r--r--   0        0        0    16487 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/cost_functions/opencl.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/cost_functions/python.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/search_techniques/__init__.py
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/search_techniques/auc_bandit.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/search_techniques/differential_evolution.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/search_techniques/exhaustive.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/search_techniques/opentuner.py
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/search_techniques/pattern_search.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/search_techniques/random.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/search_techniques/round_robin.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/search_techniques/search_technique.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/search_techniques/search_technique_1d.py
+-rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/search_techniques/simulated_annealing.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 pyatf-0.0.5/src/pyatf/search_techniques/torczon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyatf-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 pyatf-0.0.5/tests/test_range.py
+-rw-r--r--   0        0        0    12409 2020-02-02 00:00:00.000000 pyatf-0.0.5/tests/test_search_space.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyatf-0.0.5/tests/test_tp.py
+-rw-r--r--   0        0        0    14546 2020-02-02 00:00:00.000000 pyatf-0.0.5/tests/test_tuning_data.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pyatf-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 pyatf-0.0.5/LICENSE
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pyatf-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pyatf-0.0.5/PyPI/README.md
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 pyatf-0.0.5/PKG-INFO
```

### Comparing `pyatf-0.0.4/README.md` & `pyatf-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/examples/feature_demonstration/program_guided_tuning/program_guided_tuning.py` & `pyatf-0.0.5/examples/feature_demonstration/program_guided_tuning/program_guided_tuning.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/examples/feature_demonstration/result_check/result_check.py` & `pyatf-0.0.5/examples/feature_demonstration/result_check/result_check.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/examples/full_examples/bash__gcc_flags/bash__gcc_flags.py` & `pyatf-0.0.5/examples/full_examples/bash__gcc_flags/bash__gcc_flags.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/examples/full_examples/bash__gcc_flags/raytracer/raytracer.cpp` & `pyatf-0.0.5/examples/full_examples/bash__gcc_flags/raytracer/raytracer.cpp`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/examples/full_examples/bash__opentuner_matmul/bash__opentuner_matmul.py` & `pyatf-0.0.5/examples/full_examples/bash__opentuner_matmul/bash__opentuner_matmul.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/examples/full_examples/bash__opentuner_matmul/mmm_block.cpp` & `pyatf-0.0.5/examples/full_examples/bash__opentuner_matmul/mmm_block.cpp`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/examples/full_examples/cuda__saxpy/cuda__saxpy.py` & `pyatf-0.0.5/examples/full_examples/cuda__saxpy/cuda__saxpy.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/examples/full_examples/opencl__saxpy/opencl__saxpy.py` & `pyatf-0.0.5/examples/full_examples/opencl__saxpy/opencl__saxpy.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/examples/full_examples/opencl__sgemm/cltune_gemm.cl` & `pyatf-0.0.5/examples/full_examples/opencl__sgemm/cltune_gemm.cl`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/examples/full_examples/opencl__sgemm/opencl__sgemm.py` & `pyatf-0.0.5/examples/full_examples/opencl__sgemm/opencl__sgemm.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/range.py` & `pyatf-0.0.5/src/pyatf/range.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/search_space.py` & `pyatf-0.0.5/src/pyatf/search_space.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/tp.py` & `pyatf-0.0.5/src/pyatf/tp.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/tuner.py` & `pyatf-0.0.5/src/pyatf/tuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,18 @@
                                            self._abort_condition.to_json())
 
             # write tuning data
             if self._log_file:
                 json.dump(self._tuning_data.to_json(), self._log_file, indent=4)
 
             # initialize search technique
-            self._search_technique.initialize(self._search_space.num_tps)
+            if isinstance(self._search_technique, SearchTechnique1D):
+                self._search_technique.initialize(len(self._search_space))
+            else:
+                self._search_technique.initialize(self._search_space.num_tps)
 
         def make_step(self):
             # get new coordinates
             if not self._coordinates_or_indices:
                 if self._costs:
                     self._search_technique.report_costs(self._costs)
                     self._costs.clear()
```

### Comparing `pyatf-0.0.4/src/pyatf/tuning_data.py` & `pyatf-0.0.5/src/pyatf/tuning_data.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/abort_conditions/abort_condition.py` & `pyatf-0.0.5/src/pyatf/abort_conditions/abort_condition.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/abort_conditions/duration.py` & `pyatf-0.0.5/src/pyatf/abort_conditions/duration.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/abort_conditions/evaluations.py` & `pyatf-0.0.5/src/pyatf/abort_conditions/evaluations.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/abort_conditions/fraction.py` & `pyatf-0.0.5/src/pyatf/abort_conditions/fraction.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/abort_conditions/speedup.py` & `pyatf-0.0.5/src/pyatf/abort_conditions/speedup.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/cost_functions/cuda.py` & `pyatf-0.0.5/src/pyatf/cost_functions/cuda.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/cost_functions/generic.py` & `pyatf-0.0.5/src/pyatf/cost_functions/generic.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/cost_functions/opencl.py` & `pyatf-0.0.5/src/pyatf/cost_functions/opencl.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/cost_functions/python.py` & `pyatf-0.0.5/src/pyatf/cost_functions/python.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/search_techniques/auc_bandit.py` & `pyatf-0.0.5/src/pyatf/search_techniques/auc_bandit.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/search_techniques/differential_evolution.py` & `pyatf-0.0.5/src/pyatf/search_techniques/differential_evolution.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/search_techniques/exhaustive.py` & `pyatf-0.0.5/src/pyatf/search_techniques/exhaustive.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/search_techniques/opentuner.py` & `pyatf-0.0.5/src/pyatf/search_techniques/opentuner.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/search_techniques/pattern_search.py` & `pyatf-0.0.5/src/pyatf/search_techniques/pattern_search.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/search_techniques/random.py` & `pyatf-0.0.5/src/pyatf/search_techniques/random.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/search_techniques/round_robin.py` & `pyatf-0.0.5/src/pyatf/search_techniques/round_robin.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/search_techniques/search_technique.py` & `pyatf-0.0.5/src/pyatf/search_techniques/search_technique.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/search_techniques/search_technique_1d.py` & `pyatf-0.0.5/src/pyatf/search_techniques/search_technique_1d.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/search_techniques/simulated_annealing.py` & `pyatf-0.0.5/src/pyatf/search_techniques/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/src/pyatf/search_techniques/torczon.py` & `pyatf-0.0.5/src/pyatf/search_techniques/torczon.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/tests/test_range.py` & `pyatf-0.0.5/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/tests/test_search_space.py` & `pyatf-0.0.5/tests/test_search_space.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,40 +74,49 @@
                                   for data, (children, num_leafs) in gold_grandchildren.items()])
 
         for value_tree, (gold_tree, gold_num_leafs) in zip(value, gold):
             deep_compare(value_tree.root, gold_num_leafs,
                          [(data, children, num_leafs)
                           for data, (children, num_leafs) in gold_tree.items()])
 
-    def test_single_tp(self):
+    def test_single_tp_interval(self):
         tp1 = TP('tp1', Interval(1, 10))
         search_space = SearchSpace(tp1)
         self._check_cot(search_space.cot, [({tp1.values: (None, 1)}, 10)])
         self.assertEqual(10, len(search_space))
         self.assertEqual({'tp1': 1}, search_space.get_configuration((0.00001,)))
         self.assertEqual({'tp1': 1}, search_space.get_configuration((0.10000,)))
         self.assertEqual({'tp1': 8}, search_space.get_configuration((0.70001,)))
         self.assertEqual({'tp1': 8}, search_space.get_configuration((0.72351,)))
         self.assertEqual({'tp1': 8}, search_space.get_configuration((0.80000,)))
         self.assertEqual({'tp1': 10}, search_space.get_configuration((1.00000,)))
 
+    def test_single_tp_set(self):
+        tp1 = TP('tp1', Set(1, 2, 3))
+        search_space = SearchSpace(tp1)
+        self._check_cot(search_space.cot, [({tp1.values: (None, 1)}, 3)])
+        self.assertEqual(3, len(search_space))
+        self.assertEqual({'tp1': 1}, search_space.get_configuration((0.00001,)))
+        self.assertEqual({'tp1': 2}, search_space.get_configuration((0.50000,)))
+        self.assertEqual({'tp1': 3}, search_space.get_configuration((1.00000,)))
+
     def test_independent_tps(self):
         tp1 = TP('tp1', Interval(1, 10))
-        tp2 = TP('tp2', Interval(5, 10))
+        tp2 = TP('tp2', Set(5, 6, 7, 8, 9, 10))
         search_space = SearchSpace(tp1, tp2)
         self._check_cot(search_space.cot, [({tp1.values: (None, 1)}, 10), ({tp2.values: (None, 1)}, 6)])
         self.assertEqual(60, len(search_space))
         self.assertEqual({'tp1': 1, 'tp2': 5}, search_space.get_configuration((0.00001, 0.00001)))
         self.assertEqual({'tp1': 4, 'tp2': 8}, search_space.get_configuration((0.30001, 0.50001)))
         self.assertEqual({'tp1': 4, 'tp2': 10}, search_space.get_configuration((0.30001, 1.00000)))
 
     def test_dependent_tps(self):
         search_space = SearchSpace(
             TP('tp1', Interval(1, 10)),
-            TP('tp2', Interval(5, 10), lambda tp2, tp1: tp2 % tp1 == 0),
+            TP('tp2', Set(5, 6, 7, 8, 9, 10), lambda tp2, tp1: tp2 % tp1 == 0),
             TP('tp3', Interval(2, 3), lambda tp3, tp1: tp1 % tp3 == 0)
         )
         self._check_cot(search_space.cot, [
             ({
                  2: ({6: ({2: (None, 1)}, 1), 8: ({2: (None, 1)}, 1), 10: ({2: (None, 1)}, 1)}, 3),
                  3: ({6: ({3: (None, 1)}, 1), 9: ({3: (None, 1)}, 1)}, 2),
                  4: ({8: ({2: (None, 1)}, 1)}, 1),
@@ -122,15 +131,15 @@
         self.assertEqual({'tp1': 2, 'tp2': 8, 'tp3': 2}, search_space.get_configuration((0.00001, 0.66666, 1.00000)))
         self.assertEqual({'tp1': 6, 'tp2': 6, 'tp3': 2}, search_space.get_configuration((0.60000, 0.00001, 0.50000)))
         self.assertEqual({'tp1': 6, 'tp2': 6, 'tp3': 3}, search_space.get_configuration((0.60000, 1.00000, 0.50001)))
 
     def test_multiple_dependent_tp_groups(self):
         search_space = SearchSpace(
             TP('tp1', Interval(1, 10)),
-            TP('tp2', Interval(5, 10), lambda tp2, tp1: tp2 % tp1 == 0),
+            TP('tp2', Set(5, 6, 7, 8, 9, 10), lambda tp2, tp1: tp2 % tp1 == 0),
             TP('tp3', Interval(2, 3), lambda tp3, tp1: tp1 % tp3 == 0),
 
             TP('tp4', Set(min, max)),
             TP('tp5', Interval(1, 10)),
             TP('tp6', Interval(1, 10), lambda tp6, tp4, tp5: tp4(tp5, tp6) == 10)
         )
         self._check_cot(search_space.cot, [
@@ -168,19 +177,19 @@
         self.assertEqual({'tp1': 3, 'tp2': 9, 'tp3': 3, 'tp4': max, 'tp5': 1, 'tp6': 10},
                          search_space.get_configuration((0.45454, 0.90000, 1.00000, 0.05001, 0.00001, 0.64537)))
         self.assertEqual({'tp1': 4, 'tp2': 8, 'tp3': 2, 'tp4': max, 'tp5': 9, 'tp6': 10},
                          search_space.get_configuration((0.45455, 0.65410, 0.50000, 0.95348, 0.47368, 0.00001)))
         self.assertEqual({'tp1': 4, 'tp2': 8, 'tp3': 2, 'tp4': max, 'tp5': 10, 'tp6': 7},
                          search_space.get_configuration((0.45455, 0.65410, 0.50001, 1.00000, 0.47369, 0.68753)))
 
-    def test_1d_access(self):
+    def test_1d_access_interval(self):
         tp7 = TP('tp7', Interval(1, 2))
         search_space = SearchSpace(
             TP('tp1', Interval(1, 10)),
-            TP('tp2', Interval(5, 10), lambda tp2, tp1: tp2 % tp1 == 0),
+            TP('tp2', Set(5, 6, 7, 8, 9, 10), lambda tp2, tp1: tp2 % tp1 == 0),
             TP('tp3', Interval(2, 3), lambda tp3, tp1: tp1 % tp3 == 0),
 
             TP('tp4', Set(min, max)),
             TP('tp5', Interval(1, 10)),
             TP('tp6', Interval(1, 10), lambda tp6, tp4, tp5: tp4(tp5, tp6) == 10),
 
             tp7,
```

### Comparing `pyatf-0.0.4/tests/test_tp.py` & `pyatf-0.0.5/tests/test_tp.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/tests/test_tuning_data.py` & `pyatf-0.0.5/tests/test_tuning_data.py`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/LICENSE` & `pyatf-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/pyproject.toml` & `pyatf-0.0.5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyatf"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name="Richard Schulze", email="r.schulze@uni-muenster.de" },
     { name="Ari Rasch", email="a.rasch@uni-muenster.de" }
 ]
 description = "Auto-Tuning Framework (ATF) is a generic, general-purpose auto-tuning approach for programs whose tuning parameters may be constrained"
 readme = "./PyPI/README.md"
 requires-python = ">=3.9"
```

### Comparing `pyatf-0.0.4/PyPI/README.md` & `pyatf-0.0.5/PyPI/README.md`

 * *Files identical despite different names*

### Comparing `pyatf-0.0.4/PKG-INFO` & `pyatf-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatf
-Version: 0.0.4
+Version: 0.0.5
 Summary: Auto-Tuning Framework (ATF) is a generic, general-purpose auto-tuning approach for programs whose tuning parameters may be constrained
 Project-URL: Homepage, https://atf-project.org/
 Project-URL: Issues, https://github.com/atf-tuner/pyATF/issues
 Author-email: Richard Schulze <r.schulze@uni-muenster.de>, Ari Rasch <a.rasch@uni-muenster.de>
 License-File: LICENSE
 Keywords: auto-tuning,constraints,optimization,performance,tuning
 Classifier: License :: OSI Approved :: MIT License
```

