# Comparing `tmp/aidee_living_docs-1.0.3.tar.gz` & `tmp/aidee_living_docs-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aidee_living_docs-1.0.3.tar", max compression
+gzip compressed data, was "aidee_living_docs-1.0.4.tar", max compression
```

## Comparing `aidee_living_docs-1.0.3.tar` & `aidee_living_docs-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1068 2023-01-20 18:00:26.839599 aidee_living_docs-1.0.3/LICENSE
--rw-r--r--   0        0        0     2306 2023-01-20 18:00:26.839599 aidee_living_docs-1.0.3/README.md
--rw-r--r--   0        0        0     2281 2023-01-20 18:00:48.023470 aidee_living_docs-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      293 2023-01-20 18:00:26.843599 aidee_living_docs-1.0.3/src/livingdocs/__init__.py
--rw-r--r--   0        0        0      247 2023-01-20 18:00:26.843599 aidee_living_docs-1.0.3/src/livingdocs/__main__.py
--rw-r--r--   0        0        0     1428 2023-01-20 18:00:26.843599 aidee_living_docs-1.0.3/src/livingdocs/cli.py
--rw-r--r--   0        0        0     5634 2023-01-20 18:00:26.843599 aidee_living_docs-1.0.3/src/livingdocs/collecting_formatter.py
--rwxr-xr-x   0        0        0     2196 2023-01-20 18:00:26.843599 aidee_living_docs-1.0.3/src/livingdocs/create_sphinx_feature_file_page.py
--rw-r--r--   0        0        0     2485 2023-01-20 18:00:26.843599 aidee_living_docs-1.0.3/src/livingdocs/create_trace_page.py
--rw-r--r--   0        0        0      709 2023-01-20 18:00:26.843599 aidee_living_docs-1.0.3/src/livingdocs/create_userneeds_page.py
--rw-r--r--   0        0        0      652 2023-01-20 18:00:26.843599 aidee_living_docs-1.0.3/src/livingdocs/feature.jinja2
--rw-r--r--   0        0        0     1129 2023-01-20 18:00:26.843599 aidee_living_docs-1.0.3/src/livingdocs/feature_file.py
--rw-r--r--   0        0        0     1615 2023-01-20 18:00:26.843599 aidee_living_docs-1.0.3/src/livingdocs/json_formatter.py
--rw-r--r--   0        0        0        0 2023-01-20 18:00:26.843599 aidee_living_docs-1.0.3/src/livingdocs/py.typed
--rw-r--r--   0        0        0      646 2023-01-20 18:00:26.843599 aidee_living_docs-1.0.3/src/livingdocs/scenario.jinja2
--rw-r--r--   0        0        0      467 2023-01-20 18:00:26.843599 aidee_living_docs-1.0.3/src/livingdocs/template.py
--rw-r--r--   0        0        0      218 2023-01-20 18:00:26.843599 aidee_living_docs-1.0.3/src/livingdocs/userneeds.jinja2
--rw-r--r--   0        0        0      798 2023-01-20 18:00:26.843599 aidee_living_docs-1.0.3/src/livingdocs/userneeds.py
--rw-r--r--   0        0        0      646 2023-01-20 18:00:26.843599 aidee_living_docs-1.0.3/src/livingdocs/userneeds_trace.jinja2
--rw-r--r--   0        0        0     3703 1970-01-01 00:00:00.000000 aidee_living_docs-1.0.3/setup.py
--rw-r--r--   0        0        0     3144 1970-01-01 00:00:00.000000 aidee_living_docs-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2306 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/README.md
+-rw-r--r--   0        0        0     2281 2024-05-24 08:26:56.945383 aidee_living_docs-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      294 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/src/livingdocs/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/src/livingdocs/__main__.py
+-rw-r--r--   0        0        0     1429 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/src/livingdocs/cli.py
+-rw-r--r--   0        0        0     5635 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/src/livingdocs/collecting_formatter.py
+-rwxr-xr-x   0        0        0     2197 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/src/livingdocs/create_sphinx_feature_file_page.py
+-rw-r--r--   0        0        0     2486 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/src/livingdocs/create_trace_page.py
+-rw-r--r--   0        0        0      710 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/src/livingdocs/create_userneeds_page.py
+-rw-r--r--   0        0        0      652 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/src/livingdocs/feature.jinja2
+-rw-r--r--   0        0        0     1130 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/src/livingdocs/feature_file.py
+-rw-r--r--   0        0        0     1616 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/src/livingdocs/json_formatter.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/src/livingdocs/py.typed
+-rw-r--r--   0        0        0      646 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/src/livingdocs/scenario.jinja2
+-rw-r--r--   0        0        0      468 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/src/livingdocs/template.py
+-rw-r--r--   0        0        0      218 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/src/livingdocs/userneeds.jinja2
+-rw-r--r--   0        0        0      799 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/src/livingdocs/userneeds.py
+-rw-r--r--   0        0        0      646 2024-05-24 08:26:45.417390 aidee_living_docs-1.0.4/src/livingdocs/userneeds_trace.jinja2
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 aidee_living_docs-1.0.4/PKG-INFO
```

### Comparing `aidee_living_docs-1.0.3/LICENSE` & `aidee_living_docs-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aidee_living_docs-1.0.3/README.md` & `aidee_living_docs-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aidee_living_docs-1.0.3/pyproject.toml` & `aidee_living_docs-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aidee-living-docs"
-version = "1.0.3"
+version = "1.0.4"
 description = "Helpers for generating living documentation with Sphinx and Behave"
 authors = ["Aidee Health AS <hello@aidee.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/aidee-health/aidee-living-docs"
 repository = "https://github.com/aidee-health/aidee-living-docs"
 packages = [
```

### Comparing `aidee_living_docs-1.0.3/src/livingdocs/cli.py` & `aidee_living_docs-1.0.4/src/livingdocs/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """cli entry point for livingdocs.
 
 Parse command line arguments, invoke proper methods.
 """
+
 import argparse
 import logging
 import sys
 
 from . import __version__
```

### Comparing `aidee_living_docs-1.0.3/src/livingdocs/collecting_formatter.py` & `aidee_living_docs-1.0.4/src/livingdocs/collecting_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Implement Formatter functionality for Behave."""
+
 import time
 from itertools import chain
 from typing import Optional
 
 from behave.formatter.base import Formatter
 from behave.model import Feature
 from behave.model import Scenario
```

### Comparing `aidee_living_docs-1.0.3/src/livingdocs/create_sphinx_feature_file_page.py` & `aidee_living_docs-1.0.4/src/livingdocs/create_sphinx_feature_file_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Create Sphinx compatible feature page."""
+
 import pathlib
 import sys
 from glob import glob
 from os import path
 
 from jinja2 import Environment
 from jinja2 import FileSystemLoader
```

### Comparing `aidee_living_docs-1.0.3/src/livingdocs/create_trace_page.py` & `aidee_living_docs-1.0.4/src/livingdocs/create_trace_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Create traceability. Link scenarios with status to user needs."""
+
 import sys
 
 from .collecting_formatter import CollectedScenario
 from .feature_file import load_all_feature_files_in_directory
 from .feature_file import status_to_style
 from .template import convert_template
 from .userneeds import load_userneeds_from_file
```

### Comparing `aidee_living_docs-1.0.3/src/livingdocs/create_userneeds_page.py` & `aidee_living_docs-1.0.4/src/livingdocs/create_userneeds_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for generating user needs page."""
+
 import sys
 
 from .template import convert_template
 from .userneeds import load_userneeds_from_file
 
 
 def main(args=None):
```

### Comparing `aidee_living_docs-1.0.3/src/livingdocs/feature.jinja2` & `aidee_living_docs-1.0.4/src/livingdocs/feature.jinja2`

 * *Files identical despite different names*

### Comparing `aidee_living_docs-1.0.3/src/livingdocs/feature_file.py` & `aidee_living_docs-1.0.4/src/livingdocs/feature_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for creating a BDD feature file."""
+
 import json
 from glob import glob
 from os import path
 
 from .collecting_formatter import CollectedFeature
```

### Comparing `aidee_living_docs-1.0.3/src/livingdocs/json_formatter.py` & `aidee_living_docs-1.0.4/src/livingdocs/json_formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Behave JSONFormatter."""
+
 import json
 from os import path
 
 from .collecting_formatter import CollectingFormatter
 
 
 class JSONFormatter(CollectingFormatter):
```

### Comparing `aidee_living_docs-1.0.3/src/livingdocs/scenario.jinja2` & `aidee_living_docs-1.0.4/src/livingdocs/scenario.jinja2`

 * *Files identical despite different names*

### Comparing `aidee_living_docs-1.0.3/src/livingdocs/userneeds.py` & `aidee_living_docs-1.0.4/src/livingdocs/userneeds.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Parse and format user needs."""
+
 import csv
 
 
 EXPECTED_NUMBER_OF_USERNEED_COLUMNS = 2
 
 
 def load_userneeds_from_file(filename):
```

### Comparing `aidee_living_docs-1.0.3/src/livingdocs/userneeds_trace.jinja2` & `aidee_living_docs-1.0.4/src/livingdocs/userneeds_trace.jinja2`

 * *Files identical despite different names*

### Comparing `aidee_living_docs-1.0.3/setup.py` & `aidee_living_docs-1.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,93 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: aidee-living-docs
+Version: 1.0.4
+Summary: Helpers for generating living documentation with Sphinx and Behave
+Home-page: https://github.com/aidee-health/aidee-living-docs
+License: MIT
+Author: Aidee Health AS
+Author-email: hello@aidee.io
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: behave (>=1.2.6,<2.0.0)
+Project-URL: Changelog, https://github.com/aidee-health/aidee-living-docs/releases
+Project-URL: Repository, https://github.com/aidee-health/aidee-living-docs
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Aidee Living Documentation Helpers
 
-packages = \
-['livingdocs']
+[![PyPI](https://img.shields.io/pypi/v/aidee-living-docs.svg)][pypi_]
+[![Status](https://img.shields.io/pypi/status/aidee-living-docs.svg)][status]
+[![Python Version](https://img.shields.io/pypi/pyversions/aidee-living-docs)][python version]
+[![License](https://img.shields.io/pypi/l/aidee-living-docs)][license]
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['behave>=1.2.6,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['aidee-living-docs = livingdocs.cli:main',
-                     'behave2sphinx = '
-                     'livingdocs.create_sphinx_feature_file_page:main',
-                     'behave2sphinx-all = '
-                     'livingdocs.create_sphinx_feature_file_page:process_files_in_current_directory',
-                     'createtracepage = livingdocs.create_trace_page:main',
-                     'userneeds2sphinx = '
-                     'livingdocs.create_userneeds_page:main']}
-
-setup_kwargs = {
-    'name': 'aidee-living-docs',
-    'version': '1.0.3',
-    'description': 'Helpers for generating living documentation with Sphinx and Behave',
-    'long_description': '# Aidee Living Documentation Helpers\n\n[![PyPI](https://img.shields.io/pypi/v/aidee-living-docs.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/aidee-living-docs.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/aidee-living-docs)][python version]\n[![License](https://img.shields.io/pypi/l/aidee-living-docs)][license]\n\n[![Tests](https://github.com/aidee-health/aidee-living-docs/workflows/Tests/badge.svg)][tests]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/aidee-living-docs/\n[status]: https://pypi.org/project/aidee-living-docs/\n[python version]: https://pypi.org/project/aidee-living-docs\n[tests]: https://github.com/aidee-health/aidee-living-docs/actions?workflow=Tests\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- Helper functions to generate living documentation with Sphinx and Behave\n- Type safe code using [mypy](https://mypy.readthedocs.io/) for type checking\n\n## Requirements\n\n- Python 3.9-3.11\n\n## Installation\n\nYou can install _Aidee Living Documentation_ via [pip]:\n\n```console\n$ pip install aidee-living-docs\n```\n\nThis adds `aidee-living-docs` as a library, but also provides the CLI application with the same name.\n\n## Using the application from the command line\n\nThe application also provides a CLI application that is automatically added to the path when installing via pip.\n\nOnce installed with pip, type:\n\n```\naidee-living-docs --help\n```\n\nTo see which options are available.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n[file an issue]: https://github.com/aidee-health/aidee-living-docs/issues\n[pip]: https://pip.pypa.io/\n\n## Credits\n\nThis project has been heavily inspired by [Bluefruit](https://github.com/bluefruit/LivingDocumentationHelpers)\n\n<!-- github-only -->\n\n[license]: https://github.com/aidee-health/aidee-living-docs/blob/main/LICENSE\n[contributor guide]: https://github.com/aidee-health/aidee-living-docs/blob/main/CONTRIBUTING.md\n',
-    'author': 'Aidee Health AS',
-    'author_email': 'hello@aidee.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/aidee-health/aidee-living-docs',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+[![Tests](https://github.com/aidee-health/aidee-living-docs/workflows/Tests/badge.svg)][tests]
 
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+
+[pypi_]: https://pypi.org/project/aidee-living-docs/
+[status]: https://pypi.org/project/aidee-living-docs/
+[python version]: https://pypi.org/project/aidee-living-docs
+[tests]: https://github.com/aidee-health/aidee-living-docs/actions?workflow=Tests
+[pre-commit]: https://github.com/pre-commit/pre-commit
+[black]: https://github.com/psf/black
+
+## Features
+
+- Helper functions to generate living documentation with Sphinx and Behave
+- Type safe code using [mypy](https://mypy.readthedocs.io/) for type checking
+
+## Requirements
+
+- Python 3.9-3.11
+
+## Installation
+
+You can install _Aidee Living Documentation_ via [pip]:
+
+```console
+$ pip install aidee-living-docs
+```
+
+This adds `aidee-living-docs` as a library, but also provides the CLI application with the same name.
+
+## Using the application from the command line
+
+The application also provides a CLI application that is automatically added to the path when installing via pip.
+
+Once installed with pip, type:
+
+```
+aidee-living-docs --help
+```
+
+To see which options are available.
+
+## Contributing
+
+Contributions are very welcome.
+To learn more, see the [Contributor Guide].
+
+## Issues
+
+If you encounter any problems,
+please [file an issue] along with a detailed description.
+
+[file an issue]: https://github.com/aidee-health/aidee-living-docs/issues
+[pip]: https://pip.pypa.io/
+
+## Credits
+
+This project has been heavily inspired by [Bluefruit](https://github.com/bluefruit/LivingDocumentationHelpers)
+
+<!-- github-only -->
+
+[license]: https://github.com/aidee-health/aidee-living-docs/blob/main/LICENSE
+[contributor guide]: https://github.com/aidee-health/aidee-living-docs/blob/main/CONTRIBUTING.md
 
-setup(**setup_kwargs)
```

