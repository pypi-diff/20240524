# Comparing `tmp/mpl_ascii-0.6.2.tar.gz` & `tmp/mpl_ascii-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_ascii-0.6.2.tar", last modified: Sun May 19 13:36:22 2024, max compression
+gzip compressed data, was "mpl_ascii-0.6.3.tar", last modified: Fri May 24 16:57:56 2024, max compression
```

## Comparing `mpl_ascii-0.6.2.tar` & `mpl_ascii-0.6.3.tar`

### file list

```diff
@@ -1,84 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:36:22.713123 mpl_ascii-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:36:22.697123 mpl_ascii-0.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:36:22.697123 mpl_ascii-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-19 13:36:22.713123 mpl_ascii-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:36:22.709123 mpl_ascii-0.6.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_chart.txt
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_5.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_stacked.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_stacked.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/barh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/barh.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/box_plot_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/box_plot_basic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/categorical_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/categorical_variables.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/cohere.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/color_bar_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/color_bar_scatter.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/csd_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/csd_demo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/double_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/double_plot.txt
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/errorbars.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/errorbars.txt
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/errorbars_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/errorbars_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/errorbars_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/errorbars_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/errorbars_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/errorbars_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/hist_best_fit_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/hist_best_fit_line.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/hist_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/hist_simple.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/hist_simple_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/hist_simple_colors.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/line_markers.py
--rw-r--r--   0 runner    (1001) docker     (127)    38794 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/line_markers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/lines_multi_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/lines_multi_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/scatter_multi_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/scatter_multi_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/simple_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/simple_plot.txt
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/violin_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/violin_plot.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:36:22.709123 mpl_ascii-0.6.2/mpl_ascii/
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/mpl_ascii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/mpl_ascii/ascii_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/mpl_ascii/color_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    20303 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/mpl_ascii/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/mpl_ascii/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/mpl_ascii/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:36:22.709123 mpl_ascii-0.6.2/mpl_ascii.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-19 13:36:22.000000 mpl_ascii-0.6.2/mpl_ascii.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-19 13:36:22.000000 mpl_ascii-0.6.2/mpl_ascii.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:36:22.000000 mpl_ascii-0.6.2/mpl_ascii.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 13:36:22.000000 mpl_ascii-0.6.2/mpl_ascii.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 13:36:22.000000 mpl_ascii-0.6.2/mpl_ascii.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:36:22.713123 mpl_ascii-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:36:22.709123 mpl_ascii-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/tests/test_overlay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:57:56.727309 mpl_ascii-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:57:56.711309 mpl_ascii-0.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:57:56.715309 mpl_ascii-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-24 16:57:56.727309 mpl_ascii-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:57:56.723309 mpl_ascii-0.6.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_chart.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_stacked.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/barh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/barh.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/box_plot_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/box_plot_basic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/broken_line_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/broken_line_plot.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/categorical_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/categorical_variables.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/cohere.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/color_bar_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/color_bar_scatter.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/csd_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/csd_demo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/double_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/double_plot.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/errorbars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/errorbars.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/errorbars_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/errorbars_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/errorbars_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/errorbars_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/errorbars_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/errorbars_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/hist_best_fit_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/hist_best_fit_line.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/hist_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/hist_simple.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/hist_simple_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/hist_simple_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/line_markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38794 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/line_markers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/lines_multi_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/lines_multi_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/scatter_multi_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/scatter_multi_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/simple_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/simple_plot.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/violin_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/violin_plot.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:57:56.727309 mpl_ascii-0.6.3/mpl_ascii/
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/ascii_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/ax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/color_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/legend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/poly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:57:56.727309 mpl_ascii-0.6.3/mpl_ascii.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-24 16:57:56.000000 mpl_ascii-0.6.3/mpl_ascii.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-24 16:57:56.000000 mpl_ascii-0.6.3/mpl_ascii.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:57:56.000000 mpl_ascii-0.6.3/mpl_ascii.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-24 16:57:56.000000 mpl_ascii-0.6.3/mpl_ascii.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 16:57:56.000000 mpl_ascii-0.6.3/mpl_ascii.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 16:57:56.727309 mpl_ascii-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:57:56.727309 mpl_ascii-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/tests/test_overlay.py
```

### Comparing `mpl_ascii-0.6.2/.github/workflows/python-package.yml` & `mpl_ascii-0.6.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/.gitignore` & `mpl_ascii-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/CHANGELOG.md` & `mpl_ascii-0.6.3/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,23 @@
 
 ### Added
 
 - Add support for colour bars on scatter plots.
 - Add support for contour plots without colors.
 - Add support for text objects in plot.
 
+## [0.6.3] 2024-05-24
+
+### Fixed
+
+- Line plots now handle None values as matplotlib does. If a `None` value is passed into a line plot then it has line break.
+
 ## [0.6.2] 2024-05-19
 
-## Fixed
+### Fixed
 
 - `mpl_ascii` is now compatible with matplotlib 3.9.
 
 ## [0.6.1] 2024-05-11
 
 ### Fixed
```

### Comparing `mpl_ascii-0.6.2/LICENSE` & `mpl_ascii-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/Makefile` & `mpl_ascii-0.6.3/Makefile`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/PKG-INFO` & `mpl_ascii-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_ascii
-Version: 0.6.2
+Version: 0.6.3
 Summary: A matplotlib backend that produces plots using only ASCII characters
 Author: Chris Cave
 Maintainer: Chris Cave
 License: MIT License
 Project-URL: Homepage, https://github.com/chriscave/mpl_ascii
 Keywords: matplotlib,plotting,ASCII
 Requires-Python: >=3.7
```

### Comparing `mpl_ascii-0.6.2/README.md` & `mpl_ascii-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/bar_chart.py` & `mpl_ascii-0.6.3/examples/bar_chart.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/bar_chart.txt` & `mpl_ascii-0.6.3/examples/bar_chart.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/bar_color.py` & `mpl_ascii-0.6.3/examples/bar_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/bar_color.txt` & `mpl_ascii-0.6.3/examples/bar_color.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/bar_label_1.py` & `mpl_ascii-0.6.3/examples/bar_label_1.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/bar_label_1.txt` & `mpl_ascii-0.6.3/examples/bar_label_1.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/bar_label_2.py` & `mpl_ascii-0.6.3/examples/bar_label_2.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/bar_label_2.txt` & `mpl_ascii-0.6.3/examples/bar_label_2.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/bar_label_3.py` & `mpl_ascii-0.6.3/examples/bar_label_3.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/bar_label_3.txt` & `mpl_ascii-0.6.3/examples/bar_label_3.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/bar_label_4.py` & `mpl_ascii-0.6.3/examples/bar_label_4.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/bar_label_4.txt` & `mpl_ascii-0.6.3/examples/bar_label_4.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/bar_label_5.py` & `mpl_ascii-0.6.3/examples/bar_label_5.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/bar_label_5.txt` & `mpl_ascii-0.6.3/examples/bar_label_5.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/bar_stacked.py` & `mpl_ascii-0.6.3/examples/bar_stacked.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/bar_stacked.txt` & `mpl_ascii-0.6.3/examples/bar_stacked.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/barh.py` & `mpl_ascii-0.6.3/examples/barh.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/barh.txt` & `mpl_ascii-0.6.3/examples/barh.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/box_plot_basic.py` & `mpl_ascii-0.6.3/examples/box_plot_basic.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/box_plot_basic.txt` & `mpl_ascii-0.6.3/examples/box_plot_basic.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/categorical_variables.py` & `mpl_ascii-0.6.3/examples/categorical_variables.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/categorical_variables.txt` & `mpl_ascii-0.6.3/examples/categorical_variables.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/cohere.py` & `mpl_ascii-0.6.3/examples/cohere.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/cohere.txt` & `mpl_ascii-0.6.3/examples/cohere.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/color_bar_scatter.py` & `mpl_ascii-0.6.3/examples/color_bar_scatter.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/csd_demo.py` & `mpl_ascii-0.6.3/examples/csd_demo.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/csd_demo.txt` & `mpl_ascii-0.6.3/examples/csd_demo.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/double_plot.py` & `mpl_ascii-0.6.3/examples/double_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/double_plot.txt` & `mpl_ascii-0.6.3/examples/double_plot.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/errorbars.txt` & `mpl_ascii-0.6.3/examples/errorbars.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/errorbars_2.py` & `mpl_ascii-0.6.3/examples/errorbars_2.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/errorbars_2.txt` & `mpl_ascii-0.6.3/examples/errorbars_2.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/errorbars_3.py` & `mpl_ascii-0.6.3/examples/errorbars_3.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/errorbars_3.txt` & `mpl_ascii-0.6.3/examples/errorbars_3.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/errorbars_4.py` & `mpl_ascii-0.6.3/examples/errorbars_4.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/errorbars_4.txt` & `mpl_ascii-0.6.3/examples/errorbars_4.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/hist_best_fit_line.py` & `mpl_ascii-0.6.3/examples/hist_best_fit_line.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/hist_best_fit_line.txt` & `mpl_ascii-0.6.3/examples/hist_best_fit_line.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/hist_simple.py` & `mpl_ascii-0.6.3/examples/hist_simple.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/hist_simple.txt` & `mpl_ascii-0.6.3/examples/hist_simple.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/hist_simple_colors.py` & `mpl_ascii-0.6.3/examples/hist_simple_colors.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/hist_simple_colors.txt` & `mpl_ascii-0.6.3/examples/hist_simple_colors.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/line_markers.py` & `mpl_ascii-0.6.3/examples/line_markers.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/line_markers.txt` & `mpl_ascii-0.6.3/examples/line_markers.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/lines_multi_color.py` & `mpl_ascii-0.6.3/examples/lines_multi_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/lines_multi_color.txt` & `mpl_ascii-0.6.3/examples/lines_multi_color.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/scatter_multi_color.py` & `mpl_ascii-0.6.3/examples/scatter_multi_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/scatter_multi_color.txt` & `mpl_ascii-0.6.3/examples/scatter_multi_color.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/simple_plot.py` & `mpl_ascii-0.6.3/examples/simple_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/simple_plot.txt` & `mpl_ascii-0.6.3/examples/simple_plot.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/violin_plot.py` & `mpl_ascii-0.6.3/examples/violin_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/examples/violin_plot.txt` & `mpl_ascii-0.6.3/examples/violin_plot.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/mpl_ascii/ascii_canvas.py` & `mpl_ascii-0.6.3/mpl_ascii/ascii_canvas.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/mpl_ascii/color_map.py` & `mpl_ascii-0.6.3/mpl_ascii/color_map.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from typing import Dict
-import matplotlib
 from matplotlib.axes import Axes
-from matplotlib.collections import LineCollection, PathCollection, PolyCollection, QuadMesh
-from matplotlib.container import BarContainer
+from matplotlib.collections import PathCollection, QuadMesh
 from matplotlib.figure import Figure
-from matplotlib.patches import Rectangle
+
+from mpl_ascii.bar import get_bars
+from mpl_ascii.color import Char, std_color
+from mpl_ascii.line import get_lines_plots
+from mpl_ascii.poly import get_violin_plots
+from mpl_ascii.scatter import get_scatter_plots
 
 
 bar_chars = [
     "#",
     "%",
     "&",
     "@",
@@ -38,25 +41,14 @@
     "v",
     "z",
     "s",
     "i",
     "n",
 ]
 
-class Char:
-    def __init__(self, character: str, color: str) -> None:
-        self.character=character
-        self.color=color
-
-    def __str__(self) -> str:
-        return self.character
-
-
-    def __rich__(self) -> str:
-        return f"[{self.color}]{self.character}[/{self.color}]"
 
 class FigureColorMap:
     def __init__(self, figure: Figure) -> None:
         self.figure = figure
 
     def associate_color_bar(self, ax):
         ax_idx = self.figure.axes.index(ax)
@@ -106,69 +98,59 @@
         index = 0
         while True:
             yield ls[index]
             index = (index + 1) % len(ls)
 
     gen = ascii_chars(bar_chars)
     color_to_ascii = {}
-    for container in ax.containers:
-        if not isinstance(container, BarContainer):
+    bars = get_bars(ax)
+    for bar in bars:
+        color = std_color(bar.get_facecolor())
+        if color in color_to_ascii:
             continue
-        for bar in container.patches:
-            if not isinstance(bar, Rectangle):
-                continue
-            color = std_color(bar.get_facecolor())
-            if color in color_to_ascii:
-                continue
-            color_to_ascii[color] = Char(next(gen), color)
+        color_to_ascii[color] = Char(next(gen), color)
 
     gen = ascii_chars(bar_chars)
     for container in ax.collections:
         if not isinstance(container, QuadMesh):
             continue
         tick_data = [tick.get_loc() for tick in ax.yaxis.get_major_ticks()]
         cmap, norm = container.cmap, container.norm
         for td in tick_data:
             color = std_color(cmap(norm(td)))
             if color in color_to_ascii:
                 continue
             color_to_ascii[color] = Char(next(gen), color)
 
-    lines = ax.get_lines()
     gen = ascii_chars(line_chars)
+    lines = get_lines_plots(ax)
     for line in lines:
         color = std_color(line.get_color())
         if color in color_to_ascii:
             continue
         color_to_ascii[color] = Char(next(gen), color)
 
-    for collection in ax.collections:
-        if isinstance(collection, PolyCollection):
-            for color in collection.get_facecolor():
-                color = std_color(tuple(color.tolist()))
-                if color in color_to_ascii:
-                    continue
-                color_to_ascii[color] = Char(next(gen), color)
-
-        if isinstance(collection, LineCollection):
-            for color in collection.get_color():
-                color = std_color(tuple(color.tolist()))
-                if color in color_to_ascii:
-                    continue
-                color_to_ascii[color] = Char(next(gen), color)
-
+    pcolls, linecolls = get_violin_plots(ax)
+    for collection in pcolls:
+        for color in collection.get_facecolor():
+            color = std_color(tuple(color.tolist()))
+            if color in color_to_ascii:
+                continue
+            color_to_ascii[color] = Char(next(gen), color)
 
+    for collection in linecolls:
+        for color in collection.get_color():
+            color = std_color(tuple(color.tolist()))
+            if color in color_to_ascii:
+                continue
+            color_to_ascii[color] = Char(next(gen), color)
 
     gen = ascii_chars(scatter_chars)
+    collection = get_scatter_plots(ax)
     for collection in ax.collections:
-        if not isinstance(collection, PathCollection):
-            continue
         for color in collection.get_facecolor():
             color = std_color(tuple(color.tolist()))
             if color in color_to_ascii:
                 continue
             color_to_ascii[color] = Char(next(gen), color)
 
     return color_to_ascii
-
-def std_color(color):
-    return matplotlib.colors.to_hex(color)
```

### Comparing `mpl_ascii-0.6.2/mpl_ascii/overlay.py` & `mpl_ascii-0.6.3/mpl_ascii/overlay.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/mpl_ascii.egg-info/PKG-INFO` & `mpl_ascii-0.6.3/mpl_ascii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_ascii
-Version: 0.6.2
+Version: 0.6.3
 Summary: A matplotlib backend that produces plots using only ASCII characters
 Author: Chris Cave
 Maintainer: Chris Cave
 License: MIT License
 Project-URL: Homepage, https://github.com/chriscave/mpl_ascii
 Keywords: matplotlib,plotting,ASCII
 Requires-Python: >=3.7
```

### Comparing `mpl_ascii-0.6.2/mpl_ascii.egg-info/SOURCES.txt` & `mpl_ascii-0.6.3/mpl_ascii.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 examples/bar_label_5.txt
 examples/bar_stacked.py
 examples/bar_stacked.txt
 examples/barh.py
 examples/barh.txt
 examples/box_plot_basic.py
 examples/box_plot_basic.txt
+examples/broken_line_plot.py
+examples/broken_line_plot.txt
 examples/categorical_variables.py
 examples/categorical_variables.txt
 examples/cohere.py
 examples/cohere.txt
 examples/color_bar_scatter.py
 examples/color_bar_scatter.txt
 examples/csd_demo.py
@@ -58,17 +60,26 @@
 examples/scatter_multi_color.txt
 examples/simple_plot.py
 examples/simple_plot.txt
 examples/violin_plot.py
 examples/violin_plot.txt
 mpl_ascii/__init__.py
 mpl_ascii/ascii_canvas.py
+mpl_ascii/ax.py
+mpl_ascii/bar.py
+mpl_ascii/color.py
 mpl_ascii/color_map.py
+mpl_ascii/colorbar.py
 mpl_ascii/draw.py
+mpl_ascii/format.py
+mpl_ascii/legend.py
+mpl_ascii/line.py
 mpl_ascii/overlay.py
+mpl_ascii/poly.py
+mpl_ascii/scatter.py
 mpl_ascii/tools.py
 mpl_ascii.egg-info/PKG-INFO
 mpl_ascii.egg-info/SOURCES.txt
 mpl_ascii.egg-info/dependency_links.txt
 mpl_ascii.egg-info/requires.txt
 mpl_ascii.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `mpl_ascii-0.6.2/pyproject.toml` & `mpl_ascii-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.2/tests/test_overlay.py` & `mpl_ascii-0.6.3/tests/test_overlay.py`

 * *Files identical despite different names*

