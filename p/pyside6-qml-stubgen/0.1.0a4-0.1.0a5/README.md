# Comparing `tmp/pyside6_qml_stubgen-0.1.0a4.tar.gz` & `tmp/pyside6_qml_stubgen-0.1.0a5.tar.gz`

## Comparing `pyside6_qml_stubgen-0.1.0a4.tar` & `pyside6_qml_stubgen-0.1.0a5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/conftest.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/requirements.txt
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/.github/workflows/test.yml
--rw-r--r--   0        0        0    14283 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/__init__.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/__main__.py
--rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/dirty_file_detection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/py.typed
--rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/pyside_patching.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/qmlregistrar_types.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/__init__.py
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/test_run.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/README
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/qmldir
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/qmltyperegistrations1-0.cpp
--rw-r--r--   0        0        0    15603 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/types1-0.json
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/types1-0.qmltypes
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced/qmldir
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced/qmltyperegistrations1-100.cpp
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced/types1-100.json
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced/types1-100.qmltypes
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced2/qmldir
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced2/qmltyperegistrations1-100.cpp
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced2/types1-100.json
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced2/types1-100.qmltypes
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/sub/qmldir
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/sub/qmltyperegistrations2-1.cpp
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/sub/types2-1.json
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/sub/types2-1.qmltypes
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/target/__init__.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/target/advanced.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/target/advanced2.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/target/clses.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/target/clses2.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/target/submodule.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/.gitignore
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/LICENCE.md
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/README.md
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/conftest.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/requirements.txt
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/.github/workflows/test.yml
+-rw-r--r--   0        0        0    14803 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/pyside6_qml_stubgen/__init__.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/pyside6_qml_stubgen/__main__.py
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/pyside6_qml_stubgen/dirty_file_detection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/pyside6_qml_stubgen/py.typed
+-rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/pyside6_qml_stubgen/pyside_patching.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/pyside6_qml_stubgen/qmlregistrar_types.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/__init__.py
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/test_run.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/README
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/target/qmldir
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/target/qmltyperegistrations1-0.cpp
+-rw-r--r--   0        0        0    15603 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/target/types1-0.json
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/target/types1-0.qmltypes
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/target/advanced/qmldir
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/target/advanced/qmltyperegistrations1-100.cpp
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/target/advanced/types1-100.json
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/target/advanced/types1-100.qmltypes
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/target/advanced2/qmldir
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/target/advanced2/qmltyperegistrations1-100.cpp
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/target/advanced2/types1-100.json
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/target/advanced2/types1-100.qmltypes
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/target/sub/qmldir
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/target/sub/qmltyperegistrations2-1.cpp
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/target/sub/types2-1.json
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/reference/target/sub/types2-1.qmltypes
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/target/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/target/advanced.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/target/advanced2.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/target/clses.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/target/clses2.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/tests/target/submodule.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/.gitignore
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/LICENCE.md
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/README.md
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a5/PKG-INFO
```

### Comparing `pyside6_qml_stubgen-0.1.0a4/.github/workflows/test.yml` & `pyside6_qml_stubgen-0.1.0a5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/__init__.py` & `pyside6_qml_stubgen-0.1.0a5/pyside6_qml_stubgen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,36 +215,53 @@
 def import_dirty_modules(
     in_dirs: typing.Sequence[pathlib.Path],
     ignore_dirs: typing.Sequence[pathlib.Path],
     out_dir: pathlib.Path,
 ) -> tuple[pyside_patching.ExtraCollectedInfo, set[pathlib.Path]]:
     extra_info = pyside_patching.patches()
     sys.path.append(".")
+    sys_paths = sorted(
+        [pathlib.Path(p).resolve() for p in sys.path if pathlib.Path(p).is_dir()],
+        key=lambda p: len(p.parts),
+        reverse=True,
+    )
 
     all_python_files = [
-        fname
+        fname.resolve()
         for fname in itertools.chain.from_iterable(
-            in_dir.rglob("*.py") for in_dir in in_dirs
+            in_dir.rglob(suffix) for in_dir in in_dirs for suffix in ("*.py", "*.pyd")
         )
         if not any(ig in fname.parents for ig in ignore_dirs)
     ]
-    dirty_files, module_metadata, dependency_dirty_paths = (
-        dirty_file_detection.detect_new_and_dirty_files(
-            all_python_files, dirty_file_detection.load_modules_metadata(out_dir)
-        )
+    (
+        dirty_files,
+        module_metadata,
+        dependency_dirty_paths,
+    ) = dirty_file_detection.detect_new_and_dirty_files(
+        all_python_files, dirty_file_detection.load_modules_metadata(out_dir)
     )
     for fname, reason in dirty_files.items():
+        relative_fname = fname
+        for sys_p in sys_paths:
+            if sys_p in fname.parents:
+                relative_fname = fname.relative_to(sys_p)
+                break
+        else:
+            raise RuntimeError(f"Could not deduce import name for {fname}")
+
         module = ".".join(
-            [x.name for x in fname.parents if x.name][::-1] + [fname.stem]
+            [x.name for x in relative_fname.parents if x.name][::-1]
+            + [relative_fname.name.split(".")[0]]
         )
         if module.endswith(".__init__"):
             module = module.removesuffix(".__init__")
+
         print(f" -> {module} ({reason})")
         mod = importlib.import_module(module)
-        if not mod.__file__ or pathlib.Path(mod.__file__).resolve() != fname.resolve():
+        if not mod.__file__ or pathlib.Path(mod.__file__).resolve() != fname:
             raise RuntimeError(
                 f"Imported module {module} was expected to come from {fname}, but instead came from {mod.__file__}"
             )
         dirty_file_detection.recursive_module_metadata_addition(
             module, extra_info.module_dependencies, module_metadata
         )
 
@@ -252,15 +269,15 @@
         out_dir, dirty_file_detection.PythonModulesMetadata(module_metadata)
     )
 
     extra_info.resolve_delayed()
     return (
         extra_info,
         {
-            cf.resolve()
+            cf
             for cf in dirty_file_detection.imported_files()
             .union(dirty_files)
             .union(dependency_dirty_paths)
         },
     )
```

### Comparing `pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/__main__.py` & `pyside6_qml_stubgen-0.1.0a5/pyside6_qml_stubgen/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Generate QML stub files (.qmltypes) from Python modules (which use PySide6)
 
 Usage:
     pyside6-qml-stubgen <in-dir>... --out-dir=<out-dir> [--ignore=<path>...] [--metatypes-dir=<dir>] [--qmltyperegistrar-path=<path>] [--force-rebuild] [--file-relative-path=<div>]
 
 Options:
-    --ignore=<path>                     Ignore all Python files that are children of thispath
+    --ignore=<path>                     Ignore all Python files that are children of this path
     --metatypes-dir=<dir>               Directory of the Qt 6 metatype files for core modules (automatically detected if not provided)
     --qmltyperegistrar-path=<path>      Path of the qmltyperegistrar tool (automatically detected if not provided)
     --force-rebuild                     Rebuild the stubs from scratch instead of doing a partial update
     --file-relative-path=<div>          Make all paths in generated type files relative to this path
                                             (useful for if the generated stubs need to be used on different systems)
 """
```

### Comparing `pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/dirty_file_detection.py` & `pyside6_qml_stubgen-0.1.0a5/pyside6_qml_stubgen/dirty_file_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         meta.path: name
         for name, meta in modules_metadata.modules.items()
         if meta is not None
     }
     reachable_modules = {
         maybe_name
         for cf in current_files
-        if (maybe_name := module_path_to_name.get(cf.resolve()))
+        if (maybe_name := module_path_to_name.get(cf))
     }
 
     previous_reachable_modules: set[str] = set()
     while reachable_modules != previous_reachable_modules:
         previous_reachable_modules = reachable_modules.copy()
         for name in previous_reachable_modules:
             if meta := modules_metadata.modules[name]:
@@ -131,15 +131,15 @@
             else (
                 "changed"
                 if dirty_dep == module_name
                 else f"dependency {dirty_dep} changed"
             )
         )
         for cf in current_files
-        if (module_name := module_path_to_name.get(cf.resolve())) is None
+        if (module_name := module_path_to_name.get(cf)) is None
         or (dirty_dep := module_dirty[module_name])
     }
     cleaned_modules_metadata = {
         name: meta
         for name, meta in modules_metadata.modules.items()
         if name in reachable_modules and module_dirty[name] is None
     }
```

### Comparing `pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/pyside_patching.py` & `pyside6_qml_stubgen-0.1.0a5/pyside6_qml_stubgen/pyside_patching.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/qmlregistrar_types.py` & `pyside6_qml_stubgen-0.1.0a5/pyside6_qml_stubgen/qmlregistrar_types.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/test_run.py` & `pyside6_qml_stubgen-0.1.0a5/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/qmltyperegistrations1-0.cpp` & `pyside6_qml_stubgen-0.1.0a5/tests/reference/target/qmltyperegistrations1-0.cpp`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/types1-0.json` & `pyside6_qml_stubgen-0.1.0a5/tests/reference/target/types1-0.json`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/types1-0.qmltypes` & `pyside6_qml_stubgen-0.1.0a5/tests/reference/target/types1-0.qmltypes`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced/qmltyperegistrations1-100.cpp` & `pyside6_qml_stubgen-0.1.0a5/tests/reference/target/advanced/qmltyperegistrations1-100.cpp`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced/types1-100.json` & `pyside6_qml_stubgen-0.1.0a5/tests/reference/target/advanced/types1-100.json`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced/types1-100.qmltypes` & `pyside6_qml_stubgen-0.1.0a5/tests/reference/target/advanced/types1-100.qmltypes`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced2/qmltyperegistrations1-100.cpp` & `pyside6_qml_stubgen-0.1.0a5/tests/reference/target/advanced2/qmltyperegistrations1-100.cpp`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced2/types1-100.json` & `pyside6_qml_stubgen-0.1.0a5/tests/reference/target/advanced2/types1-100.json`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced2/types1-100.qmltypes` & `pyside6_qml_stubgen-0.1.0a5/tests/reference/target/advanced2/types1-100.qmltypes`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/sub/qmltyperegistrations2-1.cpp` & `pyside6_qml_stubgen-0.1.0a5/tests/reference/target/sub/qmltyperegistrations2-1.cpp`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/sub/types2-1.json` & `pyside6_qml_stubgen-0.1.0a5/tests/reference/target/sub/types2-1.json`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/sub/types2-1.qmltypes` & `pyside6_qml_stubgen-0.1.0a5/tests/reference/target/sub/types2-1.qmltypes`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/target/advanced.py` & `pyside6_qml_stubgen-0.1.0a5/tests/target/advanced.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/target/advanced2.py` & `pyside6_qml_stubgen-0.1.0a5/tests/target/advanced2.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/target/clses.py` & `pyside6_qml_stubgen-0.1.0a5/tests/target/clses.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/tests/target/clses2.py` & `pyside6_qml_stubgen-0.1.0a5/tests/target/clses2.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/LICENCE.md` & `pyside6_qml_stubgen-0.1.0a5/LICENCE.md`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/README.md` & `pyside6_qml_stubgen-0.1.0a5/README.md`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/pyproject.toml` & `pyside6_qml_stubgen-0.1.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a4/PKG-INFO` & `pyside6_qml_stubgen-0.1.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyside6-qml-stubgen
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Generate QML stub files (.qmltypes) from Python modules (which use PySide6)
 Project-URL: Homepage, https://github.com/matsjoyce/pyside6-qml-stubgen
 Project-URL: Repository, https://github.com/matsjoyce/pyside6-qml-stubgen.git
 Project-URL: Issues, https://github.com/matsjoyce/pyside6-qml-stubgen/issues
 Author: Matthew Joyce
 License-File: LICENCE.md
 Keywords: pyside6,qml,qt6,type checking
```

