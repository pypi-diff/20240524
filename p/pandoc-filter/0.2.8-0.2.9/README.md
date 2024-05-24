# Comparing `tmp/pandoc-filter-0.2.8.tar.gz` & `tmp/pandoc-filter-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc-filter-0.2.8.tar", last modified: Sun Feb 25 06:37:00 2024, max compression
+gzip compressed data, was "pandoc-filter-0.2.9.tar", last modified: Sun Feb 25 09:16:00 2024, max compression
```

## Comparing `pandoc-filter-0.2.8.tar` & `pandoc-filter-0.2.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 06:37:00.732324 pandoc-filter-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16045 2024-02-25 06:37:00.732324 pandoc-filter-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 06:37:00.732324 pandoc-filter-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 06:37:00.728324 pandoc-filter-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 06:37:00.728324 pandoc-filter-0.2.8/src/pandoc_filter/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 06:37:00.732324 pandoc-filter-0.2.8/src/pandoc_filter/filters/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/filters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 06:37:00.732324 pandoc-filter-0.2.8/src/pandoc_filter/filters/md2html/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/filters/md2html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/filters/md2html/centralize_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/filters/md2html/enhance_link_like.py
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/filters/md2html/hash_anchor_and_internal_link.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 06:37:00.732324 pandoc-filter-0.2.8/src/pandoc_filter/filters/md2md/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/filters/md2md/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/filters/md2md/convert_github_style_alert_to_hexo_style_alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/filters/md2md/enhance_equation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/filters/md2md/norm_footnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/filters/md2md/norm_internal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/filters/md2md/upload_figure_to_aliyun.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 06:37:00.732324 pandoc-filter-0.2.8/src/pandoc_filter/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/utils/hash_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/utils/html_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/utils/logging_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/utils/oss_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/utils/pandoc_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/utils/panflute_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/src/pandoc_filter/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 06:37:00.732324 pandoc-filter-0.2.8/src/pandoc_filter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16045 2024-02-25 06:37:00.000000 pandoc-filter-0.2.8/src/pandoc_filter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-02-25 06:37:00.000000 pandoc-filter-0.2.8/src/pandoc_filter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 06:37:00.000000 pandoc-filter-0.2.8/src/pandoc_filter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-25 06:37:00.000000 pandoc-filter-0.2.8/src/pandoc_filter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-25 06:37:00.000000 pandoc-filter-0.2.8/src/pandoc_filter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-25 06:37:00.000000 pandoc-filter-0.2.8/src/pandoc_filter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 06:37:00.732324 pandoc-filter-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/tests/test_md2html_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-02-25 06:35:38.000000 pandoc-filter-0.2.8/tests/test_md2md_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 09:16:00.319913 pandoc-filter-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-02-25 09:16:00.319913 pandoc-filter-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 09:16:00.319913 pandoc-filter-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 09:16:00.311912 pandoc-filter-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 09:16:00.311912 pandoc-filter-0.2.9/src/pandoc_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 09:16:00.315912 pandoc-filter-0.2.9/src/pandoc_filter/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/filters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 09:16:00.315912 pandoc-filter-0.2.9/src/pandoc_filter/filters/md2html/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/filters/md2html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/filters/md2html/centralize_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/filters/md2html/enhance_link_like.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/filters/md2html/hash_anchor_and_internal_link.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 09:16:00.315912 pandoc-filter-0.2.9/src/pandoc_filter/filters/md2md/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/filters/md2md/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/filters/md2md/convert_github_style_alert_to_hexo_style_alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/filters/md2md/enhance_equation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/filters/md2md/norm_footnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/filters/md2md/norm_internal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/filters/md2md/upload_figure_to_aliyun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 09:16:00.315912 pandoc-filter-0.2.9/src/pandoc_filter/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/utils/hash_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/utils/html_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/utils/logging_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/utils/oss_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/utils/pandoc_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/utils/panflute_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/src/pandoc_filter/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 09:16:00.315912 pandoc-filter-0.2.9/src/pandoc_filter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-02-25 09:16:00.000000 pandoc-filter-0.2.9/src/pandoc_filter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-02-25 09:16:00.000000 pandoc-filter-0.2.9/src/pandoc_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 09:16:00.000000 pandoc-filter-0.2.9/src/pandoc_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-25 09:16:00.000000 pandoc-filter-0.2.9/src/pandoc_filter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-25 09:16:00.000000 pandoc-filter-0.2.9/src/pandoc_filter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-25 09:16:00.000000 pandoc-filter-0.2.9/src/pandoc_filter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 09:16:00.315912 pandoc-filter-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/tests/test_md2html_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-02-25 09:14:44.000000 pandoc-filter-0.2.9/tests/test_md2md_filters.py
```

### Comparing `pandoc-filter-0.2.8/LICENSE` & `pandoc-filter-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/pyproject.toml` & `pandoc-filter-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter/__init__.py` & `pandoc-filter-0.2.9/src/pandoc_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter/filters/md2html/centralize_figure.py` & `pandoc-filter-0.2.9/src/pandoc_filter/filters/md2html/centralize_figure.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter/filters/md2html/enhance_link_like.py` & `pandoc-filter-0.2.9/src/pandoc_filter/filters/md2html/enhance_link_like.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter/filters/md2html/hash_anchor_and_internal_link.py` & `pandoc-filter-0.2.9/src/pandoc_filter/filters/md2html/hash_anchor_and_internal_link.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter/filters/md2md/convert_github_style_alert_to_hexo_style_alert.py` & `pandoc-filter-0.2.9/src/pandoc_filter/filters/md2md/convert_github_style_alert_to_hexo_style_alert.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter/filters/md2md/enhance_equation.py` & `pandoc-filter-0.2.9/src/pandoc_filter/filters/md2md/enhance_equation.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter/filters/md2md/norm_footnote.py` & `pandoc-filter-0.2.9/src/pandoc_filter/filters/md2md/norm_footnote.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter/filters/md2md/norm_internal_link.py` & `pandoc-filter-0.2.9/src/pandoc_filter/filters/md2md/norm_internal_link.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter/filters/md2md/upload_figure_to_aliyun.py` & `pandoc-filter-0.2.9/src/pandoc_filter/filters/md2md/upload_figure_to_aliyun.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter/scripts.py` & `pandoc-filter-0.2.9/src/pandoc_filter/scripts.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter/utils/hash_helper.py` & `pandoc-filter-0.2.9/src/pandoc_filter/utils/hash_helper.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter/utils/html_helper.py` & `pandoc-filter-0.2.9/src/pandoc_filter/utils/html_helper.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter/utils/logging_helper.py` & `pandoc-filter-0.2.9/src/pandoc_filter/utils/logging_helper.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter/utils/oss_helper.py` & `pandoc-filter-0.2.9/src/pandoc_filter/utils/oss_helper.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter/utils/pandoc_helper.py` & `pandoc-filter-0.2.9/src/pandoc_filter/utils/pandoc_helper.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter/utils/panflute_helper.py` & `pandoc-filter-0.2.9/src/pandoc_filter/utils/panflute_helper.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter.egg-info/SOURCES.txt` & `pandoc-filter-0.2.9/src/pandoc_filter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/src/pandoc_filter.egg-info/entry_points.txt` & `pandoc-filter-0.2.9/src/pandoc_filter.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/tests/test_md2html_filters.py` & `pandoc-filter-0.2.9/tests/test_md2html_filters.py`

 * *Files identical despite different names*

### Comparing `pandoc-filter-0.2.8/tests/test_md2md_filters.py` & `pandoc-filter-0.2.9/tests/test_md2md_filters.py`

 * *Files identical despite different names*

