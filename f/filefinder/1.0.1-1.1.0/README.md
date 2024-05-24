# Comparing `tmp/filefinder-1.0.1.tar.gz` & `tmp/filefinder-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filefinder-1.0.1.tar", last modified: Wed Apr 24 23:01:11 2024, max compression
+gzip compressed data, was "filefinder-1.1.0.tar", last modified: Fri May 24 17:51:48 2024, max compression
```

## Comparing `filefinder-1.0.1.tar` & `filefinder-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:11.856098 filefinder-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 23:01:07.000000 filefinder-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-24 23:01:07.000000 filefinder-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-24 23:01:11.856098 filefinder-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-24 23:01:07.000000 filefinder-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-24 23:01:07.000000 filefinder-1.0.1/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-24 23:01:07.000000 filefinder-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 23:01:11.856098 filefinder-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:11.852098 filefinder-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:11.852098 filefinder-1.0.1/src/filefinder/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 23:01:07.000000 filefinder-1.0.1/src/filefinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19135 2024-04-24 23:01:07.000000 filefinder-1.0.1/src/filefinder/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-04-24 23:01:07.000000 filefinder-1.0.1/src/filefinder/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-04-24 23:01:07.000000 filefinder-1.0.1/src/filefinder/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-24 23:01:07.000000 filefinder-1.0.1/src/filefinder/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-04-24 23:01:07.000000 filefinder-1.0.1/src/filefinder/matches.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:07.000000 filefinder-1.0.1/src/filefinder/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:11.852098 filefinder-1.0.1/src/filefinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-24 23:01:11.000000 filefinder-1.0.1/src/filefinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-24 23:01:11.000000 filefinder-1.0.1/src/filefinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:01:11.000000 filefinder-1.0.1/src/filefinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 23:01:11.000000 filefinder-1.0.1/src/filefinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 23:01:11.000000 filefinder-1.0.1/src/filefinder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:51:48.502229 filefinder-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-24 17:51:44.000000 filefinder-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-24 17:51:44.000000 filefinder-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-24 17:51:48.502229 filefinder-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-24 17:51:44.000000 filefinder-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-24 17:51:44.000000 filefinder-1.1.0/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-24 17:51:44.000000 filefinder-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 17:51:48.502229 filefinder-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:51:48.498229 filefinder-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:51:48.498229 filefinder-1.1.0/src/filefinder/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-24 17:51:44.000000 filefinder-1.1.0/src/filefinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20992 2024-05-24 17:51:44.000000 filefinder-1.1.0/src/filefinder/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-05-24 17:51:44.000000 filefinder-1.1.0/src/filefinder/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-05-24 17:51:44.000000 filefinder-1.1.0/src/filefinder/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-24 17:51:44.000000 filefinder-1.1.0/src/filefinder/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-24 17:51:44.000000 filefinder-1.1.0/src/filefinder/matches.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 17:51:44.000000 filefinder-1.1.0/src/filefinder/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:51:48.498229 filefinder-1.1.0/src/filefinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-24 17:51:48.000000 filefinder-1.1.0/src/filefinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-24 17:51:48.000000 filefinder-1.1.0/src/filefinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 17:51:48.000000 filefinder-1.1.0/src/filefinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-24 17:51:48.000000 filefinder-1.1.0/src/filefinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 17:51:48.000000 filefinder-1.1.0/src/filefinder.egg-info/top_level.txt
```

### Comparing `filefinder-1.0.1/LICENSE` & `filefinder-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `filefinder-1.0.1/PKG-INFO` & `filefinder-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filefinder
-Version: 1.0.1
+Version: 1.1.0
 Summary: Find files using a simple syntax.
 Author-email: Clément Haëck <clement.haeck@locean.ipsl.fr>
 Project-URL: Source, https://github.com/Descanonge/filefinder
 Project-URL: Documentation, https://filefinder.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -52,38 +52,38 @@
 - Find corresponding files in a directory (and sub-directories)
 - Parse values from the filenames
 - Select only filenames with specific values
 - Generate filenames
 
 ## Quick examples
 
-The following example will find all files with the structure ``Data/param_[parameter]/Temperature_[date].nc``:
+The following example will find all files with the structure ``Data/param_[parameter]/[year]/Temperature_[date].nc``:
 ``` python
 finder = Finder('/.../Data', 'param_%(parameter:fmt=.1f)/%(Y)/Temperature_%(Y)%(m)%(d).nc')
 files = finder.get_files()
 ```
 
 We can also select only some files, for instance only in january:
 ``` python
-    finder.fix_group('m', 1)
-    files = finder.get_files()
+finder.fix_group('m', 1)
+files = finder.get_files()
 ```
 
 We can retrieve values from found files:
 ``` python
-    filename, matches = finder.files[0]
-    parameter = matches["parameter"]
-    # the date as a datetime object
-    date = filefinder.library.get_date(matches)
+filename, matches = finder.files[0]
+parameter = matches["parameter"]
+# the date as a datetime object
+date = filefinder.library.get_date(matches)
 ```
 
 And we can generate a filename with a set of parameters:
 ``` python
-    finder.make_filename(parameter=0.5, Y=2000, m=1, d=1)
-    # Specifying the month is optional since we already fixed it to 1.
+finder.make_filename(parameter=0.5, Y=2000, m=1, d=1)
+# Specifying the month is optional since we already fixed it to 1.
 ```
 
 ## Requirements
 
 Python >= 3.10
 
 ## Installation
@@ -91,13 +91,19 @@
 From pip:
 ``` sh
 pip install filefinder
 ```
 
 From source:
 ``` sh
+git clone https://github.com/Descanonge/filefinder.git
+cd filefinder
+pip install -e .
+```
+or
+``` sh
 pip install -e https://github.com/Descanonge/filefinder.git#egg=filefinder
 ```
 
 ## Documentation
 
 Documentation is available at [filefinder.readthedocs.io](https://filefinder.readthedocs.io).
```

### Comparing `filefinder-1.0.1/README.md` & `filefinder-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,38 +21,38 @@
 - Find corresponding files in a directory (and sub-directories)
 - Parse values from the filenames
 - Select only filenames with specific values
 - Generate filenames
 
 ## Quick examples
 
-The following example will find all files with the structure ``Data/param_[parameter]/Temperature_[date].nc``:
+The following example will find all files with the structure ``Data/param_[parameter]/[year]/Temperature_[date].nc``:
 ``` python
 finder = Finder('/.../Data', 'param_%(parameter:fmt=.1f)/%(Y)/Temperature_%(Y)%(m)%(d).nc')
 files = finder.get_files()
 ```
 
 We can also select only some files, for instance only in january:
 ``` python
-    finder.fix_group('m', 1)
-    files = finder.get_files()
+finder.fix_group('m', 1)
+files = finder.get_files()
 ```
 
 We can retrieve values from found files:
 ``` python
-    filename, matches = finder.files[0]
-    parameter = matches["parameter"]
-    # the date as a datetime object
-    date = filefinder.library.get_date(matches)
+filename, matches = finder.files[0]
+parameter = matches["parameter"]
+# the date as a datetime object
+date = filefinder.library.get_date(matches)
 ```
 
 And we can generate a filename with a set of parameters:
 ``` python
-    finder.make_filename(parameter=0.5, Y=2000, m=1, d=1)
-    # Specifying the month is optional since we already fixed it to 1.
+finder.make_filename(parameter=0.5, Y=2000, m=1, d=1)
+# Specifying the month is optional since we already fixed it to 1.
 ```
 
 ## Requirements
 
 Python >= 3.10
 
 ## Installation
@@ -60,13 +60,19 @@
 From pip:
 ``` sh
 pip install filefinder
 ```
 
 From source:
 ``` sh
+git clone https://github.com/Descanonge/filefinder.git
+cd filefinder
+pip install -e .
+```
+or
+``` sh
 pip install -e https://github.com/Descanonge/filefinder.git#egg=filefinder
 ```
 
 ## Documentation
 
 Documentation is available at [filefinder.readthedocs.io](https://filefinder.readthedocs.io).
```

### Comparing `filefinder-1.0.1/changelog.md` & `filefinder-1.1.0/changelog.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 
+## v1.1.0
+
+- [2024-05-24] Make matches parsing lazy
+- [2024-05-24] Add filtering functions: by value range and by date range
+- [2024-05-23] Add filtering step: discard files using user-defined functions
+
 # v1.0.0
 
 Major overhaul.
 - Requirement is now python >= 3.10
 - Renamed 'matchers' to 'groups' to be consistent with regex tools.
 - Removed the 'group' spec (no more 'group:name' stuff, a group only has a name now).
 - Group definition is now orderless (rgx, fmt, etc can be specified in any order).
```

### Comparing `filefinder-1.0.1/pyproject.toml` & `filefinder-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Project build file
 
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
-version = '1.0.1'
+version = '1.1.0'
 
 name = 'filefinder'
 authors = [
     {name='Clément Haëck', email='clement.haeck@locean.ipsl.fr'}
 ]
 description = 'Find files using a simple syntax.'
```

### Comparing `filefinder-1.0.1/src/filefinder/finder.py` & `filefinder-1.1.0/src/filefinder/finder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 """Main class."""
 
 # This file is part of the 'filefinder' project
 # (http://github.com/Descanonge/filefinder) and subject
 # to the MIT License as defined in the file 'LICENSE',
 # at the root of this project. © 2021 Clément Haëck
-
+import functools
 import itertools
 import logging
 import os
 import re
-from collections.abc import Sequence
+from collections.abc import Callable, Sequence
 from copy import copy
-from typing import Any
+from typing import Any, Protocol
 
 from filefinder.group import Group, GroupKey
 from filefinder.matches import Matches, get_groups_indices
 
 logger = logging.getLogger(__name__)
 
 
+class _FilterUserFunc(Protocol):
+    """Defines the signature of filters callables (for static type checkers).
+
+    See `<https://mypy.readthedocs.io/en/stable/protocols.html#callback-protocols>`__
+    for details.
+    """
+
+    def __call__(
+        self, __finder: "Finder", filename: str, matches: Matches, **kwargs: Any
+    ) -> bool:
+        ...
+
+
+FilterPartial = Callable[["Finder", str, Matches], bool]
+
+
 class Finder:
     """Find files using a filename pattern.
 
     The Finder object is the main entrance point to this library.
     Given a root directory and a filename pattern, it can search for all
     corresponding files.
 
@@ -74,14 +90,21 @@
         self.scanned: bool = False
         """True if files have been scanned with current parameters.
 
         Is reset to False if the cache (of scanned files) is voided, for instance by
         operation like changing fixed values of groups.
         """
 
+        self.filters: list[FilterPartial] = []
+        """List of filters to apply to found files.
+
+        Each value is a :func:`partial function<functools.partial>` with keyword
+        arguments applied.
+        """
+
         self.set_pattern(pattern)
 
     @property
     def n_groups(self) -> int:
         """Number of groups in pre-regex."""
         return len(self.groups)
 
@@ -426,25 +449,59 @@
         """Return regex."""
         return self._get_regex().replace("/", re.escape(os.sep))
 
     def get_regex_subdirs(self) -> list[str]:
         """Return regexes for each sub-directory."""
         return self._get_regex().split("/")
 
-    def find_files(self):
+    def add_filter(self, func: _FilterUserFunc, **kwargs: Any):
+        """Add a filter with which to select scanned files.
+
+        See :doc:`/filtering` for details.
+
+        :rtype func: Callable
+
+        Parameters
+        ----------
+        func: ~collections.abc.Callable[[Finder, str, Matches, ...], bool]
+            Callable that returns True if the file is to be kept, False otherwise.
+        kwargs
+            Will be passed to the function when executed.
+        """
+        filt = functools.partial(func, **kwargs)
+        self.filters.append(filt)
+        self._apply_filters(filt)
+
+    def clear_filters(self) -> None:
+        """Remove all filters."""
+        self.filters.clear()
+        self._void_cache()
+
+    def _apply_filters(self, filter: FilterPartial | None = None) -> None:
+        filters = [filter] if filter is not None else self.filters
+        kept_files = []
+        for filename, matches in self._files:
+            if all(filt(self, filename, matches) for filt in filters):
+                kept_files.append((filename, matches))
+        self._files = kept_files
+
+    def find_files(self) -> None:
         """Find files to scan and store them.
 
-        Is automatically called when accessing :attr:`files` or :func:`get_files`. Sort
-        files alphabetically.
+        Is automatically called when accessing :attr:`files` or :func:`get_files`. Apply
+        all filters and sort files alphabetically.
         """
         if self.scan_everything:
             self._find_files_scan_everything()
         else:
             self._find_files_subdirectories()
 
+        if self.filters:
+            self._apply_filters()
+
         self._files.sort(key=lambda x: x[0])
 
     def _find_files_scan_everything(self) -> None:
         """Find files checking every sub-directory.
 
         Because having to check if a sub-directory matches the pattern is difficult,
         this allows for more exotic patterns where a folder separator can appear in a
```

### Comparing `filefinder-1.0.1/src/filefinder/format.py` & `filefinder-1.1.0/src/filefinder/format.py`

 * *Files identical despite different names*

### Comparing `filefinder-1.0.1/src/filefinder/group.py` & `filefinder-1.1.0/src/filefinder/group.py`

 * *Files identical despite different names*

### Comparing `filefinder-1.0.1/src/filefinder/library.py` & `filefinder-1.1.0/src/filefinder/library.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Functions to retrieve values from filename."""
 
 # This file is part of the 'filefinder' project
 # (http://github.com/Descanonge/filefinder) and subject
 # to the MIT License as defined in the file 'LICENSE',
 # at the root of this project. © 2021 Clément Haëck
 
+import datetime as dt
 import logging
 from collections.abc import Callable
-from datetime import datetime, timedelta
 
+from .finder import Finder
 from .matches import Matches
 
 logger = logging.getLogger(__name__)
 
 
-def get_date(matches: Matches, default_date: dict | None = None) -> datetime:
+def get_date(matches: Matches, default_date: dict | None = None) -> dt.datetime:
     """Retrieve date from matched elements.
 
     If a matcher is *not* found in the filename, it will be replaced by the
     element of the default date argument.
     Matchers that can be used are (in order of increasing priority):
     YBmdjHMSFxX. If two matchers have the same name, the last one in the
     pre-regex will get priority.
@@ -44,15 +45,15 @@
     def process_int(elt: str, name: str) -> dict[str, int]:
         return {name_to_datetime[name]: int(elt)}
 
     def process_month_name(elt: str, name: str) -> dict[str, int]:
         return dict(month=_find_month_number(elt))
 
     def process_doy(elt: str, name: str) -> dict[str, int]:
-        d = datetime(date["year"], 1, 1) + timedelta(days=int(elt) - 1)
+        d = dt.datetime(date["year"], 1, 1) + dt.timedelta(days=int(elt) - 1)
         return dict(month=d.month, day=d.day)
 
     date = {"year": 1970, "month": 1, "day": 1, "hour": 0, "minute": 0, "second": 0}
 
     if default_date is None:
         default_date = {}
     date.update(default_date)
@@ -91,15 +92,15 @@
             elts["S"] = elt[4:6]
 
     # Process elements
     get_elts(elts, "Ymd", process_int)
     get_elts(elts, "j", process_doy)
     get_elts(elts, "HMS", process_int)
 
-    return datetime(**date)  # type: ignore
+    return dt.datetime(**date)  # type: ignore
 
 
 def _find_month_number(name: str) -> int:
     """Find a month number from its name.
 
     Name can be the full name (January) or its three letter abbreviation (jan).
     The casing does not matter.
@@ -123,7 +124,85 @@
     name = name.lower()
     if name in names:
         return names.index(name) + 1
     if name in names_abbr:
         return names_abbr.index(name) + 1
 
     raise ValueError(f"Could not interpret month name '{name}'")
+
+
+def filter_by_range(
+    finder: Finder,
+    filename: str,
+    matches: Matches,
+    group: str,
+    min: float | None = None,
+    max: float | None = None,
+) -> bool:
+    """Filter filename using the value parsed for `group`.
+
+    Keep filename for which the value parsed for `group` fall within a specific range
+    defined by `min` and `max`.
+
+    Parameters
+    ----------
+    group
+        Name of the group to use the parsed value. The first non-discard group of that
+        name will be used.
+    min
+        If not None, the parsed value must be above this.
+    max
+        If not None, the parsed value mest be below this.
+
+    Raises
+    ------
+    TypeError
+        `min` and `max` cannot be both None.
+    """
+    if min is None and max is None:
+        raise TypeError("`min` and `max` cannot be both None.")
+
+    parsed = matches.get_value(group, parse=True, keep_discard=False)
+
+    if min is not None and parsed < min:
+        return False
+    if max is not None and parsed > max:
+        return False
+    return True
+
+
+def filter_date_range(
+    finder: Finder,
+    filename: str,
+    matches: Matches,
+    start: dt.date | str,
+    stop: dt.date | str,
+    default_date: dict | None = None,
+) -> bool:
+    """Filter filename to be between two dates.
+
+    Parameters
+    ----------
+    start, stop
+        Start and stop dates that define the range of dates to keep. Can each be a
+        :class:`datetime.date` or :class:`datetime.datetime` object; or a string in
+        which case a datetime object is created with
+        :meth:`~datetime.datetime.fromisoformat`.
+    default_date
+        Is passed to :func:`get_date`.
+
+    Returns
+    -------
+    keep
+        True if the file is within the range and must be kept. False otherwise.
+    """
+    if isinstance(start, str):
+        start = dt.datetime.fromisoformat(start)
+    if isinstance(stop, str):
+        stop = dt.datetime.fromisoformat(stop)
+
+    if start >= stop:
+        raise ValueError(f"Start ({start}) must be before stop ({stop})")
+
+    current = get_date(matches, default_date=default_date)
+
+    return start <= current <= stop
```

### Comparing `filefinder-1.0.1/src/filefinder/matches.py` & `filefinder-1.1.0/src/filefinder/matches.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,36 +43,38 @@
 
     def __init__(self, group: Group, match: re.Match, idx: int):
         self.group: Group = group
         self.match_str: str = match.group(idx + 1)
         self.start: int = match.start(idx + 1)
         self.end: int = match.end(idx + 1)
 
-        self.match_parsed: t.Any = None
-        try:
-            self.match_parsed = group.parse(self.match_str)
-        except Exception:
-            logger.debug("Failed to parse for group %s", str(group))
-
     def __repr__(self):
         """Human readable information."""
         return "\n".join([super().__repr__(), self.__str__()])
 
     def __str__(self):
         """Human readable information."""
         return f"{self.group!s} = {self.match_str}"
 
-    def get_match(self, parse: bool = True) -> str | t.Any:
+    @property
+    def match_parsed(self) -> t.Any | None:
+        """Parsed value, None if parsing was not successful."""
+        try:
+            return self.group.parse(self.match_str)
+        except Exception:
+            logger.debug("Failed to parse for group %s", str(self.group))
+            return None
+
+    def get_match(self, parse: bool = True) -> t.Any:
         """Get match string or value.
 
         Parameters
         ----------
         parse:
-            If True (default), and the parsing was successful, return the
-            parsed value instead of the matched string.
+            If True (default) return the parsed value instead of the matched string.
 
         Raises
         ------
         ValueError: Could not parse the match.
         """
         if parse:
             if self.match_parsed is None:
@@ -168,15 +170,15 @@
 
     def __len__(self) -> int:
         """Return number of matches."""
         return len(self.matches)
 
     def get_values(
         self, key: GroupKey, parse: bool = True, keep_discard: bool = False
-    ) -> list[str | t.Any]:
+    ) -> list[t.Any]:
         """Get matched values corresponding to key.
 
         Return a list of values, even if only one group is selected.
 
         Parameters
         ----------
         key:
@@ -189,15 +191,15 @@
         """
         matches = self.get_matches(key, keep_discard=keep_discard)
         values = [m.get_match(parse=parse) for m in matches]
         return values
 
     def get_value(
         self, key: GroupKey, parse: bool = True, keep_discard: bool = False
-    ) -> str | t.Any:
+    ) -> t.Any:
         """Get matched value corresponding to key.
 
         Return a single value. If multiple groups correspond to ``key``,
         the value of the first one to appear in the pattern is returned.
 
         Parameters
         ----------
```

### Comparing `filefinder-1.0.1/src/filefinder.egg-info/PKG-INFO` & `filefinder-1.1.0/src/filefinder.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filefinder
-Version: 1.0.1
+Version: 1.1.0
 Summary: Find files using a simple syntax.
 Author-email: Clément Haëck <clement.haeck@locean.ipsl.fr>
 Project-URL: Source, https://github.com/Descanonge/filefinder
 Project-URL: Documentation, https://filefinder.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -52,38 +52,38 @@
 - Find corresponding files in a directory (and sub-directories)
 - Parse values from the filenames
 - Select only filenames with specific values
 - Generate filenames
 
 ## Quick examples
 
-The following example will find all files with the structure ``Data/param_[parameter]/Temperature_[date].nc``:
+The following example will find all files with the structure ``Data/param_[parameter]/[year]/Temperature_[date].nc``:
 ``` python
 finder = Finder('/.../Data', 'param_%(parameter:fmt=.1f)/%(Y)/Temperature_%(Y)%(m)%(d).nc')
 files = finder.get_files()
 ```
 
 We can also select only some files, for instance only in january:
 ``` python
-    finder.fix_group('m', 1)
-    files = finder.get_files()
+finder.fix_group('m', 1)
+files = finder.get_files()
 ```
 
 We can retrieve values from found files:
 ``` python
-    filename, matches = finder.files[0]
-    parameter = matches["parameter"]
-    # the date as a datetime object
-    date = filefinder.library.get_date(matches)
+filename, matches = finder.files[0]
+parameter = matches["parameter"]
+# the date as a datetime object
+date = filefinder.library.get_date(matches)
 ```
 
 And we can generate a filename with a set of parameters:
 ``` python
-    finder.make_filename(parameter=0.5, Y=2000, m=1, d=1)
-    # Specifying the month is optional since we already fixed it to 1.
+finder.make_filename(parameter=0.5, Y=2000, m=1, d=1)
+# Specifying the month is optional since we already fixed it to 1.
 ```
 
 ## Requirements
 
 Python >= 3.10
 
 ## Installation
@@ -91,13 +91,19 @@
 From pip:
 ``` sh
 pip install filefinder
 ```
 
 From source:
 ``` sh
+git clone https://github.com/Descanonge/filefinder.git
+cd filefinder
+pip install -e .
+```
+or
+``` sh
 pip install -e https://github.com/Descanonge/filefinder.git#egg=filefinder
 ```
 
 ## Documentation
 
 Documentation is available at [filefinder.readthedocs.io](https://filefinder.readthedocs.io).
```

