# Comparing `tmp/mizani-0.9.2.tar.gz` & `tmp/mizani-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizani-0.9.2.tar", last modified: Thu May 25 18:59:06 2023, max compression
+gzip compressed data, was "mizani-0.9.3.tar", last modified: Fri Sep  1 12:30:43 2023, max compression
```

## Comparing `mizani-0.9.2.tar` & `mizani-0.9.3.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.018121 mizani-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 18:58:55.000000 mizani-0.9.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.006120 mizani-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.010120 mizani-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-25 18:58:55.000000 mizani-0.9.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-25 18:58:55.000000 mizani-0.9.2/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-25 18:58:55.000000 mizani-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-25 18:58:55.000000 mizani-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-25 18:58:55.000000 mizani-0.9.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-25 18:58:55.000000 mizani-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-25 18:58:55.000000 mizani-0.9.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-25 18:59:06.018121 mizani-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-25 18:58:55.000000 mizani-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-25 18:58:55.000000 mizani-0.9.2/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.010120 mizani-0.9.2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.010120 mizani-0.9.2/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/_static/copybutton.js
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/bounds.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/breaks.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13151 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/docutils.conf
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/formatters.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/palettes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/scale.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.010120 mizani-0.9.2/doc/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/sphinxext/inline_code_highlight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.014120 mizani-0.9.2/doc/theme/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/navbar-2.html
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/navbar.html
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/navbarsearchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/navbartoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/relations.html
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/searchresults.html
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/sourcelink.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.014120 mizani-0.9.2/doc/theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.006120 mizani-0.9.2/doc/theme/static/bootstrap-3.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.014120 mizani-0.9.2/doc/theme/static/bootstrap-3.4.1/css/
--rw-r--r--   0 runner    (1001) docker     (123)   124135 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/static/bootstrap-3.4.1/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.014120 mizani-0.9.2/doc/theme/static/bootstrap-3.4.1/js/
--rw-r--r--   0 runner    (1001) docker     (123)    40021 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/static/bootstrap-3.4.1/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/static/bootstrap-sphinx.css_t
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/static/bootstrap-sphinx.js_t
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.014120 mizani-0.9.2/doc/theme/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    97163 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/static/js/jquery-1.12.4.min.js
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/static/js/jquery-fix.js
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/transforms.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.014120 mizani-0.9.2/licences/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-25 18:58:55.000000 mizani-0.9.2/licences/HUSL_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-25 18:58:55.000000 mizani-0.9.2/licences/SCALES_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-25 18:58:55.000000 mizani-0.9.2/licences/SEABORN_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 18:58:55.000000 mizani-0.9.2/licences/SIX_LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.014120 mizani-0.9.2/mizani/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    26005 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/breaks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.018121 mizani-0.9.2/mizani/colors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/colors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.018121 mizani-0.9.2/mizani/colors/brewer/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/colors/brewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/colors/brewer/diverging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/colors/brewer/qualitative.py
--rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/colors/brewer/sequential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/colors/color_palette.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.018121 mizani-0.9.2/mizani/external/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/external/crayon_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/external/husl.py
--rw-r--r--   0 runner    (1001) docker     (123)    28029 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/external/xkcd_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    22688 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/palettes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/scale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.018121 mizani-0.9.2/mizani/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/tests/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/tests/test_breaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/tests/test_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/tests/test_palettes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/tests/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21685 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.018121 mizani-0.9.2/mizani.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-25 18:59:05.000000 mizani-0.9.2/mizani.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-25 18:59:06.000000 mizani-0.9.2/mizani.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 18:59:05.000000 mizani-0.9.2/mizani.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-25 18:59:05.000000 mizani-0.9.2/mizani.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 18:59:05.000000 mizani-0.9.2/mizani.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-05-25 18:58:55.000000 mizani-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 18:59:06.018121 mizani-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.018121 mizani-0.9.2/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-05-25 18:58:55.000000 mizani-0.9.2/tools/build_theme.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-25 18:58:55.000000 mizani-0.9.2/tools/gha_check_semver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-25 18:58:55.000000 mizani-0.9.2/tools/release-checklist.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.414949 mizani-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (999)       32 2023-09-01 12:30:32.000000 mizani-0.9.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.398948 mizani-0.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.402948 mizani-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (999)     2221 2023-09-01 12:30:32.000000 mizani-0.9.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (999)     2949 2023-09-01 12:30:32.000000 mizani-0.9.3/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      751 2023-09-01 12:30:32.000000 mizani-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (999)      271 2023-09-01 12:30:32.000000 mizani-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (999)      528 2023-09-01 12:30:32.000000 mizani-0.9.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (999)     1478 2023-09-01 12:30:32.000000 mizani-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)     1565 2023-09-01 12:30:32.000000 mizani-0.9.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (999)     3753 2023-09-01 12:30:43.414949 mizani-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     1043 2023-09-01 12:30:32.000000 mizani-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (999)      375 2023-09-01 12:30:32.000000 mizani-0.9.3/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.406949 mizani-0.9.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (999)     1134 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.406949 mizani-0.9.3/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (999)     3143 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/_static/copybutton.js
+-rw-r--r--   0 runner    (1001) docker     (999)     2494 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (999)      148 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/bounds.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      182 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/breaks.rst
+-rw-r--r--   0 runner    (1001) docker     (999)    13256 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (999)    11659 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (999)      118 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/docutils.conf
+-rw-r--r--   0 runner    (1001) docker     (999)      158 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/formatters.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      362 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      967 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      170 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/palettes.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      116 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/scale.rst
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.406949 mizani-0.9.3/doc/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      368 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/sphinxext/inline_code_highlight.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.406949 mizani-0.9.3/doc/theme/
+-rw-r--r--   0 runner    (1001) docker     (999)      455 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (999)     3664 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (999)       10 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (999)     2002 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/navbar-2.html
+-rw-r--r--   0 runner    (1001) docker     (999)     2072 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (999)      360 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/navbarsearchbox.html
+-rw-r--r--   0 runner    (1001) docker     (999)      305 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/navbartoc.html
+-rw-r--r--   0 runner    (1001) docker     (999)     1111 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/relations.html
+-rw-r--r--   0 runner    (1001) docker     (999)     2614 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/search.html
+-rw-r--r--   0 runner    (1001) docker     (999)      327 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (999)     1120 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/searchresults.html
+-rw-r--r--   0 runner    (1001) docker     (999)      195 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/sourcelink.html
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.406949 mizani-0.9.3/doc/theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.398948 mizani-0.9.3/doc/theme/static/bootstrap-3.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.406949 mizani-0.9.3/doc/theme/static/bootstrap-3.4.1/css/
+-rw-r--r--   0 runner    (1001) docker     (999)   124135 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/static/bootstrap-3.4.1/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.406949 mizani-0.9.3/doc/theme/static/bootstrap-3.4.1/js/
+-rw-r--r--   0 runner    (1001) docker     (999)    40021 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/static/bootstrap-3.4.1/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (999)     5924 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/static/bootstrap-sphinx.css_t
+-rw-r--r--   0 runner    (1001) docker     (999)     5162 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/static/bootstrap-sphinx.js_t
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.406949 mizani-0.9.3/doc/theme/static/js/
+-rw-r--r--   0 runner    (1001) docker     (999)    97163 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/static/js/jquery-1.12.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (999)       87 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/static/js/jquery-fix.js
+-rw-r--r--   0 runner    (1001) docker     (999)     1895 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (999)      188 2023-09-01 12:30:32.000000 mizani-0.9.3/doc/transforms.rst
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.410949 mizani-0.9.3/licences/
+-rw-r--r--   0 runner    (1001) docker     (999)     1059 2023-09-01 12:30:32.000000 mizani-0.9.3/licences/HUSL_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)       77 2023-09-01 12:30:32.000000 mizani-0.9.3/licences/SCALES_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)     1498 2023-09-01 12:30:32.000000 mizani-0.9.3/licences/SEABORN_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)     1066 2023-09-01 12:30:32.000000 mizani-0.9.3/licences/SIX_LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.410949 mizani-0.9.3/mizani/
+-rw-r--r--   0 runner    (1001) docker     (999)      172 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    15042 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (999)    26005 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/breaks.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.410949 mizani-0.9.3/mizani/colors/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/colors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.410949 mizani-0.9.3/mizani/colors/brewer/
+-rw-r--r--   0 runner    (1001) docker     (999)     1717 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/colors/brewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    17728 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/colors/brewer/diverging.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11725 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/colors/brewer/qualitative.py
+-rw-r--r--   0 runner    (1001) docker     (999)    24032 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/colors/brewer/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1942 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/colors/color_palette.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.410949 mizani-0.9.3/mizani/external/
+-rw-r--r--   0 runner    (1001) docker     (999)      104 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5055 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/external/crayon_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6488 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/external/husl.py
+-rw-r--r--   0 runner    (1001) docker     (999)    28029 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/external/xkcd_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (999)    22973 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (999)    22688 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/palettes.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7460 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/scale.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.414949 mizani-0.9.3/mizani/tests/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    13788 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/tests/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8243 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/tests/test_breaks.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8548 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/tests/test_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6085 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/tests/test_palettes.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3719 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7102 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4229 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (999)    21685 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (999)      698 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/typing.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7757 2023-09-01 12:30:32.000000 mizani-0.9.3/mizani/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.410949 mizani-0.9.3/mizani.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     3753 2023-09-01 12:30:43.000000 mizani-0.9.3/mizani.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     2085 2023-09-01 12:30:43.000000 mizani-0.9.3/mizani.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-01 12:30:43.000000 mizani-0.9.3/mizani.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      377 2023-09-01 12:30:43.000000 mizani-0.9.3/mizani.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        7 2023-09-01 12:30:43.000000 mizani-0.9.3/mizani.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)     3412 2023-09-01 12:30:32.000000 mizani-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-01 12:30:43.414949 mizani-0.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 12:30:43.414949 mizani-0.9.3/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (999)      862 2023-09-01 12:30:32.000000 mizani-0.9.3/tools/build_theme.sh
+-rw-r--r--   0 runner    (1001) docker     (999)     2215 2023-09-01 12:30:32.000000 mizani-0.9.3/tools/gha_check_semver.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2878 2023-09-01 12:30:32.000000 mizani-0.9.3/tools/release-checklist.md
```

### Comparing `mizani-0.9.2/.github/workflows/release.yml` & `mizani-0.9.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/.github/workflows/testing.yml` & `mizani-0.9.3/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/.gitignore` & `mizani-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/.readthedocs.yaml` & `mizani-0.9.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/LICENSE` & `mizani-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/Makefile` & `mizani-0.9.3/Makefile`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/PKG-INFO` & `mizani-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizani
-Version: 0.9.2
+Version: 0.9.3
 Summary: Scales for Python
 Author-email: Hassan Kibirige <has2k1@gmail.com>
 License: Copyright (c) 2016, Hassan Kibirige
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `mizani-0.9.2/README.md` & `mizani-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/Makefile` & `mizani-0.9.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/_static/copybutton.js` & `mizani-0.9.3/doc/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/_static/custom.css` & `mizani-0.9.3/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/changelog.rst` & `mizani-0.9.3/doc/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+v0.9.3
+------
+*2023-09-01*
+
+Enhancements
+************
+
+- Removed FutureWarnings when using pandas 2.1.0
+
 v0.9.2
 ------
 
 *2023-05-25*
 
 Bug Fixes
 *********
```

### Comparing `mizani-0.9.2/doc/conf.py` & `mizani-0.9.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/installation.rst` & `mizani-0.9.3/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/theme/layout.html` & `mizani-0.9.3/doc/theme/layout.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/theme/navbar-2.html` & `mizani-0.9.3/doc/theme/navbar-2.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/theme/navbar.html` & `mizani-0.9.3/doc/theme/navbar.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/theme/relations.html` & `mizani-0.9.3/doc/theme/relations.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/theme/search.html` & `mizani-0.9.3/doc/theme/search.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/theme/searchresults.html` & `mizani-0.9.3/doc/theme/searchresults.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/theme/static/bootstrap-3.4.1/css/bootstrap.min.css` & `mizani-0.9.3/doc/theme/static/bootstrap-3.4.1/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/theme/static/bootstrap-3.4.1/js/bootstrap.min.js` & `mizani-0.9.3/doc/theme/static/bootstrap-3.4.1/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/theme/static/bootstrap-sphinx.css_t` & `mizani-0.9.3/doc/theme/static/bootstrap-sphinx.css_t`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/theme/static/bootstrap-sphinx.js_t` & `mizani-0.9.3/doc/theme/static/bootstrap-sphinx.js_t`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/theme/static/js/jquery-1.12.4.min.js` & `mizani-0.9.3/doc/theme/static/js/jquery-1.12.4.min.js`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/doc/theme/theme.conf` & `mizani-0.9.3/doc/theme/theme.conf`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/licences/HUSL_LICENSE` & `mizani-0.9.3/licences/HUSL_LICENSE`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/licences/SEABORN_LICENSE` & `mizani-0.9.3/licences/SEABORN_LICENSE`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/licences/SIX_LICENSE` & `mizani-0.9.3/licences/SIX_LICENSE`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/bounds.py` & `mizani-0.9.3/mizani/bounds.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/breaks.py` & `mizani-0.9.3/mizani/breaks.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/colors/brewer/__init__.py` & `mizani-0.9.3/mizani/colors/brewer/__init__.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/colors/brewer/diverging.py` & `mizani-0.9.3/mizani/colors/brewer/diverging.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/colors/brewer/qualitative.py` & `mizani-0.9.3/mizani/colors/brewer/qualitative.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/colors/brewer/sequential.py` & `mizani-0.9.3/mizani/colors/brewer/sequential.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/colors/color_palette.py` & `mizani-0.9.3/mizani/colors/color_palette.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/external/crayon_rgb.py` & `mizani-0.9.3/mizani/external/crayon_rgb.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/external/husl.py` & `mizani-0.9.3/mizani/external/husl.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/external/xkcd_rgb.py` & `mizani-0.9.3/mizani/external/xkcd_rgb.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/formatters.py` & `mizani-0.9.3/mizani/formatters.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/palettes.py` & `mizani-0.9.3/mizani/palettes.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/scale.py` & `mizani-0.9.3/mizani/scale.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 values(potential readings) on a scale. This is perhaps the most important
 concept unpinning a scale.
 
 The **apply** methods are simple examples of how to put it all together.
 """
 import numpy as np
 import pandas as pd
-import pandas.api.types as pdtypes
 
 from .bounds import censor, rescale
 from .utils import (
     CONTINUOUS_KINDS,
     DISCRETE_KINDS,
     get_categories,
     match,
@@ -203,28 +202,29 @@
             new_data = np.asarray(new_data)
         new_data = new_data[~nan_bool_idx]
 
         if new_data.dtype.kind not in DISCRETE_KINDS:
             raise TypeError("Continuous value supplied to discrete scale")
 
         # Train i.e. get the new values
-        if pdtypes.is_categorical_dtype(new_data):
+        if isinstance(new_data.dtype, pd.CategoricalDtype):
             categories = get_categories(new_data)
             if drop:
                 present = set(new_data.drop_duplicates())
                 new = [i for i in categories if i in present]
             else:
                 new = list(categories)
         else:
             new = np.unique(new_data)
             new.sort()
 
         # update old
         old_set = set(old)
-        if pdtypes.is_categorical_dtype(new_data):
+
+        if isinstance(new_data.dtype, pd.CategoricalDtype):
             # The limits are in the order of the categories
             all_set = old_set | set(new)
             ordered_cats = categories.union(old, sort=False)
             limits = [c for c in ordered_cats if c in all_set]
         else:
             limits = old + [i for i in new if (i not in old_set)]
```

### Comparing `mizani-0.9.2/mizani/tests/test_bounds.py` & `mizani-0.9.3/mizani/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/tests/test_breaks.py` & `mizani-0.9.3/mizani/tests/test_breaks.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/tests/test_formatters.py` & `mizani-0.9.3/mizani/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/tests/test_palettes.py` & `mizani-0.9.3/mizani/tests/test_palettes.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/tests/test_scale.py` & `mizani-0.9.3/mizani/tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/tests/test_transforms.py` & `mizani-0.9.3/mizani/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/tests/test_utils.py` & `mizani-0.9.3/mizani/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/transforms.py` & `mizani-0.9.3/mizani/transforms.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/typing.py` & `mizani-0.9.3/mizani/typing.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani/utils.py` & `mizani-0.9.3/mizani/utils.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/mizani.egg-info/PKG-INFO` & `mizani-0.9.3/mizani.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizani
-Version: 0.9.2
+Version: 0.9.3
 Summary: Scales for Python
 Author-email: Hassan Kibirige <has2k1@gmail.com>
 License: Copyright (c) 2016, Hassan Kibirige
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `mizani-0.9.2/mizani.egg-info/SOURCES.txt` & `mizani-0.9.3/mizani.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/pyproject.toml` & `mizani-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/tools/build_theme.sh` & `mizani-0.9.3/tools/build_theme.sh`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/tools/gha_check_semver.py` & `mizani-0.9.3/tools/gha_check_semver.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.2/tools/release-checklist.md` & `mizani-0.9.3/tools/release-checklist.md`

 * *Files identical despite different names*

