# Comparing `tmp/rustitude-0.4.3.tar.gz` & `tmp/rustitude-0.5.0.tar.gz`

## Comparing `rustitude-0.4.3.tar` & `rustitude-0.5.0.tar`

### file list

```diff
@@ -1,51 +1,61 @@
--rw-r--r--   0     1001      127      838 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-core/Cargo.toml
--rw-r--r--   0     1001      127    17815 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-core/CHANGELOG.md
--rw-r--r--   0     1001      127    10745 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-core/README.md
--rw-r--r--   0     1001      127    37877 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-core/src/amplitude.rs
--rw-r--r--   0     1001      127    25986 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-core/src/dataset.rs
--rw-r--r--   0     1001      127     1596 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-core/src/docs-header.html
--rw-r--r--   0     1001      127    10542 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-core/src/four_momentum.rs
--rw-r--r--   0     1001      127      826 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-core/src/lib.rs
--rw-r--r--   0     1001      127     2334 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-core/src/manager.rs
--rw-r--r--   0     1001      127      504 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-gluex/Cargo.toml
--rw-r--r--   0     1001      127     8577 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-gluex/CHANGELOG.md
--rw-r--r--   0     1001      127    14640 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-gluex/README.md
--rw-r--r--   0     1001      127    24055 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-gluex/media/logo.png
--rw-r--r--   0     1001      127     3079 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-gluex/src/dalitz.rs
--rw-r--r--   0     1001      127     8422 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-gluex/src/harmonics.rs
--rw-r--r--   0     1001      127       85 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-gluex/src/lib.rs
--rw-r--r--   0     1001      127    22196 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-gluex/src/resonances.rs
--rw-r--r--   0     1001      127     7499 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-gluex/src/sdmes.rs
--rw-r--r--   0     1001      127     7940 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude-gluex/src/utils.rs
--rw-r--r--   0     1001      127      500 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude/Cargo.toml
--rw-r--r--   0     1001      127    16165 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude/CHANGELOG.md
--rw-r--r--   0     1001      127     1029 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude/pyproject.toml
--rw-r--r--   0     1001      127      137 2024-05-16 00:20:20.000000 rustitude-0.4.3/crates/rustitude/src/lib.rs
--rw-r--r--   0     1001      127    10267 2024-05-16 00:20:20.000000 rustitude-0.4.3/README.md
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 rustitude-0.4.3/py-rustitude/Cargo.toml
--rw-r--r--   0     1001      127    13135 2024-05-16 00:20:20.000000 rustitude-0.4.3/py-rustitude/CHANGELOG.md
--rw-r--r--   0     1001      127     1507 2024-05-16 00:20:20.000000 rustitude-0.4.3/py-rustitude/LICENSE
--rw-r--r--   0     1001      127    10267 2024-05-16 00:20:20.000000 rustitude-0.4.3/py-rustitude/README.md
--rw-r--r--   0     1001      127     2846 2024-05-16 00:20:20.000000 rustitude-0.4.3/py-rustitude/bacon.toml
--rw-r--r--   0     1001      127     1841 2024-05-16 00:20:20.000000 rustitude-0.4.3/py-rustitude/rustitude/__init__.py
--rw-r--r--   0     1001      127     4013 2024-05-16 00:20:20.000000 rustitude-0.4.3/py-rustitude/rustitude/__init__.pyi
--rw-r--r--   0     1001      127       90 2024-05-16 00:20:20.000000 rustitude-0.4.3/py-rustitude/rustitude/gluex/__init__.pyi
--rw-r--r--   0     1001      127       75 2024-05-16 00:20:20.000000 rustitude-0.4.3/py-rustitude/rustitude/gluex/dalitz.pyi
--rw-r--r--   0     1001      127     3778 2024-05-16 00:20:20.000000 rustitude-0.4.3/py-rustitude/rustitude/gluex/harmonics.pyi
--rw-r--r--   0     1001      127      535 2024-05-16 00:20:20.000000 rustitude-0.4.3/py-rustitude/rustitude/gluex/resonances.pyi
--rw-r--r--   0     1001      127      336 2024-05-16 00:20:20.000000 rustitude-0.4.3/py-rustitude/rustitude/gluex/sdmes.pyi
--rw-r--r--   0     1001      127        0 2024-05-16 00:20:20.000000 rustitude-0.4.3/py-rustitude/rustitude/py.typed
--rw-r--r--   0     1001      127     1487 2024-05-16 00:20:20.000000 rustitude-0.4.3/py-rustitude/src/lib.rs
--rw-r--r--   0     1001      127    44937 2024-05-16 00:20:20.000000 rustitude-0.4.3/Cargo.lock
--rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 rustitude-0.4.3/Cargo.toml
--rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 rustitude-0.4.3/pyproject.toml
--rw-r--r--   0     1001      127     1841 2024-05-16 00:20:20.000000 rustitude-0.4.3/rustitude/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-16 00:20:20.000000 rustitude-0.4.3/rustitude/py.typed
--rw-r--r--   0     1001      127     4013 2024-05-16 00:20:20.000000 rustitude-0.4.3/rustitude/__init__.pyi
--rw-r--r--   0     1001      127       75 2024-05-16 00:20:20.000000 rustitude-0.4.3/rustitude/gluex/dalitz.pyi
--rw-r--r--   0     1001      127      535 2024-05-16 00:20:20.000000 rustitude-0.4.3/rustitude/gluex/resonances.pyi
--rw-r--r--   0     1001      127       90 2024-05-16 00:20:20.000000 rustitude-0.4.3/rustitude/gluex/__init__.pyi
--rw-r--r--   0     1001      127      336 2024-05-16 00:20:20.000000 rustitude-0.4.3/rustitude/gluex/sdmes.pyi
--rw-r--r--   0     1001      127     3778 2024-05-16 00:20:20.000000 rustitude-0.4.3/rustitude/gluex/harmonics.pyi
--rw-r--r--   0     1001      127     1507 2024-05-16 00:20:20.000000 rustitude-0.4.3/LICENSE
--rw-r--r--   0        0        0    10997 1970-01-01 00:00:00.000000 rustitude-0.4.3/PKG-INFO
+-rw-r--r--   0     1001      127      838 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-core/Cargo.toml
+-rw-r--r--   0     1001      127    21695 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-core/CHANGELOG.md
+-rw-r--r--   0     1001      127    10761 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-core/README.md
+-rw-r--r--   0     1001      127    35227 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-core/src/amplitude.rs
+-rw-r--r--   0     1001      127    24301 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-core/src/dataset.rs
+-rw-r--r--   0     1001      127     1596 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-core/src/docs-header.html
+-rw-r--r--   0     1001      127    10175 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-core/src/four_momentum.rs
+-rw-r--r--   0     1001      127     1766 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-core/src/lib.rs
+-rw-r--r--   0     1001      127     6718 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-core/src/manager.rs
+-rw-r--r--   0     1001      127      572 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude/Cargo.toml
+-rw-r--r--   0     1001      127    19286 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude/CHANGELOG.md
+-rw-r--r--   0     1001      127     2160 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude/benches/kmatrix.rs
+-rw-r--r--   0     1001      127  8752686 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude/benches/test_data.parquet
+-rw-r--r--   0     1001      127      137 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude/src/lib.rs
+-rw-r--r--   0     1001      127    10261 2024-05-24 09:29:07.000000 rustitude-0.5.0/README.md
+-rw-r--r--   0     1001      127      504 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-gluex/Cargo.toml
+-rw-r--r--   0     1001      127    10271 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-gluex/CHANGELOG.md
+-rw-r--r--   0     1001      127    14641 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-gluex/README.md
+-rw-r--r--   0     1001      127    24055 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-gluex/media/logo.png
+-rw-r--r--   0     1001      127     2798 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-gluex/src/dalitz.rs
+-rw-r--r--   0     1001      127     6522 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-gluex/src/harmonics.rs
+-rw-r--r--   0     1001      127       85 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-gluex/src/lib.rs
+-rw-r--r--   0     1001      127    20668 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-gluex/src/resonances.rs
+-rw-r--r--   0     1001      127     6766 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-gluex/src/sdmes.rs
+-rw-r--r--   0     1001      127     7940 2024-05-24 09:29:07.000000 rustitude-0.5.0/crates/rustitude-gluex/src/utils.rs
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 rustitude-0.5.0/py-rustitude/Cargo.toml
+-rw-r--r--   0     1001      127    15643 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/CHANGELOG.md
+-rw-r--r--   0     1001      127     1507 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/LICENSE
+-rw-r--r--   0     1001      127    10267 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/README.md
+-rw-r--r--   0     1001      127     2846 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/bacon.toml
+-rw-r--r--   0     1001      127     1905 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/rustitude/__init__.py
+-rw-r--r--   0     1001      127     5165 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/rustitude/__init__.pyi
+-rw-r--r--   0     1001      127       90 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/rustitude/gluex/__init__.pyi
+-rw-r--r--   0     1001      127       75 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/rustitude/gluex/dalitz.pyi
+-rw-r--r--   0     1001      127     3778 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/rustitude/gluex/harmonics.pyi
+-rw-r--r--   0     1001      127      535 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/rustitude/gluex/resonances.pyi
+-rw-r--r--   0     1001      127      336 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/rustitude/gluex/sdmes.pyi
+-rw-r--r--   0     1001      127        0 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/rustitude/py.typed
+-rw-r--r--   0     1001      127     6712 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/src/amplitude.rs
+-rw-r--r--   0     1001      127     7232 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/src/dataset.rs
+-rw-r--r--   0     1001      127     1517 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/src/four_momentum.rs
+-rw-r--r--   0     1001      127      374 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/src/gluex/dalitz.rs
+-rw-r--r--   0     1001      127     2095 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/src/gluex/harmonics.rs
+-rw-r--r--   0     1001      127      430 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/src/gluex/mod.rs
+-rw-r--r--   0     1001      127     1709 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/src/gluex/resonances.rs
+-rw-r--r--   0     1001      127      874 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/src/gluex/sdmes.rs
+-rw-r--r--   0     1001      127     1051 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/src/lib.rs
+-rw-r--r--   0     1001      127     7044 2024-05-24 09:29:07.000000 rustitude-0.5.0/py-rustitude/src/manager.rs
+-rw-r--r--   0     1001      127    46093 2024-05-24 09:29:07.000000 rustitude-0.5.0/Cargo.lock
+-rw-r--r--   0        0        0     1187 1970-01-01 00:00:00.000000 rustitude-0.5.0/Cargo.toml
+-rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 rustitude-0.5.0/pyproject.toml
+-rw-r--r--   0     1001      127     1905 2024-05-24 09:29:07.000000 rustitude-0.5.0/rustitude/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-24 09:29:07.000000 rustitude-0.5.0/rustitude/py.typed
+-rw-r--r--   0     1001      127     5165 2024-05-24 09:29:07.000000 rustitude-0.5.0/rustitude/__init__.pyi
+-rw-r--r--   0     1001      127       75 2024-05-24 09:29:07.000000 rustitude-0.5.0/rustitude/gluex/dalitz.pyi
+-rw-r--r--   0     1001      127      535 2024-05-24 09:29:07.000000 rustitude-0.5.0/rustitude/gluex/resonances.pyi
+-rw-r--r--   0     1001      127       90 2024-05-24 09:29:07.000000 rustitude-0.5.0/rustitude/gluex/__init__.pyi
+-rw-r--r--   0     1001      127      336 2024-05-24 09:29:07.000000 rustitude-0.5.0/rustitude/gluex/sdmes.pyi
+-rw-r--r--   0     1001      127     3778 2024-05-24 09:29:07.000000 rustitude-0.5.0/rustitude/gluex/harmonics.pyi
+-rw-r--r--   0     1001      127     1507 2024-05-24 09:29:07.000000 rustitude-0.5.0/LICENSE
+-rw-r--r--   0        0        0    10997 1970-01-01 00:00:00.000000 rustitude-0.5.0/PKG-INFO
```

### Comparing `rustitude-0.4.3/crates/rustitude-core/Cargo.toml` & `rustitude-0.5.0/crates/rustitude-core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rustitude-core"
-version = "1.0.1"
+version = "1.1.0"
 edition = { workspace = true }
 authors = { workspace = true }
 description = { workspace = true }
 repository = { workspace = true }
 homepage = { workspace = true }
 license-file = { workspace = true }
```

### Comparing `rustitude-0.4.3/crates/rustitude-core/CHANGELOG.md` & `rustitude-0.5.0/crates/rustitude-core/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,68 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 1.1.0 (2024-05-24)
+
+### Documentation
+
+ - <csr-id-7867bc0bf9c47203f94c8720a1e84d6e86ed159d/> Update README.md
+
+### New Features
+
+ - <csr-id-d2a94a57466c0b2556850315b8902cf9528598de/> additional API so python interactions with managers can actually modify the amplitudes they manage
+ - <csr-id-6955773a3e96890efa4573d5c7bc355bb23a07e6/> add RustitudeError and remove unwraps, error handling should work in python as well
+ - <csr-id-b495892674a3fad4937de6e830241230b52880c3/> update benchmark and itertools dep, which deprecated group_by -> chunk_by
+ - <csr-id-8b1eee79d545caaca39b8b38be1f00f7762adcda/> make Model::new public to allow for proper benchmarking, and add divan benchmark for basic kmatrix
+
+### Bug Fixes
+
+ - <csr-id-dba3b5bbd9b93622c32e6042062d75da972c073e/> remove unsafe transmutes, they weren't working properly and probably aren't needed anyway
+ - <csr-id-14359c9e7af9a155c1fe64e7f809f3a4771c5e1f/> pass model and dataset to manager as reference to avoid issues using the model later, might change the way the dataset is cloned in the future
+ - <csr-id-405ed0cb2ad417ccf0041a49ce6fbd6b6693539c/> bump versions
+
+### Commit Statistics
+
+<csr-read-only-do-not-edit/>
+
+ - 11 commits contributed to the release over the course of 2 calendar days.
+ - 8 days passed between releases.
+ - 8 commits were understood as [conventional](https://www.conventionalcommits.org).
+ - 0 issues like '(#ID)' were seen in commit messages
+
+### Commit Details
+
+<csr-read-only-do-not-edit/>
+
+<details><summary>view details</summary>
+
+ * **Uncategorized**
+    - Bump versions ([`405ed0c`](https://github.com/denehoffman/rustitude/commit/405ed0cb2ad417ccf0041a49ce6fbd6b6693539c))
+    - Update README.md ([`7867bc0`](https://github.com/denehoffman/rustitude/commit/7867bc0bf9c47203f94c8720a1e84d6e86ed159d))
+    - Merge pull request #3 from denehoffman/python_reorg ([`467caac`](https://github.com/denehoffman/rustitude/commit/467caacc688f94c074d28be1ec54a422d8d9ebc0))
+    - Additional API so python interactions with managers can actually modify the amplitudes they manage ([`d2a94a5`](https://github.com/denehoffman/rustitude/commit/d2a94a57466c0b2556850315b8902cf9528598de))
+    - Remove unsafe transmutes, they weren't working properly and probably aren't needed anyway ([`dba3b5b`](https://github.com/denehoffman/rustitude/commit/dba3b5bbd9b93622c32e6042062d75da972c073e))
+    - Add RustitudeError and remove unwraps, error handling should work in python as well ([`6955773`](https://github.com/denehoffman/rustitude/commit/6955773a3e96890efa4573d5c7bc355bb23a07e6))
+    - Move all pyo3 code to the py-rustitude crate ([`9bcdb46`](https://github.com/denehoffman/rustitude/commit/9bcdb4615fdb4df5b4566673fbed955930926b7c))
+    - Merge pull request #2 from denehoffman/create_benchmarks ([`1297b92`](https://github.com/denehoffman/rustitude/commit/1297b9275dfac49f2591573b46438ff588a77c51))
+    - Update benchmark and itertools dep, which deprecated group_by -> chunk_by ([`b495892`](https://github.com/denehoffman/rustitude/commit/b495892674a3fad4937de6e830241230b52880c3))
+    - Pass model and dataset to manager as reference to avoid issues using the model later, might change the way the dataset is cloned in the future ([`14359c9`](https://github.com/denehoffman/rustitude/commit/14359c9e7af9a155c1fe64e7f809f3a4771c5e1f))
+    - Make Model::new public to allow for proper benchmarking, and add divan benchmark for basic kmatrix ([`8b1eee7`](https://github.com/denehoffman/rustitude/commit/8b1eee79d545caaca39b8b38be1f00f7762adcda))
+</details>
+
 ## 1.0.1 (2024-05-16)
 
+<csr-id-b08b3b8c8c4699a65dabdac5ff4b19fe50f511aa/>
+<csr-id-9089c84e481124ff764b24f42507ab14913fef07/>
+<csr-id-0e94ec45850cb6129924b2be27793a17c51b03c2/>
+
 ### Documentation
 
  - <csr-id-8824d4c02278fd01de0050be3c3b9c3781e39687/> update readme link
  - <csr-id-27799fd50850d43e50c42bfc24f5c9d36b6f76d7/> Update README.md (missed a spot)
  - <csr-id-53c553d44045715f91710a266e7e5f39cc71d9c9/> update readmes
 
 ### Refactor
@@ -22,26 +74,27 @@
 
  - <csr-id-0e94ec45850cb6129924b2be27793a17c51b03c2/> get rid of extra git-files and media
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
 
- - 6 commits contributed to the release.
+ - 7 commits contributed to the release.
  - 1 day passed between releases.
  - 6 commits were understood as [conventional](https://www.conventionalcommits.org).
  - 0 issues like '(#ID)' were seen in commit messages
 
 ### Commit Details
 
 <csr-read-only-do-not-edit/>
 
 <details><summary>view details</summary>
 
  * **Uncategorized**
+    - Release rustitude-core v1.0.1, rustitude-gluex v0.2.2, rustitude v0.4.3 ([`fe0c603`](https://github.com/denehoffman/rustitude/commit/fe0c6036d4816587b1d65ae2697f3b241cfe579c))
     - Get rid of extra git-files and media ([`0e94ec4`](https://github.com/denehoffman/rustitude/commit/0e94ec45850cb6129924b2be27793a17c51b03c2))
     - Update readme link ([`8824d4c`](https://github.com/denehoffman/rustitude/commit/8824d4c02278fd01de0050be3c3b9c3781e39687))
     - Change Amplitude such that new makes a new Amplitude, add conversion traits to AmpOp and PyAmpOp, and fix amplitude! macro ([`b08b3b8`](https://github.com/denehoffman/rustitude/commit/b08b3b8c8c4699a65dabdac5ff4b19fe50f511aa))
     - Major move required to have rustitude function properly as a Rust crate. I set this up very wrong the first time ([`9089c84`](https://github.com/denehoffman/rustitude/commit/9089c84e481124ff764b24f42507ab14913fef07))
     - Update README.md (missed a spot) ([`27799fd`](https://github.com/denehoffman/rustitude/commit/27799fd50850d43e50c42bfc24f5c9d36b6f76d7))
     - Update readmes ([`53c553d`](https://github.com/denehoffman/rustitude/commit/53c553d44045715f91710a266e7e5f39cc71d9c9))
 </details>
```

### Comparing `rustitude-0.4.3/crates/rustitude-core/README.md` & `rustitude-0.5.0/crates/rustitude-core/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 pub struct OmegaDalitz {
     dalitz_z: Vec<f64>,
     dalitz_sin3theta: Vec<f64>,
     lambda: Vec<f64>,
 }
 
 impl Node for OmegaDalitz {
-    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
+    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), RustitudeError> {
         (self.dalitz_z, (self.dalitz_sin3theta, self.lambda)) = dataset
             .events
             .read()
             .par_iter()
             .map(|event| {
                 let pi0 = event.daughter_p4s[0];
                 let pip = event.daughter_p4s[1];
@@ -101,15 +101,15 @@
 
                 (dalitz_z, (dalitz_sin3theta, lambda))
             })
             .unzip();
         Ok(())
     }
 
-    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError> {
+    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, RustitudeError> {
         let dalitz_z = self.dalitz_z[event.index];
         let dalitz_sin3theta = self.dalitz_sin3theta[event.index];
         let lambda = self.lambda[event.index];
         let alpha = parameters[0];
         let beta = parameters[1];
         let gamma = parameters[2];
         let delta = parameters[3];
@@ -133,17 +133,17 @@
         ]
     }
 }
 ```
 
 Let's walk through this code. First, we need to define a `struct` which has all of the general information about the amplitude, and in this case some kind of `Vec` for storing precalculated data. We consider this precalculated data to correspond to a single dataset, and each dataset gets its own copy of the amplitude `struct`. Because this particular amplitude doesn't have any input parameters, we can `#[derive(Default)]` on it to make a default constructor, which allows the amplitude to be initialized with something like `let amp = OmegaDalitz::default();`. If we wanted a parameterized constructor, we have to define our own, and while Rust has no default name for constructors, `pub fn new(...) -> rustitude_core::AmpOp` is preferred.
 
-Next, we implement the `Node` trait for the `struct`. Traits in Rust are kind of like abstract classes or interfaces in object-oriented languages, they provide some set of methods which a `struct` must implement. The first of these methods is `fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError>`. As the signature suggests, it takes a `Dataset` and mutates the `struct` in some way. It should raise a `NodeError` if anything goes wrong in the evaluation. The intended usage of this function is to precalculate some terms in the amplitude's mathematical expression, things which don't change when you update the free parameter inputs to the amplitude. In this case, the four input parameters, $`\alpha`$, $`\beta`$, $`\gamma`$, and $`\delta`$, are independent from `dalitz_z`, `dalitz_sin3theta`, and `lambda`, so we can safely calculate those ahead of time and just pull from their respective `Vec`s when needed later. I won't go too far into Rust's syntax here, but typical precalculation functions will start by iterating over the dataset's events in parallel (the line `use rayon::prelude::*;` is needed to use `par_iter` here) and collecting or unzipping that iterator into a `Vec` or group of `Vec`s.
+Next, we implement the `Node` trait for the `struct`. Traits in Rust are kind of like abstract classes or interfaces in object-oriented languages, they provide some set of methods which a `struct` must implement. The first of these methods is `fn precalculate(&mut self, dataset: &Dataset) -> Result<(), RustitudeError>`. As the signature suggests, it takes a `Dataset` and mutates the `struct` in some way. It should raise a `RustitudeError` if anything goes wrong in the evaluation. The intended usage of this function is to precalculate some terms in the amplitude's mathematical expression, things which don't change when you update the free parameter inputs to the amplitude. In this case, the four input parameters, $`\alpha`$, $`\beta`$, $`\gamma`$, and $`\delta`$, are independent from `dalitz_z`, `dalitz_sin3theta`, and `lambda`, so we can safely calculate those ahead of time and just pull from their respective `Vec`s when needed later. I won't go too far into Rust's syntax here, but typical precalculation functions will start by iterating over the dataset's events in parallel (the line `use rayon::prelude::*;` is needed to use `par_iter` here) and collecting or unzipping that iterator into a `Vec` or group of `Vec`s.
 
-The calculate step has the signature `fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError>`. This means we need to take a list of parameters and a single event and turn them into a complex value. The `Event` struct contains an `index` field which can be used to access the precalculated storage arrays made in the previous step.
+The calculate step has the signature `fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, RustitudeError>`. This means we need to take a list of parameters and a single event and turn them into a complex value. The `Event` struct contains an `index` field which can be used to access the precalculated storage arrays made in the previous step.
 
 Finally, the `parameters` function just returns a list of the parameter names in the order they are expected to be input into `calculate`. In the event that an amplitude doesn't have any free parameters (like [my implementation of the `Ylm` and `Zlm` amplitudes](https://github.com/denehoffman/rustitude/blob/main/crates/rustitude-gluex/src/harmonics.rs)), we can omit this function entirely, as the default implementation returns `vec![]`.
 
 And that's it! However, it is important to be aware of the steps which need to be taken to allow this amplitude to be used through the Python interface.
 
 ## Python Bindings
 
@@ -151,16 +151,16 @@
 
 ```rust
 use pyo3::prelude::*;
 
 // OmegaDalitz code here
 
 #[pyfunction(name = "OmegaDalitz")]
-fn omega_dalitz(name: &str) -> PyAmpOp {
-    Amplitude::new(name, Box::<OmegaDalitz>::default()).into()
+fn omega_dalitz(name: &str) -> AmpOp {
+    Amplitude::new(name, OmegaDalitz::default()).into()
 }
 
 pub fn pyo3_module(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(omega_dalitz, m)?)?;
     Ok(())
 }
 ```
```

#### html2text {}

```diff
@@ -31,15 +31,15 @@
 combinations, it is important to know how to design an amplitude which will
 work seamlessly with this crate. Let's write down the `rustitude` version of
 the [OmegaDalitz](https://github.com/JeffersonLab/halld_sim/blob/
 6544f01ac1514b0b9a53ad241cf2e8a63e1d3dfa/src/libraries/AMPTOOLS_AMPS/
 OmegaDalitz.cc) amplitude: ```rust use rayon::prelude::*; use rustitude_core::
 prelude::*; #[derive(Default)] pub struct OmegaDalitz { dalitz_z: Vec,
 dalitz_sin3theta: Vec, lambda: Vec, } impl Node for OmegaDalitz { fn
-precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
+precalculate(&mut self, dataset: &Dataset) -> Result<(), RustitudeError> {
 (self.dalitz_z, (self.dalitz_sin3theta, self.lambda)) = dataset .events .read()
 .par_iter() .map(|event| { let pi0 = event.daughter_p4s[0]; let pip =
 event.daughter_p4s[1]; let pim = event.daughter_p4s[2]; let omega = pi0 + pip +
 pim; let dalitz_s = (pip + pim).m2(); let dalitz_t = (pip + pi0).m2(); let
 dalitz_u = (pim + pi0).m2(); let m3pi = (2.0 * pip.m()) + pi0.m(); let dalitz_d
 = 2.0 * omega.m() * (omega.m() - m3pi); let dalitz_sc = (1.0 / 3.0) * (omega.m2
 () + pip.m2() + pim.m2() + pi0.m2()); let dalitz_x = f64::sqrt(3.0) * (dalitz_t
@@ -47,65 +47,65 @@
 let dalitz_z = dalitz_x * dalitz_x + dalitz_y * dalitz_y; let dalitz_sin3theta
 = f64::sin(3.0 * f64::asin(dalitz_y / f64::sqrt(dalitz_z))); let pip_omega =
 pip.boost_along(ω); let pim_omega = pim.boost_along(ω); let pi_cross =
 pip_omega.momentum().cross(&pim_omega.momentum()); let lambda = (4.0 / 3.0) *
 f64::abs(pi_cross.dot(π_cross)) / ((1.0 / 9.0) * (omega.m2() - (2.0 * pip.m() +
 pi0.m()).powi(2)).powi(2)); (dalitz_z, (dalitz_sin3theta, lambda)) }) .unzip();
 Ok(()) } fn calculate(&self, parameters: &[f64], event: &Event) -> Result
- NodeError> { let dalitz_z = self.dalitz_z[event.index]; let dalitz_sin3theta =
-self.dalitz_sin3theta[event.index]; let lambda = self.lambda[event.index]; let
-alpha = parameters[0]; let beta = parameters[1]; let gamma = parameters[2]; let
-delta = parameters[3]; Ok(f64::sqrt(f64::abs( lambda * (1.0 + 2.0 * alpha *
-dalitz_z + 2.0 * beta * dalitz_z.powf(3.0 / 2.0) * dalitz_sin3theta + 2.0 *
-gamma * dalitz_z.powi(2) + 2.0 * delta * dalitz_z.powf(5.0 / 2.0) *
-dalitz_sin3theta), )) .into()) } fn parameters(&self) -> Vec { vec!
-[ "alpha".to_string(), "beta".to_string(), "gamma".to_string(),
+ RustitudeError> { let dalitz_z = self.dalitz_z[event.index]; let
+dalitz_sin3theta = self.dalitz_sin3theta[event.index]; let lambda = self.lambda
+[event.index]; let alpha = parameters[0]; let beta = parameters[1]; let gamma =
+parameters[2]; let delta = parameters[3]; Ok(f64::sqrt(f64::abs( lambda * (1.0
++ 2.0 * alpha * dalitz_z + 2.0 * beta * dalitz_z.powf(3.0 / 2.0) *
+dalitz_sin3theta + 2.0 * gamma * dalitz_z.powi(2) + 2.0 * delta * dalitz_z.powf
+(5.0 / 2.0) * dalitz_sin3theta), )) .into()) } fn parameters(&self) -> Vec
+{ vec![ "alpha".to_string(), "beta".to_string(), "gamma".to_string(),
 "delta".to_string(), ] } } ``` Let's walk through this code. First, we need to
 define a `struct` which has all of the general information about the amplitude,
 and in this case some kind of `Vec` for storing precalculated data. We consider
 this precalculated data to correspond to a single dataset, and each dataset
 gets its own copy of the amplitude `struct`. Because this particular amplitude
 doesn't have any input parameters, we can `#[derive(Default)]` on it to make a
 default constructor, which allows the amplitude to be initialized with
 something like `let amp = OmegaDalitz::default();`. If we wanted a
 parameterized constructor, we have to define our own, and while Rust has no
 default name for constructors, `pub fn new(...) -> rustitude_core::AmpOp` is
 preferred. Next, we implement the `Node` trait for the `struct`. Traits in Rust
 are kind of like abstract classes or interfaces in object-oriented languages,
 they provide some set of methods which a `struct` must implement. The first of
 these methods is `fn precalculate(&mut self, dataset: &Dataset) -> Result<(),
-NodeError>`. As the signature suggests, it takes a `Dataset` and mutates the
-`struct` in some way. It should raise a `NodeError` if anything goes wrong in
-the evaluation. The intended usage of this function is to precalculate some
-terms in the amplitude's mathematical expression, things which don't change
-when you update the free parameter inputs to the amplitude. In this case, the
-four input parameters, $`\alpha`$, $`\beta`$, $`\gamma`$, and $`\delta`$, are
-independent from `dalitz_z`, `dalitz_sin3theta`, and `lambda`, so we can safely
-calculate those ahead of time and just pull from their respective `Vec`s when
-needed later. I won't go too far into Rust's syntax here, but typical
-precalculation functions will start by iterating over the dataset's events in
-parallel (the line `use rayon::prelude::*;` is needed to use `par_iter` here)
-and collecting or unzipping that iterator into a `Vec` or group of `Vec`s. The
-calculate step has the signature `fn calculate(&self, parameters: &[f64],
-event: &Event) -> Result
- NodeError>`. This means we need to take a list of parameters and a single
+RustitudeError>`. As the signature suggests, it takes a `Dataset` and mutates
+the `struct` in some way. It should raise a `RustitudeError` if anything goes
+wrong in the evaluation. The intended usage of this function is to precalculate
+some terms in the amplitude's mathematical expression, things which don't
+change when you update the free parameter inputs to the amplitude. In this
+case, the four input parameters, $`\alpha`$, $`\beta`$, $`\gamma`$, and
+$`\delta`$, are independent from `dalitz_z`, `dalitz_sin3theta`, and `lambda`,
+so we can safely calculate those ahead of time and just pull from their
+respective `Vec`s when needed later. I won't go too far into Rust's syntax
+here, but typical precalculation functions will start by iterating over the
+dataset's events in parallel (the line `use rayon::prelude::*;` is needed to
+use `par_iter` here) and collecting or unzipping that iterator into a `Vec` or
+group of `Vec`s. The calculate step has the signature `fn calculate(&self,
+parameters: &[f64], event: &Event) -> Result
+ RustitudeError>`. This means we need to take a list of parameters and a single
 event and turn them into a complex value. The `Event` struct contains an
 `index` field which can be used to access the precalculated storage arrays made
 in the previous step. Finally, the `parameters` function just returns a list of
 the parameter names in the order they are expected to be input into
 `calculate`. In the event that an amplitude doesn't have any free parameters
 (like [my implementation of the `Ylm` and `Zlm` amplitudes](https://github.com/
 denehoffman/rustitude/blob/main/crates/rustitude-gluex/src/harmonics.rs)), we
 can omit this function entirely, as the default implementation returns `vec!
 []`. And that's it! However, it is important to be aware of the steps which
 need to be taken to allow this amplitude to be used through the Python
 interface. ## Python Bindings To make Python bindings, `pyo3` needs to be
 included as a dependency: ```rust use pyo3::prelude::*; // OmegaDalitz code
-here #[pyfunction(name = "OmegaDalitz")] fn omega_dalitz(name: &str) -> PyAmpOp
-{ Amplitude::new(name, Box::::default()).into() } pub fn pyo3_module(m:
+here #[pyfunction(name = "OmegaDalitz")] fn omega_dalitz(name: &str) -> AmpOp
+{ Amplitude::new(name, OmegaDalitz::default()).into() } pub fn pyo3_module(m:
 &Bound<'_, PyModule>) -> PyResult<()> { m.add_function(wrap_pyfunction!
 (omega_dalitz, m)?)?; Ok(()) } ``` Rather than bind the `struct` directly, we
 prefer to bind a function which returns a `PyAmpOp`, a wrapper struct that
 implements `#[pyclass]` and can be used in the Python interface. The
 `pyo3_module` function will then need to be added to the `rustitude` crate's
 [`lib.rs`](https://github.com/denehoffman/rustitude/blob/main/src/lib.rs) file.
 This step is a bit problematic, since it means new amplitudes cannot be added
```

### Comparing `rustitude-0.4.3/crates/rustitude-core/src/amplitude.rs` & `rustitude-0.5.0/crates/rustitude-core/src/amplitude.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,33 @@
 use itertools::Itertools;
 use num::complex::Complex64;
 use parking_lot::RwLock;
-use pyo3::prelude::*;
 use rayon::prelude::*;
 use std::{
     collections::HashSet,
     fmt::{Debug, Display},
     ops::{Add, Mul},
     sync::Arc,
 };
-use thiserror::Error;
 
-use crate::dataset::{Dataset, Event};
+use crate::{
+    dataset::{Dataset, Event},
+    errors::RustitudeError,
+};
 
-#[pyclass]
 #[derive(Clone)]
 pub struct Parameter {
-    #[pyo3(get)]
     pub amplitude: String,
-    #[pyo3(get)]
     pub name: String,
-    #[pyo3(get)]
-    index: Option<usize>,
-    #[pyo3(get)]
-    fixed_index: Option<usize>,
-    #[pyo3(get)]
-    initial: f64,
-    #[pyo3(get)]
-    bounds: (f64, f64),
+    pub index: Option<usize>,
+    pub fixed_index: Option<usize>,
+    pub initial: f64,
+    pub bounds: (f64, f64),
 }
-#[pymethods]
 impl Parameter {
-    fn __str__(&self) -> String {
-        format!("{}", self)
-    }
-    fn __repr__(&self) -> String {
-        format!("{:?}", self)
-    }
-    #[new]
     pub fn new(amplitude: &str, name: &str, index: usize) -> Self {
         Self {
             amplitude: amplitude.to_string(),
             name: name.to_string(),
             index: Some(index),
             fixed_index: None,
             initial: 0.0,
@@ -84,30 +70,21 @@
         }
     }
 }
 
 /// Creates a wrapped [`AmpOp`] which can be registered by a [`crate::amplitude::Model`].
 ///
 /// This macro is a convenience method which takes a name and a [`Node`] and generates a new [`AmpOp`].
-/// ```
 #[macro_export]
 macro_rules! amplitude {
     ($name:expr, $node:expr) => {{
         Amplitude::new($name, $node).into()
     }};
 }
 
-#[derive(Debug, Clone, Error)]
-pub enum NodeError {
-    #[error("invalid parameter value")]
-    InvalidParameterValue(String),
-    #[error("evaluation error")]
-    EvaluationError(String),
-}
-
 /// A trait which contains all the required methods for a functioning [`Amplitude`].
 ///
 /// The [`Node`] trait represents any mathematical structure which takes in some parameters and some
 /// [`Event`] data and computes a [`Complex64`] for each [`Event`]. This is the fundamental
 /// building block of all analyses built with Rustitude. Nodes are intended to be optimized at the
 /// user level, so they should be implemented on structs which can store some precalculated data.
 ///
@@ -163,15 +140,15 @@
 /// impl Ylm {
 ///     fn new(wave: Wave) -> Self {
 ///         Self(wave, Vec::default())
 ///     }
 /// }
 /// impl Node for Ylm {
 ///     fn parameters(&self) -> Vec<String> { vec![] }
-///     fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
+///     fn precalculate(&mut self, dataset: &Dataset) -> Result<(), RustitudeError> {
 ///         self.1 = dataset.events.read()
 ///             .par_iter()
 ///             .map(|event| {
 ///                 let resonance = event.daughter_p4s[0] + event.daughter_p4s[1];
 ///                 let p1 = event.daughter_p4s[0];
 ///                 let recoil_res = event.recoil_p4.boost_along(&resonance); // Boost to helicity frame
 ///                 let p1_res = p1.boost_along(&resonance);
@@ -185,27 +162,27 @@
 ///                 let p = Coordinates::cartesian(p1_vec.dot(&x), p1_vec.dot(&y), p1_vec.dot(&z));
 ///                 ComplexSH::Spherical.eval(self.0.l(), self.0.m(), &p)
 ///             })
 ///             .collect();
 ///         Ok(())
 ///     }
 ///
-///     fn calculate(&self, _parameters: &[f64], event: &Event) -> Result<Complex64, NodeError> {
+///     fn calculate(&self, _parameters: &[f64], event: &Event) -> Result<Complex64, RustitudeError> {
 ///         Ok(self.1[event.index])
 ///     }
 /// }
 /// ```
 ///
 /// A [`Node`] which computes a single complex scalar entirely determined by input parameters:
 ///
 /// ```
 /// use rustitude_core::prelude::*;
 /// struct ComplexScalar;
 /// impl Node for ComplexScalar {
-///     fn calculate(&self, parameters: &[f64], _event: &Event) -> Result<Complex64, NodeError> {
+///     fn calculate(&self, parameters: &[f64], _event: &Event) -> Result<Complex64, RustitudeError> {
 ///         Ok(Complex64::new(parameters[0], parameters[1]))
 ///     }
 ///
 ///     fn parameters(&self) -> Vec<String> {
 ///         vec!["real".to_string(), "imag".to_string()]
 ///     }
 /// }
@@ -213,73 +190,39 @@
 pub trait Node: Sync + Send {
     /// A method that is run once and stores some precalculated values given a [`Dataset`] input.
     ///
     /// This method is intended to run expensive calculations which don't actually depend on the
     /// parameters. For instance, to calculate a spherical harmonic, we don't actually need any
     /// other information than what is contained in the [`Event`], so we can calculate a spherical
     /// harmonic for every event once and then retrieve the data in the [`Node::calculate`] method.
-    fn precalculate(&mut self, _dataset: &Dataset) -> Result<(), NodeError> {
+    fn precalculate(&mut self, _dataset: &Dataset) -> Result<(), RustitudeError> {
         Ok(())
     }
 
     /// A method which runs every time the amplitude is evaluated and produces a [`Complex64`].
     ///
     /// Because this method is run on every evaluation, it should be as lean as possible.
     /// Additionally, you should avoid [`rayon`]'s parallel loops inside this method since we
     /// already parallelize over the [`Dataset`]. This method expects a single [`Event`] as well as
     /// a slice of [`f64`]s. This slice is guaranteed to have the same length and order as
     /// specified in the [`Node::parameters`] method, or it will be empty if that method returns
     /// [`None`].
-    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError>;
+    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, RustitudeError>;
 
     /// A method which specifies the number and order of parameters used by the [`Node`].
     ///
     /// This method tells the [`crate::manager::Manager`] how to assign its input [`Vec`] of parameter values to
     /// each [`Node`]. If this method returns [`None`], it is implied that the [`Node`] takes no
     /// parameters as input. Otherwise, the parameter names should be listed in the same order they
     /// are expected to be given as input to the [`Node::calculate`] method.
     fn parameters(&self) -> Vec<String> {
         vec![]
     }
 }
 
-#[pyclass(name = "AmpOp")]
-#[derive(Clone)]
-pub struct PyAmpOp {
-    pub op: AmpOp,
-}
-
-impl From<AmpOp> for PyAmpOp {
-    fn from(value: AmpOp) -> Self {
-        Self { op: value }
-    }
-}
-
-#[pymethods]
-impl PyAmpOp {
-    pub fn print_tree(&self) {
-        self.op.print_tree()
-    }
-    pub fn real(&self) -> Self {
-        self.op.real().into()
-    }
-    pub fn imag(&self) -> Self {
-        self.op.imag().into()
-    }
-    pub fn norm_sqr(&self) -> Self {
-        self.op.norm_sqr().into()
-    }
-    pub fn __add__(&self, other: Self) -> Self {
-        (self.op.clone() + other.op).into()
-    }
-    pub fn __mul__(&self, other: Self) -> Self {
-        (self.op.clone() * other.op).into()
-    }
-}
-
 #[derive(Clone)]
 pub enum AmpOp {
     Amplitude(Amplitude),
     Sum(Vec<AmpOp>),
     Product(Vec<AmpOp>),
     Real(Box<AmpOp>),
     Imag(Box<AmpOp>),
@@ -553,29 +496,24 @@
 /// A struct which stores a named [`Node`].
 ///
 /// The [`Amplitude`] struct turns a [`Node`] trait into a concrete type and also stores a name
 /// associated with the [`Node`]. This allows us to distinguish multiple uses of the same [`Node`]
 /// in an analysis, and makes each [`Node`]'s parameters unique.
 ///
 /// This is mostly used interally as an intermediate step to an [`AmpOp`].
-#[pyclass]
 #[derive(Clone)]
 pub struct Amplitude {
     /// A name which uniquely identifies an [`Amplitude`] within a sum and group.
-    #[pyo3(get)]
     pub name: String,
     /// A [`Node`] which contains all of the operations needed to compute a [`Complex64`] from an
     /// [`Event`] in a [`Dataset`], a [`Vec<f64>`] of parameter values, and possibly some
     /// precomputed values.
     pub node: Arc<RwLock<Box<dyn Node>>>,
-    #[pyo3(get)]
     pub active: bool,
-    #[pyo3(get)]
     pub cache_position: usize,
-    #[pyo3(get)]
     pub parameter_index_start: usize,
 }
 impl Debug for Amplitude {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         f.debug_struct("Amplitude")
             .field("name", &self.name)
             .field("active", &self.active)
@@ -589,33 +527,19 @@
         if self.active {
             write!(f, "{}", self.name)
         } else {
             write!(f, "# {} #", self.name)
         }
     }
 }
-#[pymethods]
-impl Amplitude {
-    fn __str__(&self) -> String {
-        format!("{}", self)
-    }
-    fn __repr__(&self) -> String {
-        format!("{:?}", self)
-    }
-}
 impl From<Amplitude> for AmpOp {
     fn from(amp: Amplitude) -> Self {
         Self::Amplitude(amp)
     }
 }
-impl From<Amplitude> for PyAmpOp {
-    fn from(amp: Amplitude) -> Self {
-        AmpOp::Amplitude(amp).into()
-    }
-}
 impl Amplitude {
     pub fn new(name: &str, node: impl Node + 'static) -> Self {
         Self {
             name: name.to_string(),
             node: Arc::new(RwLock::new(Box::new(node))),
             active: true,
             cache_position: 0,
@@ -623,60 +547,61 @@
         }
     }
     pub fn register(
         &mut self,
         cache_position: usize,
         parameter_index_start: usize,
         dataset: &Dataset,
-    ) -> Result<(), NodeError> {
+    ) -> Result<(), RustitudeError> {
         self.cache_position = cache_position;
         self.parameter_index_start = parameter_index_start;
         self.precalculate(dataset)
     }
 }
 impl Node for Amplitude {
-    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
+    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), RustitudeError> {
         self.node.write().precalculate(dataset)
     }
-    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError> {
+    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, RustitudeError> {
         self.node.read().calculate(
             &parameters
                 [self.parameter_index_start..self.parameter_index_start + self.parameters().len()],
             event,
         )
     }
     fn parameters(&self) -> Vec<String> {
         self.node.read().parameters()
     }
 }
 
-#[pyclass]
 #[derive(Debug, Clone)]
 pub struct Model {
     pub root: AmpOp,
-    #[pyo3(get)]
     pub amplitudes: Vec<Amplitude>,
-    #[pyo3(get)]
     pub parameters: Vec<Parameter>,
 }
 
-#[pymethods]
 impl Model {
-    #[new]
-    fn from_pyampop(root: PyAmpOp) -> Self {
-        Self::new(root.op)
-    }
-    #[getter]
-    fn get_root(&self) -> PyResult<PyAmpOp> {
-        Ok(self.root.clone().into())
+    pub fn get_amplitude(&self, amplitude_name: &str) -> Result<Amplitude, RustitudeError> {
+        self.amplitudes
+            .iter()
+            .find(|a: &&Amplitude| a.name == amplitude_name)
+            .ok_or_else(|| RustitudeError::AmplitudeNotFoundError(amplitude_name.to_string()))
+            .cloned()
     }
-    pub fn get_parameter(&self, amplitude_name: &str, parameter_name: &str) -> Option<Parameter> {
+    pub fn get_parameter(
+        &self,
+        amplitude_name: &str,
+        parameter_name: &str,
+    ) -> Result<Parameter, RustitudeError> {
+        self.get_amplitude(amplitude_name)?;
         self.parameters
             .iter()
             .find(|p: &&Parameter| p.amplitude == amplitude_name && p.name == parameter_name)
+            .ok_or_else(|| RustitudeError::ParameterNotFoundError(parameter_name.to_string()))
             .cloned()
     }
     pub fn print_parameters(&self) {
         let any_fixed = if self.any_fixed() { 1 } else { 0 };
         if self.any_fixed() {
             println!(
                 "Fixed: {}",
@@ -696,17 +621,17 @@
     }
     pub fn constrain(
         &mut self,
         amplitude_1: &str,
         parameter_1: &str,
         amplitude_2: &str,
         parameter_2: &str,
-    ) {
-        let p1 = self.get_parameter(amplitude_1, parameter_1).unwrap();
-        let p2 = self.get_parameter(amplitude_2, parameter_2).unwrap();
+    ) -> Result<(), RustitudeError> {
+        let p1 = self.get_parameter(amplitude_1, parameter_1)?;
+        let p2 = self.get_parameter(amplitude_2, parameter_2)?;
         for par in self.parameters.iter_mut() {
             // None < Some(0)
             match p1.index.cmp(&p2.index) {
                 // p1 < p2
                 std::cmp::Ordering::Less => {
                     if par.index == p2.index {
                         par.index = p1.index;
@@ -722,70 +647,90 @@
                         par.initial = p2.initial;
                         par.fixed_index = p2.fixed_index;
                     }
                 }
             }
         }
         self.reindex_parameters();
+        Ok(())
     }
 
-    pub fn fix(&mut self, amplitude: &str, parameter: &str, value: f64) {
-        let search_par = self.get_parameter(amplitude, parameter).unwrap();
+    pub fn fix(
+        &mut self,
+        amplitude: &str,
+        parameter: &str,
+        value: f64,
+    ) -> Result<(), RustitudeError> {
+        let search_par = self.get_parameter(amplitude, parameter)?;
         let fixed_index = self.get_min_fixed_index();
         for par in self.parameters.iter_mut() {
             if par.index == search_par.index {
                 par.index = None;
                 par.initial = value;
                 par.fixed_index = fixed_index;
             }
         }
         self.reindex_parameters();
+        Ok(())
     }
-    pub fn free(&mut self, amplitude: &str, parameter: &str) {
-        let search_par = self.get_parameter(amplitude, parameter).unwrap();
+    pub fn free(&mut self, amplitude: &str, parameter: &str) -> Result<(), RustitudeError> {
+        let search_par = self.get_parameter(amplitude, parameter)?;
         let index = self.get_min_free_index();
         for par in self.parameters.iter_mut() {
             if par.fixed_index == search_par.fixed_index {
                 par.index = index;
                 par.fixed_index = None;
             }
         }
         self.reindex_parameters();
+        Ok(())
     }
-    pub fn set_bounds(&mut self, amplitude: &str, parameter: &str, bounds: (f64, f64)) {
-        let search_par = self.get_parameter(amplitude, parameter).unwrap();
+    pub fn set_bounds(
+        &mut self,
+        amplitude: &str,
+        parameter: &str,
+        bounds: (f64, f64),
+    ) -> Result<(), RustitudeError> {
+        let search_par = self.get_parameter(amplitude, parameter)?;
         if search_par.index.is_some() {
             for par in self.parameters.iter_mut() {
                 if par.index == search_par.index {
                     par.bounds = bounds;
                 }
             }
         } else {
             for par in self.parameters.iter_mut() {
                 if par.fixed_index == search_par.fixed_index {
                     par.bounds = bounds;
                 }
             }
         }
+        Ok(())
     }
-    pub fn set_initial(&mut self, amplitude: &str, parameter: &str, initial: f64) {
-        let search_par = self.get_parameter(amplitude, parameter).unwrap();
+    pub fn set_initial(
+        &mut self,
+        amplitude: &str,
+        parameter: &str,
+        initial: f64,
+    ) -> Result<(), RustitudeError> {
+        let search_par = self.get_parameter(amplitude, parameter)?;
         if search_par.index.is_some() {
             for par in self.parameters.iter_mut() {
                 if par.index == search_par.index {
                     par.initial = initial;
                 }
             }
         } else {
             for par in self.parameters.iter_mut() {
                 if par.fixed_index == search_par.fixed_index {
                     par.initial = initial;
                 }
             }
         }
+        Ok(())
     }
     pub fn get_bounds(&self) -> Vec<(f64, f64)> {
         let any_fixed = if self.any_fixed() { 1 } else { 0 };
         self.group_by_index()
             .iter()
             .skip(any_fixed)
             .filter_map(|group| group.first().map(|par| par.bounds))
@@ -812,17 +757,15 @@
     pub fn deactivate(&mut self, amplitude: &str) {
         self.amplitudes.iter_mut().for_each(|amp| {
             if amp.name == amplitude {
                 amp.active = false
             }
         })
     }
-}
-impl Model {
-    fn new(root: AmpOp) -> Self {
+    pub fn new(root: AmpOp) -> Self {
         let mut amp_names = HashSet::new();
         let amplitudes: Vec<Amplitude> = root
             .walk()
             .into_iter()
             .filter(|amp| amp_names.insert(amp.name.clone()))
             .collect();
         let parameter_tags: Vec<(String, String)> = amplitudes
@@ -841,67 +784,64 @@
             .collect();
         Self {
             root,
             amplitudes,
             parameters,
         }
     }
-    pub fn compute(&self, parameters: &[f64], event: &Event) -> f64 {
+    pub fn compute(&self, parameters: &[f64], event: &Event) -> Result<f64, RustitudeError> {
         let pars: Vec<f64> = self
             .parameters
             .iter()
             .map(|p| p.index.map_or_else(|| p.initial, |i| parameters[i]))
             .collect();
         // First, we calculate the values for the active amplitudes
         let cache: Vec<Option<Complex64>> = self
             .amplitudes
             .iter()
             .map(|amp| {
                 if amp.active {
-                    let res = amp.calculate(&pars, event).unwrap(); // unwrap panics if any
-                                                                    // errors occur in calculation
-                    Some(res)
+                    amp.calculate(&pars, event).map(Some)
                 } else {
-                    None
+                    Ok(None)
                 }
             })
-            .collect();
-        let res = self.root.compute(&cache).unwrap(); // unwrap panics if all the
-        res.re
+            .collect::<Result<Vec<Option<Complex64>>, RustitudeError>>()?;
+        Ok(self.root.compute(&cache).unwrap_or_default().re)
     }
-    pub fn load(&mut self, dataset: &Dataset) {
+    pub fn load(&mut self, dataset: &Dataset) -> Result<(), RustitudeError> {
         let mut next_cache_pos = 0;
         let mut parameter_index = 0;
-        self.amplitudes.iter_mut().for_each(|amp| {
-            amp.register(next_cache_pos, parameter_index, dataset)
-                .unwrap(); // unwrap panics if precalculate fails
+        self.amplitudes.iter_mut().try_for_each(|amp| {
+            amp.register(next_cache_pos, parameter_index, dataset)?;
             self.root.walk_mut().iter_mut().for_each(|r_amp| {
                 if r_amp.name == amp.name {
                     r_amp.cache_position = next_cache_pos;
                     r_amp.parameter_index_start = parameter_index;
                 }
             });
             next_cache_pos += 1;
             parameter_index += amp.parameters().len();
-        });
+            Ok(())
+        })
     }
     fn group_by_index(&self) -> Vec<Vec<&Parameter>> {
         self.parameters
             .iter()
             .sorted_by_key(|par| par.index)
-            .group_by(|par| par.index)
+            .chunk_by(|par| par.index)
             .into_iter()
             .map(|(_, group)| group.collect::<Vec<_>>())
             .collect()
     }
     fn group_by_index_mut(&mut self) -> Vec<Vec<&mut Parameter>> {
         self.parameters
             .iter_mut()
             .sorted_by_key(|par| par.index)
-            .group_by(|par| par.index)
+            .chunk_by(|par| par.index)
             .into_iter()
             .map(|(_, group)| group.collect())
             .collect()
     }
     fn any_fixed(&self) -> bool {
         self.parameters.iter().any(|p| p.index.is_none())
     }
@@ -937,29 +877,19 @@
 ///
 /// - `value`: The value of the scalar.
 pub struct Scalar;
 impl Node for Scalar {
     fn parameters(&self) -> Vec<String> {
         vec!["value".to_string()]
     }
-    fn calculate(&self, parameters: &[f64], _event: &Event) -> Result<Complex64, NodeError> {
+    fn calculate(&self, parameters: &[f64], _event: &Event) -> Result<Complex64, RustitudeError> {
         Ok(Complex64::new(parameters[0], 0.0))
     }
 }
 
-#[pyfunction(name = "Scalar")]
-pub fn py_scalar(name: &str) -> PyAmpOp {
-    //! Creates a named [`Scalar`].
-    //!
-    //! This is a convenience method to generate a [`PyAmpOp`] which is just a single free
-    //! parameter called `value`.
-    //!
-    //! See also: [`scalar`]
-    scalar(name).into()
-}
 pub fn scalar(name: &str) -> AmpOp {
     //! Creates a named [`Scalar`].
     //!
     //! This is a convenience method to generate an [`AmpOp`] which is just a single free
     //! parameter called `value`.
     //!
     //! # Examples
@@ -982,33 +912,23 @@
 ///
 /// # Parameters:
 ///
 /// - `real`: The real part of the complex scalar.
 /// - `imag`: The imaginary part of the complex scalar.
 pub struct ComplexScalar;
 impl Node for ComplexScalar {
-    fn calculate(&self, parameters: &[f64], _event: &Event) -> Result<Complex64, NodeError> {
+    fn calculate(&self, parameters: &[f64], _event: &Event) -> Result<Complex64, RustitudeError> {
         Ok(Complex64::new(parameters[0], parameters[1]))
     }
 
     fn parameters(&self) -> Vec<String> {
         vec!["real".to_string(), "imag".to_string()]
     }
 }
 
-#[pyfunction(name = "CScalar")]
-pub fn py_cscalar(name: &str) -> PyAmpOp {
-    //! Creates a named [`ComplexScalar`].
-    //!
-    //! This is a convenience method to generate an [`PyAmpOp`] which represents a complex
-    //! value determined by two parameters, `real` and `imag`.
-    //!
-    //! See also: [`cscalar`]
-    cscalar(name).into()
-}
 pub fn cscalar(name: &str) -> AmpOp {
     //! Creates a named [`ComplexScalar`].
     //!
     //! This is a convenience method to generate an [`AmpOp`] which represents a complex
     //! value determined by two parameters, `real` and `imag`.
     //!
     //! # Examples
@@ -1032,33 +952,23 @@
 ///
 /// # Parameters:
 ///
 /// - `mag`: The magnitude of the complex scalar.
 /// - `phi`: The phase of the complex scalar.
 pub struct PolarComplexScalar;
 impl Node for PolarComplexScalar {
-    fn calculate(&self, parameters: &[f64], _event: &Event) -> Result<Complex64, NodeError> {
+    fn calculate(&self, parameters: &[f64], _event: &Event) -> Result<Complex64, RustitudeError> {
         Ok(parameters[0] * Complex64::cis(parameters[1]))
     }
 
     fn parameters(&self) -> Vec<String> {
         vec!["mag".to_string(), "phi".to_string()]
     }
 }
 
-#[pyfunction(name = "PCScalar")]
-pub fn py_pcscalar(name: &str) -> PyAmpOp {
-    //! Creates a named [`PolarComplexScalar`].
-    //!
-    //! This is a convenience method to generate an [`PyAmpOp`] which represents a complex
-    //! value determined by two parameters, `real` and `imag`.
-    //!
-    //! See also: [`pcscalar`]
-    pcscalar(name).into()
-}
 pub fn pcscalar(name: &str) -> AmpOp {
     //! Creates a named [`PolarComplexScalar`].
     //!
     //! This is a convenience method to generate an [`AmpOp`] which represents a complex
     //! value determined by two parameters, `real` and `imag`.
     //!
     //! # Examples
@@ -1106,25 +1016,25 @@
     }
 }
 
 impl<F> Node for Piecewise<F>
 where
     F: Fn(&Event) -> f64 + Send + Sync + Copy,
 {
-    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
+    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), RustitudeError> {
         self.calculated_variable = dataset
             .events
             .read()
             .par_iter()
             .map(self.variable)
             .collect();
         Ok(())
     }
 
-    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError> {
+    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, RustitudeError> {
         let val = self.calculated_variable[event.index];
         let opt_i_bin = self.edges.iter().position(|&(l, r)| val >= l && val <= r);
         opt_i_bin.map_or_else(
             || Ok(Complex64::default()),
             |i_bin| {
                 Ok(Complex64::new(
                     parameters[i_bin * 2],
@@ -1147,24 +1057,7 @@
         name,
         Piecewise::new(bins, range, |e: &Event| {
             (e.daughter_p4s[0] + e.daughter_p4s[1]).m()
         }),
     )
     .into()
 }
-
-#[pyfunction(name = "PiecewiseM")]
-pub fn py_piecewise_m(name: &str, bins: usize, range: (f64, f64)) -> PyAmpOp {
-    piecewise_m(name, bins, range).into()
-}
-
-pub fn pyo3_module(m: &Bound<'_, PyModule>) -> PyResult<()> {
-    m.add_class::<PyAmpOp>()?;
-    m.add_class::<Parameter>()?;
-    m.add_class::<Amplitude>()?;
-    m.add_class::<Model>()?;
-    m.add_function(wrap_pyfunction!(py_scalar, m)?)?;
-    m.add_function(wrap_pyfunction!(py_cscalar, m)?)?;
-    m.add_function(wrap_pyfunction!(py_pcscalar, m)?)?;
-    m.add_function(wrap_pyfunction!(py_piecewise_m, m)?)?;
-    Ok(())
-}
```

### Comparing `rustitude-0.4.3/crates/rustitude-core/src/dataset.rs` & `rustitude-0.5.0/crates/rustitude-core/src/dataset.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,28 @@
-use std::{collections::HashMap, fmt::Display, fs::File, path::Path, sync::Arc};
+use std::{fmt::Display, fs::File, path::Path, sync::Arc};
 
 use itertools::izip;
 use nalgebra::Vector3;
 use num::Zero;
 use oxyroot::{RootFile, Slice};
 use parking_lot::RwLock;
 use parquet::{
     file::reader::{FileReader, SerializedFileReader},
     record::{Field, Row},
 };
-use pyo3::prelude::*;
 use rayon::prelude::*;
 
-use crate::prelude::FourMomentum;
+use crate::{errors::RustitudeError, prelude::FourMomentum};
 
-#[pyclass]
 #[derive(Debug, Default, Clone)]
 pub struct Event {
-    #[pyo3(get)]
     pub index: usize,
-    #[pyo3(get)]
     pub weight: f64,
-    #[pyo3(get)]
     pub beam_p4: FourMomentum,
-    #[pyo3(get)]
     pub recoil_p4: FourMomentum,
-    #[pyo3(get)]
     pub daughter_p4s: Vec<FourMomentum>,
     pub eps: Vector3<f64>,
 }
 
 impl Display for Event {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         writeln!(f, "Index: {}", self.index)?;
@@ -44,35 +37,28 @@
             f,
             "EPS: [{}, {}, {}]",
             self.eps[0], self.eps[1], self.eps[2]
         )?;
         Ok(())
     }
 }
-#[pymethods]
 impl Event {
-    pub fn __str__(&self) -> String {
-        format!("{}", self)
-    }
-    #[getter]
-    fn get_eps(&self) -> PyResult<[f64; 3]> {
-        Ok([self.eps[0], self.eps[1], self.eps[2]])
-    }
-}
-impl Event {
-    pub fn read_parquet_row(index: usize, row: Row) -> Self {
+    pub fn read_parquet_row(
+        index: usize,
+        row: Result<Row, parquet::errors::ParquetError>,
+    ) -> Result<Self, RustitudeError> {
         let mut event = Self {
             index,
             ..Default::default()
         };
         let mut e_fs: Vec<f64> = Vec::new();
         let mut px_fs: Vec<f64> = Vec::new();
         let mut py_fs: Vec<f64> = Vec::new();
         let mut pz_fs: Vec<f64> = Vec::new();
-        for (name, field) in row.get_column_iter() {
+        for (name, field) in row?.get_column_iter() {
             match (name.as_str(), field) {
                 ("E_Beam", Field::Float(value)) => {
                     event.beam_p4.set_e(f64::from(*value));
                 }
                 ("Px_Beam", Field::Float(value)) => {
                     event.beam_p4.set_px(f64::from(*value));
                 }
@@ -162,26 +148,29 @@
             .collect();
         let final_state_p4 = event.recoil_p4 + event.daughter_p4s.iter().sum();
         event.beam_p4 = event.beam_p4.boost_along(&final_state_p4);
         event.recoil_p4 = event.recoil_p4.boost_along(&final_state_p4);
         for dp4 in event.daughter_p4s.iter_mut() {
             *dp4 = dp4.boost_along(&final_state_p4);
         }
-        event
+        Ok(event)
     }
-    pub fn read_parquet_row_eps_in_beam(index: usize, row: Row) -> Self {
+    pub fn read_parquet_row_eps_in_beam(
+        index: usize,
+        row: Result<Row, parquet::errors::ParquetError>,
+    ) -> Result<Self, RustitudeError> {
         let mut event = Self {
             index,
             ..Default::default()
         };
         let mut e_fs: Vec<f64> = Vec::new();
         let mut px_fs: Vec<f64> = Vec::new();
         let mut py_fs: Vec<f64> = Vec::new();
         let mut pz_fs: Vec<f64> = Vec::new();
-        for (name, field) in row.get_column_iter() {
+        for (name, field) in row?.get_column_iter() {
             match (name.as_str(), field) {
                 ("E_Beam", Field::Float(value)) => {
                     event.beam_p4.set_e(f64::from(*value));
                 }
                 ("Px_Beam", Field::Float(value)) => {
                     event.eps[0] = f64::from(*value);
                 }
@@ -257,28 +246,32 @@
             .collect();
         let final_state_p4 = event.recoil_p4 + event.daughter_p4s.iter().sum();
         event.beam_p4 = event.beam_p4.boost_along(&final_state_p4);
         event.recoil_p4 = event.recoil_p4.boost_along(&final_state_p4);
         for dp4 in event.daughter_p4s.iter_mut() {
             *dp4 = dp4.boost_along(&final_state_p4);
         }
-        event
+        Ok(event)
     }
 
-    pub fn read_parquet_row_with_eps(index: usize, row: Row, eps: Vector3<f64>) -> Self {
+    pub fn read_parquet_row_with_eps(
+        index: usize,
+        row: Result<Row, parquet::errors::ParquetError>,
+        eps: Vector3<f64>,
+    ) -> Result<Self, RustitudeError> {
         let mut event = Self {
             index,
             eps,
             ..Default::default()
         };
         let mut e_fs: Vec<f64> = Vec::new();
         let mut px_fs: Vec<f64> = Vec::new();
         let mut py_fs: Vec<f64> = Vec::new();
         let mut pz_fs: Vec<f64> = Vec::new();
-        for (name, field) in row.get_column_iter() {
+        for (name, field) in row?.get_column_iter() {
             match (name.as_str(), field) {
                 ("E_Beam", Field::Float(value)) => {
                     event.beam_p4.set_e(f64::from(*value));
                 }
                 ("Px_Beam", Field::Float(value)) => {
                     event.beam_p4.set_px(f64::from(*value));
                 }
@@ -354,41 +347,34 @@
             .collect();
         let final_state_p4 = event.recoil_p4 + event.daughter_p4s.iter().sum();
         event.beam_p4 = event.beam_p4.boost_along(&final_state_p4);
         event.recoil_p4 = event.recoil_p4.boost_along(&final_state_p4);
         for dp4 in event.daughter_p4s.iter_mut() {
             *dp4 = dp4.boost_along(&final_state_p4);
         }
-        event
+        Ok(event)
     }
 
-    pub fn read_parquet_row_unpolarized(index: usize, row: Row) -> Self {
+    pub fn read_parquet_row_unpolarized(
+        index: usize,
+        row: Result<Row, parquet::errors::ParquetError>,
+    ) -> Result<Self, RustitudeError> {
         Self::read_parquet_row_with_eps(index, row, Vector3::default())
     }
 }
 
-#[pyclass]
 #[derive(Default, Debug, Clone)]
 pub struct Dataset {
     pub events: Arc<RwLock<Vec<Event>>>,
 }
 
-#[pymethods]
 impl Dataset {
     pub fn events(&self) -> Vec<Event> {
         self.events.read().clone()
     }
-    pub fn __len__(&self) -> PyResult<usize> {
-        Ok(self.len())
-    }
-
-    pub fn __getitem__(&self, idx: isize) -> PyResult<Py<Event>> {
-        Ok(Python::with_gil(|py| Py::new(py, self.events.read()[idx as usize].clone())).unwrap())
-    }
-
     pub fn weights(&self) -> Vec<f64> {
         self.events.read().iter().map(|e| e.weight).collect()
     }
 
     // TODO:
     // pub fn select(&mut self, query: impl Fn(&Event) -> bool + Sync + Send) -> PyDataset {}
     // pub fn reject(&mut self, query: impl Fn(&Event) -> bool + Sync + Send) -> PyDataset {}
@@ -420,224 +406,172 @@
                 .map(|i| &e.daughter_p4s[*i])
                 .sum::<FourMomentum>();
             (p1_p4 + p2_p4).m()
         };
         self.clone().split(mass, range, bins) // TODO: fix clone here eventually
     }
 
-    #[staticmethod]
-    pub fn from_events(events: Vec<Event>) -> PyResult<Self> {
-        Ok(Self {
+    pub fn from_events(events: Vec<Event>) -> Self {
+        Self {
             events: Arc::new(RwLock::new(events)),
-        })
-    }
-
-    #[staticmethod]
-    pub fn from_dict(py: Python, data: HashMap<String, PyObject>) -> PyResult<Self> {
-        let e_beam_vec: Vec<f64> = data["E_Beam"].extract(py)?;
-        let px_beam_vec: Vec<f64> = data["Px_Beam"].extract(py)?;
-        let py_beam_vec: Vec<f64> = data["Py_Beam"].extract(py)?;
-        let pz_beam_vec: Vec<f64> = data["Pz_Beam"].extract(py)?;
-        let weight_vec: Vec<f64> = data
-            .get("Weight")
-            .map_or_else(|| Ok(vec![1.0; e_beam_vec.len()]), |obj| obj.extract(py))?;
-        let eps_vec: Vec<Vector3<f64>> = data.get("EPS").map_or_else(
-            || Ok(vec![Vector3::default(); e_beam_vec.len()]),
-            |obj| {
-                obj.extract::<Vec<Vec<f64>>>(py).map(|vvf: Vec<Vec<f64>>| {
-                    vvf.into_iter()
-                        .map(Vector3::from_vec)
-                        .collect::<Vec<Vector3<f64>>>()
-                })
-            },
-        )?;
-        let e_finalstate_vec: Vec<Vec<f64>> = data["E_FinalState"].extract(py)?;
-        let px_finalstate_vec: Vec<Vec<f64>> = data["Px_FinalState"].extract(py)?;
-        let py_finalstate_vec: Vec<Vec<f64>> = data["Py_FinalState"].extract(py)?;
-        let pz_finalstate_vec: Vec<Vec<f64>> = data["Pz_FinalState"].extract(py)?;
-        Ok(Self::new(
-            (
-                e_beam_vec,
-                px_beam_vec,
-                py_beam_vec,
-                pz_beam_vec,
-                weight_vec,
-                eps_vec,
-                e_finalstate_vec,
-                px_finalstate_vec,
-                py_finalstate_vec,
-                pz_finalstate_vec,
-            )
-                .into_par_iter()
-                .enumerate()
-                .map(
-                    |(
-                        index,
-                        (
-                            e_beam,
-                            px_beam,
-                            py_beam,
-                            pz_beam,
-                            weight,
-                            eps,
-                            e_finalstate,
-                            px_finalstate,
-                            py_finalstate,
-                            pz_finalstate,
-                        ),
-                    )| {
-                        Event {
-                            index,
-                            weight,
-                            beam_p4: FourMomentum::new(e_beam, px_beam, py_beam, pz_beam),
-                            recoil_p4: FourMomentum::new(
-                                e_finalstate[0],
-                                px_finalstate[0],
-                                py_finalstate[0],
-                                pz_finalstate[0],
-                            ),
-                            daughter_p4s: e_finalstate[1..]
-                                .iter()
-                                .zip(px_finalstate[1..].iter())
-                                .zip(py_finalstate[1..].iter())
-                                .zip(pz_finalstate[1..].iter())
-                                .map(|(((e, px), py), pz)| FourMomentum::new(*e, *px, *py, *pz))
-                                .collect(),
-                            eps,
-                        }
-                    },
-                )
-                .collect(),
-        ))
+        }
     }
 
-    #[staticmethod]
-    pub fn from_parquet(path: &str) -> Self {
+    pub fn from_parquet(path: &str) -> Result<Self, RustitudeError> {
         let path = Path::new(path);
-        let file = File::open(path).unwrap();
-        let reader = SerializedFileReader::new(file).unwrap();
-        let row_iter = reader.get_row_iter(None).unwrap();
-        Self::new(
+        let file = File::open(path)?;
+        let reader = SerializedFileReader::new(file)?;
+        let row_iter = reader.get_row_iter(None)?;
+        Ok(Self::new(
             row_iter
                 .enumerate()
-                .map(|(i, row)| Event::read_parquet_row(i, row.unwrap()))
-                .collect(),
-        )
+                .map(|(i, row)| Event::read_parquet_row(i, row))
+                .collect::<Result<Vec<Event>, RustitudeError>>()?,
+        ))
     }
 
-    #[staticmethod]
-    pub fn from_parquet_eps_in_beam(path: &str) -> Self {
+    pub fn from_parquet_eps_in_beam(path: &str) -> Result<Self, RustitudeError> {
         let path = Path::new(path);
-        let file = File::open(path).unwrap();
-        let reader = SerializedFileReader::new(file).unwrap();
-        let row_iter = reader.get_row_iter(None).unwrap();
-        Self::new(
+        let file = File::open(path)?;
+        let reader = SerializedFileReader::new(file)?;
+        let row_iter = reader.get_row_iter(None)?;
+        Ok(Self::new(
             row_iter
                 .enumerate()
-                .map(|(i, row)| Event::read_parquet_row_eps_in_beam(i, row.unwrap()))
-                .collect(),
-        )
+                .map(|(i, row)| Event::read_parquet_row_eps_in_beam(i, row))
+                .collect::<Result<Vec<Event>, RustitudeError>>()?,
+        ))
     }
 
-    #[staticmethod]
-    pub fn from_parquet_with_eps(path: &str, eps: Vec<f64>) -> Self {
+    pub fn from_parquet_with_eps(path: &str, eps: Vec<f64>) -> Result<Self, RustitudeError> {
         let path = Path::new(path);
-        let file = File::open(path).unwrap();
-        let reader = SerializedFileReader::new(file).unwrap();
-        let row_iter = reader.get_row_iter(None).unwrap();
+        let file = File::open(path)?;
+        let reader = SerializedFileReader::new(file)?;
+        let row_iter = reader.get_row_iter(None)?;
         let eps_vec = Vector3::from_vec(eps);
-        Self::new(
+        Ok(Self::new(
             row_iter
                 .enumerate()
-                .map(|(i, row)| Event::read_parquet_row_with_eps(i, row.unwrap(), eps_vec))
-                .collect(),
-        )
+                .map(|(i, row)| Event::read_parquet_row_with_eps(i, row, eps_vec))
+                .collect::<Result<Vec<Event>, RustitudeError>>()?,
+        ))
     }
 
-    #[staticmethod]
-    pub fn from_parquet_unpolarized(path: &str) -> Self {
+    pub fn from_parquet_unpolarized(path: &str) -> Result<Self, RustitudeError> {
         let path = Path::new(path);
-        let file = File::open(path).unwrap();
-        let reader = SerializedFileReader::new(file).unwrap();
-        let row_iter = reader.get_row_iter(None).unwrap();
-        Self::new(
+        let file = File::open(path)?;
+        let reader = SerializedFileReader::new(file)?;
+        let row_iter = reader.get_row_iter(None)?;
+        Ok(Self::new(
             row_iter
                 .enumerate()
-                .map(|(i, row)| Event::read_parquet_row_unpolarized(i, row.unwrap()))
-                .collect(),
-        )
+                .map(|(i, row)| Event::read_parquet_row_unpolarized(i, row))
+                .collect::<Result<Vec<Event>, RustitudeError>>()?,
+        ))
     }
 
-    #[staticmethod]
-    pub fn from_root(path: &str) -> Self {
-        let ttree = RootFile::open(path).unwrap().get_tree("kin").unwrap(); // TODO:
+    pub fn from_root(path: &str) -> Result<Self, RustitudeError> {
+        let ttree = RootFile::open(path)
+            .map_err(|err| RustitudeError::OxyrootError(err.to_string()))?
+            .get_tree("kin")
+            .map_err(|err| RustitudeError::OxyrootError(err.to_string()))?;
         let weight: Vec<f64> = ttree
             .branch("Weight")
-            .unwrap()
+            .ok_or_else(|| {
+                RustitudeError::OxyrootError(format!("Could not find Weight branch in {}", path))
+            })?
             .as_iter::<f32>()
-            .unwrap()
+            .map_err(|err| RustitudeError::OxyrootError(err.to_string()))?
             .map(f64::from)
             .collect();
         let e_beam: Vec<f64> = ttree
             .branch("E_Beam")
-            .unwrap()
+            .ok_or_else(|| {
+                RustitudeError::OxyrootError(format!("Could not find E_Beam branch in {}", path))
+            })?
             .as_iter::<f32>()
-            .unwrap()
+            .map_err(|err| RustitudeError::OxyrootError(err.to_string()))?
             .map(f64::from)
             .collect();
         let px_beam: Vec<f64> = ttree
             .branch("Px_Beam")
-            .unwrap()
+            .ok_or_else(|| {
+                RustitudeError::OxyrootError(format!("Could not find Px_Beam branch in {}", path))
+            })?
             .as_iter::<f32>()
-            .unwrap()
+            .map_err(|err| RustitudeError::OxyrootError(err.to_string()))?
             .map(f64::from)
             .collect();
         let py_beam: Vec<f64> = ttree
             .branch("Py_Beam")
-            .unwrap()
+            .ok_or_else(|| {
+                RustitudeError::OxyrootError(format!("Could not find Py_Beam branch in {}", path))
+            })?
             .as_iter::<f32>()
-            .unwrap()
+            .map_err(|err| RustitudeError::OxyrootError(err.to_string()))?
             .map(f64::from)
             .collect();
         let pz_beam: Vec<f64> = ttree
             .branch("Pz_Beam")
-            .unwrap()
+            .ok_or_else(|| {
+                RustitudeError::OxyrootError(format!("Could not find Pz_Beam branch in {}", path))
+            })?
             .as_iter::<f32>()
-            .unwrap()
+            .map_err(|err| RustitudeError::OxyrootError(err.to_string()))?
             .map(f64::from)
             .collect();
         let e_fs: Vec<Vec<f64>> = ttree
             .branch("E_FinalState")
-            .unwrap()
+            .ok_or_else(|| {
+                RustitudeError::OxyrootError(format!(
+                    "Could not find E_FinalState branch in {}",
+                    path
+                ))
+            })?
             .as_iter::<Slice<f64>>()
-            .unwrap()
+            .map_err(|err| RustitudeError::OxyrootError(err.to_string()))?
             .map(|v| v.into_vec())
             .collect();
         let px_fs: Vec<Vec<f64>> = ttree
             .branch("Px_FinalState")
-            .unwrap()
+            .ok_or_else(|| {
+                RustitudeError::OxyrootError(format!(
+                    "Could not find Px_FinalState branch in {}",
+                    path
+                ))
+            })?
             .as_iter::<Slice<f64>>()
-            .unwrap()
+            .map_err(|err| RustitudeError::OxyrootError(err.to_string()))?
             .map(|v| v.into_vec())
             .collect();
         let py_fs: Vec<Vec<f64>> = ttree
             .branch("Py_FinalState")
-            .unwrap()
+            .ok_or_else(|| {
+                RustitudeError::OxyrootError(format!(
+                    "Could not find Px_FinalState branch in {}",
+                    path
+                ))
+            })?
             .as_iter::<Slice<f64>>()
-            .unwrap()
+            .map_err(|err| RustitudeError::OxyrootError(err.to_string()))?
             .map(|v| v.into_vec())
             .collect();
         let pz_fs: Vec<Vec<f64>> = ttree
             .branch("Pz_FinalState")
-            .unwrap()
+            .ok_or_else(|| {
+                RustitudeError::OxyrootError(format!(
+                    "Could not find Px_FinalState branch in {}",
+                    path
+                ))
+            })?
             .as_iter::<Slice<f64>>()
-            .unwrap()
+            .map_err(|err| RustitudeError::OxyrootError(err.to_string()))?
             .map(|v| v.into_vec())
             .collect();
-        Self::new(
+        Ok(Self::new(
             izip!(weight, e_beam, px_beam, py_beam, pz_beam, e_fs, px_fs, py_fs, pz_fs)
                 .enumerate()
                 .map(
                     |(i, (w, e_b, px_b, py_b, pz_b, e_f, px_f, py_f, pz_f))| Event {
                         index: i,
                         weight: w,
                         beam_p4: FourMomentum::new(e_b, px_b, py_b, pz_b),
@@ -650,19 +584,16 @@
                         )
                         .map(|(e, px, py, pz)| FourMomentum::new(*e, *px, *py, *pz))
                         .collect(),
                         eps: Vector3::zero(),
                     },
                 )
                 .collect(),
-        )
+        ))
     }
-}
-
-impl Dataset {
     pub fn new(events: Vec<Event>) -> Self {
         Self {
             events: Arc::new(RwLock::new(events)),
         }
     }
 
     pub fn is_empty(&self) -> bool {
@@ -710,13 +641,7 @@
         bins.into_iter().skip(1).for_each(|ub| {
             let bin_contents = self.reject(|event| variable(event) < ub);
             out.push(bin_contents);
         });
         (out, underflow, overflow)
     }
 }
-
-pub fn pyo3_module(m: &Bound<'_, PyModule>) -> PyResult<()> {
-    m.add_class::<Event>()?;
-    m.add_class::<Dataset>()?;
-    Ok(())
-}
```

### Comparing `rustitude-0.4.3/crates/rustitude-core/src/docs-header.html` & `rustitude-0.5.0/crates/rustitude-core/src/docs-header.html`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.3/crates/rustitude-core/src/four_momentum.rs` & `rustitude-0.5.0/crates/rustitude-core/src/four_momentum.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 use nalgebra::{Matrix4, Vector3, Vector4};
-use pyo3::prelude::*;
 use std::{
     fmt::Display,
     ops::{Add, Sub},
 };
 
 #[cfg(feature = "simd")]
 use std::simd::prelude::*;
 
 #[cfg(not(feature = "simd"))]
-#[pyclass]
 #[derive(Debug, Clone, PartialEq, Copy, Default)]
 pub struct FourMomentum([f64; 4]);
 
 #[cfg(feature = "simd")]
-#[pyclass]
 #[derive(Debug, Clone, PartialEq, Copy, Default)]
 pub struct FourMomentum(f64x4);
 
 impl Eq for FourMomentum {}
 
 impl Display for FourMomentum {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
@@ -29,15 +26,14 @@
             self.px(),
             self.py(),
             self.pz(),
         )
     }
 }
 
-#[pymethods]
 impl FourMomentum {
     //! A four-momentum structure with helpful methods for boosts.
     //!
     //! This is the basic structure of a Lorentz four-vector
     //! of the form $`(E, \overrightarrow{p})`$ where $`E`$ is the energy and $`\overrightarrow{p}`$ is the
     //! momentum.
     //!
@@ -46,39 +42,29 @@
     //! use rustitude_core::prelude::*;
     //!
     //! let vec_a = FourMomentum::new(1.3, 0.2, 0.3, 0.1);
     //! let vec_b = FourMomentum::new(4.2, 0.5, 0.4, 0.5);
     //! ```
 
     #[cfg(not(feature = "simd"))]
-    #[new]
     pub const fn new(e: f64, px: f64, py: f64, pz: f64) -> Self {
         //! Create a new [`FourMomentum`] from energy and momentum components.
         //!
         //! Components are listed in the order $` (E, p_x, p_y, p_z) `$
         Self([e, px, py, pz])
     }
 
     #[cfg(feature = "simd")]
-    #[new]
     pub fn new(e: f64, px: f64, py: f64, pz: f64) -> Self {
         //! Create a new [`FourMomentum`] from energy and momentum components.
         //!
         //! Components are listed in the order $` (E, p_x, p_y, p_z) `$
         Self([e, px, py, pz].into())
     }
 
-    fn __repr__(&self) -> String {
-        format!("<FourMomentum ({})>", self)
-    }
-
-    fn __str__(&self) -> String {
-        self.to_string()
-    }
-
     #[allow(clippy::missing_const_for_fn)]
     pub fn e(&self) -> f64 {
         self.0[0]
     }
     #[allow(clippy::missing_const_for_fn)]
     pub fn px(&self) -> f64 {
         self.0[1]
@@ -152,17 +138,14 @@
         //! assert_abs_diff_eq!(vec_a_COM.px(), 0.0, epsilon = 1e-15);
         //! assert_abs_diff_eq!(vec_a_COM.py(), 0.0, epsilon = 1e-15);
         //! assert_abs_diff_eq!(vec_a_COM.pz(), 0.0, epsilon = 1e-15);
         //! ```
         let m_boost = other.boost_matrix();
         (m_boost * Vector4::<f64>::from(self)).into()
     }
-}
-
-impl FourMomentum {
     pub fn momentum(&self) -> Vector3<f64> {
         //! Extract the 3-momentum as a [`nalgebra::Vector3<f64>`]
         //!
         //! # Examples
         //! ```
         //! use rustitude_core::prelude::*;
         //! use nalgebra::Vector3;
@@ -349,12 +332,7 @@
 }
 
 impl<'a> std::iter::Sum<&'a Self> for FourMomentum {
     fn sum<I: Iterator<Item = &'a Self>>(iter: I) -> Self {
         iter.fold(Self::default(), |a, b| a + *b)
     }
 }
-
-pub fn pyo3_module(m: &Bound<'_, PyModule>) -> PyResult<()> {
-    m.add_class::<FourMomentum>()?;
-    Ok(())
-}
```

### Comparing `rustitude-0.4.3/crates/rustitude-gluex/CHANGELOG.md` & `rustitude-0.5.0/crates/rustitude-gluex/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,51 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## v0.3.0 (2024-05-24)
+
+### Bug Fixes
+
+ - <csr-id-405ed0cb2ad417ccf0041a49ce6fbd6b6693539c/> bump versions
+
+### Documentation
+
+ - <csr-id-45107c4c719503310ac171186b016212bf4d5370/> Update README.md
+
+### New Features
+
+ - <csr-id-6955773a3e96890efa4573d5c7bc355bb23a07e6/> add RustitudeError and remove unwraps, error handling should work in python as well
+
+### Commit Statistics
+
+<csr-read-only-do-not-edit/>
+
+ - 5 commits contributed to the release.
+ - 8 days passed between releases.
+ - 3 commits were understood as [conventional](https://www.conventionalcommits.org).
+ - 0 issues like '(#ID)' were seen in commit messages
+
+### Commit Details
+
+<csr-read-only-do-not-edit/>
+
+<details><summary>view details</summary>
+
+ * **Uncategorized**
+    - Bump versions ([`405ed0c`](https://github.com/denehoffman/rustitude/commit/405ed0cb2ad417ccf0041a49ce6fbd6b6693539c))
+    - Update README.md ([`45107c4`](https://github.com/denehoffman/rustitude/commit/45107c4c719503310ac171186b016212bf4d5370))
+    - Merge pull request #3 from denehoffman/python_reorg ([`467caac`](https://github.com/denehoffman/rustitude/commit/467caacc688f94c074d28be1ec54a422d8d9ebc0))
+    - Add RustitudeError and remove unwraps, error handling should work in python as well ([`6955773`](https://github.com/denehoffman/rustitude/commit/6955773a3e96890efa4573d5c7bc355bb23a07e6))
+    - Move all pyo3 code to the py-rustitude crate ([`9bcdb46`](https://github.com/denehoffman/rustitude/commit/9bcdb4615fdb4df5b4566673fbed955930926b7c))
+</details>
+
 ## v0.2.2 (2024-05-16)
 
 <csr-id-0e94ec45850cb6129924b2be27793a17c51b03c2/>
 
 ### Bug Fixes
 
  - <csr-id-77054e334d90077decd54d4f970400efa1a31f47/> update amplitudes to account for changes in core
@@ -17,25 +54,26 @@
 
  - <csr-id-0e94ec45850cb6129924b2be27793a17c51b03c2/> get rid of extra git-files and media
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
 
- - 3 commits contributed to the release.
+ - 4 commits contributed to the release.
  - 2 commits were understood as [conventional](https://www.conventionalcommits.org).
  - 0 issues like '(#ID)' were seen in commit messages
 
 ### Commit Details
 
 <csr-read-only-do-not-edit/>
 
 <details><summary>view details</summary>
 
  * **Uncategorized**
+    - Release rustitude-core v1.0.1, rustitude-gluex v0.2.2, rustitude v0.4.3 ([`fe0c603`](https://github.com/denehoffman/rustitude/commit/fe0c6036d4816587b1d65ae2697f3b241cfe579c))
     - Release rustitude-gluex v0.2.2, rustitude v0.4.3 ([`0062542`](https://github.com/denehoffman/rustitude/commit/006254211c6dda1924cede7818c94ab4dcf1f49a))
     - Get rid of extra git-files and media ([`0e94ec4`](https://github.com/denehoffman/rustitude/commit/0e94ec45850cb6129924b2be27793a17c51b03c2))
     - Update amplitudes to account for changes in core ([`77054e3`](https://github.com/denehoffman/rustitude/commit/77054e334d90077decd54d4f970400efa1a31f47))
 </details>
 
 ## v0.2.1 (2024-05-15)
```

### Comparing `rustitude-0.4.3/crates/rustitude-gluex/README.md` & `rustitude-0.5.0/crates/rustitude-gluex/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 | [LowerVertexDelta.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/LowerVertexDelta.cc)             |                                                                                                     |           :x:            |
 | [OmegaDalitz.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/OmegaDalitz.cc)                       | `rustitude-gluex::dalitz::OmegaDalitz`                                                              |    :white_check_mark:    |
 | [PhaseOffset.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/PhaseOffset.cc)                       |                                                                                                     |        :bangbang:        |
 | [Pi0Regge.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/Pi0Regge.cc)                             |                                                                                                     | :heavy_exclamation_mark: |
 | [Pi0ReggeModel.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/Pi0ReggeModel.cc)                   |                                                                                                     |           :x:            |
 | [Pi0SAID.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/Pi0SAID.cc)                               |                                                                                                     |           :x:            |
 | [PiPlusRegge.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/PiPlusRegge.cc)                       |                                                                                                     |           :x:            |
-| [Piecewise.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/Piecewise.cc)                           | `rustitude::amplitude::Piecewise`                                                                   |    :white_check_mark:    |
+| [Piecewise.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/Piecewise.cc)                           | `rustitude::amplitude::PiecewiseM`                                                                   |    :white_check_mark:    |
 | [SinglePS.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/SinglePS.cc)                             | `rustitude-gluex::harmonics::OnePS`                                                                 |    :white_check_mark:    |
 | [ThreePiAngles.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/ThreePiAngles.cc)                   |                                                                                                     |        :bangbang:        |
 | [ThreePiAnglesSchilling.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/ThreePiAnglesSchilling.cc) | `rustitude-gluex::sdmes::ThreePiSDME`                                                               |    :white_check_mark:    |
 | [TwoLeptonAngles.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/TwoLeptonAngles.cc)               |                                                                                                     | :heavy_exclamation_mark: |
 | [TwoLeptonAnglesGJ.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/TwoLeptonAnglesGJ.cc)           |                                                                                                     | :heavy_exclamation_mark: |
 | [TwoPSAngles.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/TwoPSAngles.cc)                       | `rustitude-gluex::harmonics::TwoPS`                                                                 |    :white_check_mark:    |
 | [TwoPSHelicity.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/TwoPSHelicity.cc)                   | `rustitude-gluex::harmonics::TwoPS`                                                                 |    :white_check_mark:    |
```

#### html2text {}

```diff
@@ -68,15 +68,15 @@
 master/src/libraries/AMPTOOLS_AMPS/Pi0Regge.cc) | | :heavy_exclamation_mark: |
 | [Pi0ReggeModel.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/
 libraries/AMPTOOLS_AMPS/Pi0ReggeModel.cc) | | :x: | | [Pi0SAID.cc](https://
 github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/
 Pi0SAID.cc) | | :x: | | [PiPlusRegge.cc](https://github.com/JeffersonLab/
 halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/PiPlusRegge.cc) | | :x: | |
 [Piecewise.cc](https://github.com/JeffersonLab/halld_sim/blob/master/src/
-libraries/AMPTOOLS_AMPS/Piecewise.cc) | `rustitude::amplitude::Piecewise` | :
+libraries/AMPTOOLS_AMPS/Piecewise.cc) | `rustitude::amplitude::PiecewiseM` | :
 white_check_mark: | | [SinglePS.cc](https://github.com/JeffersonLab/halld_sim/
 blob/master/src/libraries/AMPTOOLS_AMPS/SinglePS.cc) | `rustitude-gluex::
 harmonics::OnePS` | :white_check_mark: | | [ThreePiAngles.cc](https://
 github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/
 ThreePiAngles.cc) | | :bangbang: | | [ThreePiAnglesSchilling.cc](https://
 github.com/JeffersonLab/halld_sim/blob/master/src/libraries/AMPTOOLS_AMPS/
 ThreePiAnglesSchilling.cc) | `rustitude-gluex::sdmes::ThreePiSDME` | :
```

### Comparing `rustitude-0.4.3/crates/rustitude-gluex/media/logo.png` & `rustitude-0.5.0/crates/rustitude-gluex/media/logo.png`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.3/crates/rustitude-gluex/src/dalitz.rs` & `rustitude-0.5.0/crates/rustitude-gluex/src/dalitz.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-use pyo3::prelude::*;
 use rayon::prelude::*;
 use rustitude_core::prelude::*;
 
 #[derive(Default)]
 pub struct OmegaDalitz {
     dalitz_z: Vec<f64>,
     dalitz_sin3theta: Vec<f64>,
     lambda: Vec<f64>,
 }
 
 impl Node for OmegaDalitz {
-    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
+    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), RustitudeError> {
         (self.dalitz_z, (self.dalitz_sin3theta, self.lambda)) = dataset
             .events
             .read()
             .par_iter()
             .map(|event| {
                 let pi0 = event.daughter_p4s[0];
                 let pip = event.daughter_p4s[1];
@@ -43,15 +42,15 @@
 
                 (dalitz_z, (dalitz_sin3theta, lambda))
             })
             .unzip();
         Ok(())
     }
 
-    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError> {
+    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, RustitudeError> {
         let dalitz_z = self.dalitz_z[event.index];
         let dalitz_sin3theta = self.dalitz_sin3theta[event.index];
         let lambda = self.lambda[event.index];
         let alpha = parameters[0];
         let beta = parameters[1];
         let gamma = parameters[2];
         let delta = parameters[3];
@@ -71,17 +70,7 @@
             "alpha".to_string(),
             "beta".to_string(),
             "gamma".to_string(),
             "delta".to_string(),
         ]
     }
 }
-
-#[pyfunction(name = "OmegaDalitz")]
-fn omega_dalitz(name: &str) -> PyAmpOp {
-    Amplitude::new(name, OmegaDalitz::default()).into()
-}
-
-pub fn pyo3_module(m: &Bound<'_, PyModule>) -> PyResult<()> {
-    m.add_function(wrap_pyfunction!(omega_dalitz, m)?)?;
-    Ok(())
-}
```

### Comparing `rustitude-0.4.3/crates/rustitude-gluex/src/resonances.rs` & `rustitude-0.5.0/crates/rustitude-gluex/src/resonances.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 use crate::utils::blatt_weisskopf;
 use crate::utils::breakup_momentum;
-use pyo3::prelude::*;
 use std::f64::consts::PI;
 
 use nalgebra::{SMatrix, SVector};
 use rayon::prelude::*;
 use rustitude_core::prelude::*;
 
 #[derive(Default)]
@@ -25,15 +24,15 @@
             p2_indices: p2_indices.into(),
             l,
             ..Default::default()
         }
     }
 }
 impl Node for BreitWigner {
-    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
+    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), RustitudeError> {
         (self.m, (self.m1, (self.m2, (self.q, self.f)))) = dataset
             .events
             .read()
             .par_iter()
             .map(|event| {
                 let p1: FourMomentum = self
                     .p1_indices
@@ -52,15 +51,15 @@
                 let f = blatt_weisskopf(m, m1, m2, self.l);
                 (m, (m1, (m2, (q, f))))
             })
             .unzip();
         Ok(())
     }
 
-    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError> {
+    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, RustitudeError> {
         let m = self.m[event.index];
         let m1 = self.m1[event.index];
         let m2 = self.m2[event.index];
         let q = self.q[event.index];
         let f = self.f[event.index];
         let m0 = parameters[0];
         let g0 = parameters[1];
@@ -200,15 +199,15 @@
                 l: 0,
             },
             Vec::default())
     }
 }
 
 impl Node for KMatrixF0 {
-    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
+    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), RustitudeError> {
         self.2 = dataset
             .events
             .read()
             .par_iter()
             .map(|event| {
                 let s = (event.daughter_p4s[0] + event.daughter_p4s[1]).m2();
                 let barrier_mat = self.1.barrier_matrix(s);
@@ -217,15 +216,15 @@
                         / (self.1.mrs[a].powi(2) - s)
                 });
                 (self.1.ikc_inv(s, self.0), pvector_constants)
             })
             .collect();
         Ok(())
     }
-    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError> {
+    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, RustitudeError> {
         let betas = SVector::<Complex64, 5>::new(
             Complex64::new(parameters[0], parameters[1]),
             Complex64::new(parameters[2], parameters[3]),
             Complex64::new(parameters[4], parameters[5]),
             Complex64::new(parameters[6], parameters[7]),
             Complex64::new(parameters[8], parameters[9]),
         );
@@ -280,15 +279,15 @@
                 l: 2,
             },
             Vec::default())
     }
 }
 
 impl Node for KMatrixF2 {
-    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
+    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), RustitudeError> {
         self.2 = dataset
             .events
             .read()
             .par_iter()
             .map(|event| {
                 let s = (event.daughter_p4s[0] + event.daughter_p4s[1]).m2();
                 let barrier_mat = self.1.barrier_matrix(s);
@@ -297,15 +296,15 @@
                         / (self.1.mrs[a].powi(2) - s)
                 });
                 (self.1.ikc_inv(s, self.0), pvector_constants)
             })
             .collect();
         Ok(())
     }
-    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError> {
+    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, RustitudeError> {
         let betas = SVector::<Complex64, 4>::new(
             Complex64::new(parameters[0], parameters[1]),
             Complex64::new(parameters[2], parameters[3]),
             Complex64::new(parameters[4], parameters[5]),
             Complex64::new(parameters[6], parameters[7]),
         );
         let (ikc_inv_vec, pvector_constants_mat) = self.2[event.index];
@@ -354,15 +353,15 @@
                 l: 0,
             },
             Vec::default())
     }
 }
 
 impl Node for KMatrixA0 {
-    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
+    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), RustitudeError> {
         self.2 = dataset
             .events
             .read()
             .par_iter()
             .map(|event| {
                 let s = (event.daughter_p4s[0] + event.daughter_p4s[1]).m2();
                 let barrier_mat = self.1.barrier_matrix(s);
@@ -371,15 +370,15 @@
                         / (self.1.mrs[a].powi(2) - s)
                 });
                 (self.1.ikc_inv(s, self.0), pvector_constants)
             })
             .collect();
         Ok(())
     }
-    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError> {
+    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, RustitudeError> {
         let betas = SVector::<Complex64, 2>::new(
             Complex64::new(parameters[0], parameters[1]),
             Complex64::new(parameters[2], parameters[3]),
         );
         let (ikc_inv_vec, pvector_constants_mat) = self.2[event.index];
         Ok(KMatrixConstants::calculate_k_matrix(
             &betas,
@@ -424,15 +423,15 @@
                 l: 2,
             },
             Vec::default())
     }
 }
 
 impl Node for KMatrixA2 {
-    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
+    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), RustitudeError> {
         self.2 = dataset
             .events
             .read()
             .par_iter()
             .map(|event| {
                 let s = (event.daughter_p4s[0] + event.daughter_p4s[1]).m2();
                 let barrier_mat = self.1.barrier_matrix(s);
@@ -441,15 +440,15 @@
                         / (self.1.mrs[a].powi(2) - s)
                 });
                 (self.1.ikc_inv(s, self.0), pvector_constants)
             })
             .collect();
         Ok(())
     }
-    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError> {
+    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, RustitudeError> {
         let betas = SVector::<Complex64, 2>::new(
             Complex64::new(parameters[0], parameters[1]),
             Complex64::new(parameters[2], parameters[3]),
         );
         let (ikc_inv_vec, pvector_constants_mat) = self.2[event.index];
         Ok(KMatrixConstants::calculate_k_matrix(
             &betas,
@@ -494,15 +493,15 @@
                 l: 1,
             },
             Vec::default())
     }
 }
 
 impl Node for KMatrixRho {
-    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
+    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), RustitudeError> {
         self.2 = dataset
             .events
             .read()
             .par_iter()
             .map(|event| {
                 let s = (event.daughter_p4s[0] + event.daughter_p4s[1]).m2();
                 let barrier_mat = self.1.barrier_matrix(s);
@@ -511,15 +510,15 @@
                         / (self.1.mrs[a].powi(2) - s)
                 });
                 (self.1.ikc_inv(s, self.0), pvector_constants)
             })
             .collect();
         Ok(())
     }
-    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError> {
+    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, RustitudeError> {
         let betas = SVector::<Complex64, 2>::new(
             Complex64::new(parameters[0], parameters[1]),
             Complex64::new(parameters[2], parameters[3]),
         );
         let (ikc_inv_vec, pvector_constants_mat) = self.2[event.index];
         Ok(KMatrixConstants::calculate_k_matrix(
             &betas,
@@ -562,15 +561,15 @@
                 l: 1,
             },
             Vec::default())
     }
 }
 
 impl Node for KMatrixPi1 {
-    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
+    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), RustitudeError> {
         self.2 = dataset
             .events
             .read()
             .par_iter()
             .map(|event| {
                 let s = (event.daughter_p4s[0] + event.daughter_p4s[1]).m2();
                 let barrier_mat = self.1.barrier_matrix(s);
@@ -579,60 +578,20 @@
                         / (self.1.mrs[a].powi(2) - s)
                 });
                 (self.1.ikc_inv(s, self.0), pvector_constants)
             })
             .collect();
         Ok(())
     }
-    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError> {
+    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, RustitudeError> {
         let betas = SVector::<Complex64, 1>::new(Complex64::new(parameters[0], parameters[1]));
         let (ikc_inv_vec, pvector_constants_mat) = self.2[event.index];
         Ok(KMatrixConstants::calculate_k_matrix(
             &betas,
             &ikc_inv_vec,
             &pvector_constants_mat,
         ))
     }
     fn parameters(&self) -> Vec<String> {
         vec!["pi1_1600 re".to_string(), "pi1_1600 im".to_string()]
     }
 }
-
-#[pyfunction(name = "BreitWigner")]
-fn breit_wigner(name: &str, p1_indices: Vec<usize>, p2_indices: Vec<usize>, l: usize) -> PyAmpOp {
-    Amplitude::new(name, BreitWigner::new(&p1_indices, &p2_indices, l)).into()
-}
-#[pyfunction(name = "KMatrixA0")]
-fn kmatrix_a0(name: &str, channel: usize) -> PyAmpOp {
-    Amplitude::new(name, KMatrixA0::new(channel)).into()
-}
-#[pyfunction(name = "KMatrixA2")]
-fn kmatrix_a2(name: &str, channel: usize) -> PyAmpOp {
-    Amplitude::new(name, KMatrixA2::new(channel)).into()
-}
-#[pyfunction(name = "KMatrixF0")]
-fn kmatrix_f0(name: &str, channel: usize) -> PyAmpOp {
-    Amplitude::new(name, KMatrixF0::new(channel)).into()
-}
-#[pyfunction(name = "KMatrixF2")]
-fn kmatrix_f2(name: &str, channel: usize) -> PyAmpOp {
-    Amplitude::new(name, KMatrixF2::new(channel)).into()
-}
-#[pyfunction(name = "KMatrixPi1")]
-fn kmatrix_pi1(name: &str, channel: usize) -> PyAmpOp {
-    Amplitude::new(name, KMatrixPi1::new(channel)).into()
-}
-#[pyfunction(name = "KMatrixRho")]
-fn kmatrix_rho(name: &str, channel: usize) -> PyAmpOp {
-    Amplitude::new(name, KMatrixRho::new(channel)).into()
-}
-
-pub fn pyo3_module(m: &Bound<'_, PyModule>) -> PyResult<()> {
-    m.add_function(wrap_pyfunction!(breit_wigner, m)?)?;
-    m.add_function(wrap_pyfunction!(kmatrix_a0, m)?)?;
-    m.add_function(wrap_pyfunction!(kmatrix_a2, m)?)?;
-    m.add_function(wrap_pyfunction!(kmatrix_f0, m)?)?;
-    m.add_function(wrap_pyfunction!(kmatrix_f2, m)?)?;
-    m.add_function(wrap_pyfunction!(kmatrix_pi1, m)?)?;
-    m.add_function(wrap_pyfunction!(kmatrix_rho, m)?)?;
-    Ok(())
-}
```

### Comparing `rustitude-0.4.3/crates/rustitude-gluex/src/sdmes.rs` & `rustitude-0.5.0/crates/rustitude-gluex/src/sdmes.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-use pyo3::prelude::*;
 use rayon::prelude::*;
 use rustitude_core::prelude::*;
 use sphrs::SHCoordinates;
 use std::f64::consts::PI;
 
 use crate::utils::Frame;
 
@@ -17,15 +16,15 @@
             frame,
             data: Vec::default(),
         }
     }
 }
 
 impl Node for TwoPiSDME {
-    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
+    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), RustitudeError> {
         self.data = dataset
             .events
             .read()
             .par_iter()
             .map(|event| {
                 let resonance = event.daughter_p4s[0] + event.daughter_p4s[1];
                 let daughter_res_vec = event.daughter_p4s[0].boost_along(&resonance).momentum();
@@ -47,15 +46,15 @@
                     pgamma,
                 )
             })
             .collect();
         Ok(())
     }
 
-    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError> {
+    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, RustitudeError> {
         let (costheta, sinsqtheta, sin2theta, phi, big_phi, pgamma) = self.data[event.index];
         let pol_angle = event.eps[0].acos();
         let r_big_phi = pol_angle * 0.017453293 + big_phi;
         let rho_000 = parameters[0];
         let rho_100 = parameters[1];
         let rho_1n10 = parameters[2];
         let rho_111 = parameters[3];
@@ -109,15 +108,15 @@
             frame,
             data: Vec::default(),
         }
     }
 }
 
 impl Node for ThreePiSDME {
-    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
+    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), RustitudeError> {
         self.data = dataset
             .events
             .read()
             .par_iter()
             .map(|event| {
                 let resonance =
                     event.daughter_p4s[0] + event.daughter_p4s[1] + event.daughter_p4s[2];
@@ -142,15 +141,15 @@
                     pgamma,
                 )
             })
             .collect();
         Ok(())
     }
 
-    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError> {
+    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, RustitudeError> {
         let (costheta, sinsqtheta, sin2theta, phi, big_phi, pgamma) = self.data[event.index];
         let pol_angle = event.eps[0].acos();
         let r_big_phi = pol_angle * 0.017453293 + big_phi;
         let rho_000 = parameters[0];
         let rho_100 = parameters[1];
         let rho_1n10 = parameters[2];
         let rho_111 = parameters[3];
@@ -188,32 +187,7 @@
             "rho_101".to_string(),
             "rho_1n11".to_string(),
             "rho_102".to_string(),
             "rho_1n12".to_string(),
         ]
     }
 }
-
-#[pyfunction]
-#[pyo3(name = "TwoPiSDME", signature = (name, frame="helicity"))]
-fn two_pi_sdme(name: &str, frame: &str) -> PyAmpOp {
-    Amplitude::new(
-        name,
-        TwoPiSDME::new(<Frame as std::str::FromStr>::from_str(frame).unwrap()),
-    )
-    .into()
-}
-#[pyfunction]
-#[pyo3(name = "ThreePiSDME", signature = (name, frame="helicity"))]
-fn three_pi_sdme(name: &str, frame: &str) -> PyAmpOp {
-    Amplitude::new(
-        name,
-        ThreePiSDME::new(<Frame as std::str::FromStr>::from_str(frame).unwrap()),
-    )
-    .into()
-}
-
-pub fn pyo3_module(m: &Bound<'_, PyModule>) -> PyResult<()> {
-    m.add_function(wrap_pyfunction!(two_pi_sdme, m)?)?;
-    m.add_function(wrap_pyfunction!(three_pi_sdme, m)?)?;
-    Ok(())
-}
```

### Comparing `rustitude-0.4.3/crates/rustitude-gluex/src/utils.rs` & `rustitude-0.5.0/crates/rustitude-gluex/src/utils.rs`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.3/crates/rustitude/CHANGELOG.md` & `rustitude-0.5.0/py-rustitude/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,78 +1,66 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## 0.4.3 (2024-05-16)
+## 0.4.3 (2024-05-24)
 
-<csr-id-e4399efe07ea8e66d9769a067c55c72d9dc09c69/>
-<csr-id-0e94ec45850cb6129924b2be27793a17c51b03c2/>
-
-### Refactor
-
- - <csr-id-e4399efe07ea8e66d9769a067c55c72d9dc09c69/> this is no longer a python crate
-
-### Style
-
- - <csr-id-0e94ec45850cb6129924b2be27793a17c51b03c2/> get rid of extra git-files and media
-
-### Commit Statistics
-
-<csr-read-only-do-not-edit/>
-
- - 3 commits contributed to the release.
- - 2 commits were understood as [conventional](https://www.conventionalcommits.org).
- - 0 issues like '(#ID)' were seen in commit messages
+<csr-id-800db450c6743d409c44b1dff74263288d63d8c1/>
+<csr-id-9d854af5046ac30aacc6c369716337a863b4279a/>
+<csr-id-9089c84e481124ff764b24f42507ab14913fef07/>
 
-### Commit Details
+### Chore
 
-<csr-read-only-do-not-edit/>
+ - <csr-id-800db450c6743d409c44b1dff74263288d63d8c1/> bump python library version
+ - <csr-id-9d854af5046ac30aacc6c369716337a863b4279a/> bump python library version
 
-<details><summary>view details</summary>
+### New Features
 
- * **Uncategorized**
-    - Release rustitude-gluex v0.2.2, rustitude v0.4.3 ([`0062542`](https://github.com/denehoffman/rustitude/commit/006254211c6dda1924cede7818c94ab4dcf1f49a))
-    - Get rid of extra git-files and media ([`0e94ec4`](https://github.com/denehoffman/rustitude/commit/0e94ec45850cb6129924b2be27793a17c51b03c2))
-    - This is no longer a python crate ([`e4399ef`](https://github.com/denehoffman/rustitude/commit/e4399efe07ea8e66d9769a067c55c72d9dc09c69))
-</details>
+ - <csr-id-d2a94a57466c0b2556850315b8902cf9528598de/> additional API so python interactions with managers can actually modify the amplitudes they manage
+ - <csr-id-6955773a3e96890efa4573d5c7bc355bb23a07e6/> add RustitudeError and remove unwraps, error handling should work in python as well
 
-## 0.4.2 (2024-05-15)
+### Bug Fixes
 
-<csr-id-9089c84e481124ff764b24f42507ab14913fef07/>
+ - <csr-id-dba3b5bbd9b93622c32e6042062d75da972c073e/> remove unsafe transmutes, they weren't working properly and probably aren't needed anyway
+ - <csr-id-b6c8e24db3376ebabbe3fc113712dc0f33072caa/> fix py-rustitude dependencies
+ - <csr-id-174a6f540fa8f2b0292a9657e87acbe65edcaf71/> readmes and licenses suck
 
 ### Refactor
 
  - <csr-id-9089c84e481124ff764b24f42507ab14913fef07/> major move required to have rustitude function properly as a Rust crate. I set this up very wrong the first time
 
-### Bug Fixes
-
- - <csr-id-174a6f540fa8f2b0292a9657e87acbe65edcaf71/> readmes and licenses suck
-
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
 
- - 5 commits contributed to the release.
- - 2 commits were understood as [conventional](https://www.conventionalcommits.org).
+ - 12 commits contributed to the release over the course of 8 calendar days.
+ - 8 commits were understood as [conventional](https://www.conventionalcommits.org).
  - 0 issues like '(#ID)' were seen in commit messages
 
 ### Commit Details
 
 <csr-read-only-do-not-edit/>
 
 <details><summary>view details</summary>
 
  * **Uncategorized**
-    - Release rustitude v0.4.2 ([`6fde79a`](https://github.com/denehoffman/rustitude/commit/6fde79a5b11d20069c36d47a272aee9bed9fd3a9))
-    - Release rustitude v0.4.2 ([`f0d5b95`](https://github.com/denehoffman/rustitude/commit/f0d5b954f659e5410fc504b460e980a1fb270936))
+    - Release py-rustitude v0.4.3 ([`85fa50e`](https://github.com/denehoffman/rustitude/commit/85fa50ee82bc94d288c2ae145cb9bc8d1ca073d2))
+    - Release py-rustitude v0.4.3 ([`573e76a`](https://github.com/denehoffman/rustitude/commit/573e76ae26b8008046cc6c4221c20bc476e18f88))
+    - Merge pull request #3 from denehoffman/python_reorg ([`467caac`](https://github.com/denehoffman/rustitude/commit/467caacc688f94c074d28be1ec54a422d8d9ebc0))
+    - Additional API so python interactions with managers can actually modify the amplitudes they manage ([`d2a94a5`](https://github.com/denehoffman/rustitude/commit/d2a94a57466c0b2556850315b8902cf9528598de))
+    - Remove unsafe transmutes, they weren't working properly and probably aren't needed anyway ([`dba3b5b`](https://github.com/denehoffman/rustitude/commit/dba3b5bbd9b93622c32e6042062d75da972c073e))
+    - Add RustitudeError and remove unwraps, error handling should work in python as well ([`6955773`](https://github.com/denehoffman/rustitude/commit/6955773a3e96890efa4573d5c7bc355bb23a07e6))
+    - Move all pyo3 code to the py-rustitude crate ([`9bcdb46`](https://github.com/denehoffman/rustitude/commit/9bcdb4615fdb4df5b4566673fbed955930926b7c))
+    - Bump python library version ([`800db45`](https://github.com/denehoffman/rustitude/commit/800db450c6743d409c44b1dff74263288d63d8c1))
+    - Fix py-rustitude dependencies ([`b6c8e24`](https://github.com/denehoffman/rustitude/commit/b6c8e24db3376ebabbe3fc113712dc0f33072caa))
     - Readmes and licenses suck ([`174a6f5`](https://github.com/denehoffman/rustitude/commit/174a6f540fa8f2b0292a9657e87acbe65edcaf71))
-    - Release rustitude-gluex v0.2.1, rustitude v0.4.2 ([`3a45077`](https://github.com/denehoffman/rustitude/commit/3a45077dcd7413ac50e5ec45dc98826b11d789fb))
+    - Bump python library version ([`9d854af`](https://github.com/denehoffman/rustitude/commit/9d854af5046ac30aacc6c369716337a863b4279a))
     - Major move required to have rustitude function properly as a Rust crate. I set this up very wrong the first time ([`9089c84`](https://github.com/denehoffman/rustitude/commit/9089c84e481124ff764b24f42507ab14913fef07))
 </details>
 
 ## 0.4.1 (2024-05-15)
 
 <csr-id-9617a27322460b378fb022ef28561f31197fc86f/>
 <csr-id-64ec5097cc99eb9bb6d73376e6d3b2788f637d9d/>
@@ -91,38 +79,14 @@
  - <csr-id-78b96b94097670af64886abb84ed263048e91e62/> update Cargo.tomls
  - <csr-id-8f2f28c972c20c0b8cef2869ab08fc4abaec5cf7/> move rustitude to crates subdirectory
 
 ### Refactor
 
  - <csr-id-097311224630f5a4d98381a11d2917ca6378ad46/> move rustitude into the crates directory and add to workspace
 
-### Commit Statistics
-
-<csr-read-only-do-not-edit/>
-
- - 7 commits contributed to the release over the course of 1 calendar day.
- - 6 commits were understood as [conventional](https://www.conventionalcommits.org).
- - 0 issues like '(#ID)' were seen in commit messages
-
-### Commit Details
-
-<csr-read-only-do-not-edit/>
-
-<details><summary>view details</summary>
-
- * **Uncategorized**
-    - Release rustitude v0.4.1 ([`9f6b0c5`](https://github.com/denehoffman/rustitude/commit/9f6b0c5570050312cc7f5ed1609d37e0f6f0aaca))
-    - Add package info into workspace ([`740a018`](https://github.com/denehoffman/rustitude/commit/740a0186ae22bdab87f514a5e035f3917a531c86))
-    - Move rustitude into the crates directory and add to workspace ([`0973112`](https://github.com/denehoffman/rustitude/commit/097311224630f5a4d98381a11d2917ca6378ad46))
-    - Merge rustitude-core to crates subdirectory ([`9617a27`](https://github.com/denehoffman/rustitude/commit/9617a27322460b378fb022ef28561f31197fc86f))
-    - More Cargo.lock and readme updates ([`64ec509`](https://github.com/denehoffman/rustitude/commit/64ec5097cc99eb9bb6d73376e6d3b2788f637d9d))
-    - Update Cargo.tomls ([`78b96b9`](https://github.com/denehoffman/rustitude/commit/78b96b94097670af64886abb84ed263048e91e62))
-    - Move rustitude to crates subdirectory ([`8f2f28c`](https://github.com/denehoffman/rustitude/commit/8f2f28c972c20c0b8cef2869ab08fc4abaec5cf7))
-</details>
-
 ## 0.4.0 (2024-05-15)
 
 <csr-id-f39aab03b7160ba3817614170d67bfcfdb22642b/>
 
 ### Bug Fixes
 
  - <csr-id-b71f07c33445f310969e445e7b158bdeef726a8d/> make add_submodule public
```

### Comparing `rustitude-0.4.3/crates/rustitude/pyproject.toml` & `rustitude-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [tool.maturin]
 module-name = "rustitude._rustitude"
 features = ["pyo3/extension-module"]
+manifest-path = "py-rustitude/Cargo.toml"
 
 [project]
 name = "rustitude"
-version = "0.4.0"
 description = "Python bindings for the Rustitude library"
 readme = "README.md"
+version = "0.5.0"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["physics", "math", "rust"]
 authors = [{ email = "dene@cmu.edu" }, { name = "Nathaniel Dene Hoffman" }]
 maintainers = [{ name = "Nathaniel Dene Hoffman", email = "dene@cmu.edu" }]
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `rustitude-0.4.3/README.md` & `rustitude-0.5.0/py-rustitude/README.md`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.3/py-rustitude/LICENSE` & `rustitude-0.5.0/py-rustitude/LICENSE`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.3/py-rustitude/README.md` & `rustitude-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 # res = m_data([1.0, 3.4, 2.8, -3.6, ... ])
 # -> [5.3, 0.2, ...], a list of intensities from the amplitude calculation
 
 # Or, what we probably want to do is find the negative log-likelihood for some choice of parameters:
 
 nll = rt.ExtendedLogLikelihood(m_data, m_mc)
 
-res = nll([10.0] * mod.get_n_free())
+res = nll([10.0] * mod.n_free)
 print(res) # prints some value for the NLL
 ```
 
 See the [`rustitude-gluex`](https://github.com/denehoffman/rustitude/tree/main/crates/rustitude-gluex) package for some of the currently implemented amplitudes (derived from GlueX's [halld_sim](https://github.com/JeffersonLab/halld_sim) repo). There are also some helper methods `Scalar`, `CScalar`, and `PCScalar` to create amplitudes which represent a single free parameter, a single complex free parameter, and a single complex free parameter in polar coordinates respectively.
 
 # TODOs
```

#### html2text {}

```diff
@@ -104,24 +104,24 @@
 up some datasets. rustitude provides an open operation that uses uproot under
 the hood: ds = rt.open('data.root') ds_mc = rt.open('mc.root') m_data =
 rt.Manager(mod, ds) m_mc = rt.Manager(mod, ds_mc) # We could stop here and
 evaluate just one dataset at a time: # res = m_data([1.0, 3.4, 2.8, -3.6, ...
 ]) # -> [5.3, 0.2, ...], a list of intensities from the amplitude calculation #
 Or, what we probably want to do is find the negative log-likelihood for some
 choice of parameters: nll = rt.ExtendedLogLikelihood(m_data, m_mc) res = nll(
-[10.0] * mod.get_n_free()) print(res) # prints some value for the NLL ``` See
-the [`rustitude-gluex`](https://github.com/denehoffman/rustitude/tree/main/
-crates/rustitude-gluex) package for some of the currently implemented
-amplitudes (derived from GlueX's [halld_sim](https://github.com/JeffersonLab/
-halld_sim) repo). There are also some helper methods `Scalar`, `CScalar`, and
-`PCScalar` to create amplitudes which represent a single free parameter, a
-single complex free parameter, and a single complex free parameter in polar
-coordinates respectively. # TODOs In no particular order, here is a list of
-what (probably) needs to be done before I will stop making any breaking
-changes: - Pure Rust parsing of ROOT files without the `uproot` backend (I have
-some moderate success with `oxyroot`, but there are still a few issues reading
-larger files) - Add plotting methods - A way to check if the number of
-parameters matches the input at compile time would be nice, not sure if it's
-possible though - Give managers a way to apply amplitudes to new datasets, like
-using the result from a fit to weight some generated Monte-Carlo for plotting
-the result. This is possible to do through Python, but a convenience method is
-probably needed - Lots of documentation - Lots of tests
+[10.0] * mod.n_free) print(res) # prints some value for the NLL ``` See the
+[`rustitude-gluex`](https://github.com/denehoffman/rustitude/tree/main/crates/
+rustitude-gluex) package for some of the currently implemented amplitudes
+(derived from GlueX's [halld_sim](https://github.com/JeffersonLab/halld_sim)
+repo). There are also some helper methods `Scalar`, `CScalar`, and `PCScalar`
+to create amplitudes which represent a single free parameter, a single complex
+free parameter, and a single complex free parameter in polar coordinates
+respectively. # TODOs In no particular order, here is a list of what (probably)
+needs to be done before I will stop making any breaking changes: - Pure Rust
+parsing of ROOT files without the `uproot` backend (I have some moderate
+success with `oxyroot`, but there are still a few issues reading larger files)
+- Add plotting methods - A way to check if the number of parameters matches the
+input at compile time would be nice, not sure if it's possible though - Give
+managers a way to apply amplitudes to new datasets, like using the result from
+a fit to weight some generated Monte-Carlo for plotting the result. This is
+possible to do through Python, but a convenience method is probably needed -
+Lots of documentation - Lots of tests
```

### Comparing `rustitude-0.4.3/py-rustitude/bacon.toml` & `rustitude-0.5.0/py-rustitude/bacon.toml`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.3/py-rustitude/rustitude/__init__.py` & `rustitude-0.5.0/py-rustitude/rustitude/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 import numpy as np
 import uproot
 
-from ._rustitude import amplitude, dataset, four_momentum, gluex, manager
+from ._rustitude import amplitude, dataset, four_momentum, gluex, manager, __version__
 from .amplitude import CScalar, PCScalar, Scalar, PiecewiseM, AmpOp, Parameter, Model, Amplitude
 from .dataset import Event, Dataset
 from .manager import ExtendedLogLikelihood, Manager
 
+__version__: str = __version__
+
 __all__ = [
+    '__version__',
     'dataset',
     'manager',
     'amplitude',
     'four_momentum',
     'Event',
     'Dataset',
     'Manager',
```

### Comparing `rustitude-0.4.3/py-rustitude/rustitude/__init__.pyi` & `rustitude-0.5.0/py-rustitude/rustitude/__init__.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,108 @@
 from pathlib import Path
 from typing import Self
 
+
 class Parameter:
     amplitude: str
     name: str
+    index: int | None
+    fixed_index: int | None
     initial: float
     bounds: tuple[float, float]
 
     def __init__(self, amplitude: str, name: str, index: int) -> None: ...
 
+
 class AmpOp:
     def print_tree(self): ...
     def real(self) -> Self: ...
     def imag(self) -> Self: ...
     def norm_sqr(self) -> Self: ...
     def __add__(self, other: Self) -> Self: ...
     def __mul__(self, other: Self) -> Self: ...
 
+
 def Scalar(name: str) -> AmpOp: ...
 def CScalar(name: str) -> AmpOp: ...
 def PCScalar(name: str) -> AmpOp: ...
 def PiecewiseM(name: str, bins: int, range: tuple[float, float]) -> AmpOp: ...
 
+
 class Amplitude:
     name: str
     active: bool
     cache_position: int
     parameter_index_start: int
 
+
 class Model:
     root: AmpOp
     amplitudes: list[Amplitude]
     parameters: list[Parameter]
+    bounds: list[tuple[float, float]]
+    initial: list[float]
+    n_free: int
 
     def __init__(self, root: AmpOp) -> None: ...
     def get_parameter(self, amplitude_name: str, parameter_name: str) -> Parameter | None: ...
     def print_parameters(self) -> None: ...
     def constrain(
         self, amplitude_1: str, parameter_1: str, amplitude_2: str, parameter_2: str
     ) -> None: ...
     def fix(self, amplitude_1: str, parameter_1: str, value: float) -> None: ...
     def free(self, amplitude_1: str, parameter_1: str) -> None: ...
     def set_bounds(
         self, amplitude_1: str, parameter_1: str, bounds: tuple[float, float]
     ) -> None: ...
     def set_initial(self, amplitude_1: str, parameter_1: str, initial: float) -> None: ...
-    def get_bounds(self) -> list[tuple[float, float]]: ...
-    def get_initial(self) -> list[float]: ...
-    def get_n_free(self) -> int: ...
     def activate(self, amplitude: str) -> None: ...
     def deactivate(self, amplitude: str) -> None: ...
 
+
 class FourMomentum:
+    e: float
+    px: float
+    py: float
+    pz: float
+    m: float
+    m2: float
+
     def __init__(self, e: float, px: float, py: float, pz: float) -> None: ...
-    def e(self) -> float: ...
-    def px(self) -> float: ...
-    def py(self) -> float: ...
-    def pz(self) -> float: ...
     def set_e(self, value: float) -> None: ...
     def set_px(self, value: float) -> None: ...
     def set_py(self, value: float) -> None: ...
     def set_pz(self, value: float) -> None: ...
-    def m2(self) -> float: ...
-    def m(self) -> float: ...
     def boost_along(self, other: FourMomentum) -> float: ...
     def __add__(self, other: FourMomentum) -> FourMomentum: ...
     def __sub__(self, other: FourMomentum) -> FourMomentum: ...
 
+
 class Event:
     index: int
     weight: float
     beam_p4: FourMomentum
     recoil_p4: FourMomentum
     daughter_p4s: list[FourMomentum]
     eps: list[float]
 
+
 class Dataset:
+    events: list[Event]
+    weights: list[float]
+
     def __getitem__(self, index: int) -> Event: ...
     def __len__(self) -> int: ...
     def split_m(
         self,
         range: tuple[float, float],  # noqa: A002
         bins: int,
         p1_indices: list[float] | None = None,
         p2_indices: list[float] | None = None,
     ) -> tuple[list[Dataset], Dataset, Dataset]: ...
-    def events(self) -> list[Event]: ...
     @staticmethod
     def from_events(events: list[Event]) -> Dataset: ...
     @staticmethod
     def from_dict(data: dict[str, list[float | list[float]]]) -> Dataset: ...
     @staticmethod
     def from_parquet(path: str) -> Dataset: ...
     @staticmethod
@@ -97,18 +110,51 @@
     @staticmethod
     def from_parquet_with_eps(path: str, eps: list[float]) -> Dataset: ...
     @staticmethod
     def from_parquet_unpolarized(path: str) -> Dataset: ...
     @staticmethod
     def from_root(path: str) -> Dataset: ...
 
+
 def open(
     file_name: str | Path, tree_name: str | None = None, *, pol_in_beam: bool = False
 ) -> Dataset: ...  # noqa: A001
 
+
 class Manager:
+    root: AmpOp
+    amplitudes: list[Amplitude]
+    parameters: list[Parameter]
+    bounds: list[tuple[float, float]]
+    initial: list[float]
+    n_free: int
+
     def __init__(self, model: Model, dataset: Dataset) -> None: ...
     def __call__(self, parameters: list[float]) -> list[float]: ...
+    def fix(self, amplitude_1: str, parameter_1: str, value: float) -> None: ...
+    def free(self, amplitude_1: str, parameter_1: str) -> None: ...
+    def set_bounds(
+        self, amplitude_1: str, parameter_1: str, bounds: tuple[float, float]
+    ) -> None: ...
+    def set_initial(self, amplitude_1: str, parameter_1: str, initial: float) -> None: ...
+    def activate(self, amplitude: str) -> None: ...
+    def deactivate(self, amplitude: str) -> None: ...
+
 
 class ExtendedLogLikelihood:
+    root: AmpOp
+    amplitudes: list[Amplitude]
+    parameters: list[Parameter]
+    bounds: list[tuple[float, float]]
+    initial: list[float]
+    n_free: int
+
     def __init__(self, data_manager: Manager, mc_manager: Manager) -> None: ...
     def __call__(self, parameters: list[float], *, num_threads: int = 1) -> float: ...
+    def fix(self, amplitude_1: str, parameter_1: str, value: float) -> None: ...
+    def free(self, amplitude_1: str, parameter_1: str) -> None: ...
+    def set_bounds(
+        self, amplitude_1: str, parameter_1: str, bounds: tuple[float, float]
+    ) -> None: ...
+    def set_initial(self, amplitude_1: str, parameter_1: str, initial: float) -> None: ...
+    def activate(self, amplitude: str) -> None: ...
+    def deactivate(self, amplitude: str) -> None: ...
```

### Comparing `rustitude-0.4.3/py-rustitude/rustitude/gluex/harmonics.pyi` & `rustitude-0.5.0/py-rustitude/rustitude/gluex/harmonics.pyi`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.3/py-rustitude/rustitude/gluex/resonances.pyi` & `rustitude-0.5.0/py-rustitude/rustitude/gluex/resonances.pyi`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.3/Cargo.lock` & `rustitude-0.5.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -258,17 +258,17 @@
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
 name = "cc"
-version = "1.0.97"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "099a5357d84c4c61eb35fc8eafa9a79a902c2f76911e5747ced4e032edd8d9b4"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 dependencies = [
  "jobserver",
  "libc",
  "once_cell",
 ]
 
 [[package]]
@@ -367,17 +367,17 @@
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "crc32fast"
-version = "1.4.0"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
+checksum = "a97769d94ddab943e4510d138150169a2758b5ef3eb191a9ee688de3e23ef7b3"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "criterion"
 version = "0.5.1"
@@ -431,17 +431,17 @@
 checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+checksum = "22ec99545bb0ed0ea7bb9b8e1e9122ea386ff8a48c0922e43f36d45ab09e0e80"
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
@@ -449,17 +449,17 @@
 name = "downcast"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1435fa1053d8b2fbbe9be7e97eca7f33d37b28409959813daefc1446a14247f1"
 
 [[package]]
 name = "either"
-version = "1.11.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
@@ -610,14 +610,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "413ee7dfc52ee1a4949ceeb7dbc8a33f2d6c088194d9f922fb8318faf1f01186"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
@@ -705,17 +714,17 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.154"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
@@ -798,17 +807,17 @@
 checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
+checksum = "87dfd01fe195c66b572b37921ad8803d010623c0aca821bea2302239d155cdae"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "nalgebra"
 version = "0.32.5"
@@ -873,15 +882,15 @@
 name = "num-derive"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed3955f1a9c7c0c15e092f9c887db08b1fc683305fdf6eb6684f22555355e202"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.63",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "num-integer"
 version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
@@ -1030,47 +1039,53 @@
 name = "pkg-config"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
 name = "plotters"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
+checksum = "a15b6eccb8484002195a3e44fe65a4ce8e93a625797a063735536fd59cb01cf3"
 dependencies = [
  "num-traits",
  "plotters-backend",
  "plotters-svg",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "plotters-backend"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e76628b4d3a7581389a35d5b6e2139607ad7c75b17aed325f210aa91f4a9609"
+checksum = "414cec62c6634ae900ea1c56128dfe87cf63e7caece0852ec76aba307cebadb7"
 
 [[package]]
 name = "plotters-svg"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
+checksum = "81b30686a7d9c3e010b84284bdd26a29f2138574f52f5eb6f794fc0ad924e705"
 dependencies = [
  "plotters-backend",
 ]
 
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
+name = "ppv-lite86"
+version = "0.2.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
+
+[[package]]
 name = "primal-bit"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6ce4fe11b2a87850ca3bd5dc9c7cb9f66e32a09edab221be406ac5ff677f2241"
 dependencies = [
  "hamming",
 ]
@@ -1090,25 +1105,26 @@
  "primal-bit",
  "primal-estimate",
  "smallvec",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.82"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
+checksum = "0b33eb56c327dec362a9e55b3ad14f9d2f0904fb5a5b03b513ab5465399e9f43"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py-rustitude"
-version = "0.4.1"
+version = "0.5.0"
 dependencies = [
+ "nalgebra",
  "pyo3",
  "rayon",
  "rustitude",
  "rustitude-core",
  "rustitude-gluex",
 ]
 
@@ -1155,40 +1171,70 @@
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.63",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.63",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "rand"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
+dependencies = [
+ "libc",
+ "rand_chacha",
+ "rand_core",
+]
+
+[[package]]
+name = "rand_chacha"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6c10a63a0fa32252be49d21e7709d4d4baf8d231c2dbce1eaa8141b9b127d88"
+dependencies = [
+ "ppv-lite86",
+ "rand_core",
+]
+
+[[package]]
+name = "rand_core"
+version = "0.6.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
+dependencies = [
+ "getrandom",
+]
+
+[[package]]
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
@@ -1255,28 +1301,29 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustitude"
-version = "0.4.3"
+version = "0.5.0"
 dependencies = [
  "criterion",
+ "rand",
  "rustitude-core",
  "rustitude-gluex",
 ]
 
 [[package]]
 name = "rustitude-core"
-version = "1.0.1"
+version = "1.1.0"
 dependencies = [
  "approx",
  "indexmap",
- "itertools 0.12.1",
+ "itertools 0.13.0",
  "nalgebra",
  "num",
  "num-complex",
  "num-traits",
  "oxyroot",
  "parking_lot",
  "parquet",
@@ -1284,15 +1331,15 @@
  "rayon",
  "sphrs",
  "thiserror",
 ]
 
 [[package]]
 name = "rustitude-gluex"
-version = "0.2.2"
+version = "0.3.0"
 dependencies = [
  "factorial",
  "nalgebra",
  "num-complex",
  "pyo3",
  "rayon",
  "rustitude-core",
@@ -1354,15 +1401,15 @@
 name = "serde_derive"
 version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.63",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
@@ -1423,47 +1470,47 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.63"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf5be731623ca1a1fb7d8be6f261a3be6d3e2337b8a1f97be944d020c8fcb704"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.60"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.60"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.63",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "thrift"
 version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e54bc85fc7faa8bc175c4bab5b92ba8d9a3ce893d0e9f42cc455c8ab16a9e09"
@@ -1576,15 +1623,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.63",
+ "syn 2.0.66",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1598,15 +1645,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.63",
+ "syn 2.0.66",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -1621,17 +1668,17 @@
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "wide"
-version = "0.7.19"
+version = "0.7.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aab6594190de06d718a5dbc5fa781ab62f8903797056480e549ca74add6b7065"
+checksum = "21e005a4cc35784183a9e39cb22e9a9c46353ef6a7f113fd8d36ddc58c15ef3c"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "winapi-util"
@@ -1746,15 +1793,15 @@
 name = "zerocopy-derive"
 version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.63",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "zstd"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
```

### Comparing `rustitude-0.4.3/Cargo.toml` & `rustitude-0.5.0/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 [workspace]
 members = ["crates/*", "py-rustitude"]
 resolver = "2"
 default-members = ["crates/*"]
 
 [workspace.package]
-version = "0.4.1"
+version = "0.5.0"
 edition = "2021"
 authors = ["Nathaniel Dene Hoffman <dene@cmu.edu>"]
 description = "A library to create and operate models for particle physics amplitude analyses"
 repository = "https://github.com/denehoffman/rustitude/"
 homepage = "https://github.com/denehoffman/rustitude/"
 license-file = "LICENSE"
 
 [workspace.dependencies]
-rustitude = { version = "0.4.1", path = "crates/rustitude", default-features = false }
-rustitude-core = { version = "1.0.0", path = "crates/rustitude-core", default-features = false }
-rustitude-gluex = { version = "0.2.0", path = "crates/rustitude-gluex", default-features = false }
-criterion = "0.5.1"
-rayon = { version = "1.8.0" }
+rustitude = { version = "0.5.0", path = "crates/rustitude", default-features = false }
+rustitude-core = { version = "1.1.0", path = "crates/rustitude-core", default-features = false }
+rustitude-gluex = { version = "0.3.0", path = "crates/rustitude-gluex", default-features = false }
+rayon = { version = "1.10.0" }
 approx = { version = "0.5.1", features = ["num-complex"] }
-nalgebra = "0.32.3"
-num = "0.4.1"
-num-complex = "0.4.4"
-num-traits = "0.2.17"
+nalgebra = "0.32.5"
+num = "0.4.3"
+num-complex = "0.4.6"
+num-traits = "0.2.19"
 parquet = "51.0.0"
 indexmap = "2.2.6"
-parking_lot = "0.12.1"
-oxyroot = "0.1.18"
-itertools = "0.12.1"
+parking_lot = "0.12.2"
+oxyroot = "0.1.24"
+itertools = "0.13.0"
 pyo3 = "0.21.2"
-thiserror = "1.0.60"
+thiserror = "1.0.61"
 factorial = "0.4.0"
 sphrs = "0.2.2"
+criterion = "0.5.1"
+rand = "0.8.5"
+
+[profile.release]
+lto = true
+codegen-units = 1
+panic = "abort"
```

### Comparing `rustitude-0.4.3/rustitude/__init__.py` & `rustitude-0.5.0/rustitude/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 import numpy as np
 import uproot
 
-from ._rustitude import amplitude, dataset, four_momentum, gluex, manager
+from ._rustitude import amplitude, dataset, four_momentum, gluex, manager, __version__
 from .amplitude import CScalar, PCScalar, Scalar, PiecewiseM, AmpOp, Parameter, Model, Amplitude
 from .dataset import Event, Dataset
 from .manager import ExtendedLogLikelihood, Manager
 
+__version__: str = __version__
+
 __all__ = [
+    '__version__',
     'dataset',
     'manager',
     'amplitude',
     'four_momentum',
     'Event',
     'Dataset',
     'Manager',
```

### Comparing `rustitude-0.4.3/rustitude/__init__.pyi` & `rustitude-0.5.0/rustitude/__init__.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,108 @@
 from pathlib import Path
 from typing import Self
 
+
 class Parameter:
     amplitude: str
     name: str
+    index: int | None
+    fixed_index: int | None
     initial: float
     bounds: tuple[float, float]
 
     def __init__(self, amplitude: str, name: str, index: int) -> None: ...
 
+
 class AmpOp:
     def print_tree(self): ...
     def real(self) -> Self: ...
     def imag(self) -> Self: ...
     def norm_sqr(self) -> Self: ...
     def __add__(self, other: Self) -> Self: ...
     def __mul__(self, other: Self) -> Self: ...
 
+
 def Scalar(name: str) -> AmpOp: ...
 def CScalar(name: str) -> AmpOp: ...
 def PCScalar(name: str) -> AmpOp: ...
 def PiecewiseM(name: str, bins: int, range: tuple[float, float]) -> AmpOp: ...
 
+
 class Amplitude:
     name: str
     active: bool
     cache_position: int
     parameter_index_start: int
 
+
 class Model:
     root: AmpOp
     amplitudes: list[Amplitude]
     parameters: list[Parameter]
+    bounds: list[tuple[float, float]]
+    initial: list[float]
+    n_free: int
 
     def __init__(self, root: AmpOp) -> None: ...
     def get_parameter(self, amplitude_name: str, parameter_name: str) -> Parameter | None: ...
     def print_parameters(self) -> None: ...
     def constrain(
         self, amplitude_1: str, parameter_1: str, amplitude_2: str, parameter_2: str
     ) -> None: ...
     def fix(self, amplitude_1: str, parameter_1: str, value: float) -> None: ...
     def free(self, amplitude_1: str, parameter_1: str) -> None: ...
     def set_bounds(
         self, amplitude_1: str, parameter_1: str, bounds: tuple[float, float]
     ) -> None: ...
     def set_initial(self, amplitude_1: str, parameter_1: str, initial: float) -> None: ...
-    def get_bounds(self) -> list[tuple[float, float]]: ...
-    def get_initial(self) -> list[float]: ...
-    def get_n_free(self) -> int: ...
     def activate(self, amplitude: str) -> None: ...
     def deactivate(self, amplitude: str) -> None: ...
 
+
 class FourMomentum:
+    e: float
+    px: float
+    py: float
+    pz: float
+    m: float
+    m2: float
+
     def __init__(self, e: float, px: float, py: float, pz: float) -> None: ...
-    def e(self) -> float: ...
-    def px(self) -> float: ...
-    def py(self) -> float: ...
-    def pz(self) -> float: ...
     def set_e(self, value: float) -> None: ...
     def set_px(self, value: float) -> None: ...
     def set_py(self, value: float) -> None: ...
     def set_pz(self, value: float) -> None: ...
-    def m2(self) -> float: ...
-    def m(self) -> float: ...
     def boost_along(self, other: FourMomentum) -> float: ...
     def __add__(self, other: FourMomentum) -> FourMomentum: ...
     def __sub__(self, other: FourMomentum) -> FourMomentum: ...
 
+
 class Event:
     index: int
     weight: float
     beam_p4: FourMomentum
     recoil_p4: FourMomentum
     daughter_p4s: list[FourMomentum]
     eps: list[float]
 
+
 class Dataset:
+    events: list[Event]
+    weights: list[float]
+
     def __getitem__(self, index: int) -> Event: ...
     def __len__(self) -> int: ...
     def split_m(
         self,
         range: tuple[float, float],  # noqa: A002
         bins: int,
         p1_indices: list[float] | None = None,
         p2_indices: list[float] | None = None,
     ) -> tuple[list[Dataset], Dataset, Dataset]: ...
-    def events(self) -> list[Event]: ...
     @staticmethod
     def from_events(events: list[Event]) -> Dataset: ...
     @staticmethod
     def from_dict(data: dict[str, list[float | list[float]]]) -> Dataset: ...
     @staticmethod
     def from_parquet(path: str) -> Dataset: ...
     @staticmethod
@@ -97,18 +110,51 @@
     @staticmethod
     def from_parquet_with_eps(path: str, eps: list[float]) -> Dataset: ...
     @staticmethod
     def from_parquet_unpolarized(path: str) -> Dataset: ...
     @staticmethod
     def from_root(path: str) -> Dataset: ...
 
+
 def open(
     file_name: str | Path, tree_name: str | None = None, *, pol_in_beam: bool = False
 ) -> Dataset: ...  # noqa: A001
 
+
 class Manager:
+    root: AmpOp
+    amplitudes: list[Amplitude]
+    parameters: list[Parameter]
+    bounds: list[tuple[float, float]]
+    initial: list[float]
+    n_free: int
+
     def __init__(self, model: Model, dataset: Dataset) -> None: ...
     def __call__(self, parameters: list[float]) -> list[float]: ...
+    def fix(self, amplitude_1: str, parameter_1: str, value: float) -> None: ...
+    def free(self, amplitude_1: str, parameter_1: str) -> None: ...
+    def set_bounds(
+        self, amplitude_1: str, parameter_1: str, bounds: tuple[float, float]
+    ) -> None: ...
+    def set_initial(self, amplitude_1: str, parameter_1: str, initial: float) -> None: ...
+    def activate(self, amplitude: str) -> None: ...
+    def deactivate(self, amplitude: str) -> None: ...
+
 
 class ExtendedLogLikelihood:
+    root: AmpOp
+    amplitudes: list[Amplitude]
+    parameters: list[Parameter]
+    bounds: list[tuple[float, float]]
+    initial: list[float]
+    n_free: int
+
     def __init__(self, data_manager: Manager, mc_manager: Manager) -> None: ...
     def __call__(self, parameters: list[float], *, num_threads: int = 1) -> float: ...
+    def fix(self, amplitude_1: str, parameter_1: str, value: float) -> None: ...
+    def free(self, amplitude_1: str, parameter_1: str) -> None: ...
+    def set_bounds(
+        self, amplitude_1: str, parameter_1: str, bounds: tuple[float, float]
+    ) -> None: ...
+    def set_initial(self, amplitude_1: str, parameter_1: str, initial: float) -> None: ...
+    def activate(self, amplitude: str) -> None: ...
+    def deactivate(self, amplitude: str) -> None: ...
```

### Comparing `rustitude-0.4.3/rustitude/gluex/resonances.pyi` & `rustitude-0.5.0/rustitude/gluex/resonances.pyi`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.3/rustitude/gluex/harmonics.pyi` & `rustitude-0.5.0/rustitude/gluex/harmonics.pyi`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.3/LICENSE` & `rustitude-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.3/PKG-INFO` & `rustitude-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rustitude
-Version: 0.4.3
+Version: 0.5.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Dist: uproot
 Requires-Dist: numpy
 License-File: LICENSE
 License-File: LICENSE
 Summary: Python bindings for the Rustitude library
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: rustitude Version: 0.4.3 Classifier: Development
+Metadata-Version: 2.3 Name: rustitude Version: 0.5.0 Classifier: Development
 Status :: 4 - Beta Classifier: Programming Language :: Python Requires-Dist:
 uproot Requires-Dist: numpy License-File: LICENSE License-File: LICENSE
 Summary: Python bindings for the Rustitude library Keywords: physics,math,rust
 Author: Nathaniel Dene Hoffman Author-email: dene@cmu.edu Maintainer-email:
 Nathaniel Dene Hoffman
 cmu.edu> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Project-URL: homepage, https://github.com/
```

