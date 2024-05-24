# Comparing `tmp/sarus_data_spec_public-4.0.2.tar.gz` & `tmp/sarus_data_spec_public-4.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus_data_spec_public-4.0.2.tar", last modified: Fri May 24 09:13:35 2024, max compression
+gzip compressed data, was "sarus_data_spec_public-4.0.2.dev0.tar", last modified: Mon May 20 12:26:15 2024, max compression
```

## Comparing `sarus_data_spec_public-4.0.2.tar` & `sarus_data_spec_public-4.0.2.dev0.tar`

### file list

```diff
@@ -1,225 +1,224 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.216332 sarus_data_spec_public-4.0.2/
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      656 2024-05-24 09:13:35.216332 sarus_data_spec_public-4.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.171332 sarus_data_spec_public-4.0.2/sarus_data_spec/
--rwxrwxrwx   0 root         (0) root         (0)      942 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.173332 sarus_data_spec_public-4.0.2/sarus_data_spec/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/arrow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8510 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/arrow/admin_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/arrow/array.py
--rw-rw-rw-   0 root         (0) root         (0)     7389 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/arrow/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     2100 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/arrow/pandas_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6266 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/arrow/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    10718 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/arrow/type.py
--rw-rw-rw-   0 root         (0) root         (0)     1014 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     4646 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/bounds.py
--rw-rw-rw-   0 root         (0) root         (0)     4266 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.174332 sarus_data_spec_public-4.0.2/sarus_data_spec/context/
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/context/public.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/context/state.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/context/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    21819 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.176332 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_rewriter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_rewriter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2314 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_rewriter/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4997 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    22994 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py
--rw-rw-rw-   0 root         (0) root         (0)    11623 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_rewriter/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_rewriter/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3438 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_rewriter/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.178332 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_validator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_validator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17255 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_validator/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3941 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_validator/parameter_kind.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_validator/privacy_limit.py
--rw-rw-rw-   0 root         (0) root         (0)     5717 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_validator/recursive_validator.py
--rw-rw-rw-   0 root         (0) root         (0)    28910 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_validator/signature.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_validator/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     5355 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_validator/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     8867 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8679 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/json_serialisation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.179332 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7629 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/async_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    32667 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6724 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/cache_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.180332 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/computations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/computations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9104 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/computations/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.180332 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/computations/local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/computations/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/computations/local/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2583 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/computations/local/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.181332 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/computations/remote/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/computations/remote/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3302 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/computations/remote/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.181332 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7120 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.182332 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.185332 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/
--rw-rw-rw-   0 root         (0) root         (0)     2662 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23600 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/external_op.py
--rw-rw-rw-   0 root         (0) root         (0)     3011 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/imblearn.py
--rw-rw-rw-   0 root         (0) root         (0)    10321 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/numpy.py
--rw-rw-rw-   0 root         (0) root         (0)    21505 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/optbinning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.187332 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/pandas/
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8155 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
--rw-rw-rw-   0 root         (0) root         (0)    31872 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py
--rw-rw-rw-   0 root         (0) root         (0)    78764 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)    37561 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
--rw-rw-rw-   0 root         (0) root         (0)     2807 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
--rw-rw-rw-   0 root         (0) root         (0)    34976 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.188332 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/shap/
--rw-rw-rw-   0 root         (0) root         (0)     4162 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/shap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26932 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/shap/explainer.py
--rw-rw-rw-   0 root         (0) root         (0)    13453 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/shap/maskers.py
--rw-rw-rw-   0 root         (0) root         (0)    14139 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/shap/plots.py
--rw-rw-rw-   0 root         (0) root         (0)     6514 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/shap/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.192332 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/
--rw-rw-rw-   0 root         (0) root         (0)      335 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20941 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
--rw-rw-rw-   0 root         (0) root         (0)     1902 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
--rw-rw-rw-   0 root         (0) root         (0)    38069 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
--rw-rw-rw-   0 root         (0) root         (0)     1678 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
--rw-rw-rw-   0 root         (0) root         (0)     2084 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
--rw-rw-rw-   0 root         (0) root         (0)     9874 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     3294 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
--rw-rw-rw-   0 root         (0) root         (0)    12690 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     8598 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     4340 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     2645 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
--rw-rw-rw-   0 root         (0) root         (0)     2884 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/skopt.py
--rw-rw-rw-   0 root         (0) root         (0)    25448 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/std.py
--rw-rw-rw-   0 root         (0) root         (0)     3011 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14158 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/xgboost.py
--rw-rw-rw-   0 root         (0) root         (0)    13494 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.196332 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17193 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
--rw-rw-rw-   0 root         (0) root         (0)     1625 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/error_estimation.py
--rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/extract.py
--rw-rw-rw-   0 root         (0) root         (0)    12256 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2922 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py
--rw-rw-rw-   0 root         (0) root         (0)    13308 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/get_item.py
--rw-rw-rw-   0 root         (0) root         (0)    11420 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/project.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/push_sql.py
--rw-rw-rw-   0 root         (0) root         (0)     8639 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.196332 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/sampling/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/sampling/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3647 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py
--rw-rw-rw-   0 root         (0) root         (0)     8885 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/select_table.py
--rw-rw-rw-   0 root         (0) root         (0)     2462 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/shuffle.py
--rw-rw-rw-   0 root         (0) root         (0)     9522 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/standard_op.py
--rw-rw-rw-   0 root         (0) root         (0)    11403 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/synthetic.py
--rw-rw-rw-   0 root         (0) root         (0)    13558 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/to_small_data.py
--rw-rw-rw-   0 root         (0) root         (0)    27871 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.197332 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/source/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/source/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/source/privacy_params.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/source/random_seed.py
--rw-rw-rw-   0 root         (0) root         (0)     3320 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/source/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.198332 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/sql_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/sql_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8985 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/sql_utils/bigdata.py
--rw-rw-rw-   0 root         (0) root         (0)     5703 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/sql_utils/queries.py
--rw-rw-rw-   0 root         (0) root         (0)    10574 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/manager/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/marginals.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/multiplicity.py
--rw-rw-rw-   0 root         (0) root         (0)     3376 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3004 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/predicate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.213332 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/
--rw-rw-rw-   0 root         (0) root         (0)     2628 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/attribute.proto
--rw-r--r--   0 root         (0) root         (0)     1507 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/attribute_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/bounds.proto
--rw-r--r--   0 root         (0) root         (0)     1712 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/bounds_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2160 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/bounds_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/constraint.proto
--rw-r--r--   0 root         (0) root         (0)     1964 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/constraint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3236 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/constraint_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1340 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/dataset.proto
--rw-r--r--   0 root         (0) root         (0)     3941 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/dataset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9653 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/dataset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/links.proto
--rw-r--r--   0 root         (0) root         (0)     2557 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/links_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4178 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/links_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/manager.proto
--rw-r--r--   0 root         (0) root         (0)     1417 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1638 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/manager_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/marginals.proto
--rw-r--r--   0 root         (0) root         (0)     1739 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/marginals_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2169 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/marginals_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/multiplicity.proto
--rw-r--r--   0 root         (0) root         (0)     1777 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/multiplicity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2178 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/multiplicity_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/path.proto
--rw-r--r--   0 root         (0) root         (0)     1449 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/path_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/path_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/predicate.proto
--rw-r--r--   0 root         (0) root         (0)     2416 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/predicate_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4839 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/predicate_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      259 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/proto_container.proto
--rw-r--r--   0 root         (0) root         (0)     1634 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/proto_container_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1821 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/proto_container_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      629 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/relation.proto
--rw-r--r--   0 root         (0) root         (0)     1545 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/relation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2606 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/relation_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1798 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/scalar.proto
--rw-r--r--   0 root         (0) root         (0)     3904 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/scalar_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9843 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/scalar_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      694 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/schema.proto
--rw-r--r--   0 root         (0) root         (0)     2611 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/schema_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4578 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/schema_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/size.proto
--rw-r--r--   0 root         (0) root         (0)     1689 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/size_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2154 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/size_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3909 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/statistics.proto
--rw-r--r--   0 root         (0) root         (0)    11222 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)    32747 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/statistics_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      646 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/status.proto
--rw-r--r--   0 root         (0) root         (0)     3258 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6181 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     7234 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/transform.proto
--rw-r--r--   0 root         (0) root         (0)    17351 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/transform_pb2.py
--rw-r--r--   0 root         (0) root         (0)    50851 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/transform_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4567 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/type.proto
--rw-r--r--   0 root         (0) root         (0)     9784 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/type_pb2.py
--rw-r--r--   0 root         (0) root         (0)    30590 2024-05-24 09:13:24.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/type_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3948 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/utilities.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    13753 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     4757 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/size.py
--rw-rw-rw-   0 root         (0) root         (0)    43603 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)    17261 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.214332 sarus_data_spec_public-4.0.2/sarus_data_spec/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14527 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/storage/local.py
--rw-rw-rw-   0 root         (0) root         (0)     5606 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/storage/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3084 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/storage/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    41088 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/transform.py
--rw-rw-rw-   0 root         (0) root         (0)   123255 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/type.py
--rw-rw-rw-   0 root         (0) root         (0)    40943 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     4998 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/sarus_data_spec/variant_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:13:35.216332 sarus_data_spec_public-4.0.2/sarus_data_spec_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)      656 2024-05-24 09:13:35.000000 sarus_data_spec_public-4.0.2/sarus_data_spec_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9212 2024-05-24 09:13:35.000000 sarus_data_spec_public-4.0.2/sarus_data_spec_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 09:13:35.000000 sarus_data_spec_public-4.0.2/sarus_data_spec_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 09:13:35.000000 sarus_data_spec_public-4.0.2/sarus_data_spec_public.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      125 2024-05-24 09:13:35.000000 sarus_data_spec_public-4.0.2/sarus_data_spec_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-24 09:13:35.000000 sarus_data_spec_public-4.0.2/sarus_data_spec_public.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     7045 2024-05-24 09:13:35.217332 sarus_data_spec_public-4.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1186 2024-05-24 09:13:01.000000 sarus_data_spec_public-4.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.184986 sarus_data_spec_public-4.0.2.dev0/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      661 2024-05-20 12:26:15.184986 sarus_data_spec_public-4.0.2.dev0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.141986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/
+-rwxrwxrwx   0 root         (0) root         (0)      947 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.143986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8510 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/admin_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2354 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/array.py
+-rw-rw-rw-   0 root         (0) root         (0)     7389 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2100 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/pandas_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6266 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    10718 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)     4646 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/bounds.py
+-rw-rw-rw-   0 root         (0) root         (0)     4364 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.144986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/context/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/context/public.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/context/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/context/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    21819 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.146986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4997 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    22994 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11623 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3438 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.148986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17255 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/parameter_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/privacy_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     5717 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/recursive_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)    28910 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     5355 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8867 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     9582 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/json_serialisation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.149986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7850 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/async_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    32667 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6724 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/cache_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.149986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9104 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.150986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/local/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2583 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/local/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.151986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/remote/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/remote/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/remote/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.151986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7120 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.151986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.155986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/
+-rw-rw-rw-   0 root         (0) root         (0)     2662 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24946 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/external_op.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/imblearn.py
+-rw-rw-rw-   0 root         (0) root         (0)    10321 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)    21505 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/optbinning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.156986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8155 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
+-rw-rw-rw-   0 root         (0) root         (0)    31872 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)    78764 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)    37561 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)    34976 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.158986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/
+-rw-rw-rw-   0 root         (0) root         (0)     4162 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26932 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)    13453 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/maskers.py
+-rw-rw-rw-   0 root         (0) root         (0)    14139 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     6514 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.160986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20941 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38069 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
+-rw-rw-rw-   0 root         (0) root         (0)     1678 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
+-rw-rw-rw-   0 root         (0) root         (0)     9874 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     3294 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    12690 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     8598 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4340 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2884 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/skopt.py
+-rw-rw-rw-   0 root         (0) root         (0)    25448 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/std.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14158 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/xgboost.py
+-rw-rw-rw-   0 root         (0) root         (0)    13273 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.164986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17193 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1625 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/error_estimation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    12256 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2922 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    13308 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/get_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11420 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/push_sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8639 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.165986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/sampling/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/sampling/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/shuffle.py
+-rw-rw-rw-   0 root         (0) root         (0)     9522 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/standard_op.py
+-rw-rw-rw-   0 root         (0) root         (0)    11403 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/synthetic.py
+-rw-rw-rw-   0 root         (0) root         (0)    13558 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/to_small_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    27871 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.166986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/source/privacy_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/source/random_seed.py
+-rw-rw-rw-   0 root         (0) root         (0)     3320 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/source/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.166986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/sql_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/sql_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8985 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/sql_utils/bigdata.py
+-rw-rw-rw-   0 root         (0) root         (0)     5703 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/sql_utils/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)    10574 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/marginals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/multiplicity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3376 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/predicate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.181986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/attribute.proto
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/attribute_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/bounds.proto
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/bounds_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/bounds_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/constraint.proto
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/constraint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3236 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/constraint_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/dataset.proto
+-rw-r--r--   0 root         (0) root         (0)     3941 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/dataset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9653 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/dataset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/links.proto
+-rw-r--r--   0 root         (0) root         (0)     2557 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/links_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4178 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/links_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/manager.proto
+-rw-r--r--   0 root         (0) root         (0)     1417 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/manager_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/manager_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/marginals.proto
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/marginals_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/marginals_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/multiplicity.proto
+-rw-r--r--   0 root         (0) root         (0)     1777 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/multiplicity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/multiplicity_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/path.proto
+-rw-r--r--   0 root         (0) root         (0)     1449 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/path_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/path_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/predicate.proto
+-rw-r--r--   0 root         (0) root         (0)     2416 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/predicate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/predicate_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      259 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/proto_container.proto
+-rw-r--r--   0 root         (0) root         (0)     1634 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/proto_container_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/proto_container_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      629 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/relation.proto
+-rw-r--r--   0 root         (0) root         (0)     1545 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/relation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/relation_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/scalar.proto
+-rw-r--r--   0 root         (0) root         (0)     3904 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/scalar_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9843 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/scalar_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      694 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/schema.proto
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/schema_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/schema_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/size.proto
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/size_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/size_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/statistics.proto
+-rw-r--r--   0 root         (0) root         (0)    11222 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/statistics_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    32747 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/statistics_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      646 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/status.proto
+-rw-r--r--   0 root         (0) root         (0)     3258 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6181 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     7135 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/transform.proto
+-rw-r--r--   0 root         (0) root         (0)    17096 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/transform_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    49955 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/transform_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4567 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/type.proto
+-rw-r--r--   0 root         (0) root         (0)     9784 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    30590 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/type_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3948 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/utilities.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    13753 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4757 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/size.py
+-rw-rw-rw-   0 root         (0) root         (0)    43603 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)    17261 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.182986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14527 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/storage/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     5606 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/storage/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3084 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/storage/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    40753 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)   123255 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/type.py
+-rw-rw-rw-   0 root         (0) root         (0)    40943 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4998 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/variant_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.184986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      661 2024-05-20 12:26:15.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9149 2024-05-20 12:26:15.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 12:26:15.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 12:26:15.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      125 2024-05-20 12:26:15.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-20 12:26:15.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     6984 2024-05-20 12:26:15.185986 sarus_data_spec_public-4.0.2.dev0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1191 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/setup.py
```

### Comparing `sarus_data_spec_public-4.0.2/PKG-INFO` & `sarus_data_spec_public-4.0.2.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus_data_spec_public
-Version: 4.0.2
+Version: 4.0.2.dev0
 Summary: A library to manage Sarus datasets
 Home-page: 
 Download-URL: 
 Author: Sarus Technologies
 Author-email: 
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/__init__.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "VariantConstraint",
 ]
 
 """A library to manage Sarus datasets"""
 # pylint: disable=unused-variable
 
 PACKAGE_NAME: Final[str] = "sarus_data_spec"
-VERSION: Final[str] = "4.0.2"
+VERSION: Final[str] = "4.0.2.dev0"
 
 try:
     import sarus_data_spec.context.worker as sw
 
     push_global_context(sw.WorkerContext())
 except ModuleNotFoundError as exception:
     if exception.name == "sarus_data_spec.context.worker":
```

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/arrow/admin_utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/admin_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/arrow/array.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/array.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/arrow/conversion.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/conversion.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/arrow/pandas_utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/arrow/schema.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/arrow/type.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/attribute.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/attribute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/base.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/bounds.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/bounds.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/constants.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,7 +164,11 @@
 # Model checkpoints
 TRAIN_STATE = "state"
 MODEL_NAME = "model_name"
 PROMPT = "prompt"
 
 # relationship spec
 SHARED_ID_SPACES = "shared-id-spaces"
+
+
+# sarus default output (for empty mock/synthetic)
+SARUS_DEFAULT_OUTPUT = "sarus_default_output"
```

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/context/public.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/context/public.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/context/typing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/context/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/dataset.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_rewriter/base.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_rewriter/simple_rules.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_rewriter/typing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_rewriter/utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_validator/base.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_validator/parameter_kind.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/parameter_kind.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_validator/privacy_limit.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/privacy_limit.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_validator/recursive_validator.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/recursive_validator.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_validator/signature.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/signature.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_validator/simple_rules.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/dataspec_validator/typing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/deprecation.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/deprecation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/factory.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/factory.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/json_serialisation.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/json_serialisation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import base64
 from datetime import date, datetime, time, timedelta, timezone
 from typing import Any
 import json
 import sys
 
 from dateutil.parser import parse
 import numpy as np
 import pandas as pd
+import pyarrow as pa
+import pyarrow.ipc as ipc
 
 
 class SarusJSONEncoder(json.JSONEncoder):
     def default(self, obj: Any) -> Any:
         if isinstance(obj, np.ndarray):
             return {"_type": "numpy.ndarray", "data": obj.tolist()}
         elif isinstance(obj, pd.DataFrame):
@@ -99,14 +102,26 @@
                 "_type": "range",
                 "data": {
                     '"start"': obj.start,
                     '"stop"': obj.stop,
                     '"step"': obj.step,
                 },
             }
+        elif isinstance(obj, pa.Table):
+            sink = pa.BufferOutputStream()
+            writer = ipc.new_stream(sink, obj.schema)
+            writer.write_table(obj)
+            writer.close()
+            serialized_data = (
+                sink.getvalue()
+            )  # This is the serialized data in a byte array format
+            base64_encoded_data = base64.b64encode(serialized_data).decode(
+                "utf-8"
+            )
+            return {"_type": "pa.Table", "data": base64_encoded_data}
         return super().default(obj)
 
     def encode_obj(self, obj: Any) -> Any:
         if isinstance(obj, tuple):
             return {
                 "_type": "tuple",
                 "data": [self.encode_obj(v) for v in obj],
@@ -194,14 +209,20 @@
                         raise ValueError("Invalid module name")
                 elif obj["_type"] == "dtype":
                     return pd.api.types.pandas_dtype(data)
                 elif obj["_type"] == "slice":
                     return slice(*data)
                 elif obj["_type"] == "range":
                     return range(data["start"], data["stop"], data["step"])
+                elif obj["_type"] == "pa.Table":
+                    binary_data = base64.b64decode(obj["data"])
+                    buffer = pa.py_buffer(binary_data)
+                    reader = ipc.open_stream(buffer)
+                    deserialized_table = reader.read_all()
+                    return deserialized_table
             return {self.decode(k): self.decode_obj(v) for k, v in obj.items()}
         elif isinstance(obj, list):
             return [self.decode_obj(v) for v in obj]
         return obj
 
     @classmethod
     def decode_bytes(cls, b: bytes, *args: Any, **kwargs: Any) -> Any:
```

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/async_utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/async_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,23 @@
 
 async def async_iter(data_list: t.Collection[T]) -> t.AsyncIterator[T]:
     """Convert a collection into an AsyncIterator."""
     for data in data_list:
         yield data
 
 
+async def is_async_iterator_empty(
+    ait: t.AsyncIterator[T],
+) -> t.Tuple[bool, t.AsyncIterator[T]]:
+    items = []
+    async for item in ait:
+        items.append(item)
+    return len(items) == 0, async_iter(items)
+
+
 async def decoupled_async_iter(
     source: t.AsyncIterator[T], buffer_size: int = 100
 ) -> t.AsyncIterator[T]:
     """Create a consumer/producer pattern using an asyncio.Queue."""
     queue: asyncio.Queue = asyncio.Queue(maxsize=buffer_size)
 
     async def producer() -> None:
```

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/base.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/cache_utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/cache_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/computations/base.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/computations/local/base.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/local/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/computations/local/schema.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/local/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/computations/remote/base.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/remote/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/base.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/__init__.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/external_op.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/external_op.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,19 @@
     compute_admin_data,
     create_admin_columns,
     merge_data_and_admin,
 )
 from sarus_data_spec.arrow.array import fit_array_to_schema_type_async_gen
 from sarus_data_spec.arrow.conversion import to_pyarrow_table
 from sarus_data_spec.arrow.schema import type_from_arrow_schema
-from sarus_data_spec.constants import MAX_MAX_MULT, MULTIPLICITY
+from sarus_data_spec.constants import (
+    MAX_MAX_MULT,
+    MULTIPLICITY,
+    SARUS_DEFAULT_OUTPUT,
+)
 from sarus_data_spec.dataset import Dataset
 from sarus_data_spec.dataspec_validator.signature import (
     SarusBoundSignature,
     SarusSignature,
     SarusSignatureValue,
 )
 from sarus_data_spec.dataspec_validator.typing import PUPKind
@@ -376,14 +380,40 @@
         transform = self.scalar.transform()
         ds_args, ds_kwargs = self.scalar.parents()
         return await async_compute_external_value(
             transform, *ds_args, **ds_kwargs
         )
 
 
+def has_sarus_default_output(external_transform: st.Transform) -> bool:
+    _, py_kwargs, _, _ = static_arguments(external_transform)
+    return SARUS_DEFAULT_OUTPUT in py_kwargs
+
+
+def sarus_default_output(external_transform: st.Transform) -> pa.Table:
+    _, py_kwargs, _, _ = static_arguments(external_transform)
+    if SARUS_DEFAULT_OUTPUT in py_kwargs:
+        default_output = py_kwargs[SARUS_DEFAULT_OUTPUT]
+        if isinstance(default_output, pa.Table):
+            return default_output
+        elif isinstance(default_output, pd.DataFrame):
+            default_table = pa.Table.from_pandas(
+                default_output, preserve_index=False
+            )
+            return default_table
+        else:
+            raise NotImplementedError(
+                f"Type {default_output} for the default output is not supported."
+            )
+    else:
+        raise ValueError(
+            f"No sarus default output for this transform: {external_transform.uuid()}"
+        )
+
+
 async def async_compute_external_value(
     transform: st.Transform,
     *ds_args: t.Union[st.DataSpec, st.Transform],
     **ds_kwargs: t.Union[st.DataSpec, st.Transform],
 ) -> t.Any:
     """Compute the value of an external transform applied on Dataspecs.
 
@@ -622,8 +652,17 @@
         table = merge_data_and_admin(data_table, output_admin_data)
 
     else:
         result = await implementation.compute(bound_signature)
         data_table = to_pyarrow_table(result)
         table = create_admin_columns(data_table)
 
-    return async_iter(table.to_batches(max_chunksize=batch_size))
+    if table.num_rows > 0:
+        ait = async_iter(table.to_batches(max_chunksize=batch_size))
+    # use default value if it exists
+    elif has_sarus_default_output(dataset.transform()):
+        default_table = sarus_default_output(dataset.transform())
+        ait = async_iter(default_table.to_batches(max_chunksize=batch_size))
+    else:
+        ait = async_iter([])
+
+    return ait
```

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/imblearn.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/imblearn.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/numpy.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/numpy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/optbinning.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/optbinning.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/scipy.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/scipy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/shap/explainer.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/explainer.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/shap/maskers.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/maskers.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/shap/plots.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/plots.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/shap/utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/skopt.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/skopt.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/std.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/std.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/typing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/external/xgboost.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/routing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/routing.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,14 @@
     Filter,
     FilterStaticChecker,
 )
 from sarus_data_spec.manager.ops.processor.standard.get_item import (
     GetItem,
     GetItemStaticChecker,
 )
-from sarus_data_spec.manager.ops.processor.standard.select_table import (
-    SelectTable,
-    SelectTableStaticChecker,
-)
 from sarus_data_spec.manager.ops.processor.standard.project import (
     Project,
     ProjectStaticChecker,
 )
 from sarus_data_spec.manager.ops.processor.standard.to_small_data import (
     ToSmallData,
     ToSmallDataStaticChecker,
@@ -247,16 +243,14 @@
         return Project, ProjectStaticChecker
     elif transform.spec() == "shuffle":
         return Shuffle, ShuffleStaticChecker
     elif transform.spec() == "synthetic":
         return Synthetic, SyntheticStaticChecker
     elif transform.spec() == "get_item":
         return GetItem, GetItemStaticChecker
-    elif transform.spec() == "select_table":
-        return SelectTable, SelectTableStaticChecker
     elif transform.spec() == "assign_budget":
         return AssignBudget, AssignBudgetStaticChecker
     elif transform.spec() == "group_by_pe":
         return GroupByPE, GroupByPEStaticChecker
     elif transform.name() == "Transcode":
         return Transcode, TranscodeStaticChecker
     elif transform.spec() == "select_sql":
```

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/error_estimation.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/error_estimation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/extract.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/extract.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/filter.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/filter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/get_item.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/get_item.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/project.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/project.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/push_sql.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/push_sql.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/sample.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/select_table.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/standard_op.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,238 +1,267 @@
+import hashlib
+import logging
 import typing as t
-import pyarrow as pa
-import numpy as np
-import pyarrow.compute as pc
 import warnings
 
-from sarus_data_spec.arrow.array import convert_record_batch
-from sarus_data_spec.constants import (
-    DATA,
-    DATASET_SLUGNAME,
-    MULTIPLICITY,
-)
-from sarus_data_spec.manager.ops.processor.standard.standard_op import (  # noqa: E501
-    StandardDatasetImplementation,
-    StandardDatasetStaticChecker,
-)
+import pyarrow as pa
 
 from sarus_data_spec.dataset import Dataset
-from sarus_data_spec.path import Path, straight_path
-from sarus_data_spec.marginals import marginals as marg_builder
-from sarus_data_spec.multiplicity import multiplicity as multiplicity_builder
-from sarus_data_spec.size import size as size_builder
-from sarus_data_spec.bounds import bounds as bounds_builder
-from sarus_data_spec.schema import schema
-import sarus_data_spec.type as sdt
-import sarus_data_spec.typing as st
+from sarus_data_spec.manager.ops.base import (
+    DatasetImplementation,
+    DatasetStaticChecker,
+    DataspecStaticChecker,
+    ScalarImplementation,
+    _ensure_batch_correct,
+)
+from sarus_data_spec.typing import Path
 
 try:
-    import sqlalchemy as sa
+    from sarus_data_spec.manager.ops.sql_utils.table_mapping import (
+        name_encoder,
+        table_mapping,
+    )
 except ModuleNotFoundError:
-    warnings.warn("sqlalchemy not installed. No sampling on bigdata")
-
-
+    warnings.warn("table_mapping not found. Cannot send sql queries.")
 try:
-    from sarus_data_spec.manager.ops.sql_utils.bigdata import (
-        path_to_quoted_string,
-        sqlalchemy_query_to_string,
-    )
-    from sarus_data_spec.manager.ops.sql_utils.schema_translations import (
-        async_sa_metadata_from_dataset,
+    from sarus_data_spec.manager.ops.sql_utils.queries import (
+        rename_and_compose_queries,
     )
 except ModuleNotFoundError:
-    warnings.warn("sql utils not installed.")
+    warnings.warn("Queries composition not available.")
+from sarus_data_spec.scalar import Scalar
+import sarus_data_spec.typing as st
 
-
-class SelectTableStaticChecker(StandardDatasetStaticChecker):
-    async def schema(self) -> st.Schema:
-        parent_schema = await self.parent_schema()
-        path = Path(self.dataset.transform().protobuf().spec.select_table.path)
-        sub_types = parent_schema.data_type().sub_types(path)
-        assert len(sub_types) == 1
-        new_type = sub_types[0]
-        # TODO: update foreign_keys/primary_keys in the type
-        previous_fields = parent_schema.type().children()
-
-        try:
-            parent_stats = (await self.parent_marginals()).statistics()
-            path = Path(
-                self.dataset.transform().protobuf().spec.select_table.path
-            )
-            tab_multiplicity = parent_stats.nodes_statistics(path)[
-                0
-            ].multiplicity()
-            properties = {MULTIPLICITY: str(tab_multiplicity)}
-        except Exception:
-            properties = {}
-        if DATA in previous_fields.keys():
-            previous_fields[DATA] = new_type
-            new_type = sdt.Struct(fields=previous_fields)
-        return schema(
-            self.dataset,
-            schema_type=new_type,
-            privacy_unit_tracking_paths=None,
-            name=self.dataset.properties().get(DATASET_SLUGNAME, None),
-            properties=properties,
-        )
+logger = logging.getLogger(__name__)
 
 
-class SelectTable(StandardDatasetImplementation):
-    """Computes schema and arrow
-    batches for a dataspec transformed by
-    a select_table transform
+class StandardDatasetStaticChecker(DatasetStaticChecker):
+    def parent(self, kind: str = "dataset") -> t.Union[st.Dataset, st.Scalar]:
+        return parent(self.dataset, kind=kind)
+
+    async def parent_schema(self) -> st.Schema:
+        parent = self.parent(kind="dataset")
+        assert isinstance(parent, Dataset)
+        return await parent.manager().async_schema(parent)
+
+    async def parent_marginals(self) -> st.Marginals:
+        parent = self.parent(kind="dataset")
+        assert isinstance(parent, Dataset)
+        return await parent.manager().async_marginals(parent)
+
+    def pup_token(self, public_context: t.Collection[str]) -> t.Optional[str]:
+        """By default we implement that the transform inherits the PUP status
+        but changes the PUP token."""
+        parent_token = self.parent().pup_token()
+        if parent_token is None:
+            return None
+
+        transform = self.dataset.transform()
+        h = hashlib.md5(usedforsecurity=False)
+        h.update(parent_token.encode("ascii"))
+        h.update(transform.protobuf().SerializeToString())
+
+        return h.hexdigest()
+
+    def rewritten_pup_token(
+        self, public_context: t.Collection[str]
+    ) -> t.Optional[str]:
+        """By default we implement that the transform inherits the PUP status
+        but changes the PUP token."""
+        parent_token = self.parent().rewritten_pup_token()
+        if parent_token is None:
+            return None
+
+        transform = self.dataset.transform()
+        h = hashlib.md5(usedforsecurity=False)
+        h.update(parent_token.encode("ascii"))
+        h.update(transform.protobuf().SerializeToString())
+
+        return h.hexdigest()
+
+
+class StandardDatasetImplementation(DatasetImplementation):
+    """Object that executes first routing among ops between
+    transformed/source and processor
     """
 
-    async def to_arrow(
-        self, batch_size: int
-    ) -> t.AsyncIterator[pa.RecordBatch]:
-        previous_ds = t.cast(Dataset, self.parent())
-        path = Path(self.dataset.transform().protobuf().spec.select_table.path)
-        parent_schema = await self.parent_schema()
+    def parents(self) -> t.List[t.Union[st.DataSpec, st.Transform]]:
+        return parents(self.dataset)
 
-        async def select_table_func(
-            batch: pa.RecordBatch,
-        ) -> pa.Array:
-            array = convert_record_batch(
-                record_batch=batch, _type=parent_schema.type()
-            )
+    def parent(self, kind: str = "dataset") -> t.Union[st.Dataset, st.Scalar]:
+        return parent(self.dataset, kind=kind)
 
-            if DATA in parent_schema.type().children():
-                old_arrays = array.flatten()
-                idx_data = array.type.get_field_index(DATA)
-                array = old_arrays[idx_data]
-                updated_array, filter_indices = select_table(
-                    _type=parent_schema.data_type(),
-                    array=array,
-                    path=path,
-                )
-                old_arrays[idx_data] = updated_array
+    async def parent_to_arrow(
+        self, batch_size: int = 10000
+    ) -> t.AsyncIterator[pa.RecordBatch]:
+        parent = self.parent(kind="dataset")
+        assert isinstance(parent, Dataset)
+        parent_iterator = await parent.manager().async_to_arrow(
+            parent, batch_size=batch_size
+        )
+        return await self.decoupled_async_iter(parent_iterator)
 
-                new_struct = pa.StructArray.from_arrays(
-                    old_arrays,
-                    names=list(parent_schema.type().children().keys()),
-                )
-                return new_struct.filter(filter_indices)
+    async def parent_schema(self) -> st.Schema:
+        parent = self.parent(kind="dataset")
+        assert isinstance(parent, Dataset)
+        return await parent.manager().async_schema(parent)
+
+    async def parent_value(self) -> t.Any:
+        parent = self.parent(kind="scalar")
+        assert isinstance(parent, Scalar)
+        return await parent.manager().async_value(parent)
+
+    async def parent_size(self) -> st.Size:
+        parent = self.parent(kind="dataset")
+        assert isinstance(parent, Dataset)
+        return await parent.manager().async_size(parent)
+
+    async def parent_multiplicity(self) -> st.Multiplicity:
+        parent = self.parent(kind="dataset")
+        assert isinstance(parent, Dataset)
+        return await parent.manager().async_multiplicity(parent)
+
+    async def parent_bounds(self) -> st.Bounds:
+        parent = self.parent(kind="dataset")
+        assert isinstance(parent, Dataset)
+        return await parent.manager().async_bounds(parent)
+
+    async def parent_marginals(self) -> st.Marginals:
+        parent = self.parent(kind="dataset")
+        assert isinstance(parent, Dataset)
+        return await parent.manager().async_marginals(parent)
 
-            updated_array, filter_indices = select_table(
-                array=array, path=path, _type=parent_schema.data_type()
-            )
-            if isinstance(updated_array, pa.StructArray):
-                return updated_array.filter(filter_indices)
-            else:
-                old_arrays[idx_data] = updated_array
-
-                new_struct = pa.StructArray.from_arrays(
-                    old_arrays,
-                    names=[path.to_strings_list()[0][-1]],
-                )
-                return new_struct.filter(filter_indices)
+    async def ensure_batch_correct(
+        self,
+        async_iterator: t.AsyncIterator[pa.RecordBatch],
+        func_to_apply: t.Callable,
+        batch_size: int,
+    ) -> t.AsyncIterator[pa.RecordBatch]:
+        """Method that executes func_to_apply on each batch
+        of the async_iterator but rather than directly returning
+        the result, it accumulates them and returns them progressively
+        so that each new batch has batch_size."""
 
-        return await self.ensure_batch_correct(
-            async_iterator=await previous_ds.async_to_arrow(
-                batch_size=batch_size
-            ),
-            batch_size=batch_size,
-            func_to_apply=select_table_func,
-        )
+        return _ensure_batch_correct(async_iterator, func_to_apply, batch_size)
 
     async def sql_implementation(
         self,
     ) -> t.Optional[t.Dict[t.Tuple[str, ...], str]]:
-        sqlalchemy_metadata = await async_sa_metadata_from_dataset(
-            t.cast(Dataset, self.parent())
+        """Returns a dict of queries equivalent to the current transform.
+        If the the transform does not change the schema, then return None"""
+        raise NotImplementedError(
+            "No SQL implementation for dataset issued from"
+            f" {self.dataset.transform().spec()} transform."
         )
-        queries: t.Dict[t.Tuple[str, ...], str] = {}
-        table_path = Path(
-            self.dataset.transform().protobuf().spec.select_table.path
-        )
-        curr_path = table_path.to_strings_list()[0]
-        full_tablename = curr_path[1:] if curr_path[0] == DATA else curr_path
-        sa_table_name = path_to_quoted_string(straight_path(full_tablename))
-        sa_table = sqlalchemy_metadata.tables[sa_table_name]
-        table_query = sa.select(sa_table)
-
-        queries[()] = sqlalchemy_query_to_string(table_query)
-        return queries
-
-    async def size(self) -> st.Size:
-        sizes = await self.parent_size()
-        path = Path(self.dataset.transform().protobuf().spec.select_table.path)
-        new_stats = sizes.statistics().nodes_statistics(path)
-        assert len(new_stats) == 1
-        return size_builder(dataset=self.dataset, statistics=new_stats[0])
-
-    async def multiplicity(self) -> st.Multiplicity:
-        multiplicities = await self.parent_multiplicity()
-        path = Path(self.dataset.transform().protobuf().spec.select_table.path)
-        new_stats = multiplicities.statistics().nodes_statistics(path)
-        assert len(new_stats) == 1
-        return multiplicity_builder(
-            dataset=self.dataset, statistics=new_stats[0]
-        )
-
-    async def bounds(self) -> st.Bounds:
-        bounds = await self.parent_bounds()
-        path = Path(self.dataset.transform().protobuf().spec.select_table.path)
-        new_stats = bounds.statistics().nodes_statistics(path)
-        assert len(new_stats) == 1
-        return bounds_builder(dataset=self.dataset, statistics=new_stats[0])
-
-    async def marginals(self) -> st.Marginals:
-        marginals = await self.parent_marginals()
-        path = Path(self.dataset.transform().protobuf().spec.select_table.path)
-        new_stats = marginals.statistics().nodes_statistics(path)
-        assert len(new_stats) == 1
-        return marg_builder(dataset=self.dataset, statistics=new_stats[0])
-
-
-def select_table(
-    array: pa.Array, path: st.Path, _type: st.Type, is_optional: bool = False
-) -> t.Tuple[pa.Array, pa.Array]:
-    """Visitor selecting columns based on the type."""
-
-    class TableSelector(sdt.TypeVisitor_):
-        batch_array: pa.Array = array
-        filter_indices: pa.Array
-
-        def Union(
-            self,
-            fields: t.Mapping[str, st.Type],
-            name: t.Optional[str] = None,
-            properties: t.Optional[t.Mapping[str, str]] = None,
-        ) -> None:
-            if len(path.sub_paths()) == 0:
-                self.batch_array = array
-                self.filter_indices = np.full_like(array, True)
-            else:
-                sub_path = path.sub_paths()[0]
-                idx = array.type.get_field_index(sub_path.label())
-
-                initial_field_selected = self.batch_array.field(
-                    "field_selected"
-                ).to_numpy(zero_copy_only=False)
-
-                self.batch_array, filter_idx = select_table(
-                    array=array.flatten()[idx],
-                    path=sub_path,
-                    _type=fields[sub_path.label()],
-                )
 
-                field_selected = pa.array(
-                    initial_field_selected == sub_path.label(), type=pa.bool_()
+    async def sql(
+        self,
+        query: t.Union[str, t.Dict[str, t.Any]],
+        dialect: t.Optional[st.SQLDialect] = None,
+        batch_size: int = 10000,
+        result_type: t.Optional[st.Type] = None,
+    ) -> t.AsyncIterator[pa.RecordBatch]:
+        """It rewrites and/or composes the query and sends it to the parent."""
+        queries_transform = await self.sql_implementation()
+        current_schema = await self.dataset.manager().async_schema(
+            self.dataset
+        )
+        parent_schema = await self.parent_schema()
+        if (
+            queries_transform is None
+            and current_schema.name() == parent_schema.name()
+        ):
+            parent_query = query
+        else:
+            table_map: dict[Path, tuple[str, ...]] = {}
+            if queries_transform is not None:
+                table_map = t.cast(
+                    dict[Path, tuple[str, ...]],
+                    table_mapping(
+                        tables=current_schema.tables(),
+                        sarus_schema_name=current_schema.name(),
+                        encoded_name_length=10,
+                        encoder_prefix_name=self.dataset.uuid(),
+                    ),
                 )
-                result = pc.and_(field_selected, filter_idx)
-                self.filter_indices = result
+            updated_queries_transform = (
+                {
+                    name_encoder(
+                        names=(self.dataset.uuid(), *tab_name),
+                        length=10,
+                    ): query_str
+                    for tab_name, query_str in queries_transform.items()
+                }
+                if queries_transform is not None
+                else None
+            )
 
-        def Struct(
-            self,
-            fields: t.Mapping[str, st.Type],
-            name: t.Optional[str] = None,
-            properties: t.Optional[t.Mapping[str, str]] = None,
-        ) -> None:
-            self.filter_indices = pa.array(
-                [True] * len(self.batch_array), type=pa.bool_()
+            parent_query = rename_and_compose_queries(
+                query_or_dict=query,
+                curr_path=[],
+                queries_transform=updated_queries_transform,
+                table_map=table_map,
             )
 
-    visitor = TableSelector()
-    _type.accept(visitor)
-    return visitor.batch_array, visitor.filter_indices
+        parent_ds = t.cast(st.Dataset, self.parent(kind="dataset"))
+        logger.info(
+            f"query {parent_query} sent to the "
+            f"parent dataset {parent_ds.uuid()}"
+        )
+        return await parent_ds.manager().async_sql(
+            dataset=parent_ds,
+            query=parent_query,
+            dialect=dialect,
+            batch_size=batch_size,
+            result_type=result_type,
+        )
+
+
+class StandardScalarStaticChecker(DataspecStaticChecker): ...
+
+
+class StandardScalarImplementation(ScalarImplementation):
+    def parent(self, kind: str = "dataset") -> st.DataSpec:
+        return parent(self.scalar, kind=kind)
+
+    def parents(self) -> t.List[t.Union[st.DataSpec, st.Transform]]:
+        return parents(self.scalar)
+
+    async def parent_to_arrow(
+        self, batch_size: int = 10000
+    ) -> t.AsyncIterator[pa.RecordBatch]:
+        parent = self.parent(kind="dataset")
+        assert isinstance(parent, Dataset)
+        parent_iterator = await parent.manager().async_to_arrow(
+            parent, batch_size=batch_size
+        )
+        return await self.decoupled_async_iter(parent_iterator)
+
+    async def parent_schema(self) -> st.Schema:
+        parent = self.parent(kind="dataset")
+        assert isinstance(parent, Dataset)
+        return await parent.manager().async_schema(parent)
+
+    async def parent_value(self) -> t.Any:
+        parent = self.parent(kind="scalar")
+        assert isinstance(parent, Scalar)
+        return await parent.manager().async_value(parent)
+
+
+def parent(dataspec: st.DataSpec, kind: str) -> t.Union[st.Dataset, st.Scalar]:
+    pars = parents(dataspec)
+    if kind == "dataset":
+        parent: t.Union[t.List[Scalar], t.List[Dataset]] = [
+            element for element in pars if isinstance(element, Dataset)
+        ]
+    else:
+        parent = [element for element in pars if isinstance(element, Scalar)]
+    assert len(parent) == 1
+    return parent[0]
+
+
+def parents(
+    dataspec: st.DataSpec,
+) -> t.List[t.Union[st.DataSpec, st.Transform]]:
+    parents_args, parents_kwargs = dataspec.parents()
+    parents_args.extend(parents_kwargs.values())
+    return parents_args
```

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/shuffle.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/shuffle.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/synthetic.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/synthetic.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/to_small_data.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/to_small_data.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/source/routing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/source/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/sql_utils/bigdata.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/sql_utils/bigdata.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/ops/sql_utils/queries.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/sql_utils/queries.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/manager/typing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/marginals.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/marginals.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/multiplicity.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/multiplicity.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/path.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/path.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/predicate.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/predicate.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/__init__.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/attribute_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/attribute_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/bounds_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/bounds_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/bounds_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/bounds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/constraint_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/constraint_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/constraint_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/constraint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/dataset.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/dataset.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/dataset_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/dataset_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/links_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/links_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/links_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/manager_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/manager_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/marginals_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/marginals_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/marginals_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/marginals_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/multiplicity_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/multiplicity_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/multiplicity_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/multiplicity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/path_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/path_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/path_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/path_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/predicate.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/predicate.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/predicate_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/predicate_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/predicate_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/predicate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/proto_container_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/proto_container_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/proto_container_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/proto_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/relation.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/relation.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/relation_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/relation_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/relation_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/relation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/scalar.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/scalar.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/scalar_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/scalar_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/scalar_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/scalar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/schema.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/schema.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/schema_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/schema_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/size_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/size_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/size_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/size_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/statistics.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/statistics.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/statistics_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/statistics_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/statistics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/status.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/status.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/status_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/status_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/status_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/transform.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/transform.proto`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
       DPSelectSql dp_select_sql = 32;
       ErrorEstimation error_estimation = 33;
       FitModel fit_model = 34;
       FitModelDP fit_model_dp = 35;
       GenerateFromModel generate_from_model = 36;
       ToSmallData to_small_data = 37;
       PushSQL push_sql = 38;
-      SelectTable select_table=39;
     }
   }
 
   message External {
     bytes arguments = 1;
     bytes named_arguments = 2;
     OpIdentifier op_identifier = 3;
@@ -331,12 +330,8 @@
     TextKind text_kind = 5;
   }
 
   message GenerateFromModel {
     int32 max_new_tokens = 1;
     double temperature = 2;
   }
-
-  message SelectTable {
-    sarus_data_spec.Path path = 1;
-  }
 }
```

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/transform_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/transform_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,147 +12,145 @@
 
 
 from sarus_data_spec.protobuf import type_pb2 as sarus__data__spec_dot_protobuf_dot_type__pb2
 from sarus_data_spec.protobuf import path_pb2 as sarus__data__spec_dot_protobuf_dot_path__pb2
 from sarus_data_spec.protobuf import scalar_pb2 as sarus__data__spec_dot_protobuf_dot_scalar__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(sarus_data_spec/protobuf/transform.proto\x1a#sarus_data_spec/protobuf/type.proto\x1a#sarus_data_spec/protobuf/path.proto\x1a%sarus_data_spec/protobuf/scalar.proto\"\xbb+\n\tTransform\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0b\n\x03\x64oc\x18\x03 \x01(\t\x12\x1d\n\x04spec\x18\x04 \x01(\x0b\x32\x0f.Transform.Spec\x12.\n\nproperties\x18\x05 \x03(\x0b\x32\x1a.Transform.PropertiesEntry\x12\x12\n\ninversible\x18\x06 \x01(\x08\x12\x19\n\x11schema_preserving\x18\x07 \x01(\x08\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xea\x0e\n\x04Spec\x12\'\n\x08identity\x18\x01 \x01(\x0b\x32\x13.Transform.IdentityH\x00\x12\'\n\x08variable\x18\x02 \x01(\x0b\x32\x13.Transform.VariableH\x00\x12\'\n\x08\x63omposed\x18\x03 \x01(\x0b\x32\x13.Transform.ComposedH\x00\x12%\n\x07project\x18\x04 \x01(\x0b\x32\x12.Transform.ProjectH\x00\x12#\n\x06\x66ilter\x18\x05 \x01(\x0b\x32\x11.Transform.FilterH\x00\x12%\n\x07shuffle\x18\x06 \x01(\x0b\x32\x12.Transform.ShuffleH\x00\x12\x1f\n\x04join\x18\x07 \x01(\x0b\x32\x0f.Transform.JoinH\x00\x12\x1f\n\x04\x63\x61st\x18\x08 \x01(\x0b\x32\x0f.Transform.CastH\x00\x12#\n\x06sample\x18\t \x01(\x0b\x32\x11.Transform.SampleH\x00\x12\x30\n\ruser_settings\x18\n \x01(\x0b\x32\x17.Transform.UserSettingsH\x00\x12?\n\x15privacy_unit_tracking\x18\x0b \x01(\x0b\x32\x1e.Transform.PrivacyUnitTrackingH\x00\x12\'\n\x08\x65xternal\x18\x0c \x01(\x0b\x32\x13.Transform.ExternalH\x00\x12)\n\tsynthetic\x18\r \x01(\x0b\x32\x14.Transform.SyntheticH\x00\x12)\n\ttranscode\x18\x0e \x01(\x0b\x32\x14.Transform.TranscodeH\x00\x12\x38\n\x11inverse_transcode\x18\x0f \x01(\x0b\x32\x1b.Transform.InverseTranscodeH\x00\x12&\n\x08get_item\x18\x10 \x01(\x0b\x32\x12.Transform.GetItemH\x00\x12J\n\x1bprivacy_unit_tracking_paths\x18\x11 \x01(\x0b\x32#.Transform.PrivacyUnitTrackingPathsH\x00\x12\x43\n\x17\x61utomatic_user_settings\x18\x12 \x01(\x0b\x32 .Transform.AutomaticUserSettingsH\x00\x12.\n\x0cpublic_paths\x18\x13 \x01(\x0b\x32\x16.Transform.PublicPathsH\x00\x12\x30\n\rassign_budget\x18\x14 \x01(\x0b\x32\x17.Transform.AssignBudgetH\x00\x12\x36\n\x10\x61utomatic_budget\x18\x15 \x01(\x0b\x32\x1a.Transform.AutomaticBudgetH\x00\x12\x37\n\x10\x61ttribute_budget\x18\x16 \x01(\x0b\x32\x1b.Transform.AttributesBudgetH\x00\x12(\n\tsd_budget\x18\x17 \x01(\x0b\x32\x13.Transform.SDBudgetH\x00\x12,\n\x0b\x64\x65rive_seed\x18\x18 \x01(\x0b\x32\x15.Transform.DeriveSeedH\x00\x12+\n\x0bgroup_by_pe\x18\x19 \x01(\x0b\x32\x14.Transform.GroupByPEH\x00\x12\x34\n\x0fsampling_ratios\x18\x1a \x01(\x0b\x32\x19.Transform.SamplingRatiosH\x00\x12*\n\nselect_sql\x18\x1b \x01(\x0b\x32\x14.Transform.SelectSqlH\x00\x12%\n\x07\x65xtract\x18\x1c \x01(\x0b\x32\x12.Transform.ExtractH\x00\x12\x38\n\x11relationship_spec\x18\x1d \x01(\x0b\x32\x1b.Transform.RelationshipSpecH\x00\x12@\n\x15\x64ifferentiated_sample\x18\x1e \x01(\x0b\x32\x1f.Transform.DifferentiatedSampleH\x00\x12;\n\x13validated_user_type\x18\x1f \x01(\x0b\x32\x1c.Transform.ValidatedUserTypeH\x00\x12/\n\rdp_select_sql\x18  \x01(\x0b\x32\x16.Transform.DPSelectSqlH\x00\x12\x36\n\x10\x65rror_estimation\x18! \x01(\x0b\x32\x1a.Transform.ErrorEstimationH\x00\x12(\n\tfit_model\x18\" \x01(\x0b\x32\x13.Transform.FitModelH\x00\x12-\n\x0c\x66it_model_dp\x18# \x01(\x0b\x32\x15.Transform.FitModelDPH\x00\x12;\n\x13generate_from_model\x18$ \x01(\x0b\x32\x1c.Transform.GenerateFromModelH\x00\x12/\n\rto_small_data\x18% \x01(\x0b\x32\x16.Transform.ToSmallDataH\x00\x12&\n\x08push_sql\x18& \x01(\x0b\x32\x12.Transform.PushSQLH\x00\x12.\n\x0cselect_table\x18\' \x01(\x0b\x32\x16.Transform.SelectTableH\x00\x42\x06\n\x04spec\x1a\xf6\x07\n\x08\x45xternal\x12\x11\n\targuments\x18\x01 \x01(\x0c\x12\x17\n\x0fnamed_arguments\x18\x02 \x01(\x0c\x12\x37\n\rop_identifier\x18\x03 \x01(\x0b\x32 .Transform.External.OpIdentifier\x1a\xd7\x04\n\x0cOpIdentifier\x12&\n\x03std\x18\x01 \x01(\x0b\x32\x17.Transform.External.StdH\x00\x12,\n\x06pandas\x18\x02 \x01(\x0b\x32\x1a.Transform.External.PandasH\x00\x12*\n\x05numpy\x18\x03 \x01(\x0b\x32\x19.Transform.External.NumpyH\x00\x12\x34\n\ntensorflow\x18\x04 \x01(\x0b\x32\x1e.Transform.External.TensorflowH\x00\x12.\n\x07sklearn\x18\x05 \x01(\x0b\x32\x1b.Transform.External.SklearnH\x00\x12?\n\x10pandas_profiling\x18\x06 \x01(\x0b\x32#.Transform.External.PandasProfilingH\x00\x12.\n\x07xgboost\x18\x07 \x01(\x0b\x32\x1b.Transform.External.XGBoostH\x00\x12*\n\x05skopt\x18\x08 \x01(\x0b\x32\x19.Transform.External.SkoptH\x00\x12\x30\n\x08imblearn\x18\t \x01(\x0b\x32\x1c.Transform.External.ImblearnH\x00\x12(\n\x04shap\x18\n \x01(\x0b\x32\x18.Transform.External.ShapH\x00\x12*\n\x05scipy\x18\x0b \x01(\x0b\x32\x19.Transform.External.ScipyH\x00\x12\x34\n\noptbinning\x18\x0c \x01(\x0b\x32\x1e.Transform.External.OptBinningH\x00\x42\x04\n\x02op\x1a\x13\n\x03Std\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x16\n\x06Pandas\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Numpy\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1a\n\nTensorflow\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x17\n\x07Sklearn\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1f\n\x0fPandasProfiling\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x17\n\x07XGBoost\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Skopt\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x18\n\x08Imblearn\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x14\n\x04Shap\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Scipy\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1a\n\nOptBinning\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\n\n\x08Identity\x1a*\n\x08Variable\x12\x10\n\x08position\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x1a\xa9\x01\n\x08\x43omposed\x12\x11\n\ttransform\x18\x01 \x01(\t\x12\x11\n\targuments\x18\x02 \x03(\t\x12@\n\x0fnamed_arguments\x18\x03 \x03(\x0b\x32\'.Transform.Composed.NamedArgumentsEntry\x1a\x35\n\x13NamedArgumentsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x34\n\x07Project\x12)\n\nprojection\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a/\n\x06\x46ilter\x12%\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a\t\n\x07Shuffle\x1a)\n\x04Join\x12!\n\x02on\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a+\n\x04\x43\x61st\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a\x61\n\x06Sample\x12\x12\n\x08\x66raction\x18\x01 \x01(\x01H\x00\x12\x0e\n\x04size\x18\x02 \x01(\x03H\x00\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.ScalarB\x0c\n\nproportion\x1av\n\x0fSchemaInference\x12:\n\x0b\x63\x61st_policy\x18\x01 \x01(\x0e\x32%.Transform.SchemaInference.CastPolicy\"\'\n\nCastPolicy\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bMOST_LIKELY\x10\x01\x1a\x16\n\x07GroupBy\x12\x0b\n\x03key\x18\x01 \x01(\t\x1a[\n\x0bToSmallData\x12\x0c\n\x04size\x18\x01 \x01(\x05\x12\x17\n\x0frandom_sampling\x18\x02 \x01(\x08\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.Scalar\x1a\\\n\x07PushSQL\x12\x1b\n\x13\x64\x61taconnection_name\x18\x01 \x01(\t\x12\x13\n\x0bschema_name\x18\x02 \x01(\t\x12\x12\n\ntable_name\x18\x03 \x01(\t\x12\x0b\n\x03uri\x18\x04 \x01(\t\x1a\x0b\n\tSynthetic\x1a\x0e\n\x0cUserSettings\x1a/\n\x15\x41utomaticUserSettings\x12\x16\n\x0emax_categories\x18\x01 \x01(\x03\x1a\x15\n\x13PrivacyUnitTracking\x1a\x0b\n\tTranscode\x1a\x12\n\x10InverseTranscode\x1ao\n\x14\x44ifferentiatedSample\x12\x12\n\x08\x66raction\x18\x01 \x01(\x01H\x00\x12\x0e\n\x04size\x18\x02 \x01(\x03H\x00\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.ScalarB\x0c\n\nproportion\x1a\x1a\n\x18PrivacyUnitTrackingPaths\x1a\r\n\x0bPublicPaths\x1a.\n\x07GetItem\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\x1a\x0e\n\x0c\x41ssignBudget\x1a\x11\n\x0f\x41utomaticBudget\x1a\x12\n\x10\x41ttributesBudget\x1a\n\n\x08SDBudget\x1a$\n\nDeriveSeed\x12\x16\n\x0erandom_integer\x18\x01 \x01(\x03\x1a\x0b\n\tGroupByPE\x1a\x10\n\x0eSamplingRatios\x1a\x12\n\x10RelationshipSpec\x1a\x88\x01\n\tSelectSql\x12\x0f\n\x05query\x18\x01 \x01(\tH\x00\x12\x34\n\x0f\x61liased_queries\x18\x02 \x01(\x0b\x32\x19.Transform.AliasedQueriesH\x00\x12*\n\x0bsql_dialect\x18\x03 \x01(\x0e\x32\x15.Transform.SQLDialectB\x08\n\x06select\x1a\x8a\x01\n\x0b\x44PSelectSql\x12\x0f\n\x05query\x18\x01 \x01(\tH\x00\x12\x34\n\x0f\x61liased_queries\x18\x02 \x01(\x0b\x32\x19.Transform.AliasedQueriesH\x00\x12*\n\x0bsql_dialect\x18\x03 \x01(\x0e\x32\x15.Transform.SQLDialectB\x08\n\x06select\x1a@\n\x0e\x41liasedQueries\x12.\n\raliased_query\x18\x01 \x03(\x0b\x32\x17.Transform.AliasedQuery\x1a\x42\n\x0c\x41liasedQuery\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\x12\r\n\x05query\x18\x02 \x01(\t\x1a\x17\n\x07\x45xtract\x12\x0c\n\x04size\x18\x01 \x01(\x05\x1a\x13\n\x11ValidatedUserType\x1a\x11\n\x0f\x45rrorEstimation\x1aV\n\x08\x46itModel\x12\x12\n\nbatch_size\x18\x01 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x02 \x01(\x05\x12&\n\ttext_kind\x18\x03 \x01(\x0b\x32\x13.Transform.TextKind\x1aN\n\x08TextKind\x12\x14\n\ntext_field\x18\x01 \x01(\tH\x00\x12\x1f\n\x04\x63hat\x18\x02 \x01(\x0b\x32\x0f.Transform.ChatH\x00\x42\x0b\n\ttext_kind\x1a\x34\n\x04\x43hat\x12\x16\n\x0equestion_field\x18\x01 \x01(\t\x12\x14\n\x0c\x61nswer_field\x18\x02 \x01(\t\x1an\n\nFitModelDP\x12\x12\n\nbatch_size\x18\x01 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x03 \x01(\x05\x12\x14\n\x0cl2_norm_clip\x18\x04 \x01(\x01\x12&\n\ttext_kind\x18\x05 \x01(\x0b\x32\x13.Transform.TextKind\x1a@\n\x11GenerateFromModel\x12\x16\n\x0emax_new_tokens\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x01\x1a\x32\n\x0bSelectTable\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\"\x80\x01\n\nSQLDialect\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08POSTGRES\x10\x01\x12\x0e\n\nSQL_SERVER\x10\x02\x12\n\n\x06MY_SQL\x10\x03\x12\x0b\n\x07SQLLITE\x10\x04\x12\n\n\x06ORACLE\x10\x05\x12\r\n\tBIG_QUERY\x10\x06\x12\x0c\n\x08REDSHIFT\x10\x07\x12\x08\n\x04HIVE\x10\x08\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(sarus_data_spec/protobuf/transform.proto\x1a#sarus_data_spec/protobuf/type.proto\x1a#sarus_data_spec/protobuf/path.proto\x1a%sarus_data_spec/protobuf/scalar.proto\"\xd7*\n\tTransform\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0b\n\x03\x64oc\x18\x03 \x01(\t\x12\x1d\n\x04spec\x18\x04 \x01(\x0b\x32\x0f.Transform.Spec\x12.\n\nproperties\x18\x05 \x03(\x0b\x32\x1a.Transform.PropertiesEntry\x12\x12\n\ninversible\x18\x06 \x01(\x08\x12\x19\n\x11schema_preserving\x18\x07 \x01(\x08\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xba\x0e\n\x04Spec\x12\'\n\x08identity\x18\x01 \x01(\x0b\x32\x13.Transform.IdentityH\x00\x12\'\n\x08variable\x18\x02 \x01(\x0b\x32\x13.Transform.VariableH\x00\x12\'\n\x08\x63omposed\x18\x03 \x01(\x0b\x32\x13.Transform.ComposedH\x00\x12%\n\x07project\x18\x04 \x01(\x0b\x32\x12.Transform.ProjectH\x00\x12#\n\x06\x66ilter\x18\x05 \x01(\x0b\x32\x11.Transform.FilterH\x00\x12%\n\x07shuffle\x18\x06 \x01(\x0b\x32\x12.Transform.ShuffleH\x00\x12\x1f\n\x04join\x18\x07 \x01(\x0b\x32\x0f.Transform.JoinH\x00\x12\x1f\n\x04\x63\x61st\x18\x08 \x01(\x0b\x32\x0f.Transform.CastH\x00\x12#\n\x06sample\x18\t \x01(\x0b\x32\x11.Transform.SampleH\x00\x12\x30\n\ruser_settings\x18\n \x01(\x0b\x32\x17.Transform.UserSettingsH\x00\x12?\n\x15privacy_unit_tracking\x18\x0b \x01(\x0b\x32\x1e.Transform.PrivacyUnitTrackingH\x00\x12\'\n\x08\x65xternal\x18\x0c \x01(\x0b\x32\x13.Transform.ExternalH\x00\x12)\n\tsynthetic\x18\r \x01(\x0b\x32\x14.Transform.SyntheticH\x00\x12)\n\ttranscode\x18\x0e \x01(\x0b\x32\x14.Transform.TranscodeH\x00\x12\x38\n\x11inverse_transcode\x18\x0f \x01(\x0b\x32\x1b.Transform.InverseTranscodeH\x00\x12&\n\x08get_item\x18\x10 \x01(\x0b\x32\x12.Transform.GetItemH\x00\x12J\n\x1bprivacy_unit_tracking_paths\x18\x11 \x01(\x0b\x32#.Transform.PrivacyUnitTrackingPathsH\x00\x12\x43\n\x17\x61utomatic_user_settings\x18\x12 \x01(\x0b\x32 .Transform.AutomaticUserSettingsH\x00\x12.\n\x0cpublic_paths\x18\x13 \x01(\x0b\x32\x16.Transform.PublicPathsH\x00\x12\x30\n\rassign_budget\x18\x14 \x01(\x0b\x32\x17.Transform.AssignBudgetH\x00\x12\x36\n\x10\x61utomatic_budget\x18\x15 \x01(\x0b\x32\x1a.Transform.AutomaticBudgetH\x00\x12\x37\n\x10\x61ttribute_budget\x18\x16 \x01(\x0b\x32\x1b.Transform.AttributesBudgetH\x00\x12(\n\tsd_budget\x18\x17 \x01(\x0b\x32\x13.Transform.SDBudgetH\x00\x12,\n\x0b\x64\x65rive_seed\x18\x18 \x01(\x0b\x32\x15.Transform.DeriveSeedH\x00\x12+\n\x0bgroup_by_pe\x18\x19 \x01(\x0b\x32\x14.Transform.GroupByPEH\x00\x12\x34\n\x0fsampling_ratios\x18\x1a \x01(\x0b\x32\x19.Transform.SamplingRatiosH\x00\x12*\n\nselect_sql\x18\x1b \x01(\x0b\x32\x14.Transform.SelectSqlH\x00\x12%\n\x07\x65xtract\x18\x1c \x01(\x0b\x32\x12.Transform.ExtractH\x00\x12\x38\n\x11relationship_spec\x18\x1d \x01(\x0b\x32\x1b.Transform.RelationshipSpecH\x00\x12@\n\x15\x64ifferentiated_sample\x18\x1e \x01(\x0b\x32\x1f.Transform.DifferentiatedSampleH\x00\x12;\n\x13validated_user_type\x18\x1f \x01(\x0b\x32\x1c.Transform.ValidatedUserTypeH\x00\x12/\n\rdp_select_sql\x18  \x01(\x0b\x32\x16.Transform.DPSelectSqlH\x00\x12\x36\n\x10\x65rror_estimation\x18! \x01(\x0b\x32\x1a.Transform.ErrorEstimationH\x00\x12(\n\tfit_model\x18\" \x01(\x0b\x32\x13.Transform.FitModelH\x00\x12-\n\x0c\x66it_model_dp\x18# \x01(\x0b\x32\x15.Transform.FitModelDPH\x00\x12;\n\x13generate_from_model\x18$ \x01(\x0b\x32\x1c.Transform.GenerateFromModelH\x00\x12/\n\rto_small_data\x18% \x01(\x0b\x32\x16.Transform.ToSmallDataH\x00\x12&\n\x08push_sql\x18& \x01(\x0b\x32\x12.Transform.PushSQLH\x00\x42\x06\n\x04spec\x1a\xf6\x07\n\x08\x45xternal\x12\x11\n\targuments\x18\x01 \x01(\x0c\x12\x17\n\x0fnamed_arguments\x18\x02 \x01(\x0c\x12\x37\n\rop_identifier\x18\x03 \x01(\x0b\x32 .Transform.External.OpIdentifier\x1a\xd7\x04\n\x0cOpIdentifier\x12&\n\x03std\x18\x01 \x01(\x0b\x32\x17.Transform.External.StdH\x00\x12,\n\x06pandas\x18\x02 \x01(\x0b\x32\x1a.Transform.External.PandasH\x00\x12*\n\x05numpy\x18\x03 \x01(\x0b\x32\x19.Transform.External.NumpyH\x00\x12\x34\n\ntensorflow\x18\x04 \x01(\x0b\x32\x1e.Transform.External.TensorflowH\x00\x12.\n\x07sklearn\x18\x05 \x01(\x0b\x32\x1b.Transform.External.SklearnH\x00\x12?\n\x10pandas_profiling\x18\x06 \x01(\x0b\x32#.Transform.External.PandasProfilingH\x00\x12.\n\x07xgboost\x18\x07 \x01(\x0b\x32\x1b.Transform.External.XGBoostH\x00\x12*\n\x05skopt\x18\x08 \x01(\x0b\x32\x19.Transform.External.SkoptH\x00\x12\x30\n\x08imblearn\x18\t \x01(\x0b\x32\x1c.Transform.External.ImblearnH\x00\x12(\n\x04shap\x18\n \x01(\x0b\x32\x18.Transform.External.ShapH\x00\x12*\n\x05scipy\x18\x0b \x01(\x0b\x32\x19.Transform.External.ScipyH\x00\x12\x34\n\noptbinning\x18\x0c \x01(\x0b\x32\x1e.Transform.External.OptBinningH\x00\x42\x04\n\x02op\x1a\x13\n\x03Std\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x16\n\x06Pandas\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Numpy\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1a\n\nTensorflow\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x17\n\x07Sklearn\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1f\n\x0fPandasProfiling\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x17\n\x07XGBoost\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Skopt\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x18\n\x08Imblearn\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x14\n\x04Shap\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Scipy\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1a\n\nOptBinning\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\n\n\x08Identity\x1a*\n\x08Variable\x12\x10\n\x08position\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x1a\xa9\x01\n\x08\x43omposed\x12\x11\n\ttransform\x18\x01 \x01(\t\x12\x11\n\targuments\x18\x02 \x03(\t\x12@\n\x0fnamed_arguments\x18\x03 \x03(\x0b\x32\'.Transform.Composed.NamedArgumentsEntry\x1a\x35\n\x13NamedArgumentsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x34\n\x07Project\x12)\n\nprojection\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a/\n\x06\x46ilter\x12%\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a\t\n\x07Shuffle\x1a)\n\x04Join\x12!\n\x02on\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a+\n\x04\x43\x61st\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a\x61\n\x06Sample\x12\x12\n\x08\x66raction\x18\x01 \x01(\x01H\x00\x12\x0e\n\x04size\x18\x02 \x01(\x03H\x00\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.ScalarB\x0c\n\nproportion\x1av\n\x0fSchemaInference\x12:\n\x0b\x63\x61st_policy\x18\x01 \x01(\x0e\x32%.Transform.SchemaInference.CastPolicy\"\'\n\nCastPolicy\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bMOST_LIKELY\x10\x01\x1a\x16\n\x07GroupBy\x12\x0b\n\x03key\x18\x01 \x01(\t\x1a[\n\x0bToSmallData\x12\x0c\n\x04size\x18\x01 \x01(\x05\x12\x17\n\x0frandom_sampling\x18\x02 \x01(\x08\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.Scalar\x1a\\\n\x07PushSQL\x12\x1b\n\x13\x64\x61taconnection_name\x18\x01 \x01(\t\x12\x13\n\x0bschema_name\x18\x02 \x01(\t\x12\x12\n\ntable_name\x18\x03 \x01(\t\x12\x0b\n\x03uri\x18\x04 \x01(\t\x1a\x0b\n\tSynthetic\x1a\x0e\n\x0cUserSettings\x1a/\n\x15\x41utomaticUserSettings\x12\x16\n\x0emax_categories\x18\x01 \x01(\x03\x1a\x15\n\x13PrivacyUnitTracking\x1a\x0b\n\tTranscode\x1a\x12\n\x10InverseTranscode\x1ao\n\x14\x44ifferentiatedSample\x12\x12\n\x08\x66raction\x18\x01 \x01(\x01H\x00\x12\x0e\n\x04size\x18\x02 \x01(\x03H\x00\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.ScalarB\x0c\n\nproportion\x1a\x1a\n\x18PrivacyUnitTrackingPaths\x1a\r\n\x0bPublicPaths\x1a.\n\x07GetItem\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\x1a\x0e\n\x0c\x41ssignBudget\x1a\x11\n\x0f\x41utomaticBudget\x1a\x12\n\x10\x41ttributesBudget\x1a\n\n\x08SDBudget\x1a$\n\nDeriveSeed\x12\x16\n\x0erandom_integer\x18\x01 \x01(\x03\x1a\x0b\n\tGroupByPE\x1a\x10\n\x0eSamplingRatios\x1a\x12\n\x10RelationshipSpec\x1a\x88\x01\n\tSelectSql\x12\x0f\n\x05query\x18\x01 \x01(\tH\x00\x12\x34\n\x0f\x61liased_queries\x18\x02 \x01(\x0b\x32\x19.Transform.AliasedQueriesH\x00\x12*\n\x0bsql_dialect\x18\x03 \x01(\x0e\x32\x15.Transform.SQLDialectB\x08\n\x06select\x1a\x8a\x01\n\x0b\x44PSelectSql\x12\x0f\n\x05query\x18\x01 \x01(\tH\x00\x12\x34\n\x0f\x61liased_queries\x18\x02 \x01(\x0b\x32\x19.Transform.AliasedQueriesH\x00\x12*\n\x0bsql_dialect\x18\x03 \x01(\x0e\x32\x15.Transform.SQLDialectB\x08\n\x06select\x1a@\n\x0e\x41liasedQueries\x12.\n\raliased_query\x18\x01 \x03(\x0b\x32\x17.Transform.AliasedQuery\x1a\x42\n\x0c\x41liasedQuery\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\x12\r\n\x05query\x18\x02 \x01(\t\x1a\x17\n\x07\x45xtract\x12\x0c\n\x04size\x18\x01 \x01(\x05\x1a\x13\n\x11ValidatedUserType\x1a\x11\n\x0f\x45rrorEstimation\x1aV\n\x08\x46itModel\x12\x12\n\nbatch_size\x18\x01 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x02 \x01(\x05\x12&\n\ttext_kind\x18\x03 \x01(\x0b\x32\x13.Transform.TextKind\x1aN\n\x08TextKind\x12\x14\n\ntext_field\x18\x01 \x01(\tH\x00\x12\x1f\n\x04\x63hat\x18\x02 \x01(\x0b\x32\x0f.Transform.ChatH\x00\x42\x0b\n\ttext_kind\x1a\x34\n\x04\x43hat\x12\x16\n\x0equestion_field\x18\x01 \x01(\t\x12\x14\n\x0c\x61nswer_field\x18\x02 \x01(\t\x1an\n\nFitModelDP\x12\x12\n\nbatch_size\x18\x01 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x03 \x01(\x05\x12\x14\n\x0cl2_norm_clip\x18\x04 \x01(\x01\x12&\n\ttext_kind\x18\x05 \x01(\x0b\x32\x13.Transform.TextKind\x1a@\n\x11GenerateFromModel\x12\x16\n\x0emax_new_tokens\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x01\"\x80\x01\n\nSQLDialect\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08POSTGRES\x10\x01\x12\x0e\n\nSQL_SERVER\x10\x02\x12\n\n\x06MY_SQL\x10\x03\x12\x0b\n\x07SQLLITE\x10\x04\x12\n\n\x06ORACLE\x10\x05\x12\r\n\tBIG_QUERY\x10\x06\x12\x0c\n\x08REDSHIFT\x10\x07\x12\x08\n\x04HIVE\x10\x08\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sarus_data_spec.protobuf.transform_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _TRANSFORM_PROPERTIESENTRY._options = None
   _TRANSFORM_PROPERTIESENTRY._serialized_options = b'8\001'
   _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._options = None
   _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._serialized_options = b'8\001'
   _TRANSFORM._serialized_start=158
-  _TRANSFORM._serialized_end=5721
+  _TRANSFORM._serialized_end=5621
   _TRANSFORM_PROPERTIESENTRY._serialized_start=338
   _TRANSFORM_PROPERTIESENTRY._serialized_end=387
   _TRANSFORM_SPEC._serialized_start=390
-  _TRANSFORM_SPEC._serialized_end=2288
-  _TRANSFORM_EXTERNAL._serialized_start=2291
-  _TRANSFORM_EXTERNAL._serialized_end=3305
-  _TRANSFORM_EXTERNAL_OPIDENTIFIER._serialized_start=2405
-  _TRANSFORM_EXTERNAL_OPIDENTIFIER._serialized_end=3004
-  _TRANSFORM_EXTERNAL_STD._serialized_start=3006
-  _TRANSFORM_EXTERNAL_STD._serialized_end=3025
-  _TRANSFORM_EXTERNAL_PANDAS._serialized_start=3027
-  _TRANSFORM_EXTERNAL_PANDAS._serialized_end=3049
-  _TRANSFORM_EXTERNAL_NUMPY._serialized_start=3051
-  _TRANSFORM_EXTERNAL_NUMPY._serialized_end=3072
-  _TRANSFORM_EXTERNAL_TENSORFLOW._serialized_start=3074
-  _TRANSFORM_EXTERNAL_TENSORFLOW._serialized_end=3100
-  _TRANSFORM_EXTERNAL_SKLEARN._serialized_start=3102
-  _TRANSFORM_EXTERNAL_SKLEARN._serialized_end=3125
-  _TRANSFORM_EXTERNAL_PANDASPROFILING._serialized_start=3127
-  _TRANSFORM_EXTERNAL_PANDASPROFILING._serialized_end=3158
-  _TRANSFORM_EXTERNAL_XGBOOST._serialized_start=3160
-  _TRANSFORM_EXTERNAL_XGBOOST._serialized_end=3183
-  _TRANSFORM_EXTERNAL_SKOPT._serialized_start=3185
-  _TRANSFORM_EXTERNAL_SKOPT._serialized_end=3206
-  _TRANSFORM_EXTERNAL_IMBLEARN._serialized_start=3208
-  _TRANSFORM_EXTERNAL_IMBLEARN._serialized_end=3232
-  _TRANSFORM_EXTERNAL_SHAP._serialized_start=3234
-  _TRANSFORM_EXTERNAL_SHAP._serialized_end=3254
-  _TRANSFORM_EXTERNAL_SCIPY._serialized_start=3256
-  _TRANSFORM_EXTERNAL_SCIPY._serialized_end=3277
-  _TRANSFORM_EXTERNAL_OPTBINNING._serialized_start=3279
-  _TRANSFORM_EXTERNAL_OPTBINNING._serialized_end=3305
-  _TRANSFORM_IDENTITY._serialized_start=3307
-  _TRANSFORM_IDENTITY._serialized_end=3317
-  _TRANSFORM_VARIABLE._serialized_start=3319
-  _TRANSFORM_VARIABLE._serialized_end=3361
-  _TRANSFORM_COMPOSED._serialized_start=3364
-  _TRANSFORM_COMPOSED._serialized_end=3533
-  _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._serialized_start=3480
-  _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._serialized_end=3533
-  _TRANSFORM_PROJECT._serialized_start=3535
-  _TRANSFORM_PROJECT._serialized_end=3587
-  _TRANSFORM_FILTER._serialized_start=3589
-  _TRANSFORM_FILTER._serialized_end=3636
-  _TRANSFORM_SHUFFLE._serialized_start=3638
-  _TRANSFORM_SHUFFLE._serialized_end=3647
-  _TRANSFORM_JOIN._serialized_start=3649
-  _TRANSFORM_JOIN._serialized_end=3690
-  _TRANSFORM_CAST._serialized_start=3692
-  _TRANSFORM_CAST._serialized_end=3735
-  _TRANSFORM_SAMPLE._serialized_start=3737
-  _TRANSFORM_SAMPLE._serialized_end=3834
-  _TRANSFORM_SCHEMAINFERENCE._serialized_start=3836
-  _TRANSFORM_SCHEMAINFERENCE._serialized_end=3954
-  _TRANSFORM_SCHEMAINFERENCE_CASTPOLICY._serialized_start=3915
-  _TRANSFORM_SCHEMAINFERENCE_CASTPOLICY._serialized_end=3954
-  _TRANSFORM_GROUPBY._serialized_start=3956
-  _TRANSFORM_GROUPBY._serialized_end=3978
-  _TRANSFORM_TOSMALLDATA._serialized_start=3980
-  _TRANSFORM_TOSMALLDATA._serialized_end=4071
-  _TRANSFORM_PUSHSQL._serialized_start=4073
-  _TRANSFORM_PUSHSQL._serialized_end=4165
-  _TRANSFORM_SYNTHETIC._serialized_start=4167
-  _TRANSFORM_SYNTHETIC._serialized_end=4178
-  _TRANSFORM_USERSETTINGS._serialized_start=4180
-  _TRANSFORM_USERSETTINGS._serialized_end=4194
-  _TRANSFORM_AUTOMATICUSERSETTINGS._serialized_start=4196
-  _TRANSFORM_AUTOMATICUSERSETTINGS._serialized_end=4243
-  _TRANSFORM_PRIVACYUNITTRACKING._serialized_start=4245
-  _TRANSFORM_PRIVACYUNITTRACKING._serialized_end=4266
-  _TRANSFORM_TRANSCODE._serialized_start=4268
-  _TRANSFORM_TRANSCODE._serialized_end=4279
-  _TRANSFORM_INVERSETRANSCODE._serialized_start=4281
-  _TRANSFORM_INVERSETRANSCODE._serialized_end=4299
-  _TRANSFORM_DIFFERENTIATEDSAMPLE._serialized_start=4301
-  _TRANSFORM_DIFFERENTIATEDSAMPLE._serialized_end=4412
-  _TRANSFORM_PRIVACYUNITTRACKINGPATHS._serialized_start=4414
-  _TRANSFORM_PRIVACYUNITTRACKINGPATHS._serialized_end=4440
-  _TRANSFORM_PUBLICPATHS._serialized_start=4442
-  _TRANSFORM_PUBLICPATHS._serialized_end=4455
-  _TRANSFORM_GETITEM._serialized_start=4457
-  _TRANSFORM_GETITEM._serialized_end=4503
-  _TRANSFORM_ASSIGNBUDGET._serialized_start=4505
-  _TRANSFORM_ASSIGNBUDGET._serialized_end=4519
-  _TRANSFORM_AUTOMATICBUDGET._serialized_start=4521
-  _TRANSFORM_AUTOMATICBUDGET._serialized_end=4538
-  _TRANSFORM_ATTRIBUTESBUDGET._serialized_start=4540
-  _TRANSFORM_ATTRIBUTESBUDGET._serialized_end=4558
-  _TRANSFORM_SDBUDGET._serialized_start=4560
-  _TRANSFORM_SDBUDGET._serialized_end=4570
-  _TRANSFORM_DERIVESEED._serialized_start=4572
-  _TRANSFORM_DERIVESEED._serialized_end=4608
-  _TRANSFORM_GROUPBYPE._serialized_start=4610
-  _TRANSFORM_GROUPBYPE._serialized_end=4621
-  _TRANSFORM_SAMPLINGRATIOS._serialized_start=4623
-  _TRANSFORM_SAMPLINGRATIOS._serialized_end=4639
-  _TRANSFORM_RELATIONSHIPSPEC._serialized_start=4641
-  _TRANSFORM_RELATIONSHIPSPEC._serialized_end=4659
-  _TRANSFORM_SELECTSQL._serialized_start=4662
-  _TRANSFORM_SELECTSQL._serialized_end=4798
-  _TRANSFORM_DPSELECTSQL._serialized_start=4801
-  _TRANSFORM_DPSELECTSQL._serialized_end=4939
-  _TRANSFORM_ALIASEDQUERIES._serialized_start=4941
-  _TRANSFORM_ALIASEDQUERIES._serialized_end=5005
-  _TRANSFORM_ALIASEDQUERY._serialized_start=5007
-  _TRANSFORM_ALIASEDQUERY._serialized_end=5073
-  _TRANSFORM_EXTRACT._serialized_start=5075
-  _TRANSFORM_EXTRACT._serialized_end=5098
-  _TRANSFORM_VALIDATEDUSERTYPE._serialized_start=5100
-  _TRANSFORM_VALIDATEDUSERTYPE._serialized_end=5119
-  _TRANSFORM_ERRORESTIMATION._serialized_start=5121
-  _TRANSFORM_ERRORESTIMATION._serialized_end=5138
-  _TRANSFORM_FITMODEL._serialized_start=5140
-  _TRANSFORM_FITMODEL._serialized_end=5226
-  _TRANSFORM_TEXTKIND._serialized_start=5228
-  _TRANSFORM_TEXTKIND._serialized_end=5306
-  _TRANSFORM_CHAT._serialized_start=5308
-  _TRANSFORM_CHAT._serialized_end=5360
-  _TRANSFORM_FITMODELDP._serialized_start=5362
-  _TRANSFORM_FITMODELDP._serialized_end=5472
-  _TRANSFORM_GENERATEFROMMODEL._serialized_start=5474
-  _TRANSFORM_GENERATEFROMMODEL._serialized_end=5538
-  _TRANSFORM_SELECTTABLE._serialized_start=5540
-  _TRANSFORM_SELECTTABLE._serialized_end=5590
-  _TRANSFORM_SQLDIALECT._serialized_start=5593
-  _TRANSFORM_SQLDIALECT._serialized_end=5721
+  _TRANSFORM_SPEC._serialized_end=2240
+  _TRANSFORM_EXTERNAL._serialized_start=2243
+  _TRANSFORM_EXTERNAL._serialized_end=3257
+  _TRANSFORM_EXTERNAL_OPIDENTIFIER._serialized_start=2357
+  _TRANSFORM_EXTERNAL_OPIDENTIFIER._serialized_end=2956
+  _TRANSFORM_EXTERNAL_STD._serialized_start=2958
+  _TRANSFORM_EXTERNAL_STD._serialized_end=2977
+  _TRANSFORM_EXTERNAL_PANDAS._serialized_start=2979
+  _TRANSFORM_EXTERNAL_PANDAS._serialized_end=3001
+  _TRANSFORM_EXTERNAL_NUMPY._serialized_start=3003
+  _TRANSFORM_EXTERNAL_NUMPY._serialized_end=3024
+  _TRANSFORM_EXTERNAL_TENSORFLOW._serialized_start=3026
+  _TRANSFORM_EXTERNAL_TENSORFLOW._serialized_end=3052
+  _TRANSFORM_EXTERNAL_SKLEARN._serialized_start=3054
+  _TRANSFORM_EXTERNAL_SKLEARN._serialized_end=3077
+  _TRANSFORM_EXTERNAL_PANDASPROFILING._serialized_start=3079
+  _TRANSFORM_EXTERNAL_PANDASPROFILING._serialized_end=3110
+  _TRANSFORM_EXTERNAL_XGBOOST._serialized_start=3112
+  _TRANSFORM_EXTERNAL_XGBOOST._serialized_end=3135
+  _TRANSFORM_EXTERNAL_SKOPT._serialized_start=3137
+  _TRANSFORM_EXTERNAL_SKOPT._serialized_end=3158
+  _TRANSFORM_EXTERNAL_IMBLEARN._serialized_start=3160
+  _TRANSFORM_EXTERNAL_IMBLEARN._serialized_end=3184
+  _TRANSFORM_EXTERNAL_SHAP._serialized_start=3186
+  _TRANSFORM_EXTERNAL_SHAP._serialized_end=3206
+  _TRANSFORM_EXTERNAL_SCIPY._serialized_start=3208
+  _TRANSFORM_EXTERNAL_SCIPY._serialized_end=3229
+  _TRANSFORM_EXTERNAL_OPTBINNING._serialized_start=3231
+  _TRANSFORM_EXTERNAL_OPTBINNING._serialized_end=3257
+  _TRANSFORM_IDENTITY._serialized_start=3259
+  _TRANSFORM_IDENTITY._serialized_end=3269
+  _TRANSFORM_VARIABLE._serialized_start=3271
+  _TRANSFORM_VARIABLE._serialized_end=3313
+  _TRANSFORM_COMPOSED._serialized_start=3316
+  _TRANSFORM_COMPOSED._serialized_end=3485
+  _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._serialized_start=3432
+  _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._serialized_end=3485
+  _TRANSFORM_PROJECT._serialized_start=3487
+  _TRANSFORM_PROJECT._serialized_end=3539
+  _TRANSFORM_FILTER._serialized_start=3541
+  _TRANSFORM_FILTER._serialized_end=3588
+  _TRANSFORM_SHUFFLE._serialized_start=3590
+  _TRANSFORM_SHUFFLE._serialized_end=3599
+  _TRANSFORM_JOIN._serialized_start=3601
+  _TRANSFORM_JOIN._serialized_end=3642
+  _TRANSFORM_CAST._serialized_start=3644
+  _TRANSFORM_CAST._serialized_end=3687
+  _TRANSFORM_SAMPLE._serialized_start=3689
+  _TRANSFORM_SAMPLE._serialized_end=3786
+  _TRANSFORM_SCHEMAINFERENCE._serialized_start=3788
+  _TRANSFORM_SCHEMAINFERENCE._serialized_end=3906
+  _TRANSFORM_SCHEMAINFERENCE_CASTPOLICY._serialized_start=3867
+  _TRANSFORM_SCHEMAINFERENCE_CASTPOLICY._serialized_end=3906
+  _TRANSFORM_GROUPBY._serialized_start=3908
+  _TRANSFORM_GROUPBY._serialized_end=3930
+  _TRANSFORM_TOSMALLDATA._serialized_start=3932
+  _TRANSFORM_TOSMALLDATA._serialized_end=4023
+  _TRANSFORM_PUSHSQL._serialized_start=4025
+  _TRANSFORM_PUSHSQL._serialized_end=4117
+  _TRANSFORM_SYNTHETIC._serialized_start=4119
+  _TRANSFORM_SYNTHETIC._serialized_end=4130
+  _TRANSFORM_USERSETTINGS._serialized_start=4132
+  _TRANSFORM_USERSETTINGS._serialized_end=4146
+  _TRANSFORM_AUTOMATICUSERSETTINGS._serialized_start=4148
+  _TRANSFORM_AUTOMATICUSERSETTINGS._serialized_end=4195
+  _TRANSFORM_PRIVACYUNITTRACKING._serialized_start=4197
+  _TRANSFORM_PRIVACYUNITTRACKING._serialized_end=4218
+  _TRANSFORM_TRANSCODE._serialized_start=4220
+  _TRANSFORM_TRANSCODE._serialized_end=4231
+  _TRANSFORM_INVERSETRANSCODE._serialized_start=4233
+  _TRANSFORM_INVERSETRANSCODE._serialized_end=4251
+  _TRANSFORM_DIFFERENTIATEDSAMPLE._serialized_start=4253
+  _TRANSFORM_DIFFERENTIATEDSAMPLE._serialized_end=4364
+  _TRANSFORM_PRIVACYUNITTRACKINGPATHS._serialized_start=4366
+  _TRANSFORM_PRIVACYUNITTRACKINGPATHS._serialized_end=4392
+  _TRANSFORM_PUBLICPATHS._serialized_start=4394
+  _TRANSFORM_PUBLICPATHS._serialized_end=4407
+  _TRANSFORM_GETITEM._serialized_start=4409
+  _TRANSFORM_GETITEM._serialized_end=4455
+  _TRANSFORM_ASSIGNBUDGET._serialized_start=4457
+  _TRANSFORM_ASSIGNBUDGET._serialized_end=4471
+  _TRANSFORM_AUTOMATICBUDGET._serialized_start=4473
+  _TRANSFORM_AUTOMATICBUDGET._serialized_end=4490
+  _TRANSFORM_ATTRIBUTESBUDGET._serialized_start=4492
+  _TRANSFORM_ATTRIBUTESBUDGET._serialized_end=4510
+  _TRANSFORM_SDBUDGET._serialized_start=4512
+  _TRANSFORM_SDBUDGET._serialized_end=4522
+  _TRANSFORM_DERIVESEED._serialized_start=4524
+  _TRANSFORM_DERIVESEED._serialized_end=4560
+  _TRANSFORM_GROUPBYPE._serialized_start=4562
+  _TRANSFORM_GROUPBYPE._serialized_end=4573
+  _TRANSFORM_SAMPLINGRATIOS._serialized_start=4575
+  _TRANSFORM_SAMPLINGRATIOS._serialized_end=4591
+  _TRANSFORM_RELATIONSHIPSPEC._serialized_start=4593
+  _TRANSFORM_RELATIONSHIPSPEC._serialized_end=4611
+  _TRANSFORM_SELECTSQL._serialized_start=4614
+  _TRANSFORM_SELECTSQL._serialized_end=4750
+  _TRANSFORM_DPSELECTSQL._serialized_start=4753
+  _TRANSFORM_DPSELECTSQL._serialized_end=4891
+  _TRANSFORM_ALIASEDQUERIES._serialized_start=4893
+  _TRANSFORM_ALIASEDQUERIES._serialized_end=4957
+  _TRANSFORM_ALIASEDQUERY._serialized_start=4959
+  _TRANSFORM_ALIASEDQUERY._serialized_end=5025
+  _TRANSFORM_EXTRACT._serialized_start=5027
+  _TRANSFORM_EXTRACT._serialized_end=5050
+  _TRANSFORM_VALIDATEDUSERTYPE._serialized_start=5052
+  _TRANSFORM_VALIDATEDUSERTYPE._serialized_end=5071
+  _TRANSFORM_ERRORESTIMATION._serialized_start=5073
+  _TRANSFORM_ERRORESTIMATION._serialized_end=5090
+  _TRANSFORM_FITMODEL._serialized_start=5092
+  _TRANSFORM_FITMODEL._serialized_end=5178
+  _TRANSFORM_TEXTKIND._serialized_start=5180
+  _TRANSFORM_TEXTKIND._serialized_end=5258
+  _TRANSFORM_CHAT._serialized_start=5260
+  _TRANSFORM_CHAT._serialized_end=5312
+  _TRANSFORM_FITMODELDP._serialized_start=5314
+  _TRANSFORM_FITMODELDP._serialized_end=5424
+  _TRANSFORM_GENERATEFROMMODEL._serialized_start=5426
+  _TRANSFORM_GENERATEFROMMODEL._serialized_end=5490
+  _TRANSFORM_SQLDIALECT._serialized_start=5493
+  _TRANSFORM_SQLDIALECT._serialized_end=5621
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/transform_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/transform_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
         DP_SELECT_SQL_FIELD_NUMBER: builtins.int
         ERROR_ESTIMATION_FIELD_NUMBER: builtins.int
         FIT_MODEL_FIELD_NUMBER: builtins.int
         FIT_MODEL_DP_FIELD_NUMBER: builtins.int
         GENERATE_FROM_MODEL_FIELD_NUMBER: builtins.int
         TO_SMALL_DATA_FIELD_NUMBER: builtins.int
         PUSH_SQL_FIELD_NUMBER: builtins.int
-        SELECT_TABLE_FIELD_NUMBER: builtins.int
         @property
         def identity(self) -> global___Transform.Identity: ...
         @property
         def variable(self) -> global___Transform.Variable: ...
         @property
         def composed(self) -> global___Transform.Composed: ...
         @property
@@ -175,16 +174,14 @@
         def fit_model_dp(self) -> global___Transform.FitModelDP: ...
         @property
         def generate_from_model(self) -> global___Transform.GenerateFromModel: ...
         @property
         def to_small_data(self) -> global___Transform.ToSmallData: ...
         @property
         def push_sql(self) -> global___Transform.PushSQL: ...
-        @property
-        def select_table(self) -> global___Transform.SelectTable: ...
         def __init__(self,
             *,
             identity : typing.Optional[global___Transform.Identity] = ...,
             variable : typing.Optional[global___Transform.Variable] = ...,
             composed : typing.Optional[global___Transform.Composed] = ...,
             project : typing.Optional[global___Transform.Project] = ...,
             filter : typing.Optional[global___Transform.Filter] = ...,
@@ -217,19 +214,18 @@
             dp_select_sql : typing.Optional[global___Transform.DPSelectSql] = ...,
             error_estimation : typing.Optional[global___Transform.ErrorEstimation] = ...,
             fit_model : typing.Optional[global___Transform.FitModel] = ...,
             fit_model_dp : typing.Optional[global___Transform.FitModelDP] = ...,
             generate_from_model : typing.Optional[global___Transform.GenerateFromModel] = ...,
             to_small_data : typing.Optional[global___Transform.ToSmallData] = ...,
             push_sql : typing.Optional[global___Transform.PushSQL] = ...,
-            select_table : typing.Optional[global___Transform.SelectTable] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["assign_budget",b"assign_budget","attribute_budget",b"attribute_budget","automatic_budget",b"automatic_budget","automatic_user_settings",b"automatic_user_settings","cast",b"cast","composed",b"composed","derive_seed",b"derive_seed","differentiated_sample",b"differentiated_sample","dp_select_sql",b"dp_select_sql","error_estimation",b"error_estimation","external",b"external","extract",b"extract","filter",b"filter","fit_model",b"fit_model","fit_model_dp",b"fit_model_dp","generate_from_model",b"generate_from_model","get_item",b"get_item","group_by_pe",b"group_by_pe","identity",b"identity","inverse_transcode",b"inverse_transcode","join",b"join","privacy_unit_tracking",b"privacy_unit_tracking","privacy_unit_tracking_paths",b"privacy_unit_tracking_paths","project",b"project","public_paths",b"public_paths","push_sql",b"push_sql","relationship_spec",b"relationship_spec","sample",b"sample","sampling_ratios",b"sampling_ratios","sd_budget",b"sd_budget","select_sql",b"select_sql","select_table",b"select_table","shuffle",b"shuffle","spec",b"spec","synthetic",b"synthetic","to_small_data",b"to_small_data","transcode",b"transcode","user_settings",b"user_settings","validated_user_type",b"validated_user_type","variable",b"variable"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["assign_budget",b"assign_budget","attribute_budget",b"attribute_budget","automatic_budget",b"automatic_budget","automatic_user_settings",b"automatic_user_settings","cast",b"cast","composed",b"composed","derive_seed",b"derive_seed","differentiated_sample",b"differentiated_sample","dp_select_sql",b"dp_select_sql","error_estimation",b"error_estimation","external",b"external","extract",b"extract","filter",b"filter","fit_model",b"fit_model","fit_model_dp",b"fit_model_dp","generate_from_model",b"generate_from_model","get_item",b"get_item","group_by_pe",b"group_by_pe","identity",b"identity","inverse_transcode",b"inverse_transcode","join",b"join","privacy_unit_tracking",b"privacy_unit_tracking","privacy_unit_tracking_paths",b"privacy_unit_tracking_paths","project",b"project","public_paths",b"public_paths","push_sql",b"push_sql","relationship_spec",b"relationship_spec","sample",b"sample","sampling_ratios",b"sampling_ratios","sd_budget",b"sd_budget","select_sql",b"select_sql","select_table",b"select_table","shuffle",b"shuffle","spec",b"spec","synthetic",b"synthetic","to_small_data",b"to_small_data","transcode",b"transcode","user_settings",b"user_settings","validated_user_type",b"validated_user_type","variable",b"variable"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal["spec",b"spec"]) -> typing.Optional[typing_extensions.Literal["identity","variable","composed","project","filter","shuffle","join","cast","sample","user_settings","privacy_unit_tracking","external","synthetic","transcode","inverse_transcode","get_item","privacy_unit_tracking_paths","automatic_user_settings","public_paths","assign_budget","automatic_budget","attribute_budget","sd_budget","derive_seed","group_by_pe","sampling_ratios","select_sql","extract","relationship_spec","differentiated_sample","validated_user_type","dp_select_sql","error_estimation","fit_model","fit_model_dp","generate_from_model","to_small_data","push_sql","select_table"]]: ...
+        def HasField(self, field_name: typing_extensions.Literal["assign_budget",b"assign_budget","attribute_budget",b"attribute_budget","automatic_budget",b"automatic_budget","automatic_user_settings",b"automatic_user_settings","cast",b"cast","composed",b"composed","derive_seed",b"derive_seed","differentiated_sample",b"differentiated_sample","dp_select_sql",b"dp_select_sql","error_estimation",b"error_estimation","external",b"external","extract",b"extract","filter",b"filter","fit_model",b"fit_model","fit_model_dp",b"fit_model_dp","generate_from_model",b"generate_from_model","get_item",b"get_item","group_by_pe",b"group_by_pe","identity",b"identity","inverse_transcode",b"inverse_transcode","join",b"join","privacy_unit_tracking",b"privacy_unit_tracking","privacy_unit_tracking_paths",b"privacy_unit_tracking_paths","project",b"project","public_paths",b"public_paths","push_sql",b"push_sql","relationship_spec",b"relationship_spec","sample",b"sample","sampling_ratios",b"sampling_ratios","sd_budget",b"sd_budget","select_sql",b"select_sql","shuffle",b"shuffle","spec",b"spec","synthetic",b"synthetic","to_small_data",b"to_small_data","transcode",b"transcode","user_settings",b"user_settings","validated_user_type",b"validated_user_type","variable",b"variable"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["assign_budget",b"assign_budget","attribute_budget",b"attribute_budget","automatic_budget",b"automatic_budget","automatic_user_settings",b"automatic_user_settings","cast",b"cast","composed",b"composed","derive_seed",b"derive_seed","differentiated_sample",b"differentiated_sample","dp_select_sql",b"dp_select_sql","error_estimation",b"error_estimation","external",b"external","extract",b"extract","filter",b"filter","fit_model",b"fit_model","fit_model_dp",b"fit_model_dp","generate_from_model",b"generate_from_model","get_item",b"get_item","group_by_pe",b"group_by_pe","identity",b"identity","inverse_transcode",b"inverse_transcode","join",b"join","privacy_unit_tracking",b"privacy_unit_tracking","privacy_unit_tracking_paths",b"privacy_unit_tracking_paths","project",b"project","public_paths",b"public_paths","push_sql",b"push_sql","relationship_spec",b"relationship_spec","sample",b"sample","sampling_ratios",b"sampling_ratios","sd_budget",b"sd_budget","select_sql",b"select_sql","shuffle",b"shuffle","spec",b"spec","synthetic",b"synthetic","to_small_data",b"to_small_data","transcode",b"transcode","user_settings",b"user_settings","validated_user_type",b"validated_user_type","variable",b"variable"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["spec",b"spec"]) -> typing.Optional[typing_extensions.Literal["identity","variable","composed","project","filter","shuffle","join","cast","sample","user_settings","privacy_unit_tracking","external","synthetic","transcode","inverse_transcode","get_item","privacy_unit_tracking_paths","automatic_user_settings","public_paths","assign_budget","automatic_budget","attribute_budget","sd_budget","derive_seed","group_by_pe","sampling_ratios","select_sql","extract","relationship_spec","differentiated_sample","validated_user_type","dp_select_sql","error_estimation","fit_model","fit_model_dp","generate_from_model","to_small_data","push_sql"]]: ...
 
     class External(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class OpIdentifier(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             STD_FIELD_NUMBER: builtins.int
             PANDAS_FIELD_NUMBER: builtins.int
@@ -907,26 +903,14 @@
         def __init__(self,
             *,
             max_new_tokens : builtins.int = ...,
             temperature : builtins.float = ...,
             ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal["max_new_tokens",b"max_new_tokens","temperature",b"temperature"]) -> None: ...
 
-    class SelectTable(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-        PATH_FIELD_NUMBER: builtins.int
-        @property
-        def path(self) -> sarus_data_spec.protobuf.path_pb2.Path: ...
-        def __init__(self,
-            *,
-            path : typing.Optional[sarus_data_spec.protobuf.path_pb2.Path] = ...,
-            ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["path",b"path"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["path",b"path"]) -> None: ...
-
     UUID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     DOC_FIELD_NUMBER: builtins.int
     SPEC_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     INVERSIBLE_FIELD_NUMBER: builtins.int
     SCHEMA_PRESERVING_FIELD_NUMBER: builtins.int
```

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/type.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/type_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/type_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/type_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/typing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/protobuf/utilities.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/utilities.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/scalar.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/scalar.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/schema.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/size.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/size.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/statistics.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/statistics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/status.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/status.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/storage/local.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/storage/local.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/storage/typing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/storage/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/storage/utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/storage/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/transform.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,40 +579,14 @@
             ),
             inversible=False,
             schema_preserving=False,
         )
     )
 
 
-def get_item(path: st.Path) -> st.Transform:
-    return Transform(
-        sp.Transform(
-            name="get_item",
-            spec=sp.Transform.Spec(
-                get_item=sp.Transform.GetItem(path=path.protobuf())
-            ),
-            inversible=False,
-            schema_preserving=False,
-        )
-    )
-
-
-def select_table(path: st.Path) -> Transform:
-    return Transform(
-        sp.Transform(
-            name="select_table",
-            spec=sp.Transform.Spec(
-                select_table=sp.Transform.SelectTable(path=path.protobuf())
-            ),
-            inversible=False,
-            schema_preserving=False,
-        )
-    )
-
-
 def shuffle() -> Transform:
     return Transform(
         sp.Transform(
             name="Shuffle",
             spec=sp.Transform.Spec(shuffle=sp.Transform.Shuffle()),
             inversible=False,
             schema_preserving=True,
@@ -787,14 +761,27 @@
             name="automatic_public_paths",
             spec=sp.Transform.Spec(public_paths=sp.Transform.PublicPaths()),
             properties={"creation_time": str(datetime.datetime.now())},
         )
     )
 
 
+def get_item(path: st.Path) -> st.Transform:
+    return Transform(
+        sp.Transform(
+            name="get_item",
+            spec=sp.Transform.Spec(
+                get_item=sp.Transform.GetItem(path=path.protobuf())
+            ),
+            inversible=False,
+            schema_preserving=False,
+        )
+    )
+
+
 def assign_budget() -> st.Transform:
     """Transform to assign a given privacy budget to a dataset.
     It is used to specify the budget to compute the attributes
     size, bounds, marginals"""
 
     return Transform(
         sp.Transform(
```

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/type.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/typing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec/variant_constraint.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/variant_constraint.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec_public.egg-info/PKG-INFO` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus_data_spec_public
-Version: 4.0.2
+Version: 4.0.2.dev0
 Summary: A library to manage Sarus datasets
 Home-page: 
 Download-URL: 
 Author: Sarus Technologies
 Author-email: 
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sarus_data_spec_public-4.0.2/sarus_data_spec_public.egg-info/SOURCES.txt` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,14 @@
 sarus_data_spec/manager/ops/processor/standard/extract.py
 sarus_data_spec/manager/ops/processor/standard/filter.py
 sarus_data_spec/manager/ops/processor/standard/generate_from_model.py
 sarus_data_spec/manager/ops/processor/standard/get_item.py
 sarus_data_spec/manager/ops/processor/standard/project.py
 sarus_data_spec/manager/ops/processor/standard/push_sql.py
 sarus_data_spec/manager/ops/processor/standard/sample.py
-sarus_data_spec/manager/ops/processor/standard/select_table.py
 sarus_data_spec/manager/ops/processor/standard/shuffle.py
 sarus_data_spec/manager/ops/processor/standard/standard_op.py
 sarus_data_spec/manager/ops/processor/standard/synthetic.py
 sarus_data_spec/manager/ops/processor/standard/to_small_data.py
 sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
 sarus_data_spec/manager/ops/processor/standard/sampling/__init__.py
 sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py
```

### Comparing `sarus_data_spec_public-4.0.2/setup.cfg` & `sarus_data_spec_public-4.0.2.dev0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 	sarus_data_spec.manager.ops.sql_utils.bigdata
 	sarus_data_spec.manager.ops.sql_utils.queries
 	sarus_data_spec.manager.ops.processor.routing
 	sarus_data_spec.manager.ops.processor.standard.standard_op
 	sarus_data_spec.manager.ops.processor.standard.visitor_selector
 	sarus_data_spec.manager.ops.processor.standard.filter
 	sarus_data_spec.manager.ops.processor.standard.get_item
-	sarus_data_spec.manager.ops.processor.standard.select_table
 	sarus_data_spec.manager.ops.processor.standard.project
 	sarus_data_spec.manager.ops.processor.standard.sample
 	sarus_data_spec.manager.ops.processor.standard.sampling.differentiated_sampling_sizes
 	sarus_data_spec.manager.ops.processor.standard.differentiated_sample
 	sarus_data_spec.manager.ops.processor.standard.extract
 	sarus_data_spec.manager.ops.processor.standard.shuffle
 	sarus_data_spec.manager.ops.processor.standard.synthetic
```

### Comparing `sarus_data_spec_public-4.0.2/setup.py` & `sarus_data_spec_public-4.0.2.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
     def run(self):
         generate_proto_code()
         build_py.run(self)
 
 
 if __name__ == "__main__":
-    setup(version="4.0.2")
+    setup(version="4.0.2.dev0")
```

