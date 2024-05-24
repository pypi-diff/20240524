# Comparing `tmp/spectrafit-1.0.0b2.tar.gz` & `tmp/spectrafit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrafit-1.0.0b2.tar", max compression
+gzip compressed data, was "spectrafit-1.0.1.tar", max compression
```

## Comparing `spectrafit-1.0.0b2.tar` & `spectrafit-1.0.1.tar`

### file list

```diff
@@ -1,85 +1,34 @@
--rw-r--r--   0        0        0     6629 2023-04-02 20:33:57.052322 spectrafit-1.0.0b2/LICENSE
--rw-r--r--   0        0        0     9347 2023-04-02 20:33:57.052322 spectrafit-1.0.0b2/README.md
--rw-r--r--   0        0        0     5892 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0       83 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/__init__.py
--rw-r--r--   0        0        0       55 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/__init__.py
--rw-r--r--   0        0        0     2614 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/cmd_model.py
--rw-r--r--   0        0        0     1763 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/file_model.py
--rw-r--r--   0        0        0    11028 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/models_model.py
--rw-r--r--   0        0        0     6799 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/notebook_model.py
--rw-r--r--   0        0        0     4807 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/report_model.py
--rw-r--r--   0        0        0     3551 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/rixs_model.py
--rw-r--r--   0        0        0       50 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/test/__init__.py
--rw-r--r--   0        0        0     2218 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/test/test_cmd_model.py
--rw-r--r--   0        0        0     2919 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/test/test_file_model.py
--rw-r--r--   0        0        0      668 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/test/test_models_model.py
--rw-r--r--   0        0        0     3029 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/test/test_notebook_model.py
--rw-r--r--   0        0        0     2445 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/test/test_rixs_model.py
--rw-r--r--   0        0        0      411 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/test/test_tools_model.py
--rw-r--r--   0        0        0     3527 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/api/tools_model.py
--rw-r--r--   0        0        0      635 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/app/app.py
--rw-r--r--   0        0        0       55 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/app/test/__init__.py
--rw-r--r--   0        0        0      430 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/app/test/test_app.py
--rw-r--r--   0        0        0    52668 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/models.py
--rw-r--r--   0        0        0     5887 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plotting.py
--rw-r--r--   0        0        0       30 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/__init__.py
--rw-r--r--   0        0        0     2093 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/color_schemas.py
--rw-r--r--   0        0        0     1921 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/converter.py
--rw-r--r--   0        0        0     5000 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/data_converter.py
--rw-r--r--   0        0        0     4320 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/file_converter.py
--rw-r--r--   0        0        0    42680 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/notebook.py
--rw-r--r--   0        0        0     8688 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/pkl_converter.py
--rw-r--r--   0        0        0     6223 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/pkl_visualizer.py
--rw-r--r--   0        0        0     7621 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/rixs_converter.py
--rw-r--r--   0        0        0    22900 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/rixs_visualizer.py
--rw-r--r--   0        0        0       38 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/test/__init__.py
--rw-r--r--   0        0        0      895 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/test/test_color_schemas.py
--rw-r--r--   0        0        0    32789 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/test/test_converter.py
--rw-r--r--   0        0        0    21548 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/test/test_notebook.py
--rw-r--r--   0        0        0     3908 2023-04-02 20:33:57.076322 spectrafit-1.0.0b2/spectrafit/plugins/test/test_rixs_visualizer.py
--rw-r--r--   0        0        0    18960 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/report.py
--rw-r--r--   0        0        0     9573 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/spectrafit.py
--rw-r--r--   0        0        0       28 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/export/place_holder
--rw-r--r--   0        0        0       12 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/import/test_abc.txt
--rw-r--r--   0        0        0    38582 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/import/test_data.csv
--rw-r--r--   0        0        0    30647 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/import/test_data.txt
--rw-r--r--   0        0        0    61631 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/import/test_data_global.csv
--rw-r--r--   0        0        0     8420 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/import/test_data_global_2.csv
--rw-r--r--   0        0        0     7804 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/import/test_data_global_3.csv
--rw-r--r--   0        0        0     1657 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/fitting_input.toml
--rw-r--r--   0        0        0     2025 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/fitting_input.yaml
--rw-r--r--   0        0        0     2563 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_globalfit.json
--rw-r--r--   0        0        0     2831 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_1.json
--rw-r--r--   0        0        0     2854 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_10.json
--rw-r--r--   0        0        0     1263 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_11.json
--rw-r--r--   0        0        0     2832 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_2.json
--rw-r--r--   0        0        0     1416 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_3.json
--rw-r--r--   0        0        0      941 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_3.toml
--rw-r--r--   0        0        0     1056 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_3.yaml
--rw-r--r--   0        0        0     1056 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_3.yml
--rw-r--r--   0        0        0     1995 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_4.json
--rw-r--r--   0        0        0     1243 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_5.json
--rw-r--r--   0        0        0     2207 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_6.json
--rw-r--r--   0        0        0     2889 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_7.json
--rw-r--r--   0        0        0     2067 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_8.json
--rw-r--r--   0        0        0     2060 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_9.json
--rw-r--r--   0        0        0     3365 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_all_models.toml
--rw-r--r--   0        0        0     2274 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_global.json
--rw-r--r--   0        0        0     2050 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_global_0.json
--rw-r--r--   0        0        0     2101 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_input_global_1.json
--rw-r--r--   0        0        0     2136 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_missing_parameter_1.json
--rw-r--r--   0        0        0     2144 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_missing_parameter_2.json
--rw-r--r--   0        0        0     2136 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_missing_parameters_1.json
--rw-r--r--   0        0        0     2144 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/scripts/test_missing_parameters_2.json
--rw-r--r--   0        0        0    13811 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/test_input.py
--rw-r--r--   0        0        0    44161 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/test_models.py
--rw-r--r--   0        0        0     5034 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/test_plot.py
--rw-r--r--   0        0        0     5626 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/test_report.py
--rw-r--r--   0        0        0    14506 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/test/test_tools.py
--rw-r--r--   0        0        0    25819 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/tools.py
--rw-r--r--   0        0        0       43 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/utilities/__init__.py
--rw-r--r--   0        0        0       40 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/utilities/test/__init__.py
--rw-r--r--   0        0        0     2937 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/utilities/test/test_transformer.py
--rw-r--r--   0        0        0     1542 2023-04-02 20:33:57.080322 spectrafit-1.0.0b2/spectrafit/utilities/transformer.py
--rw-r--r--   0        0        0    12580 1970-01-01 00:00:00.000000 spectrafit-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1498 2024-05-24 16:59:00.265830 spectrafit-1.0.1/LICENSE
+-rw-r--r--   0        0        0     9807 2024-05-24 16:59:00.265830 spectrafit-1.0.1/README.md
+-rw-r--r--   0        0        0     6667 2024-05-24 16:59:00.301830 spectrafit-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      177 2024-05-24 16:59:00.301830 spectrafit-1.0.1/spectrafit/__init__.py
+-rw-r--r--   0        0        0       55 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/api/__init__.py
+-rw-r--r--   0        0        0     3146 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/api/cmd_model.py
+-rw-r--r--   0        0        0     1803 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/api/file_model.py
+-rw-r--r--   0        0        0    14561 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/api/models_model.py
+-rw-r--r--   0        0        0     6832 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/api/notebook_model.py
+-rw-r--r--   0        0        0    21563 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/api/pptx_model.py
+-rw-r--r--   0        0        0     5063 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/api/report_model.py
+-rw-r--r--   0        0        0     3855 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/api/rixs_model.py
+-rw-r--r--   0        0        0     3333 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/api/tools_model.py
+-rw-r--r--   0        0        0      634 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/app/app.py
+-rw-r--r--   0        0        0    60936 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/models.py
+-rw-r--r--   0        0        0     6497 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/plotting.py
+-rw-r--r--   0        0        0       30 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/plugins/__init__.py
+-rw-r--r--   0        0        0     5397 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/plugins/color_schemas.py
+-rw-r--r--   0        0        0     1922 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/plugins/converter.py
+-rw-r--r--   0        0        0     5158 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/plugins/data_converter.py
+-rw-r--r--   0        0        0     4479 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/plugins/file_converter.py
+-rw-r--r--   0        0        0    14394 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/plugins/img/SpectraFit.png
+-rw-r--r--   0        0        0    45803 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/plugins/notebook.py
+-rw-r--r--   0        0        0     8922 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/plugins/pkl_converter.py
+-rw-r--r--   0        0        0     6454 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/plugins/pkl_visualizer.py
+-rw-r--r--   0        0        0    15848 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/plugins/pptx_converter.py
+-rw-r--r--   0        0        0     7675 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/plugins/rixs_converter.py
+-rw-r--r--   0        0        0    22906 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/plugins/rixs_visualizer.py
+-rw-r--r--   0        0        0    35271 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/report.py
+-rw-r--r--   0        0        0     9669 2024-05-24 16:59:00.305830 spectrafit-1.0.1/spectrafit/spectrafit.py
+-rw-r--r--   0        0        0    28149 2024-05-24 16:59:00.309830 spectrafit-1.0.1/spectrafit/tools.py
+-rw-r--r--   0        0        0       43 2024-05-24 16:59:00.309830 spectrafit-1.0.1/spectrafit/utilities/__init__.py
+-rw-r--r--   0        0        0     1529 2024-05-24 16:59:00.309830 spectrafit-1.0.1/spectrafit/utilities/transformer.py
+-rw-r--r--   0        0        0    13212 1970-01-01 00:00:00.000000 spectrafit-1.0.1/PKG-INFO
```

### Comparing `spectrafit-1.0.0b2/README.md` & `spectrafit-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,64 +1,76 @@
 [![CI - Python Package](https://github.com/Anselmoo/spectrafit/actions/workflows/python-ci.yml/badge.svg?branch=main)](https://github.com/Anselmoo/spectrafit/actions/workflows/python-ci.yml)
 [![codecov](https://codecov.io/gh/Anselmoo/spectrafit/branch/main/graph/badge.svg?token=pNIMKwWsO2)](https://codecov.io/gh/Anselmoo/spectrafit)
 [![PyPI](https://img.shields.io/pypi/v/spectrafit?logo=PyPi&logoColor=yellow)](https://pypi.org/project/spectrafit/)
 [![Conda](https://img.shields.io/conda/v/conda-forge/spectrafit?label=Anaconda.org&logo=anaconda)](https://github.com/conda-forge/spectrafit-feedstock)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spectrafit?color=gree&logo=Python&logoColor=yellow)](https://pypi.org/project/spectrafit/)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Anselmoo/spectrafit/main.svg)](https://results.pre-commit.ci/latest/github/Anselmoo/spectrafit/main)
+[![doi](https://img.shields.io/badge/10.1021/acsomega.3c09262-blue?logo=DOI&logoColor=white)](https://pubs.acs.org/doi/full/10.1021/acsomega.3c09262)
 
 <p align="center">
 <img src="https://github.com/Anselmoo/spectrafit/blob/c5f7ee05e5610fb8ef4e237a88f62977b6f832e5/docs/images/spectrafit_synopsis.png?raw=true">
 </p>
 
 # SpectraFit
 
-`SpectraFit` is a tool for quick data fitting based on the regular
-expression of distribution and linear functions via command line or
-[Jupyter Notebook](https://jupyter.org). Furthermore, it can be also used as
-a module in existing python code. A previous version of `SpectraFit` was used
-for the following publication:
-
-- [Measurement of the Ligand Field Spectra of Ferrous and Ferric Iron Chlorides Using 2p3d RIXS](https://pubs.acs.org/doi/abs/10.1021/acs.inorgchem.7b00940)
-
-Now, it is completely rewritten and is more flexible. It is supporting all
-common ASCII-data formats and it runs on `Linux`, `Windows`, and `MacOS`.
+`SpectraFit` is a Python tool for quick data fitting based on the regular
+expression of distribution and linear functions via the command line (CMD) or
+[Jupyter Notebook](https://jupyter.org) It is designed to be easy to use and
+supports all common ASCII data formats. SpectraFit runs on **Linux**,
+**Windows**, and **MacOS**.
 
 ## Scope
 
 - Fitting of 2D data, also with multiple columns as _global fitting_
 - Using established and advanced solver methods
 - Extensibility of the fitting function
 - Guarantee traceability of the fitting results
 - Saving all results in a _SQL-like-format_ (`CSV`) for publications
 - Saving all results in a _NoSQL-like-format_ (`JSON`) for project management
 - Having an API interface for Graph-databases
 
+`SpectraFit` is a tool designed for researchers and scientists who require
+immediate data fitting to a model. It proves to be especially beneficial for
+individuals working with vast datasets or who need to conduct numerous fits
+within a limited time frame. `SpectraFit's` adaptability to various platforms
+and data formats makes it a versatile tool that caters to a broad spectrum of
+scientific applications.
+
 ## Installation
 
 via pip:
 
-```terminal
+```bash
 pip install spectrafit
 
 # with support for Jupyter Notebook
 
 pip install spectrafit[jupyter]
 
+# with support for the dashboard in the Jupyter Notebook
+
+pip install spectrafit[jupyter-dash]
+
+# with support to visualize pkl-files as graph
+
+pip install spectrafit[graph]
+
 # with all upcomming features
 
 pip install spectrafit[all]
 
 # Upgrade
 
 pip install spectrafit --upgrade
 ```
 
-via conda, see also [conda-forge](https://github.com/conda-forge/spectrafit-feedstock):
+via conda, see also
+[conda-forge](https://github.com/conda-forge/spectrafit-feedstock):
 
-```terminal
+```bash
 conda install -c conda-forge spectrafit
 
 # with support for Jupyter Notebook
 
 conda install -c conda-forge spectrafit-jupyter
 
 # with all upcomming features
@@ -88,19 +100,19 @@
 
 1. [Pandas](https://pandas.pydata.org/)
 2. [statsmodels](https://www.statsmodels.org/stable/index.html)
 3. [numdifftools](https://github.com/pbrod/numdifftools)
 4. [Matplotlib](https://matplotlib.org/) in combination with
    [Seaborn](https://seaborn.pydata.org/)
 
-```terminal
+```bash
 spectrafit data_file.txt -i input_file.json
 ```
 
-```terminal
+```bash
 usage: spectrafit [-h] [-o OUTFILE] [-i INPUT] [-ov] [-e0 ENERGY_START]
                   [-e1 ENERGY_STOP] [-s SMOOTH] [-sh SHIFT] [-c COLUMN COLUMN]
                   [-sep {       ,,,;,:,|, ,s+}] [-dec {.,,}] [-hd HEADER]
                   [-g {0,1,2}] [-auto] [-np] [-v] [-vb {0,1,2}]
                   infile
 
 Fast Fitting Program for ascii txt files.
@@ -161,29 +173,29 @@
                         table `printout`.
 ```
 
 ### Jupyter Notebook
 
 Open the `Jupyter Notebook` and run the following code:
 
-```terminal
+```bash
 spectrafit-jupyter
 ```
 
-or via Docker Image:
+or via Docker Image for `<cpu>` with `amd64` and `arm64`:
 
-```terminal
-docker pull ghcr.io/anselmoo/spectrafit:latest
-docker run -it -p 8888:8888 spectrafit:latest
+```bash
+docker pull ghcr.io/anselmoo/spectrafit-<cpu>:latest
+docker run -it -p 8888:8888 spectrafit-<cpu>:latest
 ```
 
 or just:
 
-```terminal
-docker run -p 8888:8888 ghcr.io/anselmoo/spectrafit:latest
+```bash
+docker run -p 8888:8888 ghcr.io/anselmoo/spectrafit-<cpu>:latest
 ```
 
 Next define your initial model and the reference data:
 
 ```python
 from spectrafit.plugins.notebook import SpectraFitNotebook
 import pandas as pd
```

### Comparing `spectrafit-1.0.0b2/spectrafit/api/cmd_model.py` & `spectrafit-1.0.1/spectrafit/api/cmd_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 """Reference model for the API of the command line interface."""
 
-
 from datetime import datetime
 from getpass import getuser
+from hashlib import sha256
 from socket import gethostname
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 from uuid import uuid4
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import HttpUrl
+from pydantic.functional_validators import field_validator
 from spectrafit import __version__
 from spectrafit.api.tools_model import AutopeakAPI
 from spectrafit.api.tools_model import DataPreProcessingAPI
 from spectrafit.api.tools_model import GlobalFittingAPI
 
 
 class DescriptionAPI(BaseModel):
     """Model for the description command line argument."""
 
     project_name: str = Field(
         default="FittingProject",
-        alias="projectNames",
+        alias="projectName",
         description="Name of the project",
     )
     project_details: str = Field(
         default=f"Fitting Project via SpectraFit v{__version__}",
         alias="projectDetails",
         description="Project details",
     )
     keywords: List[str] = Field(
         default=["spectra"], description="Keywords for the project"
     )
     authors: List[str] = Field(
         default=["authors"], description="Authors of the project"
     )
-    references: List[HttpUrl] = Field(
+    references: List[str] = Field(
         default=["https://github.com/Anselmoo/spectrafit"],
         alias="refs",
         description="References for the project",
     )
+    metadata: Optional[Union[Dict[Any, Any], List[Any]]] = Field(
+        default=None, description="Metadata for the project"
+    )
+    license: str = "BSD-3-Clause"
     version: str = __version__
-    host_info: str = f"{getuser()}@{gethostname()}"
+    host_info: str = sha256(f"{getuser()}@{gethostname()}".encode()).hexdigest()
     timestamp: str = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     id_: str = Field(
         default=str(uuid4()), alias="id", description="Unique ID of the project"
     )
 
+    @field_validator("references")
+    @classmethod
+    def check_references(cls, v: List[str]) -> Optional[List[str]]:
+        """Check if the list of references have valid URLs."""
+        return [str(HttpUrl(url)) for url in v]
+
 
 class CMDModelAPI(BaseModel):
     """Model for the model command line argument."""
 
     infile: str
     outfile: str = Field(default="spectrafit_results")
     input: str = Field(default="fitting_input.toml")
```

### Comparing `spectrafit-1.0.0b2/spectrafit/api/file_model.py` & `spectrafit-1.0.1/spectrafit/api/file_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Callable
 from typing import List
 from typing import Optional
 from typing import Union
 
 from pydantic import BaseModel
 from pydantic import Field
-from pydantic import validator
+from pydantic.functional_validators import field_validator
 
 
 class DataFileAPI(BaseModel):
     """Definition of a data file."""
 
     skiprows: Optional[int] = Field(
         default=None,
@@ -39,22 +39,22 @@
         description="Column headers to use.",
     )
     file_suffixes: List[str] = Field(
         ...,
         description="File suffixes to use.",
     )
 
-    @validator("delimiter")
+    @field_validator("delimiter")
     @classmethod
     def check_delimiter(cls, v: str) -> Optional[str]:
         """Check if the delimiter is valid."""
         if v in {" ", "\t", ",", ";", "|", r"\s+"}:
             return v
         raise ValueError(f" {v} is not a valid delimiter.")
 
-    @validator("comment")
+    @field_validator("comment")
     @classmethod
     def check_comment(cls, v: str) -> Optional[str]:
         """Check if the comment marker is valid."""
         if v is None or v in {"#", "%"}:
             return v
         raise ValueError(f" {v} is not a valid comment marker.")
```

### Comparing `spectrafit-1.0.0b2/spectrafit/api/models_model.py` & `spectrafit-1.0.1/spectrafit/api/models_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Reference model for the API of the models distributions."""
 
-
 from typing import Callable
 from typing import List
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 
@@ -158,14 +157,26 @@
     max: Optional[float] = Field(default=None, description="Maximum sigma.")
     min: Optional[int] = Field(default=None, description="Minimum sigma.")
     vary: bool = Field(default=True, description="Vary the sigma.")
     value: Optional[float] = Field(default=None, description="Initial sigma value.")
     expr: Optional[str] = Field(default=None, description=__description__)
 
 
+class CoefficientAPI(BaseModel):
+    """Definition of the Coefficient of the models distributions."""
+
+    max: Optional[float] = Field(default=None, description="Maximum coefficient.")
+    min: Optional[int] = Field(default=None, description="Minimum coefficient.")
+    vary: bool = Field(default=True, description="Vary the coefficient.")
+    value: Optional[float] = Field(
+        default=None, description="Initial coefficient value."
+    )
+    expr: Optional[str] = Field(default=None, description=__description__)
+
+
 class PseudovoigtAPI(BaseModel):
     """Definition of the Pseudovoigt of the models distributions."""
 
     amplitude: AmplitudeAPI = AmplitudeAPI()
     center: CenterAPI = CenterAPI()
     fwhmg: FwhmgAPI = FwhmgAPI()
     fwhml: FwhmlAPI = FwhmlAPI()
@@ -276,14 +287,90 @@
     """Definition of the cumulative Voigt of the models distributions."""
 
     center: CenterAPI = CenterAPI()
     fwhmv: FwhmvAPI = FwhmvAPI()
     gamma: GammaAPI = GammaAPI()
 
 
+class Polynomia2API(BaseModel):
+    """Definition of the second order polynomial of the models distributions."""
+
+    coefficient0: CoefficientAPI = CoefficientAPI()
+    coefficient1: CoefficientAPI = CoefficientAPI()
+    coefficient2: CoefficientAPI = CoefficientAPI()
+
+
+class Polynomia3API(BaseModel):
+    """Definition of the third order polynomial of the models distributions."""
+
+    coefficient0: CoefficientAPI = CoefficientAPI()
+    coefficient1: CoefficientAPI = CoefficientAPI()
+    coefficient2: CoefficientAPI = CoefficientAPI()
+    coefficient3: CoefficientAPI = CoefficientAPI()
+
+
+class SkewnessAPI(BaseModel):
+    """Definition of the skewness of the models distributions."""
+
+    max: Optional[float] = Field(default=None, description="Maximum skewness.")
+    min: Optional[int] = Field(default=None, description="Minimum skewness.")
+    vary: bool = Field(default=True, description="Vary the skewness.")
+    value: Optional[float] = Field(default=None, description="Initial skewness value.")
+    expr: Optional[str] = Field(default=None, description=__description__)
+
+
+class KurtosisAPI(BaseModel):
+    """Definition of the kurtosis of the models distributions."""
+
+    max: Optional[float] = Field(default=None, description="Maximum kurtosis.")
+    min: Optional[int] = Field(default=None, description="Minimum kurtosis.")
+    vary: bool = Field(default=True, description="Vary the kurtosis.")
+    value: Optional[float] = Field(default=None, description="Initial kurtosis value.")
+    expr: Optional[str] = Field(default=None, description=__description__)
+
+
+class Pearson1API(BaseModel):
+    """Definition of the pearson type I of the models distributions."""
+
+    amplitude: AmplitudeAPI = AmplitudeAPI()
+    center: CenterAPI = CenterAPI()
+    sigma: SigmaAPI = SigmaAPI()
+    exponent: ExponentAPI = ExponentAPI()
+
+
+class Pearson2API(BaseModel):
+    """Definition of the pearson type II of the models distributions."""
+
+    amplitude: AmplitudeAPI = AmplitudeAPI()
+    center: CenterAPI = CenterAPI()
+    sigma: SigmaAPI = SigmaAPI()
+    exponent: ExponentAPI = ExponentAPI()
+
+
+class Pearson3API(BaseModel):
+    """Definition of the pearson type III of the models distributions."""
+
+    amplitude: AmplitudeAPI = AmplitudeAPI()
+    center: CenterAPI = CenterAPI()
+    sigma: SigmaAPI = SigmaAPI()
+    exponent: ExponentAPI = ExponentAPI()
+    skewness: SkewnessAPI = SkewnessAPI()
+
+
+class Pearson4API(BaseModel):
+    """Definition of the pearson type IV of the models distributions."""
+
+    amplitude: AmplitudeAPI = AmplitudeAPI()
+    center: CenterAPI = CenterAPI()
+    sigma: SigmaAPI = SigmaAPI()
+    exponent: ExponentAPI = ExponentAPI()
+    skewness: SkewnessAPI = SkewnessAPI()
+    kurtosis: KurtosisAPI = KurtosisAPI()
+
+
 class DistributionModelAPI(BaseModel):
     """Definition of the models distributions."""
 
     gaussian: GaussianAPI = GaussianAPI()
     lorentzian: LorentzianAPI = LorentzianAPI()
     voigt: VoigtAPI = VoigtAPI()
     pseudovoigt: PseudovoigtAPI = PseudovoigtAPI()
@@ -294,14 +381,20 @@
     erf: ErfAPI = ErfAPI()
     heaviside: HeavisideAPI = HeavisideAPI()
     atan: AtanAPI = AtanAPI()
     log: LogAPI = LogAPI()
     cgaussian: CGaussianAPI = CGaussianAPI()
     clorentzian: CLorentzianAPI = CLorentzianAPI()
     cvoigt: CVoigtAPI = CVoigtAPI()
+    polynom2: Polynomia2API = Polynomia2API()
+    polynom3: Polynomia3API = Polynomia3API()
+    pearson1: Pearson1API = Pearson1API()
+    pearson2: Pearson2API = Pearson2API()
+    pearson3: Pearson3API = Pearson3API()
+    pearson4: Pearson4API = Pearson4API()
 
 
 class ConfIntervalAPI(BaseModel):
     """Definition of Confidence Interval Function."""
 
     p_names: Optional[List[str]] = Field(
         default=None, description="List of parameters names."
```

### Comparing `spectrafit-1.0.0b2/spectrafit/api/notebook_model.py` & `spectrafit-1.0.1/spectrafit/api/notebook_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Reference model for the API of the Jupyter Notebook interface."""
 
-
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 from _plotly_utils.colors.carto import Burg
 from _plotly_utils.colors.carto import Purp_r
 from _plotly_utils.colors.carto import Teal_r
 from _plotly_utils.colors.qualitative import Plotly as PlotlyColors
 from pydantic import BaseModel
 from pydantic import Field
-from pydantic import validator
+from pydantic.functional_validators import field_validator
 
 
 class XAxisAPI(BaseModel):
     """Defintion of the X-Axis of the plotly figure."""
 
     name: str = Field(default="Energy", description="Name of the x-axis of the plot.")
     unit: Optional[str] = Field(
@@ -125,15 +124,15 @@
     color: str = Field(default="black", description="Color of the text.")
     grid: str = Field(default="lightgrey", description="Color of the grid.")
     line: str = Field(default="black", description="Color of the bottom and side line.")
     zero_line: str = Field(default="grey", description="Color of the zero line.")
     ticks: str = Field(default="black", description="Color of the ticks.")
     font: str = Field(default="black", description="Font color of the plot.")
 
-    @validator(
+    @field_validator(
         "paper",
         "layout",
         "grid",
         "line",
         "zero_line",
         "ticks",
         "font",
```

### Comparing `spectrafit-1.0.0b2/spectrafit/api/report_model.py` & `spectrafit-1.0.1/spectrafit/api/report_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Reference model for the API of the Jupyter Notebook report."""
+
 from typing import Any
 from typing import Dict
 from typing import Hashable
 from typing import List
 from typing import Union
 
 from dtale import __version__ as dtale_version
@@ -10,24 +11,25 @@
 from itables import __version__ as itables_version
 from lmfit import __version__ as lmfit_version
 from numdifftools import __version__ as numdifftools_version
 from numpy import __version__ as numpy_version
 from pandas import __version__ as pandas_version
 from plotly import __version__ as plotly_version
 from pydantic import BaseModel
+from pydantic import ConfigDict
 from pydantic import Field
 from pydantic import __version__ as pydantic_version
 from scipy import __version__ as scipy_version
 from sklearn import __version__ as sklearn_version
 from spectrafit.api.cmd_model import DescriptionAPI
 from spectrafit.api.tools_model import DataPreProcessingAPI
 from statsmodels import __version__ as statsmodels_version
 
 
-class CreditsAPI(BaseModel, allow_mutation=False):
+class CreditsAPI(BaseModel):
     """Credits API model."""
 
     dtale: str = f"dtale v{dtale_version}"
     emcee: str = f"emcee v{emcee_version}"
     itables: str = f"itables v{itables_version}"
     lmfit: str = f"lmfit v{lmfit_version}"
     numdifftools: str = f"numdifftools v{numdifftools_version}"
@@ -50,14 +52,18 @@
     confidence_interval: Union[bool, Dict[str, Any]] = Field(
         ...,
         description="Settings for the confidence interval calculation",
     )
     configurations: Dict[str, Any] = Field(
         ..., description="Settings for the fitting configuration"
     )
+    settings_solver_models: Dict[str, Any] = Field(
+        ...,
+        description="Settings for the solver models including minimizer and optimizer",
+    )
 
 
 class InputAPI(BaseModel):
     """Input API for the report endpoint."""
 
     description: DescriptionAPI = DescriptionAPI()
     credits: CreditsAPI = CreditsAPI()
@@ -97,14 +103,18 @@
         ...,
         description="Variables with their initial, optimized and optional error values",
     )
     errorbars: Dict[str, Any] = Field(
         default={},
         description="Error bar comment if values reach initial value or boundary",
     )
+    computional: Dict[str, Any] = Field(
+        ...,
+        description="Computional information like number of function evaluations",
+    )
 
 
 class OutputAPI(BaseModel):
     """Output API for the report endpoint."""
 
     df_org: Dict[Hashable, Any] = Field(
         ...,
@@ -114,19 +124,15 @@
         ...,
         description="DataFrame of the fitted data via 'records' orient",
     )
     df_pre: Dict[Hashable, Any] = Field(
         default={},
         description="DataFrame of the pre-processed data via 'records' orient",
     )
-
-    class Config:
-        """Config for the OutputAPI of arbitary types."""
-
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
 
 class ReportAPI(BaseModel):
     """Definition of the report model."""
 
     input: InputAPI = Field(
         ...,
```

### Comparing `spectrafit-1.0.0b2/spectrafit/api/rixs_model.py` & `spectrafit-1.0.1/spectrafit/api/rixs_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Reference model for the API of the Jupyter Notebook interface."""
 
-
+from typing import Any
 from typing import Optional
 from typing import Tuple
 
-import numpy as np
-
-from numpy.typing import NDArray
 from pydantic import BaseModel
+from pydantic import ConfigDict
 from pydantic import Field
 
 
 class XAxisAPI(BaseModel):
     """Defintion of the X-Axis of the plotly figure."""
 
     name: str = Field(
@@ -68,50 +66,44 @@
         default=(3, 1), description="Ratio of the XAS plot."
     )
 
 
 class RIXSModelAPI(BaseModel):
     """Definition of the RIXS model."""
 
-    incident_energy: NDArray[np.float64] = Field(
+    incident_energy: Any = Field(
         ..., description="Incident energy values."
-    )
-    emission_energy: NDArray[np.float64] = Field(
+    )  # Should be NDArray[np.float64] but that's not supported for 3.8
+    emission_energy: Any = Field(
         ..., description="Emission energy values."
-    )
-    rixs_map: NDArray[np.float64] = Field(..., description="RIXS map values.")
-
-    class Config:
-        """Configurations for the RIXSModelAPI class."""
-
-        arbitrary_types_allowed = True
+    )  # Should be NDArray[np.float64] but that's not supported for 3.8
+    rixs_map: Any = Field(
+        ..., description="RIXS map values."
+    )  # Should be NDArray[np.float64] but that's not supported for 3.8
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
 
 class RIXSPlotAPI(BaseModel):
     """Definition of the plotly figure."""
 
-    incident_energy: NDArray[np.float64] = Field(
+    incident_energy: Any = Field(
         ..., description="Incident energy values."
-    )
-    emission_energy: NDArray[np.float64] = Field(
+    )  # Should be NDArray[np.float64] but that's not supported for 3.8
+    emission_energy: Any = Field(
         ..., description="Emission energy values."
-    )
-    emission_intensity: NDArray[np.float64] = Field(
+    )  # Should be NDArray[np.float64] but that's not supported for 3.8
+    emission_intensity: Any = Field(
         ..., description="Emission intensity values (RIXS), which has to be a 2D array."
-    )
-    energy_loss: Optional[NDArray[np.float64]] = Field(
+    )  # Should be NDArray[np.float64] but that's not supported for 3.8
+    energy_loss: Optional[Any] = Field(
         default=None, description="Energy loss values."
-    )
-    energy_loss_intensity: Optional[NDArray[np.float64]] = Field(
+    )  # Should be NDArray[np.float64] but that's not supported for 3.8
+    energy_loss_intensity: Optional[Any] = Field(
         default=None,
         description="Energy loss intensity values (XES), which has to be a 2D array.",
-    )
+    )  # Should be NDArray[np.float64] but that's not supported for 3.8
     x_axis: XAxisAPI = XAxisAPI()
     y_axis: YAxisAPI = YAxisAPI()
     z_axis: ZAxisAPI = ZAxisAPI()
     main_title: MainTitleAPI = MainTitleAPI()
     size_ratio: SizeRatioAPI = SizeRatioAPI()
-
-    class Config:
-        """Configurations for the RIXSPlotAPI class."""
-
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
```

### Comparing `spectrafit-1.0.0b2/spectrafit/api/tools_model.py` & `spectrafit-1.0.1/spectrafit/api/tools_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,70 @@
 """Reference model for the API of the SpectraFit tools."""
 
-
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 from pydantic import BaseModel
-from pydantic import Extra
+from pydantic import ConfigDict
 from pydantic import Field
 
 
 class AutopeakAPI(BaseModel):
     """Definition of the auto detection of peak command line argument.
 
     The auto detection of peaks is performed by the SpectraFit tools. Here is listed the
     set of parameters that are used to control the auto detection of peaks according to
     the following `scipy.signal.find_peaks` -module; source:
     [https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.find_peaks.html](
     https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.find_peaks.html
     )
     """
 
-    model_type: Optional[str] = None
+    modeltype: Optional[str] = None
     height: Optional[List[float]] = None
     threshold: Optional[List[float]] = None
     distance: Optional[int] = None
     prominence: Optional[List[float]] = None
     width: Optional[List[float]] = None
     wlen: Optional[int] = None
     rel_height: Optional[float] = None
     plateau_size: Optional[float] = None
-
-    class Config:
-        """Activate the Validation Error Raise."""
-
-        extra = Extra.forbid
-        validate_assignment = True
+    model_config = ConfigDict(extra="forbid", validate_assignment=True)
 
 
 class DataPreProcessingAPI(BaseModel):
     """Definition of the data preprocessing command line argument."""
 
     oversampling: bool = Field(
         default=False,
         description="Oversampling the spectra by using factor of 5; default to False.",
     )
     energy_start: Optional[float] = Field(
         default=None,
-        dtypes=float,
         description="Start energy of the spectra; default to None.",
     )
     energy_stop: Optional[float] = Field(
         default=None,
-        dtypes=float,
         description="Stop energy of the spectra; default to None.",
     )
     smooth: int = Field(
         default=0,
         ge=0,
-        dtypes=int,
         description="Smoothing level of the spectra; default to 0.",
     )
     shift: float = Field(
         default=0,
-        dtypes=float,
         description="Shift the energy axis; default to 0.",
     )
     column: List[Union[int, str]] = Field(
-        min_items=1,
+        min_length=1,
         default=[0, 1],
-        dtypes=[int, str],
         description="Column of the data.",
     )
 
 
 class GlobalFittingAPI(BaseModel):
     """Definition of the global fitting routine."""
 
@@ -86,15 +75,15 @@
     """Definition of the solver of SpectraFit."""
 
     minimizer: Dict[str, Any] = Field(
         default={"nan_policy": "propagate", "calc_covar": True},
         description="Minimizer options",
     )
     optimizer: Dict[str, Any] = Field(
-        default={"max_nfev": 1000, "method": "leastsq"},
+        default={"max_nfev": None, "method": "leastsq"},
         description="Optimzer options",
     )
 
 
 class GeneralSolverModelsAPI(BaseModel):
     """Definition of the general solver of SpectraFit.
 
@@ -105,14 +94,14 @@
     """
 
     global_: int = GlobalFittingAPI().global_
     minimizer: Dict[str, Any] = SolverModelsAPI().minimizer
     optimizer: Dict[str, Any] = SolverModelsAPI().optimizer
 
 
-class ColumnNamesAPI(BaseModel, allow_mutation=False):
+class ColumnNamesAPI(BaseModel):
     """Definition of the column names of the exported model."""
 
     energy: str = "energy"
     intensity: str = "intensity"
     residual: str = "residual"
     fit: str = "fit"
```

### Comparing `spectrafit-1.0.0b2/spectrafit/app/app.py` & `spectrafit-1.0.1/spectrafit/app/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Starting jupyter lab as a app."""
 
-
 import sys
 
 from jupyterlab.labapp import main
 
 
 def jupyter() -> None:
     """Run jupyter lab as app in the absence of token."""
```

### Comparing `spectrafit-1.0.0b2/spectrafit/models.py` & `spectrafit-1.0.1/spectrafit/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Minimization models for curve fitting."""
+
 from collections import defaultdict
 from dataclasses import dataclass
 from math import log
 from math import pi
 from math import sqrt
 from typing import Any
 from typing import Dict
@@ -503,20 +504,242 @@
         return np.array(
             amplitude
             * 0.5
             * (1 + erf((x - center) / (sigma * np.sqrt(2.0))))
             * np.exp(-(((x - center) / gamma) ** 2))
         )
 
+    @staticmethod
+    def polynom2(
+        x: NDArray[np.float64],
+        coefficient0: float = 1.0,
+        coefficient1: float = 1.0,
+        coefficient2: float = 1.0,
+    ) -> NDArray[np.float64]:
+        """Return a 1-dimensional second order polynomial function.
+
+        $$
+        f(x) = c_2 x^2 + c_1 x + c_0
+        $$
+
+        Args:
+            x (NDArray[np.float64]): `x`-values of the data
+            coefficient0 (float, optional): Zeroth coefficient of the
+                 polynomial function. Defaults to 1.0.
+            coefficient1 (float, optional): First coefficient of the
+                 polynomial function. Defaults to 1.0.
+            coefficient2 (float, optional): Second coefficient of the
+                 polynomial function. Defaults to 1.0.
+
+        Returns:
+            NDArray[np.float64]: Third order polynomial function of `x`
+        """
+        return np.array(coefficient0 + coefficient1 * x + coefficient2 * x**2)
+
+    @staticmethod
+    def polynom3(
+        x: NDArray[np.float64],
+        coefficient0: float = 1.0,
+        coefficient1: float = 1.0,
+        coefficient2: float = 1.0,
+        coefficient3: float = 1.0,
+    ) -> NDArray[np.float64]:
+        """Return a 1-dimensional third order polynomial function.
+
+        $$
+        f(x) = c_3 x^3 + c_2 x^2 + c_1 x + c_0
+        $$
+
+        Args:
+            x (NDArray[np.float64]): `x`-values of the data
+            coefficient0 (float, optional): Zeroth coefficient of the
+                 polynomial function. Defaults to 1.0.
+            coefficient1 (float, optional): First coefficient of the
+                 polynomial function. Defaults to 1.0.
+            coefficient2 (float, optional): Second coefficient of the
+                 polynomial function. Defaults to 1.0.
+            coefficient3 (float, optional): Third coefficient of the
+                 polynomial function. Defaults to 1.0.
+
+        Returns:
+            NDArray[np.float64]: Third order polynomial function of `x`
+        """
+        return np.array(
+            coefficient0 + coefficient1 * x + coefficient2 * x**2 + coefficient3 * x**3
+        )
+
+    @staticmethod
+    def pearson1(
+        x: NDArray[np.float64],
+        amplitude: float = 1.0,
+        center: float = 0.0,
+        sigma: float = 1.0,
+        exponent: float = 1.0,
+    ) -> NDArray[np.float64]:
+        r"""Return a 1-dimensional Pearson type I distribution.
+
+        $$
+        f(x) = \frac{A}{\sigma \sqrt{2 \pi}} \left[1 + \frac{(x - c)^2}{\sigma^2}
+        \right]^{-\frac{1}{\nu}}
+        $$
+
+        Args:
+            x (NDArray[np.float64]): `x`-values of the data.
+            amplitude (float, optional): Amplitude of the Pearson type I function.
+                    Defaults to 1.0.
+            center (float, optional): Center of the Pearson type I function.
+                 Defaults to 0.0.
+            sigma (float, optional): Sigma of the Pearson type I function.
+                 Defaults to 1.0.
+            exponent (float, optional): Exponent of the Pearson type I function.
+                 Defaults to 1.0.
+
+        Returns:
+            NDArray[np.float64]: Pearson type I function of `x` given.
+        """
+        return np.array(
+            amplitude
+            / (sigma * np.sqrt(2 * np.pi))
+            * np.power(1 + ((x - center) / sigma) ** 2, -1 / exponent)
+        )
+
+    @staticmethod
+    def pearson2(
+        x: NDArray[np.float64],
+        amplitude: float = 1.0,
+        center: float = 0.0,
+        sigma: float = 1.0,
+        exponent: float = 1.0,
+    ) -> NDArray[np.float64]:
+        r"""Return a 1-dimensional Pearson type II distribution.
+
+        $$
+        f(x) = \frac{A}{\sigma \sqrt{2 \pi}} \left[1 + \frac{(x - c)^2}{2 \sigma^2}
+        \right]^{-\nu}
+        $$
+
+        Args:
+            x (NDArray[np.float64]): `x`-values of the data.
+            amplitude (float, optional): Amplitude of the Pearson type II function.
+                    Defaults to 1.0.
+            center (float, optional): Center of the Pearson type II function.
+                 Defaults to 0.0.
+            sigma (float, optional): Sigma of the Pearson type II function.
+                 Defaults to 1.0.
+            exponent (float, optional): Exponent of the Pearson type II function.
+                 Defaults to 1.0.
+
+        Returns:
+            NDArray[np.float64]: Pearson type II function of `x` given.
+        """
+        return np.array(
+            amplitude
+            / (sigma * np.sqrt(2 * pi))
+            * np.power(1 + ((x - center) / (2 * sigma)) ** 2, -exponent)
+        )
+
+    @staticmethod
+    def pearson3(
+        x: NDArray[np.float64],
+        amplitude: float = 1.0,
+        center: float = 0.0,
+        sigma: float = 1.0,
+        exponent: float = 1.0,
+        skewness: float = 0.0,
+    ) -> NDArray[np.float64]:
+        r"""Return a 1-dimensional Pearson type III distribution.
+
+        $$
+        f(x) = \frac{A}{\sigma \sqrt{2 \pi}} \left[1 + \frac{(x - c)^2}{2 \sigma^2}
+        \right]^{-\nu} \left[1 + \frac{\gamma}{\nu}
+        \frac{x - c}{\sigma} \right]^{-\nu - 1}
+        $$
+
+        Args:
+            x (NDArray[np.float64]): `x`-values of the data.
+            amplitude (float, optional): Amplitude of the Pearson type III function.
+                    Defaults to 1.0.
+            center (float, optional): Center of the Pearson type III function.
+                 Defaults to 0.0.
+            sigma (float, optional): Sigma of the Pearson type III function.
+                 Defaults to 1.0.
+            exponent (float, optional): Exponent of the Pearson type III function.
+                 Defaults to 1.0.
+            skewness (float, optional): Skewness of the Pearson type III function.
+                 Defaults to 0.0.
+
+        Returns:
+            NDArray[np.float64]: Pearson type III function of `x` given.
+        """
+        return np.array(
+            amplitude
+            / (sigma * np.sqrt(2 * pi))
+            * np.power(1 + ((x - center) / (2 * sigma)) ** 2, -exponent)
+            * np.power(
+                1 + (skewness / exponent) * ((x - center) / sigma), -exponent - 1
+            )
+        )
+
+    @staticmethod
+    def pearson4(
+        x: NDArray[np.float64],
+        amplitude: float = 1.0,
+        center: float = 0.0,
+        sigma: float = 1.0,
+        exponent: float = 1.0,
+        skewness: float = 0.0,
+        kurtosis: float = 0.0,
+    ) -> NDArray[np.float64]:
+        r"""Return a 1-dimensional Pearson type IV distribution.
+
+        $$
+        f(x) = \frac{A}{\sigma \sqrt{2 \pi}} \left[1 + \frac{(x - c)^2}{2 \sigma^2}
+        \right]^{-\nu} \left[1 + \frac{\gamma}{\nu}
+        \frac{x - c}{\sigma} \right]^{-\nu - 1}
+        \left[1 + \frac{\delta}{\nu}
+        \left(\frac{x - c}{\sigma}\right)^2 \right]^{-\nu - 1/2}
+        $$
+
+        Args:
+            x (NDArray[np.float64]): `x`-values of the data.
+            amplitude (float, optional): Amplitude of the Pearson type IV function.
+                    Defaults to 1.0.
+            center (float, optional): Center of the Pearson type IV function.
+                 Defaults to 0.0.
+            sigma (float, optional): Sigma of the Pearson type IV function.
+                 Defaults to 1.0.
+            exponent (float, optional): Exponent of the Pearson type IV function.
+                 Defaults to 1.0.
+            skewness (float, optional): Skewness of the Pearson type IV function.
+                 Defaults to 0.0.
+            kurtosis (float, optional): Kurtosis of the Pearson type IV function.
+                 Defaults to 0.0.
+
+        Returns:
+            NDArray[np.float64]: Pearson type IV function of `x` given.
+        """
+        return np.array(
+            amplitude
+            / (sigma * np.sqrt(2 * pi))
+            * np.power(1 + ((x - center) / (2 * sigma)) ** 2, -exponent)
+            * np.power(
+                1 + (skewness / exponent) * ((x - center) / sigma), -exponent - 1
+            )
+            * np.power(
+                1 + (kurtosis / exponent) * ((x - center) / sigma) ** 2,
+                -exponent - 1 / 2,
+            )
+        )
+
 
 @dataclass(frozen=True)
 class ReferenceKeys:
     """Reference keys for model fitting and peak detection."""
 
-    __models__ = list(DistributionModelAPI.schema()["properties"].keys())
+    __models__ = list(DistributionModelAPI.model_json_schema()["properties"].keys())
 
     __automodels__ = [
         "gaussian",
         "lorentzian",
         "voigt",
         "pseudovoigt",
     ]
@@ -524,15 +747,15 @@
     def model_check(self, model: str) -> None:
         """Check if model is available.
 
         Args:
             model (str): Model name.
 
         Raises:
-            KeyError: If the model is not supported.
+            NotImplementedError: If the model is not implemented.
         """
         if model.split("_")[0] not in self.__models__:
             raise NotImplementedError(f"{model} is not supported!")
 
     def automodel_check(self, model: str) -> None:
         """Check if model is available.
 
@@ -1000,17 +1223,17 @@
             )
 
     def define_parameters_auto(self) -> None:
         """Auto define the model parameters for local fitting."""
         positions, properties = self.__autodetect__()
         if (
             not isinstance(self.args["autopeak"], bool)
-            and "model_type" in self.args["autopeak"]
+            and "modeltype" in self.args["autopeak"]
         ):
-            _model = self.args["autopeak"]["model_type"].lower()
+            _model = self.args["autopeak"]["modeltype"].lower()
             ReferenceKeys().automodel_check(model=_model)
             models = _model
         else:
             models = "gaussian"
 
         if models == "gaussian":
             for i, (_cent, _amp, _fhmw) in enumerate(
@@ -1226,20 +1449,20 @@
             key_3 (str): The key of the third level of the input dictionary.
             value_3 (Dict[str, Any]): The value of the third level of the input
                  dictionary.
         """
         if col_i:
             if key_3 != "amplitude":
                 self.params.add(
-                    f"{key_2}_{key_3}_{key_1}_{col_i+1}",
+                    f"{key_2}_{key_3}_{key_1}_{col_i + 1}",
                     expr=f"{key_2}_{key_3}_{key_1}_1",
                 )
             else:
                 self.params.add(
-                    f"{key_2}_{key_3}_{key_1}_{col_i+1}",
+                    f"{key_2}_{key_3}_{key_1}_{col_i + 1}",
                     **value_3,
                 )
 
         else:
             self.params.add(f"{key_2}_{key_3}_{key_1}_1", **value_3)
 
     def define_parameters_global_pre(self) -> None:
@@ -1278,16 +1501,16 @@
 
         Args:
             df (pd.DataFrame): DataFrame containing the input data (`x` and `data`).
             args (Dict[str, Any]): The input file arguments as a dictionary with
                  additional information beyond the command line arguments.
         """
         super().__init__(df=df, args=args)
-        self.args_solver = SolverModelsAPI(**args).dict()
-        self.args_global = GlobalFittingAPI(**args).dict()
+        self.args_solver = SolverModelsAPI(**args).model_dump()
+        self.args_global = GlobalFittingAPI(**args).model_dump()
         self.params = self.return_params
 
     def __call__(self) -> Tuple[Minimizer, Any]:
         """Solve the fitting model.
 
         Returns:
             Tuple[Minimizer, Any]: Minimizer class and the fitting results.
@@ -1303,15 +1526,19 @@
             minimizer = Minimizer(
                 self.solve_local_fitting,
                 params=self.params,
                 fcn_args=(self.x, self.data),
                 **self.args_solver["minimizer"],
             )
 
-        return (minimizer, minimizer.minimize(**self.args_solver["optimizer"]))
+        result = minimizer.minimize(
+            **self.args_solver["optimizer"],
+        )
+        self.args_solver["optimizer"]["max_nfev"] = minimizer.max_nfev
+        return minimizer, result
 
     @staticmethod
     def solve_local_fitting(
         params: Dict[str, Parameters],
         x: NDArray[np.float64],
         data: NDArray[np.float64],
     ) -> NDArray[np.float64]:
```

### Comparing `spectrafit-1.0.0b2/spectrafit/plotting.py` & `spectrafit-1.0.1/spectrafit/plotting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,109 +1,124 @@
-"""Plotting of the fit results."""
+"""Plotting of the fit results.
+
+!!! info "About the Font Cache"
+
+    For avoiding problems with the font cache, the font cache is rebuilt at the
+    beginning of the program. This can take a few seconds. If you want to avoid
+    this, you can comment out the line `matplotlib.font_manager._rebuild()` in
+    the `plotting.py` file.
+"""
+
 from typing import Any
 from typing import Dict
+from typing import Optional
 
+import matplotlib.font_manager
 import matplotlib.pyplot as plt
 import pandas as pd
 import seaborn as sns
 
 from matplotlib.widgets import MultiCursor
 from spectrafit.api.tools_model import ColumnNamesAPI
 
 
+matplotlib.font_manager.findfont("serif", rebuild_if_missing=True)
+
 sns.set_theme(style="whitegrid")
 color = sns.color_palette("Paired")
 
 
 class PlotSpectra:
     """Plotting of the fit results."""
 
-    def __init__(self, df: pd.DataFrame, args: Dict[str, Any]) -> None:
+    def __init__(self, df: pd.DataFrame, args: Optional[Dict[str, Any]] = None) -> None:
         """Initialize the PlotSpectra class.
 
         Args:
             df (pd.DataFrame): DataFrame containing the input data (`x` and `data`),
                  as well as the best fit and the corresponding residuum. Hence, it will
                  be extended by the single contribution of the model.
-            args (Dict[str, Any]): The input file arguments as a dictionary with
-                 additional information beyond the command line arguments.
+            args (Dict[str, Any], optional): The input file arguments as a dictionary
+                 with additional information beyond the command line arguments. Only
+                 needed for global fitting. Defaults to None.
         """
         self.df = df
         self.args = args
 
     def __call__(self) -> None:
         """Plot the data and the fit."""
-        if not self.args["noplot"]:
-            if self.args["global_"]:
-                self.plot_global_spectra()
-            else:
-                self.plot_local_spectra()
+        if self.args is not None:
+            if not self.args["noplot"]:
+                if self.args["global_"]:
+                    self.plot_global_spectra()
+                else:
+                    self.plot_local_spectra()
+            plt.show()
 
     def plot_global_spectra(self) -> None:
         """Plot spectra for global fitting.
 
         !!! info "Plotting of the global spectra"
 
             The plotting routine for global fitting is similar to the local plotting
             routine, but the spectra are plotted in a grid spectra plot. The first
             row of the grid plot contains the residuals of each single fit, the
             second row the best fit of the model with single peak contributions.
         """
-        n_spec = len(list(self.args["data_statistic"])) - 1
+        n_spec: int = len(list(self.args["data_statistic"])) - 1 if self.args else 1
         _, axs = plt.subplots(
             nrows=2,
             ncols=n_spec,
             sharex=True,
             figsize=(9, 9),
             gridspec_kw={"height_ratios": [1, 2]},
         )
 
         for i in range(n_spec):
-            axs[0, i].set_title(f"Spectrum #{i+1}")
+            axs[0, i].set_title(f"Spectrum #{i + 1}")
             sns.regplot(
                 x=ColumnNamesAPI().energy,
-                y=f"{ColumnNamesAPI().residual}_{i+1}",
+                y=f"{ColumnNamesAPI().residual}_{i + 1}",
                 data=self.df,
                 ax=axs[0, i],
                 color=color[5],
             )
             axs[1, i] = sns.lineplot(
                 x=ColumnNamesAPI().energy,
-                y=f"{ColumnNamesAPI().intensity}_{i+1}",
+                y=f"{ColumnNamesAPI().intensity}_{i + 1}",
                 data=self.df,
                 ax=axs[1, i],
                 color=color[1],
             )
             axs[1, i] = sns.lineplot(
                 x=ColumnNamesAPI().energy,
-                y=f"fit_{i+1}",
+                y=f"fit_{i + 1}",
                 data=self.df,
                 ax=axs[1, i],
                 ls="--",
                 color=color[0],
             )
             peaks = [
                 peak
                 for peak in self.df.columns
-                if not peak.startswith(tuple(ColumnNamesAPI().dict().values()))
-                and peak.endswith(f"_{i+1}")
+                if not peak.startswith(tuple(ColumnNamesAPI().model_dump().values()))
+                and peak.endswith(f"_{i + 1}")
             ]
             color_peaks = sns.color_palette("rocket", len(peaks))
             for j, peak in enumerate(peaks):
                 axs[1, i] = sns.lineplot(
                     x=ColumnNamesAPI().energy,
                     y=peak,
                     data=self.df,
                     ax=axs[1, i],
                     ls=":",
                     color=color_peaks[j],
                 )
 
         plt.tight_layout()
-        plt.show()
 
     def plot_local_spectra(self) -> None:
         """Plot spectra for local fitting.
 
         `plot_spectra` performs a dual split plot. In the upper part, the residuum is
         plotted together with a linear regression line. This means, if the linear
         regression is a flat line, the fit and spectra are identically.
@@ -147,15 +162,15 @@
             ax=ax2,
             ls="--",
             color=color[0],
         )
         peaks = [
             peak
             for peak in self.df.columns
-            if peak not in list(ColumnNamesAPI().dict().values())
+            if peak not in list(ColumnNamesAPI().model_dump().values())
         ]
         color_peaks = sns.color_palette("rocket", len(peaks))
         for i, peak in enumerate(peaks):
             ax2 = sns.lineplot(
                 x=ColumnNamesAPI().energy,
                 y=peak,
                 data=self.df,
@@ -163,8 +178,7 @@
                 ls=":",
                 color=color_peaks[i],
             )
 
         _ = MultiCursor(
             fig.canvas, (ax1, ax2), color=color[4], ls="--", lw=1, horizOn=True
         )
-        plt.show()
```

### Comparing `spectrafit-1.0.0b2/spectrafit/plugins/converter.py` & `spectrafit-1.0.1/spectrafit/plugins/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Abstract base class for the converter plugins."""
+
 from abc import ABC
 from abc import abstractmethod
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import MutableMapping
```

### Comparing `spectrafit-1.0.0b2/spectrafit/plugins/data_converter.py` & `spectrafit-1.0.1/spectrafit/plugins/data_converter.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import re
 
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import List
+from typing import MutableMapping
 from typing import Optional
 
 import pandas as pd
 
 from spectrafit.api.file_model import DataFileAPI
 from spectrafit.plugins.converter import Converter
 
@@ -93,15 +94,16 @@
         """Get the arguments from the command line.
 
         Returns:
             Dict[str, Any]: Return the input file arguments as a dictionary without
                 additional information beyond the command line arguments.
         """
         parser = argparse.ArgumentParser(
-            description="Converter for 'SpectraFit' from data files to CSV files."
+            description="Converter for 'SpectraFit' from data files to CSV files.",
+            usage="%(prog)s [options] infile",
         )
         parser.add_argument(
             "infile",
             type=Path,
             help="Filename of the data file to convert.",
         )
         parser.add_argument(
@@ -118,26 +120,27 @@
             type=str,
             default="csv",
             choices=choices_export,
         )
         return vars(parser.parse_args())
 
     @staticmethod
-    def convert(infile: Path, file_format: str) -> pd.DataFrame:
+    def convert(infile: Path, file_format: str) -> MutableMapping[str, Any]:
         """Convert the input file to the target file format.
 
         Args:
             infile (Path): Input file as a path object.
             file_format (str): Target file format.
 
         Raises:
             ValueError: If the file format is not supported.
 
         Returns:
-            pd.DataFrame: The converted data as a pandas DataFrame.
+            MutableMapping[str, Any]: The converted data as a MutableMapping[str, Any],
+                which belongs to DataFrame.
         """
         if file_format.upper() not in choices:
             raise ValueError(f"File format '{file_format}' is not supported.")
 
         if callable(DataFormats.__dict__[file_format].names):
             names = DataFormats.__dict__[file_format].names(infile)
         else:
```

### Comparing `spectrafit-1.0.0b2/spectrafit/plugins/file_converter.py` & `spectrafit-1.0.1/spectrafit/plugins/file_converter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Convert the input and output files to the preferred file format."""
+
 import argparse
 import json
 
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import MutableMapping
@@ -10,58 +11,61 @@
 import tomli_w
 import yaml
 
 from spectrafit.plugins.converter import Converter
 from spectrafit.tools import read_input_file
 
 
-choices = {"json", "yaml", "yml", "toml", "lock"}
-
-
 class FileConverter(Converter):
     """Convert the input and output file to the preferred file format.
 
     !!! info "Supported file formats"
 
         Currently supported file formats:
 
         -[x] JSON
         -[x] YAML (YML)
         -[x] TOML (LOCK for the lock file)
+
+    Attributes:
+        choices (Set[str]): The choices for the file format.
     """
 
+    choices = {"json", "yaml", "yml", "toml", "lock"}
+
     def get_args(self) -> Dict[str, Any]:
         """Get the arguments from the command line.
 
         Returns:
             Dict[str, Any]: Return the input file arguments as a dictionary without
                 additional information beyond the command line arguments.
         """
         parser = argparse.ArgumentParser(
-            description="Converter for 'SpectraFit' input and output files."
+            description="Converter for 'SpectraFit' input and output files.",
+            usage="%(prog)s [options] infile",
         )
         parser.add_argument(
             "infile",
             type=Path,
             help="Filename of the 'SpectraFit' input or output file.",
         )
         parser.add_argument(
             "-f",
             "--file-format",
             help="File format for the conversion.",
             type=str,
-            choices=choices,
+            choices=self.choices,
         )
         parser.add_argument(
             "-e",
             "--export-format",
             help="File format for the export.",
             type=str,
             default="json",
-            choices=choices,
+            choices=self.choices,
         )
         return vars(parser.parse_args())
 
     @staticmethod
     def convert(infile: Path, file_format: str) -> MutableMapping[str, Any]:
         """Convert the input file to the output file.
 
@@ -71,15 +75,15 @@
 
         Raises:
             ValueError: If the input file format is not supported.
 
         Returns:
             MutableMapping[str, Any] : The converted file as a dictionary.
         """
-        if file_format not in choices:
+        if file_format not in FileConverter.choices:
             raise ValueError(f"The input file format '{file_format}' is not supported.")
 
         return read_input_file(infile)
 
     def save(self, data: Any, fname: Path, export_format: str) -> None:
         """Save the converted file.
 
@@ -95,15 +99,15 @@
         if fname.suffix[1:] == export_format:
             raise ValueError(
                 f"The input file suffix '{fname.suffix[1:]}' is similar to the"
                 f" output file format '{export_format}'."
                 "Please use a different output file suffix."
             )
 
-        if export_format not in choices:
+        if export_format not in self.choices:
             raise ValueError(
                 f"The output file format '{export_format}' is not supported."
             )
 
         if export_format == "json":
             with open(
                 fname.with_suffix(f".{export_format}"), "w", encoding="utf-8"
```

### Comparing `spectrafit-1.0.0b2/spectrafit/plugins/notebook.py` & `spectrafit-1.0.1/spectrafit/plugins/notebook.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,24 +35,27 @@
 from spectrafit.api.report_model import FitMethodAPI
 from spectrafit.api.report_model import InputAPI
 from spectrafit.api.report_model import OutputAPI
 from spectrafit.api.report_model import ReportAPI
 from spectrafit.api.report_model import SolverAPI
 from spectrafit.api.tools_model import ColumnNamesAPI
 from spectrafit.api.tools_model import DataPreProcessingAPI
+from spectrafit.api.tools_model import SolverModelsAPI
 from spectrafit.models import SolverModels
 from spectrafit.tools import PostProcessing
 from spectrafit.tools import PreProcessing
+from spectrafit.tools import exclude_none_dictionary
+from spectrafit.tools import transform_nested_types
 from spectrafit.utilities.transformer import list2dict
 
 
 class DataFrameDisplay:
     """Class for displaying a dataframe in different ways."""
 
-    def df_display(self, df: pd.DataFrame, mode: Optional[str] = None) -> None:
+    def df_display(self, df: pd.DataFrame, mode: Optional[str] = None) -> Optional[Any]:
         """Call the DataframeDisplay class.
 
         !!! info "About `df_display`"
 
             This function is used to display a dataframe in two different ways.
 
             1. Regular display mode:
@@ -71,28 +74,33 @@
 
         Args:
             df (pd.DataFrame): Dataframe to display.
             mode (str, Optional): Display mode. Defaults to None.
 
         Raises:
             ValueError: Raises ValueError if mode of displaying is not supported.
+
+        Returns:
+            Optional[Any]: Returns the dtale object for plotting in the Jupyter
+                 notebook, if mode is `dtale`.
         """
         if mode == "regular":
             self.regular_display(df=df)
         elif mode == "markdown":
             self.markdown_display(df=df)
         elif mode == "interactive":
             self.interactive_display(df=df)
         elif mode == "dtale":
-            self.dtale_display(df=df)
+            return self.dtale_display(df=df)
         elif mode is not None:
             raise ValueError(
                 f"Invalid mode: {mode}. "
                 "Valid modes are: regular, interactive, dtale, markdown."
             )
+        return None
 
     @staticmethod
     def regular_display(df: pd.DataFrame) -> None:
         """Display the dataframe in a regular way.
 
         Args:
             df (pd.DataFrame): Dataframe to display.
@@ -105,21 +113,24 @@
 
         Args:
             df (pd.DataFrame): Dataframe to display.
         """
         itables_show(df)
 
     @staticmethod
-    def dtale_display(df: pd.DataFrame) -> None:
+    def dtale_display(df: pd.DataFrame) -> Any:
         """Display the dataframe in a dtale way.
 
         Args:
             df (pd.DataFrame): Dataframe to display.
+
+        Returns:
+            Any: Returns the dtale object for plotting in the Jupyter notebook.
         """
-        dtale_show(df)
+        return dtale_show(df)
 
     @staticmethod
     def markdown_display(df: pd.DataFrame) -> None:
         """Display the dataframe in a markdown way.
 
         Args:
             df (pd.DataFrame): Dataframe to display.
@@ -221,15 +232,21 @@
             )
             fig["layout"]["yaxis1"].update(domain=[0.8, 1])
             fig["layout"]["yaxis2"].update(domain=[0, 0.7])
             fig.update_yaxes(title_text=residual_title, row=1, col=1)
         else:
             fig.update_yaxes(title_text=yaxis_title, row=1, col=1)
         fig.update_yaxes(title_text=yaxis_title, row=2, col=1)
-        fig.show()
+        fig.show(
+            config={
+                "toImageButtonOptions": dict(
+                    format="png", filename="plot_of_2_dataframes", scale=4
+                )
+            }
+        )
 
     def plot_dataframe(self, args_plot: PlotAPI, df: pd.DataFrame) -> None:
         """Plot the dataframe according to the PlotAPI arguments.
 
         Args:
             args_plot (PlotAPI): PlotAPI object for the settings of the plot.
             df (pd.DataFrame): Dataframe to plot.
@@ -243,26 +260,32 @@
             )
         )
         fig.update_yaxes(
             title_text=self.title_text(
                 name=args_plot.yaxis_title.name, unit=args_plot.yaxis_title.unit
             )
         )
-        fig.show()
+        fig.show(
+            config={
+                "toImageButtonOptions": dict(
+                    format="png", filename="plot_dataframe", scale=4
+                )
+            }
+        )
 
     def plot_global_fit(self, args_plot: PlotAPI, df: pd.DataFrame) -> None:
         """Plot the global dataframe according to the PlotAPI arguments.
 
         Args:
             args_plot (PlotAPI): PlotAPI object for the settings of the plot.
             df (pd.DataFrame): Dataframe to plot.
         """
         for i in range(
             1,
-            sum(1 for _col in df.columns if _col.startswith(ColumnNamesAPI().fit)) + 1,
+            sum(bool(_col.startswith(ColumnNamesAPI().fit)) for _col in df.columns) + 1,
         ):
             _col = [col for col in df.columns if col.endswith(str(i))]
             _col.append(ColumnNamesAPI().energy)
             _df = df[_col]
             _df = _df.rename(
                 columns={
                     f"{ColumnNamesAPI().intensity}_{i}": ColumnNamesAPI().intensity,
@@ -318,15 +341,21 @@
         )
         fig.update_yaxes(
             title_text=self.title_text(
                 name=args_plot.metric_title.name_1, unit=args_plot.metric_title.unit_1
             ),
             secondary_y=True,
         )
-        fig.show()
+        fig.show(
+            config={
+                "toImageButtonOptions": dict(
+                    format="png", filename="plot_metric", scale=4
+                )
+            }
+        )
 
     def update_layout_axes(
         self, fig: Figure, args_plot: PlotAPI, height: int
     ) -> Figure:
         """Update the layout of the plot.
 
         Args:
@@ -336,16 +365,16 @@
 
         Returns:
             Figure: Updated figure.
         """
         fig.update_layout(
             title=args_plot.title,
             legend_title=args_plot.legend_title,
-            legend=args_plot.legend.dict(),
-            font=args_plot.font.dict(),
+            legend=args_plot.legend.model_dump(),
+            font=args_plot.font.model_dump(),
             showlegend=args_plot.show_legend,
             width=args_plot.size[0],
             height=height,
             paper_bgcolor=args_plot.color.paper,
             plot_bgcolor=args_plot.color.plot,
         )
 
@@ -565,14 +594,23 @@
         Returns:
             Dict[str, Any]: Linear correlation of the spectra, fit, and components
                  as dictionary.
         """
         return self.args_out["linear_correlation"]
 
     @property
+    def get_computional(self) -> Dict[str, Any]:
+        """Get the computational time.
+
+        Returns:
+            Dict[str, Any]: Computational time as dictionary.
+        """
+        return self.args_out["fit_insights"]["computional"]
+
+    @property
     def settings_conf_interval(self) -> Union[bool, Dict[str, Any]]:
         """Confidence interval settings.
 
         Returns:
             Union[bool, Dict[str, Any]]: Confidence interval settings.
         """
         if isinstance(self.args_out["conf_interval"], dict):
@@ -624,40 +662,43 @@
     """Class for exporting results as toml."""
 
     def __init__(
         self,
         description: DescriptionAPI,
         initial_model: List[Dict[str, Dict[str, Dict[str, Any]]]],
         pre_processing: DataPreProcessingAPI,
+        settings_solver_models: SolverModelsAPI,
         fname: FnameAPI,
         args_out: Dict[str, Any],
         df_org: pd.DataFrame,
         df_fit: pd.DataFrame,
         df_pre: pd.DataFrame = pd.DataFrame(),
     ) -> None:
         """Initialize the ExportReport class.
 
         Args:
             description (DescriptionAPI): Description of the fit project.
             initial_model (List[Dict[str, Dict[str, Dict[str, Any]]]]): Initial model
                  for the fit.
             pre_processing (DataPreProcessingAPI): Data pre-processing settings.
+            settings_solver_models (SolverModelsAPI): Solver models settings.
             fname (FnameAPI): Filename of the fit project including the path, prefix,
                  and suffix.
             args_out (Dict[str, Any]): Dictionary of SpectraFit settings and results.
             df_org (pd.DataFrame): Dataframe of the original data for performing
                  the fit.
             df_fit (pd.DataFrame): Dataframe of the final fit data.
             df_pre (Optional[pd.DataFrame], optional): Dataframe of the pre-processed.
                  Defaults to pd.DataFrame().
         """
         super().__init__(args_out=args_out)
         self.description = description
         self.initial_model = initial_model
         self.pre_processing = pre_processing
+        self.settings_solver_models = settings_solver_models
         self.fname = fname
 
         self.df_org = df_org.to_dict(orient="list")
         self.df_fit = df_fit.to_dict(orient="list")
         self.df_pre = df_pre.to_dict(orient="list")
 
     @property
@@ -671,14 +712,17 @@
             description=self.description,
             initial_model=self.initial_model,
             pre_processing=self.pre_processing,
             method=FitMethodAPI(
                 global_fitting=self.settings_global_fitting,
                 confidence_interval=self.settings_conf_interval,
                 configurations=self.settings_configurations,
+                settings_solver_models=self.settings_solver_models.model_dump(
+                    exclude_none=True
+                ),
             ),
         )
 
     @property
     def make_solver_contribution(self) -> SolverAPI:
         """Make solver contribution of the report.
 
@@ -691,37 +735,49 @@
             descriptive_statistic=self.get_descriptive_statistic,
             linear_correlation=self.get_linear_correlation,
             component_correlation=self.get_component_correlation,
             confidence_interval=self.get_confidence_interval,
             covariance_matrix=self.get_covariance_matrix,
             variables=self.get_variables,
             errorbars=self.get_errorbars,
+            computional=self.get_computional,
         )
 
     @property
     def make_output_contribution(self) -> OutputAPI:
         """Make output contribution of the report.
 
         Returns:
             OutputAPI: Output contribution of the report as class.
         """
         return OutputAPI(df_org=self.df_org, df_fit=self.df_fit, df_pre=self.df_pre)
 
     def __call__(self) -> Dict[str, Any]:
         """Get the complete report as dictionary.
 
+        !!! info "About the report and `exclude_none_dictionary`"
+
+            The report is generated by using the `ReportAPI` class, which is a
+            `Pydantic`-definition of the report. The `Pydantic`-definition is
+            converted to a dictionary by using the `.model_dump()` option of `Pydantic`.
+            The `recursive_exclude_none` function is used to remove all `None` values
+            from the dictionary, which are hidden in the nested dictionaries.
+
         Returns:
             Dict[str, Any]: Report as dictionary by using the `.dict()` option of
                  pydantic. `None` is excluded.
         """
-        return ReportAPI(
+        report = ReportAPI(
             input=self.make_input_contribution,
             solver=self.make_solver_contribution,
             output=self.make_output_contribution,
-        ).dict(exclude_none=True)
+        ).model_dump(exclude_none=True)
+        report = exclude_none_dictionary(report)
+        report = transform_nested_types(report)
+        return report
 
 
 class SpectraFitNotebook(DataFramePlot, DataFrameDisplay, ExportResults):
     """Jupyter Notebook plugin for SpectraFit."""
 
     args: Dict[str, Any]
     global_: Union[bool, int] = False
@@ -873,21 +929,23 @@
             color=color,
             grid=grid,
             size=size,
         )
         self.export_args_df = FnameAPI(fname=fname, folder=folder, suffix="csv")
         self.export_args_out = FnameAPI(fname=fname, folder=folder, suffix="lock")
 
-        self.args_solver: Dict[str, Any] = {}
+        self.settings_solver_models: SolverModelsAPI = SolverModelsAPI()
         self.pre_statistic: Dict[str, Any] = {}
 
     @property
     def pre_process(self) -> None:
         """Pre-processing class."""
-        self.df, _pre_statistic = PreProcessing(df=self.df, args=self.args_pre.dict())()
+        self.df, _pre_statistic = PreProcessing(
+            df=self.df, args=self.args_pre.model_dump()
+        )()
         self.pre_statistic = _pre_statistic["data_statistic"]
         self.df_pre = self.df.copy()
 
     @property
     def return_pre_statistic(self) -> Dict[str, Any]:
         """Return the pre-processing statistic."""
         return self.pre_statistic
@@ -941,14 +999,21 @@
     def export_df_metric(self) -> None:
         """Export the dataframe."""
         if self.df_metric.empty is False:
             self.export_args_df.prefix = "metric"
             self.export_df(df=self.df_metric, args=self.export_args_df)
 
     @property
+    def export_df_peaks(self) -> None:
+        """Export the dataframe."""
+        if self.df_peaks.empty is False:
+            self.export_args_df.prefix = "peaks"
+            self.export_df(df=self.df_peaks, args=self.export_args_df)
+
+    @property
     def plot_original_df(self) -> None:
         """Plot the original spectra."""
         self.plot_dataframe(args_plot=self.args_plot, df=self.df_org)
 
     @property
     def plot_current_df(self) -> None:
         """Plot the current spectra."""
@@ -1003,14 +1068,15 @@
     def generate_report(self) -> None:
         """Generate the SpectraFit report of the final fit."""
         self.export_report(
             report=ExportReport(
                 description=self.args_desc,
                 initial_model=self.initial_model,
                 pre_processing=self.args_pre,
+                settings_solver_models=self.settings_solver_models,
                 fname=self.export_args_out,
                 args_out=self.args,
                 df_org=self.df_org,
                 df_pre=self.df_pre,
                 df_fit=self.df_fit,
             )(),
             args=self.export_args_out,
@@ -1022,14 +1088,15 @@
         show_plot: bool = True,
         show_metric: bool = True,
         show_df: bool = False,
         show_peaks: bool = False,
         conf_interval: Union[bool, Dict[str, Any]] = False,
         bar_criteria: Optional[Union[str, List[str]]] = None,
         line_criteria: Optional[Union[str, List[str]]] = None,
+        solver_settings: Optional[Dict[str, Any]] = None,
     ) -> None:
         """Solves the fit problem based on the proposed model.
 
         Args:
             initial_model (List[Dict[str, Dict[str, Dict[str, Any]]]]): List of
                  dictionary with the initial model and its fitting parameters and
                  options for the components.
@@ -1045,44 +1112,53 @@
                  the confidence interval and accelerate its. Defaults to False.
             bar_criteria (Optional[Union[str, List[str]]], optional): Criteria for the
                 bar plot. It is recommended to use attributes from `goodness of fit`
                 module. Defaults to None.
             line_criteria (Optional[Union[str, List[str]]], optional): Criteria for
                 the line plot. It is recommended to use attributes from
                 `regression metric` module. Defaults to None.
+            solver_settings (Optional[Dict[str, Any]], optional): Settings for
+                the solver models, which is split into settings for `minimizer` and
+                `optimizer`.  Defaults to None.
 
         !!! info: "About criteria"
 
             The criteria for the bar and line plot are defined as a list of strings.
             The supported keywords are defined by the built-in metrics for
             `goodness of fit` and `regression` and can be checked in [documentation](
                 https://anselmoo.github.io/spectrafit/doc/statistics/
             ).
 
         """
         self.initial_model = initial_model
 
         if isinstance(conf_interval, bool):
-            conf_interval = ConfIntervalAPI().dict() if conf_interval is True else False
+            conf_interval = (
+                ConfIntervalAPI().model_dump() if conf_interval is True else False
+            )
         elif isinstance(conf_interval, dict):
             conf_interval = ConfIntervalAPI(**conf_interval).dict(exclude_none=True)
 
+        if solver_settings is not None and isinstance(solver_settings, dict):
+            self.settings_solver_models = SolverModelsAPI(**solver_settings)
+
         self.df_fit, self.args = PostProcessing(
             self.df,
             {
                 "global_": self.global_,
                 "conf_interval": conf_interval,
             },
             *SolverModels(
                 df=self.df,
                 args={
                     "global_": self.global_,
                     "column": list(self.df.columns),
                     "autopeak": self.autopeak,
                     **list2dict(peak_list=self.initial_model),
+                    **self.settings_solver_models.model_dump(),
                 },
             )(),
         )()
         self.update_metric()
         self.update_peaks()
         if show_plot:
             self.plot_fit_df()
```

### Comparing `spectrafit-1.0.0b2/spectrafit/plugins/pkl_converter.py` & `spectrafit-1.0.1/spectrafit/plugins/pkl_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 
 from spectrafit.plugins.converter import Converter
 from spectrafit.tools import pkl2any
 from spectrafit.tools import pure_fname
 
 
 pkl_gz = "pkl.gz"
-choices_fformat = {"latin1", "utf-8", "utf-16", "utf-32"}
-choices_export = {"npy", "npz", "pkl", pkl_gz}
 
 
 class ExportData:
     """Export the data to a file.
 
     !!! info "General information"
 
@@ -121,47 +119,55 @@
 
         Currently supported file formats:
 
         -[x] pkl
         -[x] pkl.gz
         -[x] ...
 
+
+    Attributes:
+        choices_fformat (Set[str]): The choices for the file format.
+        choices_export (Set[str]): The choices for the export format.
     """
 
+    choices_fformat = {"latin1", "utf-8", "utf-16", "utf-32"}
+    choices_export = {"npy", "npz", "pkl", pkl_gz}
+
     def get_args(self) -> Dict[str, Any]:
         """Get the arguments from the command line.
 
         Returns:
             Dict[str, Any]: Return the input file arguments as a dictionary without
                 additional information beyond the command line arguments.
         """
         parser = argparse.ArgumentParser(
-            description="Converter for 'SpectraFit' from pkl files to CSV files."
+            description="Converter for 'SpectraFit' from pkl files to CSV files.",
+            usage="%(prog)s [options] infile",
         )
         parser.add_argument(
             "infile",
             type=Path,
             help="Filename of the pkl file to convert.",
         )
         parser.add_argument(
             "-f",
             "--file-format",
             help="File format for the optional encoding of the pickle file."
             " Default is 'latin1'.",
             type=str,
             default="latin1",
-            choices=choices_fformat,
+            choices=self.choices_fformat,
         )
         parser.add_argument(
             "-e",
             "--export-format",
             help="File format for export of the output file. Default is 'pkl'.",
             type=str,
             default="pkl",
-            choices=choices_export,
+            choices=self.choices_export,
         )
         return vars(parser.parse_args())
 
     @staticmethod
     def convert(infile: Path, file_format: str) -> Dict[str, Any]:
         """Convert the input file to the output file.
 
@@ -220,15 +226,15 @@
             data (Any): The converted nested dictionary of the pkl data.
             fname (Path): The filename of the output file.
             export_format (str): The file format of the output file.
 
         Raises:
             ValueError: If the export format is not supported.
         """
-        if export_format.lower() not in choices_export:
+        if export_format.lower() not in self.choices_export:
             raise ValueError(f"Unsupported file format '{export_format}'.")
 
         fname = pure_fname(fname)
 
         for key, value in data.items():
             _fname = Path(f"{fname}_{key}").with_suffix(f".{export_format}")
             ExportData(data=value, fname=_fname, export_format=export_format)()
```

### Comparing `spectrafit-1.0.0b2/spectrafit/plugins/pkl_visualizer.py` & `spectrafit-1.0.1/spectrafit/plugins/pkl_visualizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,52 +13,57 @@
 import numpy as np
 
 from spectrafit.plugins.converter import Converter
 from spectrafit.tools import pkl2any
 from spectrafit.tools import pure_fname
 
 
-choices_fformat = {"latin1", "utf-8", "utf-16", "utf-32"}
-choices_export = {"png", "pdf", "jpg", "jpeg"}
+class PklVisualizer(Converter):
+    """Visualize the pkl data as a graph.
 
+    Attributes:
+        choices_fformat (Set[str]): The choices for the file format.
+        choices_export (Set[str]): The choices for the export format.
+    """
 
-class PklVisualizer(Converter):
-    """Visualize the pkl data as a graph."""
+    choices_fformat = {"latin1", "utf-8", "utf-16", "utf-32"}
+    choices_export = {"png", "pdf", "jpg", "jpeg"}
 
     def get_args(self) -> Dict[str, Any]:
         """Get the arguments from the command line.
 
         Returns:
             Dict[str, Any]: Return the input file arguments as a dictionary without
                 additional information beyond the command line arguments.
         """
         parser = argparse.ArgumentParser(
-            description="Converter for 'SpectraFit' from pkl files to a graph."
+            description="Converter for 'SpectraFit' from pkl files to a graph.",
+            usage="%(prog)s [options] infile",
         )
         parser.add_argument(
             "infile",
             type=Path,
             help="Filename of the pkl file to convert to graph.",
         )
         parser.add_argument(
             "-f",
             "--file-format",
             help="File format for the optional encoding of the pickle file."
             " Default is 'latin1'.",
             type=str,
             default="latin1",
-            choices=choices_fformat,
+            choices=self.choices_fformat,
         )
         parser.add_argument(
             "-e",
             "--export-format",
             help="File extension for the graph export.",
             type=str,
             default="pdf",
-            choices=choices_export,
+            choices=self.choices_export,
         )
 
         return vars(parser.parse_args())
 
     @staticmethod
     def convert(infile: Path, file_format: str) -> Dict[str, Any]:
         """Convert the input file to the output file.
@@ -94,15 +99,15 @@
             data (Any): The data to save, which can be a nested dictionary.
             fname (Path): The filename of the file to save.
             export_format (str): The file format to save the graph to.
 
         Raises:
             ValueError: If the export format is not supported.
         """
-        if export_format.lower() not in choices_export:
+        if export_format.lower() not in self.choices_export:
             raise ValueError(f"Export format '{export_format}' is not supported.")
 
         plt.savefig(
             pure_fname(fname).with_suffix(f".{export_format}"),
             format=export_format,
         )
```

### Comparing `spectrafit-1.0.0b2/spectrafit/plugins/rixs_converter.py` & `spectrafit-1.0.1/spectrafit/plugins/rixs_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
         Returns:
             Dict[str, Any]: Return the input file arguments as a dictionary without
                 additional information beyond the command line arguments.
         """
         parser = argparse.ArgumentParser(
             description="Converter for 'SpectraFit' from pkl files to a JSON, TOML, "
-            "or numpy file for RIXS-Visualizer."
+            "or numpy file for RIXS-Visualizer.",
+            usage="%(prog)s [options] infile",
         )
         parser.add_argument(
             "infile",
             type=Path,
             help="Filename of the pkl file to convert to JSON, TOML, or numpy.",
         )
         parser.add_argument(
@@ -215,15 +216,15 @@
         self.save(
             data=self.create_rixs(
                 data=self.convert(args["infile"], args["file_format"]),
                 incident_energy=args["incident_energy"],
                 emission_energy=args["emission_energy"],
                 rixs_map=args["rixs_map"],
                 mode=args["mode"],
-            ).dict(),
+            ).model_dump(),
             fname=args["infile"],
             export_format=args["export_format"],
         )
 
 
 def command_line_runner() -> None:
     """Run the command line script."""
```

### Comparing `spectrafit-1.0.0b2/spectrafit/plugins/rixs_visualizer.py` & `spectrafit-1.0.1/spectrafit/plugins/rixs_visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -648,14 +648,14 @@
             incident_energy=np.array(data["incident_energy"]),
             emission_energy=np.array(data["emission_energy"]),
             rixs_map=np.array(data["rixs_map"]),
         )
 
     def __call__(self) -> None:  # pragma: no cover
         """Run the RIXS Visualizer."""
-        app = RIXSApp(**self.load_data(self.get_args()["infile"]).dict())
+        app = RIXSApp(**self.load_data(self.get_args()["infile"]).model_dump())
         app.app_run()
 
 
 def command_line_runner() -> None:
     """Run the RIXS Visualizer from the command line."""
     RIXSVisualizer()()
```

### Comparing `spectrafit-1.0.0b2/spectrafit/spectrafit.py` & `spectrafit-1.0.1/spectrafit/spectrafit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """SpectraFit, the command line tool for fitting."""
+
 import argparse
 
 from typing import Any
 from typing import Dict
 from typing import MutableMapping
 from typing import Optional
 from typing import Tuple
@@ -28,15 +29,18 @@
     """Get the arguments from the command line.
 
     Returns:
         Dict[str, Any]: Return the input file arguments as a dictionary without
              additional information beyond the command line arguments.
     """
     parser = argparse.ArgumentParser(
-        description="Fast Fitting Program for ascii txt files."
+        description="Fast Fitting Program for ascii txt files.",
+        usage="spectrafit [options] infile",
+        epilog="For more information, visit https://anselmoo.github.io/spectrafit/",
+        prog="spectrafit",
     )
     parser.add_argument("infile", type=str, help="Filename of the spectra data")
     parser.add_argument(
         "-o",
         "--outfile",
         default="spectrafit_results",
         type=str,
@@ -161,16 +165,16 @@
         action="store_true",
         default=False,
     )
     parser.add_argument(
         "-v",
         "--version",
         help="Display the current version of `SpectraFit`.",
-        action="store_true",
-        default=False,
+        action="version",
+        version=__status__.version(),
     )
     parser.add_argument(
         "-vb",
         "--verbose",
         help=(
             "Display the initial configuration parameters and fit results, as a table "
             "'1', as a dictionary '2', or not in the terminal '0'. The default option "
@@ -191,18 +195,14 @@
              dictionary with additional information beyond the command line arguments.
              Defaults to None.
     """
     __status__.welcome()
     while True:
         if not args:
             args = extracted_from_command_line_runner()
-        if args["version"]:
-            __status__.version()
-            return
-
         __status__.start()
 
         df_result, args = fitting_routine(args=args)
         PlotSpectra(df=df_result, args=args)()
         SaveResult(df=df_result, args=args)()
         args = None
 
@@ -232,15 +232,15 @@
     """
     result: Dict[str, Any] = get_args()
     _args: MutableMapping[str, Any] = read_input_file(result["input"])
 
     if "settings" in _args.keys():
         for key in _args["settings"].keys():
             result[key] = _args["settings"][key]
-    result = CMDModelAPI(**result).dict()
+    result = CMDModelAPI(**result).model_dump()
     if "description" in _args["fitting"].keys():
         result["description"] = _args["fitting"]["description"]
     if "parameters" in _args["fitting"].keys():
         if "minimizer" in _args["fitting"]["parameters"].keys():
             result["minimizer"] = _args["fitting"]["parameters"]["minimizer"]
         else:
             raise KeyError("Missing 'minimizer' in 'parameters'!")
```

### Comparing `spectrafit-1.0.0b2/spectrafit/tools.py` & `spectrafit-1.0.1/spectrafit/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Collection of essential tools for running SpectraFit."""
+
 import gzip
 import json
 import pickle
 import sys
 
 from pathlib import Path
 from typing import Any
@@ -14,15 +15,15 @@
 
 import numpy as np
 import pandas as pd
 import tomli
 import yaml
 
 from lmfit import Minimizer
-from lmfit import conf_interval
+from lmfit.confidence import ConfidenceInterval
 from lmfit.minimizer import MinimizerException
 from spectrafit.api.tools_model import ColumnNamesAPI
 from spectrafit.models import calculated_model
 from spectrafit.report import RegressionMetrics
 from spectrafit.report import fit_report_as_dict
 
 
@@ -53,15 +54,15 @@
                     2. shifted
                     3. linear oversampled
                     4. smoothed
             Dict[str,Any]: Adding a descriptive statistics to the input dictionary.
         """
         df_copy: pd.DataFrame = self.df.copy()
         self.args["data_statistic"] = df_copy.describe(
-            percentiles=np.arange(0.1, 1.0, 0.1)
+            percentiles=np.arange(0.1, 1.0, 0.1).tolist()
         ).to_dict(orient="split")
         try:
             if isinstance(self.args["energy_start"], (int, float)) or isinstance(
                 self.args["energy_stop"], (int, float)
             ):
                 df_copy = self.energy_range(df_copy, self.args)
             if self.args["shift"]:
@@ -89,15 +90,15 @@
         Returns:
             pd.DataFrame: DataFrame containing the `optimized` input data
                  (`x` and `data`), which are shrinked according to the energy range.
         """
         energy_start: Union[int, float] = args["energy_start"]
         energy_stop: Union[int, float] = args["energy_stop"]
 
-        df_copy: pd.DataFrame = df.copy()
+        df_copy = df.copy()
         if isinstance(energy_start, (int, float)) and isinstance(
             energy_stop, (int, float)
         ):
             return df_copy.loc[
                 (df[args["column"][0]] >= energy_start)
                 & (df[args["column"][0]] <= energy_stop)
             ]
@@ -248,17 +249,19 @@
                  and `intensity` is extended by a `_`  and column index; like: `energy`
                  and `intensity_1`, `intensity_2`, `intensity_...` depending on
                  the dataset size.
         """
         if self.args["global_"]:
             return df.rename(
                 columns={
-                    col: ColumnNamesAPI().energy
-                    if i == 0
-                    else f"{ColumnNamesAPI().intensity}_{i}"
+                    col: (
+                        ColumnNamesAPI().energy
+                        if i == 0
+                        else f"{ColumnNamesAPI().intensity}_{i}"
+                    )
                     for i, col in enumerate(df.columns)
                 }
             )
         return df.rename(
             columns={
                 df.columns[0]: ColumnNamesAPI().energy,
                 df.columns[1]: ColumnNamesAPI().intensity,
@@ -280,21 +283,33 @@
                 6. Covariance Matrix
                 7. _Optional_: Confidence Interval
 
             All of the above are included in the report as dictionary in `args`.
 
         """
         self.args["fit_insights"] = fit_report_as_dict(
-            self.result, modelpars=self.result.params
+            inpars=self.result, settings=self.minimizer, modelpars=self.result.params
         )
         if self.args["conf_interval"]:
             try:
-                self.args["confidence_interval"] = conf_interval(
+                _min_rel_change = self.args["conf_interval"].pop("min_rel_change", None)
+                ci = ConfidenceInterval(
                     self.minimizer, self.result, **self.args["conf_interval"]
                 )
+                if _min_rel_change is not None:
+                    ci.min_rel_change = _min_rel_change
+                    self.args["conf_interval"]["min_rel_change"] = _min_rel_change
+
+                trace = self.args["conf_interval"].get("trace")
+
+                if trace is True:
+                    self.args["confidence_interval"] = (ci.calc_all_ci(), ci.trace_dict)
+                else:
+                    self.args["confidence_interval"] = ci.calc_all_ci()
+
             except (MinimizerException, ValueError, KeyError) as exc:
                 print(f"Error: {exc} -> No confidence interval could be calculated!")
                 self.args["confidence_interval"] = {}
 
     def make_residual_fit(self) -> None:
         r"""Make the residuals of the model and the fit.
 
@@ -391,15 +406,15 @@
             module.
         """
         self.args["regression_metrics"] = RegressionMetrics(self.df)()
 
     def export_desprective_statistic2args(self) -> None:
         """Export the descriptive statistic of the spectra, fit, and contributions."""
         self.args["descriptive_statistic"] = self.df.describe(
-            percentiles=np.arange(0.1, 1, 0.1)
+            percentiles=np.arange(0.1, 1, 0.1).tolist()
         ).to_dict(orient="split")
 
 
 class SaveResult:
     """Saving the result of the fitting process."""
 
     def __init__(self, df: pd.DataFrame, args: Dict[str, Any]) -> None:
@@ -459,15 +474,15 @@
             df (pd.DataFrame): DataFrame containing the input data (`x` and `data`),
                  as well as the best fit and the corresponding residuum. Hence, it will
                  be extended by the single contribution of the model.
             args (Dict[str,Any]): The input file arguments as a dictionary with
                  additional information beyond the command line arguments.
         """
         self.df = df
-        self.args = args
+        self.args = transform_nested_types(args)
 
     def __call__(self) -> None:
         """Call the SaveResult class."""
         self.save_as_json()
         self.save_as_csv()
 
     def save_as_csv(self) -> None:
@@ -477,33 +492,34 @@
             The fit results are saved to csv files and are divided into three different
             categories:
 
                 1. The `results` of the optimization process.
                 2. The `correlation analysis` of the optimization process.
                 3. The `error analysis` of the optimization process.
         """
-        self.df.to_csv(Path(f"{self.args['outfile']}_fit.csv"), index=False)
+        _fname = Path(f"{self.args['outfile']}_fit.csv")
+        self.df.to_csv(_fname, index=False)
         pd.DataFrame(**self.args["linear_correlation"]).to_csv(
             Path(f"{self.args['outfile']}_correlation.csv"),
             index=True,
             index_label="attributes",
         )
         pd.DataFrame.from_dict(self.args["fit_insights"]["variables"]).to_csv(
-            Path(f"{self.args['outfile']}_errors.csv"),
+            Path(f"{self.args['outfile']}_components.csv"),
             index=True,
             index_label="attributes",
         )
 
     def save_as_json(self) -> None:
         """Save the fitting result as json file."""
         if self.args["outfile"]:
             with open(
                 Path(f"{self.args['outfile']}_summary.json"), "w", encoding="utf-8"
             ) as f:
-                json.dump(self.args, f, indent=4)
+                json.dump(transform_nested_types(self.args), f, indent=4)
         else:
             raise FileNotFoundError("No output file provided!")
 
 
 def read_input_file(fname: Path) -> MutableMapping[str, Any]:
     """Read the input file.
 
@@ -524,15 +540,15 @@
 
     if fname.suffix == ".toml":
         with open(fname, "rb") as f:
             args = tomli.load(f)
     elif fname.suffix == ".json":
         with open(fname, encoding="utf-8") as f:
             args = json.load(f)
-    elif fname.suffix in [".yaml", ".yml"]:
+    elif fname.suffix in {".yaml", ".yml"}:
         with open(fname, encoding="utf-8") as f:
             args = yaml.load(f, Loader=yaml.FullLoader)
     else:
         raise OSError(
             f"ERROR: Input file {fname} has not supported file format.\n"
             "Supported fileformats are: '*.json', '*.yaml', and '*.toml'"
         )
@@ -663,7 +679,57 @@
         fname (Path): The filename to be processed.
 
     Returns:
         Path: The filename without the suffix.
     """
     _fname = fname.parent / fname.stem
     return pure_fname(_fname) if _fname.suffix else _fname
+
+
+def exclude_none_dictionary(value: Dict[str, Any]) -> Dict[str, Any]:
+    """Exclude `None` values from the dictionary.
+
+    Args:
+        value (Dict[str, Any]): Dictionary to be processed to
+            exclude `None` values.
+
+    Returns:
+        Dict[str, Any]: Dictionary without `None` values.
+    """
+    if isinstance(value, list):
+        return [exclude_none_dictionary(v) for v in value if v is not None]
+    elif isinstance(value, dict):
+        return {
+            k: exclude_none_dictionary(v) for k, v in value.items() if v is not None
+        }
+    else:
+        return value
+
+
+def transform_nested_types(value: Dict[str, Any]) -> Dict[str, Any]:
+    """Transform nested types numpy values to python values.
+
+    Args:
+        value (Dict[str, Any]): Dictionary to be processed to
+            transform numpy values to python values.
+
+    Returns:
+        Dict[str, Any]: Dictionary with python values.
+    """
+    if isinstance(value, list):
+        return [transform_nested_types(v) for v in value]
+    elif isinstance(value, tuple):
+        return tuple(transform_nested_types(v) for v in value)
+    elif isinstance(value, dict):
+        return {k: transform_nested_types(v) for k, v in value.items()}
+    elif isinstance(value, np.ndarray):
+        return transform_nested_types(value.tolist())
+    elif isinstance(value, np.int32):
+        return int(value)
+    elif isinstance(value, np.int64):
+        return int(value)
+    elif isinstance(value, np.bool_):
+        return bool(value)
+    elif isinstance(value, np.float64):
+        return float(value)
+    else:
+        return value
```

### Comparing `spectrafit-1.0.0b2/spectrafit/utilities/transformer.py` & `spectrafit-1.0.1/spectrafit/utilities/transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Transformer functions for the SpectraFit."""
+
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Union
 
 from spectrafit.api.models_model import DistributionModelAPI
 
@@ -18,15 +19,15 @@
 
     Returns:
         Dict[str, Dict[str, Dict[str, Any]]]: Dictionary with the initial fitting
              parameters for the peaks.
     """
     peaks_dict: Dict[str, Dict[str, Dict[str, Any]]] = {"peaks": {}}
     for i, peak in enumerate(peak_list, start=1):
-        if list(peak.keys())[0] in DistributionModelAPI().__dict__.keys():
+        if list(peak)[0] in DistributionModelAPI().__dict__:
             peaks_dict["peaks"][f"{i}"] = peak
     return peaks_dict
 
 
 def remove_none_type(d: Any) -> Union[Dict[str, Any], List[Any]]:
     """Remove None type from dictionary in a recursive fashion.
```

### Comparing `spectrafit-1.0.0b2/PKG-INFO` & `spectrafit-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: spectrafit
-Version: 1.0.0b2
+Name: SpectraFit
+Version: 1.0.1
 Summary: Fast fitting of 2D- and 3D-Spectra with established routines
 Home-page: https://pypi.org/project/spectrafit/
 License: BSD-3-Clause
 Keywords: 2D-Spectra,3D-Spectra,fitting,curve-fitting,peak-fitting,spectrum
 Author: Anselm Hahn
 Author-email: anselm.hahn@gmail.com
 Maintainer: Anselm Hahn
@@ -18,113 +18,126 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: all
 Provides-Extra: graph
 Provides-Extra: jupyter
 Provides-Extra: jupyter-dash
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: art (>=5.8,<6.0)
+Requires-Dist: art (>=5.8,<7.0)
 Requires-Dist: dash-bootstrap-components (>=1.3.0,<2.0.0) ; extra == "jupyter-dash" or extra == "all"
 Requires-Dist: dash-bootstrap-templates (>=1.0.7,<2.0.0) ; extra == "jupyter-dash" or extra == "all"
-Requires-Dist: dtale (>=2.8.1,<3.0.0) ; extra == "jupyter" or extra == "all"
+Requires-Dist: dtale (>=3.9.0,<4.0.0) ; extra == "jupyter" or extra == "all"
 Requires-Dist: emcee (>=3.1.2,<4.0.0)
 Requires-Dist: ipywidgets (>=8.0.4,<9.0.0) ; extra == "jupyter-dash" or extra == "all"
-Requires-Dist: itables (>=1.3.4,<2.0.0) ; extra == "jupyter" or extra == "all"
+Requires-Dist: itables (>=1.3.4,<3.0.0) ; extra == "jupyter" or extra == "all"
 Requires-Dist: jupyter-dash (>=0.4.2,<0.5.0) ; extra == "jupyter-dash" or extra == "all"
-Requires-Dist: jupyterlab (>=3.5.2,<4.0.0) ; extra == "jupyter" or extra == "all"
+Requires-Dist: jupyterlab (>=3.5.2,<5.0.0) ; extra == "jupyter" or extra == "all"
 Requires-Dist: kaleido (==0.2.1) ; extra == "jupyter" or extra == "all"
-Requires-Dist: lmfit (>=1.1.0,<2.0.0)
+Requires-Dist: lmfit (>=1.2.2,<2.0.0)
 Requires-Dist: networkx[all] (>=3.0,<4.0) ; extra == "graph" or extra == "all"
 Requires-Dist: numdifftools (>=0.9.41,<0.10.0)
-Requires-Dist: numpy (>=1.23.4,<2.0.0)
+Requires-Dist: numpy (<1.26.4) ; python_version < "3.9"
+Requires-Dist: numpy (>=1.26.4,<2.0.0) ; python_version >= "3.9"
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0)
-Requires-Dist: pandas (>=1.5.0,<2.0.0)
-Requires-Dist: plotly (>=5.14.0,<6.0.0) ; extra == "jupyter" or extra == "all"
-Requires-Dist: pydantic (>=1.10.1,<2.0.0)
+Requires-Dist: pandas (<2.2.1) ; python_version < "3.9"
+Requires-Dist: pandas (>=2.2.2,<3.0.0) ; python_version >= "3.9"
+Requires-Dist: plotly (>=5.21.0,<6.0.0) ; extra == "jupyter" or extra == "all"
+Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: pydot (>=1.4.2,<2.0.0) ; extra == "graph" or extra == "all"
+Requires-Dist: python-pptx (>=0.6.22,<0.7.0) ; extra == "jupyter" or extra == "all"
 Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
-Requires-Dist: seaborn (>=0.12.0,<0.13.0)
+Requires-Dist: scipy (>=1.10.1,<2.0.0) ; python_version < "3.9"
+Requires-Dist: scipy (>=1.13.0,<2.0.0) ; python_version >= "3.9"
+Requires-Dist: seaborn (>=0.13.0,<0.14.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Project-URL: Documentation, https://anselmoo.github.io/spectrafit/
 Project-URL: Repository, https://github.com/Anselmoo/spectrafit
 Description-Content-Type: text/markdown
 
 [![CI - Python Package](https://github.com/Anselmoo/spectrafit/actions/workflows/python-ci.yml/badge.svg?branch=main)](https://github.com/Anselmoo/spectrafit/actions/workflows/python-ci.yml)
 [![codecov](https://codecov.io/gh/Anselmoo/spectrafit/branch/main/graph/badge.svg?token=pNIMKwWsO2)](https://codecov.io/gh/Anselmoo/spectrafit)
 [![PyPI](https://img.shields.io/pypi/v/spectrafit?logo=PyPi&logoColor=yellow)](https://pypi.org/project/spectrafit/)
 [![Conda](https://img.shields.io/conda/v/conda-forge/spectrafit?label=Anaconda.org&logo=anaconda)](https://github.com/conda-forge/spectrafit-feedstock)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spectrafit?color=gree&logo=Python&logoColor=yellow)](https://pypi.org/project/spectrafit/)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Anselmoo/spectrafit/main.svg)](https://results.pre-commit.ci/latest/github/Anselmoo/spectrafit/main)
+[![doi](https://img.shields.io/badge/10.1021/acsomega.3c09262-blue?logo=DOI&logoColor=white)](https://pubs.acs.org/doi/full/10.1021/acsomega.3c09262)
 
 <p align="center">
 <img src="https://github.com/Anselmoo/spectrafit/blob/c5f7ee05e5610fb8ef4e237a88f62977b6f832e5/docs/images/spectrafit_synopsis.png?raw=true">
 </p>
 
 # SpectraFit
 
-`SpectraFit` is a tool for quick data fitting based on the regular
-expression of distribution and linear functions via command line or
-[Jupyter Notebook](https://jupyter.org). Furthermore, it can be also used as
-a module in existing python code. A previous version of `SpectraFit` was used
-for the following publication:
-
-- [Measurement of the Ligand Field Spectra of Ferrous and Ferric Iron Chlorides Using 2p3d RIXS](https://pubs.acs.org/doi/abs/10.1021/acs.inorgchem.7b00940)
-
-Now, it is completely rewritten and is more flexible. It is supporting all
-common ASCII-data formats and it runs on `Linux`, `Windows`, and `MacOS`.
+`SpectraFit` is a Python tool for quick data fitting based on the regular
+expression of distribution and linear functions via the command line (CMD) or
+[Jupyter Notebook](https://jupyter.org) It is designed to be easy to use and
+supports all common ASCII data formats. SpectraFit runs on **Linux**,
+**Windows**, and **MacOS**.
 
 ## Scope
 
 - Fitting of 2D data, also with multiple columns as _global fitting_
 - Using established and advanced solver methods
 - Extensibility of the fitting function
 - Guarantee traceability of the fitting results
 - Saving all results in a _SQL-like-format_ (`CSV`) for publications
 - Saving all results in a _NoSQL-like-format_ (`JSON`) for project management
 - Having an API interface for Graph-databases
 
+`SpectraFit` is a tool designed for researchers and scientists who require
+immediate data fitting to a model. It proves to be especially beneficial for
+individuals working with vast datasets or who need to conduct numerous fits
+within a limited time frame. `SpectraFit's` adaptability to various platforms
+and data formats makes it a versatile tool that caters to a broad spectrum of
+scientific applications.
+
 ## Installation
 
 via pip:
 
-```terminal
+```bash
 pip install spectrafit
 
 # with support for Jupyter Notebook
 
 pip install spectrafit[jupyter]
 
+# with support for the dashboard in the Jupyter Notebook
+
+pip install spectrafit[jupyter-dash]
+
+# with support to visualize pkl-files as graph
+
+pip install spectrafit[graph]
+
 # with all upcomming features
 
 pip install spectrafit[all]
 
 # Upgrade
 
 pip install spectrafit --upgrade
 ```
 
-via conda, see also [conda-forge](https://github.com/conda-forge/spectrafit-feedstock):
+via conda, see also
+[conda-forge](https://github.com/conda-forge/spectrafit-feedstock):
 
-```terminal
+```bash
 conda install -c conda-forge spectrafit
 
 # with support for Jupyter Notebook
 
 conda install -c conda-forge spectrafit-jupyter
 
 # with all upcomming features
@@ -154,19 +167,19 @@
 
 1. [Pandas](https://pandas.pydata.org/)
 2. [statsmodels](https://www.statsmodels.org/stable/index.html)
 3. [numdifftools](https://github.com/pbrod/numdifftools)
 4. [Matplotlib](https://matplotlib.org/) in combination with
    [Seaborn](https://seaborn.pydata.org/)
 
-```terminal
+```bash
 spectrafit data_file.txt -i input_file.json
 ```
 
-```terminal
+```bash
 usage: spectrafit [-h] [-o OUTFILE] [-i INPUT] [-ov] [-e0 ENERGY_START]
                   [-e1 ENERGY_STOP] [-s SMOOTH] [-sh SHIFT] [-c COLUMN COLUMN]
                   [-sep {       ,,,;,:,|, ,s+}] [-dec {.,,}] [-hd HEADER]
                   [-g {0,1,2}] [-auto] [-np] [-v] [-vb {0,1,2}]
                   infile
 
 Fast Fitting Program for ascii txt files.
@@ -227,29 +240,29 @@
                         table `printout`.
 ```
 
 ### Jupyter Notebook
 
 Open the `Jupyter Notebook` and run the following code:
 
-```terminal
+```bash
 spectrafit-jupyter
 ```
 
-or via Docker Image:
+or via Docker Image for `<cpu>` with `amd64` and `arm64`:
 
-```terminal
-docker pull ghcr.io/anselmoo/spectrafit:latest
-docker run -it -p 8888:8888 spectrafit:latest
+```bash
+docker pull ghcr.io/anselmoo/spectrafit-<cpu>:latest
+docker run -it -p 8888:8888 spectrafit-<cpu>:latest
 ```
 
 or just:
 
-```terminal
-docker run -p 8888:8888 ghcr.io/anselmoo/spectrafit:latest
+```bash
+docker run -p 8888:8888 ghcr.io/anselmoo/spectrafit-<cpu>:latest
 ```
 
 Next define your initial model and the reference data:
 
 ```python
 from spectrafit.plugins.notebook import SpectraFitNotebook
 import pandas as pd
```

