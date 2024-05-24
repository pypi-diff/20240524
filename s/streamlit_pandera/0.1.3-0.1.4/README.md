# Comparing `tmp/streamlit_pandera-0.1.3.tar.gz` & `tmp/streamlit_pandera-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_pandera-0.1.3.tar", max compression
+gzip compressed data, was "streamlit_pandera-0.1.4.tar", max compression
```

## Comparing `streamlit_pandera-0.1.3.tar` & `streamlit_pandera-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2024-05-24 03:15:41.420059 streamlit_pandera-0.1.3/LICENSE
--rw-r--r--   0        0        0     2390 2024-05-24 03:15:41.420059 streamlit_pandera-0.1.3/README.md
--rw-r--r--   0        0        0     1226 2024-05-24 03:15:41.424059 streamlit_pandera-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      221 2024-05-24 03:15:41.424059 streamlit_pandera-0.1.3/streamlit_pandera/Home.py
--rw-r--r--   0        0        0        0 2024-05-24 03:15:41.424059 streamlit_pandera-0.1.3/streamlit_pandera/__init__.py
--rw-r--r--   0        0        0     1272 2024-05-24 03:16:09.308227 streamlit_pandera-0.1.3/streamlit_pandera/pages/0_Instructions.py
--rw-r--r--   0        0        0     2900 2024-05-24 03:16:09.336227 streamlit_pandera-0.1.3/streamlit_pandera/validate_file.py
--rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 streamlit_pandera-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-24 04:34:40.348513 streamlit_pandera-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2405 2024-05-24 04:34:40.348513 streamlit_pandera-0.1.4/README.md
+-rw-r--r--   0        0        0     1226 2024-05-24 04:34:40.348513 streamlit_pandera-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      383 2024-05-24 04:35:02.980533 streamlit_pandera-0.1.4/streamlit_pandera/Home.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:34:40.348513 streamlit_pandera-0.1.4/streamlit_pandera/__init__.py
+-rw-r--r--   0        0        0     1272 2024-05-24 04:35:02.992533 streamlit_pandera-0.1.4/streamlit_pandera/pages/0_Instructions.py
+-rw-r--r--   0        0        0     2345 2024-05-24 04:35:03.016533 streamlit_pandera-0.1.4/streamlit_pandera/validate_file.py
+-rw-r--r--   0        0        0     3343 1970-01-01 00:00:00.000000 streamlit_pandera-0.1.4/PKG-INFO
```

### Comparing `streamlit_pandera-0.1.3/LICENSE` & `streamlit_pandera-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_pandera-0.1.3/README.md` & `streamlit_pandera-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 poetry run pytest e2e
 ```
 
 ## Run the App
 Ready to see streamlit-pandera in action? Simply run the following command:
 
 ```bash
-poetry run streamlit run app/run.py
+poetry run streamlit run streamlit_pandera/Home.py
 ```
 
 ## Contributions
 We welcome contributions from the community! If you have any ideas, bug fixes, or enhancements, feel free to submit a pull request.
 
 ## Feedback
 We'd love to hear your feedback! Whether you have suggestions for improvement or just want to share your experience using streamlit-pandera, don't hesitate to reach out.
```

### Comparing `streamlit_pandera-0.1.3/pyproject.toml` & `streamlit_pandera-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamlit_pandera"
-version = "0.1.3"
+version = "0.1.4"
 description = "Streamlit Data Validator Tool helps you validate your data with a plethora of formats"
 authors = ["Manrique Vargas <machomaxg@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 streamlit = "^1.34.0"
```

### Comparing `streamlit_pandera-0.1.3/streamlit_pandera/pages/0_Instructions.py` & `streamlit_pandera-0.1.4/streamlit_pandera/pages/0_Instructions.py`

 * *Files identical despite different names*

### Comparing `streamlit_pandera-0.1.3/PKG-INFO` & `streamlit_pandera-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_pandera
-Version: 0.1.3
+Version: 0.1.4
 Summary: Streamlit Data Validator Tool helps you validate your data with a plethora of formats
 Author: Manrique Vargas
 Author-email: machomaxg@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -84,15 +84,15 @@
 poetry run pytest e2e
 ```
 
 ## Run the App
 Ready to see streamlit-pandera in action? Simply run the following command:
 
 ```bash
-poetry run streamlit run app/run.py
+poetry run streamlit run streamlit_pandera/Home.py
 ```
 
 ## Contributions
 We welcome contributions from the community! If you have any ideas, bug fixes, or enhancements, feel free to submit a pull request.
 
 ## Feedback
 We'd love to hear your feedback! Whether you have suggestions for improvement or just want to share your experience using streamlit-pandera, don't hesitate to reach out.
```

