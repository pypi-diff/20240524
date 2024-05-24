# Comparing `tmp/jaraco_xonsh-0.6.0.tar.gz` & `tmp/jaraco_xonsh-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco_xonsh-0.6.0.tar", last modified: Mon May 20 01:51:05 2024, max compression
+gzip compressed data, was "jaraco_xonsh-0.7.0.tar", last modified: Fri May 24 09:49:21 2024, max compression
```

## Comparing `jaraco_xonsh-0.6.0.tar` & `jaraco_xonsh-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:51:05.005307 jaraco_xonsh-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:51:04.997307 jaraco_xonsh-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:51:04.997307 jaraco_xonsh-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-20 01:51:05.005307 jaraco_xonsh-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:51:05.001307 jaraco_xonsh-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:51:05.001307 jaraco_xonsh-0.6.0/jaraco/
--rw-r--r--   0 runner    (1001) docker     (127)    12990 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/jaraco/xonsh.xsh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:51:05.001307 jaraco_xonsh-0.6.0/jaraco.xonsh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-20 01:51:04.000000 jaraco_xonsh-0.6.0/jaraco.xonsh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-20 01:51:04.000000 jaraco_xonsh-0.6.0/jaraco.xonsh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 01:51:04.000000 jaraco_xonsh-0.6.0/jaraco.xonsh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 01:51:04.000000 jaraco_xonsh-0.6.0/jaraco.xonsh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-20 01:51:04.000000 jaraco_xonsh-0.6.0/jaraco.xonsh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 01:51:04.000000 jaraco_xonsh-0.6.0/jaraco.xonsh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 01:51:05.005307 jaraco_xonsh-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:49:21.038088 jaraco_xonsh-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:49:21.034088 jaraco_xonsh-0.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:49:21.034088 jaraco_xonsh-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-24 09:49:21.038088 jaraco_xonsh-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:49:21.034088 jaraco_xonsh-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:49:21.034088 jaraco_xonsh-0.7.0/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/jaraco/xonsh.xsh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:49:21.034088 jaraco_xonsh-0.7.0/jaraco.xonsh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-24 09:49:21.000000 jaraco_xonsh-0.7.0/jaraco.xonsh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-24 09:49:21.000000 jaraco_xonsh-0.7.0/jaraco.xonsh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:49:21.000000 jaraco_xonsh-0.7.0/jaraco.xonsh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-24 09:49:21.000000 jaraco_xonsh-0.7.0/jaraco.xonsh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-24 09:49:21.000000 jaraco_xonsh-0.7.0/jaraco.xonsh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 09:49:21.000000 jaraco_xonsh-0.7.0/jaraco.xonsh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 09:49:21.038088 jaraco_xonsh-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-24 09:48:52.000000 jaraco_xonsh-0.7.0/tox.ini
```

### Comparing `jaraco_xonsh-0.6.0/.github/workflows/main.yml` & `jaraco_xonsh-0.7.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.6.0/LICENSE` & `jaraco_xonsh-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.6.0/NEWS.rst` & `jaraco_xonsh-0.7.0/NEWS.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v0.7.0
+======
+
+Features
+--------
+
+- Include in the prompt the last return code if nonzero.
+
+
 v0.5.2
 ======
 
 Bugfixes
 --------
 
 - Ensure at least the PATH is retained for shutil.which/subprocess.
```

### Comparing `jaraco_xonsh-0.6.0/PKG-INFO` & `jaraco_xonsh-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.xonsh
-Version: 0.6.0
+Version: 0.7.0
 Summary: Xonsh facilities used by jaraco
 Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
 Project-URL: Homepage, https://github.com/jaraco/jaraco.xonsh
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jaraco_xonsh-0.6.0/README.rst` & `jaraco_xonsh-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.6.0/docs/conf.py` & `jaraco_xonsh-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.6.0/jaraco/xonsh.xsh` & `jaraco_xonsh-0.7.0/jaraco/xonsh.xsh`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 # allow for local settings in ~/.local/xonsh.d
 for localf in pathlib.Path('~/.local/xonsh.d').expanduser().glob('*'):
 	source @(localf)
 
 
 import keyring
 
-$PROMPT = '{env_name:{} }{cwd_base}{branch_color}{curr_branch: {}}{RESET} {BOLD_BLUE}{prompt_end}{RESET} '
+$PROMPT = '{env_name:{} }{cwd_base}{branch_color}{curr_branch: {}}{RESET} {RED}{last_return_code_if_nonzero:[{BOLD_INTENSE_RED}{}{RED}] }{RESET}{BOLD_BLUE}{prompt_end}{RESET} '
 
 def remove_mercurial_metadata():
 	git rm .hg*
 	git commit -m "Remove Mercurial metadata"
 
 aliases['remove-mercurial-metadata'] = remove_mercurial_metadata
```

### Comparing `jaraco_xonsh-0.6.0/jaraco.xonsh.egg-info/PKG-INFO` & `jaraco_xonsh-0.7.0/jaraco.xonsh.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.xonsh
-Version: 0.6.0
+Version: 0.7.0
 Summary: Xonsh facilities used by jaraco
 Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
 Project-URL: Homepage, https://github.com/jaraco/jaraco.xonsh
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jaraco_xonsh-0.6.0/pyproject.toml` & `jaraco_xonsh-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.6.0/pytest.ini` & `jaraco_xonsh-0.7.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.6.0/tox.ini` & `jaraco_xonsh-0.7.0/tox.ini`

 * *Files identical despite different names*

