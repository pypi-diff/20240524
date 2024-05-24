# Comparing `tmp/breach_check-0.2.0.tar.gz` & `tmp/breach_check-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breach_check-0.2.0.tar", max compression
+gzip compressed data, was "breach_check-0.3.0.tar", max compression
```

## Comparing `breach_check-0.2.0.tar` & `breach_check-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0     1071 2023-11-29 17:25:44.884756 breach_check-0.2.0/LICENSE
--rw-r--r--   0        0        0     4744 2023-11-29 17:25:44.884756 breach_check-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-11-29 17:25:44.884756 breach_check-0.2.0/breach_check/__init__.py
--rw-r--r--   0        0        0     1082 2023-11-29 17:25:44.884756 breach_check-0.2.0/breach_check/__main__.py
--rw-r--r--   0        0        0     4048 2023-11-29 17:25:44.884756 breach_check-0.2.0/breach_check/breach.py
--rw-r--r--   0        0        0     4108 2023-11-29 17:25:44.884756 breach_check-0.2.0/breach_check/http.py
--rw-r--r--   0        0        0      373 2023-11-29 17:25:44.884756 breach_check-0.2.0/breach_check/logger.py
--rw-r--r--   0        0        0     2566 2023-11-29 17:25:44.884756 breach_check-0.2.0/breach_check/results.py
--rw-r--r--   0        0        0     1212 2023-11-29 17:25:44.884756 breach_check-0.2.0/breach_check/utils.py
--rw-r--r--   0        0        0      780 2023-11-29 17:25:44.884756 breach_check-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5485 1970-01-01 00:00:00.000000 breach_check-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-24 19:19:58.079295 breach_check-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4744 2024-05-24 19:19:58.079295 breach_check-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 19:19:58.079295 breach_check-0.3.0/breach_check/__init__.py
+-rw-r--r--   0        0        0     1044 2024-05-24 19:19:58.079295 breach_check-0.3.0/breach_check/__main__.py
+-rw-r--r--   0        0        0     4823 2024-05-24 19:19:58.079295 breach_check-0.3.0/breach_check/breach.py
+-rw-r--r--   0        0        0        0 2024-05-24 19:19:58.079295 breach_check-0.3.0/breach_check/breach_factory/__init__.py
+-rw-r--r--   0        0        0      789 2024-05-24 19:19:58.079295 breach_check-0.3.0/breach_check/breach_factory/base.py
+-rw-r--r--   0        0        0     1869 2024-05-24 19:19:58.079295 breach_check-0.3.0/breach_check/breach_factory/leakcheck.py
+-rw-r--r--   0        0        0     1773 2024-05-24 19:19:58.079295 breach_check-0.3.0/breach_check/breach_factory/mozilla.py
+-rw-r--r--   0        0        0     5052 2024-05-24 19:19:58.079295 breach_check-0.3.0/breach_check/http.py
+-rw-r--r--   0        0        0      373 2024-05-24 19:19:58.079295 breach_check-0.3.0/breach_check/logger.py
+-rw-r--r--   0        0        0     2648 2024-05-24 19:19:58.079295 breach_check-0.3.0/breach_check/results.py
+-rw-r--r--   0        0        0     1212 2024-05-24 19:19:58.079295 breach_check-0.3.0/breach_check/utils.py
+-rw-r--r--   0        0        0      822 2024-05-24 19:19:58.079295 breach_check-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5569 1970-01-01 00:00:00.000000 breach_check-0.3.0/PKG-INFO
```

### Comparing `breach_check-0.2.0/LICENSE` & `breach_check-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `breach_check-0.2.0/README.md` & `breach_check-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `breach_check-0.2.0/breach_check/__main__.py` & `breach_check-0.3.0/breach_check/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
+from asyncio import run
 from argparse import ArgumentParser
 from breach_check.breach import BreachChecker
 from breach_check.results import Results
-from breach_check.utils import generate_unique_filename, extract_emails, write_json_file
-from asyncio import run
-from sys import exit
+from breach_check.utils import generate_unique_filename, extract_emails
 
 
 def main():
     parser = ArgumentParser('breach-check')
     parser.add_argument('-i', '--input', dest='input_file',
                         help='input file containing emails on each line', type=str, required=True)
     parser.add_argument('-o', '--output', dest='output_file',
```

### Comparing `breach_check-0.2.0/breach_check/results.py` & `breach_check-0.3.0/breach_check/results.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,21 +22,24 @@
     def generate_result_cols(self, results_list: list[dict]) -> list[Column]:
         return [Column(header=col_header, overflow='fold') for col_header in self.extract_result_table_cols(results_list)]
 
     def _represent_results(self, results: list):
         formatted_results = []
         for result in results:
             email = result.get('email')
-            breaches = filter(
+            breaches = list(filter(
                 lambda domain: domain.strip() if domain else '',
-                [breach.get('Domain', '').strip()
+                [breach.get('name', '').strip()
                  for breach in result.get('breaches')]
-            )
+            ))
             total = result.get('total')
 
+            if not breaches:
+                breaches = ['[green]-[/green]']
+
             formatted_result = {
                 'email': email,
                 'breaches': ','.join(breaches),
                 'total': total
             }
             formatted_results.append(formatted_result)
```

### Comparing `breach_check-0.2.0/breach_check/utils.py` & `breach_check-0.3.0/breach_check/utils.py`

 * *Files identical despite different names*

### Comparing `breach_check-0.2.0/pyproject.toml` & `breach_check-0.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [tool.poetry]
 name = "breach-check"
-version = "0.2.0"
+version = "0.3.0"
 description = "check for data breaches for provided emails"
 authors = ["Dhrumil Mistry <56185972+dmdhrumilmistry@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "^3.9.0"
 rich = "^13.7.0"
+aiolimiter = "^1.1.0"
+tenacity = "^8.3.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 
 [tool.poetry.urls]
 "Home" = "https://github.com/dmdhrumilmistry/breach-check"
 "Bug Tracker" = "https://github.com/dmdhrumilmistry/breach-check/issues"
```

### Comparing `breach_check-0.2.0/PKG-INFO` & `breach_check-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: breach-check
-Version: 0.2.0
+Version: 0.3.0
 Summary: check for data breaches for provided emails
 License: MIT
 Author: Dhrumil Mistry
 Author-email: 56185972+dmdhrumilmistry@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.0,<4.0.0)
+Requires-Dist: aiolimiter (>=1.1.0,<2.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
+Requires-Dist: tenacity (>=8.3.0,<9.0.0)
 Project-URL: Bug Tracker, https://github.com/dmdhrumilmistry/breach-check/issues
 Project-URL: Home, https://github.com/dmdhrumilmistry/breach-check
 Project-URL: PayPal, https://paypal.me/dmdhrumilmistry
 Project-URL: Support, https://github.com/sponsors/dmdhrumilmistry/
 Description-Content-Type: text/markdown
 
 # Breach Check
```

