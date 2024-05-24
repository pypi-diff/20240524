# Comparing `tmp/tdict-0.2.2.tar.gz` & `tmp/tdict-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdict-0.2.2.tar", last modified: Sat Dec 25 02:19:26 2021, max compression
+gzip compressed data, was "tdict-0.3.tar", last modified: Fri May 24 05:51:52 2024, max compression
```

## Comparing `tdict-0.2.2.tar` & `tdict-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 royf       (501) staff       (20)        0 2021-12-25 02:19:26.312394 tdict-0.2.2/
--rw-r--r--   0 royf       (501) staff       (20)     1064 2019-09-09 01:00:50.000000 tdict-0.2.2/LICENSE
--rw-r--r--   0 royf       (501) staff       (20)      281 2021-12-25 02:19:26.312183 tdict-0.2.2/PKG-INFO
--rw-r--r--   0 royf       (501) staff       (20)       79 2019-09-09 01:00:50.000000 tdict-0.2.2/README.md
--rw-r--r--   0 royf       (501) staff       (20)       38 2021-12-25 02:19:26.312461 tdict-0.2.2/setup.cfg
--rw-r--r--   0 royf       (501) staff       (20)      311 2021-12-25 02:11:43.000000 tdict-0.2.2/setup.py
-drwxr-xr-x   0 royf       (501) staff       (20)        0 2021-12-25 02:19:26.310357 tdict-0.2.2/tdict/
--rw-r--r--   0 royf       (501) staff       (20)       53 2021-03-30 06:39:37.000000 tdict-0.2.2/tdict/__init__.py
--rw-r--r--   0 royf       (501) staff       (20)    11243 2021-12-25 02:07:48.000000 tdict-0.2.2/tdict/tdict.py
-drwxr-xr-x   0 royf       (501) staff       (20)        0 2021-12-25 02:19:26.311904 tdict-0.2.2/tdict.egg-info/
--rw-r--r--   0 royf       (501) staff       (20)      281 2021-12-25 02:19:26.000000 tdict-0.2.2/tdict.egg-info/PKG-INFO
--rw-r--r--   0 royf       (501) staff       (20)      175 2021-12-25 02:19:26.000000 tdict-0.2.2/tdict.egg-info/SOURCES.txt
--rw-r--r--   0 royf       (501) staff       (20)        1 2021-12-25 02:19:26.000000 tdict-0.2.2/tdict.egg-info/dependency_links.txt
--rw-r--r--   0 royf       (501) staff       (20)        6 2021-12-25 02:19:26.000000 tdict-0.2.2/tdict.egg-info/top_level.txt
+drwxr-xr-x   0 royf       (501) staff       (20)        0 2024-05-24 05:51:52.247873 tdict-0.3/
+-rw-r--r--   0 royf       (501) staff       (20)     1064 2019-09-09 01:00:50.000000 tdict-0.3/LICENSE
+-rw-r--r--   0 royf       (501) staff       (20)      251 2024-05-24 05:51:52.246320 tdict-0.3/PKG-INFO
+-rw-r--r--   0 royf       (501) staff       (20)       79 2019-09-09 01:00:50.000000 tdict-0.3/README.md
+-rw-r--r--   0 royf       (501) staff       (20)       38 2024-05-24 05:51:52.248169 tdict-0.3/setup.cfg
+-rw-r--r--   0 royf       (501) staff       (20)      309 2024-05-24 05:43:42.000000 tdict-0.3/setup.py
+drwxr-xr-x   0 royf       (501) staff       (20)        0 2024-05-24 05:51:52.238973 tdict-0.3/tdict/
+-rw-r--r--   0 royf       (501) staff       (20)       53 2021-03-30 06:39:37.000000 tdict-0.3/tdict/__init__.py
+-rw-r--r--   0 royf       (501) staff       (20)    12794 2024-05-24 05:31:16.000000 tdict-0.3/tdict/tdict.py
+drwxr-xr-x   0 royf       (501) staff       (20)        0 2024-05-24 05:51:52.244366 tdict-0.3/tdict.egg-info/
+-rw-r--r--   0 royf       (501) staff       (20)      251 2024-05-24 05:51:52.000000 tdict-0.3/tdict.egg-info/PKG-INFO
+-rw-r--r--   0 royf       (501) staff       (20)      175 2024-05-24 05:51:52.000000 tdict-0.3/tdict.egg-info/SOURCES.txt
+-rw-r--r--   0 royf       (501) staff       (20)        1 2024-05-24 05:51:52.000000 tdict-0.3/tdict.egg-info/dependency_links.txt
+-rw-r--r--   0 royf       (501) staff       (20)        6 2024-05-24 05:51:52.000000 tdict-0.3/tdict.egg-info/top_level.txt
```

### Comparing `tdict-0.2.2/LICENSE` & `tdict-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tdict-0.2.2/tdict/tdict.py` & `tdict-0.3/tdict/tdict.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 class Tdict(abc.MutableMapping):
     """
     Tree dict.
 
     Values of `str` keys can be accessed either as attributes or as items.
     Values of `tuple` keys are stored in nested `Tdict`s.
 
+    >>> from tdict import Tdict
+    >>> import json
     >>> d = Tdict(
             {'a': 1, 'sub': {tuple('non-str keys allowed'.split()): True}},
             json.loads('{"sub": {"x": 10}}'),
             b=2, **{'c': 3}, d=4)
     >>> d
     Tdict(a=1, sub=Tdict(('non-str', 'keys', 'allowed')=True, x=10), b=2, c=3, d=4)
     >>> d.a
@@ -51,14 +53,17 @@
     [('a', 101),
      ('sub', Tdict(('non-str', 'keys', 'allowed')=True, x=10, y=11)),
      ('c', 3),
      ('d', 4),
      ('e', 5),
      ('f', 6),
      ('g', 7)]
+    >>> z = d.copy()
+    >>> z.set_deep(False)
+    >>> assert list(z.items()) == list(d.items(deep=False)) == list(d.as_deep(False).items())
     >>> d * Tdict(sub=Tdict(y=7)) + dict(sub=100)
     Tdict(a=101, sub=Tdict(('non-str', 'keys', 'allowed')=101, x=110, y=177), c=3, d=4, e=5, f=6, g=7)
     >>> match d:  # new in Python 3.10
             case {'c': z}:
                 print(z)
     3
     >>> match d:  # new in Python 3.10
@@ -66,27 +71,32 @@
                 print(w)
     10
     >>> assert d[()] is d
 
     @DynamicAttrs
     """
 
-    def __init__(self, *maps, **attr):
+    def __new__(cls, *maps, deep=True, **attr):
+        return super().__new__(type('Tdict', (Tdict,), {'_deep': deep}))
+
+    def __init__(self, *maps, deep=True, **attr):
         """
 
         Args:
             *maps (Mapping): Update attributes from these `Mapping`s.
                              Values that are themselves `Mapping`s are deep-copied as sub-`Tdict`s.
+            deep (bool): whether to iterate keys, values, and items recursively by default.
             **attr: Extra attributes.
         """
         super().__init__()
         for m in maps:
-            for k, v in shallow_items(m):
+            shallow_map = vars(m) if isinstance(m, Tdict) else m
+            for k, v in shallow_map.items():
                 if isinstance(v, abc.Mapping):
-                    vars(self).setdefault(k, Tdict()).update(v)
+                    vars(self).setdefault(k, Tdict(deep=deep)).update(v)
                 else:
                     vars(self)[k] = v
         self.update(attr)
 
     def __getitem__(self, k):
         """
 
@@ -126,15 +136,15 @@
         try:
             if isinstance(k, tuple):
                 if len(k) == 0:
                     raise KeyError("cannot assign to root")
                 elif len(k) == 1:
                     vars(self)[k[0]] = v
                 elif k[0] not in vars(self):
-                    d = Tdict()
+                    d = Tdict(deep=self._deep)
                     d[k[1:]] = v
                     vars(self)[k[0]] = d
                 elif isinstance(vars(self)[k[0]], Tdict):
                     vars(self)[k[0]][k[1:]] = v
                 else:
                     raise KeyError(k[0])
             else:
@@ -164,69 +174,63 @@
                 else:
                     raise KeyError(k[0])
             else:
                 del vars(self)[k]
         except KeyError:
             raise KeyError(k) from None
 
-    def keys(self, deep=True):
+    def set_deep(self, deep):
+        type(self)._deep = deep
+
+    def as_deep(self, deep):
+        d = self.copy()
+        d.set_deep(deep)
+        return d
+
+    def keys(self, deep=None):
         """
 
         Args:
-            deep (bool)
+            deep (bool): whether to iterate recursively.
 
         Yields:
             Next key.
         """
-        if deep:
-            for k, v in vars(self).items():
-                if isinstance(v, Tdict):
-                    for k_ in v.keys():
-                        yield (k,) + k_
-                else:
-                    yield k,
+        if deep or (deep is None and self._deep):
+            return tdict_keys(self, deep)
         else:
-            yield from vars(self).keys()
+            return vars(self).keys()
 
-    def items(self, deep=True):
+    def values(self, deep=None):
         """
 
         Args:
-            deep (bool)
+            deep (bool): whether to iterate recursively.
 
         Yields:
-            Next item.
+            Next value.
         """
-        if deep:
-            for k, v in vars(self).items():
-                if isinstance(v, Tdict):
-                    for k_, v_ in v.items():
-                        yield (k,) + k_, v_
-                else:
-                    yield (k,), v
+        if deep or (deep is None and self._deep):
+            return tdict_values(self, deep)
         else:
-            yield from vars(self).items()
+            return vars(self).values()
 
-    def values(self, deep=True):
+    def items(self, deep=None):
         """
 
         Args:
-            deep (bool)
+            deep (bool): whether to iterate recursively.
 
         Yields:
-            Next value.
+            Next item.
         """
-        if deep:
-            for v in vars(self).values():
-                if isinstance(v, Tdict):
-                    yield from v.values()
-                else:
-                    yield v
+        if deep or (deep is None and self._deep):
+            return tdict_items(self, deep)
         else:
-            yield from vars(self).values()
+            return vars(self).items()
 
     def __iter__(self):
         """
 
         Yields:
             Next key.
         """
@@ -276,15 +280,15 @@
 
         Args:
             exclude: Container of shallow keys to exclude. Default: no keys excluded.
 
         Returns:
             Tdict: Deep copy of `self`.
         """
-        res = Tdict()
+        res = Tdict(deep=self._deep)
         for k, v in vars(self).items():
             if exclude is not None and k in exclude:
                 continue
             if isinstance(v, Tdict):
                 vars(res)[k] = v.copy()
             else:
                 vars(res)[k] = v
@@ -311,15 +315,16 @@
             o ((Any, Any) -> Any): Update operator, such that `x = o(x, y)` updates value `x` with new value `y`.
                 Default: replace current value, `x = y`.
 
         Returns:
             Tdict: `self` after update.
         """
         if isinstance(d, abc.Mapping):
-            for k, v in shallow_items(d):
+            shallow_map = vars(d) if isinstance(d, Tdict) else d
+            for k, v in shallow_map.items():
                 if k in vars(self):
                     v_ = vars(self)[k]
                     if isinstance(v_, Tdict):
                         if isinstance(v, abc.Mapping) or o is not None:
                             vars(self)[k].update(v, o)
                         else:
                             vars(self)[k] = v
@@ -336,26 +341,46 @@
                 elif o is None:
                     vars(self)[k] = d
                 else:
                     vars(self)[k] = o(v, d)
         return self
 
 
-def shallow_items(m):
-    if isinstance(m, Tdict):
-        return m.items(False)
-    else:
-        return m.items()
+def tdict_keys(d, deep):
+    for k, v in vars(d).items():
+        if isinstance(v, Tdict):
+            for k_ in v.keys(deep):
+                # noinspection PyProtectedMember
+                if deep or (deep is None and v._deep):
+                    yield (k,) + k_
+                else:
+                    yield k, k_
+        else:
+            yield k,
 
 
-def ensure_tdict(x):
-    if isinstance(x, abc.Mapping) and not isinstance(x, Tdict):
-        return Tdict(x)
-    else:
-        return x
+def tdict_values(d, deep):
+    for v in vars(d).values():
+        if isinstance(v, Tdict):
+            yield from v.values(deep)
+        else:
+            yield v
+
+
+def tdict_items(d, deep):
+    for k, v in vars(d).items():
+        if isinstance(v, Tdict):
+            for k_, v_ in v.items(deep):
+                # noinspection PyProtectedMember
+                if deep or (deep is None and v._deep):
+                    yield (k,) + k_, v_
+                else:
+                    yield (k, k_), v_
+        else:
+            yield (k,), v
 
 
 class _Op(object):
     def __init__(self, o, inplace=True):
         self.o = o
         self.inplace = inplace
 
@@ -379,33 +404,44 @@
     'mul': operator.imul,
     'matmul': operator.imatmul,
     'rshift': operator.irshift,
     'sub': operator.isub,
 }
 
 for name, op in _OPERATORS.items():
-    setattr(Tdict, f'__{name}__', _Op(op, False))
-    setattr(Tdict, f'__i{name}__', _Op(op, True))
+    setattr(Tdict, f'__{name}__', _Op(op, inplace=False))
+    setattr(Tdict, f'__i{name}__', _Op(op, inplace=True))
+
+
+def ensure_tdict(x, deep=True):
+    if isinstance(x, abc.Mapping) and not isinstance(x, Tdict):
+        return Tdict(x, deep=deep)
+    else:
+        return x
 
 
-def tdictify(x, through=None):
+def tdictify(x, through=None, deep=True):
     """
     Return a recursively `Tdict`ified version of `x`:
         If `x` is a `Mapping`, return a `Tdict` with the same keys and `Tdict`ified values.
         If `x` is an instance of a type in `through`, return a new instance of that type with `Tdict`ified elements.
         Otherwise, return `x`.
 
     Args:
         x: The object to `Tdict`ify.
         through (Sequence[type]): list of types through which to deep-copy and `Tdict`ify; e.g., `[list, tuple]`.
+        deep (bool): whether the constructed Tdict iterates keys, values, and items recursively by default.
 
     Returns:
         Tdict: `Tdict`ified version of `x`.
     """
     if isinstance(x, abc.Mapping):
-        return Tdict({k: tdictify(v, through) for k, v in x.items()})
+        if isinstance(x, Tdict):
+            # noinspection PyProtectedMember
+            deep = x._deep
+        shallow_map = vars(x) if isinstance(x, Tdict) else x
+        return Tdict({k: tdictify(v, through, deep=deep) for k, v in shallow_map.items()}, deep=deep)
     if through:
         for t in through:
             if isinstance(x, t):
-                # noinspection PyTypeChecker
-                return t(tdictify(v, through) for v in x)
+                return t(tdictify(v, through, deep=deep) for v in x)
     return x
```

