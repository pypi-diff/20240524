# Comparing `tmp/uv-0.2.2.tar.gz` & `tmp/uv-0.2.3.tar.gz`

## Comparing `uv-0.2.2.tar` & `uv-0.2.3.tar`

### file list

```diff
@@ -1,391 +1,393 @@
--rw-r--r--   0     1001      127      897 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-extract/Cargo.toml
--rw-r--r--   0     1001      127     1078 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-extract/src/error.rs
--rw-r--r--   0     1001      127     4113 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-extract/src/hash.rs
--rw-r--r--   0     1001      127      112 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-extract/src/lib.rs
--rw-r--r--   0     1001      127     9419 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-extract/src/stream.rs
--rw-r--r--   0     1001      127     3565 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-extract/src/sync.rs
--rw-r--r--   0     1001      127     1489 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-extract/src/tar.rs
--rw-r--r--   0     1001      127     5685 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-extract/src/vendor/cloneable_seekable_reader.rs
--rw-r--r--   0     1001      127      112 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-extract/src/vendor/mod.rs
--rw-r--r--   0     1001      127      790 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-types/Cargo.toml
--rw-r--r--   0     1001      127      423 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-types/src/builds.rs
--rw-r--r--   0     1001      127      239 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-types/src/downloads.rs
--rw-r--r--   0     1001      127     6228 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-types/src/hash.rs
--rw-r--r--   0     1001      127      219 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-types/src/lib.rs
--rw-r--r--   0     1001      127     1478 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-types/src/requirements.rs
--rw-r--r--   0     1001      127     6944 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-types/src/traits.rs
--rw-r--r--   0     1001      127     1504 2024-05-22 21:46:28.000000 uv-0.2.2/crates/install-wheel-rs/Cargo.toml
--rw-r--r--   0     1001      127      515 2024-05-22 21:46:28.000000 uv-0.2.2/crates/install-wheel-rs/Readme.md
--rw-r--r--   0     1001      127     4332 2024-05-22 21:46:28.000000 uv-0.2.2/crates/install-wheel-rs/src/lib.rs
--rw-r--r--   0     1001      127    20181 2024-05-22 21:46:28.000000 uv-0.2.2/crates/install-wheel-rs/src/linker.rs
--rw-r--r--   0     1001      127     7104 2024-05-22 21:46:28.000000 uv-0.2.2/crates/install-wheel-rs/src/metadata.rs
--rw-r--r--   0     1001      127      474 2024-05-22 21:46:28.000000 uv-0.2.2/crates/install-wheel-rs/src/record.rs
--rw-r--r--   0     1001      127     5550 2024-05-22 21:46:28.000000 uv-0.2.2/crates/install-wheel-rs/src/script.rs
--rw-r--r--   0     1001      127    11211 2024-05-22 21:46:28.000000 uv-0.2.2/crates/install-wheel-rs/src/uninstall.rs
--rw-r--r--   0     1001      127    34841 2024-05-22 21:46:28.000000 uv-0.2.2/crates/install-wheel-rs/src/wheel.rs
--rw-r--r--   0     1001      127     1808 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/Cargo.toml
--rwxr-xr-x   0     1001      127     7922 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/fetch-version-metadata.py
--rw-r--r--   0     1001      127        0 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/python/__init__.py
--rw-r--r--   0     1001      127    21931 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/python/get_interpreter_info.py
--rw-r--r--   0     1001      127    10174 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/python/packaging/LICENSE.APACHE
--rw-r--r--   0     1001      127     1344 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/python/packaging/LICENSE.BSD
--rw-r--r--   0     1001      127      316 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/python/packaging/README.md
--rw-r--r--   0     1001      127      501 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/python/packaging/__init__.py
--rw-r--r--   0     1001      127     3282 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/python/packaging/_elffile.py
--rw-r--r--   0     1001      127     9588 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/python/packaging/_manylinux.py
--rw-r--r--   0     1001      127     2696 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/python/packaging/_musllinux.py
--rw-r--r--   0     1001      127   182247 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/python-version-metadata.json
--rw-r--r--   0     1001      127    54613 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/src/discovery.rs
--rw-r--r--   0     1001      127     8958 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/src/environment.rs
--rw-r--r--   0     1001      127     1314 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/src/implementation.rs
--rw-r--r--   0     1001      127    27969 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/src/interpreter.rs
--rw-r--r--   0     1001      127    77473 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/src/lib.rs
--rw-r--r--   0     1001      127     8104 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/src/managed/downloads.rs
--rw-r--r--   0     1001      127     5960 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/src/managed/find.rs
--rw-r--r--   0     1001      127      253 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/src/managed/mod.rs
--rw-r--r--   0     1001      127   224411 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/src/managed/python_versions.inc
--rw-r--r--   0     1001      127      691 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/src/managed/python_versions.inc.mustache
--rw-r--r--   0     1001      127     4389 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/src/platform.rs
--rw-r--r--   0     1001      127      430 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/src/pointer_size.rs
--rw-r--r--   0     1001      127     3234 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/src/py_launcher.rs
--rw-r--r--   0     1001      127     7736 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/src/python_version.rs
--rw-r--r--   0     1001      127      950 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/src/target.rs
--rw-r--r--   0     1001      127     5672 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/src/virtualenv.rs
--rw-r--r--   0     1001      127     2708 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-interpreter/template-version-metadata.py
--rw-r--r--   0     1001      127      411 2024-05-22 21:46:28.000000 uv-0.2.2/crates/once-map/Cargo.toml
--rw-r--r--   0     1001      127     3940 2024-05-22 21:46:28.000000 uv-0.2.2/crates/once-map/src/lib.rs
--rw-r--r--   0     1001      127      822 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pypi-types/Cargo.toml
--rw-r--r--   0     1001      127     1609 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pypi-types/src/base_url.rs
--rw-r--r--   0     1001      127     4643 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pypi-types/src/direct_url.rs
--rw-r--r--   0     1001      127    15738 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pypi-types/src/lenient_requirement.rs
--rw-r--r--   0     1001      127      239 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pypi-types/src/lib.rs
--rw-r--r--   0     1001      127    19433 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pypi-types/src/metadata.rs
--rw-r--r--   0     1001      127      575 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pypi-types/src/scheme.rs
--rw-r--r--   0     1001      127    12178 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pypi-types/src/simple_json.rs
--rw-r--r--   0     1001      127      752 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-auth/Cargo.toml
--rw-r--r--   0     1001      127     9542 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-auth/src/cache.rs
--rw-r--r--   0     1001      127    11219 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-auth/src/credentials.rs
--rw-r--r--   0     1001      127     9340 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-auth/src/keyring.rs
--rw-r--r--   0     1001      127      992 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-auth/src/lib.rs
--rw-r--r--   0     1001      127    45581 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-auth/src/middleware.rs
--rw-r--r--   0     1001      127     4661 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-auth/src/realm.rs
--rw-r--r--   0     1001      127      507 2024-05-22 21:46:28.000000 uv-0.2.2/crates/cache-key/Cargo.toml
--rw-r--r--   0     1001      127     8335 2024-05-22 21:46:28.000000 uv-0.2.2/crates/cache-key/src/cache_key.rs
--rw-r--r--   0     1001      127    12317 2024-05-22 21:46:28.000000 uv-0.2.2/crates/cache-key/src/canonical_url.rs
--rw-r--r--   0     1001      127      620 2024-05-22 21:46:28.000000 uv-0.2.2/crates/cache-key/src/digest.rs
--rw-r--r--   0     1001      127      191 2024-05-22 21:46:28.000000 uv-0.2.2/crates/cache-key/src/lib.rs
--rw-r--r--   0     1001      127     1986 2024-05-22 21:46:28.000000 uv-0.2.2/crates/cache-key/src/stable_hash.rs
--rw-r--r--   0     1001      127     1149 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/Cargo.toml
--rw-r--r--   0     1001      127     2511 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/annotation.rs
--rw-r--r--   0     1001      127     1048 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/any.rs
--rw-r--r--   0     1001      127     4711 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/buildable.rs
--rw-r--r--   0     1001      127     6718 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/cached.rs
--rw-r--r--   0     1001      127     2474 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/editable.rs
--rw-r--r--   0     1001      127      985 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/error.rs
--rw-r--r--   0     1001      127     7205 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/file.rs
--rw-r--r--   0     1001      127     2831 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/hash.rs
--rw-r--r--   0     1001      127     3845 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/id.rs
--rw-r--r--   0     1001      127    14472 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/index_url.rs
--rw-r--r--   0     1001      127    12536 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/installed.rs
--rw-r--r--   0     1001      127    35260 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/lib.rs
--rw-r--r--   0     1001      127    10788 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/parsed_url.rs
--rw-r--r--   0     1001      127    20821 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/prioritized_distribution.rs
--rw-r--r--   0     1001      127     8302 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/requirement.rs
--rw-r--r--   0     1001      127     1228 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/requirements.rs
--rw-r--r--   0     1001      127     7983 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/resolution.rs
--rw-r--r--   0     1001      127     6914 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/resolved.rs
--rw-r--r--   0     1001      127     3233 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/specified_requirement.rs
--rw-r--r--   0     1001      127     8193 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-types/src/traits.rs
--rw-r--r--   0     1001      127     1654 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-requirements/Cargo.toml
--rw-r--r--   0     1001      127     2206 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-requirements/src/confirm.rs
--rw-r--r--   0     1001      127      318 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-requirements/src/lib.rs
--rw-r--r--   0     1001      127    10108 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-requirements/src/lookahead.rs
--rw-r--r--   0     1001      127    31011 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-requirements/src/pyproject.rs
--rw-r--r--   0     1001      127     6877 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-requirements/src/source_tree.rs
--rw-r--r--   0     1001      127     7083 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-requirements/src/sources.rs
--rw-r--r--   0     1001      127    14908 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-requirements/src/specification.rs
--rw-r--r--   0     1001      127    13090 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-requirements/src/unnamed.rs
--rw-r--r--   0     1001      127     1638 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-requirements/src/upgrade.rs
--rw-r--r--   0     1001      127    25085 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-requirements/src/workspace.rs
--rw-r--r--   0     1001      127     1004 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep440-rs/Cargo.toml
--rw-r--r--   0     1001      127    10173 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep440-rs/License-Apache
--rw-r--r--   0     1001      127     1293 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep440-rs/License-BSD
--rw-r--r--   0     1001      127     2947 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep440-rs/Readme.md
--rw-r--r--   0     1001      127     2105 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep440-rs/python/Readme.md
--rw-r--r--   0     1001      127     2922 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep440-rs/src/lib.rs
--rw-r--r--   0     1001      127   131052 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep440-rs/src/version.rs
--rw-r--r--   0     1001      127    56892 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep440-rs/src/version_specifier.rs
--rw-r--r--   0     1001      127      608 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-filename/Cargo.toml
--rw-r--r--   0     1001      127     2291 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-filename/src/lib.rs
--rw-r--r--   0     1001      127      420 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_build_tag.snap
--rw-r--r--   0     1001      127      539 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_multiple_tags.snap
--rw-r--r--   0     1001      127      398 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_single_tags.snap
--rw-r--r--   0     1001      127     7565 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-filename/src/source_dist.rs
--rw-r--r--   0     1001      127    10961 2024-05-22 21:46:28.000000 uv-0.2.2/crates/distribution-filename/src/wheel.rs
--rw-r--r--   0     1001      127      918 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-git/Cargo.toml
--rw-r--r--   0     1001      127    63247 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-git/src/git.rs
--rw-r--r--   0     1001      127    37494 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-git/src/known_hosts.rs
--rw-r--r--   0     1001      127     3843 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-git/src/lib.rs
--rw-r--r--   0     1001      127      940 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-git/src/sha.rs
--rw-r--r--   0     1001      127     5058 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-git/src/source.rs
--rw-r--r--   0     1001      127     1362 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-git/src/util/errors.rs
--rw-r--r--   0     1001      127      733 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-git/src/util/mod.rs
--rw-r--r--   0     1001      127     7295 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-git/src/util/retry.rs
--rw-r--r--   0     1001      127     1002 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-workspace/Cargo.toml
--rw-r--r--   0     1001      127     7241 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-workspace/src/combine.rs
--rw-r--r--   0     1001      127      127 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-workspace/src/lib.rs
--rw-r--r--   0     1001      127     3296 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-workspace/src/settings.rs
--rw-r--r--   0     1001      127     5558 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-workspace/src/workspace.rs
--rw-r--r--   0     1001      127     1223 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/Cargo.toml
--rw-r--r--   0     1001      127    88063 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/lib.rs
--rw-r--r--   0     1001      127     2237 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/requirement.rs
--rw-r--r--   0     1001      127     6200 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-basic.txt.snap
--rw-r--r--   0     1001      127     2683 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-a.txt.snap
--rw-r--r--   0     1001      127     2273 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-b.txt.snap
--rw-r--r--   0     1001      127      284 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-empty.txt.snap
--rw-r--r--   0     1001      127     4140 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-for-poetry.txt.snap
--rw-r--r--   0     1001      127     1816 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-a.txt.snap
--rw-r--r--   0     1001      127      828 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-b.txt.snap
--rw-r--r--   0     1001      127    11863 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-poetry-with-hashes.txt.snap
--rw-r--r--   0     1001      127     2257 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-small.txt.snap
--rw-r--r--   0     1001      127     2544 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-whitespace.txt.snap
--rw-r--r--   0     1001      127     6200 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-basic.txt.snap
--rw-r--r--   0     1001      127     2683 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-a.txt.snap
--rw-r--r--   0     1001      127     2273 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-b.txt.snap
--rw-r--r--   0     1001      127      284 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-empty.txt.snap
--rw-r--r--   0     1001      127     4140 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-for-poetry.txt.snap
--rw-r--r--   0     1001      127     1816 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-a.txt.snap
--rw-r--r--   0     1001      127      828 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-b.txt.snap
--rw-r--r--   0     1001      127    11863 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-poetry-with-hashes.txt.snap
--rw-r--r--   0     1001      127     2257 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-small.txt.snap
--rw-r--r--   0     1001      127     3692 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-bare-url.txt.snap
--rw-r--r--   0     1001      127     8155 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-editable.txt.snap
--rw-r--r--   0     1001      127     2544 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-whitespace.txt.snap
--rw-r--r--   0     1001      127     3713 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-bare-url.txt.snap
--rw-r--r--   0     1001      127     8161 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-editable.txt.snap
--rw-r--r--   0     1001      127      113 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/test-data/requirements-txt/bare-url.txt
--rw-r--r--   0     1001      127       90 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/test-data/requirements-txt/basic.txt
--rw-r--r--   0     1001      127       45 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/test-data/requirements-txt/constraints-a.txt
--rw-r--r--   0     1001      127       27 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/test-data/requirements-txt/constraints-b.txt
--rw-r--r--   0     1001      127      491 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/test-data/requirements-txt/editable.txt
--rw-r--r--   0     1001      127        0 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/test-data/requirements-txt/empty.txt
--rw-r--r--   0     1001      127      101 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/test-data/requirements-txt/for-poetry.txt
--rw-r--r--   0     1001      127       43 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/test-data/requirements-txt/include-a.txt
--rw-r--r--   0     1001      127        5 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/test-data/requirements-txt/include-b.txt
--rw-r--r--   0     1001      127     1183 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/test-data/requirements-txt/poetry-with-hashes.txt
--rw-r--r--   0     1001      127       66 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/test-data/requirements-txt/small.txt
--rw-r--r--   0     1001      127      183 2024-05-22 21:46:28.000000 uv-0.2.2/crates/requirements-txt/test-data/requirements-txt/whitespace.txt
--rw-r--r--   0     1001      127      841 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-configuration/Cargo.toml
--rw-r--r--   0     1001      127     1014 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-configuration/src/authentication.rs
--rw-r--r--   0     1001      127    10722 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-configuration/src/build_options.rs
--rw-r--r--   0     1001      127     1054 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-configuration/src/concurrency.rs
--rw-r--r--   0     1001      127     9254 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-configuration/src/config_settings.rs
--rw-r--r--   0     1001      127     1698 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-configuration/src/constraints.rs
--rw-r--r--   0     1001      127      437 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-configuration/src/lib.rs
--rw-r--r--   0     1001      127     4059 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-configuration/src/name_specifiers.rs
--rw-r--r--   0     1001      127     1706 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-configuration/src/overrides.rs
--rw-r--r--   0     1001      127     2339 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-configuration/src/package_options.rs
--rw-r--r--   0     1001      127      782 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-configuration/src/preview.rs
--rw-r--r--   0     1001      127    11893 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-configuration/src/target_triple.rs
--rw-r--r--   0     1001      127     2085 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep508-rs/Cargo.toml
--rw-r--r--   0     1001      127    10173 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep508-rs/License-Apache
--rw-r--r--   0     1001      127     1293 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep508-rs/License-BSD
--rw-r--r--   0     1001      127     3039 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep508-rs/Readme.md
--rw-r--r--   0     1001      127     4301 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep508-rs/src/cursor.rs
--rw-r--r--   0     1001      127    62005 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep508-rs/src/lib.rs
--rw-r--r--   0     1001      127    94653 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep508-rs/src/marker.rs
--rw-r--r--   0     1001      127      743 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep508-rs/src/origin.rs
--rw-r--r--   0     1001      127    12553 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep508-rs/src/unnamed.rs
--rw-r--r--   0     1001      127    18647 2024-05-22 21:46:28.000000 uv-0.2.2/crates/pep508-rs/src/verbatim_url.rs
--rw-r--r--   0     1001      127     1464 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-installer/Cargo.toml
--rw-r--r--   0     1001      127    12444 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-installer/src/compile.rs
--rw-r--r--   0     1001      127     9352 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-installer/src/downloader.rs
--rw-r--r--   0     1001      127     4349 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-installer/src/editable.rs
--rw-r--r--   0     1001      127     2833 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-installer/src/installer.rs
--rw-r--r--   0     1001      127      521 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-installer/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-installer/src/pip_compileall.py
--rw-r--r--   0     1001      127    22428 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-installer/src/plan.rs
--rw-r--r--   0     1001      127     7565 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-installer/src/satisfies.rs
--rw-r--r--   0     1001      127    22636 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-installer/src/site_packages.rs
--rw-r--r--   0     1001      127      978 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-installer/src/uninstall.rs
--rw-r--r--   0     1001      127      847 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-fs/Cargo.toml
--rw-r--r--   0     1001      127     1397 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-fs/src/cachedir.rs
--rw-r--r--   0     1001      127    11067 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-fs/src/lib.rs
--rw-r--r--   0     1001      127    10859 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-fs/src/path.rs
--rw-r--r--   0     1001      127      970 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-dispatch/Cargo.toml
--rw-r--r--   0     1001      127    10910 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-dispatch/src/lib.rs
--rw-r--r--   0     1001      127      774 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-virtualenv/Cargo.toml
--rw-r--r--   0     1001      127      109 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-virtualenv/README.md
--rw-r--r--   0     1001      127     4375 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-virtualenv/src/_virtualenv.py
--rw-r--r--   0     1001      127       20 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-virtualenv/src/activator/.gitattributes
--rw-r--r--   0     1001      127     3388 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-virtualenv/src/activator/activate
--rw-r--r--   0     1001      127     2259 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-virtualenv/src/activator/activate.bat
--rw-r--r--   0     1001      127     2655 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-virtualenv/src/activator/activate.csh
--rw-r--r--   0     1001      127     4219 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-virtualenv/src/activator/activate.fish
--rw-r--r--   0     1001      127     3903 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-virtualenv/src/activator/activate.nu
--rw-r--r--   0     1001      127     2826 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-virtualenv/src/activator/activate.ps1
--rw-r--r--   0     1001      127     2411 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-virtualenv/src/activator/activate_this.py
--rw-r--r--   0     1001      127     1728 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-virtualenv/src/activator/deactivate.bat
--rw-r--r--   0     1001      127     1215 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-virtualenv/src/activator/pydoc.bat
--rw-r--r--   0     1001      127    16565 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-virtualenv/src/bare.rs
--rw-r--r--   0     1001      127     2090 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-virtualenv/src/lib.rs
--rw-r--r--   0     1001      127      472 2024-05-22 21:46:28.000000 uv-0.2.2/crates/platform-tags/Cargo.toml
--rw-r--r--   0     1001      127      161 2024-05-22 21:46:28.000000 uv-0.2.2/crates/platform-tags/src/lib.rs
--rw-r--r--   0     1001      127     3507 2024-05-22 21:46:28.000000 uv-0.2.2/crates/platform-tags/src/platform.rs
--rw-r--r--   0     1001      127    76059 2024-05-22 21:46:28.000000 uv-0.2.2/crates/platform-tags/src/tags.rs
--rw-r--r--   0     1001      127     1145 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-build/Cargo.toml
--rw-r--r--   0     1001      127       17 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-build/.gitignore
--rw-r--r--   0     1001      127    48655 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-build/src/lib.rs
--rw-r--r--   0     1001      127     1025 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-cache/Cargo.toml
--rw-r--r--   0     1001      127      509 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-cache/src/archive.rs
--rw-r--r--   0     1001      127      195 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-cache/src/by_timestamp.rs
--rw-r--r--   0     1001      127     1768 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-cache/src/cli.rs
--rw-r--r--   0     1001      127    35224 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-cache/src/lib.rs
--rw-r--r--   0     1001      127     6138 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-cache/src/removal.rs
--rw-r--r--   0     1001      127     1663 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-cache/src/timestamp.rs
--rw-r--r--   0     1001      127     2538 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-cache/src/wheel.rs
--rw-r--r--   0     1001      127     1528 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-distribution/Cargo.toml
--rw-r--r--   0     1001      127      684 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-distribution/src/archive.rs
--rw-r--r--   0     1001      127    34434 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-distribution/src/distribution_database.rs
--rw-r--r--   0     1001      127     2185 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-distribution/src/download.rs
--rw-r--r--   0     1001      127     7053 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-distribution/src/error.rs
--rw-r--r--   0     1001      127    10371 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-distribution/src/git.rs
--rw-r--r--   0     1001      127     7145 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-distribution/src/index/built_wheel_index.rs
--rw-r--r--   0     1001      127     3435 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-distribution/src/index/cached_wheel.rs
--rw-r--r--   0     1001      127      162 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-distribution/src/index/mod.rs
--rw-r--r--   0     1001      127     8729 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-distribution/src/index/registry_wheel_index.rs
--rw-r--r--   0     1001      127      965 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-distribution/src/lib.rs
--rw-r--r--   0     1001      127      600 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-distribution/src/locks.rs
--rw-r--r--   0     1001      127     1225 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-distribution/src/reporter.rs
--rw-r--r--   0     1001      127     2029 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-distribution/src/source/built_wheel_metadata.rs
--rw-r--r--   0     1001      127    60426 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-distribution/src/source/mod.rs
--rw-r--r--   0     1001      127     1998 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-distribution/src/source/revision.rs
--rw-r--r--   0     1001      127      284 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-normalize/Cargo.toml
--rw-r--r--   0     1001      127     1620 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-normalize/src/extra_name.rs
--rw-r--r--   0     1001      127     5633 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-normalize/src/lib.rs
--rw-r--r--   0     1001      127     2847 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-normalize/src/package_name.rs
--rw-r--r--   0     1001      127      322 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-version/Cargo.toml
--rw-r--r--   0     1001      127      355 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-version/src/lib.rs
--rw-r--r--   0     1001      127     2046 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/Cargo.toml
--rw-r--r--   0     1001      127        1 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/bare.rs
--rw-r--r--   0     1001      127    17958 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/candidate_selector.rs
--rw-r--r--   0     1001      127      610 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/dependency_mode.rs
--rw-r--r--   0     1001      127     1140 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/dependency_provider.rs
--rw-r--r--   0     1001      127     1378 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/editables.rs
--rw-r--r--   0     1001      127    13709 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/error.rs
--rw-r--r--   0     1001      127     2743 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/exclude_newer.rs
--rw-r--r--   0     1001      127     1551 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/exclusions.rs
--rw-r--r--   0     1001      127     8000 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/flat_index.rs
--rw-r--r--   0     1001      127     1248 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/lib.rs
--rw-r--r--   0     1001      127    54355 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/lock.rs
--rw-r--r--   0     1001      127     8769 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/manifest.rs
--rw-r--r--   0     1001      127    12444 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/marker.rs
--rw-r--r--   0     1001      127     2149 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/options.rs
--rw-r--r--   0     1001      127     1122 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/pins.rs
--rw-r--r--   0     1001      127     6368 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/preferences.rs
--rw-r--r--   0     1001      127     4046 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/prerelease_mode.rs
--rw-r--r--   0     1001      127    12211 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/pubgrub/dependencies.rs
--rw-r--r--   0     1001      127     1088 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/pubgrub/distribution.rs
--rw-r--r--   0     1001      127      541 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/pubgrub/mod.rs
--rw-r--r--   0     1001      127     7814 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/pubgrub/package.rs
--rw-r--r--   0     1001      127     5707 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/pubgrub/priority.rs
--rw-r--r--   0     1001      127    40255 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/pubgrub/report.rs
--rw-r--r--   0     1001      127     4890 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/pubgrub/specifier.rs
--rw-r--r--   0     1001      127     1163 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/python_requirement.rs
--rw-r--r--   0     1001      127     4971 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/redirect.rs
--rw-r--r--   0     1001      127    11323 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/resolution/display.rs
--rw-r--r--   0     1001      127    24644 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/resolution/graph.rs
--rw-r--r--   0     1001      127     4430 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/resolution/mod.rs
--rw-r--r--   0     1001      127     1878 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/resolution_mode.rs
--rw-r--r--   0     1001      127     8210 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/resolver/batch_prefetch.rs
--rw-r--r--   0     1001      127     1172 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/resolver/index.rs
--rw-r--r--   0     1001      127    14010 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/resolver/locals.rs
--rw-r--r--   0     1001      127    66870 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/resolver/mod.rs
--rw-r--r--   0     1001      127     8756 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/resolver/provider.rs
--rw-r--r--   0     1001      127     1673 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/resolver/reporter.rs
--rw-r--r--   0     1001      127     8952 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/resolver/urls.rs
--rw-r--r--   0     1001      127     3280 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_optional_missing.snap
--rw-r--r--   0     1001      127      437 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_required_present.snap
--rw-r--r--   0     1001      127    23582 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/version_map.rs
--rw-r--r--   0     1001      127     1752 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/src/yanks.rs
--rw-r--r--   0     1001      127    22820 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-resolver/tests/resolver.rs
--rw-r--r--   0     1001      127     1807 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/Cargo.toml
--rw-r--r--   0     1001      127      112 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/README.md
--rw-r--r--   0     1001      127     7109 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/src/base_client.rs
--rw-r--r--   0     1001      127    30512 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/src/cached_client.rs
--rw-r--r--   0     1001      127    10417 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/src/error.rs
--rw-r--r--   0     1001      127     9211 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/src/flat_index.rs
--rw-r--r--   0     1001      127    46032 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/src/html.rs
--rw-r--r--   0     1001      127    29250 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/src/httpcache/control.rs
--rw-r--r--   0     1001      127    60607 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/src/httpcache/mod.rs
--rw-r--r--   0     1001      127      648 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/src/lib.rs
--rw-r--r--   0     1001      127     5110 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/src/linehaul.rs
--rw-r--r--   0     1001      127     1228 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/src/middleware.rs
--rw-r--r--   0     1001      127    35668 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/src/registry_client.rs
--rw-r--r--   0     1001      127     4579 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/src/remote_metadata.rs
--rw-r--r--   0     1001      127    12019 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/src/rkyvutil.rs
--rw-r--r--   0     1001      127     1146 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/tests/remote_metadata.rs
--rw-r--r--   0     1001      127     8183 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-client/tests/user_agent_version.rs
--rw-r--r--   0     1001      127      456 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-warnings/Cargo.toml
--rw-r--r--   0     1001      127     1701 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv-warnings/src/lib.rs
--rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 uv-0.2.2/crates/uv/Cargo.toml
--rw-r--r--   0     1001      127     3065 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/build.rs
--rw-r--r--   0     1001      127    79497 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/cli.rs
--rw-r--r--   0     1001      127     4158 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/cache_clean.rs
--rw-r--r--   0     1001      127      213 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/cache_dir.rs
--rw-r--r--   0     1001      127     1955 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/cache_prune.rs
--rw-r--r--   0     1001      127     4868 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/mod.rs
--rw-r--r--   0     1001      127     2316 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/pip/check.rs
--rw-r--r--   0     1001      127    28437 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/pip/compile.rs
--rw-r--r--   0     1001      127     2462 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/pip/freeze.rs
--rw-r--r--   0     1001      127    15154 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/pip/install.rs
--rw-r--r--   0     1001      127     6301 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/pip/list.rs
--rw-r--r--   0     1001      127      209 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/pip/mod.rs
--rw-r--r--   0     1001      127    25146 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/pip/operations.rs
--rw-r--r--   0     1001      127     6601 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/pip/show.rs
--rw-r--r--   0     1001      127    12804 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/pip/sync.rs
--rw-r--r--   0     1001      127     7279 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/pip/uninstall.rs
--rw-r--r--   0     1001      127     5158 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/project/lock.rs
--rw-r--r--   0     1001      127     8957 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/project/mod.rs
--rw-r--r--   0     1001      127     5926 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/project/run.rs
--rw-r--r--   0     1001      127     4014 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/project/sync.rs
--rw-r--r--   0     1001      127    10251 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/reporters.rs
--rw-r--r--   0     1001      127     3965 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/self_update.rs
--rw-r--r--   0     1001      127       20 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/tool/mod.rs
--rw-r--r--   0     1001      127     4223 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/tool/run.rs
--rw-r--r--   0     1001      127    10353 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/venv.rs
--rw-r--r--   0     1001      127      570 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/commands/version.rs
--rw-r--r--   0     1001      127    11263 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/compat/mod.rs
--rw-r--r--   0     1001      127     7723 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/editables.rs
--rw-r--r--   0     1001      127     7604 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/logging.rs
--rw-r--r--   0     1001      127    24234 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/main.rs
--rw-r--r--   0     1001      127     2326 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/printer.rs
--rw-r--r--   0     1001      127    38621 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/settings.rs
--rw-r--r--   0     1001      127     2844 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/shell.rs
--rw-r--r--   0     1001      127     4816 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/src/version.rs
--rw-r--r--   0     1001      127     4437 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/tests/cache_prune.rs
--rw-r--r--   0     1001      127    21602 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/tests/common/mod.rs
--rw-r--r--   0     1001      127    27008 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/tests/lock.rs
--rw-r--r--   0     1001      127     6060 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/tests/pip_check.rs
--rw-r--r--   0     1001      127   305226 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/tests/pip_compile.rs
--rw-r--r--   0     1001      127    19016 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/tests/pip_compile_scenarios.rs
--rw-r--r--   0     1001      127     8341 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/tests/pip_freeze.rs
--rw-r--r--   0     1001      127   151838 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/tests/pip_install.rs
--rw-r--r--   0     1001      127   159299 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/tests/pip_install_scenarios.rs
--rw-r--r--   0     1001      127    18430 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/tests/pip_list.rs
--rw-r--r--   0     1001      127    13190 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/tests/pip_show.rs
--rw-r--r--   0     1001      127   162261 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/tests/pip_sync.rs
--rw-r--r--   0     1001      127    14234 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/tests/pip_uninstall.rs
--rw-r--r--   0     1001      127     1254 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/tests/self_update.rs
--rw-r--r--   0     1001      127    18144 2024-05-22 21:46:28.000000 uv-0.2.2/crates/uv/tests/venv.rs
--rw-r--r--   0     1001      127   134714 2024-05-22 21:46:28.000000 uv-0.2.2/Cargo.lock
--rw-r--r--   0        0        0     8871 1970-01-01 00:00:00.000000 uv-0.2.2/Cargo.toml
--rw-r--r--   0     1001      127     2366 2024-05-22 21:46:28.000000 uv-0.2.2/pyproject.toml
--rw-r--r--   0     1001      127     1055 2024-05-22 21:46:28.000000 uv-0.2.2/python/uv/__main__.py
--rw-r--r--   0     1001      127      806 2024-05-22 21:46:28.000000 uv-0.2.2/python/uv/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-22 21:46:28.000000 uv-0.2.2/python/uv/py.typed
--rw-r--r--   0     1001      127    31568 2024-05-22 21:46:29.000000 uv-0.2.2/README.md
--rw-r--r--   0     1001      127       29 2024-05-22 21:46:28.000000 uv-0.2.2/rust-toolchain.toml
--rw-r--r--   0     1001      127    11356 2024-05-22 21:46:28.000000 uv-0.2.2/LICENSE-APACHE
--rw-r--r--   0     1001      127     1077 2024-05-22 21:46:28.000000 uv-0.2.2/LICENSE-MIT
--rw-r--r--   0        0        0    32935 1970-01-01 00:00:00.000000 uv-0.2.2/PKG-INFO
+-rw-r--r--   0     1001      127      752 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-auth/Cargo.toml
+-rw-r--r--   0     1001      127     9542 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-auth/src/cache.rs
+-rw-r--r--   0     1001      127    11219 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-auth/src/credentials.rs
+-rw-r--r--   0     1001      127     9340 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-auth/src/keyring.rs
+-rw-r--r--   0     1001      127      992 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-auth/src/lib.rs
+-rw-r--r--   0     1001      127    45581 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-auth/src/middleware.rs
+-rw-r--r--   0     1001      127     4661 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-auth/src/realm.rs
+-rw-r--r--   0     1001      127      790 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-types/Cargo.toml
+-rw-r--r--   0     1001      127      423 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-types/src/builds.rs
+-rw-r--r--   0     1001      127      239 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-types/src/downloads.rs
+-rw-r--r--   0     1001      127     6237 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-types/src/hash.rs
+-rw-r--r--   0     1001      127      219 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-types/src/lib.rs
+-rw-r--r--   0     1001      127     1478 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-types/src/requirements.rs
+-rw-r--r--   0     1001      127     6944 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-types/src/traits.rs
+-rw-r--r--   0     1001      127     1121 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/Cargo.toml
+-rw-r--r--   0     1001      127     2527 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/annotation.rs
+-rw-r--r--   0     1001      127     1048 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/any.rs
+-rw-r--r--   0     1001      127     4667 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/buildable.rs
+-rw-r--r--   0     1001      127     6720 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/cached.rs
+-rw-r--r--   0     1001      127      280 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/diagnostic.rs
+-rw-r--r--   0     1001      127     2474 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/editable.rs
+-rw-r--r--   0     1001      127      985 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/error.rs
+-rw-r--r--   0     1001      127     7205 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/file.rs
+-rw-r--r--   0     1001      127     2831 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/hash.rs
+-rw-r--r--   0     1001      127     3845 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/id.rs
+-rw-r--r--   0     1001      127    14472 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/index_url.rs
+-rw-r--r--   0     1001      127    12906 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/installed.rs
+-rw-r--r--   0     1001      127    35900 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/lib.rs
+-rw-r--r--   0     1001      127    20983 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/prioritized_distribution.rs
+-rw-r--r--   0     1001      127     8297 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/requirement.rs
+-rw-r--r--   0     1001      127     1228 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/requirements.rs
+-rw-r--r--   0     1001      127     8062 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/resolution.rs
+-rw-r--r--   0     1001      127     7176 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/resolved.rs
+-rw-r--r--   0     1001      127     3015 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/specified_requirement.rs
+-rw-r--r--   0     1001      127     8193 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/traits.rs
+-rw-r--r--   0     1001      127      507 2024-05-24 18:20:15.000000 uv-0.2.3/crates/cache-key/Cargo.toml
+-rw-r--r--   0     1001      127     8335 2024-05-24 18:20:15.000000 uv-0.2.3/crates/cache-key/src/cache_key.rs
+-rw-r--r--   0     1001      127    12317 2024-05-24 18:20:15.000000 uv-0.2.3/crates/cache-key/src/canonical_url.rs
+-rw-r--r--   0     1001      127      620 2024-05-24 18:20:15.000000 uv-0.2.3/crates/cache-key/src/digest.rs
+-rw-r--r--   0     1001      127      191 2024-05-24 18:20:15.000000 uv-0.2.3/crates/cache-key/src/lib.rs
+-rw-r--r--   0     1001      127     1986 2024-05-24 18:20:15.000000 uv-0.2.3/crates/cache-key/src/stable_hash.rs
+-rw-r--r--   0     1001      127     1004 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep440-rs/Cargo.toml
+-rw-r--r--   0     1001      127    10173 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep440-rs/License-Apache
+-rw-r--r--   0     1001      127     1293 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep440-rs/License-BSD
+-rw-r--r--   0     1001      127     2947 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep440-rs/Readme.md
+-rw-r--r--   0     1001      127     2105 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep440-rs/python/Readme.md
+-rw-r--r--   0     1001      127     2922 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep440-rs/src/lib.rs
+-rw-r--r--   0     1001      127   131052 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep440-rs/src/version.rs
+-rw-r--r--   0     1001      127    56892 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep440-rs/src/version_specifier.rs
+-rw-r--r--   0     1001      127      918 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/Cargo.toml
+-rw-r--r--   0     1001      127    63247 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/src/git.rs
+-rw-r--r--   0     1001      127    37494 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/src/known_hosts.rs
+-rw-r--r--   0     1001      127     3843 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/src/lib.rs
+-rw-r--r--   0     1001      127      940 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/src/sha.rs
+-rw-r--r--   0     1001      127     5058 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/src/source.rs
+-rw-r--r--   0     1001      127     1362 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/src/util/errors.rs
+-rw-r--r--   0     1001      127      733 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/src/util/mod.rs
+-rw-r--r--   0     1001      127     7295 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/src/util/retry.rs
+-rw-r--r--   0     1001      127      456 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-warnings/Cargo.toml
+-rw-r--r--   0     1001      127     1701 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-warnings/src/lib.rs
+-rw-r--r--   0     1001      127      911 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-fs/Cargo.toml
+-rw-r--r--   0     1001      127     1397 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-fs/src/cachedir.rs
+-rw-r--r--   0     1001      127    11137 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-fs/src/lib.rs
+-rw-r--r--   0     1001      127    12687 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-fs/src/path.rs
+-rw-r--r--   0     1001      127     1002 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-workspace/Cargo.toml
+-rw-r--r--   0     1001      127     7241 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-workspace/src/combine.rs
+-rw-r--r--   0     1001      127      127 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-workspace/src/lib.rs
+-rw-r--r--   0     1001      127     3296 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-workspace/src/settings.rs
+-rw-r--r--   0     1001      127     5560 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-workspace/src/workspace.rs
+-rw-r--r--   0     1001      127     1224 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/Cargo.toml
+-rw-r--r--   0     1001      127    87285 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/lib.rs
+-rw-r--r--   0     1001      127     2038 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/requirement.rs
+-rw-r--r--   0     1001      127     6200 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-basic.txt.snap
+-rw-r--r--   0     1001      127     2683 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-a.txt.snap
+-rw-r--r--   0     1001      127     2273 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-b.txt.snap
+-rw-r--r--   0     1001      127      284 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-empty.txt.snap
+-rw-r--r--   0     1001      127     4140 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-for-poetry.txt.snap
+-rw-r--r--   0     1001      127     1816 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-a.txt.snap
+-rw-r--r--   0     1001      127      828 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-b.txt.snap
+-rw-r--r--   0     1001      127    11863 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-poetry-with-hashes.txt.snap
+-rw-r--r--   0     1001      127     2257 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-small.txt.snap
+-rw-r--r--   0     1001      127     3818 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-whitespace.txt.snap
+-rw-r--r--   0     1001      127     6200 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-basic.txt.snap
+-rw-r--r--   0     1001      127     2683 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-a.txt.snap
+-rw-r--r--   0     1001      127     2273 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-b.txt.snap
+-rw-r--r--   0     1001      127      284 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-empty.txt.snap
+-rw-r--r--   0     1001      127     4140 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-for-poetry.txt.snap
+-rw-r--r--   0     1001      127     1816 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-a.txt.snap
+-rw-r--r--   0     1001      127      828 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-b.txt.snap
+-rw-r--r--   0     1001      127    11863 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-poetry-with-hashes.txt.snap
+-rw-r--r--   0     1001      127     2257 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-small.txt.snap
+-rw-r--r--   0     1001      127     6684 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-bare-url.txt.snap
+-rw-r--r--   0     1001      127     8155 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-editable.txt.snap
+-rw-r--r--   0     1001      127     3818 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-whitespace.txt.snap
+-rw-r--r--   0     1001      127     6744 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-bare-url.txt.snap
+-rw-r--r--   0     1001      127     8161 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-editable.txt.snap
+-rw-r--r--   0     1001      127      113 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/bare-url.txt
+-rw-r--r--   0     1001      127       90 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/basic.txt
+-rw-r--r--   0     1001      127       45 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/constraints-a.txt
+-rw-r--r--   0     1001      127       27 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/constraints-b.txt
+-rw-r--r--   0     1001      127      491 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/editable.txt
+-rw-r--r--   0     1001      127        0 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/empty.txt
+-rw-r--r--   0     1001      127      101 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/for-poetry.txt
+-rw-r--r--   0     1001      127       43 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/include-a.txt
+-rw-r--r--   0     1001      127        5 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/include-b.txt
+-rw-r--r--   0     1001      127     1183 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/poetry-with-hashes.txt
+-rw-r--r--   0     1001      127       66 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/small.txt
+-rw-r--r--   0     1001      127      183 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/whitespace.txt
+-rw-r--r--   0     1001      127      322 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-version/Cargo.toml
+-rw-r--r--   0     1001      127      355 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-version/src/lib.rs
+-rw-r--r--   0     1001      127     2085 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/Cargo.toml
+-rw-r--r--   0     1001      127    10173 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/License-Apache
+-rw-r--r--   0     1001      127     1293 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/License-BSD
+-rw-r--r--   0     1001      127     3039 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/Readme.md
+-rw-r--r--   0     1001      127     4301 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/src/cursor.rs
+-rw-r--r--   0     1001      127    62060 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/src/lib.rs
+-rw-r--r--   0     1001      127    94881 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/src/marker.rs
+-rw-r--r--   0     1001      127      743 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/src/origin.rs
+-rw-r--r--   0     1001      127    13353 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/src/unnamed.rs
+-rw-r--r--   0     1001      127    18647 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/src/verbatim_url.rs
+-rw-r--r--   0     1001      127     1528 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/Cargo.toml
+-rw-r--r--   0     1001      127      684 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/archive.rs
+-rw-r--r--   0     1001      127    34434 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/distribution_database.rs
+-rw-r--r--   0     1001      127     2185 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/download.rs
+-rw-r--r--   0     1001      127     6943 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/error.rs
+-rw-r--r--   0     1001      127    10363 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/git.rs
+-rw-r--r--   0     1001      127     7145 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/index/built_wheel_index.rs
+-rw-r--r--   0     1001      127     3435 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/index/cached_wheel.rs
+-rw-r--r--   0     1001      127      162 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/index/mod.rs
+-rw-r--r--   0     1001      127     8729 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/index/registry_wheel_index.rs
+-rw-r--r--   0     1001      127      965 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/lib.rs
+-rw-r--r--   0     1001      127      600 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/locks.rs
+-rw-r--r--   0     1001      127     1225 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/reporter.rs
+-rw-r--r--   0     1001      127     2029 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/source/built_wheel_metadata.rs
+-rw-r--r--   0     1001      127    60305 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/source/mod.rs
+-rw-r--r--   0     1001      127     1998 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/source/revision.rs
+-rw-r--r--   0     1001      127      897 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/Cargo.toml
+-rw-r--r--   0     1001      127     1078 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/src/error.rs
+-rw-r--r--   0     1001      127     4113 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/src/hash.rs
+-rw-r--r--   0     1001      127      112 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/src/lib.rs
+-rw-r--r--   0     1001      127     9419 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/src/stream.rs
+-rw-r--r--   0     1001      127     3565 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/src/sync.rs
+-rw-r--r--   0     1001      127     1489 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/src/tar.rs
+-rw-r--r--   0     1001      127     5685 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/src/vendor/cloneable_seekable_reader.rs
+-rw-r--r--   0     1001      127      112 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/src/vendor/mod.rs
+-rw-r--r--   0     1001      127      970 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-dispatch/Cargo.toml
+-rw-r--r--   0     1001      127    10910 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-dispatch/src/lib.rs
+-rw-r--r--   0     1001      127     1464 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/Cargo.toml
+-rw-r--r--   0     1001      127    12444 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/compile.rs
+-rw-r--r--   0     1001      127     9352 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/downloader.rs
+-rw-r--r--   0     1001      127     4349 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/editable.rs
+-rw-r--r--   0     1001      127     2833 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/installer.rs
+-rw-r--r--   0     1001      127      533 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/pip_compileall.py
+-rw-r--r--   0     1001      127    22428 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/plan.rs
+-rw-r--r--   0     1001      127     7565 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/satisfies.rs
+-rw-r--r--   0     1001      127    22962 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/site_packages.rs
+-rw-r--r--   0     1001      127      978 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/uninstall.rs
+-rw-r--r--   0     1001      127     1654 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/Cargo.toml
+-rw-r--r--   0     1001      127     2206 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/confirm.rs
+-rw-r--r--   0     1001      127      318 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/lib.rs
+-rw-r--r--   0     1001      127     9898 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/lookahead.rs
+-rw-r--r--   0     1001      127    31164 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/pyproject.rs
+-rw-r--r--   0     1001      127     6930 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/source_tree.rs
+-rw-r--r--   0     1001      127     7083 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/sources.rs
+-rw-r--r--   0     1001      127    14943 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/specification.rs
+-rw-r--r--   0     1001      127    12555 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/unnamed.rs
+-rw-r--r--   0     1001      127     1677 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/upgrade.rs
+-rw-r--r--   0     1001      127    25085 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/workspace.rs
+-rw-r--r--   0     1001      127     1025 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-cache/Cargo.toml
+-rw-r--r--   0     1001      127      509 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-cache/src/archive.rs
+-rw-r--r--   0     1001      127      195 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-cache/src/by_timestamp.rs
+-rw-r--r--   0     1001      127     1768 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-cache/src/cli.rs
+-rw-r--r--   0     1001      127    35224 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-cache/src/lib.rs
+-rw-r--r--   0     1001      127     6138 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-cache/src/removal.rs
+-rw-r--r--   0     1001      127     1663 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-cache/src/timestamp.rs
+-rw-r--r--   0     1001      127     2538 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-cache/src/wheel.rs
+-rw-r--r--   0     1001      127     1808 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/Cargo.toml
+-rwxr-xr-x   0     1001      127     7922 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/fetch-version-metadata.py
+-rw-r--r--   0     1001      127        0 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/__init__.py
+-rw-r--r--   0     1001      127    21931 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/get_interpreter_info.py
+-rw-r--r--   0     1001      127    10174 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/packaging/LICENSE.APACHE
+-rw-r--r--   0     1001      127     1344 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/packaging/LICENSE.BSD
+-rw-r--r--   0     1001      127      316 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/packaging/README.md
+-rw-r--r--   0     1001      127      501 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/packaging/__init__.py
+-rw-r--r--   0     1001      127     3282 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/packaging/_elffile.py
+-rw-r--r--   0     1001      127     9588 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/packaging/_manylinux.py
+-rw-r--r--   0     1001      127     2696 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/packaging/_musllinux.py
+-rw-r--r--   0     1001      127   182247 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python-version-metadata.json
+-rw-r--r--   0     1001      127    55660 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/discovery.rs
+-rw-r--r--   0     1001      127     9015 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/environment.rs
+-rw-r--r--   0     1001      127     1981 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/implementation.rs
+-rw-r--r--   0     1001      127    28174 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/interpreter.rs
+-rw-r--r--   0     1001      127    77357 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/lib.rs
+-rw-r--r--   0     1001      127     8104 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/managed/downloads.rs
+-rw-r--r--   0     1001      127     5960 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/managed/find.rs
+-rw-r--r--   0     1001      127      253 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/managed/mod.rs
+-rw-r--r--   0     1001      127   224411 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/managed/python_versions.inc
+-rw-r--r--   0     1001      127      691 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/managed/python_versions.inc.mustache
+-rw-r--r--   0     1001      127     4389 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/platform.rs
+-rw-r--r--   0     1001      127      430 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/pointer_size.rs
+-rw-r--r--   0     1001      127     3234 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/py_launcher.rs
+-rw-r--r--   0     1001      127     7736 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/python_version.rs
+-rw-r--r--   0     1001      127      950 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/target.rs
+-rw-r--r--   0     1001      127     5589 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/virtualenv.rs
+-rw-r--r--   0     1001      127     2708 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/template-version-metadata.py
+-rw-r--r--   0     1001      127      411 2024-05-24 18:20:15.000000 uv-0.2.3/crates/once-map/Cargo.toml
+-rw-r--r--   0     1001      127     3940 2024-05-24 18:20:15.000000 uv-0.2.3/crates/once-map/src/lib.rs
+-rw-r--r--   0     1001      127      858 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/Cargo.toml
+-rw-r--r--   0     1001      127     1014 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/authentication.rs
+-rw-r--r--   0     1001      127    10763 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/build_options.rs
+-rw-r--r--   0     1001      127     1054 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/concurrency.rs
+-rw-r--r--   0     1001      127     9239 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/config_settings.rs
+-rw-r--r--   0     1001      127     1698 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/constraints.rs
+-rw-r--r--   0     1001      127      437 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/lib.rs
+-rw-r--r--   0     1001      127     4059 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/name_specifiers.rs
+-rw-r--r--   0     1001      127     1703 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/overrides.rs
+-rw-r--r--   0     1001      127     2339 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/package_options.rs
+-rw-r--r--   0     1001      127      782 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/preview.rs
+-rw-r--r--   0     1001      127    11893 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/target_triple.rs
+-rw-r--r--   0     1001      127     2046 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/Cargo.toml
+-rw-r--r--   0     1001      127        1 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/bare.rs
+-rw-r--r--   0     1001      127    17958 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/candidate_selector.rs
+-rw-r--r--   0     1001      127      610 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/dependency_mode.rs
+-rw-r--r--   0     1001      127     1140 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/dependency_provider.rs
+-rw-r--r--   0     1001      127     1378 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/editables.rs
+-rw-r--r--   0     1001      127    13502 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/error.rs
+-rw-r--r--   0     1001      127     2743 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/exclude_newer.rs
+-rw-r--r--   0     1001      127     1551 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/exclusions.rs
+-rw-r--r--   0     1001      127     8107 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/flat_index.rs
+-rw-r--r--   0     1001      127     1248 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/lib.rs
+-rw-r--r--   0     1001      127    54353 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/lock.rs
+-rw-r--r--   0     1001      127     8769 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/manifest.rs
+-rw-r--r--   0     1001      127    12444 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/marker.rs
+-rw-r--r--   0     1001      127     2149 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/options.rs
+-rw-r--r--   0     1001      127     1122 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/pins.rs
+-rw-r--r--   0     1001      127     6069 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/preferences.rs
+-rw-r--r--   0     1001      127     4046 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/prerelease_mode.rs
+-rw-r--r--   0     1001      127    12211 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/pubgrub/dependencies.rs
+-rw-r--r--   0     1001      127     1104 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/pubgrub/distribution.rs
+-rw-r--r--   0     1001      127      541 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/pubgrub/mod.rs
+-rw-r--r--   0     1001      127     7806 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/pubgrub/package.rs
+-rw-r--r--   0     1001      127     5707 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/pubgrub/priority.rs
+-rw-r--r--   0     1001      127    40255 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/pubgrub/report.rs
+-rw-r--r--   0     1001      127     4890 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/pubgrub/specifier.rs
+-rw-r--r--   0     1001      127     1163 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/python_requirement.rs
+-rw-r--r--   0     1001      127     4963 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/redirect.rs
+-rw-r--r--   0     1001      127    11323 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolution/display.rs
+-rw-r--r--   0     1001      127    24704 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolution/graph.rs
+-rw-r--r--   0     1001      127     4643 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolution/mod.rs
+-rw-r--r--   0     1001      127     1878 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolution_mode.rs
+-rw-r--r--   0     1001      127     8210 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolver/batch_prefetch.rs
+-rw-r--r--   0     1001      127     1172 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolver/index.rs
+-rw-r--r--   0     1001      127    14028 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolver/locals.rs
+-rw-r--r--   0     1001      127    66822 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolver/mod.rs
+-rw-r--r--   0     1001      127     8756 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolver/provider.rs
+-rw-r--r--   0     1001      127     1673 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolver/reporter.rs
+-rw-r--r--   0     1001      127     8959 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolver/urls.rs
+-rw-r--r--   0     1001      127     3325 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_optional_missing.snap
+-rw-r--r--   0     1001      127      437 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_required_present.snap
+-rw-r--r--   0     1001      127    23688 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/version_map.rs
+-rw-r--r--   0     1001      127     1752 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/yanks.rs
+-rw-r--r--   0     1001      127    22281 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/tests/resolver.rs
+-rw-r--r--   0     1001      127      774 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/Cargo.toml
+-rw-r--r--   0     1001      127      109 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/README.md
+-rw-r--r--   0     1001      127     4375 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/_virtualenv.py
+-rw-r--r--   0     1001      127       20 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/.gitattributes
+-rw-r--r--   0     1001      127     3388 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/activate
+-rw-r--r--   0     1001      127     2259 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/activate.bat
+-rw-r--r--   0     1001      127     2655 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/activate.csh
+-rw-r--r--   0     1001      127     4219 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/activate.fish
+-rw-r--r--   0     1001      127     3903 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/activate.nu
+-rw-r--r--   0     1001      127     2826 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/activate.ps1
+-rw-r--r--   0     1001      127     2411 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/activate_this.py
+-rw-r--r--   0     1001      127     1728 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/deactivate.bat
+-rw-r--r--   0     1001      127     1215 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/pydoc.bat
+-rw-r--r--   0     1001      127    16565 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/bare.rs
+-rw-r--r--   0     1001      127     2090 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/lib.rs
+-rw-r--r--   0     1001      127     1179 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-build/Cargo.toml
+-rw-r--r--   0     1001      127       17 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-build/.gitignore
+-rw-r--r--   0     1001      127    48369 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-build/src/lib.rs
+-rw-r--r--   0     1001      127     1807 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/Cargo.toml
+-rw-r--r--   0     1001      127      112 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/README.md
+-rw-r--r--   0     1001      127     7109 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/base_client.rs
+-rw-r--r--   0     1001      127    30512 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/cached_client.rs
+-rw-r--r--   0     1001      127    10417 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/error.rs
+-rw-r--r--   0     1001      127     9211 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/flat_index.rs
+-rw-r--r--   0     1001      127    46032 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/html.rs
+-rw-r--r--   0     1001      127    29250 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/httpcache/control.rs
+-rw-r--r--   0     1001      127    60607 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/httpcache/mod.rs
+-rw-r--r--   0     1001      127      648 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/lib.rs
+-rw-r--r--   0     1001      127     5110 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/linehaul.rs
+-rw-r--r--   0     1001      127     1228 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/middleware.rs
+-rw-r--r--   0     1001      127    35668 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/registry_client.rs
+-rw-r--r--   0     1001      127     4579 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/remote_metadata.rs
+-rw-r--r--   0     1001      127    12019 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/rkyvutil.rs
+-rw-r--r--   0     1001      127     1146 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/tests/remote_metadata.rs
+-rw-r--r--   0     1001      127     8183 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/tests/user_agent_version.rs
+-rw-r--r--   0     1001      127      608 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-filename/Cargo.toml
+-rw-r--r--   0     1001      127     1842 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-filename/src/build_tag.rs
+-rw-r--r--   0     1001      127     2352 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-filename/src/lib.rs
+-rw-r--r--   0     1001      127      532 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_build_tag.snap
+-rw-r--r--   0     1001      127      564 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_multiple_tags.snap
+-rw-r--r--   0     1001      127      423 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_single_tags.snap
+-rw-r--r--   0     1001      127     7565 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-filename/src/source_dist.rs
+-rw-r--r--   0     1001      127    11807 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-filename/src/wheel.rs
+-rw-r--r--   0     1001      127      472 2024-05-24 18:20:15.000000 uv-0.2.3/crates/platform-tags/Cargo.toml
+-rw-r--r--   0     1001      127      161 2024-05-24 18:20:15.000000 uv-0.2.3/crates/platform-tags/src/lib.rs
+-rw-r--r--   0     1001      127     3507 2024-05-24 18:20:15.000000 uv-0.2.3/crates/platform-tags/src/platform.rs
+-rw-r--r--   0     1001      127    76059 2024-05-24 18:20:15.000000 uv-0.2.3/crates/platform-tags/src/tags.rs
+-rw-r--r--   0     1001      127      284 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-normalize/Cargo.toml
+-rw-r--r--   0     1001      127     1620 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-normalize/src/extra_name.rs
+-rw-r--r--   0     1001      127     5633 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-normalize/src/lib.rs
+-rw-r--r--   0     1001      127     2847 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-normalize/src/package_name.rs
+-rw-r--r--   0     1001      127      910 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/Cargo.toml
+-rw-r--r--   0     1001      127     1609 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/src/base_url.rs
+-rw-r--r--   0     1001      127     4643 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/src/direct_url.rs
+-rw-r--r--   0     1001      127    15762 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/src/lenient_requirement.rs
+-rw-r--r--   0     1001      127      278 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/src/lib.rs
+-rw-r--r--   0     1001      127    19633 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/src/metadata.rs
+-rw-r--r--   0     1001      127    13865 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/src/parsed_url.rs
+-rw-r--r--   0     1001      127      575 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/src/scheme.rs
+-rw-r--r--   0     1001      127    12178 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/src/simple_json.rs
+-rw-r--r--   0     1001      127     1504 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/Cargo.toml
+-rw-r--r--   0     1001      127      515 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/Readme.md
+-rw-r--r--   0     1001      127     4332 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/src/lib.rs
+-rw-r--r--   0     1001      127    20181 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/src/linker.rs
+-rw-r--r--   0     1001      127     7104 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/src/metadata.rs
+-rw-r--r--   0     1001      127      474 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/src/record.rs
+-rw-r--r--   0     1001      127     5550 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/src/script.rs
+-rw-r--r--   0     1001      127    11211 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/src/uninstall.rs
+-rw-r--r--   0     1001      127    34841 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/src/wheel.rs
+-rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 uv-0.2.3/crates/uv/Cargo.toml
+-rw-r--r--   0     1001      127     3065 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/build.rs
+-rw-r--r--   0     1001      127    79599 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/cli.rs
+-rw-r--r--   0     1001      127     4158 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/cache_clean.rs
+-rw-r--r--   0     1001      127      213 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/cache_dir.rs
+-rw-r--r--   0     1001      127     1955 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/cache_prune.rs
+-rw-r--r--   0     1001      127     4868 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/mod.rs
+-rw-r--r--   0     1001      127     2362 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/check.rs
+-rw-r--r--   0     1001      127    28326 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/compile.rs
+-rw-r--r--   0     1001      127     2474 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/freeze.rs
+-rw-r--r--   0     1001      127    15306 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/install.rs
+-rw-r--r--   0     1001      127     6313 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/list.rs
+-rw-r--r--   0     1001      127      209 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/mod.rs
+-rw-r--r--   0     1001      127    25086 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/operations.rs
+-rw-r--r--   0     1001      127     6615 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/show.rs
+-rw-r--r--   0     1001      127    12804 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/sync.rs
+-rw-r--r--   0     1001      127     7342 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/uninstall.rs
+-rw-r--r--   0     1001      127     5158 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/project/lock.rs
+-rw-r--r--   0     1001      127     9046 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/project/mod.rs
+-rw-r--r--   0     1001      127     5926 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/project/run.rs
+-rw-r--r--   0     1001      127     4014 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/project/sync.rs
+-rw-r--r--   0     1001      127    10251 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/reporters.rs
+-rw-r--r--   0     1001      127     3965 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/self_update.rs
+-rw-r--r--   0     1001      127       20 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/tool/mod.rs
+-rw-r--r--   0     1001      127     4290 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/tool/run.rs
+-rw-r--r--   0     1001      127    10247 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/venv.rs
+-rw-r--r--   0     1001      127      570 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/version.rs
+-rw-r--r--   0     1001      127    11263 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/compat/mod.rs
+-rw-r--r--   0     1001      127     7624 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/editables.rs
+-rw-r--r--   0     1001      127     7604 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/logging.rs
+-rw-r--r--   0     1001      127    24338 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/main.rs
+-rw-r--r--   0     1001      127     2326 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/printer.rs
+-rw-r--r--   0     1001      127    38621 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/settings.rs
+-rw-r--r--   0     1001      127     2844 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/shell.rs
+-rw-r--r--   0     1001      127     4816 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/version.rs
+-rw-r--r--   0     1001      127     4437 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/cache_prune.rs
+-rw-r--r--   0     1001      127    21781 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/common/mod.rs
+-rw-r--r--   0     1001      127    27008 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/lock.rs
+-rw-r--r--   0     1001      127     6060 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_check.rs
+-rw-r--r--   0     1001      127   307159 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_compile.rs
+-rw-r--r--   0     1001      127    19016 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_compile_scenarios.rs
+-rw-r--r--   0     1001      127     8341 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_freeze.rs
+-rw-r--r--   0     1001      127   151842 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_install.rs
+-rw-r--r--   0     1001      127   159299 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_install_scenarios.rs
+-rw-r--r--   0     1001      127    18430 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_list.rs
+-rw-r--r--   0     1001      127    13190 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_show.rs
+-rw-r--r--   0     1001      127   161999 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_sync.rs
+-rw-r--r--   0     1001      127    14235 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_uninstall.rs
+-rw-r--r--   0     1001      127     1254 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/self_update.rs
+-rw-r--r--   0     1001      127    18144 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/venv.rs
+-rw-r--r--   0     1001      127   133939 2024-05-24 18:20:15.000000 uv-0.2.3/Cargo.lock
+-rw-r--r--   0        0        0     8834 1970-01-01 00:00:00.000000 uv-0.2.3/Cargo.toml
+-rw-r--r--   0     1001      127     2366 2024-05-24 18:20:15.000000 uv-0.2.3/pyproject.toml
+-rw-r--r--   0     1001      127     1055 2024-05-24 18:20:15.000000 uv-0.2.3/python/uv/__main__.py
+-rw-r--r--   0     1001      127      806 2024-05-24 18:20:15.000000 uv-0.2.3/python/uv/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-24 18:20:15.000000 uv-0.2.3/python/uv/py.typed
+-rw-r--r--   0     1001      127    31568 2024-05-24 18:20:16.000000 uv-0.2.3/README.md
+-rw-r--r--   0     1001      127       29 2024-05-24 18:20:15.000000 uv-0.2.3/rust-toolchain.toml
+-rw-r--r--   0     1001      127    11356 2024-05-24 18:20:15.000000 uv-0.2.3/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1077 2024-05-24 18:20:15.000000 uv-0.2.3/LICENSE-MIT
+-rw-r--r--   0        0        0    32935 1970-01-01 00:00:00.000000 uv-0.2.3/PKG-INFO
```

### Comparing `uv-0.2.2/crates/uv-extract/Cargo.toml` & `uv-0.2.3/crates/uv-extract/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-extract/src/error.rs` & `uv-0.2.3/crates/uv-extract/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-extract/src/hash.rs` & `uv-0.2.3/crates/uv-extract/src/hash.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-extract/src/stream.rs` & `uv-0.2.3/crates/uv-extract/src/stream.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-extract/src/sync.rs` & `uv-0.2.3/crates/uv-extract/src/sync.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-extract/src/tar.rs` & `uv-0.2.3/crates/uv-extract/src/tar.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-extract/src/vendor/cloneable_seekable_reader.rs` & `uv-0.2.3/crates/uv-extract/src/vendor/cloneable_seekable_reader.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-types/Cargo.toml` & `uv-0.2.3/crates/uv-types/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-types/src/hash.rs` & `uv-0.2.3/crates/uv-types/src/hash.rs`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             // Every requirement must be either a pinned version or a direct URL.
             let id = match &requirement {
                 UnresolvedRequirement::Named(requirement) => {
                     uv_requirement_to_package_id(requirement)?
                 }
                 UnresolvedRequirement::Unnamed(requirement) => {
                     // Direct URLs are always allowed.
-                    PackageId::from_url(&requirement.url)
+                    PackageId::from_url(&requirement.url.verbatim)
                 }
             };
 
             // Every requirement must include a hash.
             if digests.is_empty() {
                 return Err(HashStrategyError::MissingHashes(requirement.to_string()));
             }
```

### Comparing `uv-0.2.2/crates/uv-types/src/requirements.rs` & `uv-0.2.3/crates/uv-types/src/requirements.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-types/src/traits.rs` & `uv-0.2.3/crates/uv-types/src/traits.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/install-wheel-rs/Cargo.toml` & `uv-0.2.3/crates/install-wheel-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/install-wheel-rs/Readme.md` & `uv-0.2.3/crates/install-wheel-rs/Readme.md`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/install-wheel-rs/src/lib.rs` & `uv-0.2.3/crates/install-wheel-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/install-wheel-rs/src/linker.rs` & `uv-0.2.3/crates/install-wheel-rs/src/linker.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/install-wheel-rs/src/metadata.rs` & `uv-0.2.3/crates/install-wheel-rs/src/metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/install-wheel-rs/src/script.rs` & `uv-0.2.3/crates/install-wheel-rs/src/script.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/install-wheel-rs/src/uninstall.rs` & `uv-0.2.3/crates/install-wheel-rs/src/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/install-wheel-rs/src/wheel.rs` & `uv-0.2.3/crates/install-wheel-rs/src/wheel.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/Cargo.toml` & `uv-0.2.3/crates/uv-interpreter/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/fetch-version-metadata.py` & `uv-0.2.3/crates/uv-interpreter/fetch-version-metadata.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/python/get_interpreter_info.py` & `uv-0.2.3/crates/uv-interpreter/python/get_interpreter_info.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/python/packaging/LICENSE.APACHE` & `uv-0.2.3/crates/uv-interpreter/python/packaging/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/python/packaging/LICENSE.BSD` & `uv-0.2.3/crates/uv-interpreter/python/packaging/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/python/packaging/_elffile.py` & `uv-0.2.3/crates/uv-interpreter/python/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/python/packaging/_manylinux.py` & `uv-0.2.3/crates/uv-interpreter/python/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/python/packaging/_musllinux.py` & `uv-0.2.3/crates/uv-interpreter/python/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/python-version-metadata.json` & `uv-0.2.3/crates/uv-interpreter/python-version-metadata.json`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/src/discovery.rs` & `uv-0.2.3/crates/uv-interpreter/src/discovery.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 use thiserror::Error;
 use tracing::{debug, instrument, trace};
 use uv_cache::Cache;
 use uv_fs::Simplified;
 use uv_warnings::warn_user_once;
 use which::which;
 
-use crate::implementation::ImplementationName;
+use crate::implementation::{ImplementationName, LenientImplementationName};
 use crate::interpreter::Error as InterpreterError;
 use crate::managed::toolchains_for_current_platform;
 use crate::py_launcher::py_list_paths;
 use crate::virtualenv::{
     conda_prefix_from_env, virtualenv_from_env, virtualenv_from_working_dir,
     virtualenv_python_executable,
 };
@@ -22,16 +22,19 @@
 use std::num::ParseIntError;
 use std::{env, io};
 use std::{path::Path, path::PathBuf, str::FromStr};
 
 /// A request to find a Python interpreter.
 ///
 /// See [`InterpreterRequest::from_str`].
-#[derive(Debug, Clone, PartialEq, Eq)]
+#[derive(Debug, Clone, PartialEq, Eq, Default)]
 pub enum InterpreterRequest {
+    /// Use any discovered Python interpreter
+    #[default]
+    Any,
     /// A Python version without an implementation name e.g. `3.10`
     Version(VersionRequest),
     /// A path to a directory containing a Python installation, e.g. `.venv`
     Directory(PathBuf),
     /// A path to a Python executable e.g. `~/bin/python`
     File(PathBuf),
     /// The name of a Python executable (i.e. for lookup in the PATH) e.g. `foopython3`
@@ -56,15 +59,15 @@
     Custom(HashSet<InterpreterSource>),
 }
 
 /// A Python interpreter version request.
 #[derive(Copy, Clone, Debug, Default, PartialEq, Eq)]
 pub enum VersionRequest {
     #[default]
-    Default,
+    Any,
     Major(u8),
     MajorMinor(u8, u8),
     MajorMinorPatch(u8, u8, u8),
 }
 
 /// The policy for discovery of "system" Python interpreters.
 #[derive(Debug, Clone, Copy, PartialEq, Eq, Default)]
@@ -293,15 +296,15 @@
     implementation: Option<&'a ImplementationName>,
 ) -> impl Iterator<Item = PathBuf> + 'a {
     // `UV_TEST_PYTHON_PATH` can be used to override `PATH` to limit Python executable availability in the test suite
     let search_path =
         env::var_os("UV_TEST_PYTHON_PATH").unwrap_or(env::var_os("PATH").unwrap_or_default());
 
     let possible_names: Vec<_> = version
-        .unwrap_or(&VersionRequest::Default)
+        .unwrap_or(&VersionRequest::Any)
         .possible_names(implementation)
         .collect();
 
     trace!(
         "Searching PATH for executables: {}",
         possible_names.join(", ")
     );
@@ -357,17 +360,17 @@
     cache: &'a Cache,
 ) -> impl Iterator<Item = Result<(InterpreterSource, Interpreter), Error>> + 'a {
     python_executables(version, implementation, sources)
         .map(|result| match result {
             Ok((source, path)) => Interpreter::query(&path, cache)
                 .map(|interpreter| (source, interpreter))
                 .inspect(|(source, interpreter)| {
-                    trace!(
-                        "Found Python interpreter {} {} at {} from {source}",
-                        interpreter.implementation_name(),
+                    debug!(
+                        "Found {} {} at `{}` ({source})",
+                        LenientImplementationName::from(interpreter.implementation_name()),
                         interpreter.python_full_version(),
                         path.display()
                     );
                 })
                 .map_err(Error::from)
                 .inspect_err(|err| trace!("{err}")),
             Err(err) => Err(err),
@@ -388,46 +391,46 @@
                         debug!(
                             "Allowing system Python interpreter at `{}`",
                             interpreter.sys_executable().display()
                         );
                         true
                     } else {
                         debug!(
-                            "Ignoring Python interpreter at `{}`: system intepreter not explicit",
+                            "Ignoring Python interpreter at `{}`: system interpreter not explicit",
                             interpreter.sys_executable().display()
                         );
                         false
                     }
                 }
                 (SystemPython::Explicit, true) => true,
                 (SystemPython::Disallowed, false) => {
                     debug!(
-                        "Ignoring Python interpreter at `{}`: system intepreter not allowed",
+                        "Ignoring Python interpreter at `{}`: system interpreter not allowed",
                         interpreter.sys_executable().display()
                     );
                     false
                 }
                 (SystemPython::Disallowed, true) => true,
                 (SystemPython::Required, true) => {
                     debug!(
-                        "Ignoring Python interpreter at `{}`: system intepreter required",
+                        "Ignoring Python interpreter at `{}`: system interpreter required",
                         interpreter.sys_executable().display()
                     );
                     false
                 }
                 (SystemPython::Required, false) => true,
             },
             // Do not drop any errors
             Err(_) => true,
         })
 }
 
 /// Check if an encountered error should stop discovery.
 ///
-/// Returns false when an error could be due to a faulty intepreter and we should continue searching for a working one.
+/// Returns false when an error could be due to a faulty interpreter and we should continue searching for a working one.
 fn should_stop_discovery(err: &Error) -> bool {
     match err {
         // When querying the interpreter fails, we will only raise errors that demonstrate that something is broken
         // If the interpreter returned a bad response, we'll continue searching for one that works
         Error::Query(err) => match err {
             InterpreterError::Encode(_)
             | InterpreterError::Io(_)
@@ -449,17 +452,17 @@
 /// the error will raised instead of attempting further candidates.
 pub fn find_interpreter(
     request: &InterpreterRequest,
     system: SystemPython,
     sources: &SourceSelector,
     cache: &Cache,
 ) -> Result<InterpreterResult, Error> {
-    debug!("Searching for interpreter that fulfills {request}");
     let result = match request {
         InterpreterRequest::File(path) => {
+            debug!("Checking for Python interpreter at {request}");
             if !sources.contains(InterpreterSource::ProvidedPath) {
                 return Err(Error::SourceNotSelected(
                     request.clone(),
                     InterpreterSource::ProvidedPath,
                 ));
             }
             if !path.try_exists()? {
@@ -469,14 +472,15 @@
             }
             DiscoveredInterpreter {
                 source: InterpreterSource::ProvidedPath,
                 interpreter: Interpreter::query(path, cache)?,
             }
         }
         InterpreterRequest::Directory(path) => {
+            debug!("Checking for Python interpreter in {request}");
             if !sources.contains(InterpreterSource::ProvidedPath) {
                 return Err(Error::SourceNotSelected(
                     request.clone(),
                     InterpreterSource::ProvidedPath,
                 ));
             }
             if !path.try_exists()? {
@@ -492,14 +496,15 @@
             }
             DiscoveredInterpreter {
                 source: InterpreterSource::ProvidedPath,
                 interpreter: Interpreter::query(executable, cache)?,
             }
         }
         InterpreterRequest::ExecutableName(name) => {
+            debug!("Searching for Python interpreter with {request}");
             if !sources.contains(InterpreterSource::SearchPath) {
                 return Err(Error::SourceNotSelected(
                     request.clone(),
                     InterpreterSource::SearchPath,
                 ));
             }
             let Some(executable) = which(name).ok() else {
@@ -509,14 +514,15 @@
             };
             DiscoveredInterpreter {
                 source: InterpreterSource::SearchPath,
                 interpreter: Interpreter::query(executable, cache)?,
             }
         }
         InterpreterRequest::Implementation(implementation) => {
+            debug!("Searching for a {request} interpreter in {sources}");
             let Some((source, interpreter)) =
                 python_interpreters(None, Some(implementation), system, sources, cache)
                     .find(|result| {
                         match result {
                             // Return the first critical error or matching interpreter
                             Err(err) => should_stop_discovery(err),
                             Ok((_source, interpreter)) => {
@@ -532,14 +538,15 @@
             };
             DiscoveredInterpreter {
                 source,
                 interpreter,
             }
         }
         InterpreterRequest::ImplementationVersion(implementation, version) => {
+            debug!("Searching for {request} in {sources}");
             let Some((source, interpreter)) =
                 python_interpreters(Some(version), Some(implementation), system, sources, cache)
                     .find(|result| {
                         match result {
                             // Return the first critical error or matching interpreter
                             Err(err) => should_stop_discovery(err),
                             Ok((_source, interpreter)) => {
@@ -561,27 +568,50 @@
                 ));
             };
             DiscoveredInterpreter {
                 source,
                 interpreter,
             }
         }
+        InterpreterRequest::Any => {
+            debug!("Searching for Python interpreter in {sources}");
+            let Some((source, interpreter)) =
+                python_interpreters(None, None, system, sources, cache)
+                    .find(|result| {
+                        match result {
+                            // Return the first critical error or interpreter
+                            Err(err) => should_stop_discovery(err),
+                            Ok(_) => true,
+                        }
+                    })
+                    .transpose()?
+            else {
+                return Ok(InterpreterResult::Err(
+                    InterpreterNotFound::NoPythonInstallation(sources.clone(), None),
+                ));
+            };
+            DiscoveredInterpreter {
+                source,
+                interpreter,
+            }
+        }
         InterpreterRequest::Version(version) => {
+            debug!("Searching for {request} in {sources}");
             let Some((source, interpreter)) =
                 python_interpreters(Some(version), None, system, sources, cache)
                     .find(|result| {
                         match result {
                             // Return the first critical error or matching interpreter
                             Err(err) => should_stop_discovery(err),
                             Ok((_source, interpreter)) => version.matches_interpreter(interpreter),
                         }
                     })
                     .transpose()?
             else {
-                let err = if matches!(version, VersionRequest::Default) {
+                let err = if matches!(version, VersionRequest::Any) {
                     InterpreterNotFound::NoPythonInstallation(sources.clone(), Some(*version))
                 } else {
                     InterpreterNotFound::NoMatchingVersion(sources.clone(), *version)
                 };
                 return Ok(InterpreterResult::Err(err));
             };
             DiscoveredInterpreter {
@@ -596,15 +626,15 @@
 
 /// Find the default Python interpreter on the system.
 ///
 /// Virtual environments are not included in discovery.
 ///
 /// See [`find_interpreter`] for more details on interpreter discovery.
 pub fn find_default_interpreter(cache: &Cache) -> Result<InterpreterResult, Error> {
-    let request = InterpreterRequest::Version(VersionRequest::Default);
+    let request = InterpreterRequest::default();
     let sources = SourceSelector::System;
 
     let result = find_interpreter(&request, SystemPython::Required, &sources, cache)?;
     if let Ok(ref found) = result {
         warn_on_unsupported_python(found.interpreter());
     }
 
@@ -617,15 +647,15 @@
 ///
 /// If a Python version is provided, we will first try to find an exact match. If
 /// that cannot be found and a patch version was requested, we will look for a match
 /// without comparing the patch version number. If that cannot be found, we fall back to
 /// the first available version.
 ///
 /// See [`find_interpreter`] for more details on interpreter discovery.
-#[instrument(skip_all, fields(?request))]
+#[instrument(skip_all, fields(request))]
 pub fn find_best_interpreter(
     request: &InterpreterRequest,
     system: SystemPython,
     cache: &Cache,
 ) -> Result<InterpreterResult, Error> {
     debug!("Starting interpreter discovery for {}", request);
 
@@ -661,15 +691,15 @@
             warn_on_unsupported_python(found.interpreter());
             return Ok(result);
         }
     }
 
     // If a Python version was requested but cannot be fulfilled, just take any version
     debug!("Looking for Python interpreter with any version");
-    let request = InterpreterRequest::Version(VersionRequest::Default);
+    let request = InterpreterRequest::Any;
     Ok(find_interpreter(
         // TODO(zanieb): Add a dedicated `Default` variant to `InterpreterRequest`
         &request, system, &sources, cache,
     )?
     .map_err(|err| {
         // Use a more general error in this case since we looked for multiple versions
         if matches!(err, InterpreterNotFound::NoMatchingVersion(..)) {
@@ -913,15 +943,15 @@
                 ".exe",
             )
         } else {
             (Cow::Borrowed("python"), Cow::Borrowed("python3"), "")
         };
 
         match self {
-            Self::Default => [Some(python3), Some(python), None, None],
+            Self::Any => [Some(python3), Some(python), None, None],
             Self::Major(major) => [
                 Some(Cow::Owned(format!("python{major}{extension}"))),
                 Some(python),
                 None,
                 None,
             ],
             Self::MajorMinor(major, minor) => [
@@ -956,15 +986,15 @@
                     (
                         Cow::Owned(format!("{name}{extension}")),
                         Cow::Owned(format!("{name}3{extension}")),
                     )
                 };
 
                 match self {
-                    Self::Default => [Some(python3), Some(python), None, None],
+                    Self::Any => [Some(python3), Some(python), None, None],
                     Self::Major(major) => [
                         Some(Cow::Owned(format!("{name}{major}{extension}"))),
                         Some(python),
                         None,
                         None,
                     ],
                     Self::MajorMinor(major, minor) => [
@@ -986,15 +1016,15 @@
             .chain(self.default_names())
             .flatten()
     }
 
     /// Check if a interpreter matches the requested Python version.
     fn matches_interpreter(self, interpreter: &Interpreter) -> bool {
         match self {
-            Self::Default => true,
+            Self::Any => true,
             Self::Major(major) => interpreter.python_major() == major,
             Self::MajorMinor(major, minor) => {
                 (interpreter.python_major(), interpreter.python_minor()) == (major, minor)
             }
             Self::MajorMinorPatch(major, minor, patch) => {
                 (
                     interpreter.python_major(),
@@ -1003,49 +1033,49 @@
                 ) == (major, minor, patch)
             }
         }
     }
 
     fn matches_version(self, version: &PythonVersion) -> bool {
         match self {
-            Self::Default => true,
+            Self::Any => true,
             Self::Major(major) => version.major() == major,
             Self::MajorMinor(major, minor) => (version.major(), version.minor()) == (major, minor),
             Self::MajorMinorPatch(major, minor, patch) => {
                 (version.major(), version.minor(), version.patch()) == (major, minor, Some(patch))
             }
         }
     }
 
     fn matches_major_minor(self, major: u8, minor: u8) -> bool {
         match self {
-            Self::Default => true,
+            Self::Any => true,
             Self::Major(self_major) => self_major == major,
             Self::MajorMinor(self_major, self_minor) => (self_major, self_minor) == (major, minor),
             Self::MajorMinorPatch(self_major, self_minor, _) => {
                 (self_major, self_minor) == (major, minor)
             }
         }
     }
 
     /// Return true if a patch version is present in the request.
     fn has_patch(self) -> bool {
         match self {
-            Self::Default => false,
+            Self::Any => false,
             Self::Major(..) => false,
             Self::MajorMinor(..) => false,
             Self::MajorMinorPatch(..) => true,
         }
     }
 
     /// Return a new `VersionRequest` without the patch version.
     #[must_use]
     fn without_patch(self) -> Self {
         match self {
-            Self::Default => Self::Default,
+            Self::Any => Self::Any,
             Self::Major(major) => Self::Major(major),
             Self::MajorMinor(major, minor) => Self::MajorMinor(major, minor),
             Self::MajorMinorPatch(major, minor, _) => Self::MajorMinor(major, minor),
         }
     }
 }
 
@@ -1078,15 +1108,15 @@
             .expect("Valid `PythonVersion`s should be valid `VersionRequest`s")
     }
 }
 
 impl fmt::Display for VersionRequest {
     fn fmt(&self, f: &mut Formatter<'_>) -> fmt::Result {
         match self {
-            Self::Default => f.write_str("default"),
+            Self::Any => f.write_str("default"),
             Self::Major(major) => write!(f, "{major}"),
             Self::MajorMinor(major, minor) => write!(f, "{major}.{minor}"),
             Self::MajorMinorPatch(major, minor, patch) => {
                 write!(f, "{major}.{minor}.{patch}")
             }
         }
     }
@@ -1157,23 +1187,24 @@
         matches!(self, SystemPython::Required)
     }
 }
 
 impl fmt::Display for InterpreterRequest {
     fn fmt(&self, f: &mut Formatter<'_>) -> fmt::Result {
         match self {
-            Self::Version(version) => write!(f, "Python @ {version}"),
-            Self::Directory(path) => write!(f, "directory {}", path.user_display()),
-            Self::File(path) => write!(f, "file {}", path.user_display()),
+            Self::Any => write!(f, "any Python"),
+            Self::Version(version) => write!(f, "Python {version}"),
+            Self::Directory(path) => write!(f, "directory `{}`", path.user_display()),
+            Self::File(path) => write!(f, "path `{}`", path.user_display()),
             Self::ExecutableName(name) => write!(f, "executable name `{name}`"),
             Self::Implementation(implementation) => {
                 write!(f, "{implementation}")
             }
             Self::ImplementationVersion(implementation, version) => {
-                write!(f, "{implementation} @ {version}")
+                write!(f, "{implementation} {version}")
             }
         }
     }
 }
 
 impl fmt::Display for InterpreterSource {
     fn fmt(&self, f: &mut Formatter<'_>) -> fmt::Result {
@@ -1189,21 +1220,21 @@
         }
     }
 }
 
 impl fmt::Display for InterpreterNotFound {
     fn fmt(&self, f: &mut Formatter<'_>) -> fmt::Result {
         match self {
-            Self::NoPythonInstallation(sources, None | Some(VersionRequest::Default)) => {
+            Self::NoPythonInstallation(sources, None | Some(VersionRequest::Any)) => {
                 write!(f, "No Python interpreters found in {sources}")
             }
             Self::NoPythonInstallation(sources, Some(version)) => {
                 write!(f, "No Python {version} interpreters found in {sources}")
             }
-            Self::NoMatchingVersion(sources, VersionRequest::Default) => {
+            Self::NoMatchingVersion(sources, VersionRequest::Any) => {
                 write!(f, "No Python interpreter found in {sources}")
             }
             Self::NoMatchingVersion(sources, version) => {
                 write!(f, "No interpreter found for Python {version} in {sources}")
             }
             Self::NoMatchingImplementation(sources, implementation) => {
                 write!(f, "No interpreter found for {implementation} in {sources}")
@@ -1221,25 +1252,19 @@
             ),
             Self::DirectoryNotFound(path) => write!(
                 f,
                 "Requested interpreter directory `{}` does not exist",
                 path.user_display()
             ),
             Self::ExecutableNotFoundInDirectory(directory, executable) => {
-                let executable = if let Ok(relative_executable) = executable.strip_prefix(directory)
-                {
-                    relative_executable.display()
-                } else {
-                    executable.user_display()
-                };
                 write!(
                     f,
                     "Interpreter directory `{}` does not contain Python executable at `{}`",
                     directory.user_display(),
-                    executable
+                    executable.user_display_from(directory)
                 )
             }
             Self::ExecutableNotFoundInSearchPath(name) => {
                 write!(f, "Requested Python executable `{name}` not found in PATH")
             }
             Self::FileNotExecutable(path) => {
                 write!(
```

### Comparing `uv-0.2.2/crates/uv-interpreter/src/environment.rs` & `uv-0.2.3/crates/uv-interpreter/src/environment.rs`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 use std::sync::Arc;
 
 use same_file::is_same_file;
 
 use uv_cache::Cache;
 use uv_fs::{LockedFile, Simplified};
 
-use crate::discovery::{InterpreterRequest, SourceSelector, SystemPython, VersionRequest};
+use crate::discovery::{InterpreterRequest, SourceSelector, SystemPython};
 use crate::virtualenv::{virtualenv_python_executable, PyVenvConfiguration};
 use crate::{
     find_default_interpreter, find_interpreter, Error, Interpreter, InterpreterSource, Target,
 };
 
 /// A Python environment, consisting of a Python [`Interpreter`] and its associated paths.
 #[derive(Debug, Clone)]
@@ -30,18 +30,21 @@
         // Detect the current Python interpreter.
         if let Some(python) = python {
             Self::from_requested_python(python, system, cache)
         } else if system.is_preferred() {
             Self::from_default_python(cache)
         } else {
             // First check for a parent intepreter
-            match Self::from_parent_interpreter(system, cache) {
-                Ok(env) => return Ok(env),
-                Err(Error::NotFound(_)) => {}
-                Err(err) => return Err(err),
+            // We gate this check to avoid an extra log message when it is not set
+            if std::env::var_os("UV_INTERNAL__PARENT_INTERPRETER").is_some() {
+                match Self::from_parent_interpreter(system, cache) {
+                    Ok(env) => return Ok(env),
+                    Err(Error::NotFound(_)) => {}
+                    Err(err) => return Err(err),
+                }
             }
 
             // Then a virtual environment
             match Self::from_virtualenv(cache) {
                 Ok(venv) => Ok(venv),
                 Err(Error::NotFound(_)) if system.is_allowed() => Self::from_default_python(cache),
                 Err(err) => Err(err),
@@ -50,15 +53,15 @@
     }
 
     /// Create a [`PythonEnvironment`] for an existing virtual environment.
     ///
     /// Allows Conda environments (via `CONDA_PREFIX`) though they are not technically virtual environments.
     pub fn from_virtualenv(cache: &Cache) -> Result<Self, Error> {
         let sources = SourceSelector::VirtualEnv;
-        let request = InterpreterRequest::Version(VersionRequest::Default);
+        let request = InterpreterRequest::Any;
         let found = find_interpreter(&request, SystemPython::Disallowed, &sources, cache)??;
 
         debug_assert!(
             found.interpreter().is_virtualenv()
                 || matches!(found.source(), InterpreterSource::CondaPrefix),
             "Not a virtualenv (source: {}, prefix: {})",
             found.source(),
@@ -70,15 +73,15 @@
             interpreter: found.into_interpreter(),
         })))
     }
 
     /// Create a [`PythonEnvironment`] for the parent interpreter i.e. the executable in `python -m uv ...`
     pub fn from_parent_interpreter(system: SystemPython, cache: &Cache) -> Result<Self, Error> {
         let sources = SourceSelector::from_sources([InterpreterSource::ParentInterpreter]);
-        let request = InterpreterRequest::Version(VersionRequest::Default);
+        let request = InterpreterRequest::Any;
         let found = find_interpreter(&request, system, &sources, cache)??;
 
         Ok(Self(Arc::new(PythonEnvironmentShared {
             root: found.interpreter().prefix().to_path_buf(),
             interpreter: found.into_interpreter(),
         })))
     }
@@ -196,26 +199,23 @@
         self.0.interpreter.scripts()
     }
 
     /// Grab a file lock for the environment to prevent concurrent writes across processes.
     pub fn lock(&self) -> Result<LockedFile, std::io::Error> {
         if let Some(target) = self.0.interpreter.target() {
             // If we're installing into a `--target`, use a target-specific lock file.
-            LockedFile::acquire(
-                target.root().join(".lock"),
-                target.root().simplified_display(),
-            )
+            LockedFile::acquire(target.root().join(".lock"), target.root().user_display())
         } else if self.0.interpreter.is_virtualenv() {
             // If the environment a virtualenv, use a virtualenv-specific lock file.
-            LockedFile::acquire(self.0.root.join(".lock"), self.0.root.simplified_display())
+            LockedFile::acquire(self.0.root.join(".lock"), self.0.root.user_display())
         } else {
             // Otherwise, use a global lock file.
             LockedFile::acquire(
                 env::temp_dir().join(format!("uv-{}.lock", cache_key::digest(&self.0.root))),
-                self.0.root.simplified_display(),
+                self.0.root.user_display(),
             )
         }
     }
 
     /// Return the [`Interpreter`] for this environment.
     ///
     /// See also [`PythonEnvironment::interpreter`].
```

### Comparing `uv-0.2.2/crates/uv-interpreter/src/interpreter.rs` & `uv-0.2.3/crates/uv-interpreter/src/interpreter.rs`

 * *Files 1% similar despite different names*

```diff
@@ -591,17 +591,21 @@
     /// Running a Python script is (relatively) expensive, and the markers won't change
     /// unless the Python executable changes, so we use the executable's last modified
     /// time as a cache key.
     pub(crate) fn query_cached(executable: &Path, cache: &Cache) -> Result<Self, Error> {
         let cache_entry = cache.entry(
             CacheBucket::Interpreter,
             "",
-            format!("{}.msgpack", digest(&executable)),
+            // We use the absolute path for the cache entry to avoid cache collisions for relative paths
+            // but we do not want to query the executable with symbolic links resolved
+            format!("{}.msgpack", digest(&uv_fs::absolutize_path(executable)?)),
         );
 
+        // We check the timestamp of the canonicalized executable to check if an underlying
+        // interpreter has been modified
         let modified = Timestamp::from_path(uv_fs::canonicalize_executable(executable)?)?;
 
         // Read from the cache.
         if cache
             .freshness(&cache_entry, None)
             .is_ok_and(Freshness::is_fresh)
         {
@@ -635,19 +639,14 @@
 
         // Otherwise, run the Python script.
         trace!(
             "Querying interpreter executable at {}",
             executable.display()
         );
         let info = Self::query(executable, cache)?;
-        trace!(
-            "Found Python {} at {}",
-            info.markers.python_full_version(),
-            executable.display()
-        );
 
         // If `executable` is a pyenv shim, a bash script that redirects to the activated
         // python executable at another path, we're not allowed to cache the interpreter info.
         if same_file::is_same_file(executable, &info.sys_executable).unwrap_or(false) {
             fs::create_dir_all(cache_entry.dir())?;
             write_atomic_sync(
                 cache_entry.path(),
```

### Comparing `uv-0.2.2/crates/uv-interpreter/src/lib.rs` & `uv-0.2.3/crates/uv-interpreter/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -582,15 +582,15 @@
                         ],
                     )?),
                 ),
                 ("PWD", Some(tempdir.path().into())),
             ],
             || {
                 let result = find_interpreter(
-                    &InterpreterRequest::Version(VersionRequest::Default),
+                    &InterpreterRequest::Any,
                     SystemPython::Allowed,
                     &SourceSelector::All,
                     &cache,
                 )
                 .unwrap()
                 .unwrap();
                 assert_eq!(
@@ -616,15 +616,15 @@
                         ],
                     )?),
                 ),
                 ("PWD", Some(tempdir.path().into())),
             ],
             || {
                 let result = find_interpreter(
-                    &InterpreterRequest::Version(VersionRequest::Default),
+                    &InterpreterRequest::Any,
                     SystemPython::Allowed,
                     &SourceSelector::All,
                     &cache,
                 )
                 .unwrap()
                 .unwrap();
                 assert_eq!(
@@ -657,15 +657,15 @@
                         ],
                     )?),
                 ),
                 ("PWD", Some(tempdir.path().into())),
             ],
             || {
                 let result = find_interpreter(
-                    &InterpreterRequest::Version(VersionRequest::Default),
+                    &InterpreterRequest::Any,
                     SystemPython::Required,
                     &SourceSelector::All,
                     &cache,
                 )
                 .unwrap()
                 .unwrap();
                 assert_eq!(
@@ -697,15 +697,15 @@
                         ],
                     )?),
                 ),
                 ("PWD", Some(tempdir.path().into())),
             ],
             || {
                 let result = find_interpreter(
-                    &InterpreterRequest::Version(VersionRequest::Default),
+                    &InterpreterRequest::Any,
                     SystemPython::Disallowed,
                     &SourceSelector::All,
                     &cache,
                 )
                 .unwrap()
                 .unwrap();
                 assert_eq!(
```

### Comparing `uv-0.2.2/crates/uv-interpreter/src/managed/downloads.rs` & `uv-0.2.3/crates/uv-interpreter/src/managed/downloads.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/src/managed/find.rs` & `uv-0.2.3/crates/uv-interpreter/src/managed/find.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/src/managed/python_versions.inc` & `uv-0.2.3/crates/uv-interpreter/src/managed/python_versions.inc`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/src/managed/python_versions.inc.mustache` & `uv-0.2.3/crates/uv-interpreter/src/managed/python_versions.inc.mustache`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/src/platform.rs` & `uv-0.2.3/crates/uv-interpreter/src/platform.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/src/py_launcher.rs` & `uv-0.2.3/crates/uv-interpreter/src/py_launcher.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/src/python_version.rs` & `uv-0.2.3/crates/uv-interpreter/src/python_version.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/src/target.rs` & `uv-0.2.3/crates/uv-interpreter/src/target.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-interpreter/src/virtualenv.rs` & `uv-0.2.3/crates/uv-interpreter/src/virtualenv.rs`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
     env, io,
     path::{Path, PathBuf},
 };
 
 use fs_err as fs;
 use pypi_types::Scheme;
 use thiserror::Error;
-use tracing::{debug, info};
 
 /// The layout of a virtual environment.
 #[derive(Debug)]
 pub struct VirtualEnvironment {
     /// The absolute path to the root of the virtualenv, e.g., `/path/to/.venv`.
     pub root: PathBuf,
 
@@ -42,33 +41,25 @@
 }
 
 /// Locate an active virtual environment by inspecting environment variables.
 ///
 /// Supports `VIRTUAL_ENV`.
 pub(crate) fn virtualenv_from_env() -> Option<PathBuf> {
     if let Some(dir) = env::var_os("VIRTUAL_ENV").filter(|value| !value.is_empty()) {
-        info!(
-            "Found active virtual environment (via VIRTUAL_ENV) at: {}",
-            Path::new(&dir).display()
-        );
         return Some(PathBuf::from(dir));
     }
 
     None
 }
 
 /// Locate an active conda environment by inspecting environment variables.
 ///
 /// Supports `CONDA_PREFIX`.
 pub(crate) fn conda_prefix_from_env() -> Option<PathBuf> {
     if let Some(dir) = env::var_os("CONDA_PREFIX").filter(|value| !value.is_empty()) {
-        info!(
-            "Found active virtual environment (via CONDA_PREFIX) at: {}",
-            Path::new(&dir).display()
-        );
         return Some(PathBuf::from(dir));
     }
 
     None
 }
 
 /// Locate a virtual environment by searching the file system.
@@ -78,25 +69,23 @@
 /// containing virtual environment is returned.
 pub(crate) fn virtualenv_from_working_dir() -> Result<Option<PathBuf>, Error> {
     let current_dir = crate::current_dir()?;
 
     for dir in current_dir.ancestors() {
         // If we're _within_ a virtualenv, return it.
         if dir.join("pyvenv.cfg").is_file() {
-            debug!("Found a virtual environment at: {}", dir.display());
             return Ok(Some(dir.to_path_buf()));
         }
 
         // Otherwise, search for a `.venv` directory.
         let dot_venv = dir.join(".venv");
         if dot_venv.is_dir() {
             if !dot_venv.join("pyvenv.cfg").is_file() {
                 return Err(Error::MissingPyVenvCfg(dot_venv));
             }
-            debug!("Found a virtual environment at: {}", dot_venv.display());
             return Ok(Some(dot_venv));
         }
     }
 
     Ok(None)
 }
 
@@ -122,16 +111,27 @@
         if executable.exists() {
             return executable;
         }
 
         // If none of these exist, return the standard location
         default_executable
     } else {
-        // Search for `python` in the `bin` directory.
-        venv.join("bin").join("python")
+        // Check for both `python3` over `python`, preferring the more specific one
+        let default_executable = venv.join("bin").join("python3");
+        if default_executable.exists() {
+            return default_executable;
+        }
+
+        let executable = venv.join("bin").join("python");
+        if executable.exists() {
+            return executable;
+        }
+
+        // If none of these exist, return the standard location
+        default_executable
     }
 }
 
 impl PyVenvConfiguration {
     /// Parse a `pyvenv.cfg` file into a [`PyVenvConfiguration`].
     pub fn parse(cfg: impl AsRef<Path>) -> Result<Self, Error> {
         let mut virtualenv = false;
```

### Comparing `uv-0.2.2/crates/uv-interpreter/template-version-metadata.py` & `uv-0.2.3/crates/uv-interpreter/template-version-metadata.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/once-map/src/lib.rs` & `uv-0.2.3/crates/once-map/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pypi-types/Cargo.toml` & `uv-0.2.3/crates/pypi-types/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,21 +12,24 @@
 [lints]
 workspace = true
 
 [dependencies]
 pep440_rs = { workspace = true }
 pep508_rs = { workspace = true }
 uv-normalize = { workspace = true }
+uv-git = { workspace = true }
 
 chrono = { workspace = true, features = ["serde"] }
+git2 = { workspace = true }
 indexmap = { workspace = true, features = ["serde"] }
 mailparse = { workspace = true }
 once_cell = { workspace = true }
 regex = { workspace = true }
 rkyv = { workspace = true }
 serde = { workspace = true }
 thiserror = { workspace = true }
 toml = { workspace = true }
 tracing = { workspace = true }
 url = { workspace = true }
 
 [dev-dependencies]
+anyhow = { workspace = true }
```

### Comparing `uv-0.2.2/crates/pypi-types/src/base_url.rs` & `uv-0.2.3/crates/pypi-types/src/base_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pypi-types/src/direct_url.rs` & `uv-0.2.3/crates/pypi-types/src/direct_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pypi-types/src/lenient_requirement.rs` & `uv-0.2.3/crates/pypi-types/src/lenient_requirement.rs`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 use once_cell::sync::Lazy;
 use regex::Regex;
 use serde::{de, Deserialize, Deserializer, Serialize};
 use tracing::warn;
 
 use pep440_rs::{VersionSpecifiers, VersionSpecifiersParseError};
-use pep508_rs::{Pep508Error, Pep508Url, Requirement, VerbatimUrl};
+use pep508_rs::{Pep508Error, Pep508Url, Requirement};
+
+use crate::VerbatimParsedUrl;
 
 /// Ex) `>=7.2.0<8.0.0`
 static MISSING_COMMA: Lazy<Regex> = Lazy::new(|| Regex::new(r"(\d)([<>=~^!])").unwrap());
 /// Ex) `!=~5.0`
 static NOT_EQUAL_TILDE: Lazy<Regex> = Lazy::new(|| Regex::new(r"!=~((?:\d\.)*\d)").unwrap());
 /// Ex) `>=1.9.*`, `<3.4.*`
 static INVALID_TRAILING_DOT_STAR: Lazy<Regex> =
@@ -110,15 +112,15 @@
             Err(err)
         }
     }
 }
 
 /// Like [`Requirement`], but attempts to correct some common errors in user-provided requirements.
 #[derive(Debug, Clone, Serialize, Deserialize, Eq, PartialEq)]
-pub struct LenientRequirement<T: Pep508Url = VerbatimUrl>(Requirement<T>);
+pub struct LenientRequirement<T: Pep508Url = VerbatimParsedUrl>(Requirement<T>);
 
 impl<T: Pep508Url> FromStr for LenientRequirement<T> {
     type Err = Pep508Error<T>;
 
     fn from_str(input: &str) -> Result<Self, Self::Err> {
         Ok(Self(parse_with_fixups(input, "requirement")?))
     }
```

### Comparing `uv-0.2.2/crates/pypi-types/src/metadata.rs` & `uv-0.2.3/crates/pypi-types/src/metadata.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 use indexmap::IndexMap;
 use mailparse::{MailHeaderMap, MailParseError};
 use serde::{Deserialize, Serialize};
 use thiserror::Error;
 use tracing::warn;
 
 use pep440_rs::{Version, VersionParseError, VersionSpecifiers, VersionSpecifiersParseError};
-use pep508_rs::{Pep508Error, Requirement, VerbatimUrl};
+use pep508_rs::{Pep508Error, Requirement};
 use uv_normalize::{ExtraName, InvalidNameError, PackageName};
 
 use crate::lenient_requirement::LenientRequirement;
-use crate::LenientVersionSpecifiers;
+use crate::{LenientVersionSpecifiers, VerbatimParsedUrl};
 
 /// Python Package Metadata 2.3 as specified in
 /// <https://packaging.python.org/specifications/core-metadata/>.
 ///
 /// This is a subset of the full metadata specification, and only includes the
 /// fields that are relevant to dependency resolution.
 ///
@@ -25,15 +25,15 @@
 #[derive(Serialize, Deserialize, Debug, Clone)]
 #[serde(rename_all = "kebab-case")]
 pub struct Metadata23 {
     // Mandatory fields
     pub name: PackageName,
     pub version: Version,
     // Optional fields
-    pub requires_dist: Vec<Requirement<VerbatimUrl>>,
+    pub requires_dist: Vec<Requirement<VerbatimParsedUrl>>,
     pub requires_python: Option<VersionSpecifiers>,
     pub provides_extras: Vec<ExtraName>,
 }
 
 /// <https://github.com/PyO3/python-pkginfo-rs/blob/d719988323a0cfea86d4737116d7917f30e819e2/src/error.rs>
 ///
 /// The error type
@@ -46,25 +46,31 @@
     #[error("metadata field {0} not found")]
     FieldNotFound(&'static str),
     #[error("invalid version: {0}")]
     Pep440VersionError(VersionParseError),
     #[error(transparent)]
     Pep440Error(#[from] VersionSpecifiersParseError),
     #[error(transparent)]
-    Pep508Error(#[from] Pep508Error<VerbatimUrl>),
+    Pep508Error(#[from] Box<Pep508Error<VerbatimParsedUrl>>),
     #[error(transparent)]
     InvalidName(#[from] InvalidNameError),
     #[error("Invalid `Metadata-Version` field: {0}")]
     InvalidMetadataVersion(String),
     #[error("Reading metadata from `PKG-INFO` requires Metadata 2.2 or later (found: {0})")]
     UnsupportedMetadataVersion(String),
     #[error("The following field was marked as dynamic: {0}")]
     DynamicField(&'static str),
 }
 
+impl From<Pep508Error<VerbatimParsedUrl>> for MetadataError {
+    fn from(error: Pep508Error<VerbatimParsedUrl>) -> Self {
+        Self::Pep508Error(Box::new(error))
+    }
+}
+
 /// From <https://github.com/PyO3/python-pkginfo-rs/blob/d719988323a0cfea86d4737116d7917f30e819e2/src/metadata.rs#LL78C2-L91C26>
 impl Metadata23 {
     /// Parse the [`Metadata23`] from a `METADATA` file, as included in a built distribution (wheel).
     pub fn parse_metadata(content: &[u8]) -> Result<Self, MetadataError> {
         let headers = Headers::parse(content)?;
 
         let name = PackageName::new(
```

### Comparing `uv-0.2.2/crates/pypi-types/src/scheme.rs` & `uv-0.2.3/crates/pypi-types/src/scheme.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pypi-types/src/simple_json.rs` & `uv-0.2.3/crates/pypi-types/src/simple_json.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-auth/Cargo.toml` & `uv-0.2.3/crates/uv-auth/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-auth/src/cache.rs` & `uv-0.2.3/crates/uv-auth/src/cache.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-auth/src/credentials.rs` & `uv-0.2.3/crates/uv-auth/src/credentials.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-auth/src/keyring.rs` & `uv-0.2.3/crates/uv-auth/src/keyring.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-auth/src/lib.rs` & `uv-0.2.3/crates/uv-auth/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-auth/src/middleware.rs` & `uv-0.2.3/crates/uv-auth/src/middleware.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-auth/src/realm.rs` & `uv-0.2.3/crates/uv-auth/src/realm.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/cache-key/src/cache_key.rs` & `uv-0.2.3/crates/cache-key/src/cache_key.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/cache-key/src/canonical_url.rs` & `uv-0.2.3/crates/cache-key/src/canonical_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/cache-key/src/digest.rs` & `uv-0.2.3/crates/cache-key/src/digest.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/cache-key/src/stable_hash.rs` & `uv-0.2.3/crates/cache-key/src/stable_hash.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/distribution-types/Cargo.toml` & `uv-0.2.3/crates/distribution-types/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 pypi-types = { workspace = true }
 uv-fs = { workspace = true }
 uv-git = { workspace = true, features = ["vendored-openssl"] }
 uv-normalize = { workspace = true }
 
 anyhow = { workspace = true }
 fs-err = { workspace = true }
-git2 = { workspace = true }
 indexmap = { workspace = true }
 itertools = { workspace = true }
 once_cell = { workspace = true }
 rkyv = { workspace = true }
 schemars = { workspace = true, optional = true }
 serde = { workspace = true, features = ["derive"] }
 serde_json = { workspace = true }
```

### Comparing `uv-0.2.2/crates/distribution-types/src/annotation.rs` & `uv-0.2.3/crates/distribution-types/src/annotation.rs`

 * *Files 12% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 }
 
 impl std::fmt::Display for SourceAnnotation {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         match self {
             Self::Requirement(origin) => match origin {
                 RequirementOrigin::File(path) => {
-                    write!(f, "-r {}", path.user_display())
+                    write!(f, "-r {}", path.portable_display())
                 }
                 RequirementOrigin::Project(path, project_name) => {
-                    write!(f, "{project_name} ({})", path.user_display())
+                    write!(f, "{project_name} ({})", path.portable_display())
                 }
             },
             Self::Constraint(origin) => {
-                write!(f, "-c {}", origin.path().user_display())
+                write!(f, "-c {}", origin.path().portable_display())
             }
             Self::Override(origin) => {
-                write!(f, "--override {}", origin.path().user_display())
+                write!(f, "--override {}", origin.path().portable_display())
             }
         }
     }
 }
 
 /// A collection of source annotations.
 #[derive(Default, Debug, Clone)]
```

### Comparing `uv-0.2.2/crates/distribution-types/src/any.rs` & `uv-0.2.3/crates/distribution-types/src/any.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/distribution-types/src/buildable.rs` & `uv-0.2.3/crates/distribution-types/src/buildable.rs`

 * *Files 2% similar despite different names*

```diff
@@ -101,31 +101,31 @@
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct GitSourceUrl<'a> {
     /// The URL with the revision and subdirectory fragment.
     pub url: &'a VerbatimUrl,
+    pub git: &'a GitUrl,
     /// The URL without the revision and subdirectory fragment.
-    pub git: Cow<'a, GitUrl>,
-    pub subdirectory: Option<Cow<'a, Path>>,
+    pub subdirectory: Option<&'a Path>,
 }
 
 impl std::fmt::Display for GitSourceUrl<'_> {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(f, "{url}", url = self.url)
     }
 }
 
 impl<'a> From<&'a GitSourceDist> for GitSourceUrl<'a> {
     fn from(dist: &'a GitSourceDist) -> Self {
         Self {
             url: &dist.url,
-            git: Cow::Borrowed(&dist.git),
-            subdirectory: dist.subdirectory.as_deref().map(Cow::Borrowed),
+            git: &dist.git,
+            subdirectory: dist.subdirectory.as_deref(),
         }
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct PathSourceUrl<'a> {
     pub url: &'a Url,
```

### Comparing `uv-0.2.2/crates/distribution-types/src/cached.rs` & `uv-0.2.3/crates/distribution-types/src/cached.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 use std::path::{Path, PathBuf};
 
 use anyhow::{anyhow, Result};
 
 use distribution_filename::WheelFilename;
 use pep508_rs::VerbatimUrl;
-use pypi_types::HashDigest;
+use pypi_types::{HashDigest, ParsedPathUrl};
 use uv_normalize::PackageName;
 
 use crate::{
     BuiltDist, Dist, DistributionMetadata, Hashed, InstalledMetadata, InstalledVersion, Name,
-    ParsedPathUrl, ParsedUrl, SourceDist, VersionOrUrlRef,
+    ParsedUrl, SourceDist, VersionOrUrlRef,
 };
 
 /// A built distribution (wheel) that exists in the local cache.
 #[derive(Debug, Clone)]
 pub enum CachedDist {
     /// The distribution exists in a registry, like `PyPI`.
     Registry(CachedRegistryDist),
```

### Comparing `uv-0.2.2/crates/distribution-types/src/editable.rs` & `uv-0.2.3/crates/distribution-types/src/editable.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/distribution-types/src/error.rs` & `uv-0.2.3/crates/distribution-types/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/distribution-types/src/file.rs` & `uv-0.2.3/crates/distribution-types/src/file.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/distribution-types/src/hash.rs` & `uv-0.2.3/crates/distribution-types/src/hash.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/distribution-types/src/id.rs` & `uv-0.2.3/crates/distribution-types/src/id.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/distribution-types/src/index_url.rs` & `uv-0.2.3/crates/distribution-types/src/index_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/distribution-types/src/installed.rs` & `uv-0.2.3/crates/distribution-types/src/installed.rs`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,24 @@
         match self {
             Self::Registry(_) => None,
             Self::Url(dist) => dist.editable.then_some(&dist.url),
             Self::EggInfo(_) => None,
             Self::LegacyEditable(dist) => Some(&dist.target_url),
         }
     }
+
+    /// Return true if the distribution refers to a local file or directory.
+    pub fn is_local(&self) -> bool {
+        match self {
+            Self::Registry(_) => false,
+            Self::Url(dist) => matches!(&*dist.direct_url, DirectUrl::LocalDirectory { .. }),
+            Self::EggInfo(_) => false,
+            Self::LegacyEditable(_) => true,
+        }
+    }
 }
 
 impl DistributionMetadata for InstalledDist {
     fn version_or_url(&self) -> VersionOrUrlRef {
         VersionOrUrlRef::Version(self.version())
     }
 }
```

### Comparing `uv-0.2.2/crates/distribution-types/src/lib.rs` & `uv-0.2.3/crates/distribution-types/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -38,48 +38,49 @@
 
 use anyhow::Result;
 use url::Url;
 
 use distribution_filename::WheelFilename;
 use pep440_rs::Version;
 use pep508_rs::{Pep508Url, VerbatimUrl};
+use pypi_types::{ParsedUrl, VerbatimParsedUrl};
 use uv_git::GitUrl;
 use uv_normalize::PackageName;
 
 pub use crate::annotation::*;
 pub use crate::any::*;
 pub use crate::buildable::*;
 pub use crate::cached::*;
+pub use crate::diagnostic::*;
 pub use crate::editable::*;
 pub use crate::error::*;
 pub use crate::file::*;
 pub use crate::hash::*;
 pub use crate::id::*;
 pub use crate::index_url::*;
 pub use crate::installed::*;
-pub use crate::parsed_url::*;
 pub use crate::prioritized_distribution::*;
 pub use crate::requirement::*;
 pub use crate::resolution::*;
 pub use crate::resolved::*;
 pub use crate::specified_requirement::*;
 pub use crate::traits::*;
 
 mod annotation;
 mod any;
 mod buildable;
 mod cached;
+mod diagnostic;
 mod editable;
 mod error;
 mod file;
 mod hash;
 mod id;
 mod index_url;
 mod installed;
-mod parsed_url;
 mod prioritized_distribution;
 mod requirement;
 mod resolution;
 mod resolved;
 mod specified_requirement;
 mod traits;
 
@@ -422,14 +423,22 @@
     pub fn is_editable(&self) -> bool {
         match self {
             Self::Source(dist) => dist.is_editable(),
             Self::Built(_) => false,
         }
     }
 
+    /// Return true if the distribution refers to a local file or directory.
+    pub fn is_local(&self) -> bool {
+        match self {
+            Self::Source(dist) => dist.is_local(),
+            Self::Built(dist) => dist.is_local(),
+        }
+    }
+
     /// Returns the [`IndexUrl`], if the distribution is from a registry.
     pub fn index(&self) -> Option<&IndexUrl> {
         match self {
             Self::Built(dist) => dist.index(),
             Self::Source(dist) => dist.index(),
         }
     }
@@ -447,14 +456,19 @@
             Self::Built(wheel) => Some(wheel.version()),
             Self::Source(source_dist) => source_dist.version(),
         }
     }
 }
 
 impl BuiltDist {
+    /// Return true if the distribution refers to a local file or directory.
+    pub fn is_local(&self) -> bool {
+        matches!(self, Self::Path(_))
+    }
+
     /// Returns the [`IndexUrl`], if the distribution is from a registry.
     pub fn index(&self) -> Option<&IndexUrl> {
         match self {
             Self::Registry(registry) => Some(&registry.best_wheel().index),
             Self::DirectUrl(_) => None,
             Self::Path(_) => None,
         }
@@ -505,14 +519,19 @@
     pub fn is_editable(&self) -> bool {
         match self {
             Self::Directory(DirectorySourceDist { editable, .. }) => *editable,
             _ => false,
         }
     }
 
+    /// Return true if the distribution refers to a local file or directory.
+    pub fn is_local(&self) -> bool {
+        matches!(self, Self::Directory(_) | Self::Path(_))
+    }
+
     /// Returns the path to the source distribution, if it's a local distribution.
     pub fn as_path(&self) -> Option<&Path> {
         match self {
             Self::Path(dist) => Some(&dist.path),
             Self::Directory(dist) => Some(&dist.path),
             _ => None,
         }
```

### Comparing `uv-0.2.2/crates/distribution-types/src/parsed_url.rs` & `uv-0.2.3/crates/pypi-types/src/parsed_url.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,141 @@
-use std::path::PathBuf;
+use std::fmt::{Display, Formatter};
+use std::path::{Path, PathBuf};
 
-use anyhow::{Error, Result};
 use thiserror::Error;
-use url::Url;
+use url::{ParseError, Url};
 
-use pep508_rs::VerbatimUrl;
+use pep508_rs::{Pep508Url, UnnamedRequirementUrl, VerbatimUrl, VerbatimUrlError};
 use uv_git::{GitSha, GitUrl};
 
+use crate::{ArchiveInfo, DirInfo, DirectUrl, VcsInfo, VcsKind};
+
 #[derive(Debug, Error)]
 pub enum ParsedUrlError {
     #[error("Unsupported URL prefix `{prefix}` in URL: `{url}` ({message})")]
     UnsupportedUrlPrefix {
         prefix: String,
         url: Url,
         message: &'static str,
     },
     #[error("Invalid path in file URL: `{0}`")]
     InvalidFileUrl(Url),
     #[error("Failed to parse Git reference from URL: `{0}`")]
     GitShaParse(Url, #[source] git2::Error),
     #[error("Not a valid URL: `{0}`")]
-    UrlParse(String, #[source] url::ParseError),
+    UrlParse(String, #[source] ParseError),
+    #[error(transparent)]
+    VerbatimUrl(#[from] VerbatimUrlError),
 }
 
 #[derive(Debug, Clone, Hash, PartialEq, PartialOrd, Eq, Ord)]
 pub struct VerbatimParsedUrl {
     pub parsed_url: ParsedUrl,
     pub verbatim: VerbatimUrl,
 }
 
+impl Pep508Url for VerbatimParsedUrl {
+    type Err = ParsedUrlError;
+
+    fn parse_url(url: &str, working_dir: Option<&Path>) -> Result<Self, Self::Err> {
+        let verbatim_url = <VerbatimUrl as Pep508Url>::parse_url(url, working_dir)?;
+        Ok(Self {
+            parsed_url: ParsedUrl::try_from(verbatim_url.to_url())?,
+            verbatim: verbatim_url,
+        })
+    }
+}
+
+impl UnnamedRequirementUrl for VerbatimParsedUrl {
+    fn parse_path(
+        path: impl AsRef<Path>,
+        working_dir: impl AsRef<Path>,
+    ) -> Result<Self, Self::Err> {
+        let verbatim = VerbatimUrl::parse_path(&path, &working_dir)?;
+        let parsed_path_url = ParsedPathUrl {
+            url: verbatim.to_url(),
+            path: working_dir.as_ref().join(path),
+            editable: false,
+        };
+        Ok(Self {
+            parsed_url: ParsedUrl::Path(parsed_path_url),
+            verbatim,
+        })
+    }
+
+    fn parse_absolute_path(path: impl AsRef<Path>) -> Result<Self, Self::Err> {
+        let verbatim = VerbatimUrl::parse_absolute_path(&path)?;
+        let parsed_path_url = ParsedPathUrl {
+            url: verbatim.to_url(),
+            path: path.as_ref().to_path_buf(),
+            editable: false,
+        };
+        Ok(Self {
+            parsed_url: ParsedUrl::Path(parsed_path_url),
+            verbatim,
+        })
+    }
+
+    fn parse_unnamed_url(url: impl AsRef<str>) -> Result<Self, Self::Err> {
+        let verbatim = <VerbatimUrl as UnnamedRequirementUrl>::parse_unnamed_url(&url)?;
+        Ok(Self {
+            parsed_url: ParsedUrl::try_from(verbatim.to_url())?,
+            verbatim,
+        })
+    }
+
+    fn with_given(self, given: impl Into<String>) -> Self {
+        Self {
+            verbatim: self.verbatim.with_given(given),
+            ..self
+        }
+    }
+
+    fn given(&self) -> Option<&str> {
+        self.verbatim.given()
+    }
+}
+
+impl Display for VerbatimParsedUrl {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
+        Display::fmt(&self.verbatim, f)
+    }
+}
+
+impl TryFrom<VerbatimUrl> for VerbatimParsedUrl {
+    type Error = ParsedUrlError;
+
+    fn try_from(verbatim_url: VerbatimUrl) -> Result<Self, Self::Error> {
+        let parsed_url = ParsedUrl::try_from(verbatim_url.to_url())?;
+        Ok(Self {
+            parsed_url,
+            verbatim: verbatim_url,
+        })
+    }
+}
+
+impl serde::ser::Serialize for VerbatimParsedUrl {
+    fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
+    where
+        S: serde::ser::Serializer,
+    {
+        self.verbatim.serialize(serializer)
+    }
+}
+
+impl<'de> serde::de::Deserialize<'de> for VerbatimParsedUrl {
+    fn deserialize<D>(deserializer: D) -> Result<VerbatimParsedUrl, D::Error>
+    where
+        D: serde::de::Deserializer<'de>,
+    {
+        let verbatim_url = VerbatimUrl::deserialize(deserializer)?;
+        Self::try_from(verbatim_url).map_err(serde::de::Error::custom)
+    }
+}
+
 /// We support three types of URLs for distributions:
 /// * The path to a file or directory (`file://`)
 /// * A Git repository (`git+https://` or `git+ssh://`), optionally with a subdirectory and/or
 ///   string to checkout.
 /// * A remote archive (`https://`), optional with a subdirectory (source dist only).
 ///
 /// A URL in a requirement `foo @ <url>` must be one of the above.
@@ -120,15 +223,15 @@
     let subdirectory = fragment
         .split('&')
         .find_map(|fragment| fragment.strip_prefix("subdirectory="))?;
     Some(PathBuf::from(subdirectory))
 }
 
 /// Return the Git reference of the given URL, if it exists.
-pub fn git_reference(url: Url) -> Result<Option<GitSha>, Error> {
+pub fn git_reference(url: Url) -> Result<Option<GitSha>, Box<ParsedUrlError>> {
     let ParsedGitUrl { url, .. } = ParsedGitUrl::try_from(url)?;
     Ok(url.precise())
 }
 
 impl TryFrom<Url> for ParsedUrl {
     type Error = ParsedUrlError;
 
@@ -168,62 +271,62 @@
             }))
         } else {
             Ok(Self::Archive(ParsedArchiveUrl::from(url)))
         }
     }
 }
 
-impl TryFrom<&ParsedUrl> for pypi_types::DirectUrl {
-    type Error = Error;
+impl TryFrom<&ParsedUrl> for DirectUrl {
+    type Error = ParsedUrlError;
 
-    fn try_from(value: &ParsedUrl) -> std::result::Result<Self, Self::Error> {
+    fn try_from(value: &ParsedUrl) -> Result<Self, Self::Error> {
         match value {
             ParsedUrl::Path(value) => Self::try_from(value),
             ParsedUrl::Git(value) => Self::try_from(value),
             ParsedUrl::Archive(value) => Self::try_from(value),
         }
     }
 }
 
-impl TryFrom<&ParsedPathUrl> for pypi_types::DirectUrl {
-    type Error = Error;
+impl TryFrom<&ParsedPathUrl> for DirectUrl {
+    type Error = ParsedUrlError;
 
     fn try_from(value: &ParsedPathUrl) -> Result<Self, Self::Error> {
         Ok(Self::LocalDirectory {
             url: value.url.to_string(),
-            dir_info: pypi_types::DirInfo {
+            dir_info: DirInfo {
                 editable: value.editable.then_some(true),
             },
         })
     }
 }
 
-impl TryFrom<&ParsedArchiveUrl> for pypi_types::DirectUrl {
-    type Error = Error;
+impl TryFrom<&ParsedArchiveUrl> for DirectUrl {
+    type Error = ParsedUrlError;
 
     fn try_from(value: &ParsedArchiveUrl) -> Result<Self, Self::Error> {
         Ok(Self::ArchiveUrl {
             url: value.url.to_string(),
-            archive_info: pypi_types::ArchiveInfo {
+            archive_info: ArchiveInfo {
                 hash: None,
                 hashes: None,
             },
             subdirectory: value.subdirectory.clone(),
         })
     }
 }
 
-impl TryFrom<&ParsedGitUrl> for pypi_types::DirectUrl {
-    type Error = Error;
+impl TryFrom<&ParsedGitUrl> for DirectUrl {
+    type Error = ParsedUrlError;
 
     fn try_from(value: &ParsedGitUrl) -> Result<Self, Self::Error> {
         Ok(Self::VcsUrl {
             url: value.url.repository().to_string(),
-            vcs_info: pypi_types::VcsInfo {
-                vcs: pypi_types::VcsKind::Git,
+            vcs_info: VcsInfo {
+                vcs: VcsKind::Git,
                 commit_id: value.url.precise().as_ref().map(ToString::to_string),
                 requested_revision: value.url.reference().as_str().map(ToString::to_string),
             },
             subdirectory: value.subdirectory.clone(),
         })
     }
 }
```

### Comparing `uv-0.2.2/crates/distribution-types/src/prioritized_distribution.rs` & `uv-0.2.3/crates/distribution-types/src/prioritized_distribution.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use distribution_filename::BuildTag;
 use std::fmt::{Display, Formatter};
 
 use pep440_rs::VersionSpecifiers;
 use platform_tags::{IncompatibleTag, TagPriority};
 use pypi_types::{HashDigest, Yanked};
 
 use crate::{
@@ -130,15 +131,15 @@
         }
     }
 }
 
 #[derive(Debug, Clone, PartialEq, Eq)]
 pub enum WheelCompatibility {
     Incompatible(IncompatibleWheel),
-    Compatible(HashComparison, TagPriority),
+    Compatible(HashComparison, TagPriority, Option<BuildTag>),
 }
 
 #[derive(Debug, PartialEq, Eq, Clone)]
 pub enum IncompatibleWheel {
     ExcludeNewer(Option<i64>),
     Tag(IncompatibleTag),
     RequiresPython(VersionSpecifiers),
@@ -241,15 +242,15 @@
     pub fn get(&self) -> Option<CompatibleDist> {
         let best_wheel = self.0.best_wheel_index.map(|i| &self.0.wheels[i]);
         match (&best_wheel, &self.0.source) {
             // If both are compatible, break ties based on the hash outcome. For example, prefer a
             // source distribution with a matching hash over a wheel with a mismatched hash. When
             // the outcomes are equivalent (e.g., both have a matching hash), prefer the wheel.
             (
-                Some((wheel, WheelCompatibility::Compatible(wheel_hash, tag_priority))),
+                Some((wheel, WheelCompatibility::Compatible(wheel_hash, tag_priority, ..))),
                 Some((sdist, SourceDistCompatibility::Compatible(sdist_hash))),
             ) => {
                 if sdist_hash > wheel_hash {
                     Some(CompatibleDist::SourceDist {
                         sdist,
                         prioritized: self,
                     })
@@ -258,15 +259,15 @@
                         wheel,
                         priority: *tag_priority,
                         prioritized: self,
                     })
                 }
             }
             // Prefer the highest-priority, platform-compatible wheel.
-            (Some((wheel, WheelCompatibility::Compatible(_, tag_priority))), _) => {
+            (Some((wheel, WheelCompatibility::Compatible(_, tag_priority, ..))), _) => {
                 Some(CompatibleDist::CompatibleWheel {
                     wheel,
                     priority: *tag_priority,
                     prioritized: self,
                 })
             }
             // If we have a compatible source distribution and an incompatible wheel, return the
@@ -305,15 +306,15 @@
 
     /// Return the incompatibility for the best wheel, if any.
     pub fn incompatible_wheel(&self) -> Option<&IncompatibleWheel> {
         self.0
             .best_wheel_index
             .map(|i| &self.0.wheels[i])
             .and_then(|(_, compatibility)| match compatibility {
-                WheelCompatibility::Compatible(_, _) => None,
+                WheelCompatibility::Compatible(_, _, _) => None,
                 WheelCompatibility::Incompatible(incompatibility) => Some(incompatibility),
             })
     }
 
     /// Return the hashes for each distribution.
     pub fn hashes(&self) -> &[HashDigest] {
         &self.0.hashes
@@ -411,29 +412,31 @@
             | CompatibleDist::IncompatibleWheel { .. } => true,
         }
     }
 }
 
 impl WheelCompatibility {
     pub fn is_compatible(&self) -> bool {
-        matches!(self, Self::Compatible(_, _))
+        matches!(self, Self::Compatible(_, _, _))
     }
 
     /// Return `true` if the current compatibility is more compatible than another.
     ///
     /// Compatible wheels are always higher more compatible than incompatible wheels.
     /// Compatible wheel ordering is determined by tag priority.
     pub fn is_more_compatible(&self, other: &Self) -> bool {
         match (self, other) {
-            (Self::Compatible(_, _), Self::Incompatible(_)) => true,
+            (Self::Compatible(_, _, _), Self::Incompatible(_)) => true,
             (
-                Self::Compatible(hash, tag_priority),
-                Self::Compatible(other_hash, other_tag_priority),
-            ) => (hash, tag_priority) > (other_hash, other_tag_priority),
-            (Self::Incompatible(_), Self::Compatible(_, _)) => false,
+                Self::Compatible(hash, tag_priority, build_tag),
+                Self::Compatible(other_hash, other_tag_priority, other_build_tag),
+            ) => {
+                (hash, tag_priority, build_tag) > (other_hash, other_tag_priority, other_build_tag)
+            }
+            (Self::Incompatible(_), Self::Compatible(_, _, _)) => false,
             (Self::Incompatible(incompatibility), Self::Incompatible(other_incompatibility)) => {
                 incompatibility.is_more_compatible(other_incompatibility)
             }
         }
     }
 }
```

### Comparing `uv-0.2.2/crates/distribution-types/src/requirement.rs` & `uv-0.2.3/crates/distribution-types/src/requirement.rs`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 use url::Url;
 
 use pep440_rs::VersionSpecifiers;
 use pep508_rs::{MarkerEnvironment, MarkerTree, RequirementOrigin, VerbatimUrl, VersionOrUrl};
 use uv_git::{GitReference, GitSha};
 use uv_normalize::{ExtraName, PackageName};
 
-use crate::{ParsedUrl, ParsedUrlError};
+use crate::{ParsedUrl, VerbatimParsedUrl};
 
 /// The requirements of a distribution, an extension over PEP 508's requirements.
 #[derive(Debug, Clone, Eq, PartialEq)]
 pub struct Requirements {
     pub dependencies: Vec<Requirement>,
     pub optional_dependencies: IndexMap<ExtraName, Vec<Requirement>>,
 }
@@ -40,39 +40,40 @@
     pub fn evaluate_markers(&self, env: Option<&MarkerEnvironment>, extras: &[ExtraName]) -> bool {
         if let Some(marker) = &self.marker {
             marker.evaluate_optional_environment(env, extras)
         } else {
             true
         }
     }
+}
 
+impl From<pep508_rs::Requirement<VerbatimParsedUrl>> for Requirement {
     /// Convert a [`pep508_rs::Requirement`] to a [`Requirement`].
-    pub fn from_pep508(requirement: pep508_rs::Requirement) -> Result<Self, Box<ParsedUrlError>> {
+    fn from(requirement: pep508_rs::Requirement<VerbatimParsedUrl>) -> Self {
         let source = match requirement.version_or_url {
             None => RequirementSource::Registry {
                 specifier: VersionSpecifiers::empty(),
                 index: None,
             },
             // The most popular case: just a name, a version range and maybe extras.
             Some(VersionOrUrl::VersionSpecifier(specifier)) => RequirementSource::Registry {
                 specifier,
                 index: None,
             },
             Some(VersionOrUrl::Url(url)) => {
-                let direct_url = ParsedUrl::try_from(url.to_url())?;
-                RequirementSource::from_parsed_url(direct_url, url)
+                RequirementSource::from_parsed_url(url.parsed_url, url.verbatim)
             }
         };
-        Ok(Requirement {
+        Requirement {
             name: requirement.name,
             extras: requirement.extras,
             marker: requirement.marker,
             source,
             origin: requirement.origin,
-        })
+        }
     }
 }
 
 impl Display for Requirement {
     /// Display the [`Requirement`], with the intention of being shown directly to a user, rather
     /// than for inclusion in a `requirements.txt` file.
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
```

### Comparing `uv-0.2.2/crates/distribution-types/src/requirements.rs` & `uv-0.2.3/crates/distribution-types/src/requirements.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/distribution-types/src/resolution.rs` & `uv-0.2.3/crates/distribution-types/src/resolution.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 use std::collections::BTreeMap;
 
 use pep508_rs::VerbatimUrl;
 use uv_normalize::{ExtraName, PackageName};
 
 use crate::{
-    BuiltDist, DirectorySourceDist, Dist, InstalledDirectUrlDist, InstalledDist, LocalEditable,
-    Name, Requirement, RequirementSource, ResolvedDist, SourceDist,
+    BuiltDist, Diagnostic, DirectorySourceDist, Dist, InstalledDirectUrlDist, InstalledDist,
+    LocalEditable, Name, Requirement, RequirementSource, ResolvedDist, SourceDist,
 };
 
 /// A set of packages pinned at specific versions.
 #[derive(Debug, Default, Clone)]
 pub struct Resolution {
     packages: BTreeMap<PackageName, ResolvedDist>,
-    diagnostics: Vec<Diagnostic>,
+    diagnostics: Vec<ResolutionDiagnostic>,
 }
 
 impl Resolution {
     /// Create a new resolution from the given pinned packages.
     pub fn new(
         packages: BTreeMap<PackageName, ResolvedDist>,
-        diagnostics: Vec<Diagnostic>,
+        diagnostics: Vec<ResolutionDiagnostic>,
     ) -> Self {
         Self {
             packages,
             diagnostics,
         }
     }
 
@@ -59,16 +59,16 @@
     }
 
     /// Return the set of [`Requirement`]s that this resolution represents.
     pub fn requirements(&self) -> impl Iterator<Item = Requirement> + '_ {
         self.packages.values().map(Requirement::from)
     }
 
-    /// Return the [`Diagnostic`]s that were produced during resolution.
-    pub fn diagnostics(&self) -> &[Diagnostic] {
+    /// Return the [`ResolutionDiagnostic`]s that were produced during resolution.
+    pub fn diagnostics(&self) -> &[ResolutionDiagnostic] {
         &self.diagnostics
     }
 
     /// Return an iterator over the [`LocalEditable`] entities in this resolution.
     pub fn editables(&self) -> impl Iterator<Item = LocalEditable> + '_ {
         self.packages.values().filter_map(|dist| match dist {
             ResolvedDist::Installable(Dist::Source(SourceDist::Directory(
@@ -95,15 +95,15 @@
             }),
             _ => None,
         })
     }
 }
 
 #[derive(Debug, Clone)]
-pub enum Diagnostic {
+pub enum ResolutionDiagnostic {
     MissingExtra {
         /// The distribution that was requested with a non-existent extra. For example,
         /// `black==23.10.0`.
         dist: ResolvedDist,
         /// The extra that was requested. For example, `colorama` in `black[colorama]`.
         extra: ExtraName,
     },
@@ -111,17 +111,17 @@
         /// The package that was requested with a yanked version. For example, `black==23.10.0`.
         dist: ResolvedDist,
         /// The reason that the version was yanked, if any.
         reason: Option<String>,
     },
 }
 
-impl Diagnostic {
+impl Diagnostic for ResolutionDiagnostic {
     /// Convert the diagnostic into a user-facing message.
-    pub fn message(&self) -> String {
+    fn message(&self) -> String {
         match self {
             Self::MissingExtra { dist, extra } => {
                 format!("The package `{dist}` does not have an extra named `{extra}`.")
             }
             Self::YankedVersion { dist, reason } => {
                 if let Some(reason) = reason {
                     format!("`{dist}` is yanked (reason: \"{reason}\").")
@@ -129,15 +129,15 @@
                     format!("`{dist}` is yanked.")
                 }
             }
         }
     }
 
     /// Returns `true` if the [`PackageName`] is involved in this diagnostic.
-    pub fn includes(&self, name: &PackageName) -> bool {
+    fn includes(&self, name: &PackageName) -> bool {
         match self {
             Self::MissingExtra { dist, .. } => name == dist.name(),
             Self::YankedVersion { dist, .. } => name == dist.name(),
         }
     }
 }
```

### Comparing `uv-0.2.2/crates/distribution-types/src/resolved.rs` & `uv-0.2.3/crates/distribution-types/src/resolved.rs`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,22 @@
     pub fn is_editable(&self) -> bool {
         match self {
             Self::Installable(dist) => dist.is_editable(),
             Self::Installed(dist) => dist.is_editable(),
         }
     }
 
+    /// Return true if the distribution refers to a local file or directory.
+    pub fn is_local(&self) -> bool {
+        match self {
+            Self::Installable(dist) => dist.is_local(),
+            Self::Installed(dist) => dist.is_local(),
+        }
+    }
+
     /// Returns the [`IndexUrl`], if the distribution is from a registry.
     pub fn index(&self) -> Option<&IndexUrl> {
         match self {
             Self::Installable(dist) => dist.index(),
             Self::Installed(_) => None,
         }
     }
```

### Comparing `uv-0.2.2/crates/distribution-types/src/specified_requirement.rs` & `uv-0.2.3/crates/distribution-types/src/specified_requirement.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use std::borrow::Cow;
 use std::fmt::{Display, Formatter};
 
 use pep508_rs::{MarkerEnvironment, UnnamedRequirement};
 use uv_normalize::ExtraName;
 
-use crate::{ParsedUrl, ParsedUrlError, Requirement, RequirementSource};
+use crate::{Requirement, RequirementSource, VerbatimParsedUrl};
 
 /// An [`UnresolvedRequirement`] with additional metadata from `requirements.txt`, currently only
 /// hashes but in the future also editable and similar information.
 #[derive(Debug, Clone, Eq, PartialEq, Hash)]
 pub struct UnresolvedRequirementSpecification {
     /// The actual requirement.
     pub requirement: UnresolvedRequirement,
@@ -25,15 +25,15 @@
 /// `pep508_rs::Requirement`.
 #[derive(Hash, Debug, Clone, Eq, PartialEq)]
 pub enum UnresolvedRequirement {
     /// The uv-specific superset over PEP 508 requirements specifier incorporating
     /// `tool.uv.sources`.
     Named(Requirement),
     /// A PEP 508-like, direct URL dependency specifier.
-    Unnamed(UnnamedRequirement),
+    Unnamed(UnnamedRequirement<VerbatimParsedUrl>),
 }
 
 impl Display for UnresolvedRequirement {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         match self {
             Self::Named(requirement) => write!(f, "{requirement}"),
             Self::Unnamed(requirement) => write!(f, "{requirement}"),
@@ -60,21 +60,17 @@
         match self {
             Self::Named(requirement) => requirement.extras.as_slice(),
             Self::Unnamed(requirement) => requirement.extras.as_slice(),
         }
     }
 
     /// Return the version specifier or URL for the requirement.
-    pub fn source(&self) -> Result<Cow<'_, RequirementSource>, Box<ParsedUrlError>> {
-        // TODO(konsti): This is a bad place to raise errors, we should have parsed the url earlier.
+    pub fn source(&self) -> Cow<'_, RequirementSource> {
         match self {
-            Self::Named(requirement) => Ok(Cow::Borrowed(&requirement.source)),
-            Self::Unnamed(requirement) => {
-                let parsed_url = ParsedUrl::try_from(requirement.url.to_url())?;
-                Ok(Cow::Owned(RequirementSource::from_parsed_url(
-                    parsed_url,
-                    requirement.url.clone(),
-                )))
-            }
+            Self::Named(requirement) => Cow::Borrowed(&requirement.source),
+            Self::Unnamed(requirement) => Cow::Owned(RequirementSource::from_parsed_url(
+                requirement.url.parsed_url.clone(),
+                requirement.url.verbatim.clone(),
+            )),
         }
     }
 }
```

### Comparing `uv-0.2.2/crates/distribution-types/src/traits.rs` & `uv-0.2.3/crates/distribution-types/src/traits.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-requirements/Cargo.toml` & `uv-0.2.3/crates/uv-requirements/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-requirements/src/confirm.rs` & `uv-0.2.3/crates/uv-requirements/src/confirm.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-requirements/src/lookahead.rs` & `uv-0.2.3/crates/uv-requirements/src/lookahead.rs`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 pub enum LookaheadError {
     #[error("Failed to download: `{0}`")]
     Download(BuiltDist, #[source] uv_distribution::Error),
     #[error("Failed to download and build: `{0}`")]
     DownloadAndBuild(SourceDist, #[source] uv_distribution::Error),
     #[error(transparent)]
     UnsupportedUrl(#[from] distribution_types::Error),
-    #[error(transparent)]
-    InvalidRequirement(#[from] Box<distribution_types::ParsedUrlError>),
 }
 
 /// A resolver for resolving lookahead requirements from direct URLs.
 ///
 /// The resolver extends certain privileges to "first-party" requirements. For example, first-party
 /// requirements are allowed to contain direct URL references, local version specifiers, and more.
 ///
@@ -207,16 +205,16 @@
             {
                 // If the metadata is already in the index, return it.
                 archive
                     .metadata
                     .requires_dist
                     .iter()
                     .cloned()
-                    .map(Requirement::from_pep508)
-                    .collect::<Result<_, _>>()?
+                    .map(Requirement::from)
+                    .collect()
             } else {
                 // Run the PEP 517 build process to extract metadata from the source distribution.
                 let archive = self
                     .database
                     .get_or_build_wheel_metadata(&dist, self.hasher.get(&dist))
                     .await
                     .map_err(|err| match &dist {
@@ -229,18 +227,15 @@
                 let requires_dist = archive.metadata.requires_dist.clone();
 
                 // Insert the metadata into the index.
                 self.index
                     .distributions()
                     .done(id, Arc::new(MetadataResponse::Found(archive)));
 
-                requires_dist
-                    .into_iter()
-                    .map(Requirement::from_pep508)
-                    .collect::<Result<_, _>>()?
+                requires_dist.into_iter().map(Requirement::from).collect()
             }
         };
 
         // Consider the dependencies to be "direct" if the requirement is a local source tree.
         let direct = if let Dist::Source(source_dist) = &dist {
             source_dist.as_path().is_some_and(std::path::Path::is_dir)
         } else {
```

### Comparing `uv-0.2.2/crates/uv-requirements/src/pyproject.rs` & `uv-0.2.3/crates/uv-requirements/src/pyproject.rs`

 * *Files 2% similar despite different names*

```diff
@@ -16,43 +16,48 @@
 use indexmap::IndexMap;
 use path_absolutize::Absolutize;
 use rustc_hash::FxHashSet;
 use serde::{Deserialize, Serialize};
 use thiserror::Error;
 use url::Url;
 
-use distribution_types::{ParsedUrlError, Requirement, RequirementSource, Requirements};
+use distribution_types::{Requirement, RequirementSource, Requirements};
 use pep440_rs::VersionSpecifiers;
-use pep508_rs::{RequirementOrigin, VerbatimUrl, VersionOrUrl};
+use pep508_rs::{Pep508Error, RequirementOrigin, VerbatimUrl, VersionOrUrl};
+use pypi_types::VerbatimParsedUrl;
 use uv_configuration::PreviewMode;
 use uv_fs::Simplified;
 use uv_git::GitReference;
 use uv_normalize::{ExtraName, PackageName};
 use uv_warnings::warn_user_once;
 
 use crate::ExtrasSpecification;
 
 #[derive(Debug, Error)]
 pub enum Pep621Error {
     #[error(transparent)]
-    Pep508(#[from] pep508_rs::Pep508Error),
+    Pep508(#[from] Box<Pep508Error<VerbatimParsedUrl>>),
     #[error("Must specify a `[project]` section alongside `[tool.uv.sources]`")]
     MissingProjectSection,
     #[error("pyproject.toml section is declared as dynamic, but must be static: `{0}`")]
     CantBeDynamic(&'static str),
     #[error("Failed to parse entry for: `{0}`")]
     LoweringError(PackageName, #[source] LoweringError),
 }
 
+impl From<Pep508Error<VerbatimParsedUrl>> for Pep621Error {
+    fn from(error: Pep508Error<VerbatimParsedUrl>) -> Self {
+        Self::Pep508(Box::new(error))
+    }
+}
+
 /// An error parsing and merging `tool.uv.sources` with
 /// `project.{dependencies,optional-dependencies}`.
 #[derive(Debug, Error)]
 pub enum LoweringError {
-    #[error("Invalid URL structure")]
-    DirectUrl(#[from] Box<ParsedUrlError>),
     #[error("Unsupported path (can't convert to URL): `{}`", _0.user_display())]
     PathToUrl(PathBuf),
     #[error("Package is not included as workspace package in `tool.uv.workspace`")]
     UndeclaredWorkspacePackage,
     #[error("Can only specify one of rev, tag, or branch")]
     MoreThanOneGitRef,
     #[error("Unable to combine options in `tool.uv.sources`")]
@@ -381,15 +386,15 @@
         dependencies,
         optional_dependencies,
     })
 }
 
 /// Combine `project.dependencies` or `project.optional-dependencies` with `tool.uv.sources`.
 pub(crate) fn lower_requirement(
-    requirement: pep508_rs::Requirement,
+    requirement: pep508_rs::Requirement<VerbatimParsedUrl>,
     project_name: &PackageName,
     project_dir: &Path,
     project_sources: &BTreeMap<PackageName, Source>,
     workspace_sources: &BTreeMap<PackageName, Source>,
     workspace_packages: &BTreeMap<PackageName, String>,
     preview: PreviewMode,
 ) -> Result<Requirement, LoweringError> {
@@ -416,15 +421,15 @@
         if has_sources && requirement.version_or_url.is_none() && &requirement.name != project_name
         {
             warn_user_once!(
                 "Missing version constraint (e.g., a lower bound) for `{}`",
                 requirement.name
             );
         }
-        return Ok(Requirement::from_pep508(requirement)?);
+        return Ok(Requirement::from(requirement));
     };
 
     if preview.is_disabled() {
         return Err(LoweringError::MissingPreview);
     }
 
     let source = match source {
@@ -676,15 +681,15 @@
         let path = uv_fs::absolutize_path(path.as_ref())?;
         RequirementsSpecification::parse_direct_pyproject_toml(
             contents,
             extras,
             path.as_ref(),
             PreviewMode::Enabled,
         )
-        .with_context(|| format!("Failed to parse `{}`", path.user_display()))
+        .with_context(|| format!("Failed to parse: `{}`", path.user_display()))
     }
 
     fn format_err(input: &str) -> String {
         let err = from_source(input, "pyproject.toml", &ExtrasSpecification::None).unwrap_err();
         let mut causes = err.chain();
         let mut message = String::new();
         message.push_str(&format!("error: {}\n", causes.next().unwrap()));
@@ -705,15 +710,15 @@
             ]
 
             [tool.uv.sources]
             tqdm = { url = "https://files.pythonhosted.org/packages/a5/d6/502a859bac4ad5e274255576cd3e15ca273cdb91731bc39fb840dd422ee9/tqdm-4.66.0-py3-none-any.whl" }
         "#};
 
         assert_snapshot!(format_err(input), @r###"
-        error: Failed to parse `pyproject.toml`
+        error: Failed to parse: `pyproject.toml`
           Caused by: Failed to parse entry for: `tqdm`
           Caused by: Can't combine URLs from both `project.dependencies` and `tool.uv.sources`
         "###);
     }
 
     #[test]
     fn too_many_git_specs() {
@@ -726,15 +731,15 @@
             ]
 
             [tool.uv.sources]
             tqdm = { git = "https://github.com/tqdm/tqdm", rev = "baaaaaab", tag = "v1.0.0" }
         "#};
 
         assert_snapshot!(format_err(input), @r###"
-        error: Failed to parse `pyproject.toml`
+        error: Failed to parse: `pyproject.toml`
           Caused by: Failed to parse entry for: `tqdm`
           Caused by: Can only specify one of rev, tag, or branch
         "###);
     }
 
     #[test]
     fn too_many_git_typo() {
@@ -748,15 +753,15 @@
 
             [tool.uv.sources]
             tqdm = { git = "https://github.com/tqdm/tqdm", ref = "baaaaaab" }
         "#};
 
         // TODO(konsti): This should tell you the set of valid fields
         assert_snapshot!(format_err(input), @r###"
-        error: Failed to parse `pyproject.toml`
+        error: Failed to parse: `pyproject.toml`
           Caused by: TOML parse error at line 9, column 8
           |
         9 | tqdm = { git = "https://github.com/tqdm/tqdm", ref = "baaaaaab" }
           |        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
         data did not match any variant of untagged enum Source
 
         "###);
@@ -774,15 +779,15 @@
 
             [tool.uv.sources]
             tqdm = { path = "tqdm", index = "torch" }
         "#};
 
         // TODO(konsti): This should tell you the set of valid fields
         assert_snapshot!(format_err(input), @r###"
-        error: Failed to parse `pyproject.toml`
+        error: Failed to parse: `pyproject.toml`
           Caused by: TOML parse error at line 9, column 8
           |
         9 | tqdm = { path = "tqdm", index = "torch" }
           |        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
         data did not match any variant of untagged enum Source
 
         "###);
@@ -813,15 +818,15 @@
             ]
 
             [tool.uv.sources]
             tqdm = { url = invalid url to tqdm-4.66.0-py3-none-any.whl" }
         "#};
 
         assert_snapshot!(format_err(input), @r###"
-        error: Failed to parse `pyproject.toml`
+        error: Failed to parse: `pyproject.toml`
           Caused by: TOML parse error at line 9, column 16
           |
         9 | tqdm = { url = invalid url to tqdm-4.66.0-py3-none-any.whl" }
           |                ^
         invalid string
         expected `"`, `'`
 
@@ -839,15 +844,15 @@
             ]
 
             [tool.uv.sources]
             tqdm = { url = "§invalid#+#*Ä" }
         "#};
 
         assert_snapshot!(format_err(input), @r###"
-        error: Failed to parse `pyproject.toml`
+        error: Failed to parse: `pyproject.toml`
           Caused by: TOML parse error at line 9, column 8
           |
         9 | tqdm = { url = "§invalid#+#*Ä" }
           |        ^^^^^^^^^^^^^^^^^^^^^^^^^^^
         data did not match any variant of untagged enum Source
 
         "###);
@@ -864,15 +869,15 @@
             ]
 
             [tool.uv.sources]
             tqdm = { workspace = true }
         "#};
 
         assert_snapshot!(format_err(input), @r###"
-        error: Failed to parse `pyproject.toml`
+        error: Failed to parse: `pyproject.toml`
           Caused by: Failed to parse entry for: `tqdm`
           Caused by: Can't combine URLs from both `project.dependencies` and `tool.uv.sources`
         "###);
     }
 
     #[test]
     fn missing_workspace_package() {
@@ -885,15 +890,15 @@
             ]
 
             [tool.uv.sources]
             tqdm = { workspace = true }
         "#};
 
         assert_snapshot!(format_err(input), @r###"
-        error: Failed to parse `pyproject.toml`
+        error: Failed to parse: `pyproject.toml`
           Caused by: Failed to parse entry for: `tqdm`
           Caused by: Package is not included as workspace package in `tool.uv.workspace`
         "###);
     }
 
     #[test]
     fn cant_be_dynamic() {
@@ -906,25 +911,25 @@
             ]
 
             [tool.uv.sources]
             tqdm = { workspace = true }
         "#};
 
         assert_snapshot!(format_err(input), @r###"
-        error: Failed to parse `pyproject.toml`
+        error: Failed to parse: `pyproject.toml`
           Caused by: pyproject.toml section is declared as dynamic, but must be static: `project.dependencies`
         "###);
     }
 
     #[test]
     fn missing_project_section() {
         let input = indoc! {"
             [tool.uv.sources]
             tqdm = { workspace = true }
         "};
 
         assert_snapshot!(format_err(input), @r###"
-        error: Failed to parse `pyproject.toml`
+        error: Failed to parse: `pyproject.toml`
           Caused by: Must specify a `[project]` section alongside `[tool.uv.sources]`
         "###);
     }
 }
```

### Comparing `uv-0.2.2/crates/uv-requirements/src/source_tree.rs` & `uv-0.2.3/crates/uv-requirements/src/source_tree.rs`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 use futures::TryStreamExt;
 use url::Url;
 
 use distribution_types::{
     BuildableSource, DirectorySourceUrl, HashPolicy, Requirement, SourceUrl, VersionId,
 };
 use pep508_rs::RequirementOrigin;
+use pypi_types::VerbatimParsedUrl;
 use uv_distribution::{DistributionDatabase, Reporter};
 use uv_fs::Simplified;
 use uv_resolver::{InMemoryIndex, MetadataResponse};
 use uv_types::{BuildContext, HashStrategy};
 
 use crate::ExtrasSpecification;
 
@@ -70,20 +71,23 @@
             .map(|source_tree| async { self.resolve_source_tree(source_tree).await })
             .collect::<FuturesOrdered<_>>()
             .try_collect()
             .await?;
         Ok(requirements
             .into_iter()
             .flatten()
-            .map(Requirement::from_pep508)
-            .collect::<Result<_, _>>()?)
+            .map(Requirement::from)
+            .collect())
     }
 
     /// Infer the package name for a given "unnamed" requirement.
-    async fn resolve_source_tree(&self, path: &Path) -> Result<Vec<pep508_rs::Requirement>> {
+    async fn resolve_source_tree(
+        &self,
+        path: &Path,
+    ) -> Result<Vec<pep508_rs::Requirement<VerbatimParsedUrl>>> {
         // Convert to a buildable source.
         let source_tree = fs_err::canonicalize(path).with_context(|| {
             format!(
                 "Failed to canonicalize path to source tree: {}",
                 path.user_display()
             )
         })?;
```

### Comparing `uv-0.2.2/crates/uv-requirements/src/sources.rs` & `uv-0.2.3/crates/uv-requirements/src/sources.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-requirements/src/specification.rs` & `uv-0.2.3/crates/uv-requirements/src/specification.rs`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 use tracing::{debug, instrument};
 
 use cache_key::CanonicalUrl;
 use distribution_types::{
     FlatIndexLocation, IndexUrl, Requirement, RequirementSource, UnresolvedRequirement,
     UnresolvedRequirementSpecification,
 };
-use pep508_rs::{UnnamedRequirement, VerbatimUrl};
+use pep508_rs::{UnnamedRequirement, UnnamedRequirementUrl};
+use pypi_types::VerbatimParsedUrl;
 use requirements_txt::{
     EditableRequirement, FindLink, RequirementEntry, RequirementsTxt, RequirementsTxtRequirement,
 };
 use uv_client::BaseClientBuilder;
 use uv_configuration::{NoBinary, NoBuild, PreviewMode};
 use uv_fs::Simplified;
 use uv_normalize::{ExtraName, PackageName};
@@ -61,28 +62,28 @@
         extras: &ExtrasSpecification,
         client_builder: &BaseClientBuilder<'_>,
         preview: PreviewMode,
     ) -> Result<Self> {
         Ok(match source {
             RequirementsSource::Package(name) => {
                 let requirement = RequirementsTxtRequirement::parse(name, std::env::current_dir()?)
-                    .with_context(|| format!("Failed to parse `{name}`"))?;
+                    .with_context(|| format!("Failed to parse: `{name}`"))?;
                 Self {
-                    requirements: vec![UnresolvedRequirementSpecification::try_from(
+                    requirements: vec![UnresolvedRequirementSpecification::from(
                         RequirementEntry {
                             requirement,
                             hashes: vec![],
                         },
-                    )?],
+                    )],
                     ..Self::default()
                 }
             }
             RequirementsSource::Editable(name) => {
                 let requirement = EditableRequirement::parse(name, None, std::env::current_dir()?)
-                    .with_context(|| format!("Failed to parse `{name}`"))?;
+                    .with_context(|| format!("Failed to parse: `{name}`"))?;
                 Self {
                     editables: vec![requirement],
                     ..Self::default()
                 }
             }
             RequirementsSource::RequirementsTxt(path) => {
                 let requirements_txt =
@@ -92,16 +93,16 @@
                         .requirements
                         .into_iter()
                         .map(UnresolvedRequirementSpecification::try_from)
                         .collect::<Result<_, _>>()?,
                     constraints: requirements_txt
                         .constraints
                         .into_iter()
-                        .map(Requirement::from_pep508)
-                        .collect::<Result<_, _>>()?,
+                        .map(Requirement::from)
+                        .collect(),
                     editables: requirements_txt.editables,
                     index_url: requirements_txt.index_url.map(IndexUrl::from),
                     extra_index_urls: requirements_txt
                         .extra_index_urls
                         .into_iter()
                         .map(IndexUrl::from)
                         .collect(),
@@ -118,25 +119,25 @@
                     no_build: requirements_txt.only_binary,
                     ..Self::default()
                 }
             }
             RequirementsSource::PyprojectToml(path) => {
                 let contents = uv_fs::read_to_string(&path).await?;
                 Self::parse_direct_pyproject_toml(&contents, extras, path.as_ref(), preview)
-                    .with_context(|| format!("Failed to parse `{}`", path.user_display()))?
+                    .with_context(|| format!("Failed to parse: `{}`", path.user_display()))?
             }
             RequirementsSource::SetupPy(path) | RequirementsSource::SetupCfg(path) => Self {
                 source_trees: vec![path.clone()],
                 ..Self::default()
             },
             RequirementsSource::SourceTree(path) => Self {
                 project: None,
                 requirements: vec![UnresolvedRequirementSpecification {
                     requirement: UnresolvedRequirement::Unnamed(UnnamedRequirement {
-                        url: VerbatimUrl::from_path(path)?,
+                        url: VerbatimParsedUrl::parse_absolute_path(path)?,
                         extras: vec![],
                         marker: None,
                         origin: None,
                     }),
                     hashes: vec![],
                 }],
                 ..Self::default()
```

### Comparing `uv-0.2.2/crates/uv-requirements/src/unnamed.rs` & `uv-0.2.3/crates/uv-requirements/src/unnamed.rs`

 * *Files 7% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 use configparser::ini::Ini;
 use futures::{stream::FuturesOrdered, TryStreamExt};
 use serde::Deserialize;
 use tracing::debug;
 
 use distribution_filename::{SourceDistFilename, WheelFilename};
 use distribution_types::{
-    BuildableSource, DirectSourceUrl, DirectorySourceUrl, GitSourceUrl, ParsedGitUrl,
-    PathSourceUrl, RemoteSource, Requirement, SourceUrl, UnresolvedRequirement,
+    BuildableSource, DirectSourceUrl, DirectorySourceUrl, GitSourceUrl, PathSourceUrl,
+    RemoteSource, Requirement, SourceUrl, UnresolvedRequirement,
     UnresolvedRequirementSpecification, VersionId,
 };
-use pep508_rs::{Scheme, UnnamedRequirement, VersionOrUrl};
-use pypi_types::Metadata10;
+use pep508_rs::{UnnamedRequirement, VersionOrUrl};
+use pypi_types::{Metadata10, ParsedUrl, VerbatimParsedUrl};
 use uv_distribution::{DistributionDatabase, Reporter};
 use uv_normalize::PackageName;
 use uv_resolver::{InMemoryIndex, MetadataResponse};
 use uv_types::{BuildContext, HashStrategy};
 
 /// Like [`RequirementsSpecification`], but with concrete names for all requirements.
 pub struct NamedRequirementsResolver<'a, Context: BuildContext> {
@@ -68,39 +68,39 @@
             database,
         } = self;
         requirements
             .into_iter()
             .map(|entry| async {
                 match entry.requirement {
                     UnresolvedRequirement::Named(requirement) => Ok(requirement),
-                    UnresolvedRequirement::Unnamed(requirement) => Ok(Requirement::from_pep508(
+                    UnresolvedRequirement::Unnamed(requirement) => Ok(Requirement::from(
                         Self::resolve_requirement(requirement, hasher, index, &database).await?,
-                    )?),
+                    )),
                 }
             })
             .collect::<FuturesOrdered<_>>()
             .try_collect()
             .await
     }
 
     /// Infer the package name for a given "unnamed" requirement.
     async fn resolve_requirement(
-        requirement: UnnamedRequirement,
+        requirement: UnnamedRequirement<VerbatimParsedUrl>,
         hasher: &HashStrategy,
         index: &InMemoryIndex,
         database: &DistributionDatabase<'a, Context>,
-    ) -> Result<pep508_rs::Requirement> {
+    ) -> Result<pep508_rs::Requirement<VerbatimParsedUrl>> {
         // If the requirement is a wheel, extract the package name from the wheel filename.
         //
         // Ex) `anyio-4.3.0-py3-none-any.whl`
-        if Path::new(requirement.url.path())
+        if Path::new(requirement.url.verbatim.path())
             .extension()
             .is_some_and(|ext| ext.eq_ignore_ascii_case("whl"))
         {
-            let filename = WheelFilename::from_str(&requirement.url.filename()?)?;
+            let filename = WheelFilename::from_str(&requirement.url.verbatim.filename()?)?;
             return Ok(pep508_rs::Requirement {
                 name: filename.name,
                 extras: requirement.extras,
                 version_or_url: Some(VersionOrUrl::Url(requirement.url)),
                 marker: requirement.marker,
                 origin: requirement.origin,
             });
@@ -108,155 +108,141 @@
 
         // If the requirement is a source archive, try to extract the package name from the archive
         // filename. This isn't guaranteed to work.
         //
         // Ex) `anyio-4.3.0.tar.gz`
         if let Some(filename) = requirement
             .url
+            .verbatim
             .filename()
             .ok()
             .and_then(|filename| SourceDistFilename::parsed_normalized_filename(&filename).ok())
         {
             return Ok(pep508_rs::Requirement {
                 name: filename.name,
                 extras: requirement.extras,
                 version_or_url: Some(VersionOrUrl::Url(requirement.url)),
                 marker: requirement.marker,
                 origin: requirement.origin,
             });
         }
 
-        let source = match Scheme::parse(requirement.url.scheme()) {
-            Some(Scheme::File) => {
-                let path = requirement
-                    .url
-                    .to_file_path()
-                    .expect("URL to be a file path");
-
-                // If the path points to a directory, attempt to read the name from static metadata.
-                if path.is_dir() {
-                    // Attempt to read a `PKG-INFO` from the directory.
-                    if let Some(metadata) = fs_err::read(path.join("PKG-INFO"))
-                        .ok()
-                        .and_then(|contents| Metadata10::parse_pkg_info(&contents).ok())
-                    {
+        let source = match &requirement.url.parsed_url {
+            // If the path points to a directory, attempt to read the name from static metadata.
+            ParsedUrl::Path(parsed_path_url) if parsed_path_url.path.is_dir() => {
+                // Attempt to read a `PKG-INFO` from the directory.
+                if let Some(metadata) = fs_err::read(parsed_path_url.path.join("PKG-INFO"))
+                    .ok()
+                    .and_then(|contents| Metadata10::parse_pkg_info(&contents).ok())
+                {
+                    debug!(
+                        "Found PKG-INFO metadata for {path} ({name})",
+                        path = parsed_path_url.path.display(),
+                        name = metadata.name
+                    );
+                    return Ok(pep508_rs::Requirement {
+                        name: metadata.name,
+                        extras: requirement.extras,
+                        version_or_url: Some(VersionOrUrl::Url(requirement.url)),
+                        marker: requirement.marker,
+                        origin: requirement.origin,
+                    });
+                }
+
+                // Attempt to read a `pyproject.toml` file.
+                let project_path = parsed_path_url.path.join("pyproject.toml");
+                if let Some(pyproject) = fs_err::read_to_string(project_path)
+                    .ok()
+                    .and_then(|contents| toml::from_str::<PyProjectToml>(&contents).ok())
+                {
+                    // Read PEP 621 metadata from the `pyproject.toml`.
+                    if let Some(project) = pyproject.project {
                         debug!(
-                            "Found PKG-INFO metadata for {path} ({name})",
-                            path = path.display(),
-                            name = metadata.name
+                            "Found PEP 621 metadata for {path} in `pyproject.toml` ({name})",
+                            path = parsed_path_url.path.display(),
+                            name = project.name
                         );
                         return Ok(pep508_rs::Requirement {
-                            name: metadata.name,
+                            name: project.name,
                             extras: requirement.extras,
                             version_or_url: Some(VersionOrUrl::Url(requirement.url)),
                             marker: requirement.marker,
                             origin: requirement.origin,
                         });
                     }
 
-                    // Attempt to read a `pyproject.toml` file.
-                    let project_path = path.join("pyproject.toml");
-                    if let Some(pyproject) = fs_err::read_to_string(project_path)
-                        .ok()
-                        .and_then(|contents| toml::from_str::<PyProjectToml>(&contents).ok())
-                    {
-                        // Read PEP 621 metadata from the `pyproject.toml`.
-                        if let Some(project) = pyproject.project {
-                            debug!(
-                                "Found PEP 621 metadata for {path} in `pyproject.toml` ({name})",
-                                path = path.display(),
-                                name = project.name
-                            );
-                            return Ok(pep508_rs::Requirement {
-                                name: project.name,
-                                extras: requirement.extras,
-                                version_or_url: Some(VersionOrUrl::Url(requirement.url)),
-                                marker: requirement.marker,
-                                origin: requirement.origin,
-                            });
-                        }
-
-                        // Read Poetry-specific metadata from the `pyproject.toml`.
-                        if let Some(tool) = pyproject.tool {
-                            if let Some(poetry) = tool.poetry {
-                                if let Some(name) = poetry.name {
-                                    debug!(
-                                        "Found Poetry metadata for {path} in `pyproject.toml` ({name})",
-                                        path = path.display(),
-                                        name = name
-                                    );
-                                    return Ok(pep508_rs::Requirement {
-                                        name,
-                                        extras: requirement.extras,
-                                        version_or_url: Some(VersionOrUrl::Url(requirement.url)),
-                                        marker: requirement.marker,
-                                        origin: requirement.origin,
-                                    });
-                                }
+                    // Read Poetry-specific metadata from the `pyproject.toml`.
+                    if let Some(tool) = pyproject.tool {
+                        if let Some(poetry) = tool.poetry {
+                            if let Some(name) = poetry.name {
+                                debug!(
+                                    "Found Poetry metadata for {path} in `pyproject.toml` ({name})",
+                                    path = parsed_path_url.path.display(),
+                                    name = name
+                                );
+                                return Ok(pep508_rs::Requirement {
+                                    name,
+                                    extras: requirement.extras,
+                                    version_or_url: Some(VersionOrUrl::Url(requirement.url)),
+                                    marker: requirement.marker,
+                                    origin: requirement.origin,
+                                });
                             }
                         }
                     }
+                }
 
-                    // Attempt to read a `setup.cfg` from the directory.
-                    if let Some(setup_cfg) = fs_err::read_to_string(path.join("setup.cfg"))
+                // Attempt to read a `setup.cfg` from the directory.
+                if let Some(setup_cfg) =
+                    fs_err::read_to_string(parsed_path_url.path.join("setup.cfg"))
                         .ok()
                         .and_then(|contents| {
                             let mut ini = Ini::new_cs();
                             ini.set_multiline(true);
                             ini.read(contents).ok()
                         })
-                    {
-                        if let Some(section) = setup_cfg.get("metadata") {
-                            if let Some(Some(name)) = section.get("name") {
-                                if let Ok(name) = PackageName::from_str(name) {
-                                    debug!(
-                                        "Found setuptools metadata for {path} in `setup.cfg` ({name})",
-                                        path = path.display(),
-                                        name = name
-                                    );
-                                    return Ok(pep508_rs::Requirement {
-                                        name,
-                                        extras: requirement.extras,
-                                        version_or_url: Some(VersionOrUrl::Url(requirement.url)),
-                                        marker: requirement.marker,
-                                        origin: requirement.origin,
-                                    });
-                                }
+                {
+                    if let Some(section) = setup_cfg.get("metadata") {
+                        if let Some(Some(name)) = section.get("name") {
+                            if let Ok(name) = PackageName::from_str(name) {
+                                debug!(
+                                    "Found setuptools metadata for {path} in `setup.cfg` ({name})",
+                                    path = parsed_path_url.path.display(),
+                                    name = name
+                                );
+                                return Ok(pep508_rs::Requirement {
+                                    name,
+                                    extras: requirement.extras,
+                                    version_or_url: Some(VersionOrUrl::Url(requirement.url)),
+                                    marker: requirement.marker,
+                                    origin: requirement.origin,
+                                });
                             }
                         }
                     }
-
-                    SourceUrl::Directory(DirectorySourceUrl {
-                        url: &requirement.url,
-                        path: Cow::Owned(path),
-                    })
-                } else {
-                    SourceUrl::Path(PathSourceUrl {
-                        url: &requirement.url,
-                        path: Cow::Owned(path),
-                    })
                 }
-            }
-            Some(Scheme::Http | Scheme::Https) => SourceUrl::Direct(DirectSourceUrl {
-                url: &requirement.url,
-            }),
-            Some(Scheme::GitSsh | Scheme::GitHttps | Scheme::GitHttp) => {
-                let git = ParsedGitUrl::try_from(requirement.url.to_url())?;
-                SourceUrl::Git(GitSourceUrl {
-                    git: Cow::Owned(git.url),
-                    subdirectory: git.subdirectory.map(Cow::Owned),
-                    url: &requirement.url,
+
+                SourceUrl::Directory(DirectorySourceUrl {
+                    url: &requirement.url.verbatim,
+                    path: Cow::Borrowed(&parsed_path_url.path),
                 })
             }
-            _ => {
-                return Err(anyhow::anyhow!(
-                    "Unsupported scheme for unnamed requirement: {}",
-                    requirement.url
-                ));
-            }
+            // If it's not a directory, assume it's a file.
+            ParsedUrl::Path(parsed_path_url) => SourceUrl::Path(PathSourceUrl {
+                url: &requirement.url.verbatim,
+                path: Cow::Borrowed(&parsed_path_url.path),
+            }),
+            ParsedUrl::Archive(parsed_archive_url) => SourceUrl::Direct(DirectSourceUrl {
+                url: &parsed_archive_url.url,
+            }),
+            ParsedUrl::Git(parsed_git_url) => SourceUrl::Git(GitSourceUrl {
+                url: &requirement.url.verbatim,
+                git: &parsed_git_url.url,
+                subdirectory: parsed_git_url.subdirectory.as_deref(),
+            }),
         };
 
         // Fetch the metadata for the distribution.
         let name = {
             let id = VersionId::from_url(source.url());
             if let Some(archive) = index
                 .distributions()
```

### Comparing `uv-0.2.2/crates/uv-requirements/src/upgrade.rs` & `uv-0.2.3/crates/uv-requirements/src/upgrade.rs`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         &BaseClientBuilder::new().connectivity(Connectivity::Offline),
     )
     .await?;
     let preferences = requirements_txt
         .requirements
         .into_iter()
         .map(Preference::from_entry)
+        .filter_map(Result::transpose)
         .collect::<Result<Vec<_>, PreferenceError>>()?;
 
     // Apply the upgrade strategy to the requirements.
     Ok(match upgrade {
         // Respect all pinned versions from the existing lockfile.
         Upgrade::None => preferences,
         // Ignore all pinned versions from the existing lockfile.
```

### Comparing `uv-0.2.2/crates/uv-requirements/src/workspace.rs` & `uv-0.2.3/crates/uv-requirements/src/workspace.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pep440-rs/Cargo.toml` & `uv-0.2.3/crates/pep440-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pep440-rs/License-Apache` & `uv-0.2.3/crates/pep440-rs/License-Apache`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pep440-rs/License-BSD` & `uv-0.2.3/crates/pep440-rs/License-BSD`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pep440-rs/Readme.md` & `uv-0.2.3/crates/pep440-rs/Readme.md`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pep440-rs/python/Readme.md` & `uv-0.2.3/crates/pep440-rs/python/Readme.md`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pep440-rs/src/lib.rs` & `uv-0.2.3/crates/pep440-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pep440-rs/src/version.rs` & `uv-0.2.3/crates/pep440-rs/src/version.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pep440-rs/src/version_specifier.rs` & `uv-0.2.3/crates/pep440-rs/src/version_specifier.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/distribution-filename/Cargo.toml` & `uv-0.2.3/crates/distribution-filename/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/distribution-filename/src/lib.rs` & `uv-0.2.3/crates/distribution-filename/src/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 use pep440_rs::Version;
 use std::fmt::{Display, Formatter};
 use std::str::FromStr;
 use uv_normalize::PackageName;
 
+pub use build_tag::{BuildTag, BuildTagError};
 pub use source_dist::{SourceDistExtension, SourceDistFilename, SourceDistFilenameError};
 pub use wheel::{WheelFilename, WheelFilenameError};
 
+mod build_tag;
 mod source_dist;
 mod wheel;
 
 #[derive(Debug, Clone)]
 pub enum DistFilename {
     SourceDistFilename(SourceDistFilename),
     WheelFilename(WheelFilename),
```

### Comparing `uv-0.2.2/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_multiple_tags.snap` & `uv-0.2.3/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_multiple_tags.snap`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 ---
 Ok(
     WheelFilename {
         name: PackageName(
             "foo",
         ),
         version: "1.2.3",
+        build_tag: None,
         python_tag: [
             "ab",
             "cd",
             "ef",
         ],
         abi_tag: [
             "gh",
```

### Comparing `uv-0.2.2/crates/distribution-filename/src/source_dist.rs` & `uv-0.2.3/crates/distribution-filename/src/source_dist.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/distribution-filename/src/wheel.rs` & `uv-0.2.3/crates/distribution-filename/src/wheel.rs`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 use thiserror::Error;
 use url::Url;
 
 use pep440_rs::{Version, VersionParseError};
 use platform_tags::{TagCompatibility, Tags};
 use uv_normalize::{InvalidNameError, PackageName};
 
+use crate::{BuildTag, BuildTagError};
+
 #[derive(Debug, Clone, Eq, PartialEq, Hash, rkyv::Archive, rkyv::Deserialize, rkyv::Serialize)]
 #[archive(check_bytes)]
 #[archive_attr(derive(Debug))]
 pub struct WheelFilename {
     pub name: PackageName,
     pub version: Version,
+    pub build_tag: Option<BuildTag>,
     pub python_tag: Vec<String>,
     pub abi_tag: Vec<String>,
     pub platform_tag: Vec<String>,
 }
 
 impl FromStr for WheelFilename {
     type Err = WheelFilenameError;
@@ -53,24 +56,14 @@
     }
 
     /// Return the [`TagCompatibility`] of the wheel with the given tags
     pub fn compatibility(&self, compatible_tags: &Tags) -> TagCompatibility {
         compatible_tags.compatibility(&self.python_tag, &self.abi_tag, &self.platform_tag)
     }
 
-    /// Get the tag for this wheel.
-    pub fn get_tag(&self) -> String {
-        format!(
-            "{}-{}-{}",
-            self.python_tag.join("."),
-            self.abi_tag.join("."),
-            self.platform_tag.join(".")
-        )
-    }
-
     /// The wheel filename without the extension.
     pub fn stem(&self) -> String {
         format!(
             "{}-{}-{}",
             self.name.as_dist_info_name(),
             self.version,
             self.get_tag()
@@ -78,14 +71,24 @@
     }
 
     /// Parse a wheel filename from the stem (e.g., `foo-1.2.3-py3-none-any`).
     pub fn from_stem(stem: &str) -> Result<Self, WheelFilenameError> {
         Self::parse(stem, stem)
     }
 
+    /// Get the tag for this wheel.
+    fn get_tag(&self) -> String {
+        format!(
+            "{}-{}-{}",
+            self.python_tag.join("."),
+            self.abi_tag.join("."),
+            self.platform_tag.join(".")
+        )
+    }
+
     /// Parse a wheel filename from the stem (e.g., `foo-1.2.3-py3-none-any`).
     ///
     /// The originating `filename` is used for high-fidelity error messages.
     fn parse(stem: &str, filename: &str) -> Result<Self, WheelFilenameError> {
         // The wheel filename should contain either five or six entries. If six, then the third
         // entry is the build tag. If five, then the third entry is the Python tag.
         // https://www.python.org/dev/peps/pep-0427/#file-name-convention
@@ -125,46 +128,55 @@
         let Some(abi_tag_or_platform_tag) = parts.next() else {
             return Err(WheelFilenameError::InvalidWheelFileName(
                 filename.to_string(),
                 "Must have a platform tag".to_string(),
             ));
         };
 
-        let (name, version, python_tag, abi_tag, platform_tag) =
+        let (name, version, build_tag, python_tag, abi_tag, platform_tag) =
             if let Some(platform_tag) = parts.next() {
                 if parts.next().is_some() {
                     return Err(WheelFilenameError::InvalidWheelFileName(
                         filename.to_string(),
                         "Must have 5 or 6 components, but has more".to_string(),
                     ));
                 }
                 (
                     name,
                     version,
+                    Some(build_tag_or_python_tag),
                     python_tag_or_abi_tag,
                     abi_tag_or_platform_tag,
                     platform_tag,
                 )
             } else {
                 (
                     name,
                     version,
+                    None,
                     build_tag_or_python_tag,
                     python_tag_or_abi_tag,
                     abi_tag_or_platform_tag,
                 )
             };
 
         let name = PackageName::from_str(name)
             .map_err(|err| WheelFilenameError::InvalidPackageName(filename.to_string(), err))?;
         let version = Version::from_str(version)
             .map_err(|err| WheelFilenameError::InvalidVersion(filename.to_string(), err))?;
+        let build_tag = build_tag
+            .map(|build_tag| {
+                BuildTag::from_str(build_tag)
+                    .map_err(|err| WheelFilenameError::InvalidBuildTag(filename.to_string(), err))
+            })
+            .transpose()?;
         Ok(Self {
             name,
             version,
+            build_tag,
             python_tag: python_tag.split('.').map(String::from).collect(),
             abi_tag: abi_tag.split('.').map(String::from).collect(),
             platform_tag: platform_tag.split('.').map(String::from).collect(),
         })
     }
 }
 
@@ -210,18 +222,20 @@
     }
 }
 
 #[derive(Error, Debug)]
 pub enum WheelFilenameError {
     #[error("The wheel filename \"{0}\" is invalid: {1}")]
     InvalidWheelFileName(String, String),
-    #[error("The wheel filename \"{0}\" has an invalid version part: {1}")]
+    #[error("The wheel filename \"{0}\" has an invalid version: {1}")]
     InvalidVersion(String, VersionParseError),
     #[error("The wheel filename \"{0}\" has an invalid package name")]
     InvalidPackageName(String, InvalidNameError),
+    #[error("The wheel filename \"{0}\" has an invalid build tag: {1}")]
+    InvalidBuildTag(String, BuildTagError),
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
@@ -272,15 +286,21 @@
         let err = WheelFilename::from_str("f!oo-1.2.3-python-abi-platform.whl").unwrap_err();
         insta::assert_snapshot!(err, @r###"The wheel filename "f!oo-1.2.3-python-abi-platform.whl" has an invalid package name"###);
     }
 
     #[test]
     fn err_invalid_version() {
         let err = WheelFilename::from_str("foo-x.y.z-python-abi-platform.whl").unwrap_err();
-        insta::assert_snapshot!(err, @r###"The wheel filename "foo-x.y.z-python-abi-platform.whl" has an invalid version part: expected version to start with a number, but no leading ASCII digits were found"###);
+        insta::assert_snapshot!(err, @r###"The wheel filename "foo-x.y.z-python-abi-platform.whl" has an invalid version: expected version to start with a number, but no leading ASCII digits were found"###);
+    }
+
+    #[test]
+    fn err_invalid_build_tag() {
+        let err = WheelFilename::from_str("foo-1.2.3-tag-python-abi-platform.whl").unwrap_err();
+        insta::assert_snapshot!(err, @r###"The wheel filename "foo-1.2.3-tag-python-abi-platform.whl" has an invalid build tag: must start with a digit"###);
     }
 
     #[test]
     fn ok_single_tags() {
         insta::assert_debug_snapshot!(WheelFilename::from_str("foo-1.2.3-foo-bar-baz.whl"));
     }
 
@@ -290,15 +310,15 @@
             "foo-1.2.3-ab.cd.ef-gh-ij.kl.mn.op.qr.st.whl"
         ));
     }
 
     #[test]
     fn ok_build_tag() {
         insta::assert_debug_snapshot!(WheelFilename::from_str(
-            "foo-1.2.3-build-python-abi-platform.whl"
+            "foo-1.2.3-12-python-abi-platform.whl"
         ));
     }
 
     #[test]
     fn from_and_to_string() {
         let wheel_names = &[
             "django_allauth-0.51.0-py3-none-any.whl",
```

### Comparing `uv-0.2.2/crates/uv-git/Cargo.toml` & `uv-0.2.3/crates/uv-git/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-git/src/git.rs` & `uv-0.2.3/crates/uv-git/src/git.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-git/src/known_hosts.rs` & `uv-0.2.3/crates/uv-git/src/known_hosts.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-git/src/lib.rs` & `uv-0.2.3/crates/uv-git/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-git/src/sha.rs` & `uv-0.2.3/crates/uv-git/src/sha.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-git/src/source.rs` & `uv-0.2.3/crates/uv-git/src/source.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-git/src/util/errors.rs` & `uv-0.2.3/crates/uv-git/src/util/errors.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-git/src/util/mod.rs` & `uv-0.2.3/crates/uv-git/src/util/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-git/src/util/retry.rs` & `uv-0.2.3/crates/uv-git/src/util/retry.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-workspace/Cargo.toml` & `uv-0.2.3/crates/uv-workspace/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-workspace/src/combine.rs` & `uv-0.2.3/crates/uv-workspace/src/combine.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-workspace/src/settings.rs` & `uv-0.2.3/crates/uv-workspace/src/settings.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-workspace/src/workspace.rs` & `uv-0.2.3/crates/uv-workspace/src/workspace.rs`

 * *Files 0% similar despite different names*

```diff
@@ -148,13 +148,13 @@
 }
 
 #[derive(thiserror::Error, Debug)]
 pub enum WorkspaceError {
     #[error(transparent)]
     Io(#[from] std::io::Error),
 
-    #[error("Failed to parse `{0}`")]
+    #[error("Failed to parse: `{0}`")]
     PyprojectToml(String, #[source] toml::de::Error),
 
-    #[error("Failed to parse `{0}`")]
+    #[error("Failed to parse: `{0}`")]
     UvToml(String, #[source] toml::de::Error),
 }
```

### Comparing `uv-0.2.2/crates/requirements-txt/Cargo.toml` & `uv-0.2.3/crates/requirements-txt/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 
 [lints]
 workspace = true
 
 [dependencies]
 distribution-types = { workspace = true }
 pep508_rs = { workspace = true }
+pypi-types = { workspace = true }
 uv-client = { workspace = true }
 uv-fs = { workspace = true }
 uv-normalize = { workspace = true }
 uv-configuration = { workspace = true }
 uv-warnings = { workspace = true }
 
 fs-err = { workspace = true }
 regex = { workspace = true }
 reqwest = { workspace = true, optional = true }
 reqwest-middleware = { workspace = true, optional = true }
-thiserror = { workspace = true }
 tracing = { workspace = true }
 unscanny = { workspace = true }
 url = { workspace = true }
 
 [features]
 http = ["reqwest", "reqwest-middleware"]
```

### Comparing `uv-0.2.2/crates/requirements-txt/src/lib.rs` & `uv-0.2.3/crates/requirements-txt/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -40,30 +40,29 @@
 use std::path::{Path, PathBuf};
 use std::str::FromStr;
 
 use tracing::instrument;
 use unscanny::{Pattern, Scanner};
 use url::Url;
 
-use distribution_types::{
-    ParsedUrlError, Requirement, UnresolvedRequirement, UnresolvedRequirementSpecification,
-};
+use distribution_types::{Requirement, UnresolvedRequirement, UnresolvedRequirementSpecification};
 use pep508_rs::{
     expand_env_vars, split_scheme, strip_host, Extras, MarkerTree, Pep508Error, Pep508ErrorSource,
     RequirementOrigin, Scheme, VerbatimUrl,
 };
+use pypi_types::VerbatimParsedUrl;
 #[cfg(feature = "http")]
 use uv_client::BaseClient;
 use uv_client::BaseClientBuilder;
 use uv_configuration::{NoBinary, NoBuild, PackageNameSpecifier};
 use uv_fs::{normalize_url_path, Simplified};
 use uv_normalize::ExtraName;
 use uv_warnings::warn_user;
 
-pub use crate::requirement::{RequirementsTxtRequirement, RequirementsTxtRequirementError};
+pub use crate::requirement::RequirementsTxtRequirement;
 
 mod requirement;
 
 /// We emit one of those for each requirements.txt entry
 enum RequirementsTxtStatement {
     /// `-r` inclusion filename
     Requirements {
@@ -199,35 +198,35 @@
     pub fn parse(
         given: &str,
         origin: Option<&Path>,
         working_dir: impl AsRef<Path>,
     ) -> Result<Self, RequirementsTxtParserError> {
         // Identify the markers.
         let (given, marker) = if let Some((requirement, marker)) = Self::split_markers(given) {
-            let marker = MarkerTree::from_str(marker).map_err(|err| {
+            let marker = MarkerTree::parse_str(marker).map_err(|err| {
                 // Map from error on the markers to error on the whole requirement.
                 let err = Pep508Error {
                     message: err.message,
                     start: requirement.len() + err.start,
                     len: err.len,
                     input: given.to_string(),
                 };
                 match err.message {
                     Pep508ErrorSource::String(_) | Pep508ErrorSource::UrlError(_) => {
                         RequirementsTxtParserError::Pep508 {
                             start: err.start,
                             end: err.start + err.len,
-                            source: err,
+                            source: Box::new(err),
                         }
                     }
                     Pep508ErrorSource::UnsupportedRequirement(_) => {
                         RequirementsTxtParserError::UnsupportedRequirement {
                             start: err.start,
                             end: err.start + err.len,
-                            source: err,
+                            source: Box::new(err),
                         }
                     }
                 }
             })?;
             (requirement, Some(marker))
         } else {
             (given, None)
@@ -244,22 +243,22 @@
                     input: given.to_string(),
                 };
                 match err.message {
                     Pep508ErrorSource::String(_) | Pep508ErrorSource::UrlError(_) => {
                         RequirementsTxtParserError::Pep508 {
                             start: err.start,
                             end: err.start + err.len,
-                            source: err,
+                            source: Box::new(err),
                         }
                     }
                     Pep508ErrorSource::UnsupportedRequirement(_) => {
                         RequirementsTxtParserError::UnsupportedRequirement {
                             start: err.start,
                             end: err.start + err.len,
-                            source: err,
+                            source: Box::new(err),
                         }
                     }
                 }
             })?;
             (requirement, extras.into_vec())
         } else {
             (given, vec![])
@@ -399,39 +398,37 @@
     /// Hashes of the downloadable packages.
     pub hashes: Vec<String>,
 }
 
 // We place the impl here instead of next to `UnresolvedRequirementSpecification` because
 // `UnresolvedRequirementSpecification` is defined in `distribution-types` and `requirements-txt`
 // depends on `distribution-types`.
-impl TryFrom<RequirementEntry> for UnresolvedRequirementSpecification {
-    type Error = Box<ParsedUrlError>;
-
-    fn try_from(value: RequirementEntry) -> Result<Self, Self::Error> {
-        Ok(Self {
+impl From<RequirementEntry> for UnresolvedRequirementSpecification {
+    fn from(value: RequirementEntry) -> Self {
+        Self {
             requirement: match value.requirement {
                 RequirementsTxtRequirement::Named(named) => {
-                    UnresolvedRequirement::Named(Requirement::from_pep508(named)?)
+                    UnresolvedRequirement::Named(Requirement::from(named))
                 }
                 RequirementsTxtRequirement::Unnamed(unnamed) => {
                     UnresolvedRequirement::Unnamed(unnamed)
                 }
             },
             hashes: value.hashes,
-        })
+        }
     }
 }
 
 /// Parsed and flattened requirements.txt with requirements and constraints
 #[derive(Debug, Default, Clone, PartialEq, Eq)]
 pub struct RequirementsTxt {
     /// The actual requirements with the hashes.
     pub requirements: Vec<RequirementEntry>,
     /// Constraints included with `-c`.
-    pub constraints: Vec<pep508_rs::Requirement>,
+    pub constraints: Vec<pep508_rs::Requirement<VerbatimParsedUrl>>,
     /// Editables with `-e`.
     pub editables: Vec<EditableRequirement>,
     /// The index URL, specified with `--index-url`.
     pub index_url: Option<VerbatimUrl>,
     /// The extra index URLs, specified with `--extra-index-url`.
     pub extra_index_urls: Vec<VerbatimUrl>,
     /// The find links locations, specified with `--find-links`.
@@ -910,38 +907,18 @@
         .map(|requirement| {
             if let Some(source) = source {
                 requirement.with_origin(RequirementOrigin::File(source.to_path_buf()))
             } else {
                 requirement
             }
         })
-        .map_err(|err| match err {
-            RequirementsTxtRequirementError::ParsedUrl(err) => {
-                RequirementsTxtParserError::ParsedUrl {
-                    source: err,
-                    start,
-                    end,
-                }
-            }
-            RequirementsTxtRequirementError::Pep508(err) => match err.message {
-                Pep508ErrorSource::String(_) | Pep508ErrorSource::UrlError(_) => {
-                    RequirementsTxtParserError::Pep508 {
-                        source: err,
-                        start,
-                        end,
-                    }
-                }
-                Pep508ErrorSource::UnsupportedRequirement(_) => {
-                    RequirementsTxtParserError::UnsupportedRequirement {
-                        source: err,
-                        start,
-                        end,
-                    }
-                }
-            },
+        .map_err(|err| RequirementsTxtParserError::Pep508 {
+            source: err,
+            start,
+            end,
         })?;
 
     let hashes = if has_hashes {
         parse_hashes(content, s)?
     } else {
         Vec::new()
     };
@@ -1064,25 +1041,25 @@
     },
     Parser {
         message: String,
         line: usize,
         column: usize,
     },
     UnsupportedRequirement {
-        source: Pep508Error,
+        source: Box<Pep508Error<VerbatimParsedUrl>>,
         start: usize,
         end: usize,
     },
     Pep508 {
-        source: Pep508Error,
+        source: Box<Pep508Error<VerbatimParsedUrl>>,
         start: usize,
         end: usize,
     },
     ParsedUrl {
-        source: Box<ParsedUrlError>,
+        source: Box<Pep508Error<VerbatimParsedUrl>>,
         start: usize,
         end: usize,
     },
     Subfile {
         source: Box<RequirementsTxtFileError>,
         start: usize,
         end: usize,
```

### Comparing `uv-0.2.2/crates/requirements-txt/src/requirement.rs` & `uv-0.2.3/crates/requirements-txt/src/requirement.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,55 @@
 use std::path::Path;
 
-use thiserror::Error;
-
-use distribution_types::ParsedUrlError;
 use pep508_rs::{
     Pep508Error, Pep508ErrorSource, RequirementOrigin, TracingReporter, UnnamedRequirement,
 };
+use pypi_types::VerbatimParsedUrl;
 
 /// A requirement specifier in a `requirements.txt` file.
 ///
 /// Analog to `SpecifiedRequirement` but with `pep508_rs::Requirement` instead of
 /// `distribution_types::Requirement`.
 #[derive(Hash, Debug, Clone, Eq, PartialEq)]
 pub enum RequirementsTxtRequirement {
     /// The uv-specific superset over PEP 508 requirements specifier incorporating
     /// `tool.uv.sources`.
-    Named(pep508_rs::Requirement),
+    Named(pep508_rs::Requirement<VerbatimParsedUrl>),
     /// A PEP 508-like, direct URL dependency specifier.
-    Unnamed(UnnamedRequirement),
+    Unnamed(UnnamedRequirement<VerbatimParsedUrl>),
 }
 
 impl RequirementsTxtRequirement {
     /// Set the source file containing the requirement.
     #[must_use]
     pub fn with_origin(self, origin: RequirementOrigin) -> Self {
         match self {
             Self::Named(requirement) => Self::Named(requirement.with_origin(origin)),
             Self::Unnamed(requirement) => Self::Unnamed(requirement.with_origin(origin)),
         }
     }
 }
 
-#[derive(Debug, Error)]
-pub enum RequirementsTxtRequirementError {
-    #[error(transparent)]
-    ParsedUrl(#[from] Box<ParsedUrlError>),
-    #[error(transparent)]
-    Pep508(#[from] Pep508Error),
-}
-
 impl RequirementsTxtRequirement {
     /// Parse a requirement as seen in a `requirements.txt` file.
     pub fn parse(
         input: &str,
         working_dir: impl AsRef<Path>,
-    ) -> Result<Self, RequirementsTxtRequirementError> {
+    ) -> Result<Self, Box<Pep508Error<VerbatimParsedUrl>>> {
         // Attempt to parse as a PEP 508-compliant requirement.
         match pep508_rs::Requirement::parse(input, &working_dir) {
             Ok(requirement) => Ok(Self::Named(requirement)),
             Err(err) => match err.message {
                 Pep508ErrorSource::UnsupportedRequirement(_) => {
                     // If that fails, attempt to parse as a direct URL requirement.
                     Ok(Self::Unnamed(UnnamedRequirement::parse(
                         input,
                         &working_dir,
                         &mut TracingReporter,
                     )?))
                 }
-                _ => Err(RequirementsTxtRequirementError::Pep508(err)),
+                _ => Err(err),
             },
         }
+        .map_err(Box::new)
     }
 }
```

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-basic.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-basic.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-a.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-a.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-b.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-b.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-for-poetry.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-for-poetry.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-a.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-a.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-b.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-b.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-poetry-with-hashes.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-poetry-with-hashes.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-small.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-small.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-whitespace.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-small.txt.snap`

 * *Files 19% similar despite different names*

```diff
@@ -4,67 +4,62 @@
 ---
 RequirementsTxt {
     requirements: [
         RequirementEntry {
             requirement: Named(
                 Requirement {
                     name: PackageName(
-                        "numpy",
+                        "tqdm",
                     ),
                     extras: [],
-                    version_or_url: None,
+                    version_or_url: Some(
+                        VersionSpecifier(
+                            VersionSpecifiers(
+                                [
+                                    VersionSpecifier {
+                                        operator: Equal,
+                                        version: "4.65.0",
+                                    },
+                                ],
+                            ),
+                        ),
+                    ),
                     marker: None,
                     origin: Some(
                         File(
-                            "<REQUIREMENTS_DIR>/whitespace.txt",
+                            "<REQUIREMENTS_DIR>/small.txt",
                         ),
                     ),
                 },
             ),
             hashes: [],
         },
         RequirementEntry {
             requirement: Named(
                 Requirement {
                     name: PackageName(
-                        "pandas",
+                        "tomli-w",
                     ),
-                    extras: [
-                        ExtraName(
-                            "tabulate",
-                        ),
-                    ],
+                    extras: [],
                     version_or_url: Some(
-                        Url(
-                            VerbatimUrl {
-                                url: Url {
-                                    scheme: "https",
-                                    cannot_be_a_base: false,
-                                    username: "",
-                                    password: None,
-                                    host: Some(
-                                        Domain(
-                                            "github.com",
-                                        ),
-                                    ),
-                                    port: None,
-                                    path: "/pandas-dev/pandas",
-                                    query: None,
-                                    fragment: None,
-                                },
-                                given: Some(
-                                    "https://github.com/pandas-dev/pandas",
-                                ),
-                            },
+                        VersionSpecifier(
+                            VersionSpecifiers(
+                                [
+                                    VersionSpecifier {
+                                        operator: Equal,
+                                        version: "1.0.0",
+                                    },
+                                ],
+                            ),
                         ),
                     ),
                     marker: None,
                     origin: Some(
                         File(
-                            "<REQUIREMENTS_DIR>/whitespace.txt",
+                            "<REQUIREMENTS_DIR>/small.txt",
                         ),
                     ),
                 },
             ),
             hashes: [],
         },
     ],
```

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-basic.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-basic.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-a.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-a.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-b.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-b.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-for-poetry.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-for-poetry.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-a.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-a.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-b.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-b.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-poetry-with-hashes.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-poetry-with-hashes.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-bare-url.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-whitespace.txt.snap`

 * *Files 14% similar despite different names*

```diff
@@ -1,101 +1,92 @@
 ---
 source: crates/requirements-txt/src/lib.rs
 expression: actual
 ---
 RequirementsTxt {
     requirements: [
         RequirementEntry {
-            requirement: Unnamed(
-                UnnamedRequirement {
-                    url: VerbatimUrl {
-                        url: Url {
-                            scheme: "file",
-                            cannot_be_a_base: false,
-                            username: "",
-                            password: None,
-                            host: None,
-                            port: None,
-                            path: "<REQUIREMENTS_DIR>/scripts/packages/black_editable",
-                            query: None,
-                            fragment: None,
-                        },
-                        given: Some(
-                            "./scripts/packages/black_editable",
-                        ),
-                    },
+            requirement: Named(
+                Requirement {
+                    name: PackageName(
+                        "numpy",
+                    ),
                     extras: [],
+                    version_or_url: None,
                     marker: None,
                     origin: Some(
                         File(
-                            "<REQUIREMENTS_DIR>/bare-url.txt",
+                            "<REQUIREMENTS_DIR>/whitespace.txt",
                         ),
                     ),
                 },
             ),
             hashes: [],
         },
         RequirementEntry {
-            requirement: Unnamed(
-                UnnamedRequirement {
-                    url: VerbatimUrl {
-                        url: Url {
-                            scheme: "file",
-                            cannot_be_a_base: false,
-                            username: "",
-                            password: None,
-                            host: None,
-                            port: None,
-                            path: "<REQUIREMENTS_DIR>/scripts/packages/black_editable",
-                            query: None,
-                            fragment: None,
-                        },
-                        given: Some(
-                            "./scripts/packages/black_editable",
-                        ),
-                    },
+            requirement: Named(
+                Requirement {
+                    name: PackageName(
+                        "pandas",
+                    ),
                     extras: [
                         ExtraName(
-                            "dev",
+                            "tabulate",
                         ),
                     ],
-                    marker: None,
-                    origin: Some(
-                        File(
-                            "<REQUIREMENTS_DIR>/bare-url.txt",
+                    version_or_url: Some(
+                        Url(
+                            VerbatimParsedUrl {
+                                parsed_url: Archive(
+                                    ParsedArchiveUrl {
+                                        url: Url {
+                                            scheme: "https",
+                                            cannot_be_a_base: false,
+                                            username: "",
+                                            password: None,
+                                            host: Some(
+                                                Domain(
+                                                    "github.com",
+                                                ),
+                                            ),
+                                            port: None,
+                                            path: "/pandas-dev/pandas",
+                                            query: None,
+                                            fragment: None,
+                                        },
+                                        subdirectory: None,
+                                    },
+                                ),
+                                verbatim: VerbatimUrl {
+                                    url: Url {
+                                        scheme: "https",
+                                        cannot_be_a_base: false,
+                                        username: "",
+                                        password: None,
+                                        host: Some(
+                                            Domain(
+                                                "github.com",
+                                            ),
+                                        ),
+                                        port: None,
+                                        path: "/pandas-dev/pandas",
+                                        query: None,
+                                        fragment: None,
+                                    },
+                                    given: Some(
+                                        "https://github.com/pandas-dev/pandas",
+                                    ),
+                                },
+                            },
                         ),
                     ),
-                },
-            ),
-            hashes: [],
-        },
-        RequirementEntry {
-            requirement: Unnamed(
-                UnnamedRequirement {
-                    url: VerbatimUrl {
-                        url: Url {
-                            scheme: "file",
-                            cannot_be_a_base: false,
-                            username: "",
-                            password: None,
-                            host: None,
-                            port: None,
-                            path: "/scripts/packages/black_editable",
-                            query: None,
-                            fragment: None,
-                        },
-                        given: Some(
-                            "file:///scripts/packages/black_editable",
-                        ),
-                    },
-                    extras: [],
                     marker: None,
                     origin: Some(
                         File(
-                            "<REQUIREMENTS_DIR>/bare-url.txt",
+                            "<REQUIREMENTS_DIR>/whitespace.txt",
                         ),
                     ),
                 },
             ),
             hashes: [],
         },
     ],
```

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-editable.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-editable.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-whitespace.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-whitespace.txt.snap`

 * *Files 20% similar despite different names*

```diff
@@ -31,33 +31,55 @@
                     extras: [
                         ExtraName(
                             "tabulate",
                         ),
                     ],
                     version_or_url: Some(
                         Url(
-                            VerbatimUrl {
-                                url: Url {
-                                    scheme: "https",
-                                    cannot_be_a_base: false,
-                                    username: "",
-                                    password: None,
-                                    host: Some(
-                                        Domain(
-                                            "github.com",
+                            VerbatimParsedUrl {
+                                parsed_url: Archive(
+                                    ParsedArchiveUrl {
+                                        url: Url {
+                                            scheme: "https",
+                                            cannot_be_a_base: false,
+                                            username: "",
+                                            password: None,
+                                            host: Some(
+                                                Domain(
+                                                    "github.com",
+                                                ),
+                                            ),
+                                            port: None,
+                                            path: "/pandas-dev/pandas",
+                                            query: None,
+                                            fragment: None,
+                                        },
+                                        subdirectory: None,
+                                    },
+                                ),
+                                verbatim: VerbatimUrl {
+                                    url: Url {
+                                        scheme: "https",
+                                        cannot_be_a_base: false,
+                                        username: "",
+                                        password: None,
+                                        host: Some(
+                                            Domain(
+                                                "github.com",
+                                            ),
                                         ),
+                                        port: None,
+                                        path: "/pandas-dev/pandas",
+                                        query: None,
+                                        fragment: None,
+                                    },
+                                    given: Some(
+                                        "https://github.com/pandas-dev/pandas",
                                     ),
-                                    port: None,
-                                    path: "/pandas-dev/pandas",
-                                    query: None,
-                                    fragment: None,
                                 },
-                                given: Some(
-                                    "https://github.com/pandas-dev/pandas",
-                                ),
                             },
                         ),
                     ),
                     marker: None,
                     origin: Some(
                         File(
                             "<REQUIREMENTS_DIR>/whitespace.txt",
```

### Comparing `uv-0.2.2/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-editable.txt.snap` & `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-editable.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/requirements-txt/test-data/requirements-txt/poetry-with-hashes.txt` & `uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/poetry-with-hashes.txt`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-configuration/Cargo.toml` & `uv-0.2.3/crates/uv-configuration/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 [dependencies]
 distribution-types = { workspace = true }
 pep508_rs = { workspace = true }
 platform-tags = { workspace = true }
 uv-auth = { workspace = true }
 uv-normalize = { workspace = true }
 
-anyhow = { workspace = true }
 clap = { workspace = true, features = ["derive"], optional = true }
-itertools = { workspace = true }
+either = { workspace = true }
 rustc-hash = { workspace = true }
 schemars = { workspace = true, optional = true }
 serde = { workspace = true }
 serde_json = { workspace = true }
 tracing = { workspace = true }
 
+[dev-dependencies]
+anyhow = { workspace = true }
+
 [features]
 default = []
```

### Comparing `uv-0.2.2/crates/uv-configuration/src/authentication.rs` & `uv-0.2.3/crates/uv-configuration/src/authentication.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-configuration/src/build_options.rs` & `uv-0.2.3/crates/uv-configuration/src/build_options.rs`

 * *Files 0% similar despite different names*

```diff
@@ -216,14 +216,15 @@
     /// the first index before moving on to the next. Further, if a version is found to be
     /// incompatible in the first index, we do not reconsider that version in subsequent indexes,
     /// even if the secondary index might contain compatible versions (e.g., variants of the same
     /// versions with different ABI tags or Python version constraints).
     ///
     /// See: <https://peps.python.org/pep-0708/>
     #[cfg_attr(feature = "clap", clap(alias = "unsafe-any-match"))]
+    #[serde(alias = "unsafe-any-match")]
     UnsafeFirstMatch,
     /// Search for every package name across all indexes, preferring the "best" version found. If a
     /// package version is in multiple indexes, only look at the entry for the first index.
     ///
     /// In this strategy, we look for every package across all indexes. When resolving, we consider
     /// all versions from all indexes, choosing the "best" version found (typically, the highest
     /// compatible version).
```

### Comparing `uv-0.2.2/crates/uv-configuration/src/concurrency.rs` & `uv-0.2.3/crates/uv-configuration/src/concurrency.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-configuration/src/config_settings.rs` & `uv-0.2.3/crates/uv-configuration/src/config_settings.rs`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     /// The key of the setting. For example, given `key=value`, this would be `key`.
     key: String,
     /// The value of the setting. For example, given `key=value`, this would be `value`.
     value: String,
 }
 
 impl FromStr for ConfigSettingEntry {
-    type Err = anyhow::Error;
+    type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
         let Some((key, value)) = s.split_once('=') else {
-            return Err(anyhow::anyhow!(
+            return Err(format!(
                 "Invalid config setting: {s} (expected `KEY=VALUE`)"
             ));
         };
         Ok(Self {
             key: key.trim().to_string(),
             value: value.trim().to_string(),
         })
```

### Comparing `uv-0.2.2/crates/uv-configuration/src/constraints.rs` & `uv-0.2.3/crates/uv-configuration/src/constraints.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-configuration/src/name_specifiers.rs` & `uv-0.2.3/crates/uv-configuration/src/name_specifiers.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-configuration/src/overrides.rs` & `uv-0.2.3/crates/uv-configuration/src/overrides.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use std::hash::BuildHasherDefault;
 
-use itertools::Either;
+use either::Either;
 use rustc_hash::FxHashMap;
 
 use distribution_types::Requirement;
 use uv_normalize::PackageName;
 
 /// A set of overrides for a set of requirements.
 #[derive(Debug, Default, Clone)]
```

### Comparing `uv-0.2.2/crates/uv-configuration/src/package_options.rs` & `uv-0.2.3/crates/uv-configuration/src/package_options.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-configuration/src/preview.rs` & `uv-0.2.3/crates/uv-configuration/src/preview.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-configuration/src/target_triple.rs` & `uv-0.2.3/crates/uv-configuration/src/target_triple.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pep508-rs/Cargo.toml` & `uv-0.2.3/crates/pep508-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pep508-rs/License-Apache` & `uv-0.2.3/crates/pep508-rs/License-Apache`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pep508-rs/License-BSD` & `uv-0.2.3/crates/pep508-rs/License-BSD`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pep508-rs/Readme.md` & `uv-0.2.3/crates/pep508-rs/Readme.md`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pep508-rs/src/cursor.rs` & `uv-0.2.3/crates/pep508-rs/src/cursor.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pep508-rs/src/lib.rs` & `uv-0.2.3/crates/pep508-rs/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 //! let dependency_specification = Requirement::<VerbatimUrl>::from_str(marker).unwrap();
 //! assert_eq!(dependency_specification.name.as_ref(), "requests");
 //! assert_eq!(dependency_specification.extras, vec![ExtraName::from_str("security").unwrap(), ExtraName::from_str("tests").unwrap()]);
 //! ```
 
 #![warn(missing_docs)]
 
-use cursor::Cursor;
 #[cfg(feature = "pyo3")]
 use std::collections::hash_map::DefaultHasher;
 use std::collections::HashSet;
 use std::error::Error;
 use std::fmt::{Debug, Display, Formatter};
 #[cfg(feature = "pyo3")]
 use std::hash::{Hash, Hasher};
@@ -35,26 +34,26 @@
     pymodule, types::PyModule, IntoPy, PyObject, PyResult, Python,
 };
 use serde::{de, Deserialize, Deserializer, Serialize, Serializer};
 use thiserror::Error;
 use unicode_width::UnicodeWidthChar;
 use url::Url;
 
+use cursor::Cursor;
 pub use marker::{
     ExtraOperator, MarkerEnvironment, MarkerEnvironmentBuilder, MarkerExpression, MarkerOperator,
     MarkerTree, MarkerValue, MarkerValueString, MarkerValueVersion, MarkerWarningKind,
     StringVersion,
 };
+pub use origin::RequirementOrigin;
 #[cfg(feature = "pyo3")]
 use pep440_rs::PyVersion;
 use pep440_rs::{Version, VersionSpecifier, VersionSpecifiers};
 #[cfg(feature = "non-pep508-extensions")]
-pub use unnamed::UnnamedRequirement;
-// Parity with the crates.io version of pep508_rs
-pub use origin::RequirementOrigin;
+pub use unnamed::{UnnamedRequirement, UnnamedRequirementUrl};
 pub use uv_normalize::{ExtraName, InvalidNameError, PackageName};
 pub use verbatim_url::{
     expand_env_vars, split_scheme, strip_host, Scheme, VerbatimUrl, VerbatimUrlError,
 };
 
 mod cursor;
 mod marker;
@@ -119,15 +118,15 @@
             self.input,
             " ".repeat(start_offset),
             "^".repeat(underline_len)
         )
     }
 }
 
-/// We need this to allow e.g. anyhow's `.context()`
+/// We need this to allow anyhow's `.context()` and `AsDynError`.
 impl<E: Error + Debug, T: Pep508Url<Err = E>> std::error::Error for Pep508Error<T> {}
 
 #[cfg(feature = "pyo3")]
 create_exception!(
     pep508,
     PyPep508Error,
     pyo3::exceptions::PyValueError,
@@ -151,25 +150,14 @@
     /// `requests [security,tests] >= 2.8.1, == 2.8.* ; python_version > "3.8"`.
     /// Those are a nested and/or tree.
     pub marker: Option<MarkerTree>,
     /// The source file containing the requirement.
     pub origin: Option<RequirementOrigin>,
 }
 
-impl Requirement {
-    /// Set the source file containing the requirement.
-    #[must_use]
-    pub fn with_origin(self, origin: RequirementOrigin) -> Self {
-        Self {
-            origin: Some(origin),
-            ..self
-        }
-    }
-}
-
 impl<T: Pep508Url + Display> Display for Requirement<T> {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.name)?;
         if !self.extras.is_empty() {
             write!(
                 f,
                 "[{}]",
@@ -449,18 +437,27 @@
             }),
         };
         Self {
             marker: Some(marker),
             ..self
         }
     }
+
+    /// Set the source file containing the requirement.
+    #[must_use]
+    pub fn with_origin(self, origin: RequirementOrigin) -> Self {
+        Self {
+            origin: Some(origin),
+            ..self
+        }
+    }
 }
 
 /// Type to parse URLs from `name @ <url>` into. Defaults to [`url::Url`].
-pub trait Pep508Url: Clone + Display + Debug {
+pub trait Pep508Url: Display + Debug + Sized {
     /// String to URL parsing error
     type Err: Error + Debug;
 
     /// Parse a url from `name @ <url>`. Defaults to [`url::Url::parse_url`].
     fn parse_url(url: &str, working_dir: Option<&Path>) -> Result<Self, Self::Err>;
 }
 
@@ -1132,15 +1129,15 @@
         Requirement::<VerbatimUrl>::from_str(input)
             .unwrap_err()
             .to_string()
     }
 
     #[cfg(feature = "non-pep508-extensions")]
     fn parse_unnamed_err(input: &str) -> String {
-        crate::UnnamedRequirement::from_str(input)
+        crate::UnnamedRequirement::<VerbatimUrl>::from_str(input)
             .unwrap_err()
             .to_string()
     }
 
     #[cfg(windows)]
     #[test]
     fn test_preprocess_url_windows() {
@@ -1252,36 +1249,37 @@
         let numpy = Requirement::<Url>::from_str("numpy >=1.19, <2.0 ").unwrap();
         assert_eq!(numpy.name.as_ref(), "numpy");
     }
 
     #[test]
     #[cfg(feature = "non-pep508-extensions")]
     fn direct_url_no_extras() {
-        let numpy = crate::UnnamedRequirement::from_str("https://files.pythonhosted.org/packages/28/4a/46d9e65106879492374999e76eb85f87b15328e06bd1550668f79f7b18c6/numpy-1.26.4-cp312-cp312-win32.whl").unwrap();
+        let numpy = crate::UnnamedRequirement::<VerbatimUrl>::from_str("https://files.pythonhosted.org/packages/28/4a/46d9e65106879492374999e76eb85f87b15328e06bd1550668f79f7b18c6/numpy-1.26.4-cp312-cp312-win32.whl").unwrap();
         assert_eq!(numpy.url.to_string(), "https://files.pythonhosted.org/packages/28/4a/46d9e65106879492374999e76eb85f87b15328e06bd1550668f79f7b18c6/numpy-1.26.4-cp312-cp312-win32.whl");
         assert_eq!(numpy.extras, vec![]);
     }
 
     #[test]
     #[cfg(all(unix, feature = "non-pep508-extensions"))]
     fn direct_url_extras() {
-        let numpy =
-            crate::UnnamedRequirement::from_str("/path/to/numpy-1.26.4-cp312-cp312-win32.whl[dev]")
-                .unwrap();
+        let numpy = crate::UnnamedRequirement::<VerbatimUrl>::from_str(
+            "/path/to/numpy-1.26.4-cp312-cp312-win32.whl[dev]",
+        )
+        .unwrap();
         assert_eq!(
             numpy.url.to_string(),
             "file:///path/to/numpy-1.26.4-cp312-cp312-win32.whl"
         );
         assert_eq!(numpy.extras, vec![ExtraName::from_str("dev").unwrap()]);
     }
 
     #[test]
     #[cfg(all(windows, feature = "non-pep508-extensions"))]
     fn direct_url_extras() {
-        let numpy = crate::UnnamedRequirement::from_str(
+        let numpy = crate::UnnamedRequirement::<VerbatimUrl>::from_str(
             "C:\\path\\to\\numpy-1.26.4-cp312-cp312-win32.whl[dev]",
         )
         .unwrap();
         assert_eq!(
             numpy.url.to_string(),
             "file:///C:/path/to/numpy-1.26.4-cp312-cp312-win32.whl"
         );
@@ -1455,15 +1453,16 @@
         assert_eq!(pip_url, expected);
     }
 
     #[test]
     fn test_marker_parsing() {
         let marker = r#"python_version == "2.7" and (sys_platform == "win32" or (os_name == "linux" and implementation_name == 'cpython'))"#;
         let actual =
-            parse_markers_cursor::<Url>(&mut Cursor::new(marker), &mut TracingReporter).unwrap();
+            parse_markers_cursor::<VerbatimUrl>(&mut Cursor::new(marker), &mut TracingReporter)
+                .unwrap();
         let expected = MarkerTree::And(vec![
             MarkerTree::Expression(MarkerExpression::Version {
                 key: MarkerValueVersion::PythonVersion,
                 specifier: VersionSpecifier::from_pattern(
                     pep440_rs::Operator::Equal,
                     "2.7".parse().unwrap(),
                 )
```

### Comparing `uv-0.2.2/crates/pep508-rs/src/marker.rs` & `uv-0.2.3/crates/pep508-rs/src/marker.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1546,14 +1546,19 @@
 
     fn from_str(markers: &str) -> Result<Self, Self::Err> {
         parse_markers(markers, &mut TracingReporter)
     }
 }
 
 impl MarkerTree {
+    /// Like [`FromStr::from_str`], but the caller chooses the return type generic.
+    pub fn parse_str<T: Pep508Url>(markers: &str) -> Result<Self, Pep508Error<T>> {
+        parse_markers(markers, &mut TracingReporter)
+    }
+
     /// Parse a [`MarkerTree`] from a string with the given reporter.
     pub fn parse_reporter(
         markers: &str,
         reporter: &mut impl Reporter,
     ) -> Result<Self, Pep508Error> {
         parse_markers(markers, reporter)
     }
```

### Comparing `uv-0.2.2/crates/pep508-rs/src/origin.rs` & `uv-0.2.3/crates/pep508-rs/src/origin.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/pep508-rs/src/unnamed.rs` & `uv-0.2.3/crates/pep508-rs/src/unnamed.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,90 @@
-use std::fmt::{Display, Formatter};
+use std::fmt::{Debug, Display, Formatter};
+use std::hash::Hash;
 use std::path::Path;
 use std::str::FromStr;
 
-use serde::{de, Deserialize, Deserializer, Serialize, Serializer};
-
 use uv_fs::normalize_url_path;
 use uv_normalize::ExtraName;
 
 use crate::marker::parse_markers_cursor;
 use crate::{
     expand_env_vars, parse_extras_cursor, split_extras, split_scheme, strip_host, Cursor,
-    MarkerEnvironment, MarkerTree, Pep508Error, Pep508ErrorSource, Reporter, RequirementOrigin,
-    Scheme, TracingReporter, VerbatimUrl, VerbatimUrlError,
+    MarkerEnvironment, MarkerTree, Pep508Error, Pep508ErrorSource, Pep508Url, Reporter,
+    RequirementOrigin, Scheme, TracingReporter, VerbatimUrl, VerbatimUrlError,
 };
 
+/// An extension over [`Pep508Url`] that also supports parsing unnamed requirements, namely paths.
+///
+/// The error type is fixed to the same as the [`Pep508Url`] impl error.
+pub trait UnnamedRequirementUrl: Pep508Url {
+    /// Parse a URL from a relative or absolute path.
+    fn parse_path(path: impl AsRef<Path>, working_dir: impl AsRef<Path>)
+        -> Result<Self, Self::Err>;
+
+    /// Parse a URL from an absolute path.
+    fn parse_absolute_path(path: impl AsRef<Path>) -> Result<Self, Self::Err>;
+
+    /// Parse a URL from a string.
+    fn parse_unnamed_url(given: impl AsRef<str>) -> Result<Self, Self::Err>;
+
+    /// Set the verbatim representation of the URL.
+    #[must_use]
+    fn with_given(self, given: impl Into<String>) -> Self;
+
+    /// Return the original string as given by the user, if available.
+    fn given(&self) -> Option<&str>;
+}
+
+impl UnnamedRequirementUrl for VerbatimUrl {
+    fn parse_path(
+        path: impl AsRef<Path>,
+        working_dir: impl AsRef<Path>,
+    ) -> Result<Self, VerbatimUrlError> {
+        Self::parse_path(path, working_dir)
+    }
+
+    fn parse_absolute_path(path: impl AsRef<Path>) -> Result<Self, Self::Err> {
+        Self::parse_absolute_path(path)
+    }
+
+    fn parse_unnamed_url(given: impl AsRef<str>) -> Result<Self, Self::Err> {
+        Ok(Self::parse_url(given)?)
+    }
+
+    fn with_given(self, given: impl Into<String>) -> Self {
+        self.with_given(given)
+    }
+
+    fn given(&self) -> Option<&str> {
+        self.given()
+    }
+}
+
 /// A PEP 508-like, direct URL dependency specifier without a package name.
 ///
 /// In a `requirements.txt` file, the name of the package is optional for direct URL
 /// dependencies. This isn't compliant with PEP 508, but is common in `requirements.txt`, which
 /// is implementation-defined.
 #[derive(Hash, Debug, Clone, Eq, PartialEq)]
-pub struct UnnamedRequirement {
+pub struct UnnamedRequirement<Url: UnnamedRequirementUrl = VerbatimUrl> {
     /// The direct URL that defines the version specifier.
-    pub url: VerbatimUrl,
+    pub url: Url,
     /// The list of extras such as `security`, `tests` in
     /// `requests [security,tests] >= 2.8.1, == 2.8.* ; python_version > "3.8"`.
     pub extras: Vec<ExtraName>,
     /// The markers such as `python_version > "3.8"` in
     /// `requests [security,tests] >= 2.8.1, == 2.8.* ; python_version > "3.8"`.
     /// Those are a nested and/or tree.
     pub marker: Option<MarkerTree>,
     /// The source file containing the requirement.
     pub origin: Option<RequirementOrigin>,
 }
 
-impl UnnamedRequirement {
+impl<Url: UnnamedRequirementUrl> UnnamedRequirement<Url> {
     /// Returns whether the markers apply for the given environment
     pub fn evaluate_markers(&self, env: &MarkerEnvironment, extras: &[ExtraName]) -> bool {
         self.evaluate_optional_environment(Some(env), extras)
     }
 
     /// Returns whether the markers apply for the given environment
     pub fn evaluate_optional_environment(
@@ -57,17 +103,30 @@
     #[must_use]
     pub fn with_origin(self, origin: RequirementOrigin) -> Self {
         Self {
             origin: Some(origin),
             ..self
         }
     }
+
+    /// Parse a PEP 508-like direct URL requirement without a package name.
+    pub fn parse(
+        input: &str,
+        working_dir: impl AsRef<Path>,
+        reporter: &mut impl Reporter,
+    ) -> Result<Self, Pep508Error<Url>> {
+        parse_unnamed_requirement(
+            &mut Cursor::new(input),
+            Some(working_dir.as_ref()),
+            reporter,
+        )
+    }
 }
 
-impl Display for UnnamedRequirement {
+impl<Url: UnnamedRequirementUrl> Display for UnnamedRequirement<Url> {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.url)?;
         if !self.extras.is_empty() {
             write!(
                 f,
                 "[{}]",
                 self.extras
@@ -80,71 +139,35 @@
         if let Some(marker) = &self.marker {
             write!(f, " ; {}", marker)?;
         }
         Ok(())
     }
 }
 
-/// <https://github.com/serde-rs/serde/issues/908#issuecomment-298027413>
-impl<'de> Deserialize<'de> for UnnamedRequirement {
-    fn deserialize<D>(deserializer: D) -> Result<Self, D::Error>
-    where
-        D: Deserializer<'de>,
-    {
-        let s = String::deserialize(deserializer)?;
-        FromStr::from_str(&s).map_err(de::Error::custom)
-    }
-}
-
-/// <https://github.com/serde-rs/serde/issues/1316#issue-332908452>
-impl Serialize for UnnamedRequirement {
-    fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
-    where
-        S: Serializer,
-    {
-        serializer.collect_str(self)
-    }
-}
-
-impl FromStr for UnnamedRequirement {
-    type Err = Pep508Error<VerbatimUrl>;
+impl<Url: UnnamedRequirementUrl> FromStr for UnnamedRequirement<Url> {
+    type Err = Pep508Error<Url>;
 
     /// Parse a PEP 508-like direct URL requirement without a package name.
     fn from_str(input: &str) -> Result<Self, Self::Err> {
         parse_unnamed_requirement(&mut Cursor::new(input), None, &mut TracingReporter)
     }
 }
 
-impl UnnamedRequirement {
-    /// Parse a PEP 508-like direct URL requirement without a package name.
-    pub fn parse(
-        input: &str,
-        working_dir: impl AsRef<Path>,
-        reporter: &mut impl Reporter,
-    ) -> Result<Self, Pep508Error<VerbatimUrl>> {
-        parse_unnamed_requirement(
-            &mut Cursor::new(input),
-            Some(working_dir.as_ref()),
-            reporter,
-        )
-    }
-}
-
 /// Parse a PEP 508-like direct URL specifier without a package name.
 ///
 /// Unlike pip, we allow extras on URLs and paths.
-fn parse_unnamed_requirement(
+fn parse_unnamed_requirement<Url: UnnamedRequirementUrl>(
     cursor: &mut Cursor,
     working_dir: Option<&Path>,
     reporter: &mut impl Reporter,
-) -> Result<UnnamedRequirement, Pep508Error<VerbatimUrl>> {
+) -> Result<UnnamedRequirement<Url>, Pep508Error<Url>> {
     cursor.eat_whitespace();
 
     // Parse the URL itself, along with any extras.
-    let (url, extras) = parse_unnamed_url(cursor, working_dir)?;
+    let (url, extras) = parse_unnamed_url::<Url>(cursor, working_dir)?;
     let requirement_end = cursor.pos();
 
     // wsp*
     cursor.eat_whitespace();
     // quoted_marker?
     let marker = if cursor.peek_char() == Some(';') {
         // Skip past the semicolon
@@ -187,21 +210,21 @@
         marker,
         origin: None,
     })
 }
 
 /// Create a `VerbatimUrl` to represent the requirement, and extracts any extras at the end of the
 /// URL, to comply with the non-PEP 508 extensions.
-fn preprocess_unnamed_url(
+fn preprocess_unnamed_url<Url: UnnamedRequirementUrl>(
     url: &str,
     #[cfg_attr(not(feature = "non-pep508-extensions"), allow(unused))] working_dir: Option<&Path>,
     cursor: &Cursor,
     start: usize,
     len: usize,
-) -> Result<(VerbatimUrl, Vec<ExtraName>), Pep508Error<VerbatimUrl>> {
+) -> Result<(Url, Vec<ExtraName>), Pep508Error<Url>> {
     // Split extras _before_ expanding the URL. We assume that the extras are not environment
     // variables. If we parsed the extras after expanding the URL, then the verbatim representation
     // of the URL itself would be ambiguous, since it would consist of the environment variable,
     // which would expand to _more_ than the URL.
     let (url, extras) = if let Some((url, extras)) = split_extras(url) {
         (url, Some(extras))
     } else {
@@ -231,91 +254,89 @@
                 let path = strip_host(path);
 
                 // Transform, e.g., `/C:/Users/ferris/wheel-0.42.0.tar.gz` to `C:\Users\ferris\wheel-0.42.0.tar.gz`.
                 let path = normalize_url_path(path);
 
                 #[cfg(feature = "non-pep508-extensions")]
                 if let Some(working_dir) = working_dir {
-                    let url = VerbatimUrl::parse_path(path.as_ref(), working_dir)
+                    let url = Url::parse_path(path.as_ref(), working_dir)
                         .map_err(|err| Pep508Error {
-                            message: Pep508ErrorSource::<VerbatimUrl>::UrlError(err),
+                            message: Pep508ErrorSource::UrlError(err),
                             start,
                             len,
                             input: cursor.to_string(),
                         })?
                         .with_given(url.to_string());
                     return Ok((url, extras));
                 }
 
-                let url = VerbatimUrl::parse_absolute_path(path.as_ref())
+                let url = Url::parse_absolute_path(path.as_ref())
                     .map_err(|err| Pep508Error {
-                        message: Pep508ErrorSource::<VerbatimUrl>::UrlError(err),
+                        message: Pep508ErrorSource::UrlError(err),
                         start,
                         len,
                         input: cursor.to_string(),
                     })?
                     .with_given(url.to_string());
                 Ok((url, extras))
             }
             // Ex) `https://download.pytorch.org/whl/torch_stable.html`
             Some(_) => {
                 // Ex) `https://download.pytorch.org/whl/torch_stable.html`
-                let url = VerbatimUrl::parse_url(expanded.as_ref())
+                let url = Url::parse_unnamed_url(expanded.as_ref())
                     .map_err(|err| Pep508Error {
-                        message: Pep508ErrorSource::<VerbatimUrl>::UrlError(VerbatimUrlError::Url(
-                            err,
-                        )),
+                        message: Pep508ErrorSource::UrlError(err),
                         start,
                         len,
                         input: cursor.to_string(),
                     })?
                     .with_given(url.to_string());
                 Ok((url, extras))
             }
 
             // Ex) `C:\Users\ferris\wheel-0.42.0.tar.gz`
             _ => {
                 if let Some(working_dir) = working_dir {
-                    let url = VerbatimUrl::parse_path(expanded.as_ref(), working_dir)
+                    let url = Url::parse_path(expanded.as_ref(), working_dir)
                         .map_err(|err| Pep508Error {
-                            message: Pep508ErrorSource::<VerbatimUrl>::UrlError(err),
+                            message: Pep508ErrorSource::UrlError(err),
                             start,
                             len,
                             input: cursor.to_string(),
                         })?
                         .with_given(url.to_string());
                     return Ok((url, extras));
                 }
 
-                let url = VerbatimUrl::parse_absolute_path(expanded.as_ref())
+                let url = Url::parse_absolute_path(expanded.as_ref())
                     .map_err(|err| Pep508Error {
                         message: Pep508ErrorSource::UrlError(err),
                         start,
                         len,
                         input: cursor.to_string(),
                     })?
                     .with_given(url.to_string());
                 Ok((url, extras))
             }
         }
     } else {
         // Ex) `../editable/`
         if let Some(working_dir) = working_dir {
-            let url = VerbatimUrl::parse_path(expanded.as_ref(), working_dir)
+            let url = Url::parse_path(expanded.as_ref(), working_dir)
                 .map_err(|err| Pep508Error {
-                    message: Pep508ErrorSource::<VerbatimUrl>::UrlError(err),
+                    message: Pep508ErrorSource::UrlError(err),
                     start,
                     len,
                     input: cursor.to_string(),
                 })?
                 .with_given(url.to_string());
             return Ok((url, extras));
         }
 
-        let url = VerbatimUrl::parse_absolute_path(expanded.as_ref())
+        let url = Url::parse_absolute_path(expanded.as_ref())
             .map_err(|err| Pep508Error {
                 message: Pep508ErrorSource::UrlError(err),
                 start,
                 len,
                 input: cursor.to_string(),
             })?
             .with_given(url.to_string());
@@ -325,18 +346,18 @@
 
 /// Like [`crate::parse_url`], but allows for extras to be present at the end of the URL, to comply
 /// with the non-PEP 508 extensions.
 ///
 /// For example:
 /// - `https://download.pytorch.org/whl/torch_stable.html[dev]`
 /// - `../editable[dev]`
-fn parse_unnamed_url(
+fn parse_unnamed_url<Url: UnnamedRequirementUrl>(
     cursor: &mut Cursor,
     working_dir: Option<&Path>,
-) -> Result<(VerbatimUrl, Vec<ExtraName>), Pep508Error<VerbatimUrl>> {
+) -> Result<(Url, Vec<ExtraName>), Pep508Error<Url>> {
     // wsp*
     cursor.eat_whitespace();
     // <URI_reference>
     let (start, len) = cursor.take_while(|char| !char.is_whitespace());
     let url = cursor.slice(start, len);
     if url.is_empty() {
         return Err(Pep508Error {
```

### Comparing `uv-0.2.2/crates/pep508-rs/src/verbatim_url.rs` & `uv-0.2.3/crates/pep508-rs/src/verbatim_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-installer/Cargo.toml` & `uv-0.2.3/crates/uv-installer/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-installer/src/compile.rs` & `uv-0.2.3/crates/uv-installer/src/compile.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-installer/src/downloader.rs` & `uv-0.2.3/crates/uv-installer/src/downloader.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-installer/src/editable.rs` & `uv-0.2.3/crates/uv-installer/src/editable.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-installer/src/installer.rs` & `uv-0.2.3/crates/uv-installer/src/installer.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-installer/src/lib.rs` & `uv-0.2.3/crates/uv-installer/src/lib.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pub use compile::{compile_tree, CompileError};
 pub use downloader::{Downloader, Reporter as DownloadReporter};
 pub use editable::{is_dynamic, BuiltEditable, InstalledEditable, ResolvedEditable};
 pub use installer::{Installer, Reporter as InstallReporter};
 pub use plan::{Plan, Planner};
-pub use site_packages::{Diagnostic, SatisfiesResult, SitePackages};
+pub use site_packages::{SatisfiesResult, SitePackages, SitePackagesDiagnostic};
 pub use uninstall::{uninstall, UninstallError};
 
 mod compile;
 mod downloader;
 mod editable;
 mod installer;
 mod plan;
```

### Comparing `uv-0.2.2/crates/uv-installer/src/pip_compileall.py` & `uv-0.2.3/crates/uv-installer/src/pip_compileall.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-installer/src/plan.rs` & `uv-0.2.3/crates/uv-installer/src/plan.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-installer/src/satisfies.rs` & `uv-0.2.3/crates/uv-installer/src/satisfies.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-installer/src/site_packages.rs` & `uv-0.2.3/crates/uv-installer/src/site_packages.rs`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 
 use anyhow::{Context, Result};
 use fs_err as fs;
 use rustc_hash::{FxHashMap, FxHashSet};
 use url::Url;
 
 use distribution_types::{
-    InstalledDist, Name, Requirement, UnresolvedRequirement, UnresolvedRequirementSpecification,
+    Diagnostic, InstalledDist, Name, Requirement, UnresolvedRequirement,
+    UnresolvedRequirementSpecification,
 };
 use pep440_rs::{Version, VersionSpecifiers};
+use pypi_types::VerbatimParsedUrl;
 use requirements_txt::EditableRequirement;
 use uv_cache::{ArchiveTarget, ArchiveTimestamp};
 use uv_interpreter::PythonEnvironment;
 use uv_normalize::PackageName;
 use uv_types::InstalledPackagesProvider;
 
 use crate::is_dynamic;
@@ -184,28 +186,28 @@
 
     /// Returns `true` if there are any installed packages.
     pub fn any(&self) -> bool {
         self.distributions.iter().any(Option::is_some)
     }
 
     /// Validate the installed packages in the virtual environment.
-    pub fn diagnostics(&self) -> Result<Vec<Diagnostic>> {
+    pub fn diagnostics(&self) -> Result<Vec<SitePackagesDiagnostic>> {
         let mut diagnostics = Vec::new();
 
         for (package, indexes) in &self.by_name {
             let mut distributions = indexes.iter().flat_map(|index| &self.distributions[*index]);
 
             // Find the installed distribution for the given package.
             let Some(distribution) = distributions.next() else {
                 continue;
             };
 
             if let Some(conflict) = distributions.next() {
                 // There are multiple installed distributions for the same package.
-                diagnostics.push(Diagnostic::DuplicatePackage {
+                diagnostics.push(SitePackagesDiagnostic::DuplicatePackage {
                     package: package.clone(),
                     paths: std::iter::once(distribution.path().to_owned())
                         .chain(std::iter::once(conflict.path().to_owned()))
                         .chain(distributions.map(|dist| dist.path().to_owned()))
                         .collect(),
                 });
                 continue;
@@ -214,25 +216,25 @@
             for index in indexes {
                 let Some(distribution) = &self.distributions[*index] else {
                     continue;
                 };
 
                 // Determine the dependencies for the given package.
                 let Ok(metadata) = distribution.metadata() else {
-                    diagnostics.push(Diagnostic::IncompletePackage {
+                    diagnostics.push(SitePackagesDiagnostic::IncompletePackage {
                         package: package.clone(),
                         path: distribution.path().to_owned(),
                     });
                     continue;
                 };
 
                 // Verify that the package is compatible with the current Python version.
                 if let Some(requires_python) = metadata.requires_python.as_ref() {
                     if !requires_python.contains(self.venv.interpreter().python_version()) {
-                        diagnostics.push(Diagnostic::IncompatiblePythonVersion {
+                        diagnostics.push(SitePackagesDiagnostic::IncompatiblePythonVersion {
                             package: package.clone(),
                             version: self.venv.interpreter().python_version().clone(),
                             requires_python: requires_python.clone(),
                         });
                     }
                 }
 
@@ -242,34 +244,36 @@
                         continue;
                     }
 
                     let installed = self.get_packages(&dependency.name);
                     match installed.as_slice() {
                         [] => {
                             // No version installed.
-                            diagnostics.push(Diagnostic::MissingDependency {
+                            diagnostics.push(SitePackagesDiagnostic::MissingDependency {
                                 package: package.clone(),
                                 requirement: dependency.clone(),
                             });
                         }
                         [installed] => {
                             match &dependency.version_or_url {
                                 None | Some(pep508_rs::VersionOrUrl::Url(_)) => {
                                     // Nothing to do (accept any installed version).
                                 }
                                 Some(pep508_rs::VersionOrUrl::VersionSpecifier(
                                     version_specifier,
                                 )) => {
                                     // The installed version doesn't satisfy the requirement.
                                     if !version_specifier.contains(installed.version()) {
-                                        diagnostics.push(Diagnostic::IncompatibleDependency {
-                                            package: package.clone(),
-                                            version: installed.version().clone(),
-                                            requirement: dependency.clone(),
-                                        });
+                                        diagnostics.push(
+                                            SitePackagesDiagnostic::IncompatibleDependency {
+                                                package: package.clone(),
+                                                version: installed.version().clone(),
+                                                requirement: dependency.clone(),
+                                            },
+                                        );
                                     }
                                 }
                             }
                         }
                         _ => {
                             // There are multiple installed distributions for the same package.
                         }
@@ -334,17 +338,17 @@
                     // Add the dependencies to the queue.
                     for dependency in metadata.requires_dist {
                         if dependency.evaluate_markers(
                             self.venv.interpreter().markers(),
                             &requirement.extras,
                         ) {
                             let dependency = UnresolvedRequirementSpecification {
-                                requirement: UnresolvedRequirement::Named(
-                                    Requirement::from_pep508(dependency)?,
-                                ),
+                                requirement: UnresolvedRequirement::Named(Requirement::from(
+                                    dependency,
+                                )),
                                 hashes: vec![],
                             };
                             if seen.insert(dependency.clone()) {
                                 stack.push(dependency);
                             }
                         }
                     }
@@ -356,25 +360,27 @@
             }
         }
 
         // Verify that all non-editable requirements are met.
         while let Some(entry) = stack.pop() {
             let installed = match &entry.requirement {
                 UnresolvedRequirement::Named(requirement) => self.get_packages(&requirement.name),
-                UnresolvedRequirement::Unnamed(requirement) => self.get_urls(requirement.url.raw()),
+                UnresolvedRequirement::Unnamed(requirement) => {
+                    self.get_urls(requirement.url.verbatim.raw())
+                }
             };
             match installed.as_slice() {
                 [] => {
                     // The package isn't installed.
                     return Ok(SatisfiesResult::Unsatisfied(entry.requirement.to_string()));
                 }
                 [distribution] => {
                     match RequirementSatisfaction::check(
                         distribution,
-                        entry.requirement.source()?.as_ref(),
+                        entry.requirement.source().as_ref(),
                     )? {
                         RequirementSatisfaction::Mismatch | RequirementSatisfaction::OutOfDate => {
                             return Ok(SatisfiesResult::Unsatisfied(entry.requirement.to_string()))
                         }
                         RequirementSatisfaction::Satisfied => {}
                     }
                     // Validate that the installed version satisfies the constraints.
@@ -398,17 +404,17 @@
                     // Add the dependencies to the queue.
                     for dependency in metadata.requires_dist {
                         if dependency.evaluate_markers(
                             self.venv.interpreter().markers(),
                             entry.requirement.extras(),
                         ) {
                             let dependency = UnresolvedRequirementSpecification {
-                                requirement: UnresolvedRequirement::Named(
-                                    Requirement::from_pep508(dependency)?,
-                                ),
+                                requirement: UnresolvedRequirement::Named(Requirement::from(
+                                    dependency,
+                                )),
                                 hashes: vec![],
                             };
                             if seen.insert(dependency.clone()) {
                                 stack.push(dependency);
                             }
                         }
                     }
@@ -445,15 +451,15 @@
 
     fn into_iter(self) -> Self::IntoIter {
         self.distributions.into_iter().flatten()
     }
 }
 
 #[derive(Debug)]
-pub enum Diagnostic {
+pub enum SitePackagesDiagnostic {
     IncompletePackage {
         /// The package that is missing metadata.
         package: PackageName,
         /// The path to the package.
         path: PathBuf,
     },
     IncompatiblePythonVersion {
@@ -464,35 +470,35 @@
         /// The version of Python that is required.
         requires_python: VersionSpecifiers,
     },
     MissingDependency {
         /// The package that is missing a dependency.
         package: PackageName,
         /// The dependency that is missing.
-        requirement: pep508_rs::Requirement,
+        requirement: pep508_rs::Requirement<VerbatimParsedUrl>,
     },
     IncompatibleDependency {
         /// The package that has an incompatible dependency.
         package: PackageName,
         /// The version of the package that is installed.
         version: Version,
         /// The dependency that is incompatible.
-        requirement: pep508_rs::Requirement,
+        requirement: pep508_rs::Requirement<VerbatimParsedUrl>,
     },
     DuplicatePackage {
         /// The package that has multiple installed distributions.
         package: PackageName,
         /// The installed versions of the package.
         paths: Vec<PathBuf>,
     },
 }
 
-impl Diagnostic {
+impl Diagnostic for SitePackagesDiagnostic {
     /// Convert the diagnostic into a user-facing message.
-    pub fn message(&self) -> String {
+    fn message(&self) -> String {
         match self {
             Self::IncompletePackage { package, path } => format!(
                 "The package `{package}` is broken or incomplete (unable to read `METADATA`). Consider recreating the virtualenv, or removing the package directory at: {}.", path.display(),
             ),
             Self::IncompatiblePythonVersion {
                 package,
                 version,
@@ -521,15 +527,15 @@
                     paths.iter().fold(String::new(), |acc, path| acc + &format!("\n  - {}", path.display()))
                 )
             }
         }
     }
 
     /// Returns `true` if the [`PackageName`] is involved in this diagnostic.
-    pub fn includes(&self, name: &PackageName) -> bool {
+    fn includes(&self, name: &PackageName) -> bool {
         match self {
             Self::IncompletePackage { package, .. } => name == package,
             Self::IncompatiblePythonVersion { package, .. } => name == package,
             Self::MissingDependency { package, .. } => name == package,
             Self::IncompatibleDependency {
                 package,
                 requirement,
```

### Comparing `uv-0.2.2/crates/uv-installer/src/uninstall.rs` & `uv-0.2.3/crates/uv-installer/src/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-fs/Cargo.toml` & `uv-0.2.3/crates/uv-fs/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 
 [dependencies]
 uv-warnings = { workspace = true }
 
 backoff = { workspace = true }
 cachedir = { workspace = true }
 dunce = { workspace = true }
+either = { workspace = true }
 encoding_rs_io = { workspace = true }
 fs-err = { workspace = true }
 fs2 = { workspace = true }
 once_cell = { workspace = true }
 path-absolutize = { workspace = true }
+path-slash = { workspace = true }
 tempfile = { workspace = true }
 tracing = { workspace = true }
 urlencoding = { workspace = true }
 
 [target.'cfg(windows)'.dependencies]
 junction = { workspace = true }
```

### Comparing `uv-0.2.2/crates/uv-fs/src/cachedir.rs` & `uv-0.2.3/crates/uv-fs/src/cachedir.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-fs/src/lib.rs` & `uv-0.2.3/crates/uv-fs/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use std::fmt::Display;
 use std::path::{Path, PathBuf};
 
 use fs2::FileExt;
 use fs_err as fs;
 use tempfile::NamedTempFile;
-use tracing::{debug, error, warn};
+use tracing::{debug, error, trace, warn};
 
 use uv_warnings::warn_user;
 
 pub use crate::path::*;
 
 pub mod cachedir;
 mod path;
@@ -285,17 +285,20 @@
 /// A file lock that is automatically released when dropped.
 #[derive(Debug)]
 pub struct LockedFile(fs_err::File);
 
 impl LockedFile {
     pub fn acquire(path: impl AsRef<Path>, resource: impl Display) -> Result<Self, std::io::Error> {
         let file = fs_err::File::create(path.as_ref())?;
-        debug!("Trying to lock if free: {}", path.as_ref().user_display());
+        trace!("Checking lock for `{resource}`");
         match file.file().try_lock_exclusive() {
-            Ok(()) => Ok(Self(file)),
+            Ok(()) => {
+                debug!("Acquired lock for `{resource}`");
+                Ok(Self(file))
+            }
             Err(err) => {
                 // Log error code and enum kind to help debugging more exotic failures
                 debug!("Try lock error, waiting for exclusive lock: {:?}", err);
                 warn_user!(
                     "Waiting to acquire lock for {} (lockfile: {})",
                     resource,
                     path.user_display(),
```

### Comparing `uv-0.2.2/crates/uv-fs/src/path.rs` & `uv-0.2.3/crates/uv-fs/src/path.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+use either::Either;
 use std::borrow::Cow;
 use std::path::{Component, Path, PathBuf};
 
 use once_cell::sync::Lazy;
+use path_slash::PathExt;
 
 /// The current working directory.
 pub static CWD: Lazy<PathBuf> =
     Lazy::new(|| std::env::current_dir().expect("The current directory must exist"));
 
 /// The current working directory, canonicalized.
 pub static CANONICAL_CWD: Lazy<PathBuf> = Lazy::new(|| {
@@ -21,49 +23,91 @@
     /// On Windows, this will strip the `\\?\` prefix from paths. On other platforms, it's a no-op.
     fn simplified(&self) -> &Path;
 
     /// Render a [`Path`] for display.
     ///
     /// On Windows, this will strip the `\\?\` prefix from paths. On other platforms, it's
     /// equivalent to [`std::path::Display`].
-    fn simplified_display(&self) -> std::path::Display;
+    fn simplified_display(&self) -> impl std::fmt::Display;
 
     /// Canonicalize a path without a `\\?\` prefix on Windows.
     fn simple_canonicalize(&self) -> std::io::Result<PathBuf>;
 
     /// Render a [`Path`] for user-facing display.
     ///
     /// Like [`simplified_display`], but relativizes the path against the current working directory.
-    fn user_display(&self) -> std::path::Display;
+    fn user_display(&self) -> impl std::fmt::Display;
+
+    /// Render a [`Path`] for user-facing display, where the [`Path`] is relative to a base path.
+    ///
+    /// If the [`Path`] is not relative to the base path, will attempt to relativize the path
+    /// against the current working directory.
+    fn user_display_from(&self, base: impl AsRef<Path>) -> impl std::fmt::Display;
+
+    /// Render a [`Path`] for user-facing display using a portable representation.
+    ///
+    /// Like [`user_display`], but uses a portable representation for relative paths.
+    fn portable_display(&self) -> impl std::fmt::Display;
 }
 
 impl<T: AsRef<Path>> Simplified for T {
     fn simplified(&self) -> &Path {
         dunce::simplified(self.as_ref())
     }
 
-    fn simplified_display(&self) -> std::path::Display {
+    fn simplified_display(&self) -> impl std::fmt::Display {
         dunce::simplified(self.as_ref()).display()
     }
 
     fn simple_canonicalize(&self) -> std::io::Result<PathBuf> {
         dunce::canonicalize(self.as_ref())
     }
 
-    fn user_display(&self) -> std::path::Display {
+    fn user_display(&self) -> impl std::fmt::Display {
         let path = dunce::simplified(self.as_ref());
 
         // Attempt to strip the current working directory, then the canonicalized current working
         // directory, in case they differ.
-        path.strip_prefix(CWD.simplified())
-            .unwrap_or_else(|_| {
+        let path = path.strip_prefix(CWD.simplified()).unwrap_or_else(|_| {
+            path.strip_prefix(CANONICAL_CWD.simplified())
+                .unwrap_or(path)
+        });
+
+        path.display()
+    }
+
+    fn user_display_from(&self, base: impl AsRef<Path>) -> impl std::fmt::Display {
+        let path = dunce::simplified(self.as_ref());
+
+        // Attempt to strip the base, then the current working directory, then the canonicalized
+        // current working directory, in case they differ.
+        let path = path.strip_prefix(base.as_ref()).unwrap_or_else(|_| {
+            path.strip_prefix(CWD.simplified()).unwrap_or_else(|_| {
                 path.strip_prefix(CANONICAL_CWD.simplified())
                     .unwrap_or(path)
             })
-            .display()
+        });
+
+        path.display()
+    }
+
+    fn portable_display(&self) -> impl std::fmt::Display {
+        let path = dunce::simplified(self.as_ref());
+
+        // Attempt to strip the current working directory, then the canonicalized current working
+        // directory, in case they differ.
+        let path = path.strip_prefix(CWD.simplified()).unwrap_or_else(|_| {
+            path.strip_prefix(CANONICAL_CWD.simplified())
+                .unwrap_or(path)
+        });
+
+        // Use a portable representation for relative paths.
+        path.to_slash()
+            .map(Either::Left)
+            .unwrap_or_else(|| Either::Right(path.display()))
     }
 }
 
 pub trait PythonExt {
     /// Escape a [`Path`] for use in Python code.
     fn escape_for_python(&self) -> String;
 }
```

### Comparing `uv-0.2.2/crates/uv-dispatch/Cargo.toml` & `uv-0.2.3/crates/uv-dispatch/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-dispatch/src/lib.rs` & `uv-0.2.3/crates/uv-dispatch/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-virtualenv/Cargo.toml` & `uv-0.2.3/crates/uv-virtualenv/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-virtualenv/src/_virtualenv.py` & `uv-0.2.3/crates/uv-virtualenv/src/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-virtualenv/src/activator/activate` & `uv-0.2.3/crates/uv-virtualenv/src/activator/activate`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-virtualenv/src/activator/activate.bat` & `uv-0.2.3/crates/uv-virtualenv/src/activator/activate.bat`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-virtualenv/src/activator/activate.csh` & `uv-0.2.3/crates/uv-virtualenv/src/activator/activate.csh`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-virtualenv/src/activator/activate.fish` & `uv-0.2.3/crates/uv-virtualenv/src/activator/activate.fish`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-virtualenv/src/activator/activate.nu` & `uv-0.2.3/crates/uv-virtualenv/src/activator/activate.nu`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-virtualenv/src/activator/activate.ps1` & `uv-0.2.3/crates/uv-virtualenv/src/activator/activate.ps1`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-virtualenv/src/activator/activate_this.py` & `uv-0.2.3/crates/uv-virtualenv/src/activator/activate_this.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-virtualenv/src/activator/deactivate.bat` & `uv-0.2.3/crates/uv-virtualenv/src/activator/deactivate.bat`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-virtualenv/src/activator/pydoc.bat` & `uv-0.2.3/crates/uv-virtualenv/src/activator/pydoc.bat`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-virtualenv/src/bare.rs` & `uv-0.2.3/crates/uv-virtualenv/src/bare.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-virtualenv/src/lib.rs` & `uv-0.2.3/crates/uv-virtualenv/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/platform-tags/src/platform.rs` & `uv-0.2.3/crates/platform-tags/src/platform.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/platform-tags/src/tags.rs` & `uv-0.2.3/crates/platform-tags/src/tags.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-build/Cargo.toml` & `uv-0.2.3/crates/uv-build/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 [lints]
 workspace = true
 
 [dependencies]
 distribution-types = { workspace = true }
 pep440_rs = { workspace = true }
 pep508_rs = { workspace = true }
+pypi-types = { workspace = true }
 uv-fs = { workspace = true }
 uv-interpreter = { workspace = true }
 uv-types = { workspace = true }
 uv-configuration = { workspace = true }
 uv-virtualenv = { workspace = true }
 
 anyhow = { workspace = true }
```

### Comparing `uv-0.2.2/crates/uv-build/src/lib.rs` & `uv-0.2.3/crates/uv-build/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 use serde::{de, Deserialize, Deserializer};
 use tempfile::{tempdir_in, TempDir};
 use thiserror::Error;
 use tokio::process::Command;
 use tokio::sync::{Mutex, Semaphore};
 use tracing::{debug, info_span, instrument, Instrument};
 
-use distribution_types::{ParsedUrlError, Requirement, Resolution};
+use distribution_types::{Requirement, Resolution};
 use pep440_rs::Version;
 use pep508_rs::PackageName;
+use pypi_types::VerbatimParsedUrl;
 use uv_configuration::{BuildKind, ConfigSettings, SetupPyStrategy};
 use uv_fs::{PythonExt, Simplified};
 use uv_interpreter::{Interpreter, PythonEnvironment};
 use uv_types::{BuildContext, BuildIsolation, SourceBuildTrait};
 
 /// e.g. `pygraphviz/graphviz_wrap.c:3020:10: fatal error: graphviz/cgraph.h: No such file or directory`
 static MISSING_HEADER_RE_GCC: Lazy<Regex> = Lazy::new(|| {
@@ -62,26 +63,24 @@
 static WHEEL_NOT_FOUND_RE: Lazy<Regex> =
     Lazy::new(|| Regex::new(r"error: invalid command 'bdist_wheel'").unwrap());
 
 /// The default backend to use when PEP 517 is used without a `build-system` section.
 static DEFAULT_BACKEND: Lazy<Pep517Backend> = Lazy::new(|| Pep517Backend {
     backend: "setuptools.build_meta:__legacy__".to_string(),
     backend_path: None,
-    requirements: vec![Requirement::from_pep508(
+    requirements: vec![Requirement::from(
         pep508_rs::Requirement::from_str("setuptools >= 40.8.0").unwrap(),
-    )
-    .unwrap()],
+    )],
 });
 
 /// The requirements for `--legacy-setup-py` builds.
 static SETUP_PY_REQUIREMENTS: Lazy<[Requirement; 2]> = Lazy::new(|| {
     [
-        Requirement::from_pep508(pep508_rs::Requirement::from_str("setuptools >= 40.8.0").unwrap())
-            .unwrap(),
-        Requirement::from_pep508(pep508_rs::Requirement::from_str("wheel").unwrap()).unwrap(),
+        Requirement::from(pep508_rs::Requirement::from_str("setuptools >= 40.8.0").unwrap()),
+        Requirement::from(pep508_rs::Requirement::from_str("wheel").unwrap()),
     ]
 });
 
 #[derive(Error, Debug)]
 pub enum Error {
     #[error(transparent)]
     IO(#[from] io::Error),
@@ -112,16 +111,14 @@
         stdout: String,
         stderr: String,
         #[source]
         missing_header_cause: MissingHeaderCause,
     },
     #[error("Failed to build PATH for build script")]
     BuildScriptPath(#[source] env::JoinPathsError),
-    #[error("Failed to parse requirements from build backend")]
-    DirectUrl(#[source] Box<ParsedUrlError>),
 }
 
 #[derive(Debug)]
 pub enum MissingLibrary {
     Header(String),
     Linker(String),
     PythonPackage(String),
@@ -240,15 +237,15 @@
 }
 
 /// The `[build-system]` section of a pyproject.toml as specified in PEP 517.
 #[derive(Deserialize, Debug, Clone, PartialEq, Eq)]
 #[serde(rename_all = "kebab-case")]
 pub struct BuildSystem {
     /// PEP 508 dependencies required to execute the build system.
-    pub requires: Vec<pep508_rs::Requirement>,
+    pub requires: Vec<pep508_rs::Requirement<VerbatimParsedUrl>>,
     /// A string naming a Python object that will be used to perform the build.
     pub build_backend: Option<String>,
     /// Specify that their backend code is hosted in-tree, this key contains a list of directories.
     pub backend_path: Option<BackendPath>,
 }
 
 impl BackendPath {
@@ -597,17 +594,16 @@
                         backend: build_system
                             .build_backend
                             .unwrap_or_else(|| "setuptools.build_meta:__legacy__".to_string()),
                         backend_path: build_system.backend_path,
                         requirements: build_system
                             .requires
                             .into_iter()
-                            .map(Requirement::from_pep508)
-                            .collect::<Result<_, _>>()
-                            .map_err(|err| Box::new(Error::DirectUrl(err)))?,
+                            .map(Requirement::from)
+                            .collect(),
                     }
                 } else {
                     // If a `pyproject.toml` is present, but `[build-system]` is missing, proceed with
                     // a PEP 517 build using the default backend, to match `pip` and `build`.
                     default_backend.clone()
                 };
                 Ok((Some(backend), pyproject_toml.project))
@@ -978,28 +974,24 @@
             ),
             &output,
             version_id,
         )
     })?;
 
     // Deserialize the requirements from the output file.
-    let extra_requires: Vec<pep508_rs::Requirement> = serde_json::from_slice::<Vec<pep508_rs::Requirement>>(&contents).map_err(|err| {
+    let extra_requires: Vec<pep508_rs::Requirement<VerbatimParsedUrl>> = serde_json::from_slice::<Vec<pep508_rs::Requirement<VerbatimParsedUrl>>>(&contents).map_err(|err| {
         Error::from_command_output(
             format!(
                 "Build backend failed to return extra requires with `get_requires_for_build_{build_kind}`: {err}"
             ),
             &output,
             version_id,
         )
     })?;
-    let extra_requires: Vec<_> = extra_requires
-        .into_iter()
-        .map(Requirement::from_pep508)
-        .collect::<Result<_, _>>()
-        .map_err(Error::DirectUrl)?;
+    let extra_requires: Vec<_> = extra_requires.into_iter().map(Requirement::from).collect();
 
     // Some packages (such as tqdm 4.66.1) list only extra requires that have already been part of
     // the pyproject.toml requires (in this case, `wheel`). We can skip doing the whole resolution
     // and installation again.
     // TODO(konstin): Do we still need this when we have a fast resolver?
     if extra_requires
         .iter()
```

### Comparing `uv-0.2.2/crates/uv-cache/Cargo.toml` & `uv-0.2.3/crates/uv-cache/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-cache/src/cli.rs` & `uv-0.2.3/crates/uv-cache/src/cli.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-cache/src/lib.rs` & `uv-0.2.3/crates/uv-cache/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -610,15 +610,15 @@
 impl CacheBucket {
     fn to_str(self) -> &'static str {
         match self {
             Self::BuiltWheels => "built-wheels-v3",
             Self::FlatIndex => "flat-index-v0",
             Self::Git => "git-v0",
             Self::Interpreter => "interpreter-v1",
-            Self::Simple => "simple-v7",
+            Self::Simple => "simple-v8",
             Self::Wheels => "wheels-v1",
             Self::Archive => "archive-v0",
         }
     }
 
     /// Remove a package from the cache bucket.
     ///
```

### Comparing `uv-0.2.2/crates/uv-cache/src/removal.rs` & `uv-0.2.3/crates/uv-cache/src/removal.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-cache/src/timestamp.rs` & `uv-0.2.3/crates/uv-cache/src/timestamp.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-cache/src/wheel.rs` & `uv-0.2.3/crates/uv-cache/src/wheel.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-distribution/Cargo.toml` & `uv-0.2.3/crates/uv-distribution/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-distribution/src/archive.rs` & `uv-0.2.3/crates/uv-distribution/src/archive.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-distribution/src/distribution_database.rs` & `uv-0.2.3/crates/uv-distribution/src/distribution_database.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-distribution/src/download.rs` & `uv-0.2.3/crates/uv-distribution/src/download.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-distribution/src/error.rs` & `uv-0.2.3/crates/uv-distribution/src/error.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 use std::path::PathBuf;
 
 use tokio::task::JoinError;
 use zip::result::ZipError;
 
 use distribution_filename::WheelFilenameError;
-use distribution_types::ParsedUrlError;
 use pep440_rs::Version;
 use pypi_types::HashDigest;
 use uv_client::BetterReqwestError;
 use uv_fs::Simplified;
 use uv_normalize::PackageName;
 
 #[derive(Debug, thiserror::Error)]
@@ -24,16 +23,14 @@
     #[error("Expected an absolute path, but received: {}", _0.user_display())]
     RelativePath(PathBuf),
     #[error(transparent)]
     JoinRelativeUrl(#[from] pypi_types::JoinRelativeError),
     #[error("Git operation failed")]
     Git(#[source] anyhow::Error),
     #[error(transparent)]
-    DirectUrl(#[from] Box<ParsedUrlError>),
-    #[error(transparent)]
     Reqwest(#[from] BetterReqwestError),
     #[error(transparent)]
     Client(#[from] uv_client::Error),
 
     // Cache writing error
     #[error("Failed to read from the distribution cache")]
     CacheRead(#[source] std::io::Error),
```

### Comparing `uv-0.2.2/crates/uv-distribution/src/git.rs` & `uv-0.2.3/crates/uv-distribution/src/git.rs`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 use fs_err::tokio as fs;
 use once_cell::sync::Lazy;
 use rustc_hash::FxHashMap;
 use tracing::debug;
 use url::Url;
 
 use cache_key::{CanonicalUrl, RepositoryUrl};
-use distribution_types::ParsedGitUrl;
+use pypi_types::ParsedGitUrl;
 use uv_cache::{Cache, CacheBucket};
 use uv_fs::LockedFile;
 use uv_git::{Fetch, GitReference, GitSha, GitSource, GitUrl};
 
 use crate::error::Error;
 use crate::reporter::Facade;
 use crate::Reporter;
```

### Comparing `uv-0.2.2/crates/uv-distribution/src/index/built_wheel_index.rs` & `uv-0.2.3/crates/uv-distribution/src/index/built_wheel_index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-distribution/src/index/cached_wheel.rs` & `uv-0.2.3/crates/uv-distribution/src/index/cached_wheel.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-distribution/src/index/registry_wheel_index.rs` & `uv-0.2.3/crates/uv-distribution/src/index/registry_wheel_index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-distribution/src/lib.rs` & `uv-0.2.3/crates/uv-distribution/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-distribution/src/locks.rs` & `uv-0.2.3/crates/uv-distribution/src/locks.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-distribution/src/reporter.rs` & `uv-0.2.3/crates/uv-distribution/src/reporter.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-distribution/src/source/built_wheel_metadata.rs` & `uv-0.2.3/crates/uv-distribution/src/source/built_wheel_metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-distribution/src/source/mod.rs` & `uv-0.2.3/crates/uv-distribution/src/source/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -13,20 +13,19 @@
 use tracing::{debug, info_span, instrument, Instrument};
 use url::Url;
 use zip::ZipArchive;
 
 use distribution_filename::WheelFilename;
 use distribution_types::{
     BuildableSource, DirectorySourceDist, DirectorySourceUrl, Dist, FileLocation, GitSourceUrl,
-    HashPolicy, Hashed, LocalEditable, ParsedArchiveUrl, PathSourceUrl, RemoteSource, SourceDist,
-    SourceUrl,
+    HashPolicy, Hashed, LocalEditable, PathSourceUrl, RemoteSource, SourceDist, SourceUrl,
 };
 use install_wheel_rs::metadata::read_archive_metadata;
 use platform_tags::Tags;
-use pypi_types::{HashDigest, Metadata23};
+use pypi_types::{HashDigest, Metadata23, ParsedArchiveUrl};
 use uv_cache::{
     ArchiveTimestamp, CacheBucket, CacheEntry, CacheShard, CachedByTimestamp, Freshness, Timestamp,
     WheelCache,
 };
 use uv_client::{
     CacheControl, CachedClientError, Connectivity, DataWithCachePolicy, RegistryClient,
 };
@@ -1022,27 +1021,25 @@
         // Before running the build, check that the hashes match.
         if hashes.is_validate() {
             return Err(Error::HashesNotSupportedGit(source.to_string()));
         }
 
         // Resolve to a precise Git SHA.
         let url = if let Some(url) = resolve_precise(
-            &resource.git,
+            resource.git,
             self.build_context.cache(),
             self.reporter.as_ref(),
         )
         .await?
         {
             Cow::Owned(url)
         } else {
-            Cow::Borrowed(resource.git.as_ref())
+            Cow::Borrowed(resource.git)
         };
 
-        let subdirectory = resource.subdirectory.as_deref();
-
         // Fetch the Git repository.
         let fetch =
             fetch_git_archive(&url, self.build_context.cache(), self.reporter.as_ref()).await?;
 
         let git_sha = fetch.git().precise().expect("Exact commit after checkout");
         let cache_shard = self.build_context.cache().shard(
             CacheBucket::BuiltWheels,
@@ -1058,15 +1055,15 @@
 
         let task = self
             .reporter
             .as_ref()
             .map(|reporter| reporter.on_build_start(source));
 
         let (disk_filename, filename, metadata) = self
-            .build_distribution(source, fetch.path(), subdirectory, &cache_shard)
+            .build_distribution(source, fetch.path(), resource.subdirectory, &cache_shard)
             .await?;
 
         if let Some(task) = task {
             if let Some(reporter) = self.reporter.as_ref() {
                 reporter.on_build_complete(source, task);
             }
         }
@@ -1098,27 +1095,25 @@
         // Before running the build, check that the hashes match.
         if hashes.is_validate() {
             return Err(Error::HashesNotSupportedGit(source.to_string()));
         }
 
         // Resolve to a precise Git SHA.
         let url = if let Some(url) = resolve_precise(
-            &resource.git,
+            resource.git,
             self.build_context.cache(),
             self.reporter.as_ref(),
         )
         .await?
         {
             Cow::Owned(url)
         } else {
-            Cow::Borrowed(resource.git.as_ref())
+            Cow::Borrowed(resource.git)
         };
 
-        let subdirectory = resource.subdirectory.as_deref();
-
         // Fetch the Git repository.
         let fetch =
             fetch_git_archive(&url, self.build_context.cache(), self.reporter.as_ref()).await?;
 
         let git_sha = fetch.git().precise().expect("Exact commit after checkout");
         let cache_shard = self.build_context.cache().shard(
             CacheBucket::BuiltWheels,
@@ -1139,15 +1134,15 @@
                 debug!("Using cached metadata for: {source}");
                 return Ok(ArchiveMetadata::from(metadata));
             }
         }
 
         // If the backend supports `prepare_metadata_for_build_wheel`, use it.
         if let Some(metadata) = self
-            .build_metadata(source, fetch.path(), subdirectory)
+            .build_metadata(source, fetch.path(), resource.subdirectory)
             .boxed_local()
             .await?
         {
             // Store the metadata.
             fs::create_dir_all(metadata_entry.dir())
                 .await
                 .map_err(Error::CacheWrite)?;
@@ -1161,15 +1156,15 @@
         // Otherwise, we need to build a wheel.
         let task = self
             .reporter
             .as_ref()
             .map(|reporter| reporter.on_build_start(source));
 
         let (_disk_filename, _filename, metadata) = self
-            .build_distribution(source, fetch.path(), subdirectory, &cache_shard)
+            .build_distribution(source, fetch.path(), resource.subdirectory, &cache_shard)
             .await?;
 
         if let Some(task) = task {
             if let Some(reporter) = self.reporter.as_ref() {
                 reporter.on_build_complete(source, task);
             }
         }
```

### Comparing `uv-0.2.2/crates/uv-distribution/src/source/revision.rs` & `uv-0.2.3/crates/uv-distribution/src/source/revision.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-normalize/src/extra_name.rs` & `uv-0.2.3/crates/uv-normalize/src/extra_name.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-normalize/src/lib.rs` & `uv-0.2.3/crates/uv-normalize/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-normalize/src/package_name.rs` & `uv-0.2.3/crates/uv-normalize/src/package_name.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/Cargo.toml` & `uv-0.2.3/crates/uv-resolver/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/candidate_selector.rs` & `uv-0.2.3/crates/uv-resolver/src/candidate_selector.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/dependency_mode.rs` & `uv-0.2.3/crates/uv-resolver/src/dependency_mode.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/dependency_provider.rs` & `uv-0.2.3/crates/uv-resolver/src/dependency_provider.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/editables.rs` & `uv-0.2.3/crates/uv-resolver/src/editables.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/error.rs` & `uv-0.2.3/crates/uv-resolver/src/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 use indexmap::IndexMap;
 use pubgrub::range::Range;
 use pubgrub::report::{DefaultStringReporter, DerivationTree, External, Reporter};
 use rustc_hash::{FxHashMap, FxHashSet};
 
 use dashmap::DashMap;
-use distribution_types::{BuiltDist, IndexLocations, InstalledDist, ParsedUrlError, SourceDist};
+use distribution_types::{BuiltDist, IndexLocations, InstalledDist, SourceDist};
 use pep440_rs::Version;
 use pep508_rs::Requirement;
 use uv_normalize::PackageName;
 
 use crate::candidate_selector::CandidateSelector;
 use crate::dependency_provider::UvDependencyProvider;
 use crate::pubgrub::{PubGrubPackage, PubGrubPackageInner, PubGrubPython, PubGrubReportFormatter};
@@ -92,18 +92,14 @@
 
     #[error("Attempted to construct an invalid version specifier")]
     InvalidVersion(#[from] pep440_rs::VersionSpecifierBuildError),
 
     #[error("In `--require-hashes` mode, all requirements must be pinned upfront with `==`, but found: `{0}`")]
     UnhashedPackage(PackageName),
 
-    // TODO(konsti): Attach the distribution that contained the invalid requirement as error source.
-    #[error("Failed to parse requirements")]
-    DirectUrl(#[from] Box<ParsedUrlError>),
-
     /// Something unexpected happened.
     #[error("{0}")]
     Failure(String),
 }
 
 impl<T> From<tokio::sync::mpsc::error::SendError<T>> for ResolveError {
     /// Drop the value we want to send to not leak the private type we're sending.
```

### Comparing `uv-0.2.2/crates/uv-resolver/src/exclude_newer.rs` & `uv-0.2.3/crates/uv-resolver/src/exclude_newer.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/exclusions.rs` & `uv-0.2.3/crates/uv-resolver/src/exclusions.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/flat_index.rs` & `uv-0.2.3/crates/uv-resolver/src/flat_index.rs`

 * *Files 6% similar despite different names*

```diff
@@ -171,28 +171,31 @@
         let priority = match filename.compatibility(tags) {
             TagCompatibility::Incompatible(tag) => {
                 return WheelCompatibility::Incompatible(IncompatibleWheel::Tag(tag))
             }
             TagCompatibility::Compatible(priority) => priority,
         };
 
-        // Check if hashes line up
+        // Check if hashes line up.
         let hash = if let HashPolicy::Validate(required) = hasher.get_package(&filename.name) {
             if hashes.is_empty() {
                 HashComparison::Missing
             } else if required.iter().any(|hash| hashes.contains(hash)) {
                 HashComparison::Matched
             } else {
                 HashComparison::Mismatched
             }
         } else {
             HashComparison::Matched
         };
 
-        WheelCompatibility::Compatible(hash, priority)
+        // Break ties with the build tag.
+        let build_tag = filename.build_tag.clone();
+
+        WheelCompatibility::Compatible(hash, priority, build_tag)
     }
 
     /// Get the [`FlatDistributions`] for the given package name.
     pub fn get(&self, package_name: &PackageName) -> Option<&FlatDistributions> {
         self.index.get(package_name)
     }
```

### Comparing `uv-0.2.2/crates/uv-resolver/src/lib.rs` & `uv-0.2.3/crates/uv-resolver/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/lock.rs` & `uv-0.2.3/crates/uv-resolver/src/lock.rs`

 * *Files 0% similar despite different names*

```diff
@@ -8,22 +8,21 @@
 
 use rustc_hash::FxHashMap;
 use url::Url;
 
 use distribution_filename::WheelFilename;
 use distribution_types::{
     BuiltDist, DirectUrlBuiltDist, DirectUrlSourceDist, DirectorySourceDist, Dist, FileLocation,
-    GitSourceDist, IndexUrl, ParsedArchiveUrl, ParsedGitUrl, PathBuiltDist, PathSourceDist,
-    RegistryBuiltDist, RegistryBuiltWheel, RegistrySourceDist, RemoteSource, Resolution,
-    ResolvedDist, ToUrlError,
+    GitSourceDist, IndexUrl, PathBuiltDist, PathSourceDist, RegistryBuiltDist, RegistryBuiltWheel,
+    RegistrySourceDist, RemoteSource, Resolution, ResolvedDist, ToUrlError,
 };
 use pep440_rs::Version;
 use pep508_rs::{MarkerEnvironment, VerbatimUrl};
 use platform_tags::{TagCompatibility, TagPriority, Tags};
-use pypi_types::HashDigest;
+use pypi_types::{HashDigest, ParsedArchiveUrl, ParsedGitUrl};
 use uv_git::{GitReference, GitSha};
 use uv_normalize::PackageName;
 
 use crate::resolution::AnnotatedDist;
 
 #[derive(Clone, Debug, serde::Deserialize, serde::Serialize)]
 #[serde(into = "LockWire", try_from = "LockWire")]
```

### Comparing `uv-0.2.2/crates/uv-resolver/src/manifest.rs` & `uv-0.2.3/crates/uv-resolver/src/manifest.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/marker.rs` & `uv-0.2.3/crates/uv-resolver/src/marker.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/options.rs` & `uv-0.2.3/crates/uv-resolver/src/options.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/pins.rs` & `uv-0.2.3/crates/uv-resolver/src/pins.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/preferences.rs` & `uv-0.2.3/crates/uv-resolver/src/preferences.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 use std::str::FromStr;
 use std::sync::Arc;
 
 use rustc_hash::FxHashMap;
 use tracing::trace;
 
-use distribution_types::{ParsedUrlError, Requirement, RequirementSource};
+use distribution_types::{Requirement, RequirementSource};
 use pep440_rs::{Operator, Version};
-use pep508_rs::{MarkerEnvironment, UnnamedRequirement};
+use pep508_rs::MarkerEnvironment;
 use pypi_types::{HashDigest, HashError};
 use requirements_txt::{RequirementEntry, RequirementsTxtRequirement};
 use uv_normalize::PackageName;
 
 #[derive(thiserror::Error, Debug)]
 pub enum PreferenceError {
-    #[error("direct URL requirements without package names are not supported: `{0}`")]
-    Bare(UnnamedRequirement),
     #[error(transparent)]
     Hash(#[from] HashError),
-    #[error(transparent)]
-    ParsedUrl(#[from] Box<ParsedUrlError>),
 }
 
 /// A pinned requirement, as extracted from a `requirements.txt` file.
 #[derive(Clone, Debug)]
 pub struct Preference {
     requirement: Requirement,
     hashes: Vec<HashDigest>,
 }
 
 impl Preference {
     /// Create a [`Preference`] from a [`RequirementEntry`].
-    pub fn from_entry(entry: RequirementEntry) -> Result<Self, PreferenceError> {
-        Ok(Self {
+    pub fn from_entry(entry: RequirementEntry) -> Result<Option<Self>, PreferenceError> {
+        Ok(Some(Self {
             requirement: match entry.requirement {
-                RequirementsTxtRequirement::Named(requirement) => {
-                    Requirement::from_pep508(requirement)?
-                }
-                RequirementsTxtRequirement::Unnamed(requirement) => {
-                    return Err(PreferenceError::Bare(requirement));
+                RequirementsTxtRequirement::Named(requirement) => Requirement::from(requirement),
+                RequirementsTxtRequirement::Unnamed(_) => {
+                    return Ok(None);
                 }
             },
             hashes: entry
                 .hashes
                 .iter()
                 .map(String::as_str)
                 .map(HashDigest::from_str)
                 .collect::<Result<_, _>>()?,
-        })
+        }))
     }
 
     /// Create a [`Preference`] from a [`Requirement`].
     pub fn from_requirement(requirement: Requirement) -> Self {
         Self {
             requirement,
             hashes: Vec::new(),
```

### Comparing `uv-0.2.2/crates/uv-resolver/src/prerelease_mode.rs` & `uv-0.2.3/crates/uv-resolver/src/prerelease_mode.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/pubgrub/dependencies.rs` & `uv-0.2.3/crates/uv-resolver/src/pubgrub/dependencies.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/pubgrub/distribution.rs` & `uv-0.2.3/crates/uv-resolver/src/pubgrub/distribution.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-use distribution_types::{DistributionMetadata, Name, VerbatimParsedUrl, VersionOrUrlRef};
+use distribution_types::{DistributionMetadata, Name, VersionOrUrlRef};
 use pep440_rs::Version;
+use pypi_types::VerbatimParsedUrl;
 use uv_normalize::PackageName;
 
 #[derive(Debug)]
 pub(crate) enum PubGrubDistribution<'a> {
     Registry(&'a PackageName, &'a Version),
     Url(&'a PackageName, &'a VerbatimParsedUrl),
 }
```

### Comparing `uv-0.2.2/crates/uv-resolver/src/pubgrub/mod.rs` & `uv-0.2.3/crates/uv-resolver/src/pubgrub/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/pubgrub/package.rs` & `uv-0.2.3/crates/uv-resolver/src/pubgrub/package.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-use distribution_types::VerbatimParsedUrl;
 use pep508_rs::MarkerTree;
+use pypi_types::VerbatimParsedUrl;
 use std::fmt::{Display, Formatter};
 use std::ops::Deref;
 use std::sync::Arc;
 use uv_normalize::{ExtraName, PackageName};
 
 use crate::resolver::Urls;
```

### Comparing `uv-0.2.2/crates/uv-resolver/src/pubgrub/priority.rs` & `uv-0.2.3/crates/uv-resolver/src/pubgrub/priority.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/pubgrub/report.rs` & `uv-0.2.3/crates/uv-resolver/src/pubgrub/report.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/pubgrub/specifier.rs` & `uv-0.2.3/crates/uv-resolver/src/pubgrub/specifier.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/python_requirement.rs` & `uv-0.2.3/crates/uv-resolver/src/python_requirement.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/redirect.rs` & `uv-0.2.3/crates/uv-resolver/src/redirect.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use url::Url;
 
-use distribution_types::{ParsedGitUrl, ParsedUrl, VerbatimParsedUrl};
 use pep508_rs::VerbatimUrl;
+use pypi_types::{ParsedGitUrl, ParsedUrl, VerbatimParsedUrl};
 use uv_distribution::git_url_to_precise;
 use uv_git::GitReference;
 
 /// Given a [`VerbatimUrl`] and a redirect, apply the redirect to the URL while preserving as much
 /// of the verbatim representation as possible.
 fn apply_redirect(url: &VerbatimUrl, redirect: Url) -> VerbatimUrl {
     let redirect = VerbatimUrl::from_url(redirect);
```

### Comparing `uv-0.2.2/crates/uv-resolver/src/resolution/display.rs` & `uv-0.2.3/crates/uv-resolver/src/resolution/display.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/resolution/graph.rs` & `uv-0.2.3/crates/uv-resolver/src/resolution/graph.rs`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 use pubgrub::range::Range;
 use pubgrub::solver::{Kind, State};
 use pubgrub::type_aliases::SelectedDependencies;
 use rustc_hash::{FxHashMap, FxHashSet};
 
 use distribution_types::{
-    Diagnostic, Dist, DistributionMetadata, Name, ParsedUrlError, Requirement, ResolvedDist,
-    VersionId, VersionOrUrlRef,
+    Dist, DistributionMetadata, Name, Requirement, ResolutionDiagnostic, ResolvedDist, VersionId,
+    VersionOrUrlRef,
 };
 use pep440_rs::{Version, VersionSpecifier};
 use pep508_rs::MarkerEnvironment;
-use pypi_types::Yanked;
+use pypi_types::{ParsedUrlError, Yanked};
 use uv_normalize::PackageName;
 
 use crate::dependency_provider::UvDependencyProvider;
 use crate::editables::Editables;
 use crate::pins::FilePins;
 use crate::preferences::Preferences;
 use crate::pubgrub::{PubGrubDistribution, PubGrubPackageInner};
@@ -33,15 +33,15 @@
 #[derive(Debug)]
 pub struct ResolutionGraph {
     /// The underlying graph.
     pub(crate) petgraph: petgraph::graph::Graph<AnnotatedDist, Range<Version>, petgraph::Directed>,
     /// The set of editable requirements in this resolution.
     pub(crate) editables: Editables,
     /// Any diagnostics that were encountered while building the graph.
-    pub(crate) diagnostics: Vec<Diagnostic>,
+    pub(crate) diagnostics: Vec<ResolutionDiagnostic>,
 }
 
 impl ResolutionGraph {
     /// Create a new graph from the resolved PubGrub state.
     #[allow(clippy::too_many_arguments)]
     pub(crate) fn from_state(
         selection: &SelectedDependencies<UvDependencyProvider>,
@@ -86,15 +86,15 @@
                             .push(extra.clone());
                     } else {
                         let dist = pins
                             .get(name, version)
                             .unwrap_or_else(|| panic!("Every package should be pinned: {name:?}"))
                             .clone();
 
-                        diagnostics.push(Diagnostic::MissingExtra {
+                        diagnostics.push(ResolutionDiagnostic::MissingExtra {
                             dist,
                             extra: extra.clone(),
                         });
                     }
                 }
                 PubGrubPackageInner::Package {
                     name,
@@ -107,15 +107,15 @@
                             extras
                                 .entry(name.clone())
                                 .or_insert_with(Vec::new)
                                 .push(extra.clone());
                         } else {
                             let dist = Dist::from_editable(name.clone(), editable.built.clone())?;
 
-                            diagnostics.push(Diagnostic::MissingExtra {
+                            diagnostics.push(ResolutionDiagnostic::MissingExtra {
                                 dist: dist.into(),
                                 extra: extra.clone(),
                             });
                         }
                     } else {
                         let dist = PubGrubDistribution::from_url(name, url);
 
@@ -137,15 +137,15 @@
                             extras
                                 .entry(name.clone())
                                 .or_insert_with(Vec::new)
                                 .push(extra.clone());
                         } else {
                             let dist = Dist::from_url(name.clone(), url_to_precise(url.clone()))?;
 
-                            diagnostics.push(Diagnostic::MissingExtra {
+                            diagnostics.push(ResolutionDiagnostic::MissingExtra {
                                 dist: dist.into(),
                                 extra: extra.clone(),
                             });
                         }
                     }
                 }
                 _ => {}
@@ -173,21 +173,21 @@
                         .expect("Every package should be pinned")
                         .clone();
 
                     // Track yanks for any registry distributions.
                     match dist.yanked() {
                         None | Some(Yanked::Bool(false)) => {}
                         Some(Yanked::Bool(true)) => {
-                            diagnostics.push(Diagnostic::YankedVersion {
+                            diagnostics.push(ResolutionDiagnostic::YankedVersion {
                                 dist: dist.clone(),
                                 reason: None,
                             });
                         }
                         Some(Yanked::Reason(reason)) => {
-                            diagnostics.push(Diagnostic::YankedVersion {
+                            diagnostics.push(ResolutionDiagnostic::YankedVersion {
                                 dist: dist.clone(),
                                 reason: Some(reason.clone()),
                             });
                         }
                     }
 
                     // Extract the hashes, preserving those that were already present in the
@@ -407,16 +407,16 @@
         self.petgraph
             .into_nodes_edges()
             .0
             .into_iter()
             .map(|node| node.weight.dist)
     }
 
-    /// Return the [`Diagnostic`]s that were encountered while building the graph.
-    pub fn diagnostics(&self) -> &[Diagnostic] {
+    /// Return the [`ResolutionDiagnostic`]s that were encountered while building the graph.
+    pub fn diagnostics(&self) -> &[ResolutionDiagnostic] {
         &self.diagnostics
     }
 
     /// Return the marker tree specific to this resolution.
     ///
     /// This accepts a manifest, in-memory-index and marker environment. All
     /// of which should be the same values given to the resolver that produced
@@ -508,16 +508,16 @@
                 )
             };
             let requirements: Vec<_> = archive
                 .metadata
                 .requires_dist
                 .iter()
                 .cloned()
-                .map(Requirement::from_pep508)
-                .collect::<anyhow::Result<_, _>>()?;
+                .map(Requirement::from)
+                .collect();
             for req in manifest.apply(requirements.iter()) {
                 let Some(ref marker_tree) = req.marker else {
                     continue;
                 };
                 add_marker_params_from_tree(marker_tree, &mut seen_marker_values);
             }
         }
```

### Comparing `uv-0.2.2/crates/uv-resolver/src/resolution/mod.rs` & `uv-0.2.3/crates/uv-resolver/src/resolution/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -31,53 +31,55 @@
     /// format.
     ///
     /// This typically results in a PEP 508 representation of the requirement, but will write an
     /// unnamed requirement for relative paths, which can't be represented with PEP 508 (but are
     /// supported in `requirements.txt`).
     pub(crate) fn to_requirements_txt(&self, include_extras: bool) -> Cow<str> {
         // If the URL is not _definitively_ an absolute `file://` URL, write it as a relative path.
-        if let VersionOrUrlRef::Url(url) = self.dist.version_or_url() {
-            let given = url.verbatim();
-            match split_scheme(&given) {
-                Some((scheme, path)) => {
-                    match Scheme::parse(scheme) {
-                        Some(Scheme::File) => {
-                            if path
-                                .strip_prefix("//localhost")
-                                .filter(|path| path.starts_with('/'))
-                                .is_some()
-                            {
-                                // Always absolute; nothing to do.
-                            } else if let Some(path) = path.strip_prefix("//") {
-                                // Strip the prefix, to convert, e.g., `file://flask-3.0.3-py3-none-any.whl` to `flask-3.0.3-py3-none-any.whl`.
-                                //
-                                // However, we should allow any of the following:
-                                // - `file://flask-3.0.3-py3-none-any.whl`
-                                // - `file://C:\Users\user\flask-3.0.3-py3-none-any.whl`
-                                // - `file:///C:\Users\user\flask-3.0.3-py3-none-any.whl`
-                                if !path.starts_with("${PROJECT_ROOT}")
-                                    && !Path::new(path).has_root()
+        if self.dist.is_local() {
+            if let VersionOrUrlRef::Url(url) = self.dist.version_or_url() {
+                let given = url.verbatim();
+                match split_scheme(&given) {
+                    Some((scheme, path)) => {
+                        match Scheme::parse(scheme) {
+                            Some(Scheme::File) => {
+                                if path
+                                    .strip_prefix("//localhost")
+                                    .filter(|path| path.starts_with('/'))
+                                    .is_some()
                                 {
-                                    return Cow::Owned(path.to_string());
+                                    // Always absolute; nothing to do.
+                                } else if let Some(path) = path.strip_prefix("//") {
+                                    // Strip the prefix, to convert, e.g., `file://flask-3.0.3-py3-none-any.whl` to `flask-3.0.3-py3-none-any.whl`.
+                                    //
+                                    // However, we should allow any of the following:
+                                    // - `file:///flask-3.0.3-py3-none-any.whl`
+                                    // - `file://C:\Users\user\flask-3.0.3-py3-none-any.whl`
+                                    // - `file:///C:\Users\user\flask-3.0.3-py3-none-any.whl`
+                                    if !path.starts_with("${PROJECT_ROOT}")
+                                        && !Path::new(path).has_root()
+                                    {
+                                        return Cow::Owned(path.to_string());
+                                    }
+                                } else {
+                                    // Ex) `file:./flask-3.0.3-py3-none-any.whl`
+                                    return given;
                                 }
-                            } else {
-                                // Ex) `file:./flask-3.0.3-py3-none-any.whl`
+                            }
+                            Some(_) => {}
+                            None => {
+                                // Ex) `flask @ C:\Users\user\flask-3.0.3-py3-none-any.whl`
                                 return given;
                             }
                         }
-                        Some(_) => {}
-                        None => {
-                            // Ex) `flask @ C:\Users\user\flask-3.0.3-py3-none-any.whl`
-                            return given;
-                        }
                     }
-                }
-                None => {
-                    // Ex) `flask @ flask-3.0.3-py3-none-any.whl`
-                    return given;
+                    None => {
+                        // Ex) `flask @ flask-3.0.3-py3-none-any.whl`
+                        return given;
+                    }
                 }
             }
         }
 
         if self.extras.is_empty() || !include_extras {
             self.dist.verbatim()
         } else {
```

### Comparing `uv-0.2.2/crates/uv-resolver/src/resolution_mode.rs` & `uv-0.2.3/crates/uv-resolver/src/resolution_mode.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/resolver/batch_prefetch.rs` & `uv-0.2.3/crates/uv-resolver/src/resolver/batch_prefetch.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/resolver/index.rs` & `uv-0.2.3/crates/uv-resolver/src/resolver/index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/resolver/locals.rs` & `uv-0.2.3/crates/uv-resolver/src/resolver/locals.rs`

 * *Files 0% similar despite different names*

```diff
@@ -199,17 +199,18 @@
 #[cfg(test)]
 mod tests {
     use std::str::FromStr;
 
     use anyhow::Result;
     use url::Url;
 
-    use distribution_types::{ParsedUrl, RequirementSource};
+    use distribution_types::RequirementSource;
     use pep440_rs::{Operator, Version, VersionSpecifier, VersionSpecifiers};
     use pep508_rs::VerbatimUrl;
+    use pypi_types::ParsedUrl;
 
     use crate::resolver::locals::{iter_locals, Locals};
 
     #[test]
     fn extract_locals() -> Result<()> {
         // Extract from a source distribution in a URL.
         let url = VerbatimUrl::from_url(Url::parse("https://example.com/foo-1.0.0+local.tar.gz")?);
```

### Comparing `uv-0.2.2/crates/uv-resolver/src/resolver/mod.rs` & `uv-0.2.3/crates/uv-resolver/src/resolver/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1059,16 +1059,16 @@
                 // Determine if the distribution is editable.
                 if let Some(editable) = self.editables.get(name) {
                     let requirements: Vec<_> = editable
                         .metadata
                         .requires_dist
                         .iter()
                         .cloned()
-                        .map(Requirement::from_pep508)
-                        .collect::<Result<_, _>>()?;
+                        .map(Requirement::from)
+                        .collect();
                     let dependencies = PubGrubDependencies::from_requirements(
                         &requirements,
                         &self.constraints,
                         &self.overrides,
                         Some(name),
                         extra.as_ref(),
                         &self.urls,
@@ -1166,16 +1166,16 @@
                     }
                 };
 
                 let requirements: Vec<_> = metadata
                     .requires_dist
                     .iter()
                     .cloned()
-                    .map(Requirement::from_pep508)
-                    .collect::<Result<_, _>>()?;
+                    .map(Requirement::from)
+                    .collect();
                 let dependencies = PubGrubDependencies::from_requirements(
                     &requirements,
                     &self.constraints,
                     &self.overrides,
                     Some(name),
                     extra.as_ref(),
                     &self.urls,
```

### Comparing `uv-0.2.2/crates/uv-resolver/src/resolver/provider.rs` & `uv-0.2.3/crates/uv-resolver/src/resolver/provider.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/resolver/reporter.rs` & `uv-0.2.3/crates/uv-resolver/src/resolver/reporter.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/src/resolver/urls.rs` & `uv-0.2.3/crates/uv-resolver/src/resolver/urls.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
+use distribution_types::{RequirementSource, Verbatim};
 use rustc_hash::FxHashMap;
 use tracing::debug;
 
-use distribution_types::{
-    ParsedArchiveUrl, ParsedGitUrl, ParsedPathUrl, ParsedUrl, RequirementSource, Verbatim,
-    VerbatimParsedUrl,
-};
 use pep508_rs::{MarkerEnvironment, VerbatimUrl};
+use pypi_types::{ParsedArchiveUrl, ParsedGitUrl, ParsedPathUrl, ParsedUrl, VerbatimParsedUrl};
 use uv_distribution::is_same_reference;
 use uv_git::GitUrl;
 use uv_normalize::PackageName;
 
 use crate::{DependencyMode, Manifest, ResolveError};
 
 /// A map of package names to their associated, required URLs.
```

### Comparing `uv-0.2.2/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_optional_missing.snap` & `uv-0.2.3/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_optional_missing.snap`

 * *Files 12% similar despite different names*

```diff
@@ -52,14 +52,15 @@
                         ),
                         size: None,
                         filename: WheelFilename {
                             name: PackageName(
                                 "anyio",
                             ),
                             version: "4.3.0",
+                            build_tag: None,
                             python_tag: [
                                 "py3",
                             ],
                             abi_tag: [
                                 "none",
                             ],
                             platform_tag: [
```

### Comparing `uv-0.2.2/crates/uv-resolver/src/version_map.rs` & `uv-0.2.3/crates/uv-resolver/src/version_map.rs`

 * *Files 0% similar despite different names*

```diff
@@ -550,15 +550,18 @@
             {
                 HashComparison::Matched
             } else {
                 HashComparison::Mismatched
             }
         };
 
-        WheelCompatibility::Compatible(hash, priority)
+        // Break ties with the build tag.
+        let build_tag = filename.build_tag.clone();
+
+        WheelCompatibility::Compatible(hash, priority, build_tag)
     }
 }
 
 /// Represents a possibly initialized [`PrioritizedDist`] for
 /// a single version of a package.
 #[derive(Debug)]
 enum LazyPrioritizedDist {
```

### Comparing `uv-0.2.2/crates/uv-resolver/src/yanks.rs` & `uv-0.2.3/crates/uv-resolver/src/yanks.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-resolver/tests/resolver.rs` & `uv-0.2.3/crates/uv-resolver/tests/resolver.rs`

 * *Files 4% similar despite different names*

```diff
@@ -163,18 +163,17 @@
         let snapshot = anstream::adapter::strip_str(&format!("{}", $value)).to_string();
         insta::assert_snapshot!(&snapshot, @$snapshot)
     };
 }
 
 #[tokio::test]
 async fn black() -> Result<()> {
-    let manifest = Manifest::simple(vec![Requirement::from_pep508(
+    let manifest = Manifest::simple(vec![Requirement::from(
         pep508_rs::Requirement::from_str("black<=23.9.1").unwrap(),
-    )
-    .unwrap()]);
+    )]);
     let options = OptionsBuilder::new()
         .exclude_newer(Some(*EXCLUDE_NEWER))
         .build();
 
     let resolution = resolve(manifest, options, &MARKERS_311, &TAGS_311).await?;
 
     assert_snapshot!(DisplayResolutionGraph::from(&resolution), @r###"
@@ -192,18 +191,17 @@
     "###);
 
     Ok(())
 }
 
 #[tokio::test]
 async fn black_colorama() -> Result<()> {
-    let manifest = Manifest::simple(vec![Requirement::from_pep508(
+    let manifest = Manifest::simple(vec![Requirement::from(
         pep508_rs::Requirement::from_str("black[colorama]<=23.9.1").unwrap(),
-    )
-    .unwrap()]);
+    )]);
     let options = OptionsBuilder::new()
         .exclude_newer(Some(*EXCLUDE_NEWER))
         .build();
 
     let resolution = resolve(manifest, options, &MARKERS_311, &TAGS_311).await?;
 
     assert_snapshot!(DisplayResolutionGraph::from(&resolution), @r###"
@@ -224,18 +222,17 @@
 
     Ok(())
 }
 
 /// Resolve Black with an invalid extra. The resolver should ignore the extra.
 #[tokio::test]
 async fn black_tensorboard() -> Result<()> {
-    let manifest = Manifest::simple(vec![Requirement::from_pep508(
+    let manifest = Manifest::simple(vec![Requirement::from(
         pep508_rs::Requirement::from_str("black[tensorboard]<=23.9.1").unwrap(),
-    )
-    .unwrap()]);
+    )]);
     let options = OptionsBuilder::new()
         .exclude_newer(Some(*EXCLUDE_NEWER))
         .build();
 
     let resolution = resolve(manifest, options, &MARKERS_311, &TAGS_311).await?;
 
     assert_snapshot!(DisplayResolutionGraph::from(&resolution), @r###"
@@ -253,18 +250,17 @@
     "###);
 
     Ok(())
 }
 
 #[tokio::test]
 async fn black_python_310() -> Result<()> {
-    let manifest = Manifest::simple(vec![Requirement::from_pep508(
+    let manifest = Manifest::simple(vec![Requirement::from(
         pep508_rs::Requirement::from_str("black<=23.9.1").unwrap(),
-    )
-    .unwrap()]);
+    )]);
     let options = OptionsBuilder::new()
         .exclude_newer(Some(*EXCLUDE_NEWER))
         .build();
 
     let resolution = resolve(manifest, options, &MARKERS_310, &TAGS_310).await?;
 
     assert_snapshot!(DisplayResolutionGraph::from(&resolution), @r###"
@@ -289,22 +285,20 @@
 }
 
 /// Resolve `black` with a constraint on `mypy-extensions`, to ensure that constraints are
 /// respected.
 #[tokio::test]
 async fn black_mypy_extensions() -> Result<()> {
     let manifest = Manifest::new(
-        vec![
-            Requirement::from_pep508(pep508_rs::Requirement::from_str("black<=23.9.1").unwrap())
-                .unwrap(),
-        ],
-        Constraints::from_requirements(vec![Requirement::from_pep508(
+        vec![Requirement::from(
+            pep508_rs::Requirement::from_str("black<=23.9.1").unwrap(),
+        )],
+        Constraints::from_requirements(vec![Requirement::from(
             pep508_rs::Requirement::from_str("mypy-extensions<0.4.4").unwrap(),
-        )
-        .unwrap()]),
+        )]),
         Overrides::default(),
         vec![],
         None,
         vec![],
         Exclusions::default(),
         vec![],
     );
@@ -332,22 +326,20 @@
 }
 
 /// Resolve `black` with a constraint on `mypy-extensions[extra]`, to ensure that extras are
 /// ignored when resolving constraints.
 #[tokio::test]
 async fn black_mypy_extensions_extra() -> Result<()> {
     let manifest = Manifest::new(
-        vec![
-            Requirement::from_pep508(pep508_rs::Requirement::from_str("black<=23.9.1").unwrap())
-                .unwrap(),
-        ],
-        Constraints::from_requirements(vec![Requirement::from_pep508(
+        vec![Requirement::from(
+            pep508_rs::Requirement::from_str("black<=23.9.1").unwrap(),
+        )],
+        Constraints::from_requirements(vec![Requirement::from(
             pep508_rs::Requirement::from_str("mypy-extensions[extra]<0.4.4").unwrap(),
-        )
-        .unwrap()]),
+        )]),
         Overrides::default(),
         vec![],
         None,
         vec![],
         Exclusions::default(),
         vec![],
     );
@@ -375,22 +367,20 @@
 }
 
 /// Resolve `black` with a redundant constraint on `flake8`, to ensure that constraints don't
 /// introduce new dependencies.
 #[tokio::test]
 async fn black_flake8() -> Result<()> {
     let manifest = Manifest::new(
-        vec![
-            Requirement::from_pep508(pep508_rs::Requirement::from_str("black<=23.9.1").unwrap())
-                .unwrap(),
-        ],
-        Constraints::from_requirements(vec![Requirement::from_pep508(
+        vec![Requirement::from(
+            pep508_rs::Requirement::from_str("black<=23.9.1").unwrap(),
+        )],
+        Constraints::from_requirements(vec![Requirement::from(
             pep508_rs::Requirement::from_str("flake8<1").unwrap(),
-        )
-        .unwrap()]),
+        )]),
         Overrides::default(),
         vec![],
         None,
         vec![],
         Exclusions::default(),
         vec![],
     );
@@ -415,18 +405,17 @@
     "###);
 
     Ok(())
 }
 
 #[tokio::test]
 async fn black_lowest() -> Result<()> {
-    let manifest = Manifest::simple(vec![Requirement::from_pep508(
+    let manifest = Manifest::simple(vec![Requirement::from(
         pep508_rs::Requirement::from_str("black>21").unwrap(),
-    )
-    .unwrap()]);
+    )]);
     let options = OptionsBuilder::new()
         .resolution_mode(ResolutionMode::Lowest)
         .exclude_newer(Some(*EXCLUDE_NEWER))
         .build();
 
     let resolution = resolve(manifest, options, &MARKERS_311, &TAGS_311).await?;
 
@@ -445,18 +434,17 @@
     "###);
 
     Ok(())
 }
 
 #[tokio::test]
 async fn black_lowest_direct() -> Result<()> {
-    let manifest = Manifest::simple(vec![Requirement::from_pep508(
+    let manifest = Manifest::simple(vec![Requirement::from(
         pep508_rs::Requirement::from_str("black>21").unwrap(),
-    )
-    .unwrap()]);
+    )]);
     let options = OptionsBuilder::new()
         .resolution_mode(ResolutionMode::LowestDirect)
         .exclude_newer(Some(*EXCLUDE_NEWER))
         .build();
 
     let resolution = resolve(manifest, options, &MARKERS_311, &TAGS_311).await?;
 
@@ -476,20 +464,22 @@
 
     Ok(())
 }
 
 #[tokio::test]
 async fn black_respect_preference() -> Result<()> {
     let manifest = Manifest::new(
-        vec![Requirement::from_pep508(pep508_rs::Requirement::from_str("black<=23.9.1")?).unwrap()],
+        vec![Requirement::from(pep508_rs::Requirement::from_str(
+            "black<=23.9.1",
+        )?)],
         Constraints::default(),
         Overrides::default(),
-        vec![Preference::from_requirement(
-            Requirement::from_pep508(pep508_rs::Requirement::from_str("black==23.9.0")?).unwrap(),
-        )],
+        vec![Preference::from_requirement(Requirement::from(
+            pep508_rs::Requirement::from_str("black==23.9.0")?,
+        ))],
         None,
         vec![],
         Exclusions::default(),
         vec![],
     );
 
     let options = OptionsBuilder::new()
@@ -514,20 +504,22 @@
 
     Ok(())
 }
 
 #[tokio::test]
 async fn black_ignore_preference() -> Result<()> {
     let manifest = Manifest::new(
-        vec![Requirement::from_pep508(pep508_rs::Requirement::from_str("black<=23.9.1")?).unwrap()],
+        vec![Requirement::from(pep508_rs::Requirement::from_str(
+            "black<=23.9.1",
+        )?)],
         Constraints::default(),
         Overrides::default(),
-        vec![Preference::from_requirement(
-            Requirement::from_pep508(pep508_rs::Requirement::from_str("black==23.9.2")?).unwrap(),
-        )],
+        vec![Preference::from_requirement(Requirement::from(
+            pep508_rs::Requirement::from_str("black==23.9.2")?,
+        ))],
         None,
         vec![],
         Exclusions::default(),
         vec![],
     );
     let options = OptionsBuilder::new()
         .exclude_newer(Some(*EXCLUDE_NEWER))
@@ -550,18 +542,17 @@
     "###);
 
     Ok(())
 }
 
 #[tokio::test]
 async fn black_disallow_prerelease() -> Result<()> {
-    let manifest = Manifest::simple(vec![Requirement::from_pep508(
+    let manifest = Manifest::simple(vec![Requirement::from(
         pep508_rs::Requirement::from_str("black<=20.0").unwrap(),
-    )
-    .unwrap()]);
+    )]);
     let options = OptionsBuilder::new()
         .prerelease_mode(PreReleaseMode::Disallow)
         .exclude_newer(Some(*EXCLUDE_NEWER))
         .build();
 
     let err = resolve(manifest, options, &MARKERS_311, &TAGS_311)
         .await
@@ -574,18 +565,17 @@
     "###);
 
     Ok(())
 }
 
 #[tokio::test]
 async fn black_allow_prerelease_if_necessary() -> Result<()> {
-    let manifest = Manifest::simple(vec![Requirement::from_pep508(
+    let manifest = Manifest::simple(vec![Requirement::from(
         pep508_rs::Requirement::from_str("black<=20.0").unwrap(),
-    )
-    .unwrap()]);
+    )]);
     let options = OptionsBuilder::new()
         .prerelease_mode(PreReleaseMode::IfNecessary)
         .exclude_newer(Some(*EXCLUDE_NEWER))
         .build();
 
     let err = resolve(manifest, options, &MARKERS_311, &TAGS_311)
         .await
@@ -598,18 +588,17 @@
     "###);
 
     Ok(())
 }
 
 #[tokio::test]
 async fn pylint_disallow_prerelease() -> Result<()> {
-    let manifest = Manifest::simple(vec![Requirement::from_pep508(
+    let manifest = Manifest::simple(vec![Requirement::from(
         pep508_rs::Requirement::from_str("pylint==2.3.0").unwrap(),
-    )
-    .unwrap()]);
+    )]);
     let options = OptionsBuilder::new()
         .prerelease_mode(PreReleaseMode::Disallow)
         .exclude_newer(Some(*EXCLUDE_NEWER))
         .build();
 
     let resolution = resolve(manifest, options, &MARKERS_311, &TAGS_311).await?;
 
@@ -624,18 +613,17 @@
     "###);
 
     Ok(())
 }
 
 #[tokio::test]
 async fn pylint_allow_prerelease() -> Result<()> {
-    let manifest = Manifest::simple(vec![Requirement::from_pep508(
+    let manifest = Manifest::simple(vec![Requirement::from(
         pep508_rs::Requirement::from_str("pylint==2.3.0").unwrap(),
-    )
-    .unwrap()]);
+    )]);
     let options = OptionsBuilder::new()
         .prerelease_mode(PreReleaseMode::Allow)
         .exclude_newer(Some(*EXCLUDE_NEWER))
         .build();
 
     let resolution = resolve(manifest, options, &MARKERS_311, &TAGS_311).await?;
 
@@ -651,18 +639,16 @@
 
     Ok(())
 }
 
 #[tokio::test]
 async fn pylint_allow_explicit_prerelease_without_marker() -> Result<()> {
     let manifest = Manifest::simple(vec![
-        Requirement::from_pep508(pep508_rs::Requirement::from_str("pylint==2.3.0").unwrap())
-            .unwrap(),
-        Requirement::from_pep508(pep508_rs::Requirement::from_str("isort>=5.0.0").unwrap())
-            .unwrap(),
+        Requirement::from(pep508_rs::Requirement::from_str("pylint==2.3.0").unwrap()),
+        Requirement::from(pep508_rs::Requirement::from_str("isort>=5.0.0").unwrap()),
     ]);
     let options = OptionsBuilder::new()
         .prerelease_mode(PreReleaseMode::Explicit)
         .exclude_newer(Some(*EXCLUDE_NEWER))
         .build();
 
     let resolution = resolve(manifest, options, &MARKERS_311, &TAGS_311).await?;
@@ -679,18 +665,16 @@
 
     Ok(())
 }
 
 #[tokio::test]
 async fn pylint_allow_explicit_prerelease_with_marker() -> Result<()> {
     let manifest = Manifest::simple(vec![
-        Requirement::from_pep508(pep508_rs::Requirement::from_str("pylint==2.3.0").unwrap())
-            .unwrap(),
-        Requirement::from_pep508(pep508_rs::Requirement::from_str("isort>=5.0.0b").unwrap())
-            .unwrap(),
+        Requirement::from(pep508_rs::Requirement::from_str("pylint==2.3.0").unwrap()),
+        Requirement::from(pep508_rs::Requirement::from_str("isort>=5.0.0b").unwrap()),
     ]);
     let options = OptionsBuilder::new()
         .prerelease_mode(PreReleaseMode::Explicit)
         .exclude_newer(Some(*EXCLUDE_NEWER))
         .build();
 
     let resolution = resolve(manifest, options, &MARKERS_311, &TAGS_311).await?;
@@ -708,18 +692,17 @@
     Ok(())
 }
 
 /// Resolve `msgraph-sdk==1.0.0`, which depends on `msgraph-core>=1.0.0a2`. The resolver should
 /// fail with a pre-release-centric hint.
 #[tokio::test]
 async fn msgraph_sdk() -> Result<()> {
-    let manifest = Manifest::simple(vec![Requirement::from_pep508(
+    let manifest = Manifest::simple(vec![Requirement::from(
         pep508_rs::Requirement::from_str("msgraph-sdk==1.0.0").unwrap(),
-    )
-    .unwrap()]);
+    )]);
     let options = OptionsBuilder::new()
         .exclude_newer(Some(*EXCLUDE_NEWER))
         .build();
 
     let err = resolve(manifest, options, &MARKERS_311, &TAGS_311)
         .await
         .unwrap_err();
```

### Comparing `uv-0.2.2/crates/uv-client/Cargo.toml` & `uv-0.2.3/crates/uv-client/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-client/src/base_client.rs` & `uv-0.2.3/crates/uv-client/src/base_client.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-client/src/cached_client.rs` & `uv-0.2.3/crates/uv-client/src/cached_client.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-client/src/error.rs` & `uv-0.2.3/crates/uv-client/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-client/src/flat_index.rs` & `uv-0.2.3/crates/uv-client/src/flat_index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-client/src/html.rs` & `uv-0.2.3/crates/uv-client/src/html.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-client/src/httpcache/control.rs` & `uv-0.2.3/crates/uv-client/src/httpcache/control.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-client/src/httpcache/mod.rs` & `uv-0.2.3/crates/uv-client/src/httpcache/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-client/src/lib.rs` & `uv-0.2.3/crates/uv-client/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-client/src/linehaul.rs` & `uv-0.2.3/crates/uv-client/src/linehaul.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-client/src/middleware.rs` & `uv-0.2.3/crates/uv-client/src/middleware.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-client/src/registry_client.rs` & `uv-0.2.3/crates/uv-client/src/registry_client.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-client/src/remote_metadata.rs` & `uv-0.2.3/crates/uv-client/src/remote_metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-client/src/rkyvutil.rs` & `uv-0.2.3/crates/uv-client/src/rkyvutil.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-client/tests/remote_metadata.rs` & `uv-0.2.3/crates/uv-client/tests/remote_metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-client/tests/user_agent_version.rs` & `uv-0.2.3/crates/uv-client/tests/user_agent_version.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv-warnings/src/lib.rs` & `uv-0.2.3/crates/uv-warnings/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/Cargo.toml` & `uv-0.2.3/crates/uv/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "uv"
-version = "0.2.2"
+version = "0.2.3"
 edition = { workspace = true }
 rust-version = { workspace = true }
 homepage = { workspace = true }
 documentation = { workspace = true }
 repository = { workspace = true }
 authors = { workspace = true }
 license = { workspace = true }
@@ -15,14 +15,15 @@
 
 [dependencies]
 distribution-types = { workspace = true }
 install-wheel-rs = { workspace = true, features = ["clap"], default-features = false }
 pep440_rs = { workspace = true }
 pep508_rs = { workspace = true }
 platform-tags = { workspace = true }
+pypi-types = { workspace = true }
 requirements-txt = { workspace = true, features = ["http"] }
 uv-auth = { workspace = true }
 uv-cache = { workspace = true, features = ["clap"] }
 uv-client = { workspace = true }
 uv-configuration = { workspace = true, features = ["clap"] }
 uv-dispatch = { workspace = true }
 uv-distribution = { workspace = true }
```

### Comparing `uv-0.2.2/crates/uv/build.rs` & `uv-0.2.3/crates/uv/build.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/src/cli.rs` & `uv-0.2.3/crates/uv/src/cli.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1942,14 +1942,18 @@
 
     /// Use the given package to provide the command.
     ///
     /// By default, the package name is assumed to match the command name.
     #[arg(long)]
     pub(crate) from: Option<String>,
 
+    /// Include the following extra requirements.
+    #[arg(long)]
+    pub(crate) with: Vec<String>,
+
     /// The Python interpreter to use to build the run environment.
     #[arg(
         long,
         short,
         env = "UV_PYTHON",
         verbatim_doc_comment,
         group = "discovery"
```

### Comparing `uv-0.2.2/crates/uv/src/commands/cache_clean.rs` & `uv-0.2.3/crates/uv/src/commands/cache_clean.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/src/commands/cache_prune.rs` & `uv-0.2.3/crates/uv/src/commands/cache_prune.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/src/commands/mod.rs` & `uv-0.2.3/crates/uv/src/commands/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/src/commands/pip/check.rs` & `uv-0.2.3/crates/uv/src/commands/pip/check.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 use std::fmt::Write;
 use std::time::Instant;
 
 use anyhow::Result;
 use owo_colors::OwoColorize;
 use tracing::debug;
 
-use distribution_types::InstalledDist;
+use distribution_types::{Diagnostic, InstalledDist};
 use uv_cache::Cache;
 use uv_fs::Simplified;
-use uv_installer::{Diagnostic, SitePackages};
+use uv_installer::{SitePackages, SitePackagesDiagnostic};
 use uv_interpreter::{PythonEnvironment, SystemPython};
 
 use crate::commands::{elapsed, ExitStatus};
 use crate::printer::Printer;
 
 /// Check for incompatibilities in installed packages.
 pub(crate) fn pip_check(
@@ -49,15 +49,16 @@
             "Checked {} in {}",
             format!("{} package{}", packages.len(), s).bold(),
             elapsed(start.elapsed())
         )
         .dimmed()
     )?;
 
-    let diagnostics: Vec<Diagnostic> = site_packages.diagnostics()?.into_iter().collect();
+    let diagnostics: Vec<SitePackagesDiagnostic> =
+        site_packages.diagnostics()?.into_iter().collect();
 
     if diagnostics.is_empty() {
         writeln!(
             printer.stderr(),
             "{}",
             "All installed packages are compatible".to_string().dimmed()
         )?;
```

### Comparing `uv-0.2.2/crates/uv/src/commands/pip/compile.rs` & `uv-0.2.3/crates/uv/src/commands/pip/compile.rs`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 use indexmap::IndexMap;
 use itertools::Itertools;
 use owo_colors::OwoColorize;
 use tempfile::tempdir_in;
 use tracing::debug;
 
 use distribution_types::{
-    IndexLocations, LocalEditable, LocalEditables, ParsedUrlError, SourceAnnotation,
-    SourceAnnotations, Verbatim,
+    IndexLocations, LocalEditable, LocalEditables, SourceAnnotation, SourceAnnotations, Verbatim,
 };
 use distribution_types::{Requirement, Requirements};
 use install_wheel_rs::linker::LinkMode;
 use platform_tags::Tags;
 use requirements_txt::EditableRequirement;
 use uv_auth::store_credentials_from_url;
 use uv_cache::Cache;
@@ -174,15 +173,15 @@
         let sources = SourceSelector::from_settings(system);
         find_interpreter(&request, system, &sources, &cache)??
     } else {
         let request = if let Some(version) = python_version.as_ref() {
             // TODO(zanieb): We should consolidate `VersionRequest` and `PythonVersion`
             InterpreterRequest::Version(VersionRequest::from(version))
         } else {
-            InterpreterRequest::Version(VersionRequest::Default)
+            InterpreterRequest::default()
         };
         find_best_interpreter(&request, system, &cache)??
     }
     .into_interpreter();
 
     debug!(
         "Using Python {} interpreter at {} for builds",
@@ -468,25 +467,25 @@
             .map(|built_editable| {
                 let requirements = Requirements {
                     dependencies: built_editable
                         .metadata
                         .requires_dist
                         .iter()
                         .cloned()
-                        .map(Requirement::from_pep508)
-                        .collect::<Result<_, _>>()?,
+                        .map(Requirement::from)
+                        .collect(),
                     optional_dependencies: IndexMap::default(),
                 };
-                Ok::<_, Box<ParsedUrlError>>(BuiltEditableMetadata {
+                BuiltEditableMetadata {
                     built: built_editable.editable,
                     metadata: built_editable.metadata,
                     requirements,
-                })
+                }
             })
-            .collect::<Result<_, _>>()?;
+            .collect();
 
         // Validate that the editables are compatible with the target Python version.
         for editable in &editables {
             if let Some(python_requires) = editable.metadata.requires_python.as_ref() {
                 if !python_requires.contains(python_requirement.target()) {
                     return Err(anyhow!(
                         "Editable `{}` requires Python {}, but resolution targets Python {}",
@@ -704,15 +703,15 @@
     custom_compile_command: Option<String>,
 ) -> String {
     if let Some(cmd_str) = custom_compile_command {
         return cmd_str;
     }
     let args = env::args_os()
         .skip(1)
-        .map(|arg| arg.user_display().to_string())
+        .map(|arg| arg.to_string_lossy().to_string())
         .scan(None, move |skip_next, arg| {
             if matches!(skip_next, Some(true)) {
                 // Reset state; skip this iteration.
                 *skip_next = None;
                 return Some(None);
             }
```

### Comparing `uv-0.2.2/crates/uv/src/commands/pip/freeze.rs` & `uv-0.2.3/crates/uv/src/commands/pip/freeze.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use std::fmt::Write;
 
 use anyhow::Result;
 use itertools::Itertools;
 use owo_colors::OwoColorize;
 use tracing::debug;
 
-use distribution_types::{InstalledDist, Name};
+use distribution_types::{Diagnostic, InstalledDist, Name};
 use uv_cache::Cache;
 use uv_fs::Simplified;
 use uv_installer::SitePackages;
 use uv_interpreter::{PythonEnvironment, SystemPython};
 
 use crate::commands::ExitStatus;
 use crate::printer::Printer;
```

### Comparing `uv-0.2.2/crates/uv/src/commands/pip/install.rs` & `uv-0.2.3/crates/uv/src/commands/pip/install.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 use std::borrow::Cow;
 use std::fmt::Write;
 
 use anstream::eprint;
+use distribution_types::{IndexLocations, Resolution};
 use fs_err as fs;
 use itertools::Itertools;
 use owo_colors::OwoColorize;
 use tracing::{debug, enabled, Level};
 
-use distribution_types::{IndexLocations, Resolution};
 use install_wheel_rs::linker::LinkMode;
 use platform_tags::Tags;
 use uv_auth::store_credentials_from_url;
 use uv_cache::Cache;
 use uv_client::{BaseClientBuilder, Connectivity, FlatIndexClient, RegistryClientBuilder};
 use uv_configuration::{
     Concurrency, ConfigSettings, IndexStrategy, NoBinary, NoBuild, PreviewMode, Reinstall,
@@ -155,41 +155,43 @@
     }
 
     let _lock = venv.lock()?;
 
     // Determine the set of installed packages.
     let site_packages = SitePackages::from_executable(&venv)?;
 
-    // If the requirements are already satisfied, we're done. Ideally, the resolver would be fast
-    // enough to let us remove this check. But right now, for large environments, it's an order of
-    // magnitude faster to validate the environment than to resolve the requirements.
+    // Check if the current environment satisfies the requirements.
+    // Ideally, the resolver would be fast enough to let us remove this check. But right now, for large environments,
+    // it's an order of magnitude faster to validate the environment than to resolve the requirements.
     if reinstall.is_none()
         && upgrade.is_none()
         && source_trees.is_empty()
         && overrides.is_empty()
         && uv_lock.is_none()
     {
         match site_packages.satisfies(&requirements, &editables, &constraints)? {
+            // If the requirements are already satisfied, we're done.
             SatisfiesResult::Fresh {
                 recursive_requirements,
             } => {
                 if enabled!(Level::DEBUG) {
                     for requirement in recursive_requirements
                         .iter()
                         .map(|entry| entry.requirement.to_string())
                         .sorted()
                     {
                         debug!("Requirement satisfied: {requirement}");
                     }
                 }
-
-                debug!(
-                    "All editables satisfied: {}",
-                    editables.iter().map(ToString::to_string).join(" | ")
-                );
+                if !editables.is_empty() {
+                    debug!(
+                        "All editables satisfied: {}",
+                        editables.iter().map(ToString::to_string).join(" | ")
+                    );
+                }
                 let num_requirements = requirements.len() + editables.len();
                 let s = if num_requirements == 1 { "" } else { "s" };
                 writeln!(
                     printer.stderr(),
                     "{}",
                     format!(
                         "Audited {} in {}",
```

### Comparing `uv-0.2.2/crates/uv/src/commands/pip/list.rs` & `uv-0.2.3/crates/uv/src/commands/pip/list.rs`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 use anyhow::Result;
 use itertools::Itertools;
 use owo_colors::OwoColorize;
 use serde::Serialize;
 use tracing::debug;
 use unicode_width::UnicodeWidthStr;
 
-use distribution_types::{InstalledDist, Name};
+use distribution_types::{Diagnostic, InstalledDist, Name};
 use uv_cache::Cache;
 use uv_fs::Simplified;
 use uv_installer::SitePackages;
 use uv_interpreter::{PythonEnvironment, SystemPython};
 use uv_normalize::PackageName;
 
 use crate::commands::ExitStatus;
```

### Comparing `uv-0.2.2/crates/uv/src/commands/pip/operations.rs` & `uv-0.2.3/crates/uv/src/commands/pip/operations.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 //! Common operations shared across the `pip` API and subcommands.
 
+use pypi_types::{ParsedUrl, ParsedUrlError};
 use std::fmt::Write;
 use std::path::PathBuf;
 
 use anyhow::{anyhow, Context};
 use itertools::Itertools;
 use owo_colors::OwoColorize;
 use tracing::debug;
 
 use distribution_types::{
-    CachedDist, Diagnostic, InstalledDist, Requirement, UnresolvedRequirementSpecification,
+    CachedDist, Diagnostic, InstalledDist, Requirement, ResolutionDiagnostic,
+    UnresolvedRequirementSpecification,
 };
 use distribution_types::{
     DistributionMetadata, IndexLocations, InstalledMetadata, InstalledVersion, LocalDist, Name,
-    ParsedUrl, RequirementSource, Resolution,
+    RequirementSource, Resolution,
 };
 use install_wheel_rs::linker::LinkMode;
 use pep440_rs::{VersionSpecifier, VersionSpecifiers};
 use pep508_rs::{MarkerEnvironment, VerbatimUrl};
 use platform_tags::Tags;
 use uv_cache::Cache;
 use uv_client::{BaseClientBuilder, RegistryClient};
@@ -172,15 +174,15 @@
 
     // Collect constraints and overrides.
     let constraints = Constraints::from_requirements(constraints);
     let overrides = Overrides::from_requirements(overrides);
     let python_requirement = PythonRequirement::from_marker_environment(interpreter, markers);
 
     // Map the editables to their metadata.
-    let editables = editables.as_metadata().map_err(Error::ParsedUrl)?;
+    let editables = editables.as_metadata();
 
     // Determine any lookahead requirements.
     let lookaheads = match options.dependency_mode {
         DependencyMode::Transitive => {
             LookaheadResolver::new(
                 &requirements,
                 &constraints,
@@ -704,15 +706,15 @@
         }
     }
     Ok(())
 }
 
 /// Report any diagnostics on resolved distributions.
 pub(crate) fn diagnose_resolution(
-    diagnostics: &[Diagnostic],
+    diagnostics: &[ResolutionDiagnostic],
     printer: Printer,
 ) -> Result<(), Error> {
     for diagnostic in diagnostics {
         writeln!(
             printer.stderr(),
             "{}{} {}",
             "warning".yellow().bold(),
@@ -765,15 +767,12 @@
     #[error(transparent)]
     Fmt(#[from] std::fmt::Error),
 
     #[error(transparent)]
     Lookahead(#[from] uv_requirements::LookaheadError),
 
     #[error(transparent)]
-    ParsedUrl(Box<distribution_types::ParsedUrlError>),
-
-    #[error(transparent)]
     Anyhow(#[from] anyhow::Error),
 
     #[error("Installed distribution has unsupported type")]
-    UnsupportedInstalledDist(#[source] Box<distribution_types::ParsedUrlError>),
+    UnsupportedInstalledDist(#[source] Box<ParsedUrlError>),
 }
```

### Comparing `uv-0.2.2/crates/uv/src/commands/pip/show.rs` & `uv-0.2.3/crates/uv/src/commands/pip/show.rs`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 use anyhow::Result;
 use itertools::{Either, Itertools};
 use owo_colors::OwoColorize;
 use rustc_hash::FxHashMap;
 use tracing::debug;
 
-use distribution_types::Name;
+use distribution_types::{Diagnostic, Name};
 use uv_cache::Cache;
 use uv_fs::Simplified;
 use uv_installer::SitePackages;
 use uv_interpreter::{PythonEnvironment, SystemPython};
 use uv_normalize::PackageName;
 
 use crate::commands::ExitStatus;
```

### Comparing `uv-0.2.2/crates/uv/src/commands/pip/sync.rs` & `uv-0.2.3/crates/uv/src/commands/pip/sync.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/src/commands/pip/uninstall.rs` & `uv-0.2.3/crates/uv/src/commands/pip/uninstall.rs`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 use anyhow::Result;
 use itertools::{Either, Itertools};
 use owo_colors::OwoColorize;
 use tracing::debug;
 
 use distribution_types::{InstalledMetadata, Name, Requirement, UnresolvedRequirement};
 use pep508_rs::UnnamedRequirement;
+use pypi_types::VerbatimParsedUrl;
 use uv_cache::Cache;
 use uv_client::{BaseClientBuilder, Connectivity};
 use uv_configuration::{KeyringProviderType, PreviewMode};
 use uv_fs::Simplified;
 use uv_interpreter::{PythonEnvironment, SystemPython, Target};
 use uv_requirements::{RequirementsSource, RequirementsSpecification};
 
@@ -90,15 +91,15 @@
 
     let _lock = venv.lock()?;
 
     // Index the current `site-packages` directory.
     let site_packages = uv_installer::SitePackages::from_executable(&venv)?;
 
     // Partition the requirements into named and unnamed requirements.
-    let (named, unnamed): (Vec<Requirement>, Vec<UnnamedRequirement>) = spec
+    let (named, unnamed): (Vec<Requirement>, Vec<UnnamedRequirement<VerbatimParsedUrl>>) = spec
         .requirements
         .into_iter()
         .partition_map(|entry| match entry.requirement {
             UnresolvedRequirement::Named(requirement) => Either::Left(requirement),
             UnresolvedRequirement::Unnamed(requirement) => Either::Right(requirement),
         });
 
@@ -114,15 +115,15 @@
         packages
     };
 
     // Sort and deduplicate the unnamed requirements, which are keyed by URL rather than package name.
     let urls = {
         let mut urls = unnamed
             .into_iter()
-            .map(|requirement| requirement.url.to_url())
+            .map(|requirement| requirement.url.verbatim.to_url())
             .collect::<Vec<_>>();
         urls.sort_unstable();
         urls.dedup();
         urls
     };
 
     // Map to the local distributions.
```

### Comparing `uv-0.2.2/crates/uv/src/commands/project/lock.rs` & `uv-0.2.3/crates/uv/src/commands/project/lock.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/src/commands/project/mod.rs` & `uv-0.2.3/crates/uv/src/commands/project/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -110,33 +110,34 @@
         &client_builder,
         preview,
     )
     .await?;
 
     // Check if the current environment satisfies the requirements
     let site_packages = SitePackages::from_executable(&venv)?;
-
-    // If the requirements are already satisfied, we're done.
     if spec.source_trees.is_empty() {
         match site_packages.satisfies(&spec.requirements, &spec.editables, &spec.constraints)? {
+            // If the requirements are already satisfied, we're done.
             SatisfiesResult::Fresh {
                 recursive_requirements,
             } => {
                 debug!(
                     "All requirements satisfied: {}",
                     recursive_requirements
                         .iter()
                         .map(|entry| entry.requirement.to_string())
                         .sorted()
                         .join(" | ")
                 );
-                debug!(
-                    "All editables satisfied: {}",
-                    spec.editables.iter().map(ToString::to_string).join(", ")
-                );
+                if !spec.editables.is_empty() {
+                    debug!(
+                        "All editables satisfied: {}",
+                        spec.editables.iter().map(ToString::to_string).join(", ")
+                    );
+                }
                 return Ok(venv);
             }
             SatisfiesResult::Unsatisfied(requirement) => {
                 debug!("At least one requirement is not satisfied: {requirement}");
             }
         }
     }
```

### Comparing `uv-0.2.2/crates/uv/src/commands/project/run.rs` & `uv-0.2.3/crates/uv/src/commands/project/run.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/src/commands/project/sync.rs` & `uv-0.2.3/crates/uv/src/commands/project/sync.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/src/commands/reporters.rs` & `uv-0.2.3/crates/uv/src/commands/reporters.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/src/commands/self_update.rs` & `uv-0.2.3/crates/uv/src/commands/self_update.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/src/commands/tool/run.rs` & `uv-0.2.3/crates/uv/src/commands/tool/run.rs`

 * *Files 3% similar despite different names*

```diff
@@ -21,28 +21,31 @@
 /// Run a command.
 #[allow(clippy::too_many_arguments)]
 pub(crate) async fn run(
     target: String,
     args: Vec<OsString>,
     python: Option<String>,
     from: Option<String>,
+    with: Vec<String>,
     _isolated: bool,
     preview: PreviewMode,
     connectivity: Connectivity,
     cache: &Cache,
     printer: Printer,
 ) -> Result<ExitStatus> {
     if preview.is_disabled() {
         warn_user!("`uv tool run` is experimental and may change without warning.");
     }
 
-    // TODO(zanieb): Allow users to pass additional requirements
     let requirements = [RequirementsSource::from_package(
         from.unwrap_or_else(|| target.clone()),
-    )];
+    )]
+    .into_iter()
+    .chain(with.into_iter().map(RequirementsSource::from_package))
+    .collect::<Vec<_>>();
 
     // TODO(zanieb): When implementing project-level tools, discover the project and check if it has the tool
     // TOOD(zanieb): Determine if we sould layer on top of the project environment if it is present
 
     // If necessary, create an environment for the ephemeral requirements.
     debug!("Syncing ephemeral environment.");
```

### Comparing `uv-0.2.2/crates/uv/src/commands/venv.rs` & `uv-0.2.3/crates/uv/src/commands/venv.rs`

 * *Files 2% similar despite different names*

```diff
@@ -221,24 +221,22 @@
         )
         .with_options(OptionsBuilder::new().exclude_newer(exclude_newer).build());
 
         // Resolve the seed packages.
         let requirements = if interpreter.python_tuple() < (3, 12) {
             // Only include `setuptools` and `wheel` on Python <3.12
             vec![
-                Requirement::from_pep508(pep508_rs::Requirement::from_str("pip").unwrap()).unwrap(),
-                Requirement::from_pep508(pep508_rs::Requirement::from_str("setuptools").unwrap())
-                    .unwrap(),
-                Requirement::from_pep508(pep508_rs::Requirement::from_str("wheel").unwrap())
-                    .unwrap(),
+                Requirement::from(pep508_rs::Requirement::from_str("pip").unwrap()),
+                Requirement::from(pep508_rs::Requirement::from_str("setuptools").unwrap()),
+                Requirement::from(pep508_rs::Requirement::from_str("wheel").unwrap()),
             ]
         } else {
-            vec![
-                Requirement::from_pep508(pep508_rs::Requirement::from_str("pip").unwrap()).unwrap(),
-            ]
+            vec![Requirement::from(
+                pep508_rs::Requirement::from_str("pip").unwrap(),
+            )]
         };
 
         // Resolve and install the requirements.
         //
         // Since the virtual environment is empty, and the set of requirements is trivial (no
         // constraints, no editables, etc.), we can use the build dispatch APIs directly.
         let resolution = build_dispatch
```

### Comparing `uv-0.2.2/crates/uv/src/commands/version.rs` & `uv-0.2.3/crates/uv/src/commands/version.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/src/compat/mod.rs` & `uv-0.2.3/crates/uv/src/compat/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/src/editables.rs` & `uv-0.2.3/crates/uv/src/editables.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 use std::ops::Deref;
 
 use anyhow::{anyhow, Context, Result};
 use indexmap::IndexMap;
 use owo_colors::OwoColorize;
 
 use distribution_types::{
-    InstalledDist, LocalEditable, LocalEditables, Name, ParsedUrlError, Requirement, Requirements,
+    InstalledDist, LocalEditable, LocalEditables, Name, Requirement, Requirements,
 };
 use platform_tags::Tags;
 use requirements_txt::EditableRequirement;
 use uv_cache::{ArchiveTarget, ArchiveTimestamp, Cache};
 use uv_client::RegistryClient;
 use uv_configuration::{Concurrency, Reinstall};
 use uv_dispatch::BuildDispatch;
@@ -155,32 +155,32 @@
 
         Ok(Self {
             editables,
             temp_dir,
         })
     }
 
-    pub(crate) fn as_metadata(&self) -> Result<Vec<BuiltEditableMetadata>, Box<ParsedUrlError>> {
+    pub(crate) fn as_metadata(&self) -> Vec<BuiltEditableMetadata> {
         self.iter()
             .map(|editable| {
                 let dependencies: Vec<_> = editable
                     .metadata()
                     .requires_dist
                     .iter()
                     .cloned()
-                    .map(Requirement::from_pep508)
-                    .collect::<Result<_, _>>()?;
-                Ok::<_, Box<ParsedUrlError>>(BuiltEditableMetadata {
+                    .map(Requirement::from)
+                    .collect();
+                BuiltEditableMetadata {
                     built: editable.local().clone(),
                     metadata: editable.metadata().clone(),
                     requirements: Requirements {
                         dependencies,
                         optional_dependencies: IndexMap::default(),
                     },
-                })
+                }
             })
             .collect()
     }
 
     /// Convert an [`EditableRequirement`] into a [`LocalEditable`].
     pub(crate) fn from_requirement(editable: EditableRequirement) -> LocalEditable {
         LocalEditable {
```

### Comparing `uv-0.2.2/crates/uv/src/logging.rs` & `uv-0.2.3/crates/uv/src/logging.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/src/main.rs` & `uv-0.2.3/crates/uv/src/main.rs`

 * *Files 1% similar despite different names*

```diff
@@ -610,19 +610,23 @@
         Commands::GenerateShellCompletion { shell } => {
             shell.generate(&mut Cli::command(), &mut stdout());
             Ok(ExitStatus::Success)
         }
         Commands::Tool(ToolNamespace {
             command: ToolCommand::Run(args),
         }) => {
+            // Initialize the cache.
+            let cache = cache.init()?;
+
             commands::run_tool(
                 args.target,
                 args.args,
                 args.python,
                 args.from,
+                args.with,
                 globals.isolated,
                 globals.preview,
                 globals.connectivity,
                 &cache,
                 printer,
             )
             .await
```

### Comparing `uv-0.2.2/crates/uv/src/printer.rs` & `uv-0.2.3/crates/uv/src/printer.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/src/settings.rs` & `uv-0.2.3/crates/uv/src/settings.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/src/shell.rs` & `uv-0.2.3/crates/uv/src/shell.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/src/version.rs` & `uv-0.2.3/crates/uv/src/version.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/tests/cache_prune.rs` & `uv-0.2.3/crates/uv/tests/cache_prune.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/tests/common/mod.rs` & `uv-0.2.3/crates/uv/tests/common/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -399,15 +399,17 @@
                 let request = InterpreterRequest::Version(
                     VersionRequest::from_str(python_version)
                         .expect("The test version request must be valid"),
                 );
                 let sources = SourceSelector::All;
                 if let Ok(found) = find_interpreter(
                     &request,
-                    uv_interpreter::SystemPython::Allowed,
+                    // Without required, we could pick the current venv here and the test fails
+                    // because the venv subcommand requires a system interpreter.
+                    uv_interpreter::SystemPython::Required,
                     &sources,
                     &cache,
                 )
                 .unwrap()
                 {
                     vec![found
                         .into_interpreter()
```

### Comparing `uv-0.2.2/crates/uv/tests/lock.rs` & `uv-0.2.3/crates/uv/tests/lock.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/tests/pip_check.rs` & `uv-0.2.3/crates/uv/tests/pip_check.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/tests/pip_compile.rs` & `uv-0.2.3/crates/uv/tests/pip_compile.rs`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                 .arg("requirements.in"), @r###"
         success: false
         exit_code: 2
         ----- stdout -----
 
         ----- stderr -----
         warning: Requirements file requirements.in does not contain any dependencies
-        error: failed to canonicalize path `[VENV]/bin/python`
+        error: failed to canonicalize path `[VENV]/bin/python3`
           Caused by: No such file or directory (os error 2)
         "###
         );
     }
 
     context
         .temp_dir
@@ -761,15 +761,15 @@
     uv_snapshot!(context.filters(), context.compile()
             .arg("pyproject.toml"), @r###"
     success: false
     exit_code: 2
     ----- stdout -----
 
     ----- stderr -----
-    error: Failed to parse `pyproject.toml`
+    error: Failed to parse: `pyproject.toml`
       Caused by: TOML parse error at line 5, column 8
       |
     5 | name = "!project"
       |        ^^^^^^^^^^
     Not a valid package or extra name: "!project". Names must start and end with a letter or digit and may only contain -, _, ., and alphanumeric characters.
 
     "###
@@ -1759,199 +1759,184 @@
           And because you require flask==3.0.0, we can conclude that the requirements are unsatisfiable.
     "###
     );
 
     Ok(())
 }
 
-/// Request `anyio` via two different URLs which resolve to the same canonical version.
+/// Request `uv-public-pypackage` via two different URLs which resolve to the same canonical version.
 #[test]
 fn compatible_repeated_url_dependency() -> Result<()> {
     let context = TestContext::new("3.12");
     let requirements_in = context.temp_dir.child("requirements.in");
     requirements_in.write_str(indoc! {r"
-        anyio @ git+https://github.com/agronholm/anyio.git@4.3.0
-        anyio @ git+https://github.com/agronholm/anyio@4.3.0
+        uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage.git@0.0.2
+        uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage@0.0.2
     "})?;
 
     uv_snapshot!(context.compile()
             .arg("requirements.in"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
     # This file was autogenerated by uv via the following command:
     #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2024-03-25T00:00:00Z requirements.in
-    anyio @ git+https://github.com/agronholm/anyio@437a7e310925a962cab4a58fcd2455fbcd578d51
+    uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389
         # via -r requirements.in
-    idna==3.6
-        # via anyio
-    sniffio==1.3.1
-        # via anyio
 
     ----- stderr -----
-    Resolved 3 packages in [TIME]
+    Resolved 1 package in [TIME]
     "###
     );
 
     Ok(())
 }
 
-/// Request `anyio` via two different URLs which resolve to the same repository, but different
-/// commits.
+/// Request `uv-public-pypackage` via two different URLs which resolve to the same repository, but
+/// different commits.
 #[test]
 fn conflicting_repeated_url_dependency() -> Result<()> {
     let context = TestContext::new("3.12");
     let requirements_in = context.temp_dir.child("requirements.in");
     requirements_in.write_str(indoc! {r"
-        anyio @ git+https://github.com/agronholm/anyio.git@4.3.0
-        anyio @ git+https://github.com/agronholm/anyio.git@4.0.0
+        uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage.git@0.0.2
+        uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage.git@0.0.1
     "})?;
 
     uv_snapshot!(context.compile()
             .arg("requirements.in"), @r###"
     success: false
     exit_code: 2
     ----- stdout -----
 
     ----- stderr -----
-    error: Requirements contain conflicting URLs for package `anyio`:
-    - git+https://github.com/agronholm/anyio.git@4.3.0
-    - git+https://github.com/agronholm/anyio.git@4.0.0
+    error: Requirements contain conflicting URLs for package `uv-public-pypackage`:
+    - git+https://github.com/astral-test/uv-public-pypackage.git@0.0.2
+    - git+https://github.com/astral-test/uv-public-pypackage.git@0.0.1
     "###
     );
 
     Ok(())
 }
 
-/// Request `anyio` via three different URLs: `4.3.0`, a short SHA, and a precise SHA. All three
-/// are compatible, since they resolve to the same canonical version.
+/// Request `uv-public-pypackage` via three different URLs: `0.0.2`, a short SHA, and a precise SHA.
+/// All three are compatible, since they resolve to the same canonical version.
 #[test]
 fn compatible_narrowed_url_dependency() -> Result<()> {
     let context = TestContext::new("3.12");
     let requirements_in = context.temp_dir.child("requirements.in");
     requirements_in.write_str(indoc! {r"
-        anyio @ git+https://github.com/agronholm/anyio.git@4.3.0
-        anyio @ git+https://github.com/agronholm/anyio@437a7e31
-        anyio @ git+https://github.com/agronholm/anyio@437a7e310925a962cab4a58fcd2455fbcd578d51
+        uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage.git@0.0.2
+        uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage.git@b270df1
+        uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage.git@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389
     "})?;
 
     uv_snapshot!(context.compile()
             .arg("requirements.in"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
     # This file was autogenerated by uv via the following command:
     #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2024-03-25T00:00:00Z requirements.in
-    anyio @ git+https://github.com/agronholm/anyio@437a7e310925a962cab4a58fcd2455fbcd578d51
+    uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage.git@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389
         # via -r requirements.in
-    idna==3.6
-        # via anyio
-    sniffio==1.3.1
-        # via anyio
 
     ----- stderr -----
-    Resolved 3 packages in [TIME]
+    Resolved 1 package in [TIME]
     "###
     );
 
     Ok(())
 }
 
-/// Request `anyio` via three different URLs: a precise SHA, a short SHA, and `4.3.0`. All three
-/// are compatible, since they resolve to the same canonical version.
+/// Request `uv-public-pypackage` via three different URLs: a precise SHA, a short SHA, and `4.3.0`.
+/// All three are compatible, since they resolve to the same canonical version.
 #[test]
 fn compatible_broader_url_dependency() -> Result<()> {
     let context = TestContext::new("3.12");
     let requirements_in = context.temp_dir.child("requirements.in");
     requirements_in.write_str(indoc! {r"
-        anyio @ git+https://github.com/agronholm/anyio@437a7e310925a962cab4a58fcd2455fbcd578d51
-        anyio @ git+https://github.com/agronholm/anyio@437a7e31
-        anyio @ git+https://github.com/agronholm/anyio.git@4.3.0
+        uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage.git@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389
+        uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage.git@b270df1
+        uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage.git@0.0.2
     "})?;
 
     uv_snapshot!(context.compile()
             .arg("requirements.in"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
     # This file was autogenerated by uv via the following command:
     #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2024-03-25T00:00:00Z requirements.in
-    anyio @ git+https://github.com/agronholm/anyio.git@437a7e310925a962cab4a58fcd2455fbcd578d51
+    uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage.git@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389
         # via -r requirements.in
-    idna==3.6
-        # via anyio
-    sniffio==1.3.1
-        # via anyio
 
     ----- stderr -----
-    Resolved 3 packages in [TIME]
+    Resolved 1 package in [TIME]
     "###
     );
 
     Ok(())
 }
 
-/// Request `anyio` via two different URLs: `4.3.0`, and a precise SHA, followed by `4.3.0` again.
-/// All three are compatible, since they resolve to the same canonical version.
+/// Request `uv-public-pypackage` via two different URLs: `0.0.2`, and a precise SHA, followed by
+/// `0.0.2` again. All three are compatible, since they resolve to the same canonical version.
 #[test]
 fn compatible_repeated_narrowed_url_dependency() -> Result<()> {
     let context = TestContext::new("3.12");
     let requirements_in = context.temp_dir.child("requirements.in");
     requirements_in.write_str(indoc! {r"
-        anyio @ git+https://github.com/agronholm/anyio.git@4.3.0
-        anyio @ git+https://github.com/agronholm/anyio@437a7e310925a962cab4a58fcd2455fbcd578d51
-        anyio @ git+https://github.com/agronholm/anyio.git@4.3.0
+        uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage.git@0.0.2
+        uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage.git@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389
+        uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage.git@0.0.2
     "})?;
 
     uv_snapshot!(context.compile()
             .arg("requirements.in"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
     # This file was autogenerated by uv via the following command:
     #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2024-03-25T00:00:00Z requirements.in
-    anyio @ git+https://github.com/agronholm/anyio.git@437a7e310925a962cab4a58fcd2455fbcd578d51
+    uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage.git@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389
         # via -r requirements.in
-    idna==3.6
-        # via anyio
-    sniffio==1.3.1
-        # via anyio
 
     ----- stderr -----
-    Resolved 3 packages in [TIME]
+    Resolved 1 package in [TIME]
     "###
     );
 
     Ok(())
 }
 
-/// Request `anyio` via three different URLs: `4.3.0`, a precise SHA, and `master`.
+/// Request `uv-public-pypackage` via three different URLs: `0.0.2`, a precise SHA, and
+/// `test-branch`.
 ///
-/// Although `4.3.0` and the precise SHA resolve to the same canonical version, `master` resolves to
-/// a different version, so there should be a conflict.
+/// Although `0.0.2` and the precise SHA resolve to the same canonical version, `test-branch`
+/// resolves to a different version, so there should be a conflict.
 #[test]
 fn incompatible_narrowed_url_dependency() -> Result<()> {
     let context = TestContext::new("3.12");
     let requirements_in = context.temp_dir.child("requirements.in");
     requirements_in.write_str(indoc! {r"
-        anyio @ git+https://github.com/agronholm/anyio.git@4.3.0
-        anyio @ git+https://github.com/agronholm/anyio@437a7e310925a962cab4a58fcd2455fbcd578d51
-        anyio @ git+https://github.com/agronholm/anyio.git@master
+        uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage.git@0.0.2
+        uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389
+        uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage@test-branch
     "})?;
 
     uv_snapshot!(context.compile()
             .arg("requirements.in"), @r###"
     success: false
     exit_code: 2
     ----- stdout -----
 
     ----- stderr -----
-    error: Requirements contain conflicting URLs for package `anyio`:
-    - git+https://github.com/agronholm/anyio@437a7e310925a962cab4a58fcd2455fbcd578d51
-    - git+https://github.com/agronholm/anyio.git@master
+    error: Requirements contain conflicting URLs for package `uv-public-pypackage`:
+    - git+https://github.com/astral-test/uv-public-pypackage@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389
+    - git+https://github.com/astral-test/uv-public-pypackage@test-branch
     "###
     );
 
     Ok(())
 }
 
 /// Request `hatchling_editable`, which depends on `https://files.pythonhosted.org/packages/ef/a6/62565a6e1cf69e10f5727360368e451d4b7f58beeac6173dc9db836a5b46/iniconfig-2.0.0-py3-none-any.whl`.
@@ -3201,15 +3186,15 @@
     ----- stdout -----
     # This file was autogenerated by uv via the following command:
     #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2024-03-25T00:00:00Z requirements.in
     blinker==1.7.0
         # via flask
     click==8.1.7
         # via flask
-    ${URL}
+    flask @ ${URL}
         # via -r requirements.in
     itsdangerous==2.1.2
         # via flask
     jinja2==3.1.3
         # via flask
     markupsafe==2.1.5
         # via
@@ -3242,15 +3227,15 @@
     ----- stdout -----
     # This file was autogenerated by uv via the following command:
     #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2024-03-25T00:00:00Z requirements.in
     blinker==1.7.0
         # via flask
     click==8.1.7
         # via flask
-    ${URL}
+    flask @ ${URL}
         # via -r requirements.in
     itsdangerous==2.1.2
         # via flask
     jinja2==3.1.3
         # via flask
     markupsafe==2.1.5
         # via
@@ -5282,14 +5267,55 @@
     ----- stderr -----
     Resolved 1 package in [TIME]
     "###);
 
     Ok(())
 }
 
+/// Resolve a registry package (`black`) with an unnamed URL preference. The preference should be
+/// ignored.
+#[test]
+fn compile_unnamed_preference() -> Result<()> {
+    let context = TestContext::new("3.12");
+    let requirements_in = context.temp_dir.child("requirements.in");
+    requirements_in.write_str("black")?;
+
+    let requirements_txt = context.temp_dir.child("requirements.txt");
+    requirements_txt.write_str("./scripts/packages/black_editable")?;
+
+    uv_snapshot!(context
+        .compile()
+        .arg("requirements.in")
+        .arg("-o")
+        .arg("requirements.txt"), @r###"
+    success: true
+    exit_code: 0
+    ----- stdout -----
+    # This file was autogenerated by uv via the following command:
+    #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2024-03-25T00:00:00Z requirements.in -o requirements.txt
+    black==24.3.0
+        # via -r requirements.in
+    click==8.1.7
+        # via black
+    mypy-extensions==1.0.0
+        # via black
+    packaging==24.0
+        # via black
+    pathspec==0.12.1
+        # via black
+    platformdirs==4.2.0
+        # via black
+
+    ----- stderr -----
+    Resolved 6 packages in [TIME]
+    "###);
+
+    Ok(())
+}
+
 /// Resolve a package from a `requirements.in` file, with a `constraints.txt` pinning that package
 /// to a specific URL.
 #[test]
 fn compile_constraints_compatible_url() -> Result<()> {
     let context = TestContext::new("3.12");
     let requirements_in = context.temp_dir.child("requirements.in");
     requirements_in.write_str("anyio>4")?;
@@ -5454,15 +5480,18 @@
     uv_snapshot!(context.compile()
             .arg("requirements.in"), @r###"
     success: false
     exit_code: 2
     ----- stdout -----
 
     ----- stderr -----
-    error: Unsupported URL prefix `bzr` in URL: `bzr+https://example.com/anyio` (Bazaar is not supported)
+    error: Couldn't parse requirement in `requirements.in` at position 0
+      Caused by: Unsupported URL prefix `bzr` in URL: `bzr+https://example.com/anyio` (Bazaar is not supported)
+    anyio @ bzr+https://example.com/anyio
+            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     "###
     );
 
     Ok(())
 }
 
 /// Resolve a package with `--no-deps`, including a valid extra.
@@ -7519,15 +7548,15 @@
 
     uv_snapshot!(context.filters(), context.compile()
         .arg(requirements_in.canonicalize()?), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
     # This file was autogenerated by uv via the following command:
-    #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2024-03-25T00:00:00Z requirements.in
+    #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2024-03-25T00:00:00Z [TEMP_DIR]/requirements.in
     anyio==4.3.0
         # via -r requirements.in
     idna==3.6
         # via anyio
     sniffio==1.3.1
         # via anyio
 
@@ -7556,15 +7585,15 @@
     // The local version should _not_ be included in the resolution
     uv_snapshot!(context.filters(), context.compile()
         .arg(requirements_in.canonicalize()?), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
     # This file was autogenerated by uv via the following command:
-    #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2024-03-25T00:00:00Z requirements.in
+    #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2024-03-25T00:00:00Z [TEMP_DIR]/requirements.in
     anyio==4.3.0
         # via -r requirements.in
     idna==3.6
         # via anyio
     sniffio==1.3.1
         # via anyio
 
@@ -7588,15 +7617,15 @@
         .arg(requirements_in.canonicalize()?)
         .arg("--output-file")
         .arg(requirements_txt.canonicalize()?), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
     # This file was autogenerated by uv via the following command:
-    #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2024-03-25T00:00:00Z requirements.in --output-file requirements.txt
+    #    uv pip compile --cache-dir [CACHE_DIR] --exclude-newer 2024-03-25T00:00:00Z [TEMP_DIR]/requirements.in --output-file [TEMP_DIR]/requirements.txt
     anyio==4.3.0
         # via -r requirements.in
     idna==3.6
         # via anyio
     sniffio==1.3.1
         # via anyio
```

### Comparing `uv-0.2.2/crates/uv/tests/pip_compile_scenarios.rs` & `uv-0.2.3/crates/uv/tests/pip_compile_scenarios.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/tests/pip_freeze.rs` & `uv-0.2.3/crates/uv/tests/pip_freeze.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/tests/pip_install.rs` & `uv-0.2.3/crates/uv/tests/pip_install.rs`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         .arg("-r")
         .arg("pyproject.toml"), @r###"
     success: false
     exit_code: 2
     ----- stdout -----
 
     ----- stderr -----
-    error: Failed to parse `pyproject.toml`
+    error: Failed to parse: `pyproject.toml`
       Caused by: TOML parse error at line 1, column 5
       |
     1 | 123 - 456
       |     ^
     expected `.`, `=`
 
     "###
@@ -167,15 +167,15 @@
         .arg("-r")
         .arg("pyproject.toml"), @r###"
     success: false
     exit_code: 2
     ----- stdout -----
 
     ----- stderr -----
-    error: Failed to parse `pyproject.toml`
+    error: Failed to parse: `pyproject.toml`
       Caused by: TOML parse error at line 1, column 1
       |
     1 | [project]
       | ^^^^^^^^^
     missing field `name`
 
     "###
@@ -205,15 +205,15 @@
         .arg("-r")
         .arg("pyproject.toml"), @r###"
     success: false
     exit_code: 2
     ----- stdout -----
 
     ----- stderr -----
-    error: Failed to parse `pyproject.toml`
+    error: Failed to parse: `pyproject.toml`
       Caused by: after parsing '1.0', found '.x', which is not part of a valid version
     flask==1.0.x
          ^^^^^^^
     "###
     );
 
     Ok(())
@@ -5010,15 +5010,15 @@
         .arg("--extra")
         .arg("utils"), @r###"
     success: false
     exit_code: 2
     ----- stdout -----
 
     ----- stderr -----
-    error: Failed to parse `pyproject.toml`
+    error: Failed to parse: `pyproject.toml`
       Caused by: Failed to parse entry for: `tqdm`
       Caused by: `tool.uv.sources` is a preview feature; use `--preview` or set `UV_PREVIEW=1` to enable it
     "###
     );
 
     Ok(())
 }
```

### Comparing `uv-0.2.2/crates/uv/tests/pip_install_scenarios.rs` & `uv-0.2.3/crates/uv/tests/pip_install_scenarios.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/tests/pip_list.rs` & `uv-0.2.3/crates/uv/tests/pip_list.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/tests/pip_show.rs` & `uv-0.2.3/crates/uv/tests/pip_show.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/tests/pip_sync.rs` & `uv-0.2.3/crates/uv/tests/pip_sync.rs`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     } else {
         uv_snapshot!(context.filters(), command(&context).arg("requirements.txt"), @r###"
         success: false
         exit_code: 2
         ----- stdout -----
 
         ----- stderr -----
-        error: failed to canonicalize path `[VENV]/bin/python`
+        error: failed to canonicalize path `[VENV]/bin/python3`
           Caused by: No such file or directory (os error 2)
         "###);
     }
 
     assert!(predicates::path::missing().eval(&context.venv));
 
     Ok(())
@@ -509,61 +509,67 @@
 /// Install a package into a virtual environment from a Git repository.
 #[test]
 #[cfg(feature = "git")]
 fn install_git_commit() -> Result<()> {
     let context = TestContext::new("3.12");
 
     let requirements_txt = context.temp_dir.child("requirements.txt");
-    requirements_txt.write_str("werkzeug @ git+https://github.com/pallets/werkzeug.git@af160e0b6b7ddd81c22f1652c728ff5ac72d5c74")?;
+    requirements_txt.write_str("uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389")?;
 
     uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--strict"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Downloaded 1 package in [TIME]
     Installed 1 package in [TIME]
-     + werkzeug==2.0.0 (from git+https://github.com/pallets/werkzeug.git@af160e0b6b7ddd81c22f1652c728ff5ac72d5c74)
+     + uv-public-pypackage==0.1.0 (from git+https://github.com/astral-test/uv-public-pypackage@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389)
     "###
     );
 
-    context.assert_command("import werkzeug").success();
+    context
+        .assert_command("import uv_public_pypackage")
+        .success();
 
     Ok(())
 }
 
 /// Install a package into a virtual environment from a Git repository.
 #[test]
 #[cfg(feature = "git")]
 fn install_git_tag() -> Result<()> {
     let context = TestContext::new("3.12");
 
     let requirements_txt = context.temp_dir.child("requirements.txt");
-    requirements_txt.write_str("werkzeug @ git+https://github.com/pallets/WerkZeug.git@2.0.0")?;
+    requirements_txt.write_str(
+        "uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage@test-tag",
+    )?;
 
     uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--strict"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Downloaded 1 package in [TIME]
     Installed 1 package in [TIME]
-     + werkzeug==2.0.0 (from git+https://github.com/pallets/WerkZeug.git@af160e0b6b7ddd81c22f1652c728ff5ac72d5c74)
+     + uv-public-pypackage==0.1.0 (from git+https://github.com/astral-test/uv-public-pypackage@0dacfd662c64cb4ceb16e6cf65a157a8b715b979)
     "###
     );
 
-    context.assert_command("import werkzeug").success();
+    context
+        .assert_command("import uv_public_pypackage")
+        .success();
 
     Ok(())
 }
 
 /// Install two packages from the same Git repository.
 #[test]
 #[cfg(feature = "git")]
@@ -598,88 +604,94 @@
 
 /// Install a source distribution into a virtual environment.
 #[test]
 fn install_sdist() -> Result<()> {
     let context = TestContext::new("3.12");
 
     let requirements_txt = context.temp_dir.child("requirements.txt");
-    requirements_txt.write_str("Werkzeug==0.9.6")?;
+    requirements_txt.write_str("source-distribution==0.0.1")?;
 
     uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--strict"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Downloaded 1 package in [TIME]
     Installed 1 package in [TIME]
-     + werkzeug==0.9.6
+     + source-distribution==0.0.1
     "###
     );
 
-    context.assert_command("import werkzeug").success();
+    context
+        .assert_command("import source_distribution")
+        .success();
 
     Ok(())
 }
 
 /// Install a source distribution into a virtual environment.
 #[test]
 fn install_sdist_url() -> Result<()> {
     let context = TestContext::new("3.12");
 
     let requirements_txt = context.temp_dir.child("requirements.txt");
-    requirements_txt.write_str("Werkzeug @ https://files.pythonhosted.org/packages/63/69/5702e5eb897d1a144001e21d676676bcb87b88c0862f947509ea95ea54fc/Werkzeug-0.9.6.tar.gz")?;
+    requirements_txt.write_str("source-distribution @ https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz")?;
 
     uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--strict"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Downloaded 1 package in [TIME]
     Installed 1 package in [TIME]
-     + werkzeug==0.9.6 (from https://files.pythonhosted.org/packages/63/69/5702e5eb897d1a144001e21d676676bcb87b88c0862f947509ea95ea54fc/Werkzeug-0.9.6.tar.gz)
+     + source-distribution==0.0.1 (from https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz)
     "###
     );
 
-    context.assert_command("import werkzeug").success();
+    context
+        .assert_command("import source_distribution")
+        .success();
 
     Ok(())
 }
 
 /// Install a package with source archive format `.tar.bz2`.
 #[test]
 fn install_sdist_archive_type_bz2() -> Result<()> {
     let context = TestContext::new("3.8");
 
     let requirements_txt = context.temp_dir.child("requirements.txt");
-    requirements_txt.write_str("bz2==1.0.0")?;
+    requirements_txt.write_str(&format!(
+        "bz2 @ {}",
+        context
+            .workspace_root
+            .join("scripts/links/bz2-1.0.0.tar.bz2")
+            .display()
+    ))?;
 
-    uv_snapshot!(command(&context)
+    uv_snapshot!(context.filters(), command(&context)
         .arg("requirements.txt")
-        .arg("--no-binary")
-        .arg(":all:")
-        .arg("--strict")
-        .arg("--find-links")
-        .arg(context.workspace_root.join("scripts/links/")), @r###"
+        .arg("--strict"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Downloaded 1 package in [TIME]
     Installed 1 package in [TIME]
-     + bz2==1.0.0
+     + bz2==1.0.0 (from file://[WORKSPACE]/scripts/links/bz2-1.0.0.tar.bz2)
     "###
     );
 
     Ok(())
 }
 
 /// Attempt to re-install a package into a virtual environment from a URL. The second install
@@ -1167,51 +1179,14 @@
     );
 
     context.assert_command("import wheel").success();
 
     Ok(())
 }
 
-/// The `ujson` package includes a `[build-system]`, but no `build-backend`. It lists some explicit
-/// build requirements, but _also_ depends on `wheel` and `setuptools`:
-/// ```toml
-/// [build-system]
-/// requires = ["setuptools>=42", "setuptools_scm[toml]>=3.4"]
-/// ```
-///
-/// Like `pip` and `build`, we should use PEP 517 here and respect the `requires`, but use the
-/// default build backend.
-#[test]
-#[cfg(unix)] // https://github.com/astral-sh/uv/issues/1238
-fn install_ujson() -> Result<()> {
-    let context = TestContext::new("3.12");
-
-    let requirements_txt = context.temp_dir.child("requirements.txt");
-    requirements_txt.write_str("ujson @ https://files.pythonhosted.org/packages/43/1a/b0a027144aa5c8f4ea654f4afdd634578b450807bb70b9f8bad00d6f6d3c/ujson-5.7.0.tar.gz")?;
-
-    uv_snapshot!(command(&context)
-        .arg("requirements.txt")
-        .arg("--strict"), @r###"
-    success: true
-    exit_code: 0
-    ----- stdout -----
-
-    ----- stderr -----
-    Resolved 1 package in [TIME]
-    Downloaded 1 package in [TIME]
-    Installed 1 package in [TIME]
-     + ujson==5.7.0 (from https://files.pythonhosted.org/packages/43/1a/b0a027144aa5c8f4ea654f4afdd634578b450807bb70b9f8bad00d6f6d3c/ujson-5.7.0.tar.gz)
-    "###
-    );
-
-    context.assert_command("import ujson").success();
-
-    Ok(())
-}
-
 /// This package includes a `[build-system]`, but no `build-backend`.
 ///
 /// It lists some explicit build requirements that are necessary to build the distribution:
 /// ```toml
 /// [build-system]
 /// requires = ["Cython<3", "setuptools", "wheel"]
 /// ```
@@ -1251,130 +1226,130 @@
 
 /// Check that we show the right messages on cached, direct URL source distribution installs.
 #[test]
 fn install_url_source_dist_cached() -> Result<()> {
     let context = TestContext::new("3.12");
 
     let requirements_txt = context.temp_dir.child("requirements.txt");
-    requirements_txt.write_str("tqdm @ https://files.pythonhosted.org/packages/62/06/d5604a70d160f6a6ca5fd2ba25597c24abd5c5ca5f437263d177ac242308/tqdm-4.66.1.tar.gz")?;
+    requirements_txt.write_str("source_distribution @ https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz")?;
 
-    let filters = if cfg!(windows) {
-        [("warning: The package `tqdm` requires `colorama ; platform_system == 'Windows'`, but it's not installed.\n", "")]
-            .into_iter()
-            .chain(context.filters())
-            .collect()
-    } else {
-        context.filters()
-    };
-    uv_snapshot!(filters, command(&context)
+    uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--strict"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Downloaded 1 package in [TIME]
     Installed 1 package in [TIME]
-     + tqdm==4.66.1 (from https://files.pythonhosted.org/packages/62/06/d5604a70d160f6a6ca5fd2ba25597c24abd5c5ca5f437263d177ac242308/tqdm-4.66.1.tar.gz)
+     + source-distribution==0.0.1 (from https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz)
     "###
     );
 
-    context.assert_command("import tqdm").success();
+    context
+        .assert_command("import source_distribution")
+        .success();
 
     // Re-run the installation in a new virtual environment.
     let parent = context.temp_dir.child("parent");
     parent.create_dir_all()?;
     let venv = create_venv(&parent, &context.cache_dir, "3.12");
 
-    uv_snapshot!(filters, command(&context)
+    uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--strict")
         .env("VIRTUAL_ENV", venv.as_os_str()), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Installed 1 package in [TIME]
-     + tqdm==4.66.1 (from https://files.pythonhosted.org/packages/62/06/d5604a70d160f6a6ca5fd2ba25597c24abd5c5ca5f437263d177ac242308/tqdm-4.66.1.tar.gz)
+     + source-distribution==0.0.1 (from https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz)
     "###
     );
 
-    context.assert_command("import tqdm").success();
+    context
+        .assert_command("import source_distribution")
+        .success();
 
     // Clear the cache, then re-run the installation in a new virtual environment.
     let parent = context.temp_dir.child("parent");
     parent.create_dir_all()?;
     let venv = create_venv(&parent, &context.cache_dir, "3.12");
 
     uv_snapshot!(Command::new(get_bin())
         .arg("clean")
-        .arg("tqdm")
+        .arg("source_distribution")
         .arg("--cache-dir")
         .arg(context.cache_dir.path())
         .env("VIRTUAL_ENV", venv.as_os_str())
         .current_dir(&context.temp_dir), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
-    Removed 127 files for tqdm ([SIZE])
+    Removed 13 files for source-distribution ([SIZE])
     "###
     );
 
-    uv_snapshot!(filters, command(&context)
+    uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--strict")
         .env("VIRTUAL_ENV", venv.as_os_str()), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Downloaded 1 package in [TIME]
     Installed 1 package in [TIME]
-     + tqdm==4.66.1 (from https://files.pythonhosted.org/packages/62/06/d5604a70d160f6a6ca5fd2ba25597c24abd5c5ca5f437263d177ac242308/tqdm-4.66.1.tar.gz)
+     + source-distribution==0.0.1 (from https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz)
     "###
     );
 
-    context.assert_command("import tqdm").success();
+    context
+        .assert_command("import source_distribution")
+        .success();
 
     Ok(())
 }
 
 /// Check that we show the right messages on cached, Git source distribution installs.
 #[test]
 #[cfg(feature = "git")]
 fn install_git_source_dist_cached() -> Result<()> {
     let context = TestContext::new("3.12");
 
     let requirements_txt = context.temp_dir.child("requirements.txt");
-    requirements_txt.write_str("werkzeug @ git+https://github.com/pallets/werkzeug.git@af160e0b6b7ddd81c22f1652c728ff5ac72d5c74")?;
+    requirements_txt.write_str("uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389")?;
 
     uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--strict"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Downloaded 1 package in [TIME]
     Installed 1 package in [TIME]
-     + werkzeug==2.0.0 (from git+https://github.com/pallets/werkzeug.git@af160e0b6b7ddd81c22f1652c728ff5ac72d5c74)
+     + uv-public-pypackage==0.1.0 (from git+https://github.com/astral-test/uv-public-pypackage@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389)
     "###
     );
 
-    context.assert_command("import werkzeug").success();
+    context
+        .assert_command("import uv_public_pypackage")
+        .success();
 
     // Re-run the installation in a new virtual environment.
     let parent = context.temp_dir.child("parent");
     parent.create_dir_all()?;
     let venv = create_venv(&parent, &context.cache_dir, "3.12");
 
     uv_snapshot!(command(&context)
@@ -1384,19 +1359,19 @@
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Installed 1 package in [TIME]
-     + werkzeug==2.0.0 (from git+https://github.com/pallets/werkzeug.git@af160e0b6b7ddd81c22f1652c728ff5ac72d5c74)
+     + uv-public-pypackage==0.1.0 (from git+https://github.com/astral-test/uv-public-pypackage@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389)
     "###
     );
 
-    check_command(&venv, "import werkzeug", &context.temp_dir);
+    check_command(&venv, "import uv_public_pypackage", &context.temp_dir);
 
     // Clear the cache, then re-run the installation in a new virtual environment.
     let parent = context.temp_dir.child("parent");
     parent.create_dir_all()?;
     let venv = create_venv(&parent, &context.cache_dir, "3.12");
 
     let filters = if cfg!(windows) {
@@ -1415,63 +1390,66 @@
         .env("VIRTUAL_ENV", venv.as_os_str())
         .current_dir(&context.temp_dir), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
-    Removed 4 files for werkzeug ([SIZE])
+    No cache entries found for werkzeug
     "###
     );
 
     uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--strict")
         .env("VIRTUAL_ENV", venv.as_os_str()), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
-    Downloaded 1 package in [TIME]
     Installed 1 package in [TIME]
-     + werkzeug==2.0.0 (from git+https://github.com/pallets/werkzeug.git@af160e0b6b7ddd81c22f1652c728ff5ac72d5c74)
+     + uv-public-pypackage==0.1.0 (from git+https://github.com/astral-test/uv-public-pypackage@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389)
     "###
     );
 
-    context.assert_command("import werkzeug").success();
+    context
+        .assert_command("import uv_public_pypackage")
+        .success();
 
     Ok(())
 }
 
 /// Check that we show the right messages on cached, registry source distribution installs.
 #[test]
 fn install_registry_source_dist_cached() -> Result<()> {
     let context = TestContext::new("3.12");
 
     let requirements_txt = context.temp_dir.child("requirements.txt");
-    requirements_txt.write_str("future==0.18.3")?;
+    requirements_txt.write_str("source_distribution==0.0.1")?;
 
     uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--strict"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Downloaded 1 package in [TIME]
     Installed 1 package in [TIME]
-     + future==0.18.3
+     + source-distribution==0.0.1
     "###
     );
 
-    context.assert_command("import future").success();
+    context
+        .assert_command("import source_distribution")
+        .success();
 
     // Re-run the installation in a new virtual environment.
     let parent = context.temp_dir.child("parent");
     parent.create_dir_all()?;
     let venv = create_venv(&parent, &context.cache_dir, "3.12");
 
     uv_snapshot!(command(&context)
@@ -1481,51 +1459,53 @@
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Installed 1 package in [TIME]
-     + future==0.18.3
+     + source-distribution==0.0.1
     "###
     );
 
-    context.assert_command("import future").success();
+    context
+        .assert_command("import source_distribution")
+        .success();
 
     // Clear the cache, then re-run the installation in a new virtual environment.
     let parent = context.temp_dir.child("parent");
     parent.create_dir_all()?;
     let venv = create_venv(&parent, &context.cache_dir, "3.12");
 
     let filters: Vec<(&str, &str)> = if cfg!(windows) {
         // On Windows, the number of files removed is different.
-        [("Removed 616 files", "Removed 617 files")]
+        [("Removed 13 files", "Removed 14 files")]
             .into_iter()
             .chain(context.filters())
             .collect()
     } else {
         // For some Linux distributions, like Gentoo, the number of files removed is different.
-        [("Removed 615 files", "Removed 617 files")]
+        [("Removed 12 files", "Removed 14 files")]
             .into_iter()
             .chain(context.filters())
             .collect()
     };
     uv_snapshot!(filters, Command::new(get_bin())
         .arg("clean")
-        .arg("future")
+        .arg("source_distribution")
         .arg("--cache-dir")
         .arg(context.cache_dir.path())
         .env("VIRTUAL_ENV", venv.as_os_str())
         .current_dir(&context.temp_dir), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
-    Removed 617 files for future ([SIZE])
+    Removed 14 files for source-distribution ([SIZE])
     "###
     );
 
     uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--strict")
         .env("VIRTUAL_ENV", venv.as_os_str()), @r###"
@@ -1533,56 +1513,60 @@
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Downloaded 1 package in [TIME]
     Installed 1 package in [TIME]
-     + future==0.18.3
+     + source-distribution==0.0.1
     "###
     );
 
-    context.assert_command("import future").success();
+    context
+        .assert_command("import source_distribution")
+        .success();
 
     Ok(())
 }
 
 /// Check that we show the right messages on cached, local source distribution installs.
 #[test]
 fn install_path_source_dist_cached() -> Result<()> {
     let context = TestContext::new("3.12");
 
     // Download a source distribution.
-    let response = reqwest::blocking::get("https://files.pythonhosted.org/packages/b0/b4/bc2baae3970c282fae6c2cb8e0f179923dceb7eaffb0e76170628f9af97b/wheel-0.42.0.tar.gz")?;
-    let archive = context.temp_dir.child("wheel-0.42.0.tar.gz");
+    let response = reqwest::blocking::get("https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz")?;
+    let archive = context.temp_dir.child("source_distribution-0.0.1.tar.gz");
     let mut archive_file = fs_err::File::create(archive.path())?;
     std::io::copy(&mut response.bytes()?.as_ref(), &mut archive_file)?;
 
     let requirements_txt = context.temp_dir.child("requirements.txt");
     requirements_txt.write_str(&format!(
-        "wheel @ {}",
+        "source-distribution @ {}",
         Url::from_file_path(archive.path()).unwrap()
     ))?;
 
     uv_snapshot!(context.filters(), command(&context)
         .arg("requirements.txt")
         .arg("--strict"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Downloaded 1 package in [TIME]
     Installed 1 package in [TIME]
-     + wheel==0.42.0 (from file://[TEMP_DIR]/wheel-0.42.0.tar.gz)
+     + source-distribution==0.0.1 (from file://[TEMP_DIR]/source_distribution-0.0.1.tar.gz)
     "###
     );
 
-    context.assert_command("import wheel").success();
+    context
+        .assert_command("import source_distribution")
+        .success();
 
     // Re-run the installation in a new virtual environment.
     let parent = context.temp_dir.child("parent");
     parent.create_dir_all()?;
     let venv = create_venv(&parent, &context.cache_dir, "3.12");
 
     uv_snapshot!(context.filters(), command(&context)
@@ -1592,46 +1576,40 @@
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Installed 1 package in [TIME]
-     + wheel==0.42.0 (from file://[TEMP_DIR]/wheel-0.42.0.tar.gz)
+     + source-distribution==0.0.1 (from file://[TEMP_DIR]/source_distribution-0.0.1.tar.gz)
     "###
     );
 
-    context.assert_command("import wheel").success();
+    context
+        .assert_command("import source_distribution")
+        .success();
 
     // Clear the cache, then re-run the installation in a new virtual environment.
     let parent = context.temp_dir.child("parent");
     parent.create_dir_all()?;
     let venv = create_venv(&parent, &context.cache_dir, "3.12");
 
-    let filters = if cfg!(windows) {
-        [("Removed 3 files", "Removed 4 files")]
-            .into_iter()
-            .chain(context.filters())
-            .collect()
-    } else {
-        context.filters()
-    };
-    uv_snapshot!(filters, Command::new(get_bin())
+    uv_snapshot!(Command::new(get_bin())
         .arg("clean")
-        .arg("wheel")
+        .arg("source-distribution")
         .arg("--cache-dir")
         .arg(context.cache_dir.path())
         .env("VIRTUAL_ENV", venv.as_os_str())
         .current_dir(&context.temp_dir), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
-    Removed 103 files for wheel ([SIZE])
+    Removed 13 files for source-distribution ([SIZE])
     "###
     );
 
     uv_snapshot!(context.filters(), command(&context)
         .arg("requirements.txt")
         .arg("--strict")
         .env("VIRTUAL_ENV", venv.as_os_str()), @r###"
@@ -1639,19 +1617,21 @@
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Downloaded 1 package in [TIME]
     Installed 1 package in [TIME]
-     + wheel==0.42.0 (from file://[TEMP_DIR]/wheel-0.42.0.tar.gz)
+     + source-distribution==0.0.1 (from file://[TEMP_DIR]/source_distribution-0.0.1.tar.gz)
     "###
     );
 
-    context.assert_command("import wheel").success();
+    context
+        .assert_command("import source_distribution")
+        .success();
 
     Ok(())
 }
 
 /// Check that we show the right messages on cached, local source distribution installs.
 #[test]
 fn install_path_built_dist_cached() -> Result<()> {
@@ -2015,53 +1995,57 @@
 /// Verify that we can force reinstall of Git dependencies.
 #[test]
 #[cfg(feature = "git")]
 fn reinstall_git() -> Result<()> {
     let context = TestContext::new("3.12");
 
     let requirements_txt = context.temp_dir.child("requirements.txt");
-    requirements_txt.write_str("werkzeug @ git+https://github.com/pallets/werkzeug.git@af160e0b6b7ddd81c22f1652c728ff5ac72d5c74")?;
+    requirements_txt.write_str("uv-public-pypackage @ git+https://github.com/astral-test/uv-public-pypackage@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389")?;
 
     uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--strict"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Downloaded 1 package in [TIME]
     Installed 1 package in [TIME]
-     + werkzeug==2.0.0 (from git+https://github.com/pallets/werkzeug.git@af160e0b6b7ddd81c22f1652c728ff5ac72d5c74)
+     + uv-public-pypackage==0.1.0 (from git+https://github.com/astral-test/uv-public-pypackage@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389)
     "###
     );
 
-    context.assert_command("import werkzeug").success();
+    context
+        .assert_command("import uv_public_pypackage")
+        .success();
 
     // Re-run the installation with `--reinstall`.
     uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--reinstall-package")
-        .arg("WerkZeug")
+        .arg("uv-public-pypackage")
         .arg("--strict"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Uninstalled 1 package in [TIME]
     Installed 1 package in [TIME]
-     - werkzeug==2.0.0 (from git+https://github.com/pallets/werkzeug.git@af160e0b6b7ddd81c22f1652c728ff5ac72d5c74)
-     + werkzeug==2.0.0 (from git+https://github.com/pallets/werkzeug.git@af160e0b6b7ddd81c22f1652c728ff5ac72d5c74)
+     - uv-public-pypackage==0.1.0 (from git+https://github.com/astral-test/uv-public-pypackage@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389)
+     + uv-public-pypackage==0.1.0 (from git+https://github.com/astral-test/uv-public-pypackage@b270df1a2fb5d012294e9aaf05e7e0bab1e6a389)
     "###
     );
 
-    context.assert_command("import werkzeug").success();
+    context
+        .assert_command("import uv_public_pypackage")
+        .success();
 
     Ok(())
 }
 
 /// Verify that we can force refresh of cached data.
 #[test]
 fn refresh() -> Result<()> {
@@ -3565,30 +3549,30 @@
 /// Include the hash for _just_ the source distribution with `--no-binary`.
 #[test]
 fn require_hashes_source_no_binary() -> Result<()> {
     let context = TestContext::new("3.12");
 
     let requirements_txt = context.temp_dir.child("requirements.txt");
     requirements_txt
-        .write_str("anyio==4.0.0 --hash=sha256:f7ed51751b2c2add651e5747c891b47e26d2a21be5d32d9311dfe9692f3e5d7a")?;
+        .write_str("source-distribution==0.0.1 --hash=sha256:1f83ed7498336c7f2ab9b002cf22583d91115ebc624053dc4eb3a45694490106")?;
 
     uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--no-binary")
         .arg(":all:")
         .arg("--require-hashes"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Downloaded 1 package in [TIME]
     Installed 1 package in [TIME]
-     + anyio==4.0.0
+     + source-distribution==0.0.1
     "###
     );
 
     Ok(())
 }
 
 /// Include the hash for _just_ the source distribution, with `--binary-only`.
@@ -3695,28 +3679,28 @@
 /// Include the hash for a source distribution specified as a direct URL dependency.
 #[test]
 fn require_hashes_source_url() -> Result<()> {
     let context = TestContext::new("3.12");
 
     let requirements_txt = context.temp_dir.child("requirements.txt");
     requirements_txt
-        .write_str("anyio @ https://files.pythonhosted.org/packages/74/17/5075225ee1abbb93cd7fc30a2d343c6a3f5f71cf388f14768a7a38256581/anyio-4.0.0.tar.gz --hash=sha256:f7ed51751b2c2add651e5747c891b47e26d2a21be5d32d9311dfe9692f3e5d7a")?;
+        .write_str("source-distribution @ https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz --hash=sha256:1f83ed7498336c7f2ab9b002cf22583d91115ebc624053dc4eb3a45694490106")?;
 
     uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--require-hashes"), @r###"
     success: true
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Downloaded 1 package in [TIME]
     Installed 1 package in [TIME]
-     + anyio==4.0.0 (from https://files.pythonhosted.org/packages/74/17/5075225ee1abbb93cd7fc30a2d343c6a3f5f71cf388f14768a7a38256581/anyio-4.0.0.tar.gz)
+     + source-distribution==0.0.1 (from https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz)
     "###
     );
 
     // Reinstall with the right hash, and verify that it's reused.
     uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--reinstall")
@@ -3725,72 +3709,72 @@
     exit_code: 0
     ----- stdout -----
 
     ----- stderr -----
     Resolved 1 package in [TIME]
     Uninstalled 1 package in [TIME]
     Installed 1 package in [TIME]
-     - anyio==4.0.0 (from https://files.pythonhosted.org/packages/74/17/5075225ee1abbb93cd7fc30a2d343c6a3f5f71cf388f14768a7a38256581/anyio-4.0.0.tar.gz)
-     + anyio==4.0.0 (from https://files.pythonhosted.org/packages/74/17/5075225ee1abbb93cd7fc30a2d343c6a3f5f71cf388f14768a7a38256581/anyio-4.0.0.tar.gz)
+     - source-distribution==0.0.1 (from https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz)
+     + source-distribution==0.0.1 (from https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz)
     "###
     );
 
     // Reinstall with the wrong hash, and verify that it's rejected despite being cached.
     let requirements_txt = context.temp_dir.child("requirements.txt");
     requirements_txt
-        .write_str("anyio @ https://files.pythonhosted.org/packages/74/17/5075225ee1abbb93cd7fc30a2d343c6a3f5f71cf388f14768a7a38256581/anyio-4.0.0.tar.gz --hash=sha256:a7ed51751b2c2add651e5747c891b47e26d2a21be5d32d9311dfe9692f3e5d7a")?;
+        .write_str("source-distribution @ https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz --hash=sha256:a7ed51751b2c2add651e5747c891b47e26d2a21be5d32d9311dfe9692f3e5d7a")?;
 
     uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--reinstall")
         .arg("--require-hashes"), @r###"
     success: false
     exit_code: 2
     ----- stdout -----
 
     ----- stderr -----
-    error: Failed to download and build `anyio @ https://files.pythonhosted.org/packages/74/17/5075225ee1abbb93cd7fc30a2d343c6a3f5f71cf388f14768a7a38256581/anyio-4.0.0.tar.gz`
-      Caused by: Hash mismatch for `anyio @ https://files.pythonhosted.org/packages/74/17/5075225ee1abbb93cd7fc30a2d343c6a3f5f71cf388f14768a7a38256581/anyio-4.0.0.tar.gz`
+    error: Failed to download and build `source-distribution @ https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz`
+      Caused by: Hash mismatch for `source-distribution @ https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz`
 
     Expected:
       sha256:a7ed51751b2c2add651e5747c891b47e26d2a21be5d32d9311dfe9692f3e5d7a
 
     Computed:
-      sha256:f7ed51751b2c2add651e5747c891b47e26d2a21be5d32d9311dfe9692f3e5d7a
+      sha256:1f83ed7498336c7f2ab9b002cf22583d91115ebc624053dc4eb3a45694490106
     "###
     );
 
     Ok(())
 }
 
 /// Include the _wrong_ hash for a source distribution specified as a direct URL dependency.
 #[test]
 fn require_hashes_source_url_mismatch() -> Result<()> {
     let context = TestContext::new("3.12");
 
     let requirements_txt = context.temp_dir.child("requirements.txt");
     requirements_txt
-        .write_str("anyio @ https://files.pythonhosted.org/packages/74/17/5075225ee1abbb93cd7fc30a2d343c6a3f5f71cf388f14768a7a38256581/anyio-4.0.0.tar.gz --hash=sha256:a7ed51751b2c2add651e5747c891b47e26d2a21be5d32d9311dfe9692f3e5d7a")?;
+        .write_str("source-distribution @ https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz --hash=sha256:a7ed51751b2c2add651e5747c891b47e26d2a21be5d32d9311dfe9692f3e5d7a")?;
 
     uv_snapshot!(command(&context)
         .arg("requirements.txt")
         .arg("--require-hashes"), @r###"
     success: false
     exit_code: 2
     ----- stdout -----
 
     ----- stderr -----
-    error: Failed to download and build `anyio @ https://files.pythonhosted.org/packages/74/17/5075225ee1abbb93cd7fc30a2d343c6a3f5f71cf388f14768a7a38256581/anyio-4.0.0.tar.gz`
-      Caused by: Hash mismatch for `anyio @ https://files.pythonhosted.org/packages/74/17/5075225ee1abbb93cd7fc30a2d343c6a3f5f71cf388f14768a7a38256581/anyio-4.0.0.tar.gz`
+    error: Failed to download and build `source-distribution @ https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz`
+      Caused by: Hash mismatch for `source-distribution @ https://files.pythonhosted.org/packages/10/1f/57aa4cce1b1abf6b433106676e15f9fa2c92ed2bd4cf77c3b50a9e9ac773/source_distribution-0.0.1.tar.gz`
 
     Expected:
       sha256:a7ed51751b2c2add651e5747c891b47e26d2a21be5d32d9311dfe9692f3e5d7a
 
     Computed:
-      sha256:f7ed51751b2c2add651e5747c891b47e26d2a21be5d32d9311dfe9692f3e5d7a
+      sha256:1f83ed7498336c7f2ab9b002cf22583d91115ebc624053dc4eb3a45694490106
     "###
     );
 
     Ok(())
 }
 
 /// Include the hash for a built distribution specified as a direct URL dependency.
```

### Comparing `uv-0.2.2/crates/uv/tests/pip_uninstall.rs` & `uv-0.2.3/crates/uv/tests/pip_uninstall.rs`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         .arg("flask==1.0.x")
         .current_dir(&temp_dir), @r###"
     success: false
     exit_code: 2
     ----- stdout -----
 
     ----- stderr -----
-    error: Failed to parse `flask==1.0.x`
+    error: Failed to parse: `flask==1.0.x`
       Caused by: after parsing '1.0', found '.x', which is not part of a valid version
     flask==1.0.x
          ^^^^^^^
     "###);
 
     Ok(())
 }
```

### Comparing `uv-0.2.2/crates/uv/tests/self_update.rs` & `uv-0.2.3/crates/uv/tests/self_update.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/crates/uv/tests/venv.rs` & `uv-0.2.3/crates/uv/tests/venv.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/Cargo.lock` & `uv-0.2.3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -391,21 +391,23 @@
 version = "0.0.0"
 dependencies = [
  "anyhow",
  "codspeed-criterion-compat",
  "criterion",
  "distribution-filename",
  "distribution-types",
+ "install-wheel-rs",
  "once_cell",
  "pep508_rs",
  "platform-tags",
  "tokio",
  "uv-cache",
  "uv-client",
  "uv-configuration",
+ "uv-dispatch",
  "uv-distribution",
  "uv-interpreter",
  "uv-resolver",
  "uv-types",
 ]
 
 [[package]]
@@ -1098,15 +1100,14 @@
 name = "distribution-types"
 version = "0.0.1"
 dependencies = [
  "anyhow",
  "cache-key",
  "distribution-filename",
  "fs-err",
- "git2",
  "indexmap",
  "itertools 0.13.0",
  "once_cell",
  "pep440_rs",
  "pep508_rs",
  "platform-tags",
  "pypi-types",
@@ -1801,15 +1802,14 @@
 checksum = "763a5a8f45087d6bcea4222e7b72c291a054edf80e4ef6efd2a4979878c7bea3"
 dependencies = [
  "console",
  "instant",
  "number_prefix",
  "portable-atomic",
  "unicode-width",
- "vt100",
 ]
 
 [[package]]
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
@@ -2483,14 +2483,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07ba0ad7e047712414213ff67533e6dd477af0a4e1d14fb52343e53d30ea9397"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
+name = "path-slash"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1e91099d4268b0e11973f036e885d652fb0b21fedcf69738c627f94db6a44f42"
+
+[[package]]
 name = "pathdiff"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8835116a5c179084a830efb3adc117ab007512b535bc1a21c991d3b32a6b44dd"
 
 [[package]]
 name = "pep440_rs"
@@ -2854,27 +2860,30 @@
  "syn 2.0.64",
 ]
 
 [[package]]
 name = "pypi-types"
 version = "0.0.1"
 dependencies = [
+ "anyhow",
  "chrono",
+ "git2",
  "indexmap",
  "mailparse",
  "once_cell",
  "pep440_rs",
  "pep508_rs",
  "regex",
  "rkyv",
  "serde",
  "thiserror",
  "toml",
  "tracing",
  "url",
+ "uv-git",
  "uv-normalize",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3070,20 +3079,20 @@
  "assert_fs",
  "distribution-types",
  "fs-err",
  "indoc",
  "insta",
  "itertools 0.13.0",
  "pep508_rs",
+ "pypi-types",
  "regex",
  "reqwest",
  "reqwest-middleware",
  "tempfile",
  "test-case",
- "thiserror",
  "tokio",
  "tracing",
  "unscanny",
  "url",
  "uv-client",
  "uv-configuration",
  "uv-fs",
@@ -4229,26 +4238,14 @@
  "serde_json",
  "svg",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
-name = "tracing-indicatif"
-version = "0.3.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "069580424efe11d97c3fef4197fa98c004fa26672cc71ad8770d224e23b1951d"
-dependencies = [
- "indicatif",
- "tracing",
- "tracing-core",
- "tracing-subscriber",
-]
-
-[[package]]
 name = "tracing-log"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee855f1f400bd0e5c02d150ae5de3840039a3f54b025156404e34c23c03f47c3"
 dependencies = [
  "log",
  "once_cell",
@@ -4470,15 +4467,15 @@
 name = "uuid"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 
 [[package]]
 name = "uv"
-version = "0.2.2"
+version = "0.2.3"
 dependencies = [
  "anstream",
  "anyhow",
  "assert_cmd",
  "assert_fs",
  "axoupdater",
  "base64 0.22.1",
@@ -4499,14 +4496,15 @@
  "miette",
  "mimalloc",
  "owo-colors",
  "pep440_rs",
  "pep508_rs",
  "platform-tags",
  "predicates",
+ "pypi-types",
  "rayon",
  "regex",
  "requirements-txt",
  "reqwest",
  "rustc-hash",
  "serde",
  "serde_json",
@@ -4573,14 +4571,15 @@
  "fs-err",
  "indoc",
  "insta",
  "itertools 0.13.0",
  "once_cell",
  "pep440_rs",
  "pep508_rs",
+ "pypi-types",
  "regex",
  "rustc-hash",
  "serde",
  "serde_json",
  "tempfile",
  "thiserror",
  "tokio",
@@ -4668,15 +4667,15 @@
 [[package]]
 name = "uv-configuration"
 version = "0.0.1"
 dependencies = [
  "anyhow",
  "clap",
  "distribution-types",
- "itertools 0.13.0",
+ "either",
  "pep508_rs",
  "platform-tags",
  "rustc-hash",
  "schemars",
  "serde",
  "serde_json",
  "tracing",
@@ -4698,25 +4697,25 @@
  "install-wheel-rs",
  "itertools 0.13.0",
  "mimalloc",
  "owo-colors",
  "pep508_rs",
  "poloto",
  "pretty_assertions",
+ "pypi-types",
  "resvg",
  "rustc-hash",
  "schemars",
  "serde",
  "serde_json",
  "tagu",
  "tikv-jemallocator",
  "tokio",
  "tracing",
  "tracing-durations-export",
- "tracing-indicatif",
  "tracing-subscriber",
  "uv-build",
  "uv-cache",
  "uv-client",
  "uv-configuration",
  "uv-dispatch",
  "uv-fs",
@@ -4814,20 +4813,22 @@
 [[package]]
 name = "uv-fs"
 version = "0.0.1"
 dependencies = [
  "backoff",
  "cachedir",
  "dunce",
+ "either",
  "encoding_rs_io",
  "fs-err",
  "fs2",
  "junction",
  "once_cell",
  "path-absolutize",
+ "path-slash",
  "tempfile",
  "tracing",
  "urlencoding",
  "uv-warnings",
 ]
 
 [[package]]
@@ -5052,15 +5053,15 @@
  "uv-configuration",
  "uv-interpreter",
  "uv-normalize",
 ]
 
 [[package]]
 name = "uv-version"
-version = "0.2.2"
+version = "0.2.3"
 
 [[package]]
 name = "uv-virtualenv"
 version = "0.0.4"
 dependencies = [
  "fs-err",
  "itertools 0.13.0",
@@ -5120,47 +5121,14 @@
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
-name = "vt100"
-version = "0.15.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84cd863bf0db7e392ba3bd04994be3473491b31e66340672af5d11943c6274de"
-dependencies = [
- "itoa",
- "log",
- "unicode-width",
- "vte",
-]
-
-[[package]]
-name = "vte"
-version = "0.11.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f5022b5fbf9407086c180e9557be968742d839e68346af7792b8592489732197"
-dependencies = [
- "arrayvec",
- "utf8parse",
- "vte_generate_state_changes",
-]
-
-[[package]]
-name = "vte_generate_state_changes"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d257817081c7dffcdbab24b9e62d2def62e2ff7d00b1c20062551e6cccc145ff"
-dependencies = [
- "proc-macro2",
- "quote",
-]
-
-[[package]]
 name = "wait-timeout"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f200f5b12eb75f8c1ed65abd4b2db8a6e1b138a20de009dacee265a2498f3f6"
 dependencies = [
  "libc",
 ]
```

### Comparing `uv-0.2.2/Cargo.toml` & `uv-0.2.3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 ctrlc = { version = "3.4.4" }
 dashmap = { version = "5.5.3" }
 data-encoding = { version = "2.5.0" }
 derivative = { version = "2.2.0" }
 directories = { version = "5.0.1" }
 dirs-sys = { version = "0.4.1" }
 dunce = { version = "1.0.4" }
-either = { version = "1.9.0" }
+either = { version = "1.12.0" }
 encoding_rs_io = { version = "0.1.7" }
 flate2 = { version = "1.0.28", default-features = false }
 fs-err = { version = "2.11.0" }
 fs2 = { version = "0.4.3" }
 futures = { version = "0.3.30" }
 git2 = { version = "0.18.1" }
 glob = { version = "0.3.1" }
@@ -94,14 +94,15 @@
 mailparse = { version = "0.15.0" }
 md-5 = { version = "0.10.6" }
 miette = { version = "7.2.0" }
 nanoid = { version = "0.4.0" }
 once_cell = { version = "1.19.0" }
 owo-colors = { version = "4.0.0" }
 path-absolutize = { version = "3.1.1" }
+path-slash = { version = "0.2.1" }
 pathdiff = { version = "0.2.1" }
 petgraph = { version = "0.6.4" }
 platform-info = { version = "2.0.2" }
 pubgrub = { git = "https://github.com/astral-sh/pubgrub", rev = "0e684a874c9fb8f74738cd8875524c80e3d4820b" }
 pyo3 = { version = "0.21.0" }
 pyo3-log = { version = "0.10.0" }
 rand = { version = "0.8.5" }
@@ -130,15 +131,14 @@
 tokio = { version = "1.35.1", features = ["fs", "io-util", "macros", "process", "rt-multi-thread", "sync"] }
 tokio-stream = { version = "0.1.14" }
 tokio-tar = { version = "0.3.1" }
 tokio-util = { version = "0.7.10", features = ["compat"] }
 toml = { version = "0.8.12" }
 tracing = { version = "0.1.40" }
 tracing-durations-export = { version = "0.2.0", features = ["plot"] }
-tracing-indicatif = { version = "0.3.6" }
 tracing-subscriber = { version = "0.3.18", features = ["env-filter", "json", "registry"] }
 tracing-tree = { version = "0.3.0" }
 unicode-width = { version = "0.1.11" }
 unscanny = { version = "0.1.0" }
 url = { version = "2.5.0" }
 urlencoding = { version = "2.1.3" }
 wiremock = { version = "0.6.0" }
@@ -211,15 +211,14 @@
 # The archive format to use for windows builds (defaults .zip)
 windows-archive = ".zip"
 # The archive format to use for non-windows builds (defaults .tar.xz)
 unix-archive = ".tar.gz"
 # Target platforms to build apps for (Rust target-triple syntax)
 targets = [
   "aarch64-apple-darwin",
-  "aarch64-unknown-linux-gnu",
   "aarch64-unknown-linux-musl",
   "arm-unknown-linux-musleabihf",
   "armv7-unknown-linux-gnueabihf",
   "armv7-unknown-linux-musleabihf",
   "i686-pc-windows-msvc",
   "i686-unknown-linux-gnu",
   "i686-unknown-linux-musl",
```

### Comparing `uv-0.2.2/pyproject.toml` & `uv-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "uv"
-version = "0.2.2"
+version = "0.2.3"
 description = "An extremely fast Python package installer and resolver, written in Rust."
 authors = [{ name = "Astral Software Inc.", email = "hey@astral.sh" }]
 requires-python = ">=3.8"
 keywords = [
   "uv", "requirements", "packaging"
 ]
 classifiers = [
```

### Comparing `uv-0.2.2/python/uv/__main__.py` & `uv-0.2.3/python/uv/__main__.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/python/uv/__init__.py` & `uv-0.2.3/python/uv/__init__.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/README.md` & `uv-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/LICENSE-APACHE` & `uv-0.2.3/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/LICENSE-MIT` & `uv-0.2.3/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `uv-0.2.2/PKG-INFO` & `uv-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: uv
-Version: 0.2.2
+Version: 0.2.3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

