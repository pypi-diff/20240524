# Comparing `tmp/tscat-0.2.0.tar.gz` & `tmp/tscat-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tscat-0.2.0.tar", last modified: Tue Nov 29 22:56:37 2022, max compression
+gzip compressed data, was "tscat-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tscat-0.2.0.tar` & `tscat-0.3.0.tar`

### file list

```diff
@@ -1,42 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 22:56:37.000000 tscat-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2022-11-29 22:56:28.000000 tscat-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2022-11-29 22:56:28.000000 tscat-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-11-29 22:56:28.000000 tscat-0.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2022-11-29 22:56:28.000000 tscat-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2022-11-29 22:56:28.000000 tscat-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2022-11-29 22:56:37.000000 tscat-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2022-11-29 22:56:28.000000 tscat-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 22:56:37.000000 tscat-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2022-11-29 22:56:28.000000 tscat-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-11-29 22:56:28.000000 tscat-0.2.0/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4835 2022-11-29 22:56:28.000000 tscat-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-11-29 22:56:28.000000 tscat-0.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-11-29 22:56:28.000000 tscat-0.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      319 2022-11-29 22:56:28.000000 tscat-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2022-11-29 22:56:28.000000 tscat-0.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      767 2022-11-29 22:56:28.000000 tscat-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2022-11-29 22:56:28.000000 tscat-0.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2022-11-29 22:56:28.000000 tscat-0.2.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      438 2022-11-29 22:56:37.000000 tscat-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2022-11-29 22:56:28.000000 tscat-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 22:56:37.000000 tscat-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2022-11-29 22:56:28.000000 tscat-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22618 2022-11-29 22:56:28.000000 tscat-0.2.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9799 2022-11-29 22:56:28.000000 tscat-0.2.0/tests/test_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2022-11-29 22:56:28.000000 tscat-0.2.0/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    16179 2022-11-29 22:56:28.000000 tscat-0.2.0/tests/test_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2022-11-29 22:56:28.000000 tscat-0.2.0/tests/test_mypy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2022-11-29 22:56:28.000000 tscat-0.2.0/tests/test_perf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 22:56:37.000000 tscat-0.2.0/tscat/
--rw-r--r--   0 runner    (1001) docker     (123)    13964 2022-11-29 22:56:28.000000 tscat-0.2.0/tscat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2022-11-29 22:56:28.000000 tscat-0.2.0/tscat/filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 22:56:37.000000 tscat-0.2.0/tscat/orm_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)    11084 2022-11-29 22:56:28.000000 tscat-0.2.0/tscat/orm_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2022-11-29 22:56:28.000000 tscat-0.2.0/tscat/orm_sqlalchemy/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 22:56:37.000000 tscat-0.2.0/tscat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2022-11-29 22:56:37.000000 tscat-0.2.0/tscat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2022-11-29 22:56:37.000000 tscat-0.2.0/tscat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-29 22:56:37.000000 tscat-0.2.0/tscat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-29 22:56:37.000000 tscat-0.2.0/tscat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      178 2022-11-29 22:56:37.000000 tscat-0.2.0/tscat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-11-29 22:56:37.000000 tscat-0.2.0/tscat.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1572 2024-05-24 12:58:45.600963 tscat-0.3.0/LICENSE
+-rw-r--r--   0        0        0      627 2024-05-24 12:58:45.600963 tscat-0.3.0/README.rst
+-rw-r--r--   0        0        0     1673 2024-05-24 12:58:45.604963 tscat-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      597 2024-05-24 12:58:45.604963 tscat-0.3.0/tscat/__init__.py
+-rw-r--r--   0        0        0    14211 2024-05-24 12:58:45.604963 tscat-0.3.0/tscat/base.py
+-rw-r--r--   0        0        0     2875 2024-05-24 12:58:45.604963 tscat-0.3.0/tscat/filtering.py
+-rw-r--r--   0        0        0    14373 2024-05-24 12:58:45.604963 tscat-0.3.0/tscat/import_export.py
+-rw-r--r--   0        0        0    12422 2024-05-24 12:58:45.604963 tscat-0.3.0/tscat/orm_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     3633 2024-05-24 12:58:45.604963 tscat-0.3.0/tscat/orm_sqlalchemy/alembic.ini
+-rw-r--r--   0        0        0     1886 2024-05-24 12:58:45.604963 tscat-0.3.0/tscat/orm_sqlalchemy/migrations/README
+-rw-r--r--   0        0        0     2124 2024-05-24 12:58:45.604963 tscat-0.3.0/tscat/orm_sqlalchemy/migrations/env.py
+-rw-r--r--   0        0        0      635 2024-05-24 12:58:45.604963 tscat-0.3.0/tscat/orm_sqlalchemy/migrations/script.py.mako
+-rw-r--r--   0        0        0     3183 2024-05-24 12:58:45.604963 tscat-0.3.0/tscat/orm_sqlalchemy/migrations/versions/0c057a8951ba_initial_migration.py
+-rw-r--r--   0        0        0      782 2024-05-24 12:58:45.604963 tscat-0.3.0/tscat/orm_sqlalchemy/migrations/versions/9a655086fb51_add_rating_field_to_event.py
+-rw-r--r--   0        0        0     3272 2024-05-24 12:58:45.604963 tscat-0.3.0/tscat/orm_sqlalchemy/orm.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:58:45.604963 tscat-0.3.0/tscat/py.typed
+-rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 tscat-0.3.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tscat-0.2.0/LICENSE` & `tscat-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tscat-0.2.0/PKG-INFO` & `tscat-0.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 Metadata-Version: 2.1
 Name: tscat
-Version: 0.2.0
+Version: 0.3.0
 Summary: A library which stores, loads and filters time-series-events and catalogues.
-Home-page: https://github.com/SciQLop/tscat
-Author: Patrick Boettcher
-Author-email: p@yai.se
-License: GNU General Public License v3
-Description: ======================
-        Time Series Catalogues
-        ======================
-        
-        .. image:: https://github.com/SciQLop/tscat/actions/workflows/test_main.yml/badge.svg
-                :target: https://github.com/pboettch/tscat/actions/workflows/test_main.yml
-        
-        .. image:: https://codecov.io/gh/SciQLop/tscat/branch/main/graph/badge.svg
-                :target: https://codecov.io/gh/SciQLop/tscat
-                :alt: Coverage Status
-        
-        
-        A library which stores, loads and filters time-series-events and associates them catalogues and
-        dynamic catalogues (filter-based).
-        
-        
-        * Free software: GNU General Public License v3
-        * Documentation: https://tscat.readthedocs.io.
-        
-        
-        Features
-        --------
-        
-        * TODO
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.0.0 (2021-07-01)
-        ------------------
-        
-        * First release on PyPI.
-        
-Keywords: tscat
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
+Keywords: satellite,plasma-physics,nasa-data,amda,cdpp,CDF
+Author-email: Patrick Boettcher <p@yai.se>
+Maintainer-email: Patrick Boettcher <p@yai.se>, Alexis Jeandet <alexis.jeandet@member.fsf.org>
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Provides-Extra: dev
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: alembic
+Requires-Dist: typing_extensions>=3.7
+Requires-Dist: sqlalchemy[mypy]<2,>=1.4.0
+Requires-Dist: appdirs>=1.4.4 
+Requires-Dist: SQLAlchemy_Utils>=0.37.8
+Requires-Dist: orjson
+Requires-Dist: astropy
+Requires-Dist: sphinx ; extra == "doc"
+Requires-Dist: sphinx_rtd_theme ; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints ; extra == "doc"
+Requires-Dist: flake8 ; extra == "test"
+Requires-Dist: appdirs-stubs ; extra == "test"
+Requires-Dist: pytest>=4.6.5 ; extra == "test"
+Requires-Dist: pytest ; extra == "test"
+Requires-Dist: pytest-pep8 ; extra == "test"
+Requires-Dist: pytest-cov ; extra == "test"
+Requires-Dist: pytest-timeout ; extra == "test"
+Requires-Dist: ddt ; extra == "test"
+Project-URL: documentation, https://github.com/SciQLop/tscat
+Project-URL: homepage, https://github.com/SciQLop/tscat
+Project-URL: repository, https://github.com/SciQLop/tscat
+Provides-Extra: doc
+Provides-Extra: test
+
+======================
+Time Series Catalogues
+======================
+
+.. image:: https://github.com/SciQLop/tscat/actions/workflows/test_main.yml/badge.svg
+        :target: https://github.com/pboettch/tscat/actions/workflows/test_main.yml
+
+.. image:: https://codecov.io/gh/SciQLop/tscat/branch/main/graph/badge.svg
+        :target: https://codecov.io/gh/SciQLop/tscat
+        :alt: Coverage Status
+
+
+A library which stores, loads and filters time-series-events and associates them catalogues and
+dynamic catalogues (filter-based).
+
+
+* Free software: GNU General Public License v3
+* Documentation: https://tscat.readthedocs.io.
+
```

### Comparing `tscat-0.2.0/tscat/__init__.py` & `tscat-0.3.0/tscat/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,53 @@
-"""Top-level package for Time Series Catalogues."""
-
-__author__ = """Patrick Boettcher"""
-__email__ = 'p@yai.se'
-__version__ = '0.2.0'
-
-from .filtering import Predicate, UUID as UUIDFilter
-
-import json
+import datetime as dt
 import re
-from typing import Dict, List, Union, Tuple, Iterable, Any, TYPE_CHECKING
-from uuid import uuid4, UUID
+from dataclasses import dataclass
+from typing import Any, Dict, Iterable, List, Optional, TYPE_CHECKING, Tuple, Union
+from uuid import UUID, uuid4
 
 from . import orm_sqlalchemy
+from .filtering import Predicate
 
 if TYPE_CHECKING:
     from .orm_sqlalchemy.orm import Event, Catalogue
 
-import datetime as dt
-
 _valid_key = re.compile(r'^[A-Za-z][A-Za-z_0-9]*$')
 
 _backend = None
 
 
 def backend() -> orm_sqlalchemy.Backend:
     global _backend
     if not _backend:  # pragma: no cover
         _backend = orm_sqlalchemy.Backend()  # during tests this line should never be called - this it's uncovered
     return _backend
 
 
 def _listify(v) -> Union[List, Tuple]:
-    if type(v) in [list, tuple]:
+    if isinstance(v, (list, tuple)):
         return v
     else:
         return [v]
 
 
 def _verify_attribute_names(kwargs: Dict) -> Dict:
     for k in kwargs.keys():
         if not _valid_key.match(k):
             raise ValueError('Invalid key-name for event-meta-data in kwargs:', k)
     return kwargs
 
 
 class Session:
-    def __init__(self):
+    def __init__(self) -> None:
         self.entities: List[Union['Event', 'Catalogue']] = []
 
-    def __enter__(self):
+    def __enter__(self) -> 'Session':
         return self
 
-    def __exit__(self, exc_type, exc_value, exc_tb):
+    def __exit__(self, exc_type, exc_value, exc_tb) -> None:
         backend().add_and_flush(self.entities)
 
     def create_event(self, *args: Any, **kwargs: Any) -> '_Event':
         e = _Event(*args, **kwargs)
         self.entities.append(e._backend_entity)
         return e
 
@@ -72,14 +64,17 @@
     @staticmethod
     def remove_events_from_catalogue(catalogue: '_Catalogue', events: Union['_Event', List['_Event']]):
         backend().remove_events_from_catalogue(catalogue._backend_entity,
                                                [event._backend_entity for event in _listify(events)])
 
 
 class _BackendBasedEntity:
+    def __init__(self):
+        self._removed = False
+
     def representation(self, name: str) -> str:
         fix = ', '.join(k + '=' + str(v) for k, v in self.fixed_attributes().items())
         kv = ', '.join(k + '=' + str(v) for k, v in self.variable_attributes().items())
         return f'{name}({fix}) attributes({kv})'
 
     def dump(self) -> dict:
         ret = self.variable_attributes()
@@ -132,43 +127,47 @@
 
         for k in sorted(filter(_valid_key.match, self.__dict__.keys())):
             if self.__dict__[k] != o.__dict__[k]:
                 return False
         return True
 
     def remove(self, permanently: bool = False) -> None:
+        self._removed = True
+
         backend().remove(self._backend_entity, permanently=permanently)
         if permanently:
             del self._backend_entity
 
-    def is_removed(self) -> bool:
-        return backend().is_removed(self._backend_entity)
-
     def restore(self) -> None:
         backend().restore(self._backend_entity)
 
+    def is_removed(self) -> bool:
+        return self._removed
+
 
 class _Event(_BackendBasedEntity):
-    _fixed_keys = ['start', 'stop', 'author', 'uuid', 'tags', 'products']
+    _fixed_keys = ['start', 'stop', 'author', 'uuid', 'tags', 'products', 'rating']
 
     def __init__(self, start: dt.datetime, stop: dt.datetime,
                  author: str,
-                 uuid: str = None,
+                 uuid: Optional[str] = None,
                  tags: Iterable[str] = [],
                  products: Iterable[str] = [],
+                 rating: Optional[int] = None,
                  _insert: bool = True,
                  **kwargs):
         self._in_ctor = True
         super().__init__()
 
         self.start = start
         self.stop = stop
         self.author = author
         self.tags = list(tags)
         self.products = list(products)
+        self.rating = rating
 
         if not uuid:
             self.uuid = str(uuid4())
         else:
             self.uuid = uuid
 
         _verify_attribute_names(kwargs)
@@ -178,14 +177,15 @@
             self._backend_entity = backend().add_event({
                 'start': self.start,
                 'stop': self.stop,
                 'author': self.author,
                 'uuid': self.uuid,
                 'tags': self.tags,
                 'products': self.products,
+                'rating': self.rating,
                 'attributes': kwargs,
             })
 
         self._in_ctor = False
 
     def __setattr__(self, key, value):
         if key == 'uuid':
@@ -193,30 +193,38 @@
         elif key == 'start' and hasattr(self, 'stop'):
             if value > self.stop:
                 raise ValueError("start date has to be before stop date")
         elif key == 'stop' and hasattr(self, 'start'):
             if value < self.start:
                 raise ValueError("stop date has to be after start date")
         elif key in ['tags', 'products']:
-            if any(type(v) != str for v in value):
+            if any(not isinstance(v, str) for v in value):
                 raise ValueError("a tag has to be a string")
+            if any(',' in v for v in value):
+                raise ValueError("a string-list value shall not contain a comma")
+        elif key == 'rating':
+            if value is not None:
+                if not isinstance(value, int):
+                    raise ValueError("rating has to be an integer value")
+                if value < 1 or value > 10:
+                    raise ValueError("rating has to be between 1 and 10")
 
         super(_Event, self).__setattr__(key, value)
 
     def __repr__(self):
         return self.representation('Event')
 
 
 class _Catalogue(_BackendBasedEntity):
     _fixed_keys = ['name', 'author', 'uuid', 'tags', 'predicate']
 
     def __init__(self, name: str, author: str,
-                 uuid: str = None,
+                 uuid: Optional[str] = None,
                  tags: Iterable[str] = [],
-                 predicate: Predicate = None,
+                 predicate: Optional[Predicate] = None,
                  _insert: bool = True,
                  **kwargs):
         self._in_ctor = True
 
         super().__init__()
 
         self.name = name
@@ -251,16 +259,18 @@
     def __setattr__(self, key, value):
         if key == 'uuid':
             UUID(value, version=4)  # throws an exception if not valid
         elif key == 'name':
             if not value:
                 raise ValueError('Catalogue name cannot be emtpy.')
         elif key == 'tags':
-            if any(type(v) != str for v in value):
+            if any(not isinstance(v, str) for v in value):
                 raise ValueError("a tag has to be a string")
+            if any(',' in v for v in value):
+                raise ValueError("a string-list value shall not contain a comma")
 
         super(_Catalogue, self).__setattr__(key, value)
 
     def __repr__(self):
         return self.representation('Catalogue')
 
 
@@ -272,20 +282,20 @@
 def create_catalogue(*args, events: List[_Event] = [], **kwargs) -> _Catalogue:
     with Session() as s:
         c = s.create_catalogue(*args, **kwargs)
         s.add_events_to_catalogue(c, events)
         return c
 
 
-def add_events_to_catalogue(catalogue: _Catalogue, events: List[_Event]) -> None:
+def add_events_to_catalogue(catalogue: _Catalogue, events: Union[_Event, List[_Event]]) -> None:
     with Session() as s:
         s.add_events_to_catalogue(catalogue, events)
 
 
-def remove_events_from_catalogue(catalogue: _Catalogue, events: List[_Event]) -> None:
+def remove_events_from_catalogue(catalogue: _Catalogue, events: Union[_Event, List[_Event]]) -> None:
     with Session() as s:
         s.remove_events_from_catalogue(catalogue, events)
 
 
 def get_catalogues(base: Union[Predicate, _Event, None] = None, removed_items: bool = False) -> List[_Catalogue]:
     base_dict: Dict[str, Union[Predicate, 'Event', None, bool]]
 
@@ -299,125 +309,101 @@
     base_dict.update({'removed': removed_items})
 
     catalogues = []
     for cat in backend().get_catalogues(base_dict):
         c = _Catalogue(cat['name'], cat['author'], cat['uuid'], cat['tags'], cat['predicate'],
                        _insert=False, **cat['attributes'])
         c._backend_entity = cat['entity']
+        c._removed = removed_items
         catalogues += [c]
     return catalogues
 
 
-def get_events(base: Union[Predicate, _Catalogue, None] = None, removed_items: bool = False) -> List[_Event]:
-    base_dict: Dict[str, Union[Predicate, 'Catalogue', None, bool]]
-    if isinstance(base, Predicate):
-        base_dict = {'predicate': base}
-    elif isinstance(base, _Catalogue):
-        base_dict = {'entity': base._backend_entity,
-                     'predicate': base.predicate}
-    else:
-        base_dict = {}
+def __backend_to_event(ev: Dict, removed_item: bool) -> _Event:
+    e = _Event(ev['start'], ev['stop'], ev['author'], ev['uuid'], ev['tags'], ev['products'], ev['rating'],
+               **ev['attributes'], _insert=False)
+    e._removed = removed_item
+    e._backend_entity = ev['entity']
+    return e
 
-    base_dict.update({'removed': removed_items})
 
+def _get_events_from_predicate_or_none(base: Union[Predicate, None], removed_items: bool) -> List[_Event]:
+    base_dict: Dict = {'removed': removed_items}
+    if isinstance(base, Predicate):
+        base_dict.update({'predicate': base})
     events = []
     for ev in backend().get_events(base_dict):
-        e = _Event(ev['start'], ev['stop'], ev['author'], ev['uuid'], ev['tags'], ev['products'],
-                   **ev['attributes'], _insert=False)
-        e._backend_entity = ev['entity']
-        events.append(e)
+        events.append(__backend_to_event(ev, removed_items))
     return events
 
 
-def save() -> None:
-    backend().commit()
-
-
-def discard() -> None:
-    backend().rollback()
-
-
-def has_unsaved_changes() -> bool:
-    return backend().has_unsaved_changes()
-
-
-def export_json(catalogue: _Catalogue) -> str:
-    events = get_events(catalogue)
-
-    events_uuids = [event.uuid for event in events]
-
-    catalogue_dump = catalogue.dump()
-    catalogue_dump.update({"events": events_uuids})
-    export_dict = {
-        'catalogues': [catalogue_dump],
-        'events': [event.dump() for event in events],
-    }
-    return json.dumps(export_dict, default=str)
-
+@dataclass
+class EventQueryInformation:
+    assigned: bool
 
-def canonicalize_json_import(jsons: str) -> dict:
-    import_dict = json.loads(jsons)
 
-    # check events and catalogues for existing entities
-    # if existing and identical - remove from import-dict
-    # if existing and not identical raise
-    # if not existing import
+def _get_events_from_catalogue(base: _Catalogue, removed_items: bool, assigned_only: bool, filtered_only: bool) \
+    -> Tuple[List[_Event], List[EventQueryInformation]]:
+    base_dict = {'entity': base._backend_entity,
+                 'predicate': base.predicate,
+                 'removed': removed_items}
+    if assigned_only:
+        del base_dict['predicate']
+    if filtered_only:
+        del base_dict['entity']
 
+    events = []
+    query_info = []
+    for ev in backend().get_events(base_dict):
+        events.append(__backend_to_event(ev, removed_items))
+        query_info.append(EventQueryInformation(assigned=ev['is_assigned']))
 
-    uuids = [event['uuid'] for event in import_dict['events']]
-    events = backend().get_events_by_uuid_list(uuids)
-
-    for event in import_dict['events'][:]:
-        if event['uuid'] not in events:
-            continue
+    return events, query_info
 
-        check_event = events[event['uuid']]
-        del check_event['entity']
-        check_event.update(check_event['attributes'])
-        del check_event['attributes']
 
-        check_event['start'] = str(check_event['start'])
-        check_event['stop'] = str(check_event['stop'])
+# MultipleDispatch
+def get_events(base: Union[Predicate, _Catalogue, None] = None,
+               removed_items: bool = False,
+               **kwargs: Any) -> Optional[Union[List[_Event], Tuple[List[_Event], List[EventQueryInformation]]]]:
+    """ Get events from the database.
+        If base is a Predicate, all events matching the predicate are returned.
+        If base is a Catalogue, all events in the catalogue are returned.
+        If base is None, all events are returned.
+        If removed_items is True, also removed events are returned.
+        If assigned_only is True, only events that are assigned to a catalogue are returned.
+        If filtered_only is True, only events that are filtered by a catalogue are returned.
+
+        Parameters
+        ----------
+        base: Predicate, Catalogue or None
+            The base for the query (see above)
+        removed_items: bool
+            If True, also removed events are returned
+        assigned_only: bool
+            If True, only events that have been added (assigned) to a catalogue are returned. If a predicate is given
+            this parameter is ignored.
+        filtered_only: bool
+            If True, only events that are filtered (matching the predicate) by the predicate of a
+            catalogue are returned. If a predicate is given this parameter is ignored.
+    """
+    if base is None or isinstance(base, Predicate):
+        return _get_events_from_predicate_or_none(base, removed_items)
+    elif isinstance(base, _Catalogue):
+        return _get_events_from_catalogue(base, removed_items,
+                                          assigned_only=kwargs.get('assigned_only', False),
+                                          filtered_only=kwargs.get('filtered_only', False))
+    else:
+        raise ValueError('base has to be a Predicate, Catalogue or None')  # pragma: no cover
 
-        if check_event != event:
-            raise ValueError(f'Import: event with UUID {event["uuid"]} already exists in database, ' +
-                             'but with different values.')
-        import_dict['events'].remove(event)
 
-    for catalogue in import_dict['catalogues'][:]:
-        check_catalogue = get_catalogues(UUIDFilter(catalogue['uuid']))
-        if len(check_catalogue) != 0:
-            events_uuids = [event.uuid for event in get_events(check_catalogue[0])]
-            catalogue_dump = check_catalogue[0].dump()
-            catalogue_dump.update({'events': events_uuids})
+def save() -> None:
+    backend().commit()
 
-            if catalogue_dump != catalogue:
-                raise ValueError(f'Import: catalogue with UUID {catalogue["uuid"]} already exists in database, ' +
-                                 'but with different values.')
-            import_dict['catalogues'].remove(catalogue)
 
-    return import_dict
+def discard() -> None:
+    backend().rollback()
 
 
-def import_canonicalized_dict(import_dict: dict) -> None:
-    event_of_uuid = {}
+def has_unsaved_changes() -> bool:
+    return backend().has_unsaved_changes()
 
-    # import all new events
-    with Session() as s:
-        for event in import_dict['events']:
-            event['start'] = dt.datetime.fromisoformat(event['start'])
-            event['stop'] = dt.datetime.fromisoformat(event['stop'])
-            event_of_uuid[event['uuid']] = s.create_event(**event)
-
-        for catalogue_dict in import_dict['catalogues']:
-            catalogue_events = [event_of_uuid[uuid] if uuid in event_of_uuid
-                                else get_events(UUIDFilter(uuid))[0]
-                                for uuid in catalogue_dict['events']]
-            del catalogue_dict['events']
-
-            catalogue = s.create_catalogue(**catalogue_dict)
-            s.add_events_to_catalogue(catalogue, catalogue_events)
-
-
-def import_json(jsons: str) -> None:
-    import_dict = canonicalize_json_import(jsons)
-    import_canonicalized_dict(import_dict)
+### Generic Import/Export
```

### Comparing `tscat-0.2.0/tscat/filtering.py` & `tscat-0.3.0/tscat/filtering.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 class UUID(Comparison):
     def __init__(self, uuid_: str):
         uuid.UUID(uuid_, version=4)
         super().__init__('==', Field('uuid'), uuid_)
 
 
 class InCatalogue(Predicate):
-    def __init__(self, catalogue: Union['_Catalogue', None] = None):
+    def __init__(self, catalogue: '_Catalogue'):
         self.catalogue = catalogue
 
     def __repr__(self):
         return f"InCatalogue({self.catalogue})"
 
 
 class PredicateRecursionError(Exception):
```

### Comparing `tscat-0.2.0/tscat/orm_sqlalchemy/__init__.py` & `tscat-0.3.0/tscat/orm_sqlalchemy/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from appdirs import user_data_dir
 
 from typing import Union, List, Dict, Type, Set
 from typing_extensions import Literal
 
 from sqlalchemy import create_engine, and_, or_, not_, event, func, cast, String
 from sqlalchemy.orm import Session, Query
+from sqlalchemy.pool.base import _ConnectionFairy
 
 from operator import __eq__, __ne__, __ge__, __gt__, __le__, __lt__
 
 
 def _serialize_json(obj):
     return orjson.dumps(obj, option=orjson.OPT_NAIVE_UTC).decode('utf-8')
 
@@ -122,37 +123,60 @@
         elif isinstance(pred, In):
             return self._visit_in(pred)
         elif isinstance(pred, InCatalogue):
             return self._visit_in_catalogue(pred)
 
 
 class Backend:
-    def __init__(self, testing=False):
-        if testing:
-            url = 'sqlite://'  # memory database
+    def __init__(self, testing: Union[bool, str] = False):
+        if testing is True:
+            sqlite_filename = ""
+        elif isinstance(testing, str):
+            sqlite_filename = 'file:memdb1?mode=memory&cache=shared'  # memory database
+
         else:  # pragma: no cover
             db_file_path = user_data_dir('tscat')
             if not os.path.exists(db_file_path):
                 os.makedirs(db_file_path)
-            url = f'sqlite:///{db_file_path}/backend.sqlite'
+            sqlite_filename = f'{db_file_path}/backend.sqlite'
 
         # self.engine = create_engine(url, echo=True,
-        self.engine = create_engine(url,
+        self.engine = create_engine(f'sqlite:///{sqlite_filename}',
                                     json_serializer=_serialize_json,
                                     json_deserializer=_deserialize_json)
 
+        # copy testing database to memory
+        if isinstance(testing, str):
+            import sqlite3
+            source = sqlite3.connect(testing)
+            assert isinstance(self.engine.raw_connection(), _ConnectionFairy)
+            assert isinstance(self.engine.raw_connection().connection, sqlite3.Connection)  # type: ignore
+            source.backup(self.engine.raw_connection().connection, pages=-1)  # type: ignore
+
+        # tempt alembic migration of the database
+        from alembic.config import Config
+        from alembic import command
+        alembic_cfg = Config(os.path.join(os.path.dirname(__file__), 'alembic.ini'))
+        alembic_cfg.set_main_option("script_location", os.path.join(os.path.dirname(__file__), 'migrations'))
+        alembic_cfg.set_main_option("sqlalchemy.url", f'sqlite:///{sqlite_filename}')
+        command.upgrade(alembic_cfg, "head")
+
         # use BEGIN EXCLUSIVE to lock database exclusively to one process
         @event.listens_for(self.engine, "begin")
         def do_begin(conn):
             conn.exec_driver_sql("BEGIN EXCLUSIVE")
 
         orm.Base.metadata.create_all(self.engine)
 
         self.session = Session(bind=self.engine, autoflush=True)
 
+    def close(self):
+        self.session.close()
+        self.engine.dispose()
+
     def _specialiced_serialization(self, key, value):
         if key == "predicate":
             return pickle.dumps(value, protocol=3)
 
     def add_catalogue(self, catalogue: Dict) -> orm.Catalogue:
         serialized_predicate = self._specialiced_serialization('predicate', catalogue['predicate']) \
             if catalogue['predicate'] is not None else None
@@ -169,14 +193,15 @@
     def add_event(self, event: Dict) -> orm.Event:
         return orm.Event(event['start'],
                          event['stop'],
                          event['author'],
                          event['uuid'],
                          event['tags'],
                          event['products'],
+                         event['rating'],
                          event['attributes'])
 
     def add_events_to_catalogue(self, catalogue: orm.Catalogue, events: List[orm.Event]) -> None:
         for e in events:
             if e in catalogue.events:
                 raise ValueError('Event is already in catalogue.')
         catalogue.events.extend(events)
@@ -203,71 +228,76 @@
                       field: Union[Literal['events'], Literal['catalogues']],
                       removed: bool = False) -> Query:
         f = None
 
         if base.get('predicate', None) is not None:
             f = PredicateVisitor(orm_class).visit_predicate(base['predicate'])
 
+        entity_filter = None
         if base.get('entity') is not None:
             entity_filter = getattr(orm_class, field).any(id=base['entity'].id)
             if f is not None:
                 f = or_(f, entity_filter)
             else:
                 f = entity_filter
 
         if f is None:
             f = getattr(orm_class, 'removed') == removed
         else:
             f = and_(getattr(orm_class, 'removed') == removed, f)
 
-        q = self.session.query(orm_class)
+        q = self.session.query(orm_class, entity_filter)
         if f is not None:
             q = q.filter(f)
         return q
 
     def get_catalogues(self, base: Dict = {}) -> List[Dict]:
         catalogues = []
-        for c in self._create_query(base, orm.Catalogue, 'events', removed=base['removed']):
+        for (c, assigned) in self._create_query(base, orm.Catalogue, 'events', removed=base['removed']):
             catalogue = {"name": c.name,
                          "author": c.author,
                          "uuid": c.uuid,
                          "tags": c.tags,
                          "predicate": pickle.loads(c.predicate) if c.predicate else None,
                          "attributes": c.attributes,
                          "entity": c}
             catalogues.append(catalogue)
 
         return catalogues
 
     def get_events(self, base: Dict = {}) -> List[Dict]:
         events = []
-        for e in self._create_query(base, orm.Event, 'catalogues', removed=base['removed']):
+        for (e, assigned) in self._create_query(base, orm.Event, 'catalogues', removed=base['removed']):
             event = {
                 "start": e.start,
                 "stop": e.stop,
                 "author": e.author,
                 "uuid": e.uuid,
                 "tags": e.tags,
                 "products": e.products,
+                "rating": e.rating,
                 "attributes": e.attributes,
-                "entity": e}
+                "entity": e,
+                "is_assigned": assigned,
+            }
             events.append(event)
 
         return events
 
     def get_events_by_uuid_list(self, uuids: List[str]) -> Dict[str, Dict]:
         d = {}
         for e in self.session.query(orm.Event).filter(orm.Event.uuid.in_(uuids)).all():
             d[e.uuid] = {
                 "start": e.start,
                 "stop": e.stop,
                 "author": e.author,
                 "uuid": e.uuid,
                 "tags": e.tags,
                 "products": e.products,
+                "rating": e.rating,
                 "attributes": e.attributes,
                 "entity": e}
 
         return d
 
     def add_and_flush(self, entity_list: List[Union[orm.Event, orm.Catalogue]]):
         self.session.add_all(entity_list)
@@ -281,17 +311,14 @@
 
     def has_unsaved_changes(self) -> bool:
         return self.session.in_transaction()
 
     def remove(self, entity: Union[orm.Catalogue, orm.Event], permanently: bool = False) -> None:
         if permanently:
             self.session.delete(entity)
+            self.session.flush()
         else:
             entity.removed = True
 
     @staticmethod
     def restore(entity: Union[orm.Catalogue, orm.Event]) -> None:
         entity.removed = False
-
-    @staticmethod
-    def is_removed(entity: Union[orm.Catalogue, orm.Event]) -> bool:
-        return entity.removed
```

### Comparing `tscat-0.2.0/tscat/orm_sqlalchemy/orm.py` & `tscat-0.3.0/tscat/orm_sqlalchemy/orm.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,30 +30,32 @@
 
     start = Column(DateTime, nullable=False)
     stop = Column(DateTime, nullable=False)
     author = Column(UnicodeText, nullable=False)
 
     tags: List[str] = Column(ScalarListType(str), default=[], info={"type": (list, "string_list")})
     products: List[str] = Column(ScalarListType(str), default=[], info={"type": (list, "string_list")})
+    rating: int = Column(Integer, default=None, nullable=True)
 
     removed: bool = Column(Boolean, default=False, nullable=False)
 
     attributes: Dict[str, Any] = Column(MutableDict.as_mutable(JSON))
 
-    def __init__(self, start, stop, author, uuid, tags, products, attributes):
+    def __init__(self, start, stop, author, uuid, tags, products, rating, attributes):
         self.start = start
         self.stop = stop
         self.author = author
         self.uuid = uuid
         self.tags = tags
         self.products = products
+        self.rating = rating
         self.attributes = attributes
 
     def __repr__(self):  # pragma: no cover
-        return f'Event({self.id}: {self.start}, {self.stop}, {self.author}), {self.removed}, meta=' + self._proxied.__repr__()
+        return f'Event({self.id}: {self.start}, {self.stop}, {self.author}), {self.removed}, meta=' + self.attributes.__repr__()
 
 
 class Catalogue(Base):
     __tablename__ = 'catalogues'
 
     id = Column(Integer, primary_key=True, autoincrement=True)
 
@@ -78,8 +80,8 @@
         self.author = author
         self.uuid = uuid
         self.tags = tags
         self.predicate = predicate
         self.attributes = attributes
 
     def __repr__(self):  # pragma: no cover
-        return f'Catalogue({self.id}: {self.name}, {self.author}, {self.removed}), attrs=' + self._proxied.__repr__()
+        return f'Catalogue({self.id}: {self.name}, {self.author}, {self.removed}), attrs=' + self.attributes.__repr__()
```

