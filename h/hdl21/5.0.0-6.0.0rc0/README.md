# Comparing `tmp/hdl21-5.0.0.tar.gz` & `tmp/hdl21-6.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdl21-5.0.0.tar", last modified: Tue Nov 14 18:40:10 2023, max compression
+gzip compressed data, was "hdl21-6.0.0rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hdl21-5.0.0.tar` & `hdl21-6.0.0rc0.tar`

### file list

```diff
@@ -1,139 +1,87 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.347716 hdl21-5.0.0/
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.325531 hdl21-5.0.0/.github/
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.328471 hdl21-5.0.0/.github/workflows/
--rw-r--r--   0 dan        (501) staff       (20)     3458 2023-07-11 14:50:48.000000 hdl21-5.0.0/.github/workflows/test.yaml
--rw-r--r--   0 dan        (501) staff       (20)     2559 2023-06-07 23:06:22.000000 hdl21-5.0.0/.gitignore
--rw-r--r--   0 dan        (501) staff       (20)      164 2023-03-17 23:05:04.000000 hdl21-5.0.0/.pre-commit-config.yaml
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.328636 hdl21-5.0.0/.vscode/
--rw-r--r--   0 dan        (501) staff       (20)      280 2023-06-07 23:06:22.000000 hdl21-5.0.0/.vscode/settings.json
--rw-r--r--   0 dan        (501) staff       (20)      513 2021-04-16 16:11:28.000000 hdl21-5.0.0/Cargo.toml
--rw-r--r--   0 dan        (501) staff       (20)     1521 2021-04-16 16:18:38.000000 hdl21-5.0.0/LICENSE
--rw-r--r--   0 dan        (501) staff       (20)    58141 2023-11-14 18:40:10.347485 hdl21-5.0.0/PKG-INFO
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.329106 hdl21-5.0.0/SampleSitePdks/
--rw-r--r--   0 dan        (501) staff       (20)     1121 2022-06-13 20:52:07.000000 hdl21-5.0.0/SampleSitePdks/readme.md
--rw-r--r--   0 dan        (501) staff       (20)      982 2023-11-14 18:31:59.000000 hdl21-5.0.0/SampleSitePdks/setup.py
--rw-r--r--   0 dan        (501) staff       (20)     1521 2023-07-11 14:50:48.000000 hdl21-5.0.0/SampleSitePdks/sitepdks.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.330541 hdl21-5.0.0/examples/
--rw-r--r--   0 dan        (501) staff       (20)      634 2022-11-29 06:32:17.000000 hdl21-5.0.0/examples/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     2310 2023-07-11 16:27:41.000000 hdl21-5.0.0/examples/bundles.py
--rw-r--r--   0 dan        (501) staff       (20)     2675 2023-06-23 19:51:39.000000 hdl21-5.0.0/examples/diff_ota.py
--rw-r--r--   0 dan        (501) staff       (20)     4494 2022-11-29 06:32:17.000000 hdl21-5.0.0/examples/encoder.py
--rw-r--r--   0 dan        (501) staff       (20)     3596 2023-06-26 21:03:45.000000 hdl21-5.0.0/examples/idac.py
--rw-r--r--   0 dan        (501) staff       (20)     1727 2023-06-23 19:51:39.000000 hdl21-5.0.0/examples/mos_sim.py
--rw-r--r--   0 dan        (501) staff       (20)     7408 2022-12-01 18:46:32.000000 hdl21-5.0.0/examples/rdac.py
--rw-r--r--   0 dan        (501) staff       (20)     3768 2022-11-29 06:32:17.000000 hdl21-5.0.0/examples/ro.py
--rw-r--r--   0 dan        (501) staff       (20)      566 2023-07-11 16:27:41.000000 hdl21-5.0.0/examples/test_examples.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.336955 hdl21-5.0.0/hdl21/
--rw-r--r--   0 dan        (501) staff       (20)     1357 2023-11-14 18:31:59.000000 hdl21-5.0.0/hdl21/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     4721 2023-06-26 21:03:45.000000 hdl21-5.0.0/hdl21/attrmagic.py
--rw-r--r--   0 dan        (501) staff       (20)    18972 2023-10-17 23:20:13.000000 hdl21-5.0.0/hdl21/bundle.py
--rw-r--r--   0 dan        (501) staff       (20)     2400 2022-11-01 16:11:00.000000 hdl21-5.0.0/hdl21/call.py
--rw-r--r--   0 dan        (501) staff       (20)     1650 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/concat.py
--rw-r--r--   0 dan        (501) staff       (20)      566 2023-01-09 00:49:33.000000 hdl21-5.0.0/hdl21/concatable.py
--rw-r--r--   0 dan        (501) staff       (20)      773 2023-01-09 00:49:33.000000 hdl21-5.0.0/hdl21/connect.py
--rw-r--r--   0 dan        (501) staff       (20)     2541 2023-10-25 18:18:42.000000 hdl21-5.0.0/hdl21/datatype.py
--rw-r--r--   0 dan        (501) staff       (20)      538 2023-06-26 21:03:45.000000 hdl21-5.0.0/hdl21/default.py
--rw-r--r--   0 dan        (501) staff       (20)     1674 2023-06-23 17:09:45.000000 hdl21-5.0.0/hdl21/diff_pair.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.338465 hdl21-5.0.0/hdl21/elab/
--rw-r--r--   0 dan        (501) staff       (20)       57 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/elab/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     1346 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/elab/default.py
--rw-r--r--   0 dan        (501) staff       (20)     3345 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/elab/elab.py
--rw-r--r--   0 dan        (501) staff       (20)      800 2023-10-17 23:20:13.000000 hdl21-5.0.0/hdl21/elab/elaboratable.py
--rw-r--r--   0 dan        (501) staff       (20)        0 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/elab/elaborator.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.338826 hdl21-5.0.0/hdl21/elab/helpers/
--rw-r--r--   0 dan        (501) staff       (20)        0 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/elab/helpers/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     3732 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/elab/helpers/resolve_ref_types.py
--rw-r--r--   0 dan        (501) staff       (20)     2966 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/elab/helpers/width.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.340810 hdl21-5.0.0/hdl21/elab/passes/
--rw-r--r--   0 dan        (501) staff       (20)      526 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/elab/passes/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     3999 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/elab/passes/arrays.py
--rw-r--r--   0 dan        (501) staff       (20)    10361 2023-10-25 18:18:42.000000 hdl21-5.0.0/hdl21/elab/passes/base.py
--rw-r--r--   0 dan        (501) staff       (20)     9167 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/elab/passes/conntypes.py
--rw-r--r--   0 dan        (501) staff       (20)    18486 2023-10-25 18:18:42.000000 hdl21-5.0.0/hdl21/elab/passes/flatten_bundles.py
--rw-r--r--   0 dan        (501) staff       (20)     3458 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/elab/passes/inst_bundles.py
--rw-r--r--   0 dan        (501) staff       (20)      612 2023-10-25 18:18:42.000000 hdl21-5.0.0/hdl21/elab/passes/mark_modules.py
--rw-r--r--   0 dan        (501) staff       (20)     4947 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/elab/passes/orphanage.py
--rw-r--r--   0 dan        (501) staff       (20)    14002 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/elab/passes/portrefs.py
--rw-r--r--   0 dan        (501) staff       (20)     7343 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/elab/passes/slices.py
--rw-r--r--   0 dan        (501) staff       (20)     4662 2023-06-26 21:03:45.000000 hdl21-5.0.0/hdl21/external_module.py
--rw-r--r--   0 dan        (501) staff       (20)     7466 2023-11-06 19:15:02.000000 hdl21-5.0.0/hdl21/generator.py
--rw-r--r--   0 dan        (501) staff       (20)     6015 2023-11-14 18:27:36.000000 hdl21-5.0.0/hdl21/generators.py
--rw-r--r--   0 dan        (501) staff       (20)    12854 2023-10-17 23:20:13.000000 hdl21-5.0.0/hdl21/instance.py
--rw-r--r--   0 dan        (501) staff       (20)     3286 2023-10-25 19:35:07.000000 hdl21-5.0.0/hdl21/instantiable.py
--rw-r--r--   0 dan        (501) staff       (20)      294 2023-06-26 21:03:45.000000 hdl21-5.0.0/hdl21/literal.py
--rw-r--r--   0 dan        (501) staff       (20)    15194 2023-10-11 05:16:17.000000 hdl21-5.0.0/hdl21/module.py
--rw-r--r--   0 dan        (501) staff       (20)     1383 2023-08-25 22:51:16.000000 hdl21-5.0.0/hdl21/netlisting.py
--rw-r--r--   0 dan        (501) staff       (20)     1273 2022-11-01 16:11:00.000000 hdl21-5.0.0/hdl21/noconn.py
--rw-r--r--   0 dan        (501) staff       (20)      191 2023-01-09 00:49:23.000000 hdl21-5.0.0/hdl21/one_or_more.py
--rw-r--r--   0 dan        (501) staff       (20)    12472 2023-10-25 18:18:42.000000 hdl21-5.0.0/hdl21/params.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.341562 hdl21-5.0.0/hdl21/pdk/
--rw-r--r--   0 dan        (501) staff       (20)       83 2023-06-09 23:37:53.000000 hdl21-5.0.0/hdl21/pdk/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     1648 2023-09-05 17:20:37.000000 hdl21-5.0.0/hdl21/pdk/corner.py
--rw-r--r--   0 dan        (501) staff       (20)     3225 2023-10-11 16:45:30.000000 hdl21-5.0.0/hdl21/pdk/installation.py
--rw-r--r--   0 dan        (501) staff       (20)     6198 2023-09-05 17:20:37.000000 hdl21-5.0.0/hdl21/pdk/pdk.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.341965 hdl21-5.0.0/hdl21/pdk/sample_pdk/
--rw-r--r--   0 dan        (501) staff       (20)      861 2022-12-15 00:46:13.000000 hdl21-5.0.0/hdl21/pdk/sample_pdk/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     5253 2023-09-05 17:20:37.000000 hdl21-5.0.0/hdl21/pdk/sample_pdk/pdk.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.342103 hdl21-5.0.0/hdl21/pdk/sample_pdk/resources/
--rw-r--r--   0 dan        (501) staff       (20)      639 2023-06-23 19:51:39.000000 hdl21-5.0.0/hdl21/pdk/sample_pdk/resources/models.sp
--rw-r--r--   0 dan        (501) staff       (20)     1470 2022-12-15 00:46:13.000000 hdl21-5.0.0/hdl21/pdk/sample_pdk/test_sample_pdk.py
--rw-r--r--   0 dan        (501) staff       (20)      703 2022-08-12 23:32:38.000000 hdl21-5.0.0/hdl21/pdk/test_pdk.py
--rw-r--r--   0 dan        (501) staff       (20)     1331 2023-10-25 18:18:42.000000 hdl21-5.0.0/hdl21/portref.py
--rw-r--r--   0 dan        (501) staff       (20)    18789 2023-10-25 18:18:42.000000 hdl21-5.0.0/hdl21/prefix.py
--rw-r--r--   0 dan        (501) staff       (20)    23649 2023-10-25 18:18:42.000000 hdl21-5.0.0/hdl21/primitives.py
--rw-r--r--   0 dan        (501) staff       (20)     2300 2023-03-17 23:05:04.000000 hdl21-5.0.0/hdl21/props.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.342533 hdl21-5.0.0/hdl21/proto/
--rw-r--r--   0 dan        (501) staff       (20)      197 2023-08-15 21:10:54.000000 hdl21-5.0.0/hdl21/proto/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    18211 2023-10-25 18:18:42.000000 hdl21-5.0.0/hdl21/proto/exporting.py
--rw-r--r--   0 dan        (501) staff       (20)    15400 2023-10-17 23:20:13.000000 hdl21-5.0.0/hdl21/proto/importing.py
--rw-r--r--   0 dan        (501) staff       (20)     1724 2023-09-05 17:20:37.000000 hdl21-5.0.0/hdl21/qualname.py
--rw-r--r--   0 dan        (501) staff       (20)     2442 2023-07-11 16:27:41.000000 hdl21-5.0.0/hdl21/role.py
--rw-r--r--   0 dan        (501) staff       (20)     4042 2023-09-05 17:20:37.000000 hdl21-5.0.0/hdl21/scalar.py
--rw-r--r--   0 dan        (501) staff       (20)     9569 2023-10-11 16:45:30.000000 hdl21-5.0.0/hdl21/signal.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.343464 hdl21-5.0.0/hdl21/sim/
--rw-r--r--   0 dan        (501) staff       (20)       90 2023-08-25 22:51:16.000000 hdl21-5.0.0/hdl21/sim/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    14308 2023-11-14 18:28:27.000000 hdl21-5.0.0/hdl21/sim/data.py
--rw-r--r--   0 dan        (501) staff       (20)     8328 2022-10-17 22:32:24.000000 hdl21-5.0.0/hdl21/sim/delay.py
--rw-r--r--   0 dan        (501) staff       (20)    13662 2023-08-25 22:51:16.000000 hdl21-5.0.0/hdl21/sim/proto.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.343819 hdl21-5.0.0/hdl21/sim/tests/
--rw-r--r--   0 dan        (501) staff       (20)     9850 2023-06-26 21:03:45.000000 hdl21-5.0.0/hdl21/sim/tests/test_sim.py
--rw-r--r--   0 dan        (501) staff       (20)     5378 2023-10-25 18:18:42.000000 hdl21-5.0.0/hdl21/slice.py
--rw-r--r--   0 dan        (501) staff       (20)     2123 2023-01-09 00:49:33.000000 hdl21-5.0.0/hdl21/sliceable.py
--rw-r--r--   0 dan        (501) staff       (20)     3957 2023-10-25 18:18:42.000000 hdl21-5.0.0/hdl21/source_info.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.345716 hdl21-5.0.0/hdl21/tests/
--rw-r--r--   0 dan        (501) staff       (20)        0 2021-04-16 16:15:12.000000 hdl21-5.0.0/hdl21/tests/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     1091 2022-11-26 00:08:30.000000 hdl21-5.0.0/hdl21/tests/content.py
--rw-r--r--   0 dan        (501) staff       (20)     1733 2023-10-25 18:18:42.000000 hdl21-5.0.0/hdl21/tests/test_builtin_generators.py
--rw-r--r--   0 dan        (501) staff       (20)    23843 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/tests/test_bundles.py
--rw-r--r--   0 dan        (501) staff       (20)     5483 2023-10-24 23:26:54.000000 hdl21-5.0.0/hdl21/tests/test_conns.py
--rw-r--r--   0 dan        (501) staff       (20)     7395 2023-10-25 18:18:42.000000 hdl21-5.0.0/hdl21/tests/test_doc_examples.py
--rw-r--r--   0 dan        (501) staff       (20)    18297 2023-10-17 23:20:13.000000 hdl21-5.0.0/hdl21/tests/test_exports.py
--rw-r--r--   0 dan        (501) staff       (20)    45297 2023-11-14 18:31:59.000000 hdl21-5.0.0/hdl21/tests/test_hdl21.py
--rw-r--r--   0 dan        (501) staff       (20)     5267 2023-06-26 21:03:45.000000 hdl21-5.0.0/hdl21/tests/test_params.py
--rw-r--r--   0 dan        (501) staff       (20)    15814 2023-09-05 17:20:37.000000 hdl21-5.0.0/hdl21/tests/test_prefix.py
--rw-r--r--   0 dan        (501) staff       (20)      741 2022-10-17 20:35:07.000000 hdl21-5.0.0/hdl21/tests/test_source_info.py
--rw-r--r--   0 dan        (501) staff       (20)      372 2023-03-17 23:05:04.000000 hdl21-5.0.0/hdl21/visibility.py
--rw-r--r--   0 dan        (501) staff       (20)     3739 2023-10-17 23:20:13.000000 hdl21-5.0.0/hdl21/walker.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.337728 hdl21-5.0.0/hdl21.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)    58141 2023-11-14 18:40:10.000000 hdl21-5.0.0/hdl21.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     2573 2023-11-14 18:40:10.000000 hdl21-5.0.0/hdl21.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-11-14 18:40:10.000000 hdl21-5.0.0/hdl21.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)      133 2023-11-14 18:40:10.000000 hdl21-5.0.0/hdl21.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       15 2023-11-14 18:40:10.000000 hdl21-5.0.0/hdl21.egg-info/top_level.txt
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.346003 hdl21-5.0.0/pdks/
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.346288 hdl21-5.0.0/pdks/Asap7/
--rw-r--r--   0 dan        (501) staff       (20)        0 2022-05-03 17:59:57.000000 hdl21-5.0.0/pdks/Asap7/readme.md
--rw-r--r--   0 dan        (501) staff       (20)      888 2023-11-14 18:31:59.000000 hdl21-5.0.0/pdks/Asap7/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.346632 hdl21-5.0.0/pdks/Sky130/
--rw-r--r--   0 dan        (501) staff       (20)    20435 2023-09-05 17:20:37.000000 hdl21-5.0.0/pdks/Sky130/readme.md
--rw-r--r--   0 dan        (501) staff       (20)      912 2023-11-14 18:31:59.000000 hdl21-5.0.0/pdks/Sky130/setup.py
--rw-r--r--   0 dan        (501) staff       (20)      643 2023-07-11 14:50:48.000000 hdl21-5.0.0/pdks/readme.md
--rw-r--r--   0 dan        (501) staff       (20)    57841 2023-09-05 17:20:37.000000 hdl21-5.0.0/readme.md
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.346800 hdl21-5.0.0/scratch/
--rw-r--r--   0 dan        (501) staff       (20)        0 2021-09-08 00:13:15.000000 hdl21-5.0.0/scratch/empty
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:10.347207 hdl21-5.0.0/scripts/
--rwxr-xr-x   0 dan        (501) staff       (20)      279 2023-06-07 23:06:22.000000 hdl21-5.0.0/scripts/install-dev.sh
--rwxr-xr-x   0 dan        (501) staff       (20)      160 2023-06-07 23:06:22.000000 hdl21-5.0.0/scripts/install-pypi.sh
--rw-r--r--   0 dan        (501) staff       (20)     2350 2023-03-17 23:05:04.000000 hdl21-5.0.0/scripts/primtable.py
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-11-14 18:40:10.347767 hdl21-5.0.0/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)     1393 2023-11-14 18:31:59.000000 hdl21-5.0.0/setup.py
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

### Comparing `hdl21-5.0.0/LICENSE` & `hdl21-6.0.0rc0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2021, Dan Fritchman
+Copyright (c) 2021-24, Dan Fritchman
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `hdl21-5.0.0/PKG-INFO` & `hdl21-6.0.0rc0/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: hdl21
-Version: 5.0.0
-Summary: Hardware Description Library
-Home-page: https://github.com/dan-fritchman/Hdl21
-Author: Dan Fritchman
-Author-email: dan@fritch.mn
-Requires-Python: >=3.7, <3.12
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # HDL21
 
 ## Analog Hardware Description Library in Python
 
 [![pypi](https://img.shields.io/badge/pypi-hdl21-blue)](https://pypi.org/project/hdl21/)
 [![python-versions](https://img.shields.io/badge/python-3.7_3.8_3.9_3.10_3.11-blue)](https://codecov.io/gh/dan-fritchman/Hdl21)
 [![test](https://github.com/dan-fritchman/Hdl21/actions/workflows/test.yaml/badge.svg)](https://github.com/dan-fritchman/Hdl21/actions/workflows/test.yaml)
@@ -1280,16 +1268,14 @@
 - Clone this repository & navigate to it.
 - `bash scripts/install-dev.sh`. See the note below.
 - `pytest -s` should yield something like:
 
 ```
 $ pytest -s
 ============================ test session starts =============================
-platform darwin -- Python 3.10.0, pytest-7.1.2, pluggy-1.0.0
-plugins: anyio-3.5.0, cov-3.0.0
 collected 126 items
 
 hdl21/pdk/test_pdk.py ...
 hdl21/pdk/sample_pdk/test_sample_pdk.py ...
 hdl21/sim/tests/test_sim.py .........s
 hdl21/tests/test_builtin_generators.py ..
 hdl21/tests/test_bundles.py ............
```

### Comparing `hdl21-5.0.0/hdl21/__init__.py` & `hdl21-6.0.0rc0/hdl21/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ 
 # Hdl21 Hardware Description Library 
 """
 
-__version__ = "5.0.0"  # NOTE: VLSIR_VERSION
+__version__ = "6.0.0rc0"  # VLSIR_VERSION
 
 # Internal (python) module aliases, overridden by names such as the `module` decorator function.
 from . import module as _module_module
 from . import bundle as _bundle_module
 from . import external_module as _external_module_module
 from . import instance as _instance_module
 from . import generator as _generator_module
```

### Comparing `hdl21-5.0.0/hdl21/attrmagic.py` & `hdl21-6.0.0rc0/hdl21/attrmagic.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/bundle.py` & `hdl21-6.0.0rc0/hdl21/bundle.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/call.py` & `hdl21-6.0.0rc0/hdl21/call.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/concat.py` & `hdl21-6.0.0rc0/hdl21/concat.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/concatable.py` & `hdl21-6.0.0rc0/hdl21/concatable.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/connect.py` & `hdl21-6.0.0rc0/hdl21/connect.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/datatype.py` & `hdl21-6.0.0rc0/hdl21/datatype.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,23 +23,61 @@
   - Importing this function into other packages is therefore highly discouraged. (Copying it is quite easy though.) 
 - `@datatype` only works on modules which are imported before `_update_forward_refs()` is run. 
   - Generally this means modules which are imported as part of `__init__.py`
 - `@datatype` is designed solely to work on `pydantic.dataclasses.dataclass`es. 
   - Notable exceptions include *union types* thereof, which do not have the necessary fields/ methods. 
 """
 
-from pydantic import Extra
-from pydantic.dataclasses import dataclass
 from typing import TypeVar, Type, Optional
+from pydantic import __version__ as _pydantic_version
+
 
+_pydantic_major_version = int(_pydantic_version.split(".")[0])
+if _pydantic_major_version > 2 or _pydantic_major_version < 1:
+    msg = "Error reading Pydantic version. Should be either 1.x or 2.x."
+    raise ImportError(msg)
+
+if _pydantic_major_version == 1:
+    from pydantic import Extra, BaseModel
+    from pydantic.json import pydantic_encoder as pydantic_json_encoder
+
+    PYDANTIC_V2 = False
+
+    class OurBaseConfig:
+        allow_extra = Extra.forbid
+
+    class AllowArbConfig(OurBaseConfig):
+        arbitrary_types_allowed = True
+
+    def _update_forward_refs():
+        """Update all the forward type-references"""
+        for tp in datatypes:
+            tp.__pydantic_model__.update_forward_refs()
+
+else:  # _pydantic_major_version==2
+    from pydantic import Extra, BaseModel, RootModel, BeforeValidator
+    from pydantic.deprecated.json import pydantic_encoder as pydantic_json_encoder
+
+    PYDANTIC_V2 = True
+    OurBaseConfig = dict(allow_extra="forbid", validate_default=True)
+    AllowArbConfig = dict(
+        allow_extra="forbid", validate_default=True, arbitrary_types_allowed=True
+    )
+
+    def _update_forward_refs():
+        """Update all the forward type-references"""
+        ...
+        # for tp in datatypes:
+        #     tp.model_rebuild()
 
-# The list of defined datatypes
-datatypes = []
+
+from pydantic.dataclasses import dataclass
 
 T = TypeVar("T")
+datatypes = []  # The list of defined datatypes
 
 
 def _datatype(cls: Type[T], *, config: Optional[Type] = None, **kwargs) -> Type[T]:
     """# Inner implementation of `@datatype`"""
 
     # Get the default `Config` if none is provided
     config = config or OurBaseConfig
@@ -59,26 +97,7 @@
     # `Union[Type[T], Callable[[Type[T]], Type[T]]`
     # But do ya really want that, or just to know it works as a decorator.
 
     inner = lambda c: _datatype(c, **kwargs)
     if cls is None:
         return inner  # Called with parens, e.g. `@datatype()`
     return inner(cls)  # Called without parens
-
-
-def _update_forward_refs():
-    """Update all the forward type-references"""
-    for tp in datatypes:
-        tp.__pydantic_model__.update_forward_refs()
-
-
-"""
-# Define a few common pydantic model `Config`s
-"""
-
-
-class OurBaseConfig:
-    allow_extra = Extra.forbid
-
-
-class AllowArbConfig(OurBaseConfig):
-    arbitrary_types_allowed = True
```

### Comparing `hdl21-5.0.0/hdl21/default.py` & `hdl21-6.0.0rc0/hdl21/default.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/diff_pair.py` & `hdl21-6.0.0rc0/hdl21/diff_pair.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/elab/default.py` & `hdl21-6.0.0rc0/hdl21/elab/default.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/elab/elab.py` & `hdl21-6.0.0rc0/hdl21/elab/elab.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/elab/elaboratable.py` & `hdl21-6.0.0rc0/hdl21/elab/elaboratable.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/elab/helpers/resolve_ref_types.py` & `hdl21-6.0.0rc0/hdl21/elab/helpers/resolve_ref_types.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/elab/helpers/width.py` & `hdl21-6.0.0rc0/hdl21/elab/helpers/width.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/elab/passes/__init__.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/elab/passes/arrays.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/arrays.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/elab/passes/base.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/base.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/elab/passes/conntypes.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/conntypes.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/elab/passes/flatten_bundles.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/flatten_bundles.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,14 @@
             path_from_self = path_suffix.prepend(name)
             if path_from_self in self.signals:
                 msg = f"Error Flattening Bundles: colliding flattened Signal names for {sig} and {self.signals[path_from_self]}"
                 raise RuntimeError(msg)
             self.signals[path_from_self] = sig
 
 
-BundleScope.__pydantic_model__.update_forward_refs()
-
-
 @datatype(config=AllowArbConfig)
 class BundlePortEntry:
     """# Bundle-Port Entry in the Cache
     Hashable combination of a Module and a portname."""
 
     module: Module
     portname: str
```

### Comparing `hdl21-5.0.0/hdl21/elab/passes/inst_bundles.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/inst_bundles.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/elab/passes/mark_modules.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/mark_modules.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/elab/passes/orphanage.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/orphanage.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/elab/passes/portrefs.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/portrefs.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/elab/passes/slices.py` & `hdl21-6.0.0rc0/hdl21/elab/passes/slices.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/external_module.py` & `hdl21-6.0.0rc0/hdl21/external_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,26 +50,27 @@
 
     @property
     def Params(self) -> Type:
         """Type-style alias for the parameter-type."""
         return self.paramtype
 
     def __post_init__(self):
+        """Post-Constructor Checks"""
+
         # Check for a valid parameter-type
         if not isparamclass(self.paramtype) and self.paramtype not in (dict, Dict):
             msg = f"Invalid parameter type {self.paramtype} for {self}. "
             msg += "Param types must be either `@paramclass`es or `dict`."
             raise ValueError(msg)
 
         # Internal tracking data: defining module/import-path
         self._source_info: Optional[SourceInfo] = source_info(get_pymodule=True)
         self._importpath = None
 
-    def __post_init_post_parse__(self):
-        """After type-checking, do some more checks on values"""
+        # Now do some more checks on values
         for p in self.port_list:
             if not p.name:
                 raise ValueError(f"Unnamed Primitive Port {p} for {self.name}")
             if p.vis != Visibility.PORT:
                 msg = f"Invalid Primitive Port {p.name} on {self.name}; must have PORT visibility"
                 raise ValueError(msg)
 
@@ -95,15 +96,15 @@
     """# External Module Call
     A combination of an `ExternalModule` and its Parameter-values, typically generated by calling the `ExternalModule`.
     """
 
     module: ExternalModule
     params: Any
 
-    def __post_init_post_parse__(self):
+    def __post_init__(self):
         # Type-validate our parameters
         if not isinstance(self.params, self.module.paramtype):
             msg = f"Invalid parameter type {type(self.params)} for ExternalModule {self.module.name}. Must be {self.module.paramtype}"
             raise TypeError(msg)
 
     @property
     def name(self) -> str:
```

### Comparing `hdl21-5.0.0/hdl21/generator.py` & `hdl21-6.0.0rc0/hdl21/generator.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/generators.py` & `hdl21-6.0.0rc0/hdl21/generators.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/instance.py` & `hdl21-6.0.0rc0/hdl21/instance.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/instantiable.py` & `hdl21-6.0.0rc0/hdl21/instantiable.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,29 @@
 """
 Type-alias for `Instantiable` hdl21 types. Each is valid as the `of` field of `hdl21.Instance`s, 
 and thus supports its "connect by call" and "connect by assignment" semantics. 
 """
 
-import copy
+# Std-Lib Imports
+from __future__ import annotations
 from typing import Any, Union, Dict
+import copy
 
-from pydantic import BaseModel
-
-from .datatype import AllowArbConfig
+# Local Imports
+from .datatype import AllowArbConfig, _pydantic_major_version
 from .module import Module
 from .primitives import PrimitiveCall
 from .external_module import ExternalModuleCall
 
 
 # Instantiable types-union
 InstantiableUnion = Union[Module, ExternalModuleCall, PrimitiveCall]
 
 
-class Instantiable(BaseModel):
-    """
-    # Instantiable
-
-    Generally this means
-    ````python
-    Union[Module, ExternalModuleCall, PrimitiveCall]
-    ```
-    with some customized checking and error handling.
-    """
-
-    __root__: InstantiableUnion
-    Config = AllowArbConfig
-
-    def __init__(self, *_, **__):
-        # Brick any attempts to create instances
-        msg = f"Invalid attempt to instantiate an `Instantiable` directly. "
-        raise RuntimeError(msg)
-
-    @classmethod
-    def __get_validators__(cls):
-        yield assert_instantiable
-
-
-def assert_instantiable(i: Any) -> Instantiable:
+def assert_instantiable(i: Any) -> "Instantiable":
     """# Assert that `i` is an `Instantiable` type."""
     if not is_instantiable(i):
         return invalid(i)
     return i
 
 
 def is_instantiable(val: Any) -> bool:
@@ -70,15 +47,15 @@
     elif isinstance(val, _Instance):
         msg += f"Did you mean to use its target module `{val.of}` instead?"
     else:  # Generic message for everything else
         msg += f"Valid `Instantiable` types include: {list(InstantiableUnion.__args__)}"
     raise TypeError(msg)
 
 
-def qualname(i: Instantiable) -> str:
+def qualname(i: "Instantiable") -> str:
     """Path-qualified name of Instantiable `i`"""
     from .qualname import qualname as module_qualname
 
     if isinstance(i, PrimitiveCall):
         # These have no "qualification" paths, just a singular name.
         return i.name
 
@@ -87,20 +64,57 @@
         return module_qualname(i)
     if isinstance(i, ExternalModuleCall):
         return module_qualname(i.module)
 
     raise TypeError(f"Invalid Instantiable {i}")
 
 
-def io(i: Instantiable) -> Dict[str, "Connectable"]:
+def io(i: "Instantiable") -> Dict[str, "Connectable"]:
     """
     Get a complete dictionary of IO ports for `i`, including all types: Signals and Bundles.
     Copies the Instantiable's top-level dictionary so that it is not modified by consumers.
     """
 
     rv = copy.copy(i.ports)
     if hasattr(i, "bundle_ports"):
         rv.update(copy.copy(i.bundle_ports))
     return rv
 
 
+_doc = """
+# Instantiable
+
+Generally this means
+````python
+Union[Module, ExternalModuleCall, PrimitiveCall]
+```
+with some customized checking and error handling.
+"""
+
+if _pydantic_major_version == 1:
+    from .datatype import BaseModel
+
+    class Instantiable(BaseModel):
+        # "Custom root types" implementation
+
+        __doc__ = _doc
+        __root__: InstantiableUnion
+        Config = AllowArbConfig
+
+        def __init__(self, *_, **__):
+            # Brick any attempts to create instances
+            msg = f"Invalid attempt to instantiate an `Instantiable` directly. "
+            raise RuntimeError(msg)
+
+        @classmethod
+        def __get_validators__(cls):
+            yield assert_instantiable
+
+else:
+    from .datatype import BeforeValidator
+    from typing import Annotated
+
+    Instantiable = Annotated[InstantiableUnion, BeforeValidator(assert_instantiable)]
+    Instantiable.__doc__ = _doc
+
+
 __all__ = ["Instantiable", "is_instantiable"]
```

### Comparing `hdl21-5.0.0/hdl21/module.py` & `hdl21-6.0.0rc0/hdl21/module.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/netlisting.py` & `hdl21-6.0.0rc0/hdl21/netlisting.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from typing import IO, Union, Optional
 
 # Import the core netlisting from `vlsirtools`
 import vlsir
 from vlsirtools.netlist import (
-    netlist as vlisr_netlist,
+    netlist as vlsir_netlist,
     NetlistFormat,
     NetlistFormatSpec,
     NetlistOptions,
 )
 
 from .elab import Elaboratables
 from .proto import to_proto
@@ -47,11 +47,11 @@
     # Convert to the Vlsir `Package` if necessary
     if not isinstance(src, vlsir.circuit.Package):
         pkg = to_proto(top=src, domain=domain)
     else:
         pkg = src
 
     # And invoke the VLSIR netlister
-    return vlisr_netlist(pkg=pkg, dest=dest, **kwargs)
+    return vlsir_netlist(pkg=pkg, dest=dest, **kwargs)
 
 
 __all__ = ["netlist", "NetlistFormat", "NetlistFormatSpec", "NetlistOptions"]
```

### Comparing `hdl21-5.0.0/hdl21/noconn.py` & `hdl21-6.0.0rc0/hdl21/noconn.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     An optional `name` field allows guidance for external netlisting,
     for cases in which consistent naming is desirable (e.g. for waveform probing).
     """
 
     name: Optional[str] = None
 
-    def __post_init_post_parse__(self) -> None:
+    def __post_init__(self) -> None:
         # Internal management data
         # Connected port references
         self._connected_ports: Set[PortRef] = set()
 
     def __eq__(self, other: "NoConn") -> bool:
         """`NoConn`s are "equal" only if identical objects."""
         return self is other
```

### Comparing `hdl21-5.0.0/hdl21/params.py` & `hdl21-6.0.0rc0/hdl21/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Optional, Any, Type, TypeVar, Dict
 
 # PyPi Imports
 import pydantic
 
 # Local Imports
 from .default import Default
-from .datatype import AllowArbConfig
+from .datatype import AllowArbConfig, pydantic_json_encoder
 
 T = TypeVar("T")
 
 
 def paramclass(cls: Type[T]) -> Type[T]:
     """# Parameter-Class Creation Decorator
 
@@ -289,15 +289,15 @@
     # Dataclasses also require custom handling, as the default encoder deep-copies them,
     # often invoking methods not supported on several Hdl21 types.
     # Convert to (shallow) dictionaries instead.
     if dataclasses.is_dataclass(obj):
         return {f.name: getattr(obj, f.name) for f in dataclasses.fields(obj)}
 
     # Not an Hdl21 type. Hand off to pydantic.
-    return pydantic.json.pydantic_encoder(obj)
+    return pydantic_json_encoder(obj)
 
 
 # Shortcut for parameter-less generators.
 # Defines the empty-value `@paramclass`.
 @paramclass
 class HasNoParams:
     """# HasNoParams
```

### Comparing `hdl21-5.0.0/hdl21/pdk/corner.py` & `hdl21-6.0.0rc0/hdl21/pdk/corner.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/pdk/installation.py` & `hdl21-6.0.0rc0/hdl21/pdk/installation.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/pdk/pdk.py` & `hdl21-6.0.0rc0/hdl21/pdk/pdk.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/pdk/sample_pdk/__init__.py` & `hdl21-6.0.0rc0/hdl21/pdk/sample_pdk/__init__.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/pdk/sample_pdk/pdk.py` & `hdl21-6.0.0rc0/hdl21/pdk/sample_pdk/pdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     """Sample PDK MOS Transistor Parameters"""
 
     w = h.Param(dtype=h.Scalar, desc="Width in resolution units", default=1 * µ)
     l = h.Param(dtype=h.Scalar, desc="Length in resolution units", default=1 * µ)
     nf = h.Param(dtype=h.Scalar, desc="Number of parallel fingers", default=1)
     m = h.Param(dtype=h.Scalar, desc="Number of parallel fingers", default=1)
 
-    def __post_init_post_parse__(self):
+    def __post_init__(self):
         """Value Checks"""
         if self.w <= 0:
             raise ValueError(f"MosParams with invalid width {self.w}")
         if self.l <= 0:
             raise ValueError(f"MosParams with invalid length {self.l}")
         if self.nf <= 0:
             msg = f"MosParams with invalid number parallel fingers {self.nf}"
```

### Comparing `hdl21-5.0.0/hdl21/pdk/sample_pdk/resources/models.sp` & `hdl21-6.0.0rc0/hdl21/pdk/sample_pdk/resources/models.sp`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/pdk/sample_pdk/test_sample_pdk.py` & `hdl21-6.0.0rc0/hdl21/pdk/sample_pdk/test_sample_pdk.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/pdk/test_pdk.py` & `hdl21-6.0.0rc0/hdl21/pdk/test_pdk.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/portref.py` & `hdl21-6.0.0rc0/hdl21/portref.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Created from a combination of a parent `Instance` and a port-name.
     """
 
     # Core fields: the Instance and port name
     inst: _Instance
     portname: str
 
-    def __post_init_post_parse__(self):
+    def __post_init__(self):
         # Inner management data
         self._connected_ports: Set[PortRef] = set()
         self.resolved: Union[None, "Signal", "BundleInstance"] = None
         self._slices: Set["Slice"] = set()
         self._concats: Set["Concat"] = set()
         self._width: Optional[int] = None
```

### Comparing `hdl21-5.0.0/hdl21/prefix.py` & `hdl21-6.0.0rc0/hdl21/prefix.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,25 +179,28 @@
     @classmethod
     def new(cls, number: Decimal, prefix: Prefix = Prefix.UNIT) -> "Prefixed":
         """Create a new Prefixed number.
         Alias for `Prefixed(number=number, prefix=prefix), and a (slight) shorthand
         for using arguments by-position, which `pydantic.BaseModel` does not support."""
         return cls(number=number, prefix=prefix)
 
-    @classmethod
-    def validate(cls, v: Union["Prefixed", "ToPrefixed"]) -> "Prefixed":
-        """Validate `v` as a `Prefixed` number, or convert to `Prefixed` if applicable.
-        While usable elsewhere, `validate` is primarily intended for use in type-validated
-        dataclass trees, such as those generated in `paramclass`es."""
-
-        return to_prefixed(v)
-
-    @classmethod
-    def __get_validators__(cls):
-        yield cls.validate
+    #
+    # FIXME: pending potential deprecation #157
+    #
+    # @classmethod
+    # def validate(cls, v: Union["Prefixed", "ToPrefixed"]) -> "Prefixed":
+    #     """Validate `v` as a `Prefixed` number, or convert to `Prefixed` if applicable.
+    #     While usable elsewhere, `validate` is primarily intended for use in type-validated
+    #     dataclass trees, such as those generated in `paramclass`es."""
+    #
+    #     return to_prefixed(v)
+    #
+    # @classmethod
+    # def __get_validators__(cls):
+    #     yield cls.validate
 
     def __hash__(self):
         return hash((self.number, self.prefix))
 
     def __int__(self) -> int:
         return int(self.number) * 10**self.prefix.value
 
@@ -331,15 +334,15 @@
         return round(lhs.number, EPSILON) >= round(rhs.number, EPSILON)
 
 
 # Union of the types which can be converted to `Prefixed`
 ToPrefixed = Union[int, float, str, Decimal]
 
 
-def to_prefixed(v: Union[Prefixed, "ToPrefixed"]) -> Prefixed:
+def to_prefixed(v: Union[Prefixed, ToPrefixed]) -> Prefixed:
     """Convert any convertible type to a `Prefixed` number."""
 
     if isinstance(v, Prefixed):
         return v  # Valid as-is, return it.
     if isinstance(v, Decimal):
         return Prefixed(number=v)  # Also pretty much done
     # Convert the remaining convertible types to `Decimal` inline
```

### Comparing `hdl21-5.0.0/hdl21/primitives.py` & `hdl21-6.0.0rc0/hdl21/primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
     name: str  # Primitive Name
     desc: str  # String Description
     port_list: List[Signal]  # Ordered Port List
     paramtype: Type[object]  # Class/ Type of valid Parameters
     primtype: PrimitiveType  # Ideal vs Physical Primitive-Type
 
-    def __post_init_post_parse__(self):
+    def __post_init__(self):
         """After type-checking, do plenty more checks on values"""
         if not isparamclass(self.paramtype):
             msg = f"Invalid Primitive param-type {self.paramtype} for {self.name}, must be an `hdl21.paramclass`"
             raise TypeError(msg)
         for p in self.port_list:
             if not p.name:
                 raise ValueError(f"Unnamed Primitive Port {p} for {self.name}")
@@ -139,15 +139,15 @@
     """Primitive Call
     A combination of a Primitive and its Parameter-values,
     typically generated by calling the Primitive."""
 
     prim: Primitive
     params: Any = NoParams
 
-    def __post_init_post_parse__(self):
+    def __post_init__(self):
         # Type-validate our parameters
         if not isinstance(self.params, self.prim.paramtype):
             msg = f"Invalid parameters {self.params} for Primitive {self.prim}. Must be {self.prim.paramtype}"
             raise TypeError(msg)
 
     @property
     def name(self) -> str:
@@ -183,15 +183,16 @@
 # Stores aliases on the side.
 _primitives: Dict[str, PrimLibEntry] = dict()
 
 
 def _add(prim: Primitive, aliases: List[str]) -> Primitive:
     """Add a primitive to this library.
     Ensures its identifier matches its `name` field, and adds any aliases to the global namespace.
-    This is a private function and should be used solely during `hdl21.primitives` import-time."""
+    This is a private function and should be used solely during `hdl21.primitives` import-time.
+    """
     global _primitives
 
     if prim.name in _primitives or prim.name in globals():
         raise ValueError(f"Duplicate primitive name {prim.name}")
 
     # Add the combination as a new entry
     entry = PrimLibEntry(prim, aliases)
@@ -251,15 +252,15 @@
     mult = Param(dtype=Optional[Scalar], desc="Multiplier", default=None)
 
     tp = Param(dtype=MosType, desc="MosType (Nmos/ Pmos)", default=MosType.NMOS)
     vth = Param(dtype=MosVth, desc="Threshold voltage specifier", default=MosVth.STD)
     family = Param(dtype=MosFamily, desc="Device family", default=MosFamily.NONE)
     model = Param(dtype=Optional[str], desc="Model (Name)", default=None)
 
-    # def __post_init_post_parse__(self):
+    # def __post_init__(self):
     #     """Value Checks"""
     #     # FIXME: re-introduce these, for the case in which the parameters are `Prefixed` and not `Literal` values.
     #     if self.w <= 0:
     #         raise ValueError(f"MosParams with invalid width {self.w}")
     #     if self.l <= 0:
     #         raise ValueError(f"MosParams with invalid length {self.l}")
     #     if self.nf <= 0:
@@ -374,17 +375,17 @@
     ),
     aliases=["C", "Cap", "Capacitor", "IdealC", "IdealCap"],
 )
 
 
 @paramclass
 class PhysicalCapacitorParams:
-    c = Param(dtype=Scalar, desc="Capacitance (F)", default=None)
-    w = Param(dtype=Scalar, desc="Width in resolution units", default=None)
-    l = Param(dtype=Scalar, desc="Length in resolution units", default=None)
+    w = Param(dtype=Optional[Scalar], desc="Width in resolution units", default=None)
+    l = Param(dtype=Optional[Scalar], desc="Length in resolution units", default=None)
+    c = Param(dtype=Optional[Scalar], desc="Capacitance (F)", default=None)
     model = Param(dtype=Optional[str], desc="Model (Name)", default=None)
     mult = Param(dtype=Optional[str], desc="Multiplier", default=None)
 
 
 PhysicalCapacitor = _add(
     prim=Primitive(
         name="PhysicalCapacitor",
@@ -650,15 +651,15 @@
     l = Param(dtype=Optional[Scalar], desc="Length in resolution units", default=None)
     tp = Param(
         dtype=BipolarType, desc="Bipolar Type (NPN/ PNP)", default=BipolarType.NPN
     )
     model = Param(dtype=Optional[str], desc="Model (Name)", default=None)
     mult = Param(dtype=Optional[Scalar], desc="Multiplier", default=None)
 
-    def __post_init_post_parse__(self):
+    def __post_init__(self):
         """Value Checks"""
         if self.w is not None and self.w <= 0:
             raise ValueError(f"BipolarParams with invalid width {self.w}")
         if self.l is not None and self.l <= 0:
             raise ValueError(f"BipolarParams with invalid length {self.l}")
```

### Comparing `hdl21-5.0.0/hdl21/props.py` & `hdl21-6.0.0rc0/hdl21/props.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/proto/exporting.py` & `hdl21-6.0.0rc0/hdl21/proto/exporting.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,17 +369,14 @@
     # Enum-valued parameters must also be strings, or fail
     if isinstance(val, Enum):
         if not isinstance(val.value, str):
             raise TypeError(f"Enum-valued parameters must be strings, not {val.value}")
         return vlsir.ParamValue(literal=val.value)
 
     # Internal numeric (and number-like) types
-    if isinstance(val, Scalar):
-        # `Scalar` will either have an internal `Literal` or `Prefixed` value.
-        val = val.inner
     if isinstance(val, Literal):  # String/ expression literals
         return vlsir.ParamValue(literal=val.text)
     if isinstance(val, Prefixed):
         return vlsir.ParamValue(prefixed=export_prefixed(val))
 
     # Standard-Lib Numbers
     if isinstance(val, Decimal):
```

### Comparing `hdl21-5.0.0/hdl21/proto/importing.py` & `hdl21-6.0.0rc0/hdl21/proto/importing.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/qualname.py` & `hdl21-6.0.0rc0/hdl21/qualname.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/role.py` & `hdl21-6.0.0rc0/hdl21/role.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/scalar.py` & `hdl21-6.0.0rc0/hdl21/scalar.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,96 +1,83 @@
+# Std-Lib Imports
+from __future__ import annotations
 from typing import Union
 from decimal import Decimal
-from pydantic import BaseModel
 
 # Local Imports
+from .datatype import _pydantic_major_version
 from .prefix import Prefixed
 from .literal import Literal
 
 
-# Union of types convertible into `Scalar`
-ToScalar = Union[Prefixed, Literal, str, int, float, Decimal]
-
-
-class Scalar(BaseModel):
-    """
-    # The `Scalar` parameter type
-
-    Generally this means
-    ```python
-    Union[Prefixed, Literal]
-    ```
-    with built-in automatic conversions from each of:
-    ```python
-    [str, int, float, Decimal]
-    ```
-    when used in `paramclass` definitions.
-
-    `Scalar` is particularly designed for parameter-values of `Primitive`s and of simulations.
-    Most such parameters "want" to be the `Prefixed` type, for reasons outlined in
-    https://github.com/dan-fritchman/Hdl21#prefixed-numeric-parameters.
-
-    They often also need a string-valued escape hatch, e.g. when referring to out-of-Hdl21 quantities
-    such as parameters in external netlists or simulation decks.
-    These out-of-Hdl21 expressions are represented by the `Literal` type, a simple wrapper around `str`.
-
-    Where possible `Scalar` prefers to use the `Prefixed` variant.
-    Strings and built-in numbers (int, float, Decimal) are converted to `Prefixed` inline by the `validate` method.
-    All of the `validate` mechanisms work for `Scalar`s used as fields in `pydantic.dataclasses`.
-    which crucially include all `hdl21.paramclass`es.
-
-    While defined as a type, `Scalar` is not instantiable.
-    It is really a class-based statement of `Union[Prefixed, Literal]`, with class methods to aid in validation.
-
-    If writing "primitive-like" parameters - e.g. those that go into SPICE simulations,
-    or are provided to PDK-level devices, it is very likely that you will want to:
-
-    * Use `Scalar` as a parameter type, i.e. the `dtype` field of `Param`s.
-    * Never actually instantiate a `Scalar` directly, including for its default value.
-
-    Example:
-
-    ```python
-    import hdl21 as h
-    from hdl21.prefix import NANO, µ
-    from decimal import Decimal
-
-    @h.paramclass
-    class MyMosParams:
-        w = h.Param(dtype=h.Scalar, desc="Width", default=1e-6) # Default `float` converts to a `Prefixed`
-        l = h.Param(dtype=h.Scalar, desc="Length", default="w/5") # Default `str` converts to a `Literal`
-
-    # Example instantiations
-    MyMosParams(w=Decimal(1e-6), l=3*µ)
-    MyMosParams(w=h.Literal("sim_param_width"), l=h.Prefixed.new(20, NANO))
-    MyMosParams(w="11*l", l=11)
-    ```
-    """
+# The shared docstring
+_doc = """
+# The `Scalar` parameter type
+
+Generally this means
+```python
+Union[Prefixed, Literal]
+```
+with built-in automatic conversions from each of:
+```python
+[str, int, float, Decimal]
+```
+when used in `paramclass` definitions.
+
+`Scalar` is particularly designed for parameter-values of `Primitive`s and of simulations.
+Most such parameters "want" to be the `Prefixed` type, for reasons outlined in
+https://github.com/dan-fritchman/Hdl21#prefixed-numeric-parameters.
+
+They often also need a string-valued escape hatch, e.g. when referring to out-of-Hdl21 quantities
+such as parameters in external netlists or simulation decks.
+These out-of-Hdl21 expressions are represented by the `Literal` type, a simple wrapper around `str`.
+
+Where possible `Scalar` prefers to use the `Prefixed` variant.
+Strings and built-in numbers (int, float, Decimal) are converted to `Prefixed` inline by the `validate` method.
+All of the `validate` mechanisms work for `Scalar`s used as fields in `pydantic.dataclasses`.
+which crucially include all `hdl21.paramclass`es.
+
+While defined as a type, `Scalar` is not instantiable.
+It is really a class-based statement of `Union[Prefixed, Literal]`, with class methods to aid in validation.
+
+If writing "primitive-like" parameters - e.g. those that go into SPICE simulations,
+or are provided to PDK-level devices, it is very likely that you will want to:
+
+* Use `Scalar` as a parameter type, i.e. the `dtype` field of `Param`s.
+* Never actually instantiate a `Scalar` directly, including for its default value.
+
+Example:
+
+```python
+import hdl21 as h
+from hdl21.prefix import NANO, µ
+from decimal import Decimal
 
-    # The Pydantic "custom root types" feature is really what makes this work:
-    # https://docs.pydantic.dev/latest/usage/models/#custom-root-types
+@h.paramclass
+class MyMosParams:
+w = h.Param(dtype=h.Scalar, desc="Width", default=1e-6) # Default `float` converts to a `Prefixed`
+l = h.Param(dtype=h.Scalar, desc="Length", default="w/5") # Default `str` converts to a `Literal`
+
+# Example instantiations
+MyMosParams(w=Decimal(1e-6), l=3*µ)
+MyMosParams(w=h.Literal("sim_param_width"), l=h.Prefixed.new(20, NANO))
+MyMosParams(w="11*l", l=11)
+```
+"""
 
-    __root__: Union[Prefixed, Literal]
 
-    def __init__(self, *_, **__):
-        # Brick any attempts to create instances
-        msg = f"Invalid attempt to instantiate a `Scalar` directly. "
-        msg += f"Create either of its variants `Prefixed` or `Literal` instead, "
-        msg += f"or use their built-in conversions from strings, ints, floats, and Decimals."
-        raise RuntimeError(msg)
-
-    @classmethod
-    def __get_validators__(cls):
-        yield to_scalar
+# Union of types convertible into `Scalar`
+ToScalar = Union[Prefixed, Literal, str, int, float, Decimal]
 
 
 def to_scalar(v: ToScalar) -> Union[Prefixed, Literal]:
     """# Validate and convert anything in the `ToScalar` set of types to a `Prefixed` or `Literal`.
     Most importantly this handles the case in which `v` is a *string*,
-    which attempts conversion to a `Prefixed`, and falls back to a `Literal` on failure."""
+    which attempts conversion to a `Prefixed`, and falls back to a `Literal` on failure.
+    """
 
     if isinstance(v, (Prefixed, Literal)):
         return v  # Valid as-is, return it.
 
     # Now the important case: strings
     if isinstance(v, str):
         try:  # Try to convert to a Prefixed, which internally converts to a Decimal
@@ -98,9 +85,39 @@
         except Exception:  # Catch all exceptions
             return Literal(text=v)
 
     # Everything else - notably including `int` and `float` - must be convertible to `Prefixed`, or fails in its validation.
     return Prefixed(number=v)
 
 
+if _pydantic_major_version == 1:
+    from .datatype import BaseModel
+
+    class Scalar(BaseModel):
+        # The Pydantic "custom root types" feature is really what makes this work:
+        # https://docs.pydantic.dev/latest/usage/models/#custom-root-types
+        __root__: Union[Prefixed, Literal]
+        __doc__ = _doc
+
+        def __init__(self, *_, **__):
+            # Brick any attempts to create instances
+            msg = f"Invalid attempt to instantiate a `Scalar` directly. "
+            msg += f"Create either of its variants `Prefixed` or `Literal` instead, "
+            msg += f"or use their built-in conversions from strings, ints, floats, and Decimals."
+            raise RuntimeError(msg)
+
+        @classmethod
+        def __get_validators__(cls):
+            yield to_scalar
+
+else:
+    from .datatype import BeforeValidator
+    from typing import Annotated
+
+    # Union of types convertible into `Scalar`
+    Scalar = Annotated[
+        Union[Prefixed, Literal],
+        BeforeValidator(to_scalar),
+    ]
+
 __all__ = ["Scalar", "ToScalar", "to_scalar"]
-__doc__ = Scalar.__doc__
+__doc__ = _doc
```

### Comparing `hdl21-5.0.0/hdl21/signal.py` & `hdl21-6.0.0rc0/hdl21/signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     related_clk: Optional["Signal"] = field(repr=False, default=None)
     # Related clock signal
     related_pwr: Optional["Signal"] = field(repr=False, default=None)
     # Related power signal
     related_gnd: Optional["Signal"] = field(repr=False, default=None)
     # Related ground signal
 
-    def __post_init_post_parse__(self):
+    def __post_init__(self):
         if self.width < 1:
             raise ValueError(f"Signal {self.name} width must be positive")
         self._parent_module: Optional["Module"] = None
         self._slices: Set["Slice"] = set()
         self._concats: Set["Concat"] = set()
         self._connected_ports: Set["PortRef"] = set()
```

### Comparing `hdl21-5.0.0/hdl21/sim/data.py` & `hdl21-6.0.0rc0/hdl21/sim/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,30 +203,30 @@
 
     @property
     def tp(self) -> AnalysisType:
         return AnalysisType.NOISE
 
 
 @simattr
-@datatype
+@datatype(config=AllowArbConfig)
 class SweepAnalysis:
     """Sweep over `inner` analyses"""
 
     inner: List["Analysis"]  # Inner Analyses
     var: Union[str, Param]  # Sweep variable, or its name
     sweep: Sweep  # Sweep Values
     name: Optional[str] = None  # Optional analysis name
 
     @property
     def tp(self) -> AnalysisType:
         return AnalysisType.SWEEP
 
 
 @simattr
-@datatype
+@datatype(config=AllowArbConfig)
 class MonteCarlo:
     """Add monte-carlo variations to one or more `inner` analyses."""
 
     inner: List["Analysis"]  # Inner Analyses
     npts: int  # Number of points
     name: Optional[str] = None  # Optional analysis name
 
@@ -281,15 +281,15 @@
     """Save Control-Element
     Adds content to the target simulation output"""
 
     targ: SaveTarget
 
 
 @simattr
-@datatype
+@datatype(config=AllowArbConfig)
 class Meas:
     """Measurement"""
 
     analysis: Union["Analysis", str]  # Target `Analysis`, or its type-name
     expr: str  # Measured expression. FIXME: just a string to be evaluated, no in-Python semantics
     name: Optional[str] = None  # Measurement name
```

### Comparing `hdl21-5.0.0/hdl21/sim/delay.py` & `hdl21-6.0.0rc0/hdl21/sim/delay.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/sim/proto.py` & `hdl21-6.0.0rc0/hdl21/sim/proto.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,12 +357,10 @@
 def export_float(num: Union[float, int, Decimal, Prefixed, Scalar]) -> float:
     """Export a `Number` union-type to a float, or protobuf float/double."""
     if num is None:
         # FIXME: this is the protobuf default, but we really wanna make fields that use it optional
         return 0.0
     if isinstance(num, float):
         return num
-    if isinstance(num, Scalar):
-        return float(num.inner)
     if isinstance(num, (int, str, Decimal, Prefixed)):
         return float(num)
     raise TypeError(f"Invalid value for proto float: {num}")
```

### Comparing `hdl21-5.0.0/hdl21/sim/tests/test_sim.py` & `hdl21-6.0.0rc0/hdl21/sim/tests/test_sim.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/slice.py` & `hdl21-6.0.0rc0/hdl21/slice.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     # Parent Connectable.
     # Really of union-type `Sliceable`, which is more painful to type-check statically,
     # although the constructor does it procedurally.
     parent: Any
     # Python index, i.e. that passed to square brackets
     index: Union[int, slice]
 
-    def __post_init_post_parse__(self):
+    def __post_init__(self):
         if not is_sliceable(self.parent):
             raise TypeError(f"{self.parent} is not Sliceable")
         self._connected_ports: Set["PortRef"] = set()
         self._inner: Optional[SliceInner] = None
         self._slices: WeakSet[Slice] = set()
         self._concats: WeakSet["Concat"] = set()
```

### Comparing `hdl21-5.0.0/hdl21/sliceable.py` & `hdl21-6.0.0rc0/hdl21/sliceable.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/source_info.py` & `hdl21-6.0.0rc0/hdl21/source_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,25 +22,19 @@
 
 """
 
 import inspect
 from pathlib import Path
 from types import ModuleType, FrameType
 from typing import Optional
-from pydantic import Extra
 
-from .datatype import datatype
+from .datatype import datatype, AllowArbConfig
 
 
-class Config:
-    arbitrary_types_allowed = True
-    allow_extra = Extra.forbid
-
-
-@datatype(config=Config)
+@datatype(config=AllowArbConfig)
 class SourceInfo:
     """# Python Source Info"""
 
     filepath: Path
     linenum: int
     pymodule: Optional[ModuleType] = None
```

### Comparing `hdl21-5.0.0/hdl21/tests/content.py` & `hdl21-6.0.0rc0/hdl21/tests/content.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/tests/test_builtin_generators.py` & `hdl21-6.0.0rc0/hdl21/tests/test_builtin_generators.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/tests/test_bundles.py` & `hdl21-6.0.0rc0/hdl21/tests/test_bundles.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/tests/test_conns.py` & `hdl21-6.0.0rc0/hdl21/tests/test_conns.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/tests/test_doc_examples.py` & `hdl21-6.0.0rc0/hdl21/tests/test_doc_examples.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/tests/test_exports.py` & `hdl21-6.0.0rc0/hdl21/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/tests/test_hdl21.py` & `hdl21-6.0.0rc0/hdl21/tests/test_hdl21.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import copy, pytest
 import hdl21 as h
 
 T = TypeVar("T")
 
 
 def test_version():
-    assert h.__version__ == "5.0.0"  # NOTE: VLSIR_VERSION
+    assert h.__version__ == "6.0.0rc0"  # VLSIR_VERSION
 
 
 def test_module1():
     """Initial Module Test"""
 
     @h.module
     class M1:
```

### Comparing `hdl21-5.0.0/hdl21/tests/test_params.py` & `hdl21-6.0.0rc0/hdl21/tests/test_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,16 +113,17 @@
 
     with pytest.raises(RuntimeError):
         # Test that sub-classing a h.paramclass fails
 
         class D(C):
             ...
 
-    with pytest.raises(TypeError):
+    with pytest.raises((TypeError, ValidationError)):
         # Test that missing arguments fail
+        # Note whether this is `TypeError` or `ValidationError` depends on the version of Pydantic.
         c = C()
 
     with pytest.raises(ValidationError):
         # Test invalid argument types fail
 
         c = C(a=TabError)
```

### Comparing `hdl21-5.0.0/hdl21/tests/test_prefix.py` & `hdl21-6.0.0rc0/hdl21/tests/test_prefix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest as pt
 from decimal import Decimal
 from pydantic import ValidationError
 from pydantic.dataclasses import dataclass
 
 import hdl21 as h
+from hdl21.datatype import OurBaseConfig
 
 
 def test_decimal():
     """This isn't a test of Hdl21 so much as a demo and reminder of how
     the standard library's `Decimal` works, particularly in conjunction with
     our widely-used `pydantic.dataclasses`.
 
@@ -128,15 +129,14 @@
     assert (1 * e(1)) * (1 * e(2)) == 1 * e(3)
     assert 2 * (1 * e(2)) == 2 * e(2)
     assert (1 * e(2)) * 2 == 2 * e(2)
     assert (1 * e(2)) * 2.0 == 2.0 * e(2)
 
 
 def test_prefixed_div():
-
     """Test `Prefixed` True Division"""
     from hdl21.prefix import e
 
     assert (1 * e(0)) / 2 == 0.5 * e(0)
     assert (1 * e(0)) / (2 * e(0)) == 0.5 * e(0)
     assert 2 / (1 * e(0)) == 2 * e(0)
     assert 6 / (3 * e(0)) == 2 * e(0)
@@ -474,18 +474,19 @@
     with pt.raises(TypeError):
         assert Exponent(K, Decimal(0)) / [] == NotImplemented
     with pt.raises(TypeError):
         assert Exponent(K, Decimal(0)) ** [] == NotImplemented
     assert e([]) == NotImplemented
 
 
+@pt.mark.xfail(reason="Testing for #157 pydantic v2")
 def test_prefixed_and_scalar_conversions():
     """Test inline conversions of built-in numeric types to `Prefixed` and `Scalar`."""
 
-    @dataclass
+    @dataclass(config=OurBaseConfig)
     class P:
         x: h.Prefixed
         y: h.Scalar
 
     # Test with int for each
     p = P(x=1, y=1)
     assert p.x == h.Prefixed(number=Decimal(1))
```

### Comparing `hdl21-5.0.0/hdl21/tests/test_source_info.py` & `hdl21-6.0.0rc0/hdl21/tests/test_source_info.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21/walker.py` & `hdl21-6.0.0rc0/hdl21/walker.py`

 * *Files identical despite different names*

### Comparing `hdl21-5.0.0/hdl21.egg-info/PKG-INFO` & `hdl21-6.0.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 Metadata-Version: 2.1
 Name: hdl21
-Version: 5.0.0
+Version: 6.0.0rc0
 Summary: Hardware Description Library
-Home-page: https://github.com/dan-fritchman/Hdl21
-Author: Dan Fritchman
-Author-email: dan@fritch.mn
-Requires-Python: >=3.7, <3.12
+Keywords: HDL,EDA,analog,circuit
+Author: Thomas Pluck, Kennedy Caisley, Zeyi Wang, Arya Reais-Parsi, Vighnesh Iyer
+Author-email: Dan Fritchman <dan@fritch.mn>, Curtis Mayberry <Curtisma3@gmail.com>
+Maintainer-email: Dan Fritchman <dan@fritch.mn>
+Requires-Python: >=3.7, <3.13
 Description-Content-Type: text/markdown
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
+Requires-Dist: vlsir>=6.0.0rc0,<7
+Requires-Dist: vlsirtools>=6.0.0rc0,<7
+Requires-Dist: pydantic>=1.9.0,<2.7
+Requires-Dist: pytest==7.1 ; extra == "dev"
+Requires-Dist: coverage ; extra == "dev"
+Requires-Dist: pytest-cov ; extra == "dev"
+Requires-Dist: pre-commit==2.20 ; extra == "dev"
+Requires-Dist: black==22.6 ; extra == "dev"
+Requires-Dist: flit ; extra == "dev"
+Project-URL: Bug Tracker, https://github.com/dan-fritchman/Hdl21/issues
+Project-URL: Documentation, https://github.com/dan-fritchman/Hdl21/blob/main/readme.md
+Project-URL: Homepage, https://github.com/dan-fritchman/Hdl21
+Project-URL: Repository, https://github.com/dan-fritchman/Hdl21
 Provides-Extra: dev
-License-File: LICENSE
 
 # HDL21
 
 ## Analog Hardware Description Library in Python
 
 [![pypi](https://img.shields.io/badge/pypi-hdl21-blue)](https://pypi.org/project/hdl21/)
 [![python-versions](https://img.shields.io/badge/python-3.7_3.8_3.9_3.10_3.11-blue)](https://codecov.io/gh/dan-fritchman/Hdl21)
@@ -1280,16 +1296,14 @@
 - Clone this repository & navigate to it.
 - `bash scripts/install-dev.sh`. See the note below.
 - `pytest -s` should yield something like:
 
 ```
 $ pytest -s
 ============================ test session starts =============================
-platform darwin -- Python 3.10.0, pytest-7.1.2, pluggy-1.0.0
-plugins: anyio-3.5.0, cov-3.0.0
 collected 126 items
 
 hdl21/pdk/test_pdk.py ...
 hdl21/pdk/sample_pdk/test_sample_pdk.py ...
 hdl21/sim/tests/test_sim.py .........s
 hdl21/tests/test_builtin_generators.py ..
 hdl21/tests/test_bundles.py ............
@@ -1303,7 +1317,8 @@
 pdks/Sky130/sky130/test_sky130.py ....
 
 ================= 119 passed, 1 skipped, 6 xfailed in 0.55s ==================
 ```
 
 Note: Hdl21 is commonly co-developed with the [VLSIR](https://github.com/Vlsir/Vlsir) interchange formats.
 The [scripts](./scripts) folder includes two short installation scripts which install VLSIR from either PyPi or GitHub. Tweaks to PyPi-released versions Hdl21 may be able to use the PyPi versions of VLSIR. Most Hdl21 development cannot, and should clone VLSIR from GitHub. The `install-dev` script will install VLSIR alongside `Hdl21/`, i.e. in the parent directory of the Hdl21 clone.
+
```

