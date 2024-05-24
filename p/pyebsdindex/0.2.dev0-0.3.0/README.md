# Comparing `tmp/pyebsdindex-0.2.dev0.tar.gz` & `tmp/pyebsdindex-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyebsdindex-0.2.dev0.tar", last modified: Sat May  6 11:03:22 2023, max compression
+gzip compressed data, was "pyebsdindex-0.3.0.tar", last modified: Thu May 23 21:09:37 2024, max compression
```

## Comparing `pyebsdindex-0.2.dev0.tar` & `pyebsdindex-0.3.0.tar`

### file list

```diff
@@ -1,92 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.504583 pyebsdindex-0.2.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    48700 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/IPFCubic.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    49952 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/IPFCubic.png
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/License
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-06 11:03:22.504583 pyebsdindex-0.2.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/RELEASE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.488583 pyebsdindex-0.2.dev0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.488583 pyebsdindex-0.2.dev0/doc/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.492583 pyebsdindex-0.2.dev0/doc/_static/colormap_banners/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_static/colormap_banners/banner0.png
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_static/colormap_banners/banner1.png
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_static/colormap_banners/create_colormap_banners.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.492583 pyebsdindex-0.2.dev0/doc/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.492583 pyebsdindex-0.2.dev0/doc/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/custom-attribute-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/custom-function-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/custom-method-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.492583 pyebsdindex-0.2.dev0/doc/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.492583 pyebsdindex-0.2.dev0/doc/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.496583 pyebsdindex-0.2.dev0/doc/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/tutorials/NLPAR_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   634518 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/tutorials/ebsd_index_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/tutorials/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.496583 pyebsdindex-0.2.dev0/doc/user/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/user/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/user/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.500583 pyebsdindex-0.2.dev0/pyebsdindex/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.500583 pyebsdindex-0.2.dev0/pyebsdindex/EBSDImage/
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/EBSDImage/IPFcolor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/EBSDImage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/_ebsd_index_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    21731 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/_ebsd_index_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    21899 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/band_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)    34349 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/band_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/crystal_sym.py
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/crystallometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/ebsd_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    31299 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/ebsd_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/ebsdfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/nlpar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.500583 pyebsdindex-0.2.dev0/pyebsdindex/opencl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/opencl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26661 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/opencl/band_detect_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/opencl/clkernels.cl
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/opencl/openclparam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/opencl/radon_fast_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/pairlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/pcopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/radon_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    22234 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    51672 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/rotlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/spherical_radon_fast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.504583 pyebsdindex-0.2.dev0/pyebsdindex/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.484583 pyebsdindex-0.2.dev0/pyebsdindex/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.504583 pyebsdindex-0.2.dev0/pyebsdindex/tests/data/al_sim_20kv/
--rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/data/al_sim_20kv/generate_al_sim_20kv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/numbatest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/raytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/rotlibunittest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/test_ebsd_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/test_pcopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tripletlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.500583 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-06 11:03:22.504583 pyebsdindex-0.2.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.831491 pyebsdindex-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   368506 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/IPFCubic.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   147377 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/IPFCubic.png
+-rw-r--r--   0 runner    (1001) docker     (127)   197654 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/IPFHex.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    82053 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/IPFHex.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/License
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-23 21:09:37.831491 pyebsdindex-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/RELEASE.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.811491 pyebsdindex-0.3.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.811491 pyebsdindex-0.3.0/doc/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.811491 pyebsdindex-0.3.0/doc/_static/colormap_banners/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/_static/colormap_banners/banner0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/_static/colormap_banners/banner1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/_static/colormap_banners/create_colormap_banners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.811491 pyebsdindex-0.3.0/doc/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.811491 pyebsdindex-0.3.0/doc/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/_templates/custom-attribute-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/_templates/custom-function-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/_templates/custom-method-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.811491 pyebsdindex-0.3.0/doc/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.811491 pyebsdindex-0.3.0/doc/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.815491 pyebsdindex-0.3.0/doc/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/tutorials/NLPAR_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1570100 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/tutorials/ebsd_index_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/tutorials/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.815491 pyebsdindex-0.3.0/doc/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/user/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/doc/user/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.819491 pyebsdindex-0.3.0/pyebsdindex/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.823491 pyebsdindex-0.3.0/pyebsdindex/EBSDImage/
+-rw-r--r--   0 runner    (1001) docker     (127)    12490 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/EBSDImage/IPFcolor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/EBSDImage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34888 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/_ebsd_index_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33740 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/_ebsd_index_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28606 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/band_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/crystal_sym.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/crystallometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/ebsd_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50809 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/ebsd_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12787 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/ebsdfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/misorientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/nlpar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29024 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/nlpar_cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.823491 pyebsdindex-0.3.0/pyebsdindex/opencl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/opencl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29511 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/opencl/band_detect_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28523 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/opencl/clkernels.cl
+-rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/opencl/clnlpar.cl
+-rw-r--r--   0 runner    (1001) docker     (127)    20626 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/opencl/nlpar_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28570 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/opencl/nlpar_clray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/opencl/openclparam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/opencl/radon_fast_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/opencl/test.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/pairlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20611 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/pcopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14993 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/radon_fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22234 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51834 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/rotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.827491 pyebsdindex-0.3.0/pyebsdindex/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.807491 pyebsdindex-0.3.0/pyebsdindex/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.827491 pyebsdindex-0.3.0/pyebsdindex/tests/data/al_sim_20kv/
+-rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/tests/data/al_sim_20kv/generate_al_sim_20kv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/tests/numbatest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/tests/raytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/tests/rotlibunittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/tests/test_ebsd_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/tests/test_pcopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/tests/test_tripletvote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67523 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/pyebsdindex/tripletvote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:37.827491 pyebsdindex-0.3.0/pyebsdindex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-23 21:09:37.000000 pyebsdindex-0.3.0/pyebsdindex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-23 21:09:37.000000 pyebsdindex-0.3.0/pyebsdindex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:09:37.000000 pyebsdindex-0.3.0/pyebsdindex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-23 21:09:37.000000 pyebsdindex-0.3.0/pyebsdindex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 21:09:37.000000 pyebsdindex-0.3.0/pyebsdindex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:09:37.000000 pyebsdindex-0.3.0/pyebsdindex.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-23 21:09:37.831491 pyebsdindex-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-23 21:09:33.000000 pyebsdindex-0.3.0/setup.py
```

### Comparing `pyebsdindex-0.2.dev0/.readthedocs.yaml` & `pyebsdindex-0.3.0/.readthedocs.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# ..readthedocs.yaml
+# .readthedocs.yaml
 # Read the Docs configuration file
 # See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
 
 # Required
 version: 2
 
 # Build documentation in the doc/ directory with Sphinx
 sphinx:
   configuration: doc/conf.py
 
 # Set the version of Python and other tools you might need
 build:
-  os: ubuntu-20.04
+  os: ubuntu-22.04
   tools:
-    python: "3.9"
+    python: "3.11"
 
 # Build doc in all formats (HTML, PDF and ePub)
 formats:
   - htmlzip
   - pdf
 
 # Python environment for building the docs
```

### Comparing `pyebsdindex-0.2.dev0/License` & `pyebsdindex-0.3.0/License`

 * *Files 1% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 that you changed the software and should note the date and nature of any such change.
 Please explicitly acknowledge the US Naval Research Laboratory as the original source.
 This software can be redistributed and/or modified freely provided that any derivative
 works bear some notice that they are derived from it, and any modified versions bear
 some notice that they have been modified.
 
 Author: David Rowenhorst; 
-The US Naval Research Laboratory Date: 21 Aug 2020
+The US Naval Research Laboratory Date: 22 May 2024
```

### Comparing `pyebsdindex-0.2.dev0/PKG-INFO` & `pyebsdindex-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,32 @@
-Metadata-Version: 2.1
-Name: pyebsdindex
-Version: 0.2.dev0
-Summary: Python based tool for Hough/Radon based EBSD indexing
-Home-page: https://pyebsdindex.readthedocs.io
-Download-URL: https://pypi.python.org/pypi/pyebsdindex
-Author: ['Dave Rowenhorst', 'Håkon Wiik Ånes']
-Maintainer: Dave Rowenhorst
-Maintainer-email: 
-License: Custom
-Project-URL: Bug Tracker, https://github.com/USNavalResearchLaboratory/PyEBSDIndex/issues
-Project-URL: Documentation, https://pyebsdindex.readthedocs.io
-Project-URL: Source Code, https://github.com/USNavalResearchLaboratory/PyEBSDIndex
-Keywords: EBSD,electron backscatter diffraction,HI,Hough indexing,NLPAR
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: Other/Proprietary License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: doc
-Provides-Extra: tests
-Provides-Extra: gpu
-Provides-Extra: parallel
-Provides-Extra: dev
-Provides-Extra: all
-License-File: License
-
 # PyEBSDIndex
 
-Python based tool for Hough/Radon based EBSD orientation indexing.
+Python based tool for Radon based EBSD orientation indexing.
 
-[![Build status](https://github.com/USNavalResearchLaboratory/PyEBSDIndex/actions/workflows/build.yml/badge.svg)](https://github.com/USNavalResearchLaboratory/PyEBSDIndex/actions/workflows/build.yml)
+[![Tests status](https://github.com/USNavalResearchLaboratory/PyEBSDIndex/actions/workflows/tests.yml/badge.svg)](https://github.com/USNavalResearchLaboratory/PyEBSDIndex/actions/workflows/tests.yml)
 [![Documentation status](https://readthedocs.org/projects/pyebsdindex/badge/?version=latest)](https://pyebsdindex.readthedocs.io/en/latest/)
 [![PyPI version](https://img.shields.io/pypi/v/pyebsdindex.svg)](https://pypi.python.org/pypi/pyebsdindex)
 
-The pattern processing is based on a GPU pipeline, and is based on the work of S. I.
-Wright and B. L. Adams. Metallurgical Transactions A-Physical Metallurgy and Materials
-Science, 23(3):759–767, 1992, and N. Krieger Lassen. Automated Determination of Crystal
-Orientations from Electron Backscattering Patterns. PhD thesis, The Technical University
-of Denmark, 1994.
+The pattern processing is based on a GPU pipeline.  Details can be found
+in D. J. Rowenhorst, P. G. Callahan, H. W. Ånes. Fast Radon transforms for
+high-precision EBSD orientation determination using PyEBSDIndex. Journal of
+Applied Crystallography, 57(1):3–19, 2024. and is based on the work of S. I.
+Wright and B. L. Adams. Metallurgical Transactions A-Physical Metallurgy and
+Materials Science, 23(3):759–767, 1992, and N. Krieger Lassen. Automated
+Determination of Crystal Orientations from Electron Backscattering Patterns.
+PhD thesis, The Technical University of Denmark, 1994. 
 
 The band indexing is achieved through triplet voting using the methods outlined by A.
 Morawiec. Acta Crystallographica Section A Foundations and Advances, 76(6):719–734,
 2020.
 
 Additionally NLPAR pattern processing is included (original distribution
 [NLPAR](https://github.com/USNavalResearchLaboratory/NLPAR); P. T. Brewick, S. I.
 Wright, and D. J. Rowenhorst. Ultramicroscopy, 200:50–61, May 2019.).
 
 Documentation with installation instructions, a user guide, API reference, changelog,
 and contributing guide is available at https://pyebsdindex.readthedocs.io.
 
 ## Installation
 
-See [the documentation](https://pyebsdindex.readthedocs.io/en/latest/installation.html)
+See [the documentation](https://pyebsdindex.readthedocs.io/en/stable/installation.html)
 for installation instructions.
```

### Comparing `pyebsdindex-0.2.dev0/RELEASE.rst` & `pyebsdindex-0.3.0/RELEASE.rst`

 * *Files 13% similar despite different names*

```diff
@@ -21,10 +21,10 @@
   published to PyPI.
 
 Post-release action
 -------------------
 - Monitor the `documentation build
   <https://readthedocs.org/projects/pyebsdindex/builds>`_ to ensure that the new stable
   documentation is successfully built from the release.
-- Make a post-release PR to ``main`` with ``__version__`` updated (or reverted), e.g. to
-  "0.4.dev0", and any updates to this guide if necessary.
+- Make a post-release PR to ``main`` with ``__version__`` in ``__init__.py`` updated (or reverted),
+  and in ``CHANGELOG.rst`` e.g. to "0.4.dev0", and any updates to this guide if necessary
 - Tidy up GitHub issues.
```

### Comparing `pyebsdindex-0.2.dev0/doc/Makefile` & `pyebsdindex-0.3.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/doc/_static/colormap_banners/banner0.png` & `pyebsdindex-0.3.0/doc/_static/colormap_banners/banner0.png`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/doc/_static/colormap_banners/banner1.png` & `pyebsdindex-0.3.0/doc/_static/colormap_banners/banner1.png`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/doc/_static/colormap_banners/create_colormap_banners.py` & `pyebsdindex-0.3.0/doc/_static/colormap_banners/create_colormap_banners.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/doc/_static/custom.css` & `pyebsdindex-0.3.0/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/doc/_templates/custom-class-template.rst` & `pyebsdindex-0.3.0/doc/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/doc/_templates/custom-module-template.rst` & `pyebsdindex-0.3.0/doc/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/doc/conf.py` & `pyebsdindex-0.3.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/doc/dev/index.rst` & `pyebsdindex-0.3.0/doc/dev/index.rst`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/doc/index.rst` & `pyebsdindex-0.3.0/doc/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===================================
 PyEBSDIndex |release| documentation
 ===================================
 
-Python based tool for Hough/Radon based EBSD orientation indexing.
+Python based tool for Radon based EBSD orientation indexing.
 
 The pattern processing is based on a GPU pipeline, and is based on the work of S. I.
 Wright and B. L. Adams. Metallurgical Transactions A-Physical Metallurgy and Materials
 Science, 23(3):759–767, 1992, and N. C. Krieger Lassen. Automated Determination of
 Crystal Orientations from Electron Backscattering Patterns. PhD thesis, The Technical
 University of Denmark, 1994.
```

### Comparing `pyebsdindex-0.2.dev0/doc/make.bat` & `pyebsdindex-0.3.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/doc/reference/index.rst` & `pyebsdindex-0.3.0/doc/reference/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -28,7 +28,8 @@
 .. autosummary::
     :toctree: generated
     :template: custom-module-template.rst
 
     ebsd_index
     nlpar
     pcopt
+    tripletvote
```

### Comparing `pyebsdindex-0.2.dev0/doc/tutorials/NLPAR_demo.ipynb` & `pyebsdindex-0.3.0/doc/tutorials/NLPAR_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/doc/user/installation.rst` & `pyebsdindex-0.3.0/doc/user/installation.rst`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/__init__.py` & `pyebsdindex-0.3.0/pyebsdindex/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 __author__ = "Dave Rowenhorst"
 __author_email__ = ""
 # Initial committer first, then sorted by line contributions
 __credits__ = [
     "Dave Rowenhorst",
     "Håkon Wiik Ånes",
 ]
-__description__ = "Python based tool for Hough/Radon based EBSD indexing"
+__description__ = "Python based tool for Radon based EBSD indexing"
 __name__ = "pyebsdindex"
-__version__ = "0.2.dev0"
+__version__ = "0.3.0"
 
 
-# Try to import only once
+# Try to import only once - also will perform check that at least one GPU is found.
 try:
+    _pyopencl_installed = False
     import pyopencl
-    _pyopencl_installed = True
+    from pyebsdindex.opencl import openclparam
+    testcl = openclparam.OpenClParam()
+    try:
+        gpu = testcl.get_gpu()
+        if len(gpu) > 0:
+            _pyopencl_installed = True
+    except:
+        raise ImportError('pyopencl could not find GPU')
 except ImportError:
     _pyopencl_installed = False
 
 try:
     import ray
     _ray_installed = True
 except ImportError:
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/band_detect.py` & `pyebsdindex-0.3.0/pyebsdindex/band_detect.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,69 @@
-"""This software was developed by employees of the US Naval Research Laboratory (NRL), an
-agency of the Federal Government. Pursuant to title 17 section 105 of the United States
-Code, works of NRL employees are not subject to copyright protection, and this software
-is in the public domain. PyEBSDIndex is an experimental system. NRL assumes no
-responsibility whatsoever for its use by other parties, and makes no guarantees,
-expressed or implied, about its quality, reliability, or any other characteristic. We
-would appreciate acknowledgment if the software is used. To the extent that NRL may hold
-copyright in countries other than the United States, you are hereby granted the
-non-exclusive irrevocable and unconditional right to print, publish, prepare derivative
-works and distribute this software, in any medium, or authorize others to do so on your
-behalf, on a royalty-free basis throughout the world. You may improve, modify, and
-create derivative works of the software or any portion of the software, and you may copy
-and distribute such modifications or works. Modified works should carry a notice stating
-that you changed the software and should note the date and nature of any such change.
-Please explicitly acknowledge the US Naval Research Laboratory as the original source.
-This software can be redistributed and/or modified freely provided that any derivative
-works bear some notice that they are derived from it, and any modified versions bear
-some notice that they have been modified.
-
-Author: David Rowenhorst;
-The US Naval Research Laboratory Date: 21 Aug 2020"""
-
-from os import environ
-from pathlib import PurePath
+# This software was developed by employees of the US Naval Research Laboratory (NRL), an
+# agency of the Federal Government. Pursuant to title 17 section 105 of the United States
+# Code, works of NRL employees are not subject to copyright protection, and this software
+# is in the public domain. PyEBSDIndex is an experimental system. NRL assumes no
+# responsibility whatsoever for its use by other parties, and makes no guarantees,
+# expressed or implied, about its quality, reliability, or any other characteristic. We
+# would appreciate acknowledgment if the software is used. To the extent that NRL may hold
+# copyright in countries other than the United States, you are hereby granted the
+# non-exclusive irrevocable and unconditional right to print, publish, prepare derivative
+# works and distribute this software, in any medium, or authorize others to do so on your
+# behalf, on a royalty-free basis throughout the world. You may improve, modify, and
+# create derivative works of the software or any portion of the software, and you may copy
+# and distribute such modifications or works. Modified works should carry a notice stating
+# that you changed the software and should note the date and nature of any such change.
+# Please explicitly acknowledge the US Naval Research Laboratory as the original source.
+# This software can be redistributed and/or modified freely provided that any derivative
+# works bear some notice that they are derived from it, and any modified versions bear
+# some notice that they have been modified.
+#
+#
+# Author: David Rowenhorst;
+# The US Naval Research Laboratory Date: 22 May 2024
+#
+# For further information see:
+# David J. Rowenhorst, Patrick G. Callahan, Håkon W. Ånes. Fast Radon transforms for
+# high-precision EBSD orientation determination using PyEBSDIndex.
+# Journal of Applied Crystallography, 57(1):3–19, 2024.
+# DOI: 10.1107/S1600576723010221
+#
+#
+
+"""Class that reads in EBSD patterns, and finds the bands within those patterns using a Radon Transform."""
+
+#from os import environ
+import os
+from pathlib import PurePath, Path
 import platform
-import tempfile
+# import tempfile
 from timeit import default_timer as timer
 
 import matplotlib.pyplot as plt
 import numba
 import numpy as np
-from scipy.ndimage import gaussian_filter
-from scipy.ndimage import grey_dilation as scipy_grey_dilation
-import scipy.optimize as opt
 
-from pyebsdindex import radon_fast
+import scipy.ndimage as scipyndim #import gaussian_filter, dilation ...
+#from scipy.ndimage #import grey_dilation as scipy_grey_dilation
+#from scipy.ndimage #import median_filter
+import scipy.optimize as scipyopt
 
+from pyebsdindex import radon_fast
 
-tempdir = PurePath("/tmp" if platform.system() == "Darwin" else tempfile.gettempdir())
-tempdir = tempdir.joinpath('numba')
-environ["NUMBA_CACHE_DIR"] = str(tempdir)
+tempdir = PurePath(Path.home())
+#tempdir = PurePath("/tmp" if platform.system() == "Darwin" else tempfile.gettempdir())
+#tempdir = tempdir.joinpath('numbacache')
+tempdir = tempdir.joinpath('.pyebsdindex').joinpath('numbacache')
+Path(tempdir).mkdir(parents=True, exist_ok=True)
+os.environ["NUMBA_CACHE_DIR"] = str(tempdir)+str(os.sep)
 
 RADEG = 180.0/np.pi
 
 
-class BandDetect:
+class BandDetect():
   def __init__(
     self,
     patterns=None,
     patDim=None,
     nTheta=180,
     nRho=90,
     tSigma=None,
@@ -67,36 +83,52 @@
     self.tSigma = tSigma
     self.rSigma = rSigma
     self.kernel = None
     self.peakPad = np.array([11, 11])
     self.padding = np.array([11, 11])
     self.rhoMaskFrac = rhoMaskFrac
 
+    self.rhomask1thresh = None
+    self.rhomask1 = None
+
     self.nBands = nBands
     self.EDAXIQ = False
     self.backgroundsub = None
+    self.patternmask = None
+    self.useCPU = True
 
     self.dataType = np.dtype([('id', np.int32), ('max', np.float32), \
                     ('maxloc', np.float32, (2)), ('avemax', np.float32), ('aveloc', np.float32, (2)),\
                     ('pqmax', np.float32), ('width', np.float32), ('theta', np.float32), ('rho', np.float32),
-                    ('valid', np.int8)])
+                    ('valid', np.int8),('band_match_index', np.int32, (2))])
 
 
     if (patterns is None) and (patDim is None):
       pass
     else:
       if (patterns is not None):
         self.patDim = np.asarray(patterns.shape[-2:])
       else:
         self.patDim = np.asarray(patDim)
+      patternmask = None
+      if 'patternmask' in kwargs :
+        patternmask = kwargs.get('patternmask')
+
+      patternmaskindex = None
+      if 'patternmaskindex' in kwargs:
+        patternmaskindex = kwargs.get('patternmaskindex')
+      #print(patternmask)
       self.band_detect_setup(patterns, self.patDim,self.nTheta,self.nRho,\
-                self.tSigma, self.rSigma,self.rhoMaskFrac,self.nBands)
+                             self.tSigma, self.rSigma,self.rhoMaskFrac,self.nBands,
+                             patternmask = patternmask,patternmaskindex = patternmaskindex,
+                             **kwargs)
 
   def band_detect_setup(self, patterns=None,patDim=None,nTheta=None,nRho=None,\
-                      tSigma=None, rSigma=None,rhoMaskFrac=None,nBands=None):
+                      tSigma=None, rSigma=None,rhoMaskFrac=None,nBands=None,
+                      patternmask=None, patternmaskindex=None, **kwargs):
     p_dim = None
     recalc_radon = False
     recalc_masks = False
     if (patterns is None) and (patDim is not None):
       p_dim = np.asarray(patDim, dtype=np.int64)
     if patterns is not None:
       p_dim = np.shape(patterns)[-2:]  # this will catch if someone sends in a [1 x N x M] image
@@ -122,23 +154,80 @@
       self.nRho = nRho
       recalc_radon = True
       recalc_masks = True
 
     if self.dRho is None:
       recalc_radon = True
 
+    #recalc_radon = True
     if recalc_radon == True:
-      #self.rhoMax = 0.5 * np.float32(np.sqrt(np.float32(self.patDim[0])**2  + np.float32(self.patDim[1])**2))
-      self.rhoMax = 0.5 * np.float32(self.patDim.min())
+      if (self.rhoMaskFrac < 1) and (self.rhoMaskFrac > 0):
+        self.rhoMax = 0.5 * np.float32(self.patDim.min())
+      else:
+        self.rhoMax = 0.5 * np.float32(np.sqrt(np.float32(self.patDim[-2])**2  + np.float32(self.patDim[-1])**2))
+
+      self.rhomask1thresh = np.float32(self.patDim.min())*0.1
+
       self.dRho = self.rhoMax/np.float32(self.nRho)
-      self.radonPlan = radon_fast.Radon(imageDim=self.patDim, nTheta=self.nTheta, nRho=self.nRho, rhoMax=self.rhoMax)
-      temp = np.ones(self.patDim[-2:], dtype=np.float32)
-      back = self.radonPlan.radon_faster(temp,fixArtifacts=True)
-      back = (back > 0).astype(np.float32) / (back + 1.0e-12)
-      self.rdnNorm = back
+      self.radonPlan = radon_fast.Radon(imageDim=self.patDim,
+                                        nTheta=self.nTheta, nRho=self.nRho,
+                                        rhoMax=self.rhoMax,
+                                        mask=patternmask, maskindex=patternmaskindex)
+
+      if patternmask is not None:
+        back = np.array(patternmask > 0).astype(np.float32)
+      else:
+        back = np.ones(self.patDim[-2:], dtype=np.float32)
+
+
+
+      rdnmask = self.radonPlan.radon_faster(back,fixArtifacts=False, normalization=False)
+      #plt.imshow(rdnmask >= self.rhomask1thresh)
+      self.rhomask1 = (rdnmask[:,:,0] >= self.rhomask1thresh).astype(np.ubyte)
+
+      rdnmask = rdnmask > 0
+      rdnmask = rdnmask.squeeze()
+
+      if self.rhoMaskFrac >= 1:
+        s = np.ones(( 3, 1))
+        rdnmask = scipyndim.binary_erosion(rdnmask, structure=s, iterations = int(self.rhoMaskFrac) )
+      else:
+        cmask = self._circmask(back)
+        rdncmask = rdnmask.copy()
+        if self.rhoMaskFrac > 0:
+          mskinx = int(self.nRho*self.rhoMaskFrac)
+          if mskinx == 0:
+            mskinx = 1
+          rdncmask[0:mskinx, :] = 0
+          rdncmask[-mskinx:, :] = 0
+
+          #thresh = 0.5 * (np.min(back.shape[-2:]) * (1.0 - self.rhoMaskFrac))
+          #cmask = (cmask < thresh).astype(np.float32)
+        elif self.rhoMaskFrac < 0:
+          mskinx = int(-1*self.nRho * self.rhoMaskFrac)
+          #rdncmask[0:mskinx, :] = 0
+          #rdncmask[-mskinx:, :] = 0
+
+          cmask = (cmask < self.rhoMax * (1.0 + self.rhoMaskFrac)).astype(np.float32)
+          rdncmask = (self.radonPlan.radon_faster(cmask, fixArtifacts=False) > 0).squeeze()
+          #plt.imshow(cmask); print(thresh)
+        else:
+          pass
+          #cmask[:,...] = (cmask > -1).astype(np.float32)
+
+
+        #rdncmask = (self.radonPlan.radon_faster(cmask, fixArtifacts=False) > 0).squeeze()
+
+        rdnmask *= (rdncmask > 0).astype(bool)
+
+
+
+      self.rdnmask = rdnmask > 0
+      #back = (back > 0).astype(np.float32) / (back + 1.0e-12)
+      #self.rdnNorm = back
 
 
     if tSigma is not None:
       self.tSigma = tSigma
       recalc_masks = True
     if rSigma is not None:
       self.rSigma = rSigma
@@ -159,18 +248,18 @@
       recalc_masks = True
 
     if recalc_masks == True:
       ksz = np.array([np.max([np.int64(4*self.rSigma), 5]), np.max([np.int64(4*self.tSigma), 5])])
       ksz = ksz + ((ksz % 2) == 0)
       kernel = np.zeros(ksz, dtype=np.float32)
       kernel[(ksz[0]/2).astype(int),(ksz[1]/2).astype(int) ] = 1
-      kernel = -1.0*gaussian_filter(kernel, [self.rSigma, self.tSigma], order=[2,0])
+      kernel = -1.0*scipyndim.gaussian_filter(kernel, [self.rSigma, self.tSigma], order=[2,0])
       self.kernel = kernel.reshape((1,ksz[0], ksz[1]))
       #self.peakPad = np.array(np.around([ 4*ksz[0], 20.0/self.dTheta]), dtype=np.int64)
-      self.peakPad = np.array(np.around([3 * ksz[0], 4 * ksz[1]]), dtype=np.int64)
+      self.peakPad = np.array(np.around([2 * ksz[0], 2 * ksz[1]]), dtype=np.int64)
       self.peakPad += 1 - np.mod(self.peakPad, 2)  # make sure we have it as odd.
 
     self.padding = np.array([np.max( [self.peakPad[0], self.padding[0]] ), np.max([self.peakPad[1], self.padding[1]])])
 
     if nBands is not None:
       self.nBands = nBands
 
@@ -212,29 +301,26 @@
 
       if method.upper() == 'RANDOMSTRIDE':
         stride = np.random.choice(npats, size = nsample, replace = False )
         stride = np.sort(stride)
       elif method.upper() == 'EVENSTRIDE':
         step = int(npats / nsample) # not great, but maybe good enough.
         stride = np.arange(0,npats, step, dypte = np.uint64)
-      pat1 = fileobj.read_data(convertToFloat=True,patStartCount=[stride[0], 1],returnArrayOnly=True)
+      pat1 = fileobj.read_data(convertToFloat=True,patStartCount=[stride[0], 1],returnArrayOnly=True)[0]
       for i in stride[1:]:
-        pat1 += fileobj.read_data(convertToFloat=True,patStartCount=[i, 1],returnArrayOnly=True)
+        pat1 += fileobj.read_data(convertToFloat=True,patStartCount=[i, 1],returnArrayOnly=True)[0]
       back = pat1 / float(len(stride))
       #pshape = pat1.shape
     # a bit of image processing.
     if back is not None:
-      #if sigma is None:
-       #sigma = 2.0 * float(pshape[-1]) / 80.0
-      #back[0,:,:] = gaussian_filter(back[0,:,:], sigma = sigma )
+      back = np.squeeze(back)
       back = self.backsub_fit(back)
-      #back -= np.mean(back)
     self.backgroundsub = back
 
-  def backsub_fit(self, back):
+  def backsub_fit(self, back, mask = None):
     # This function will fit a 2D gaussian on top of a plane to the averaged set of patterns (data) that is provided.
     # It will automatically use whatever mask is defined for valid data.
     # If the gaussian fit fails to converge, it will fall back to just using the mean set of patterns for the background
     # with a warning.
     def gaussian_surf(x, y, a, x0, y0, sigx, sigy, c, d, e):
     # equation for 2D gaussian on top of a plane.
       return a * np.exp(- ((x - x0) ** 2) / (2.0 * sigx ** 2) - ((y - y0) ** 2) / (2.0 * sigy ** 2)) + c + d * x + e * y
@@ -250,36 +336,38 @@
     nx = back.shape[-1]
     ny = back.shape[-2]
     #plt.imshow(back)
     x = np.arange(nx, dtype=float)
     x = (np.broadcast_to(x.reshape(1,nx), (ny, nx))).ravel()
     y = np.arange(ny, dtype=float)
     y = (np.broadcast_to(y, (nx, ny)).T).ravel()
-    # make a circular mask - even if not EDAX, this should work OK.
-    cx = (np.arange(nx) - nx*0.5)**2
-    cy = (np.arange(ny) - ny*0.5)**2
-    cmask = np.sqrt(np.broadcast_to(cx.reshape(1,nx), (ny, nx)) + np.broadcast_to(cy, (nx, ny)).T) < (ny*0.49)
-
+    if mask is None:
+      # make a circular mask - even if not EDAX, this should work OK.
+      cx = (np.arange(nx) - nx*0.5)**2
+      cy = (np.arange(ny) - ny*0.5)**2
+      cmask = np.sqrt(np.broadcast_to(cx.reshape(1,nx), (ny, nx)) + np.broadcast_to(cy, (nx, ny)).T) < (ny*0.49)
+    else:
+      cmask = mask
     # need to grab only the values that are in the mask.
     wh = np.nonzero(cmask.ravel())[0]
     xwh = x[wh]
     ywh = y[wh]
     xywh = np.vstack((xwh, ywh))
-    zwh = (back.ravel())[wh]
+    zwh = (scipyndim.median_filter(np.squeeze(back),3).ravel())[wh]
     whmx = np.unravel_index(back.argmax(), back.shape)
     minz = zwh.min()
     # initialize a guess for the parameters.
     # [gauss amplitude, max loc x, max loc y, sigx, sigy, const offset, slope x, slope y]
     p0 = [(zwh.max() - zwh.min())*0.1, whmx[1], whmx[0], nx/2.355, ny/2.355, minz, 0, 0]
     try:
-      popt, pcov = opt.curve_fit(fit_gauss, xywh, zwh, p0)
+      popt, pcov = scipyopt.curve_fit(fit_gauss, xywh, zwh, p0)
       backfit = (gaussian_surf(x, y, *popt)).reshape(ny, nx)
       #print(p0, popt)
     except RuntimeError:
-      print('Warning: no convergence on back subtract ... using mean of the patterns.')
+      print('Warning: no convergence on background gaussian fit ... using mean of the patterns.')
       print('This may not be ideal for scans with few grains across the width of the scan.')
       backfit = back
     backfit -= np.mean(backfit)
     #f, axarr = plt.subplots(1, 3)
     #f.set_size_inches(10, 4)
     #axarr[0].imshow(data[0,:,:].squeeze(), cmap='gray')
     #axarr[1].imshow(data[0,:,:].squeeze() - backfit, cmap='gray')
@@ -298,14 +386,15 @@
     else:
       patterns = patternsIn
 
     shape = patterns.shape
     nPats = shape[0]
 
     bandData = np.zeros((nPats,self.nBands),dtype=self.dataType)
+    bandData['band_match_index'] = -100
     if chunksize < 0:
       nchunks = 1
       chunksize = nPats
       chunk_start_end = [[0,nPats]]
     else:
       nchunks = (np.ceil(nPats / chunksize)).astype(np.compat.long)
       chunk_start_end = [[i * chunksize, (i + 1) * chunksize] for i in range(nchunks)]
@@ -340,51 +429,50 @@
     if verbose > 0:
       print('Radon Time:',rdntime)
       print('Convolution Time:', convtime)
       print('Peak ID Time:', lmaxtime)
       print('Band Label Time:', blabeltime)
       print('Total Band Find Time:',tottime)
     if verbose > 1:
-      plt.clf()
-
-      if len(rdnConv.shape) == 3:
-        im2show = rdnConv[self.padding[0]:-self.padding[0],self.padding[1]:-self.padding[1], -1]
-      else:
-        im2show = rdnConv[self.padding[0]:-self.padding[0],self.padding[1]:-self.padding[1]]
-
-      rhoMaskTrim = np.int32(im2show.shape[0] * self.rhoMaskFrac)
-      mean = np.mean(im2show[rhoMaskTrim:-rhoMaskTrim, 1:-2])
-      stdv = np.std(im2show[rhoMaskTrim:-rhoMaskTrim, 1:-2])
-
-      im2show -= mean
-      im2show /= stdv
-      im2show = im2show.clip(-4, None)
-      im2show += 6
-      im2show[0:rhoMaskTrim,:] = 0
-      im2show[-rhoMaskTrim:,:] = 0
-      im2show = np.fliplr(im2show)
-
-      plt.figure()
-      plt.imshow(im2show, cmap='gray', extent=[self.radonPlan.theta.min(), self.radonPlan.theta.max(),
-                                               self.radonPlan.rho.min(), self.radonPlan.rho.max()],
-                 interpolation='none', zorder=1, aspect='auto')
-      width = bandData['width'][-1, :]
-      width /= width.min()
-      width *= 2
-      xplt = np.squeeze(
-        180.0 - np.interp(bandData['aveloc'][-1, :, 1], np.arange(self.radonPlan.nTheta), self.radonPlan.theta))
-      yplt = np.squeeze(
-        -1.0 * np.interp(bandData['aveloc'][-1, :, 0], np.arange(self.radonPlan.nRho), self.radonPlan.rho))
-
-      plt.scatter(y=yplt, x=xplt, c='r', s=width, zorder=2)
-
-      for pt in range(self.nBands):
-        plt.annotate(str(pt + 1), np.squeeze([xplt[pt], yplt[pt]]), color='yellow')
-      plt.xlim(0,180)
-      plt.ylim(-self.rhoMax, self.rhoMax)
+      self._display_radon_pattern(rdnConv, bandData, patterns)
+      # if len(rdnConv.shape) == 3:
+      #   im2show = rdnConv[self.padding[0]:-self.padding[0],self.padding[1]:-self.padding[1], -1]
+      # else:
+      #   im2show = rdnConv[self.padding[0]:-self.padding[0],self.padding[1]:-self.padding[1]]
+      #
+      # rhoMaskTrim = np.int32(im2show.shape[0] * self.rhoMaskFrac)
+      # mean = np.mean(im2show[rhoMaskTrim:-rhoMaskTrim, 1:-2])
+      # stdv = np.std(im2show[rhoMaskTrim:-rhoMaskTrim, 1:-2])
+      #
+      # im2show -= mean
+      # im2show /= stdv
+      # im2show = im2show.clip(-4, None)
+      # im2show += 6
+      # im2show[0:rhoMaskTrim,:] = 0
+      # im2show[-rhoMaskTrim:,:] = 0
+      # im2show = np.fliplr(im2show)
+      #
+      # plt.figure()
+      # plt.imshow(im2show, cmap='gray', extent=[self.radonPlan.theta.min(), self.radonPlan.theta.max(),
+      #                                          self.radonPlan.rho.min(), self.radonPlan.rho.max()],
+      #            interpolation='none', zorder=1, aspect='auto')
+      # width = bandData['width'][-1, :]
+      # width /= width.min()
+      # width *= 2
+      # xplt = np.squeeze(
+      #   180.0 - np.interp(bandData['aveloc'][-1, :, 1]+0.5, np.arange(self.radonPlan.nTheta), self.radonPlan.theta))
+      # yplt = np.squeeze(
+      #   -1.0 * np.interp(bandData['aveloc'][-1, :, 0]-0.5, np.arange(self.radonPlan.nRho), self.radonPlan.rho))
+      #
+      # plt.scatter(y=yplt, x=xplt, c='r', s=width, zorder=2)
+      #
+      # for pt in range(self.nBands):
+      #   plt.annotate(str(pt + 1), np.squeeze([xplt[pt]+4, yplt[pt]]), color='yellow')
+      # plt.xlim(0,180)
+      # plt.ylim(-self.rhoMax, self.rhoMax)
 
 
     return bandData
 
   def radonPad(self,radon,rPad=0,tPad = 0, mirrorTheta = True):
     # function for padding the radon transform
     # theta padding (tPad) will use the symmetry of the radon and will vertical flip the transform and place it on
@@ -438,15 +526,15 @@
       radon[0:self.padding[0], :,:] = radon[self.padding[0],:,:].reshape(1,shp[1], shp[2])
       radon[-self.padding[0]:, :,:] = radon[-self.padding[0]-1, :,:].reshape(1, shp[1],shp[2])
 
 
     rdnConv = np.zeros_like(radon)
 
     for i in range(shp[2]):
-      rdnConv[:,:,i] = -1.0 * gaussian_filter(np.squeeze(radon[:,:,i]),[self.rSigma,self.tSigma],order=[2,0])
+      rdnConv[:,:,i] = -1.0 * scipyndim.gaussian_filter(np.squeeze(radon[:,:,i]),[self.rSigma,self.tSigma],order=[2,0])
 
     #print(rdnConv.min(),rdnConv.max())
     mns = (rdnConv[self.padding[0]:shprdn[1]-self.padding[0],self.padding[1]:shprdn[1]-self.padding[1],:]).min(axis=0).min(axis=0)
 
     rdnConv -= mns.reshape((1,1, shp[2]))
     rdnConv = rdnConv.clip(min=0.0)
 
@@ -454,26 +542,29 @@
 
   def rdn_local_max(self, rdn, clparams=None, rdn_gpu=None, use_gpu=False):
 
     shp = rdn.shape
     # find the local max
     lMaxK = (self.peakPad[0],self.peakPad[1],1)
 
-    lMaxRdn = scipy_grey_dilation(rdn,size=lMaxK)
+    lMaxRdn = scipyndim.grey_dilation(rdn,size=lMaxK)
     #lMaxRdn[:,:,0:self.peakPad[1]] = 0
     #lMaxRdn[:,:,-self.peakPad[1]:] = 0
     #location of the max is where the local max is equal to the original.
     lMaxRdn = lMaxRdn == rdn
 
-    rhoMaskTrim = np.int32((shp[0] - 2 * self.padding[0]) * self.rhoMaskFrac + self.padding[0])
-    lMaxRdn[0:rhoMaskTrim,:,:] = 0
-    lMaxRdn[-rhoMaskTrim:,:,:] = 0
-    lMaxRdn[:,0:self.padding[1],:] = 0
-    lMaxRdn[:,-self.padding[1]:,:] = 0
+    #rhoMaskTrim = np.int32((shp[0] - 2 * self.padding[0]) * self.rhoMaskFrac + self.padding[0])
+    #lMaxRdn[0:rhoMaskTrim,:,:] = 0
+    #lMaxRdn[-rhoMaskTrim:,:,:] = 0
+    #lMaxRdn[:,0:self.padding[1],:] = 0
+    #lMaxRdn[:,-self.padding[1]:,:] = 0
     #print("Traditional:",timer() - tic)
+    maskrnd = np.zeros((self.nRho + 2 * self.padding[0], self.nTheta + 2 * self.padding[1],1), dtype=np.ubyte)
+    maskrnd[self.padding[0]:-self.padding[0], self.padding[1]:-self.padding[1],0] = self.rdnmask.astype(np.ubyte)
+    lMaxRdn *= maskrnd.astype(bool)
     return lMaxRdn
 
 
   def band_label(self,nPats,rdnConvIn,rdnNormIn,lMaxRdnIn):
     bandData = np.zeros((nPats,self.nBands),dtype=self.dataType)
 
 
@@ -558,18 +649,96 @@
         dxx = nn[1,2] + nn[1,0] - 2 * nn[1,1]
         dyy = nn[2,1] + nn[0,1] - 2 * nn[1,1]
         dxy = 0.25*(nn[2,2] - nn [0,2] - nn[2,0] + nn[0,0])
         #det = 1.0 / (dxx * dyy - dxy * dxy)
         det = (dxx * dyy - dxy * dxy)
         det = det if np.fabs(det) > 1e-12 else 1.0e-12
         det = 1.0/det
-        cnn = c - (dyy * dx - dxy * dy) * det
-        rnn = r - (dxx * dy - dxy * dx) * det
+        dc =  (dyy * dx - dxy * dy) * det
+        rc = (dxx * dy - dxy * dx) * det
+        dc = max(-1.0, dc) ; rc = max(-1.0, rc)
+        dc = min(1.0, dc) ;  rc = min(1.0, rc)
+        cnn = c - dc
+        rnn = r - rc
         bandData_aveloc[q,i,:] = np.array([rnn,cnn])
         bandData_valid[q,i] = 1
 
     return bandData_max,bandData_avemax,bandData_maxloc,bandData_aveloc, bandData_valid, bandData_width
+  def _display_radon_pattern(self, rdnConvarray, bandData, patterns):
+    if len(rdnConvarray.shape) == 3:
+      im2show = rdnConvarray[self.padding[0]:-self.padding[0], self.padding[1]:-self.padding[1], -1]
+    else:
+      im2show = rdnConvarray[self.padding[0]:-self.padding[0], self.padding[1]:-self.padding[1]]
+
+    im2show *= self.rdnmask
+    #rhoMaskTrim = np.int32(im2show.shape[0] * self.rhoMaskFrac)
+    #mean = np.mean(im2show[rhoMaskTrim:-rhoMaskTrim, 1:-2])
+    #stdv = np.std(im2show[rhoMaskTrim:-rhoMaskTrim, 1:-2])
+    mean = np.mean(im2show, where=(self.rdnmask >0))
+    stdv = np.std(im2show, where=(self.rdnmask >0))
+
+
+    im2show -= mean
+    im2show /= stdv
+    im2show = im2show.clip(-4, None)
+    im2show += 6
+    #im2show[0:rhoMaskTrim, :] = 0
+    #im2show[-rhoMaskTrim:, :] = 0
+
+    im2show = np.fliplr(im2show)
+    fig = plt.figure(figsize=(12, 4))
+    subrdn = fig.add_subplot(121, xlim=(0, 180), ylim=(-self.rhoMax, self.rhoMax))
+    subrdn.imshow(
+      im2show,
+      cmap='gray',
+      extent=[0, 180, -self.rhoMax, self.rhoMax],
+      interpolation='none',
+      zorder=1,
+      aspect='auto'
+    )
+    width = bandData['width'][-1, :]
+    width /= width.min()
+    width *= 2.0
+    xplt = np.squeeze(
+      180.0 - np.interp(bandData['aveloc'][-1, :, 1] + 0.5, np.arange(self.radonPlan.nTheta), self.radonPlan.theta))
+    yplt = np.squeeze(
+      -1.0 * np.interp(bandData['aveloc'][-1, :, 0] - 0.5, np.arange(self.radonPlan.nRho), self.radonPlan.rho))
+
+    subrdn.scatter(y=yplt, x=xplt, c='r', s=width, zorder=2)
+
+    for pt in range(self.nBands):
+      subrdn.annotate(str(pt + 1), np.squeeze([xplt[pt] + 4, yplt[pt]]), color='yellow')
+    # subrdn.xlim(0,180)
+    # subrdn.ylim(-self.rhoMax, self.rhoMax)
+    subpat = fig.add_subplot(122)
+    pat1 = patterns[-1, :, :].copy().squeeze().astype(float)
+    minpat = pat1.min()
+    pdim = pat1.shape
+    pat1 = np.concatenate((pat1.flatten(), [minpat]))
+    patmask = np.copy(self.radonPlan.mask).astype(int)
+
+    #patdisplay = np.zeros(patmask.size)
+    patdisplay = pat1[[self.radonPlan.maskindex.flatten().clip(-1,).astype(int)]]
+    patdisplay = patdisplay.reshape(self.radonPlan.maskindex.shape)
+
+    patdisplay *= (patmask != 0).astype(int)
+    patdisplay += minpat*(patmask ==0).astype(float)
+
+    subpat.imshow(patdisplay, cmap='gray')
+  def _circmask(self, im):
+    nx = im.shape[-1]
+    ny = im.shape[-2]
+    # plt.imshow(back)
+    x = np.arange(nx, dtype=float)
+    x = (np.broadcast_to(x.reshape(1, nx), (ny, nx))).ravel()
+    y = np.arange(ny, dtype=float)
+    y = (np.broadcast_to(y, (nx, ny)).T).ravel()
 
+      # make a circular mask - even if not EDAX, this should work OK.
+    cx = (np.arange(nx) - nx * 0.5) ** 2
+    cy = (np.arange(ny) - ny * 0.5) ** 2
+    cmask = np.sqrt(np.broadcast_to(cx.reshape(1, nx), (ny, nx)) + np.broadcast_to(cy, (nx, ny)).T) #< (ny * 0.49)
+    return cmask
 def getopenclparam(**kwargs): # dummy function to maintain compatability with openCL version
   return None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/crystallometry.py` & `pyebsdindex-0.3.0/pyebsdindex/crystallometry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-'''This software was developed by employees of the US Naval Research Laboratory (NRL), an
-agency of the Federal Government. Pursuant to title 17 section 105 of the United States
-Code, works of NRL employees are not subject to copyright protection, and this software
-is in the public domain. PyEBSDIndex is an experimental system. NRL assumes no
-responsibility whatsoever for its use by other parties, and makes no guarantees,
-expressed or implied, about its quality, reliability, or any other characteristic. We
-would appreciate acknowledgment if the software is used. To the extent that NRL may hold
-copyright in countries other than the United States, you are hereby granted the
-non-exclusive irrevocable and unconditional right to print, publish, prepare derivative
-works and distribute this software, in any medium, or authorize others to do so on your
-behalf, on a royalty-free basis throughout the world. You may improve, modify, and
-create derivative works of the software or any portion of the software, and you may copy
-and distribute such modifications or works. Modified works should carry a notice stating
-that you changed the software and should note the date and nature of any such change.
-Please explicitly acknowledge the US Naval Research Laboratory as the original source.
-This software can be redistributed and/or modified freely provided that any derivative
-works bear some notice that they are derived from it, and any modified versions bear
-some notice that they have been modified.
-
-This borrows heavily from Marc De Graef's EMsoft package. Many functions here
-are Python translations of functions from it.
-
-
-Author: David Rowenhorst, Patrick Callahan;
-The US Naval Research Laboratory Date: 21 Aug 2020'''
+# This software was developed by employees of the US Naval Research Laboratory (NRL), an
+# agency of the Federal Government. Pursuant to title 17 section 105 of the United States
+# Code, works of NRL employees are not subject to copyright protection, and this software
+# is in the public domain. PyEBSDIndex is an experimental system. NRL assumes no
+# responsibility whatsoever for its use by other parties, and makes no guarantees,
+# expressed or implied, about its quality, reliability, or any other characteristic. We
+# would appreciate acknowledgment if the software is used. To the extent that NRL may hold
+# copyright in countries other than the United States, you are hereby granted the
+# non-exclusive irrevocable and unconditional right to print, publish, prepare derivative
+# works and distribute this software, in any medium, or authorize others to do so on your
+# behalf, on a royalty-free basis throughout the world. You may improve, modify, and
+# create derivative works of the software or any portion of the software, and you may copy
+# and distribute such modifications or works. Modified works should carry a notice stating
+# that you changed the software and should note the date and nature of any such change.
+# Please explicitly acknowledge the US Naval Research Laboratory as the original source.
+# This software can be redistributed and/or modified freely provided that any derivative
+# works bear some notice that they are derived from it, and any modified versions bear
+# some notice that they have been modified.
+#
+# This borrows heavily from Marc De Graef's EMsoft package. Many functions here
+# are Python translations of functions from it.
+#
+#
+# Author: David Rowenhorst, Patrick Callahan;
+# The US Naval Research Laboratory Date: 22 May 2024
 
 
 import numpy as np
 import math as math
 from functools import reduce
 
 ## This borrows heavily from Marc De Graef's EMsoft package. Many functions here
 ## are Python translations of functions from it.
 
 
 
 class CrystalPlane:
-    def __init__(self,hkl = [0,0,0],centering = 'F'):
+    def __init__(self,hkl = (0,0,0),centering = 'F'):
         self.hkl = np.array(hkl)
         self.allowed = True
         self.lattice_centering = centering
         self.d = 0.0
         self.g = 0.0
 
     def is_g_allowed(self):
@@ -78,14 +78,16 @@
         ca = np.cos(alpha*np.pi/180)
         cb = np.cos( beta*np.pi/180)
         cg = np.cos(gamma*np.pi/180)
         sa = np.sin(alpha*np.pi/180)
         sb = np.sin( beta*np.pi/180)
         sg = np.sin(gamma*np.pi/180)
         tg = np.tan(gamma*np.pi/180)
+        fabg = ca*cb-cg
+
 
         #compute the real space metric tensor
         self.metricTensor = np.zeros([3,3])
         self.metricTensor[0,0] = a**2.0
         self.metricTensor[1,1] = b**2.0
         self.metricTensor[2,2] = c**2.0
         self.metricTensor[1,0] = a*b*cg
@@ -123,14 +125,28 @@
         self.directStructureMatrix[1,1] = b*sg
         self.directStructureMatrix[2,1] = -c*(cb*cg-ca)/sg
         self.directStructureMatrix[0,2] = 0.0
         self.directStructureMatrix[1,2] = 0.0
         self.directStructureMatrix[2,2] = self.volume/(a*b*sg)
         self.directStructureMatrix = self.directStructureMatrix.transpose()
         self.directStructureMatrix[np.abs(self.directStructureMatrix) < smallThreshold] = 0
+
+        # Compute inverse direct stucture matrix
+        self.invDirectStructureMatrix = np.zeros([3, 3])
+        self.invDirectStructureMatrix[0, 0] = 1.0/a
+        self.invDirectStructureMatrix[1, 0] = -1.0/(a * tg)
+        self.invDirectStructureMatrix[2, 0] = b*c * (cg*ca-cb)/(self.volume * sg)
+        self.invDirectStructureMatrix[0, 1] = 0.0
+        self.invDirectStructureMatrix[1, 1] = 1.0/(b * sg)
+        self.invDirectStructureMatrix[2, 1] = a*c*(cb*cg-ca)/(self.volume*sg)
+        self.invDirectStructureMatrix[0, 2] = 0.0
+        self.invDirectStructureMatrix[1, 2] = 0.0
+        self.invDirectStructureMatrix[2, 2] = a*b*sg/(self.volume)
+        self.invDirectStructureMatrix = self.invDirectStructureMatrix.transpose()
+        self.invDirectStructureMatrix[np.abs(self.invDirectStructureMatrix) < smallThreshold] = 0
         
         #compute reciprocal structure matrix
         self.reciprocalStructureMatrix = np.zeros([3,3])
         self.reciprocalStructureMatrix[0,0] = 1.0/a
         self.reciprocalStructureMatrix[1,0] = 0.0
         self.reciprocalStructureMatrix[2,0] = 0.0
         self.reciprocalStructureMatrix[0,1] = -1.0/(a*tg)
@@ -138,14 +154,18 @@
         self.reciprocalStructureMatrix[2,1] = 0.0
         self.reciprocalStructureMatrix[0,2] = b*c*(cg*ca-cb)/(self.volume*sg)
         self.reciprocalStructureMatrix[1,2] = a*c*(cb*cg-ca)/(self.volume*sg)
         self.reciprocalStructureMatrix[2,2] = (a*b*sg)/self.volume
         self.reciprocalStructureMatrix = self.reciprocalStructureMatrix.transpose()
         self.reciprocalStructureMatrix[np.abs(self.reciprocalStructureMatrix) < smallThreshold] = 0
 
+        # Compute inverse reciprocal stucture matrix
+        self.invReciprocalStructureMatrix = np.zeros([3, 3])
+        self.invReciprocalStructureMatrix = np.transpose(self.directStructureMatrix)
+
     # def get_lattice_centering(self):
     #     self.latticeCentering = self.spaceGroup[0]
 
     # def is_g_allowed(self,g):
     #     get_lattice_centering()
     #     allowed = True
     #     if lattice_centering == 'F':
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/ebsd_index.py` & `pyebsdindex-0.3.0/pyebsdindex/ebsd_index.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,21 @@
 # This software can be redistributed and/or modified freely provided that any derivative
 # works bear some notice that they are derived from it, and any modified versions bear
 # some notice that they have been modified.
 #
 # Author: David Rowenhorst;
 # The US Naval Research Laboratory Date: 21 Aug 2020
 
-"""Setup and handling of Hough indexing runs of EBSD patterns."""
+"""Setup and handling of Radon indexing runs of EBSD patterns."""
 
 from pyebsdindex import _ray_installed
 from pyebsdindex._ebsd_index_single import EBSDIndexer, index_pats
 
 if _ray_installed:
-    from pyebsdindex._ebsd_index_parallel import index_pats_distributed, IndexerRay
+    from pyebsdindex._ebsd_index_parallel import index_pats_distributed
 
 
 __all__ = [
     "EBSDIndexer",
-    "IndexerRay",
     "index_pats",
     "index_pats_distributed",
 ]
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/ebsd_pattern.py` & `pyebsdindex-0.3.0/pyebsdindex/ebsd_pattern.py`

 * *Files 22% similar despite different names*

```diff
@@ -43,45 +43,62 @@
   ftype = file_type
   if ftype == str(''):
     extension = str.lower(Path(filepath).suffix)
     if (extension == '.up1'):
       ftype = 'UP1'
     elif (extension == '.up2'):
       ftype = 'UP2'
+    elif (extension == '.ebsp'):
+      ftype = 'EBSP'
     elif (extension == '.oh5'):
       ftype = 'OH5'
     elif (extension == '.h5'):
       ftype = 'H5'
+    elif (extension == '.h5oina'):
+      ftype = 'H5OINA'
     else:
       raise ValueError('Error: extension not recognized')
 
   if (ftype.upper() == 'UP1') or (ftype.upper() == 'UP2'):
     ebsdfileobj = UPFile(path)
+  if (ftype.upper() == 'EBSP'):
+    ebsdfileobj = EBSPFile(path)
   if (ftype.upper() == 'OH5'):
     ebsdfileobj = EDAXOH5(path)
     if hdf5path is None: #automatically chose the first data group
       ebsdfileobj.get_data_paths()
       ebsdfileobj.set_data_path(pathindex=0)
+  if (ftype.upper() == 'H5OINA'):
+    ebsdfileobj = OXFORDOINA(path)
+    if hdf5path is None: #automatically chose the first data group
+      ebsdfileobj.get_data_paths()
+      ebsdfileobj.set_data_path(pathindex=0)
   if (ftype.upper() == 'H5'):
     ebsdfileobj = HDF5PatFile(path) # if the path variable is a list,
     # the second item is set to be the hdf5 path to the patterns.
     try:
       f = h5py.File(Path(pathtemp[0]).expanduser(),'r+')
     except:
       print("File Not Found:",str(Path(pathtemp[0])))
       return -1
 
-    if 'Manufacture' in f.keys():
-      vendor = str(f['Manufacture'][()][0])
+    if 'Manufacturer' in f.keys():
+      vendor = f['Manufacturer'][()]
+      if type(vendor) is np.ndarray:
+        vendor = vendor[0]
+      vendor = str(vendor.decode(encoding='UTF-8'))
       if vendor.upper() == 'EDAX':
         ebsdfileobj = EDAXOH5(path)
-      if vendor.upper() >= 'BRUKER NANO':
+      if vendor.upper() == 'BRUKER NANO':
         ebsdfileobj = BRUKERH5(path)
     if 'manufacturer' in f.keys():
-      vendor = str((f['manufacturer'][()][0]).decode('UTF-8'))
+      vendor = f['manufacturer'][()]
+      if type(vendor) is np.ndarray:
+        vendor = vendor[0]
+      vendor = str(vendor.decode('UTF-8'))
       if vendor >= 'kikuchipy':
         ebsdfileobj = KIKUCHIPYH5(path)
     if ebsdfileobj.h5patdatpth is None: #automatically chose the first data group
       ebsdfileobj.get_data_paths()
       ebsdfileobj.set_data_path(pathindex=0)
   ebsdfileobj.read_header()
   return ebsdfileobj
@@ -156,20 +173,22 @@
     self.filepath = None
     self.filetype = None
     self.patternW = None
     self.patternH = None
     self.nFileCols = None
     self.nFileRows = None
     self.nPatterns = None
-    self.hexFlag = None
+    self.hexflag = None
     self.xStep = None
     self.yStep = None
     self.patStart = [0,0] #starting point of the pattern location in the file. len==1
     # if 2D, then it is the row/column starting points
     self.patterns = None
+    self.xyLocations = None
+    # The x,y locations of the pattern collection relative to the center of the SEM field-of-view.
 
 
 
 
 # a class template for any EBSD pattern file type.
 # Any EBSD file class should inheret this class.
 class EBSDPatternFile():
@@ -178,16 +197,18 @@
     self.vendor = None
     self.version = None
     self.nCols = None
     self.nRows = None
     self.nPatterns = None
     self.patternW = None
     self.patternH = None
-    self.xStep = None
+    self.xStep = None  # assumming square grid data, with constant step size
     self.yStep = None
+    self.xyCenter = np.array([0.0, 0.0])
+    # This is the location of the center of the scan relative to center of SEM field-of-view
     self.hexflag = False
     self.filetype = filetype
     self.filedatatype = np.uint8  # the data type of the patterns within the file
 
   def set_filepath(self, path=None):
     if path is not None:
       ptemp = np.atleast_1d(path)
@@ -198,15 +219,15 @@
 
   def read_data(self,path=None,convertToFloat=False,patStartCount = [0,-1],returnArrayOnly=False):
     if path is not None:
       self.set_filepath(path)
       self.read_header()
     if self.version is None:
       self.read_header()
-
+    patStartCount = np.array(patStartCount, dtype=np.int64)
     # bitD = 8 * (self.bitdepth == 8) + 16 * (self.bitdepth == 16)
 
     # # this will allow for overriding the original file spec -- not sure why would want to but ...
     # if (bitdepth == 8):
     #   bitD = 8
     # if (bitdepth == 16):
     #   bitD = 16
@@ -220,80 +241,84 @@
     if convertToFloat == True:
       typeout = np.float32
     else:
       typeout = self.filedatatype
 
     pStartEnd = np.asarray(patStartCount, dtype=np.int64)
     if pStartEnd.ndim == 1: # read a continuous set of patterns.
-      patStart = patStartCount[0]
-      nPatToRead = patStartCount[-1]
+      patStart = int(patStartCount[0])
+      nPatToRead = int(patStartCount[-1])
       if nPatToRead == -1:
-        nPatToRead = self.nPatterns - patStart
+        nPatToRead = int(self.nPatterns - patStart)
       if nPatToRead == 0:
         nPatToRead = 1
       if (patStart + nPatToRead) > self.nPatterns:
-        nPatToRead = self.nPatterns - patStart
+        nPatToRead = int(self.nPatterns - patStart)
 
 
       # this function does the actual reading from the file.
-      readpats = self.pat_reader(patStart, nPatToRead)
+      readpats, xyloc = self.pat_reader(patStart, nPatToRead)
       patterns = readpats.astype(typeout)
 
 
 
     elif pStartEnd.ndim == 2: # read a slab of patterns.
-        colstart = pStartEnd[0,0]
-        ncolread = pStartEnd[1,0]
-        rowstart = pStartEnd[0,1]
-        nrowread = pStartEnd[1,1]
+        colstart = int(pStartEnd[0,0])
+        ncolread = int(pStartEnd[1,0])
+        rowstart = int(pStartEnd[0,1])
+        nrowread = int(pStartEnd[1,1])
 
         patStart = [colstart, rowstart]
         if ncolread < 0:
-          ncolread = self.nCols - colstart
+          ncolread = int(self.nCols - colstart)
         if nrowread < 0:
-          nrowread = self.nRows - rowstart
+          nrowread = int(self.nRows - rowstart)
 
         if (colstart+ncolread) > self.nCols:
-          ncolread = self.nCols - colstart
+          ncolread = int(self.nCols - colstart)
 
         if (rowstart+nrowread) > self.nRows:
-          nrowread = self.nRows - rowstart
+          nrowread = int(self.nRows - rowstart)
         nrowread = np.uint64(nrowread)
         ncolread = np.uint64(ncolread)
         nPatToRead = [ncolread, nrowread]
 
         patterns = np.zeros([int(ncolread*nrowread),self.patternH,self.patternW],dtype=typeout)
+        xyloc = np.zeros([int(ncolread*nrowread),2],dtype=np.float32)
 
         for i in range(nrowread):
-          pstart = int(((rowstart+i)*self.nCols)+colstart)
-          ptemp = self.read_data(convertToFloat=convertToFloat,patStartCount = [pstart,ncolread],returnArrayOnly=True)
+          pstart = int(int(int(rowstart+i)*self.nCols)+colstart)
+          ptemp, xyloctemp = self.read_data(convertToFloat=convertToFloat,patStartCount = [pstart,ncolread],returnArrayOnly=True)
 
           patterns[int(i*ncolread):int((i+1)*ncolread), :, :] = ptemp
+          xyloc[int(i*ncolread):int((i+1)*ncolread), :] = xyloctemp
 
     if returnArrayOnly == True:
-      return patterns
+      return patterns, xyloc
     else:  # package this up in an EBSDPatterns Object
       patsout = EBSDPatterns()
       patsout.vendor = self.vendor
       patsout.file = Path(self.filepath).expanduser()
       patsout.filetype = self.filetype
       patsout.patternW = self.patternW
       patsout.patternH = self.patternH
-      patsout.nFileCols = self.nCols
-      patsout.nFileRows = self.nRows
+      patsout.nFileCols = np.uint64(self.nCols)
+      patsout.nFileRows = np.uint64(self.nRows)
       patsout.nPatterns = np.array(nPatToRead)
-      patsout.hexFlag = self.hexFlag
+      patsout.hexflag = self.hexflag
       patsout.xStep = self.xStep
       patsout.yStep = self.yStep
       patsout.patStart = np.array(patStart)
       patsout.patterns = patterns
+      patsout.xyLocations = xyloc
       return patsout # note this function uses multiple return statements
 
-  def pat_reader(self, patStart, nPatToRead):
-    '''Depending on the file type, it will return a numpy array of patterns.'''
+  def pat_reader(self, patStart=0, nPatToRead=1):
+    '''Depending on the file type, it will return a numpy array of patterns, and the positions of the patterns
+    in the scan.'''
     pass
 
   def write_header(self):
     pass
 
   def write_data(self, newpatterns=None, patStartCount = [0,-1], writeHead=False,
                  flt2int='clip', scalevalue = 0.98, maxScale = None):
@@ -323,49 +348,49 @@
       max = maxScale
 
     pStartEnd = np.asarray(patStartCount)
     # npats == number of patterns in the newpatterns
     # self.nPatterns == number of patterns in the file
     # nPats to write == number of patterns to write out
     if pStartEnd.ndim == 1:  # write a continuous set of patterns.
-      patStart = patStartCount[0]
-      nPatToWrite = patStartCount[-1]
+      patStart = int(patStartCount[0])
+      nPatToWrite = int(patStartCount[-1])
       if nPatToWrite == -1:
         nPatToWrite = npats
       if nPatToWrite == 0:
         nPatToWrite = 1
       if (patStart + nPatToWrite) > self.nPatterns:
         nPatToWrite = self.nPatterns - patStart
 
       typewrite = self.filedatatype
       pat2write = pat_flt2int(pats,typeout=typewrite,method=flt2int,scalevalue=scalevalue,maxScale=None)
       self.pat_writer(pat2write,patStart,nPatToWrite, typewrite)
 
     elif pStartEnd.ndim == 2: # write a slab of patterns.
-        colstart = pStartEnd[0,0]
-        ncolwrite = pStartEnd[1,0]
-        rowstart = pStartEnd[0,1]
-        nrowwrite = pStartEnd[1,1]
+        colstart = int(pStartEnd[0,0])
+        ncolwrite = int(pStartEnd[1,0])
+        rowstart = int(pStartEnd[0,1])
+        nrowwrite = int(pStartEnd[1,1])
 
         patStart = [colstart, rowstart]
         if ncolwrite < 0:
-          ncolwrite = self.nCols - colstart
+          ncolwrite = int(self.nCols - colstart)
         if nrowwrite < 0:
-          nrowwrite = self.nRows - rowstart
+          nrowwrite = int(self.nRows - rowstart)
 
         if (colstart+ncolwrite) > self.nCols:
-          ncolwrite = self.nCols - colstart
+          ncolwrite = int(self.nCols - colstart)
 
         if (rowstart+nrowwrite) > self.nRows:
-          nrowwrite = self.nRows - rowstart
+          nrowwrite = int(self.nRows - rowstart)
 
 
         for i in range(nrowwrite):
-          pstart = ((rowstart+i)*self.nCols)+colstart
-          self.write_data(newpatterns = pats[i*ncolwrite:(i+1)*ncolwrite, :, :], patStartCount=[pstart,ncolwrite],writeHead=False,
+          pstart = int(int(int(rowstart+i)*self.nCols)+colstart)
+          self.write_data(newpatterns = pats[int(i*ncolwrite):int((i+1)*ncolwrite), :, :], patStartCount=[pstart,ncolwrite],writeHead=False,
                           flt2int=flt2int,scalevalue=0.98, maxScale = max)
   def pat_writer(self, pat2write, patStart, nPatToWrite, typewrite):
     pass
 
 
   def copy_file(self, newpath, **kwargs):
     src = Path(self.filepath).expanduser().resolve()
@@ -376,31 +401,31 @@
       dst = Path(str(src.expanduser().resolve())+'.copy')
     shutil.copyfile(src,dst)
 
   def copy_obj(self):
     return copy.deepcopy(self)
 
   def set_scan_rc(self, rc=(0,0)): # helper function for pattern files that don't record the scan rows and columns
-    self.nCols = rc[1]
-    self.nRows = rc[0]
-    self.nPatterns = self.nCols * self.nRows
+    self.nCols = np.uint64(rc[1])
+    self.nRows = np.uint64(rc[0])
+    self.nPatterns = np.uint64(self.nCols * self.nRows)
 
 
 class UPFile(EBSDPatternFile):
 
   def __init__(self, path=None):
     EBSDPatternFile.__init__(self, path)
     self.filetype = 'UP'
     self.vendor = 'EDAX'
     self.filedatatype = None
     #UP only attributes
     #self.bitdepth = None
     self.filePos = None  # file location in bytes where pattern data starts
     self.extraPatterns = 0
-    self.hexFlag = 0
+    self.hexflag = 0
 
 
   def read_header(self,path=None,bitdepth=None):  # readInterval=[0, -1], arrayOnly=False,
     if path is not None:
       self.filepath = path
 
     extension = str.lower(Path(self.filepath).suffix)
@@ -431,35 +456,45 @@
 
     self.version = np.fromfile(f, dtype=np.uint32, count=1)[0]
     if self.version == 1:
       dat = np.fromfile(f, dtype=np.uint32, count=3)
       self.patternW = dat[0]
       self.patternH = dat[1]
       self.filePos = dat[2]
-      self.nPatterns = np.int((Path(self.filepath).expanduser().stat().st_size - 16) /
+      self.nPatterns = int((Path(self.filepath).expanduser().stat().st_size - 16) /
                               (self.patternW * self.patternH * (self.filedatatype(0).nbytes)))
+      if self.xStep is None:
+        self.xStep = 0.0
+      if self.yStep is None:
+        self.yStep = 0.0
+      if self.nCols is None:
+        self.nCols = np.uint64(1)
+      if self.nCols == 0:
+        self.nCols = np.uint64(1)
+      if self.nRows is None:
+        self.nRows = np.uint64(np.floor(self.nPatterns/self.nCols))
 
     elif self.version >= 3:
       dat = np.fromfile(f, dtype=np.uint32, count=3)
       self.patternW = dat[0]
       self.patternH = dat[1]
       self.filePos = dat[2]
       self.extraPatterns = np.fromfile(f, dtype=np.uint8, count=1)[0]
       dat = np.fromfile(f, dtype=np.uint32, count=2)
-      self.nCols = dat[0]
-      self.nRows = dat[1]
-      self.nPatterns = np.int(self.nCols.astype(np.uint64) * self.nRows.astype(np.uint64))
-      self.hexFlag = np.fromfile(f, dtype=np.uint8, count=1)[0]
+      self.nCols = np.uint64(dat[0])
+      self.nRows = np.uint64(dat[1])
+      self.nPatterns = int(self.nCols.astype(np.uint64) * self.nRows.astype(np.uint64))
+      self.hexflag = np.fromfile(f, dtype=np.uint8, count=1)[0]
       dat = np.fromfile(f, dtype=np.float64, count=2)
       self.xStep = dat[0]
       self.yStep = dat[1]
     f.close()
     return 0 #note this function uses multiple returns
 
-  def pat_reader(self, patStart, nPatToRead):
+  def pat_reader(self, patStart=0, nPatToRead=1):
     try:
       f = open(Path(self.filepath).expanduser(),'rb')
     except:
       print("File Not Found:",str(Path(self.filepath)))
       return -1
 
     f.seek(self.filePos)
@@ -467,15 +502,23 @@
     typeread = self.filedatatype
     typebyte = self.filedatatype(0).nbytes
 
     f.seek(int(nPerPat * patStart * typebyte),1)
     readpats = np.fromfile(f,dtype=typeread,count=int(nPatToRead * nPerPat))
     readpats = readpats.reshape(nPatToRead,self.patternH,self.patternW)
     f.close()
-    return readpats
+    yx = np.unravel_index(np.arange(int(patStart), int(patStart+nPatToRead), dtype = np.uint64),
+                          (int(self.nRows), int(self.nCols)))
+
+    xyloc = np.array([yx[1],yx[0]]).T.copy().astype(np.float32)
+    xyloc[:,0] -= self.nCols * 0.5
+    xyloc[:, 1] -= self.nRows * 0.5
+    xyloc[:,0] *= self.xStep
+    xyloc[:,1] *= self.yStep
+    return readpats, xyloc
 
 
   def write_header(self, writeBlank=False, bitdepth=None):
 
     filepath = self.filepath
     extension = str.lower(Path(filepath).suffix)
     try:
@@ -504,28 +547,35 @@
       else:
         f = open(Path(filepath).expanduser(),'w+b')
         f.seek(0)
     except:
       print("File Not Found:", str(Path(filepath)))
       return -1
 
+    if self.version is None:
+      self.version = 3
+
     np.asarray(self.version, dtype=np.uint32).tofile(f)
     if self.version == 1:
+      if self.filePos is None:
+        self.filePos = 16
       np.asarray(self.patternW,dtype=np.uint32).tofile(f)
       np.asarray(self.patternH,dtype=np.uint32).tofile(f)
       np.asarray(self.filePos,dtype=np.uint32).tofile(f)
 
     elif self.version >= 3:
+      if self.filePos is None:
+        self.filePos = 42
       np.asarray(self.patternW,dtype=np.uint32).tofile(f)
       np.asarray(self.patternH,dtype=np.uint32).tofile(f)
       np.asarray(self.filePos,dtype=np.uint32).tofile(f)
       np.asarray(self.extraPatterns,dtype=np.uint8).tofile(f)
       np.asarray(self.nCols,dtype=np.uint32).tofile(f)
       np.asarray(self.nRows,dtype=np.uint32).tofile(f)
-      np.asarray(self.hexFlag,dtype=np.uint8).tofile(f)
+      np.asarray(self.hexflag,dtype=np.uint8).tofile(f)
       np.asarray(self.xStep,dtype=np.float64).tofile(f)
       np.asarray(self.yStep,dtype=np.float64).tofile(f)
 
     if writeBlank == True:
       typewrite = self.filedatatype
       # if self.bitdepth == 8:
       #   type = np.uint8
@@ -537,40 +587,44 @@
         for i in range(self.nCols):
           blank.tofile(f)
     f.close()
 
 
   def pat_writer(self, pat2write, patStart, nPatToWrite, typewrite):
     try:
-      f = open(Path(self.filepath).expanduser(),'br+')
-      f.seek(0,0)
-    except:
-      print("File Not Found:",str(Path(self.filepath)))
+      with open(Path(self.filepath).expanduser(),'br+') as f:
+        #print(patStart)
+        f.seek(0,0)
+        nPerPat = int(self.patternW * self.patternH)
+        nPerPatByte = int(nPerPat * typewrite(0).nbytes)
+        f.seek(int(nPerPatByte * (patStart) + self.filePos), 0)
+        pat2write[0:nPatToWrite, :, :].tofile(f)
+        #print(patStart)
+    except Exception as e:
+      print(e)
+      print(str(Path(self.filepath)))
       return -1
 
-    nPerPat = self.patternW * self.patternH
-    nPerPatByte = nPerPat * typewrite(0).nbytes
-    f.seek(int(nPerPatByte * (patStart) + self.filePos),0)
-    pat2write[0:nPatToWrite,:,:].tofile(f)
-    f.close()
+
+
 
 
 
   def file_from_pattern_obj(self, patternobj, filepath=None, bitdepth = None):
     if self.version is None:
       self.version = 3
     if self.xStep is None:
       self.xStep = 1.0
     if self.yStep is None:
       self.yStep = 1.0
 
 
     self.filePos = 42  # file location in bytes where pattern data starts
     self.extraPatterns = 0
-    self.hexFlag = 0
+    self.hexflag = 0
 
     if isinstance(patternobj, EBSDPatterns):
       shp = (patternobj.nPatterns.prod(),patternobj.patternH,patternobj.patternW)
       mx = patternobj.patterns.max()
     elif isinstance(patternobj, np.ndarray):
       shp = patternobj.shape
       mx = patternobj.max()
@@ -578,22 +632,427 @@
       if ndim == 2: #
         shp = (1,shp[0], shp[1])
       elif ndim == 3:
         shp = shp
     self.patternH = shp[1]
     self.patternW = shp[2]
 
-    self.nCols = shp[0]
-    self.nRows = 1
-    self.nPatterns = shp[0]
+    self.nCols = np.uint64(shp[0])
+    self.nRows = np.uint64(1)
+    self.nPatterns = np.uint64(shp[0])
 
     if bitdepth is None: #make a guess
       self.bitdepth = 16
       if mx <= 256:
         self.bitdepth = 8
+  def copy_file(self, newpath, **kwargs):
+    src = Path(self.filepath).expanduser().resolve()
+    if newpath is not None:
+      path = np.atleast_1d(newpath)
+      dst = Path(path[0]).expanduser().resolve()
+    else:
+      dst = Path(str(src.expanduser().resolve())+'.copy')
+    try:
+      if 'empty_data' in kwargs:
+        if kwargs['empty_data'] == True:
+          with open(src, 'rb') as srcf:
+            head = srcf.read(self.filePos)
+            size = srcf.seek(0, 2)
+            #print('checkpoint' ,size)
+          with open(dst, 'wb') as dstf:
+            head = dstf.write(head)
+            #print('write head')
+            dstf.seek(size-1,0)
+            #print('seek done')
+            dstf.write(b"\0")
+          return
+    except:
+      pass
+    shutil.copyfile(src,dst)
+
+class EBSPFile(EBSDPatternFile):
+  """
+    Notes
+    -----
+    Information about the .ebsp file format was generously provided by
+    Oxford Instruments.
+    """
+  def __init__(self, path=None):
+    EBSDPatternFile.__init__(self, path)
+    self.filetype = 'EBSP'
+    self.vendor = 'OXFORD'
+    self.filedatatype = None
+    # EBSP only attributes
+    # self.bitdepth = None
+    self.filePos = None  # file location in bytes where each pattern data starts
+    self.hasxypos = False
+
+  def read_header(self, path=None, bitdepth=None):  # readInterval=[0, -1], arrayOnly=False,
+    if path is not None:
+      self.filepath = path
+
+    try:
+      f = open(Path(self.filepath).expanduser(), 'rb')
+    except:
+      print("File Not Found:", str(Path(self.filepath)))
+      return -1
+
+    f.seek(0)
+    version = np.fromfile(f, dtype=np.int64, count=1)
+    version = int(-1*version)
+    if version <= 0:
+      self.version = 0
+    else:
+      self.version = version
+
+    per_pat_header = 4
+    if self.version >= 5:
+      per_pat_header = 6
+
+    if self.version >= 1:
+      memoffset = 8
+      if self.version >= 4:
+        self.mysterybyte = np.fromfile(f, dtype=np.uint8, count=1)
+        memoffset = 9
+      #loc0 = int(np.fromfile(f, dtype=np.uint64, count=1))
+      #currentloc = f.tell()
+      #loc1 = loc0
+      #npat = 0
+
+      #while loc1 != currentloc:
+      #  loc11 = int(np.fromfile(f, dtype=np.uint64, count = 1))
+      #  loc1 = min([loc1, loc11])
+      #  currentloc = f.tell()
+
+      # do the same as above, but in memory ... so much faster
+      loc0 = 0
+      counter = 0
+      while loc0 == 0: # check for non-stored points.
+        loc0 = int(np.fromfile(f, dtype=np.uint64, count=1))
+        counter += 1
+      f.seek(-8*counter, 1) # move back 8 bytes (or however far we needed to move into the file to find a legitamte offset.
+
+      loc02N = np.fromfile(f, dtype=np.uint64, count=int((loc0)/8+0.001))
+
+
+      if self.version <=4:
+        loc1 = int((loc0-memoffset)/8+0.001)
+
+        counter = 0
+        while loc1 != counter:
+          if loc02N[counter] != 0:  # a non-stored pattern? Crazy.
+            loc_i = int((loc02N[counter]-memoffset)/8)
+            loc1 = min([loc1, loc_i])
+          counter += 1
+
+
+        self.nPatterns = int((counter))
+      elif self.version == 5:
+        f.seek(loc02N[0], 0)
+        patdata = np.fromfile(f, dtype=np.uint32, count=per_pat_header)
+        if patdata[0] == 1:
+          print("Sorry, compressed EBSP files are not supported")
+          return None
+        patternW = int(patdata[-2])
+        patternH = int(patdata[-3])
+        magic_indx = patternH + (patternW << 32)
+        wh = np.nonzero(loc02N == magic_indx)
+        self.nPatterns = wh[0].min()
+
+
+
+      if self.version == 0:
+        f.seek(0)
+      if self.version >=1.0:
+        f.seek(8)
+      if self.version >= 4:
+        f.seek(1,1)
+
+
+
+      self.filePos = np.fromfile(f, dtype=np.uint64, count=self.nPatterns)
+
+      # going to assume that all patterns are the same as the first pattern the file.
+      f.seek(self.filePos[0])
+      #patdata = np.fromfile(f, dtype=np.uint32, count=4)
+      #patdata0 = np.fromfile(f, dtype=np.uint8, count=1)
+
+      #patdata = np.fromfile(f, dtype=np.uint32, count=4)
+
+      patdata = np.fromfile(f, dtype=np.uint32, count=per_pat_header)
+
+      if patdata[0] == 1:
+        print("Sorry, compressed EBSP files are not supported")
+        return None
+
+      #print(loc0, patdata)
+      #f.seek(self.filePos[2])
+      #print(np.fromfile(f, dtype=np.uint32, count=4))
+      #print(np.fromfile(f, dtype=np.uint32, count=8))
+      #print(np.fromfile(f, dtype=np.uint32, count=1))
+
+      self.patternW = np.uint32(patdata[-2])
+      self.patternH = np.uint32(patdata[-3])
+      nbytespat = patdata[-1]
+
+
+      #if self.version == 1:
+      bitdepth = nbytespat / (self.patternW * self.patternH) * 8
+      #elif self.version >= 2:
+      #bitdepth = nbytespat
+
+      if bitdepth == 8:
+        self.filedatatype = np.uint8
+      if bitdepth == 16:
+        self.filedatatype = np.uint16
+      if bitdepth == 32:
+        self.filedatatype = np.uint32
+
+
+      #self.nPatterns = int(
+      #                (Path(self.filepath).expanduser().stat().st_size - int(8)) /
+      #                        (24 + 18 +
+      #                         int(self.patternW) * int(self.patternH) * int(self.filedatatype(0).nbytes)))
+
+      #print(self.nPatterns)
+
+
+
+      xall = np.zeros(self.nPatterns, dtype=np.float64)
+      yall = np.zeros(self.nPatterns, dtype=np.float64)
+      self.hasxypos = False
+      if self.version != 0:
+        if self.version ==1:
+          footoffset = 0
+          self.hasxypos = True
+        else:
+          loc0 = np.min(self.filePos[self.filePos > 0])
+          f.seek(int(loc0 + 4*per_pat_header + nbytespat))
+          havepos = np.fromfile(f, dtype=np.uint8, count=1)
+          if havepos > 0:
+            footoffset = 1
+            self.hasxypos = True
+
+      if self.hasxypos == False:
+        self.xStep = 1.0
+        self.yStep = 1.0
+        self.nCols = 1
+        self.nRows = self.nPatterns
+      else:
+        for i in range(self.nPatterns):
+          if self.filePos[i] > 0:
+            f.seek(int(self.filePos[i] + 4*per_pat_header + nbytespat + footoffset))
+
+            x1 = np.fromfile(f, dtype=np.float64, count=1)
+            #print(x1, i)
+            xall[i] = x1
+            f.seek(footoffset, 1)
+            yall[i] = np.fromfile(f, dtype=np.float64, count=1)
+
+
+        self.xStep = xall[1] - xall[0]
+        if self.xStep > 1e-6:
+          ncol = (xall.max() - xall.min()) / self.xStep
+          ncol = np.round(ncol+1)
+        else:
+          ncol = 1
+
+        self.nCols = np.uint64(ncol)
+
+
+        self.yStep = yall[0] - yall[self.nCols]
+
+        if self.yStep > 1e-6:
+          nrow = (yall.max() - yall.min()) / self.yStep
+          nrow = np.round(nrow+1)
+          self.nRows = int(nrow)
+        else:
+          self.nRows = int(self.nPatterns/self.nCols+0.001)
+
+      if self.xStep is None:
+        self.xStep = 1.0
+      if self.yStep is None:
+        self.yStep = 1.0
+      if self.nCols is None:
+        self.nCols = np.uint64(1)
+      if self.nCols == 0:
+        self.nCols = np.uint64(1)
+      if self.nRows is None:
+        self.nRows = np.uint64(np.floor(self.nPatterns / self.nCols))
+    f.close()
+
+    return 0  # note this function uses multiple returns
+
+  def pat_reader(self, patStart=0, nPatToRead=1):
+    try:
+      f = open(Path(self.filepath).expanduser(), 'rb')
+    except:
+      print("File Not Found:", str(Path(self.filepath)))
+      return -1
+
+    readpats = np.zeros((nPatToRead, self.patternH * self.patternW), dtype=self.filedatatype)
+    xyloc = np.zeros((nPatToRead, 2), dtype=np.float64)
+    # f.seek(self.filePos)
+    nPerPat = self.patternW * self.patternH
+    typeread = self.filedatatype
+    typebyte = self.filedatatype(0).nbytes
+
+    readxypos = self.hasxypos
+    if self.version == 1:
+      xyoffset = 0
+    else:
+      xyoffset = 1
+
+    per_pat_head = 16
+    if self.version >= 5:
+      per_pat_head = 24
+
+    for i in range(int(patStart), int(patStart + nPatToRead)):
+      ii = int(i - patStart)
+      if self.filePos[i] > 0:
+        f.seek(int(self.filePos[i] + per_pat_head))
+        readpats[ii, :] = np.fromfile(f, dtype=typeread, count=int(nPerPat))
+        if readxypos == True:
+          f.seek(xyoffset, 1)
+          xyloc[ii, 0] = np.fromfile(f, dtype=np.float64, count=1)
+          f.seek(xyoffset, 1)
+          xyloc[ii, 1] = np.fromfile(f, dtype=np.float64, count=1)
+
+    readpats = readpats.reshape(nPatToRead, self.patternH, self.patternW)
+    f.close()
+
+    # yx = np.unravel_index(np.arange(int(patStart), int(patStart+nPatToRead), dtype = np.uint64),
+    #                       (int(self.nRows), int(self.nCols)))
+
+    # xyloc = np.array([yx[1],yx[0]]).T.copy().astype(np.float32)
+    # xyloc[:,0] -= self.nCols * 0.5
+    # xyloc[:, 1] -= self.nRows * 0.5
+    # xyloc[:,0] *= self.xStep
+    # xyloc[:,1] *= self.yStep
+    return readpats, xyloc
+
+  def write_header(self, writeBlank=False, bitdepth=8):
+
+    filepath = self.filepath
+    extension = str.lower(Path(filepath).suffix)
+    try:
+      if (bitdepth is None) and (self.filedatatype is None):
+        raise ValueError('Error: extension not recognized, set "bitdepth" parameter')
+      elif (bitdepth == 8):
+        self.filedatatype = np.uint8
+      elif (bitdepth == 16):
+        self.filedatatype = np.uint16
+    except ValueError as exp:
+      print(exp)
+      return -1
+
+    try:
+      if os.path.isfile(Path(self.filepath).expanduser()):
+        f = open(Path(filepath).expanduser(), 'r+b')
+        f.seek(0)
+      else:
+        f = open(Path(filepath).expanduser(), 'w+b')
+        f.seek(0)
+    except:
+      print("File Not Found:", str(Path(filepath)))
+      return -1
+
+    if self.version is None:
+      self.version = 2
+
+    if self.version > 0:
+      version = np.uint64(-self.version)
+      np.asarray(version, dtype=np.uint64).tofile(f)
+
+    if self.version >= 0:
+      if self.filePos is None:
+        file_head_length = 0
+        pat_footer_length = 0
+        if self.version >= 1:
+          file_head_length = 8
+          pat_footer_length = 16
+        if self.version >= 2:
+          if self.hasxypos == True:
+            pat_footer_length = 18
+          else:
+            pat_footer_length = 1
+
+        if self.version >= 4:
+          file_head_length = 9
+
+        self.filePos = np.arange(
+          self.nPatterns, dtype=np.uint64)*(16+pat_footer_length+self.patternH*self.patternW*self.filedatatype(0).nbytes)\
+                       +file_head_length+8*self.nPatterns
+
+      if self.version >= 4:
+        np.uint8(0).tofile(f)
+
+      np.asarray(self.filePos, dtype=np.uint64).tofile(f)
+
+    if writeBlank == True:
+      typewrite = self.filedatatype
+      # if self.bitdepth == 8:
+      #   type = np.uint8
+      # if self.bitdepth == 16:
+      #   type = np.uint16
+
+      blank = np.zeros((self.patternH, self.patternW), dtype=typewrite)
+      pathead = np.array([0, self.patternH, self.patternW,
+                          self.patternH * self.patternW * self.filedatatype(0).nbytes], dtype=np.uint32)
+
+      for j in range(self.nRows):
+        for i in range(self.nCols):
+          pathead.tofile(f)
+          blank.tofile(f)
+          if (self.version > 0) and self.hasxypos:
+            if self.version >= 2:
+              np.uint8(1).tofile(f)
+            np.float64(i * self.xStep - 0.5*(self.nCols*self.xStep)).tofile(f)
+            if self.version >= 2:
+              np.uint8(1).tofile(f)
+            np.float64(j * self.yStep - 0.5*(self.nRows*self.yStep)).tofile(f)
+          else: # no xy_pos info
+            if self.version >= 2:
+              np.uint8(0).tofile(f)
+    f.close()
+
+  def pat_writer(self, pat2write, patStart, nPatToWrite, typewrite=None):
+    try:
+      f = open(Path(self.filepath).expanduser(), 'br+')
+      f.seek(0, 0)
+    except:
+      print("File Not Found:", str(Path(self.filepath)))
+      return -1
+
+    nPerPat = self.patternW * self.patternH
+    nPerPatByte = nPerPat * typewrite(0).nbytes
+    pathead = np.array([0, int(self.patternH), int(self.patternW),
+                        int(self.patternH * self.patternW * self.filedatatype(0).nbytes)], dtype=np.uint32)
+
+    write_xypos = self.hasxypos
+
+    for i in range(int(patStart), int(patStart + nPatToWrite)):
+      if int(self.filePos[i]) > 0:
+        f.seek(int(self.filePos[i]), 0)
+        ii = int(i - patStart)
+        pathead.tofile(f)
+        pat2write[ii, :, :].tofile(f)
+        if write_xypos:
+          if self.version >= 2:
+            np.uint8(1).tofile(f)
+          yx = np.array(np.unravel_index(i, (self.nRows, self.nCols))).astype(np.float64)
+          yx[1] -= float(self.nCols * 0.5)
+          yx[1] *= self.xStep
+          yx[0] -= float(self.nRows * 0.5)
+          yx[0] *= self.yStep
+          np.float64(yx[1]).tofile(f)
+          if self.version >= 2:
+            np.uint8(1).tofile(f)
+          np.float64(yx[0]).tofile(f)
+    f.close()
 
 
 class HDF5PatFile(EBSDPatternFile):
   def __init__(self, path=None):
     filepath = None
     hdf5path = None
     self.patternh5id = 'Pattern'  # the name used for the pattern dataset array in the h5 file.
@@ -643,41 +1102,49 @@
         if 'EBSD' in f[grpset]:
           if 'Data' in f[grpset + '/EBSD/']:
             if self.patternh5id in f[grpset + '/EBSD/Data']:
               if (grpset  not in self.h5datagroups):
                 self.h5datagroups.append(grpset)
       else:
         self.h5othergrps.append(grpset)
-
+    f.close()
     if len(self.h5datagroups) < 1:
       print("No viable EBSD patterns found:",str(Path(self.filepath)))
       return -2
     else:
       if verbose > 0:
         print(self.h5datagroups)
     return len(self.h5datagroups)
 
 
 
-  def pat_reader(self,patStart,nPatToRead):
+  def pat_reader(self,patStart=0,nPatToRead=1):
     '''This is a basic function that will read a chunk of patterns from the HDF5 file.
     Mainly this is intended to be called by the parent class function read_data.
     It assumes that patterns are laid out in a HDF5 dataset as an array
     of N patterns x pattern height x pattern width.  '''
     try:
       f = h5py.File(Path(self.filepath).expanduser(),'r')
     except:
       print("File Not Found:",str(Path(self.filepath)))
       return -1
 
     patterndset = f[self.h5patdatpth]
     readpats = np.array(patterndset[int(patStart):int(patStart+nPatToRead), :, :])
     readpats = readpats.reshape(nPatToRead,self.patternH,self.patternW)
     f.close()
-    return readpats
+    yx = np.unravel_index(np.arange(patStart, patStart + nPatToRead), (self.nRows, self.nCols))
+
+    xyloc = np.array([yx[1], yx[0]]).T.copy().astype(np.float32)
+    xyloc[:, 0] -= self.nCols * 0.5
+    xyloc[:, 1] -= self.nRows * 0.5
+    xyloc[:, 0] *= self.xStep
+    xyloc[:, 1] *= self.yStep
+
+    return readpats, xyloc
 
   def copy_file(self, newpath, **kwargs):
     # oh - this is a mess!
     pathtemp = np.atleast_1d(newpath)
     fpath = Path(pathtemp[0]).expanduser().resolve()
     #print(pathtemp)
     hdf5path = None
@@ -757,14 +1224,24 @@
     if self.h5patdatpth is not None:
       dset = f[self.h5patdatpth]
       shp = np.array(dset.shape)
       self.patternW = shp[-1]
       self.patternH = shp[-2]
       self.nPatterns = shp[-3]
       self.filedatatype = dset.dtype.type
+      if self.xStep is None:
+        self.xStep = 0.0
+      if self.yStep is None:
+        self.yStep = 0.0
+      if self.nCols is None:
+        self.nCols = np.uint64(1)
+      if self.nCols == 0:
+        self.nCols = np.uint64(1)
+      if self.nRows is None:
+        self.nRows = np.uint64(np.floor(self.nPatterns/self.nCols))
 
 class EDAXOH5(HDF5PatFile):
   def __init__(self, path=None):
     HDF5PatFile.__init__(self, path)
     self.vendor = 'EDAX'
     #EDAXOH5 only attributes
     self.filedatatype = None # np.uint8
@@ -787,15 +1264,15 @@
 
     try:
       f = h5py.File(Path(self.filepath).expanduser(),'r')
     except:
       print("File Not Found:",str(Path(self.filepath)))
       return -1
 
-    self.version = str(f['Version'][()][0])
+    self.version = str(f['Version'][()][0].decode('UTF-8'))
 
     if self.version  >= 'OIM Analysis 8.6.00':
       ngrp = self.get_data_paths()
       if ngrp <= 0:
         f.close()
         return -2 # no data groups with patterns found.
       if self.h5patdatpth is None: # default to the first datagroup
@@ -804,17 +1281,17 @@
       dset = f[self.h5patdatpth]
       shp = np.array(dset.shape)
       self.patternW = shp[-1]
       self.patternH = shp[-2]
       self.nPatterns = shp[-3]
       self.filedatatype = dset.dtype.type
       headerpath = (f[self.h5patdatpth].parent.parent)["Header"]
-      self.nCols = np.int32(headerpath['nColumns'][()][0])
-      self.nRows = np.int32(headerpath['nRows'][()][0])
-      self.hexFlag = np.int32(headerpath['Grid Type'][()][0] == 'HexGrid')
+      self.nCols = np.uint32(headerpath['nColumns'][()][0])
+      self.nRows = np.uint32(headerpath['nRows'][()][0])
+      self.hexflag = np.uint32(headerpath['Grid Type'][()][0] == 'HexGrid')
 
       self.xStep = np.float32(headerpath['Step X'][()][0])
       self.yStep = np.float32(headerpath['Step Y'][()][0])
 
     return 0 #note this function uses multiple returns
 
 class KIKUCHIPYH5(HDF5PatFile):
@@ -859,17 +1336,17 @@
       dset = f[self.h5patdatpth]
       shp = np.array(dset.shape)
       self.patternW = shp[-1]
       self.patternH = shp[-2]
       self.nPatterns = shp[-3]
       self.filedatatype = dset.dtype.type
       headerpath = (f[self.h5patdatpth].parent.parent)["Header"]
-      self.nCols = np.int32(headerpath['n_columns'][()][0])
-      self.nRows = np.int32(headerpath['n_rows'][()][0])
-      self.hexFlag = np.int32(headerpath['grid_type'][()][0] == 'hexagonal')
+      self.nCols = np.uint32(headerpath['n_columns'][()][0])
+      self.nRows = np.uint32(headerpath['n_rows'][()][0])
+      self.hexflag = np.uint32(headerpath['grid_type'][()][0] == 'hexagonal')
 
       self.xStep = np.float32(headerpath['step_x'][()][0])
       self.yStep = np.float32(headerpath['step_y'][()][0])
 
     return 0 #note this function uses multiple returns
 
 
@@ -897,15 +1374,15 @@
 
     try:
       f = h5py.File(Path(self.filepath).expanduser().resolve(),'r')
     except:
       print("File Not Found:",str(Path(self.filepath)))
       return -1
 
-    self.version = str(f['Version'][()][0])
+    self.version = str(f['Version'][()].decode('UTF-8'))
 
     if self.version.upper()  >= 'ESPIRT 2.X':
       ngrp = self.get_data_paths()
       if ngrp <= 0:
         f.close()
         return -2 # no data groups with patterns found.
       if self.h5patdatpth is None: # default to the first datagroup
@@ -914,15 +1391,118 @@
       dset = f[self.h5patdatpth]
       shp = np.array(dset.shape)
       self.patternW = shp[-1]
       self.patternH = shp[-2]
       self.nPatterns = shp[-3]
       self.filedatatype = dset.dtype.type
       headerpath = (f[self.h5patdatpth].parent.parent)["Header"]
-      self.nCols = np.int32(headerpath['NCOLS'][()][0])
-      self.nRows = np.int32(headerpath['NROWS'][()][0])
-      #self.hexFlag = np.int32(f[headerpath+'Grid Type'][()][0] == 'HexGrid')
+      self.nCols = np.uint32(headerpath['NCOLS'][()])
+      self.nRows = np.uint32(headerpath['NROWS'][()])
+      #self.hexflag = np.int32(f[headerpath+'Grid Type'][()][0] == 'HexGrid')
+
+      self.xStep = np.float32(headerpath['XSTEP'][()])
+      self.yStep = np.float32(headerpath['YSTEP'][()])
+
+    return 0 #note this function uses multiple returns
+
+class OXFORDOINA(HDF5PatFile):
+  def __init__(self, path=None):
+    HDF5PatFile.__init__(self, path)
+    self.vendor = 'OXFORD'
+    #OXFORDOINA only attributes
+    self.filedatatype = None # np.uint8
+    self.patternh5id = 'Processed Patterns' # Could also be 'Raw Patterns'
+
+    if self.filepath is not None:
+      self.get_data_paths()
+
+  def set_data_path(self, datapath=None, pathindex=0): #overloaded from parent - will default to first group.
+    if datapath is not None:
+      self.h5patdatpth = datapath
+    else:
+      if len(self.h5datagroups) > 0:
+        #self.activegroupid = pathindex
+        self.h5patdatpth = self.h5datagroups[pathindex] + '/EBSD/Data/' + self.patternh5id
+  def get_data_paths(self, verbose=0, getraw = False):
+    '''Based on the OINA spec this will search for viable Pattern Datasets '''
+    try:
+      f = h5py.File(self.filepath,'r')
+    except:
+      print("File Not Found:",str(Path(self.filepath)))
+      return -1
+    self.h5datagroups = []
+    self.h5othergrps = []
+    if getraw is True:
+      self.patternh5id = 'Raw Patterns'
+    groupsets = list(f.keys())
+    for grpset in groupsets:
+      if isinstance(f[grpset],h5py.Group):
+        if 'EBSD' in f[grpset]:
+          if 'Data' in f[grpset + '/EBSD/']:
+            if self.patternh5id in f[grpset + '/EBSD/Data']:
+              if (grpset  not in self.h5datagroups):
+                self.h5datagroups.append(grpset)
+      else:
+        self.h5othergrps.append(grpset)
+    f.close()
+
+    if (len(self.h5datagroups) < 1) and (getraw is False):
+      self.get_data_paths(self, verbose=False, getraw=True)
+
+    if len(self.h5datagroups) < 1:
+      print("No viable EBSD patterns found:",str(Path(self.filepath)))
+      return -2
+    else:
+      if verbose > 0:
+        print(self.h5datagroups)
+    return len(self.h5datagroups)
+  def read_header(self, path=None):
+    
+    if path is not None:
+      self.filepath = path
+
+    try:
+      f = h5py.File(Path(self.filepath).expanduser(),'r')
+    except:
+      print("File Not Found:",str(Path(self.filepath)))
+      return -1
+
+    self.version = str(f['Format Version'][()][0].decode('UTF-8'))
+
+    if self.version >= '5.0':
+      ngrp = self.get_data_paths()
+      if ngrp <= 0:
+        f.close()
+        return -2 # no data groups with patterns found.
+      if self.h5patdatpth is None: # default to the first datagroup
+        self.set_data_path(pathindex=0)
+
+      dset = f[self.h5patdatpth]
+      shp = np.array(dset.shape)
+      self.patternW = shp[-1]
+      self.patternH = shp[-2]
+      self.nPatterns = shp[-3]
+      self.filedatatype = dset.dtype.type
+      headerpath = (f[self.h5patdatpth].parent.parent)["Header"]
+      self.nCols = np.uint32(headerpath['X Cells'][()][0])
+      self.nRows = np.uint32(headerpath['Y Cells'][()][0])
+      #self.hexflag = np.int32(headerpath['Grid Type'][()][0] == 'HexGrid')
 
-      self.xStep = np.float32(headerpath['XSTEP'][()][0])
-      self.yStep = np.float32(headerpath['YSTEP'][()][0])
+      self.xStep = np.float32(headerpath['X Step'][()][0])
+      self.yStep = np.float32(headerpath['Y Step'][()][0])
 
     return 0 #note this function uses multiple returns
+
+  def pat_reader(self, patStart=0, nPatToRead=1):
+
+    patterns, xyloc = HDF5PatFile.pat_reader(self, patStart, nPatToRead)
+    try:
+      f = h5py.File(Path(self.filepath).expanduser(),'r')
+      xloc = (f[self.h5patdatpth].parent)["Beam Position X"]
+      xyloc[:,0] = np.array(xloc[int(patStart):int(patStart + nPatToRead)]).astype(np.float32)
+      yloc = (f[self.h5patdatpth].parent)["Beam Position Y"]
+      xyloc[:, 1] = np.array(yloc[int(patStart):int(patStart + nPatToRead)]).astype(np.float32)
+      f.close()
+    except:
+      print("File Not Found:",str(Path(self.filepath)))
+
+    return patterns, xyloc
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/nlpar.py` & `pyebsdindex-0.3.0/pyebsdindex/nlpar_cpu.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,17 +14,20 @@
 # that you changed the software and should note the date and nature of any such change.
 # Please explicitly acknowledge the US Naval Research Laboratory as the original source.
 # This software can be redistributed and/or modified freely provided that any derivative
 # works bear some notice that they are derived from it, and any modified versions bear
 # some notice that they have been modified.
 #
 # Author: David Rowenhorst;
-# The US Naval Research Laboratory Date: 21 Aug 2020
+# The US Naval Research Laboratory Date: 22 May 2024
+
+# For more info see
+# Patrick T. Brewick, Stuart I. Wright, David J. Rowenhorst. Ultramicroscopy, 200:50–61, May 2019.
+
 
-"""Non-local pattern averaging and re-indexing (NLPAR)."""
 
 from pathlib import Path
 from timeit import default_timer as timer
 
 import numba
 import numpy as np
 import scipy.optimize as opt
@@ -37,27 +40,28 @@
 
 __all__ = [
     "NLPAR",
 ]
 
 
 class NLPAR:
-  def __init__(self, filename=None,  lam=0.7, searchradius=3,dthresh=0.0, nrows = None, ncols = None):
+  def __init__(self, filename=None,  lam=0.7, searchradius=3,dthresh=0.0, nrows = None, ncols = None, **kwargs):
     self.lam = lam
     self.searchradius = searchradius
     self.dthresh = dthresh
     self.filepath = None
     self.hdfdatapath = None
     self.filepathout = None
     self.hdfdatapathout = None
     #self.patternfile = None
     #self.patternfileout = None
     self.setfile(filename)
     self.mask = None
     self.sigma = None
+    self.sigmann = 1
     self.nrows = None
     self.ncols = None
     if nrows is not None:
       self.nrows = nrows
     if ncols is not None:
       self.ncols = ncols
 
@@ -70,22 +74,31 @@
     hdf5path = None
     if pathtemp.size > 1:
       hdf5path = pathtemp[1]
     if fpath is not None:
       self.filepath = Path(fpath)
       self.hdfdatapath = hdf5path
 
+  def setoutfile(self, patternfile, filepath=None):
+    """Set the output file.
 
-
-
-  def setoutfile(self,patternfile, filepath=None):
-    '''patternfile is an input pattern file object from ebsd_pattern.  Filepath is a string.
-    In the future I want to be able to specify the HDF5 data path to store the output data, but that
-    is proving to be a bit of a mess.  For now, a copy of the original HDF5 is made, and the NLPAR patterns will be
-    overwritten on top of the originals. '''
+    Parameters
+    ----------
+    patternfile
+      Input pattern file object from ebsd_pattern.
+    filepath
+      String.
+
+    Notes
+    -----
+    In the future I want to be able to specify the HDF5 data path to
+    store the output data, but that is proving to be a bit of a mess.
+    For now, a copy of the original HDF5 is made, and the NLPAR patterns
+    will be overwritten on top of the originals.
+    """
     self.filepathout = None
     self.hdfdatapathout = None
     pathtemp = np.atleast_1d(filepath)
     fpath = pathtemp[0]
     hdf5path = None
     #if pathtemp.size > 1:
     #  hdf5path = pathtemp[1]
@@ -97,74 +110,90 @@
         pathok = self.filepathout.exists()
         if pathok:
           pathok = not self.filepathout.samefile(patternfile.filepath)
           if not pathok:
             raise ValueError('Error: File input and output are exactly the same.')
             return
 
-        patternfile.copy_file([self.filepathout,self.hdfdatapathout] )
+        patternfile.copy_file([self.filepathout,self.hdfdatapathout], empty_data=True)
         return  # fpath and (maybe) hdf5 path were set manually.
       else: # this is a hdf5 file
         if self.hdfdatapathout is None:
-          patternfile.copy_file(self.filepathout)
+          patternfile.copy_file(self.filepathout, empty_data=True)
           self.hdfdatapathout = patternfile.h5patdatpth
           return
         else:
-          patternfile.copy_file([self.filepathout, self.hdfdatapathout])
+          patternfile.copy_file([self.filepathout, self.hdfdatapathout], empty_data=True)
           return
 
     if patternfile is not None: # the user has set no path.
       hdf5path = None
-      if patternfile.filetype == 'UP':
+      
+      if patternfile.filetype in ['UP', 'EBSP']:
         p = Path(patternfile.filepath)
         appnd = "_NLPAR_l{:1.2f}".format(self.lam) + "sr{:d}".format(self.searchradius)
         newfilepath = str(p.parent / Path(p.stem + appnd + p.suffix))
-        patternfile.copy_file(newfilepath)
+        patternfile.copy_file(newfilepath,empty_data=True)
 
       if patternfile.filetype == 'HDF5':
         hdf5path_tmp = str(patternfile.h5patdatpth).split('/')
         if hdf5path_tmp[0] == '':
           hdf5path_org =  hdf5path_tmp[1]
         else:
           hdf5path_org = hdf5path_tmp[0]
         p = Path(patternfile.filepath)
         appnd = "_NLPAR_l{:1.2f}".format(self.lam) + "sr{:d}".format(self.searchradius)
         hdf5path = hdf5path_org+appnd
         newfilepath = str(p.parent / Path(p.stem + appnd + p.suffix))
         #patternfile.copy_file([newfilepath, hdf5path_org], newh5path=hdf5path)
-        patternfile.copy_file([newfilepath])
+        patternfile.copy_file([newfilepath], empty_data=True)
         hdf5path = patternfile.h5patdatpth
 
       self.filepathout = newfilepath
       self.hdfdatapathout = hdf5path
       return
 
   def getinfileobj(self):
     if self.filepath is not None:
       fID = ebsd_pattern.get_pattern_file_obj([self.filepath, self.hdfdatapath])
-      if fID.nRows is not None:
-        self.nrows = fID.nRows
-      else:
-        fID.nRows = self.nrows
-      if fID.nCols is not None:
-        self.ncols = fID.nCols
-      else:
-        fID.nCols = self.ncols
+      if (fID.nRows is not None):
+        if (self.nrows is None):
+          self.nrows = fID.nRows
+        else:
+          fID.nRows = self.nrows
+
+      if (fID.nCols is not None):
+        if (self.ncols is None):
+          self.ncols = fID.nCols
+        else:
+          fID.nCols = self.ncols
+
       return fID
+
     else:
       return None
 
   def getoutfileobj(self):
     if self.filepathout is not None:
-      return ebsd_pattern.get_pattern_file_obj([self.filepathout, self.hdfdatapathout])
+      fID = ebsd_pattern.get_pattern_file_obj([self.filepathout, self.hdfdatapathout])
+      if self.nrows is not None:
+        fID.nRows = self.nrows
+      else:
+        self.nrows = fID.nRows
+
+      if self.ncols is not None:
+        fID.nCols = self.ncols
+      else:
+        self.ncols = fID.nCols
+      return fID
     else:
       return None
 
   def opt_lambda(self,chunksize=0,saturation_protect=True,automask=True, backsub = False,
-                 target_weights=[0.5, 0.34, 0.25], dthresh=0.0, autoupdate=True):
+                target_weights=(0.5, 0.34, 0.25), dthresh=0.0, autoupdate=True, verbose = 2, **kwargs):
 
     target_weights = np.asarray(target_weights)
 
     def loptfunc(lam,d2,tw,dthresh):
       temp = (d2 > dthresh).choose(dthresh, d2)
       dw = np.exp(-(temp) / lam ** 2)
       w = np.sum(dw, axis=2) + 1e-12
@@ -206,29 +235,35 @@
     nn = np.uint64(nn)
 
     if (automask is True) and (self.mask is None):
       self.mask = (self.automask(pheight,pwidth))
     if self.mask is None:
       self.mask = np.ones((pheight,pwidth),dtype=np.uint8)
 
+    self.mask = (self.mask).astype(np.uint8)
     indices = np.asarray((self.mask.flatten().nonzero())[0],np.uint64)
 
     sigma = np.zeros((nrows,ncols),dtype=np.float32)+1e24
     colstartcount = np.asarray([0,ncols],dtype=np.int64)
 
 
     dthresh = np.float32(dthresh)
     lamopt_values = []
+    
     for j in range(0,nrows,chunksize):
-      print('Block',j)
+
+      if verbose >= 2:
+        print("begin row: ", j, "/", nrows, sep='', end='\r')
+      #print('Block',j)
+
       #rowstartread = np.int64(max(0,j - nn))
       rowstartread = np.int64(j)
       rowend = min(j + chunksize + nn,nrows)
       rowcountread = np.int64(rowend - rowstartread)
-      data = patternfile.read_data(patStartCount=[[0,rowstartread],[ncols,rowcountread]],
+      data, xyloc = patternfile.read_data(patStartCount=[[0,rowstartread],[ncols,rowcountread]],
                                         convertToFloat=True,returnArrayOnly=True)
 
       shp = data.shape
 
       if backsub is True:
         data = self.backsub(data)
         #back = np.mean(data, axis=0)
@@ -239,33 +274,42 @@
       rowstartcount = np.asarray([0,rowcountread],dtype=np.int64)
       sigchunk, (d2,n2, dij) = self.sigma_numba(data,nn,rowcountread,ncols,rowstartcount,colstartcount,indices,saturation_protect)
       tmp = (sigma[j:j + rowstartcount[1],:] < sigchunk).choose( sigchunk, sigma[j:j + rowstartcount[1],:])
       sigma[j:j + rowstartcount[1],:] = tmp
 
 
       d2norm(d2, n2, dij, sigchunk)
+
+
       lamopt_values_chnk = []
       for tw in target_weights:
         lam = 1.0
         lambopt1 = opt.minimize(loptfunc,lam,args=(d2,tw,dthresh),method='Nelder-Mead',
                                 bounds = [[0.001, 10.0]],options={'fatol': 0.0001})
         lamopt_values_chnk.append(lambopt1['x'])
 
 
       lamopt_values.append(lamopt_values_chnk)
+
+    if verbose >= 2:
+      print('', end='')
     lamopt_values = np.asarray(lamopt_values)
-    print("Range of lambda values: ", np.mean(lamopt_values, axis = 0).flatten())
-    print("Optimal Choice: ", np.median(np.mean(lamopt_values, axis = 0)))
+    if verbose >=1:
+      print("Range of lambda values: ", np.mean(lamopt_values, axis = 0).flatten())
+      print("Optimal Choice: ", np.median(np.mean(lamopt_values, axis = 0)))
+
     if autoupdate == True:
       self.lam = np.median(np.mean(lamopt_values, axis = 0))
     if self.sigma is None:
       self.sigma = sigma
+    return np.mean(lamopt_values, axis = 0).flatten()
 
   def calcnlpar(self, chunksize=0, searchradius=None, lam = None, dthresh = None, saturation_protect=True, automask=True,
-                filename=None, fileout=None, reset_sigma=True, backsub = False, rescale = False):
+               filename=None, fileout=None, reset_sigma=False, backsub = False, rescale = False,verbose=2,
+                **kwargs):
 
     if lam is not None:
       self.lam = lam
 
     if dthresh is not None:
       self.dthresh = dthresh
 
@@ -275,16 +319,16 @@
     lam = np.float32(self.lam)
     dthresh = np.float32(self.dthresh)
     sr = np.int64(self.searchradius)
 
     if filename is not None:
       self.setfile(filepath=filename)
 
-    if reset_sigma:
-      self.sigma = None
+
+
 
     patternfile = self.getinfileobj()
 
     #if filepathout is not None:
     self.setoutfile(patternfile, filepath=fileout)
 
     patternfileout = self.getoutfileobj()
@@ -317,45 +361,55 @@
 
     indices = np.asarray( (self.mask.flatten().nonzero())[0], np.uint64)
     calcsigma = False
     if self.sigma is None:
       calcsigma = True
       self.sigma = np.zeros((nrows, ncols), dtype=np.float32)+1e24
 
+    if reset_sigma:
+      self.sigma = None
 
-    if np.asarray(self.sigma).size == 1:
+    if (np.asarray(self.sigma).size == 1) and (self.sigma is not None):
       tmp = np.asarray(self.sigma)[0]
       self.sigma =  np.zeros((nrows, ncols), dtype=np.float32)+tmp
       calcsigma = False
 
     shpsigma = np.asarray(self.sigma).shape
     if (shpsigma[0] != nrows) and (shpsigma[1] != ncols):
       self.sigma = np.zeros((nrows,ncols),dtype=np.float32) + 1e24
       calcsigma = True
 
-
     sigma = np.asarray(self.sigma)
+
     scalemethod = 'clip'
     if rescale == True:
       if np.issubdtype(patternfileout.filedatatype, np.integer):
         mxval = np.iinfo(patternfileout.filedatatype).max
         scalemethod = 'fullscale'
       else: # not int, so no rescale.
         rescale = False
 
     nthreadpos = numba.get_num_threads()
     #numba.set_num_threads(36)
     colstartcount = np.asarray([0,ncols],dtype=np.int64)
-    print(lam, sr, dthresh)
+    if verbose >= 1:
+      print("lambda:", self.lam, "search radius:", self.searchradius, "dthresh:", self.dthresh)
 
     for j in range(0,nrows,chunksize):
+      #print('Row start', j)
+      if verbose >= 2:
+        print("begin row: ", j, "/", nrows, sep='', end='\r')
+
       rowstartread = np.int64(max(0, j-sr))
       rowend = min(j + chunksize+sr,nrows)
+
+      if (rowend - rowstartread) < (2*sr+1):
+        rowstartread = np.int64(max(0, rowend - (2*sr+1)))
       rowcountread = np.int64(rowend-rowstartread)
-      data = patternfile.read_data(patStartCount = [[0,rowstartread], [ncols,rowcountread]],
+      data, xyloc = patternfile.read_data(patStartCount = [[0,rowstartread], [ncols,rowcountread]],
                                         convertToFloat=True,returnArrayOnly=True)
 
       shpdata = data.shape
 
       if backsub is True:
         data = self.backsub(data)
 
@@ -367,41 +421,47 @@
         sigchunk, tmp = self.sigma_numba(data,1,rowcountread,ncols,rowstartcount,colstartcount,indices,saturation_protect)
         del tmp
         tmp = (sigma[rowstartread:rowend,:] < sigchunk).choose(sigchunk,sigma[rowstartread:rowend,:])
         sigma[rowstartread:rowend,:] = tmp
       else:
         sigchunk = sigma[rowstartread:rowend,:]
 
-      print('Block', j)
+      #dataout = data
+
       dataout = self.nlpar_nb(data,lam, sr, dthresh, sigchunk,
                               rowcountread,ncols,indices,saturation_protect)
 
       dataout = dataout.reshape(rowcountread, ncols, phw)
       dataout = dataout[j-rowstartread:, :, : ]
       shpout = dataout.shape
       dataout = dataout.reshape(shpout[0]*shpout[1], pheight, pwidth)
       if rescale == True:
         for i in range(dataout.shape[0]):
           temp = dataout[i,:,:]
           temp -= temp.min()
-          temp *= float(mxval)/temp.max()
+          temp *= np.float32(mxval)/temp.max()
           dataout[i,:,:] = temp
 
       patternfileout.write_data(newpatterns=dataout,patStartCount = [[0,j], [ncols, shpout[0]]],
                                      flt2int='clip',scalevalue=1.0 )
       #self.patternfileout.write_data(newpatterns=dataout,patStartCount=[j*ncols,shpout[0]*shpout[1]],
       #                               flt2int='clip',scalevalue=1.0 )
       #return dataout
       #sigma[j:j+rowstartcount[1],:] += \
       #  sigchunk[rowstartcount[0]:rowstartcount[0]+rowstartcount[1],:]
-    numba.set_num_threads(nthreadpos)
 
 
-  def calcsigma(self,chunksize=0,nn=1,saturation_protect=True,automask=True):
+    if verbose >= 2:
+      print('', end='')
 
+    numba.set_num_threads(nthreadpos)
+    return str(patternfileout.filepath)
+
+  def calcsigma(self,chunksize=0,nn=1,saturation_protect=True,automask=True):
+    self.sigmann = nn
     patternfile = self.getinfileobj()
 
 
     nrows = np.int64(self.nrows)#np.uint64(patternfile.nRows)
     ncols = np.int64(self.ncols)#np.uint64(patternfile.nCols)
 
     pwidth = np.uint64(patternfile.patternW)
@@ -416,40 +476,42 @@
 
 
     nn = np.uint64(nn)
 
     if (automask is True) and (self.mask is None):
       self.mask = (self.automask(pheight,pwidth))
     if self.mask is None:
-      self.mask = np.ones((pheight,pwidth), dytype=np.uint8)
+      self.mask = np.ones((pheight,pwidth), dtype=np.uint8)
 
     indices = np.asarray( (self.mask.flatten().nonzero())[0], np.uint64)
 
     sigma = np.zeros((nrows, ncols), dtype=np.float32)
     #d_nn = np.zeros((nrows, ncols, int((2*nn+1)**2)), dtype=np.float32)
     colstartcount = np.asarray([0,ncols],dtype=np.int64)
-    dave = 0.0
+
     for j in range(0,nrows,chunksize):
       rowstartread = np.int64(max(0, j-nn))
       rowend = min(j + chunksize+nn,nrows)
+      if (rowend - rowstartread) < (3):
+        rowstartread = np.int64(max(0, rowend - (3)))
       rowcountread = np.int64(rowend-rowstartread)
-      data = patternfile.read_data(patStartCount = [[0,rowstartread], [ncols,rowcountread]],
+      data, xyloc = patternfile.read_data(patStartCount = [[0,rowstartread], [ncols,rowcountread]],
                                         convertToFloat=True,returnArrayOnly=True)
 
       shp = data.shape
       data = data.reshape(data.shape[0], phw)
 
       #data = None
       if rowend == nrows:
         rowstartcount = np.asarray([j-rowstartread,rowcountread - (j-rowstartread) ], dtype=np.int64)
       else:
         rowstartcount = np.asarray([j-rowstartread,chunksize ], dtype=np.int64)
-      dtic = timer()
+
       sigchunk, temp = self.sigma_numba(data,nn, rowcountread,ncols,rowstartcount,colstartcount,indices,saturation_protect)
-      dave += (timer() - dtic)
+
       sigma[j:j+rowstartcount[1],:] += \
         sigchunk[rowstartcount[0]:rowstartcount[0]+rowstartcount[1],:]
 
     return sigma
 
   def backsub(self, data):
     # This function will fit a 2D gaussian on top of a plane to the averaged set of patterns (data) that is provided.
@@ -553,39 +615,41 @@
         count = 0
         for j_nn in range(nn_r_start,nn_r_end ):
           for i_nn in range(nn_c_start,nn_c_end):
             dij[j,i,count,0] = np.uint64(j_nn)
             dij[j,i,count,1] = np.uint64(i_nn) # want to save this for labmda optimization
             indx_nn = i_nn+ncols*j_nn
             d2 = np.float32(0.0)
-            n2 = np.float32(0.0)
+            n2 = np.float32(1.0e-12)
             nout[j,i,count] = n0 # want to save this for labmda optimization
             if not((i == i_nn) and (j == j_nn)):
               for q in range(shpind[0]):
                 d0 = data[indx_0, indices[q]]
                 d1 = data[indx_nn, indices[q]]
                 if (d1 < mxval) and (d0 < mxval):
                   n2 += 1.0
                   d2 += (d0 - d1)**2
               nout[j,i,count] = n2
-              s0 = d2 / np.float32(n2 * 2.0)
+
               if d2 >= 1.e-3: #sometimes EDAX collects the same pattern twice
+                s0 = d2 / np.float32(n2 * 2.0)
                 if s0 < mind:
                   mind = s0
             dout[j,i,count] = d2 # want to save this for labmda optimization
 
             count += 1
 
         sigma[j,i] = np.sqrt(mind)
+        #if sigma[j,i] > 1e12:
+        #  print(sigma[j,i], dout[j,i,:], nout[i,j,:])
     return sigma,( dout, nout, dij)
 
   @staticmethod
-  @numba.jit(nopython=True,cache=True,fastmath=True,parallel=True)
+  @numba.jit(nopython=True,cache=True,fastmath=False,parallel=True)
   def nlpar_nb(data,lam, sr, dthresh, sigma, nrows,ncols,indices,saturation_protect=True):
-
     def getpairid(idx0, idx1):
       idx0_t = int(idx0)
       idx1_t = int(idx1)
       if idx0 < idx1:
         pairid = idx0_t + (idx1_t << 32)
       else:
         pairid = idx1_t + (idx0_t << 32)
@@ -662,8 +726,86 @@
           weights[i_nn] /= sum
           #print(weights[i_nn], ' \n')
           for q in range(shpdata[1]):
             dataout[indx_0, q] += data[indx_nn, q]*weights[i_nn]
         #print('_______', '\n')
     return dataout
 
+  def _calcchunks(self, patdim, ncol, nrow, target_bytes=2e9, col_overlap=0, row_overlap=0, col_offset=0, row_offset=0):
+
+    col_overlap = min(col_overlap, ncol - 1)
+    row_overlap = min(row_overlap, nrow - 1)
+
+    byteperpat = patdim[-1] * patdim[-2] * 4 * 2  # assume a 4 byte float input and output array
+    byteperdataset = byteperpat * ncol * nrow
+    nchunks = int(np.ceil(byteperdataset / target_bytes))
+
+    ncolchunks = (max(np.round(np.sqrt(nchunks * float(ncol) / nrow)), 1))
+    colstep = max((ncol / ncolchunks), 1)
+    ncolchunks = max(ncol / colstep, 1)
+    colstepov = min(colstep + 2 * col_overlap, ncol)
+    ncolchunks = max(int(np.ceil(ncolchunks)), 1)
+    colstep = max(int(np.round(colstep)), 1)
+    colstepov = min(colstep + 2 * col_overlap, ncol)
+
+    nrowchunks = max(np.ceil(nchunks / ncolchunks), 1)
+    rowstep = max((nrow / nrowchunks), 1)
+    nrowchunks = max(nrow / rowstep, 1)
+    rowstepov = min(rowstep + 2 * row_overlap, nrow)
+    nrowchunks = max(int(np.ceil(nrowchunks)), 1)
+    rowstep = max(int(np.round(rowstep)), 1)
+    rowstepov = min(rowstep + 2 * row_overlap, nrow)
+
+    # colchunks = np.round(np.arange(ncolchunks+1)*ncol/ncolchunks).astype(int)
+    colchunks = np.zeros((ncolchunks, 2), dtype=int)
+    colchunks[:, 0] = (np.arange(ncolchunks) * colstep).astype(int)
+    colchunks[:, 1] = colchunks[:, 0] + colstepov - int(col_overlap)
+    colchunks[:, 0] -= col_overlap
+    colchunks[0, 0] = 0;
+
+    for i in range(ncolchunks - 1):
+      if colchunks[i + 1, 0] >= ncol:
+        colchunks = colchunks[0:i + 1, :]
+
+    ncolchunks = colchunks.shape[0]
+    colchunks[-1, 1] = ncol
+
+    colchunks += col_offset
+
+    # colproc = np.zeros((ncolchunks, 2), dtype=int)
+    # if ncolchunks > 1:
+    #   colproc[1:, 0] = col_overlap
+    # if ncolchunks > 1:
+    #   colproc[0:, 1] = colchunks[:, 1] - colchunks[:, 0] - col_overlap
+    # colproc[-1, 1] = colchunks[-1, 1] - colchunks[-1, 0]
+
+    # rowchunks = np.round(np.arange(nrowchunks + 1) * nrow / nrowchunks).astype(int)
+    rowchunks = np.zeros((nrowchunks, 2), dtype=int)
+    rowchunks[:, 0] = (np.arange(nrowchunks) * rowstep).astype(int)
+    rowchunks[:, 1] = rowchunks[:, 0] + rowstepov - int(row_overlap)
+    rowchunks[:, 0] -= row_overlap
+    rowchunks[0, 0] = 0;
+
+    for i in range(nrowchunks - 1):
+      if rowchunks[i + 1, 0] >= nrow:
+        rowchunks = rowchunks[0:i + 1, :]
+
+    nrowchunks = rowchunks.shape[0]
+    rowchunks[-1, 1] = nrow
+
+    rowchunks += row_offset
+
+    # rowproc = np.zeros((nrowchunks, 2), dtype=int)
+    # if nrowchunks > 1:
+    #   rowproc[1:, 0] = row_overlap
+    # if nrowchunks > 1:
+    #   rowproc[0:, 1] = rowchunks[:, 1] - rowchunks[:, 0] - row_overlap
+    # rowproc[-1, 1] = rowchunks[-1, 1] - rowchunks[-1, 0]
+
+    return ncolchunks, nrowchunks, colchunks, rowchunks
+
+  # def asciiupdate(self, nrow, ncol, completematrix):
+  #   cm = completematrix
+  #   ncdisplay = min(ncol, 80)
+  #   nrow
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/opencl/band_detect_cl.py` & `pyebsdindex-0.3.0/pyebsdindex/opencl/band_detect_cl.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,20 +28,19 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pyopencl as cl
 
 from pyebsdindex import band_detect
 from pyebsdindex.opencl import openclparam
+import scipy
 
 #from os import environ
 #environ['PYOPENCL_COMPILER_OUTPUT'] = '1'
-tempdir = PurePath("/tmp" if platform.system() == "Darwin" else tempfile.gettempdir())
-tempdir = tempdir.joinpath('numba')
-environ["NUMBA_CACHE_DIR"] = str(tempdir)
+
 
 RADEG = 180.0/np.pi
 
 
 
 class BandDetect(band_detect.BandDetect):
   def __init__( self, **kwargs):
@@ -61,17 +60,28 @@
     #  print(type(clparams.queue))
 
     try:
       tic0 = timer()
       tic = timer()
       ndim = patternsIn.ndim
       if ndim == 2:
-        patterns = np.expand_dims(patternsIn, axis=0)
+        patterns = (np.expand_dims(patternsIn, axis=0)).copy()
       else:
-        patterns = patternsIn
+        patterns = (patternsIn).copy()
+
+      pscale = np.array([0.0, 1.0])
+
+      if patterns.dtype.kind =='f':
+        mxp = patterns.max()
+        mnp = patterns.min()
+        patterns -= mnp
+        patterns *= (2**16-2.0)/(mxp - mnp)
+        pscale[:] = np.array([mnp,(mxp - mnp) ])
+        patterns = patterns.astype(np.uint16)
+
 
       shape = patterns.shape
       nPats = shape[0]
 
       bandData = np.zeros((nPats,self.nBands),dtype=self.dataType)
       if chunksize < 0:
         nchunks = 1
@@ -87,29 +97,32 @@
       lmaxtime = 0.0
       blabeltime = 0.0
 
       for chnk in chunk_start_end:
         tic1 = timer()
         nPatsChunk = chnk[1] - chnk[0]
         #rdnNorm, clparams, rdnNorm_gpu = self.calc_rdn(patterns[chnk[0]:chnk[1],:,:], clparams, use_gpu=self.CLOps[0])
-        rdnNorm, clparams = self.radon_fasterCL(patterns[chnk[0]:chnk[1],:,:], self.padding,
+        rdnNorm, clparams = self.radon_fasterCL(patterns[chnk[0]:chnk[1],:,:], padding=self.padding,
                                                                        fixArtifacts=False, background=self.backgroundsub,
                                                                        returnBuff=True, clparams=clparams)
 
+        #rdnNorm, clparams = self.rdn_mask(rdnNorm, clparams=clparams, returnBuff=False)
+
         #if (self.EDAXIQ == True): # I think EDAX actually uses the convolved radon for IQ
           #nTp = self.nTheta + 2 * self.padding[1]
           #nRp = self.nRho + 2 * self.padding[0]
           #nImCL = int(rdnNorm_gpu.size/(nTp*nRp*4))
           #rdnNorm_nocov = np.zeros((nRp,nTp,nImCL),dtype=np.float32)
           #cl.enqueue_copy(clparams.queue,rdnNorm_nocov,rdnNorm,is_blocking=True)
 
         rdntime += timer() - tic1
         tic1 = timer()
-        rdnConv, clparams = self.rdn_convCL2(rdnNorm, clparams=clparams, returnBuff=True)
+        rdnConv, clparams = self.rdn_convCL2(rdnNorm, clparams=clparams, returnBuff=True, separableKernel=True)
         rdnNorm.release()
+
         convtime += timer()-tic1
         tic1 = timer()
         lMaxRdn, clparams =  self.rdn_local_maxCL(rdnConv, clparams=clparams, returnBuff=True)
         lmaxtime +=  timer()-tic1
         tic1 = timer()
 
         bandDataChunk = self.band_labelCL(rdnConv, lMaxRdn, clparams=clparams)
@@ -127,67 +140,84 @@
         #                                    use_gpu = self.CLOps[3], clparams=clparams )
 
         if (verbose > 1) and (chnk[1] == nPats): # need to pull the radonconv off the gpu
           nTp = self.nTheta + 2 * self.padding[1]
           nRp = self.nRho + 2 * self.padding[0]
           nImCL = int(rdnConv.size / (nTp * nRp * 4))
           rdnConvarray = np.zeros((nRp,nTp,nImCL),dtype=np.float32)
+
           cl.enqueue_copy(clparams.queue,rdnConvarray,rdnConv,is_blocking=True)
+
           rdnConvarray = rdnConvarray[:,:,0:chnk[1]-chnk[0] ]
+          #plt.imshow(rdnConvarray.squeeze())
 
         rdnConv.release()
+        rdnConv = None
+
         blabeltime += timer() - tic1
 
+      bandData['avemax'] *= pscale[1]
+      bandData['avemax'] += pscale[0]
+      bandData['max'] *= pscale[1]
+      bandData['max'] += pscale[0]
       tottime = timer() - tic0
       # going to manually clear the clparams queue -- this should clear the memory of the queue off the GPU
 
       #if clparams is not None:
-        #clparams.queue.finish()
-        #clparams.queue = None
+      #  clparams.queue.finish()
+      #  clparams.queue = None
 
       if verbose > 0:
         print('Radon Time:',rdntime)
         print('Convolution Time:', convtime)
         print('Peak ID Time:', lmaxtime)
         print('Band Label Time:', blabeltime)
         print('Total Band Find Time:',tottime)
       if verbose > 1:
-        plt.clf()
-
-        if len(rdnConvarray.shape) == 3:
-          im2show = rdnConvarray[self.padding[0]:-self.padding[0],self.padding[1]:-self.padding[1], -1]
-        else:
-          im2show = rdnConvarray[self.padding[0]:-self.padding[0],self.padding[1]:-self.padding[1]]
-
-        rhoMaskTrim = np.int32(im2show.shape[0] * self.rhoMaskFrac)
-        mean = np.mean(im2show[rhoMaskTrim:-rhoMaskTrim, 1:-2])
-        stdv = np.std(im2show[rhoMaskTrim:-rhoMaskTrim, 1:-2])
-        im2show -= mean
-        im2show /= stdv
-        im2show = im2show.clip(-4, None)
-        im2show += 6
-        im2show[0:rhoMaskTrim,:] = 0
-        im2show[-rhoMaskTrim:,:] = 0
-        im2show = np.fliplr(im2show)
-        plt.figure()
-        plt.imshow(im2show, cmap='gray', extent=[0, 180, -self.rhoMax, self.rhoMax],
-                   interpolation='none', zorder=1, aspect='auto')
-        width = bandData['width'][-1, :]
-        width /= width.min()
-        width *= 2
-        xplt = np.squeeze(180.0 - np.interp(bandData['aveloc'][-1,:,1], np.arange(self.radonPlan.nTheta), self.radonPlan.theta))
-        yplt = np.squeeze( -1.0 * np.interp(bandData['aveloc'][-1,:,0], np.arange(self.radonPlan.nRho), self.radonPlan.rho))
-
-        plt.scatter(y=yplt, x=xplt, c='r', s=width, zorder=2)
-
-        for pt in range(self.nBands):
-          plt.annotate(str(pt + 1),np.squeeze([xplt[pt],yplt[pt]]), color='yellow')
-        plt.xlim(0,180)
-        plt.ylim(-self.rhoMax, self.rhoMax)
-
+        self._display_radon_pattern(rdnConvarray, bandData, patterns)
+        # if len(rdnConvarray.shape) == 3:
+        #   im2show = rdnConvarray[self.padding[0]:-self.padding[0],self.padding[1]:-self.padding[1], -1]
+        # else:
+        #   im2show = rdnConvarray[self.padding[0]:-self.padding[0],self.padding[1]:-self.padding[1]]
+        #
+        # rhoMaskTrim = np.int32(im2show.shape[0] * self.rhoMaskFrac)
+        # mean = np.mean(im2show[rhoMaskTrim:-rhoMaskTrim, 1:-2])
+        # stdv = np.std(im2show[rhoMaskTrim:-rhoMaskTrim, 1:-2])
+        # im2show -= mean
+        # im2show /= stdv
+        # im2show = im2show.clip(-4, None)
+        # im2show += 6
+        # im2show[0:rhoMaskTrim,:] = 0
+        # im2show[-rhoMaskTrim:,:] = 0
+        #
+        # im2show = np.fliplr(im2show)
+        # fig = plt.figure(figsize=(12, 4))
+        # subrdn = fig.add_subplot(121, xlim=(0, 180), ylim=(-self.rhoMax, self.rhoMax))
+        # subrdn.imshow(
+        #     im2show,
+        #     cmap='gray',
+        #     extent=[0, 180, -self.rhoMax, self.rhoMax],
+        #     interpolation='none',
+        #     zorder=1,
+        #     aspect='auto'
+        # )
+        # width = bandData['width'][-1, :]
+        # width /= width.min()
+        # width *= 2.0
+        # xplt = np.squeeze(180.0 - np.interp(bandData['aveloc'][-1,:,1]+0.5, np.arange(self.radonPlan.nTheta), self.radonPlan.theta))
+        # yplt = np.squeeze( -1.0 * np.interp(bandData['aveloc'][-1,:,0]-0.5, np.arange(self.radonPlan.nRho), self.radonPlan.rho))
+        #
+        # subrdn.scatter(y=yplt, x=xplt, c='r', s=width, zorder=2)
+        #
+        # for pt in range(self.nBands):
+        #   subrdn.annotate(str(pt + 1), np.squeeze([xplt[pt] + 4, yplt[pt]]), color='yellow')
+        # #subrdn.xlim(0,180)
+        # #subrdn.ylim(-self.rhoMax, self.rhoMax)
+        # subpat = fig.add_subplot(122)
+        # subpat.imshow(patterns[-1, :, :], cmap='gray')
 
     except Exception as e: # something went wrong - try the CPU
       print(e)
       bandData = band_detect.BandDetect.find_bands(self, patternsIn, verbose=verbose, chunksize=-1, **kwargs)
 
     return bandData
 
@@ -221,75 +251,84 @@
       image = image.reshape(1, shapeIm[0], shapeIm[1])
       shapeIm = np.shape(image)
     else:
       nIm = shapeIm[0]
     #  reform = False
 
     clvtypesize = 16 # this is the vector size to be used in the openCL implementation.
-    nImCL = np.int32(clvtypesize * (np.int64(np.ceil(nIm/clvtypesize))))
-    # there is something very strange that happens if the number of images
-    # is a exact multiple of the max group size (typically 256)
-    mxGroupSz = gpu[gpu_id].get_info(cl.device_info.MAX_WORK_GROUP_SIZE)
-    #nImCL += np.int64(16 * (1 - np.int64(np.mod(nImCL, mxGroupSz ) > 0)))
-    image_align = np.ones((shapeIm[1], shapeIm[2], nImCL), dtype = np.float32)
-    image_align[:,:,0:nIm] = np.transpose(image, [1,2,0]).copy()
-    shpRdn = np.asarray( ((self.nRho+2*padding[0]), (self.nTheta+2*padding[1]), nImCL),dtype=np.uint64)
-    radon_gpu = cl.Buffer(ctx,mf.READ_WRITE,size=int((self.nRho+2*padding[0])*(self.nTheta+2*padding[1])*nImCL*4))
+    nImCL = np.uint64(clvtypesize * (np.int64(np.ceil(nIm/clvtypesize))))
+    imtype = image.dtype
+
+    tict = timer()
+    #image_align = np.ones((shapeIm[1], shapeIm[2], nImCL), dtype = imtype)
+    #image_align[:,:,0:nIm] = np.transpose(image, [1,2,0]).copy()
+    toct = timer()
+
+
+
     #radon_gpu = cl.Buffer(ctx,mf.READ_WRITE,size=radon.nbytes)
     #radon_gpu = cl.Buffer(ctx,mf.READ_WRITE | mf.COPY_HOST_PTR,hostbuf=radon)
-    image_gpu = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=image_align)
-    rdnIndx_gpu = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=self.radonPlan.indexPlan)
-
+    image_gpu = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=image)
     imstep = np.uint64(np.product(shapeIm[-2:]))
-    indxstep = np.uint64(self.radonPlan.indexPlan.shape[-1])
-    rdnstep = np.uint64(self.nRho * self.nTheta)
-
-    padRho = np.uint64(padding[0])
-    padTheta = np.uint64(padding[1])
     tic = timer()
 
     nImChunk = np.uint64(nImCL/clvtypesize)
+    image_gpuflt = cl.Buffer(ctx, mf.READ_WRITE, size=int(int(shapeIm[1])*int(shapeIm[2])*int(nImCL) * int(4)))  # 32-bit float
+
+
+    if image.dtype.type is np.float32:
+      prg.loadfloat32(queue, (shapeIm[2], shapeIm[1], nIm), None, image_gpu, image_gpuflt, nImCL)
+    if image.dtype.type is np.ubyte:
+      prg.loadubyte8(queue, (shapeIm[2], shapeIm[1], nIm), None, image_gpu, image_gpuflt, nImCL)
+    if image.dtype.type is np.uint16:
+      prg.loaduint16(queue, (shapeIm[2], shapeIm[1], nIm), None, image_gpu, image_gpuflt, nImCL)
+    queue.flush()
+    image_gpu.release()
+    image_gpu = None
+
+
 
     if background is not None:
       back_gpu = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=background.astype(np.float32))
-      prg.backSub(queue,(imstep, 1, 1),None,image_gpu,back_gpu,nImChunk)
-      imBack = np.zeros((shapeIm[1], shapeIm[2], nImCL),dtype=np.float32)
-      cl.enqueue_copy(queue,imBack,image_gpu,is_blocking=True)
-
+      prg.backSub(queue,(imstep, 1, 1),None,image_gpuflt,back_gpu,nImChunk)
+      #imBack = np.zeros((shapeIm[1], shapeIm[2], nImCL),dtype=np.float32)
+      #cl.enqueue_copy(queue,imBack,image_gpu,is_blocking=True)
 
-    prg.radonSum(queue,(nImChunk,rdnstep),None,rdnIndx_gpu,image_gpu,radon_gpu,
+    indxstep = np.uint64(self.radonPlan.indexPlan.shape[-1])
+    rdnstep = np.uint64(self.nRho * self.nTheta)
+    padRho = np.uint64(padding[0])
+    padTheta = np.uint64(padding[1])
+    shpRdn = np.asarray(((self.nRho + 2 * padding[0]), (self.nTheta + 2 * padding[1]), nImCL), dtype=np.uint64)
+    radon_gpu = cl.Buffer(ctx, mf.READ_WRITE,
+                          size=int((self.nRho + 2 * padding[0]) * (self.nTheta + 2 * padding[1]) * nImCL * 4))
+
+    rdnIndx_gpu = cl.Buffer(ctx, mf.READ_ONLY | mf.COPY_HOST_PTR, hostbuf=self.radonPlan.indexPlan)
+    cl.enqueue_fill_buffer(queue, radon_gpu, np.float32(self.radonPlan.missingval), 0, radon_gpu.size)
+    prg.radonSum(queue,(nImChunk,rdnstep),None,rdnIndx_gpu,image_gpuflt,radon_gpu,
                   imstep, indxstep,
                  shpRdn[0], shpRdn[1],
                  padRho, padTheta, np.uint64(self.nTheta))
 
 
     if (fixArtifacts == True):
-       prg.radonFixArt(queue,(nImChunk,self.nRho),None,radon_gpu,
+       prg.radonFixArt(queue,(nImChunk,shpRdn[0]),None,radon_gpu,
                        shpRdn[0],shpRdn[1],padTheta)
 
-
+    rdnIndx_gpu.release()
+    rdnIndx_gpu = None
 
 
     if returnBuff == False:
       radon = np.zeros([self.nRho + 2 * padding[0],self.nTheta + 2 * padding[1],nImCL],dtype=np.float32)
       cl.enqueue_copy(queue,radon,radon_gpu,is_blocking=True)
       radon_gpu.release()
       radon = radon[:,:, 0:nIm]
       radon_gpu = None
       #clparams = None
-      rdnIndx_gpu.release()
-      rdnIndx_gpu = None
-      image_gpu.release()
-      image_gpu = None
       return radon, clparams
-    else:
-      rdnIndx_gpu.release()
-      rdnIndx_gpu = None
-      image_gpu.release()
-      image_gpu = None
 
     return radon_gpu, clparams
 
 
 
   def rdn_convCL2(self, radonIn, clparams=None, separableKernel=True, returnBuff = True):
     # this will run (eventually sequential) convolutions and identify the peaks in the convolution
@@ -346,24 +385,40 @@
       rdn_gpu = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=radonCL)
       shp = (nRp, nTp, nImCL)
 
     nImChunk = np.uint64(nImCL / clvtypesize)
     resultConv = np.full(shp,0.0,dtype=np.float32)
 
     rdnConv_gpu = cl.Buffer(ctx,mf.WRITE_ONLY ,size=resultConv.nbytes)
-    # pad out the radon buffers
-    prg.radonPadTheta(queue,(shp[2],shp[0],1),None,rdn_gpu,
-                    np.uint64(shp[0]),np.uint64(shp[1]),np.uint64(self.padding[1]))
-    prg.radonPadRho(queue,(shp[2],shp[1],1),None,rdn_gpu,
-                      np.uint64(shp[0]),np.uint64(shp[1]),np.uint64(self.padding[0]))
+
+    # maskrnd = np.zeros((self.nRho + 2 * self.padding[0], self.nTheta + 2 * self.padding[1]), dtype=np.ubyte)
+    # maskrnd[self.padding[0]:-self.padding[0], self.padding[1]:-self.padding[1]] = self.rhomask1
+    #
+    # maskrnd = maskrnd.astype(np.ubyte)
+    # maskrnd_gpu = cl.Buffer(ctx, mf.READ_ONLY | mf.COPY_HOST_PTR, hostbuf=maskrnd)
+    #
+    # prg.maskrdn(queue, (np.uint32(nT), np.uint32(nR)), None, rdn_gpu, maskrnd_gpu,
+    #             np.uint64(shp[1]), np.uint64(nImChunk),
+    #             np.uint64(self.padding[1]), np.uint64(self.padding[0]))
+
+    # # pad out the radon buffers
+    # prg.radonPadTheta(queue,(shp[2],shp[0],1),None,rdn_gpu,
+    #                 np.uint64(shp[0]),np.uint64(shp[1]),np.uint64(self.padding[1]))
+
+    #prg.radonPadRho2(queue,(shp[2],shp[1],1),None,rdn_gpu,
+    #                  np.uint64(shp[0]),np.uint64(shp[1]),np.uint64(self.padding[0]+1))
+
+    prg.radonPadRho2(queue, (shp[2], shp[1], 1), None, rdn_gpu,
+                 np.uint64(shp[0]),np.uint64(shp[1]),np.uint64(shp[0]//2-1))
+
     kern_gpu = None
     if separableKernel == False:
       # for now I will assume that the kernel(s) can fit in local memory on the GPU
       # also going to assume that there is only one kernel -- this will be something to fix at some point.
-      k0 = self.kernel[0,:,:]
+      k0 = np.array(self.kernel[0,:,:], dtype=np.float32)
       kshp = np.asarray(k0.shape, dtype=np.int32)
       pad = kshp/2
       kern_gpu = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=k0)
       prg.convolution3d2d(queue,(np.int32((shp[1]-2*pad[1])),np.int32((shp[0]-2*pad[0])), nImChunk),None,
                         rdn_gpu, kern_gpu,np.int32(shp[1]),np.int32(shp[0]),np.int32(shp[2]),
                         np.int32(kshp[1]), np.int32(kshp[0]), np.int32(pad[1]), np.int32(pad[0]), rdnConv_gpu)
 
@@ -371,29 +426,29 @@
 
       #tic = timer()
     else: # convolution is separable
       tempConvbuff = cl.Buffer(ctx,mf.HOST_NO_ACCESS,size=(shp[0]*shp[1]*shp[2]*4))
 
       kshp = np.asarray(self.kernel[0,:,:].shape,dtype=np.int32)
       pad = kshp
-      k0x = np.require(self.kernel[0, np.int64(kshp[0] / 2), :], requirements=['C', 'A', 'W', 'O'])
+      k0x = np.require(self.kernel[0, np.int64(kshp[0] / 2), :], requirements=['C', 'A', 'W', 'O'], dtype=np.float32)
       k0x *= 1.0 / k0x.sum()
       k0x = (k0x[...,:]).reshape(1,kshp[1])
 
 
 
       kshp = np.asarray(k0x.shape,dtype=np.int32)
 
       kern_gpu_x = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=k0x)
       prg.convolution3d2d(queue,(np.int32((shp[1]-2*pad[1])),np.int32((shp[0]-2*pad[0])), nImChunk),None,
                           rdn_gpu,kern_gpu_x,np.int32(shp[1]),np.int32(shp[0]),np.int32(shp[2]),
                           np.int32(kshp[1]),np.int32(kshp[0]),np.int32(pad[1]),np.int32(pad[0]),tempConvbuff)
 
       kshp = np.asarray(self.kernel[0,:,:].shape,dtype=np.int32)
-      k0y = np.require(self.kernel[0, :, np.int32(kshp[1] / 2)], requirements=['C', 'A', 'W', 'O'])
+      k0y = np.require(self.kernel[0, :, np.int32(kshp[1] / 2)], requirements=['C', 'A', 'W', 'O'], dtype=np.float32)
       k0y *= 1.0 / k0y.sum()
       k0y = (k0y[...,:]).reshape(kshp[0],1)
       kshp = np.asarray(k0y.shape,dtype=np.int32)
 
       kern_gpu_y = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=k0y)
       prg.convolution3d2d(queue,(np.int32((shp[1]-2*pad[1])),np.int32((shp[0]-2*pad[0])), nImChunk),None,
                           tempConvbuff,kern_gpu_y,np.int32(shp[1]),np.int32(shp[0]),np.int32(shp[0]),
@@ -429,15 +484,15 @@
       rdnConv_gpu = None
       return resultConv, clparams
     else:
       return rdnConv_gpu, clparams
 
 
 
-  def rdn_local_maxCL(self,radonIn,clparams=None,  returnBuff = True):
+  def rdn_local_maxCL(self,radonIn, clparams=None,  returnBuff = True):
     # this will run a morphological max kernel over the convolved radon array
     # the local max identifies the location of the peak max within
     # the window size.
 
     tic = timer()
     clvtypesize = 16  # this is the vector size to be used in the openCL implementation.
 
@@ -481,20 +536,21 @@
         radon = radonIn
       shp = radon.shape
       nIm = shp[2]
       nImCL = np.int32(clvtypesize * (np.int64(np.ceil(nIm / clvtypesize))))
       # there is something very strange that happens if the number of images
       # is a exact multiple of the max group size (typically 256)
       mxGroupSz = gpu[gpu_id].get_info(cl.device_info.MAX_WORK_GROUP_SIZE)
-      nImCL += np.int(16 * (1 - np.int(np.mod(nImCL,mxGroupSz) > 0)))
+      nImCL += np.int64(16 * (1 - np.int64(np.mod(nImCL,mxGroupSz) > 0)))
       radonCL = np.zeros((nRp,nTp,nImCL),dtype=np.float32)
       radonCL[:,:,0:shp[2]] = radon
       rdn_gpu = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=radonCL)
       shp = (nRp,nTp,nImCL)
 
+
     nImChunk = np.uint64(nImCL / clvtypesize)
     #out = np.zeros((shp), dtype = np.int32)
 
     lmaxX = cl.Buffer(ctx, mf.READ_WRITE, size=rdn_gpu.size)
     lmaxXY = cl.Buffer(ctx, mf.READ_WRITE, size=rdn_gpu.size)
 
 
@@ -511,32 +567,42 @@
     #                         np.int64(self.padding[1]),np.int64(self.padding[0]),
     #                         np.int64(1),np.int64(self.peakPad[0]))
     #
     # prg.morphDilateKernelBF(queue,(np.uint32(nT),np.uint32(nR),nImChunk),None,lmaxX,lmaxXY,
     #                         np.int64(shp[1]),np.int64(shp[0]),
     #                         np.int64(self.padding[1]),np.int64(self.padding[0]),
     #                         np.int64(self.peakPad[1]),np.int64(1))
-
+    # calculate the max in the x direction
     prg.morphDilateKernelBF(queue, (np.uint32(shp[1]), np.uint32(nR), nImChunk), None, rdn_gpu, lmaxX,
                             np.int64(shp[1]), np.int64(shp[0]),
                             np.int64(0), np.int64(self.padding[0]),
                             np.int64(self.peakPad[1]), np.int64(1))
-
+    # take the max in the x output, use as input, and calculate in the y direction
     prg.morphDilateKernelBF(queue, (np.uint32(nT), np.uint32(nR), nImChunk), None, lmaxX, lmaxXY,
                             np.int64(shp[1]), np.int64(shp[0]),
                             np.int64(self.padding[1]), np.int64(self.padding[0]),
                             np.int64(1), np.int64(self.peakPad[0]))
 
     local_max = np.zeros((shp),dtype=np.ubyte)
     local_max_gpu = cl.Buffer(ctx,mf.WRITE_ONLY,size=local_max.nbytes)
 
     prg.im1EQim2(queue,(np.uint32(nT),np.uint32(nR),nImCL),None, lmaxXY, rdn_gpu, local_max_gpu,
                  np.uint64(shp[1]),np.uint64(shp[0]),
                  np.uint64(self.padding[1]),np.uint64(self.padding[0]))
 
+    maskrnd = np.zeros((self.nRho + 2 * self.padding[0] , self.nTheta + 2 * self.padding[1]), dtype=np.ubyte)
+    maskrnd[self.padding[0]:-self.padding[0], self.padding[1]:-self.padding[1]] = self.rdnmask.astype(np.ubyte)
+
+    maskrnd = maskrnd.astype(np.ubyte)
+    maskrnd_gpu = cl.Buffer(ctx, mf.READ_ONLY | mf.COPY_HOST_PTR, hostbuf=maskrnd)
+
+    prg.maxmask(queue, (np.uint32(nT), np.uint32(nR)), None, local_max_gpu, maskrnd_gpu,
+                 np.uint64(shp[1]), np.uint64(nImChunk),
+                 np.uint64(self.padding[1]), np.uint64(self.padding[0]))
+
     queue.flush()
 
 
     if returnBuff == False:
       local_maxX = np.zeros((shp), dtype=np.float32)
       local_maxXY = np.zeros((shp), dtype=np.float32)
       cl.enqueue_copy(queue,local_max,local_max_gpu,is_blocking=True)
@@ -558,15 +624,15 @@
       lmaxX.release()
       lmaxXY.release()
       return local_max_gpu, clparams
 
 
   def band_labelCL(self,rdnConvIn, lMaxRdnIn,clparams=None):
 
-    # an attempt to to run the band label on the GPU
+    # an attempt to run the band label on the GPU
 
     tic = timer()
 
 
     if clparams is not None:
       if clparams.queue is None:
         clparams.get_queue()
@@ -633,25 +699,26 @@
     maxloc_gpu = cl.Buffer(ctx,mf.WRITE_ONLY,size=maxloc.nbytes)
     aveval = np.zeros((nIm,self.nBands),dtype=np.float32) - 2.0e6
     aveval_gpu = cl.Buffer(ctx,mf.WRITE_ONLY,size=aveval.nbytes)
     width = np.zeros((nIm, self.nBands), dtype=np.float32)
     width_gpu = cl.Buffer(ctx, mf.WRITE_ONLY, size=width.nbytes)
     aveloc = np.zeros((nIm,self.nBands,2),dtype=np.float32)
     aveloc_gpu = cl.Buffer(ctx,mf.WRITE_ONLY,size=aveloc.nbytes)
-    rhoMaskTrim = np.int64((shp[0] - 2 * self.padding[0]) * self.rhoMaskFrac + self.padding[0])
-
+    #rhoMaskTrim = np.int64((shp[0] - 2 * self.padding[0]) * self.rhoMaskFrac + self.padding[0])
+    rhoMaskTrim = np.int64(self.padding[0])
 
     prg.maxlabel(queue,(nIm, 1,1),(1,1,1),
                  lMaxRdn_gpu,rdnConv_gpu,
                  maxloc_gpu, maxval_gpu,
                  aveloc_gpu,aveval_gpu,
                  width_gpu,
                  np.int64(shp[1]),np.int64(shp[0]),
                  np.int64(self.padding[1]),rhoMaskTrim,np.int64(self.nBands) )
 
+
     queue.finish()
     cl.enqueue_copy(queue,maxval,maxval_gpu,is_blocking=False)
     cl.enqueue_copy(queue,maxloc,maxloc_gpu,is_blocking=False)
     cl.enqueue_copy(queue,aveval,aveval_gpu,is_blocking=False)
     cl.enqueue_copy(queue,aveloc,aveloc_gpu,is_blocking=False)
     cl.enqueue_copy(queue, width, width_gpu, is_blocking=True)
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/opencl/clkernels.cl` & `pyebsdindex-0.3.0/pyebsdindex/opencl/clkernels.cl`

 * *Files 15% similar despite different names*

```diff
@@ -18,14 +18,81 @@
 works bear some notice that they are derived from it, and any modified versions bear
 some notice that they have been modified.
 
 Author: David Rowenhorst; 
 The US Naval Research Laboratory Date: 21 Aug 2020
 */
 
+// simple program to convert a 8-bit byte to float and transpose array
+__kernel void loadubyte8( const __global uchar *im1, __global float *im1flt, const unsigned long int nImCL)
+  {
+  const unsigned long int x = get_global_id(0);
+  const unsigned long int y = get_global_id(1);
+  const unsigned long int z = get_global_id(2);
+  const unsigned long int nx = get_global_size(0);
+  const unsigned long int ny = get_global_size(1);
+  //const unsigned long int nz = get_global_size(2);
+  
+  const unsigned long int indx1 = x + nx*y + nx*ny*z;
+  const unsigned long int indx2 = z + nImCL*(x + nx*y); // transpose z->x, x->y, y->z 
+  uchar imVal;
+  float imValflt;
+
+  imVal =  im1[indx1];
+  imValflt = convert_float(imVal);
+  im1flt[indx2] = imValflt;
+  
+  
+}
+
+
+// simple program to convert a 8-bit byte to float and transpose array
+__kernel void loaduint16( const __global ushort *im1, __global float *im1flt, const unsigned long int nImCL)
+  {
+  const unsigned long int x = get_global_id(0);
+  const unsigned long int y = get_global_id(1);
+  const unsigned long int z = get_global_id(2);
+  const unsigned long int nx = get_global_size(0);
+  const unsigned long int ny = get_global_size(1);
+  //const unsigned long int nz = get_global_size(2);
+  
+  const unsigned long int indx1 = x + nx*y + nx*ny*z;
+  const unsigned long int indx2 = z + nImCL*(x + nx*y); // transpose z->x, x->y, y->z 
+  ushort imVal;
+  float imValflt;
+
+  imVal =  im1[indx1];
+  imValflt = convert_float(imVal);
+  im1flt[indx2] = imValflt;
+  
+  
+}
+
+
+
+// simple program to convert a float to float and transpose array
+__kernel void loaduufloat32( const __global float *im1, __global float *im1flt, const unsigned long int nImCL)
+  {
+  const unsigned long int x = get_global_id(0);
+  const unsigned long int y = get_global_id(1);
+  const unsigned long int z = get_global_id(2);
+  const unsigned long int nx = get_global_size(0);
+  const unsigned long int ny = get_global_size(1);
+  //const unsigned long int nz = get_global_size(2);
+  
+  const unsigned long int indx1 = x + nx*y + nx*ny*z;
+  const unsigned long int indx2 = z + nImCL*(x + nx*y); // transpose z->x, x->y, y->z 
+  float imVal;
+
+  imVal =  im1[indx1];
+  im1flt[indx2] = imVal;
+  
+  
+}
+
 
 //Do a background subtract on the pattern
 __kernel void backSub( __global float16 *im1, __global const float *back,
                         const unsigned long int nImChunk)
   {
   const unsigned long int xy = get_global_id(0);
   //const unsigned long int szim = get_global_size(0);
@@ -39,14 +106,37 @@
     imVal =  im1[indx+i];
     imVal -= b1;   
     im1[indx+i] = imVal;
   }
   
 }
 
+//Do a background division on the pattern
+__kernel void backDiv( __global float16 *im1, __global const float *back,
+                        const unsigned long int nImChunk)
+  {
+  const unsigned long int xy = get_global_id(0);
+  //const unsigned long int szim = get_global_size(0);
+  unsigned long i;
+  float16 imVal;
+
+  float b1 = back[xy];
+  if (b1 < 1.0){
+    b1 = 1.0;
+  }
+  
+  const unsigned long indx = nImChunk * xy;
+  for(i = 0; i< nImChunk; ++i){
+    imVal =  im1[indx+i];
+    imVal /= b1;   
+    im1[indx+i] = imVal;
+  }
+  
+}
+
 
 __kernel void radonSum(
       __global const unsigned long int *rdnIndx, __global const float16 *images, __global float16 *radon,
       const unsigned long int imstep, const unsigned long int indxstep,
       const unsigned int long nRhoP, const unsigned long int nThetaP,
       const unsigned long int rhoPad, const unsigned long int thetaPad,const unsigned long int nTheta )
     {
@@ -70,35 +160,65 @@
         sum += images[idx*nImChunk + gid_im];
         count += 1.0;
       }
     }
 
 
     const unsigned long int rndIndx = (theta+thetaPad + (rho+rhoPad)*nThetaP)*nImChunk + gid_im;
-    radon[rndIndx] = sum/count;
-    //radon[rndIndx] = gid_im;
+    if (count > 1.0e-6){
+      radon[rndIndx] = sum/count;}
+    else{
+      radon[rndIndx] = -1.0;
+    }
+    
     }
 
-  __kernel void radonFixArt(
+__kernel void radonFixArt(
       __global float16 *radon,
       const unsigned long int nRho, const unsigned long int nTheta,
       const unsigned long int thetaPad)
   {
     const unsigned long int gid_im = get_global_id(0);
     const unsigned long int nImChunk = get_global_size(0);
     const unsigned long int rho = get_global_id(1);
     const unsigned long int rhoIndx = nTheta * rho;
     //rndIndx = nTheta * nRho * gid_im + (nTheta * rho);
-
-    //radon[gid_rdn+thetaPad] = radon[gid_rdn+thetaPad+1];
+    
     radon[(thetaPad + rhoIndx)*nImChunk + gid_im] = radon[(thetaPad + 1 + rhoIndx)*nImChunk + gid_im];
-    //radon[gid_rdn+nTheta-1-thetaPad] = radon[gid_rdn+nTheta-2-thetaPad];
+   
     radon[(nTheta-1-thetaPad + rhoIndx)*nImChunk + gid_im] = radon[(+nTheta-2-thetaPad + rhoIndx)*nImChunk + gid_im];
+    //}
   }
 
+
+// // Makes a mask based on if the Radon has missing values -- returns byte array.
+// // There is NOT ability to include padding in x and y ... yet.  
+// __kernel void maskrdn( __global const float *im1, __global uchar *out, const float misval)
+// {
+//   // IDs of work-item represent x and y coordinates in image
+//   //const unsigned long int x = get_global_id(0)+padx;
+//   //const unsigned long int y = get_global_id(1)+pady;
+//   const unsigned long x = get_global_id(0);
+//   const unsigned long int imszx = get_global_size(0);
+//   const unsigned long y = get_global_id(1);
+//   const unsigned long int z = get_global_id(2);
+//   const unsigned long int nImChunk = get_global_size(2);
+//   //const int16 yes = (int16)(1);
+//   //const int16 no = (int16)(0);
+
+//   const unsigned long int indx = (x + imszx*y)*nImChunk + z;
+//   const float im1val = im1[indx];
+  
+//   const float diff = fabs(im1val - misval);
+//   //out[indx] = (diff < 1.0e-6f) ? yes: no;
+//   out[indx] = (diff < 1.0e-5f) ? 0: 1;
+// }
+
+
+
 // Padding of the radon Theta -- 0 and 180* are symmetric with a vertical flip.
 __kernel void radonPadTheta(
       __global float *radon,
       const unsigned long int nRho, const unsigned long int nTheta,
       const unsigned long int thetaPad)
   {
     const unsigned long int gid_im = get_global_id(0);
@@ -139,14 +259,59 @@
         gid_rdn2 = ((nTheta* (nRho-1-rhoPad+i)) + gid_theta)*nImChunk + gid_im;
         radon[gid_rdn1] = rd1p;
         radon[gid_rdn2] = rd2p;
     }
 
   }
 
+
+  // Padding of the radon Rho -- copy the previous line to the next row ...
+  __kernel void radonPadRho2(
+      __global float *radon,
+      const unsigned long int nRho, const unsigned long int nTheta,
+      const unsigned long int rhoPad)
+  {
+    const unsigned long int z = get_global_id(0);
+    const unsigned long int nImChunk = get_global_size(0);
+    const unsigned long int gid_theta = get_global_id(1);
+    unsigned long int i, gid_rdn1, gid_rdn2;
+    //indxim = nTheta * nRho * z;
+    //rd1p =  radon[indxim + (nTheta * rhoPad) + gid_theta] ;
+    //rd2p =  radon[ indxim + (nTheta * (nRho -1 - rhoPad)) + gid_theta] ;
+    
+    gid_rdn1 = ((nTheta*rhoPad) + gid_theta)*nImChunk + z;
+    gid_rdn2 = ((nTheta* (nRho-1-rhoPad)) + gid_theta)*nImChunk + z;
+
+    float rd1p =  radon[gid_rdn1];
+    float rd2p =  radon[gid_rdn2];
+    
+
+    for (i = 0; i <= rhoPad; ++i){
+
+        //gid_rdn1 = indxim + (nTheta*i) + gid_theta;
+        //gid_rdn2 = indxim + (nTheta* (nRho-1-rhoPad+i)) + gid_theta;
+        
+        gid_rdn1 = ( (nTheta* (rhoPad - i)) + gid_theta)*nImChunk + z;
+        gid_rdn2 = ((nTheta* (nRho-1-rhoPad+i)) + gid_theta)*nImChunk + z;
+        
+        if (radon[gid_rdn1] < 0){
+          radon[gid_rdn1] = rd1p;
+        }
+
+        if (radon[gid_rdn2] < 0){
+          radon[gid_rdn2] = rd2p;
+        }
+        rd1p =  radon[gid_rdn1] ;
+        rd2p =  radon[gid_rdn2] ;
+
+    }
+
+  }
+
+
 // Convolution of a stack of images by a 2D kernel
 // At somepoint we might want to consider the ability to chain together convolutions -- keeping the max at each pixel...
 __kernel void convolution3d2d( __global const float16 *in, __constant float *kern, const int imszx, const int imszy, const int imszz, 
   const int kszx, const int kszy, const int padx, const int pady, __global float16 *out)
 {
   // IDs of work-item represent x and y coordinates in image
   const long x = get_global_id(0) + padx;
@@ -304,14 +469,72 @@
   const float diff = fabs(im1val - im2val);
   //out[indx] = (diff < 1.0e-6f) ? yes: no;
   out[indx] = (diff < 1.0e-5f) ? 1: 0;
   
   
 }
 
+// Is image1 (can be a stack of images) EQ to image2 (can be a stack) -- returns byte array.
+// There is ability to include padding in x and y
+__kernel void maskrdn( __global float16 *im1, __global const uchar *mask,
+                        const unsigned long imszx, const unsigned long nImChunk,
+                        const unsigned long padx, const unsigned long pady)
+{
+  // IDs of work-item represent x and y coordinates in image
+  //const unsigned long int x = get_global_id(0)+padx;
+  //const unsigned long int y = get_global_id(1)+pady;
+  const unsigned long x = get_global_id(0) + padx;
+  const unsigned long y = get_global_id(1) + pady;
+  unsigned long int indx_z,i;
+  
+
+  //const unsigned long int indx = (x + imszx*y)*nImChunk + z;
+  const unsigned long int indx = (x + imszx*y);
+  const uchar test = mask[indx];
+  if (test < 1){
+    for (i=0; i<nImChunk; ++i){
+      indx_z = indx*nImChunk + i;
+      im1[indx_z] = -1.0;
+    }
+    
+  }
+  
+  
+}
+
+
+// Is image1 (can be a stack of images) EQ to image2 (can be a stack) -- returns byte array.
+// There is ability to include padding in x and y
+__kernel void maxmask( __global uchar16 *im1, __global const uchar *mask,
+                        const unsigned long imszx, const unsigned long imszz, 
+                        const unsigned long padx, const unsigned long pady)
+{
+  // IDs of work-item represent x and y coordinates in image
+  //const unsigned long int x = get_global_id(0)+padx;
+  //const unsigned long int y = get_global_id(1)+pady;
+  const unsigned long x = get_global_id(0) + padx;
+  const unsigned long y = get_global_id(1) + pady;
+  unsigned long int indx_z,i;
+  
+
+  //const unsigned long int indx = (x + imszx*y)*nImChunk + z;
+  const unsigned long int indx = (x + imszx*y);
+  const uchar test = mask[indx];
+  if (test < 1){
+    for (i=0; i<imszz; ++i){
+      indx_z = indx*imszz + i;
+      im1[indx_z] = 0;
+    }
+    
+  }
+  
+  
+}
+
+
 //this is a dirty little sort for getting the max locations ordered.  Will order accending.  
 // Keeping only the top nmax points.  Need to have maxval1d primed so that maxval1d[nmax] is larger 
 // than anything that will occur on its own.  
 void dirtsort( __global float *maxval1d, __global long int *maxloc1d,
                 long int newloc, float newmax, unsigned long nmax);
 
 void dirtsort( __global float *maxval1d, __global long int *maxloc1d,
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/opencl/radon_fast_cl.py` & `pyebsdindex-0.3.0/pyebsdindex/opencl/radon_fast_cl.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,17 @@
     if clparams is None:
       self.clparams = openclparam.OpenClParam()
       self.clparams.get_queue()
     else:
       self.clparams = clparams
 
 
-  def radon_fasterCL(self,image,padding = np.array([0,0]), fixArtifacts = False, background = None, returnBuff = True, clparams=None ):
+  def radon_fasterCL(self,image,padding = np.array([0,0]), fixArtifacts = False,
+                     background = None, background_method = 'SUBTRACT',
+                     returnBuff = True, clparams=None ):
 
     tic = timer()
     # make sure we have an OpenCL environment
     if clparams is not None:
       if clparams.queue is None:
         clparams.get_queue()
       gpu = clparams.gpu
@@ -104,27 +106,30 @@
     padTheta = np.uint64(padding[1])
     tic = timer()
 
     nImChunk = np.uint64(nImCL/clvtypesize)
 
     if background is not None:
       back_gpu = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=background.astype(np.float32))
-      prg.backSub(queue,(imstep, 1, 1),None,image_gpu,back_gpu,nImChunk)
-      imBack = np.zeros((shapeIm[1], shapeIm[2], nImCL),dtype=np.float32)
-      cl.enqueue_copy(queue,imBack,image_gpu,is_blocking=True)
-
+      if str.upper(background_method) == 'DIVIDE':
+        prg.backDiv(queue,(imstep, 1, 1),None,image_gpu,back_gpu,nImChunk)
+      else:
+        prg.backSub(queue,(imstep, 1, 1),None,image_gpu,back_gpu,nImChunk)
+        #imBack = np.zeros((shapeIm[1], shapeIm[2], nImCL),dtype=np.float32)
+        #cl.enqueue_copy(queue,imBack,image_gpu,is_blocking=True)
 
+    cl.enqueue_fill_buffer(queue, radon_gpu, np.float32(self.missingval), 0, radon_gpu.size)
     prg.radonSum(queue,(nImChunk,rdnstep),None,rdnIndx_gpu,image_gpu,radon_gpu,
                   imstep, indxstep,
                  shpRdn[0], shpRdn[1],
                  padRho, padTheta, np.uint64(self.nTheta))
 
 
     if (fixArtifacts == True):
-       prg.radonFixArt(queue,(nImChunk,self.nRho),None,radon_gpu,
+       prg.radonFixArt(queue,(nImChunk,shpRdn[0]),None,radon_gpu,
                        shpRdn[0],shpRdn[1],padTheta)
 
 
 
 
     if returnBuff == False:
       radon = np.zeros([self.nRho + 2 * padding[0],self.nTheta + 2 * padding[1],nImCL],dtype=np.float32)
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/pairlib.py` & `pyebsdindex-0.3.0/pyebsdindex/pairlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     #libANG, libID = self.sortlib_id(libANG,libID,findDups = True)
     #print(libANG)
     #print(libANG.shape)
     angTable = self.calc_pole_dot(sympolesComplete,sympolesComplete)
     angTable = np.arccos(angTable)*RADEG
     famindx0 = ((np.concatenate( ([0],np.cumsum(nFamComplete)) ))[0:-1]).astype(dtype=np.int)
     cartPoles = self.xstalplane2cart(sympolesComplete)
-    cartPoles /= np.linalg.norm(cartPoles, axis = 1).reshape(np.int(cartPoles.size/3),1)
+    cartPoles /= np.linalg.norm(cartPoles, axis = 1).reshape(int(cartPoles.size/3),1)
     self.completelib = {
                    'poles' : sympolesComplete,
                    'polesCart': cartPoles,
                    'angTable' : angTable,
                    'nFamily'  : nFamComplete,
                    'famIndex' : famindx0
                   }
@@ -208,16 +208,16 @@
       testSum = np.sum( (test < -0.99999).astype(np.int32)*np.arange(nf).reshape(1,nf), axis = 1)
       whpos = np.nonzero( np.logical_or(testSum < np.arange(nf), (testSum == 0)))[0]
       polesout = polesout[whpos, :]
     return polesout
 
   def calc_pole_dot(self,poles1,poles2,rMetricTensor = np.identity(3)):
 
-    p1 = poles1.reshape(np.int(poles1.size / 3), 3)
-    p2 = poles2.reshape(np.int(poles2.size / 3), 3)
+    p1 = poles1.reshape(int(poles1.size // 3), 3)
+    p2 = poles2.reshape(int(poles2.size // 3), 3)
 
     n1 = p1.shape[0]
     n2 = p2.shape[0]
 
     t1 = p1.dot(rMetricTensor)
     t2 = rMetricTensor.dot(p2.T)
     dot = t1.dot(p2.T)
@@ -239,15 +239,15 @@
     LUTA = np.array([[0,1,2],[0,2,1],[1,0,2],[1,2,0],[2,0,1],[2,1,0]])
     LUTB = np.array([[0,1,2],[1,0,2],[0,2,1],[2,0,1],[1,2,0],[2,1,0]])
 
     LUT = np.zeros((3,3,3,3), dtype=np.int64)
     for i in range(6):
       LUT[:, LUTA[i,0], LUTA[i,1], LUTA[i,2]] = LUTB[i,:]
 
-    ntrips = np.int(libANG.size / 3)
+    ntrips = int(libANG.size // 3)
     for i in range(ntrips):
       temp = np.squeeze(libANG[i,:])
       srt = np.argsort(temp)
       libANG[i,:] = temp[srt]
       srt2 = LUT[:,srt[0], srt[1], srt[2]]
       temp2 = libID[i,:]
       temp2 = temp2[srt2]
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/radon_fast.py` & `pyebsdindex-0.3.0/pyebsdindex/radon_fast.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,55 +16,72 @@
 This software can be redistributed and/or modified freely provided that any derivative
 works bear some notice that they are derived from it, and any modified versions bear
 some notice that they have been modified.
 
 Author: David Rowenhorst;
 The US Naval Research Laboratory Date: 21 Aug 2020"""
 
-from os import environ
+#from os import environ
+import os
+from pathlib import PurePath, Path
 from timeit import default_timer as timer
 
 from numba import jit, prange
 import numpy as np
 
+tempdir = PurePath(Path.home())
+#tempdir = PurePath("/tmp" if platform.system() == "Darwin" else tempfile.gettempdir())
+tempdir = tempdir.joinpath('.pyebsdindex').joinpath('numbacache')
+#tempdir = tempdir.joinpath('numbacache')
+Path(tempdir).mkdir(parents=True, exist_ok=True)
+os.environ["NUMBA_CACHE_DIR"] = str(tempdir)+str(os.sep)
+
 RADEG = 180.0/np.pi
 DEGRAD = np.pi/180.0
 
 
 
 class Radon:
-  def __init__(self, image=None, imageDim=None, nTheta=180, nRho=90, rhoMax=None):
+  def __init__(self, image=None, imageDim=None, nTheta=180, nRho=90, rhoMax=None,
+               mask=None, maskindex = None, missingval = -1.0):
     self.nTheta = nTheta
     self.nRho = nRho
     self.rhoMax = rhoMax
-    self.indexPlan = None
+    self.mask = mask
+    self.maskindex = maskindex
+    self.missingval = missingval
     if (image is None) and (imageDim is None):
       self.theta = None
       self.rho = None
       self.imDim = None
     else:
       if image is not None:
         self.imDim = np.asarray(image.shape[-2:])
       else:
         self.imDim = np.asarray(imageDim[-2:])
-      self.radon_plan_setup(imageDim=self.imDim, nTheta=self.nTheta, nRho=self.nRho, rhoMax=self.rhoMax)
+      self.masksetup()
+      #self.radon_plan_setup(imageDim=self.imDim, nTheta=self.nTheta, nRho=self.nRho, rhoMax=self.rhoMax)
 
   def radon_plan_setup(self, image=None, imageDim=None, nTheta=None, nRho=None, rhoMax=None):
     if (image is None) and (imageDim is not None):
-      imDim = np.asarray(imageDim, dtype=np.int64)
+      self.imDim = np.asarray(imageDim, dtype=np.int64)
     elif (image is not None):
-      imDim =  np.shape(image)[-2:] # this will catch if someone sends in a [1 x N x M] image
-    else:
+      self.imDim =  np.asarray(np.shape(image)[-2:]) # this will catch if someone sends in a [1 x N x M] image
+
+    if self.imDim is None:
       return -1
-    imDim = np.asarray(imDim)
-    self.imDim = imDim
+    imDim = self.imDim
+
+
+
     if (nTheta is not None) : self.nTheta = nTheta
     if (nRho is not None): self.nRho = nRho
     #self.rhoMax = rhoMax if (rhoMax is not None) else np.round(np.linalg.norm(imDim)*0.5)
-    self.rhoMax = rhoMax if (rhoMax is not None) else (np.linalg.norm(imDim) * 0.5)
+    if (rhoMax is not None): self.rhoMax = rhoMax
+    if (self.rhoMax is None): self.rhoMax = (np.linalg.norm(imDim) * 0.5)
 
     deltaRho = float(2 * self.rhoMax) / (self.nRho)
     self.theta = np.arange(self.nTheta, dtype = np.float32)*180.0/self.nTheta
     self.rho = np.arange(self.nRho, dtype = np.float32)*deltaRho - (self.rhoMax-deltaRho)
 
     xmin = -1.0*(self.imDim[1]-1)*0.5
     ymin = -1.0*(self.imDim[0]-1)*0.5
@@ -93,107 +110,172 @@
         b1 = b1.reshape(self.nRho, 1)
         #indx_y = np.floor(a[i]*m+b1).astype(np.int64)
         indx_y = np.round(a[i] * m + b1).astype(np.int64)
         indx_y = np.where(indx_y < 0, outofbounds, indx_y)
         indx_y = np.where(indx_y >= self.imDim[0], outofbounds, indx_y)
         #indx_y = np.clip(indx_y, 0, self.imDim[1])
         indx1D = np.clip(m+self.imDim[1]*indx_y, 0, outofbounds)
+        # for j in range(self.nRho):
+        #   indx_good = indx1D[j,:].flatten()
+        #   whgood = np.nonzero(indx_good < outofbounds)[0]
+        #   if whgood.size > 0:
+        #     maskval = self.mask.flatten()[indx_good[whgood]]
+        #     newindex = self.maskindex.flatten()[indx_good[whgood]]
+        #
+        #     whmask = np.nonzero((maskval > 0) & (newindex >= 0))[0]
+        #     indx1D[j,:] = outofbounds
+        #     if (whmask.size > 0):
+        #       indx1D[j, 0:whmask.size] = newindex[whmask]
         self.indexPlan[:,i, 0:self.imDim[1]] = indx1D
       else:
         b1 /= cTheta[i]
         b1 = b1.reshape(self.nRho, 1)
         #if cTheta[i] > 0:
           #indx_x = np.floor(a[i]*n + b1).astype(np.int64)
         #else:
           #indx_x = np.ceil(a[i] * n + b1).astype(np.int64)
         indx_x = np.round(a[i] * n + b1).astype(np.int64)
         indx_x = np.where(indx_x < 0, outofbounds, indx_x)
         indx_x = np.where(indx_x >= self.imDim[1], outofbounds, indx_x)
         indx1D = np.clip(indx_x+self.imDim[1]*n, 0, outofbounds)
+        # for j in range(self.nRho):
+        #   indx_good = indx1D[j,:].flatten()
+        #   whgood = np.nonzero(indx_good < outofbounds)[0]
+        #   if whgood.size > 0:
+        #
+        #     maskval = (self.mask.flatten())[indx_good[whgood]]
+        #     newindex = (self.maskindex.flatten())[indx_good[whgood]]
+        #
+        #     whmask = np.nonzero( (maskval > 0) & (newindex >= 0) )[0]
+        #     indx1D[j,:] = outofbounds
+        #     if (whmask.size > 0):
+        #       indx1D[j, 0:whmask.size] = newindex[whmask]
+
         self.indexPlan[:, i, 0:self.imDim[0]] = indx1D
-      self.indexPlan.sort(axis = -1)
+    tempindx = self.indexPlan.flatten()
+    mask = np.concatenate( (self.mask.flatten(), np.array([0,0])))
+    tempindx = np.where(mask[tempindx] > 0, tempindx, outofbounds)
+    maskindex = np.concatenate((self.maskindex.flatten(), np.array([-1,-1])))
+    tempindx = np.where(maskindex[tempindx] >= 0, maskindex[tempindx], outofbounds)
+    self.indexPlan = tempindx.reshape([self.nRho,self.nTheta,self.imDim.max()])
+    self.indexPlan.sort(axis = -1)
+
+
+  def masksetup(self,mask=None, maskindex=None):
+    if mask is not None:
+      self.mask = np.array(mask).astype(int)
+    if maskindex is not None:
+      self.maskindex = np.array(maskindex).astype(np.int64)
+
+    nPx = int(self.imDim[0]) * int(self.imDim[1])
+
+    if self.mask is None:
+      self.mask = np.ones(self.imDim)
+    if self.maskindex is None:
+      self.maskindex = np.arange(nPx, dtype = np.int64)
+      self.maskindex = self.maskindex.reshape(self.imDim)
+
+    #if (self.mask.shape != self.imDim).all():
+    #  raise Exception("mask and image must have same size")
+    #  #return -1
+    #if (self.maskindex.shape != self.imDim).all():
+    #  raise Exception("mask index array and image must have same size")
+    #  #return -2
+    if self.maskindex.max() >= nPx:
+      raise Exception("max of index array must be less than the total number of pixel in the array")
+      #return -3
 
+    self.radon_plan_setup()
 
-  def radon_fast(self, imageIn, padding = np.array([0,0]), fixArtifacts = False, background = None):
+  def radon_fast(self, imageIn, padding = np.array([0,0]), fixArtifacts = False,
+                 background = None, background_method = 'SUBTRACT'):
     tic = timer()
     shapeIm = np.shape(imageIn)
     if imageIn.ndim == 2:
       nIm = 1
       image = imageIn[np.newaxis, : ,:]
       reform = True
     else:
+      image = imageIn
       nIm = shapeIm[0]
       reform = False
 
     if background is None:
-      image = imageIn.reshape(-1)
+      pass
+      #image = image.reshape(-1)
     else:
-      image = imageIn - background
-      image = image.reshape(-1)
+      if str.upper(background_method) == 'DIVIDE':
+        image = imageIn / background
+      else:
+        image = imageIn - background
+      #image = image.reshape(-1)
 
     nPx = shapeIm[-1]*shapeIm[-2]
-    im = np.zeros(nPx+1, dtype=np.float32)
+    im = np.zeros(nPx+2, dtype=np.float32)
     #radon = np.zeros([nIm, self.nRho, self.nTheta], dtype=np.float32)
-    radon = np.zeros([nIm,self.nRho + 2 * padding[0],self.nTheta + 2 * padding[1]],dtype=np.float32)
+    radon = np.full([nIm,self.nRho + 2 * padding[0],self.nTheta + 2 * padding[1]], self.missingval, dtype=np.float32)
     shpRdn = radon.shape
     norm = np.sum(self.indexPlan < nPx, axis = 2 ) + 1.0e-12
     for i in np.arange(nIm):
-      im[:-1] = image[i,:,:].flatten()
-      radon[i, padding[0]:shpRdn[1]-padding[0], padding[1]:shpRdn[2]-padding[1]] = np.sum(im.take(self.indexPlan.astype(np.int64)), axis=2) / norm
+      im[:-2] = (image[i,:,:].flatten()).astype(np.float32)
+      radon[i, padding[0]:shpRdn[1]-padding[0], padding[1]:shpRdn[2]-padding[1]] = (
+          np.sum(im.take(self.indexPlan.astype(np.int64)), axis=2) / norm)
+      radon[i, padding[0]:shpRdn[1]-padding[0], padding[1]:shpRdn[2]-padding[1]] += -1.0*(norm < 1.0).astype(float)
 
     if (fixArtifacts == True):
       radon[:,:,0] = radon[:,:,1]
       radon[:,:,-1] = radon[:,:,-2]
 
     radon = np.transpose(radon, [1,2,0]).copy()
 
     if reform==True:
       image = image.reshape(shapeIm)
 
     #print(timer()-tic)
     return radon
 
-  def radon_faster(self,imageIn,padding = np.array([0,0]), fixArtifacts = False, background = None):
+  def radon_faster(self,imageIn,padding = np.array([0,0]), fixArtifacts = False, background = None, normalization=True):
     tic = timer()
     shapeIm = np.shape(imageIn)
     if imageIn.ndim == 2:
       nIm = 1
       #image = image[np.newaxis, : ,:]
       #reform = True
     else:
       nIm = shapeIm[0]
     #  reform = False
 
     if background is None:
-      image = imageIn.reshape(-1)
+      image = (imageIn.reshape(-1)).astype(np.float32)
     else:
       image = imageIn - background
-      image = image.reshape(-1)
+      image = (image.reshape(-1)).astype(np.float32)
 
     nPx = shapeIm[-1]*shapeIm[-2]
     indxDim = np.asarray(self.indexPlan.shape)
     #radon = np.zeros([nIm, self.nRho+2*padding[0], self.nTheta+2*padding[1]], dtype=np.float32)
-    radon = np.zeros([self.nRho + 2 * padding[0],self.nTheta + 2 * padding[1], nIm],dtype=np.float32)
+    radon = np.full([self.nRho + 2 * padding[0],self.nTheta + 2 * padding[1], nIm],self.missingval,dtype=np.float32)
     shp = radon.shape
 
-    counter = self.rdn_loops(image,self.indexPlan,nIm,nPx,indxDim,radon, np.asarray(padding))
+    counter = self.rdn_loops(image,self.indexPlan,nIm,nPx,indxDim,radon,
+                             np.asarray(padding), np.float32(normalization > 0))
 
     if (fixArtifacts == True):
       radon[:,padding[1],:] = radon[:,padding[1]+1,:]
       radon[:,shp[1]-1-padding[1],:] = radon[:,shp[1]-padding[1]-2,:]
 
 
     image = image.reshape(shapeIm)
 
     #print(timer()-tic)
     return radon#, counter
 
   @staticmethod
   @jit(nopython=True, fastmath=True, cache=True, parallel=False)
-  def rdn_loops(images,index,nIm,nPx,indxdim,radon, padding):
+  def rdn_loops(images,index,nIm,nPx,indxdim,radon, padding, norm):
     nRho = indxdim[0]
     nTheta = indxdim[1]
     nIndex = indxdim[2]
     #counter = np.zeros((nRho, nTheta, nIm), dtype=np.float32)
     count = 0.0
     sum = 0.0
     for q in prange(nIm):
@@ -208,32 +290,31 @@
           for k in range(nIndex):
             indx1 = index[i,j,k]
             if (indx1 >= nPx):
               break
             #radon[q, i, j] += images[imstart+indx1]
             sum += images[imstart + indx1]
             count += 1.0
-          #if count >= 1.0:
+          if count >= 1.0:
+            if norm < 0.001:
+              count =1.0
             #counter[ip,jp, q] = count
-          radon[ip,jp,q] = sum/(count + 1.0e-12)
+            radon[ip,jp,q] = sum/count
+
     #return counter
 
   def radon2pole(self,bandData,PC=None,vendor='EDAX'):
     # Following Krieger-Lassen1994 eq 3.1.6 //figure 3.1.1
     if PC is None:
       PC = np.array([0.471659,0.675044,0.630139])
     ven = str.upper(vendor)
 
     nPats = bandData.shape[0]
     nBands = bandData.shape[1]
 
-    # This translation from the Radon to theta and rho assumes that the first pixel read
-    # in off the detector is in the bottom left corner. -- No longer the assumption --- see below.
-    # theta = self.radonPlan.theta[np.array(bandData['aveloc'][:,:,1], dtype=np.int)]/RADEG
-    # rho = self.radonPlan.rho[np.array(bandData['aveloc'][:, :, 0], dtype=np.int)]
 
     # This translation from the Radon to theta and rho assumes that the first pixel read
     # in off the detector is in the top left corner.
 
     #theta = np.pi - self.radonPlan.theta[np.array(bandData['aveloc'][:,:,1],dtype=np.int64)] / RADEG
     #rho = -1.0 * self.radonPlan.rho[np.array(bandData['aveloc'][:,:,0],dtype=np.int64)]
 
@@ -264,15 +345,17 @@
           pctemp = np.tile(pctemp[0,:], nPats).reshape(nPats,4)
       t = pctemp[:,0:3]
       t[:,2] /= pctemp[:,3] # normalize by pixel size
 
 
 
     dimf = np.array(self.imDim, dtype=np.float32)
-    if ven in ['EDAX', 'OXFORD']:
+    if ven in ['EDAX']:
+      t *= np.array([dimf[1], dimf[0], -np.min(dimf[0:2])])
+    if ven in ['OXFORD']:
       t *= np.array([dimf[1], dimf[1], -dimf[1]])
     if ven == 'EMSOFT':
       t[:, 0] *= -1.0
       t += np.array([dimf[1] / 2.0, dimf[0] / 2.0, 0.0])
       t[:, 2] *= -1.0
     if ven in ['KIKUCHIPY', 'BRUKER']:
       t *=  np.array([dimf[1], dimf[0], -dimf[0]])
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/rotations.py` & `pyebsdindex-0.3.0/pyebsdindex/rotations.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/rotlib.py` & `pyebsdindex-0.3.0/pyebsdindex/rotlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,21 +47,24 @@
 # If the inputs are not in C-order or not aligned, a copy of the input will be made. 
 #
 #
 '''
 
 import numpy as np
 import numba
-from os import environ
+import os
 import tempfile
-from pathlib import PurePath
+from pathlib import PurePath, Path
 import platform
-tempdir = PurePath("/tmp" if platform.system() == "Darwin" else tempfile.gettempdir())
-tempdir = tempdir.joinpath('numba')
-environ["NUMBA_CACHE_DIR"] = str(tempdir)
+tempdir = PurePath(Path.home())
+#tempdir = PurePath("/tmp" if platform.system() == "Darwin" else tempfile.gettempdir())
+#tempdir = tempdir.joinpath('numbacache')
+tempdir = tempdir.joinpath('.pyebsdindex').joinpath('numbacache')
+Path(tempdir).mkdir(parents=True, exist_ok=True)
+os.environ["NUMBA_CACHE_DIR"] = str(tempdir)+str(os.sep)
 
 P = 1
 eps = 1.0e-12 # used for "closeto" approximations in Numba code
 PI = np.pi
 PI2 = 2.0 * np.pi
 nbcache = True # switch to false for debugging.
 nbParallel = False # decide if parallelism is desired.
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/tests/conftest.py` & `pyebsdindex-0.3.0/pyebsdindex/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png` & `pyebsdindex-0.3.0/pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/tests/data/al_sim_20kv/generate_al_sim_20kv.py` & `pyebsdindex-0.3.0/pyebsdindex/tests/data/al_sim_20kv/generate_al_sim_20kv.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/tests/numbatest.py` & `pyebsdindex-0.3.0/pyebsdindex/tests/numbatest.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/tests/raytest.py` & `pyebsdindex-0.3.0/pyebsdindex/tests/raytest.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/tests/rotlibunittest.py` & `pyebsdindex-0.3.0/pyebsdindex/tests/rotlibunittest.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 pi = np.pi
 RADDEG = 180.0/pi
 # I had some issues with the periodic boundaries in cubochoric/homochoric/quaternion spaces, so I am using
 # quaternion misorientation to evaluate the error.
 
 def testrotlib(float32=False, return_quat=False, seed = 1, n = 1000000):
-  n = np.int(n)
+  n = int(n)
   np.random.seed(seed)
   qu = (np.random.random((n,4))*2.0-1)
   if float32 is True:
     qu = qu.astype(np.float32)
   qu = quatnorm(qu)
   qu[0, :] = np.array([1.0, 0.0, 0.0, 0.0])
   qu[1, :] = np.array([0.0,0.0,0.0,-1.0])
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/tests/test_ebsd_index.py` & `pyebsdindex-0.3.0/pyebsdindex/tests/test_ebsd_index.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,18 +40,18 @@
         indexer = EBSDIndexer()
         assert indexer.phaselist == ["FCC"]
         assert indexer.sampleTilt == 70
         assert indexer.camElev == 5.3
         assert indexer.vendor == "EDAX"
 
     def test_index_pats(self, pattern_al_sim_20kv):
-        """Test Hough indexing and setting/passing projection center
+        """Test Radon indexing and setting/passing projection center
         values.
         """
-        pc = (0.4, 0.6, 0.5)
+        pc = (0.4, 0.72, 0.6)
 
         # Set PC upon initialization of indexer
         indexer = EBSDIndexer(PC=pc, patDim=pattern_al_sim_20kv.shape)
         data = indexer.index_pats(pattern_al_sim_20kv)[0]
         assert np.allclose(data[0]["quat"], data[1]["quat"])
 
         # Pass PC upon indexing
@@ -63,18 +63,19 @@
 
         # Expected rotation
         euler = np.rad2deg(qu2eu(data[0]["quat"]))
         assert np.isclose(euler, self._possible_euler, atol=2).any()
 
     @pytest.mark.skipif(not _ray_installed, reason="ray is not installed")
     def test_index_pats_multi(self, pattern_al_sim_20kv):
-        """Test Hough indexing parallelized with ray."""
+        """Test Radon indexing parallelized with ray."""
         from pyebsdindex.ebsd_index import index_pats_distributed
 
         patterns = np.repeat(pattern_al_sim_20kv[None, ...], 4, axis=0)
-        indexer = EBSDIndexer(PC=(0.4, 0.6, 0.5), patDim=patterns.shape[1:])
-        data = index_pats_distributed(patterns, ebsd_indexer_obj=indexer)
+        indexer = EBSDIndexer(PC=(0.4, 0.72, 0.6), patDim=patterns.shape[1:])
+        data = index_pats_distributed(patsin=patterns, ebsd_indexer_obj=indexer)[0]
 
         # Expected rotation
         euler = np.rad2deg(qu2eu(data[0]["quat"]))
+
         assert np.isclose(euler[0], self._possible_euler, atol=2).any()
         assert np.allclose(euler[0], euler[1:])
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/tests/test_package.py` & `pyebsdindex-0.3.0/pyebsdindex/tests/test_package.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,25 +35,32 @@
     from pyebsdindex.opencl.band_detect_cl import BandDetect as BandDetectCL
     assert issubclass(BandDetectCL, BandDetect)
 
 
 @pytest.mark.skipif(_pyopencl_installed, reason="pyopencl is installed")
 def test_unavailable_functionality_without_pyopencl():
     with pytest.raises(ImportError):
-        from pyebsdindex.opencl.band_detect_cl import BandDetect
 
+        from pyebsdindex.opencl import openclparam
+        try:
+            clparam = openclparam.OpenClParam()
+            gpu = clparam.get_gpu()
+            if len(gpu) < 1:
+                raise ImportError('')
+        except:
+            raise ImportError('')
 
 @pytest.mark.skipif(not _ray_installed, reason="ray is not installed")
 def test_available_functionality_with_ray():
     from pyebsdindex.ebsd_index import index_pats_distributed
-    from pyebsdindex.ebsd_index import IndexerRay
+    #from pyebsdindex.ebsd_index import IndexerRay
 
-    assert callable(index_pats_distributed)
-    _ = IndexerRay.remote()
+    #assert callable(index_pats_distributed)
+    #_ = IndexerRay.remote()
 
 
 @pytest.mark.skipif(_ray_installed, reason="ray is installed")
 def test_unavailable_functionality_without_ray():
     with pytest.raises(ImportError):
         from pyebsdindex.ebsd_index import index_pats_distributed
-    with pytest.raises(ImportError):
-        from pyebsdindex.ebsd_index import IndexerRay
+    #with pytest.raises(ImportError):
+    #    from pyebsdindex.ebsd_index import IndexerRay
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex/tests/test_pcopt.py` & `pyebsdindex-0.3.0/pyebsdindex/tests/test_pcopt.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 import numpy as np
 
 from pyebsdindex import ebsd_index, pcopt
 
 
 class TestPCOptimization:
     def test_pc_optimize(self, pattern_al_sim_20kv):
-        pc0 = (0.4, 0.6, 0.5)
+        pc0 = (0.4, 0.72, 0.6)
         indexer = ebsd_index.EBSDIndexer(patDim=pattern_al_sim_20kv.shape)
         new_pc = pcopt.optimize(pattern_al_sim_20kv, indexer, PC0=pc0)
         assert np.allclose(new_pc, pc0, atol=0.05)
 
     def test_pc_optimize_pso(self, pattern_al_sim_20kv):
-        pc0 = (0.4, 0.6, 0.5)
+        pc0 = (0.4, 0.72, 0.6)
         indexer = ebsd_index.EBSDIndexer(patDim=pattern_al_sim_20kv.shape)
         new_pc = pcopt.optimize_pso(pattern_al_sim_20kv, indexer, PC0=pc0)
         assert np.allclose(new_pc, pc0, atol=0.05)
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex.egg-info/SOURCES.txt` & `pyebsdindex-0.3.0/pyebsdindex.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .readthedocs.yaml
 CHANGELOG.rst
 CONTRIBUTING.rst
 IPFCubic.pdf
 IPFCubic.png
+IPFHex.pdf
+IPFHex.png
 License
 MANIFEST.in
 README.md
 RELEASE.rst
 setup.cfg
 setup.py
 doc/Makefile
@@ -31,44 +33,49 @@
 doc/tutorials/index.rst
 doc/user/index.rst
 doc/user/installation.rst
 pyebsdindex/__init__.py
 pyebsdindex/_ebsd_index_parallel.py
 pyebsdindex/_ebsd_index_single.py
 pyebsdindex/band_detect.py
-pyebsdindex/band_vote.py
 pyebsdindex/crystal_sym.py
 pyebsdindex/crystallometry.py
 pyebsdindex/ebsd_index.py
 pyebsdindex/ebsd_pattern.py
 pyebsdindex/ebsdfile.py
+pyebsdindex/misorientation.py
 pyebsdindex/nlpar.py
+pyebsdindex/nlpar_cpu.py
 pyebsdindex/pairlib.py
 pyebsdindex/pcopt.py
 pyebsdindex/radon_fast.py
 pyebsdindex/rotations.py
 pyebsdindex/rotlib.py
-pyebsdindex/spherical_radon_fast.py
-pyebsdindex/tripletlib.py
+pyebsdindex/tripletvote.py
 pyebsdindex.egg-info/PKG-INFO
 pyebsdindex.egg-info/SOURCES.txt
 pyebsdindex.egg-info/dependency_links.txt
 pyebsdindex.egg-info/requires.txt
 pyebsdindex.egg-info/top_level.txt
 pyebsdindex.egg-info/zip-safe
 pyebsdindex/EBSDImage/IPFcolor.py
 pyebsdindex/EBSDImage/__init__.py
 pyebsdindex/opencl/__init__.py
 pyebsdindex/opencl/band_detect_cl.py
 pyebsdindex/opencl/clkernels.cl
+pyebsdindex/opencl/clnlpar.cl
+pyebsdindex/opencl/nlpar_cl.py
+pyebsdindex/opencl/nlpar_clray.py
 pyebsdindex/opencl/openclparam.py
 pyebsdindex/opencl/radon_fast_cl.py
+pyebsdindex/opencl/test.cl
 pyebsdindex/tests/__init__.py
 pyebsdindex/tests/conftest.py
 pyebsdindex/tests/numbatest.py
 pyebsdindex/tests/raytest.py
 pyebsdindex/tests/rotlibunittest.py
 pyebsdindex/tests/test_ebsd_index.py
 pyebsdindex/tests/test_package.py
 pyebsdindex/tests/test_pcopt.py
+pyebsdindex/tests/test_tripletvote.py
 pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png
 pyebsdindex/tests/data/al_sim_20kv/generate_al_sim_20kv.py
```

### Comparing `pyebsdindex-0.2.dev0/pyebsdindex.egg-info/requires.txt` & `pyebsdindex-0.3.0/pyebsdindex.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 h5py
 matplotlib
 numpy
-numba
-pyswarms
+numba>=0.53
 scipy
 
 [all]
 pyopencl
 ray[default]>=1.13
+pydantic<2
 nbsphinx>=0.7
 numpydoc
 pydata-sphinx-theme
 sphinx>=3.0.2
 sphinx-codeautolink[ipython]
 sphinx-copybutton>=0.2.5
 sphinx-design
@@ -30,14 +30,15 @@
 sphinx-design
 sphinx-gallery
 coverage>=5.0
 pytest>=5.4
 pytest-cov>=2.8.1
 pyopencl
 ray[default]>=1.13
+pydantic<2
 
 [doc]
 nbsphinx>=0.7
 numpydoc
 pydata-sphinx-theme
 sphinx>=3.0.2
 sphinx-codeautolink[ipython]
@@ -46,12 +47,13 @@
 sphinx-gallery
 
 [gpu]
 pyopencl
 
 [parallel]
 ray[default]>=1.13
+pydantic<2
 
 [tests]
 coverage>=5.0
 pytest>=5.4
 pytest-cov>=2.8.1
```

### Comparing `pyebsdindex-0.2.dev0/setup.py` & `pyebsdindex-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,21 +19,22 @@
         "sphinx-copybutton              >= 0.2.5",
         "sphinx-design",
         "sphinx-gallery",
     ],
     "tests": [
         "coverage                       >= 5.0",
         "pytest                         >= 5.4",
-        "pytest-cov                     >= 2.8.1"
+        "pytest-cov                     >= 2.8.1",
     ],
     "gpu": [
         "pyopencl",
     ],
     "parallel": [
         "ray[default]                   >= 1.13",
+        "pydantic                       < 2",
     ]
 }
 # Create a development installation "dev" including "doc" and "tests"
 # projects
 extra_feature_requirements["dev"] = list(
     chain(*list(extra_feature_requirements.values()))
 )
@@ -56,27 +57,28 @@
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: Other/Proprietary License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Physics",
     ],
     keywords=[
         "EBSD",
         "electron backscatter diffraction",
         "HI",
-        "Hough indexing",
+        "Radon indexing",
         "NLPAR",
     ],
     zip_safe=True,
     # Contact
     author=__credits__,
     download_url="https://pypi.python.org/pypi/pyebsdindex",
     maintainer=__author__,
@@ -89,16 +91,15 @@
     url="https://pyebsdindex.readthedocs.io",
     # Dependencies
     extras_require=extra_feature_requirements,
     install_requires=[
         "h5py",
         "matplotlib",
         "numpy",
-        "numba",
-        "pyswarms",
+        "numba>=0.53",
         "scipy",
     ],
     # Files to include when distributing package (see also MANIFEST.in)
     packages=find_packages(),
     package_dir={"pyebsdindex": "pyebsdindex"},
     include_package_data=True,
 )
```

