# Comparing `tmp/mdformat_gfm_alerts-1.0.0.tar.gz` & `tmp/mdformat_gfm_alerts-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdformat_gfm_alerts-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mdformat_gfm_alerts-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mdformat_gfm_alerts-1.0.0.tar` & `mdformat_gfm_alerts-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      612 2024-05-20 13:06:11.288616 mdformat_gfm_alerts-1.0.0/.copier-answers.yml
--rw-r--r--   0        0        0     1819 2024-05-20 13:06:11.288616 mdformat_gfm_alerts-1.0.0/.gitignore
--rw-r--r--   0        0        0     1592 2024-05-20 13:06:11.288616 mdformat_gfm_alerts-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      295 2024-05-20 13:06:11.288616 mdformat_gfm_alerts-1.0.0/.pre-commit-test.yaml
--rw-r--r--   0        0        0     2886 2024-05-20 13:06:11.288616 mdformat_gfm_alerts-1.0.0/.ruff.toml
--rw-r--r--   0        0        0       21 2024-05-20 13:06:11.288616 mdformat_gfm_alerts-1.0.0/.tool-versions
--rw-r--r--   0        0        0      276 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/.yamllint.yaml
--rw-r--r--   0        0        0     1370 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1073 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/LICENSE
--rw-r--r--   0        0        0     2741 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/README.md
--rw-r--r--   0        0        0      110 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/__init__.py
--rw-r--r--   0        0        0      149 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/factories/__init__.py
--rw-r--r--   0        0        0     3185 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/factories/_gfm_blockquote_factories.py
--rw-r--r--   0        0        0       88 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/mdit_plugins/__init__.py
--rw-r--r--   0        0        0     3002 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/mdit_plugins/_gfm_alerts.py
--rw-r--r--   0        0        0     1300 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/plugin.py
--rw-r--r--   0        0        0     1200 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      751 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/tox.ini
--rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 mdformat_gfm_alerts-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      612 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/.copier-answers.yml
+-rw-r--r--   0        0        0     1819 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1592 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      295 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/.pre-commit-test.yaml
+-rw-r--r--   0        0        0     2886 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/.ruff.toml
+-rw-r--r--   0        0        0       21 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/.tool-versions
+-rw-r--r--   0        0        0      276 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/.yamllint.yaml
+-rw-r--r--   0        0        0     1370 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1073 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2741 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/README.md
+-rw-r--r--   0        0        0      110 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/mdformat_gfm_alerts/__init__.py
+-rw-r--r--   0        0        0      149 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/mdformat_gfm_alerts/factories/__init__.py
+-rw-r--r--   0        0        0     3185 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/mdformat_gfm_alerts/factories/_gfm_blockquote_factories.py
+-rw-r--r--   0        0        0       88 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/mdformat_gfm_alerts/mdit_plugins/__init__.py
+-rw-r--r--   0        0        0     3030 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/mdformat_gfm_alerts/mdit_plugins/_gfm_alerts.py
+-rw-r--r--   0        0        0     1300 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/mdformat_gfm_alerts/plugin.py
+-rw-r--r--   0        0        0     1200 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      751 2024-05-24 01:15:57.608119 mdformat_gfm_alerts-1.0.1/tox.ini
+-rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 mdformat_gfm_alerts-1.0.1/PKG-INFO
```

### Comparing `mdformat_gfm_alerts-1.0.0/.copier-answers.yml` & `mdformat_gfm_alerts-1.0.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `mdformat_gfm_alerts-1.0.0/.gitignore` & `mdformat_gfm_alerts-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mdformat_gfm_alerts-1.0.0/.pre-commit-config.yaml` & `mdformat_gfm_alerts-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mdformat_gfm_alerts-1.0.0/.ruff.toml` & `mdformat_gfm_alerts-1.0.1/.ruff.toml`

 * *Files identical despite different names*

### Comparing `mdformat_gfm_alerts-1.0.0/CONTRIBUTING.md` & `mdformat_gfm_alerts-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mdformat_gfm_alerts-1.0.0/LICENSE` & `mdformat_gfm_alerts-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mdformat_gfm_alerts-1.0.0/README.md` & `mdformat_gfm_alerts-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/factories/_gfm_blockquote_factories.py` & `mdformat_gfm_alerts-1.0.1/mdformat_gfm_alerts/factories/_gfm_blockquote_factories.py`

 * *Files identical despite different names*

### Comparing `mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/mdit_plugins/_gfm_alerts.py` & `mdformat_gfm_alerts-1.0.1/mdformat_gfm_alerts/mdit_plugins/_gfm_alerts.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 GFM_ALERTS_PREFIX = "gfm_alert"
 """Prefix used to differentiate the parsed output."""
 
 INLINE_SEP = "\n\n"
 """Separator to differentiate the title and inline content (if present)."""
 
 PATTERNS = {
-    # Note '> ' prefix is removed when parsing
-    r"^\*\*(?P<title>Note|Warning)\*\*",
+    # Note '> ' prefix is removed when parsing and trailing ":" if found
+    r"^\*\*(?P<title>Note|Warning)\*\*:?",
     # FYI: This is intentionally strict. Keep in sync with supported titles
     r"^\\?\[!(?P<title>NOTE|TIP|IMPORTANT|WARNING|CAUTION)\\?\]",
 }
 """Patterns specific to GitHub Alerts."""
 
 
 def format_gfm_alerts_markup(
```

### Comparing `mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/plugin.py` & `mdformat_gfm_alerts-1.0.1/mdformat_gfm_alerts/plugin.py`

 * *Files identical despite different names*

### Comparing `mdformat_gfm_alerts-1.0.0/pyproject.toml` & `mdformat_gfm_alerts-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mdformat_gfm_alerts-1.0.0/tox.ini` & `mdformat_gfm_alerts-1.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `mdformat_gfm_alerts-1.0.0/PKG-INFO` & `mdformat_gfm_alerts-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdformat_gfm_alerts
-Version: 1.0.0
+Version: 1.0.1
 Summary: An mdformat plugin for `gfm_alerts`.
 Keywords: markdown,markdown-it,mdformat
 Author-email: kyleking <dev.act.kyle@gmail.com>
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

