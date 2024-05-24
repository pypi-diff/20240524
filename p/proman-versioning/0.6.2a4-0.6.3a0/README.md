# Comparing `tmp/proman_versioning-0.6.2a4.tar.gz` & `tmp/proman_versioning-0.6.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proman_versioning-0.6.2a4.tar", last modified: Fri May 10 04:38:16 2024, max compression
+gzip compressed data, was "proman_versioning-0.6.3a0.tar", last modified: Fri May 24 00:48:41 2024, max compression
```

## Comparing `proman_versioning-0.6.2a4.tar` & `proman_versioning-0.6.3a0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:38:16.390022 proman_versioning-0.6.2a4/
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-10 04:38:16.390022 proman_versioning-0.6.2a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-10 04:37:25.000000 proman_versioning-0.6.2a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 04:38:16.390022 proman_versioning-0.6.2a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:38:16.382022 proman_versioning-0.6.2a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:38:16.386022 proman_versioning-0.6.2a4/src/proman_versioning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-10 04:38:16.000000 proman_versioning-0.6.2a4/src/proman_versioning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-10 04:38:16.000000 proman_versioning-0.6.2a4/src/proman_versioning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 04:38:16.000000 proman_versioning-0.6.2a4/src/proman_versioning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 04:38:16.000000 proman_versioning-0.6.2a4/src/proman_versioning.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-10 04:38:16.000000 proman_versioning-0.6.2a4/src/proman_versioning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 04:38:16.000000 proman_versioning-0.6.2a4/src/proman_versioning.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:38:16.386022 proman_versioning-0.6.2a4/src/versioning/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-10 04:37:25.000000 proman_versioning-0.6.2a4/src/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:38:16.386022 proman_versioning-0.6.2a4/src/versioning/grammars/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/grammars/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/grammars/conventional_commits.lark
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/grammars/conventional_commits.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/vcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16146 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:38:16.386022 proman_versioning-0.6.2a4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-10 04:37:25.000000 proman_versioning-0.6.2a4/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/tests/test_versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:48:41.124482 proman_versioning-0.6.3a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-24 00:48:41.120482 proman_versioning-0.6.3a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-24 00:48:02.000000 proman_versioning-0.6.3a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 00:48:41.124482 proman_versioning-0.6.3a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:48:41.116482 proman_versioning-0.6.3a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:48:41.120482 proman_versioning-0.6.3a0/src/proman_versioning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-24 00:48:41.000000 proman_versioning-0.6.3a0/src/proman_versioning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-24 00:48:41.000000 proman_versioning-0.6.3a0/src/proman_versioning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 00:48:41.000000 proman_versioning-0.6.3a0/src/proman_versioning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-24 00:48:41.000000 proman_versioning-0.6.3a0/src/proman_versioning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-24 00:48:41.000000 proman_versioning-0.6.3a0/src/proman_versioning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 00:48:41.000000 proman_versioning-0.6.3a0/src/proman_versioning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:48:41.120482 proman_versioning-0.6.3a0/src/versioning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-24 00:48:02.000000 proman_versioning-0.6.3a0/src/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/src/versioning/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/src/versioning/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/src/versioning/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/src/versioning/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/src/versioning/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/src/versioning/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:48:41.120482 proman_versioning-0.6.3a0/src/versioning/grammars/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/src/versioning/grammars/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/src/versioning/grammars/conventional_commits.lark
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/src/versioning/grammars/conventional_commits.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/src/versioning/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/src/versioning/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16146 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/src/versioning/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:48:41.120482 proman_versioning-0.6.3a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-24 00:48:02.000000 proman_versioning-0.6.3a0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-24 00:48:25.000000 proman_versioning-0.6.3a0/tests/test_versioning.py
```

### Comparing `proman_versioning-0.6.2a4/LICENSE.md` & `proman_versioning-0.6.3a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proman_versioning-0.6.2a4/PKG-INFO` & `proman_versioning-0.6.3a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proman-versioning
-Version: 0.6.2a4
+Version: 0.6.3a0
 Summary: Project Management Versioning Tool.
 Author-email: "Jesse P. Johnson" <jpj6652@gmail.com>
 Maintainer-email: "Jesse P. Johnson" <jpj6652@gmail.com>
 License: LGPL-3.0
 Project-URL: homepage, https://github.com/python-proman/proman-versioning
 Project-URL: repository, https://github.com/python-proman/proman-versioning
 Keywords: versioning,semver,calver,pep440,configuration management
@@ -14,22 +14,24 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6.2
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: lark-parser>=0.10.0
 Requires-Dist: argufy>=0.1.1-alpha.12
 Requires-Dist: transitions>=0.8.4
-Requires-Dist: pygit2>=1.6.1
+Requires-Dist: pygit2>=1.15
 Requires-Dist: cffi>=1.15.0
 Requires-Dist: packaging>=21.3
 Requires-Dist: compendium>=0.1.3
 Provides-Extra: changelog
 Requires-Dist: mdutils; extra == "changelog"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
```

### Comparing `proman_versioning-0.6.2a4/README.md` & `proman_versioning-0.6.3a0/README.md`

 * *Files identical despite different names*

### Comparing `proman_versioning-0.6.2a4/pyproject.toml` & `proman_versioning-0.6.3a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proman-versioning"
-version = "0.6.2a4"
+version = "0.6.3a0"
 description = "Project Management Versioning Tool."
 readme = "README.md"
 license = {text = "LGPL-3.0"}
 keywords = ["versioning", "semver", "calver", "pep440", "configuration management"]
 requires-python = ">=3.6.2"
 authors = [{name = "Jesse P. Johnson", email = "jpj6652@gmail.com"}]
 maintainers = [{name = "Jesse P. Johnson", email = "jpj6652@gmail.com"}]
@@ -19,30 +19,32 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Topic :: Software Development :: Libraries",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Topic :: Software Development :: Libraries"
 ]
 
 dependencies = [
     "lark-parser>=0.10.0",
     "argufy>=0.1.1-alpha.12",
     "transitions>=0.8.4",
-    "pygit2>=1.6.1",
+    "pygit2>=1.15",
     "cffi>=1.15.0",
     "packaging>=21.3",
-    "compendium>=0.1.3",
+    "compendium>=0.1.3"
 ]
 
 [project.optional-dependencies]
 changelog = [
-    "mdutils",
+    "mdutils"
 ]
 build = [
     "build",
     "proman-versioning>=0.5.0-alpha.2",
     "twine"
 ]
 dev = [
@@ -66,15 +68,14 @@
     "docstr-coverage>=1.2.0",
     "mkdocs>=1.2.2",
     "mkdocs-material>=7.2.0",
     "mkdocstrings[python]>=0.16.2",
     "pydocstyle[toml]>=6.1.1"
 ]
 
-
 [project.scripts]
 version = "versioning.__main__:main"
 
 [project.urls]
 homepage = "https://github.com/python-proman/proman-versioning"
 repository = "https://github.com/python-proman/proman-versioning"
 
@@ -88,23 +89,19 @@
 filepath = "src/versioning/__init__.py"
 pattern = "__version__ = '${version}'"
 
 [[tool.proman.versioning.files]]
 filepath = "tests/test_version.py"
 pattern = "__version__ == '${version}'"
 
-[[tool.proman.versioning.files]]
-filepath = "pyproject.toml"
-pattern = "version = \"${version}\""
-
 [tool.pydocstyle]
 ignore = [
     "D203",
     "D213",
-    "D300",
+    "D300"
 ]
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.black]
@@ -121,14 +118,15 @@
     | dist
   )
 )
 '''
 
 [tool.pylint]
 fail-under = 9.0
+ignored-modules = ["pygit2"]
 
 [tool.pylint."FORMAT"]
 max-line-length = 79
 
 [tool.pylint."MESSAGES CONTROL"]
 disable = [
     "C0103",
```

### Comparing `proman_versioning-0.6.2a4/src/proman_versioning.egg-info/PKG-INFO` & `proman_versioning-0.6.3a0/src/proman_versioning.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proman-versioning
-Version: 0.6.2a4
+Version: 0.6.3a0
 Summary: Project Management Versioning Tool.
 Author-email: "Jesse P. Johnson" <jpj6652@gmail.com>
 Maintainer-email: "Jesse P. Johnson" <jpj6652@gmail.com>
 License: LGPL-3.0
 Project-URL: homepage, https://github.com/python-proman/proman-versioning
 Project-URL: repository, https://github.com/python-proman/proman-versioning
 Keywords: versioning,semver,calver,pep440,configuration management
@@ -14,22 +14,24 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6.2
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: lark-parser>=0.10.0
 Requires-Dist: argufy>=0.1.1-alpha.12
 Requires-Dist: transitions>=0.8.4
-Requires-Dist: pygit2>=1.6.1
+Requires-Dist: pygit2>=1.15
 Requires-Dist: cffi>=1.15.0
 Requires-Dist: packaging>=21.3
 Requires-Dist: compendium>=0.1.3
 Provides-Extra: changelog
 Requires-Dist: mdutils; extra == "changelog"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
```

### Comparing `proman_versioning-0.6.2a4/src/proman_versioning.egg-info/SOURCES.txt` & `proman_versioning-0.6.3a0/src/proman_versioning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proman_versioning-0.6.2a4/src/versioning/__init__.py` & `proman_versioning-0.6.3a0/src/versioning/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from versioning.vcs import Git
 from versioning.version import Version  # noqa
 
 __author__ = 'Jesse P. Johnson'
 __author_email__ = 'jpj6652@gmail.com'
 __title__ = 'proman-versioning'
 __description__ = 'Workflows to manage project versioning.'
-__version__ = '0.6.2a4'
+__version__ = '0.6.3a0'
 __license__ = 'LGPL-3.0'
 __copyright__ = 'Copyright 2021 Jesse Johnson.'
 __all__ = (
     'ReleaseController',
     'get_release_controller',
     'Version',
 )
```

### Comparing `proman_versioning-0.6.2a4/src/versioning/changelog.py` & `proman_versioning-0.6.3a0/src/versioning/changelog.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     def _categorize_commit(self, commit: 'Commit') -> Tuple[str, List[str]]:
         """Get changes associated with a release."""
         parser = CommitMessageParser()
         parser.parse(commit.message.rstrip())
         # scope = parser.title['scope']
         row = [
-            commit.hex,
+            str(commit.id),
             parser.title['type'],
             parser.title['description'],
         ]
 
         if parser.title['type'] == 'feat':
             section = 'added'
         elif parser.title['type'] == 'fix':
```

### Comparing `proman_versioning-0.6.2a4/src/versioning/cli.py` & `proman_versioning-0.6.3a0/src/versioning/cli.py`

 * *Files identical despite different names*

### Comparing `proman_versioning-0.6.2a4/src/versioning/config.py` & `proman_versioning-0.6.3a0/src/versioning/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     if os.path.exists(f"{CURRENT_DIR}/.git")
     else discover_repository(CURRENT_DIR)
 )
 if REPO_DIR is None:
     raise VersioningException('Unable to locate git repository.')
 PROJECT_DIR = os.path.abspath(os.path.join(REPO_DIR, os.pardir))
 CONFIG_FILES = [
+    os.path.join(PROJECT_DIR, '.version'),
     os.path.join(PROJECT_DIR, '.versioning'),
     os.path.join(PROJECT_DIR, 'pyproject.toml'),
     # TODO: add setup.cfg
 ]
 
 GRAMMAR_PATH: str = os.path.join(
     os.path.dirname(__file__), 'grammars', 'conventional_commits.lark'
@@ -132,31 +133,29 @@
     def __post_init__(
         self, filepaths: List[str], defaults: Dict[str, Any]
     ) -> None:
         """Initialize settings from configuration."""
         super().__init__(filepaths=filepaths, separator='.', defaults=defaults)
 
         # load configuration from paths in order or precedence
-        config = (
-            self.lookup(
-                'proman.versioning',
-                'tool.proman.versioning',
-                'tool.poetry.versioning',
-            )
-            or {}
-        )
-
-        if (
-            self.templates == []
-            and 'files' in config
-            and config['files'] != []
-        ):
-            self.templates = config['files']
-        # else:
-        #     raise VersioningException('no versioned files provided')
+        config = self.lookup('versioning', 'tool.proman.versioning') or {}
+        if 'files' in config and config['files'] != []:
+            self.templates += config['files']
+
+        self.templates += [
+            {
+                'filepath': os.path.basename(x),
+                'pattern': "version = \"${version}\"",
+            }
+            for x in filepaths
+            if os.path.exists(x)
+            and os.path.basename(x)
+            not in [x['filepath'] for x in self.templates]
+        ]
+        # os.path.relpath(CONFIG_FILES[0], start=PROJECT_DIR),
 
         if 'types' not in config:
             angular_convention = [
                 'build',
                 'ci',
                 'docs',
                 'perf',
@@ -164,18 +163,18 @@
                 'style',
                 'test',
             ]
             config['types'] = angular_convention
         self.parser = ParserConfig(config=config)
 
         config_version = self.lookup(
+            'version',
             'project.version',
             'proman.version',
             'tool.proman.version',
-            'tool.poetry.version',
         )
         # if config_version is None:
         #     raise VersioningException('no version found in filepaths')
 
         # TODO: use different version based on config
         self.version = Version(
             version=str(config_version),
```

### Comparing `proman_versioning-0.6.2a4/src/versioning/controller.py` & `proman_versioning-0.6.3a0/src/versioning/controller.py`

 * *Files identical despite different names*

### Comparing `proman_versioning-0.6.2a4/src/versioning/grammars/conventional_commits.lark` & `proman_versioning-0.6.3a0/src/versioning/grammars/conventional_commits.lark`

 * *Files identical despite different names*

### Comparing `proman_versioning-0.6.2a4/src/versioning/grammars/conventional_commits.py` & `proman_versioning-0.6.3a0/src/versioning/grammars/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `proman_versioning-0.6.2a4/src/versioning/vcs.py` & `proman_versioning-0.6.3a0/src/versioning/vcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Parse git commit messages."""
 
 # import logging
 import os
 from typing import Any, List, Optional
 
 from pygit2 import (
-    GIT_OBJ_COMMIT,
+    GIT_OBJECT_COMMIT,
     Commit,
     RemoteCallbacks,
     Repository,
     Signature,
     Tag,
     UserPass,
 )
@@ -127,16 +127,16 @@
 
     def tag(
         self, name: str, branch: Optional[str] = None, **kwargs: Any
     ) -> Optional[Tag]:
         """Create tag."""
         ref = f"refs/heads/{branch}" if branch else self.ref
         commit = self.repo.resolve_refish(ref)[0]
-        oid = commit.hex
-        kind = kwargs.get('kind', GIT_OBJ_COMMIT)
+        oid = str(commit.id)
+        kind = kwargs.get('kind', GIT_OBJECT_COMMIT)
 
         # tagger = pygit2.Signature('Alice Doe', 'adoe@example.com', 12347, 0)
         tagger = Signature(self.username, self.email)
         message = kwargs.get('message')
         if not kwargs.get('dry_run', False):
             tag = self.repo.create_tag(
                 name, oid, kind, tagger, message or f"ci: {name}"
```

### Comparing `proman_versioning-0.6.2a4/src/versioning/version.py` & `proman_versioning-0.6.3a0/src/versioning/version.py`

 * *Files identical despite different names*

### Comparing `proman_versioning-0.6.2a4/tests/test_controller.py` & `proman_versioning-0.6.3a0/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `proman_versioning-0.6.2a4/tests/test_versioning.py` & `proman_versioning-0.6.3a0/tests/test_versioning.py`

 * *Files identical despite different names*

