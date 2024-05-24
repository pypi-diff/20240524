# Comparing `tmp/pe-configurator-1.0.3.tar.gz` & `tmp/pe_configurator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pe-configurator-1.0.3.tar", last modified: Fri Dec  1 20:10:56 2023, max compression
+gzip compressed data, was "pe_configurator-1.0.4.tar", last modified: Fri May 24 10:36:06 2024, max compression
```

## Comparing `pe-configurator-1.0.3.tar` & `pe_configurator-1.0.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.577722 pe-configurator-1.0.3/
--rw-r--r--   0 hestelles   (501) staff       (20)     1349 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/.gitlab-ci.yml
--rw-r--r--   0 hestelles   (501) staff       (20)      538 2023-12-01 20:03:46.000000 pe-configurator-1.0.3/CHANGELOG.md
--rw-r--r--   0 hestelles   (501) staff       (20)     1100 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/LICENSE
--rw-r--r--   0 hestelles   (501) staff       (20)    11764 2023-12-01 20:10:56.576196 pe-configurator-1.0.3/PKG-INFO
--rw-r--r--   0 hestelles   (501) staff       (20)    10809 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/README.md
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.565808 pe-configurator-1.0.3/blueprints/
--rw-r--r--   0 hestelles   (501) staff       (20)      192 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/blueprints/test.yaml
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.565938 pe-configurator-1.0.3/data/
--rw-r--r--   0 hestelles   (501) staff       (20)  2290335 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/data/calibration_files.txt
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.567739 pe-configurator-1.0.3/docs/
--rw-r--r--   0 hestelles   (501) staff       (20)      580 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/docs/Makefile
--rw-r--r--   0 hestelles   (501) staff       (20)     2402 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/docs/conf.py
--rw-r--r--   0 hestelles   (501) staff       (20)      653 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/docs/index.rst
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.568279 pe-configurator-1.0.3/docs/source/
--rw-r--r--   0 hestelles   (501) staff       (20)     8634 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/docs/source/examples.rst
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.568751 pe-configurator-1.0.3/docs/source/images/
--rw-r--r--   0 hestelles   (501) staff       (20)    63225 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/docs/source/images/MECO_gw190521.png
--rw-r--r--   0 hestelles   (501) staff       (20)   130355 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/docs/source/images/fake_chirpmass_railing.png
--rw-r--r--   0 hestelles   (501) staff       (20)   121175 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/docs/source/images/fake_mass_ratio_rail_low.png
--rw-r--r--   0 hestelles   (501) staff       (20)     1299 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/docs/source/installation.rst
--rw-r--r--   0 hestelles   (501) staff       (20)    12337 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/docs/source/logic.md
--rw-r--r--   0 hestelles   (501) staff       (20)    10258 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/docs/source/logic.rst
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.569069 pe-configurator-1.0.3/docs/templates/
--rw-r--r--   0 hestelles   (501) staff       (20)      639 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/docs/templates/custom-class-template.rst
--rw-r--r--   0 hestelles   (501) staff       (20)     1465 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/docs/templates/custom-module-template.rst
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.569193 pe-configurator-1.0.3/examples/
--rw-r--r--   0 hestelles   (501) staff       (20)     8196 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/examples/.DS_Store
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.569961 pe-configurator-1.0.3/examples/test_GW190412/
--rw-r--r--   0 hestelles   (501) staff       (20)   821276 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/examples/test_GW190412/test.html
--rw-r--r--   0 hestelles   (501) staff       (20)      669 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/examples/test_GW190412/test.json
--rw-r--r--   0 hestelles   (501) staff       (20)     8592 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/examples/test_GW190412/test.pdf
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.570861 pe-configurator-1.0.3/examples/test_GW190521/
--rw-r--r--   0 hestelles   (501) staff       (20)   822260 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/examples/test_GW190521/test.html
--rw-r--r--   0 hestelles   (501) staff       (20)      710 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/examples/test_GW190521/test.json
--rw-r--r--   0 hestelles   (501) staff       (20)     8565 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/examples/test_GW190521/test.pdf
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.571720 pe-configurator-1.0.3/examples/test_GW190814/
--rw-r--r--   0 hestelles   (501) staff       (20)   844645 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/examples/test_GW190814/test.html
--rw-r--r--   0 hestelles   (501) staff       (20)      699 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/examples/test_GW190814/test.json
--rw-r--r--   0 hestelles   (501) staff       (20)     8839 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/examples/test_GW190814/test.pdf
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.572513 pe-configurator-1.0.3/examples/test_GW190814_fake_detchar_recommendation/
--rw-r--r--   0 hestelles   (501) staff       (20)   851571 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/examples/test_GW190814_fake_detchar_recommendation/test.html
--rw-r--r--   0 hestelles   (501) staff       (20)      762 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/examples/test_GW190814_fake_detchar_recommendation/test.json
--rw-r--r--   0 hestelles   (501) staff       (20)     9727 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/examples/test_GW190814_fake_detchar_recommendation/test.pdf
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.573344 pe-configurator-1.0.3/examples/test_GW191109/
--rw-r--r--   0 hestelles   (501) staff       (20)   846106 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/examples/test_GW191109/test.html
--rw-r--r--   0 hestelles   (501) staff       (20)      682 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/examples/test_GW191109/test.json
--rw-r--r--   0 hestelles   (501) staff       (20)     8663 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/examples/test_GW191109/test.pdf
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.575625 pe-configurator-1.0.3/pe_configurator.egg-info/
--rw-r--r--   0 hestelles   (501) staff       (20)    11764 2023-12-01 20:10:56.000000 pe-configurator-1.0.3/pe_configurator.egg-info/PKG-INFO
--rw-r--r--   0 hestelles   (501) staff       (20)     1725 2023-12-01 20:10:56.000000 pe-configurator-1.0.3/pe_configurator.egg-info/SOURCES.txt
--rw-r--r--   0 hestelles   (501) staff       (20)        1 2023-12-01 20:10:56.000000 pe-configurator-1.0.3/pe_configurator.egg-info/dependency_links.txt
--rw-r--r--   0 hestelles   (501) staff       (20)      142 2023-12-01 20:10:56.000000 pe-configurator-1.0.3/pe_configurator.egg-info/entry_points.txt
--rw-r--r--   0 hestelles   (501) staff       (20)      118 2023-12-01 20:10:56.000000 pe-configurator-1.0.3/pe_configurator.egg-info/requires.txt
--rw-r--r--   0 hestelles   (501) staff       (20)       15 2023-12-01 20:10:56.000000 pe-configurator-1.0.3/pe_configurator.egg-info/top_level.txt
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.574670 pe-configurator-1.0.3/peconfigurator/
--rw-r--r--   0 hestelles   (501) staff       (20)    11911 2023-12-01 20:03:46.000000 pe-configurator-1.0.3/peconfigurator/asimov.py
--rw-r--r--   0 hestelles   (501) staff       (20)       73 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/peconfigurator/asimov_template.yaml
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.575220 pe-configurator-1.0.3/peconfigurator/auxiliary/
--rw-r--r--   0 hestelles   (501) staff       (20)        0 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/peconfigurator/auxiliary/__init__.py
--rw-r--r--   0 hestelles   (501) staff       (20)    13191 2023-12-01 20:03:46.000000 pe-configurator-1.0.3/peconfigurator/auxiliary/make_report.py
--rw-r--r--   0 hestelles   (501) staff       (20)     5669 2023-12-01 20:03:46.000000 pe-configurator-1.0.3/peconfigurator/auxiliary/plotting.py
--rw-r--r--   0 hestelles   (501) staff       (20)    17933 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/peconfigurator/auxiliary/produce_fake_posteriors.ipynb
--rw-r--r--   0 hestelles   (501) staff       (20)     9685 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/peconfigurator/auxiliary/run_analyzer.py
--rwxr-xr-x   0 hestelles   (501) staff       (20)    10429 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/peconfigurator/get_settings.py
--rwxr-xr-x   0 hestelles   (501) staff       (20)    28221 2023-12-01 20:03:46.000000 pe-configurator-1.0.3/peconfigurator/proc_samples.py
--rw-r--r--   0 hestelles   (501) staff       (20)     2897 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/peconfigurator/run_on_many_events.py
--rw-r--r--   0 hestelles   (501) staff       (20)     1349 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/pyproject.toml
--rw-r--r--   0 hestelles   (501) staff       (20)       38 2023-12-01 20:10:56.577762 pe-configurator-1.0.3/setup.cfg
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.575346 pe-configurator-1.0.3/tests/
-drwxr-xr-x   0 hestelles   (501) staff       (20)        0 2023-12-01 20:10:56.575458 pe-configurator-1.0.3/tests/test_auxiliary/
--rw-r--r--   0 hestelles   (501) staff       (20)     1468 2023-12-01 20:03:46.000000 pe-configurator-1.0.3/tests/test_auxiliary/test_plotting.py
--rwxr-xr-x   0 hestelles   (501) staff       (20)     6016 2023-12-01 17:16:43.000000 pe-configurator-1.0.3/tests/test_get_settings.py
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:06.736513 pe_configurator-1.0.4/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     1349 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/.gitlab-ci.yml
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)      752 2024-05-24 10:25:02.000000 pe_configurator-1.0.4/CHANGELOG.md
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     1100 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/LICENSE
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)    11764 2024-05-24 10:36:06.000000 pe_configurator-1.0.4/PKG-INFO
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)    10809 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/README.md
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:05.000000 pe_configurator-1.0.4/blueprints/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)      192 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/blueprints/test.yaml
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:05.000000 pe_configurator-1.0.4/data/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)  2290335 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/data/calibration_files.txt
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:05.000000 pe_configurator-1.0.4/docs/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)      580 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/docs/Makefile
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     2402 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/docs/conf.py
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)      653 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/docs/index.rst
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:05.000000 pe_configurator-1.0.4/docs/source/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     8634 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/docs/source/examples.rst
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:05.000000 pe_configurator-1.0.4/docs/source/images/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)    63225 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/docs/source/images/MECO_gw190521.png
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)   130355 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/docs/source/images/fake_chirpmass_railing.png
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)   121175 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/docs/source/images/fake_mass_ratio_rail_low.png
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     1299 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/docs/source/installation.rst
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)    12337 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/docs/source/logic.md
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)    10258 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/docs/source/logic.rst
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:05.000000 pe_configurator-1.0.4/docs/templates/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)      639 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/docs/templates/custom-class-template.rst
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     1465 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/docs/templates/custom-module-template.rst
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:05.000000 pe_configurator-1.0.4/examples/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     8196 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/examples/.DS_Store
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:06.000000 pe_configurator-1.0.4/examples/test_GW190412/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)   821276 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/examples/test_GW190412/test.html
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)      669 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/examples/test_GW190412/test.json
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     8592 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/examples/test_GW190412/test.pdf
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:06.124490 pe_configurator-1.0.4/examples/test_GW190521/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)   822260 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/examples/test_GW190521/test.html
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)      710 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/examples/test_GW190521/test.json
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     8565 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/examples/test_GW190521/test.pdf
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:06.288497 pe_configurator-1.0.4/examples/test_GW190814/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)   844645 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/examples/test_GW190814/test.html
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)      699 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/examples/test_GW190814/test.json
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     8839 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/examples/test_GW190814/test.pdf
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:06.432502 pe_configurator-1.0.4/examples/test_GW190814_fake_detchar_recommendation/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)   851571 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/examples/test_GW190814_fake_detchar_recommendation/test.html
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)      762 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/examples/test_GW190814_fake_detchar_recommendation/test.json
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     9727 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/examples/test_GW190814_fake_detchar_recommendation/test.pdf
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:06.540506 pe_configurator-1.0.4/examples/test_GW191109/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)   846106 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/examples/test_GW191109/test.html
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)      682 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/examples/test_GW191109/test.json
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     8663 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/examples/test_GW191109/test.pdf
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:06.600508 pe_configurator-1.0.4/pe_configurator.egg-info/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)    11764 2024-05-24 10:36:04.000000 pe_configurator-1.0.4/pe_configurator.egg-info/PKG-INFO
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     1725 2024-05-24 10:36:05.000000 pe_configurator-1.0.4/pe_configurator.egg-info/SOURCES.txt
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)        1 2024-05-24 10:36:04.000000 pe_configurator-1.0.4/pe_configurator.egg-info/dependency_links.txt
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)      142 2024-05-24 10:36:04.000000 pe_configurator-1.0.4/pe_configurator.egg-info/entry_points.txt
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)      118 2024-05-24 10:36:04.000000 pe_configurator-1.0.4/pe_configurator.egg-info/requires.txt
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)       15 2024-05-24 10:36:04.000000 pe_configurator-1.0.4/pe_configurator.egg-info/top_level.txt
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:06.640510 pe_configurator-1.0.4/peconfigurator/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)    11911 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/peconfigurator/asimov.py
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)       73 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/peconfigurator/asimov_template.yaml
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:06.692512 pe_configurator-1.0.4/peconfigurator/auxiliary/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)        0 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/peconfigurator/auxiliary/__init__.py
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)    13191 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/peconfigurator/auxiliary/make_report.py
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     5669 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/peconfigurator/auxiliary/plotting.py
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)    17933 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/peconfigurator/auxiliary/produce_fake_posteriors.ipynb
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     9685 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/peconfigurator/auxiliary/run_analyzer.py
+-rwxr-xr-x   0 hestelles  (3651) cluster   (1111)    10789 2024-05-24 10:17:48.000000 pe_configurator-1.0.4/peconfigurator/get_settings.py
+-rwxr-xr-x   0 hestelles  (3651) cluster   (1111)    29159 2024-05-24 10:17:48.000000 pe_configurator-1.0.4/peconfigurator/proc_samples.py
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     2897 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/peconfigurator/run_on_many_events.py
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     1349 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/pyproject.toml
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)       38 2024-05-24 10:36:06.000000 pe_configurator-1.0.4/setup.cfg
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:06.696512 pe_configurator-1.0.4/tests/
+drwxr-xr-x   0 hestelles  (3651) cluster   (1111)        0 2024-05-24 10:36:06.712513 pe_configurator-1.0.4/tests/test_auxiliary/
+-rw-r--r--   0 hestelles  (3651) cluster   (1111)     1468 2024-05-16 18:01:19.000000 pe_configurator-1.0.4/tests/test_auxiliary/test_plotting.py
+-rwxr-xr-x   0 hestelles  (3651) cluster   (1111)     6363 2024-05-24 10:17:48.000000 pe_configurator-1.0.4/tests/test_get_settings.py
```

### Comparing `pe-configurator-1.0.3/.gitlab-ci.yml` & `pe_configurator-1.0.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/LICENSE` & `pe_configurator-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/PKG-INFO` & `pe_configurator-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe-configurator
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tools to identify waveform settings and prior bounds for gravitational wave parameter estimation.
 Author-email: Hector Estelles <hector.estelles@ligo.org>, Serguei Ossokine <serguei.ossokine@ligo.org>, Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/pe/get_eob_settings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pe-configurator-1.0.3/README.md` & `pe_configurator-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/data/calibration_files.txt` & `pe_configurator-1.0.4/data/calibration_files.txt`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/docs/Makefile` & `pe_configurator-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/docs/conf.py` & `pe_configurator-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/docs/index.rst` & `pe_configurator-1.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/docs/source/examples.rst` & `pe_configurator-1.0.4/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/docs/source/images/MECO_gw190521.png` & `pe_configurator-1.0.4/docs/source/images/MECO_gw190521.png`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/docs/source/images/fake_chirpmass_railing.png` & `pe_configurator-1.0.4/docs/source/images/fake_chirpmass_railing.png`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/docs/source/images/fake_mass_ratio_rail_low.png` & `pe_configurator-1.0.4/docs/source/images/fake_mass_ratio_rail_low.png`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/docs/source/installation.rst` & `pe_configurator-1.0.4/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/docs/source/logic.md` & `pe_configurator-1.0.4/docs/source/logic.md`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/docs/source/logic.rst` & `pe_configurator-1.0.4/docs/source/logic.rst`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/docs/templates/custom-class-template.rst` & `pe_configurator-1.0.4/docs/templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/docs/templates/custom-module-template.rst` & `pe_configurator-1.0.4/docs/templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/examples/.DS_Store` & `pe_configurator-1.0.4/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/examples/test_GW190412/test.html` & `pe_configurator-1.0.4/examples/test_GW190412/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/examples/test_GW190412/test.json` & `pe_configurator-1.0.4/examples/test_GW190412/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/examples/test_GW190412/test.pdf` & `pe_configurator-1.0.4/examples/test_GW190412/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/examples/test_GW190521/test.html` & `pe_configurator-1.0.4/examples/test_GW190521/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/examples/test_GW190521/test.json` & `pe_configurator-1.0.4/examples/test_GW190521/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/examples/test_GW190521/test.pdf` & `pe_configurator-1.0.4/examples/test_GW190521/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/examples/test_GW190814/test.html` & `pe_configurator-1.0.4/examples/test_GW190814/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/examples/test_GW190814/test.json` & `pe_configurator-1.0.4/examples/test_GW190814/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/examples/test_GW190814/test.pdf` & `pe_configurator-1.0.4/examples/test_GW190814/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/examples/test_GW190814_fake_detchar_recommendation/test.html` & `pe_configurator-1.0.4/examples/test_GW190814_fake_detchar_recommendation/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/examples/test_GW190814_fake_detchar_recommendation/test.json` & `pe_configurator-1.0.4/examples/test_GW190814_fake_detchar_recommendation/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/examples/test_GW190814_fake_detchar_recommendation/test.pdf` & `pe_configurator-1.0.4/examples/test_GW190814_fake_detchar_recommendation/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/examples/test_GW191109/test.html` & `pe_configurator-1.0.4/examples/test_GW191109/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/examples/test_GW191109/test.json` & `pe_configurator-1.0.4/examples/test_GW191109/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/examples/test_GW191109/test.pdf` & `pe_configurator-1.0.4/examples/test_GW191109/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/pe_configurator.egg-info/PKG-INFO` & `pe_configurator-1.0.4/pe_configurator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe-configurator
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tools to identify waveform settings and prior bounds for gravitational wave parameter estimation.
 Author-email: Hector Estelles <hector.estelles@ligo.org>, Serguei Ossokine <serguei.ossokine@ligo.org>, Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/pe/get_eob_settings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pe-configurator-1.0.3/pe_configurator.egg-info/SOURCES.txt` & `pe_configurator-1.0.4/pe_configurator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/peconfigurator/asimov.py` & `pe_configurator-1.0.4/peconfigurator/asimov.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/peconfigurator/auxiliary/make_report.py` & `pe_configurator-1.0.4/peconfigurator/auxiliary/make_report.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/peconfigurator/auxiliary/plotting.py` & `pe_configurator-1.0.4/peconfigurator/auxiliary/plotting.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/peconfigurator/auxiliary/produce_fake_posteriors.ipynb` & `pe_configurator-1.0.4/peconfigurator/auxiliary/produce_fake_posteriors.ipynb`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/peconfigurator/auxiliary/run_analyzer.py` & `pe_configurator-1.0.4/peconfigurator/auxiliary/run_analyzer.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/peconfigurator/get_settings.py` & `pe_configurator-1.0.4/peconfigurator/get_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     return fmeco
 
 
 def estimate_seglen(
     fLow: float,
     m_total_min: float,
     safety_factor: float = 0.03,
+    tukey_window_rollon: float = 1.0,
+    post_trigger_duration: float = 2.0,
     q: float = 5.0,
     chi1z: float = 0.99,
     chi2z: float = 0.99,
 ) -> Tuple[float]:
     """Estimate the required segment length. By default uses the SEOBNRv4ROM
     function + some additional esimtate of the length of the ringdown. Assumes
     a 0.4 second roll-on plus 2 second pad.
@@ -72,15 +74,15 @@
     except:
         wf_len = LS.SimIMRPhenomXASDuration(m1, m2, chi1z, chi2z, fLow)
 
 
     wf_len += tmerge
     # Make the waveform slightly longer just for safety
     safe_len = wf_len * (1.0 + safety_factor)
-    full_len = safe_len + 2 + 0.4  # Padding and roll-on
+    full_len = safe_len + post_trigger_duration + tukey_window_rollon  # Padding and roll-on
     seglen = 2 ** (np.floor(np.log2(full_len)) + 1)  # Next power  of 2
     return safe_len, full_len, seglen
 
 
 def next_power_of_2(x):
     return 1 if x == 0 else 2 ** (x - 1).bit_length()
 
@@ -240,14 +242,20 @@
 
     p.add_argument(
         "--ell_max",
         type=int,
         help="Max ell for Nyquist check when HM enabled",
         default=3,
     )
+    p.add_argument(
+        "--tukey_window_rollon",
+        type=float,
+        help="Time for the Tukey window applied during data conditioning.",
+        default=1.0,
+    )
     args = p.parse_args()
     amp_order, freq, hm_dominated = get_amp_order(
         args.m_total_max, args.f_low, HM=args.HM, m_HM=args.ell_max,
     )
 
     # Print summary
     click.echo("#" * 30 + " SUMMARY " + 30 * "#")
@@ -291,20 +299,20 @@
     print(
         "The minimum sampling rate to use is {}, the next power of two is {}".format(
             srate_min, srate_min_next_pow_2
         )
     )
     if args.estimate_seglen:
         wf_length, length_estimate, seglen = estimate_seglen(
-            args.f_low, args.m_total_min, q=args.mass_ratio
+            args.f_low, args.m_total_min,tukey_window_rollon=args.tukey_window_rollon, q=args.mass_ratio
         )
         print(
             "Estimated length of waveform starting at fLow={}: {} sec".format(
                 args.f_low, wf_length
             )
         )
         print(
-            "Total length,including 2 sec padding + 0.4 sec tapering: {} sec".format(
-                length_estimate
+            "Total length,including 2 sec padding + {} sec tapering: {} sec".format(
+                args.tukey_window_rollon, length_estimate
             )
         )
         print("Recommended seglen: {} sec".format(seglen))
```

### Comparing `pe-configurator-1.0.3/peconfigurator/proc_samples.py` & `pe_configurator-1.0.4/peconfigurator/proc_samples.py`

 * *Files 7% similar despite different names*

```diff
@@ -222,14 +222,26 @@
     parser.add_argument(
         "--detchar_seglen",
         type=float,
         help="Maximum segment length allowed by detchar analysis. If provided, seglen recommendations above this value will be ignored.",
         default=-1,
     )
     parser.add_argument(
+        "--tukey_window_rollon",
+        type=float,
+        help="Time for the Tukey window applied during data conditioning.",
+        default=1.0,
+    )
+    parser.add_argument(
+        "--post_trigger_duration",
+        type=float,
+        help="Time for post-trigger duration.",
+        default=2.0,
+    )
+    parser.add_argument(
         "--enforce_ellmax",
         action="store_true",
         help="Enforce that the input ell-max is employed, regardless of the mass of the system",
     )
     parser.add_argument("--legacy",action="store_true",help="If true, f_start takes into account EOB limitations. Note that for high total mass if the segment length is based on f_start, this may result in very long segments. **Use with caution**")
     args = parser.parse_args()
 
@@ -393,15 +405,15 @@
 
     click.echo("Estimating seglen based on posterior samples")
 
     # seglen section
     # Compute the seglen from the actual samples
     safelens, fulllens, seglens = zip(
         *[
-            estimate_seglen(f_start, mt, q=1.0 / qp, chi1z=s1z, chi2z=s2z)
+            estimate_seglen(f_start, mt, tukey_window_rollon=args.tukey_window_rollon, post_trigger_duration=args.post_trigger_duration, q=1.0 / qp, chi1z=s1z, chi2z=s2z)
             for mt, qp, s1z, s2z in tqdm(list(zip(mtot, q, chi1z, chi2z)))
         ]
     )
     nopad_len = np.max(safelens)
     max_seglen = np.max(seglens)
 
     # Compute a conservative estimate for seglen
@@ -414,14 +426,16 @@
     q_max = q[idx_max]
     eta_max = eta_from_q(q_max)
     # Given the lower bound of recommended chirp mass compute the corresponding total mass
     mt_lower_bound = mt_from_eta_mc(eta_max, chirpmass_min_bound)
     nopad, full, pof2 = estimate_seglen(
         f_start,
         mt_lower_bound,
+        tukey_window_rollon=args.tukey_window_rollon,
+        post_trigger_duration=args.post_trigger_duration,
         q=1 / q_max,
         chi1z=chi1z[idx_max],
         chi2z=chi2z[idx_max],
     )
     # Store the actual value we computed for logging
     pof2_log = pof2
 
@@ -446,25 +460,29 @@
             detchar_checks["consistent_seglen"] = False
 
             # Input minimum might be incompatible with new recommended segment length
             # Find if this is the case and report a new recommended minimum frequency
             _, _, aux_pof2 = estimate_seglen(
                 f_start,
                 mt_lower_bound,
+                tukey_window_rollon=args.tukey_window_rollon,
+                post_trigger_duration=args.post_trigger_duration,
                 q=1 / q_max,
                 chi1z=0.99,
                 chi2z=0.99,
             )
             while aux_pof2 > pof2:
                 f_start = (
                     f_start + 0.05
                 )  # We increment total mass until we find an allowed value
                 _, _, aux_pof2 = estimate_seglen(
                     f_start,
                     mt_lower_bound,
+                    tukey_window_rollon=args.tukey_window_rollon,
+                    post_trigger_duration=args.post_trigger_duration,
                     q=1 / q_max,
                     chi1z=0.99,
                     chi2z=0.99,
                 )
 
             # Overwrite f_start for this special case.
             if flow_aux < f_start:
@@ -632,14 +650,16 @@
         else:
             # f_start wasn't forced
             # Recompute the segment length from f_ref
 
             nopad_aux, full_aux, aux_pof2 = estimate_seglen(
                 f_ref,
                 mt_lower_bound,
+                tukey_window_rollon=args.tukey_window_rollon,
+                post_trigger_duration=args.post_trigger_duration,
                 q=1 / q_max,
                 chi1z=0.99,
                 chi2z=0.99,
             )
             # Check if the new segment length is longer than the detchar seglen
             # If it is, that means we can't start at f_low, overwrite f_ref
             # to f_start
@@ -670,15 +690,15 @@
     # Write the suggested settings to the log
     click.echo()
     click.echo(30 * "+" + " Suggested settings " + 30 * "+")
     # Sampling rate
     click.echo(f"Real required srate  {max_real_rate}, as power of 2: {max_srate}")
 
     # Segment length
-    seglen_msg = f"Real seglen: {nopad}, with padding+rollon: {full}, as power of 2: {pof2_log}"
+    seglen_msg = f"Real seglen: {nopad}, with padding + rollon: {full}, as power of 2: {pof2_log}"
     # Take into account detchar recommendation
     if pof2_log > pof2:
         seglen_msg += f" overwritten by detchar recommendation to {pof2}"
 
     click.echo(seglen_msg)
     click.echo("Check from samples:")
     click.echo(
```

### Comparing `pe-configurator-1.0.3/peconfigurator/run_on_many_events.py` & `pe_configurator-1.0.4/peconfigurator/run_on_many_events.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/pyproject.toml` & `pe_configurator-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/tests/test_auxiliary/test_plotting.py` & `pe_configurator-1.0.4/tests/test_auxiliary/test_plotting.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-1.0.3/tests/test_get_settings.py` & `pe_configurator-1.0.4/tests/test_get_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             + 1.0593147376898773 * x2
             - 0.06378640753152783 * x4
         )
     res = lalsim.SimIMRPhenomXUtilsMftoHz(fring_tmp, m1 + m2) / (1.0 - erad)
     return res
 
 
-def manual_seglen(m1, m2, chi1z, chi2z, flow):
+def manual_seglen(m1, m2, chi1z, chi2z, flow, tukey_window_rollon, post_trigger_duration):
     """Compute the seglen by the following procedure:
     1. Actually evolve SEOBNRv4_opt in time domain
     2. Check that the seglen that we return is strictly greater than what
     we got in step 1.
     """
     distance = 400 * 1e6 * lal.PC_SI
     iota = 0.0
@@ -92,15 +92,15 @@
         delta_t,
         flow,
         flow,
         lal.CreateDict(),
         lalsim.GetApproximantFromString("SEOBNRv4_opt"),
     )
     duration = len(hp.data.data) * delta_t
-    with_rollon = duration + 2.4
+    with_rollon = duration + post_trigger_duration + tukey_window_rollon
     seglen = 2 ** (np.floor(np.log2(with_rollon)) + 1)  # Next power  of 2
     return duration, with_rollon, seglen
 
 
 @pytest.mark.parametrize(
     "m_total,HM,m_HM,expected",
     [
@@ -124,29 +124,29 @@
     assert np.allclose(f_start, expected[1], rtol=2e-2), "f_start was not correct!"
 
 
 @pytest.mark.skipif(
     "LAL_DATA_PATH" not in os.environ, reason="LAL_DATA_PATH not found",
 )
 @pytest.mark.parametrize(
-    "m1,m2,chi1z,chi2z,flow",
+    "m1,m2,chi1z,chi2z,flow,tukey_window_rollon,post_trigger_duration",
     [
-        (40.0, 20.0, 0.8, 0.8, 20.0),
-        (40.0, 20.0, -0.99, -0.99, 20.0),
-        (40.0, 20.0, 0.8, 0.8, 10.0),
-        (80.0, 20.0, 0.99, -0.8, 10.0),
-        (300.0, 50.0, 0.99, 0.8, 10.0),
+        (40.0, 20.0, 0.8, 0.8, 20.0, 1.0, 2.0),
+        (40.0, 20.0, -0.99, -0.99, 20.0, 1.0, 2.0),
+        (40.0, 20.0, 0.8, 0.8, 10.0, 1.0, 2.0),
+        (80.0, 20.0, 0.99, -0.8, 10.0, 1.0, 2.0),
+        (300.0, 50.0, 0.99, 0.8, 10.0, 1.0, 2.0),
     ],
 )
-def test_estimate_seglen(m1, m2, chi1z, chi2z, flow):
+def test_estimate_seglen(m1, m2, chi1z, chi2z, flow, tukey_window_rollon,post_trigger_duration):
     """ Test that the seglen is correct. This is done
     by comparing to an independent estimate of the seglen"""
-    duration, roll_on, seglen_check = manual_seglen(m1, m2, chi1z, chi2z, flow)
+    duration, roll_on, seglen_check = manual_seglen(m1, m2, chi1z, chi2z, flow, tukey_window_rollon,post_trigger_duration)
     full_len, with_pad, seglen = estimate_seglen(
-        flow, m1 + m2, safety_factor=0.03, q=m1 / m2, chi1z=chi1z, chi2z=chi2z
+        flow, m1 + m2, safety_factor=0.03, tukey_window_rollon=tukey_window_rollon,post_trigger_duration=post_trigger_duration, q=m1 / m2, chi1z=chi1z, chi2z=chi2z
     )
     assert np.allclose(seglen, seglen_check), "seg lengths are not the same"
     assert np.allclose(
         full_len, duration, rtol=1e-1
     ), "Estimated durations differ by more than 10 %"
```

