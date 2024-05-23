# Comparing `tmp/parliamentarch-1.0.tar.gz` & `tmp/parliamentarch-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parliamentarch-1.0.tar", last modified: Sun May 19 16:24:27 2024, max compression
+gzip compressed data, was "parliamentarch-1.0.1.tar", last modified: Thu May 23 22:39:07 2024, max compression
```

## Comparing `parliamentarch-1.0.tar` & `parliamentarch-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:24:27.438959 parliamentarch-1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:24:27.434960 parliamentarch-1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:24:27.438959 parliamentarch-1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-19 16:24:20.000000 parliamentarch-1.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-19 16:24:20.000000 parliamentarch-1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 16:24:20.000000 parliamentarch-1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-19 16:24:20.000000 parliamentarch-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-05-19 16:24:20.000000 parliamentarch-1.0/LISEZMOI.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-05-19 16:24:27.438959 parliamentarch-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-05-19 16:24:20.000000 parliamentarch-1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-19 16:24:20.000000 parliamentarch-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 16:24:27.438959 parliamentarch-1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:24:27.434960 parliamentarch-1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:24:27.438959 parliamentarch-1.0/src/ParliamentArch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-05-19 16:24:27.000000 parliamentarch-1.0/src/ParliamentArch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-19 16:24:27.000000 parliamentarch-1.0/src/ParliamentArch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 16:24:27.000000 parliamentarch-1.0/src/ParliamentArch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 16:24:27.000000 parliamentarch-1.0/src/ParliamentArch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:24:27.438959 parliamentarch-1.0/src/parliamentarch/
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-19 16:24:20.000000 parliamentarch-1.0/src/parliamentarch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-19 16:24:20.000000 parliamentarch-1.0/src/parliamentarch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-19 16:24:20.000000 parliamentarch-1.0/src/parliamentarch/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-19 16:24:20.000000 parliamentarch-1.0/src/parliamentarch/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-19 16:24:20.000000 parliamentarch-1.0/src/parliamentarch/svg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:39:07.085309 parliamentarch-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:39:07.081309 parliamentarch-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:39:07.081309 parliamentarch-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/LISEZMOI.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-05-23 22:39:07.085309 parliamentarch-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:39:07.085309 parliamentarch-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:39:07.081309 parliamentarch-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:39:07.085309 parliamentarch-1.0.1/src/ParliamentArch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-05-23 22:39:07.000000 parliamentarch-1.0.1/src/ParliamentArch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-23 22:39:07.000000 parliamentarch-1.0.1/src/ParliamentArch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:39:07.000000 parliamentarch-1.0.1/src/ParliamentArch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 22:39:07.000000 parliamentarch-1.0.1/src/ParliamentArch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:39:07.085309 parliamentarch-1.0.1/src/parliamentarch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/src/parliamentarch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/src/parliamentarch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/src/parliamentarch/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/src/parliamentarch/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/src/parliamentarch/svg.py
```

### Comparing `parliamentarch-1.0/.github/workflows/python-package.yml` & `parliamentarch-1.0.1/.github/workflows/python-package.yml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.12"]
+        python-version: ["3.11"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `parliamentarch-1.0/.github/workflows/python-publish.yml` & `parliamentarch-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `parliamentarch-1.0/LICENSE` & `parliamentarch-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parliamentarch-1.0/LISEZMOI.rst` & `parliamentarch-1.0.1/LISEZMOI.rst`

 * *Files identical despite different names*

### Comparing `parliamentarch-1.0/PKG-INFO` & `parliamentarch-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParliamentArch
-Version: 1.0
+Version: 1.0.1
 Summary: Generation of arch-styled parliamentary arches
 Author: Gouvernathor
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Gouvernathor
         
         Redistribution and use in source and binary forms, with or without
@@ -29,15 +29,15 @@
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Repository, https://github.com/Gouvernathor/parliamentarch
-Requires-Python: >=3.12
+Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Parliamentarch
 ==============
 
 Utility math functions for the generation of arch-styled parliamentary arches.
@@ -55,14 +55,15 @@
 The result is the hemicycle. Now, to place the seats so that they make the form
 of the hemicycle:
 
 - The hemicycle fits in a 2:1 rectangle, which we will consider in a "landscape"
   orientation, and with the cut diameter being on the bottom (the top left and
   top right corners of the rectangle are empty).
 - The seats will placed in rows, such that:
+
   - The rows are semicircular arcs concentric to the inner and outer arcs.
 
   - The difference between the radii of two consecutive rows is a constant
     called the "row thickness" (radii is the plural of radius).
 
   - The seat are circles (or disks) of equal radius. That radius divided by half
     of the row thickness makes the "seat radius factor".
```

### Comparing `parliamentarch-1.0/README.rst` & `parliamentarch-1.0.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 The result is the hemicycle. Now, to place the seats so that they make the form
 of the hemicycle:
 
 - The hemicycle fits in a 2:1 rectangle, which we will consider in a "landscape"
   orientation, and with the cut diameter being on the bottom (the top left and
   top right corners of the rectangle are empty).
 - The seats will placed in rows, such that:
+
   - The rows are semicircular arcs concentric to the inner and outer arcs.
 
   - The difference between the radii of two consecutive rows is a constant
     called the "row thickness" (radii is the plural of radius).
 
   - The seat are circles (or disks) of equal radius. That radius divided by half
     of the row thickness makes the "seat radius factor".
```

### Comparing `parliamentarch-1.0/src/ParliamentArch.egg-info/PKG-INFO` & `parliamentarch-1.0.1/src/ParliamentArch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParliamentArch
-Version: 1.0
+Version: 1.0.1
 Summary: Generation of arch-styled parliamentary arches
 Author: Gouvernathor
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Gouvernathor
         
         Redistribution and use in source and binary forms, with or without
@@ -29,15 +29,15 @@
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Repository, https://github.com/Gouvernathor/parliamentarch
-Requires-Python: >=3.12
+Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Parliamentarch
 ==============
 
 Utility math functions for the generation of arch-styled parliamentary arches.
@@ -55,14 +55,15 @@
 The result is the hemicycle. Now, to place the seats so that they make the form
 of the hemicycle:
 
 - The hemicycle fits in a 2:1 rectangle, which we will consider in a "landscape"
   orientation, and with the cut diameter being on the bottom (the top left and
   top right corners of the rectangle are empty).
 - The seats will placed in rows, such that:
+
   - The rows are semicircular arcs concentric to the inner and outer arcs.
 
   - The difference between the radii of two consecutive rows is a constant
     called the "row thickness" (radii is the plural of radius).
 
   - The seat are circles (or disks) of equal radius. That radius divided by half
     of the row thickness makes the "seat radius factor".
```

### Comparing `parliamentarch-1.0/src/parliamentarch/__init__.py` & `parliamentarch-1.0.1/src/parliamentarch/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 from inspect import signature
-from io import TextIOBase
 
 from .geometry import get_seats_centers
 from .svg import SeatData, dispatch_seats, get_grouped_svg
 from ._util import filter_kwargs, write_from_get
 
 __all__ = ("get_svg_from_attribution", "write_svg_from_attribution", "SeatData")
 
-_GET_SEATS_CENTERS_PARAM_NAMES = {k for k, p in signature(get_seats_centers).parameters.items() if p.kind==p.KEYWORD_ONLY}
-_WRITE_GROUPED_SVG_PARAM_NAMES = {k for k, p in signature(get_grouped_svg).parameters.items() if p.kind==p.KEYWORD_ONLY}
+_GET_SEATS_CENTERS_PARAM_NAMES = {k: p for k, p in signature(get_seats_centers).parameters.items() if p.kind==p.KEYWORD_ONLY}
+_WRITE_GROUPED_SVG_PARAM_NAMES = {k: p for k, p in signature(get_grouped_svg).parameters.items() if p.kind==p.KEYWORD_ONLY}
 
 def get_svg_from_attribution(attrib: dict[SeatData, int], **kwargs) -> str:
     nseats = sum(attrib.values())
     get_seats_centers_kwargs, write_grouped_svg_kwargs, kwargs = filter_kwargs(_GET_SEATS_CENTERS_PARAM_NAMES, _WRITE_GROUPED_SVG_PARAM_NAMES, **kwargs)
 
     if kwargs:
         raise TypeError("Unknown parameters : " + ", ".join(kwargs))
 
     results = get_seats_centers(nseats, **get_seats_centers_kwargs)
     seat_centers_by_group = dispatch_seats(attrib, sorted(results, key=results.__getitem__, reverse=True))
     return get_grouped_svg(seat_centers_by_group, results.seat_actual_radius, **write_grouped_svg_kwargs)
 
+_sig = signature(get_svg_from_attribution)
+_attrib_param = _sig.parameters["attrib"]
+get_svg_from_attribution.__signature__ = _sig.replace(parameters=(
+    _attrib_param,
+    *_GET_SEATS_CENTERS_PARAM_NAMES.values(),
+    *_WRITE_GROUPED_SVG_PARAM_NAMES.values()
+))
+del _sig, _attrib_param
+
 write_svg_from_attribution = write_from_get(get_svg_from_attribution)
```

### Comparing `parliamentarch-1.0/src/parliamentarch/__main__.py` & `parliamentarch-1.0.1/src/parliamentarch/__main__.py`

 * *Files identical despite different names*

### Comparing `parliamentarch-1.0/src/parliamentarch/_util.py` & `parliamentarch-1.0.1/src/parliamentarch/_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections.abc import Callable, Container, Sequence
 from inspect import Parameter, signature
 from io import TextIOBase
-from typing import NamedTuple
+from typing import NamedTuple, TypeVar
 
 class FactoryDict(dict):
     def __init__(self, default_factory, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.default_factory = default_factory
 
     def __missing__(self, key):
@@ -48,20 +48,23 @@
         if isinstance(file, str):
             with open(file, "w") as f:
                 return write_func(f, *args, **kwargs)
         print(get_func(*args, **kwargs), file=file)
 
     get_sig = signature(get_func)
     write_sig = get_sig.replace(
-        parameters=[_file_parameter] + list(get_sig.parameters.values()))
+        parameters=[_file_parameter] + list(get_sig.parameters.values()),
+        return_annotation=None,
+    )
     write_func.__signature__ = write_sig
     write_func.__name__ = get_func.__name__.replace("get_", "write_")
     return write_func
 
-def filter_kwargs[V](
+V = TypeVar("V") # PY3.11 compat
+def filter_kwargs(
         *sets: Container[str],
         **kwargs: V,
         ) -> list[dict[str, V]]:
     """
     The length of the list is one more than the number of sets passed.
     The sets may actually be any container.
     """
```

### Comparing `parliamentarch-1.0/src/parliamentarch/geometry.py` & `parliamentarch-1.0.1/src/parliamentarch/geometry.py`

 * *Files identical despite different names*

### Comparing `parliamentarch-1.0/src/parliamentarch/svg.py` & `parliamentarch-1.0.1/src/parliamentarch/svg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections.abc import Iterable
 from functools import cached_property
-from io import TextIOBase
 import re
+from typing import TypeVar
 import warnings
 
 from ._util import Color, UnPicklable, write_from_get
 
 __all__ = ("SeatData", "dispatch_seats", "write_svg", "write_grouped_svg", "get_svg", "get_grouped_svg")
 
 class SeatData(UnPicklable):
@@ -35,15 +35,16 @@
                 return c
 
         self.data = data
         self.color = accepted_color(color)
         self.border_size = border_size
         self.border_color = accepted_color(border_color)
 
-def dispatch_seats[S](
+S = TypeVar("S") # PY3.11 compat
+def dispatch_seats(
         group_seats: dict[SeatData, int],
         seats: Iterable[S],
         ) -> dict[SeatData, list[S]]:
     """
     From a dict of groups associating the groups in a given order
     to the number of seats each group has,
     and an iterable of seats in a given order,
```

