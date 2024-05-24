# Comparing `tmp/epmatools-0.0.3.tar.gz` & `tmp/epmatools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epmatools-0.0.3.tar", last modified: Mon May 20 05:38:58 2024, max compression
+gzip compressed data, was "epmatools-0.0.4.tar", last modified: Fri May 24 18:09:13 2024, max compression
```

## Comparing `epmatools-0.0.3.tar` & `epmatools-0.0.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:38:58.654909 epmatools-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:38:58.642909 epmatools-0.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-20 05:38:53.000000 epmatools-0.0.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:38:58.642909 epmatools-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-20 05:38:53.000000 epmatools-0.0.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-20 05:38:53.000000 epmatools-0.0.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-20 05:38:53.000000 epmatools-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-20 05:38:53.000000 epmatools-0.0.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-20 05:38:53.000000 epmatools-0.0.3/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-20 05:38:53.000000 epmatools-0.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-20 05:38:58.654909 epmatools-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-20 05:38:53.000000 epmatools-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-20 05:38:53.000000 epmatools-0.0.3/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:38:58.642909 epmatools-0.0.3/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-20 05:38:53.000000 epmatools-0.0.3/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-20 05:38:53.000000 epmatools-0.0.3/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-20 05:38:53.000000 epmatools-0.0.3/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 05:38:53.000000 epmatools-0.0.3/doc/demo.nblink
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-20 05:38:53.000000 epmatools-0.0.3/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 05:38:53.000000 epmatools-0.0.3/doc/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-20 05:38:53.000000 epmatools-0.0.3/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-20 05:38:53.000000 epmatools-0.0.3/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-20 05:38:53.000000 epmatools-0.0.3/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:38:58.650910 epmatools-0.0.3/epmatools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-20 05:38:58.000000 epmatools-0.0.3/epmatools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-20 05:38:58.000000 epmatools-0.0.3/epmatools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 05:38:58.000000 epmatools-0.0.3/epmatools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-20 05:38:58.000000 epmatools-0.0.3/epmatools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-20 05:38:58.000000 epmatools-0.0.3/epmatools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 05:38:58.000000 epmatools-0.0.3/epmatools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:38:58.642909 epmatools-0.0.3/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)  2981627 2024-05-20 05:38:53.000000 epmatools-0.0.3/notebooks/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-20 05:38:53.000000 epmatools-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 05:38:58.654909 epmatools-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 05:38:53.000000 epmatools-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:38:58.650910 epmatools-0.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-20 05:38:53.000000 epmatools-0.0.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 05:38:53.000000 epmatools-0.0.3/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 05:38:58.000000 epmatools-0.0.3/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:38:58.638909 epmatools-0.0.3/src/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:38:58.650910 epmatools-0.0.3/src/data/maps/
--rw-r--r--   0 runner    (1001) docker     (127)  1331930 2024-05-20 05:38:53.000000 epmatools-0.0.3/src/data/maps/ex1.h5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:38:58.650910 epmatools-0.0.3/src/data/oxides/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-20 05:38:53.000000 epmatools-0.0.3/src/data/oxides/avgpelite.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-20 05:38:53.000000 epmatools-0.0.3/src/data/oxides/grt_profile.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-20 05:38:53.000000 epmatools-0.0.3/src/data/oxides/minerals.csv
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-20 05:38:53.000000 epmatools-0.0.3/src/data/oxides/pyroxenes.csv
--rw-r--r--   0 runner    (1001) docker     (127)    39348 2024-05-20 05:38:53.000000 epmatools-0.0.3/src/datatables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-05-20 05:38:53.000000 epmatools-0.0.3/src/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    43992 2024-05-20 05:38:53.000000 epmatools-0.0.3/src/maps.py
--rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-20 05:38:53.000000 epmatools-0.0.3/src/minerals.py
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-05-20 05:38:53.000000 epmatools-0.0.3/src/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:38:58.650910 epmatools-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:38:53.000000 epmatools-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-20 05:38:53.000000 epmatools-0.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-20 05:38:53.000000 epmatools-0.0.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-20 05:38:53.000000 epmatools-0.0.3/tests/test_epmatools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:09:12.996367 epmatools-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:09:12.980367 epmatools-0.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-24 18:09:07.000000 epmatools-0.0.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:09:12.980367 epmatools-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-24 18:09:07.000000 epmatools-0.0.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-24 18:09:07.000000 epmatools-0.0.4/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-24 18:09:07.000000 epmatools-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-24 18:09:07.000000 epmatools-0.0.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 18:09:07.000000 epmatools-0.0.4/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-24 18:09:07.000000 epmatools-0.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-24 18:09:12.996367 epmatools-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-24 18:09:07.000000 epmatools-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-24 18:09:07.000000 epmatools-0.0.4/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:09:12.984367 epmatools-0.0.4/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-24 18:09:07.000000 epmatools-0.0.4/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-24 18:09:07.000000 epmatools-0.0.4/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-24 18:09:07.000000 epmatools-0.0.4/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-24 18:09:07.000000 epmatools-0.0.4/doc/demo.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-24 18:09:07.000000 epmatools-0.0.4/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-24 18:09:07.000000 epmatools-0.0.4/doc/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-24 18:09:07.000000 epmatools-0.0.4/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-24 18:09:07.000000 epmatools-0.0.4/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-24 18:09:07.000000 epmatools-0.0.4/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:09:12.996367 epmatools-0.0.4/epmatools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-24 18:09:12.000000 epmatools-0.0.4/epmatools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-24 18:09:12.000000 epmatools-0.0.4/epmatools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:09:12.000000 epmatools-0.0.4/epmatools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 18:09:12.000000 epmatools-0.0.4/epmatools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-24 18:09:12.000000 epmatools-0.0.4/epmatools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 18:09:12.000000 epmatools-0.0.4/epmatools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:09:12.984367 epmatools-0.0.4/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)  2981627 2024-05-24 18:09:07.000000 epmatools-0.0.4/notebooks/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-24 18:09:07.000000 epmatools-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 18:09:12.996367 epmatools-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 18:09:07.000000 epmatools-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:09:12.992367 epmatools-0.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-24 18:09:07.000000 epmatools-0.0.4/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-24 18:09:07.000000 epmatools-0.0.4/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 18:09:12.000000 epmatools-0.0.4/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:09:12.980367 epmatools-0.0.4/src/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:09:12.992367 epmatools-0.0.4/src/data/maps/
+-rw-r--r--   0 runner    (1001) docker     (127)  1331930 2024-05-24 18:09:07.000000 epmatools-0.0.4/src/data/maps/ex1.h5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:09:12.992367 epmatools-0.0.4/src/data/oxides/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-24 18:09:07.000000 epmatools-0.0.4/src/data/oxides/avgpelite.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-24 18:09:07.000000 epmatools-0.0.4/src/data/oxides/grt_profile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-24 18:09:07.000000 epmatools-0.0.4/src/data/oxides/minerals.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-24 18:09:07.000000 epmatools-0.0.4/src/data/oxides/pyroxenes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    39309 2024-05-24 18:09:07.000000 epmatools-0.0.4/src/datatables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-05-24 18:09:07.000000 epmatools-0.0.4/src/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43992 2024-05-24 18:09:07.000000 epmatools-0.0.4/src/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-24 18:09:07.000000 epmatools-0.0.4/src/minerals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-24 18:09:07.000000 epmatools-0.0.4/src/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:09:12.996367 epmatools-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:09:07.000000 epmatools-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-24 18:09:07.000000 epmatools-0.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-24 18:09:07.000000 epmatools-0.0.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-24 18:09:07.000000 epmatools-0.0.4/tests/test_epmatools.py
```

### Comparing `epmatools-0.0.3/.github/workflows/ci.yml` & `epmatools-0.0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/.github/workflows/pypi.yml` & `epmatools-0.0.4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/.gitignore` & `epmatools-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/LICENSE.md` & `epmatools-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/PKG-INFO` & `epmatools-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epmatools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tools to manipulate EPMA analyses
 Maintainer-email: Ondrej Lexa <lexa.ondrej@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `epmatools-0.0.3/README.md` & `epmatools-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/doc/Makefile` & `epmatools-0.0.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/doc/api.rst` & `epmatools-0.0.4/doc/api.rst`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/doc/conf.py` & `epmatools-0.0.4/doc/conf.py`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/doc/make.bat` & `epmatools-0.0.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/environment-dev.yml` & `epmatools-0.0.4/environment-dev.yml`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/epmatools.egg-info/PKG-INFO` & `epmatools-0.0.4/epmatools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epmatools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tools to manipulate EPMA analyses
 Maintainer-email: Ondrej Lexa <lexa.ondrej@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `epmatools-0.0.3/epmatools.egg-info/SOURCES.txt` & `epmatools-0.0.4/epmatools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/notebooks/demo.ipynb` & `epmatools-0.0.4/notebooks/demo.ipynb`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/pyproject.toml` & `epmatools-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/src/data/maps/ex1.h5` & `epmatools-0.0.4/src/data/maps/ex1.h5`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/src/data/oxides/grt_profile.csv` & `epmatools-0.0.4/src/data/oxides/grt_profile.csv`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/src/data/oxides/minerals.csv` & `epmatools-0.0.4/src/data/oxides/minerals.csv`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/src/datatables.py` & `epmatools-0.0.4/src/datatables.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,20 +30,22 @@
         @wraps(func)
         def wrapper(self, *args, **kwargs):
             df = func(self, *args, **kwargs)
             res = self._data.copy()
             res[self._valid] = df
             # parse dekwargs
             newargs = dict(
-                units = wrapper.dekwargs.get("units", self.units),
-                desc = wrapper.dekwargs.get("desc", self.desc)
+                units=wrapper.dekwargs.get("units", self.units),
+                desc=wrapper.dekwargs.get("desc", self.desc),
             )
             return type(self)(res, name=self.name, **newargs)
+
         wrapper.dekwargs = dekwargs
         return wrapper
+
     return inner
 
 
 class Compo:
     def __init__(self, df, **kwargs):
         # Check argument (convert Series to DataFrame if needed)
         if isinstance(df, pd.Series):
@@ -78,30 +80,20 @@
                 raise ValueError(f"Index must be on of {self._valid}")
         if isinstance(index, slice):
             return self.finalize(self._data.loc[index].copy())
         else:
             raise TypeError("Only string could be used as index.")
 
     def finalize(self, vals, **kwargs):
-        if hasattr(self, 'mineral'):
-            return type(self)(
-                vals,
-                units=kwargs.get("units", self.units),
-                name=kwargs.get("name", self.name),
-                desc=kwargs.get("desc", self.desc),
-                mineral=self.mineral,
-            )
-        else:
-            return type(self)(
-                vals,
-                units=kwargs.get("units", self.units),
-                name=kwargs.get("name", self.name),
-                desc=kwargs.get("desc", self.desc),
-            )
-
+        return type(self)(
+            vals,
+            units=kwargs.get("units", self.units),
+            name=kwargs.get("name", self.name),
+            desc=kwargs.get("desc", self.desc),
+        )
 
     def reversed(self):
         """Return in reversed order"""
         res = self._data.reindex(index=self._data.index[::-1])
         return self.finalize(res)
 
     def iterrows(self, what=None):
@@ -154,15 +146,17 @@
         """Set index of datatable
 
         Args:
             key (str or list like): Either name of column (see ``Oxides.others``) or
                 collection of same length as datatable
         """
         assert key in self._others, f"Column name must be one of {self._others}"
-        return self.finalize(self._data.reset_index(drop=True).set_index(key, drop=False))
+        return self.finalize(
+            self._data.reset_index(drop=True).set_index(key, drop=False)
+        )
 
     def reset_index(self):
         """Reset index to default pandas.RangeIndex"""
         return self.finalize(self._data.reset_index(drop=True))
 
     def head(self, n=5):
         """Return first n rows
@@ -1068,15 +1062,15 @@
         >>> d = Oxides.apfu(mindb.Garnet_Fe2())
 
     """
 
     def __init__(self, df, mineral, **kwargs):
         super().__init__(df, **kwargs)
         self.parse_columns()
-        self.decimals = kwargs.get("decimals", 3)
+        self.decimals = kwargs.get("decimals", 4)
         self.mineral = mineral
 
     def __repr__(self):
         return "\n".join(
             [
                 f"APFU[{self.mineral}]: {self.name} [{self.units}] - {self.desc}",
                 f"{self.df.round(decimals=self.decimals)}",
@@ -1088,14 +1082,23 @@
             self.df.style.set_caption(
                 f"APFU[{self.mineral}]: {self.name} [{self.units}] - {self.desc}"
             )
             .format(precision=self.decimals)
             .to_html()
         )
 
+    def finalize(self, vals, **kwargs):
+        return type(self)(
+            vals,
+            mineral=self.mineral,
+            units=kwargs.get("units", self.units),
+            name=kwargs.get("name", self.name),
+            desc=kwargs.get("desc", self.desc),
+        )
+
     def endmembers(self, force=False):
         """Calculate endmembers proportions
 
         Args:
             force (bool, optional): when True, remaining cations are added to last site
 
         """
```

### Comparing `epmatools-0.0.3/src/io.py` & `epmatools-0.0.4/src/io.py`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/src/maps.py` & `epmatools-0.0.4/src/maps.py`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/src/minerals.py` & `epmatools-0.0.4/src/minerals.py`

 * *Files identical despite different names*

### Comparing `epmatools-0.0.3/src/plotting.py` & `epmatools-0.0.4/src/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import math
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.colors as mcolors
 from matplotlib.widgets import SpanSelector
+from matplotlib.ticker import MaxNLocator
 
 
 def plot_grt_profile(em, **kwargs):
     """Plot garnet profiles.
 
     Note:
         Endmembers have to be properly ordered.
@@ -107,40 +108,41 @@
     data2 = kwargs.get("data2", ["Prp", "Sps", "Grs"])
     datalim1 = kwargs.get("datalim1", None)
     datalim2 = kwargs.get("datalim2", None)
     filename = kwargs.get("filename", None)
     maxticks = kwargs.get("maxticks", 20)
     colors1 = list(mcolors.TABLEAU_COLORS.keys())[: len(data1)]
     colors2 = list(mcolors.TABLEAU_COLORS.keys())[len(data1) : len(data1) + len(data2)]
+    fig, ax1 = plt.subplots()
     if kwargs.get("percents", False):
-        em = 100 * em
+        multiple = 100
         unit = " [%]"
     else:
+        multiple = 1
         unit = " [prop.]"
     if kwargs.get("use_index", False):
         xvals = em.index
         xlabel = kwargs.get("xlabel", "index")
     else:
         xvals = range(len(em))
         xlabel = kwargs.get("xlabel", "position")
-    fig, ax1 = plt.subplots()
     ax1.set_xlabel(xlabel)
     # omit
     if kwargs.get("omit", None) is not None:
         em.loc[kwargs.get("omit")] = np.nan
     if kwargs.get("twin", True):
         ax1.set_ylabel(" ".join(data1) + unit)
-        h1 = ax1.plot(xvals, em[data1], marker="o", ms=4)
+        h1 = ax1.plot(xvals, multiple * em[data1], marker="o", ms=4)
         for h, color in zip(h1, colors1):
             h.set_color(color)
         if datalim1 is not None:
             ax1.set_ylim(datalim1[0], datalim1[1])
         ax2 = ax1.twinx()
         ax2.set_ylabel(" ".join(data2) + unit)
-        h2 = ax2.plot(xvals, em[data2], marker="o", ms=4)
+        h2 = ax2.plot(xvals, multiple * em[data2], marker="o", ms=4)
         for h, color in zip(h2, colors2):
             h.set_color(color)
         if datalim2 is not None:
             ax2.set_ylim(datalim2[0], datalim2[1])
         plt.legend(
             h1 + h2,
             data1 + data2,
@@ -148,30 +150,30 @@
             loc=3,
             ncol=len(data1 + data2),
             mode="expand",
             borderaxespad=0.0,
         )
     else:
         ax1.set_ylabel(" ".join(data1 + data2) + unit)
-        h1 = ax1.plot(xvals, em[data1 + data2], marker="o", ms=4)
+        h1 = ax1.plot(xvals, multiple * em[data1 + data2], marker="o", ms=4)
         for h, color in zip(h1, colors1 + colors2):
             h.set_color(color)
         if datalim1 is not None:
             ax1.set_ylim(datalim1[0], datalim1[1])
         plt.legend(
             h1,
             data1 + data2,
             bbox_to_anchor=(0.0, 1.02, 1.0, 0.102),
             loc=3,
             ncol=len(data1 + data2),
             mode="expand",
             borderaxespad=0.0,
         )
     # Find at most maxticks ticks on the x-axis at 'nice' locations
-    xloc = plt.MaxNLocator(maxticks - 1)
+    xloc = MaxNLocator(maxticks - 1, integer=True)
     ax1.xaxis.set_major_locator(xloc)
     ax1.tick_params(axis="x", labelrotation=kwargs.get("xticks_rotation", 0))
     fig.tight_layout()
     if filename is not None:
         fig.savefig(filename)
     else:
         # if index used, spanselector created
```

