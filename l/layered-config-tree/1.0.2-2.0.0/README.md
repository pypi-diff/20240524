# Comparing `tmp/layered_config_tree-1.0.2.tar.gz` & `tmp/layered_config_tree-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layered_config_tree-1.0.2.tar", last modified: Fri Apr 26 21:35:52 2024, max compression
+gzip compressed data, was "layered_config_tree-2.0.0.tar", last modified: Fri May 24 15:10:49 2024, max compression
```

## Comparing `layered_config_tree-1.0.2.tar` & `layered_config_tree-2.0.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.450951 layered_config_tree-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.446951 layered_config_tree-1.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.446951 layered_config_tree-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/.github/workflows/update_readme.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-26 21:35:52.450951 layered_config_tree-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.446951 layered_config_tree-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.446951 layered_config_tree-1.0.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.446951 layered_config_tree-1.0.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/docs/source/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.446951 layered_config_tree-1.0.2/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/python_versions.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 21:35:52.450951 layered_config_tree-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.442951 layered_config_tree-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.446951 layered_config_tree-1.0.2/src/layered_config_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/src/layered_config_tree/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/src/layered_config_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 21:35:52.000000 layered_config_tree-1.0.2/src/layered_config_tree/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/src/layered_config_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19980 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/src/layered_config_tree/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.450951 layered_config_tree-1.0.2/src/layered_config_tree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-26 21:35:52.000000 layered_config_tree-1.0.2/src/layered_config_tree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-26 21:35:52.000000 layered_config_tree-1.0.2/src/layered_config_tree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 21:35:52.000000 layered_config_tree-1.0.2/src/layered_config_tree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 21:35:48.000000 layered_config_tree-1.0.2/src/layered_config_tree.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-26 21:35:52.000000 layered_config_tree-1.0.2/src/layered_config_tree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-26 21:35:52.000000 layered_config_tree-1.0.2/src/layered_config_tree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.450951 layered_config_tree-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17155 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/tests/test_basic_functionality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.450951 layered_config_tree-1.0.2/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/tests/test_data/mock_model_specification.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/tests/test_data/mock_model_specification.yml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/tests/test_ingestion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/update_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:10:49.460974 layered_config_tree-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:10:49.456974 layered_config_tree-2.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:10:49.456974 layered_config_tree-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/.github/workflows/update_readme.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-24 15:10:49.460974 layered_config_tree-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:10:49.456974 layered_config_tree-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:10:49.456974 layered_config_tree-2.0.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:10:49.456974 layered_config_tree-2.0.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:10:49.456974 layered_config_tree-2.0.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/python_versions.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 15:10:49.460974 layered_config_tree-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:10:49.452974 layered_config_tree-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:10:49.456974 layered_config_tree-2.0.0/src/layered_config_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/src/layered_config_tree/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/src/layered_config_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 15:10:49.000000 layered_config_tree-2.0.0/src/layered_config_tree/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/src/layered_config_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21513 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/src/layered_config_tree/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/src/layered_config_tree/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:10:49.460974 layered_config_tree-2.0.0/src/layered_config_tree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-24 15:10:49.000000 layered_config_tree-2.0.0/src/layered_config_tree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-24 15:10:49.000000 layered_config_tree-2.0.0/src/layered_config_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:10:49.000000 layered_config_tree-2.0.0/src/layered_config_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:10:45.000000 layered_config_tree-2.0.0/src/layered_config_tree.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-24 15:10:49.000000 layered_config_tree-2.0.0/src/layered_config_tree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 15:10:49.000000 layered_config_tree-2.0.0/src/layered_config_tree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:10:49.460974 layered_config_tree-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18405 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/tests/test_basic_functionality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:10:49.460974 layered_config_tree-2.0.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/tests/test_data/mock_model_specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/tests/test_data/mock_model_specification.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/tests/test_ingestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-24 15:10:39.000000 layered_config_tree-2.0.0/update_readme.py
```

### Comparing `layered_config_tree-1.0.2/.github/pull_request_template.md` & `layered_config_tree-2.0.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.2/.github/workflows/build.yml` & `layered_config_tree-2.0.0/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -44,17 +44,18 @@
         run: |
           python -m pip install --upgrade pip
       - name: Install dependencies
         run: |
           pip install .[dev]
       - name: Lint
         run: |
-          pip install black==22.3.0 isort
+          pip install black==22.3.0 isort mypy
           black . --check --diff
           isort . --check --verbose --only-modified --diff
+          mypy .
       - name: Test
         run: |
           if "${{ github.event_name == 'schedule' }}"; then
             pytest --runslow ./tests
           else
             pytest ./tests
           fi
```

### Comparing `layered_config_tree-1.0.2/.github/workflows/deploy.yml` & `layered_config_tree-2.0.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.2/.github/workflows/update_readme.yml` & `layered_config_tree-2.0.0/.github/workflows/update_readme.yml`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.2/.gitignore` & `layered_config_tree-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.2/.readthedocs.yaml` & `layered_config_tree-2.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.2/CODE_OF_CONDUCT.rst` & `layered_config_tree-2.0.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.2/CONTRIBUTING.rst` & `layered_config_tree-2.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.2/LICENSE.txt` & `layered_config_tree-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.2/PKG-INFO` & `layered_config_tree-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layered_config_tree
-Version: 1.0.2
+Version: 2.0.0
 Summary: Layered Config Tree is a configuration structure which supports cascading layers.
 Home-page: https://github.com/ihmeuw/layered_config_tree
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -34,22 +34,27 @@
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: sphinx-click; extra == "dev"
 Requires-Dist: IPython; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: sphinxcontrib-video; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
+Requires-Dist: black==22.3.0; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: types-PyYAML; extra == "dev"
+Requires-Dist: types-setuptools; extra == "dev"
 
 ===================
 Layered Config Tree
 ===================
 
 Layered Config Tree is a configuration structure that supports cascading layers.
 
-**Supported Python versions: 3.8, 3.9, 3.10, 3.11**
+**Supported Python versions: 3.9, 3.10, 3.11**
 
 You can install ``layered_config_tree`` from PyPI with pip:
 
   ``> pip install layered_config_tree``
 
 or build it from from source:
```

### Comparing `layered_config_tree-1.0.2/README.rst` & `layered_config_tree-2.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ===================
 Layered Config Tree
 ===================
 
 Layered Config Tree is a configuration structure that supports cascading layers.
 
-**Supported Python versions: 3.8, 3.9, 3.10, 3.11**
+**Supported Python versions: 3.9, 3.10, 3.11**
 
 You can install ``layered_config_tree`` from PyPI with pip:
 
   ``> pip install layered_config_tree``
 
 or build it from from source:
```

### Comparing `layered_config_tree-1.0.2/docs/Makefile` & `layered_config_tree-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.2/docs/source/conf.py` & `layered_config_tree-2.0.0/docs/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,37 +13,35 @@
 import sys
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 from pathlib import Path
 
-from docutils.nodes import Text
-from sphinx.ext.intersphinx import missing_reference
-
 import layered_config_tree
 
 base_dir = Path(layered_config_tree.__file__).parent
+from typing import Optional
 
-about = {}
+about: dict[str, str] = {}
 with (base_dir / "__about__.py").open() as f:
     exec(f.read(), about)
 
 sys.path.insert(0, str(Path("..").resolve()))
 
 # -- Project information -----------------------------------------------------
 
 project = about["__title__"]
 copyright = f'2024, {about["__author__"]}'
 author = about["__author__"]
 
 # The short X.Y version.
-version = layered_config_tree.__version__
+version = layered_config_tree.__version__  # type: ignore[attr-defined]
 # The full version, including alpha/beta/rc tags.
-release = layered_config_tree.__version__
+release = layered_config_tree.__version__  # type: ignore[attr-defined]
 
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 
 needs_sphinx = "4.0"
@@ -86,15 +84,15 @@
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = []
+exclude_patterns: list[Optional[str]] = []
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
 
@@ -135,15 +133,15 @@
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = f'{about["__title__"]}doc'
 
 
 # -- Options for LaTeX output ---------------------------------------------
 
-latex_elements = {
+latex_elements: dict[str, str] = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
     # Additional stuff for the LaTeX preamble.
@@ -219,33 +217,14 @@
 
 
 # -- nitpicky mode --------------------------------------------------------
 # Ensures that all references in the docs resolve.
 
 nitpicky = True
 
-nitpick_ignore = []
+nitpick_ignore: list[tuple[str, str]] = []
 # for line in open("../nitpick-exceptions"):
 #     if line.strip() == "" or line.startswith("#"):
 #         continue
 #     dtype, target = line.split(None, 1)
 #     target = target.strip()
 #     nitpick_ignore.append((dtype, target))
-
-
-# Fix sphinx warnings when for literal Ellipses in type hints.
-def setup(app):
-    app.connect("missing-reference", __sphinx_issue_8127)
-
-
-def __sphinx_issue_8127(app, env, node, contnode):
-    reftarget = node.get("reftarget", None)
-    if reftarget == "..":
-        node["reftype"] = "data"
-        node["reftarget"] = "Ellipsis"
-        text_node = next(iter(contnode.traverse(lambda n: n.tagname == "#text")))
-        replacement_node = Text("...", "")
-        if text_node.parent is not None:
-            text_node.parent.replace(text_node, replacement_node)
-        else:  # e.g. happens in rtype fields
-            contnode = replacement_node
-        return missing_reference(app, env, node, contnode)
```

### Comparing `layered_config_tree-1.0.2/setup.py` & `layered_config_tree-2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,35 +29,45 @@
     sys.exit(1)
 
 
 if __name__ == "__main__":
     base_dir = Path(__file__).parent
     src_dir = base_dir / "src"
 
-    about = {}
+    about: dict[str, str] = {}
     with (src_dir / "layered_config_tree" / "__about__.py").open() as f:
         exec(f.read(), about)
 
     with (base_dir / "README.rst").open() as f:
         long_description = f.read()
 
-    install_requirements = ["pyyaml>=5.1"]
+    install_requirements = [
+        "pyyaml>=5.1",
+    ]
     setup_requirements = ["setuptools_scm"]
     test_requirements = [
         "pytest",
         "pytest-mock",
     ]
     doc_requirements = [
         "sphinx>=4.0",
         "sphinx-rtd-theme",
         "sphinx-click",
         "IPython",
         "matplotlib",
         "sphinxcontrib-video",
     ]
+    dev_requirements = [
+        "black==22.3.0",
+        "isort",
+        "mypy",
+        # typing extensions
+        "types-PyYAML",
+        "types-setuptools",
+    ]
 
     setup(
         name=about["__title__"],
         description=about["__summary__"],
         long_description=long_description,
         license=about["__license__"],
         url=about["__uri__"],
@@ -80,15 +90,15 @@
         packages=find_packages(where="src"),
         include_package_data=True,
         install_requires=install_requirements,
         tests_require=test_requirements,
         extras_require={
             "docs": doc_requirements,
             "test": test_requirements,
-            "dev": doc_requirements + test_requirements,
+            "dev": doc_requirements + test_requirements + dev_requirements,
         },
         zip_safe=False,
         use_scm_version={
             "write_to": "src/layered_config_tree/_version.py",
             "write_to_template": '__version__ = "{version}"\n',
             "tag_regex": r"^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$",
         },
```

### Comparing `layered_config_tree-1.0.2/src/layered_config_tree/exceptions.py` & `layered_config_tree-2.0.0/src/layered_config_tree/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Any, Optional
+from typing import Optional
+
+from layered_config_tree.types import NestedDictValue
 
 
 class ConfigurationError(Exception):
     """Base class for configuration errors."""
 
     def __init__(self, message: str, value_name: Optional[str] = None):
         super().__init__(message)
@@ -26,13 +28,18 @@
         The original source of the configuration value.
     value
         The original configuration value.
 
     """
 
     def __init__(
-        self, message: str, name: str, layer: Optional[str], source: Optional[str], value: Any
+        self,
+        message: str,
+        name: str,
+        layer: Optional[str],
+        source: Optional[str],
+        value: NestedDictValue,
     ):
         self.layer = layer
         self.source = source
         self.value = value
         super().__init__(message, name)
```

### Comparing `layered_config_tree-1.0.2/src/layered_config_tree/main.py` & `layered_config_tree-2.0.0/src/layered_config_tree/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,24 +23,28 @@
     >>> config.section_a.item2
     'value2'
     >>> config.section_b.item1
     'value6'
 
 """
 
+from __future__ import annotations
+
+from collections.abc import Iterable
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Optional, Union
 
 import yaml
 
 from layered_config_tree import (
     ConfigurationError,
     ConfigurationKeyError,
     DuplicatedConfigurationError,
 )
+from layered_config_tree.types import InputData, NestedDict, NestedDictValue, NodeValue
 
 
 class ConfigNode:
     """A priority based configuration value.
 
     A :class:`ConfigNode` represents a single configuration value with
     priority-based layers.  The intent is to allow a value to be set from
@@ -63,56 +67,56 @@
     eases debugging and analysis of simulation code.
 
     This class should not be instantiated directly. All interaction should
     take place by manipulating a :class:`LayeredConfigTree` object.
 
     """
 
-    def __init__(self, layers: List[str], name: str):
+    def __init__(self, layers: list[str], name: str):
         self._name = name
         self._layers = layers
-        self._values = {}
+        self._values: dict[str, tuple[Optional[str], NodeValue]] = {}
         self._frozen = False
         self._accessed = False
 
     @property
     def name(self) -> str:
         """The name of this configuration value."""
         return self._name
 
     @property
     def accessed(self) -> bool:
         """Returns whether this node has been accessed."""
         return self._accessed
 
     @property
-    def metadata(self) -> List[Dict[str, Any]]:
+    def metadata(self) -> list[dict[str, Union[Optional[str], NodeValue]]]:
         """Returns all values and associated metadata for this node."""
         result = []
         for layer in self._layers:
             if layer in self._values:
                 result.append(
                     {
                         "layer": layer,
                         "source": self._values[layer][0],
                         "value": self._values[layer][1],
                     }
                 )
         return result
 
-    def freeze(self):
+    def freeze(self) -> None:
         """Causes the :class:`ConfigNode` node to become read only.
 
         This can be used to create a contract around when the configuration is
         modifiable.
 
         """
         self._frozen = True
 
-    def get_value(self, layer: Optional[str] = None) -> Any:
+    def get_value(self, layer: Optional[str] = None) -> NodeValue:
         """Returns the value at the specified layer.
 
         If no layer is specified, the outermost (highest priority) layer
         at which a value has been set will be used.
 
         Parameters
         ----------
@@ -125,15 +129,15 @@
             If no value has been set at any layer.
 
         """
         value = self._get_value_with_source(layer)[1]
         self._accessed = True
         return value
 
-    def update(self, value: Any, layer: Optional[str], source: Optional[str]):
+    def update(self, value: NodeValue, layer: Optional[str], source: Optional[str]) -> None:
         """Set a value for a layer with optional metadata about source.
 
         Parameters
         ----------
         value
             Data to store in the node.
         layer
@@ -172,15 +176,15 @@
                 layer=layer,
                 source=source,
                 value=value,
             )
         else:
             self._values[layer] = (source, value)
 
-    def _get_value_with_source(self, layer: Optional[str]) -> Tuple[str, Any]:
+    def _get_value_with_source(self, layer: Optional[str]) -> tuple[Optional[str], NodeValue]:
         """Returns a (source, value) tuple at the specified layer.
 
         If no layer is specified, the outermost (highest priority) layer
         at which a value has been set will be used.
 
         Parameters
         ----------
@@ -200,43 +204,49 @@
             if layer in self._values:
                 return self._values[layer]
 
         raise ConfigurationKeyError(
             f"No value stored in this ConfigNode {self.name}.", self.name
         )
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         return bool(self._values)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         out = []
         for m in reversed(self.metadata):
             layer, source, value = m.values()
             out.append(f"{layer}: {value}\n    source: {source}")
         return "\n".join(out)
 
-    def __str__(self):
+    def __str__(self) -> str:
         if not self:
             return ""
         layer, _, value = self.metadata[-1].values()
         return f"{layer}: {value}"
 
 
 class LayeredConfigTree:
     """A container for configuration information.
 
     Each configuration value is exposed as an attribute the value of which
     is determined by the outermost layer which has the key defined.
 
     """
 
+    # Define type annotations here since they're indirectly defined below
+    _layers: list[str]
+    _children: dict[str, Union["LayeredConfigTree", "ConfigNode"]]
+    _frozen: bool
+    _name: str
+
     def __init__(
         self,
-        data: Union[Dict, str, Path, "LayeredConfigTree"] = None,
-        layers: List[str] = None,
+        data: Optional[InputData] = None,
+        layers: list[str] = [],
         name: str = "",
     ):
         """
         Parameters
         ----------
         data
             The :class:`LayeredConfigTree` accepts many kinds of data:
@@ -266,64 +276,66 @@
         """
         self.__dict__["_layers"] = layers if layers else ["base"]
         self.__dict__["_children"] = {}
         self.__dict__["_frozen"] = False
         self.__dict__["_name"] = name
         self.update(data, layer=self._layers[0], source="initial data")
 
-    def freeze(self):
+    def freeze(self) -> None:
         """Causes the LayeredConfigTree to become read only.
 
         This is useful for loading and then freezing configurations that
         should not be modified at runtime.
 
         """
         self.__dict__["_frozen"] = True
         for child in self.values():
             child.freeze()
 
-    def items(self) -> Iterable[Tuple[str, Union["LayeredConfigTree", ConfigNode]]]:
+    def items(self) -> Iterable[tuple[str, Union["LayeredConfigTree", ConfigNode]]]:
         """Return an iterable of all (child_name, child) pairs."""
         return self._children.items()
 
     def keys(self) -> Iterable[str]:
         """Return an Iterable of all child names."""
         return self._children.keys()
 
-    def values(self) -> Iterable:
+    def values(self) -> Iterable[Union[LayeredConfigTree, ConfigNode]]:
         """Return an Iterable of all children."""
         return self._children.values()
 
-    def unused_keys(self) -> List[str]:
+    def unused_keys(self) -> list[str]:
         """Lists all values in the LayeredConfigTree that haven't been accessed."""
         unused = []
         for name, child in self.items():
             if isinstance(child, ConfigNode):
                 if not child.accessed:
                     unused.append(name)
             else:
                 for grandchild_name in child.unused_keys():
                     unused.append(f"{name}.{grandchild_name}")
         return unused
 
-    def to_dict(self) -> Dict:
+    def to_dict(self) -> NestedDict:
         """Converts the LayeredConfigTree into a nested dictionary.
 
         All metadata is lost in this conversion.
 
         """
         result = {}
         for name, child in self.items():
             if isinstance(child, ConfigNode):
                 result[name] = child.get_value(layer=None)
             else:
-                result[name] = child.to_dict()
+                result[name] = child.to_dict()  # type: ignore[assignment]
         return result
 
-    def get_from_layer(self, name: str, layer: str = None) -> Any:
+    def get_from_layer(
+        self, name: str, layer: Optional[str] = None
+    ) -> Union[NodeValue, "LayeredConfigTree"]:
         """Get a configuration value from the provided layer.
 
         If no layer is specified, the outermost (highest priority) layer
         at which a value has been set will be used.
 
         Parameters
         ----------
@@ -341,36 +353,36 @@
         if isinstance(child, ConfigNode):
             return child.get_value(layer)
         else:
             return child
 
     def update(
         self,
-        data: Union[Dict, str, Path, "LayeredConfigTree", None],
-        layer: str = None,
-        source: str = None,
-    ):
+        data: Optional[InputData],
+        layer: Optional[str] = None,
+        source: Optional[str] = None,
+    ) -> None:
         """Adds additional data into the :class:`LayeredConfigTree`.
 
         Parameters
         ----------
         data
             :func:`~LayeredConfigTree.update` accepts many types of data.
 
              - :class:`dict` : Flat or nested dictionaries may be provided.
                Keys of dictionaries at all levels must be strings.
-             - :class:`LayeredConfigTree` : Another :class:`LayeredConfigTree` can be
-               used. All source information will be ignored and the
-               provided layer and source will be used to set the metadata.
              - :class:`str` : Strings provided can be yaml formatted strings,
                which will be parsed into a dictionary using standard yaml
                parsing. Alternatively, a path to a yaml file may be provided
                and the file will be read in and parsed.
              - :class:`pathlib.Path` : A path object to a yaml file will
                be interpreted the same as a string representation.
+             - :class:`LayeredConfigTree` : Another :class:`LayeredConfigTree` can be
+               used. All source information will be ignored and the
+               provided layer and source will be used to set the metadata.
         layer
             The name of the layer to store the value in.  If no layer is
             provided, the value will be set in the outermost (highest priority)
             layer.
         source
             The source to attribute the value to.
 
@@ -387,50 +399,63 @@
 
         """
         if data is not None:
             data, source = self._coerce(data, source)
             for k, v in data.items():
                 self._set_with_metadata(k, v, layer, source)
 
-    def metadata(self, name: str) -> List[Dict[str, Any]]:
+    def metadata(self, name: str) -> list[NestedDict]:
         if name in self:
-            return self._children[name].metadata
+            return self._children[name].metadata  # type: ignore[return-value]
         name = f"{self._name}.{name}" if self._name else name
         raise ConfigurationKeyError(f"No configuration value with name {name}", name)
 
     @staticmethod
     def _coerce(
-        data: Union[Dict, str, Path, "LayeredConfigTree"], source: Union[str, None]
-    ) -> Tuple[Dict, Union[str, None]]:
+        data: InputData,
+        source: Optional[str],
+    ) -> tuple[NestedDict, Optional[str]]:
         """Coerces data into dictionary format."""
         if isinstance(data, dict):
             return data, source
         elif (isinstance(data, str) and data.endswith((".yaml", ".yml"))) or isinstance(
             data, Path
         ):
             source = source if source else str(data)
             with open(data) as f:
                 data = f.read()
             data = yaml.full_load(data)
+            if not isinstance(data, dict):
+                raise ValueError(
+                    f"Loaded yaml file {data} should be a dictionary but is type {type(data)}"
+                )
             return data, source
         elif isinstance(data, str):
             data = yaml.full_load(data)
+            if not isinstance(data, dict):
+                raise ValueError(
+                    f"Loaded yaml file {data} should be a dictionary but is type {type(data)}"
+                )
             return data, source
         elif isinstance(data, LayeredConfigTree):
             return data.to_dict(), source
         else:
             raise ConfigurationError(
                 f"LayeredConfigTree can only update from dictionaries, strings, paths and LayeredConfigTrees. "
                 f"You passed in {type(data)}",
                 value_name=None,
             )
 
     def _set_with_metadata(
-        self, name: str, value: Any, layer: Optional[str], source: Optional[str]
-    ):
+        self,
+        name: str,
+        value: Union[NestedDictValue, str, Path, "LayeredConfigTree"],
+        layer: Optional[str],
+        source: Optional[str],
+    ) -> None:
         """Set a value in the named layer with the given source.
 
         Parameters
         ----------
         name
             The name of the value.
         value
@@ -473,90 +498,93 @@
                 self._children[name] = ConfigNode(list(self._layers), name=self._name)
             if isinstance(self._children[name], LayeredConfigTree):
                 name = f"{self._name}.{name}" if self._name else name
                 raise ConfigurationError(
                     f"Can't assign a value to a LayeredConfigTree.", name
                 )
 
-        self._children[name].update(value, layer, source)
+        self._children[name].update(value, layer, source)  # type: ignore[arg-type]
 
-    def __setattr__(self, name, value):
+    def __setattr__(self, name: str, value: NestedDictValue) -> None:
         """Set a value on the outermost layer."""
         if name not in self:
             raise ConfigurationKeyError(
                 "New configuration keys can only be created with the update method.",
                 self._name,
             )
         self._set_with_metadata(name, value, layer=None, source=None)
 
-    def __setitem__(self, name, value):
+    def __setitem__(self, name: str, value: NestedDictValue) -> None:
         """Set a value on the outermost layer."""
         if name not in self:
             raise ConfigurationKeyError(
                 "New configuration keys can only be created with the update method.",
                 self._name,
             )
         self._set_with_metadata(name, value, layer=None, source=None)
 
-    def __getattr__(self, name):
+    # FIXME: We expect the return to be a ConfigNode or LayeredConfigTree but
+    # the type checker doesn't know what you're getting back in chained
+    # attribute calls. We return Any as a workaround.
+    def __getattr__(self, name: str) -> Any:
         """Get a value from the outermost layer in which it appears."""
         return self.get_from_layer(name)
 
     # We need custom definitions of __getstate__ and __setstate__
     # because of our custom attribute getters/setters.
     # Specifically:
     # * The pickle module will invoke our __getattr__ checking for __getstate__
     #   and __setstate__, and only catch AttributeError (not ConfigurationKeyError), and
     # * Calling __getattr__ before we have set up the state doesn't work,
     #   because it leads to an infinite loop looking for the module's
     #   actual attributes (not config keys)
-    def __getstate__(self):
+    def __getstate__(self) -> NestedDict:
         return self.__dict__
 
-    def __setstate__(self, state: Dict):
+    def __setstate__(self, state: NestedDict) -> None:
         for k, v in state.items():
             self.__dict__[k] = v
 
-    def __getitem__(self, name):
+    def __getitem__(self, name: str) -> Union[NodeValue, "LayeredConfigTree"]:
         """Get a value from the outermost layer in which it appears."""
         return self.get_from_layer(name)
 
-    def __delattr__(self, name):
+    def __delattr__(self, name: str) -> None:
         if name in self:
             del self._children[name]
 
-    def __delitem__(self, name):
+    def __delitem__(self, name: str) -> None:
         if name in self:
             del self._children[name]
 
-    def __contains__(self, name):
+    def __contains__(self, name: str) -> bool:
         """Test if a configuration key exists in any layer."""
         return name in self._children
 
-    def __iter__(self):
+    def __iter__(self) -> Iterable[str]:
         """Dictionary-like iteration."""
         return iter(self._children)
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._children)
 
-    def __dir__(self):
+    def __dir__(self) -> list[str]:
         return list(self._children.keys()) + dir(super(LayeredConfigTree, self))
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "\n".join(
             [
                 "{}:\n    {}".format(name, repr(c).replace("\n", "\n    "))
                 for name, c in self._children.items()
             ]
         )
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "\n".join(
             [
                 "{}:\n    {}".format(name, str(c).replace("\n", "\n    "))
                 for name, c in self._children.items()
             ]
         )
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         raise NotImplementedError
```

### Comparing `layered_config_tree-1.0.2/src/layered_config_tree.egg-info/PKG-INFO` & `layered_config_tree-2.0.0/src/layered_config_tree.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layered_config_tree
-Version: 1.0.2
+Version: 2.0.0
 Summary: Layered Config Tree is a configuration structure which supports cascading layers.
 Home-page: https://github.com/ihmeuw/layered_config_tree
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -34,22 +34,27 @@
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: sphinx-click; extra == "dev"
 Requires-Dist: IPython; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: sphinxcontrib-video; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
+Requires-Dist: black==22.3.0; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: types-PyYAML; extra == "dev"
+Requires-Dist: types-setuptools; extra == "dev"
 
 ===================
 Layered Config Tree
 ===================
 
 Layered Config Tree is a configuration structure that supports cascading layers.
 
-**Supported Python versions: 3.8, 3.9, 3.10, 3.11**
+**Supported Python versions: 3.9, 3.10, 3.11**
 
 You can install ``layered_config_tree`` from PyPI with pip:
 
   ``> pip install layered_config_tree``
 
 or build it from from source:
```

### Comparing `layered_config_tree-1.0.2/src/layered_config_tree.egg-info/SOURCES.txt` & `layered_config_tree-2.0.0/src/layered_config_tree.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 docs/source/_static/style.css
 docs/source/_templates/layout.html
 src/layered_config_tree/__about__.py
 src/layered_config_tree/__init__.py
 src/layered_config_tree/_version.py
 src/layered_config_tree/exceptions.py
 src/layered_config_tree/main.py
+src/layered_config_tree/types.py
 src/layered_config_tree.egg-info/PKG-INFO
 src/layered_config_tree.egg-info/SOURCES.txt
 src/layered_config_tree.egg-info/dependency_links.txt
 src/layered_config_tree.egg-info/not-zip-safe
 src/layered_config_tree.egg-info/requires.txt
 src/layered_config_tree.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `layered_config_tree-1.0.2/tests/conftest.py` & `layered_config_tree-2.0.0/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from pathlib import Path
 
 import pytest
 
 
-def pytest_addoption(parser):
+def pytest_addoption(parser: pytest.Parser) -> None:
     parser.addoption("--runslow", action="store_true", default=False, help="run slow tests")
 
 
-def pytest_configure(config):
+def pytest_configure(config: pytest.Config) -> None:
     config.addinivalue_line("markers", "slow: mark test as slow to run")
 
 
-def pytest_collection_modifyitems(config, items):
+def pytest_collection_modifyitems(
+    config: pytest.Config, items: list[pytest.Function]
+) -> None:
     if config.getoption("--runslow"):
         # --runslow given in cli: do not skip slow tests
         return
     skip_slow = pytest.mark.skip(reason="need --runslow option to run")
     for item in items:
         if "slow" in item.keywords:
             item.add_marker(skip_slow)
 
 
 @pytest.fixture
-def test_data_dir():
+def test_data_dir() -> Path:
     data_dir = Path(__file__).resolve().parent / "test_data"
     assert data_dir.exists(), "Test directory structure is broken"
     return data_dir
 
 
 @pytest.fixture(params=[".yaml", ".yml"])
-def test_spec(request, test_data_dir):
+def test_spec(request: pytest.FixtureRequest, test_data_dir: Path) -> Path:
     return test_data_dir / f"mock_model_specification{request.param}"
```

### Comparing `layered_config_tree-1.0.2/tests/test_basic_functionality.py` & `layered_config_tree-2.0.0/tests/test_basic_functionality.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,163 +1,168 @@
 import pickle
 import textwrap
+from pathlib import Path
 
 import pytest
 import yaml
 
 from layered_config_tree import (
     ConfigNode,
     ConfigurationError,
     ConfigurationKeyError,
     DuplicatedConfigurationError,
     LayeredConfigTree,
 )
+from layered_config_tree.types import NestedDict
 
 
 @pytest.fixture(params=list(range(1, 5)))
-def layers(request):
+def layers(request: pytest.FixtureRequest) -> list[str]:
     return [f"layer_{i}" for i in range(1, request.param + 1)]
 
 
 @pytest.fixture
-def layers_and_values(layers):
+def layers_and_values(layers: list[str]) -> dict[str, str]:
     return {layer: f"test_value_{i+1}" for i, layer in enumerate(layers)}
 
 
 @pytest.fixture
-def empty_node(layers):
+def empty_node(layers: list[str]) -> ConfigNode:
     return ConfigNode(layers, name="test_node")
 
 
 @pytest.fixture
-def full_node(layers_and_values):
+def full_node(layers_and_values: dict[str, str]) -> ConfigNode:
     n = ConfigNode(list(layers_and_values.keys()), name="test_node")
     for layer, value in layers_and_values.items():
         n.update(value, layer, source=None)
     return n
 
 
 @pytest.fixture
-def empty_tree(layers):
+def empty_tree(layers: list[str]) -> LayeredConfigTree:
     return LayeredConfigTree(layers=layers)
 
 
-def test_node_creation(empty_node):
+def test_node_creation(empty_node: ConfigNode) -> None:
     assert not empty_node
     assert not empty_node.accessed
     assert not empty_node.metadata
     assert not repr(empty_node)
     assert not str(empty_node)
 
 
-def test_full_node_update(full_node):
+def test_full_node_update(full_node: ConfigNode) -> None:
     assert full_node
     assert not full_node.accessed
     assert len(full_node.metadata) == len(full_node._layers)
     assert repr(full_node)
     assert str(full_node)
 
 
-def test_node_update_no_args():
+def test_node_update_no_args() -> None:
     n = ConfigNode(["base"], name="test_node")
-    n.update("test_value", layer=None, source=None)
-    assert n._values["base"] == (None, "test_value")
+    n.update("test_value", layer=None, source="some_source")
+    assert n._values["base"] == ("some_source", "test_value")
 
     n = ConfigNode(["layer_1", "layer_2"], name="test_node")
-    n.update("test_value", layer=None, source=None)
+    n.update("test_value", layer=None, source="some_source")
     assert "layer_1" not in n._values
-    assert n._values["layer_2"] == (None, "test_value")
+    assert n._values["layer_2"] == ("some_source", "test_value")
 
 
-def test_node_update_with_args():
-    n = ConfigNode(["base"], name="test_node")
-    n.update("test_value", layer=None, source="test")
-    assert n._values["base"] == ("test", "test_value")
-
-    n = ConfigNode(["base"], name="test_node")
-    n.update("test_value", layer="base", source="test")
-    assert n._values["base"] == ("test", "test_value")
-
-    n = ConfigNode(["layer_1", "layer_2"], name="test_node")
-    n.update("test_value", layer=None, source="test")
-    assert "layer_1" not in n._values
-    assert n._values["layer_2"] == ("test", "test_value")
-
-    n = ConfigNode(["layer_1", "layer_2"], name="test_node")
-    n.update("test_value", layer="layer_1", source="test")
-    assert "layer_2" not in n._values
-    assert n._values["layer_1"] == ("test", "test_value")
-
-    n = ConfigNode(["layer_1", "layer_2"], name="test_node")
-    n.update("test_value", layer="layer_2", source="test")
-    assert "layer_1" not in n._values
-    assert n._values["layer_2"] == ("test", "test_value")
-
-    n = ConfigNode(["layer_1", "layer_2"], name="test_node")
-    n.update("test_value", layer="layer_1", source="test")
-    n.update("test_value", layer="layer_2", source="test")
-    assert n._values["layer_1"] == ("test", "test_value")
-    assert n._values["layer_2"] == ("test", "test_value")
-
-
-def test_node_frozen_update():
-    n = ConfigNode(["base"], name="test_node")
-    n.freeze()
+def test_node_update_with_args() -> None:
+    cn = ConfigNode(["base"], name="test_node")
+    cn.update("test_value", layer=None, source="test")
+    assert cn._values["base"] == ("test", "test_value")
+
+    cn = ConfigNode(["base"], name="test_node")
+    cn.update("test_value", layer="base", source="test")
+    assert cn._values["base"] == ("test", "test_value")
+
+    cn = ConfigNode(["layer_1", "layer_2"], name="test_node")
+    cn.update("test_value", layer=None, source="test")
+    assert "layer_1" not in cn._values
+    assert cn._values["layer_2"] == ("test", "test_value")
+
+    cn = ConfigNode(["layer_1", "layer_2"], name="test_node")
+    cn.update("test_value", layer="layer_1", source="test")
+    assert "layer_2" not in cn._values
+    assert cn._values["layer_1"] == ("test", "test_value")
+
+    cn = ConfigNode(["layer_1", "layer_2"], name="test_node")
+    cn.update("test_value", layer="layer_2", source="test")
+    assert "layer_1" not in cn._values
+    assert cn._values["layer_2"] == ("test", "test_value")
+
+    cn = ConfigNode(["layer_1", "layer_2"], name="test_node")
+    cn.update("test_value", layer="layer_1", source="test")
+    cn.update("test_value", layer="layer_2", source="test")
+    assert cn._values["layer_1"] == ("test", "test_value")
+    assert cn._values["layer_2"] == ("test", "test_value")
+
+
+def test_node_frozen_update() -> None:
+    cn = ConfigNode(["base"], name="test_node")
+    cn.freeze()
     with pytest.raises(ConfigurationError):
-        n.update("test_val", layer=None, source=None)
+        cn.update("test_val", layer=None, source=None)
 
 
-def test_node_bad_layer_update():
-    n = ConfigNode(["base"], name="test_node")
+def test_node_bad_layer_update() -> None:
+    cn = ConfigNode(["base"], name="test_node")
     with pytest.raises(ConfigurationKeyError):
-        n.update("test_value", layer="layer_1", source=None)
+        cn.update("test_value", layer="layer_1", source=None)
 
 
-def test_node_duplicate_update():
-    n = ConfigNode(["base"], name="test_node")
-    n.update("test_value", layer=None, source=None)
+def test_node_duplicate_update() -> None:
+    cn = ConfigNode(["base"], name="test_node")
+    cn.update("test_value", layer=None, source=None)
     with pytest.raises(DuplicatedConfigurationError):
-        n.update("test_value", layer=None, source=None)
+        cn.update("test_value", layer=None, source=None)
 
 
-def test_node_get_value_with_source_empty(empty_node):
+def test_node_get_value_with_source_empty(empty_node: ConfigNode) -> None:
     with pytest.raises(ConfigurationKeyError):
         empty_node._get_value_with_source(layer=None)
 
     for layer in empty_node._layers:
         with pytest.raises(ConfigurationKeyError):
             empty_node._get_value_with_source(layer=layer)
 
     assert not empty_node.accessed
 
 
-def test_node_get_value_with_source(full_node):
+def test_node_get_value_with_source(full_node: ConfigNode) -> None:
     assert full_node._get_value_with_source(layer=None) == (
         None,
         f"test_value_{len(full_node._layers)}",
     )
 
     for i, layer in enumerate(full_node._layers):
-        assert full_node._get_value_with_source(layer=layer) == (None, f"test_value_{i+1}")
+        assert full_node._get_value_with_source(layer=layer) == (
+            None,
+            f"test_value_{i+1}",
+        )
 
     assert not full_node.accessed
 
 
-def test_node_get_value_empty(empty_node):
+def test_node_get_value_empty(empty_node: ConfigNode) -> None:
     with pytest.raises(ConfigurationKeyError):
         empty_node.get_value()
 
     for layer in empty_node._layers:
         with pytest.raises(ConfigurationKeyError):
             empty_node.get_value()
 
     assert not empty_node.accessed
 
 
-def test_node_get_value(full_node):
+def test_node_get_value(full_node: ConfigNode) -> None:
     assert full_node.get_value() == f"test_value_{len(full_node._layers)}"
     assert full_node.accessed
     full_node._accessed = False
 
     assert full_node.get_value(layer=None) == f"test_value_{len(full_node._layers)}"
     assert full_node.accessed
     full_node._accessed = False
@@ -166,363 +171,370 @@
         assert full_node.get_value(layer=layer) == f"test_value_{i + 1}"
         assert full_node.accessed
         full_node._accessed = False
 
     assert not full_node.accessed
 
 
-def test_node_repr():
-    n = ConfigNode(["base"], name="test_node")
-    n.update("test_value", layer="base", source="test")
-    s = """\
+def test_node_repr() -> None:
+    cn = ConfigNode(["base"], name="test_node")
+    cn.update("test_value", layer="base", source="test")
+    expected_str = """\
         base: test_value
             source: test"""
-    assert repr(n) == textwrap.dedent(s)
+    assert repr(cn) == textwrap.dedent(expected_str)
 
-    n = ConfigNode(["base", "layer_1"], name="test_node")
-    n.update("test_value", layer="base", source="test")
-    s = """\
+    cn = ConfigNode(["base", "layer_1"], name="test_node")
+    cn.update("test_value", layer="base", source="test")
+    expected_str = """\
         base: test_value
             source: test"""
-    assert repr(n) == textwrap.dedent(s)
+    assert repr(cn) == textwrap.dedent(expected_str)
 
-    n = ConfigNode(["base", "layer_1"], name="test_node")
-    n.update("test_value", layer=None, source="test")
-    s = """\
+    cn = ConfigNode(["base", "layer_1"], name="test_node")
+    cn.update("test_value", layer=None, source="test")
+    expected_str = """\
         layer_1: test_value
             source: test"""
-    assert repr(n) == textwrap.dedent(s)
+    assert repr(cn) == textwrap.dedent(expected_str)
 
-    n = ConfigNode(["base", "layer_1"], name="test_node")
-    n.update("test_value", layer="base", source="test")
-    n.update("test_value", layer="layer_1", source="test")
-    s = """\
+    cn = ConfigNode(["base", "layer_1"], name="test_node")
+    cn.update("test_value", layer="base", source="test")
+    cn.update("test_value", layer="layer_1", source="test")
+    expected_str = """\
         layer_1: test_value
             source: test
         base: test_value
             source: test"""
-    assert repr(n) == textwrap.dedent(s)
+    assert repr(cn) == textwrap.dedent(expected_str)
 
 
-def test_node_str():
-    n = ConfigNode(["base"], name="test_node")
-    n.update("test_value", layer="base", source="test")
-    s = "base: test_value"
-    assert str(n) == s
-
-    n = ConfigNode(["base", "layer_1"], name="test_node")
-    n.update("test_value", layer="base", source="test")
-    s = "base: test_value"
-    assert str(n) == s
-
-    n = ConfigNode(["base", "layer_1"], name="test_node")
-    n.update("test_value", layer=None, source="test")
-    s = "layer_1: test_value"
-    assert str(n) == s
-
-    n = ConfigNode(["base", "layer_1"], name="test_node")
-    n.update("test_value", layer="base", source="test")
-    n.update("test_value", layer="layer_1", source="test")
-    s = "layer_1: test_value"
-    assert str(n) == s
+def test_node_str() -> None:
+    cn = ConfigNode(["base"], name="test_node")
+    cn.update("test_value", layer="base", source="test")
+    expected_str = "base: test_value"
+    assert str(cn) == expected_str
+
+    cn = ConfigNode(["base", "layer_1"], name="test_node")
+    cn.update("test_value", layer="base", source="test")
+    expected_str = "base: test_value"
+    assert str(cn) == expected_str
+
+    cn = ConfigNode(["base", "layer_1"], name="test_node")
+    cn.update("test_value", layer=None, source="test")
+    expected_str = "layer_1: test_value"
+    assert str(cn) == expected_str
 
+    cn = ConfigNode(["base", "layer_1"], name="test_node")
+    cn.update("test_value", layer="base", source="test")
+    cn.update("test_value", layer="layer_1", source="test")
+    expected_str = "layer_1: test_value"
+    assert str(cn) == expected_str
 
-def test_tree_creation(empty_tree):
+
+def test_tree_creation(empty_tree: LayeredConfigTree) -> None:
     assert len(empty_tree) == 0
     assert not empty_tree.items()
     assert not empty_tree.values()
     assert not empty_tree.keys()
     assert not repr(empty_tree)
     assert not str(empty_tree)
     assert not empty_tree._children
     assert empty_tree.to_dict() == {}
 
 
-def test_tree_coerce_dict():
-    d, s = {}, "test"
-    assert LayeredConfigTree._coerce(d, s) == (d, s)
-    d, s = {"key": "val"}, "test"
-    assert LayeredConfigTree._coerce(d, s) == (d, s)
-    d = {"key1": {"sub_key1": ["val", "val", "val"], "sub_key2": "val"}, "key2": "val"}
-    s = "test"
-    assert LayeredConfigTree._coerce(d, s) == (d, s)
+def test_tree_coerce_dict() -> None:
+    data: NestedDict
+    data = {}
+    src = "test"
+    assert LayeredConfigTree._coerce(data, src) == (data, src)
+    data = {"key": "val"}
+    assert LayeredConfigTree._coerce(data, src) == (data, src)
+    data = {"key1": {"sub_key1": ["val", "val", "val"], "sub_key2": "val"}, "key2": "val"}
+    assert LayeredConfigTree._coerce(data, src) == (data, src)
 
 
-def test_tree_coerce_str():
-    d = """"""
-    s = "test"
-    assert LayeredConfigTree._coerce(d, s) == (None, s)
-    d = """\
+def test_tree_coerce_str() -> None:
+    src = "test"
+    data = """\
     key: val"""
-    assert LayeredConfigTree._coerce(d, s) == ({"key": "val"}, s)
-    d = """\
+    assert LayeredConfigTree._coerce(data, src) == ({"key": "val"}, src)
+    data = """\
     key1:
         sub_key1:
             - val
             - val
             - val
         sub_key2: val
     key2: val"""
-    r = {"key1": {"sub_key1": ["val", "val", "val"], "sub_key2": "val"}, "key2": "val"}
-    assert LayeredConfigTree._coerce(d, s) == (r, s)
-    d = """\
+    expected_dict = {
+        "key1": {"sub_key1": ["val", "val", "val"], "sub_key2": "val"},
+        "key2": "val",
+    }
+    assert LayeredConfigTree._coerce(data, src) == (expected_dict, src)
+    data = """\
         key1:
             sub_key1: [val, val, val]
             sub_key2: val
         key2: val"""
-    r = {"key1": {"sub_key1": ["val", "val", "val"], "sub_key2": "val"}, "key2": "val"}
-    assert LayeredConfigTree._coerce(d, s) == (r, s)
+    expected_dict = {
+        "key1": {"sub_key1": ["val", "val", "val"], "sub_key2": "val"},
+        "key2": "val",
+    }
+    assert LayeredConfigTree._coerce(data, src) == (expected_dict, src)
 
 
-def test_tree_coerce_yaml(tmpdir):
-    d = """\
+def test_tree_coerce_yaml(tmp_path: Path) -> None:
+    data_to_write = """\
      key1:
          sub_key1:
              - val
              - val
              - val
          sub_key2: [val, val]
      key2: val"""
-    r = {
+    expected_dict = {
         "key1": {"sub_key1": ["val", "val", "val"], "sub_key2": ["val", "val"]},
         "key2": "val",
     }
-    s = "test"
-    p = tmpdir.join("model_spec.yaml")
-    with p.open("w") as f:
-        f.write(d)
-    assert LayeredConfigTree._coerce(str(p), s) == (r, s)
-    assert LayeredConfigTree._coerce(str(p), None) == (r, str(p))
+    src = "test"
+    model_spec_path = tmp_path / "model_spec.yaml"
+    with model_spec_path.open("w") as f:
+        f.write(data_to_write)
+    assert LayeredConfigTree._coerce(str(model_spec_path), src) == (expected_dict, src)
+    assert LayeredConfigTree._coerce(str(model_spec_path), None) == (
+        expected_dict,
+        str(model_spec_path),
+    )
 
 
-def test_single_layer():
-    d = LayeredConfigTree()
-    d.update({"test_key": "test_value", "test_key2": "test_value2"})
+def test_single_layer() -> None:
+    lct = LayeredConfigTree()
+    lct.update({"test_key": "test_value", "test_key2": "test_value2"})
 
-    assert d.test_key == "test_value"
-    assert d.test_key2 == "test_value2"
+    assert lct.test_key == "test_value"
+    assert lct.test_key2 == "test_value2"
 
     with pytest.raises(DuplicatedConfigurationError):
-        d.test_key2 = "test_value3"
+        lct.test_key2 = "test_value3"
 
-    assert d.test_key2 == "test_value2"
-    assert d.test_key == "test_value"
+    assert lct.test_key2 == "test_value2"
+    assert lct.test_key == "test_value"
 
 
-def test_dictionary_style_access():
-    d = LayeredConfigTree()
-    d.update({"test_key": "test_value", "test_key2": "test_value2"})
+def test_dictionary_style_access() -> None:
+    lct = LayeredConfigTree()
+    lct.update({"test_key": "test_value", "test_key2": "test_value2"})
 
-    assert d["test_key"] == "test_value"
-    assert d["test_key2"] == "test_value2"
+    assert lct["test_key"] == "test_value"
+    assert lct["test_key2"] == "test_value2"
 
     with pytest.raises(DuplicatedConfigurationError):
-        d["test_key2"] = "test_value3"
+        lct["test_key2"] = "test_value3"
 
-    assert d["test_key2"] == "test_value2"
-    assert d["test_key"] == "test_value"
+    assert lct["test_key2"] == "test_value2"
+    assert lct["test_key"] == "test_value"
 
 
-def test_get_missing_key():
-    d = LayeredConfigTree()
+def test_get_missing_key() -> None:
+    lct = LayeredConfigTree()
     with pytest.raises(ConfigurationKeyError):
-        _ = d.missing_key
+        _ = lct.missing_key
 
 
-def test_set_missing_key():
-    d = LayeredConfigTree()
+def test_set_missing_key() -> None:
+    lct = LayeredConfigTree()
     with pytest.raises(ConfigurationKeyError):
-        d.missing_key = "test_value"
+        lct.missing_key = "test_value"
     with pytest.raises(ConfigurationKeyError):
-        d["missing_key"] = "test_value"
+        lct["missing_key"] = "test_value"
 
 
-def test_multiple_layer_get():
-    d = LayeredConfigTree(layers=["first", "second", "third"])
-    d._set_with_metadata("test_key", "test_with_source_value", "first", source=None)
-    d._set_with_metadata("test_key", "test_value2", "second", source=None)
-    d._set_with_metadata("test_key", "test_value3", "third", source=None)
+def test_multiple_layer_get() -> None:
+    lct = LayeredConfigTree(layers=["first", "second", "third"])
+    lct._set_with_metadata("test_key", "test_with_source_value", "first", source=None)
+    lct._set_with_metadata("test_key", "test_value2", "second", source=None)
+    lct._set_with_metadata("test_key", "test_value3", "third", source=None)
 
-    d._set_with_metadata("test_key2", "test_value4", "first", source=None)
-    d._set_with_metadata("test_key2", "test_value5", "second", source=None)
+    lct._set_with_metadata("test_key2", "test_value4", "first", source=None)
+    lct._set_with_metadata("test_key2", "test_value5", "second", source=None)
 
-    d._set_with_metadata("test_key3", "test_value6", "first", source=None)
+    lct._set_with_metadata("test_key3", "test_value6", "first", source=None)
 
-    assert d.test_key == "test_value3"
-    assert d.test_key2 == "test_value5"
-    assert d.test_key3 == "test_value6"
+    assert lct.test_key == "test_value3"
+    assert lct.test_key2 == "test_value5"
+    assert lct.test_key3 == "test_value6"
 
 
-def test_outer_layer_set():
-    d = LayeredConfigTree(layers=["inner", "outer"])
-    d._set_with_metadata("test_key", "test_value", "inner", source=None)
-    d._set_with_metadata("test_key", "test_value3", layer=None, source=None)
-    assert d.test_key == "test_value3"
-    assert d["test_key"] == "test_value3"
+def test_outer_layer_set() -> None:
+    lct = LayeredConfigTree(layers=["inner", "outer"])
+    lct._set_with_metadata("test_key", "test_value", "inner", source=None)
+    lct._set_with_metadata("test_key", "test_value3", layer=None, source=None)
+    assert lct.test_key == "test_value3"
+    assert lct["test_key"] == "test_value3"
 
-    d = LayeredConfigTree(layers=["inner", "outer"])
-    d._set_with_metadata("test_key", "test_value", "inner", source=None)
-    d.test_key = "test_value3"
-    assert d.test_key == "test_value3"
-    assert d["test_key"] == "test_value3"
+    lct = LayeredConfigTree(layers=["inner", "outer"])
+    lct._set_with_metadata("test_key", "test_value", "inner", source=None)
+    lct.test_key = "test_value3"
+    assert lct.test_key == "test_value3"
+    assert lct["test_key"] == "test_value3"
 
-    d = LayeredConfigTree(layers=["inner", "outer"])
-    d._set_with_metadata("test_key", "test_value", "inner", source=None)
-    d["test_key"] = "test_value3"
-    assert d.test_key == "test_value3"
-    assert d["test_key"] == "test_value3"
+    lct = LayeredConfigTree(layers=["inner", "outer"])
+    lct._set_with_metadata("test_key", "test_value", "inner", source=None)
+    lct["test_key"] = "test_value3"
+    assert lct.test_key == "test_value3"
+    assert lct["test_key"] == "test_value3"
 
 
-def test_update_dict():
-    d = LayeredConfigTree(layers=["inner", "outer"])
-    d.update({"test_key": "test_value", "test_key2": "test_value2"}, layer="inner")
-    d.update({"test_key": "test_value3"}, layer="outer")
+def test_update_dict() -> None:
+    lct = LayeredConfigTree(layers=["inner", "outer"])
+    lct.update({"test_key": "test_value", "test_key2": "test_value2"}, layer="inner")
+    lct.update({"test_key": "test_value3"}, layer="outer")
 
-    assert d.test_key == "test_value3"
-    assert d.test_key2 == "test_value2"
+    assert lct.test_key == "test_value3"
+    assert lct.test_key2 == "test_value2"
 
 
-def test_update_dict_nested():
-    d = LayeredConfigTree(layers=["inner", "outer"])
-    d.update(
+def test_update_dict_nested() -> None:
+    lct = LayeredConfigTree(layers=["inner", "outer"])
+    lct.update(
         {"test_container": {"test_key": "test_value", "test_key2": "test_value2"}},
         layer="inner",
     )
     with pytest.raises(DuplicatedConfigurationError):
-        d.update({"test_container": {"test_key": "test_value3"}}, layer="inner")
+        lct.update({"test_container": {"test_key": "test_value3"}}, layer="inner")
 
-    assert d.test_container.test_key == "test_value"
-    assert d.test_container.test_key2 == "test_value2"
+    assert lct.test_container.test_key == "test_value"
+    assert lct.test_container.test_key2 == "test_value2"
 
-    d.update({"test_container": {"test_key2": "test_value4"}}, layer="outer")
+    lct.update({"test_container": {"test_key2": "test_value4"}}, layer="outer")
 
-    assert d.test_container.test_key2 == "test_value4"
+    assert lct.test_container.test_key2 == "test_value4"
 
 
-def test_source_metadata():
-    d = LayeredConfigTree(layers=["inner", "outer"])
-    d.update({"test_key": "test_value"}, layer="inner", source="initial_load")
-    d.update({"test_key": "test_value2"}, layer="outer", source="update")
+def test_source_metadata() -> None:
+    lct = LayeredConfigTree(layers=["inner", "outer"])
+    lct.update({"test_key": "test_value"}, layer="inner", source="initial_load")
+    lct.update({"test_key": "test_value2"}, layer="outer", source="update")
 
-    assert d.metadata("test_key") == [
+    assert lct.metadata("test_key") == [
         {"layer": "inner", "source": "initial_load", "value": "test_value"},
         {"layer": "outer", "source": "update", "value": "test_value2"},
     ]
 
 
-def test_exception_on_source_for_missing_key():
-    d = LayeredConfigTree(layers=["inner", "outer"])
-    d.update({"test_key": "test_value"}, layer="inner", source="initial_load")
+def test_exception_on_source_for_missing_key() -> None:
+    lct = LayeredConfigTree(layers=["inner", "outer"])
+    lct.update({"test_key": "test_value"}, layer="inner", source="initial_load")
 
     with pytest.raises(ConfigurationKeyError):
-        d.metadata("missing_key")
+        lct.metadata("missing_key")
 
 
-def test_unused_keys():
-    d = LayeredConfigTree(
+def test_unused_keys() -> None:
+    lct = LayeredConfigTree(
         {"test_key": {"test_key2": "test_value", "test_key3": "test_value2"}}
     )
 
-    assert d.unused_keys() == ["test_key.test_key2", "test_key.test_key3"]
-
-    _ = d.test_key.test_key2
+    assert lct.unused_keys() == ["test_key.test_key2", "test_key.test_key3"]
+    _ = lct.test_key.test_key2
 
-    assert d.unused_keys() == ["test_key.test_key3"]
+    assert lct.unused_keys() == ["test_key.test_key3"]
 
-    _ = d.test_key.test_key3
+    _ = lct.test_key.test_key3
 
-    assert not d.unused_keys()
+    assert not lct.unused_keys()
 
 
-def test_to_dict_dict():
+def test_to_dict_dict() -> None:
     test_dict = {"configuration": {"time": {"start": {"year": 2000}}}}
-    config = LayeredConfigTree(test_dict)
-    assert config.to_dict() == test_dict
+    lct = LayeredConfigTree(test_dict)
+    assert lct.to_dict() == test_dict
 
 
-def test_to_dict_yaml(test_spec):
-    config = LayeredConfigTree(str(test_spec))
+def test_to_dict_yaml(test_spec: Path) -> None:
+    lct = LayeredConfigTree(str(test_spec))
     with test_spec.open() as f:
         yaml_config = yaml.full_load(f)
-    assert yaml_config == config.to_dict()
+    assert yaml_config == lct.to_dict()
 
 
-def test_equals():
+def test_equals() -> None:
     # TODO: Assert should succeed, instead of raising, once equality is
     # implemented for LayeredConfigTrees
     with pytest.raises(NotImplementedError):
         test_dict = {"configuration": {"time": {"start": {"year": 2000}}}}
-        config = LayeredConfigTree(test_dict)
-        config2 = LayeredConfigTree(test_dict.copy())
-        assert config == config2
+        lct = LayeredConfigTree(test_dict)
+        lct2 = LayeredConfigTree(test_dict.copy())
+        assert lct == lct2
 
 
-def test_to_from_pickle():
+def test_to_from_pickle() -> None:
     test_dict = {"configuration": {"time": {"start": {"year": 2000}}}}
     second_layer = {"configuration": {"time": {"start": {"year": 2001}}}}
-    config = LayeredConfigTree(test_dict, layers=["first_layer", "second_layer"])
-    config.update(second_layer, layer="second_layer")
-    unpickled = pickle.loads(pickle.dumps(config))
+    lct = LayeredConfigTree(test_dict, layers=["first_layer", "second_layer"])
+    lct.update(second_layer, layer="second_layer")
+    unpickled = pickle.loads(pickle.dumps(lct))
 
     # We can't just assert unpickled == config because
     # equals doesn't work with our custom attribute
     # accessor scheme (also why pickling didn't use to work).
     # See the previous xfailed test.
-    assert unpickled.to_dict() == config.to_dict()
-    assert unpickled._frozen == config._frozen
-    assert unpickled._name == config._name
-    assert unpickled._layers == config._layers
+    assert unpickled.to_dict() == lct.to_dict()
+    assert unpickled._frozen == lct._frozen
+    assert unpickled._name == lct._name
+    assert unpickled._layers == lct._layers
 
 
-def test_freeze():
-    config = LayeredConfigTree(data={"configuration": {"time": {"start": {"year": 2000}}}})
-    config.freeze()
+def test_freeze() -> None:
+    lct = LayeredConfigTree(data={"configuration": {"time": {"start": {"year": 2000}}}})
+    lct.freeze()
 
     with pytest.raises(ConfigurationError):
-        config.update(data={"configuration": {"time": {"end": {"year": 2001}}}})
+        lct.update(data={"configuration": {"time": {"end": {"year": 2001}}}})
 
 
-def test_retrieval_behavior():
+def test_retrieval_behavior() -> None:
     layer_inner = "inner"
     layer_middle = "middle"
     layer_outer = "outer"
 
     default_cfg_value = "value_a"
 
     layer_list = [layer_inner, layer_middle, layer_outer]
     # update the LayeredConfigTree layers in different order and verify that has no effect on
     #  the values retrieved ("outer" is retrieved when no layer is specified regardless of
     #  the initialization order
     for scenario in [layer_list, reversed(layer_list)]:
-        cfg = LayeredConfigTree(layers=layer_list)
+        lct = LayeredConfigTree(layers=layer_list)
         for layer in scenario:
-            cfg.update({default_cfg_value: layer}, layer=layer)
-        assert cfg.get_from_layer(default_cfg_value) == layer_outer
-        assert cfg.get_from_layer(default_cfg_value, layer=layer_outer) == layer_outer
-        assert cfg.get_from_layer(default_cfg_value, layer=layer_middle) == layer_middle
-        assert cfg.get_from_layer(default_cfg_value, layer=layer_inner) == layer_inner
+            lct.update({default_cfg_value: layer}, layer=layer)
+        assert lct.get_from_layer(default_cfg_value) == layer_outer
+        assert lct.get_from_layer(default_cfg_value, layer=layer_outer) == layer_outer
+        assert lct.get_from_layer(default_cfg_value, layer=layer_middle) == layer_middle
+        assert lct.get_from_layer(default_cfg_value, layer=layer_inner) == layer_inner
 
 
-def test_repr_display():
+def test_repr_display() -> None:
     expected_repr = """\
     Key1:
         override_2: value_ov_2
             source: ov2_src
         override_1: value_ov_1
             source: ov1_src
         base: value_base
             source: base_src"""
     # codifies the notion that repr() displays values from most to least overridden
     #  regardless of initialization order
     layers = ["base", "override_1", "override_2"]
-    cfg = LayeredConfigTree(layers=layers)
+    lct = LayeredConfigTree(layers=layers)
 
-    cfg.update({"Key1": "value_ov_2"}, layer="override_2", source="ov2_src")
-    cfg.update({"Key1": "value_ov_1"}, layer="override_1", source="ov1_src")
-    cfg.update({"Key1": "value_base"}, layer="base", source="base_src")
-    assert repr(cfg) == textwrap.dedent(expected_repr)
-
-    cfg = LayeredConfigTree(layers=layers)
-    cfg.update({"Key1": "value_base"}, layer="base", source="base_src")
-    cfg.update({"Key1": "value_ov_1"}, layer="override_1", source="ov1_src")
-    cfg.update({"Key1": "value_ov_2"}, layer="override_2", source="ov2_src")
-    assert repr(cfg) == textwrap.dedent(expected_repr)
+    lct.update({"Key1": "value_ov_2"}, layer="override_2", source="ov2_src")
+    lct.update({"Key1": "value_ov_1"}, layer="override_1", source="ov1_src")
+    lct.update({"Key1": "value_base"}, layer="base", source="base_src")
+    assert repr(lct) == textwrap.dedent(expected_repr)
+
+    lct = LayeredConfigTree(layers=layers)
+    lct.update({"Key1": "value_base"}, layer="base", source="base_src")
+    lct.update({"Key1": "value_ov_1"}, layer="override_1", source="ov1_src")
+    lct.update({"Key1": "value_ov_2"}, layer="override_2", source="ov2_src")
+    assert repr(lct) == textwrap.dedent(expected_repr)
```

### Comparing `layered_config_tree-1.0.2/update_readme.py` & `layered_config_tree-2.0.0/update_readme.py`

 * *Files identical despite different names*

