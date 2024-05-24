# Comparing `tmp/dieke-0.4.0.tar.gz` & `tmp/dieke-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dieke-0.4.0.tar", last modified: Wed May 22 02:24:15 2019, max compression
+gzip compressed data, was "dieke-0.4.1.tar", last modified: Fri May 24 10:46:24 2024, max compression
```

## Comparing `dieke-0.4.0.tar` & `dieke-0.4.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 jevon     (1000) jevon     (1000)        0 2019-05-22 02:24:15.000000 dieke-0.4.0/
--rw-r--r--   0 jevon     (1000) jevon     (1000)      164 2019-05-22 02:23:53.000000 dieke-0.4.0/AUTHORS.rst
--rw-r--r--   0 jevon     (1000) jevon     (1000)      737 2019-05-22 02:23:53.000000 dieke-0.4.0/README.rst
--rw-r--r--   0 jevon     (1000) jevon     (1000)    35147 2019-05-22 02:23:53.000000 dieke-0.4.0/LICENSE
-drwxr-xr-x   0 jevon     (1000) jevon     (1000)        0 2019-05-22 02:24:15.000000 dieke-0.4.0/tests/
-drwxr-xr-x   0 jevon     (1000) jevon     (1000)        0 2019-05-22 02:24:15.000000 dieke-0.4.0/tests/comparison_with_mike/
--rw-r--r--   0 jevon     (1000) jevon     (1000)     6399 2019-05-22 02:23:53.000000 dieke-0.4.0/tests/comparison_with_mike/comparison_with_mikes_log_file.py
--rw-r--r--   0 jevon     (1000) jevon     (1000)     3018 2019-05-22 02:23:53.000000 dieke-0.4.0/tests/comparison_with_mike/eryso_example.py
--rw-r--r--   0 jevon     (1000) jevon     (1000)  2812850 2019-05-22 02:23:53.000000 dieke-0.4.0/tests/comparison_with_mike/375.cfit.log.txt
--rw-r--r--   0 jevon     (1000) jevon     (1000)     4504 2019-05-22 02:23:53.000000 dieke-0.4.0/tests/comparison_with_mike/comparison_with_sebastian_matricies.py
--rw-r--r--   0 jevon     (1000) jevon     (1000)     2339 2019-05-22 02:23:53.000000 dieke-0.4.0/tests/comparison_with_mike/comparison_with_mikes_notes.py
--rw-r--r--   0 jevon     (1000) jevon     (1000)  2569461 2019-05-22 02:23:53.000000 dieke-0.4.0/tests/comparison_with_mike/f11cf_matel.p.gz
--rw-r--r--   0 jevon     (1000) jevon     (1000)     8092 2019-05-22 02:23:53.000000 dieke-0.4.0/tests/test_dieke.py
--rw-r--r--   0 jevon     (1000) jevon     (1000)      685 2019-05-22 02:23:53.000000 dieke-0.4.0/setup.py
--rw-r--r--   0 jevon     (1000) jevon     (1000)     1314 2019-05-22 02:24:15.000000 dieke-0.4.0/PKG-INFO
--rw-r--r--   0 jevon     (1000) jevon     (1000)      317 2019-05-22 02:23:53.000000 dieke-0.4.0/MANIFEST.in
--rw-r--r--   0 jevon     (1000) jevon     (1000)     3500 2019-05-22 02:23:53.000000 dieke-0.4.0/CONTRIBUTING.rst
-drwxr-xr-x   0 jevon     (1000) jevon     (1000)        0 2019-05-22 02:24:15.000000 dieke-0.4.0/dieke.egg-info/
--rw-r--r--   0 jevon     (1000) jevon     (1000)     1416 2019-05-22 02:24:15.000000 dieke-0.4.0/dieke.egg-info/SOURCES.txt
--rw-r--r--   0 jevon     (1000) jevon     (1000)        1 2019-05-22 02:24:15.000000 dieke-0.4.0/dieke.egg-info/dependency_links.txt
--rw-r--r--   0 jevon     (1000) jevon     (1000)     1314 2019-05-22 02:24:15.000000 dieke-0.4.0/dieke.egg-info/PKG-INFO
--rw-r--r--   0 jevon     (1000) jevon     (1000)       41 2019-05-22 02:24:15.000000 dieke-0.4.0/dieke.egg-info/requires.txt
--rw-r--r--   0 jevon     (1000) jevon     (1000)        6 2019-05-22 02:24:15.000000 dieke-0.4.0/dieke.egg-info/top_level.txt
--rw-r--r--   0 jevon     (1000) jevon     (1000)      447 2019-05-22 02:24:15.000000 dieke-0.4.0/setup.cfg
-drwxr-xr-x   0 jevon     (1000) jevon     (1000)        0 2019-05-22 02:24:15.000000 dieke-0.4.0/docs/
--rw-r--r--   0 jevon     (1000) jevon     (1000)      598 2019-05-22 02:23:53.000000 dieke-0.4.0/docs/index.rst
--rw-r--r--   0 jevon     (1000) jevon     (1000)       27 2019-05-22 02:23:53.000000 dieke-0.4.0/docs/readme.rst
--rw-r--r--   0 jevon     (1000) jevon     (1000)      119 2019-05-22 02:23:53.000000 dieke-0.4.0/docs/code.rst
--rw-r--r--   0 jevon     (1000) jevon     (1000)       28 2019-05-22 02:23:53.000000 dieke-0.4.0/docs/authors.rst
--rw-r--r--   0 jevon     (1000) jevon     (1000)     1118 2019-05-22 02:23:53.000000 dieke-0.4.0/docs/installation.rst
--rwxr-xr-x   0 jevon     (1000) jevon     (1000)     4811 2019-05-22 02:23:53.000000 dieke-0.4.0/docs/conf.py
--rw-r--r--   0 jevon     (1000) jevon     (1000)     3083 2019-05-22 02:23:53.000000 dieke-0.4.0/docs/format_of_crosswhite_datafiles.rst
--rw-r--r--   0 jevon     (1000) jevon     (1000)       65 2019-05-22 02:23:53.000000 dieke-0.4.0/docs/usage.rst
--rw-r--r--   0 jevon     (1000) jevon     (1000)      606 2019-05-22 02:23:53.000000 dieke-0.4.0/docs/Makefile
--rw-r--r--   0 jevon     (1000) jevon     (1000)       28 2019-05-22 02:23:53.000000 dieke-0.4.0/docs/history.rst
--rw-r--r--   0 jevon     (1000) jevon     (1000)      767 2019-05-22 02:23:53.000000 dieke-0.4.0/docs/make.bat
--rw-r--r--   0 jevon     (1000) jevon     (1000)       33 2019-05-22 02:23:53.000000 dieke-0.4.0/docs/contributing.rst
-drwxr-xr-x   0 jevon     (1000) jevon     (1000)        0 2019-05-22 02:24:15.000000 dieke-0.4.0/dieke/
-drwxr-xr-x   0 jevon     (1000) jevon     (1000)        0 2019-05-22 02:24:15.000000 dieke-0.4.0/dieke/data/
--rw-r--r--   0 jevon     (1000) jevon     (1000)   121910 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/FIT91sub.for
--rw-r--r--   0 jevon     (1000) jevon     (1000)   820687 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f7mp.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)   651500 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f5mp.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)    67029 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f4nm.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)     2061 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f2nm.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)   216021 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f4mp.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)    51506 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f3mp.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)    51826 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f11mp.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)      520 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/README.txt
--rw-r--r--   0 jevon     (1000) jevon     (1000)      796 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/dy3xtal.d2d
--rw-r--r--   0 jevon     (1000) jevon     (1000)   418128 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f7nm.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)    13848 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f3nm.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)     8362 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f12mp.dat.broken
--rw-r--r--   0 jevon     (1000) jevon     (1000)   217269 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f10mp.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)   198590 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f5nm.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)  1204553 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f8mp.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)    10527 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f12mp.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)     8412 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f2mp.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)   358015 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f6nm.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)  1198515 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f6mp.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)    33746 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/XTAL91.for
--rw-r--r--   0 jevon     (1000) jevon     (1000)    23531 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/FIT91.for
--rw-r--r--   0 jevon     (1000) jevon     (1000)    67180 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/XTAL91sub.for
--rw-r--r--   0 jevon     (1000) jevon     (1000)   654401 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/f9mp.dat
--rw-r--r--   0 jevon     (1000) jevon     (1000)     1585 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/data/dy3fit.c2v
--rw-r--r--   0 jevon     (1000) jevon     (1000)    22016 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/carnall89params.xls
--rw-r--r--   0 jevon     (1000) jevon     (1000)     6907 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/njsymbols.py
--rw-r--r--   0 jevon     (1000) jevon     (1000)    26319 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/__init__.py
--rw-r--r--   0 jevon     (1000) jevon     (1000)    42646 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/sljcalc.py
--rw-r--r--   0 jevon     (1000) jevon     (1000)     4975 2019-05-22 02:23:53.000000 dieke-0.4.0/dieke/wigner.py
--rw-r--r--   0 jevon     (1000) jevon     (1000)      259 2019-05-22 02:23:53.000000 dieke-0.4.0/HISTORY.rst
+drwxr-xr-x   0 lonje61p (1689172356) 1462496566        0 2024-05-24 10:46:24.928562 dieke-0.4.1/
+-rw-r--r--   0 lonje61p (1689172356) 1462496566      164 2022-05-17 01:57:17.000000 dieke-0.4.1/AUTHORS.rst
+-rw-r--r--   0 lonje61p (1689172356) 1462496566     3500 2022-05-17 01:57:17.000000 dieke-0.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 lonje61p (1689172356) 1462496566      259 2022-05-17 01:57:17.000000 dieke-0.4.1/HISTORY.rst
+-rw-r--r--   0 lonje61p (1689172356) 1462496566    35147 2022-05-17 01:57:17.000000 dieke-0.4.1/LICENSE
+-rw-r--r--   0 lonje61p (1689172356) 1462496566      317 2022-05-17 01:57:17.000000 dieke-0.4.1/MANIFEST.in
+-rw-r--r--   0 lonje61p (1689172356) 1462496566     1098 2024-05-24 10:46:24.928646 dieke-0.4.1/PKG-INFO
+-rw-r--r--   0 lonje61p (1689172356) 1462496566      737 2022-05-17 01:57:17.000000 dieke-0.4.1/README.rst
+drwxr-xr-x   0 lonje61p (1689172356) 1462496566        0 2024-05-24 10:46:24.895394 dieke-0.4.1/dieke/
+-rw-r--r--   0 lonje61p (1689172356) 1462496566    26301 2024-05-24 10:33:48.000000 dieke-0.4.1/dieke/__init__.py
+-rw-r--r--   0 lonje61p (1689172356) 1462496566    22016 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/carnall89params.xls
+drwxr-xr-x   0 lonje61p (1689172356) 1462496566        0 2024-05-24 10:46:24.914457 dieke-0.4.1/dieke/data/
+-rw-r--r--   0 lonje61p (1689172356) 1462496566    23531 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/FIT91.for
+-rw-r--r--   0 lonje61p (1689172356) 1462496566   121910 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/FIT91sub.for
+-rw-r--r--   0 lonje61p (1689172356) 1462496566      520 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/README.txt
+-rw-r--r--   0 lonje61p (1689172356) 1462496566    33746 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/XTAL91.for
+-rw-r--r--   0 lonje61p (1689172356) 1462496566    67180 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/XTAL91sub.for
+-rw-r--r--   0 lonje61p (1689172356) 1462496566     1585 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/dy3fit.c2v
+-rw-r--r--   0 lonje61p (1689172356) 1462496566      796 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/dy3xtal.d2d
+-rw-r--r--   0 lonje61p (1689172356) 1462496566   217269 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f10mp.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566    51826 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f11mp.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566    10527 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f12mp.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566     8362 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f12mp.dat.broken
+-rw-r--r--   0 lonje61p (1689172356) 1462496566     8412 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f2mp.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566     2061 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f2nm.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566    51506 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f3mp.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566    13848 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f3nm.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566   216021 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f4mp.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566    67029 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f4nm.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566   651500 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f5mp.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566   198590 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f5nm.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566  1198515 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f6mp.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566   358015 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f6nm.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566   820687 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f7mp.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566   418128 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f7nm.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566  1204553 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f8mp.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566   654401 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/data/f9mp.dat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566     6907 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/njsymbols.py
+-rw-r--r--   0 lonje61p (1689172356) 1462496566    42646 2022-05-17 01:57:17.000000 dieke-0.4.1/dieke/sljcalc.py
+-rw-r--r--   0 lonje61p (1689172356) 1462496566     5008 2024-05-24 09:54:22.000000 dieke-0.4.1/dieke/wigner.py
+drwxr-xr-x   0 lonje61p (1689172356) 1462496566        0 2024-05-24 10:46:24.896014 dieke-0.4.1/dieke.egg-info/
+-rw-r--r--   0 lonje61p (1689172356) 1462496566     1098 2024-05-24 10:46:24.000000 dieke-0.4.1/dieke.egg-info/PKG-INFO
+-rw-r--r--   0 lonje61p (1689172356) 1462496566     1416 2024-05-24 10:46:24.000000 dieke-0.4.1/dieke.egg-info/SOURCES.txt
+-rw-r--r--   0 lonje61p (1689172356) 1462496566        1 2024-05-24 10:46:24.000000 dieke-0.4.1/dieke.egg-info/dependency_links.txt
+-rw-r--r--   0 lonje61p (1689172356) 1462496566       41 2024-05-24 10:46:24.000000 dieke-0.4.1/dieke.egg-info/requires.txt
+-rw-r--r--   0 lonje61p (1689172356) 1462496566        6 2024-05-24 10:46:24.000000 dieke-0.4.1/dieke.egg-info/top_level.txt
+drwxr-xr-x   0 lonje61p (1689172356) 1462496566        0 2024-05-24 10:46:24.917388 dieke-0.4.1/docs/
+-rw-r--r--   0 lonje61p (1689172356) 1462496566      606 2022-05-17 01:57:17.000000 dieke-0.4.1/docs/Makefile
+-rw-r--r--   0 lonje61p (1689172356) 1462496566       28 2022-05-17 01:57:17.000000 dieke-0.4.1/docs/authors.rst
+-rw-r--r--   0 lonje61p (1689172356) 1462496566      119 2022-05-17 01:57:17.000000 dieke-0.4.1/docs/code.rst
+-rwxr-xr-x   0 lonje61p (1689172356) 1462496566     4811 2022-05-17 01:57:17.000000 dieke-0.4.1/docs/conf.py
+-rw-r--r--   0 lonje61p (1689172356) 1462496566       33 2022-05-17 01:57:17.000000 dieke-0.4.1/docs/contributing.rst
+-rw-r--r--   0 lonje61p (1689172356) 1462496566     3083 2022-05-17 01:57:17.000000 dieke-0.4.1/docs/format_of_crosswhite_datafiles.rst
+-rw-r--r--   0 lonje61p (1689172356) 1462496566       28 2022-05-17 01:57:17.000000 dieke-0.4.1/docs/history.rst
+-rw-r--r--   0 lonje61p (1689172356) 1462496566      598 2022-05-17 01:57:17.000000 dieke-0.4.1/docs/index.rst
+-rw-r--r--   0 lonje61p (1689172356) 1462496566     1118 2022-05-17 01:57:17.000000 dieke-0.4.1/docs/installation.rst
+-rw-r--r--   0 lonje61p (1689172356) 1462496566      767 2022-05-17 01:57:17.000000 dieke-0.4.1/docs/make.bat
+-rw-r--r--   0 lonje61p (1689172356) 1462496566       27 2022-05-17 01:57:17.000000 dieke-0.4.1/docs/readme.rst
+-rw-r--r--   0 lonje61p (1689172356) 1462496566       65 2022-05-17 01:57:17.000000 dieke-0.4.1/docs/usage.rst
+-rw-r--r--   0 lonje61p (1689172356) 1462496566      447 2024-05-24 10:46:24.929018 dieke-0.4.1/setup.cfg
+-rw-r--r--   0 lonje61p (1689172356) 1462496566      685 2024-05-24 10:40:05.000000 dieke-0.4.1/setup.py
+drwxr-xr-x   0 lonje61p (1689172356) 1462496566        0 2024-05-24 10:46:24.917540 dieke-0.4.1/tests/
+drwxr-xr-x   0 lonje61p (1689172356) 1462496566        0 2024-05-24 10:46:24.923102 dieke-0.4.1/tests/comparison_with_mike/
+-rw-r--r--   0 lonje61p (1689172356) 1462496566  2812850 2022-05-17 01:57:17.000000 dieke-0.4.1/tests/comparison_with_mike/375.cfit.log.txt
+-rw-r--r--   0 lonje61p (1689172356) 1462496566     6399 2022-05-17 01:57:17.000000 dieke-0.4.1/tests/comparison_with_mike/comparison_with_mikes_log_file.py
+-rw-r--r--   0 lonje61p (1689172356) 1462496566     2339 2022-05-17 01:57:17.000000 dieke-0.4.1/tests/comparison_with_mike/comparison_with_mikes_notes.py
+-rw-r--r--   0 lonje61p (1689172356) 1462496566     4504 2022-05-17 01:57:17.000000 dieke-0.4.1/tests/comparison_with_mike/comparison_with_sebastian_matricies.py
+-rw-r--r--   0 lonje61p (1689172356) 1462496566     3018 2022-05-17 01:57:17.000000 dieke-0.4.1/tests/comparison_with_mike/eryso_example.py
+-rw-r--r--   0 lonje61p (1689172356) 1462496566  2569461 2022-05-17 01:57:17.000000 dieke-0.4.1/tests/comparison_with_mike/f11cf_matel.p.gz
+-rw-r--r--   0 lonje61p (1689172356) 1462496566    10160 2022-07-22 01:50:26.000000 dieke-0.4.1/tests/test_dieke.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dieke-0.4.0/README.rst` & `dieke-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/LICENSE` & `dieke-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/tests/comparison_with_mike/comparison_with_mikes_log_file.py` & `dieke-0.4.1/tests/comparison_with_mike/comparison_with_mikes_log_file.py`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/tests/comparison_with_mike/eryso_example.py` & `dieke-0.4.1/tests/comparison_with_mike/eryso_example.py`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/tests/comparison_with_mike/375.cfit.log.txt` & `dieke-0.4.1/tests/comparison_with_mike/375.cfit.log.txt`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/tests/comparison_with_mike/comparison_with_sebastian_matricies.py` & `dieke-0.4.1/tests/comparison_with_mike/comparison_with_sebastian_matricies.py`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/tests/comparison_with_mike/comparison_with_mikes_notes.py` & `dieke-0.4.1/tests/comparison_with_mike/comparison_with_mikes_notes.py`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/tests/comparison_with_mike/f11cf_matel.p.gz` & `dieke-0.4.1/tests/comparison_with_mike/f11cf_matel.p.gz`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/tests/test_dieke.py` & `dieke-0.4.1/tests/test_dieke.py`

 * *Files 15% similar despite different names*

```diff
@@ -263,7 +263,69 @@
     # This is more of a test because it it only looks at the ground multiplet
     assert(np.max(np.abs(
         calc_nrg_levels[0:8]-seb_levels[0:8]))
            < 0.6 )
 
 
     
+def test_Nd_LaF3():
+    """
+    Tests that we give the same results as Carnall 1989 for Nd:LaF3
+    """
+
+    #energy levels from Carnall's paper
+    #actually I've change 6113 from the carnall paper to 
+    # 6313 because they obvioiusly made a typo!
+
+    carnall_levels = [5, 48, 153, 304, 513,
+                        1965, 2027, 2070, 2089, 2193, 2226,
+                        3902, 3970, 4033, 4087, 4115, 4205, 4267,
+                        5804, 5871, 5999, 6163, 6185, 6313, 6445, 6538, 
+                        11596, 11638,  
+                        ]
+    carnall_levels = np.array(carnall_levels)
+    carnall_levels = carnall_levels-np.min(carnall_levels)
+    
+    nf = 3  # 3 f-electrons means we're dealing with Nd
+    Nd = dieke.RareEarthIon(nf)
+    cfparams = dieke.readLaF3params(nf)
+    
+    # Number of levels and states
+    numLSJ = Nd.numlevels()
+    numLSJmJ = Nd.numstates()
+
+    
+
+    # Make a free-ion Hamiltonian
+    H0 = np.zeros([numLSJmJ, numLSJmJ])
+    for k in cfparams.keys():
+        if k in Nd.FreeIonMatrix:
+            H0 = H0+cfparams[k]*Nd.FreeIonMatrix[k]
+
+    # Add in the crystal field terms 
+    H = H0
+    for k in [2, 4, 6]:
+        for q in range(0, k+1):
+            if 'B%d%d' % (k, q) in cfparams:
+                if q == 0:
+                    H = H+cfparams['B%d%d' % (k, q)]*Nd.Cmatrix(k, q)
+                else:
+                    Bkq = cfparams['B%d%d' % (k, q)]
+                    Bkmq = (-1)**q*np.conj(Bkq)  # B_{k,-q}
+                    Ckq = Nd.Cmatrix(k, q)
+                    Ckmq = Nd.Cmatrix(k, -q)
+                    # See page 44, eq 3.1 of the crystal field handbook
+                    H = H + Bkq*Ckq + Bkmq*Ckmq
+
+
+
+    # Diagonalise the result
+    (evals, evects) = np.linalg.eig(H)
+    E0 = np.min(evals)
+    calc_nrg_levels = np.sort(evals-E0)
+    calc_nrg_levels = np.real(calc_nrg_levels[::2])
+
+    #import pdb; pdb.set_trace()
+    # Assert that they all agree within one wave number
+    assert(np.max(np.abs(
+        calc_nrg_levels[0:len(carnall_levels)]-carnall_levels))
+           < 2.0 )
```

### Comparing `dieke-0.4.0/setup.py` & `dieke-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dieke",
-    version='0.4.0',
+    version='0.4.1',
     author="Jevon Longdell",
     author_email="jevon.longdell@gmail.com",
     description="Crystal field calculations for the rare earths",
     long_description=long_description,
     url="https://github.com/jevonlongdell/dieke",
     packages=['dieke'],
     install_requires=[
         'pandas',
         'xlrd',
         'numpy',
         'scipy',
         'matplotlib',
         'sympy'
     ],
-    classifiers=(
+    classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
-    ),
+    ],
     include_package_data=True
 )
```

### Comparing `dieke-0.4.0/PKG-INFO` & `dieke-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dieke
-Version: 0.4.0
+Version: 0.4.1
 Summary: Crystal field calculations for the rare earths
 Home-page: https://github.com/jevonlongdell/dieke
 Author: Jevon Longdell
 Author-email: jevon.longdell@gmail.com
-License: UNKNOWN
-Description: =====
-        Dieke
-        =====
-        .. image:: https://img.shields.io/pypi/v/dieke.svg
-                :target: https://pypi.python.org/pypi/dieke
-        
-        .. image:: https://travis-ci.org/jevonlongdell/dieke.svg?branch=master
-                :target: https://travis-ci.org/jevonlongdell/dieke
-        
-        .. image:: https://readthedocs.org/projects/dieke/badge/?version=latest
-                :target: https://dieke.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        Crystal field calculations for the Rare Earths
-        
-        
-        * Free software: GNU General Public License v3
-        * Documentation: https://dieke.readthedocs.io.
-        * Requires Python 3.5 or higher
-        
-        Features
-        --------
-        
-        * Reads Crosswhite Fortran datafiles into python code.
-        
-        * Still work in progress. Treat results with caution.
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=====
+Dieke
+=====
+.. image:: https://img.shields.io/pypi/v/dieke.svg
+        :target: https://pypi.python.org/pypi/dieke
+
+.. image:: https://travis-ci.org/jevonlongdell/dieke.svg?branch=master
+        :target: https://travis-ci.org/jevonlongdell/dieke
+
+.. image:: https://readthedocs.org/projects/dieke/badge/?version=latest
+        :target: https://dieke.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+Crystal field calculations for the Rare Earths
+
+
+* Free software: GNU General Public License v3
+* Documentation: https://dieke.readthedocs.io.
+* Requires Python 3.5 or higher
+
+Features
+--------
+
+* Reads Crosswhite Fortran datafiles into python code.
+
+* Still work in progress. Treat results with caution.
+
```

### Comparing `dieke-0.4.0/CONTRIBUTING.rst` & `dieke-0.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke.egg-info/SOURCES.txt` & `dieke-0.4.1/dieke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke.egg-info/PKG-INFO` & `dieke-0.4.1/dieke.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dieke
-Version: 0.4.0
+Version: 0.4.1
 Summary: Crystal field calculations for the rare earths
 Home-page: https://github.com/jevonlongdell/dieke
 Author: Jevon Longdell
 Author-email: jevon.longdell@gmail.com
-License: UNKNOWN
-Description: =====
-        Dieke
-        =====
-        .. image:: https://img.shields.io/pypi/v/dieke.svg
-                :target: https://pypi.python.org/pypi/dieke
-        
-        .. image:: https://travis-ci.org/jevonlongdell/dieke.svg?branch=master
-                :target: https://travis-ci.org/jevonlongdell/dieke
-        
-        .. image:: https://readthedocs.org/projects/dieke/badge/?version=latest
-                :target: https://dieke.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        Crystal field calculations for the Rare Earths
-        
-        
-        * Free software: GNU General Public License v3
-        * Documentation: https://dieke.readthedocs.io.
-        * Requires Python 3.5 or higher
-        
-        Features
-        --------
-        
-        * Reads Crosswhite Fortran datafiles into python code.
-        
-        * Still work in progress. Treat results with caution.
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=====
+Dieke
+=====
+.. image:: https://img.shields.io/pypi/v/dieke.svg
+        :target: https://pypi.python.org/pypi/dieke
+
+.. image:: https://travis-ci.org/jevonlongdell/dieke.svg?branch=master
+        :target: https://travis-ci.org/jevonlongdell/dieke
+
+.. image:: https://readthedocs.org/projects/dieke/badge/?version=latest
+        :target: https://dieke.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+Crystal field calculations for the Rare Earths
+
+
+* Free software: GNU General Public License v3
+* Documentation: https://dieke.readthedocs.io.
+* Requires Python 3.5 or higher
+
+Features
+--------
+
+* Reads Crosswhite Fortran datafiles into python code.
+
+* Still work in progress. Treat results with caution.
+
```

### Comparing `dieke-0.4.0/docs/index.rst` & `dieke-0.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/docs/installation.rst` & `dieke-0.4.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/docs/conf.py` & `dieke-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/docs/format_of_crosswhite_datafiles.rst` & `dieke-0.4.1/docs/format_of_crosswhite_datafiles.rst`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/docs/Makefile` & `dieke-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/docs/make.bat` & `dieke-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/FIT91sub.for` & `dieke-0.4.1/dieke/data/FIT91sub.for`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f7mp.dat` & `dieke-0.4.1/dieke/data/f7mp.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f5mp.dat` & `dieke-0.4.1/dieke/data/f5mp.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f4nm.dat` & `dieke-0.4.1/dieke/data/f4nm.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f2nm.dat` & `dieke-0.4.1/dieke/data/f2nm.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f4mp.dat` & `dieke-0.4.1/dieke/data/f4mp.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f3mp.dat` & `dieke-0.4.1/dieke/data/f3mp.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f11mp.dat` & `dieke-0.4.1/dieke/data/f11mp.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/README.txt` & `dieke-0.4.1/dieke/data/README.txt`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/dy3xtal.d2d` & `dieke-0.4.1/dieke/data/dy3xtal.d2d`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f7nm.dat` & `dieke-0.4.1/dieke/data/f7nm.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f3nm.dat` & `dieke-0.4.1/dieke/data/f3nm.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f12mp.dat.broken` & `dieke-0.4.1/dieke/data/f12mp.dat.broken`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f10mp.dat` & `dieke-0.4.1/dieke/data/f10mp.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f5nm.dat` & `dieke-0.4.1/dieke/data/f5nm.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f8mp.dat` & `dieke-0.4.1/dieke/data/f8mp.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f12mp.dat` & `dieke-0.4.1/dieke/data/f12mp.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f2mp.dat` & `dieke-0.4.1/dieke/data/f2mp.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f6nm.dat` & `dieke-0.4.1/dieke/data/f6nm.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f6mp.dat` & `dieke-0.4.1/dieke/data/f6mp.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/XTAL91.for` & `dieke-0.4.1/dieke/data/XTAL91.for`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/FIT91.for` & `dieke-0.4.1/dieke/data/FIT91.for`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/XTAL91sub.for` & `dieke-0.4.1/dieke/data/XTAL91sub.for`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/f9mp.dat` & `dieke-0.4.1/dieke/data/f9mp.dat`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/data/dy3fit.c2v` & `dieke-0.4.1/dieke/data/dy3fit.c2v`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/carnall89params.xls` & `dieke-0.4.1/dieke/carnall89params.xls`

 * *Files 0% similar despite different names*

```diff
@@ -64,16 +64,16 @@
 000003f0: ffff ffff ffff ffff ffff ffff ffff ffff  ................
 00000400: 5200 6f00 6f00 7400 2000 4500 6e00 7400  R.o.o.t. .E.n.t.
 00000410: 7200 7900 0000 0000 0000 0000 0000 0000  r.y.............
 00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000440: 1600 0500 ffff ffff ffff ffff 0100 0000  ................
 00000450: 2008 0200 0000 0000 c000 0000 0000 0046   ..............F
-00000460: 0000 0000 5299 d7cb 10e8 d401 a079 7b67  ....R........y{g
-00000470: 50fa d401 0300 0000 4003 0000 0000 0000  P.......@.......
+00000460: 0000 0000 5299 d7cb 10e8 d401 6029 7788  ....R.......`)w.
+00000470: 689d d801 0300 0000 4003 0000 0000 0000  h.......@.......
 00000480: 5700 6f00 7200 6b00 6200 6f00 6f00 6b00  W.o.r.k.b.o.o.k.
 00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004c0: 1200 0201 0200 0000 0300 0000 ffff ffff  ................
 000004d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -156,16 +156,16 @@
 000009b0: 0000 0000 0b00 0000 0000 0000 1e10 0000  ................
 000009c0: 0100 0000 0700 0000 5368 6565 7431 000c  ........Sheet1..
 000009d0: 1000 0002 0000 001e 0000 000b 0000 0057  ...............W
 000009e0: 6f72 6b73 6865 6574 7300 0300 0000 0100  orksheets.......
 000009f0: 0000 0000 a800 0000 0300 0000 0000 0000  ................
 00000a00: 0908 1000 0006 0500 6732 cd07 d980 0100  ........g2......
 00000a10: 0606 0000 e100 0200 b004 c100 0200 0000  ................
-00000a20: e200 0000 5c00 7000 0b00 004a 6f6e 6f20  ....\.p....Jono 
-00000a30: 4576 6572 7473 2020 2020 2020 2020 2020  Everts          
+00000a20: e200 0000 5c00 7000 1500 004d 6963 726f  ....\.p....Micro
+00000a30: 736f 6674 204f 6666 6963 6520 5573 6572  soft Office User
 00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000a90: 2020 2020 2020 2020 4200 0200 b004 6101          B.....a.
 00000aa0: 0200 0000 c001 0000 3d01 0200 0100 9c00  ........=.......
```

### Comparing `dieke-0.4.0/dieke/njsymbols.py` & `dieke-0.4.1/dieke/njsymbols.py`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/__init__.py` & `dieke-0.4.1/dieke/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,42 +14,41 @@
 
 np.seterr(all='raise')
 
 """Top-level package for Dieke."""
 
 __author__ = """Jevon Longdell"""
 __email__ = 'jevon.longdell@gmail.com'
-__version__ = '0.4.0'
+__version__ = '0.4.1'
 
 
-def emptymatrix(n,dtype='double'):
-    return lil_matrix((n,n),dtype=dtype)
+def emptymatrix(n, dtype='double'):
+    return lil_matrix((n, n), dtype=dtype)
 #    return np.mat(np.zeros((n,n)))
 
 
 
 class RareEarthIon:
     def __init__(self, nf):
         (self.LStermLabels,
-           self.Uk,
-           self.LSJlevelLabels,
-           self.freeion_mat,
-           self.LSJmJstateLabels,
-           self.FreeIonMatrix,
-           self.Ckq) = makeMatricies(nf)
+         self.Uk,
+         self.LSJlevelLabels,
+         self.freeion_mat,
+         self.LSJmJstateLabels,
+         self.FreeIonMatrix,
+         self.Ckq) = makeMatricies(nf)
         self.N = factorial(14)//(factorial(nf)*factorial(14-nf))
         self.N = int(round(self.N))
         self.nf = nf
 
         L = emptymatrix(self.N, 'double')
         S = emptymatrix(self.N, 'double')
         J = emptymatrix(self.N, 'double')
         mJ = emptymatrix(self.N, 'double')
 
-        
         # The index given in the crosswhite data files
         # to distinguish different terms that have the same
         # L and S
         cwidx = emptymatrix(self.N, 'int')
 
         for ii in range(self.N):
             L[ii, ii] = LfromStateLabel(self.LSJmJstateLabels[ii])
```

### Comparing `dieke-0.4.0/dieke/sljcalc.py` & `dieke-0.4.1/dieke/sljcalc.py`

 * *Files identical despite different names*

### Comparing `dieke-0.4.0/dieke/wigner.py` & `dieke-0.4.1/dieke/wigner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import division
 from scipy.special import factorial
-from scipy import  floor, sqrt
+#from scipy import  floor, sqrt
+from numpy import floor, sqrt  
 from numpy import arange
 
 def Wigner3j(j1,j2,j3,m1,m2,m3):
 #======================================================================
 # Wigner3j.m by David Terr, Raytheon, 6-17-04
 #
 # Compute the Wigner 3j symbol using the Racah formula [1].
```

