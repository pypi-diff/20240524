# Comparing `tmp/frogr-0.0.0.tar.gz` & `tmp/frogr-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frogr-0.0.0.tar", max compression
+gzip compressed data, was "frogr-0.0.1.tar", max compression
```

## Comparing `frogr-0.0.0.tar` & `frogr-0.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35878 2023-04-06 15:27:30.387575 frogr-0.0.0/LICENSE
--rw-r--r--   0        0        0     3831 2023-06-27 10:02:10.115842 frogr-0.0.0/README.md
--rw-r--r--   0        0        0     2107 2024-05-22 06:41:34.500610 frogr-0.0.0/pyproject.toml
--rw-r--r--   0        0        0    12292 2023-04-06 15:24:05.047964 frogr-0.0.0/src/frogr/.DS_Store
--rw-r--r--   0        0        0       14 2023-04-06 15:27:30.398672 frogr-0.0.0/src/frogr/__init__.py
--rw-r--r--   0        0        0      202 2023-04-06 16:31:29.335586 frogr-0.0.0/src/frogr/__main__.py
--rw-r--r--   0        0        0     8196 2023-01-19 18:50:01.701080 frogr-0.0.0/src/frogr/data/.DS_Store
--rw-r--r--   0        0        0    87372 2023-04-06 15:27:30.400274 frogr-0.0.0/src/frogr/data/chem/chem_dummy.ncdf
--rw-r--r--   0        0        0    11097 2023-04-06 15:27:30.401947 frogr-0.0.0/src/frogr/data/chem/coeff9_NASA_sc.dat
--rwxr-xr-x   0        0        0    92675 2023-04-06 15:27:30.402954 frogr-0.0.0/src/frogr/data/chem/coeff_NASA_mb.dat
--rw-r--r--   0        0        0   104159 2023-04-06 15:27:30.404212 frogr-0.0.0/src/frogr/data/chem/coeff_NASA_sc.dat
--rw-r--r--   0        0        0      276 2023-04-06 15:27:30.404793 frogr-0.0.0/src/frogr/data/chem/general_input.in
--rw-r--r--   0        0        0    12956 2024-05-22 06:38:49.444200 frogr-0.0.0/src/frogr/io.py
--rw-r--r--   0        0        0        0 2023-04-06 15:27:30.405480 frogr-0.0.0/src/frogr/py.typed
--rw-r--r--   0        0        0     5568 2024-05-22 06:38:49.446444 frogr-0.0.0/src/frogr/runner.py
--rw-r--r--   0        0        0     8196 2023-01-19 18:50:06.720310 frogr-0.0.0/src/frogr/taurex/.DS_Store
--rw-r--r--   0        0        0     6008 2024-05-22 06:44:13.050571 frogr-0.0.0/src/frogr/taurex/__init__.py
--rw-r--r--   0        0        0     1066 2023-06-26 16:21:22.385056 frogr-0.0.0/src/frogr/util.py
--rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 frogr-0.0.0/setup.py
--rw-r--r--   0        0        0     4886 1970-01-01 00:00:00.000000 frogr-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35878 2023-04-06 15:27:30.387575 frogr-0.0.1/LICENSE
+-rw-r--r--   0        0        0     3831 2023-06-27 10:02:10.115842 frogr-0.0.1/README.md
+-rw-r--r--   0        0        0     2124 2024-05-24 11:00:51.993698 frogr-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0    12292 2023-04-06 15:24:05.047964 frogr-0.0.1/src/frogr/.DS_Store
+-rw-r--r--   0        0        0       14 2023-04-06 15:27:30.398672 frogr-0.0.1/src/frogr/__init__.py
+-rw-r--r--   0        0        0      202 2023-04-06 16:31:29.335586 frogr-0.0.1/src/frogr/__main__.py
+-rw-r--r--   0        0        0     8196 2023-01-19 18:50:01.701080 frogr-0.0.1/src/frogr/data/.DS_Store
+-rw-r--r--   0        0        0    87372 2023-04-06 15:27:30.400274 frogr-0.0.1/src/frogr/data/chem/chem_dummy.ncdf
+-rw-r--r--   0        0        0    11097 2023-04-06 15:27:30.401947 frogr-0.0.1/src/frogr/data/chem/coeff9_NASA_sc.dat
+-rwxr-xr-x   0        0        0    92675 2023-04-06 15:27:30.402954 frogr-0.0.1/src/frogr/data/chem/coeff_NASA_mb.dat
+-rw-r--r--   0        0        0   104159 2023-04-06 15:27:30.404212 frogr-0.0.1/src/frogr/data/chem/coeff_NASA_sc.dat
+-rw-r--r--   0        0        0      276 2023-04-06 15:27:30.404793 frogr-0.0.1/src/frogr/data/chem/general_input.in
+-rw-r--r--   0        0        0    12956 2024-05-22 06:38:49.444200 frogr-0.0.1/src/frogr/io.py
+-rw-r--r--   0        0        0        0 2023-04-06 15:27:30.405480 frogr-0.0.1/src/frogr/py.typed
+-rw-r--r--   0        0        0     5568 2024-05-22 06:38:49.446444 frogr-0.0.1/src/frogr/runner.py
+-rw-r--r--   0        0        0     8196 2023-01-19 18:50:06.720310 frogr-0.0.1/src/frogr/taurex/.DS_Store
+-rw-r--r--   0        0        0     6008 2024-05-22 06:44:13.050571 frogr-0.0.1/src/frogr/taurex/__init__.py
+-rw-r--r--   0        0        0     1066 2023-06-26 16:21:22.385056 frogr-0.0.1/src/frogr/util.py
+-rw-r--r--   0        0        0     4969 1970-01-01 00:00:00.000000 frogr-0.0.1/setup.py
+-rw-r--r--   0        0        0     4904 1970-01-01 00:00:00.000000 frogr-0.0.1/PKG-INFO
```

### Comparing `frogr-0.0.0/LICENSE` & `frogr-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frogr-0.0.0/README.md` & `frogr-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `frogr-0.0.0/pyproject.toml` & `frogr-0.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "frogr"
-version = "0.0.0"
+version = "0.0.1"
 description = "ATMOpy"
 authors = ["M. F. Bieger <mb987@exeter.ac.uk>"]
 license = "GPL-3.0"
 readme = "README.md"
-homepage = "https://github.com/mfbieger/atmopy"
-repository = "https://github.com/mfbieger/atmopy"
+homepage = "https://github.com/michellebieger/atmopy"
+repository = "https://github.com/michellebieger/atmopy"
 documentation = "https://atmopy.readthedocs.io"
 classifiers = ["Development Status :: 1 - Planning"]
 
 [tool.poetry.urls]
-Changelog = "https://github.com/mfbieger/atmopy/releases"
+Changelog = "https://github.com/michellebieger/atmopy/releases"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 taurex = "^3.1.1a0"
 astropy = "^5.1.1"
 scipy = "^1.9.3"
 matplotlib = "^3.7.1"
@@ -45,15 +45,15 @@
 sphinx-autobuild = ">=2021.3.14"
 sphinx-click = ">=3.0.2"
 typeguard = ">=2.13.3"
 xdoctest = { extras = ["colors"], version = ">=0.15.10" }
 myst-parser = { version = ">=0.16.1" }
 
 [tool.poetry.scripts]
-atmopy = "atmopy.__main__:main"
+frogr = "frogr.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
 black = { version = "^22.10.0", allow-prereleases = true }
 ipython = "^8.6.0"
 jupyterlab = "^3.5.0"
 
 [tool.coverage.paths]
@@ -80,13 +80,13 @@
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 
 [tool.poetry.plugins] # Optional super table
 
 [tool.poetry.plugins."taurex.plugins"]
-atmo = "atmopy.taurex"
+frogr = "atmopy.taurex"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `frogr-0.0.0/src/frogr/.DS_Store` & `frogr-0.0.1/src/frogr/.DS_Store`

 * *Files identical despite different names*

### Comparing `frogr-0.0.0/src/frogr/data/.DS_Store` & `frogr-0.0.1/src/frogr/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `frogr-0.0.0/src/frogr/data/chem/chem_dummy.ncdf` & `frogr-0.0.1/src/frogr/data/chem/chem_dummy.ncdf`

 * *Files identical despite different names*

### Comparing `frogr-0.0.0/src/frogr/data/chem/coeff9_NASA_sc.dat` & `frogr-0.0.1/src/frogr/data/chem/coeff9_NASA_sc.dat`

 * *Files identical despite different names*

### Comparing `frogr-0.0.0/src/frogr/data/chem/coeff_NASA_mb.dat` & `frogr-0.0.1/src/frogr/data/chem/coeff_NASA_mb.dat`

 * *Files identical despite different names*

### Comparing `frogr-0.0.0/src/frogr/data/chem/coeff_NASA_sc.dat` & `frogr-0.0.1/src/frogr/data/chem/coeff_NASA_sc.dat`

 * *Files identical despite different names*

### Comparing `frogr-0.0.0/src/frogr/io.py` & `frogr-0.0.1/src/frogr/io.py`

 * *Files identical despite different names*

### Comparing `frogr-0.0.0/src/frogr/runner.py` & `frogr-0.0.1/src/frogr/runner.py`

 * *Files identical despite different names*

### Comparing `frogr-0.0.0/src/frogr/taurex/.DS_Store` & `frogr-0.0.1/src/frogr/taurex/.DS_Store`

 * *Files identical despite different names*

### Comparing `frogr-0.0.0/src/frogr/taurex/__init__.py` & `frogr-0.0.1/src/frogr/taurex/__init__.py`

 * *Files identical despite different names*

### Comparing `frogr-0.0.0/src/frogr/util.py` & `frogr-0.0.1/src/frogr/util.py`

 * *Files identical despite different names*

### Comparing `frogr-0.0.0/setup.py` & `frogr-0.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,27 @@
  'ipywidgets>=8.0.4,<9.0.0',
  'matplotlib>=3.7.1,<4.0.0',
  'scipy>=1.9.3,<2.0.0',
  'taurex>=3.1.1a0,<4.0.0',
  'twine>=4.0.2,<5.0.0']
 
 entry_points = \
-{'console_scripts': ['atmopy = atmopy.__main__:main'],
- 'taurex.plugins': ['atmo = atmopy.taurex']}
+{'console_scripts': ['frogr = frogr.__main__:main'],
+ 'taurex.plugins': ['frogr = atmopy.taurex']}
 
 setup_kwargs = {
     'name': 'frogr',
-    'version': '0.0.0',
+    'version': '0.0.1',
     'description': 'ATMOpy',
     'long_description': '# frogr: from gas to retrieval\n\n[![PyPI](https://img.shields.io/pypi/v/atmopy.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/atmopy.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/atmopy)][python version]\n[![License](https://img.shields.io/pypi/l/atmopy)][license]\n\n[![Read the documentation at https://frogr-from-gas-to-retrieval.readthedocs.io/](https://img.shields.io/readthedocs/atmopy/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/mfbieger/atmopy/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/mfbieger/atmopy/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/frogr/\n[status]: https://pypi.org/project/frogr/\n[python version]: https://pypi.org/project/frogr\n[read the docs]: https://frogr-from-gas-to-retrieval.readthedocs.io/\n[tests]: https://github.com/michellebieger/frogr/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/michellebieger/frogr\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- Use the ATMO equilibrium chemistry plugin in your TauREx 3.1 forward models and retrievals.\n\n## Requirements\n\n- Ensure that you have a working installation of ATMO on your machine (https://www.gitlab.erc-atmo.eu/1-2d_tools/atmo). If you need access to ATMO, please contact Pascal Tremblin: pascal.tremblin@cea.fr\n- You will need a working installation of TauREx 3.1 on your machine, with associated required Python packages: https://taurex3-public.readthedocs.io/\n\n## Installation\n\n<!-- You can install _frogr_ via [pip] from [PyPI]:\n\n```console\n$ pip install frogr\n```\n\nAlternatively, clone this Github and install via terminal with. This is done by: -->\n\nYou can install _frogr_ by cloning this Github and installing via the terminal. This is done by:\n\nCloning the directory using:\n\n```console\n$ git clone https://github.com/michellebieger/frogr.git\n```\n\nMove into frogr\'s folder:\n\n```console\n$ cd frogr\n```\n\nInstall by then typing in:\n\n```console\n$ pip install .\n```\n\nIf you are unable to install, a common error for HPC systems can be the Poetry log install requirements, which dictate a high-level version of Python. Try creating a new conda environment and then try pip installing once more:\n\n```console\n$ conda create -n [insertpreferredenvname] python=3.8\n```\n\nYou can check the installation by importing frogr into Python:\n\n```console\n$ python -c "import atmopy"\n```\n\nTo check that TauREx 3.1 has correctly registered your plugin:\n\n```console\n$ taurex --plugins\n```\n\nIf there are no errors, you have been successful!\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n## License\n\nDistributed under the terms of the [GPL 3.0 license][license],\n_frogr_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems, please email michellebieger@live.com with a detailed description of the issue.\n\n<!-- please [file an issue] along with a detailed description. -->\n\n## Credits\n\nThis project was generated from [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n\n<!-- [file an issue]: https://github.com/mfbieger/frogr/issues -->\n\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/michellebieger/frogr/blob/main/LICENSE\n[contributor guide]: https://github.com/michellebieger/frogr/blob/main/CONTRIBUTING.md\n[command-line reference]: https://frogr-from-gas-to-retrieval.readthedocs.io/en/latest/usage.html\n',
     'author': 'M. F. Bieger',
     'author_email': 'mb987@exeter.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/mfbieger/atmopy',
+    'url': 'https://github.com/michellebieger/atmopy',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `frogr-0.0.0/PKG-INFO` & `frogr-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: frogr
-Version: 0.0.0
+Version: 0.0.1
 Summary: ATMOpy
-Home-page: https://github.com/mfbieger/atmopy
+Home-page: https://github.com/michellebieger/atmopy
 License: GPL-3.0
 Author: M. F. Bieger
 Author-email: mb987@exeter.ac.uk
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: astropy (>=5.1.1,<6.0.0)
 Requires-Dist: ipywidgets (>=8.0.4,<9.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
 Requires-Dist: taurex (>=3.1.1a0,<4.0.0)
 Requires-Dist: twine (>=4.0.2,<5.0.0)
-Project-URL: Changelog, https://github.com/mfbieger/atmopy/releases
+Project-URL: Changelog, https://github.com/michellebieger/atmopy/releases
 Project-URL: Documentation, https://atmopy.readthedocs.io
-Project-URL: Repository, https://github.com/mfbieger/atmopy
+Project-URL: Repository, https://github.com/michellebieger/atmopy
 Description-Content-Type: text/markdown
 
 # frogr: from gas to retrieval
 
 [![PyPI](https://img.shields.io/pypi/v/atmopy.svg)][pypi_]
 [![Status](https://img.shields.io/pypi/status/atmopy.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/atmopy)][python version]
```

