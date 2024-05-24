# Comparing `tmp/test_autochem-0.1.0.tar.gz` & `tmp/test_autochem-0.2.0.tar.gz`

## Comparing `test_autochem-0.1.0.tar` & `test_autochem-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 test_autochem-0.1.0/.gitattributes
--rw-r--r--   0        0        0    53433 2020-02-02 00:00:00.000000 test_autochem-0.1.0/pixi.lock
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 test_autochem-0.1.0/src/automol/__init__.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 test_autochem-0.1.0/src/autoreact/__init__.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 test_autochem-0.1.0/src/molsym/__init__.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 test_autochem-0.1.0/src/phydat/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 test_autochem-0.1.0/.gitignore
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 test_autochem-0.1.0/hatch.toml
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 test_autochem-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 test_autochem-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 test_autochem-0.2.0/.gitattributes
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 test_autochem-0.2.0/example.pypirc
+-rw-r--r--   0        0        0    53433 2020-02-02 00:00:00.000000 test_autochem-0.2.0/pixi.lock
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 test_autochem-0.2.0/src/automol/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 test_autochem-0.2.0/src/autoreact/__init__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 test_autochem-0.2.0/src/molsym/__init__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 test_autochem-0.2.0/src/phydat/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 test_autochem-0.2.0/.gitignore
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 test_autochem-0.2.0/hatch.toml
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 test_autochem-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 test_autochem-0.2.0/PKG-INFO
```

### Comparing `test_autochem-0.1.0/pixi.lock` & `test_autochem-0.2.0/pixi.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1230,17 +1230,17 @@
   - python >=3.7
   license: Apache-2.0
   license_family: Apache
   size: 15064
   timestamp: 1708953086199
 - kind: pypi
   name: test-autochem
-  version: 0.1.0
+  version: 0.2.0
   path: .
-  sha256: a634c403a8f2be5cefb6fcfdacc1c8d580fdccee9088f27120a6ff86a9acc1a0
+  sha256: e651d4d1b128281fdf3a4c0175f7141beb3954037d2d433124a0fdb2747e3d21
   requires_python: '>=3.11'
   editable: true
 - kind: conda
   name: tk
   version: 8.6.13
   build: h1abcd95_1
   build_number: 1
```

