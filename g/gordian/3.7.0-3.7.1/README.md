# Comparing `tmp/gordian-3.7.0.tar.gz` & `tmp/gordian-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gordian-3.7.0.tar", last modified: Thu Oct 26 16:36:20 2023, max compression
+gzip compressed data, was "dist/gordian-3.7.1.tar", last modified: Thu May 23 22:46:39 2024, max compression
```

## Comparing `gordian-3.7.0.tar` & `gordian-3.7.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:36:20.000000 gordian-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2023-10-26 16:35:53.000000 gordian-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9023 2023-10-26 16:36:20.000000 gordian-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8731 2023-10-26 16:35:53.000000 gordian-3.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:36:20.000000 gordian-3.7.0/gordian/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2023-10-26 16:35:53.000000 gordian-3.7.0/gordian/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:36:20.000000 gordian-3.7.0/gordian/files/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-10-26 16:35:53.000000 gordian-3.7.0/gordian/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-10-26 16:35:53.000000 gordian-3.7.0/gordian/files/base_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2023-10-26 16:35:53.000000 gordian-3.7.0/gordian/files/changelog_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-10-26 16:35:53.000000 gordian-3.7.0/gordian/files/json_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-10-26 16:35:53.000000 gordian-3.7.0/gordian/files/markdown_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-10-26 16:35:53.000000 gordian-3.7.0/gordian/files/plaintext_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-10-26 16:35:53.000000 gordian-3.7.0/gordian/files/yaml_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2023-10-26 16:35:53.000000 gordian-3.7.0/gordian/gordian.py
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2023-10-26 16:35:53.000000 gordian-3.7.0/gordian/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2023-10-26 16:35:53.000000 gordian-3.7.0/gordian/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:36:20.000000 gordian-3.7.0/gordian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9023 2023-10-26 16:36:20.000000 gordian-3.7.0/gordian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-10-26 16:36:20.000000 gordian-3.7.0/gordian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-26 16:36:20.000000 gordian-3.7.0/gordian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-26 16:36:20.000000 gordian-3.7.0/gordian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-10-26 16:36:20.000000 gordian-3.7.0/gordian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-26 16:36:20.000000 gordian-3.7.0/gordian.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      449 2023-10-26 16:36:20.000000 gordian-3.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      924 2023-10-26 16:35:53.000000 gordian-3.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:36:20.000000 gordian-3.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2023-10-26 16:35:53.000000 gordian-3.7.0/tests/test_base_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2023-10-26 16:35:53.000000 gordian-3.7.0/tests/test_changelog_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-10-26 16:35:53.000000 gordian-3.7.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2023-10-26 16:35:53.000000 gordian-3.7.0/tests/test_gordian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-10-26 16:35:53.000000 gordian-3.7.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9029 2023-10-26 16:35:53.000000 gordian-3.7.0/tests/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2023-10-26 16:35:53.000000 gordian-3.7.0/tests/test_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:46:39.000000 gordian-3.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-05-23 22:46:20.000000 gordian-3.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-23 22:46:39.000000 gordian-3.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-23 22:46:20.000000 gordian-3.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:46:39.000000 gordian-3.7.1/gordian/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-23 22:46:20.000000 gordian-3.7.1/gordian/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:46:39.000000 gordian-3.7.1/gordian/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-23 22:46:20.000000 gordian-3.7.1/gordian/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-23 22:46:20.000000 gordian-3.7.1/gordian/files/base_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-23 22:46:20.000000 gordian-3.7.1/gordian/files/changelog_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 22:46:20.000000 gordian-3.7.1/gordian/files/json_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-23 22:46:20.000000 gordian-3.7.1/gordian/files/markdown_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-23 22:46:20.000000 gordian-3.7.1/gordian/files/plaintext_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-23 22:46:20.000000 gordian-3.7.1/gordian/files/yaml_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-05-23 22:46:20.000000 gordian-3.7.1/gordian/gordian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-23 22:46:20.000000 gordian-3.7.1/gordian/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-23 22:46:20.000000 gordian-3.7.1/gordian/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:46:39.000000 gordian-3.7.1/gordian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-23 22:46:39.000000 gordian-3.7.1/gordian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-23 22:46:39.000000 gordian-3.7.1/gordian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:46:39.000000 gordian-3.7.1/gordian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 22:46:39.000000 gordian-3.7.1/gordian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-23 22:46:39.000000 gordian-3.7.1/gordian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 22:46:39.000000 gordian-3.7.1/gordian.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-23 22:46:39.000000 gordian-3.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-23 22:46:20.000000 gordian-3.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:46:39.000000 gordian-3.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-23 22:46:20.000000 gordian-3.7.1/tests/test_base_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-23 22:46:20.000000 gordian-3.7.1/tests/test_changelog_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-23 22:46:20.000000 gordian-3.7.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-23 22:46:20.000000 gordian-3.7.1/tests/test_gordian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-23 22:46:20.000000 gordian-3.7.1/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-05-23 22:46:20.000000 gordian-3.7.1/tests/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-23 22:46:20.000000 gordian-3.7.1/tests/test_transformations.py
```

### Comparing `gordian-3.7.0/LICENSE` & `gordian-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gordian-3.7.0/PKG-INFO` & `gordian-3.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gordian
-Version: 3.7.0
+Version: 3.7.1
 Summary: A tool to search and replace files in a Git repo
 Home-page: https://github.com/argoproj-labs/gordian
 Author: Intuit
 Author-email: cg-sre@intuit.com
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
@@ -169,15 +169,15 @@
 The `GIT_PASSWORD` or `password=` may also contain a Personal Access Token instead of the account password.
 
 # Development
 The simplest way to hit the ground running if you want to contribute with code is using docker.
 
 Launch a python container
 ```shell
-localhost$ docker run --rm -it  -v $(pwd):$(pwd) -w $(pwd) python:3.7-stretch bash
+localhost$ docker run --rm -it  -v $(pwd):$(pwd) -w $(pwd)  python:3.11-slim-bullseye bash
 ```
 
 Install the project and test dependencies in developer mode
 ```shell
 container# pip install -e .[test]
 ```
```

### Comparing `gordian-3.7.0/README.md` & `gordian-3.7.1/gordian.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: gordian
+Version: 3.7.1
+Summary: A tool to search and replace files in a Git repo
+Home-page: https://github.com/argoproj-labs/gordian
+Author: Intuit
+Author-email: cg-sre@intuit.com
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 <div align="center">
 <img width="200"
 src=".github/gordian-logo.png">
 </div>
 
 Gordian
 ========
@@ -158,15 +169,15 @@
 The `GIT_PASSWORD` or `password=` may also contain a Personal Access Token instead of the account password.
 
 # Development
 The simplest way to hit the ground running if you want to contribute with code is using docker.
 
 Launch a python container
 ```shell
-localhost$ docker run --rm -it  -v $(pwd):$(pwd) -w $(pwd) python:3.7-stretch bash
+localhost$ docker run --rm -it  -v $(pwd):$(pwd) -w $(pwd)  python:3.11-slim-bullseye bash
 ```
 
 Install the project and test dependencies in developer mode
 ```shell
 container# pip install -e .[test]
 ```
```

### Comparing `gordian-3.7.0/gordian/files/base_file.py` & `gordian-3.7.1/gordian/files/base_file.py`

 * *Files identical despite different names*

### Comparing `gordian-3.7.0/gordian/files/changelog_file.py` & `gordian-3.7.1/gordian/files/changelog_file.py`

 * *Files identical despite different names*

### Comparing `gordian-3.7.0/gordian/files/yaml_file.py` & `gordian-3.7.1/gordian/files/yaml_file.py`

 * *Files identical despite different names*

### Comparing `gordian-3.7.0/gordian/gordian.py` & `gordian-3.7.1/gordian/gordian.py`

 * *Files identical despite different names*

### Comparing `gordian-3.7.0/gordian/repo.py` & `gordian-3.7.1/gordian/repo.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,23 +122,26 @@
         if source_branch:
             self.branch_name = f"refs/heads/{source_branch}"
             self.source_branch = self.branch_name
         else:
             self.branch_name = f"refs/heads/{datetime.datetime.now().strftime('%Y-%m-%d-%H%M%S.%f')}"
             self.source_branch = self.target_ref
 
-    @retry(GithubException, tries=3, delay=1, backoff=2)
+    @retry((GithubException, TimeoutError), tries=3, delay=1, backoff=2)
     def _get_repo_contents(self, path):
         try:
             logger.debug(f'Fetching repo contents {path}...')
             return self._source_repo.get_contents(path, self.target_branch)
         except GithubException as e:
             if e.status == 404:
                 raise e
             logger.info(f'Error fetching repo contents: {e}')
+        except TimeoutError as e:
+            logger.info(f'Error fetching repo contents: {e}')
+            raise e
 
     @retry(GithubException, tries=3, delay=1, backoff=2)
     def _make_branch(self):
         branch = self._get_branch()
         logger.debug(f'Creating branch {self.branch_name}')
 
         try:
@@ -244,10 +247,10 @@
             minor = patch = '0'
         elif self.semver_label == 'minor':
             minor = str(int(minor) + 1)
             patch = '0'
         elif self.semver_label == 'patch':
             patch = str(int(patch) + 1)
         self.new_version = '.'.join([major, minor, patch])
-    
+
     def get_github_client(self):
         return self._github
```

### Comparing `gordian-3.7.0/gordian/transformations.py` & `gordian-3.7.1/gordian/transformations.py`

 * *Files identical despite different names*

### Comparing `gordian-3.7.0/gordian.egg-info/PKG-INFO` & `gordian-3.7.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: gordian
-Version: 3.7.0
-Summary: A tool to search and replace files in a Git repo
-Home-page: https://github.com/argoproj-labs/gordian
-Author: Intuit
-Author-email: cg-sre@intuit.com
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 <div align="center">
 <img width="200"
 src=".github/gordian-logo.png">
 </div>
 
 Gordian
 ========
@@ -169,15 +158,15 @@
 The `GIT_PASSWORD` or `password=` may also contain a Personal Access Token instead of the account password.
 
 # Development
 The simplest way to hit the ground running if you want to contribute with code is using docker.
 
 Launch a python container
 ```shell
-localhost$ docker run --rm -it  -v $(pwd):$(pwd) -w $(pwd) python:3.7-stretch bash
+localhost$ docker run --rm -it  -v $(pwd):$(pwd) -w $(pwd)  python:3.11-slim-bullseye bash
 ```
 
 Install the project and test dependencies in developer mode
 ```shell
 container# pip install -e .[test]
 ```
```

### Comparing `gordian-3.7.0/gordian.egg-info/SOURCES.txt` & `gordian-3.7.1/gordian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gordian-3.7.0/setup.py` & `gordian-3.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup_reqs = ["pytest", "pytest-cov", "pytest-runner", "flake8"]
 setuptools.setup(
     name="gordian",
-    version="3.7.0",
+    version="3.7.1",
     author="Intuit",
     author_email="cg-sre@intuit.com",
     description="A tool to search and replace files in a Git repo",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/argoproj-labs/gordian",
     install_requires=["pygithub<2.0.0", "pyyaml", "jsonpatch", "deepdiff", "retry"],
```

### Comparing `gordian-3.7.0/tests/test_base_file.py` & `gordian-3.7.1/tests/test_base_file.py`

 * *Files identical despite different names*

### Comparing `gordian-3.7.0/tests/test_changelog_file.py` & `gordian-3.7.1/tests/test_changelog_file.py`

 * *Files identical despite different names*

### Comparing `gordian-3.7.0/tests/test_gordian.py` & `gordian-3.7.1/tests/test_gordian.py`

 * *Files identical despite different names*

### Comparing `gordian-3.7.0/tests/test_parser.py` & `gordian-3.7.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `gordian-3.7.0/tests/test_repo.py` & `gordian-3.7.1/tests/test_repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,7 +202,27 @@
         self.assertEquals(self.repo.files, [repository_file])
 
     def test__get_github_client(self):
         repo = Repo('test_repo', branch='', github=self.mock_git)
 
         self.assertIsNotNone(repo.get_github_client())
         self.assertEqual(repo.get_github_client(), self.mock_git)
+    
+    def test_get_repo_contents_timeout_error(self):
+        self.repo._set_target_branch('target')
+        self.repo.files = []
+        self.repo._source_repo = MagicMock()
+        self.repo._source_repo.get_contents.side_effect = TimeoutError('Read Timeout')
+        with pytest.raises(Exception) as context:
+            self.repo._get_repo_contents(path='test/afile.txt')
+        assert "Read Timeout" in str(context.value)
+        self.repo._source_repo.get_contents.assert_has_calls([call('test/afile.txt', 'target'), call('test/afile.txt', 'target'), call('test/afile.txt', 'target')])
+
+    
+    def test_get_repo_contents(self):
+        self.repo._set_target_branch('target')
+        self.repo.files = []
+        self.repo._source_repo = MagicMock()
+        repository_file = MagicMock(path='test/afile.txt', type='not_dir')
+        self.repo._source_repo.get_contents.side_effect = [repository_file]
+        self.repo._get_repo_contents(path='test/afile.txt')
+        self.repo._source_repo.get_contents.assert_has_calls([call('test/afile.txt', 'target')])
```

### Comparing `gordian-3.7.0/tests/test_transformations.py` & `gordian-3.7.1/tests/test_transformations.py`

 * *Files identical despite different names*

