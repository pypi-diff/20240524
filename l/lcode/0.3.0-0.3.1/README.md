# Comparing `tmp/lcode-0.3.0.tar.gz` & `tmp/lcode-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcode-0.3.0.tar", last modified: Tue May 14 08:10:11 2024, max compression
+gzip compressed data, was "lcode-0.3.1.tar", last modified: Fri May 24 16:18:36 2024, max compression
```

## Comparing `lcode-0.3.0.tar` & `lcode-0.3.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.843410 lcode-0.3.0/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     2200 2024-03-12 08:52:48.000000 lcode-0.3.0/LICENSE
--rw-r--r--   0 tuev      (1000) tuev      (1000)     2543 2024-05-14 08:10:11.839410 lcode-0.3.0/PKG-INFO
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1702 2024-05-14 06:32:26.000000 lcode-0.3.0/README.md
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.815409 lcode-0.3.0/lcode/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      142 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1288 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/__main__.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.819409 lcode-0.3.0/lcode/alt_beam_generator/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)        0 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/alt_beam_generator/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     7164 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/alt_beam_generator/beam_generator.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     2470 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/alt_beam_generator/beam_segment_shape.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1458 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/alt_beam_generator/beam_shape.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1756 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/alt_beam_generator/eshape.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     2334 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/alt_beam_generator/rshape.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1496 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/alt_beam_generator/xishape.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.823409 lcode-0.3.0/lcode/beam/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      259 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    18315 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/beam/beam_calculate.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     5729 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/beam/beam_io.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     5580 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/beam/data.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)        0 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam/profiles.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     2232 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam/weights.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.827410 lcode-0.3.0/lcode/beam3d/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      382 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam3d/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     7022 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/beam3d/beam_calculator.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     3329 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/beam3d/beam_io.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     7220 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam3d/data.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    12891 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/beam3d/move.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     5112 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/beam3d/weights.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.827410 lcode-0.3.0/lcode/beam_generator/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)       31 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam_generator/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     4901 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam_generator/beam_generator.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     6595 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam_generator/beam_generator2.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     6379 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/beam_generator/beam_profiles.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.831410 lcode-0.3.0/lcode/config/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)       27 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/config/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    10536 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/config/config.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      157 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/config/default_config.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     3296 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/config/default_config_values.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     3222 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/config/template.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.835409 lcode-0.3.0/lcode/diagnostics/
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.835409 lcode-0.3.0/lcode/diagnostics/FXi/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     5332 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/FXi/FXi.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      466 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/FXi/Strategy.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     3928 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/FXi/Strategy3D.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     2148 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/FXi/StrategyCircular.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)       35 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/FXi/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      154 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    33325 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/diagnostics_3d.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      464 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/diagnostics/diagnostics_class.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     2320 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/diagnostics/diagnostics_list.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     4115 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/particles.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      120 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/diagnostics/process.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    19254 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/slice.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     7654 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/targets.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1790 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/diagnostics/utils.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.835409 lcode-0.3.0/lcode/examples/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     9778 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/examples/high-R.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1196 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/examples/original-ssm.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.835409 lcode-0.3.0/lcode/mpi/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)       74 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/mpi/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     4077 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/mpi/beam_io.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1860 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/mpi/transport.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1646 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/mpi/util.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.839410 lcode-0.3.0/lcode/plasma/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      115 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/plasma/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1287 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma/data.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     8303 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma/fields.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     4499 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma/initialization.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     7970 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma/move.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     2450 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/plasma/ode.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     4711 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma/profiles.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     4641 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma/rhoj.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     3822 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma/solver.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.839410 lcode-0.3.0/lcode/plasma3d/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      115 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/plasma3d/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1292 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma3d/data.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    13022 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma3d/fields.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    20487 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma3d/initialization.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    14630 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma3d/move.py
--rwxrwxr-x   0 tuev      (1000) tuev      (1000)    11495 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma3d/noise_filter.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     5942 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma3d/profile.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)      748 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/plasma3d/rhoj.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     3002 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma3d/solver.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    11309 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/plasma3d/weights.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.839410 lcode-0.3.0/lcode/push_solvers/
--rw-rw-r--   0 tuev      (1000) tuev      (1000)        0 2024-03-12 08:52:48.000000 lcode-0.3.0/lcode/push_solvers/__init__.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    11080 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/push_solvers/push_solver.py
--rw-rw-r--   0 tuev      (1000) tuev      (1000)    11311 2024-05-14 06:32:26.000000 lcode-0.3.0/lcode/simulation.py
-drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-14 08:10:11.815409 lcode-0.3.0/lcode.egg-info/
--rw-r--r--   0 tuev      (1000) tuev      (1000)     2543 2024-05-14 08:10:11.000000 lcode-0.3.0/lcode.egg-info/PKG-INFO
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     2213 2024-05-14 08:10:11.000000 lcode-0.3.0/lcode.egg-info/SOURCES.txt
--rw-rw-r--   0 tuev      (1000) tuev      (1000)        1 2024-05-14 08:10:11.000000 lcode-0.3.0/lcode.egg-info/dependency_links.txt
--rw-rw-r--   0 tuev      (1000) tuev      (1000)       36 2024-05-14 08:10:11.000000 lcode-0.3.0/lcode.egg-info/requires.txt
--rw-rw-r--   0 tuev      (1000) tuev      (1000)        6 2024-05-14 08:10:11.000000 lcode-0.3.0/lcode.egg-info/top_level.txt
--rw-rw-r--   0 tuev      (1000) tuev      (1000)       38 2024-05-14 08:10:11.843410 lcode-0.3.0/setup.cfg
--rw-rw-r--   0 tuev      (1000) tuev      (1000)     1534 2024-05-14 06:32:26.000000 lcode-0.3.0/setup.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-24 16:18:36.368404 lcode-0.3.1/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     2200 2024-03-12 08:52:48.000000 lcode-0.3.1/LICENSE
+-rw-r--r--   0 tuev      (1000) tuev      (1000)     2543 2024-05-24 16:18:36.368404 lcode-0.3.1/PKG-INFO
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1702 2024-05-14 06:32:26.000000 lcode-0.3.1/README.md
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-24 16:18:36.360404 lcode-0.3.1/lcode/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      142 2024-05-24 16:18:24.000000 lcode-0.3.1/lcode/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1288 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/__main__.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-24 16:18:36.364404 lcode-0.3.1/lcode/alt_beam_generator/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)        0 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/alt_beam_generator/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     7164 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/alt_beam_generator/beam_generator.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     2470 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/alt_beam_generator/beam_segment_shape.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1458 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/alt_beam_generator/beam_shape.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1756 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/alt_beam_generator/eshape.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     2334 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/alt_beam_generator/rshape.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1496 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/alt_beam_generator/xishape.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-24 16:18:36.364404 lcode-0.3.1/lcode/beam/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      259 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/beam/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    18315 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/beam/beam_calculate.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     5729 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/beam/beam_io.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     5580 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/beam/data.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)        0 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/beam/profiles.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     2232 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/beam/weights.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-24 16:18:36.364404 lcode-0.3.1/lcode/beam3d/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      382 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/beam3d/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     7022 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/beam3d/beam_calculator.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     3329 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/beam3d/beam_io.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     7220 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/beam3d/data.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    12891 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/beam3d/move.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     5112 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/beam3d/weights.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-24 16:18:36.364404 lcode-0.3.1/lcode/beam_generator/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)       31 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/beam_generator/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     4901 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/beam_generator/beam_generator.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     6595 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/beam_generator/beam_generator2.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     6379 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/beam_generator/beam_profiles.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-24 16:18:36.364404 lcode-0.3.1/lcode/config/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)       27 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/config/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    10536 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/config/config.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      157 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/config/default_config.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     3296 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/config/default_config_values.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     3222 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/config/template.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-24 16:18:36.364404 lcode-0.3.1/lcode/diagnostics/
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-24 16:18:36.364404 lcode-0.3.1/lcode/diagnostics/FXi/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     5332 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/diagnostics/FXi/FXi.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      466 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/diagnostics/FXi/Strategy.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     3928 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/diagnostics/FXi/Strategy3D.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     2148 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/diagnostics/FXi/StrategyCircular.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)       35 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/diagnostics/FXi/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      154 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/diagnostics/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    33325 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/diagnostics/diagnostics_3d.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      464 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/diagnostics/diagnostics_class.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     2320 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/diagnostics/diagnostics_list.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     4115 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/diagnostics/particles.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      120 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/diagnostics/process.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    19254 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/diagnostics/slice.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     7654 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/diagnostics/targets.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1790 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/diagnostics/utils.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-24 16:18:36.364404 lcode-0.3.1/lcode/examples/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     9778 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/examples/high-R.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1196 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/examples/original-ssm.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-24 16:18:36.364404 lcode-0.3.1/lcode/mpi/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)       74 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/mpi/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     4077 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/mpi/beam_io.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1860 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/mpi/transport.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1646 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/mpi/util.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-24 16:18:36.364404 lcode-0.3.1/lcode/plasma/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      115 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/plasma/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1287 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/plasma/data.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     8303 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/plasma/fields.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     4499 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/plasma/initialization.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     7970 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/plasma/move.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     2450 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/plasma/ode.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     4711 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/plasma/profiles.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     4641 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/plasma/rhoj.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     3822 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/plasma/solver.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-24 16:18:36.368404 lcode-0.3.1/lcode/plasma3d/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      115 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/plasma3d/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1292 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/plasma3d/data.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    13022 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/plasma3d/fields.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    20487 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/plasma3d/initialization.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    14630 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/plasma3d/move.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    11139 2024-05-24 16:18:24.000000 lcode-0.3.1/lcode/plasma3d/noise_filter.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     5942 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/plasma3d/profile.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)      748 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/plasma3d/rhoj.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     3002 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/plasma3d/solver.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    11309 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/plasma3d/weights.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-24 16:18:36.368404 lcode-0.3.1/lcode/push_solvers/
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)        0 2024-03-12 08:52:48.000000 lcode-0.3.1/lcode/push_solvers/__init__.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    11080 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/push_solvers/push_solver.py
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)    11311 2024-05-14 06:32:26.000000 lcode-0.3.1/lcode/simulation.py
+drwxrwxr-x   0 tuev      (1000) tuev      (1000)        0 2024-05-24 16:18:36.360404 lcode-0.3.1/lcode.egg-info/
+-rw-r--r--   0 tuev      (1000) tuev      (1000)     2543 2024-05-24 16:18:36.000000 lcode-0.3.1/lcode.egg-info/PKG-INFO
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     2213 2024-05-24 16:18:36.000000 lcode-0.3.1/lcode.egg-info/SOURCES.txt
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)        1 2024-05-24 16:18:36.000000 lcode-0.3.1/lcode.egg-info/dependency_links.txt
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)       36 2024-05-24 16:18:36.000000 lcode-0.3.1/lcode.egg-info/requires.txt
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)        6 2024-05-24 16:18:36.000000 lcode-0.3.1/lcode.egg-info/top_level.txt
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)       38 2024-05-24 16:18:36.368404 lcode-0.3.1/setup.cfg
+-rw-rw-r--   0 tuev      (1000) tuev      (1000)     1534 2024-05-14 06:32:26.000000 lcode-0.3.1/setup.py
```

### Comparing `lcode-0.3.0/LICENSE` & `lcode-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/PKG-INFO` & `lcode-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcode
-Version: 0.3.0
+Version: 0.3.1
 Summary: LCODE is a free software for simulationplasma wakefield acceleration based on QSA.
 Home-page: https://lcode.info
 Download-URL: https://github.com/lcodePy-team/lcodePy
 Author: lcodePy-team
 Author-email: team@lcode.info
 License: BSD-3-Clause-extended
 Keywords: plasma wakefield acceleration,quasistatic approximation,numerical simulation
```

### Comparing `lcode-0.3.0/README.md` & `lcode-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/__main__.py` & `lcode-0.3.1/lcode/__main__.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/alt_beam_generator/beam_generator.py` & `lcode-0.3.1/lcode/alt_beam_generator/beam_generator.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/alt_beam_generator/beam_segment_shape.py` & `lcode-0.3.1/lcode/alt_beam_generator/beam_segment_shape.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/alt_beam_generator/beam_shape.py` & `lcode-0.3.1/lcode/alt_beam_generator/beam_shape.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/alt_beam_generator/eshape.py` & `lcode-0.3.1/lcode/alt_beam_generator/eshape.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/alt_beam_generator/rshape.py` & `lcode-0.3.1/lcode/alt_beam_generator/rshape.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/alt_beam_generator/xishape.py` & `lcode-0.3.1/lcode/alt_beam_generator/xishape.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/beam/beam_calculate.py` & `lcode-0.3.1/lcode/beam/beam_calculate.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/beam/beam_io.py` & `lcode-0.3.1/lcode/beam/beam_io.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/beam/data.py` & `lcode-0.3.1/lcode/beam/data.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/beam/weights.py` & `lcode-0.3.1/lcode/beam/weights.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/beam3d/beam_calculator.py` & `lcode-0.3.1/lcode/beam3d/beam_calculator.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/beam3d/beam_io.py` & `lcode-0.3.1/lcode/beam3d/beam_io.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/beam3d/data.py` & `lcode-0.3.1/lcode/beam3d/data.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/beam3d/move.py` & `lcode-0.3.1/lcode/beam3d/move.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/beam3d/weights.py` & `lcode-0.3.1/lcode/beam3d/weights.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/beam_generator/beam_generator.py` & `lcode-0.3.1/lcode/beam_generator/beam_generator.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/beam_generator/beam_generator2.py` & `lcode-0.3.1/lcode/beam_generator/beam_generator2.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/beam_generator/beam_profiles.py` & `lcode-0.3.1/lcode/beam_generator/beam_profiles.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/config/config.py` & `lcode-0.3.1/lcode/config/config.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/config/default_config_values.py` & `lcode-0.3.1/lcode/config/default_config_values.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/config/template.py` & `lcode-0.3.1/lcode/config/template.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/diagnostics/FXi/FXi.py` & `lcode-0.3.1/lcode/diagnostics/FXi/FXi.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/diagnostics/FXi/Strategy3D.py` & `lcode-0.3.1/lcode/diagnostics/FXi/Strategy3D.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/diagnostics/FXi/StrategyCircular.py` & `lcode-0.3.1/lcode/diagnostics/FXi/StrategyCircular.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/diagnostics/diagnostics_3d.py` & `lcode-0.3.1/lcode/diagnostics/diagnostics_3d.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/diagnostics/diagnostics_list.py` & `lcode-0.3.1/lcode/diagnostics/diagnostics_list.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/diagnostics/particles.py` & `lcode-0.3.1/lcode/diagnostics/particles.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/diagnostics/slice.py` & `lcode-0.3.1/lcode/diagnostics/slice.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/diagnostics/targets.py` & `lcode-0.3.1/lcode/diagnostics/targets.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/diagnostics/utils.py` & `lcode-0.3.1/lcode/diagnostics/utils.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/examples/high-R.py` & `lcode-0.3.1/lcode/examples/high-R.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/examples/original-ssm.py` & `lcode-0.3.1/lcode/examples/original-ssm.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/mpi/beam_io.py` & `lcode-0.3.1/lcode/mpi/beam_io.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/mpi/transport.py` & `lcode-0.3.1/lcode/mpi/transport.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/mpi/util.py` & `lcode-0.3.1/lcode/mpi/util.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/plasma/data.py` & `lcode-0.3.1/lcode/plasma/data.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/plasma/fields.py` & `lcode-0.3.1/lcode/plasma/fields.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/plasma/initialization.py` & `lcode-0.3.1/lcode/plasma/initialization.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/plasma/move.py` & `lcode-0.3.1/lcode/plasma/move.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/plasma/ode.py` & `lcode-0.3.1/lcode/plasma/ode.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/plasma/profiles.py` & `lcode-0.3.1/lcode/plasma/profiles.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/plasma/rhoj.py` & `lcode-0.3.1/lcode/plasma/rhoj.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/plasma/solver.py` & `lcode-0.3.1/lcode/plasma/solver.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/plasma3d/data.py` & `lcode-0.3.1/lcode/plasma3d/data.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/plasma3d/fields.py` & `lcode-0.3.1/lcode/plasma3d/fields.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/plasma3d/initialization.py` & `lcode-0.3.1/lcode/plasma3d/initialization.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/plasma3d/move.py` & `lcode-0.3.1/lcode/plasma3d/move.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/plasma3d/noise_filter.py` & `lcode-0.3.1/lcode/plasma3d/noise_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,50 +3,56 @@
 import numba as nb
 from ..config.config import Config
 from .data import Arrays
 
 
 def get_inhomogeneity_calculator_cupy(config):
     cp = config.xp
-    calculate_inhomoginity_kernel = cp.RawKernel(r'''
-        extern "C" __global__
-        void calculate_inhomoginity_kernel(const float* d_offt, float* d_inhom
-                                           int size){
-            int i = blockDim.x * blockIdx.x + threadIdx.x;
-            int j = blockDim.y * blockIdx.y + threadIdx.y;
-
-            if (j !=0 && j != size-1){
-                d_offt_01 = d_offt[i, j+1];
-                d_offt_00 = d_offt[i, j];
-                d_offt_02 = d_offt[i, j+2];
-                if (d_offt_00 && d_offt_01 && d_offt_02){
-                    d_inhom[i, j+1] = d_offt_01 - (d_offt_00 + d_offt_02) / 2;
+    calculate_inhomogeneity_kernel = cp.ElementwiseKernel(
+        in_params="""
+            int64 size, raw float64 d_offt 
+        """,
+        out_params="""
+            raw float64 d_inhom
+        """,
+        operation=""" 
+            if (((i) % size != 0) && ((i+1) % size != 0)){
+                if (d_offt[i-1] && d_offt[i] && d_offt[i+1]){
+                    d_inhom[i] = d_offt[i] - (d_offt[i-1] + d_offt[i+1]) / 2;
                 }
-            }
-        }
-        ''', 
-        'calculate_inhomoginity_kernel'
+            }else{
+                if(i % size == 0){
+                    if (d_offt[i] && d_offt[i+1] && d_offt[i+2]){
+                        d_inhom[i] = d_offt[i] - 2*d_offt[i+1] + d_offt[i+2];
+                   }
+                }else{
+                    if (d_offt[i] && d_offt[i-1] && d_offt[i-2]){
+                        d_inhom[i] = d_offt[i] - 2*d_offt[i-1] + d_offt[i-2];
+                    }
+                } 
+            } 
+        """,
+        name='calculate_inhomogeneity_kernel'
     )
 
-    def calculate_inhomoginity_cupy(d_offt, axis):
+    def calculate_inhomogeneity_cupy(d_offt, axis):
         if axis: d_offt = d_offt.T
+        
+        size = d_offt.shape[0]
+        d_offt = d_offt.ravel()
         d_inhom = cp.zeros_like(d_offt)
-        size = d_inhom.shape[0]
-        calculate_inhomoginity_kernel(d_offt, d_inhom, size)
-        mask = (d_offt[:, 0] != 0) * (d_offt[:, 1] != 0) * (d_offt[:, 2] != 0)
-        d_inhom[mask, 0] = d_offt[mask, 0] - 2*d_offt[mask, 1] + d_offt[mask, 2]
         
-        mask = (d_offt[:, -1] != 0) * (d_offt[:, -2] != 0) * (d_offt[:, -3] != 0)
-        d_inhom[mask, -1] = d_offt[mask, -1] - 2*d_offt[mask, -2] + d_offt[mask, -3]
+        calculate_inhomogeneity_kernel(size, d_offt, d_inhom, size = size**2)
+        
+        d_inhom = d_inhom.reshape(size, size)
             
-
         if axis: d_inhom = d_inhom.T
         return d_inhom
+    return calculate_inhomogeneity_cupy
 
-    return calculate_inhomoginity_cupy
 
 
 @nb.njit(parallel=True)
 def calculate_inhomogeneity_numba(d_offt, axis):
     if axis: d_offt = d_offt.T
     d_inhom = np.zeros_like(d_offt)
     size = d_inhom.shape[0]
@@ -55,23 +61,14 @@
             d_offt_01 = d_offt[i, j+1]
             if not d_offt_01:
                 continue
             d_offt_00 = d_offt[i, j]
             d_offt_02 = d_offt[i, j+2]
             if d_offt_00 and d_offt_02:
                 d_inhom[i, j+1] = d_offt_01 - (d_offt_00 + d_offt_02) / 2
-                continue
-            d_offt_03 = d_offt[i, j+3]
-            if d_offt_03:
-                d_inhom[i, j+1] = d_offt_01 - 2*d_offt_02 + d_offt_03
-                continue
-            d_offt_00_1 = d_offt[i, j-1]
-            if d_offt_00_1:
-                d_inhom[i, j+1] = d_offt_01 - 2*d_offt_00 + d_offt_00_1
-                continue
     
     mask = (d_offt[:, 0] != 0) * (d_offt[:, 1] != 0) * (d_offt[:, 2] != 0)
     d_inhom[mask, 0] = d_offt[mask, 0] - 2*d_offt[mask, 1] + d_offt[mask, 2]
     
     mask = (d_offt[:, -1] != 0) * (d_offt[:, -2] != 0) * (d_offt[:, -3] != 0)
     d_inhom[mask, -1] = d_offt[mask, -1] - 2*d_offt[mask, -2] + d_offt[mask, -3]
```

### Comparing `lcode-0.3.0/lcode/plasma3d/profile.py` & `lcode-0.3.1/lcode/plasma3d/profile.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/plasma3d/rhoj.py` & `lcode-0.3.1/lcode/plasma3d/rhoj.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/plasma3d/solver.py` & `lcode-0.3.1/lcode/plasma3d/solver.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/plasma3d/weights.py` & `lcode-0.3.1/lcode/plasma3d/weights.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/push_solvers/push_solver.py` & `lcode-0.3.1/lcode/push_solvers/push_solver.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode/simulation.py` & `lcode-0.3.1/lcode/simulation.py`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/lcode.egg-info/PKG-INFO` & `lcode-0.3.1/lcode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcode
-Version: 0.3.0
+Version: 0.3.1
 Summary: LCODE is a free software for simulationplasma wakefield acceleration based on QSA.
 Home-page: https://lcode.info
 Download-URL: https://github.com/lcodePy-team/lcodePy
 Author: lcodePy-team
 Author-email: team@lcode.info
 License: BSD-3-Clause-extended
 Keywords: plasma wakefield acceleration,quasistatic approximation,numerical simulation
```

### Comparing `lcode-0.3.0/lcode.egg-info/SOURCES.txt` & `lcode-0.3.1/lcode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lcode-0.3.0/setup.py` & `lcode-0.3.1/setup.py`

 * *Files identical despite different names*

