# Comparing `tmp/dissect_cstruct-4.0.dev0.tar.gz` & `tmp/dissect_cstruct-4.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect_cstruct-4.0.dev0.tar", last modified: Fri May 17 14:33:57 2024, max compression
+gzip compressed data, was "dissect_cstruct-4.0.dev1.tar", last modified: Fri May 24 19:22:12 2024, max compression
```

## Comparing `dissect_cstruct-4.0.dev0.tar` & `dissect_cstruct-4.0.dev1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.717146 dissect_cstruct-4.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-05-17 14:33:57.713146 dissect_cstruct-4.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.701146 dissect_cstruct-4.0.dev0/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.705146 dissect_cstruct-4.0.dev0/dissect/cstruct/
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/bitbuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14851 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/cstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    20806 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.709146 dissect_cstruct-4.0.dev0/dissect/cstruct/types/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/char.py
--rw-r--r--   0 runner    (1001) docker     (127)     6616 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/leb128.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/packed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23954 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/void.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/wchar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.713146 dissect_cstruct-4.0.dev0/dissect.cstruct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-05-17 14:33:57.000000 dissect_cstruct-4.0.dev0/dissect.cstruct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-17 14:33:57.000000 dissect_cstruct-4.0.dev0/dissect.cstruct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:33:57.000000 dissect_cstruct-4.0.dev0/dissect.cstruct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 14:33:57.000000 dissect_cstruct-4.0.dev0/dissect.cstruct.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.709146 dissect_cstruct-4.0.dev0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/examples/disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/examples/mirai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/examples/pe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/examples/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/examples/secdesc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:33:57.717146 dissect_cstruct-4.0.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.713146 dissect_cstruct-4.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.713146 dissect_cstruct-4.0.dev0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/data/testdef.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.713146 dissect_cstruct-4.0.dev0/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_bitbuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_bitfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     8853 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)    12932 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_int.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_leb128.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_packed.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_union.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_void.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_wchar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:22:12.673052 dissect_cstruct-4.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-05-24 19:22:12.673052 dissect_cstruct-4.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:22:12.661052 dissect_cstruct-4.0.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:22:12.665052 dissect_cstruct-4.0.dev1/dissect/cstruct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/bitbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14851 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/cstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20806 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:22:12.669052 dissect_cstruct-4.0.dev1/dissect/cstruct/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/types/char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6616 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/types/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/types/flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/types/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/types/leb128.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/types/packed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/types/pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23954 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/types/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/types/void.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/types/wchar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/dissect/cstruct/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:22:12.673052 dissect_cstruct-4.0.dev1/dissect.cstruct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-05-24 19:22:12.000000 dissect_cstruct-4.0.dev1/dissect.cstruct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-24 19:22:12.000000 dissect_cstruct-4.0.dev1/dissect.cstruct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 19:22:12.000000 dissect_cstruct-4.0.dev1/dissect.cstruct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 19:22:12.000000 dissect_cstruct-4.0.dev1/dissect.cstruct.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:22:12.669052 dissect_cstruct-4.0.dev1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/examples/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/examples/mirai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/examples/pe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/examples/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/examples/secdesc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-24 19:22:07.000000 dissect_cstruct-4.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 19:22:12.677052 dissect_cstruct-4.0.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:22:12.673052 dissect_cstruct-4.0.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:22:12.673052 dissect_cstruct-4.0.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/data/testdef.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:22:12.673052 dissect_cstruct-4.0.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_bitbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_bitfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_types_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_types_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_types_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8853 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_types_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_types_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12932 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_types_int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_types_leb128.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_types_packed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_types_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_types_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_types_union.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_types_void.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_types_wchar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-24 19:22:00.000000 dissect_cstruct-4.0.dev1/tox.ini
```

### Comparing `dissect_cstruct-4.0.dev0/LICENSE` & `dissect_cstruct-4.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/PKG-INFO` & `dissect_cstruct-4.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.cstruct
-Version: 4.0.dev0
+Version: 4.0.dev1
 Summary: A Dissect module implementing a parser for C-like structures: structure parsing in Python made easy
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cstruct
 Project-URL: repository, https://github.com/fox-it/dissect.cstruct
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect_cstruct-4.0.dev0/README.md` & `dissect_cstruct-4.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/__init__.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/bitbuffer.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/bitbuffer.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/compiler.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/compiler.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/cstruct.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/cstruct.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/expression.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,8 +295,11 @@
 
         while len(self.stack) != 0:
             if self.stack[-1] == "(":
                 raise ExpressionParserError("Invalid expression")
 
             self.evaluate_exp()
 
+        if len(self.queue) != 1:
+            raise ExpressionParserError("Invalid expression")
+
         return self.queue[0]
```

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/parser.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/parser.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/types/__init__.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/types/base.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/types/base.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/types/char.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/types/char.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/types/enum.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/types/enum.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/types/flag.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/types/flag.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/types/int.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/types/int.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/types/leb128.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/types/leb128.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/types/packed.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/types/packed.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/types/pointer.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/types/pointer.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/types/structure.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/types/structure.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/types/wchar.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/types/wchar.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect/cstruct/utils.py` & `dissect_cstruct-4.0.dev1/dissect/cstruct/utils.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/dissect.cstruct.egg-info/PKG-INFO` & `dissect_cstruct-4.0.dev1/dissect.cstruct.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.cstruct
-Version: 4.0.dev0
+Version: 4.0.dev1
 Summary: A Dissect module implementing a parser for C-like structures: structure parsing in Python made easy
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cstruct
 Project-URL: repository, https://github.com/fox-it/dissect.cstruct
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect_cstruct-4.0.dev0/dissect.cstruct.egg-info/SOURCES.txt` & `dissect_cstruct-4.0.dev1/dissect.cstruct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/examples/disk.py` & `dissect_cstruct-4.0.dev1/examples/disk.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/examples/mirai.py` & `dissect_cstruct-4.0.dev1/examples/mirai.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/examples/pe.py` & `dissect_cstruct-4.0.dev1/examples/pe.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/examples/protobuf.py` & `dissect_cstruct-4.0.dev1/examples/protobuf.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/examples/secdesc.py` & `dissect_cstruct-4.0.dev1/examples/secdesc.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/pyproject.toml` & `dissect_cstruct-4.0.dev1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -42,7 +42,8 @@
 [tool.setuptools]
 license-files = ["LICENSE", "COPYRIGHT"]
 
 [tool.setuptools.packages.find]
 include = ["dissect.*"]
 
 [tool.setuptools_scm]
+local_scheme = "no-local-version"
```

### Comparing `dissect_cstruct-4.0.dev0/tests/docs/Makefile` & `dissect_cstruct-4.0.dev1/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/docs/conf.py` & `dissect_cstruct-4.0.dev1/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_align.py` & `dissect_cstruct-4.0.dev1/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_basic.py` & `dissect_cstruct-4.0.dev1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_bitbuffer.py` & `dissect_cstruct-4.0.dev1/tests/test_bitbuffer.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_bitfield.py` & `dissect_cstruct-4.0.dev1/tests/test_bitfield.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_compiler.py` & `dissect_cstruct-4.0.dev1/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_ctypes.py` & `dissect_cstruct-4.0.dev1/tests/test_ctypes.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_expression.py` & `dissect_cstruct-4.0.dev1/tests/test_expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     [
         ("0b", ExpressionTokenizerError, "Invalid binary or hex notation"),
         ("0x", ExpressionTokenizerError, "Invalid binary or hex notation"),
         ("$", ExpressionTokenizerError, "Tokenizer does not recognize following token '\\$'"),
         ("-", ExpressionParserError, "Invalid expression: not enough operands"),
         ("(", ExpressionParserError, "Invalid expression"),
         (")", ExpressionParserError, "Invalid expression"),
+        (" ", ExpressionParserError, "Invalid expression"),
         ("()", ExpressionParserError, "Parser expected an expression, instead received empty parenthesis. Index: 1"),
         ("0()", ExpressionParserError, "Parser expected sizeof or an arethmethic operator instead got: '0'"),
         ("sizeof)", ExpressionParserError, "Invalid sizeof operation"),
         ("sizeof(0 +)", ExpressionParserError, "Invalid sizeof operation"),
     ],
 )
 def test_expression_failure(expression: str, exception: type, message: str) -> None:
```

### Comparing `dissect_cstruct-4.0.dev0/tests/test_parser.py` & `dissect_cstruct-4.0.dev1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_types_base.py` & `dissect_cstruct-4.0.dev1/tests/test_types_base.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_types_char.py` & `dissect_cstruct-4.0.dev1/tests/test_types_char.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_types_custom.py` & `dissect_cstruct-4.0.dev1/tests/test_types_custom.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_types_enum.py` & `dissect_cstruct-4.0.dev1/tests/test_types_enum.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_types_flag.py` & `dissect_cstruct-4.0.dev1/tests/test_types_flag.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_types_int.py` & `dissect_cstruct-4.0.dev1/tests/test_types_int.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_types_leb128.py` & `dissect_cstruct-4.0.dev1/tests/test_types_leb128.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_types_packed.py` & `dissect_cstruct-4.0.dev1/tests/test_types_packed.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_types_pointer.py` & `dissect_cstruct-4.0.dev1/tests/test_types_pointer.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_types_structure.py` & `dissect_cstruct-4.0.dev1/tests/test_types_structure.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_types_union.py` & `dissect_cstruct-4.0.dev1/tests/test_types_union.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_types_wchar.py` & `dissect_cstruct-4.0.dev1/tests/test_types_wchar.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tests/test_utils.py` & `dissect_cstruct-4.0.dev1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dissect_cstruct-4.0.dev0/tox.ini` & `dissect_cstruct-4.0.dev1/tox.ini`

 * *Files identical despite different names*

