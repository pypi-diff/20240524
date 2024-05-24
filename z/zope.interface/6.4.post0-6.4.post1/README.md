# Comparing `tmp/zope.interface-6.4.post0.tar.gz` & `tmp/zope.interface-6.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.interface-6.4.post0.tar", last modified: Wed May 22 06:43:23 2024, max compression
+gzip compressed data, was "zope.interface-6.4.post1.tar", last modified: Thu May 23 07:17:23 2024, max compression
```

## Comparing `zope.interface-6.4.post0.tar` & `zope.interface-6.4.post1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.410102 zope.interface-6.4.post0/
--rw-r--r--   0 m.howitz   (502) staff       (20)      588 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/.coveragerc
--rwxr-xr-x   0 m.howitz   (502) staff       (20)     2259 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/.manylinux-install.sh
--rwxr-xr-x   0 m.howitz   (502) staff       (20)      509 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/.manylinux.sh
--rw-r--r--   0 m.howitz   (502) staff       (20)      664 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/.readthedocs.yaml
--rw-r--r--   0 m.howitz   (502) staff       (20)    39533 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/CHANGES.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      799 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/CONTRIBUTING.md
--rw-r--r--   0 m.howitz   (502) staff       (20)       32 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/COPYRIGHT.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/LICENSE.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)      558 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/MANIFEST.in
--rw-r--r--   0 m.howitz   (502) staff       (20)    42589 2024-05-22 06:43:23.409971 zope.interface-6.4.post0/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)     1353 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/README.rst
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.394587 zope.interface-6.4.post0/benchmarks/
--rw-r--r--   0 m.howitz   (502) staff       (20)     8497 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/benchmarks/micro.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      838 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/build.cmd
--rw-r--r--   0 m.howitz   (502) staff       (20)      215 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/buildout.cfg
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.397470 zope.interface-6.4.post0/docs/
--rw-r--r--   0 m.howitz   (502) staff       (20)     5592 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/Makefile
--rw-r--r--   0 m.howitz   (502) staff       (20)    41051 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/README.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    33998 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/README.ru.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    18817 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/adapter.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    21169 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/adapter.ru.rst
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.398522 zope.interface-6.4.post0/docs/api/
--rw-r--r--   0 m.howitz   (502) staff       (20)      691 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/api/adapters.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1283 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/api/common.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     2465 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/api/components.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    21746 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/api/declarations.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      165 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/api/index.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      687 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/api/ro.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     9948 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/api/specifications.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       28 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/changes.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     9130 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/conf.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1742 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/foodforthought.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     9509 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/hacking.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     6537 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/human.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    10681 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/human.ru.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      639 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/index.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     5110 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/make.bat
--rw-r--r--   0 m.howitz   (502) staff       (20)       68 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/requirements.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)    10222 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/verify.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      570 2024-05-22 06:43:23.410475 zope.interface-6.4.post0/setup.cfg
--rw-r--r--   0 m.howitz   (502) staff       (20)     5020 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/setup.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.391102 zope.interface-6.4.post0/src/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.398692 zope.interface-6.4.post0/src/zope/
--rw-r--r--   0 m.howitz   (502) staff       (20)       56 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/__init__.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.402369 zope.interface-6.4.post0/src/zope/interface/
--rw-r--r--   0 m.howitz   (502) staff       (20)     3460 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4369 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/_compat.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1057 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/_flatten.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    57205 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/_zope_interface_coptimizations.c
--rw-r--r--   0 m.howitz   (502) staff       (20)    36218 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/adapter.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3892 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/advice.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.404089 zope.interface-6.4.post0/src/zope/interface/common/
--rw-r--r--   0 m.howitz   (502) staff       (20)    10462 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3027 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/builtins.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     6792 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/collections.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    20964 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/idatetime.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5368 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/interfaces.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1242 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/io.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4678 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/mapping.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1682 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/numbers.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5526 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/sequence.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.405487 zope.interface-6.4.post0/src/zope/interface/common/tests/
--rw-r--r--   0 m.howitz   (502) staff       (20)     5476 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/tests/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3907 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/tests/basemapping.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1345 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/tests/test_builtins.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5718 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/tests/test_collections.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1923 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/tests/test_idatetime.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      813 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/tests/test_import_interfaces.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1663 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/tests/test_io.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1394 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/tests/test_numbers.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    43007 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/declarations.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4068 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/document.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     8636 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/exceptions.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    39409 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/interface.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    50126 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/interfaces.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    25829 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/registry.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    24157 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/ro.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.409061 zope.interface-6.4.post0/src/zope/interface/tests/
--rw-r--r--   0 m.howitz   (502) staff       (20)     3961 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      898 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/advisory_testing.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      912 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/dummy.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      890 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/idummy.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      839 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/m1.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3015 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/odd.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    79479 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_adapter.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     6040 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_advice.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1290 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_compile_flags.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    82140 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_declarations.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    17164 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_document.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1120 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_element.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     6412 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_exceptions.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    92312 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_interface.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4377 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_interfaces.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     7566 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_odd_declarations.py
--rw-r--r--   0 m.howitz   (502) staff       (20)   112910 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_registry.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    14124 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_ro.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1934 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_sorting.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    19191 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_verify.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     7226 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/verify.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.409299 zope.interface-6.4.post0/src/zope.interface.egg-info/
--rw-r--r--   0 m.howitz   (502) staff       (20)    42589 2024-05-22 06:43:23.000000 zope.interface-6.4.post0/src/zope.interface.egg-info/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)     2940 2024-05-22 06:43:23.000000 zope.interface-6.4.post0/src/zope.interface.egg-info/SOURCES.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-05-22 06:43:23.000000 zope.interface-6.4.post0/src/zope.interface.egg-info/dependency_links.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        5 2024-05-22 06:43:23.000000 zope.interface-6.4.post0/src/zope.interface.egg-info/namespace_packages.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-05-22 06:43:23.000000 zope.interface-6.4.post0/src/zope.interface.egg-info/not-zip-safe
--rw-r--r--   0 m.howitz   (502) staff       (20)      170 2024-05-22 06:43:23.000000 zope.interface-6.4.post0/src/zope.interface.egg-info/requires.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        5 2024-05-22 06:43:23.000000 zope.interface-6.4.post0/src/zope.interface.egg-info/top_level.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     2132 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-23 07:17:23.860713 zope.interface-6.4.post1/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      609 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/.coveragerc
+-rwxr-xr-x   0 m.howitz   (502) staff       (20)     2267 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/.manylinux-install.sh
+-rwxr-xr-x   0 m.howitz   (502) staff       (20)      509 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/.manylinux.sh
+-rw-r--r--   0 m.howitz   (502) staff       (20)      664 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/.readthedocs.yaml
+-rw-r--r--   0 m.howitz   (502) staff       (20)    39690 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      799 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      558 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)    42746 2024-05-23 07:17:23.860538 zope.interface-6.4.post1/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1353 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/README.rst
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-23 07:17:23.845610 zope.interface-6.4.post1/benchmarks/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8497 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/benchmarks/micro.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      838 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/build.cmd
+-rw-r--r--   0 m.howitz   (502) staff       (20)      215 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/buildout.cfg
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-23 07:17:23.848307 zope.interface-6.4.post1/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5592 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)    41051 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    33998 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/README.ru.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    18817 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/adapter.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    21169 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/adapter.ru.rst
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-23 07:17:23.849582 zope.interface-6.4.post1/docs/api/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      691 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/api/adapters.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1283 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/api/common.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2465 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/api/components.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    21746 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/api/declarations.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      165 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/api/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      687 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/api/ro.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9948 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/api/specifications.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/changes.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9130 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1742 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/foodforthought.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9509 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/hacking.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6537 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/human.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10681 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/human.ru.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      639 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5110 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/make.bat
+-rw-r--r--   0 m.howitz   (502) staff       (20)       68 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/requirements.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10222 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/docs/verify.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      570 2024-05-23 07:17:23.861136 zope.interface-6.4.post1/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5020 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-23 07:17:23.842302 zope.interface-6.4.post1/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-23 07:17:23.849767 zope.interface-6.4.post1/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       56 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-23 07:17:23.853208 zope.interface-6.4.post1/src/zope/interface/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3460 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4369 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/_compat.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1057 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/_flatten.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    57205 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/_zope_interface_coptimizations.c
+-rw-r--r--   0 m.howitz   (502) staff       (20)    36218 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/adapter.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3892 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/advice.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-23 07:17:23.854598 zope.interface-6.4.post1/src/zope/interface/common/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10462 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3027 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/builtins.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6792 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/collections.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    20964 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/idatetime.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5368 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1242 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/io.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4678 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/mapping.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1682 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/numbers.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5526 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/sequence.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-23 07:17:23.855853 zope.interface-6.4.post1/src/zope/interface/common/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5476 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3907 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/tests/basemapping.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1345 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/tests/test_builtins.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5718 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/tests/test_collections.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1923 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/tests/test_idatetime.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      813 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/tests/test_import_interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1663 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/tests/test_io.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1394 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/common/tests/test_numbers.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    43007 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/declarations.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4068 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/document.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8636 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/exceptions.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    39409 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/interface.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    50126 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    25829 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/registry.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    24157 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/ro.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-23 07:17:23.859503 zope.interface-6.4.post1/src/zope/interface/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3961 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      898 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/advisory_testing.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      912 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/dummy.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      890 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/idummy.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      839 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/m1.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3015 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/odd.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    79479 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/test_adapter.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6040 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/test_advice.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1290 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/test_compile_flags.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    82140 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/test_declarations.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    17164 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/test_document.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1120 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/test_element.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6412 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/test_exceptions.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    92312 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/test_interface.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4377 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/test_interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7566 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/test_odd_declarations.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)   112910 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/test_registry.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    14124 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/test_ro.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1934 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/test_sorting.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    19191 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/tests/test_verify.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7226 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope/interface/verify.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-23 07:17:23.859769 zope.interface-6.4.post1/src/zope.interface.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    42746 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope.interface.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2940 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope.interface.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope.interface.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope.interface.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope.interface.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      170 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope.interface.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/src/zope.interface.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2132 2024-05-23 07:17:23.000000 zope.interface-6.4.post1/tox.ini
```

### Comparing `zope.interface-6.4.post0/.coveragerc` & `zope.interface-6.4.post1/.coveragerc`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     src/
     .tox/*/lib/python*/site-packages/
     .tox/pypy*/site-packages/
 
 [report]
 show_missing = true
 precision = 2
+ignore_errors = True
 exclude_lines =
     except ImportError:
     if __name__ == '__main__':
     pragma: no cover
     pragma: nocover
     raise AssertionError
     raise NotImplementedError
```

### Comparing `zope.interface-6.4.post0/.manylinux-install.sh` & `zope.interface-6.4.post1/.manylinux-install.sh`

 * *Files 6% similar despite different names*

```diff
@@ -38,22 +38,22 @@
         *) echo 'py';;
     esac
 }
 
 # Compile wheels
 for PYBIN in /opt/python/*/bin; do
     if \
-       [[ "${PYBIN}" == *"cp313"* ]] || \
-       [[ "${PYBIN}" == *"cp311"* ]] || \
-       [[ "${PYBIN}" == *"cp312"* ]] || \
-       [[ "${PYBIN}" == *"cp37"* ]] || \
-       [[ "${PYBIN}" == *"cp38"* ]] || \
-       [[ "${PYBIN}" == *"cp39"* ]] || \
-       [[ "${PYBIN}" == *"cp310"* ]] ; then
-        if [[ "${PYBIN}" == *"cp313"* ]] ; then
+       [[ "${PYBIN}" == *"cp313/"* ]] || \
+       [[ "${PYBIN}" == *"cp311/"* ]] || \
+       [[ "${PYBIN}" == *"cp312/"* ]] || \
+       [[ "${PYBIN}" == *"cp37/"* ]] || \
+       [[ "${PYBIN}" == *"cp38/"* ]] || \
+       [[ "${PYBIN}" == *"cp39/"* ]] || \
+       [[ "${PYBIN}" == *"cp310/"* ]] ; then
+        if [[ "${PYBIN}" == *"cp313/"* ]] ; then
             "${PYBIN}/pip" install --pre -e /io/
             "${PYBIN}/pip" wheel /io/ --pre -w wheelhouse/
         else
             "${PYBIN}/pip" install -e /io/
             "${PYBIN}/pip" wheel /io/ -w wheelhouse/
         fi
         if [ `uname -m` == 'aarch64' ]; then
```

### Comparing `zope.interface-6.4.post0/.readthedocs.yaml` & `zope.interface-6.4.post1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/CHANGES.rst` & `zope.interface-6.4.post1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
  Changes
 =========
 
+6.4.post1 (2024-05-23)
+======================
+
+- Publish missing Windows wheels.
+  (`#295 <https://github.com/zopefoundation/zope.interface/issues/295>`_)
+
+
 6.4.post0 (2024-05-22)
 ======================
 
 - The sdist of version 6.4 was uploaded to PyPI as
   ``zope_interface-6.4.tar.gz`` instead of ``zope.interface-6.4-py2.tar.gz``
   which cannot be installed by ``zc.buildout``.  This release is a re-release
   of version 6.4 with the correct sdist name.
```

### Comparing `zope.interface-6.4.post0/CONTRIBUTING.md` & `zope.interface-6.4.post1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/LICENSE.txt` & `zope.interface-6.4.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/MANIFEST.in` & `zope.interface-6.4.post1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/PKG-INFO` & `zope.interface-6.4.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.interface
-Version: 6.4.post0
+Version: 6.4.post1
 Summary: Interfaces for Python
 Home-page: https://github.com/zopefoundation/zope.interface
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: interface,components,plugins
 Classifier: Development Status :: 5 - Production/Stable
@@ -71,14 +71,21 @@
 
 For detailed documentation, please see https://zopeinterface.readthedocs.io/en/latest/
 
 =========
  Changes
 =========
 
+6.4.post1 (2024-05-23)
+======================
+
+- Publish missing Windows wheels.
+  (`#295 <https://github.com/zopefoundation/zope.interface/issues/295>`_)
+
+
 6.4.post0 (2024-05-22)
 ======================
 
 - The sdist of version 6.4 was uploaded to PyPI as
   ``zope_interface-6.4.tar.gz`` instead of ``zope.interface-6.4-py2.tar.gz``
   which cannot be installed by ``zc.buildout``.  This release is a re-release
   of version 6.4 with the correct sdist name.
```

### Comparing `zope.interface-6.4.post0/README.rst` & `zope.interface-6.4.post1/README.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/benchmarks/micro.py` & `zope.interface-6.4.post1/benchmarks/micro.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/build.cmd` & `zope.interface-6.4.post1/build.cmd`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/Makefile` & `zope.interface-6.4.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/README.rst` & `zope.interface-6.4.post1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/README.ru.rst` & `zope.interface-6.4.post1/docs/README.ru.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/adapter.rst` & `zope.interface-6.4.post1/docs/adapter.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/adapter.ru.rst` & `zope.interface-6.4.post1/docs/adapter.ru.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/api/adapters.rst` & `zope.interface-6.4.post1/docs/api/adapters.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/api/common.rst` & `zope.interface-6.4.post1/docs/api/common.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/api/components.rst` & `zope.interface-6.4.post1/docs/api/components.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/api/declarations.rst` & `zope.interface-6.4.post1/docs/api/declarations.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/api/ro.rst` & `zope.interface-6.4.post1/docs/api/ro.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/api/specifications.rst` & `zope.interface-6.4.post1/docs/api/specifications.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/conf.py` & `zope.interface-6.4.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/foodforthought.rst` & `zope.interface-6.4.post1/docs/foodforthought.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/hacking.rst` & `zope.interface-6.4.post1/docs/hacking.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/human.rst` & `zope.interface-6.4.post1/docs/human.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/human.ru.rst` & `zope.interface-6.4.post1/docs/human.ru.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/index.rst` & `zope.interface-6.4.post1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/make.bat` & `zope.interface-6.4.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/docs/verify.rst` & `zope.interface-6.4.post1/docs/verify.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/setup.cfg` & `zope.interface-6.4.post1/setup.cfg`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/setup.py` & `zope.interface-6.4.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 long_description = (
         read('README.rst')
         + '\n' +
         read('CHANGES.rst')
         )
 
 setup(name='zope.interface',
-      version='6.4.post0',
+      version='6.4.post1',
       url='https://github.com/zopefoundation/zope.interface',
       license='ZPL 2.1',
       description='Interfaces for Python',
       author='Zope Foundation and Contributors',
       author_email='zope-dev@zope.org',
       long_description=long_description,
       classifiers=[
```

### Comparing `zope.interface-6.4.post0/src/zope/interface/__init__.py` & `zope.interface-6.4.post1/src/zope/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/_compat.py` & `zope.interface-6.4.post1/src/zope/interface/_compat.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/_flatten.py` & `zope.interface-6.4.post1/src/zope/interface/_flatten.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/_zope_interface_coptimizations.c` & `zope.interface-6.4.post1/src/zope/interface/_zope_interface_coptimizations.c`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/adapter.py` & `zope.interface-6.4.post1/src/zope/interface/adapter.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/advice.py` & `zope.interface-6.4.post1/src/zope/interface/advice.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/__init__.py` & `zope.interface-6.4.post1/src/zope/interface/common/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/builtins.py` & `zope.interface-6.4.post1/src/zope/interface/common/builtins.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/collections.py` & `zope.interface-6.4.post1/src/zope/interface/common/collections.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/idatetime.py` & `zope.interface-6.4.post1/src/zope/interface/common/idatetime.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/interfaces.py` & `zope.interface-6.4.post1/src/zope/interface/common/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/io.py` & `zope.interface-6.4.post1/src/zope/interface/common/io.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/mapping.py` & `zope.interface-6.4.post1/src/zope/interface/common/mapping.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/numbers.py` & `zope.interface-6.4.post1/src/zope/interface/common/numbers.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/sequence.py` & `zope.interface-6.4.post1/src/zope/interface/common/sequence.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/tests/__init__.py` & `zope.interface-6.4.post1/src/zope/interface/common/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/tests/basemapping.py` & `zope.interface-6.4.post1/src/zope/interface/common/tests/basemapping.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/tests/test_builtins.py` & `zope.interface-6.4.post1/src/zope/interface/common/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/tests/test_collections.py` & `zope.interface-6.4.post1/src/zope/interface/common/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/tests/test_idatetime.py` & `zope.interface-6.4.post1/src/zope/interface/common/tests/test_idatetime.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/tests/test_import_interfaces.py` & `zope.interface-6.4.post1/src/zope/interface/common/tests/test_import_interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/tests/test_io.py` & `zope.interface-6.4.post1/src/zope/interface/common/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/common/tests/test_numbers.py` & `zope.interface-6.4.post1/src/zope/interface/common/tests/test_numbers.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/declarations.py` & `zope.interface-6.4.post1/src/zope/interface/declarations.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/document.py` & `zope.interface-6.4.post1/src/zope/interface/document.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/exceptions.py` & `zope.interface-6.4.post1/src/zope/interface/exceptions.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/interface.py` & `zope.interface-6.4.post1/src/zope/interface/interface.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/interfaces.py` & `zope.interface-6.4.post1/src/zope/interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/registry.py` & `zope.interface-6.4.post1/src/zope/interface/registry.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/ro.py` & `zope.interface-6.4.post1/src/zope/interface/ro.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/__init__.py` & `zope.interface-6.4.post1/src/zope/interface/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/advisory_testing.py` & `zope.interface-6.4.post1/src/zope/interface/tests/advisory_testing.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/dummy.py` & `zope.interface-6.4.post1/src/zope/interface/tests/dummy.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/idummy.py` & `zope.interface-6.4.post1/src/zope/interface/tests/idummy.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/m1.py` & `zope.interface-6.4.post1/src/zope/interface/tests/m1.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/odd.py` & `zope.interface-6.4.post1/src/zope/interface/tests/odd.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/test_adapter.py` & `zope.interface-6.4.post1/src/zope/interface/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/test_advice.py` & `zope.interface-6.4.post1/src/zope/interface/tests/test_advice.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/test_compile_flags.py` & `zope.interface-6.4.post1/src/zope/interface/tests/test_compile_flags.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/test_declarations.py` & `zope.interface-6.4.post1/src/zope/interface/tests/test_declarations.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/test_document.py` & `zope.interface-6.4.post1/src/zope/interface/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/test_element.py` & `zope.interface-6.4.post1/src/zope/interface/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/test_exceptions.py` & `zope.interface-6.4.post1/src/zope/interface/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/test_interface.py` & `zope.interface-6.4.post1/src/zope/interface/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/test_interfaces.py` & `zope.interface-6.4.post1/src/zope/interface/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/test_odd_declarations.py` & `zope.interface-6.4.post1/src/zope/interface/tests/test_odd_declarations.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/test_registry.py` & `zope.interface-6.4.post1/src/zope/interface/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/test_ro.py` & `zope.interface-6.4.post1/src/zope/interface/tests/test_ro.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/test_sorting.py` & `zope.interface-6.4.post1/src/zope/interface/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/tests/test_verify.py` & `zope.interface-6.4.post1/src/zope/interface/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope/interface/verify.py` & `zope.interface-6.4.post1/src/zope/interface/verify.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/src/zope.interface.egg-info/PKG-INFO` & `zope.interface-6.4.post1/src/zope.interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.interface
-Version: 6.4.post0
+Version: 6.4.post1
 Summary: Interfaces for Python
 Home-page: https://github.com/zopefoundation/zope.interface
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: interface,components,plugins
 Classifier: Development Status :: 5 - Production/Stable
@@ -71,14 +71,21 @@
 
 For detailed documentation, please see https://zopeinterface.readthedocs.io/en/latest/
 
 =========
  Changes
 =========
 
+6.4.post1 (2024-05-23)
+======================
+
+- Publish missing Windows wheels.
+  (`#295 <https://github.com/zopefoundation/zope.interface/issues/295>`_)
+
+
 6.4.post0 (2024-05-22)
 ======================
 
 - The sdist of version 6.4 was uploaded to PyPI as
   ``zope_interface-6.4.tar.gz`` instead of ``zope.interface-6.4-py2.tar.gz``
   which cannot be installed by ``zc.buildout``.  This release is a re-release
   of version 6.4 with the correct sdist name.
```

### Comparing `zope.interface-6.4.post0/src/zope.interface.egg-info/SOURCES.txt` & `zope.interface-6.4.post1/src/zope.interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.4.post0/tox.ini` & `zope.interface-6.4.post1/tox.ini`

 * *Files identical despite different names*

