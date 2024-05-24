# Comparing `tmp/seedbank-0.2.0a2.tar.gz` & `tmp/seedbank-0.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seedbank-0.2.0a2.tar", last modified: Tue May 14 15:14:58 2024, max compression
+gzip compressed data, was "seedbank-0.2.0b1.tar", last modified: Fri May 24 07:53:34 2024, max compression
```

## Comparing `seedbank-0.2.0a2.tar` & `seedbank-0.2.0b1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:58.630687 seedbank-0.2.0a2/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-14 15:14:58.630687 seedbank-0.2.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:58.622687 seedbank-0.2.0a2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:58.622687 seedbank-0.2.0a2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/docs/_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/docs/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/docs/extending.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/docs/patterns.rst
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/justfile
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:58.622687 seedbank-0.2.0a2/seedbank/
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/cupy.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/numba.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:58.626687 seedbank-0.2.0a2/seedbank.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-14 15:14:58.000000 seedbank-0.2.0a2/seedbank.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-14 15:14:58.000000 seedbank-0.2.0a2/seedbank.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:14:58.000000 seedbank-0.2.0a2/seedbank.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-14 15:14:58.000000 seedbank-0.2.0a2/seedbank.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 15:14:58.000000 seedbank-0.2.0a2/seedbank.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:14:58.630687 seedbank-0.2.0a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:58.626687 seedbank-0.2.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/init_seed.json
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/init_seed.toml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/init_seed.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/test_cupy_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/test_derive.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/test_init_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/test_numba.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/test_process_seed.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/test_randomstate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:53:34.388944 seedbank-0.2.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-24 07:53:34.388944 seedbank-0.2.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:53:34.376944 seedbank-0.2.0b1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:53:34.376944 seedbank-0.2.0b1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/docs/_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/docs/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/docs/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/docs/patterns.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/justfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:53:34.380944 seedbank-0.2.0b1/seedbank/
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/cupy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/numba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/seedbank/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:53:34.384944 seedbank-0.2.0b1/seedbank.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-24 07:53:34.000000 seedbank-0.2.0b1/seedbank.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-24 07:53:34.000000 seedbank-0.2.0b1/seedbank.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 07:53:34.000000 seedbank-0.2.0b1/seedbank.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-24 07:53:34.000000 seedbank-0.2.0b1/seedbank.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 07:53:34.000000 seedbank-0.2.0b1/seedbank.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 07:53:34.388944 seedbank-0.2.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:53:34.384944 seedbank-0.2.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/init_seed.json
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/init_seed.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/init_seed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/test_cupy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/test_derive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/test_init_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/test_numba.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/test_process_seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-24 07:53:29.000000 seedbank-0.2.0b1/tests/test_randomstate.py
```

### Comparing `seedbank-0.2.0a2/.gitignore` & `seedbank-0.2.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/LICENSE.md` & `seedbank-0.2.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/PKG-INFO` & `seedbank-0.2.0b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seedbank
-Version: 0.2.0a2
+Version: 0.2.0b1
 Summary: Common infrastructure for seeding random number generators.
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2021–2023 Boise State University
         Copyright (c) 2023-2024 Drexel University and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `seedbank-0.2.0a2/README.md` & `seedbank-0.2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/docs/_templates/footer.html` & `seedbank-0.2.0b1/docs/_templates/footer.html`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/docs/api.rst` & `seedbank-0.2.0b1/docs/api.rst`

 * *Files 9% similar despite different names*

```diff
@@ -19,26 +19,25 @@
 
 Seed Material
 -------------
 
 SeedBank seeds (either root seeds or keys for derived RNGs) can be specified in a number
 of formats.
 
-.. py:attribute:: SeedLike
-    :canonical: _keys.SeedLike
+.. py:data:: SeedLike
 
     “Seed-like” data is data that can be used as seed material. This includes:
 
     - :py:class:`numpy.random.SeedSequence` (used as-is)
     - :py:class:`int` (wrapped in a :py:class:`numpy.random.SeedSequence`)
     - :py:class:`str` (encoded in UTF-8 and hashed)
     - :py:class:`bytes` (hashed)
     - :py:class:`numpy.ndarray` (converted to uint32)
 
-.. py:attribute:: RNGKey
+.. py:data:: RNGKey
     :canonical: _keys.RNGKey
 
     ``RNGKey`` is the type of seed-like data (:py:attr:`SeedLike`) *except* for
     :py:class:`~numpy.random.SeedSequence`.
 
 Obtaining Seeds
 ---------------
```

### Comparing `seedbank-0.2.0a2/docs/conf.py` & `seedbank-0.2.0b1/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import sys
+
 sys.path.insert(0, os.path.abspath(".."))
 
 import seedbank
 
 project = "SeedBank"
 copyright = "2023 Michael Ekstrand"
 author = "Michael D. Ekstrand"
@@ -20,22 +21,19 @@
 
 source_suffix = ".rst"
 
 pygments_style = "sphinx"
 highlight_language = "python3"
 
 html_theme = "furo"
-html_theme_options = {
-}
+html_theme_options = {}
 templates_path = ["_templates"]
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3/", None),
     "numpy": ("https://docs.scipy.org/doc/numpy/", None),
     "sklearn": ("https://scikit-learn.org/stable/", None),
 }
 
-autodoc_default_options = {
-    "members": True,
-    "member-order": "bysource"
-}
+autodoc_default_options = {"members": True, "member-order": "bysource"}
 autodoc_typehints = "description"
+# autodoc_type_aliases = {"SeedLike": "seedbank.SeedLike"}
```

### Comparing `seedbank-0.2.0a2/docs/extending.rst` & `seedbank-0.2.0b1/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/docs/index.rst` & `seedbank-0.2.0b1/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 - NumPy legacy random :py:mod:`numpy.random` (with :py:func:`numpy.random.seed`)
 - PyTorch (with :py:func:`torch.manual_seed`)
 - Numba's `NumPy random`_
 - TensorFlow (with :py:func:`tf.random.set_seed`)
 - cupy (with :py:func:`cupy.random.seed`, also exposing :py:func:`seedbank.cupy_rng`)
 
 In addition, it will initialize a root seed for constructing new-style NumPy
-:py:func:`numpy.random.Generator` instances.
+:py:class:`numpy.random.Generator` instances (:py:func:`~seedbank.numpy_rng`),
+and can construct legacy :py:class:`~numpy.random.RandomState` instances from this
+same seed (:py:func:`~seedbank.numpy_random_state`).
 
 If SeedBank doesn't support your RNG yet, please submit a `pull request`_.
 
 .. _`pull request`: https://github.com/lenskit/seedbank
 
 .. _`NumPy random`: https://numba.readthedocs.io/en/stable/reference/numpysupported.html#random
```

### Comparing `seedbank-0.2.0a2/docs/patterns.rst` & `seedbank-0.2.0b1/docs/patterns.rst`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/justfile` & `seedbank-0.2.0b1/justfile`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/pyproject.toml` & `seedbank-0.2.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,14 @@
 
 [tool.ruff]
 line-length = 100
 target-version = "py310"
 exclude = [
   ".git",
   "__pycache__",
-  "docs/conf.py",
   "build",
   "dist",
 ]
 
 [tool.ruff.lint]
 select = ["E", "F", "I"]
```

### Comparing `seedbank-0.2.0a2/seedbank/__init__.py` & `seedbank-0.2.0b1/seedbank/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import logging
 from importlib import import_module
 from importlib.metadata import PackageNotFoundError, version
 from types import ModuleType
 
 import numpy as np
+from numpy.random import SeedSequence
 from typing_extensions import Optional
 
 from seedbank._keys import RNGKey, SeedLike, make_seed
 from seedbank._state import SeedState
 
 try:
     __version__ = version("seedbank")
@@ -43,15 +44,15 @@
     "seedbank.numba",
     "seedbank.cupy",
     "seedbank.tensorflow",
     "seedbank.torch",
 ]
 
 
-def initialize(seed: SeedLike, *keys: RNGKey):
+def initialize(seed: SeedLike, *keys: RNGKey) -> SeedSequence:
     """
     Initialize the random infrastructure with a seed.  This function should generally be
     called very early in the setup.  This initializes all known and available RNGs with
     a seed derived from the specified seed.
 
     If you do **not** call this function, a default root seed is used, so functions like
     :func:`derive_seed` and :func:`numpy_rng` work, but all other random number generators
@@ -74,15 +75,15 @@
             mod = import_module(mod)
         if mod.is_available():
             mod.seed(_root_state)
 
     return _root_state.seed
 
 
-def derive_seed(*keys: RNGKey, base: Optional[np.random.SeedSequence] = None):
+def derive_seed(*keys: RNGKey, base: Optional[np.random.SeedSequence] = None) -> SeedSequence:
     """
     Derive a seed from the root seed, optionally with additional seed keys.
 
     Args:
         keys:
             Additional components to add to the spawn key for reproducible derivation.
             If unspecified, the seed's internal counter is incremented (by calling
@@ -92,15 +93,15 @@
 
     Returns:
         The random seed.
     """
     return _root_state.derive(base, keys).seed
 
 
-def root_seed():
+def root_seed() -> SeedSequence:
     """
     Get the current root seed.
 
     Returns:
         numpy.random.SeedSequence:
             The root seed.
     """
```

### Comparing `seedbank-0.2.0a2/seedbank/_config.py` & `seedbank-0.2.0b1/seedbank/_config.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/seedbank/_keys.py` & `seedbank-0.2.0b1/seedbank/_keys.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # pyright: reportUnnecessaryIsInstance=false
+from __future__ import annotations
+
 import hashlib
 from typing import Any, Literal, Sequence, TypeAlias, overload
 
 import numpy as np
 import numpy.typing as npt
 
 Entropy: TypeAlias = int | Sequence[int] | npt.NDArray[np.uint32]
```

### Comparing `seedbank-0.2.0a2/seedbank/_state.py` & `seedbank-0.2.0b1/seedbank/_state.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/seedbank/cupy.py` & `seedbank-0.2.0b1/seedbank/cupy.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     if cupy is None:
         warnings.warn("cupy not available, skipping seed")
 
     _log.debug("initializing CuPy root RNG")
     cupy.random.seed(state.int_seed)
 
 
-def cupy_rng(spec: Optional[SeedLike | cupy.random.Generator] = None):
+def cupy_rng(spec: Optional[SeedLike | cupy.random.Generator] = None) -> cupy.random.Generator:
     """
     Get a CuPy random number generator.  This works like :func:`numpy_rng`, but
     it returns a :class:`cupy.random.Generator` instead.
 
     Args:
         spec:
             The spec for this RNG.  Can be any of the following types:
```

### Comparing `seedbank-0.2.0a2/seedbank/numba.py` & `seedbank-0.2.0b1/seedbank/numba.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/seedbank/numpy.py` & `seedbank-0.2.0b1/seedbank/numpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 
 import numpy as np
 from typing_extensions import Optional, TypeAlias
 
 from . import derive_seed, int_seed
 from ._keys import SeedLike, make_seed
```

### Comparing `seedbank-0.2.0a2/seedbank/tensorflow.py` & `seedbank-0.2.0b1/seedbank/tensorflow.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/seedbank.egg-info/PKG-INFO` & `seedbank-0.2.0b1/seedbank.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seedbank
-Version: 0.2.0a2
+Version: 0.2.0b1
 Summary: Common infrastructure for seeding random number generators.
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2021–2023 Boise State University
         Copyright (c) 2023-2024 Drexel University and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `seedbank-0.2.0a2/seedbank.egg-info/SOURCES.txt` & `seedbank-0.2.0b1/seedbank.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .editorconfig
 .gitattributes
 .gitignore
+CITATION.cff
 LICENSE.md
 MANIFEST.in
 README.md
 justfile
 pyproject.toml
 docs/api.rst
 docs/conf.py
```

### Comparing `seedbank-0.2.0a2/tests/test_cupy_generator.py` & `seedbank-0.2.0b1/tests/test_cupy_generator.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/tests/test_derive.py` & `seedbank-0.2.0b1/tests/test_derive.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/tests/test_generator.py` & `seedbank-0.2.0b1/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/tests/test_init.py` & `seedbank-0.2.0b1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/tests/test_init_file.py` & `seedbank-0.2.0b1/tests/test_init_file.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/tests/test_process_seed.py` & `seedbank-0.2.0b1/tests/test_process_seed.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a2/tests/test_randomstate.py` & `seedbank-0.2.0b1/tests/test_randomstate.py`

 * *Files identical despite different names*

