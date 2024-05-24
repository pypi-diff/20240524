# Comparing `tmp/plopp-24.4.0.tar.gz` & `tmp/plopp-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plopp-24.4.0.tar", last modified: Tue Apr 16 14:08:48 2024, max compression
+gzip compressed data, was "plopp-24.5.0.tar", last modified: Fri May 24 12:02:57 2024, max compression
```

## Comparing `plopp-24.4.0.tar` & `plopp-24.5.0.tar`

### file list

```diff
@@ -1,277 +1,274 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.881412 plopp-24.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-16 14:08:37.000000 plopp-24.4.0/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.837412 plopp-24.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.841412 plopp-24.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/copier.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/nightly_at_main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/nightly_at_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/python-version-ci
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/unpinned.yml
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-16 14:08:37.000000 plopp-24.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-16 14:08:37.000000 plopp-24.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-16 14:08:37.000000 plopp-24.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-16 14:08:37.000000 plopp-24.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-16 14:08:37.000000 plopp-24.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 14:08:37.000000 plopp-24.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-16 14:08:48.881412 plopp-24.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-16 14:08:37.000000 plopp-24.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.841412 plopp-24.4.0/conda/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-16 14:08:37.000000 plopp-24.4.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.841412 plopp-24.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.841412 plopp-24.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/anaconda-icon.js
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/circle-exclamation.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.841412 plopp-24.4.0/docs/_static/customization/
--rw-r--r--   0 runner    (1001) docker     (127)   114427 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/customization/custom-interfaces.png
--rw-r--r--   0 runner    (1001) docker     (127)    44133 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/customization/graph-node-tips.png
--rw-r--r--   0 runner    (1001) docker     (127)    54880 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/customization/subplots.png
--rw-r--r--   0 runner    (1001) docker     (127)    19228 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/customization/tweaking-figures.png
--rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.845412 plopp-24.4.0/docs/_static/gallery/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/gallery/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   211913 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/gallery/peeling-layers-thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (127)    18766 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/gallery/scatter3d-with-slider-thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (127)    66718 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (127)    76311 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    76253 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.845412 plopp-24.4.0/docs/_static/plot-types/
--rw-r--r--   0 runner    (1001) docker     (127)    37065 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/plot-types/image-plot.png
--rw-r--r--   0 runner    (1001) docker     (127)    47635 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/plot-types/inspector-plot.png
--rw-r--r--   0 runner    (1001) docker     (127)    15510 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/plot-types/line-plot.png
--rw-r--r--   0 runner    (1001) docker     (127)    72368 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/plot-types/scatter-plot.png
--rw-r--r--   0 runner    (1001) docker     (127)   186659 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/plot-types/scatter3d-plot.png
--rw-r--r--   0 runner    (1001) docker     (127)    55181 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/plot-types/slicer-plot.png
--rw-r--r--   0 runner    (1001) docker     (127)    50020 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/plot-types/super-plot.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.845412 plopp-24.4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_templates/class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_templates/doc_version.html
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_templates/module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_templates/scipp-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_templates/scipp-module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.845412 plopp-24.4.0/docs/about/
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/about/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.849412 plopp-24.4.0/docs/api-reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/api-reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/api-reference/matplotlib.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/api-reference/plotly.md
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/api-reference/pythreejs.md
--rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.849412 plopp-24.4.0/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/developer/coding-conventions.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/developer/dependency-management.md
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/developer/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/developer/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.849412 plopp-24.4.0/docs/gallery/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/interactive-masking.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/masking-a-range.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/nyc-taxi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/peeling-layers.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/polar-plots.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/rectangle-selection.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/scatter3d-with-slider.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/scatter3d-with-threshold.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/tiled-random-samples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/updating-scatter.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.849412 plopp-24.4.0/docs/user-guide/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.849412 plopp-24.4.0/docs/user-guide/customization/
--rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/customization/custom-interfaces.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/customization/graph-node-tips.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/customization/subplots.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/customization/tweaking-figures.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.853412 plopp-24.4.0/docs/user-guide/getting-started/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/getting-started/numpy-pandas-xarray.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/getting-started/overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/getting-started/saving-figures.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.853412 plopp-24.4.0/docs/user-guide/plot-types/
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/plot-types/image-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/plot-types/inspector-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/plot-types/line-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/plot-types/scatter-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/plot-types/scatter3d-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/plot-types/slicer-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/plot-types/super-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-16 14:08:37.000000 plopp-24.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.857412 plopp-24.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/basetest.in
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/basetest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/constraints.in
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/make_base.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/mini.in
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/mini.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/mypy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/nightly.in
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/nightly.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/noplotly.in
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/noplotly.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/optional.in
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.857412 plopp-24.4.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    53363 2024-04-16 14:08:37.000000 plopp-24.4.0/resources/logo-plopp-2022.svg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-16 14:08:48.881412 plopp-24.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.833412 plopp-24.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.857412 plopp-24.4.0/src/plopp/
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.861412 plopp-24.4.0/src/plopp/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.861412 plopp-24.4.0/src/plopp/backends/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17975 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/static.py
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/tiled.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.861412 plopp-24.4.0/src/plopp/backends/plotly/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/plotly/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/plotly/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/plotly/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.865412 plopp-24.4.0/src/plopp/backends/pythreejs/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/pythreejs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/pythreejs/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/pythreejs/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/pythreejs/outline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/pythreejs/point_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.865412 plopp-24.4.0/src/plopp/core/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/core/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/core/limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/core/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/core/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/core/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.865412 plopp-24.4.0/src/plopp/data/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/data/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/data/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/data/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.869412 plopp-24.4.0/src/plopp/graphics/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/basefig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/colormapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/graphicalview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/lineview.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/scatter3dview.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/scatterview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/tiled.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.869412 plopp-24.4.0/src/plopp/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/scatter3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/superplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/xyplot.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.873412 plopp-24.4.0/src/plopp/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/checkboxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    13963 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/clip3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    10244 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/cut3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/debounce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/drawing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/linesave.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/slice.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.881412 plopp-24.4.0/src/plopp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-16 14:08:48.000000 plopp-24.4.0/src/plopp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-16 14:08:48.000000 plopp-24.4.0/src/plopp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:08:48.000000 plopp-24.4.0/src/plopp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-16 14:08:48.000000 plopp-24.4.0/src/plopp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 14:08:48.000000 plopp-24.4.0/src/plopp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.873412 plopp-24.4.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.837412 plopp-24.4.0/tests/backends/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.873412 plopp-24.4.0/tests/backends/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_canvas_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_figure_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_imageview_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_interactive_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_line_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_lineview_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_scatter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_tiled_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.873412 plopp-24.4.0/tests/backends/plotly/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/plotly/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/plotly/plotly_canvas_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/plotly/plotly_figure_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/plotly/plotly_line_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.877412 plopp-24.4.0/tests/backends/pythreejs/
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/pythreejs/pythreejs_canvas_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/pythreejs/pythreejs_figure_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.877412 plopp-24.4.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/core/graph_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/core/limits_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/core/node_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/core/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.877412 plopp-24.4.0/tests/graphics/
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/graphics/colormapper_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/graphics/imageview_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/graphics/lineview_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/graphics/scatter3dview_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/graphics/scatterview_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/high_level_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/minimal_plot_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/package_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.877412 plopp-24.4.0/tests/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/common_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/inspector_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/plot_1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/plot_2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/scatter3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/scatter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/slicer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/superplot_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/xyplot_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.881412 plopp-24.4.0/tests/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/widgets/box_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/widgets/checkboxes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/widgets/clip3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/widgets/cut3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/widgets/slice_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-16 14:08:37.000000 plopp-24.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.289464 plopp-24.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-24 12:02:52.000000 plopp-24.5.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.241464 plopp-24.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-24 12:02:52.000000 plopp-24.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.245464 plopp-24.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-24 12:02:52.000000 plopp-24.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-24 12:02:52.000000 plopp-24.5.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-24 12:02:52.000000 plopp-24.5.0/.github/workflows/nightly_at_main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-24 12:02:52.000000 plopp-24.5.0/.github/workflows/nightly_at_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-24 12:02:52.000000 plopp-24.5.0/.github/workflows/python-version-ci
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-24 12:02:52.000000 plopp-24.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-24 12:02:52.000000 plopp-24.5.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-24 12:02:52.000000 plopp-24.5.0/.github/workflows/unpinned.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-24 12:02:52.000000 plopp-24.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-24 12:02:52.000000 plopp-24.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-24 12:02:52.000000 plopp-24.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-24 12:02:52.000000 plopp-24.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-24 12:02:52.000000 plopp-24.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 12:02:52.000000 plopp-24.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-24 12:02:57.289464 plopp-24.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-24 12:02:52.000000 plopp-24.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.245464 plopp-24.5.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-24 12:02:52.000000 plopp-24.5.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.245464 plopp-24.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.245464 plopp-24.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/anaconda-icon.js
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/circle-exclamation.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.249464 plopp-24.5.0/docs/_static/customization/
+-rw-r--r--   0 runner    (1001) docker     (127)   114427 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/customization/custom-interfaces.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44133 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/customization/graph-node-tips.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54880 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/customization/subplots.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19228 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/customization/tweaking-figures.png
+-rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.249464 plopp-24.5.0/docs/_static/gallery/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/gallery/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   211913 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/gallery/peeling-layers-thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18766 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/gallery/scatter3d-with-slider-thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66718 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76311 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    76253 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.249464 plopp-24.5.0/docs/_static/plot-types/
+-rw-r--r--   0 runner    (1001) docker     (127)    37065 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/plot-types/image-plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47635 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/plot-types/inspector-plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15510 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/plot-types/line-plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    72368 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/plot-types/scatter-plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)   186659 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/plot-types/scatter3d-plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55181 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/plot-types/slicer-plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50020 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_static/plot-types/super-plot.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.253464 plopp-24.5.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_templates/class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_templates/doc_version.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_templates/module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_templates/scipp-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/_templates/scipp-module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.253464 plopp-24.5.0/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/about/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.253464 plopp-24.5.0/docs/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/api-reference/matplotlib.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/api-reference/plotly.md
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/api-reference/pythreejs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.253464 plopp-24.5.0/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/developer/coding-conventions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/developer/dependency-management.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/developer/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/developer/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.257464 plopp-24.5.0/docs/gallery/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/gallery/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7835 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/gallery/interactive-masking.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/gallery/masking-a-range.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/gallery/nyc-taxi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/gallery/peeling-layers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/gallery/polar-plots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/gallery/rectangle-selection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/gallery/scatter3d-with-slider.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/gallery/scatter3d-with-threshold.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/gallery/tiled-random-samples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/gallery/updating-scatter.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.257464 plopp-24.5.0/docs/user-guide/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.257464 plopp-24.5.0/docs/user-guide/customization/
+-rw-r--r--   0 runner    (1001) docker     (127)    17775 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/user-guide/customization/custom-interfaces.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/user-guide/customization/graph-node-tips.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/user-guide/customization/subplots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/user-guide/customization/tweaking-figures.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.257464 plopp-24.5.0/docs/user-guide/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/user-guide/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8953 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/user-guide/getting-started/numpy-pandas-xarray.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/user-guide/getting-started/overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/user-guide/getting-started/saving-figures.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/user-guide/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.257464 plopp-24.5.0/docs/user-guide/plot-types/
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/user-guide/plot-types/image-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/user-guide/plot-types/inspector-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/user-guide/plot-types/line-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/user-guide/plot-types/scatter-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/user-guide/plot-types/scatter3d-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/user-guide/plot-types/slicer-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-24 12:02:52.000000 plopp-24.5.0/docs/user-guide/plot-types/super-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-24 12:02:52.000000 plopp-24.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.265464 plopp-24.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/basetest.in
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/basetest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/constraints.in
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/make_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/mini.in
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/mini.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/nightly.in
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/nightly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/noplotly.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/noplotly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/optional.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-24 12:02:52.000000 plopp-24.5.0/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.265464 plopp-24.5.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    53363 2024-05-24 12:02:52.000000 plopp-24.5.0/resources/logo-plopp-2022.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 12:02:57.289464 plopp-24.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.237464 plopp-24.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.265464 plopp-24.5.0/src/plopp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.265464 plopp-24.5.0/src/plopp/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.269464 plopp-24.5.0/src/plopp/backends/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18030 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/matplotlib/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/matplotlib/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/matplotlib/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/matplotlib/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/matplotlib/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/matplotlib/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/matplotlib/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/matplotlib/tiled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/matplotlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.269464 plopp-24.5.0/src/plopp/backends/plotly/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11005 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/plotly/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/plotly/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/plotly/line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.269464 plopp-24.5.0/src/plopp/backends/pythreejs/
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/pythreejs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/pythreejs/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/pythreejs/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/pythreejs/outline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/backends/pythreejs/point_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.273464 plopp-24.5.0/src/plopp/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/core/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/core/limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/core/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/core/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.273464 plopp-24.5.0/src/plopp/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/data/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/data/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/data/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.273464 plopp-24.5.0/src/plopp/graphics/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/graphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/graphics/basefig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/graphics/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/graphics/colormapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/graphics/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/graphics/graphicalview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/graphics/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/graphics/lineview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/graphics/scatter3dview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/graphics/scatterview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/graphics/tiled.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.277464 plopp-24.5.0/src/plopp/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/plotting/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/plotting/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/plotting/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/plotting/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/plotting/scatter3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/plotting/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/plotting/superplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/plotting/xyplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.277464 plopp-24.5.0/src/plopp/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/widgets/checkboxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13989 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/widgets/clip3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/widgets/cut3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/widgets/debounce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/widgets/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/widgets/linesave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/widgets/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/widgets/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/widgets/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-05-24 12:02:52.000000 plopp-24.5.0/src/plopp/widgets/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.285464 plopp-24.5.0/src/plopp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-24 12:02:57.000000 plopp-24.5.0/src/plopp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-05-24 12:02:57.000000 plopp-24.5.0/src/plopp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:02:57.000000 plopp-24.5.0/src/plopp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-24 12:02:57.000000 plopp-24.5.0/src/plopp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 12:02:57.000000 plopp-24.5.0/src/plopp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.281464 plopp-24.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.241464 plopp-24.5.0/tests/backends/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.281464 plopp-24.5.0/tests/backends/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/matplotlib/mpl_canvas_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/matplotlib/mpl_figure_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/matplotlib/mpl_image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/matplotlib/mpl_imageview_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/matplotlib/mpl_interactive_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/matplotlib/mpl_line_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/matplotlib/mpl_lineview_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/matplotlib/mpl_scatter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/matplotlib/mpl_tiled_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/matplotlib/mpl_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.281464 plopp-24.5.0/tests/backends/plotly/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/plotly/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/plotly/plotly_canvas_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/plotly/plotly_figure_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/plotly/plotly_line_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.281464 plopp-24.5.0/tests/backends/pythreejs/
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/pythreejs/pythreejs_canvas_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/pythreejs/pythreejs_figure_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.285464 plopp-24.5.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/core/graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/core/limits_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/core/node_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/core/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.285464 plopp-24.5.0/tests/graphics/
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/graphics/colormapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/graphics/imageview_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/graphics/lineview_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/graphics/scatter3dview_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/graphics/scatterview_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/high_level_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/minimal_plot_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/package_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.285464 plopp-24.5.0/tests/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/plotting/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/plotting/inspector_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12457 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/plotting/plot_1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/plotting/plot_2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/plotting/scatter3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/plotting/scatter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/plotting/slicer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/plotting/superplot_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/plotting/xyplot_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:02:57.285464 plopp-24.5.0/tests/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/widgets/box_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/widgets/checkboxes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/widgets/clip3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/widgets/cut3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-24 12:02:52.000000 plopp-24.5.0/tests/widgets/slice_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-24 12:02:52.000000 plopp-24.5.0/tox.ini
```

### Comparing `plopp-24.4.0/.github/workflows/ci.yml` & `plopp-24.5.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/.github/workflows/docs.yml` & `plopp-24.5.0/.github/workflows/docs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -61,13 +61,13 @@
       - run: tox -e linkcheck
         if: ${{ inputs.linkcheck }}
       - uses: actions/upload-artifact@v4
         with:
           name: docs_html
           path: html/
 
-      - uses: JamesIves/github-pages-deploy-action@v4.5.0
+      - uses: JamesIves/github-pages-deploy-action@v4.6.0
         if: ${{ inputs.publish }}
         with:
           branch: gh-pages
           folder: html
           single-commit: true
```

### Comparing `plopp-24.4.0/.github/workflows/nightly_at_main.yml` & `plopp-24.5.0/.github/workflows/nightly_at_main.yml`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/.github/workflows/nightly_at_release.yml` & `plopp-24.5.0/.github/workflows/nightly_at_release.yml`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/.github/workflows/release.yml` & `plopp-24.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/.github/workflows/test.yml` & `plopp-24.5.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/.github/workflows/unpinned.yml` & `plopp-24.5.0/.github/workflows/unpinned.yml`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/.pre-commit-config.yaml` & `plopp-24.5.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -9,42 +9,29 @@
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
-  - repo: https://github.com/psf/black-pre-commit-mirror
-    rev: 23.11.0
-    hooks:
-      - id: black
   - repo: https://github.com/kynan/nbstripout
     rev: 0.6.0
     hooks:
       - id: nbstripout
         types: [ "jupyter" ]
         args: [ "--drop-empty-cells",
                 "--extra-keys 'metadata.language_info.version cell.metadata.jp-MarkdownHeadingCollapsed cell.metadata.pycharm'" ]
-  - repo: https://github.com/pycqa/flake8
-    rev: 6.1.0
-    hooks:
-      - id: flake8
-        types: ["python"]
-        additional_dependencies: ["flake8-bugbear==23.9.16"]
-  - repo: https://github.com/pycqa/bandit
-    rev: 1.7.5
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.4.3
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
     rev: v2.2.6
     hooks:
       - id: codespell
         additional_dependencies:
           - tomli
   - repo: https://github.com/pre-commit/pygrep-hooks
```

### Comparing `plopp-24.4.0/CODE_OF_CONDUCT.md` & `plopp-24.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/CONTRIBUTING.md` & `plopp-24.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/LICENSE` & `plopp-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/PKG-INFO` & `plopp-24.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plopp
-Version: 24.4.0
+Version: 24.5.0
 Summary: Visualization library for Scipp
 Author: Scipp contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
         
@@ -38,31 +38,32 @@
 Project-URL: Source, https://github.com/scipp/plopp
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.5
 Provides-Extra: scipp
 Requires-Dist: scipp; extra == "scipp"
 Provides-Extra: all
 Requires-Dist: scipp; extra == "all"
 Requires-Dist: ipympl; extra == "all"
 Requires-Dist: pythreejs; extra == "all"
 Requires-Dist: mpltoolbox; extra == "all"
+Requires-Dist: ipywidgets; extra == "all"
+Requires-Dist: graphviz; extra == "all"
 
 <img src="docs/_static/logo.svg" width="50%" />
 
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
 [![PyPI badge](http://img.shields.io/pypi/v/plopp.svg)](https://pypi.python.org/pypi/plopp)
 [![Anaconda-Server Badge](https://anaconda.org/scipp/plopp/badges/version.svg)](https://anaconda.org/scipp/plopp)
 [![Documentation](https://img.shields.io/badge/docs-online-success)](https://scipp.github.io/plopp/)
```

### Comparing `plopp-24.4.0/README.md` & `plopp-24.5.0/README.md`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/conda/meta.yaml` & `plopp-24.5.0/conda/meta.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 
 
 requirements:
   build:
     - setuptools
     - setuptools_scm
   run:
-    - python>=3.9
+    - python>=3.10
+
   {% for package in dependencies %}
     - {% if package == "graphviz" %}python-graphviz{% else %}{{ package }}{% endif %}
   {% endfor %}
 
 
 test:
   imports:
```

### Comparing `plopp-24.4.0/docs/_static/anaconda-icon.js` & `plopp-24.5.0/docs/_static/anaconda-icon.js`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/circle-exclamation.svg` & `plopp-24.5.0/docs/_static/circle-exclamation.svg`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/customization/custom-interfaces.png` & `plopp-24.5.0/docs/_static/customization/custom-interfaces.png`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/customization/graph-node-tips.png` & `plopp-24.5.0/docs/_static/customization/graph-node-tips.png`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/customization/subplots.png` & `plopp-24.5.0/docs/_static/customization/subplots.png`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/customization/tweaking-figures.png` & `plopp-24.5.0/docs/_static/customization/tweaking-figures.png`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/favicon.ico` & `plopp-24.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/gallery/peeling-layers-thumbnail.png` & `plopp-24.5.0/docs/_static/gallery/peeling-layers-thumbnail.png`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/gallery/scatter3d-with-slider-thumbnail.png` & `plopp-24.5.0/docs/_static/gallery/scatter3d-with-slider-thumbnail.png`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png` & `plopp-24.5.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/logo-dark.svg` & `plopp-24.5.0/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/logo.svg` & `plopp-24.5.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/plot-types/image-plot.png` & `plopp-24.5.0/docs/_static/plot-types/image-plot.png`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/plot-types/inspector-plot.png` & `plopp-24.5.0/docs/_static/plot-types/inspector-plot.png`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/plot-types/line-plot.png` & `plopp-24.5.0/docs/_static/plot-types/line-plot.png`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/plot-types/scatter-plot.png` & `plopp-24.5.0/docs/_static/plot-types/scatter-plot.png`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/plot-types/scatter3d-plot.png` & `plopp-24.5.0/docs/_static/plot-types/scatter3d-plot.png`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/plot-types/slicer-plot.png` & `plopp-24.5.0/docs/_static/plot-types/slicer-plot.png`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_static/plot-types/super-plot.png` & `plopp-24.5.0/docs/_static/plot-types/super-plot.png`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_templates/class-template.rst` & `plopp-24.5.0/docs/_templates/class-template.rst`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_templates/module-template.rst` & `plopp-24.5.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_templates/scipp-class-template.rst` & `plopp-24.5.0/docs/_templates/scipp-class-template.rst`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/_templates/scipp-module-template.rst` & `plopp-24.5.0/docs/_templates/scipp-module-template.rst`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/about/index.md` & `plopp-24.5.0/docs/about/index.md`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/api-reference/index.md` & `plopp-24.5.0/docs/api-reference/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 ```{eval-rst}
 .. autosummary::
    :toctree: ../generated
 
    widgets.Box
    widgets.Checkboxes
    widgets.HBar
+   widgets.RangeSliceWidget
    widgets.SliceWidget
    widgets.VBar
 
    widgets.tools.AxesTool
    widgets.tools.ButtonTool
    widgets.tools.CameraTool
    widgets.tools.ColorTool
```

### Comparing `plopp-24.4.0/docs/conf.py` & `plopp-24.5.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import os
 import sys
 from importlib.metadata import version as get_version
 
 sys.path.insert(0, os.path.abspath('.'))
 
 # General information about the project.
-project = u'Plopp'
-copyright = u'2024 Scipp contributors'
-author = u'Scipp contributors'
+project = 'Plopp'
+copyright = '2024 Scipp contributors'
+author = 'Scipp contributors'
 
 html_show_sourcelink = True
 
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
     'sphinx.ext.doctest',
```

### Comparing `plopp-24.4.0/docs/developer/coding-conventions.md` & `plopp-24.5.0/docs/developer/coding-conventions.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Coding conventions
 
 ## Code formatting
 
-There are no explicit code formatting conventions since we use `black` to enforce a format.
+There are no explicit code formatting conventions since we use `ruff` to enforce a format.
 
 ## Docstring format
 
 We use the [NumPy docstring format](https://www.sphinx-doc.org/en/master/usage/extensions/example_numpy.html).
 We use `sphinx-autodocs-typehints` to automatically insert type hints into the docstrings.
 Our format thus deviates from the default NumPy example given by the link above.
 Docstrings should therefore be laid out as follows, including spacing and punctuation:
```

### Comparing `plopp-24.4.0/docs/developer/dependency-management.md` & `plopp-24.5.0/docs/developer/dependency-management.md`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/developer/getting-started.md` & `plopp-24.5.0/docs/developer/getting-started.md`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ## Running tests
 
 `````{tab-set}
 ````{tab-item} tox
 Run the tests using
 
 ```sh
-tox -e py39
+tox -e py310
 ```
 
 (or just `tox` if you want to run all environments).
 
 ````
 ````{tab-item} Manually
 Run the tests using
```

### Comparing `plopp-24.4.0/docs/gallery/index.ipynb` & `plopp-24.5.0/docs/gallery/index.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/gallery/interactive-masking.ipynb` & `plopp-24.5.0/docs/gallery/interactive-masking.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9940175028344671%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'import scipp as sc')], delete: [3, 2]}}, 7: {'source': "*

 * *            '{insert: [(12, "fig = pp.imagefigure(masking_node, norm=\'log\')\\n")], delete: [14, '*

 * *            "1, 0]}}, 8: {'id': 'c3c1343d-845b-4a1f-9f28-978837169aa1', 'source': {insert: [(0, "*

 * *            "'from ipywidgets import HBox\\n'), (1, '\\n')], delete: [7, 6]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.14'}}"}*

```diff
@@ -22,16 +22,15 @@
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
                 "import plopp as pp\n",
-                "import scipp as sc\n",
-                "import numpy as np"
+                "import scipp as sc"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d252eb07-78fc-416b-addc-7b9f273ba7a8",
             "metadata": {
                 "editable": true,
@@ -166,59 +165,57 @@
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "from plopp.widgets import Box\n",
-                "\n",
                 "data_node = pp.Node(da)\n",
                 "\n",
                 "\n",
                 "def apply_masks(da, *masks):\n",
                 "    out = da.copy(deep=False)\n",
                 "    for i, mask in enumerate(masks):\n",
                 "        out.masks[str(i)] = mask\n",
                 "    return out\n",
                 "\n",
                 "\n",
                 "masking_node = pp.Node(apply_masks, data_node)\n",
                 "\n",
-                "fig = pp.figure2d(masking_node, norm='log')\n",
+                "fig = pp.imagefigure(masking_node, norm='log')\n",
                 "\n",
                 "r = RectangleTool(\n",
                 "    figure=fig, input_node=data_node, func=define_mask, destination=masking_node\n",
                 ")\n",
                 "fig.toolbar['roi'] = r"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fcf38064-eafe-407e-818c-e3516bd33195",
+            "id": "c3c1343d-845b-4a1f-9f28-978837169aa1",
             "metadata": {
                 "editable": true,
                 "nbsphinx": "hidden",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
+                "from ipywidgets import HBox\n",
+                "\n",
                 "r.value = True\n",
                 "\n",
                 "r._tool.click(50, 200)\n",
                 "r._tool.click(200, 250)\n",
                 "r._tool.click(30, 50)\n",
                 "r._tool.click(250, 170)\n",
                 "\n",
-                "from ipywidgets import HBox\n",
-                "\n",
                 "fig.children = [\n",
                 "    fig.top_bar,\n",
                 "    HBox([fig.left_bar, fig.canvas.to_image(), fig.right_bar]),\n",
                 "    fig.bottom_bar,\n",
                 "]"
             ]
         },
@@ -316,13 +313,14 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3"
+            "pygments_lexer": "ipython3",
+            "version": "3.10.14"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `plopp-24.4.0/docs/gallery/masking-a-range.ipynb` & `plopp-24.5.0/docs/gallery/masking-a-range.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930854301948052%*

 * *Differences: {"'cells'": '{1: {\'source\': {delete: [3]}}, 5: {\'source\': {insert: [(27, "image = '*

 * *            'pp.imagefigure(mask_node, norm=\'log\')\\n"), (28, "lines = pp.linefigure(sum_node, '*

 * *            'grid=True, ls=\'solid\', marker=\'\')\\n"), (29, \'ipw.VBox([slider, image, '*

 * *            "lines])')], delete: [29, 28, 27]}}, 6: {'source': ['pp.show_graph(lines)']}, 7: "*

 * *            "{'source': {insert: [(2, "*

 * *            '"image.save(\'../_static/gallery/masking-a-range-thumbnail.png\')")], delete: [2]}}}', […]*

```diff
@@ -30,15 +30,14 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
                 "import plopp as pp\n",
                 "import scipp as sc\n",
-                "import numpy as np\n",
                 "import ipywidgets as ipw"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f99ea04f-3b3b-49df-b4a2-99aa9bd8090a",
             "metadata": {
@@ -120,17 +119,17 @@
                 "# Add mask\n",
                 "mask_node = add_mask(da, trunc_range=slider_node)\n",
                 "\n",
                 "# Node that sums along the y dimension\n",
                 "sum_node = pp.Node(sc.sum, mask_node, dim=ydim)\n",
                 "\n",
                 "# Make figures\n",
-                "fig2d = pp.figure2d(mask_node, norm='log')\n",
-                "fig1d = pp.figure1d(sum_node, grid=True, ls='solid', marker='')\n",
-                "ipw.VBox([slider, fig2d, fig1d])"
+                "image = pp.imagefigure(mask_node, norm='log')\n",
+                "lines = pp.linefigure(sum_node, grid=True, ls='solid', marker='')\n",
+                "ipw.VBox([slider, image, lines])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7201be42-c726-43cd-b6ad-65cf8f2941b3",
             "metadata": {
@@ -138,15 +137,15 @@
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "pp.show_graph(fig1d)"
+                "pp.show_graph(lines)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "37373128-b948-4100-a761-87229730c62a",
             "metadata": {
@@ -157,15 +156,15 @@
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# This cell is used to generate the thumbnail for the docs gallery.\n",
                 "# It is hidden from the online documentation.\n",
-                "fig2d.save('../_static/gallery/masking-a-range-thumbnail.png')"
+                "image.save('../_static/gallery/masking-a-range-thumbnail.png')"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -176,13 +175,14 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3"
+            "pygments_lexer": "ipython3",
+            "version": "3.10.14"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `plopp-24.4.0/docs/gallery/nyc-taxi.ipynb` & `plopp-24.5.0/docs/gallery/nyc-taxi.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996843434343434%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(8, "fig2d = pp.imagefigure(slice_node, '*

 * *            'norm=\'log\')\\n"), (17, "fig1d = pp.linefigure(sum_lat, smooth, norm=\'log\')\\n")], '*

 * *            'delete: [17, 8]}}}'}*

```diff
@@ -50,24 +50,24 @@
                 "slider = ipw.IntSlider(description='Hour:', min=0, max=23)\n",
                 "slider_node = pp.widget_node(slider)\n",
                 "\n",
                 "# Node that actually does the slicing\n",
                 "slice_node = pp.Node(lambda da, ind: da['hour', ind], da=data, ind=slider_node)\n",
                 "\n",
                 "# Add a 2D figure to show the NYC map\n",
-                "fig2d = pp.figure2d(slice_node, norm='log')\n",
+                "fig2d = pp.imagefigure(slice_node, norm='log')\n",
                 "\n",
                 "# Add a node after the slicing to sum along the latitude dimension\n",
                 "sum_lat = pp.Node(sc.sum, slice_node, dim='latitude')\n",
                 "\n",
                 "# Add a node after the sum that performs as Gaussian smoothing\n",
                 "smooth = pp.Node(gaussian_filter, sum_lat, sigma=5)\n",
                 "\n",
                 "# Add a 1D figure that will display both raw sum and smoothed data\n",
-                "fig1d = pp.figure1d(sum_lat, smooth, norm='log')\n",
+                "fig1d = pp.linefigure(sum_lat, smooth, norm='log')\n",
                 "\n",
                 "widgets.Box([slider, fig2d, fig1d])  # Container box"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1622d0e3-0f33-45db-a9fd-f112d308e3d0",
```

### Comparing `plopp-24.4.0/docs/gallery/peeling-layers.ipynb` & `plopp-24.5.0/docs/gallery/peeling-layers.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9942336309523809%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, 'import scipp as sc')], delete: [2, 1]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.14'}}"}*

```diff
@@ -28,16 +28,15 @@
                     "slide_type": ""
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import plopp as pp\n",
-                "import scipp as sc\n",
-                "import numpy as np"
+                "import scipp as sc"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "78466f8a-ad5a-49d0-84f2-4c997ed7b4ff",
             "metadata": {
                 "editable": true,
@@ -125,13 +124,14 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3"
+            "pygments_lexer": "ipython3",
+            "version": "3.10.14"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `plopp-24.4.0/docs/gallery/polar-plots.ipynb` & `plopp-24.5.0/docs/gallery/polar-plots.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996290545203589%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(17, 'ax.set_xlim(0, 2 * np.pi)\\n')], delete: [17]}}, 8: "*

 * *            '{\'source\': {insert: [(7, \'    coords={\\n\'), (8, "        \'theta\': '*

 * *            'sc.array(dims=[\'theta\'], values=theta, unit=\'rad\'),\\n"), (9, "        \'phi\': '*

 * *            'sc.array(dims=[\'phi\'], values=phi, unit=\'rad\'),\\n"), (10, \'    },\\n\')], '*

 * *            'delete: [8, 7]}}}'}*

```diff
@@ -44,15 +44,15 @@
                 "\n",
                 "# Construct figure axes with Matplotlib\n",
                 "fig = plt.Figure(figsize=(5, 5))\n",
                 "ax = fig.add_subplot(projection='polar')\n",
                 "\n",
                 "# Make the plot and tweak the axes\n",
                 "p = pp.plot(da, ax=ax)\n",
-                "ax.set_xlim(0, 2*np.pi)\n",
+                "ax.set_xlim(0, 2 * np.pi)\n",
                 "ax.grid(True)\n",
                 "p"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3178873e-a71a-4b66-8eb7-da88113d1f95",
@@ -143,16 +143,18 @@
                 "# Make data\n",
                 "N = 50\n",
                 "r = np.random.normal(loc=50, scale=5, size=(N, N))\n",
                 "theta = np.radians(np.linspace(180, 200, N))\n",
                 "phi = np.radians(np.linspace(0, 90, N))\n",
                 "da = sc.DataArray(\n",
                 "    data=sc.array(dims=['phi', 'theta'], values=r, unit='m'),\n",
-                "    coords={'theta': sc.array(dims=['theta'], values=theta, unit='rad'),\n",
-                "            'phi': sc.array(dims=['phi'], values=phi, unit='rad')},\n",
+                "    coords={\n",
+                "        'theta': sc.array(dims=['theta'], values=theta, unit='rad'),\n",
+                "        'phi': sc.array(dims=['phi'], values=phi, unit='rad'),\n",
+                "    },\n",
                 ")\n",
                 "\n",
                 "# Make axes\n",
                 "fig = plt.figure(figsize=(5, 5))\n",
                 "ax = fig.add_subplot(projection='polar')\n",
                 "ax.set_rorigin(0)\n",
                 "ax.grid(True)\n",
```

### Comparing `plopp-24.4.0/docs/gallery/rectangle-selection.ipynb` & `plopp-24.5.0/docs/gallery/rectangle-selection.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9917756401961565%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict([('editable', True), ('slideshow', "*

 * *            "OrderedDict([('slide_type', '')])), ('tags', [])])}}, 1: {'source': {insert: [(2, "*

 * *            '\'import scipp as sc\')], delete: [3, 2]}}, 7: {\'source\': {insert: [(4, "f2d = '*

 * *            'pp.imagefigure(data_node, norm=\'log\')\\n"), (5, \'f1d = pp.linefigure()\\n\')], '*

 * *            "delete: [5, 4]}}, 8: {'id': '8a372fcb-ffdf-47af-84b3-588926391e8d', 'metadata': "*

 * *            "{'editable': True, 'slide […]*

```diff
@@ -1,13 +1,19 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "da024b16-3a9d-4761-983b-ecb94ef192ad",
-            "metadata": {},
+            "metadata": {
+                "editable": true,
+                "slideshow": {
+                    "slide_type": ""
+                },
+                "tags": []
+            },
             "source": [
                 "# Rectangle selection\n",
                 "\n",
                 "In this example, we will use a custom drawing tool to draw rectangles on a 2D figure.\n",
                 "The data inside the rectangles will be summed along the vertical dimension,\n",
                 "and displayed on a one-dimensional plot below the image."
             ]
@@ -23,16 +29,15 @@
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
                 "import plopp as pp\n",
-                "import scipp as sc\n",
-                "import numpy as np"
+                "import scipp as sc"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d252eb07-78fc-416b-addc-7b9f273ba7a8",
             "metadata": {},
             "source": [
@@ -145,41 +150,46 @@
             },
             "outputs": [],
             "source": [
                 "from plopp.widgets import Box\n",
                 "\n",
                 "data_node = pp.Node(da)\n",
                 "\n",
-                "f2d = pp.figure2d(data_node, norm='log')\n",
-                "f1d = pp.figure1d()\n",
+                "f2d = pp.imagefigure(data_node, norm='log')\n",
+                "f1d = pp.linefigure()\n",
                 "\n",
                 "r = RectangleTool(figure=f2d, input_node=data_node, func=vertical_sum, destination=f1d)\n",
                 "f2d.toolbar['roi'] = r\n",
                 "\n",
                 "box = Box([f2d, f1d])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4b0f4619-6d13-4acf-867e-36ae9f234040",
+            "id": "8a372fcb-ffdf-47af-84b3-588926391e8d",
             "metadata": {
-                "nbsphinx": "hidden"
+                "editable": true,
+                "nbsphinx": "hidden",
+                "slideshow": {
+                    "slide_type": ""
+                },
+                "tags": []
             },
             "outputs": [],
             "source": [
+                "from ipywidgets import HBox\n",
+                "\n",
                 "r.value = True\n",
                 "\n",
                 "r._tool.click(50, 200)\n",
                 "r._tool.click(200, 250)\n",
                 "r._tool.click(30, 50)\n",
                 "r._tool.click(250, 170)\n",
                 "\n",
-                "from ipywidgets import HBox\n",
-                "\n",
                 "f1 = box[0]\n",
                 "f1.children = [\n",
                 "    f1.top_bar,\n",
                 "    HBox([f1.left_bar, f1.canvas.to_image(), f1.right_bar]),\n",
                 "    f1.bottom_bar,\n",
                 "]\n",
                 "f2 = box[1]\n",
@@ -241,13 +251,14 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3"
+            "pygments_lexer": "ipython3",
+            "version": "3.10.14"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `plopp-24.4.0/docs/gallery/scatter3d-with-slider.ipynb` & `plopp-24.5.0/docs/gallery/scatter3d-with-slider.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9700186965811965%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(0, '## Generate data on a curved panel\\n'), (1, '\\n')]}}, "*

 * *            "4: {'source': {insert: [(0, '## A slider selecting a single data slice\\n'), (1, "*

 * *            "'\\n'), (4, 'and a `scatter3dfigure`.')], delete: [2]}}, 5: {'source': {insert: [(6, "*

 * *            "'fig = pp.scatter3dfigure(slice_node, pixel_size=0.3)\\n')], delete: [6]}}, insert: "*

 * *            "[(6, OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'caaa6846-e5b4-4179-9b48-bfb15692dde […]*

```diff
@@ -25,14 +25,16 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f99ea04f-3b3b-49df-b4a2-99aa9bd8090a",
             "metadata": {},
             "source": [
+                "## Generate data on a curved panel\n",
+                "\n",
                 "We first generate some data that represents events detected on a cylindrical detector panel,\n",
                 "as a function of time."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -70,17 +72,19 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "604b3530-76e0-4fb0-88b3-a731ffb5a162",
             "metadata": {},
             "source": [
+                "## A slider selecting a single data slice\n",
+                "\n",
                 "We then construct our interface with a slider,\n",
                 "a node that slices our data at the index of the slider,\n",
-                "and a `figure3d`."
+                "and a `scatter3dfigure`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7be6d610-c6c4-47b5-a7b1-5be4673a775d",
             "metadata": {},
@@ -88,23 +92,57 @@
             "source": [
                 "# Use Plopp's widget to slice dimensions\n",
                 "slider = pw.SliceWidget(da, dims=['time'])\n",
                 "slider_node = pp.widget_node(slider)\n",
                 "\n",
                 "slice_node = pw.slice_dims(data_array=da, slices=slider_node)\n",
                 "\n",
-                "fig = pp.figure3d(slice_node, pixel_size=0.3)\n",
+                "fig = pp.scatter3dfigure(slice_node, pixel_size=0.3)\n",
                 "\n",
                 "# Set slider in the middle so panel isn't all dark\n",
                 "slider.controls['time']['slider'].value = 23\n",
                 "\n",
                 "pp.widgets.Box([fig, slider])"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "caaa6846-e5b4-4179-9b48-bfb15692dde4",
+            "metadata": {},
+            "source": [
+                "## A slider slicing out a range\n",
+                "\n",
+                "It is also possible to use a `RangeSliceWidget` to create a slider with two handles that selects a data range instead of slicing using a single index:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "e6b5f4d3",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Use Plopp's widget to slice dimensions\n",
+                "slider = pw.RangeSliceWidget(da, dims=['time'])\n",
+                "slider_node = pp.widget_node(slider)\n",
+                "\n",
+                "slice_node = pw.slice_dims(data_array=da, slices=slider_node)\n",
+                "\n",
+                "# Sum over the selected range of time dimension\n",
+                "sum_slices = pp.Node(sc.sum, slice_node, dim='time')\n",
+                "\n",
+                "fig = pp.scatter3dfigure(sum_slices, pixel_size=0.3)\n",
+                "\n",
+                "# Set slider in the middle so panel isn't all dark\n",
+                "slider.controls['time']['slider'].value = (0, 12)\n",
+                "\n",
+                "pp.widgets.Box([fig, slider])"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "7e46c83c-9692-4ed3-b125-88c09ebaf76f",
             "metadata": {},
             "outputs": [],
             "source": [
                 "pp.show_graph(fig)"
```

### Comparing `plopp-24.4.0/docs/gallery/scatter3d-with-threshold.ipynb` & `plopp-24.5.0/docs/gallery/scatter3d-with-threshold.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/gallery/tiled-random-samples.ipynb` & `plopp-24.5.0/docs/gallery/tiled-random-samples.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981746031746032%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'from collections.abc import Callable, Generator')], "*

 * *            'delete: [3]}}, 2: {\'source\': {insert: [(22, "    np.random.rayleigh: {\'scale\': '*

 * *            '[2, 3, 4]},\\n"), (24, \'\\n\'), (29, \'    key_arg_pairs = [\\n\'), (30, \'        '*

 * *            "[(key, val) for val in values] for key, values in arguments_map.items()\\n'), (31, "*

 * *            "'    ]\\n'), (34, '\\n'), (38, '\\n'), (41, '    return "*

 * *            '",".join([key_arg_name(key, arg) for […]*

```diff
@@ -14,15 +14,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import scipp as sc\n",
                 "import plopp as pp\n",
-                "from typing import Callable, Generator"
+                "from collections.abc import Callable, Generator"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -45,52 +45,58 @@
                 "    np.random.power: {'a': [1, 2, 4]},\n",
                 "    np.random.triangular: {'left': [0], 'right': [1], 'mode': [0.2, 0.4, 0.8]},\n",
                 "    np.random.vonmises: {'mu': [0], 'kappa': [1, 2, 4]},\n",
                 "    np.random.exponential: {'scale': [1, 2, 3]},\n",
                 "    np.random.wald: {'mean': [1], 'scale': [16, 32, 64]},\n",
                 "    np.random.weibull: {'a': [2, 4, 8, 16]},\n",
                 "    np.random.f: {'dfnum': [100], 'dfden': [100]},\n",
-                "    np.random.rayleigh: {'scale': [2, 3, 4]}\n",
+                "    np.random.rayleigh: {'scale': [2, 3, 4]},\n",
                 "}\n",
                 "\n",
+                "\n",
                 "def generate_kwargs(arguments_map: dict[str, list]) -> Generator[dict, None, None]:\n",
                 "    from itertools import product\n",
                 "\n",
-                "    key_arg_pairs = [[(key, val) for val in values] for key, values in arguments_map.items()]\n",
+                "    key_arg_pairs = [\n",
+                "        [(key, val) for val in values] for key, values in arguments_map.items()\n",
+                "    ]\n",
                 "    for arguments in product(*key_arg_pairs):\n",
                 "        yield {str(args[0]): args[1] for args in arguments}\n",
                 "\n",
+                "\n",
                 "def key_arg_name(key: str, arg) -> str:\n",
                 "    return \": \".join([key, str(arg)])\n",
                 "\n",
+                "\n",
                 "def keys_args_name(**kwargs) -> str:\n",
-                "    return \",\".join([key_arg_name(key, arg) for key, arg in kwargs.items()])\n"
+                "    return \",\".join([key_arg_name(key, arg) for key, arg in kwargs.items()])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Collect samples\n",
                 "def sample_and_hist(pdf: Callable, size: int, **kwargs):\n",
                 "    samples = sc.array(dims=['event'], values=pdf(size=size, **kwargs), unit='1')\n",
-                "    \n",
-                "    return samples.hist(event=10)/len(samples)\n",
                 "\n",
-                "plots = dict()\n",
+                "    return samples.hist(event=10) / len(samples)\n",
+                "\n",
+                "\n",
+                "plots = {}\n",
                 "\n",
                 "for pdf, arguments_map in pdf_maps.items():\n",
                 "    hists = {\n",
                 "        keys_args_name(**kwargs): sample_and_hist(pdf, size=10_000, **kwargs)\n",
-                "        for kwargs in generate_kwargs(arguments_map)    \n",
+                "        for kwargs in generate_kwargs(arguments_map)\n",
                 "    }\n",
                 "    plot = pp.plot(hists, title=f\"{pdf.__name__} distribution\", alpha=0.8, linewidth=4)\n",
-                "    plots[pdf.__name__] = plot\n"
+                "    plots[pdf.__name__] = plot"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `plopp-24.4.0/docs/gallery/updating-scatter.ipynb` & `plopp-24.5.0/docs/gallery/updating-scatter.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985923423423424%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, '\\n'), (9, 'slider = ipw.FloatSlider(\\n'), (10, '    "*

 * *            'min=0,\\n\'), (11, \'    max=60,\\n\'), (12, \'    value=30,\\n\'), (13, "    '*

 * *            'description=\'Position of orange group\',\\n"), (14, "    '*

 * *            'style={\'description_width\': \'initial\'},\\n"), (15, "    layout={\'width\': '*

 * *            '\'500px\'},\\n"), (16, \')\\n\'), (18, \'\\n\'), (25, \'\\n\')], delete: [11, 10, 9, '*

 * *            '8]}}}'}*

```diff
@@ -16,31 +16,38 @@
             "id": "dceddbd2-09ea-43cd-a9ba-0510ccfe1560",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import plopp as pp\n",
                 "import scipp as sc\n",
                 "import ipywidgets as ipw\n",
+                "\n",
                 "%matplotlib widget\n",
                 "\n",
                 "a = pp.Node(pp.data.scatter())\n",
                 "b = pp.Node(pp.data.scatter(seed=2) * 10.0)\n",
                 "\n",
-                "slider = ipw.FloatSlider(min=0, max=60, value=30,\n",
-                "                         description='Position of orange group',\n",
-                "                         style={'description_width': 'initial'},\n",
-                "                         layout={'width': '500px'})\n",
+                "slider = ipw.FloatSlider(\n",
+                "    min=0,\n",
+                "    max=60,\n",
+                "    value=30,\n",
+                "    description='Position of orange group',\n",
+                "    style={'description_width': 'initial'},\n",
+                "    layout={'width': '500px'},\n",
+                ")\n",
                 "slider_node = pp.widget_node(slider)\n",
                 "\n",
+                "\n",
                 "@pp.node\n",
                 "def move(da, x):\n",
                 "    out = da.copy(deep=False)\n",
                 "    out.coords['x'] = da.coords['x'] + sc.scalar(x, unit=da.coords['x'].unit)\n",
                 "    return out\n",
                 "\n",
+                "\n",
                 "move_node = move(da=b, x=slider_node)\n",
                 "\n",
                 "f = pp.scatter({'a': a, 'b': move_node}, cbar=False)\n",
                 "f.bottom_bar.add(slider)\n",
                 "f.canvas.xrange = [-40, 100]\n",
                 "f"
             ]
```

### Comparing `plopp-24.4.0/docs/index.md` & `plopp-24.5.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/user-guide/customization/custom-interfaces.ipynb` & `plopp-24.5.0/docs/user-guide/customization/custom-interfaces.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991125511652472%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(2, 'fig = pp.imagefigure(data_node)\\n')], delete: [2]}}, "*

 * *            "11: {'source': {insert: [(6, 'fig = pp.imagefigure(smooth_node)')], delete: [6]}}, "*

 * *            "17: {'source': {insert: [(9, 'fig = pp.imagefigure(smooth_node)')], delete: [9]}}, "*

 * *            "25: {'source': {insert: [(7, 'fig2d = pp.imagefigure(smooth_node)\\n'), (14, 'fig1d = "*

 * *            "pp.linefigure(sum_raw, sum_smoothed)')], delete: [14, 7]}}, 30: {'source': {insert: "*

 * *            '[(0, […]*

```diff
@@ -78,15 +78,15 @@
             "execution_count": null,
             "id": "424ad72b-5f66-46a2-ad29-9ec67847b5f3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "data_node = pp.Node(da)\n",
                 "\n",
-                "fig = pp.figure2d(data_node)\n",
+                "fig = pp.imagefigure(data_node)\n",
                 "\n",
                 "pp.show_graph(data_node)  # display the graph"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4e299e9a-da48-47bd-bbae-33572c241e79",
@@ -165,15 +165,15 @@
             "source": [
                 "from scipp.scipy.ndimage import gaussian_filter\n",
                 "\n",
                 "data_node = pp.Node(da)\n",
                 "\n",
                 "smooth_node = pp.Node(gaussian_filter, data_node, sigma=5)\n",
                 "\n",
-                "fig = pp.figure2d(smooth_node)"
+                "fig = pp.imagefigure(smooth_node)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "dcd46e8d-947c-4866-b9c1-a0a70ee56774",
             "metadata": {},
             "source": [
@@ -235,15 +235,15 @@
                 "data_node = pp.Node(da)\n",
                 "\n",
                 "slider = ipw.IntSlider(min=1, max=20)\n",
                 "slider_node = pp.widget_node(slider)\n",
                 "\n",
                 "smooth_node = pp.Node(gaussian_filter, data_node, sigma=slider_node)\n",
                 "\n",
-                "fig = pp.figure2d(smooth_node)"
+                "fig = pp.imagefigure(smooth_node)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c671a291-bf40-40f7-9e03-75dbd77997b2",
             "metadata": {},
             "source": [
@@ -331,22 +331,22 @@
                 "data_node = pp.Node(da)\n",
                 "\n",
                 "slider = ipw.IntSlider(min=1, max=20, value=10)\n",
                 "slider_node = pp.widget_node(slider)\n",
                 "\n",
                 "smooth_node = pp.Node(gaussian_filter, data_node, sigma=slider_node)\n",
                 "\n",
-                "fig2d = pp.figure2d(smooth_node)\n",
+                "fig2d = pp.imagefigure(smooth_node)\n",
                 "\n",
                 "# Sum the raw data along the vertical dimension\n",
                 "sum_raw = pp.Node(sc.sum, data_node, dim='y')\n",
                 "# Sum the smoothed data along the vertical dimension\n",
                 "sum_smoothed = pp.Node(sc.sum, smooth_node, dim='y')\n",
                 "# Give two nodes to a figure to display both on the same axes\n",
-                "fig1d = pp.figure1d(sum_raw, sum_smoothed)"
+                "fig1d = pp.linefigure(sum_raw, sum_smoothed)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "36c9ea09-8701-465c-beec-f55d371192ee",
             "metadata": {},
             "source": [
@@ -394,15 +394,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "29a6345c-d530-4278-8896-b6baca81d2aa",
             "metadata": {},
             "outputs": [],
             "source": [
-                "da.masks['close_to_300'] = abs(da.data - sc.scalar(300.0, unit='K')) < sc.scalar(1.0, unit='K')\n",
+                "da.masks['close_to_300'] = abs(da.data - sc.scalar(300.0, unit='K')) < sc.scalar(\n",
+                "    1.0, unit='K'\n",
+                ")\n",
                 "da.masks['large_x'] = da.coords['x'] > sc.scalar(150.0, unit='m')\n",
                 "da"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "38984bbe-b161-4cfd-8994-e69774497555",
@@ -528,27 +530,27 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "6e53a3c6-37eb-4a68-8431-50294dbb789d",
             "metadata": {},
             "source": [
-                "Finally, we add a 2D figure to the `hide_node`,\n",
-                "and a 1D figure after the slicing has been performed."
+                "Finally, we add an image figure to the `hide_node`,\n",
+                "and a line figure after the slicing has been performed."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "b8acfe84-4061-4639-ab44-22edd71d4259",
             "metadata": {},
             "outputs": [],
             "source": [
-                "fig2d = pp.figure2d(hide_node)\n",
-                "fig1d = pp.figure1d(slice_node)\n",
+                "fig2d = pp.imagefigure(hide_node)\n",
+                "fig1d = pp.linefigure(slice_node)\n",
                 "\n",
                 "pp.show_graph(masks_node)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `plopp-24.4.0/docs/user-guide/customization/graph-node-tips.ipynb` & `plopp-24.5.0/docs/user-guide/customization/graph-node-tips.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999737652698179%*

 * *Differences: {"'cells'": "{11: {'source': {insert: [(10, 'fig = pp.linefigure(a)\\n')], delete: [10]}}, 12: "*

 * *            "{'source': {insert: [(9, 'pp.linefigure(diff)')], delete: [9]}}, 13: {'source': "*

 * *            "{insert: [(10, 'All the examples for working with nodes and graphs presented so far "*

 * *            'have been using the lower-level `linefigure`, `imagefigure` and `scatter3dfigure` as '*

 * *            "views for the data.\\n')], delete: [10]}}}"}*

```diff
@@ -142,15 +142,15 @@
                 "# Noisy data\n",
                 "a = pp.Node(\n",
                 "    sc.DataArray(\n",
                 "        data=sc.array(dims=['time'], values=signal),\n",
                 "        coords={'time': sc.arange('time', 100.0, unit='s')},\n",
                 "    )\n",
                 ")\n",
-                "fig = pp.figure1d(a)\n",
+                "fig = pp.linefigure(a)\n",
                 "fig"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9747ac74-cd16-41e2-a82c-9f23b3a59530",
@@ -162,15 +162,15 @@
                 "        data=sc.array(dims=['time'], values=noise),\n",
                 "        coords={'time': sc.arange('time', 100.0, unit='s')},\n",
                 "    )\n",
                 ")\n",
                 "\n",
                 "# Remove noise from signal\n",
                 "diff = a - b\n",
-                "pp.figure1d(diff)"
+                "pp.linefigure(diff)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f1ac8cab-78ca-4a50-b1d5-30144d7cdbb5",
             "metadata": {},
             "source": [
@@ -180,15 +180,15 @@
                 "\n",
                 "<img src=\"../../_static/circle-exclamation.svg\" width=\"16\" height=\"16\" />\n",
                 "&nbsp;\n",
                 "New in version 23.10.0.\n",
                 "\n",
                 "</div>\n",
                 "\n",
-                "All the examples for working with nodes and graphs presented so far have been using the lower-level `figure1d`, `figure2d` and `figure3d` as views for the data.\n",
+                "All the examples for working with nodes and graphs presented so far have been using the lower-level `linefigure`, `imagefigure` and `scatter3dfigure` as views for the data.\n",
                 "\n",
                 "These functions accept graph nodes as input, and provide visualizations for 1D, 2D or scatter 3D data.\n",
                 "\n",
                 "However, say that at the end point of a graph, in the node that is providing the final result, the data still has three dimensions.\n",
                 "One common way of visualizing such data is as a 2D image with a slider to navigate the third dimension.\n",
                 "\n",
                 "Instead of having to manually set up a slider and a node for the slicing,\n",
```

### Comparing `plopp-24.4.0/docs/user-guide/customization/subplots.ipynb` & `plopp-24.5.0/docs/user-guide/customization/subplots.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999007936507937%*

 * *Differences: {"'cells'": "{7: {'source': {delete: [2]}}}"}*

```diff
@@ -110,15 +110,14 @@
             "execution_count": null,
             "id": "40c4c95a-0b3c-4603-be82-f1555bba07bc",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%matplotlib inline\n",
                 "import plopp as pp\n",
-                "import matplotlib.pyplot as plt\n",
                 "\n",
                 "da = pp.data.data3d()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3b377e93-f7a5-4903-9bb2-a90c1844c3c7",
```

### Comparing `plopp-24.4.0/docs/user-guide/customization/tweaking-figures.ipynb` & `plopp-24.5.0/docs/user-guide/customization/tweaking-figures.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/user-guide/getting-started/installation.md` & `plopp-24.5.0/docs/user-guide/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/user-guide/getting-started/numpy-pandas-xarray.ipynb` & `plopp-24.5.0/docs/user-guide/getting-started/numpy-pandas-xarray.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955021121351767%*

 * *Differences: {"'cells'": "{18: {'source': {insert: [(8, 'for x, y in zip(lon, lat, strict=True):\\n')], delete: "*

 * *            '[8]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.14'}}"}*

```diff
@@ -250,15 +250,15 @@
                 "\n",
                 "tool = inspect_plot.children[0].toolbar['inspect']\n",
                 "tool.value = True\n",
                 "\n",
                 "lon = [265, 235, 281]\n",
                 "lat = [42, 32, 23]\n",
                 "\n",
-                "for x, y in zip(lon, lat):\n",
+                "for x, y in zip(lon, lat, strict=True):\n",
                 "    tool._tool.click(x, y)\n",
                 "\n",
                 "\n",
                 "def update(pl):\n",
                 "    from ipywidgets import HBox\n",
                 "\n",
                 "    f1 = pl.children[0]\n",
@@ -300,13 +300,14 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3"
+            "pygments_lexer": "ipython3",
+            "version": "3.10.14"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `plopp-24.4.0/docs/user-guide/getting-started/overview.ipynb` & `plopp-24.5.0/docs/user-guide/getting-started/overview.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/user-guide/getting-started/saving-figures.ipynb` & `plopp-24.5.0/docs/user-guide/getting-started/saving-figures.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/user-guide/index.md` & `plopp-24.5.0/docs/user-guide/index.md`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/user-guide/plot-types/image-plot.ipynb` & `plopp-24.5.0/docs/user-guide/plot-types/image-plot.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996376811594203%*

 * *Differences: {"'cells'": '{19: {\'source\': {insert: [(0, "da.masks[\'yband\'] = abs(da.coords[\'y\'] - '*

 * *            'sc.scalar(20, unit=\'m\')) < sc.scalar(\\n"), (1, "    5, unit=\'m\'\\n"), (2, '*

 * *            "')\\n')], delete: [0]}}}"}*

```diff
@@ -180,15 +180,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8538b35f-a439-4b8a-84f7-e5a305bd3588",
             "metadata": {},
             "outputs": [],
             "source": [
-                "da.masks['yband'] = abs(da.coords['y'] - sc.scalar(20, unit='m')) < sc.scalar(5, unit='m')\n",
+                "da.masks['yband'] = abs(da.coords['y'] - sc.scalar(20, unit='m')) < sc.scalar(\n",
+                "    5, unit='m'\n",
+                ")\n",
                 "da.plot()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "234f96fc-b05c-42e9-8443-67c8c8865560",
             "metadata": {},
```

### Comparing `plopp-24.4.0/docs/user-guide/plot-types/inspector-plot.ipynb` & `plopp-24.5.0/docs/user-guide/plot-types/inspector-plot.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995969742063492%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(8, 'for _ in range(N):\\n')], delete: [8]}}, 7: {'source': "*

 * *            "{insert: [(2, 'for _ in range(N):\\n')], delete: [2]}}}"}*

```diff
@@ -54,15 +54,15 @@
                 "\n",
                 "np.random.seed(123)\n",
                 "N = 3\n",
                 "\n",
                 "tool = p.children[0].toolbar['inspect']\n",
                 "tool.value = True\n",
                 "\n",
-                "for i in range(N):\n",
+                "for _ in range(N):\n",
                 "    x, y = 40 * np.random.random(2)\n",
                 "    tool._tool.click(x, y)\n",
                 "\n",
                 "\n",
                 "def update(pl):\n",
                 "    from ipywidgets import HBox\n",
                 "\n",
@@ -128,15 +128,15 @@
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "outputs": [],
             "source": [
                 "tool = p.children[0].toolbar['inspect']\n",
                 "tool.value = True\n",
-                "for i in range(N):\n",
+                "for _ in range(N):\n",
                 "    x, y = 40 * np.random.random(2)\n",
                 "    tool._tool.click(x, y)\n",
                 "update(p)"
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `plopp-24.4.0/docs/user-guide/plot-types/line-plot.ipynb` & `plopp-24.5.0/docs/user-guide/plot-types/line-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/user-guide/plot-types/scatter-plot.ipynb` & `plopp-24.5.0/docs/user-guide/plot-types/scatter-plot.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994212962962963%*

 * *Differences: {"'cells'": '{11: {\'source\': ["pp.scatter({\'a\': a, \'b\': b}, color={\'a\': \'k\', \'b\': '*

 * *            '\'g\'})"]}}'}*

```diff
@@ -115,16 +115,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6ca3ace6-a4f6-4019-ab4e-bdbfd40373ce",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pp.scatter({'a': a, 'b': b},\n",
-                "          color={'a': 'k', 'b': 'g'})"
+                "pp.scatter({'a': a, 'b': b}, color={'a': 'k', 'b': 'g'})"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f4c0c18e-4ca1-4e7a-8fa5-f87239882fd4",
             "metadata": {},
             "source": [
```

### Comparing `plopp-24.4.0/docs/user-guide/plot-types/scatter3d-plot.ipynb` & `plopp-24.5.0/docs/user-guide/plot-types/scatter3d-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/user-guide/plot-types/slicer-plot.ipynb` & `plopp-24.5.0/docs/user-guide/plot-types/slicer-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/docs/user-guide/plot-types/super-plot.ipynb` & `plopp-24.5.0/docs/user-guide/plot-types/super-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/requirements/base.txt` & `plopp-24.5.0/requirements/base.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # SHA1:4cd3601ec67cc825f41ee1c26350c11397dec7de
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
-fonttools==4.47.2
+fonttools==4.51.0
     # via matplotlib
 kiwisolver==1.4.5
     # via matplotlib
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via -r base.in
-numpy==1.26.3
+numpy==1.26.4
     # via
     #   contourpy
     #   matplotlib
     #   scipp
-packaging==23.2
+packaging==24.0
     # via matplotlib
-pillow==10.2.0
+pillow==10.3.0
     # via matplotlib
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via matplotlib
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via matplotlib
 scipp==24.2.0
     # via -r base.in
 six==1.16.0
     # via python-dateutil
```

### Comparing `plopp-24.4.0/requirements/ci.txt` & `plopp-24.5.0/requirements/ci.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 # SHA1:6344d52635ea11dca331a3bc6eb1833c4c64d585
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-cachetools==5.3.2
+cachetools==5.3.3
     # via tox
 certifi==2024.2.2
     # via requests
 chardet==5.2.0
     # via tox
 charset-normalizer==3.3.2
     # via requests
 colorama==0.4.6
     # via tox
 distlib==0.3.8
     # via virtualenv
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   tox
     #   virtualenv
 gitdb==4.0.11
     # via gitpython
-gitpython==3.1.41
+gitpython==3.1.43
     # via -r ci.in
-idna==3.6
+idna==3.7
     # via requests
-packaging==23.2
+packaging==24.0
     # via
     #   -r ci.in
     #   pyproject-api
     #   tox
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   tox
     #   virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via tox
 pyproject-api==1.6.1
     # via tox
 requests==2.31.0
     # via -r ci.in
 smmap==5.0.1
     # via gitdb
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.12.1
+tox==4.15.0
     # via -r ci.in
-urllib3==2.2.0
+urllib3==2.2.1
     # via requests
-virtualenv==20.25.0
+virtualenv==20.26.2
     # via tox
```

### Comparing `plopp-24.4.0/requirements/constraints.txt` & `plopp-24.5.0/requirements/noplotly.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,53 @@
-# SHA1:e834d540057a673dbbdf8add99b78a7a53d08425
+# SHA1:79cb2f5f444ce019e8436997f3a8111673f38cd4
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
+-r base.txt
+-r basetest.txt
 asttokens==2.4.1
     # via stack-data
-backcall==0.2.0
-    # via ipython
+comm==0.2.2
+    # via ipywidgets
 decorator==5.1.1
     # via ipython
 executing==2.0.1
     # via stack-data
-ipython==8.9.0
-    # via -r constraints.in
+ipython==8.24.0
+    # via ipywidgets
+ipywidgets==8.1.2
+    # via -r noplotly.in
 jedi==0.19.1
     # via ipython
-matplotlib-inline==0.1.6
+jupyterlab-widgets==3.0.10
+    # via ipywidgets
+matplotlib-inline==0.1.7
     # via ipython
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pickleshare==0.7.5
+prompt-toolkit==3.0.43
     # via ipython
-prompt-toolkit==3.0.36
-    # via
-    #   -r constraints.in
-    #   ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pygments==2.17.2
+pygments==2.18.0
     # via ipython
-six==1.16.0
-    # via asttokens
 stack-data==0.6.3
     # via ipython
-traitlets==5.14.1
+traitlets==5.14.3
     # via
+    #   comm
     #   ipython
+    #   ipywidgets
     #   matplotlib-inline
+typing-extensions==4.11.0
+    # via ipython
 wcwidth==0.2.13
     # via prompt-toolkit
+widgetsnbextension==4.0.10
+    # via ipywidgets
```

### Comparing `plopp-24.4.0/requirements/dev.txt` & `plopp-24.5.0/requirements/dev.txt`

 * *Files 25% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 -r docs.txt
 -r mypy.txt
 -r static.txt
 -r test.txt
 -r wheels.txt
 annotated-types==0.6.0
     # via pydantic
-anyio==4.2.0
+anyio==4.3.0
     # via
     #   httpx
     #   jupyter-server
 argon2-cffi==23.1.0
     # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
@@ -28,110 +28,108 @@
     # via jupyterlab
 cffi==1.16.0
     # via argon2-cffi-bindings
 click==8.1.7
     # via
     #   pip-compile-multi
     #   pip-tools
-copier==9.1.1
+copier==9.2.0
     # via -r dev.in
-dunamai==1.19.0
+dunamai==1.21.1
     # via copier
 fqdn==1.5.1
     # via jsonschema
 funcy==2.0
     # via copier
 h11==0.14.0
     # via httpcore
-httpcore==1.0.2
+httpcore==1.0.5
     # via httpx
-httpx==0.26.0
+httpx==0.27.0
     # via jupyterlab
 isoduration==20.11.0
     # via jsonschema
 jinja2-ansible-filters==1.3.2
     # via copier
-json5==0.9.14
+json5==0.9.25
     # via jupyterlab-server
 jsonpointer==2.4
     # via jsonschema
-jsonschema[format-nongpl]==4.21.1
+jsonschema[format-nongpl]==4.22.0
     # via
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
-jupyter-events==0.9.0
+jupyter-events==0.10.0
     # via jupyter-server
-jupyter-lsp==2.2.2
+jupyter-lsp==2.2.5
     # via jupyterlab
-jupyter-server==2.12.5
+jupyter-server==2.14.0
     # via
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   notebook-shim
-jupyter-server-terminals==0.5.2
+jupyter-server-terminals==0.5.3
     # via jupyter-server
-jupyterlab==4.1.0
+jupyterlab==4.2.0
     # via -r dev.in
-jupyterlab-server==2.25.2
+jupyterlab-server==2.27.1
     # via jupyterlab
-notebook-shim==0.2.3
+notebook-shim==0.2.4
     # via jupyterlab
 overrides==7.7.0
     # via jupyter-server
 pathspec==0.12.1
     # via copier
 pip-compile-multi==2.6.3
     # via -r dev.in
-pip-tools==7.3.0
+pip-tools==7.4.1
     # via pip-compile-multi
-plumbum==1.8.2
+plumbum==1.8.3
     # via copier
-prometheus-client==0.19.0
+prometheus-client==0.20.0
     # via jupyter-server
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==2.6.0
+pydantic==2.7.1
     # via copier
-pydantic-core==2.16.1
+pydantic-core==2.18.2
     # via pydantic
 python-json-logger==2.0.7
     # via jupyter-events
-pyyaml-include==1.3.2
-    # via copier
-questionary==2.0.1
+questionary==1.10.0
     # via copier
 rfc3339-validator==0.1.4
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
-send2trash==1.8.2
+send2trash==1.8.3
     # via jupyter-server
-sniffio==1.3.0
+sniffio==1.3.1
     # via
     #   anyio
     #   httpx
-terminado==0.18.0
+terminado==0.18.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
 toposort==1.10
     # via pip-compile-multi
-types-python-dateutil==2.8.19.20240106
+types-python-dateutil==2.9.0.20240316
     # via arrow
 uri-template==1.3.0
     # via jsonschema
 webcolors==1.13
     # via jsonschema
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via jupyter-server
-wheel==0.42.0
+wheel==0.43.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `plopp-24.4.0/requirements/docs.txt` & `plopp-24.5.0/requirements/docs.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,75 +3,75 @@
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r base.txt
 -r optional.txt
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
 alabaster==0.7.16
     # via sphinx
 attrs==23.2.0
     # via
     #   jsonschema
     #   referencing
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   nbconvert
     #   pydata-sphinx-theme
 bleach==6.1.0
     # via nbconvert
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
-debugpy==1.8.0
+debugpy==1.8.1
     # via ipykernel
 defusedxml==0.7.1
     # via nbconvert
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx
 fastjsonschema==2.19.1
     # via nbformat
 gitdb==4.0.11
     # via gitpython
-gitpython==3.1.41
+gitpython==3.1.43
     # via -r docs.in
-h5py==3.10.0
+h5py==3.11.0
     # via -r docs.in
-idna==3.6
+idna==3.7
     # via requests
 imagesize==1.4.1
     # via sphinx
-ipykernel==6.29.0
+ipykernel==6.29.4
     # via -r docs.in
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   myst-parser
     #   nbconvert
     #   nbsphinx
     #   sphinx
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbconvert
     #   nbformat
 jupyterlab-pygments==0.3.0
@@ -80,109 +80,109 @@
     # via
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   nbconvert
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mistune==3.0.2
     # via nbconvert
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via -r docs.in
-nbclient==0.9.0
+nbclient==0.10.0
     # via nbconvert
-nbconvert==7.14.2
+nbconvert==7.16.4
     # via nbsphinx
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   nbclient
     #   nbconvert
     #   nbsphinx
-nbsphinx==0.9.3
+nbsphinx==0.9.4
     # via -r docs.in
 nest-asyncio==1.6.0
     # via ipykernel
 pandocfilters==1.5.1
     # via nbconvert
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   jupyter-core
     #   pooch
-pooch==1.8.0
+pooch==1.8.1
     # via -r docs.in
 psutil==5.9.8
     # via ipykernel
 pydata-sphinx-theme==0.15.2
     # via -r docs.in
 pyyaml==6.0.1
     # via myst-parser
-pyzmq==25.1.2
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
-referencing==0.33.0
+referencing==0.35.1
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   -r docs.in
     #   pooch
     #   sphinx
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
 smmap==5.0.1
     # via gitdb
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   -r docs.in
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
     #   sphinx-copybutton
     #   sphinx-design
     #   sphinx-gallery
-sphinx-autodoc-typehints==1.25.3
+sphinx-autodoc-typehints==2.1.0
     # via -r docs.in
 sphinx-copybutton==0.5.2
     # via -r docs.in
 sphinx-design==0.5.0
     # via -r docs.in
-sphinx-gallery==0.15.0
+sphinx-gallery==0.16.0
     # via -r docs.in
 sphinxcontrib-applehelp==1.0.8
     # via sphinx
 sphinxcontrib-devhelp==1.0.6
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-tinycss2==1.2.1
+tinycss2==1.3.0
     # via nbconvert
+tomli==2.0.1
+    # via sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-typing-extensions==4.9.0
-    # via pydata-sphinx-theme
-urllib3==2.2.0
+urllib3==2.2.1
     # via requests
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
```

### Comparing `plopp-24.4.0/requirements/make_base.py` & `plopp-24.5.0/requirements/make_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import sys
 from argparse import ArgumentParser
 from pathlib import Path
-from typing import List
 
 import tomli
 
 parser = ArgumentParser()
 parser.add_argument(
     "--nightly",
     default="",
@@ -16,15 +15,15 @@
 
 CUSTOM_AUTO_SEPARATOR = """
 # --- END OF CUSTOM SECTION ---
 # The following was generated by 'tox -e deps', DO NOT EDIT MANUALLY!
 """
 
 
-def write_dependencies(dependency_name: str, dependencies: List[str]) -> None:
+def write_dependencies(dependency_name: str, dependencies: list[str]) -> None:
     path = Path(f"{dependency_name}.in")
     if path.exists():
         sections = path.read_text().split(CUSTOM_AUTO_SEPARATOR)
         if len(sections) > 1:
             custom = sections[0]
         else:
             custom = ""
```

### Comparing `plopp-24.4.0/requirements/optional.txt` & `plopp-24.5.0/requirements/optional.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,139 +3,136 @@
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 asttokens==2.4.1
     # via stack-data
-backcall==0.2.0
-    # via ipython
-comm==0.2.1
+comm==0.2.2
     # via ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
 decorator==5.1.1
     # via ipython
+exceptiongroup==1.2.1
+    # via ipython
 executing==2.0.1
     # via stack-data
-fonttools==4.47.2
+fonttools==4.51.0
     # via matplotlib
-graphviz==0.20.1
+graphviz==0.20.3
     # via -r optional.in
 ipydatawidgets==4.3.5
     # via pythreejs
-ipympl==0.9.3
+ipympl==0.9.4
     # via -r optional.in
-ipython==8.9.0
+ipython==8.24.0
     # via
-    #   -c constraints.in
     #   ipympl
     #   ipywidgets
 ipython-genutils==0.2.0
     # via ipympl
-ipywidgets==8.1.1
+ipywidgets==8.1.2
     # via
     #   ipydatawidgets
     #   ipympl
     #   pythreejs
 jedi==0.19.1
     # via ipython
-jupyterlab-widgets==3.0.9
+jupyterlab-widgets==3.0.10
     # via ipywidgets
 kaleido==0.2.1
     # via -r optional.in
 kiwisolver==1.4.5
     # via matplotlib
-matplotlib==3.8.2
+matplotlib==3.9.0
     # via
     #   ipympl
     #   mpltoolbox
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via ipython
-mpltoolbox==23.9.0
+mpltoolbox==24.5.0
     # via -r optional.in
-numpy==1.26.3
+numpy==1.26.4
     # via
     #   contourpy
     #   ipydatawidgets
     #   ipympl
     #   matplotlib
     #   mpltoolbox
     #   pandas
     #   pyarrow
     #   pythreejs
     #   scipy
     #   xarray
-packaging==23.2
+packaging==24.0
     # via
     #   matplotlib
     #   plotly
     #   xarray
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   -r optional.in
     #   xarray
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pickleshare==0.7.5
-    # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   ipympl
     #   matplotlib
-plotly==5.18.0
+plotly==5.22.0
     # via -r optional.in
-prompt-toolkit==3.0.36
-    # via
-    #   -c constraints.in
-    #   ipython
+prompt-toolkit==3.0.43
+    # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.1.0
     # via -r optional.in
-pygments==2.17.2
+pygments==2.18.0
     # via ipython
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via matplotlib
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   matplotlib
     #   pandas
 pythreejs==2.4.2
     # via -r optional.in
 pytz==2024.1
     # via pandas
-scipy==1.12.0
+scipy==1.13.0
     # via -r optional.in
 six==1.16.0
     # via
     #   asttokens
     #   python-dateutil
 stack-data==0.6.3
     # via ipython
-tenacity==8.2.3
+tenacity==8.3.0
     # via plotly
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipympl
     #   ipython
     #   ipywidgets
     #   matplotlib-inline
     #   pythreejs
     #   traittypes
 traittypes==0.2.1
     # via ipydatawidgets
-tzdata==2023.4
+typing-extensions==4.11.0
+    # via ipython
+tzdata==2024.1
     # via pandas
 wcwidth==0.2.13
     # via prompt-toolkit
-widgetsnbextension==4.0.9
+widgetsnbextension==4.0.10
     # via ipywidgets
-xarray==2024.1.1
+xarray==2024.5.0
     # via -r optional.in
```

### Comparing `plopp-24.4.0/resources/logo-plopp-2022.svg` & `plopp-24.5.0/resources/logo-plopp-2022.svg`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/src/plopp/__init__.py` & `plopp-24.5.0/src/plopp/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
-
-# flake8: noqa E402
+# ruff: noqa: E402, F401
 
 import importlib.metadata
 
 try:
     __version__ = importlib.metadata.version(__package__ or __name__)
 except importlib.metadata.PackageNotFoundError:
     __version__ = "0.0.0"
@@ -28,15 +27,15 @@
     tiled,
 )
 from .plotting import inspector, plot, scatter, scatter3d, slicer, superplot, xyplot
 
 del importlib
 
 
-def show():
+def show() -> None:
     """
     A function to display all the currently opened figures (note that this only applies
     to the figures created via the Matplotlib backend).
     See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.show.html for more
     details.
     """
     import matplotlib.pyplot as plt
```

### Comparing `plopp-24.4.0/src/plopp/backends/common.py` & `plopp-24.5.0/src/plopp/backends/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Dict, Literal, Optional, Tuple
+from typing import Literal
 
 import numpy as np
 import scipp as sc
 
 from ..core.limits import find_limits, fix_empty_range
 from ..core.utils import merge_masks
 
@@ -23,18 +23,18 @@
 
 @dataclass
 class BoundingBox:
     """
     A bounding box in 2D space.
     """
 
-    xmin: Optional[float] = None
-    xmax: Optional[float] = None
-    ymin: Optional[float] = None
-    ymax: Optional[float] = None
+    xmin: float | None = None
+    xmax: float | None = None
+    ymin: float | None = None
+    ymax: float | None = None
 
     def union(self, other: BoundingBox) -> BoundingBox:
         """
         Return the union of this bounding box with another one.
         """
 
         return BoundingBox(
@@ -42,19 +42,19 @@
             xmax=_none_max(self.xmax, other.xmax),
             ymin=_none_min(self.ymin, other.ymin),
             ymax=_none_max(self.ymax, other.ymax),
         )
 
 
 def axis_bounds(
-    keys: Tuple[str, str],
+    keys: tuple[str, str],
     x: sc.DataArray,
     scale: Literal['linear', 'log'],
     pad=False,
-) -> Dict[str, float]:
+) -> dict[str, float]:
     """
     Find sensible limits for an axis, depending on linear or log scale.
 
     Parameters
     ----------
     keys:
         The keys to use for constructing a bounding box. The keys should be
@@ -64,15 +64,15 @@
         The data array to find limits for.
     scale:
         The scale of the axis (linear or log).
     pad:
         Whether to pad the limits.
     """
     values = fix_empty_range(find_limits(x, scale=scale, pad=pad))
-    bounds = {k: v for k, v in zip(keys, (val.value for val in values))}
+    bounds = dict(zip(keys, (val.value for val in values), strict=True))
     return bounds
 
 
 def make_line_data(data: sc.DataArray, dim: str) -> dict:
     """
     Prepare data for plotting a line.
     This includes extracting the x and y values, and optionally the error bars and masks
```

### Comparing `plopp-24.4.0/src/plopp/backends/manager.py` & `plopp-24.5.0/src/plopp/backends/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,74 +52,92 @@
     def is_interactive(self):
         return self._backends['2d'].is_interactive()
 
     def canvas2d(self, *args, **kwargs):
         try:
             _canvas2d = self._backends['2d'].canvas2d
         except AttributeError:
-            raise ValueError(f'Unsupported backend \'{self["2d"]}\' for canvas2d.')
+            raise ValueError(
+                f'Unsupported backend \'{self["2d"]}\' for canvas2d.'
+            ) from None
         return _canvas2d(*args, **kwargs)
 
     def canvas3d(self, *args, **kwargs):
         try:
             _canvas3d = self._backends['3d'].canvas3d
         except AttributeError:
-            raise ValueError(f'Unsupported backend \'{self["3d"]}\' for canvas3d.')
+            raise ValueError(
+                f'Unsupported backend \'{self["3d"]}\' for canvas3d.'
+            ) from None
         return _canvas3d(*args, **kwargs)
 
     def line(self, *args, **kwargs):
         try:
             _line = self._backends['2d'].line
         except AttributeError:
-            raise ValueError(f'Unsupported backend \'{self["2d"]}\' for line (1D).')
+            raise ValueError(
+                f'Unsupported backend \'{self["2d"]}\' for line (1D).'
+            ) from None
         return _line(*args, **kwargs)
 
     def image(self, *args, **kwargs):
         try:
             _image = self._backends['2d'].image
         except AttributeError:
-            raise ValueError(f'Unsupported backend \'{self["2d"]}\' for image (2D).')
+            raise ValueError(
+                f'Unsupported backend \'{self["2d"]}\' for image (2D).'
+            ) from None
         return _image(*args, **kwargs)
 
     def scatter(self, *args, **kwargs):
         try:
             _scatter = self._backends['2d'].scatter
         except AttributeError:
-            raise ValueError(f'Unsupported backend \'{self["2d"]}\' for scatter.')
+            raise ValueError(
+                f'Unsupported backend \'{self["2d"]}\' for scatter.'
+            ) from None
         return _scatter(*args, **kwargs)
 
     def point_cloud(self, *args, **kwargs):
         try:
             _point_cloud = self._backends['3d'].point_cloud
         except AttributeError:
             raise ValueError(
                 f'Unsupported backend \'{self["3d"]}\' for point_cloud (3D).'
-            )
+            ) from None
         return _point_cloud(*args, **kwargs)
 
     def figure1d(self, *args, **kwargs):
         try:
             _figure1d = self._backends['2d'].figure1d
         except AttributeError:
-            raise ValueError(f'Unsupported backend \'{self["2d"]}\' for figure1d.')
+            raise ValueError(
+                f'Unsupported backend \'{self["2d"]}\' for figure1d.'
+            ) from None
         return _figure1d(*args, **kwargs)
 
     def figure2d(self, *args, **kwargs):
         try:
             _figure2d = self._backends['2d'].figure2d
         except AttributeError:
-            raise ValueError(f'Unsupported backend \'{self["2d"]}\' for figure2d.')
+            raise ValueError(
+                f'Unsupported backend \'{self["2d"]}\' for figure2d.'
+            ) from None
         return _figure2d(*args, **kwargs)
 
     def figure3d(self, *args, **kwargs):
         try:
             _figure3d = self._backends['3d'].figure3d
         except AttributeError:
-            raise ValueError(f'Unsupported backend \'{self["3d"]}\' for figure3d.')
+            raise ValueError(
+                f'Unsupported backend \'{self["3d"]}\' for figure3d.'
+            ) from None
         return _figure3d(*args, **kwargs)
 
     def tiled(self, *args, **kwargs):
         try:
             _tiled = self._backends['2d'].tiled
         except AttributeError:
-            raise ValueError(f'Unsupported backend \'{self["2d"]}\' for tiled.')
+            raise ValueError(
+                f'Unsupported backend \'{self["2d"]}\' for tiled.'
+            ) from None
         return _tiled(*args, **kwargs)
```

### Comparing `plopp-24.4.0/src/plopp/backends/matplotlib/__init__.py` & `plopp-24.5.0/src/plopp/backends/matplotlib/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,7 +71,10 @@
         return _make_figure(*args, **kwargs)
 
     def tiled(self, *args, **kwargs):
         """ """
         from .tiled import Tiled as TiledMpl
 
         return TiledMpl(*args, **kwargs)
+
+
+__all__ = ["MatplotlibBackend"]
```

### Comparing `plopp-24.4.0/src/plopp/backends/matplotlib/canvas.py` & `plopp-24.5.0/src/plopp/backends/matplotlib/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Literal, Optional, Tuple, Union
+from typing import Literal
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipp as sc
 from matplotlib import dates as mdates
 from matplotlib.collections import QuadMesh
 from mpl_toolkits.axes_grid1 import make_axes_locatable
@@ -15,34 +15,32 @@
 from .utils import fig_to_bytes, is_sphinx_build, make_figure
 
 
 def _to_floats(x: np.ndarray) -> np.ndarray:
     return mdates.date2num(x) if np.issubdtype(x.dtype, np.datetime64) else x
 
 
-def _none_if_not_finite(x: Union[float, int, None]) -> Union[float, int, None]:
+def _none_if_not_finite(x: float | None) -> float | int | None:
     if x is None:
         return None
     return x if np.isfinite(x) else None
 
 
-def _cursor_value_to_variable(
-    x: Union[float, int], dtype: sc.DType, unit: str
-) -> sc.Variable:
+def _cursor_value_to_variable(x: float, dtype: sc.DType, unit: str) -> sc.Variable:
     if dtype == sc.DType.datetime64:
         # Annoying chain of conversion but matplotlib has its own way of converting
         # dates to numbers (number of days since epoch), and num2date returns a python
         # datetime object, while scipp expects a numpy datetime64.
         return sc.scalar(np.datetime64(mdates.num2date(x).replace(tzinfo=None))).to(
             unit=unit
         )
     return sc.scalar(x, unit=unit)
 
 
-def _cursor_formatter(x: Union[float, int], dtype: sc.DType, unit: str) -> str:
+def _cursor_formatter(x: float, dtype: sc.DType, unit: str) -> str:
     if dtype == sc.DType.datetime64:
         return mdates.num2date(x).replace(tzinfo=None).isoformat()
     return scalar_to_string(sc.scalar(x, unit=unit))
 
 
 class Canvas:
     """
@@ -85,23 +83,23 @@
         ``(x, y)`` coordinates of the legend's anchor point in axes coordinates.
     """
 
     def __init__(
         self,
         ax: plt.Axes = None,
         cax: plt.Axes = None,
-        figsize: Optional[Tuple[float, float]] = None,
-        title: str = None,
+        figsize: tuple[float, float] | None = None,
+        title: str | None = None,
         grid: bool = False,
-        vmin: Union[sc.Variable, int, float] = None,
-        vmax: Union[sc.Variable, int, float] = None,
+        vmin: sc.Variable | float = None,
+        vmax: sc.Variable | float = None,
         autoscale: Literal['auto', 'grow'] = 'auto',
         aspect: Literal['auto', 'equal'] = 'auto',
         cbar: bool = False,
-        legend: Union[bool, Tuple[float, float]] = True,
+        legend: bool | tuple[float, float] = True,
         **ignored,
     ):
         # Note on the `**ignored`` keyword arguments: the figure which owns the canvas
         # creates both the canvas and an artist object (Line or Image). The figure
         # accepts keyword arguments, and has to somehow forward them to the canvas and
         # the artist. Since the figure has no detailed knowledge of the underlying
         # backend that implements the canvas, it cannot have specific arguments (such
@@ -214,17 +212,21 @@
                 # Here get_segments() can return empty segments in the case where the
                 # data values are NaN, which we filter out.
                 lengths = np.array([len(segs) for segs in segments])
                 line_mask = sc.array(dims=['x'], values=c._plopp_mask[lengths > 0])
                 line_y = sc.DataArray(
                     data=sc.array(
                         dims=['x', 'y'],
-                        values=np.array([s for (s, l) in zip(segments, lengths) if l])[
-                            ..., 1
-                        ],
+                        values=np.array(
+                            [
+                                s
+                                for (s, length) in zip(segments, lengths, strict=True)
+                                if length
+                            ]
+                        )[..., 1],
                     ),
                     masks={'mask': line_mask},
                 )
                 line_bbox = BoundingBox(
                     **axis_bounds(('ymin', 'ymax'), line_y, self.yscale, pad=True)
                 )
                 bbox = bbox.union(line_bbox)
@@ -429,22 +431,22 @@
         return self.ax.get_xlim()[1]
 
     @xmax.setter
     def xmax(self, value: float):
         self.ax.set_xlim(self.xmin, value)
 
     @property
-    def xrange(self) -> Tuple[float, float]:
+    def xrange(self) -> tuple[float, float]:
         """
         Get or set the range/limits of the x-axis.
         """
         return self.ax.get_xlim()
 
     @xrange.setter
-    def xrange(self, value: Tuple[float, float]):
+    def xrange(self, value: tuple[float, float]):
         self.ax.set_xlim(value)
 
     @property
     def ymin(self) -> float:
         """
         Get or set the lower (bottom) bound of the y-axis.
         """
@@ -462,22 +464,22 @@
         return self.ax.get_ylim()[1]
 
     @ymax.setter
     def ymax(self, value: float):
         self.ax.set_ylim(self.ymin, value)
 
     @property
-    def yrange(self) -> Tuple[float, float]:
+    def yrange(self) -> tuple[float, float]:
         """
         Get or set the range/limits of the y-axis.
         """
         return self.ax.get_ylim()
 
     @yrange.setter
-    def yrange(self, value: Tuple[float, float]):
+    def yrange(self, value: tuple[float, float]):
         self.ax.set_ylim(value)
 
     @property
     def grid(self) -> bool:
         """
         Get or set the visibility of the grid.
         """
```

### Comparing `plopp-24.4.0/src/plopp/backends/matplotlib/figure.py` & `plopp-24.5.0/src/plopp/backends/matplotlib/figure.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/src/plopp/backends/matplotlib/image.py` & `plopp-24.5.0/src/plopp/backends/matplotlib/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import uuid
-from typing import Tuple
 
 import numpy as np
 import scipp as sc
 
 from ...core.utils import coord_as_bin_edges, merge_masks, repeat, scalar_to_string
 from .canvas import Canvas
 
@@ -179,15 +178,15 @@
         new_values:
             New data to update the mesh values from.
         """
         self._data = new_values
         self._data_with_bin_edges.data = new_values.data
 
     def format_coord(
-        self, xslice: Tuple[str, sc.Variable], yslice: Tuple[str, sc.Variable]
+        self, xslice: tuple[str, sc.Variable], yslice: tuple[str, sc.Variable]
     ) -> str:
         """
         Format the coordinates of the mouse pointer to show the value of the
         data at that point.
 
         Parameters
         ----------
```

### Comparing `plopp-24.4.0/src/plopp/backends/matplotlib/interactive.py` & `plopp-24.5.0/src/plopp/backends/matplotlib/interactive.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/src/plopp/backends/matplotlib/line.py` & `plopp-24.5.0/src/plopp/backends/matplotlib/line.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import uuid
-from typing import Dict
 
 import numpy as np
 import scipp as sc
 from matplotlib.dates import date2num
 from matplotlib.lines import Line2D
 from numpy.typing import ArrayLike
 
@@ -65,15 +64,15 @@
             data=make_line_data(data=self._data, dim=self._dim),
             number=number,
             **args,
         )
 
     def _make_line(
         self,
-        data: Dict,
+        data: dict,
         number: int,
         errorbars: bool = True,
         mask_color: str = 'black',
         **kwargs,
     ):
         """
         Create either plot markers or a step function, depending on whether the data
```

### Comparing `plopp-24.4.0/src/plopp/backends/matplotlib/scatter.py` & `plopp-24.5.0/src/plopp/backends/matplotlib/scatter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import uuid
-from typing import Optional
 
 import numpy as np
 import scipp as sc
 from matplotlib.lines import Line2D
 
 from ...core.utils import merge_masks
 from .canvas import Canvas
@@ -18,15 +17,15 @@
 
     def __init__(
         self,
         canvas: Canvas,
         data: sc.DataArray,
         x: str = 'x',
         y: str = 'y',
-        size: Optional[str] = None,
+        size: str | None = None,
         number: int = 0,
         mask_color: str = 'black',
         cbar: bool = False,
         **kwargs,
     ):
         self._canvas = canvas
         self._ax = self._canvas.ax
```

### Comparing `plopp-24.4.0/src/plopp/backends/matplotlib/static.py` & `plopp-24.5.0/src/plopp/backends/matplotlib/static.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/src/plopp/backends/matplotlib/tiled.py` & `plopp-24.5.0/src/plopp/backends/matplotlib/tiled.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from __future__ import annotations
 
-from typing import Optional, Tuple, Union
+from typing import Any
 
 import numpy as np
 from matplotlib import gridspec
 
-from ..protocols import FigureLike
+from ...core.typing import FigureLike
 from .static import get_repr_maker
 from .utils import copy_figure, is_interactive_backend, make_figure
 
 
 class Tiled:
     """
     A tiled figure.
@@ -63,42 +63,44 @@
 
     """
 
     def __init__(
         self,
         nrows: int,
         ncols: int,
-        figsize: Optional[Tuple[float, float]] = None,
-        **kwargs,
-    ):
+        figsize: tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> None:
         self.nrows = nrows
         self.ncols = ncols
         self.fig = make_figure(
-            figsize=(min(6.0 * ncols, 15.0), min(4.0 * nrows, 15.0))
-            if figsize is None
-            else figsize,
+            figsize=(
+                (min(6.0 * ncols, 15.0), min(4.0 * nrows, 15.0))
+                if figsize is None
+                else figsize
+            ),
             layout='constrained',
         )
 
         self.gs = gridspec.GridSpec(nrows, ncols, figure=self.fig, **kwargs)
         self.axes = []
         self.views = np.full((nrows, ncols), None)
         self._history = []
 
     def __setitem__(
         self,
-        inds: Union[int, slice, Tuple[int, int], Tuple[slice, slice]],
+        inds: int | slice | tuple[int, int] | tuple[slice, slice],
         view: FigureLike,
-    ):
+    ) -> None:
         new_view = copy_figure(view, ax=self.fig.add_subplot(self.gs[inds]))
         self.views[inds] = new_view
         self._history.append((inds, new_view))
 
     def __getitem__(
-        self, inds: Union[int, slice, Tuple[int, int], Tuple[slice, slice]]
+        self, inds: int | slice | tuple[int, int] | tuple[slice, slice]
     ) -> FigureLike:
         return self.views[inds]
 
     def _repr_mimebundle_(self, include=None, exclude=None) -> dict:
         """
         Mimebundle display representation for jupyter notebooks.
         """
@@ -108,29 +110,29 @@
             out = {'text/plain': f'TiledFigure(nrows={self.nrows}, ncols={self.ncols})'}
             npoints = sum(
                 len(line.get_xdata()) for ax in self.axes for line in ax.lines
             )
             out.update(get_repr_maker(npoints=npoints)(self.fig))
             return out
 
-    def save(self, filename: str, **kwargs):
+    def save(self, filename: str, **kwargs: Any) -> None:
         """
         Save the figure to file.
         The default directory for writing the file is the same as the
         directory where the script or notebook is running.
 
         Parameters
         ----------
         filename:
             Name of the output file. Possible file extensions are ``.jpg``, ``.png``,
             ``.svg``, and ``.pdf``.
         """
         self.fig.savefig(filename, **{**{'bbox_inches': 'tight'}, **kwargs})
 
-    def show(self):
+    def show(self) -> None:
         """
         Make a call to Matplotlib's underlying ``show`` function.
         """
         self.fig.show()
 
     def __add__(self, other: Tiled) -> Tiled:
         if not isinstance(other, self.__class__):
@@ -155,15 +157,15 @@
         for inds, view in self._history:
             out[inds] = view
         for inds, view in other._history:
             out[inds[0] + self.nrows, inds[1]] = view
         return out
 
 
-def hstack(left: Union[Tiled, FigureLike], right: Union[Tiled, FigureLike]) -> Tiled:
+def hstack(left: Tiled | FigureLike, right: Tiled | FigureLike) -> Tiled:
     """
     Display two views side by side.
 
     Parameters
     ----------
     left:
         The view to display on the left.
@@ -183,15 +185,15 @@
         return left + t
     else:
         t = Tiled(1, 1)
         t[0, 0] = left
         return t + right
 
 
-def vstack(top: Union[Tiled, FigureLike], bottom: Union[Tiled, FigureLike]) -> Tiled:
+def vstack(top: Tiled | FigureLike, bottom: Tiled | FigureLike) -> Tiled:
     """
     Display two views on top of each other.
 
     Parameters
     ----------
     top:
         The view to display on the top.
```

### Comparing `plopp-24.4.0/src/plopp/backends/matplotlib/utils.py` & `plopp-24.5.0/src/plopp/backends/matplotlib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from io import BytesIO
-from typing import Literal, Tuple, Union
+from typing import Literal
 
 import matplotlib as mpl
 from matplotlib.pyplot import Figure, _get_backend_mod
 
-from ..protocols import FigureLike
+from ...core.typing import FigureLike
 
 
 def fig_to_bytes(fig: Figure, form: Literal['png', 'svg'] = 'png') -> bytes:
     """
     Convert a Matplotlib figure to png (default) or svg bytes.
 
     Parameters
@@ -25,17 +25,19 @@
     fig.savefig(buf, format=form, bbox_inches='tight')
     buf.seek(0)
     return buf.getvalue()
 
 
 def is_interactive_backend() -> bool:
     """
-    Return `True` if the current backend used by Matplotlib is the widget backend.
+    Return ``True`` if the current backend used by Matplotlib is the widget/ipympl
+    backend.
     """
-    return 'ipympl' in mpl.get_backend()
+    backend = mpl.get_backend()
+    return any(x in backend for x in ("ipympl", "widget"))
 
 
 def make_figure(*args, **kwargs) -> Figure:
     """
     Create a new figure.
 
     If we use ``plt.figure()`` directly, the figures auto-show in the notebooks.
@@ -52,20 +54,20 @@
     if not is_interactive_backend():
         return Figure(*args, **kwargs)
     backend = _get_backend_mod()
     manager = backend.new_figure_manager(1, *args, FigureClass=Figure, **kwargs)
     return manager.canvas.figure
 
 
-def make_legend(leg: Union[bool, Tuple[float, float]]):
+def make_legend(leg: bool | tuple[float, float]):
     """
     Create a dict of arguments to be used in the legend creation.
     """
     leg_args = {}
-    if isinstance(leg, (list, tuple)):
+    if isinstance(leg, list | tuple):
         leg_args = {'loc': leg}
     elif not isinstance(leg, bool):
         raise TypeError(f"Legend must be a bool, tuple, or a list, not {type(leg)}")
     return leg_args
 
 
 def require_interactive_backend(func: str):
```

### Comparing `plopp-24.4.0/src/plopp/backends/plotly/__init__.py` & `plopp-24.5.0/src/plopp/backends/plotly/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,7 +28,10 @@
     def figure1d(self, *args, **kwargs):
         """
         See :class:`figure.Figure` for details.
         """
         from .figure import Figure as FigPlotly
 
         return FigPlotly(*args, **kwargs)
+
+
+__all__ = ["PlotlyBackend"]
```

### Comparing `plopp-24.4.0/src/plopp/backends/plotly/canvas.py` & `plopp-24.5.0/src/plopp/backends/plotly/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Literal, Tuple, Union
+from typing import Literal
 
 import numpy as np
 import scipp as sc
 
 from ...core.utils import maybe_variable_to_number
 from ..common import BoundingBox, axis_bounds
 
@@ -34,18 +34,18 @@
         The behavior of the axis limits. If ``auto``, the limits automatically
         adjusts every time the data changes. If ``grow``, the limits are allowed to
         grow with time but they do not shrink.
     """
 
     def __init__(
         self,
-        figsize: Tuple[float, float] = None,
-        title: str = None,
-        vmin: Union[sc.Variable, int, float] = None,
-        vmax: Union[sc.Variable, int, float] = None,
+        figsize: tuple[float, float] | None = None,
+        title: str | None = None,
+        vmin: sc.Variable | float = None,
+        vmax: sc.Variable | float = None,
         autoscale: Literal['auto', 'grow'] = 'auto',
         **ignored,
     ):
         # Note on the `**ignored`` keyword arguments: the figure which owns the canvas
         # creates both the canvas and an artist object (Line or Image). The figure
         # accepts keyword arguments, and has to somehow forward them to the canvas and
         # the artist. Since the figure has no detailed knowledge of the underlying
@@ -254,22 +254,22 @@
         return self.fig.layout.xaxis.range[1]
 
     @xmax.setter
     def xmax(self, value: float):
         self.fig.layout.xaxis.range = [self.xmin, value]
 
     @property
-    def xrange(self) -> Tuple[float, float]:
+    def xrange(self) -> tuple[float, float]:
         """
         Get or set the range/limits of the x-axis.
         """
         return self.fig.layout.xaxis.range
 
     @xrange.setter
-    def xrange(self, value: Tuple[float, float]):
+    def xrange(self, value: tuple[float, float]):
         self.fig.layout.xaxis.range = value
 
     @property
     def ymin(self) -> float:
         """
         Get or set the lower (bottom) bound of the y-axis.
         """
@@ -287,22 +287,22 @@
         return self.fig.layout.yaxis.range[1]
 
     @ymax.setter
     def ymax(self, value: float):
         self.fig.layout.yaxis.range = [self.ymin, value]
 
     @property
-    def yrange(self) -> Tuple[float, float]:
+    def yrange(self) -> tuple[float, float]:
         """
         Get or set the range/limits of the y-axis.
         """
         return self.fig.layout.yaxis.range
 
     @yrange.setter
-    def yrange(self, value: Tuple[float, float]):
+    def yrange(self, value: tuple[float, float]):
         self.fig.layout.yaxis.range = value
 
     def reset_mode(self):
         """
         Reset the modebar mode to nothing, to disable all zoom/pan tools.
         """
         self.fig.update_layout(dragmode=False)
```

### Comparing `plopp-24.4.0/src/plopp/backends/plotly/figure.py` & `plopp-24.5.0/src/plopp/backends/plotly/figure.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/src/plopp/backends/plotly/line.py` & `plopp-24.5.0/src/plopp/backends/plotly/line.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import uuid
-from typing import Dict
 
 import numpy as np
 import scipp as sc
 
 from ..common import make_line_data
 from .canvas import Canvas
 
@@ -59,15 +58,15 @@
             data=make_line_data(data=self._data, dim=self._dim),
             number=number,
             **args,
         )
 
     def _make_line(
         self,
-        data: Dict,
+        data: dict,
         number: int,
         errorbars: bool = True,
         mask_color: str = 'black',
         mode='markers',
         marker=None,
         **kwargs,
     ):
```

### Comparing `plopp-24.4.0/src/plopp/backends/pythreejs/__init__.py` & `plopp-24.5.0/src/plopp/backends/pythreejs/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,7 +28,10 @@
     def figure3d(self, *args, **kwargs):
         """
         See :class:`figure.Figure` for details.
         """
         from .figure import Figure as FigP3js
 
         return FigP3js(*args, **kwargs)
+
+
+__all__ = ["PythreejsBackend"]
```

### Comparing `plopp-24.4.0/src/plopp/backends/pythreejs/canvas.py` & `plopp-24.5.0/src/plopp/backends/pythreejs/canvas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from copy import copy
-from typing import Any, Optional, Tuple
+from typing import Any
 
 import ipywidgets as ipw
 import numpy as np
 import scipp as sc
 
 from ...graphics import Camera
 
@@ -28,17 +28,17 @@
         to customize the title appearance.
     camera:
         Initial camera configuration (position, target).
     """
 
     def __init__(
         self,
-        figsize: Tuple[int, int] = (600, 400),
-        title: Optional[str] = None,
-        camera: Optional[Camera] = None,
+        figsize: tuple[int, int] = (600, 400),
+        title: str | None = None,
+        camera: Camera | None = None,
     ):
         import pythreejs as p3
 
         self.dims = {}
         self.units = {}
         self.outline = None
         self.axticks = None
@@ -81,28 +81,28 @@
         dtypes:
             The data types of the data.
         """
         self.units = units
         self.dims = dims
         self.dtypes = dtypes
 
-    def make_outline(self, limits: Tuple[sc.Variable, sc.Variable, sc.Variable]):
+    def make_outline(self, limits: tuple[sc.Variable, sc.Variable, sc.Variable]):
         """
         Create an outline box with ticklabels, given a range in the XYZ directions.
         """
         from .outline import Outline
 
         if self.outline is not None:
             self.remove(self.outline)
         self.outline = Outline(limits=limits)
         self.add(self.outline)
         self._update_camera(limits=limits)
         self.axes_3d.scale = [self.camera.far] * 3
 
-    def _update_camera(self, limits: Tuple[sc.Variable, sc.Variable, sc.Variable]):
+    def _update_camera(self, limits: tuple[sc.Variable, sc.Variable, sc.Variable]):
         """
         Update the camera position when a new object is added to the canvas.
         The camera will look at the mean position of all the objects, and its position
         will be far enough from the center to see all the objects.
         This 'Home' position will be backed up so it can be used when resetting the
         camera via the ``home`` function.
         """
@@ -181,27 +181,27 @@
 
     def camera_z_normal(self):
         """
         View scene along the Z normal.
         """
         self._camera_normal(position=self.camera_backup["z_normal"].copy(), ind=2)
 
-    def _camera_normal(self, position: Tuple[float, float, float], ind: int):
+    def _camera_normal(self, position: tuple[float, float, float], ind: int):
         """
         Move camera to requested normal, and flip if current position is equal
         to the requested position.
         """
         if np.allclose(self.camera.position, position):
             position[ind] = 2.0 * self.camera_backup["center"][ind] - position[ind]
         self.move_camera(position=position)
 
     def move_camera(
         self,
-        position: Tuple[float, float, float],
-        look_at: Optional[Tuple[float, float, float]] = None,
+        position: tuple[float, float, float],
+        look_at: tuple[float, float, float] | None = None,
     ):
         """
         Move the camera to the supplied position.
 
         Parameters
         ----------
         position:
```

### Comparing `plopp-24.4.0/src/plopp/backends/pythreejs/figure.py` & `plopp-24.5.0/src/plopp/backends/pythreejs/figure.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/src/plopp/backends/pythreejs/outline.py` & `plopp-24.5.0/src/plopp/backends/pythreejs/outline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import List, Tuple
 
 import numpy as np
 import pythreejs as p3
 from matplotlib import ticker
 from scipp import Variable
 
 from ...core.utils import value_to_string
@@ -15,40 +14,40 @@
     """
     Compute the difference between two bounds along a given axis.
     """
     return (x[axis][1] - x[axis][0]).value
 
 
 def _get_offsets(
-    limits: Tuple[Variable, Variable, Variable], axis: int, ind: int
+    limits: tuple[Variable, Variable, Variable], axis: int, ind: int
 ) -> np.ndarray:
     """
     Compute offsets for 3 dimensions, along the edges of the box.
     """
     offsets = np.array([limits[i][ind].value for i in range(3)])
     offsets[axis] = 0
     return offsets
 
 
-def _make_geometry(limits: Tuple[Variable, Variable, Variable]) -> p3.EdgesGeometry:
+def _make_geometry(limits: tuple[Variable, Variable, Variable]) -> p3.EdgesGeometry:
     """
     Make a geometry to represent the edges of a cubic box.
     """
     return p3.EdgesGeometry(
         p3.BoxBufferGeometry(
             width=_get_delta(limits, axis=0),
             height=_get_delta(limits, axis=1),
             depth=_get_delta(limits, axis=2),
         )
     )
 
 
 def _make_sprite(
     string: str,
-    position: Tuple[float, float, float],
+    position: tuple[float, float, float],
     color: str = "black",
     size: float = 1.0,
 ) -> p3.Sprite:
     """
     Make a text-based sprite for axis tick.
     """
     sm = p3.SpriteMaterial(
@@ -73,15 +72,17 @@
         dimension for that direction, as well as a unit, which will be used to label
         the corresponding axis.
     tick_size:
         A number to scale the tick size.
     """
 
     def __init__(
-        self, limits: Tuple[Variable, Variable, Variable], tick_size: float = None
+        self,
+        limits: tuple[Variable, Variable, Variable],
+        tick_size: float | None = None,
     ):
         center = [var.mean().value for var in limits]
         if tick_size is None:
             tick_size = 0.05 * np.mean([_get_delta(limits, axis=i) for i in range(3)])
 
         self.box = p3.LineSegments(
             geometry=_make_geometry(limits),
@@ -95,15 +96,15 @@
         )
 
         super().__init__()
         for obj in (self.box, self.ticks, self.labels):
             self.add(obj)
 
     def _make_ticks(
-        self, limits: Tuple[Variable, Variable, Variable], tick_size: float
+        self, limits: tuple[Variable, Variable, Variable], tick_size: float
     ) -> p3.Group:
         """
         Create tick labels on outline edges
         """
         ticks_group = p3.Group()
         iden = np.identity(3, dtype=np.float32)
         ticker_ = ticker.MaxNLocator(5)
@@ -119,16 +120,16 @@
                             size=tick_size,
                         )
                     )
         return ticks_group
 
     def _make_labels(
         self,
-        limits: Tuple[Variable, Variable, Variable],
-        center: List[float],
+        limits: tuple[Variable, Variable, Variable],
+        center: list[float],
         tick_size: float,
     ) -> p3.Group:
         """
         Create axes labels (coord dimension and unit) on outline edges
         """
         labels_group = p3.Group()
         for axis in range(3):
```

### Comparing `plopp-24.4.0/src/plopp/backends/pythreejs/point_cloud.py` & `plopp-24.5.0/src/plopp/backends/pythreejs/point_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import uuid
-from typing import Tuple, Union
 
 import numpy as np
 import scipp as sc
 
 
 def _check_ndim(data):
     if data.ndim != 1:
@@ -40,15 +39,15 @@
     def __init__(
         self,
         *,
         x: str,
         y: str,
         z: str,
         data: sc.DataArray,
-        pixel_size: Union[sc.Variable, float, int] = 1,
+        pixel_size: sc.Variable | float = 1,
         opacity: float = 1,
     ):
         """
         Make a point cloud using pythreejs
         """
         import pythreejs as p3
 
@@ -57,15 +56,15 @@
         self._x = x
         self._y = y
         self._z = z
         self._id = uuid.uuid4().hex
 
         self._pixel_size = pixel_size
         if hasattr(self._pixel_size, 'unit'):
-            if len(set([self._data.coords[dim].unit for dim in [x, y, z]])) > 1:
+            if len({self._data.coords[dim].unit for dim in [x, y, z]}) > 1:
                 raise ValueError(
                     f'The supplied pixel_size has unit {self._pixel_size.unit}, but '
                     'the spatial coordinates do not all have the same units. In this '
                     'case the pixel_size should just be a float with no unit.'
                 )
             else:
                 self._pixel_size = self._pixel_size.to(
@@ -122,15 +121,15 @@
         ----------
         new_values:
             New data to update the point cloud values from.
         """
         _check_ndim(new_values)
         self._data = new_values
 
-    def get_limits(self) -> Tuple[sc.Variable, sc.Variable, sc.Variable]:
+    def get_limits(self) -> tuple[sc.Variable, sc.Variable, sc.Variable]:
         """
         Get the spatial extent of all the points in the cloud.
         """
         xcoord = self._data.coords[self._x]
         ycoord = self._data.coords[self._y]
         zcoord = self._data.coords[self._z]
         half_pixel = 0.5 * self._pixel_size
```

### Comparing `plopp-24.4.0/src/plopp/core/graph.py` & `plopp-24.5.0/src/plopp/core/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from html import escape
 from itertools import chain
-from typing import Union
 
 from .node import Node
 from .view import View
 
 
 def _make_graphviz_digraph(*args, **kwargs):
     try:
         from graphviz import Digraph
     except ImportError:
         raise RuntimeError(
             "Failed to import `graphviz`. "
             "Use `pip install graphviz` (requires installed `graphviz` executable) or "
             "`conda install -c conda-forge python-graphviz`."
-        )
+        ) from None
     return Digraph(*args, **kwargs)
 
 
 def _walk_graph(start, nodes, edges, views, labels):
     label = (
         escape(str(start.func)) + '\nid = ' + start.id
         if start.name is None
@@ -90,15 +89,15 @@
                 parent,
                 child,
                 label=labels.get(parent, '') if child not in views else '',
             )
     return dot
 
 
-def show_graph(entry: Union[Node, View], **kwargs):
+def show_graph(entry: Node | View, **kwargs):
     """
     Display the connected nodes and views as a graph.
 
     Parameters
     ----------
     entry:
         An entry point in the graph (node or view). This can be any node/view in the
@@ -115,15 +114,15 @@
     dot.attr('node', shape='box', height='0.1')
     nodes = {}
     edges = {}
     views = {}
     labels = {}
     # If input is a View, get the underlying node
     if hasattr(entry, 'graph_nodes'):
-        entry = list(entry.graph_nodes.values())[0]
+        entry = next(iter(entry.graph_nodes.values()))
     _walk_graph(
         start=entry,
         nodes=nodes,
         edges=edges,
         views=views,
         labels=labels,
     )
```

### Comparing `plopp-24.4.0/src/plopp/core/helpers.py` & `plopp-24.5.0/src/plopp/core/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Callable
+from collections.abc import Callable
+from typing import Any
 
 from .node import Node
 
 
 def node(func: Callable) -> Callable:
     """
     Create a :class:`Node` from a callable.
@@ -13,15 +14,15 @@
 
     Parameters
     ----------
     func:
         The callable to create the :class:`Node`.
     """
 
-    def make_node(*args, **kwargs):
+    def make_node(*args: Any, **kwargs: Any) -> None:
         return Node(func, *args, **kwargs)
 
     return make_node
 
 
 def widget_node(widget) -> Node:
     """
```

### Comparing `plopp-24.4.0/src/plopp/core/limits.py` & `plopp-24.5.0/src/plopp/core/limits.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Literal, Tuple
+from typing import Literal
 
 import numpy as np
 import scipp as sc
 
 from .utils import merge_masks
 
 
 def find_limits(
     x: sc.DataArray,
     scale: Literal['linear', 'log'] = 'linear',
     pad: bool = False,
-) -> Tuple[sc.Variable, sc.Variable]:
+) -> tuple[sc.Variable, sc.Variable]:
     """
     Find sensible limits, depending on linear or log scale.
     If there are no finite values in the array, raise an error.
     If there are no positive values in the array, and the scale is log, fall back to
     some sensible default values.
     """
     is_datetime = x.dtype == sc.DType.datetime64
@@ -65,16 +65,16 @@
             p = (finite_max - finite_min) * delta
             finite_min -= p
             finite_max += p
     return (sc.scalar(finite_min, unit=x.unit), sc.scalar(finite_max, unit=x.unit))
 
 
 def fix_empty_range(
-    lims: Tuple[sc.Variable, sc.Variable]
-) -> Tuple[sc.Variable, sc.Variable]:
+    lims: tuple[sc.Variable, sc.Variable],
+) -> tuple[sc.Variable, sc.Variable]:
     """
     Range correction in case xmin == xmax
     """
     if lims[0].value != lims[1].value:
         return lims
     if lims[0].value == 0.0:
         dx = sc.scalar(0.5, unit=lims[0].unit)
```

### Comparing `plopp-24.4.0/src/plopp/core/node.py` & `plopp-24.5.0/src/plopp/core/node.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from __future__ import annotations
 
 import uuid
 from itertools import chain
-from typing import Any, List, Union
+from typing import Any
 
 from .view import View
 
 
-def _no_replace_append(container: List[Node], item: Node, kind: str):
+def _no_replace_append(container: list[Node], item: Node, kind: str) -> None:
     """
     Append ``item`` to ``container`` if it is not already in it.
     """
     if item in container:
         tpe = 'View' if kind == 'view' else 'Node'
         raise ValueError(f"{tpe} {item} is already a {kind} in {container}.")
     container.append(item)
@@ -34,15 +34,15 @@
     *parents:
         Positional arguments that represent the positional arguments of the function
         ``func``.
     *kwparents:
         Keyword arguments that represent the keyword arguments of the function ``func``.
     """
 
-    def __init__(self, func: Any, *parents, **kwparents):
+    def __init__(self, func: Any, *parents: Any, **kwparents: Any) -> None:
         func_is_callable = callable(func)
         self._input_value = None
         if func_is_callable:
             self.func = func
         else:
             self._input_value = func
             self.func = lambda: func
@@ -62,22 +62,22 @@
                     (f'arg_{i}' for i in range(len(self.parents))),
                     self.kwparents.keys(),
                 )
             )
             fname = getattr(self.func, "__name__", str(self.func))
             self.name = f'{fname}({args_string})'
         else:
-            val_str = f'={repr(func)}' if isinstance(func, (int, float, str)) else ""
+            val_str = f'={func!r}' if isinstance(func, int | float | str) else ""
             self.name = f'Input <{type(func).__name__}{val_str}>'
 
         # Attempt to set children after setting name in case error message is needed
         for parent in chain(self.parents, self.kwparents.values()):
             _no_replace_append(parent.children, self, 'child')
 
-    def __call__(self):
+    def __call__(self) -> Any:
         return self.request_data()
 
     @property
     def id(self) -> str:
         """
         The unique uuid of the node. This differs from the ``name`` which can be any
         string.
@@ -94,32 +94,37 @@
     @property
     def is_input_node(self) -> bool:
         """
         Whether the node is an input node.
         """
         return self._input_value is not None
 
-    def remove(self):
+    def remove(self) -> None:
         """
         Remove the node from the graph.
         This attempts to remove clear the list of parents of the node.
         The operation fails is the node has children, as removing it would leave the
         graph in an ill-defined state.
         """
-        if self.children:
-            raise RuntimeError(
-                f"Cannot delete node because it has children {self.children}."
-            )
+        for child in self.children:
+            if self in child.parents:
+                child.parents.remove(self)
+            child.kwparents = {
+                key: parent for key, parent in child.kwparents.items() if parent != self
+            }
+            child._data = None
+        self.children.clear()
         for view in self.views:
             del view.graph_nodes[self.id]
         for parent in chain(self.parents, self.kwparents.values()):
             parent.children.remove(self)
         self.views.clear()
         self.parents.clear()
         self.kwparents.clear()
+        self._data = None
 
     def request_data(self) -> Any:
         """
         Request data from the node. This in turn requests data from all of the node's
         parents, and passes those results as arguments to the node's own ``func``.
         The result from calling the function is cached, to limit the number of times
         the graph is traversed.
@@ -128,38 +133,38 @@
             args = (parent.request_data() for parent in self.parents)
             kwargs = {
                 key: parent.request_data() for key, parent in self.kwparents.items()
             }
             self._data = self.func(*args, **kwargs)
         return self._data
 
-    def add_parents(self, *parents: Node):
+    def add_parents(self, *parents: Node) -> None:
         """
         Add one or more parents to the node.
         """
         for parent in parents:
             _no_replace_append(self.parents, parent, 'parent')
             _no_replace_append(parent.children, self, 'child')
 
-    def add_kwparents(self, **parents: Node):
+    def add_kwparents(self, **parents: Node) -> None:
         """
         Add one or more keyword parents to the node.
         """
         for key, parent in parents.items():
             self.kwparents[key] = parent
             _no_replace_append(parent.children, self, 'child')
 
-    def add_view(self, view: View):
+    def add_view(self, view: View) -> None:
         """
         Add a view to the node.
         """
         _no_replace_append(self.views, view, 'view')
         view.graph_nodes[self.id] = self
 
-    def notify_children(self, message: Any):
+    def notify_children(self, message: Any) -> None:
         """
         Notify all of the node's children with ``message``.
         Receiving a notification also means that the local copy of the data is
         out-of-date, and it is thus reset.
 
         Parameters
         ----------
@@ -167,45 +172,50 @@
             The message to pass to the children.
         """
         self._data = None
         self.notify_views(message)
         for child in self.children:
             child.notify_children(message)
 
-    def notify_views(self, message: Any):
+    def notify_views(self, message: Any) -> None:
         """
         Notify the node's views with ``message``.
 
         Parameters
         ----------
         message:
             The message to pass to the views.
         """
         for view in self.views:
             view.notify_view({"node_id": self.id, "message": message})
 
+    def __eq__(self, other: Node | Any) -> bool:
+        if not isinstance(other, Node):
+            return False
+        return self.id == other.id
+
     def __repr__(self) -> str:
         return f"Node(name={self.name})"
 
-    def __add__(self, other: Union[Node, Any]) -> Node:
+    def __add__(self, other: Node | Any) -> Node:
         return Node(lambda x, y: x + y, self, other)
 
-    def __radd__(self, other: Union[Node, Any]) -> Node:
+    def __radd__(self, other: Node | Any) -> Node:
         return Node(lambda x, y: x + y, other, self)
 
-    def __sub__(self, other: Union[Node, Any]) -> Node:
+    def __sub__(self, other: Node | Any) -> Node:
         return Node(lambda x, y: x - y, self, other)
 
-    def __rsub__(self, other: Union[Node, Any]) -> Node:
+    def __rsub__(self, other: Node | Any) -> Node:
         return Node(lambda x, y: x - y, other, self)
 
-    def __mul__(self, other: Union[Node, Any]) -> Node:
+    def __mul__(self, other: Node | Any) -> Node:
         return Node(lambda x, y: x * y, self, other)
 
-    def __rmul__(self, other: Union[Node, Any]) -> Node:
+    def __rmul__(self, other: Node | Any) -> Node:
         return Node(lambda x, y: x * y, other, self)
 
-    def __truediv__(self, other: Union[Node, Any]) -> Node:
+    def __truediv__(self, other: Node | Any) -> Node:
         return Node(lambda x, y: x / y, self, other)
 
-    def __rtruediv__(self, other: Union[Node, Any]) -> Node:
+    def __rtruediv__(self, other: Node | Any) -> Node:
         return Node(lambda x, y: x / y, other, self)
```

### Comparing `plopp-24.4.0/src/plopp/core/utils.py` & `plopp-24.5.0/src/plopp/core/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import uuid
 from functools import reduce
-from typing import Dict, Optional, Union
 
 import scipp as sc
 
 
-def coord_as_bin_edges(da: sc.DataArray, key: str, dim: str = None) -> sc.Variable:
+def coord_as_bin_edges(
+    da: sc.DataArray, key: str, dim: str | None = None
+) -> sc.Variable:
     """
     If coordinate ``key`` in DataArray ``da`` is already bin edges, return it unchanged.
     If it is midpoints, return as bin edges.
 
     Parameters
     ----------
     da:
@@ -66,15 +67,15 @@
     new_shape.insert(index, n)
     return x.broadcast(dims=new_dims, shape=new_shape).flatten(
         dims=[dim, dummy_dim], to=dim
     )
 
 
 def maybe_number_to_variable(
-    x: Union[int, float, sc.Variable], unit: Optional[str] = None
+    x: float | sc.Variable, unit: str | None = None
 ) -> sc.Variable:
     """
     If the input is a raw number, convert to a variable.
     If a unit is requested, perform the conversion to that unit before returning.
     If the input is a variable, return it (potentially converted to the requested unit).
 
     Parameters
@@ -82,22 +83,20 @@
     x:
         The input int or float.
     unit:
         The unit to use for the output variable.
     """
     return (
         sc.scalar(x, unit=unit)
-        if isinstance(x, (int, float))
+        if isinstance(x, int | float)
         else (x.to(unit=unit) if unit is not None else x)
     )
 
 
-def maybe_variable_to_number(
-    x: Union[int, float, sc.Variable], unit=None
-) -> Union[int, float]:
+def maybe_variable_to_number(x: float | sc.Variable, unit=None) -> float:
     """
     If the input is a variable, return its value.
     If a unit is requested, perform the conversion to that unit first.
     If the input is a number, return it unchanged.
 
     Parameters
     ----------
@@ -109,15 +108,15 @@
     if hasattr(x, 'unit'):
         if unit is not None:
             x = x.to(unit=unit)
         x = x.values if x.dims else x.value
     return x
 
 
-def name_with_unit(var: sc.Variable, name: str = None) -> str:
+def name_with_unit(var: sc.Variable, name: str | None = None) -> str:
     """
     Make a string from a variable dimension and its unit.
     The variable dimension can be overridden by specifying the ``name`` directly.
 
     Parameters
     ----------
     var:
@@ -132,15 +131,15 @@
         text = str(var.dims[-1])
     if var.unit is not None:
         unit_str = 'datetime' if var.dtype == sc.DType.datetime64 else var.unit
         text += (" " if text else "") + f"[{unit_str}]"
     return text
 
 
-def value_to_string(val: Union[int, float], precision: int = 3) -> str:
+def value_to_string(val: float, precision: int = 3) -> str:
     """
     Convert a number to a human readable string.
 
     Parameters
     ----------
     val:
         The input number.
@@ -150,15 +149,15 @@
     if (not isinstance(val, float)) or (val == 0):
         text = str(val)
     elif (abs(val) >= 10.0 ** (precision + 1)) or (
         abs(val) <= 10.0 ** (-precision - 1)
     ):
         text = "{val:.{prec}e}".format(val=val, prec=precision)
     else:
-        text = "{}".format(val)
+        text = str(val)
         if len(text) > precision + 2 + (text[0] == '-'):
             text = "{val:.{prec}f}".format(val=val, prec=precision)
     return text
 
 
 def scalar_to_string(var: sc.Variable, precision: int = 3) -> str:
     """
@@ -173,15 +172,15 @@
     """
     out = value_to_string(var.value, precision=precision)
     if (var.unit not in (None, "")) and var.dtype != sc.DType.datetime64:
         out += f" {var.unit}"
     return out
 
 
-def merge_masks(masks: Dict[str, sc.Variable]) -> sc.Variable:
+def merge_masks(masks: dict[str, sc.Variable]) -> sc.Variable:
     """
     Combine all masks into a single one using the OR operation.
 
     Parameters
     ----------
     masks:
         The dict holding the masks to be combined.
@@ -203,17 +202,15 @@
         return value_to_string(x.value) + (f" [{x.unit}]" if x.unit is not None else "")
     out = ':'.join([value_to_string(v) for v in x.values])
     if x.unit is not None:
         out += f" [{x.unit}]"
     return out
 
 
-def make_compatible(
-    x: sc.Variable, *, unit: Union[str, None], dim: Optional[str] = None
-):
+def make_compatible(x: sc.Variable, *, unit: str | None, dim: str | None = None):
     """
     Raise exception if the dimensions of the supplied variable do not contain the
     requested dimension.
     Then, if the variable unit differs from the requested unit, attempt a conversion.
 
     Parameters
     ----------
```

### Comparing `plopp-24.4.0/src/plopp/core/view.py` & `plopp-24.5.0/src/plopp/core/view.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+from __future__ import annotations
 
 import uuid
 from abc import abstractmethod
-from typing import Any, Dict
+from typing import TYPE_CHECKING, Any
+
+if TYPE_CHECKING:
+    from .node import Node
 
 
 class View:
     """
     A (typically graphical) representation of the data.
     A view must be attached to one or more :class:`Node`.
     Upon receiving a notification from a parent node, it usually requests data from that
@@ -15,51 +19,51 @@
 
     Parameters
     ----------
     *nodes:
         The nodes that are attached to the view.
     """
 
-    def __init__(self, *nodes):
+    def __init__(self, *nodes: Node) -> None:
         self._id = uuid.uuid4().hex
         self.graph_nodes = {}
         for node in nodes:
             node.add_view(self)
         self.artists = {}
 
     @property
-    def id(self):
+    def id(self) -> str:
         """
         The unique id of the view.
         """
         return self._id
 
-    def notify_view(self, message: Dict[str, Any]):
+    def notify_view(self, message: dict[str, Any]) -> None:
         """
         When a notification is received, request data from the corresponding parent node
         and update the relevant artist.
 
         Parameters
         ----------
         *message:
             The notification message containing the node id it originated from.
         """
         node_id = message["node_id"]
         new_values = self.graph_nodes[node_id].request_data()
         self.update(**{node_id: new_values})
 
     @abstractmethod
-    def update(self, *args, **kwargs):
+    def update(self, *args: Any, **kwargs: Any) -> None:
         """
         Update function which is called when a notification is received.
         This has to be overridden by any child class.
         """
         ...
 
-    def render(self):
+    def render(self) -> None:
         """
         At the end of figure creation, this function is called to request data from
         all parent nodes and draw the figure.
         """
         self.update(
             **{node.id: node.request_data() for node in self.graph_nodes.values()}
         )
```

### Comparing `plopp-24.4.0/src/plopp/data/examples.py` & `plopp-24.5.0/src/plopp/data/examples.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     rng = np.random.default_rng()
     shape = (npeaks, per_peak)
     x = np.empty(shape)
     y = np.empty(shape)
     xcenters = rng.uniform(0, nx, size=npeaks)
     ycenters = rng.choice([ny / 4, ny / 2, 3 * ny / 4], size=npeaks)
     spreads = rng.uniform(0, spread, size=npeaks)
-    for i, (xc, yc, sp) in enumerate(zip(xcenters, ycenters, spreads)):
+    for i, (xc, yc, sp) in enumerate(zip(xcenters, ycenters, spreads, strict=True)):
         xy = np.random.normal(loc=(xc, yc), scale=sp, size=[per_peak, 2])
         x[i, :] = xy[:, 0]
         y[i, :] = xy[:, 1]
 
     xcoord = sc.array(dims=['row'], values=x.ravel(), unit='cm')
     ycoord = sc.array(dims=['row'], values=y.ravel(), unit='cm')
     table = sc.DataArray(
```

### Comparing `plopp-24.4.0/src/plopp/data/factory.py` & `plopp-24.5.0/src/plopp/data/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import List, Optional
 
 import numpy as np
 import scipp as sc
 
 default_dim_list = ['x', 'y', 'z', 'time', 'temperature']
 
 
 def variable(
     ndim: int = 1,
     variances: bool = False,
     dtype: str = 'float64',
     unit: str = 'm/s',
-    dims: Optional[List[str]] = None,
-    dim_list: List[str] = default_dim_list,
+    dims: list[str] | None = None,
+    dim_list: list[str] = default_dim_list,
 ) -> sc.Variable:
     """
     Generate a sample ``Variable`` containing data based on a sine function.
 
     Parameters
     ----------
     ndim:
@@ -57,16 +56,16 @@
     variances: bool = False,
     binedges: bool = False,
     labels: bool = False,
     masks: bool = False,
     ragged: bool = False,
     dtype: str = 'float64',
     unit: str = 'm/s',
-    dims: Optional[List[str]] = None,
-    dim_list: List[str] = default_dim_list,
+    dims: list[str] | None = None,
+    dim_list: list[str] = default_dim_list,
 ) -> sc.DataArray:
     """
     Generate a sample ``DataArray`` containing data based on a sine function, with
     coordinates. Optionally add masks, labels, attributes.
     It is also possible to turn the coordinates into bin-edges, or make a ragged (2d)
     coordinate.
 
@@ -90,15 +89,15 @@
         The output variable's unit.
     dims:
         List of dimension labels. If ``None``, they will be auto-generated.
     dim_list:
         List of dimension labels to use if no ``dims`` are provided.
     """
 
-    coord_units = dict(zip(dim_list, ['m', 'm', 'm', 's', 'K']))
+    coord_units = dict(zip(dim_list, ['m', 'm', 'm', 's', 'K'], strict=True))
 
     data = variable(
         ndim=ndim,
         variances=variances,
         dims=dims,
         dtype=dtype,
         unit=unit,
@@ -135,15 +134,15 @@
         mesh = np.meshgrid(*grid, indexing="ij")
         coord_dict[data.dims[-1]] = sc.array(
             dims=data.dims, values=mesh[-1] + np.indices(mesh[-1].shape)[0]
         )
     return sc.DataArray(data=data, coords=coord_dict, masks=mask_dict)
 
 
-def dataset(entries: List[str] = None, **kwargs) -> sc.Dataset:
+def dataset(entries: list[str] | None = None, **kwargs) -> sc.Dataset:
     """
     Generate a sample ``Dataset``. See :func:`data_array` for more options.
 
     Parameters
     ----------
     entries:
         A list of names for the elements of the dataset.
```

### Comparing `plopp-24.4.0/src/plopp/graphics/basefig.py` & `plopp-24.5.0/src/plopp/graphics/basefig.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/src/plopp/graphics/camera.py` & `plopp-24.5.0/src/plopp/graphics/camera.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from collections.abc import Sequence
-from typing import Any, Optional, Tuple, Union
+from typing import Any
 
 import scipp as sc
 
 from ..core.utils import maybe_variable_to_number
 
 
 def _vector_to_tuple(
-    vector: Union[sc.Variable, Sequence[sc.Variable], Sequence[float]]
-) -> Tuple[Union[sc.Variable, float], ...]:
+    vector: sc.Variable | Sequence[sc.Variable] | Sequence[float],
+) -> tuple[sc.Variable | float, ...]:
     if isinstance(vector, sc.Variable):
         return (vector.fields.x, vector.fields.y, vector.fields.z)
     else:
         return tuple(v for v in vector)
 
 
 class Camera:
@@ -37,35 +37,31 @@
     far:
         The distance to the far clipping plane (how far from the camera objects can be
         before they disappear), as a :func:`scipp.scalar` or a single number.
     """
 
     def __init__(
         self,
-        position: Optional[
-            Union[sc.Variable, Sequence[sc.Variable], Sequence[float]]
-        ] = None,
-        look_at: Optional[
-            Union[sc.Variable, Sequence[sc.Variable], Sequence[float]]
-        ] = None,
-        near: Optional[Union[sc.Variable, float]] = None,
-        far: Optional[Union[sc.Variable, float]] = None,
+        position: sc.Variable | Sequence[sc.Variable] | Sequence[float] | None = None,
+        look_at: sc.Variable | Sequence[sc.Variable] | Sequence[float] | None = None,
+        near: sc.Variable | float | None = None,
+        far: sc.Variable | float | None = None,
     ):
         self._parsed_contents = None
         self._raw_contents = {}
         if position is not None:
             self._raw_contents['position'] = _vector_to_tuple(position)
         if look_at is not None:
             self._raw_contents['look_at'] = _vector_to_tuple(look_at)
         if near is not None:
             self._raw_contents['near'] = near
         if far is not None:
             self._raw_contents['far'] = far
 
-    def get(self, key: str, default: Optional[Any] = None) -> Any:
+    def get(self, key: str, default: Any | None = None) -> Any:
         """
         Attribute getter.
         If units have been set, the value will be converted to the specified units.
         Otherwise, the raw value will be returned.
 
         Parameters
         ----------
@@ -91,21 +87,23 @@
             The unit of the x axis.
         yunit:
             The unit of the y axis.
         zunit:
             The unit of the z axis.
         """
         self._parsed_contents = {}
-        for key in set(self._raw_contents) & set(('position', 'look_at')):
+        for key in set(self._raw_contents) & {'position', 'look_at'}:
             self._parsed_contents[key] = tuple(
                 maybe_variable_to_number(x, unit=u)
-                for x, u in zip(self._raw_contents[key], [xunit, yunit, zunit])
+                for x, u in zip(
+                    self._raw_contents[key], [xunit, yunit, zunit], strict=True
+                )
             )
 
-        for key in set(self._raw_contents) & set(('near', 'far')):
+        for key in set(self._raw_contents) & {'near', 'far'}:
             if isinstance(self._raw_contents[key], sc.Variable):
                 if not (xunit == yunit == zunit):
                     raise sc.UnitError(
                         'All axes must have the same unit when specifying a clipping '
                         f'plane with a unit. Units are: {xunit}, {yunit}, {zunit}.'
                     )
             self._parsed_contents[key] = maybe_variable_to_number(
@@ -115,39 +113,39 @@
     def has_units(self) -> bool:
         """
         Check if units have been set.
         """
         return self._parsed_contents is not None
 
     @property
-    def position(self) -> Union[Tuple[float, float, float], None]:
+    def position(self) -> tuple[float, float, float] | None:
         """
         The position of the camera. If camera units have been set, the position returned
         will be converted to the specified units.
         """
         self.get('position')
 
     @property
-    def look_at(self) -> Union[Tuple[float, float, float], None]:
+    def look_at(self) -> tuple[float, float, float] | None:
         """
         The point the camera is looking at. If camera units have been set, the position
         returned will be converted to the specified units.
         """
         self.get('look_at')
 
     @property
-    def near(self) -> Union[float, None]:
+    def near(self) -> float | None:
         """
         The distance to the near clipping plane (how close to the camera objects can be
         before they disappear).
         """
         self.get('near')
 
     @property
-    def far(self) -> Union[float, None]:
+    def far(self) -> float | None:
         """
         The distance to the far clipping plane (how far from the camera objects can be
         before they disappear).
         """
         self.get('far')
 
     def __repr__(self):
```

### Comparing `plopp-24.4.0/src/plopp/graphics/colormapper.py` & `plopp-24.5.0/src/plopp/graphics/colormapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from collections.abc import Iterable
 from copy import copy
 from functools import reduce
-from typing import Any, Literal, Optional, Tuple, Union
+from typing import Any, Literal
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import scipp as sc
 from matplotlib.colorbar import ColorbarBase
 from matplotlib.colors import Colormap, LinearSegmentedColormap, LogNorm, Normalize
 
 from ..backends.matplotlib.utils import fig_to_bytes
 from ..core.limits import find_limits, fix_empty_range
 from ..core.utils import maybe_variable_to_number, merge_masks
-from .common import args_to_update
 
 
-def _get_cmap(name: str, nan_color: str = None) -> Colormap:
+def _get_cmap(name: str, nan_color: str | None = None) -> Colormap:
     """
     Get a colormap object from a colormap name.
 
     Parameters
     ----------
     name:
         Name of the colormap. If the name is just a single html color, this will
@@ -90,24 +89,24 @@
         The color used for representing NAN values.
     figsize:
         The size of the figure next to which the colorbar will be displayed.
     """
 
     def __init__(
         self,
-        canvas: Optional[Any] = None,
+        canvas: Any | None = None,
         cbar: bool = True,
         cmap: str = 'viridis',
         mask_cmap: str = 'gray',
         norm: Literal['linear', 'log'] = 'linear',
         autoscale: Literal['auto', 'grow'] = 'auto',
-        vmin: Optional[Union[sc.Variable, int, float]] = None,
-        vmax: Optional[Union[sc.Variable, int, float]] = None,
-        nan_color: Optional[str] = None,
-        figsize: Optional[Tuple[float, float]] = None,
+        vmin: sc.Variable | float | None = None,
+        vmax: sc.Variable | float | None = None,
+        nan_color: str | None = None,
+        figsize: tuple[float, float] | None = None,
     ):
         self.cax = canvas.cax if canvas is not None else None
         self.cmap = _get_cmap(cmap, nan_color=nan_color)
         self.mask_cmap = _get_cmap(mask_cmap, nan_color=nan_color)
         self.user_vmin = vmin
         self.user_vmax = vmax
         self.vmin = np.inf
@@ -230,15 +229,15 @@
 
     def update(self, *args, **kwargs):
         """
         Update the colorscale bounds taking into account new values,
         by either supplying a dictionary of new data or by keyword arguments.
         We also update the colorbar widget if it exists.
         """
-        new = args_to_update(*args, **kwargs)
+        new = dict(*args, **kwargs)
         for key, data in new.items():
             if self.name is None:
                 self.name = data.name
                 # If name is None, this is the first time update is called
                 if self.user_vmin is not None:
                     self.user_vmin = maybe_variable_to_number(
                         self.user_vmin, unit=self.unit
```

### Comparing `plopp-24.4.0/src/plopp/graphics/figure.py` & `plopp-24.5.0/src/plopp/graphics/figure.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/src/plopp/graphics/graphicalview.py` & `plopp-24.5.0/src/plopp/graphics/graphicalview.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
 
 from ..core import Node, View
 from ..core.utils import make_compatible, name_with_unit
-from .common import args_to_update
 
 
 class GraphicalView(View):
     """
     Base class for graphical 1d and 2d views.
     It is used to represent line plots, scatter plots, and image plots (heatmaps).
     In addition to ``View``, it updates the canvas axes and labels when new data is
@@ -22,15 +21,15 @@
 
     def update(self, *args, **kwargs):
         """
         Update the view with new data by either supplying a dictionary of
         new data or by keyword arguments.
         """
 
-        new = args_to_update(*args, **kwargs)
+        new = dict(*args, **kwargs)
         for key, new_values in new.items():
             if new_values.ndim != self._ndim:
                 raise ValueError(
                     f"Expected {self._ndim} dimension(s), but got {new_values.ndim}."
                 )
 
             coords = {}
```

### Comparing `plopp-24.4.0/src/plopp/graphics/imageview.py` & `plopp-24.5.0/src/plopp/graphics/imageview.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Dict, Literal, Optional, Tuple, Union
+from typing import Literal
 
 import scipp as sc
 
 from .. import backends
+from ..core.typing import FigureLike
 from .colormapper import ColorMapper
 from .graphicalview import GraphicalView
 
 
 class ImageView(GraphicalView):
     """
     ImageView that makes a visual representation of two-dimensional data.
@@ -68,24 +69,24 @@
 
     def __init__(
         self,
         *nodes,
         cmap: str = 'viridis',
         mask_cmap: str = 'gray',
         norm: Literal['linear', 'log'] = 'linear',
-        vmin: Optional[Union[sc.Variable, int, float]] = None,
-        vmax: Optional[Union[sc.Variable, int, float]] = None,
+        vmin: sc.Variable | float | None = None,
+        vmax: sc.Variable | float | None = None,
         autoscale: Literal['auto', 'grow'] = 'auto',
-        scale: Optional[Dict[str, str]] = None,
+        scale: dict[str, str] | None = None,
         aspect: Literal['auto', 'equal'] = 'auto',
         grid: bool = False,
         cbar: bool = True,
-        title: Optional[str] = None,
-        figsize: Optional[Tuple[float, float]] = None,
-        format: Optional[Literal['svg', 'png']] = None,
+        title: str | None = None,
+        figsize: tuple[float, float] | None = None,
+        format: Literal['svg', 'png'] | None = None,
         **kwargs,
     ):
         super().__init__(*nodes)
 
         # Note: the order of dims matters here, reversing it would transpose the image
         self._dims = {'y': None, 'x': None}
         self._ndim = 2
@@ -110,15 +111,15 @@
         self.canvas.autoscale()
         self.canvas.finalize()
 
     def make_artist(self, new_values):
         return backends.image(canvas=self.canvas, data=new_values, **self._kwargs)
 
 
-def imagefigure(*args, **kwargs):
+def imagefigure(*args, **kwargs) -> FigureLike:
     """
     Create a figure to represent two-dimensional data from one or more graph node(s).
 
     .. versionadded:: 24.04.0
 
     Examples
     --------
```

### Comparing `plopp-24.4.0/src/plopp/graphics/lineview.py` & `plopp-24.5.0/src/plopp/graphics/lineview.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Dict, Literal, Optional, Tuple, Union
+from typing import Literal
 
 import scipp as sc
 
 from .. import backends
+from ..core.typing import FigureLike
 from .graphicalview import GraphicalView
 
 
 class LineView(GraphicalView):
     """
     View that makes a visual representation of one-dimensional data.
     It has a :class:`Canvas` and a specialized ``update`` function that generates
@@ -63,26 +64,26 @@
         - ``matplotlib.pyplot.step`` for 1d data with a bin-edge coordinate
     """
 
     def __init__(
         self,
         *nodes,
         norm: Literal['linear', 'log'] = 'linear',
-        vmin: Optional[Union[sc.Variable, int, float]] = None,
-        vmax: Optional[Union[sc.Variable, int, float]] = None,
+        vmin: sc.Variable | float | None = None,
+        vmax: sc.Variable | float | None = None,
         autoscale: Literal['auto', 'grow'] = 'auto',
-        scale: Optional[Dict[str, str]] = None,
+        scale: dict[str, str] | None = None,
         errorbars: bool = True,
         mask_color: str = 'black',
         aspect: Literal['auto', 'equal'] = 'auto',
         grid: bool = False,
-        title: Optional[str] = None,
-        figsize: Tuple[float, float] = None,
-        format: Optional[Literal['svg', 'png']] = None,
-        legend: Union[bool, Tuple[float, float]] = True,
+        title: str | None = None,
+        figsize: tuple[float, float] | None = None,
+        format: Literal['svg', 'png'] | None = None,
+        legend: bool | tuple[float, float] = True,
         **kwargs,
     ):
         super().__init__(*nodes)
 
         self._dims = {'x': None}
         self._ndim = 1
         self._scale = {} if scale is None else scale
@@ -113,15 +114,15 @@
             number=len(self.artists),
             errorbars=self._errorbars,
             mask_color=self._mask_color,
             **self._kwargs,
         )
 
 
-def linefigure(*args, **kwargs):
+def linefigure(*args, **kwargs) -> FigureLike:
     """
     Create a figure to represent one-dimensional data from one or more graph node(s).
 
     .. versionadded:: 24.04.0
 
     Examples
     --------
```

### Comparing `plopp-24.4.0/src/plopp/graphics/scatter3dview.py` & `plopp-24.5.0/src/plopp/graphics/scatter3dview.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Literal, Optional, Tuple, Union
+from typing import Literal
 
 import scipp as sc
 
 from .. import backends
 from ..core import View
+from ..core.typing import FigureLike
 from ..core.utils import make_compatible
 from .camera import Camera
 from .colormapper import ColorMapper
-from .common import args_to_update
 
 
 class Scatter3dView(View):
     """
     View that makes a visual representation of three-dimensional scatter data.
     It has a :class:`Canvas`, a :class:`ColorMapper` and a specialized ``update``
     function that generates :class:`PointCloud` artists.
@@ -59,19 +59,19 @@
         *nodes,
         x: str = 'x',
         y: str = 'y',
         z: str = 'z',
         cmap: str = 'viridis',
         mask_cmap: str = 'gray',
         norm: Literal['linear', 'log'] = 'linear',
-        vmin: Optional[Union[sc.Variable, int, float]] = None,
-        vmax: Optional[Union[sc.Variable, int, float]] = None,
-        figsize: Tuple[int, int] = (600, 400),
-        title: Optional[str] = None,
-        camera: Optional[Camera] = None,
+        vmin: sc.Variable | float | None = None,
+        vmax: sc.Variable | float | None = None,
+        figsize: tuple[int, int] = (600, 400),
+        title: str | None = None,
+        camera: Camera | None = None,
         **kwargs,
     ):
         super().__init__(*nodes)
 
         self._x = x
         self._y = y
         self._z = z
@@ -92,15 +92,15 @@
         self.render()
 
     def update(self, *args, **kwargs):
         """
         Update the view with new point clouds by either supplying a dictionary of
         new data or by keyword arguments.
         """
-        new = args_to_update(*args, **kwargs)
+        new = dict(*args, **kwargs)
         mapping = {'x': self._x, 'y': self._y, 'z': self._z}
         for key, new_values in new.items():
             if self.canvas.empty:
                 self.canvas.set_axes(
                     dims=mapping,
                     units={
                         x: new_values.coords[dim].unit for x, dim in mapping.items()
@@ -128,15 +128,15 @@
                 self.canvas.add(pts.points)
                 if key in self._original_artists:
                     self.canvas.make_outline(limits=self.get_limits())
 
             self.artists[key].update(new_values=new_values)
         self.colormapper.update(**new)
 
-    def get_limits(self) -> Tuple[sc.Variable, sc.Variable, sc.Variable]:
+    def get_limits(self) -> tuple[sc.Variable, sc.Variable, sc.Variable]:
         """
         Get global limits for all the point clouds in the scene.
         """
         xmin = None
         xmax = None
         ymin = None
         ymax = None
@@ -183,15 +183,15 @@
         key:
             The id of the object to be removed.
         """
         self.canvas.remove(self.artists[key].points)
         del self.artists[key]
 
 
-def scatter3dfigure(*args, **kwargs):
+def scatter3dfigure(*args, **kwargs) -> FigureLike:
     """
     Create a figure to represent three-dimensional data from one or more graph node(s).
 
     .. versionadded:: 24.04.0
 
     Examples
     --------
```

### Comparing `plopp-24.4.0/src/plopp/graphics/scatterview.py` & `plopp-24.5.0/src/plopp/graphics/scatterview.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
 
-from typing import Dict, Literal, Optional, Tuple, Union
+from typing import Literal
 
 import scipp as sc
 
 from .. import backends
+from ..core.typing import FigureLike
 from .colormapper import ColorMapper
 from .graphicalview import GraphicalView
 
 
 class ScatterView(GraphicalView):
     """ """
 
     def __init__(
         self,
         *nodes,
         x: str = 'x',
         y: str = 'y',
-        size: Optional[str] = None,
+        size: str | None = None,
         norm: Literal['linear', 'log'] = 'linear',
-        vmin: Optional[Union[sc.Variable, int, float]] = None,
-        vmax: Optional[Union[sc.Variable, int, float]] = None,
+        vmin: sc.Variable | float | None = None,
+        vmax: sc.Variable | float | None = None,
         autoscale: Literal['auto', 'grow'] = 'auto',
-        scale: Optional[Dict[str, str]] = None,
+        scale: dict[str, str] | None = None,
         mask_color: str = 'black',
         aspect: Literal['auto', 'equal'] = 'auto',
         grid: bool = False,
-        title: Optional[str] = None,
-        figsize: Tuple[float, float] = None,
-        format: Optional[Literal['svg', 'png']] = None,
-        legend: Union[bool, Tuple[float, float]] = True,
+        title: str | None = None,
+        figsize: tuple[float, float] | None = None,
+        format: Literal['svg', 'png'] | None = None,
+        legend: bool | tuple[float, float] = True,
         cmap: str = 'viridis',
         mask_cmap: str = 'gray',
         cbar: bool = False,
         **kwargs,
     ):
         super().__init__(*nodes)
 
@@ -85,15 +86,15 @@
             number=len(self.artists),
             mask_color=self._mask_color,
             cbar=self._cbar,
             **self._kwargs,
         )
 
 
-def scatterfigure(*args, **kwargs):
+def scatterfigure(*args, **kwargs) -> FigureLike:
     """
     Create a figure to represent scatter data from one or more graph node(s).
 
     .. versionadded:: 24.04.0
 
     Examples
     --------
```

### Comparing `plopp-24.4.0/src/plopp/graphics/tiled.py` & `plopp-24.5.0/src/plopp/graphics/tiled.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/src/plopp/plotting/common.py` & `plopp-24.5.0/src/plopp/plotting/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import warnings
-from typing import Any, Callable, List, Optional, Union
+from collections.abc import Callable
+from typing import Any
 
 import numpy as np
 import scipp as sc
 
 from .. import backends
 from ..core import Node
 from ..core.typing import Plottable, PlottableMulti
@@ -42,15 +43,15 @@
     if 'pandas' in str(type(obj)):
         return sc.compat.from_pandas(obj)
     if 'xarray' in str(type(obj)):
         return sc.compat.from_xarray(obj)
     return obj
 
 
-def _maybe_to_variable(obj: Union[Plottable, list]) -> Plottable:
+def _maybe_to_variable(obj: Plottable | list) -> Plottable:
     """
     Attempt to convert the input to a Variable.
     If the input is either a list or a numpy array, it will be converted.
     Otherwise, the input will be returned unchanged.
     """
     out = obj
     if isinstance(out, list):
@@ -74,15 +75,15 @@
     out = _maybe_to_variable(obj)
     if not isinstance(out, sc.Variable):
         raise TypeError(f"Cannot convert input of type {type(obj)} to a Variable.")
     return out
 
 
 def to_data_array(
-    obj: Union[Plottable, list],
+    obj: Plottable | list,
 ) -> sc.DataArray:
     """
     Convert an input to a DataArray, potentially adding fake coordinates if they are
     missing.
 
     Parameters
     ----------
@@ -151,22 +152,22 @@
     if da.shape != da.values.shape:
         raise TypeError(
             f'The input has dtype {da.dtype} which is not supported by Plopp.'
         )
 
 
 def _all_dims_sorted(var, order='ascending'):
-    return all([sc.allsorted(var, dim, order=order) for dim in var.dims])
+    return all(sc.allsorted(var, dim, order=order) for dim in var.dims)
 
 
 def preprocess(
-    obj: Union[Plottable, list],
-    name: Optional[str] = None,
+    obj: Plottable | list,
+    name: str | None = None,
     ignore_size: bool = False,
-    coords: Optional[List[str]] = None,
+    coords: list[str] | None = None,
 ) -> sc.DataArray:
     """
     Pre-process input data for plotting.
     This involves:
 
       - converting the input to a data array
       - filling in missing dimension coords if needed
@@ -215,15 +216,15 @@
                     stacklevel=2,
                 )
         except sc.DTypeError:
             pass
     return out
 
 
-def input_to_nodes(obj: PlottableMulti, processor: Callable) -> List[Node]:
+def input_to_nodes(obj: PlottableMulti, processor: Callable) -> list[Node]:
     """
     Convert an input or dict of inputs to a list of nodes that provide pre-processed
     data.
 
     Parameters
     ----------
     obj:
@@ -254,9 +255,9 @@
         The name of the function that called this function.
     """
     raise ValueError(
         f'The {origin} function can only plot a single 2d data entry. If you want '
         'to create multiple figures, see the documentation on subplots at '
         'https://scipp.github.io/plopp/customization/subplots.html. If you '
         'want to plot two images onto the same axes, use the lower-level '
-        'plopp.figure2d function.'
+        'plopp.imagefigure function.'
     )
```

### Comparing `plopp-24.4.0/src/plopp/plotting/inspector.py` & `plopp-24.5.0/src/plopp/plotting/inspector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Dict, Literal
+from typing import Literal
 
 import scipp as sc
 
 from ..core import Node
 from ..core.typing import Plottable
 from ..core.utils import coord_as_bin_edges
 from ..graphics import imagefigure, linefigure
@@ -24,23 +24,23 @@
 def _apply_op(da: sc.DataArray, op: str, dim: str) -> sc.DataArray:
     out = getattr(sc, op)(da, dim=dim)
     if out.name:
         out.name = f'{op} of {out.name}'
     return out
 
 
-def _slice_xy(da: sc.DataArray, xy: Dict[str, Dict[str, int]]) -> sc.DataArray:
+def _slice_xy(da: sc.DataArray, xy: dict[str, dict[str, int]]) -> sc.DataArray:
     x = xy['x']
     y = xy['y']
     return da[y['dim'], y['value']][x['dim'], x['value']]
 
 
 def inspector(
     obj: Plottable,
-    dim: str = None,
+    dim: str | None = None,
     *,
     operation: Literal['sum', 'mean', 'min', 'max'] = 'sum',
     orientation: Literal['horizontal', 'vertical'] = 'horizontal',
     **kwargs,
 ):
     """
     Inspector takes in a three-dimensional input and applies a reduction operation
```

### Comparing `plopp-24.4.0/src/plopp/plotting/plot.py` & `plopp-24.5.0/src/plopp/plotting/plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from functools import partial
-from typing import Dict, List, Literal, Optional, Tuple, Union
+from typing import Literal
 
 from scipp import Variable
 
-from ..core.typing import PlottableMulti
+from ..core.typing import FigureLike, PlottableMulti
 from ..graphics import imagefigure, linefigure
 from .common import input_to_nodes, preprocess, raise_multiple_inputs_for_2d_plot_error
 
 
 def plot(
     obj: PlottableMulti,
     *,
     aspect: Literal['auto', 'equal'] = 'auto',
     cbar: bool = True,
-    coords: Optional[List[str]] = None,
+    coords: list[str] | None = None,
     errorbars: bool = True,
-    figsize: Tuple[float, float] = None,
+    figsize: tuple[float, float] | None = None,
     grid: bool = False,
     ignore_size: bool = False,
     mask_color: str = 'black',
     norm: Literal['linear', 'log'] = 'linear',
-    scale: Optional[Dict[str, str]] = None,
-    title: Optional[str] = None,
-    vmin: Optional[Union[Variable, int, float]] = None,
-    vmax: Optional[Union[Variable, int, float]] = None,
+    scale: dict[str, str] | None = None,
+    title: str | None = None,
+    vmin: Variable | float | None = None,
+    vmax: Variable | float | None = None,
     autoscale: Literal['auto', 'grow'] = 'auto',
-    legend: Union[bool, Tuple[float, float]] = True,
+    legend: bool | tuple[float, float] = True,
     **kwargs,
-):
+) -> FigureLike:
     """Plot a Scipp object.
 
     Parameters
     ----------
     obj:
         The object to be plotted.
     aspect:
```

### Comparing `plopp-24.4.0/src/plopp/plotting/scatter.py` & `plopp-24.5.0/src/plopp/plotting/scatter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
 
 import uuid
 from functools import partial
-from typing import Literal, Optional, Tuple, Union
+from typing import Literal
 
 import scipp as sc
 
-from ..core.typing import PlottableMulti
+from ..core.typing import FigureLike, PlottableMulti
 from .common import check_not_binned, from_compatible_lib, input_to_nodes
 
 
 def _preprocess_scatter(
     obj: PlottableMulti,
     x: str,
     y: str,
-    size: Optional[str],
-    name: Optional[str] = None,
+    size: str | None,
+    name: str | None = None,
 ):
     da = from_compatible_lib(obj)
     check_not_binned(da)
 
     cnames = [x, y]
     if size is not None:
         cnames.append(size)
@@ -34,24 +34,24 @@
 
 
 def scatter(
     obj: PlottableMulti,
     *,
     x: str = 'x',
     y: str = 'y',
-    size: Optional[Union[str, float]] = None,
-    figsize: Tuple[float, float] = None,
+    size: str | float | None = None,
+    figsize: tuple[float, float] | None = None,
     norm: Literal['linear', 'log'] = 'linear',
-    title: str = None,
-    vmin: Union[sc.Variable, int, float] = None,
-    vmax: Union[sc.Variable, int, float] = None,
+    title: str | None = None,
+    vmin: sc.Variable | float = None,
+    vmax: sc.Variable | float = None,
     cbar: bool = False,
     cmap: str = 'viridis',
     **kwargs,
-):
+) -> FigureLike:
     """
     Make a two-dimensional scatter plot.
 
     .. versionadded:: 24.04.0
 
     Parameters
     ----------
```

### Comparing `plopp-24.4.0/src/plopp/plotting/scatter3d.py` & `plopp-24.5.0/src/plopp/plotting/scatter3d.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import uuid
 from functools import partial
-from typing import Literal, Optional, Tuple, Union
+from typing import Literal
 
 import scipp as sc
 
-from ..core.typing import PlottableMulti
+from ..core.typing import FigureLike, PlottableMulti
 from ..graphics import Camera
 from .common import check_not_binned, from_compatible_lib, input_to_nodes
 
 
 def _preprocess_scatter(
     obj: PlottableMulti,
     x: str,
     y: str,
     z: str,
-    pos: Optional[str],
-    name: Optional[str] = None,
+    pos: str | None,
+    name: str | None = None,
 ) -> sc.DataArray:
     da = from_compatible_lib(obj)
     check_not_binned(da)
 
     if pos is not None:
         coords = {k: getattr(da.coords[pos].fields, k) for k in (x, y, z)}
     else:
@@ -38,24 +38,24 @@
 
 def scatter3d(
     obj: PlottableMulti,
     *,
     x: str = 'x',
     y: str = 'y',
     z: str = 'z',
-    pos: str = None,
-    figsize: Tuple[int, int] = (600, 400),
+    pos: str | None = None,
+    figsize: tuple[int, int] = (600, 400),
     norm: Literal['linear', 'log'] = 'linear',
-    title: str = None,
-    vmin: Union[sc.Variable, int, float] = None,
-    vmax: Union[sc.Variable, int, float] = None,
+    title: str | None = None,
+    vmin: sc.Variable | float = None,
+    vmax: sc.Variable | float = None,
     cmap: str = 'viridis',
-    camera: Optional[Camera] = None,
+    camera: Camera | None = None,
     **kwargs,
-):
+) -> FigureLike:
     """Make a three-dimensional scatter plot.
 
     To specify the positions of the scatter points, you can use:
 
     - a single coordinate inside the supplied data array that has dtype ``vector3``
       (use the ``pos`` parameter to specify the name of the coordinate).
     - three coordinates from the data array, whose names are specified using the
@@ -98,15 +98,15 @@
     from ..graphics import scatter3dfigure
     from ..widgets import ClippingPlanes, ToggleTool
 
     if 'ax' in kwargs:
         raise ValueError(
             'Keyword "ax" detected. Embedding 3D scatter plots inside Matplotlib axes '
             'is not supported. See '
-            'https://scipp.github.io/plopp/customization/subplots.html#FAQ:-subplots-with-3D-scatter-plots'  # noqa: E501
+            'https://scipp.github.io/plopp/customization/subplots.html#FAQ:-subplots-with-3D-scatter-plots'
         )
 
     nodes = input_to_nodes(
         obj, processor=partial(_preprocess_scatter, x=x, y=y, z=z, pos=pos)
     )
 
     fig = scatter3dfigure(
```

### Comparing `plopp-24.4.0/src/plopp/plotting/slicer.py` & `plopp-24.5.0/src/plopp/plotting/slicer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import warnings
 from functools import partial, reduce
 from itertools import groupby
-from typing import List, Literal, Optional, Union
+from typing import Literal
 
 from scipp.typing import VariableLike
 
 from ..core import widget_node
-from ..core.typing import PlottableMulti
+from ..core.typing import FigureLike, PlottableMulti
 from ..graphics import imagefigure, linefigure
 from .common import (
     input_to_nodes,
     preprocess,
     raise_multiple_inputs_for_2d_plot_error,
     require_interactive_backend,
 )
@@ -57,19 +57,19 @@
         The additional arguments are forwarded to the underlying 1D or 2D figures.
     """
 
     def __init__(
         self,
         obj: PlottableMulti,
         *,
-        keep: List[str] = None,
+        keep: list[str] | None = None,
         autoscale: Literal['auto', 'grow', 'fixed'] = 'auto',
-        coords: Optional[List[str]] = None,
-        vmin: Union[VariableLike, int, float] = None,
-        vmax: Union[VariableLike, int, float] = None,
+        coords: list[str] | None = None,
+        vmin: VariableLike | float = None,
+        vmax: VariableLike | float = None,
         **kwargs,
     ):
         nodes = input_to_nodes(
             obj, processor=partial(preprocess, ignore_size=True, coords=coords)
         )
 
         dims = nodes[0]().dims
@@ -141,21 +141,21 @@
         )
         self.figure.bottom_bar.add(self.slider)
 
 
 def slicer(
     obj: PlottableMulti,
     *,
-    keep: List[str] = None,
+    keep: list[str] | None = None,
     autoscale: Literal['auto', 'grow', 'fixed'] = 'auto',
-    coords: Optional[List[str]] = None,
-    vmin: Union[VariableLike, int, float] = None,
-    vmax: Union[VariableLike, int, float] = None,
+    coords: list[str] | None = None,
+    vmin: VariableLike | float = None,
+    vmax: VariableLike | float = None,
     **kwargs,
-):
+) -> FigureLike:
     """
     Plot a multi-dimensional object by slicing one or more of the dimensions.
     This will produce one slider per sliced dimension, below the figure.
 
     Parameters
     ----------
     obj:
```

### Comparing `plopp-24.4.0/src/plopp/plotting/superplot.py` & `plopp-24.5.0/src/plopp/plotting/superplot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Optional
 
-from ..core.typing import Plottable
+from ..core.typing import FigureLike, Plottable
 from .common import require_interactive_backend
 from .slicer import Slicer
 
 
 def superplot(
     obj: Plottable,
-    keep: Optional[str] = None,
+    keep: str | None = None,
     **kwargs,
-):
+) -> FigureLike:
     """
     Plot a multi-dimensional object as a one-dimensional line, slicing all but one
     dimension. This will produce one slider per sliced dimension, below the figure.
     In addition, a tool for saving the currently displayed line is added on the right
     hand side of the figure.
 
     Parameters
```

### Comparing `plopp-24.4.0/src/plopp/plotting/xyplot.py` & `plopp-24.5.0/src/plopp/plotting/xyplot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Union
 
 import scipp as sc
 from numpy import ndarray
 
 from ..core import Node
+from ..core.typing import FigureLike
 from ..graphics import linefigure
 from .common import to_variable
 
 
 def _make_data_array(x: sc.Variable, y: sc.Variable) -> sc.DataArray:
     """
     Make a data array from the supplied variables, using ``x`` as the coordinate and
@@ -23,18 +23,18 @@
     y:
         The variable to use as the data.
     """
     return sc.DataArray(data=y, coords={x.dim: x})
 
 
 def xyplot(
-    x: Union[sc.Variable, ndarray, list, Node],
-    y: Union[sc.Variable, ndarray, list, Node],
+    x: sc.Variable | ndarray | list | Node,
+    y: sc.Variable | ndarray | list | Node,
     **kwargs,
-):
+) -> FigureLike:
     """
     Make a one-dimensional plot of one variable ``y`` as a function of another ``x``.
 
     .. versionadded:: 23.10.0
 
     Parameters
     ----------
```

### Comparing `plopp-24.4.0/src/plopp/utils.py` & `plopp-24.5.0/src/plopp/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
 
 import functools
 import warnings
-from typing import Callable
+from collections.abc import Callable
 
 from .core.typing import VisibleDeprecationWarning
 
 
 def deprecated(message: str = '') -> Callable:
     def decorator(function: Callable) -> Callable:
         @functools.wraps(function)
```

### Comparing `plopp-24.4.0/src/plopp/widgets/box.py` & `plopp-24.5.0/src/plopp/widgets/box.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def __len__(self):
         return len(self.children)
 
     def add(self, obj: Widget):
         """
         Append a widget to the list of children.
         """
-        self.children = list(self.children) + [obj]
+        self.children = [*self.children, obj]
 
     def remove(self, obj: Widget):
         """
         Remove a widget from the list of children.
         """
         children = list(self.children)
         children.remove(obj)
@@ -62,11 +62,11 @@
     ----------
 
     widgets:
         List of widgets to place in the box.
     """
 
     def __init__(self, widgets):
-        children = []
-        for view in widgets:
-            children.append(HBar(view) if isinstance(view, (list, tuple)) else view)
+        children = [
+            HBar(view) if isinstance(view, list | tuple) else view for view in widgets
+        ]
         super().__init__(children)
```

### Comparing `plopp-24.4.0/src/plopp/widgets/checkboxes.py` & `plopp-24.5.0/src/plopp/widgets/checkboxes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
+from collections.abc import Callable
 from html import escape
-from typing import Callable, Dict, List
 
 import ipywidgets as ipw
 
 
 class Checkboxes(ipw.HBox):
     """
     Widget providing a list of checkboxes, along with a button to toggle them all.
@@ -17,15 +17,15 @@
         List of strings to create the names for the different checkboxes.
     description:
         Global description for all the checkboxes.
     value:
         Default value to set all the checkboxes to.
     """
 
-    def __init__(self, entries: List[str], description: str = "", value: bool = True):
+    def __init__(self, entries: list[str], description: str = "", value: bool = True):
         self.checkboxes = {}
         self._lock = False
         self.description = ipw.Label(value=description)
 
         for key in entries:
             self.checkboxes[key] = ipw.Checkbox(
                 value=value,
@@ -57,12 +57,12 @@
         super().__init__(to_hbox)
 
     def _plopp_observe_(self, callback: Callable, **kwargs):
         for chbx in self.checkboxes.values():
             chbx.observe(callback, **kwargs)
 
     @property
-    def value(self) -> Dict[str, bool]:
+    def value(self) -> dict[str, bool]:
         """
         Returns a dict containing one entry per checkbox, giving the checkbox's value.
         """
         return {key: chbx.value for key, chbx in self.checkboxes.items()}
```

### Comparing `plopp-24.4.0/src/plopp/widgets/clip3d.py` & `plopp-24.5.0/src/plopp/widgets/clip3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
 
 import uuid
+from collections.abc import Callable
 from functools import partial, reduce
-from typing import Any, Callable, Dict, List, Literal, Tuple
+from typing import Any, Literal
 
 import ipywidgets as ipw
 import numpy as np
 import pythreejs as p3
 import scipp as sc
 
 from ..core import Node
 from ..graphics import BaseFig
 from .debounce import debounce
 from .style import BUTTON_LAYOUT
 
 
-def _xor(x: List[sc.Variable]) -> sc.Variable:
+def _xor(x: list[sc.Variable]) -> sc.Variable:
     dim = uuid.uuid4().hex
     return sc.concat(x, dim).sum(dim) == sc.scalar(1, unit=None)
 
 
 OPERATIONS = {
     'or': partial(reduce, lambda x, y: sc.logical_or(x, y)),
     'and': partial(reduce, lambda x, y: sc.logical_and(x, y)),
     'xor': _xor,
 }
 
 
-def select(da: sc.DataArray, s: Tuple[str, sc.Variable]) -> sc.DataArray:
+def select(da: sc.DataArray, s: tuple[str, sc.Variable]) -> sc.DataArray:
     return da[s]
 
 
 class Clip3dTool(ipw.HBox):
     """
     A tool that provides a slider to extract a slab of points in a three-dimensional
     scatter plot, and add it to the scene as an opaque cut. The slider controls the
@@ -54,15 +55,15 @@
         Color of the cut's outline.
     linewidth:
         Width of the line delineating the outline.
     """
 
     def __init__(
         self,
-        limits: Tuple[sc.Variable, sc.Variable, sc.Variable],
+        limits: tuple[sc.Variable, sc.Variable, sc.Variable],
         direction: Literal['x', 'y', 'z'],
         update: Callable,
         color: str = 'red',
         linewidth: float = 1.5,
         border_visible: bool = True,
     ):
         self._limits = limits
@@ -117,15 +118,15 @@
 
         self.cut_visible = ipw.Button(
             icon='eye-slash',
             tooltip='Hide cut',
             layout={'width': '16px', 'padding': '0px'},
         )
 
-        for outline, val in zip(self.outlines, self.slider.value):
+        for outline, val in zip(self.outlines, self.slider.value, strict=True):
             pos = list(center)
             pos[axis] = val
             outline.position = pos
             outline.visible = self._border_visible
 
         self.unit_label = ipw.Label(f'[{self._unit}]')
         self.cut_visible.on_click(self.toggle)
@@ -152,26 +153,26 @@
         for outline in self.outlines:
             outline.visible = value
         # The call to this function comes from the parent widget, so we need to
         # remember the state of the button, so that when we toggle the visbiility of
         # the cut, the border visibility is in sync with the parent button.
         self._border_visible = value
 
-    def move(self, value: Dict[str, Any]):
+    def move(self, value: dict[str, Any]):
         """
         Move the outline of the cut according to new position given by the slider.
         """
         # Early return if relative difference between new and old value is small.
         # This also prevents flickering of an existing cut when a new cut is added.
         if (
-            np.abs((np.array(value['new']) - np.array(value['old']))).max()
+            np.abs(np.array(value['new']) - np.array(value['old'])).max()
             < 0.01 * self.slider.step
         ):
             return
-        for outline, val in zip(self.outlines, value['new']):
+        for outline, val in zip(self.outlines, value['new'], strict=True):
             pos = list(outline.position)
             axis = 'xyz'.index(self._direction)
             pos[axis] = val
             outline.position = pos
         self._throttled_update()
 
     @property
@@ -302,15 +303,15 @@
             direction=direction,
             limits=self._limits,
             update=self.update_state,
             border_visible=self.cut_borders_visibility.value,
         )
         self._view.canvas.add(cut.outlines)
         self.cuts.append(cut)
-        self.tabs.children = list(self.tabs.children) + [cut]
+        self.tabs.children = [*self.tabs.children, cut]
         self.tabs.selected_index = len(self.cuts) - 1
         self.update_controls()
         self.update_state()
 
     def _remove_cut(self, _):
         cut = self.cuts.pop(self.tabs.selected_index)
         self._view.canvas.remove(cut.outlines)
@@ -329,34 +330,34 @@
         self.cut_borders_visibility.disabled = not at_least_one_cut
         self.cut_operation.disabled = not at_least_one_cut
         self.tabs.titles = [cut._direction.upper() for cut in self.cuts]
         self.opacity.disabled = not at_least_one_cut
         opacity = self.opacity.value if at_least_one_cut else 1.0
         self._set_opacity({'new': opacity})
 
-    def _set_opacity(self, change: Dict[str, Any]):
+    def _set_opacity(self, change: dict[str, Any]):
         """
         Set the opacity of the original point clouds in the figure, not the cuts.
         """
         self._view.set_opacity(change['new'])
 
     def toggle_visibility(self):
         """
         Toggle the visibility of the control buttons for making the cuts.
         """
         self.layout.display = None if self.layout.display == 'none' else 'none'
 
-    def toggle_border_visibility(self, change: Dict[str, Any]):
+    def toggle_border_visibility(self, change: dict[str, Any]):
         """
         Toggle the visibility of the borders of the cuts.
         """
         for cut in self.cuts:
             cut.toggle_border(change['new'])
 
-    def change_operation(self, change: Dict[str, Any]):
+    def change_operation(self, change: dict[str, Any]):
         """
         Change the operation to combine multiple cuts.
         """
         self._operation = change['new'].lower()
         self.update_state()
 
     def update_state(self):
```

### Comparing `plopp-24.4.0/src/plopp/widgets/cut3d.py` & `plopp-24.5.0/src/plopp/widgets/cut3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 
 from functools import partial
-from typing import Any, Dict, Literal, Tuple
+from typing import Any, Literal
 
 import ipywidgets as ipw
 import numpy as np
 import scipp as sc
 
 from ..core import View, node
 from ..utils import deprecated
@@ -46,15 +46,15 @@
     **kwargs:
         The kwargs are forwarded to the ToggleButton from ``ipywidgets``.
     """
 
     def __init__(
         self,
         view: View,
-        limits: Tuple[sc.Variable, sc.Variable, sc.Variable],
+        limits: tuple[sc.Variable, sc.Variable, sc.Variable],
         direction: Literal['x', 'y', 'z'],
         value: bool = False,
         color: str = 'red',
         linewidth: float = 1.5,
         **kwargs,
     ):
         import pythreejs as p3
@@ -131,27 +131,27 @@
                 ipw.VBox(
                     [self.slider, ipw.HBox([self.readout, self.unit_label])],
                     layout={'align_items': 'center'},
                 ),
             ]
         )
 
-    def toggle(self, change: Dict[str, Any]):
+    def toggle(self, change: dict[str, Any]):
         """
         Toggle the tool on and off.
         """
         self.outline.visible = change['new']
         for widget in (self.slider, self.plus_minus, self.readout):
             widget.disabled = not change['new']
         if change['new']:
             self._add_cut()
         else:
             self._remove_cut()
 
-    def move(self, value: Dict[str, Any]):
+    def move(self, value: dict[str, Any]):
         """
         Move the outline of the cut according to new position given by the slider.
         """
         pos = list(self.outline.position)
         axis = 'xyz'.index(self._direction)
         pos[axis] = value['new']
         self.outline.position = pos
@@ -303,15 +303,15 @@
         a low value. If all cuts are inactive, set the opacity back to 1.
         """
         active_cut = any([self.cut_x.value, self.cut_y.value, self.cut_z.value])
         self.opacity.disabled = not active_cut
         opacity = self.opacity.value if active_cut else 1.0
         self._set_opacity({'new': opacity})
 
-    def _set_opacity(self, change: Dict[str, Any]):
+    def _set_opacity(self, change: dict[str, Any]):
         """
         Set the opacity of the original point clouds in the figure, not the cuts.
         """
         self._fig.set_opacity(change['new'])
 
     def toggle_visibility(self):
         """
```

### Comparing `plopp-24.4.0/src/plopp/widgets/debounce.py` & `plopp-24.5.0/src/plopp/widgets/debounce.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
 
 import asyncio
-from typing import Callable
+from collections.abc import Callable
 
 
 class Timer:
     """
     From:
     https://ipywidgets.readthedocs.io/en/8.0.2/examples/Widget%20Events.html#Debouncing
     """
```

### Comparing `plopp-24.4.0/src/plopp/widgets/drawing.py` & `plopp-24.5.0/src/plopp/widgets/drawing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
+from collections.abc import Callable
 from functools import partial
-from typing import Any, Callable, Union
+from typing import Any
 
 import scipp as sc
 
-from ..backends.protocols import FigureLike
 from ..core import Node, node
+from ..core.typing import FigureLike
 from .tools import ToggleTool
 
 
 def is_figure(x):
     from ..backends.matplotlib.interactive import InteractiveFig
 
     return isinstance(x, InteractiveFig)
@@ -47,15 +48,15 @@
 
     def __init__(
         self,
         figure: FigureLike,
         input_node: Node,
         tool: Any,
         func: Callable,
-        destination: Union[FigureLike, Node],
+        destination: FigureLike | Node,
         get_artist_info: Callable,
         value: bool = False,
         **kwargs,
     ):
         super().__init__(callback=self.start_stop, value=value, **kwargs)
 
         self._figure = figure
@@ -98,14 +99,15 @@
     def remove_node(self, artist):
         nodeid = artist.nodeid
         draw_node = self._draw_nodes[nodeid]
         output_node = self._output_nodes[nodeid]
         if self._destination_is_fig:
             self._destination.artists[output_node.id].remove()
             del self._destination.artists[output_node.id]
+            self._destination.canvas.draw()
         output_node.remove()
         draw_node.remove()
 
     def start_stop(self):
         """
         Toggle start or stop of the tool.
         """
```

### Comparing `plopp-24.4.0/src/plopp/widgets/linesave.py` & `plopp-24.5.0/src/plopp/widgets/linesave.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from functools import partial
-from typing import Any, Dict
+from typing import Any
 
 import ipywidgets as ipw
 from matplotlib.colors import to_hex
 
 from ..core import Node, View
 from ..core.utils import coord_element_to_string
 from .box import VBar
@@ -36,15 +36,15 @@
         self.button.on_click(self.save_line)
         self.container = VBar()
         super().__init__([self.button, self.container], layout={'width': '350px'})
 
     def _update_container(self):
         self.container.children = [line['tool'] for line in self._lines.values()]
 
-    def save_line(self, change: Dict[str, Any] = None):
+    def save_line(self, change: dict[str, Any] | None = None):
         from ..widgets import ColorTool
 
         data = self._data_node.request_data()
         node = Node(data)
         node.name = f'Save node {len(self._lines)}'
         line_id = node._id
         node.add_view(self._fig._view)
@@ -58,15 +58,15 @@
         self._lines[line_id] = {'line': line, 'tool': tool, 'node': node}
         self._update_container()
         tool.color.observe(
             partial(self.change_line_color, line_id=line_id), names='value'
         )
         tool.button.on_click(partial(self.remove_line, line_id=line_id))
 
-    def change_line_color(self, change: Dict[str, Any], line_id: str):
+    def change_line_color(self, change: dict[str, Any], line_id: str):
         self._lines[line_id]['line'].color = change['new']
 
-    def remove_line(self, change: Dict[str, Any], line_id: str):
+    def remove_line(self, change: dict[str, Any], line_id: str):
         self._lines[line_id]['line'].remove()
         self._lines[line_id]['node'].remove()
         del self._lines[line_id]
         self._update_container()
```

### Comparing `plopp-24.4.0/src/plopp/widgets/slice.py` & `plopp-24.5.0/src/plopp/widgets/slice.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,50 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Any, Callable, Dict, List
+from collections.abc import Callable
+from typing import Any
 
 import ipywidgets as ipw
 import scipp as sc
 
 from ..core import node
 from ..core.utils import coord_element_to_string
 from .box import VBar
 
 
-class SliceWidget(VBar):
-    """
-    Widgets containing a slider for each of the requested dimensions.
-    The widget uses the input data array to determine the range each slider should have.
-    Each slider also comes with a checkbox to toggle on and off the slider's continuous
-    update.
-
-    Parameters
-    ----------
-    da:
-        The input data array.
-    dims:
-        The dimensions to make sliders for.
-    """
-
-    def __init__(self, da: sc.DataArray, dims: List[str]):
+class _BaseSliceWidget(VBar):
+    def __init__(self, da: sc.DataArray, dims: list[str], range: bool):
         if isinstance(dims, str):
             dims = [dims]
         self._slider_dims = dims
         self.controls = {}
         self.view = None
         children = []
 
         for dim in self._slider_dims:
             coord = (
                 da.coords[dim]
                 if dim in da.coords
                 else sc.arange(dim, da.sizes[dim], unit=None)
             )
-            slider = ipw.IntSlider(
-                step=1,
-                description=dim,
-                min=0,
-                max=da.sizes[dim] - 1,
-                continuous_update=True,
-                readout=False,
-                layout={"width": "200px"},
-                style={'description_width': 'initial'},
-            )
+            widget_args = {
+                'step': 1,
+                'description': dim,
+                'min': 0,
+                'max': da.sizes[dim] - 1,
+                'continuous_update': True,
+                'readout': False,
+                'layout': {"width": "200px"},
+                'style': {'description_width': 'initial'},
+            }
+            if range:
+                slider = ipw.IntRangeSlider(**widget_args)
+            else:
+                slider = ipw.IntSlider(**widget_args)
             continuous_update = ipw.Checkbox(
                 value=True,
                 tooltip="Continuous update",
                 indent=False,
                 layout={"width": "20px"},
             )
             label = ipw.Label(value=coord_element_to_string(coord[dim, 0]))
@@ -66,15 +57,15 @@
                 'coord': coord,
             }
             slider.observe(self._update_label, names='value')
             children.append(ipw.HBox([continuous_update, slider, label]))
 
         super().__init__(children)
 
-    def _update_label(self, change: Dict[str, Any]):
+    def _update_label(self, change: dict[str, Any]):
         """
         Update the readout label with the coordinate value, instead of the integer
         readout index.
         """
         dim = change['owner'].description
         coord = self.controls[dim]['coord'][dim, change['new']]
         self.controls[dim]['label'].value = coord_element_to_string(coord)
@@ -84,31 +75,73 @@
         Special method which is used instead of the ``observe`` method of ``ipywidgets``
         because overriding the ``observe`` method of the ``VBox`` causes issues.
         """
         for dim in self.controls:
             self.controls[dim]['slider'].observe(callback, **kwargs)
 
     @property
-    def value(self) -> Dict[str, int]:
+    def value(self) -> dict[str, int | tuple[int]]:
         """
         The widget value, as a dict containing the dims as keys and the slider indices
         as values.
         """
         return {dim: self.controls[dim]['slider'].value for dim in self._slider_dims}
 
 
+class SliceWidget(_BaseSliceWidget):
+    """
+    Widgets containing a slider for each of the requested dimensions.
+    The widget uses the input data array to determine the range each slider should have.
+    Each slider also comes with a checkbox to toggle on and off the slider's continuous
+    update.
+
+    Parameters
+    ----------
+    da:
+        The input data array.
+    dims:
+        The dimensions to make sliders for.
+    """
+
+    def __init__(self, da: sc.DataArray, dims: list[str]):
+        super().__init__(da, dims, range=False)
+
+
+class RangeSliceWidget(_BaseSliceWidget):
+    """
+    Widgets containing a slider for each of the requested dimensions.
+    The widget uses the input data array to determine the range each slider should have.
+    Each slider also comes with a checkbox to toggle on and off the slider's continuous
+    update.
+
+    .. versionadded:: 24.04.0
+
+    Parameters
+    ----------
+    da:
+        The input data array.
+    dims:
+        The dimensions to make sliders for.
+    """
+
+    def __init__(self, da: sc.DataArray, dims: list[str]):
+        super().__init__(da, dims, range=True)
+
+
 @node
-def slice_dims(data_array: sc.DataArray, slices: Dict[str, slice]) -> sc.DataArray:
+def slice_dims(data_array: sc.DataArray, slices: dict[str, slice]) -> sc.DataArray:
     """
     Slice the data according to input slices.
 
     Parameters
     ----------
     data_array:
         The input data array to be sliced.
     slices:
         Dict of slices to apply for each dimension.
     """
     out = data_array
     for dim, sl in slices.items():
+        if isinstance(sl, tuple):
+            sl = slice(*sl)
         out = out[dim, sl]
     return out
```

### Comparing `plopp-24.4.0/src/plopp/widgets/toolbar.py` & `plopp-24.5.0/src/plopp/widgets/toolbar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Any, Dict, Optional
+from typing import Any
 
 from ipywidgets import VBox
 
 from ..graphics import ColorMapper
 from . import tools
 
 
@@ -15,15 +15,15 @@
 
     Parameters
     ----------
     tools:
         Dictionary of tools to populate the toolbar.
     """
 
-    def __init__(self, tools: Dict[str, Any] = None):
+    def __init__(self, tools: dict[str, Any] | None = None):
         self.tools = {}
         if tools is not None:
             for key, tool in tools.items():
                 if isinstance(tool.callback, dict):
                     for name, cb in tool.callback.items():
                         setattr(self, name, cb)
                 else:
@@ -45,15 +45,15 @@
         self._update_children()
 
     def _update_children(self):
         self.children = list(self.tools.values())
 
 
 def make_toolbar_canvas2d(
-    canvas: Any, colormapper: Optional[ColorMapper] = None
+    canvas: Any, colormapper: ColorMapper | None = None
 ) -> Toolbar:
     """
     Create a toolbar for a 2D canvas.
     If the colormapper is defined, add a button to toggle the norm of the colormapper.
 
     Parameters
     ----------
@@ -74,15 +74,15 @@
             colormapper.toggle_norm, value=colormapper.norm == 'log'
         )
     tool_list['save'] = tools.SaveTool(canvas.download_figure)
     return Toolbar(tools=tool_list)
 
 
 def make_toolbar_canvas3d(
-    canvas: Any, colormapper: Optional[ColorMapper] = None
+    canvas: Any, colormapper: ColorMapper | None = None
 ) -> Toolbar:
     """
     Create a toolbar for a 3D canvas.
     If the colormapper is defined, add a button to toggle the norm of the colormapper.
 
     Parameters
     ----------
```

### Comparing `plopp-24.4.0/src/plopp/widgets/tools.py` & `plopp-24.5.0/src/plopp/widgets/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
+from collections.abc import Callable
 from functools import partial
-from typing import Callable, List, Optional, Union
 
 import ipywidgets as ipw
 
 from .style import BUTTON_LAYOUT
 
 
 class ButtonTool(ipw.Button):
@@ -17,15 +17,15 @@
     ----------
     callback:
         The function that will be called when the button is clicked.
     **kwargs:
         All other kwargs are forwarded to ipywidgets.Button.
     """
 
-    def __init__(self, callback: Callable = None, **kwargs):
+    def __init__(self, callback: Callable | None = None, **kwargs):
         super().__init__(**{**BUTTON_LAYOUT, **kwargs})
         self.callback = callback
         self.on_click(self)
 
     def __call__(self, *ignored):
         self.callback()
 
@@ -103,19 +103,19 @@
     **kwargs:
         All other kwargs are forwarded to ipywidgets.ToggleButton.
     """
 
     def __init__(
         self,
         callback: Callable,
-        options: List[str],
-        icons: Optional[List[str]] = None,
-        tooltips: List[str] = None,
-        descriptions: List[str] = None,
-        value: Optional[str] = None,
+        options: list[str],
+        icons: list[str] | None = None,
+        tooltips: list[str] | None = None,
+        descriptions: list[str] | None = None,
+        value: str | None = None,
         **kwargs,
     ):
         self.callback = callback
         self._options = options
         self._buttons = {}
         for i, key in enumerate(self._options):
             tb = ipw.ToggleButton(
@@ -139,15 +139,15 @@
         for name in set(self._buttons.keys()) - {key}:
             if self._buttons[name].value:
                 self._buttons[name].value = False
         self._lock = False
         self.callback()
 
     @property
-    def value(self) -> Union[str, None]:
+    def value(self) -> str | None:
         for b in self._buttons.values():
             if b.value:
                 return b._option
 
 
 HomeTool = partial(ButtonTool, icon='home', tooltip='Autoscale view')
 """Return home tool."""
@@ -192,15 +192,15 @@
     ----------
     canvas:
         The canvas to act upon.
     value:
         Set the initially selected button. No button selected if ``None``.
     """
 
-    def __init__(self, callback: Callable, value: bool = None, **kwargs):
+    def __init__(self, callback: Callable, value: bool | None = None, **kwargs):
         self._callback = callback
         super().__init__(
             callback=self._panzoom,
             options=['pan', 'zoom'],
             icons=['arrows', 'search-plus'],
             tooltips=['Pan', 'Zoom'],
             value=value,
```

### Comparing `plopp-24.4.0/src/plopp.egg-info/PKG-INFO` & `plopp-24.5.0/src/plopp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plopp
-Version: 24.4.0
+Version: 24.5.0
 Summary: Visualization library for Scipp
 Author: Scipp contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
         
@@ -38,31 +38,32 @@
 Project-URL: Source, https://github.com/scipp/plopp
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.5
 Provides-Extra: scipp
 Requires-Dist: scipp; extra == "scipp"
 Provides-Extra: all
 Requires-Dist: scipp; extra == "all"
 Requires-Dist: ipympl; extra == "all"
 Requires-Dist: pythreejs; extra == "all"
 Requires-Dist: mpltoolbox; extra == "all"
+Requires-Dist: ipywidgets; extra == "all"
+Requires-Dist: graphviz; extra == "all"
 
 <img src="docs/_static/logo.svg" width="50%" />
 
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
 [![PyPI badge](http://img.shields.io/pypi/v/plopp.svg)](https://pypi.python.org/pypi/plopp)
 [![Anaconda-Server Badge](https://anaconda.org/scipp/plopp/badges/version.svg)](https://anaconda.org/scipp/plopp)
 [![Documentation](https://img.shields.io/badge/docs-online-success)](https://scipp.github.io/plopp/)
```

### Comparing `plopp-24.4.0/src/plopp.egg-info/SOURCES.txt` & `plopp-24.5.0/src/plopp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 .pre-commit-config.yaml
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 tox.ini
 .github/dependabot.yml
 .github/workflows/ci.yml
-.github/workflows/copier.yml
 .github/workflows/docs.yml
 .github/workflows/nightly_at_main.yml
 .github/workflows/nightly_at_release.yml
 .github/workflows/python-version-ci
 .github/workflows/release.yml
 .github/workflows/test.yml
 .github/workflows/unpinned.yml
@@ -120,15 +118,14 @@
 src/plopp.egg-info/SOURCES.txt
 src/plopp.egg-info/dependency_links.txt
 src/plopp.egg-info/requires.txt
 src/plopp.egg-info/top_level.txt
 src/plopp/backends/__init__.py
 src/plopp/backends/common.py
 src/plopp/backends/manager.py
-src/plopp/backends/protocols.py
 src/plopp/backends/matplotlib/__init__.py
 src/plopp/backends/matplotlib/canvas.py
 src/plopp/backends/matplotlib/figure.py
 src/plopp/backends/matplotlib/image.py
 src/plopp/backends/matplotlib/interactive.py
 src/plopp/backends/matplotlib/line.py
 src/plopp/backends/matplotlib/scatter.py
@@ -156,15 +153,14 @@
 src/plopp/data/examples.py
 src/plopp/data/factory.py
 src/plopp/data/testing.py
 src/plopp/graphics/__init__.py
 src/plopp/graphics/basefig.py
 src/plopp/graphics/camera.py
 src/plopp/graphics/colormapper.py
-src/plopp/graphics/common.py
 src/plopp/graphics/figure.py
 src/plopp/graphics/graphicalview.py
 src/plopp/graphics/imageview.py
 src/plopp/graphics/lineview.py
 src/plopp/graphics/scatter3dview.py
 src/plopp/graphics/scatterview.py
 src/plopp/graphics/tiled.py
```

### Comparing `plopp-24.4.0/tests/backends/matplotlib/mpl_canvas_test.py` & `plopp-24.5.0/tests/backends/matplotlib/mpl_canvas_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,9 +48,9 @@
         fname = os.path.join(path, f'plopp_fig.{ext}')
         canvas.save(filename=fname)
         assert os.path.isfile(fname)
 
 
 def test_save_to_disk_with_bad_extension_raises():
     canvas = Canvas()
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='txt'):
         canvas.save(filename='plopp_fig.txt')
```

### Comparing `plopp-24.4.0/tests/backends/matplotlib/mpl_figure_test.py` & `plopp-24.5.0/tests/backends/matplotlib/mpl_figure_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 import numpy as np
+import pytest
 import scipp as sc
 
 from plopp.backends.matplotlib import MatplotlibBackend
 from plopp.backends.matplotlib.interactive import InteractiveFig
 from plopp.backends.matplotlib.static import StaticFig
 from plopp.core import Node
 from plopp.graphics.imageview import ImageView
@@ -13,27 +14,29 @@
 
 def test_create_static_fig1d():
     b = MatplotlibBackend()
     fig = b.figure1d(View=LineView)
     assert isinstance(fig, StaticFig)
 
 
-def test_create_interactive_fig1d(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_create_interactive_fig1d():
     b = MatplotlibBackend()
     fig = b.figure1d(View=LineView)
     assert isinstance(fig, InteractiveFig)
 
 
 def test_create_static_fig2d():
     b = MatplotlibBackend()
     fig = b.figure2d(View=ImageView)
     assert isinstance(fig, StaticFig)
 
 
-def test_create_interactive_fig2d(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_create_interactive_fig2d():
     b = MatplotlibBackend()
     fig = b.figure2d(View=ImageView)
     assert isinstance(fig, InteractiveFig)
 
 
 def test_datetime_compatibility_between_1d_and_2d_figures():
     b = MatplotlibBackend()
```

### Comparing `plopp-24.4.0/tests/backends/matplotlib/mpl_image_test.py` & `plopp-24.5.0/tests/backends/matplotlib/mpl_image_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/backends/matplotlib/mpl_imageview_test.py` & `plopp-24.5.0/tests/backends/matplotlib/mpl_imageview_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,18 +71,18 @@
     fig = ImageView(Node(da))
     assert [t.get_text() for t in fig.canvas.ax.get_xticklabels()] == strings
 
 
 def test_kwargs_are_forwarded_to_artist():
     da = data_array(ndim=2)
     fig = ImageView(Node(da), rasterized=True)
-    artist = list(fig.artists.values())[0]
+    [artist] = fig.artists.values()
     assert artist._mesh.get_rasterized()
     fig = ImageView(Node(da), rasterized=False)
-    artist = list(fig.artists.values())[0]
+    [artist] = fig.artists.values()
     assert not artist._mesh.get_rasterized()
 
 
 def test_figsize():
     da = data_array(ndim=2)
     size = (8.1, 8.3)
     fig = ImageView(Node(da), figsize=size)
```

### Comparing `plopp-24.4.0/tests/backends/matplotlib/mpl_interactive_test.py` & `plopp-24.5.0/tests/backends/matplotlib/mpl_interactive_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
+import pytest
+
 from plopp import Node
 from plopp.backends.matplotlib.interactive import InteractiveFig
 from plopp.data.testing import data_array
 from plopp.graphics.imageview import ImageView
 from plopp.graphics.lineview import LineView
 
 
-def test_logx_1d_toolbar_button(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_logx_1d_toolbar_button():
     da = data_array(ndim=1)
     fig = InteractiveFig(LineView, Node(da), scale={'xx': 'log'})
     assert fig.toolbar['logx'].value
 
 
-def test_logy_1d_toolbar_button(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_logy_1d_toolbar_button():
     da = data_array(ndim=1)
     fig = InteractiveFig(LineView, Node(da), norm='log')
     assert fig.toolbar['logy'].value
 
 
-def test_logxy_2d_toolbar_buttons(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_logxy_2d_toolbar_buttons():
     da = data_array(ndim=2)
     fig = InteractiveFig(ImageView, Node(da), scale={'xx': 'log', 'yy': 'log'})
     assert fig.toolbar['logx'].value
     assert fig.toolbar['logy'].value
 
 
-def test_log_norm_2d_toolbar_button(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_log_norm_2d_toolbar_button():
     da = data_array(ndim=2)
     fig = InteractiveFig(ImageView, Node(da), norm='log')
     assert fig.toolbar['lognorm'].value
```

### Comparing `plopp-24.4.0/tests/backends/matplotlib/mpl_line_test.py` & `plopp-24.5.0/tests/backends/matplotlib/mpl_line_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/backends/matplotlib/mpl_lineview_test.py` & `plopp-24.5.0/tests/backends/matplotlib/mpl_lineview_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/backends/matplotlib/mpl_scatter_test.py` & `plopp-24.5.0/tests/backends/matplotlib/mpl_scatter_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/backends/matplotlib/mpl_tiled_test.py` & `plopp-24.5.0/tests/backends/matplotlib/mpl_tiled_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/backends/matplotlib/mpl_utils_test.py` & `plopp-24.5.0/tests/backends/matplotlib/mpl_utils_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
+import pytest
+
 from plopp import Node
 from plopp.backends.matplotlib.interactive import InteractiveFig
 from plopp.backends.matplotlib.static import StaticFig
 from plopp.backends.matplotlib.utils import copy_figure
 from plopp.data.testing import data_array
 from plopp.graphics.lineview import LineView
 
@@ -38,13 +40,15 @@
     do_test_copy(StaticFig)
 
 
 def test_copy_static_keeps_kwargs():
     do_test_copy_keeps_kwargs(StaticFig)
 
 
-def test_copy_interactive(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_copy_interactive():
     do_test_copy(InteractiveFig)
 
 
-def test_copy_interactive_keeps_kwargs(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_copy_interactive_keeps_kwargs():
     do_test_copy_keeps_kwargs(InteractiveFig)
```

### Comparing `plopp-24.4.0/tests/backends/plotly/plotly_canvas_test.py` & `plopp-24.5.0/tests/backends/plotly/plotly_canvas_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,9 +40,9 @@
         fname = os.path.join(path, f'plopp_fig.{ext}')
         canvas.save(filename=fname)
         assert os.path.isfile(fname)
 
 
 def test_save_to_disk_with_bad_extension_raises():
     canvas = Canvas()
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='txt'):
         canvas.save(filename='plopp_fig.txt')
```

### Comparing `plopp-24.4.0/tests/backends/plotly/plotly_figure_test.py` & `plopp-24.5.0/tests/backends/plotly/plotly_figure_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/backends/plotly/plotly_line_test.py` & `plopp-24.5.0/tests/backends/plotly/plotly_line_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/backends/pythreejs/pythreejs_canvas_test.py` & `plopp-24.5.0/tests/backends/pythreejs/pythreejs_canvas_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/backends/pythreejs/pythreejs_figure_test.py` & `plopp-24.5.0/tests/backends/pythreejs/pythreejs_figure_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py` & `plopp-24.5.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/conftest.py` & `plopp-24.5.0/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 
 import matplotlib
 import matplotlib.pyplot as plt
 import pytest
 
 
 @pytest.fixture(autouse=True)
-def reset_mpl_defaults():
+def _reset_mpl_defaults():
     matplotlib.rcdefaults()
     matplotlib.use('Agg')
 
 
 @pytest.fixture(autouse=True)
-def close_figures():
+def _close_figures():
     """
     Force closing all figures after each test case.
     Otherwise, the figures consume a lot of memory and matplotlib complains.
     """
     yield
     for fig in map(plt.figure, plt.get_fignums()):
         plt.close(fig)
 
 
-@pytest.fixture
-def use_ipympl():
+@pytest.fixture()
+def _use_ipympl():
     matplotlib.use('module://ipympl.backend_nbagg')
 
 
 def pytest_sessionfinish(session, exitstatus):
     """
     When running no tests (e.g. in the noplotly tox env), pytest returns the exit code
     5, which causes the tox to fail. We use this to catch the exit status and convert
```

### Comparing `plopp-24.4.0/tests/core/graph_test.py` & `plopp-24.5.0/tests/core/graph_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/core/limits_test.py` & `plopp-24.5.0/tests/core/limits_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/core/node_test.py` & `plopp-24.5.0/tests/core/node_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -122,15 +122,32 @@
     a.notify_children(message='hello from a')
     assert log == 'abcd'  # 'a' should only appear once in the log
     log = ''
     c.notify_children(message='hello from c')
     assert log == 'cd'  # 'c' requests data from 'a' but 'a' is cached so no 'a' in log
 
 
-def test_remove_node():
+def test_remove_node_args():
+    a = Node(lambda: 5)
+    b = Node(lambda x: x - 2, a)
+    c = Node(lambda x: x + 2, a)
+    bv = DataView(b)
+    cv = DataView(c)
+    assert a is b.parents[0]
+    assert b in a.children
+    assert c in a.children
+    assert bv in b.views
+    b.remove()
+    assert bv not in b.views
+    assert b not in a.children
+    assert c in a.children
+    assert cv in c.views
+
+
+def test_remove_node_kwargs():
     a = Node(lambda: 5)
     b = Node(lambda x: x - 2, x=a)
     c = Node(lambda x: x + 2, x=a)
     bv = DataView(b)
     cv = DataView(c)
     assert 'x' in b.kwparents
     assert a is b.kwparents['x']
@@ -140,22 +157,48 @@
     b.remove()
     assert bv not in b.views
     assert b not in a.children
     assert c in a.children
     assert cv in c.views
 
 
-def test_cannot_remove_node_with_children():
+def test_remove_node_with_children_args():
+    a = Node(lambda: 5)
+    b = Node(lambda x: x - 2, a)
+    av = DataView(a)
+    a.remove()
+    assert b not in a.children
+    assert a not in b.parents
+    assert a not in b.kwparents.values()
+    assert av not in a.views
+
+
+def test_remove_node_with_children_multiple_args():
+    a = Node(lambda: 5)
+    b = Node(lambda: 3)
+    c = Node(lambda: 11)
+    d = Node(lambda *args: sum(args), a, b, c)
+    assert d() == 19
+    a.remove()
+    assert d() == 14
+    b.remove()
+    assert d() == 11
+    c.remove()
+    assert d() == 0
+
+
+def test_remove_node_with_children_kwargs():
     a = Node(lambda: 5)
     b = Node(lambda x: x - 2, x=a)
     av = DataView(a)
-    with pytest.raises(RuntimeError, match="Cannot delete node"):
-        a.remove()
-    assert b in a.children
-    assert av in a.views
+    a.remove()
+    assert b not in a.children
+    assert a not in b.parents
+    assert a not in b.kwparents.values()
+    assert av not in a.views
 
 
 def add(x, y):
     return x + y
 
 
 def test_node_converts_raw_data_to_Node():
```

### Comparing `plopp-24.4.0/tests/core/utils_test.py` & `plopp-24.5.0/tests/core/utils_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/graphics/colormapper_test.py` & `plopp-24.5.0/tests/graphics/colormapper_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     assert mapper.normalizer.vmax == (da.max() * const).value
 
 
 def test_rgba():
     da = data_array(ndim=2, unit='K')
     mapper = ColorMapper()
     colors = mapper.rgba(da)
-    assert colors.shape == da.data.shape + (4,)
+    assert colors.shape == (*da.data.shape, 4)
 
 
 def test_rgba_with_masks():
     da1 = data_array(ndim=2, unit='K')
     da2 = data_array(ndim=2, unit='K', masks=True)
     mapper = ColorMapper()
     assert not np.allclose(mapper.rgba(da1), mapper.rgba(da2))
```

### Comparing `plopp-24.4.0/tests/graphics/imageview_test.py` & `plopp-24.5.0/tests/graphics/imageview_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,30 +31,30 @@
         fig.update(data3d=data_array(ndim=3))
 
 
 def test_create_with_node():
     da = data_array(ndim=2)
     fig = ImageView(Node(da))
     assert len(fig.artists) == 1
-    assert sc.identical(list(fig.artists.values())[0]._data, da)
+    assert sc.identical(next(iter(fig.artists.values()))._data, da)
 
 
 def test_create_with_bin_edges():
     da = data_array(ndim=2, binedges=True)
     fig = ImageView(Node(da))
     assert len(fig.artists) == 1
-    assert sc.identical(list(fig.artists.values())[0]._data, da)
+    assert sc.identical(next(iter(fig.artists.values()))._data, da)
 
 
 def test_create_with_only_one_bin_edge_coord():
     da = data_array(ndim=2, binedges=True)
     da.coords['xx'] = sc.midpoints(da.coords['xx'])
     fig = ImageView(Node(da))
     assert len(fig.artists) == 1
-    assert sc.identical(list(fig.artists.values())[0]._data, da)
+    assert sc.identical(next(iter(fig.artists.values()))._data, da)
 
 
 def test_log_norm():
     fig = ImageView(norm='log')
     assert fig.colormapper.norm == 'log'
```

### Comparing `plopp-24.4.0/tests/graphics/lineview_test.py` & `plopp-24.5.0/tests/graphics/lineview_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,35 +31,35 @@
         fig.update(data3d=data_array(ndim=3))
 
 
 def test_create_with_node():
     da = data_array(ndim=1)
     fig = LineView(Node(da))
     assert len(fig.artists) == 1
-    line = list(fig.artists.values())[0]
+    [line] = fig.artists.values()
     assert sc.identical(line._data, da)
     assert line._error is None
 
 
 def test_with_errorbars():
     da = data_array(ndim=1, variances=True)
     fig = LineView(Node(da))
     assert len(fig.artists) == 1
-    line = list(fig.artists.values())[0]
+    [line] = fig.artists.values()
     assert line._error is not None
     fig = LineView(Node(da), errorbars=False)
-    line = list(fig.artists.values())[0]
+    [line] = fig.artists.values()
     assert line._error is None
 
 
 def test_with_binedges():
     da = data_array(ndim=1, binedges=True)
     fig = LineView(Node(da))
     assert len(fig.artists) == 1
-    line = list(fig.artists.values())[0]
+    [line] = fig.artists.values()
     assert sc.identical(line._data, da)
     xdata = line._line.get_xdata()
     assert np.allclose(xdata, da.coords['xx'].values)
     assert len(xdata) == da.sizes['xx'] + 1
 
 
 def test_log_norm():
@@ -69,38 +69,38 @@
     assert fig.canvas.yscale == 'log'
 
 
 def test_update_grows_limits():
     da = data_array(ndim=1)
     fig = LineView(Node(da))
     old_lims = fig.canvas.yrange
-    key = list(fig.artists.keys())[0]
+    [key] = fig.artists.keys()
     fig.update({key: da * 2.5})
     new_lims = fig.canvas.yrange
     assert new_lims[0] < old_lims[0]
     assert new_lims[1] > old_lims[1]
 
 
 def test_update_does_shrink_limits_if_auto_mode():
     da = data_array(ndim=1)
     fig = LineView(Node(da), autoscale='auto')
     old_lims = fig.canvas.yrange
-    key = list(fig.artists.keys())[0]
+    [key] = fig.artists.keys()
     const = 0.5
     fig.update({key: da * const})
     new_lims = fig.canvas.yrange
     assert new_lims[0] == old_lims[0] * const
     assert new_lims[1] == old_lims[1] * const
 
 
 def test_update_does_not_shrink_limits_if_grow_mode():
     da = data_array(ndim=1)
     fig = LineView(Node(da), autoscale='grow')
     old_lims = fig.canvas.yrange
-    key = list(fig.artists.keys())[0]
+    [key] = fig.artists.keys()
     fig.update({key: da * 0.5})
     new_lims = fig.canvas.yrange
     assert new_lims[0] == old_lims[0]
     assert new_lims[1] == old_lims[1]
 
 
 def test_vmin():
```

### Comparing `plopp-24.4.0/tests/graphics/scatter3dview_test.py` & `plopp-24.5.0/tests/graphics/scatter3dview_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 from plopp.graphics.scatter3dview import Scatter3dView
 
 
 def test_creation():
     da = scatter()
     fig = Scatter3dView(Node(da), x='x', y='y', z='z')
     assert len(fig.artists) == 1
-    key = list(fig.artists.keys())[0]
+    [key] = fig.artists.keys()
     assert sc.identical(fig.artists[key]._data, da)
 
 
 def test_update():
     da = scatter()
     fig = Scatter3dView(Node(da), x='x', y='y', z='z')
     assert len(fig.artists) == 1
-    key = list(fig.artists.keys())[0]
+    [key] = fig.artists.keys()
     fig.update({key: da * 3.3})
     assert sc.identical(fig.artists[key]._data, da * 3.3)
 
 
 def test_log_norm():
     da = scatter()
     fig = Scatter3dView(Node(da), x='x', y='y', z='z', norm='log')
```

### Comparing `plopp-24.4.0/tests/graphics/scatterview_test.py` & `plopp-24.5.0/tests/graphics/scatterview_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 from plopp.graphics.scatterview import ScatterView
 
 
 def test_creation():
     da = scatter_data()
     fig = ScatterView(Node(da), x='x', y='y')
     assert len(fig.artists) == 1
-    key = list(fig.artists.keys())[0]
+    [key] = fig.artists.keys()
     assert sc.identical(fig.artists[key]._data, da)
 
 
 def test_update():
     da = scatter_data()
     fig = ScatterView(Node(da), x='x', y='y')
     assert len(fig.artists) == 1
-    key = list(fig.artists.keys())[0]
+    [key] = fig.artists.keys()
     fig.update({key: da * 3.3})
     assert sc.identical(fig.artists[key]._data, da * 3.3)
 
 
 def test_raises_for_new_data_with_incompatible_coordinate():
     a = scatter_data()
     b = scatter_data()
```

### Comparing `plopp-24.4.0/tests/high_level_test.py` & `plopp-24.5.0/tests/high_level_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/plotting/common_test.py` & `plopp-24.5.0/tests/plotting/common_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         (sc.DType.rotation3, (4,)),
         (sc.DType.translation3, (3,)),
         (sc.DType.vector3, (3,)),
     ],
 )
 def test_preprocess_raises_for_unsupported_dtype(dtype_and_shape):
     dtype, shape = dtype_and_shape
-    x = np.random.random(shape + (5,))
+    x = np.random.random((*shape, 5))
     values = x / np.broadcast_to(
         np.linalg.norm(x, axis=tuple(range(len(shape)))), x.shape
     )
     v = sc.Variable(dims=['x'], values=values.T, dtype=dtype)
     with pytest.raises(
         TypeError,
         match=f'The input has dtype {dtype} which is not supported by Plopp',
```

### Comparing `plopp-24.4.0/tests/plotting/inspector_test.py` & `plopp-24.5.0/tests/plotting/inspector_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,50 +2,56 @@
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 import pytest
 import scipp as sc
 
 import plopp as pp
 
 
-def test_creation(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_creation():
     da = pp.data.data3d()
     pp.inspector(da)
 
 
-def test_from_node(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_from_node():
     da = pp.data.data3d()
     pp.inspector(pp.Node(da))
 
 
-def test_multiple_inputs_raises(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_multiple_inputs_raises():
     da = pp.data.data3d()
     with pytest.raises(TypeError, match='Cannot convert input of type'):
         pp.inspector({'a': da, 'b': 2.3 * da})
 
 
-def test_bad_number_of_dims_raises(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_bad_number_of_dims_raises():
     with pytest.raises(
         ValueError,
         match='The inspector plot currently only works with three-dimensional data',
     ):
         pp.inspector(pp.data.data2d())
     with pytest.raises(
         ValueError,
         match='The inspector plot currently only works with three-dimensional data',
     ):
         pp.inspector(pp.data.data_array(ndim=4))
 
 
-def test_raises_ValueError_when_given_binned_data(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_raises_ValueError_when_given_binned_data():
     da = sc.data.table_xyz(100).bin(x=10, y=20, z=30)
     with pytest.raises(ValueError, match='Cannot plot binned data'):
         pp.inspector(da, orientation='vertical')
 
 
-def test_line_creation(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_line_creation():
     da = pp.data.data3d()
     ip = pp.inspector(da)
     fig2d = ip[0][0]
     fig1d = ip[0][1]
     # Activate the inspector tool
     fig2d.toolbar['inspect'].value = True
     assert not fig1d.canvas.dims
@@ -53,15 +59,16 @@
     fig2d.toolbar['inspect']._tool.click(10, 10)
     assert fig1d.canvas.dims == {'x': da.dims[-1]}
     assert len(fig1d.artists) == 1
     fig2d.toolbar['inspect']._tool.click(20, 15)
     assert len(fig1d.artists) == 2
 
 
-def test_line_removal(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_line_removal():
     da = pp.data.data3d()
     ip = pp.inspector(da)
     fig2d = ip[0][0]
     fig1d = ip[0][1]
     fig2d.toolbar['inspect'].value = True
     assert not fig1d.canvas.dims
     assert len(fig1d.artists) == 0
@@ -72,13 +79,14 @@
     assert len(fig1d.artists) == 2
     fig2d.toolbar['inspect']._tool.remove(1)
     assert len(fig1d.artists) == 1
     fig2d.toolbar['inspect']._tool.remove(0)
     assert len(fig1d.artists) == 0
 
 
-def test_operation(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_operation():
     da = pp.data.data3d()
     ip_sum = pp.inspector(da, operation='sum')
     ip_mean = pp.inspector(da, operation='mean')
     assert ip_sum[0][0]._view.colormapper.vmax > ip_mean[0][0]._view.colormapper.vmax
     assert ip_sum[0][0]._view.colormapper.vmin < ip_mean[0][0]._view.colormapper.vmin
```

### Comparing `plopp-24.4.0/tests/plotting/plot_1d_test.py` & `plopp-24.5.0/tests/plotting/plot_1d_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         fig.save(filename=fname)
         assert os.path.isfile(fname)
 
 
 def test_save_to_disk_with_bad_extension_raises():
     da = data_array(ndim=1)
     fig = pp.plot(da)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='txt'):
         fig.save(filename='plopp_fig1d.txt')
 
 
 def test_plot_xarray_data_array_1d():
     import xarray as xr
 
     N = 50
@@ -259,15 +259,15 @@
 
 def test_plot_pandas_series():
     import pandas as pd
 
     s = pd.Series(np.arange(100.0), name='MyDataSeries')
     p = pp.plot(s)
     assert p.canvas.dims['x'] == 'row'
-    assert list(p._view.artists.values())[0].label == 'MyDataSeries'
+    assert next(iter(p._view.artists.values())).label == 'MyDataSeries'
 
 
 def test_plot_pandas_dataframe():
     import pandas as pd
 
     df = pd.DataFrame(
         {
```

### Comparing `plopp-24.4.0/tests/plotting/plot_2d_test.py` & `plopp-24.5.0/tests/plotting/plot_2d_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         fig.save(filename=fname)
         assert os.path.isfile(fname)
 
 
 def test_save_to_disk_with_bad_extension_raises():
     da = data_array(ndim=2)
     fig = pp.plot(da)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='txt'):
         fig.save(filename='plopp_fig2d.txt')
 
 
 def test_plot_raises_with_multiple_2d_inputs():
     a = data_array(ndim=2)
     b = 3.3 * a
     with pytest.raises(
```

### Comparing `plopp-24.4.0/tests/plotting/scatter3d_test.py` & `plopp-24.5.0/tests/plotting/scatter3d_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,31 +30,31 @@
     x = sc.linspace(dim='x', start=-10.0, stop=10.0, num=nx, unit='m')
     y = sc.linspace(dim='y', start=-10.0, stop=10.0, num=ny, unit='m')
     da = sc.DataArray(
         data=sc.array(dims=['x', 'y'], values=np.random.rand(nx, ny)),
         coords={'position': sc.spatial.as_vectors(x, y, 0.0 * sc.units.m)},
     )
     p = pp.scatter3d(da, pos="position")
-    assert list(p.artists.values())[0].data.ndim == 1
+    assert next(iter(p.artists.values())).data.ndim == 1
     nz = 12
     z = sc.linspace(dim='z', start=-10.0, stop=10.0, num=nz, unit='m')
     da = sc.DataArray(
         data=sc.array(dims=['x', 'y', 'z'], values=np.random.rand(nx, ny, nz)),
         coords={'position': sc.spatial.as_vectors(x, y, z)},
     )
     p = pp.scatter3d(da, pos="position")
-    assert list(p.artists.values())[0].data.ndim == 1
+    assert next(iter(p.artists.values())).data.ndim == 1
 
 
 def test_scatter3d_can_plot_scalar_data():
     da = sc.DataArray(
         data=sc.scalar(1.2), coords={'position': sc.vector(value=[1, 2, 3])}
     )
     p = pp.scatter3d(da, pos='position')
-    assert list(p.artists.values())[0].data.ndim == 1
+    assert next(iter(p.artists.values())).data.ndim == 1
 
 
 def test_raises_ValueError_when_given_binned_data():
     nx = 10
     da = sc.data.table_xyz(100).bin(x=nx)
     x = sc.linspace(dim='x', start=-10.0, stop=10.0, num=nx, unit='m')
     da.coords['position'] = sc.spatial.as_vectors(x, x, x)
```

### Comparing `plopp-24.4.0/tests/plotting/scatter_test.py` & `plopp-24.5.0/tests/plotting/scatter_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/plotting/slicer_test.py` & `plopp-24.5.0/tests/plotting/slicer_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,146 +5,162 @@
 import scipp as sc
 
 from plopp import Node
 from plopp.data.testing import data_array, dataset
 from plopp.plotting.slicer import Slicer
 
 
-def test_creation_keep_two_dims(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_creation_keep_two_dims():
     da = data_array(ndim=3)
     sl = Slicer(da, keep=['xx', 'yy'])
     assert sl.slider.value == {'zz': 0}
     assert sl.slider.controls['zz']['slider'].max == da.sizes['zz'] - 1
     assert sc.identical(sl.slice_nodes[0].request_data(), da['zz', 0])
 
 
-def test_creation_keep_one_dim(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_creation_keep_one_dim():
     da = data_array(ndim=3)
     sl = Slicer(da, keep=['xx'])
     assert sl.slider.value == {'zz': 0, 'yy': 0}
     assert sl.slider.controls['yy']['slider'].max == da.sizes['yy'] - 1
     assert sl.slider.controls['zz']['slider'].max == da.sizes['zz'] - 1
     assert sc.identical(sl.slice_nodes[0].request_data(), da['yy', 0]['zz', 0])
 
 
-def test_update_keep_two_dims(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_update_keep_two_dims():
     da = data_array(ndim=3)
     sl = Slicer(da, keep=['xx', 'yy'])
     assert sl.slider.value == {'zz': 0}
     assert sc.identical(sl.slice_nodes[0].request_data(), da['zz', 0])
     sl.slider.controls['zz']['slider'].value = 5
     assert sl.slider.value == {'zz': 5}
     assert sc.identical(sl.slice_nodes[0].request_data(), da['zz', 5])
 
 
-def test_update_keep_one_dim(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_update_keep_one_dim():
     da = data_array(ndim=3)
     sl = Slicer(da, keep=['xx'])
     assert sl.slider.value == {'zz': 0, 'yy': 0}
     assert sc.identical(sl.slice_nodes[0].request_data(), da['yy', 0]['zz', 0])
     sl.slider.controls['yy']['slider'].value = 5
     assert sl.slider.value == {'zz': 0, 'yy': 5}
     assert sc.identical(sl.slice_nodes[0].request_data(), da['yy', 5]['zz', 0])
     sl.slider.controls['zz']['slider'].value = 8
     assert sl.slider.value == {'zz': 8, 'yy': 5}
     assert sc.identical(sl.slice_nodes[0].request_data(), da['yy', 5]['zz', 8])
 
 
-def test_with_dataset(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_with_dataset():
     ds = dataset(ndim=2)
     sl = Slicer(ds, keep=['xx'])
     nodes = list(sl.figure.graph_nodes.values())
     sl.slider.controls['yy']['slider'].value = 5
     assert sc.identical(nodes[0].request_data(), ds['a']['yy', 5])
     assert sc.identical(nodes[1].request_data(), ds['b']['yy', 5])
 
 
-def test_with_data_group(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_with_data_group():
     da = data_array(ndim=2)
     dg = sc.DataGroup(a=da, b=da * 2.5)
     sl = Slicer(dg, keep=['xx'])
     nodes = list(sl.figure.graph_nodes.values())
     sl.slider.controls['yy']['slider'].value = 5
     assert sc.identical(nodes[0].request_data(), dg['a']['yy', 5])
     assert sc.identical(nodes[1].request_data(), dg['b']['yy', 5])
 
 
-def test_with_dict_of_data_arrays(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_with_dict_of_data_arrays():
     a = data_array(ndim=2)
     b = data_array(ndim=2) * 2.5
     sl = Slicer({'a': a, 'b': b}, keep=['xx'])
     nodes = list(sl.figure.graph_nodes.values())
     sl.slider.controls['yy']['slider'].value = 5
     assert sc.identical(nodes[0].request_data(), a['yy', 5])
     assert sc.identical(nodes[1].request_data(), b['yy', 5])
 
 
-def test_with_data_arrays_same_shape_different_coord(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_with_data_arrays_same_shape_different_coord():
     a = data_array(ndim=2)
     b = data_array(ndim=2) * 2.5
     b.coords['xx'] *= 1.5
     Slicer({'a': a, 'b': b}, keep=['xx'])
 
 
-def test_with_data_arrays_different_shape_along_keep_dim(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_with_data_arrays_different_shape_along_keep_dim():
     a = data_array(ndim=2)
     b = data_array(ndim=2) * 2.5
     Slicer({'a': a, 'b': b['xx', :10]}, keep=['xx'])
 
 
-def test_with_data_arrays_different_shape_along_non_keep_dim_raises(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_with_data_arrays_different_shape_along_non_keep_dim_raises():
     a = data_array(ndim=2)
     b = data_array(ndim=2) * 2.5
     with pytest.raises(
         ValueError, match='Slicer plot: all inputs must have the same sizes'
     ):
         Slicer({'a': a, 'b': b['yy', :10]}, keep=['xx'])
 
 
-def test_raises_ValueError_when_given_binned_data(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_raises_ValueError_when_given_binned_data():
     da = sc.data.table_xyz(100).bin(x=10, y=20)
     with pytest.raises(ValueError, match='Cannot plot binned data'):
         Slicer(da, keep=['xx'])
 
 
+@pytest.mark.usefixtures('_use_ipympl')
 @pytest.mark.parametrize('ndim', [2, 3])
-def test_from_node(use_ipympl, ndim):
+def test_from_node(ndim):
     da = data_array(ndim=ndim)
     Slicer(Node(da))
 
 
-def test_mixing_raw_data_and_nodes(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_mixing_raw_data_and_nodes():
     a = data_array(ndim=2)
     b = 6.7 * a
     Slicer({'a': Node(a), 'b': Node(b)})
     Slicer({'a': a, 'b': Node(b)})
     Slicer({'a': Node(a), 'b': b})
 
 
-def test_raises_when_requested_keep_dims_do_not_exist(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_raises_when_requested_keep_dims_do_not_exist():
     da = data_array(ndim=3)
     with pytest.raises(
         ValueError, match='Slicer plot: one or more of the requested dims to be kept'
     ):
         Slicer(da, keep=['time'])
 
 
-def test_raises_when_number_of_keep_dims_requested_is_bad(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_raises_when_number_of_keep_dims_requested_is_bad():
     da = data_array(ndim=4)
     with pytest.raises(
         ValueError, match='Slicer plot: the number of dims to be kept must be 1 or 2'
     ):
         Slicer(da, keep=['xx', 'yy', 'zz'])
     with pytest.raises(
         ValueError, match='Slicer plot: the list of dims to be kept cannot be empty'
     ):
         Slicer(da, keep=[])
 
 
-def test_autoscale_fixed(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_autoscale_fixed():
     da = sc.DataArray(
         data=sc.arange('x', 5 * 10 * 20).fold(dim='x', sizes={'z': 20, 'y': 10, 'x': 5})
     )
     sl = Slicer(da, keep=['y', 'x'], autoscale='fixed')
     assert sl.figure._view.colormapper.vmin == 0
     assert sl.figure._view.colormapper.vmax == 5 * 10 * 20 - 1
     sl.slider.controls['z']['slider'].value = 5
```

### Comparing `plopp-24.4.0/tests/plotting/superplot_test.py` & `plopp-24.5.0/tests/plotting/superplot_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 import scipp as sc
 
 from plopp import Node
 from plopp.data.testing import data_array
 from plopp.plotting.superplot import superplot
 
 
-def test_creation(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_creation():
     da = data_array(ndim=2)
     sp = superplot(da, keep='xx')
     assert len(sp.right_bar[0]._lines) == 0
 
 
-def test_from_node(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_from_node():
     da = data_array(ndim=2)
     superplot(Node(da))
 
 
-def test_save_line(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_save_line():
     da = data_array(ndim=2)
     sp = superplot(da, keep='xx')
     tool = sp.right_bar[0]
     assert len(tool._lines) == 0
     tool.save_line()
     assert len(tool._lines) == 1
     line = list(tool._lines.values())[-1]
@@ -35,15 +38,16 @@
     tool.save_line()
     assert len(tool._lines) == 2
     line = list(tool._lines.values())[-1]
     assert sc.identical(line['line']._data, da['yy', 5])
     assert len(tool.container.children) == 2
 
 
-def test_remove_line(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_remove_line():
     da = data_array(ndim=2)
     sp = superplot(da, keep='xx')
     tool = sp.right_bar[0]
     assert len(tool._lines) == 0
     tool.save_line()
     slider = sp.bottom_bar[0]
     slider.controls['yy']['slider'].value = 5
@@ -62,21 +66,23 @@
     assert len(tool.container.children) == 2
 
     tool.remove_line(change=None, line_id=last_line)
     assert last_line not in tool._lines
     assert len(tool.container.children) == 1
 
 
-def test_change_line_color(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_change_line_color():
     da = data_array(ndim=2)
     sp = superplot(da, keep='xx')
     tool = sp.right_bar[0]
     tool.save_line()
     line_id = list(tool._lines.keys())[-1]
     tool.change_line_color(change={'new': '#000000'}, line_id=line_id)
     assert tool._lines[line_id]['line'].color == '#000000'
 
 
-def test_raises_ValueError_when_given_binned_data(use_ipympl):
+@pytest.mark.usefixtures('_use_ipympl')
+def test_raises_ValueError_when_given_binned_data():
     da = sc.data.table_xyz(100).bin(x=10, y=20)
     with pytest.raises(ValueError, match='Cannot plot binned data'):
         superplot(da, keep='x')
```

### Comparing `plopp-24.4.0/tests/plotting/xyplot_test.py` & `plopp-24.5.0/tests/plotting/xyplot_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,23 +55,23 @@
 
 
 def test_xyplot_variable_kwargs():
     x = sc.arange('time', 20.0, unit='s')
     y = sc.arange('time', 100.0, 120.0, unit='K')
     fig = pp.xyplot(x, y, color='red', vmin=102.0, vmax=115.0)
     assert np.allclose(fig.canvas.yrange, [102.0, 115.0])
-    line = list(fig.artists.values())[0]
+    [line] = fig.artists.values()
     assert line.color == 'red'
 
 
 def test_xyplot_bin_edges():
     x = sc.arange('time', 21.0, unit='s')
     y = sc.arange('time', 100.0, 120.0, unit='K')
     fig = pp.xyplot(x, y)
-    line = list(fig.artists.values())[0]
+    [line] = fig.artists.values()
     assert len(line._line.get_xdata()) == 21
 
 
 def test_xyplot_from_nodes():
     x = sc.arange('time', 20.0, unit='s')
     y = sc.arange('time', 100.0, 120.0, unit='K')
     pp.xyplot(pp.Node(x), y)
```

### Comparing `plopp-24.4.0/tests/widgets/box_test.py` & `plopp-24.5.0/tests/widgets/box_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/widgets/checkboxes_test.py` & `plopp-24.5.0/tests/widgets/checkboxes_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/widgets/clip3d_test.py` & `plopp-24.5.0/tests/widgets/clip3d_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/widgets/cut3d_test.py` & `plopp-24.5.0/tests/widgets/cut3d_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.4.0/tests/widgets/slice_test.py` & `plopp-24.5.0/tests/widgets/slice_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
+import pytest
 from scipp import identical
 
 from plopp.data.testing import data_array
-from plopp.widgets import SliceWidget, slice_dims
+from plopp.widgets import RangeSliceWidget, SliceWidget, slice_dims
 
 
-def test_slice_creation():
+@pytest.mark.parametrize("widget", [SliceWidget, RangeSliceWidget])
+def test_slice_creation(widget):
     da = data_array(ndim=3)
-    sw = SliceWidget(da, dims=['yy', 'xx'])
+    sw = widget(da, dims=['yy', 'xx'])
     assert sw._slider_dims == ['yy', 'xx']
     assert sw.controls['xx']['slider'].min == 0
     assert sw.controls['xx']['slider'].max == da.sizes['xx'] - 1
     assert sw.controls['xx']['slider'].description == 'xx'
     assert sw.controls['yy']['slider'].min == 0
     assert sw.controls['yy']['slider'].max == da.sizes['yy'] - 1
     assert sw.controls['yy']['slider'].description == 'yy'
@@ -41,7 +43,14 @@
 
 
 def test_slice_dims():
     da = data_array(ndim=3)
     slices = {'xx': 8, 'yy': 7}
     expected = da['xx', slices['xx']]['yy', slices['yy']]
     assert identical(slice_dims().func(da, slices=slices), expected)
+
+
+def test_range_slice_dims():
+    da = data_array(ndim=3)
+    slices = {'xx': (8, 9), 'yy': (7, 10)}
+    expected = da['xx', slice(*slices['xx'])]['yy', slice(*slices['yy'])]
+    assert identical(slice_dims().func(da, slices=slices), expected)
```

### Comparing `plopp-24.4.0/tox.ini` & `plopp-24.5.0/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py39
+envlist = py310
 isolated_build = true
 
 [testenv]
 deps = -r requirements/test.txt
 setenv =
   JUPYTER_PLATFORM_DIRS = 1
 commands = pytest {posargs}
@@ -16,31 +16,34 @@
 [testenv:noplotly]
 description = Test that plotly tests are skipped if plotly is not installed
 deps = -r requirements/noplotly.txt
 commands = pytest tests/backends/plotly
 
 [testenv:nightly]
 deps = -r requirements/nightly.txt
-commands = pytest
+commands = pytest {posargs}
 
 [testenv:unpinned]
 description = Test with unpinned dependencies, as a user would install now.
 deps =
   -r requirements/basetest.txt
   -r requirements/base.in
   -r requirements/optional.in
   plopp
-commands = pytest
+commands = pytest {posargs}
 
 [testenv:docs]
 description = invoke sphinx-build to build the HTML docs
 deps = -r requirements/docs.txt
 allowlist_externals=find
-commands = python -m sphinx -j2 -v -b html -d {toxworkdir}/docs_doctrees docs html
-           python -m sphinx -j2 -v -b doctest -d {toxworkdir}/docs_doctrees docs html
+# pydata_sphinx_theme raises a warning that it's not parallel-write-safe
+# https://github.com/pydata/pydata-sphinx-theme/issues/1643, removing -j2 for now
+# from SPHINXOPTS
+commands = python -m sphinx -W -v -b html -d {toxworkdir}/docs_doctrees docs html
+           python -m sphinx -W -v -b doctest -d {toxworkdir}/docs_doctrees docs html
            find html -type f -name "*.ipynb" -not -path "html/_sources/*" -delete
 
 [testenv:releasedocs]
 description = invoke sphinx-build to build the HTML docs from a released version
 skip_install = true
 deps =
   plopp=={posargs}
```

