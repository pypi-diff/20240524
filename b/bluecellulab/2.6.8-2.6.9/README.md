# Comparing `tmp/bluecellulab-2.6.8.tar.gz` & `tmp/bluecellulab-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluecellulab-2.6.8.tar", last modified: Thu May  2 14:56:42 2024, max compression
+gzip compressed data, was "bluecellulab-2.6.9.tar", last modified: Fri May  3 14:09:40 2024, max compression
```

## Comparing `bluecellulab-2.6.8.tar` & `bluecellulab-2.6.9.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.631790 bluecellulab-2.6.8/
--rwxr-xr-x   0 runner    (1001) docker     (127)      147 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/.compile_mod.sh
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.615790 bluecellulab-2.6.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.615790 bluecellulab-2.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)    91984 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-02 14:56:42.631790 bluecellulab-2.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.615790 bluecellulab-2.6.8/bluecellulab/
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.619790 bluecellulab-2.6.8/bluecellulab/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/analysis/inject_sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.619790 bluecellulab-2.6.8/bluecellulab/cell/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/cell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.619790 bluecellulab-2.6.8/bluecellulab/cell/ballstick/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/cell/ballstick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/cell/ballstick/emodel.hoc
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/cell/ballstick/morphology.asc
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/cell/cell_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    31487 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/cell/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    18091 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/cell/injector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/cell/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/cell/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/cell/recording.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/cell/section_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/cell/serialized_sections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/cell/sonata_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/cell/stimuli_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/cell/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.623790 bluecellulab-2.6.8/bluecellulab/circuit/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.623790 bluecellulab-2.6.8/bluecellulab/circuit/circuit_access/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit/circuit_access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14273 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit/circuit_access/bluepy_circuit_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit/circuit_access/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit/circuit_access/sonata_circuit_access.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.623790 bluecellulab-2.6.8/bluecellulab/circuit/config/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit/config/bluepy_simulation_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit/config/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit/config/sections.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit/config/sonata_simulation_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit/iotools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit/node_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit/simulation_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit/synapse_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    33672 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/circuit_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.627790 bluecellulab-2.6.8/bluecellulab/hoc/
--rw-r--r--   0 runner    (1001) docker     (127)    16435 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/hoc/Cell.hoc
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/hoc/RNGSettings.hoc
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/hoc/TDistFunc.hoc
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/hoc/TStim.hoc
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/hoc/fileUtils.hoc
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/neuron_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/plotwindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/psection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/psegment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/rngsettings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.627790 bluecellulab-2.6.8/bluecellulab/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/simulation/neuron_globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/simulation/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/simulation/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.627790 bluecellulab-2.6.8/bluecellulab/stimulus/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/stimulus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15686 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/stimulus/circuit_stimulus_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14874 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/stimulus/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.627790 bluecellulab-2.6.8/bluecellulab/synapse/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/synapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/synapse/synapse_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    16871 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/synapse/synapse_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    11213 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/type_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/bluecellulab/verbosity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.631790 bluecellulab-2.6.8/bluecellulab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-02 14:56:42.000000 bluecellulab-2.6.8/bluecellulab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-02 14:56:42.000000 bluecellulab-2.6.8/bluecellulab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:56:42.000000 bluecellulab-2.6.8/bluecellulab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 14:56:42.000000 bluecellulab-2.6.8/bluecellulab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 14:56:42.000000 bluecellulab-2.6.8/bluecellulab.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.627790 bluecellulab-2.6.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.627790 bluecellulab-2.6.8/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    52552 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/docs/images/voltage-readme.png
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/docs/requirements_docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.631790 bluecellulab-2.6.8/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.631790 bluecellulab-2.6.8/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/docs/source/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/docs/source/compiling-mechanisms.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/docs/source/list_of_stim.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:56:42.631790 bluecellulab-2.6.8/docs/source/logo/
--rw-r--r--   0 runner    (1001) docker     (127)   333321 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/docs/source/logo/BlueCelluLabBanner.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:56:42.631790 bluecellulab-2.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-02 14:56:35.000000 bluecellulab-2.6.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.517277 bluecellulab-2.6.9/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      147 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/.compile_mod.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.505277 bluecellulab-2.6.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.505277 bluecellulab-2.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    91984 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-03 14:09:40.517277 bluecellulab-2.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.505277 bluecellulab-2.6.9/bluecellulab/
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.509277 bluecellulab-2.6.9/bluecellulab/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/analysis/inject_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.509277 bluecellulab-2.6.9/bluecellulab/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/cell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.509277 bluecellulab-2.6.9/bluecellulab/cell/ballstick/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/cell/ballstick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/cell/ballstick/emodel.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/cell/ballstick/morphology.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/cell/cell_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31487 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/cell/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18091 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/cell/injector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/cell/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/cell/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/cell/recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/cell/section_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/cell/serialized_sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/cell/sonata_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/cell/stimuli_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/cell/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.513277 bluecellulab-2.6.9/bluecellulab/circuit/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.513277 bluecellulab-2.6.9/bluecellulab/circuit/circuit_access/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit/circuit_access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14273 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit/circuit_access/bluepy_circuit_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit/circuit_access/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit/circuit_access/sonata_circuit_access.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.513277 bluecellulab-2.6.9/bluecellulab/circuit/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit/config/bluepy_simulation_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit/config/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit/config/sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit/config/sonata_simulation_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit/iotools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit/node_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit/simulation_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit/synapse_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33672 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/circuit_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.513277 bluecellulab-2.6.9/bluecellulab/hoc/
+-rw-r--r--   0 runner    (1001) docker     (127)    16435 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/hoc/Cell.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/hoc/RNGSettings.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/hoc/TDistFunc.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/hoc/TStim.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/hoc/fileUtils.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/neuron_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/plotwindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/psection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/psegment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/rngsettings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.513277 bluecellulab-2.6.9/bluecellulab/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/simulation/neuron_globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/simulation/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/simulation/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.517277 bluecellulab-2.6.9/bluecellulab/stimulus/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/stimulus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15686 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/stimulus/circuit_stimulus_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14874 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/stimulus/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.517277 bluecellulab-2.6.9/bluecellulab/synapse/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/synapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/synapse/synapse_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16871 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/synapse/synapse_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11213 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/type_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/bluecellulab/verbosity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.517277 bluecellulab-2.6.9/bluecellulab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-03 14:09:40.000000 bluecellulab-2.6.9/bluecellulab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-03 14:09:40.000000 bluecellulab-2.6.9/bluecellulab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:09:40.000000 bluecellulab-2.6.9/bluecellulab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-03 14:09:40.000000 bluecellulab-2.6.9/bluecellulab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 14:09:40.000000 bluecellulab-2.6.9/bluecellulab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.517277 bluecellulab-2.6.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.517277 bluecellulab-2.6.9/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    52552 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/docs/images/voltage-readme.png
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/docs/requirements_docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.517277 bluecellulab-2.6.9/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.517277 bluecellulab-2.6.9/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/docs/source/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/docs/source/compiling-mechanisms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/docs/source/list_of_stim.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:09:40.517277 bluecellulab-2.6.9/docs/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)   333321 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/docs/source/logo/BlueCelluLabBanner.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-03 14:09:32.000000 bluecellulab-2.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 14:09:40.517277 bluecellulab-2.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-03 14:09:33.000000 bluecellulab-2.6.9/tox.ini
```

### Comparing `bluecellulab-2.6.8/.github/dependabot.yml` & `bluecellulab-2.6.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/.github/workflows/release.yml` & `bluecellulab-2.6.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/.github/workflows/test.yml` & `bluecellulab-2.6.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/.gitlab-ci.yml` & `bluecellulab-2.6.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/.zenodo.json` & `bluecellulab-2.6.9/.zenodo.json`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/CHANGELOG.rst` & `bluecellulab-2.6.9/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/LICENSE` & `bluecellulab-2.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/PKG-INFO` & `bluecellulab-2.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluecellulab
-Version: 2.6.8
+Version: 2.6.9
 Summary: Biologically detailed neural network simulations and analysis.
 Author: Blue Brain Project, EPFL
 License: Apache2.0
 Project-URL: Homepage, https://github.com/BlueBrain/BlueCelluLab
 Project-URL: Documentation, https://bluecellulab.readthedocs.io/
 Keywords: computational neuroscience,simulation,analysis,SONATA,neural networks,neuron,Blue Brain Project
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bluecellulab-2.6.8/README.rst` & `bluecellulab-2.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/__init__.py` & `bluecellulab-2.6.9/bluecellulab/__init__.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/analysis/inject_sequence.py` & `bluecellulab-2.6.9/bluecellulab/analysis/inject_sequence.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/cell/ballstick/emodel.hoc` & `bluecellulab-2.6.9/bluecellulab/cell/ballstick/emodel.hoc`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/cell/cell_dict.py` & `bluecellulab-2.6.9/bluecellulab/cell/cell_dict.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/cell/core.py` & `bluecellulab-2.6.9/bluecellulab/cell/core.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/cell/injector.py` & `bluecellulab-2.6.9/bluecellulab/cell/injector.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/cell/plotting.py` & `bluecellulab-2.6.9/bluecellulab/cell/plotting.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/cell/random.py` & `bluecellulab-2.6.9/bluecellulab/cell/random.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/cell/section_distance.py` & `bluecellulab-2.6.9/bluecellulab/cell/section_distance.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/cell/serialized_sections.py` & `bluecellulab-2.6.9/bluecellulab/cell/serialized_sections.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/cell/sonata_proxy.py` & `bluecellulab-2.6.9/bluecellulab/cell/sonata_proxy.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/cell/stimuli_generator.py` & `bluecellulab-2.6.9/bluecellulab/cell/stimuli_generator.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/cell/template.py` & `bluecellulab-2.6.9/bluecellulab/cell/template.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/circuit/circuit_access/bluepy_circuit_access.py` & `bluecellulab-2.6.9/bluecellulab/circuit/circuit_access/bluepy_circuit_access.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/circuit/circuit_access/definition.py` & `bluecellulab-2.6.9/bluecellulab/circuit/circuit_access/definition.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/circuit/circuit_access/sonata_circuit_access.py` & `bluecellulab-2.6.9/bluecellulab/circuit/circuit_access/sonata_circuit_access.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/circuit/config/bluepy_simulation_config.py` & `bluecellulab-2.6.9/bluecellulab/circuit/config/bluepy_simulation_config.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/circuit/config/definition.py` & `bluecellulab-2.6.9/bluecellulab/circuit/config/definition.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/circuit/config/sections.py` & `bluecellulab-2.6.9/bluecellulab/circuit/config/sections.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/circuit/config/sonata_simulation_config.py` & `bluecellulab-2.6.9/bluecellulab/circuit/config/sonata_simulation_config.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/circuit/format.py` & `bluecellulab-2.6.9/bluecellulab/circuit/format.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/circuit/iotools.py` & `bluecellulab-2.6.9/bluecellulab/circuit/iotools.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/circuit/node_id.py` & `bluecellulab-2.6.9/bluecellulab/circuit/node_id.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/circuit/simulation_access.py` & `bluecellulab-2.6.9/bluecellulab/circuit/simulation_access.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/circuit/synapse_properties.py` & `bluecellulab-2.6.9/bluecellulab/circuit/synapse_properties.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/circuit/validate.py` & `bluecellulab-2.6.9/bluecellulab/circuit/validate.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/circuit_simulation.py` & `bluecellulab-2.6.9/bluecellulab/circuit_simulation.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/connection.py` & `bluecellulab-2.6.9/bluecellulab/connection.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/dendrogram.py` & `bluecellulab-2.6.9/bluecellulab/dendrogram.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/exceptions.py` & `bluecellulab-2.6.9/bluecellulab/exceptions.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/graph.py` & `bluecellulab-2.6.9/bluecellulab/graph.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/hoc/Cell.hoc` & `bluecellulab-2.6.9/bluecellulab/hoc/Cell.hoc`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/hoc/RNGSettings.hoc` & `bluecellulab-2.6.9/bluecellulab/hoc/RNGSettings.hoc`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/hoc/TDistFunc.hoc` & `bluecellulab-2.6.9/bluecellulab/hoc/TDistFunc.hoc`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/hoc/TStim.hoc` & `bluecellulab-2.6.9/bluecellulab/hoc/TStim.hoc`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/hoc/fileUtils.hoc` & `bluecellulab-2.6.9/bluecellulab/hoc/fileUtils.hoc`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/importer.py` & `bluecellulab-2.6.9/bluecellulab/importer.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/neuron_interpreter.py` & `bluecellulab-2.6.9/bluecellulab/neuron_interpreter.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/plotwindow.py` & `bluecellulab-2.6.9/bluecellulab/plotwindow.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/psection.py` & `bluecellulab-2.6.9/bluecellulab/psection.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/psegment.py` & `bluecellulab-2.6.9/bluecellulab/psegment.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/rngsettings.py` & `bluecellulab-2.6.9/bluecellulab/rngsettings.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/simulation/neuron_globals.py` & `bluecellulab-2.6.9/bluecellulab/simulation/neuron_globals.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/simulation/parallel.py` & `bluecellulab-2.6.9/bluecellulab/simulation/parallel.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/simulation/simulation.py` & `bluecellulab-2.6.9/bluecellulab/simulation/simulation.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/stimulus/circuit_stimulus_definitions.py` & `bluecellulab-2.6.9/bluecellulab/stimulus/circuit_stimulus_definitions.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/stimulus/factory.py` & `bluecellulab-2.6.9/bluecellulab/stimulus/factory.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/synapse/synapse_factory.py` & `bluecellulab-2.6.9/bluecellulab/synapse/synapse_factory.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/synapse/synapse_types.py` & `bluecellulab-2.6.9/bluecellulab/synapse/synapse_types.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/tools.py` & `bluecellulab-2.6.9/bluecellulab/tools.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/utils.py` & `bluecellulab-2.6.9/bluecellulab/utils.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab/verbosity.py` & `bluecellulab-2.6.9/bluecellulab/verbosity.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/bluecellulab.egg-info/PKG-INFO` & `bluecellulab-2.6.9/bluecellulab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluecellulab
-Version: 2.6.8
+Version: 2.6.9
 Summary: Biologically detailed neural network simulations and analysis.
 Author: Blue Brain Project, EPFL
 License: Apache2.0
 Project-URL: Homepage, https://github.com/BlueBrain/BlueCelluLab
 Project-URL: Documentation, https://bluecellulab.readthedocs.io/
 Keywords: computational neuroscience,simulation,analysis,SONATA,neural networks,neuron,Blue Brain Project
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bluecellulab-2.6.8/bluecellulab.egg-info/SOURCES.txt` & `bluecellulab-2.6.9/bluecellulab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/docs/Makefile` & `bluecellulab-2.6.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/docs/images/voltage-readme.png` & `bluecellulab-2.6.9/docs/images/voltage-readme.png`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/docs/make.bat` & `bluecellulab-2.6.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/docs/source/compiling-mechanisms.rst` & `bluecellulab-2.6.9/docs/source/compiling-mechanisms.rst`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/docs/source/conf.py` & `bluecellulab-2.6.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/docs/source/list_of_stim.rst` & `bluecellulab-2.6.9/docs/source/list_of_stim.rst`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/docs/source/logo/BlueCelluLabBanner.jpg` & `bluecellulab-2.6.9/docs/source/logo/BlueCelluLabBanner.jpg`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/pyproject.toml` & `bluecellulab-2.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bluecellulab-2.6.8/tox.ini` & `bluecellulab-2.6.9/tox.ini`

 * *Files identical despite different names*

