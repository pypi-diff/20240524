# Comparing `tmp/flask_app_install-0.1.4.tar.gz` & `tmp/flask_app_install-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_app_install-0.1.4.tar", last modified: Wed May 22 04:12:16 2024, max compression
+gzip compressed data, was "flask_app_install-0.1.5.tar", last modified: Thu May 23 21:55:46 2024, max compression
```

## Comparing `flask_app_install-0.1.4.tar` & `flask_app_install-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 04:12:16.688405 flask_app_install-0.1.4/
-drwxrwxrwx   0        0        0        0 2024-05-22 04:12:16.683865 flask_app_install-0.1.4/Flask_App_Install.egg-info/
--rw-rw-rw-   0        0        0      951 2024-05-22 04:12:16.000000 flask_app_install-0.1.4/Flask_App_Install.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2024-05-22 04:12:16.000000 flask_app_install-0.1.4/Flask_App_Install.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 04:12:16.000000 flask_app_install-0.1.4/Flask_App_Install.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-22 04:12:16.000000 flask_app_install-0.1.4/Flask_App_Install.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-22 04:12:16.000000 flask_app_install-0.1.4/Flask_App_Install.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2024-05-18 13:06:21.000000 flask_app_install-0.1.4/LICENCE
--rw-rw-rw-   0        0        0      951 2024-05-22 04:12:16.685865 flask_app_install-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      166 2024-05-22 03:28:51.000000 flask_app_install-0.1.4/README.md
--rw-rw-rw-   0        0        0      360 2024-05-20 13:06:13.000000 flask_app_install-0.1.4/run.sh
--rw-rw-rw-   0        0        0       42 2024-05-22 04:12:16.688846 flask_app_install-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1464 2024-05-22 04:12:04.000000 flask_app_install-0.1.4/setup.py
--rw-rw-rw-   0        0        0      209 2024-05-20 12:43:39.000000 flask_app_install-0.1.4/setup.sh
-drwxrwxrwx   0        0        0        0 2024-05-22 04:12:16.681867 flask_app_install-0.1.4/src/
--rw-rw-rw-   0        0        0      106 2024-05-20 07:36:38.000000 flask_app_install-0.1.4/src/__init__.py
--rw-rw-rw-   0        0        0     2029 2024-05-22 03:11:11.000000 flask_app_install-0.1.4/src/app.py
--rw-rw-rw-   0        0        0      372 2024-05-20 07:38:30.000000 flask_app_install-0.1.4/src/writefile_app.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:55:46.423781 flask_app_install-0.1.5/
+drwxrwxrwx   0        0        0        0 2024-05-23 21:55:46.415483 flask_app_install-0.1.5/Flask_App_Install.egg-info/
+-rw-rw-rw-   0        0        0     1085 2024-05-23 21:55:46.000000 flask_app_install-0.1.5/Flask_App_Install.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-05-23 21:55:46.000000 flask_app_install-0.1.5/Flask_App_Install.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 21:55:46.000000 flask_app_install-0.1.5/Flask_App_Install.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-23 21:55:46.000000 flask_app_install-0.1.5/Flask_App_Install.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-23 21:55:46.000000 flask_app_install-0.1.5/Flask_App_Install.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2024-05-18 13:06:21.000000 flask_app_install-0.1.5/LICENCE
+-rw-rw-rw-   0        0        0     1085 2024-05-23 21:55:46.415483 flask_app_install-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-05-23 21:51:57.000000 flask_app_install-0.1.5/README.md
+-rw-rw-rw-   0        0        0      360 2024-05-20 13:06:13.000000 flask_app_install-0.1.5/run.sh
+-rw-rw-rw-   0        0        0       42 2024-05-23 21:55:46.426499 flask_app_install-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1404 2024-05-23 21:55:00.000000 flask_app_install-0.1.5/setup.py
+-rw-rw-rw-   0        0        0      209 2024-05-20 12:43:39.000000 flask_app_install-0.1.5/setup.sh
+drwxrwxrwx   0        0        0        0 2024-05-23 21:55:46.406534 flask_app_install-0.1.5/src/
+-rw-rw-rw-   0        0        0      154 2024-05-23 21:55:31.000000 flask_app_install-0.1.5/src/__init__.py
+-rw-rw-rw-   0        0        0     2305 2024-05-22 05:48:23.000000 flask_app_install-0.1.5/src/app.py
+-rw-rw-rw-   0        0        0      546 2024-05-23 21:50:12.000000 flask_app_install-0.1.5/src/application.py
+-rw-rw-rw-   0        0        0      360 2024-05-22 04:23:22.000000 flask_app_install-0.1.5/src/writefile_app.py
```

### Comparing `flask_app_install-0.1.4/Flask_App_Install.egg-info/PKG-INFO` & `flask_app_install-0.1.5/Flask_App_Install.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask_App_Install
-Version: 0.1.4
+Version: 0.1.5
 Summary: Sets up a basic Flask App with Javascipt Functionality
 Author: kunaalg
 Author-email: <kunaal@runcode.in>
 Keywords: python,Flask,App,Javascript,Function,math
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -15,20 +15,33 @@
 License-File: LICENCE
 Requires-Dist: datetime
 Requires-Dist: pandas
 Requires-Dist: requests
 Requires-Dist: numpy
 Requires-Dist: flask
 Requires-Dist: virtualenv
-Requires-Dist: pipreqs
-Requires-Dist: pip-tools
 
 
+Initiate the Virtual Env
+import venv 
+
+venv_path = venv.EnvBuilder()
+
+
+
 Install the Package:
 
 Create a file called start.py
 
 from src.app import create_app
 
-Call the create_app() function 
+Call the create_app() function
+
+
+else
+
+
+from src.application import application 
+
+Call the application() function
 
 Update the HTML & JS files as required
```

### Comparing `flask_app_install-0.1.4/LICENCE` & `flask_app_install-0.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `flask_app_install-0.1.4/PKG-INFO` & `flask_app_install-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask_App_Install
-Version: 0.1.4
+Version: 0.1.5
 Summary: Sets up a basic Flask App with Javascipt Functionality
 Author: kunaalg
 Author-email: <kunaal@runcode.in>
 Keywords: python,Flask,App,Javascript,Function,math
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -15,20 +15,33 @@
 License-File: LICENCE
 Requires-Dist: datetime
 Requires-Dist: pandas
 Requires-Dist: requests
 Requires-Dist: numpy
 Requires-Dist: flask
 Requires-Dist: virtualenv
-Requires-Dist: pipreqs
-Requires-Dist: pip-tools
 
 
+Initiate the Virtual Env
+import venv 
+
+venv_path = venv.EnvBuilder()
+
+
+
 Install the Package:
 
 Create a file called start.py
 
 from src.app import create_app
 
-Call the create_app() function 
+Call the create_app() function
+
+
+else
+
+
+from src.application import application 
+
+Call the application() function
 
 Update the HTML & JS files as required
```

### Comparing `flask_app_install-0.1.4/setup.py` & `flask_app_install-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,36 +3,35 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 DESCRIPTION = 'Sets up a basic Flask App with Javascipt Functionality'
 LONG_DESCRIPTION = 'A package that sets up a basic Flask App Boilerplate with Javascript Functionality.'
 
 # Setting up
 setup(
     name="Flask_App_Install",
     version=VERSION,
     author="kunaalg",
     author_email="<kunaal@runcode.in>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
-    include_package_data=True,
+    include_package_data=False,
     data_files=[
         ('src/writefile_app.py', ['src/writefile_app.py']),
         ('src/app.py', ['src/app.py']),
-        ('src/run.sh', ['run.sh']),
         ],
     packages=find_packages(),
     scripts=['run.sh','setup.sh'],
-    install_requires=['datetime', 'pandas', 'requests', 'numpy', 'flask', 'virtualenv', 'pipreqs', 'pip-tools'],
+    install_requires=['datetime', 'pandas', 'requests', 'numpy', 'flask', 'virtualenv'],
     keywords=['python', 'Flask', 'App', 'Javascript', 'Function', 'math'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `flask_app_install-0.1.4/src/app.py` & `flask_app_install-0.1.5/src/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 import os
+from pathlib import *
 from flask import Flask, jsonify, render_template, request
 
 def create_index_html():
     html_content = """
     <!DOCTYPE html>
-    <html>
+    <html lang='EN'>
     <head>
         <meta charset="utf-8">
         <meta http-equiv="X-UA-Compatible" content="IE=edge">
         <title>FlaskApplication</title>
         <meta name="description" content="">
         <meta name="viewport" content="width=device-width, initial-scale=1">
         <link rel="stylesheet" href="">
         <title>Flask App</title>
         <script src="{{ url_for('static', filename='js/script.js') }}"></script>
     </head>
     <body>
+        <form id="myForm">
+            <label for="name">Name:</label><br>
+            <input type="text" id="name" name="name"><br>
+            <input type="submit" value="Submit">
+        </form>
+        <p id="result"></p>
         <!-- rest of your HTML code -->
     </body>
     </html>
     """
     new_directory = 'templates'
     if not os.path.exists(new_directory):
         os.makedirs(new_directory)
@@ -49,15 +56,15 @@
         f.write(js_content)
 
 def create_app():
     app = Flask(__name__)
 
     @app.route('/')
     def index():
-        return render_template('index.html')
+        return render_template.absolute(('index.html'))
 
     @app.route('/process', methods=['POST'])
     def process():
         name = request.form['name']
         return jsonify({'result': 'Hello, ' + name + '!'})
 
     create_index_html()
```

