# Comparing `tmp/pdbeccdutils-0.8.4.tar.gz` & `tmp/pdbeccdutils-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbeccdutils-0.8.4.tar", last modified: Tue Oct 31 09:38:52 2023, max compression
+gzip compressed data, was "pdbeccdutils-0.8.5.tar", last modified: Fri May 24 08:45:00 2024, max compression
```

## Comparing `pdbeccdutils-0.8.4.tar` & `pdbeccdutils-0.8.5.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:52.917446 pdbeccdutils-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2023-10-31 09:38:52.917446 pdbeccdutils-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:52.905446 pdbeccdutils-0.8.4/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:52.905446 pdbeccdutils-0.8.4/pdbeccdutils/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:52.905446 pdbeccdutils-0.8.4/pdbeccdutils/computations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/computations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/computations/parity_method.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:52.909446 pdbeccdutils-0.8.4/pdbeccdutils/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11668 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/core/boundmolecule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13164 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/core/ccd_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/core/ccd_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21379 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/core/clc_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    17458 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/core/clc_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27323 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/core/component.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15219 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/core/depictions.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/core/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4029 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/core/fragment_library.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12731 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/core/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8271 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/core/prd_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    14037 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/core/prd_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:52.909446 pdbeccdutils-0.8.4/pdbeccdutils/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:52.909446 pdbeccdutils-0.8.4/pdbeccdutils/data/coordgen_templates/
--rw-r--r--   0 runner    (1001) docker     (127)    10551 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/data/coordgen_templates/templates.mae
--rw-r--r--   0 runner    (1001) docker     (127)   160441 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/data/fragment_library.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:52.909446 pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/adamantane.sdf
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/cube.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/decahydrocorrin.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/hem.sdf
--rw-r--r--   0 runner    (1001) docker     (127)      777 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/nonbornane.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/phorbine.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/porphin.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/porphycene.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/ru_complex.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/ru_complex2.sdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:52.909446 pdbeccdutils-0.8.4/pdbeccdutils/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9113 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/helpers/cif_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/helpers/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11760 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/helpers/drawing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/helpers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    10216 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/helpers/mol_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:52.909446 pdbeccdutils-0.8.4/pdbeccdutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16148 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/scripts/boundmolecule_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15620 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/scripts/process_components_cif_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/scripts/setup_pubchem_library_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:52.913446 pdbeccdutils-0.8.4/pdbeccdutils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_bound_molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_boundmolecule_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_clc_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_clc_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10398 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_file_writing.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_fragment_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_inchi_key_matches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_load_eoh_cif.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_parity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_process_components_cif_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_property_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_rdkit_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_residue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_scaffold_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_web_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/test_write_img.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/tests/tst_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:52.913446 pdbeccdutils-0.8.4/pdbeccdutils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/utils/pubchem_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/pdbeccdutils/utils/web_services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 09:38:52.905446 pdbeccdutils-0.8.4/pdbeccdutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2023-10-31 09:38:52.000000 pdbeccdutils-0.8.4/pdbeccdutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2023-10-31 09:38:52.000000 pdbeccdutils-0.8.4/pdbeccdutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 09:38:52.000000 pdbeccdutils-0.8.4/pdbeccdutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-10-31 09:38:52.000000 pdbeccdutils-0.8.4/pdbeccdutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 09:38:52.000000 pdbeccdutils-0.8.4/pdbeccdutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-10-31 09:38:52.000000 pdbeccdutils-0.8.4/pdbeccdutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-31 09:38:52.000000 pdbeccdutils-0.8.4/pdbeccdutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 09:38:52.917446 pdbeccdutils-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2023-10-31 09:38:39.000000 pdbeccdutils-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:45:00.850932 pdbeccdutils-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-24 08:45:00.846932 pdbeccdutils-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:45:00.834932 pdbeccdutils-0.8.5/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:45:00.834932 pdbeccdutils-0.8.5/pdbeccdutils/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:45:00.834932 pdbeccdutils-0.8.5/pdbeccdutils/computations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/computations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/computations/parity_method.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:45:00.838932 pdbeccdutils-0.8.5/pdbeccdutils/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11668 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/core/boundmolecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/core/ccd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43808 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/core/ccd_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21379 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/core/clc_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16653 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/core/clc_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27510 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/core/component.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15219 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/core/depictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/core/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4029 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/core/fragment_library.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13191 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/core/prd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13497 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/core/prd_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:45:00.838932 pdbeccdutils-0.8.5/pdbeccdutils/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:45:00.838932 pdbeccdutils-0.8.5/pdbeccdutils/data/coordgen_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/data/coordgen_templates/templates.mae
+-rw-r--r--   0 runner    (1001) docker     (127)   160441 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/data/fragment_library.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:45:00.838932 pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/adamantane.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/cube.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/decahydrocorrin.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/hem.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/nonbornane.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/phorbine.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/porphin.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/porphycene.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/ru_complex.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/ru_complex2.sdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:45:00.842932 pdbeccdutils-0.8.5/pdbeccdutils/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/helpers/cif_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/helpers/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/helpers/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/helpers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/helpers/mol_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:45:00.842932 pdbeccdutils-0.8.5/pdbeccdutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/scripts/boundmolecule_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15620 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/scripts/process_components_cif_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/scripts/setup_pubchem_library_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:45:00.846932 pdbeccdutils-0.8.5/pdbeccdutils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_bound_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_boundmolecule_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_clc_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_clc_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_file_writing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_fragment_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_inchi_key_matches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_load_eoh_cif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_parity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_process_components_cif_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_property_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_rdkit_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_residue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_scaffold_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_web_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/test_write_img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/tests/tst_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:45:00.846932 pdbeccdutils-0.8.5/pdbeccdutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/utils/pubchem_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/pdbeccdutils/utils/web_services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:45:00.846932 pdbeccdutils-0.8.5/pdbeccdutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-24 08:45:00.000000 pdbeccdutils-0.8.5/pdbeccdutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-24 08:45:00.000000 pdbeccdutils-0.8.5/pdbeccdutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:45:00.000000 pdbeccdutils-0.8.5/pdbeccdutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-24 08:45:00.000000 pdbeccdutils-0.8.5/pdbeccdutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:45:00.000000 pdbeccdutils-0.8.5/pdbeccdutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-24 08:45:00.000000 pdbeccdutils-0.8.5/pdbeccdutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 08:45:00.000000 pdbeccdutils-0.8.5/pdbeccdutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 08:45:00.850932 pdbeccdutils-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-24 08:44:56.000000 pdbeccdutils-0.8.5/setup.py
```

### Comparing `pdbeccdutils-0.8.4/LICENSE` & `pdbeccdutils-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/PKG-INFO` & `pdbeccdutils-0.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbeccdutils
-Version: 0.8.4
+Version: 0.8.5
 Summary: Toolkit to deal with wwPDB chemical components definitions for small molecules.
 Home-page: http://pypi.python.org/pypi/pdbeccdutils/
 Author: Protein Data Bank in Europe
 Author-email: pdbehelp@ebi.ac.uk
 License: Apache License 2.0.
 Project-URL: Source code, https://github.com/PDBeurope/ccdutils
 Project-URL: Documentation, https://pdbeurope.github.io/ccdutils/
```

### Comparing `pdbeccdutils-0.8.4/README.md` & `pdbeccdutils-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/doc/conf.py` & `pdbeccdutils-0.8.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/computations/parity_method.py` & `pdbeccdutils-0.8.5/pdbeccdutils/computations/parity_method.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/core/boundmolecule.py` & `pdbeccdutils-0.8.5/pdbeccdutils/core/boundmolecule.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/core/ccd_reader.py` & `pdbeccdutils-0.8.5/pdbeccdutils/core/ccd_reader.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/core/ccd_writer.py` & `pdbeccdutils-0.8.5/pdbeccdutils/core/ccd_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from xml.etree import ElementTree as ET
 from xml.etree.ElementTree import Element, SubElement
 
 import pdbeccdutils
 import rdkit
 import gemmi
 from gemmi import cif
-from pdbeccdutils.helpers import cif_tools
+from pdbeccdutils.helpers import cif_tools, mol_tools
 from pdbeccdutils.core.component import Component
 from pdbeccdutils.core.exceptions import CCDUtilsError
 from pdbeccdutils.core.models import ConformerType
 
 
 def write_molecule(
     path,
@@ -115,42 +115,23 @@
     Returns:
         str: String representation of the component in the PDB format.
     """
     (mol_to_save, conf_id, conf_type) = _prepate_structure(
         component, remove_hs, conf_type
     )
 
-    info = rdkit.Chem.rdchem.AtomPDBResidueInfo()
-    info.SetResidueName(f"{component.id:>3}")
-    info.SetTempFactor(20.0)
-    info.SetOccupancy(1.0)
-    info.SetChainId("A")
-    info.SetResidueNumber(1)
-    info.SetIsHeteroAtom(True)
-
-    for atom in mol_to_save.GetAtoms():
-        flag = _get_alt_atom_name(atom) if alt_names else _get_atom_name(atom)
-        atom_name = f"{flag:<4}"  # make sure it is 4 characters
-        info.SetName(atom_name)
-        atom.SetMonomerInfo(info)
-
     pdb_title = [
         f"HEADER    {conf_type.name} coordinates",
         f" for PDB-CCD {component.id}",
         f"COMPND    {component.id}",
         f"AUTHOR    pdbccdutils {pdbeccdutils.__version__}",
         f"AUTHOR    RDKit {rdkit.__version__}",
     ]
 
-    try:
-        pdb_body = rdkit.Chem.MolToPDBBlock(mol_to_save, conf_id)
-    except Exception:
-        pdb_body = _to_pdb_str_fallback(
-            mol_to_save, component.id, conf_id, conf_type.name
-        )
+    pdb_body = _to_pdb_str_fallback(mol_to_save, component.id, conf_id, alt_names)
 
     return "\n".join(pdb_title + [pdb_body])
 
 
 def to_sdf_str(
     component: Component,
     remove_hs: bool = True,
@@ -182,15 +163,15 @@
             try:
                 conf_id = -1
                 if c != ConformerType.AllConformers:
                     conf_id = component.get_conformer(c).GetId()
 
                 block = [
                     f"{component.id} - {c.name} conformer",
-                    rdkit.Chem.MolToMolBlock(mol_to_save, confId=conf_id).strip(),
+                    rdkit.Chem.MolToMolBlock(mol_to_save, confId=conf_id).strip("\n"),
                     "$$$$\n",
                 ]
                 mol_block += block
             except ValueError as e:
                 if str(e) == "Bad Conformer Id":
                     pass
                 else:
@@ -941,15 +922,15 @@
                     break
 
         atom_count = mol.GetNumAtoms()
         bond_count = mol.GetNumBonds()
 
         content += [
             f"{ccd_id} - {c.name} conformer",
-            "    RDKit   3D",
+            "     RDKit          3D",
             "\n" f"{atom_count:>3}{bond_count:3}  0  0  0  0  0  0  0  0999 V2000",
         ]
 
         for i in range(0, atom_count):
             pos = rdkit_conformer.GetAtomPosition(i)
             atom = mol.GetAtomWithIdx(i)
             sdf_charge = __charge_to_sdf(atom.GetFormalCharge())
@@ -968,61 +949,61 @@
                 )
             )
         content.append("M  END")
         content.append("$$$$\n")
     return content
 
 
-def _to_pdb_str_fallback(mol, component_id, conf_id, conf_name="Model"):
-    """Fallback method to generate PDB file in case the default one in
-    RDKit fails.
+def _to_pdb_str_fallback(mol, component_id, conf_id, alt_names):
+    """Method to generate PDB file
 
     Args:
         mol (rdkit.Chem.rdchem.Mol): Molecule to be written.
         component_id (str): Component id.
         conf_id (int): conformer id to be written.
-        conf_name (str): conformer name to be written.
+        alt_names (bool): atom names or alternate names.
 
     Returns:
         str: String representation the component in the PDB format.
     """
     conformer_ids = []
-    content = [
-        f"HEADER    {conf_name} coordinates for PDB-CCD {component_id}",
-        f"COMPND    {component_id}",
-        f"AUTHOR    pdbccdutils {pdbeccdutils.__version__}",
-        f"AUTHOR    RDKit {rdkit.__version__}",
-    ]
 
     if conf_id == -1:
         conformer_ids = [c.GetId() for c in mol.GetConformers()]
     else:
         conformer_ids = [conf_id]
 
+    content = []
     for m in conformer_ids:
         rdkit_conformer = mol.GetConformer(m)
 
         for i in range(0, mol.GetNumAtoms()):
             atom = mol.GetAtomWithIdx(i)
+            atom_name = _get_alt_atom_name(atom) if alt_names else _get_atom_name(atom)
+            atom_symbol = atom.GetSymbol()
+            # Atom name spans from column 13-16. For 4 letter atom names and 2 letter atom symbol it starts from column 13
+            # and for others column starts from 14
+            col_align = "{:<6}{:>5}  {:<3} {:>3} {}{:>4}{}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6.2f}{:>6.2f}          {:>2}"
+            if len(atom_name) == 4 or len(atom_symbol) == 2:
+                col_align = "{:<6}{:>5} {:<4} {:>3} {}{:>4}{}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6.2f}{:>6.2f}          {:>2}"
 
-            s = "{:<6}{:>5} {:<4} {:>3} {}{:>4}{}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6.2f}{:>6.2f}          {:>2}{:>2}".format(
+            s = col_align.format(
                 "HETATM",
                 i + 1,
-                atom.GetProp("name"),
+                atom_name,
                 component_id,
                 "A",
                 1,
                 " ",
                 rdkit_conformer.GetAtomPosition(i).x,
                 rdkit_conformer.GetAtomPosition(i).y,
                 rdkit_conformer.GetAtomPosition(i).z,
                 1,
                 20,
-                atom.GetSymbol(),
-                atom.GetFormalCharge(),
+                atom.GetSymbol().upper(),
             )
             content.append(s)
 
         for i in range(0, mol.GetNumAtoms()):
             pivot = mol.GetAtomWithIdx(i)
             s = "CONECT{:>5}".format(i + 1)
 
@@ -1185,38 +1166,38 @@
         "substructure_inchikeys",
     ]
     substructure_loop = cif_block_copy.init_loop(
         substructure_category, substructure_fields
     )
 
     for i, scaffold in enumerate(component.scaffolds):
-        mol = rdkit.Chem.MolFromSmiles(scaffold.smiles)
-        inchi = rdkit.Chem.MolToInchi(mol)
-        inchikey = rdkit.Chem.MolToInchiKey(mol)
+        smiles = rdkit.Chem.MolToSmiles(scaffold.mol)
+        inchi = mol_tools.inchi_from_mol(scaffold.mol).inchi
+        inchikey = mol_tools.inchikey_from_inchi(inchi)
         new_row = [
             component.id,
             scaffold.name,
             f"S{i+1}",
             "scaffold",
-            scaffold.smiles,
+            smiles,
             inchi or None,
             inchikey or None,
         ]
         substructure_loop.add_row(cif.quote_list(new_row))
 
     for j, fragment in enumerate(component.fragments):
-        mol = rdkit.Chem.MolFromSmiles(fragment.smiles)
-        inchi = rdkit.Chem.MolToInchi(mol)
-        inchikey = rdkit.Chem.MolToInchiKey(mol)
+        smiles = rdkit.Chem.MolToSmiles(fragment.mol)
+        inchi = mol_tools.inchi_from_mol(fragment.mol).inchi
+        inchikey = mol_tools.inchikey_from_inchi(inchi)
         new_row = [
             component.id,
             fragment.name,
             f"F{j+1}",
             "fragment",
-            fragment.smiles,
+            smiles,
             inchi or None,
             inchikey or None,
         ]
         substructure_loop.add_row(cif.quote_list(new_row))
 
     mapping_category = "_pdbe_chem_comp_substructure_mapping."
     mapping_fields = ["comp_id", "atom_id", "substructure_id", "substructure_ordinal"]
```

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/core/clc_reader.py` & `pdbeccdutils-0.8.5/pdbeccdutils/core/clc_reader.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/core/clc_writer.py` & `pdbeccdutils-0.8.5/pdbeccdutils/core/clc_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,40 +87,24 @@
 
     Returns:
         str: String representation of the component in the PDB format.
     """
     (mol_to_save, conf_id, conf_type) = ccd_writer._prepate_structure(
         component, remove_hs, conf_type
     )
-    residue_numbers = _get_residue_number(mol_to_save)
-    for atom in mol_to_save.GetAtoms():
-        flag = ccd_writer._get_atom_name(atom)
-        atom_name = f"{flag:<4}"  # make sure it is 4 characters
-        res_info = atom.GetPDBResidueInfo()
-        res_num = residue_numbers[atom.GetProp("residue_id")]
-        res_info.SetResidueNumber(res_num)
-        res_info.SetName(atom_name)
-        res_info.SetTempFactor(20.0)
-        res_info.SetOccupancy(1.0)
-        res_info.SetChainId("A")
 
     pdb_title = [
         f"HEADER    {conf_type.name} coordinates",
         f" for PDB-CLC {component.id}",
         f"COMPND    {component.id}",
         f"AUTHOR    pdbccdutils {pdbeccdutils.__version__}",
         f"AUTHOR    RDKit {rdkit.__version__}",
     ]
 
-    try:
-        pdb_body = rdkit.Chem.MolToPDBBlock(mol_to_save, conf_id)
-    except Exception:
-        pdb_body = _to_pdb_str_fallback(
-            mol_to_save, component.id, conf_id, conf_type.name
-        )
+    pdb_body = _to_pdb_str_fallback(mol_to_save, conf_id)
 
     return "\n".join(pdb_title + [pdb_body])
 
 
 def to_cml_str(component: Component, remove_hs=True, conf_type=ConformerType.Model):
     """Converts structure to the EBI representation of the molecule in
     CML format: http://cml.sourceforge.net/schema/cmlCore.xsd
@@ -229,62 +213,58 @@
         "",
     )
     inchi_e.text = component.inchi
 
     return root
 
 
-def _to_pdb_str_fallback(mol, component_id, conf_id, conf_name="Model"):
-    """Fallback method to generate PDB file in case the default one in
-    RDKit fails.
+def _to_pdb_str_fallback(mol, conf_id):
+    """Method to generate PDB file
 
     Args:
         mol (rdkit.Chem.rdchem.Mol): Molecule to be written.
-        component_id (str): Component id.
         conf_id (int): conformer id to be written.
-        conf_name (str): conformer name to be written.
 
     Returns:
         str: String representation the component in the PDB format.
     """
     conformer_ids = []
-    content = [
-        f"HEADER    {conf_name} coordinates for PDB-CLC {component_id}",
-        f"COMPND    {component_id}",
-        f"AUTHOR    pdbccdutils {pdbeccdutils.__version__}",
-        f"AUTHOR    RDKit {rdkit.__version__}",
-    ]
+    content = []
 
     if conf_id == -1:
         conformer_ids = [c.GetId() for c in mol.GetConformers()]
     else:
         conformer_ids = [conf_id]
 
     residue_numbers = _get_residue_number(mol)
     for m in conformer_ids:
         rdkit_conformer = mol.GetConformer(m)
         for i in range(0, mol.GetNumAtoms()):
             atom = mol.GetAtomWithIdx(i)
             res_info = atom.GetPDBResidueInfo()
+            atom_name = atom.GetProp("name")
+            atom_symbol = atom.GetSymbol().upper()
+            col_align = "{:<6}{:>5}  {:<3} {:>3} {}{:>4}{}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6.2f}{:>6.2f}          {:>2}"
+            if len(atom_name) == 4 or len(atom_symbol) == 2:
+                col_align = "{:<6}{:>5} {:<4} {:>3} {}{:>4}{}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6.2f}{:>6.2f}          {:>2}"
 
-            s = "{:<6}{:>5} {:<4} {:>3} {}{:>4}{}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6.2f}{:>6.2f}          {:>2}{:>2}".format(
+            s = col_align.format(
                 "HETATM",
                 i + 1,
-                atom.GetProp("name"),
+                atom_name,
                 res_info.GetResidueName(),
                 "A",
                 residue_numbers[atom.GetProp("residue_id")],
                 " ",
                 rdkit_conformer.GetAtomPosition(i).x,
                 rdkit_conformer.GetAtomPosition(i).y,
                 rdkit_conformer.GetAtomPosition(i).z,
                 1,
                 20,
-                atom.GetSymbol(),
-                atom.GetFormalCharge(),
+                atom_symbol,
             )
             content.append(s)
 
         for i in range(0, mol.GetNumAtoms()):
             pivot = mol.GetAtomWithIdx(i)
             s = "CONECT{:>5}".format(i + 1)
```

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/core/component.py` & `pdbeccdutils-0.8.5/pdbeccdutils/core/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import logging
 import re
 from datetime import date
 from typing import Any, Dict, List, Tuple
 
 import rdkit
 import gemmi
-from rdkit.Chem import BRICS, Draw
+from rdkit.Chem import BRICS, Draw, BondType
 from rdkit.Chem.rdMolDescriptors import Properties
 from rdkit.Chem.Scaffolds import MurckoScaffold
 
 from pdbeccdutils.core.depictions import DepictionManager, DepictionResult
 from pdbeccdutils.core.exceptions import CCDUtilsError
 from pdbeccdutils.helpers import mol_tools
 from pdbeccdutils.core.fragment_library import FragmentLibrary
@@ -223,18 +223,20 @@
     def inchi_from_rdkit(self) -> str:
         """Provides the InChI worked out by RDKit.
 
         Returns:
             str: the InChI or empty '' if there was an error finding it.
         """
         if not self._inchi_from_rdkit:
-            try:
-                self._inchi_from_rdkit = rdkit.Chem.inchi.MolToInchi(self.mol)
-            except ValueError:
+            inchi_result = mol_tools.inchi_from_mol(self.mol)
+            if inchi_result.errors:
                 self._inchi_from_rdkit = ""
+            else:
+                self._inchi_from_rdkit = inchi_result.inchi
+
         return self._inchi_from_rdkit
 
     @property
     def inchikey_from_rdkit(self) -> str:
         """Provides the InChIKey worked out by RDKit.
 
         Returns:
@@ -508,18 +510,22 @@
 
         if names:
             for i, a in enumerate(self.mol2D.GetAtoms()):
                 atom_name = get_atom_name(a)
                 options.atomLabels[i] = atom_name
                 a.SetProp("molFileAlias", atom_name)
 
+        mol_tools.change_bonds_type(self.mol2D, BondType.DATIVE, BondType.ZERO)
+
         drawing.draw_molecule(
             self.mol2D, drawer, file_name, wedge_bonds, atom_highlight, bond_highlight
         )
 
+        mol_tools.change_bonds_type(self.mol2D, BondType.ZERO, BondType.ZERO)
+
     def export_2d_annotation(self, file_name: str, wedge_bonds: bool = True) -> None:
         """Generates 2D depiction in JSON format with annotation of
         bonds and atoms to be redrawn in the interactions component.
 
         Args:
             file_name (str): Path to the file
         """
@@ -671,17 +677,15 @@
                 matches = self.mol_no_h.GetSubstructMatches(v.mol)
 
                 if not matches:
                     continue
 
                 key = f"{fragment_library.name}_{v.name}"
                 if key not in self._fragments:
-                    temp[key] = SubstructureMapping(
-                        v.name, rdkit.Chem.MolToSmiles(v.mol), v.source, matches
-                    )
+                    temp[key] = SubstructureMapping(v.name, v.mol, v.source, matches)
 
             except Exception:
                 logging.warning(f"Error mapping fragment {v.name}.")
 
         self._fragments.update(temp)
 
         return list(temp.values())
@@ -714,26 +718,27 @@
 
                 for mol in brics_mols:
                     rdkit.Chem.RemoveHs(mol)
 
                 brics_hits = [self.mol_no_h.GetSubstructMatches(i) for i in brics_mols]
 
                 for index, brics_hit in enumerate(brics_hits):
-                    smiles = rdkit.Chem.MolToSmiles(brics_mols[index])
+                    brics_mol = brics_mols[index]
+                    smiles = rdkit.Chem.MolToSmiles(brics_mol)
                     name = scaffolding_method.name
                     source = "RDKit scaffolds"
                     key = f"{name}_{smiles}"
                     brics_hit = conversions.listit(brics_hit)
 
                     if not smiles:
                         continue
 
                     if key not in self._scaffolds:
                         self._scaffolds[key] = SubstructureMapping(
-                            name, smiles, source, brics_hit
+                            name, brics_mol, source, brics_hit
                         )
 
                 return brics_mols
 
             for s in scaffolds:
                 scaffold_atom_names = [atom.GetProp("name") for atom in s.GetAtoms()]
                 mapping = []
@@ -752,15 +757,15 @@
                 if not smiles:
                     continue
 
                 if name in self._scaffolds:
                     self._scaffolds[name].mappings.append(mapping)
                 else:
                     self._scaffolds[name] = SubstructureMapping(
-                        name, smiles, source, [mapping]
+                        name, s, source, [mapping]
                     )
 
             return scaffolds
 
         except (RuntimeError, ValueError):
             raise CCDUtilsError(
                 f"Computing scaffolds using method {scaffolding_method.name} failed."
@@ -798,10 +803,10 @@
 
         for v in struct_mapping.values():
             mappings = []
 
             for m in v.mappings:
                 atom_names = [self.mol.GetAtomWithIdx(idx).GetProp("name") for idx in m]
                 mappings.append(atom_names)
-            res.append(SubstructureMapping(v.name, v.smiles, v.source, mappings))
+            res.append(SubstructureMapping(v.name, v.mol, v.source, mappings))
 
         return res
```

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/core/depictions.py` & `pdbeccdutils-0.8.5/pdbeccdutils/core/depictions.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/core/fragment_library.py` & `pdbeccdutils-0.8.5/pdbeccdutils/core/fragment_library.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/core/models.py` & `pdbeccdutils-0.8.5/pdbeccdutils/core/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,21 +266,21 @@
 
 @dataclass
 class SubstructureMapping:
     """Represents a fragment hit in the component
 
     Args:
         name (str): Name of the substructure.
-        smiles (str): SMILES representation of the substructure
+        mol (Chem.rdchem.Mol): RDKit Mol object
         source (str): Where does this fragment come from.
         mapping (List[List[Any]]): Mappings with atom names or indices.
     """
 
     name: str
-    smiles: str
+    mol: Chem.rdchem.Mol
     source: str
     mappings: List[List[Any]]
 
 
 class Subcomponent:
     """Represents a subcompoent in a component
 
@@ -304,19 +304,38 @@
 
         return True
 
 
 class BoundMolecule:
     def __init__(self, graph):
         self.graph = graph
-        self.id = "-".join(x.id for x in graph.nodes)
-        self.orig_id = "-".join(
-            x.orig_id if isinstance(x, AssemblyResidue) else x.id for x in graph.nodes
+        self.nodes = sorted(self.graph, key=lambda l: (int(l.res_id), l.chain))
+
+    @property
+    def id(self) -> str:
+        """Returns Id of boundmolecule as combination of
+        chain and residue ids
+        """
+        return "-".join(x.id for x in self.nodes)
+
+    @property
+    def orig_id(self) -> str:
+        """Returns id of boundmolecule without
+        symmetry operator
+        """
+        return "-".join(
+            x.orig_id if isinstance(x, AssemblyResidue) else x.id for x in self.nodes
         )
-        self.name = "_".join(x.name for x in graph.nodes)
+
+    @property
+    def name(self) -> str:
+        """Returns name of boundmolecule as a
+        combination of residue names
+        """
+        return "_".join(x.name for x in self.nodes)
 
     def __eq__(self, other) -> bool:
         """Checks the equality of two BoundMolecule objects
 
         Returns:
             True if id of the BoundMolecules are same else False
         """
```

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/core/prd_reader.py` & `pdbeccdutils-0.8.5/pdbeccdutils/core/prd_reader.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/core/prd_writer.py` & `pdbeccdutils-0.8.5/pdbeccdutils/core/prd_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,41 +111,23 @@
     Returns:
         str: String representation of the component in the PDB format.
     """
     (mol_to_save, conf_id, conf_type) = ccd_writer._prepate_structure(
         component, remove_hs, conf_type
     )
 
-    for atom in mol_to_save.GetAtoms():
-        flag = (
-            ccd_writer._get_alt_atom_name(atom)
-            if alt_names
-            else ccd_writer._get_atom_name(atom)
-        )
-        atom_name = f"{flag:<4}"  # make sure it is 4 characters
-        res_info = atom.GetPDBResidueInfo()
-        res_info.SetName(atom_name)
-        res_info.SetTempFactor(20.0)
-        res_info.SetOccupancy(1.0)
-        res_info.SetChainId("A")
-
     pdb_title = [
         f"HEADER    {conf_type.name} coordinates",
         f" for PDB-PRD {component.id}",
         f"COMPND    {component.id}",
         f"AUTHOR    pdbccdutils {pdbeccdutils.__version__}",
         f"AUTHOR    RDKit {rdkit.__version__}",
     ]
 
-    try:
-        pdb_body = rdkit.Chem.MolToPDBBlock(mol_to_save, conf_id)
-    except Exception:
-        pdb_body = _to_pdb_str_fallback(
-            mol_to_save, component.id, conf_id, conf_type.name
-        )
+    pdb_body = _to_pdb_str_fallback(mol_to_save, conf_id, alt_names)
 
     return "\n".join(pdb_title + [pdb_body])
 
 
 def to_pdb_ccd_cif_file(path, component: Component, remove_hs=True):
     """Converts structure to the PDB CIF format. Both model and ideal
     coordinates are stored. In case ideal coordinates are missing, rdkit
@@ -365,62 +347,63 @@
     """
     return atom.GetProp("residue_id") if atom.HasProp("residue_id") else None
 
 
 # region fallbacks
 
 
-def _to_pdb_str_fallback(mol, component_id, conf_id, conf_name="Model"):
-    """Fallback method to generate PDB file in case the default one in
-    RDKit fails.
+def _to_pdb_str_fallback(mol, conf_id, alt_names):
+    """Method to generate PDB file
 
     Args:
         mol (rdkit.Chem.rdchem.Mol): Molecule to be written.
-        component_id (str): Component id.
         conf_id (int): conformer id to be written.
-        conf_name (str): conformer name to be written.
+        alt_names (bool): atom names or alternate names.
 
     Returns:
         str: String representation the component in the PDB format.
     """
     conformer_ids = []
-    content = [
-        f"HEADER    {conf_name} coordinates for PDB-CCD {component_id}",
-        f"COMPND    {component_id}",
-        f"AUTHOR    pdbccdutils {pdbeccdutils.__version__}",
-        f"AUTHOR    RDKit {rdkit.__version__}",
-    ]
+    content = []
 
     if conf_id == -1:
         conformer_ids = [c.GetId() for c in mol.GetConformers()]
     else:
         conformer_ids = [conf_id]
 
     for m in conformer_ids:
         rdkit_conformer = mol.GetConformer(m)
 
         for i in range(0, mol.GetNumAtoms()):
             atom = mol.GetAtomWithIdx(i)
             res_info = atom.GetPDBResidueInfo()
+            atom_name = (
+                ccd_writer._get_alt_atom_name(atom)
+                if alt_names
+                else ccd_writer._get_atom_name(atom)
+            )
+            atom_symbol = atom.GetSymbol().upper()
+            col_align = "{:<6}{:>5}  {:<3} {:>3} {}{:>4}{}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6.2f}{:>6.2f}          {:>2}"
+            if len(atom_name) == 4 or len(atom_symbol) == 2:
+                col_align = "{:<6}{:>5} {:<4} {:>3} {}{:>4}{}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6.2f}{:>6.2f}          {:>2}"
 
-            s = "{:<6}{:>5} {:<4} {:>3} {}{:>4}{}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6.2f}{:>6.2f}          {:>2}{:>2}".format(
+            s = col_align.format(
                 "HETATM",
                 i + 1,
-                atom.GetProp("name"),
+                atom_name,
                 res_info.GetResidueName(),
                 "A",
                 res_info.GetResidueNumber(),
                 " ",
                 rdkit_conformer.GetAtomPosition(i).x,
                 rdkit_conformer.GetAtomPosition(i).y,
                 rdkit_conformer.GetAtomPosition(i).z,
                 1,
                 20,
-                atom.GetSymbol(),
-                atom.GetFormalCharge(),
+                atom_symbol,
             )
             content.append(s)
 
         for i in range(0, mol.GetNumAtoms()):
             pivot = mol.GetAtomWithIdx(i)
             s = "CONECT{:>5}".format(i + 1)
```

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/data/coordgen_templates/templates.mae` & `pdbeccdutils-0.8.5/pdbeccdutils/data/coordgen_templates/templates.mae`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/data/fragment_library.tsv` & `pdbeccdutils-0.8.5/pdbeccdutils/data/fragment_library.tsv`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/adamantane.sdf` & `pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/adamantane.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/cube.sdf` & `pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/cube.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/decahydrocorrin.sdf` & `pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/decahydrocorrin.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/hem.sdf` & `pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/hem.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/nonbornane.sdf` & `pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/nonbornane.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/phorbine.sdf` & `pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/phorbine.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/porphin.sdf` & `pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/porphin.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/porphycene.sdf` & `pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/porphycene.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/ru_complex.sdf` & `pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/ru_complex.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/data/general_templates/ru_complex2.sdf` & `pdbeccdutils-0.8.5/pdbeccdutils/data/general_templates/ru_complex2.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/helpers/cif_tools.py` & `pdbeccdutils-0.8.5/pdbeccdutils/helpers/cif_tools.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/helpers/conversions.py` & `pdbeccdutils-0.8.5/pdbeccdutils/helpers/conversions.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/helpers/drawing.py` & `pdbeccdutils-0.8.5/pdbeccdutils/helpers/drawing.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/helpers/helper.py` & `pdbeccdutils-0.8.5/pdbeccdutils/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/helpers/mol_tools.py` & `pdbeccdutils-0.8.5/pdbeccdutils/helpers/mol_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 """
 Set of methods for molecular sanitization and work with conformers
 """
 
 import re
 import sys
 from io import StringIO
+from rdkit.Chem import BondType
 from pdbeccdutils.core.models import (
     InChIFromRDKit,
     MolFromRDKit,
     ConformerType,
     SanitisationResult,
 )
 from contextlib import redirect_stderr
@@ -169,28 +170,26 @@
             smarts_metal_check = rdkit.Chem.MolFromSmarts(
                 METALS_SMART + "~[{}]".format(element)
             )
             metal_atom_bonds = rwmol.GetSubstructMatches(smarts_metal_check)
             rdkit.Chem.SanitizeMol(
                 rwmol, sanitizeOps=rdkit.Chem.SanitizeFlags.SANITIZE_CLEANUP
             )
-
-            for metal_index, atom_index in metal_atom_bonds:
+            for metal_index, other_index in metal_atom_bonds:
                 metal_atom = rwmol.GetAtomWithIdx(metal_index)
-                erroneous_atom = rwmol.GetAtomWithIdx(atom_index)
-
-                # change the bond type to dative
-                bond = rwmol.GetBondBetweenAtoms(
-                    metal_atom.GetIdx(), erroneous_atom.GetIdx()
-                )
-                bond.SetBondType(rdkit.Chem.BondType.SINGLE)
-
-                if erroneous_atom.GetExplicitValence() == valency:
-                    erroneous_atom.SetFormalCharge(erroneous_atom.GetFormalCharge() + 1)
-                    metal_atom.SetFormalCharge(metal_atom.GetFormalCharge() - 1)
+                other_atom = rwmol.GetAtomWithIdx(other_index)
+                # alter the bond to be dative towards the metal -
+                if other_atom.GetExplicitValence() == valency:
+                    rwmol.RemoveBond(metal_atom.GetIdx(), other_atom.GetIdx())
+                    rwmol.AddBond(
+                        other_atom.GetIdx(),
+                        metal_atom.GetIdx(),
+                        rdkit.Chem.BondType.DATIVE,
+                    )
+            rwmol.UpdatePropertyCache()  # regenerates valence records
 
         attempts -= 1
 
     sys.stderr = saved_std_err
 
     return False
 
@@ -219,18 +218,23 @@
     Args:
         mol: rdkit.Chem.rdchem.Mol object
 
     Returns:
         InChIFromRDKit: NamedTuple containing inchi, warnings and errors
         generated.
     """
+
+    # Alter Dative bond type to Single as InChI calculation doesn't work in mol
+    # with Dative bond
+    mol_copy = rdkit.Chem.RWMol(mol)
+    change_bonds_type(mol_copy, BondType.DATIVE, BondType.SINGLE)
     try:
         rdkit_stream = StringIO()  # redirecting rdkit logs
         with redirect_stderr(rdkit_stream):
-            inchi = rdkit.Chem.inchi.MolToInchi(mol)
+            inchi = rdkit.Chem.inchi.MolToInchi(mol_copy)
             warnings = None
             errors = None
             rdkit_log = rdkit_stream.getvalue()
             if "WARNING" in rdkit_log:
                 start_index = re.search(r"\bWARNING\b:", rdkit_log).end()
                 warnings = rdkit_log[start_index:].strip()
             elif "ERROR" in rdkit_log:
@@ -317,7 +321,21 @@
     atom_coords_list = [
         atom_position[i] if not np.isnan(atom_position[i]) else 0.0 for i in range(3)
     ]
     atom_coords = rdkit.Chem.rdGeometry.Point3D(
         atom_coords_list[0], atom_coords_list[1], atom_coords_list[2]
     )
     conformer.SetAtomPosition(atom_id, atom_coords)
+
+
+def change_bonds_type(mol, from_type, to_type) -> None:
+    """
+    alters all bonds that are from_type to to_type
+
+    Args:
+        mol (rdkit.Chem.rdchem.Mol): Mol object from RDKit
+        from_type: Bond type to be changed
+        to_type: Type of bond to be set
+    """
+    for bond in mol.GetBonds():
+        if bond.GetBondType() == from_type:
+            bond.SetBondType(to_type)
```

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/scripts/boundmolecule_cli.py` & `pdbeccdutils-0.8.5/pdbeccdutils/scripts/boundmolecule_cli.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/scripts/process_components_cif_cli.py` & `pdbeccdutils-0.8.5/pdbeccdutils/scripts/process_components_cif_cli.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/scripts/setup_pubchem_library_cli.py` & `pdbeccdutils-0.8.5/pdbeccdutils/scripts/setup_pubchem_library_cli.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/conftest.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/test_boundmolecule_cli.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/test_boundmolecule_cli.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/test_clc_reader.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/test_clc_reader.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/test_clc_writer.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/test_clc_writer.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/test_file_writing.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/test_file_writing.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         for ideal in True, False:
             for remove_h in True, False:
                 conformer = ConformerType.Ideal if ideal else ConformerType.Model
                 conf_id = component.get_conformer(conformer).GetId()
                 rdkit_mol = component.mol_no_h if remove_h else component.mol
 
                 pdb_repr = ccd_writer._to_pdb_str_fallback(
-                    rdkit_mol, component.id, conf_id
+                    rdkit_mol, component.id, conf_id, False
                 )
 
                 assert pdb_repr
                 mol = Chem.MolFromPDBBlock(pdb_repr, sanitize=False, removeHs=False)
 
                 assert isinstance(mol, Chem.rdchem.Mol)
                 assert mol.GetNumAtoms() == rdkit_mol.GetNumAtoms()
```

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/test_fragment_library.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/test_fragment_library.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/test_helper_methods.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/test_helper_methods.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/test_load_eoh_cif.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/test_load_eoh_cif.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/test_parity.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/test_parity.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/test_process_components_cif_cli.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/test_process_components_cif_cli.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/test_property_generation.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/test_property_generation.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/test_rdkit_fixtures.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/test_rdkit_fixtures.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/test_residue.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/test_residue.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/test_scaffold_generation.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/test_scaffold_generation.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         component = ccd_reader.read_pdb_cif_file(cif_filename(ccd_id)).component
         result = component.get_scaffolds()
 
         mol = result[0]
 
         assert Chem.MolToSmiles(mol) == smiles
         assert component.scaffolds
-        assert component.scaffolds[0].smiles == smiles
+        assert Chem.MolToSmiles(component.scaffolds[0].mol) == smiles
 
     @staticmethod
     @pytest.mark.parametrize("ccd_id", ["EOH", "DMS"])
     def test_scaffold_absent(ccd_id):
         component = ccd_reader.read_pdb_cif_file(cif_filename(ccd_id)).component
         result = component.get_scaffolds()
```

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/test_web_services.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/test_web_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pytest
 from rdkit import Chem
 
 from pdbeccdutils.core import ccd_reader
 from pdbeccdutils.tests.tst_utilities import cif_filename
 from pdbeccdutils.utils.pubchem_downloader import PubChemDownloader
 
-ids_to_test = ["MAN", "NAG", "SO4", "GOL", "SAC", "VIA", "GLU"]
+ids_to_test = ["NAG", "SO4", "GOL", "SAC", "VIA", "GLU"]
 
 
 class TestWebServices:
     @staticmethod
     @pytest.mark.parametrize("het_code", ids_to_test)
     def test_components_layouts_downloaded(tmp_path, het_code):
         dl = PubChemDownloader(str(tmp_path))
```

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/test_write_img.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/test_write_img.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/tests/tst_utilities.py` & `pdbeccdutils-0.8.5/pdbeccdutils/tests/tst_utilities.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/utils/pubchem_downloader.py` & `pdbeccdutils-0.8.5/pdbeccdutils/utils/pubchem_downloader.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils/utils/web_services.py` & `pdbeccdutils-0.8.5/pdbeccdutils/utils/web_services.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils.egg-info/PKG-INFO` & `pdbeccdutils-0.8.5/pdbeccdutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbeccdutils
-Version: 0.8.4
+Version: 0.8.5
 Summary: Toolkit to deal with wwPDB chemical components definitions for small molecules.
 Home-page: http://pypi.python.org/pypi/pdbeccdutils/
 Author: Protein Data Bank in Europe
 Author-email: pdbehelp@ebi.ac.uk
 License: Apache License 2.0.
 Project-URL: Source code, https://github.com/PDBeurope/ccdutils
 Project-URL: Documentation, https://pdbeurope.github.io/ccdutils/
```

### Comparing `pdbeccdutils-0.8.4/pdbeccdutils.egg-info/SOURCES.txt` & `pdbeccdutils-0.8.5/pdbeccdutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.8.4/setup.py` & `pdbeccdutils-0.8.5/setup.py`

 * *Files identical despite different names*

