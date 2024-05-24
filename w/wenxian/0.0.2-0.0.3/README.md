# Comparing `tmp/wenxian-0.0.2.tar.gz` & `tmp/wenxian-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wenxian-0.0.2.tar", last modified: Tue May 21 08:11:15 2024, max compression
+gzip compressed data, was "wenxian-0.0.3.tar", last modified: Fri May 24 08:18:21 2024, max compression
```

## Comparing `wenxian-0.0.2.tar` & `wenxian-0.0.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:15.444022 wenxian-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-21 08:11:11.000000 wenxian-0.0.2/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 08:11:11.000000 wenxian-0.0.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:15.436022 wenxian-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:15.440022 wenxian-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-21 08:11:11.000000 wenxian-0.0.2/.github/workflows/comment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-21 08:11:11.000000 wenxian-0.0.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-21 08:11:11.000000 wenxian-0.0.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-21 08:11:11.000000 wenxian-0.0.2/.github/workflows/test_action.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-21 08:11:11.000000 wenxian-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-21 08:11:11.000000 wenxian-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-21 08:11:11.000000 wenxian-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-21 08:11:15.444022 wenxian-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-21 08:11:11.000000 wenxian-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-21 08:11:11.000000 wenxian-0.0.2/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:15.440022 wenxian-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 08:11:11.000000 wenxian-0.0.2/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-21 08:11:11.000000 wenxian-0.0.2/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-21 08:11:11.000000 wenxian-0.0.2/docs/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-21 08:11:11.000000 wenxian-0.0.2/docs/pyworker.js
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-21 08:11:11.000000 wenxian-0.0.2/docs/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-21 08:11:11.000000 wenxian-0.0.2/docs/webworker.js
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-21 08:11:11.000000 wenxian-0.0.2/docs/wenxian.js
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-21 08:11:11.000000 wenxian-0.0.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-21 08:11:11.000000 wenxian-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 08:11:15.444022 wenxian-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:15.440022 wenxian-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 08:11:11.000000 wenxian-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21737 2024-05-21 08:11:11.000000 wenxian-0.0.2/tests/cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-21 08:11:11.000000 wenxian-0.0.2/tests/test_bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-21 08:11:11.000000 wenxian-0.0.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-21 08:11:11.000000 wenxian-0.0.2/tests/test_from_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-21 08:11:11.000000 wenxian-0.0.2/tests/test_identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:15.444022 wenxian-0.0.2/wenxian/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:15.444022 wenxian-0.0.2/wenxian/feeder/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/feeder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/feeder/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/feeder/crossref.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/feeder/feeder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/feeder/pubmed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/feeder/semanticscholar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/feeder/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/from_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:15.444022 wenxian-0.0.2/wenxian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-21 08:11:15.000000 wenxian-0.0.2/wenxian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-21 08:11:15.000000 wenxian-0.0.2/wenxian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:11:15.000000 wenxian-0.0.2/wenxian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 08:11:15.000000 wenxian-0.0.2/wenxian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-21 08:11:15.000000 wenxian-0.0.2/wenxian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 08:11:15.000000 wenxian-0.0.2/wenxian.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:18:21.307695 wenxian-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-24 08:18:17.000000 wenxian-0.0.3/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-24 08:18:17.000000 wenxian-0.0.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:18:21.299695 wenxian-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:18:21.303695 wenxian-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-24 08:18:17.000000 wenxian-0.0.3/.github/workflows/comment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-24 08:18:17.000000 wenxian-0.0.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-24 08:18:17.000000 wenxian-0.0.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-24 08:18:17.000000 wenxian-0.0.3/.github/workflows/test_action.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-24 08:18:17.000000 wenxian-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-24 08:18:17.000000 wenxian-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-24 08:18:17.000000 wenxian-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-24 08:18:21.307695 wenxian-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-24 08:18:17.000000 wenxian-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-24 08:18:17.000000 wenxian-0.0.3/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:18:21.303695 wenxian-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-24 08:18:17.000000 wenxian-0.0.3/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-24 08:18:17.000000 wenxian-0.0.3/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-24 08:18:17.000000 wenxian-0.0.3/docs/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-24 08:18:17.000000 wenxian-0.0.3/docs/pyworker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-24 08:18:17.000000 wenxian-0.0.3/docs/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-24 08:18:17.000000 wenxian-0.0.3/docs/webworker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-24 08:18:17.000000 wenxian-0.0.3/docs/wenxian.js
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-24 08:18:17.000000 wenxian-0.0.3/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-24 08:18:17.000000 wenxian-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 08:18:21.307695 wenxian-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:18:21.303695 wenxian-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 08:18:17.000000 wenxian-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21737 2024-05-24 08:18:17.000000 wenxian-0.0.3/tests/cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-24 08:18:17.000000 wenxian-0.0.3/tests/test_bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-24 08:18:17.000000 wenxian-0.0.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-24 08:18:17.000000 wenxian-0.0.3/tests/test_from_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-24 08:18:17.000000 wenxian-0.0.3/tests/test_identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:18:21.303695 wenxian-0.0.3/wenxian/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-24 08:18:17.000000 wenxian-0.0.3/wenxian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-24 08:18:17.000000 wenxian-0.0.3/wenxian/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:18:21.307695 wenxian-0.0.3/wenxian/feeder/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 08:18:17.000000 wenxian-0.0.3/wenxian/feeder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-24 08:18:17.000000 wenxian-0.0.3/wenxian/feeder/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-24 08:18:17.000000 wenxian-0.0.3/wenxian/feeder/crossref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-24 08:18:17.000000 wenxian-0.0.3/wenxian/feeder/feeder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-24 08:18:17.000000 wenxian-0.0.3/wenxian/feeder/pubmed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-24 08:18:17.000000 wenxian-0.0.3/wenxian/feeder/semanticscholar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-24 08:18:17.000000 wenxian-0.0.3/wenxian/feeder/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-24 08:18:17.000000 wenxian-0.0.3/wenxian/from_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-24 08:18:17.000000 wenxian-0.0.3/wenxian/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:18:17.000000 wenxian-0.0.3/wenxian/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-24 08:18:17.000000 wenxian-0.0.3/wenxian/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:18:21.307695 wenxian-0.0.3/wenxian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-24 08:18:21.000000 wenxian-0.0.3/wenxian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-24 08:18:21.000000 wenxian-0.0.3/wenxian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:18:21.000000 wenxian-0.0.3/wenxian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 08:18:21.000000 wenxian-0.0.3/wenxian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-24 08:18:21.000000 wenxian-0.0.3/wenxian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 08:18:21.000000 wenxian-0.0.3/wenxian.egg-info/top_level.txt
```

### Comparing `wenxian-0.0.2/.github/workflows/comment.yaml` & `wenxian-0.0.3/.github/workflows/comment.yaml`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/.github/workflows/release.yaml` & `wenxian-0.0.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/.github/workflows/test.yaml` & `wenxian-0.0.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/.github/workflows/test_action.yaml` & `wenxian-0.0.3/.github/workflows/test_action.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             @Article{He_arXiv_2015_p1512.03385,
                 author =   {Kaiming He and Xiangyu Zhang and Shaoqing Ren and Jian Sun},
                 title =    {{Deep Residual Learning for Image Recognition}},
                 journal =  {arXiv},
                 year =     2015,
                 pages =    {1512.03385},
                 doi =      {10.48550/arXiv.1512.03385},
-                annote =   {Deeper neural networks are more difficult to train. We present a
+                abstract = {Deeper neural networks are more difficult to train. We present a
                          residual learning framework to ease the training of networks that are
                          substantially deeper than those used previously. We explicitly
                          reformulate the layers as learning residual functions with reference
                          to the layer inputs, instead of learning unreferenced functions. We
                          provide comprehensive empirical evidence showing that these residual
                          networks are easier to optimize, and can gain accuracy from
                          considerably increased depth. On the ImageNet dataset we evaluate
```

### Comparing `wenxian-0.0.2/.gitignore` & `wenxian-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/.pre-commit-config.yaml` & `wenxian-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/LICENSE` & `wenxian-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/PKG-INFO` & `wenxian-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wenxian
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate references.
 Author-email: Jinzhe Zeng <jinzhe.zeng@rutgers.edu>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `wenxian-0.0.2/README.md` & `wenxian-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/action.yml` & `wenxian-0.0.3/action.yml`

 * *Files 25% similar despite different names*

```diff
@@ -7,18 +7,14 @@
 outputs:
   bibtex:
     description: "Generated BibTeX entry"
     value: ${{ steps.run-wenxian.outputs.bibtex }}
 runs:
   using: composite
   steps:
-    - name: Setup Python
-      uses: actions/setup-python@v5
-      with:
-        python-version: "3.8 - 3.12"
     - name: Run wenxian
       id: run-wenxian
       run: |
         {
           echo 'bibtex<<EOF'
           pipx run --spec ${{ github.action_path }} wenxian from $INPUT_IDENTIFIER
           echo EOF
```

### Comparing `wenxian-0.0.2/docs/index.html` & `wenxian-0.0.3/docs/index.html`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/docs/logo.svg` & `wenxian-0.0.3/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/docs/pyworker.js` & `wenxian-0.0.3/docs/pyworker.js`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/docs/style.css` & `wenxian-0.0.3/docs/style.css`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/docs/webworker.js` & `wenxian-0.0.3/docs/webworker.js`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/docs/wenxian.js` & `wenxian-0.0.3/docs/wenxian.js`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/pyproject.toml` & `wenxian-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/tests/cases.py` & `wenxian-0.0.3/tests/cases.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,18 @@
         @Article{Zeng_JChemTheoryComput_2023_v19_p1261,
             author =   {Jinzhe Zeng and Yujun Tao and Timothy J. Giese and Darrin M. York},
             title =    {{QD{\ensuremath{\pi}}: A Quantum Deep Potential Interaction Model for
                      Drug Discovery}},
             journal =  {J. Chem. Theory Comput.},
             year =     2023,
             volume =   19,
-            issue =    4,
+            number =   4,
             pages =    {1261--1275},
             doi =      {10.1021/acs.jctc.2c01172},
-            annote =   {We report QD{\ensuremath{\pi}}-v1.0 for modeling the internal energy
+            abstract = {We report QD{\ensuremath{\pi}}-v1.0 for modeling the internal energy
                      of drug molecules containing H, C, N, and O atoms. The
                      QD{\ensuremath{\pi}} model is in the form of a quantum
                      mechanical/machine learning potential correction
                      (QM/{\ensuremath{\Delta}}-MLP) that uses a fast third-order self-
                      consistent density-functional tight-binding (DFTB3/3OB) model that is
                      corrected to a quantitatively high-level of accuracy through a deep-
                      learning potential (DeepPot-SE). The model has the advantage that it
@@ -184,15 +184,15 @@
                          Zhang and Han Wang and Weinan E},
                 title =    {{DP-GEN: A concurrent learning platform for the generation of reliable
                          deep learning based potential energy models}},
                 journal =  {arXiv},
                 year =     2019,
                 pages =    {1910.12690},
                 doi =      {10.48550/arXiv.1910.12690},
-                annote =   {In recent years, promising deep learning based interatomic potential
+                abstract = {In recent years, promising deep learning based interatomic potential
                          energy surface (PES) models have been proposed that can potentially
                          allow us to perform molecular dynamics simulations for large scale
                          systems with quantum accuracy. However, making these models truly
                          reliable and practically useful is still a very non-trivial task. A
                          key component in this task is the generation of datasets used in model
                          training. In this paper, we introduce the Deep Potential GENerator
                          (DP-GEN), an open-source software platform that implements the
@@ -311,18 +311,18 @@
                          and Anurag Kumar Singh and Sikai Yao and Jingchao Zhang and Renata
                          Wentzcovitch and Jiequn Han and Jie Liu and Weile Jia and Darrin M.
                          York and Weinan E and Roberto Car and Linfeng Zhang and Han Wang},
                 title =    {{DeePMD-kit v2: A software package for deep potential models}},
                 journal =  {J. Chem. Phys.},
                 year =     2023,
                 volume =   159,
-                issue =    5,
+                number =   5,
                 pages =    054801,
                 doi =      {10.1063/5.0155600},
-                annote =   {DeePMD-kit is a powerful open-source software package that facilitates
+                abstract = {DeePMD-kit is a powerful open-source software package that facilitates
                          molecular dynamics simulations using machine learning potentials known
                          as Deep Potential (DP) models. This package, which was released in
                          2017, has been widely used in the fields of physics, chemistry,
                          biology, and material science for studying atomistic systems. The
                          current version of DeePMD-kit offers numerous advanced features, such
                          as DeepPot-SE, attention-based and hybrid descriptors, the ability to
                          fit tensile properties, type embedding, model deviation, DP-range
@@ -365,16 +365,16 @@
             @Article{Zeng_EnergyFuels_2021_v35_p762,
                 author =   {Jinzhe Zeng and Linfeng Zhang and Han Wang and Tong Zhu},
                 title =    {{Exploring the Chemical Space of Linear Alkane Pyrolysis via Deep
                          Potential GENerator}},
                 journal =  {Energy Fuels},
                 year =     2021,
                 volume =   35,
-                issue =    1,
+                number =   1,
                 pages =    {762--769},
                 doi =      {10.1021/acs.energyfuels.0c03211},
-                annote =   {Reactive molecular dynamics (MD) simulation is a powerful tool to
+                abstract = {Reactive molecular dynamics (MD) simulation is a powerful tool to
                          study the reaction mechanism of complex chemical systems. Central to
                          the method is the potential energy surface (PES) that can desc...},
             }""").strip(),
     ),
 ]
```

### Comparing `wenxian-0.0.2/tests/test_cli.py` & `wenxian-0.0.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/tests/test_from_identifier.py` & `wenxian-0.0.3/tests/test_from_identifier.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/wenxian/__main__.py` & `wenxian-0.0.3/wenxian/__main__.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/wenxian/feeder/arxiv.py` & `wenxian-0.0.3/wenxian/feeder/arxiv.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/wenxian/feeder/crossref.py` & `wenxian-0.0.3/wenxian/feeder/crossref.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/wenxian/feeder/feeder.py` & `wenxian-0.0.3/wenxian/feeder/feeder.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/wenxian/feeder/pubmed.py` & `wenxian-0.0.3/wenxian/feeder/pubmed.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/wenxian/feeder/semanticscholar.py` & `wenxian-0.0.3/wenxian/feeder/semanticscholar.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/wenxian/feeder/session.py` & `wenxian-0.0.3/wenxian/feeder/session.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/wenxian/from_identifier.py` & `wenxian-0.0.3/wenxian/from_identifier.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/wenxian/identifier.py` & `wenxian-0.0.3/wenxian/identifier.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.2/wenxian/reference.py` & `wenxian-0.0.3/wenxian/reference.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,24 +96,25 @@
         if self.pages is None:
             page_string = None
         elif isinstance(self.pages, tuple):
             page_string = "--".join(str(x) for x in self.pages)
         else:
             page_string = str(self.pages)
 
+        # See https://us.mirrors.cicku.me/ctan/macros/latex/contrib/biblatex/doc/biblatex.pdf
         data = {
             "author": author_string,
             "title": self.title,
             "journal": self.journal_abbr,
             "year": self.year,
             "volume": self.volume,
-            "issue": self.issue,
+            "number": self.issue,
             "pages": page_string,
             "doi": self.doi,
-            "annote": self.annote,
+            "abstract": self.annote,
         }
         start = f"@Article{{{self.key},"
         end = "}\n"
         items = [start]
         for key, value in data.items():
             if value is None:
                 continue
```

### Comparing `wenxian-0.0.2/wenxian.egg-info/PKG-INFO` & `wenxian-0.0.3/wenxian.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wenxian
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate references.
 Author-email: Jinzhe Zeng <jinzhe.zeng@rutgers.edu>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `wenxian-0.0.2/wenxian.egg-info/SOURCES.txt` & `wenxian-0.0.3/wenxian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

