# Comparing `tmp/calitp_map_utils-2023.8.2.tar.gz` & `tmp/calitp_map_utils-2024.5.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_map_utils-2023.8.2.tar", max compression
+gzip compressed data, was "calitp_map_utils-2024.5.23.tar", max compression
```

## Comparing `calitp_map_utils-2023.8.2.tar` & `calitp_map_utils-2024.5.23.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3674 2023-08-04 18:45:45.347002 calitp_map_utils-2023.8.2/README.md
--rw-r--r--   0        0        0     5454 2023-08-04 18:45:45.347002 calitp_map_utils-2023.8.2/calitp_map_utils/__init__.py
--rw-r--r--   0        0        0       44 2023-08-04 18:45:45.347002 calitp_map_utils-2023.8.2/calitp_map_utils/__main__.py
--rw-r--r--   0        0        0     1441 2023-08-04 18:45:45.347002 calitp_map_utils-2023.8.2/calitp_map_utils/cli.py
--rw-r--r--   0        0        0      637 2023-08-04 18:45:45.347002 calitp_map_utils-2023.8.2/pyproject.toml
--rw-r--r--   0        0        0     4296 1970-01-01 00:00:00.000000 calitp_map_utils-2023.8.2/PKG-INFO
+-rw-r--r--   0        0        0     3693 2024-05-24 18:19:54.730478 calitp_map_utils-2024.5.23/README.md
+-rw-r--r--   0        0        0     5454 2024-05-24 18:19:54.730478 calitp_map_utils-2024.5.23/calitp_map_utils/__init__.py
+-rw-r--r--   0        0        0       44 2024-05-24 18:19:54.730478 calitp_map_utils-2024.5.23/calitp_map_utils/__main__.py
+-rw-r--r--   0        0        0     1441 2024-05-24 18:19:54.730478 calitp_map_utils-2024.5.23/calitp_map_utils/cli.py
+-rw-r--r--   0        0        0      639 2024-05-24 18:19:54.734478 calitp_map_utils-2024.5.23/pyproject.toml
+-rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 calitp_map_utils-2024.5.23/PKG-INFO
```

### Comparing `calitp_map_utils-2023.8.2/README.md` & `calitp_map_utils-2024.5.23/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 ## calitp_map_utils
 
 As mentioned above, `calitp_map_utils` is a small utility library that defines Pydantic types that can be used for
 data validation as well as Typescript types for type-hinting in the Svelte app. Also, the library contains
 a few CLI commands to facilitate validating pre-existing data with those types and/or generate a quick URL
 with state for testing.
 
-TODO: a GitHub Action workflow exists to build the package, but it does not currently publish to pypi; right now
-that is done manually with `poetry publish`.
+A GitHub Action workflow exists to build the package and publish it to PyPi. Be sure to bump the version date in `pyproject.toml` in any pull request that updates the library.
 
 ## Developing the maps app
 
 You can run a development server locally; use the calitp-map-utils CLI to generate a valid state URL for testing.
 
 ```bash
 npm run dev
@@ -34,14 +33,15 @@
 Netlify sites deployed via `netlify deploy ...` with `--alias=some-alias` and/or without the `--prod` flag (see below).
 
 ## Build and deploy to Netlify
 
 The site is deployed to production on merges to main, as defined in [../../.github/workflows/deploy-apps-maps.yml](../../.github/workflows/deploy-apps-maps.yml).
 
 You may also deploy manually with the following:
+
 ```bash
 (from the apps/maps folder)
 npm run build
 netlify deploy --site=embeddable-maps-calitp-org --dir=build
 ```
 
 By default, this deploys a preview site with a generated alias prefix. You may pass an explicit alias with `--alias=<some-alias>`
```

### Comparing `calitp_map_utils-2023.8.2/calitp_map_utils/__init__.py` & `calitp_map_utils-2024.5.23/calitp_map_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `calitp_map_utils-2023.8.2/calitp_map_utils/cli.py` & `calitp_map_utils-2024.5.23/calitp_map_utils/cli.py`

 * *Files identical despite different names*

### Comparing `calitp_map_utils-2023.8.2/pyproject.toml` & `calitp_map_utils-2024.5.23/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "calitp_map_utils"
-version = "2023.8.2"
+version = "2024.5.23"
 description = ""
 authors = ["Andrew Vaccaro <andrew.v@jarv.us>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "~3.9"
+python = "~3.11"
 pyyaml = "^6.0"
 typer = "^0.9.0"
 pydantic = "^1.10.7"
 tqdm = "^4.64.0"
 geojson-pydantic = "^0.6.1"
 requests = "^2.24.0"
 furl = "^2.1.3"
```

### Comparing `calitp_map_utils-2023.8.2/PKG-INFO` & `calitp_map_utils-2024.5.23/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: calitp-map-utils
-Version: 2023.8.2
+Name: calitp_map_utils
+Version: 2024.5.23
 Summary: 
 Author: Andrew Vaccaro
 Author-email: andrew.v@jarv.us
-Requires-Python: >=3.9,<3.10
+Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: furl (>=2.1.3,<3.0.0)
 Requires-Dist: gcsfs (>=2023.6.0,<2024.0.0)
 Requires-Dist: geojson-pydantic (>=0.6.1,<0.7.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.24.0,<3.0.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
@@ -30,16 +30,15 @@
 ## calitp_map_utils
 
 As mentioned above, `calitp_map_utils` is a small utility library that defines Pydantic types that can be used for
 data validation as well as Typescript types for type-hinting in the Svelte app. Also, the library contains
 a few CLI commands to facilitate validating pre-existing data with those types and/or generate a quick URL
 with state for testing.
 
-TODO: a GitHub Action workflow exists to build the package, but it does not currently publish to pypi; right now
-that is done manually with `poetry publish`.
+A GitHub Action workflow exists to build the package and publish it to PyPi. Be sure to bump the version date in `pyproject.toml` in any pull request that updates the library.
 
 ## Developing the maps app
 
 You can run a development server locally; use the calitp-map-utils CLI to generate a valid state URL for testing.
 
 ```bash
 npm run dev
@@ -53,14 +52,15 @@
 Netlify sites deployed via `netlify deploy ...` with `--alias=some-alias` and/or without the `--prod` flag (see below).
 
 ## Build and deploy to Netlify
 
 The site is deployed to production on merges to main, as defined in [../../.github/workflows/deploy-apps-maps.yml](../../.github/workflows/deploy-apps-maps.yml).
 
 You may also deploy manually with the following:
+
 ```bash
 (from the apps/maps folder)
 npm run build
 netlify deploy --site=embeddable-maps-calitp-org --dir=build
 ```
 
 By default, this deploys a preview site with a generated alias prefix. You may pass an explicit alias with `--alias=<some-alias>`
```

