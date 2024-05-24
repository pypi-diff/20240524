# Comparing `tmp/giphon-0.1.8.tar.gz` & `tmp/giphon-0.2.0.tar.gz`

## Comparing `giphon-0.1.8.tar` & `giphon-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 giphon-0.1.8/src/giphon/__about__.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 giphon-0.1.8/src/giphon/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 giphon-0.1.8/src/giphon/__main__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 giphon-0.1.8/src/giphon/git.py
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 giphon-0.1.8/src/giphon/gitlab.py
--rw-r--r--   0        0        0     7234 2020-02-02 00:00:00.000000 giphon-0.1.8/src/giphon/siphon.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 giphon-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 giphon-0.1.8/tests/test_git.py
--rw-r--r--   0        0        0    10343 2020-02-02 00:00:00.000000 giphon-0.1.8/tests/test_gitlab.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 giphon-0.1.8/tests/test_siphon.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 giphon-0.1.8/tests/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 giphon-0.1.8/.gitignore
--rw-r--r--   0        0        0    10933 2020-02-02 00:00:00.000000 giphon-0.1.8/LICENSE
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 giphon-0.1.8/README.md
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 giphon-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 giphon-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 giphon-0.2.0/src/giphon/__about__.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 giphon-0.2.0/src/giphon/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 giphon-0.2.0/src/giphon/__main__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 giphon-0.2.0/src/giphon/envvars.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 giphon-0.2.0/src/giphon/git.py
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 giphon-0.2.0/src/giphon/gitlab.py
+-rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 giphon-0.2.0/src/giphon/siphon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 giphon-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 giphon-0.2.0/tests/test_envvars.py
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 giphon-0.2.0/tests/test_git.py
+-rw-r--r--   0        0        0    10361 2020-02-02 00:00:00.000000 giphon-0.2.0/tests/test_gitlab.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 giphon-0.2.0/tests/test_siphon.py
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 giphon-0.2.0/tests/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 giphon-0.2.0/.gitignore
+-rw-r--r--   0        0        0    10933 2020-02-02 00:00:00.000000 giphon-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 giphon-0.2.0/README.md
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 giphon-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 giphon-0.2.0/PKG-INFO
```

### Comparing `giphon-0.1.8/src/giphon/git.py` & `giphon-0.2.0/src/giphon/git.py`

 * *Files identical despite different names*

### Comparing `giphon-0.1.8/src/giphon/gitlab.py` & `giphon-0.2.0/src/giphon/gitlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from logging import Logger
 from pathlib import Path
 from typing import Generator, List, Union
+from urllib.parse import quote_plus
 
 from gitlab import Gitlab
 from gitlab.base import RESTObject
 from gitlab.exceptions import GitlabHttpError, GitlabListError
 from gitlab.v4.objects import Group, GroupVariable, Project, ProjectVariable
 
 Variable = Union[ProjectVariable, GroupVariable]
@@ -21,17 +22,16 @@
         path (Path): the path to save the environment variables to
         element (Union[gitlab.v4.objects.Group, gitlab.v4.objects.Project]):
           The Gitlab group or project to get the environment variables from
         logger (Logger): the logger to use to generate logs
     """
 
     def _save_environment_variable(variable: Variable, env_path: Path) -> None:
-        scope = variable.environment_scope
-
-        key = f'{variable.key}-{scope.replace("*", "STAR").replace("/", "-")}'
+        escaped_scope = quote_plus(variable.environment_scope)
+        key = f"{variable.variable_type}:{variable.key}:{escaped_scope}"
 
         with open(os.path.join(env_path, f"{key}"), "w") as f:
             f.write(variable.value)
 
     gitlab_element_path = os.path.join(
         path, get_gitlab_element_full_path(element)
     )
```

### Comparing `giphon-0.1.8/src/giphon/siphon.py` & `giphon-0.2.0/src/giphon/siphon.py`

 * *Files 9% similar despite different names*

```diff
@@ -102,35 +102,14 @@
 ) -> None:
     """
     Siphon contents from a Gitlab instance or group.
 
     This function traverses recursively a Gitlab instance or group in order to
     copy locally all of the project's repositories and their environment
     variables, while keeping the arborescence.
-
-    Args:
-        namespace (Path): The Gitlab namespace to recusively siphon.
-          Use `/` to siphon the instance.
-        output (Path): The target path to clone the repositories to.", ).
-        gitlab_token (str): The Personal Access Token for the Gitlab v4 API."
-        gitlab_url (str): The URL for the Gitlab Instance. Defaults to
-          "https://gitlab.com".
-        fetch_repositories (bool, optional): Whether to fetch remotes on
-          repositories that already exist. Defaults to True.
-        save_ci_variables (bool, optional): Whether to download CI/CD
-          variables to a .env directory.. Defaults to True.
-        clone_archived (bool, optional): Whether to clone archived repository.
-          Defaults to False.
-        clone_through_ssh (bool, optional): Whether to clone using ssh or
-          https.
-        gitlab_username: (str, optional): The username to use when cloning
-          through https.
-        verbose (bool, optional): Whether the outputs should be verbose.
-          Defaults to False.
-
     """
     logger = _setup_logger(
         __name__, logging.INFO if verbose <= 0 else logging.DEBUG
     )
 
     with Progress(
         SpinnerColumn(),
```

### Comparing `giphon-0.1.8/tests/test_git.py` & `giphon-0.2.0/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `giphon-0.1.8/tests/test_gitlab.py` & `giphon-0.2.0/tests/test_gitlab.py`

 * *Files 4% similar despite different names*

```diff
@@ -277,21 +277,21 @@
 
         output = no_error_output.getvalue()
         # Test the stdout of the function
 
         assert output == (
             "Would have made the path random_path/the_group/.gitlab/.env\n"
             "Entered mock open with args ('random_path/the_group/.gitlab/.env/"
-            "ipsum-lorem', 'w') and kwargs {}\n"
+            "file:ipsum:lorem', 'w') and kwargs {}\n"
             "Would have written dolor\n"
             "Entered mock open with args ('random_path/the_group/.gitlab/.env/"
-            "ipsum-lorem', 'w') and kwargs {}\n"
+            "env_var:ipsum:lorem', 'w') and kwargs {}\n"
             "Would have written dolor\n"
             "Entered mock open with args ('random_path/the_group/.gitlab/.env/"
-            "ipsum-lorem', 'w') and kwargs {}\n"
+            "file:ipsum:lorem', 'w') and kwargs {}\n"
             "Would have written dolor\n"
         )
 
     # Monkeypatch group with variables, but listing variables raises an
     # exception
     with monkeypatch.context() as m:
         m.setattr(
```

### Comparing `giphon-0.1.8/tests/test_siphon.py` & `giphon-0.2.0/tests/test_siphon.py`

 * *Files identical despite different names*

### Comparing `giphon-0.1.8/tests/utils.py` & `giphon-0.2.0/tests/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -127,18 +127,19 @@
         )
         self.list_must_error = list_must_error
 
     def list(self, *args, **kwargs):
         if self.list_must_error:
             raise GitlabListError
         return [
-            _MockGitlabVariable(),
-            _MockGitlabVariable(),
-            _MockGitlabVariable(),
+            _MockGitlabVariable(variable_type="file"),
+            _MockGitlabVariable(variable_type="env_var"),
+            _MockGitlabVariable(variable_type="file"),
         ]
 
 
 class _MockGitlabVariable:
-    def __init__(self, *args, **kwargs):
+    def __init__(self, variable_type: str, *args, **kwargs):
         self.environment_scope = "lorem"
         self.key = "ipsum"
         self.value = "dolor"
+        self.variable_type = variable_type
```

### Comparing `giphon-0.1.8/.gitignore` & `giphon-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `giphon-0.1.8/LICENSE` & `giphon-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `giphon-0.1.8/README.md` & `giphon-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Logo](https://raw.githubusercontent.com/kabooboo/giphon/0.1.8/docs/assets/logo.png)
+![Logo](https://raw.githubusercontent.com/kabooboo/giphon/0.2.0/docs/assets/logo.png)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/giphon) [![Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://pypi.org/project/black/) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/kabooboo/giphon/test.yml?label=tests)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) ![PyPI](https://img.shields.io/pypi/v/giphon) ![PyPI - License](https://img.shields.io/pypi/l/giphon) ![GitHub Repo stars](https://img.shields.io/github/stars/kabooboo/giphon?style=social)
 
 ---
 
 ✨ Giphon is the contraction of 🦊 _Gitlab_ and 🫗 _siphon_. This CLI tools allows users
 to recursively clone all projects in a given Gitlab group or instance.
@@ -13,15 +13,15 @@
 structure into a directory structure.
 
 Locally cloned projects enable users to use familiar CLI tools such as `grep`
 and `sed` directly into the projects' tree structure.
 
 ## Demo
 
-![Usage GIF](https://raw.githubusercontent.com/kabooboo/giphon/0.1.8/docs/assets/usage.gif)
+![Usage GIF](https://raw.githubusercontent.com/kabooboo/giphon/0.2.0/docs/assets/usage.gif)
 
 ## Installation
 
 To install `giphon`, simply run:
 
 ```sh
 pip install --user giphon
```

### Comparing `giphon-0.1.8/pyproject.toml` & `giphon-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
 ]
 dependencies = [
   "typer>=0.7",
-  "python-gitlab>=3,<4",
+  "python-gitlab>=3,<5",
   "GitPython>=3,<4",
   "rich>=12,<14",
 ]
 description = "Copy locally a Gitlab group or instance"
 dynamic = ["version"]
 keywords = [
   "gitlab",
```

### Comparing `giphon-0.1.8/PKG-INFO` & `giphon-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: giphon
-Version: 0.1.8
+Version: 0.2.0
 Summary: Copy locally a Gitlab group or instance
 Project-URL: Bug Reports, https://github.com/kabooboo/giphon/issues
 Project-URL: Documentation, https://github.com/kabooboo/giphon
 Project-URL: Homepage, https://github.com/kabooboo/giphon
 Project-URL: Source Code, https://github.com/kabooboo/giphon
 Author-email: Gabriel Creti <gabrielcreti@gmail.com>
 License-File: LICENSE
@@ -19,22 +19,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.7
 Requires-Dist: gitpython<4,>=3
-Requires-Dist: python-gitlab<4,>=3
+Requires-Dist: python-gitlab<5,>=3
 Requires-Dist: rich<14,>=12
 Requires-Dist: typer>=0.7
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
-![Logo](https://raw.githubusercontent.com/kabooboo/giphon/0.1.8/docs/assets/logo.png)
+![Logo](https://raw.githubusercontent.com/kabooboo/giphon/0.2.0/docs/assets/logo.png)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/giphon) [![Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://pypi.org/project/black/) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/kabooboo/giphon/test.yml?label=tests)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) ![PyPI](https://img.shields.io/pypi/v/giphon) ![PyPI - License](https://img.shields.io/pypi/l/giphon) ![GitHub Repo stars](https://img.shields.io/github/stars/kabooboo/giphon?style=social)
 
 ---
 
 ✨ Giphon is the contraction of 🦊 _Gitlab_ and 🫗 _siphon_. This CLI tools allows users
 to recursively clone all projects in a given Gitlab group or instance.
@@ -45,15 +45,15 @@
 structure into a directory structure.
 
 Locally cloned projects enable users to use familiar CLI tools such as `grep`
 and `sed` directly into the projects' tree structure.
 
 ## Demo
 
-![Usage GIF](https://raw.githubusercontent.com/kabooboo/giphon/0.1.8/docs/assets/usage.gif)
+![Usage GIF](https://raw.githubusercontent.com/kabooboo/giphon/0.2.0/docs/assets/usage.gif)
 
 ## Installation
 
 To install `giphon`, simply run:
 
 ```sh
 pip install --user giphon
```

