# Comparing `tmp/cefi-4.7.0.tar.gz` & `tmp/cefi-4.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefi-4.7.0.tar", max compression
+gzip compressed data, was "cefi-4.7.1.tar", max compression
```

## Comparing `cefi-4.7.0.tar` & `cefi-4.7.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2024-04-28 14:49:54.464340 cefi-4.7.0/LICENSE
--rw-r--r--   0        0        0     2661 2024-04-28 14:49:54.464340 cefi-4.7.0/README.md
--rw-r--r--   0        0        0       87 2024-04-28 14:50:33.680206 cefi-4.7.0/cefi/__init__.py
--rw-r--r--   0        0        0      439 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/config.py
--rw-r--r--   0        0        0     3617 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/default_settings.toml
--rw-r--r--   0        0        0      158 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/handler/__init__.py
--rw-r--r--   0        0        0    13356 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/handler/capitalcom.py
--rw-r--r--   0        0        0     5517 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/handler/ccxt.py
--rw-r--r--   0        0        0     9225 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/handler/client.py
--rw-r--r--   0        0        0     1938 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/handler/ctrader.py
--rw-r--r--   0        0        0     7006 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/handler/ib_sync.py
--rw-r--r--   0        0        0     8586 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/main.py
--rw-r--r--   0        0        0     3782 2024-04-28 14:50:33.680206 cefi-4.7.0/pyproject.toml
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-24 10:37:04.958595 cefi-4.7.1/LICENSE
+-rw-r--r--   0        0        0     2661 2024-05-24 10:37:04.958595 cefi-4.7.1/README.md
+-rw-r--r--   0        0        0       87 2024-05-24 10:37:48.010424 cefi-4.7.1/cefi/__init__.py
+-rw-r--r--   0        0        0      439 2024-05-24 10:37:04.958595 cefi-4.7.1/cefi/config.py
+-rw-r--r--   0        0        0     3617 2024-05-24 10:37:04.958595 cefi-4.7.1/cefi/default_settings.toml
+-rw-r--r--   0        0        0      158 2024-05-24 10:37:04.958595 cefi-4.7.1/cefi/handler/__init__.py
+-rw-r--r--   0        0        0    13356 2024-05-24 10:37:04.958595 cefi-4.7.1/cefi/handler/capitalcom.py
+-rw-r--r--   0        0        0     5517 2024-05-24 10:37:04.958595 cefi-4.7.1/cefi/handler/ccxt.py
+-rw-r--r--   0        0        0     9225 2024-05-24 10:37:04.958595 cefi-4.7.1/cefi/handler/client.py
+-rw-r--r--   0        0        0     1938 2024-05-24 10:37:04.958595 cefi-4.7.1/cefi/handler/ctrader.py
+-rw-r--r--   0        0        0     7006 2024-05-24 10:37:04.958595 cefi-4.7.1/cefi/handler/ib_sync.py
+-rw-r--r--   0        0        0     8586 2024-05-24 10:37:04.958595 cefi-4.7.1/cefi/main.py
+-rw-r--r--   0        0        0     3782 2024-05-24 10:37:48.010424 cefi-4.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.7.1/PKG-INFO
```

### Comparing `cefi-4.7.0/LICENSE` & `cefi-4.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cefi-4.7.0/README.md` & `cefi-4.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cefi-4.7.0/cefi/default_settings.toml` & `cefi-4.7.1/cefi/default_settings.toml`

 * *Files identical despite different names*

### Comparing `cefi-4.7.0/cefi/handler/capitalcom.py` & `cefi-4.7.1/cefi/handler/capitalcom.py`

 * *Files identical despite different names*

### Comparing `cefi-4.7.0/cefi/handler/ccxt.py` & `cefi-4.7.1/cefi/handler/ccxt.py`

 * *Files identical despite different names*

### Comparing `cefi-4.7.0/cefi/handler/client.py` & `cefi-4.7.1/cefi/handler/client.py`

 * *Files identical despite different names*

### Comparing `cefi-4.7.0/cefi/handler/ctrader.py` & `cefi-4.7.1/cefi/handler/ctrader.py`

 * *Files identical despite different names*

### Comparing `cefi-4.7.0/cefi/handler/ib_sync.py` & `cefi-4.7.1/cefi/handler/ib_sync.py`

 * *Files identical despite different names*

### Comparing `cefi-4.7.0/cefi/main.py` & `cefi-4.7.1/cefi/main.py`

 * *Files identical despite different names*

### Comparing `cefi-4.7.0/pyproject.toml` & `cefi-4.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "cefi"
-version = "4.7.0"
+version = "4.7.1"
 description = "A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)"
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["cex, cefi, crypto, exchange, broker"]
 packages = [
     {include = "cefi"}
@@ -293,16 +293,16 @@
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "7.3.7"
 pydata-sphinx-theme = "^0.15.0"
 sphinx-hoverxref = "^1.3.0"
 sphinx_copybutton = "0.5.2"
-myst_parser = "^2.0.0"
-sphinx_design = "^0.5.0"
+myst_parser = "^3.0.0"
+sphinx_design = "^0.6.0"
 
 
 
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
```

### Comparing `cefi-4.7.0/PKG-INFO` & `cefi-4.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefi
-Version: 4.7.0
+Version: 4.7.1
 Summary: A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT
 Keywords: cex, cefi, crypto, exchange, broker
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cefi Version: 4.7.0 Summary: A python library, to
+Metadata-Version: 2.1 Name: cefi Version: 4.7.1 Summary: A python library, to
 interact with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT Keywords: cex, cefi, crypto, exchange, broker Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: capitalcom-python
```

