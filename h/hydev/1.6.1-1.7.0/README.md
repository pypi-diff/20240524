# Comparing `tmp/hydev-1.6.1.tar.gz` & `tmp/hydev-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydev-1.6.1.tar", max compression
+gzip compressed data, was "hydev-1.7.0.tar", max compression
```

## Comparing `hydev-1.6.1.tar` & `hydev-1.7.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      252 2024-05-01 07:45:10.622666 hydev-1.6.1/LICENSE
--rw-r--r--   0        0        0     2525 2024-05-17 09:00:35.471316 hydev-1.6.1/pyproject.toml
--rw-r--r--   0        0        0       35 2024-05-01 07:45:10.622666 hydev-1.6.1/src/hydev/__init__.py
--rw-r--r--   0        0        0     2042 2024-05-17 08:58:47.890790 hydev-1.6.1/src/hydev/common_pyproject.toml
--rw-r--r--   0        0        0     7919 2024-05-06 08:56:45.854405 hydev-1.6.1/src/hydev/main.py
--rw-r--r--   0        0        0     2888 2024-05-01 08:00:36.151190 hydev-1.6.1/src/hydev/utils.py
--rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 hydev-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0      252 2024-05-01 07:45:10.622666 hydev-1.7.0/LICENSE
+-rw-r--r--   0        0        0     2551 2024-05-24 11:25:00.097518 hydev-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-05-01 07:45:10.622666 hydev-1.7.0/src/hydev/__init__.py
+-rw-r--r--   0        0        0     2042 2024-05-17 08:58:47.890790 hydev-1.7.0/src/hydev/common_pyproject.toml
+-rw-r--r--   0        0        0     7919 2024-05-06 08:56:45.854405 hydev-1.7.0/src/hydev/main.py
+-rw-r--r--   0        0        0     2888 2024-05-01 08:00:36.151190 hydev-1.7.0/src/hydev/utils.py
+-rw-r--r--   0        0        0     2365 1970-01-01 00:00:00.000000 hydev-1.7.0/PKG-INFO
```

### Comparing `hydev-1.6.1/pyproject.toml` & `hydev-1.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hydev"
-version = "1.6.1"
+version = "1.7.0"
 description = "Common tooling and configuration for pythonic development"
 authors = ["hoverhell <hoverhell@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.scripts]
 hydautoflake = "hydev.main:Autoflake.run_cli"
 hydblack = "hydev.main:Black.run_cli"
@@ -20,35 +20,35 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 # Libs
 click = "^8.1.7"
 pyyaml = "^6.0.1"
 toml = "^0.10.2"
 # Tooling
-poetry = "^1.8.2"
-pre-commit = "^3.7.0"
+poetry = "^1.8.3"
+pre-commit = "^3.7.1"
 # Debug conveniences
 coloredlogs = "^15.0.1"
 ipdb = "^0.13.13"
 # Formatting
 autoflake = "^2.3.1"
 black = "^24.4.2"
 isort = "^5.13.2"
 # `flake8`
-flake8 = "^6.1.0"
+flake8 = "^7.0.0"
 flake8-broken-line = "^1.0.0"
 flake8-debugger = "^4.1.2"
 flake8-mock-x2 = "^0.4.1"
 flake8-print = "^5.0.0"
 flake8-pytest-style = "^2.0.0"
 flake8-use-fstring = "^1.4"
 # `mypy`
 mypy = "^1.10.0"
 # `pytest`
-pytest = "^8.2.0"
+pytest = "^8.2.1"
 pytest-asyncio = "^0.23.2"
 pytest-blockage = "^0.2.4"
 pytest-cov = "^5.0.0"
 pytest-deadfixtures = "^2.2.1"
 pytest-env = "^1.1.3"
 pytest-timeout = "^2.3.1"
 # `django`
@@ -57,15 +57,15 @@
 django-extra-checks = {version = "^0.13.3", optional = true}
 django-migration-linter = {version = "^5.1.0", optional = true}
 django-querycount = {version = "^0.8.3", optional = true}
 django-split-settings = {version = "^1.3.1", optional = true}
 django-stubs = {version = "^5.0.0", optional = true}
 django-stubs-ext = {version = "^5.0.0", optional = true}
 django-test-migrations = {version = "^1.3.0", optional = true}
-flake8-django = {version = "^1.4", optional = true}
+flake8-django-hhupd = {version = "^1.4.1", optional = true}
 pytest-django = {version = "^4.8.0", optional = true}
 # ...
 poetry-plugin-up = "^0.7.1"
 
 [tool.poetry.extras]
 django = [
     "django-coverage-plugin",
@@ -73,19 +73,19 @@
     "django-extra-checks",
     "django-migration-linter",
     "django-querycount",
     "django-split-settings",
     "django-stubs",
     "django-stubs-ext",
     "django-test-migrations",
-    "flake8-django",
+    "flake8-django-hhupd",
     "pytest-django",
 ]
 
 [tool.poetry.group.dev.dependencies]
 types-toml = "^0.10.8.7"
-types-requests = "^2.31.0.10"
-types-pyyaml = "^6.0.12.12"
+types-requests = "^2.32.0.20240523"
+types-pyyaml = "^6.0.12.20240311"
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hydev-1.6.1/src/hydev/common_pyproject.toml` & `hydev-1.7.0/src/hydev/common_pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydev-1.6.1/src/hydev/main.py` & `hydev-1.7.0/src/hydev/main.py`

 * *Files identical despite different names*

### Comparing `hydev-1.6.1/src/hydev/utils.py` & `hydev-1.7.0/src/hydev/utils.py`

 * *Files identical despite different names*

### Comparing `hydev-1.6.1/PKG-INFO` & `hydev-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydev
-Version: 1.6.1
+Version: 1.7.0
 Summary: Common tooling and configuration for pythonic development
 License: MIT
 Author: hoverhell
 Author-email: hoverhell@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,29 +20,29 @@
 Requires-Dist: django-extra-checks (>=0.13.3,<0.14.0) ; extra == "django"
 Requires-Dist: django-migration-linter (>=5.1.0,<6.0.0) ; extra == "django"
 Requires-Dist: django-querycount (>=0.8.3,<0.9.0) ; extra == "django"
 Requires-Dist: django-split-settings (>=1.3.1,<2.0.0) ; extra == "django"
 Requires-Dist: django-stubs (>=5.0.0,<6.0.0) ; extra == "django"
 Requires-Dist: django-stubs-ext (>=5.0.0,<6.0.0) ; extra == "django"
 Requires-Dist: django-test-migrations (>=1.3.0,<2.0.0) ; extra == "django"
-Requires-Dist: flake8 (>=6.1.0,<7.0.0)
+Requires-Dist: flake8 (>=7.0.0,<8.0.0)
 Requires-Dist: flake8-broken-line (>=1.0.0,<2.0.0)
 Requires-Dist: flake8-debugger (>=4.1.2,<5.0.0)
-Requires-Dist: flake8-django (>=1.4,<2.0) ; extra == "django"
+Requires-Dist: flake8-django-hhupd (>=1.4.1,<2.0.0) ; extra == "django"
 Requires-Dist: flake8-mock-x2 (>=0.4.1,<0.5.0)
 Requires-Dist: flake8-print (>=5.0.0,<6.0.0)
 Requires-Dist: flake8-pytest-style (>=2.0.0,<3.0.0)
 Requires-Dist: flake8-use-fstring (>=1.4,<2.0)
 Requires-Dist: ipdb (>=0.13.13,<0.14.0)
 Requires-Dist: isort (>=5.13.2,<6.0.0)
 Requires-Dist: mypy (>=1.10.0,<2.0.0)
-Requires-Dist: poetry (>=1.8.2,<2.0.0)
+Requires-Dist: poetry (>=1.8.3,<2.0.0)
 Requires-Dist: poetry-plugin-up (>=0.7.1,<0.8.0)
-Requires-Dist: pre-commit (>=3.7.0,<4.0.0)
-Requires-Dist: pytest (>=8.2.0,<9.0.0)
+Requires-Dist: pre-commit (>=3.7.1,<4.0.0)
+Requires-Dist: pytest (>=8.2.1,<9.0.0)
 Requires-Dist: pytest-asyncio (>=0.23.2,<0.24.0)
 Requires-Dist: pytest-blockage (>=0.2.4,<0.3.0)
 Requires-Dist: pytest-cov (>=5.0.0,<6.0.0)
 Requires-Dist: pytest-deadfixtures (>=2.2.1,<3.0.0)
 Requires-Dist: pytest-django (>=4.8.0,<5.0.0) ; extra == "django"
 Requires-Dist: pytest-env (>=1.1.3,<2.0.0)
 Requires-Dist: pytest-timeout (>=2.3.1,<3.0.0)
```

