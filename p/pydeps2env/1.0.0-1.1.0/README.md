# Comparing `tmp/pydeps2env-1.0.0.tar.gz` & `tmp/pydeps2env-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeps2env-1.0.0.tar", last modified: Mon Mar 11 20:52:17 2024, max compression
+gzip compressed data, was "pydeps2env-1.1.0.tar", last modified: Fri May 24 08:28:07 2024, max compression
```

## Comparing `pydeps2env-1.0.0.tar` & `pydeps2env-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 20:52:17.093450 pydeps2env-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-03-11 20:52:17.004792 pydeps2env-1.0.0/.github/
-drwxrwxrwx   0        0        0        0 2024-03-11 20:52:17.031337 pydeps2env-1.0.0/.github/workflows/
--rw-rw-rw-   0        0        0     1375 2024-03-11 20:49:58.000000 pydeps2env-1.0.0/.github/workflows/test.yml
--rw-rw-rw-   0        0        0      864 2024-03-11 20:17:45.000000 pydeps2env-1.0.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1549 2024-03-09 09:26:55.000000 pydeps2env-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     6762 2024-03-11 20:52:17.091421 pydeps2env-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3787 2024-03-11 20:49:58.000000 pydeps2env-1.0.0/README.md
--rw-rw-rw-   0        0        0     2010 2024-03-11 20:49:58.000000 pydeps2env-1.0.0/action.yml
-drwxrwxrwx   0        0        0        0 2024-03-11 20:52:17.046712 pydeps2env-1.0.0/pydeps2env/
--rw-rw-rw-   0        0        0      262 2024-03-09 09:26:55.000000 pydeps2env-1.0.0/pydeps2env/__init__.py
--rw-rw-rw-   0        0        0      427 2024-03-11 20:52:16.000000 pydeps2env-1.0.0/pydeps2env/_version.py
--rw-rw-rw-   0        0        0     7751 2024-03-11 20:17:45.000000 pydeps2env-1.0.0/pydeps2env/environment.py
--rw-rw-rw-   0        0        0     2007 2024-03-11 20:19:26.000000 pydeps2env-1.0.0/pydeps2env/generate_environment.py
-drwxrwxrwx   0        0        0        0 2024-03-11 20:52:17.089419 pydeps2env-1.0.0/pydeps2env.egg-info/
--rw-rw-rw-   0        0        0     6762 2024-03-11 20:52:16.000000 pydeps2env-1.0.0/pydeps2env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2024-03-11 20:52:16.000000 pydeps2env-1.0.0/pydeps2env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 20:52:16.000000 pydeps2env-1.0.0/pydeps2env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-03-11 20:52:16.000000 pydeps2env-1.0.0/pydeps2env.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2024-03-11 20:52:16.000000 pydeps2env-1.0.0/pydeps2env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-11 20:52:16.000000 pydeps2env-1.0.0/pydeps2env.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1700 2024-03-09 09:26:55.000000 pydeps2env-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-11 20:52:17.093450 pydeps2env-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-11 20:52:17.087421 pydeps2env-1.0.0/test/
--rw-rw-rw-   0        0        0       92 2024-03-11 20:19:28.000000 pydeps2env-1.0.0/test/environment.yaml
--rw-rw-rw-   0        0        0      704 2024-03-11 20:17:45.000000 pydeps2env-1.0.0/test/pyproject.toml
--rw-rw-rw-   0        0        0       21 2024-03-11 20:17:45.000000 pydeps2env-1.0.0/test/requirements.txt
--rw-rw-rw-   0        0        0      437 2024-03-11 20:17:45.000000 pydeps2env-1.0.0/test/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 08:28:07.849813 pydeps2env-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-05-24 08:28:07.582126 pydeps2env-1.1.0/.github/
+drwxrwxrwx   0        0        0        0 2024-05-24 08:28:07.656145 pydeps2env-1.1.0/.github/workflows/
+-rw-rw-rw-   0        0        0     1708 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/.github/workflows/test.yml
+-rw-rw-rw-   0        0        0     3353 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/.gitignore
+-rw-rw-rw-   0        0        0      860 2024-05-24 06:39:01.000000 pydeps2env-1.1.0/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1549 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     8649 2024-05-24 08:28:07.838356 pydeps2env-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5649 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/README.md
+-rw-rw-rw-   0        0        0     2524 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/action.yml
+drwxrwxrwx   0        0        0        0 2024-05-24 08:28:07.694659 pydeps2env-1.1.0/pydeps2env/
+-rw-rw-rw-   0        0        0      485 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/pydeps2env/__init__.py
+-rw-rw-rw-   0        0        0      427 2024-05-24 08:28:07.000000 pydeps2env-1.1.0/pydeps2env/_version.py
+-rw-rw-rw-   0        0        0    10476 2024-05-24 06:38:57.000000 pydeps2env-1.1.0/pydeps2env/environment.py
+-rw-rw-rw-   0        0        0     4987 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/pydeps2env/generate_environment.py
+drwxrwxrwx   0        0        0        0 2024-05-24 08:28:07.829795 pydeps2env-1.1.0/pydeps2env.egg-info/
+-rw-rw-rw-   0        0        0     8649 2024-05-24 08:28:07.000000 pydeps2env-1.1.0/pydeps2env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      634 2024-05-24 08:28:07.000000 pydeps2env-1.1.0/pydeps2env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 08:28:07.000000 pydeps2env-1.1.0/pydeps2env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-24 08:28:07.000000 pydeps2env-1.1.0/pydeps2env.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2024-05-24 08:28:07.000000 pydeps2env-1.1.0/pydeps2env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-24 08:28:07.000000 pydeps2env-1.1.0/pydeps2env.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1835 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 08:28:07.849813 pydeps2env-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 08:28:07.803475 pydeps2env-1.1.0/test/
+-rw-rw-rw-   0        0        0      817 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/test/definition.yaml
+-rw-rw-rw-   0        0        0       92 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/test/environment.yaml
+-rw-rw-rw-   0        0        0      133 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/test/local.yaml
+-rw-rw-rw-   0        0        0      805 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/test/pyproject.toml
+-rw-rw-rw-   0        0        0       34 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/test/requirements.txt
+-rw-rw-rw-   0        0        0      437 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/test/setup.cfg
+-rw-rw-rw-   0        0        0     2071 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/test/test_environment.py
+drwxrwxrwx   0        0        0        0 2024-05-24 08:28:07.811923 pydeps2env-1.1.0/test/test_package/
+-rw-rw-rw-   0        0        0      892 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/test/test_package/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-24 08:28:07.822682 pydeps2env-1.1.0/test/test_package/testproject/
+-rw-rw-rw-   0        0        0       85 2024-05-23 11:04:28.000000 pydeps2env-1.1.0/test/test_package/testproject/__init__.py
```

### Comparing `pydeps2env-1.0.0/.github/workflows/test.yml` & `pydeps2env-1.1.0/.github/workflows/test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 on: [push, pull_request, workflow_dispatch]
 
 jobs:
+  pytest:
+    name: pytest
+    runs-on: ubuntu-latest
+    strategy:
+      fail-fast: false
+    steps:
+    - uses: actions/checkout@v4
+    - uses: actions/setup-python@v5
+      with:
+        python-version: '3.10'
+    - name: pip install package
+      run: pip install .[test]
+    - name: run pytest
+      run: pytest
+
   demo_job:
     name: action
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
```

### Comparing `pydeps2env-1.0.0/.pre-commit-config.yaml` & `pydeps2env-1.1.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
   - id: trailing-whitespace
     args: [--markdown-linebreak-ext=md]
   - id: end-of-file-fixer
   - id: check-yaml
   # ----- Python formatting -----
-- repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: v0.3.2
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  rev: v0.4.4
   hooks:
       # Run ruff linter.
   - id: ruff
     args:
     - --quiet
     - --fix
       # Run ruff formatter.
   - id: ruff-format
   # ----- repo maintenance -----
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.12.0
+  rev: v2.13.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --indent, '2']
 - repo: https://github.com/tox-dev/pyproject-fmt
-  rev: 1.7.0
+  rev: 2.1.3
   hooks:
   - id: pyproject-fmt
 - repo: https://github.com/abravalheri/validate-pyproject
-  rev: v0.16
+  rev: v0.18
   hooks:
   - id: validate-pyproject
```

### Comparing `pydeps2env-1.0.0/LICENSE` & `pydeps2env-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeps2env-1.0.0/PKG-INFO` & `pydeps2env-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeps2env
-Version: 1.0.0
+Version: 1.1.0
 Summary: A python helper to generate conda environment files from project dependencies.
 Author-email: Çağtay Fabry <cagtay.fabry@bam.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Cagtay Fabry
         All rights reserved.
         
@@ -48,23 +48,23 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging
 Requires-Dist: pyyaml
-Requires-Dist: tomli
+Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 # pydeps2env
 
 An easy way to create conda environment files from you python project dependencies.  
-Creates a conda `environment.yml` file from python package dependencies listed in a `pyproject.toml` or `setup.cfg` file.
+Creates a conda `environment.yml` file from python package dependencies listed in on or multiple different source formats like `pyproject.toml`, `setup.cfg`, `environment.yaml` or `requirements.txt` files.
 
 The project contains
 - GitHub action
 - python package
 - command line script
 
 ```mermaid
@@ -97,15 +97,15 @@
     "boltons",
 ]
 [project.optional-dependencies]
 test = ["pytest"]
 pip_only = ["bidict"]
 ```
 
-The default parameters will output this sorted `environment.yml` (note that the `python` dependency will always be the first item on the list):
+The default parameters will output this sorted `environment.yml` (note that the `python` dependency specification will always be the first item on the list):
 
 ```yaml
 channels:
   - defaults
 dependencies:
   - python>=3.8,<3.10
   - boltons
@@ -129,21 +129,79 @@
   - setuptools>=40.9.0
   - setuptools_scm
   - wheel
   - pip:
     - bidict
 ```
 
-## configuration options
+## basic usage (python)
+
+Create an `Environment` using Python and export it to an `environment.yaml` file.
+
+```python
+from pydeps2env import Environment
+
+env = Environment("./test/pyproject.toml[doc]")
+env.export("my_environment.yaml")
+```
+
+## basic usage (command line)
+
+Combine multiple source files into a single environment file (including build dependencies).
+Install pandas using `pip`.
+
+```bash
+pydeps2env ./test/setup.cfg ./test/pyproject.toml[doc] ./test/environment.yaml ./test/requirements.txt -o output.yaml -c defaults --extras test -b include --pip pandas
+```
+
+## advanced usage (definition file)
+
+Users can store complex configurations in a single yaml file and create the desired output using `create_from_definition`.
+Example definition file:
+
+```yaml
+# the target file to create
+output: test-configuration.yaml
+# default name of the environment
+name: test-env
+# conda channels to include
+channels:
+- conda-forge
+- defaults
+# list of source files that define sub environments
+# these will be loaded as Environment()
+sources:
+- ./test/environment.yaml
+- ./test/local.yaml
+- ./test/pyproject.toml[doc]
+- ./test/requirements.txt
+- https://github.com/CagtayFabry/pydeps2env/blob/custom_deps/pyproject.toml
+# extras to apply to all sources and packages
+extras:
+- test
+# dependencies that should be removed after collection
+remove:
+- pyyaml
+additional_requirements:
+- urllib3
+# include build system dependencies
+# list of dependencies that must be pip installed (excluding auto-sorted depedencies like urls)
+pip:
+- urllib3
+include_build_system: include
+
+```
+
+## configuration options (GitHub action)
 
 To customize the output the input options are available to the action:
 
 ### files
 
-Specify the location of the `'setup.cfg'` or `'pyproject.toml'` files to parse. (defaults to `'pyproject.toml'`)
+Specify the location of the dependencies files to parse. (defaults to 'pyproject.toml')
 Multiple files can be listed. This will result in a combined environment file.
 
 ### output:
 
 Specify the location and name of the conda environment file to generate. (defaults to `'environment.yml'`)
 
 ### channels:
@@ -160,15 +218,16 @@
 ### build_system:
 
 If set to `'include'` the dependencies listed under `[build-system]` (or `[options:setup_requires]` in `setup.cfg`) will be added to the environment (default
 is `'omit'` so no setup dependencies will be installed).
 
 ### pip
 List of packages to install via `pip` instead of `conda`.
-The dependencies will be listet under the `pip:` section in the environment file.
+The dependencies will be listed under the `pip:` section in the environment file.
+If a dependency is listed with its URN, it will always be installed via pip (e.g. `pydeps2env @ git+https://github.com/CagtayFabry/pydeps2env`)
 
 ## example
 
 ```yaml
 steps:
   - uses: CagtayFabry/pydeps2env@v1.0.0
     with:
```

### Comparing `pydeps2env-1.0.0/pydeps2env/environment.py` & `pydeps2env-1.1.0/pydeps2env/environment.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 from __future__ import annotations
 
-from dataclasses import dataclass, field
+from dataclasses import dataclass, field, InitVar
 from packaging.requirements import Requirement
 from pathlib import Path
 from collections import defaultdict
 import configparser
-import tomli as tomllib
+import sys
 import yaml
-import warnings
+from io import StringIO, BytesIO
+from warnings import warn
+
+if sys.version_info < (3, 11):
+    import tomli as tomllib
+else:
+    import tomllib
 
 
 def clean_list(item: list, sort: bool = True) -> list:
     """Remove duplicate entries from a list."""
     pass
 
 
 def split_extras(filename: str) -> tuple[str, set]:
     """Split extras requirements indicated in []."""
     if "[" in filename:
         filename, extras = filename.split("[", 1)
         extras = set(extras.split("]", 1)[0].split(","))
     else:
-        extras = {}
+        extras = set()
     return filename, extras
 
 
 def add_requirement(
     req: Requirement | str,
     requirements: dict[str, Requirement],
     mode: str = "combine",
@@ -35,14 +41,22 @@
     if not isinstance(req, Requirement):
         req = Requirement(req)
 
     if req.name not in requirements:
         requirements[req.name] = req
     elif mode == "combine":
         requirements[req.name].specifier &= req.specifier
+        if req.url:
+            if requirements[req.name].url and requirements[req.name].url != req.url:
+                warn(
+                    f"Replacing url for package {req.name}: {requirements[req.name].url} -> req.url",
+                    UserWarning,
+                    stacklevel=1,
+                )
+                requirements[req.name].url = req.url
     elif mode == "replace":
         requirements[req.name] = req
     else:
         raise ValueError(f"Unknown `mode` for add_requirement: {mode}")
 
 
 def combine_requirements(
@@ -57,160 +71,225 @@
 
 
 @dataclass
 class Environment:
     filename: str | Path
     channels: list[str] = field(default_factory=lambda: ["conda-forge"])
     extras: set[str] | list[str] = field(default_factory=set)
-    pip_packages: set[str] = field(default_factory=set)  # install via pip
+    pip_packages: set[str] = field(
+        default_factory=set
+    )  # names of packages to install via pip
+    extra_requirements: InitVar[list[str]] = None
     requirements: dict[str, Requirement] = field(default_factory=dict, init=False)
     build_system: dict[str, Requirement] = field(default_factory=dict, init=False)
 
-    def __post_init__(self):
+    def __post_init__(self, extra_requirements):
+        print(self.filename)
         # cleanup duplicates etc.
         self.extras = set(self.extras)
         self.channels = list(dict.fromkeys(self.channels))
         self.pip_packages = set(self.pip_packages)
 
+        if self.filename:
+            self._read_source()
+
+        if extra_requirements:
+            self.add_requirements(extra_requirements)
+
+        # packages with url specification must be pip installed
+        self.pip_packages |= {req.name for req in self.requirements.values() if req.url}
+
+    def add_requirements(self, requirements: list[str]):
+        """Add a list of additional requirements to the environment."""
+
+        for req in requirements:
+            add_requirement(req, self.requirements)
+
+    def add_build_system(self, requirements: list[str]):
+        """Manually add a list of additional requirements to the build system specification."""
+
+        for req in requirements:
+            add_requirement(req, self.build_system)
+
+    def _read_source(self):
+        """Read and parse source definition and add requirements."""
+
+        # parse and remove extra specs from filename
         if isinstance(self.filename, str):
             self.filename, extras = split_extras(self.filename)
             self.extras |= set(extras)
 
-        if Path(self.filename).suffix == ".toml":
-            self.load_pyproject()
-        elif Path(self.filename).suffix == ".cfg":
-            self.load_config()
-        elif Path(self.filename).suffix in [".yaml", ".yml"]:
-            self.load_yaml()
-        elif Path(self.filename).suffix in [".txt"]:
-            self.load_txt()
+        # store suffix for later parsing
+        self._suffix = Path(self.filename).suffix
+
+        # read file contents into bytes
+        _filename = self.filename
+        if isinstance(_filename, str) and _filename.startswith("http"):
+            import urllib.request
+
+            if "/github.com/" in _filename:
+                _filename = _filename.replace(
+                    "/github.com/", "/raw.githubusercontent.com/"
+                )
+                _filename = _filename.replace("/blob/", "/")
+            with urllib.request.urlopen(_filename) as f:
+                _contents: bytes = f.read()  # read raw content into bytes
+        else:
+            with open(_filename, "rb") as f:
+                _contents: bytes = f.read()
+
+        if self._suffix == ".toml":
+            self.load_pyproject(_contents)
+        elif self._suffix == ".cfg":
+            self.load_config(_contents)
+        elif self._suffix in [".yaml", ".yml"]:
+            self.load_yaml(_contents)
+        elif self._suffix in [".txt"]:
+            self.load_txt(_contents)
         else:
             raise ValueError(f"Unsupported input {self.filename}")
 
-    def load_pyproject(self):
+    def load_pyproject(self, contents: bytes):
         """Load contents from a toml file (assume pyproject.toml layout)."""
-        with open(self.filename, "rb") as fh:
-            cp = defaultdict(dict, tomllib.load(fh))
 
-        if python := cp["project"].get("requires-python"):
-            add_requirement("python" + python, self.requirements)
+        tomldict = tomllib.load(BytesIO(contents))
+        cp = defaultdict(dict, tomldict)
 
-        for dep in cp.get("project").get("dependencies"):
-            add_requirement(dep, self.requirements)
-
-        for dep in cp.get("build-system").get("requires"):
-            add_requirement(dep, self.build_system)
+        if python := cp["project"].get("requires-python"):
+            self.add_requirements(["python" + python])
 
+        self.add_requirements(cp.get("project").get("dependencies"))
+        self.add_build_system(cp.get("build-system").get("requires"))
         for e in self.extras:
-            extra_deps = cp.get("project").get("optional-dependencies").get(e)
-            if not extra_deps:
-                continue
-            for dep in extra_deps:
-                add_requirement(dep, self.requirements)
+            self.add_requirements(cp.get("project").get("optional-dependencies").get(e))
 
-    def load_config(self):
+    def load_config(self, contents: bytes):
         """Load contents from a cfg file (assume setup.cfg layout)."""
         cp = configparser.ConfigParser(
             converters={
                 "list": lambda x: [i.strip() for i in x.split("\n") if i.strip()]
             }
         )
-        cp.read(self.filename)
 
-        if python := cp.get("options", "python_requires"):
-            add_requirement("python" + python, self.requirements)
+        cp.read_string(contents.decode("UTF-8"))
 
-        for dep in cp.getlist("options", "install_requires"):
-            add_requirement(dep, self.requirements)
-
-        for dep in cp.getlist("options", "setup_requires"):
-            add_requirement(dep, self.build_system)
+        if python := cp.get("options", "python_requires"):
+            self.add_requirements(["python" + python])
 
+        self.add_requirements(cp.getlist("options", "install_requires"))
+        self.add_build_system(cp.getlist("options", "setup_requires"))
         for e in self.extras:
-            extra_deps = cp.getlist("options.extras_require", e)
-            if not extra_deps:
-                continue
-            for dep in extra_deps:
-                add_requirement(dep, self.requirements)
+            self.add_requirements(cp.getlist("options.extras_require", e))
 
-    def load_yaml(self):
+    def load_yaml(self, contents: bytes):
         """Load a conda-style environment.yaml file."""
-        with open(self.filename, "r") as f:
-            env = yaml.load(f.read(), yaml.SafeLoader)
+        env = yaml.load(contents.decode(), yaml.SafeLoader)
 
         self.channels += env.get("channels", [])
         self.channels = list(dict.fromkeys(self.channels))
 
         for dep in env.get("dependencies"):
             if isinstance(dep, str):
                 add_requirement(dep, self.requirements)
             elif isinstance(dep, dict) and "pip" in dep:
                 add_requirement("pip", self.requirements)
                 for pip_dep in dep["pip"]:
                     req = Requirement(pip_dep)
                     self.pip_packages |= {req.name}
                     add_requirement(req, self.requirements)
 
-    def load_txt(self):
+    def load_txt(self, contents: bytes):
         """Load simple list of requirements from txt file."""
-        with open(self.filename, "r") as f:
-            deps = f.readlines()
+        deps = StringIO(contents.decode()).readlines()
 
-        for dep in deps:
-            add_requirement(dep, self.requirements)
+        self.add_requirements([dep.strip() for dep in deps])
 
     def _get_dependencies(
-        self, include_build_system: bool = True
+        self,
+        include_build_system: bool = True,
+        remove: list[str] = None,
     ) -> tuple[list[str], list[str]]:
         """Get the default conda environment entries."""
 
+        if remove is None:
+            remove = []
+
         reqs = self.requirements.copy()
         if include_build_system:
             reqs = combine_requirements(reqs, self.build_system)
 
         _python = reqs.pop("python", None)
 
-        deps = [str(r) for r in reqs.values() if r.name not in self.pip_packages]
+        _pip_packages = self.pip_packages
+        # _pip_packages |= {r.name for r in reqs.values() if r.url}
+
+        deps = [
+            str(r)
+            for r in reqs.values()
+            if not r.url  # install via pip
+            and r.name not in _pip_packages
+            and r.name not in remove
+        ]
         deps.sort(key=str.lower)
         if _python:
             deps = [str(_python)] + deps
 
-        pip = [str(r) for r in reqs.values() if r.name in self.pip_packages]
+        pip = [
+            r
+            for r in reqs.values()
+            if (r.name in _pip_packages or r.url) and r.name not in remove
+        ]
+        # string formatting
+        pip = [str(r) if not r.url else f"{r.name}@ {r.url}" for r in pip]
         pip.sort(key=str.lower)
 
         return deps, pip
 
     def export(
         self,
         outfile: str | Path = "environment.yaml",
         include_build_system: bool = True,
+        remove: list[str] = None,
+        name: str = None,
     ):
-        deps, pip = self._get_dependencies(include_build_system=include_build_system)
+        """Export the environment to a yaml or txt file."""
+        if remove is None:
+            remove = []
 
-        conda_env = {"channels": self.channels, "dependencies": deps.copy()}
+        deps, pip = self._get_dependencies(
+            include_build_system=include_build_system, remove=remove
+        )
+
+        conda_env = {
+            "name": name,
+            "channels": self.channels,
+            "dependencies": deps.copy(),
+        }
         if pip:
             if "pip" not in self.requirements:
                 conda_env["dependencies"] += ["pip"]
             conda_env["dependencies"] += [{"pip": pip}]
 
+        conda_env = {k: v for k, v in conda_env.items() if v}
+
         if outfile is None:
             return conda_env
 
         p = Path(outfile)
         if p.suffix in [".txt"]:
             deps += pip
             deps.sort(key=str.lower)
             with open(p, "w") as outfile:
                 outfile.writelines("\n".join(deps))
         else:
             if p.suffix not in [".yaml", ".yml"]:
-                warnings.warn(
+                warn(
                     f"Unknown environment format `{p.suffix}`, generating conda yaml output."
                 )
             with open(p, "w") as outfile:
-                yaml.dump(conda_env, outfile, default_flow_style=False)
+                yaml.dump(conda_env, outfile, default_flow_style=False, sort_keys=False)
 
     def combine(self, other: Environment):
         """Merge other Environment requirements into this Environment."""
         self.requirements = combine_requirements(self.requirements, other.requirements)
         self.build_system = combine_requirements(self.build_system, other.build_system)
         self.pip_packages = self.pip_packages | other.pip_packages
```

### Comparing `pydeps2env-1.0.0/pydeps2env.egg-info/PKG-INFO` & `pydeps2env-1.1.0/pydeps2env.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeps2env
-Version: 1.0.0
+Version: 1.1.0
 Summary: A python helper to generate conda environment files from project dependencies.
 Author-email: Çağtay Fabry <cagtay.fabry@bam.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Cagtay Fabry
         All rights reserved.
         
@@ -48,23 +48,23 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging
 Requires-Dist: pyyaml
-Requires-Dist: tomli
+Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 # pydeps2env
 
 An easy way to create conda environment files from you python project dependencies.  
-Creates a conda `environment.yml` file from python package dependencies listed in a `pyproject.toml` or `setup.cfg` file.
+Creates a conda `environment.yml` file from python package dependencies listed in on or multiple different source formats like `pyproject.toml`, `setup.cfg`, `environment.yaml` or `requirements.txt` files.
 
 The project contains
 - GitHub action
 - python package
 - command line script
 
 ```mermaid
@@ -97,15 +97,15 @@
     "boltons",
 ]
 [project.optional-dependencies]
 test = ["pytest"]
 pip_only = ["bidict"]
 ```
 
-The default parameters will output this sorted `environment.yml` (note that the `python` dependency will always be the first item on the list):
+The default parameters will output this sorted `environment.yml` (note that the `python` dependency specification will always be the first item on the list):
 
 ```yaml
 channels:
   - defaults
 dependencies:
   - python>=3.8,<3.10
   - boltons
@@ -129,21 +129,79 @@
   - setuptools>=40.9.0
   - setuptools_scm
   - wheel
   - pip:
     - bidict
 ```
 
-## configuration options
+## basic usage (python)
+
+Create an `Environment` using Python and export it to an `environment.yaml` file.
+
+```python
+from pydeps2env import Environment
+
+env = Environment("./test/pyproject.toml[doc]")
+env.export("my_environment.yaml")
+```
+
+## basic usage (command line)
+
+Combine multiple source files into a single environment file (including build dependencies).
+Install pandas using `pip`.
+
+```bash
+pydeps2env ./test/setup.cfg ./test/pyproject.toml[doc] ./test/environment.yaml ./test/requirements.txt -o output.yaml -c defaults --extras test -b include --pip pandas
+```
+
+## advanced usage (definition file)
+
+Users can store complex configurations in a single yaml file and create the desired output using `create_from_definition`.
+Example definition file:
+
+```yaml
+# the target file to create
+output: test-configuration.yaml
+# default name of the environment
+name: test-env
+# conda channels to include
+channels:
+- conda-forge
+- defaults
+# list of source files that define sub environments
+# these will be loaded as Environment()
+sources:
+- ./test/environment.yaml
+- ./test/local.yaml
+- ./test/pyproject.toml[doc]
+- ./test/requirements.txt
+- https://github.com/CagtayFabry/pydeps2env/blob/custom_deps/pyproject.toml
+# extras to apply to all sources and packages
+extras:
+- test
+# dependencies that should be removed after collection
+remove:
+- pyyaml
+additional_requirements:
+- urllib3
+# include build system dependencies
+# list of dependencies that must be pip installed (excluding auto-sorted depedencies like urls)
+pip:
+- urllib3
+include_build_system: include
+
+```
+
+## configuration options (GitHub action)
 
 To customize the output the input options are available to the action:
 
 ### files
 
-Specify the location of the `'setup.cfg'` or `'pyproject.toml'` files to parse. (defaults to `'pyproject.toml'`)
+Specify the location of the dependencies files to parse. (defaults to 'pyproject.toml')
 Multiple files can be listed. This will result in a combined environment file.
 
 ### output:
 
 Specify the location and name of the conda environment file to generate. (defaults to `'environment.yml'`)
 
 ### channels:
@@ -160,15 +218,16 @@
 ### build_system:
 
 If set to `'include'` the dependencies listed under `[build-system]` (or `[options:setup_requires]` in `setup.cfg`) will be added to the environment (default
 is `'omit'` so no setup dependencies will be installed).
 
 ### pip
 List of packages to install via `pip` instead of `conda`.
-The dependencies will be listet under the `pip:` section in the environment file.
+The dependencies will be listed under the `pip:` section in the environment file.
+If a dependency is listed with its URN, it will always be installed via pip (e.g. `pydeps2env @ git+https://github.com/CagtayFabry/pydeps2env`)
 
 ## example
 
 ```yaml
 steps:
   - uses: CagtayFabry/pydeps2env@v1.0.0
     with:
```

### Comparing `pydeps2env-1.0.0/pyproject.toml` & `pydeps2env-1.1.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,25 @@
+[build-system]
+build-backend = "setuptools.build_meta"
+requires = [
+  "setuptools>=64",
+  "setuptools-scm[toml]>=6.2",
+]
+
 [project]
 name = "pydeps2env"
 description = "A python helper to generate conda environment files from project dependencies."
-readme = {file = "README.md", content-type="text/markdown"}
+readme = { file = "README.md", content-type = "text/markdown" }
 keywords = [
   "conda",
   "pyproject",
 ]
-license = {file = "LICENSE", name="BSD License"}
+license = { file = "LICENSE", name = "BSD License" }
 authors = [
-    {name="Çağtay Fabry", email="cagtay.fabry@bam.de"},
+  { name = "Çağtay Fabry", email = "cagtay.fabry@bam.de" },
 ]
 requires-python = ">=3.9"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: BSD License",
   "Natural Language :: English",
@@ -27,33 +34,32 @@
 dynamic = [
   # see: https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html#dynamic-metadata
   "version", # version gets derived from git by setuptools_scm.
 ]
 dependencies = [
   "packaging",
   "pyyaml",
-  "tomli",
+  "tomli; python_version<'3.11'",
 ]
-[project.optional-dependencies]
-test = [
+optional-dependencies.test = [
   # needed to run the test suite
   "pytest",
   "pytest-cov",
 ]
-[project.urls]
-bug_tracker = "https://github.com/CagtayFabry/pydeps2env/-/issues"
-repository = "https://github.com/CagtayFabry/pydeps2env"
-[project.scripts]
-pydeps2env = "pydeps2env.generate_environment:main"
-
-[build-system]
-build-backend = "setuptools.build_meta"
-requires = [
-  "setuptools>=64",
-  "setuptools_scm[toml]>=6.2",
-]
+urls.bug_tracker = "https://github.com/CagtayFabry/pydeps2env/-/issues"
+urls.repository = "https://github.com/CagtayFabry/pydeps2env"
+scripts.pydeps2env = "pydeps2env.generate_environment:main"
 
 [tool.setuptools.packages]
-find = {exclude = ["test", "resources"]}
+find = { exclude = [
+  "test",
+  "resources",
+] }
 
 [tool.setuptools_scm]
 write_to = "pydeps2env/_version.py"
+
+[tool.pytest.ini_options]
+addopts = "--tb=short --color=yes -rsw --cov=pydeps2env"
+testpaths = [
+  "test",
+]
```

### Comparing `pydeps2env-1.0.0/test/pyproject.toml` & `pydeps2env-1.1.0/test/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,35 @@
+[build-system]
+build-backend = "setuptools.build_meta"
+requires = [
+  "setuptools>=40.9",
+  "setuptools-scm",
+  "wheel",
+]
+
 [project]
 name = "test"
 requires-python = ">=3.8,<3.10"
 classifiers = [
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
   "boltons",
-  "IPython",
+  "ipython",
   "numpy>=1.20",
   "pandas>=1",
+  "pydeps2env @ git+https://github.com/CagtayFabry/pydeps2env.git",
 ]
-[project.optional-dependencies]
-doc = [
+optional-dependencies.doc = [
   "sphinx",
 ]
-pip_only = [
+optional-dependencies.pip_only = [
   "bidict",
 ]
-test = [
+optional-dependencies.test = [
   "pytest",
 ]
-[project.urls]
-author = "Cagtay Fabry <cagtay.fabry@bam.de>"
-author_email = "cagtay.fabry@bam.de"
-home_page = "https://github.com/CagtayFabry/pydeps2env"
-
-[build-system]
-build-backend = "setuptools.build_meta"
-requires = [
-  "setuptools>=40.9",
-  "setuptools_scm",
-  "wheel",
-]
+urls.author = "Cagtay Fabry <cagtay.fabry@bam.de>"
+urls.author_email = "cagtay.fabry@bam.de"
+urls.home_page = "https://github.com/CagtayFabry/pydeps2env"
```

