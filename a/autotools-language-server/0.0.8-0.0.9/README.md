# Comparing `tmp/autotools-language-server-0.0.8.tar.gz` & `tmp/autotools_language_server-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotools-language-server-0.0.8.tar", last modified: Tue Aug 29 08:44:53 2023, max compression
+gzip compressed data, was "autotools_language_server-0.0.9.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `autotools-language-server-0.0.8.tar` & `autotools_language_server-0.0.9.tar`

### file list

```diff
@@ -1,65 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.927182 autotools-language-server-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.919182 autotools-language-server-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (999)      336 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.923182 autotools-language-server-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)     2853 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (999)      631 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/.github/workflows/nix.yml
--rw-r--r--   0 runner    (1001) docker     (999)     2021 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (999)      101 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/.gitlint
--rw-r--r--   0 runner    (1001) docker     (999)     2870 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      211 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (999)      157 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (999)    35149 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     7445 2023-08-29 08:44:53.927182 autotools-language-server-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     5935 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.923182 autotools-language-server-0.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.923182 autotools-language-server-0.0.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (999)      110 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/docs/api/autotools-language-server.md
--rw-r--r--   0 runner    (1001) docker     (999)     2083 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (999)      299 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (999)       70 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.923182 autotools-language-server-0.0.8/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (999)     1776 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (999)     1003 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (999)       94 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/docs/resources/requirements.md
--rw-r--r--   0 runner    (1001) docker     (999)     1006 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/flake.nix
--rw-r--r--   0 runner    (1001) docker     (999)     2968 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.923182 autotools-language-server-0.0.8/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (999)       90 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (999)       53 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.923182 autotools-language-server-0.0.8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (999)      203 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/scripts/generate-api.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (999)      254 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/scripts/generate-requirements.md.pl
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.923182 autotools-language-server-0.0.8/sdist/
--rw-r--r--   0 runner    (1001) docker     (999)     1268 2023-08-29 08:44:53.000000 autotools-language-server-0.0.8/sdist/_autotools-language-server
--rw-r--r--   0 runner    (1001) docker     (999)     4082 2023-08-29 08:44:53.000000 autotools-language-server-0.0.8/sdist/autotools-language-server
--rw-r--r--   0 runner    (1001) docker     (999)      452 2023-08-29 08:44:53.000000 autotools-language-server-0.0.8/sdist/autotools-language-server.1
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-29 08:44:53.927182 autotools-language-server-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.919182 autotools-language-server-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.923182 autotools-language-server-0.0.8/src/autotools_language_server/
--rw-r--r--   0 runner    (1001) docker     (999)      403 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/src/autotools_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1089 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/src/autotools_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (999)      608 2023-08-29 08:44:53.000000 autotools-language-server-0.0.8/src/autotools_language_server/_metainfo.py
--rw-r--r--   0 runner    (1001) docker     (999)      160 2023-08-29 08:44:53.000000 autotools-language-server-0.0.8/src/autotools_language_server/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.923182 autotools-language-server-0.0.8/src/autotools_language_server/api/
--rw-r--r--   0 runner    (1001) docker     (999)      422 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/src/autotools_language_server/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3513 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/src/autotools_language_server/api/autoconf.py
--rw-r--r--   0 runner    (1001) docker     (999)     2510 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/src/autotools_language_server/api/make.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.919182 autotools-language-server-0.0.8/src/autotools_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.923182 autotools-language-server-0.0.8/src/autotools_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (999)   444789 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/src/autotools_language_server/assets/json/autotools.json
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/src/autotools_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (999)     6222 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/src/autotools_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.923182 autotools-language-server-0.0.8/src/autotools_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     7445 2023-08-29 08:44:53.000000 autotools-language-server-0.0.8/src/autotools_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1402 2023-08-29 08:44:53.000000 autotools-language-server-0.0.8/src/autotools_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-29 08:44:53.000000 autotools-language-server-0.0.8/src/autotools_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       86 2023-08-29 08:44:53.000000 autotools-language-server-0.0.8/src/autotools_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)       37 2023-08-29 08:44:53.000000 autotools-language-server-0.0.8/src/autotools_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       26 2023-08-29 08:44:53.000000 autotools-language-server-0.0.8/src/autotools_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.927182 autotools-language-server-0.0.8/templates/
--rw-r--r--   0 runner    (1001) docker     (999)       59 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (999)      273 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (999)       58 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:44:53.927182 autotools-language-server-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (999)      376 2023-08-29 08:44:43.000000 autotools-language-server-0.0.8/tests/server_test.py
+-rw-r--r--   0        0        0       20 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/.cmake-format.yaml
+-rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/.cmakelintrc
+-rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/.github/FUNDING.yml
+-rw-r--r--   0        0        0     2702 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/.github/workflows/main.yml
+-rw-r--r--   0        0        0     2021 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/.gitignore
+-rwxr-xr-x   0        0        0      101 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/.gitlint
+-rw-r--r--   0        0        0     3005 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      211 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/.readthedocs.yaml
+-rwxr-xr-x   0        0        0      157 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/.yamllint.yaml
+-rw-r--r--   0        0        0      564 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/CMakeLists.txt
+-rw-r--r--   0        0        0    35149 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/LICENSE
+-rw-r--r--   0        0        0     6105 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/README.md
+-rw-r--r--   0        0        0       80 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/docs/api/autotools-language-server.md
+-rw-r--r--   0        0        0     2125 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/docs/conf.py
+-rw-r--r--   0        0        0      299 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/docs/index.md
+-rwxr-xr-x   0        0        0      105 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/docs/requirements.txt
+-rw-r--r--   0        0        0     1776 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/docs/resources/configure.md
+-rw-r--r--   0        0        0      996 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/docs/resources/install.md
+-rw-r--r--   0        0        0      155 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/docs/resources/requirements.md
+-rw-r--r--   0        0        0     3126 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/pyproject.toml
+-rwxr-xr-x   0        0        0       90 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/requirements/dev.txt
+-rwxr-xr-x   0        0        0       65 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      403 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/src/autotools_language_server/__init__.py
+-rw-r--r--   0        0        0     1089 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/src/autotools_language_server/__main__.py
+-rw-r--r--   0        0        0      580 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/src/autotools_language_server/_tree_sitter.py
+-rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/src/autotools_language_server/_version.py
+-rw-r--r--   0        0        0      422 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/src/autotools_language_server/api/__init__.py
+-rw-r--r--   0        0        0     3513 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/src/autotools_language_server/api/autoconf.py
+-rw-r--r--   0        0        0     2510 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/src/autotools_language_server/api/make.py
+-rw-r--r--   0        0        0   444789 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/src/autotools_language_server/assets/json/autotools.json
+-rw-r--r--   0        0        0     2967 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/src/autotools_language_server/diagnostics.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/src/autotools_language_server/py.typed
+-rw-r--r--   0        0        0     8168 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/src/autotools_language_server/server.py
+-rw-r--r--   0        0        0       59 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/templates/class.txt
+-rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/templates/def.txt
+-rw-r--r--   0        0        0      522 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/templates/metainfo.py
+-rw-r--r--   0        0        0       58 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/templates/noarg.txt
+-rwxr-xr-x   0        0        0      137 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/tests/Makefile
+-rw-r--r--   0        0        0       27 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/tests/common.mk
+-rw-r--r--   0        0        0      540 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/tests/diagnostics_test.py
+-rw-r--r--   0        0        0      376 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/tests/server_test.py
+-rw-r--r--   0        0        0     7712 2022-11-09 12:37:21.000000 autotools_language_server-0.0.9/PKG-INFO
```

### Comparing `autotools-language-server-0.0.8/.github/workflows/main.yml` & `autotools_language_server-0.0.9/.github/workflows/main.yml`

 * *Files 16% similar despite different names*

```diff
@@ -11,80 +11,74 @@
   workflow_dispatch:
 
 # https://github.com/softprops/action-gh-release/issues/236
 permissions:
   contents: write
 
 env:
+  CMAKE_GENERATOR: Ninja
   PYTHONUTF8: "1"
   python-version: 3.x
   cache: pip
 
 jobs:
-  test:
+  build-wheels-and-test:
     strategy:
       fail-fast: false
       matrix:
         runs-on:
           - ubuntu-latest
           - macos-latest
-          - windows-latest
-    runs-on: ${{matrix.runs-on}}
+          # OSError: [WinError 193] %1 is not a valid Win32 application
+          # - windows-latest
+    runs-on: ${{ matrix.runs-on }}
     steps:
       - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: docker/setup-qemu-action@v2.2.0
+        if: runner.os == 'Linux'
+      - uses: pypa/cibuildwheel@v2.14.1
+      - uses: actions/upload-artifact@v3
         with:
-          python-version: ${{env.python-version}}
-          cache: ${{env.cache}}
-          cache-dependency-path: |-
-            requirements.txt
-            requirements/dev.txt
-      - name: Install dependencies
-        run: |
-          pip install -e '.[dev]'
-      - name: Test
-        run: |
-          pytest --cov
-      - uses: codecov/codecov-action@v3
+          path: |
+            wheelhouse/*.whl
+
   build:
-    needs: test
-    strategy:
-      fail-fast: false
-      matrix:
-        runs-on:
-          - ubuntu-latest
-          - macos-latest
-          - windows-latest
-    runs-on: ${{matrix.runs-on}}
+    needs:
+      - build-wheels-and-test
+    runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: ${{env.python-version}}
           cache: ${{env.cache}}
           cache-dependency-path: |-
             requirements.txt
             requirements/dev.txt
       - name: Install dependencies
         run: |
           pip install build
-      - name: Build
+      - name: Build sdist
         run: |
-          pyproject-build
+          pyproject-build -s
       - uses: pypa/gh-action-pypi-publish@release/v1
-        if: runner.os == 'Linux' && startsWith(github.ref, 'refs/tags/')
+        if: startsWith(github.ref, 'refs/tags/')
         with:
-          password: ${{secrets.PYPI_API_TOKEN}}
+          password: ${{ secrets.PYPI_API_TOKEN }}
       - uses: actions/upload-artifact@v3
-        if: runner.os == 'Linux' && ! startsWith(github.ref, 'refs/tags/')
+        if: ${{ ! startsWith(github.ref, 'refs/tags/') }}
         with:
           path: |
             dist/*
+      - uses: actions/download-artifact@v3
+        with:
+          name: artifact
+          path: dist
       - uses: softprops/action-gh-release@v1
-        if: runner.os == 'Linux' && startsWith(github.ref, 'refs/tags/')
+        if: startsWith(github.ref, 'refs/tags/')
         with:
           # body_path: build/CHANGELOG.md
           files: |
             dist/*
 
   deploy-aur:
     needs: build
```

### Comparing `autotools-language-server-0.0.8/.gitignore` & `autotools_language_server-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `autotools-language-server-0.0.8/.pre-commit-config.yaml` & `autotools_language_server-0.0.9/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -19,15 +19,15 @@
       - id: debug-statements
       - id: requirements-txt-fixer
       - id: check-xml
       - id: check-yaml
       - id: check-toml
       - id: check-json
   - repo: https://github.com/Lucas-C/pre-commit-hooks
-    rev: v1.5.1
+    rev: v1.5.4
     hooks:
       - id: remove-crlf
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.5
     hooks:
       - id: codespell
         additional_dependencies:
@@ -51,63 +51,68 @@
     hooks:
       - id: actionlint
   - repo: https://github.com/adrienverge/yamllint
     rev: v1.32.0
     hooks:
       - id: yamllint
   - repo: https://github.com/executablebooks/mdformat
-    rev: 0.7.16
+    rev: 0.7.17
     hooks:
       - id: mdformat
         additional_dependencies:
           - mdformat-pyproject
           - mdformat-gfm
           - mdformat-myst
           - mdformat-toc
           - mdformat-deflist
           - mdformat-beautysh
           - mdformat-black
           - mdformat-config
   - repo: https://github.com/DavidAnson/markdownlint-cli2
-    rev: v0.8.1
+    rev: v0.9.2
     hooks:
       - id: markdownlint-cli2
         additional_dependencies:
           - markdown-it-texmath@0.9.1
-  - repo: https://github.com/perltidy/perltidy
-    rev: "20230309.04"
-    hooks:
-      - id: perltidy
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/pycqa/pydocstyle
     rev: 6.3.0
     hooks:
       - id: pydocstyle
         additional_dependencies:
           - tomli
   - repo: https://github.com/kumaraditya303/mirrors-pyright
-    rev: v1.1.316
+    rev: v1.1.325
     hooks:
       - id: pyright
   - repo: https://github.com/PyCQA/bandit
     rev: 1.7.5
     hooks:
       - id: bandit
         args:
           - -cpyproject.toml
         additional_dependencies:
           - tomli
-  - repo: https://github.com/nix-community/nixpkgs-fmt
-    rev: v1.3.0
+  - repo: https://github.com/cmake-lint/cmake-lint
+    rev: 1.4.2
+    hooks:
+      - id: cmakelint
+  - repo: https://github.com/cheshirekow/cmake-format-precommit
+    rev: v0.6.13
     hooks:
-      - id: nixpkgs-fmt
+      - id: cmake-format
+        additional_dependencies:
+          - pyyaml
+      - id: cmake-lint
+        additional_dependencies:
+          - pyyaml
 
 ci:
   skip:
     - pyright
```

### Comparing `autotools-language-server-0.0.8/LICENSE` & `autotools_language_server-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autotools-language-server-0.0.8/PKG-INFO` & `autotools_language_server-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 Metadata-Version: 2.1
 Name: autotools-language-server
-Version: 0.0.8
+Version: 0.0.9
 Summary: autotools language server
-Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
+Keywords: autotools language server
+Author-Email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
-Project-URL: Homepage, https://autotools-language-server.readthedocs.io
-Project-URL: Download, https://github.com/Freed-Wu/autotools-language-server/releases
-Project-URL: Bug Report, https://github.com/Freed-Wu/autotools-language-server/issues
-Project-URL: Source, https://github.com/Freed-Wu/autotools-language-server
-Keywords: autotools,language server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
@@ -22,18 +18,25 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Project-URL: Homepage, https://autotools-language-server.readthedocs.io
+Project-URL: Download, https://github.com/Freed-Wu/autotools-language-server/releases
+Project-URL: Bug report, https://github.com/Freed-Wu/autotools-language-server/issues
+Project-URL: Source, https://github.com/Freed-Wu/autotools-language-server
+Requires-Python: >=3.10
+Requires-Dist: platformdirs
+Requires-Dist: pygls
+Requires-Dist: tree-sitter
+Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: dev
-License-File: LICENSE
+Description-Content-Type: text/markdown
 
 # autotools-language-server
 
 [![readthedocs](https://shields.io/readthedocs/autotools-language-server)](https://autotools-language-server.readthedocs.io)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Freed-Wu/autotools-language-server/main.svg)](https://results.pre-commit.ci/latest/github/Freed-Wu/autotools-language-server/main)
 [![github/workflow](https://github.com/Freed-Wu/autotools-language-server/actions/workflows/main.yml/badge.svg)](https://github.com/Freed-Wu/autotools-language-server/actions)
 [![codecov](https://codecov.io/gh/Freed-Wu/autotools-language-server/branch/main/graph/badge.svg)](https://codecov.io/gh/Freed-Wu/autotools-language-server)
@@ -69,27 +72,30 @@
 [![pypi/format](https://shields.io/pypi/format/autotools-language-server)](https://pypi.org/project/autotools-language-server/#files)
 [![pypi/implementation](https://shields.io/pypi/implementation/autotools-language-server)](https://pypi.org/project/autotools-language-server/#files)
 [![pypi/pyversions](https://shields.io/pypi/pyversions/autotools-language-server)](https://pypi.org/project/autotools-language-server/#files)
 
 Language server for [autotools](https://www.gnu.org/software/autotools). Support:
 
 - `configure.ac`
-
 - `Makefile.am`
-
 - `Makefile`
 
-- [x] document hover
+Support:
 
+- [x] document hover
 - [x] completion
+- [x] diagnostic
+- [ ] go to definition
 
 ![document hover](https://github.com/SchemaStore/schemastore/assets/32936898/d8a2cdf1-d62b-46f4-87a9-12701ab660a6)
 
 ![completion](https://github.com/SchemaStore/schemastore/assets/32936898/fa0c523d-cb51-4870-92a4-07d64c624221)
 
+![diagnostic](https://github.com/Freed-Wu/autotools-language-server/assets/32936898/a1b35e66-7046-42e0-8db8-b636e711764d)
+
 Read
 [![readthedocs](https://shields.io/readthedocs/autotools-language-server)](https://autotools-language-server.readthedocs.io)
 to know more.
 
 ## Similar Projects
 
 - [cmake-language-server](https://github.com/regen100/cmake-language-server)
```

### Comparing `autotools-language-server-0.0.8/README.md` & `autotools_language_server-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,27 +36,30 @@
 [![pypi/format](https://shields.io/pypi/format/autotools-language-server)](https://pypi.org/project/autotools-language-server/#files)
 [![pypi/implementation](https://shields.io/pypi/implementation/autotools-language-server)](https://pypi.org/project/autotools-language-server/#files)
 [![pypi/pyversions](https://shields.io/pypi/pyversions/autotools-language-server)](https://pypi.org/project/autotools-language-server/#files)
 
 Language server for [autotools](https://www.gnu.org/software/autotools). Support:
 
 - `configure.ac`
-
 - `Makefile.am`
-
 - `Makefile`
 
-- [x] document hover
+Support:
 
+- [x] document hover
 - [x] completion
+- [x] diagnostic
+- [ ] go to definition
 
 ![document hover](https://github.com/SchemaStore/schemastore/assets/32936898/d8a2cdf1-d62b-46f4-87a9-12701ab660a6)
 
 ![completion](https://github.com/SchemaStore/schemastore/assets/32936898/fa0c523d-cb51-4870-92a4-07d64c624221)
 
+![diagnostic](https://github.com/Freed-Wu/autotools-language-server/assets/32936898/a1b35e66-7046-42e0-8db8-b636e711764d)
+
 Read
 [![readthedocs](https://shields.io/readthedocs/autotools-language-server)](https://autotools-language-server.readthedocs.io)
 to know more.
 
 ## Similar Projects
 
 - [cmake-language-server](https://github.com/regen100/cmake-language-server)
```

### Comparing `autotools-language-server-0.0.8/docs/conf.py` & `autotools_language_server-0.0.9/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
     "sphinx.ext.githubpages",
     "myst_parser",
-    "sphinxcontrib.eval",
+    "sphinxcontrib.autofile",
+    "sphinxcontrib.requirements_txt",
 ]
 
 myst_heading_anchors = 3
 myst_title_to_header = True
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
```

### Comparing `autotools-language-server-0.0.8/docs/resources/configure.md` & `autotools_language_server-0.0.9/docs/resources/configure.md`

 * *Files identical despite different names*

### Comparing `autotools-language-server-0.0.8/docs/resources/install.md` & `autotools_language_server-0.0.9/docs/resources/install.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Install
 
 ## [AUR](https://aur.archlinux.org/packages/autotools-language-server)
 
 ```sh
-yay -S python-autotools-language-server
+yay -S autotools-language-server
 ```
 
 ## [NUR](https://nur.nix-community.org/repos/Freed-Wu)
 
 ```nix
 { config, pkgs, ... }:
 {
```

### Comparing `autotools-language-server-0.0.8/pyproject.toml` & `autotools_language_server-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
-requires = ["setuptools_scm[toml] >= 6.2", "setuptools-generate >= 0.0.6"]
-build-backend = "setuptools.build_meta"
+requires = ["scikit-build-core"]
+build-backend = "scikit_build_core.build"
 
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [project]
 name = "autotools-language-server"
 description = "autotools language server"
 readme = "README.md"
-requires-python = ">= 3.7"
+# type_a | type_b
+requires-python = ">= 3.10"
 keywords = ["autotools", "language server"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Topic :: Software Development :: Build Tools",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: Microsoft :: Windows",
@@ -24,15 +25,21 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dynamic = ["version", "dependencies", "optional-dependencies"]
+# dynamic = ["version", "dependencies", "optional-dependencies"]
+# https://github.com/pypa/twine/issues/753
+dynamic = ["version"]
+dependencies = ["platformdirs", "pygls", "tree-sitter"]
+
+[project.optional-dependencies]
+dev = ["pytest-cov"]
 
 [[project.authors]]
 name = "Wu Zhenyu"
 email = "wuzhenyu@ustc.edu"
 
 [project.license]
 text = "GPL v3"
@@ -42,36 +49,38 @@
 Download = "https://github.com/Freed-Wu/autotools-language-server/releases"
 "Bug Report" = "https://github.com/Freed-Wu/autotools-language-server/issues"
 Source = "https://github.com/Freed-Wu/autotools-language-server"
 
 [project.scripts]
 autotools-language-server = "autotools_language_server.__main__:main"
 
-[tool.setuptools.package-data]
-autotools_language_server = ["py.typed", "assets/**"]
+[tool.scikit-build]
+experimental = true
+
+[tool.scikit-build.metadata.version]
+provider = "scikit_build_core.metadata.setuptools_scm"
 
-[tool.setuptools.data-files]
-"share/man/man1" = ["sdist/autotools-language-server.1"]
-"share/bash-completion/completions" = ["sdist/autotools-language-server"]
-"share/zsh/site-functions" = ["sdist/_autotools-language-server"]
+[tool.scikit-build.sdist]
+include = ["src/autotools_language_server/_version.py"]
+
+[[tool.scikit-build.generate]]
+path = "autotools_language_server/_metainfo.py"
+template-path = "templates/metainfo.py"
 
 [tool.setuptools.dynamic.dependencies]
 file = "requirements.txt"
 
 # begin: scripts/update-pyproject.toml.pl
 [tool.setuptools.dynamic.optional-dependencies.dev]
 file = "requirements/dev.txt"
 # end: scripts/update-pyproject.toml.pl
 
 [tool.setuptools_scm]
 write_to = "src/autotools_language_server/_version.py"
 
-[tool.setuptools-generate]
-write-to = "src/autotools_language_server/_metainfo.py"
-
 [tool.mdformat]
 number = true
 
 [tool.black]
 line-length = 79
 
 [tool.isort]
@@ -93,9 +102,10 @@
 ]
 
 [tool.bandit.assert_used]
 skips = ["*_test.py", "test_*.py"]
 
 [tool.cibuildwheel]
 archs = ["all"]
-before-test = "pip install pytest"
+skip = "*37-* *38-* *39-*"
+before-test = "pip install -rrequirements.txt -rrequirements/dev.txt"
 test-command = "pytest {project}"
```

### Comparing `autotools-language-server-0.0.8/src/autotools_language_server/__main__.py` & `autotools_language_server-0.0.9/src/autotools_language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `autotools-language-server-0.0.8/src/autotools_language_server/api/autoconf.py` & `autotools_language_server-0.0.9/src/autotools_language_server/api/autoconf.py`

 * *Files identical despite different names*

### Comparing `autotools-language-server-0.0.8/src/autotools_language_server/api/make.py` & `autotools_language_server-0.0.9/src/autotools_language_server/api/make.py`

 * *Files identical despite different names*

### Comparing `autotools-language-server-0.0.8/src/autotools_language_server/assets/json/autotools.json` & `autotools_language_server-0.0.9/src/autotools_language_server/assets/json/autotools.json`

 * *Files identical despite different names*

### Comparing `autotools-language-server-0.0.8/src/autotools_language_server/server.py` & `autotools_language_server-0.0.9/src/autotools_language_server/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,59 @@
 r"""Server
 ==========
 """
 import json
 import os
 import re
 from typing import Any, Literal, Tuple
+from urllib.parse import unquote, urlparse
 
 from lsprotocol.types import (
     INITIALIZE,
     TEXT_DOCUMENT_COMPLETION,
+    TEXT_DOCUMENT_DID_CHANGE,
+    TEXT_DOCUMENT_DID_OPEN,
     TEXT_DOCUMENT_HOVER,
     CompletionItem,
     CompletionItemKind,
     CompletionList,
     CompletionParams,
+    Diagnostic,
+    DiagnosticSeverity,
+    DidChangeTextDocumentParams,
     Hover,
     InitializeParams,
     MarkupContent,
     MarkupKind,
     Position,
     Range,
     TextDocumentPositionParams,
 )
 from platformdirs import user_cache_dir
 from pygls.server import LanguageServer
 
+from ._tree_sitter import get_parser
+from .diagnostics import diagnostic
+
 
 def check_extension(
-    uri: str,
+    path: str,
 ) -> Literal["config", "make", ""]:
     r"""Check extension.
 
-    :param uri:
-    :type uri: str
+    :param path:
+    :type path: str
     :rtype: Literal["config", "make", ""]
     """
     if (
-        uri.split(os.path.extsep)[-1] in ["mk"]
-        or os.path.basename(uri).split(os.path.extsep)[0] == "Makefile"
+        path.split(os.path.extsep)[-1] in ["mk"]
+        or os.path.basename(path).split(os.path.extsep)[0] == "Makefile"
     ):
         return "make"
-    if os.path.basename(uri) == "configure.ac":
+    if os.path.basename(path) == "configure.ac":
         return "config"
     return ""
 
 
 def get_document(
     method: Literal["builtin", "cache", "system"] = "builtin"
 ) -> dict[str, tuple[str, str]]:
@@ -95,14 +104,16 @@
 
         :param args:
         :type args: Any
         :rtype: None
         """
         super().__init__(*args)
         self.document = {}
+        self.parser = get_parser()
+        self.tree = self.parser.parse(b"")
 
         @self.feature(INITIALIZE)
         def initialize(params: InitializeParams) -> None:
             opts = params.initialization_options
             method = getattr(opts, "method", "builtin")
             self.document = get_document(method)  # type: ignore
 
@@ -110,15 +121,17 @@
         def hover(params: TextDocumentPositionParams) -> Hover | None:
             r"""Hover.
 
             :param params:
             :type params: TextDocumentPositionParams
             :rtype: Hover | None
             """
-            if not check_extension(params.text_document.uri):
+            if not check_extension(
+                unquote(urlparse(params.text_document.uri).path)
+            ):
                 return None
             word = self._cursor_word(
                 params.text_document.uri, params.position, True
             )
             if not word:
                 return None
             result = self.document.get(word[0])
@@ -135,15 +148,17 @@
         def completions(params: CompletionParams) -> CompletionList:
             r"""Completions.
 
             :param params:
             :type params: CompletionParams
             :rtype: CompletionList
             """
-            if not check_extension(params.text_document.uri):
+            if not check_extension(
+                unquote(urlparse(params.text_document.uri).path)
+            ):
                 return CompletionList(is_incomplete=False, items=[])
             word = self._cursor_word(
                 params.text_document.uri, params.position, False
             )
             token = "" if word is None else word[0]
             items = [
                 CompletionItem(
@@ -151,18 +166,58 @@
                     kind=CompletionItemKind.Function,
                     documentation=self.document[x][0],
                     insert_text=x,
                 )
                 for x in self.document
                 if x.startswith(token)
                 and self.document[x][1]
-                == check_extension(params.text_document.uri)
+                == check_extension(
+                    unquote(urlparse(params.text_document.uri).path)
+                )
             ]
             return CompletionList(is_incomplete=False, items=items)
 
+        @self.feature(TEXT_DOCUMENT_DID_OPEN)
+        @self.feature(TEXT_DOCUMENT_DID_CHANGE)
+        def did_change(params: DidChangeTextDocumentParams) -> None:
+            r"""Did change.
+
+            :param params:
+            :type params: DidChangeTextDocumentParams
+            :rtype: None
+            """
+            if (
+                check_extension(
+                    unquote(urlparse(params.text_document.uri).path)
+                )
+                != "make"
+            ):
+                return None
+            doc = self.workspace.get_document(params.text_document.uri)
+            source = doc.source
+            self.tree = self.parser.parse(bytes(source, "utf-8"))
+            diagnostics = [
+                Diagnostic(
+                    range=Range(
+                        Position(node.start_point[0], node.start_point[1]),
+                        Position(node.end_point[0], node.end_point[1]),
+                    ),
+                    message=message,
+                    severity=getattr(DiagnosticSeverity, severity),
+                    source="autotools-language-server",
+                )
+                for node, message, severity in diagnostic(
+                    self.tree,
+                    os.path.dirname(
+                        unquote(urlparse(params.text_document.uri).path)
+                    ),
+                )
+            ]
+            self.publish_diagnostics(doc.uri, diagnostics)
+
     def _cursor_line(self, uri: str, position: Position) -> str:
         r"""Cursor line.
 
         :param uri:
         :type uri: str
         :param position:
         :type position: Position
```

