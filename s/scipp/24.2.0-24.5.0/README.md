# Comparing `tmp/scipp-24.2.0.tar.gz` & `tmp/scipp-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipp-24.2.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "scipp-24.5.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `scipp-24.2.0.tar` & `scipp-24.5.0.tar`

### file list

```diff
@@ -1,883 +1,880 @@
--rw-r--r--   0        0        0      462 2022-11-09 12:37:21.000000 scipp-24.2.0/.buildconfig/ci-linux.yml
--rw-r--r--   0        0        0      383 2022-11-09 12:37:21.000000 scipp-24.2.0/.buildconfig/ci-macos.yml
--rw-r--r--   0        0        0      385 2022-11-09 12:37:21.000000 scipp-24.2.0/.buildconfig/ci-windows.yml
--rw-r--r--   0        0        0       59 2022-11-09 12:37:21.000000 scipp-24.2.0/.clang-format
--rw-r--r--   0        0        0     6160 2022-11-09 12:37:21.000000 scipp-24.2.0/.clang-tidy
--rw-r--r--   0        0        0      574 2022-11-09 12:37:21.000000 scipp-24.2.0/.cmake-format.json
--rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 scipp-24.2.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0      454 2022-11-09 12:37:21.000000 scipp-24.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1594 2022-11-09 12:37:21.000000 scipp-24.2.0/.github/workflows/conda.yml
--rw-r--r--   0        0        0     2103 2022-11-09 12:37:21.000000 scipp-24.2.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     2141 2022-11-09 12:37:21.000000 scipp-24.2.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     2955 2022-11-09 12:37:21.000000 scipp-24.2.0/.github/workflows/pr_and_main.yml
--rw-r--r--   0        0        0     1005 2022-11-09 12:37:21.000000 scipp-24.2.0/.github/workflows/release-nightly.yml
--rw-r--r--   0        0        0     4933 2022-11-09 12:37:21.000000 scipp-24.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      351 2022-11-09 12:37:21.000000 scipp-24.2.0/.github/workflows/rename-dev-wheels.py
--rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 scipp-24.2.0/.github/workflows/weekly.yml
--rw-r--r--   0        0        0      913 2022-11-09 12:37:21.000000 scipp-24.2.0/.github/workflows/wheel.yml
--rw-r--r--   0        0        0      623 2022-11-09 12:37:21.000000 scipp-24.2.0/.gitignore
--rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 scipp-24.2.0/.gitmodules
--rw-r--r--   0        0        0     2049 2022-11-09 12:37:21.000000 scipp-24.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 scipp-24.2.0/.vscode/settings.json
--rw-r--r--   0        0        0     2766 2022-11-09 12:37:21.000000 scipp-24.2.0/CMakeLists.txt
--rw-r--r--   0        0        0     3965 2022-11-09 12:37:21.000000 scipp-24.2.0/CMakePresets.json
--rw-r--r--   0        0        0     5479 2022-11-09 12:37:21.000000 scipp-24.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 scipp-24.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1553 2022-11-09 12:37:21.000000 scipp-24.2.0/LICENSE
--rw-r--r--   0        0        0      112 2022-11-09 12:37:21.000000 scipp-24.2.0/MANIFEST.in
--rw-r--r--   0        0        0     1842 2022-11-09 12:37:21.000000 scipp-24.2.0/README.md
--rw-r--r--   0        0        0     1453 2022-11-09 12:37:21.000000 scipp-24.2.0/asv.conf.json
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 scipp-24.2.0/benchmarks/__init__.py
--rw-r--r--   0        0        0     2622 2022-11-09 12:37:21.000000 scipp-24.2.0/benchmarks/bin.py
--rw-r--r--   0        0        0     3474 2022-11-09 12:37:21.000000 scipp-24.2.0/benchmarks/binned.py
--rw-r--r--   0        0        0      650 2022-11-09 12:37:21.000000 scipp-24.2.0/benchmarks/variable.py
--rw-r--r--   0        0        0      639 2022-11-09 12:37:21.000000 scipp-24.2.0/cmake/docs.cmake
--rw-r--r--   0        0        0     1162 2022-11-09 12:37:21.000000 scipp-24.2.0/conda/README.md
--rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 scipp-24.2.0/conda/cmake-package-test/CMakeLists.txt
--rw-r--r--   0        0        0      223 2022-11-09 12:37:21.000000 scipp-24.2.0/conda/cmake-package-test/README.md
--rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 scipp-24.2.0/conda/cmake-package-test/build.py
--rw-r--r--   0        0        0       80 2022-11-09 12:37:21.000000 scipp-24.2.0/conda/cmake-package-test/main.cpp
--rw-r--r--   0        0        0     2786 2022-11-09 12:37:21.000000 scipp-24.2.0/conda/meta.yaml
--rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 scipp-24.2.0/conda/variants/linux_64.yaml
--rw-r--r--   0        0        0       71 2022-11-09 12:37:21.000000 scipp-24.2.0/conda/variants/osx_64.yaml
--rw-r--r--   0        0        0       74 2022-11-09 12:37:21.000000 scipp-24.2.0/conda/variants/osx_arm64.yaml
--rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 scipp-24.2.0/conda/variants/win_64.yaml
--rw-r--r--   0        0        0     1409 2022-11-09 12:37:21.000000 scipp-24.2.0/cppcheck-suppressions.txt
--rw-r--r--   0        0        0      105 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/.gitignore
--rw-r--r--   0        0        0     4458 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/_static/anaconda-icon.js
--rw-r--r--   0        0        0   137750 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/_static/favicon.ico
--rw-r--r--   0        0        0    12917 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/_static/logo-2022.svg
--rw-r--r--   0        0        0    13113 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/_static/logo-dark.svg
--rw-r--r--   0        0        0   152456 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/_static/title-filtering-1d-plot.svg
--rw-r--r--   0        0        0    59695 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/_static/title-repr-html.png
--rw-r--r--   0        0        0    90813 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/_static/title-show-svg.png
--rw-r--r--   0        0        0      176 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/_templates/doc_version.html
--rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/_templates/scipp-class-template.rst
--rw-r--r--   0        0        0     1217 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/_templates/scipp-module-template.rst
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/_templates/scipp-sphinxext-template.rst
--rw-r--r--   0        0        0      112 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/_templates/scipp-type-template.rst
--rw-r--r--   0        0        0     3079 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/about/about.rst
--rw-r--r--   0        0        0     2145 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/about/contributing.rst
--rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/about/index.rst
--rw-r--r--   0        0        0     5355 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/about/migration/23-01.ipynb
--rw-r--r--   0        0        0       88 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/about/migration-notes.rst
--rw-r--r--   0        0        0    66489 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/about/release-notes.rst
--rw-r--r--   0        0        0     1490 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/about/roadmap.rst
--rw-r--r--   0        0        0     8600 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/conf.py
--rw-r--r--   0        0        0     2336 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0001-remove-dataset-masking-support.rst
--rw-r--r--   0        0        0     1353 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0002-remove-instrument-view-projection-options.rst
--rw-r--r--   0        0        0     3017 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0003-refactor-plotting-code-with-mvc-pattern.rst
--rw-r--r--   0        0        0      975 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0004-use-ipympl-backend-for-matplotlib.rst
--rw-r--r--   0        0        0     1618 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0005-remove-need-for-bins-property-when-calling-bin-or-histogram.rst
--rw-r--r--   0        0        0     3389 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0006-add-readonly-flags.rst
--rw-r--r--   0        0        0     1900 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0007-do-not-support-args-referencing-x-or-y.rst
--rw-r--r--   0        0        0     2534 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0008-consistent-multi-dimensional-coords.rst
--rw-r--r--   0        0        0     1570 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0009-handle-dimensionless-as-non-counts.rst
--rw-r--r--   0        0        0     2327 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0010-acknowledge-stability-and-maintainability-tasks.rst
--rw-r--r--   0        0        0     9772 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0011-renaming-of-dimensions-in-transform_coords.rst
--rw-r--r--   0        0        0     3847 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0012-rebin-should-apply-irreducible-masks.rst
--rw-r--r--   0        0        0     4061 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0013-plot-should-not-resample-automatically.rst
--rw-r--r--   0        0        0     4264 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0014-switch-calendar-versioning.rst
--rw-r--r--   0        0        0     1737 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0015-disable-support-for-broadcasting-variances.rst
--rw-r--r--   0        0        0     6585 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0016-do-not-support-attrs.rst
--rw-r--r--   0        0        0     6379 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/adr/0017-restrict-dataset-to-items-with-matching-dimensionality.rst
--rw-r--r--   0        0        0      110 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/architecture-decision-records.rst
--rw-r--r--   0        0        0     5369 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/coding-conventions.rst
--rw-r--r--   0        0        0     4300 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/dependencies.rst
--rw-r--r--   0        0        0     8687 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/getting-started.rst
--rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/index.rst
--rw-r--r--   0        0        0     8234 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/internals/concepts.ipynb
--rw-r--r--   0        0        0     2358 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/internals/constructing_variables.rst
--rw-r--r--   0        0        0     1499 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/internals/customizing.rst
--rw-r--r--   0        0        0      173 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/internals/index.rst
--rw-r--r--   0        0        0     8157 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/internals/multi_dimensional_indexing.rst
--rw-r--r--   0        0        0     5063 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/internals/transform.rst
--rw-r--r--   0        0        0     3723 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/internals/variable_implementation.rst
--rw-r--r--   0        0        0     4213 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/notebook-style-guide.ipynb
--rw-r--r--   0        0        0    16406 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/project/scipp-as-cpp-or-python-library.md
--rw-r--r--   0        0        0     2924 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/releasing-scipp.rst
--rw-r--r--   0        0        0     1685 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/development/tooling.rst
--rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/doxygen_index.md
--rw-r--r--   0        0        0      616 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/environments/developer.yml
--rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/environments/scipp.yml
--rw-r--r--   0        0        0     5905 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/getting-started/faq.rst
--rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/getting-started/index.rst
--rw-r--r--   0        0        0     3316 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/getting-started/installation.rst
--rw-r--r--   0        0        0     8120 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/getting-started/overview.rst
--rw-r--r--   0        0        0     5100 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/getting-started/quick-start.ipynb
--rw-r--r--   0        0        0        5 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/getting-started/tutorials/.gitignore
--rw-r--r--   0        0        0    22829 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/getting-started/tutorials/from-tabular-data-to-binned-data.ipynb
--rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/getting-started/tutorials/index.rst
--rw-r--r--   0        0        0     8886 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/getting-started/tutorials/prepare_data_rhessi.py
--rw-r--r--   0        0        0    38255 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/getting-started/tutorials/solar_flares.ipynb
--rw-r--r--   0        0        0    37305 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/multi_dimensional_indexing/multi_index_binned_1d_setups.svg
--rw-r--r--   0        0        0    27965 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/multi_dimensional_indexing/multi_index_binned_2d_setups.svg
--rw-r--r--   0        0        0    30700 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/multi_dimensional_indexing/multi_index_dense_setups.svg
--rw-r--r--   0        0        0   122317 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/multi_dimensional_indexing/view_index_delta.svg
--rw-r--r--   0        0        0    34041 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/multi_dimensional_indexing/view_index_flattening.svg
--rw-r--r--   0        0        0    46617 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/multi_dimensional_indexing/view_index_increment_full.svg
--rw-r--r--   0        0        0    37002 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/multi_dimensional_indexing/view_index_increment_partial.svg
--rw-r--r--   0        0        0    71142 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/plotting-1d-keep-event.png
--rw-r--r--   0        0        0    81853 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/plotting-1d-pick-event.png
--rw-r--r--   0        0        0    85238 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/plotting-1d-slider-event.png
--rw-r--r--   0        0        0    78661 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/plotting-2d-slider-event.png
--rw-r--r--   0        0        0    60702 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/transform_coords/base_rules.svg
--rw-r--r--   0        0        0   127544 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/transform_coords/cycle-contraction.svg
--rw-r--r--   0        0        0    49251 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/transform_coords/cycle.svg
--rw-r--r--   0        0        0    56259 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/transform_coords/cycle_rules.svg
--rw-r--r--   0        0        0   137381 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/transform_coords/fractional-colors.svg
--rw-r--r--   0        0        0    83957 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/transform_coords/larger_examples.svg
--rw-r--r--   0        0        0    43658 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/transform_coords/slice-transform-concat.svg
--rw-r--r--   0        0        0    55508 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/transform_coords/split-join.svg
--rw-r--r--   0        0        0    66888 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/variable_classes.dia
--rw-r--r--   0        0        0    13207 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/images/variable_classes.svg
--rw-r--r--   0        0        0     5305 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/index.rst
--rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/reference/classes.rst
--rw-r--r--   0        0        0      337 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/reference/creation-functions.rst
--rw-r--r--   0        0        0     8279 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/reference/dtype.ipynb
--rw-r--r--   0        0        0     2875 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/reference/error-propagation.rst
--rw-r--r--   0        0        0     2885 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/reference/free-functions.rst
--rw-r--r--   0        0        0      242 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/reference/index.rst
--rw-r--r--   0        0        0     9492 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/reference/linear-algebra.ipynb
--rw-r--r--   0        0        0     6649 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/reference/logging.ipynb
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/reference/modules.rst
--rw-r--r--   0        0        0     8463 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/reference/ownership-mechanism-and-readonly-flags.ipynb
--rw-r--r--   0        0        0     3331 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/reference/testing.rst
--rw-r--r--   0        0        0    20494 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/reference/units.ipynb
--rw-r--r--   0        0        0    14159 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/binned-data/binned-data.ipynb
--rw-r--r--   0        0        0    14492 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/binned-data/computation.ipynb
--rw-r--r--   0        0        0    15065 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/binned-data/filtering.ipynb
--rw-r--r--   0        0        0     7744 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/binned-data/histogramming-grouping-and-binning.ipynb
--rw-r--r--   0        0        0     1344 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/binned-data/prepare-filtering-data.py
--rw-r--r--   0        0        0      184 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/binned-data.rst
--rw-r--r--   0        0        0    13947 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/computation.ipynb
--rw-r--r--   0        0        0    20717 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/coordinate-transformations.ipynb
--rw-r--r--   0        0        0    17883 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/data-structures/creating-arrays-and-datasets.ipynb
--rw-r--r--   0        0        0    19716 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/data-structures/data-structures.ipynb
--rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/data-structures.rst
--rw-r--r--   0        0        0     5950 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/groupby.ipynb
--rw-r--r--   0        0        0      269 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/index.rst
--rw-r--r--   0        0        0     7301 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/masking.ipynb
--rw-r--r--   0        0        0     8665 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/plotting.ipynb
--rw-r--r--   0        0        0     6055 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/reading-and-writing-files.ipynb
--rw-r--r--   0        0        0    12308 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/representations-and-tables.ipynb
--rw-r--r--   0        0        0    27224 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/slicing.ipynb
--rw-r--r--   0        0        0    21269 2022-11-09 12:37:21.000000 scipp-24.2.0/docs/user-guide/tips-tricks-and-anti-patterns.ipynb
--rw-r--r--   0        0        0     7122 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/CMakeLists.txt
--rw-r--r--   0        0        0     3224 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/CMakeLists.txt
--rw-r--r--   0        0        0     1972 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/accumulate_benchmark.cpp
--rw-r--r--   0        0        0     2253 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/bin_benchmark.cpp
--rw-r--r--   0        0        0     2777 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/buckets_benchmark.cpp
--rw-r--r--   0        0        0      988 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/common.h
--rw-r--r--   0        0        0     9097 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/dataset_benchmark.cpp
--rw-r--r--   0        0        0     6586 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/dataset_operations_benchmark.cpp
--rw-r--r--   0        0        0     2721 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/element_array_view_benchmark.cpp
--rw-r--r--   0        0        0     4358 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/events_histogram_op_benchmark.cpp
--rw-r--r--   0        0        0     4577 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/groupby_benchmark.cpp
--rw-r--r--   0        0        0     2193 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/histogram_benchmark.cpp
--rw-r--r--   0        0        0     6414 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/legacy_cow_ptr.h
--rw-r--r--   0        0        0    14878 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/legacy_dataset_benchmark.cpp
--rw-r--r--   0        0        0     9270 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/legacy_histogram_benchmark.cpp
--rw-r--r--   0        0        0     1028 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/multi_index_benchmark.cpp
--rw-r--r--   0        0        0     1969 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/slice_benchmark.cpp
--rw-r--r--   0        0        0    10108 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/transform_benchmark.cpp
--rw-r--r--   0        0        0     7050 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/variable_benchmark.cpp
--rw-r--r--   0        0        0      909 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/benchmark/variable_common.h
--rw-r--r--   0        0        0     3101 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/.conan-recipes/llnl-units/conanfile.py
--rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/.conan-recipes/pybind11/conandata.yml
--rw-r--r--   0        0        0     4988 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/.conan-recipes/pybind11/conanfile.py
--rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/.conan-recipes/pybind11/conanmanifest.txt
--rw-r--r--   0        0        0    29291 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/CodeCoverage.cmake
--rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/IPO.cmake
--rw-r--r--   0        0        0      174 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/generated.h.in
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/sanitizers-cmake/.git
--rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/sanitizers-cmake/.gitignore
--rw-r--r--   0        0        0     1518 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/sanitizers-cmake/CMakeLists.txt
--rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/sanitizers-cmake/LICENSE
--rw-r--r--   0        0        0     3474 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/sanitizers-cmake/README.md
--rw-r--r--   0        0        0     2144 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/sanitizers-cmake/cmake/FindASan.cmake
--rw-r--r--   0        0        0     2292 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/sanitizers-cmake/cmake/FindMSan.cmake
--rwxr-xr-x   0        0        0     3737 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/sanitizers-cmake/cmake/FindSanitizers.cmake
--rw-r--r--   0        0        0     2555 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/sanitizers-cmake/cmake/FindTSan.cmake
--rw-r--r--   0        0        0     1696 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/sanitizers-cmake/cmake/FindUBSan.cmake
--rwxr-xr-x   0        0        0     2011 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/sanitizers-cmake/cmake/asan-wrapper
--rwxr-xr-x   0        0        0     7684 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/sanitizers-cmake/cmake/sanitize-helpers.cmake
--rw-r--r--   0        0        0     2072 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/sanitizers-cmake/tests/CMakeLists.txt
--rw-r--r--   0        0        0     1513 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/sanitizers-cmake/tests/asan_test.cpp
--rw-r--r--   0        0        0     1513 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/sanitizers-cmake/tests/shortest.ext.test.cpp
--rw-r--r--   0        0        0     2560 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/scipp-conan.cmake
--rw-r--r--   0        0        0      910 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/scipp-config.cmake.in
--rw-r--r--   0        0        0     5641 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/scipp-functions.cmake
--rw-r--r--   0        0        0     1450 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/scipp-install.cmake
--rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/scipp-test.cmake
--rw-r--r--   0        0        0     3242 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/cmake/scipp-util.cmake
--rw-r--r--   0        0        0      763 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/common/CMakeLists.txt
--rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/common/include/scipp/common/constants.h
--rw-r--r--   0        0        0     1364 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/common/include/scipp/common/except.h
--rw-r--r--   0        0        0      810 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/common/include/scipp/common/index.h
--rw-r--r--   0        0        0     4952 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/common/include/scipp/common/index_composition.h
--rw-r--r--   0        0        0      836 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/common/include/scipp/common/initialization.h
--rw-r--r--   0        0        0     4796 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/common/include/scipp/common/numeric.h
--rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/common/include/scipp/common/overloaded.h
--rw-r--r--   0        0        0      582 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/common/include/scipp/common/ranges.h
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/common/include/scipp/common/span.h
--rw-r--r--   0        0        0    18029 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/common/include/scipp/common/span.hpp.in
--rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/common/test/CMakeLists.txt
--rw-r--r--   0        0        0     6395 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/common/test/index_test.cpp
--rw-r--r--   0        0        0     1499 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/common/test/isarange_test.cpp
--rw-r--r--   0        0        0     2078 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/common/test/islinspace_test.cpp
--rw-r--r--   0        0        0     2649 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/common/test/numeric_test.cpp
--rw-r--r--   0        0        0     2997 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/CMakeLists.txt
--rw-r--r--   0        0        0     1146 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/dict.cpp
--rw-r--r--   0        0        0     5723 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/dimensions.cpp
--rw-r--r--   0        0        0     2201 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/dtype.cpp
--rw-r--r--   0        0        0     3184 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/element_array_view.cpp
--rw-r--r--   0        0        0     3965 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/except.cpp
--rw-r--r--   0        0        0     5011 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/aligned_allocator.h
--rw-r--r--   0        0        0     2878 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/array_to_string.h
--rw-r--r--   0        0        0      599 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/bucket.h
--rw-r--r--   0        0        0     2409 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/bucket_array_view.h
--rw-r--r--   0        0        0    12686 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/dict.h
--rw-r--r--   0        0        0     3552 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/dimensions.h
--rw-r--r--   0        0        0     5494 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/dtype.h
--rw-r--r--   0        0        0     1817 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/eigen.h
--rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/arg_list.h
--rw-r--r--   0        0        0     9240 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/arithmetic.h
--rw-r--r--   0        0        0     9270 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/bin.h
--rw-r--r--   0        0        0     2322 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/bin_detail.h
--rw-r--r--   0        0        0     5602 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/comparison.h
--rw-r--r--   0        0        0     2040 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/creation.h
--rw-r--r--   0        0        0     1099 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/cumulative.h
--rw-r--r--   0        0        0     7515 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/event_operations.h
--rw-r--r--   0        0        0     1415 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/geometric_operations.h
--rw-r--r--   0        0        0     3805 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/histogram.h
--rw-r--r--   0        0        0     1744 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/hyperbolic.h
--rw-r--r--   0        0        0     1749 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/logical.h
--rw-r--r--   0        0        0     5733 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/map_to_bins.h
--rw-r--r--   0        0        0     7145 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/math.h
--rw-r--r--   0        0        0     2706 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/rebin.h
--rw-r--r--   0        0        0      896 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/reduction.h
--rw-r--r--   0        0        0     1758 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/sort.h
--rw-r--r--   0        0        0     4628 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/special_values.h
--rw-r--r--   0        0        0     2108 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/to_unit.h
--rw-r--r--   0        0        0     2056 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/trigonometry.h
--rw-r--r--   0        0        0     5872 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element/util.h
--rw-r--r--   0        0        0     5467 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element_array.h
--rw-r--r--   0        0        0     5432 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/element_array_view.h
--rw-r--r--   0        0        0     4373 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/except.h
--rw-r--r--   0        0        0      466 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/flags.h
--rw-r--r--   0        0        0      576 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/has_eval.h
--rw-r--r--   0        0        0     1518 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/histogram.h
--rw-r--r--   0        0        0     2329 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/memory_pool.h
--rw-r--r--   0        0        0    11578 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/multi_index.h
--rw-r--r--   0        0        0     1007 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/parallel-fallback.h
--rw-r--r--   0        0        0     1288 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/parallel-tbb.h
--rw-r--r--   0        0        0     4024 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/sizes.h
--rw-r--r--   0        0        0     1287 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/slice.h
--rw-r--r--   0        0        0     5162 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/spatial_transforms.h
--rw-r--r--   0        0        0     2125 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/strides.h
--rw-r--r--   0        0        0     1880 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/string.h
--rw-r--r--   0        0        0     1827 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/subbin_sizes.h
--rw-r--r--   0        0        0     1157 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/tag_util.h
--rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/time_point.h
--rw-r--r--   0        0        0     4760 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/transform_common.h
--rw-r--r--   0        0        0    11054 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/value_and_variance.h
--rw-r--r--   0        0        0     3306 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/values_and_variances.h
--rw-r--r--   0        0        0     3839 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/include/scipp/core/view_index.h
--rw-r--r--   0        0        0     8626 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/multi_index.cpp
--rw-r--r--   0        0        0      914 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/rename.h
--rw-r--r--   0        0        0     6893 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/sizes.cpp
--rw-r--r--   0        0        0     1865 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/slice.cpp
--rw-r--r--   0        0        0     1420 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/strides.cpp
--rw-r--r--   0        0        0     5180 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/string.cpp
--rw-r--r--   0        0        0     3667 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/subbin_sizes.cpp
--rw-r--r--   0        0        0     1544 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/CMakeLists.txt
--rw-r--r--   0        0        0    29139 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/arithmetic_parameters.h
--rw-r--r--   0        0        0     3501 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/array_to_string_test.cpp
--rw-r--r--   0        0        0    17135 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/dict_test.cpp
--rw-r--r--   0        0        0     9648 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/dimensions_test.cpp
--rw-r--r--   0        0        0     2462 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/dtype_test.cpp
--rw-r--r--   0        0        0      808 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/eigen_test.cpp
--rw-r--r--   0        0        0     8633 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/element_arithmetic_test.cpp
--rw-r--r--   0        0        0     4525 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/element_array_test.cpp
--rw-r--r--   0        0        0    17688 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/element_array_view_test.cpp
--rw-r--r--   0        0        0     1838 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/element_bin_detail_test.cpp
--rw-r--r--   0        0        0     8174 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/element_comparison_test.cpp
--rw-r--r--   0        0        0     5551 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/element_event_operations_test.cpp
--rw-r--r--   0        0        0     1336 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/element_geometric_operations_test.cpp
--rw-r--r--   0        0        0     2767 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/element_histogram_test.cpp
--rw-r--r--   0        0        0     2494 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/element_hyperbolic_test.cpp
--rw-r--r--   0        0        0     2340 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/element_logical_test.cpp
--rw-r--r--   0        0        0     3068 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/element_map_to_bins_test.cpp
--rw-r--r--   0        0        0     7918 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/element_math_test.cpp
--rw-r--r--   0        0        0    13263 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/element_special_values_test.cpp
--rw-r--r--   0        0        0     3919 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/element_to_unit_test.cpp
--rw-r--r--   0        0        0     6999 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/element_trigonometry_test.cpp
--rw-r--r--   0        0        0     5296 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/element_util_test.cpp
--rw-r--r--   0        0        0     2365 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/generate_arithmetic_parameters.py
--rw-r--r--   0        0        0    19137 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/multi_index_test.cpp
--rw-r--r--   0        0        0     4297 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/sizes_test.cpp
--rw-r--r--   0        0        0     2090 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/slice_test.cpp
--rw-r--r--   0        0        0     2444 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/spatial_transforms_test.cpp
--rw-r--r--   0        0        0      487 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/strides_test.cpp
--rw-r--r--   0        0        0     1605 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/string_test.cpp
--rw-r--r--   0        0        0     4735 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/subbin_sizes_test.cpp
--rw-r--r--   0        0        0     1504 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/time_point_test.cpp
--rw-r--r--   0        0        0     1475 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/transform_common_test.cpp
--rw-r--r--   0        0        0    10385 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/value_and_variance_test.cpp
--rw-r--r--   0        0        0     4447 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/test/view_index_test.cpp
--rw-r--r--   0        0        0     1177 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/core/view_index.cpp
--rw-r--r--   0        0        0     2584 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/CMakeLists.txt
--rw-r--r--   0        0        0     8025 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/arithmetic.cpp
--rw-r--r--   0        0        0      702 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/astype.cpp
--rw-r--r--   0        0        0    29481 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/bin.cpp
--rw-r--r--   0        0        0      489 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/bin_common.h
--rw-r--r--   0        0        0     4820 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/bin_detail.cpp
--rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/bin_detail.h
--rw-r--r--   0        0        0    16739 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/bins.cpp
--rw-r--r--   0        0        0      999 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/bins_util.h
--rw-r--r--   0        0        0     3389 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/counts.cpp
--rw-r--r--   0        0        0     7397 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/data_array.cpp
--rw-r--r--   0        0        0    12992 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/dataset.cpp
--rw-r--r--   0        0        0     5851 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/dataset_operations_common.h
--rw-r--r--   0        0        0     3558 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/except.cpp
--rw-r--r--   0        0        0     5543 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/extract.cpp
--rw-r--r--   0        0        0    15263 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/groupby.cpp
--rw-r--r--   0        0        0     5612 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/histogram.cpp
--rw-r--r--   0        0        0      208 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/arithmetic.h
--rw-r--r--   0        0        0      413 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/astype.h
--rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/bin.h
--rw-r--r--   0        0        0     3446 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/bins.h
--rw-r--r--   0        0        0     4459 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/bins_view.h
--rw-r--r--   0        0        0     1420 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/counts.h
--rw-r--r--   0        0        0     4902 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/data_array.h
--rw-r--r--   0        0        0    12346 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/dataset.h
--rw-r--r--   0        0        0     2214 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/dataset_util.h
--rw-r--r--   0        0        0     2645 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/except.h
--rw-r--r--   0        0        0      750 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/extract.h
--rw-r--r--   0        0        0     3158 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/groupby.h
--rw-r--r--   0        0        0      850 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/histogram.h
--rw-r--r--   0        0        0      171 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/hyperbolic.h
--rw-r--r--   0        0        0      205 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/logical.h
--rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/math.h
--rw-r--r--   0        0        0      636 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/mean.h
--rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/nanmean.h
--rw-r--r--   0        0        0      671 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/rebin.h
--rw-r--r--   0        0        0     2090 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/shape.h
--rw-r--r--   0        0        0     8069 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/sized_dict.h
--rw-r--r--   0        0        0      822 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/sized_dict_forward.h
--rw-r--r--   0        0        0     1917 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/slice.h
--rw-r--r--   0        0        0     1027 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/sort.h
--rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/special_values.h
--rw-r--r--   0        0        0     1181 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/string.h
--rw-r--r--   0        0        0      473 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/to_unit.h
--rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/trigonometry.h
--rw-r--r--   0        0        0     1022 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/include/scipp/dataset/util.h
--rw-r--r--   0        0        0      986 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/mean.cpp
--rw-r--r--   0        0        0     1047 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/nanmean.cpp
--rw-r--r--   0        0        0     4897 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/operations.cpp
--rw-r--r--   0        0        0     1207 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/rebin.cpp
--rw-r--r--   0        0        0    12651 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/shape.cpp
--rw-r--r--   0        0        0    16768 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/sized_dict.cpp
--rw-r--r--   0        0        0     2604 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/slice.cpp
--rw-r--r--   0        0        0     3580 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/sort.cpp
--rw-r--r--   0        0        0     4645 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/string.cpp
--rw-r--r--   0        0        0     1720 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/CMakeLists.txt
--rw-r--r--   0        0        0     1636 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/astype_test.cpp
--rw-r--r--   0        0        0     5195 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/attributes_test.cpp
--rw-r--r--   0        0        0    34019 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/bin_test.cpp
--rw-r--r--   0        0        0     7673 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/binned_arithmetic_test.cpp
--rw-r--r--   0        0        0     2519 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/binned_creation_test.cpp
--rw-r--r--   0        0        0     9381 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/bins_reduction_test.cpp
--rw-r--r--   0        0        0    20826 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/bins_test.cpp
--rw-r--r--   0        0        0     3447 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/bins_view_test.cpp
--rw-r--r--   0        0        0    19172 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/concat_test.cpp
--rw-r--r--   0        0        0    14221 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/coords_view_test.cpp
--rw-r--r--   0        0        0     4445 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/copy_test.cpp
--rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/counts_test.cpp
--rw-r--r--   0        0        0     4829 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/data_array_arithmetic_test.cpp
--rw-r--r--   0        0        0    11093 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/data_array_comparison_test.cpp
--rw-r--r--   0        0        0    11989 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/data_array_test.cpp
--rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/data_view_test.cpp
--rw-r--r--   0        0        0    27585 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/dataset_arithmetic_test.cpp
--rw-r--r--   0        0        0     6879 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/dataset_comparison_test.cpp
--rw-r--r--   0        0        0     5606 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/dataset_operations_test.cpp
--rw-r--r--   0        0        0    30843 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/dataset_test.cpp
--rw-r--r--   0        0        0     4748 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/dataset_test_common.cpp
--rw-r--r--   0        0        0     3089 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/dataset_test_common.h
--rw-r--r--   0        0        0     3795 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/dataset_view_test.cpp
--rw-r--r--   0        0        0     3423 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/equals_nan_test.cpp
--rw-r--r--   0        0        0     3851 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/event_data_operations_consistency_test.cpp
--rw-r--r--   0        0        0     3234 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/except_test.cpp
--rw-r--r--   0        0        0     4592 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/generated_test.cpp
--rw-r--r--   0        0        0    33843 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/groupby_test.cpp
--rw-r--r--   0        0        0    20875 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/histogram_test.cpp
--rw-r--r--   0        0        0     3357 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/logical_reduction_test.cpp
--rw-r--r--   0        0        0     1850 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/masks_test.cpp
--rw-r--r--   0        0        0    10331 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/mean_test.cpp
--rw-r--r--   0        0        0     2756 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/merge_test.cpp
--rw-r--r--   0        0        0     5310 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/minmax_test.cpp
--rw-r--r--   0        0        0    11513 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/rebin_test.cpp
--rw-r--r--   0        0        0     2647 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/self_assignment_test.cpp
--rw-r--r--   0        0        0     8848 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/set_slice_test.cpp
--rw-r--r--   0        0        0    31449 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/shape_test.cpp
--rw-r--r--   0        0        0    16244 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/size_of_test.cpp
--rw-r--r--   0        0        0    13721 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/slice_by_value_test.cpp
--rw-r--r--   0        0        0    23135 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/slice_test.cpp
--rw-r--r--   0        0        0     8470 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/sort_test.cpp
--rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/string_test.cpp
--rw-r--r--   0        0        0    13030 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/sum_test.cpp
--rw-r--r--   0        0        0     1196 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/test_data_arrays.cpp
--rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/test_data_arrays.h
--rw-r--r--   0        0        0     4594 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/test/to_unit_test.cpp
--rw-r--r--   0        0        0      745 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/to_unit.cpp
--rw-r--r--   0        0        0     7730 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/util.cpp
--rw-r--r--   0        0        0     7492 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/variable_instantiate_bin_elements.cpp
--rw-r--r--   0        0        0      865 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/variable_instantiate_dataset.cpp
--rw-r--r--   0        0        0     3349 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/dataset/variable_reduction.cpp
--rw-r--r--   0        0        0        6 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/.gitignore
--rw-r--r--   0        0        0     1608 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/CMakeLists.txt
--rw-r--r--   0        0        0     1063 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/benchmark/variable.py
--rw-r--r--   0        0        0    21133 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/bind_data_access.h
--rw-r--r--   0        0        0    13077 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/bind_data_array.h
--rw-r--r--   0        0        0    15104 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/bind_operators.h
--rw-r--r--   0        0        0    13380 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/bind_slice_methods.h
--rw-r--r--   0        0        0     8029 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/bind_units.cpp
--rw-r--r--   0        0        0     7927 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/bins.cpp
--rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/comparison.cpp
--rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/counts.cpp
--rw-r--r--   0        0        0     1165 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/cumulative.cpp
--rw-r--r--   0        0        0    11119 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/dataset.cpp
--rw-r--r--   0        0        0      823 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/dim.h
--rw-r--r--   0        0        0     1843 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/docstring.cpp
--rw-r--r--   0        0        0     1713 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/docstring.h
--rw-r--r--   0        0        0    11316 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/dtype.cpp
--rw-r--r--   0        0        0     1759 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/dtype.h
--rw-r--r--   0        0        0     4530 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/element_array_view.cpp
--rw-r--r--   0        0        0     3123 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/except.cpp
--rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/format.h
--rw-r--r--   0        0        0      260 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/generated.cpp.in
--rw-r--r--   0        0        0     1008 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/geometry.cpp
--rw-r--r--   0        0        0     2894 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/groupby.cpp
--rw-r--r--   0        0        0     1182 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/histogram.cpp
--rw-r--r--   0        0        0     1255 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/numpy.cpp
--rw-r--r--   0        0        0    12432 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/numpy.h
--rw-r--r--   0        0        0     4093 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/operations.cpp
--rw-r--r--   0        0        0     1610 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/py_object.cpp
--rw-r--r--   0        0        0     1499 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/py_object.h
--rw-r--r--   0        0        0      736 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/pybind11.h
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/reduction.cpp
--rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/rename.h
--rw-r--r--   0        0        0     2572 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/scipp.cpp
--rw-r--r--   0        0        0     3519 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/shape.cpp
--rw-r--r--   0        0        0      785 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/slice_utils.cpp
--rw-r--r--   0        0        0      337 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/slice_utils.h
--rw-r--r--   0        0        0     1580 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/transform.cpp
--rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/trigonometry.cpp
--rw-r--r--   0        0        0     2787 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/unary.cpp
--rw-r--r--   0        0        0     4282 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/unit.cpp
--rw-r--r--   0        0        0     1615 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/unit.h
--rw-r--r--   0        0        0     4305 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/variable.cpp
--rw-r--r--   0        0        0     3076 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/variable_creation.cpp
--rw-r--r--   0        0        0    13092 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/variable_init.cpp
--rw-r--r--   0        0        0      507 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/variable_instantiate_py_object.cpp
--rw-r--r--   0        0        0     4042 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/python/view.h
--rw-r--r--   0        0        0      945 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/dataset_binary.cpp.in
--rw-r--r--   0        0        0      532 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/dataset_binary.h.in
--rw-r--r--   0        0        0      938 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/dataset_inplace.cpp.in
--rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/dataset_inplace.h.in
--rw-r--r--   0        0        0     1379 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/dataset_reduction.cpp.in
--rw-r--r--   0        0        0      561 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/dataset_reduction.h.in
--rw-r--r--   0        0        0      547 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/dataset_unary.cpp.in
--rw-r--r--   0        0        0      399 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/dataset_unary.h.in
--rw-r--r--   0        0        0      702 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/python_binary.cpp.in
--rw-r--r--   0        0        0      830 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/python_reduction.cpp.in
--rw-r--r--   0        0        0      917 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/python_unary.cpp.in
--rw-r--r--   0        0        0     1030 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/variable_binary.cpp.in
--rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/variable_binary.h.in
--rw-r--r--   0        0        0      759 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/variable_inplace.cpp.in
--rw-r--r--   0        0        0      446 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/variable_inplace.h.in
--rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/variable_unary.cpp.in
--rw-r--r--   0        0        0      497 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/templates/variable_unary.h.in
--rw-r--r--   0        0        0      218 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/test/CMakeLists.txt
--rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/test/fix_typed_test_suite_warnings.h
--rw-r--r--   0        0        0     1387 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/test/random.h
--rw-r--r--   0        0        0     3334 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/test/test_macros.h
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/test/test_nans.h
--rw-r--r--   0        0        0     1575 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/test/test_operations.h
--rw-r--r--   0        0        0      788 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/test/test_print_variable.h
--rw-r--r--   0        0        0      458 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/test/test_util.h
--rw-r--r--   0        0        0     1331 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/units/CMakeLists.txt
--rw-r--r--   0        0        0     2442 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/units/dim.cpp
--rw-r--r--   0        0        0      617 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/units/except.cpp
--rw-r--r--   0        0        0     2871 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/units/include/scipp/units/dim.h
--rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/units/include/scipp/units/except.h
--rw-r--r--   0        0        0      660 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/units/include/scipp/units/string.h
--rw-r--r--   0        0        0     4650 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/units/include/scipp/units/unit.h
--rw-r--r--   0        0        0      849 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/units/string.cpp
--rw-r--r--   0        0        0      663 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/units/test/CMakeLists.txt
--rw-r--r--   0        0        0     2458 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/units/test/dim_test.cpp
--rw-r--r--   0        0        0    11794 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/units/test/unit_test.cpp
--rw-r--r--   0        0        0     7297 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/units/unit.cpp
--rw-r--r--   0        0        0     3517 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/CMakeLists.txt
--rw-r--r--   0        0        0     4113 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/arithmetic.cpp
--rw-r--r--   0        0        0     2762 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/astype.cpp
--rw-r--r--   0        0        0     1225 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/bin_array_variable.cpp
--rw-r--r--   0        0        0     3392 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/bin_detail.cpp
--rw-r--r--   0        0        0      902 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/bin_util.cpp
--rw-r--r--   0        0        0     2968 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/bins.cpp
--rw-r--r--   0        0        0     2583 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/comparison.cpp
--rw-r--r--   0        0        0     3744 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/creation.cpp
--rw-r--r--   0        0        0     2085 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/cumulative.cpp
--rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/except.cpp
--rw-r--r--   0        0        0     7890 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/accumulate.h
--rw-r--r--   0        0        0     2393 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/arithmetic.h
--rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/astype.h
--rw-r--r--   0        0        0     5536 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/bin_array_model.h
--rw-r--r--   0        0        0    11591 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/bin_array_variable.tcc
--rw-r--r--   0        0        0     1200 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/bin_detail.h
--rw-r--r--   0        0        0      418 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/bin_util.h
--rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/bins.h
--rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/comparison.h
--rw-r--r--   0        0        0     1220 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/creation.h
--rw-r--r--   0        0        0      784 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/cumulative.h
--rw-r--r--   0        0        0     5542 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/element_array_model.h
--rw-r--r--   0        0        0     7218 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/element_array_variable.tcc
--rw-r--r--   0        0        0      831 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/except.h
--rw-r--r--   0        0        0      244 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/hyperbolic.h
--rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/inv.h
--rw-r--r--   0        0        0      206 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/logical.h
--rw-r--r--   0        0        0      452 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/math.h
--rw-r--r--   0        0        0      534 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/misc_operations.h
--rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/operations.h
--rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/pow.h
--rw-r--r--   0        0        0      587 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/rebin.h
--rw-r--r--   0        0        0     4065 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/reduction.h
--rw-r--r--   0        0        0     1681 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/shape.h
--rw-r--r--   0        0        0      628 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/slice.h
--rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/sort.h
--rw-r--r--   0        0        0     1195 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/special_values.h
--rw-r--r--   0        0        0     2498 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/string.h
--rw-r--r--   0        0        0     5128 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/structure_array_model.h
--rw-r--r--   0        0        0     3401 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/structure_array_variable.tcc
--rw-r--r--   0        0        0     1392 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/structures.h
--rw-r--r--   0        0        0      794 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/subspan_view.h
--rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/to_unit.h
--rw-r--r--   0        0        0    33404 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/transform.h
--rw-r--r--   0        0        0     4163 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/transform_subspan.h
--rw-r--r--   0        0        0      283 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/trigonometry.h
--rw-r--r--   0        0        0     1998 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/util.h
--rw-r--r--   0        0        0     8922 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/variable.h
--rw-r--r--   0        0        0     5827 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/variable.tcc
--rw-r--r--   0        0        0     2438 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/variable_concept.h
--rw-r--r--   0        0        0     5335 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/variable_factory.h
--rw-r--r--   0        0        0     3650 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/variable_keyword_arg_constructor.h
--rw-r--r--   0        0        0     4049 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/include/scipp/variable/visit.h
--rw-r--r--   0        0        0     1876 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/inv.cpp
--rw-r--r--   0        0        0     1245 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/math.cpp
--rw-r--r--   0        0        0     1230 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/operations.cpp
--rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/operations_common.h
--rw-r--r--   0        0        0     4257 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/pow.cpp
--rw-r--r--   0        0        0     7550 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/rebin.cpp
--rw-r--r--   0        0        0    10235 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/reduction.cpp
--rw-r--r--   0        0        0     5616 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/shape.cpp
--rw-r--r--   0        0        0     4893 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/slice.cpp
--rw-r--r--   0        0        0      774 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/sort.cpp
--rw-r--r--   0        0        0     1662 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/special_values.cpp
--rw-r--r--   0        0        0     4598 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/string.cpp
--rw-r--r--   0        0        0     3639 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/structures.cpp
--rw-r--r--   0        0        0     3840 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/subspan_view.cpp
--rw-r--r--   0        0        0     1681 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/CMakeLists.txt
--rw-r--r--   0        0        0     6920 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/accumulate_test.cpp
--rw-r--r--   0        0        0     4457 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/arithmetic_test.cpp
--rw-r--r--   0        0        0     4364 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/astype_test.cpp
--rw-r--r--   0        0        0     5879 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/bin_array_model_test.cpp
--rw-r--r--   0        0        0     1044 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/bin_util_test.cpp
--rw-r--r--   0        0        0    13678 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/comparison_test.cpp
--rw-r--r--   0        0        0     4680 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/concat_test.cpp
--rw-r--r--   0        0        0     2842 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/copy_test.cpp
--rw-r--r--   0        0        0     7013 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/creation_test.cpp
--rw-r--r--   0        0        0     2749 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/cumulative_test.cpp
--rw-r--r--   0        0        0     1620 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/equals_nan_test.cpp
--rw-r--r--   0        0        0     1827 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/hyperbolic_test.cpp
--rw-r--r--   0        0        0     2696 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/inv_test.cpp
--rw-r--r--   0        0        0     2028 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/linalg_test.cpp
--rw-r--r--   0        0        0    20416 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/math_test.cpp
--rw-r--r--   0        0        0     6402 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/mean_test.cpp
--rw-r--r--   0        0        0    36450 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/operations_test.cpp
--rw-r--r--   0        0        0    14117 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/rebin_test.cpp
--rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/reduce_logical_test.cpp
--rw-r--r--   0        0        0     6591 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/reduce_various_test.cpp
--rw-r--r--   0        0        0    12521 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/shape_test.cpp
--rw-r--r--   0        0        0     2528 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/slice_test.cpp
--rw-r--r--   0        0        0     1538 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/sort_test.cpp
--rw-r--r--   0        0        0     9531 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/special_values_test.cpp
--rw-r--r--   0        0        0     6371 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/subspan_view_test.cpp
--rw-r--r--   0        0        0     2691 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/sum_test.cpp
--rw-r--r--   0        0        0     2319 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/test_variables.cpp
--rw-r--r--   0        0        0      371 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/test_variables.h
--rw-r--r--   0        0        0    11990 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/to_unit_test.cpp
--rw-r--r--   0        0        0    25693 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/transform_binary_test.cpp
--rw-r--r--   0        0        0    20584 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/transform_test.cpp
--rw-r--r--   0        0        0     6304 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/transform_test_helpers.cpp
--rw-r--r--   0        0        0     2895 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/transform_test_helpers.h
--rw-r--r--   0        0        0    11461 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/transform_unary_test.cpp
--rw-r--r--   0        0        0     6676 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/trigonometry_test.cpp
--rw-r--r--   0        0        0     6417 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/util_test.cpp
--rw-r--r--   0        0        0    10945 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/variable_bin_test.cpp
--rw-r--r--   0        0        0     8872 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/variable_comparison_test.cpp
--rw-r--r--   0        0        0     1168 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/variable_custom_type_test.cpp
--rw-r--r--   0        0        0     7124 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/variable_keyword_args_constructor_test.cpp
--rw-r--r--   0        0        0     3486 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/variable_scalar_accessors_test.cpp
--rw-r--r--   0        0        0     3806 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/variable_structure_test.cpp
--rw-r--r--   0        0        0    42123 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/test/variable_test.cpp
--rw-r--r--   0        0        0     2839 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/to_unit.cpp
--rw-r--r--   0        0        0     4829 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/util.cpp
--rw-r--r--   0        0        0    11003 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/variable.cpp
--rw-r--r--   0        0        0      218 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/variable_concept.cpp
--rw-r--r--   0        0        0     3483 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/variable_factory.cpp
--rw-r--r--   0        0        0     1010 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/variable_instantiate_basic.cpp
--rw-r--r--   0        0        0     2677 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/variable_instantiate_bin_elements.cpp
--rw-r--r--   0        0        0     3851 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/variable_instantiate_linalg.cpp
--rw-r--r--   0        0        0     2426 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/variable_instantiate_map_elements.cpp
--rw-r--r--   0        0        0     1980 2022-11-09 12:37:21.000000 scipp-24.2.0/lib/variable/variable_instantiate_view_elements.cpp
--rw-r--r--   0        0        0     3987 2022-11-09 12:37:21.000000 scipp-24.2.0/pyproject.toml
--rw-r--r--   0        0        0       27 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/asv.in
--rw-r--r--   0        0        0      348 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/asv.txt
--rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/base.in
--rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/base.txt
--rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/build.in
--rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/build.txt
--rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/ci.in
--rw-r--r--   0        0        0      936 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/ci.txt
--rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/coverage.in
--rw-r--r--   0        0        0      243 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/coverage.txt
--rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/docs.in
--rw-r--r--   0        0        0     3450 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/docs.txt
--rw-r--r--   0        0        0       74 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/extra.in
--rw-r--r--   0        0        0     2134 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/extra.txt
--rw-r--r--   0        0        0       11 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/static.in
--rw-r--r--   0        0        0      575 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/static.txt
--rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/test.in
--rw-r--r--   0        0        0      664 2022-11-09 12:37:21.000000 scipp-24.2.0/requirements/test.txt
--rw-r--r--   0        0        0   643740 2022-11-09 12:37:21.000000 scipp-24.2.0/resources/logo-2019-09-07.svg
--rw-r--r--   0        0        0   107538 2022-11-09 12:37:21.000000 scipp-24.2.0/resources/logo-2021.svg
--rw-r--r--   0        0        0    69135 2022-11-09 12:37:21.000000 scipp-24.2.0/resources/logo-2022.svg
--rw-r--r--   0        0        0      226 2022-11-09 12:37:21.000000 scipp-24.2.0/setup.cfg
--rw-r--r--   0        0        0     8510 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/__init__.py
--rw-r--r--   0        0        0     3496 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/_binding.py
--rw-r--r--   0        0        0      557 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/_extend_units.py
--rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/_scipp.pyi
--rw-r--r--   0        0        0      475 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/binning/__init__.py
--rw-r--r--   0        0        0      358 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/compat/__init__.py
--rw-r--r--   0        0        0     6008 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/compat/dict.py
--rw-r--r--   0        0        0     6957 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/compat/pandas_compat.py
--rw-r--r--   0        0        0     3971 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/compat/wrapping.py
--rw-r--r--   0        0        0     5713 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/compat/xarray_compat.py
--rw-r--r--   0        0        0     4941 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/constants/__init__.py
--rw-r--r--   0        0        0      255 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/coords/__init__.py
--rw-r--r--   0        0        0      863 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/coords/coord.py
--rw-r--r--   0        0        0     2573 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/coords/coord_table.py
--rw-r--r--   0        0        0     5213 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/coords/graph.py
--rw-r--r--   0        0        0      378 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/coords/options.py
--rw-r--r--   0        0        0     7452 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/coords/rule.py
--rw-r--r--   0        0        0    12288 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/coords/transform_coords.py
--rw-r--r--   0        0        0     7091 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/__init__.py
--rw-r--r--   0        0        0      623 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/_cpp_wrapper_util.py
--rw-r--r--   0        0        0      727 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/_sizes.py
--rw-r--r--   0        0        0      701 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/argument_handlers.py
--rw-r--r--   0        0        0     5742 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/arithmetic.py
--rw-r--r--   0        0        0     2072 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/assignments.py
--rw-r--r--   0        0        0     6809 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/bin_remapping.py
--rw-r--r--   0        0        0    26751 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/binning.py
--rw-r--r--   0        0        0    19709 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/bins.py
--rw-r--r--   0        0        0     8807 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/comparison.py
--rw-r--r--   0        0        0     3125 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/concepts.py
--rw-r--r--   0        0        0     1092 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/counts.py
--rw-r--r--   0        0        0      479 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/cpp_classes.py
--rw-r--r--   0        0        0    43849 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/cpp_classes.pyi
--rw-r--r--   0        0        0     1362 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/cumulative.py
--rw-r--r--   0        0        0    21746 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/data_group.py
--rw-r--r--   0        0        0      858 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/dataset.py
--rw-r--r--   0        0        0     1348 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/deprecation.py
--rw-r--r--   0        0        0     5237 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/dimensions.py
--rw-r--r--   0        0        0     1093 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/domains.py
--rw-r--r--   0        0        0      892 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/groupby.py
--rw-r--r--   0        0        0     3156 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/hyperbolic.py
--rw-r--r--   0        0        0     5258 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/like.py
--rw-r--r--   0        0        0     1740 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/logical.py
--rw-r--r--   0        0        0     9715 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/math.py
--rw-r--r--   0        0        0    10196 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/operations.py
--rw-r--r--   0        0        0    28660 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/reduction.py
--rw-r--r--   0        0        0    14212 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/shape.py
--rw-r--r--   0        0        0     1462 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/structured.py
--rw-r--r--   0        0        0     3782 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/trigonometry.py
--rw-r--r--   0        0        0     2064 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/unary.py
--rw-r--r--   0        0        0     1688 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/util.py
--rw-r--r--   0        0        0    29376 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/core/variable.py
--rw-r--r--   0        0        0    18462 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/curve_fit.py
--rw-r--r--   0        0        0     3208 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/data/__init__.py
--rw-r--r--   0        0        0       86 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/format/__init__.py
--rw-r--r--   0        0        0     2151 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/format/_parse.py
--rw-r--r--   0        0        0     7534 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/format/formatter.py
--rw-r--r--   0        0        0     1963 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/geometry.py
--rw-r--r--   0        0        0      629 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/io/__init__.py
--rw-r--r--   0        0        0     4834 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/io/csv.py
--rw-r--r--   0        0        0    14718 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/io/hdf5.py
--rw-r--r--   0        0        0     8064 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/logging.py
--rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/object_list.py
--rw-r--r--   0        0        0     2718 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/operations.py
--rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/plotting.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/py.typed
--rw-r--r--   0        0        0     3139 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/reduction.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/scipy/__init__.py
--rw-r--r--   0        0        0     2261 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/scipy/integrate/__init__.py
--rw-r--r--   0        0        0     7498 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/scipy/interpolate/__init__.py
--rw-r--r--   0        0        0    10453 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/scipy/ndimage/__init__.py
--rw-r--r--   0        0        0     9025 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/scipy/optimize/__init__.py
--rw-r--r--   0        0        0     5097 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/scipy/signal/__init__.py
--rw-r--r--   0        0        0     1170 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/serialization.py
--rw-r--r--   0        0        0    12031 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/spatial/__init__.py
--rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/sphinxext/__init__.py
--rw-r--r--   0        0        0     4183 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/sphinxext/autoplot.py
--rw-r--r--   0        0        0      330 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/testing/__init__.py
--rw-r--r--   0        0        0     8202 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/testing/assertions.py
--rw-r--r--   0        0        0    10050 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/testing/strategies.py
--rw-r--r--   0        0        0     2877 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/typing.py
--rw-r--r--   0        0        0     6561 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/units/__init__.py
--rw-r--r--   0        0        0      289 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/utils/__init__.py
--rw-r--r--   0        0        0     3906 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/utils/collapse_and_slices.py
--rw-r--r--   0        0        0     2638 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/utils/comparison.py
--rw-r--r--   0        0        0      507 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/utils/graph.py
--rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/utils/profile.py
--rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/utils/pyshell.py
--rw-r--r--   0        0        0     1315 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/utils/to_string.py
--rw-r--r--   0        0        0      276 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/visualization/__init__.py
--rw-r--r--   0        0        0     1322 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/visualization/colors.py
--rw-r--r--   0        0        0     5621 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/visualization/formatting_datagroup_html.py
--rw-r--r--   0        0        0    16215 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/visualization/formatting_html.py
--rw-r--r--   0        0        0     1484 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/visualization/html.py
--rw-r--r--   0        0        0     2634 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/visualization/resources.py
--rw-r--r--   0        0        0    19531 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/visualization/show.py
--rw-r--r--   0        0        0     7304 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/visualization/table.py
--rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/visualization/templates/__init__.py
--rw-r--r--   0        0        0     3267 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/visualization/templates/datagroup.css
--rw-r--r--   0        0        0      831 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/visualization/templates/dg_atomic_row.html
--rw-r--r--   0        0        0     1238 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/visualization/templates/dg_collapsible_row.html
--rw-r--r--   0        0        0      711 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/visualization/templates/dg_detail_list.html
--rw-r--r--   0        0        0      888 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/visualization/templates/dg_repr.html
--rw-r--r--   0        0        0     1574 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/visualization/templates/icons-svg-inline.html
--rw-r--r--   0        0        0     8904 2022-11-09 12:37:21.000000 scipp-24.2.0/src/scipp/visualization/templates/style.css
--rw-r--r--   0        0        0    38090 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/binning_test.py
--rw-r--r--   0        0        0    22256 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/bins_test.py
--rw-r--r--   0        0        0      520 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/common_test.py
--rw-r--r--   0        0        0    11635 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/compat/dict_test.py
--rw-r--r--   0        0        0    10818 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/compat/pandas_compat_test.py
--rw-r--r--   0        0        0     3317 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/compat/wrapping_test.py
--rw-r--r--   0        0        0    12129 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/compat/xarray_compat_test.py
--rw-r--r--   0        0        0     3397 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/concepts_test.py
--rw-r--r--   0        0        0      621 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1051 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/constants/constants_test.py
--rw-r--r--   0        0        0     5531 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/coords/graph_test.py
--rw-r--r--   0        0        0    33516 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/coords/transform_coords_test.py
--rw-r--r--   0        0        0    11791 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/core/arithmetic_test.py
--rw-r--r--   0        0        0     9864 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/core/comparison_test.py
--rw-r--r--   0        0        0     3700 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/core/logical_test.py
--rw-r--r--   0        0        0     5185 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/core/math_test.py
--rw-r--r--   0        0        0    32253 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/core/reduction_test.py
--rw-r--r--   0        0        0      823 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/counts_test.py
--rw-r--r--   0        0        0      692 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/cumulative_test.py
--rw-r--r--   0        0        0    16498 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/curve_fit_test.py
--rw-r--r--   0        0        0    22469 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/data_array_test.py
--rw-r--r--   0        0        0    29026 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/data_group_test.py
--rw-r--r--   0        0        0    22932 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/dataset_test.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/datasetslice_test.py
--rw-r--r--   0        0        0     9834 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/datetime_test.py
--rw-r--r--   0        0        0    15850 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/dicts_test.py
--rw-r--r--   0        0        0     5168 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/domains_test.py
--rw-r--r--   0        0        0     2870 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/dtype_test.py
--rw-r--r--   0        0        0     2375 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/dynamic_binding_test.py
--rw-r--r--   0        0        0     2326 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/elemwise_func_test.py
--rw-r--r--   0        0        0     6815 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/format/format_test.py
--rw-r--r--   0        0        0     4424 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/html/html_repr_test.py
--rw-r--r--   0        0        0     2813 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/hypothesis/bin_test.py
--rw-r--r--   0        0        0      799 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/hypothesis/histogram_test.py
--rw-r--r--   0        0        0     1401 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/hypothesis/lookup_test.py
--rw-r--r--   0        0        0     6183 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/hypothesis/strategies_test.py
--rw-r--r--   0        0        0     2571 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/hypothesis/to_unit_test.py
--rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/io/csv_test.py
--rw-r--r--   0        0        0    11020 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/io/hdf5_test.py
--rw-r--r--   0        0        0     2153 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/iteration_test.py
--rw-r--r--   0        0        0     5562 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/lifetime_test.py
--rw-r--r--   0        0        0     4885 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/linalg_test.py
--rw-r--r--   0        0        0     7981 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/lookup_test.py
--rw-r--r--   0        0        0     3437 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/numpy_test.py
--rw-r--r--   0        0        0    12993 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/ownership_dataset_test.py
--rw-r--r--   0        0        0    18450 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/ownership_variable_test.py
--rw-r--r--   0        0        0     1032 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/python_scalar_operations_test.py
--rw-r--r--   0        0        0     5952 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/readonly_test.py
--rw-r--r--   0        0        0     1522 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/reduce_test.py
--rw-r--r--   0        0        0     4440 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/rename_test.py
--rw-r--r--   0        0        0     2481 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/repr_test.py
--rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/scipp_test.py
--rw-r--r--   0        0        0     2354 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/scipy/integrate_test.py
--rw-r--r--   0        0        0     5900 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/scipy/interpolate/interp1d_test.py
--rw-r--r--   0        0        0     7065 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/scipy/ndimage/footprint_filter_test.py
--rw-r--r--   0        0        0     5238 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/scipy/ndimage/gaussian_filter_test.py
--rw-r--r--   0        0        0    10274 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/scipy/optimize/curve_fit_test.py
--rw-r--r--   0        0        0     1383 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/scipy/signal/butter_test.py
--rw-r--r--   0        0        0     5855 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/scipy/signal/sosfiltfilt_test.py
--rw-r--r--   0        0        0      604 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/serialization_test.py
--rw-r--r--   0        0        0     1619 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/setitem_test.py
--rw-r--r--   0        0        0     4927 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/shape_test.py
--rw-r--r--   0        0        0     1083 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/show_test.py
--rw-r--r--   0        0        0     4682 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/slice_bins_test.py
--rw-r--r--   0        0        0     5732 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/slice_by_condition_test.py
--rw-r--r--   0        0        0     3637 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/slice_by_index_list_test.py
--rw-r--r--   0        0        0     4715 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/slice_test.py
--rw-r--r--   0        0        0     9288 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/slicebyvalue_test.py
--rw-r--r--   0        0        0     2584 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/spatial/affine_test.py
--rw-r--r--   0        0        0     6782 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/spatial/linear_transform_test.py
--rw-r--r--   0        0        0     3508 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/spatial/rotation_test.py
--rw-r--r--   0        0        0      999 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/spatial/scaling_test.py
--rw-r--r--   0        0        0     1694 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/spatial/translation_test.py
--rw-r--r--   0        0        0     1834 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/spatial/vector_test.py
--rw-r--r--   0        0        0     1223 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/structured_test.py
--rw-r--r--   0        0        0    21595 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/testing/assertions_test.py
--rw-r--r--   0        0        0     2381 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/to_unit_test.py
--rw-r--r--   0        0        0     9478 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/unit_test.py
--rw-r--r--   0        0        0     2396 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/utils/collapse_and_slices_test.py
--rw-r--r--   0        0        0     3697 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/utils/comparison_test.py
--rw-r--r--   0        0        0     1698 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/utils/to_string_test.py
--rw-r--r--   0        0        0    35241 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/variable_creation_test.py
--rw-r--r--   0        0        0    16486 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/variable_init_test.py
--rw-r--r--   0        0        0     1843 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/variable_py_object_test.py
--rw-r--r--   0        0        0     3115 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/variable_reduction_test.py
--rw-r--r--   0        0        0     3678 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/variable_scalar_test.py
--rw-r--r--   0        0        0    22894 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/variable_test.py
--rw-r--r--   0        0        0     2701 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/variable_view_test.py
--rw-r--r--   0        0        0     4462 2022-11-09 12:37:21.000000 scipp-24.2.0/tests/variance_broadcast_test.py
--rw-r--r--   0        0        0      510 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/README.md
--rw-r--r--   0        0        0     6101 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/benchmark_build.py
--rw-r--r--   0        0        0      772 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/debug/debug_multi_index_fragment.h
--rw-r--r--   0        0        0      854 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/debug/debugout.h
--rw-r--r--   0        0        0     9399 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/metatoenv.py
--rw-r--r--   0        0        0      252 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/migration/README.md
--rw-r--r--   0        0        0     1160 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/migration/scipp-0.11-hdf5-files.py
--rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/migration/scipp-0.12-hdf5-files.py
--rw-r--r--   0        0        0     2206 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/migration/scipp-0.13-hdf5-files.py
--rw-r--r--   0        0        0     6846 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/plot_benchmarks.py
--rwxr-xr-x   0        0        0      139 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/run-tests.sh.in
--rwxr-xr-x   0        0        0       67 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/run_asan.sh
--rwxr-xr-x   0        0        0     1145 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/run_sanitizer.sh
--rwxr-xr-x   0        0        0       69 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/run_ubsan.sh
--rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/scipp-coverage-index.html
--rw-r--r--   0        0        0     1744 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/stubgen/README.md
--rw-r--r--   0        0        0     4237 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/stubgen/__init__.py
--rw-r--r--   0        0        0      556 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/stubgen/__main__.py
--rw-r--r--   0        0        0     2236 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/stubgen/config.py
--rw-r--r--   0        0        0     5395 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/stubgen/parse.py
--rw-r--r--   0        0        0      390 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/stubgen/stub_template.py.template
--rw-r--r--   0        0        0     7684 2022-11-09 12:37:21.000000 scipp-24.2.0/tools/stubgen/transformer.py
--rw-r--r--   0        0        0     4207 2022-11-09 12:37:21.000000 scipp-24.2.0/tox.ini
--rw-r--r--   0        0        0     5774 2022-11-09 12:37:21.000000 scipp-24.2.0/PKG-INFO
+-rw-r--r--   0        0        0      462 2022-11-09 12:37:21.000000 scipp-24.5.0/.buildconfig/ci-linux.yml
+-rw-r--r--   0        0        0      383 2022-11-09 12:37:21.000000 scipp-24.5.0/.buildconfig/ci-macos.yml
+-rw-r--r--   0        0        0      385 2022-11-09 12:37:21.000000 scipp-24.5.0/.buildconfig/ci-windows.yml
+-rw-r--r--   0        0        0       59 2022-11-09 12:37:21.000000 scipp-24.5.0/.clang-format
+-rw-r--r--   0        0        0     6160 2022-11-09 12:37:21.000000 scipp-24.5.0/.clang-tidy
+-rw-r--r--   0        0        0      574 2022-11-09 12:37:21.000000 scipp-24.5.0/.cmake-format.json
+-rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 scipp-24.5.0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      454 2022-11-09 12:37:21.000000 scipp-24.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1598 2022-11-09 12:37:21.000000 scipp-24.5.0/.github/workflows/conda.yml
+-rw-r--r--   0        0        0     2104 2022-11-09 12:37:21.000000 scipp-24.5.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     2142 2022-11-09 12:37:21.000000 scipp-24.5.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     2957 2022-11-09 12:37:21.000000 scipp-24.5.0/.github/workflows/pr_and_main.yml
+-rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 scipp-24.5.0/.github/workflows/release-nightly.yml
+-rw-r--r--   0        0        0     5110 2022-11-09 12:37:21.000000 scipp-24.5.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      403 2022-11-09 12:37:21.000000 scipp-24.5.0/.github/workflows/rename-dev-wheels.py
+-rw-r--r--   0        0        0      792 2022-11-09 12:37:21.000000 scipp-24.5.0/.github/workflows/weekly.yml
+-rw-r--r--   0        0        0      951 2022-11-09 12:37:21.000000 scipp-24.5.0/.github/workflows/wheel.yml
+-rw-r--r--   0        0        0      623 2022-11-09 12:37:21.000000 scipp-24.5.0/.gitignore
+-rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 scipp-24.5.0/.gitmodules
+-rw-r--r--   0        0        0     1675 2022-11-09 12:37:21.000000 scipp-24.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 scipp-24.5.0/.vscode/settings.json
+-rw-r--r--   0        0        0     3083 2022-11-09 12:37:21.000000 scipp-24.5.0/CMakeLists.txt
+-rw-r--r--   0        0        0     3965 2022-11-09 12:37:21.000000 scipp-24.5.0/CMakePresets.json
+-rw-r--r--   0        0        0     5479 2022-11-09 12:37:21.000000 scipp-24.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 scipp-24.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1553 2022-11-09 12:37:21.000000 scipp-24.5.0/LICENSE
+-rw-r--r--   0        0        0      112 2022-11-09 12:37:21.000000 scipp-24.5.0/MANIFEST.in
+-rw-r--r--   0        0        0     1842 2022-11-09 12:37:21.000000 scipp-24.5.0/README.md
+-rw-r--r--   0        0        0     1453 2022-11-09 12:37:21.000000 scipp-24.5.0/asv.conf.json
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 scipp-24.5.0/benchmarks/__init__.py
+-rw-r--r--   0        0        0     2902 2022-11-09 12:37:21.000000 scipp-24.5.0/benchmarks/bin.py
+-rw-r--r--   0        0        0     3730 2022-11-09 12:37:21.000000 scipp-24.5.0/benchmarks/binned.py
+-rw-r--r--   0        0        0      650 2022-11-09 12:37:21.000000 scipp-24.5.0/benchmarks/variable.py
+-rw-r--r--   0        0        0      639 2022-11-09 12:37:21.000000 scipp-24.5.0/cmake/docs.cmake
+-rw-r--r--   0        0        0     1162 2022-11-09 12:37:21.000000 scipp-24.5.0/conda/README.md
+-rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 scipp-24.5.0/conda/cmake-package-test/CMakeLists.txt
+-rw-r--r--   0        0        0      223 2022-11-09 12:37:21.000000 scipp-24.5.0/conda/cmake-package-test/README.md
+-rw-r--r--   0        0        0     1094 2022-11-09 12:37:21.000000 scipp-24.5.0/conda/cmake-package-test/build.py
+-rw-r--r--   0        0        0       80 2022-11-09 12:37:21.000000 scipp-24.5.0/conda/cmake-package-test/main.cpp
+-rw-r--r--   0        0        0     2786 2022-11-09 12:37:21.000000 scipp-24.5.0/conda/meta.yaml
+-rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 scipp-24.5.0/conda/variants/linux_64.yaml
+-rw-r--r--   0        0        0       71 2022-11-09 12:37:21.000000 scipp-24.5.0/conda/variants/osx_64.yaml
+-rw-r--r--   0        0        0       74 2022-11-09 12:37:21.000000 scipp-24.5.0/conda/variants/osx_arm64.yaml
+-rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 scipp-24.5.0/conda/variants/win_64.yaml
+-rw-r--r--   0        0        0     1409 2022-11-09 12:37:21.000000 scipp-24.5.0/cppcheck-suppressions.txt
+-rw-r--r--   0        0        0       96 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/.gitignore
+-rw-r--r--   0        0        0     4458 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/_static/anaconda-icon.js
+-rw-r--r--   0        0        0   137750 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/_static/favicon.ico
+-rw-r--r--   0        0        0    12917 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/_static/logo-2022.svg
+-rw-r--r--   0        0        0    13113 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/_static/logo-dark.svg
+-rw-r--r--   0        0        0   152456 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/_static/title-filtering-1d-plot.svg
+-rw-r--r--   0        0        0    59695 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/_static/title-repr-html.png
+-rw-r--r--   0        0        0    90813 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/_static/title-show-svg.png
+-rw-r--r--   0        0        0      176 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/_templates/doc_version.html
+-rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/_templates/scipp-class-template.rst
+-rw-r--r--   0        0        0     1217 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/_templates/scipp-module-template.rst
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/_templates/scipp-sphinxext-template.rst
+-rw-r--r--   0        0        0      112 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/_templates/scipp-type-template.rst
+-rw-r--r--   0        0        0     3079 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/about/about.rst
+-rw-r--r--   0        0        0     2145 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/about/contributing.rst
+-rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/about/index.rst
+-rw-r--r--   0        0        0     5355 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/about/migration/23-01.ipynb
+-rw-r--r--   0        0        0       88 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/about/migration-notes.rst
+-rw-r--r--   0        0        0    66489 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/about/release-notes.rst
+-rw-r--r--   0        0        0     1490 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/about/roadmap.rst
+-rw-r--r--   0        0        0     8655 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/conf.py
+-rw-r--r--   0        0        0     2336 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0001-remove-dataset-masking-support.rst
+-rw-r--r--   0        0        0     1353 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0002-remove-instrument-view-projection-options.rst
+-rw-r--r--   0        0        0     3017 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0003-refactor-plotting-code-with-mvc-pattern.rst
+-rw-r--r--   0        0        0      975 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0004-use-ipympl-backend-for-matplotlib.rst
+-rw-r--r--   0        0        0     1618 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0005-remove-need-for-bins-property-when-calling-bin-or-histogram.rst
+-rw-r--r--   0        0        0     3389 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0006-add-readonly-flags.rst
+-rw-r--r--   0        0        0     1900 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0007-do-not-support-args-referencing-x-or-y.rst
+-rw-r--r--   0        0        0     2534 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0008-consistent-multi-dimensional-coords.rst
+-rw-r--r--   0        0        0     1570 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0009-handle-dimensionless-as-non-counts.rst
+-rw-r--r--   0        0        0     2327 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0010-acknowledge-stability-and-maintainability-tasks.rst
+-rw-r--r--   0        0        0     9772 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0011-renaming-of-dimensions-in-transform_coords.rst
+-rw-r--r--   0        0        0     3847 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0012-rebin-should-apply-irreducible-masks.rst
+-rw-r--r--   0        0        0     4061 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0013-plot-should-not-resample-automatically.rst
+-rw-r--r--   0        0        0     4264 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0014-switch-calendar-versioning.rst
+-rw-r--r--   0        0        0     1737 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0015-disable-support-for-broadcasting-variances.rst
+-rw-r--r--   0        0        0     6585 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0016-do-not-support-attrs.rst
+-rw-r--r--   0        0        0     6379 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/adr/0017-restrict-dataset-to-items-with-matching-dimensionality.rst
+-rw-r--r--   0        0        0      110 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/architecture-decision-records.rst
+-rw-r--r--   0        0        0     5368 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/coding-conventions.rst
+-rw-r--r--   0        0        0     4300 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/dependencies.rst
+-rw-r--r--   0        0        0     8687 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/getting-started.rst
+-rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/index.rst
+-rw-r--r--   0        0        0     8296 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/internals/concepts.ipynb
+-rw-r--r--   0        0        0     2358 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/internals/constructing_variables.rst
+-rw-r--r--   0        0        0     1499 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/internals/customizing.rst
+-rw-r--r--   0        0        0      173 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/internals/index.rst
+-rw-r--r--   0        0        0     8157 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/internals/multi_dimensional_indexing.rst
+-rw-r--r--   0        0        0     5063 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/internals/transform.rst
+-rw-r--r--   0        0        0     3723 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/internals/variable_implementation.rst
+-rw-r--r--   0        0        0     4213 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/notebook-style-guide.ipynb
+-rw-r--r--   0        0        0    16406 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/project/scipp-as-cpp-or-python-library.md
+-rw-r--r--   0        0        0     2924 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/releasing-scipp.rst
+-rw-r--r--   0        0        0     1685 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/development/tooling.rst
+-rw-r--r--   0        0        0      576 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/environments/developer.yml
+-rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/environments/scipp.yml
+-rw-r--r--   0        0        0     5905 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/getting-started/faq.rst
+-rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/getting-started/index.rst
+-rw-r--r--   0        0        0     3286 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/getting-started/installation.rst
+-rw-r--r--   0        0        0     8109 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/getting-started/overview.rst
+-rw-r--r--   0        0        0     5073 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/getting-started/quick-start.ipynb
+-rw-r--r--   0        0        0        5 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/getting-started/tutorials/.gitignore
+-rw-r--r--   0        0        0    22825 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/getting-started/tutorials/from-tabular-data-to-binned-data.ipynb
+-rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/getting-started/tutorials/index.rst
+-rw-r--r--   0        0        0     8802 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/getting-started/tutorials/prepare_data_rhessi.py
+-rw-r--r--   0        0        0    38291 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/getting-started/tutorials/solar_flares.ipynb
+-rw-r--r--   0        0        0    37305 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/multi_dimensional_indexing/multi_index_binned_1d_setups.svg
+-rw-r--r--   0        0        0    27965 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/multi_dimensional_indexing/multi_index_binned_2d_setups.svg
+-rw-r--r--   0        0        0    30700 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/multi_dimensional_indexing/multi_index_dense_setups.svg
+-rw-r--r--   0        0        0   122317 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/multi_dimensional_indexing/view_index_delta.svg
+-rw-r--r--   0        0        0    34041 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/multi_dimensional_indexing/view_index_flattening.svg
+-rw-r--r--   0        0        0    46617 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/multi_dimensional_indexing/view_index_increment_full.svg
+-rw-r--r--   0        0        0    37002 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/multi_dimensional_indexing/view_index_increment_partial.svg
+-rw-r--r--   0        0        0    71142 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/plotting-1d-keep-event.png
+-rw-r--r--   0        0        0    81853 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/plotting-1d-pick-event.png
+-rw-r--r--   0        0        0    85238 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/plotting-1d-slider-event.png
+-rw-r--r--   0        0        0    78661 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/plotting-2d-slider-event.png
+-rw-r--r--   0        0        0    60702 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/transform_coords/base_rules.svg
+-rw-r--r--   0        0        0   127544 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/transform_coords/cycle-contraction.svg
+-rw-r--r--   0        0        0    49251 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/transform_coords/cycle.svg
+-rw-r--r--   0        0        0    56259 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/transform_coords/cycle_rules.svg
+-rw-r--r--   0        0        0   137381 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/transform_coords/fractional-colors.svg
+-rw-r--r--   0        0        0    83957 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/transform_coords/larger_examples.svg
+-rw-r--r--   0        0        0    43658 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/transform_coords/slice-transform-concat.svg
+-rw-r--r--   0        0        0    55508 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/transform_coords/split-join.svg
+-rw-r--r--   0        0        0    66888 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/variable_classes.dia
+-rw-r--r--   0        0        0    13207 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/images/variable_classes.svg
+-rw-r--r--   0        0        0     5305 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/index.rst
+-rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/reference/classes.rst
+-rw-r--r--   0        0        0      337 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/reference/creation-functions.rst
+-rw-r--r--   0        0        0     8279 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/reference/dtype.ipynb
+-rw-r--r--   0        0        0     2875 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/reference/error-propagation.rst
+-rw-r--r--   0        0        0     2737 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/reference/free-functions.rst
+-rw-r--r--   0        0        0      242 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/reference/index.rst
+-rw-r--r--   0        0        0     9553 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/reference/linear-algebra.ipynb
+-rw-r--r--   0        0        0     6626 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/reference/logging.ipynb
+-rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/reference/modules.rst
+-rw-r--r--   0        0        0     8470 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/reference/ownership-mechanism-and-readonly-flags.ipynb
+-rw-r--r--   0        0        0     3331 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/reference/testing.rst
+-rw-r--r--   0        0        0    20556 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/reference/units.ipynb
+-rw-r--r--   0        0        0    14176 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/binned-data/binned-data.ipynb
+-rw-r--r--   0        0        0    14539 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/binned-data/computation.ipynb
+-rw-r--r--   0        0        0    15043 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/binned-data/filtering.ipynb
+-rw-r--r--   0        0        0     7868 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/binned-data/histogramming-grouping-and-binning.ipynb
+-rw-r--r--   0        0        0     1344 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/binned-data/prepare-filtering-data.py
+-rw-r--r--   0        0        0      184 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/binned-data.rst
+-rw-r--r--   0        0        0    13978 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/computation.ipynb
+-rw-r--r--   0        0        0    20727 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/coordinate-transformations.ipynb
+-rw-r--r--   0        0        0    17903 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/data-structures/creating-arrays-and-datasets.ipynb
+-rw-r--r--   0        0        0    19716 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/data-structures/data-structures.ipynb
+-rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/data-structures.rst
+-rw-r--r--   0        0        0     6008 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/groupby.ipynb
+-rw-r--r--   0        0        0      269 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/index.rst
+-rw-r--r--   0        0        0     7302 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/masking.ipynb
+-rw-r--r--   0        0        0     8665 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/plotting.ipynb
+-rw-r--r--   0        0        0     6030 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/reading-and-writing-files.ipynb
+-rw-r--r--   0        0        0    12367 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/representations-and-tables.ipynb
+-rw-r--r--   0        0        0    27277 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/slicing.ipynb
+-rw-r--r--   0        0        0    21269 2022-11-09 12:37:21.000000 scipp-24.5.0/docs/user-guide/tips-tricks-and-anti-patterns.ipynb
+-rw-r--r--   0        0        0     7122 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/CMakeLists.txt
+-rw-r--r--   0        0        0     3224 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/CMakeLists.txt
+-rw-r--r--   0        0        0     1972 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/accumulate_benchmark.cpp
+-rw-r--r--   0        0        0     2253 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/bin_benchmark.cpp
+-rw-r--r--   0        0        0     2777 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/buckets_benchmark.cpp
+-rw-r--r--   0        0        0      988 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/common.h
+-rw-r--r--   0        0        0     9097 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/dataset_benchmark.cpp
+-rw-r--r--   0        0        0     6586 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/dataset_operations_benchmark.cpp
+-rw-r--r--   0        0        0     2721 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/element_array_view_benchmark.cpp
+-rw-r--r--   0        0        0     4358 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/events_histogram_op_benchmark.cpp
+-rw-r--r--   0        0        0     4577 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/groupby_benchmark.cpp
+-rw-r--r--   0        0        0     2193 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/histogram_benchmark.cpp
+-rw-r--r--   0        0        0     6414 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/legacy_cow_ptr.h
+-rw-r--r--   0        0        0    14878 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/legacy_dataset_benchmark.cpp
+-rw-r--r--   0        0        0     9270 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/legacy_histogram_benchmark.cpp
+-rw-r--r--   0        0        0     1028 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/multi_index_benchmark.cpp
+-rw-r--r--   0        0        0     1969 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/slice_benchmark.cpp
+-rw-r--r--   0        0        0    10108 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/transform_benchmark.cpp
+-rw-r--r--   0        0        0     7050 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/variable_benchmark.cpp
+-rw-r--r--   0        0        0      909 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/benchmark/variable_common.h
+-rw-r--r--   0        0        0     3101 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/.conan-recipes/llnl-units/conanfile.py
+-rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/.conan-recipes/pybind11/conandata.yml
+-rw-r--r--   0        0        0     4632 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/.conan-recipes/pybind11/conanfile.py
+-rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/.conan-recipes/pybind11/conanmanifest.txt
+-rw-r--r--   0        0        0    29291 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/CodeCoverage.cmake
+-rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/IPO.cmake
+-rw-r--r--   0        0        0      174 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/generated.h.in
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/sanitizers-cmake/.git
+-rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/sanitizers-cmake/.gitignore
+-rw-r--r--   0        0        0     1518 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/sanitizers-cmake/CMakeLists.txt
+-rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/sanitizers-cmake/LICENSE
+-rw-r--r--   0        0        0     3474 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/sanitizers-cmake/README.md
+-rw-r--r--   0        0        0     2144 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/sanitizers-cmake/cmake/FindASan.cmake
+-rw-r--r--   0        0        0     2292 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/sanitizers-cmake/cmake/FindMSan.cmake
+-rwxr-xr-x   0        0        0     3737 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/sanitizers-cmake/cmake/FindSanitizers.cmake
+-rw-r--r--   0        0        0     2555 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/sanitizers-cmake/cmake/FindTSan.cmake
+-rw-r--r--   0        0        0     1696 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/sanitizers-cmake/cmake/FindUBSan.cmake
+-rwxr-xr-x   0        0        0     2011 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/sanitizers-cmake/cmake/asan-wrapper
+-rwxr-xr-x   0        0        0     7684 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/sanitizers-cmake/cmake/sanitize-helpers.cmake
+-rw-r--r--   0        0        0     2072 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/sanitizers-cmake/tests/CMakeLists.txt
+-rw-r--r--   0        0        0     1513 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/sanitizers-cmake/tests/asan_test.cpp
+-rw-r--r--   0        0        0     1513 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/sanitizers-cmake/tests/shortest.ext.test.cpp
+-rw-r--r--   0        0        0     2560 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/scipp-conan.cmake
+-rw-r--r--   0        0        0      910 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/scipp-config.cmake.in
+-rw-r--r--   0        0        0     5641 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/scipp-functions.cmake
+-rw-r--r--   0        0        0     1450 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/scipp-install.cmake
+-rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/scipp-test.cmake
+-rw-r--r--   0        0        0     3242 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/cmake/scipp-util.cmake
+-rw-r--r--   0        0        0      763 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/common/CMakeLists.txt
+-rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/common/include/scipp/common/constants.h
+-rw-r--r--   0        0        0     1364 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/common/include/scipp/common/except.h
+-rw-r--r--   0        0        0      810 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/common/include/scipp/common/index.h
+-rw-r--r--   0        0        0     4952 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/common/include/scipp/common/index_composition.h
+-rw-r--r--   0        0        0      836 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/common/include/scipp/common/initialization.h
+-rw-r--r--   0        0        0     4796 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/common/include/scipp/common/numeric.h
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/common/include/scipp/common/overloaded.h
+-rw-r--r--   0        0        0      582 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/common/include/scipp/common/ranges.h
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/common/include/scipp/common/span.h
+-rw-r--r--   0        0        0    18029 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/common/include/scipp/common/span.hpp.in
+-rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/common/test/CMakeLists.txt
+-rw-r--r--   0        0        0     6395 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/common/test/index_test.cpp
+-rw-r--r--   0        0        0     1499 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/common/test/isarange_test.cpp
+-rw-r--r--   0        0        0     2078 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/common/test/islinspace_test.cpp
+-rw-r--r--   0        0        0     2649 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/common/test/numeric_test.cpp
+-rw-r--r--   0        0        0     2997 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/CMakeLists.txt
+-rw-r--r--   0        0        0     1146 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/dict.cpp
+-rw-r--r--   0        0        0     5723 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/dimensions.cpp
+-rw-r--r--   0        0        0     2201 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/dtype.cpp
+-rw-r--r--   0        0        0     3184 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/element_array_view.cpp
+-rw-r--r--   0        0        0     3965 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/except.cpp
+-rw-r--r--   0        0        0     5011 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/aligned_allocator.h
+-rw-r--r--   0        0        0     2878 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/array_to_string.h
+-rw-r--r--   0        0        0      599 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/bucket.h
+-rw-r--r--   0        0        0     2409 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/bucket_array_view.h
+-rw-r--r--   0        0        0    13194 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/dict.h
+-rw-r--r--   0        0        0     3552 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/dimensions.h
+-rw-r--r--   0        0        0     5494 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/dtype.h
+-rw-r--r--   0        0        0     1817 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/eigen.h
+-rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/arg_list.h
+-rw-r--r--   0        0        0     9240 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/arithmetic.h
+-rw-r--r--   0        0        0     9270 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/bin.h
+-rw-r--r--   0        0        0     2322 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/bin_detail.h
+-rw-r--r--   0        0        0     5602 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/comparison.h
+-rw-r--r--   0        0        0     2040 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/creation.h
+-rw-r--r--   0        0        0     1099 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/cumulative.h
+-rw-r--r--   0        0        0     7515 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/event_operations.h
+-rw-r--r--   0        0        0     1415 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/geometric_operations.h
+-rw-r--r--   0        0        0     3805 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/histogram.h
+-rw-r--r--   0        0        0     1744 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/hyperbolic.h
+-rw-r--r--   0        0        0     1749 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/logical.h
+-rw-r--r--   0        0        0     5733 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/map_to_bins.h
+-rw-r--r--   0        0        0     7145 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/math.h
+-rw-r--r--   0        0        0     2706 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/rebin.h
+-rw-r--r--   0        0        0      896 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/reduction.h
+-rw-r--r--   0        0        0     1758 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/sort.h
+-rw-r--r--   0        0        0     4628 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/special_values.h
+-rw-r--r--   0        0        0     2108 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/to_unit.h
+-rw-r--r--   0        0        0     2056 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/trigonometry.h
+-rw-r--r--   0        0        0     5872 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element/util.h
+-rw-r--r--   0        0        0     5467 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element_array.h
+-rw-r--r--   0        0        0     5432 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/element_array_view.h
+-rw-r--r--   0        0        0     4373 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/except.h
+-rw-r--r--   0        0        0      466 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/flags.h
+-rw-r--r--   0        0        0      576 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/has_eval.h
+-rw-r--r--   0        0        0     1518 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/histogram.h
+-rw-r--r--   0        0        0     2329 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/memory_pool.h
+-rw-r--r--   0        0        0    11578 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/multi_index.h
+-rw-r--r--   0        0        0     1007 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/parallel-fallback.h
+-rw-r--r--   0        0        0     1288 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/parallel-tbb.h
+-rw-r--r--   0        0        0     4024 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/sizes.h
+-rw-r--r--   0        0        0     1287 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/slice.h
+-rw-r--r--   0        0        0     5162 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/spatial_transforms.h
+-rw-r--r--   0        0        0     2125 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/strides.h
+-rw-r--r--   0        0        0     1880 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/string.h
+-rw-r--r--   0        0        0     1827 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/subbin_sizes.h
+-rw-r--r--   0        0        0     1157 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/tag_util.h
+-rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/time_point.h
+-rw-r--r--   0        0        0     4760 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/transform_common.h
+-rw-r--r--   0        0        0    11054 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/value_and_variance.h
+-rw-r--r--   0        0        0     3306 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/values_and_variances.h
+-rw-r--r--   0        0        0     3839 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/include/scipp/core/view_index.h
+-rw-r--r--   0        0        0     8626 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/multi_index.cpp
+-rw-r--r--   0        0        0      914 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/rename.h
+-rw-r--r--   0        0        0     6893 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/sizes.cpp
+-rw-r--r--   0        0        0     1865 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/slice.cpp
+-rw-r--r--   0        0        0     1420 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/strides.cpp
+-rw-r--r--   0        0        0     5180 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/string.cpp
+-rw-r--r--   0        0        0     3667 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/subbin_sizes.cpp
+-rw-r--r--   0        0        0     1544 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/CMakeLists.txt
+-rw-r--r--   0        0        0    29139 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/arithmetic_parameters.h
+-rw-r--r--   0        0        0     3501 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/array_to_string_test.cpp
+-rw-r--r--   0        0        0    17697 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/dict_test.cpp
+-rw-r--r--   0        0        0     9648 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/dimensions_test.cpp
+-rw-r--r--   0        0        0     2462 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/dtype_test.cpp
+-rw-r--r--   0        0        0      808 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/eigen_test.cpp
+-rw-r--r--   0        0        0     8693 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/element_arithmetic_test.cpp
+-rw-r--r--   0        0        0     4525 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/element_array_test.cpp
+-rw-r--r--   0        0        0    17688 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/element_array_view_test.cpp
+-rw-r--r--   0        0        0     1838 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/element_bin_detail_test.cpp
+-rw-r--r--   0        0        0     8174 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/element_comparison_test.cpp
+-rw-r--r--   0        0        0     5551 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/element_event_operations_test.cpp
+-rw-r--r--   0        0        0     1336 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/element_geometric_operations_test.cpp
+-rw-r--r--   0        0        0     2767 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/element_histogram_test.cpp
+-rw-r--r--   0        0        0     2494 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/element_hyperbolic_test.cpp
+-rw-r--r--   0        0        0     2340 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/element_logical_test.cpp
+-rw-r--r--   0        0        0     3068 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/element_map_to_bins_test.cpp
+-rw-r--r--   0        0        0     7918 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/element_math_test.cpp
+-rw-r--r--   0        0        0    13263 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/element_special_values_test.cpp
+-rw-r--r--   0        0        0     3919 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/element_to_unit_test.cpp
+-rw-r--r--   0        0        0     6999 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/element_trigonometry_test.cpp
+-rw-r--r--   0        0        0     5296 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/element_util_test.cpp
+-rw-r--r--   0        0        0     2365 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/generate_arithmetic_parameters.py
+-rw-r--r--   0        0        0    19137 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/multi_index_test.cpp
+-rw-r--r--   0        0        0     4297 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/sizes_test.cpp
+-rw-r--r--   0        0        0     2090 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/slice_test.cpp
+-rw-r--r--   0        0        0     2444 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/spatial_transforms_test.cpp
+-rw-r--r--   0        0        0      487 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/strides_test.cpp
+-rw-r--r--   0        0        0     1605 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/string_test.cpp
+-rw-r--r--   0        0        0     4735 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/subbin_sizes_test.cpp
+-rw-r--r--   0        0        0     1504 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/time_point_test.cpp
+-rw-r--r--   0        0        0     1475 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/transform_common_test.cpp
+-rw-r--r--   0        0        0    10385 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/value_and_variance_test.cpp
+-rw-r--r--   0        0        0     4447 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/test/view_index_test.cpp
+-rw-r--r--   0        0        0     1177 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/core/view_index.cpp
+-rw-r--r--   0        0        0     2584 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/CMakeLists.txt
+-rw-r--r--   0        0        0     8025 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/arithmetic.cpp
+-rw-r--r--   0        0        0      702 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/astype.cpp
+-rw-r--r--   0        0        0    29481 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/bin.cpp
+-rw-r--r--   0        0        0      489 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/bin_common.h
+-rw-r--r--   0        0        0     4820 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/bin_detail.cpp
+-rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/bin_detail.h
+-rw-r--r--   0        0        0    16739 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/bins.cpp
+-rw-r--r--   0        0        0      999 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/bins_util.h
+-rw-r--r--   0        0        0     3389 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/counts.cpp
+-rw-r--r--   0        0        0     7397 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/data_array.cpp
+-rw-r--r--   0        0        0    12992 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/dataset.cpp
+-rw-r--r--   0        0        0     5851 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/dataset_operations_common.h
+-rw-r--r--   0        0        0     3558 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/except.cpp
+-rw-r--r--   0        0        0     5543 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/extract.cpp
+-rw-r--r--   0        0        0    15263 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/groupby.cpp
+-rw-r--r--   0        0        0     5612 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/histogram.cpp
+-rw-r--r--   0        0        0      208 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/arithmetic.h
+-rw-r--r--   0        0        0      413 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/astype.h
+-rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/bin.h
+-rw-r--r--   0        0        0     3446 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/bins.h
+-rw-r--r--   0        0        0     5857 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/bins_view.h
+-rw-r--r--   0        0        0     1420 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/counts.h
+-rw-r--r--   0        0        0     4902 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/data_array.h
+-rw-r--r--   0        0        0    12346 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/dataset.h
+-rw-r--r--   0        0        0     2214 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/dataset_util.h
+-rw-r--r--   0        0        0     2645 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/except.h
+-rw-r--r--   0        0        0      750 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/extract.h
+-rw-r--r--   0        0        0     3158 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/groupby.h
+-rw-r--r--   0        0        0      850 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/histogram.h
+-rw-r--r--   0        0        0      171 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/hyperbolic.h
+-rw-r--r--   0        0        0      205 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/logical.h
+-rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/math.h
+-rw-r--r--   0        0        0      636 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/mean.h
+-rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/nanmean.h
+-rw-r--r--   0        0        0      671 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/rebin.h
+-rw-r--r--   0        0        0     2090 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/shape.h
+-rw-r--r--   0        0        0     8069 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/sized_dict.h
+-rw-r--r--   0        0        0      822 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/sized_dict_forward.h
+-rw-r--r--   0        0        0     1917 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/slice.h
+-rw-r--r--   0        0        0     1027 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/sort.h
+-rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/special_values.h
+-rw-r--r--   0        0        0     1181 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/string.h
+-rw-r--r--   0        0        0      473 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/to_unit.h
+-rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/trigonometry.h
+-rw-r--r--   0        0        0     1022 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/include/scipp/dataset/util.h
+-rw-r--r--   0        0        0      986 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/mean.cpp
+-rw-r--r--   0        0        0     1047 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/nanmean.cpp
+-rw-r--r--   0        0        0     4897 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/operations.cpp
+-rw-r--r--   0        0        0     1207 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/rebin.cpp
+-rw-r--r--   0        0        0    12651 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/shape.cpp
+-rw-r--r--   0        0        0    16768 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/sized_dict.cpp
+-rw-r--r--   0        0        0     2604 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/slice.cpp
+-rw-r--r--   0        0        0     3580 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/sort.cpp
+-rw-r--r--   0        0        0     4645 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/string.cpp
+-rw-r--r--   0        0        0     1720 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/CMakeLists.txt
+-rw-r--r--   0        0        0     1636 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/astype_test.cpp
+-rw-r--r--   0        0        0     5195 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/attributes_test.cpp
+-rw-r--r--   0        0        0    34019 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/bin_test.cpp
+-rw-r--r--   0        0        0     7673 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/binned_arithmetic_test.cpp
+-rw-r--r--   0        0        0     2519 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/binned_creation_test.cpp
+-rw-r--r--   0        0        0     9381 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/bins_reduction_test.cpp
+-rw-r--r--   0        0        0    20826 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/bins_test.cpp
+-rw-r--r--   0        0        0     3447 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/bins_view_test.cpp
+-rw-r--r--   0        0        0    19172 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/concat_test.cpp
+-rw-r--r--   0        0        0    14221 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/coords_view_test.cpp
+-rw-r--r--   0        0        0     4445 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/copy_test.cpp
+-rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/counts_test.cpp
+-rw-r--r--   0        0        0     4829 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/data_array_arithmetic_test.cpp
+-rw-r--r--   0        0        0    11093 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/data_array_comparison_test.cpp
+-rw-r--r--   0        0        0    11989 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/data_array_test.cpp
+-rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/data_view_test.cpp
+-rw-r--r--   0        0        0    27585 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/dataset_arithmetic_test.cpp
+-rw-r--r--   0        0        0     6879 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/dataset_comparison_test.cpp
+-rw-r--r--   0        0        0     5606 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/dataset_operations_test.cpp
+-rw-r--r--   0        0        0    30843 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/dataset_test.cpp
+-rw-r--r--   0        0        0     4748 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/dataset_test_common.cpp
+-rw-r--r--   0        0        0     3089 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/dataset_test_common.h
+-rw-r--r--   0        0        0     3795 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/dataset_view_test.cpp
+-rw-r--r--   0        0        0     3423 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/equals_nan_test.cpp
+-rw-r--r--   0        0        0     3851 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/event_data_operations_consistency_test.cpp
+-rw-r--r--   0        0        0     3234 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/except_test.cpp
+-rw-r--r--   0        0        0     4592 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/generated_test.cpp
+-rw-r--r--   0        0        0    33843 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/groupby_test.cpp
+-rw-r--r--   0        0        0    20875 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/histogram_test.cpp
+-rw-r--r--   0        0        0     3357 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/logical_reduction_test.cpp
+-rw-r--r--   0        0        0     1850 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/masks_test.cpp
+-rw-r--r--   0        0        0    10331 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/mean_test.cpp
+-rw-r--r--   0        0        0     2756 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/merge_test.cpp
+-rw-r--r--   0        0        0     5310 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/minmax_test.cpp
+-rw-r--r--   0        0        0    11513 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/rebin_test.cpp
+-rw-r--r--   0        0        0     2647 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/self_assignment_test.cpp
+-rw-r--r--   0        0        0     8848 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/set_slice_test.cpp
+-rw-r--r--   0        0        0    31449 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/shape_test.cpp
+-rw-r--r--   0        0        0    16244 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/size_of_test.cpp
+-rw-r--r--   0        0        0    13721 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/slice_by_value_test.cpp
+-rw-r--r--   0        0        0    23135 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/slice_test.cpp
+-rw-r--r--   0        0        0     8470 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/sort_test.cpp
+-rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/string_test.cpp
+-rw-r--r--   0        0        0    13030 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/sum_test.cpp
+-rw-r--r--   0        0        0     1196 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/test_data_arrays.cpp
+-rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/test_data_arrays.h
+-rw-r--r--   0        0        0     4594 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/test/to_unit_test.cpp
+-rw-r--r--   0        0        0      745 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/to_unit.cpp
+-rw-r--r--   0        0        0     7730 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/util.cpp
+-rw-r--r--   0        0        0     7492 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/variable_instantiate_bin_elements.cpp
+-rw-r--r--   0        0        0      865 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/variable_instantiate_dataset.cpp
+-rw-r--r--   0        0        0     3349 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/dataset/variable_reduction.cpp
+-rw-r--r--   0        0        0        6 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/.gitignore
+-rw-r--r--   0        0        0     1557 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/CMakeLists.txt
+-rw-r--r--   0        0        0     1077 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/benchmark/variable.py
+-rw-r--r--   0        0        0    21243 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/bind_data_access.h
+-rw-r--r--   0        0        0    13221 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/bind_data_array.h
+-rw-r--r--   0        0        0    15104 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/bind_operators.h
+-rw-r--r--   0        0        0    13380 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/bind_slice_methods.h
+-rw-r--r--   0        0        0     8029 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/bind_units.cpp
+-rw-r--r--   0        0        0     8751 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/bins.cpp
+-rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/comparison.cpp
+-rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/counts.cpp
+-rw-r--r--   0        0        0     1165 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/cumulative.cpp
+-rw-r--r--   0        0        0    11084 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/dataset.cpp
+-rw-r--r--   0        0        0      823 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/dim.h
+-rw-r--r--   0        0        0     1843 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/docstring.cpp
+-rw-r--r--   0        0        0     1713 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/docstring.h
+-rw-r--r--   0        0        0    11316 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/dtype.cpp
+-rw-r--r--   0        0        0     1759 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/dtype.h
+-rw-r--r--   0        0        0     4530 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/element_array_view.cpp
+-rw-r--r--   0        0        0     3123 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/except.cpp
+-rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/format.h
+-rw-r--r--   0        0        0      260 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/generated.cpp.in
+-rw-r--r--   0        0        0     1008 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/geometry.cpp
+-rw-r--r--   0        0        0     2894 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/groupby.cpp
+-rw-r--r--   0        0        0     1182 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/histogram.cpp
+-rw-r--r--   0        0        0     1255 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/numpy.cpp
+-rw-r--r--   0        0        0    12432 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/numpy.h
+-rw-r--r--   0        0        0     4093 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/operations.cpp
+-rw-r--r--   0        0        0     1610 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/py_object.cpp
+-rw-r--r--   0        0        0     1499 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/py_object.h
+-rw-r--r--   0        0        0      736 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/pybind11.h
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/reduction.cpp
+-rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/rename.h
+-rw-r--r--   0        0        0     2572 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/scipp.cpp
+-rw-r--r--   0        0        0     3519 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/shape.cpp
+-rw-r--r--   0        0        0      785 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/slice_utils.cpp
+-rw-r--r--   0        0        0      337 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/slice_utils.h
+-rw-r--r--   0        0        0     1580 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/transform.cpp
+-rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/trigonometry.cpp
+-rw-r--r--   0        0        0     2787 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/unary.cpp
+-rw-r--r--   0        0        0     4282 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/unit.cpp
+-rw-r--r--   0        0        0     1615 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/unit.h
+-rw-r--r--   0        0        0     4305 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/variable.cpp
+-rw-r--r--   0        0        0     3076 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/variable_creation.cpp
+-rw-r--r--   0        0        0    13092 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/variable_init.cpp
+-rw-r--r--   0        0        0      507 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/variable_instantiate_py_object.cpp
+-rw-r--r--   0        0        0     4042 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/python/view.h
+-rw-r--r--   0        0        0      945 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/dataset_binary.cpp.in
+-rw-r--r--   0        0        0      532 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/dataset_binary.h.in
+-rw-r--r--   0        0        0      938 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/dataset_inplace.cpp.in
+-rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/dataset_inplace.h.in
+-rw-r--r--   0        0        0     1379 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/dataset_reduction.cpp.in
+-rw-r--r--   0        0        0      561 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/dataset_reduction.h.in
+-rw-r--r--   0        0        0      547 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/dataset_unary.cpp.in
+-rw-r--r--   0        0        0      399 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/dataset_unary.h.in
+-rw-r--r--   0        0        0      702 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/python_binary.cpp.in
+-rw-r--r--   0        0        0      830 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/python_reduction.cpp.in
+-rw-r--r--   0        0        0      917 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/python_unary.cpp.in
+-rw-r--r--   0        0        0     1030 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/variable_binary.cpp.in
+-rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/variable_binary.h.in
+-rw-r--r--   0        0        0      759 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/variable_inplace.cpp.in
+-rw-r--r--   0        0        0      446 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/variable_inplace.h.in
+-rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/variable_unary.cpp.in
+-rw-r--r--   0        0        0      497 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/templates/variable_unary.h.in
+-rw-r--r--   0        0        0      218 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/test/CMakeLists.txt
+-rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/test/fix_typed_test_suite_warnings.h
+-rw-r--r--   0        0        0     1387 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/test/random.h
+-rw-r--r--   0        0        0     3334 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/test/test_macros.h
+-rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/test/test_nans.h
+-rw-r--r--   0        0        0     1575 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/test/test_operations.h
+-rw-r--r--   0        0        0      788 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/test/test_print_variable.h
+-rw-r--r--   0        0        0      458 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/test/test_util.h
+-rw-r--r--   0        0        0     1331 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/units/CMakeLists.txt
+-rw-r--r--   0        0        0     2442 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/units/dim.cpp
+-rw-r--r--   0        0        0      617 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/units/except.cpp
+-rw-r--r--   0        0        0     2871 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/units/include/scipp/units/dim.h
+-rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/units/include/scipp/units/except.h
+-rw-r--r--   0        0        0      660 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/units/include/scipp/units/string.h
+-rw-r--r--   0        0        0     4650 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/units/include/scipp/units/unit.h
+-rw-r--r--   0        0        0      849 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/units/string.cpp
+-rw-r--r--   0        0        0      663 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/units/test/CMakeLists.txt
+-rw-r--r--   0        0        0     2458 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/units/test/dim_test.cpp
+-rw-r--r--   0        0        0    11943 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/units/test/unit_test.cpp
+-rw-r--r--   0        0        0     7361 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/units/unit.cpp
+-rw-r--r--   0        0        0     3517 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/CMakeLists.txt
+-rw-r--r--   0        0        0     4113 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/arithmetic.cpp
+-rw-r--r--   0        0        0     2762 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/astype.cpp
+-rw-r--r--   0        0        0     1225 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/bin_array_variable.cpp
+-rw-r--r--   0        0        0     3392 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/bin_detail.cpp
+-rw-r--r--   0        0        0      902 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/bin_util.cpp
+-rw-r--r--   0        0        0     2968 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/bins.cpp
+-rw-r--r--   0        0        0     2583 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/comparison.cpp
+-rw-r--r--   0        0        0     3744 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/creation.cpp
+-rw-r--r--   0        0        0     2085 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/cumulative.cpp
+-rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/except.cpp
+-rw-r--r--   0        0        0     7890 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/accumulate.h
+-rw-r--r--   0        0        0     2393 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/arithmetic.h
+-rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/astype.h
+-rw-r--r--   0        0        0     5536 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/bin_array_model.h
+-rw-r--r--   0        0        0    11591 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/bin_array_variable.tcc
+-rw-r--r--   0        0        0     1200 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/bin_detail.h
+-rw-r--r--   0        0        0      418 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/bin_util.h
+-rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/bins.h
+-rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/comparison.h
+-rw-r--r--   0        0        0     1220 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/creation.h
+-rw-r--r--   0        0        0      784 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/cumulative.h
+-rw-r--r--   0        0        0     5542 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/element_array_model.h
+-rw-r--r--   0        0        0     7218 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/element_array_variable.tcc
+-rw-r--r--   0        0        0      831 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/except.h
+-rw-r--r--   0        0        0      244 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/hyperbolic.h
+-rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/inv.h
+-rw-r--r--   0        0        0      206 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/logical.h
+-rw-r--r--   0        0        0      452 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/math.h
+-rw-r--r--   0        0        0      534 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/misc_operations.h
+-rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/operations.h
+-rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/pow.h
+-rw-r--r--   0        0        0      587 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/rebin.h
+-rw-r--r--   0        0        0     4065 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/reduction.h
+-rw-r--r--   0        0        0     1681 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/shape.h
+-rw-r--r--   0        0        0      628 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/slice.h
+-rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/sort.h
+-rw-r--r--   0        0        0     1195 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/special_values.h
+-rw-r--r--   0        0        0     2498 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/string.h
+-rw-r--r--   0        0        0     5128 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/structure_array_model.h
+-rw-r--r--   0        0        0     3401 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/structure_array_variable.tcc
+-rw-r--r--   0        0        0     1392 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/structures.h
+-rw-r--r--   0        0        0      794 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/subspan_view.h
+-rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/to_unit.h
+-rw-r--r--   0        0        0    33612 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/transform.h
+-rw-r--r--   0        0        0     4163 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/transform_subspan.h
+-rw-r--r--   0        0        0      283 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/trigonometry.h
+-rw-r--r--   0        0        0     1998 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/util.h
+-rw-r--r--   0        0        0     8922 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/variable.h
+-rw-r--r--   0        0        0     5827 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/variable.tcc
+-rw-r--r--   0        0        0     2438 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/variable_concept.h
+-rw-r--r--   0        0        0     5335 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/variable_factory.h
+-rw-r--r--   0        0        0     3650 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/variable_keyword_arg_constructor.h
+-rw-r--r--   0        0        0     4049 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/include/scipp/variable/visit.h
+-rw-r--r--   0        0        0     1876 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/inv.cpp
+-rw-r--r--   0        0        0     1245 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/math.cpp
+-rw-r--r--   0        0        0     1230 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/operations.cpp
+-rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/operations_common.h
+-rw-r--r--   0        0        0     4257 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/pow.cpp
+-rw-r--r--   0        0        0     7550 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/rebin.cpp
+-rw-r--r--   0        0        0    10235 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/reduction.cpp
+-rw-r--r--   0        0        0     5616 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/shape.cpp
+-rw-r--r--   0        0        0     4893 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/slice.cpp
+-rw-r--r--   0        0        0      774 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/sort.cpp
+-rw-r--r--   0        0        0     1662 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/special_values.cpp
+-rw-r--r--   0        0        0     4598 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/string.cpp
+-rw-r--r--   0        0        0     3639 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/structures.cpp
+-rw-r--r--   0        0        0     3840 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/subspan_view.cpp
+-rw-r--r--   0        0        0     1681 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/CMakeLists.txt
+-rw-r--r--   0        0        0     6920 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/accumulate_test.cpp
+-rw-r--r--   0        0        0     4457 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/arithmetic_test.cpp
+-rw-r--r--   0        0        0     4364 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/astype_test.cpp
+-rw-r--r--   0        0        0     5879 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/bin_array_model_test.cpp
+-rw-r--r--   0        0        0     1044 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/bin_util_test.cpp
+-rw-r--r--   0        0        0    13678 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/comparison_test.cpp
+-rw-r--r--   0        0        0     4680 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/concat_test.cpp
+-rw-r--r--   0        0        0     2842 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/copy_test.cpp
+-rw-r--r--   0        0        0     7013 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/creation_test.cpp
+-rw-r--r--   0        0        0     2749 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/cumulative_test.cpp
+-rw-r--r--   0        0        0     1620 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/equals_nan_test.cpp
+-rw-r--r--   0        0        0     1827 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/hyperbolic_test.cpp
+-rw-r--r--   0        0        0     2696 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/inv_test.cpp
+-rw-r--r--   0        0        0     2028 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/linalg_test.cpp
+-rw-r--r--   0        0        0    20416 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/math_test.cpp
+-rw-r--r--   0        0        0     6402 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/mean_test.cpp
+-rw-r--r--   0        0        0    36450 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/operations_test.cpp
+-rw-r--r--   0        0        0    14117 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/rebin_test.cpp
+-rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/reduce_logical_test.cpp
+-rw-r--r--   0        0        0     6591 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/reduce_various_test.cpp
+-rw-r--r--   0        0        0    12521 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/shape_test.cpp
+-rw-r--r--   0        0        0     2528 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/slice_test.cpp
+-rw-r--r--   0        0        0     1538 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/sort_test.cpp
+-rw-r--r--   0        0        0     9531 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/special_values_test.cpp
+-rw-r--r--   0        0        0     6371 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/subspan_view_test.cpp
+-rw-r--r--   0        0        0     2691 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/sum_test.cpp
+-rw-r--r--   0        0        0     2319 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/test_variables.cpp
+-rw-r--r--   0        0        0      371 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/test_variables.h
+-rw-r--r--   0        0        0    11990 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/to_unit_test.cpp
+-rw-r--r--   0        0        0    26227 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/transform_binary_test.cpp
+-rw-r--r--   0        0        0    20584 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/transform_test.cpp
+-rw-r--r--   0        0        0     6304 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/transform_test_helpers.cpp
+-rw-r--r--   0        0        0     2895 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/transform_test_helpers.h
+-rw-r--r--   0        0        0    11461 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/transform_unary_test.cpp
+-rw-r--r--   0        0        0     6676 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/trigonometry_test.cpp
+-rw-r--r--   0        0        0     6417 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/util_test.cpp
+-rw-r--r--   0        0        0    10945 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/variable_bin_test.cpp
+-rw-r--r--   0        0        0     8872 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/variable_comparison_test.cpp
+-rw-r--r--   0        0        0     1168 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/variable_custom_type_test.cpp
+-rw-r--r--   0        0        0     7124 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/variable_keyword_args_constructor_test.cpp
+-rw-r--r--   0        0        0     3486 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/variable_scalar_accessors_test.cpp
+-rw-r--r--   0        0        0     3806 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/variable_structure_test.cpp
+-rw-r--r--   0        0        0    42123 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/test/variable_test.cpp
+-rw-r--r--   0        0        0     2839 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/to_unit.cpp
+-rw-r--r--   0        0        0     4829 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/util.cpp
+-rw-r--r--   0        0        0    11003 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/variable.cpp
+-rw-r--r--   0        0        0      218 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/variable_concept.cpp
+-rw-r--r--   0        0        0     3483 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/variable_factory.cpp
+-rw-r--r--   0        0        0     1010 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/variable_instantiate_basic.cpp
+-rw-r--r--   0        0        0     2677 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/variable_instantiate_bin_elements.cpp
+-rw-r--r--   0        0        0     3851 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/variable_instantiate_linalg.cpp
+-rw-r--r--   0        0        0     2426 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/variable_instantiate_map_elements.cpp
+-rw-r--r--   0        0        0     1980 2022-11-09 12:37:21.000000 scipp-24.5.0/lib/variable/variable_instantiate_view_elements.cpp
+-rw-r--r--   0        0        0     5627 2022-11-09 12:37:21.000000 scipp-24.5.0/pyproject.toml
+-rw-r--r--   0        0        0       27 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/asv.in
+-rw-r--r--   0        0        0      348 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/asv.txt
+-rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/base.in
+-rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/base.txt
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/build.in
+-rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/build.txt
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/ci.in
+-rw-r--r--   0        0        0      936 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/ci.txt
+-rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/coverage.in
+-rw-r--r--   0        0        0      243 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/coverage.txt
+-rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/docs.in
+-rw-r--r--   0        0        0     3450 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/docs.txt
+-rw-r--r--   0        0        0       74 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/extra.in
+-rw-r--r--   0        0        0     2134 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/extra.txt
+-rw-r--r--   0        0        0       11 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/static.in
+-rw-r--r--   0        0        0      575 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/static.txt
+-rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/test.in
+-rw-r--r--   0        0        0      664 2022-11-09 12:37:21.000000 scipp-24.5.0/requirements/test.txt
+-rw-r--r--   0        0        0   643740 2022-11-09 12:37:21.000000 scipp-24.5.0/resources/logo-2019-09-07.svg
+-rw-r--r--   0        0        0   107538 2022-11-09 12:37:21.000000 scipp-24.5.0/resources/logo-2021.svg
+-rw-r--r--   0        0        0    69135 2022-11-09 12:37:21.000000 scipp-24.5.0/resources/logo-2022.svg
+-rw-r--r--   0        0        0     8343 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/__init__.py
+-rw-r--r--   0        0        0     5840 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/_binding.py
+-rw-r--r--   0        0        0      557 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/_extend_units.py
+-rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/_scipp.pyi
+-rw-r--r--   0        0        0      478 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/binning/__init__.py
+-rw-r--r--   0        0        0      358 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/compat/__init__.py
+-rw-r--r--   0        0        0     6003 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/compat/dict.py
+-rw-r--r--   0        0        0     6918 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/compat/pandas_compat.py
+-rw-r--r--   0        0        0     5151 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/compat/wrapping.py
+-rw-r--r--   0        0        0     5820 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/compat/xarray_compat.py
+-rw-r--r--   0        0        0     4940 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/constants/__init__.py
+-rw-r--r--   0        0        0      255 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/coords/__init__.py
+-rw-r--r--   0        0        0      829 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/coords/coord.py
+-rw-r--r--   0        0        0     2555 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/coords/coord_table.py
+-rw-r--r--   0        0        0     5150 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/coords/graph.py
+-rw-r--r--   0        0        0      378 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/coords/options.py
+-rw-r--r--   0        0        0     7465 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/coords/rule.py
+-rw-r--r--   0        0        0    12238 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/coords/transform_coords.py
+-rw-r--r--   0        0        0     6838 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/__init__.py
+-rw-r--r--   0        0        0      889 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/_cpp_wrapper_util.py
+-rw-r--r--   0        0        0      702 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/_sizes.py
+-rw-r--r--   0        0        0      683 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/argument_handlers.py
+-rw-r--r--   0        0        0     5812 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/arithmetic.py
+-rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/assignments.py
+-rw-r--r--   0        0        0     6779 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/bin_remapping.py
+-rw-r--r--   0        0        0    24940 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/binning.py
+-rw-r--r--   0        0        0    19188 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/bins.py
+-rw-r--r--   0        0        0     9031 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/comparison.py
+-rw-r--r--   0        0        0     3718 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/concepts.py
+-rw-r--r--   0        0        0     1043 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/counts.py
+-rw-r--r--   0        0        0      486 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/cpp_classes.py
+-rw-r--r--   0        0        0    43936 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/cpp_classes.pyi
+-rw-r--r--   0        0        0     1349 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/cumulative.py
+-rw-r--r--   0        0        0    21510 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/data_group.py
+-rw-r--r--   0        0        0      827 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/dataset.py
+-rw-r--r--   0        0        0     1370 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/deprecation.py
+-rw-r--r--   0        0        0     5221 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/dimensions.py
+-rw-r--r--   0        0        0     1093 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/domains.py
+-rw-r--r--   0        0        0      836 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/groupby.py
+-rw-r--r--   0        0        0     3109 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/hyperbolic.py
+-rw-r--r--   0        0        0     5258 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/like.py
+-rw-r--r--   0        0        0     1788 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/logical.py
+-rw-r--r--   0        0        0     9596 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/math.py
+-rw-r--r--   0        0        0    10767 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/operations.py
+-rw-r--r--   0        0        0    28650 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/reduction.py
+-rw-r--r--   0        0        0    14075 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/shape.py
+-rw-r--r--   0        0        0     2181 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/structured.py
+-rw-r--r--   0        0        0     3732 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/trigonometry.py
+-rw-r--r--   0        0        0     2289 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/unary.py
+-rw-r--r--   0        0        0     1664 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/util.py
+-rw-r--r--   0        0        0    30301 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/core/variable.py
+-rw-r--r--   0        0        0    18785 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/curve_fit.py
+-rw-r--r--   0        0        0     3208 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/data/__init__.py
+-rw-r--r--   0        0        0       90 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/format/__init__.py
+-rw-r--r--   0        0        0     2904 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/format/_parse.py
+-rw-r--r--   0        0        0     7854 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/format/formatter.py
+-rw-r--r--   0        0        0      647 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/io/__init__.py
+-rw-r--r--   0        0        0     4806 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/io/csv.py
+-rw-r--r--   0        0        0    14762 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/io/hdf5.py
+-rw-r--r--   0        0        0     8052 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/logging.py
+-rw-r--r--   0        0        0     1065 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/object_list.py
+-rw-r--r--   0        0        0     2711 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/operations.py
+-rw-r--r--   0        0        0      352 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/plotting.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/py.typed
+-rw-r--r--   0        0        0     3128 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/reduction.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/scipy/__init__.py
+-rw-r--r--   0        0        0     2413 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/scipy/integrate/__init__.py
+-rw-r--r--   0        0        0     7834 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/scipy/interpolate/__init__.py
+-rw-r--r--   0        0        0    11206 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/scipy/ndimage/__init__.py
+-rw-r--r--   0        0        0    10308 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/scipy/optimize/__init__.py
+-rw-r--r--   0        0        0     5092 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/scipy/signal/__init__.py
+-rw-r--r--   0        0        0     1110 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/serialization.py
+-rw-r--r--   0        0        0    11937 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/spatial/__init__.py
+-rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/sphinxext/__init__.py
+-rw-r--r--   0        0        0     4127 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/sphinxext/autoplot.py
+-rw-r--r--   0        0        0      330 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/testing/__init__.py
+-rw-r--r--   0        0        0     8963 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/testing/assertions.py
+-rw-r--r--   0        0        0    10567 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/testing/strategies.py
+-rw-r--r--   0        0        0     2898 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/typing.py
+-rw-r--r--   0        0        0     6551 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/units/__init__.py
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/utils/__init__.py
+-rw-r--r--   0        0        0     3858 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/utils/collapse_and_slices.py
+-rw-r--r--   0        0        0     2604 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/utils/comparison.py
+-rw-r--r--   0        0        0      507 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/utils/graph.py
+-rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/utils/profile.py
+-rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/utils/pyshell.py
+-rw-r--r--   0        0        0     1307 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/utils/to_string.py
+-rw-r--r--   0        0        0      276 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/visualization/__init__.py
+-rw-r--r--   0        0        0     1306 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/visualization/colors.py
+-rw-r--r--   0        0        0     5600 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/visualization/formatting_datagroup_html.py
+-rw-r--r--   0        0        0    16215 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/visualization/formatting_html.py
+-rw-r--r--   0        0        0     1484 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/visualization/html.py
+-rw-r--r--   0        0        0     2650 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/visualization/resources.py
+-rw-r--r--   0        0        0    19419 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/visualization/show.py
+-rw-r--r--   0        0        0     7259 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/visualization/table.py
+-rw-r--r--   0        0        0      138 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/visualization/templates/__init__.py
+-rw-r--r--   0        0        0     3267 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/visualization/templates/datagroup.css
+-rw-r--r--   0        0        0      831 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/visualization/templates/dg_atomic_row.html
+-rw-r--r--   0        0        0     1238 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/visualization/templates/dg_collapsible_row.html
+-rw-r--r--   0        0        0      711 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/visualization/templates/dg_detail_list.html
+-rw-r--r--   0        0        0      888 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/visualization/templates/dg_repr.html
+-rw-r--r--   0        0        0     1574 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/visualization/templates/icons-svg-inline.html
+-rw-r--r--   0        0        0     8904 2022-11-09 12:37:21.000000 scipp-24.5.0/src/scipp/visualization/templates/style.css
+-rw-r--r--   0        0        0    37563 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/binning_test.py
+-rw-r--r--   0        0        0    24556 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/bins_test.py
+-rw-r--r--   0        0        0      520 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/common_test.py
+-rw-r--r--   0        0        0    11635 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/compat/dict_test.py
+-rw-r--r--   0        0        0    10818 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/compat/pandas_compat_test.py
+-rw-r--r--   0        0        0     3336 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/compat/wrapping_test.py
+-rw-r--r--   0        0        0    12169 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/compat/xarray_compat_test.py
+-rw-r--r--   0        0        0     3397 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/concepts_test.py
+-rw-r--r--   0        0        0      615 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     1051 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/constants/constants_test.py
+-rw-r--r--   0        0        0     5527 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/coords/graph_test.py
+-rw-r--r--   0        0        0    33736 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/coords/transform_coords_test.py
+-rw-r--r--   0        0        0    11791 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/core/arithmetic_test.py
+-rw-r--r--   0        0        0     9870 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/core/comparison_test.py
+-rw-r--r--   0        0        0     3700 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/core/logical_test.py
+-rw-r--r--   0        0        0     5210 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/core/math_test.py
+-rw-r--r--   0        0        0    32253 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/core/reduction_test.py
+-rw-r--r--   0        0        0      823 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/counts_test.py
+-rw-r--r--   0        0        0      692 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/cumulative_test.py
+-rw-r--r--   0        0        0    18423 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/curve_fit_test.py
+-rw-r--r--   0        0        0    22550 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/data_array_test.py
+-rw-r--r--   0        0        0    29107 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/data_group_test.py
+-rw-r--r--   0        0        0    22959 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/dataset_test.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/datasetslice_test.py
+-rw-r--r--   0        0        0     9961 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/datetime_test.py
+-rw-r--r--   0        0        0    15855 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/dicts_test.py
+-rw-r--r--   0        0        0     5168 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/domains_test.py
+-rw-r--r--   0        0        0     2870 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/dtype_test.py
+-rw-r--r--   0        0        0     2375 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/dynamic_binding_test.py
+-rw-r--r--   0        0        0     2326 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/elemwise_func_test.py
+-rw-r--r--   0        0        0     7077 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/format/format_test.py
+-rw-r--r--   0        0        0     4424 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/html/html_repr_test.py
+-rw-r--r--   0        0        0     2824 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/hypothesis/bin_test.py
+-rw-r--r--   0        0        0      810 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/hypothesis/histogram_test.py
+-rw-r--r--   0        0        0     1412 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/hypothesis/lookup_test.py
+-rw-r--r--   0        0        0     6183 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/hypothesis/strategies_test.py
+-rw-r--r--   0        0        0     2571 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/hypothesis/to_unit_test.py
+-rw-r--r--   0        0        0     2201 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/io/csv_test.py
+-rw-r--r--   0        0        0    11016 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/io/hdf5_test.py
+-rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/iteration_test.py
+-rw-r--r--   0        0        0     5664 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/lifetime_test.py
+-rw-r--r--   0        0        0     4660 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/linalg_test.py
+-rw-r--r--   0        0        0     8011 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/lookup_test.py
+-rw-r--r--   0        0        0     3434 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/numpy_test.py
+-rw-r--r--   0        0        0    12995 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/ownership_dataset_test.py
+-rw-r--r--   0        0        0    18448 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/ownership_variable_test.py
+-rw-r--r--   0        0        0     1032 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/python_scalar_operations_test.py
+-rw-r--r--   0        0        0     5958 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/readonly_test.py
+-rw-r--r--   0        0        0     1522 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/reduce_test.py
+-rw-r--r--   0        0        0     4440 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/rename_test.py
+-rw-r--r--   0        0        0     3940 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/repr_test.py
+-rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/scipp_test.py
+-rw-r--r--   0        0        0     2354 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/scipy/integrate_test.py
+-rw-r--r--   0        0        0     5900 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/scipy/interpolate/interp1d_test.py
+-rw-r--r--   0        0        0     7061 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/scipy/ndimage/footprint_filter_test.py
+-rw-r--r--   0        0        0     5242 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/scipy/ndimage/gaussian_filter_test.py
+-rw-r--r--   0        0        0    10329 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/scipy/optimize/curve_fit_test.py
+-rw-r--r--   0        0        0     1383 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/scipy/signal/butter_test.py
+-rw-r--r--   0        0        0     5855 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/scipy/signal/sosfiltfilt_test.py
+-rw-r--r--   0        0        0      604 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/serialization_test.py
+-rw-r--r--   0        0        0     1619 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/setitem_test.py
+-rw-r--r--   0        0        0     5153 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/shape_test.py
+-rw-r--r--   0        0        0     1083 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/show_test.py
+-rw-r--r--   0        0        0     4821 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/slice_bins_test.py
+-rw-r--r--   0        0        0     5708 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/slice_by_condition_test.py
+-rw-r--r--   0        0        0     3637 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/slice_by_index_list_test.py
+-rw-r--r--   0        0        0     4715 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/slice_test.py
+-rw-r--r--   0        0        0     9292 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/slicebyvalue_test.py
+-rw-r--r--   0        0        0     2584 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/spatial/affine_test.py
+-rw-r--r--   0        0        0     6782 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/spatial/linear_transform_test.py
+-rw-r--r--   0        0        0     3500 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/spatial/rotation_test.py
+-rw-r--r--   0        0        0      999 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/spatial/scaling_test.py
+-rw-r--r--   0        0        0     1694 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/spatial/translation_test.py
+-rw-r--r--   0        0        0     1834 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/spatial/vector_test.py
+-rw-r--r--   0        0        0     1226 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/structured_test.py
+-rw-r--r--   0        0        0    21595 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/testing/assertions_test.py
+-rw-r--r--   0        0        0     2381 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/to_unit_test.py
+-rw-r--r--   0        0        0     9613 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/unit_test.py
+-rw-r--r--   0        0        0     2359 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/utils/collapse_and_slices_test.py
+-rw-r--r--   0        0        0     3697 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/utils/comparison_test.py
+-rw-r--r--   0        0        0     1698 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/utils/to_string_test.py
+-rw-r--r--   0        0        0    35624 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/variable_creation_test.py
+-rw-r--r--   0        0        0    16605 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/variable_init_test.py
+-rw-r--r--   0        0        0     1843 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/variable_py_object_test.py
+-rw-r--r--   0        0        0     3115 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/variable_reduction_test.py
+-rw-r--r--   0        0        0     3678 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/variable_scalar_test.py
+-rw-r--r--   0        0        0    23092 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/variable_test.py
+-rw-r--r--   0        0        0     2701 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/variable_view_test.py
+-rw-r--r--   0        0        0     4462 2022-11-09 12:37:21.000000 scipp-24.5.0/tests/variance_broadcast_test.py
+-rw-r--r--   0        0        0      510 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/README.md
+-rw-r--r--   0        0        0     6134 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/benchmark_build.py
+-rw-r--r--   0        0        0      772 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/debug/debug_multi_index_fragment.h
+-rw-r--r--   0        0        0      854 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/debug/debugout.h
+-rw-r--r--   0        0        0     9363 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/metatoenv.py
+-rw-r--r--   0        0        0      252 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/migration/README.md
+-rw-r--r--   0        0        0     1161 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/migration/scipp-0.11-hdf5-files.py
+-rw-r--r--   0        0        0      953 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/migration/scipp-0.12-hdf5-files.py
+-rw-r--r--   0        0        0     2207 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/migration/scipp-0.13-hdf5-files.py
+-rw-r--r--   0        0        0     6886 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/plot_benchmarks.py
+-rwxr-xr-x   0        0        0      139 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/run-tests.sh.in
+-rwxr-xr-x   0        0        0       67 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/run_asan.sh
+-rwxr-xr-x   0        0        0     1145 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/run_sanitizer.sh
+-rwxr-xr-x   0        0        0       69 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/run_ubsan.sh
+-rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/scipp-coverage-index.html
+-rw-r--r--   0        0        0     1744 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/stubgen/README.md
+-rw-r--r--   0        0        0     4512 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/stubgen/__init__.py
+-rw-r--r--   0        0        0      556 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/stubgen/__main__.py
+-rw-r--r--   0        0        0     2212 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/stubgen/config.py
+-rw-r--r--   0        0        0     5454 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/stubgen/parse.py
+-rw-r--r--   0        0        0      446 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/stubgen/stub_template.py.template
+-rw-r--r--   0        0        0     9860 2022-11-09 12:37:21.000000 scipp-24.5.0/tools/stubgen/transformer.py
+-rw-r--r--   0        0        0     4207 2022-11-09 12:37:21.000000 scipp-24.5.0/tox.ini
+-rw-r--r--   0        0        0     5616 2022-11-09 12:37:21.000000 scipp-24.5.0/PKG-INFO
```

### Comparing `scipp-24.2.0/.clang-tidy` & `scipp-24.5.0/.clang-tidy`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/.cmake-format.json` & `scipp-24.5.0/.cmake-format.json`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/.github/workflows/conda.yml` & `scipp-24.5.0/.github/workflows/conda.yml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     shell: bash -l {0}  # required for conda env
 
 jobs:
   build_conda:
     name: Package build (${{ inputs.target }}, py${{ inputs.python-version }})
     runs-on: ${{ inputs.os }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: true
           fetch-depth: 0  # history required so cmake can determine version
 
       - uses: conda-incubator/setup-miniconda@v3
       - run: >
           conda install
@@ -43,11 +43,11 @@
           --variant-config-files=${CONDA_PREFIX}/conda_build_config.yaml
           --variant-config-files=${GITHUB_WORKSPACE}/conda/variants/${{ inputs.target }}.yaml
           --python="${{ inputs.python-version }}.* *_cpython"
           --no-anaconda-upload
           --override-channels
           --output-folder conda/package conda
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
-          name: conda-package-${{ inputs.os }}-py${{ inputs.python-version }}
+          name: conda-package-${{ inputs.target }}-py${{ inputs.python-version }}
           path: conda/package/*/scipp*.tar.bz2
```

### Comparing `scipp-24.2.0/.github/workflows/coverage.yml` & `scipp-24.5.0/.github/workflows/coverage.yml`

 * *Files 2% similar despite different names*

```diff
@@ -19,32 +19,32 @@
           # a matching gcov is used. Otherwise coverage results are incomplete/broken.
           sudo apt install --yes lcov g++-11
           sudo update-alternatives --install /usr/bin/g++ g++ /usr/bin/g++-11 100
           sudo update-alternatives --install /usr/bin/gcov gcov /usr/bin/gcov-11 100
           sudo update-alternatives --set g++ "/usr/bin/g++-11"
           sudo update-alternatives --set gcov "/usr/bin/gcov-11"
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: true
           fetch-depth: 0  # history required so cmake can determine version
 
       - name: Disable TBB for much faster compilation.
         run: cat .buildconfig/ci-linux.yml | grep -v 'gxx\|tbb' > env.yml
 
       - name: Setup conda environment
         uses: mamba-org/setup-micromamba@v1
         with:
           micromamba-version: 1.5.6-0
           environment-file: env.yml
           cache-environment: true
-          create-args: python=3.9
+          create-args: python=3.10
 
       - name: ccache
-        uses: hendrikmuhs/ccache-action@v1.2.12
+        uses: hendrikmuhs/ccache-action@v1.2.13
         with:
           key: coverage
 
       - name: C++ coverage
         run: |
           mkdir coverage_html
           cmake --preset coverage
@@ -56,14 +56,14 @@
           tox -e coverage
           rm -f coverage_html/python/.gitignore
 
       - name: Setup HTML
         run: mv tools/scipp-coverage-index.html coverage_html/index.html
 
       - name: Deploy
-        uses: JamesIves/github-pages-deploy-action@v4.5.0
+        uses: JamesIves/github-pages-deploy-action@v4.6.1
         with:
           repository-name: scipp/scipp-coverage
           branch: main
           folder: coverage_html
           single-commit: true
           ssh-key: ${{ secrets.COVERAGE_DEPLOY_KEY }}
```

### Comparing `scipp-24.2.0/.github/workflows/docs.yml` & `scipp-24.5.0/.github/workflows/docs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -35,36 +35,36 @@
 
 jobs:
   docs:
     name: Build documentation
     runs-on: ubuntu-22.04
     steps:
       - run: sudo apt install --yes graphviz pandoc
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           ref: ${{ inputs.branch == '' && github.ref_name || inputs.branch }}
           fetch-depth: 0  # history required so cmake can determine version
       - uses: actions/setup-python@v3
         with:
-          python-version: '3.9'
+          python-version: '3.10'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: |
           sleep 120  # PyPI upload have a small delay until visible, avoid workflow fails in release builds
           tox --skip-pkg-install -e docs -- scipp==${VERSION}
           echo "target=$(python docs/version.py --version=${VERSION} --action=get-target)" >> $GITHUB_ENV
         if: ${{ inputs.publish }}
       - run: tox -e docs
         if: ${{ !inputs.publish }}
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           name: html
           path: html/
 
-      - uses: JamesIves/github-pages-deploy-action@v4.5.0
+      - uses: JamesIves/github-pages-deploy-action@v4.6.1
         if: ${{ inputs.publish }}
         with:
           repository-name: scipp/scipp.github.io
           branch: master
           folder: html
           target-folder: ${{ env.target }}
           single-commit: true
```

### Comparing `scipp-24.2.0/.github/workflows/pr_and_main.yml` & `scipp-24.5.0/.github/workflows/pr_and_main.yml`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,18 @@
   cancel-in-progress: true  # cancel jobs from previous push
 
 jobs:
   formatting:
     runs-on: ubuntu-22.04
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - uses: actions/setup-python@v3
         with:
-          python-version: '3.9'
+          python-version: '3.10'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: tox -e static
       - uses: stefanzweifel/git-auto-commit-action@v5
         with:
           commit_message: Apply automatic formatting
 
@@ -36,18 +36,18 @@
     strategy:
       fail-fast: false
       matrix:
         variant:
         - {os: ubuntu-22.04, cmake-preset: ci-linux}
         - {os: macos-11, cmake-preset: ci-macos}
         - {os: windows-2019, cmake-preset: ci-windows}
-        python-version: ["3.9"]
+        python-version: ["3.10"]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: true
           fetch-depth: 0  # history required so cmake can determine version
 
       - uses: ilammy/msvc-dev-cmd@v1  # Required to set up MSVC dev environment for Ninja builds.
 
       - name: Setup conda environment
@@ -55,15 +55,15 @@
         with:
           micromamba-version: 1.5.6-0
           environment-file: .buildconfig/${{ matrix.variant.cmake-preset }}.yml
           cache-environment: true
           create-args: python=${{ matrix.python-version }}
 
       - name: ccache
-        uses: hendrikmuhs/ccache-action@v1.2.12
+        uses: hendrikmuhs/ccache-action@v1.2.13
         with:
           key: ${{ matrix.variant.os }}
 
       - name: Cache conan setup
         id: conan-cache-key
         run: |
           echo "key=$(/bin/date -u "+%Y%m%d")" >> $GITHUB_OUTPUT
```

### Comparing `scipp-24.2.0/.github/workflows/release-nightly.yml` & `scipp-24.5.0/.github/workflows/release-nightly.yml`

 * *Files 18% similar despite different names*

```diff
@@ -8,32 +8,35 @@
 jobs:
   build_wheels:
     name: Wheels
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-22.04]
-        build: [cp39, cp310]
+        build: [cp310]
     uses: ./.github/workflows/wheel.yml
     with:
       os: ${{ matrix.os }}
       build: ${{ matrix.build }}
 
   release:
     name: Make Release on GitHub
     needs: build_wheels
     runs-on: ubuntu-22.04
     permissions:
       contents: write
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/download-artifact@v3
+      - uses: actions/checkout@v4
+      - uses: actions/download-artifact@v4
+        with:
+          path: dist
+          merge-multiple: true
       - uses: actions/setup-python@v4
         with:
-          python-version: 3.9
+          python-version: "3.10"
       - run: python .github/workflows/rename-dev-wheels.py
       - uses: ncipollo/release-action@v1
         with:
           allowUpdates: true
           artifacts: 'dist/*.whl'
           body: 'Nightly release for testing of downstream projects.'
           makeLatest: false
```

### Comparing `scipp-24.2.0/.github/workflows/release.yml` & `scipp-24.5.0/.github/workflows/release.yml`

 * *Files 16% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     shell: bash -l {0}  # required for conda env
 
 jobs:
   check_release:
     name: Check if package can be released
     runs-on: ubuntu-22.04
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - uses: actions/setup-python@v3
         with:
-          python-version: '3.9'
+          python-version: '3.10'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: tox -e check-release
         if: github.event_name == 'release' && github.event.action == 'published'
 
   build_conda:
     name: Conda
@@ -29,97 +29,105 @@
     strategy:
       matrix:
         variant:
           - {os: ubuntu-22.04, target: linux_64}
           - {os: macos-11, target: osx_64}
           - {os: macos-11, target: osx_arm64}
           - {os: windows-2019, target: win_64}
-        python-version: ["3.9", "3.10", "3.11"]
+        python-version: ["3.10", "3.11"]
     uses: ./.github/workflows/conda.yml
     with:
       os: ${{ matrix.variant.os }}
       target: ${{ matrix.variant.target }}
       python-version: ${{ matrix.python-version }}
 
   build_sdist:
     name: Build SDist
     needs: check_release
     runs-on: ubuntu-22.04
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         submodules: true
         fetch-depth: 0  # history required so cmake can determine version
 
     - name: Build SDist
       run: pipx run build --sdist
 
     - name: Check metadata
       run: pipx run twine check dist/*
 
-    - uses: actions/upload-artifact@v3
+    - uses: actions/upload-artifact@v4
       with:
         name: dist
         path: dist/*.tar.gz
 
   build_wheels:
     name: Wheels
     needs: check_release
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-22.04, macos-11, windows-2019]
-        build: [cp39, cp310, cp311, cp312]
+        build: [cp310, cp311, cp312]
     uses: ./.github/workflows/wheel.yml
     with:
       os: ${{ matrix.os }}
       build: ${{ matrix.build }}
 
   upload_pypi:
     name: Deploy PyPI
     needs: [build_wheels, build_sdist, build_conda]
     runs-on: ubuntu-22.04
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
+        with:
+          path: dist
+          merge-multiple: true
+          pattern: 'dist*'
       - uses: actions/setup-python@v3
-      - uses: pypa/gh-action-pypi-publish@v1.8.11
+      - uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
 
   upload_conda:
     name: Deploy Conda Forge
     needs: [build_wheels, build_sdist, build_conda]
     runs-on: ubuntu-22.04
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
+        with:
+          path: dist
+          merge-multiple: true
+          pattern: 'conda*'
       - uses: conda-incubator/setup-miniconda@v3
         with:
-          python-version: '3.9'
+          python-version: '3.10'
       - run: conda install -c conda-forge --yes anaconda-client
       - run: anaconda --token ${{ secrets.ANACONDATOKEN }} upload --user scipp --label main $(ls conda-package-*/*/*.tar.bz2)
 
   manage-versions:
     name: Manage Versions
     needs: check_release
     runs-on: ubuntu-22.04
     outputs:
       version-new: ${{ steps.version.outputs.new }}
       version-replaced: ${{ steps.version.outputs.replaced }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0  # history required so cmake can determine version
       - uses: actions/setup-python@v3
         with:
-          python-version: '3.9'
+          python-version: '3.10'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - name: Set outputs
         id: version
         run: |
           echo "new=$(python docs/version.py --version=${GITHUB_REF_NAME} --action=is-new)" >> $GITHUB_OUTPUT
           echo "replaced=$(python docs/version.py --version=${GITHUB_REF_NAME} --action=get-replaced)" >> $GITHUB_OUTPUT
@@ -145,15 +153,15 @@
   assets:
     name: Upload docs
     needs: docs
     runs-on: 'ubuntu-22.04'
     permissions:
       contents: write  # This is needed so that the action can upload the asset
     steps:
-    - uses: actions/download-artifact@v3
+    - uses: actions/download-artifact@v4
     - name: Zip documentation
       run: |
         mv html documentation-${{ github.ref_name }}
         zip -r documentation-${{ github.ref_name }}.zip documentation-${{ github.ref_name }}
     - name: Upload release assets
       uses: svenstaro/upload-release-action@v2
       with:
```

### Comparing `scipp-24.2.0/.github/workflows/weekly.yml` & `scipp-24.5.0/.github/workflows/weekly.yml`

 * *Files 4% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 
 jobs:
   build_conda:
     strategy:
       matrix:
         variant:
           - {os: ubuntu-22.04, target: linux_64}
-        python-version: ["3.9", "3.11"]
+        python-version: ["3.10", "3.11"]
     uses: ./.github/workflows/conda.yml
     with:
       os: ${{ matrix.variant.os }}
       target: ${{ matrix.variant.target }}
       python-version: ${{ matrix.python-version }}
 
   build_wheels:
     strategy:
       matrix:
         os: [ubuntu-22.04]
-        build: [cp39, cp312]
+        build: [cp310, cp312]
     uses: ./.github/workflows/wheel.yml
     with:
       os: ${{ matrix.os }}
       build: ${{ matrix.build }}
```

### Comparing `scipp-24.2.0/.github/workflows/wheel.yml` & `scipp-24.5.0/.github/workflows/wheel.yml`

 * *Files 24% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 
 jobs:
   build_wheels:
     name: Wheels on ${{ inputs.os }}-${{ inputs.build }}
     runs-on: ${{ inputs.os }}
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         submodules: true
         fetch-depth: 0  # history required so cmake can determine version
 
-    - uses: pypa/cibuildwheel@v2.16.5
+    - uses: pypa/cibuildwheel@v2.18.1
       env:
         CIBW_BUILD: ${{ inputs.build }}-*
         MACOSX_DEPLOYMENT_TARGET: "10.15"
 
     - name: Verify clean directory
       run: git diff --exit-code
       shell: bash
 
     - name: Upload wheels
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       with:
-        name: dist
-        path: wheelhouse/*.whl
+        name: dist-${{ inputs.os }}-${{ inputs.build }}
+        path: wheelhouse/*.whl
```

### Comparing `scipp-24.2.0/.gitignore` & `scipp-24.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/.pre-commit-config.yaml` & `scipp-24.5.0/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -8,24 +8,14 @@
       - id: check-toml
       - id: check-yaml
         exclude: conda/meta.yaml
       - id: detect-private-key
       - id: trailing-whitespace
         args: [ --markdown-linebreak-ext=md ]
         exclude: '\.svg'
-  - repo: https://github.com/pycqa/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-        name: isort (python)
-  - repo: https://github.com/psf/black
-    rev: 23.1.0
-    hooks:
-      - id: black
-        exclude: src/scipp/core/cpp_classes.pyi
   - repo: https://github.com/pre-commit/mirrors-clang-format
     rev: v15.0.4
     hooks:
       - id: clang-format
         types: [ "c++" ]
   - repo: https://github.com/cheshirekow/cmake-format-precommit
     rev: v0.6.13
@@ -34,26 +24,22 @@
   - repo: https://github.com/kynan/nbstripout
     rev: 0.6.0
     hooks:
       - id: nbstripout
         types: [ "jupyter" ]
         args: [ "--drop-empty-cells",
                 "--extra-keys 'metadata.language_info.version cell.metadata.jp-MarkdownHeadingCollapsed cell.metadata.pycharm'" ]
-  - repo: https://github.com/pycqa/flake8
-    rev: 4.0.1
-    hooks:
-      - id: flake8
-        types: ["python"]
-        additional_dependencies: ["flake8-bugbear==22.10.27"]
-  - repo: https://github.com/pycqa/bandit
-    rev: 1.7.4
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.4.1
     hooks:
-      - id: bandit
-        additional_dependencies: ["bandit[toml]"]
-        args: ["-c", "pyproject.toml"]
+      - id: ruff
+        args: [ --fix ]
+        types_or: [ python, pyi, jupyter ]
+      - id: ruff-format
+        types_or: [ python, pyi ]
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.2
     hooks:
       - id: codespell
         additional_dependencies:
           - tomli
   - repo: https://github.com/pre-commit/pygrep-hooks
```

### Comparing `scipp-24.2.0/CMakeLists.txt` & `scipp-24.5.0/CMakeLists.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,51 +2,60 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # ~~~
 cmake_minimum_required(VERSION 3.21)
 
 cmake_policy(SET CMP0091 NEW)
 
-execute_process(
-  COMMAND git describe --tags --exclude nightly
-  WORKING_DIRECTORY "${CMAKE_SOURCE_DIR}"
-  RESULT_VARIABLE HAVE_GIT_VERSION_INFO
-  OUTPUT_VARIABLE GIT_VERSION_INFO
-  OUTPUT_STRIP_TRAILING_WHITESPACE
-)
-# We get something like 23.08.0-266-g068b161fe, remove the -g<hash> part
-string(REGEX REPLACE "-g[0-9a-f]+$" "" GIT_VERSION_INFO ${GIT_VERSION_INFO})
-# Replace '-' with '.dev' for PEP440 compatibility
-string(REGEX REPLACE "-" ".dev" SCIPP_VERSION_PEP440 ${GIT_VERSION_INFO})
-# Cmake does not like letters, remove the dev, will act as "tweak" number
-string(REGEX REPLACE "-" "" SCIPP_VERSION_CMAKE ${GIT_VERSION_INFO})
-
-project(
-  scipp
-  VERSION ${SCIPP_VERSION_CMAKE}
-  LANGUAGES CXX
-)
+if(SKBUILD)
+  project(
+    ${SKBUILD_PROJECT_NAME}
+    VERSION ${SKBUILD_PROJECT_VERSION}
+    LANGUAGES CXX
+  )
+  add_definitions(-DSCIPP_VERSION="${SKBUILD_PROJECT_VERSION_FULL}")
+  message(STATUS "Got version from SKBUILD: ${SKBUILD_PROJECT_VERSION_FULL}")
+else()
+  execute_process(
+    COMMAND git describe --tags --exclude nightly
+    WORKING_DIRECTORY "${CMAKE_SOURCE_DIR}"
+    RESULT_VARIABLE HAVE_GIT_VERSION_INFO
+    OUTPUT_VARIABLE GIT_VERSION_INFO
+    OUTPUT_STRIP_TRAILING_WHITESPACE
+  )
+  # We get something like 23.08.0-266-g068b161fe, remove the -g<hash> part
+  string(REGEX REPLACE "-g[0-9a-f]+$" "" GIT_VERSION_INFO ${GIT_VERSION_INFO})
+  # Replace '-' with '.dev' for PEP440 compatibility
+  string(REGEX REPLACE "-" ".dev" SCIPP_VERSION_PEP440 ${GIT_VERSION_INFO})
+  # Cmake does not like letters, remove the dev, will act as "tweak" number
+  string(REGEX REPLACE "-" "" SCIPP_VERSION_CMAKE ${GIT_VERSION_INFO})
+
+  project(
+    scipp
+    VERSION ${SCIPP_VERSION_CMAKE}
+    LANGUAGES CXX
+  )
+  if(${HAVE_GIT_VERSION_INFO} EQUAL 0)
+    message(STATUS "Got version from Git: ${GIT_VERSION_INFO}")
+    add_definitions(-DSCIPP_VERSION="${SCIPP_VERSION_PEP440}")
+  endif()
+endif()
 
 if(NOT CMAKE_BUILD_TYPE)
   set(CMAKE_BUILD_TYPE
       "Release"
       CACHE
         STRING
         "Choose the type of build, options are: Debug Release RelWithDebInfo MinSizeRel."
         FORCE
   )
 endif()
 
 set(CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake")
 
-if(${HAVE_GIT_VERSION_INFO} EQUAL 0)
-  message(STATUS "Got version from Git: ${GIT_VERSION_INFO}")
-  add_definitions(-DSCIPP_VERSION="${SCIPP_VERSION_PEP440}")
-endif()
-
 # Custom install target for docs to depend on.
 add_custom_target(
   install-scipp COMMAND cmake --build ${CMAKE_CURRENT_BINARY_DIR} --target
                         install
 )
 
 include(docs)
```

### Comparing `scipp-24.2.0/CMakePresets.json` & `scipp-24.5.0/CMakePresets.json`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/CODE_OF_CONDUCT.md` & `scipp-24.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/LICENSE` & `scipp-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/README.md` & `scipp-24.5.0/README.md`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/asv.conf.json` & `scipp-24.5.0/asv.conf.json`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/benchmarks/bin.py` & `scipp-24.5.0/benchmarks/bin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+from typing import ClassVar
+
 import numpy as np
 
 import scipp as sc
 from scipp.binning import make_binned
 
 
 class Bin2dRebinLongDim:
     """
     Benchmark sc.bin, changing existing long dimension
     """
 
-    params = (list(2 ** np.arange(10, 16)),)
-    param_names = ['nbin']
-    timeout = 300.0
+    params: ClassVar[tuple[list[int]]] = (list(2 ** np.arange(10, 16)),)
+    param_names: ClassVar[list[str]] = ['nbin']
+    timeout: ClassVar[float] = 300.0
 
     def setup(self, nbin):
         binned = sc.data.binned_x(nevent=2 * nbin, nbin=nbin)
         y = sc.linspace(dim='y', start=0, stop=1, num=2, unit='m')
         self.da = make_binned(binned, edges=[y])
         self.da_transposed = self.da.transpose().copy()
 
@@ -35,41 +37,41 @@
 
 
 class Bin1d:
     """
     Benchmark sc.bin, for 1d binning.
     """
 
-    params = (list(2 ** np.arange(0, 20)),)
+    params: ClassVar[tuple[list[int]]] = (list(2 ** np.arange(0, 20)),)
     # For full runs (too large for CI) use:
     # params = (list(2 ** np.arange(0, 25)),)
-    param_names = ['nbin']
-    timeout = 300.0
+    param_names: ClassVar[list[str]] = ['nbin']
+    timeout: ClassVar[float] = 300.0
 
     def setup(self, nbin):
         self.table = sc.data.table_xyz(50_000_000)
         self.x = sc.linspace(dim='x', start=0, stop=1, num=nbin + 1, unit='m')
 
     def time_bin_table(self, nbin):
         make_binned(self.table, edges=[self.x])
 
 
 class Group1d:
     """
     Benchmark sc.group, for 1d grouping.
     """
 
-    nevent = [1_000, 1_000_000, 10_000_000, 100_000_000]
-    ngroup = list(2 ** np.arange(2, 20))
+    nevent: ClassVar[list[int]] = [1_000, 1_000_000, 10_000_000, 100_000_000]
+    ngroup: ClassVar[list[int]] = list(2 ** np.arange(2, 20))
     # For full runs (too large for CI) use:
     # nevent = [1_000, 1_000_000, 10_000_000, 100_000_000]
     # ngroup = list(2 ** np.arange(2, 25))
-    params = (nevent, ngroup)
-    param_names = ['nevent', 'ngroup']
-    timeout = 300.0
+    params: ClassVar[tuple[list[int], list[int]]] = (nevent, ngroup)
+    param_names: ClassVar[list[str]] = ['nevent', 'ngroup']
+    timeout: ClassVar[float] = 300.0
 
     def setup(self, nevent, ngroup):
         self.table = sc.data.table_xyz(nevent)
         self.table.coords['group'] = (ngroup * self.table.coords['x']).to(dtype='int64')
         del self.table.coords['x']
         self.contiguous_groups = sc.arange('group', ngroup, unit='m')
         self.groups = sc.arange('group', ngroup, unit='m')
```

### Comparing `scipp-24.2.0/benchmarks/binned.py` & `scipp-24.5.0/benchmarks/binned.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+from typing import ClassVar
+
 import numpy as np
 
 import scipp as sc
 from scipp.binning import make_binned
 
 
 class Binned1d:
     """
     Benchmark different aspects of binned data
     """
 
-    params = (list(10 ** np.arange(8)), list(10 ** np.arange(0, 7)))
-    param_names = ['nevent', 'nbin']
+    params: ClassVar[tuple[list[int], list[int]]] = (
+        list(10 ** np.arange(8)),
+        list(10 ** np.arange(0, 7)),
+    )
+    param_names: ClassVar[list[str]] = ['nevent', 'nbin']
 
     def setup(self, nevent, nbin):
         self.da = sc.data.binned_x(nevent, nbin)
 
     def time_bins_constituents(self, nevent, nbin):
-        self.da.bins.constituents
+        self.da.bins.constituents  # noqa: B018
 
     def time_bins_size(self, nevent, nbin):
         self.da.bins.size()
 
     def time_bins_sum(self, nevent, nbin):
         self.da.bins.sum()
 
@@ -34,17 +39,17 @@
 
 
 class Binned2dConcat:
     """
     Benchmark reduction with 'concat' for 2d binned data
     """
 
-    params = ([1, 2, 4, 8, 16, 32, 64, 128],)
-    param_names = ['nbin']
-    timeout = 300.0
+    params: ClassVar[tuple[list[int]]] = ([1, 2, 4, 8, 16, 32, 64, 128],)
+    param_names: ClassVar[list[str]] = ['nbin']
+    timeout: ClassVar[int] = 300.0
 
     def setup(self, nbin):
         nx = 100000
         binned = sc.data.binned_x(nevent=2 * nx, nbin=nx)
         y = sc.linspace(dim='y', start=0, stop=1, num=nbin + 1, unit='m')
         self.da = make_binned(binned, edges=[y])
 
@@ -53,17 +58,17 @@
 
 
 class Binned2dConcatInner:
     """
     Benchmark reduction with 'concat' along inner for 2d binned data
     """
 
-    params = (list(2 ** np.arange(10, 16)),)
-    param_names = ['nbin']
-    timeout = 300.0
+    params: ClassVar[tuple[list[int]]] = (list(2 ** np.arange(10, 16)),)
+    param_names: ClassVar[list[str]] = ['nbin']
+    timeout: ClassVar[float] = 300.0
 
     def setup(self, nbin):
         binned = sc.data.binned_x(nevent=2 * nbin, nbin=nbin)
         y = sc.linspace(dim='y', start=0, stop=1, num=2, unit='m')
         self.da = make_binned(binned, edges=[y])
 
     def time_bins_concat_long_outer(self, nbin):
```

### Comparing `scipp-24.2.0/benchmarks/variable.py` & `scipp-24.5.0/benchmarks/variable.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/cmake/docs.cmake` & `scipp-24.5.0/cmake/docs.cmake`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/conda/README.md` & `scipp-24.5.0/conda/README.md`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/conda/cmake-package-test/CMakeLists.txt` & `scipp-24.5.0/conda/cmake-package-test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/conda/cmake-package-test/build.py` & `scipp-24.5.0/conda/cmake-package-test/build.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# ruff: noqa: S603, S607
+
 import os
 import subprocess
 import sys
 
 shell = sys.platform == 'win32'
 
 os.chdir(os.path.dirname(os.path.realpath(__file__)))
@@ -20,15 +22,15 @@
     cmake_flags.append(
         f'-DCMAKE_OSX_DEPLOYMENT_TARGET={os.getenv("OSX_VERSION", "10.14")}'
     )
 elif sys.platform == 'win32':
     cmake_flags.extend(['-G', 'Visual Studio 16 2019'])
 
 subprocess.check_call(
-    ['cmake'] + cmake_flags + ['..'], stderr=subprocess.STDOUT, shell=shell
+    ['cmake', *cmake_flags, '..'], stderr=subprocess.STDOUT, shell=shell
 )
 # Show cmake settings
 subprocess.check_call(
     ['cmake', '-B', '.', '-S', '..', '-LA'], stderr=subprocess.STDOUT, shell=shell
 )
 # TODO For some reason transitive dependencies such as boost include dirs to not work
 # on Windows
```

### Comparing `scipp-24.2.0/conda/meta.yaml` & `scipp-24.5.0/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/cppcheck-suppressions.txt` & `scipp-24.5.0/cppcheck-suppressions.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/_static/anaconda-icon.js` & `scipp-24.5.0/docs/_static/anaconda-icon.js`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/_static/favicon.ico` & `scipp-24.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/_static/logo-2022.svg` & `scipp-24.5.0/docs/_static/logo-2022.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/_static/logo-dark.svg` & `scipp-24.5.0/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/_static/title-filtering-1d-plot.svg` & `scipp-24.5.0/docs/_static/title-filtering-1d-plot.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/_static/title-repr-html.png` & `scipp-24.5.0/docs/_static/title-repr-html.png`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/_static/title-show-svg.png` & `scipp-24.5.0/docs/_static/title-show-svg.png`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/_templates/scipp-class-template.rst` & `scipp-24.5.0/docs/_templates/scipp-class-template.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/_templates/scipp-module-template.rst` & `scipp-24.5.0/docs/_templates/scipp-module-template.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/about/about.rst` & `scipp-24.5.0/docs/about/about.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/about/contributing.rst` & `scipp-24.5.0/docs/about/contributing.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/about/migration/23-01.ipynb` & `scipp-24.5.0/docs/about/migration/23-01.ipynb`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/about/release-notes.rst` & `scipp-24.5.0/docs/about/release-notes.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/about/roadmap.rst` & `scipp-24.5.0/docs/about/roadmap.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/conf.py` & `scipp-24.5.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import sys
 
 import scipp
 
 sys.path.insert(0, os.path.abspath('.'))
 
 # General information about the project.
-project = u'Scipp'
-copyright = u'2024 Scipp contributors'
-author = u'Scipp contributors'
+project = 'Scipp'
+copyright = '2024 Scipp contributors'
+author = 'Scipp contributors'
 
 html_show_sourcelink = True
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
@@ -62,15 +62,15 @@
     'MetaDataMap': 'MetaDataMap',
     'array_like': 'array_like',
 }
 
 rst_epilog = f"""
 .. |SCIPP_RELEASE_MONTH| replace:: {os.popen("git show -s --format=%cd --date=format:'%B %Y'").read()}
 .. |SCIPP_VERSION| replace:: {os.popen("git describe --tags --abbrev=0").read()}
-"""  # noqa: E501
+"""  # noqa: E501, S605, S607
 
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
     'numpy': ('https://numpy.org/doc/stable/', None),
     'pandas': ('https://pandas.pydata.org/docs/', None),
     'scipy': ('https://docs.scipy.org/doc/scipy/', None),
     'xarray': ('https://xarray.pydata.org/en/stable/', None),
@@ -126,15 +126,21 @@
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store', '**.ipynb_checkpoints']
+exclude_patterns = [
+    '_build',
+    'Thumbs.db',
+    '.DS_Store',
+    '**.ipynb_checkpoints',
+    'development/project',
+]
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = 'sphinx'
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
```

### Comparing `scipp-24.2.0/docs/development/adr/0001-remove-dataset-masking-support.rst` & `scipp-24.5.0/docs/development/adr/0001-remove-dataset-masking-support.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/adr/0002-remove-instrument-view-projection-options.rst` & `scipp-24.5.0/docs/development/adr/0002-remove-instrument-view-projection-options.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/adr/0003-refactor-plotting-code-with-mvc-pattern.rst` & `scipp-24.5.0/docs/development/adr/0003-refactor-plotting-code-with-mvc-pattern.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/adr/0004-use-ipympl-backend-for-matplotlib.rst` & `scipp-24.5.0/docs/development/adr/0004-use-ipympl-backend-for-matplotlib.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/adr/0005-remove-need-for-bins-property-when-calling-bin-or-histogram.rst` & `scipp-24.5.0/docs/development/adr/0005-remove-need-for-bins-property-when-calling-bin-or-histogram.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/adr/0006-add-readonly-flags.rst` & `scipp-24.5.0/docs/development/adr/0006-add-readonly-flags.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/adr/0007-do-not-support-args-referencing-x-or-y.rst` & `scipp-24.5.0/docs/development/adr/0007-do-not-support-args-referencing-x-or-y.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/adr/0008-consistent-multi-dimensional-coords.rst` & `scipp-24.5.0/docs/development/adr/0008-consistent-multi-dimensional-coords.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/adr/0009-handle-dimensionless-as-non-counts.rst` & `scipp-24.5.0/docs/development/adr/0009-handle-dimensionless-as-non-counts.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/adr/0010-acknowledge-stability-and-maintainability-tasks.rst` & `scipp-24.5.0/docs/development/adr/0010-acknowledge-stability-and-maintainability-tasks.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/adr/0011-renaming-of-dimensions-in-transform_coords.rst` & `scipp-24.5.0/docs/development/adr/0011-renaming-of-dimensions-in-transform_coords.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/adr/0012-rebin-should-apply-irreducible-masks.rst` & `scipp-24.5.0/docs/development/adr/0012-rebin-should-apply-irreducible-masks.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/adr/0013-plot-should-not-resample-automatically.rst` & `scipp-24.5.0/docs/development/adr/0013-plot-should-not-resample-automatically.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/adr/0014-switch-calendar-versioning.rst` & `scipp-24.5.0/docs/development/adr/0014-switch-calendar-versioning.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/adr/0015-disable-support-for-broadcasting-variances.rst` & `scipp-24.5.0/docs/development/adr/0015-disable-support-for-broadcasting-variances.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/adr/0016-do-not-support-attrs.rst` & `scipp-24.5.0/docs/development/adr/0016-do-not-support-attrs.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/adr/0017-restrict-dataset-to-items-with-matching-dimensionality.rst` & `scipp-24.5.0/docs/development/adr/0017-restrict-dataset-to-items-with-matching-dimensionality.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/coding-conventions.rst` & `scipp-24.5.0/docs/development/coding-conventions.rst`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 -------
 
 As a general rule all new functionality and bug fixes should be accompanied with sufficient unit tests to demonstrate that the feature or fix works as intended.
 
 Formatting
 ----------
 
-There are no explicit formatting conventions since we use ``clang-format`` (C++) and ``black`` (Python).
+There are no explicit formatting conventions since we use ``clang-format`` (C++) and ``ruff`` (Python).
 
 Docstrings
 ~~~~~~~~~~
 
 The exception to this are Python docstrings, for which we use the
 `NumPy docstring format <https://www.sphinx-doc.org/en/master/usage/extensions/example_numpy.html>`_.
 We use a tool to automatically insert type hints into the docstrings.
```

### Comparing `scipp-24.2.0/docs/development/dependencies.rst` & `scipp-24.5.0/docs/development/dependencies.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/getting-started.rst` & `scipp-24.5.0/docs/development/getting-started.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/internals/concepts.ipynb` & `scipp-24.5.0/docs/development/internals/concepts.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9966742740258627%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(3, "x = sc.Variable(dims=[\'x\'], values=[1, 2, 3, '*

 * *            '4])\\n"), (4, "da = sc.DataArray(data=x, coords={\'x\': x}, masks={\'x\': sc.less(x, '*

 * *            '2 * sc.units.one)})\\n"), (5, "ds = sc.Dataset(data={\'a\': da})")], delete: [7, 6, '*

 * *            "5, 4, 3]}}, 7: {'source': {insert: [(2, 'except RuntimeError:\\n')], delete: [2]}}, "*

 * *            '18: {\'source\': {insert: [(0, "edges = sc.Variable(dims=[\'x\'], values=[1, 2, 3, 4, '*

 * *            '5])\\n […]*

```diff
@@ -16,19 +16,17 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import scipp as sc\n",
                 "\n",
-                "x = sc.Variable(dims=['x'], values=[1,2,3,4])\n",
-                "da = sc.DataArray(data=x,\n",
-                "                  coords={'x':x},\n",
-                "                  masks={'x':sc.less(x, 2 * sc.units.one)})\n",
-                "ds = sc.Dataset(data={'a':da})"
+                "x = sc.Variable(dims=['x'], values=[1, 2, 3, 4])\n",
+                "da = sc.DataArray(data=x, coords={'x': x}, masks={'x': sc.less(x, 2 * sc.units.one)})\n",
+                "ds = sc.Dataset(data={'a': da})"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Consider a data array `da` and a dataset `ds` with an aligned coord and an aligned mask.\n",
@@ -92,15 +90,15 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "try:\n",
                 "    ok = da['x', 0:1] + da['x', 1:2]\n",
-                "except:\n",
+                "except RuntimeError:\n",
                 "    ok = False\n",
                 "assert not ok"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -207,21 +205,24 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "edges = sc.Variable(dims=['x'], values=[1,2,3,4,5])\n",
+                "edges = sc.Variable(dims=['x'], values=[1, 2, 3, 4, 5])\n",
                 "da.coords['x'] = edges\n",
                 "assert sc.identical(sc.concat([da['x', :2], da['x', 2:]], 'x'), da)\n",
                 "assert sc.identical(sc.concat([da['x', 0], da['x', 1]], 'x'), da['x', 0:2])\n",
                 "assert sc.identical(sc.concat([da['x', :-1], da['x', -1]], 'x'), da)\n",
-                "da_yx = sc.concat([da['x', :2], da['x', 2:]], 'y') # create 2-D coord\n",
-                "assert sc.identical(da_yx.coords['x'], sc.concat([da.coords['x']['x', :3], da.coords['x']['x', 2:]], 'y'))"
+                "da_yx = sc.concat([da['x', :2], da['x', 2:]], 'y')  # create 2-D coord\n",
+                "assert sc.identical(\n",
+                "    da_yx.coords['x'],\n",
+                "    sc.concat([da.coords['x']['x', :3], da.coords['x']['x', 2:]], 'y'),\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "2-D coords for a dimension prevent operations between slices that are not along that dimension:"
@@ -234,21 +235,25 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "da_2d = sc.DataArray(\n",
                 "    data=sc.zeros(dims=['y', 'x'], shape=[2, 2]),\n",
                 "    coords={\n",
-                "        'x':sc.Variable(dims=['y', 'x'], values=np.array([[1, 2], [3, 4]])),\n",
-                "        'y':sc.Variable(dims=['y'], values=[3, 4])})\n",
+                "        'x': sc.Variable(dims=['y', 'x'], values=np.array([[1, 2], [3, 4]])),\n",
+                "        'y': sc.Variable(dims=['y'], values=[3, 4]),\n",
+                "    },\n",
+                ")\n",
                 "\n",
-                "da_2d['x', 0] + da_2d['x', 1] # Same as with 1-D coord: x-coord differs but not aligned due to slice.\n",
+                "(\n",
+                "    da_2d['x', 0] + da_2d['x', 1]\n",
+                ")  # Same as with 1-D coord: x-coord differs but not aligned due to slice.\n",
                 "try:\n",
                 "    # 'y' sliced, so 'x' coord is aligned and yields different values from slices of 2-D coord.\n",
-                "    da_2d['y', 0] + da_2d['y', 1] \n",
+                "    da_2d['y', 0] + da_2d['y', 1]\n",
                 "except RuntimeError:\n",
                 "    ok = False\n",
                 "else:\n",
                 "    ok = True\n",
                 "assert not ok"
             ]
         },
@@ -335,13 +340,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.9.18"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `scipp-24.2.0/docs/development/internals/constructing_variables.rst` & `scipp-24.5.0/docs/development/internals/constructing_variables.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/internals/customizing.rst` & `scipp-24.5.0/docs/development/internals/customizing.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/internals/multi_dimensional_indexing.rst` & `scipp-24.5.0/docs/development/internals/multi_dimensional_indexing.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/internals/transform.rst` & `scipp-24.5.0/docs/development/internals/transform.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/internals/variable_implementation.rst` & `scipp-24.5.0/docs/development/internals/variable_implementation.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/notebook-style-guide.ipynb` & `scipp-24.5.0/docs/development/notebook-style-guide.ipynb`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/project/scipp-as-cpp-or-python-library.md` & `scipp-24.5.0/docs/development/project/scipp-as-cpp-or-python-library.md`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/releasing-scipp.rst` & `scipp-24.5.0/docs/development/releasing-scipp.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/development/tooling.rst` & `scipp-24.5.0/docs/development/tooling.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/getting-started/faq.rst` & `scipp-24.5.0/docs/getting-started/faq.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/getting-started/installation.rst` & `scipp-24.5.0/docs/getting-started/installation.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. _installation:
 
 Installation
 ============
 
-Scipp requires Python 3.8 or above.
+Scipp requires Python 3.10 or above.
 
 Conda
 -----
 
 The easiest way to install Scipp is using `conda <https://docs.conda.io>`_.
 Packages from `Anaconda Cloud <https://conda.anaconda.org/scipp>`_ are available for Linux, macOS, and Windows.
 It is recommended to create an environment rather than installing individual packages.
@@ -60,39 +60,39 @@
 
 .. note::
    Installing Scipp on Windows requires ``Microsoft Visual Studio 2019 C++ Runtime`` (and versions above) installed.
    Visit https://support.microsoft.com/en-us/topic/the-latest-supported-visual-c-downloads-2647da03-1eea-4433-9aff-95f26a218cc0 for the up to date version of the library.
 
 After installation the module, Scipp can be imported in Python.
 Note that only the bare essential dependencies are installed.
-If you wish to use plotting functionality you will also need to install ``plopp`` and ``ipywidgets``.
+If you wish to use plotting functionality you will also need to install ``plopp``, ``ipympl``, and ``pythreejs``.
 
 To update or remove Scipp use `conda update <https://docs.conda.io/projects/conda/en/latest/commands/update.html>`_ and `conda remove <https://docs.conda.io/projects/conda/en/latest/commands/remove.html>`_.
 
 Pip
 ---
 
 Scipp is available from `PyPI <https://pypi.org/>`_ via ``pip``:
 
 .. code-block:: sh
 
    pip install scipp
 
 By default, this is only a minimal install without optional dependencies.
-To install components for additional submodules, use the ``all`` extras of the module:
+To install all optional dependencies, including libraries for interactive plotting in Jupyter, use:
 
 .. code-block:: sh
 
    pip install scipp[all]
 
-This will install everything that is needed, with the exception of plotting libraries for interactive use in Jupyter.
-These are available in the ``interactive`` extra.
-We recommend combining this with ``all``:
+
+You can also leave out the interactive tools and bring in only functional optional dependencies,
+such as ``h5py`` and ``scipy``, use ``extra`` instead of ``all``:
 
 .. code-block:: sh
 
-   pip install scipp[all,interactive]
+   pip install scipp[extra]
 
 From source
 -----------
 
 See the `Getting Started <../development/getting-started.rst>`_ page in the Development section.
```

### Comparing `scipp-24.2.0/docs/getting-started/overview.rst` & `scipp-24.5.0/docs/getting-started/overview.rst`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 - `Pandas <https://pandas.pydata.org/>`_ is a mature and extremely powerful package if you are mainly working with tabular 1-D data.
   Compared with Scipp it lacks support for multi-dimensional labeled data, binned data, and physical units.
 - `Xarray <https://docs.xarray.dev>`_ supports multi-dimensional labeled data similar to Scipp, but is considerably more mature.
   Compared with Scipp it lacks support for binned data and physical units.
   Experimental support for physical units using `Pint <https://pint.readthedocs.io>`_ is available with `pint-xarray <https://pint-xarray.readthedocs.io>`_.
   Xarray comes with `Dask <https://www.dask.org/>`_ support for highly scalable parallel computing.
-- `Awkward Array <https://awkward-array.readthedocs.io>`_ is a powerful package for nested, variable-sized data.
+- `Awkward Array <https://awkward-array.org>`_ is a powerful package for nested, variable-sized data.
   Its support for records is similar to Scipp's binned data.
   Compared with Scipp it lacks support for multi-dimensional labeled data and physical units.
   It may be combined with Xarray (and Pint) to achieve this, but support for multi-dimensional binning operations may be lacking.
 
 
 The data array concept
 ----------------------
```

### Comparing `scipp-24.2.0/docs/getting-started/quick-start.ipynb` & `scipp-24.5.0/docs/getting-started/quick-start.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996527777777777%*

 * *Differences: {"'cells'": '{13: {\'source\': {insert: [(0, "dataset = sc.Dataset(data={\'a\': var}, '*

 * *            'coords={\'x\': x, \'y\': y, \'aux\': x})\\n")], delete: [2, 1, 0]}}}'}*

```diff
@@ -121,17 +121,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "dataset = sc.Dataset(\n",
-                "    data={'a': var},\n",
-                "    coords={'x': x, 'y': y, 'aux': x})\n",
+                "dataset = sc.Dataset(data={'a': var}, coords={'x': x, 'y': y, 'aux': x})\n",
                 "dataset['b'] = array\n",
                 "sc.show(dataset)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `scipp-24.2.0/docs/getting-started/tutorials/from-tabular-data-to-binned-data.ipynb` & `scipp-24.5.0/docs/getting-started/tutorials/from-tabular-data-to-binned-data.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999944885361552%*

 * *Differences: {"'cells'": "{23: {'source': {insert: [(1, 'solution1 = {}\\n')], delete: [1]}}}"}*

```diff
@@ -275,15 +275,15 @@
                 "tags": [
                     "solution"
                 ]
             },
             "outputs": [],
             "source": [
                 "binned_z = table.bin(z_pos=100)\n",
-                "solution1 = dict()\n",
+                "solution1 = {}\n",
                 "solution1['histogrammed'] = table.hist(z_pos=100)\n",
                 "solution1['binned'] = binned_z.hist()\n",
                 "solution1['binned_high_resolution'] = binned_z.bin(z_pos=300).hist()\n",
                 "sc.plot(solution1)"
             ]
         },
         {
```

### Comparing `scipp-24.2.0/docs/getting-started/tutorials/prepare_data_rhessi.py` & `scipp-24.5.0/docs/getting-started/tutorials/prepare_data_rhessi.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 """
 
 from __future__ import annotations
 
 import re
 from datetime import date, datetime, time, timedelta
 from pathlib import Path
-from typing import Dict, Union
 
 import numpy as np
 import pooch
 
 import scipp as sc
 
 # IMPORTANT
@@ -72,15 +71,15 @@
     return date(day=int(day), month=parse_month(month), year=int(year))
 
 
 def parse_time(t) -> time:
     return time.fromisoformat(t)
 
 
-def parse_datetimes(d, start, peak, end) -> Dict[str, Union[np.datetime64, int]]:
+def parse_datetimes(d, start, peak, end) -> dict[str, np.datetime64 | int]:
     d = parse_date(d)
     start = parse_time(start)
     peak = parse_time(peak)
     end = parse_time(end)
 
     start_datetime = datetime.combine(d, start)
     peak_date = d + timedelta(days=1) if peak < start else d
@@ -211,15 +210,15 @@
             "quality": event_array("quality", None),
             **{key: event_array(key, None) for key in list(values)},
             "description": sc.scalar(
                 "X-ray flares recorded by NASA's Reuven Ramaty High Energy Solar"
                 " Spectroscopic Imager (RHESSI) Small Explorer"
             ),
             "url": sc.scalar(
-                "https://hesperia.gsfc.nasa.gov/rhessi3/data-access/rhessi-data/flare-list/index.html"  # noqa
+                "https://hesperia.gsfc.nasa.gov/rhessi3/data-access/rhessi-data/flare-list/index.html"
             ),
             "citation": sc.scalar("https://doi.org/10.1023/A:1022428818870"),
         },
     )
 
 
 def prefilter(da):
@@ -233,29 +232,26 @@
     # only high quality
     da = da[da.attrs["quality"] < sc.index(3)]
     del da.attrs["quality"]
     # PS - Possible Solar Flare; in front detectors, but no position
     da = da[~da.attrs.pop("PS")]
 
     for flag in FLAGS:
-        try:
-            del da.attrs[flag]
-        except KeyError:
-            pass
+        da.attrs.pop(flag, None)
     return da
 
 
 def remove_events(da, rng):
     """
     Define fictitious efficiencies for the different collimators of the detector.
     Uses a 3x3 detector grid with arbitrarily chosen apertures.
     Events are removed randomly based on the efficiencies such that the data
     can be normalised using `events / efficiency`.
     """
-    print("removing events based on detector efficiency")
+    print("removing events based on detector efficiency")  # noqa: T201
     collimator_x = sc.array(
         dims=["x"], values=[-1000, -300, 300, 1000], unit="asec", dtype="float64"
     )
     collimator_y = sc.array(
         dims=["y"], values=[-600, -200, 200, 600], unit="asec", dtype="float64"
     )
     efficiency = sc.DataArray(
```

### Comparing `scipp-24.2.0/docs/getting-started/tutorials/solar_flares.ipynb` & `scipp-24.5.0/docs/getting-started/tutorials/solar_flares.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999740362246594%*

 * *Differences: {"'cells'": '{89: {\'source\': {insert: [(2, \'\\n\'), (9, "    aspect=\'equal\',\\n"), (10, "    '*

 * *            'cmap=\'magma\',\\n"), (11, "    norm=\'log\',\\n")], delete: [8]}}}'}*

```diff
@@ -1138,21 +1138,24 @@
             "execution_count": null,
             "id": "1ec0b5a7-ede2-4bdf-b638-708187c5e50a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
                 "import plopp as pp\n",
+                "\n",
                 "temporal_and_spatial = spatial.bin(peak_time=10)\n",
                 "p = pp.slicer(\n",
                 "    temporal_and_spatial.hist(),\n",
                 "    keep=['y', 'x'],\n",
                 "    vmin=sc.scalar(1),\n",
                 "    autoscale='fixed',\n",
-                "    aspect='equal', cmap='magma', norm='log',\n",
+                "    aspect='equal',\n",
+                "    cmap='magma',\n",
+                "    norm='log',\n",
                 ")\n",
                 "p[0].canvas.xlabel = 'x [asec]'\n",
                 "p[0].canvas.ylabel = 'y [asec]'\n",
                 "p"
             ]
         },
         {
```

### Comparing `scipp-24.2.0/docs/images/multi_dimensional_indexing/multi_index_binned_1d_setups.svg` & `scipp-24.5.0/docs/images/multi_dimensional_indexing/multi_index_binned_1d_setups.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/multi_dimensional_indexing/multi_index_binned_2d_setups.svg` & `scipp-24.5.0/docs/images/multi_dimensional_indexing/multi_index_binned_2d_setups.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/multi_dimensional_indexing/multi_index_dense_setups.svg` & `scipp-24.5.0/docs/images/multi_dimensional_indexing/multi_index_dense_setups.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/multi_dimensional_indexing/view_index_delta.svg` & `scipp-24.5.0/docs/images/multi_dimensional_indexing/view_index_delta.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/multi_dimensional_indexing/view_index_flattening.svg` & `scipp-24.5.0/docs/images/multi_dimensional_indexing/view_index_flattening.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/multi_dimensional_indexing/view_index_increment_full.svg` & `scipp-24.5.0/docs/images/multi_dimensional_indexing/view_index_increment_full.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/multi_dimensional_indexing/view_index_increment_partial.svg` & `scipp-24.5.0/docs/images/multi_dimensional_indexing/view_index_increment_partial.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/plotting-1d-keep-event.png` & `scipp-24.5.0/docs/images/plotting-1d-keep-event.png`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/plotting-1d-pick-event.png` & `scipp-24.5.0/docs/images/plotting-1d-pick-event.png`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/plotting-1d-slider-event.png` & `scipp-24.5.0/docs/images/plotting-1d-slider-event.png`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/plotting-2d-slider-event.png` & `scipp-24.5.0/docs/images/plotting-2d-slider-event.png`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/transform_coords/base_rules.svg` & `scipp-24.5.0/docs/images/transform_coords/base_rules.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/transform_coords/cycle-contraction.svg` & `scipp-24.5.0/docs/images/transform_coords/cycle-contraction.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/transform_coords/cycle.svg` & `scipp-24.5.0/docs/images/transform_coords/cycle.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/transform_coords/cycle_rules.svg` & `scipp-24.5.0/docs/images/transform_coords/cycle_rules.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/transform_coords/fractional-colors.svg` & `scipp-24.5.0/docs/images/transform_coords/fractional-colors.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/transform_coords/larger_examples.svg` & `scipp-24.5.0/docs/images/transform_coords/larger_examples.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/transform_coords/slice-transform-concat.svg` & `scipp-24.5.0/docs/images/transform_coords/slice-transform-concat.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/transform_coords/split-join.svg` & `scipp-24.5.0/docs/images/transform_coords/split-join.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/variable_classes.dia` & `scipp-24.5.0/docs/images/variable_classes.dia`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/images/variable_classes.svg` & `scipp-24.5.0/docs/images/variable_classes.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/index.rst` & `scipp-24.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/reference/classes.rst` & `scipp-24.5.0/docs/reference/classes.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/reference/dtype.ipynb` & `scipp-24.5.0/docs/reference/dtype.ipynb`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/reference/error-propagation.rst` & `scipp-24.5.0/docs/reference/error-propagation.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/reference/free-functions.rst` & `scipp-24.5.0/docs/reference/free-functions.rst`

 * *Files 3% similar despite different names*

```diff
@@ -164,23 +164,14 @@
    sinh
    cosh
    tanh
    asinh
    acosh
    atanh
 
-Geometric
-~~~~~~~~~
-
-.. autosummary::
-   :toctree: ../generated/functions
-
-   geometry.position
-   geometry.rotation_matrix_from_quaternion_coeffs
-
 Group-by (split-apply-combine)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Reduction
 ---------
 
 .. autosummary::
```

### Comparing `scipp-24.2.0/docs/reference/linear-algebra.ipynb` & `scipp-24.5.0/docs/reference/linear-algebra.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988432188953023%*

 * *Differences: {"'cells'": '{11: {\'source\': {insert: [(5, "    data=sc.array(dims=[\'x\', \'y\'], '*

 * *            'values=np.random.rand(nx, ny)),\\n"), (6, "    coords={\'position\': '*

 * *            'sc.spatial.as_vectors(x, y, 0.0 * sc.units.m)},\\n")], delete: [6, 5]}}, 13: '*

 * *            '{\'source\': {insert: [(0, "sensor.coords[\'position\'][\'x\', 5:].fields.x += 0.1 * '*

 * *            'sc.units.m\\n"), (1, "sensor.coords[\'position\'][\'y\', 5:].fields.y += 0.05 * '*

 * *            'sc.units.m\\n")], delete: [1, 0]}}, 15: { […]*

```diff
@@ -135,16 +135,16 @@
             "outputs": [],
             "source": [
                 "nx = 12\n",
                 "ny = 12\n",
                 "x = sc.linspace(dim='x', start=-0.1, stop=0.1, num=nx, unit='m')\n",
                 "y = sc.linspace(dim='y', start=-0.1, stop=0.1, num=ny, unit='m')\n",
                 "sensor = sc.DataArray(\n",
-                "    data=sc.array(dims=['x','y'], values=np.random.rand(nx, ny)),\n",
-                "    coords={'position':sc.geometry.position(x, y, 0.0*sc.units.m)}\n",
+                "    data=sc.array(dims=['x', 'y'], values=np.random.rand(nx, ny)),\n",
+                "    coords={'position': sc.spatial.as_vectors(x, y, 0.0 * sc.units.m)},\n",
                 ")\n",
                 "pp.scatter3d(sensor, pos=\"position\", pixel_size=0.01)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1d852b52-613c-4168-88f2-1de4340c77b8",
@@ -156,16 +156,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "207e32b8-3e7f-4a79-8821-e9bdefe48e98",
             "metadata": {},
             "outputs": [],
             "source": [
-                "sensor.coords['position']['x',5:].fields.x += 0.1 * sc.units.m\n",
-                "sensor.coords['position']['y',5:].fields.y += 0.05 * sc.units.m\n",
+                "sensor.coords['position']['x', 5:].fields.x += 0.1 * sc.units.m\n",
+                "sensor.coords['position']['y', 5:].fields.y += 0.05 * sc.units.m\n",
                 "\n",
                 "pp.scatter3d(sensor, pos=\"position\", pixel_size=0.01)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "bbf54580-29d3-40bb-96bd-a93f3ff4c26f",
@@ -177,19 +177,23 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "83fe9f32-26cc-43d0-b6fa-ae761f09b221",
             "metadata": {},
             "outputs": [],
             "source": [
-                "rotation = sc.spatial.linear_transform(value=[[ 0.8660254, 0.0000000, 0.5000000],\n",
-                "                            [ 0.0000000, 1.0000000, 0.0000000],\n",
-                "                            [-0.5000000, 0.0000000, 0.8660254]])\n",
+                "rotation = sc.spatial.linear_transform(\n",
+                "    value=[\n",
+                "        [0.8660254, 0.0000000, 0.5000000],\n",
+                "        [0.0000000, 1.0000000, 0.0000000],\n",
+                "        [-0.5000000, 0.0000000, 0.8660254],\n",
+                "    ]\n",
+                ")\n",
                 "\n",
-                "sensor.coords['position']['x',5:] = rotation * sensor.coords['position']['x',5:]\n",
+                "sensor.coords['position']['x', 5:] = rotation * sensor.coords['position']['x', 5:]\n",
                 "pp.scatter3d(sensor, pos=\"position\", pixel_size=0.01)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0b6b58d4-6b8d-4d12-a885-41eb0cec192d",
             "metadata": {},
@@ -203,16 +207,19 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "6784591d-fa75-4da9-a5ef-52ca9e3ae222",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from scipp.spatial import rotations_from_rotvecs\n",
-                "rotation_back = rotations_from_rotvecs(rotation_vectors=sc.vector(value=[0, -30.0, 0], unit=sc.units.deg))\n",
-                "sensor.coords['position']['x',5:] = rotation_back * sensor.coords['position']['x',5:]\n",
+                "\n",
+                "rotation_back = rotations_from_rotvecs(\n",
+                "    rotation_vectors=sc.vector(value=[0, -30.0, 0], unit=sc.units.deg)\n",
+                ")\n",
+                "sensor.coords['position']['x', 5:] = rotation_back * sensor.coords['position']['x', 5:]\n",
                 "pp.scatter3d(sensor, pos=\"position\", pixel_size=0.01)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f7296c82-a193-48c3-9b4d-c4339403be85",
             "metadata": {},
```

### Comparing `scipp-24.2.0/docs/reference/logging.ipynb` & `scipp-24.5.0/docs/reference/logging.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986293859649122%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, '\\n')]}}, 5: {'source': {insert: [(1, '\\n')]}}, 15: "*

 * *            '{\'source\': ["logger.info(\'The HTML representation of a Variable: %s\', '*

 * *            'sc.arange(\'h\', 10, 15))"]}, 17: {\'source\': ["logger.info(\'A Variable converted '*

 * *            'to string: %r\', sc.arange(\'r\', 100, 105))"]}}'}*

```diff
@@ -21,14 +21,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "6fe5c6cf-0260-45c0-a525-48af9905429b",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import scipp as sc\n",
+                "\n",
                 "logger = sc.get_logger()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ed3fcbae-1a9e-492e-96fd-b46883d48483",
             "metadata": {},
@@ -58,14 +59,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "1456dece-9774-4aac-bea1-3b6baa872b99",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import logging\n",
+                "\n",
                 "stream_handler = logging.StreamHandler()\n",
                 "stream_handler.setLevel(logging.INFO)\n",
                 "logger.addHandler(stream_handler)\n",
                 "logger.setLevel(logging.INFO)"
             ]
         },
         {
@@ -180,16 +182,15 @@
             "metadata": {
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
             "source": [
-                "logger.info('The HTML representation of a Variable: %s',\n",
-                "            sc.arange('h', 10, 15))"
+                "logger.info('The HTML representation of a Variable: %s', sc.arange('h', 10, 15))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f575a862-a2e5-48c0-baf9-b01ba506f584",
             "metadata": {},
             "source": [
@@ -199,16 +200,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2a4ac578-7b9e-4882-b58f-aaa45e9fedbb",
             "metadata": {},
             "outputs": [],
             "source": [
-                "logger.info('A Variable converted to string: %r', \n",
-                "            sc.arange('r', 100, 105))"
+                "logger.info('A Variable converted to string: %r', sc.arange('r', 100, 105))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b1884cd9",
             "metadata": {},
             "source": [
```

### Comparing `scipp-24.2.0/docs/reference/modules.rst` & `scipp-24.5.0/docs/reference/modules.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/reference/ownership-mechanism-and-readonly-flags.ipynb` & `scipp-24.5.0/docs/reference/ownership-mechanism-and-readonly-flags.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994724893162393%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, '\\n')]}}, 16: {'source': {insert: [(0, "*

 * *            '"ds[\'a\'].masks[\'m\'] = da.coords[\'x\'] < 670 * sc.Unit(\'m\')\\n")], delete: '*

 * *            "[0]}}, 18: {'source': {insert: [(1, '# the coords *dict* is copied,\\n')], delete: "*

 * *            '[1]}}}'}*

```diff
@@ -26,14 +26,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "11645e21-4977-4796-8e24-a5eff607adeb",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import scipp as sc\n",
+                "\n",
                 "var = sc.arange(dim='x', unit='m', start=0, stop=12)\n",
                 "var['x', 4:6]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4964a047-7428-4bfc-8133-ad97ac201b5e",
@@ -180,15 +181,15 @@
             "execution_count": null,
             "id": "b5a3bcd2-314d-40e7-90f5-8668de91a437",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "ds['a'].masks['m'] = (da.coords['x'] < 670 * sc.Unit('m'))\n",
+                "ds['a'].masks['m'] = da.coords['x'] < 670 * sc.Unit('m')\n",
                 "'m' in da.masks  # the masks *dict* is copied"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e6f2a020-2438-447d-a64d-a641eb0469e2",
             "metadata": {},
@@ -202,15 +203,15 @@
             "id": "918c4cbf-130d-4c9f-a644-16d9a6a82244",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "da.coords['x'] *= -1\n",
-                "# the coords *dict* is copied, \n",
+                "# the coords *dict* is copied,\n",
                 "# but the 'x' coordinate references same buffer\n",
                 "ds.coords['x']"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b6051d12-a1c0-4a4f-8a0c-c10c83fa3398",
```

### Comparing `scipp-24.2.0/docs/reference/testing.rst` & `scipp-24.5.0/docs/reference/testing.rst`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/reference/units.ipynb` & `scipp-24.5.0/docs/reference/units.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996078431372549%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(0, 'also_volume = length**3\\n')], delete: [0]}}, 40: "*

 * *            '{\'source\': [\'print(\\n\', "    sc.Unit(\'mm\'),\\n", "    '*

 * *            'sc.Unit(\'microsecond\'),\\n", "    sc.Unit(\'micro s\'),\\n", "    '*

 * *            'sc.Unit(\'us\'),\\n", "    sc.Unit(\'MJ\'),\\n", \')\']}, 42: {\'source\': '*

 * *            '["print(sc.Unit(\'m^2\'), sc.Unit(\'m**2\'), sc.Unit(\'m\') ** 2)"]}}'}*

```diff
@@ -56,15 +56,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "also_volume = length ** 3\n",
+                "also_volume = length**3\n",
                 "also_volume"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -443,16 +443,21 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(sc.Unit('mm'), sc.Unit('microsecond'),\n",
-                "      sc.Unit('micro s'), sc.Unit('us'), sc.Unit('MJ'))"
+                "print(\n",
+                "    sc.Unit('mm'),\n",
+                "    sc.Unit('microsecond'),\n",
+                "    sc.Unit('micro s'),\n",
+                "    sc.Unit('us'),\n",
+                "    sc.Unit('MJ'),\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "You can also specify exponents for units or exponentiate the `Unit` object:"
@@ -460,15 +465,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(sc.Unit('m^2'), sc.Unit('m**2'), sc.Unit('m')**2)"
+                "print(sc.Unit('m^2'), sc.Unit('m**2'), sc.Unit('m') ** 2)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Conversion Between Units of Different Scales\n",
```

### Comparing `scipp-24.2.0/docs/user-guide/binned-data/binned-data.ipynb` & `scipp-24.5.0/docs/user-guide/binned-data/binned-data.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992235999129382%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(5, 'np.random.seed(1)  # Fixed for reproducibility')], "*

 * *            "delete: [5]}}, 3: {'source': {insert: [(1, 'values = 10 * np.random.rand(N)\\n'), (5, "*

 * *            '"        \'position\': sc.array(\\n"), (6, "            dims=[\'row\'], '*

 * *            'values=[f\'site-{i}\' for i in range(N)]\\n"), (7, \'        ),\\n\'), (8, "        '*

 * *            '\'x\': sc.array(dims=[\'row\'], unit=\'m\', values=np.random.rand(N)),\\n"), (9, '*

 * *            '"        \'y\': sc.a […]*

```diff
@@ -46,15 +46,15 @@
             "outputs": [],
             "source": [
                 "%matplotlib inline\n",
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "import scipp as sc\n",
                 "\n",
-                "np.random.seed(1) # Fixed for reproducibility"
+                "np.random.seed(1)  # Fixed for reproducibility"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Consider a list of measurements at various \"points\" in space.\n",
@@ -64,21 +64,25 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "N = 50\n",
-                "values = 10*np.random.rand(N)\n",
+                "values = 10 * np.random.rand(N)\n",
                 "table = sc.DataArray(\n",
                 "    data=sc.array(dims=['row'], unit=sc.units.counts, values=values, variances=values),\n",
                 "    coords={\n",
-                "        'position':sc.array(dims=['row'], values=['site-{}'.format(i) for i in range(N)]),\n",
-                "        'x':sc.array(dims=['row'], unit='m', values=np.random.rand(N)),\n",
-                "        'y':sc.array(dims=['row'], unit='m', values=np.random.rand(N))})\n",
+                "        'position': sc.array(\n",
+                "            dims=['row'], values=[f'site-{i}' for i in range(N)]\n",
+                "        ),\n",
+                "        'x': sc.array(dims=['row'], unit='m', values=np.random.rand(N)),\n",
+                "        'y': sc.array(dims=['row'], unit='m', values=np.random.rand(N)),\n",
+                "    },\n",
+                ")\n",
                 "table"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -127,21 +131,20 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "fig, ax = plt.subplots(dpi=96)\n",
                 "scatter = ax.scatter(\n",
-                "    x=table.coords['x'].values,\n",
-                "    y=table.coords['y'].values,\n",
-                "    c=table.values)\n",
+                "    x=table.coords['x'].values, y=table.coords['y'].values, c=table.values\n",
+                ")\n",
                 "ax.set_xlabel('x [{}]'.format(table.coords['x'].unit))\n",
                 "ax.set_ylabel('y [{}]'.format(table.coords['y'].unit))\n",
                 "cbar = plt.colorbar(scatter)\n",
-                "cbar.set_label(\"[{}]\".format(table.unit))"
+                "cbar.set_label(f\"[{table.unit}]\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This shows the distribution in space, but for real datasets with millions of points this is not practical.\n",
@@ -192,24 +195,23 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "fig, ax = plt.subplots(dpi=96)\n",
                 "buffer = binned.bins.constituents['data']\n",
                 "scatter = ax.scatter(\n",
-                "    x=buffer.coords['x'].values,\n",
-                "    y=buffer.coords['y'].values,\n",
-                "    c=buffer.values)\n",
+                "    x=buffer.coords['x'].values, y=buffer.coords['y'].values, c=buffer.values\n",
+                ")\n",
                 "ax.set_xlabel('x [{}]'.format(binned.coords['x'].unit))\n",
                 "ax.set_ylabel('y [{}]'.format(binned.coords['y'].unit))\n",
                 "ax.set_xticks(binned.coords['x'].values)\n",
                 "ax.set_yticks(binned.coords['y'].values)\n",
                 "ax.grid()\n",
                 "cbar = fig.colorbar(scatter)\n",
-                "cbar.set_label(\"[{}]\".format(table.unit))"
+                "cbar.set_label(f\"[{table.unit}]\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This is essentially the same figure as the scatter plot for the original `data`.\n",
@@ -390,15 +392,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "da = table.bin(y=4, x=2)\n",
                 "del da.coords['y']\n",
                 "del da.bins.coords['y']\n",
-                "da = da.rename_dims({'y':'time'})\n",
+                "da = da.rename_dims({'y': 'time'})\n",
                 "da.coords['time'] = sc.arange('time', 4, unit='s')\n",
                 "da"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `scipp-24.2.0/docs/user-guide/binned-data/computation.ipynb` & `scipp-24.5.0/docs/user-guide/binned-data/computation.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984934041184041%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(3, \'table = sc.array(\\n\'), (4, "    dims=[\'event\'], '*

 * *            'values=[0, 1, 3, 1, 1, 1, 42, 1, 1, 1, 1, 1], dtype=\'float64\'\\n"), (5, \')\\n\')], '*

 * *            'delete: [3]}}, 5: {\'source\': {insert: [(0, "begin = sc.array(dims=[\'x\'], '*

 * *            'values=[0, 6, 6, 8], unit=None)\\n"), (1, "end = sc.array(dims=[\'x\'], values=[6, 6, '*

 * *            '8, 12], unit=None)\\n")], delete: [1, 0]}}, 15: {\'source\': {insert: [(0, \'times = '*

 * *            'sc.ar […]*

```diff
@@ -62,15 +62,17 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import scipp as sc\n",
                 "\n",
-                "table = sc.array(dims=['event'], values=[0,1,3,1,1,1,42,1,1,1,1,1], dtype='float64')\n",
+                "table = sc.array(\n",
+                "    dims=['event'], values=[0, 1, 3, 1, 1, 1, 42, 1, 1, 1, 1, 1], dtype='float64'\n",
+                ")\n",
                 "sc.table(table)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -79,16 +81,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "begin = sc.array(dims=['x'], values=[0,6,6,8], unit=None)\n",
-                "end = sc.array(dims=['x'], values=[6,6,8,12], unit=None)\n",
+                "begin = sc.array(dims=['x'], values=[0, 6, 6, 8], unit=None)\n",
+                "end = sc.array(dims=['x'], values=[6, 6, 8, 12], unit=None)\n",
                 "var = sc.bins(begin=begin, end=end, dim='event', data=table)\n",
                 "sc.show(var)\n",
                 "var"
             ]
         },
         {
             "cell_type": "markdown",
@@ -176,21 +178,23 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "times = sc.array(dims=['event'],\n",
-                "                 unit='us', # micro second\n",
-                "                 values=[0,1,3,1,1,1,4,1,1,2,1,1],\n",
-                "                 dtype='float64')\n",
+                "times = sc.array(\n",
+                "    dims=['event'],\n",
+                "    unit='us',  # micro second\n",
+                "    values=[0, 1, 3, 1, 1, 1, 4, 1, 1, 2, 1, 1],\n",
+                "    dtype='float64',\n",
+                ")\n",
                 "weights = sc.ones(dims=['event'], unit='counts', shape=[12], with_variances=True)\n",
                 "\n",
-                "table = sc.DataArray(data=weights, coords={'time':times})\n",
+                "table = sc.DataArray(data=weights, coords={'time': times})\n",
                 "sc.table(table)\n",
                 "table"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -202,15 +206,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "var = sc.bins(begin=begin, end=end, dim='event', data=table)\n",
-                "a = sc.DataArray(data=var, coords={'x':sc.Variable(dims=['x'], values=np.arange(4.0))})\n",
+                "a = sc.DataArray(data=var, coords={'x': sc.Variable(dims=['x'], values=np.arange(4.0))})\n",
                 "a"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -322,17 +326,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "sc.show(a['x',2].value)\n",
+                "sc.show(a['x', 2].value)\n",
                 "a.bins.concatenate(a, out=a)\n",
-                "sc.show(a['x',2].value)\n",
+                "sc.show(a['x', 2].value)\n",
                 "a.bins.sum().plot()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -342,17 +346,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "zero = a.copy()\n",
-                "sc.show(zero['x',2].value)\n",
+                "sc.show(zero['x', 2].value)\n",
                 "zero.bins.concatenate(-zero, out=zero)\n",
-                "sc.show(zero['x',2].value)\n",
+                "sc.show(zero['x', 2].value)\n",
                 "zero.bins.sum().plot()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -365,15 +369,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "time_bins = sc.array(dims=['time'], unit=sc.units.us, values=[0.0, 3.0, 6.0])\n",
                 "weight = sc.array(dims=['time'], values=[10.0, 3.0])\n",
-                "hist = sc.DataArray(data=weight, coords={'time':time_bins})\n",
+                "hist = sc.DataArray(data=weight, coords={'time': time_bins})\n",
                 "hist"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -406,15 +410,15 @@
                 "tags": [
                     "raises-exception"
                 ]
             },
             "outputs": [],
             "source": [
                 "weight = sc.array(dims=['time'], values=[10.0, 3.0], variances=[10.0, 3.0])\n",
-                "hist = sc.DataArray(data=weight, coords={'time':time_bins})\n",
+                "hist = sc.DataArray(data=weight, coords={'time': time_bins})\n",
                 "a.bins /= sc.lookup(func=hist, dim='time')"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
```

### Comparing `scipp-24.2.0/docs/user-guide/binned-data/filtering.ipynb` & `scipp-24.5.0/docs/user-guide/binned-data/filtering.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988591269841269%*

 * *Differences: {"'cells'": '{17: {\'source\': {insert: [(0, "da = '*

 * *            "da.transform_coords(good_pulse=good_pulse).bins['good_pulse', "*

 * *            'sc.index(True)]\\n")], delete: [1, 0]}}, 19: {\'source\': {insert: [(1, \'filtered = '*

 * *            "da.transform_coords(strain=interpolate_strain).bin(strain=100)')], delete: [2, 1]}}, "*

 * *            "23: {'source': {insert: [(3, 'charge_per_strain_value = "*

 * *            'charge_per_time_interval.bin(\\n\'), (4, "    '*

 * *            'strain=filtered.coords[\'strain\']\\n […]*

```diff
@@ -280,16 +280,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "da = da.transform_coords(good_pulse=good_pulse) \\\n",
-                "       .bins['good_pulse', sc.index(True)]\n",
+                "da = da.transform_coords(good_pulse=good_pulse).bins['good_pulse', sc.index(True)]\n",
                 "da"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -301,16 +300,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "interpolate_strain = sc.lookup(strain, mode='previous')\n",
-                "filtered = da.transform_coords(strain=interpolate_strain) \\\n",
-                "             .bin(strain=100)"
+                "filtered = da.transform_coords(strain=interpolate_strain).bin(strain=100)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We can histogram and plot the result, but the figure is not very illuminating.\n",
@@ -343,15 +341,17 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "proton_charge = dg['proton_charge']\n",
                 "charge_per_time_interval = proton_charge.bin(time=strain.coords['time'])\n",
                 "charge_per_time_interval.coords['strain'] = strain.data\n",
-                "charge_per_strain_value = charge_per_time_interval.bin(strain=filtered.coords['strain']).hist()"
+                "charge_per_strain_value = charge_per_time_interval.bin(\n",
+                "    strain=filtered.coords['strain']\n",
+                ").hist()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We can then normalize our data and obtain a more meaningful plot.\n",
@@ -360,15 +360,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "normalized = (filtered/charge_per_strain_value)\n",
+                "normalized = filtered / charge_per_strain_value\n",
                 "normalized.hist(strain=30, dspacing=300).plot()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `scipp-24.2.0/docs/user-guide/binned-data/histogramming-grouping-and-binning.ipynb` & `scipp-24.5.0/docs/user-guide/binned-data/histogramming-grouping-and-binning.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996232057416268%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, '\\n'), (4, 'values = 10 * np.random.rand(N)\\n'), (6, "*

 * *            '\'    data=sc.array(\\n\'), (7, "        dims=[\'position\'], unit=sc.units.counts, '*

 * *            'values=values, variances=values\\n"), (8, \'    ),\\n\'), (10, "        \'x\': '*

 * *            'sc.array(dims=[\'position\'], unit=\'m\', values=np.random.rand(N)),\\n"), (11, '*

 * *            '"        \'y\': sc.array(dims=[\'position\'], unit=\'m\', '*

 * *            'values=np.random.rand(N)),\\n"), (12, \ […]*

```diff
@@ -18,23 +18,27 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import scipp as sc\n",
+                "\n",
                 "N = 5000\n",
-                "values = 10*np.random.rand(N)\n",
+                "values = 10 * np.random.rand(N)\n",
                 "table = sc.DataArray(\n",
-                "    data=sc.array(dims=['position'], unit=sc.units.counts, values=values, variances=values),\n",
+                "    data=sc.array(\n",
+                "        dims=['position'], unit=sc.units.counts, values=values, variances=values\n",
+                "    ),\n",
                 "    coords={\n",
-                "        'x':sc.array(dims=['position'], unit='m', values=np.random.rand(N)),\n",
-                "        'y':sc.array(dims=['position'], unit='m', values=np.random.rand(N))\n",
-                "    })\n",
-                "table.values *= 1.0/np.exp(5.0*table.coords['x'].values)\n",
+                "        'x': sc.array(dims=['position'], unit='m', values=np.random.rand(N)),\n",
+                "        'y': sc.array(dims=['position'], unit='m', values=np.random.rand(N)),\n",
+                "    },\n",
+                ")\n",
+                "table.values *= 1.0 / np.exp(5.0 * table.coords['x'].values)\n",
                 "sc.table(table['position', :5])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -47,19 +51,21 @@
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "xbins = sc.linspace('x', 0, 1, num=40, unit='m')\n",
-                "ds = sc.Dataset({\n",
-                "    'histogram': table.hist(x=xbins),\n",
-                "    'groupby': table.groupby('x', bins=xbins).sum('position'),\n",
-                "    'bin': table.bin(x=xbins).bins.sum(),\n",
-                "})\n",
+                "ds = sc.Dataset(\n",
+                "    {\n",
+                "        'histogram': table.hist(x=xbins),\n",
+                "        'groupby': table.groupby('x', bins=xbins).sum('position'),\n",
+                "        'bin': table.bin(x=xbins).bins.sum(),\n",
+                "    }\n",
+                ")\n",
                 "ds.plot()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -150,16 +156,18 @@
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "binned = table.bin(x=xbins)\n",
-                "binned.coords['param'] = sc.array(dims=['x'], values=(np.random.random(39)*4).astype(np.int32))\n",
-                "grouped = binned.groupby('param').bins.concat('x')\n",
+                "binned.coords['param'] = sc.array(\n",
+                "    dims=['x'], values=(np.random.random(39) * 4).astype(np.int32)\n",
+                ")\n",
+                "grouped = binned.groupby('param').concat('x')\n",
                 "grouped"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -256,13 +264,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.10.14"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `scipp-24.2.0/docs/user-guide/binned-data/prepare-filtering-data.py` & `scipp-24.5.0/docs/user-guide/binned-data/prepare-filtering-data.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/user-guide/computation.ipynb` & `scipp-24.5.0/docs/user-guide/computation.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984629319955407%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(0, 'result = a / b\\n')], delete: [0]}}, 4: {'source': "*

 * *            "['a.values / np.transpose(b.values)']}, 6: {'source': ['a.variances / "*

 * *            'np.transpose(b.variances)\']}, 10: {\'source\': {insert: [(0, "var_xy = '*

 * *            'sc.array(dims=[\'x\', \'y\'], values=np.arange(6).reshape((2, 3)))\\n")], delete: '*

 * *            '[0]}}, 21: {\'source\': {insert: [(1, \'    data={\\n\'), (2, "        \'a\': '*

 * *            'sc.array(dims=[\'x\', \'y\'], values=rng. […]*

```diff
@@ -55,25 +55,25 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "result = a/b\n",
+                "result = a / b\n",
                 "result.values"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "a.values/np.transpose(b.values)"
+                "a.values / np.transpose(b.values)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -83,15 +83,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "a.variances/np.transpose(b.variances)"
+                "a.variances / np.transpose(b.variances)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The implementation assumes uncorrelated data and is otherwise based on, e.g., [Wikipedia: Propagation of uncertainty](https://en.wikipedia.org/wiki/Propagation_of_uncertainty#Example_formulae).\n",
@@ -126,15 +126,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "var_xy = sc.array(dims=['x', 'y'], values=np.arange(6).reshape((2,3)))\n",
+                "var_xy = sc.array(dims=['x', 'y'], values=np.arange(6).reshape((2, 3)))\n",
                 "print(var_xy.values)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -249,26 +249,28 @@
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "d1 = sc.Dataset(\n",
-                "    data={'a': sc.array(dims=['x', 'y'], values=rng.random((2, 3))),\n",
-                "          'b': sc.array(dims=['y', 'x'], values=rng.random((3, 2))),\n",
-                "          'c': sc.array(dims=['x', 'y'], values=rng.random((2, 3)))},\n",
-                "    coords={\n",
-                "        'x': sc.arange('x', 2.0, unit='m'),\n",
-                "        'y': sc.arange('y', 3.0, unit='m')})\n",
+                "    data={\n",
+                "        'a': sc.array(dims=['x', 'y'], values=rng.random((2, 3))),\n",
+                "        'b': sc.array(dims=['y', 'x'], values=rng.random((3, 2))),\n",
+                "        'c': sc.array(dims=['x', 'y'], values=rng.random((2, 3))),\n",
+                "    },\n",
+                "    coords={'x': sc.arange('x', 2.0, unit='m'), 'y': sc.arange('y', 3.0, unit='m')},\n",
+                ")\n",
                 "d2 = sc.Dataset(\n",
-                "    data={'a': sc.array(dims=['x', 'y'], values=rng.random((2, 3))),\n",
-                "          'b': sc.array(dims=['y', 'x'], values=rng.random((3, 2)))},\n",
-                "    coords={\n",
-                "        'x': sc.arange('x', 2.0, unit='m'),\n",
-                "        'y': sc.arange('y', 3.0, unit='m')})"
+                "    data={\n",
+                "        'a': sc.array(dims=['x', 'y'], values=rng.random((2, 3))),\n",
+                "        'b': sc.array(dims=['y', 'x'], values=rng.random((3, 2))),\n",
+                "    },\n",
+                "    coords={'x': sc.arange('x', 2.0, unit='m'), 'y': sc.arange('y', 3.0, unit='m')},\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
@@ -343,18 +345,21 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "da1 = sc.DataArray(sc.arange('x', 8).fold('x', {'x': 4, 'y': 2}),\n",
-                "                   coords={'x': sc.arange('x', 4), 'y': sc.arange('y', 2)})\n",
-                "da2 = sc.DataArray(sc.arange('x', 4),\n",
-                "                   coords={'x': 10*sc.arange('x', 4), 'y': sc.arange('y', 2)})"
+                "da1 = sc.DataArray(\n",
+                "    sc.arange('x', 8).fold('x', {'x': 4, 'y': 2}),\n",
+                "    coords={'x': sc.arange('x', 4), 'y': sc.arange('y', 2)},\n",
+                ")\n",
+                "da2 = sc.DataArray(\n",
+                "    sc.arange('x', 4), coords={'x': 10 * sc.arange('x', 4), 'y': sc.arange('y', 2)}\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
@@ -510,16 +515,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "rad = 3.141593*sc.units.rad\n",
-                "deg = 180.0*sc.units.deg\n",
+                "rad = 3.141593 * sc.units.rad\n",
+                "deg = 180.0 * sc.units.deg\n",
                 "print(sc.sin(rad))\n",
                 "print(sc.sin(deg))\n",
                 "try:\n",
                 "    rad + deg\n",
                 "except Exception as e:\n",
                 "    print(str(e))"
             ]
```

### Comparing `scipp-24.2.0/docs/user-guide/coordinate-transformations.ipynb` & `scipp-24.5.0/docs/user-guide/coordinate-transformations.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998039874551972%*

 * *Differences: {"'cells'": '{13: {\'source\': {insert: [(17, "    seconds_per_day = sc.scalar(24 * 60 * 60, '*

 * *            'unit=\'s\')\\n")], delete: [17]}}, 27: {\'source\': {insert: [(2, "binned = '*

 * *            "sc.bin(transformed.flatten(to='dummy'), latitude=latitude, "*

 * *            'local_time=time_edges)")], delete: [2]}}}'}*

```diff
@@ -203,15 +203,15 @@
                 "    long = sc.to_unit(longitude, unit='deg', copy=False)\n",
                 "    angular_velocity = (360.0 * sc.Unit('deg')) / (24.0 * sc.Unit('hour'))\n",
                 "    offset = (long / angular_velocity).astype('int64') + 12 * sc.Unit('hour')\n",
                 "    return sc.to_unit(offset, datetime.unit) + datetime\n",
                 "\n",
                 "\n",
                 "def time(local_datetime):\n",
-                "    seconds_per_day = sc.scalar(24 * 60 * 60, unit='s/D')\n",
+                "    seconds_per_day = sc.scalar(24 * 60 * 60, unit='s')\n",
                 "    start_day = sc.scalar(start.value.astype('datetime64[D]'))\n",
                 "    start_day_in_seconds = sc.scalar(start_day.values.astype('datetime64[s]'))\n",
                 "    offset = local_datetime - start_day_in_seconds\n",
                 "    time = (offset % seconds_per_day).astype('float64')\n",
                 "    return time"
             ]
         },
@@ -417,15 +417,15 @@
             "execution_count": null,
             "id": "fd70c693-881d-4701-851b-c15441909496",
             "metadata": {},
             "outputs": [],
             "source": [
                 "time_edges = sc.linspace(dim='local_time', unit='s', start=0, stop=24 * 60 * 60, num=6)\n",
                 "latitude = sc.linspace(dim='latitude', unit='deg', start=-90, stop=90, num=13)\n",
-                "binned = sc.bin(transformed.flatten(to='dummy'), edges=[latitude, time_edges])"
+                "binned = sc.bin(transformed.flatten(to='dummy'), latitude=latitude, local_time=time_edges)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "be960584-fa38-48f7-890a-6a85d480a9aa",
             "metadata": {},
             "source": [
```

### Comparing `scipp-24.2.0/docs/user-guide/data-structures/creating-arrays-and-datasets.ipynb` & `scipp-24.5.0/docs/user-guide/data-structures/creating-arrays-and-datasets.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997348484848485%*

 * *Differences: {"'cells'": "{44: {'source': {insert: [(2, 'data = x**2\\n')], delete: [2]}}, 50: {'source': "*

 * *            '{insert: [(1, \'\\n\')]}}, 52: {\'source\': {insert: [(1, \'\\n\'), (2, "df = '*

 * *            'pd.DataFrame({\'x\': 10 * np.arange(5), \'y\': np.linspace(0.1, 0.5, 5)})\\n")], '*

 * *            'delete: [1]}}}'}*

```diff
@@ -454,15 +454,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "x = sc.linspace('x', start=1.5, stop=3.0, num=4, unit='m')\n",
                 "m = sc.array(dims=['x'], values=[True, False, True, False])\n",
-                "data = x ** 2\n",
+                "data = x**2\n",
                 "sc.DataArray(data, coords={'x': x}, masks={'m': m})"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -524,14 +524,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from io import BytesIO\n",
+                "\n",
                 "buffer = BytesIO()\n",
                 "v = sc.arange('x', start=1.0, stop=5.0, step=1.0, unit='s')\n",
                 "v.save_hdf5(buffer)\n",
                 "sc.io.load_hdf5(buffer)"
             ]
         },
         {
@@ -547,15 +548,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
-                "df = pd.DataFrame({'x': 10*np.arange(5), 'y': np.linspace(0.1, 0.5, 5)})\n",
+                "\n",
+                "df = pd.DataFrame({'x': 10 * np.arange(5), 'y': np.linspace(0.1, 0.5, 5)})\n",
                 "df"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
```

### Comparing `scipp-24.2.0/docs/user-guide/data-structures/data-structures.ipynb` & `scipp-24.5.0/docs/user-guide/data-structures/data-structures.ipynb`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/user-guide/groupby.ipynb` & `scipp-24.5.0/docs/user-guide/groupby.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977631578947368%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(0, "param = sc.Variable(dims=[\'x\'], values=[1, 3, 1, 1, '*

 * *            '5, 3])\\n"), (1, "values = sc.Variable(dims=[\'x\', \'y\'], values=np.random.rand(6, '*

 * *            '16))\\n")], delete: [1, 0]}}, 4: {\'source\': {insert: [(4, "        \'y\': '*

 * *            'sc.Variable(dims=[\'y\'], values=np.arange(16)),\\n"), (5, \'    },\\n\'), (6, '*

 * *            '\')\\n\')], delete: [5, 4]}}, 10: {\'source\': {insert: [(1, "values = '*

 * *            'sc.Variable(dims=[\'x\', \' […]*

```diff
@@ -30,16 +30,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "param = sc.Variable(dims=['x'], values=[1,3,1,1,5,3])\n",
-                "values = sc.Variable(dims=['x', 'y'], values=np.random.rand(6,16))\n",
+                "param = sc.Variable(dims=['x'], values=[1, 3, 1, 1, 5, 3])\n",
+                "values = sc.Variable(dims=['x', 'y'], values=np.random.rand(6, 16))\n",
                 "values += 1.0 + param"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -52,16 +52,17 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "data = sc.DataArray(\n",
                 "    values,\n",
                 "    coords={\n",
                 "        'x': sc.Variable(dims=['x'], values=np.arange(6)),\n",
-                "        'y': sc.Variable(dims=['y'], values=np.arange(16))\n",
-                "    })\n",
+                "        'y': sc.Variable(dims=['y'], values=np.arange(16)),\n",
+                "    },\n",
+                ")\n",
                 "sc.plot(data)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -112,30 +113,31 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "param = sc.Variable(dims=['x'], values=np.random.rand(16))\n",
-                "values = sc.Variable(dims=['x', 'y'], values=np.random.rand(16,16))\n",
-                "values += 1.0 + 5.0*param"
+                "values = sc.Variable(dims=['x', 'y'], values=np.random.rand(16, 16))\n",
+                "values += 1.0 + 5.0 * param"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "data = sc.DataArray(\n",
                 "    values,\n",
                 "    coords={\n",
                 "        'x': sc.Variable(dims=['x'], values=np.arange(16)),\n",
-                "        'y': sc.Variable(dims=['y'], values=np.arange(16))\n",
-                "    })\n",
+                "        'y': sc.Variable(dims=['y'], values=np.arange(16)),\n",
+                "    },\n",
+                ")\n",
                 "sc.plot(data)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -186,15 +188,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "grouped = sc.groupby(data, group=param, bins=bins).mean('x') # note the lack of quotes around param!\n",
+                "grouped = sc.groupby(data, group=param, bins=bins).mean(\n",
+                "    'x'\n",
+                ")  # note the lack of quotes around param!\n",
                 "sc.plot(grouped)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
```

### Comparing `scipp-24.2.0/docs/user-guide/masking.ipynb` & `scipp-24.5.0/docs/user-guide/masking.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996212121212121%*

 * *Differences: {"'cells'": '{12: {\'source\': {insert: [(0, "ds = sc.Dataset(data={\'a\': a})\\n")], delete: '*

 * *            '[0]}}}'}*

```diff
@@ -134,15 +134,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ds = sc.Dataset(data={'a':a})\n",
+                "ds = sc.Dataset(data={'a': a})\n",
                 "ds['a'].masks['x']"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `scipp-24.2.0/docs/user-guide/plotting.ipynb` & `scipp-24.5.0/docs/user-guide/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/docs/user-guide/reading-and-writing-files.ipynb` & `scipp-24.5.0/docs/user-guide/reading-and-writing-files.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999065934065934%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(4, "var = sc.Variable(dims=[\'x\', \'y\'], '*

 * *            'values=np.random.rand(9, 3))\\n"), (5, "a = sc.DataArray(data=var, coords={\'x\': '*

 * *            'x})\\n")], delete: [5, 4]}}, 6: {\'source\': {insert: [(2, "ds = '*

 * *            'sc.io.load_csv(StringIO(csv_content), header_parser=\'bracket\')\\n")], delete: [4, '*

 * *            '3, 2]}}}'}*

```diff
@@ -33,16 +33,16 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import scipp as sc\n",
                 "\n",
                 "x = sc.Variable(dims=['x'], values=np.arange(10))\n",
-                "var = sc.Variable(dims=['x', 'y'], values=np.random.rand(9,3))\n",
-                "a = sc.DataArray(data=var, coords={'x':x})\n",
+                "var = sc.Variable(dims=['x', 'y'], values=np.random.rand(9, 3))\n",
+                "a = sc.DataArray(data=var, coords={'x': x})\n",
                 "\n",
                 "a.save_hdf5(filename='test.hdf5')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -100,17 +100,15 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from io import StringIO\n",
                 "\n",
-                "ds = sc.io.load_csv(\n",
-                "    StringIO(csv_content),\n",
-                "    header_parser='bracket')\n",
+                "ds = sc.io.load_csv(StringIO(csv_content), header_parser='bracket')\n",
                 "ds"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `scipp-24.2.0/docs/user-guide/representations-and-tables.ipynb` & `scipp-24.5.0/docs/user-guide/representations-and-tables.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974508281573499%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(0, "x = sc.arange(\'x\', 2.0)\\n"), (1, "y = '*

 * *            'sc.arange(\'y\', 4.0, unit=\'m\')\\n"), (2, "labels = sc.arange(\'y\', start=7.0, '*

 * *            'stop=10.0)\\n"), (4, \'    data={\\n\'), (5, "        \'a\': sc.array(\\n"), (6, '*

 * *            '"            dims=[\'y\', \'x\'],\\n"), (7, \'            values=np.random.random((3, '*

 * *            "2)),\\n'), (8, '            variances=0.1 * np.random.random((3, 2)),\\n'), (9, "*

 * *            '"            unit=\'an […]*

```diff
@@ -38,23 +38,28 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "x = sc.arange('x', 2.)\n",
-                "y = sc.arange('y', 4., unit='m')\n",
-                "labels = sc.arange('y', start=7., stop=10.)\n",
+                "x = sc.arange('x', 2.0)\n",
+                "y = sc.arange('y', 4.0, unit='m')\n",
+                "labels = sc.arange('y', start=7.0, stop=10.0)\n",
                 "ds = sc.Dataset(\n",
-                "    data={'a':sc.array(dims=['y', 'x'],\n",
-                "                       values=np.random.random((3, 2)),\n",
-                "                       variances=0.1 * np.random.random((3, 2)),\n",
-                "                       unit='angstrom')},\n",
-                "    coords={'x':x, 'y':y, 'y_label':labels})\n",
+                "    data={\n",
+                "        'a': sc.array(\n",
+                "            dims=['y', 'x'],\n",
+                "            values=np.random.random((3, 2)),\n",
+                "            variances=0.1 * np.random.random((3, 2)),\n",
+                "            unit='angstrom',\n",
+                "        )\n",
+                "    },\n",
+                "    coords={'x': x, 'y': y, 'y_label': labels},\n",
+                ")\n",
                 "ds['b'] = ds['a']"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -442,13 +447,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.9.18"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `scipp-24.2.0/docs/user-guide/slicing.ipynb` & `scipp-24.5.0/docs/user-guide/slicing.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975840336134454%*

 * *Differences: {"'cells'": '{33: {\'source\': {insert: [(3, "        \'b\': sc.array(dims=[\'x\', \'y\'], '*

 * *            'values=np.random.rand(3, 2)),\\n"), (4, \'    },\\n\')], delete: [3]}}, 39: '*

 * *            '{\'source\': ["assert sc.identical(d[\'x\', 1:2][\'a\'], d[\'a\'][\'x\', 1:2])\\n", '*

 * *            '"assert sc.identical(d[\'x\', 1:2][\'a\'].coords[\'x\'], d.coords[\'x\'][\'x\', '*

 * *            '1:2])"]}}',*

 * * "'metadata'": "{'language_info': {'version': '3.9.18'}}"}*

```diff
@@ -374,15 +374,16 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "d = sc.Dataset(\n",
                 "    data={\n",
                 "        'a': sc.array(dims=['y', 'x'], values=np.random.rand(2, 3)),\n",
-                "        'b': sc.array(dims=['x', 'y'], values=np.random.rand(3, 2))},\n",
+                "        'b': sc.array(dims=['x', 'y'], values=np.random.rand(3, 2)),\n",
+                "    },\n",
                 "    coords={\n",
                 "        'x': sc.array(dims=['x'], values=np.arange(3.0), unit='m'),\n",
                 "        'y': sc.array(dims=['y'], values=np.arange(2.0), unit='m'),\n",
                 "    },\n",
                 ")\n",
                 "sc.show(d)"
             ]
@@ -435,16 +436,16 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "d['x', 1:2]['a'] == d['a']['x', 1:2]\n",
-                "d['x', 1:2]['a'].coords['x'] == d.coords['x']['x', 1:2]"
+                "assert sc.identical(d['x', 1:2]['a'], d['a']['x', 1:2])\n",
+                "assert sc.identical(d['x', 1:2]['a'].coords['x'], d.coords['x']['x', 1:2])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Label-based indexing\n",
@@ -952,13 +953,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.5"
+            "version": "3.9.18"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `scipp-24.2.0/docs/user-guide/tips-tricks-and-anti-patterns.ipynb` & `scipp-24.5.0/docs/user-guide/tips-tricks-and-anti-patterns.ipynb`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/CMakeLists.txt` & `scipp-24.5.0/lib/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/CMakeLists.txt` & `scipp-24.5.0/lib/benchmark/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/accumulate_benchmark.cpp` & `scipp-24.5.0/lib/benchmark/accumulate_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/bin_benchmark.cpp` & `scipp-24.5.0/lib/benchmark/bin_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/buckets_benchmark.cpp` & `scipp-24.5.0/lib/benchmark/buckets_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/common.h` & `scipp-24.5.0/lib/benchmark/common.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/dataset_benchmark.cpp` & `scipp-24.5.0/lib/benchmark/dataset_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/dataset_operations_benchmark.cpp` & `scipp-24.5.0/lib/benchmark/dataset_operations_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/element_array_view_benchmark.cpp` & `scipp-24.5.0/lib/benchmark/element_array_view_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/events_histogram_op_benchmark.cpp` & `scipp-24.5.0/lib/benchmark/events_histogram_op_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/groupby_benchmark.cpp` & `scipp-24.5.0/lib/benchmark/groupby_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/histogram_benchmark.cpp` & `scipp-24.5.0/lib/benchmark/histogram_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/legacy_cow_ptr.h` & `scipp-24.5.0/lib/benchmark/legacy_cow_ptr.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/legacy_dataset_benchmark.cpp` & `scipp-24.5.0/lib/benchmark/legacy_dataset_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/legacy_histogram_benchmark.cpp` & `scipp-24.5.0/lib/benchmark/legacy_histogram_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/multi_index_benchmark.cpp` & `scipp-24.5.0/lib/benchmark/multi_index_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/slice_benchmark.cpp` & `scipp-24.5.0/lib/benchmark/slice_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/transform_benchmark.cpp` & `scipp-24.5.0/lib/benchmark/transform_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/variable_benchmark.cpp` & `scipp-24.5.0/lib/benchmark/variable_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/benchmark/variable_common.h` & `scipp-24.5.0/lib/benchmark/variable_common.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/.conan-recipes/llnl-units/conanfile.py` & `scipp-24.5.0/lib/cmake/.conan-recipes/llnl-units/conanfile.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/.conan-recipes/pybind11/conanfile.py` & `scipp-24.5.0/lib/cmake/.conan-recipes/pybind11/conanfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# flake8: noqa
+# ruff: noqa: F403
 import functools
 import os
 
 from conan.errors import ConanInvalidConfiguration
 from conan.tools.files import copy, get, replace_in_file
 from conan.tools.layout import basic_layout
 from conan.tools.scm import Version
@@ -68,26 +68,14 @@
             replace_in_file(
                 self,
                 os.path.join(
                     self.package_folder,
                     "lib",
                     "cmake",
                     "pybind11",
-                    "pybind11Common.cmake",
-                ),
-                "if(TARGET pybind11::lto)",
-                "if(FALSE)",
-            )
-            replace_in_file(
-                self,
-                os.path.join(
-                    self.package_folder,
-                    "lib",
-                    "cmake",
-                    "pybind11",
                     "pybind11Common.cmake",
                 ),
                 "add_library(",
                 "# add_library(",
             )
 
     def package_id(self):
```

### Comparing `scipp-24.2.0/lib/cmake/CodeCoverage.cmake` & `scipp-24.5.0/lib/cmake/CodeCoverage.cmake`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/IPO.cmake` & `scipp-24.5.0/lib/cmake/IPO.cmake`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/sanitizers-cmake/CMakeLists.txt` & `scipp-24.5.0/lib/cmake/sanitizers-cmake/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/sanitizers-cmake/LICENSE` & `scipp-24.5.0/lib/cmake/sanitizers-cmake/LICENSE`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/sanitizers-cmake/README.md` & `scipp-24.5.0/lib/cmake/sanitizers-cmake/README.md`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/sanitizers-cmake/cmake/FindASan.cmake` & `scipp-24.5.0/lib/cmake/sanitizers-cmake/cmake/FindASan.cmake`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/sanitizers-cmake/cmake/FindMSan.cmake` & `scipp-24.5.0/lib/cmake/sanitizers-cmake/cmake/FindMSan.cmake`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/sanitizers-cmake/cmake/FindSanitizers.cmake` & `scipp-24.5.0/lib/cmake/sanitizers-cmake/cmake/FindSanitizers.cmake`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/sanitizers-cmake/cmake/FindTSan.cmake` & `scipp-24.5.0/lib/cmake/sanitizers-cmake/cmake/FindTSan.cmake`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/sanitizers-cmake/cmake/FindUBSan.cmake` & `scipp-24.5.0/lib/cmake/sanitizers-cmake/cmake/FindUBSan.cmake`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/sanitizers-cmake/cmake/asan-wrapper` & `scipp-24.5.0/lib/cmake/sanitizers-cmake/cmake/asan-wrapper`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/sanitizers-cmake/cmake/sanitize-helpers.cmake` & `scipp-24.5.0/lib/cmake/sanitizers-cmake/cmake/sanitize-helpers.cmake`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/sanitizers-cmake/tests/CMakeLists.txt` & `scipp-24.5.0/lib/cmake/sanitizers-cmake/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/sanitizers-cmake/tests/asan_test.cpp` & `scipp-24.5.0/lib/cmake/sanitizers-cmake/tests/asan_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/sanitizers-cmake/tests/shortest.ext.test.cpp` & `scipp-24.5.0/lib/cmake/sanitizers-cmake/tests/shortest.ext.test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/scipp-conan.cmake` & `scipp-24.5.0/lib/cmake/scipp-conan.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # ~~~
 execute_process(
   COMMAND conan export .
   WORKING_DIRECTORY "${CMAKE_CURRENT_LIST_DIR}/.conan-recipes/llnl-units"
                     COMMAND_ECHO STDOUT
 )
 execute_process(
-  COMMAND conan export . 2.10.0@
+  COMMAND conan export . 2.12.0@
   WORKING_DIRECTORY "${CMAKE_CURRENT_LIST_DIR}/.conan-recipes/pybind11"
                     COMMAND_ECHO STDOUT
 )
 
 # Conan dependencies
 if(NOT EXISTS "${CMAKE_CURRENT_BINARY_DIR}/conan.cmake")
   message(
@@ -54,15 +54,15 @@
 conan_cmake_configure(
   REQUIRES
   ${CONAN_BENCHMARK}
   boost/1.79.0
   eigen/3.4.0
   gtest/1.11.0
   LLNL-Units/0.9.1
-  pybind11/2.10.0
+  pybind11/2.12.0
   ${CONAN_ONETBB}
   OPTIONS
   benchmark:shared=False
   boost:header_only=True
   gtest:shared=False
   LLNL-Units:shared=False
   LLNL-Units:fPIC=True
```

### Comparing `scipp-24.2.0/lib/cmake/scipp-config.cmake.in` & `scipp-24.5.0/lib/cmake/scipp-config.cmake.in`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/scipp-functions.cmake` & `scipp-24.5.0/lib/cmake/scipp-functions.cmake`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/scipp-install.cmake` & `scipp-24.5.0/lib/cmake/scipp-install.cmake`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/cmake/scipp-util.cmake` & `scipp-24.5.0/lib/cmake/scipp-util.cmake`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/common/CMakeLists.txt` & `scipp-24.5.0/lib/common/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/common/include/scipp/common/except.h` & `scipp-24.5.0/lib/common/include/scipp/common/except.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/common/include/scipp/common/index.h` & `scipp-24.5.0/lib/common/include/scipp/common/index.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/common/include/scipp/common/index_composition.h` & `scipp-24.5.0/lib/common/include/scipp/common/index_composition.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/common/include/scipp/common/initialization.h` & `scipp-24.5.0/lib/common/include/scipp/common/initialization.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/common/include/scipp/common/numeric.h` & `scipp-24.5.0/lib/common/include/scipp/common/numeric.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/common/include/scipp/common/ranges.h` & `scipp-24.5.0/lib/common/include/scipp/common/ranges.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/common/include/scipp/common/span.hpp.in` & `scipp-24.5.0/lib/common/include/scipp/common/span.hpp.in`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/common/test/CMakeLists.txt` & `scipp-24.5.0/lib/common/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/common/test/index_test.cpp` & `scipp-24.5.0/lib/common/test/index_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/common/test/isarange_test.cpp` & `scipp-24.5.0/lib/common/test/isarange_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/common/test/islinspace_test.cpp` & `scipp-24.5.0/lib/common/test/islinspace_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/common/test/numeric_test.cpp` & `scipp-24.5.0/lib/common/test/numeric_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/CMakeLists.txt` & `scipp-24.5.0/lib/core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/dict.cpp` & `scipp-24.5.0/lib/core/dict.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/dimensions.cpp` & `scipp-24.5.0/lib/core/dimensions.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/dtype.cpp` & `scipp-24.5.0/lib/core/dtype.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/element_array_view.cpp` & `scipp-24.5.0/lib/core/element_array_view.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/except.cpp` & `scipp-24.5.0/lib/core/except.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/aligned_allocator.h` & `scipp-24.5.0/lib/core/include/scipp/core/aligned_allocator.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/array_to_string.h` & `scipp-24.5.0/lib/core/include/scipp/core/array_to_string.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/bucket.h` & `scipp-24.5.0/lib/core/include/scipp/core/bucket.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/bucket_array_view.h` & `scipp-24.5.0/lib/core/include/scipp/core/bucket_array_view.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/dict.h` & `scipp-24.5.0/lib/core/include/scipp/core/dict.h`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,29 @@
 
   decltype(auto) operator->() const {
     using Result = typename BaseIterator::template TemporaryItem<
         std::decay_t<decltype(**this)>>;
     return Result(**this);
   }
 
+  template <class F> auto transform(F &&func) const & {
+    return BaseIterator::transform(
+        [new_f = std::forward<F>(func), old_f = this->m_func](const auto &x) {
+          return new_f(old_f(x));
+        });
+  }
+
+  template <class F> auto transform(F &&func) && {
+    // Make a copy for old_f to avoid referencing a member of *this.
+    return BaseIterator::transform(
+        [new_f = std::forward<F>(func), old_f = this->m_func](const auto &x) {
+          return new_f(old_f(x));
+        });
+  }
+
 private:
   std::decay_t<Func> m_func;
 };
 
 template <class I, class F>
 TransformIterator(I, F) -> TransformIterator<std::decay_t<I>, std::decay_t<F>>;
 } // namespace scipp::core::dict_detail
```

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/dimensions.h` & `scipp-24.5.0/lib/core/include/scipp/core/dimensions.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/dtype.h` & `scipp-24.5.0/lib/core/include/scipp/core/dtype.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/eigen.h` & `scipp-24.5.0/lib/core/include/scipp/core/eigen.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/arg_list.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/arg_list.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/arithmetic.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/arithmetic.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/bin.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/bin.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/bin_detail.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/bin_detail.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/comparison.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/comparison.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/creation.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/creation.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/cumulative.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/cumulative.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/event_operations.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/event_operations.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/geometric_operations.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/geometric_operations.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/histogram.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/histogram.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/hyperbolic.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/hyperbolic.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/logical.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/logical.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/map_to_bins.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/map_to_bins.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/math.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/math.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/rebin.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/rebin.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/reduction.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/reduction.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/sort.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/sort.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/special_values.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/special_values.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/to_unit.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/to_unit.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/trigonometry.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/trigonometry.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element/util.h` & `scipp-24.5.0/lib/core/include/scipp/core/element/util.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element_array.h` & `scipp-24.5.0/lib/core/include/scipp/core/element_array.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/element_array_view.h` & `scipp-24.5.0/lib/core/include/scipp/core/element_array_view.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/except.h` & `scipp-24.5.0/lib/core/include/scipp/core/except.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/has_eval.h` & `scipp-24.5.0/lib/core/include/scipp/core/has_eval.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/histogram.h` & `scipp-24.5.0/lib/core/include/scipp/core/histogram.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/memory_pool.h` & `scipp-24.5.0/lib/core/include/scipp/core/memory_pool.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/multi_index.h` & `scipp-24.5.0/lib/core/include/scipp/core/multi_index.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/parallel-fallback.h` & `scipp-24.5.0/lib/core/include/scipp/core/parallel-fallback.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/parallel-tbb.h` & `scipp-24.5.0/lib/core/include/scipp/core/parallel-tbb.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/sizes.h` & `scipp-24.5.0/lib/core/include/scipp/core/sizes.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/slice.h` & `scipp-24.5.0/lib/core/include/scipp/core/slice.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/spatial_transforms.h` & `scipp-24.5.0/lib/core/include/scipp/core/spatial_transforms.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/strides.h` & `scipp-24.5.0/lib/core/include/scipp/core/strides.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/string.h` & `scipp-24.5.0/lib/core/include/scipp/core/string.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/subbin_sizes.h` & `scipp-24.5.0/lib/core/include/scipp/core/subbin_sizes.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/tag_util.h` & `scipp-24.5.0/lib/core/include/scipp/core/tag_util.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/time_point.h` & `scipp-24.5.0/lib/core/include/scipp/core/time_point.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/transform_common.h` & `scipp-24.5.0/lib/core/include/scipp/core/transform_common.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/value_and_variance.h` & `scipp-24.5.0/lib/core/include/scipp/core/value_and_variance.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/values_and_variances.h` & `scipp-24.5.0/lib/core/include/scipp/core/values_and_variances.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/include/scipp/core/view_index.h` & `scipp-24.5.0/lib/core/include/scipp/core/view_index.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/multi_index.cpp` & `scipp-24.5.0/lib/core/multi_index.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/rename.h` & `scipp-24.5.0/lib/core/rename.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/sizes.cpp` & `scipp-24.5.0/lib/core/sizes.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/slice.cpp` & `scipp-24.5.0/lib/core/slice.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/strides.cpp` & `scipp-24.5.0/lib/core/strides.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/string.cpp` & `scipp-24.5.0/lib/core/string.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/subbin_sizes.cpp` & `scipp-24.5.0/lib/core/subbin_sizes.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/CMakeLists.txt` & `scipp-24.5.0/lib/core/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/arithmetic_parameters.h` & `scipp-24.5.0/lib/core/test/arithmetic_parameters.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/array_to_string_test.cpp` & `scipp-24.5.0/lib/core/test/array_to_string_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/dict_test.cpp` & `scipp-24.5.0/lib/core/test/dict_test.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -555,14 +555,34 @@
   EXPECT_EQ(*it, -823 / 2.0);
   ++it;
   EXPECT_EQ(*it, 14 / 2.0);
   ++it;
   EXPECT_EQ(it, dict.end());
 }
 
+TEST(Dict, transform_iterator_chained) {
+  DimDict dict{{Dim::Energy, -823}, {Dim::Row, 14}};
+
+  auto it = dict.begin()
+                .transform([](const auto &x) {
+                  return std::pair{x.first, 2 * x.second};
+                })
+                .transform([](const auto &x) {
+                  return std::pair{Dim::Energy, x.second};
+                });
+
+  EXPECT_EQ(it->first, Dim::Energy);
+  EXPECT_EQ(it->second, 2 * -823);
+  ++it;
+  EXPECT_EQ(it->first, Dim::Energy);
+  EXPECT_EQ(it->second, 2 * 14);
+  ++it;
+  EXPECT_EQ(it, dict.end());
+}
+
 TEST(Dict, transform_iterator_compare_with_end_with_transform) {
   DimDict dict{{Dim::Time, 72}, {Dim::Y, 41}};
 
   const auto f = [](const auto &x) { return x; };
 
   auto it = dict.values_begin().transform(f);
   ++it;
```

### Comparing `scipp-24.2.0/lib/core/test/dimensions_test.cpp` & `scipp-24.5.0/lib/core/test/dimensions_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/dtype_test.cpp` & `scipp-24.5.0/lib/core/test/dtype_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/eigen_test.cpp` & `scipp-24.5.0/lib/core/test/eigen_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/element_arithmetic_test.cpp` & `scipp-24.5.0/lib/core/test/element_arithmetic_test.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -196,15 +196,16 @@
     this->expect_eq(mod(p.dividend, p.divisor), p.remainder);
   }
 }
 
 TEST(ElementArithmeticDivisionTest, units) {
   EXPECT_EQ(divide(units::m, units::s), units::m / units::s);
   EXPECT_EQ(floor_divide(units::m, units::s), units::m / units::s);
-  EXPECT_EQ(mod(units::m, units::s), units::m);
+  EXPECT_EQ(mod(units::m, units::m), units::m);
+  EXPECT_THROW(mod(units::m, units::s), except::UnitError);
 }
 
 class ElementNanArithmeticTest : public ::testing::Test {
 protected:
   double x = 1.0;
   double y = 2.0;
   double dNaN = std::numeric_limits<double>::quiet_NaN();
```

### Comparing `scipp-24.2.0/lib/core/test/element_array_test.cpp` & `scipp-24.5.0/lib/core/test/element_array_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/element_array_view_test.cpp` & `scipp-24.5.0/lib/core/test/element_array_view_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/element_bin_detail_test.cpp` & `scipp-24.5.0/lib/core/test/element_bin_detail_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/element_comparison_test.cpp` & `scipp-24.5.0/lib/core/test/element_comparison_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/element_event_operations_test.cpp` & `scipp-24.5.0/lib/core/test/element_event_operations_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/element_geometric_operations_test.cpp` & `scipp-24.5.0/lib/core/test/element_geometric_operations_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/element_histogram_test.cpp` & `scipp-24.5.0/lib/core/test/element_histogram_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/element_hyperbolic_test.cpp` & `scipp-24.5.0/lib/core/test/element_hyperbolic_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/element_logical_test.cpp` & `scipp-24.5.0/lib/core/test/element_logical_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/element_map_to_bins_test.cpp` & `scipp-24.5.0/lib/core/test/element_map_to_bins_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/element_math_test.cpp` & `scipp-24.5.0/lib/core/test/element_math_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/element_special_values_test.cpp` & `scipp-24.5.0/lib/core/test/element_special_values_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/element_to_unit_test.cpp` & `scipp-24.5.0/lib/core/test/element_to_unit_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/element_trigonometry_test.cpp` & `scipp-24.5.0/lib/core/test/element_trigonometry_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/element_util_test.cpp` & `scipp-24.5.0/lib/core/test/element_util_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/generate_arithmetic_parameters.py` & `scipp-24.5.0/lib/core/test/generate_arithmetic_parameters.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/multi_index_test.cpp` & `scipp-24.5.0/lib/core/test/multi_index_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/sizes_test.cpp` & `scipp-24.5.0/lib/core/test/sizes_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/slice_test.cpp` & `scipp-24.5.0/lib/core/test/slice_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/spatial_transforms_test.cpp` & `scipp-24.5.0/lib/core/test/spatial_transforms_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/string_test.cpp` & `scipp-24.5.0/lib/core/test/string_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/subbin_sizes_test.cpp` & `scipp-24.5.0/lib/core/test/subbin_sizes_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/time_point_test.cpp` & `scipp-24.5.0/lib/core/test/time_point_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/transform_common_test.cpp` & `scipp-24.5.0/lib/core/test/transform_common_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/value_and_variance_test.cpp` & `scipp-24.5.0/lib/core/test/value_and_variance_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/test/view_index_test.cpp` & `scipp-24.5.0/lib/core/test/view_index_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/core/view_index.cpp` & `scipp-24.5.0/lib/core/view_index.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/CMakeLists.txt` & `scipp-24.5.0/lib/dataset/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/arithmetic.cpp` & `scipp-24.5.0/lib/dataset/arithmetic.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/astype.cpp` & `scipp-24.5.0/lib/dataset/astype.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/bin.cpp` & `scipp-24.5.0/lib/dataset/bin.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/bin_detail.cpp` & `scipp-24.5.0/lib/dataset/bin_detail.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/bin_detail.h` & `scipp-24.5.0/lib/dataset/bin_detail.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/bins.cpp` & `scipp-24.5.0/lib/dataset/bins.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/bins_util.h` & `scipp-24.5.0/lib/dataset/bins_util.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/counts.cpp` & `scipp-24.5.0/lib/dataset/counts.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/data_array.cpp` & `scipp-24.5.0/lib/dataset/data_array.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/dataset.cpp` & `scipp-24.5.0/lib/dataset/dataset.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/dataset_operations_common.h` & `scipp-24.5.0/lib/dataset/dataset_operations_common.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/except.cpp` & `scipp-24.5.0/lib/dataset/except.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/extract.cpp` & `scipp-24.5.0/lib/dataset/extract.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/groupby.cpp` & `scipp-24.5.0/lib/dataset/groupby.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/histogram.cpp` & `scipp-24.5.0/lib/dataset/histogram.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/bin.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/bin.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/bins.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/bins.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/counts.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/counts.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/data_array.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/data_array.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/dataset.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/dataset.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/dataset_util.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/dataset_util.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/except.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/except.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/extract.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/extract.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/groupby.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/groupby.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/histogram.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/histogram.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/mean.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/mean.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/nanmean.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/nanmean.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/rebin.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/rebin.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/shape.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/shape.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/sized_dict.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/sized_dict.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/sized_dict_forward.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/sized_dict_forward.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/slice.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/slice.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/sort.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/sort.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/string.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/string.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/include/scipp/dataset/util.h` & `scipp-24.5.0/lib/dataset/include/scipp/dataset/util.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/mean.cpp` & `scipp-24.5.0/lib/dataset/mean.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/nanmean.cpp` & `scipp-24.5.0/lib/dataset/nanmean.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/operations.cpp` & `scipp-24.5.0/lib/dataset/operations.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/rebin.cpp` & `scipp-24.5.0/lib/dataset/rebin.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/shape.cpp` & `scipp-24.5.0/lib/dataset/shape.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/sized_dict.cpp` & `scipp-24.5.0/lib/dataset/sized_dict.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/slice.cpp` & `scipp-24.5.0/lib/dataset/slice.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/sort.cpp` & `scipp-24.5.0/lib/dataset/sort.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/string.cpp` & `scipp-24.5.0/lib/dataset/string.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/CMakeLists.txt` & `scipp-24.5.0/lib/dataset/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/astype_test.cpp` & `scipp-24.5.0/lib/dataset/test/astype_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/attributes_test.cpp` & `scipp-24.5.0/lib/dataset/test/attributes_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/bin_test.cpp` & `scipp-24.5.0/lib/dataset/test/bin_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/binned_arithmetic_test.cpp` & `scipp-24.5.0/lib/dataset/test/binned_arithmetic_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/binned_creation_test.cpp` & `scipp-24.5.0/lib/dataset/test/binned_creation_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/bins_reduction_test.cpp` & `scipp-24.5.0/lib/dataset/test/bins_reduction_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/bins_test.cpp` & `scipp-24.5.0/lib/dataset/test/bins_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/bins_view_test.cpp` & `scipp-24.5.0/lib/dataset/test/bins_view_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/concat_test.cpp` & `scipp-24.5.0/lib/dataset/test/concat_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/coords_view_test.cpp` & `scipp-24.5.0/lib/dataset/test/coords_view_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/copy_test.cpp` & `scipp-24.5.0/lib/dataset/test/copy_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/counts_test.cpp` & `scipp-24.5.0/lib/dataset/test/counts_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/data_array_arithmetic_test.cpp` & `scipp-24.5.0/lib/dataset/test/data_array_arithmetic_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/data_array_comparison_test.cpp` & `scipp-24.5.0/lib/dataset/test/data_array_comparison_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/data_array_test.cpp` & `scipp-24.5.0/lib/dataset/test/data_array_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/data_view_test.cpp` & `scipp-24.5.0/lib/dataset/test/data_view_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/dataset_arithmetic_test.cpp` & `scipp-24.5.0/lib/dataset/test/dataset_arithmetic_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/dataset_comparison_test.cpp` & `scipp-24.5.0/lib/dataset/test/dataset_comparison_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/dataset_operations_test.cpp` & `scipp-24.5.0/lib/dataset/test/dataset_operations_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/dataset_test.cpp` & `scipp-24.5.0/lib/dataset/test/dataset_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/dataset_test_common.cpp` & `scipp-24.5.0/lib/dataset/test/dataset_test_common.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/dataset_test_common.h` & `scipp-24.5.0/lib/dataset/test/dataset_test_common.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/dataset_view_test.cpp` & `scipp-24.5.0/lib/dataset/test/dataset_view_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/equals_nan_test.cpp` & `scipp-24.5.0/lib/dataset/test/equals_nan_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/event_data_operations_consistency_test.cpp` & `scipp-24.5.0/lib/dataset/test/event_data_operations_consistency_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/except_test.cpp` & `scipp-24.5.0/lib/dataset/test/except_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/generated_test.cpp` & `scipp-24.5.0/lib/dataset/test/generated_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/groupby_test.cpp` & `scipp-24.5.0/lib/dataset/test/groupby_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/histogram_test.cpp` & `scipp-24.5.0/lib/dataset/test/histogram_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/logical_reduction_test.cpp` & `scipp-24.5.0/lib/dataset/test/logical_reduction_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/masks_test.cpp` & `scipp-24.5.0/lib/dataset/test/masks_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/mean_test.cpp` & `scipp-24.5.0/lib/dataset/test/mean_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/merge_test.cpp` & `scipp-24.5.0/lib/dataset/test/merge_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/minmax_test.cpp` & `scipp-24.5.0/lib/dataset/test/minmax_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/rebin_test.cpp` & `scipp-24.5.0/lib/dataset/test/rebin_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/self_assignment_test.cpp` & `scipp-24.5.0/lib/dataset/test/self_assignment_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/set_slice_test.cpp` & `scipp-24.5.0/lib/dataset/test/set_slice_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/shape_test.cpp` & `scipp-24.5.0/lib/dataset/test/shape_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/size_of_test.cpp` & `scipp-24.5.0/lib/dataset/test/size_of_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/slice_by_value_test.cpp` & `scipp-24.5.0/lib/dataset/test/slice_by_value_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/slice_test.cpp` & `scipp-24.5.0/lib/dataset/test/slice_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/sort_test.cpp` & `scipp-24.5.0/lib/dataset/test/sort_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/string_test.cpp` & `scipp-24.5.0/lib/dataset/test/string_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/sum_test.cpp` & `scipp-24.5.0/lib/dataset/test/sum_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/test_data_arrays.cpp` & `scipp-24.5.0/lib/dataset/test/test_data_arrays.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/test_data_arrays.h` & `scipp-24.5.0/lib/dataset/test/test_data_arrays.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/test/to_unit_test.cpp` & `scipp-24.5.0/lib/dataset/test/to_unit_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/to_unit.cpp` & `scipp-24.5.0/lib/dataset/to_unit.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/util.cpp` & `scipp-24.5.0/lib/dataset/util.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/variable_instantiate_bin_elements.cpp` & `scipp-24.5.0/lib/dataset/variable_instantiate_bin_elements.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/variable_instantiate_dataset.cpp` & `scipp-24.5.0/lib/dataset/variable_instantiate_dataset.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/dataset/variable_reduction.cpp` & `scipp-24.5.0/lib/dataset/variable_reduction.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/CMakeLists.txt` & `scipp-24.5.0/lib/python/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -51,17 +51,14 @@
 set_target_properties(_scipp PROPERTIES CXX_VISIBILITY_PRESET hidden)
 set_target_properties(
   _scipp
   PROPERTIES INSTALL_RPATH
              "${CMAKE_INSTALL_RPATH}/${RELATIVE_LIB}/${CMAKE_INSTALL_LIBDIR}"
 )
 
-pybind11_strip(_scipp)
-pybind11_extension(_scipp)
-
 if(PRECOMPILED_HEADERS)
   target_precompile_headers(_scipp PRIVATE pybind11.h)
 endif()
 
 add_sanitizers(_scipp)
 
 install(TARGETS _scipp DESTINATION ${PYTHONDIR})
```

### Comparing `scipp-24.2.0/lib/python/benchmark/variable.py` & `scipp-24.5.0/lib/python/benchmark/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,8 +37,8 @@
         'avg_iteration_time': total_time,
         'mbytes_per_second': bytes_per_second / 1e6,
     }
 
 
 if __name__ == '__main__':
     for a in [1e7, 1e8, 1e9, 5e9]:
-        print('assign_from_numpy_1d', assign_from_numpy_1d(int(a)))
+        print('assign_from_numpy_1d', assign_from_numpy_1d(int(a)))  # noqa: T201
```

### Comparing `scipp-24.2.0/lib/python/bind_data_access.h` & `scipp-24.5.0/lib/python/bind_data_access.h`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 /// @file
 /// @author Simon Heybrock
 #pragma once
 
 #include <algorithm>
 #include <variant>
 
+#include <pybind11/typing.h>
+
 #include "scipp/core/dtype.h"
 #include "scipp/core/eigen.h"
 #include "scipp/core/spatial_transforms.h"
 #include "scipp/core/tag_util.h"
 #include "scipp/dataset/dataset.h"
 #include "scipp/dataset/except.h"
 #include "scipp/variable/shape.h"
@@ -443,15 +445,15 @@
 template <class T, class... Ignored>
 void bind_common_data_properties(pybind11::class_<T, Ignored...> &c) {
   c.def_property_readonly(
       "dims",
       [](const T &self) {
         const auto &labels = self.dims().labels();
         const auto ndim = static_cast<size_t>(self.ndim());
-        py::tuple dims(ndim);
+        py::typing::Tuple<py::str, py::ellipsis> dims(ndim);
         for (size_t i = 0; i < ndim; ++i) {
           dims[i] = labels[i].name();
         }
         return dims;
       },
       "Dimension labels of the data (read-only).",
       py::return_value_policy::move);
@@ -464,28 +466,28 @@
       "Number of dimensions of the data (read-only).",
       py::return_value_policy::move);
   c.def_property_readonly(
       "shape",
       [](const T &self) {
         const auto &sizes = self.dims().sizes();
         const auto ndim = static_cast<size_t>(self.ndim());
-        py::tuple shape(ndim);
+        py::typing::Tuple<int, py::ellipsis> shape(ndim);
         for (size_t i = 0; i < ndim; ++i) {
           shape[i] = sizes[i];
         }
         return shape;
       },
       "Shape of the data (read-only).", py::return_value_policy::move);
   c.def_property_readonly(
       "sizes",
       [](const T &self) {
         const auto &dims = self.dims();
         // Use py::dict directly instead of std::map in order to guarantee
         // that items are stored in the order of insertion.
-        py::dict sizes;
+        py::typing::Dict<py::str, int> sizes;
         for (const auto label : dims.labels()) {
           sizes[label.name().c_str()] = dims[label];
         }
         return sizes;
       },
       "dict mapping dimension labels to dimension sizes (read-only).",
       py::return_value_policy::move);
```

### Comparing `scipp-24.2.0/lib/python/bind_data_array.h` & `scipp-24.5.0/lib/python/bind_data_array.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 // SPDX-License-Identifier: BSD-3-Clause
 // Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 /// @file
 /// @author Simon Heybrock
 #pragma once
 
+#include <pybind11/typing.h>
+
 #include "scipp/dataset/dataset.h"
 #include "scipp/variable/variable_factory.h"
 
 #include "bind_operators.h"
 #include "pybind11.h"
 #include "view.h"
 
@@ -121,15 +123,15 @@
 }
 
 template <class T, class... Ignored>
 void bind_pop(pybind11::class_<T, Ignored...> &view) {
   view.def(
       "_pop",
       [](T &self, const std::string &key) {
-        return py::cast(self.extract(typename T::key_type{key}));
+        return self.extract(typename T::key_type{key});
       },
       py::arg("k"));
 }
 
 template <class T, class... Ignored>
 void bind_set_aligned(pybind11::class_<T, Ignored...> &view) {
   view.def(
@@ -155,18 +157,24 @@
 template <class T, class... Ignored>
 void bind_dict_popitem(pybind11::class_<T, Ignored...> &view) {
   view.def("popitem", [](T &self) {
     typename T::key_type key;
     for (const auto &k : keys_view(self))
       key = k;
     const auto item = py::cast(self.extract(key));
+
+    using Pair =
+        py::typing::Tuple<py::str, std::decay_t<decltype(self.extract(key))>>;
+    Pair result(2);
     if constexpr (std::is_same_v<typename T::key_type, Dim>)
-      return std::tuple{key.name(), item};
+      result[0] = key.name();
     else
-      return std::tuple{key, item};
+      result[0] = key;
+    result[1] = item;
+    return result;
   });
 }
 
 template <class T, class... Ignored>
 void bind_dict_copy(pybind11::class_<T, Ignored...> &view) {
   view.def(
           "copy",
@@ -302,15 +310,15 @@
       "data",
       py::cpp_function([](T &self) { return self.data(); },
                        py::return_value_policy::copy),
       [](T &self, const Variable &data) { self.setData(data); },
       R"(Underlying data item.)");
   c.def_property_readonly(
       "coords", [](T &self) -> decltype(auto) { return self.coords(); },
-      R"(Dict of aligned coords.)");
+      R"(Dict of coords.)");
   c.def_property_readonly(
       "deprecated_meta", [](T &self) -> decltype(auto) { return self.meta(); },
       R"(Dict of coords and attrs.)");
   c.def_property_readonly(
       "deprecated_attrs",
       [](T &self) -> decltype(auto) { return self.attrs(); },
       R"(Dict of attrs.)");
```

### Comparing `scipp-24.2.0/lib/python/bind_operators.h` & `scipp-24.5.0/lib/python/bind_operators.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/bind_slice_methods.h` & `scipp-24.5.0/lib/python/bind_slice_methods.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/bind_units.cpp` & `scipp-24.5.0/lib/python/bind_units.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/bins.cpp` & `scipp-24.5.0/lib/python/bins.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -99,22 +99,42 @@
   bind_pop(c);
   if constexpr (HasAlignment) {
     bind_set_aligned(c);
   }
 }
 
 template <class T> void bind_bins_view(py::module &m) {
+  bind_helper_view<str_items_view,
+                   decltype(dataset::bins_view<T>(Variable{}).coords())>(
+      m, "_BinsCoords");
+  bind_helper_view<items_view,
+                   decltype(dataset::bins_view<T>(Variable{}).masks())>(
+      m, "_BinsMasks");
+  bind_helper_view<str_keys_view,
+                   decltype(dataset::bins_view<T>(Variable{}).coords())>(
+      m, "_BinsCoords");
+  bind_helper_view<keys_view,
+                   decltype(dataset::bins_view<T>(Variable{}).masks())>(
+      m, "_BinsMasks");
+  bind_helper_view<values_view,
+                   decltype(dataset::bins_view<T>(Variable{}).coords())>(
+      m, "_BinsCoords");
+  bind_helper_view<values_view,
+                   decltype(dataset::bins_view<T>(Variable{}).masks())>(
+      m, "_BinsMasks");
+
   py::class_<decltype(dataset::bins_view<T>(Variable{}))> c(
       m, "_BinsViewDataArray");
   bind_bins_map_view<decltype(dataset::bins_view<T>(Variable{}).meta())>(
       m, "_BinsMeta");
-  bind_bins_map_view<decltype(dataset::bins_view<T>(Variable{}).coords()),
-                     true>(m, "_BinsCoords");
-  bind_bins_map_view<decltype(dataset::bins_view<T>(Variable{}).masks())>(
-      m, "_BinsMasks");
+  bind_mutable_view_no_dim<
+      decltype(dataset::bins_view<T>(Variable{}).coords())>(
+      m, "_BinsCoords", "Dict of event coords.");
+  bind_mutable_view<decltype(dataset::bins_view<T>(Variable{}).masks())>(
+      m, "_BinsMasks", "Dict of event masks.");
   bind_bins_map_view<decltype(dataset::bins_view<T>(Variable{}).attrs())>(
       m, "_BinsAttrs");
   bind_data_array_properties(c);
   m.def("_bins_view",
         [](const Variable &var) { return dataset::bins_view<T>(var); });
 }
```

### Comparing `scipp-24.2.0/lib/python/comparison.cpp` & `scipp-24.5.0/lib/python/comparison.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/counts.cpp` & `scipp-24.5.0/lib/python/counts.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/cumulative.cpp` & `scipp-24.5.0/lib/python/cumulative.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/dataset.cpp` & `scipp-24.5.0/lib/python/dataset.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         return DataArray{data, to_cpp_dict<Dim, Variable>(coords),
                          to_cpp_dict<std::string, Variable>(masks),
                          to_cpp_dict<Dim, Variable>(attrs), name};
       }),
       py::arg("data"), py::kw_only(), py::arg("coords") = py::dict(),
       py::arg("masks") = py::dict(), py::arg("attrs") = py::dict(),
       py::arg("name") = std::string{},
-      R"doc(__init__(self, data: Variable, coords: Union[typing.Mapping[str, Variable], Iterable[Tuple[str, Variable]]] = {}, masks: Union[typing.Mapping[str, Variable], Iterable[Tuple[str, Variable]]] = {}, attrs: Union[typing.Mapping[str, Variable], Iterable[Tuple[str, Variable]]] = {}, name: str = '') -> None
+      R"doc(__init__(self, data: Variable, coords: Union[Mapping[str, Variable], Iterable[tuple[str, Variable]]] = {}, masks: Union[Mapping[str, Variable], Iterable[tuple[str, Variable]]] = {}, attrs: Union[Mapping[str, Variable], Iterable[tuple[str, Variable]]] = {}, name: str = '') -> None
 
           DataArray initializer.
 
           Parameters
           ----------
           data:
               Data and optionally variances.
@@ -229,15 +229,15 @@
         const auto coords_dict =
             coords.is_none() ? py::dict() : py::dict(coords);
         auto d = dataset_from_data_and_coords(data_dict, coords_dict);
         return d.is_valid() ? d : dataset_from_coords(coords_dict);
       }),
       py::arg("data") = py::none{}, py::kw_only(),
       py::arg("coords") = py::none{},
-      R"doc(__init__(self, data: Union[typing.Mapping[str, Union[Variable, DataArray]], Iterable[Tuple[str, Union[Variable, DataArray]]]] = {}, coords: Union[typing.Mapping[str, Variable], Iterable[Tuple[str, Variable]]] = {}) -> None
+      R"doc(__init__(self, data: Union[Mapping[str, Union[Variable, DataArray]], Iterable[tuple[str, Union[Variable, DataArray]]]] = {}, coords: Union[Mapping[str, Variable], Iterable[tuple[str, Variable]]] = {}) -> None
 
       Dataset initializer.
 
       Parameters
       ----------
       data:
           Dictionary of name and data pairs.
```

### Comparing `scipp-24.2.0/lib/python/dim.h` & `scipp-24.5.0/lib/python/dim.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/docstring.cpp` & `scipp-24.5.0/lib/python/docstring.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/docstring.h` & `scipp-24.5.0/lib/python/docstring.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/dtype.cpp` & `scipp-24.5.0/lib/python/dtype.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/dtype.h` & `scipp-24.5.0/lib/python/dtype.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/element_array_view.cpp` & `scipp-24.5.0/lib/python/element_array_view.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/except.cpp` & `scipp-24.5.0/lib/python/except.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/geometry.cpp` & `scipp-24.5.0/lib/python/geometry.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/groupby.cpp` & `scipp-24.5.0/lib/python/groupby.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/histogram.cpp` & `scipp-24.5.0/lib/python/histogram.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/numpy.cpp` & `scipp-24.5.0/lib/python/numpy.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/numpy.h` & `scipp-24.5.0/lib/python/numpy.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/operations.cpp` & `scipp-24.5.0/lib/python/operations.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/py_object.cpp` & `scipp-24.5.0/lib/python/py_object.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/py_object.h` & `scipp-24.5.0/lib/python/py_object.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/pybind11.h` & `scipp-24.5.0/lib/python/pybind11.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/scipp.cpp` & `scipp-24.5.0/lib/python/scipp.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/shape.cpp` & `scipp-24.5.0/lib/python/shape.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/slice_utils.cpp` & `scipp-24.5.0/lib/python/slice_utils.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/transform.cpp` & `scipp-24.5.0/lib/python/transform.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/trigonometry.cpp` & `scipp-24.5.0/lib/python/trigonometry.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/unary.cpp` & `scipp-24.5.0/lib/python/unary.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/unit.cpp` & `scipp-24.5.0/lib/python/unit.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/unit.h` & `scipp-24.5.0/lib/python/unit.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/variable.cpp` & `scipp-24.5.0/lib/python/variable.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/variable_creation.cpp` & `scipp-24.5.0/lib/python/variable_creation.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/variable_init.cpp` & `scipp-24.5.0/lib/python/variable_init.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/python/view.h` & `scipp-24.5.0/lib/python/view.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/templates/dataset_binary.cpp.in` & `scipp-24.5.0/lib/templates/dataset_binary.cpp.in`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/templates/dataset_binary.h.in` & `scipp-24.5.0/lib/templates/dataset_binary.h.in`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/templates/dataset_inplace.cpp.in` & `scipp-24.5.0/lib/templates/dataset_inplace.cpp.in`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/templates/dataset_inplace.h.in` & `scipp-24.5.0/lib/templates/dataset_inplace.h.in`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/templates/dataset_reduction.cpp.in` & `scipp-24.5.0/lib/templates/dataset_reduction.cpp.in`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/templates/dataset_reduction.h.in` & `scipp-24.5.0/lib/templates/dataset_reduction.h.in`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/templates/dataset_unary.cpp.in` & `scipp-24.5.0/lib/templates/dataset_unary.cpp.in`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/templates/python_binary.cpp.in` & `scipp-24.5.0/lib/templates/python_binary.cpp.in`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/templates/python_reduction.cpp.in` & `scipp-24.5.0/lib/templates/python_reduction.cpp.in`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/templates/python_unary.cpp.in` & `scipp-24.5.0/lib/templates/python_unary.cpp.in`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/templates/variable_binary.cpp.in` & `scipp-24.5.0/lib/templates/variable_binary.cpp.in`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/templates/variable_binary.h.in` & `scipp-24.5.0/lib/templates/variable_binary.h.in`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/templates/variable_inplace.cpp.in` & `scipp-24.5.0/lib/templates/variable_inplace.cpp.in`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/templates/variable_unary.cpp.in` & `scipp-24.5.0/lib/templates/variable_unary.cpp.in`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/test/fix_typed_test_suite_warnings.h` & `scipp-24.5.0/lib/test/fix_typed_test_suite_warnings.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/test/random.h` & `scipp-24.5.0/lib/test/random.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/test/test_macros.h` & `scipp-24.5.0/lib/test/test_macros.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/test/test_nans.h` & `scipp-24.5.0/lib/test/test_nans.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/test/test_operations.h` & `scipp-24.5.0/lib/test/test_operations.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/test/test_print_variable.h` & `scipp-24.5.0/lib/test/test_print_variable.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/units/CMakeLists.txt` & `scipp-24.5.0/lib/units/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/units/dim.cpp` & `scipp-24.5.0/lib/units/dim.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/units/except.cpp` & `scipp-24.5.0/lib/units/except.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/units/include/scipp/units/dim.h` & `scipp-24.5.0/lib/units/include/scipp/units/dim.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/units/include/scipp/units/except.h` & `scipp-24.5.0/lib/units/include/scipp/units/except.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/units/include/scipp/units/string.h` & `scipp-24.5.0/lib/units/include/scipp/units/string.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/units/include/scipp/units/unit.h` & `scipp-24.5.0/lib/units/include/scipp/units/unit.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/units/string.cpp` & `scipp-24.5.0/lib/units/string.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/units/test/CMakeLists.txt` & `scipp-24.5.0/lib/units/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/units/test/dim_test.cpp` & `scipp-24.5.0/lib/units/test/dim_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/units/test/unit_test.cpp` & `scipp-24.5.0/lib/units/test/unit_test.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -117,18 +117,21 @@
   EXPECT_EQ(counts / counts, units::dimensionless);
 }
 
 TEST(UnitTest, modulo) {
   Unit one{units::dimensionless};
   Unit l{units::m};
   Unit t{units::s};
-  EXPECT_EQ(l % one, l);
-  EXPECT_EQ(t % one, t);
+  Unit none{units::none};
   EXPECT_EQ(l % l, l);
-  EXPECT_EQ(l % t, l);
+  EXPECT_EQ(t % t, t);
+  EXPECT_THROW(l % t, except::UnitError);
+  EXPECT_THROW(l % one, except::UnitError);
+  EXPECT_THROW(l % none, except::UnitError);
+  EXPECT_THROW(t % l, except::UnitError);
 }
 
 TEST(UnitTest, pow) {
   EXPECT_EQ(pow(units::m, 0), units::one);
   EXPECT_EQ(pow(units::m, 1), units::m);
   EXPECT_EQ(pow(units::m, 2), units::m * units::m);
   EXPECT_EQ(pow(units::m, -1), units::one / units::m);
```

### Comparing `scipp-24.2.0/lib/units/unit.cpp` & `scipp-24.5.0/lib/units/unit.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -125,19 +125,18 @@
   if (llnl::units::divides_overflows(a.underlying(), b.underlying()))
     throw except::UnitError("Unsupported unit as result of division: (" +
                             a.name() + ") / (" + b.name() + ')');
   return Unit{a.underlying() / b.underlying()};
 }
 
 Unit operator%(const Unit &a, const Unit &b) {
-  if (a == none && b == none)
+  if (a == b)
     return a;
-  expect_not_none(a, "modulo");
-  expect_not_none(b, "modulo");
-  return a;
+  throw except::UnitError("Cannot perform modulo operation with " + a.name() +
+                          " and " + b.name() + ". Units must be the same.");
 }
 
 Unit operator-(const Unit &a) { return a; }
 
 Unit abs(const Unit &a) { return a; }
 
 Unit floor(const Unit &a) { return a; }
```

### Comparing `scipp-24.2.0/lib/variable/CMakeLists.txt` & `scipp-24.5.0/lib/variable/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/arithmetic.cpp` & `scipp-24.5.0/lib/variable/arithmetic.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/astype.cpp` & `scipp-24.5.0/lib/variable/astype.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/bin_array_variable.cpp` & `scipp-24.5.0/lib/variable/bin_array_variable.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/bin_detail.cpp` & `scipp-24.5.0/lib/variable/bin_detail.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/bin_util.cpp` & `scipp-24.5.0/lib/variable/bin_util.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/bins.cpp` & `scipp-24.5.0/lib/variable/bins.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/comparison.cpp` & `scipp-24.5.0/lib/variable/comparison.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/creation.cpp` & `scipp-24.5.0/lib/variable/creation.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/cumulative.cpp` & `scipp-24.5.0/lib/variable/cumulative.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/except.cpp` & `scipp-24.5.0/lib/variable/except.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/accumulate.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/accumulate.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/arithmetic.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/arithmetic.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/astype.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/astype.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/bin_array_model.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/bin_array_model.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/bin_array_variable.tcc` & `scipp-24.5.0/lib/variable/include/scipp/variable/bin_array_variable.tcc`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/bin_detail.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/bin_detail.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/bins.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/bins.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/comparison.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/comparison.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/creation.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/creation.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/cumulative.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/cumulative.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/element_array_model.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/element_array_model.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/element_array_variable.tcc` & `scipp-24.5.0/lib/variable/include/scipp/variable/element_array_variable.tcc`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/except.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/except.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/misc_operations.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/misc_operations.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/pow.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/pow.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/rebin.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/rebin.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/reduction.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/reduction.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/shape.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/shape.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/slice.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/slice.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/sort.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/sort.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/special_values.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/special_values.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/string.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/string.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/structure_array_model.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/structure_array_model.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/structure_array_variable.tcc` & `scipp-24.5.0/lib/variable/include/scipp/variable/structure_array_variable.tcc`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/structures.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/structures.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/subspan_view.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/subspan_view.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/transform.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/transform.h`

 * *Files 1% similar despite different names*

```diff
@@ -649,14 +649,20 @@
   }
   template <class... Ts, class Op, class Var, class... Other>
   static void transform(Op op, const std::string_view &name, Var &&var,
                         const Other &...other) {
     using namespace detail;
     (scipp::expect::includes(var.dims(), other.dims()), ...);
 
+    if (!is_bins(var) && ((is_bins(other) || ...))) {
+      throw except::BinnedDataError(
+          "Cannot apply inplace operation where target is "
+          "not binned but arguments are binned");
+    }
+
     if constexpr (!std::is_base_of_v<
                       core::transform_flags::force_variance_broadcast_t, Op>) {
       if (const auto dims = merge(var.dims(), other.dims()...);
           (bad_variance_broadcast(dims, other) || ...))
         throw_variances_broadcast_error(var, other...);
       if (is_bins(var) || (is_bins(other) || ...))
         if (((other.has_variances() && !is_bins(other)) || ...))
```

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/transform_subspan.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/transform_subspan.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/util.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/util.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/variable.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/variable.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/variable.tcc` & `scipp-24.5.0/lib/variable/include/scipp/variable/variable.tcc`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/variable_concept.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/variable_concept.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/variable_factory.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/variable_factory.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/variable_keyword_arg_constructor.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/variable_keyword_arg_constructor.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/include/scipp/variable/visit.h` & `scipp-24.5.0/lib/variable/include/scipp/variable/visit.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/inv.cpp` & `scipp-24.5.0/lib/variable/inv.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/math.cpp` & `scipp-24.5.0/lib/variable/math.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/operations.cpp` & `scipp-24.5.0/lib/variable/operations.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/operations_common.h` & `scipp-24.5.0/lib/variable/operations_common.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/pow.cpp` & `scipp-24.5.0/lib/variable/pow.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/rebin.cpp` & `scipp-24.5.0/lib/variable/rebin.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/reduction.cpp` & `scipp-24.5.0/lib/variable/reduction.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/shape.cpp` & `scipp-24.5.0/lib/variable/shape.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/slice.cpp` & `scipp-24.5.0/lib/variable/slice.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/sort.cpp` & `scipp-24.5.0/lib/variable/sort.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/special_values.cpp` & `scipp-24.5.0/lib/variable/special_values.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/string.cpp` & `scipp-24.5.0/lib/variable/string.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/structures.cpp` & `scipp-24.5.0/lib/variable/structures.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/subspan_view.cpp` & `scipp-24.5.0/lib/variable/subspan_view.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/CMakeLists.txt` & `scipp-24.5.0/lib/variable/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/accumulate_test.cpp` & `scipp-24.5.0/lib/variable/test/accumulate_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/arithmetic_test.cpp` & `scipp-24.5.0/lib/variable/test/arithmetic_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/astype_test.cpp` & `scipp-24.5.0/lib/variable/test/astype_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/bin_array_model_test.cpp` & `scipp-24.5.0/lib/variable/test/bin_array_model_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/bin_util_test.cpp` & `scipp-24.5.0/lib/variable/test/bin_util_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/comparison_test.cpp` & `scipp-24.5.0/lib/variable/test/comparison_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/concat_test.cpp` & `scipp-24.5.0/lib/variable/test/concat_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/copy_test.cpp` & `scipp-24.5.0/lib/variable/test/copy_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/creation_test.cpp` & `scipp-24.5.0/lib/variable/test/creation_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/cumulative_test.cpp` & `scipp-24.5.0/lib/variable/test/cumulative_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/equals_nan_test.cpp` & `scipp-24.5.0/lib/variable/test/equals_nan_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/hyperbolic_test.cpp` & `scipp-24.5.0/lib/variable/test/hyperbolic_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/inv_test.cpp` & `scipp-24.5.0/lib/variable/test/inv_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/linalg_test.cpp` & `scipp-24.5.0/lib/variable/test/linalg_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/math_test.cpp` & `scipp-24.5.0/lib/variable/test/math_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/mean_test.cpp` & `scipp-24.5.0/lib/variable/test/mean_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/operations_test.cpp` & `scipp-24.5.0/lib/variable/test/operations_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/rebin_test.cpp` & `scipp-24.5.0/lib/variable/test/rebin_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/reduce_logical_test.cpp` & `scipp-24.5.0/lib/variable/test/reduce_logical_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/reduce_various_test.cpp` & `scipp-24.5.0/lib/variable/test/reduce_various_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/shape_test.cpp` & `scipp-24.5.0/lib/variable/test/shape_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/slice_test.cpp` & `scipp-24.5.0/lib/variable/test/slice_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/sort_test.cpp` & `scipp-24.5.0/lib/variable/test/sort_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/special_values_test.cpp` & `scipp-24.5.0/lib/variable/test/special_values_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/subspan_view_test.cpp` & `scipp-24.5.0/lib/variable/test/subspan_view_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/sum_test.cpp` & `scipp-24.5.0/lib/variable/test/sum_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/test_variables.cpp` & `scipp-24.5.0/lib/variable/test/test_variables.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/to_unit_test.cpp` & `scipp-24.5.0/lib/variable/test/to_unit_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/transform_binary_test.cpp` & `scipp-24.5.0/lib/variable/test/transform_binary_test.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -589,14 +589,24 @@
   auto b = make_bins(indicesB, Dim::Event, table);
   ASSERT_THROW_DISCARD(transform<pair_self_t<double>>(a, b, op, name),
                        except::BinnedDataError);
   ASSERT_THROW(transform_in_place<pair_self_t<double>>(a, b, op_in_place, name),
                except::BinnedDataError);
 }
 
+TEST_F(TransformBinaryTest, inplace_nonbinned_lhs_binned_rhs) {
+  auto a = makeVariable<double>(Dims{Dim::X}, Shape{2}, Values{1.0, 2.0});
+  const auto indices = makeVariable<std::pair<scipp::index, scipp::index>>(
+      Dims{Dim::X}, Shape{2}, Values{std::pair{0, 3}, std::pair{3, 3}});
+  const auto table = makeVariable<double>(Dims{Dim::Event}, Shape{4});
+  auto b = make_bins(indices, Dim::Event, table);
+  ASSERT_THROW(transform_in_place<pair_self_t<double>>(a, b, op_in_place, name),
+               except::BinnedDataError);
+}
+
 class TransformTest_events_binary_values_variances_size_fail
     : public ::testing::Test {
 protected:
   Variable indicesA = makeVariable<std::pair<scipp::index, scipp::index>>(
       Dims{Dim::X}, Shape{2}, Values{std::pair{0, 2}, std::pair{2, 4}});
   Variable indicesB = makeVariable<std::pair<scipp::index, scipp::index>>(
       Dims{Dim::X}, Shape{2}, Values{std::pair{0, 2}, std::pair{2, 3}});
```

### Comparing `scipp-24.2.0/lib/variable/test/transform_test.cpp` & `scipp-24.5.0/lib/variable/test/transform_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/transform_test_helpers.cpp` & `scipp-24.5.0/lib/variable/test/transform_test_helpers.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/transform_test_helpers.h` & `scipp-24.5.0/lib/variable/test/transform_test_helpers.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/transform_unary_test.cpp` & `scipp-24.5.0/lib/variable/test/transform_unary_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/trigonometry_test.cpp` & `scipp-24.5.0/lib/variable/test/trigonometry_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/util_test.cpp` & `scipp-24.5.0/lib/variable/test/util_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/variable_bin_test.cpp` & `scipp-24.5.0/lib/variable/test/variable_bin_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/variable_comparison_test.cpp` & `scipp-24.5.0/lib/variable/test/variable_comparison_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/variable_custom_type_test.cpp` & `scipp-24.5.0/lib/variable/test/variable_custom_type_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/variable_keyword_args_constructor_test.cpp` & `scipp-24.5.0/lib/variable/test/variable_keyword_args_constructor_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/variable_scalar_accessors_test.cpp` & `scipp-24.5.0/lib/variable/test/variable_scalar_accessors_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/variable_structure_test.cpp` & `scipp-24.5.0/lib/variable/test/variable_structure_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/test/variable_test.cpp` & `scipp-24.5.0/lib/variable/test/variable_test.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/to_unit.cpp` & `scipp-24.5.0/lib/variable/to_unit.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/util.cpp` & `scipp-24.5.0/lib/variable/util.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/variable.cpp` & `scipp-24.5.0/lib/variable/variable.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/variable_factory.cpp` & `scipp-24.5.0/lib/variable/variable_factory.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/variable_instantiate_basic.cpp` & `scipp-24.5.0/lib/variable/variable_instantiate_basic.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/variable_instantiate_bin_elements.cpp` & `scipp-24.5.0/lib/variable/variable_instantiate_bin_elements.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/variable_instantiate_linalg.cpp` & `scipp-24.5.0/lib/variable/variable_instantiate_linalg.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/variable_instantiate_map_elements.cpp` & `scipp-24.5.0/lib/variable/variable_instantiate_map_elements.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/lib/variable/variable_instantiate_view_elements.cpp` & `scipp-24.5.0/lib/variable/variable_instantiate_view_elements.cpp`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/requirements/build.txt` & `scipp-24.5.0/requirements/build.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/requirements/ci.txt` & `scipp-24.5.0/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/requirements/docs.txt` & `scipp-24.5.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/requirements/extra.txt` & `scipp-24.5.0/requirements/extra.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/requirements/static.txt` & `scipp-24.5.0/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/requirements/test.txt` & `scipp-24.5.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/resources/logo-2019-09-07.svg` & `scipp-24.5.0/resources/logo-2019-09-07.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/resources/logo-2021.svg` & `scipp-24.5.0/resources/logo-2021.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/resources/logo-2022.svg` & `scipp-24.5.0/resources/logo-2022.svg`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/src/scipp/__init__.py` & `scipp-24.5.0/src/scipp/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
-# flake8: noqa
+# ruff: noqa: E402, F401, F821
 """Multi-dimensional data arrays with labeled dimensions.
 
 Scipp provides
 
 * Physical units are stored with each data or coord array and are handled in arithmetic operations.
 * Histograms, i.e., bin-edge axes, which are by 1 longer than the data extent.
 * Support for non-regular or scattered data and non-destructive binning.
 * Support for masks stored with data.
 * Propagation of uncertainties.
 
 See the online documentation for user guides and an API reference: https://scipp.github.io/
-"""
+"""  # noqa: E501
 
 from .core import __version__
 
 # Import classes
 from .core import Variable, DataArray, DataGroup, Dataset, DType, Unit
 
 # Import errors
@@ -32,37 +32,36 @@
     UnitError,
     VariableError,
     VariancesError,
 )
 
 # Import submodules
 from . import units
-from . import geometry
 
 # Import functions
 
 # Import python functions
 from .visualization import show, make_svg, to_html, make_html, table
 
-setattr(Variable, '_repr_html_', make_html)
-setattr(DataArray, '_repr_html_', make_html)
-setattr(Dataset, '_repr_html_', make_html)
+Variable._repr_html_ = make_html
+DataArray._repr_html_ = make_html
+Dataset._repr_html_ = make_html
 del visualization
 
 from .io.hdf5 import save_hdf5 as _save_hdf5
 
-setattr(Variable, 'save_hdf5', _save_hdf5)
-setattr(DataArray, 'save_hdf5', _save_hdf5)
-setattr(Dataset, 'save_hdf5', _save_hdf5)
-setattr(DataGroup, 'save_hdf5', _save_hdf5)
+Variable.save_hdf5 = _save_hdf5
+DataArray.save_hdf5 = _save_hdf5
+Dataset.save_hdf5 = _save_hdf5
+DataGroup.save_hdf5 = _save_hdf5
 del _save_hdf5
 
 from .format import format_variable as _format_variable
 
-setattr(Variable, '__format__', _format_variable)
+Variable.__format__ = _format_variable
 del _format_variable
 
 from ._extend_units import extend_units
 
 extend_units()
 del extend_units
 
@@ -244,21 +243,19 @@
 
 from . import data
 from . import spatial
 from .operations import elemwise_func
 
 del operations
 
-from .core.binning import histogram
-
 from .plotting import plot
 
-setattr(Variable, 'plot', plot)
-setattr(DataArray, 'plot', plot)
-setattr(Dataset, 'plot', plot)
+Variable.plot = plot
+DataArray.plot = plot
+Dataset.plot = plot
 del plotting
 
 from .core.util import VisibleDeprecationWarning
 
 del core
 
 from .curve_fit import curve_fit
@@ -337,15 +334,14 @@
     'floor',
     'floor_divide',
     'fold',
     'format',
     'from_dict',
     'full',
     'full_like',
-    'geometry',
     'geomspace',
     'get_logger',
     'greater',
     'greater_equal',
     'group',
     'groupby',
     'hist',
```

### Comparing `scipp-24.2.0/src/scipp/_extend_units.py` & `scipp-24.5.0/src/scipp/_extend_units.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/src/scipp/compat/dict.py` & `scipp-24.5.0/src/scipp/compat/dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,22 @@
 
 from __future__ import annotations
 
 from collections import defaultdict
 
 import numpy as np
 
-from ..core import vectors  # NOQA
-from ..core import DataArray, Dataset, DType, Variable, vector
+from ..core import (
+    DataArray,
+    Dataset,
+    DType,
+    Variable,
+    vector,
+    vectors,
+)
 from ..spatial import linear_transform, linear_transforms
 from ..typing import VariableLike
 
 
 def to_dict(scipp_obj: VariableLike) -> dict:
     """Convert a Scipp object (Variable, DataArray or Dataset)
     to a Python :class:`dict`.
@@ -180,15 +186,15 @@
 
 def _dict_to_data_array(d):
     """Convert a Python dict to a Scipp DataArray."""
     d = dict(d)
     if "data" not in d:
         raise KeyError(
             "To create a DataArray, the supplied dict must contain "
-            "'data'. Got {}.".format(d.keys())
+            f"'data'. Got {d.keys()}."
         )
     out = {"coords": {}, "masks": {}, "attrs": {}}
     for key in out.keys():
         if key in d:
             for name, item in d[key].items():
                 out[key][name] = _dict_to_variable(item)
     out["data"] = _dict_to_variable(d["data"])
```

### Comparing `scipp-24.2.0/src/scipp/compat/pandas_compat.py` & `scipp-24.5.0/src/scipp/compat/pandas_compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Callable, Iterable, Literal, Optional, Tuple, Union
+from collections.abc import Callable, Iterable
+from typing import TYPE_CHECKING, Literal
 
 from ..core import DataArray, Dataset, Unit, UnitError, array
 from ..typing import VariableLike
 from ..units import default_unit
 
 if TYPE_CHECKING:
     import pandas as pd
@@ -52,15 +53,15 @@
         name=name,
     )
 
 
 def from_pandas_dataframe(
     df: pd.DataFrame,
     *,
-    data_columns: Optional[Union[str, Iterable[str]]] = None,
+    data_columns: str | Iterable[str] | None = None,
     include_trivial_index: bool = False,
     header_parser: HeaderParserArg = None,
 ) -> Dataset:
     import pandas as pd
 
     columns = (
         from_pandas_series(
@@ -81,17 +82,17 @@
         data = {name: coords.pop(name) for name in data_columns}
         coords = {name: coord.data for name, coord in coords.items()}
 
     return Dataset(data, coords=coords)
 
 
 def from_pandas(
-    pd_obj: Union[pd.DataFrame, pd.Series],
+    pd_obj: pd.DataFrame | pd.Series,
     *,
-    data_columns: Optional[Union[str, Iterable[str]]] = None,
+    data_columns: str | Iterable[str] | None = None,
     include_trivial_index: bool = False,
     header_parser: HeaderParserArg = None,
 ) -> VariableLike:
     """Converts a pandas.DataFrame or pandas.Series object into a
     scipp Dataset or DataArray respectively.
 
     Parameters
@@ -142,19 +143,19 @@
             include_trivial_index=include_trivial_index,
             header_parser=header_parser,
         )
     else:
         raise ValueError(f"from_pandas: cannot convert type '{type(pd_obj)}'")
 
 
-HeaderParser = Callable[[str], Tuple[str, Optional[Unit]]]
-HeaderParserArg = Optional[Union[Literal["bracket"], HeaderParser]]
+HeaderParser = Callable[[str], tuple[str, Unit | None]]
+HeaderParserArg = Literal["bracket"] | HeaderParser | None
 
 
-def parse_bracket_header(head: str) -> Tuple[str, Optional[Unit]]:
+def parse_bracket_header(head: str) -> tuple[str, Unit | None]:
     """Parses strings of the form ``name [unit]``.
 
     ``name`` may be any string that does not contain the character ``[``.
     And ``unit`` must be a valid unit string to be parsed by ``sc.Unit(unit)``.
     Whitespace between the name and unit is removed.
 
     Both name and unit, including brackets, are optional.
@@ -203,15 +204,15 @@
 
 
 _HEADER_PARSERS = {
     "bracket": parse_bracket_header,
 }
 
 
-def _parse_header(header: str, parser: HeaderParserArg) -> Tuple[str, Optional[Unit]]:
+def _parse_header(header: str, parser: HeaderParserArg) -> tuple[str, Unit | None]:
     if parser is None:
         return header, default_unit
     if callable(parser):
         return parser(header)
     if (parser := _HEADER_PARSERS.get(parser)) is not None:
         return parser(header)
     else:
```

### Comparing `scipp-24.2.0/src/scipp/compat/xarray_compat.py` & `scipp-24.5.0/src/scipp/compat/xarray_compat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING
 from warnings import warn
 
 from ..core import DataArray, Dataset, Unit, Variable
 from ..typing import VariableLike
 from ..units import default_unit
 
 if TYPE_CHECKING:
     import xarray as xr
 
 
-def from_xarray(obj: Union[xr.Variable, xr.DataArray, xr.Dataset]) -> VariableLike:
+def from_xarray(obj: xr.Variable | xr.DataArray | xr.Dataset) -> VariableLike:
     """Convert an xarray object to the corresponding scipp object.
     Attributes named `"units"` are used to set the units of the Variables.
     All other DataArray attributes are kept, but attributes of Variables, Coordinates
     and Datasets are dropped.
 
     Parameters
     ----------
@@ -42,15 +42,15 @@
         return _from_xarray_dataarray(obj)
     elif isinstance(obj, xr.Dataset):
         return _from_xarray_dataset(obj)
     else:
         raise ValueError(f"from_xarray: cannot convert type '{type(obj)}'")
 
 
-def to_xarray(obj: VariableLike) -> Union[xr.Variable, xr.DataArray, xr.Dataset]:
+def to_xarray(obj: VariableLike) -> xr.Variable | xr.DataArray | xr.Dataset:
     """Convert a scipp object to the corresponding xarray object.
 
     Warning
     -------
     Any masks and variances in the input will be stripped during the conversion.
     Binned data is not supported.
 
@@ -75,15 +75,15 @@
         return _to_xarray_dataarray(obj)
     elif isinstance(obj, Dataset):
         return _to_xarray_dataset(obj)
     else:
         raise ValueError(f"to_xarray: cannot convert type '{type(obj)}'")
 
 
-def _from_xarray_variable(xr_obj: Union[xr.Coordinate, xr.DataArray]) -> Variable:
+def _from_xarray_variable(xr_obj: xr.Coordinate | xr.DataArray) -> Variable:
     """Converts an xarray Coordinate or the data in a DataArray to a scipp.Variable."""
     unit = xr_obj.attrs.get('units', None)
     return Variable(
         dims=xr_obj.dims,
         values=xr_obj.values,
         unit=Unit(unit) if unit is not None else default_unit,
     )
@@ -94,25 +94,29 @@
     in either an xarray Coordinate or DataArray.
     """
     import xarray as xr
 
     if var.bins is not None:
         raise ValueError("Xarray does not support binned data.")
     if var.variances is not None:
-        warn("Variances of variable were stripped when converting to Xarray.")
+        warn(
+            "Variances of variable were stripped when converting to Xarray.",
+            stacklevel=3,
+        )
     attrs = {'units': str(var.unit)} if var.unit is not None else None
     return xr.Variable(dims=var.dims, data=var.values, attrs=attrs)
 
 
 def _from_xarray_dataarray(da: xr.DataArray) -> DataArray:
     """Converts an xarray.DataArray object to a scipp.DataArray object."""
     if da.attrs and set(da.attrs) != {"units"}:
         warn(
             "Input data contains some attributes which have been dropped during the "
-            "conversion."
+            "conversion.",
+            stacklevel=3,
         )
     coords = {
         f"{name}": _from_xarray_variable(coord) for name, coord in da.coords.items()
     }
     scipp_da = DataArray(
         data=_from_xarray_variable(da),
         coords=coords,
@@ -127,15 +131,16 @@
 def _to_xarray_dataarray(da: DataArray) -> xr.DataArray:
     """Converts a scipp.DataArray object to an xarray.DataArray object."""
     import xarray as xr
 
     if da.masks:
         warn(
             "Some masks were found in the DataArray. "
-            "These have been removed when converting to Xarray."
+            "These have been removed when converting to Xarray.",
+            stacklevel=3,
         )
     out = xr.DataArray(_to_xarray_variable(da.data))
     for key, coord in da.coords.items():
         for dim in coord.dims:
             if da.meta.is_edges(key, dim=dim):
                 raise ValueError("Xarray does not support coordinates with bin edges.")
         out.coords[key] = _to_xarray_variable(coord)
@@ -144,15 +149,16 @@
 
 
 def _from_xarray_dataset(ds: xr.Dataset) -> Dataset:
     """Converts an xarray.Dataset object to a scipp.Dataset object."""
     if ds.attrs:
         warn(
             "Input data contains some attributes which have been dropped during the "
-            "conversion."
+            "conversion.",
+            stacklevel=3,
         )
     sc_data = {k: _from_xarray_dataarray(v) for k, v in ds.items()}
     # The non-indexed coordinates of items also show up as global coordinates in an
     # Xarray dataset, so we make sure we exclude those when we add the remaining coords,
     # after creating the dataset from the individual data arrays.
     coords_in_data_arrays = []
     for item in ds.values():
```

### Comparing `scipp-24.2.0/src/scipp/constants/__init__.py` & `scipp-24.5.0/src/scipp/constants/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# flake8: noqa: E501
+# ruff: noqa: E501
 r"""
 Physical and mathematical constants with units.
 This module a wrapper around `scipy.constants <https://docs.scipy.org/doc/scipy/reference/constants.html>`_
 and requires the ``scipy`` package to be installed.
 
 Mathematical constants:
 
@@ -53,14 +53,15 @@
 constants.
 The database is accessed using :py:func:`scipp.constants.physical_constants`.
 
 .. [CODATA2018] CODATA Recommended Values of the Fundamental
    Physical Constants 2018.
    https://physics.nist.gov/cuu/Constants/
 """
+
 import math as _math
 
 from .. import Variable, as_const, scalar
 
 
 def physical_constants(key: str, with_variance: bool = False) -> Variable:
     """
```

### Comparing `scipp-24.2.0/src/scipp/coords/coord.py` & `scipp-24.5.0/src/scipp/coords/coord.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Jan-Lukas Wynen
 
 import dataclasses
-from typing import Optional
 
 from ..core import Variable
 
 
 @dataclasses.dataclass
 class Coord:
-    dense: Optional[Variable]  # for dense variable or bin-coord
-    event: Optional[Variable]
+    dense: Variable | None  # for dense variable or bin-coord
+    event: Variable | None
     aligned: bool
     usages: int = -1  # negative for unlimited usages
 
     @property
     def has_dense(self) -> bool:
         return self.dense is not None
```

### Comparing `scipp-24.2.0/src/scipp/coords/coord_table.py` & `scipp-24.5.0/src/scipp/coords/coord_table.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Jan-Lukas Wynen
 
 import dataclasses
-from typing import Dict, Iterable, List, Set, Tuple
+from collections.abc import Iterable
 
 from .coord import Coord
 from .options import Options
 from .rule import FetchRule, RenameRule, Rule, rule_output_names
 
 
 class CoordTable:
     """
     Stores a dictionary of coordinates for use in coord transforms.
 
     Coords have an associated number of usages.
     When that number drops to 0, the coord is removed.
     """
 
-    def __init__(self, rules: List[Rule], targets: Set[str], options: Options):
+    def __init__(self, rules: list[Rule], targets: set[str], options: Options):
         self._coords = {}
         self._total_usages = _apply_keep_options(
             _count_usages(rules), rules, targets, options
         )
         # Preserve all targets regardless of keep_* options.
         for name in targets:
             self._total_usages[name] = -1
@@ -39,42 +39,42 @@
             # But the caller of `consume` does need it, so return `coord` as is.
             self._coords[name] = dataclasses.replace(coord, dense=None, event=None)
         return coord
 
     def total_usages(self, name: str) -> int:
         return self._total_usages.get(name, -1)
 
-    def items(self) -> Iterable[Tuple[str, Coord]]:
+    def items(self) -> Iterable[tuple[str, Coord]]:
         yield from self._coords.items()
 
 
-def _count_usages(rules: List[Rule]) -> Dict[str, int]:
+def _count_usages(rules: list[Rule]) -> dict[str, int]:
     usages = {}
     for rule in rules:
         for name in rule.dependencies:
             usages.setdefault(name, 0)
             usages[name] += 1
     return usages
 
 
 def _apply_keep_options(
-    usages: Dict[str, int], rules: List[Rule], targets: Set[str], options: Options
-) -> Dict[str, int]:
+    usages: dict[str, int], rules: list[Rule], targets: set[str], options: Options
+) -> dict[str, int]:
     def out_names(rule_type):
         yield from filter(
             lambda name: name not in targets, rule_output_names(rules, rule_type)
         )
 
     def handle_in(names):
         for name in names:
             usages[name] = -1
 
     inputs = set(out_names(FetchRule))
     aliases = set(out_names(RenameRule))
-    all_inputs = set(dep for rule in rules for dep in rule.dependencies)
+    all_inputs = {dep for rule in rules for dep in rule.dependencies}
     if options.keep_inputs:
         handle_in(inputs)
     if options.keep_intermediate:
         handle_in(all_inputs - inputs - aliases)
     if options.keep_aliases:
         handle_in(aliases)
     return usages
```

### Comparing `scipp-24.2.0/src/scipp/coords/graph.py` & `scipp-24.5.0/src/scipp/coords/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock, Jan-Lukas Wynen
 
 from __future__ import annotations
 
 import collections
+from collections.abc import Callable, Iterable
 from graphlib import TopologicalSorter
-from typing import Callable, Dict, Iterable, List, Set, Tuple, Union
 
 from ..core import DataArray
 from ..utils.graph import make_graphviz_digraph
 from .rule import ComputeRule, FetchRule, RenameRule, Rule
 
-GraphDict = Dict[Union[str, Tuple[str, ...]], Union[str, Callable]]
+GraphDict = dict[str | tuple[str, ...], str | Callable]
 
 
 class Graph:
-    def __init__(self, graph: Union[GraphDict, Dict[str, Rule]]):
+    def __init__(self, graph: GraphDict | dict[str, Rule]):
         if not isinstance(graph, collections.abc.Mapping):
             raise TypeError("'graph' must be a dict")
         if not graph:
             self._rules = {}
         elif isinstance(next(iter(graph.values())), Rule):
-            self._rules: Dict[str, Rule] = graph
+            self._rules: dict[str, Rule] = graph
         else:
-            self._rules: Dict[str, Rule] = _convert_to_rule_graph(graph)
+            self._rules: dict[str, Rule] = _convert_to_rule_graph(graph)
 
     def __getitem__(self, name: str) -> Rule:
         return self._rules[name]
 
-    def items(self) -> Iterable[Tuple[str, Rule]]:
+    def items(self) -> Iterable[tuple[str, Rule]]:
         yield from self._rules.items()
 
     def parents_of(self, node: str) -> Iterable[str]:
         try:
             yield from self._rules[node].dependencies
         except KeyError:
             # Input nodes have no parents but are not represented in the
@@ -49,15 +49,15 @@
         yield from self._rules.keys()
 
     def nodes_topologically(self) -> Iterable[str]:
         yield from TopologicalSorter(
             {out: rule.dependencies for out, rule in self._rules.items()}
         ).static_order()
 
-    def graph_for(self, da: DataArray, targets: Set[str]) -> Graph:
+    def graph_for(self, da: DataArray, targets: set[str]) -> Graph:
         """
         Construct a graph containing only rules needed for the given DataArray
         and targets, including FetchRules for the inputs.
         """
         subgraph = {}
         depth_first_stack = list(targets)
         while depth_first_stack:
@@ -105,33 +105,32 @@
                 else:
                     name = output
                 for arg in rule.dependencies:
                     dot.edge(arg, name)
         return dot
 
 
-def rule_sequence(rules: Graph) -> List[Rule]:
+def rule_sequence(rules: Graph) -> list[Rule]:
     already_used = set()
     result = []
-    for rule in filter(
-        lambda r: r not in already_used,
-        map(lambda n: rules[n], rules.nodes_topologically()),
+    for rule in (
+        r for n in rules.nodes_topologically() if (r := rules[n]) not in already_used
     ):
         already_used.add(rule)
         result.append(rule)
     return result
 
 
 def _make_rule(products, producer) -> Rule:
     if isinstance(producer, str):
         return RenameRule(products, producer)
     return ComputeRule(products, producer)
 
 
-def _convert_to_rule_graph(graph: GraphDict) -> Dict[str, Rule]:
+def _convert_to_rule_graph(graph: GraphDict) -> dict[str, Rule]:
     rule_graph = {}
     for products, producer in graph.items():
         products = (products,) if isinstance(products, str) else tuple(products)
         rule = _make_rule(products, producer)
         for product in products:
             if product in rule_graph:
                 raise ValueError(
```

### Comparing `scipp-24.2.0/src/scipp/coords/rule.py` & `scipp-24.5.0/src/scipp/coords/rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 They provide a common interface for renaming and computing new coordinates.
 """
 
 from __future__ import annotations
 
 import inspect
 from abc import ABC, abstractmethod
+from collections.abc import Callable, Iterable, Mapping
 from copy import copy
 from functools import partial
-from typing import Any, Callable, Dict, Iterable, List, Mapping, Tuple
+from typing import Any
 
 from ..core import Variable
 from .coord import Coord
 
 try:
     from typing import Protocol as _Protocol
 
@@ -30,24 +31,24 @@
 
 except ImportError:
     _Protocol = object
     _CoordProvider = Any
 
 
 class Rule(ABC):
-    def __init__(self, out_names: Tuple[str, ...]):
+    def __init__(self, out_names: tuple[str, ...]):
         self.out_names = out_names
 
     @abstractmethod
-    def __call__(self, coords: _CoordProvider) -> Dict[str, Coord]:
+    def __call__(self, coords: _CoordProvider) -> dict[str, Coord]:
         """Evaluate the rule."""
 
     @property
     @abstractmethod
-    def dependencies(self) -> Tuple[str]:
+    def dependencies(self) -> tuple[str]:
         """Return names of coords that this rule needs as inputs."""
 
     def _format_out_names(self):
         return f'({", ".join(self.out_names)})'
 
 
 class FetchRule(Rule):
@@ -55,75 +56,75 @@
     Get coords from the provided dict-like sources.
 
     Can be used to abstract away retrieving coords from the input DataArray.
     """
 
     def __init__(
         self,
-        out_names: Tuple[str, ...],
+        out_names: tuple[str, ...],
         dense_sources: Mapping[str, Variable],
         event_sources: Mapping[str, Variable],
     ):
         super().__init__(out_names)
         self._dense_sources = dense_sources
         self._event_sources = event_sources
 
-    def __call__(self, coords: _CoordProvider) -> Dict[str, Coord]:
+    def __call__(self, coords: _CoordProvider) -> dict[str, Coord]:
         return {
             out_name: Coord(
                 dense=self._dense_sources.get(out_name, None),
                 event=self._event_sources.get(out_name, None),
                 aligned=True,
             )
             for out_name in self.out_names
         }
 
     @property
-    def dependencies(self) -> Tuple[str]:
-        return ()  # type: ignore
+    def dependencies(self) -> tuple[str, ...]:
+        return ()
 
     def __str__(self):
         return f'Input   {self._format_out_names()}'
 
 
 class RenameRule(Rule):
     """
     Return the input coordinate and give it a new name.
     """
 
-    def __init__(self, out_names: Tuple[str, ...], in_name: str):
+    def __init__(self, out_names: tuple[str, ...], in_name: str):
         super().__init__(out_names)
         self._in_name = in_name
 
-    def __call__(self, coords: _CoordProvider) -> Dict[str, Coord]:
+    def __call__(self, coords: _CoordProvider) -> dict[str, Coord]:
         # Shallow copy the _Coord object to allow the alias to have
         # a different alignment and usage count than the original.
         return {
             out_name: copy(coords.consume(self._in_name)) for out_name in self.out_names
         }
 
     @property
-    def dependencies(self) -> Tuple[str]:
-        return tuple((self._in_name,))
+    def dependencies(self) -> tuple[str, ...]:
+        return (self._in_name,)
 
     def __str__(self):
         return f'Rename  {self._format_out_names()} <- {self._in_name}'
 
 
 class ComputeRule(Rule):
     """
     Compute new coordinates using the provided callable.
     """
 
-    def __init__(self, out_names: Tuple[str, ...], func: Callable):
+    def __init__(self, out_names: tuple[str, ...], func: Callable):
         super().__init__(out_names)
         self._func = func
         self._arg_names = _arg_names(func)
 
-    def __call__(self, coords: _CoordProvider) -> Dict[str, Coord]:
+    def __call__(self, coords: _CoordProvider) -> dict[str, Coord]:
         inputs = {
             name: coords.consume(coord) for coord, name in self._arg_names.items()
         }
         outputs = None
         if any(coord.has_event for coord in inputs.values()):
             outputs = self._compute_with_events(inputs)
         if all(coord.has_dense for coord in inputs.values()):
@@ -157,36 +158,36 @@
                 event=var if var.bins is not None else None,
                 aligned=True,
             )
             for name, var in outputs.items()
         }
         return outputs
 
-    def _without_unrequested(self, d: Dict[str, Any]) -> Dict[str, Any]:
+    def _without_unrequested(self, d: dict[str, Any]) -> dict[str, Any]:
         missing_outputs = [key for key in self.out_names if key not in d]
         if missing_outputs:
             raise TypeError(
                 f'transform_coords was expected to compute {missing_outputs} '
                 f'using `{self._func.__name__}` but the function returned '
                 f'{list(d.keys())} instead.'
             )
         return {key: d[key] for key in self.out_names}
 
-    def _to_dict(self, output) -> Dict[str, Variable]:
+    def _to_dict(self, output) -> dict[str, Variable]:
         if not isinstance(output, dict):
             if len(self.out_names) != 1:
                 raise TypeError(
                     'Function returned a single output but '
                     f'{len(self.out_names)} were expected.'
                 )
             return {self.out_names[0]: output}
         return output
 
     @property
-    def dependencies(self) -> Tuple[str]:
+    def dependencies(self) -> tuple[str, ...]:
         return tuple(self._arg_names)
 
     @property
     def func_name(self) -> str:
         return self._func.__name__
 
     def __str__(self):
@@ -195,32 +196,32 @@
         name = getattr(self._func, '__name__', repr(self._func))
         return (
             f'Compute {self._format_out_names()} = {name}'
             f'({", ".join(self.dependencies)})'
         )
 
 
-def rules_of_type(rules: List[Rule], rule_type: type) -> Iterable[Rule]:
+def rules_of_type(rules: list[Rule], rule_type: type) -> Iterable[Rule]:
     yield from filter(lambda rule: isinstance(rule, rule_type), rules)
 
 
-def rule_output_names(rules: List[Rule], rule_type: type) -> Iterable[str]:
+def rule_output_names(rules: list[Rule], rule_type: type) -> Iterable[str]:
     for rule in rules_of_type(rules, rule_type):
         yield from rule.out_names
 
 
-def _arg_names(func) -> Dict[str, str]:
+def _arg_names(func) -> dict[str, str]:
     spec = inspect.getfullargspec(func)
     if spec.varargs is not None or spec.varkw is not None:
         raise ValueError(
             'Function with variable arguments not allowed in '
             f'conversion graph: `{func.__name__}`.'
         )
     if inspect.isfunction(func) or func.__class__ == partial:
         args = spec.args
     else:
         # Strip off the 'self'. Objects returned by functools.partial are not
         # functions, but nevertheless do not have 'self'.
         args = spec.args[1:]
     names = tuple(args + spec.kwonlyargs)
     coords = getattr(func, '__transform_coords_input_keys__', names)
-    return dict(zip(coords, names))
+    return dict(zip(coords, names, strict=True))
```

### Comparing `scipp-24.2.0/src/scipp/coords/transform_coords.py` & `scipp-24.5.0/src/scipp/coords/transform_coords.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock, Jan-Lukas Wynen
+from collections.abc import Callable, Iterable, Mapping
 from dataclasses import fields
 from fractions import Fraction
-from typing import Callable, Dict, Iterable, List, Mapping, Optional, Set, Union
 
 from ..core import DataArray, Dataset, DimensionError, VariableError, bins, empty
 from ..logging import get_logger
 from .coord_table import Coord, CoordTable
 from .graph import Graph, GraphDict, rule_sequence
 from .options import Options
 from .rule import ComputeRule, FetchRule, RenameRule, Rule, rule_output_names
 
 
 def transform_coords(
-    x: Union[DataArray, Dataset],
-    targets: Optional[Union[str, Iterable[str]]] = None,
+    x: DataArray | Dataset,
+    targets: str | Iterable[str] | None = None,
     /,
-    graph: Optional[GraphDict] = None,
+    graph: GraphDict | None = None,
     *,
     rename_dims: bool = True,
     keep_aliases: bool = True,
     keep_intermediate: bool = True,
     keep_inputs: bool = True,
     quiet: bool = False,
     **kwargs: Callable,
-) -> Union[DataArray, Dataset]:
+) -> DataArray | Dataset:
     """Compute new coords based on transformations of input coords.
 
     See the section in the user guide on
     `Coordinate transformations <../../user-guide/coordinate-transformations.rst>`_
     for detailed explanations.
 
     Parameters
@@ -140,15 +140,15 @@
     else:
         targets = {targets} if isinstance(targets, str) else set(targets)
 
     _transform = _transform_dataset if isinstance(x, Dataset) else _transform_data_array
     return _transform(x, targets=targets, graph=Graph(graph), options=options)
 
 
-def show_graph(graph: GraphDict, size: str = None, simplified: bool = False):
+def show_graph(graph: GraphDict, size: str | None = None, simplified: bool = False):
     """Show graphical representation of a graph as required by
     :py:func:`transform_coords`
 
     Requires the `python-graphviz` package.
 
     Parameters
     ----------
@@ -170,20 +170,20 @@
         `documentation <https://graphviz.readthedocs.io/en/stable/api.html#graphviz.Digraph>`_
         for details.
 
     Raises
     ------
     RuntimeError
         If graphviz is not installed.
-    """  # noqa
+    """
     return Graph(graph).show(size=size, simplified=simplified)
 
 
 def _transform_data_array(
-    original: DataArray, targets: Set[str], graph: Graph, options: Options
+    original: DataArray, targets: set[str], graph: Graph, options: Options
 ) -> DataArray:
     graph = graph.graph_for(original, targets)
     rules = rule_sequence(graph)
     working_coords = CoordTable(rules, targets, options)
     dim_coords = set()
     for rule in rules:
         for name, coord in rule(working_coords).items():
@@ -200,15 +200,15 @@
     if not options.quiet:
         _log_transform(rules, targets, dim_name_changes, working_coords)
     res = _store_results(original, working_coords, targets)
     return res.rename_dims(dim_name_changes)
 
 
 def _transform_dataset(
-    original: Dataset, targets: Set[str], graph: Graph, *, options: Options
+    original: Dataset, targets: set[str], graph: Graph, *, options: Options
 ) -> Dataset:
     # Note the inefficiency here in datasets with multiple items: Coord transform is
     # repeated for every item rather than sharing what is possible. Since we may have
     # dataset items with binned data this is far from trivial. Unless we have clear
     # performance requirements, we go with the safe and simple solution.
     if len(original) > 0:
         return Dataset(
@@ -223,16 +223,16 @@
     transformed = _transform_data_array(
         dummy, targets=targets, graph=graph, options=options
     )
     return Dataset(coords=transformed.coords)
 
 
 def _log_transform(
-    rules: List[Rule],
-    targets: Set[str],
+    rules: list[Rule],
+    targets: set[str],
     dim_name_changes: Mapping[str, str],
     coords: CoordTable,
 ) -> None:
     inputs = set(rule_output_names(rules, FetchRule))
     byproducts = {
         name
         for name in (
@@ -288,27 +288,27 @@
                 store(da.bins, coord.event)
             except (DimensionError, VariableError):
                 # Thrown on mismatching bin indices, e.g. slice
                 da.data = da.data.copy()
                 store(da.bins, coord.event)
 
 
-def _store_results(da: DataArray, coords: CoordTable, targets: Set[str]) -> DataArray:
+def _store_results(da: DataArray, coords: CoordTable, targets: set[str]) -> DataArray:
     da = da.copy(deep=False)
     # See #2773 for why this is necessary.
     if da.bins is not None:
         da.data = bins(**da.bins.constituents)
     for name, coord in coords.items():
         if name in targets:
             coord.aligned = True
         _store_coord(da, name, coord)
     return da
 
 
-def _color_dims(graph: Graph, dim_coords: Set[str]) -> Dict[str, Dict[str, Fraction]]:
+def _color_dims(graph: Graph, dim_coords: set[str]) -> dict[str, dict[str, Fraction]]:
     colors = {
         coord: {dim: Fraction(0, 1) for dim in dim_coords} for coord in graph.nodes()
     }
     for dim in dim_coords:
         colors[dim][dim] = Fraction(1, 1)
         depth_first_stack = [dim]
         while depth_first_stack:
@@ -321,21 +321,21 @@
                         1, len(children)
                     )
             depth_first_stack.extend(children)
 
     return colors
 
 
-def _has_full_color_of_dim(colors: Dict[str, Fraction], dim: str) -> bool:
+def _has_full_color_of_dim(colors: dict[str, Fraction], dim: str) -> bool:
     return all(
         fraction == 1 if d == dim else fraction != 1 for d, fraction in colors.items()
     )
 
 
-def _dim_name_changes(rule_graph: Graph, dim_coords: Set[str]) -> Dict[str, str]:
+def _dim_name_changes(rule_graph: Graph, dim_coords: set[str]) -> dict[str, str]:
     colors = _color_dims(rule_graph, dim_coords)
     nodes = list(rule_graph.nodes_topologically())[::-1]
     name_changes = {}
     for dim in dim_coords:
         for node in nodes:
             if _has_full_color_of_dim(colors[node], dim):
                 name_changes[dim] = node
```

### Comparing `scipp-24.2.0/src/scipp/core/__init__.py` & `scipp-24.5.0/src/scipp/core/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
 
-# flake8: noqa
+# ruff: noqa: E402, F401, F403, F821
 from .._scipp import _debug_
 
 if _debug_:
     import warnings
 
     warnings.warn(
-        'You are running a "Debug" build of Scipp. For optimal performance use a "Release" build.'
+        'You are running a "Debug" build of Scipp. '
+        'For optimal performance use a "Release" build.',
+        stacklevel=1,
     )
     del warnings
 del _debug_
 
 from .._scipp import __version__
 from .cpp_classes import (
     Coords,
     DataArray,
     Dataset,
+    DefaultUnit,
     DType,
     GroupByDataArray,
     GroupByDataset,
     Masks,
     Unit,
     Variable,
 )
@@ -50,55 +53,48 @@
     _rename_data_array,
     _rename_dataset,
 )
 
 
 from .deprecation import _deprecated_attrs, _deprecated_meta, _deprecated_drop_attrs
 
-setattr(DataArray, 'attrs', property(_deprecated_attrs))
-setattr(DataArray, 'meta', property(_deprecated_meta))
-setattr(DataArray, 'drop_attrs', _deprecated_drop_attrs)
+DataArray.attrs = property(_deprecated_attrs)
+DataArray.meta = property(_deprecated_meta)
+DataArray.drop_attrs = _deprecated_drop_attrs
 del _deprecated_attrs, _deprecated_meta, _deprecated_drop_attrs
 
 for cls in (Variable, DataArray, Dataset):
-    setattr(cls, 'rename_dims', _rename_dims)
-setattr(Variable, 'rename', _rename_variable)
-setattr(DataArray, 'rename', _rename_data_array)
-setattr(Dataset, 'rename', _rename_dataset)
+    cls.rename_dims = _rename_dims
+Variable.rename = _rename_variable
+DataArray.rename = _rename_data_array
+Dataset.rename = _rename_dataset
 del _rename_dims, _rename_variable, _rename_data_array, _rename_dataset, cls
 
 from .bins import _bins, _set_bins
 
-setattr(Variable, 'bins', property(_bins, _set_bins))
-setattr(DataArray, 'bins', property(_bins, _set_bins))
-setattr(Dataset, 'bins', property(_bins, _set_bins))
+Variable.bins = property(_bins, _set_bins)
+DataArray.bins = property(_bins, _set_bins)
+Dataset.bins = property(_bins, _set_bins)
 
 from .structured import _fields
 
-setattr(
-    Variable,
-    'fields',
-    property(
-        _fields,
-        doc="""Provides access to fields of structured types such as vectors or matrices.""",
-    ),
+Variable.fields = property(
+    _fields,
+    doc='Provides access to fields of structured types such as vectors or matrices.',
 )
+del _fields
 
-from .bins import _groupby_bins, Bins
-
-setattr(GroupByDataArray, 'bins', property(_groupby_bins))
-setattr(GroupByDataset, 'bins', property(_groupby_bins))
-del _groupby_bins
+from .bins import Bins
 
 # Prevent unwanted conversion to numpy arrays by operations. Properly defining
 # __array_ufunc__ should be possible by converting non-scipp arguments to
 # variables. The most difficult part is probably mapping the ufunc to scipp
 # functions.
 for _cls in (Variable, DataArray, Dataset):
-    setattr(_cls, '__array_ufunc__', None)
+    _cls.__array_ufunc__ = None
 del _cls
 
 
 from .arithmetic import add, divide, floor_divide, mod, multiply, negative, subtract
 from .binning import bin, group, hist, nanhist, rebin
 from .bins import Lookup, lookup, bins, bins_like
 from .comparison import (
@@ -189,18 +185,18 @@
     datetimes,
     epoch,
 )
 from .like import zeros_like, ones_like, empty_like, full_like
 
 from .assignments import assign_coords, assign_masks, assign_attrs
 
-setattr(Dataset, 'assign_coords', assign_coords)
-setattr(DataArray, 'assign_coords', assign_coords)
-setattr(DataArray, 'assign_masks', assign_masks)
-setattr(DataArray, 'assign_attrs', assign_attrs)
+Dataset.assign_coords = assign_coords
+DataArray.assign_coords = assign_coords
+DataArray.assign_masks = assign_masks
+DataArray.assign_attrs = assign_attrs
 del assign_coords, assign_masks, assign_attrs
 
 # Remove submodules to reduce clutter
 del (
     arithmetic,
     assignments,
     binning,
@@ -232,14 +228,15 @@
     'DType',
     'DTypeError',
     'DataArray',
     'DataArrayError',
     'DataGroup',
     'Dataset',
     'DatasetError',
+    'DefaultUnit',
     'DimensionError',
     'GroupByDataArray',
     'GroupByDataset',
     'Lookup',
     'Masks',
     'Unit',
     'UnitError',
```

### Comparing `scipp-24.2.0/src/scipp/core/_sizes.py` & `scipp-24.5.0/src/scipp/core/_sizes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-from typing import Dict, List, Optional, Sequence, Tuple, Union
+from collections.abc import Sequence
+from typing import Any
 
 
 def _parse_dims_shape_sizes(
-    dims: Optional[Union[List[str], Tuple[str, ...]]] = None,
-    shape: Optional[Sequence[int]] = None,
-    sizes: Optional[Dict[str, int]] = None,
-):
+    dims: Sequence[str] | None = None,
+    shape: Sequence[int] | None = None,
+    sizes: dict[str, int] | None = None,
+) -> dict[str, Any]:
     if sizes is not None:
         if dims is not None or shape is not None:
             raise ValueError(
                 "When sizes is specified, dims and shape must "
-                "both be None. Got dims: {}, shape: {}".format(dims, shape)
+                f"both be None. Got dims: {dims}, shape: {shape}"
             )
         dims = list(sizes.keys())
         shape = list(sizes.values())
     return {"dims": dims, "shape": shape}
```

### Comparing `scipp-24.2.0/src/scipp/core/argument_handlers.py` & `scipp-24.5.0/src/scipp/core/argument_handlers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Dict, TypeVar, Union
+from typing import TypeVar
 
 from ..typing import Variable
 
 _ValueType = TypeVar('_ValueType', str, Variable)
 
 
 def combine_dict_args(
-    arg: Union[Dict[str, _ValueType], None], kwargs: Dict[str, _ValueType]
-) -> Dict[str, _ValueType]:
+    arg: dict[str, _ValueType] | None, kwargs: dict[str, _ValueType]
+) -> dict[str, _ValueType]:
     pos_dict = {} if arg is None else arg
 
     overlapped = set(pos_dict).intersection(kwargs)
     if overlapped:
         raise ValueError(
-            'The names passed in the dict and as keyword arguments must be distinct.'
+            'The names passed in the dict and as keyword arguments must be distinct. '
             f'Following names are used in both arguments: {overlapped}'
         )
 
     return {**pos_dict, **kwargs}
```

### Comparing `scipp-24.2.0/src/scipp/core/arithmetic.py` & `scipp-24.5.0/src/scipp/core/arithmetic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Jan-Lukas Wynen
 
 from __future__ import annotations
 
 from .._scipp import core as _cpp
-from ..typing import VariableLike
+from ..typing import VariableLike, VariableLikeType
 from ._cpp_wrapper_util import call_func as _call_cpp_func
 
 
 def add(a: VariableLike, b: VariableLike) -> VariableLike:
     """Element-wise addition.
 
     Equivalent to::
@@ -212,15 +212,15 @@
     ----
     See the guide on `computation <../../user-guide/computation.rst>`_ for
     general concepts and broadcasting behavior.
     """
     return _call_cpp_func(_cpp.multiply, left, right)
 
 
-def negative(a) -> VariableLike:
+def negative(a: VariableLikeType) -> VariableLikeType:
     """Element-wise negative.
 
     Equivalent to::
 
         -a
 
     Parameters
@@ -229,15 +229,15 @@
         Input data.
 
     Returns
     -------
     :
         ``a`` with flipped signs.
     """
-    return _call_cpp_func(_cpp.negative, a)
+    return _call_cpp_func(_cpp.negative, a)  # type: ignore[return-value]
 
 
 def subtract(minuend: VariableLike, subtrahend: VariableLike) -> VariableLike:
     """Element-wise difference.
 
     Equivalent to::
```

### Comparing `scipp-24.2.0/src/scipp/core/assignments.py` & `scipp-24.5.0/src/scipp/core/assignments.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from __future__ import annotations
 
-from typing import Dict, Literal, Optional, Union
+from typing import Literal, TypeVar
 
-from ..typing import DataArray, Dataset, Variable
 from .argument_handlers import combine_dict_args
+from .cpp_classes import DataArray, Dataset, Variable
+
+_T = TypeVar('_T', Dataset, DataArray)
 
 
 def _assign(
-    obj: Union[Dataset, DataArray],
+    obj: _T,
     name: Literal['coords', 'masks', 'attrs'],
-    obj_attrs: Optional[Dict[str, Variable]] = None,
+    obj_attrs: dict[str, Variable] | None = None,
     /,
-    **kw_obj_attrs,
-) -> Union[Dataset, DataArray]:
+    **kw_obj_attrs: Variable,
+) -> _T:
     out = obj.copy(deep=False)
     collected = combine_dict_args(obj_attrs, kw_obj_attrs)
     for key, value in collected.items():
         getattr(out, name)[key] = value
     return out
 
 
 def assign_coords(
-    self, coords: Optional[Dict[str, Variable]] = None, /, **coords_kwargs
-) -> Union[DataArray, Dataset]:
+    self: _T, coords: dict[str, Variable] | None = None, /, **coords_kwargs: Variable
+) -> _T:
     """Return new object with updated or inserted coordinate.
 
     Parameters
     ----------
     coords :
         New coordinates.
 
@@ -42,15 +44,18 @@
         ``scipp.DataArray`` or ``scipp.Dataset`` with updated coordinates.
 
     """
     return _assign(self, 'coords', coords, **coords_kwargs)
 
 
 def assign_masks(
-    self, masks: Optional[Dict[str, Variable]] = None, /, **masks_kwargs
+    self: DataArray,
+    masks: dict[str, Variable] | None = None,
+    /,
+    **masks_kwargs: Variable,
 ) -> DataArray:
     """Return new object with updated or inserted masks.
 
     Parameters
     ----------
     masks :
         New masks.
@@ -64,15 +69,18 @@
         ``scipp.DataArray`` with updated masks.
 
     """
     return _assign(self, 'masks', masks, **masks_kwargs)
 
 
 def assign_attrs(
-    self, attrs: Optional[Dict[str, Variable]] = None, /, **attrs_kwargs
+    self: DataArray,
+    attrs: dict[str, Variable] | None = None,
+    /,
+    **attrs_kwargs: Variable,
 ) -> DataArray:
     """Return new object with updated or inserted attrs.
 
     Parameters
     ----------
     attrs :
         New attrs.
```

### Comparing `scipp-24.2.0/src/scipp/core/bin_remapping.py` & `scipp-24.5.0/src/scipp/core/bin_remapping.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
 import itertools
 import uuid
 from math import prod
-from typing import Dict, List
 
 from .._scipp import core as _cpp
 from ..typing import Dims, VariableLikeType
 from .concepts import concrete_dims, irreducible_mask, rewrap_reduced_data
 from .cpp_classes import DataArray, Variable
 from .cumulative import cumsum
 from .operations import where
@@ -39,15 +38,15 @@
     end = cumsum(sizes)
     begin = end - sizes
     data = var if var.bins is None else var.bins.constituents['data']
     dim = var.dim if var.bins is None else var.bins.constituents['dim']
     return _cpp._bins_no_validate(data=data, dim=dim, begin=begin, end=end)
 
 
-def _concat_bins(var: Variable, dim: List[str]) -> Variable:
+def _concat_bins(var: Variable, dim: list[str]) -> Variable:
     # To concat bins, two things need to happen:
     # 1. Data needs to be written to a contiguous chunk.
     # 2. New bin begin/end indices need to be setup.
     # If the dims to concatenate are the *inner* dims a call to `copy()` performs 1.
     # Otherwise, we first transpose and then `copy()`.
     # For step 2. we simply sum the (transposed) input bin sizes over the concat dims,
     # which `_with_bin_sizes` can use to compute new begin/end indices.
@@ -58,19 +57,19 @@
     out = var.transpose(unchanged_dims + changed_dims).copy()
     sizes = out.bins.size().sum(changed_dims)
     return _with_bin_sizes(out, sizes)
 
 
 def _combine_bins(
     var: Variable,
-    coords: Dict[str, Variable],
-    edges: List[Variable],
-    groups: List[Variable],
+    coords: dict[str, Variable],
+    edges: list[Variable],
+    groups: list[Variable],
     dim: Dims,
-) -> Dict[str, Variable]:
+) -> dict[str, Variable]:
     from .binning import make_binned
 
     # Overview
     # --------
     # The purpose of this code is to combine existing bins, but in a more general
     # manner than `concat`, which combines all bins along a dimension. Here we operate
     # more like `groupby`, which combines selected subsets and creates a new output dim.
@@ -122,15 +121,15 @@
     # copies of slices, but here we can leverage the same mechanism.
     # Then we call `_with_bin_sizes` to put in place new indices, "merging" the
     # reordered input bins to desired output bins.
     return _with_bin_sizes(source.copy(), sizes=params.data.bins.sum())
 
 
 def combine_bins(
-    da: DataArray, edges: List[Variable], groups: List[Variable], dim: Dims
+    da: DataArray, edges: list[Variable], groups: list[Variable], dim: Dims
 ) -> DataArray:
     masked = hide_masked(da, dim)
     if len(edges) == 0 and len(groups) == 0:
         data = _concat_bins(masked, dim=dim)
     else:
         names = [coord.dim for coord in itertools.chain(edges, groups)]
         coords = {name: da.coords[name] for name in names}
```

### Comparing `scipp-24.2.0/src/scipp/core/binning.py` & `scipp-24.5.0/src/scipp/core/binning.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
 import itertools
-import warnings
+from collections.abc import Sequence
 from numbers import Integral
-from typing import Dict, Optional, Sequence, Union, overload
+from typing import overload
 
 from .._scipp import core as _cpp
 from .bin_remapping import combine_bins
 from .cpp_classes import BinEdgeError, CoordError, DataArray, Dataset, DType, Variable
 from .data_group import DataGroup, data_group_overload
 from .math import round as round_
 from .shape import concat
-from .util import VisibleDeprecationWarning
 from .variable import arange, array, epoch, linspace, scalar
 
 
 @overload
-def make_histogrammed(x: Union[Variable, DataArray], *, edges: Variable) -> DataArray:
-    ...
+def make_histogrammed(x: Variable | DataArray, *, edges: Variable) -> DataArray: ...
 
 
 @overload
-def make_histogrammed(x: Dataset, *, edges: Variable) -> Dataset:
-    ...
+def make_histogrammed(x: Dataset, *, edges: Variable) -> Dataset: ...
 
 
 def make_histogrammed(x, *, edges):
     """Create dense data by histogramming data into given bins.
 
     If the input is binned data, then existing binning dimensions are preserved.
     Histogramming along an existing binned dimension will replace this binning.
@@ -67,19 +64,19 @@
                     "unless event data coordinate for histogramming is available."
                 )
             return make_histogrammed(x.bins.sum(), edges=edges)
     return _cpp.histogram(x, edges)
 
 
 def make_binned(
-    x: Union[Variable, DataArray],
+    x: Variable | DataArray,
     *,
-    edges: Optional[Sequence[Variable]] = None,
-    groups: Optional[Sequence[Variable]] = None,
-    erase: Optional[Sequence[str]] = None,
+    edges: Sequence[Variable] | None = None,
+    groups: Sequence[Variable] | None = None,
+    erase: Sequence[str] | None = None,
 ) -> DataArray:
     """Create binned data by binning input along all dimensions given by edges or
     groups.
 
     Usually :py:func:`scipp.bin` or :py:func:`scipp.group` should be preferred,
     unless the more precise control over which dimensions should be erased is required,
     or unless grouping and binning at the same time is required.
@@ -199,15 +196,15 @@
         bound.value = np.nextafter(
             bound.value, (bound + scalar(1, unit=bound.unit, dtype=bound.dtype)).value
         )
     return bound
 
 
 def _parse_coords_arg(
-    x: Union[Variable, DataArray, Dataset], name: str, arg: Union[int, Variable]
+    x: Variable | DataArray | Dataset, name: str, arg: int | Variable
 ) -> Variable:
     if isinstance(arg, Variable) and name in arg.dims:
         return arg
     coord = _get_coord(x, name)
     start = coord.min()
     if (
         not isinstance(x, Variable)
@@ -215,18 +212,16 @@
         and x.coords.is_edges(name, name)
     ):
         stop = coord.max()  # existing bin-edges, do not extend
     else:
         stop = _upper_bound(coord)
     if start > stop:
         raise ValueError(
-            (
-                'Empty data range, cannot automatically determine bounds. '
-                'Must provide concrete bin edges.'
-            )
+            'Empty data range, cannot automatically determine bounds. '
+            'Must provide concrete bin edges.'
         )
     if isinstance(arg, Integral):
         if start.dtype == DType.datetime64:
             base = epoch(unit=start.unit)
             return base + round_(
                 linspace(name, start - base, stop - base, num=arg + 1)
             ).to(dtype='int64')
@@ -236,18 +231,18 @@
     step = arg.to(dtype=start.dtype, unit=start.unit)
     if step.value == 0:
         raise ValueError("Step size cannot be 0.")
     return arange(name, start, stop + step, step=step)
 
 
 def _make_edges(
-    x: Union[Variable, DataArray, Dataset],
-    arg_dict: Optional[Dict[str, Union[int, Variable]]],
-    kwargs: Dict[str, Union[int, Variable]],
-) -> Dict[str, Variable]:
+    x: Variable | DataArray | Dataset,
+    arg_dict: dict[str, int | Variable] | None,
+    kwargs: dict[str, int | Variable],
+) -> dict[str, Variable]:
     if arg_dict is not None:
         kwargs = dict(**arg_dict, **kwargs)
     return {name: _parse_coords_arg(x, name, arg) for name, arg in kwargs.items()}
 
 
 def _find_replaced_dims(x, dims):
     if x.bins is None:
@@ -258,40 +253,37 @@
             if dim not in coord.dims:
                 erase = erase.union(coord.dims)
     return [dim for dim in erase if dim not in dims]
 
 
 @overload
 def hist(
-    x: Union[Variable, DataArray],
-    arg_dict: Optional[Dict[str, Union[int, Variable]]] = None,
+    x: Variable | DataArray,
+    arg_dict: dict[str, int | Variable] | None = None,
     /,
-    **kwargs: Union[int, Variable],
-) -> DataArray:
-    ...
+    **kwargs: int | Variable,
+) -> DataArray: ...
 
 
 @overload
 def hist(
     x: Dataset,
-    arg_dict: Optional[Dict[str, Union[int, Variable]]] = None,
+    arg_dict: dict[str, int | Variable] | None = None,
     /,
-    **kwargs: Union[int, Variable],
-) -> Dataset:
-    ...
+    **kwargs: int | Variable,
+) -> Dataset: ...
 
 
 @overload
 def hist(
     x: DataGroup,
-    arg_dict: Optional[Dict[str, Union[int, Variable]]] = None,
+    arg_dict: dict[str, int | Variable] | None = None,
     /,
-    **kwargs: Union[int, Variable],
-) -> DataGroup:
-    ...
+    **kwargs: int | Variable,
+) -> DataGroup: ...
 
 
 @data_group_overload
 def hist(x, arg_dict=None, /, **kwargs):
     """Compute a histogram.
 
     Bin edges can be specified in three ways:
@@ -378,29 +370,29 @@
       {'x': 20}
 
     Histogram binned data along an additional dimension:
 
       >>> binned = table.bin(x=10)
       >>> binned.hist(y=5).sizes
       {'x': 10, 'y': 5}
-    """  # noqa #501
+    """  # noqa: E501
     edges = _make_edges(x, arg_dict, kwargs)
     erase = _find_replaced_dims(x, edges)
     if isinstance(x, Variable) and len(edges) != 1:
         raise ValueError(
             "Edges for exactly one dimension must be specified when "
             "binning or histogramming a variable."
         )
     if len(edges) == 0:
         if x.bins is None:
             raise TypeError("Data is not binned so bin edges must be provided.")
         return x.bins.sum()
     if len(edges) == 1:
         # TODO Note that this may swap dims, is that ok?
-        out = make_histogrammed(x, edges=list(edges.values())[0])
+        out = make_histogrammed(x, edges=next(iter(edges.values())))
     else:
         edges = list(edges.values())
         # If histogramming by the final edges needs to use a non-event coord then we
         # must not erase that dim, since it removes the coord required for histogramming
         if isinstance(x, DataArray) and x.bins is not None:
             hist_dim = edges[-1].dims[-1]
             if hist_dim not in x.bins.coords:
@@ -413,30 +405,28 @@
         if dim in out.dims:
             out = out.sum(dim)
     return out
 
 
 @overload
 def nanhist(
-    x: Union[Variable, DataArray],
-    arg_dict: Optional[Dict[str, Union[int, Variable]]] = None,
+    x: Variable | DataArray,
+    arg_dict: dict[str, int | Variable] | None = None,
     /,
-    **kwargs: Union[int, Variable],
-) -> DataArray:
-    ...
+    **kwargs: int | Variable,
+) -> DataArray: ...
 
 
 @overload
 def nanhist(
     x: DataGroup,
-    arg_dict: Optional[Dict[str, Union[int, Variable]]] = None,
+    arg_dict: dict[str, int | Variable] | None = None,
     /,
-    **kwargs: Union[int, Variable],
-) -> DataGroup:
-    ...
+    **kwargs: int | Variable,
+) -> DataGroup: ...
 
 
 @data_group_overload
 def nanhist(x, arg_dict=None, /, **kwargs):
     """Compute a histogram, skipping NaN values.
 
     Like :py:func:`scipp.hist`, but NaN values are skipped. See there for details and
@@ -462,30 +452,28 @@
     if x.bins is None:
         raise TypeError("Data is not binned so bin edges must be provided.")
     return x.bins.nansum()
 
 
 @overload
 def bin(
-    x: Union[Variable, DataArray],
-    arg_dict: Optional[Dict[str, Union[int, Variable]]] = None,
+    x: Variable | DataArray,
+    arg_dict: dict[str, int | Variable] | None = None,
     /,
-    **kwargs: Union[int, Variable],
-) -> DataArray:
-    ...
+    **kwargs: int | Variable,
+) -> DataArray: ...
 
 
 @overload
 def bin(
     x: DataGroup,
-    arg_dict: Optional[Dict[str, Union[int, Variable]]] = None,
+    arg_dict: dict[str, int | Variable] | None = None,
     /,
-    **kwargs: Union[int, Variable],
-) -> DataGroup:
-    ...
+    **kwargs: int | Variable,
+) -> DataGroup: ...
 
 
 @data_group_overload
 def bin(x, arg_dict=None, /, **kwargs):
     """Create binned data by binning input along all dimensions given by edges.
 
     Bin edges can be specified in three ways:
@@ -574,64 +562,48 @@
 
     Bin binned data along an additional dimension:
 
       >>> binned = table.bin(x=10)
       >>> binned.bin(y=5).sizes
       {'x': 10, 'y': 5}
     """
-    if arg_dict is None:
-        for name, item in kwargs.items():
-            if name in ('edges', 'groups', 'erase') and isinstance(item, list):
-                warnings.warn(
-                    "The 'edges', 'groups', and 'erase' keyword arguments "
-                    "are deprecated. Use, e.g., 'sc.bin(da, x=x_edges)' or "
-                    "'sc.group(da, groups)'. See the documentation for details.",
-                    UserWarning,
-                )
-                return make_binned(x, **kwargs)
     edges = _make_edges(x, arg_dict, kwargs)
     erase = _find_replaced_dims(x, edges)
     return make_binned(x, edges=list(edges.values()), erase=erase)
 
 
 @overload
 def rebin(
     x: DataArray,
-    arg_dict: Dict[str, Union[int, Variable]] = None,
-    deprecated=None,
+    arg_dict: dict[str, int | Variable] | None = None,
     /,
-    **kwargs: Union[int, Variable],
-) -> DataArray:
-    ...
+    **kwargs: int | Variable,
+) -> DataArray: ...
 
 
 @overload
 def rebin(
     x: Dataset,
-    arg_dict: Dict[str, Union[int, Variable]] = None,
-    deprecated=None,
+    arg_dict: dict[str, int | Variable] | None = None,
     /,
-    **kwargs: Union[int, Variable],
-) -> Dataset:
-    ...
+    **kwargs: int | Variable,
+) -> Dataset: ...
 
 
 @overload
 def rebin(
     x: DataGroup,
-    arg_dict: Dict[str, Union[int, Variable]] = None,
-    deprecated=None,
+    arg_dict: dict[str, int | Variable] | None = None,
     /,
-    **kwargs: Union[int, Variable],
-) -> DataGroup:
-    ...
+    **kwargs: int | Variable,
+) -> DataGroup: ...
 
 
 @data_group_overload
-def rebin(x, arg_dict=None, deprecated=None, /, **kwargs):
+def rebin(x, arg_dict=None, /, **kwargs):
     """Rebin a data array or dataset.
 
     The coordinate of the input for the dimension to be rebinned must contain bin edges,
     i.e., the data must be histogrammed.
 
     If the input has masks that contain the dimension being rebinned then those
     masks are applied to the data before rebinning. That is, masked values are treated
@@ -682,24 +654,14 @@
 
     Rebin a data array along two of its dimensions:
 
       >>> da = table.hist(x=100, y=100)
       >>> da.rebin(x=4, y=6).sizes
       {'x': 4, 'y': 6}
     """
-    if isinstance(arg_dict, str):
-        if deprecated is not None or 'bins' in kwargs:
-            warnings.warn(
-                "The 'bins' keyword argument and positional syntax for setting bin "
-                "edges is deprecated. Use, e.g., 'sc.rebin(da, x=x_edges)'. See the "
-                "documentation for details.",
-                UserWarning,
-            )
-            bins = {'bins': deprecated, **kwargs}
-            return _cpp.rebin(x, arg_dict, **bins)
     edges = _make_edges(x, arg_dict, kwargs)
     out = x
     for dim, edge in edges.items():
         out = _cpp.rebin(out, dim, edge)
     return out
 
 
@@ -711,15 +673,15 @@
     coord = x.bins.coords.get(arg) if x.bins is not None else None
     if coord is None:
         coord = x.coords.get(arg)
     _require_coord(arg, coord)
     if coord.bins is not None:
         coord = coord.copy().bins.constituents['data']
 
-    if coord.values.size == 0:
+    if 0 in coord.shape:
         unique = coord.values[0:0]
     # We are currently using np.unique to find all unique groups. This can be very slow
     # for large inputs. In many cases groups are in a bounded range of integers, and we
     # can sometimes bypass a full call to np.unique by checking a sub-range first
     elif coord.dtype in (DType.int32, DType.int64):
         min_ = coord.min().value
         max_ = coord.max().value
@@ -731,25 +693,23 @@
             unique = np.unique(values[: len(values) // pivot])
     else:
         unique = np.unique(coord.values)
     return array(dims=[arg], values=unique, unit=coord.unit)
 
 
 @overload
-def group(x: DataArray, /, *args: Union[str, Variable]) -> DataArray:
-    ...
+def group(x: DataArray, /, *args: str | Variable) -> DataArray: ...
 
 
 @overload
-def group(x: DataGroup, /, *args: Union[str, Variable]) -> DataGroup:
-    ...
+def group(x: DataGroup, /, *args: str | Variable) -> DataGroup: ...
 
 
 @data_group_overload
-def group(x, /, *args: Union[str, Variable]):
+def group(x, /, *args: str | Variable):
     """Create binned data by grouping input by one or more coordinates.
 
     Grouping can be specified in two ways: (1) When a string is provided the unique
     values of the corresponding coordinate are used as groups. (2) When a Scipp variable
     is provided then the variable's values are used as groups.
 
     Note that option (1) may be very slow if the input is very large.
@@ -829,18 +789,7 @@
       >>> binned = table.bin(x=10)
       >>> binned.group('a').sizes
       {'x': 10, 'a': 10}
     """
     groups = [_make_groups(x, name) for name in args]
     erase = _find_replaced_dims(x, [g.dim for g in groups])
     return make_binned(x, groups=groups, erase=erase)
-
-
-def histogram(
-    x: Union[DataArray, Dataset], *, bins: Variable
-) -> Union[DataArray, Dataset]:
-    """Deprecated. See :py:func:`scipp.hist`."""
-    warnings.warn("'histogram' is deprecated. Use 'hist' instead.", UserWarning)
-    warnings.warn(
-        "'histogram' is deprecated. Use 'hist' instead.", VisibleDeprecationWarning
-    )
-    return make_histogrammed(x, edges=bins)
```

### Comparing `scipp-24.2.0/src/scipp/core/bins.py` & `scipp-24.5.0/src/scipp/core/bins.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
-import warnings
-from typing import Callable, Dict, Literal, Optional, Tuple, Union
+from collections.abc import Callable
+from typing import Literal
 
 from .._scipp import core as _cpp
 from ..typing import Dims, MetaDataMap, VariableLike
 from ._cpp_wrapper_util import call_func as _call_cpp_func
 from .bin_remapping import concat_bins
 from .cpp_classes import Variable
 from .data_group import DataGroup
@@ -28,15 +28,15 @@
     """
 
     def __init__(
         self,
         op: Callable,
         func: _cpp.DataArray,
         dim: str,
-        fill_value: Optional[Variable] = None,
+        fill_value: Variable | None = None,
     ):
         if (
             not func.masks
             and func.ndim == 1
             and len(func) > 0
             and func.dtype in [_cpp.DType.bool, _cpp.DType.int32, _cpp.DType.int64]
         ):
@@ -62,18 +62,18 @@
     def __getitem__(self, var: Variable) -> Variable:
         """Return table values for the given points."""
         return self(var)
 
 
 def lookup(
     func: _cpp.DataArray,
-    dim: Optional[str] = None,
+    dim: str | None = None,
     *,
-    mode: Optional[Literal['previous', 'nearest']] = None,
-    fill_value: Optional[_cpp.Variable] = None,
+    mode: Literal['previous', 'nearest'] | None = None,
+    fill_value: _cpp.Variable | None = None,
 ) -> Lookup:
     """Create a "lookup table" from a histogram (data array with bin-edge coord).
 
     The lookup table can be used to map, e.g., time-stamps to corresponding values
     given by a time-series log.
 
     Parameters
@@ -160,15 +160,15 @@
         _cpp.buckets.scale(self._obj, lut.func, lut.dim)
         return self
 
     def __itruediv__(self, lut: lookup):
         _cpp.buckets.scale(self._obj, _cpp.reciprocal(lut.func), lut.dim)
         return self
 
-    def __getitem__(self, key: Tuple[str, Union[_cpp.Variable, slice]]):
+    def __getitem__(self, key: tuple[str, _cpp.Variable | slice]):
         """
         Extract events from bins based on labels or label ranges and return a copy.
 
         This is similar to regular label-based indexing, but considers the event-coords,
         i.e., the coord values of individual bin entries. Unlike normal label-based
         indexing this returns a copy, as a subset of events is extracted.
         """
@@ -264,194 +264,194 @@
 
     @property
     def unit(self) -> _cpp.Unit:
         """Unit of the bin elements"""
         return self.constituents['data'].unit
 
     @unit.setter
-    def unit(self, unit: Union[_cpp.Unit, str]):
+    def unit(self, unit: _cpp.Unit | str):
         """Set unit of the bin elements"""
         self.constituents['data'].unit = unit
 
     @property
     def dtype(self) -> _cpp.DType:
         """Data type of the bin elements."""
         return self.constituents['data'].dtype
 
     @property
     def aligned(self) -> bool:
         """Alignment flag for coordinates of bin elements."""
         return self.constituents['data'].aligned
 
     @property
-    def constituents(self) -> Dict[str, Union[str, _cpp.Variable, _cpp.DataArray]]:
+    def constituents(self) -> dict[str, str | _cpp.Variable | _cpp.DataArray]:
         """Constituents of binned data, as supported by :py:func:`sc.bins`."""
         return _call_cpp_func(_cpp.bins_constituents, self._data())
 
-    def sum(self) -> Union[_cpp.Variable, _cpp.DataArray]:
+    def sum(self) -> _cpp.Variable | _cpp.DataArray:
         """Sum of events in each bin.
 
         Returns
         -------
         :
             The sum of each of the input bins.
 
         See Also
         --------
         scipp.sum:
             For summing non-bin data or summing bins.
         """
         return _call_cpp_func(_cpp.bins_sum, self._obj)
 
-    def nansum(self) -> Union[_cpp.Variable, _cpp.DataArray]:
+    def nansum(self) -> _cpp.Variable | _cpp.DataArray:
         """Sum of events in each bin ignoring NaN's.
 
         Returns
         -------
         :
             The sum of each of the input bins without NaN's.
 
         See Also
         --------
         scipp.nansum:
             For summing non-bin data or summing bins.
         """
         return _call_cpp_func(_cpp.bins_nansum, self._obj)
 
-    def mean(self) -> Union[_cpp.Variable, _cpp.DataArray]:
+    def mean(self) -> _cpp.Variable | _cpp.DataArray:
         """Arithmetic mean of events in each bin.
 
         Returns
         -------
         :
             The mean of each of the input bins.
 
         See Also
         --------
         scipp.mean:
             For calculating the mean of non-bin data or across bins.
         """
         return _call_cpp_func(_cpp.bins_mean, self._obj)
 
-    def nanmean(self) -> Union[_cpp.Variable, _cpp.DataArray]:
+    def nanmean(self) -> _cpp.Variable | _cpp.DataArray:
         """Arithmetic mean of events in each bin ignoring NaN's.
 
         Returns
         -------
         :
             The mean of each of the input bins without NaN's.
 
         See Also
         --------
         scipp.nanmean:
             For calculating the mean of non-bin data or across bins.
         """
         return _call_cpp_func(_cpp.bins_nanmean, self._obj)
 
-    def max(self) -> Union[_cpp.Variable, _cpp.DataArray]:
+    def max(self) -> _cpp.Variable | _cpp.DataArray:
         """Maximum of events in each bin.
 
         Returns
         -------
         :
             The maximum of each of the input bins.
 
         See Also
         --------
         scipp.max:
             For calculating the maximum of non-bin data or across bins.
         """
         return _call_cpp_func(_cpp.bins_max, self._obj)
 
-    def nanmax(self) -> Union[_cpp.Variable, _cpp.DataArray]:
+    def nanmax(self) -> _cpp.Variable | _cpp.DataArray:
         """Maximum of events in each bin ignoring NaN's.
 
         Returns
         -------
         :
             The maximum of each of the input bins without NaN's.
 
         See Also
         --------
         scipp.nanmax:
             For calculating the maximum of non-bin data or across bins.
         """
         return _call_cpp_func(_cpp.bins_nanmax, self._obj)
 
-    def min(self) -> Union[_cpp.Variable, _cpp.DataArray]:
+    def min(self) -> _cpp.Variable | _cpp.DataArray:
         """Minimum of events in each bin.
 
         Returns
         -------
         :
             The minimum of each of the input bins.
 
         See Also
         --------
         scipp.min:
             For calculating the minimum of non-bin data or across bins.
         """
         return _call_cpp_func(_cpp.bins_min, self._obj)
 
-    def nanmin(self) -> Union[_cpp.Variable, _cpp.DataArray]:
+    def nanmin(self) -> _cpp.Variable | _cpp.DataArray:
         """Minimum of events in each bin ignoring NaN's.
 
         Returns
         -------
         :
             The minimum of each of the input bins without NaN's.
 
         See Also
         --------
         scipp.nanmin:
             For calculating the minimum of non-bin data or across bins.
         """
         return _call_cpp_func(_cpp.bins_nanmin, self._obj)
 
-    def all(self) -> Union[_cpp.Variable, _cpp.DataArray]:
+    def all(self) -> _cpp.Variable | _cpp.DataArray:
         """Logical AND of events in each bin ignoring NaN's.
 
         Returns
         -------
         :
             The AND of each of the input bins without NaN's.
 
         See Also
         --------
         scipp.all:
             For performing an AND of non-bin data or across bins.
         """
         return _call_cpp_func(_cpp.bins_all, self._obj)
 
-    def any(self) -> Union[_cpp.Variable, _cpp.DataArray]:
+    def any(self) -> _cpp.Variable | _cpp.DataArray:
         """Logical OR of events in each bin ignoring NaN's.
 
         Returns
         -------
         :
             The OR of each of the input bins without NaN's.
 
         See Also
         --------
         scipp.all:
             For performing an OR of non-bin data or across bins.
         """
         return _call_cpp_func(_cpp.bins_any, self._obj)
 
-    def size(self) -> Union[_cpp.Variable, _cpp.DataArray]:
+    def size(self) -> _cpp.Variable | _cpp.DataArray:
         """Number of events or elements in a bin.
 
         Returns
         -------
         :
             The number of elements in each of the input bins.
         """
         return _call_cpp_func(_cpp.bin_sizes, self._obj)
 
-    def concat(self, dim: Dims = None) -> Union[_cpp.Variable, _cpp.DataArray]:
+    def concat(self, dim: Dims = None) -> _cpp.Variable | _cpp.DataArray:
         """Concatenate bins element-wise by concatenating bin contents along
         their internal bin dimension.
 
         This is a reduction operation similar to :py:func:`scipp.sum` but operates on
         binned data. Elements (bins) are concatenated along their internal dimension.
 
         Parameters
@@ -464,18 +464,18 @@
         :
             All bins along `dim` concatenated into a single bin.
         """
         return concat_bins(self._obj, dim)
 
     def concatenate(
         self,
-        other: Union[_cpp.Variable, _cpp.DataArray],
+        other: _cpp.Variable | _cpp.DataArray,
         *,
-        out: Optional[_cpp.DataArray] = None,
-    ) -> Union[_cpp.Variable, _cpp.DataArray]:
+        out: _cpp.DataArray | None = None,
+    ) -> _cpp.Variable | _cpp.DataArray:
         """Concatenate bins element-wise by concatenating bin contents along
         their internal bin dimension.
 
         The bins to concatenate are obtained element-wise from `self` and `other`.
 
         Parameters
         ----------
@@ -500,55 +500,37 @@
             if self._obj is out:
                 _call_cpp_func(_cpp.buckets.append, self._obj, other)
             else:
                 out = _call_cpp_func(_cpp.buckets.concatenate, self._obj, other)
             return out
 
 
-class GroupbyBins:
-    """Proxy for operations on bins of a groupby object."""
-
-    def __init__(self, obj):
-        self._obj = obj
-
-    def concat(self, dim):
-        warnings.warn(
-            "groupby(...).bins.concat(dim) is deprecated. Use `group` or `bin` instead",
-            UserWarning,
-        )
-        return self._obj.concat(dim)
-
-
-def _bins(obj):
+def _bins(obj) -> Bins | None:
     """
     Returns helper :py:class:`scipp.Bins` allowing bin-wise operations
     to be performed or `None` if not binned data.
     """
     if _cpp.is_bins(obj):
         return Bins(obj)
     else:
         return None
 
 
-def _set_bins(obj, bins: Bins):
+def _set_bins(obj, bins: Bins) -> None:
     # Should only be used by __iadd__ and friends
     if obj is not bins._obj:
         raise ValueError("Cannot set bins with a new object")
 
 
-def _groupby_bins(obj):
-    return GroupbyBins(obj)
-
-
 def bins(
     *,
     data: VariableLike,
     dim: str,
-    begin: Optional[_cpp.Variable] = None,
-    end: Optional[_cpp.Variable] = None,
+    begin: _cpp.Variable | None = None,
+    end: _cpp.Variable | None = None,
 ) -> _cpp.Variable:
     """Create a binned variable from bin indices.
 
     The elements of the returned variable are "bins", defined as views into
     ``data``. The returned variable keeps and manages a copy of ``data``
     internally.
 
@@ -581,15 +563,15 @@
 
     See Also
     --------
     scipp.bin:
         For creating DataArrays based on binning of coord value
         instead of explicitly given index ranges.
     """
-    if any([isinstance(x, DataGroup) for x in [begin, end, data]]):
+    if any(isinstance(x, DataGroup) for x in [begin, end, data]):
         raise ValueError("`scipp.bins` does not support DataGroup arguments.")
     return _call_cpp_func(_cpp.bins, begin, end, dim, data)
 
 
 def bins_like(x: VariableLike, fill_value: _cpp.Variable) -> _cpp.Variable:
     """Create a binned variable by "broadcasting" fill values to bins of given sizes.
```

### Comparing `scipp-24.2.0/src/scipp/core/comparison.py` & `scipp-24.5.0/src/scipp/core/comparison.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
-# flake8: noqa: E501
+# ruff: noqa: E501
 
 from __future__ import annotations
 
+from typing import Any
+
 import numpy as np
 
 from .._scipp import core as _cpp
 from ..typing import VariableLike
 from . import data_group
 from ._cpp_wrapper_util import call_func as _call_cpp_func
 from .cpp_classes import DataArray, Dataset, Variable
@@ -146,18 +148,18 @@
     """
     return _call_cpp_func(_cpp.not_equal, x, y)
 
 
 def _identical_data_groups(
     x: data_group.DataGroup, y: data_group.DataGroup, *, equal_nan: bool
 ) -> bool:
-    def compare(a, b):
+    def compare(a: Any, b: Any) -> bool:
         if not isinstance(a, type(b)):
             return False
-        if isinstance(a, (Variable, DataArray, Dataset, data_group.DataGroup)):
+        if isinstance(a, Variable | DataArray | Dataset | data_group.DataGroup):
             return identical(a, b, equal_nan=equal_nan)
         if isinstance(a, np.ndarray):
             return np.array_equal(a, b, equal_nan=equal_nan)
         # Explicit conversion to bool in case __eq__ returns
         # something else like an array.
         return bool(a == b)
 
@@ -186,15 +188,15 @@
         dims, shapes, coords, and masks. Else False.
     """
     if isinstance(x, data_group.DataGroup):
         if not isinstance(y, data_group.DataGroup):
             raise TypeError("Both or neither of the arguments must be a DataGroup")
         return _identical_data_groups(x, y, equal_nan=equal_nan)
 
-    return _call_cpp_func(_cpp.identical, x, y, equal_nan=equal_nan)
+    return _call_cpp_func(_cpp.identical, x, y, equal_nan=equal_nan)  # type: ignore[return-value]
 
 
 def isclose(
     x: _cpp.Variable,
     y: _cpp.Variable,
     *,
     rtol: _cpp.Variable = None,
@@ -259,15 +261,21 @@
     if atol is None:
         atol = scalar(1e-8, unit=y.unit)
     if rtol is None:
         rtol = scalar(1e-5, unit=None if atol.unit is None else _cpp.units.one)
     return _call_cpp_func(_cpp.isclose, x, y, rtol, atol, equal_nan)
 
 
-def allclose(x, y, rtol=None, atol=None, equal_nan=False) -> True:
+def allclose(
+    x: _cpp.Variable,
+    y: _cpp.Variable,
+    rtol: _cpp.Variable = None,
+    atol: _cpp.Variable = None,
+    equal_nan: bool = False,
+) -> bool:
     """Checks if all elements in the inputs are close to each other.
 
     Verifies that ALL element-wise comparisons meet the condition:
 
     abs(x - y) <= atol + rtol * abs(y)
 
     If both x and y have variances, the variances are also compared
@@ -313,10 +321,10 @@
         True if for all elements ``value <= atol + rtol * abs(y)``, otherwise False.
 
     See Also
     --------
     scipp.isclose:
         Compares element-wise with specified tolerances.
     """
-    return _call_cpp_func(
+    return _call_cpp_func(  # type:ignore[no-any-return]
         _cpp.all, isclose(x, y, rtol=rtol, atol=atol, equal_nan=equal_nan)
-    ).value
+    ).value  # type: ignore[union-attr]
```

### Comparing `scipp-24.2.0/src/scipp/core/counts.py` & `scipp-24.5.0/src/scipp/core/counts.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Matthew Andrew
 
-from typing import Union
 
 from .._scipp import core as _cpp
 from ._cpp_wrapper_util import call_func as _call_cpp_func
 
 
 def counts_to_density(
-    x: Union[_cpp.DataArray, _cpp.Dataset], dim: str
-) -> Union[_cpp.DataArray, _cpp.Dataset]:
+    x: _cpp.DataArray | _cpp.Dataset, dim: str
+) -> _cpp.DataArray | _cpp.Dataset:
     """Converts counts to count density on a given dimension.
 
     Parameters
     ----------
     x:
         Data as counts.
     dim:
@@ -25,16 +24,16 @@
     :
         Data as count density.
     """
     return _call_cpp_func(_cpp.counts_to_density, x, dim)
 
 
 def density_to_counts(
-    x: Union[_cpp.DataArray, _cpp.Dataset], dim: str
-) -> Union[_cpp.DataArray, _cpp.Dataset]:
+    x: _cpp.DataArray | _cpp.Dataset, dim: str
+) -> _cpp.DataArray | _cpp.Dataset:
     """Converts counts to count density on a given dimension.
 
     Parameters
     ----------
     x:
         Data as count density.
     dim:
```

### Comparing `scipp-24.2.0/src/scipp/core/cpp_classes.pyi` & `scipp-24.5.0/src/scipp/core/cpp_classes.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ############################################
 #               ATTENTION                  #
 # This file was generated by tools/stubgen #
 # Do not edit!                             #
 ############################################
-# flake8: noqa
+# ruff: noqa: F403
 
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
@@ -66,128 +66,128 @@
 
 class BinnedDataError(RuntimeError):
     ...
 
 class CoordError(RuntimeError):
     ...
 
-class Coords:
+class Coords(Mapping[str, Variable]):
 
     def __contains__(self, arg0: str) -> bool:
         ...
 
     def __copy__(self) -> Coords:
         ...
 
     def __deepcopy__(self, arg0: dict) -> Coords:
         ...
 
     def __delitem__(self, arg0: str) -> None:
         ...
 
-    def __eq__(self, arg0: object) -> bool:  # type: ignore[override]
+    def __eq__(self, arg0: object) -> bool:  # type: ignore[override, unused-ignore]
         ...
 
     def __getitem__(self, arg0: str) -> Variable:
         ...
 
-    def __iter__(self) -> Iterator:
+    def __iter__(self) -> Iterator[str]:
         ...
 
     def __len__(self) -> int:
         ...
 
-    def __ne__(self, arg0: object) -> bool:  # type: ignore[override]
+    def __ne__(self, arg0: object) -> bool:  # type: ignore[override, unused-ignore]
         ...
 
     def __repr__(self) -> str:
         ...
 
     def __setitem__(self, arg0: str, arg1: Variable) -> None:
         ...
 
     def __str__(self) -> str:
         ...
 
     def _ipython_key_completions_(self) -> list:
         ...
 
-    def _pop(self, k: str) -> Any:
+    def _pop(self, k: str) -> Variable:
         ...
 
     def clear(self) -> None:
         ...
 
     def copy(self, deep: bool=True) -> Coords:
         ...
 
-    def get(self, key, default=None):
+    def get(self, key: str, default: Variable | None=None) -> Variable | None:
         ...
 
     def is_edges(self, key: str, dim: Optional[str]=None) -> bool:
         ...
 
     def items(self) -> Coords_items_view:
         ...
 
     def keys(self) -> Coords_keys_view:
         ...
 
-    def pop(self, key, default=_NoDefault):
+    def pop(self, key: str, default: Any=_NoDefault) -> Variable | None:
         ...
 
-    def popitem(self) -> Tuple[str, Any]:
+    def popitem(self) -> tuple[str, Variable]:
         ...
 
     def set_aligned(self, key: str, aligned: bool) -> None:
         ...
 
     def update(self, other: Any=None, /, **kwargs) -> None:
         ...
 
     def values(self) -> Coords_values_view:
         ...
 
 class Coords_items_view:
 
-    def __eq__(self, arg0: object) -> bool:  # type: ignore[override]
+    def __eq__(self, arg0: object) -> bool:  # type: ignore[override, unused-ignore]
         ...
 
-    def __iter__(self) -> Iterator:
+    def __iter__(self) -> Iterator[tuple[str, Variable]]:
         ...
 
     def __len__(self) -> int:
         ...
 
     def __repr__(self) -> str:
         ...
 
     def __str__(self) -> str:
         ...
 
 class Coords_keys_view:
 
-    def __eq__(self, arg0: object) -> bool:  # type: ignore[override]
+    def __eq__(self, arg0: object) -> bool:  # type: ignore[override, unused-ignore]
         ...
 
-    def __iter__(self) -> Iterator:
+    def __iter__(self) -> Iterator[str]:
         ...
 
     def __len__(self) -> int:
         ...
 
     def __repr__(self) -> str:
         ...
 
     def __str__(self) -> str:
         ...
 
 class Coords_values_view:
 
-    def __iter__(self) -> Iterator:
+    def __iter__(self) -> Iterator[Variable]:
         ...
 
     def __len__(self) -> int:
         ...
 
     def __repr__(self) -> str:
         ...
@@ -200,15 +200,15 @@
     DataArrayView: DType = ...
     Dataset: DType = ...
     DatasetView: DType = ...
     PyObject: DType = ...
     Variable: DType = ...
     VariableView: DType = ...
 
-    def __eq__(self, arg0: object) -> bool:  # type: ignore[override]
+    def __eq__(self, arg0: object) -> bool:  # type: ignore[override, unused-ignore]
         ...
 
     def __init__(self, arg0: Any) -> None:
         ...
 
     def __repr__(self) -> str:
         ...
@@ -265,15 +265,15 @@
 
     def __copy__(self) -> DataArray:
         ...
 
     def __deepcopy__(self, arg0: dict) -> DataArray:
         ...
 
-    def __eq__(self, arg0: object) -> DataArray:  # type: ignore[override]
+    def __eq__(self, arg0: object) -> DataArray:  # type: ignore[override, unused-ignore]
         ...
 
     @overload
     def __floordiv__(self, arg0: DataArray) -> DataArray:
         ...
 
     @overload
@@ -301,35 +301,35 @@
         ...
 
     @overload
     def __getitem__(self, arg0: Variable) -> DataArray:
         ...
 
     @overload
-    def __getitem__(self, arg0: Tuple[str, Variable]) -> DataArray:
+    def __getitem__(self, arg0: tuple[str, Variable]) -> DataArray:
         ...
 
     @overload
-    def __getitem__(self, arg0: Tuple[str, int]) -> DataArray:
+    def __getitem__(self, arg0: tuple[str, int]) -> DataArray:
         ...
 
     @overload
-    def __getitem__(self, arg0: Tuple[str, slice]) -> DataArray:
+    def __getitem__(self, arg0: tuple[str, slice]) -> DataArray:
         ...
 
     @overload
     def __getitem__(self, arg0: ellipsis) -> DataArray:
         ...
 
     @overload
-    def __getitem__(self, arg0: List[int]) -> DataArray:
+    def __getitem__(self, arg0: list[int]) -> DataArray:
         ...
 
     @overload
-    def __getitem__(self, arg0: Tuple[str, List[int]]) -> DataArray:
+    def __getitem__(self, arg0: tuple[str, list[int]]) -> DataArray:
         ...
 
     @overload
     def __gt__(self, arg0: DataArray) -> DataArray:
         ...
 
     @overload
@@ -388,15 +388,15 @@
     def __imul__(self, arg0: Variable) -> DataArray:
         ...
 
     @overload
     def __imul__(self, arg0: float) -> DataArray:
         ...
 
-    def __init__(self, data: Variable, coords: Union[Mapping[str, Variable], Iterable[Tuple[str, Variable]]]={}, masks: Union[Mapping[str, Variable], Iterable[Tuple[str, Variable]]]={}, attrs: Union[Mapping[str, Variable], Iterable[Tuple[str, Variable]]]={}, name: str='') -> None:
+    def __init__(self, data: Variable, coords: Union[Mapping[str, Variable], Iterable[tuple[str, Variable]]]={}, masks: Union[Mapping[str, Variable], Iterable[tuple[str, Variable]]]={}, attrs: Union[Mapping[str, Variable], Iterable[tuple[str, Variable]]]={}, name: str='') -> None:
         ...
 
     def __invert__(self) -> DataArray:
         ...
 
     @overload
     def __ior__(self, arg0: DataArray) -> DataArray:
@@ -481,15 +481,15 @@
     def __mul__(self, arg0: Variable) -> DataArray:
         ...
 
     @overload
     def __mul__(self, arg0: float) -> DataArray:
         ...
 
-    def __ne__(self, arg0: object) -> DataArray:  # type: ignore[override]
+    def __ne__(self, arg0: object) -> DataArray:  # type: ignore[override, unused-ignore]
         ...
 
     def __neg__(self) -> DataArray:
         ...
 
     @overload
     def __or__(self, arg0: DataArray) -> DataArray:
@@ -532,35 +532,35 @@
     def __rsub__(self, arg0: float) -> DataArray:
         ...
 
     def __rtruediv__(self, arg0: float) -> DataArray:
         ...
 
     @overload
-    def __setitem__(self, arg0: Tuple[str, Variable], arg1: Variable) -> None:
+    def __setitem__(self, arg0: tuple[str, Variable], arg1: Variable) -> None:
         ...
 
     @overload
-    def __setitem__(self, arg0: Tuple[str, Variable], arg1: DataArray) -> None:
+    def __setitem__(self, arg0: tuple[str, Variable], arg1: DataArray) -> None:
         ...
 
     @overload
     def __setitem__(self, arg0: int, arg1: Any) -> None:
         ...
 
     @overload
     def __setitem__(self, arg0: slice, arg1: Any) -> None:
         ...
 
     @overload
-    def __setitem__(self, arg0: Tuple[str, int], arg1: Any) -> None:
+    def __setitem__(self, arg0: tuple[str, int], arg1: Any) -> None:
         ...
 
     @overload
-    def __setitem__(self, arg0: Tuple[str, slice], arg1: Any) -> None:
+    def __setitem__(self, arg0: tuple[str, slice], arg1: Any) -> None:
         ...
 
     @overload
     def __setitem__(self, arg0: ellipsis, arg1: Any) -> None:
         ...
 
     def __sizeof__(self) -> int:
@@ -605,57 +605,57 @@
     @overload
     def __xor__(self, arg0: Variable) -> DataArray:
         ...
 
     def _ipython_key_completions_(self) -> list:
         ...
 
-    def _rename_dims(self, arg0: Dict[str, str]) -> DataArray:
+    def _rename_dims(self, arg0: dict[str, str]) -> DataArray:
         ...
 
     def _repr_html_(self) -> str:
         ...
 
-    def all(self, dim: Optional[str]=None) -> VariableLikeType:
+    def all(self, dim: str | None=None) -> DataArray:
         ...
 
-    def any(self, dim: Optional[str]=None) -> VariableLikeType:
+    def any(self, dim: str | None=None) -> DataArray:
         ...
 
-    def assign_attrs(self, attrs: Optional[Dict[str, Variable]]=None, /, **attrs_kwargs) -> DataArray:
+    def assign_attrs(self, attrs: dict[str, Variable] | None=None, /, **attrs_kwargs: Variable) -> DataArray:
         ...
 
-    def assign_coords(self, coords: Optional[Dict[str, Variable]]=None, /, **coords_kwargs) -> Union[DataArray, Dataset]:
+    def assign_coords(self, coords: dict[str, Variable] | None=None, /, **coords_kwargs: Variable) -> _T:
         ...
 
-    def assign_masks(self, masks: Optional[Dict[str, Variable]]=None, /, **masks_kwargs) -> DataArray:
+    def assign_masks(self, masks: dict[str, Variable] | None=None, /, **masks_kwargs: Variable) -> DataArray:
         ...
 
     def astype(self, type: Any, *, copy: bool=True) -> DataArray:
         ...
 
     @property
     def attrs(self):
         ...
 
     def bin(self, arg_dict=None, /, **kwargs):
         ...
 
     @property
-    def bins(self):
+    def bins(self) -> Bins | None:
         ...
 
     @bins.setter
-    def bins(self, bins: Bins):
+    def bins(self, bins: Bins) -> None:
         ...
 
-    def broadcast(self, dims: Optional[Union[List[str], Tuple[str, ...]]]=None, shape: Optional[Sequence[int]]=None, sizes: Optional[Dict[str, int]]=None) -> VariableLikeType:
+    def broadcast(self, dims: list[str] | tuple[str, ...] | None=None, shape: Sequence[int] | None=None, sizes: dict[str, int] | None=None) -> DataArray:
         ...
 
-    def ceil(self, *, out: Optional[VariableLike]=None) -> VariableLike:
+    def ceil(self, *, out: VariableLike | None=None) -> VariableLike:
         ...
 
     @property
     def coords(self) -> Coords:
         ...
 
     def copy(self, deep: bool=True) -> DataArray:
@@ -674,172 +674,172 @@
         ...
 
     @overload
     def deprecated_drop_attrs(self, arg0: str) -> DataArray:
         ...
 
     @overload
-    def deprecated_drop_attrs(self, arg0: List[str]) -> DataArray:
+    def deprecated_drop_attrs(self, arg0: list[str]) -> DataArray:
         ...
 
     @property
     def deprecated_meta(self) -> Coords:
         ...
 
     @property
     def dim(self) -> str:
         ...
 
     @property
-    def dims(self) -> tuple:
+    def dims(self) -> tuple[str, ...]:
         ...
 
     def drop_attrs(self, *args, **kwargs):
         ...
 
     @overload
     def drop_coords(self, arg0: str) -> DataArray:
         ...
 
     @overload
-    def drop_coords(self, arg0: List[str]) -> DataArray:
+    def drop_coords(self, arg0: list[str]) -> DataArray:
         ...
 
     @overload
     def drop_masks(self, arg0: str) -> DataArray:
         ...
 
     @overload
-    def drop_masks(self, arg0: List[str]) -> DataArray:
+    def drop_masks(self, arg0: list[str]) -> DataArray:
         ...
 
     @property
     def dtype(self) -> DType:
         ...
 
-    def flatten(self, dims: Optional[Union[List[str], Tuple[str, ...]]]=None, to: Optional[str]=None) -> VariableLikeType:
+    def flatten(self, dims: list[str] | tuple[str, ...] | None=None, to: str | None=None) -> DataArray:
         ...
 
-    def floor(self, *, out: Optional[VariableLike]=None) -> VariableLike:
+    def floor(self, *, out: VariableLike | None=None) -> VariableLike:
         ...
 
-    def fold(self, dim: str, sizes: Optional[Dict[str, int]]=None, dims: Optional[Union[List[str], Tuple[str, ...]]]=None, shape: Optional[Sequence[int]]=None) -> VariableLikeType:
+    def fold(self, dim: str, sizes: dict[str, int] | None=None, dims: list[str] | tuple[str, ...] | None=None, shape: Sequence[int] | None=None) -> DataArray:
         ...
 
-    def group(self, /, *args: Union[str, Variable]):
+    def group(self, /, *args: str | Variable):
         ...
 
-    def groupby(self, /, group: Union[Variable, str], *, bins: Optional[Variable]=None) -> Union[GroupByDataArray, GroupByDataset]:
+    def groupby(self, /, group: Variable | str, *, bins: Variable | None=None) -> GroupByDataArray | GroupByDataset:
         ...
 
     def hist(self, arg_dict=None, /, **kwargs):
         ...
 
     @property
     def masks(self) -> Masks:
         ...
 
-    def max(self, dim: Optional[str]=None) -> VariableLikeType:
+    def max(self, dim: str | None=None) -> DataArray:
         ...
 
-    def mean(self, dim: Optional[str]=None) -> VariableLikeType:
+    def mean(self, dim: str | None=None) -> DataArray:
         ...
 
-    def median(self, dim: Dims=None) -> VariableLikeType:
+    def median(self, dim: Dims=None) -> DataArray:
         ...
 
     @property
     def meta(self):
         ...
 
-    def min(self, dim: Optional[str]=None) -> VariableLikeType:
+    def min(self, dim: str | None=None) -> DataArray:
         ...
 
     @property
     def name(self) -> str:
         ...
 
     @name.setter
     def name(self, arg1: str) -> None:
         ...
 
     def nanhist(self, arg_dict=None, /, **kwargs):
         ...
 
-    def nanmax(self, dim: Optional[str]=None) -> VariableLikeType:
+    def nanmax(self, dim: str | None=None) -> DataArray:
         ...
 
-    def nanmean(self, dim: Optional[str]=None) -> VariableLikeType:
+    def nanmean(self, dim: str | None=None) -> DataArray:
         ...
 
-    def nanmedian(self, dim: Dims=None) -> VariableLikeType:
+    def nanmedian(self, dim: Dims=None) -> DataArray:
         ...
 
-    def nanmin(self, dim: Optional[str]=None) -> VariableLikeType:
+    def nanmin(self, dim: str | None=None) -> DataArray:
         ...
 
-    def nanstd(self, dim: Dims=None, *, ddof: int) -> VariableLikeType:
+    def nanstd(self, dim: Dims=None, *, ddof: int) -> DataArray:
         ...
 
-    def nansum(self, dim: Optional[str]=None) -> VariableLikeType:
+    def nansum(self, dim: str | None=None) -> DataArray:
         ...
 
-    def nanvar(self, dim: Dims=None, *, ddof: int) -> VariableLikeType:
+    def nanvar(self, dim: Dims=None, *, ddof: int) -> DataArray:
         ...
 
     @property
     def ndim(self) -> int:
         ...
 
-    def plot(*args, **kwargs):
+    def plot(*args: Any, **kwargs: Any) -> None:
         ...
 
     def rebin(self, arg_dict=None, deprecated=None, /, **kwargs):
         ...
 
-    def rename(self, dims_dict: Dict[str, str]=None, /, **names: str) -> DataArray:
+    def rename(self, dims_dict: dict[str, str] | None=None, /, **names: str) -> DataArray:
         ...
 
-    def rename_dims(self, dims_dict: Optional[Dict[str, str]]=None, /, **names: str) -> VariableLikeType:
+    def rename_dims(self, dims_dict: dict[str, str] | None=None, /, **names: str) -> DataArray:
         ...
 
-    def round(self, *, out: Optional[VariableLike]=None) -> VariableLike:
+    def round(self, *, out: VariableLike | None=None) -> VariableLike:
         ...
 
-    def save_hdf5(self, filename: Union[str, Path]) -> None:
+    def save_hdf5(self, filename: str | Path) -> None:
         ...
 
     @property
-    def shape(self) -> tuple:
+    def shape(self) -> tuple[int, ...]:
         ...
 
     @property
     def size(self) -> int:
         ...
 
     @property
-    def sizes(self) -> dict:
+    def sizes(self) -> dict[str, int]:
         ...
 
-    def squeeze(self, dim: Optional[Union[str, List[str], Tuple[str, ...]]]=None) -> VariableLikeType:
+    def squeeze(self, dim: str | list[str] | tuple[str, ...] | None=None) -> DataArray:
         ...
 
-    def std(self, dim: Dims=None, *, ddof: int) -> VariableLikeType:
+    def std(self, dim: Dims=None, *, ddof: int) -> DataArray:
         ...
 
-    def sum(self, dim: Dims=None) -> VariableLikeType:
+    def sum(self, dim: Dims=None) -> DataArray:
         ...
 
-    def to(self, *, unit: Optional[Union[Unit, str]]=None, dtype: Optional[Any]=None, copy: bool=True) -> VariableLikeType:
+    def to(self, *, unit: Unit | str | None=None, dtype: Any | None=None, copy: bool=True) -> DataArray:
         ...
 
-    def transform_coords(self, targets: Optional[Union[str, Iterable[str]]]=None, /, graph: Optional[GraphDict]=None, *, rename_dims: bool=True, keep_aliases: bool=True, keep_intermediate: bool=True, keep_inputs: bool=True, quiet: bool=False, **kwargs: Callable) -> Union[DataArray, Dataset]:
+    def transform_coords(self, targets: str | Iterable[str] | None=None, /, graph: GraphDict | None=None, *, rename_dims: bool=True, keep_aliases: bool=True, keep_intermediate: bool=True, keep_inputs: bool=True, quiet: bool=False, **kwargs: Callable) -> DataArray | Dataset:
         ...
 
-    def transpose(self, dims: Optional[Union[List[str], Tuple[str, ...]]]=None) -> VariableLikeType:
+    def transpose(self, dims: list[str] | tuple[str, ...] | None=None) -> DataArray:
         ...
 
     def underlying_size(self) -> int:
         ...
 
     @property
     def unit(self) -> Optional[Unit]:
@@ -861,15 +861,15 @@
     def values(self) -> Any:
         ...
 
     @values.setter
     def values(self, arg1: Any) -> None:
         ...
 
-    def var(self, dim: Dims=None, *, ddof: int) -> VariableLikeType:
+    def var(self, dim: Dims=None, *, ddof: int) -> DataArray:
         ...
 
     @property
     def variance(self) -> Any:
         ...
 
     @variance.setter
@@ -883,15 +883,15 @@
     @variances.setter
     def variances(self, arg1: Any) -> None:
         ...
 
 class DataArrayError(RuntimeError):
     ...
 
-class Dataset:
+class Dataset(Mapping[str, DataArray]):
 
     def __abs__(self) -> Dataset:
         ...
 
     @overload
     def __add__(self, arg0: Dataset) -> Dataset:
         ...
@@ -932,35 +932,35 @@
         ...
 
     @overload
     def __getitem__(self, arg0: Variable) -> Dataset:
         ...
 
     @overload
-    def __getitem__(self, arg0: Tuple[str, Variable]) -> Dataset:
+    def __getitem__(self, arg0: tuple[str, Variable]) -> Dataset:
         ...
 
     @overload
-    def __getitem__(self, arg0: Tuple[str, int]) -> Dataset:
+    def __getitem__(self, arg0: tuple[str, int]) -> Dataset:
         ...
 
     @overload
-    def __getitem__(self, arg0: Tuple[str, slice]) -> Dataset:
+    def __getitem__(self, arg0: tuple[str, slice]) -> Dataset:
         ...
 
     @overload
     def __getitem__(self, arg0: ellipsis) -> Dataset:
         ...
 
     @overload
-    def __getitem__(self, arg0: List[int]) -> Dataset:
+    def __getitem__(self, arg0: list[int]) -> Dataset:
         ...
 
     @overload
-    def __getitem__(self, arg0: Tuple[str, List[int]]) -> Dataset:
+    def __getitem__(self, arg0: tuple[str, list[int]]) -> Dataset:
         ...
 
     @overload
     def __iadd__(self, arg0: Dataset) -> Dataset:
         ...
 
     @overload
@@ -987,15 +987,15 @@
     def __imul__(self, arg0: Variable) -> Dataset:
         ...
 
     @overload
     def __imul__(self, arg0: float) -> Dataset:
         ...
 
-    def __init__(self, data: Union[Mapping[str, Union[Variable, DataArray]], Iterable[Tuple[str, Union[Variable, DataArray]]]]={}, coords: Union[Mapping[str, Variable], Iterable[Tuple[str, Variable]]]={}) -> None:
+    def __init__(self, data: Union[Mapping[str, Union[Variable, DataArray]], Iterable[tuple[str, Union[Variable, DataArray]]]]={}, coords: Union[Mapping[str, Variable], Iterable[tuple[str, Variable]]]={}) -> None:
         ...
 
     @overload
     def __isub__(self, arg0: Dataset) -> Any:
         ...
 
     @overload
@@ -1006,15 +1006,15 @@
     def __isub__(self, arg0: Variable) -> Any:
         ...
 
     @overload
     def __isub__(self, arg0: float) -> Any:
         ...
 
-    def __iter__(self) -> Iterator:
+    def __iter__(self) -> Iterator[str]:
         ...
 
     @overload
     def __itruediv__(self, arg0: Dataset) -> Dataset:
         ...
 
     @overload
@@ -1052,31 +1052,31 @@
         ...
 
     @overload
     def __setitem__(self, arg0: str, arg1: DataArray) -> None:
         ...
 
     @overload
-    def __setitem__(self, arg0: Tuple[str, Variable], arg1: Dataset) -> None:
+    def __setitem__(self, arg0: tuple[str, Variable], arg1: Dataset) -> None:
         ...
 
     @overload
     def __setitem__(self, arg0: int, arg1: Any) -> None:
         ...
 
     @overload
     def __setitem__(self, arg0: slice, arg1: Any) -> None:
         ...
 
     @overload
-    def __setitem__(self, arg0: Tuple[str, int], arg1: Any) -> None:
+    def __setitem__(self, arg0: tuple[str, int], arg1: Any) -> None:
         ...
 
     @overload
-    def __setitem__(self, arg0: Tuple[str, slice], arg1: Any) -> None:
+    def __setitem__(self, arg0: tuple[str, slice], arg1: Any) -> None:
         ...
 
     @overload
     def __setitem__(self, arg0: ellipsis, arg1: Any) -> None:
         ...
 
     def __sizeof__(self) -> int:
@@ -1105,38 +1105,38 @@
     @overload
     def __truediv__(self, arg0: Variable) -> Dataset:
         ...
 
     def _ipython_key_completions_(self) -> list:
         ...
 
-    def _pop(self, k: str) -> Any:
+    def _pop(self, k: str) -> DataArray:
         ...
 
-    def _rename_dims(self, arg0: Dict[str, str]) -> Dataset:
+    def _rename_dims(self, arg0: dict[str, str]) -> Dataset:
         ...
 
     def _repr_html_(self) -> str:
         ...
 
-    def all(self, dim: Optional[str]=None) -> VariableLikeType:
+    def all(self, dim: str | None=None) -> Dataset:
         ...
 
-    def any(self, dim: Optional[str]=None) -> VariableLikeType:
+    def any(self, dim: str | None=None) -> Dataset:
         ...
 
-    def assign_coords(self, coords: Optional[Dict[str, Variable]]=None, /, **coords_kwargs) -> Union[DataArray, Dataset]:
+    def assign_coords(self, coords: dict[str, Variable] | None=None, /, **coords_kwargs: Variable) -> _T:
         ...
 
     @property
-    def bins(self):
+    def bins(self) -> Bins | None:
         ...
 
     @bins.setter
-    def bins(self, bins: Bins):
+    def bins(self, bins: Bins) -> None:
         ...
 
     def clear(self) -> None:
         ...
 
     @property
     def coords(self) -> Coords:
@@ -1146,171 +1146,171 @@
         ...
 
     @property
     def dim(self) -> str:
         ...
 
     @property
-    def dims(self) -> tuple:
+    def dims(self) -> tuple[str, ...]:
         ...
 
     @overload
     def drop_coords(self, arg0: str) -> Dataset:
         ...
 
     @overload
-    def drop_coords(self, arg0: List[str]) -> Dataset:
+    def drop_coords(self, arg0: list[str]) -> Dataset:
         ...
 
-    def get(self, key, default=None):
+    def get(self, key: str, default: DataArray | None=None) -> DataArray | None:
         ...
 
-    def groupby(self, /, group: Union[Variable, str], *, bins: Optional[Variable]=None) -> Union[GroupByDataArray, GroupByDataset]:
+    def groupby(self, /, group: Variable | str, *, bins: Variable | None=None) -> GroupByDataArray | GroupByDataset:
         ...
 
     def hist(self, arg_dict=None, /, **kwargs):
         ...
 
     def items(self) -> Dataset_items_view:
         ...
 
     def keys(self) -> Dataset_keys_view:
         ...
 
-    def max(self, dim: Optional[str]=None) -> VariableLikeType:
+    def max(self, dim: str | None=None) -> Dataset:
         ...
 
-    def mean(self, dim: Optional[str]=None) -> VariableLikeType:
+    def mean(self, dim: str | None=None) -> Dataset:
         ...
 
-    def median(self, dim: Dims=None) -> VariableLikeType:
+    def median(self, dim: Dims=None) -> Dataset:
         ...
 
     @property
     def meta(self) -> Coords:
         ...
 
-    def min(self, dim: Optional[str]=None) -> VariableLikeType:
+    def min(self, dim: str | None=None) -> Dataset:
         ...
 
-    def nanmax(self, dim: Optional[str]=None) -> VariableLikeType:
+    def nanmax(self, dim: str | None=None) -> Dataset:
         ...
 
-    def nanmean(self, dim: Optional[str]=None) -> VariableLikeType:
+    def nanmean(self, dim: str | None=None) -> Dataset:
         ...
 
-    def nanmedian(self, dim: Dims=None) -> VariableLikeType:
+    def nanmedian(self, dim: Dims=None) -> Dataset:
         ...
 
-    def nanmin(self, dim: Optional[str]=None) -> VariableLikeType:
+    def nanmin(self, dim: str | None=None) -> Dataset:
         ...
 
-    def nanstd(self, dim: Dims=None, *, ddof: int) -> VariableLikeType:
+    def nanstd(self, dim: Dims=None, *, ddof: int) -> Dataset:
         ...
 
-    def nansum(self, dim: Optional[str]=None) -> VariableLikeType:
+    def nansum(self, dim: str | None=None) -> Dataset:
         ...
 
-    def nanvar(self, dim: Dims=None, *, ddof: int) -> VariableLikeType:
+    def nanvar(self, dim: Dims=None, *, ddof: int) -> Dataset:
         ...
 
     @property
     def ndim(self) -> int:
         ...
 
-    def plot(*args, **kwargs):
+    def plot(*args: Any, **kwargs: Any) -> None:
         ...
 
-    def pop(self, key, default=_NoDefault):
+    def pop(self, key: str, default: Any=_NoDefault) -> DataArray | None:
         ...
 
     def rebin(self, arg_dict=None, deprecated=None, /, **kwargs):
         ...
 
-    def rename(self, dims_dict: Dict[str, str]=None, /, **names: str) -> Dataset:
+    def rename(self, dims_dict: dict[str, str] | None=None, /, **names: str) -> Dataset:
         ...
 
-    def rename_dims(self, dims_dict: Optional[Dict[str, str]]=None, /, **names: str) -> VariableLikeType:
+    def rename_dims(self, dims_dict: dict[str, str] | None=None, /, **names: str) -> Dataset:
         ...
 
-    def save_hdf5(self, filename: Union[str, Path]) -> None:
+    def save_hdf5(self, filename: str | Path) -> None:
         ...
 
     @property
-    def shape(self) -> tuple:
+    def shape(self) -> tuple[int, ...]:
         ...
 
     @property
-    def sizes(self) -> dict:
+    def sizes(self) -> dict[str, int]:
         ...
 
-    def squeeze(self, dim: Optional[Union[str, List[str], Tuple[str, ...]]]=None) -> VariableLikeType:
+    def squeeze(self, dim: str | list[str] | tuple[str, ...] | None=None) -> Dataset:
         ...
 
-    def std(self, dim: Dims=None, *, ddof: int) -> VariableLikeType:
+    def std(self, dim: Dims=None, *, ddof: int) -> Dataset:
         ...
 
-    def sum(self, dim: Dims=None) -> VariableLikeType:
+    def sum(self, dim: Dims=None) -> Dataset:
         ...
 
-    def transform_coords(self, targets: Optional[Union[str, Iterable[str]]]=None, /, graph: Optional[GraphDict]=None, *, rename_dims: bool=True, keep_aliases: bool=True, keep_intermediate: bool=True, keep_inputs: bool=True, quiet: bool=False, **kwargs: Callable) -> Union[DataArray, Dataset]:
+    def transform_coords(self, targets: str | Iterable[str] | None=None, /, graph: GraphDict | None=None, *, rename_dims: bool=True, keep_aliases: bool=True, keep_intermediate: bool=True, keep_inputs: bool=True, quiet: bool=False, **kwargs: Callable) -> DataArray | Dataset:
         ...
 
     def underlying_size(self) -> int:
         ...
 
     def update(self, other: Any=None, /, **kwargs) -> None:
         ...
 
     def values(self) -> Dataset_values_view:
         ...
 
-    def var(self, dim: Dims=None, *, ddof: int) -> VariableLikeType:
+    def var(self, dim: Dims=None, *, ddof: int) -> Dataset:
         ...
 
 class DatasetError(RuntimeError):
     ...
 
 class Dataset_items_view:
 
-    def __eq__(self, arg0: object) -> bool:  # type: ignore[override]
+    def __eq__(self, arg0: object) -> bool:  # type: ignore[override, unused-ignore]
         ...
 
-    def __iter__(self) -> Iterator:
+    def __iter__(self) -> Iterator[tuple[str, DataArray]]:
         ...
 
     def __len__(self) -> int:
         ...
 
     def __repr__(self) -> str:
         ...
 
     def __str__(self) -> str:
         ...
 
 class Dataset_keys_view:
 
-    def __eq__(self, arg0: object) -> bool:  # type: ignore[override]
+    def __eq__(self, arg0: object) -> bool:  # type: ignore[override, unused-ignore]
         ...
 
-    def __iter__(self) -> Iterator:
+    def __iter__(self) -> Iterator[str]:
         ...
 
     def __len__(self) -> int:
         ...
 
     def __repr__(self) -> str:
         ...
 
     def __str__(self) -> str:
         ...
 
 class Dataset_values_view:
 
-    def __iter__(self) -> Iterator:
+    def __iter__(self) -> Iterator[DataArray]:
         ...
 
     def __len__(self) -> int:
         ...
 
     def __repr__(self) -> str:
         ...
@@ -1331,15 +1331,15 @@
     def all(self, dim: str) -> DataArray:
         ...
 
     def any(self, dim: str) -> DataArray:
         ...
 
     @property
-    def bins(self):
+    def bins(self) -> GroupbyBins:
         ...
 
     def concat(self, dim: str) -> DataArray:
         ...
 
     def max(self, dim: str) -> DataArray:
         ...
@@ -1367,15 +1367,15 @@
     def all(self, dim: str) -> Dataset:
         ...
 
     def any(self, dim: str) -> Dataset:
         ...
 
     @property
-    def bins(self):
+    def bins(self) -> GroupbyBins:
         ...
 
     def concat(self, dim: str) -> Dataset:
         ...
 
     def max(self, dim: str) -> Dataset:
         ...
@@ -1394,125 +1394,125 @@
 
     def nansum(self, dim: str) -> Dataset:
         ...
 
     def sum(self, dim: str) -> Dataset:
         ...
 
-class Masks:
+class Masks(Mapping[str, Variable]):
 
     def __contains__(self, arg0: str) -> bool:
         ...
 
     def __copy__(self) -> Masks:
         ...
 
     def __deepcopy__(self, arg0: dict) -> Masks:
         ...
 
     def __delitem__(self, arg0: str) -> None:
         ...
 
-    def __eq__(self, arg0: object) -> bool:  # type: ignore[override]
+    def __eq__(self, arg0: object) -> bool:  # type: ignore[override, unused-ignore]
         ...
 
     def __getitem__(self, arg0: str) -> Variable:
         ...
 
-    def __iter__(self) -> Iterator:
+    def __iter__(self) -> Iterator[str]:
         ...
 
     def __len__(self) -> int:
         ...
 
-    def __ne__(self, arg0: object) -> bool:  # type: ignore[override]
+    def __ne__(self, arg0: object) -> bool:  # type: ignore[override, unused-ignore]
         ...
 
     def __repr__(self) -> str:
         ...
 
     def __setitem__(self, arg0: str, arg1: Variable) -> None:
         ...
 
     def __str__(self) -> str:
         ...
 
     def _ipython_key_completions_(self) -> list:
         ...
 
-    def _pop(self, k: str) -> Any:
+    def _pop(self, k: str) -> Variable:
         ...
 
     def clear(self) -> None:
         ...
 
     def copy(self, deep: bool=True) -> Masks:
         ...
 
-    def get(self, key, default=None):
+    def get(self, key: str, default: Variable | None=None) -> Variable | None:
         ...
 
     def is_edges(self, key: str, dim: Optional[str]=None) -> bool:
         ...
 
     def items(self) -> Masks_items_view:
         ...
 
     def keys(self) -> Masks_keys_view:
         ...
 
-    def pop(self, key, default=_NoDefault):
+    def pop(self, key: str, default: Any=_NoDefault) -> Variable | None:
         ...
 
-    def popitem(self) -> Tuple[str, Any]:
+    def popitem(self) -> tuple[str, Variable]:
         ...
 
     def update(self, other: Any=None, /, **kwargs) -> None:
         ...
 
     def values(self) -> Masks_values_view:
         ...
 
 class Masks_items_view:
 
-    def __eq__(self, arg0: object) -> bool:  # type: ignore[override]
+    def __eq__(self, arg0: object) -> bool:  # type: ignore[override, unused-ignore]
         ...
 
-    def __iter__(self) -> Iterator:
+    def __iter__(self) -> Iterator[tuple[str, Variable]]:
         ...
 
     def __len__(self) -> int:
         ...
 
     def __repr__(self) -> str:
         ...
 
     def __str__(self) -> str:
         ...
 
 class Masks_keys_view:
 
-    def __eq__(self, arg0: object) -> bool:  # type: ignore[override]
+    def __eq__(self, arg0: object) -> bool:  # type: ignore[override, unused-ignore]
         ...
 
-    def __iter__(self) -> Iterator:
+    def __iter__(self) -> Iterator[str]:
         ...
 
     def __len__(self) -> int:
         ...
 
     def __repr__(self) -> str:
         ...
 
     def __str__(self) -> str:
         ...
 
 class Masks_values_view:
 
-    def __iter__(self) -> Iterator:
+    def __iter__(self) -> Iterator[Variable]:
         ...
 
     def __len__(self) -> int:
         ...
 
     def __repr__(self) -> str:
         ...
@@ -1527,27 +1527,27 @@
 
     def __abs__(self) -> Unit:
         ...
 
     def __add__(self, arg0: Unit) -> Unit:
         ...
 
-    def __eq__(self, arg0: object) -> bool:  # type: ignore[override]
+    def __eq__(self, arg0: object) -> bool:  # type: ignore[override, unused-ignore]
         ...
 
     def __hash__(self) -> int:
         ...
 
     def __init__(self, arg0: str) -> None:
         ...
 
     def __mul__(self, arg0: Unit) -> Unit:
         ...
 
-    def __ne__(self, arg0: object) -> bool:  # type: ignore[override]
+    def __ne__(self, arg0: object) -> bool:  # type: ignore[override, unused-ignore]
         ...
 
     def __pow__(self, arg0: int) -> Unit:
         ...
 
     def __repr__(self) -> str:
         ...
@@ -1611,15 +1611,15 @@
 
     def __copy__(self) -> Variable:
         ...
 
     def __deepcopy__(self, arg0: dict) -> Variable:
         ...
 
-    def __eq__(self, arg0: object) -> Variable:  # type: ignore[override]
+    def __eq__(self, arg0: object) -> Variable:  # type: ignore[override, unused-ignore]
         ...
 
     def __float__(self) -> float:
         ...
 
     @overload
     def __floordiv__(self, arg0: Variable) -> Variable:
@@ -1653,31 +1653,31 @@
         ...
 
     @overload
     def __getitem__(self, arg0: Variable) -> Variable:
         ...
 
     @overload
-    def __getitem__(self, arg0: Tuple[str, int]) -> Variable:
+    def __getitem__(self, arg0: tuple[str, int]) -> Variable:
         ...
 
     @overload
-    def __getitem__(self, arg0: Tuple[str, slice]) -> Variable:
+    def __getitem__(self, arg0: tuple[str, slice]) -> Variable:
         ...
 
     @overload
     def __getitem__(self, arg0: ellipsis) -> Variable:
         ...
 
     @overload
-    def __getitem__(self, arg0: List[int]) -> Variable:
+    def __getitem__(self, arg0: list[int]) -> Variable:
         ...
 
     @overload
-    def __getitem__(self, arg0: Tuple[str, List[int]]) -> Variable:
+    def __getitem__(self, arg0: tuple[str, list[int]]) -> Variable:
         ...
 
     @overload
     def __gt__(self, arg0: Variable) -> Variable:
         ...
 
     @overload
@@ -1797,15 +1797,15 @@
     def __mul__(self, arg0: DataArray) -> DataArray:
         ...
 
     @overload
     def __mul__(self, arg0: float) -> Variable:
         ...
 
-    def __ne__(self, arg0: object) -> Variable:  # type: ignore[override]
+    def __ne__(self, arg0: object) -> Variable:  # type: ignore[override, unused-ignore]
         ...
 
     def __neg__(self) -> Variable:
         ...
 
     def __or__(self, arg0: Variable) -> Variable:
         ...
@@ -1851,19 +1851,19 @@
         ...
 
     @overload
     def __setitem__(self, arg0: slice, arg1: Any) -> None:
         ...
 
     @overload
-    def __setitem__(self, arg0: Tuple[str, int], arg1: Any) -> None:
+    def __setitem__(self, arg0: tuple[str, int], arg1: Any) -> None:
         ...
 
     @overload
-    def __setitem__(self, arg0: Tuple[str, slice], arg1: Any) -> None:
+    def __setitem__(self, arg0: tuple[str, slice], arg1: Any) -> None:
         ...
 
     @overload
     def __setitem__(self, arg0: ellipsis, arg1: Any) -> None:
         ...
 
     def __sizeof__(self) -> int:
@@ -1895,164 +1895,164 @@
 
     def __xor__(self, arg0: Variable) -> Variable:
         ...
 
     def _ipython_key_completions_(self) -> list:
         ...
 
-    def _rename_dims(self, arg0: Dict[str, str]) -> Variable:
+    def _rename_dims(self, arg0: dict[str, str]) -> Variable:
         ...
 
     def _repr_html_(self) -> str:
         ...
 
     @property
     def aligned(self) -> bool:
         ...
 
-    def all(self, dim: Optional[str]=None) -> VariableLikeType:
+    def all(self, dim: str | None=None) -> Variable:
         ...
 
-    def any(self, dim: Optional[str]=None) -> VariableLikeType:
+    def any(self, dim: str | None=None) -> Variable:
         ...
 
     def astype(self, type: Any, *, copy: bool=True) -> Variable:
         ...
 
     def bin(self, arg_dict=None, /, **kwargs):
         ...
 
     @property
-    def bins(self):
+    def bins(self) -> Bins | None:
         ...
 
     @bins.setter
-    def bins(self, bins: Bins):
+    def bins(self, bins: Bins) -> None:
         ...
 
-    def broadcast(self, dims: Optional[Union[List[str], Tuple[str, ...]]]=None, shape: Optional[Sequence[int]]=None, sizes: Optional[Dict[str, int]]=None) -> VariableLikeType:
+    def broadcast(self, dims: list[str] | tuple[str, ...] | None=None, shape: Sequence[int] | None=None, sizes: dict[str, int] | None=None) -> Variable:
         ...
 
-    def ceil(self, *, out: Optional[VariableLike]=None) -> VariableLike:
+    def ceil(self, *, out: VariableLike | None=None) -> VariableLike:
         ...
 
     def copy(self, deep: bool=True) -> Variable:
         ...
 
-    def cumsum(self, dim: Optional[str]=None, mode: Literal['exclusive', 'inclusive']='inclusive') -> VariableLikeType:
+    def cumsum(self, dim: str | None=None, mode: Literal['exclusive', 'inclusive']='inclusive') -> Variable:
         ...
 
     @property
     def dim(self) -> str:
         ...
 
     @property
-    def dims(self) -> tuple:
+    def dims(self) -> tuple[str, ...]:
         ...
 
     @property
     def dtype(self) -> DType:
         ...
 
     @property
-    def fields(self):
+    def fields(self) -> Any:
         ...
 
-    def flatten(self, dims: Optional[Union[List[str], Tuple[str, ...]]]=None, to: Optional[str]=None) -> VariableLikeType:
+    def flatten(self, dims: list[str] | tuple[str, ...] | None=None, to: str | None=None) -> Variable:
         ...
 
-    def floor(self, *, out: Optional[VariableLike]=None) -> VariableLike:
+    def floor(self, *, out: VariableLike | None=None) -> VariableLike:
         ...
 
-    def fold(self, dim: str, sizes: Optional[Dict[str, int]]=None, dims: Optional[Union[List[str], Tuple[str, ...]]]=None, shape: Optional[Sequence[int]]=None) -> VariableLikeType:
+    def fold(self, dim: str, sizes: dict[str, int] | None=None, dims: list[str] | tuple[str, ...] | None=None, shape: Sequence[int] | None=None) -> Variable:
         ...
 
     def hist(self, arg_dict=None, /, **kwargs):
         ...
 
-    def max(self, dim: Optional[str]=None) -> VariableLikeType:
+    def max(self, dim: str | None=None) -> Variable:
         ...
 
-    def mean(self, dim: Optional[str]=None) -> VariableLikeType:
+    def mean(self, dim: str | None=None) -> Variable:
         ...
 
-    def median(self, dim: Dims=None) -> VariableLikeType:
+    def median(self, dim: Dims=None) -> Variable:
         ...
 
-    def min(self, dim: Optional[str]=None) -> VariableLikeType:
+    def min(self, dim: str | None=None) -> Variable:
         ...
 
     def nanhist(self, arg_dict=None, /, **kwargs):
         ...
 
-    def nanmax(self, dim: Optional[str]=None) -> VariableLikeType:
+    def nanmax(self, dim: str | None=None) -> Variable:
         ...
 
-    def nanmean(self, dim: Optional[str]=None) -> VariableLikeType:
+    def nanmean(self, dim: str | None=None) -> Variable:
         ...
 
-    def nanmedian(self, dim: Dims=None) -> VariableLikeType:
+    def nanmedian(self, dim: Dims=None) -> Variable:
         ...
 
-    def nanmin(self, dim: Optional[str]=None) -> VariableLikeType:
+    def nanmin(self, dim: str | None=None) -> Variable:
         ...
 
-    def nanstd(self, dim: Dims=None, *, ddof: int) -> VariableLikeType:
+    def nanstd(self, dim: Dims=None, *, ddof: int) -> Variable:
         ...
 
-    def nansum(self, dim: Optional[str]=None) -> VariableLikeType:
+    def nansum(self, dim: str | None=None) -> Variable:
         ...
 
-    def nanvar(self, dim: Dims=None, *, ddof: int) -> VariableLikeType:
+    def nanvar(self, dim: Dims=None, *, ddof: int) -> Variable:
         ...
 
     @property
     def ndim(self) -> int:
         ...
 
-    def plot(*args, **kwargs):
+    def plot(*args: Any, **kwargs: Any) -> None:
         ...
 
-    def rename(self, dims_dict: Dict[str, str]=None, /, **names: str) -> Variable:
+    def rename(self, dims_dict: dict[str, str] | None=None, /, **names: str) -> Variable:
         ...
 
-    def rename_dims(self, dims_dict: Optional[Dict[str, str]]=None, /, **names: str) -> VariableLikeType:
+    def rename_dims(self, dims_dict: dict[str, str] | None=None, /, **names: str) -> Variable:
         ...
 
-    def round(self, *, out: Optional[VariableLike]=None) -> VariableLike:
+    def round(self, *, out: VariableLike | None=None) -> VariableLike:
         ...
 
-    def save_hdf5(self, filename: Union[str, Path]) -> None:
+    def save_hdf5(self, filename: str | Path) -> None:
         ...
 
     @property
-    def shape(self) -> tuple:
+    def shape(self) -> tuple[int, ...]:
         ...
 
     @property
     def size(self) -> int:
         ...
 
     @property
-    def sizes(self) -> dict:
+    def sizes(self) -> dict[str, int]:
         ...
 
-    def squeeze(self, dim: Optional[Union[str, List[str], Tuple[str, ...]]]=None) -> VariableLikeType:
+    def squeeze(self, dim: str | list[str] | tuple[str, ...] | None=None) -> Variable:
         ...
 
-    def std(self, dim: Dims=None, *, ddof: int) -> VariableLikeType:
+    def std(self, dim: Dims=None, *, ddof: int) -> Variable:
         ...
 
-    def sum(self, dim: Dims=None) -> VariableLikeType:
+    def sum(self, dim: Dims=None) -> Variable:
         ...
 
-    def to(self, *, unit: Optional[Union[Unit, str]]=None, dtype: Optional[Any]=None, copy: bool=True) -> VariableLikeType:
+    def to(self, *, unit: Unit | str | None=None, dtype: Any | None=None, copy: bool=True) -> Variable:
         ...
 
-    def transpose(self, dims: Optional[Union[List[str], Tuple[str, ...]]]=None) -> VariableLikeType:
+    def transpose(self, dims: list[str] | tuple[str, ...] | None=None) -> Variable:
         ...
 
     def underlying_size(self) -> int:
         ...
 
     @property
     def unit(self) -> Optional[Unit]:
@@ -2074,15 +2074,15 @@
     def values(self) -> Any:
         ...
 
     @values.setter
     def values(self, arg1: Any) -> None:
         ...
 
-    def var(self, dim: Dims=None, *, ddof: int) -> VariableLikeType:
+    def var(self, dim: Dims=None, *, ddof: int) -> Variable:
         ...
 
     @property
     def variance(self) -> Any:
         ...
 
     @variance.setter
@@ -2097,8 +2097,8 @@
     def variances(self, arg1: Any) -> None:
         ...
 
 class VariableError(RuntimeError):
     ...
 
 class VariancesError(RuntimeError):
-    ...
+    ...
```

### Comparing `scipp-24.2.0/src/scipp/core/cumulative.py` & `scipp-24.5.0/src/scipp/core/cumulative.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
 
-from typing import Literal, Optional
+from typing import Literal
 
 from .._scipp import core as _cpp
 from ..typing import VariableLikeType
 from ._cpp_wrapper_util import call_func as _call_cpp_func
 from .concepts import transform_data
 
 
 def cumsum(
     a: VariableLikeType,
-    dim: Optional[str] = None,
+    dim: str | None = None,
     mode: Literal['exclusive', 'inclusive'] = 'inclusive',
 ) -> VariableLikeType:
     """Return the cumulative sum along the specified dimension.
 
     See :py:func:`scipp.sum` on how rounding errors for float32 inputs are handled.
 
     Parameters
```

### Comparing `scipp-24.2.0/src/scipp/core/data_group.py` & `scipp-24.5.0/src/scipp/core/data_group.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,21 @@
 from __future__ import annotations
 
 import copy
 import functools
 import itertools
 import numbers
 import operator
-from collections.abc import MutableMapping
+from collections.abc import Callable, Iterable, MutableMapping
 from functools import wraps
 from typing import (
     TYPE_CHECKING,
     Any,
-    Callable,
-    Dict,
-    Iterable,
     NoReturn,
-    Optional,
-    Tuple,
     TypeVar,
-    Union,
     cast,
     overload,
 )
 
 import numpy as np
 
 from .. import _binding
@@ -53,17 +47,17 @@
     if isinstance(item, Bins):
         return True
     return hasattr(item, 'bins') and item.bins is not None
 
 
 def _summarize(item):
     if isinstance(item, DataGroup):
-        return f'{type(item).__name__}({len(item)}, {item.sizes})\n'
+        return f'{type(item).__name__}({len(item)}, {item.sizes})'
     if hasattr(item, 'sizes'):
-        return f'{type(item).__name__}({item.sizes})\n'
+        return f'{type(item).__name__}({item.sizes})'
     return str(item)
 
 
 def _is_positional_index(key) -> bool:
     def is_int(x):
         return isinstance(x, numbers.Integral)
 
@@ -74,15 +68,15 @@
             return True
         if key.start is None and key.stop is None and key.step is None:
             return True
     return False
 
 
 def _is_list_index(key) -> bool:
-    return isinstance(key, (list, np.ndarray))
+    return isinstance(key, list | np.ndarray)
 
 
 class DataGroup(MutableMapping):
     """
     A dict-like group of data. Additionally provides dims and shape properties.
 
     DataGroup acts like a Python dict but additionally supports Scipp functionality
@@ -91,34 +85,32 @@
     structures.
 
     .. versionadded:: 23.01.0
     """
 
     def __init__(self, /, *args, **kwargs):
         self._items = dict(*args, **kwargs)
-        if not all([isinstance(k, str) for k in self._items.keys()]):
+        if not all(isinstance(k, str) for k in self._items.keys()):
             raise ValueError("DataGroup keys must be strings.")
 
     def __copy__(self) -> DataGroup:
         return DataGroup(copy.copy(self._items))
 
     def __len__(self) -> int:
         """Return the number of items in the data group."""
         return len(self._items)
 
     def __iter__(self):
         yield from self._items
 
     @overload
-    def __getitem__(self, name: str) -> Any:
-        ...
+    def __getitem__(self, name: str) -> Any: ...
 
     @overload
-    def __getitem__(self, name: ScippIndex) -> DataGroup:
-        ...
+    def __getitem__(self, name: ScippIndex) -> DataGroup: ...
 
     def __getitem__(self, name):
         """Return item of given name or index all items.
 
         When ``name`` is a string, return the item of the given name. Otherwise, this
         returns a new DataGroup, with items created by indexing the items in this
         DataGroup. This may perform, e.g., Scipp's positional indexing, label-based
@@ -160,16 +152,15 @@
                 if (isinstance(var, Bins) or dim in _item_dims(var))
                 else var
                 for key, var in self.items()
             }
         )
 
     @overload
-    def __setitem__(self, name: str, value: Any):
-        ...
+    def __setitem__(self, name: str, value: Any): ...
 
     def __setitem__(self, name, value):
         """Set self[key] to value."""
         if isinstance(name, str):
             self._items[name] = value
         else:
             raise TypeError('Keys must be strings')
@@ -181,40 +172,40 @@
     def __sizeof__(self) -> int:
         return self.underlying_size()
 
     def underlying_size(self) -> int:
         # TODO Return the underlying size of all items in DataGroup
         total_size = super.__sizeof__(self)
         for item in self.values():
-            if isinstance(item, (DataArray, Dataset, Variable, DataGroup)):
+            if isinstance(item, DataArray | Dataset | Variable | DataGroup):
                 total_size += item.underlying_size()
             elif hasattr(item, 'nbytes'):
                 total_size += item.nbytes
             else:
                 total_size += item.__sizeof__()
 
         return total_size
 
     @property
-    def dims(self) -> Tuple[Optional[str], ...]:
+    def dims(self) -> tuple[str | None, ...]:
         """Union of dims of all items. Non-Scipp items are handled as dims=()."""
         return tuple(self.sizes)
 
     @property
     def ndim(self):
         """Number of dimensions, i.e., len(self.dims)."""
         return len(self.dims)
 
     @property
-    def shape(self) -> Tuple[Optional[int], ...]:
+    def shape(self) -> tuple[int | None, ...]:
         """Union of shape of all items. Non-Scipp items are handled as shape=()."""
         return tuple(self.sizes.values())
 
     @property
-    def sizes(self) -> Dict[str, Optional[int]]:
+    def sizes(self) -> dict[str, int | None]:
         """Dict combining dims and shape, i.e., mapping dim labels to their size."""
         all_sizes = {}
         for x in self.values():
             for dim, size in getattr(x, 'sizes', {}).items():
                 all_sizes.setdefault(dim, set()).add(size)
         return {d: next(iter(s)) if len(s) == 1 else None for d, s in all_sizes.items()}
 
@@ -222,15 +213,15 @@
         from ..visualization.formatting_datagroup_html import datagroup_repr
 
         return datagroup_repr(self)
 
     def __repr__(self):
         r = f'DataGroup(sizes={self.sizes}, keys=[\n'
         for name, var in self.items():
-            r += f'    {name}: {_summarize(var)[:-1]},\n'
+            r += f'    {name}: {_summarize(var)},\n'
         r += '])'
         return r
 
     def __str__(self):
         return f'DataGroup(sizes={self.sizes}, keys={list(self.keys())})'
 
     @property
@@ -240,15 +231,15 @@
         return self.apply(operator.attrgetter('bins'))
 
     def apply(self, func: Callable, *args, **kwargs) -> DataGroup:
         """Call func on all values and return new DataGroup containing the results."""
         return DataGroup({key: func(v, *args, **kwargs) for key, v in self.items()})
 
     def _transform_dim(
-        self, func: Callable, *, dim: Union[None, str, Iterable[str]], **kwargs
+        self, func: Callable, *, dim: None | str | Iterable[str], **kwargs
     ) -> DataGroup:
         """Transform items that depend on one or more dimensions given by `dim`."""
         dims = (dim,) if isinstance(dim, str) else dim
 
         def intersects(item):
             item_dims = _item_dims(item)
             if dims is None:
@@ -261,20 +252,20 @@
                 if not intersects(v)
                 else operator.methodcaller(func, dim, **kwargs)(v)
                 for key, v in self.items()
             }
         )
 
     def _reduce(
-        self, method: str, dim: Union[None, str, Tuple[str, ...]] = None, **kwargs
+        self, method: str, dim: None | str | tuple[str, ...] = None, **kwargs
     ) -> DataGroup:
         reduce_all = operator.methodcaller(method, **kwargs)
 
         def _reduce_child(v, dim):
-            if isinstance(v, (GroupByDataArray, GroupByDataset)):
+            if isinstance(v, GroupByDataArray | GroupByDataset):
                 child_dims = (dim,)
             else:
                 child_dims = _item_dims(v)
             # Reduction operations on binned data implicitly reduce over bin content.
             # Therefore, a purely dimension-based logic is not sufficient to determine
             # if the item has to be reduced or not.
             binned = _is_binned(v)
@@ -286,15 +277,15 @@
                 dims_to_reduce = dim if dim in child_dims else ()
             else:
                 dims_to_reduce = tuple(d for d in dim if d in child_dims)
             if dims_to_reduce == () and binned:
                 return reduce_all(v)
             return (
                 v
-                if dims_to_reduce == tuple()
+                if dims_to_reduce == ()
                 else operator.methodcaller(method, dims_to_reduce, **kwargs)(v)
             )
 
         return DataGroup({key: _reduce_child(v, dim) for key, v in self.items()})
 
     def copy(self, deep: bool = True) -> DataGroup:
         return copy.deepcopy(self) if deep else copy.copy(self)
@@ -313,15 +304,15 @@
 
     def broadcast(self, *args, **kwargs):
         return self.apply(operator.methodcaller('broadcast', *args, **kwargs))
 
     def ceil(self, *args, **kwargs):
         return self.apply(operator.methodcaller('ceil', *args, **kwargs))
 
-    def flatten(self, dims: Union[None, Iterable[str]] = None, **kwargs):
+    def flatten(self, dims: None | Iterable[str] = None, **kwargs):
         return self._transform_dim('flatten', dim=dims, **kwargs)
 
     def floor(self, *args, **kwargs):
         return self.apply(operator.methodcaller('floor', *args, **kwargs))
 
     def fold(self, dim: str, **kwargs):
         return self._transform_dim('fold', dim=dim, **kwargs)
@@ -394,159 +385,159 @@
 
     def to(self, *args, **kwargs):
         return self.apply(operator.methodcaller('to', *args, **kwargs))
 
     def transform_coords(self, *args, **kwargs):
         return self.apply(operator.methodcaller('transform_coords', *args, **kwargs))
 
-    def transpose(self, dims: Union[None, Tuple[str, ...]] = None):
+    def transpose(self, dims: None | tuple[str, ...] = None):
         return self._transform_dim('transpose', dim=dims)
 
     def var(self, *args, **kwargs):
         return self._reduce('var', *args, **kwargs)
 
     def plot(self, *args, **kwargs):
         import plopp
 
         return plopp.plot(self, *args, **kwargs)
 
     def __eq__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Item-wise equal."""
         return data_group_nary(operator.eq, self, other)
 
     def __ne__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Item-wise not-equal."""
         return data_group_nary(operator.ne, self, other)
 
     def __gt__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Item-wise greater-than."""
         return data_group_nary(operator.gt, self, other)
 
     def __ge__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Item-wise greater-equal."""
         return data_group_nary(operator.ge, self, other)
 
     def __lt__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Item-wise less-than."""
         return data_group_nary(operator.lt, self, other)
 
     def __le__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Item-wise less-equal."""
         return data_group_nary(operator.le, self, other)
 
     def __add__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Apply ``add`` item-by-item."""
         return data_group_nary(operator.add, self, other)
 
     def __sub__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Apply ``sub`` item-by-item."""
         return data_group_nary(operator.sub, self, other)
 
     def __mul__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Apply ``mul`` item-by-item."""
         return data_group_nary(operator.mul, self, other)
 
     def __truediv__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Apply ``truediv`` item-by-item."""
         return data_group_nary(operator.truediv, self, other)
 
     def __floordiv__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Apply ``floordiv`` item-by-item."""
         return data_group_nary(operator.floordiv, self, other)
 
     def __mod__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Apply ``mod`` item-by-item."""
         return data_group_nary(operator.mod, self, other)
 
     def __pow__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Apply ``pow`` item-by-item."""
         return data_group_nary(operator.pow, self, other)
 
     def __radd__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Apply ``add`` item-by-item."""
         return data_group_nary(operator.add, other, self)
 
     def __rsub__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Apply ``sub`` item-by-item."""
         return data_group_nary(operator.sub, other, self)
 
     def __rmul__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Apply ``mul`` item-by-item."""
         return data_group_nary(operator.mul, other, self)
 
     def __rtruediv__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Apply ``truediv`` item-by-item."""
         return data_group_nary(operator.truediv, other, self)
 
     def __rfloordiv__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Apply ``floordiv`` item-by-item."""
         return data_group_nary(operator.floordiv, other, self)
 
     def __rmod__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Apply ``mod`` item-by-item."""
         return data_group_nary(operator.mod, other, self)
 
     def __rpow__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Apply ``pow`` item-by-item."""
         return data_group_nary(operator.pow, other, self)
 
     def __and__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Return the element-wise ``and`` of items."""
         return data_group_nary(operator.and_, self, other)
 
     def __or__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Return the element-wise ``or`` of items."""
         return data_group_nary(operator.or_, self, other)
 
     def __xor__(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
+        self, other: DataGroup | DataArray | Variable | numbers.Real
     ) -> DataGroup:
         """Return the element-wise ``xor`` of items."""
         return data_group_nary(operator.xor, self, other)
 
     def __invert__(self) -> DataGroup:
         """Return the element-wise ``or`` of items."""
         return self.apply(operator.invert)
@@ -631,17 +622,15 @@
 # it is simpler than for DataGroup because the latter supports more data types.
 # So for now, we went with the simple solution and
 # not support in-place operations at all.
 #
 # Binding these functions dynamically has the added benefit that type checkers think
 # that the operations are not implemented.
 def _make_inplace_binary_op(name: str):
-    def impl(
-        self, other: Union[DataGroup, DataArray, Variable, numbers.Real]
-    ) -> NoReturn:
+    def impl(self, other: DataGroup | DataArray | Variable | numbers.Real) -> NoReturn:
         raise TypeError(f'In-place operation i{name} is not supported by DataGroup.')
 
     return impl
 
 
 for _name in ('add', 'sub', 'mul', 'truediv', 'floordiv', 'mod', 'pow'):
     full_name = f'__i{_name}__'
```

### Comparing `scipp-24.2.0/src/scipp/core/deprecation.py` & `scipp-24.5.0/src/scipp/core/deprecation.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 def _warn_attr_removal():
     warnings.warn(
         "sc.DataArray.attrs has been deprecated and will be removed in Scipp v24.12.0. "
         "The deprecation includes sc.DataArray.meta and sc.DataArray.drop_attrs. "
         "For unaligned coords, use sc.DataArray.coords and unset the alignment flag. "
         "For other attributes, use a higher-level data structure.",
         VisibleDeprecationWarning,
+        stacklevel=3,
     )
 
 
 def _deprecated_attrs(cls):
     """
     Dict of attrs.
```

### Comparing `scipp-24.2.0/src/scipp/core/dimensions.py` & `scipp-24.5.0/src/scipp/core/dimensions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
-from typing import Dict, Optional
 
 from .._scipp.core import CoordError, DataArray, Dataset, Variable
 from ..typing import VariableLikeType
 from .argument_handlers import combine_dict_args
 from .bins import bins
 from .variable import scalar
 
 
 def _rename_dims(
-    self: VariableLikeType, dims_dict: Optional[Dict[str, str]] = None, /, **names: str
+    self: VariableLikeType, dims_dict: dict[str, str] | None = None, /, **names: str
 ) -> VariableLikeType:
     """Rename dimensions.
 
     The renaming can be defined:
 
     - using a dict mapping the old to new names, e.g.
       ``rename_dims({'x': 'a', 'y': 'b'})``
@@ -40,15 +39,15 @@
     :
         A new object with renamed dimensions.
     """
     return self._rename_dims(combine_dict_args(dims_dict, names))
 
 
 def _rename_variable(
-    var: Variable, dims_dict: Dict[str, str] = None, /, **names: str
+    var: Variable, dims_dict: dict[str, str] | None = None, /, **names: str
 ) -> Variable:
     """Rename dimension labels.
 
     The renaming can be defined:
 
     - using a dict mapping the old to new names, e.g. ``rename({'x': 'a', 'y': 'b'})``
     - using keyword arguments, e.g. ``rename(x='a', y='b')``
@@ -74,15 +73,15 @@
     scipp.Variable.rename_dims:
         Equivalent for ``Variable`` but differs for ``DataArray`` and ``Dataset``.
     """
     return var.rename_dims(combine_dict_args(dims_dict, names))
 
 
 def _rename_data_array(
-    da: DataArray, dims_dict: Dict[str, str] = None, /, **names: str
+    da: DataArray, dims_dict: dict[str, str] | None = None, /, **names: str
 ) -> DataArray:
     """Rename the dimensions, coordinates, and attributes.
 
     The renaming can be defined:
 
     - using a dict mapping the old to new names, e.g. ``rename({'x': 'a', 'y': 'b'})``
     - using keyword arguments, e.g. ``rename(x='a', y='b')``
@@ -126,15 +125,15 @@
             for meta in (out.bins.coords, out.bins.deprecated_attrs):
                 if old in meta:
                     meta[new] = meta.pop(old)
     return out
 
 
 def _rename_dataset(
-    ds: Dataset, dims_dict: Dict[str, str] = None, /, **names: str
+    ds: Dataset, dims_dict: dict[str, str] | None = None, /, **names: str
 ) -> Dataset:
     """Rename the dimensions, coordinates and attributes of all the items.
 
     The renaming can be defined:
 
     - using a dict mapping the old to new names, e.g. ``rename({'x': 'a', 'y': 'b'})``
     - using keyword arguments, e.g. ``rename(x='a', y='b')``
```

### Comparing `scipp-24.2.0/src/scipp/core/domains.py` & `scipp-24.5.0/src/scipp/core/domains.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/src/scipp/core/hyperbolic.py` & `scipp-24.5.0/src/scipp/core/hyperbolic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from __future__ import annotations
 
-from typing import Optional
-
 from .._scipp import core as _cpp
 from ..typing import VariableLikeType
 from ._cpp_wrapper_util import call_func as _call_cpp_func
 
 
 def sinh(
-    x: VariableLikeType, *, out: Optional[VariableLikeType] = None
+    x: VariableLikeType, *, out: VariableLikeType | None = None
 ) -> VariableLikeType:
     """Element-wise hyperbolic sine.
 
     The input unit must be dimensionless.
 
     Parameters
     ----------
@@ -29,15 +27,15 @@
     : Same type as input
         The hyperbolic sine values of the input.
     """
     return _call_cpp_func(_cpp.sinh, x, out=out)
 
 
 def cosh(
-    x: VariableLikeType, *, out: Optional[VariableLikeType] = None
+    x: VariableLikeType, *, out: VariableLikeType | None = None
 ) -> VariableLikeType:
     """Element-wise hyperbolic cosine.
 
     The input unit must be dimensionless.
 
     Parameters
     ----------
@@ -51,15 +49,15 @@
     : Same type as input
         The hyperbolic cosine values of the input.
     """
     return _call_cpp_func(_cpp.cosh, x, out=out)
 
 
 def tanh(
-    x: VariableLikeType, *, out: Optional[VariableLikeType] = None
+    x: VariableLikeType, *, out: VariableLikeType | None = None
 ) -> VariableLikeType:
     """Element-wise hyperbolic tangent.
 
     The input unit must be dimensionless.
 
     Parameters
     ----------
@@ -73,15 +71,15 @@
     : Same type as input
         The hyperbolic tangent values of the input.
     """
     return _call_cpp_func(_cpp.tanh, x, out=out)
 
 
 def asinh(
-    x: VariableLikeType, *, out: Optional[VariableLikeType] = None
+    x: VariableLikeType, *, out: VariableLikeType | None = None
 ) -> VariableLikeType:
     """Element-wise inverse hyperbolic sine.
 
     The input unit must be dimensionless.
 
     Parameters
     ----------
@@ -95,15 +93,15 @@
     : Same type as input
         The inverse hyperbolic sine values of the input.
     """
     return _call_cpp_func(_cpp.asinh, x, out=out)
 
 
 def acosh(
-    x: VariableLikeType, *, out: Optional[VariableLikeType] = None
+    x: VariableLikeType, *, out: VariableLikeType | None = None
 ) -> VariableLikeType:
     """Element-wise inverse hyperbolic cosine.
 
     The input unit must be dimensionless.
 
     Parameters
     ----------
@@ -117,15 +115,15 @@
     : Same type as input
         The inverse hyperbolic cosine values of the input.
     """
     return _call_cpp_func(_cpp.acosh, x, out=out)
 
 
 def atanh(
-    x: VariableLikeType, *, out: Optional[VariableLikeType] = None
+    x: VariableLikeType, *, out: VariableLikeType | None = None
 ) -> VariableLikeType:
     """Element-wise inverse hyperbolic tangent.
 
     The input unit must be dimensionless.
 
     Parameters
     ----------
```

### Comparing `scipp-24.2.0/src/scipp/core/like.py` & `scipp-24.5.0/src/scipp/core/like.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/src/scipp/core/logical.py` & `scipp-24.5.0/src/scipp/core/logical.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Jan-Lukas Wynen
 from __future__ import annotations
 
 from .._scipp import core as _cpp
-from ..typing import VariableLike
+from ..typing import VariableLikeType
 from ._cpp_wrapper_util import call_func as _call_cpp_func
 
 
-def logical_not(x: VariableLike) -> VariableLike:
+def logical_not(x: VariableLikeType) -> VariableLikeType:
     """Element-wise logical negation.
 
     Equivalent to::
 
         ~a
 
     Parameters
@@ -24,15 +24,15 @@
     -------
     :
         The logical inverse of ``x``.
     """
     return _call_cpp_func(_cpp.logical_not, x)
 
 
-def logical_and(a: VariableLike, b: VariableLike) -> VariableLike:
+def logical_and(a: VariableLikeType, b: VariableLikeType) -> VariableLikeType:
     """Element-wise logical and.
 
     Equivalent to::
 
         a & b
 
     Parameters
@@ -46,15 +46,15 @@
     -------
     :
         The logical and of the elements of ``a`` and ``b``.
     """
     return _call_cpp_func(_cpp.logical_and, a, b)
 
 
-def logical_or(a: VariableLike, b: VariableLike) -> VariableLike:
+def logical_or(a: VariableLikeType, b: VariableLikeType) -> VariableLikeType:
     """Element-wise logical or.
 
     Equivalent to::
 
         a | b
 
     Parameters
@@ -68,15 +68,15 @@
     -------
     :
         The logical or of the elements of ``a`` and ``b``.
     """
     return _call_cpp_func(_cpp.logical_or, a, b)
 
 
-def logical_xor(a: VariableLike, b: VariableLike) -> VariableLike:
+def logical_xor(a: VariableLikeType, b: VariableLikeType) -> VariableLikeType:
     """Element-wise logical exclusive-or.
 
     Equivalent to::
 
         a ^ b
 
     Parameters
```

### Comparing `scipp-24.2.0/src/scipp/core/math.py` & `scipp-24.5.0/src/scipp/core/math.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
 from __future__ import annotations
 
 from numbers import Real
-from typing import Optional, Union
 
 from .._scipp import core as _cpp
 from ..typing import VariableLike
 from ._cpp_wrapper_util import call_func as _call_cpp_func
 from .variable import scalar
 
 
 def abs(
-    x: Union[VariableLike, _cpp.Unit], *, out: Optional[_cpp.Variable] = None
-) -> Union[VariableLike, _cpp.Unit]:
+    x: VariableLike | _cpp.Unit, *, out: _cpp.Variable | None = None
+) -> VariableLike | _cpp.Unit:
     """Element-wise absolute value.
 
     Parameters
     ----------
     x:
         Input data.
     out:
@@ -150,16 +149,16 @@
     :
         Scalar elements computed as the norm values of the input elements.
     """
     return _call_cpp_func(_cpp.norm, x, out=None)
 
 
 def reciprocal(
-    x: Union[VariableLike, _cpp.Unit], *, out: Optional[_cpp.Variable] = None
-) -> Union[VariableLike, _cpp.Unit]:
+    x: VariableLike | _cpp.Unit, *, out: _cpp.Variable | None = None
+) -> VariableLike | _cpp.Unit:
     """Element-wise reciprocal.
 
     Parameters
     ----------
     x:
         Input data.
     out:
@@ -175,16 +174,16 @@
     :
         The reciprocal values of the input.
     """
     return _call_cpp_func(_cpp.reciprocal, x, out=out)
 
 
 def pow(
-    base: Union[VariableLike, _cpp.Unit], exponent: Union[VariableLike, Real]
-) -> Union[VariableLike, _cpp.Unit]:
+    base: VariableLike | _cpp.Unit, exponent: VariableLike | Real
+) -> VariableLike | _cpp.Unit:
     """Element-wise power.
 
     If the base has a unit, the exponent must be scalar in order to get
     a well-defined unit in the result.
 
     Parameters
     ----------
@@ -205,16 +204,16 @@
     """
     if not isinstance(base, _cpp.Unit) and isinstance(exponent, Real):
         exponent = scalar(exponent)
     return _call_cpp_func(_cpp.pow, base, exponent)
 
 
 def sqrt(
-    x: Union[VariableLike, _cpp.Unit], *, out: Optional[_cpp.Variable] = None
-) -> Union[VariableLike, _cpp.Unit]:
+    x: VariableLike | _cpp.Unit, *, out: _cpp.Variable | None = None
+) -> VariableLike | _cpp.Unit:
     """Element-wise square-root.
 
     Parameters
     ----------
     x:
         Input data.
     out:
@@ -229,15 +228,15 @@
     -------
     :
         The square-root values of the input.
     """
     return _call_cpp_func(_cpp.sqrt, x, out=out)
 
 
-def exp(x: VariableLike, *, out: Optional[VariableLike] = None) -> VariableLike:
+def exp(x: VariableLike, *, out: VariableLike | None = None) -> VariableLike:
     """Element-wise exponential.
 
     Parameters
     ----------
     x:
         Input data.
     out:
@@ -247,15 +246,15 @@
     -------
     :
         e raised to the power of the input.
     """
     return _call_cpp_func(_cpp.exp, x, out=out)
 
 
-def log(x: VariableLike, *, out: Optional[VariableLike] = None) -> VariableLike:
+def log(x: VariableLike, *, out: VariableLike | None = None) -> VariableLike:
     """Element-wise natural logarithm.
 
     Parameters
     ----------
     x:
         Input data.
     out:
@@ -265,15 +264,15 @@
     -------
     :
         Base e logarithm of the input.
     """
     return _call_cpp_func(_cpp.log, x, out=out)
 
 
-def log10(x: VariableLike, *, out: Optional[VariableLike] = None) -> VariableLike:
+def log10(x: VariableLike, *, out: VariableLike | None = None) -> VariableLike:
     """Element-wise base 10 logarithm.
 
     Parameters
     ----------
     x:
         Input data.
     out:
@@ -283,15 +282,15 @@
     -------
     :
         Base 10 logarithm of the input.
     """
     return _call_cpp_func(_cpp.log10, x, out=out)
 
 
-def round(x: VariableLike, *, out: Optional[VariableLike] = None) -> VariableLike:
+def round(x: VariableLike, *, out: VariableLike | None = None) -> VariableLike:
     """
     Round to the nearest integer of all values passed in x.
 
     Note: if the number being rounded is halfway between two integers it will
     round to the nearest even number. For example 1.5 and 2.5 will both round
     to 2.0, -0.5 and 0.5 will both round to 0.0.
 
@@ -306,15 +305,15 @@
     -------
     :
         Rounded version of the data passed to the nearest integer.
     """
     return _call_cpp_func(_cpp.rint, x, out=out)
 
 
-def floor(x: VariableLike, *, out: Optional[VariableLike] = None) -> VariableLike:
+def floor(x: VariableLike, *, out: VariableLike | None = None) -> VariableLike:
     """
     Round down to the nearest integer of all values passed in x.
 
     Parameters
     ----------
     x:
         Input data.
@@ -325,15 +324,15 @@
     -------
     :
         Rounded down version of the data passed.
     """
     return _call_cpp_func(_cpp.floor, x, out=out)
 
 
-def ceil(x: VariableLike, *, out: Optional[VariableLike] = None) -> VariableLike:
+def ceil(x: VariableLike, *, out: VariableLike | None = None) -> VariableLike:
     """
     Round up to the nearest integer of all values passed in x.
 
     Parameters
     ----------
     x:
         Input data.
@@ -368,15 +367,15 @@
     ----------
     x:
         Input data.
     """
     return _cpp.erfc(x)
 
 
-def midpoints(x: _cpp.Variable, dim: Optional[str] = None) -> _cpp.Variable:
+def midpoints(x: _cpp.Variable, dim: str | None = None) -> _cpp.Variable:
     """
     Computes the points in the middle of adjacent elements of x.
 
     The midpoint of two numbers :math:`a` and :math:`b` is
     :math:`(a + b) / 2`.
     This formula encounters under- or overflow for
     very small or very large inputs.
```

### Comparing `scipp-24.2.0/src/scipp/core/operations.py` & `scipp-24.5.0/src/scipp/core/operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Matthew Andrew
 from __future__ import annotations
 
-from typing import Any, Dict, Literal, Optional, TypeVar, Union, overload
+from typing import Any, Literal, TypeVar, overload
 
 from .._scipp import core as _cpp
 from ..typing import ScippIndex, VariableLikeType
 from ._cpp_wrapper_util import call_func as _call_cpp_func
 from .comparison import identical
-from .cpp_classes import Dataset, DatasetError, Variable
+from .cpp_classes import DataArray, Dataset, DatasetError, Variable
 from .data_group import DataGroup
 from .unary import to_unit
 
-_ContainerWithCoords = TypeVar('_ContainerWithCoords', _cpp.DataArray, _cpp.Dataset)
+_T = TypeVar('_T', Variable, DataGroup)
+_VarDaDg = TypeVar('_VarDaDg', Variable, DataArray, DataGroup)
+_DsDg = TypeVar('_DsDg', Dataset, DataGroup)
 
 
-def islinspace(x: Variable, dim: str = None) -> Variable:
+def islinspace(x: _T, dim: str | None = None) -> _T:
     """Check if the values of a variable are evenly spaced.
 
     Parameters
     ----------
     x:
         Variable to check.
     dim:
@@ -29,22 +31,22 @@
     Returns
     -------
     :
         Variable of value True if the variable contains regularly
         spaced values, variable of value False otherwise.
     """
     if dim is None:
-        return _call_cpp_func(_cpp.islinspace, x)
+        return _call_cpp_func(_cpp.islinspace, x)  # type: ignore[return-value]
     else:
-        return _call_cpp_func(_cpp.islinspace, x, dim)
+        return _call_cpp_func(_cpp.islinspace, x, dim)  # type: ignore[return-value]
 
 
 def issorted(
-    x: Variable, dim: str, order: Literal['ascending', 'descending'] = 'ascending'
-) -> Variable:
+    x: _T, dim: str, order: Literal['ascending', 'descending'] = 'ascending'
+) -> _T:
     """Check if the values of a variable are sorted.
 
     - If ``order`` is 'ascending',
       check if values are non-decreasing along ``dim``.
     - If ``order`` is 'descending',
       check if values are non-increasing along ``dim``.
 
@@ -64,20 +66,34 @@
         variable with the corresponding boolean value for whether
         it was sorted along the given dim for the other dimensions.
 
     See Also
     --------
     scipp.allsorted
     """
-    return _call_cpp_func(_cpp.issorted, x, dim, order)
+    return _call_cpp_func(_cpp.issorted, x, dim, order)  # type: ignore[return-value]
 
 
+@overload
 def allsorted(
     x: Variable, dim: str, order: Literal['ascending', 'descending'] = 'ascending'
-) -> bool:
+) -> bool: ...
+
+
+@overload
+def allsorted(
+    x: DataGroup, dim: str, order: Literal['ascending', 'descending'] = 'ascending'
+) -> DataGroup: ...
+
+
+def allsorted(
+    x: Variable | DataGroup,
+    dim: str,
+    order: Literal['ascending', 'descending'] = 'ascending',
+) -> bool | DataGroup:
     """Check if all values of a variable are sorted.
 
     - If ``order`` is 'ascending',
       check if values are non-decreasing along ``dim``.
     - If ``order`` is 'descending',
       check if values are non-increasing along ``dim``.
 
@@ -101,15 +117,15 @@
     scipp.issorted
     """
     return _call_cpp_func(_cpp.allsorted, x, dim, order)
 
 
 def sort(
     x: VariableLikeType,
-    key: Union[str, Variable],
+    key: str | Variable,
     order: Literal['ascending', 'descending'] = 'ascending',
 ) -> VariableLikeType:
     """Sort variable along a dimension by a sort key or dimension label.
 
     - If ``order`` is 'ascending',
       sort such that values are non-decreasing according to ``key``.
     - If ``order`` is 'descending',
@@ -130,15 +146,15 @@
         The sorted equivalent of the input with the same type.
 
     Raises
     ------
     scipp.DimensionError
         If the key is a Variable that does not have exactly 1 dimension.
     """
-    return _call_cpp_func(_cpp.sort, x, key, order)
+    return _call_cpp_func(_cpp.sort, x, key, order)  # type: ignore[return-value]
 
 
 def values(x: VariableLikeType) -> VariableLikeType:
     """Return the input without variances.
 
     Parameters
     ----------
@@ -150,15 +166,15 @@
     : scipp.typing.VariableLike
         The same as the input but without variances.
 
     See Also
     --------
     scipp.variances, scipp.stddevs
     """
-    return _call_cpp_func(_cpp.values, x)
+    return _call_cpp_func(_cpp.values, x)  # type: ignore[return-value]
 
 
 def variances(x: VariableLikeType) -> VariableLikeType:
     """Return the input's variances as values.
 
     Parameters
     ----------
@@ -171,15 +187,15 @@
         The same as the input but with values set to the input's variances
         and without variances itself.
 
     See Also
     --------
     scipp.values, scipp.stddevs
     """
-    return _call_cpp_func(_cpp.variances, x)
+    return _call_cpp_func(_cpp.variances, x)  # type: ignore[return-value]
 
 
 def stddevs(x: VariableLikeType) -> VariableLikeType:
     """Return the input's standard deviations as values.
 
     Parameters
     ----------
@@ -192,15 +208,15 @@
         The same as the input but with values set to standard deviations computed
         from the input's variances and without variances itself.
 
     See Also
     --------
     scipp.values, scipp.variances
     """
-    return _call_cpp_func(_cpp.stddevs, x)
+    return _call_cpp_func(_cpp.stddevs, x)  # type: ignore[return-value]
 
 
 def where(condition: Variable, x: Variable, y: Variable) -> Variable:
     """Return elements chosen from x or y depending on condition.
 
     Parameters
     ----------
@@ -213,24 +229,24 @@
 
     Returns
     -------
     :
         Variable with elements from x where condition is True
         and elements from y elsewhere.
     """
-    return _call_cpp_func(_cpp.where, condition, x, y)
+    return _call_cpp_func(_cpp.where, condition, x, y)  # type: ignore[return-value]
 
 
 def to(
-    var: VariableLikeType,  # noqa
+    var: _VarDaDg,
     *,
-    unit: Optional[Union[_cpp.Unit, str]] = None,
-    dtype: Optional[Any] = None,
+    unit: _cpp.Unit | str | None = None,
+    dtype: Any | None = None,
     copy: bool = True,
-) -> VariableLikeType:
+) -> _VarDaDg:
     """Converts a Variable or DataArray to a different dtype and/or a different unit.
 
     If the dtype and unit are both unchanged and ``copy`` is `False`,
     the object is returned without making a deep copy.
 
     This method will choose whether to do the dtype or units translation first, by
     using the following rules in order:
@@ -295,49 +311,40 @@
 
     if convert_dtype_first:
         return to_unit(var.astype(dtype, copy=copy), unit=unit, copy=False)
     else:
         return to_unit(var, unit=unit, copy=copy).astype(dtype, copy=False)
 
 
-@overload
-def merge(lhs: Dataset, rhs: Dataset) -> Dataset:
-    ...
-
-
-@overload
-def merge(lhs: DataGroup, rhs: DataGroup) -> DataGroup:
-    ...
-
-
-def merge(lhs, rhs):
+def merge(lhs: _DsDg, rhs: _DsDg) -> _DsDg:
     """Merge two datasets or data groups into one.
 
     If an item appears in both inputs, it must have an identical value in both.
 
     Parameters
     ----------
-    lhs:
+    lhs: Dataset | DataGroup
         First dataset or data group.
-    rhs:
+    rhs: Dataset | DataGroup
         Second dataset or data group.
 
     Returns
     -------
-    :
+    : Dataset | DataGroup
         A new object that contains the union of all data items,
         coords, masks and attributes.
 
     Raises
     ------
     scipp.DatasetError
         If there are conflicting items with different content.
     """
-    if isinstance(lhs, Dataset) or isinstance(rhs, Dataset):
-        return _call_cpp_func(_cpp.merge, lhs, rhs)
+    # Check both arguments to make `_cpp.merge` raise TypeError on mismatch.
+    if isinstance(lhs, Dataset) or isinstance(rhs, Dataset):  # type: ignore[redundant-expr]
+        return _call_cpp_func(_cpp.merge, lhs, rhs)  # type: ignore[return-value]
     return _merge_data_group(lhs, rhs)
 
 
 def _generic_identical(a: Any, b: Any) -> bool:
     try:
         return identical(a, b)
     except TypeError:
@@ -355,17 +362,17 @@
         if k in res and not _generic_identical(res[k], v):
             raise DatasetError(f"Cannot merge data groups. Mismatch in item {k}")
         res[k] = v
     return res
 
 
 def label_based_index_to_positional_index(
-    sizes: Dict[str, int],
+    sizes: dict[str, int],
     coord: Variable,
-    index: Union[slice[Optional[Variable]], Variable],
+    index: slice | Variable,
 ) -> ScippIndex:
     """Returns the positional index equivalent to label based indexing
     the coord with values."""
     dim, *inds = _call_cpp_func(
         _cpp.label_based_index_to_positional_index,
         list(sizes.keys()),
         list(sizes.values()),
```

### Comparing `scipp-24.2.0/src/scipp/core/reduction.py` & `scipp-24.5.0/src/scipp/core/reduction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
 
 from __future__ import annotations
 
-from typing import Any, Callable, Optional
+from collections.abc import Callable
+from typing import Any
 
 import numpy as np
 
 from .._scipp import core as _cpp
 from ..typing import Dims, VariableLikeType
 from . import concepts
 from ._cpp_wrapper_util import call_func as _call_cpp_func
 from .data_group import DataGroup, data_group_nary
 from .variable import array
 
 
-def mean(x: VariableLikeType, dim: Optional[str] = None) -> VariableLikeType:
+def mean(x: VariableLikeType, dim: str | None = None) -> VariableLikeType:
     """Arithmetic mean of elements in the input.
 
     If the input has variances, the variances stored in the output are based on
     the "standard deviation of the mean", i.e.,
     :math:`\\sigma_{mean} = \\sigma / \\sqrt{N}`.
     :math:`N` is the length of the input dimension.
     :math:`\\sigma` is estimated as the average of the standard deviations of
@@ -52,15 +53,15 @@
     """
     if dim is None:
         return _call_cpp_func(_cpp.mean, x)
     else:
         return _call_cpp_func(_cpp.mean, x, dim=dim)
 
 
-def nanmean(x: VariableLikeType, dim: Optional[str] = None) -> VariableLikeType:
+def nanmean(x: VariableLikeType, dim: str | None = None) -> VariableLikeType:
     """Arithmetic mean of elements in the input ignoring NaN's.
 
     If the input has variances, the variances stored in the output are based on
     the "standard deviation of the mean", i.e.,
     :math:`\\sigma_{mean} = \\sigma / \\sqrt{N}`.
     :math:`N` is the length of the input dimension.
     :math:`\\sigma` is estimated as the average of the standard deviations of
@@ -633,15 +634,15 @@
     elif isinstance(dim, str):
         return _call_cpp_func(_cpp.sum, x, dim=dim)
     for d in dim:
         x = _call_cpp_func(_cpp.sum, x, d)
     return x
 
 
-def nansum(x: VariableLikeType, dim: Optional[str] = None) -> VariableLikeType:
+def nansum(x: VariableLikeType, dim: str | None = None) -> VariableLikeType:
     """Sum of elements in the input ignoring NaN's.
 
     See :py:func:`scipp.sum` on how rounding errors for float32 inputs are handled.
 
     Parameters
     ----------
     x: scipp.typing.VariableLike
@@ -662,15 +663,15 @@
     """
     if dim is None:
         return _call_cpp_func(_cpp.nansum, x)
     else:
         return _call_cpp_func(_cpp.nansum, x, dim=dim)
 
 
-def min(x: VariableLikeType, dim: Optional[str] = None) -> VariableLikeType:
+def min(x: VariableLikeType, dim: str | None = None) -> VariableLikeType:
     """Minimum of elements in the input.
 
     Warning
     -------
 
     Scipp returns DBL_MAX or INT_MAX for empty inputs of float or int dtype,
     respectively, while NumPy raises. Note that in the case of :py:class:`DataArray`,
@@ -701,15 +702,15 @@
     """
     if dim is None:
         return _call_cpp_func(_cpp.min, x)
     else:
         return _call_cpp_func(_cpp.min, x, dim=dim)
 
 
-def max(x: VariableLikeType, dim: Optional[str] = None) -> VariableLikeType:
+def max(x: VariableLikeType, dim: str | None = None) -> VariableLikeType:
     """Maximum of elements in the input.
 
     Warning
     -------
 
     Scipp returns DBL_MIN or INT_MIN for empty inputs of float or int dtype,
     respectively, while NumPy raises. Note that in the case of :py:class:`DataArray`,
@@ -740,15 +741,15 @@
     """
     if dim is None:
         return _call_cpp_func(_cpp.max, x)
     else:
         return _call_cpp_func(_cpp.max, x, dim=dim)
 
 
-def nanmin(x: VariableLikeType, dim: Optional[str] = None) -> VariableLikeType:
+def nanmin(x: VariableLikeType, dim: str | None = None) -> VariableLikeType:
     """Minimum of elements in the input ignoring NaN's.
 
     Warning
     -------
 
     Scipp returns DBL_MAX or INT_MAX for empty inputs of float or int dtype,
     respectively, while NumPy raises. Note that in the case of :py:class:`DataArray`,
@@ -779,15 +780,15 @@
     """
     if dim is None:
         return _call_cpp_func(_cpp.nanmin, x)
     else:
         return _call_cpp_func(_cpp.nanmin, x, dim=dim)
 
 
-def nanmax(x: VariableLikeType, dim: Optional[str] = None) -> VariableLikeType:
+def nanmax(x: VariableLikeType, dim: str | None = None) -> VariableLikeType:
     """Maximum of elements in the input ignoring NaN's.
 
     Warning
     -------
 
     Scipp returns DBL_MIN or INT_MIN for empty inputs of float or int dtype,
     respectively, while NumPy raises. Note that in the case of :py:class:`DataArray`,
@@ -818,15 +819,15 @@
     """
     if dim is None:
         return _call_cpp_func(_cpp.nanmax, x)
     else:
         return _call_cpp_func(_cpp.nanmax, x, dim=dim)
 
 
-def all(x: VariableLikeType, dim: Optional[str] = None) -> VariableLikeType:
+def all(x: VariableLikeType, dim: str | None = None) -> VariableLikeType:
     """Logical AND over input values.
 
     Parameters
     ----------
     x: scipp.typing.VariableLike
         Input data.
     dim:
@@ -846,15 +847,15 @@
     """
     if dim is None:
         return _call_cpp_func(_cpp.all, x)
     else:
         return _call_cpp_func(_cpp.all, x, dim=dim)
 
 
-def any(x: VariableLikeType, dim: Optional[str] = None) -> VariableLikeType:
+def any(x: VariableLikeType, dim: str | None = None) -> VariableLikeType:
     """Logical OR over input values.
 
     Parameters
     ----------
     x: scipp.typing.VariableLike
         Input data.
     dim:
```

### Comparing `scipp-24.2.0/src/scipp/core/shape.py` & `scipp-24.5.0/src/scipp/core/shape.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Matthew Andrew
-# flake8: noqa: E501
+# ruff: noqa: E501
 
-from typing import Dict, List, Optional, Sequence, Tuple, Union
+from collections.abc import Sequence
 
 import numpy as np
 
 from .._scipp import core as _cpp
 from ..typing import VariableLikeType
 from . import data_group
 from ._cpp_wrapper_util import call_func as _call_cpp_func
 from ._sizes import _parse_dims_shape_sizes
 from .concepts import transform_data
 
 
 def broadcast(
     x: VariableLikeType,
-    dims: Optional[Union[List[str], Tuple[str, ...]]] = None,
-    shape: Optional[Sequence[int]] = None,
-    sizes: Optional[Dict[str, int]] = None,
+    dims: list[str] | tuple[str, ...] | None = None,
+    shape: Sequence[int] | None = None,
+    sizes: dict[str, int] | None = None,
 ) -> VariableLikeType:
     """Broadcast a Variable or a DataArray.
 
     If the input is a DataArray, coordinates and attributes are shallow-copied
     and masks are deep-copied.
 
     Note that Scipp operations broadcast automatically, so using this function
@@ -120,17 +120,17 @@
         return data_group._apply_to_items(concat, x, dim)
     return _call_cpp_func(_cpp.concat, x, dim)
 
 
 def fold(
     x: VariableLikeType,
     dim: str,
-    sizes: Optional[Dict[str, int]] = None,
-    dims: Optional[Union[List[str], Tuple[str, ...]]] = None,
-    shape: Optional[Sequence[int]] = None,
+    sizes: dict[str, int] | None = None,
+    dims: list[str] | tuple[str, ...] | None = None,
+    shape: Sequence[int] | None = None,
 ) -> VariableLikeType:
     """Fold a single dimension of a variable or data array into multiple dims.
 
     One and only one of these sets of arguments must be given:
 
     - ``dims`` and ``shape``
     - ``sizes``
@@ -206,28 +206,26 @@
     if minus_one_count == 1:
         ind = new_shape.index(-1)
         new_shape[ind] = 1
         new_volume = np.prod(new_shape)
         dim_size = x.sizes[dim] // new_volume
         if x.sizes[dim] % new_volume != 0:
             raise ValueError(
-                "-1 in new shape was computed to be {}, but the original "
-                "shape {} cannot be divided by {}.".format(
-                    dim_size, x.sizes[dim], dim_size
-                )
+                f"-1 in new shape was computed to be {dim_size}, but the original "
+                f"shape {x.sizes[dim]} cannot be divided by {dim_size}."
             )
         new_shape[ind] = dim_size
 
     return _call_cpp_func(_cpp.fold, x, dim, sizes["dims"], new_shape)
 
 
 def flatten(
     x: VariableLikeType,
-    dims: Optional[Union[List[str], Tuple[str, ...]]] = None,
-    to: Optional[str] = None,
+    dims: list[str] | tuple[str, ...] | None = None,
+    to: str | None = None,
 ) -> VariableLikeType:
     """Flatten multiple dimensions into a single dimension.
 
     If the input has a bin-edge coordinate that cannot be joined together it will not
     be included in the output.
 
     If the input is a DataArray then coords, masks, and attrs that contain at least one
@@ -311,15 +309,15 @@
         # makes more sense for the dims that we want to flatten to come first
         # in the argument list.
         raise ValueError("The final flattened dimension is required.")
     return _call_cpp_func(_cpp.flatten, x, dims, to)
 
 
 def transpose(
-    x: VariableLikeType, dims: Optional[Union[List[str], Tuple[str, ...]]] = None
+    x: VariableLikeType, dims: list[str] | tuple[str, ...] | None = None
 ) -> VariableLikeType:
     """Transpose dimensions of the input.
 
     Parameters
     ----------
     x: scipp.typing.VariableLike
         Object to transpose.
@@ -337,15 +335,15 @@
     scipp.DimensionError
         If ``dims`` are incompatible with the input data.
     """
     return _call_cpp_func(_cpp.transpose, x, dims if dims is not None else [])
 
 
 def squeeze(
-    x: VariableLikeType, dim: Optional[Union[str, List[str], Tuple[str, ...]]] = None
+    x: VariableLikeType, dim: str | list[str] | tuple[str, ...] | None = None
 ) -> VariableLikeType:
     """Remove dimensions of length 1.
 
     This is equivalent to indexing the squeezed dimensions with index 0, that is
     ``squeeze(x, ['x', 'y'])`` is equivalent to ``x['x', 0]['y', 0]``.
 
     Parameters
```

### Comparing `scipp-24.2.0/src/scipp/core/trigonometry.py` & `scipp-24.5.0/src/scipp/core/trigonometry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
 
 from __future__ import annotations
 
-from typing import Optional
-
 from .._scipp import core as _cpp
 from ..typing import VariableLikeType
 from ._cpp_wrapper_util import call_func as _call_cpp_func
 
 
 def sin(
-    x: VariableLikeType, *, out: Optional[VariableLikeType] = None
+    x: VariableLikeType, *, out: VariableLikeType | None = None
 ) -> VariableLikeType:
     """Element-wise sine.
 
     The input must have a plane-angle unit, i.e. ``rad``, ``deg``.
 
     Parameters
     ----------
@@ -30,15 +28,15 @@
     : Same type as input
         The sine values of the input.
     """
     return _call_cpp_func(_cpp.sin, x, out=out)
 
 
 def cos(
-    x: VariableLikeType, *, out: Optional[VariableLikeType] = None
+    x: VariableLikeType, *, out: VariableLikeType | None = None
 ) -> VariableLikeType:
     """Element-wise cosine.
 
     The input must have a plane-angle unit, i.e. ``rad``, ``deg``.
 
     Parameters
     ----------
@@ -52,15 +50,15 @@
     : Same type as input
         The cosine values of the input.
     """
     return _call_cpp_func(_cpp.cos, x, out=out)
 
 
 def tan(
-    x: VariableLikeType, *, out: Optional[VariableLikeType] = None
+    x: VariableLikeType, *, out: VariableLikeType | None = None
 ) -> VariableLikeType:
     """Element-wise tangent.
 
     The input must have a plane-angle unit, i.e. ``rad``, ``deg``.
 
     Parameters
     ----------
@@ -74,15 +72,15 @@
     : Same type as input
         The tangent values of the input.
     """
     return _call_cpp_func(_cpp.tan, x, out=out)
 
 
 def asin(
-    x: VariableLikeType, *, out: Optional[VariableLikeType] = None
+    x: VariableLikeType, *, out: VariableLikeType | None = None
 ) -> VariableLikeType:
     """Element-wise inverse sine.
 
     Parameters
     ----------
     x: scipp.typing.VariableLike
         Input data.
@@ -94,15 +92,15 @@
     : Same type as input
         The inverse sine values of the input in radians.
     """
     return _call_cpp_func(_cpp.asin, x, out=out)
 
 
 def acos(
-    x: VariableLikeType, *, out: Optional[VariableLikeType] = None
+    x: VariableLikeType, *, out: VariableLikeType | None = None
 ) -> VariableLikeType:
     """Element-wise inverse cosine.
 
     Parameters
     ----------
     x: scipp.typing.VariableLike
         Input data.
@@ -114,15 +112,15 @@
     : Same type as input
         The inverse cosine values of the input in radians.
     """
     return _call_cpp_func(_cpp.acos, x, out=out)
 
 
 def atan(
-    x: VariableLikeType, *, out: Optional[VariableLikeType] = None
+    x: VariableLikeType, *, out: VariableLikeType | None = None
 ) -> VariableLikeType:
     """Element-wise inverse tangent.
 
     Parameters
     ----------
     x: scipp.typing.VariableLike
         Input data.
@@ -134,15 +132,15 @@
     : Same type as input
         The inverse tangent values of the input in radians.
     """
     return _call_cpp_func(_cpp.atan, x, out=out)
 
 
 def atan2(
-    *, y: _cpp.Variable, x: _cpp.Variable, out: Optional[_cpp.Variable] = None
+    *, y: _cpp.Variable, x: _cpp.Variable, out: _cpp.Variable | None = None
 ) -> _cpp.Variable:
     """Element-wise inverse tangent of y/x determining the correct quadrant.
 
     Parameters
     ----------
     y:
         Input y values.
```

### Comparing `scipp-24.2.0/src/scipp/core/unary.py` & `scipp-24.5.0/src/scipp/core/unary.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Matthew Andrew
-from typing import Union as _Union
 
 from .._scipp import core as _cpp
+from ..typing import VariableLikeType
 from ._cpp_wrapper_util import call_func as _call_cpp_func
 
 
-def isnan(x: _cpp.Variable) -> _cpp.Variable:
+def isnan(x: VariableLikeType) -> VariableLikeType:
     """Element-wise isnan (true if an element is nan)."""
-    return _call_cpp_func(_cpp.isnan, x)
+    return _call_cpp_func(_cpp.isnan, x)  # type: ignore[return-value]
 
 
-def isinf(x: _cpp.Variable) -> _cpp.Variable:
+def isinf(x: VariableLikeType) -> VariableLikeType:
     """Element-wise isinf (true if an element is inf)."""
-    return _call_cpp_func(_cpp.isinf, x)
+    return _call_cpp_func(_cpp.isinf, x)  # type: ignore[return-value]
 
 
-def isfinite(x: _cpp.Variable) -> _cpp.Variable:
+def isfinite(x: VariableLikeType) -> VariableLikeType:
     """Element-wise isfinite (true if an element is finite)."""
-    return _call_cpp_func(_cpp.isfinite, x)
+    return _call_cpp_func(_cpp.isfinite, x)  # type: ignore[return-value]
 
 
-def isposinf(x: _cpp.Variable) -> _cpp.Variable:
+def isposinf(x: VariableLikeType) -> VariableLikeType:
     """Element-wise isposinf (true if an element is a positive infinity)."""
-    return _call_cpp_func(_cpp.isposinf, x)
+    return _call_cpp_func(_cpp.isposinf, x)  # type: ignore[return-value]
 
 
-def isneginf(x: _cpp.Variable) -> _cpp.Variable:
+def isneginf(x: VariableLikeType) -> VariableLikeType:
     """Element-wise isneginf (true if an element is a negative infinity)."""
-    return _call_cpp_func(_cpp.isneginf, x)
+    return _call_cpp_func(_cpp.isneginf, x)  # type: ignore[return-value]
 
 
 def to_unit(
-    x: _cpp.Variable, unit: _Union[_cpp.Unit, str], *, copy: bool = True
-) -> _cpp.Variable:
+    x: VariableLikeType, unit: _cpp.Unit | str, *, copy: bool = True
+) -> VariableLikeType:
     """Convert the variable to a different unit.
 
     Raises a :class:`scipp.UnitError` if the input unit is not compatible
     with the provided unit, e.g., `m` cannot be converted to `s`.
 
     If the input dtype is an integer type or datetime64, the output is rounded
     and returned with the same dtype as the input.
 
     Parameters
     ----------
-    x:
+    x: VariableLike
         Input variable.
     unit:
         Desired target unit.
     copy:
         If `False`, return the input object if possible, i.e.
         if the unit is unchanged.
         If `True`, the function always returns a new object.
@@ -62,8 +62,8 @@
     Examples
     --------
 
       >>> var = 1.2 * sc.Unit('m')
       >>> sc.to_unit(var, unit='mm')
       <scipp.Variable> ()    float64             [mm]  1200
     """
-    return _call_cpp_func(_cpp.to_unit, x=x, unit=unit, copy=copy)
+    return _call_cpp_func(_cpp.to_unit, x=x, unit=unit, copy=copy)  # type: ignore[return-value]
```

### Comparing `scipp-24.2.0/src/scipp/core/util.py` & `scipp-24.5.0/src/scipp/core/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
-from typing import Dict
 
 from ..typing import VariableLikeType
 from .cpp_classes import DataArray, Dataset, Variable
 from .like import empty_like
 
 
-def _copy_dict_for_overwrite(mapping: Dict[str, Variable]) -> Dict[str, Variable]:
+def _copy_dict_for_overwrite(mapping: dict[str, Variable]) -> dict[str, Variable]:
     return {name: copy_for_overwrite(var) for name, var in mapping.items()}
 
 
 def copy_for_overwrite(obj: VariableLikeType) -> VariableLikeType:
     """
     Copy a Scipp object for overwriting.
```

### Comparing `scipp-24.2.0/src/scipp/core/variable.py` & `scipp-24.5.0/src/scipp/core/variable.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Matthew Andrew
-# flake8: noqa: E501
+# ruff: noqa: E501
 
 from __future__ import annotations
 
 import warnings
+from collections.abc import Iterable, Sequence
 from contextlib import contextmanager
-from typing import Any, Iterable, Optional, Sequence, TypeVar, Union
+from typing import Any, Generator, TypeVar
 
 import numpy as _np
 from numpy.typing import ArrayLike
 
 from .._scipp import core as _cpp
 from ..typing import DTypeLike
-from ..units import default_unit
+from ..units import DefaultUnit, default_unit
 from ._sizes import _parse_dims_shape_sizes
 from .cpp_classes import DType, Unit, Variable
 
-NumberOrVar = TypeVar('NumberOrVar', Union[int, float], Variable)
+NumberOrVar = TypeVar('NumberOrVar', int, float, Variable)
 
 
 def scalar(
     value: Any,
     *,
     variance: Any = None,
-    unit: Union[Unit, str, None] = default_unit,
-    dtype: Optional[DTypeLike] = None,
+    unit: Unit | str | DefaultUnit | None = default_unit,
+    dtype: DTypeLike | None = None,
 ) -> Variable:
     """Constructs a zero dimensional :class:`Variable` with a unit and optional
     variance.
 
     Parameters
     ----------
     value:
@@ -71,20 +72,20 @@
 
     Calling ``scalar`` with a list (or similar array-like object) will store that
     object in a scalar variable and *not* create an array variable:
 
       >>> sc.scalar([1, 2, 3])
       <scipp.Variable> ()   PyObject           <no unit>  [1, 2, 3]
     """
-    return _cpp.Variable(
+    return _cpp.Variable(  # type: ignore[no-any-return]
         dims=(), values=value, variances=variance, unit=unit, dtype=dtype
     )
 
 
-def index(value: Any, *, dtype: Optional[DTypeLike] = None) -> Variable:
+def index(value: Any, *, dtype: DTypeLike | None = None) -> Variable:
     """Constructs a zero dimensional :class:`Variable` representing an index.
 
     This is equivalent to calling :py:func:`scipp.scalar` with unit=None.
 
     Parameters
     ----------
     value:
@@ -109,18 +110,18 @@
       <scipp.Variable> ()      int64           <no unit>  123
     """
     return scalar(value=value, dtype=dtype, unit=None)
 
 
 def zeros(
     *,
-    dims: Sequence[str] = None,
-    shape: Sequence[int] = None,
-    sizes: dict = None,
-    unit: Union[Unit, str, None] = default_unit,
+    dims: Sequence[str] | None = None,
+    shape: Sequence[int] | None = None,
+    sizes: dict[str, int] | None = None,
+    unit: Unit | str | DefaultUnit | None = default_unit,
     dtype: DTypeLike = DType.float64,
     with_variances: bool = False,
 ) -> Variable:
     """Constructs a :class:`Variable` with default initialized values with
     given dimension labels and shape.
 
     The dims and shape can also be specified using a `sizes` dict.
@@ -163,28 +164,28 @@
       >>> sc.zeros(sizes={'y': 3}, with_variances=True)
       <scipp.Variable> (y: 3)    float64  [dimensionless]  [0, 0, 0]  [0, 0, 0]
 
       >>> sc.zeros(sizes={'z': 3}, unit='kg', dtype=int)
       <scipp.Variable> (z: 3)      int64             [kg]  [0, 0, 0]
     """
 
-    return _cpp.zeros(
+    return _cpp.zeros(  # type: ignore[no-any-return]
         **_parse_dims_shape_sizes(dims, shape, sizes),
         unit=unit,
         dtype=dtype,
         with_variances=with_variances,
     )
 
 
 def ones(
     *,
-    dims: Sequence[str] = None,
-    shape: Sequence[int] = None,
-    sizes: dict = None,
-    unit: Union[Unit, str, None] = default_unit,
+    dims: Sequence[str] | None = None,
+    shape: Sequence[int] | None = None,
+    sizes: dict[str, int] | None = None,
+    unit: Unit | str | DefaultUnit | None = default_unit,
     dtype: DTypeLike = DType.float64,
     with_variances: bool = False,
 ) -> Variable:
     """Constructs a :class:`Variable` with values initialized to 1 with
     given dimension labels and shape.
 
     The dims and shape can also be specified using a `sizes` dict.
@@ -224,28 +225,28 @@
 
       >>> sc.ones(sizes={'y': 3}, with_variances=True)
       <scipp.Variable> (y: 3)    float64  [dimensionless]  [1, 1, 1]  [1, 1, 1]
 
       >>> sc.ones(sizes={'z': 3}, unit='kg', dtype=int)
       <scipp.Variable> (z: 3)      int64             [kg]  [1, 1, 1]
     """
-    return _cpp.ones(
+    return _cpp.ones(  # type: ignore[no-any-return]
         **_parse_dims_shape_sizes(dims, shape, sizes),
         unit=unit,
         dtype=dtype,
         with_variances=with_variances,
     )
 
 
 def empty(
     *,
-    dims: Sequence[str] = None,
-    shape: Sequence[int] = None,
-    sizes: dict = None,
-    unit: Union[Unit, str, None] = default_unit,
+    dims: Sequence[str] | None = None,
+    shape: Sequence[int] | None = None,
+    sizes: dict[str, int] | None = None,
+    unit: Unit | str | DefaultUnit | None = default_unit,
     dtype: DTypeLike = DType.float64,
     with_variances: bool = False,
     aligned: bool = True,
 ) -> Variable:
     """Constructs a :class:`Variable` with uninitialized values with given
     dimension labels and shape.
 
@@ -288,32 +289,32 @@
     --------
 
       >>> var = sc.empty(dims=['x'], shape=[4])
       >>> var[:] = sc.scalar(2.0)  # initialize values before printing
       >>> var
       <scipp.Variable> (x: 4)    float64  [dimensionless]  [2, 2, 2, 2]
     """
-    return _cpp.empty(
+    return _cpp.empty(  # type: ignore[no-any-return]
         **_parse_dims_shape_sizes(dims, shape, sizes),
         unit=unit,
         dtype=dtype,
         with_variances=with_variances,
         aligned=aligned,
     )
 
 
 def full(
     *,
     value: Any,
     variance: Any = None,
-    dims: Sequence[str] = None,
-    shape: Sequence[int] = None,
-    sizes: dict = None,
-    unit: Union[Unit, str, None] = default_unit,
-    dtype: Optional[DTypeLike] = None,
+    dims: Sequence[str] | None = None,
+    shape: Sequence[int] | None = None,
+    sizes: dict[str, int] | None = None,
+    unit: Unit | str | DefaultUnit | None = default_unit,
+    dtype: DTypeLike | None = None,
 ) -> Variable:
     """Constructs a :class:`Variable` with values initialized to the specified
     value with given dimension labels and shape.
 
     The dims and shape can also be specified using a `sizes` dict.
 
     Parameters
@@ -361,15 +362,15 @@
         scalar(value=value, variance=variance, unit=unit, dtype=dtype)
         .broadcast(**_parse_dims_shape_sizes(dims, shape, sizes))
         .copy()
     )
 
 
 def vector(
-    value: Union[_np.ndarray, list], *, unit: Union[Unit, str, None] = default_unit
+    value: ArrayLike, *, unit: Unit | str | DefaultUnit | None = default_unit
 ) -> Variable:
     """Constructs a zero dimensional :class:`Variable` holding a single length-3
     vector.
 
     Parameters
     ----------
     value:
@@ -400,16 +401,16 @@
     """
     return vectors(dims=(), values=value, unit=unit)
 
 
 def vectors(
     *,
     dims: Sequence[str],
-    values: Union[_np.ndarray, list],
-    unit: Union[Unit, str, None] = default_unit,
+    values: ArrayLike,
+    unit: Unit | str | DefaultUnit | None = default_unit,
 ) -> Variable:
     """Constructs a :class:`Variable` with given dimensions holding an array
     of length-3 vectors.
 
     Parameters
     ----------
     dims:
@@ -443,24 +444,26 @@
       >>> var.values
       array([[1., 2., 3.],
              [4., 5., 6.]])
 
       >>> sc.vectors(dims=['x'], values=[[1, 2, 3], [4, 5, 6]], unit='mm')
       <scipp.Variable> (x: 2)    vector3             [mm]  [(1, 2, 3), (4, 5, 6)]
     """
-    return _cpp.Variable(dims=dims, values=values, unit=unit, dtype=DType.vector3)
+    return _cpp.Variable(  # type: ignore[no-any-return]
+        dims=dims, values=values, unit=unit, dtype=DType.vector3
+    )
 
 
 def array(
     *,
     dims: Iterable[str],
     values: ArrayLike,
-    variances: Optional[ArrayLike] = None,
-    unit: Union[Unit, str, None] = default_unit,
-    dtype: Optional[DTypeLike] = None,
+    variances: ArrayLike | None = None,
+    unit: Unit | str | DefaultUnit | None = default_unit,
+    dtype: DTypeLike | None = None,
 ) -> Variable:
     """Constructs a :class:`Variable` with given dimensions, containing given
     values and optional variances.
 
     Dimension and value shape must match.
     Only keyword arguments accepted.
 
@@ -513,33 +516,35 @@
       <scipp.Variable> (x: 3)      int64              [m]  [1, 2, 3]
 
     Setting variances:
 
       >>> sc.array(dims=['x'], values=[1.0, 2.0, 3.0], variances=[0.1, 0.2, 0.3])
       <scipp.Variable> (x: 3)    float64  [dimensionless]  [1, 2, 3]  [0.1, 0.2, 0.3]
     """
-    return _cpp.Variable(
+    return _cpp.Variable(  # type: ignore[no-any-return]
         dims=dims, values=values, variances=variances, unit=unit, dtype=dtype
     )
 
 
-def _expect_no_variances(args):
+def _expect_no_variances(args: dict[str, Variable | None]) -> None:
     has_variances = [
         key
         for key, val in args.items()
         if val is not None and val.variances is not None
     ]
     if has_variances:
         raise _cpp.VariancesError(
             'Arguments cannot have variances. ' f'Passed variances in {has_variances}'
         )
 
 
 # Assumes that all arguments are Variable or None.
-def _ensure_same_unit(*, unit, args: dict):
+def _ensure_same_unit(
+    *, unit: Unit | str | DefaultUnit | None, args: dict[str, Variable | None]
+) -> tuple[dict[str, Variable | None], Unit | str | DefaultUnit | None]:
     if unit == default_unit:
         units = {key: val.unit for key, val in args.items() if val is not None}
         if len(set(units.values())) != 1:
             raise _cpp.UnitError(
                 f'All units of the following arguments must be equal: {units}. '
                 'You can specify a unit explicitly with the `unit` argument.'
             )
@@ -547,15 +552,17 @@
     return {
         key: _cpp.to_unit(val, unit, copy=False).value if val is not None else None
         for key, val in args.items()
     }, unit
 
 
 # Process arguments of arange, linspace, etc and return them as plain numbers or None.
-def _normalize_range_args(*, unit, **kwargs):
+def _normalize_range_args(
+    *, unit: Unit | str | DefaultUnit | None, **kwargs: Any
+) -> tuple[dict[str, Any], Unit | str | DefaultUnit | None]:
     is_var = {
         key: isinstance(val, _cpp.Variable)
         for key, val in kwargs.items()
         if val is not None
     }
     if any(is_var.values()):
         if not all(is_var.values()):
@@ -572,16 +579,16 @@
 def linspace(
     dim: str,
     start: NumberOrVar,
     stop: NumberOrVar,
     num: int,
     *,
     endpoint: bool = True,
-    unit: Union[Unit, str, None] = default_unit,
-    dtype: Optional[DTypeLike] = None,
+    unit: Unit | str | DefaultUnit | None = default_unit,
+    dtype: DTypeLike | None = None,
 ) -> Variable:
     """Constructs a :class:`Variable` with `num` evenly spaced samples,
     calculated over the interval `[start, stop]`.
 
     Parameters
     ----------
     dim:
@@ -632,16 +639,16 @@
 def geomspace(
     dim: str,
     start: NumberOrVar,
     stop: NumberOrVar,
     num: int,
     *,
     endpoint: bool = True,
-    unit: Union[Unit, str, None] = default_unit,
-    dtype: Optional[DTypeLike] = None,
+    unit: Unit | str | DefaultUnit | None = default_unit,
+    dtype: DTypeLike | None = None,
 ) -> Variable:
     """Constructs a :class:`Variable` with values spaced evenly on a log scale
     (a geometric progression).
 
     This is similar to :py:func:`scipp.logspace`, but with endpoints specified
     directly instead of as exponents.
     Each output sample is a constant multiple of the previous.
@@ -696,17 +703,17 @@
 def logspace(
     dim: str,
     start: NumberOrVar,
     stop: NumberOrVar,
     num: int,
     *,
     endpoint: bool = True,
-    base: Union[int, float] = 10.0,
-    unit: Union[Unit, str, None] = default_unit,
-    dtype: Optional[DTypeLike] = None,
+    base: float = 10.0,
+    unit: Unit | str | DefaultUnit | None = default_unit,
+    dtype: DTypeLike | None = None,
 ) -> Variable:
     """Constructs a :class:`Variable` with values spaced evenly on a log scale.
 
     This is similar to :py:func:`scipp.geomspace`, but with endpoints specified
     as exponents.
 
     Parameters
@@ -764,20 +771,20 @@
         unit=unit,
         dtype=dtype,
     )
 
 
 def arange(
     dim: str,
-    start: Union[NumberOrVar, _np.datetime64, str],
-    stop: Optional[Union[NumberOrVar, _np.datetime64, str]] = None,
-    step: Optional[NumberOrVar] = None,
+    start: NumberOrVar | _np.datetime64 | str,
+    stop: NumberOrVar | _np.datetime64 | str | None = None,
+    step: NumberOrVar | None = None,
     *,
-    unit: Union[Unit, str, None] = default_unit,
-    dtype: Optional[DTypeLike] = None,
+    unit: Unit | str | DefaultUnit | None = default_unit,
+    dtype: DTypeLike | None = None,
 ) -> Variable:
     """Creates a :class:`Variable` with evenly spaced values within a given interval.
 
     Values are generated within the half-open interval [start, stop).
     In other words, the interval including start but excluding stop.
 
     ``start``, ``stop``, and ``step`` may be given as plain values or as 0-D variables.
@@ -838,58 +845,62 @@
       >>> sc.arange('t', '2000-01-01T01:00:00', '2000-01-01T01:01:30', 30 * sc.Unit('s'), dtype='datetime64')
       <scipp.Variable> (t: 3)  datetime64              [s]  [2000-01-01T01:00:00, 2000-01-01T01:00:30, 2000-01-01T01:01:00]
 
     Note that in this case the datetime ``start`` and ``stop`` strings implicitly
     define the unit. The ``step`` must have the same unit.
     """
     if dtype == 'datetime64' and isinstance(start, str):
-        start = datetime(start)
-        stop = stop if stop is None else datetime(stop)
+        start = datetime(start)  # type: ignore[assignment]
+        if not isinstance(stop, str) and stop is not None:
+            raise TypeError(
+                'Argument `stop` must be a string or `None` if `start` is a string.'
+            )
+        stop = stop if stop is None else datetime(stop)  # type: ignore[assignment]
     range_args, unit = _normalize_range_args(
         unit=unit, start=start, stop=stop, step=step
     )
-    args = [x for x in [start, stop, step] if x is not None]
     types = [
         x.values.dtype if isinstance(x, _cpp.Variable) else _np.asarray(x).dtype
-        for x in args
+        for x in (start, stop, step)
+        if x is not None
     ]
     if dtype is None:
         candidates = set(types)
         if len(candidates) == 1:
             dtype = next(iter(candidates))
-    if dtype is not None and dtype != str('datetime64'):
+    if dtype is not None and dtype != 'datetime64':
         numpy_dtype = str(dtype) if isinstance(dtype, DType) else dtype
     else:
         numpy_dtype = None
     return array(
         dims=[dim],
         values=_np.arange(**range_args, dtype=numpy_dtype),
         unit=unit,
         dtype=dtype,
     )
 
 
 @contextmanager
-def _timezone_warning_as_error():
+def _timezone_warning_as_error() -> Generator[None, None, None]:
     with warnings.catch_warnings():
         warnings.filterwarnings(
             'error', category=DeprecationWarning, message='parsing timezone'
         )
         try:
             yield
         except DeprecationWarning:
             raise ValueError(
                 'Parsing timezone aware datetimes is not supported'
             ) from None
 
 
 def datetime(
-    value: Union[str, int, _np.datetime64],
+    value: str | int | _np.datetime64,
     *,
-    unit: Optional[Union[Unit, str, None]] = default_unit,
+    unit: Unit | str | DefaultUnit | None = default_unit,
 ) -> Variable:
     """Constructs a zero dimensional :class:`Variable` with a dtype of datetime64.
 
     Parameters
     ----------
     value:
 
@@ -931,15 +942,18 @@
     if isinstance(value, str):
         with _timezone_warning_as_error():
             return scalar(_np.datetime64(value), unit=unit)
     return scalar(value, unit=unit, dtype=_cpp.DType.datetime64)
 
 
 def datetimes(
-    *, dims, values: ArrayLike, unit: Optional[Union[Unit, str, None]] = default_unit
+    *,
+    dims: Sequence[str],
+    values: ArrayLike,
+    unit: Unit | str | DefaultUnit | None = default_unit,
 ) -> Variable:
     """Constructs an array :class:`Variable` with a dtype of datetime64.
 
     Parameters
     ----------
     dims:
         Dimension labels
@@ -977,15 +991,15 @@
     np_unit_str = f'[{u}]' if (u := _cpp.to_numpy_time_string(unit)) else ''
     with _timezone_warning_as_error():
         return array(
             dims=dims, values=_np.asarray(values, dtype=f'datetime64{np_unit_str}')
         )
 
 
-def epoch(*, unit: Union[Unit, str]) -> Variable:
+def epoch(*, unit: Unit | str | DefaultUnit | None) -> Variable:
     """Constructs a zero dimensional :class:`Variable` with a dtype of
     datetime64 that contains Scipp's epoch.
 
     Currently, the epoch of datetimes in Scipp is the Unix epoch 1970-01-01T00:00:00.
 
     Parameters
     ----------
```

### Comparing `scipp-24.2.0/src/scipp/curve_fit.py` & `scipp-24.5.0/src/scipp/curve_fit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
+from collections.abc import Callable, Mapping, Sequence
 from inspect import getfullargspec
 from numbers import Real
-from typing import Callable, Dict, Mapping, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
-from .core import BinEdgeError, DataArray, DataGroup, Variable, array, scalar, stddevs
+from .core import (
+    BinEdgeError,
+    DataArray,
+    DataGroup,
+    Variable,
+    array,
+    irreducible_mask,
+    scalar,
+    stddevs,
+)
 from .units import default_unit, dimensionless
 
 
 def _as_scalar(obj, unit):
     if unit == default_unit:
         return obj
     return scalar(value=obj, unit=unit)
 
 
 def _wrap_scipp_func(f, p_names, p_units):
-    _params = {k: _as_scalar(0.0, u) for k, u in zip(p_names, p_units)}
+    _params = {k: _as_scalar(0.0, u) for k, u in zip(p_names, p_units, strict=True)}
 
     def func(x, *args):
-        for k, v in zip(p_names, args):
+        for k, v in zip(p_names, args, strict=True):
             if isinstance(_params[k], Variable):
                 _params[k].value = v
             else:
                 _params[k] = v
         return f(**x, **_params).values
 
     return func
@@ -33,16 +42,16 @@
 
 def _wrap_numpy_func(f, p_names, coord_names):
     def func(x, *args):
         # If there is only one predictor variable x might be a 1D array.
         # Make x 2D for consistency.
         if len(x.shape) == 1:
             x = x.reshape(1, -1)
-        coords = {c: arr for c, arr in zip(coord_names, x)}
-        params = {k: v for k, v in zip(p_names, args)}
+        coords = dict(zip(coord_names, x, strict=True))
+        params = dict(zip(p_names, args, strict=True))
         return f(**coords, **params)
 
     return func
 
 
 def _get_sigma(da):
     if da.variances is None:
@@ -66,15 +75,15 @@
                 data=array(
                     dims=map_over,
                     values=pdata[..., i] if pdata.ndim > 1 else pdata[i],
                     variances=variances[..., i] if variances.ndim > 1 else variances[i],
                     unit=u,
                 ),
             )
-            for i, (p, u) in enumerate(zip(params, p_units))
+            for i, (p, u) in enumerate(zip(params, p_units, strict=True))
         }
     )
     dgcov = DataGroup(
         {
             p: DataGroup(
                 {
                     q: DataArray(
@@ -90,60 +99,62 @@
                                 if q_u == default_unit
                                 else q_u
                                 if p_u == default_unit
                                 else p_u * q_u
                             ),
                         ),
                     )
-                    for j, (q, q_u) in enumerate(zip(params, p_units))
+                    for j, (q, q_u) in enumerate(zip(params, p_units, strict=True))
                 }
             )
-            for i, (p, p_u) in enumerate(zip(params, p_units))
+            for i, (p, p_u) in enumerate(zip(params, p_units, strict=True))
         }
     )
     for c in da.coords:
         if set(map_over).intersection(da.coords[c].dims):
             for p in dg:
                 dg[p].coords[c] = da.coords[c]
                 for q in dgcov[p]:
                     dgcov[p][q].coords[c] = da.coords[c]
-
     for m in da.masks:
-        if set(map_over).intersection(da.masks[m].dims):
+        # Drop masks that don't fit the output data
+        if set(da.masks[m].dims).issubset(set(dg.dims)):
             for p in dg:
-                dg[p].masks[c] = da.masks[c]
+                dg[p].masks[m] = da.masks[m]
                 for q in dgcov[p]:
-                    dgcov[p][q].masks[c] = da.masks[c]
+                    dgcov[p][q].masks[m] = da.masks[m]
     return dg, dgcov
 
 
 def _prepare_numpy_outputs(da, params, map_over):
     shape = [da.sizes[d] for d in map_over]
-    dg = np.empty(shape + [len(params)])
+    dg = np.empty([*shape, len(params)])
     dgcov = np.empty(shape + 2 * [len(params)])
     return dg, dgcov
 
 
 def _make_defaults(f, coords, params):
     spec = getfullargspec(f)
-    all_args = set((*spec.args, *spec.kwonlyargs))
+    all_args = {*spec.args, *spec.kwonlyargs}
     if not set(coords).issubset(all_args):
         raise ValueError("Function must take the provided coords as arguments")
     default_arguments = dict(
-        zip(spec.args[-len(spec.defaults) :], spec.defaults) if spec.defaults else {},
+        zip(spec.args[-len(spec.defaults) :], spec.defaults, strict=True)
+        if spec.defaults
+        else {},
         **(spec.kwonlydefaults or {}),
     )
     return {
         **{a: 1.0 for a in all_args - set(coords)},
         **default_arguments,
         **(params or {}),
     }
 
 
-def _get_specific_bounds(bounds, name, unit) -> Tuple[float, float]:
+def _get_specific_bounds(bounds, name, unit) -> tuple[float, float]:
     if name not in bounds:
         return -np.inf, np.inf
     b = bounds[name]
     if len(b) != 2:
         raise ValueError(
             "Parameter bounds must be given as a tuple of length 2. "
             f"Got a collection of length {len(b)} as bounds for '{name}'."
@@ -154,15 +165,15 @@
             b[1].to(unit=unit, dtype=float).value,
         )
     return b
 
 
 def _parse_bounds(
     bounds, params
-) -> Union[Tuple[float, float], Tuple[np.ndarray, np.ndarray]]:
+) -> tuple[float, float] | tuple[np.ndarray, np.ndarray]:
     if bounds is None:
         return -np.inf, np.inf
 
     bounds_tuples = [
         _get_specific_bounds(
             bounds, name, param.unit if isinstance(param, Variable) else dimensionless
         )
@@ -197,27 +208,33 @@
                 (dg[i], dgcov[i]),
                 **kwargs,
             )
 
         return
 
     fda = da.flatten(to='row')
-
-    for m in fda.masks.values():
-        fda = fda[~m]
+    mask = irreducible_mask(fda.masks, 'row')
+    if mask is not None:
+        fda = fda[~mask]
 
     if not unsafe_numpy_f:
         # Making the coords into a dict improves runtime,
         # probably because of pybind overhead.
         X = dict(fda.coords)
     else:
         X = np.vstack([c.values for c in fda.coords.values()], dtype='float')
 
     import scipy.optimize as opt
 
+    if len(fda) < len(dg):
+        # More parameters than data points, unable to fit, abort.
+        dg[:] = np.nan
+        dgcov[:] = np.nan
+        return
+
     try:
         popt, pcov = opt.curve_fit(
             f,
             X,
             fda.data.values,
             p0,
             sigma=_get_sigma(fda),
@@ -232,26 +249,24 @@
             raise err
 
     dg[:] = popt
     dgcov[:] = pcov
 
 
 def curve_fit(
-    coords: Union[Sequence[str], Mapping[str, Union[str, Variable]]],
+    coords: Sequence[str] | Mapping[str, str | Variable],
     f: Callable,
     da: DataArray,
     *,
-    p0: Dict[str, Union[Variable, Real]] = None,
-    bounds: Optional[
-        Dict[str, Union[Tuple[Variable, Variable], Tuple[Real, Real]]]
-    ] = None,
-    reduce_dims: Sequence[str] = tuple(),
+    p0: dict[str, Variable | Real] | None = None,
+    bounds: dict[str, tuple[Variable, Variable] | tuple[Real, Real]] | None = None,
+    reduce_dims: Sequence[str] = (),
     unsafe_numpy_f: bool = False,
     **kwargs,
-) -> Tuple[DataGroup, DataGroup]:
+) -> tuple[DataGroup, DataGroup]:
     """Use non-linear least squares to fit a function, f, to data.
     The function interface is similar to that of :py:func:`xarray.DataArray.curvefit`.
 
     .. versionadded:: 23.12.0
 
     This is a wrapper around :py:func:`scipy.optimize.curve_fit`. See there for
     indepth documentation and keyword arguments. The differences are:
```

### Comparing `scipp-24.2.0/src/scipp/data/__init__.py` & `scipp-24.5.0/src/scipp/data/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/src/scipp/format/formatter.py` & `scipp-24.5.0/src/scipp/format/formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Gregory Tucker, Jan-Lukas Wynen
 
-from typing import Any, List, Tuple
+from collections.abc import Sequence
+from typing import Any
 
 import numpy as np
+import numpy.typing as npt
 
 import scipp
 
 from ..core.cpp_classes import DType, Unit, Variable
 from ..core.data_group import DataGroup
-from ._parse import FormatSpec, FormatType, parse
+from ._parse import FormatSpec, FormatType, Selection, parse
 
 
-def format_variable(self, format_spec: str) -> str:
+def format_variable(self: Variable, format_spec: str) -> str:
     """String formats the Variable according to the provided specification.
 
     Parameters
     ----------
     format_spec:
         Format specification;
         only 'c' for Compact error-reporting supported at present.
@@ -38,15 +40,15 @@
 
 def _format_unit(data: Variable) -> str:
     if data.unit is None:
         return '<no unit>'
     return f'[{data.unit}]'
 
 
-def _format_element(elem: Any, *, dtype: DType, spec: str):
+def _format_element(elem: Any, *, dtype: DType, spec: str) -> str:
     if spec:
         return f'{elem:{spec}}'
     if dtype in (DType.float64, DType.float32):
         # Replicate behavior of C++ formatter.
         return f'{elem:g}'
     if dtype == DType.string:
         return f'"{elem}"'
@@ -55,23 +57,23 @@
 
 def _format_scalar(data: Any, *, dtype: DType, spec: FormatSpec) -> str:
     if spec.length == 0:
         return '...'
     return _format_element(data, dtype=dtype, spec=spec.nested)
 
 
-def _as_flat_array(data):
+def _as_flat_array(data: npt.ArrayLike) -> npt.ArrayLike:
     if isinstance(data, np.ndarray):
         return data.flat
     if 'ElementArray' in repr(type(data)):
         return data
     return np.array([data])
 
 
-def _format_array_flat(data, *, dtype: DType, spec: FormatSpec) -> str:
+def _format_array_flat(data: Any, *, dtype: DType, spec: FormatSpec) -> str:
     if dtype in (
         DType.Variable,
         DType.DataArray,
         DType.Dataset,
         DType.VariableView,
         DType.DataArrayView,
         DType.DatasetView,
@@ -83,37 +85,38 @@
             return _format_array_flat_scipp_objects(data)
         elif isinstance(data, DataGroup):
             return _format_data_group_element(data)
     data = _as_flat_array(data)
     return _format_array_flat_regular(data, dtype=dtype, spec=spec)
 
 
-def _format_array_flat_scipp_objects(data) -> str:
+def _format_array_flat_scipp_objects(data: npt.ArrayLike) -> str:
     # Fallback because ElementArrayView does not allow us to
     # slice and access elements nicely.
     return str(data)
 
 
-def _format_data_group_element(data: scipp.DataGroup):
+def _format_data_group_element(data: scipp.DataGroup) -> str:
     return f'[{data}]'
 
 
-def _element_ranges(spec: FormatSpec) -> Tuple[slice, slice]:
-    if spec.selection == '^':
-        return slice(None, spec.length // 2), slice(-spec.length // 2, None)
-    if spec.selection == '<':
-        return slice(None, spec.length), slice(0, 0)
-    if spec.selection == '>':
-        return slice(0, 0), slice(-spec.length, None)
+def _element_ranges(spec: FormatSpec) -> tuple[slice, slice]:
+    match spec.selection:
+        case Selection.edges:
+            return slice(None, spec.length // 2), slice(-spec.length // 2, None)
+        case Selection.begin:
+            return slice(None, spec.length), slice(0, 0)
+        case Selection.end:
+            return slice(0, 0), slice(-spec.length, None)
 
 
 def _format_array_flat_regular(
-    data: np.ndarray, *, dtype: DType, spec: FormatSpec
+    data: Sequence[Any], *, dtype: DType, spec: FormatSpec
 ) -> str:
-    def _format_all_in(d) -> List[str]:
+    def _format_all_in(d: Sequence[Any]) -> list[str]:
         return [_format_element(e, dtype=dtype, spec=spec.nested) for e in d]
 
     if len(data) <= spec.length:
         elements = _format_all_in(data)
     elif spec.length == 0:
         elements = ['...']
     else:
@@ -162,25 +165,27 @@
     unt = "" if var.unit == Unit('dimensionless') else f" {var.unit}"
 
     # Iterate over array values to handle no- and infinite-precision cases
     if variances is None:
         formatted = [_format_element_compact(v) for v in values]
     else:
         formatted = [
-            _format_element_compact(*_round(v, e)) for v, e in zip(values, variances)
+            _format_element_compact(*_round(v, e))
+            for v, e in zip(values, variances, strict=True)
         ]
     return f"{', '.join(formatted)}{unt}"
 
 
 def _is_numeric(dtype: DType) -> bool:
-    dtype = str(dtype)
-    return any([x in dtype for x in ('float', 'int')])
+    return any(x in str(dtype) for x in ('float', 'int'))
 
 
-def _round(value, variance):
+def _round(
+    value: float, variance: float | None
+) -> tuple[float, float | None, float | None]:
     from numpy import floor, log10, power, round, sqrt
 
     # Treat 'infinite' precision the same as no variance
     if variance is None or variance == 0:
         return value, None, None
 
     # The uncertainty is the square root of the variance
@@ -208,15 +213,17 @@
     if precision > -1:
         # pad the error to have the right number of trailing zeros
         error *= int(positive_power)
 
     return value, error, precision
 
 
-def _format_element_compact(value, error=None, precision=None):
+def _format_element_compact(
+    value: float, error: float | None = None, precision: float | None = None
+) -> str:
     # Build the appropriate format string:
     # No variance (or infinite precision) values take no formatting string
     # Positive precision implies no decimals, with format '0.0f'
     format = '' if precision is None else f'0.{max(0, int(-precision)):d}f'
 
     # Format the value using the generated format string
     formatted = "{v:{s}}".format(v=value, s=format)
```

### Comparing `scipp-24.2.0/src/scipp/io/__init__.py` & `scipp-24.5.0/src/scipp/io/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @file
 # @author Simon Heybrock
 
-# flake8: noqa
+# ruff: noqa: F403
 
 """File input and output.
 
 All functions listed here are also available in :mod:`scipp.io` module directly,
 e.g., as ``scipp.io.load_hdf5``.
 
 See also `Reading and Writing Files <../../user-guide/reading-and-writing-files.ipynb>`_.
@@ -17,13 +17,13 @@
 .. currentmodule:: scipp.io
 
 .. autosummary::
 
    csv.load_csv
    hdf5.load_hdf5
    hdf5.save_hdf5
-"""
+"""  # noqa: E501
 
 from .csv import load_csv
 from .hdf5 import load_hdf5, save_hdf5
 
 __all__ = ["load_csv", "load_hdf5", "save_hdf5"]
```

### Comparing `scipp-24.2.0/src/scipp/io/csv.py` & `scipp-24.5.0/src/scipp/io/csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,44 +17,44 @@
 
 See Also
 --------
 pandas.read_csv:
     More details on the underlying parser.
 """
 
+from collections.abc import Iterable
 from io import BytesIO, StringIO
 from os import PathLike
-from typing import Iterable, Optional, Union
 
 from ..compat.pandas_compat import HeaderParserArg, from_pandas
 from ..core import Dataset
 
 
 # The typehint of filepath_or_buffer is less generic than in pd.read_csv
 # because the definitions of protocols are private in pandas.
 def _load_dataframe(
-    filepath_or_buffer: Union[str, PathLike, StringIO, BytesIO],
+    filepath_or_buffer: str | PathLike | StringIO | BytesIO,
     sep: str,
 ):
     try:
         import pandas as pd
     except ImportError:
         raise ImportError(
             "Pandas is required to load CSV files but not install. "
             "Install it with `pip install pandas` or "
             "`conda install -c conda-forge pandas`."
         ) from None
     return pd.read_csv(filepath_or_buffer, sep=sep)
 
 
 def load_csv(
-    filename: Union[str, PathLike, StringIO, BytesIO],
+    filename: str | PathLike | StringIO | BytesIO,
     *,
-    sep: Optional[str] = ',',
-    data_columns: Optional[Union[str, Iterable[str]]] = None,
+    sep: str | None = ',',
+    data_columns: str | Iterable[str] | None = None,
     header_parser: HeaderParserArg = None,
 ) -> Dataset:
     """Load a CSV file as a dataset.
 
     This function currently uses Pandas to load the file and converts the result
     into a :class:`scipp.Dataset`.
     Pandas is not a hard dependency of Scipp and will thus not be installed
```

### Comparing `scipp-24.2.0/src/scipp/io/hdf5.py` & `scipp-24.5.0/src/scipp/io/hdf5.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @file
 # @author Simon Heybrock
 
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Union
+from typing import Any, ClassVar
 
 import numpy as np
 
 from ..core.cpp_classes import Unit
 from ..logging import get_logger
 from ..typing import VariableLike
 
@@ -38,15 +38,15 @@
         d.vector3,
         d.linear_transform3,
         d.affine_transform3,
         d.translation3,
         d.rotation3,
     ]
     names = [str(dtype) for dtype in dtypes]
-    return dict(zip(names, dtypes))
+    return dict(zip(names, dtypes, strict=True))
 
 
 def _as_hdf5_type(a):
     if np.issubdtype(a.dtype, np.datetime64):
         return a.view(np.int64)
     return a
 
@@ -324,27 +324,27 @@
         group.attrs['name'] = data.name
         if VariableIO.write(group.create_group('data'), var=data.data) is None:
             return None
         views = [data.coords, data.masks, data.attrs]
         # Note that we write aligned and unaligned coords into the same group.
         # Distinction is via an attribute, which is more natural than having
         # 2 separate groups.
-        for view_name, view in zip(['coords', 'masks', 'attrs'], views):
+        for view_name, view in zip(['coords', 'masks', 'attrs'], views, strict=True):
             subgroup = group.create_group(view_name)
             _write_mapping(subgroup, view, override.get(view_name))
         return group
 
     @staticmethod
     def read(group, override=None):
         _check_scipp_header(group, 'DataArray')
         if override is None:
             override = {}
         from ..core import DataArray
 
-        contents = dict()
+        contents = {}
         contents['name'] = group.attrs['name']
         contents['data'] = VariableIO.read(group['data'])
         for category in ['coords', 'masks', 'attrs']:
             contents[category] = _read_mapping(group[category], override.get(category))
         return DataArray(**contents)
 
 
@@ -412,15 +412,15 @@
             _check_scipp_header(group, type_name)
             return convert(group['entry'][()])
 
     return GenericIO
 
 
 class HDF5IO:
-    _handlers = {
+    _handlers: ClassVar[dict[str, Any]] = {
         'Variable': VariableIO,
         'DataArray': DataArrayIO,
         'Dataset': DatasetIO,
         'DataGroup': DataGroupIO,
         'str': _direct_io(str, convert=lambda b: b.decode('utf-8')),
         'ndarray': _direct_io(np.ndarray, convert=lambda x: x),
         **{
@@ -454,21 +454,21 @@
         return handler.write(group, data, **kwargs)
 
     @classmethod
     def read(cls, group, **kwargs):
         return cls._handlers[group.attrs['scipp-type']].read(group, **kwargs)
 
 
-def save_hdf5(obj: VariableLike, filename: Union[str, Path]) -> None:
+def save_hdf5(obj: VariableLike, filename: str | Path) -> None:
     """Write an object out to file in HDF5 format."""
     import h5py
 
     with h5py.File(filename, 'w') as f:
         HDF5IO.write(f, obj)
 
 
-def load_hdf5(filename: Union[str, Path]) -> VariableLike:
+def load_hdf5(filename: str | Path) -> VariableLike:
     """Load a Scipp-HDF5 file."""
     import h5py
 
     with h5py.File(filename, 'r') as f:
         return HDF5IO.read(f)
```

### Comparing `scipp-24.2.0/src/scipp/logging.py` & `scipp-24.5.0/src/scipp/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 import html
 import logging
 import time
 from copy import copy
 from dataclasses import dataclass
-from typing import Any, Dict, Optional, Tuple
+from typing import Any
 
 from .core import DataArray, Dataset, Variable
 from .utils import running_in_jupyter
 from .visualization import make_html
 from .visualization.resources import load_style
 
 
@@ -135,15 +135,15 @@
     widget = get_log_widget()
     if widget is None:
         return
     widget.clear()
 
 
 def _has_html_repr(x: Any) -> bool:
-    return isinstance(x, (DataArray, Dataset, Variable))
+    return isinstance(x, DataArray | Dataset | Variable)
 
 
 def _make_html(x) -> str:
     return f'<div class="sc-log-html-payload">{make_html(x)}</div>'
 
 
 # This class is used with the log formatter to distinguish between str and repr.
@@ -159,28 +159,28 @@
     def __str__(self):
         return self._PATTERN.format(self._i)
 
     def __repr__(self):
         return repr(self._arg)
 
 
-def _preprocess_format_args(args) -> Tuple[Tuple, Dict[str, Any]]:
+def _preprocess_format_args(args) -> tuple[tuple, dict[str, Any]]:
     format_args = []
     replacements = {}
     for i, arg in enumerate(args):
         if _has_html_repr(arg):
             tag = _ReplacementPattern(i, arg)
             format_args.append(tag)
             replacements[str(tag)] = arg
         else:
             format_args.append(arg)
     return tuple(format_args), replacements
 
 
-def _replace_html_repr(message: str, replacements: Dict[str, str]) -> str:
+def _replace_html_repr(message: str, replacements: dict[str, str]) -> str:
     # Do separate check `key in message` in order to avoid calling
     # _make_html unnecessarily. Linear string searches are likely less
     # expensive than HTML formatting.
     for key, repl in replacements.items():
         if key in message:
             message = message.replace(key, _make_html(repl))
     return message
@@ -247,22 +247,22 @@
     Create a new widget log handler.
     :raises RuntimeError: If Python is not running in Jupyter.
     """
     handler = WidgetHandler(level=logging.INFO, widget=make_log_widget())
     return handler
 
 
-def get_widget_handler() -> Optional[WidgetHandler]:
+def get_widget_handler() -> WidgetHandler | None:
     """
     Return the widget handler installed in the Scipp logger.
     If multiple widget handlers are installed, only the first one is returned.
     If no widget handler is installed, returns ``None``.
     """
     try:
-        return next(  # type: ignore
+        return next(  # type: ignore[return-value]
             filter(
                 lambda handler: isinstance(handler, WidgetHandler),
                 get_logger().handlers,
             )
         )
     except StopIteration:
         return None
```

### Comparing `scipp-24.2.0/src/scipp/object_list.py` & `scipp-24.5.0/src/scipp/object_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     out = ''
     for category in ['Variable', 'DataArray', 'Dataset']:
         names = ipython.magic(f"who_ls {category}")
         out += (
             f"<details open=\"open\"><summary>{category}s:" f"({len(names)})</summary>"
         )
         for name in names:
-            html = make_html(eval(name, scope))  # nosec: B307
+            html = make_html(eval(name, scope))  # noqa: S307
             out += (
                 f"<details style=\"padding-left:2em\"><summary>"
                 f"{name}</summary>{html}</details>"
             )
         out += "</details>"
     from IPython.core.display import HTML, display
```

### Comparing `scipp-24.2.0/src/scipp/operations.py` & `scipp-24.5.0/src/scipp/operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
 import functools
+from collections.abc import Callable
 from inspect import signature
-from typing import Callable, Optional
 
 from ._scipp.core import transform as cpp_transform
 from .core import Variable
 
 
 def _as_numba_cfunc(function, unit_func=None):
     import numba
@@ -17,17 +17,17 @@
     cfunc = numba.cfunc(dtype + '(' + ','.join([dtype] * narg) + ')')(function)
     cfunc.unit_func = function if unit_func is None else unit_func
     cfunc.name = function.__name__
     return cfunc
 
 
 def elemwise_func(
-    func: Optional[Callable] = None,
+    func: Callable | None = None,
     *,
-    unit_func: Optional[Callable] = None,
+    unit_func: Callable | None = None,
     dtype: str = 'float64',
     auto_convert_dtypes: bool = False,
 ) -> Callable:
     """
     Create a function for transforming input variables based on element-wise operation.
 
     This uses ``numba.cfunc`` to compile a kernel that Scipp can use for transforming
```

### Comparing `scipp-24.2.0/src/scipp/reduction.py` & `scipp-24.5.0/src/scipp/reduction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
 import uuid
-from typing import Iterable, List
+from collections.abc import Iterable
 
 from .core import concat, reduction
 from .typing import VariableLike
 
 
 class BinsReducer:
     def __init__(self, obj: VariableLike, dim: str):
@@ -15,15 +15,15 @@
 
     def concat(self):
         """Element-wise 'concat' across bins of inputs passed to :py:func:`scipp.reduce`."""  # noqa: E501
         return self._obj.bins.concat(self._dim)
 
 
 class Reducer:
-    def __init__(self, x: List[VariableLike]):
+    def __init__(self, x: list[VariableLike]):
         self._dim = uuid.uuid4().hex
         # concat in init avoids repeated costly step in case of multiple reductions
         self._obj = concat(x, dim=self._dim)
 
     @property
     def bins(self):
         return BinsReducer(self._obj, self._dim)
@@ -79,9 +79,9 @@
       >>> sc.reduce([a, b]).max()
       <scipp.Variable> (x: 4)    float64  [dimensionless]  [0.2, 0.4, 0.666667, 1]
       >>> sc.reduce([a, b]).sum()
       <scipp.Variable> (x: 4)    float64  [dimensionless]  [0.2, 0.733333, 1.26667, 1.8]
 
     :param x: List or tuple of variables or data arrays
     :return: Reducer helper object with methods such as ``sum()`` or ``max()``
-    """  # noqa: E501
+    """
     return Reducer(list(x))
```

### Comparing `scipp-24.2.0/src/scipp/scipy/integrate/__init__.py` & `scipp-24.5.0/src/scipp/scipy/integrate/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,35 +3,39 @@
 # @author Simon Heybrock
 """Sub-package for integration.
 
 This subpackage provides wrappers for a subset of functions from
 :py:mod:`scipy.integrate`.
 """
 
-from typing import Callable
+from collections.abc import Callable
+from typing import Any
+
+import numpy.typing as npt
 
 from ...compat.wrapping import wrap1d
 from ...core import DataArray, array
 
 
-def _integrate(func: Callable, da: DataArray, dim: str, **kwargs) -> DataArray:
+def _integrate(
+    func: Callable[..., npt.NDArray[Any]], da: DataArray, dim: str, **kwargs: Any
+) -> DataArray:
     if 'dx' in kwargs:
         raise ValueError(
             "Invalid argument 'dx': Spacing of integration points is "
             f"given by the '{dim}' coord."
         )
     integral = func(x=da.coords[dim].values, y=da.values, **kwargs)
     dims = [d for d in da.dims if d != dim]
-    return DataArray(
-        data=array(dims=dims, values=integral, unit=da.unit * da.coords[dim].unit)
-    )
+    unit = da.unit * da.coords[dim].unit  # type: ignore[operator]  # from unit = None
+    return DataArray(data=array(dims=dims, values=integral, unit=unit))
 
 
 @wrap1d()
-def trapezoid(da: DataArray, dim: str, **kwargs) -> DataArray:
+def trapezoid(da: DataArray, dim: str, **kwargs: Any) -> DataArray:
     """Integrate data array along the given dimension with
     the composite trapezoidal rule.
 
     This is a wrapper around :py:func:`scipy.integrate.trapezoid`.
 
     Examples:
 
@@ -46,15 +50,15 @@
     """
     import scipy.integrate as integ
 
     return _integrate(integ.trapezoid, da, dim, **kwargs)
 
 
 @wrap1d()
-def simpson(da: DataArray, dim: str, **kwargs) -> DataArray:
+def simpson(da: DataArray, dim: str, **kwargs: Any) -> DataArray:
     """Integrate data array along the given dimension with the composite Simpson's rule.
 
     This is a wrapper around :py:func:`scipy.integrate.simpson`.
 
     Examples:
 
       >>> x = sc.geomspace(dim='x', start=0.1, stop=0.4, num=4, unit='m')
```

### Comparing `scipp-24.2.0/src/scipp/scipy/interpolate/__init__.py` & `scipp-24.5.0/src/scipp/scipy/interpolate/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,75 +3,78 @@
 # @author Simon Heybrock
 """Sub-package for objects used in interpolation.
 
 This subpackage provides wrappers for a subset of functions from
 :py:mod:`scipy.interpolate`.
 """
 
-from typing import Any, Callable, Literal, Union
+from __future__ import annotations
+
+from typing import Any, Literal, Protocol, TypeVar
 
 import numpy as np
+import numpy.typing as npt
 
 from ...compat.wrapping import wrap1d
-from ...core import (  # NOQA
+from ...core import (
     DataArray,
     DimensionError,
     DType,
     UnitError,
     Variable,
     empty,
     epoch,
     irreducible_mask,
 )
 
+_ArrayOrVar = TypeVar('_ArrayOrVar', npt.NDArray[Any], Variable)
+
 
-def _as_interpolation_type(x):
+def _as_interpolation_type(x: _ArrayOrVar) -> _ArrayOrVar:
     if isinstance(x, np.ndarray):
         if x.dtype.kind == 'M':
             return x.astype('int64', copy=False)
     else:
         if x.dtype == DType.datetime64:
             return x - epoch(unit=x.unit)
     return x
 
 
-def _midpoints(var, dim):
+def _midpoints(var: Variable, dim: str) -> Variable:
     a = var[dim, :-1]
     b = var[dim, 1:]
     return _as_interpolation_type(a) + 0.5 * (b - a)
 
 
-def _drop_masked(da, dim):
+def _drop_masked(da: DataArray, dim: str) -> DataArray:
     if (mask := irreducible_mask(da.masks, dim)) is not None:
         return da[~mask]
     return da
 
 
 @wrap1d(is_partial=True, accept_masks=True)
 def interp1d(
     da: DataArray,
     dim: str,
     *,
-    kind: Union[
-        int,
-        Literal[
-            'linear',
-            'nearest',
-            'nearest-up',
-            'zero',
-            'slinear',
-            'quadratic',
-            'cubic',
-            'previous',
-            'next',
-        ],
+    kind: int
+    | Literal[
+        'linear',
+        'nearest',
+        'nearest-up',
+        'zero',
+        'slinear',
+        'quadratic',
+        'cubic',
+        'previous',
+        'next',
     ] = 'linear',
     fill_value: Any = np.nan,
-    **kwargs,
-) -> Callable:
+    **kwargs: Any,
+) -> _Interp1dImpl:
     """Interpolate a 1-D function.
 
     A data array is used to approximate some function f: y = f(x), where y is given by
     the array values and x is is given by the coordinate for the given dimension. This
     class returns a function whose call method uses interpolation to find the value of
     new points.
 
@@ -158,30 +161,38 @@
                                   float64  [dimensionless]  (x)  [0.155548, 0.266977, ..., 0.918992, 0.963297]
 
     .. plot:: :context: close-figs
 
       >>> sc.plot({'original':da,
       ...          'interp1d':f(xnew),
       ...          'interp1d-midpoints':f(xnew, midpoints=True)})
-    """  # noqa #501
+    """  # noqa: E501
     import scipy.interpolate as inter
 
     da = _drop_masked(da, dim)
 
-    def func(xnew: Variable, *, midpoints=False) -> DataArray:
+    def func(xnew: Variable, *, midpoints: bool = False) -> DataArray:
         """Compute interpolation function defined by ``interp1d``
         at interpolation points.
 
-        :param xnew: Interpolation points.
-        :param midpoints: Interpolate at midpoints of given points. The result will be
-                          a histogram. Default is ``False``.
-        :return: Interpolated data array with new coord given by interpolation points
-                 and data given by interpolation function evaluated at the
-                 interpolation points (or evaluated at the midpoints of the given
-                 points).
+        Parameters
+        ----------
+        xnew:
+            Interpolation points.
+        midpoints:
+            Interpolate at midpoints of given points.
+            The result will be a histogram.
+            Default is ``False``.
+
+        Returns
+        -------
+        :
+            Interpolated data array with new coord given by interpolation points
+            and data given by interpolation function evaluated at the
+            interpolation points (or evaluated at the midpoints of the given points).
         """
         if xnew.unit != da.coords[dim].unit:
             raise UnitError(
                 f"Unit of interpolation points '{xnew.unit}' does not match unit "
                 f"'{da.coords[dim].unit}' of points defining the interpolation "
                 "function along dimension '{dim}'."
             )
@@ -205,8 +216,12 @@
         ynew = empty(sizes=sizes, unit=da.unit, dtype=da.dtype)
         ynew.values = f(x_.values)
         return DataArray(data=ynew, coords={dim: xnew})
 
     return func
 
 
+class _Interp1dImpl(Protocol):
+    def __call__(self, xnew: Variable, *, midpoints: bool = False) -> DataArray: ...
+
+
 __all__ = ['interp1d']
```

### Comparing `scipp-24.2.0/src/scipp/scipy/ndimage/__init__.py` & `scipp-24.5.0/src/scipp/scipy/ndimage/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,87 +2,107 @@
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
 """Sub-package for multidimensional image processing.
 
 This subpackage provides wrappers for a subset of functions from
 :py:mod:`scipy.ndimage`.
 """
+
+from collections.abc import Callable, Mapping
 from functools import wraps
-from typing import Callable, Dict, Optional, Union
+from typing import Any, Protocol, TypeVar
 
 import scipy.ndimage
 
-from ...core import (  # NOQA
+from ...core import (
     CoordError,
     DataArray,
     DimensionError,
     Variable,
     VariancesError,
     empty_like,
     islinspace,
     ones,
 )
-from ...typing import VariableLike, VariableLikeType
+from ...typing import VariableLike
+
+_T = TypeVar('_T', Variable, DataArray)
 
 
-def _ndfilter(func: Callable) -> Callable:
+def _ndfilter(
+    func: Callable[..., _T],
+) -> Callable[..., _T]:
     @wraps(func)
-    def function(x: Union[Variable, DataArray], **kwargs) -> Union[Variable, DataArray]:
+    def function(x: _T, **kwargs: Any) -> _T:
         if 'output' in kwargs:
             raise TypeError("The 'output' argument is not supported")
         if x.variances is not None:
             raise VariancesError(
                 "Filter cannot be applied to input array with variances."
             )
         if getattr(x, 'masks', None):
             raise ValueError("Filter cannot be applied to input array with masks.")
         return func(x, **kwargs)
 
     return function
 
 
-def _delta_to_positional(x: Union[Variable, DataArray], dim, index, dtype):
+def _delta_to_positional(
+    x: Any,
+    dim: str,
+    index: float | Variable | Mapping[str, float | Variable],
+    dtype: type,
+) -> Any:
     if not isinstance(index, Variable):
         return index
     coord = x.coords[dim]
     if not islinspace(coord, dim).value:
         raise CoordError(
             f"Data points not regularly spaced along {dim}. To ignore this, "
             f"provide a plain value (convertible to {dtype.__name__}) instead of a "
             "scalar variable. Note that this will correspond to plain positional "
             "indices/offsets."
         )
     pos = (len(coord) - 1) * (index.to(unit=coord.unit) / (coord[-1] - coord[0])).value
     return dtype(pos)
 
 
-def _require_matching_dims(index, x, name):
+def _require_matching_dims(
+    index: Mapping[str, float | Variable],
+    x: VariableLike,
+    name: str | None,
+) -> None:
     if set(index) != set(x.dims):
         raise KeyError(
             f"Data has dims={x.dims} but input argument '{name}' provides "
             f"values for {tuple(index)}"
         )
 
 
-def _positional_index(x: Union[Variable, DataArray], index, name=None, dtype=int):
-    if not isinstance(index, dict):
+def _positional_index(
+    x: Any,
+    index: float | Variable | Mapping[str, float | Variable],
+    name: str | None = None,
+    dtype: type = int,
+) -> list[Any]:
+    if not isinstance(index, Mapping):
         return [_delta_to_positional(x, dim, index, dtype=dtype) for dim in x.dims]
     _require_matching_dims(index, x, name)
     return [_delta_to_positional(x, dim, index[dim], dtype=dtype) for dim in x.dims]
 
 
 @_ndfilter
 def gaussian_filter(
-    x: VariableLikeType,
+    x: _T,
     /,
     *,
-    sigma: Union[int, float, Variable, Dict[str, Union[int, float, Variable]]],
-    order: Optional[Union[int, Dict[str, int]]] = 0,
-    **kwargs,
-) -> VariableLikeType:
+    sigma: float | Variable | Mapping[str, float | Variable],
+    order: int | Mapping[str, int] | None = 0,
+    **kwargs: Any,
+) -> _T:
     """
     Multidimensional Gaussian filter.
 
     This is a wrapper around :py:func:`scipy.ndimage.gaussian_filter`. See there for
     full argument description. There are two key differences:
 
     - This wrapper uses explicit dimension labels in the ``sigma`` and ``order``
@@ -148,57 +168,78 @@
 
     .. plot:: :context: close-figs
 
       >>> filtered = gaussian_filter(da, sigma={'x':sc.scalar(0.01, unit='mm'),
       ...                                       'y':sc.scalar(1.0, unit='mm')})
       >>> filtered.plot()
     """
-    sigma = _positional_index(x, sigma, name='sigma', dtype=float)
-    if isinstance(order, dict):
+    sigma_values = _positional_index(x, sigma, name='sigma', dtype=float)
+    if isinstance(order, Mapping):
         _require_matching_dims(order, x, 'order')
-        order = [order[dim] for dim in x.dims]
+        order = [order[dim] for dim in x.dims]  # type: ignore[assignment]
     out = empty_like(x)
     scipy.ndimage.gaussian_filter(
-        x.values, sigma=sigma, order=order, output=out.values, **kwargs
+        x.values, sigma=sigma_values, order=order, output=out.values, **kwargs
     )
     return out
 
 
-def _make_footprint(x: Union[Variable, DataArray], size, footprint) -> Variable:
+def _make_footprint(
+    x: Variable | DataArray,
+    size: int | Variable | Mapping[str, int | Variable] | None,
+    footprint: Variable | None,
+) -> Variable:
     if footprint is None:
-        size = _positional_index(x, size, name='size')
-        footprint = ones(dims=x.dims, shape=size, dtype='bool')
+        if size is None:
+            raise ValueError("Provide either 'footprint' or 'size'.")
+        footprint = ones(
+            dims=x.dims, shape=_positional_index(x, size, name='size'), dtype='bool'
+        )
     else:
         if size is not None:
             raise ValueError("Provide either 'size' or 'footprint', not both.")
         if set(footprint.dims) != set(x.dims):
             raise DimensionError(
                 f"Dimensions {footprint.dims} must match data dimensions {x.dim}"
             )
     return footprint
 
 
-def _make_footprint_filter(name, example=True, extra_args=''):
+class _FootprintFilter(Protocol):
+    def __call__(
+        self,
+        x: _T,
+        /,
+        *,
+        size: int | Variable | Mapping[str, int | Variable] | None = None,
+        footprint: Variable | None = None,
+        origin: int | Variable | Mapping[str, int | Variable] | None = 0,
+        **kwargs: Any,
+    ) -> _T: ...
+
+
+def _make_footprint_filter(
+    name: str, example: bool = True, extra_args: str = ''
+) -> _FootprintFilter:
     def footprint_filter(
-        x: VariableLike,
+        x: _T,
         /,
         *,
-        size: Optional[Union[int, Variable, Dict[str, Union[int, Variable]]]] = None,
-        footprint: Optional[Variable] = None,
-        origin: Optional[Union[int, Variable, Dict[str, Union[int, Variable]]]] = 0,
-        **kwargs,
-    ) -> VariableLike:
+        size: int | Variable | Mapping[str, int | Variable] | None = None,
+        footprint: Variable | None = None,
+        origin: int | Variable | Mapping[str, int | Variable] = 0,
+        **kwargs: Any,
+    ) -> _T:
         footprint = _make_footprint(x, size=size, footprint=footprint)
-        origin = _positional_index(x, origin, name='origin')
         out = empty_like(x)
         scipy_filter = getattr(scipy.ndimage, name)
         scipy_filter(
             x.values,
             footprint=footprint.values,
-            origin=origin,
+            origin=_positional_index(x, origin, name='origin'),
             output=out.values,
             **kwargs,
         )
         return out
 
     footprint_filter.__name__ = name
     if extra_args:
```

### Comparing `scipp-24.2.0/src/scipp/scipy/optimize/__init__.py` & `scipp-24.5.0/src/scipp/scipy/optimize/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,125 +3,159 @@
 # @author Simon Heybrock
 """Sub-package for optimization such as curve fitting.
 
 This subpackage provides wrappers for a subset of functions from
 :py:mod:`scipy.optimize`.
 """
 
+from collections.abc import Callable, Iterable
 from inspect import getfullargspec
 from numbers import Real
-from typing import Callable, Dict, Optional, Tuple, Union
+from typing import Any
 
 import numpy as np
+import numpy.typing as npt
 
-from ...core import BinEdgeError, DataArray, Variable, scalar, stddevs
+from ...core import (
+    BinEdgeError,
+    DataArray,
+    DefaultUnit,
+    Unit,
+    Variable,
+    scalar,
+    stddevs,
+)
+from ...typing import VariableLike
 from ...units import default_unit, dimensionless
 from ..interpolate import _drop_masked
 
 
-def _as_scalar(obj, unit):
+def _as_scalar(obj: Any, unit: Unit | DefaultUnit | None) -> Any:
     if unit == default_unit:
         return obj
-    return scalar(value=obj, unit=unit)
+    return scalar(
+        value=obj,
+        unit=unit,  # type:ignore[arg-type] # unit cannot be DefaultUnit here
+    )
 
 
-def _wrap_func(f, p_names, p_units):
-    def func(x, *args):
-        p = {k: _as_scalar(v, u) for k, v, u in zip(p_names, args, p_units)}
-        return f(x, **p).values
+def _wrap_func(
+    f: Callable[..., Variable | DataArray],
+    p_names: Iterable[str],
+    p_units: Iterable[Unit | DefaultUnit | None],
+) -> Callable[..., npt.NDArray[Any]]:
+    def func(x: VariableLike, *args: Any) -> npt.NDArray[Any]:
+        p = {
+            k: _as_scalar(v, u) for k, v, u in zip(p_names, args, p_units, strict=True)
+        }
+        return f(x, **p).values  # type: ignore[no-any-return]
 
     return func
 
 
-def _get_sigma(da):
+def _get_sigma(
+    da: Variable | DataArray,
+) -> npt.NDArray[np.float64 | np.float32] | None:
     if da.variances is None:
         return None
 
     sigma = stddevs(da).values
     if not sigma.all():
         raise ValueError(
             'There is a 0 in the input variances. This would break the optimizer. '
             'Mask the offending elements, remove them, or assign a meaningful '
             'variance if possible before calling curve_fit.'
         )
-    return sigma
+    return sigma  # type: ignore[no-any-return]
 
 
-def _covariance_with_units(p_names, pcov_values, units):
-    pcov = {}
+def _covariance_with_units(
+    p_names: list[str],
+    pcov_values: npt.NDArray[np.float64 | np.float32],
+    units: list[Unit | DefaultUnit],
+) -> dict[str, dict[str, Variable | Real]]:
+    pcov: dict[str, dict[str, Variable | Real]] = {}
     for i, row in enumerate(pcov_values):
         pcov[p_names[i]] = {}
         for j, elem in enumerate(row):
             ui = units[i]
             uj = units[j]
             u = ui
             if u == default_unit:
                 u = uj
             elif uj != default_unit:
-                u = ui * uj
+                u = ui * uj  # type: ignore[operator]  # neither operand is DefaultUnit
             pcov[p_names[i]][p_names[j]] = _as_scalar(elem, u)
     return pcov
 
 
-def _make_defaults(f, p0):
+def _make_defaults(
+    f: Callable[..., Any], p0: dict[str, Variable | float] | None
+) -> dict[str, Any]:
     spec = getfullargspec(f)
     if len(spec.args) != 1 or spec.varargs is not None:
         raise ValueError("Fit function must take exactly one positional argument")
     defaults = {} if spec.kwonlydefaults is None else spec.kwonlydefaults
-    kwargs = {arg: 1.0 for arg in spec.kwonlyargs if arg not in defaults}
+    kwargs: dict[str, Any] = {
+        arg: 1.0 for arg in spec.kwonlyargs if arg not in defaults
+    }
     if p0 is not None:
         kwargs.update(p0)
     return kwargs
 
 
-def _get_specific_bounds(bounds, name, unit) -> Tuple[float, float]:
+def _get_specific_bounds(
+    bounds: dict[str, tuple[Variable, Variable] | tuple[float, float]],
+    name: str,
+    unit: Unit | None,
+) -> tuple[float, float]:
     if name not in bounds:
         return -np.inf, np.inf
     b = bounds[name]
     if len(b) != 2:
         raise ValueError(
             "Parameter bounds must be given as a tuple of length 2. "
             f"Got a collection of length {len(b)} as bounds for '{name}'."
         )
     if isinstance(b[0], Variable):
         return (
-            b[0].to(unit=unit, dtype=float).value,
-            b[1].to(unit=unit, dtype=float).value,
+            b[0].to(unit=unit, dtype=float).value,  # type: ignore[attr-defined]
+            b[1].to(unit=unit, dtype=float).value,  # type: ignore[attr-defined]
         )
     return b
 
 
 def _parse_bounds(
-    bounds, params
-) -> Union[Tuple[float, float], Tuple[np.ndarray, np.ndarray]]:
+    bounds: dict[str, tuple[Variable, Variable] | tuple[float, float]] | None,
+    params: dict[str, Any],
+) -> (
+    tuple[float, float]
+    | tuple[npt.NDArray[np.float64 | np.float32], npt.NDArray[np.float64 | np.float32]]
+):
     if bounds is None:
         return -np.inf, np.inf
 
     bounds_tuples = [
         _get_specific_bounds(
             bounds, name, param.unit if isinstance(param, Variable) else dimensionless
         )
         for name, param in params.items()
     ]
     bounds_array = np.array(bounds_tuples).T
     return bounds_array[0], bounds_array[1]
 
 
 def curve_fit(
-    f: Callable,
+    f: Callable[..., Variable | DataArray],
     da: DataArray,
     *,
-    p0: Dict[str, Union[Variable, Real]] = None,
-    bounds: Optional[
-        Dict[str, Union[Tuple[Variable, Variable], Tuple[Real, Real]]]
-    ] = None,
-    **kwargs,
-) -> Tuple[
-    Dict[str, Union[Variable, Real]], Dict[str, Dict[str, Union[Variable, Real]]]
-]:
+    p0: dict[str, Variable | float] | None = None,
+    bounds: dict[str, tuple[Variable, Variable] | tuple[float, float]] | None = None,
+    **kwargs: Any,
+) -> tuple[dict[str, Variable | float], dict[str, dict[str, Variable | float]]]:
     """Use non-linear least squares to fit a function, f, to data.
 
     This is a wrapper around :py:func:`scipy.optimize.curve_fit`. See there for a
     complete description of parameters. The differences are:
 
     - Instead of separate xdata, ydata, and sigma arguments, the input data array
       defines provides these, with sigma defined as the square root of the variances,
@@ -224,26 +258,28 @@
     import scipy.optimize as opt
 
     da = _drop_masked(da, da.dim)
     params = _make_defaults(f, p0)
     p_units = [
         p.unit if isinstance(p, Variable) else default_unit for p in params.values()
     ]
-    p0 = [p.value if isinstance(p, Variable) else p for p in params.values()]
+    p0_values = [p.value if isinstance(p, Variable) else p for p in params.values()]
     popt, pcov = opt.curve_fit(
         f=_wrap_func(f, params.keys(), p_units),
         xdata=da.coords[da.dim],
         ydata=da.values,
         sigma=_get_sigma(da),
-        p0=p0,
+        p0=p0_values,
         bounds=_parse_bounds(bounds, params),
         **kwargs,
     )
     popt = {
         name: scalar(value=val, variance=var, unit=u)
-        for name, val, var, u in zip(params.keys(), popt, np.diag(pcov), p_units)
+        for name, val, var, u in zip(
+            params.keys(), popt, np.diag(pcov), p_units, strict=True
+        )
     }
     pcov = _covariance_with_units(list(params.keys()), pcov, p_units)
     return popt, pcov
 
 
 __all__ = ['curve_fit']
```

### Comparing `scipp-24.2.0/src/scipp/scipy/signal/__init__.py` & `scipp-24.5.0/src/scipp/scipy/signal/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
 """Sub-package for signal processing such as smoothing.
 
 This subpackage provides wrappers for a subset of functions from
 :py:mod:`scipy.signal`.
 """
+
 from dataclasses import dataclass
-from typing import Union
+from typing import Any
 
-from numpy import ndarray
+import numpy.typing as npt
 
 from ...compat.wrapping import wrap1d
-from ...core import (  # NOQA
+from ...core import (
     CoordError,
     DataArray,
     UnitError,
     Variable,
     array,
     identical,
     islinspace,
@@ -30,33 +31,31 @@
     """
     Second-order sections representation returned by :py:func:`scipp.signal.butter`.
 
     This is used as input to :py:func:`scipp.signal.sosfiltfilt`.
     """
 
     coord: Variable
-    sos: ndarray
+    sos: npt.NDArray[Any]
 
-    def filtfilt(
-        self, obj: Union[Variable, DataArray], dim: str, **kwargs
-    ) -> DataArray:
+    def filtfilt(self, obj: Variable | DataArray, dim: str, **kwargs: Any) -> DataArray:
         """
         Forwards to :py:func:`scipp.signal.sosfiltfilt` with sos argument set to the SOS
         instance.
         """
         return sosfiltfilt(obj, dim=dim, sos=self, **kwargs)
 
 
 def _frequency(coord: Variable) -> Variable:
     if not islinspace(coord).value:
         raise CoordError("Data is not regularly sampled, cannot compute frequency.")
     return (len(coord) - 1) / (coord[-1] - coord[0])
 
 
-def butter(coord: Variable, *, N: int, Wn: Variable, **kwargs) -> SOS:
+def butter(coord: Variable, *, N: int, Wn: Variable, **kwargs: Any) -> SOS:
     """
     Butterworth digital and analog filter design.
 
     Design an Nth-order digital or analog Butterworth filter and return the filter
     coefficients.
 
     This is intended for use with :py:func:`scipp.scipy.signal.sosfiltfilt`. See there
@@ -87,15 +86,15 @@
     return SOS(
         coord=coord.copy(),
         sos=scipy.signal.butter(N=N, Wn=Wn.values, fs=fs, output='sos', **kwargs),
     )
 
 
 @wrap1d(keep_coords=True)
-def _sosfiltfilt(da: DataArray, dim: str, *, sos: SOS, **kwargs) -> DataArray:
+def _sosfiltfilt(da: DataArray, dim: str, *, sos: SOS, **kwargs: Any) -> DataArray:
     if not identical(da.coords[dim], sos.coord):
         raise CoordError(
             f"Coord\n{da.coords[dim]}\nof filter dimension '{dim}' does "
             f"not match coord\n{sos.coord}\nused for creating the "
             "second-order sections representation by "
             "scipp.scipy.signal.butter."
         )
@@ -106,15 +105,15 @@
         unit=da.unit,
         values=scipy.signal.sosfiltfilt(sos.sos, da.values, **kwargs),
     )
     return DataArray(data=data)
 
 
 def sosfiltfilt(
-    obj: Union[Variable, DataArray], dim: str, *, sos: SOS, **kwargs
+    obj: Variable | DataArray, dim: str, *, sos: SOS, **kwargs: Any
 ) -> DataArray:
     """
     A forward-backward digital filter using cascaded second-order sections.
 
     This is a wrapper around :py:func:`scipy.signal.sosfiltfilt`. See there for a
     complete description of parameters. The differences are:
```

### Comparing `scipp-24.2.0/src/scipp/serialization.py` & `scipp-24.5.0/src/scipp/serialization.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
-from typing import Dict, List, Tuple, Union
 
 from .core import DataArray, Dataset, Variable
 
 
-def serialize(var: Union[Variable, DataArray, Dataset]) -> Tuple[Dict, List[bytes]]:
+def serialize(var: Variable | DataArray | Dataset) -> tuple[dict, list[bytes]]:
     """Serialize Scipp object."""
     from io import BytesIO
 
     import h5py
 
     from .io.hdf5 import HDF5IO
 
@@ -18,17 +17,15 @@
     buf = BytesIO()
     with h5py.File(buf, "w") as f:
         HDF5IO.write(f, var)
     frames = [buf.getvalue()]
     return header, frames
 
 
-def deserialize(
-    header: Dict, frames: List[bytes]
-) -> Union[Variable, DataArray, Dataset]:
+def deserialize(header: dict, frames: list[bytes]) -> Variable | DataArray | Dataset:
     """Deserialize Scipp object."""
     from io import BytesIO
 
     import h5py
 
     from .io.hdf5 import HDF5IO
```

### Comparing `scipp-24.2.0/src/scipp/spatial/__init__.py` & `scipp-24.5.0/src/scipp/spatial/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 --------
 scipp.vector:
     Construct a scalar variable holding a 3-vector.
 scipp.vectors:
     Construct an array variable holding 3-vectors.
 """
 
-from typing import Sequence, Union
+from collections.abc import Sequence
 
 import numpy as _np
 import numpy as np
 
 from .. import units
 from .._scipp import core as _core_cpp
 from ..core import DType, Unit, UnitError, Variable, vectors
@@ -72,16 +72,16 @@
         _core_cpp.geometry.as_vectors,
         *(c.to(dtype='float64', copy=False) for c in (x, y, z)),
     )
 
 
 def translation(
     *,
-    unit: Union[Unit, str] = units.dimensionless,
-    value: Union[_np.ndarray, list],
+    unit: Unit | str = units.dimensionless,
+    value: _np.ndarray | list,
 ):
     """
     Creates a translation transformation from a single provided 3-vector.
 
     Parameters
     ----------
     unit:
@@ -96,16 +96,16 @@
     """
     return translations(dims=(), unit=unit, values=value)
 
 
 def translations(
     *,
     dims: Sequence[str],
-    unit: Union[Unit, str] = units.dimensionless,
-    values: Union[_np.ndarray, list],
+    unit: Unit | str = units.dimensionless,
+    values: _np.ndarray | list,
 ):
     """
     Creates translation transformations from multiple 3-vectors.
 
     Parameters
     ----------
     dims:
@@ -121,15 +121,15 @@
         An array variable of dtype ``translation3``.
     """
     return _core_cpp.Variable(
         dims=dims, unit=unit, values=values, dtype=DType.translation3
     )
 
 
-def scaling_from_vector(*, value: Union[_np.ndarray, list]):
+def scaling_from_vector(*, value: _np.ndarray | list):
     """
     Creates a scaling transformation from a provided 3-vector.
 
     Parameters
     ----------
     value:
         A list or NumPy array of 3 values, corresponding to scaling
@@ -139,15 +139,15 @@
     -------
     :
        A scalar variable of dtype ``linear_transform3``.
     """
     return linear_transforms(dims=[], values=_np.diag(value))
 
 
-def scalings_from_vectors(*, dims: Sequence[str], values: Union[_np.ndarray, list]):
+def scalings_from_vectors(*, dims: Sequence[str], values: _np.ndarray | list):
     """
     Creates scaling transformations from corresponding to the provided 3-vectors.
 
     Parameters
     ----------
     dims:
         The dimensions of the variable.
@@ -165,15 +165,15 @@
     for field_name, index in (("xx", 0), ("yy", 1), ("zz", 2)):
         matrices.fields[field_name] = Variable(
             dims=dims, values=np.asarray(values)[:, index], dtype="float64"
         )
     return matrices
 
 
-def rotation(*, value: Union[_np.ndarray, list]):
+def rotation(*, value: _np.ndarray | list):
     """
     Creates a rotation-type variable from the provided quaternion coefficients.
 
     The quaternion coefficients are provided in scalar-last order (x, y, z, w), where
     x, y, z and w form the quaternion
 
     .. math::
@@ -198,15 +198,15 @@
     -------
     :
         A scalar variable of dtype ``rotation3``.
     """
     return rotations(dims=(), values=value)
 
 
-def rotations(*, dims: Sequence[str], values: Union[_np.ndarray, list]):
+def rotations(*, dims: Sequence[str], values: _np.ndarray | list):
     """
     Creates a rotation-type variable from the provided quaternion coefficients.
 
     The quaternion coefficients are provided in scalar-last order (x, y, z, w), where
     x, y, z and w form the quaternion
 
     .. math::
@@ -310,16 +310,16 @@
     return vectors(
         dims=rotation.dims, values=r.as_rotvec(degrees=unit == units.deg), unit=unit
     )
 
 
 def affine_transform(
     *,
-    unit: Union[Unit, str] = units.dimensionless,
-    value: Union[_np.ndarray, list],
+    unit: Unit | str = units.dimensionless,
+    value: _np.ndarray | list,
 ):
     """
     Initializes a single affine transformation from the provided affine matrix
     coefficients.
 
     Parameters
     ----------
@@ -335,16 +335,16 @@
     """
     return affine_transforms(dims=[], unit=unit, values=value)
 
 
 def affine_transforms(
     *,
     dims: Sequence[str],
-    unit: Union[Unit, str] = units.dimensionless,
-    values: Union[_np.ndarray, list],
+    unit: Unit | str = units.dimensionless,
+    values: _np.ndarray | list,
 ):
     """
     Initializes affine transformations from the provided affine matrix
     coefficients.
 
     Parameters
     ----------
@@ -366,16 +366,16 @@
         values=_to_eigen_layout(values),
         dtype=DType.affine_transform3,
     )
 
 
 def linear_transform(
     *,
-    unit: Union[Unit, str] = units.dimensionless,
-    value: Union[_np.ndarray, list],
+    unit: Unit | str = units.dimensionless,
+    value: _np.ndarray | list,
 ):
     """Constructs a zero dimensional :class:`Variable` holding a single 3x3
     matrix.
 
     Parameters
     ----------
     value:
@@ -394,16 +394,16 @@
         values=value,
     )
 
 
 def linear_transforms(
     *,
     dims: Sequence[str],
-    unit: Union[Unit, str] = units.dimensionless,
-    values: Union[_np.ndarray, list],
+    unit: Unit | str = units.dimensionless,
+    values: _np.ndarray | list,
 ):
     """Constructs a :class:`Variable` with given dimensions holding an array
     of 3x3 matrices.
 
     Parameters
     ----------
     dims:
```

### Comparing `scipp-24.2.0/src/scipp/sphinxext/autoplot.py` & `scipp-24.5.0/src/scipp/sphinxext/autoplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,68 +36,67 @@
         >>> sc.arange('x',5).plot()
 
 Disabling autoplot
 ------------------
 ``autoplot`` can be disabled by using the ``.. autoplot-disable::`` directive
 anywhere (on its own line) in a docstring.
 This will disable autoplot for the entire docstring.
-"""  # noqa: E501
+"""
 
 import re
-from typing import List, Optional
 
 from sphinx.util.docutils import SphinxDirective
 
 # If this pattern matches any line of a code block,
 # that block is assumed to produce plots.
 PLOT_PATTERN = re.compile(r'\.plot\(')
 # Pattern to detect existing plot directives.
 PLOT_DIRECTIVE_PATTERN = re.compile(r'^\s*\.\. plot::.*')
 # Pattern to detect directive to disable autoplot.
 DISABLE_DIRECTIVE_PATTERN = re.compile(r'^\s*\.\. autoplot-disable::.*')
 
 
-def _previous_nonempty_line(lines: List[str], index: int) -> Optional[str]:
+def _previous_nonempty_line(lines: list[str], index: int) -> str | None:
     index -= 1
     while index >= 0 and not lines[index].strip():
         index -= 1
     return lines[index] if index >= 0 else None
 
 
 def _indentation_of(s: str) -> int:
     return len(s) - len(s.lstrip())
 
 
-def _process_block(lines: List[str], begin: int, end: int) -> List[str]:
+def _process_block(lines: list[str], begin: int, end: int) -> list[str]:
     block = lines[begin:end]
     if PLOT_PATTERN.search(block[-1]) is not None:
         prev = _previous_nonempty_line(lines, begin)
         if prev and PLOT_DIRECTIVE_PATTERN.match(prev) is None:
             # If the block is not preceded by any text or directives (e.g. comes right
             # after the 'Examples' header), its indentation is stripped in `lines`.
             # Adding some indentation here fixes that but also modifies indentation
             # if the block is already indented. That should not cause problems.
             return [
                 ' ' * _indentation_of(prev) + '.. plot::',
                 '',
-                *map(lambda x: '    ' + x, block),
+                *('    ' + x for x in block),
             ]
     return block
 
 
 def _is_start_of_block(line: str) -> bool:
     return line.lstrip().startswith('>>>')
 
 
 def _is_part_of_block(line: str) -> bool:
     stripped = line.lstrip()
     return stripped.startswith('>>>') or stripped.startswith('...')
 
 
-def add_plot_directives(app, what, name, obj, options, lines: List[str]):
+def add_plot_directives(app, what, name, obj, options, lines: list[str]):
     new_lines = []
     block_begin = None
     for i, line in enumerate(lines):
         if DISABLE_DIRECTIVE_PATTERN.match(line):
             return
         if block_begin is None:
             if _is_start_of_block(line):
```

### Comparing `scipp-24.2.0/src/scipp/testing/assertions.py` & `scipp-24.5.0/src/scipp/testing/assertions.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,55 +7,74 @@
 Place the following code in your ``conftest.py``:
 
 .. code-block:: python
 
     pytest.register_assert_rewrite('scipp.testing.assertions')
 
 """
+
+from collections.abc import Callable, Iterator, Mapping
 from contextlib import contextmanager
-from typing import Any, Callable, Iterator, Mapping, TypeVar
+from typing import Any, TypeVar
 
 import numpy as np
 
 from ..core import DataArray, DataGroup, Dataset, Variable
 
 # Exception notes are formatted as 'PREPOSITION {loc}',
 # where 'loc' is set by the concrete assertion functions to indicate coords, attrs, etc.
 # 'PREPOSITION' is replaced at the top level to produce exception messages like:
 #
 # [...]
 # in coord 'x'
 # of data group item 'b'
 # of data group item 'a'
 
-T = TypeVar('T')
+_T = TypeVar('_T', Variable, DataArray)
 
 
 def assert_allclose(
-    a: T, b: T, rtol: Variable = None, atol: Variable = None, **kwargs
+    a: _T,
+    b: _T,
+    rtol: Variable | None = None,
+    atol: Variable | None = None,
+    **kwargs: Any,
 ) -> None:
     """Raise an AssertionError if two objects don't have similar values
     or if their other properties are not identical.
 
     Parameters
     ----------
     a:
         The actual object to check.
     b:
         The desired, expected object.
+    rtol:
+        Tolerance value relative (to b).
+        Can be a scalar or non-scalar.
+        Cannot have variances.
+        Defaults to scalar 1e-7 if unset.
+    atol:
+        Tolerance value absolute.
+        Can be a scalar or non-scalar.
+        Cannot have variances.
+        Defaults to scalar 0 if unset and takes units from y arg.
+    kwargs:
+        Additional arguments to pass to :func:`numpy.testing.assert_allclose`
+        which is used for comparing data.
 
     Raises
     ------
     AssertionError
         If the objects are not identical.
     """
     return _assert_similar(_assert_allclose_impl, a, b, rtol=rtol, atol=atol, **kwargs)
 
 
-def assert_identical(a: T, b: T) -> None:
+def assert_identical(a: _T, b: _T) -> None:
     """Raise an AssertionError if two objects are not identical.
 
     For Scipp objects, ``assert_identical(a, b)`` is equivalent to
     ``assert sc.identical(a, b, equal_nan=True)`` but produces a more precise
     error message in pytest.
     If this function is called with arguments that are not supported by
     :func:`scipp.identical`, it calls ``assert a == b``.
@@ -76,15 +95,15 @@
     ------
     AssertionError
         If the objects are not identical.
     """
     return _assert_similar(_assert_identical_impl, a, b)
 
 
-def _assert_similar(impl: Callable, *args, **kwargs) -> None:
+def _assert_similar(impl: Callable[..., None], *args: Any, **kwargs: Any) -> None:
     try:
         impl(*args, **kwargs)
     except AssertionError as exc:
         if hasattr(exc, '__notes__'):
             # See comment above.
             notes = []
             rest = -1
@@ -97,47 +116,48 @@
                 note.replace('PREPOSITION', 'of') for note in exc.__notes__[rest + 1 :]
             )
             exc.__notes__ = notes
         raise
 
 
 def _assert_identical_impl(
-    a: T,
-    b: T,
+    a: _T,
+    b: _T,
 ) -> None:
     _assert_identical_structure(a, b)
     _assert_identical_data(a, b)
 
 
 def _assert_allclose_impl(
-    a: T,
-    b: T,
-    **kwargs,
+    a: _T,
+    b: _T,
+    **kwargs: Any,
 ) -> None:
     _assert_identical_structure(a, b)
     _assert_allclose_data(a, b, **kwargs)
 
 
 def _assert_identical_structure(
-    a: T,
-    b: T,
+    a: _T,
+    b: _T,
 ) -> None:
     assert type(a) == type(b)
     if isinstance(a, Variable):
         _assert_identical_variable_structure(a, b)
     elif isinstance(a, DataArray):
         _assert_identical_data_array_structure(a, b)
 
 
 def _assert_identical_variable_structure(a: Variable, b: Variable) -> None:
     assert a.sizes == b.sizes
     assert a.unit == b.unit
     assert a.dtype == b.dtype
     assert (a.bins is None) == (b.bins is None)
     if a.bins is not None:
+        assert b.bins is not None
         assert a.bins.unit == b.bins.unit
     else:
         if a.variances is not None:
             assert b.variances is not None, 'a has variances but b does not'
         else:
             assert b.variances is None, 'a has no variances but b does'
 
@@ -161,28 +181,27 @@
         assert a.aligned == b.aligned
 
 
 def _assert_mapping_eq(
     a: Mapping[str, Any],
     b: Mapping[str, Any],
     map_name: str,
-    **kwargs,
 ) -> None:
     with _add_note(map_name + 's'):
         assert a.keys() == b.keys()
     for name, val_a in a.items():
         with _add_note("{} '{}'", map_name, name):
             val_b = b[name]
             _assert_identical_impl(val_a, val_b)
             _assert_identical_alignment(val_a, val_b)
 
 
 def _assert_identical_data(
-    a: T,
-    b: T,
+    a: _T,
+    b: _T,
 ) -> None:
     if isinstance(a, Variable):
         _assert_identical_variable_data(a, b)
     elif isinstance(a, DataArray):
         _assert_identical_variable_data(a.data, b.data)
     elif isinstance(a, Dataset):
         _assert_identical_dataset(a, b)
@@ -208,39 +227,45 @@
             with _add_note('variances'):
                 np.testing.assert_array_equal(
                     a.variances, b.variances, err_msg='when comparing variances'
                 )
 
 
 def _assert_identical_binned_variable_data(a: Variable, b: Variable) -> None:
+    assert a.bins is not None
+    assert b.bins is not None
     _assert_identical_impl(a.bins.concat().value, b.bins.concat().value)
 
 
 def _assert_allclose_data(
-    a: T,
-    b: T,
-    **kwargs,
+    a: _T,
+    b: _T,
+    **kwargs: Any,
 ) -> None:
     if isinstance(a, Variable):
         _assert_allclose_variable_data(a, b, **kwargs)
     elif isinstance(a, DataArray):
         _assert_allclose_variable_data(a.data, b.data, **kwargs)
     else:
         raise NotImplementedError
 
 
-def _assert_allclose_variable_data(a: Variable, b: Variable, **kwargs) -> None:
+def _assert_allclose_variable_data(a: Variable, b: Variable, **kwargs: Any) -> None:
     if a.bins is None:
         _assert_allclose_dense_variable_data(a, b, **kwargs)
     else:
         _assert_allclose_binned_variable_data(a, b, **kwargs)
 
 
 def _assert_allclose_dense_variable_data(
-    a: Variable, b: Variable, rtol: Variable = None, atol: Variable = None, **kwargs
+    a: Variable,
+    b: Variable,
+    rtol: Variable | None = None,
+    atol: Variable | None = None,
+    **kwargs: Any,
 ) -> None:
     if rtol is not None:
         kwargs['rtol'] = rtol.to(unit='dimensionless').value
     if atol is not None:
         if hasattr(a, 'unit'):
             atol = atol.to(unit=a.unit)
         else:
@@ -258,16 +283,18 @@
                     b.variances,
                     err_msg='when comparing variances',
                     **kwargs,
                 )
 
 
 def _assert_allclose_binned_variable_data(
-    a: Variable, b: Variable, rtol: Variable, atol: Variable, **kwargs
+    a: Variable, b: Variable, **kwargs: Any
 ) -> None:
+    assert a.bins is not None
+    assert b.bins is not None
     _assert_allclose_impl(a.bins.concat().value, b.bins.concat().value, **kwargs)
 
 
 @contextmanager
 def _add_note(loc: str, *args: str) -> Iterator[None]:
     try:
         yield
```

### Comparing `scipp-24.2.0/src/scipp/testing/strategies.py` & `scipp-24.5.0/src/scipp/testing/strategies.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Jan-Lukas Wynen
 """
 Search strategies for hypothesis to generate inputs for tests.
 """
 
+from collections.abc import Callable, Sequence
 from functools import partial
-from typing import Any, Callable, Dict, Optional, Sequence, Union
+from typing import Any
 
 import numpy as np
 from hypothesis import strategies as st
-from hypothesis.core import Ex
+from hypothesis.core import Ex  # type: ignore[attr-defined]
 from hypothesis.errors import InvalidArgument
 from hypothesis.extra import numpy as npst
 
 from ..core import DataArray, DType, Unit, Variable
 from ..core import variable as creation
 
 
@@ -28,15 +29,15 @@
         ),
         min_size=0,
         max_size=50,
     )
 
 
 def sizes_dicts(
-    ndim: Optional[Union[int, st.SearchStrategy]] = None
+    ndim: int | st.SearchStrategy | None = None,
 ) -> st.SearchStrategy:
     if isinstance(ndim, st.SearchStrategy):
         return ndim.flatmap(lambda n: sizes_dicts(ndim=n))
     keys = dims()
     values = st.integers(min_value=1, max_value=10)
     if ndim is None:
         # The constructor of sc.Variable in Python only supports
@@ -57,16 +58,16 @@
     return st.sampled_from([f'float{size}' for size in sizes])
 
 
 def scalar_numeric_dtypes() -> st.SearchStrategy:
     return st.sampled_from((integer_dtypes, floating_dtypes)).flatmap(lambda f: f())
 
 
-def _variables_from_fixed_args(args: dict) -> st.SearchStrategy:
-    def make_array(variances: bool):
+def _variables_from_fixed_args(args: dict[str, Any]) -> st.SearchStrategy:
+    def make_array(variances: bool) -> st.SearchStrategy:
         elements = args['elements']
         if elements is None and variances:
             # Make sure that variances are non-negative and
             # let the user decide otherwise.
             elements = st.floats(
                 min_value=0.0, width=32 if np.dtype(args['dtype']) == np.float32 else 64
             )
@@ -83,45 +84,50 @@
         partial(creation.array, dims=list(args['sizes'].keys()), unit=args['unit']),
         values=make_array(False),
         variances=make_array(True) if args['with_variances'] else st.none(),
     )
 
 
 class _ConditionallyWithVariances:
-    def __init__(self):
+    def __init__(self) -> None:
         self._strategy = st.booleans()
 
-    def __call__(self, draw, dtype) -> bool:
+    def __call__(self, draw: st.DrawFn, dtype: DType) -> bool:
         if dtype in (DType.float32, DType.float64):
             return draw(self._strategy)
         return False
 
 
 @st.composite
-def _concrete_args(draw, args: dict) -> dict:
-    def _draw(x):
-        return draw(x) if isinstance(x, st.SearchStrategy) else x
+def _concrete_args(
+    draw: st.DrawFn, args: dict[str, st.SearchStrategy | Any]
+) -> dict[str, Any]:
+    def _draw(x: st.SearchStrategy[Ex] | Ex) -> Ex:
+        return draw(x) if isinstance(x, st.SearchStrategy) else x  # type:ignore[no-any-return]
 
     concrete = {key: _draw(val) for key, val in args.items()}
     if isinstance(concrete['with_variances'], _ConditionallyWithVariances):
         concrete['with_variances'] = concrete['with_variances'](draw, concrete['dtype'])
     return concrete
 
 
 def _variable_arg_strategies(
     *,
-    ndim: Union[int, st.SearchStrategy, None] = None,
-    sizes: Union[Dict[str, int], st.SearchStrategy, None] = None,
-    unit: Union[str, Unit, st.SearchStrategy, None] = None,
-    dtype: Union[str, DType, type, st.SearchStrategy, None] = None,
-    with_variances: Union[bool, st.SearchStrategy, None] = None,
-    elements: Union[int, float, st.SearchStrategy, None] = None,
-    fill: Union[int, float, st.SearchStrategy, None] = None,
-    unique: Union[bool, st.SearchStrategy, None] = None,
-):
+    ndim: int | st.SearchStrategy | None = None,
+    sizes: dict[str, int] | st.SearchStrategy | None = None,
+    unit: str | Unit | st.SearchStrategy | None = None,
+    dtype: str | DType | type | st.SearchStrategy | None = None,
+    with_variances: bool
+    | st.SearchStrategy
+    | _ConditionallyWithVariances
+    | None = None,
+    elements: float | st.SearchStrategy | None = None,
+    fill: float | st.SearchStrategy | None = None,
+    unique: bool | st.SearchStrategy | None = None,
+) -> dict[str, st.SearchStrategy | Any]:
     if ndim is not None:
         if sizes is not None:
             raise InvalidArgument(
                 'Arguments `ndim` and `sizes` cannot both be used. '
                 f'Got {ndim=}, {sizes=}.'
             )
     if sizes is None:
@@ -129,43 +135,43 @@
     if unit is None:
         unit = units()
     if dtype is None:
         # TODO other dtypes?
         dtype = scalar_numeric_dtypes()
     if with_variances is None:
         with_variances = _ConditionallyWithVariances()
-    return dict(
-        sizes=sizes,
-        unit=unit,
-        dtype=dtype,
-        with_variances=with_variances,
-        elements=elements,
-        fill=fill,
-        unique=unique,
-    )
+    return {
+        'sizes': sizes,
+        'unit': unit,
+        'dtype': dtype,
+        'with_variances': with_variances,
+        'elements': elements,
+        'fill': fill,
+        'unique': unique,
+    }
 
 
 # This implementation is designed such that the individual strategies
 # for default arguments are constructed only once, namely when
 # `variables` is called. Sampling via `_concrete_args` then reuses
 # those strategies.
 # A previous implementation constructed those component strategies inside
 # an `st.composite` function for every example drawn. This led to high
 # memory consumption by hypothesis and failed
 # `hypothesis.HealthCheck.data_too_large`.
 def variables(
     *,
-    ndim: Union[int, st.SearchStrategy, None] = None,
-    sizes: Union[Dict[str, int], st.SearchStrategy, None] = None,
-    unit: Union[str, Unit, st.SearchStrategy, None] = None,
-    dtype: Union[str, DType, type, st.SearchStrategy, None] = None,
-    with_variances: Union[bool, st.SearchStrategy, None] = None,
-    elements: Union[int, float, st.SearchStrategy, None] = None,
-    fill: Union[int, float, st.SearchStrategy, None] = None,
-    unique: Union[bool, st.SearchStrategy, None] = None,
+    ndim: int | st.SearchStrategy | None = None,
+    sizes: dict[str, int] | st.SearchStrategy | None = None,
+    unit: str | Unit | st.SearchStrategy | None = None,
+    dtype: str | DType | type | st.SearchStrategy | None = None,
+    with_variances: bool | st.SearchStrategy | None = None,
+    elements: float | st.SearchStrategy | None = None,
+    fill: float | st.SearchStrategy | None = None,
+    unique: bool | st.SearchStrategy | None = None,
 ) -> st.SearchStrategy[Variable]:
     args = _variable_arg_strategies(
         ndim=ndim,
         sizes=sizes,
         unit=unit,
         dtype=dtype,
         with_variances=with_variances,
@@ -175,22 +181,22 @@
     )
     return _concrete_args(args).flatmap(_variables_from_fixed_args)
 
 
 def n_variables(
     n: int,
     *,
-    ndim: Union[int, st.SearchStrategy, None] = None,
-    sizes: Union[Dict[str, int], st.SearchStrategy, None] = None,
-    unit: Union[str, Unit, st.SearchStrategy, None] = None,
-    dtype: Union[str, DType, type, st.SearchStrategy, None] = None,
-    with_variances: Union[bool, st.SearchStrategy, None] = None,
-    elements: Union[int, float, st.SearchStrategy, None] = None,
-    fill: Union[int, float, st.SearchStrategy, None] = None,
-    unique: Union[bool, st.SearchStrategy, None] = None,
+    ndim: int | st.SearchStrategy | None = None,
+    sizes: dict[str, int] | st.SearchStrategy | None = None,
+    unit: str | Unit | st.SearchStrategy | None = None,
+    dtype: str | DType | type | st.SearchStrategy | None = None,
+    with_variances: bool | st.SearchStrategy | None = None,
+    elements: float | st.SearchStrategy | None = None,
+    fill: float | st.SearchStrategy | None = None,
+    unique: bool | st.SearchStrategy | None = None,
 ) -> st.SearchStrategy[tuple[Variable]]:
     args = _variable_arg_strategies(
         ndim=ndim,
         sizes=sizes,
         unit=unit,
         dtype=dtype,
         with_variances=with_variances,
@@ -204,63 +210,63 @@
 
 
 @st.composite
 def coord_dicts(
     draw: Callable[[st.SearchStrategy[Ex]], Ex],
     *,
     sizes: dict[str, int],
-    args: Optional[dict[str, Any]] = None,
+    args: dict[str, Any] | None = None,
     bin_edges: bool = True,
 ) -> dict[str, Variable]:
     args = args or {}
     args['sizes'] = sizes
     try:
         del args['ndim']
     except KeyError:
         pass
 
     if bin_edges:
 
-        def size_increment():
-            return draw(st.integers(min_value=0, max_value=1))
+        def size_increment() -> int:
+            return draw(st.integers(min_value=0, max_value=1))  # type:ignore[arg-type, return-value]
 
     else:
 
-        def size_increment():
+        def size_increment() -> int:
             return 0
 
     if not sizes:
         return {}
 
-    names_and_sizes = draw(
-        st.lists(
+    names_and_sizes: list[tuple[Any, tuple[str, int]]] = draw(  # type: ignore[assignment]
+        st.lists(  # type: ignore[arg-type]
             st.sampled_from(list(sizes))
             .map(lambda dim: (dim, sizes[dim] + size_increment()))
             .flatmap(
                 lambda item: (st.just(item[0]) | dims()).map(lambda name: (name, item))
             ),
             min_size=0,
             max_size=6,
         )
     )
     return {
-        name: draw(variables(**{**args, 'sizes': {dim: size}}))
+        name: draw(variables(**{**args, 'sizes': {dim: size}}))  # type: ignore[arg-type, misc]
         for name, (dim, size) in names_and_sizes
     }
 
 
 @st.composite
 def dataarrays(
     draw: Callable[[st.SearchStrategy[Ex]], Ex],
     *,
-    data_args: Optional[dict[str, Any]] = None,
+    data_args: dict[str, Any] | None = None,
     coords: bool = True,
-    coord_args: Optional[dict[str, Any]] = None,
+    coord_args: dict[str, Any] | None = None,
     masks: bool = True,
-    mask_args: Optional[dict[str, Any]] = None,
+    mask_args: dict[str, Any] | None = None,
     bin_edges: bool = True,
 ) -> DataArray:
     """Generate data arrays with coords and masks.
 
     The data variable can be any variable supported by
     ``scipp.testing.strategies.variables``.
     The coordinates and masks are constrained to be one-dimensional where the
@@ -286,27 +292,29 @@
         If ``True``, coords may be bin edges.
 
     See Also
     --------
     scipp.testing.strategies.variables:
         For allowed items in ``*_args`` dicts.
     """
-    data = draw(variables(**(data_args or {})))
-    if coords:
-        coords_dict = draw(
-            coord_dicts(sizes=data.sizes, args=coord_args, bin_edges=bin_edges)
+    data: Variable = draw(variables(**(data_args or {})))  # type: ignore[arg-type, assignment]
+
+    coords_dict: dict[str, Variable] = (
+        draw(  # type: ignore[assignment]
+            coord_dicts(sizes=data.sizes, args=coord_args, bin_edges=bin_edges)  # type: ignore[arg-type]
         )
-    else:
-        coords_dict = {}
+        if coords
+        else {}
+    )
 
     if masks:
         mask_args = mask_args or {}
         mask_args['dtype'] = bool
-        masks_dict = draw(
-            coord_dicts(sizes=data.sizes, args=mask_args, bin_edges=False)
+        masks_dict: dict[str, Variable] = draw(  # type: ignore[assignment]
+            coord_dicts(sizes=data.sizes, args=mask_args, bin_edges=False)  # type: ignore[arg-type]
         )
     else:
         masks_dict = {}
 
     return DataArray(
         data,
         coords=coords_dict,
```

### Comparing `scipp-24.2.0/src/scipp/typing.py` & `scipp-24.5.0/src/scipp/typing.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,72 +44,72 @@
 def has_numeric_type(obj: _std_typing.Any) -> bool:
     """
     Return False if the dtype is either vector or string.
     """
     return (not has_vector_type(obj)) and (not has_string_type(obj))
 
 
-Dims = _std_typing.Union[None, str, _std_typing.Sequence[str]]
+Dims: _std_typing.TypeAlias = str | _std_typing.Sequence[str] | None
 """
 Describes dimensions to operate on.
 
 Can be a string (for a single dimension) or a sequence of strings (multiple dimensions).
 A value of ``None`` indicates "all dimensions."
 """
 
-VariableLike = _std_typing.Union[Variable, DataArray, Dataset, DataGroup]
+VariableLike: _std_typing.TypeAlias = Variable | DataArray | Dataset | DataGroup
 """Any object that behaves like a :class:`scipp.Variable`.
 
 More concretely, an array with labeled dimensions which supports slicing and
 arithmetic:
 
 - :class:`scipp.DataArray`
 - :class:`scipp.DataGroup`
 - :class:`scipp.Dataset`
 - :class:`scipp.Variable`
 """
 
-MetaDataMap = _std_typing.MutableMapping[str, Variable]
+MetaDataMap: _std_typing.TypeAlias = _std_typing.MutableMapping[str, Variable]
 """dict-like object mapping dimension labels to Variables."""
 
 VariableLikeType = _std_typing.TypeVar(
-    'VariableLikeType', Variable, DataArray, Dataset, DataGroup
+    'VariableLikeType', bound=Variable | DataArray | Dataset | DataGroup
 )
 """TypeVar for use in annotations.
 
 Should be hidden in rendered documentation in favor of VariableLike.
 """
 
-DTypeLike = _std_typing.Union[numpy.typing.DTypeLike, DType]
+DTypeLike: _std_typing.TypeAlias = numpy.typing.DTypeLike | DType
 """Anything that can be interpreted as a dtype.
 
 This includes
 
 - :class:`scipp.DType`
 - everything that is supported by
   `numpy.DTypeLike <https://numpy.org/devdocs/reference/typing.html#numpy.typing.DTypeLike>`_
   e.g.
 
   - :class:`numpy.dtype`
   - :class:`type` objects like :class:`int` and :class:`float`
   - names of dtypes as strings like ``'int32'`` and ``'float64'``
-"""  # noqa: E501
+"""
 
 if _std_typing.TYPE_CHECKING:
     from enum import Enum
 
     class ellipsis(Enum):
         Ellipsis = "..."
 
 else:
     ellipsis = type(Ellipsis)
 
-ScippIndex = _std_typing.Union[
-    ellipsis,
-    int,
-    tuple,
-    slice,
-    list,
-    np.ndarray,
-    _std_typing.Tuple[str, _std_typing.Union[int, slice, list, np.ndarray, Variable]],
-    Variable,
-]
+ScippIndex: _std_typing.TypeAlias = (
+    ellipsis
+    | int
+    | tuple
+    | slice
+    | list
+    | np.ndarray
+    | tuple[str, int | slice | list | np.ndarray | Variable]
+    | Variable
+)
```

### Comparing `scipp-24.2.0/src/scipp/units/__init__.py` & `scipp-24.5.0/src/scipp/units/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 Special:
  - default_unit (used by some functions to deduce a unit)
 
 .. seealso::
     :py:class:`scipp.Unit` to construct other units.
 """
 
+from collections.abc import Iterator
 from contextlib import contextmanager
-from typing import Dict, Iterable, Tuple, Union
 
 from .._scipp.core import add_unit_alias as _add_unit_alias
 from .._scipp.core import clear_unit_aliases as _clear_unit_aliases
-from .._scipp.core.units import (  # NOQA
+from .._scipp.core.units import (
     K,
     angstrom,
     counts,
     default_unit,
     deg,
     dimensionless,
     kg,
@@ -48,15 +48,15 @@
     mm,
     ns,
     one,
     rad,
     s,
     us,
 )
-from ..core.cpp_classes import Unit, Variable, VariancesError
+from ..core.cpp_classes import DefaultUnit, Unit, Variable, VariancesError
 
 
 class UnitAliases:
     """Manager for unit aliases.
 
     Aliases override how units are converted to and from strings.
     The table is similar to a :class:`dict` and maps alias names to units.
@@ -67,19 +67,19 @@
     Attention
     ---------
     This class is a singleton and should never be instantiated by user code.
     Instead, use it through :attr:`scipp.units.aliases`.
     """
 
     def __init__(self):
-        if any(map(lambda x: isinstance(x, UnitAliases), globals().values())):
+        if any(isinstance(x, UnitAliases) for x in globals().values()):
             raise RuntimeError('There can be only one instance of _Aliases')
-        self._aliases: Dict[str, Unit] = {}
+        self._aliases: dict[str, Unit] = {}
 
-    def __setitem__(self, alias: str, unit: Union[str, Unit, Variable]):
+    def __setitem__(self, alias: str, unit: str | Unit | Variable):
         """Define a new unit alias."""
         unit = _build_unit(unit)
         if self._aliases.get(alias) == unit:
             return
         if unit in self.values():
             raise ValueError(f"There already is an alias for unit '{unit!r}'")
         _add_unit_alias(name=alias, unit=unit)
@@ -99,15 +99,15 @@
 
     def clear(self):
         """Remove all aliases."""
         self._aliases.clear()
         _clear_unit_aliases()
 
     @contextmanager
-    def scoped(self, **kwargs: Union[str, Unit]):
+    def scoped(self, **kwargs: str | Unit):
         """Contextmanager to define temporary aliases.
 
         Defines new aliases based on ``kwargs`` for the duration of the context.
         When exiting the context, all temporary aliases are removed.
 
         It is possible to define additional aliases in the context.
         They are not removed when the context manager exits unless they override
@@ -169,40 +169,40 @@
         for name, unit in kwargs.items():
             self[name] = unit
         yield
         self._del_aliases(*kwargs)
         for name, unit in overridden.items():
             self[name] = unit
 
-    def __iter__(self) -> Iterable[str]:
+    def __iter__(self) -> Iterator[str]:
         """Iterator over alias names."""
         yield from self.keys()
 
-    def keys(self) -> Iterable[str]:
+    def keys(self) -> Iterator[str]:
         """Iterator over alias names."""
         yield from self._aliases.keys()
 
-    def values(self) -> Iterable[Unit]:
+    def values(self) -> Iterator[Unit]:
         """Iterator over aliased units."""
         yield from self._aliases.values()
 
-    def items(self) -> Iterable[Tuple[str, Unit]]:
+    def items(self) -> Iterator[tuple[str, Unit]]:
         """Iterator over pairs of alias names and units."""
         yield from self._aliases.items()
 
     # Making copies would allow _Alias's internal map and
     # LLNL/Unit's global map to get out of sync.
     def __copy__(self):
         raise TypeError('UnitAliases is a singleton and must not be copied')
 
     def __deepcopy__(self):
         raise TypeError('UnitAliases is a singleton and must not be copied')
 
 
-def _build_unit(x: Union[str, Unit, Variable]) -> Unit:
+def _build_unit(x: str | Unit | Variable) -> Unit:
     if isinstance(x, Unit):
         return x
     if isinstance(x, str):
         return Unit(x)
     if x.variance is not None:
         raise VariancesError('Cannot define a unit with a variance')
     # Convert to float first to make sure the variable only contains a
@@ -210,14 +210,15 @@
     return Unit(str(float(x.value))) * x.unit
 
 
 aliases = UnitAliases()
 """Table of unit aliases."""
 
 __all__ = [
+    'DefaultUnit',
     'angstrom',
     'counts',
     'default_unit',
     'deg',
     'dimensionless',
     'kg',
     'K',
```

### Comparing `scipp-24.2.0/src/scipp/utils/collapse_and_slices.py` & `scipp-24.5.0/src/scipp/utils/collapse_and_slices.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,26 @@
 
 # Other imports
 import numpy as np
 
 
 def _to_slices(scipp_obj, slice_dims, slice_shape, volume):
     # Create container to collect all 1D slices as 1D variables
-    all_slices = dict()
+    all_slices = {}
 
     # Go through the dims that need to be collapsed, and create an array that
     # holds the range of indices for each dimension
     # Say we have [Y, 5], and [Z, 3], then dim_list will contain
     # [[0, 1, 2, 3, 4], [0, 1, 2]]
-    dim_list = []
-    for dim in slice_dims:
-        dim_list.append(np.arange(slice_shape[dim], dtype=np.int32))
+    dim_list = [np.arange(slice_shape[dim], dtype=np.int32) for dim in slice_dims]
     # Next create a grid of indices
     # grid will contain
     # [ [[0, 1, 2, 3, 4], [0, 1, 2, 3, 4], [0, 1, 2, 3, 4]],
     #   [[0, 0, 0, 0, 0], [1, 1, 1, 1, 1], [2, 2, 2, 2, 2]] ]
-    grid = np.meshgrid(*[x for x in dim_list])
+    grid = np.meshgrid(*list(dim_list))
     # Reshape the grid to have a 2D array of length volume, i.e.
     # [ [0, 1, 2, 3, 4, 0, 1, 2, 3, 4, 0, 1, 2, 3, 4],
     #   [0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 2, 2, 2, 2, 2] ]
     res = np.reshape(grid, (len(slice_dims), volume))
     # Now make a master array which also includes the dimension labels, i.e.
     # [ [Y, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y],
     #   [0, 1, 2, 3, 4, 0, 1, 2, 3, 4, 0, 1, 2, 3, 4],
@@ -50,15 +48,15 @@
 
     # Extract each entry from the slice_list
     for line in slice_list:
         vslice = scipp_obj
         key = ""
         for s in line:
             vslice = vslice[s[0], s[1]]
-            key += "{}:{}-".format(str(s[0]), s[1])
+            key += f"{s[0]}:{s[1]}-"
         all_slices[key[:-1]] = vslice
 
     return all_slices
 
 
 def collapse(scipp_obj, keep):
     """
@@ -79,16 +77,16 @@
 
     dims = scipp_obj.dims
     shape = scipp_obj.shape
 
     # Gather list of dimensions that are to be collapsed
     slice_dims = []
     volume = 1
-    slice_shape = dict()
-    for d, size in zip(dims, shape):
+    slice_shape = {}
+    for d, size in zip(dims, shape, strict=True):
         if d != keep:
             slice_dims.append(d)
             slice_shape[d] = size
             volume *= size
 
     return _to_slices(scipp_obj, slice_dims, slice_shape, volume)
```

### Comparing `scipp-24.2.0/src/scipp/utils/comparison.py` & `scipp-24.5.0/src/scipp/utils/comparison.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Owen Arnold
 """
 Advanced comparisons.
 """
-from typing import Optional
 
 from ..core import CoordError, DataArray, DType, Variable, all, isclose
 
 
 def isnear(
     x: DataArray,
     y: DataArray,
-    rtol: Optional[Variable] = None,
-    atol: Optional[Variable] = None,
+    rtol: Variable | None = None,
+    atol: Variable | None = None,
     include_attrs: bool = True,
     include_data: bool = True,
     equal_nan: bool = True,
 ) -> bool:
     """
     Similar to scipp.isclose, but intended to compare whole DataArrays.
     Coordinates compared element by element with
```

### Comparing `scipp-24.2.0/src/scipp/utils/profile.py` & `scipp-24.5.0/src/scipp/utils/profile.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/src/scipp/utils/pyshell.py` & `scipp-24.5.0/src/scipp/utils/pyshell.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/src/scipp/utils/to_string.py` & `scipp-24.5.0/src/scipp/utils/to_string.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,11 +34,11 @@
         else:
             text = raw_text
     elif (abs(val) >= 10.0 ** (precision + 1)) or (
         abs(val) <= 10.0 ** (-precision - 1)
     ):
         text = "{val:.{prec}e}".format(val=val, prec=precision)
     else:
-        text = "{}".format(val)
+        text = f"{val}"
         if len(text) > precision + 2 + (text[0] == '-'):
             text = "{val:.{prec}f}".format(val=val, prec=precision)
     return text
```

### Comparing `scipp-24.2.0/src/scipp/visualization/colors.py` & `scipp-24.5.0/src/scipp/visualization/colors.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 def rgb_to_hex(rgb):
     hex_value = []
     for i in rgb:
         h = hex(int(i))[2:]
         if len(h) < 2:
-            h = "{}0".format(h)
+            h = f"{h}0"
         hex_value.append(h)
     return "#" + "".join(hex_value)
 
 
 def make_random_color(fmt='rgb'):
     """
     Generate a random color.
@@ -44,10 +44,10 @@
         return rgb.astype(np.float) / 255.0
     elif fmt == 'rgba':
         return np.concatenate((rgb.astype(np.float) / 255.0, [1.0]))
     elif fmt == 'hex':
         return rgb_to_hex(rgb)
     else:
         raise RuntimeError(
-            "Unknown color format {}. Possible choices are: "
-            "rgb, dec, rgba, and hex.".format(fmt)
+            f"Unknown color format {fmt}. Possible choices are: "
+            "rgb, dec, rgba, and hex."
         )
```

### Comparing `scipp-24.2.0/src/scipp/visualization/formatting_datagroup_html.py` & `scipp-24.5.0/src/scipp/visualization/formatting_datagroup_html.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import uuid
 from string import Template
-from typing import Union
 
 import numpy as np
 
 from ..core.cpp_classes import DataArray, Dataset, Variable
 from ..core.data_group import DataGroup
 from ..units import dimensionless
 from .formatting_html import escape, inline_variable_repr
@@ -16,15 +15,15 @@
     load_collapsible_row_tpl,
     load_dg_detail_list_tpl,
     load_dg_repr_tpl,
     load_dg_style,
 )
 
 
-def _format_shape(var: Union[Variable, DataArray, Dataset, DataGroup], br_at=30) -> str:
+def _format_shape(var: Variable | DataArray | Dataset | DataGroup, br_at=30) -> str:
     """Return HTML Component that represents the shape of ``var``"""
     shape_list = [f"{escape(str(dim))}: {size}" for dim, size in var.sizes.items()]
     if sum([len(line) - line.count('\\') for line in shape_list]) < br_at:
         return f"({', '.join(shape_list)})"
     else:
         return f"({', <br>&nbsp'.join(shape_list)})"
 
@@ -41,15 +40,15 @@
     """Inline preview of a dictionary"""
     name, item = name_item
     name = _format_atomic_value(name, maxidx=maxidx)
     type_repr = _format_atomic_value(type(item).__name__, maxidx=maxidx)
     return "(" + ": ".join((name, type_repr)) + ")"
 
 
-def _format_multi_dim_data(var: Union[Dataset, np.ndarray]) -> str:
+def _format_multi_dim_data(var: Dataset | np.ndarray) -> str:
     """Inline preview of single or multi-dimensional data"""
     if isinstance(var, Dataset):
         view_iterable = list(var.items())
         var_len = len(var)
         first_idx, last_idx = 0, -1
         format_item = _format_dictionary_item
     elif isinstance(var, np.ndarray):
@@ -74,22 +73,22 @@
     """Return HTML Component that contains summary of ``var``"""
     shape_repr = escape("()")
     unit = ''
     dtype_str = ''
     preview = ''
     parent_obj_str = ''
     objtype_str = type(var).__name__
-    if isinstance(var, (Dataset, DataArray, Variable)):
+    if isinstance(var, Dataset | DataArray | Variable):
         parent_obj_str = "scipp"
         shape_repr = _format_shape(var)
-    if isinstance(var, (DataArray, Variable)):
+    if isinstance(var, DataArray | Variable):
         preview = inline_variable_repr(var)
         dtype_str = str(var.dtype)
         if var.unit is not None:
-            unit = '𝟙' if var.unit == dimensionless else str(var.unit)
+            unit = '𝟙' if var.unit == dimensionless else str(var.unit)  # noqa: RUF001
     elif isinstance(var, Dataset):
         preview = escape(_format_multi_dim_data(var))
     elif isinstance(var, np.ndarray):
         parent_obj_str = "numpy"
         preview = f"shape={var.shape}, dtype={var.dtype}, values="
         preview += escape(_format_multi_dim_data(var))
 
@@ -111,30 +110,30 @@
 
 def _collapsible_summary(var: DataGroup, name: str, name_spaces: list) -> str:
     parent_type = "scipp"
     objtype = type(var).__name__
     shape_repr = _format_shape(var)
     checkbox_id = escape("summary-" + str(uuid.uuid4()))
     depth = len(name_spaces)
-    subsection = _datagroup_detail(var, name_spaces + [name])
+    subsection = _datagroup_detail(var, [*name_spaces, name])
     html_tpl = load_collapsible_row_tpl()
 
     return Template(html_tpl).substitute(
         name=escape(str(name)),
         parent=escape(parent_type),
         objtype=escape(objtype),
         shape_repr=shape_repr,
         summary_section_id=checkbox_id,
         depth=depth,
         checkbox_status='',
         subsection=subsection,
     )
 
 
-def _datagroup_detail(dg: DataGroup, name_spaces: list = None) -> str:
+def _datagroup_detail(dg: DataGroup, name_spaces: list | None = None) -> str:
     if name_spaces is None:
         name_spaces = []
     summary_rows = []
     for name, item in dg.items():
         if isinstance(item, DataGroup):
             collapsible_row = _collapsible_summary(item, name, name_spaces)
             summary_rows.append(collapsible_row)
@@ -145,15 +144,15 @@
 
     dg_detail_tpl = Template(load_dg_detail_list_tpl())
     return dg_detail_tpl.substitute(summary_rows=''.join(summary_rows))
 
 
 def datagroup_repr(dg: DataGroup) -> str:
     """Return HTML Component containing details of ``dg``"""
-    obj_type = "scipp.{} ".format(type(dg).__name__)
+    obj_type = f"scipp.{type(dg).__name__} "
     checkbox_status = "checked" if len(dg) < 15 else ''
     header_id = "datagroup-view-" + str(uuid.uuid4())
     details = _datagroup_detail(dg)
     html = Template(load_dg_repr_tpl())
     return html.substitute(
         style_sheet=load_dg_style(),
         header_id=header_id,
```

### Comparing `scipp-24.2.0/src/scipp/visualization/formatting_html.py` & `scipp-24.5.0/src/scipp/visualization/formatting_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from .._scipp import core as sc
 from ..core import stddevs
 from ..utils import value_to_string
 from .resources import load_icons, load_style
 
 BIN_EDGE_LABEL = "[bin-edge]"
-STDDEV_PREFIX = "σ = "
+STDDEV_PREFIX = "σ = "  # noqa: RUF001
 VARIANCES_SYMBOL = "σ²"
 SPARSE_PREFIX = "len={}"
 
 
 def escape(content: str) -> str:
     """
     Escape dollar-sign($) as well as html special characters.
@@ -77,17 +77,17 @@
     shape = item.shape[bin_dim]
     return SPARSE_PREFIX.format(shape)
 
 
 def _get_events(var, variances, ellipsis_after):
     dim = var.bins.constituents['dim']
     dims = var.bins.constituents['data'].dims
-    bin_dim = dict(zip(dims, range(len(dims))))[dim]
+    bin_dim = dict(zip(dims, range(len(dims)), strict=True))[dim]
     s = []
-    if not isinstance(var.values, (sc.Variable, sc.DataArray, sc.Dataset)):
+    if not isinstance(var.values, sc.Variable | sc.DataArray | sc.Dataset):
         size = len(var.values)
         i = 0
 
         data = retrieve(var, variances=variances)
         while i < size:
             if i == ellipsis_after and size > 2 * ellipsis_after + 1:
                 s.append("...")
@@ -103,15 +103,15 @@
             )
         )
     return s
 
 
 def _format_events(var, has_variances):
     s = _get_events(var, has_variances, ellipsis_after=2)
-    return f'binned data [{", ".join([row for row in s])}]'
+    return f'binned data [{", ".join(s)}]'
 
 
 def _ordered_dict(data):
     data_ordered = collections.OrderedDict(
         sorted(data.items(), key=lambda t: str(t[0]))
     )
     return data_ordered
@@ -164,27 +164,24 @@
         dim: " class='sc-has-index'" if dim in coords else "" for dim in dims
     }
 
     dims_li = "".join(
         f"<li><span{dim_css_map[dim]}>"
         f"{escape(str(dim))}</span>: "
         f"{size if size is not None else 'Events' }</li>"
-        for dim, size in zip(dims, sizes)
+        for dim, size in zip(dims, sizes, strict=True)
     )
 
     return f"<ul class='sc-dim-list'>{dims_li}</ul>"
 
 
 def _icon(icon_name):
     # icon_name is defined in icon-svg-inline.html
     return (
-        "<svg class='icon sc-{0}'>"
-        "<use xlink:href='#{0}'>"
-        "</use>"
-        "</svg>".format(icon_name)
+        f"<svg class='icon sc-{icon_name}'><use xlink:href='#{icon_name}'></use></svg>"
     )
 
 
 def summarize_coord(dim, var, ds=None):
     return summarize_variable(str(dim), var, is_aligned=var.aligned, embedded_in=ds)
 
 
@@ -275,15 +272,15 @@
 def _make_dim_str(var, bin_edges, add_dim_size=False):
     dims_text = ', '.join(
         '{}{}{}'.format(
             str(dim),
             _make_dim_labels(dim, bin_edges),
             f': {size}' if add_dim_size and size is not None else '',
         )
-        for dim, size in zip(var.dims, var.shape)
+        for dim, size in zip(var.dims, var.shape, strict=True)
     )
     return dims_text
 
 
 def _format_common(is_index):
     cssclass_aligned = " class='sc-aligned'" if is_index else ""
 
@@ -310,15 +307,15 @@
             _find_bin_edges(var, embedded_in) if embedded_in is not None else None,
             add_dim_size,
         )
     )
     if var.unit is None:
         unit = ''
     else:
-        unit = '𝟙' if var.unit == sc.units.dimensionless else str(var.unit)
+        unit = '𝟙' if var.unit == sc.units.dimensionless else str(var.unit)  # noqa: RUF001
 
     disabled, attrs_ul = _make_inline_attributes(var, has_attrs, embedded_in)
 
     preview = _make_row(inline_variable_repr(var))
     data_repr = short_data_repr_html(var)
     if var.bins is None:
         data_repr = "Values:<br>" + data_repr
@@ -420,15 +417,15 @@
         n_items=n_items,
         enabled=enabled,
         collapsed=collapsed,
     )
 
 
 def dim_section(dataset):
-    coords = dataset.coords if hasattr(dataset, "coords") else dict()
+    coords = dataset.coords if hasattr(dataset, "coords") else {}
     dim_list = format_dims(dataset.dims, dataset.shape, coords)
 
     return collapsible_section(
         "Dimensions", inline_details=dim_list, enabled=False, collapsed=True
     )
 
 
@@ -495,15 +492,15 @@
             " <span class='sc-underlying-size'>out of "
             f"{human_readable_size(underlying_size)}</span>"
         )
     return res + ")"
 
 
 def dataset_repr(ds):
-    obj_type = "scipp.{}".format(type(ds).__name__)
+    obj_type = f"scipp.{type(ds).__name__}"
     header_components = [
         f"<div class='sc-obj-type'>{escape(obj_type)} " + _format_size(ds) + "</div>"
     ]
 
     sections = [dim_section(ds)]
 
     if len(ds.coords) > 0:
@@ -517,15 +514,15 @@
         if len(ds.deprecated_attrs) > 0:
             sections.append(attr_section(ds.deprecated_attrs, ds))
 
     return _obj_repr(header_components, sections)
 
 
 def variable_repr(var):
-    obj_type = "scipp.{}".format(type(var).__name__)
+    obj_type = f"scipp.{type(var).__name__}"
 
     header_components = [
         f"<div class='sc-obj-type'>{escape(obj_type)} " + _format_size(var) + "</div>"
     ]
 
     sections = [variable_section(var)]
```

### Comparing `scipp-24.2.0/src/scipp/visualization/html.py` & `scipp-24.5.0/src/scipp/visualization/html.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/src/scipp/visualization/resources.py` & `scipp-24.5.0/src/scipp/visualization/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from functools import lru_cache, partial
 
 
 def _read_text(filename):
     return (
         importlib.resources.files('scipp.visualization.templates')
         .joinpath(filename)
-        .read_text()
+        .read_text(encoding='utf-8')
     )
 
 
 def _preprocess_style(raw_css: str) -> str:
     import re
 
     # line breaks are not needed
```

### Comparing `scipp-24.2.0/src/scipp/visualization/show.py` & `scipp-24.5.0/src/scipp/visualization/show.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
 from __future__ import annotations
 
 from html import escape
-from typing import Optional
 
 import numpy as np
 
 from .._scipp import core as sc
 from ..typing import VariableLike
 from . import colors
 from .resources import load_style
@@ -60,34 +59,34 @@
         self._variable = variable
         self._target_dims = target_dims
         if self._target_dims is None:
             self._target_dims = self._dims()
         self._show_alignment = show_alignment
         self._x_stride = 1
         if len(self._dims()) > 3:
-            raise RuntimeError("Cannot visualize {}-D data".format(len(self._dims())))
+            raise RuntimeError(f"Cannot visualize {len(self._dims())}-D data")
 
     def _dims(self):
         dims = self._variable.dims
         return dims
 
     def _draw_box(self, origin_x, origin_y, color, xlen=1):
         return (
             " ".join(
                 [
                     '<rect',
                     'style="fill:{};fill-opacity:1;stroke:#000;stroke-width:0.05"',
                     'id="rect"',
                     'width="xlen" height="1" x="origin_x" y="origin_y"/>',
                     '<path',
-                    'style="fill:{};stroke:#000;stroke-width:0.05;stroke-linejoin:round"',  # noqa #501
+                    'style="fill:{};stroke:#000;stroke-width:0.05;stroke-linejoin:round"',
                     'd="m origin_x origin_y l 0.3 -0.3 h xlen l -0.3 0.3 z"',
                     'id="path1" />',
                     '<path',
-                    'style="fill:{};stroke:#000;stroke-width:0.05;stroke-linejoin:round"',  # noqa #501
+                    'style="fill:{};stroke:#000;stroke-width:0.05;stroke-linejoin:round"',
                     'd="m origin_x origin_y m xlen 0 l 0.3 -0.3 v 1 l -0.3 0.3 z"',
                     'id="path2" />',
                 ]
             )
             .format(*_color_variants(color))
             .replace("origin_x", str(origin_x))
             .replace("origin_y", str(origin_y))
@@ -105,15 +104,15 @@
         depth = shape[-3] + 1
         return 0.3 * depth
 
     def _extents(self):
         """Compute 3D extent, remapping dimension order to target dim order"""
         shape = self._variable.shape
         dims = self._dims()
-        d = dict(zip(dims, shape))
+        d = dict(zip(dims, shape, strict=True))
         e = []
         max_extent = _cubes_in_full_width // 2
         for dim in self._target_dims:
             if dim in d:
                 e.append(min(d[dim], max_extent))
             else:
                 e.append(1)
@@ -280,15 +279,15 @@
         if self._variable.variances is not None:
             items.append(('variances', color))
         if self._variable.values is not None:
             items.append(('values', color))
 
         for i, (name, color) in enumerate(items):
             svg += '<g>'
-            svg += '<title>{}</title>'.format(name)
+            svg += f'<title>{name}</title>'
             svg += self._draw_array(
                 color=color,
                 offset=offset
                 + np.array(
                     [
                         (len(items) - i - 1) * self._variance_offset(),
                         i * self._variance_offset(),
@@ -297,17 +296,17 @@
                 events=self._variable.bins is not None,
             )
             svg += '</g>'
             svg += self._draw_labels(offset=offset)
         svg += '</g>'
         svg += self._draw_bins_buffer()
         return (
-            svg.replace('#normal-font', '{}px'.format(_normal_font))
-            .replace('#small-font', '{}px'.format(_small_font))
-            .replace('#smaller-font', '{}px'.format(_smaller_font))
+            svg.replace('#normal-font', f'{_normal_font}px')
+            .replace('#small-font', f'{_small_font}px')
+            .replace('#smaller-font', f'{_smaller_font}px')
         )
 
     def make_svg(self, content_only=False):
         if content_only:
             return self.draw(color=colors.STYLE['data'])
         return _build_svg(
             self.make_svg(content_only=True),
@@ -373,17 +372,17 @@
     def _dims(self):
         dims = self._dataset.dims
         if isinstance(self._dataset, sc.DataArray):
             # Handle, e.g., bin edges of a slice, where data lacks the edge dim
             for item in self._dataset.deprecated_meta.values():
                 for dim in item.dims:
                     if dim not in dims:
-                        dims = (dim,) + dims
+                        dims = (dim, *dims)
         if len(dims) > 3:
-            raise RuntimeError("Cannot visualize {}-D data".format(len(dims)))
+            raise RuntimeError(f"Cannot visualize {len(dims)}-D data")
         return dims
 
     def make_svg(self, content_only=False):
         content = ''
         width = 0
         height = 0
         margin = 0.5
@@ -435,18 +434,20 @@
                         area_z.append(item)
                 else:
                     area_xy.append(item)
 
         ds = self._dataset
         if isinstance(ds, sc.DataArray):
             categories = zip(
-                ['coords', 'masks', 'attrs'], [ds.coords, ds.masks, ds.deprecated_attrs]
+                ['coords', 'masks', 'attrs'],
+                [ds.coords, ds.masks, ds.deprecated_attrs],
+                strict=True,
             )
         else:
-            categories = zip(['coords'], [ds.coords])
+            categories = zip(['coords'], [ds.coords], strict=True)
         for what, items in categories:
             for name, var in sorted(items.items()):
                 item = DrawerItem(
                     name,
                     var,
                     colors.STYLE[what],
                     show_alignment=what == 'coords',
@@ -478,42 +479,40 @@
                 )
             return content, width, height
 
         top = 0
         left = 0
 
         c, w, h = draw_area(area_xy, 'y')
-        content += '<g transform="translate(0,{})">{}</g>'.format(height, c)
+        content += f'<g transform="translate(0,{height})">{c}</g>'
         c_x, w_x, h_x = draw_area(area_x, 'y')
         c_y, w_y, h_y = draw_area(area_y, 'x', reverse=True)
         height += max(h, h_y)
         width += max(w, w_x)
 
         c, w, h = draw_area(area_z, 'x')
-        content += '<g transform="translate({},{})">{}</g>'.format(width, height - h, c)
+        content += f'<g transform="translate({width},{height - h})">{c}</g>'
         width += w
 
-        content += '<g transform="translate({},{})">{}</g>'.format(
-            -w_y, height - h_y, c_y
-        )
+        content += f'<g transform="translate({-w_y},{height - h_y})">{c_y}</g>'
 
         c, w_0d, h_0d = draw_area(area_0d, 'x', reverse=True, truncate=True)
-        content += '<g transform="translate({},{})">{}</g>'.format(-w_0d, height, c)
+        content += f'<g transform="translate({-w_0d},{height})">{c}</g>'
         width += max(w_y, w_0d)
         left -= max(w_y, w_0d)
 
-        content += '<g transform="translate(0,{})">{}</g>'.format(height, c_x)
+        content += f'<g transform="translate(0,{height})">{c_x}</g>'
         height += max(h_x, h_0d)
 
         if content_only:
             return content
         return _build_svg(content, left, top, max(_cubes_in_full_width, width), height)
 
 
-def make_svg(container: VariableLike, content_only: Optional[bool] = False) -> str:
+def make_svg(container: VariableLike, content_only: bool | None = False) -> str:
     """
     Return an SVG representation of a variable, data array, or dataset.
     """
     if isinstance(container, sc.Variable):
         draw = VariableDrawer(container)
     else:
         draw = DatasetDrawer(container)
```

### Comparing `scipp-24.2.0/src/scipp/visualization/table.py` & `scipp-24.5.0/src/scipp/visualization/table.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Dict, List, Union
 
 import numpy as np
 
 from .. import DataArray, Dataset, DType, Variable
 from ..typing import VariableLike
 
 CENTER = 'text-align: center;'
@@ -31,32 +30,32 @@
     return f'{v.value:.{prec}f}&plusmn;{err:.{prec}f}'
 
 
 def _var_name_with_unit(name: str, var: Variable) -> str:
     out = f'<span style="font-weight: bold;">{name}</span>'
     unit = var.bins.unit if var.bins is not None else var.unit
     if unit is not None:
-        out += ' [𝟙]' if unit == 'dimensionless' else f' [{unit}]'
+        out += ' [𝟙]' if unit == 'dimensionless' else f' [{unit}]'  # noqa: RUF001
     return out
 
 
-def _add_td_tags(cell_list: List[str], border: str = '') -> List[str]:
+def _add_td_tags(cell_list: list[str], border: str = '') -> list[str]:
     td = f' style="{border}"' if border else ''
     td = f'<td{td}>'
     return [f'{td}{cell}</td>' for cell in cell_list]
 
 
 def _make_variable_column(
     name: str,
     var: Variable,
     indices: list,
     need_bin_edge: bool,
     is_bin_edge,
     border: str = '',
-) -> List[str]:
+) -> list[str]:
     head = [_var_name_with_unit(name, var)]
     rows = []
     for i in indices:
         if i is None:
             rows.append('...')
         else:
             rows.append(_string_in_cell(var[i]))
@@ -68,15 +67,15 @@
     return _add_td_tags(head, border=border + BOTTOM_BORDER) + _add_td_tags(
         rows, border=border
     )
 
 
 def _make_data_array_table(
     da: DataArray, indices: list, bin_edges: bool, no_left_border: bool = False
-) -> List[list]:
+) -> list[list]:
     out = [
         _make_variable_column(
             name='',
             var=da.data,
             indices=indices,
             need_bin_edge=bin_edges,
             is_bin_edge=False,
@@ -134,15 +133,15 @@
                 f'<th style="{CENTER}" '
                 f'colspan="{len(da.deprecated_attrs)}">Attributes</th>'
             )
     out += '</tr>'
     return out
 
 
-def _to_html_table(header: str, body: List[list]) -> str:
+def _to_html_table(header: str, body: list[list]) -> str:
     out = '<table>' + header
     ncols = len(body)
     nrows = len(body[0])
     for i in range(nrows):
         out += '<tr>' + ''.join([body[j][i] for j in range(ncols)]) + '</tr>'
     out += '</table>'
     return out
@@ -173,25 +172,25 @@
                 if var.dims == da.data.dims
             },
             masks={key: var.broadcast(sizes=da.sizes) for key, var in da.masks.items()},
         )
     return Dataset(out)
 
 
-def _to_dataset(obj: Union[VariableLike, dict]) -> Dataset:
+def _to_dataset(obj: VariableLike | dict) -> Dataset:
     if isinstance(obj, DataArray):
         return Dataset({obj.name: obj})
     if isinstance(obj, Variable):
         return Dataset(data={"": obj})
     if isinstance(obj, dict):
         return Dataset(obj)
     return obj
 
 
-def table(obj: Dict[str, Union[Variable, DataArray]], max_rows: int = 20):
+def table(obj: dict[str, Variable | DataArray], max_rows: int = 20):
     """Create an HTML table from the contents of the supplied object.
 
     Possible inputs are:
      - Variable
      - DataArray
      - Dataset
      - dict of Variable
@@ -214,15 +213,15 @@
 
     obj = _strip_scalars_and_broadcast_masks(obj)
 
     # Limit the number of rows to be printed
     size = obj.shape[0]
     if size > max_rows:
         half = int(max_rows / 2)
-        inds = list(range(half)) + [None] + list(range(size - half, size))
+        inds = [*range(half), None, *range(size - half, size)]
     else:
         inds = range(size)
 
     bin_edges = _find_bin_edges(obj)
 
     header = _make_sections_header(obj)
     if len(obj) > 1:
```

### Comparing `scipp-24.2.0/src/scipp/visualization/templates/datagroup.css` & `scipp-24.5.0/src/scipp/visualization/templates/datagroup.css`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/src/scipp/visualization/templates/dg_atomic_row.html` & `scipp-24.5.0/src/scipp/visualization/templates/dg_atomic_row.html`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/src/scipp/visualization/templates/dg_collapsible_row.html` & `scipp-24.5.0/src/scipp/visualization/templates/dg_collapsible_row.html`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/src/scipp/visualization/templates/dg_detail_list.html` & `scipp-24.5.0/src/scipp/visualization/templates/dg_detail_list.html`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/src/scipp/visualization/templates/dg_repr.html` & `scipp-24.5.0/src/scipp/visualization/templates/dg_repr.html`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/src/scipp/visualization/templates/icons-svg-inline.html` & `scipp-24.5.0/src/scipp/visualization/templates/icons-svg-inline.html`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/src/scipp/visualization/templates/style.css` & `scipp-24.5.0/src/scipp/visualization/templates/style.css`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/binning_test.py` & `scipp-24.5.0/tests/binning_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,21 +229,21 @@
     assert sc.identical(coord, expected)
 
 
 @pytest.mark.parametrize('dtype', ['int32', 'int64'])
 def test_bin_integer_coord_by_fractional_stepsize_raises(dtype):
     table = sc.data.table_xyz(100)
     table.coords['label'] = (table.coords['x'] * 10).to(dtype=dtype)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Step size'):
         table.bin(label=sc.scalar(0.5, unit='m'))
 
 
 def test_bin_with_automatic_bin_bounds_raises_if_no_events():
     table = sc.data.table_xyz(0)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Empty data range'):
         table.bin(x=4)
 
 
 def test_bin_with_manual_bin_bounds_not_raises_if_no_events():
     table = sc.data.table_xyz(0)
     table.bin(x=sc.linspace('x', 0, 1, 4, unit=table.coords['x'].unit))
 
@@ -255,15 +255,17 @@
     assert da.sizes == {'label': 10}
 
 
 def test_group_by_2d():
     table = sc.data.table_xyz(100)
     table.coords['label'] = (table.coords['x'] * 10).to(dtype='int64')
     da = table.bin(y=333).group('label')
-    da.coords['label'] = (sc.arange('y', 0, 333) * da.coords['label']) % 23
+    da.coords['label'] = (sc.arange('y', 0, 333) * da.coords['label']) % sc.scalar(
+        23, unit='m'
+    )
     grouped = da.group('label')
     assert grouped.sizes == {'y': 333, 'label': 23}
 
 
 def test_bin_erases_dims_automatically_if_labels_for_same_dim():
     table = sc.data.table_xyz(100)
     table.coords['x2'] = table.coords['x'] * 2
@@ -580,50 +582,20 @@
 def test_binning_low_level_functions_exist():
     from scipp import binning
 
     binning.make_binned
     binning.make_histogrammed
 
 
-def test_histogram_deprecated_name():
-    da = sc.data.table_xyz(100)
-    x = sc.linspace('x', 0, 1, num=10, unit='m')
-    with pytest.warns(UserWarning):
-        result = sc.histogram(da, bins=x)
-    assert sc.identical(result, da.hist(x=x))
-
-
-def test_bin_deprecated_arguments():
-    da = sc.data.table_xyz(100)
-    x = sc.linspace('x', 0, 1, num=10, unit='m')
-    with pytest.warns(UserWarning):
-        result = sc.bin(da, edges=[x])
-    assert sc.identical(result, da.bin(x=x))
-
-
-def test_rebin_deprecated_keyword_arguments():
-    da = sc.data.table_xyz(100).hist(x=100)
-    x = sc.linspace('x', 0, 1, num=10, unit='m')
-    with pytest.warns(UserWarning):
-        result = sc.rebin(da, 'x', bins=x)
-    assert sc.identical(result, da.rebin(x=x))
-
-
-def test_rebin_deprecated_positional_arguments():
-    da = sc.data.table_xyz(100).hist(x=100)
-    x = sc.linspace('x', 0, 1, num=10, unit='m')
-    with pytest.warns(UserWarning):
-        result = sc.rebin(da, 'x', x)
-    assert sc.identical(result, da.rebin(x=x))
-
-
 @pytest.mark.parametrize('op', ['bin', 'hist', 'nanhist'])
 def test_raises_ValueError_given_variable_and_multiple_edges(op):
     var = sc.array(dims=['row'], values=[1, 2, 3])
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError, match='Edges for exactly one dimension must be specified'
+    ):
         getattr(var, op)(x=2, y=2)
 
 
 def test_variable_hist_equivalent_to_hist_of_data_array_with_counts():
     data = sc.ones(dims=['row'], shape=[4], unit='counts')
     coord = sc.array(dims=['row'], values=[2, 2, 1, 3])
     da = sc.DataArray(data, coords={'x': coord})
@@ -1013,22 +985,22 @@
     assert not sc.identical(grouped.coords['y'], doubled_groups)
     edges *= 2
     groups *= 2
     assert_identical(grouped.coords['x'], doubled_edges)
     assert_identical(grouped.coords['y'], doubled_groups)
 
 
-@pytest.fixture
+@pytest.fixture()
 def noncontiguous_var() -> sc.Variable:
     var = sc.linspace('x', 0, 1, 101, unit='m')[::2]
     assert not var.values.data.contiguous
     return var
 
 
-@pytest.fixture
+@pytest.fixture()
 def contiguous_var(noncontiguous_var: sc.Variable) -> sc.Variable:
     var = noncontiguous_var.copy()
     assert var.values.data.contiguous
     return var
 
 
 def test_noncontiguous_binning(
@@ -1060,7 +1032,15 @@
         ::10
     ]
     contiguous_idx = sc.arange(dim='idx', start=0, stop=1000, step=10, dtype=int)
     assert not nonnontiguous_idx.values.data.contiguous
     assert contiguous_idx.values.data.contiguous
 
     assert_identical(table.group(nonnontiguous_idx), table.group(contiguous_idx))
+
+
+def test_group_automatic_groups_works_with_string_coord():
+    keys = sc.array(dims=['row'], values=['a', 'b', 'c', 'a', 'b', 'c'])
+    table = sc.DataArray(sc.ones(dims=['row'], shape=[6]), coords={'key': keys})
+    assert sc.identical(
+        table.group('key').coords['key'], sc.array(dims=['key'], values=['a', 'b', 'c'])
+    )
```

### Comparing `scipp-24.2.0/tests/bins_test.py` & `scipp-24.5.0/tests/bins_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 import numpy as np
 import pytest
 from numpy.random import default_rng
 
 import scipp as sc
 
 
+def get_coords(x):
+    return x.coords
+
+
+def get_masks(x):
+    return x.masks
+
+
 def test_dense_data_properties_are_none():
     var = sc.scalar(1)
     assert var.bins is None
 
 
 def test_bins_default_begin_end():
     data = sc.Variable(dims=['x'], values=[1, 2, 3, 4])
@@ -105,15 +113,15 @@
 
 
 def test_bins_raises_when_DataGroup_given():
     data = sc.Variable(dims=['x'], values=[1, 2, 3, 4])
     begin = sc.Variable(dims=['y'], values=[0, 2], dtype=sc.DType.int64, unit=None)
     end = sc.Variable(dims=['y'], values=[2, 4], dtype=sc.DType.int64, unit=None)
     dg = sc.DataGroup(a=data)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='DataGroup argument'):
         sc.bins(begin=begin, end=end, dim='x', data=dg)
 
 
 def test_bins_of_transpose():
     data = sc.Variable(dims=['row'], values=[1, 2, 3, 4])
     begin = sc.Variable(
         dims=['x', 'y'], values=[[0, 1], [2, 3]], dtype=sc.DType.int64, unit=None
@@ -181,14 +189,76 @@
     with pytest.raises(sc.UnitError):
         var.bins.coords['time'].unit = 'K'
     assert var.bins.coords['time'].bins.unit == ''
     var.bins.coords['time'].bins.unit = 'K'
     assert var.bins.coords['time'].bins.unit == 'K'
 
 
+def test_bins_view_coords_iterators():
+    var = make_binned()
+    assert set(var.bins.coords) == {'time'}
+    assert set(var.bins.coords.keys()) == {'time'}
+    [value] = var.bins.coords.values()
+    assert sc.identical(value, var.bins.coords['time'])
+    [(key, value)] = var.bins.coords.items()
+    assert key == 'time'
+    assert sc.identical(value, var.bins.coords['time'])
+
+
+def test_bins_view_masks_iterators():
+    var = make_binned()
+    assert set(var.bins.masks) == {'mask'}
+    assert set(var.bins.masks.keys()) == {'mask'}
+    [value] = var.bins.masks.values()
+    assert sc.identical(value, var.bins.data == var.bins.data)
+    [(key, value)] = var.bins.masks.items()
+    assert key == 'mask'
+    assert sc.identical(value, var.bins.data == var.bins.data)
+
+
+@pytest.mark.parametrize('get', [get_coords, get_masks])
+def test_bins_view_mapping_clear(get):
+    var = make_binned()
+    assert len(get(var.bins)) == 1
+    get(var.bins).clear()
+    assert len(get(var.bins)) == 0
+
+
+@pytest.mark.parametrize('param', [(get_coords, 'time'), (get_masks, 'mask')])
+def test_bins_view_mapping_delitem(param):
+    get, name = param
+    var = make_binned()
+    del get(var.bins)[name]
+    assert len(get(var.bins)) == 0
+
+
+def test_bins_view_coords_update():
+    var = make_binned()
+    var.bins.coords.update({'extra': 2 * var.bins.coords['time']})
+    assert set(var.bins.coords) == {'time', 'extra'}
+    assert sc.identical(var.bins.coords['time'], make_binned().bins.coords['time'])
+    assert sc.identical(var.bins.coords['extra'], 2 * make_binned().bins.coords['time'])
+
+
+def test_bins_view_masks_update():
+    var = make_binned()
+    var.bins.masks.update({'extra': ~var.bins.masks['mask']})
+    assert set(var.bins.masks) == {'mask', 'extra'}
+    assert sc.identical(var.bins.masks['mask'], make_binned().bins.masks['mask'])
+    assert sc.identical(var.bins.masks['extra'], ~make_binned().bins.masks['mask'])
+
+
+@pytest.mark.parametrize('param', [(get_coords, 'time'), (get_masks, 'mask')])
+def test_bins_view_mapping_pop(param):
+    get, name = param
+    var = make_binned()
+    x = get(var.bins).pop(name)
+    assert sc.identical(x, get(make_binned().bins)[name])
+
+
 def test_bins_view_data_unit():
     var = make_binned()
     with pytest.raises(sc.UnitError):
         var.bins.data.unit = 'K'
     assert var.bins.data.bins.unit == ''
     var.bins.data.bins.unit = 'K'
     assert var.bins.data.bins.unit == 'K'
@@ -214,15 +284,15 @@
     values = np.ones(N)
     data = sc.DataArray(
         data=sc.Variable(
             dims=['position'], unit=sc.units.counts, values=values, variances=values
         ),
         coords={
             'position': sc.Variable(
-                dims=['position'], values=['site-{}'.format(i) for i in range(N)]
+                dims=['position'], values=[f'site-{i}' for i in range(N)]
             ),
             'x': sc.Variable(dims=['position'], unit=sc.units.m, values=[0.2] * 5),
             'y': sc.Variable(dims=['position'], unit=sc.units.m, values=[0.2] * 5),
         },
         masks={
             'test-mask': sc.Variable(
                 dims=['position'], values=[True, False, True, False, True]
@@ -425,23 +495,23 @@
     # Prototype is data array with binned data
     binned = sc.DataArray(data=binned)
     assert sc.identical(sc.bins_like(binned, dense), expected)
     # Broadcast
     expected_data = sc.array(dims=['row'], values=[1.1, 1.1, 1.1, 1.1])
     expected = sc.bins(begin=begin, end=end, dim='row', data=expected_data)
     assert sc.identical(sc.bins_like(binned, dense['x', 0]), expected)
+    dense = dense.rename_dims({'x': 'y'})
     with pytest.raises(sc.DimensionError):
-        dense = dense.rename_dims({'x': 'y'})
-        sc.bins_like(binned, dense),
+        (sc.bins_like(binned, dense),)
 
 
 def test_bins_like_raises_when_given_data_group():
     binned = sc.data.binned_x(100, 10)
     dg = sc.DataGroup(a=binned.data)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='DataGroup argument'):
         sc.bins_like(dg, sc.scalar(0.1))
 
 
 def test_bins_concat():
     table = sc.data.table_xyz(nrow=100)
     table.data = sc.arange('row', 100, dtype='float64')
     da = table.bin(x=4, y=5)
```

### Comparing `scipp-24.2.0/tests/common_test.py` & `scipp-24.5.0/tests/common_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/compat/dict_test.py` & `scipp-24.5.0/tests/compat/dict_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/compat/pandas_compat_test.py` & `scipp-24.5.0/tests/compat/pandas_compat_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/compat/wrapping_test.py` & `scipp-24.5.0/tests/compat/wrapping_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 )
 def test_wrap1d_metadata_func1d(da):
     check_metadata(func1d(da, dim='xx'), da, x=None)
 
 
 @pytest.mark.parametrize('func', [factory1d, func1d])
 def test_wrap1d_fail_axis_given(func):
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='dim.*axis'):
         func(make_array(), axis=0, dim='xx')
 
 
 @pytest.mark.parametrize('func', [factory1d, func1d])
 def test_wrap1d_fail_variances(func):
     da = make_array()
     da.variances = da.values
```

### Comparing `scipp-24.2.0/tests/compat/xarray_compat_test.py` & `scipp-24.5.0/tests/compat/xarray_compat_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,15 +299,15 @@
     xr_da = to_xarray(sc_da)
     assert xr_da.coords['a2dcoord'].dims == ("xx", "yy")
     assert np.array_equal(
         xr_da.coords['a2dcoord'].values, sc_da.coords['a2dcoord'].values
     )
 
 
-@pytest.mark.parametrize('coord', ('xx', 'yy'))
+@pytest.mark.parametrize('coord', ['xx', 'yy'])
 def test_to_xarray_dataarray_with_unaligned_coords(coord):
     sc_da = sc.DataArray(
         sc.arange('aux', 0.0, 90, 2, unit='counts').fold(
             'aux', sizes={'yy': 9, 'xx': 5}
         ),
         coords={
             'xx': sc.arange('xx', 5.0, unit='m'),
@@ -342,24 +342,24 @@
 def test_to_xarray_dataarray_fails_on_bin_edges():
     sc_da = sc.DataArray(
         sc.arange('aux', 0.0, 90, 2, unit='counts').fold(
             'aux', sizes={'xx': 5, 'yy': 9}
         ),
         coords={'xx': sc.arange('xx', 6.0, unit='s')},
     )
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='bin edges'):
         _ = to_xarray(sc_da)
 
 
 def test_to_xarray_dataarray_fails_on_binned_data():
     buffer = sc.DataArray(
         sc.ones(sizes={'event': 5}), coords={'id': sc.arange('event', 5)}
     )
     binned = buffer.bin(id=3)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='binned data'):
         _ = to_xarray(binned)
 
 
 def test_to_xarray_dataarray_masks_dropped():
     sc_da = sc.DataArray(
         sc.arange('aux', 0.0, 90, 2, unit='counts').fold(
             'aux', sizes={'xx': 5, 'yy': 9}
```

### Comparing `scipp-24.2.0/tests/concepts_test.py` & `scipp-24.5.0/tests/concepts_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/conftest.py` & `scipp-24.5.0/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import os
-from typing import Any, List
+from typing import Any
 
 import pytest
 
 import scipp as sc
 
 # Silence warning from Jupyter
 os.environ['JUPYTER_PLATFORM_DIRS'] = '1'
 
 pytest.register_assert_rewrite('scipp.testing.assertions')
 
 
-def pytest_assertrepr_compare(op: str, left: Any, right: Any) -> List[str]:
+def pytest_assertrepr_compare(op: str, left: Any, right: Any) -> list[str]:
     if isinstance(left, sc.Unit) and isinstance(right, sc.Unit):
         return [f'Unit({left}) {op} Unit({right})']
     if isinstance(left, sc.DType) or isinstance(right, sc.DType):
         return [f'{left!r} {op} {right!r}']
```

### Comparing `scipp-24.2.0/tests/constants/constants_test.py` & `scipp-24.5.0/tests/constants/constants_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/coords/graph_test.py` & `scipp-24.5.0/tests/coords/graph_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import scipp.coords.graph as scgraph
 from scipp.coords.rule import ComputeRule, FetchRule, RenameRule
 
 
 def graph_0():
     r"""
     a b c
-    |╳| |
+    |X| |
     e d |
     |  \|
     g   f
     """
 
     def fd(a, b):
         pass
@@ -44,15 +44,15 @@
 
 
 def graph_2():
     r"""
     a
     |
     b   c d
-    |\ /╳ |
+    |\ / \|
     | e   f
     g_____|
     """
 
     def fe(b, d, c):
         pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scipp-24.2.0/tests/coords/transform_coords_test.py` & `scipp-24.5.0/tests/coords/transform_coords_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 import functools
+from graphlib import CycleError
 
 import numpy as np
 import pytest
 
 import scipp as sc
 
 
@@ -66,25 +67,25 @@
     return b + d
 
 
 def split(*, a):
     return {'b': a, 'c': 2 * a}
 
 
-@pytest.fixture
+@pytest.fixture()
 def a():
     return sc.arange(dim='a', start=0, stop=4)
 
 
-@pytest.fixture
+@pytest.fixture()
 def b():
     return sc.arange(dim='b', start=2, stop=6)
 
 
-@pytest.fixture
+@pytest.fixture()
 def c():
     return sc.arange(dim='c', start=4, stop=8)
 
 
 def test_diamond_graph(a):
     #   *a
     #  /  \
@@ -321,17 +322,17 @@
     # dim coords: a, c
     # a's contribution to d is only 1/2 because it gets blocked by c.
     original = sc.DataArray(data=a + c, coords={'a': a})
     da = original.transform_coords(['d'], graph=graph)
     assert da.dims == ('a', 'd')
 
 
-@pytest.mark.parametrize('keep_inputs', (True, False))
-@pytest.mark.parametrize('keep_intermediates', (True, False))
-@pytest.mark.parametrize('keep_aliases', (True, False))
+@pytest.mark.parametrize('keep_inputs', [True, False])
+@pytest.mark.parametrize('keep_intermediates', [True, False])
+@pytest.mark.parametrize('keep_aliases', [True, False])
 def test_dim_rename_keep_arguments_have_no_effect(
     a, b, keep_inputs, keep_intermediates, keep_aliases
 ):
     # *x
     #  |
     #  y
     #  |
@@ -359,31 +360,31 @@
     original = sc.DataArray(data=a, coords={'a': a})
     da = original.transform_coords(['b'], graph={'b': 'a'})
     assert da.dims == ('b',)
     da = original.transform_coords(['b'], graph={'b': 'a'}, rename_dims=False)
     assert da.dims == ('a',)
 
 
-@pytest.fixture
+@pytest.fixture()
 def binned_in_a_b():
     events = sc.DataArray(
         data=sc.arange('event', 10, unit='counts'),
         coords={
             'a': sc.array(dims=['event'], values=np.random.rand(10), unit='m'),
             'b': sc.array(dims=['event'], values=np.random.rand(10), unit='m'),
         },
     )
     binned = events.bin(a=2, b=2)
     # use non-bin-edge coord
     binned.coords['b'] = sc.arange('b', 2, unit='m')
     return binned
 
 
-@pytest.mark.parametrize('keep_inputs', (True, False))
-@pytest.mark.parametrize('keep_intermediate', (True, False))
+@pytest.mark.parametrize('keep_inputs', [True, False])
+@pytest.mark.parametrize('keep_intermediate', [True, False])
 def test_keep_aliases_dense(a, b, keep_inputs, keep_intermediate):
     original = sc.DataArray(data=a + b, coords={'a': a, 'b': b})
     graph = {'d': 'c', 'c': 'ab', 'ab': ab}
     da = original.transform_coords(
         ['d'],
         graph=graph,
         keep_aliases=True,
@@ -391,16 +392,16 @@
         keep_intermediate=keep_intermediate,
     )
     assert 'c' in da.coords
     assert not da.coords['c'].aligned
     assert 'd' in da.coords
 
 
-@pytest.mark.parametrize('keep_inputs', (True, False))
-@pytest.mark.parametrize('keep_intermediate', (True, False))
+@pytest.mark.parametrize('keep_inputs', [True, False])
+@pytest.mark.parametrize('keep_intermediate', [True, False])
 def test_not_keep_aliases_dense(a, b, keep_inputs, keep_intermediate):
     original = sc.DataArray(data=a + b, coords={'a': a, 'b': b})
     graph = {'d': 'c', 'c': 'ab', 'ab': ab}
     da = original.transform_coords(
         ['d'],
         graph=graph,
         keep_aliases=False,
@@ -418,16 +419,16 @@
         keep_inputs=keep_inputs,
         keep_intermediate=keep_intermediate,
     )
     assert 'c' in da.coords
     assert 'd' in da.coords
 
 
-@pytest.mark.parametrize('keep_inputs', (True, False))
-@pytest.mark.parametrize('keep_intermediate', (True, False))
+@pytest.mark.parametrize('keep_inputs', [True, False])
+@pytest.mark.parametrize('keep_intermediate', [True, False])
 def test_keep_aliases_binned(binned_in_a_b, keep_inputs, keep_intermediate):
     graph = {'d': 'c', 'c': 'ab', 'ab': ab}
     da = binned_in_a_b.transform_coords(
         ['d'],
         graph=graph,
         keep_aliases=True,
         keep_inputs=keep_inputs,
@@ -437,16 +438,16 @@
     assert not da.coords['c'].aligned
     assert 'c' in da.bins.coords
     assert not da.bins.coords['c'].bins.aligned
     assert 'd' in da.coords
     assert 'd' in da.bins.coords
 
 
-@pytest.mark.parametrize('keep_inputs', (True, False))
-@pytest.mark.parametrize('keep_intermediate', (True, False))
+@pytest.mark.parametrize('keep_inputs', [True, False])
+@pytest.mark.parametrize('keep_intermediate', [True, False])
 def test_not_keep_aliases_binned(binned_in_a_b, keep_inputs, keep_intermediate):
     graph = {'d': 'c', 'c': 'ab', 'ab': ab}
     da = binned_in_a_b.transform_coords(
         ['d'],
         graph=graph,
         keep_aliases=False,
         keep_inputs=keep_inputs,
@@ -467,16 +468,16 @@
     )
     assert 'c' in da.coords
     assert 'c' in da.bins.coords
     assert 'd' in da.coords
     assert 'd' in da.bins.coords
 
 
-@pytest.mark.parametrize('keep_aliases', (True, False))
-@pytest.mark.parametrize('keep_intermediate', (True, False))
+@pytest.mark.parametrize('keep_aliases', [True, False])
+@pytest.mark.parametrize('keep_intermediate', [True, False])
 def test_keep_inputs_dense(a, b, keep_aliases, keep_intermediate):
     original = sc.DataArray(data=a + b, coords={'a': a, 'b': b})
     graph = {'c': 'ab', 'ab': ab}
     da = original.transform_coords(
         ['c'],
         graph=graph,
         keep_aliases=keep_aliases,
@@ -485,16 +486,16 @@
     )
     assert 'a' in da.coords
     assert not da.coords['a'].aligned
     assert 'b' in da.coords
     assert not da.coords['b'].aligned
 
 
-@pytest.mark.parametrize('keep_aliases', (True, False))
-@pytest.mark.parametrize('keep_intermediate', (True, False))
+@pytest.mark.parametrize('keep_aliases', [True, False])
+@pytest.mark.parametrize('keep_intermediate', [True, False])
 def test_not_keep_inputs_dense(a, b, keep_aliases, keep_intermediate):
     original = sc.DataArray(data=a + b, coords={'a': a, 'b': b})
     graph = {'c': 'ab', 'ab': ab}
     da = original.transform_coords(
         ['c'],
         graph=graph,
         keep_aliases=keep_aliases,
@@ -513,16 +514,16 @@
         keep_intermediate=keep_intermediate,
     )
     assert 'a' in da.coords
     assert da.coords['a'].aligned
     assert 'b' not in da.coords
 
 
-@pytest.mark.parametrize('keep_aliases', (True, False))
-@pytest.mark.parametrize('keep_intermediate', (True, False))
+@pytest.mark.parametrize('keep_aliases', [True, False])
+@pytest.mark.parametrize('keep_intermediate', [True, False])
 def test_keep_inputs_binned(binned_in_a_b, keep_aliases, keep_intermediate):
     graph = {'c': 'ab', 'ab': ab}
     da = binned_in_a_b.transform_coords(
         ['c'],
         graph=graph,
         keep_aliases=keep_aliases,
         keep_inputs=True,
@@ -534,16 +535,16 @@
     assert not da.bins.coords['a'].bins.aligned
     assert 'b' in da.coords
     assert not da.coords['b'].aligned
     assert 'b' in da.bins.coords
     assert not da.bins.coords['b'].bins.aligned
 
 
-@pytest.mark.parametrize('keep_aliases', (True, False))
-@pytest.mark.parametrize('keep_intermediate', (True, False))
+@pytest.mark.parametrize('keep_aliases', [True, False])
+@pytest.mark.parametrize('keep_intermediate', [True, False])
 def test_not_keep_inputs_binned(binned_in_a_b, keep_aliases, keep_intermediate):
     graph = {'c': 'ab', 'ab': ab}
     da = binned_in_a_b.transform_coords(
         ['c'],
         graph=graph,
         keep_aliases=keep_aliases,
         keep_inputs=False,
@@ -564,32 +565,32 @@
     )
     assert 'a' in da.coords
     assert 'a' in da.bins.coords
     assert 'b' not in da.meta
     assert 'b' not in da.bins.meta
 
 
-@pytest.mark.parametrize('keep_aliases', (True, False))
-@pytest.mark.parametrize('keep_inputs', (True, False))
+@pytest.mark.parametrize('keep_aliases', [True, False])
+@pytest.mark.parametrize('keep_inputs', [True, False])
 def test_keep_intermediate_dense(a, b, keep_aliases, keep_inputs):
     original = sc.DataArray(data=a + b, coords={'a': a, 'b': b})
     graph = {'c': 'ab', 'ab': ab}
     da = original.transform_coords(
         ['c'],
         graph=graph,
         keep_aliases=keep_aliases,
         keep_inputs=keep_inputs,
         keep_intermediate=True,
     )
     assert 'ab' in da.coords
     assert not da.coords['ab'].aligned
 
 
-@pytest.mark.parametrize('keep_aliases', (True, False))
-@pytest.mark.parametrize('keep_inputs', (True, False))
+@pytest.mark.parametrize('keep_aliases', [True, False])
+@pytest.mark.parametrize('keep_inputs', [True, False])
 def test_not_keep_intermediate_dense(a, b, keep_aliases, keep_inputs):
     original = sc.DataArray(data=a + b, coords={'a': a, 'b': b})
     graph = {'c': 'ab', 'ab': ab}
     da = original.transform_coords(
         ['c'],
         graph=graph,
         keep_aliases=keep_aliases,
@@ -606,16 +607,16 @@
         keep_inputs=keep_inputs,
         keep_intermediate=False,
     )
     assert 'ab' in da.coords
     assert da.coords['ab'].aligned
 
 
-@pytest.mark.parametrize('keep_aliases', (True, False))
-@pytest.mark.parametrize('keep_inputs', (True, False))
+@pytest.mark.parametrize('keep_aliases', [True, False])
+@pytest.mark.parametrize('keep_inputs', [True, False])
 def test_keep_intermediate_binned(binned_in_a_b, keep_aliases, keep_inputs):
     graph = {'c': 'ab', 'ab': ab}
     da = binned_in_a_b.transform_coords(
         ['c'],
         graph=graph,
         keep_aliases=keep_aliases,
         keep_inputs=keep_inputs,
@@ -623,16 +624,16 @@
     )
     assert 'ab' in da.coords
     assert not da.coords['ab'].aligned
     assert 'ab' in da.bins.coords
     assert not da.bins.coords['ab'].bins.aligned
 
 
-@pytest.mark.parametrize('keep_aliases', (True, False))
-@pytest.mark.parametrize('keep_inputs', (True, False))
+@pytest.mark.parametrize('keep_aliases', [True, False])
+@pytest.mark.parametrize('keep_inputs', [True, False])
 def test_not_keep_intermediate_binned(binned_in_a_b, keep_aliases, keep_inputs):
     graph = {'c': 'ab', 'ab': ab}
     da = binned_in_a_b.transform_coords(
         ['c'],
         graph=graph,
         keep_aliases=keep_aliases,
         keep_inputs=keep_inputs,
@@ -732,15 +733,15 @@
     # `a*b` is indeed the product of `a` and `b`
     assert sc.identical(converted.coords['a*b'], renamed.meta['a'] * renamed.meta['b'])
     assert sc.identical(
         converted.bins.coords['a*b'], renamed.bins.meta['a'] * renamed.bins.meta['b']
     )
 
 
-@pytest.mark.parametrize('slice_', (slice(0, 2), slice(2, 4)))
+@pytest.mark.parametrize('slice_', [slice(0, 2), slice(2, 4)])
 def test_binned_slice_computes_correct_results(slice_):
     events = sc.DataArray(
         sc.ones(dims=['event'], shape=[10]), coords={'x': sc.arange('event', 10.0)}
     )
     da = sc.bin(events, x=sc.arange('x', 0.0, 10.0, 2.0))
     sliced = da['x', slice_]
 
@@ -870,23 +871,23 @@
     graph = {'ab': ab, 'abc': abc}
     with pytest.raises(KeyError):
         original.transform_coords(['ab', 'abc'], graph)
 
 
 def test_cycles(a):
     original = sc.DataArray(data=a, coords={'a': a, 'b': a})
-    with pytest.raises(ValueError):
+    with pytest.raises(CycleError):
         original.transform_coords(['c'], graph={'c': 'c'})
-    with pytest.raises(ValueError):
+    with pytest.raises(CycleError):
         original.transform_coords(['c'], graph={'c': 'd', 'd': 'c'})
-    with pytest.raises(ValueError):
+    with pytest.raises(CycleError):
         original.transform_coords(['c'], graph={'c': 'd', 'd': 'e', 'e': 'c'})
-    with pytest.raises(ValueError):
+    with pytest.raises(CycleError):
         original.transform_coords(['c'], graph={'c': bc})
-    with pytest.raises(ValueError):
+    with pytest.raises(CycleError):
         original.transform_coords(['c'], graph={'c': 'd', 'd': bc})
 
 
 def test_new_dim_in_coord(a):
     def x(a):
         return a.rename_dims({'a': 'x'})
 
@@ -904,21 +905,21 @@
 
 def test_vararg_fail(a):
     original = sc.DataArray(data=a, coords={'a': a})
 
     def func(*args):
         pass
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='variable arguments'):
         original.transform_coords(['b'], graph={'b': func})
 
     def func(**kwargs):
         pass
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='variable arguments'):
         original.transform_coords(['b'], graph={'b': func})
 
 
 def test_arg_vs_kwarg_kwonly(a):
     def arg(a):
         return a
 
@@ -958,19 +959,19 @@
 
     def to_bc(*, a):
         return {'b': a, 'c': a}
 
     def to_bd(*, a):
         return {'b': a, 'd': a}
 
-    with pytest.raises(ValueError):
-        graph = {'b': 'a', ('b', 'c'): to_bc}
+    graph = {'b': 'a', ('b', 'c'): to_bc}
+    with pytest.raises(ValueError, match='Duplicate output name'):
         original.transform_coords(['b'], graph=graph)
-    with pytest.raises(ValueError):
-        graph = {('b', 'd'): to_bd, ('b', 'c'): to_bc}
+    graph = {('b', 'd'): to_bd, ('b', 'c'): to_bc}
+    with pytest.raises(ValueError, match='Duplicate output name'):
         original.transform_coords(['b'], graph=graph)
     # b only named once in graph
     graph = {'b': to_bd, 'c': to_bc}
     da = original.transform_coords(['b'], graph=graph)
     assert 'b' in da.coords
 
 
@@ -1008,21 +1009,21 @@
 def test_keyword_syntax_without_entries_and_graph_returns_unchanged():
     da = sc.data.table_xyz(nrow=10)
     assert sc.identical(da.transform_coords(graph={'b': 'y'}), da)
 
 
 def test_raises_when_keyword_syntax_combined_with_targets():
     da = sc.data.table_xyz(nrow=10)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Explicit targets or graph'):
         da.transform_coords('a', a=lambda x: x)
 
 
 def test_raises_when_keyword_syntax_combined_with_graph():
     da = sc.data.table_xyz(nrow=10)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Explicit targets or graph'):
         da.transform_coords(a=lambda x: x, graph={'b': 'y'})
 
 
 def test_raises_when_keyword_syntax_clashes_with_graph_argument():
     da = sc.data.table_xyz(nrow=10)
     with pytest.raises(TypeError):
         da.transform_coords('x', graph=lambda x: x)
```

### Comparing `scipp-24.2.0/tests/core/arithmetic_test.py` & `scipp-24.5.0/tests/core/arithmetic_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/core/comparison_test.py` & `scipp-24.5.0/tests/core/comparison_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 def test_allclose_no_unit():
     a = sc.array(dims=['x'], values=[1, 2, 3], unit=None)
     assert sc.allclose(a, a)
 
 
 @pytest.mark.parametrize(
-    't', (lambda x: x, sc.DataArray, lambda x: sc.Dataset({'a': x}))
+    't', [lambda x: x, sc.DataArray, lambda x: sc.Dataset({'a': x})]
 )
 def test_identical(t):
     assert sc.identical(t(sc.scalar(1.23)), t(sc.scalar(1.23)))
     assert not sc.identical(t(sc.scalar(1.23)), t(sc.scalar(1.23, unit='m')))
     assert not sc.identical(t(sc.scalar(1.23)), t(sc.scalar(5.2)))
     assert not sc.identical(t(sc.scalar(1.23)), t(sc.array(dims=['x'], values=[1.23])))
     assert sc.identical(
@@ -231,25 +231,25 @@
     ds = sc.Dataset({"a": sc.scalar(1)})
     with pytest.raises(TypeError):
         sc.identical(dg, ds)
     with pytest.raises(TypeError):
         sc.identical(ds, dg)
 
 
-@pytest.fixture
+@pytest.fixture()
 def small():
     return sc.scalar(1.0)
 
 
-@pytest.fixture
+@pytest.fixture()
 def medium():
     return sc.scalar(2.0)
 
 
-@pytest.fixture
+@pytest.fixture()
 def large():
     return sc.scalar(3.0)
 
 
 def test_eq(small, medium, large):
     assert not (small == medium).value
     assert not (small == medium.value).value
```

### Comparing `scipp-24.2.0/tests/core/logical_test.py` & `scipp-24.5.0/tests/core/logical_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/core/math_test.py` & `scipp-24.5.0/tests/core/math_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,76 +6,81 @@
 import scipy
 
 import scipp as sc
 
 
 @pytest.mark.parametrize(
     'funcs',
-    (
+    [
         (sc.erf, scipy.special.erf),
         (sc.erfc, scipy.special.erfc),
         (sc.exp, np.exp),
         (sc.log, np.log),
         (sc.log10, np.log10),
         (sc.sqrt, np.sqrt),
         (sc.sinh, np.sinh),
         (sc.cosh, np.cosh),
         (sc.tanh, np.tanh),
         (sc.asinh, np.arcsinh),
         (sc.atanh, np.arctanh),
-    ),
+    ],
 )
 def test_unary_math_compare_to_numpy_dimensionless(funcs):
     sc_f, ref = funcs
     assert sc.allclose(sc_f(sc.scalar(0.512)), sc.scalar(ref(0.512)))
 
 
 def test_unary_math_compare_to_numpy_dimensionless_acosh():
     # Cannot use the value in the generic function
     assert sc.allclose(sc.acosh(sc.scalar(1.612)), sc.scalar(np.arccosh(1.612)))
 
 
-@pytest.mark.parametrize('func', (sc.exp, sc.log, sc.log10, sc.sqrt, sc.sinh))
+@pytest.mark.parametrize('func', [sc.exp, sc.log, sc.log10, sc.sqrt, sc.sinh])
 def test_unary_math_out(func):
     out = sc.scalar(np.nan)
     func(sc.scalar(0.932), out=out)
     assert sc.identical(out, func(sc.scalar(0.932)))
 
 
 @pytest.mark.parametrize(
-    'funcs', ((sc.sin, np.sin), (sc.cos, np.cos), (sc.tan, np.tan))
+    'funcs', [(sc.sin, np.sin), (sc.cos, np.cos), (sc.tan, np.tan)]
 )
 def test_compare_unary_math_to_numpy_trigonometry(funcs):
     sc_f, ref = funcs
     assert sc.allclose(sc_f(sc.scalar(0.512, unit='rad')), sc.scalar(ref(0.512)))
 
 
-@pytest.mark.parametrize('func', (sc.sin, sc.cos, sc.tan))
+@pytest.mark.parametrize('func', [sc.sin, sc.cos, sc.tan])
 def test_unary_math_trigonometry_out(func):
     out = sc.scalar(np.nan)
     func(sc.scalar(0.932, unit='rad'), out=out)
     assert sc.identical(out, func(sc.scalar(0.932, unit='rad')))
 
 
 @pytest.mark.parametrize(
-    'funcs', ((sc.asin, np.arcsin), (sc.acos, np.arccos), (sc.atan, np.arctan))
+    'funcs', [(sc.asin, np.arcsin), (sc.acos, np.arccos), (sc.atan, np.arctan)]
 )
 def test_compare_unary_math_to_numpy_inv_trigonometry(funcs):
     sc_f, ref = funcs
     assert sc.allclose(sc_f(sc.scalar(0.512)), sc.scalar(ref(0.512), unit='rad'))
 
 
-@pytest.mark.parametrize('func', (sc.asin, sc.acos, sc.atan))
+@pytest.mark.parametrize('func', [sc.asin, sc.acos, sc.atan])
 def test_unary_math_inv_trigonometry_out(func):
     out = sc.scalar(np.nan, unit='rad')
     func(sc.scalar(0.932), out=out)
     assert sc.identical(out, func(sc.scalar(0.932)))
 
 
-@pytest.mark.parametrize('args', ((sc.sqrt, sc.Unit('m^2'), sc.Unit('m')),))
+@pytest.mark.parametrize(
+    'args',
+    [
+        (sc.sqrt, sc.Unit('m^2'), sc.Unit('m')),
+    ],
+)
 def test_unary_math_unit(args):
     func, inp, expected = args
     assert func(inp) == expected
 
 
 def test_abs():
     assert sc.identical(sc.abs(sc.scalar(-72)), sc.scalar(72))
```

### Comparing `scipp-24.2.0/tests/core/reduction_test.py` & `scipp-24.5.0/tests/core/reduction_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -936,15 +936,15 @@
     da = sc.DataArray(data=data, masks={'mask': mask})
     da.sum()
 
 
 # See docstring of these functions about why the `ddof` parameter is required.
 # This test exists to prevent accidental or intentional but not thoroughly
 # thought-out changes.
-@pytest.mark.parametrize('opname', ('var', 'nanvar', 'std', 'nanstd'))
+@pytest.mark.parametrize('opname', ['var', 'nanvar', 'std', 'nanstd'])
 def test_variance_reductions_require_ddof_param(opname):
     data = sc.zeros(sizes={'x': 2})
 
     func = getattr(sc, opname)
     with pytest.raises(TypeError, match='ddof'):
         func(data)
```

### Comparing `scipp-24.2.0/tests/counts_test.py` & `scipp-24.5.0/tests/counts_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/cumulative_test.py` & `scipp-24.5.0/tests/cumulative_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/curve_fit_test.py` & `scipp-24.5.0/tests/curve_fit_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
 import numpy as np
 import pytest
 
 import scipp as sc
 from scipp import curve_fit
 from scipp.compat.xarray_compat import from_xarray, to_xarray
+from scipp.testing import assert_identical
+
+
+@pytest.fixture()
+def rng():
+    return np.random.default_rng(seed=1234)
 
 
 def func(x, a, b):
     return a * sc.exp(-b * x)
 
 
 def func2d(x, t, a, b):
@@ -49,91 +55,93 @@
     return sc.DataArray(data, coords=da_coords)
 
 
 def array1d(*, a=1.2, b=1.3, noise_scale=0.1, size=50):
     return array(
         # Note, dim name different from coord name to make sure
         # the code doesn't depend on them being the same.
-        coords=dict(x=dict(dim='xx', start=-0.1, stop=4.0, num=size)),
+        coords={'x': {'dim': 'xx', 'start': -0.1, 'stop': 4.0, 'num': size}},
         f=partial(func, a=a, b=b),
         noise_scale=noise_scale,
     )
 
 
 def array2d(*, a=1.2, b=1.3, noise_scale=0.1, size=20):
     return array(
-        coords=dict(
-            x=dict(dim='xx', start=-0.1, stop=4.0, num=size),
-            t=dict(dim='tt', start=0.0, stop=1.0, num=size // 2),
-        ),
+        coords={
+            'x': {'dim': 'xx', 'start': -0.1, 'stop': 4.0, 'num': size},
+            't': {'dim': 'tt', 'start': 0.0, 'stop': 1.0, 'num': size // 2},
+        },
         f=partial(func2d, a=a, b=b),
         noise_scale=noise_scale,
     )
 
 
 def array3d(*, a=1.2, b=1.3, noise_scale=0.1, size=10):
     return array(
-        coords=dict(
-            x=dict(dim='xx', start=-0.1, stop=4.0, num=size),
-            t=dict(dim='tt', start=0.0, stop=1.0, num=size // 2),
-            y=dict(dim='yy', start=2.0, stop=4.0, num=size),
-        ),
+        coords={
+            'x': {'dim': 'xx', 'start': -0.1, 'stop': 4.0, 'num': size},
+            't': {'dim': 'tt', 'start': 0.0, 'stop': 1.0, 'num': size // 2},
+            'y': {'dim': 'yy', 'start': 2.0, 'stop': 4.0, 'num': size},
+        },
         f=partial(func3d, a=a, b=b),
         noise_scale=noise_scale,
     )
 
 
 def array1d_from_vars(*, a, b, noise_scale=0.1, size=50):
     return array(
-        coords=dict(x=dict(dim='xx', start=0.1, stop=4.0, num=size, unit='m')),
+        coords={
+            'x': {'dim': 'xx', 'start': 0.1, 'stop': 4.0, 'num': size, 'unit': 'm'}
+        },
         f=partial(func, a=a, b=b),
         noise_scale=noise_scale,
     )
 
 
 def test_should_not_raise_given_function_with_dimensionless_params_and_1d_array():
     curve_fit(['x'], func, array1d())
 
 
 @pytest.mark.parametrize(
-    "p0, params, bounds",
-    (
-        (None, dict(a=1.2, b=1.3), None),
-        (dict(a=3, b=2), dict(a=1.2, b=1.3), None),
-        (dict(a=0.2, b=-1), dict(a=1.2, b=1.3), {'a': (-3, 3), 'b': (-2, 2)}),
-        (dict(a=0.2, b=-1), dict(a=1.2, b=1.3), {'a': (-3, 1.1), 'b': (-2, 1.1)}),
-    ),
+    ('p0', 'params', 'bounds'),
+    [
+        (None, {'a': 1.2, 'b': 1.3}, None),
+        ({'a': 3, 'b': 2}, {'a': 1.2, 'b': 1.3}, None),
+        ({'a': 0.2, 'b': -1}, {'a': 1.2, 'b': 1.3}, {'a': (-3, 3), 'b': (-2, 2)}),
+        ({'a': 0.2, 'b': -1}, {'a': 1.2, 'b': 1.3}, {'a': (-3, 1.1), 'b': (-2, 1.1)}),
+    ],
 )
 @pytest.mark.parametrize(
     "dims",
-    (
-        dict(x=10, t=10, y=10),
-        dict(x=5, t=8, y=7),
-    ),
+    [
+        {'x': 10, 't': 10, 'y': 10},
+        {'x': 5, 't': 8, 'y': 7},
+    ],
 )
 @pytest.mark.parametrize(
-    "coords, reduce_dims",
-    (
+    ('coords', 'reduce_dims'),
+    [
         (['x'], []),
         (['x'], ['y']),
         (['x'], ['t', 'y']),
         (['x', 't'], []),
         (['x', 't'], ['y']),
         (['x', 't', 'y'], []),
-    ),
+    ],
 )
 def test_compare_to_curve_fit_xarray(dims, coords, reduce_dims, p0, params, bounds):
     _ = pytest.importorskip('xarray')
     f, fxarray = {
         1: (func, func_np),
         2: (func2d, lambda x, a, b: func2d_np(*x, a, b)),
         3: (func3d, lambda x, a, b: func3d_np(*x, a, b)),
     }[len(coords)]
     da = array(
-        {c: dict(start=1, stop=3, num=n) for c, n in dims.items()},
+        {c: {'start': 1, 'stop': 3, 'num': n} for c, n in dims.items()},
         partial(func3d, **params),
         noise_scale=0.0,
     )
 
     result, _ = curve_fit(
         coords,
         f,
@@ -192,25 +200,25 @@
 
 
 def test_should_raise_TypeError_when_sigma_given_as_param():
     with pytest.raises(TypeError):
         curve_fit(['x'], func, array1d(), sigma=np.arange(4))
 
 
-def test_should_raise_ValueError_when_sigma_contains_zeros():
+def test_should_raise_ValueError_when_sigma_contains_zeros(rng):
     da = array1d(size=50)
-    da.variances = np.random.default_rng().normal(0.0, 0.1, size=50) ** 2
+    da.variances = rng.normal(0.0, 0.1, size=50) ** 2
     da['xx', 21].variance = 0.0
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='0 in the input variances'):
         curve_fit(['x'], func, da)
 
 
-def test_does_not_raise_when_sigma_contains_zeros_that_is_masked():
+def test_does_not_raise_when_sigma_contains_zeros_that_is_masked(rng):
     da = array1d(size=50)
-    da.variances = np.random.default_rng().normal(0.0, 0.1, size=50) ** 2
+    da.variances = rng.normal(0.0, 0.1, size=50) ** 2
     da.masks['m'] = sc.full(value=False, sizes=da.sizes)
     da['xx', 21].variance = 0.0
     da.masks['m']['xx', 21] = True
     curve_fit(['x'], func, da)
 
 
 def test_should_raise_KeyError_when_data_array_has_no_coord():
@@ -236,20 +244,20 @@
     da.masks['mask'][-5:] = sc.scalar(True)
     masked, _ = curve_fit(['x'], func, da)
     assert not sc.identical(masked['a'], unmasked['a'])
     assert not sc.identical(masked['b'], unmasked['b'])
 
 
 @pytest.mark.parametrize(
-    "f,array,coords",
-    (
+    ('f', 'array', 'coords'),
+    [
         (func, array1d, ['x']),
         (func2d, array2d, ['x', 't']),
         (func3d, array3d, ['x', 't', 'y']),
-    ),
+    ],
 )
 @pytest.mark.parametrize(
     "noise_scale",
     [1e-1, 1e-2, 1e-3, 1e-6, 1e-9],
 )
 def test_optimized_params_approach_real_params_as_data_noise_decreases(
     noise_scale, f, array, coords
@@ -260,20 +268,20 @@
     )
     assert sc.allclose(
         popt['b'].data, sc.scalar(1.5), rtol=sc.scalar(2.0 * noise_scale)
     )
 
 
 @pytest.mark.parametrize(
-    "f,array,coords",
-    (
+    ('f', 'array', 'coords'),
+    [
         (func3d, array3d, ['x', 't', 'y']),
         (func3d, array3d, ['y', 'x', 't']),
         (func3d, array3d, ['t', 'y', 'x']),
-    ),
+    ],
 )
 @pytest.mark.parametrize(
     "noise_scale",
     [1e-1, 1e-2, 1e-3, 1e-6, 1e-9],
 )
 def test_order_of_coords_does_not_matter(noise_scale, f, array, coords):
     popt, _ = curve_fit(coords, f, array(a=1.7, b=1.5, noise_scale=noise_scale))
@@ -282,27 +290,27 @@
     )
     assert sc.allclose(
         popt['b'].data, sc.scalar(1.5), rtol=sc.scalar(2.0 * noise_scale)
     )
 
 
 @pytest.mark.parametrize(
-    "f,fnp,array,coords",
-    (
+    ('f', 'fnp', 'array', 'coords'),
+    [
         (func, func_np, array1d, ['x']),
         (func2d, func2d_np, array2d, ['x', 't']),
         (func3d, func3d_np, array3d, ['x', 't', 'y']),
-    ),
+    ],
 )
 def test_scipp_fun_and_numpy_fun_finds_same_optimized_params(f, fnp, array, coords):
     data = array(a=1.7, b=1.5, noise_scale=1e-2)
     popt, _ = curve_fit(coords, f, data)
     popt_np, _ = curve_fit(coords, fnp, data, unsafe_numpy_f=True)
 
-    for p, p_np in zip(popt.values(), popt_np.values()):
+    for p, p_np in zip(popt.values(), popt_np.values(), strict=True):
         assert sc.allclose(p.data, p_np.data, rtol=sc.scalar(2.0 * 1e-2))
 
 
 def test_optimized_params_variances_are_diag_of_covariance_matrix():
     popt, pcov = curve_fit(['x'], func, array1d(a=1.7, b=1.5))
     assert popt['a'].variances == pcov['a']['a'].data.values
     assert popt['b'].variances == pcov['b']['b'].data.values
@@ -319,15 +327,15 @@
         ['x'], func, sc.concat([da[:mask_pos], da[mask_pos + mask_size :]], da.dim)
     )
     assert sc.identical(masked['a'], removed['a'])
     assert sc.identical(masked['b'], removed['b'])
 
 
 @pytest.mark.parametrize(
-    "variance,expected",
+    ('variance', 'expected'),
     [(1e9, 1.0), (1, 2.0), (1 / 3, 3.0), (1e-9, 5.0)],
     ids=['disabled', 'equal', 'high', 'dominant'],
 )
 def test_variances_determine_weights(variance, expected):
     x = sc.array(dims=['x'], values=[1, 2, 3, 4])
     y = sc.array(
         dims=['x'], values=[1.0, 5.0, 1.0, 1.0], variances=[1.0, 1.0, 1.0, 1.0]
@@ -474,29 +482,29 @@
 
 def test_can_pass_extra_kwargs():
     data = array1d()
 
     # Does not raise
     curve_fit(['x'], func, data, method='lm')
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='method'):
         curve_fit(['x'], func, data, method='bad_method')
 
 
 def test_can_rename_coords():
     def func(apple, *, a, b):
         return a * sc.exp(-b * apple)
 
-    curve_fit(dict(apple='x'), func, array1d())
+    curve_fit({'apple': 'x'}, func, array1d())
 
 
 def test_can_use_non_coord_in_fit():
     data = array1d()
     z = data.coords['x'].copy()
-    curve_fit(dict(x=z), func, data)
+    curve_fit({'x': z}, func, data)
 
 
 def test_1d_mask():
     noise_scale = 0.01
     da = array1d(a=1.2, b=1.3, noise_scale=noise_scale)
     mask = (da.coords['x'] > 1) & (da.coords['x'] < 2)
     da.data += sc.where(mask, sc.scalar(1000_000), sc.scalar(0))
@@ -506,14 +514,31 @@
         res['a'].data, sc.scalar(1.2), atol=sc.scalar(noise_scale, unit='dimensionless')
     )
     assert sc.allclose(
         res['b'].data, sc.scalar(1.3), atol=sc.scalar(noise_scale, unit='dimensionless')
     )
 
 
+def test_several_masks():
+    noise_scale = 0.01
+    da = array1d(a=1.2, b=1.3, noise_scale=noise_scale)
+    mask1 = (da.coords['x'] > 1) & (da.coords['x'] <= 1.5)
+    mask2 = (da.coords['x'] > 1.5) & (da.coords['x'] <= 2)
+    da.data += sc.where(mask1 | mask2, sc.scalar(1000_000), sc.scalar(0))
+    da.masks['high1'] = mask1
+    da.masks['high2'] = mask2
+    res, _ = curve_fit(['x'], func, da)
+    assert sc.allclose(
+        res['a'].data, sc.scalar(1.2), atol=sc.scalar(noise_scale, unit='dimensionless')
+    )
+    assert sc.allclose(
+        res['b'].data, sc.scalar(1.3), atol=sc.scalar(noise_scale, unit='dimensionless')
+    )
+
+
 def test_2d_mask():
     noise_scale = 0.01
     da = array2d(a=1.2, b=1.3, noise_scale=noise_scale)
     mask = (
         (da.coords['x'] > 1)
         & (da.coords['x'] < 2)
         & (da.coords['t'] > 0.4)
@@ -524,7 +549,38 @@
     res, _ = curve_fit(['x', 't'], func2d, da)
     assert sc.allclose(
         res['a'].data, sc.scalar(1.2), atol=sc.scalar(noise_scale, unit='dimensionless')
     )
     assert sc.allclose(
         res['b'].data, sc.scalar(1.3), atol=sc.scalar(noise_scale, unit='dimensionless')
     )
+
+
+def test_mask_persists_only_if_fit_is_not_over_mask_dimension():
+    noise_scale = 0.01
+    da = array2d(a=1.2, b=1.3, noise_scale=noise_scale)
+    mask = (da.coords['t'] > 0.4) & (da.coords['t'] < 0.6)
+    da.masks['high'] = mask
+    da.masks['mixed_dims'] = mask & (da.coords['x'] > 0.4)
+    res, _ = curve_fit(['x'], func, da)
+
+    assert 'high' in res['a'].masks
+    assert_identical(res['a'].masks['high'], mask)
+
+    assert 'mixed_dims' not in res['a'].masks
+
+
+def test_param_values_set_to_nan_if_too_few_to_fit():
+    da = array1d(a=1.2, b=1.3, noise_scale=0.01)
+
+    # Mask everything
+    da.masks['mask'] = da.coords['x'] > float('-inf')
+
+    res, cov = curve_fit(['x'], func, da)
+    assert sc.isnan(res['a'].data).all()
+    assert sc.isnan(cov['a']['b'].data).all()
+
+    # Unmask two entries
+    da.masks['mask'][:2] = sc.scalar(False)
+    res, cov = curve_fit(['x'], func, da)
+    assert not sc.isnan(res['a'].data).any()
+    assert not sc.isnan(cov['a']['b'].data).any()
```

### Comparing `scipp-24.2.0/tests/data_array_test.py` & `scipp-24.5.0/tests/data_array_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,17 +82,17 @@
         attrs={'meta': a.attrs['meta']},
         masks={'mask1': a.masks['mask1']},
     )
 
     assert sc.identical(a, c)
 
 
-@pytest.mark.parametrize('coords_wrapper', (dict, lambda d: d), ids=['dict', 'Coords'])
-@pytest.mark.parametrize('attrs_wrapper', (dict, lambda d: d), ids=['dict', 'Attrs'])
-@pytest.mark.parametrize('masks_wrapper', (dict, lambda d: d), ids=['dict', 'Masks'])
+@pytest.mark.parametrize('coords_wrapper', [dict, lambda d: d], ids=['dict', 'Coords'])
+@pytest.mark.parametrize('attrs_wrapper', [dict, lambda d: d], ids=['dict', 'Attrs'])
+@pytest.mark.parametrize('masks_wrapper', [dict, lambda d: d], ids=['dict', 'Masks'])
 def test_init_from_existing_metadata(coords_wrapper, attrs_wrapper, masks_wrapper):
     da1 = sc.DataArray(
         sc.arange('x', 4),
         coords={'x': sc.arange('x', 5, unit='m'), 'y': sc.scalar(12.34)},
         attrs={'a': sc.arange('x', 4, unit='s'), 'b': sc.scalar('attr-b')},
         masks={'m': sc.array(dims=['x'], values=[False, True, True, False, False])},
     )
@@ -502,15 +502,15 @@
     )
 
 
 def test_assign_coords_overlapping_names():
     data = sc.array(dims=['x', 'y', 'z'], values=np.random.rand(4, 3, 5))
     da = sc.DataArray(data)
     coord0 = sc.linspace('x', start=0.2, stop=1.61, num=4)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='names .* distinct'):
         da.assign_coords({'coord0': coord0}, coord0=coord0)
 
 
 def test_assign_update_coords():
     data = sc.array(dims=['x', 'y', 'z'], values=np.random.rand(4, 3, 5))
     coord0_o = sc.linspace('x', start=0.2, stop=1.61, num=4)
     coord1_o = sc.linspace('y', start=1, stop=4, num=4)
@@ -550,15 +550,15 @@
     )
 
 
 def test_assign_masks_overlapping_names():
     data = sc.array(dims=['x', 'y', 'z'], values=np.random.rand(4, 3, 5))
     da = sc.DataArray(data)
     mask0 = sc.array(dims=['x'], values=[False, True, True, False])
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='names .* distinct'):
         da.assign_masks({'mask0': mask0}, mask0=mask0)
 
 
 def test_assign_update_masks():
     data = sc.array(dims=['x', 'y', 'z'], values=np.random.rand(4, 3, 5))
     mask0_o = sc.array(dims=['x'], values=[False, True, True, False])
     mask1_o = sc.array(dims=['y'], values=[1, 2, 4])
@@ -599,15 +599,15 @@
     )
 
 
 def test_assign_attrs_overlapping_names():
     data = sc.array(dims=['x', 'y', 'z'], values=np.random.rand(4, 3, 5))
     attr0 = sc.scalar('attribute_0')
     da = sc.DataArray(data)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='names .* distinct'):
         da.assign_attrs({'attr0': attr0}, attr0=attr0)
 
 
 def test_assign_update_attrs():
     data = sc.array(dims=['x', 'y', 'z'], values=np.random.rand(4, 3, 5))
     attr0_o = sc.scalar('attribute_0')
     attr1_o = sc.linspace('y', start=0.2, stop=1.61, num=4)
```

### Comparing `scipp-24.2.0/tests/data_group_test.py` & `scipp-24.5.0/tests/data_group_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     dg = sc.DataGroup(items)
     assert tuple(dg.keys()) == ('a', 'b', 'c', 'd')
 
 
 def test_init_raises_when_keys_are_not_strings():
     d = {1: 0}
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='DataGroup keys must be strings'):
         sc.DataGroup(d)
 
 
 @pytest.mark.parametrize(
     'copy_func', [copy.deepcopy, sc.DataGroup.copy, lambda x: x.copy(deep=True)]
 )
 def test_deepcopy(copy_func):
@@ -423,44 +423,44 @@
     assert 'c' not in result
     assert sc.identical(result['a'], op(inner, x))
 
 
 @pytest.mark.parametrize(
     'op', BINARY_NUMBER_OPERATIONS, ids=BINARY_NUMBER_OPERATION_NAMES
 )
-@pytest.mark.parametrize('typ', (int, float))
-@pytest.mark.parametrize('reverse', (False, True))
+@pytest.mark.parametrize('typ', [int, float])
+@pytest.mark.parametrize('reverse', [False, True])
 def test_arithmetic_data_group_with_builtin(op, typ, reverse):
     op = reverse_op(op, reverse)
     x = sc.arange('x', 1, 5)
     dg = sc.DataGroup({'a': x})
     other = typ(31)
     result = op(dg, other)
     assert 'a' in result
     assert sc.identical(result['a'], op(x, other))
 
 
 @pytest.mark.parametrize(
     'op', BINARY_NUMBER_OPERATIONS, ids=BINARY_NUMBER_OPERATION_NAMES
 )
-@pytest.mark.parametrize('reverse', (False, True))
+@pytest.mark.parametrize('reverse', [False, True])
 def test_arithmetic_data_group_with_variable(op, reverse):
     op = reverse_op(op, reverse)
     x = sc.arange('x', 1, 5, unit='m')
     dg = sc.DataGroup({'a': x})
     other = 2 * x
     result = op(dg, other)
     assert 'a' in result
     assert sc.identical(result['a'], op(x, other))
 
 
 @pytest.mark.parametrize(
     'op', BINARY_NUMBER_OPERATIONS, ids=BINARY_NUMBER_OPERATION_NAMES
 )
-@pytest.mark.parametrize('reverse', (False, True))
+@pytest.mark.parametrize('reverse', [False, True])
 def test_arithmetic_data_group_with_data_array(op, reverse):
     op = reverse_op(op, reverse)
     x = sc.DataArray(sc.arange('x', 1, 5, unit='m'), coords={'x': sc.arange('x', 5)})
     dg = sc.DataGroup({'a': x})
     other = 2 * x
     result = op(dg, other)
     assert 'a' in result
@@ -487,25 +487,25 @@
     assert 'a' in result
     assert 'b' not in result
     assert sc.identical(result['a'], x ** (2 * x))
 
 
 @pytest.mark.parametrize(
     'other',
-    (
+    [
         3,
         sc.arange('x', 0, 4, dtype='int64'),
         sc.DataArray(
             sc.arange('x', 0, 4, dtype='int64'),
             coords={'x': sc.arange('x', 5, dtype='int64')},
         ),
-    ),
+    ],
     ids=('int', 'Variable', 'DataArray'),
 )
-@pytest.mark.parametrize('reverse', (False, True))
+@pytest.mark.parametrize('reverse', [False, True])
 def test_pow_data_group_with_other(other, reverse):
     op = reverse_op(lambda a, b: a**b, reverse)
     x = sc.arange('x', 1, 5, dtype='int64')
     dg = sc.DataGroup({'a': x})
     result = op(dg, other)
     assert 'a' in result
     assert sc.identical(result['a'], op(x, other))
@@ -536,23 +536,23 @@
     dg = sc.DataGroup({'a': x})
     result = ~dg
     assert sc.identical(result['a'], ~x)
 
 
 @pytest.mark.parametrize(
     'op',
-    (
+    [
         operator.iadd,
         operator.isub,
         operator.imul,
         operator.imod,
         operator.itruediv,
         operator.ifloordiv,
         operator.ipow,
-    ),
+    ],
 )
 def test_inplace_is_disabled(op):
     x = sc.arange('x', 1, 5, dtype='int64')
     dg1 = sc.DataGroup({'a': x.copy()})
     dg2 = sc.DataGroup({'a': x.copy()})
     with pytest.raises(TypeError):
         op(dg1, dg2)
@@ -618,15 +618,15 @@
     assert isinstance(result, sc.DataGroup)
     assert sc.identical(result['a'], sc.atan2(y=dg1['a'], x=dg2['a']))
 
 
 def test_elemwise_unary_raises_with_out_arg():
     dg = sc.DataGroup(a=sc.linspace('x', 0.0, 1.0, num=4, unit='rad'))
     out = sc.DataGroup()
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='`out` argument is not supported'):
         sc.sin(dg, out=out)
 
 
 def test_construction_from_dataset_creates_dataarray_items():
     ds = sc.Dataset({'a': sc.scalar(1), 'b': sc.scalar(2)}, coords={'x': sc.scalar(3)})
     dg = sc.DataGroup(ds)
     assert len(dg) == 2
@@ -792,15 +792,15 @@
         b='another string',
     )
     with pytest.raises(sc.DatasetError):
         sc.merge(dg1, dg2)
 
 
 @pytest.mark.parametrize(
-    'func', (sc.bin, lambda x, /, *args, **kwargs: x.bin(*args, **kwargs))
+    'func', [sc.bin, lambda x, /, *args, **kwargs: x.bin(*args, **kwargs)]
 )
 def test_bin(func):
     dg = sc.DataGroup(
         {
             'da': sc.DataArray(
                 10 * sc.arange('x', 5.0), coords={'x': sc.arange('x', 5.0)}
             ),
@@ -844,29 +844,29 @@
     'var',
     'nanmedian',
     'nanstd',
     'nanvar',
 )
 
 
-@pytest.mark.parametrize('dim', ('x', None))
+@pytest.mark.parametrize('dim', ['x', None])
 @pytest.mark.parametrize('op', reduction_ops)
 def test_reduction_op_ignores_python_objects(op, dim):
     dtype = 'bool' if op in ('all', 'any') else 'float64'
     if 'std' in op or 'var' in op:
         op = operator.methodcaller(op, dim=dim, ddof=0)
     else:
         op = operator.methodcaller(op, dim=dim)
     dg = sc.DataGroup(a=sc.ones(dims=['x', 'y'], shape=(2, 3), dtype=dtype), b='abc')
     result = op(dg)
     assert_identical(result['a'], op(dg['a']))
     assert result['b'] == dg['b']
 
 
-@pytest.mark.parametrize('dim', ('x', None))
+@pytest.mark.parametrize('dim', ['x', None])
 @pytest.mark.parametrize('op', reduction_ops)
 def test_reduction_op_ignores_numpy_arrays(op, dim):
     dtype = 'bool' if op in ('all', 'any') else 'float64'
     if 'std' in op or 'var' in op:
         op = operator.methodcaller(op, dim=dim, ddof=0)
     else:
         op = operator.methodcaller(op, dim=dim)
@@ -890,15 +890,15 @@
         b=sc.ones(dims=['y'], shape=(2,), dtype=dtype),
     )
     result = op(dg)
     assert_identical(result['a'], op(dg['a']))
     assert_identical(result['b'], dg['b'])
 
 
-@pytest.mark.parametrize('dim', ('x', None))
+@pytest.mark.parametrize('dim', ['x', None])
 @pytest.mark.parametrize('opname', bin_reduction_ops)
 def test_reduction_op_handles_bin_without_dim(opname, dim):
     dtype = 'bool' if opname in ('all', 'any') else 'float64'
     op = operator.methodcaller(opname, dim=dim)
     content = sc.ones(dims=['row'], shape=[6], dtype=dtype)
     binned = sc.bins(begin=sc.index(0), end=sc.index(6), data=content, dim='row')
     dg = sc.DataGroup(a=sc.ones(dims=['x', 'y'], shape=(2, 3), dtype=dtype), b=binned)
```

### Comparing `scipp-24.2.0/tests/dataset_test.py` & `scipp-24.5.0/tests/dataset_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -716,15 +716,15 @@
 
 
 def test_assign_coords_overlapping_names():
     data = sc.array(dims=['x', 'y', 'z'], values=np.random.rand(4, 3, 5))
     ds = sc.Dataset(data={'data0': data})
     coord0 = sc.linspace('x', start=0.2, stop=1.61, num=4)
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='names .* distinct'):
         ds.assign_coords({'coord0': coord0}, coord0=coord0)
 
 
 def test_assign_update_coords():
     data = sc.array(dims=['x', 'y', 'z'], values=np.random.rand(4, 3, 5))
     coord0_o = sc.linspace('x', start=0.2, stop=1.61, num=4)
     coord1_o = sc.linspace('y', start=1, stop=4, num=3)
```

### Comparing `scipp-24.2.0/tests/datetime_test.py` & `scipp-24.5.0/tests/datetime_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 
 def _mismatch_pairs(units):
     yield from filter(lambda t: t[0] != t[1], itertools.product(units, units))
 
 
 def _make_arrays(units, num_arrays, minsize=1):
     size = np.random.randint(minsize, minsize + 5)
-    units = units if isinstance(units, (tuple, list)) else [units] * num_arrays
+    units = units if isinstance(units, tuple | list) else [units] * num_arrays
     res = [
         np.array(
             [np.datetime64(np.random.randint(0, 100000), unit) for _ in range(size)]
         )
         for unit in units
     ]
     if num_arrays == 1:
         return res[0]
     return res
 
 
 def _make_datetimes(units, num):
-    units = units if isinstance(units, (tuple, list)) else [units] * num
+    units = units if isinstance(units, tuple | list) else [units] * num
     res = [np.datetime64(np.random.randint(0, 1000), unit) for unit in units]
     if num == 1:
         return res[0]
     return res
 
 
 @pytest.mark.parametrize("unit", _UNIT_STRINGS)
@@ -70,21 +70,21 @@
     var = sc.Variable(dims=(), dtype=sc.DType.datetime64, unit=unit, values=value)
     assert var.dtype == sc.DType.datetime64
     assert var.unit == unit
     assert var.value.dtype == f'datetime64[{unit}]'
     assert var.value == np.datetime64(value, unit)
 
 
-@pytest.mark.parametrize("unit1,unit2", _mismatch_pairs(_UNIT_STRINGS))
+@pytest.mark.parametrize(('unit1', 'unit2'), _mismatch_pairs(_UNIT_STRINGS))
 def test_construct_0d_datetime_mismatch(unit1, unit2):
-    with pytest.raises(ValueError):
-        sc.Variable(dims=(), unit=unit1, dtype=f'datetime64[{unit2}]')
+    with pytest.raises(ValueError, match='unit encoded in the dtype'):
+        sc.scalar(1, unit=unit1, dtype=f'datetime64[{unit2}]')
 
 
-@pytest.mark.parametrize("unit1,unit2", _mismatch_pairs(('s', 'ms', 'us', 'ns')))
+@pytest.mark.parametrize(('unit1', 'unit2'), _mismatch_pairs(('s', 'ms', 'us', 'ns')))
 def test_construct_0d_datetime_unit_conversion(unit1, unit2):
     value = np.datetime64(2315169201, unit1)
     expected = sc.to_unit(sc.Variable(dims=(), values=value), unit2)
     assert sc.identical(sc.Variable(dims=(), values=value, unit=unit2), expected)
     assert sc.identical(
         sc.Variable(dims=(), values=value, dtype=f'datetime64[{unit2}]'), expected
     )
@@ -111,19 +111,19 @@
 def test_0d_datetime_setter(unit):
     initial, replacement = _make_datetimes(unit, 2)
     var = sc.Variable(dims=(), values=initial)
     var.value = replacement
     assert sc.identical(var, sc.Variable(dims=(), values=replacement))
 
 
-@pytest.mark.parametrize("unit1,unit2", _mismatch_pairs(_UNIT_STRINGS))
+@pytest.mark.parametrize(('unit1', 'unit2'), _mismatch_pairs(_UNIT_STRINGS))
 def test_0d_datetime_setter_mismatch(unit1, unit2):
     initial, replacement = _make_datetimes((unit1, unit2), 2)
     var1 = sc.Variable(dims=(), values=initial)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='unit'):
         var1.value = replacement
 
 
 @pytest.mark.parametrize("unit", _UNIT_STRINGS)
 def test_construct_datetime(unit):
     dtype = f'datetime64[{unit}]'
     values = _make_arrays(unit, 1)
@@ -148,21 +148,21 @@
     dtype_str = f'datetime64[{unit}]'
     assert var.dtype == sc.DType.datetime64
     assert var.unit == unit
     assert var.values.dtype == dtype_str
     np.testing.assert_array_equal(var.values, values.astype(dtype_str))
 
 
-@pytest.mark.parametrize("unit1,unit2", _mismatch_pairs(_UNIT_STRINGS))
+@pytest.mark.parametrize(('unit1', 'unit2'), _mismatch_pairs(_UNIT_STRINGS))
 def test_construct_datetime_mismatch(unit1, unit2):
-    with pytest.raises(ValueError):
-        sc.Variable(dims=['x'], unit=unit1, dtype=f'datetime64[{unit2}]')
+    with pytest.raises(ValueError, match='unit encoded in the dtype'):
+        sc.array(dims=['x'], values=[1], unit=unit1, dtype=f'datetime64[{unit2}]')
 
 
-@pytest.mark.parametrize("unit1,unit2", _mismatch_pairs(('s', 'ms', 'us', 'ns')))
+@pytest.mark.parametrize(('unit1', 'unit2'), _mismatch_pairs(('s', 'ms', 'us', 'ns')))
 def test_construct_datetime_unit_conversion(unit1, unit2):
     values = _make_arrays(unit1, 1)
     expected = sc.to_unit(sc.Variable(dims=['x'], values=values), unit2)
     assert sc.identical(sc.Variable(dims=['x'], values=values, unit=unit2), expected)
     assert sc.identical(
         sc.Variable(dims=['x'], values=values, dtype=f'datetime64[{unit2}]'), expected
     )
@@ -190,19 +190,19 @@
     initial, replacement = _make_arrays(unit, 2)
     var = sc.Variable(dims=['x'], values=initial)
     var.values = replacement
     np.testing.assert_array_equal(var.values, replacement)
     assert sc.identical(var, sc.Variable(dims=['x'], values=replacement))
 
 
-@pytest.mark.parametrize("unit1,unit2", _mismatch_pairs(_UNIT_STRINGS))
+@pytest.mark.parametrize(('unit1', 'unit2'), _mismatch_pairs(_UNIT_STRINGS))
 def test_datetime_setter_mismatch(unit1, unit2):
     initial, replacement = _make_arrays((unit1, unit2), 2)
     var1 = sc.Variable(dims=['x'], values=initial)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='unit'):
         var1.values = replacement
 
 
 @pytest.mark.parametrize("unit", _UNIT_STRINGS)
 def test_datetime_slicing(unit):
     values1, values2 = _make_arrays(unit, 2, minsize=4)
     var = sc.Variable(dims=['x'], values=values1)
```

### Comparing `scipp-24.2.0/tests/dicts_test.py` & `scipp-24.5.0/tests/dicts_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,15 +461,15 @@
     assert mapview0.items() != mapview1.items()
 
     mapview0['y'] = sc.scalar(3.0)
     assert mapview0.items() == mapview1.items()
 
 
 @pytest.mark.parametrize(
-    "make,mapping",
+    ('make', 'mapping'),
     [
         (make_data_array, "coords"),
         (make_dataset, "coords"),
     ],
 )
 def test_set_aligned(make, mapping):
     d = make(sc.arange('x', 4.0, unit='m'))
```

### Comparing `scipp-24.2.0/tests/domains_test.py` & `scipp-24.5.0/tests/domains_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/dtype_test.py` & `scipp-24.5.0/tests/dtype_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # @author Simon Heybrock
 import numpy as np
 import pytest
 
 import scipp as sc
 
 
-@pytest.mark.parametrize('dt', (sc.DType.int32, sc.DType.float64, sc.DType.string))
+@pytest.mark.parametrize('dt', [sc.DType.int32, sc.DType.float64, sc.DType.string])
 def test_dtype_comparison_equal(dt):
     assert dt == dt
 
 
-@pytest.mark.parametrize('other', (sc.DType.int32, sc.DType.float64, sc.DType.string))
+@pytest.mark.parametrize('other', [sc.DType.int32, sc.DType.float64, sc.DType.string])
 def test_dtype_comparison_not_equal(other):
     assert sc.DType.int64 != other
 
 
-@pytest.mark.parametrize('name', ('int64', 'float32', 'str'))
+@pytest.mark.parametrize('name', ['int64', 'float32', 'str'])
 def test_dtype_comparison_str(name):
     assert sc.DType(name) == name
     assert name == sc.DType(name)
     assert sc.DType(name) != 'bool'
     assert 'bool' != sc.DType(name)
```

### Comparing `scipp-24.2.0/tests/dynamic_binding_test.py` & `scipp-24.5.0/tests/dynamic_binding_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,31 +16,31 @@
         var.copy(), coords={'x': sc.arange('x', 4), 'y': 0.1 * sc.arange('y', 3)}
     )
     return var, da
 
 
 @pytest.mark.parametrize(
     'func_name',
-    ('cumsum', 'max', 'mean', 'min', 'nanmax', 'nanmean', 'nanmin', 'nansum', 'sum'),
+    ['cumsum', 'max', 'mean', 'min', 'nanmax', 'nanmean', 'nanmin', 'nansum', 'sum'],
 )
 def test_bound_methods_reduction_variable(func_name):
     var, _ = make_containers()
     func = getattr(sc, func_name)
     assert sc.identical(getattr(var, func_name)(), func(var))
 
 
-@pytest.mark.parametrize('func_name', ('any', 'all'))
+@pytest.mark.parametrize('func_name', ['any', 'all'])
 def test_bound_methods_reduction_variable_bool(func_name):
     rng = np.random.default_rng(87415)
     var = sc.array(dims=['x', 'y'], values=rng.choice([True, False], (4, 3)))
     func = getattr(sc, func_name)
     assert sc.identical(getattr(var, func_name)(), func(var))
 
 
-@pytest.mark.parametrize('func_name', ('mean', 'nanmean', 'nansum', 'sum'))
+@pytest.mark.parametrize('func_name', ['mean', 'nanmean', 'nansum', 'sum'])
 def test_bound_methods_reduction_dataarray(func_name):
     _, da = make_containers()
     func = getattr(sc, func_name)
     assert sc.identical(getattr(da, func_name)(), func(da))
 
 
 def test_bound_methods_shape():
```

### Comparing `scipp-24.2.0/tests/elemwise_func_test.py` & `scipp-24.5.0/tests/elemwise_func_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/format/format_test.py` & `scipp-24.5.0/tests/format/format_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 import pytest
 
 import scipp as sc
 
 
 @pytest.mark.parametrize(
     'var',
-    (
+    [
         sc.scalar(1),
         sc.scalar(-4, dtype='int32'),
         sc.scalar(3.1, variance=0.1, unit='m'),
         sc.scalar(2.1, variance=0.1, dtype='float32'),
         sc.array(dims=['x', 't'], values=np.ones((3, 4)), unit='kg/s'),
         sc.scalar('some string'),
         sc.array(dims=['s'], values=['str', '2']),
         sc.scalar(6134, dtype='datetime64', unit='s'),
         sc.array(dims=['e'], values=[512, 1662], unit='s'),
-    ),
+    ],
 )
 def test_variable_default(var):
     assert f'{var}' == str(var)
     assert f'{var:}' == str(var)
     assert f'{var::}' == str(var)
-    assert '{:}'.format(var) == str(var)
+    assert '{:}'.format(var) == str(var)  # noqa: UP032, RUF100
 
 
-@pytest.mark.parametrize('s', ('^', ''))
+@pytest.mark.parametrize('s', ['^', ''])
 def test_variable_default_length_central(s):
     var = sc.arange('x', 10)
     assert '[0, 1, ..., 8, 9]' in f'{var:{s}}'
     assert '[0, 1, ..., 8, 9]' in f'{var:{s}#4}'
     assert '[0, 1, ..., 7, 8, 9]' in f'{var:{s}#5}'
     assert '[0, 1, 2, ..., 7, 8, 9]' in f'{var:{s}#6}'
 
@@ -186,35 +186,35 @@
             dims=['ga'], values=values, variances=np.array(errors) ** 2, unit=unit
         )
         assert f'{var:c}' == expected
 
 
 def test_variable_compact_raises_for_length():
     var = sc.scalar(2)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Invalid format spec'):
         f'{var:#3c}'
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Invalid format spec'):
         f'{var:#4c}'
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Invalid format spec'):
         f'{var:#6c}'
 
 
 def test_variable_compact_raises_for_selection():
     var = sc.scalar(2)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Invalid format spec'):
         f'{var:<c}'
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Invalid format spec'):
         f'{var:>c}'
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Invalid format spec'):
         f'{var:^c}'
 
 
 def test_variable_compact_raises_for_nested():
     var = sc.scalar(2)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Invalid format spec'):
         f'{var:c:f}'
 
 
 def test_variable_compact_only_supports_numeric_dtype():
     var = sc.scalar('a string')
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Compact formatting.*string'):
         f'{var:c}'
```

### Comparing `scipp-24.2.0/tests/html/html_repr_test.py` & `scipp-24.5.0/tests/html/html_repr_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/hypothesis/bin_test.py` & `scipp-24.5.0/tests/hypothesis/bin_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 import numpy as np
 from hypothesis import given, settings
 from hypothesis import strategies as st
 
 import scipp as sc
 from scipp.testing import strategies as scst
 
-float_args = dict(
-    min_value=-1e300,
-    max_value=1e300,
-    allow_nan=False,
-    allow_infinity=False,
-    allow_subnormal=False,
-)
+float_args = {
+    'min_value': -1e300,
+    'max_value': 1e300,
+    'allow_nan': False,
+    'allow_infinity': False,
+    'allow_subnormal': False,
+}
 
 
 @given(st.floats(**float_args), st.floats(**float_args))
 def test_bin_2d_linspace_bounds(a, b):
     x = sc.array(dims=['row'], values=[a, b])
     table = sc.DataArray(sc.ones(dims=['row'], shape=[2]))
     table.coords['x'] = x
```

### Comparing `scipp-24.2.0/tests/hypothesis/histogram_test.py` & `scipp-24.5.0/tests/hypothesis/histogram_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 # @author Simon Heybrock
 import numpy as np
 from hypothesis import given
 from hypothesis import strategies as st
 
 import scipp as sc
 
-float_args = dict(
-    min_value=-1e300,
-    max_value=1e300,
-    allow_nan=False,
-    allow_infinity=False,
-    allow_subnormal=False,
-)
+float_args = {
+    'min_value': -1e300,
+    'max_value': 1e300,
+    'allow_nan': False,
+    'allow_infinity': False,
+    'allow_subnormal': False,
+}
 
 
 @given(st.floats(**float_args), st.floats(**float_args))
 def test_histogram_linspace_bounds(a, b):
     x = sc.array(dims=['row'], values=[a, b])
     table = sc.DataArray(sc.ones(dims=['row'], shape=[2]))
     table.coords['x'] = x
```

### Comparing `scipp-24.2.0/tests/hypothesis/lookup_test.py` & `scipp-24.5.0/tests/hypothesis/lookup_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 # @author Simon Heybrock
 import numpy as np
 from hypothesis import given
 from hypothesis import strategies as st
 
 import scipp as sc
 
-float_args = dict(
-    min_value=-1e300,
-    max_value=1e300,
-    allow_nan=False,
-    allow_infinity=False,
-    allow_subnormal=False,
-)
+float_args = {
+    'min_value': -1e300,
+    'max_value': 1e300,
+    'allow_nan': False,
+    'allow_infinity': False,
+    'allow_subnormal': False,
+}
 
 
 @given(st.floats(**float_args), st.floats(**float_args))
 def test_lookup_linspace_bounds(a, b):
     x = sc.array(dims=['row'], values=[a, b])
     upper = x.max()
     upper.value = np.nextafter(upper.value, np.inf)
```

### Comparing `scipp-24.2.0/tests/hypothesis/strategies_test.py` & `scipp-24.5.0/tests/hypothesis/strategies_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/hypothesis/to_unit_test.py` & `scipp-24.5.0/tests/hypothesis/to_unit_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/io/csv_test.py` & `scipp-24.5.0/tests/io/csv_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,21 @@
             'y': sc.array(dims=['row'], values=[2, 5, 8, 11], dtype='int64'),
             'z': sc.array(dims=['row'], values=[3, 6, 9, 12], dtype='int64'),
         }
     )
     assert_identical(loaded, expected)
 
 
-@pytest.mark.parametrize('sep', ('\t', '/'))
+@pytest.mark.parametrize('sep', ['\t', '/'])
 def test_load_csv_dataset_choose_separator(sep):
     csv = '''x,y,z
 1,2,3
 4,5,6
 7,8,9
-10,11,12'''.replace(
-        ',', sep
-    )
+10,11,12'''.replace(',', sep)
 
     loaded = sc.io.load_csv(StringIO(csv), sep=sep)
     expected = sc.Dataset(
         {
             'x': sc.array(dims=['row'], values=[1, 4, 7, 10], dtype='int64'),
             'y': sc.array(dims=['row'], values=[2, 5, 8, 11], dtype='int64'),
             'z': sc.array(dims=['row'], values=[3, 6, 9, 12], dtype='int64'),
```

### Comparing `scipp-24.2.0/tests/io/hdf5_test.py` & `scipp-24.5.0/tests/io/hdf5_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,15 @@
 def test_data_array_dtype_string():
     a = sc.DataArray(data=sc.Variable(dims=['x'], values=['abc', 'def']))
     check_roundtrip(a)
     check_roundtrip(a['x', 0])
 
 
 def test_data_array_unsupported_PyObject_coord():
-    obj = sc.scalar(dict())
+    obj = sc.scalar({})
     a = sc.DataArray(data=x, coords={'obj': obj})
     b = roundtrip(a)
     assert not sc.identical(a, b)
     del a.coords['obj']
     assert sc.identical(a, b)
     a.attrs['obj'] = obj
     assert not sc.identical(a, b)
```

### Comparing `scipp-24.2.0/tests/iteration_test.py` & `scipp-24.5.0/tests/iteration_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,35 +23,35 @@
         yield d['x', 0]
 
 
 def test_dataset_iter(dataset_abc):
     found = set()
     for key in dataset_abc:
         found.add(key)
-    assert found == set(['a', 'b', 'c'])
+    assert found == {'a', 'b', 'c'}
 
 
 def test_dataset_keys(dataset_abc):
-    assert set(dataset_abc.keys()) == set(['a', 'b', 'c'])
+    assert set(dataset_abc.keys()) == {'a', 'b', 'c'}
 
 
 def test_dataset_values(dataset_abc):
     found = set()
     for value in dataset_abc.values():
         found.add(value.name)
-    assert found == set(['a', 'b', 'c'])
+    assert found == {'a', 'b', 'c'}
 
 
 def test_dataset_items(dataset_abc):
     assert len(dataset_abc.items()) == 3
     found = set()
     for name, value in dataset_abc.items():
         assert name == value.name
         found.add(name)
-    assert found == set(['a', 'b', 'c'])
+    assert found == {'a', 'b', 'c'}
 
 
 def make_coords_xyz():
     return sc.Dataset(
         coords={
             'x': 1.0 * sc.units.m,
             'y': 2.0 * sc.units.m,
@@ -61,30 +61,30 @@
 
 
 def test_dataset_coords_iter():
     d = make_coords_xyz()
     found = set()
     for key in d.coords:
         found.add(str(key))
-    assert found == set(['x', 'y', 'z'])
+    assert found == {'x', 'y', 'z'}
 
 
 def test_dataset_coords_keys():
     d = make_coords_xyz()
-    assert set(d.coords.keys()) == set(['x', 'y', 'z'])
+    assert set(d.coords.keys()) == {'x', 'y', 'z'}
 
 
 def test_dataset_coords_values():
     d = make_coords_xyz()
     found = set()
     for value in d.coords.values():
         found.add(value.value)
-    assert found == set([1.0, 2.0, 3.0])
+    assert found == {1.0, 2.0, 3.0}
 
 
 def test_dataset_coords_items():
     d = make_coords_xyz()
     assert len(d.coords.items()) == 3
     found = set()
     for dim in d.coords:
         found.add(str(dim))
-    assert found == set(['x', 'y', 'z'])
+    assert found == {'x', 'y', 'z'}
```

### Comparing `scipp-24.2.0/tests/lifetime_test.py` & `scipp-24.5.0/tests/lifetime_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,25 +46,25 @@
     assert (d + d).coords['x'].values[-1] == 9
     assert (d + d).coords['aux'].values[-1] == 9
 
 
 def test_lifetime_items_iter():
     var = sc.Variable(dims=['x'], values=np.arange(10))
     d = sc.Dataset(data={'a': var}, coords={'x': var, 'aux': var})
-    for _, item in (d + d).items():
+    for _, item in (d + d).items():  # noqa: PERF102
         assert sc.identical(item.data, var + var)
-    for _, coord in (d + d).coords.items():
+    for _, coord in (d + d).coords.items():  # noqa: PERF102
         assert sc.identical(coord, var)
-    for _, item in d['x', 1:5].items():
+    for _, item in d['x', 1:5].items():  # noqa: PERF102
         assert sc.identical(item.data, var['x', 1:5])
-    for _, coord in d['x', 1:5].coords.items():
+    for _, coord in d['x', 1:5].coords.items():  # noqa: PERF102
         assert sc.identical(coord, var['x', 1:5])
-    for _, item in (d + d)['x', 1:5].items():
+    for _, item in (d + d)['x', 1:5].items():  # noqa: PERF102
         assert sc.identical(item.data, (var + var)['x', 1:5])
-    for _, coord in (d + d)['x', 1:5].coords.items():
+    for _, coord in (d + d)['x', 1:5].coords.items():  # noqa: PERF102
         assert sc.identical(coord, var['x', 1:5])
 
 
 def test_lifetime_single_value():
     d = sc.Dataset(data={'a': sc.Variable(dims=['x'], values=np.arange(10))})
     var = sc.scalar(d)
     assert var.value['a'].values[-1] == 9
```

### Comparing `scipp-24.2.0/tests/linalg_test.py` & `scipp-24.5.0/tests/linalg_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,22 +111,14 @@
         var['x', 0] = vec + vec
     with pytest.raises(sc.VariableError):
         var.fields.x = 1.1 * sc.units.m
     assert not var.values.flags['WRITEABLE']
     assert not var.fields.x.values.flags['WRITEABLE']
 
 
-def test_matrix_from_quat_coeffs_list():
-    sc.geometry.rotation_matrix_from_quaternion_coeffs([1, 2, 3, 4])
-
-
-def test_matrix_from_quat_coeffs_numpy():
-    sc.geometry.rotation_matrix_from_quaternion_coeffs(np.arange(4))
-
-
 def test_elements_binned():
     data = sc.array(dims=['x'], values=[1, 2, 3, 4])
     var = sc.bins(dim='x', data=data)
     assert var.fields is None
 
     data = sc.vectors(dims=['x'], values=np.arange(6).reshape(2, 3))
     var = sc.bins(dim='x', data=data)
```

### Comparing `scipp-24.2.0/tests/lookup_test.py` & `scipp-24.5.0/tests/lookup_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import scipp as sc
 
 
 @pytest.mark.parametrize('mode', ['nearest', 'previous'])
 def test_raises_with_histogram_if_mode_set(mode):
     da = sc.DataArray(sc.arange('x', 4), coords={'x': sc.arange('x', 5)})
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Input is a histogram'):
         sc.lookup(da, mode=mode)
 
 
 @pytest.mark.parametrize("dtype", ['bool', 'int32', 'int64', 'float32', 'float64'])
 def test_histogram(dtype):
     x_lin = sc.linspace(dim='xx', start=0, stop=1, num=4)
     x = x_lin.copy()
```

### Comparing `scipp-24.2.0/tests/numpy_test.py` & `scipp-24.5.0/tests/numpy_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,10 +82,11 @@
 def test__array_ufunc___disabled(obj):
     with pytest.raises(TypeError, match="does not support ufuncs"):
         obj + a
     with pytest.raises(TypeError, match="unsupported operand type"):
         a * obj
     with pytest.raises(TypeError, match="does not support ufuncs"):
         obj += a
+
+    b = np.arange(2)
     with pytest.raises(TypeError, match="does not support ufuncs"):
-        b = np.arange(2)
         b += obj
```

### Comparing `scipp-24.2.0/tests/ownership_dataset_test.py` & `scipp-24.5.0/tests/ownership_dataset_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     ),
     ids=['dict', 'iterator', 'Coords'],
 )
 def masks_arg_wrapper(request):
     return request.param
 
 
-@pytest.fixture
+@pytest.fixture()
 def data_array_and_components(coords_arg_wrapper, attrs_arg_wrapper, masks_arg_wrapper):
     v, c, a, m = data_array_components()
     da = sc.DataArray(
         v,
         coords=coords_arg_wrapper('x', c),
         attrs=attrs_arg_wrapper('a', a),
         masks=masks_arg_wrapper('m', m),
@@ -247,15 +247,15 @@
     assert sc.identical(da_deepcopy, make_data_array()[0])
     assert sc.identical(da_methcopy, modified)
     assert sc.identical(da_methdeepcopy, make_data_array()[0])
 
 
 @pytest.mark.parametrize(
     'data_array_wrapper',
-    (lambda k, v: {k: v}, lambda k, v: {k: v}.items(), lambda k, v: sc.Dataset({k: v})),
+    [lambda k, v: {k: v}, lambda k, v: {k: v}.items(), lambda k, v: sc.Dataset({k: v})],
     ids=['dict', 'iterator', 'Dataset'],
 )
 def test_own_dset_init(data_array_wrapper):
     da, *_ = make_data_array()
     dset = sc.Dataset(data_array_wrapper('da1', da))
 
     dset['da1']['x', 0] = -10
```

### Comparing `scipp-24.2.0/tests/ownership_variable_test.py` & `scipp-24.5.0/tests/ownership_variable_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 
 def make_variable(data, variances=None, **kwargs):
     """
     Make a Variable with default dimensions from data
     while avoiding copies beyond what sc.Variable does.
     """
-    if isinstance(data, (list, tuple)):
+    if isinstance(data, list | tuple):
         data = np.array(data)
-    if variances is not None and isinstance(variances, (list, tuple)):
+    if variances is not None and isinstance(variances, list | tuple):
         variances = np.array(variances)
     if isinstance(data, np.ndarray):
         dims = ['x', 'y'][: np.ndim(data)]
         return sc.array(dims=dims, values=data, variances=variances, **kwargs)
     return sc.scalar(data, **kwargs)
```

### Comparing `scipp-24.2.0/tests/python_scalar_operations_test.py` & `scipp-24.5.0/tests/python_scalar_operations_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/readonly_test.py` & `scipp-24.5.0/tests/readonly_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,26 +36,26 @@
         assert not var['x', 1].variances.flags['WRITEABLE']
     with pytest.raises(sc.VariableError):
         var['x', 1] = var['x', 0]
     assert sc.identical(var, original)
 
 
 def assert_dict_writable(d):
-    key = list(d.keys())[0]
+    key = next(iter(d.keys()))
     del d[key]
     assert key not in d
     d['new'] = sc.scalar(4)
     assert 'new' in d
 
 
 def assert_dict_readonly(d, error=sc.DataArrayError):
     with pytest.raises(error):
         d['new'] = sc.scalar(4)
     assert 'new' not in d
-    key = list(d.keys())[0]
+    key = next(iter(d.keys()))
     with pytest.raises(error):
         del d[key]
     assert key in d
 
 
 def assert_readonly_data_array(da, readonly_data: bool):
     N = da.sizes['x']
```

### Comparing `scipp-24.2.0/tests/reduce_test.py` & `scipp-24.5.0/tests/reduce_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/rename_test.py` & `scipp-24.5.0/tests/rename_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/scipy/integrate_test.py` & `scipp-24.5.0/tests/scipy/integrate_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/scipy/interpolate/interp1d_test.py` & `scipp-24.5.0/tests/scipy/interpolate/interp1d_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/scipy/ndimage/footprint_filter_test.py` & `scipp-24.5.0/tests/scipy/ndimage/footprint_filter_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 import numpy as np
 import pytest
 import scipy.ndimage
 
 import scipp as sc
-from scipp.scipy.ndimage import (  # NOQA
+from scipp.scipy.ndimage import (
     generic_filter,
     maximum_filter,
     median_filter,
     minimum_filter,
     percentile_filter,
     rank_filter,
 )
@@ -70,15 +70,15 @@
     with pytest.raises(sc.VariancesError):
         filter_func(da, size=2)
 
 
 def test_raises_ValueError_when_data_has_masks(filter_func):
     da = make_histogram2d()
     da.masks['mask'] = da.coords['x'] == da.coords['x']
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='mask'):
         filter_func(da, size=2)
 
 
 def test_raises_TypeError_if_size_given_as_array_like(filter_func):
     da = make_histogram2d()
     with pytest.raises(TypeError):
         filter_func(da, size=[2, 3])
@@ -213,22 +213,22 @@
     assert sc.identical(result, reference)
 
 
 def test_attributes_are_propagated(simple_filter_func):
     da = make_histogram2d()
     da.attrs['attr'] = sc.scalar(1.2)
     result = simple_filter_func(da, size=2)
-    assert set(result.attrs) == set(['attr'])
+    assert set(result.attrs) == {'attr'}
     assert sc.identical(result.attrs['attr'], da.attrs['attr'])
 
 
 def test_coordinates_are_propagated(simple_filter_func):
     da = make_histogram2d()
     result = simple_filter_func(da, size=2)
-    assert set(result.coords) == set(['x', 'y'])
+    assert set(result.coords) == {'x', 'y'}
     assert sc.identical(result.coords['x'], da.coords['x'])
     assert sc.identical(result.coords['y'], da.coords['y'])
 
 
 def test_input_is_not_modified(simple_filter_func):
     original = make_histogram2d()
     da = original.copy()
```

### Comparing `scipp-24.2.0/tests/scipy/ndimage/gaussian_filter_test.py` & `scipp-24.5.0/tests/scipy/ndimage/gaussian_filter_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     with pytest.raises(sc.VariancesError):
         gaussian_filter(da, sigma=1.5)
 
 
 def test_raises_ValueError_when_data_has_masks():
     da = make_histogram2d()
     da.masks['mask'] = da.coords['x'] == da.coords['x']
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='mask'):
         gaussian_filter(da, sigma=1.5)
 
 
 def test_raises_TypeError_if_sigma_given_as_array_like():
     da = make_histogram2d()
     with pytest.raises(TypeError):
         gaussian_filter(da, sigma=[1.5, 2.5])
@@ -143,22 +143,22 @@
     assert sc.identical(result, reference)
 
 
 def test_attributes_are_propagated():
     da = make_histogram2d()
     da.attrs['attr'] = sc.scalar(1.2)
     result = gaussian_filter(da, sigma=3.4)
-    assert set(result.attrs) == set(['attr'])
+    assert set(result.attrs) == {'attr'}
     assert sc.identical(result.attrs['attr'], da.attrs['attr'])
 
 
 def test_coordinates_are_propagated():
     da = make_histogram2d()
     result = gaussian_filter(da, sigma=3.4)
-    assert set(result.coords) == set(['x', 'y'])
+    assert set(result.coords) == {'x', 'y'}
     assert sc.identical(result.coords['x'], da.coords['x'])
     assert sc.identical(result.coords['y'], da.coords['y'])
 
 
 def test_input_is_not_modified():
     original = make_histogram2d()
     da = original.copy()
```

### Comparing `scipp-24.2.0/tests/scipy/optimize/curve_fit_test.py` & `scipp-24.5.0/tests/scipy/optimize/curve_fit_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         curve_fit(func, array1d(), sigma=np.arange(4))
 
 
 def test_should_raise_ValueError_when_sigma_contains_zeros():
     da = array1d(size=50)
     da.variances = np.random.default_rng().normal(0.0, 0.1, size=50) ** 2
     da['xx', 21].variance = 0.0
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='0 in the input variances'):
         curve_fit(func, da)
 
 
 def test_does_not_raise_when_sigma_contains_zeros_that_is_masked():
     da = array1d(size=50)
     da.variances = np.random.default_rng().normal(0.0, 0.1, size=50) ** 2
     da.masks['m'] = sc.full(value=False, sizes=da.sizes)
@@ -136,15 +136,15 @@
         func, sc.concat([da[:mask_pos], da[mask_pos + mask_size :]], da.dim)
     )
     assert sc.identical(masked['a'], removed['a'])
     assert sc.identical(masked['b'], removed['b'])
 
 
 @pytest.mark.parametrize(
-    "variance,expected",
+    ('variance', 'expected'),
     [(1e9, 1.0), (1, 2.0), (1 / 3, 3.0), (1e-9, 5.0)],
     ids=['disabled', 'equal', 'high', 'dominant'],
 )
 def test_variances_determine_weights(variance, expected):
     x = sc.array(dims=['x'], values=[1, 2, 3, 4])
     y = sc.array(
         dims=['x'], values=[1.0, 5.0, 1.0, 1.0], variances=[1.0, 1.0, 1.0, 1.0]
@@ -282,9 +282,9 @@
 
 def test_can_pass_extra_kwargs():
     data = array1d()
 
     # Does not raise
     curve_fit(func, data, method='lm')
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='method'):
         curve_fit(func, data, method='bad_method')
```

### Comparing `scipp-24.2.0/tests/scipy/signal/butter_test.py` & `scipp-24.5.0/tests/scipy/signal/butter_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/scipy/signal/sosfiltfilt_test.py` & `scipp-24.5.0/tests/scipy/signal/sosfiltfilt_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/serialization_test.py` & `scipp-24.5.0/tests/serialization_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/setitem_test.py` & `scipp-24.5.0/tests/setitem_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/shape_test.py` & `scipp-24.5.0/tests/shape_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,19 +35,19 @@
     )
     assert sc.identical(sc.broadcast(da, sizes={'x': 6, 'y': 3}), expected)
     assert sc.identical(sc.broadcast(da, dims=['x', 'y'], shape=[6, 3]), expected)
 
 
 def test_broadcast_fails_with_bad_inputs():
     x = sc.array(dims=['x'], values=np.arange(6.0))
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='dims and shape must both be None'):
         _ = sc.broadcast(x, sizes={'x': 6, 'y': 3}, dims=['x', 'y'], shape=[6, 3])
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='dims and shape must both be None'):
         _ = sc.broadcast(x, sizes={'x': 6, 'y': 3}, dims=['x', 'y'])
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='dims and shape must both be None'):
         _ = sc.broadcast(x, sizes={'x': 6, 'y': 3}, shape=[6, 3])
 
 
 def test_concat():
     var = sc.scalar(1.0)
     assert sc.identical(
         sc.concat([var, var + var, 3 * var], 'x'),
@@ -120,17 +120,17 @@
     with pytest.raises(sc.DimensionError):
         sc.fold(da, dim='x', sizes={'x': -1, 'y': -1})
 
 
 def test_fold_raises_non_divisible():
     x = sc.array(dims=['x'], values=np.arange(10.0))
     da = sc.DataArray(x)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match=r'original shape \d+ cannot be divided by'):
         sc.fold(x, dim='x', sizes={'x': 3, 'y': -1})
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match=r'original shape \d+ cannot be divided by'):
         sc.fold(da, dim='x', sizes={'x': -1, 'y': 3})
 
 
 def test_flatten_variable():
     var = sc.arange('r', 6).fold('r', sizes={'a': 2, 'b': 3})
     assert sc.identical(sc.flatten(var, dims=['a', 'b'], to='f'), sc.arange('f', 6))
     assert sc.identical(sc.flatten(var, to='f'), sc.arange('f', 6))
```

### Comparing `scipp-24.2.0/tests/show_test.py` & `scipp-24.5.0/tests/show_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/slice_bins_test.py` & `scipp-24.5.0/tests/slice_bins_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -100,23 +100,25 @@
 
 
 def test_slice_bins_with_step_raises():
     da = sc.data.table_xyz(100).bin(x=10)
     start = sc.scalar(0.1, unit='m')
     stop = sc.scalar(0.4, unit='m')
     step = sc.scalar(0.1, unit='m')
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Label-based indexing with step'):
         da.bins['z', start:stop:step]
 
 
 def test_slice_bins_with_int_index_raises():
     da = sc.data.table_xyz(100).bin(x=10)
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError, match='Bins can only by sliced using label-based indexing'
+    ):
         da.bins['z', 1:4]
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Unsupported key'):
         da.bins['z', 1]
 
 
 def test_bins_slicing_open_start_too_small_stop_given():
     table = sc.data.table_xyz(nrow=100)
     da = table.bin(x=7)
     too_small_stop = da.bins.meta['x'].min() - 0.001 * sc.Unit('m')
```

### Comparing `scipp-24.2.0/tests/slice_by_condition_test.py` & `scipp-24.5.0/tests/slice_by_condition_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,16 +106,16 @@
     da.coords['edges'] = sc.concat([da.coords['xx'], da.coords['xx'][-1] + 1], 'xx')
     condition = sc.array(dims=['xx'], values=[True, False, True, True])
     assert sc.identical(da[condition], sc.concat([base['xx', 0], base['xx', 2:]], 'xx'))
 
 
 def test_non_boolean_condition_raises_DTypeError():
     var = make_var()
+    condition = (var < 3).to(dtype='int32')
     with pytest.raises(sc.DTypeError):
-        condition = (var < 3).to(dtype='int32')
         var[condition]
 
 
 def test_all_false_condition_with_wrong_dims_raises_DimensionError():
     var = make_var()
     condition = sc.array(dims=['not-in-var'], values=[False, False, False])
     with pytest.raises(sc.DimensionError):
@@ -155,42 +155,42 @@
     condition = sc.array(dims=['xx'], values=[False, True, False])
     with pytest.raises(sc.DimensionError):
         var[condition]
 
 
 def test_all_false_2d_condition_raises_DimensionError():
     var = make_var()
+    condition = var != var
     with pytest.raises(sc.DimensionError):
-        condition = var != var
         var[condition]
 
 
 def test_all_true_2d_condition_raises_DimensionError():
     # Strictly speaking this could be supported, but having this odd special case
     # work would likely add more confusion and bugs surfacing add surpising times.
     var = make_var()
+    condition = var == var
     with pytest.raises(sc.DimensionError):
-        condition = var == var
         var[condition]
 
 
 def test_2d_condition_raises_DimensionError():
     var = make_var()
+    condition = var < 3
     with pytest.raises(sc.DimensionError):
-        condition = var < 3
         var[condition]
 
 
 def test_0d_false_condition_raises_DimensionError():
     var = make_var()
+    condition = sc.scalar(False)
     with pytest.raises(sc.DimensionError):
-        condition = sc.scalar(False)
         var[condition]
 
 
 def test_0d_true_condition_raises_DimensionError():
     # Strictly speaking this could be supported, but having this odd special case
     # work would likely add more confusion and bugs surfacing add surpising times.
     var = make_var()
+    condition = sc.scalar(True)
     with pytest.raises(sc.DimensionError):
-        condition = sc.scalar(True)
         var[condition]
```

### Comparing `scipp-24.2.0/tests/slice_by_index_list_test.py` & `scipp-24.5.0/tests/slice_by_index_list_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/slice_test.py` & `scipp-24.5.0/tests/slice_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/slicebyvalue_test.py` & `scipp-24.5.0/tests/slicebyvalue_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,63 +182,63 @@
     var = sc.arange('x', 4)
     da = sc.DataArray(var, coords={'x': var})
     with pytest.raises(sc.DimensionError):
         da[sc.scalar(1) : sc.scalar(3)]
 
 
 @pytest.mark.parametrize(
-    'da, coord',
-    (
+    ('da', 'coord'),
+    [
         (sc.data.binned_x(8, 15), 'x'),
         *product(
             (
                 sc.DataArray(
                     sc.array(dims=('x', 'y'), values=np.random.randn(5, 10)),
                     coords={
                         'x': sc.arange('x', 5),
                         'y': sc.linspace('y', -1, 1, 10),
                     },
                 ),
             ),
             ('x', 'y'),
         ),
-    ),
+    ],
 )
 @pytest.mark.parametrize(
     's',
-    (
+    [
         (-2, 0),
         (-2, 0.1),
         (-2, 3.5),
         (-2, 10),
         (0, 0.1),
         (0, 3.5),
         (0, 10),
         (0.1, 3.5),
         (0.1, 10),
         (3.5, 10),
         (1, None),
         (None, 0.6),
         (None, None),
-    ),
+    ],
 )
 def test_label_based_index_to_positional_index(da, coord, s):
     s = slice(
         *(
             sc.scalar(v, unit=da.coords[coord].unit) if v is not None else None
             for v in s
         )
     )
     ind = label_based_index_to_positional_index(da.sizes, da.coords[coord], s)
     assert_identical(da[coord, s], da[ind])
 
 
 @pytest.mark.parametrize(
     'a',
-    (-2, 0, 0.1, 3.5, 10, 0.6),
+    [-2, 0, 0.1, 3.5, 10, 0.6],
 )
 def test_label_based_index_to_positional_index_scalar(a):
     da = sc.DataArray(
         sc.array(dims=('x', 'y'), values=np.random.randn(6, 10)),
         coords={
             'x': sc.array(dims=['x'], values=[-2, 0, 0.1, 0.6, 3.5, 10]),
             'y': sc.linspace('y', -1, 1, 10),
```

### Comparing `scipp-24.2.0/tests/spatial/affine_test.py` & `scipp-24.5.0/tests/spatial/affine_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/spatial/linear_transform_test.py` & `scipp-24.5.0/tests/spatial/linear_transform_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/spatial/rotation_test.py` & `scipp-24.5.0/tests/spatial/rotation_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,21 @@
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 from math import pi
 
 import numpy as np
 import pytest
 
 import scipp as sc
-from scipp.spatial import rotations_from_rotvecs  # NOQA
-from scipp.spatial import inv, rotation, rotation_as_rotvec, rotations
+from scipp.spatial import (
+    inv,
+    rotation,
+    rotation_as_rotvec,
+    rotations,
+    rotations_from_rotvecs,
+)
 
 
 def test_from_rotvec_bad_unit():
     with pytest.raises(sc.UnitError):
         rotations_from_rotvecs(sc.vector(value=[90, 0, 0], unit="m"))
```

### Comparing `scipp-24.2.0/tests/spatial/scaling_test.py` & `scipp-24.5.0/tests/spatial/scaling_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/spatial/translation_test.py` & `scipp-24.5.0/tests/spatial/translation_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/spatial/vector_test.py` & `scipp-24.5.0/tests/spatial/vector_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,12 +44,12 @@
         sc.spatial.as_vectors(v, v, sc.scalar(1.0, unit='s'))
     with pytest.raises(sc.UnitError):
         sc.spatial.as_vectors(v, sc.scalar(1.0, unit='s'), v)
     with pytest.raises(sc.UnitError):
         sc.spatial.as_vectors(sc.scalar(1.0, unit='s'), v, v)
 
 
-@pytest.mark.parametrize('dtype', ('float32', 'int64'))
+@pytest.mark.parametrize('dtype', ['float32', 'int64'])
 def test_as_vectors_does_not_require_float64(dtype):
     v = sc.scalar(1.0, unit='m', dtype=dtype)
     w = sc.scalar(1.0, unit='m', dtype='float64')
     assert sc.allclose(sc.spatial.as_vectors(v, v, v), sc.spatial.as_vectors(w, w, w))
```

### Comparing `scipp-24.2.0/tests/structured_test.py` & `scipp-24.5.0/tests/structured_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 
 
 def test_structured_fields_dict_like():
     assert 'x' in var.fields
     assert 'y' in var.fields
     assert 'z' in var.fields
     assert 't' not in var.fields
-    assert set(var.fields.keys()) == set(['x', 'y', 'z'])
+    assert set(var.fields.keys()) == {'x', 'y', 'z'}
     found = []
     for field in var.fields:
         found.append(field)
         assert sc.identical(var.fields[field], getattr(var.fields, field))
-    assert set(found) == set(['x', 'y', 'z'])
+    assert set(found) == {'x', 'y', 'z'}
     var2 = var.copy()
     var2.fields['x'] += 1.0 * sc.units.m
     assert sc.identical(var2, sc.vector(value=np.array([2, 2, 3]), unit=sc.units.m))
 
 
 def test_structured_fields_keys_values():
     keys = list(var.fields.keys())
     values = list(var.fields.values())
-    for items in [dict(zip(keys, values)), dict(var.fields.items())]:
+    for items in [dict(zip(keys, values, strict=True)), dict(var.fields.items())]:
         assert len(keys) == 3
         assert len(values) == 3
         assert sc.identical(items['x'], 1.0 * sc.units.m)
         assert sc.identical(items['y'], 2.0 * sc.units.m)
         assert sc.identical(items['z'], 3.0 * sc.units.m)
```

### Comparing `scipp-24.2.0/tests/testing/assertions_test.py` & `scipp-24.5.0/tests/testing/assertions_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,37 +19,37 @@
 
 pytest_mark_parameterize_assert_similar = pytest.mark.parametrize(
     'assert_similar',
     [assert_identical, assert_allclose_use_identical_if_nonnumerical_dtype],
 )
 
 
-@pytest.mark.parametrize('a', (3, -1.2, 'hjh wed', [], {4}))
+@pytest.mark.parametrize('a', [3, -1.2, 'hjh wed', [], {4}])
 def test_assert_similar_builtin_equal(a):
     assert_identical(deepcopy(a), deepcopy(a))
 
 
-@pytest.mark.parametrize('a', (3, -1.2, 'hjh wed', [], {4}))
-@pytest.mark.parametrize('b', (1, 0.2, 'll', [7], {}))
+@pytest.mark.parametrize('a', [3, -1.2, 'hjh wed', [], {4}])
+@pytest.mark.parametrize('b', [1, 0.2, 'll', [7], {}])
 def test_assert_similar_builtin_mismatch(a, b):
     with pytest.raises(AssertionError):
         assert_identical(a, b)
 
 
 @pytest_mark_parameterize_assert_similar
 @pytest.mark.parametrize(
     'a',
-    (
+    [
         sc.scalar(3),
         sc.scalar(7.12, variance=0.33, unit='m'),
         sc.scalar('jja ow=-'),
         sc.arange('u', 9.5, 13.0, 0.4),
         sc.linspace('ppl', 3.7, -99, 10, unit='kg'),
         sc.array(dims=['ww', 'gas'], values=[[np.nan], [3]]),
-    ),
+    ],
 )
 def test_assert_similar_variable_equal(assert_similar, a):
     assert_similar(deepcopy(a), deepcopy(a))
 
 
 @pytest_mark_parameterize_assert_similar
 def test_assert_similar_variable_dim_mismatch(
@@ -166,29 +166,29 @@
     with pytest.raises(AssertionError):
         assert_similar(b, a)
 
 
 @pytest_mark_parameterize_assert_similar
 @pytest.mark.parametrize(
     'a',
-    (
+    [
         sc.DataArray(sc.scalar(91, unit='F')),
         sc.DataArray(sc.scalar(6.4), coords={'g': sc.scalar(4)}),
         sc.DataArray(sc.scalar(6.4), attrs={'rat': sc.scalar(0.01)}),
         sc.DataArray(sc.scalar(6.4), masks={'m': sc.scalar(False)}),
         sc.DataArray(
             sc.arange('y', 6.1, unit='mm'),
             coords={'y': sc.arange('y', 6.1, unit='s') * 3, 'e': sc.arange('y', 8)},
             attrs={
                 'w': sc.scalar('wws'),
                 'qkk': sc.array(dims=['t'], values=[1.0, 2.0], variances=[0.0, 0.1]),
             },
             masks={'1': sc.arange('y', 7) < 4},
         ),
-    ),
+    ],
 )
 def test_assert_similar_data_arrays_equal(assert_similar, a):
     assert_similar(deepcopy(a), deepcopy(a))
 
 
 @pytest_mark_parameterize_assert_similar
 def test_assert_similar_data_array_data_mismatch(
@@ -339,29 +339,29 @@
         assert_similar(a, b)
     with pytest.raises(AssertionError):
         assert_similar(b, a)
 
 
 @pytest.mark.parametrize(
     'a',
-    (
+    [
         sc.Dataset({'f': sc.scalar(91, unit='F')}),
         sc.Dataset({'r': sc.scalar(6.4)}, coords={'g': sc.scalar(4)}),
         sc.Dataset({'2': sc.arange('u', 5)}),
         sc.Dataset(
             {
                 'yy': sc.DataArray(
                     sc.arange('w', 15).fold('w', {'i': 3, 'yy': 5}),
                     attrs={'a': sc.scalar([2, 3])},
                     masks={'m': sc.arange('yy', 5) < 2},
                 ),
             },
             coords={'i': sc.arange('w', 15).fold('w', {'i': 3, 'yy': 5})},
         ),
-    ),
+    ],
 )
 def test_assert_similar_datasets_equal(a):
     assert_identical(deepcopy(a), deepcopy(a))
 
 
 def test_assert_similar_dataset_data_key_mismatch():
     a = sc.Dataset({'a': sc.arange('t', 3)})
@@ -388,21 +388,21 @@
         assert_identical(a, b)
     with pytest.raises(AssertionError):
         assert_identical(b, a)
 
 
 @pytest.mark.parametrize(
     'a',
-    (
+    [
         sc.DataGroup(),
         sc.DataGroup({'hg': 4}),
         sc.DataGroup({'ii': sc.scalar(3.01, unit='s')}),
         sc.DataGroup({'Å': [5, 2], 'pl': sc.arange(';', 6)}),
         sc.DataGroup({'q': sc.DataGroup({'ik': sc.arange('ik', 2)})}),
-    ),
+    ],
 )
 def test_assert_similar_data_group_equal(a):
     assert_identical(deepcopy(a), deepcopy(a))
 
 
 def test_assert_similar_data_group_keys_mismatch():
     a = sc.DataGroup({'a': sc.arange('ook', 9)})
@@ -439,28 +439,28 @@
     with pytest.raises(AssertionError):
         assert_identical(b, a)
 
 
 @pytest_mark_parameterize_assert_similar
 @pytest.mark.parametrize(
     'buffer',
-    (
+    [
         sc.ones(sizes={'e': 10}, unit='counts'),
         sc.arange('.', 13, unit='m'),
         sc.DataArray(sc.zeros(sizes={'bm': 10}), coords={'bm': sc.arange('bm', 10)}),
-    ),
+    ],
 )
 @pytest.mark.parametrize(
     'indices',
-    (
+    [
         sc.array(dims=['lm'], values=[0, 3, 8, 10], dtype='int64', unit=None),
         sc.array(dims=['h'], values=[2, 4, 10], dtype='int64', unit=None),
         sc.array(dims=['lka'], values=[0, 6], dtype='int64', unit=None),
         sc.array(dims=['l we'], values=[], dtype='int64', unit=None),
-    ),
+    ],
 )
 def test_assert_similar_binned_variable_equal(assert_similar, buffer, indices):
     begin, end = indices[:-1], indices[1:]
     a = sc.bins(data=buffer, dim=buffer.dim, begin=begin, end=end)
     assert_similar(deepcopy(a), deepcopy(a))
 
 
@@ -473,25 +473,25 @@
     )
     assert_similar(deepcopy(da), deepcopy(da))
 
 
 @pytest_mark_parameterize_assert_similar
 @pytest.mark.parametrize(
     'buffer',
-    (
+    [
         sc.ones(sizes={'e': 10}, unit='counts'),
         sc.DataArray(sc.zeros(sizes={'bm': 10}), coords={'bm': sc.arange('bm', 10)}),
-    ),
+    ],
 )
 @pytest.mark.parametrize(
     'indices',
-    (
+    [
         sc.array(dims=['lm'], values=[0, 3, 8, 10], dtype='int64', unit=None),
         sc.array(dims=['l we'], values=[], dtype='int64', unit=None),
-    ),
+    ],
 )
 def test_assert_similar_binned_variable_unit_mismatch(assert_similar, buffer, indices):
     begin, end = indices[:-1], indices[1:]
     a = sc.bins(data=buffer, dim=buffer.dim, begin=begin, end=end)
     buffer = deepcopy(buffer)
     buffer.unit = 'm'
     b = sc.bins(data=buffer, dim=buffer.dim, begin=begin, end=end)
@@ -503,25 +503,25 @@
 
 @pytest.mark.parametrize(
     'assert_similar',
     [assert_identical, assert_allclose_use_identical_if_nonnumerical_dtype],
 )
 @pytest.mark.parametrize(
     'buffer',
-    (
+    [
         sc.ones(sizes={'e': 10}, unit='counts'),
         sc.DataArray(sc.zeros(sizes={'bm': 10}), coords={'bm': sc.arange('bm', 10)}),
-    ),
+    ],
 )
 @pytest.mark.parametrize(
     'indices',
-    (
+    [
         sc.array(dims=['lm'], values=[0, 3, 8, 10], dtype='int64', unit=None),
         sc.array(dims=['l we'], values=[2, 6], dtype='int64', unit=None),
-    ),
+    ],
 )
 def test_assert_similar_binned_variable_value_mismatch(assert_similar, buffer, indices):
     begin, end = indices[:-1], indices[1:]
     a = sc.bins(data=buffer, dim=buffer.dim, begin=begin, end=end)
     buffer = deepcopy(buffer)
     buffer[3] = -1
     b = sc.bins(data=buffer, dim=buffer.dim, begin=begin, end=end)
@@ -533,18 +533,18 @@
 
 @pytest.mark.parametrize(
     'assert_similar',
     [assert_identical, assert_allclose_use_identical_if_nonnumerical_dtype],
 )
 @pytest.mark.parametrize(
     'indices',
-    (
+    [
         sc.array(dims=['lm'], values=[0, 3, 8, 10], dtype='int64', unit=None),
         sc.array(dims=['l we'], values=[1, 6], dtype='int64', unit=None),
-    ),
+    ],
 )
 def test_assert_similar_binned_variable_coord_mismatch(assert_similar, indices):
     buffer = sc.DataArray(
         sc.zeros(sizes={'bm': 10}), coords={'bm': sc.arange('bm', 10)}
     )
     begin, end = indices[:-1], indices[1:]
     a = sc.bins(data=buffer, dim=buffer.dim, begin=begin, end=end)
@@ -617,25 +617,25 @@
 
 def difference_exceeding_tolerance(a, b, rtol):
     return rtol * np.sign(b - a) * np.maximum(np.abs(b), np.abs(a))
 
 
 @pytest.mark.parametrize(
     'a',
-    (
+    [
         sc.array(dims=['x'], values=[1000, -1, 0.001, -2.3]),
         sc.scalar(2.3),
         sc.scalar(-2.0, unit='m'),
         sc.DataArray(
             sc.ones(sizes={'rv': 9}),
             coords={'rv': sc.arange('rv', 9), 'j': sc.scalar(3.1)},
         ),
-    ),
+    ],
 )
-@pytest.mark.parametrize('rtol', (1e-8, 1e-5, 1e-3, 1e-1))
+@pytest.mark.parametrize('rtol', [1e-8, 1e-5, 1e-3, 1e-1])
 def test_allclose_different_tolerances(rtol, a):
     np.random.seed(321)
     rtol = sc.scalar(rtol, unit='dimensionless')
     b = a.copy()
     b.values += difference_within_tolerance(a.values, b.values, rtol.value)
     assert_allclose(a, b, rtol=rtol)
     b.values += difference_exceeding_tolerance(a.values, b.values, rtol.value)
```

### Comparing `scipp-24.2.0/tests/to_unit_test.py` & `scipp-24.5.0/tests/to_unit_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/unit_test.py` & `scipp-24.5.0/tests/unit_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 # @file
 # @author Simon Heybrock
 import copy
 
 import pytest
 
 import scipp as sc
-from scipp._scipp.core import units_identical as units_identical  # noqa
+from scipp._scipp.core import units_identical as units_identical
 
 
 @pytest.fixture(autouse=True)
-def clean_unit_aliases():
+def _clean_unit_aliases():
     sc.units.aliases.clear()
     yield
     sc.units.aliases.clear()
 
 
 def test_cannot_construct_unit_without_arguments():
     with pytest.raises(TypeError):
-        sc.Unit()  # noqa
+        sc.Unit()
 
 
 def test_default_unit():
     u = sc.Unit('')
     assert u == sc.units.dimensionless
 
 
@@ -42,25 +42,25 @@
     assert sc.Unit('us') == 'µs'
 
 
 def test_constructor_raises_with_bad_input():
     with pytest.raises(sc.UnitError):
         sc.Unit('abcdef')  # does not parse
     with pytest.raises(TypeError):
-        sc.Unit(5)  # type: ignore # neither str nor Unit
+        sc.Unit(5)  # type: ignore[call-arg] # neither str nor Unit
 
 
 def test_unit_str_format():
     assert str(sc.units.m) == 'm'
     assert str(sc.units.us) == 'µs'
 
 
-@pytest.mark.parametrize('u', (sc.units.angstrom, sc.Unit('angstrom')))
+@pytest.mark.parametrize('u', [sc.units.angstrom, sc.Unit('angstrom')])
 def test_angstrom_str_format(u):
-    assert str(u) in ('\u212B', '\u00C5')
+    assert str(u) in ('\u212b', '\u00c5')
 
 
 def test_unit_repr():
     assert repr(sc.Unit('dimensionless')) == 'Unit(1)'
     assert repr(sc.Unit('m')) == 'Unit(m)'
     assert repr(sc.Unit('uK/rad')) == 'Unit(1e-06*K*rad**-1)'
     assert repr(sc.Unit('m^2/s^3')) == 'Unit(m**2*s**-3)'
@@ -78,15 +78,15 @@
 def test_degC_square():
     two_degC = sc.scalar(2.0, unit='degC')
     assert two_degC**2 == sc.scalar(4.0, unit='degC^2')
     assert sc.sqrt(two_degC**2) == two_degC
 
 
 @pytest.mark.parametrize(
-    'u', ('m', 'kg', 's', 'A', 'cd', 'K', 'mol', 'counts', '$', 'rad')
+    'u', ['m', 'kg', 's', 'A', 'cd', 'K', 'mol', 'counts', '$', 'rad']
 )
 def test_unit_repr_uses_all_bases(u):
     assert repr(sc.Unit(u)) == f'Unit({u})'
     assert repr(sc.Unit(u) ** 2) == f'Unit({u}**2)'
 
 
 def test_unit_property_from_str():
@@ -109,34 +109,34 @@
 def test_default_unit_for_string_is_none():
     var = sc.scalar('abcdef')
     assert var.unit is None
 
 
 @pytest.mark.parametrize(
     'u_str',
-    (
+    [
         'one',
         'm',
         'count / s',
         '12.3 * m/A*kg^2/rad^3',
         'count',
         'decibels',
         'CXCUN[1]',
         'arbitraryunit',
         'EQXUN[1]',
         'Sv',
         'degC',
-    ),
+    ],
 )
 def test_dict_roundtrip(u_str):
     u = sc.Unit(u_str)
     assert units_identical(sc.Unit.from_dict(u.to_dict()), u)
 
 
-@pytest.mark.parametrize('unit_type', (str, sc.Unit))
+@pytest.mark.parametrize('unit_type', [str, sc.Unit])
 def test_unit_alias_overrides_str_formatting(unit_type):
     sc.units.aliases['clucks'] = unit_type('19.3 m*A')
     clucks = sc.Unit('19.3 m*A')
     assert str(clucks) == 'clucks'
     assert str(sc.Unit('one') / clucks) == '1/clucks'
     assert str(clucks**2) == 'clucks^2'
     assert str(clucks * sc.Unit('kg')) == 'clucks*kg'
@@ -198,21 +198,21 @@
     sc.units.aliases['angstrom'] = 'angstrom'
     assert sc.Unit('angstrom') == '10**-10 m'
 
 
 def test_defining_conflicting_alias_raises():
     sc.units.aliases['speed'] = 'm/s'
     sc.units.aliases['zoomy'] = 'm/ms'
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='There already is an alias'):
         sc.units.aliases['fastness'] = 'm/s'
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='There already is an alias'):
         sc.units.aliases['fastness'] = '100*cm/s'
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='There already is an alias'):
         sc.units.aliases['fastness'] = sc.scalar(1000, unit='mm/s')
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='There already is an alias'):
         sc.units.aliases['zoomy'] = 'm/s'
     assert 'fastness' not in sc.units.aliases
 
 
 def test_can_remove_unit_alias():
     sc.units.aliases['clucks'] = '19.3 m*A'
     sc.units.aliases['dogyear'] = '4492800s'
```

### Comparing `scipp-24.2.0/tests/utils/collapse_and_slices_test.py` & `scipp-24.5.0/tests/utils/collapse_and_slices_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,25 +41,25 @@
     assert sc.identical(collapsed['y:1-x:1'], d['sample']['y', 1]['x', 1])
 
 
 def test_collapse_dataset():
     d = make_dataset()
     collapsed = sc.collapse(d, keep='tof')
     # In a Dataset, the order of the dims is not fixed
-    first_key = list(collapsed.keys())[0]
+    first_key = next(iter(collapsed.keys()))
     if first_key.startswith('x'):
         dim1 = 'x'
         dim2 = 'y'
     else:
         dim1 = 'y'
         dim2 = 'x'
-    assert sc.identical(collapsed['{}:0-{}:0'.format(dim1, dim2)], d[dim2, 0][dim1, 0])
-    assert sc.identical(collapsed['{}:0-{}:1'.format(dim1, dim2)], d[dim2, 1][dim1, 0])
-    assert sc.identical(collapsed['{}:1-{}:0'.format(dim1, dim2)], d[dim2, 0][dim1, 1])
-    assert sc.identical(collapsed['{}:1-{}:1'.format(dim1, dim2)], d[dim2, 1][dim1, 1])
+    assert sc.identical(collapsed[f'{dim1}:0-{dim2}:0'], d[dim2, 0][dim1, 0])
+    assert sc.identical(collapsed[f'{dim1}:0-{dim2}:1'], d[dim2, 1][dim1, 0])
+    assert sc.identical(collapsed[f'{dim1}:1-{dim2}:0'], d[dim2, 0][dim1, 1])
+    assert sc.identical(collapsed[f'{dim1}:1-{dim2}:1'], d[dim2, 1][dim1, 1])
 
 
 def test_slices_data_array():
     d = make_dataset()
     collapsed = sc.slices(d['sample'], dim='x')
     assert sc.identical(collapsed['x:0'], d['sample']['x', 0])
     assert sc.identical(collapsed['x:1'], d['sample']['x', 1])
```

### Comparing `scipp-24.2.0/tests/utils/comparison_test.py` & `scipp-24.5.0/tests/utils/comparison_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/utils/to_string_test.py` & `scipp-24.5.0/tests/utils/to_string_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/variable_creation_test.py` & `scipp-24.5.0/tests/variable_creation_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     value = 'temp'
     var = sc.scalar(value)
     expected = sc.Variable(dims=(), values=value)
     assert sc.identical(var, expected)
 
 
 def test_scalar_throws_if_wrong_dtype_provided_for_str_types():
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Cannot convert values'):
         sc.scalar(value='temp', unit=sc.units.one, dtype=sc.DType.float64)
 
 
 def test_scalar_throws_UnitError_if_not_parsable():
     with pytest.raises(sc.UnitError):
         sc.scalar(value=1, unit='abcdef')
 
@@ -82,16 +82,16 @@
 
 def test_index_unit_is_none():
     i = sc.index(5)
     assert i.unit is None
 
 
 def test_index_raises_if_unit_given():
-    with pytest.raises(TypeError):
-        sc.index(5, unit='')  # type: ignore
+    with pytest.raises(TypeError, match='unexpected keyword argument'):
+        sc.index(5, unit='')  # type: ignore[call-arg]
 
 
 def test_zeros_creates_variable_with_correct_dims_and_shape():
     var = sc.zeros(dims=['x', 'y', 'z'], shape=[1, 2, 3])
     expected = sc.Variable(dims=['x', 'y', 'z'], values=np.zeros([1, 2, 3]))
     assert sc.identical(var, expected)
 
@@ -165,15 +165,15 @@
 
 def test_ones_dtypes():
     for dtype in (int, float, bool):
         assert sc.ones(dims=(), shape=(), dtype=dtype).value == dtype(1)
     assert sc.ones(
         dims=(), shape=(), unit='s', dtype='datetime64'
     ).value == np.datetime64(1, 's')
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='string'):
         sc.ones(dims=(), shape=(), dtype=str)
 
 
 def test_full_float_default_unit_is_dimensionless():
     var = sc.full(dims=(), shape=(), value=1.2)
     assert var.unit == sc.units.one
 
@@ -364,15 +364,15 @@
         raise NotImplementedError()
 
 
 @pytest.mark.parametrize(
     'ndim_and_slice_dim',
     [(ndim, slice_dim) for ndim in range(1, 7) for slice_dim in range(ndim)],
 )
-@pytest.mark.parametrize('step', (2, -1, -2))
+@pytest.mark.parametrize('step', [2, -1, -2])
 def test_array_nd_sliced_c_layout(ndim_and_slice_dim, step):
     ndim, slice_dim = ndim_and_slice_dim
     shape = list(range(2, ndim + 2))
     values = np.arange(np.prod(shape)).reshape(shape)
     values = slice_array_in_dim(values, slice_dim, step)
     var = sc.array(dims=[f'dim_{d}' for d in range(ndim)], values=values)
     assert var.ndim == ndim
@@ -385,15 +385,15 @@
     [
         (ndim, slice_dim0, slice_dim1)
         for ndim in range(1, 7)
         for slice_dim0 in range(ndim)
         for slice_dim1 in range(ndim)
     ],
 )
-@pytest.mark.parametrize('step', (2, -1, -2))
+@pytest.mark.parametrize('step', [2, -1, -2])
 def test_array_nd_sliced_twice_c_layout(ndim_and_slice_dims, step):
     ndim, slice_dim0, slice_dim1 = ndim_and_slice_dims
     shape = list(range(2, ndim + 2))
     values = np.arange(np.prod(shape)).reshape(shape)
     values = slice_array_in_dim(
         slice_array_in_dim(values, slice_dim0, step), slice_dim1, step
     )
@@ -403,15 +403,15 @@
     np.testing.assert_array_equal(var.values, values)
 
 
 @pytest.mark.parametrize(
     'ndim_and_slice_dim',
     [(ndim, slice_dim) for ndim in range(1, 7) for slice_dim in range(ndim)],
 )
-@pytest.mark.parametrize('step', (2, -1, -2))
+@pytest.mark.parametrize('step', [2, -1, -2])
 def test_array_nd_sliced_fortran_layout(ndim_and_slice_dim, step):
     ndim, slice_dim = ndim_and_slice_dim
     shape = list(range(2, ndim + 2))
     values = np.arange(np.prod(shape)).reshape(shape)
     values = np.asfortranarray(values)
     values = slice_array_in_dim(values, slice_dim, step)
     var = sc.array(dims=[f'dim_{d}' for d in range(ndim)], values=values)
@@ -425,15 +425,15 @@
     [
         (ndim, slice_dim0, slice_dim1)
         for ndim in range(1, 7)
         for slice_dim0 in range(ndim)
         for slice_dim1 in range(ndim)
     ],
 )
-@pytest.mark.parametrize('step', (2, -1, -2))
+@pytest.mark.parametrize('step', [2, -1, -2])
 def test_array_nd_sliced_twice_fortran_layout(ndim_and_slice_dims, step):
     ndim, slice_dim0, slice_dim1 = ndim_and_slice_dims
     shape = list(range(2, ndim + 2))
     values = np.arange(np.prod(shape)).reshape(shape)
     values = np.asfortranarray(values)
     values = slice_array_in_dim(
         slice_array_in_dim(values, slice_dim0, step), slice_dim1, step
@@ -557,31 +557,31 @@
 
 def test_linspace_none_unit():
     assert sc.linspace('x', 1.2, 103.0, 51, unit=None).unit is None
 
 
 @pytest.mark.parametrize(
     'range_fns',
-    (
+    [
         (sc.linspace, np.linspace),
         (sc.geomspace, np.geomspace),
         (sc.logspace, np.logspace),
-    ),
+    ],
     ids=('linspace', 'geomspace', 'logspace'),
 )
 def test_xyzspace_with_variables(range_fns):
     sc_fn, np_fn = range_fns
     var = sc_fn('x', sc.scalar(1.0), sc.scalar(5.0), 4)
     values = np_fn(1.0, 5.0, 4)
     assert sc.identical(var, sc.array(dims=['x'], values=values))
 
 
 @pytest.mark.parametrize(
     'range_fns',
-    ((sc.linspace, np.linspace), (sc.geomspace, np.geomspace)),
+    [(sc.linspace, np.linspace), (sc.geomspace, np.geomspace)],
     ids=('linspace', 'geomspace'),
 )
 def test_xyzspace_with_variables_set_unit(range_fns):
     sc_fn, np_fn = range_fns
     var = sc_fn(
         'x', sc.scalar(1.0, unit='m'), sc.scalar(5000.0, unit='mm'), 4, unit='m'
     )
@@ -592,36 +592,36 @@
 def test_logspace_with_variables_set_unit():
     assert sc.identical(
         sc.logspace('x', sc.scalar(1.0), sc.scalar(3.0), 3, unit='m'),
         sc.array(dims=['x'], values=[10.0, 100.0, 1000.0], unit='m'),
     )
 
 
-@pytest.mark.parametrize('unit', (sc.units.default_unit, 'one', 'm'))
+@pytest.mark.parametrize('unit', [sc.units.default_unit, 'one', 'm'])
 def test_logspace_with_variables_input_must_be_dimensionless(unit):
     with pytest.raises(sc.UnitError):
         sc.logspace('x', sc.scalar(1.0), sc.scalar(3.0, unit='m'), 4, unit=unit)
     with pytest.raises(sc.UnitError):
         sc.logspace('x', sc.scalar(1.0, unit='m'), sc.scalar(3.0), 4, unit=unit)
     with pytest.raises(sc.UnitError):
         sc.logspace(
             'x', sc.scalar(1.0, unit='m'), sc.scalar(3.0, unit='m'), 4, unit=unit
         )
 
 
 @pytest.mark.parametrize(
     'range_fn',
-    (sc.linspace, sc.geomspace, sc.logspace),
+    [sc.linspace, sc.geomspace, sc.logspace],
     ids=('linspace', 'geomspace', 'logspace'),
 )
 def test_xyzspace_with_variables_num_cannot_be_variable(range_fn):
     start = sc.scalar(1)
     stop = sc.scalar(3)
     with pytest.raises(TypeError):
-        range_fn('x', start, stop, sc.scalar(3))  # type: ignore
+        range_fn('x', start, stop, sc.scalar(3))
 
 
 def test_logspace():
     values = np.logspace(2.0, 3.0, num=4)
     var = sc.logspace('y', 2.0, 3.0, num=4, unit='s')
     expected = sc.Variable(dims=['y'], values=values, unit='s', dtype=sc.DType.float64)
     assert sc.identical(var, expected)
@@ -667,15 +667,15 @@
     with pytest.raises(TypeError):
         sc.arange(
             't', '2022-08-02T06:42:45', '2022-08-02T06:43:33', 16, dtype='datetime64'
         )
 
 
 def test_arange_datetime_from_str_raises_given_string_with_timezone():
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='timezone'):
         sc.arange(
             't',
             '2022-08-02T06:42:45Z',
             '2022-08-02T06:43:33Z',
             16 * sc.Unit('s'),
             dtype='datetime64',
         )
@@ -708,15 +708,15 @@
         dims=['t'],
         values=['2013-04-25T14:09:11', '2013-04-25T14:10:13', '2013-04-25T14:11:15'],
         unit='s',
     )
     assert sc.identical(var, expected)
 
 
-@pytest.mark.parametrize('unit', ('one', sc.units.default_unit))
+@pytest.mark.parametrize('unit', ['one', sc.units.default_unit])
 def test_arange_with_variables(unit):
     start = sc.scalar(1)
     stop = sc.scalar(4)
     step = sc.scalar(1)
     assert sc.identical(
         sc.arange('x', start, stop, step, unit=unit),
         sc.array(dims=['x'], values=[1, 2, 3], unit='one', dtype='int64'),
@@ -817,17 +817,17 @@
 
 def test_arange_with_variables_mixed_types_not_allowed():
     start = sc.scalar(1, unit='m')
     stop = 4
     step = sc.scalar(1, unit='m')
     unit = 'm'
     with pytest.raises(TypeError):
-        sc.arange('x', start, stop, step)  # type: ignore
+        sc.arange('x', start, stop, step)  # type: ignore[type-var]
     with pytest.raises(TypeError):
-        sc.arange('x', start, stop, step, unit=unit)  # type: ignore
+        sc.arange('x', start, stop, step, unit=unit)  # type: ignore[type-var]
 
 
 def test_arange_with_variables_requires_scalar():
     with pytest.raises(sc.DimensionError):
         sc.arange('x', sc.array(dims=['x'], values=[1, 2]))
     with pytest.raises(sc.DimensionError):
         sc.arange('x', sc.scalar(1), sc.array(dims=['x'], values=[1, 2]))
@@ -852,30 +852,30 @@
     )
     assert sc.identical(
         sc.arange('x', sc.scalar(1), sc.scalar(4.0), sc.scalar(1), dtype='int64'),
         sc.array(dims=['x'], values=[1, 2, 3], dtype='int64'),
     )
 
 
-@pytest.mark.parametrize('dtype', (np.int32, np.int64, np.float32, np.float64))
+@pytest.mark.parametrize('dtype', [np.int32, np.int64, np.float32, np.float64])
 def test_arange_with_uniform_numpy_arg_dtype_creates_array_with_same_dtype(dtype):
     assert sc.identical(
         sc.arange('x', dtype(2)), sc.array(dims=['x'], values=[0, 1], dtype=dtype)
     )
     assert sc.identical(
         sc.arange('x', dtype(2), dtype(4)),
         sc.array(dims=['x'], values=[2, 3], dtype=dtype),
     )
     assert sc.identical(
         sc.arange('x', dtype(2), dtype(4), dtype(2)),
         sc.array(dims=['x'], values=[2], dtype=dtype),
     )
 
 
-@pytest.mark.parametrize('dtype', (np.int32, np.int64, np.float32, np.float64))
+@pytest.mark.parametrize('dtype', [np.int32, np.int64, np.float32, np.float64])
 def test_arange_with_uniform_scipp_arg_dtype_creates_array_with_same_dtype(dtype):
     assert sc.identical(
         sc.arange('x', sc.scalar(2, dtype=dtype)),
         sc.array(dims=['x'], values=[0, 1], dtype=dtype),
     )
     assert sc.identical(
         sc.arange('x', sc.scalar(2, dtype=dtype), sc.scalar(4, dtype=dtype)),
@@ -890,20 +890,20 @@
         ),
         sc.array(dims=['x'], values=[2], dtype=dtype),
     )
 
 
 @pytest.mark.parametrize(
     ('dtype', 'larger'),
-    (
+    [
         (np.int32, np.int64),
         (np.float32, np.float64),
         (np.int32, np.float64),
         (np.int64, np.float64),
-    ),
+    ],
 )
 def test_arange_with_non_uniform_arg_dtype_creates_array_with_larger_dtype(
     dtype, larger
 ):
     assert sc.identical(
         sc.arange('x', dtype(2), larger(4)),
         sc.array(dims=['x'], values=[2, 3], dtype=larger),
@@ -926,49 +926,52 @@
     )
 
 
 def test_zeros_sizes():
     dims = ['x', 'y', 'z']
     shape = [2, 3, 4]
     assert sc.identical(
-        sc.zeros(dims=dims, shape=shape), sc.zeros(sizes=dict(zip(dims, shape)))
+        sc.zeros(dims=dims, shape=shape),
+        sc.zeros(sizes=dict(zip(dims, shape, strict=True))),
     )
-    with pytest.raises(ValueError):
-        sc.zeros(dims=dims, shape=shape, sizes=dict(zip(dims, shape)))
+    with pytest.raises(ValueError, match='dims and shape must both be None'):
+        sc.zeros(dims=dims, shape=shape, sizes=dict(zip(dims, shape, strict=True)))
 
 
 def test_ones_sizes():
     dims = ['x', 'y', 'z']
     shape = [2, 3, 4]
     assert sc.identical(
-        sc.ones(dims=dims, shape=shape), sc.ones(sizes=dict(zip(dims, shape)))
+        sc.ones(dims=dims, shape=shape),
+        sc.ones(sizes=dict(zip(dims, shape, strict=True))),
     )
-    with pytest.raises(ValueError):
-        sc.ones(dims=dims, shape=shape, sizes=dict(zip(dims, shape)))
+    with pytest.raises(ValueError, match='dims and shape must both be None'):
+        sc.ones(dims=dims, shape=shape, sizes=dict(zip(dims, shape, strict=True)))
 
 
 def test_empty_sizes():
     dims = ['x', 'y', 'z']
     shape = [2, 3, 4]
     _compare_properties(
-        sc.empty(dims=dims, shape=shape), sc.empty(sizes=dict(zip(dims, shape)))
+        sc.empty(dims=dims, shape=shape),
+        sc.empty(sizes=dict(zip(dims, shape, strict=True))),
     )
-    with pytest.raises(ValueError):
-        sc.empty(dims=dims, shape=shape, sizes=dict(zip(dims, shape)))
+    with pytest.raises(ValueError, match='dims and shape must both be None'):
+        sc.empty(dims=dims, shape=shape, sizes=dict(zip(dims, shape, strict=True)))
 
 
 @pytest.mark.parametrize('timezone', ['Z', '-05:00', '+02'])
 def test_datetime_raises_given_string_with_timezone(timezone):
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='timezone'):
         sc.datetime(f'2152-11-25T13:13:46{timezone}')
 
 
 @pytest.mark.parametrize('timezone', ['Z', '-05:00', '+02'])
 def test_datetimes_raises_given_string_with_timezone(timezone):
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='timezone'):
         sc.datetimes(dims=['time'], values=[f'2152-11-25T13:13:46{timezone}'], unit='s')
 
 
 def test_datetime():
     assert sc.identical(
         sc.datetime('1970', unit='Y'), sc.scalar(np.datetime64('1970', 'Y'))
     )
```

### Comparing `scipp-24.2.0/tests/variable_init_test.py` & `scipp-24.5.0/tests/variable_init_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     (sc.DType.int32, sc.DType.int32, 2),
     (sc.DType.int64, sc.DType.int64, 3),
     (sc.DType.float32, sc.DType.float32, 4.5),
     (sc.DType.float64, sc.DType.float64, 5.6),
     (sc.DType.bool, sc.DType.bool, False),
     (sc.DType.string, sc.DType.string, 'def'),
     (sc.DType.datetime64, sc.DType.datetime64, 123),
-    (sc.DType.PyObject, sc.DType.PyObject, dict()),
+    (sc.DType.PyObject, sc.DType.PyObject, {}),
     (np.int32, sc.DType.int32, 6),
     (np.int64, sc.DType.int64, 7),
     (np.float32, sc.DType.float32, 8.9),
     (np.float64, sc.DType.float64, 9.1),
     (np.dtype(bool), sc.DType.bool, True),
     (np.dtype(str), sc.DType.string, 'ghi'),
     (np.dtype('datetime64'), sc.DType.datetime64, 456),
@@ -87,30 +87,30 @@
     assert var.dims == ()
     assert var.ndim == 0
     assert var.dtype == sc.DType.float64
     assert var.unit == sc.units.dimensionless
 
 
 @pytest.mark.parametrize(
-    'args', ((sc.DType.int64, 1), (sc.DType.bool, True), (sc.DType.string, 'a'))
+    'args', [(sc.DType.int64, 1), (sc.DType.bool, True), (sc.DType.string, 'a')]
 )
 def test_create_scalar_with_value(args):
     dtype, value = args
     var = sc.Variable(dims=(), values=value)
     assert var.value == value
     assert var.dims == ()
     assert var.ndim == 0
     assert var.dtype == dtype
     if dtype in (sc.DType.string, sc.DType.bool):
         assert var.unit is None
     else:
         assert var.unit == sc.units.one
 
 
-@pytest.mark.parametrize('args', ((sc.DType.bool, True), (sc.DType.string, 'a')))
+@pytest.mark.parametrize('args', [(sc.DType.bool, True), (sc.DType.string, 'a')])
 def test_create_scalar_with_value_array(args):
     dtype, value = args
     var = sc.Variable(dims=(), values=np.array(value))
     assert var.value == value
     assert var.dims == ()
     assert var.ndim == 0
     assert var.dtype == dtype
@@ -139,15 +139,15 @@
     var = v['x', 0].copy()
     var.unit = sc.units.m
     assert sc.identical(var, np.float32(0.0) * sc.units.m)
     var.unit = sc.units.m ** (-1)
     assert sc.identical(var, np.float32(0.0) / sc.units.m)
 
 
-@pytest.mark.parametrize('variance', (1, True, 'a', sc.Variable(dims=(), values=1.2)))
+@pytest.mark.parametrize('variance', [1, True, 'a', sc.Variable(dims=(), values=1.2)])
 def test_create_scalar_invalid_variance(variance):
     with pytest.raises(sc.VariancesError):
         sc.Variable(dims=(), variances=variance)
 
 
 @pytest.mark.parametrize(
     "unit",
@@ -186,130 +186,130 @@
     for dtype, expected, val in DTYPE_INPUT_TO_EXPECTED:
         unit = 'ns' if expected == sc.DType.datetime64 else 'one'
         assert sc.scalar(val, dtype=dtype, unit=unit).dtype == expected
 
 
 @pytest.mark.parametrize(
     "val_and_dtype",
-    (
+    [
         (np.int32(2), 'int32'),
         (np.int64(42), 'int64'),
         (np.float32(5.4), 'float32'),
         (np.float64(9.9), 'float64'),
         (np.bool_(True), 'bool'),
-    ),
+    ],
 )
 def test_create_scalar_numpy_type(val_and_dtype):
     val, dtype = val_and_dtype
     assert sc.scalar(val).dtype == dtype
 
 
-@pytest.mark.parametrize("dtype", (None, sc.DType.Variable, sc.Variable))
+@pytest.mark.parametrize("dtype", [None, sc.DType.Variable, sc.Variable])
 def test_create_scalar_dtype_Variable(dtype):
     elem = sc.Variable(dims=['x'], values=np.arange(4.0))
     var = sc.Variable(dims=(), values=elem, dtype=dtype)
     assert sc.identical(var.value, elem)
     assert var.dims == ()
     assert var.ndim == 0
     assert var.dtype == sc.DType.Variable
     assert var.unit is None
     var = sc.Variable(dims=(), values=elem['x', 1:3], dtype=dtype)
     assert var.dtype == sc.DType.Variable
 
 
-@pytest.mark.parametrize("dtype", (None, sc.DType.DataArray, sc.DataArray))
+@pytest.mark.parametrize("dtype", [None, sc.DType.DataArray, sc.DataArray])
 def test_create_scalar_dtype_DataArray(dtype):
     elem = sc.DataArray(data=sc.Variable(dims=['x'], values=np.arange(4.0)))
     var = sc.Variable(dims=(), values=elem, dtype=dtype)
     assert sc.identical(var.value, elem)
     assert var.dims == ()
     assert var.ndim == 0
     assert var.dtype == sc.DType.DataArray
     assert var.unit is None
     var = sc.Variable(dims=(), values=elem['x', 1:3], dtype=dtype)
     assert var.dtype == sc.DType.DataArray
 
 
-@pytest.mark.parametrize("dtype", (None, sc.DType.Dataset, sc.Dataset))
+@pytest.mark.parametrize("dtype", [None, sc.DType.Dataset, sc.Dataset])
 def test_create_scalar_dtype_Dataset(dtype):
     elem = sc.Dataset(data={'a': sc.Variable(dims=['x'], values=np.arange(4.0))})
     var = sc.Variable(dims=(), values=elem, dtype=dtype)
     assert sc.identical(var.value, elem)
     assert var.dims == ()
     assert var.ndim == 0
     assert var.dtype == sc.DType.Dataset
     assert var.unit is None
     var = sc.Variable(dims=(), values=elem['x', 1:3], dtype=dtype)
     assert var.dtype == sc.DType.Dataset
 
 
 @pytest.mark.parametrize(
     "dtype",
-    (
+    [
         1,
         2.3,
         'string',
         sc.scalar(0),
         sc.DataArray(sc.scalar(1)),
         sc.Dataset({'a': sc.scalar(3)}),
-    ),
+    ],
 )
 def test_create_scalar_with_instance_as_dtype(dtype):
     with pytest.raises(TypeError):
         sc.Variable(dims=(), values=dtype, dtype=dtype)
 
 
-@pytest.mark.parametrize("dtype", (str, sc.Variable, sc.DataArray, sc.Dataset))
+@pytest.mark.parametrize("dtype", [str, sc.Variable, sc.DataArray, sc.Dataset])
 def test_create_scalar_value_must_be_convertible_to_dtype(dtype):
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Cannot convert values'):
         sc.Variable(dims=(), values=0, dtype=dtype)
 
 
-@pytest.mark.parametrize('value', (1, 1.2, True))
-@pytest.mark.parametrize('dtype', (np.int32, np.int64, np.float32, np.float64, bool))
+@pytest.mark.parametrize('value', [1, 1.2, True])
+@pytest.mark.parametrize('dtype', [np.int32, np.int64, np.float32, np.float64, bool])
 def test_create_scalar_conversion(value, dtype):
     converted = np.array(value, dtype=dtype).item()
     var = sc.Variable(dims=(), values=value, dtype=dtype)
     assert var.value == converted
 
 
-@pytest.mark.parametrize('value', (1, 1.2, True))
-@pytest.mark.parametrize('dtype', (sc.DType.string, sc.DType.Variable))
+@pytest.mark.parametrize('value', [1, 1.2, True])
+@pytest.mark.parametrize('dtype', [sc.DType.string, sc.DType.Variable])
 def test_create_scalar_invalid_conversion_numeric(value, dtype):
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Cannot convert values'):
         sc.Variable(dims=(), values=value, dtype=dtype)
 
 
 @pytest.mark.parametrize(
-    'dtype', (sc.DType.int32, sc.DType.int64, sc.DType.float64, sc.DType.Variable)
+    'dtype', [sc.DType.int32, sc.DType.int64, sc.DType.float64, sc.DType.Variable]
 )
 def test_create_scalar_invalid_conversion_str(dtype):
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Cannot convert values'):
         sc.Variable(dims=(), values='abc', dtype=dtype)
 
 
 def test_create_1d_size_4():
     var = sc.Variable(dims=['x'], values=np.arange(4.0), unit=sc.units.m)
     assert var.shape == (4,)
     np.testing.assert_array_equal(var.values, [0, 1, 2, 3])
     assert var.dims == ('x',)
     assert var.ndim == 1
     assert var.dtype == sc.DType.float64
     assert var.unit == sc.units.m
 
 
-@pytest.mark.parametrize('values_type', (tuple, list, np.array))
+@pytest.mark.parametrize('values_type', [tuple, list, np.array])
 @pytest.mark.parametrize(
     'dtype_and_values',
-    (
+    [
         (sc.DType.int64, [1, 2]),
         (sc.DType.float64, [1.2, 3.4]),
         (sc.DType.bool, [True, False]),
         (sc.DType.string, ['a', 'bc']),
-    ),
+    ],
 )
 def test_create_1d_dtype(values_type, dtype_and_values):
     def check(v):
         if dtype == sc.DType.int64:
             # The dtype varies between Windows and Linux / MacOS.
             assert v.dtype in (sc.DType.int32, sc.DType.int64)
         else:
@@ -339,34 +339,34 @@
     assert var.dtype == sc.DType.float32
     var = sc.Variable(dims=['x'], values=np.arange(4), dtype=np.dtype(np.int64))
     assert var.dtype == sc.DType.int64
     var = sc.Variable(dims=['x'], values=np.arange(4), dtype=np.dtype(np.int32))
     assert var.dtype == sc.DType.int32
 
 
-@pytest.mark.parametrize('values_type', (tuple, list, np.array))
+@pytest.mark.parametrize('values_type', [tuple, list, np.array])
 def test_create_1d_values_array_like(values_type):
     values = np.arange(5.0)
     var = sc.Variable(dims=['x'], values=values_type(values))
     assert var.dtype == sc.DType.float64
     np.testing.assert_array_equal(var.values, values)
     assert var.variances is None
 
 
-@pytest.mark.parametrize('variances_type', (tuple, list, np.array))
+@pytest.mark.parametrize('variances_type', [tuple, list, np.array])
 def test_create_1d_variances_array_like(variances_type):
     variances = np.arange(5.0)
     var = sc.Variable(dims=['x'], variances=variances_type(variances))
     assert var.dtype == sc.DType.float64
     np.testing.assert_array_equal(var.values, np.zeros_like(variances))
     np.testing.assert_array_equal(var.variances, variances)
 
 
-@pytest.mark.parametrize('values_type', (tuple, list, np.array))
-@pytest.mark.parametrize('variances_type', (tuple, list, np.array))
+@pytest.mark.parametrize('values_type', [tuple, list, np.array])
+@pytest.mark.parametrize('variances_type', [tuple, list, np.array])
 def test_create_1d_values_and_variances_array_like(values_type, variances_type):
     values = np.arange(5.0)
     variances = np.arange(5.0) * 0.1
     var = sc.Variable(
         dims=['x'], values=values_type(values), variances=variances_type(variances)
     )
     assert var.dtype == sc.DType.float64
@@ -384,16 +384,16 @@
     values = np.array([{1, 2}, (3, 4)], dtype=object)
     var = sc.Variable(dims=['x'], values=values)
     check(var)
     var = sc.Variable(dims=['x'], values=values, dtype=sc.DType.PyObject)
     check(var)
 
 
-@pytest.mark.parametrize('dtype', (int, float, bool))
-@pytest.mark.parametrize('values', ([1, 2], [1.2, 3.4], [True, False]))
+@pytest.mark.parametrize('dtype', [int, float, bool])
+@pytest.mark.parametrize('values', [[1, 2], [1.2, 3.4], [True, False]])
 def test_create_1d_override_dtype(dtype, values):
     var = sc.Variable(dims=['x'], values=values, dtype=dtype)
     converted = np.array(values).astype(dtype)
     scipp_dtype = sc.Variable(dims=['x'], values=converted).dtype
     assert var.dtype == scipp_dtype
     np.testing.assert_array_equal(var.values, converted)
 
@@ -406,15 +406,15 @@
     assert var.dims == ('x',)
     assert var.ndim == 1
     assert var.dtype == sc.DType.vector3
     assert var.unit == sc.units.m
 
 
 def test_create_1d_bad_dims():
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='number of dimensions'):
         sc.Variable(dims=['x', 'y'], values=[1, 2])
 
 
 def test_create_2d_inner_size_3():
     var = sc.Variable(
         dims=['x', 'y'], values=np.arange(6.0).reshape(2, 3), unit=sc.units.m
     )
@@ -423,45 +423,45 @@
     np.testing.assert_array_equal(var.values[1], [3, 4, 5])
     assert var.dims == ('x', 'y')
     assert var.ndim == 2
     assert var.dtype == sc.DType.float64
     assert var.unit == sc.units.m
 
 
-@pytest.mark.parametrize('inner_values_type', (tuple, list, np.array))
-@pytest.mark.parametrize('outer_values_type', (tuple, list, np.array))
+@pytest.mark.parametrize('inner_values_type', [tuple, list, np.array])
+@pytest.mark.parametrize('outer_values_type', [tuple, list, np.array])
 def test_create_2d_values_array_like(inner_values_type, outer_values_type):
     values = np.arange(15.0).reshape(3, 5)
     expected = sc.Variable(dims=('x', 'y'), values=values)
 
     var = sc.Variable(
         dims=['x', 'y'],
         values=outer_values_type([inner_values_type(val) for val in values]),
     )
     assert sc.identical(var, expected)
 
 
-@pytest.mark.parametrize('inner_variances_type', (tuple, list, np.array))
-@pytest.mark.parametrize('outer_variances_type', (tuple, list, np.array))
+@pytest.mark.parametrize('inner_variances_type', [tuple, list, np.array])
+@pytest.mark.parametrize('outer_variances_type', [tuple, list, np.array])
 def test_create_2d_variances_array_like(inner_variances_type, outer_variances_type):
     variances = np.arange(15.0).reshape(3, 5)
     var = sc.Variable(
         dims=['x', 'y'],
         variances=outer_variances_type(
             [inner_variances_type(val) for val in variances]
         ),
     )
     np.testing.assert_array_equal(var.values, np.zeros_like(variances))
     np.testing.assert_array_equal(var.variances, variances)
 
 
-@pytest.mark.parametrize('inner_values_type', (tuple, list, np.array))
-@pytest.mark.parametrize('outer_values_type', (tuple, list, np.array))
-@pytest.mark.parametrize('inner_variances_type', (tuple, list, np.array))
-@pytest.mark.parametrize('outer_variances_type', (tuple, list, np.array))
+@pytest.mark.parametrize('inner_values_type', [tuple, list, np.array])
+@pytest.mark.parametrize('outer_values_type', [tuple, list, np.array])
+@pytest.mark.parametrize('inner_variances_type', [tuple, list, np.array])
+@pytest.mark.parametrize('outer_variances_type', [tuple, list, np.array])
 def test_create_2d_values_and_variances_array_like(
     inner_values_type, outer_values_type, inner_variances_type, outer_variances_type
 ):
     values = np.arange(15.0).reshape(3, 5)
     variances = np.arange(15.0).reshape(3, 5) + 15
     expected = sc.Variable(dims=('x', 'y'), values=values, variances=variances)
```

### Comparing `scipp-24.2.0/tests/variable_py_object_test.py` & `scipp-24.5.0/tests/variable_py_object_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/variable_reduction_test.py` & `scipp-24.5.0/tests/variable_reduction_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/variable_scalar_test.py` & `scipp-24.5.0/tests/variable_scalar_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,21 @@
 def test_scalar_Variable_values_property_PyObject():
     var = sc.scalar([1, 2])
     assert var.dtype == sc.DType.PyObject
     assert var.values == [1, 2]
 
 
 @pytest.mark.parametrize(
-    'var', (sc.scalar(3.1), sc.scalar(-2), sc.scalar('abc'), sc.scalar([1, 2]))
+    'var', [sc.scalar(3.1), sc.scalar(-2), sc.scalar('abc'), sc.scalar([1, 2])]
 )
 def test_scalar_Variable_value_is_same_as_values(var):
     assert var.value == var.values
 
 
-@pytest.mark.parametrize('var', (sc.scalar(4), sc.scalar(4.61), sc.scalar('4')))
+@pytest.mark.parametrize('var', [sc.scalar(4), sc.scalar(4.61), sc.scalar('4')])
 def test_scalar_Variable_conversion_to_builtin_int(var):
     assert int(var) == 4
 
 
 def test_scalar_Variable_conversion_to_builtin_int_bad_dtype():
     var = sc.vector(value=[1, 2, 3])
     with pytest.raises(TypeError):
@@ -64,15 +64,15 @@
 
 def test_conversion_to_builtin_int_fails_with_array():
     var = sc.array(dims=['x'], values=[1])
     with pytest.raises(sc.DimensionError):
         int(var)
 
 
-@pytest.mark.parametrize('var', (sc.scalar(-3), sc.scalar(-3.0), sc.scalar('-3.0')))
+@pytest.mark.parametrize('var', [sc.scalar(-3), sc.scalar(-3.0), sc.scalar('-3.0')])
 def test_scalar_Variable_conversion_to_builtin_float(var):
     assert float(var) == -3.0
 
 
 def test_scalar_Variable_conversion_to_builtin_float_bad_dtype():
     var = sc.vector(value=[1.0, 2.0, 3.0])
     with pytest.raises(TypeError):
```

### Comparing `scipp-24.2.0/tests/variable_test.py` & `scipp-24.5.0/tests/variable_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,22 +106,22 @@
     assert var.value == 1.2
     assert var.values.shape == ()
     assert var.values == 1.2
 
 
 @pytest.mark.parametrize(
     'dtypes',
-    (
+    [
         ('int32', np.int32),
         ('int64', np.int64),
         ('float32', np.float32),
         ('float64', np.float64),
         ('datetime64', np.datetime64),
         ('bool', bool),
-    ),
+    ],
 )
 def test_0d_scalar_access_dtype(dtypes):
     dtype, expected = dtypes
     assert isinstance(sc.scalar(7, unit='s', dtype=dtype).value, expected)
 
 
 def test_0D_scalar_string():
@@ -149,15 +149,15 @@
     var = sc.empty(dims=['x'], shape=(2,))
     assert len(var.values) == 2
     assert var.values.shape == (2,)
     var.values[1] = 1.2
     assert var.values[1] == 1.2
 
 
-@pytest.mark.parametrize('dtype', ('int32', 'int64', 'float32', 'float64'))
+@pytest.mark.parametrize('dtype', ['int32', 'int64', 'float32', 'float64'])
 def test_1d_access_dtype(dtype):
     assert sc.array(dims=['xx'], values=[-9], dtype=dtype).values.dtype == dtype
 
 
 def test_1D_set_from_list():
     var = sc.empty(dims=['x'], shape=(2,))
     var.values = [1.0, 2.0]
@@ -337,21 +337,21 @@
 
 
 def test_1d_variance_access():
     v = sc.array(dims=['yy'], values=[0.0, -5.2], variances=[0.1, 2.2])
     np.testing.assert_array_equal(v.variances, [0.1, 2.2])
 
 
-@pytest.mark.parametrize('dtypes', (('float32', np.float32), ('float64', np.float64)))
+@pytest.mark.parametrize('dtypes', [('float32', np.float32), ('float64', np.float64)])
 def test_0d_scalar_variance_access_dtype(dtypes):
     dtype, expected = dtypes
     assert isinstance(sc.scalar(4.1, variance=4.9, dtype=dtype).variance, expected)
 
 
-@pytest.mark.parametrize('dtype', ('float32', 'float64'))
+@pytest.mark.parametrize('dtype', ['float32', 'float64'])
 def test_1d_variance_access_dtype(dtype):
     assert (
         sc.array(
             dims=['xx'], values=[2.13], variances=[0.4], dtype=dtype
         ).variances.dtype
         == dtype
     )
@@ -435,15 +435,17 @@
     assert sc.identical(xy.rename_dims({'y': 'w'}, x='z'), zw)
     assert sc.identical(xy, original)
 
 
 def test_rename_dims_dict_and_kwargs_must_be_distinct():
     values = np.arange(6).reshape(2, 3)
     xy = sc.Variable(dims=['x', 'y'], values=values)
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError, match='The names passed in the dict and as keyword arguments'
+    ):
         xy.rename_dims({'x': 'w'}, x='z')
 
 
 def test_rename():
     values = np.arange(6).reshape(2, 3)
     xy = sc.Variable(dims=['x', 'y'], values=values)
     original = xy.copy()
@@ -462,15 +464,17 @@
     assert sc.identical(xy.rename({'y': 'w'}, x='z'), zw)
     assert sc.identical(xy, original)
 
 
 def test_rename_dict_and_kwargs_must_be_distinct():
     values = np.arange(6).reshape(2, 3)
     xy = sc.Variable(dims=['x', 'y'], values=values)
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError, match='The names passed in the dict and as keyword arguments'
+    ):
         xy.rename({'x': 'w'}, x='z')
 
 
 def test_rename_self_and_dims_dict_are_position_only():
     values = np.arange(6).reshape(2, 3)
     xy = sc.Variable(dims=['x', 'y'], values=values)
     zy = sc.Variable(dims=['z', 'y'], values=values)
@@ -714,15 +718,15 @@
         sc.array(dims=["x"], values=[1000, 2000, 3000], dtype="int64", unit="mm"),
     )
 
 
 def test_to_without_any_arguments():
     data = sc.array(dims=["x"], values=[1, 2, 3], dtype="int64", unit="m")
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Must provide dtype or unit or both'):
         data.to()
 
 
 def test_setting_float_unit_property_to_default_gives_dimensionless():
     var = sc.scalar(1.2, unit='m')
     var.unit = sc.units.default_unit
     assert var.unit == sc.units.one
```

### Comparing `scipp-24.2.0/tests/variable_view_test.py` & `scipp-24.5.0/tests/variable_view_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tests/variance_broadcast_test.py` & `scipp-24.5.0/tests/variance_broadcast_test.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tools/benchmark_build.py` & `scipp-24.5.0/tools/benchmark_build.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,49 +9,48 @@
 import subprocess
 import sys
 from dataclasses import dataclass, field
 from datetime import timedelta
 from itertools import chain, groupby
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import Dict, List
 
 
 @dataclass
 class Case:
     name: str
-    cmake_args: Dict[str, str] = field(default_factory=dict)
-    build_args: List[str] = field(default_factory=list)
+    cmake_args: dict[str, str] = field(default_factory=dict)
+    build_args: list[str] = field(default_factory=list)
 
 
 ##############################
 #      CONFIGURATION         #
 
 # Source directory, defaults to root of scipp repository.
 SRCDIR = None
 
 # Build target for CMake.
 TARGET = "install"
 
 # CMake configuration arguments used for every case.
-COMMON_CMAKE_ARGS = dict(
-    CMAKE_CXX_COMPILER=None,
-    CMAKE_BUILD_TYPE="Debug",
-    CMAKE_INTERPROCEDURAL_OPTIMIZATION="OFF",
-    DYNAMIC_LIB="ON",
-)
+COMMON_CMAKE_ARGS = {
+    "CMAKE_CXX_COMPILER": None,
+    "CMAKE_BUILD_TYPE": "Debug",
+    "CMAKE_INTERPROCEDURAL_OPTIMIZATION": "OFF",
+    "DYNAMIC_LIB": "ON",
+}
 
 # Build arguments used for every case.
 COMMON_BUILD_ARGS = ['-j6']
 
 # Cases to benchmark, each can specify a set of options
 # for configuration and build.
 CASES = [
     Case(name='base'),
-    Case(name='feature', cmake_args=dict(MY_FEATURE='ON')),
+    Case(name='feature', cmake_args={"MY_FEATURE": 'ON'}),
     Case(name='serial', build_args=['-j1']),
 ]
 
 # For every set of files provided here, the build is re-run after touching
 # those files. A clean build is always performed to set the baseline
 # and configure the setup.
 TOUCH = [
@@ -97,15 +96,15 @@
             f'-DPython_EXECUTABLE={sys.executable}',
             str(SRCDIR),
         ]
     )
 
     try:
         subprocess.run(
-            ['cmake', *cmake_args],
+            ['cmake', *cmake_args],  # noqa: S603, S607
             capture_output=True,
             check=True,
             encoding='utf-8',
             cwd=build_dir,
         )
     except subprocess.CalledProcessError as err:
         print(
@@ -118,15 +117,15 @@
 class Times:
     real: timedelta
     user: timedelta
 
     @classmethod
     def parse(cls, msg):
         time_pattern = re.compile(r'(real|user|sys)\s+(\d+)m(\d+)[,.]?(\d*)s')
-        times_dict = dict()
+        times_dict = {}
         for line in msg.rsplit('\n', 10)[
             1:
         ]:  # do not look at all of the output, it can get very long
             match = time_pattern.match(line)
             if match:
                 # Truncate sub second results, those will not be reliable.
                 times_dict[match[1]] = timedelta(
@@ -148,15 +147,15 @@
     try:
         res = subprocess.run(
             ' '.join(['time', 'cmake', *build_args]),
             capture_output=True,
             check=True,
             encoding='utf-8',
             cwd=build_dir,
-            shell=True,
+            shell=True,  # noqa: S602
         )
     except subprocess.CalledProcessError as err:
         print(f"Build '{case.name}' failed:\n{err.stdout}\n{err.stderr}")
         sys.exit(1)
 
     return Times.parse(res.stderr)
 
@@ -165,15 +164,15 @@
     print('Result:\n')
     results = sorted(
         sorted(results, key=lambda t: t[0]),
         key=lambda t: ' '.join('' if t[1] == 'clean' else str(t[1])),
     )
     printed_names = False
     for touch, group in groupby(results, key=lambda t: t[1]):
-        names, _, times = zip(*group)
+        names, _, times = zip(*group, strict=True)
         if not printed_names:
             print(
                 '                      '
                 + '  '.join(f'{name:20s}' for name in names)
                 + '\n'
             )
             printed_names = True
@@ -192,15 +191,15 @@
             + '\n'
         )
 
 
 def main():
     results = []
     with TemporaryDirectory(dir='./') as working_dir:
-        for case, dirs in zip(CASES, make_dirs(working_dir)):
+        for case, dirs in zip(CASES, make_dirs(working_dir), strict=True):
             print(f"Running '{case.name}'")
             print('    Clean build')
             configure(case, *dirs)
             times = build(case, dirs[0])
             results.append((case.name, ['clean'], times))
 
             for touch in TOUCH:
```

### Comparing `scipp-24.2.0/tools/debug/debug_multi_index_fragment.h` & `scipp-24.5.0/tools/debug/debug_multi_index_fragment.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tools/debug/debugout.h` & `scipp-24.5.0/tools/debug/debugout.h`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tools/metatoenv.py` & `scipp-24.5.0/tools/metatoenv.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             if key.count('[') > 0:
                 left = key.find('[')
                 right = key.find(']')
                 if key.count(']') != key.count('[') or right < left:
                     raise RuntimeError(
                         "Bad preprocessing selector: "
                         "unmatched square brackets or closing bracket "
-                        "found before opening bracket: {}".format(key)
+                        f"found before opening bracket: {key}"
                     )
                 selector = key[left : right + 1]
                 if selector.startswith('[not'):
                     if (platform in selector) or (
                         selector.replace('[not', '')[:-1].strip() in platform
                     ):
                         ok = False
@@ -169,52 +169,52 @@
     From: https://stackoverflow.com/a/7205107/13086629
     """
     if path is None:
         path = []
     for key in b:
         if key in a:
             if isinstance(a[key], dict) and isinstance(b[key], dict):
-                _merge_dicts(a[key], b[key], path + [str(key)])
+                _merge_dicts(a[key], b[key], [*path, str(key)])
             elif a[key] == b[key]:
                 pass  # same leaf value
             else:
-                raise Exception('Conflict at %s' % '.'.join(path + [str(key)]))
+                raise Exception('Conflict at {}'.format('.'.join((*path, str(key)))))
         else:
             a[key] = b[key]
     return a
 
 
 def _write_dict(d, file_handle, indent):
     for key, value in d.items():
-        file_handle.write((" " * indent) + "- {}\n".format(key))
+        file_handle.write((" " * indent) + f"- {key}\n")
         if isinstance(value, dict):
             _write_dict(value, file_handle=file_handle, indent=indent + 2)
 
 
 def main(metafile, envfile, envname, channels, platform, extra, mergewith):
     # Find current platform
     if platform is None:
         platform_mapping = {"Linux": "linux", "Darwin": "osx", "Windows": "win"}
         platform = platform_mapping[_platform.system()]
 
     # Read and parse metafile
-    with open(metafile, "r") as f:
+    with open(metafile) as f:
         metacontent = f.readlines()
     meta = _parse_yaml(metacontent)
 
     # Merge three dicts into one
     meta_dependencies = meta["requirements:"]["build:"].copy()
     reduce(
         _merge_dicts,
         [meta_dependencies, meta["requirements:"]["run:"], meta["test:"]["requires:"]],
     )
 
     # Read file with additional dependencies
     if len(mergewith) > 0:
-        with open(mergewith, "r") as f:
+        with open(mergewith) as f:
             mergecontent = f.readlines()
         additional = _parse_yaml(mergecontent)
         additional_dependencies = additional["dependencies:"]
         _merge_dicts(meta_dependencies, additional_dependencies)
         channels = set(channels + list(additional["channels:"].keys()))
 
     # Add dependencies added via the command line
@@ -233,18 +233,18 @@
     with open(envfile, "w") as out:
         out.write("##############################################################\n")
         out.write("# WARNING! This environment file was generated from the\n")
         out.write("# conda/meta.yaml file using the metatoenv.py tool.\n")
         out.write("# Do not update this file in-place.\n")
         out.write("# Use metatoenv.py to create a new file.\n")
         out.write("##############################################################\n\n")
-        out.write("name: {}\n".format(envname))
+        out.write(f"name: {envname}\n")
         out.write("channels:\n")
         for channel in channels:
-            out.write("  - {}\n".format(channel))
+            out.write(f"  - {channel}\n")
         out.write("dependencies:\n")
         _write_dict(meta_dependencies, file_handle=out, indent=2)
 
 
 if __name__ == '__main__':
     args = parser.parse_args()
```

### Comparing `scipp-24.2.0/tools/migration/scipp-0.11-hdf5-files.py` & `scipp-24.5.0/tools/migration/scipp-0.11-hdf5-files.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Convert pre-0.11 HDF5 files to 0.11-compatible files.
 
 Changes are:
 
 * Rename dtype vector_3_float64 to vector3
 * Rename dtype matrix_3_float64 to linear_transform3
 """
+
 import sys
 from shutil import copyfile
 
 import h5py
 
 
 def migrate_object(name, obj):
```

### Comparing `scipp-24.2.0/tools/migration/scipp-0.12-hdf5-files.py` & `scipp-24.5.0/tools/migration/scipp-0.12-hdf5-files.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 Convert pre-0.12 HDF5 files to 0.12-compatible files.
 
 Changes are:
 
 * Unit of values of `begin` and `end` indices for binned data removed
 """
+
 import sys
 from shutil import copyfile
 
 import h5py
 
 
 def migrate_object(name, obj):
```

### Comparing `scipp-24.2.0/tools/migration/scipp-0.13-hdf5-files.py` & `scipp-24.5.0/tools/migration/scipp-0.13-hdf5-files.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 Convert pre-0.13 HDF5 files to 0.13-compatible files.
 
 Changes are:
 
 * Names of coords, attrs, masks, and dataset items are encoded via attributes.
 """
+
 import sys
 from shutil import copyfile
 
 import h5py
 
 
 # NOTE copied from scipp.io.hdf5 at Git ref a74103329
```

### Comparing `scipp-24.2.0/tools/plot_benchmarks.py` & `scipp-24.5.0/tools/plot_benchmarks.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,24 +108,26 @@
         else 'meta'
         for c in data.columns
     ]
 
 
 def group_plots(data, designations):
     """Return the number of distinct plot groups and the groups themselves."""
-    meta_columns = [c for c, d in zip(data.columns, designations) if d == 'meta']
+    meta_columns = [
+        c for c, d in zip(data.columns, designations, strict=True) if d == 'meta'
+    ]
     groups = data.groupby(meta_columns)
     return len(groups), [group for _, group in groups]
 
 
 def plot_title(data, designations):
     """Format a title for a plot of ``data``."""
     return ', '.join(
         f'{c}={data[c].unique()[0]}'
-        for c, d in zip(data.columns, designations)
+        for c, d in zip(data.columns, designations, strict=True)
         if d == 'meta'
     )
 
 
 def get_unit(data, name):
     """Return the unit for an axis label for column ``name``."""
     if name in ('real_time', 'cpu_time'):
```

### Comparing `scipp-24.2.0/tools/run_sanitizer.sh` & `scipp-24.5.0/tools/run_sanitizer.sh`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tools/stubgen/README.md` & `scipp-24.5.0/tools/stubgen/README.md`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tools/stubgen/__init__.py` & `scipp-24.5.0/tools/stubgen/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ast
 import enum
 import inspect
+from collections.abc import Iterable
 from string import Template
-from typing import Iterable, List, Optional, Type
 
 from .config import (
     DISABLE_TYPE_CHECK_OVERRIDE,
     HEADER,
     INCLUDE_DOCS,
     TEMPLATE_FILE,
     class_is_excluded,
@@ -21,33 +21,33 @@
     )
 
 
 def _add_suppression_comments(code: str) -> str:
     def _add_override(s: str) -> str:
         for name in DISABLE_TYPE_CHECK_OVERRIDE:
             if name in s:
-                return s + '  # type: ignore[override]'
+                return s + '  # type: ignore[override, unused-ignore]'
         return s
 
     return '\n'.join(_add_override(line) for line in code.splitlines())
 
 
-def _build_method(cls: Type[type], method_name: str) -> [ast.FunctionDef]:
+def _build_method(cls: type[type], method_name: str) -> [ast.FunctionDef]:
     meth = inspect.getattr_static(cls, method_name)
     return [
         fix_method(m, cls_name=cls.__name__) for m in parse_method(meth, method_name)
     ]
 
 
-def _build_property(cls: Type[type], property_name: str) -> [ast.FunctionDef]:
+def _build_property(cls: type[type], property_name: str) -> [ast.FunctionDef]:
     prop = inspect.getattr_static(cls, property_name)
     return [fix_property(p) for p in parse_property(prop, property_name)]
 
 
-def _build_attr(cls: Type[type], attr_name: str) -> [ast.Expr]:
+def _build_attr(cls: type[type], attr_name: str) -> [ast.Expr]:
     typ: str = ast.parse(type(getattr(cls, attr_name)).__name__).body[0].value.id
     return [
         ast.AnnAssign(
             target=ast.Name(id=attr_name, ctx=ast.Store()),
             annotation=ast.Name(id=typ, ctx=ast.Load()),
             value=ast.Constant(value=Ellipsis),
             simple=1,
@@ -59,34 +59,43 @@
     function = enum.auto()
     instancemethod = enum.auto()
     prop = enum.auto()
     attr = enum.auto()
     skip = enum.auto()
 
 
-def _classify(obj: object, member_name: str, cls: Type[type]) -> _Member:
+def _classify(obj: object, member_name: str, cls: type[type]) -> _Member:
     if 'pybind11_static_property' in repr(inspect.getattr_static(cls, member_name)):
         return _Member.attr
     if inspect.isbuiltin(obj):
         return _Member.skip
     if inspect.isdatadescriptor(obj):
         return _Member.prop
     if inspect.isfunction(obj):
         return _Member.function
     if inspect.isroutine(obj) and 'instancemethod' in repr(obj):
         return _Member.instancemethod
     return _Member.skip
 
 
-def _get_bases(cls: Type[type]) -> List[ast.Name]:
-    base_classes = [base for base in cls.__bases__ if 'pybind11' not in repr(base)]
-    return [ast.Name(id=cls.__name__) for cls in base_classes]
+def _get_bases(cls: type[type]) -> list[ast.Name]:
+    bases = [
+        ast.Name(id=base.__name__)
+        for base in cls.__bases__
+        if 'pybind11' not in repr(base)
+    ]
+    # Bindings do not set base classes for mappings, so inject them manually.
+    if cls.__name__ in ('Coords', 'Masks'):
+        bases.append(ast.Name(id='Mapping[str, Variable]'))
+    if cls.__name__ == 'Dataset':
+        bases.append(ast.Name(id='Mapping[str, DataArray]'))
+    return bases
 
 
-def _build_class(cls: Type[type]) -> Optional[ast.ClassDef]:
+def _build_class(cls: type[type]) -> ast.ClassDef | None:
     print(f'Generating class {cls.__name__}')
     body = []
     if cls.__doc__ and INCLUDE_DOCS:
         body.append(ast.Expr(value=ast.Constant(value=cls.__doc__)))
 
     for member_name, member in inspect.getmembers(cls):
         member_class = _classify(member, member_name, cls)
@@ -113,15 +122,15 @@
 
     if not INCLUDE_DOCS:
         cls = ast.fix_missing_locations(RemoveDocstring().visit(cls))
 
     return ast.fix_missing_locations(cls)
 
 
-def _cpp_classes() -> Iterable[Type[type]]:
+def _cpp_classes() -> Iterable[type[type]]:
     from scipp._scipp import core
 
     for name, cls in inspect.getmembers(core, inspect.isclass):
         if not class_is_excluded(name):
             yield cls
```

### Comparing `scipp-24.2.0/tools/stubgen/__main__.py` & `scipp-24.5.0/tools/stubgen/__main__.py`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/tools/stubgen/config.py` & `scipp-24.5.0/tools/stubgen/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import ast
 from pathlib import Path
-from typing import List
 
 # The name of the C++ module that contains the classes we generate stubs for.
 CPP_CORE_MODULE_NAME = 'scipp._scipp.core'
 
 # Template for the generated stub.
 TEMPLATE_FILE = Path(__file__).resolve().parent / 'stub_template.py.template'
 
@@ -33,16 +32,16 @@
 
 def class_is_excluded(name: str) -> bool:
     """Return True if a class stub should be omitted."""
     return name.startswith('ElementArrayView') or name.startswith('_')
 
 
 def _squash_binary_more_narrow_type(
-    overloads: List[ast.FunctionDef],
-) -> List[ast.FunctionDef]:
+    overloads: list[ast.FunctionDef],
+) -> list[ast.FunctionDef]:
     # A lot of binary functions have overloads for int and float.
     # But the former is superseded by the latter because int is more narrow than float.
     # Drop all int overloads in this case.
     rhs_types = []
     for overload in overloads:
         ann = overload.args.args[1].annotation
         if isinstance(ann, ast.Name):
@@ -53,14 +52,14 @@
     if 'int' in rhs_types and 'float' in rhs_types:
         squashed = list(overloads)
         del squashed[rhs_types.index('int')]
         return squashed
     return overloads
 
 
-def squash_overloads(overloads: List[ast.FunctionDef]) -> List[ast.FunctionDef]:
+def squash_overloads(overloads: list[ast.FunctionDef]) -> list[ast.FunctionDef]:
     """Combine overloads if a stub for only one is required."""
     if overloads[0].name in ('__eq__', '__ne__'):
         return overloads[:1]
     if len(overloads[0].args.args) == 2:
         return _squash_binary_more_narrow_type(overloads)
     return overloads
```

### Comparing `scipp-24.2.0/tools/stubgen/parse.py` & `scipp-24.5.0/tools/stubgen/parse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Parser for function docstrings."""
+
 import ast
 import inspect
 import re
-from typing import Any, List, Optional, Tuple
+from typing import Any
 
 from .config import CPP_CORE_MODULE_NAME, squash_overloads
 from .transformer import (
     AddOverloadedDecorator,
     DropFunctionBody,
+    OverwriteSignature,
     RemoveDecorators,
     SetFunctionName,
     add_decorator,
 )
 
 
 def _is_overloaded(docstring: str) -> bool:
@@ -89,64 +91,66 @@
     docstring = _fix_cpp_namespace_access(docstring)
     docstring = _fix_default_arg_repr(docstring)
     if _is_overloaded(docstring):
         return _make_code_for_parse_overloaded(docstring, name)
     return _make_code_for_parse_single(docstring, name)
 
 
-def _parse_instancemethod(func: object, name: Optional[str]) -> List[ast.FunctionDef]:
+def _parse_instancemethod(func: object, name: str | None) -> list[ast.FunctionDef]:
     """Parse docstring of a method generated by Pybind11."""
     node = ast.parse(
         _make_instancemethod_code_for_parse(inspect.getdoc(func), name or func.__name__)
     )
     body = node.body
-    body = squash_overloads(body)  # type: ignore
+    body = squash_overloads(body)
     if len(body) > 1:
         transformer = AddOverloadedDecorator()
         return [transformer.visit(meth) for meth in body]
-    return body  # type: ignore
+    return body
 
 
 def _make_regular_method_code_for_parse(
     signature: inspect.Signature, name: str, docstring: str
 ) -> str:
     sig = f'def {name}{signature}:'
     if not docstring:
         return sig + ' ...'
     return f'{sig}\n{_make_docstring(docstring)}'
 
 
-def _unwrap(func: Any) -> Tuple[Any, int]:
+def _unwrap(func: Any) -> tuple[Any, int]:
     i = 0
     while hasattr(func, '__wrapped__'):
         i += 1
         func = func.__wrapped__
     return func, i
 
 
-def _parse_regular_method(func: Any, name: Optional[str]) -> List[ast.FunctionDef]:
+def _parse_regular_method(func: Any, name: str | None) -> list[ast.FunctionDef]:
     """Parse a function defined in Python."""
     func, n_decorators = _unwrap(func)
     node = ast.parse(inspect.getsource(func))
     node = DropFunctionBody().visit(node)
     node = RemoveDecorators(n_decorators).visit(node)
     if name is not None:
         node = SetFunctionName(name).visit(node)
+    if (sig := getattr(func, '__signature__', None)) is not None:
+        node = OverwriteSignature(sig).visit(node)
     node = ast.fix_missing_locations(node)
-    return node.body  # type: ignore
+    return node.body
 
 
-def parse_method(func: Any, name: Optional[str] = None) -> List[ast.FunctionDef]:
+def parse_method(func: Any, name: str | None = None) -> list[ast.FunctionDef]:
     if inspect.isfunction(func):
         x = _parse_regular_method(func, name)
         return x
     return _parse_instancemethod(func, name)
 
 
-def _make_property(prop: property, name: str, part: str) -> Optional[ast.FunctionDef]:
+def _make_property(prop: property, name: str, part: str) -> ast.FunctionDef | None:
     func = getattr(
         prop, {'getter': 'fget', 'setter': 'fset', 'deleter': 'fdel'}[part], None
     )
     if func is None:
         return None
 
     if part == 'getter':
@@ -156,15 +160,15 @@
             value=ast.Name(id=name, ctx=ast.Load()), attr=part, ctx=ast.Load()
         )
 
     (meth,) = parse_method(func, name)
     return add_decorator(meth, deco)
 
 
-def parse_property(prop: property, name: str) -> List[ast.FunctionDef]:
+def parse_property(prop: property, name: str) -> list[ast.FunctionDef]:
     return list(
         filter(
             lambda p: p is not None,
             (
                 _make_property(prop, name=name, part=part)
                 for part in ('getter', 'setter', 'deleter')
             ),
```

### Comparing `scipp-24.2.0/tools/stubgen/transformer.py` & `scipp-24.5.0/tools/stubgen/transformer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Transform an AST to fix type annotations."""
 
 import ast
-from typing import Optional, Union
+import inspect
 
 from .config import CPP_CORE_MODULE_NAME
 
 
-def unqualified_cpp_class(node: Union[ast.Attribute, ast.Name]) -> Optional[str]:
+def unqualified_cpp_class(node: ast.Attribute | ast.Name) -> str | None:
     """Return the unqualified name of a C++ class in _scipp.core.
     Returns None if the class is not in _scipp.core.
     ``node`` should be a type annotation.
     """
     pieces = []
     while isinstance(node, ast.Attribute):
         pieces.append(node.attr)
@@ -18,31 +18,37 @@
     pieces.append(node.id)
     if pieces[1:] != CPP_CORE_MODULE_NAME.split('.')[::-1]:
         return None
     return pieces[0]
 
 
 def replace_function(base: ast.FunctionDef, **kwargs) -> ast.FunctionDef:
-    args = dict(
-        name=base.name,
-        args=base.args,
-        body=base.body,
-        decorator_list=base.decorator_list,
-        returns=base.returns,
-        type_comment=base.type_comment,
-    )
+    args = {
+        'name': base.name,
+        'args': base.args,
+        'body': base.body,
+        'decorator_list': base.decorator_list,
+        'returns': base.returns,
+        'type_comment': base.type_comment,
+    }
     return ast.FunctionDef(**{**args, **kwargs})
 
 
 def add_decorator(
-    base: ast.FunctionDef, decorator: Union[ast.Name, ast.Attribute]
+    base: ast.FunctionDef, decorator: ast.Name | ast.Attribute
 ) -> ast.FunctionDef:
     return replace_function(base, decorator_list=[decorator, *base.decorator_list])
 
 
+def get_first_argument(node: ast.arguments) -> ast.arg:
+    if node.posonlyargs:
+        return node.posonlyargs[0]
+    return node.args[0]
+
+
 class AddOverloadedDecorator(ast.NodeTransformer):
     def visit_FunctionDef(self, node: ast.FunctionDef) -> ast.FunctionDef:
         self.generic_visit(node)
         return add_decorator(node, decorator=ast.Name(id='overload', ctx=ast.Load()))
 
 
 class RemoveDecorators(ast.NodeTransformer):
@@ -60,21 +66,21 @@
 
 
 class FixSelfArgName(ast.NodeTransformer):
     """Ensure that the first argument is called self."""
 
     def visit_arguments(self, node: ast.arguments) -> ast.arguments:
         self.generic_visit(node)
-        keep = dict(
-            kwonlyargs=node.kwonlyargs,
-            vararg=node.vararg,
-            kwarg=node.kwarg,
-            kw_defaults=node.kw_defaults,
-            defaults=node.defaults,
-        )
+        keep = {
+            'kwonlyargs': node.kwonlyargs,
+            'vararg': node.vararg,
+            'kwarg': node.kwarg,
+            'kw_defaults': node.kw_defaults,
+            'defaults': node.defaults,
+        }
         if node.posonlyargs and node.posonlyargs[0].arg != 'self':
             return ast.arguments(
                 posonlyargs=[
                     ast.arg('self', annotation=None, type_comment=None),
                     *node.posonlyargs[1:],
                 ],
                 args=node.args,
@@ -98,28 +104,63 @@
     def visit_arg(self, node: ast.arg) -> ast.arg:
         if node.arg != 'self':
             self.generic_visit(node)
             return node
         return ast.arg(node.arg, None, None)
 
 
+class ReplaceTypeVarInReturn(ast.NodeTransformer):
+    """Replace TypeVars in return annotations with concrete types.
+
+    Some functions are defined as generic functions in Python, e.g.,
+
+    .. code-block:: python
+
+        def sum(x: VariableLikeType, dim: Dims = None) -> VariableLikeType:
+
+    When those functions are bound as methods, the return type is constrained by
+    the class that the method is bound to.
+    So this transformer replaces the annotation by the class name.
+    """
+
+    TYPE_VARS = ('VariableLikeType', '_VarDaDg')
+
+    def __init__(self, cls_name: str) -> None:
+        self.cls_name = cls_name
+
+    def visit_FunctionDef(self, node: ast.FunctionDef) -> ast.FunctionDef:
+        self.generic_visit(node)
+        for type_var in self.TYPE_VARS:
+            if isinstance(node.returns, ast.Name) and node.returns.id == type_var:
+                first_arg = get_first_argument(node.args)
+                try:
+                    self_annotation = first_arg.annotation.id
+                except AttributeError:
+                    continue
+                if self_annotation == type_var:
+                    return replace_function(
+                        node, returns=ast.Name(id=self.cls_name, ctx=ast.Load())
+                    )
+        return node
+
+
 class ShortenCppClassAnnotation(ast.NodeTransformer):
     """Remove module qualification from scipp classes."""
 
-    def visit_Attribute(self, node: ast.Attribute) -> Union[ast.Attribute, ast.Name]:
+    def visit_Attribute(self, node: ast.Attribute) -> ast.Attribute | ast.Name:
         self.generic_visit(node)
         if (cls := unqualified_cpp_class(node)) is not None:
             return ast.Name(cls)
         if isinstance(node.value, ast.Name) and node.value.id == '_cpp':
             return ast.Name(id=node.attr, ctx=ast.Load())
         return node
 
 
 class DropTypingModule(ast.NodeTransformer):
-    def visit_Attribute(self, node: ast.Attribute) -> Union[ast.Attribute, ast.Name]:
+    def visit_Attribute(self, node: ast.Attribute) -> ast.Attribute | ast.Name:
         self.generic_visit(node)
         if isinstance(node.value, ast.Name) and node.value.id == 'typing':
             return ast.Name(id=node.attr, ctx=ast.Load())
         return node
 
 
 class DropFunctionBody(ast.NodeTransformer):
@@ -141,14 +182,35 @@
         self.target_name = name
 
     def visit_FunctionDef(self, node: ast.FunctionDef) -> ast.FunctionDef:
         self.generic_visit(node)
         return replace_function(node, name=self.target_name)
 
 
+class OverwriteSignature(ast.NodeTransformer):
+    """Replaces a function signature by the given signature."""
+
+    def __init__(self, sig: inspect.Signature) -> None:
+        self.sig = sig
+
+    def visit_FunctionDef(self, node: ast.FunctionDef) -> ast.FunctionDef:
+        self.generic_visit(node)
+        code = f'def f{self.sig}: ...'
+        # A hack to work around _NoDefault.__repr__
+        # I can't think of a better way to do this :(
+        code = code.replace('NotSpecified', '_NoDefault')
+        target = ast.parse(code).body[0]
+        r = replace_function(
+            node,
+            args=target.args,
+            returns=target.returns,
+        )
+        return r
+
+
 class FixArgumentFromSupertypes(ast.NodeTransformer):
     def __init__(self) -> None:
         self._do_replacement = False
 
     def visit_FunctionDef(self, node: ast.FunctionDef) -> ast.FunctionDef:
         if node.name in ('__eq__', '__ne__'):
             self._do_replacement = True
@@ -177,15 +239,15 @@
         '__ior__',
         '__ipow__',
         '__irshift__' '__isub__',
         '__itruediv__',
         '__ixor__',
     )
 
-    def __init__(self, cls: Optional[str]) -> None:
+    def __init__(self, cls: str | None) -> None:
         self.cls = cls
 
     def visit_FunctionDef(self, node: ast.FunctionDef) -> ast.FunctionDef:
         self.generic_visit(node)
         if (
             node.name in self.METHODS
             and isinstance(node.returns, ast.Name)
@@ -224,14 +286,15 @@
     node = ObjectToAny().visit(node)
     node = ReplaceNoneType().visit(node)
     node = DropTypingModule().visit(node)
     return node
 
 
 def fix_method(node: ast.AST, cls_name: str) -> ast.AST:
+    node = ReplaceTypeVarInReturn(cls_name).visit(node)  # Must be before FixSelfArgName
     node = _fix_common(node)
     node = FixObjectReturnType(cls_name).visit(node)
     node = FixArgumentFromSupertypes().visit(node)
     node = ast.fix_missing_locations(node)
     return node
```

### Comparing `scipp-24.2.0/tox.ini` & `scipp-24.5.0/tox.ini`

 * *Files identical despite different names*

### Comparing `scipp-24.2.0/PKG-INFO` & `scipp-24.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipp
-Version: 24.2.0
+Version: 24.5.0
 Summary: Multi-dimensional data arrays with labeled dimensions
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scipp contributors (https://github.com/scipp)
         All rights reserved.
         
@@ -33,52 +33,50 @@
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Project-URL: Documentation, https://scipp.github.io/
 Project-URL: Source, https://github.com/scipp/scipp
 Project-URL: Bug tracker, https://github.com/scipp/scipp/issues
 Project-URL: Changelog, https://scipp.github.io/about/release-notes.html
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Requires-Dist: numpy>=1.20
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: matplotlib; extra == "test"
 Requires-Dist: bs4; extra == "test"
 Requires-Dist: ipython; extra == "test"
-Requires-Dist: h5py; extra == "all"
-Requires-Dist: scipy>=1.7.0; extra == "all"
-Requires-Dist: graphviz; extra == "all"
-Requires-Dist: pooch; extra == "all"
-Requires-Dist: plopp; extra == "all"
-Requires-Dist: matplotlib; extra == "all"
-Requires-Dist: ipympl; extra == "interactive"
-Requires-Dist: ipython; extra == "interactive"
-Requires-Dist: ipywidgets; extra == "interactive"
-Requires-Dist: matplotlib; extra == "interactive"
-Requires-Dist: jupyterlab; extra == "interactive"
-Requires-Dist: jupyterlab-widgets; extra == "interactive"
-Requires-Dist: jupyter_nbextensions_configurator; extra == "interactive"
-Requires-Dist: nodejs; extra == "interactive"
-Requires-Dist: plopp; extra == "interactive"
-Requires-Dist: pythreejs; extra == "interactive"
+Requires-Dist: h5py; extra == "extra"
+Requires-Dist: scipy>=1.7.0; extra == "extra"
+Requires-Dist: graphviz; extra == "extra"
+Requires-Dist: pooch; extra == "extra"
+Requires-Dist: plopp; extra == "extra"
+Requires-Dist: matplotlib; extra == "extra"
+Requires-Dist: scipp[extra]; extra == "all"
+Requires-Dist: ipympl; extra == "all"
+Requires-Dist: ipython; extra == "all"
+Requires-Dist: ipywidgets; extra == "all"
+Requires-Dist: jupyterlab; extra == "all"
+Requires-Dist: jupyterlab-widgets; extra == "all"
+Requires-Dist: jupyter_nbextensions_configurator; extra == "all"
+Requires-Dist: nodejs; extra == "all"
+Requires-Dist: pythreejs; extra == "all"
 Provides-Extra: test
+Provides-Extra: extra
 Provides-Extra: all
-Provides-Extra: interactive
 Description-Content-Type: text/markdown
 
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
 [![PyPI badge](http://img.shields.io/pypi/v/scipp.svg)](https://pypi.python.org/pypi/scipp)
 [![Anaconda-Server Badge](https://anaconda.org/scipp/scipp/badges/version.svg)](https://anaconda.org/scipp/scipp)
 [![License: BSD 3-Clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](LICENSE)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4019/badge)](https://bestpractices.coreinfrastructure.org/projects/4019)
```

