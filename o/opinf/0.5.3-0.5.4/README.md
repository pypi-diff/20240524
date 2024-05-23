# Comparing `tmp/opinf-0.5.3.tar.gz` & `tmp/opinf-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opinf-0.5.3.tar", last modified: Wed May 22 19:40:13 2024, max compression
+gzip compressed data, was "opinf-0.5.4.tar", last modified: Thu May 23 22:33:31 2024, max compression
```

## Comparing `opinf-0.5.3.tar` & `opinf-0.5.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.046631 opinf-0.5.3/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1079 2024-05-01 20:01:45.000000 opinf-0.5.3/LICENSE
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     4709 2024-05-22 19:40:13.045617 opinf-0.5.3/PKG-INFO
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1924 2024-05-22 19:31:31.000000 opinf-0.5.3/README.md
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1703 2024-05-22 19:31:31.000000 opinf-0.5.3/pyproject.toml
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       38 2024-05-22 19:40:13.046689 opinf-0.5.3/setup.cfg
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      161 2024-05-01 20:01:45.000000 opinf-0.5.3/setup.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:12.994347 opinf-0.5.3/src/
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.001176 opinf-0.5.3/src/opinf/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      394 2024-05-22 15:36:52.000000 opinf-0.5.3/src/opinf/__init__.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.011859 opinf-0.5.3/src/opinf/basis/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      148 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/basis/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     9891 2024-05-15 19:23:26.000000 opinf-0.5.3/src/opinf/basis/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    10006 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/basis/_linear.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    20882 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/basis/_multi.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    42659 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/basis/_pod.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.013566 opinf-0.5.3/src/opinf/ddt/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      128 2024-05-22 15:36:52.000000 opinf-0.5.3/src/opinf/ddt/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     9495 2024-05-22 15:36:52.000000 opinf-0.5.3/src/opinf/ddt/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    44500 2024-05-22 15:27:01.000000 opinf-0.5.3/src/opinf/ddt/_finite_difference.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      565 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/errors.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.016794 opinf-0.5.3/src/opinf/lift/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      134 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/lift/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     5162 2024-05-22 18:42:48.000000 opinf-0.5.3/src/opinf/lift/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     5660 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/lift/_polynomial.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.021406 opinf-0.5.3/src/opinf/lstsq/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     2764 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/lstsq/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     7598 2024-05-22 19:31:31.000000 opinf-0.5.3/src/opinf/lstsq/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    18892 2024-05-22 19:31:31.000000 opinf-0.5.3/src/opinf/lstsq/_tikhonov.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      937 2024-05-22 19:31:31.000000 opinf-0.5.3/src/opinf/lstsq/_total.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.022259 opinf-0.5.3/src/opinf/models/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      142 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/models/__init__.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.025003 opinf-0.5.3/src/opinf/models/mono/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      183 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/models/mono/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    12644 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/models/mono/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    42167 2024-05-22 19:31:31.000000 opinf-0.5.3/src/opinf/models/mono/_nonparametric.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    55668 2024-05-22 19:31:31.000000 opinf-0.5.3/src/opinf/models/mono/_parametric.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.028412 opinf-0.5.3/src/opinf/models/multi/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      185 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/models/multi/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      106 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/models/multi/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      105 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/models/multi/_nonparametric.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       99 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/models/multi/_parametric.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.031191 opinf-0.5.3/src/opinf/operators/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      178 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/operators/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    22275 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/operators/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    35038 2024-05-22 19:31:31.000000 opinf-0.5.3/src/opinf/operators/_interpolate.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    51458 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/operators/_nonparametric.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.032804 opinf-0.5.3/src/opinf/post/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      111 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/post/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     7938 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/post/_errors.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.036975 opinf-0.5.3/src/opinf/pre/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      155 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/pre/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    11550 2024-05-22 17:53:23.000000 opinf-0.5.3/src/opinf/pre/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    18031 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/pre/_multi.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    27382 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/pre/_shiftscale.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.038210 opinf-0.5.3/src/opinf/roms/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      168 2024-01-12 21:51:13.000000 opinf-0.5.3/src/opinf/roms/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     3611 2024-05-01 16:12:45.000000 opinf-0.5.3/src/opinf/roms/_nonparametric.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       52 2024-01-12 21:52:14.000000 opinf-0.5.3/src/opinf/roms/_parametric.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.043860 opinf-0.5.3/src/opinf/utils/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      178 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/utils/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     4070 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/utils/_hdf5.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      784 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/utils/_mpl_config.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      355 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/utils/_repr.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     3881 2024-05-22 19:31:31.000000 opinf-0.5.3/src/opinf/utils/_reprojection.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1015 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/utils/_requires.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     3089 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/utils/_timer.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.044637 opinf-0.5.3/src/opinf.egg-info/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     4709 2024-05-22 19:40:12.000000 opinf-0.5.3/src/opinf.egg-info/PKG-INFO
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1545 2024-05-22 19:40:12.000000 opinf-0.5.3/src/opinf.egg-info/SOURCES.txt
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        1 2024-05-22 19:40:12.000000 opinf-0.5.3/src/opinf.egg-info/dependency_links.txt
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      156 2024-05-22 19:40:12.000000 opinf-0.5.3/src/opinf.egg-info/requires.txt
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        6 2024-05-22 19:40:12.000000 opinf-0.5.3/src/opinf.egg-info/top_level.txt
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-23 22:33:31.983497 opinf-0.5.4/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1079 2024-05-01 20:01:45.000000 opinf-0.5.4/LICENSE
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     4709 2024-05-23 22:33:31.981526 opinf-0.5.4/PKG-INFO
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1924 2024-05-22 19:31:31.000000 opinf-0.5.4/README.md
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1703 2024-05-22 19:31:31.000000 opinf-0.5.4/pyproject.toml
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       38 2024-05-23 22:33:31.983564 opinf-0.5.4/setup.cfg
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      161 2024-05-01 20:01:45.000000 opinf-0.5.4/setup.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-23 22:33:31.920129 opinf-0.5.4/src/
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-23 22:33:31.925507 opinf-0.5.4/src/opinf/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      425 2024-05-23 22:31:57.000000 opinf-0.5.4/src/opinf/__init__.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-23 22:33:31.937830 opinf-0.5.4/src/opinf/basis/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      148 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/basis/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     9891 2024-05-15 19:23:26.000000 opinf-0.5.4/src/opinf/basis/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    10006 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/basis/_linear.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    20882 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/basis/_multi.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    42659 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/basis/_pod.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-23 22:33:31.939574 opinf-0.5.4/src/opinf/ddt/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      128 2024-05-22 15:36:52.000000 opinf-0.5.4/src/opinf/ddt/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     9495 2024-05-22 15:36:52.000000 opinf-0.5.4/src/opinf/ddt/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    44500 2024-05-22 15:27:01.000000 opinf-0.5.4/src/opinf/ddt/_finite_difference.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      565 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/errors.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-23 22:33:31.946225 opinf-0.5.4/src/opinf/lift/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      134 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/lift/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     5162 2024-05-22 18:42:48.000000 opinf-0.5.4/src/opinf/lift/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     5660 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/lift/_polynomial.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-23 22:33:31.948791 opinf-0.5.4/src/opinf/lstsq/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     2764 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/lstsq/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     7598 2024-05-22 19:31:31.000000 opinf-0.5.4/src/opinf/lstsq/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    18892 2024-05-22 19:31:31.000000 opinf-0.5.4/src/opinf/lstsq/_tikhonov.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      937 2024-05-22 19:31:31.000000 opinf-0.5.4/src/opinf/lstsq/_total.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-23 22:33:31.949752 opinf-0.5.4/src/opinf/models/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      142 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/models/__init__.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-23 22:33:31.955479 opinf-0.5.4/src/opinf/models/mono/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      183 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/models/mono/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    12644 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/models/mono/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    42167 2024-05-22 19:31:31.000000 opinf-0.5.4/src/opinf/models/mono/_nonparametric.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    55668 2024-05-22 19:31:31.000000 opinf-0.5.4/src/opinf/models/mono/_parametric.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-23 22:33:31.957209 opinf-0.5.4/src/opinf/models/multi/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      185 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/models/multi/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      106 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/models/multi/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      105 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/models/multi/_nonparametric.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       99 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/models/multi/_parametric.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-23 22:33:31.964520 opinf-0.5.4/src/opinf/operators/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      178 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/operators/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    22275 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/operators/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    35038 2024-05-22 19:31:31.000000 opinf-0.5.4/src/opinf/operators/_interpolate.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    51458 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/operators/_nonparametric.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-23 22:33:31.965915 opinf-0.5.4/src/opinf/post/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      111 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/post/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     7938 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/post/_errors.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-23 22:33:31.970165 opinf-0.5.4/src/opinf/pre/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      155 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/pre/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    11564 2024-05-23 22:31:57.000000 opinf-0.5.4/src/opinf/pre/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    18045 2024-05-23 22:31:57.000000 opinf-0.5.4/src/opinf/pre/_multi.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    27396 2024-05-23 22:31:57.000000 opinf-0.5.4/src/opinf/pre/_shiftscale.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-23 22:33:31.971635 opinf-0.5.4/src/opinf/roms/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      168 2024-05-23 22:31:57.000000 opinf-0.5.4/src/opinf/roms/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    11201 2024-05-23 22:31:57.000000 opinf-0.5.4/src/opinf/roms/_nonparametric.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       66 2024-05-23 22:31:57.000000 opinf-0.5.4/src/opinf/roms/_parametric.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-23 22:33:31.979513 opinf-0.5.4/src/opinf/utils/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      178 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/utils/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     4070 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/utils/_hdf5.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      784 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/utils/_mpl_config.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      355 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/utils/_repr.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     3881 2024-05-22 19:31:31.000000 opinf-0.5.4/src/opinf/utils/_reprojection.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1015 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/utils/_requires.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     3089 2024-05-01 20:01:45.000000 opinf-0.5.4/src/opinf/utils/_timer.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-23 22:33:31.980283 opinf-0.5.4/src/opinf.egg-info/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     4709 2024-05-23 22:33:31.000000 opinf-0.5.4/src/opinf.egg-info/PKG-INFO
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1545 2024-05-23 22:33:31.000000 opinf-0.5.4/src/opinf.egg-info/SOURCES.txt
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        1 2024-05-23 22:33:31.000000 opinf-0.5.4/src/opinf.egg-info/dependency_links.txt
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      156 2024-05-23 22:33:31.000000 opinf-0.5.4/src/opinf.egg-info/requires.txt
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        6 2024-05-23 22:33:31.000000 opinf-0.5.4/src/opinf.egg-info/top_level.txt
```

### Comparing `opinf-0.5.3/LICENSE` & `opinf-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/PKG-INFO` & `opinf-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opinf
-Version: 0.5.3
+Version: 0.5.4
 Summary: Operator Inference for data-driven model reduction of dynamical systems.
 Author-email: Willcox Research Group <kwillcox@oden.utexas.edu>
 Maintainer-email: "Shane A. McQuarrie" <smcquar@sandia.gov>
 License: MIT License
         
         Copyright (c) 2023 Willcox Research Group
```

### Comparing `opinf-0.5.3/README.md` & `opinf-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/pyproject.toml` & `opinf-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/basis/_base.py` & `opinf-0.5.4/src/opinf/basis/_base.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/basis/_linear.py` & `opinf-0.5.4/src/opinf/basis/_linear.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/basis/_multi.py` & `opinf-0.5.4/src/opinf/basis/_multi.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/basis/_pod.py` & `opinf-0.5.4/src/opinf/basis/_pod.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/ddt/_base.py` & `opinf-0.5.4/src/opinf/ddt/_base.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/ddt/_finite_difference.py` & `opinf-0.5.4/src/opinf/ddt/_finite_difference.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/errors.py` & `opinf-0.5.4/src/opinf/errors.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/lift/_base.py` & `opinf-0.5.4/src/opinf/lift/_base.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/lift/_polynomial.py` & `opinf-0.5.4/src/opinf/lift/_polynomial.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/lstsq/__init__.py` & `opinf-0.5.4/src/opinf/lstsq/__init__.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/lstsq/_base.py` & `opinf-0.5.4/src/opinf/lstsq/_base.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/lstsq/_tikhonov.py` & `opinf-0.5.4/src/opinf/lstsq/_tikhonov.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/lstsq/_total.py` & `opinf-0.5.4/src/opinf/lstsq/_total.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/models/mono/_base.py` & `opinf-0.5.4/src/opinf/models/mono/_base.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/models/mono/_nonparametric.py` & `opinf-0.5.4/src/opinf/models/mono/_nonparametric.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/models/mono/_parametric.py` & `opinf-0.5.4/src/opinf/models/mono/_parametric.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/operators/_base.py` & `opinf-0.5.4/src/opinf/operators/_base.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/operators/_interpolate.py` & `opinf-0.5.4/src/opinf/operators/_interpolate.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/operators/_nonparametric.py` & `opinf-0.5.4/src/opinf/operators/_nonparametric.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/post/_errors.py` & `opinf-0.5.4/src/opinf/post/_errors.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/pre/_base.py` & `opinf-0.5.4/src/opinf/pre/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
             untransform.
         locs : slice or (p,) ndarray of integers or None
             If given, assume ``states_transformed`` contains the transformed
             snapshots at only the `p` indices described by ``locs``.
 
         Returns
         -------
-        states: (n, ...) or (p, ...) ndarray
+        states_untransformed: (n, ...) or (p, ...) ndarray
             Matrix of `n`-dimensional untransformed snapshots, or the `p`
             entries of such at the indices specified by ``locs``.
         """
         raise NotImplementedError  # pragma: no cover
 
     # Model persistence -------------------------------------------------------
     def save(self, savefile, overwrite=False):
```

### Comparing `opinf-0.5.3/src/opinf/pre/_multi.py` & `opinf-0.5.4/src/opinf/pre/_multi.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
             If given, assume ``states_transformed`` contains the `p` entries
             of each transformed state variable at the indices specified by
             ``locs``. This option requires each state variable to have the
             same dimension.
 
         Returns
         -------
-        states: (n, ...) or (num_variables*p, ...) ndarray
+        states_untransformed: (n, ...) or (num_variables*p, ...) ndarray
             Matrix of `n`-dimensional untransformed snapshots, or the
             :math:`n_q p` entries of such at the indices specified by ``locs``.
         """
         if locs is not None:
             if len(set(self.variable_sizes)) > 1:
                 raise ValueError(
                     "'locs != None' requires that "
```

### Comparing `opinf-0.5.3/src/opinf/pre/_shiftscale.py` & `opinf-0.5.4/src/opinf/pre/_shiftscale.py`

 * *Files 0% similar despite different names*

```diff
@@ -630,15 +630,15 @@
             untransform.
         locs : slice or (p,) ndarray of integers or None
             If given, assume ``states_transformed`` contains the transformed
             snapshots at only the `p` indices described by ``locs``.
 
         Returns
         -------
-        states: (n, ...) or (p, ...) ndarray
+        states_untransformed: (n, ...) or (p, ...) ndarray
             Matrix of `n`-dimensional untransformed snapshots, or the `p`
             entries of such at the indices specified by ``locs``.
         """
         self._check_is_trained()
 
         if locs is not None:
             if isinstance(locs, slice):
```

### Comparing `opinf-0.5.3/src/opinf/utils/_hdf5.py` & `opinf-0.5.4/src/opinf/utils/_hdf5.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/utils/_mpl_config.py` & `opinf-0.5.4/src/opinf/utils/_mpl_config.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/utils/_reprojection.py` & `opinf-0.5.4/src/opinf/utils/_reprojection.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/utils/_requires.py` & `opinf-0.5.4/src/opinf/utils/_requires.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf/utils/_timer.py` & `opinf-0.5.4/src/opinf/utils/_timer.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.3/src/opinf.egg-info/PKG-INFO` & `opinf-0.5.4/src/opinf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opinf
-Version: 0.5.3
+Version: 0.5.4
 Summary: Operator Inference for data-driven model reduction of dynamical systems.
 Author-email: Willcox Research Group <kwillcox@oden.utexas.edu>
 Maintainer-email: "Shane A. McQuarrie" <smcquar@sandia.gov>
 License: MIT License
         
         Copyright (c) 2023 Willcox Research Group
```

### Comparing `opinf-0.5.3/src/opinf.egg-info/SOURCES.txt` & `opinf-0.5.4/src/opinf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

