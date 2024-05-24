# Comparing `tmp/commitlint-0.2.1.tar.gz` & `tmp/commitlint-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitlint-0.2.1.tar", last modified: Thu Feb  1 12:33:22 2024, max compression
+gzip compressed data, was "commitlint-1.0.0.tar", last modified: Fri May 24 16:07:34 2024, max compression
```

## Comparing `commitlint-0.2.1.tar` & `commitlint-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,33 @@
-drwxr-xr-x   0 aj3sh      (501) staff       (20)        0 2024-02-01 12:33:22.106002 commitlint-0.2.1/
--rw-r--r--   0 aj3sh      (501) staff       (20)    35149 2024-01-12 10:01:39.000000 commitlint-0.2.1/LICENSE
--rw-r--r--   0 aj3sh      (501) staff       (20)     2958 2024-02-01 12:33:22.105927 commitlint-0.2.1/PKG-INFO
--rw-r--r--   0 aj3sh      (501) staff       (20)     2146 2024-02-01 12:31:39.000000 commitlint-0.2.1/README.md
--rw-r--r--   0 aj3sh      (501) staff       (20)       90 2024-01-23 16:35:28.000000 commitlint-0.2.1/pyproject.toml
--rw-r--r--   0 aj3sh      (501) staff       (20)     1021 2024-02-01 12:33:22.106327 commitlint-0.2.1/setup.cfg
-drwxr-xr-x   0 aj3sh      (501) staff       (20)        0 2024-02-01 12:33:22.101059 commitlint-0.2.1/src/
-drwxr-xr-x   0 aj3sh      (501) staff       (20)        0 2024-02-01 12:33:22.104021 commitlint-0.2.1/src/commitlint/
--rw-r--r--   0 aj3sh      (501) staff       (20)      114 2024-01-23 16:35:28.000000 commitlint-0.2.1/src/commitlint/__init__.py
--rw-r--r--   0 aj3sh      (501) staff       (20)     5039 2024-01-28 10:37:48.000000 commitlint-0.2.1/src/commitlint/cli.py
--rw-r--r--   0 aj3sh      (501) staff       (20)     3516 2024-01-28 10:34:14.000000 commitlint-0.2.1/src/commitlint/commitlint.py
--rw-r--r--   0 aj3sh      (501) staff       (20)      100 2024-01-23 16:35:28.000000 commitlint-0.2.1/src/commitlint/constants.py
--rw-r--r--   0 aj3sh      (501) staff       (20)      451 2024-01-23 16:35:28.000000 commitlint-0.2.1/src/commitlint/exceptions.py
--rw-r--r--   0 aj3sh      (501) staff       (20)     3136 2024-01-28 10:37:48.000000 commitlint-0.2.1/src/commitlint/git_helpers.py
--rw-r--r--   0 aj3sh      (501) staff       (20)      719 2024-01-23 16:35:29.000000 commitlint-0.2.1/src/commitlint/messages.py
-drwxr-xr-x   0 aj3sh      (501) staff       (20)        0 2024-02-01 12:33:22.105698 commitlint-0.2.1/src/commitlint.egg-info/
--rw-r--r--   0 aj3sh      (501) staff       (20)     2958 2024-02-01 12:33:22.000000 commitlint-0.2.1/src/commitlint.egg-info/PKG-INFO
--rw-r--r--   0 aj3sh      (501) staff       (20)      471 2024-02-01 12:33:22.000000 commitlint-0.2.1/src/commitlint.egg-info/SOURCES.txt
--rw-r--r--   0 aj3sh      (501) staff       (20)        1 2024-02-01 12:33:22.000000 commitlint-0.2.1/src/commitlint.egg-info/dependency_links.txt
--rw-r--r--   0 aj3sh      (501) staff       (20)       51 2024-02-01 12:33:22.000000 commitlint-0.2.1/src/commitlint.egg-info/entry_points.txt
--rw-r--r--   0 aj3sh      (501) staff       (20)       11 2024-02-01 12:33:22.000000 commitlint-0.2.1/src/commitlint.egg-info/top_level.txt
-drwxr-xr-x   0 aj3sh      (501) staff       (20)        0 2024-02-01 12:33:22.105388 commitlint-0.2.1/tests/
--rw-r--r--   0 aj3sh      (501) staff       (20)     7648 2024-01-23 16:35:29.000000 commitlint-0.2.1/tests/test_cli.py
--rw-r--r--   0 aj3sh      (501) staff       (20)     3009 2024-01-23 16:35:29.000000 commitlint-0.2.1/tests/test_git_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:07:34.897770 commitlint-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-24 16:07:26.000000 commitlint-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-24 16:07:34.897770 commitlint-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-24 16:07:26.000000 commitlint-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-24 16:07:26.000000 commitlint-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-24 16:07:34.897770 commitlint-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:07:34.893770 commitlint-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:07:34.897770 commitlint-1.0.0/src/commitlint/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-24 16:07:26.000000 commitlint-1.0.0/src/commitlint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-24 16:07:26.000000 commitlint-1.0.0/src/commitlint/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-05-24 16:07:26.000000 commitlint-1.0.0/src/commitlint/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-24 16:07:26.000000 commitlint-1.0.0/src/commitlint/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-24 16:07:26.000000 commitlint-1.0.0/src/commitlint/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-24 16:07:26.000000 commitlint-1.0.0/src/commitlint/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-24 16:07:26.000000 commitlint-1.0.0/src/commitlint/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-24 16:07:26.000000 commitlint-1.0.0/src/commitlint/git_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:07:34.897770 commitlint-1.0.0/src/commitlint/linter/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-24 16:07:26.000000 commitlint-1.0.0/src/commitlint/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-24 16:07:26.000000 commitlint-1.0.0/src/commitlint/linter/_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-24 16:07:26.000000 commitlint-1.0.0/src/commitlint/linter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-24 16:07:26.000000 commitlint-1.0.0/src/commitlint/linter/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-24 16:07:26.000000 commitlint-1.0.0/src/commitlint/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:07:34.897770 commitlint-1.0.0/src/commitlint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-24 16:07:34.000000 commitlint-1.0.0/src/commitlint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-24 16:07:34.000000 commitlint-1.0.0/src/commitlint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:07:34.000000 commitlint-1.0.0/src/commitlint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-24 16:07:34.000000 commitlint-1.0.0/src/commitlint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 16:07:34.000000 commitlint-1.0.0/src/commitlint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:07:34.897770 commitlint-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-05-24 16:07:26.000000 commitlint-1.0.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-24 16:07:26.000000 commitlint-1.0.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-24 16:07:26.000000 commitlint-1.0.0/tests/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-24 16:07:26.000000 commitlint-1.0.0/tests/test_git_helpers.py
```

### Comparing `commitlint-0.2.1/LICENSE` & `commitlint-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commitlint-0.2.1/setup.cfg` & `commitlint-1.0.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = commitlint
-version = 0.2.1
-license = MIT
+version = attr: commitlint.__version__.__version__
+license = GPL-3.0
 author = opensource-nepal
 author_email = aj3sshh@gmail.com, sugatbajracharya49@gmail.com
 description = commitlint is is a pre-commit hook designed to lint your commit messages according to the Conventional Commits standard.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = 
 	commitlint
```

### Comparing `commitlint-0.2.1/tests/test_git_helpers.py` & `commitlint-1.0.0/tests/test_git_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # type: ignore
 # pylint: disable=all
 import subprocess
 from unittest.mock import patch
 
 import pytest
 
-from src.commitlint.exceptions import (
+from commitlint.exceptions import (
     GitCommitNotFoundException,
     GitInvalidCommitRangeException,
 )
-from src.commitlint.git_helpers import (
+from commitlint.git_helpers import (
     get_commit_message_of_hash,
     get_commit_messages_of_hash_range,
 )
 
 DELIMITER = "========commit-delimiter========"
 
 
 @pytest.fixture
 def mock_subprocess():
-    with patch("src.commitlint.git_helpers.subprocess") as mock_subprocess:
+    with patch("commitlint.git_helpers.subprocess") as mock_subprocess:
         mock_subprocess.PIPE = subprocess.PIPE
         mock_subprocess.CalledProcessError = subprocess.CalledProcessError
         yield mock_subprocess
 
 
 def test_get_commit_message_of_hash_success(mock_subprocess):
     hash_value = "abc123"
@@ -48,15 +48,15 @@
     )
 
     with pytest.raises(GitCommitNotFoundException):
         get_commit_message_of_hash(hash_value)
 
 
 @patch(
-    "src.commitlint.git_helpers.get_commit_message_of_hash",
+    "commitlint.git_helpers.get_commit_message_of_hash",
     return_value="From commit message",
 )
 def test_get_commit_messages_of_hash_range_success(
     _mock_get_commit_message_of_hash, mock_subprocess
 ):
     from_hash = "abc123"
     to_hash = "def456"
@@ -78,15 +78,15 @@
         ],
         text=True,
         stderr=subprocess.PIPE,
     )
 
 
 @patch(
-    "src.commitlint.git_helpers.get_commit_message_of_hash",
+    "commitlint.git_helpers.get_commit_message_of_hash",
     return_value="From commit message",
 )
 def test_get_commit_messages_of_hash_range_failure(
     _mock_get_commit_message_of_hash, mock_subprocess
 ):
     from_hash = "invalid_hash"
     to_hash = "def456"
```

