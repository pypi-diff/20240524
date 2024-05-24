# Comparing `tmp/movement-0.0.8.tar.gz` & `tmp/movement-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movement-0.0.8.tar", last modified: Thu Oct 12 17:10:40 2023, max compression
+gzip compressed data, was "movement-0.0.9.tar", last modified: Mon Oct 30 10:30:30 2023, max compression
```

## Comparing `movement-0.0.8.tar` & `movement-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:10:40.357233 movement-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:10:40.349233 movement-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:10:40.353233 movement-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-10-12 17:10:30.000000 movement-0.0.8/.github/workflows/docs_build_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-10-12 17:10:30.000000 movement-0.0.8/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-10-12 17:10:30.000000 movement-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    13756 2023-10-12 17:10:30.000000 movement-0.0.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-10-12 17:10:30.000000 movement-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-10-12 17:10:30.000000 movement-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2023-10-12 17:10:40.357233 movement-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2023-10-12 17:10:30.000000 movement-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:10:40.353233 movement-0.0.8/movement/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-10-12 17:10:30.000000 movement-0.0.8/movement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2023-10-12 17:10:30.000000 movement-0.0.8/movement/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:10:40.357233 movement-0.0.8/movement/io/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-12 17:10:30.000000 movement-0.0.8/movement/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13042 2023-10-12 17:10:30.000000 movement-0.0.8/movement/io/load_poses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2023-10-12 17:10:30.000000 movement-0.0.8/movement/io/poses_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2023-10-12 17:10:30.000000 movement-0.0.8/movement/io/save_poses.py
--rw-r--r--   0 runner    (1001) docker     (127)    12483 2023-10-12 17:10:30.000000 movement-0.0.8/movement/io/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2023-10-12 17:10:30.000000 movement-0.0.8/movement/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:10:40.353233 movement-0.0.8/movement.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2023-10-12 17:10:40.000000 movement-0.0.8/movement.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-10-12 17:10:40.000000 movement-0.0.8/movement.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 17:10:40.000000 movement-0.0.8/movement.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2023-10-12 17:10:40.000000 movement-0.0.8/movement.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-12 17:10:40.000000 movement-0.0.8/movement.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2023-10-12 17:10:30.000000 movement-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-12 17:10:40.357233 movement-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 10:30:30.787737 movement-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 10:30:30.783737 movement-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 10:30:30.783737 movement-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2023-10-30 10:30:22.000000 movement-0.0.9/.github/workflows/docs_build_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-10-30 10:30:22.000000 movement-0.0.9/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-10-30 10:30:22.000000 movement-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    13365 2023-10-30 10:30:22.000000 movement-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2023-10-30 10:30:22.000000 movement-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2023-10-30 10:30:22.000000 movement-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2023-10-30 10:30:30.787737 movement-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2023-10-30 10:30:22.000000 movement-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 10:30:30.783737 movement-0.0.9/movement/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2023-10-30 10:30:22.000000 movement-0.0.9/movement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2023-10-30 10:30:22.000000 movement-0.0.9/movement/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 10:30:30.787737 movement-0.0.9/movement/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-30 10:30:22.000000 movement-0.0.9/movement/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13042 2023-10-30 10:30:22.000000 movement-0.0.9/movement/io/load_poses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2023-10-30 10:30:22.000000 movement-0.0.9/movement/io/poses_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2023-10-30 10:30:22.000000 movement-0.0.9/movement/io/save_poses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12483 2023-10-30 10:30:22.000000 movement-0.0.9/movement/io/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2023-10-30 10:30:22.000000 movement-0.0.9/movement/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 10:30:30.787737 movement-0.0.9/movement.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2023-10-30 10:30:30.000000 movement-0.0.9/movement.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2023-10-30 10:30:30.000000 movement-0.0.9/movement.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 10:30:30.000000 movement-0.0.9/movement.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2023-10-30 10:30:30.000000 movement-0.0.9/movement.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-30 10:30:30.000000 movement-0.0.9/movement.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2023-10-30 10:30:22.000000 movement-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-30 10:30:30.787737 movement-0.0.9/setup.cfg
```

### Comparing `movement-0.0.8/.github/workflows/docs_build_and_deploy.yml` & `movement-0.0.9/.github/workflows/docs_build_and_deploy.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Build Sphinx docs and deploy to GitHub Pages
+name: Docs
 
 # Generate the documentation on all merges to main, all pull requests, or by
 # manual workflow dispatch. The build job can be used as a CI check that the
 # docs still build successfully. The deploy job only runs when a tag is
 # pushed and actually moves the generated html to the gh-pages branch
 # (which triggers a GitHub pages deployment).
 on:
@@ -15,20 +15,22 @@
   workflow_dispatch:
 
 jobs:
   build_sphinx_docs:
     name: Build Sphinx Docs
     runs-on: ubuntu-latest
     steps:
-      - uses: neuroinformatics-unit/actions/build_sphinx_docs@v2
+      - uses: neuroinformatics-unit/actions/build_sphinx_docs@main
+        with:
+          python-version: 3.11
 
   deploy_sphinx_docs:
     name: Deploy Sphinx Docs
     needs: build_sphinx_docs
     permissions:
       contents: write
     if: github.event_name == 'push' && github.ref_type == 'tag'
     runs-on: ubuntu-latest
     steps:
-      - uses: neuroinformatics-unit/actions/deploy_sphinx_docs@v2
+      - uses: neuroinformatics-unit/actions/deploy_sphinx_docs@main
         with:
           secret_input: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `movement-0.0.8/.github/workflows/test_and_deploy.yml` & `movement-0.0.9/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `movement-0.0.8/.gitignore` & `movement-0.0.9/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 local_settings.py
 
 # Flask instance folder
 instance/
 
 # Sphinx documentation
 docs/build/
-docs/source/auto_examples/
-docs/source/auto_api/
+docs/source/examples/
+docs/source/api/
 
 # MkDocs documentation
 /site/
 
 # PyBuilder
 target/
```

### Comparing `movement-0.0.8/CONTRIBUTING.md` & `movement-0.0.9/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 # How to Contribute
 
-**Contributors to movement are absolutely encouraged**, whether to fix a bug,
-develop a new feature, or improve the documentation.
-If you're unsure about any part of the contributing process, please get in touch.
-It's best to reach out in public, e.g. by [opening an issue](https://github.com/neuroinformatics-unit/movement/issues)
-so that others can benefit from the discussion.
-
 ## Contributing code
 
 ### Creating a development environment
 
 It is recommended to use [conda](https://docs.conda.io/en/latest/)
 or [mamba](https://mamba.readthedocs.io/en/latest/index.html) to create a
 development environment for movement. In the following we assume you have
@@ -189,26 +183,26 @@
 e.g.:
 
 ```rst
 My new module
 --------------
 .. currentmodule:: movement.new_module
 .. autosummary::
-    :toctree: auto_api
+    :toctree: api
 
     new_function
     NewClass
 ```
 
 For this to work, your functions/classes/methods will need to have docstrings
 that follow the [numpydoc](https://numpydoc.readthedocs.io/en/latest/format.html) style.
 
 ### Updating the examples
 We use [sphinx-gallery](https://sphinx-gallery.github.io/stable/index.html)
-to create the [examples](https://movement.neuroinformatics.dev/auto_examples/index.html).
+to create the [examples](https://movement.neuroinformatics.dev/examples/index.html).
 To add new examples, you will need to create a new `.py` file in `examples/`.
 The file should be structured as specified in the relevant
 [sphinx-gallery documentation](https://sphinx-gallery.github.io/stable/syntax.html).
 
 
 ### Building the documentation locally
 We recommend that you build and view the documentation website locally, before you push it.
```

### Comparing `movement-0.0.8/LICENSE` & `movement-0.0.9/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
-Copyright (c) 2023, Niko Sirmpilatze
+Copyright (c) 2023, University College London
+
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `movement-0.0.8/PKG-INFO` & `movement-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movement
-Version: 0.0.8
+Version: 0.0.9
 Summary: Analysis of body movement
 Author-email: Niko Sirmpilatze <niko.sirbiladze@gmail.com>, Chang Huan Lo <changhuan.lo@ucl.ac.uk>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/neuroinformatics-unit/movement
 Project-URL: Bug Tracker, https://github.com/neuroinformatics-unit/movement/issues
 Project-URL: Documentation, https://movement.neuroinformatics.dev/
 Project-URL: Source Code, https://github.com/neuroinformatics-unit/movement
@@ -48,37 +48,46 @@
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![project chat](https://img.shields.io/badge/zulip-join_chat-brightgreen.svg)](https://neuroinformatics.zulipchat.com/#narrow/stream/406001-Movement/topic/Welcome!)
 
 # movement
 
-Kinematic analysis of animal 🐝 🦀 🐀 🐒 body movements for neuroscience and ethology research 🔬.
+Python tools for analysing body movements across space and time, to aid the study of animal behaviour in neuroscience.
 
-- Read the [documentation](https://movement.neuroinformatics.dev) for more information.
-- If you wish to contribute, please read the [contributing guide](./CONTRIBUTING.md).
-- Join us on [zulip](https://neuroinformatics.zulipchat.com/#narrow/stream/406001-Movement/topic/Welcome!) to chat with the team. We welcome your questions and suggestions.
+> **Note**
+> Read the [documentation](https://movement.neuroinformatics.dev) for more information, including [installation instructions](https://movement.neuroinformatics.dev/getting_started.html#installation) and [examples](https://movement.neuroinformatics.dev/examples/index.html).
+
+- [Overview](#overview)
+- [Status](#status)
+- [Join the movement](#join-the-movement)
+- [License](#license)
+- [Package template](#package-template)
+
+
+## Overview
+
+Pose estimation tools, such as [DeepLabCut](https://www.mackenziemathislab.org/deeplabcut) and [SLEAP](https://sleap.ai/) are now commonplace when processing video data of animal behaviour. There is not yet a standardised, easy-to-use way to process the pose tracks produced from these software packages.
+
+movement aims to provide a consistent modular interface to analyse pose tracks, allowing steps such as data cleaning, visualisation and motion quantification.
+We aim to support a range of pose estimation packages, along with 2D or 3D tracking of single or multiple animals.
+
+Find out more on our [mission and scope](https://movement.neuroinformatics.dev/community/mission-scope.html) statement and our [roadmap](https://movement.neuroinformatics.dev/community/roadmap.html).
 
 ## Status
 > **Warning**
 > - 🏗️ The package is currently in early development. Stay tuned ⌛
 > - It is not sufficiently tested to be used for scientific analysis
 > - The interface is subject to changes.
 
-## Aims
-* Load pose tracks from pose estimation software packages (e.g. [DeepLabCut](http://www.mackenziemathislab.org/deeplabcut) or [SLEAP](https://sleap.ai/))
-* Evaluate the quality of the tracks and perform data cleaning operations
-* Calculate kinematic variables (e.g. speed, acceleration, joint angles, etc.)
-* Produce reports and visualise the results
-
-## Related projects
-The following projects cover related needs and served as inspiration for this project:
-* [DLC2Kinematics](https://github.com/AdaptiveMotorControlLab/DLC2Kinematics)
-* [PyRat](https://github.com/pyratlib/pyrat)
-* [Kino](https://github.com/BrancoLab/Kino)
-* [WAZP](https://github.com/SainsburyWellcomeCentre/WAZP)
+## Join the movement
+
+Contributions to movement are absolutely encouraged, whether to fix a bug, develop a new feature, or improve the documentation.
+To help you get started, we have prepared a detailed [contributing guide](https://movement.neuroinformatics.dev/community/contributing.html).
+
+You are welcome to chat with the team on [zulip](https://neuroinformatics.zulipchat.com/#narrow/stream/406001-Movement/topic/Welcome!). You may also [open an issue](https://github.com/neuroinformatics-unit/movement/issues) to report a bug or request a new feature.
 
 ## License
 ⚖️ [BSD 3-Clause](./LICENSE)
 
-## Template
+## Package template
 This package layout and configuration (including pre-commit hooks and GitHub actions) have been copied from the [python-cookiecutter](https://github.com/neuroinformatics-unit/python-cookiecutter) template.
```

### Comparing `movement-0.0.8/README.md` & `movement-0.0.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -4,37 +4,46 @@
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![project chat](https://img.shields.io/badge/zulip-join_chat-brightgreen.svg)](https://neuroinformatics.zulipchat.com/#narrow/stream/406001-Movement/topic/Welcome!)
 
 # movement
 
-Kinematic analysis of animal 🐝 🦀 🐀 🐒 body movements for neuroscience and ethology research 🔬.
+Python tools for analysing body movements across space and time, to aid the study of animal behaviour in neuroscience.
 
-- Read the [documentation](https://movement.neuroinformatics.dev) for more information.
-- If you wish to contribute, please read the [contributing guide](./CONTRIBUTING.md).
-- Join us on [zulip](https://neuroinformatics.zulipchat.com/#narrow/stream/406001-Movement/topic/Welcome!) to chat with the team. We welcome your questions and suggestions.
+> **Note**
+> Read the [documentation](https://movement.neuroinformatics.dev) for more information, including [installation instructions](https://movement.neuroinformatics.dev/getting_started.html#installation) and [examples](https://movement.neuroinformatics.dev/examples/index.html).
+
+- [Overview](#overview)
+- [Status](#status)
+- [Join the movement](#join-the-movement)
+- [License](#license)
+- [Package template](#package-template)
+
+
+## Overview
+
+Pose estimation tools, such as [DeepLabCut](https://www.mackenziemathislab.org/deeplabcut) and [SLEAP](https://sleap.ai/) are now commonplace when processing video data of animal behaviour. There is not yet a standardised, easy-to-use way to process the pose tracks produced from these software packages.
+
+movement aims to provide a consistent modular interface to analyse pose tracks, allowing steps such as data cleaning, visualisation and motion quantification.
+We aim to support a range of pose estimation packages, along with 2D or 3D tracking of single or multiple animals.
+
+Find out more on our [mission and scope](https://movement.neuroinformatics.dev/community/mission-scope.html) statement and our [roadmap](https://movement.neuroinformatics.dev/community/roadmap.html).
 
 ## Status
 > **Warning**
 > - 🏗️ The package is currently in early development. Stay tuned ⌛
 > - It is not sufficiently tested to be used for scientific analysis
 > - The interface is subject to changes.
 
-## Aims
-* Load pose tracks from pose estimation software packages (e.g. [DeepLabCut](http://www.mackenziemathislab.org/deeplabcut) or [SLEAP](https://sleap.ai/))
-* Evaluate the quality of the tracks and perform data cleaning operations
-* Calculate kinematic variables (e.g. speed, acceleration, joint angles, etc.)
-* Produce reports and visualise the results
-
-## Related projects
-The following projects cover related needs and served as inspiration for this project:
-* [DLC2Kinematics](https://github.com/AdaptiveMotorControlLab/DLC2Kinematics)
-* [PyRat](https://github.com/pyratlib/pyrat)
-* [Kino](https://github.com/BrancoLab/Kino)
-* [WAZP](https://github.com/SainsburyWellcomeCentre/WAZP)
+## Join the movement
+
+Contributions to movement are absolutely encouraged, whether to fix a bug, develop a new feature, or improve the documentation.
+To help you get started, we have prepared a detailed [contributing guide](https://movement.neuroinformatics.dev/community/contributing.html).
+
+You are welcome to chat with the team on [zulip](https://neuroinformatics.zulipchat.com/#narrow/stream/406001-Movement/topic/Welcome!). You may also [open an issue](https://github.com/neuroinformatics-unit/movement/issues) to report a bug or request a new feature.
 
 ## License
 ⚖️ [BSD 3-Clause](./LICENSE)
 
-## Template
+## Package template
 This package layout and configuration (including pre-commit hooks and GitHub actions) have been copied from the [python-cookiecutter](https://github.com/neuroinformatics-unit/python-cookiecutter) template.
```

### Comparing `movement-0.0.8/movement/datasets.py` & `movement-0.0.9/movement/datasets.py`

 * *Files identical despite different names*

### Comparing `movement-0.0.8/movement/io/load_poses.py` & `movement-0.0.9/movement/io/load_poses.py`

 * *Files identical despite different names*

### Comparing `movement-0.0.8/movement/io/poses_accessor.py` & `movement-0.0.9/movement/io/poses_accessor.py`

 * *Files identical despite different names*

### Comparing `movement-0.0.8/movement/io/save_poses.py` & `movement-0.0.9/movement/io/save_poses.py`

 * *Files identical despite different names*

### Comparing `movement-0.0.8/movement/io/validators.py` & `movement-0.0.9/movement/io/validators.py`

 * *Files identical despite different names*

### Comparing `movement-0.0.8/movement/logging.py` & `movement-0.0.9/movement/logging.py`

 * *Files identical despite different names*

### Comparing `movement-0.0.8/movement.egg-info/PKG-INFO` & `movement-0.0.9/movement.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movement
-Version: 0.0.8
+Version: 0.0.9
 Summary: Analysis of body movement
 Author-email: Niko Sirmpilatze <niko.sirbiladze@gmail.com>, Chang Huan Lo <changhuan.lo@ucl.ac.uk>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/neuroinformatics-unit/movement
 Project-URL: Bug Tracker, https://github.com/neuroinformatics-unit/movement/issues
 Project-URL: Documentation, https://movement.neuroinformatics.dev/
 Project-URL: Source Code, https://github.com/neuroinformatics-unit/movement
@@ -48,37 +48,46 @@
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![project chat](https://img.shields.io/badge/zulip-join_chat-brightgreen.svg)](https://neuroinformatics.zulipchat.com/#narrow/stream/406001-Movement/topic/Welcome!)
 
 # movement
 
-Kinematic analysis of animal 🐝 🦀 🐀 🐒 body movements for neuroscience and ethology research 🔬.
+Python tools for analysing body movements across space and time, to aid the study of animal behaviour in neuroscience.
 
-- Read the [documentation](https://movement.neuroinformatics.dev) for more information.
-- If you wish to contribute, please read the [contributing guide](./CONTRIBUTING.md).
-- Join us on [zulip](https://neuroinformatics.zulipchat.com/#narrow/stream/406001-Movement/topic/Welcome!) to chat with the team. We welcome your questions and suggestions.
+> **Note**
+> Read the [documentation](https://movement.neuroinformatics.dev) for more information, including [installation instructions](https://movement.neuroinformatics.dev/getting_started.html#installation) and [examples](https://movement.neuroinformatics.dev/examples/index.html).
+
+- [Overview](#overview)
+- [Status](#status)
+- [Join the movement](#join-the-movement)
+- [License](#license)
+- [Package template](#package-template)
+
+
+## Overview
+
+Pose estimation tools, such as [DeepLabCut](https://www.mackenziemathislab.org/deeplabcut) and [SLEAP](https://sleap.ai/) are now commonplace when processing video data of animal behaviour. There is not yet a standardised, easy-to-use way to process the pose tracks produced from these software packages.
+
+movement aims to provide a consistent modular interface to analyse pose tracks, allowing steps such as data cleaning, visualisation and motion quantification.
+We aim to support a range of pose estimation packages, along with 2D or 3D tracking of single or multiple animals.
+
+Find out more on our [mission and scope](https://movement.neuroinformatics.dev/community/mission-scope.html) statement and our [roadmap](https://movement.neuroinformatics.dev/community/roadmap.html).
 
 ## Status
 > **Warning**
 > - 🏗️ The package is currently in early development. Stay tuned ⌛
 > - It is not sufficiently tested to be used for scientific analysis
 > - The interface is subject to changes.
 
-## Aims
-* Load pose tracks from pose estimation software packages (e.g. [DeepLabCut](http://www.mackenziemathislab.org/deeplabcut) or [SLEAP](https://sleap.ai/))
-* Evaluate the quality of the tracks and perform data cleaning operations
-* Calculate kinematic variables (e.g. speed, acceleration, joint angles, etc.)
-* Produce reports and visualise the results
-
-## Related projects
-The following projects cover related needs and served as inspiration for this project:
-* [DLC2Kinematics](https://github.com/AdaptiveMotorControlLab/DLC2Kinematics)
-* [PyRat](https://github.com/pyratlib/pyrat)
-* [Kino](https://github.com/BrancoLab/Kino)
-* [WAZP](https://github.com/SainsburyWellcomeCentre/WAZP)
+## Join the movement
+
+Contributions to movement are absolutely encouraged, whether to fix a bug, develop a new feature, or improve the documentation.
+To help you get started, we have prepared a detailed [contributing guide](https://movement.neuroinformatics.dev/community/contributing.html).
+
+You are welcome to chat with the team on [zulip](https://neuroinformatics.zulipchat.com/#narrow/stream/406001-Movement/topic/Welcome!). You may also [open an issue](https://github.com/neuroinformatics-unit/movement/issues) to report a bug or request a new feature.
 
 ## License
 ⚖️ [BSD 3-Clause](./LICENSE)
 
-## Template
+## Package template
 This package layout and configuration (including pre-commit hooks and GitHub actions) have been copied from the [python-cookiecutter](https://github.com/neuroinformatics-unit/python-cookiecutter) template.
```

### Comparing `movement-0.0.8/pyproject.toml` & `movement-0.0.9/pyproject.toml`

 * *Files identical despite different names*

