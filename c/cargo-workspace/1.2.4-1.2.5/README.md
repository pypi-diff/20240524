# Comparing `tmp/cargo_workspace-1.2.4.tar.gz` & `tmp/cargo_workspace-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cargo_workspace-1.2.4.tar", last modified: Wed May 15 10:18:54 2024, max compression
+gzip compressed data, was "cargo_workspace-1.2.5.tar", last modified: Fri May 24 18:28:27 2024, max compression
```

## Comparing `cargo_workspace-1.2.4.tar` & `cargo_workspace-1.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vados      (501) staff       (20)        0 2024-05-15 10:18:54.337038 cargo_workspace-1.2.4/
--rw-r--r--   0 vados      (501) staff       (20)     1154 2024-05-15 10:18:54.336847 cargo_workspace-1.2.4/PKG-INFO
--rw-r--r--   0 vados      (501) staff       (20)      565 2024-02-24 14:50:43.000000 cargo_workspace-1.2.4/README.md
-drwxr-xr-x   0 vados      (501) staff       (20)        0 2024-05-15 10:18:54.334950 cargo_workspace-1.2.4/cargo_workspace/
--rw-r--r--   0 vados      (501) staff       (20)      247 2024-03-25 13:04:02.000000 cargo_workspace-1.2.4/cargo_workspace/__init__.py
--rw-r--r--   0 vados      (501) staff       (20)      822 2024-03-25 11:26:03.000000 cargo_workspace-1.2.4/cargo_workspace/dependency.py
--rw-r--r--   0 vados      (501) staff       (20)     8827 2024-05-15 10:13:02.000000 cargo_workspace-1.2.4/cargo_workspace/lib.py
--rw-r--r--   0 vados      (501) staff       (20)     5613 2024-03-25 13:11:07.000000 cargo_workspace-1.2.4/cargo_workspace/version.py
-drwxr-xr-x   0 vados      (501) staff       (20)        0 2024-05-15 10:18:54.336530 cargo_workspace-1.2.4/cargo_workspace.egg-info/
--rw-r--r--   0 vados      (501) staff       (20)     1154 2024-05-15 10:18:54.000000 cargo_workspace-1.2.4/cargo_workspace.egg-info/PKG-INFO
--rw-r--r--   0 vados      (501) staff       (20)      344 2024-05-15 10:18:54.000000 cargo_workspace-1.2.4/cargo_workspace.egg-info/SOURCES.txt
--rw-r--r--   0 vados      (501) staff       (20)        1 2024-05-15 10:18:54.000000 cargo_workspace-1.2.4/cargo_workspace.egg-info/dependency_links.txt
--rw-r--r--   0 vados      (501) staff       (20)       35 2024-05-15 10:18:54.000000 cargo_workspace-1.2.4/cargo_workspace.egg-info/requires.txt
--rw-r--r--   0 vados      (501) staff       (20)       16 2024-05-15 10:18:54.000000 cargo_workspace-1.2.4/cargo_workspace.egg-info/top_level.txt
--rw-r--r--   0 vados      (501) staff       (20)      708 2024-05-15 10:18:50.000000 cargo_workspace-1.2.4/pyproject.toml
--rw-r--r--   0 vados      (501) staff       (20)       38 2024-05-15 10:18:54.337082 cargo_workspace-1.2.4/setup.cfg
-drwxr-xr-x   0 vados      (501) staff       (20)        0 2024-05-15 10:18:54.336185 cargo_workspace-1.2.4/tests/
--rw-r--r--   0 vados      (501) staff       (20)    14405 2024-05-15 10:18:33.000000 cargo_workspace-1.2.4/tests/test_lib.py
+drwxr-xr-x   0 vados      (501) staff       (20)        0 2024-05-24 18:28:27.837996 cargo_workspace-1.2.5/
+-rw-r--r--   0 vados      (501) staff       (20)     1154 2024-05-24 18:28:27.837778 cargo_workspace-1.2.5/PKG-INFO
+-rw-r--r--   0 vados      (501) staff       (20)      565 2024-02-24 14:50:43.000000 cargo_workspace-1.2.5/README.md
+drwxr-xr-x   0 vados      (501) staff       (20)        0 2024-05-24 18:28:27.835428 cargo_workspace-1.2.5/cargo_workspace/
+-rw-r--r--   0 vados      (501) staff       (20)      267 2024-05-24 18:27:28.000000 cargo_workspace-1.2.5/cargo_workspace/__init__.py
+-rw-r--r--   0 vados      (501) staff       (20)     1559 2024-05-24 18:28:23.000000 cargo_workspace-1.2.5/cargo_workspace/dependency.py
+-rw-r--r--   0 vados      (501) staff       (20)     8865 2024-05-24 18:27:04.000000 cargo_workspace-1.2.5/cargo_workspace/lib.py
+-rw-r--r--   0 vados      (501) staff       (20)     5613 2024-03-25 13:11:07.000000 cargo_workspace-1.2.5/cargo_workspace/version.py
+drwxr-xr-x   0 vados      (501) staff       (20)        0 2024-05-24 18:28:27.837465 cargo_workspace-1.2.5/cargo_workspace.egg-info/
+-rw-r--r--   0 vados      (501) staff       (20)     1154 2024-05-24 18:28:27.000000 cargo_workspace-1.2.5/cargo_workspace.egg-info/PKG-INFO
+-rw-r--r--   0 vados      (501) staff       (20)      344 2024-05-24 18:28:27.000000 cargo_workspace-1.2.5/cargo_workspace.egg-info/SOURCES.txt
+-rw-r--r--   0 vados      (501) staff       (20)        1 2024-05-24 18:28:27.000000 cargo_workspace-1.2.5/cargo_workspace.egg-info/dependency_links.txt
+-rw-r--r--   0 vados      (501) staff       (20)       35 2024-05-24 18:28:27.000000 cargo_workspace-1.2.5/cargo_workspace.egg-info/requires.txt
+-rw-r--r--   0 vados      (501) staff       (20)       16 2024-05-24 18:28:27.000000 cargo_workspace-1.2.5/cargo_workspace.egg-info/top_level.txt
+-rw-r--r--   0 vados      (501) staff       (20)      708 2024-05-24 18:13:20.000000 cargo_workspace-1.2.5/pyproject.toml
+-rw-r--r--   0 vados      (501) staff       (20)       38 2024-05-24 18:28:27.838038 cargo_workspace-1.2.5/setup.cfg
+drwxr-xr-x   0 vados      (501) staff       (20)        0 2024-05-24 18:28:27.836969 cargo_workspace-1.2.5/tests/
+-rw-r--r--   0 vados      (501) staff       (20)    14428 2024-05-24 18:09:41.000000 cargo_workspace-1.2.5/tests/test_lib.py
```

### Comparing `cargo_workspace-1.2.4/PKG-INFO` & `cargo_workspace-1.2.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cargo_workspace
-Version: 1.2.4
+Version: 1.2.5
 Summary: Parse a cargo workspace and analyze its packages
 Author-email: Oliver Tale-Yazdi <oliver@tasty.limo>
 Project-URL: Homepage, https://github.com/ggwpez/py-cargo-workspace
 Keywords: cargo,rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `cargo_workspace-1.2.4/README.md` & `cargo_workspace-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `cargo_workspace-1.2.4/cargo_workspace/lib.py` & `cargo_workspace-1.2.5/cargo_workspace/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import toml
 
-from .dependency import Dependencies
+from .dependency import Dependencies, DependencyLocation
 from .version import Version, CargoVersion, CargoVersionBump
 
 class Crate:
 	def __init__(self, manifest, path, root_dir=None):
 		Crate.__ensure_is_manifest(manifest)
 		self._manifest = manifest
 		self._path = path
@@ -65,18 +65,18 @@
 		deps = {}
 		for kind in kinds:
 			table = f"{kind}-dependencies" if kind != 'normal' else 'dependencies'
 			table = self._manifest.get(table, None)
 			if table is None:
 				continue
    
-			for dep in table:
+			for name, v in table.items():
 				if not kind in deps:
 					deps[kind] = []
-				deps[kind].append(dep)
+				deps[kind].append((name, v))
 		return Dependencies.from_map(deps)
 
 	def _get_version(self):
 		if not 'version' in self._crate():
 			raise ValueError(f'Could not find version in crate manifest at {self._path}')
 		return Version.from_str(self._crate()['version']).cargo_convention()
```

### Comparing `cargo_workspace-1.2.4/cargo_workspace/version.py` & `cargo_workspace-1.2.5/cargo_workspace/version.py`

 * *Files identical despite different names*

### Comparing `cargo_workspace-1.2.4/cargo_workspace.egg-info/PKG-INFO` & `cargo_workspace-1.2.5/cargo_workspace.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cargo_workspace
-Version: 1.2.4
+Version: 1.2.5
 Summary: Parse a cargo workspace and analyze its packages
 Author-email: Oliver Tale-Yazdi <oliver@tasty.limo>
 Project-URL: Homepage, https://github.com/ggwpez/py-cargo-workspace
 Keywords: cargo,rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `cargo_workspace-1.2.4/pyproject.toml` & `cargo_workspace-1.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cargo_workspace"
-version = "1.2.4"
+version = "1.2.5"
 requires-python = ">=3.6"
 authors = [
     { name = "Oliver Tale-Yazdi", email="oliver@tasty.limo" },
 ]
 description = "Parse a cargo workspace and analyze its packages"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `cargo_workspace-1.2.4/tests/test_lib.py` & `cargo_workspace-1.2.5/tests/test_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,16 @@
 	assert crates[0].full_path == "../polkadot-sdk/bridges/bin/runtime-common/Cargo.toml"
 	assert crates[0].version.into_mmp() == Version(7)
 	assert crates[0].version.into_xyz() == Version(0, 7)
 	assert crates[0].version.suffix is None
 	assert crates[0].publish
  
 	deps = crates.find_by_name("polkadot-sdk-frame").dependencies
+	for _ in deps:
+		pass
 	assert len(deps) > 0
 	normal_dep = deps.find_by_name('frame-support')
 	assert normal_dep.name == 'frame-support'
 	assert crates.find_by_name("polkadot-sdk-frame").description == "Experimental: The single package to get you started with building frame pallets and runtimes"
 
 	assert len(crates.abs_paths) == len(crates)
 	assert len(crates.rel_paths) == len(crates)
```

