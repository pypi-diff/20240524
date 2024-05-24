# Comparing `tmp/mpltoolbox-24.5.0.tar.gz` & `tmp/mpltoolbox-24.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpltoolbox-24.5.0.tar", last modified: Mon May  6 10:51:30 2024, max compression
+gzip compressed data, was "mpltoolbox-24.5.1.tar", last modified: Fri May 24 12:12:24 2024, max compression
```

## Comparing `mpltoolbox-24.5.0.tar` & `mpltoolbox-24.5.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.893834 mpltoolbox-24.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.885834 mpltoolbox-24.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.885834 mpltoolbox-24.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-06 10:51:30.893834 mpltoolbox-24.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.889834 mpltoolbox-24.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/callbacks.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/ellipses.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.889834 mpltoolbox-24.5.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    75876 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    95767 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/lines.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/points.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/polygons.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/programmatic-control.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/rectangles.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/spans.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-06 10:51:30.893834 mpltoolbox-24.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.885834 mpltoolbox-24.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.889834 mpltoolbox-24.5.0/src/mpltoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/ellipses.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/hspans.py
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/points.py
--rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/rectangles.py
--rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/vspans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.893834 mpltoolbox-24.5.0/src/mpltoolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-06 10:51:30.000000 mpltoolbox-24.5.0/src/mpltoolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-06 10:51:30.000000 mpltoolbox-24.5.0/src/mpltoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:51:30.000000 mpltoolbox-24.5.0/src/mpltoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 10:51:30.000000 mpltoolbox-24.5.0/src/mpltoolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 10:51:30.000000 mpltoolbox-24.5.0/src/mpltoolbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.893834 mpltoolbox-24.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/tests/lines_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/tests/points_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:12:24.318737 mpltoolbox-24.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:12:24.306737 mpltoolbox-24.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:12:24.310737 mpltoolbox-24.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-24 12:12:24.318737 mpltoolbox-24.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:12:24.314737 mpltoolbox-24.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/docs/callbacks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/docs/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/docs/ellipses.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:12:24.314737 mpltoolbox-24.5.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    75876 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    95767 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/docs/lines.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/docs/points.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/docs/polygons.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/docs/programmatic-control.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/docs/rectangles.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/docs/spans.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-24 12:12:24.318737 mpltoolbox-24.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:12:24.310737 mpltoolbox-24.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:12:24.318737 mpltoolbox-24.5.1/src/mpltoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/src/mpltoolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/src/mpltoolbox/ellipses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/src/mpltoolbox/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/src/mpltoolbox/hspans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/src/mpltoolbox/lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/src/mpltoolbox/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/src/mpltoolbox/points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/src/mpltoolbox/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/src/mpltoolbox/rectangles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/src/mpltoolbox/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/src/mpltoolbox/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/src/mpltoolbox/vspans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:12:24.318737 mpltoolbox-24.5.1/src/mpltoolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-24 12:12:24.000000 mpltoolbox-24.5.1/src/mpltoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-24 12:12:24.000000 mpltoolbox-24.5.1/src/mpltoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:12:24.000000 mpltoolbox-24.5.1/src/mpltoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 12:12:24.000000 mpltoolbox-24.5.1/src/mpltoolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 12:12:24.000000 mpltoolbox-24.5.1/src/mpltoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:12:24.318737 mpltoolbox-24.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/tests/lines_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-24 12:12:18.000000 mpltoolbox-24.5.1/tests/points_test.py
```

### Comparing `mpltoolbox-24.5.0/.github/workflows/ci.yml` & `mpltoolbox-24.5.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/.readthedocs.yaml` & `mpltoolbox-24.5.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/LICENSE` & `mpltoolbox-24.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/PKG-INFO` & `mpltoolbox-24.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpltoolbox
-Version: 24.5.0
+Version: 24.5.1
 Summary: Interactive tools for matplotlib
 Home-page: https://github.com/scipp/mpltoolbox
 Author: Neil Vaytet
 Author-email: neil.vaytet@esss.se
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/mpltoolbox/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mpltoolbox-24.5.0/README.md` & `mpltoolbox-24.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/docs/callbacks.ipynb` & `mpltoolbox-24.5.1/docs/callbacks.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/docs/conf.py` & `mpltoolbox-24.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/docs/demo.ipynb` & `mpltoolbox-24.5.1/docs/demo.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/docs/ellipses.ipynb` & `mpltoolbox-24.5.1/docs/ellipses.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/docs/images/favicon.ico` & `mpltoolbox-24.5.1/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/docs/images/logo.png` & `mpltoolbox-24.5.1/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/docs/images/logo.svg` & `mpltoolbox-24.5.1/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/docs/index.rst` & `mpltoolbox-24.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/docs/lines.ipynb` & `mpltoolbox-24.5.1/docs/lines.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/docs/points.ipynb` & `mpltoolbox-24.5.1/docs/points.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/docs/polygons.ipynb` & `mpltoolbox-24.5.1/docs/polygons.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/docs/programmatic-control.ipynb` & `mpltoolbox-24.5.1/docs/programmatic-control.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/docs/rectangles.ipynb` & `mpltoolbox-24.5.1/docs/rectangles.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/docs/spans.ipynb` & `mpltoolbox-24.5.1/docs/spans.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/setup.cfg` & `mpltoolbox-24.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/src/mpltoolbox/ellipses.py` & `mpltoolbox-24.5.1/src/mpltoolbox/ellipses.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/src/mpltoolbox/hspans.py` & `mpltoolbox-24.5.1/src/mpltoolbox/hspans.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,29 +10,28 @@
 
 
 class Hspan(Patch):
     def __init__(
         self, x: float, y: float, number: int, ax: Axes, hide_median=False, **kwargs
     ):
         super().__init__(x=x, y=y, number=number, ax=ax, **kwargs)
-        self._vertices.set_transform(self._patch.get_transform())
         self._median = self._ax.axhline(y, ls="dashed", color=self.edgecolor)
+        self._vertices.set_transform(self._median.get_transform())
         if hide_median:
             self._median.set_visible(False)
 
     def __repr__(self):
         return (
             f"VSpan: bottom={self.bottom}, top={self.top}, "
             f"edgecolor={self.edgecolor}, facecolor={self.facecolor}"
         )
 
     def _update_vertices(self):
         super()._update_vertices()
-        corners = self._patch.get_xy()
-        mid = 0.5 * (corners[0, 1] + corners[1, 1])
+        mid = 0.5 * (self.bottom + self.top)
         self._median.set_ydata([mid, mid])
 
     def _make_patch(self, x, y, **kwargs):
         self._patch = self._ax.axhspan(y, y, **kwargs)
 
     def _make_vertices(self) -> Tuple[float]:
         return ([0.5, 0.5], [self.bottom, self.top])
@@ -46,57 +45,77 @@
 
     def remove(self):
         super().remove()
         self._median.remove()
 
     @property
     def bottom(self) -> float:
-        return self._patch.get_xy()[0, 1]
+        xy = self._patch.get_xy()
+        if len(xy) > 2:
+            return xy[0, 1]
+        return xy[1]
 
     @bottom.setter
     def bottom(self, y: float):
-        corners = self._patch.get_xy()
-        for i in [0, 3]:
-            corners[i, 1] = y
-        if len(corners) > 3:
-            corners[4, 1] = y
+        xy = self._patch.get_xy()
+        if len(xy) > 2:
+            for i in [0, 3]:
+                xy[i, 1] = y
+            if len(xy) > 3:
+                xy[4, 1] = y
+            else:
+                xy += [xy[0, 0], y]
+            self._patch.set_xy(xy)
         else:
-            corners += [corners[0, 0], y]
-        self._patch.set_xy(corners)
+            self._patch.set(height=xy[1] - y + self.height, xy=(0, y))
         self._update_vertices()
 
     @property
     def top(self) -> float:
-        return self._patch.get_xy()[1, 1]
+        xy = self._patch.get_xy()
+        if len(xy) > 2:
+            return xy[1, 1]
+        return xy[1] + self.height
 
     @top.setter
     def top(self, y: float):
-        corners = self._patch.get_xy()
-        for i in [1, 2]:
-            corners[i, 1] = y
-        self._patch.set_xy(corners)
+        xy = self._patch.get_xy()
+        if len(xy) > 2:
+            for i in [1, 2]:
+                xy[i, 1] = y
+            self._patch.set_xy(xy)
+        else:
+            self._patch.set(height=y - xy[1])
         self._update_vertices()
 
     @property
     def height(self) -> float:
+        if hasattr(self._patch, "get_height"):
+            return self._patch.get_height()
         corners = self._patch.get_xy()
         return corners[1, 1] - corners[0, 1]
 
     @property
     def xy(self) -> Tuple[float]:
-        corners = self._patch.get_xy().copy()
-        return (corners[:, 0], corners[:, 1])
+        return (0, self.bottom)
 
     @xy.setter
-    def xy(self, xy: Tuple[float]):
-        corners = self._patch.get_xy()
-        corners[:, 1] = xy[1]
-        self._patch.set_xy(corners)
+    def xy(self, value: Tuple[float]):
+        _xy = self._patch.get_xy()
+        if len(_xy) > 2:
+            _xy[:, 1] += value[1] - _xy[0, 1]
+        else:
+            _xy = (0, value[1])
+        self._patch.set_xy(_xy)
         self._update_vertices()
 
+    def set(self, **kwargs):
+        super().set(**kwargs)
+        self._median.set(**kwargs)
+
 
 Hspans = partial(Tool, spawner=Hspan)
 Hspans.__doc__ = """
 Hspans: Add horizontal spans to the supplied axes.
 
 Controls:
   - Left-click and hold to make new spans
```

### Comparing `mpltoolbox-24.5.0/src/mpltoolbox/lines.py` & `mpltoolbox-24.5.1/src/mpltoolbox/lines.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/src/mpltoolbox/patch.py` & `mpltoolbox-24.5.1/src/mpltoolbox/patch.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,17 @@
         hide_vertices: bool = False,
         **kwargs,
     ):
         self._max_clicks = 2
         self._ax = ax
         kwargs = parse_kwargs(kwargs, number)
         defaut_color = f"C{number}"
-        if set(["ec", "edgecolor"]).isdisjoint(set(kwargs.keys())):
+        if {"ec", "edgecolor"}.isdisjoint(set(kwargs.keys())):
             kwargs["ec"] = defaut_color
-        if set(["fc", "facecolor"]).isdisjoint(set(kwargs.keys())):
+        if {"fc", "facecolor"}.isdisjoint(set(kwargs.keys())):
             kwargs["fc"] = to_rgb(defaut_color) + (0.05,)
         self._make_patch(x=x, y=y, **kwargs)
         (self._vertices,) = self._ax.plot(
             *self._make_vertices(), "o", ls="None", mec=self.edgecolor, mfc="None"
         )
         if hide_vertices:
             self._vertices.set_visible(False)
@@ -89,14 +89,18 @@
         self._patch.update(kwargs)
         self._update_vertices()
 
     @property
     def vertices(self):
         return self._vertices.get_data()
 
+    def set(self, **kwargs):
+        self._patch.set(**kwargs)
+        self._vertices.set(**kwargs)
+
     def set_picker(self, pick: float):
         self._patch.set_picker(pick)
         self._vertices.set_picker(pick)
 
     def is_moveable(self, artist: Artist) -> bool:
         return artist is self._vertices
```

### Comparing `mpltoolbox-24.5.0/src/mpltoolbox/points.py` & `mpltoolbox-24.5.1/src/mpltoolbox/points.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/src/mpltoolbox/polygons.py` & `mpltoolbox-24.5.1/src/mpltoolbox/polygons.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/src/mpltoolbox/rectangles.py` & `mpltoolbox-24.5.1/src/mpltoolbox/rectangles.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/src/mpltoolbox/tool.py` & `mpltoolbox-24.5.1/src/mpltoolbox/tool.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/src/mpltoolbox/vspans.py` & `mpltoolbox-24.5.1/src/mpltoolbox/vspans.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,29 +16,28 @@
         y: float,
         number: int,
         ax: Axes,
         hide_median: bool = False,
         **kwargs,
     ):
         super().__init__(x=x, y=y, number=number, ax=ax, **kwargs)
-        self._vertices.set_transform(self._patch.get_transform())
         self._median = self._ax.axvline(x, ls="dashed", color=self.edgecolor)
+        self._vertices.set_transform(self._median.get_transform())
         if hide_median:
             self._median.set_visible(False)
 
     def __repr__(self):
         return (
             f"VSpan: left={self.left}, right={self.right}, "
             f"edgecolor={self.edgecolor}, facecolor={self.facecolor}"
         )
 
     def _update_vertices(self):
         super()._update_vertices()
-        corners = self._patch.get_xy()
-        mid = 0.5 * (corners[0, 0] + corners[2, 0])
+        mid = 0.5 * (self.left + self.right)
         self._median.set_xdata([mid, mid])
 
     def _make_patch(self, x: float, y: float, **kwargs):
         self._patch = self._ax.axvspan(x, x, **kwargs)
 
     def _make_vertices(self) -> Tuple[float]:
         return ([self.left, self.right], [0.5, 0.5])
@@ -52,57 +51,77 @@
 
     def remove(self):
         super().remove()
         self._median.remove()
 
     @property
     def left(self) -> float:
-        return self._patch.get_xy()[0, 0]
+        xy = self._patch.get_xy()
+        if len(xy) > 2:
+            return xy[0, 0]
+        return xy[0]
 
     @left.setter
     def left(self, x: float):
-        corners = self._patch.get_xy()
-        for i in [0, 1]:
-            corners[i, 0] = x
-        if len(corners) > 3:
-            corners[4, 0] = x
+        xy = self._patch.get_xy()
+        if len(xy) > 2:
+            for i in [0, 1]:
+                xy[i, 0] = x
+            if len(xy) > 3:
+                xy[4, 0] = x
+            else:
+                xy += [x, xy[0, 1]]
+            self._patch.set_xy(xy)
         else:
-            corners += [x, corners[0, 1]]
-        self._patch.set_xy(corners)
+            self._patch.set(width=xy[0] - x + self.width, xy=(x, 0))
         self._update_vertices()
 
     @property
     def right(self) -> float:
-        return self._patch.get_xy()[2, 0]
+        xy = self._patch.get_xy()
+        if len(xy) > 2:
+            return xy[2, 0]
+        return xy[0] + self.width
 
     @right.setter
     def right(self, x: float):
-        corners = self._patch.get_xy()
-        for i in [2, 3]:
-            corners[i, 0] = x
-        self._patch.set_xy(corners)
+        xy = self._patch.get_xy()
+        if len(xy) > 2:
+            for i in [2, 3]:
+                xy[i, 0] = x
+            self._patch.set_xy(xy)
+        else:
+            self._patch.set_width(x - xy[0])
         self._update_vertices()
 
     @property
     def width(self) -> float:
+        if hasattr(self._patch, "get_width"):
+            return self._patch.get_width()
         corners = self._patch.get_xy()
         return corners[2, 0] - corners[0, 0]
 
     @property
     def xy(self) -> Tuple[float]:
-        corners = self._patch.get_xy().copy()
-        return (corners[:, 0], corners[:, 1])
+        return (self.left, 0)
 
     @xy.setter
-    def xy(self, xy: Tuple[float]):
-        corners = self._patch.get_xy()
-        corners[:, 0] = xy[0]
-        self._patch.set_xy(corners)
+    def xy(self, value: Tuple[float]):
+        _xy = self._patch.get_xy()
+        if len(_xy) > 2:
+            _xy[:, 0] += value[0] - _xy[0, 0]
+        else:
+            _xy = (value[0], 0)
+        self._patch.set_xy(_xy)
         self._update_vertices()
 
+    def set(self, **kwargs):
+        super().set(**kwargs)
+        self._median.set(**kwargs)
+
 
 Vspans = partial(Tool, spawner=Vspan)
 Vspans.__doc__ = """
 Vspans: Add vertical spans to the supplied axes.
 
 Controls:
   - Left-click and hold to make new spans
```

### Comparing `mpltoolbox-24.5.0/src/mpltoolbox.egg-info/PKG-INFO` & `mpltoolbox-24.5.1/src/mpltoolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpltoolbox
-Version: 24.5.0
+Version: 24.5.1
 Summary: Interactive tools for matplotlib
 Home-page: https://github.com/scipp/mpltoolbox
 Author: Neil Vaytet
 Author-email: neil.vaytet@esss.se
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/mpltoolbox/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mpltoolbox-24.5.0/src/mpltoolbox.egg-info/SOURCES.txt` & `mpltoolbox-24.5.1/src/mpltoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/tests/conftest.py` & `mpltoolbox-24.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/tests/lines_test.py` & `mpltoolbox-24.5.1/tests/lines_test.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.5.0/tests/points_test.py` & `mpltoolbox-24.5.1/tests/points_test.py`

 * *Files identical despite different names*

