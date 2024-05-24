# Comparing `tmp/behaverse-0.0.5.dev2.tar.gz` & `tmp/behaverse-0.0.5.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "behaverse-0.0.5.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "behaverse-0.0.5.dev3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `behaverse-0.0.5.dev2.tar` & `behaverse-0.0.5.dev3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1759 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/.github/workflows/docs-publish.yml
--rw-r--r--   0        0        0     1243 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      160 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/.gitignore
--rw-r--r--   0        0        0      158 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/.pypirc
--rw-r--r--   0        0        0      375 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/.vscode/settings.json
--rw-r--r--   0        0        0     1071 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/LICENSE
--rw-r--r--   0        0        0      890 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/README.md
--rw-r--r--   0        0        0       54 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/docs/.gitignore
--rw-r--r--   0        0        0       22 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/docs/_extensions/machow/interlinks/.gitignore
--rw-r--r--   0        0        0      126 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/docs/_extensions/machow/interlinks/_extension.yml
--rw-r--r--   0        0        0     6853 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/docs/_extensions/machow/interlinks/interlinks.lua
--rw-r--r--   0        0        0     1367 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/docs/_quarto.yml
--rw-r--r--   0        0        0     1147 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/docs/getting_started.qmd
--rw-r--r--   0        0        0      261 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/docs/index.qmd
--rw-r--r--   0        0        0      829 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/docs/system_design.qmd
--rw-r--r--   0        0        0      209 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/environment.yml
--rw-r--r--   0        0        0     1724 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/examples/1 Getting Started with Behaverse Data.ipynb
--rw-r--r--   0        0        0     1788 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/pyproject.toml
--rw-r--r--   0        0        0      494 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/src/behaverse/__init__.py
--rw-r--r--   0        0        0      284 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/src/behaverse/additional_storage/huggingface.py
--rw-r--r--   0        0        0      276 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/src/behaverse/additional_storage/osf.py
--rw-r--r--   0        0        0      278 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/src/behaverse/additional_storage/ulhpc.py
--rw-r--r--   0        0        0      279 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/src/behaverse/additional_storage/zenodo.py
--rw-r--r--   0        0        0       27 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/src/behaverse/conftest.py
--rw-r--r--   0        0        0     7188 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/src/behaverse/dataset.py
--rw-r--r--   0        0        0      238 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/src/behaverse/dataset_description.py
--rw-r--r--   0        0        0     1694 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/src/behaverse/dataset_test.py
--rw-r--r--   0        0        0     1612 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/src/behaverse/dvc_storage.py
--rw-r--r--   0        0        0      535 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/src/behaverse/dvc_storage_test.py
--rw-r--r--   0        0        0     2487 2024-05-23 10:33:03.785006 behaverse-0.0.5.dev2/src/behaverse/functional.py
--rw-r--r--   0        0        0       28 2024-05-23 10:33:03.789006 behaverse-0.0.5.dev2/src/behaverse/functions_test.py
--rw-r--r--   0        0        0     2565 2024-05-23 10:33:03.789006 behaverse-0.0.5.dev2/src/behaverse/http_storage.py
--rw-r--r--   0        0        0     1898 2024-05-23 10:33:03.789006 behaverse-0.0.5.dev2/src/behaverse/utils.py
--rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 behaverse-0.0.5.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1781 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/.github/workflows/docs-publish.yml
+-rw-r--r--   0        0        0     1243 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      160 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/.gitignore
+-rw-r--r--   0        0        0      158 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/.pypirc
+-rw-r--r--   0        0        0      375 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/.vscode/settings.json
+-rw-r--r--   0        0        0     1071 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/LICENSE
+-rw-r--r--   0        0        0      984 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/README.md
+-rw-r--r--   0        0        0       54 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/docs/.gitignore
+-rw-r--r--   0        0        0       22 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/docs/_extensions/machow/interlinks/.gitignore
+-rw-r--r--   0        0        0      126 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/docs/_extensions/machow/interlinks/_extension.yml
+-rw-r--r--   0        0        0     6853 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/docs/_extensions/machow/interlinks/interlinks.lua
+-rw-r--r--   0        0        0     1367 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/docs/_quarto.yml
+-rw-r--r--   0        0        0     1147 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/docs/getting_started.qmd
+-rw-r--r--   0        0        0      261 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/docs/index.qmd
+-rw-r--r--   0        0        0     1255 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/docs/system_design.qmd
+-rw-r--r--   0        0        0      209 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/environment.yml
+-rw-r--r--   0        0        0     1724 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/examples/1 Getting Started with Behaverse Data.ipynb
+-rw-r--r--   0        0        0     1788 2024-05-23 11:50:42.756699 behaverse-0.0.5.dev3/pyproject.toml
+-rw-r--r--   0        0        0      494 2024-05-23 11:50:42.760699 behaverse-0.0.5.dev3/src/behaverse/__init__.py
+-rw-r--r--   0        0        0      284 2024-05-23 11:50:42.760699 behaverse-0.0.5.dev3/src/behaverse/additional_storage/huggingface.py
+-rw-r--r--   0        0        0      276 2024-05-23 11:50:42.760699 behaverse-0.0.5.dev3/src/behaverse/additional_storage/osf.py
+-rw-r--r--   0        0        0      278 2024-05-23 11:50:42.760699 behaverse-0.0.5.dev3/src/behaverse/additional_storage/ulhpc.py
+-rw-r--r--   0        0        0      279 2024-05-23 11:50:42.760699 behaverse-0.0.5.dev3/src/behaverse/additional_storage/zenodo.py
+-rw-r--r--   0        0        0       27 2024-05-23 11:50:42.760699 behaverse-0.0.5.dev3/src/behaverse/conftest.py
+-rw-r--r--   0        0        0     7188 2024-05-23 11:50:42.760699 behaverse-0.0.5.dev3/src/behaverse/dataset.py
+-rw-r--r--   0        0        0      238 2024-05-23 11:50:42.760699 behaverse-0.0.5.dev3/src/behaverse/dataset_description.py
+-rw-r--r--   0        0        0     1694 2024-05-23 11:50:42.760699 behaverse-0.0.5.dev3/src/behaverse/dataset_test.py
+-rw-r--r--   0        0        0     1619 2024-05-23 11:50:42.760699 behaverse-0.0.5.dev3/src/behaverse/dvc_storage.py
+-rw-r--r--   0        0        0      535 2024-05-23 11:50:42.760699 behaverse-0.0.5.dev3/src/behaverse/dvc_storage_test.py
+-rw-r--r--   0        0        0     2487 2024-05-23 11:50:42.760699 behaverse-0.0.5.dev3/src/behaverse/functional.py
+-rw-r--r--   0        0        0       28 2024-05-23 11:50:42.760699 behaverse-0.0.5.dev3/src/behaverse/functions_test.py
+-rw-r--r--   0        0        0     2565 2024-05-23 11:50:42.760699 behaverse-0.0.5.dev3/src/behaverse/http_storage.py
+-rw-r--r--   0        0        0     1898 2024-05-23 11:50:42.760699 behaverse-0.0.5.dev3/src/behaverse/utils.py
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 behaverse-0.0.5.dev3/PKG-INFO
```

### Comparing `behaverse-0.0.5.dev2/.github/workflows/docs-publish.yml` & `behaverse-0.0.5.dev3/.github/workflows/docs-publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         uses: actions/upload-artifact@v4
         with:
           name: _site.tar.gz
           path: docs/_site.tar.gz
           retention-days: 1
 
   deploy:
+    name: 🚀 Deploy
     needs: build
     environment:
       name: github-pages
       url: ${{ steps.deployment.outputs.page_url }}
     runs-on: ubuntu-latest
     permissions:
       id-token: write  # for trusted publishing
```

### Comparing `behaverse-0.0.5.dev2/.github/workflows/pypi-publish.yml` & `behaverse-0.0.5.dev3/.github/workflows/pypi-publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: 📦 Publish Python Package
 
 on:
   release:
     types: [published]
   # push:
   #   branches:
-  #     - python
+  #     - Python
 
 permissions:
   contents: read
 
 jobs:
   build:
     name: 📦 Build distribution
```

### Comparing `behaverse-0.0.5.dev2/LICENSE` & `behaverse-0.0.5.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.5.dev2/README.md` & `behaverse-0.0.5.dev3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -8,21 +8,26 @@
 
 ```bash
 pip install behaverse
 ```
 
 ## Usage
 
-See the [documentation](https://behaverse.github.io/) for more information on how to use the package.
+See the [Behaverse website](https://behaverse.github.io/) for more information on how to use the package.
 
+## License
+
+TODO
+
+## Contributing
 
 
-## Development
+### Development
 
-Before starting development, you need to install the dependencies:
+Before starting development, you need to install the dependencies. You can do this by creating a new conda environment as defined in the `environment.yml` file:
 
 ```bash
 mamba env create -f environment.yml
 mamba activate behaverse
 ```
 
 ### Documentation
@@ -32,21 +37,15 @@
 ```bash
 cd docs
 quartodoc build && quartodoc interlinks && quarto preview
 ```
 
 The documentation will be available in the `docs/_site/` directory.
 
-## License
 
-TODO
-
-## Contributing
-
-TODO
 
 ## Acknowledgements
 
 TODO
 
 ## Citation
```

### Comparing `behaverse-0.0.5.dev2/docs/_extensions/machow/interlinks/interlinks.lua` & `behaverse-0.0.5.dev3/docs/_extensions/machow/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.5.dev2/docs/_quarto.yml` & `behaverse-0.0.5.dev3/docs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.5.dev2/docs/getting_started.qmd` & `behaverse-0.0.5.dev3/docs/getting_started.qmd`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.5.dev2/examples/1 Getting Started with Behaverse Data.ipynb` & `behaverse-0.0.5.dev3/examples/1 Getting Started with Behaverse Data.ipynb`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.5.dev2/pyproject.toml` & `behaverse-0.0.5.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.5.dev2/src/behaverse/dataset.py` & `behaverse-0.0.5.dev3/src/behaverse/dataset.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.5.dev2/src/behaverse/dataset_test.py` & `behaverse-0.0.5.dev3/src/behaverse/dataset_test.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.5.dev2/src/behaverse/dvc_storage.py` & `behaverse-0.0.5.dev3/src/behaverse/dvc_storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     from dvc.api import DVCFileSystem
 
     assert name is not None, 'Dataset name is required.'
 
     # FIXME: query DVC registry for the url of the dataset
 
     repo = 'git@github.com:behaverse/behaverse.git'
-    fs = DVCFileSystem(repo, rev='Registry', remote='ulhpc')
+    fs = DVCFileSystem(repo, rev='Registry', remote='aion-cluster')
 
     dest = Path(kwargs.get('dest',
                            Path.home() / '.behaverse' / 'datasets' / f'{name.replace("/", "-")}.tar.gz'))
 
     if dest.exists():
         return extract_dataset(name)
```

### Comparing `behaverse-0.0.5.dev2/src/behaverse/dvc_storage_test.py` & `behaverse-0.0.5.dev3/src/behaverse/dvc_storage_test.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.5.dev2/src/behaverse/functional.py` & `behaverse-0.0.5.dev3/src/behaverse/functional.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.5.dev2/src/behaverse/http_storage.py` & `behaverse-0.0.5.dev3/src/behaverse/http_storage.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.5.dev2/src/behaverse/utils.py` & `behaverse-0.0.5.dev3/src/behaverse/utils.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.5.dev2/PKG-INFO` & `behaverse-0.0.5.dev3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: behaverse
-Version: 0.0.5.dev2
+Version: 0.0.5.dev3
 Summary: Behaverse Python Package.
 Author-email: xCIT Development Team <contact@xcit.org>
 Maintainer-email: Morteza Ansarinia <ansarinia@me.com>, Hoorieh Afkari <hoorieh.afkari@uni.lu>, Pedro Cardoso-Leite <pedro.cardosoleite@uni.lu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -37,21 +37,26 @@
 
 ```bash
 pip install behaverse
 ```
 
 ## Usage
 
-See the [documentation](https://behaverse.github.io/) for more information on how to use the package.
+See the [Behaverse website](https://behaverse.github.io/) for more information on how to use the package.
 
+## License
+
+TODO
+
+## Contributing
 
 
-## Development
+### Development
 
-Before starting development, you need to install the dependencies:
+Before starting development, you need to install the dependencies. You can do this by creating a new conda environment as defined in the `environment.yml` file:
 
 ```bash
 mamba env create -f environment.yml
 mamba activate behaverse
 ```
 
 ### Documentation
@@ -61,21 +66,15 @@
 ```bash
 cd docs
 quartodoc build && quartodoc interlinks && quarto preview
 ```
 
 The documentation will be available in the `docs/_site/` directory.
 
-## License
 
-TODO
-
-## Contributing
-
-TODO
 
 ## Acknowledgements
 
 TODO
 
 ## Citation
```

