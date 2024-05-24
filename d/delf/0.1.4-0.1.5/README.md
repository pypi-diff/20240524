# Comparing `tmp/delf-0.1.4.tar.gz` & `tmp/delf-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delf-0.1.4.tar", max compression
+gzip compressed data, was "delf-0.1.5.tar", max compression
```

## Comparing `delf-0.1.4.tar` & `delf-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35147 2022-03-03 04:30:48.399678 delf-0.1.4/LICENSE
--rw-r--r--   0        0        0     2595 2023-12-04 22:57:37.645182 delf-0.1.4/README.md
--rw-r--r--   0        0        0      672 2024-05-09 22:10:08.702014 delf-0.1.4/pyproject.toml
--rwxr-xr-x   0        0        0    74409 2023-10-22 15:01:59.198220 delf-0.1.4/src/delf.py
--rw-r--r--   0        0        0     3350 1970-01-01 00:00:00.000000 delf-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35147 2022-03-03 04:30:48.399678 delf-0.1.5/LICENSE
+-rw-r--r--   0        0        0    10125 2024-05-24 15:09:17.786521 delf-0.1.5/README.md
+-rw-r--r--   0        0        0      678 2024-05-24 15:22:53.232721 delf-0.1.5/pyproject.toml
+-rwxr-xr-x   0        0        0    74409 2023-10-22 15:01:59.198220 delf-0.1.5/src/delf.py
+-rw-r--r--   0        0        0    10679 1970-01-01 00:00:00.000000 delf-0.1.5/PKG-INFO
```

### Comparing `delf-0.1.4/LICENSE` & `delf-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `delf-0.1.4/pyproject.toml` & `delf-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [tool.poetry]
 name = "delf"
-version = "0.1.4"
+version = "0.1.5"
 description = "yet another elf dump tool"
 authors = ["terminaldweller <devi@terminaldweller.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 keywords = ["elf", "capstone"]
 classifiers = [
     "Environment :: Console",
 ]
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.12"
 capstone = "^4.0.2"
 setuptools = "^69.5.1"
 
 [tool.poetry.scripts]
 delf = "delf:main"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.6.1"
 pylint = "^3.0.2"
 bandit = "^1.7.5"
 ruff = "^0.1.1"
-black = "^23.10.0"
+black = ">=23.10,<25.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `delf-0.1.4/src/delf.py` & `delf-0.1.5/src/delf.py`

 * *Files identical despite different names*

