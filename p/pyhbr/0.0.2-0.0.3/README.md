# Comparing `tmp/pyhbr-0.0.2.tar.gz` & `tmp/pyhbr-0.0.3.tar.gz`

## Comparing `pyhbr-0.0.2.tar` & `pyhbr-0.0.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 pyhbr-0.0.2/mkdocs.yml
--rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 pyhbr-0.0.2/requirements.txt
--rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 pyhbr-0.0.2/docs/arc_hbr.md
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyhbr-0.0.2/docs/data_sources.md
--rw-r--r--   0        0        0    17380 2020-02-02 00:00:00.000000 pyhbr-0.0.2/docs/design.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pyhbr-0.0.2/docs/index.md
--rw-r--r--   0        0        0    19366 2020-02-02 00:00:00.000000 pyhbr-0.0.2/docs/modelling.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyhbr-0.0.2/docs/reference.md
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pyhbr-0.0.2/docs/verification.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/__init__.py
--rw-r--r--   0        0        0    16833 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/common.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/analysis/__init__.py
--rw-r--r--   0        0        0    19503 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/analysis/acs.py
--rw-r--r--   0        0        0    24144 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/analysis/arc_hbr.py
--rw-r--r--   0        0        0    16790 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/analysis/calibration.py
--rw-r--r--   0        0        0     9496 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/analysis/describe.py
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/analysis/dim_reduce.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/analysis/fit.py
--rw-r--r--   0        0        0    12984 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/analysis/model.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/analysis/patient_viewer.py
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/analysis/roc.py
--rw-r--r--   0        0        0    26531 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/analysis/stability.py
--rw-r--r--   0        0        0    10138 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/clinical_codes/__init__.py
--rw-r--r--   0        0        0     7288 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/clinical_codes/counting.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/clinical_codes/codes_editor/__init__.py
--rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/clinical_codes/codes_editor/codes_editor.py
--rw-r--r--   0        0        0  1414802 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/clinical_codes/files/icd10.yaml
--rw-r--r--   0        0        0  1426408 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/clinical_codes/files/icd10_arc_hbr.yaml
--rw-r--r--   0        0        0  1388282 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/clinical_codes/files/icd10_blank.yaml
--rw-r--r--   0        0        0  1414802 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/clinical_codes/files/icd10_dim_reduce.yaml
--rw-r--r--   0        0        0  1390637 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/clinical_codes/files/icd10_test.yaml
--rw-r--r--   0        0        0  1146170 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/clinical_codes/files/opcs4_arc_hbr.yaml
--rw-r--r--   0        0        0  1144037 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/clinical_codes/files/opcs4_blank.yaml
--rw-r--r--   0        0        0  1144037 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/clinical_codes/files/opcs4_dim_reduce.yaml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/data_source/__init__.py
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/data_source/hes.py
--rw-r--r--   0        0        0     9811 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/data_source/hic.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/data_source/hic_covid.py
--rw-r--r--   0        0        0    14424 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/data_source/icb.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/middle/__init__.py
--rw-r--r--   0        0        0    17281 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/middle/from_hic.py
--rw-r--r--   0        0        0    26482 2020-02-02 00:00:00.000000 pyhbr-0.0.2/src/pyhbr/middle/from_icb.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pyhbr-0.0.2/tests/test_example.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pyhbr-0.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pyhbr-0.0.2/LICENSE
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 pyhbr-0.0.2/README.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pyhbr-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 pyhbr-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 pyhbr-0.0.3/mkdocs.yml
+-rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 pyhbr-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 pyhbr-0.0.3/docs/arc_hbr.md
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyhbr-0.0.3/docs/data_sources.md
+-rw-r--r--   0        0        0    17380 2020-02-02 00:00:00.000000 pyhbr-0.0.3/docs/design.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pyhbr-0.0.3/docs/index.md
+-rw-r--r--   0        0        0    19366 2020-02-02 00:00:00.000000 pyhbr-0.0.3/docs/modelling.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyhbr-0.0.3/docs/reference.md
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pyhbr-0.0.3/docs/verification.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/__init__.py
+-rw-r--r--   0        0        0    16833 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/common.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/analysis/__init__.py
+-rw-r--r--   0        0        0    19503 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/analysis/acs.py
+-rw-r--r--   0        0        0    24144 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/analysis/arc_hbr.py
+-rw-r--r--   0        0        0    16790 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/analysis/calibration.py
+-rw-r--r--   0        0        0     9496 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/analysis/describe.py
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/analysis/dim_reduce.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/analysis/fit.py
+-rw-r--r--   0        0        0    12984 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/analysis/model.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/analysis/patient_viewer.py
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/analysis/roc.py
+-rw-r--r--   0        0        0    26531 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/analysis/stability.py
+-rw-r--r--   0        0        0    10138 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/clinical_codes/__init__.py
+-rw-r--r--   0        0        0     7288 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/clinical_codes/counting.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/clinical_codes/codes_editor/__init__.py
+-rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/clinical_codes/codes_editor/codes_editor.py
+-rw-r--r--   0        0        0  1414802 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/clinical_codes/files/icd10.yaml
+-rw-r--r--   0        0        0  1426408 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/clinical_codes/files/icd10_arc_hbr.yaml
+-rw-r--r--   0        0        0  1388282 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/clinical_codes/files/icd10_blank.yaml
+-rw-r--r--   0        0        0  1414802 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/clinical_codes/files/icd10_dim_reduce.yaml
+-rw-r--r--   0        0        0  1390637 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/clinical_codes/files/icd10_test.yaml
+-rw-r--r--   0        0        0  1146170 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/clinical_codes/files/opcs4_arc_hbr.yaml
+-rw-r--r--   0        0        0  1144037 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/clinical_codes/files/opcs4_blank.yaml
+-rw-r--r--   0        0        0  1144037 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/clinical_codes/files/opcs4_dim_reduce.yaml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/data_source/__init__.py
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/data_source/hes.py
+-rw-r--r--   0        0        0     9811 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/data_source/hic.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/data_source/hic_covid.py
+-rw-r--r--   0        0        0    14424 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/data_source/icb.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/middle/__init__.py
+-rw-r--r--   0        0        0    17281 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/middle/from_hic.py
+-rw-r--r--   0        0        0    26482 2020-02-02 00:00:00.000000 pyhbr-0.0.3/src/pyhbr/middle/from_icb.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pyhbr-0.0.3/tests/test_example.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pyhbr-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pyhbr-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 pyhbr-0.0.3/README.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pyhbr-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 pyhbr-0.0.3/PKG-INFO
```

### Comparing `pyhbr-0.0.2/mkdocs.yml` & `pyhbr-0.0.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/requirements.txt` & `pyhbr-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/docs/arc_hbr.md` & `pyhbr-0.0.3/docs/arc_hbr.md`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/docs/design.md` & `pyhbr-0.0.3/docs/design.md`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/docs/modelling.md` & `pyhbr-0.0.3/docs/modelling.md`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/common.py` & `pyhbr-0.0.3/src/pyhbr/common.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/analysis/acs.py` & `pyhbr-0.0.3/src/pyhbr/analysis/acs.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/analysis/arc_hbr.py` & `pyhbr-0.0.3/src/pyhbr/analysis/arc_hbr.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/analysis/calibration.py` & `pyhbr-0.0.3/src/pyhbr/analysis/calibration.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/analysis/describe.py` & `pyhbr-0.0.3/src/pyhbr/analysis/describe.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/analysis/dim_reduce.py` & `pyhbr-0.0.3/src/pyhbr/analysis/dim_reduce.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/analysis/fit.py` & `pyhbr-0.0.3/src/pyhbr/analysis/fit.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/analysis/model.py` & `pyhbr-0.0.3/src/pyhbr/analysis/model.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/analysis/patient_viewer.py` & `pyhbr-0.0.3/src/pyhbr/analysis/patient_viewer.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/analysis/roc.py` & `pyhbr-0.0.3/src/pyhbr/analysis/roc.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/analysis/stability.py` & `pyhbr-0.0.3/src/pyhbr/analysis/stability.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/clinical_codes/__init__.py` & `pyhbr-0.0.3/src/pyhbr/clinical_codes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/clinical_codes/counting.py` & `pyhbr-0.0.3/src/pyhbr/clinical_codes/counting.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/clinical_codes/codes_editor/codes_editor.py` & `pyhbr-0.0.3/src/pyhbr/clinical_codes/codes_editor/codes_editor.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/clinical_codes/files/icd10.yaml` & `pyhbr-0.0.3/src/pyhbr/clinical_codes/files/icd10.yaml`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/clinical_codes/files/icd10_arc_hbr.yaml` & `pyhbr-0.0.3/src/pyhbr/clinical_codes/files/icd10_arc_hbr.yaml`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/clinical_codes/files/icd10_blank.yaml` & `pyhbr-0.0.3/src/pyhbr/clinical_codes/files/icd10_blank.yaml`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/clinical_codes/files/icd10_dim_reduce.yaml` & `pyhbr-0.0.3/src/pyhbr/clinical_codes/files/icd10_dim_reduce.yaml`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/clinical_codes/files/icd10_test.yaml` & `pyhbr-0.0.3/src/pyhbr/clinical_codes/files/icd10_test.yaml`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/clinical_codes/files/opcs4_arc_hbr.yaml` & `pyhbr-0.0.3/src/pyhbr/clinical_codes/files/opcs4_arc_hbr.yaml`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/clinical_codes/files/opcs4_blank.yaml` & `pyhbr-0.0.3/src/pyhbr/clinical_codes/files/opcs4_blank.yaml`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/clinical_codes/files/opcs4_dim_reduce.yaml` & `pyhbr-0.0.3/src/pyhbr/clinical_codes/files/opcs4_dim_reduce.yaml`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/data_source/hes.py` & `pyhbr-0.0.3/src/pyhbr/data_source/hes.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/data_source/hic.py` & `pyhbr-0.0.3/src/pyhbr/data_source/hic.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/data_source/hic_covid.py` & `pyhbr-0.0.3/src/pyhbr/data_source/hic_covid.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/data_source/icb.py` & `pyhbr-0.0.3/src/pyhbr/data_source/icb.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/middle/from_hic.py` & `pyhbr-0.0.3/src/pyhbr/middle/from_hic.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/src/pyhbr/middle/from_icb.py` & `pyhbr-0.0.3/src/pyhbr/middle/from_icb.py`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/LICENSE` & `pyhbr-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhbr-0.0.2/README.md` & `pyhbr-0.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Python Package for Tool/Model Development
 
 This package will contain all the data analysis, model development, and other utilities developed as part of the BHF HBR project.
 
 ## Package Installation
 
-The intention is to host `pyhbr` on PyPI. For now, it is available on TestPyPi, and can be installed using:
+To install the latest version of the package, run
 
 ```bash
-pip install -i https://test.pypi.org/simple/ pyhbr
+pip install pyhbr
 ```
 
 Dependency versions have not yet been worked out in detail, so you might encounter problems. For now, the dependencies used in the development environment are stored in `requirements.txt`. (This is a wider set of dependencies than is required for `pyhbr`, and includes the dependencies for all scripts in this repository.)
 
 Instead of using pip, it is possible to install the package on from this git repository. On Windows, using VS Code, follow these steps:
 
 1. Install Python 3 (>= 3.11)
```

### Comparing `pyhbr-0.0.2/pyproject.toml` & `pyhbr-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyhbr"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="John Scott", email="john.scott@uhbw.nhs.uk" },
 ]
 description = "Tools for bleeding/ischaemia risk estimation in PCI patients"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pyhbr-0.0.2/PKG-INFO` & `pyhbr-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyhbr
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools for bleeding/ischaemia risk estimation in PCI patients
 Project-URL: Homepage, https://github.com/jrs0/hbr_uhbw
 Author-email: John Scott <john.scott@uhbw.nhs.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -21,18 +21,18 @@
 
 # Python Package for Tool/Model Development
 
 This package will contain all the data analysis, model development, and other utilities developed as part of the BHF HBR project.
 
 ## Package Installation
 
-The intention is to host `pyhbr` on PyPI. For now, it is available on TestPyPi, and can be installed using:
+To install the latest version of the package, run
 
 ```bash
-pip install -i https://test.pypi.org/simple/ pyhbr
+pip install pyhbr
 ```
 
 Dependency versions have not yet been worked out in detail, so you might encounter problems. For now, the dependencies used in the development environment are stored in `requirements.txt`. (This is a wider set of dependencies than is required for `pyhbr`, and includes the dependencies for all scripts in this repository.)
 
 Instead of using pip, it is possible to install the package on from this git repository. On Windows, using VS Code, follow these steps:
 
 1. Install Python 3 (>= 3.11)
```

