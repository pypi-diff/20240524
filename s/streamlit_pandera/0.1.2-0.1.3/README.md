# Comparing `tmp/streamlit_pandera-0.1.2.tar.gz` & `tmp/streamlit_pandera-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_pandera-0.1.2.tar", max compression
+gzip compressed data, was "streamlit_pandera-0.1.3.tar", max compression
```

## Comparing `streamlit_pandera-0.1.2.tar` & `streamlit_pandera-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1063 2024-05-19 22:58:24.565899 streamlit_pandera-0.1.2/LICENSE
--rw-r--r--   0        0        0     2350 2024-05-19 22:58:24.565899 streamlit_pandera-0.1.2/README.md
--rw-r--r--   0        0        0     1243 2024-05-19 22:58:24.569899 streamlit_pandera-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 22:58:24.569899 streamlit_pandera-0.1.2/streamlit_pandera/__init__.py
--rw-r--r--   0        0        0     2873 2024-05-19 22:58:24.569899 streamlit_pandera-0.1.2/streamlit_pandera/validate_file.py
--rw-r--r--   0        0        0     3320 1970-01-01 00:00:00.000000 streamlit_pandera-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-24 03:15:41.420059 streamlit_pandera-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2390 2024-05-24 03:15:41.420059 streamlit_pandera-0.1.3/README.md
+-rw-r--r--   0        0        0     1226 2024-05-24 03:15:41.424059 streamlit_pandera-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      221 2024-05-24 03:15:41.424059 streamlit_pandera-0.1.3/streamlit_pandera/Home.py
+-rw-r--r--   0        0        0        0 2024-05-24 03:15:41.424059 streamlit_pandera-0.1.3/streamlit_pandera/__init__.py
+-rw-r--r--   0        0        0     1272 2024-05-24 03:16:09.308227 streamlit_pandera-0.1.3/streamlit_pandera/pages/0_Instructions.py
+-rw-r--r--   0        0        0     2900 2024-05-24 03:16:09.336227 streamlit_pandera-0.1.3/streamlit_pandera/validate_file.py
+-rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 streamlit_pandera-0.1.3/PKG-INFO
```

### Comparing `streamlit_pandera-0.1.2/LICENSE` & `streamlit_pandera-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_pandera-0.1.2/README.md` & `streamlit_pandera-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Welcome to Data Validator!
 
+[Go to App](https://pandera.streamlit.app)
 
-[![Test](https://github.com/resilientinfrastructure/streamlit-pandera/actions/workflows/e2e.yml/badge.svg)](https://github.com/resilientinfrastructure/streamlit-pandera/actions/workflows/e2e.yml)
+[![Release](https://github.com/resilientinfrastructure/streamlit-pandera/actions/workflows/publish_pypi.yml/badge.svg)](https://github.com/resilientinfrastructure/streamlit-pandera/actions/workflows/publish_pypi.yml)
 
 Data Validator is your go-to tool for clean data ingestion and validation, seamlessly integrating Streamlit and Panderas to make your data processing tasks a breeze.
 
 ## Features
 
 - **Easy Data Ingestion:** Select your file format (CSV or JSON) and provide a URL to a Panderas schema.
 - **Streamlined Validation:** With just a few clicks, submit your selections and validate your data effortlessly.
@@ -40,14 +41,15 @@
 ### Step 2: Provide Panderas Schema URL
 Enter the URL to the Panderas schema you want to use for validation. Don't worry, we support various schema sources to suit your needs.
 
 ### Step 3: Submit and Validate
 Hit that submit button and let streamlit-pandera work its magic! Your data will be validated against the specified schema in no time.
 
 
+
 [Go to Demo](https://youtu.be/9Ry_A9LgrbQ)
 
 [![Video](http://img.youtube.com/vi/9Ry_A9LgrbQ/0.jpg)](https://youtu.be/9Ry_A9LgrbQ)
 
 
 ## Run Tests
 To ensure everything is functioning smoothly, run the tests using the following commands:
@@ -58,15 +60,15 @@
 poetry run pytest e2e
 ```
 
 ## Run the App
 Ready to see streamlit-pandera in action? Simply run the following command:
 
 ```bash
-poetry run streamlit run streamlit_panderas/validate_file.py
+poetry run streamlit run app/run.py
 ```
 
 ## Contributions
 We welcome contributions from the community! If you have any ideas, bug fixes, or enhancements, feel free to submit a pull request.
 
 ## Feedback
 We'd love to hear your feedback! Whether you have suggestions for improvement or just want to share your experience using streamlit-pandera, don't hesitate to reach out.
```

### Comparing `streamlit_pandera-0.1.2/pyproject.toml` & `streamlit_pandera-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "streamlit_pandera"
-version = "0.1.2"
+version = "0.1.3"
 description = "Streamlit Data Validator Tool helps you validate your data with a plethora of formats"
 authors = ["Manrique Vargas <machomaxg@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 streamlit = "^1.34.0"
 validators = "^0.28.1"
 io_file_validator = "^0.1.3"
 pipx = "^1.5.0"
 cookiecutter = "^2.6.0"
 wheel = "*"
-pytest = "7.4.0"
 playwright = "1.39.0"
 requests = "2.31.0"
 pytest-playwright-snapshot = "1.0"
 pytest-rerunfailures = "12.0"
 pandera = { version = "^0.7.2", extras = ["io"] }
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `streamlit_pandera-0.1.2/streamlit_pandera/validate_file.py` & `streamlit_pandera-0.1.3/streamlit_pandera/validate_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         page_title="Data Validator Home",
         page_icon="📊",
     )
     supported_files = ["csv", "json"]
     if additional_supported_files and isinstance(additional_supported_files, list):
         supported_files.extend(additional_supported_files)
 
-    st.write("# Data Validation Tool! 📊")
+    st.write("# Data Validation Tool Using Pandera Yaml Schemas! 📊")
     set_selectbox(supported_files)
     set_format_type_form()
     if st.session_state["panderas_url"] is not None and st.session_state["file_format"] is not None:
         if st.session_state["file_format"] == "csv":
             validator.url = st.session_state["panderas_url"]
             validator.file_format = st.session_state["file_format"]
         elif st.session_state["file_format"] == "json":
```

### Comparing `streamlit_pandera-0.1.2/PKG-INFO` & `streamlit_pandera-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: streamlit_pandera
-Version: 0.1.2
+Version: 0.1.3
 Summary: Streamlit Data Validator Tool helps you validate your data with a plethora of formats
 Author: Manrique Vargas
 Author-email: machomaxg@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cookiecutter (>=2.6.0,<3.0.0)
 Requires-Dist: io_file_validator (>=0.1.3,<0.2.0)
 Requires-Dist: pandera[io] (>=0.7.2,<0.8.0)
 Requires-Dist: pipx (>=1.5.0,<2.0.0)
 Requires-Dist: playwright (==1.39.0)
-Requires-Dist: pytest (==7.4.0)
 Requires-Dist: pytest-playwright-snapshot (==1.0)
 Requires-Dist: pytest-rerunfailures (==12.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: streamlit (>=1.34.0,<2.0.0)
 Requires-Dist: validators (>=0.28.1,<0.29.0)
 Requires-Dist: wheel
 Description-Content-Type: text/markdown
 
 # Welcome to Data Validator!
 
+[Go to App](https://pandera.streamlit.app)
 
-[![Test](https://github.com/resilientinfrastructure/streamlit-pandera/actions/workflows/e2e.yml/badge.svg)](https://github.com/resilientinfrastructure/streamlit-pandera/actions/workflows/e2e.yml)
+[![Release](https://github.com/resilientinfrastructure/streamlit-pandera/actions/workflows/publish_pypi.yml/badge.svg)](https://github.com/resilientinfrastructure/streamlit-pandera/actions/workflows/publish_pypi.yml)
 
 Data Validator is your go-to tool for clean data ingestion and validation, seamlessly integrating Streamlit and Panderas to make your data processing tasks a breeze.
 
 ## Features
 
 - **Easy Data Ingestion:** Select your file format (CSV or JSON) and provide a URL to a Panderas schema.
 - **Streamlined Validation:** With just a few clicks, submit your selections and validate your data effortlessly.
@@ -65,14 +65,15 @@
 ### Step 2: Provide Panderas Schema URL
 Enter the URL to the Panderas schema you want to use for validation. Don't worry, we support various schema sources to suit your needs.
 
 ### Step 3: Submit and Validate
 Hit that submit button and let streamlit-pandera work its magic! Your data will be validated against the specified schema in no time.
 
 
+
 [Go to Demo](https://youtu.be/9Ry_A9LgrbQ)
 
 [![Video](http://img.youtube.com/vi/9Ry_A9LgrbQ/0.jpg)](https://youtu.be/9Ry_A9LgrbQ)
 
 
 ## Run Tests
 To ensure everything is functioning smoothly, run the tests using the following commands:
@@ -83,15 +84,15 @@
 poetry run pytest e2e
 ```
 
 ## Run the App
 Ready to see streamlit-pandera in action? Simply run the following command:
 
 ```bash
-poetry run streamlit run streamlit_panderas/validate_file.py
+poetry run streamlit run app/run.py
 ```
 
 ## Contributions
 We welcome contributions from the community! If you have any ideas, bug fixes, or enhancements, feel free to submit a pull request.
 
 ## Feedback
 We'd love to hear your feedback! Whether you have suggestions for improvement or just want to share your experience using streamlit-pandera, don't hesitate to reach out.
```

