# Comparing `tmp/treelite-4.1.2.tar.gz` & `tmp/treelite-4.2.0.tar.gz`

## Comparing `treelite-4.1.2.tar` & `treelite-4.2.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/CMakeLists.txt
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/LICENSE
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/cmake/Doxygen.cmake
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/cmake/ExternalLibs.cmake
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/cmake/Sanitizer.cmake
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/cmake/TreeliteConfig.cmake.in
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/cmake/Utils.cmake
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/cmake/Version.cmake
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/cmake/version.h.in
--rw-r--r--   0        0        0    42322 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/c_api.h
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/c_api_error.h
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/contiguous_array.h
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/error.h
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/gtil.h
--rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/logging.h
--rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/model_builder.h
--rw-r--r--   0        0        0    20925 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/model_loader.h
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/pybuffer_frame.h
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/thread_local.h
--rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/tree.h
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/detail/contiguous_array.h
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/detail/file_utils.h
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/detail/omp_exception.h
--rw-r--r--   0        0        0     7948 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/detail/serializer.h
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/detail/serializer_mixins.h
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/detail/threading_utils.h
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/detail/tree.h
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/enum/operator.h
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/enum/task_type.h
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/enum/tree_node_type.h
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/include/treelite/enum/typeinfo.h
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/CMakeLists.txt
--rw-r--r--   0        0        0    11389 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/field_accessor.cc
--rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/json_serializer.cc
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/logging.cc
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/model_concat.cc
--rw-r--r--   0        0        0    19505 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/serializer.cc
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/c_api/c_api_error.cc
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/c_api/c_api_utils.h
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/c_api/field_accessor.cc
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/c_api/gtil.cc
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/c_api/logging.cc
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/c_api/model.cc
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/c_api/model_builder.cc
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/c_api/model_loader.cc
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/c_api/serializer.cc
--rw-r--r--   0        0        0     5959 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/c_api/sklearn.cc
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/enum/operator.cc
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/enum/task_type.cc
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/enum/tree_node_type.cc
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/enum/typeinfo.cc
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/gtil/config.cc
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/gtil/output_shape.cc
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/gtil/postprocessor.cc
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/gtil/postprocessor.h
--rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/gtil/predict.cc
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/model_builder/metadata.cc
--rw-r--r--   0        0        0    18423 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/model_builder/model_builder.cc
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/model_builder/detail/json_parsing.h
--rw-r--r--   0        0        0    22109 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/model_loader/lightgbm.cc
--rw-r--r--   0        0        0    26078 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/model_loader/sklearn.cc
--rw-r--r--   0        0        0    31149 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/model_loader/xgboost_json.cc
--rw-r--r--   0        0        0    17766 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/model_loader/xgboost_legacy.cc
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/model_loader/detail/lightgbm.h
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/model_loader/detail/string_utils.h
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/model_loader/detail/xgboost.cc
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/model_loader/detail/xgboost.h
--rw-r--r--   0        0        0    19413 2020-02-02 00:00:00.000000 treelite-4.1.2/cpp_src/src/model_loader/detail/xgboost_json.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treelite-4.1.2/packager/__init__.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 treelite-4.1.2/packager/build_config.py
--rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 treelite-4.1.2/packager/nativelib.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 treelite-4.1.2/packager/pep517.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 treelite-4.1.2/packager/sdist.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 treelite-4.1.2/packager/util.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/VERSION
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/__init__.py
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/compat.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/core.py
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/frontend.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/libpath.py
--rw-r--r--   0        0        0    19254 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/model.py
--rw-r--r--   0        0        0    12385 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/model_builder.py
--rw-r--r--   0        0        0    18542 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/model_builder_legacy.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/path_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/py.typed
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/util.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/gtil/__init__.py
--rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/gtil/gtil.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/sklearn/__init__.py
--rw-r--r--   0        0        0    19243 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/sklearn/importer.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 treelite-4.1.2/treelite/sklearn/isolation_forest.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 treelite-4.1.2/README.rst
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 treelite-4.1.2/hatch_build.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 treelite-4.1.2/pyproject.toml
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 treelite-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/CMakeLists.txt
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/LICENSE
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/cmake/Doxygen.cmake
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/cmake/ExternalLibs.cmake
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/cmake/Sanitizer.cmake
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/cmake/TreeliteConfig.cmake.in
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/cmake/Utils.cmake
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/cmake/Version.cmake
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/cmake/version.h.in
+-rw-r--r--   0        0        0    42322 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/c_api.h
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/c_api_error.h
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/contiguous_array.h
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/error.h
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/gtil.h
+-rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/logging.h
+-rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/model_builder.h
+-rw-r--r--   0        0        0    20925 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/model_loader.h
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/pybuffer_frame.h
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/thread_local.h
+-rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/tree.h
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/detail/contiguous_array.h
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/detail/file_utils.h
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/detail/omp_exception.h
+-rw-r--r--   0        0        0     7948 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/detail/serializer.h
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/detail/serializer_mixins.h
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/detail/threading_utils.h
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/detail/tree.h
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/enum/operator.h
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/enum/task_type.h
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/enum/tree_node_type.h
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/enum/typeinfo.h
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/CMakeLists.txt
+-rw-r--r--   0        0        0    11389 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/field_accessor.cc
+-rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/json_serializer.cc
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/logging.cc
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_concat.cc
+-rw-r--r--   0        0        0    19505 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/serializer.cc
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/c_api_error.cc
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/c_api_utils.h
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/field_accessor.cc
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/gtil.cc
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/logging.cc
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/model.cc
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/model_builder.cc
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/model_loader.cc
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/serializer.cc
+-rw-r--r--   0        0        0     5959 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/sklearn.cc
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/enum/operator.cc
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/enum/task_type.cc
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/enum/tree_node_type.cc
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/enum/typeinfo.cc
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/gtil/config.cc
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/gtil/output_shape.cc
+-rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/gtil/postprocessor.cc
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/gtil/postprocessor.h
+-rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/gtil/predict.cc
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_builder/metadata.cc
+-rw-r--r--   0        0        0    18784 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_builder/model_builder.cc
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_builder/detail/json_parsing.h
+-rw-r--r--   0        0        0    22109 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/lightgbm.cc
+-rw-r--r--   0        0        0    26078 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/sklearn.cc
+-rw-r--r--   0        0        0    31217 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/xgboost_json.cc
+-rw-r--r--   0        0        0    17766 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/xgboost_legacy.cc
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/detail/lightgbm.h
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/detail/string_utils.h
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/detail/xgboost.cc
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/detail/xgboost.h
+-rw-r--r--   0        0        0    19413 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/detail/xgboost_json.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treelite-4.2.0/packager/__init__.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 treelite-4.2.0/packager/build_config.py
+-rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 treelite-4.2.0/packager/nativelib.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 treelite-4.2.0/packager/pep517.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 treelite-4.2.0/packager/sdist.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 treelite-4.2.0/packager/util.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/VERSION
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/__init__.py
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/compat.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/core.py
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/frontend.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/libpath.py
+-rw-r--r--   0        0        0    19254 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/model.py
+-rw-r--r--   0        0        0    12385 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/model_builder.py
+-rw-r--r--   0        0        0    18542 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/model_builder_legacy.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/path_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/py.typed
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/util.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/gtil/__init__.py
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/gtil/gtil.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/sklearn/__init__.py
+-rw-r--r--   0        0        0    19233 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/sklearn/importer.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/sklearn/isolation_forest.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 treelite-4.2.0/README.rst
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 treelite-4.2.0/hatch_build.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 treelite-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 treelite-4.2.0/PKG-INFO
```

### Comparing `treelite-4.1.2/cpp_src/CMakeLists.txt` & `treelite-4.2.0/cpp_src/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cmake_policy(SET CMP0025 NEW)
 cmake_policy(SET CMP0091 NEW)
 set(CMAKE_FIND_NO_INSTALL_PREFIX TRUE FORCE)
 cmake_minimum_required(VERSION 3.16 FATAL_ERROR)
 
-project(treelite LANGUAGES CXX C VERSION 4.1.2)
+project(treelite LANGUAGES CXX C VERSION 4.2.0)
 
 # Check compiler versions
 # Use latest compilers to ensure that std::filesystem is available
 if(MSVC)
   if(MSVC_VERSION LESS 1930)
     message(FATAL_ERROR "Need Visual Studio 2022 or newer to build Treelite")
   endif()
```

### Comparing `treelite-4.1.2/cpp_src/LICENSE` & `treelite-4.2.0/cpp_src/LICENSE`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/cmake/ExternalLibs.cmake` & `treelite-4.2.0/cpp_src/cmake/ExternalLibs.cmake`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/cmake/Sanitizer.cmake` & `treelite-4.2.0/cpp_src/cmake/Sanitizer.cmake`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/cmake/Utils.cmake` & `treelite-4.2.0/cpp_src/cmake/Utils.cmake`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/c_api.h` & `treelite-4.2.0/cpp_src/include/treelite/c_api.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/c_api_error.h` & `treelite-4.2.0/cpp_src/include/treelite/c_api_error.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/contiguous_array.h` & `treelite-4.2.0/cpp_src/include/treelite/contiguous_array.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/gtil.h` & `treelite-4.2.0/cpp_src/include/treelite/gtil.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/logging.h` & `treelite-4.2.0/cpp_src/include/treelite/logging.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/model_builder.h` & `treelite-4.2.0/cpp_src/include/treelite/model_builder.h`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,21 @@
  * \brief Model builder interface.
  * \note A model builder object must be accessed by a single thread. For parallel tree construction,
  *       build multiple model objects and then concatenate them.
  */
 class ModelBuilder {
  public:
   /*!
+   * \brief Set a flag to control validation behavior.
+   * Currently, we support "check_orphaned_nodes" (defaults to true).
+   * \param flag Name of the flag
+   * \param value Value to set the flag
+   */
+  virtual void SetValidationFlag(std::string const& flag, bool value) = 0;
+  /*!
    * \brief Start a new tree
    */
   virtual void StartTree() = 0;
   /*!
    * \brief End the current tree
    */
   virtual void EndTree() = 0;
```

### Comparing `treelite-4.1.2/cpp_src/include/treelite/model_loader.h` & `treelite-4.2.0/cpp_src/include/treelite/model_loader.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/pybuffer_frame.h` & `treelite-4.2.0/cpp_src/include/treelite/pybuffer_frame.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/thread_local.h` & `treelite-4.2.0/cpp_src/include/treelite/thread_local.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/tree.h` & `treelite-4.2.0/cpp_src/include/treelite/tree.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/detail/contiguous_array.h` & `treelite-4.2.0/cpp_src/include/treelite/detail/contiguous_array.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/detail/file_utils.h` & `treelite-4.2.0/cpp_src/include/treelite/detail/file_utils.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/detail/omp_exception.h` & `treelite-4.2.0/cpp_src/include/treelite/detail/omp_exception.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/detail/serializer.h` & `treelite-4.2.0/cpp_src/include/treelite/detail/serializer.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/detail/serializer_mixins.h` & `treelite-4.2.0/cpp_src/include/treelite/detail/serializer_mixins.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/detail/threading_utils.h` & `treelite-4.2.0/cpp_src/include/treelite/detail/threading_utils.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/detail/tree.h` & `treelite-4.2.0/cpp_src/include/treelite/detail/tree.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/enum/operator.h` & `treelite-4.2.0/cpp_src/include/treelite/enum/operator.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/enum/task_type.h` & `treelite-4.2.0/cpp_src/include/treelite/enum/task_type.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/enum/tree_node_type.h` & `treelite-4.2.0/cpp_src/include/treelite/enum/tree_node_type.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/include/treelite/enum/typeinfo.h` & `treelite-4.2.0/cpp_src/include/treelite/enum/typeinfo.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/CMakeLists.txt` & `treelite-4.2.0/cpp_src/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/field_accessor.cc` & `treelite-4.2.0/cpp_src/src/field_accessor.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/json_serializer.cc` & `treelite-4.2.0/cpp_src/src/json_serializer.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/logging.cc` & `treelite-4.2.0/cpp_src/src/logging.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/model_concat.cc` & `treelite-4.2.0/cpp_src/src/model_concat.cc`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
               << "has a different num_class than the first model object (at index 0)";
           TREELITE_CHECK(concatenated_model->leaf_vector_shape == objs[i]->leaf_vector_shape)
               << "Model object at index " << i
               << "has a different leaf_vector_shape than the first model object (at index 0)";
           auto& casted = std::get<ModelType>(objs[i]->variant_);
           std::transform(casted.trees.begin(), casted.trees.end(),
               std::back_inserter(concatenated_model_concrete.trees),
-              [](const auto& tree) { return tree.Clone(); });
+              [](auto const& tree) { return tree.Clone(); });
           concatenated_model->target_id.Extend(objs[i]->target_id);
           concatenated_model->class_id.Extend(objs[i]->class_id);
         }
       },
       objs[0]->variant_);
   TREELITE_CHECK_EQ(concatenated_model->target_id.Size(), concatenated_model->GetNumTree());
   TREELITE_CHECK_EQ(concatenated_model->class_id.Size(), concatenated_model->GetNumTree());
```

### Comparing `treelite-4.1.2/cpp_src/src/serializer.cc` & `treelite-4.2.0/cpp_src/src/serializer.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/c_api/c_api_error.cc` & `treelite-4.2.0/cpp_src/src/c_api/c_api_error.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/c_api/c_api_utils.h` & `treelite-4.2.0/cpp_src/src/c_api/c_api_utils.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/c_api/field_accessor.cc` & `treelite-4.2.0/cpp_src/src/c_api/field_accessor.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/c_api/gtil.cc` & `treelite-4.2.0/cpp_src/src/c_api/gtil.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/c_api/logging.cc` & `treelite-4.2.0/cpp_src/src/c_api/logging.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/c_api/model.cc` & `treelite-4.2.0/cpp_src/src/c_api/model.cc`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 }
 
 int TreeliteConcatenateModelObjects(
     TreeliteModelHandle const* objs, std::size_t len, TreeliteModelHandle* out) {
   API_BEGIN();
   std::vector<treelite::Model const*> model_objs(len, nullptr);
   std::transform(objs, objs + len, model_objs.begin(),
-      [](TreeliteModelHandle e) { return static_cast<const treelite::Model*>(e); });
+      [](TreeliteModelHandle e) { return static_cast<treelite::Model const*>(e); });
   auto concatenated_model = ConcatenateModelObjects(model_objs);
   *out = static_cast<TreeliteModelHandle>(concatenated_model.release());
   API_END();
 }
 
 int TreeliteFreeModel(TreeliteModelHandle handle) {
   API_BEGIN();
```

### Comparing `treelite-4.1.2/cpp_src/src/c_api/model_builder.cc` & `treelite-4.2.0/cpp_src/src/c_api/model_builder.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/c_api/model_loader.cc` & `treelite-4.2.0/cpp_src/src/c_api/model_loader.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/c_api/serializer.cc` & `treelite-4.2.0/cpp_src/src/c_api/serializer.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/c_api/sklearn.cc` & `treelite-4.2.0/cpp_src/src/c_api/sklearn.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/enum/operator.cc` & `treelite-4.2.0/cpp_src/src/enum/operator.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/enum/task_type.cc` & `treelite-4.2.0/cpp_src/src/enum/task_type.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/enum/tree_node_type.cc` & `treelite-4.2.0/cpp_src/src/enum/tree_node_type.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/enum/typeinfo.cc` & `treelite-4.2.0/cpp_src/src/enum/typeinfo.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/gtil/config.cc` & `treelite-4.2.0/cpp_src/src/gtil/config.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/gtil/output_shape.cc` & `treelite-4.2.0/cpp_src/src/gtil/output_shape.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/gtil/postprocessor.cc` & `treelite-4.2.0/cpp_src/src/gtil/postprocessor.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/gtil/postprocessor.h` & `treelite-4.2.0/cpp_src/src/gtil/postprocessor.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/gtil/predict.cc` & `treelite-4.2.0/cpp_src/src/gtil/predict.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/model_builder/metadata.cc` & `treelite-4.2.0/cpp_src/src/model_builder/metadata.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/model_builder/model_builder.cc` & `treelite-4.2.0/cpp_src/src/model_builder/model_builder.cc`

 * *Files 2% similar despite different names*

```diff
@@ -62,31 +62,39 @@
         expected_leaf_size_{},
         model_{Model::Create<ThresholdT, LeafOutputT>()},
         current_tree_{},
         node_id_map_{},
         current_node_key_{},
         current_node_id_{},
         current_state_{ModelBuilderState::kExpectTree},
-        metadata_initialized_{false} {}
+        metadata_initialized_{false},
+        flag_check_orphaned_nodes_{true} {}
 
   ModelBuilderImpl(Metadata const& metadata, TreeAnnotation const& tree_annotation,
       PostProcessorFunc const& postprocessor, std::vector<double> const& base_scores,
       std::optional<std::string> const& attributes)
       : expected_num_tree_{},
         expected_leaf_size_{},
         model_{Model::Create<ThresholdT, LeafOutputT>()},
         current_tree_{},
         node_id_map_{},
         current_node_key_{},
         current_node_id_{},
         current_state_{ModelBuilderState::kExpectTree},
-        metadata_initialized_{false} {
+        metadata_initialized_{false},
+        flag_check_orphaned_nodes_{true} {
     InitializeMetadataImpl(metadata, tree_annotation, postprocessor, base_scores, attributes);
   }
 
+  void SetValidationFlag(std::string const& flag, bool value) override {
+    if (flag == "check_orphaned_nodes") {
+      flag_check_orphaned_nodes_ = value;
+    }
+  }
+
   void StartTree() override {
     CheckStateWithDiagnostic("StartTree()", {ModelBuilderState::kExpectTree}, current_state_);
 
     current_tree_ = Tree<ThresholdT, LeafOutputT>();
     current_tree_.Init();
 
     current_state_ = ModelBuilderState::kExpectNode;
@@ -117,25 +125,27 @@
           TREELITE_LOG(FATAL) << "Node with key " << right_key << " not found";
         }
         current_tree_.SetChildren(i, cleft, cright);
         orphaned[cleft] = false;
         orphaned[cright] = false;
       }
     }
-    auto itr = std::find(orphaned.begin(), orphaned.end(), true);
-    if (itr != orphaned.end()) {
-      auto orphaned_node_id = *itr;
-      for (auto [k, v] : node_id_map_) {
-        if (v == orphaned_node_id) {
-          TREELITE_LOG(FATAL) << "Node with key " << k << " is orphaned -- it cannot be reached "
-                              << "from the root node";
+    if (flag_check_orphaned_nodes_) {
+      auto itr = std::find(orphaned.begin(), orphaned.end(), true);
+      if (itr != orphaned.end()) {
+        auto orphaned_node_id = *itr;
+        for (auto [k, v] : node_id_map_) {
+          if (v == orphaned_node_id) {
+            TREELITE_LOG(FATAL) << "Node with key " << k << " is orphaned -- it cannot be reached "
+                                << "from the root node";
+          }
         }
+        TREELITE_LOG(FATAL) << "Node at index " << orphaned_node_id << " is orphaned "
+                            << "-- it cannot be reached from the root node";
       }
-      TREELITE_LOG(FATAL) << "Node at index " << orphaned_node_id << " is orphaned "
-                          << "-- it cannot be reached from the root node";
     }
 
     auto& trees = std::get<ModelPreset<ThresholdT, LeafOutputT>>(model_->variant_).trees;
     trees.push_back(std::move(current_tree_));
 
     node_id_map_.clear();
     current_state_ = ModelBuilderState::kExpectTree;
@@ -288,14 +298,15 @@
   std::unique_ptr<Model> model_;
   Tree<ThresholdT, LeafOutputT> current_tree_;
   std::map<int, int> node_id_map_;  // user-defined ID -> internal ID
   int current_node_key_;  // current node ID (user-defined)
   int current_node_id_;  // current node ID (internal)
   ModelBuilderState current_state_;
   bool metadata_initialized_{false};
+  bool flag_check_orphaned_nodes_{true};
 
   void CheckStateWithDiagnostic(std::string const& func_name,
       std::vector<ModelBuilderState> const& valid_states, ModelBuilderState actual_state) {
     auto error = [&](std::string const& msg) {
       TREELITE_LOG(FATAL) << "Unexpected call to " << func_name << ". " << msg;
     };
     if (std::find(valid_states.begin(), valid_states.end(), actual_state) == valid_states.end()) {
```

### Comparing `treelite-4.1.2/cpp_src/src/model_builder/detail/json_parsing.h` & `treelite-4.2.0/cpp_src/src/model_builder/detail/json_parsing.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/model_loader/lightgbm.cc` & `treelite-4.2.0/cpp_src/src/model_loader/lightgbm.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/model_loader/sklearn.cc` & `treelite-4.2.0/cpp_src/src/model_loader/sklearn.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/model_loader/xgboost_json.cc` & `treelite-4.2.0/cpp_src/src/model_loader/xgboost_json.cc`

 * *Files 1% similar despite different names*

```diff
@@ -373,14 +373,15 @@
 /******************************************************************************
  * GBTreeHandler
  * ***************************************************************************/
 bool GBTreeModelHandler::StartArray() {
   if (this->should_ignore_upcoming_value()) {
     return push_handler<IgnoreHandler>();
   }
+  output.builder->SetValidationFlag("check_orphaned_nodes", false);
   return (push_key_handler<RegTreeArrayHandler, std::vector<ParsedRegTreeParams>>(
               "trees", reg_tree_params, *output.builder)
           || push_key_handler<ArrayHandler<int>, std::vector<int>>("tree_info", output.tree_info)
           || push_key_handler<IgnoreHandler>("iteration_indptr"));
 }
 
 bool GBTreeModelHandler::StartObject() {
```

### Comparing `treelite-4.1.2/cpp_src/src/model_loader/xgboost_legacy.cc` & `treelite-4.2.0/cpp_src/src/model_loader/xgboost_legacy.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/model_loader/detail/lightgbm.h` & `treelite-4.2.0/cpp_src/src/model_loader/detail/lightgbm.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/model_loader/detail/string_utils.h` & `treelite-4.2.0/cpp_src/src/model_loader/detail/string_utils.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/model_loader/detail/xgboost.cc` & `treelite-4.2.0/cpp_src/src/model_loader/detail/xgboost.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/model_loader/detail/xgboost.h` & `treelite-4.2.0/cpp_src/src/model_loader/detail/xgboost.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/cpp_src/src/model_loader/detail/xgboost_json.h` & `treelite-4.2.0/cpp_src/src/model_loader/detail/xgboost_json.h`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/packager/build_config.py` & `treelite-4.2.0/packager/build_config.py`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/packager/nativelib.py` & `treelite-4.2.0/packager/nativelib.py`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/packager/pep517.py` & `treelite-4.2.0/packager/pep517.py`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/packager/sdist.py` & `treelite-4.2.0/packager/sdist.py`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/packager/util.py` & `treelite-4.2.0/packager/util.py`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/treelite/compat.py` & `treelite-4.2.0/treelite/compat.py`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/treelite/core.py` & `treelite-4.2.0/treelite/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         # Building docs
         return None  # type: ignore
     if sys.version_info >= (3, 8) and sys.platform == "win32":
         # pylint: disable=no-member
         os.add_dll_directory(
             os.path.join(os.path.normpath(sys.base_prefix), "Library", "bin")
         )
-    lib = ctypes.cdll.LoadLibrary(lib_path[0])
+    lib = ctypes.CDLL(lib_path[0], mode=ctypes.RTLD_GLOBAL)
     lib.TreeliteGetLastError.restype = ctypes.c_char_p
     lib.log_callback = _log_callback
     lib.warn_callback = _warn_callback
     if lib.TreeliteRegisterLogCallback(lib.log_callback) != 0:
         raise TreeliteError(py_str(lib.TreeliteGetLastError()))
     if lib.TreeliteRegisterWarningCallback(lib.warn_callback) != 0:
         raise TreeliteError(py_str(lib.TreeliteGetLastError()))
```

### Comparing `treelite-4.1.2/treelite/frontend.py` & `treelite-4.2.0/treelite/frontend.py`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/treelite/libpath.py` & `treelite-4.2.0/treelite/libpath.py`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/treelite/model.py` & `treelite-4.2.0/treelite/model.py`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/treelite/model_builder.py` & `treelite-4.2.0/treelite/model_builder.py`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/treelite/model_builder_legacy.py` & `treelite-4.2.0/treelite/model_builder_legacy.py`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/treelite/util.py` & `treelite-4.2.0/treelite/util.py`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/treelite/gtil/gtil.py` & `treelite-4.2.0/treelite/gtil/gtil.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,36 +159,35 @@
         )
     if len(data.shape) != 2:
         raise ValueError('Argument "data" must be a 2D array')
 
     is_dense = isinstance(data, np.ndarray)
 
     if is_dense:
-        data = np.array(
-            data, copy=False, dtype=typestr_to_numpy_type(model.input_type), order="C"
+        data = np.asarray(
+            data, dtype=typestr_to_numpy_type(model.input_type), order="C"
         )
         if data.shape[1] < model.num_feature:
             # Pad missing features with NAs
             data = np.pad(
                 data,
                 ((0, 0), (0, model.num_feature - data.shape[1])),
                 "constant",
                 constant_values="nan",
             )
             assert data.shape[1] == model.num_feature
     else:
         assert isinstance(data, csr_matrix)
-        elems = np.array(
+        elems = np.asarray(
             data.data,
-            copy=False,
             dtype=typestr_to_numpy_type(model.input_type),
             order="C",
         )
-        col_ind = np.array(data.indices, copy=False, dtype=np.uint64, order="C")
-        row_ptr = np.array(data.indptr, copy=False, dtype=np.uint64, order="C")
+        col_ind = np.asarray(data.indices, dtype=np.uint64, order="C")
+        row_ptr = np.asarray(data.indptr, dtype=np.uint64, order="C")
     output_shape_ptr = ctypes.POINTER(ctypes.c_uint64)()
     output_ndim = ctypes.c_uint64()
     _check_call(
         _LIB.TreeliteGTILGetOutputShape(
             model.handle,
             ctypes.c_uint64(data.shape[0]),
             config.handle,
```

### Comparing `treelite-4.1.2/treelite/sklearn/__init__.py` & `treelite-4.2.0/treelite/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/treelite/sklearn/importer.py` & `treelite-4.2.0/treelite/sklearn/importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         """Add an array to the collection"""
         if self.dtype != "void":
             assert array.dtype == self.dtype
         if expected_shape:
             assert (
                 array.shape == expected_shape
             ), f"Expected shape: {expected_shape}, Got shape {array.shape}"
-        v = np.array(array, copy=False, dtype=self.dtype, order="C")
+        v = np.asarray(array, dtype=self.dtype, order="C")
         self.collection.append(v)
 
     def as_c_array(self):
         """Prepare the collection to pass as an argument of a C function"""
         if not self.collection:
             return None  # return nullptr to represent empty array
         for v in self.collection:
```

### Comparing `treelite-4.1.2/treelite/sklearn/isolation_forest.py` & `treelite-4.2.0/treelite/sklearn/isolation_forest.py`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/hatch_build.py` & `treelite-4.2.0/hatch_build.py`

 * *Files identical despite different names*

### Comparing `treelite-4.1.2/pyproject.toml` & `treelite-4.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "hatchling>=1.12.1"
 ]
 backend-path = ["."]
 build-backend = "packager.pep517"
 
 [project]
 name = "treelite"
-version = "4.1.2"
+version = "4.2.0"
 authors = [
     {name = "Hyunsu Cho", email = "chohyu01@cs.washington.edu"}
 ]
 description = "Treelite: Universal model exchange format for decision tree forests"
 readme = {file = "README.rst", content-type = "text/x-rst"}
 requires-python = ">=3.8"
 license = {text = "Apache-2.0"}
@@ -39,7 +39,19 @@
 scikit-learn = ["scikit-learn"]
 testing = ["scikit-learn", "pytest", "hypothesis", "pandas"]
 
 [tool.mypy]
 plugins = "numpy.typing.mypy_plugin"
 
 [tool.hatch.build.targets.wheel.hooks.custom]
+
+[tool.ruff]
+line-length = 120
+
+# this should be set to the oldest version of python treelite supports
+target-version = "py38"
+
+[tool.ruff.lint]
+select = [
+    # numpy 2.0 deprecations/removals
+    "NPY201",
+]
```

### Comparing `treelite-4.1.2/PKG-INFO` & `treelite-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: treelite
-Version: 4.1.2
+Version: 4.2.0
 Summary: Treelite: Universal model exchange format for decision tree forests
 Project-URL: documentation, https://treelite.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/dmlc/treelite
 Author-email: Hyunsu Cho <chohyu01@cs.washington.edu>
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

