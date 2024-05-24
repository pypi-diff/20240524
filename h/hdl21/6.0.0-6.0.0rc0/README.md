# Comparing `tmp/hdl21-6.0.0.tar.gz` & `tmp/hdl21-6.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdl21-6.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "hdl21-6.0.0rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hdl21-6.0.0.tar` & `hdl21-6.0.0rc0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     1524 2024-05-24 16:13:54.035427 hdl21-6.0.0/LICENSE
--rw-r--r--   0        0        0     1351 2024-05-24 17:12:01.391321 hdl21-6.0.0/hdl21/__init__.py
--rw-r--r--   0        0        0     4721 2023-06-26 21:03:45.980722 hdl21-6.0.0/hdl21/attrmagic.py
--rw-r--r--   0        0        0    18972 2023-10-17 23:20:13.077158 hdl21-6.0.0/hdl21/bundle.py
--rw-r--r--   0        0        0     2400 2022-11-01 16:11:00.768707 hdl21-6.0.0/hdl21/call.py
--rw-r--r--   0        0        0     1650 2023-10-24 23:26:54.749518 hdl21-6.0.0/hdl21/concat.py
--rw-r--r--   0        0        0      566 2023-01-09 00:49:33.208004 hdl21-6.0.0/hdl21/concatable.py
--rw-r--r--   0        0        0      773 2023-01-09 00:49:33.208159 hdl21-6.0.0/hdl21/connect.py
--rw-r--r--   0        0        0     3503 2024-04-19 00:12:11.461991 hdl21-6.0.0/hdl21/datatype.py
--rw-r--r--   0        0        0      538 2023-06-26 21:03:45.982266 hdl21-6.0.0/hdl21/default.py
--rw-r--r--   0        0        0     1674 2023-06-23 17:09:45.589894 hdl21-6.0.0/hdl21/diff_pair.py
--rw-r--r--   0        0        0       57 2023-10-24 23:26:54.750052 hdl21-6.0.0/hdl21/elab/__init__.py
--rw-r--r--   0        0        0     1346 2023-10-24 23:26:54.750234 hdl21-6.0.0/hdl21/elab/default.py
--rw-r--r--   0        0        0     3345 2023-10-24 23:26:54.750574 hdl21-6.0.0/hdl21/elab/elab.py
--rw-r--r--   0        0        0      800 2023-10-17 23:20:13.077961 hdl21-6.0.0/hdl21/elab/elaboratable.py
--rw-r--r--   0        0        0        0 2023-10-24 23:26:54.750602 hdl21-6.0.0/hdl21/elab/elaborator.py
--rw-r--r--   0        0        0        0 2023-10-24 23:26:54.750838 hdl21-6.0.0/hdl21/elab/helpers/__init__.py
--rw-r--r--   0        0        0     3732 2023-10-24 23:26:54.751019 hdl21-6.0.0/hdl21/elab/helpers/resolve_ref_types.py
--rw-r--r--   0        0        0     2966 2023-10-24 23:26:54.751487 hdl21-6.0.0/hdl21/elab/helpers/width.py
--rw-r--r--   0        0        0      526 2023-10-24 23:26:54.751790 hdl21-6.0.0/hdl21/elab/passes/__init__.py
--rw-r--r--   0        0        0     3999 2023-10-24 23:26:54.751963 hdl21-6.0.0/hdl21/elab/passes/arrays.py
--rw-r--r--   0        0        0    10361 2023-10-25 18:18:42.178696 hdl21-6.0.0/hdl21/elab/passes/base.py
--rw-r--r--   0        0        0     9167 2023-10-24 23:26:54.752348 hdl21-6.0.0/hdl21/elab/passes/conntypes.py
--rw-r--r--   0        0        0    18431 2024-04-19 00:12:11.462546 hdl21-6.0.0/hdl21/elab/passes/flatten_bundles.py
--rw-r--r--   0        0        0     3458 2023-10-24 23:26:54.752848 hdl21-6.0.0/hdl21/elab/passes/inst_bundles.py
--rw-r--r--   0        0        0      612 2023-10-25 18:18:42.179947 hdl21-6.0.0/hdl21/elab/passes/mark_modules.py
--rw-r--r--   0        0        0     4947 2023-10-24 23:26:54.753171 hdl21-6.0.0/hdl21/elab/passes/orphanage.py
--rw-r--r--   0        0        0    14002 2023-10-24 23:26:54.753499 hdl21-6.0.0/hdl21/elab/passes/portrefs.py
--rw-r--r--   0        0        0     7343 2023-10-24 23:26:54.753663 hdl21-6.0.0/hdl21/elab/passes/slices.py
--rw-r--r--   0        0        0     4629 2024-04-19 00:12:11.462923 hdl21-6.0.0/hdl21/external_module.py
--rw-r--r--   0        0        0     6867 2024-04-19 00:12:11.463252 hdl21-6.0.0/hdl21/flatten.py
--rw-r--r--   0        0        0     7466 2023-11-14 19:05:18.679788 hdl21-6.0.0/hdl21/generator.py
--rw-r--r--   0        0        0     6015 2023-11-14 18:27:36.627503 hdl21-6.0.0/hdl21/generators.py
--rw-r--r--   0        0        0    12854 2023-10-17 23:20:13.080563 hdl21-6.0.0/hdl21/instance.py
--rw-r--r--   0        0        0     3709 2024-04-19 00:12:11.463890 hdl21-6.0.0/hdl21/instantiable.py
--rw-r--r--   0        0        0      294 2023-06-26 21:03:45.983897 hdl21-6.0.0/hdl21/literal.py
--rw-r--r--   0        0        0    15194 2023-10-11 05:16:17.107499 hdl21-6.0.0/hdl21/module.py
--rw-r--r--   0        0        0     1383 2024-05-24 16:02:31.216886 hdl21-6.0.0/hdl21/netlisting.py
--rw-r--r--   0        0        0     1262 2024-04-19 00:12:11.464249 hdl21-6.0.0/hdl21/noconn.py
--rw-r--r--   0        0        0      191 2023-01-09 00:49:23.102402 hdl21-6.0.0/hdl21/one_or_more.py
--rw-r--r--   0        0        0    12486 2024-04-19 00:12:11.464832 hdl21-6.0.0/hdl21/params.py
--rw-r--r--   0        0        0       83 2023-06-09 23:37:53.336517 hdl21-6.0.0/hdl21/pdk/__init__.py
--rw-r--r--   0        0        0     1648 2023-09-05 17:20:37.565597 hdl21-6.0.0/hdl21/pdk/corner.py
--rw-r--r--   0        0        0     3225 2023-10-11 16:45:30.223184 hdl21-6.0.0/hdl21/pdk/installation.py
--rw-r--r--   0        0        0     6198 2023-09-05 17:20:37.565977 hdl21-6.0.0/hdl21/pdk/pdk.py
--rw-r--r--   0        0        0      861 2022-12-15 00:46:13.488638 hdl21-6.0.0/hdl21/pdk/sample_pdk/__init__.py
--rw-r--r--   0        0        0     5242 2024-04-19 00:12:11.465238 hdl21-6.0.0/hdl21/pdk/sample_pdk/pdk.py
--rw-r--r--   0        0        0      891 2023-09-05 17:20:37.566263 hdl21-6.0.0/hdl21/pdk/sample_pdk/readme.md
--rw-r--r--   0        0        0      639 2023-06-23 19:51:39.211397 hdl21-6.0.0/hdl21/pdk/sample_pdk/resources/models.sp
--rw-r--r--   0        0        0     1470 2022-12-15 00:46:13.489266 hdl21-6.0.0/hdl21/pdk/sample_pdk/test_sample_pdk.py
--rw-r--r--   0        0        0      703 2022-08-12 23:32:38.552761 hdl21-6.0.0/hdl21/pdk/test_pdk.py
--rw-r--r--   0        0        0     1320 2024-04-19 00:12:11.465531 hdl21-6.0.0/hdl21/portref.py
--rw-r--r--   0        0        0    18875 2024-04-19 00:12:11.465914 hdl21-6.0.0/hdl21/prefix.py
--rw-r--r--   0        0        0    23640 2024-04-19 00:12:11.466351 hdl21-6.0.0/hdl21/primitives.py
--rw-r--r--   0        0        0     2300 2023-03-17 23:05:04.241227 hdl21-6.0.0/hdl21/props.py
--rw-r--r--   0        0        0      197 2023-08-15 21:10:54.038539 hdl21-6.0.0/hdl21/proto/__init__.py
--rw-r--r--   0        0        0    18076 2024-04-19 00:12:11.466841 hdl21-6.0.0/hdl21/proto/exporting.py
--rw-r--r--   0        0        0    15400 2023-10-17 23:20:13.081575 hdl21-6.0.0/hdl21/proto/importing.py
--rw-r--r--   0        0        0     1724 2023-09-05 17:20:37.566918 hdl21-6.0.0/hdl21/qualname.py
--rw-r--r--   0        0        0     2442 2023-07-11 16:27:41.287966 hdl21-6.0.0/hdl21/role.py
--rw-r--r--   0        0        0     4333 2024-04-19 00:12:11.467210 hdl21-6.0.0/hdl21/scalar.py
--rw-r--r--   0        0        0     9558 2024-04-19 00:12:11.467489 hdl21-6.0.0/hdl21/signal.py
--rw-r--r--   0        0        0       90 2023-08-25 22:51:16.177675 hdl21-6.0.0/hdl21/sim/__init__.py
--rw-r--r--   0        0        0    14377 2024-04-19 00:12:11.467827 hdl21-6.0.0/hdl21/sim/data.py
--rw-r--r--   0        0        0     8328 2022-10-17 22:32:24.400554 hdl21-6.0.0/hdl21/sim/delay.py
--rw-r--r--   0        0        0    13598 2024-04-19 00:12:11.468128 hdl21-6.0.0/hdl21/sim/proto.py
--rw-r--r--   0        0        0     9850 2024-03-26 21:17:20.629599 hdl21-6.0.0/hdl21/sim/tests/test_sim.py
--rw-r--r--   0        0        0     5367 2024-04-19 00:12:11.468343 hdl21-6.0.0/hdl21/slice.py
--rw-r--r--   0        0        0     2123 2023-01-09 00:49:33.208993 hdl21-6.0.0/hdl21/sliceable.py
--rw-r--r--   0        0        0     3872 2024-04-19 00:12:11.468526 hdl21-6.0.0/hdl21/source_info.py
--rw-r--r--   0        0        0        0 2021-04-16 16:15:12.000000 hdl21-6.0.0/hdl21/tests/__init__.py
--rw-r--r--   0        0        0     1091 2022-11-26 00:08:30.567369 hdl21-6.0.0/hdl21/tests/content.py
--rw-r--r--   0        0        0     1733 2023-10-25 18:18:42.184650 hdl21-6.0.0/hdl21/tests/test_builtin_generators.py
--rw-r--r--   0        0        0    23843 2023-10-24 23:26:54.754232 hdl21-6.0.0/hdl21/tests/test_bundles.py
--rw-r--r--   0        0        0     5483 2023-10-24 23:26:54.754515 hdl21-6.0.0/hdl21/tests/test_conns.py
--rw-r--r--   0        0        0     7395 2023-10-25 18:18:42.185052 hdl21-6.0.0/hdl21/tests/test_doc_examples.py
--rw-r--r--   0        0        0    18297 2023-10-17 23:20:13.083034 hdl21-6.0.0/hdl21/tests/test_exports.py
--rw-r--r--   0        0        0     4496 2024-01-12 04:47:03.357676 hdl21-6.0.0/hdl21/tests/test_flatten.py
--rw-r--r--   0        0        0    45291 2024-05-24 17:12:01.391451 hdl21-6.0.0/hdl21/tests/test_hdl21.py
--rw-r--r--   0        0        0     5386 2024-04-19 00:12:11.468859 hdl21-6.0.0/hdl21/tests/test_params.py
--rw-r--r--   0        0        0    15930 2024-04-19 00:12:11.469166 hdl21-6.0.0/hdl21/tests/test_prefix.py
--rw-r--r--   0        0        0      741 2022-10-17 20:35:07.208645 hdl21-6.0.0/hdl21/tests/test_source_info.py
--rw-r--r--   0        0        0      372 2023-03-17 23:05:04.244780 hdl21-6.0.0/hdl21/visibility.py
--rw-r--r--   0        0        0     3739 2023-10-17 23:20:13.083776 hdl21-6.0.0/hdl21/walker.py
--rw-r--r--   0        0        0     1470 2024-05-24 17:12:01.379871 hdl21-6.0.0/pyproject.toml
--rw-r--r--   0        0        0    57748 2024-05-24 16:17:45.223110 hdl21-6.0.0/readme.md
--rw-r--r--   0        0        0    58987 1970-01-01 00:00:00.000000 hdl21-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1524 2024-05-24 16:13:54.035427 hdl21-6.0.0rc0/LICENSE
+-rw-r--r--   0        0        0     1354 2024-05-24 16:15:34.878694 hdl21-6.0.0rc0/hdl21/__init__.py
+-rw-r--r--   0        0        0     4721 2023-06-26 21:03:45.980722 hdl21-6.0.0rc0/hdl21/attrmagic.py
+-rw-r--r--   0        0        0    18972 2023-10-17 23:20:13.077158 hdl21-6.0.0rc0/hdl21/bundle.py
+-rw-r--r--   0        0        0     2400 2022-11-01 16:11:00.768707 hdl21-6.0.0rc0/hdl21/call.py
+-rw-r--r--   0        0        0     1650 2023-10-24 23:26:54.749518 hdl21-6.0.0rc0/hdl21/concat.py
+-rw-r--r--   0        0        0      566 2023-01-09 00:49:33.208004 hdl21-6.0.0rc0/hdl21/concatable.py
+-rw-r--r--   0        0        0      773 2023-01-09 00:49:33.208159 hdl21-6.0.0rc0/hdl21/connect.py
+-rw-r--r--   0        0        0     3503 2024-04-19 00:12:11.461991 hdl21-6.0.0rc0/hdl21/datatype.py
+-rw-r--r--   0        0        0      538 2023-06-26 21:03:45.982266 hdl21-6.0.0rc0/hdl21/default.py
+-rw-r--r--   0        0        0     1674 2023-06-23 17:09:45.589894 hdl21-6.0.0rc0/hdl21/diff_pair.py
+-rw-r--r--   0        0        0       57 2023-10-24 23:26:54.750052 hdl21-6.0.0rc0/hdl21/elab/__init__.py
+-rw-r--r--   0        0        0     1346 2023-10-24 23:26:54.750234 hdl21-6.0.0rc0/hdl21/elab/default.py
+-rw-r--r--   0        0        0     3345 2023-10-24 23:26:54.750574 hdl21-6.0.0rc0/hdl21/elab/elab.py
+-rw-r--r--   0        0        0      800 2023-10-17 23:20:13.077961 hdl21-6.0.0rc0/hdl21/elab/elaboratable.py
+-rw-r--r--   0        0        0        0 2023-10-24 23:26:54.750602 hdl21-6.0.0rc0/hdl21/elab/elaborator.py
+-rw-r--r--   0        0        0        0 2023-10-24 23:26:54.750838 hdl21-6.0.0rc0/hdl21/elab/helpers/__init__.py
+-rw-r--r--   0        0        0     3732 2023-10-24 23:26:54.751019 hdl21-6.0.0rc0/hdl21/elab/helpers/resolve_ref_types.py
+-rw-r--r--   0        0        0     2966 2023-10-24 23:26:54.751487 hdl21-6.0.0rc0/hdl21/elab/helpers/width.py
+-rw-r--r--   0        0        0      526 2023-10-24 23:26:54.751790 hdl21-6.0.0rc0/hdl21/elab/passes/__init__.py
+-rw-r--r--   0        0        0     3999 2023-10-24 23:26:54.751963 hdl21-6.0.0rc0/hdl21/elab/passes/arrays.py
+-rw-r--r--   0        0        0    10361 2023-10-25 18:18:42.178696 hdl21-6.0.0rc0/hdl21/elab/passes/base.py
+-rw-r--r--   0        0        0     9167 2023-10-24 23:26:54.752348 hdl21-6.0.0rc0/hdl21/elab/passes/conntypes.py
+-rw-r--r--   0        0        0    18431 2024-04-19 00:12:11.462546 hdl21-6.0.0rc0/hdl21/elab/passes/flatten_bundles.py
+-rw-r--r--   0        0        0     3458 2023-10-24 23:26:54.752848 hdl21-6.0.0rc0/hdl21/elab/passes/inst_bundles.py
+-rw-r--r--   0        0        0      612 2023-10-25 18:18:42.179947 hdl21-6.0.0rc0/hdl21/elab/passes/mark_modules.py
+-rw-r--r--   0        0        0     4947 2023-10-24 23:26:54.753171 hdl21-6.0.0rc0/hdl21/elab/passes/orphanage.py
+-rw-r--r--   0        0        0    14002 2023-10-24 23:26:54.753499 hdl21-6.0.0rc0/hdl21/elab/passes/portrefs.py
+-rw-r--r--   0        0        0     7343 2023-10-24 23:26:54.753663 hdl21-6.0.0rc0/hdl21/elab/passes/slices.py
+-rw-r--r--   0        0        0     4629 2024-04-19 00:12:11.462923 hdl21-6.0.0rc0/hdl21/external_module.py
+-rw-r--r--   0        0        0     6867 2024-04-19 00:12:11.463252 hdl21-6.0.0rc0/hdl21/flatten.py
+-rw-r--r--   0        0        0     7466 2023-11-14 19:05:18.679788 hdl21-6.0.0rc0/hdl21/generator.py
+-rw-r--r--   0        0        0     6015 2023-11-14 18:27:36.627503 hdl21-6.0.0rc0/hdl21/generators.py
+-rw-r--r--   0        0        0    12854 2023-10-17 23:20:13.080563 hdl21-6.0.0rc0/hdl21/instance.py
+-rw-r--r--   0        0        0     3709 2024-04-19 00:12:11.463890 hdl21-6.0.0rc0/hdl21/instantiable.py
+-rw-r--r--   0        0        0      294 2023-06-26 21:03:45.983897 hdl21-6.0.0rc0/hdl21/literal.py
+-rw-r--r--   0        0        0    15194 2023-10-11 05:16:17.107499 hdl21-6.0.0rc0/hdl21/module.py
+-rw-r--r--   0        0        0     1383 2024-05-24 16:02:31.216886 hdl21-6.0.0rc0/hdl21/netlisting.py
+-rw-r--r--   0        0        0     1262 2024-04-19 00:12:11.464249 hdl21-6.0.0rc0/hdl21/noconn.py
+-rw-r--r--   0        0        0      191 2023-01-09 00:49:23.102402 hdl21-6.0.0rc0/hdl21/one_or_more.py
+-rw-r--r--   0        0        0    12486 2024-04-19 00:12:11.464832 hdl21-6.0.0rc0/hdl21/params.py
+-rw-r--r--   0        0        0       83 2023-06-09 23:37:53.336517 hdl21-6.0.0rc0/hdl21/pdk/__init__.py
+-rw-r--r--   0        0        0     1648 2023-09-05 17:20:37.565597 hdl21-6.0.0rc0/hdl21/pdk/corner.py
+-rw-r--r--   0        0        0     3225 2023-10-11 16:45:30.223184 hdl21-6.0.0rc0/hdl21/pdk/installation.py
+-rw-r--r--   0        0        0     6198 2023-09-05 17:20:37.565977 hdl21-6.0.0rc0/hdl21/pdk/pdk.py
+-rw-r--r--   0        0        0      861 2022-12-15 00:46:13.488638 hdl21-6.0.0rc0/hdl21/pdk/sample_pdk/__init__.py
+-rw-r--r--   0        0        0     5242 2024-04-19 00:12:11.465238 hdl21-6.0.0rc0/hdl21/pdk/sample_pdk/pdk.py
+-rw-r--r--   0        0        0      891 2023-09-05 17:20:37.566263 hdl21-6.0.0rc0/hdl21/pdk/sample_pdk/readme.md
+-rw-r--r--   0        0        0      639 2023-06-23 19:51:39.211397 hdl21-6.0.0rc0/hdl21/pdk/sample_pdk/resources/models.sp
+-rw-r--r--   0        0        0     1470 2022-12-15 00:46:13.489266 hdl21-6.0.0rc0/hdl21/pdk/sample_pdk/test_sample_pdk.py
+-rw-r--r--   0        0        0      703 2022-08-12 23:32:38.552761 hdl21-6.0.0rc0/hdl21/pdk/test_pdk.py
+-rw-r--r--   0        0        0     1320 2024-04-19 00:12:11.465531 hdl21-6.0.0rc0/hdl21/portref.py
+-rw-r--r--   0        0        0    18875 2024-04-19 00:12:11.465914 hdl21-6.0.0rc0/hdl21/prefix.py
+-rw-r--r--   0        0        0    23640 2024-04-19 00:12:11.466351 hdl21-6.0.0rc0/hdl21/primitives.py
+-rw-r--r--   0        0        0     2300 2023-03-17 23:05:04.241227 hdl21-6.0.0rc0/hdl21/props.py
+-rw-r--r--   0        0        0      197 2023-08-15 21:10:54.038539 hdl21-6.0.0rc0/hdl21/proto/__init__.py
+-rw-r--r--   0        0        0    18076 2024-04-19 00:12:11.466841 hdl21-6.0.0rc0/hdl21/proto/exporting.py
+-rw-r--r--   0        0        0    15400 2023-10-17 23:20:13.081575 hdl21-6.0.0rc0/hdl21/proto/importing.py
+-rw-r--r--   0        0        0     1724 2023-09-05 17:20:37.566918 hdl21-6.0.0rc0/hdl21/qualname.py
+-rw-r--r--   0        0        0     2442 2023-07-11 16:27:41.287966 hdl21-6.0.0rc0/hdl21/role.py
+-rw-r--r--   0        0        0     4333 2024-04-19 00:12:11.467210 hdl21-6.0.0rc0/hdl21/scalar.py
+-rw-r--r--   0        0        0     9558 2024-04-19 00:12:11.467489 hdl21-6.0.0rc0/hdl21/signal.py
+-rw-r--r--   0        0        0       90 2023-08-25 22:51:16.177675 hdl21-6.0.0rc0/hdl21/sim/__init__.py
+-rw-r--r--   0        0        0    14377 2024-04-19 00:12:11.467827 hdl21-6.0.0rc0/hdl21/sim/data.py
+-rw-r--r--   0        0        0     8328 2022-10-17 22:32:24.400554 hdl21-6.0.0rc0/hdl21/sim/delay.py
+-rw-r--r--   0        0        0    13598 2024-04-19 00:12:11.468128 hdl21-6.0.0rc0/hdl21/sim/proto.py
+-rw-r--r--   0        0        0     9850 2024-03-26 21:17:20.629599 hdl21-6.0.0rc0/hdl21/sim/tests/test_sim.py
+-rw-r--r--   0        0        0     5367 2024-04-19 00:12:11.468343 hdl21-6.0.0rc0/hdl21/slice.py
+-rw-r--r--   0        0        0     2123 2023-01-09 00:49:33.208993 hdl21-6.0.0rc0/hdl21/sliceable.py
+-rw-r--r--   0        0        0     3872 2024-04-19 00:12:11.468526 hdl21-6.0.0rc0/hdl21/source_info.py
+-rw-r--r--   0        0        0        0 2021-04-16 16:15:12.000000 hdl21-6.0.0rc0/hdl21/tests/__init__.py
+-rw-r--r--   0        0        0     1091 2022-11-26 00:08:30.567369 hdl21-6.0.0rc0/hdl21/tests/content.py
+-rw-r--r--   0        0        0     1733 2023-10-25 18:18:42.184650 hdl21-6.0.0rc0/hdl21/tests/test_builtin_generators.py
+-rw-r--r--   0        0        0    23843 2023-10-24 23:26:54.754232 hdl21-6.0.0rc0/hdl21/tests/test_bundles.py
+-rw-r--r--   0        0        0     5483 2023-10-24 23:26:54.754515 hdl21-6.0.0rc0/hdl21/tests/test_conns.py
+-rw-r--r--   0        0        0     7395 2023-10-25 18:18:42.185052 hdl21-6.0.0rc0/hdl21/tests/test_doc_examples.py
+-rw-r--r--   0        0        0    18297 2023-10-17 23:20:13.083034 hdl21-6.0.0rc0/hdl21/tests/test_exports.py
+-rw-r--r--   0        0        0     4496 2024-01-12 04:47:03.357676 hdl21-6.0.0rc0/hdl21/tests/test_flatten.py
+-rw-r--r--   0        0        0    45294 2024-05-24 16:16:09.970544 hdl21-6.0.0rc0/hdl21/tests/test_hdl21.py
+-rw-r--r--   0        0        0     5386 2024-04-19 00:12:11.468859 hdl21-6.0.0rc0/hdl21/tests/test_params.py
+-rw-r--r--   0        0        0    15930 2024-04-19 00:12:11.469166 hdl21-6.0.0rc0/hdl21/tests/test_prefix.py
+-rw-r--r--   0        0        0      741 2022-10-17 20:35:07.208645 hdl21-6.0.0rc0/hdl21/tests/test_source_info.py
+-rw-r--r--   0        0        0      372 2023-03-17 23:05:04.244780 hdl21-6.0.0rc0/hdl21/visibility.py
+-rw-r--r--   0        0        0     3739 2023-10-17 23:20:13.083776 hdl21-6.0.0rc0/hdl21/walker.py
+-rw-r--r--   0        0        0     1479 2024-05-24 16:19:22.875923 hdl21-6.0.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    57748 2024-05-24 16:17:45.223110 hdl21-6.0.0rc0/readme.md
+-rw-r--r--   0        0        0    58996 1970-01-01 00:00:00.000000 hdl21-6.0.0rc0/PKG-INFO
```

### Comparing `hdl21-6.0.0/LICENSE` & `hdl21-6.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/__init__.py` & `hdl21-6.0.0rc0/hdl21/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ 
 # Hdl21 Hardware Description Library 
 """
 
-__version__ = "6.0.0"  # VLSIR_VERSION
+__version__ = "6.0.0rc0"  # VLSIR_VERSION
 
 # Internal (python) module aliases, overridden by names such as the `module` decorator function.
 from . import module as _module_module
 from . import bundle as _bundle_module
 from . import external_module as _external_module_module
 from . import instance as _instance_module
 from . import generator as _generator_module
```

### Comparing `hdl21-6.0.0/hdl21/attrmagic.py` & `hdl21-6.0.0rc0/hdl21/attrmagic.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/bundle.py` & `hdl21-6.0.0rc0/hdl21/bundle.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/call.py` & `hdl21-6.0.0rc0/hdl21/call.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/concat.py` & `hdl21-6.0.0rc0/hdl21/concat.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/concatable.py` & `hdl21-6.0.0rc0/hdl21/concatable.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/connect.py` & `hdl21-6.0.0rc0/hdl21/connect.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/datatype.py` & `hdl21-6.0.0rc0/hdl21/datatype.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/default.py` & `hdl21-6.0.0rc0/hdl21/default.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/diff_pair.py` & `hdl21-6.0.0rc0/hdl21/diff_pair.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/elab/default.py` & `hdl21-6.0.0rc0/hdl21/elab/default.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/elab/elab.py` & `hdl21-6.0.0rc0/hdl21/elab/elab.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/elab/elaboratable.py` & `hdl21-6.0.0rc0/hdl21/elab/elaboratable.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/elab/helpers/resolve_ref_types.py` & `hdl21-6.0.0rc0/hdl21/elab/helpers/resolve_ref_types.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/elab/helpers/width.py` & `hdl21-6.0.0rc0/hdl21/elab/helpers/width.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/elab/passes/__init__.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/elab/passes/arrays.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/arrays.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/elab/passes/base.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/base.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/elab/passes/conntypes.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/conntypes.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/elab/passes/flatten_bundles.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/flatten_bundles.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/elab/passes/inst_bundles.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/inst_bundles.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/elab/passes/mark_modules.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/mark_modules.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/elab/passes/orphanage.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/orphanage.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/elab/passes/portrefs.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/portrefs.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/elab/passes/slices.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/slices.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/external_module.py` & `hdl21-6.0.0rc0/hdl21/external_module.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/flatten.py` & `hdl21-6.0.0rc0/hdl21/flatten.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/generator.py` & `hdl21-6.0.0rc0/hdl21/generator.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/generators.py` & `hdl21-6.0.0rc0/hdl21/generators.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/instance.py` & `hdl21-6.0.0rc0/hdl21/instance.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/instantiable.py` & `hdl21-6.0.0rc0/hdl21/instantiable.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/module.py` & `hdl21-6.0.0rc0/hdl21/module.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/netlisting.py` & `hdl21-6.0.0rc0/hdl21/netlisting.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/noconn.py` & `hdl21-6.0.0rc0/hdl21/noconn.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/params.py` & `hdl21-6.0.0rc0/hdl21/params.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/pdk/corner.py` & `hdl21-6.0.0rc0/hdl21/pdk/corner.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/pdk/installation.py` & `hdl21-6.0.0rc0/hdl21/pdk/installation.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/pdk/pdk.py` & `hdl21-6.0.0rc0/hdl21/pdk/pdk.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/pdk/sample_pdk/__init__.py` & `hdl21-6.0.0rc0/hdl21/pdk/sample_pdk/__init__.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/pdk/sample_pdk/pdk.py` & `hdl21-6.0.0rc0/hdl21/pdk/sample_pdk/pdk.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/pdk/sample_pdk/readme.md` & `hdl21-6.0.0rc0/hdl21/pdk/sample_pdk/readme.md`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/pdk/sample_pdk/resources/models.sp` & `hdl21-6.0.0rc0/hdl21/pdk/sample_pdk/resources/models.sp`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/pdk/sample_pdk/test_sample_pdk.py` & `hdl21-6.0.0rc0/hdl21/pdk/sample_pdk/test_sample_pdk.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/pdk/test_pdk.py` & `hdl21-6.0.0rc0/hdl21/pdk/test_pdk.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/portref.py` & `hdl21-6.0.0rc0/hdl21/portref.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/prefix.py` & `hdl21-6.0.0rc0/hdl21/prefix.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/primitives.py` & `hdl21-6.0.0rc0/hdl21/primitives.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/props.py` & `hdl21-6.0.0rc0/hdl21/props.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/proto/exporting.py` & `hdl21-6.0.0rc0/hdl21/proto/exporting.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/proto/importing.py` & `hdl21-6.0.0rc0/hdl21/proto/importing.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/qualname.py` & `hdl21-6.0.0rc0/hdl21/qualname.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/role.py` & `hdl21-6.0.0rc0/hdl21/role.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/scalar.py` & `hdl21-6.0.0rc0/hdl21/scalar.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/signal.py` & `hdl21-6.0.0rc0/hdl21/signal.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/sim/data.py` & `hdl21-6.0.0rc0/hdl21/sim/data.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/sim/delay.py` & `hdl21-6.0.0rc0/hdl21/sim/delay.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/sim/proto.py` & `hdl21-6.0.0rc0/hdl21/sim/proto.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/sim/tests/test_sim.py` & `hdl21-6.0.0rc0/hdl21/sim/tests/test_sim.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/slice.py` & `hdl21-6.0.0rc0/hdl21/slice.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/sliceable.py` & `hdl21-6.0.0rc0/hdl21/sliceable.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/source_info.py` & `hdl21-6.0.0rc0/hdl21/source_info.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/tests/content.py` & `hdl21-6.0.0rc0/hdl21/tests/content.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/tests/test_builtin_generators.py` & `hdl21-6.0.0rc0/hdl21/tests/test_builtin_generators.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/tests/test_bundles.py` & `hdl21-6.0.0rc0/hdl21/tests/test_bundles.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/tests/test_conns.py` & `hdl21-6.0.0rc0/hdl21/tests/test_conns.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/tests/test_doc_examples.py` & `hdl21-6.0.0rc0/hdl21/tests/test_doc_examples.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/tests/test_exports.py` & `hdl21-6.0.0rc0/hdl21/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/tests/test_flatten.py` & `hdl21-6.0.0rc0/hdl21/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/tests/test_hdl21.py` & `hdl21-6.0.0rc0/hdl21/tests/test_hdl21.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import copy, pytest
 import hdl21 as h
 
 T = TypeVar("T")
 
 
 def test_version():
-    assert h.__version__ == "6.0.0"  # VLSIR_VERSION
+    assert h.__version__ == "6.0.0rc0"  # VLSIR_VERSION
 
 
 def test_module1():
     """Initial Module Test"""
 
     @h.module
     class M1:
```

### Comparing `hdl21-6.0.0/hdl21/tests/test_params.py` & `hdl21-6.0.0rc0/hdl21/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/tests/test_prefix.py` & `hdl21-6.0.0rc0/hdl21/tests/test_prefix.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/tests/test_source_info.py` & `hdl21-6.0.0rc0/hdl21/tests/test_source_info.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/hdl21/walker.py` & `hdl21-6.0.0rc0/hdl21/walker.py`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/pyproject.toml` & `hdl21-6.0.0rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "hdl21"
 description = "Hardware Description Library"
-version = "6.0.0" # VLSIR_VERSION
+version = "6.0.0rc0" # VLSIR_VERSION
 dependencies = [
-  "vlsir>=6.0.0,<7",      # VLSIR_VERSION
-  "vlsirtools>=6.0.0,<7", # VLSIR_VERSION
+  "vlsir>=6.0.0rc0,<7",      # VLSIR_VERSION
+  "vlsirtools>=6.0.0rc0,<7", # VLSIR_VERSION
   "pydantic>=1.9.0,<2.7",
 ]
 requires-python = ">=3.7, <3.13"
 maintainers = [{ name = "Dan Fritchman", email = "dan@fritch.mn" }]
 authors = [
   { name = "Dan Fritchman", email = "dan@fritch.mn" },
   { name = "Thomas Pluck" },
```

### Comparing `hdl21-6.0.0/readme.md` & `hdl21-6.0.0rc0/readme.md`

 * *Files identical despite different names*

### Comparing `hdl21-6.0.0/PKG-INFO` & `hdl21-6.0.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: hdl21
-Version: 6.0.0
+Version: 6.0.0rc0
 Summary: Hardware Description Library
 Keywords: HDL,EDA,analog,circuit
 Author: Thomas Pluck, Kennedy Caisley, Zeyi Wang, Arya Reais-Parsi, Vighnesh Iyer
 Author-email: Dan Fritchman <dan@fritch.mn>, Curtis Mayberry <Curtisma3@gmail.com>
 Maintainer-email: Dan Fritchman <dan@fritch.mn>
 Requires-Python: >=3.7, <3.13
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
-Requires-Dist: vlsir>=6.0.0,<7
-Requires-Dist: vlsirtools>=6.0.0,<7
+Requires-Dist: vlsir>=6.0.0rc0,<7
+Requires-Dist: vlsirtools>=6.0.0rc0,<7
 Requires-Dist: pydantic>=1.9.0,<2.7
 Requires-Dist: pytest==7.1 ; extra == "dev"
 Requires-Dist: coverage ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pre-commit==2.20 ; extra == "dev"
 Requires-Dist: black==22.6 ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
```

