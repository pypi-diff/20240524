# Comparing `tmp/dao-scripts-1.2.2.tar.gz` & `tmp/dao_scripts-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dao-scripts-1.2.2.tar", last modified: Wed Dec 13 18:09:27 2023, max compression
+gzip compressed data, was "dao_scripts-1.3.0.tar", last modified: Fri May 24 16:15:18 2024, max compression
```

## Comparing `dao-scripts-1.2.2.tar` & `dao_scripts-1.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:09:27.177775 dao-scripts-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:09:27.169775 dao-scripts-1.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:09:27.173775 dao-scripts-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/.github/workflows/update-datasets.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     6616 2023-12-13 18:09:27.177775 dao-scripts-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:09:27.177775 dao-scripts-1.2.2/dao_scripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6616 2023-12-13 18:09:27.000000 dao-scripts-1.2.2/dao_scripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      957 2023-12-13 18:09:27.000000 dao-scripts-1.2.2/dao_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 18:09:27.000000 dao-scripts-1.2.2/dao_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-13 18:09:27.000000 dao-scripts-1.2.2/dao_scripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-13 18:09:27.000000 dao-scripts-1.2.2/dao_scripts.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-12-13 18:09:27.000000 dao-scripts-1.2.2/dao_scripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-13 18:09:27.000000 dao-scripts-1.2.2/dao_scripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2023-12-13 18:09:27.177775 dao-scripts-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:09:27.173775 dao-scripts-1.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-13 18:09:27.000000 dao-scripts-1.2.2/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:09:27.173775 dao-scripts-1.2.2/src/aragon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/aragon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/aragon/dao_names.json
--rw-r--r--   0 runner    (1001) docker     (127)     8421 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/aragon/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:09:27.177775 dao-scripts-1.2.2/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7996 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/common/api_requester.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/common/blockscout.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/common/cryptocompare.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/common/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:09:27.177775 dao-scripts-1.2.2/src/daohaus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/daohaus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/daohaus/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:09:27.177775 dao-scripts-1.2.2/src/daostack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/daostack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/daostack/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/endpoints.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     5256 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:09:27.177775 dao-scripts-1.2.2/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/src/utils/uploadDataWarehouse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:09:27.177775 dao-scripts-1.2.2/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:09:27.177775 dao-scripts-1.2.2/test/daohaus/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/test/daohaus/test_verify_daohaus_collectors.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-13 18:09:17.000000 dao-scripts-1.2.2/test/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:15:18.722087 dao_scripts-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:15:18.710087 dao_scripts-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:15:18.714087 dao_scripts-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/.github/workflows/update-datasets.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-24 16:15:18.722087 dao_scripts-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:15:18.718087 dao_scripts-1.3.0/dao_scripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-24 16:15:18.000000 dao_scripts-1.3.0/dao_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-24 16:15:18.000000 dao_scripts-1.3.0/dao_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:15:18.000000 dao_scripts-1.3.0/dao_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-24 16:15:18.000000 dao_scripts-1.3.0/dao_scripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 16:15:18.000000 dao_scripts-1.3.0/dao_scripts.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-24 16:15:18.000000 dao_scripts-1.3.0/dao_scripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 16:15:18.000000 dao_scripts-1.3.0/dao_scripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-24 16:15:18.722087 dao_scripts-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:15:18.718087 dao_scripts-1.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 16:15:18.000000 dao_scripts-1.3.0/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:15:18.718087 dao_scripts-1.3.0/src/aragon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/aragon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/aragon/dao_names.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/aragon/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:15:18.718087 dao_scripts-1.3.0/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/common/api_requester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/common/blockscout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/common/cryptocompare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/common/thegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:15:18.718087 dao_scripts-1.3.0/src/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/daohaus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/daohaus/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:15:18.718087 dao_scripts-1.3.0/src/daostack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/daostack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/daostack/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/endpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5665 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:15:18.718087 dao_scripts-1.3.0/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/src/utils/uploadDataWarehouse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:15:18.718087 dao_scripts-1.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-24 16:15:14.000000 dao_scripts-1.3.0/test/test_placeholder.py
```

### Comparing `dao-scripts-1.2.2/.github/workflows/ci.yml` & `dao_scripts-1.3.0/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 on: [push]
 
 jobs:
   testing_python:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8","3.9","3.10", "3.11"]
+        python-version: ["3.9","3.10", "3.11", "3.12"]
     env:
       DEBUG: TRUE
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
```

### Comparing `dao-scripts-1.2.2/.github/workflows/update-datasets.yml` & `dao_scripts-1.3.0/.github/workflows/update-datasets.yml`

 * *Files 23% similar despite different names*

```diff
@@ -25,14 +25,18 @@
       uses: actions/upload-artifact@v3
       with:
         name: datawarehouse
         path: ./datawarehouse/
   upload_dw:
     runs-on: ubuntu-latest
     environment: daviddavo
+    strategy:
+      fail-fast: false
+      matrix:
+        repo: ["zenodo","kaggle"]
     needs: [update_dw]
     steps:
     - name: Download artifact
       uses: actions/download-artifact@v3
       with:
         name: datawarehouse
         path: ./datawarehouse/
@@ -41,15 +45,16 @@
         python-version: '3.11'
     - name: Install dao-scripts
       run: pip install 'dao-scripts[upload]>=1.1.14'
     - name: Patch Zenodo client (provisional)
       run: |
         FILE="$(python -c "from zenodo_client import api; print(api.__file__)")"
         echo "Modyfing file $FILE"
-        sed -i 's/_prepare_new_version(new_deposition_data\["metadata"\]\["version"\])/_prepare_new_version(new_deposition_data["metadata"].get("version", ""))/g' $FILE
+        sed -i 's/_prepare_new_version(new_deposition_data\["metadata"\]\["version"\])/_prepare_new_version(new_deposition_data["metadata"].get("version", ""))/g' "$FILE"
+        sed -i 's/json=new_deposition_data/json={"metadata": new_deposition_data\["metadata"\]}/g' "$FILE"
     - name: Upload dataset
-      run: dao-utils-upload-dw
+      run: dao-utils-upload-dw ${{matrix.repo}}
       env:
         KAGGLE_USERNAME: ${{ secrets.KAGGLE_USERNAME }}
         KAGGLE_KEY: ${{ secrets.KAGGLE_KEY }}
         ZENODO_DEPOSITION_ID: ${{ secrets.ZENODO_DEPOSITION_ID }}
         ZENODO_API_TOKEN: ${{ secrets.ZENODO_API_TOKEN }}
```

### Comparing `dao-scripts-1.2.2/.gitignore` & `dao_scripts-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.2.2/CHANGELOG.md` & `dao_scripts-1.3.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
+## 1.3.0 - 2024-04-24
+- Improved and standarized logging #10
+- The Graph Hosted Service sunsetting
+  - Added DAOA_THE_GRAPH_API_KEY variable (now needed)
+
 ## 1.2.2 - 2023-12-13
 - Changed daohaus names cache folder
 
 ## 1.2.1 - 2023-12-12
 - Fixed error that made impossible getting DAOhaus proposals
 
 ## 1.2.0 - 2023-12-12
```

### Comparing `dao-scripts-1.2.2/README.md` & `dao_scripts-1.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,300 +1,399 @@
-00000000: 2320 4441 4f2d 416e 616c 797a 6572 2773  # DAO-Analyzer's
-00000010: 2063 6163 6865 2d73 6372 6970 7473 0a0a   cache-scripts..
-00000020: 2323 2053 6574 2d75 7020 2620 5275 6e6e  ## Set-up & Runn
-00000030: 696e 670a 0a54 6865 2065 6173 6965 7374  ing..The easiest
-00000040: 206d 6574 686f 6420 6279 2066 6172 2074   method by far t
-00000050: 6f20 646f 776e 6c6f 6164 2061 6e64 2072  o download and r
-00000060: 756e 2074 6865 2061 7070 6c69 6361 7469  un the applicati
-00000070: 6f6e 2069 7320 746f 2075 7365 2070 6970  on is to use pip
-00000080: 2074 6f20 696e 7374 616c 6c20 6974 0a0a   to install it..
-00000090: 6060 600a 7069 7020 696e 7374 616c 6c20  ```.pip install 
-000000a0: 6461 6f2d 7363 7269 7074 730a 6060 600a  dao-scripts.```.
-000000b0: 0a54 6865 6e2c 2079 6f75 2063 616e 2075  .Then, you can u
-000000c0: 7365 2074 6869 7320 7363 7269 7074 2075  se this script u
-000000d0: 7369 6e67 2074 6865 2063 6f6d 6d61 6e64  sing the command
-000000e0: 2060 6461 6f61 2d63 6163 6865 2d73 6372   `daoa-cache-scr
-000000f0: 6970 7473 6020 6f72 2060 6461 6f2d 7363  ipts` or `dao-sc
-00000100: 7269 7074 7360 0a0a 2323 2320 446f 776e  ripts`..### Down
-00000110: 6c6f 6164 0a45 6e74 6572 2069 6e20 796f  load.Enter in yo
-00000120: 7572 2074 6572 6d69 6e61 6c20 2867 6974  ur terminal (git
-00000130: 206d 7573 7420 6265 2069 6e73 7461 6c6c   must be install
-00000140: 6564 2920 616e 6420 7772 6974 6520 646f  ed) and write do
-00000150: 776e 3a0a 0a60 6060 0a67 6974 2063 6c6f  wn:..```.git clo
-00000160: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
-00000170: 622e 636f 6d2f 4772 6173 6961 2f64 616f  b.com/Grasia/dao
-00000180: 2d73 6372 6970 7473 0a60 6060 0a0a 4166  -scripts.```..Af
-00000190: 7465 7220 7468 6174 2c20 6d6f 7665 2074  ter that, move t
-000001a0: 6f20 7468 6520 7265 706f 7369 746f 7279  o the repository
-000001b0: 2072 6f6f 7420 6469 7265 6374 6f72 7920   root directory 
-000001c0: 7769 7468 3a0a 0a60 6060 0a63 6420 6461  with:..```.cd da
-000001d0: 6f2d 7363 7269 7074 730a 6060 600a 0a23  o-scripts.```..#
-000001e0: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
-000001f0: 416c 6c20 636f 6465 2068 6173 2062 6565  All code has bee
-00000200: 6e20 7465 7374 6564 206f 6e20 4c69 6e75  n tested on Linu
-00000210: 782c 2062 7574 2069 7420 7368 6f75 6c64  x, but it should
-00000220: 2077 6f72 6b20 6f6e 2057 696e 646f 7773   work on Windows
-00000230: 2061 6e64 206d 6163 4f53 2c20 2763 6175   and macOS, 'cau
-00000240: 7365 2069 7420 6a75 7374 2075 7365 7320  se it just uses 
-00000250: 7468 6520 5079 7468 6f6e 2065 6e76 6972  the Python envir
-00000260: 6f6e 6d65 6e74 2e0a 0a53 6f2c 2079 6f75  onment...So, you
-00000270: 206d 7573 7420 696e 7374 616c 6c20 7468   must install th
-00000280: 6520 666f 6c6c 6f77 696e 6720 6465 7065  e following depe
-00000290: 6e64 656e 6369 6573 2074 6f20 7275 6e20  ndencies to run 
-000002a0: 7468 6520 746f 6f6c 3a0a 0a2a 2070 7974  the tool:..* pyt
-000002b0: 686f 6e33 2028 332e 3130 206f 7220 6c61  hon3 (3.10 or la
-000002c0: 7465 7229 0a2a 2070 7974 686f 6e33 2d70  ter).* python3-p
-000002d0: 6970 0a0a 4e6f 772c 2069 6e73 7461 6c6c  ip..Now, install
-000002e0: 2074 6865 2050 7974 686f 6e20 6465 7065   the Python depe
-000002f0: 6e64 656e 6369 6573 3a0a 0a60 7069 7033  ndencies:..`pip3
-00000300: 2069 6e73 7461 6c6c 202d 7220 7265 7175   install -r requ
-00000310: 6972 656d 656e 7473 2e74 7874 600a 0a49  irements.txt`..I
-00000320: 6620 796f 7520 646f 6e27 7420 7761 6e74  f you don't want
-00000330: 2074 6f20 7368 6172 6520 5079 7468 6f6e   to share Python
-00000340: 2064 6570 656e 6465 6e63 6965 7320 616d   dependencies am
-00000350: 6f6e 6720 6f74 6865 7220 7072 6f6a 6563  ong other projec
-00000360: 7473 2c20 796f 7520 7368 6f75 6c64 2075  ts, you should u
-00000370: 7365 2061 2076 6972 7475 616c 2065 6e76  se a virtual env
-00000380: 6972 6f6e 6d65 6e74 2c20 7375 6368 2061  ironment, such a
-00000390: 7320 5b76 6972 7475 616c 656e 765d 2868  s [virtualenv](h
-000003a0: 7474 7073 3a2f 2f64 6f63 732e 7079 7468  ttps://docs.pyth
-000003b0: 6f6e 2d67 7569 6465 2e6f 7267 2f64 6576  on-guide.org/dev
-000003c0: 2f76 6972 7475 616c 656e 7673 2f29 2e0a  /virtualenvs/)..
-000003d0: 0a23 2323 2048 6f77 2074 6f20 7275 6e20  .### How to run 
-000003e0: 6974 3f0a 4966 2079 6f75 2077 616e 7420  it?.If you want 
-000003f0: 616c 6c20 7468 6520 6461 7461 2075 7365  all the data use
-00000400: 6420 696e 2074 6865 2061 7070 2c20 796f  d in the app, yo
-00000410: 7520 6361 6e20 6a75 7374 2075 7365 3a0a  u can just use:.
-00000420: 0a60 6060 0a64 616f 2d73 6372 6970 7473  .```.dao-scripts
-00000430: 0a60 6060 0a0a 7468 6973 2077 696c 6c20  .```..this will 
-00000440: 6372 6561 7465 2061 2066 6f6c 6465 7220  create a folder 
-00000450: 6361 6c6c 6564 2060 6461 7461 7761 7265  called `dataware
-00000460: 686f 7573 6560 2077 6974 6820 6120 6c6f  house` with a lo
-00000470: 7420 6f66 2066 696c 6573 2069 6e20 4170  t of files in Ap
-00000480: 6163 6865 2773 2061 7272 6f77 2066 6f72  ache's arrow for
-00000490: 6d61 742e 0a0a 596f 7520 6361 6e20 696d  mat...You can im
-000004a0: 706f 7274 2074 686f 7365 2066 696c 6573  port those files
-000004b0: 2074 6f20 6070 616e 6461 7360 2077 6974   to `pandas` wit
-000004c0: 6820 6072 6561 645f 6665 6174 6865 7260  h `read_feather`
-000004d0: 2e20 466f 7220 6578 616d 706c 653a 0a0a  . For example:..
-000004e0: 6060 6070 7974 686f 6e0a 7064 2e72 6561  ```python.pd.rea
-000004f0: 645f 6665 6174 6865 7228 2764 6174 6177  d_feather('dataw
-00000500: 6172 6568 6f75 7365 2f61 7261 676f 6e2f  arehouse/aragon/
-00000510: 6170 7073 2e61 7272 2729 0a60 6060 0a0a  apps.arr').```..
-00000520: 2323 2055 7361 6765 2067 7569 6465 0a49  ## Usage guide.I
-00000530: 6620 796f 7520 646f 6e27 7420 7761 6e74  f you don't want
-00000540: 2061 6c6c 2074 6865 2064 6174 6120 2861   all the data (a
-00000550: 6e64 2069 7420 6361 6e20 7461 6b65 2061  nd it can take a
-00000560: 206c 6f74 206f 6620 7469 6d65 292c 2079   lot of time), y
-00000570: 6f75 2068 6176 6520 6120 6c6f 7420 6f66  ou have a lot of
-00000580: 206f 7074 696f 6e73 2061 7661 696c 6162   options availab
-00000590: 6c65 2074 6f20 7365 6c65 6374 2077 6869  le to select whi
-000005a0: 6368 6576 6572 2064 6174 6120 796f 7520  chever data you 
-000005b0: 7761 6e74 2e20 5468 6520 6675 6c6c 2060  want. The full `
-000005c0: 2d2d 6865 6c70 6020 6f75 7470 7574 2069  --help` output i
-000005d0: 730a 0a60 6060 0a75 7361 6765 3a20 6461  s..```.usage: da
-000005e0: 6f61 2d63 6163 6865 2d73 6372 6970 7473  oa-cache-scripts
-000005f0: 205b 2d68 5d20 5b2d 565d 205b 2d70 205b   [-h] [-V] [-p [
-00000600: 7b61 7261 676f 6e2c 6461 6f68 6175 732c  {aragon,daohaus,
-00000610: 6461 6f73 7461 636b 7d20 2e2e 2e5d 5d0a  daostack} ...]].
-00000620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000630: 2020 2020 2020 2020 2020 5b2d 2d69 676e            [--ign
-00000640: 6f72 652d 6572 726f 7273 207c 202d 2d6e  ore-errors | --n
-00000650: 6f2d 6967 6e6f 7265 2d65 7272 6f72 735d  o-ignore-errors]
-00000660: 205b 2d64 5d20 5b2d 665d 205b 2d46 5d20   [-d] [-f] [-F] 
-00000670: 5b2d 2d73 6b69 702d 6461 6f68 6175 732d  [--skip-daohaus-
-00000680: 6e61 6d65 735d 0a20 2020 2020 2020 2020  names].         
-00000690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006a0: 205b 2d6e 207b 6d61 696e 6e65 742c 6172   [-n {mainnet,ar
-000006b0: 6269 7472 756d 2c78 6461 692c 706f 6c79  bitrum,xdai,poly
-000006c0: 676f 6e7d 205b 7b6d 6169 6e6e 6574 2c61  gon} [{mainnet,a
-000006d0: 7262 6974 7275 6d2c 7864 6169 2c70 6f6c  rbitrum,xdai,pol
-000006e0: 7967 6f6e 7d20 2e2e 2e5d 5d0a 2020 2020  ygon} ...]].    
-000006f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000700: 2020 2020 2020 5b2d 6320 434f 4c4c 4543        [-c COLLEC
-00000710: 544f 5253 205b 434f 4c4c 4543 544f 5253  TORS [COLLECTORS
-00000720: 202e 2e2e 5d5d 205b 2d2d 626c 6f63 6b2d   ...]] [--block-
-00000730: 6461 7465 7469 6d65 2042 4c4f 434b 5f44  datetime BLOCK_D
-00000740: 4154 4554 494d 455d 0a20 2020 2020 2020  ATETIME].       
-00000750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000760: 2020 205b 2d44 2044 4154 4157 4152 4548     [-D DATAWAREH
-00000770: 4f55 5345 5d20 5b2d 2d63 632d 6170 692d  OUSE] [--cc-api-
-00000780: 6b65 7920 4343 5f41 5049 5f4b 4559 5d0a  key CC_API_KEY].
-00000790: 0a4d 6169 6e20 7363 7269 7074 2074 6f20  .Main script to 
-000007a0: 706f 7075 6c61 7465 2064 616f 2d61 6e61  populate dao-ana
-000007b0: 6c79 7a65 7220 6361 6368 650a 0a6f 7074  lyzer cache..opt
-000007c0: 696f 6e73 3a0a 2020 2d68 2c20 2d2d 6865  ions:.  -h, --he
-000007d0: 6c70 2020 2020 2020 2020 2020 2020 7368  lp            sh
-000007e0: 6f77 2074 6869 7320 6865 6c70 206d 6573  ow this help mes
-000007f0: 7361 6765 2061 6e64 2065 7869 740a 2020  sage and exit.  
-00000800: 2d56 2c20 2d2d 7665 7273 696f 6e20 2020  -V, --version   
-00000810: 2020 2020 2020 4469 7370 6c61 7973 2074        Displays t
-00000820: 6865 2076 6572 7369 6f6e 2061 6e64 2065  he version and e
-00000830: 7869 7473 0a20 202d 7020 5b7b 6172 6167  xits.  -p [{arag
-00000840: 6f6e 2c64 616f 6861 7573 2c64 616f 7374  on,daohaus,daost
-00000850: 6163 6b7d 202e 2e2e 5d2c 202d 2d70 6c61  ack} ...], --pla
-00000860: 7466 6f72 6d73 205b 7b61 7261 676f 6e2c  tforms [{aragon,
-00000870: 6461 6f68 6175 732c 6461 6f73 7461 636b  daohaus,daostack
-00000880: 7d20 2e2e 2e5d 0a20 2020 2020 2020 2020  } ...].         
-00000890: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-000008a0: 6865 2070 6c61 7466 6f72 6d73 2074 6f20  he platforms to 
-000008b0: 7570 6461 7465 2e20 4576 6572 7920 706c  update. Every pl
-000008c0: 6174 666f 726d 2069 7320 7570 6461 7465  atform is update
-000008d0: 6420 6279 2064 6566 6175 6c74 2e0a 2020  d by default..  
-000008e0: 2d2d 6967 6e6f 7265 2d65 7272 6f72 732c  --ignore-errors,
-000008f0: 202d 2d6e 6f2d 6967 6e6f 7265 2d65 7272   --no-ignore-err
-00000900: 6f72 730a 2020 2020 2020 2020 2020 2020  ors.            
-00000910: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
-00000920: 6865 7220 746f 2069 676e 6f72 6520 6572  her to ignore er
-00000930: 726f 7273 2061 6e64 2063 6f6e 7469 6e75  rors and continu
-00000940: 6520 2864 6566 6175 6c74 3a20 5472 7565  e (default: True
-00000950: 290a 2020 2d64 2c20 2d2d 6465 6275 6720  ).  -d, --debug 
-00000960: 2020 2020 2020 2020 2020 5368 6f77 7320            Shows 
-00000970: 6465 6275 6720 696e 666f 0a20 202d 662c  debug info.  -f,
-00000980: 202d 2d66 6f72 6365 2020 2020 2020 2020   --force        
-00000990: 2020 2052 656d 6f76 6573 2074 6865 2063     Removes the c
-000009a0: 6163 6865 2062 6566 6f72 6520 7570 6461  ache before upda
-000009b0: 7469 6e67 0a20 202d 462c 202d 2d64 656c  ting.  -F, --del
-000009c0: 6574 652d 666f 7263 6520 2020 2052 656d  ete-force    Rem
-000009d0: 6f76 6573 2074 6865 2064 6174 6177 6172  oves the datawar
-000009e0: 6568 6f75 7365 2066 6f6c 6465 7220 6265  ehouse folder be
-000009f0: 666f 7265 2064 6f69 6e67 2061 6e79 7468  fore doing anyth
-00000a00: 696e 670a 2020 2d2d 736b 6970 2d64 616f  ing.  --skip-dao
-00000a10: 6861 7573 2d6e 616d 6573 2020 536b 6970  haus-names  Skip
-00000a20: 7320 7468 6520 7374 6570 206f 6620 6765  s the step of ge
-00000a30: 7474 696e 6720 4461 6f68 6175 7320 4d6f  tting Daohaus Mo
-00000a40: 6c6f 6368 2773 206e 616d 6573 2c20 7768  loch's names, wh
-00000a50: 6963 6820 7461 6b65 7320 736f 6d65 2074  ich takes some t
-00000a60: 696d 650a 2020 2020 2d6e 207b 6d61 696e  ime.    -n {main
-00000a70: 6e65 742c 6172 6269 7472 756d 2c78 6461  net,arbitrum,xda
-00000a80: 692c 706f 6c79 676f 6e7d 205b 7b6d 6169  i,polygon} [{mai
-00000a90: 6e6e 6574 2c61 7262 6974 7275 6d2c 7864  nnet,arbitrum,xd
-00000aa0: 6169 2c70 6f6c 7967 6f6e 7d20 2e2e 2e5d  ai,polygon} ...]
-00000ab0: 2c20 2d2d 6e65 7477 6f72 6b73 207b 6d61  , --networks {ma
-00000ac0: 696e 6e65 742c 6172 6269 7472 756d 2c78  innet,arbitrum,x
-00000ad0: 6461 692c 706f 6c79 676f 6e7d 205b 7b6d  dai,polygon} [{m
-00000ae0: 6169 6e6e 6574 2c61 7262 6974 7275 6d2c  ainnet,arbitrum,
-00000af0: 7864 6169 2c70 6f6c 7967 6f6e 7d20 2e2e  xdai,polygon} ..
-00000b00: 2e5d 0a20 2020 2020 2020 2020 2020 2020  .].             
-00000b10: 2020 2020 2020 2020 2020 204e 6574 776f             Netwo
-00000b20: 726b 7320 746f 2075 7064 6174 652e 2045  rks to update. E
-00000b30: 7665 7279 206e 6574 776f 726b 2069 7320  very network is 
-00000b40: 7570 6461 7465 6420 6279 2064 6566 6175  updated by defau
-00000b50: 6c74 0a20 202d 6320 434f 4c4c 4543 544f  lt.  -c COLLECTO
-00000b60: 5253 205b 434f 4c4c 4543 544f 5253 202e  RS [COLLECTORS .
-00000b70: 2e2e 5d2c 202d 2d63 6f6c 6c65 6374 6f72  ..], --collector
-00000b80: 7320 434f 4c4c 4543 544f 5253 205b 434f  s COLLECTORS [CO
-00000b90: 4c4c 4543 544f 5253 202e 2e2e 5d0a 2020  LLECTORS ...].  
-00000ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bb0: 2020 2020 2020 436f 6c6c 6563 746f 7273        Collectors
-00000bc0: 2074 6f20 7275 6e2e 2046 6f72 2065 7861   to run. For exa
-00000bd0: 6d70 6c65 3a20 6172 6167 6f6e 2f63 6173  mple: aragon/cas
-00000be0: 7473 0a20 202d 2d62 6c6f 636b 2d64 6174  ts.  --block-dat
-00000bf0: 6574 696d 6520 424c 4f43 4b5f 4441 5445  etime BLOCK_DATE
-00000c00: 5449 4d45 0a20 2020 2020 2020 2020 2020  TIME.           
-00000c10: 2020 2020 2020 2020 2020 2020 2047 6574               Get
-00000c20: 2064 6174 6120 7570 2074 6f20 6120 626c   data up to a bl
-00000c30: 6f63 6b20 6461 7465 7469 6d65 2028 696e  ock datetime (in
-00000c40: 7075 7420 696e 2049 534f 2066 6f72 6d61  put in ISO forma
-00000c50: 7429 0a20 202d 4420 4441 5441 5741 5245  t).  -D DATAWARE
-00000c60: 484f 5553 452c 202d 2d64 6174 6177 6172  HOUSE, --datawar
-00000c70: 6568 6f75 7365 2044 4154 4157 4152 4548  ehouse DATAWAREH
-00000c80: 4f55 5345 0a20 2020 2020 2020 2020 2020  OUSE.           
-00000c90: 2020 2020 2020 2020 2020 2020 2053 7065               Spe
-00000ca0: 6369 6669 6573 2074 6865 2064 6573 7469  cifies the desti
-00000cb0: 6e61 7469 6f6e 2066 6f6c 6465 7220 6f66  nation folder of
-00000cc0: 2074 6865 2064 6174 6177 6172 6568 6f75   the datawarehou
-00000cd0: 7365 0a20 202d 2d63 632d 6170 692d 6b65  se.  --cc-api-ke
-00000ce0: 7920 4343 5f41 5049 5f4b 4559 0a20 2020  y CC_API_KEY.   
-00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d00: 2020 2020 2053 6574 2074 6865 2043 7279       Set the Cry
-00000d10: 7074 6f43 6f6d 7061 7265 2041 5049 206b  ptoCompare API k
-00000d20: 6579 2028 6f76 6572 7269 6465 7320 656e  ey (overrides en
-00000d30: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-00000d40: 6c65 290a 6060 600a 0a23 2323 2047 6574  le).```..### Get
-00000d50: 7469 6e67 206f 6e6c 7920 6461 7461 2066  ting only data f
-00000d60: 726f 6d20 6120 706c 6174 666f 726d 0a59  rom a platform.Y
-00000d70: 6f75 2063 616e 2073 656c 6563 7420 7468  ou can select th
-00000d80: 6520 706c 6174 666f 726d 2074 6f20 646f  e platform to do
-00000d90: 776e 6c6f 6164 2064 6174 6120 6162 6f75  wnload data abou
-00000da0: 7420 7769 7468 2074 6865 2060 2d2d 706c  t with the `--pl
-00000db0: 6174 666f 726d 6020 7365 6c65 6374 6f72  atform` selector
-00000dc0: 2e20 4c65 7427 7320 646f 776e 6c6f 6164  . Let's download
-00000dd0: 206f 6e6c 7920 6461 7461 2066 6f72 2064   only data for d
-00000de0: 616f 7374 6163 6b20 616e 6420 6172 6167  aostack and arag
-00000df0: 6f6e 3a0a 0a60 6060 0a64 616f 612d 6361  on:..```.daoa-ca
-00000e00: 6368 652d 7363 7269 7074 7320 2d2d 706c  che-scripts --pl
-00000e10: 6174 666f 726d 7320 6461 6f73 7461 636b  atforms daostack
-00000e20: 2061 7261 676f 6e0a 6060 600a 0a23 2323   aragon.```..###
-00000e30: 2047 6574 7469 6e67 206f 6e6c 7920 6461   Getting only da
-00000e40: 7461 2066 726f 6d20 6120 6e65 7477 6f72  ta from a networ
-00000e50: 6b0a 596f 7520 6361 6e20 7365 6c65 6374  k.You can select
-00000e60: 2074 6865 2063 6861 696e 2074 6f20 6765   the chain to ge
-00000e70: 7420 6461 7461 2066 726f 6d20 7769 7468  t data from with
-00000e80: 2074 6865 2060 2d2d 6e65 7477 6f72 6b73   the `--networks
-00000e90: 6020 7377 6974 6368 2e20 466f 7220 6578  ` switch. For ex
-00000ea0: 616d 706c 652c 2074 6f20 6765 7420 6461  ample, to get da
-00000eb0: 7461 206f 6e6c 7920 666f 7220 7864 6169  ta only for xdai
-00000ec0: 206e 6574 776f 726b 2c20 796f 7520 6361   network, you ca
-00000ed0: 6e20 646f 3a0a 0a60 6060 0a64 616f 612d  n do:..```.daoa-
-00000ee0: 6361 6368 652d 7363 7269 7074 7320 2d2d  cache-scripts --
-00000ef0: 6e65 7477 6f72 6b73 2078 6461 690a 6060  networks xdai.``
-00000f00: 600a 0a23 2320 4163 6b6e 6f77 6c65 6467  `..## Acknowledg
-00000f10: 656d 656e 7473 0a0a 4441 4f2d 416e 616c  ements..DAO-Anal
-00000f20: 797a 6572 2069 7320 6372 6561 7465 6420  yzer is created 
-00000f30: 756e 6465 7220 7468 6520 756d 6272 656c  under the umbrel
-00000f40: 6c61 206f 6620 7477 6f20 7265 7365 6172  la of two resear
-00000f50: 6368 2070 726f 6a65 6374 733a 2043 6861  ch projects: Cha
-00000f60: 696e 2043 6f6d 6d75 6e69 7479 2c20 6675  in Community, fu
-00000f70: 6e64 6564 2062 7920 7468 6520 5370 616e  nded by the Span
-00000f80: 6973 6820 4d69 6e69 7374 7279 206f 6620  ish Ministry of 
-00000f90: 5363 6965 6e63 6520 616e 6420 496e 6e6f  Science and Inno
-00000fa0: 7661 7469 6f6e 2028 5254 4932 3031 38e2  vation (RTI2018.
-00000fb0: 8090 3039 3638 3230 e280 9041 e280 9049  ..096820...A...I
-00000fc0: 3030 2920 616e 6420 6c65 6420 6279 204a  00) and led by J
-00000fd0: 6176 6965 7220 4172 726f 796f 2061 6e64  avier Arroyo and
-00000fe0: 2053 616d 6572 2048 6173 7361 6e3b 2061   Samer Hassan; a
-00000ff0: 6e64 2050 3250 204d 6f64 656c 732c 2066  nd P2P Models, f
-00001000: 756e 6465 6420 6279 2074 6865 2045 7572  unded by the Eur
-00001010: 6f70 6561 6e20 5265 7365 6172 6368 2043  opean Research C
-00001020: 6f75 6e63 696c 2028 4552 432d 3230 3137  ouncil (ERC-2017
-00001030: 2d53 5447 2036 3235 2067 7261 6e74 206e  -STG 625 grant n
-00001040: 6f2e 3a20 3735 3932 3029 2c20 6c65 6420  o.: 75920), led 
-00001050: 6279 2053 616d 6572 2048 6173 7361 6e2e  by Samer Hassan.
-00001060: 0a0a 2323 2043 6974 6520 6173 0a0a 596f  ..## Cite as..Yo
-00001070: 7520 6361 6e20 6a75 7374 2063 6974 6520  u can just cite 
-00001080: 6f6e 6520 6f66 206f 7572 2070 7562 6c69  one of our publi
-00001090: 6361 7469 6f6e 733a 0a0a 3e20 4a61 7669  cations:..> Javi
-000010a0: 6572 2041 7272 6f79 6f2c 2044 6176 6964  er Arroyo, David
-000010b0: 2044 6176 c3b3 2c20 456c 656e 6120 4d61   Dav.., Elena Ma
-000010c0: 7274 c3ad 6e65 7a2d 5669 6365 6e74 652c  rt..nez-Vicente,
-000010d0: 2059 6f75 7373 6566 2046 6171 6972 2d52   Youssef Faqir-R
-000010e0: 6861 7a6f 7569 2c20 616e 6420 5361 6d65  hazoui, and Same
-000010f0: 7220 4861 7373 616e 2028 3230 3232 292e  r Hassan (2022).
-00001100: 2022 4441 4f2d 416e 616c 797a 6572 3a20   "DAO-Analyzer: 
-00001110: 4578 706c 6f72 696e 6720 4163 7469 7669  Exploring Activi
-00001120: 7479 2061 6e64 2050 6172 7469 6369 7061  ty and Participa
-00001130: 7469 6f6e 2069 6e20 426c 6f63 6b63 6861  tion in Blockcha
-00001140: 696e 204f 7267 616e 697a 6174 696f 6e73  in Organizations
-00001150: 2e22 2e20 436f 6d70 616e 696f 6e20 5075  .". Companion Pu
-00001160: 626c 6963 6174 696f 6e20 6f66 2074 6865  blication of the
-00001170: 2032 3032 3220 436f 6e66 6572 656e 6365   2022 Conference
-00001180: 206f 6e20 436f 6d70 7574 6572 2053 7570   on Computer Sup
-00001190: 706f 7274 6564 2043 6f6f 7065 7261 7469  ported Cooperati
-000011a0: 7665 2057 6f72 6b20 616e 6420 536f 6369  ve Work and Soci
-000011b0: 616c 2043 6f6d 7075 7469 6e67 2028 4353  al Computing (CS
-000011c0: 4357 2732 3220 436f 6d70 616e 696f 6e29  CW'22 Companion)
-000011d0: 2e20 4143 4d2c 2031 3933 e280 9331 3936  . ACM, 193...196
-000011e0: 2e0a 0a4f 722c 2069 6620 796f 7520 7761  ...Or, if you wa
-000011f0: 6e74 2074 6f20 6578 706c 6963 6974 6c79  nt to explicitly
-00001200: 2063 6974 6520 7468 6520 6170 706c 6963   cite the applic
-00001210: 6174 696f 6e3a 0a0a 3e20 4172 726f 796f  ation:..> Arroyo
-00001220: 2c20 4a61 7669 6572 2c20 4461 76c3 b32c  , Javier, Dav..,
-00001230: 2044 6176 6964 2c20 4661 7169 722d 5268   David, Faqir-Rh
-00001240: 617a 6f75 692c 2059 6f75 7373 6566 2c20  azoui, Youssef, 
-00001250: 2620 4d61 7274 c3ad 6e65 7a20 5669 6365  & Mart..nez Vice
-00001260: 6e74 652c 2045 6c65 6e61 2e20 2832 3032  nte, Elena. (202
-00001270: 3329 2e20 4441 4f20 416e 616c 797a 6572  3). DAO Analyzer
-00001280: 2e20 5a65 6e6f 646f 2e20 6874 7470 733a  . Zenodo. https:
-00001290: 2f2f 646f 692e 6f72 672f 3130 2e35 3238  //doi.org/10.528
-000012a0: 312f 7a65 6e6f 646f 2e37 3636 3936 3839  1/zenodo.7669689
-000012b0: 0a0a                                     ..
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 0a20 2020 203c 6120 6872 6566 3d22  ">.    <a href="
+00000020: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000030: 2f70 726f 6a65 6374 2f64 616f 2d73 6372  /project/dao-scr
+00000040: 6970 7473 2f22 3e0a 2020 2020 2020 2020  ipts/">.        
+00000050: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000060: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000070: 2f70 7970 692f 762f 6461 6f2d 7363 7269  /pypi/v/dao-scri
+00000080: 7074 7322 2061 6c74 3d22 5079 5049 223e  pts" alt="PyPI">
+00000090: 0a20 2020 203c 2f61 3e0a 2020 2020 3c61  .    </a>.    <a
+000000a0: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+000000b0: 6f69 2e6f 7267 2f31 302e 3532 3831 2f7a  oi.org/10.5281/z
+000000c0: 656e 6f64 6f2e 3130 3933 3833 3539 223e  enodo.10938359">
+000000d0: 0a20 2020 2020 2020 203c 696d 6720 7372  .        <img sr
+000000e0: 633d 2268 7474 7073 3a2f 2f7a 656e 6f64  c="https://zenod
+000000f0: 6f2e 6f72 672f 6261 6467 652f 444f 492f  o.org/badge/DOI/
+00000100: 3130 2e35 3238 312f 7a65 6e6f 646f 2e31  10.5281/zenodo.1
+00000110: 3039 3338 3335 392e 7376 6722 2061 6c74  0938359.svg" alt
+00000120: 3d22 444f 4920 3130 2e35 3238 312f 7a65  ="DOI 10.5281/ze
+00000130: 6e6f 646f 2e31 3039 3338 3335 392e 7376  nodo.10938359.sv
+00000140: 6722 3e0a 2020 2020 3c2f 613e 0a20 2020  g">.    </a>.   
+00000150: 203c 6120 6872 6566 3d22 2e2f 4c49 4345   <a href="./LICE
+00000160: 4e53 4522 3e0a 2020 2020 2020 3c69 6d67  NSE">.      <img
+00000170: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000180: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000190: 6875 622f 6c69 6365 6e73 652f 6772 6173  hub/license/gras
+000001a0: 6961 2f64 616f 2d73 6372 6970 7473 2220  ia/dao-scripts" 
+000001b0: 616c 743d 224c 6963 656e 7365 223e 0a20  alt="License">. 
+000001c0: 2020 203c 2f61 3e0a 2020 2020 3c61 2068     </a>.    <a h
+000001d0: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
+000001e0: 2e6b 6167 676c 652e 636f 6d2f 6461 7461  .kaggle.com/data
+000001f0: 7365 7473 2f64 6176 6964 6461 766f 2f64  sets/daviddavo/d
+00000200: 616f 2d61 6e61 6c79 7a65 7222 3e0a 2020  ao-analyzer">.  
+00000210: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000220: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000230: 732e 696f 2f62 6164 6765 2f4b 6167 676c  s.io/badge/Kaggl
+00000240: 652d 3230 4245 4646 3f6c 6f67 6f3d 4b61  e-20BEFF?logo=Ka
+00000250: 6767 6c65 266c 6f67 6f43 6f6c 6f72 3d77  ggle&logoColor=w
+00000260: 6869 7465 2220 616c 743d 224b 6167 676c  hite" alt="Kaggl
+00000270: 6522 3e0a 2020 2020 3c2f 613e 0a3c 2f70  e">.    </a>.</p
+00000280: 3e0a 0a23 2044 414f 2d41 6e61 6c79 7a65  >..# DAO-Analyze
+00000290: 7227 7320 6361 6368 652d 7363 7269 7074  r's cache-script
+000002a0: 730a 0a23 2320 5365 742d 7570 2026 2052  s..## Set-up & R
+000002b0: 756e 6e69 6e67 0a0a 5468 6520 6561 7369  unning..The easi
+000002c0: 6573 7420 6d65 7468 6f64 2062 7920 6661  est method by fa
+000002d0: 7220 746f 2064 6f77 6e6c 6f61 6420 616e  r to download an
+000002e0: 6420 7275 6e20 7468 6520 6170 706c 6963  d run the applic
+000002f0: 6174 696f 6e20 6973 2074 6f20 7573 6520  ation is to use 
+00000300: 7069 7020 746f 2069 6e73 7461 6c6c 2069  pip to install i
+00000310: 740a 0a60 6060 0a70 6970 2069 6e73 7461  t..```.pip insta
+00000320: 6c6c 2064 616f 2d73 6372 6970 7473 0a60  ll dao-scripts.`
+00000330: 6060 0a0a 5468 656e 2c20 796f 7520 6361  ``..Then, you ca
+00000340: 6e20 7573 6520 7468 6973 2073 6372 6970  n use this scrip
+00000350: 7420 7573 696e 6720 7468 6520 636f 6d6d  t using the comm
+00000360: 616e 6420 6064 616f 612d 6361 6368 652d  and `daoa-cache-
+00000370: 7363 7269 7074 7360 206f 7220 6064 616f  scripts` or `dao
+00000380: 2d73 6372 6970 7473 600a 0a23 2323 2044  -scripts`..### D
+00000390: 6f77 6e6c 6f61 640a 456e 7465 7220 696e  ownload.Enter in
+000003a0: 2079 6f75 7220 7465 726d 696e 616c 2028   your terminal (
+000003b0: 6769 7420 6d75 7374 2062 6520 696e 7374  git must be inst
+000003c0: 616c 6c65 6429 2061 6e64 2077 7269 7465  alled) and write
+000003d0: 2064 6f77 6e3a 0a0a 6060 600a 6769 7420   down:..```.git 
+000003e0: 636c 6f6e 6520 6874 7470 733a 2f2f 6769  clone https://gi
+000003f0: 7468 7562 2e63 6f6d 2f47 7261 7369 612f  thub.com/Grasia/
+00000400: 6461 6f2d 7363 7269 7074 730a 6060 600a  dao-scripts.```.
+00000410: 0a41 6674 6572 2074 6861 742c 206d 6f76  .After that, mov
+00000420: 6520 746f 2074 6865 2072 6570 6f73 6974  e to the reposit
+00000430: 6f72 7920 726f 6f74 2064 6972 6563 746f  ory root directo
+00000440: 7279 2077 6974 683a 0a0a 6060 600a 6364  ry with:..```.cd
+00000450: 2064 616f 2d73 6372 6970 7473 0a60 6060   dao-scripts.```
+00000460: 0a0a 2323 2320 496e 7374 616c 6c61 7469  ..### Installati
+00000470: 6f6e 0a41 6c6c 2063 6f64 6520 6861 7320  on.All code has 
+00000480: 6265 656e 2074 6573 7465 6420 6f6e 204c  been tested on L
+00000490: 696e 7578 2c20 6275 7420 6974 2073 686f  inux, but it sho
+000004a0: 756c 6420 776f 726b 206f 6e20 5769 6e64  uld work on Wind
+000004b0: 6f77 7320 616e 6420 6d61 634f 532c 2027  ows and macOS, '
+000004c0: 6361 7573 6520 6974 206a 7573 7420 7573  cause it just us
+000004d0: 6573 2074 6865 2050 7974 686f 6e20 656e  es the Python en
+000004e0: 7669 726f 6e6d 656e 742e 0a0a 536f 2c20  vironment...So, 
+000004f0: 796f 7520 6d75 7374 2069 6e73 7461 6c6c  you must install
+00000500: 2074 6865 2066 6f6c 6c6f 7769 6e67 2064   the following d
+00000510: 6570 656e 6465 6e63 6965 7320 746f 2072  ependencies to r
+00000520: 756e 2074 6865 2074 6f6f 6c3a 0a0a 2a20  un the tool:..* 
+00000530: 7079 7468 6f6e 3320 2833 2e31 3020 6f72  python3 (3.10 or
+00000540: 206c 6174 6572 290a 2a20 7079 7468 6f6e   later).* python
+00000550: 332d 7069 700a 0a4e 6f77 2c20 696e 7374  3-pip..Now, inst
+00000560: 616c 6c20 7468 6520 5079 7468 6f6e 2064  all the Python d
+00000570: 6570 656e 6465 6e63 6965 733a 0a0a 6070  ependencies:..`p
+00000580: 6970 3320 696e 7374 616c 6c20 2d72 2072  ip3 install -r r
+00000590: 6571 7569 7265 6d65 6e74 732e 7478 7460  equirements.txt`
+000005a0: 0a0a 4966 2079 6f75 2064 6f6e 2774 2077  ..If you don't w
+000005b0: 616e 7420 746f 2073 6861 7265 2050 7974  ant to share Pyt
+000005c0: 686f 6e20 6465 7065 6e64 656e 6369 6573  hon dependencies
+000005d0: 2061 6d6f 6e67 206f 7468 6572 2070 726f   among other pro
+000005e0: 6a65 6374 732c 2079 6f75 2073 686f 756c  jects, you shoul
+000005f0: 6420 7573 6520 6120 7669 7274 7561 6c20  d use a virtual 
+00000600: 656e 7669 726f 6e6d 656e 742c 2073 7563  environment, suc
+00000610: 6820 6173 205b 7669 7274 7561 6c65 6e76  h as [virtualenv
+00000620: 5d28 6874 7470 733a 2f2f 646f 6373 2e70  ](https://docs.p
+00000630: 7974 686f 6e2d 6775 6964 652e 6f72 672f  ython-guide.org/
+00000640: 6465 762f 7669 7274 7561 6c65 6e76 732f  dev/virtualenvs/
+00000650: 292e 0a0a 2323 2320 486f 7720 746f 2072  )...### How to r
+00000660: 756e 2069 743f 0a49 6620 796f 7520 7761  un it?.If you wa
+00000670: 6e74 2061 6c6c 2074 6865 2064 6174 6120  nt all the data 
+00000680: 7573 6564 2069 6e20 7468 6520 6170 702c  used in the app,
+00000690: 2079 6f75 2063 616e 206a 7573 7420 7573   you can just us
+000006a0: 653a 0a0a 6060 600a 6461 6f2d 7363 7269  e:..```.dao-scri
+000006b0: 7074 730a 6060 600a 0a74 6869 7320 7769  pts.```..this wi
+000006c0: 6c6c 2063 7265 6174 6520 6120 666f 6c64  ll create a fold
+000006d0: 6572 2063 616c 6c65 6420 6064 6174 6177  er called `dataw
+000006e0: 6172 6568 6f75 7365 6020 7769 7468 2061  arehouse` with a
+000006f0: 206c 6f74 206f 6620 6669 6c65 7320 696e   lot of files in
+00000700: 2041 7061 6368 6527 7320 6172 726f 7720   Apache's arrow 
+00000710: 666f 726d 6174 2e0a 0a59 6f75 2063 616e  format...You can
+00000720: 2069 6d70 6f72 7420 7468 6f73 6520 6669   import those fi
+00000730: 6c65 7320 746f 2060 7061 6e64 6173 6020  les to `pandas` 
+00000740: 7769 7468 2060 7265 6164 5f66 6561 7468  with `read_feath
+00000750: 6572 602e 2046 6f72 2065 7861 6d70 6c65  er`. For example
+00000760: 3a0a 0a60 6060 7079 7468 6f6e 0a70 642e  :..```python.pd.
+00000770: 7265 6164 5f66 6561 7468 6572 2827 6461  read_feather('da
+00000780: 7461 7761 7265 686f 7573 652f 6172 6167  tawarehouse/arag
+00000790: 6f6e 2f61 7070 732e 6172 7227 290a 6060  on/apps.arr').``
+000007a0: 600a 0a23 2320 5573 6167 6520 6775 6964  `..## Usage guid
+000007b0: 650a 4966 2079 6f75 2064 6f6e 2774 2077  e.If you don't w
+000007c0: 616e 7420 616c 6c20 7468 6520 6461 7461  ant all the data
+000007d0: 2028 616e 6420 6974 2063 616e 2074 616b   (and it can tak
+000007e0: 6520 6120 6c6f 7420 6f66 2074 696d 6529  e a lot of time)
+000007f0: 2c20 796f 7520 6861 7665 2061 206c 6f74  , you have a lot
+00000800: 206f 6620 6f70 7469 6f6e 7320 6176 6169   of options avai
+00000810: 6c61 626c 6520 746f 2073 656c 6563 7420  lable to select 
+00000820: 7768 6963 6865 7665 7220 6461 7461 2079  whichever data y
+00000830: 6f75 2077 616e 742e 2054 6865 2066 756c  ou want. The ful
+00000840: 6c20 602d 2d68 656c 7060 206f 7574 7075  l `--help` outpu
+00000850: 7420 6973 0a0a 6060 600a 7573 6167 653a  t is..```.usage:
+00000860: 2064 616f 612d 6361 6368 652d 7363 7269   daoa-cache-scri
+00000870: 7074 7320 5b2d 685d 205b 2d56 5d20 5b2d  pts [-h] [-V] [-
+00000880: 7020 5b7b 6172 6167 6f6e 2c64 616f 6861  p [{aragon,daoha
+00000890: 7573 2c64 616f 7374 6163 6b7d 202e 2e2e  us,daostack} ...
+000008a0: 5d5d 0a20 2020 2020 2020 2020 2020 2020  ]].             
+000008b0: 2020 2020 2020 2020 2020 2020 205b 2d2d               [--
+000008c0: 6967 6e6f 7265 2d65 7272 6f72 7320 7c20  ignore-errors | 
+000008d0: 2d2d 6e6f 2d69 676e 6f72 652d 6572 726f  --no-ignore-erro
+000008e0: 7273 5d20 5b2d 645d 205b 2d66 5d20 5b2d  rs] [-d] [-f] [-
+000008f0: 465d 205b 2d2d 736b 6970 2d64 616f 6861  F] [--skip-daoha
+00000900: 7573 2d6e 616d 6573 5d0a 2020 2020 2020  us-names].      
+00000910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000920: 2020 2020 5b2d 6e20 7b6d 6169 6e6e 6574      [-n {mainnet
+00000930: 2c61 7262 6974 7275 6d2c 7864 6169 2c70  ,arbitrum,xdai,p
+00000940: 6f6c 7967 6f6e 7d20 5b7b 6d61 696e 6e65  olygon} [{mainne
+00000950: 742c 6172 6269 7472 756d 2c78 6461 692c  t,arbitrum,xdai,
+00000960: 706f 6c79 676f 6e7d 202e 2e2e 5d5d 0a20  polygon} ...]]. 
+00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000980: 2020 2020 2020 2020 205b 2d63 2043 4f4c           [-c COL
+00000990: 4c45 4354 4f52 5320 5b43 4f4c 4c45 4354  LECTORS [COLLECT
+000009a0: 4f52 5320 2e2e 2e5d 5d20 5b2d 2d62 6c6f  ORS ...]] [--blo
+000009b0: 636b 2d64 6174 6574 696d 6520 424c 4f43  ck-datetime BLOC
+000009c0: 4b5f 4441 5445 5449 4d45 5d0a 2020 2020  K_DATETIME].    
+000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009e0: 2020 2020 2020 5b2d 4420 4441 5441 5741        [-D DATAWA
+000009f0: 5245 484f 5553 455d 0a0a 4d61 696e 2073  REHOUSE]..Main s
+00000a00: 6372 6970 7420 746f 2070 6f70 756c 6174  cript to populat
+00000a10: 6520 6461 6f2d 616e 616c 797a 6572 2063  e dao-analyzer c
+00000a20: 6163 6865 0a0a 6f70 7469 6f6e 733a 0a20  ache..options:. 
+00000a30: 202d 682c 202d 2d68 656c 7020 2020 2020   -h, --help     
+00000a40: 2020 2020 2020 2073 686f 7720 7468 6973         show this
+00000a50: 2068 656c 7020 6d65 7373 6167 6520 616e   help message an
+00000a60: 6420 6578 6974 0a20 202d 562c 202d 2d76  d exit.  -V, --v
+00000a70: 6572 7369 6f6e 2020 2020 2020 2020 2044  ersion         D
+00000a80: 6973 706c 6179 7320 7468 6520 7665 7273  isplays the vers
+00000a90: 696f 6e20 616e 6420 6578 6974 730a 2020  ion and exits.  
+00000aa0: 2d70 205b 7b61 7261 676f 6e2c 6461 6f68  -p [{aragon,daoh
+00000ab0: 6175 732c 6461 6f73 7461 636b 7d20 2e2e  aus,daostack} ..
+00000ac0: 2e5d 2c20 2d2d 706c 6174 666f 726d 7320  .], --platforms 
+00000ad0: 5b7b 6172 6167 6f6e 2c64 616f 6861 7573  [{aragon,daohaus
+00000ae0: 2c64 616f 7374 6163 6b7d 202e 2e2e 5d0a  ,daostack} ...].
+00000af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b00: 2020 2020 2020 2020 5468 6520 706c 6174          The plat
+00000b10: 666f 726d 7320 746f 2075 7064 6174 652e  forms to update.
+00000b20: 2045 7665 7279 2070 6c61 7466 6f72 6d20   Every platform 
+00000b30: 6973 2075 7064 6174 6564 2062 7920 6465  is updated by de
+00000b40: 6661 756c 742e 0a20 202d 2d69 676e 6f72  fault..  --ignor
+00000b50: 652d 6572 726f 7273 2c20 2d2d 6e6f 2d69  e-errors, --no-i
+00000b60: 676e 6f72 652d 6572 726f 7273 0a20 2020  gnore-errors.   
+00000b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b80: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
+00000b90: 6967 6e6f 7265 2065 7272 6f72 7320 616e  ignore errors an
+00000ba0: 6420 636f 6e74 696e 7565 2028 6465 6661  d continue (defa
+00000bb0: 756c 743a 2054 7275 6529 0a20 202d 642c  ult: True).  -d,
+00000bc0: 202d 2d64 6562 7567 2020 2020 2020 2020   --debug        
+00000bd0: 2020 2053 686f 7773 2064 6562 7567 2069     Shows debug i
+00000be0: 6e66 6f0a 2020 2d66 2c20 2d2d 666f 7263  nfo.  -f, --forc
+00000bf0: 6520 2020 2020 2020 2020 2020 5265 6d6f  e           Remo
+00000c00: 7665 7320 7468 6520 6361 6368 6520 6265  ves the cache be
+00000c10: 666f 7265 2075 7064 6174 696e 670a 2020  fore updating.  
+00000c20: 2d46 2c20 2d2d 6465 6c65 7465 2d66 6f72  -F, --delete-for
+00000c30: 6365 2020 2020 5265 6d6f 7665 7320 7468  ce    Removes th
+00000c40: 6520 6461 7461 7761 7265 686f 7573 6520  e datawarehouse 
+00000c50: 666f 6c64 6572 2062 6566 6f72 6520 646f  folder before do
+00000c60: 696e 6720 616e 7974 6869 6e67 0a20 202d  ing anything.  -
+00000c70: 2d73 6b69 702d 6461 6f68 6175 732d 6e61  -skip-daohaus-na
+00000c80: 6d65 7320 2053 6b69 7073 2074 6865 2073  mes  Skips the s
+00000c90: 7465 7020 6f66 2067 6574 7469 6e67 2044  tep of getting D
+00000ca0: 616f 6861 7573 204d 6f6c 6f63 6827 7320  aohaus Moloch's 
+00000cb0: 6e61 6d65 732c 2077 6869 6368 2074 616b  names, which tak
+00000cc0: 6573 2073 6f6d 6520 7469 6d65 0a20 2020  es some time.   
+00000cd0: 202d 6e20 7b6d 6169 6e6e 6574 2c61 7262   -n {mainnet,arb
+00000ce0: 6974 7275 6d2c 7864 6169 2c70 6f6c 7967  itrum,xdai,polyg
+00000cf0: 6f6e 7d20 5b7b 6d61 696e 6e65 742c 6172  on} [{mainnet,ar
+00000d00: 6269 7472 756d 2c78 6461 692c 706f 6c79  bitrum,xdai,poly
+00000d10: 676f 6e7d 202e 2e2e 5d2c 202d 2d6e 6574  gon} ...], --net
+00000d20: 776f 726b 7320 7b6d 6169 6e6e 6574 2c61  works {mainnet,a
+00000d30: 7262 6974 7275 6d2c 7864 6169 2c70 6f6c  rbitrum,xdai,pol
+00000d40: 7967 6f6e 7d20 5b7b 6d61 696e 6e65 742c  ygon} [{mainnet,
+00000d50: 6172 6269 7472 756d 2c78 6461 692c 706f  arbitrum,xdai,po
+00000d60: 6c79 676f 6e7d 202e 2e2e 5d0a 2020 2020  lygon} ...].    
+00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d80: 2020 2020 4e65 7477 6f72 6b73 2074 6f20      Networks to 
+00000d90: 7570 6461 7465 2e20 4576 6572 7920 6e65  update. Every ne
+00000da0: 7477 6f72 6b20 6973 2075 7064 6174 6564  twork is updated
+00000db0: 2062 7920 6465 6661 756c 740a 2020 2d63   by default.  -c
+00000dc0: 2043 4f4c 4c45 4354 4f52 5320 5b43 4f4c   COLLECTORS [COL
+00000dd0: 4c45 4354 4f52 5320 2e2e 2e5d 2c20 2d2d  LECTORS ...], --
+00000de0: 636f 6c6c 6563 746f 7273 2043 4f4c 4c45  collectors COLLE
+00000df0: 4354 4f52 5320 5b43 4f4c 4c45 4354 4f52  CTORS [COLLECTOR
+00000e00: 5320 2e2e 2e5d 0a20 2020 2020 2020 2020  S ...].         
+00000e10: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+00000e20: 6f6c 6c65 6374 6f72 7320 746f 2072 756e  ollectors to run
+00000e30: 2e20 466f 7220 6578 616d 706c 653a 2061  . For example: a
+00000e40: 7261 676f 6e2f 6361 7374 730a 2020 2d2d  ragon/casts.  --
+00000e50: 626c 6f63 6b2d 6461 7465 7469 6d65 2042  block-datetime B
+00000e60: 4c4f 434b 5f44 4154 4554 494d 450a 2020  LOCK_DATETIME.  
+00000e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e80: 2020 2020 2020 4765 7420 6461 7461 2075        Get data u
+00000e90: 7020 746f 2061 2062 6c6f 636b 2064 6174  p to a block dat
+00000ea0: 6574 696d 6520 2869 6e70 7574 2069 6e20  etime (input in 
+00000eb0: 4953 4f20 666f 726d 6174 290a 2020 2d44  ISO format).  -D
+00000ec0: 2044 4154 4157 4152 4548 4f55 5345 2c20   DATAWAREHOUSE, 
+00000ed0: 2d2d 6461 7461 7761 7265 686f 7573 6520  --datawarehouse 
+00000ee0: 4441 5441 5741 5245 484f 5553 450a 2020  DATAWAREHOUSE.  
+00000ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f00: 2020 2020 2020 5370 6563 6966 6965 7320        Specifies 
+00000f10: 7468 6520 6465 7374 696e 6174 696f 6e20  the destination 
+00000f20: 666f 6c64 6572 206f 6620 7468 6520 6461  folder of the da
+00000f30: 7461 7761 7265 686f 7573 650a 6060 600a  tawarehouse.```.
+00000f40: 0a23 2323 2047 6574 7469 6e67 206f 6e6c  .### Getting onl
+00000f50: 7920 6461 7461 2066 726f 6d20 6120 706c  y data from a pl
+00000f60: 6174 666f 726d 0a59 6f75 2063 616e 2073  atform.You can s
+00000f70: 656c 6563 7420 7468 6520 706c 6174 666f  elect the platfo
+00000f80: 726d 2074 6f20 646f 776e 6c6f 6164 2064  rm to download d
+00000f90: 6174 6120 6162 6f75 7420 7769 7468 2074  ata about with t
+00000fa0: 6865 2060 2d2d 706c 6174 666f 726d 6020  he `--platform` 
+00000fb0: 7365 6c65 6374 6f72 2e20 4c65 7427 7320  selector. Let's 
+00000fc0: 646f 776e 6c6f 6164 206f 6e6c 7920 6461  download only da
+00000fd0: 7461 2066 6f72 2064 616f 7374 6163 6b20  ta for daostack 
+00000fe0: 616e 6420 6172 6167 6f6e 3a0a 0a60 6060  and aragon:..```
+00000ff0: 0a64 616f 612d 6361 6368 652d 7363 7269  .daoa-cache-scri
+00001000: 7074 7320 2d2d 706c 6174 666f 726d 7320  pts --platforms 
+00001010: 6461 6f73 7461 636b 2061 7261 676f 6e0a  daostack aragon.
+00001020: 6060 600a 0a23 2323 2047 6574 7469 6e67  ```..### Getting
+00001030: 206f 6e6c 7920 6461 7461 2066 726f 6d20   only data from 
+00001040: 6120 6e65 7477 6f72 6b0a 596f 7520 6361  a network.You ca
+00001050: 6e20 7365 6c65 6374 2074 6865 2063 6861  n select the cha
+00001060: 696e 2074 6f20 6765 7420 6461 7461 2066  in to get data f
+00001070: 726f 6d20 7769 7468 2074 6865 2060 2d2d  rom with the `--
+00001080: 6e65 7477 6f72 6b73 6020 7377 6974 6368  networks` switch
+00001090: 2e20 466f 7220 6578 616d 706c 652c 2074  . For example, t
+000010a0: 6f20 6765 7420 6461 7461 206f 6e6c 7920  o get data only 
+000010b0: 666f 7220 7864 6169 206e 6574 776f 726b  for xdai network
+000010c0: 2c20 796f 7520 6361 6e20 646f 3a0a 0a60  , you can do:..`
+000010d0: 6060 0a64 616f 612d 6361 6368 652d 7363  ``.daoa-cache-sc
+000010e0: 7269 7074 7320 2d2d 6e65 7477 6f72 6b73  ripts --networks
+000010f0: 2078 6461 690a 6060 600a 0a23 2320 4163   xdai.```..## Ac
+00001100: 6b6e 6f77 6c65 6467 656d 656e 7473 0a0a  knowledgements..
+00001110: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00001120: 6572 223e 0a3c 696d 6720 7372 633d 2268  er">.<img src="h
+00001130: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001140: 6d2f 4772 6173 6961 2f64 616f 2d61 6e61  m/Grasia/dao-ana
+00001150: 6c79 7a65 722f 626c 6f62 2f6d 6173 7465  lyzer/blob/maste
+00001160: 722f 6461 6f5f 616e 616c 797a 6572 2f77  r/dao_analyzer/w
+00001170: 6562 2f61 7373 6574 732f 6c6f 676f 2d6d  eb/assets/logo-m
+00001180: 696e 6973 7465 7269 6f2e 706e 673f 7261  inisterio.png?ra
+00001190: 773d 7472 7565 220a 2020 2020 2061 6c74  w=true".     alt
+000011a0: 3d22 4c6f 676f 204d 696e 6973 7465 7269  ="Logo Ministeri
+000011b0: 6f20 6465 2043 6965 6e63 6961 2065 2049  o de Ciencia e I
+000011c0: 6e6e 6f76 6163 69c3 b36e 2e20 476f 6269  nnovaci..n. Gobi
+000011d0: 6572 6e6f 2064 6520 4573 7061 c3b1 6122  erno de Espa..a"
+000011e0: 0a20 2020 2020 7374 796c 653d 226d 6178  .     style="max
+000011f0: 2d68 6569 6768 743a 2033 656d 220a 3e3c  -height: 3em".><
+00001200: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00001210: 2f67 6974 6875 622e 636f 6d2f 4772 6173  /github.com/Gras
+00001220: 6961 2f64 616f 2d61 6e61 6c79 7a65 722f  ia/dao-analyzer/
+00001230: 626c 6f62 2f6d 6173 7465 722f 6461 6f5f  blob/master/dao_
+00001240: 616e 616c 797a 6572 2f77 6562 2f61 7373  analyzer/web/ass
+00001250: 6574 732f 6c6f 676f 2d65 7263 2e70 6e67  ets/logo-erc.png
+00001260: 3f72 6177 3d74 7275 6522 0a20 2020 2020  ?raw=true".     
+00001270: 616c 743d 224c 6f67 6f74 6970 6f20 4575  alt="Logotipo Eu
+00001280: 726f 7065 616e 2052 6573 6561 7263 6820  ropean Research 
+00001290: 436f 756e 6369 6c22 0a20 2020 2020 7374  Council".     st
+000012a0: 796c 653d 226d 6178 2d68 6569 6768 743a  yle="max-height:
+000012b0: 2033 656d 220a 3e3c 696d 6720 7372 633d   3em".><img src=
+000012c0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000012d0: 636f 6d2f 4772 6173 6961 2f64 616f 2d61  com/Grasia/dao-a
+000012e0: 6e61 6c79 7a65 722f 626c 6f62 2f6d 6173  nalyzer/blob/mas
+000012f0: 7465 722f 6461 6f5f 616e 616c 797a 6572  ter/dao_analyzer
+00001300: 2f77 6562 2f61 7373 6574 732f 6c6f 676f  /web/assets/logo
+00001310: 2d67 7261 7369 612e 706e 673f 7261 773d  -grasia.png?raw=
+00001320: 7472 7565 220a 2020 2020 2061 6c74 3d22  true".     alt="
+00001330: 4c6f 676f 2047 5241 5349 4120 5543 4d22  Logo GRASIA UCM"
+00001340: 0a20 2020 2020 7374 796c 653d 226d 6178  .     style="max
+00001350: 2d68 6569 6768 743a 2033 656d 220a 3e3c  -height: 3em".><
+00001360: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00001370: 2f67 6974 6875 622e 636f 6d2f 4772 6173  /github.com/Gras
+00001380: 6961 2f64 616f 2d61 6e61 6c79 7a65 722f  ia/dao-analyzer/
+00001390: 626c 6f62 2f6d 6173 7465 722f 6461 6f5f  blob/master/dao_
+000013a0: 616e 616c 797a 6572 2f77 6562 2f61 7373  analyzer/web/ass
+000013b0: 6574 732f 6c6f 676f 2d75 636d 2e70 6e67  ets/logo-ucm.png
+000013c0: 3f72 6177 3d74 7275 6522 0a20 2020 2020  ?raw=true".     
+000013d0: 616c 743d 224c 6f67 6f20 556e 6976 6572  alt="Logo Univer
+000013e0: 7369 6461 6420 436f 6d70 6c75 7465 6e73  sidad Complutens
+000013f0: 6520 6465 204d 6164 7269 6422 0a20 2020  e de Madrid".   
+00001400: 2020 7374 796c 653d 226d 6178 2d68 6569    style="max-hei
+00001410: 6768 743a 2033 656d 220a 3e0a 3c2f 6469  ght: 3em".>.</di
+00001420: 763e 0a0a 4441 4f2d 416e 616c 797a 6572  v>..DAO-Analyzer
+00001430: 2069 7320 6372 6561 7465 6420 756e 6465   is created unde
+00001440: 7220 7468 6520 756d 6272 656c 6c61 206f  r the umbrella o
+00001450: 6620 6d75 6c74 6970 6c65 2072 6573 6561  f multiple resea
+00001460: 7263 6820 7072 6f6a 6563 7473 3a20 0a2d  rch projects: .-
+00001470: 2043 6861 696e 2043 6f6d 6d75 6e69 7479   Chain Community
+00001480: 2c20 6675 6e64 6564 2062 7920 7468 6520  , funded by the 
+00001490: 5370 616e 6973 6820 4d69 6e69 7374 7279  Spanish Ministry
+000014a0: 206f 6620 5363 6965 6e63 6520 616e 6420   of Science and 
+000014b0: 496e 6e6f 7661 7469 6f6e 2028 5b52 5449  Innovation ([RTI
+000014c0: 3230 3138 e280 9030 3936 3832 30e2 8090  2018...096820...
+000014d0: 41e2 8090 4930 305d 2868 7474 7073 3a2f  A...I00](https:/
+000014e0: 2f70 726f 6475 6363 696f 6e63 6965 6e74  /produccioncient
+000014f0: 6966 6963 612e 7563 6d2e 6573 2f70 726f  ifica.ucm.es/pro
+00001500: 7965 6374 6f73 2f34 3831 3033 2f64 6574  yectos/48103/det
+00001510: 616c 6c65 2929 2061 6e64 206c 6564 2062  alle)) and led b
+00001520: 7920 4a61 7669 6572 2041 7272 6f79 6f20  y Javier Arroyo 
+00001530: 616e 6420 5361 6d65 7220 4861 7373 616e  and Samer Hassan
+00001540: 0a2d 2050 3250 204d 6f64 656c 732c 2066  .- P2P Models, f
+00001550: 756e 6465 6420 6279 2074 6865 2045 7572  unded by the Eur
+00001560: 6f70 6561 6e20 5265 7365 6172 6368 2043  opean Research C
+00001570: 6f75 6e63 696c 2028 4552 432d 3230 3137  ouncil (ERC-2017
+00001580: 2d53 5447 2036 3235 2067 7261 6e74 206e  -STG 625 grant n
+00001590: 6f2e 3a20 3735 3932 3029 2c20 6c65 6420  o.: 75920), led 
+000015a0: 6279 2053 616d 6572 2048 6173 7361 6e2e  by Samer Hassan.
+000015b0: 0a2d 2044 414f 6170 706c 6963 6174 696f  .- DAOapplicatio
+000015c0: 6e73 2c20 6675 6e64 6564 2062 7920 7468  ns, funded by th
+000015d0: 6520 5370 616e 6973 6820 4d69 6e69 7374  e Spanish Minist
+000015e0: 7279 206f 6620 5363 6965 6e63 6520 616e  ry of Science an
+000015f0: 6420 496e 6e6f 7661 7469 6f6e 2028 5b50  d Innovation ([P
+00001600: 4944 3230 3231 2d31 3237 3935 364f 422d  ID2021-127956OB-
+00001610: 4930 305d 2868 7474 7073 3a2f 2f70 726f  I00](https://pro
+00001620: 6475 6363 696f 6e63 6965 6e74 6966 6963  duccioncientific
+00001630: 612e 7563 6d2e 6573 2f70 726f 7965 6374  a.ucm.es/proyect
+00001640: 6f73 2f35 3531 3137 312f 6465 7461 6c6c  os/551171/detall
+00001650: 6529 2920 616e 6420 6c65 6420 6279 204a  e)) and led by J
+00001660: 6176 6965 7220 4172 726f 796f 2c20 5361  avier Arroyo, Sa
+00001670: 6d65 7220 4861 7373 616e 2061 6e64 206d  mer Hassan and m
+00001680: 6172 6961 2043 7275 7a20 5661 6c69 656e  aria Cruz Valien
+00001690: 7465 0a0a 2323 2043 6974 6520 6173 0a0a  te..## Cite as..
+000016a0: 596f 7520 6361 6e20 6a75 7374 2063 6974  You can just cit
+000016b0: 6520 6f6e 6520 6f66 206f 7572 2070 7562  e one of our pub
+000016c0: 6c69 6361 7469 6f6e 733a 0a0a 3e20 4a61  lications:..> Ja
+000016d0: 7669 6572 2041 7272 6f79 6f2c 2044 6176  vier Arroyo, Dav
+000016e0: 6964 2044 6176 c3b3 2c20 456c 656e 6120  id Dav.., Elena 
+000016f0: 4d61 7274 c3ad 6e65 7a2d 5669 6365 6e74  Mart..nez-Vicent
+00001700: 652c 2059 6f75 7373 6566 2046 6171 6972  e, Youssef Faqir
+00001710: 2d52 6861 7a6f 7569 2c20 616e 6420 5361  -Rhazoui, and Sa
+00001720: 6d65 7220 4861 7373 616e 2028 3230 3232  mer Hassan (2022
+00001730: 292e 2022 4441 4f2d 416e 616c 797a 6572  ). "DAO-Analyzer
+00001740: 3a20 4578 706c 6f72 696e 6720 4163 7469  : Exploring Acti
+00001750: 7669 7479 2061 6e64 2050 6172 7469 6369  vity and Partici
+00001760: 7061 7469 6f6e 2069 6e20 426c 6f63 6b63  pation in Blockc
+00001770: 6861 696e 204f 7267 616e 697a 6174 696f  hain Organizatio
+00001780: 6e73 2e22 2e20 436f 6d70 616e 696f 6e20  ns.". Companion 
+00001790: 5075 626c 6963 6174 696f 6e20 6f66 2074  Publication of t
+000017a0: 6865 2032 3032 3220 436f 6e66 6572 656e  he 2022 Conferen
+000017b0: 6365 206f 6e20 436f 6d70 7574 6572 2053  ce on Computer S
+000017c0: 7570 706f 7274 6564 2043 6f6f 7065 7261  upported Coopera
+000017d0: 7469 7665 2057 6f72 6b20 616e 6420 536f  tive Work and So
+000017e0: 6369 616c 2043 6f6d 7075 7469 6e67 2028  cial Computing (
+000017f0: 4353 4357 2732 3220 436f 6d70 616e 696f  CSCW'22 Companio
+00001800: 6e29 2e20 4143 4d2c 2031 3933 e280 9331  n). ACM, 193...1
+00001810: 3936 2e0a 0a4f 722c 2069 6620 796f 7520  96...Or, if you 
+00001820: 7761 6e74 2074 6f20 6578 706c 6963 6974  want to explicit
+00001830: 6c79 2063 6974 6520 7468 6520 6170 706c  ly cite the appl
+00001840: 6963 6174 696f 6e3a 0a0a 3e20 4172 726f  ication:..> Arro
+00001850: 796f 2c20 4a61 7669 6572 2c20 4461 76c3  yo, Javier, Dav.
+00001860: b32c 2044 6176 6964 2c20 4661 7169 722d  ., David, Faqir-
+00001870: 5268 617a 6f75 692c 2059 6f75 7373 6566  Rhazoui, Youssef
+00001880: 2c20 2620 4d61 7274 c3ad 6e65 7a20 5669  , & Mart..nez Vi
+00001890: 6365 6e74 652c 2045 6c65 6e61 2e20 2832  cente, Elena. (2
+000018a0: 3032 3329 2e20 4441 4f20 416e 616c 797a  023). DAO Analyz
+000018b0: 6572 2e20 5a65 6e6f 646f 2e20 6874 7470  er. Zenodo. http
+000018c0: 733a 2f2f 646f 692e 6f72 672f 3130 2e35  s://doi.org/10.5
+000018d0: 3238 312f 7a65 6e6f 646f 2e37 3636 3936  281/zenodo.76696
+000018e0: 3839 0a0a                                89..
```

### Comparing `dao-scripts-1.2.2/dao_scripts.egg-info/SOURCES.txt` & `dao_scripts-1.3.0/dao_scripts.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .envrc
 .gitignore
 CHANGELOG.md
+LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/ci.yml
 .github/workflows/update-datasets.yml
 dao_scripts.egg-info/PKG-INFO
@@ -16,26 +17,26 @@
 dao_scripts.egg-info/top_level.txt
 src/__init__.py
 src/__main__.py
 src/_version.py
 src/argparser.py
 src/config.py
 src/endpoints.json
+src/logging.py
 src/main.py
 src/metadata.py
 src/aragon/__init__.py
 src/aragon/dao_names.json
 src/aragon/runner.py
 src/common/__init__.py
 src/common/api_requester.py
 src/common/blockscout.py
 src/common/common.py
 src/common/cryptocompare.py
-src/common/graphql.py
+src/common/thegraph.py
 src/daohaus/__init__.py
 src/daohaus/runner.py
 src/daostack/__init__.py
 src/daostack/runner.py
 src/utils/__init__.py
 src/utils/uploadDataWarehouse.py
-test/test_placeholder.py
-test/daohaus/test_verify_daohaus_collectors.py
+test/test_placeholder.py
```

### Comparing `dao-scripts-1.2.2/setup.cfg` & `dao_scripts-1.3.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 	Changelog = https://github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Sociology
 	Typing :: Typed
 	Topic :: Utilities
 
 [options]
-python_requires = >= 3.8
+python_requires = >= 3.9
 install_requires = 
+	dynaconf >= 3.0.0
 	gql >= 3.0.0a1
 	numpy >= 1.17.3
 	pandas >= 1.3.4
 	portalocker >= 2.3.2
 	pyarrow >= 6.0.0
 	requests >= 2.26.0
 	requests-cache >= 0.8.1
@@ -81,15 +82,15 @@
 	__pycache__,
 	.*,
 	dist
 max-complexity = 10
 max-line-length = 100
 
 [tox:tox]
-envlist = py{38,39,310,311}
+envlist = py{39,310,311,312}
 
 [testenv]
 deps = .[dev]
 wheel_build_env = build
 commands = 
 	pytest
```

### Comparing `dao-scripts-1.2.2/setup.py` & `dao_scripts-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.2.2/src/aragon/dao_names.json` & `dao_scripts-1.3.0/src/aragon/dao_names.json`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.2.2/src/aragon/runner.py` & `dao_scripts-1.3.0/src/aragon/runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 from gql.dsl import DSLField
 import pandas as pd
 import numpy as np
 import json
 
 from ..aragon import __name__ as aragon_module_name
 from ..common.cryptocompare import CCPricesCollector
-from ..common import ENDPOINTS, Collector
-from ..common.graphql import GraphQLCollector, GraphQLRunner
+from ..common import ENDPOINTS, Collector, NetworkRunner
+from ..common.thegraph import TheGraphCollector
 from ..common.blockscout import BlockscoutBallancesCollector
 
-class AppsCollector(GraphQLCollector):
+class AppsCollector(TheGraphCollector):
     def __init__(self, runner, network: str):
-        super().__init__('apps', runner, endpoint=ENDPOINTS[network]['aragon'], network=network)
+        super().__init__('apps', network, ENDPOINTS[network]['aragon'], runner)
 
     def query(self, **kwargs) -> DSLField:
         ds = self.schema
         return ds.Query.apps(**kwargs).select(
             ds.App.id,
             ds.App.isForwarder,
             ds.App.isUpgradeable,
@@ -35,17 +35,17 @@
             ds.App.organization.select(ds.Organization.id)
         )
 
 class BalancesCollector(BlockscoutBallancesCollector):
     def __init__(self, runner, base, network: str):
         super().__init__(runner, addr_key='recoveryVault', base=base, network=network)
 
-class CastsCollector(GraphQLCollector):
+class CastsCollector(TheGraphCollector):
     def __init__(self, runner, network: str):
-        super().__init__('casts', runner, endpoint=ENDPOINTS[network]['aragon_voting'], network=network, pbar_enabled=False)
+        super().__init__('casts', network, ENDPOINTS[network]['aragon_voting'], runner, pbar_enabled=False)
 
         @self.postprocessor
         def changeColumnNames(df: pd.DataFrame) -> pd.DataFrame:
             df = df.rename(columns={
                 'voterId':'voter', 
                 'voteAppAddress':'appAddress',
                 'voteOrgAddress':'orgAddress'})
@@ -62,19 +62,19 @@
             ds.Cast.vote.select(
                 ds.Vote.id,
                 ds.Vote.orgAddress,
                 ds.Vote.appAddress
             )
         )
 
-class OrganizationsCollector(GraphQLCollector):
+class OrganizationsCollector(TheGraphCollector):
     DAO_NAMES=pkgutil.get_data(aragon_module_name, 'dao_names.json')
 
     def __init__(self, runner, network: str):
-        super().__init__('organizations', runner, endpoint=ENDPOINTS[network]['aragon'], network=network)
+        super().__init__('organizations', network, ENDPOINTS[network]['aragon'], runner)
 
         @self.postprocessor
         def set_dead_recoveryVault(df: pd.DataFrame) -> pd.DataFrame:
             if df.empty: return df
 
             df['recoveryVault'] = df['recoveryVault'].replace(r'^0x0+$', np.NaN, regex=True)
             return df
@@ -109,17 +109,17 @@
         ds = self.schema
         return ds.Query.organizations(**kwargs).select(
             ds.Organization.id,
             ds.Organization.createdAt,
             ds.Organization.recoveryVault
         )
 
-class MiniMeTokensCollector(GraphQLCollector):
+class MiniMeTokensCollector(TheGraphCollector):
     def __init__(self, runner, network: str):
-        super().__init__('miniMeTokens', runner, endpoint=ENDPOINTS[network]['aragon_tokens'], network=network, pbar_enabled=False)
+        super().__init__('miniMeTokens', network, ENDPOINTS[network]['aragon_tokens'], runner, pbar_enabled=False)
 
     def query(self, **kwargs) -> DSLField:
         ds = self.schema
         return ds.Query.miniMeTokens(**kwargs).select(
             ds.MiniMeToken.id,
             ds.MiniMeToken.address,
             ds.MiniMeToken.totalSupply,
@@ -127,17 +127,17 @@
             ds.MiniMeToken.name,
             ds.MiniMeToken.symbol,
             ds.MiniMeToken.orgAddress,
             ds.MiniMeToken.appAddress,
             ds.MiniMeToken.lastUpdateAt
         )
 
-class TokenHoldersCollector(GraphQLCollector):
-    def __init__(self, runner: GraphQLRunner, network: str):
-        super().__init__('tokenHolders', runner, endpoint=ENDPOINTS[network]['aragon_tokens'], network=network)
+class TokenHoldersCollector(TheGraphCollector):
+    def __init__(self, runner: NetworkRunner, network: str):
+        super().__init__('tokenHolders', network, ENDPOINTS[network]['aragon_tokens'], runner)
 
         @self.postprocessor
         def add_minitokens(df: pd.DataFrame) -> pd.DataFrame:
             if df.empty: return df
 
             tokens = runner.filterCollector(name='miniMeTokens', network=network).df
             tokens = tokens.rename(columns={'address':'tokenAddress', 'orgAddress':'organizationAddress'})
@@ -152,31 +152,31 @@
             ds.TokenHolder.lastUpdateAt,
             ds.TokenHolder.balance
         )
 
 class TokenPricesCollector(CCPricesCollector):
     pass
 
-class ReposCollector(GraphQLCollector):
+class ReposCollector(TheGraphCollector):
     def __init__(self, runner, network: str):
-        super().__init__('repos', runner, network=network, endpoint=ENDPOINTS[network]['aragon'])
+        super().__init__('repos', network, ENDPOINTS[network]['aragon'], runner)
 
     def query(self, **kwargs) -> DSLField:
         ds = self.schema
         return ds.Query.repos(**kwargs).select(
             ds.Repo.id,
             ds.Repo.address,
             ds.Repo.name,
             ds.Repo.node,
             ds.Repo.appCount
         )
 
-class TransactionsCollector(GraphQLCollector):
+class TransactionsCollector(TheGraphCollector):
     def __init__(self, runner, network: str):
-        super().__init__('transactions', runner, network=network, endpoint=ENDPOINTS[network]['aragon_finance'])
+        super().__init__('transactions', network, ENDPOINTS[network]['aragon_finance'], runner)
 
     def query(self, **kwargs) -> DSLField:
         ds = self.schema
         return ds.Query.transactions(**kwargs).select(
             ds.Transaction.id,
             ds.Transaction.orgAddress,
             ds.Transaction.appAddress,
@@ -184,17 +184,17 @@
             ds.Transaction.entity,
             ds.Transaction.isIncoming,
             ds.Transaction.amount,
             ds.Transaction.date,
             ds.Transaction.reference
         )
 
-class VotesCollector(GraphQLCollector):
+class VotesCollector(TheGraphCollector):
     def __init__(self, runner, network: str):
-        super().__init__('votes', runner, network=network, endpoint=ENDPOINTS[network]['aragon_voting'])
+        super().__init__('votes', network, ENDPOINTS[network]['aragon_voting'], runner)
 
     def query(self, **kwargs) -> DSLField:
         ds = self.schema
         return ds.Query.votes(**kwargs).select(
             ds.Vote.id,
             ds.Vote.orgAddress,
             ds.Vote.appAddress,
@@ -210,35 +210,32 @@
             ds.Vote.nay,
             ds.Vote.voteNum,
             ds.Vote.votingPower,
             # Textual information
             ds.Vote.metadata,
         )
 
-class AragonRunner(GraphQLRunner):
+class AragonRunner(NetworkRunner):
     name: str = 'aragon'
 
     def __init__(self, dw=None):
         super().__init__(dw)
         self._collectors: List[Collector] = []
-        ## TODO: Fix aragon-tokens xdai subgraph and redeploy
-        self.networks = ['mainnet']
 
         for n in self.networks: 
             self._collectors.extend([
                 AppsCollector(self, n),
                 CastsCollector(self, n),
                 MiniMeTokensCollector(self, n),
                 ReposCollector(self, n),
                 TransactionsCollector(self, n),
                 TokenHoldersCollector(self, n),
-                VotesCollector(self, n)
+                VotesCollector(self, n),
+                oc := OrganizationsCollector(self, n),
+                BalancesCollector(self, oc, n),
             ])
-            oc = OrganizationsCollector(self, n)
-            bc = BalancesCollector(self, oc, n)
-            self._collectors += [oc, bc]
         
         self._collectors.append(CCPricesCollector(self))
 
     @property
     def collectors(self) -> List[Collector]:
         return self._collectors
```

### Comparing `dao-scripts-1.2.2/src/argparser.py` & `dao_scripts-1.3.0/src/argparser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from argparse import ArgumentParser, BooleanOptionalAction, SUPPRESS
 from typing import List
 
 from datetime import datetime
 import pathlib
-import os
 
 from . import config
 
 class CacheScriptsArgParser(ArgumentParser):
     def __init__(self, available_platforms: List[str], available_networks: List[str]):
         super().__init__(description="Main script to populate dao-analyzer cache")
 
@@ -22,39 +21,34 @@
             choices=available_platforms,
             nargs='*',
             type=str,
             default=available_platforms,
             help="The platforms to update. Every platform is updated by default."
         )
         self.add_argument(
-            "--ignore-errors",
-            default=True,
+            "--raise-runner-errors",
+            default=False,
             action=BooleanOptionalAction,
             help="Whether to ignore errors and continue")
         self.add_argument(
             "-d", "--debug",
-            action='store_true', default=False,
+            dest="DEBUG", action='store_true', default=False,
             help="Shows debug info"
         )
         self.add_argument(
             "-f", "--force",
             action='store_true', default=False,
             help="Removes the cache before updating"
         )
         self.add_argument(
             "-F", "--delete-force",
             action="store_true", default=False,
             help="Removes the datawarehouse folder before doing anything"
         )
         self.add_argument(
-            "--skip-daohaus-names",
-            action="store_true", default=False,
-            help="Skips the step of getting Daohaus Moloch's names, which takes some time"
-        )
-        self.add_argument(
             "--skip-token-balances",
             action="store_true", default=False,
             help="Skips the step of getting every DAO token balances, which takes some time"
         )
         self.add_argument(
             "-n", "--networks",
             nargs="+",
@@ -66,40 +60,41 @@
         self.add_argument(
             "-c", "--collectors",
             nargs="+",
             required=False,
             help="Collectors to run. For example: aragon/casts"
         )
         self.add_argument(
-            "--block-datetime",
+            "-B", "--block-datetime",
             required=False,
             type=datetime.fromisoformat,
             help="Get data up to a block datetime (input in ISO format)"
         )
         self.add_argument(
             "-D", "--datawarehouse",
             help="Specifies the destination folder of the datawarehouse",
             required=False,
             type=pathlib.Path,
             default=config.DEFAULT_DATAWAREHOUSE
         )
         self.add_argument(
-            "--cc-api-key",
-            help="Set the CryptoCompare API key (overrides environment variable)",
-            required=False,
-            type=str,
-            default=os.getenv('DAOA_CC_API_KEY')
-        )
-        self.add_argument(
             "--only-updatable",
+            dest='run_only_updatable',
             help=SUPPRESS, # "Run only updatable collectors (only for testing)",
             action='store_true',
             required=False,
             default=False
         )
         self.add_argument(
             "--daostack-all",
             help="Obtain all DAOs in DAOstack, not only registered ones",
-            action='store_true',
+            action='store_false',
             required=False,
-            default=False,
+            # For the user is "daostack_all", for us is "registered only"
+            dest='daostack__registered_only',
+            default=True,
+        )
+        self.add_argument(
+            "--daohaus-skip-names",
+            action="store_true", default=False, dest='daohaus__skip_names',
+            help="Skips the step of getting Daohaus Moloch's names, which takes some time"
         )
```

### Comparing `dao-scripts-1.2.2/src/common/api_requester.py` & `dao_scripts-1.3.0/src/common/api_requester.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import re
 import requests
 from functools import partial
 
 import logging
 import sys
 from tqdm import tqdm
-from typing import Dict, List, Union, Iterable
+from typing import Optional, Union, Iterable, Callable
 
 class GQLQueryException(Exception):
     def __init__(self, errors, msg="Errors in GraphQL Query"):
         super().__init__(msg)
         self.__errors = errors
 
     def errorsString(self) -> str:
@@ -80,60 +80,61 @@
 class GQLRequester:
     ELEMS_PER_CHUNK: int = 1000
 
     def __init__(self, endpoint: str, pbar_enabled: bool=True, introspection=True) -> None:
         self.__transport = RequestsHTTPTransport(endpoint)
         self.__client: Client = Client(transport=self.__transport, fetch_schema_from_transport=introspection)
         self.pbar = IndexProgressBar if pbar_enabled else RequestProgressSpinner
+        self.logger = logging.getLogger('dao-scripts.gql-requester')
 
-        logging.debug(f"Invoked ApiRequester with endpoint: {endpoint}")
+        self.logger.debug(f"Invoked ApiRequester with endpoint: {endpoint}")
 
     def get_schema(self) -> DSLSchema:
         with self.__client:
             assert(self.__client.schema is not None)
             return DSLSchema(self.__client.schema)
 
-    def request(self, query: Union[DSLQuery, DSLField, str]) -> Dict:
+    def request(self, query: Union[DSLQuery, DSLField, str]) -> dict:
         """
         Requests data from endpoint.
         """
         if isinstance(query, DSLField):
             query = DSLQuery(query)
 
-        logging.debug(f"Requesting: {query}")
+        self.logger.debug(f"Requesting: {query}")
 
         if isinstance(query, DSLQuery):
             result = self.__client.execute(dsl_gql(query))
         else:
             result = self.__client.execute(gql(query))
         
         if "errors" in result:
             raise GQLQueryException(result["errors"])
 
         return result
 
-    def request_single(self, q: Union[DSLQuery, DSLField, str]) -> Dict:
+    def request_single(self, q: Union[DSLQuery, DSLField, str]) -> dict:
         result = self.request(q)
         if result and len(result.values()) == 1:
             return next(iter(result.values()))
         else:
             raise 
 
-    def n_requests(self, query:DSLType, index='id', last_index: str = "", block_hash: str = None) -> List[Dict]:
+    def n_requests(self, query: Callable[..., DSLField], index='id', last_index: str = "", block_hash: Optional[str] = None) -> list[dict]:
         """
         Requests all chunks from endpoint.
 
         Parameters:
             * query: json to request
             * index: dict key to use as index
             * last_index: used to continue the request
             * block_hash: make the request to that block hash
         """
-        elements: List[Dict] = list()
-        result = Dict
+        elements: list[dict] = list()
+        result = dict()
         
         # do-while structure
         exit: bool = False
 
         with self.pbar() as pbar:
             while not exit:
                 query_args = {
@@ -167,26 +168,26 @@
 
     def __str__(self):
         return super().__str__() + ":\n" + self.errorsString()
 
 class CryptoCompareRequester:
     BASEURL = 'https://min-api.cryptocompare.com/data/'
 
-    def __init__(self, api_key: str = None, pbar_enabled: bool = True):
-        self.logger = logging.getLogger('ccrequester')
+    def __init__(self, api_key: Optional[str] = None, pbar_enabled: bool = True):
+        self.logger = logging.getLogger('dao-scripts.ccrequester')
         self.pbar = partial(tqdm, delay=1, file=sys.stdout, desc="Requesting",
             dynamic_ncols=True)
         
         if not api_key:
-            logging.warning(f'Invalid api key: {api_key}')
+            self.logger.warning('CryptoCompare API key is not set')
             api_key = ""
 
         self.api_key = api_key
 
-    def _build_headers(self) -> Dict[str, str]:
+    def _build_headers(self) -> dict[str, str]:
         return {
           'Authorization': 'Apikey ' + self.api_key
         }
 
     def _request(self, url: str, params=None):
         if params is None:
             params = {}
@@ -200,15 +201,15 @@
         # - "Complex" ones which have Response, Message, Type, etc fields
         # - "Simple" ones where the data is the response per se
         if r.ok:
             j = r.json()
             if 'Data' not in j:
                 return j
             if "HasWarning" in j and j["HasWarning"]:
-                logging.warning("Warning in query", r.url, ":", j["Message"])
+                self.logger.warning("Warning in query", r.url, ":", j["Message"])
             if j["Type"] == 100:
                 return j['Data']
         
         raise CryptoCompareQueryException(j["Message"])
     
     def get_available_coin_list(self):
         return self._request(self.BASEURL + 'blockchain/list').values()
```

### Comparing `dao-scripts-1.2.2/src/common/blockscout.py` & `dao_scripts-1.3.0/src/common/blockscout.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import pandas as pd
 import requests
-import logging
 from functools import partial
 from tqdm import tqdm
 from time import sleep
-from typing import Union
+from typing import Union, Optional
 
 import numpy as np
 
 from ..metadata import Block
 from .. import config
 
 from . import ENDPOINTS
 from .common import NetworkCollector, solve_decimals
 from .cryptocompare import cc_postprocessor
-from .graphql import GraphQLCollector
 
 MSG_NO_TOKENS_FOUND = "No tokens found"
 
 class BlockscoutBallancesCollector(NetworkCollector):
     ERR_SLEEP = 60
 
-    def __init__(self, runner, base: GraphQLCollector, name: str='tokenBalances', network: str='mainnet', addr_key: str='id'):
+    def __init__(self, runner, base: NetworkCollector, name: str='tokenBalances', network: str='mainnet', addr_key: str='id'):
         """ Initializes a ballance collector that uses blockscout
         
         Parameters:
             name (str): The name of the collector (and filename)
             runner (Runner): The runner in which it's based
             network (str): The network to run on
             base (GraphQLCollector): The DAOs/organizations collector to get the DAO list from
@@ -33,24 +31,24 @@
         """
         super().__init__(name, runner, network)
         self.base = base
         self.addr_key = addr_key
 
     def verify(self) -> bool:
         if config.skip_token_balances:
-            logging.warning('Skipping token balances because --skip-token-balances flag was set')
+            self.logger.warning('Skipping token balances because --skip-token-balances flag was set')
             return False
         else:
             return super().verify()
 
     @property
     def endpoint(self) -> str:
         return ENDPOINTS[self.network]['blockscout']
 
-    def _get_from_address(self, addr: str, retry: int = 0, maxretries: int = 3, block: Union[int, Block] = None, ignore_errors=False) -> pd.DataFrame: # noqa: C901
+    def _get_from_address(self, addr: str, retry: int = 0, maxretries: int = 3, block: Union[int, Block, None] = None, ignore_errors=False) -> pd.DataFrame: # noqa: C901
         if retry >= maxretries:
             raise ValueError(f"Too many retries {retry}/{maxretries}")
 
         blockn = block
         if blockn is None:
             blockn = 'latest'
         elif isinstance(blockn, Block):
@@ -79,40 +77,40 @@
                 df['address'] = addr
                 df['network'] = self.network
                 df['id'] = 'token-' + df['contractAddress'] + '-org-' + df['address']
                 return df
             elif j['message'] == MSG_NO_TOKENS_FOUND:
                 return pd.DataFrame()
             else:
-                logging.warning(f"Status {j['status']}, message: {j['message']}")
+                self.logger.warning(f"Status {j['status']}, message: {j['message']}")
                 return pd.DataFrame()
         elif r.status_code == 429: # Too many requests
-            logging.warning(f"Too many requests, sleep and retry {retry}/{maxretries} time")
+            self.logger.warning(f"Too many requests, sleep and retry {retry}/{maxretries} time")
             sleep(self.ERR_SLEEP)
             return self._get_from_address(addr, retry=retry+1, maxretries=maxretries)
         elif r.status_code == 503:
-            logging.warning(f"Service unavailable, sleep and retry {retry}/{maxretries} time")
+            self.logger.warning(f"Service unavailable, sleep and retry {retry}/{maxretries} time")
             sleep(self.ERR_SLEEP)
             return self._get_from_address(addr, retry=retry+1, maxretries=maxretries)
         elif r.status_code == 504: # Gateway Time-out (Response too large)
-            logging.warning(f"Requests returned Gateway Time-out, ignoring response for addr {addr}")
+            self.logger.warning(f"Requests returned Gateway Time-out, ignoring response for addr {addr}")
             return pd.DataFrame() 
         else:
-            logging.error(f'Requests failed for address "{addr}" with status code {r.status_code}: {r.reason}')
+            self.logger.error(f'Requests failed for address "{addr}" with status code {r.status_code}: {r.reason}')
             if ignore_errors:
                 return pd.DataFrame()
             else:
                 raise ValueError(f"Requests failed for address {addr[:12]}... with status code {r.status_code}: {r.reason}")
 
-    def run(self, force=False, block: Block = None, prev_block: Block = None, **kwargs):
+    def run(self, force=False, block: Optional[Block] = None, prev_block: Optional[Block] = None, **kwargs):
         # For each of the DAOs in the df, get the token balance
         addresses = self.base.df[self.addr_key].drop_duplicates()
 
         if addresses.empty:
-            logging.warning("No addresses returned, not running blockscout collector")
+            self.logger.warning("No addresses returned, not running blockscout collector")
             return
 
         ptqdm = partial(tqdm, delay=1, desc="Requesting token balances", 
             unit='req', dynamic_ncols=True)
         toApply = partial(self._get_from_address, block=block, ignore_errors=True)
         df = pd.concat(map(toApply, ptqdm(addresses)), ignore_index=True)
```

### Comparing `dao-scripts-1.2.2/src/common/common.py` & `dao_scripts-1.3.0/src/common/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import List, Dict, Iterable
+from typing import Optional, Iterable
 import logging
 import sys
 import json
 from datetime import datetime, timezone
 import traceback
 import pkgutil
 
@@ -15,15 +15,32 @@
 
 from .api_requester import GQLRequester
 from ..metadata import RunnerMetadata, Block
 from .. import config
 from dao_analyzer import cache_scripts
 
 # To be able to obtain endpoints.json
-ENDPOINTS: Dict = json.loads(pkgutil.get_data(cache_scripts.__name__, 'endpoints.json'))
+ENDPOINTS: dict = json.loads(pkgutil.get_data(cache_scripts.__name__, 'endpoints.json'))
+THE_GRAPH_URL_TEMPLATE = 'https://gateway-arbitrum.network.thegraph.com/api/{api_key}/subgraphs/id/{subgraph_id}'
+THE_GRAPH_DEPLOYMENT_TEMPLATE = 'https://gateway-arbitrum.network.thegraph.com/api/{api_key}/deployments/id/{deployment_id}'
+
+def get_graph_url(subgraph_id: str) -> str:
+    if subgraph_id.startswith("http"):
+        return subgraph_id
+
+    if subgraph_id.startswith("Qm"):
+        return THE_GRAPH_DEPLOYMENT_TEMPLATE.format(
+            api_key=config.THE_GRAPH_API_KEY,
+            deployment_id=subgraph_id,
+        )
+
+    return THE_GRAPH_URL_TEMPLATE.format(
+        api_key=config.THE_GRAPH_API_KEY,
+        subgraph_id=subgraph_id,
+    )
 
 def solve_decimals(df: pd.DataFrame) -> pd.DataFrame:
     """ Adds the balanceFloat column to the dataframe
 
     This column is a precalculated value of tokenBalance / 10 ** tokenDecimals as float
     """
     dkey, bkey, fkey = 'decimals', 'balance', 'balanceFloat'
@@ -37,14 +54,18 @@
     INDEX = ['network', 'id']
     
     def __init__(self, name:str, runner: 'Runner'):
         self.name: str = name
         self.runner = runner
 
     @property
+    def logger(self):
+        return logging.getLogger(f'dao_analyzer.collectors.{self.collectorid}')
+
+    @property
     def data_path(self) -> Path:
         return self.runner.basedir / (self.name + '.arr')
 
     @property
     def long_name(self) -> str:
         return f"{self.runner.name}/{self.name}"
 
@@ -63,15 +84,15 @@
         """
         return True
 
     def _update_data(self, df: pd.DataFrame, force: bool = False) -> pd.DataFrame:
         """ Updates the dataframe in `self.data_path` with the new data.
         """
         if df.empty:
-            logging.warning("Empty dataframe, not updating file")
+            self.logger.warning("Empty dataframe, not updating file")
             return
 
         if not self.data_path.is_file():
             df.reset_index(drop=True).to_feather(self.data_path)
             return
 
         prev_df: pd.DataFrame = pd.read_feather(self.data_path)
@@ -102,127 +123,128 @@
     def collectorid(self) -> str:
         return '-'.join([super().collectorid, self.network])
 
 class UpdatableCollector(Collector): # Flag class
     pass
 
 class Runner(ABC):
-    def __init__(self, dw: Path = Path()):
+    def __init__(self, dw: Path):
         self.__dw: Path = dw
 
-    def set_dw(self, dw) -> Path:
-        self.__dw = dw
+    @property
+    def logger(self):
+        return logging.getLogger(f'dao_analyzer.runner.{self.name}')
 
     @property
     def cache(self) -> Path:
         # Common cache folder for everyone
         return self.__dw / '.cache'
 
     @property
     def basedir(self) -> Path:
         return self.__dw / self.name
 
     @property
-    def collectors(self) -> List[Collector]:
+    def collectors(self) -> list[Collector]:
         return []
 
     def run(self, **kwargs):
         raise NotImplementedError
 
 class NetworkRunner(Runner, ABC):
-    def __init__(self, dw = None):
+    def __init__(self, dw):
         super().__init__(dw)
         self.networks = {n for n,v in ENDPOINTS.items() if self.name in v and not n.startswith('_')}
 
     def filterCollectors(self, 
         networks: Iterable[str] = [],
         names: Iterable[str] = [],
         long_names: Iterable[str] = []
     ) -> Iterable[Collector]:
-        result = self.collectors
+        result: Iterable[Collector] = self.collectors
 
-        if config.only_updatable:
+        if config.run_only_updatable:
             result = filter(lambda c: isinstance(c, UpdatableCollector), result)
 
         # networks ^ (names v long_names)
         if networks:
             # GraphQLCollector => c.network in networks
             # a => b : not(a) or b
             result = filter(lambda c: not isinstance(c, NetworkCollector) or c.network in networks, result)
 
         if names or long_names:
             result = (c for c in result if c.name in names or c.long_name in long_names)
 
         return result
 
     def filterCollector(self,
-        collector_id: str = None,
-        network: str = None,
-        name: str = None,
-        long_name: str = None,
-    ) -> Collector:
+        collector_id: Optional[str] = None,
+        network: Optional[str] = None,
+        name: Optional[str] = None,
+        long_name: Optional[str] = None,
+    ) -> Optional[Collector]:
         if collector_id:
             return next((c for c in self.collectors if c.collectorid == collector_id), None)
 
         return next(self.filterCollectors(
             networks=[network] if network else [],
             names=[name] if name else [],
             long_names=[long_name] if long_name else []
         ), None)
 
-    @staticmethod
     @retry(retry=retry_if_exception_type(TransportQueryError), wait=wait_exponential(max=10), stop=stop_after_attempt(3))
-    def validated_block(network: str, prev_block: Block = None) -> Block:
-        requester = GQLRequester(ENDPOINTS[network]["_blocks"])
+    def validated_block(self, network: str, prev_block: Optional[Block] = None, until_date: Optional[datetime] = None) -> Optional[Block]:
+        requester = GQLRequester(get_graph_url(ENDPOINTS[network]['_blocks']))
         ds = requester.get_schema()
 
         number_gte = prev_block.number if prev_block else 0
         
         args = {
             "first": 1,
             "skip": config.SKIP_INVALID_BLOCKS,
             "orderBy": "number",
             "orderDirection": "desc",
             "where": {
                 "number_gte": number_gte
             }
         }
 
-        if config.block_datetime:
+        # TODO: SET THE UNTIL_DATE
+        if until_date:
             del args["skip"]
             del args["where"]["number_gte"]
-            args["where"]["timestamp_lte"] = int(config.block_datetime.timestamp())
+            args["where"]["timestamp_lte"] = int(until_date.timestamp())
 
         response = requester.request(ds.Query.blocks(**args).select(
             ds.Block.id,
             ds.Block.number,
             ds.Block.timestamp
         ))["blocks"]
     
         if len(response) == 0:
-            logging.warning(f"Blocks query returned no response with args {args}")
+            self.logger.warning(f"Blocks query returned no response with args {args}")
             return prev_block
 
         return Block(response[0])
 
     @staticmethod
-    def _verifyCollectors(tocheck: Iterable[Collector]):
+    def _verifyCollectors(tocheck: Iterable[Collector]) -> Iterable[Collector]:
         verified = []
         for c in tqdm(list(tocheck), desc="Verifying"):
             try:
                 if c.verify():
                     verified.append(c)
                 else:
                     print(f"Verified returned false for {c.collectorid} (view logs the see why)")
             except Exception:
                 print(f"Won't run {c.collectorid}", file=sys.stderr)
                 traceback.print_exc()
         return verified
 
-    def run(self, networks: List[str] = [], force=False, collectors=None):
+    def run(self, networks: list[str] = [], force=False, collectors=None, until_date: Optional[datetime]=None):
         self.basedir.mkdir(parents=True, exist_ok=True)
 
         print("Verifying collectors")
         verified = self._verifyCollectors(self.filterCollectors(
             networks=networks,
             long_names=collectors
         ))
@@ -235,22 +257,26 @@
             blocks: dict[str, Block] = {}
             for c in verified:
                 try:
                     if isinstance(c, NetworkCollector):
                         if c.network not in blocks:
                             # Getting a block more recent than the one in the metadata (just to narrow down the search)
                             print("Requesting a block number...", end='\r')
-                            blocks[c.network] = self.validated_block(c.network, None if force else metadata[c.collectorid].block)
+                            blocks[c.network] = self.validated_block(
+                                network=c.network, 
+                                prev_block=None if force else metadata[c.collectorid].block,
+                                until_date=until_date,
+                            )
                             print(f"Using block {blocks[c.network].id} for {c.network} (ts: {blocks[c.network].timestamp.isoformat()})")
 
                         print(f"Running collector {c.long_name} ({c.network})")
                         olderBlock = blocks[c.network] < metadata[c.collectorid].block
                         if not force and olderBlock:
                             print("Warning: Forcing because requesting an older block")
-                            logging.warning("Forcing because using an older block")
+                            self.logger.warning("Forcing because using an older block")
 
                         # Running the collector
                         c.run(
                             force=force or olderBlock, 
                             block=blocks[c.network],
                             prev_block=metadata[c.collectorid].block,
                         )
@@ -262,12 +288,13 @@
                         c.run(
                             force=force,
                         )
 
                     metadata[c.collectorid].last_update = datetime.now(timezone.utc)
                 except Exception as e:
                     metadata.errors[c.collectorid] = e.__str__()
-                    if config.ignore_errors:
-                        print(traceback.format_exc())
-                    else:
+                    if config.raise_runner_errors:
                         raise e
+                    else:
+                        # TODO: Use a logger instead
+                        print(traceback.format_exc(), file=sys.stderr)
             print(f'--- {self.name}\'s datawarehouse updated ---')
```

### Comparing `dao-scripts-1.2.2/src/common/cryptocompare.py` & `dao_scripts-1.3.0/src/common/cryptocompare.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from .common import Collector, NetworkRunner
 
 import logging
 
 EMPTY_KEY_MSG = \
 """\
 Empty CryptoCompare API key. You can obtain one from https://www.cryptocompare.com/cryptopian/api-keys
-You can set the API key using --cc-api-key argument or the DAOA_CC_API_KEY env variable.
+You can set the API key using the DAOA_CC_API_KEY env variable.
 """
 
 def cc_postprocessor(df: pd.DataFrame) -> pd.DataFrame:
-    ccrequester = CryptoCompareRequester(api_key=config.cc_api_key)
+    ccrequester = CryptoCompareRequester(api_key=config.CC_API_KEY)
 
     tokenSymbols = df['symbol'].drop_duplicates()
 
     # TODO: Get only the ones with available symbols (relaxedValidation=False)
     df_fiat = pd.DataFrame.from_dict(ccrequester.get_symbols_price(tokenSymbols, relaxedValidation=True), orient='index')
 
     def _apply_values(row):
@@ -37,19 +37,19 @@
     df = df.apply(_apply_values, axis='columns')
 
     return df
 
 class CCPricesCollector(Collector):
     def __init__(self, runner: NetworkRunner, name: str='tokenPrices'):
         super().__init__(name, runner)
-        self.requester = CryptoCompareRequester(api_key=config.cc_api_key)
+        self.requester = CryptoCompareRequester(api_key=config.CC_API_KEY)
 
     def verify(self) -> bool:
         if not self.requester.api_key:
-            logging.warning(EMPTY_KEY_MSG)
+            self.logger.warning(EMPTY_KEY_MSG)
             return False
 
         return super().verify()
     
     @property
     def base(self):
         return self.runner.filterCollector(name='tokenBalances')
```

### Comparing `dao-scripts-1.2.2/src/daohaus/runner.py` & `dao_scripts-1.3.0/src/daohaus/runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 from tqdm import tqdm
 from gql.dsl import DSLField
 
 from .. import config
 from ..common.common import solve_decimals
 from ..common.cryptocompare import cc_postprocessor
 
-from ..common import ENDPOINTS, Collector
-from ..common.graphql import GraphQLCollector, GraphQLRunner, add_where
+from ..common import ENDPOINTS, Collector, NetworkRunner
+from ..common.thegraph import TheGraphCollector, add_where
 
 DATA_ENDPOINT: str = "https://data.daohaus.club/dao/{id}"
 
-class MembersCollector(GraphQLCollector):
+class MembersCollector(TheGraphCollector):
     def __init__(self, runner, network: str):
-        super().__init__('members', runner, network=network, endpoint=ENDPOINTS[network]['daohaus'])
+        super().__init__('members', network, ENDPOINTS[network]['daohaus'], runner)
 
     def query(self, **kwargs) -> DSLField:
         ds = self.schema
         return ds.Query.members(**kwargs).select(
             ds.Member.id,
             ds.Member.createdAt,
             ds.Member.molochAddress,
@@ -38,28 +38,28 @@
             ds.Member.shares,
             ds.Member.loot,
             ds.Member.exists,
             ds.Member.tokenTribute,
             ds.Member.didRagequit
         )
 
-class MolochesCollector(GraphQLCollector):
+class MolochesCollector(TheGraphCollector):
     def __init__(self, runner, network: str):
-        super().__init__('moloches', runner, network=network, endpoint=ENDPOINTS[network]['daohaus'])
+        super().__init__('moloches', network, ENDPOINTS[network]['daohaus'], runner)
 
         @self.postprocessor
         def moloch_id(df: pd.DataFrame) -> pd.DataFrame:
             df['molochAddress'] = df['id']
             return df
 
         @self.postprocessor
         def moloch_names(df: pd.DataFrame) -> pd.DataFrame:
             df = df.rename(columns={"title":"name"})
 
-            if config.skip_daohaus_names:
+            if config.daohaus.skip_names:
                 return df
 
             cached = requests_cache.CachedSession(self.runner.cache / 'daohaus_names_cache', 
                 use_cache_dir=False, 
                 expire_after=timedelta(days=30)
             )
             tqdm.pandas(desc="Getting moloch names")
@@ -88,17 +88,17 @@
             # ds.Moloch.timestamp, # Removed from daohaus-stats
             ds.Moloch.createdAt,
             ds.Moloch.totalShares,
             ds.Moloch.guildBankAddress,
             ds.Moloch.totalLoot,
         )
 
-class ProposalsCollector(GraphQLCollector):
+class ProposalsCollector(TheGraphCollector):
     def __init__(self, runner, network: str):
-        super().__init__('proposals', runner, network=network, endpoint=ENDPOINTS[network]["daohaus"])
+        super().__init__('proposals', network, ENDPOINTS[network]['daohaus'], runner)
 
     def query(self, **kwargs) -> DSLField:
         ds = self.schema
         return ds.Query.proposals(**kwargs).select(
             ds.Proposal.id,
             ds.Proposal.createdAt,
             ds.Proposal.proposalId,
@@ -119,32 +119,32 @@
             ds.Proposal.didPass,
             ds.Proposal.yesShares,
             ds.Proposal.noShares,
             # Textual information
             ds.Proposal.details,
         )
     
-class RageQuitCollector(GraphQLCollector):
+class RageQuitCollector(TheGraphCollector):
     def __init__(self, runner, network: str):
-        super().__init__('rageQuits', runner, network=network, endpoint=ENDPOINTS[network]["daohaus"])
+        super().__init__('rageQuits', network, ENDPOINTS[network]['daohaus'], runner)
 
     def query(self, **kwargs) -> DSLField:
         ds = self.schema
         return ds.Query.rageQuits(**kwargs).select(
             ds.RageQuit.id,
             ds.RageQuit.createdAt,
             ds.RageQuit.molochAddress,
             ds.RageQuit.memberAddress,
             ds.RageQuit.shares,
             ds.RageQuit.loot
         )
 
-class TokenBalancesCollector(GraphQLCollector):
+class TokenBalancesCollector(TheGraphCollector):
     def __init__(self, runner, network: str):
-        super().__init__('tokenBalances', runner, network=network, endpoint=ENDPOINTS[network]["daohaus"])
+        super().__init__('tokenBalances', network, ENDPOINTS[network]['daohaus'], runner)
 
         @self.postprocessor
         def change_col_names(df: pd.DataFrame) -> pd.DataFrame:
             return df.rename(columns={
                 'molochId': 'molochAddress',
                 'tokenTokenAddress': 'tokenAddress',
                 'tokenDecimals': 'decimals',
@@ -159,16 +159,16 @@
             df['bank'] = df[bank_idx].idxmax(1)
             df['bank'] = df['bank'].str.lower()
             df['bank'] = df['bank'].str.replace('bank', '')
             df = df.drop(columns=bank_idx)
         
             return df
         
-        self.postprocessors.append(solve_decimals)
-        self.postprocessors.append(cc_postprocessor)
+        self.postprocessor(solve_decimals)
+        self.postprocessor(cc_postprocessor)
 
     def query(self, **kwargs) -> DSLField:
         ds = self.schema
         return ds.Query.tokenBalances(**add_where(kwargs, guildBank=True, tokenBalance_gt=0)).select(
             ds.TokenBalance.id,
             ds.TokenBalance.moloch.select(
                 ds.Moloch.id
@@ -180,17 +180,17 @@
             ),
             ds.TokenBalance.guildBank,
             ds.TokenBalance.memberBank,
             ds.TokenBalance.ecrowBank,
             ds.TokenBalance.tokenBalance
         )
 
-class VoteCollector(GraphQLCollector):
+class VoteCollector(TheGraphCollector):
     def __init__(self, runner, network: str):
-        super().__init__('votes', runner, network=network, endpoint=ENDPOINTS[network]["daohaus"])
+        super().__init__('votes', network, ENDPOINTS[network]['daohaus'], runner)
 
         @self.postprocessor
         def changeColumnNames(df: pd.DataFrame) -> pd.DataFrame:
             return df.rename(columns={"proposalId":"proposalAddress"})
 
     def query(self, **kwargs) -> DSLField:
         ds = self.schema
@@ -200,19 +200,19 @@
             ds.Vote.proposal.select(ds.Proposal.id),
             ds.Vote.molochAddress,
             ds.Vote.memberAddress,
             ds.Vote.memberPower,
             ds.Vote.uintVote
         )
 
-class DaohausRunner(GraphQLRunner):
+class DaohausRunner(NetworkRunner):
     name: str = 'daohaus'
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, dw):
+        super().__init__(dw)
         self._collectors: List[Collector] = []
         for n in self.networks:
             self._collectors.extend([
                 MembersCollector(self, n),
                 MolochesCollector(self, n),
                 ProposalsCollector(self, n),
                 RageQuitCollector(self, n),
```

### Comparing `dao-scripts-1.2.2/src/daostack/runner.py` & `dao_scripts-1.3.0/src/daostack/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 import pandas as pd
 from gql.dsl import DSLField
 
 from .. import config
 from ..common.blockscout import BlockscoutBallancesCollector
 from ..common.cryptocompare import CCPricesCollector
 
-from ..common import ENDPOINTS, Collector
-from ..common.graphql import GraphQLCollector, GraphQLRunner, add_where
+from ..common import ENDPOINTS, Collector, NetworkRunner
+from ..common.thegraph import TheGraphCollector, add_where
 
 def _changeProposalColumnNames(df: pd.DataFrame) -> pd.DataFrame:
     df = df.rename(columns={
         'daoId': 'dao',
         'proposalId': 'proposal'
     })
     return df
@@ -34,17 +34,17 @@
     
     return _remove_phantom_daos
 
 class BalancesCollector(BlockscoutBallancesCollector):
     def __init__(self, runner, base, network: str):
         super().__init__(runner, base=base, network=network, addr_key='dao')
 
-class DaosCollector(GraphQLCollector):
+class DaosCollector(TheGraphCollector):
     def __init__(self, runner, network: str):
-        super().__init__('daos', runner, network=network, endpoint=ENDPOINTS[network]['daostack'])
+        super().__init__('daos', network, ENDPOINTS[network]['daostack'], runner)
         
         @self.postprocessor
         def changeColumnNames(df: pd.DataFrame) -> pd.DataFrame:
             df = df.rename(columns={
                 'nativeTokenId':'nativeToken',
                 'nativeReputationId':'nativeReputation'})
             return df
@@ -56,41 +56,41 @@
 
             df['dao'] = df['id']
             return df
 
     def query(self, **kwargs) -> DSLField:
         ds = self.schema
 
-        where = { 'register': 'registered' }
-        if config.daostack_all:
-            where.pop('register')
+        where = dict()
+        if config.daostack.registered_only:
+            where['register'] = 'registered'
         
         return ds.Query.daos(**add_where(kwargs, **where)).select(
             ds.DAO.id,
             ds.DAO.name,
             ds.DAO.register,
             ds.DAO.nativeToken.select(ds.Token.id),
             ds.DAO.nativeReputation.select(ds.Rep.id)
         )
 
-class ProposalsCollector(GraphQLCollector):
+class ProposalsCollector(TheGraphCollector):
     def __init__(self, runner, network: str, daoC: DaosCollector):
-        super().__init__('proposals', runner, network=network, endpoint=ENDPOINTS[network]['daostack'])
+        super().__init__('proposals', network, ENDPOINTS[network]['daostack'], runner)
 
         @self.postprocessor
         def changeColumnNames(df: pd.DataFrame) -> pd.DataFrame:
             return df.rename(columns={
                 'daoId': 'dao',
             }).rename(columns=self._stripGenesis)
 
         @self.postprocessor
         def deleteColums(df: pd.DataFrame) -> pd.DataFrame:
             return df.drop(columns=['competition'], errors='ignore')
 
-        self.postprocessors.append(_remove_phantom_daos_wr(daoC))
+        self.postprocessor(_remove_phantom_daos_wr(daoC))
 
     @staticmethod
     def _stripGenesis(s: str):
         tostrip='genesisProtocolParams'
 
         if s and len(s) > 1 and s.startswith(tostrip):
             s = s[len(tostrip):]
@@ -135,38 +135,36 @@
                 ds.GenesisProtocolParam.minimumDaoBounty,
                 ds.GenesisProtocolParam.daoBountyConst,
             ),
             ds.Proposal.dao.select(ds.DAO.id),
             ds.Proposal.competition.select(ds.CompetitionProposal.id)
         )
 
-class ReputationHoldersCollector(GraphQLCollector):
+class ReputationHoldersCollector(TheGraphCollector):
     def __init__(self, runner, network: str, daoC: DaosCollector):
-        super().__init__('reputationHolders', runner, network=network, endpoint=ENDPOINTS[network]['daostack'])
+        super().__init__('reputationHolders', network, ENDPOINTS[network]['daostack'], runner)
         self.postprocessor(_changeProposalColumnNames)
-
-        self.postprocessors.append(_remove_phantom_daos_wr(daoC))
+        self.postprocessor(_remove_phantom_daos_wr(daoC))
 
     def query(self, **kwargs) -> DSLField:
         ds = self.schema
         return ds.Query.reputationHolders(**kwargs).select(
             ds.ReputationHolder.id,
             ds.ReputationHolder.contract,
             ds.ReputationHolder.address,
             ds.ReputationHolder.balance,
             ds.ReputationHolder.createdAt,
             ds.ReputationHolder.dao.select(ds.DAO.id)
         )
 
-class StakesCollector(GraphQLCollector):
+class StakesCollector(TheGraphCollector):
     def __init__(self, runner, network: str, daoC: DaosCollector):
-        super().__init__('stakes', runner, network=network, endpoint=ENDPOINTS[network]['daostack'])
+        super().__init__('stakes',network, ENDPOINTS[network]['daostack'], runner)
         self.postprocessor(_changeProposalColumnNames)
-    
-        self.postprocessors.append(_remove_phantom_daos_wr(daoC))
+        self.postprocessor(_remove_phantom_daos_wr(daoC))
 
     def query(self, **kwargs) -> DSLField:
         ds = self.schema
         return ds.Query.proposalStakes(**kwargs).select(
             ds.ProposalStake.id,
             ds.ProposalStake.createdAt,
             ds.ProposalStake.staker,
@@ -175,36 +173,35 @@
             ds.ProposalStake.dao.select(ds.DAO.id),
             ds.ProposalStake.proposal.select(ds.Proposal.id)
         )
 
 class TokenPricesCollector(CCPricesCollector):
     pass
 
-class VotesCollector(GraphQLCollector):
+class VotesCollector(TheGraphCollector):
     def __init__(self, runner, network: str, daoC: DaosCollector):
-        super().__init__('votes', runner, network=network, endpoint=ENDPOINTS[network]['daostack'])
+        super().__init__('votes', network, ENDPOINTS[network]['daostack'], runner)
         self.postprocessor(_changeProposalColumnNames)
-
-        self.postprocessors.append(_remove_phantom_daos_wr(daoC))
+        self.postprocessor(_remove_phantom_daos_wr(daoC))
 
     def query(self, **kwargs) -> DSLField:
         ds = self.schema
         return ds.Query.proposalVotes(**kwargs).select(
             ds.ProposalVote.id,
             ds.ProposalVote.createdAt,
             ds.ProposalVote.voter,
             ds.ProposalVote.outcome,
             ds.ProposalVote.reputation,
             ds.ProposalVote.dao.select(ds.DAO.id),
             ds.ProposalVote.proposal.select(ds.Proposal.id)
         )
 
-class CommonRepEventCollector(GraphQLCollector):
+class CommonRepEventCollector(TheGraphCollector):
     def __init__(self, name, runner, base, network: str): 
-        super().__init__(name, runner, network=network, endpoint=ENDPOINTS[network]['daostack'])
+        super().__init__(name, network, ENDPOINTS[network]['daostack'], runner)
         self.base = base
 
         @self.postprocessor
         def add_dao_id(df: pd.DataFrame) -> pd.DataFrame:
             """ Using the contract info, appends the DAO id.
             Used by ReputationMintsCollector and ReputationBurnsCollector
             """
@@ -226,15 +223,15 @@
             )
 
             # Get only the dao field
             df = df[prev_cols + wants]
             
             return df
 
-        self.postprocessors.append(_remove_phantom_daos_wr(self.base))
+        self.postprocessor(_remove_phantom_daos_wr(self.base))
 
 class ReputationMintsCollector(CommonRepEventCollector):
     def __init__(self, *args, **kwargs):
         super().__init__('reputationMints', *args, **kwargs)
 
     def query(self, **kwargs) -> DSLField:
         ds = self.schema
@@ -258,19 +255,19 @@
             # ds.ReputationBurn.txHash, # Not used
             ds.ReputationBurn.contract,
             ds.ReputationBurn.address,
             ds.ReputationBurn.amount,
             ds.ReputationBurn.createdAt
         )
 
-class DaostackRunner(GraphQLRunner):
+class DaostackRunner(NetworkRunner):
     name: str = 'daostack'
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, dw):
+        super().__init__(dw)
         self._collectors: List[Collector] = []
         for n in self.networks:
             dc = DaosCollector(self, n)
 
             self._collectors.extend([
                 dc,
                 ProposalsCollector(self, n, dc),
```

### Comparing `dao-scripts-1.2.2/src/main.py` & `dao_scripts-1.3.0/src/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,157 +1,163 @@
 #!/usr/bin/env python3
-from typing import Dict
-
 from datetime import datetime
+import logging.handlers
 from pathlib import Path
 import portalocker as pl
 import os
 import tempfile
 import shutil
 import sys
 from sys import stderr
 
 import logging
-from logging.handlers import RotatingFileHandler
+
+from argparse import Namespace
 
 from .aragon.runner import AragonRunner
 from .daohaus.runner import DaohausRunner
 from .daostack.runner import DaostackRunner
-from .common import Runner, ENDPOINTS
+from .common import ENDPOINTS, NetworkRunner
 from .argparser import CacheScriptsArgParser
+from ._version import __version__
+from .logging import setup_logging, finish_logging
 from . import config
 
-LOG_FILE_FORMAT = "[%(levelname)s] - %(asctime)s - %(name)s - : %(message)s in %(pathname)s:%(lineno)d"
-LOG_STREAM_FORMAT = "%(levelname)s: %(message)s"
-
-AVAILABLE_PLATFORMS: Dict[str, Runner] = {
+AVAILABLE_PLATFORMS: dict[str, type[NetworkRunner]] = {
     AragonRunner.name: AragonRunner,
     DaohausRunner.name: DaohausRunner,
     DaostackRunner.name: DaostackRunner
 }
 
 # Get available networks from Runners
 AVAILABLE_NETWORKS = {n for n in ENDPOINTS.keys() if not n.startswith('_')}
 
-def _call_platform(platform: str, datawarehouse: Path, force: bool=False, networks=None, collectors=None):
-    p = AVAILABLE_PLATFORMS[platform]()
-    p.set_dw(datawarehouse)
-    p.run(networks=networks, force=force, collectors=collectors)
+def _call_platform(platform: str, datawarehouse: Path, force: bool=False, networks=None, collectors=None, block_datetime=None):
+    p = AVAILABLE_PLATFORMS[platform](datawarehouse)
+    p.run(networks=networks, force=force, collectors=collectors, until_date=block_datetime)
 
 def _is_good_version(datawarehouse: Path) -> bool:
     versionfile = datawarehouse / 'version.txt'
     if not versionfile.is_file():
         return False
 
     with open(versionfile, 'r') as vf:
-        l = vf.readline().strip()
-        return l == config.CACHE_SCRIPTS_VERSION
+        return vf.readline().strip() == __version__
 
-def main_aux(datawarehouse: Path):
-    if config.delete_force or not _is_good_version(datawarehouse):
-        if not config.delete_force:
-            print(f"datawarehouse version is not version {config.CACHE_SCRIPTS_VERSION}, upgrading")
-
-        # We skip the dotfiles like .lock
-        for p in datawarehouse.glob('[!.]*'):
-            if p.is_dir():
-                shutil.rmtree(p)
-            else:
-                p.unlink()
-
-    logger = logging.getLogger()
-    logger.propagate = True
-    filehandler = RotatingFileHandler(
-        filename=config.datawarehouse / 'cache_scripts.log',
-        maxBytes=config.LOGGING_MAX_MB * 2**20,
-        backupCount=config.LOGGING_BACKUP_COUNT,
-    )
-
-    filehandler.setFormatter(logging.Formatter(LOG_FILE_FORMAT))
-    logger.addHandler(filehandler)
-    logger.setLevel(level=logging.DEBUG if config.debug else logging.INFO)
-
-    logging.getLogger('gql.transport.requests').setLevel(level=logging.DEBUG if config.debug else logging.WARNING)
-
-    # Log errors to STDERR
-    streamhandler = logging.StreamHandler(stderr)
-    streamhandler.setLevel(logging.WARNING if config.debug else logging.ERROR)
-    streamhandler.setFormatter(logging.Formatter(LOG_STREAM_FORMAT))
-    logger.addHandler(streamhandler)
-
-    logging.info("Running dao-scripts with arguments: %s", sys.orig_argv)
+def run_all(
+    datawarehouse: Path, delete_force: bool, 
+    platforms: list[str], networks: list[str], collectors: list[str], 
+    block_datetime: datetime, force: bool
+):
 
     # The default config is every platform
-    if not config.platforms:
-        config.platforms = AVAILABLE_PLATFORMS.keys()
+    if not platforms:
+        platforms = list(AVAILABLE_PLATFORMS.keys())
 
     # Now calling the platform and deleting if needed
-    for p in config.platforms:
-        _call_platform(p, datawarehouse, config.force, config.networks, config.collectors)
+    for platform in platforms:
+        _call_platform(platform, datawarehouse, force, networks, collectors, block_datetime)
 
     # write date
     data_date: str = str(datetime.now().isoformat())
 
-    if config.block_datetime:
-        data_date = config.block_datetime.isoformat()
+    if block_datetime:
+        data_date = block_datetime.isoformat()
 
     with open(datawarehouse / 'update_date.txt', 'w') as f:
         print(data_date, file=f)
 
     with open(datawarehouse / 'version.txt', 'w') as f:
-        print(config.CACHE_SCRIPTS_VERSION, file=f)
+        print(__version__, file=f)
 
-def main_lock(datawarehouse: Path):
+def lock_and_run(args: Namespace):
+    datawarehouse: Path = args.datawarehouse
     datawarehouse.mkdir(exist_ok=True)
     
     # Lock for the datawarehouse (also used by the dash)
     p_lock: Path = datawarehouse / '.lock'
 
     # Exclusive lock for the chache-scripts (no two cache-scripts running)
     cs_lock: Path = datawarehouse / '.cs.lock'
 
     try:
         with pl.Lock(cs_lock, 'w', timeout=1) as lock, \
-             tempfile.TemporaryDirectory(prefix="datawarehouse_") as tmp_dw:
+             tempfile.TemporaryDirectory(prefix="datawarehouse_") as tmp_dw_str:
 
             # Writing pid and dir name to lock (debugging)
-            tmp_dw = Path(tmp_dw)
+            tmp_dw = Path(tmp_dw_str)
             print(os.getpid(), file=lock)
             print(tmp_dw, file=lock)
             lock.flush()
+            (datawarehouse / '.running').symlink_to(tmp_dw)
 
-            ignore = shutil.ignore_patterns('*.log', '.lock*')
-
-            # We want to copy the dw, so we open it as readers
-            p_lock.touch(exist_ok=True)
-            with pl.Lock(p_lock, 'r', timeout=1, flags=pl.LOCK_SH | pl.LOCK_NB):
-                shutil.copytree(datawarehouse, tmp_dw, dirs_exist_ok=True, ignore=ignore)
-
-            main_aux(datawarehouse=tmp_dw)
+            # Used to tell the loggers to use errors.log or the main logs
+            copied_dw = False
 
-            with pl.Lock(p_lock, 'w', timeout=10):
-                shutil.copytree(tmp_dw, datawarehouse, dirs_exist_ok=True, ignore=ignore)
+            try:
+                ignore = shutil.ignore_patterns('.lock*', 'logs/*')
 
-            # Removing pid from lock
-            lock.truncate(0)
+                # We want to copy the dw, so we open it as readers
+                p_lock.touch(exist_ok=True)
+                with pl.Lock(p_lock, 'r', timeout=1, flags=pl.LOCK_SH | pl.LOCK_NB):
+                    shutil.copytree(datawarehouse, tmp_dw, dirs_exist_ok=True, ignore=ignore)
+
+                if args.delete_force or not _is_good_version(datawarehouse):
+                    if not args.delete_force:
+                        print(f"datawarehouse version is not version {__version__}, upgrading")
+
+                    # We skip the dotfiles like .lock
+                    for p in datawarehouse.glob('[!.]*'):
+                        if p.is_dir():
+                            shutil.rmtree(p)
+                        else:
+                            p.unlink()
+
+                setup_logging(tmp_dw, datawarehouse, config.DEBUG)
+                logger = logging.getLogger('dao_analyzer.main')
+                logger.info(">>> Running dao-scripts with arguments: %s", sys.orig_argv)
+
+                # Execute the scripts in the aux datawarehouse
+                run_all(
+                    datawarehouse=tmp_dw,
+                    delete_force=args.delete_force,
+                    platforms=args.platforms,
+                    networks=args.networks,
+                    collectors=args.collectors,
+                    block_datetime=args.block_datetime,
+                    force=args.force,
+                )
+
+                # Copying back the dw
+                logger.info(f"<<< Copying back the datawarehouse from {tmp_dw} to {datawarehouse}")
+                with pl.Lock(p_lock, 'w', timeout=10):
+                    shutil.copytree(tmp_dw, datawarehouse, dirs_exist_ok=True, ignore=ignore)
+                
+                copied_dw = True
+            finally:
+                # Removing pid from lock
+                lock.truncate(0)
+                (datawarehouse / '.running').unlink()
+                finish_logging(errors=not copied_dw)
     except pl.LockException:
         with open(cs_lock, 'r') as f:
             pid = int(f.readline())
 
         print(f"The cache_scripts are already being run with pid {pid}", file=stderr)
         exit(1)
 
 def main():
     parser = CacheScriptsArgParser(
         available_platforms=list(AVAILABLE_PLATFORMS.keys()),
         available_networks=AVAILABLE_NETWORKS)
 
-    config.populate_args(parser.parse_args())
+    args = parser.parse_args()
+    config.args2config(args)
 
-    if config.display_version:
-        print(config.CACHE_SCRIPTS_VERSION)
+    if args.display_version:
+        print(__version__)
         exit(0)
 
-    main_lock(config.datawarehouse)
+    lock_and_run(args)
 
 if __name__ == '__main__':
     main()
```

### Comparing `dao-scripts-1.2.2/src/metadata.py` & `dao_scripts-1.3.0/src/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
     Created on: 23-nov-2021
 
     Copyright 2021 David Davó
         <david@ddavo.me>
 """
 from json.encoder import JSONEncoder
-from typing import Dict
+from typing import Optional
 import json
 from functools import total_ordering
 from datetime import datetime, timezone
 
 from . import config
 
 @total_ordering
@@ -22,15 +22,15 @@
         self.timestamp = datetime.min
 
         if isinstance(init, dict):
             self.number = int(init["number"]) if "number" in init else self.number
             self.id = init["id"] if "id" in init else self.id
 
             if "timestamp" in init:
-                if init["timestamp"].isdigit():
+                if isinstance(init['timestamp'], int) or init["timestamp"].isdigit():
                     self.timestamp = datetime.fromtimestamp(int(init["timestamp"]))
                 else:
                     self.timestamp = datetime.fromisoformat(init["timestamp"])
             
         if self.timestamp.tzinfo is None:
             self.timestamp = self.timestamp.replace(tzinfo=timezone.utc)
 
@@ -52,15 +52,15 @@
         }
 
     def __str__(self):
         return self.toDict().__str__()
 
 class CollectorMetaData:
     def __init__(self, c: str, d = None):
-        self.block = Block()
+        self.block: Optional[Block] = Block()
         self._collector: str = c
         self.last_update: datetime = datetime.now(timezone.utc)
 
         if d:
             self.block = Block(d["block"]) if "block" in d else None
             self.last_update = datetime.fromisoformat(d["last_update"])
 
@@ -85,16 +85,16 @@
             return o.toDict()
         else:
             return super().default(o)
 
 class RunnerMetadata:
     def __init__(self, runner):
         self._path = runner.basedir / 'metadata.json'
-        self.collectorMetaData: Dict[str, CollectorMetaData] = {}
-        self.errors: Dict[str, str] = {}
+        self.collectorMetaData: dict[str, CollectorMetaData] = {}
+        self.errors: dict[str, str] = {}
         self._setPrev()
 
     def _setPrev(self):
         self._prev = (self.errors.copy(), self.collectorMetaData.copy())
     
     @property
     def dirty(self) -> bool:
@@ -121,15 +121,15 @@
 
     def dump(self):
         with open(self._path, 'w') as f:
             json.dump({
                 "metadata": self.collectorMetaData,
                 "errors": self.errors
             }, f, 
-                indent=2 if config.debug else None, 
+                indent=2 if config.DEBUG else None, 
                 cls=MetadataEncoder)
 
     def ifdump(self):
         if self.dirty:
             self.dump()
 
     def __enter__(self):
```

### Comparing `dao-scripts-1.2.2/src/utils/uploadDataWarehouse.py` & `dao_scripts-1.3.0/src/utils/uploadDataWarehouse.py`

 * *Files identical despite different names*

