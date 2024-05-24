# Comparing `tmp/dkist_quality-1.0.2.tar.gz` & `tmp/dkist_quality-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_quality-1.0.2.tar", last modified: Thu May 23 16:11:43 2024, max compression
+gzip compressed data, was "dkist_quality-1.0.3.tar", last modified: Fri May 24 18:16:09 2024, max compression
```

## Comparing `dkist_quality-1.0.2.tar` & `dkist_quality-1.0.3.tar`

### file list

```diff
@@ -1,33 +1,30 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 16:11:43.829722 dkist_quality-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     3104 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      468 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2150 2024-05-23 16:11:43.829722 dkist_quality-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1229 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2513 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 16:11:43.825722 dkist_quality-1.0.2/dkist_quality/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/dkist_quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-05-23 16:11:43.000000 dkist_quality-1.0.2/dkist_quality/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 16:11:43.829722 dkist_quality-1.0.2/dkist_quality/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    91676 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/dkist_quality/fonts/Oswald-Bold.ttf
--rw-rw-rw-   0 root         (0) root         (0)    91400 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/dkist_quality/fonts/Oswald-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      871 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/dkist_quality/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)    37316 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/dkist_quality/report.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 16:11:43.829722 dkist_quality-1.0.2/dkist_quality/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/dkist_quality/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11866 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/dkist_quality/tests/test_report.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/dkist_quality/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 16:11:43.829722 dkist_quality-1.0.2/dkist_quality.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2150 2024-05-23 16:11:43.000000 dkist_quality-1.0.2/dkist_quality.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      668 2024-05-23 16:11:43.000000 dkist_quality-1.0.2/dkist_quality.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-23 16:11:43.000000 dkist_quality-1.0.2/dkist_quality.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-23 16:11:43.000000 dkist_quality-1.0.2/dkist_quality.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      147 2024-05-23 16:11:43.000000 dkist_quality-1.0.2/dkist_quality.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 16:11:43.000000 dkist_quality-1.0.2/dkist_quality.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 16:11:43.829722 dkist_quality-1.0.2/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/licenses/TEMPLATE_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)     2032 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-23 16:11:43.829722 dkist_quality-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1214 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-24 18:16:09.416220 dkist_quality-1.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     3104 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      468 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2160 2024-05-24 18:16:09.416220 dkist_quality-1.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2791 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-24 18:16:09.412220 dkist_quality-1.0.3/dkist_quality/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/dkist_quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-05-24 18:16:09.000000 dkist_quality-1.0.3/dkist_quality/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-24 18:16:09.416220 dkist_quality-1.0.3/dkist_quality/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    91676 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/dkist_quality/fonts/Oswald-Bold.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    91400 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/dkist_quality/fonts/Oswald-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      871 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/dkist_quality/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)    37316 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/dkist_quality/report.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-24 18:16:09.416220 dkist_quality-1.0.3/dkist_quality/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/dkist_quality/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11866 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/dkist_quality/tests/test_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/dkist_quality/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-24 18:16:09.416220 dkist_quality-1.0.3/dkist_quality.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2160 2024-05-24 18:16:09.000000 dkist_quality-1.0.3/dkist_quality.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      605 2024-05-24 18:16:09.000000 dkist_quality-1.0.3/dkist_quality.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-24 18:16:09.000000 dkist_quality-1.0.3/dkist_quality.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-24 18:16:08.000000 dkist_quality-1.0.3/dkist_quality.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-05-24 18:16:09.000000 dkist_quality-1.0.3/dkist_quality.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-24 18:16:09.000000 dkist_quality-1.0.3/dkist_quality.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-24 18:16:09.416220 dkist_quality-1.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1214 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/tox.ini
```

### Comparing `dkist_quality-1.0.2/.gitignore` & `dkist_quality-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.2/.pre-commit-config.yaml` & `dkist_quality-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.2/PKG-INFO` & `dkist_quality-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: dkist-quality
-Version: 1.0.2
+Version: 1.0.3
 Summary: DKIST library for generating quality report pdf
 Author-email: NSO / AURA <dkistdc@nso.edu>
-License: BSD 3-Clause
+License: MIT
 Project-URL: repository, https://bitbucket.org/dkistdc/dkist-quality
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 Requires-Dist: reportlab>=4.0.4
 Requires-Dist: matplotlib>=3.6
 Requires-Dist: seaborn>=0.13.0
 Requires-Dist: dacite>=1.8.0
 Requires-Dist: natsort>=8.0.0
-Requires-Dist: pydantic<2,>=1.10.4
+Requires-Dist: pydantic>=1.10.4
 Provides-Extra: test
 Requires-Dist: tox>=4; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: Pygments; extra == "test"
 Requires-Dist: PyPDF4; extra == "test"
```

### Comparing `dkist_quality-1.0.2/README.rst` & `dkist_quality-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.2/bitbucket-pipelines.yml` & `dkist_quality-1.0.3/bitbucket-pipelines.yml`

 * *Files 15% similar despite different names*

```diff
@@ -16,18 +16,24 @@
         caches:
           - pip
         name: Scan
         script:
           - pip install -U pip setuptools wheel
           - pip install .
           - pip freeze | grep -v @ > requirements.txt
-          - curl -L -o snyk https://github.com/snyk/snyk/releases/download/$SNYK_VERSION/snyk-linux
           - cat requirements.txt
+          - echo $SNYK_VERSION
+          - curl -L -o snyk https://github.com/snyk/snyk/releases/download/$SNYK_VERSION/snyk-linux
           - chmod 755 snyk
-          - ./snyk -d test --all-projects --fail-on=upgradable
+          - ./snyk -d auth $SNYK_TOKEN
+          - echo $SNYK_IGNORE
+          - for id in $SNYK_IGNORE; do echo Ignoring $id; ./snyk ignore $id; done
+          - cat .snyk || echo "No .snyk found. Probably because there was nothing to ignore."
+          - echo $SNYK_CLI_COMMAND
+          - $SNYK_CLI_COMMAND
 
     - step: &test311
         caches:
           - pip
         name: Test Python 3.11
         script:
           - pip install -U pip
```

### Comparing `dkist_quality-1.0.2/dkist_quality/fonts/Oswald-Bold.ttf` & `dkist_quality-1.0.3/dkist_quality/fonts/Oswald-Bold.ttf`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.2/dkist_quality/fonts/Oswald-Regular.ttf` & `dkist_quality-1.0.3/dkist_quality/fonts/Oswald-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.2/dkist_quality/json_encoder.py` & `dkist_quality-1.0.3/dkist_quality/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.2/dkist_quality/report.py` & `dkist_quality-1.0.3/dkist_quality/report.py`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.2/dkist_quality/tests/test_report.py` & `dkist_quality-1.0.3/dkist_quality/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.2/dkist_quality.egg-info/PKG-INFO` & `dkist_quality-1.0.3/dkist_quality.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: dkist-quality
-Version: 1.0.2
+Version: 1.0.3
 Summary: DKIST library for generating quality report pdf
 Author-email: NSO / AURA <dkistdc@nso.edu>
-License: BSD 3-Clause
+License: MIT
 Project-URL: repository, https://bitbucket.org/dkistdc/dkist-quality
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 Requires-Dist: reportlab>=4.0.4
 Requires-Dist: matplotlib>=3.6
 Requires-Dist: seaborn>=0.13.0
 Requires-Dist: dacite>=1.8.0
 Requires-Dist: natsort>=8.0.0
-Requires-Dist: pydantic<2,>=1.10.4
+Requires-Dist: pydantic>=1.10.4
 Provides-Extra: test
 Requires-Dist: tox>=4; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: Pygments; extra == "test"
 Requires-Dist: PyPDF4; extra == "test"
```

### Comparing `dkist_quality-1.0.2/dkist_quality.egg-info/SOURCES.txt` & `dkist_quality-1.0.3/dkist_quality.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 .pre-commit-config.yaml
+LICENSE
 MANIFEST.in
 README.rst
 bitbucket-pipelines.yml
 pyproject.toml
 tox.ini
 dkist_quality/__init__.py
 dkist_quality/_version.py
@@ -15,11 +16,8 @@
 dkist_quality.egg-info/dependency_links.txt
 dkist_quality.egg-info/not-zip-safe
 dkist_quality.egg-info/requires.txt
 dkist_quality.egg-info/top_level.txt
 dkist_quality/fonts/Oswald-Bold.ttf
 dkist_quality/fonts/Oswald-Regular.ttf
 dkist_quality/tests/__init__.py
-dkist_quality/tests/test_report.py
-licenses/LICENSE.rst
-licenses/README.rst
-licenses/TEMPLATE_LICENSE.rst
+dkist_quality/tests/test_report.py
```

### Comparing `dkist_quality-1.0.2/pyproject.toml` & `dkist_quality-1.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 
 [project]
 name = "dkist-quality"
 description = "DKIST library for generating quality report pdf"
 readme = "README.rst"
 requires-python = ">=3.10"
 classifiers = [
-    "License :: OSI Approved :: BSD License",
+    "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-license = { text = "BSD 3-Clause" }
+license = { text = "MIT" }
 authors = [
   { name = "NSO / AURA", email = "dkistdc@nso.edu" },
 ]
 # the current version of Airflow does not support pydantic v2
 dependencies = [
     "reportlab>=4.0.4",
     "matplotlib>=3.6",
     "seaborn>=0.13.0",
     "dacite>=1.8.0",
     "natsort>=8.0.0",
-    "pydantic>=1.10.4,<2",
+    "pydantic>=1.10.4",
 ]
 dynamic = ["version"]
 
 # tox is not required to run the tests, but simplifies IDE integration
 # Pygments is solely to support README.rst rendering
 [project.optional-dependencies]
 test = [
@@ -73,14 +73,15 @@
  "dkist_quality/__init*",
  "dkist_quality/conftest.py",
  "dkist_quality/*setup_package*",
  "dkist_quality/tests/*",
  "dkist_quality/*/tests/*",
  "dkist_quality/extern/*",
  "dkist_quality/version*",
+ "dkist_quality/_version*",
  "*/dkist_quality/__init*",
  "*/dkist_quality/conftest.py",
  "*/dkist_quality/*setup_package*",
  "*/dkist_quality/tests/*",
  "*/dkist_quality/*/tests/*",
  "*/dkist_quality/extern/*",
  "*/dkist_quality/version*",
```

### Comparing `dkist_quality-1.0.2/tox.ini` & `dkist_quality-1.0.3/tox.ini`

 * *Files identical despite different names*

