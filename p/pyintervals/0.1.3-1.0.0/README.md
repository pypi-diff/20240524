# Comparing `tmp/pyintervals-0.1.3.tar.gz` & `tmp/pyintervals-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyintervals-0.1.3.tar", max compression
+gzip compressed data, was "pyintervals-1.0.0.tar", max compression
```

## Comparing `pyintervals-0.1.3.tar` & `pyintervals-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0      167 2023-10-04 16:33:27.887011 pyintervals-0.1.3/CHANGELOG.rst
--rw-r--r--   0        0        0     1085 2023-10-04 04:47:43.408222 pyintervals-0.1.3/LICENSE
--rw-r--r--   0        0        0     5890 2023-10-12 10:58:24.254230 pyintervals-0.1.3/README.rst
--rw-r--r--   0        0        0     1436 2023-10-12 10:59:51.648712 pyintervals-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      248 2023-10-12 10:57:11.879727 pyintervals-0.1.3/src/pyintervals/__init__.py
--rw-r--r--   0        0        0     2156 2023-10-12 10:57:11.883552 pyintervals-0.1.3/src/pyintervals/interval.py
--rw-r--r--   0        0        0        0 2023-10-12 10:57:11.883864 pyintervals-0.1.3/src/pyintervals/py.typed
--rw-r--r--   0        0        0     6856 1970-01-01 00:00:00.000000 pyintervals-0.1.3/setup.py
--rw-r--r--   0        0        0     6802 1970-01-01 00:00:00.000000 pyintervals-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      278 2023-10-12 11:11:19.665215 pyintervals-1.0.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1085 2023-10-04 04:47:43.408222 pyintervals-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5888 2024-05-24 18:25:58.313277 pyintervals-1.0.0/README.rst
+-rw-r--r--   0        0        0     1553 2024-05-24 18:25:58.316928 pyintervals-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      381 2024-05-05 14:26:01.917644 pyintervals-1.0.0/src/pyintervals/__init__.py
+-rw-r--r--   0        0        0      110 2024-05-05 14:26:01.921345 pyintervals-1.0.0/src/pyintervals/constants.py
+-rw-r--r--   0        0        0     2369 2024-05-05 14:26:01.932591 pyintervals-1.0.0/src/pyintervals/interval.py
+-rw-r--r--   0        0        0     3108 2024-05-05 14:26:01.933982 pyintervals-1.0.0/src/pyintervals/interval_handler.py
+-rw-r--r--   0        0        0        0 2023-10-12 10:57:11.883864 pyintervals-1.0.0/src/pyintervals/py.typed
+-rw-r--r--   0        0        0     1111 2024-05-05 14:26:01.965880 pyintervals-1.0.0/src/pyintervals/search.py
+-rw-r--r--   0        0        0     3827 2024-05-05 14:26:01.970198 pyintervals-1.0.0/src/pyintervals/time_value_node.py
+-rw-r--r--   0        0        0     6803 1970-01-01 00:00:00.000000 pyintervals-1.0.0/PKG-INFO
```

### Comparing `pyintervals-0.1.3/LICENSE` & `pyintervals-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyintervals-0.1.3/README.rst` & `pyintervals-1.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -129,16 +129,16 @@
 
 ✅ = implemented, 🚧 = planned, ❌ = not planned
 
 - Fundamentals:
     - ✅ Overlap controls
     - ✅ Contain controls
 - Interval Handler:
-    - 🚧 Own intervals with associated values
-    - 🚧 Provide value projection graph
+    - ✅ Own intervals with associated values
+    - ✅ Provide value projection graph
     - 🚧 Query value over time
     - 🚧 Access intervals overlapping with a specific timespan
 - Single-level Pegging:
     - 🚧 Introduce object association to Intervals
     - 🚧 Single level pegging with first-in-first-out
     - 🚧 Enable callback for pegging quantity
     - 🚧 Enable callback for pegging matching
```

### Comparing `pyintervals-0.1.3/pyproject.toml` & `pyintervals-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "pyintervals"
-version = "0.1.3"
+version = "1.0.0"
 description = "Efficient interval operations."
 authors = ["Serkan Kalay <serkanosmankalay@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 readme = "README.rst"
 packages = [
     {include = "pyintervals", from = "src"},
     {include = "pyintervals/py.typed", from = "src"}
 ]
 include = ["CHANGELOG.rst", "README.rst"]
@@ -21,25 +22,27 @@
     "interval",
     "timespan",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<4.0"
 importlib-metadata = {version = ">=1,<5", python = "<3.8"}
+sortedcontainers = "^2.4.0"
+sortedcontainers-stubs = "^2.4.2"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.0.1"
-pytest-cov = "^4.0.0"
+pytest = ">=7.0.1,<9.0.0"
+pytest-cov = ">=4,<6"
 pytest-benchmark = "^4.0.0"
 
 [tool.poetry.group.typecheck.dependencies]
-mypy = ">=0.982,<1.7"
+mypy = ">=0.982,<1.11"
 
 [tool.poetry.group.linting.dependencies]
-black = ">=22.10,<24.0"
+black = ">=22.10,<25.0"
 flake8 = ">=5.0.4,<7.0.0"
 isort = "^5.7.0"
 
 [tool.poetry.group.dev.dependencies]
 tox = ">=3.26,<5.0"
 
 [tool.black]
```

### Comparing `pyintervals-0.1.3/setup.py` & `pyintervals-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,182 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyintervals
+Version: 1.0.0
+Summary: Efficient interval operations.
+Home-page: https://github.com/serkankalay/pyintervals
+License: MIT
+Keywords: interval,timespan
+Author: Serkan Kalay
+Author-email: serkanosmankalay@gmail.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.8
+Requires-Dist: importlib-metadata (>=1,<5) ; python_version < "3.8"
+Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
+Requires-Dist: sortedcontainers-stubs (>=2.4.2,<3.0.0)
+Project-URL: Repository, https://github.com/serkankalay/pyintervals
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': 'src'}
+📐 pyintervals
+===============================
 
-packages = \
-['pyintervals']
+.. image:: https://img.shields.io/pypi/v/pyintervals.svg?style=flat-square&color=blue
+   :target: https://pypi.python.org/pypi/pyintervals
 
-package_data = \
-{'': ['*']}
-
-modules = \
-['py']
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata>=1,<5']}
-
-setup_kwargs = {
-    'name': 'pyintervals',
-    'version': '0.1.3',
-    'description': 'Efficient interval operations.',
-    'long_description': "📐 pyintervals\n===============================\n\n.. image:: https://img.shields.io/pypi/v/pyintervals.svg?style=flat-square&color=blue\n   :target: https://pypi.python.org/pypi/pyintervals\n\n.. image:: https://img.shields.io/pypi/pyversions/pyintervals.svg?style=flat-square\n   :target: https://pypi.python.org/pypi/pyintervals\n\n.. image:: https://img.shields.io/pypi/l/pyintervals.svg?style=flat-square&color=blue\n   :target: https://pypi.python.org/pypi/pyintervals\n\n.. image:: https://img.shields.io/badge/mypy-strict-forestgreen?style=flat-square\n   :target: https://mypy.readthedocs.io/en/stable/command_line.html#cmdoption-mypy-strict\n\n.. image:: https://img.shields.io/badge/coverage-99%25-forestgreen?style=flat-square\n   :target: https://github.com/serkankalay/pyintervals\n\n.. image::  https://img.shields.io/github/actions/workflow/status/serkankalay/pyintervals/tests.yml?branch=master&style=flat-square\n   :target: https://github.com/serkankalay/pyintervals\n\n**Execute efficient interval operations in Python.**\n\n*(Currently in active development. Leave a* ⭐️ *on GitHub if you're interested how this develops!)*\n\nWhy?\n--------\n\nInspired by a discussion and initial implementation in a professional project\nand a library I've been using in one of my previous jobs, **pyintervals** is born.\n\nIntervals pop-up frequently in programming, specifically in domains where you\nhave an activity or a proxy for it.\n\n- Suppose you are implementing a single machine scheduling algorithm.\n  In order to schedule an operation, you need to makes sure that the machine is available\n  during your desired time of operation.\n- Or you are implementing a booking system and need to check\n  that the hotel has at least 1 room with desired number of beds for the dates selected.\n  For such cases, you need to control some information overlapping with an interval.\n\nAs the examples suggest, **pyintervals** defines intervals with date and time.\nHowever, adding support for other comparable types such as ``int``, ``float`` is also possible.\n\nHow?\n--------\n\nDeclare ``Interval`` objects with **pyintervals** and check whether they ``overlap`` with each other or\none ``contains`` the other.\n\n.. code-block:: python\n\n  from pyintervals import Interval, overlaps, contains\n  from datetime import datetime\n\n  my_first_interval = Interval(start=datetime(2017,5,20,12,15),end=datetime(2024,10,10,19,0))\n  my_second_interval = Interval(start=datetime(2024,10,6,7,21),end=datetime(2024,10,10,19,0))\n\n  overlaps(my_first_interval, my_second_interval)\n  >>> True\n\n  my_first_interval.overlaps_with(my_second_interval)\n  >>> True\n\n  contains(my_first_interval, my_second_interval)\n  >>> True\n\n  my_first_interval.contains(my_second_interval)\n  >>> True\n\n  my_third_interval=Interval(start=datetime(1988,5,21,10,45),end=datetime(1989,6,20,1,30))\n  overlaps(my_first_interval,my_third_interval)\n  >>> False\n\n  contains(my_first_interval,my_third_interval)\n  >>> False\n\n**pyintervals** also support `degenerate` intervals, which have their ``start`` equal to their ``end``.\n\n.. code-block:: python\n\n  my_degenerate_interval = Interval(start=datetime(2024,10,10,9,0), end=datetime(2024,10,10,9,0))\n\n  overlaps(my_first_interval, my_degenerate_interval)\n  >>> True\n\n  my_same_degenerate_interval = Interval(start=datetime(2024,10,10,9,0), end=datetime(2024,10,10,9,0))\n\n  overlaps(my_degenerate_interval, my_same_degenerate_interval)\n  >>> True\n\nWhat else?\n-----------\n\nInterval concept also leads to `aggregate value over time`. Let's dive with an example:\n\nLet there be a beautiful and exclusive patisserie and you heard it from a foodie friend.\nShe/he suggested you to go there as soon as possible.\nYou checked your agenda and seems you have an empty spot at your calendar starting at 12:30.\nThe place is open between 9:00-12:00 and 13:00 - 16:00 daily.\n\nIf you want to programatically check whether the shop is open at a given time **T**, then\nyou need to iterate over `all (in the worst case)` the time intervals the patisserie is open\nfor the time you are curious about, 12:30 in this case. This will take `O(n)` time.\n\nLinear time is nice but can we not improve it? Well, with **pyintervals**, you can! `(with an upcoming feature)`\nWhat we essentially are curious about is the status of that beautiful store at a given time.\n**pintervals** `will` allow you fetch this value in `O(log n)` time.\n\nSee roadmap_ for the list of available and upcoming features.\n\nWhen?\n---------\n\nStart with **pyintervals** right away with\n\n.. code-block:: bash\n\n  pip install pyintervals\n\n.. _roadmap:\n\nRoadmap\n---------\n**pyintervals** is in active development and not feature complete yet. Please see below\nfor completed and planned features.\n\nFeatures:\n\n✅ = implemented, 🚧 = planned, ❌ = not planned\n\n- Fundamentals:\n    - ✅ Overlap controls\n    - ✅ Contain controls\n- Interval Handler:\n    - 🚧 Own intervals with associated values\n    - 🚧 Provide value projection graph\n    - 🚧 Query value over time\n    - 🚧 Access intervals overlapping with a specific timespan\n- Single-level Pegging:\n    - 🚧 Introduce object association to Intervals\n    - 🚧 Single level pegging with first-in-first-out\n    - 🚧 Enable callback for pegging quantity\n    - 🚧 Enable callback for pegging matching\n- Support other comparable types\n    - 🚧 Define comparable protocol and generics\n    - 🚧 Adapt Interval and Interval Handler concepts\n\nAcknowledgements\n----------------\n\nFollowing resources and people have inspired **pyintervals**:\n\n- `Always use [closed, open) intervals <https://fhur.me/posts/always-use-closed-open-intervalshttps://fhur.me/posts/always-use-closed-open-intervals>`_\n- `Arie Bovenberg <https://github.com/ariebovenberg>`_\n- `pdfje (for initial setup of this project) <https://github.com/ariebovenberg/pdfje>`_\n- `Sam de Wringer <https://github.com/samdewr>`_\n- Tim Lamballais-Tessensohn\n",
-    'author': 'Serkan Kalay',
-    'author_email': 'serkanosmankalay@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/serkankalay/pyintervals',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'py_modules': modules,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8.1,<4.0.0',
-}
+.. image:: https://img.shields.io/pypi/pyversions/pyintervals.svg?style=flat-square
+   :target: https://pypi.python.org/pypi/pyintervals
 
+.. image:: https://img.shields.io/pypi/l/pyintervals.svg?style=flat-square&color=blue
+   :target: https://pypi.python.org/pypi/pyintervals
+
+.. image:: https://img.shields.io/badge/mypy-strict-forestgreen?style=flat-square
+   :target: https://mypy.readthedocs.io/en/stable/command_line.html#cmdoption-mypy-strict
+
+.. image:: https://img.shields.io/badge/coverage-99%25-forestgreen?style=flat-square
+   :target: https://github.com/serkankalay/pyintervals
+
+.. image::  https://img.shields.io/github/actions/workflow/status/serkankalay/pyintervals/tests.yml?branch=master&style=flat-square
+   :target: https://github.com/serkankalay/pyintervals
+
+**Execute efficient interval operations in Python.**
+
+*(Currently in active development. Leave a* ⭐️ *on GitHub if you're interested how this develops!)*
+
+Why?
+--------
+
+Inspired by a discussion and initial implementation in a professional project
+and a library I've been using in one of my previous jobs, **pyintervals** is born.
+
+Intervals pop-up frequently in programming, specifically in domains where you
+have an activity or a proxy for it.
+
+- Suppose you are implementing a single machine scheduling algorithm.
+  In order to schedule an operation, you need to makes sure that the machine is available
+  during your desired time of operation.
+- Or you are implementing a booking system and need to check
+  that the hotel has at least 1 room with desired number of beds for the dates selected.
+  For such cases, you need to control some information overlapping with an interval.
+
+As the examples suggest, **pyintervals** defines intervals with date and time.
+However, adding support for other comparable types such as ``int``, ``float`` is also possible.
+
+How?
+--------
+
+Declare ``Interval`` objects with **pyintervals** and check whether they ``overlap`` with each other or
+one ``contains`` the other.
+
+.. code-block:: python
+
+  from pyintervals import Interval, overlaps, contains
+  from datetime import datetime
+
+  my_first_interval = Interval(start=datetime(2017,5,20,12,15),end=datetime(2024,10,10,19,0))
+  my_second_interval = Interval(start=datetime(2024,10,6,7,21),end=datetime(2024,10,10,19,0))
+
+  overlaps(my_first_interval, my_second_interval)
+  >>> True
+
+  my_first_interval.overlaps_with(my_second_interval)
+  >>> True
+
+  contains(my_first_interval, my_second_interval)
+  >>> True
+
+  my_first_interval.contains(my_second_interval)
+  >>> True
+
+  my_third_interval=Interval(start=datetime(1988,5,21,10,45),end=datetime(1989,6,20,1,30))
+  overlaps(my_first_interval,my_third_interval)
+  >>> False
+
+  contains(my_first_interval,my_third_interval)
+  >>> False
+
+**pyintervals** also support `degenerate` intervals, which have their ``start`` equal to their ``end``.
+
+.. code-block:: python
+
+  my_degenerate_interval = Interval(start=datetime(2024,10,10,9,0), end=datetime(2024,10,10,9,0))
+
+  overlaps(my_first_interval, my_degenerate_interval)
+  >>> True
+
+  my_same_degenerate_interval = Interval(start=datetime(2024,10,10,9,0), end=datetime(2024,10,10,9,0))
+
+  overlaps(my_degenerate_interval, my_same_degenerate_interval)
+  >>> True
+
+What else?
+-----------
+
+Interval concept also leads to `aggregate value over time`. Let's dive with an example:
+
+Let there be a beautiful and exclusive patisserie and you heard it from a foodie friend.
+She/he suggested you to go there as soon as possible.
+You checked your agenda and seems you have an empty spot at your calendar starting at 12:30.
+The place is open between 9:00-12:00 and 13:00 - 16:00 daily.
+
+If you want to programatically check whether the shop is open at a given time **T**, then
+you need to iterate over `all (in the worst case)` the time intervals the patisserie is open
+for the time you are curious about, 12:30 in this case. This will take `O(n)` time.
+
+Linear time is nice but can we not improve it? Well, with **pyintervals**, you can! `(with an upcoming feature)`
+What we essentially are curious about is the status of that beautiful store at a given time.
+**pintervals** `will` allow you fetch this value in `O(log n)` time.
+
+See roadmap_ for the list of available and upcoming features.
+
+When?
+---------
+
+Start with **pyintervals** right away with
+
+.. code-block:: bash
+
+  pip install pyintervals
+
+.. _roadmap:
+
+Roadmap
+---------
+**pyintervals** is in active development and not feature complete yet. Please see below
+for completed and planned features.
+
+Features:
+
+✅ = implemented, 🚧 = planned, ❌ = not planned
+
+- Fundamentals:
+    - ✅ Overlap controls
+    - ✅ Contain controls
+- Interval Handler:
+    - ✅ Own intervals with associated values
+    - ✅ Provide value projection graph
+    - 🚧 Query value over time
+    - 🚧 Access intervals overlapping with a specific timespan
+- Single-level Pegging:
+    - 🚧 Introduce object association to Intervals
+    - 🚧 Single level pegging with first-in-first-out
+    - 🚧 Enable callback for pegging quantity
+    - 🚧 Enable callback for pegging matching
+- Support other comparable types
+    - 🚧 Define comparable protocol and generics
+    - 🚧 Adapt Interval and Interval Handler concepts
+
+Acknowledgements
+----------------
+
+Following resources and people have inspired **pyintervals**:
+
+- `Always use [closed, open) intervals <https://fhur.me/posts/always-use-closed-open-intervalshttps://fhur.me/posts/always-use-closed-open-intervals>`_
+- `Arie Bovenberg <https://github.com/ariebovenberg>`_
+- `pdfje (for initial setup of this project) <https://github.com/ariebovenberg/pdfje>`_
+- `Sam de Wringer <https://github.com/samdewr>`_
+- Tim Lamballais-Tessensohn
 
-setup(**setup_kwargs)
```

