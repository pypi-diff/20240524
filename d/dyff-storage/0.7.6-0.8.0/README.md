# Comparing `tmp/dyff_storage-0.7.6.tar.gz` & `tmp/dyff_storage-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_storage-0.7.6.tar", last modified: Wed May 22 20:09:26 2024, max compression
+gzip compressed data, was "dyff_storage-0.8.0.tar", last modified: Thu May 23 22:41:49 2024, max compression
```

## Comparing `dyff_storage-0.7.6.tar` & `dyff_storage-0.8.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:09:26.933917 dyff_storage-0.7.6/
--rw-rw-rw-   0 root         (0) root         (0)      701 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1707 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      520 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2577 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3477 2024-05-22 20:09:26.932917 dyff_storage-0.7.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:09:26.919917 dyff_storage-0.7.6/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:09:26.925917 dyff_storage-0.7.6/dyff/storage/
--rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:09:26.926917 dyff_storage-0.7.6/dyff/storage/backend/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:09:26.927917 dyff_storage-0.7.6/dyff/storage/backend/base/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/base/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     6196 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/base/command.py
--rw-rw-rw-   0 root         (0) root         (0)    13398 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/base/query.py
--rw-rw-rw-   0 root         (0) root         (0)     3061 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/base/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:09:26.927917 dyff_storage-0.7.6/dyff/storage/backend/gcloud/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/gcloud/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6656 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/gcloud/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:09:26.928917 dyff_storage-0.7.6/dyff/storage/backend/kafka/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9209 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/kafka/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:09:26.929917 dyff_storage-0.7.6/dyff/storage/backend/mock/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/mock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/mock/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:09:26.929917 dyff_storage-0.7.6/dyff/storage/backend/mongodb/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/mongodb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7184 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/mongodb/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    23188 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/mongodb/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:09:26.930917 dyff_storage-0.7.6/dyff/storage/backend/s3/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15744 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/backend/s3/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    10386 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/config.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/dynamic_import.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2946 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/paths.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/dyff/storage/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:09:26.932917 dyff_storage-0.7.6/dyff_storage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3477 2024-05-22 20:09:26.000000 dyff_storage-0.7.6/dyff_storage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1176 2024-05-22 20:09:26.000000 dyff_storage-0.7.6/dyff_storage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 20:09:26.000000 dyff_storage-0.7.6/dyff_storage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-05-22 20:09:26.000000 dyff_storage-0.7.6/dyff_storage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-22 20:09:26.000000 dyff_storage-0.7.6/dyff_storage.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 20:09:26.933917 dyff_storage-0.7.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:09:26.932917 dyff_storage-0.7.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-05-22 20:09:20.000000 dyff_storage-0.7.6/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.775149 dyff_storage-0.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)      701 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      520 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-05-23 22:41:49.775149 dyff_storage-0.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.762149 dyff_storage-0.8.0/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.768149 dyff_storage-0.8.0/dyff/storage/
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.769149 dyff_storage-0.8.0/dyff/storage/backend/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.770149 dyff_storage-0.8.0/dyff/storage/backend/base/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2584 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/base/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     6196 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/base/command.py
+-rw-rw-rw-   0 root         (0) root         (0)    13398 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/base/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/base/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.770149 dyff_storage-0.8.0/dyff/storage/backend/gcloud/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/gcloud/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6656 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/gcloud/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.771149 dyff_storage-0.8.0/dyff/storage/backend/kafka/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9209 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/kafka/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.771149 dyff_storage-0.8.0/dyff/storage/backend/mock/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/mock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/mock/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.772149 dyff_storage-0.8.0/dyff/storage/backend/mongodb/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/mongodb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7252 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/mongodb/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    23188 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/mongodb/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.772149 dyff_storage-0.8.0/dyff/storage/backend/s3/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15691 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/s3/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    10386 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/dynamic_import.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2946 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/paths.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.774149 dyff_storage-0.8.0/dyff_storage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-05-23 22:41:49.000000 dyff_storage-0.8.0/dyff_storage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-05-23 22:41:49.000000 dyff_storage-0.8.0/dyff_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 22:41:49.000000 dyff_storage-0.8.0/dyff_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-05-23 22:41:49.000000 dyff_storage-0.8.0/dyff_storage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-23 22:41:49.000000 dyff_storage-0.8.0/dyff_storage.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 22:41:49.775149 dyff_storage-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.774149 dyff_storage-0.8.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/tests/test_import.py
```

### Comparing `dyff_storage-0.7.6/.gitignore` & `dyff_storage-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/.gitlab-ci.yml` & `dyff_storage-0.8.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/.licenserc.yaml` & `dyff_storage-0.8.0/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/.pre-commit-config.yaml` & `dyff_storage-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/.secrets.baseline` & `dyff_storage-0.8.0/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/CODE_OF_CONDUCT.md` & `dyff_storage-0.8.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/LICENSE` & `dyff_storage-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/PKG-INFO` & `dyff_storage-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.7.6
+Version: 0.8.0
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff_storage-0.7.6/README.md` & `dyff_storage-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/dyff/storage/__init__.py` & `dyff_storage-0.8.0/dyff/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/dyff/storage/backend/base/command.py` & `dyff_storage-0.8.0/dyff/storage/backend/base/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/dyff/storage/backend/base/query.py` & `dyff_storage-0.8.0/dyff/storage/backend/base/query.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/dyff/storage/backend/base/storage.py` & `dyff_storage-0.8.0/dyff/storage/backend/base/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/dyff/storage/backend/gcloud/storage.py` & `dyff_storage-0.8.0/dyff/storage/backend/gcloud/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/dyff/storage/backend/kafka/command.py` & `dyff_storage-0.8.0/dyff/storage/backend/kafka/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/dyff/storage/backend/mock/command.py` & `dyff_storage-0.8.0/dyff/storage/backend/mock/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/dyff/storage/backend/mongodb/auth.py` & `dyff_storage-0.8.0/dyff/storage/backend/mongodb/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import pymongo
 import pymongo.read_concern
 import pymongo.read_preferences
 import pymongo.write_concern
 from pymongo.client_session import ClientSession
 
 from dyff.schema import ids
-from dyff.schema.platform import APIKey
+from dyff.schema.platform import Account, APIKey, Identity
 from dyff.storage import timestamp
-from dyff.storage.backend.base.auth import Account, AuthBackend, Identity
+from dyff.storage.backend.base.auth import AuthBackend
 from dyff.storage.config import config
 from dyff.storage.exceptions import EntityExistsError
 
 
 class MongoDBAuthBackend(AuthBackend):
     def __init__(self):
         connection_string = config.api.auth.mongodb.connection_string
@@ -43,15 +43,15 @@
     ) -> Optional[Account]:
         filter = {}
         if id is not None:
             filter["_id"] = id
         if name is not None:
             filter["name"] = name
         if identity is not None:
-            identity_dict = identity.dict()
+            identity_dict = identity.model_dump(mode="json")
             for identity_key, identity_value in identity_dict.items():
                 if identity_value is not None:
                     filter[f"identity.{identity_key}"] = identity_value
         if len(filter) == 0:
             raise ValueError("must specify at least one of {id, name, identity}")
         result = self._accounts_db.accounts.find_one(filter, session=session)
         if result:
@@ -60,15 +60,15 @@
             del result["_id"]
             return Account.parse_obj(result)
         return None
 
     def _insert_account(
         self, account: Account, *, session: Optional[ClientSession] = None
     ) -> None:
-        d = account.dict()
+        d = account.model_dump(mode="json")
         d["_id"] = d["id"]
         del d["id"]
         self._accounts_db.accounts.insert_one(d, session=session)
 
     def create_account(self, name: str, identity: Optional[Identity] = None) -> Account:
         """Create a new Account.
 
@@ -128,15 +128,15 @@
         if account is None:
             raise ValueError(f"no Account with .id {account_id}")
         if any(account_key.id == api_key.id for account_key in account.apiKeys):
             raise ValueError(f"APIKey with .id {api_key.id} already exists")
         # Don't have to translate APIKey.id because APIKey isn't a
         # top-level entity
         self._accounts_db.accounts.update_one(
-            {"_id": account_id}, {"$push": {"apiKeys": api_key.dict()}}
+            {"_id": account_id}, {"$push": {"apiKeys": api_key.model_dump(mode="json")}}
         )
 
     def revoke_api_key(self, account_id: str, api_key_id: str) -> None:
         """Revoke an APIKey associated with an Account.
 
         Parameters:
         account_id: The unique identifier of the Account.
@@ -148,15 +148,15 @@
         filtered = [api_key for api_key in account.apiKeys if api_key.id != api_key_id]
         if len(filtered) == len(account.apiKeys):
             raise ValueError(f"no APIKey with .id {api_key_id} in account")
         # Don't have to translate APIKey.id because APIKey isn't a
         # top-level entity
         self._accounts_db.accounts.update_one(
             {"_id": account_id},
-            {"$set": {"apiKeys": [key.dict() for key in filtered]}},
+            {"$set": {"apiKeys": [key.model_dump(mode="json") for key in filtered]}},
         )
 
     def revoke_all_api_keys(self, account_id: str) -> None:
         """Revoke all API keys for the given Account.
 
         Parameters:
         account_id: The unique identifier of the Account.
```

### Comparing `dyff_storage-0.7.6/dyff/storage/backend/mongodb/query.py` & `dyff_storage-0.8.0/dyff/storage/backend/mongodb/query.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/dyff/storage/backend/s3/storage.py` & `dyff_storage-0.8.0/dyff/storage/backend/s3/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,19 +168,18 @@
 
 
 def _translate_errors(fn):
     @functools.wraps(fn)
     def _impl(*args, **kwargs):
         try:
             return fn(*args, **kwargs)
-        except Exception as ex:
-            if isinstance(ex, minio.S3Error):
-                if ex.code in ["NoSuchKey", "NoSuchBucket", "ResourceNotFound"]:
-                    raise KeyError(f"{ex._resource} ({ex.code})")
-            raise ex
+        except minio.S3Error as ex:
+            if ex.code in ["NoSuchKey", "NoSuchBucket", "ResourceNotFound"]:
+                raise KeyError(f"{ex._resource} ({ex.code})")
+            raise
 
     return _impl
 
 
 class S3StorageBackend(StorageBackend):
     @_translate_errors
     def storage_size(self, path: str) -> int:
```

### Comparing `dyff_storage-0.7.6/dyff/storage/config.py` & `dyff_storage-0.8.0/dyff/storage/config.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/dyff/storage/paths.py` & `dyff_storage-0.8.0/dyff/storage/paths.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/dyff/storage/timestamp.py` & `dyff_storage-0.8.0/dyff/storage/timestamp.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/dyff_storage.egg-info/PKG-INFO` & `dyff_storage-0.8.0/dyff_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.7.6
+Version: 0.8.0
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff_storage-0.7.6/dyff_storage.egg-info/SOURCES.txt` & `dyff_storage-0.8.0/dyff_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/makefile` & `dyff_storage-0.8.0/makefile`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/pyproject.toml` & `dyff_storage-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.6/tests/test_import.py` & `dyff_storage-0.8.0/tests/test_import.py`

 * *Files identical despite different names*

