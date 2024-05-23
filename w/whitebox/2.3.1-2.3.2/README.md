# Comparing `tmp/whitebox-2.3.1.tar.gz` & `tmp/whitebox-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whitebox-2.3.1.tar", last modified: Wed Mar 29 18:40:17 2023, max compression
+gzip compressed data, was "whitebox-2.3.2.tar", last modified: Thu May 23 23:26:22 2024, max compression
```

## Comparing `whitebox-2.3.1.tar` & `whitebox-2.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:40:17.845955 whitebox-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-29 18:40:02.000000 whitebox-2.3.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-03-29 18:40:02.000000 whitebox-2.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-29 18:40:02.000000 whitebox-2.3.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-29 18:40:02.000000 whitebox-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-29 18:40:02.000000 whitebox-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-03-29 18:40:17.845955 whitebox-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-03-29 18:40:02.000000 whitebox-2.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:40:17.841956 whitebox-2.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-29 18:40:02.000000 whitebox-2.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-29 18:40:02.000000 whitebox-2.3.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-03-29 18:40:02.000000 whitebox-2.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-29 18:40:02.000000 whitebox-2.3.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-29 18:40:02.000000 whitebox-2.3.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-29 18:40:02.000000 whitebox-2.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-29 18:40:02.000000 whitebox-2.3.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-29 18:40:02.000000 whitebox-2.3.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-29 18:40:02.000000 whitebox-2.3.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-29 18:40:02.000000 whitebox-2.3.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-29 18:40:17.845955 whitebox-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-29 18:40:02.000000 whitebox-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:40:17.845955 whitebox-2.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-29 18:40:02.000000 whitebox-2.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-29 18:40:02.000000 whitebox-2.3.1/tests/test_whitebox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:40:17.845955 whitebox-2.3.1/whitebox/
--rwxr-xr-x   0 runner    (1001) docker     (123)      175 2023-03-29 18:40:02.000000 whitebox-2.3.1/whitebox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-03-29 18:40:02.000000 whitebox-2.3.1/whitebox/automation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      401 2023-03-29 18:40:02.000000 whitebox-2.3.1/whitebox/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-03-29 18:40:02.000000 whitebox-2.3.1/whitebox/download_wbt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2605 2023-03-29 18:40:02.000000 whitebox-2.3.1/whitebox/example.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-03-29 18:40:02.000000 whitebox-2.3.1/whitebox/whitebox.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-03-29 18:40:02.000000 whitebox-2.3.1/whitebox/whitebox_example.py
--rw-r--r--   0 runner    (1001) docker     (123)   503114 2023-03-29 18:40:02.000000 whitebox-2.3.1/whitebox/whitebox_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:40:17.845955 whitebox-2.3.1/whitebox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-03-29 18:40:17.000000 whitebox-2.3.1/whitebox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-29 18:40:17.000000 whitebox-2.3.1/whitebox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 18:40:17.000000 whitebox-2.3.1/whitebox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-29 18:40:17.000000 whitebox-2.3.1/whitebox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 18:40:17.000000 whitebox-2.3.1/whitebox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-29 18:40:17.000000 whitebox-2.3.1/whitebox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-29 18:40:17.000000 whitebox-2.3.1/whitebox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:26:22.160380 whitebox-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-23 23:26:14.000000 whitebox-2.3.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-23 23:26:14.000000 whitebox-2.3.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-23 23:26:14.000000 whitebox-2.3.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 23:26:14.000000 whitebox-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-23 23:26:14.000000 whitebox-2.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-05-23 23:26:22.160380 whitebox-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10105 2024-05-23 23:26:14.000000 whitebox-2.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:26:22.156381 whitebox-2.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-23 23:26:14.000000 whitebox-2.3.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 23:26:14.000000 whitebox-2.3.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-05-23 23:26:14.000000 whitebox-2.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 23:26:14.000000 whitebox-2.3.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 23:26:14.000000 whitebox-2.3.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-23 23:26:14.000000 whitebox-2.3.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-23 23:26:14.000000 whitebox-2.3.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-23 23:26:14.000000 whitebox-2.3.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 23:26:14.000000 whitebox-2.3.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-23 23:26:14.000000 whitebox-2.3.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-23 23:26:22.164381 whitebox-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-23 23:26:14.000000 whitebox-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:26:22.160380 whitebox-2.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 23:26:14.000000 whitebox-2.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-23 23:26:14.000000 whitebox-2.3.2/tests/test_whitebox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:26:22.160380 whitebox-2.3.2/whitebox/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-05-23 23:26:14.000000 whitebox-2.3.2/whitebox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-23 23:26:14.000000 whitebox-2.3.2/whitebox/automation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-05-23 23:26:14.000000 whitebox-2.3.2/whitebox/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-05-23 23:26:14.000000 whitebox-2.3.2/whitebox/download_wbt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2605 2024-05-23 23:26:14.000000 whitebox-2.3.2/whitebox/example.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-23 23:26:14.000000 whitebox-2.3.2/whitebox/whitebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-05-23 23:26:14.000000 whitebox-2.3.2/whitebox/whitebox_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)   503655 2024-05-23 23:26:14.000000 whitebox-2.3.2/whitebox/whitebox_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:26:22.160380 whitebox-2.3.2/whitebox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-05-23 23:26:22.000000 whitebox-2.3.2/whitebox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-23 23:26:22.000000 whitebox-2.3.2/whitebox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 23:26:22.000000 whitebox-2.3.2/whitebox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 23:26:22.000000 whitebox-2.3.2/whitebox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 23:26:22.000000 whitebox-2.3.2/whitebox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 23:26:22.000000 whitebox-2.3.2/whitebox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 23:26:22.000000 whitebox-2.3.2/whitebox.egg-info/top_level.txt
```

### Comparing `whitebox-2.3.1/CONTRIBUTING.rst` & `whitebox-2.3.2/CONTRIBUTING.rst`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Types of Contributions
 ----------------------
 
 Report Bugs
 ~~~~~~~~~~~
 
-Report bugs at https://github.com/giswqs/whitebox/issues.
+Report bugs at https://github.com/opengeos/whitebox/issues.
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
@@ -41,15 +41,15 @@
 whitebox could always use more documentation, whether as part of the
 official whitebox docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Submit Feedback
 ~~~~~~~~~~~~~~~
 
-The best way to send feedback is to file an issue at https://github.com/giswqs/whitebox/issues.
+The best way to send feedback is to file an issue at https://github.com/opengeos/whitebox/issues.
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that contributions
   are welcome :)
@@ -98,17 +98,14 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
-3. The pull request should work for Python 3.4, 3.5 and 3.6, and for PyPy. Check
-   https://travis-ci.org/giswqs/whitebox/pull_requests
-   and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
```

### Comparing `whitebox-2.3.1/LICENSE` & `whitebox-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whitebox-2.3.1/PKG-INFO` & `whitebox-2.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: whitebox
-Version: 2.3.1
+Version: 2.3.2
 Summary: An advanced geospatial data analysis platform 
-Home-page: https://github.com/giswqs/whitebox
+Home-page: https://github.com/opengeos/whitebox
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: whitebox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: Click>=6.0
 
 ===============
 whitebox-python
 ===============
 
 .. image:: https://colab.research.google.com/assets/colab-badge.svg
         :target: https://gishub.org/whitebox-colab
@@ -33,45 +34,36 @@
 
 .. image:: https://pepy.tech/badge/whitebox
         :target: https://pepy.tech/project/whitebox
 
 .. image:: https://anaconda.org/conda-forge/whitebox/badges/version.svg
         :target: https://anaconda.org/conda-forge/whitebox
 
-.. image:: https://img.shields.io/travis/giswqs/whitebox-python.svg
-        :target: https://travis-ci.org/giswqs/whitebox-python
-
-.. image:: https://ci.appveyor.com/api/projects/status/a7r1hna30kjbsmk3?svg=true
-        :target: https://ci.appveyor.com/project/giswqs/whitebox-python
-
 .. image:: https://readthedocs.org/projects/whitebox/badge/?version=latest
         :target: https://whitebox.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
         :target: https://opensource.org/licenses/MIT
 
-.. image:: https://img.shields.io/twitter/follow/giswqs?style=social   
-        :target: https://twitter.com/giswqs
-
 .. image:: https://img.shields.io/badge/Donate-Buy%20me%20a%20coffee-yellowgreen.svg
-        :target: https://www.buymeacoffee.com/giswqs
+        :target: https://www.buymeacoffee.com/opengeos
 
 
 Important Note
 --------------
 .. image:: https://i.imgur.com/Ic8BA7C.png
 
 This repository is related to the WhiteboxTools Python Frontend only. You can report issues to this repo if you have problems installing this Python package. If you encounter any tool functioning specific errors, please `open an issue`_ on Dr. John Lindsay's WhiteboxTools_ repo.  
 
 **Links**
 
 * Authors: Dr. John Lindsay (https://jblindsay.github.io/ghrg/index.html)
 * Contributors: Dr. Qiusheng Wu (https://wetlands.io)
-* GitHub repo: https://github.com/giswqs/whitebox-python
+* GitHub repo: https://github.com/opengeos/whitebox-python
 * WhiteboxTools: https://github.com/jblindsay/whitebox-tools
 * User Manual: https://www.whiteboxgeo.com/manual/wbt_book/intro.html
 * PyPI: https://pypi.org/project/whitebox/
 * conda-forge: https://anaconda.org/conda-forge/whitebox
 * Documentation: https://whitebox.readthedocs.io
 * Binder: https://gishub.org/whitebox-cloud
 * Free software: `MIT license`_
@@ -223,44 +215,44 @@
 The WhiteboxTools library currently supports read/writing raster data in Whitebox GAT, GeoTIFF, ESRI (ArcGIS) ASCII and binary (.flt & .hdr), GRASS GIS, Idrisi, SAGA GIS (binary and ASCII), and Surfer 7 data formats. At present, there is limited ability in WhiteboxTools to read vector geospatial data. Support for Shapefile (and other common vector formats) will be enhanced within the library soon. 
 
 Contributing
 ------------
 
 If you would like to contribute to the project as a developer, follow these instructions to get started:
 
-1. Fork the whitebox project (https://github.com/giswqs/whitebox-python)
+1. Fork the whitebox project (https://github.com/opengeos/whitebox-python)
 2. Create your feature branch (git checkout -b my-new-feature)
 3. Commit your changes (git commit -am 'Add some feature')
 4. Push to the branch (git push origin my-new-feature)
 5. Create a new Pull Request
 
 License
 -------
 
 The **whitebox** package is distributed under the `MIT license`_, a permissive open-source (free software) license.
 
 
 Reporting Bugs
 --------------
-Report bugs at https://github.com/giswqs/whitebox-python/issues.
+Report bugs at https://github.com/opengeos/whitebox-python/issues.
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-.. _example.py: https://github.com/giswqs/whitebox/blob/master/whitebox/example.py
+.. _example.py: https://github.com/opengeos/whitebox/blob/master/whitebox/example.py
 .. _WhiteboxTools: https://github.com/jblindsay/whitebox-tools
 .. _webpage: https://jblindsay.github.io/ghrg/index.html
 .. _jblindsay: https://github.com/jblindsay
 .. _`Geomorphometry and Hydrogeomatics Research Group`: https://jblindsay.github.io/ghrg/index.html
 .. _`conda user guide`: https://conda.io/docs/user-guide/install/index.html
 .. _`managing Python environment`: https://conda.io/docs/user-guide/tasks/manage-environments.html
 .. _`WhiteboxTools Usage`: https://github.com/jblindsay/whitebox-tools#3-usage
```

### Comparing `whitebox-2.3.1/README.rst` & `whitebox-2.3.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -13,45 +13,36 @@
 
 .. image:: https://pepy.tech/badge/whitebox
         :target: https://pepy.tech/project/whitebox
 
 .. image:: https://anaconda.org/conda-forge/whitebox/badges/version.svg
         :target: https://anaconda.org/conda-forge/whitebox
 
-.. image:: https://img.shields.io/travis/giswqs/whitebox-python.svg
-        :target: https://travis-ci.org/giswqs/whitebox-python
-
-.. image:: https://ci.appveyor.com/api/projects/status/a7r1hna30kjbsmk3?svg=true
-        :target: https://ci.appveyor.com/project/giswqs/whitebox-python
-
 .. image:: https://readthedocs.org/projects/whitebox/badge/?version=latest
         :target: https://whitebox.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
         :target: https://opensource.org/licenses/MIT
 
-.. image:: https://img.shields.io/twitter/follow/giswqs?style=social   
-        :target: https://twitter.com/giswqs
-
 .. image:: https://img.shields.io/badge/Donate-Buy%20me%20a%20coffee-yellowgreen.svg
-        :target: https://www.buymeacoffee.com/giswqs
+        :target: https://www.buymeacoffee.com/opengeos
 
 
 Important Note
 --------------
 .. image:: https://i.imgur.com/Ic8BA7C.png
 
 This repository is related to the WhiteboxTools Python Frontend only. You can report issues to this repo if you have problems installing this Python package. If you encounter any tool functioning specific errors, please `open an issue`_ on Dr. John Lindsay's WhiteboxTools_ repo.  
 
 **Links**
 
 * Authors: Dr. John Lindsay (https://jblindsay.github.io/ghrg/index.html)
 * Contributors: Dr. Qiusheng Wu (https://wetlands.io)
-* GitHub repo: https://github.com/giswqs/whitebox-python
+* GitHub repo: https://github.com/opengeos/whitebox-python
 * WhiteboxTools: https://github.com/jblindsay/whitebox-tools
 * User Manual: https://www.whiteboxgeo.com/manual/wbt_book/intro.html
 * PyPI: https://pypi.org/project/whitebox/
 * conda-forge: https://anaconda.org/conda-forge/whitebox
 * Documentation: https://whitebox.readthedocs.io
 * Binder: https://gishub.org/whitebox-cloud
 * Free software: `MIT license`_
@@ -203,44 +194,44 @@
 The WhiteboxTools library currently supports read/writing raster data in Whitebox GAT, GeoTIFF, ESRI (ArcGIS) ASCII and binary (.flt & .hdr), GRASS GIS, Idrisi, SAGA GIS (binary and ASCII), and Surfer 7 data formats. At present, there is limited ability in WhiteboxTools to read vector geospatial data. Support for Shapefile (and other common vector formats) will be enhanced within the library soon. 
 
 Contributing
 ------------
 
 If you would like to contribute to the project as a developer, follow these instructions to get started:
 
-1. Fork the whitebox project (https://github.com/giswqs/whitebox-python)
+1. Fork the whitebox project (https://github.com/opengeos/whitebox-python)
 2. Create your feature branch (git checkout -b my-new-feature)
 3. Commit your changes (git commit -am 'Add some feature')
 4. Push to the branch (git push origin my-new-feature)
 5. Create a new Pull Request
 
 License
 -------
 
 The **whitebox** package is distributed under the `MIT license`_, a permissive open-source (free software) license.
 
 
 Reporting Bugs
 --------------
-Report bugs at https://github.com/giswqs/whitebox-python/issues.
+Report bugs at https://github.com/opengeos/whitebox-python/issues.
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-.. _example.py: https://github.com/giswqs/whitebox/blob/master/whitebox/example.py
+.. _example.py: https://github.com/opengeos/whitebox/blob/master/whitebox/example.py
 .. _WhiteboxTools: https://github.com/jblindsay/whitebox-tools
 .. _webpage: https://jblindsay.github.io/ghrg/index.html
 .. _jblindsay: https://github.com/jblindsay
 .. _`Geomorphometry and Hydrogeomatics Research Group`: https://jblindsay.github.io/ghrg/index.html
 .. _`conda user guide`: https://conda.io/docs/user-guide/install/index.html
 .. _`managing Python environment`: https://conda.io/docs/user-guide/tasks/manage-environments.html
 .. _`WhiteboxTools Usage`: https://github.com/jblindsay/whitebox-tools#3-usage
```

### Comparing `whitebox-2.3.1/docs/Makefile` & `whitebox-2.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `whitebox-2.3.1/docs/conf.py` & `whitebox-2.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `whitebox-2.3.1/docs/installation.rst` & `whitebox-2.3.2/docs/installation.rst`

 * *Files 12% similar despite different names*

```diff
@@ -28,24 +28,24 @@
 
 The sources for whitebox can be downloaded from the `Github repo`_.
 
 You can either clone the public repository:
 
 .. code-block:: console
 
-    $ git clone git://github.com/giswqs/whitebox
+    $ git clone git://github.com/opengeos/whitebox
 
 Or download the `tarball`_:
 
 .. code-block:: console
 
-    $ curl  -OL https://github.com/giswqs/whitebox/tarball/master
+    $ curl  -OL https://github.com/opengeos/whitebox/tarball/master
 
 Once you have a copy of the source, you can install it with:
 
 .. code-block:: console
 
     $ python setup.py install
 
 
-.. _Github repo: https://github.com/giswqs/whitebox
-.. _tarball: https://github.com/giswqs/whitebox/tarball/master
+.. _Github repo: https://github.com/opengeos/whitebox
+.. _tarball: https://github.com/opengeos/whitebox/tarball/master
```

### Comparing `whitebox-2.3.1/docs/make.bat` & `whitebox-2.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `whitebox-2.3.1/docs/usage.rst` & `whitebox-2.3.2/docs/usage.rst`

 * *Files 16% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     wbt.verbose = False
     wbt.feature_preserving_denoise("DEM.tif", "smoothed.tif", filter=9)
     wbt.breach_depressions("smoothed.tif", "breached.tif")
     wbt.d_inf_flow_accumulation("breached.tif", "flow_accum.tif")
 
 Check the example.py_ for more details.
 
-.. _example.py: https://github.com/giswqs/whitebox/blob/master/whitebox/example.py
+.. _example.py: https://github.com/opengeos/whitebox/blob/master/whitebox/example.py
```

### Comparing `whitebox-2.3.1/setup.py` & `whitebox-2.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,11 +44,11 @@
     include_package_data=True,
     keywords='whitebox',
     name='whitebox',
     packages=find_packages(include=['whitebox']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
-    url='https://github.com/giswqs/whitebox',
-    version='2.3.1',
+    url='https://github.com/opengeos/whitebox',
+    version='2.3.2',
     zip_safe=False,
 )
```

### Comparing `whitebox-2.3.1/tests/test_whitebox.py` & `whitebox-2.3.2/tests/test_whitebox.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
     def tearDown(self):
         """Tear down test fixtures, if any."""
 
     def test_000_something(self):
         """Test something."""
 
-    def test_command_line_interface(self):
-        """Test the CLI."""
-        runner = CliRunner()
-        result = runner.invoke(cli.main)
-        assert result.exit_code == 0
-        assert 'whitebox.cli.main' in result.output
-        help_result = runner.invoke(cli.main, ['--help'])
-        assert help_result.exit_code == 0
-        assert '--help  Show this message and exit.' in help_result.output
+    # def test_command_line_interface(self):
+    #     """Test the CLI."""
+    #     runner = CliRunner()
+    #     result = runner.invoke(cli.main)
+    #     assert result.exit_code == 0
+    #     assert 'whitebox.cli.main' in result.output
+    #     help_result = runner.invoke(cli.main, ['--help'])
+    #     assert help_result.exit_code == 0
+    #     assert '--help  Show this message and exit.' in help_result.output
```

### Comparing `whitebox-2.3.1/whitebox/automation.py` & `whitebox-2.3.2/whitebox/automation.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,33 +28,40 @@
 init_img_dir = os.path.join(WBT_dir, "img")
 new_img_dir = os.path.join(work_dir, "img")
 init_plugin_dir = os.path.join(WBT_dir, "plugins")
 new_plugin_dir = os.path.join(work_dir, "plugins")
 
 if not os.path.exists(zip_path):
     print("Downloading WhiteboxTools binary ...")
-    # url = "https://github.com/giswqs/whitebox-bin/raw/master/WhiteboxTools_linux_amd64.zip"
+    # url = "https://github.com/opengeos/whitebox-bin/raw/master/WhiteboxTools_linux_amd64.zip"
     url = "https://www.whiteboxgeo.com/WBT_Linux/WhiteboxTools_linux_amd64.zip"
     urllib.request.urlretrieve(url, zip_path)  # Download WhiteboxTools
 else:
     print("WhiteboxTools binary already exists.")
 
 if os.path.exists(WBT_dir):
     shutil.rmtree(WBT_dir)
 
 print("Decompressing {} ...".format(linux_zip))
 with zipfile.ZipFile(zip_path, "r") as tar_ref:
     tar_ref.extractall(work_dir)
 
+zip_dir = os.path.join(work_dir, linux_zip.split(".")[0])
+src_dir = os.path.join(zip_dir, "WBT")
+shutil.move(src_dir, WBT_dir)
+
 if os.path.exists(new_img_dir):
     shutil.rmtree(new_img_dir)
 
 if os.path.exists(new_plugin_dir):
     shutil.rmtree(new_plugin_dir)
 
+if os.path.exists(zip_dir):
+    shutil.rmtree(zip_dir)
+
 shutil.copytree(init_img_dir, new_img_dir)
 shutil.copytree(init_plugin_dir, new_plugin_dir)
 
 
 # print("Generating wb_runner.py ...")
 # with open(os.path.join(WBT_dir, "wb_runner.py")) as f_runner:
 #     lines = f_runner.readlines()
@@ -107,12 +114,12 @@
             f.write("            os.chdir(work_dir)\n")
 
 
 shutil.move(
     os.path.join(WBT_dir, "whitebox_tools"), os.path.join(work_dir, "whitebox_tools")
 )
 
-shutil.move(
-    os.path.join(WBT_dir, "whitebox_runner"), os.path.join(work_dir, "whitebox_runner")
-)
+# shutil.move(
+#     os.path.join(WBT_dir, "whitebox_runner"), os.path.join(work_dir, "whitebox_runner")
+# )
 
 f.close()
```

### Comparing `whitebox-2.3.1/whitebox/download_wbt.py` & `whitebox-2.3.2/whitebox/download_wbt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 def download_wbt(linux_musl=False, reset=False, verbose=True):
     """Downloads WhiteboxTools pre-complied binary for first-time use
 
     Args:
         linux_musl (bool, optional): Whether to download the musl version of WhiteboxTools for Linux. Defaults to False.
         reset (bool, optional): Whether to reset the WhiteboxTools installation. Defaults to False.
         verbose (bool, optional): Whether to print verbose messages. Defaults to True.
-   
+
     """
     import glob
     import os
     import sys
     import platform
     import zipfile
     import tarfile
@@ -32,21 +32,29 @@
     new_img_dir = os.path.join(pkg_dir, "img")
     init_plugin_dir = os.path.join(exe_dir, "plugins")
     new_plugin_dir = os.path.join(pkg_dir, "plugins")
 
     links = {
         "Windows": "https://www.whiteboxgeo.com/WBT_Windows/WhiteboxTools_win_amd64.zip",
         "Darwin": "https://www.whiteboxgeo.com/WBT_Darwin/WhiteboxTools_darwin_amd64.zip",
+        "Darwin-arm": "https://www.whiteboxgeo.com/WBT_Darwin/WhiteboxTools_darwin_m_series.zip",
         "Linux": "https://www.whiteboxgeo.com/WBT_Linux/WhiteboxTools_linux_amd64.zip",
-        "Linux-musl": "https://www.whiteboxgeo.com/WBT_Linux/WhiteboxTools_linux_musl.zip"
+        "Linux-musl": "https://www.whiteboxgeo.com/WBT_Linux/WhiteboxTools_linux_musl.zip",
     }
 
-    if linux_musl or ('google.colab' in sys.modules) or (os.environ.get('WBT_LINUX', False) == "MUSL"):
+    if (
+        linux_musl
+        or ("google.colab" in sys.modules)
+        or (os.environ.get("WBT_LINUX", False) == "MUSL")
+    ):
         links["Linux"] = links["Linux-musl"]
 
+    if platform.system() == "Darwin" and platform.processor() == "arm":
+        links["Darwin"] = links["Darwin-arm"]
+
     # These are backup links only used to pass GitHub automated tests. WhiteboxGeo links frequently encounter timeout errors, which fail the automated tests.
     backup_links = {
         "Windows": "https://github.com/giswqs/whitebox-bin/raw/master/WhiteboxTools_win_amd64.zip",
         "Darwin": "https://github.com/giswqs/whitebox-bin/raw/master/WhiteboxTools_darwin_amd64.zip",
         "Linux": "https://github.com/giswqs/whitebox-bin/raw/master/WhiteboxTools_linux_amd64.zip",
     }
 
@@ -116,58 +124,69 @@
 
                         tar.extractall(path, members, numeric_owner=numeric_owner)
 
                     safe_extract(tar_ref, pkg_dir)
             if verbose:
                 print("WhiteboxTools package directory: {}".format(pkg_dir))
 
+            zip_dir = zip_name.split(".")[0]
+            src_dir = os.path.join(zip_dir, "WBT")
+
+            if os.path.exists(src_dir):
+                shutil.move(src_dir, pkg_dir)
+
             if os.path.exists(new_img_dir):
                 shutil.rmtree(new_img_dir)
             if os.path.exists(new_plugin_dir):
                 shutil.rmtree(new_plugin_dir)
 
+            if os.path.exists(zip_dir):
+                shutil.rmtree(zip_dir)
+
             shutil.copytree(init_img_dir, new_img_dir)
             shutil.copytree(init_plugin_dir, new_plugin_dir)
 
             exe_ext = ""  # file extension for MacOS/Linux
             if platform.system() == "Windows":
                 exe_ext = ".exe"
             exe_name = "whitebox_tools{}".format(exe_ext)
             exe_path = os.path.join(exe_dir, exe_name)
-            runner_name = "whitebox_runner{}".format(exe_ext)
-            runner_path = os.path.join(exe_dir, runner_name)
+            # runner_name = "whitebox_runner{}".format(exe_ext)
+            # runner_path = os.path.join(exe_dir, runner_name)
 
             # grant executable permission
             if platform.system() != "Windows":
                 os.system("chmod 755 " + exe_path)
-                os.system("chmod 755 " + runner_path)
+                # os.system("chmod 755 " + runner_path)
             plugins = list(
                 set(glob.glob(os.path.join(new_plugin_dir, "*")))
                 - set(glob.glob(os.path.join(new_plugin_dir, "*.json")))
             )
             if platform.system() != "Windows":
                 for plugin in plugins:
                     os.system("chmod 755 " + plugin)
 
             exe_path_new = os.path.join(pkg_dir, exe_name)
             shutil.copy(exe_path, exe_path_new)
-            runner_path_new = os.path.join(pkg_dir, runner_name)
-            shutil.copy(runner_path, runner_path_new)
+            # runner_path_new = os.path.join(pkg_dir, runner_name)
+            # shutil.copy(runner_path, runner_path_new)
 
             try:
                 os.remove(zip_name)
             except:
                 pass
 
             # # The official WhiteboxTools Linux binary from whiteboxgeo.com requires GLIBC 2.29,
             # # which is incompatible with Google Colab that uses GLIBC 2.27. The following code
             # # downloads the binary that is compatible with Google Colab.
             if "google.colab" in sys.modules:
                 # url = "https://github.com/giswqs/whitebox-bin/raw/master/WhiteboxTools_ubuntu_18.04.zip"
-                url = "https://www.whiteboxgeo.com/WBT_Linux/WhiteboxTools_linux_musl.zip"
+                url = (
+                    "https://www.whiteboxgeo.com/WBT_Linux/WhiteboxTools_linux_musl.zip"
+                )
 
                 zip_name = os.path.join(pkg_dir, os.path.basename(url))
                 try:
                     request = urllib.request.urlopen(url, timeout=500)
                     with open(zip_name, "wb") as f:
                         f.write(request.read())
                     os.remove(exe_path)
@@ -185,16 +204,16 @@
 
             webbrowser.open("https://www.whiteboxgeo.com/", new=2)
 
         if not os.path.exists(work_dir):
             if verbose:
                 print("Downloading testdata ...")
             os.mkdir(work_dir)
-            dem_url = "https://github.com/giswqs/whitebox-python/raw/master/examples/testdata/DEM.tif"
-            dep_url = "https://github.com/giswqs/whitebox-python/raw/master/examples/testdata/DEM.dep"
+            dem_url = "https://github.com/opengeos/whitebox-python/raw/master/examples/testdata/DEM.tif"
+            dep_url = "https://github.com/opengeos/whitebox-python/raw/master/examples/testdata/DEM.dep"
             urllib.request.urlretrieve(dem_url, os.path.join(work_dir, "DEM.tif"))
             urllib.request.urlretrieve(dep_url, os.path.join(work_dir, "DEM.dep"))
 
     except:
         print("Unexpected error:", sys.exc_info()[0])
         raise
```

### Comparing `whitebox-2.3.1/whitebox/example.py` & `whitebox-2.3.2/whitebox/example.py`

 * *Files identical despite different names*

### Comparing `whitebox-2.3.1/whitebox/whitebox_example.py` & `whitebox-2.3.2/whitebox/whitebox_example.py`

 * *Files identical despite different names*

### Comparing `whitebox-2.3.1/whitebox/whitebox_tools.py` & `whitebox-2.3.2/whitebox/whitebox_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 def download_wbt(linux_musl=False, reset=False, verbose=True):
     """Downloads WhiteboxTools pre-complied binary for first-time use
 
     Args:
         linux_musl (bool, optional): Whether to download the musl version of WhiteboxTools for Linux. Defaults to False.
         reset (bool, optional): Whether to reset the WhiteboxTools installation. Defaults to False.
         verbose (bool, optional): Whether to print verbose messages. Defaults to True.
-   
+
     """
     import glob
     import os
     import sys
     import platform
     import zipfile
     import tarfile
@@ -61,21 +61,29 @@
     new_img_dir = os.path.join(pkg_dir, "img")
     init_plugin_dir = os.path.join(exe_dir, "plugins")
     new_plugin_dir = os.path.join(pkg_dir, "plugins")
 
     links = {
         "Windows": "https://www.whiteboxgeo.com/WBT_Windows/WhiteboxTools_win_amd64.zip",
         "Darwin": "https://www.whiteboxgeo.com/WBT_Darwin/WhiteboxTools_darwin_amd64.zip",
+        "Darwin-arm": "https://www.whiteboxgeo.com/WBT_Darwin/WhiteboxTools_darwin_m_series.zip",
         "Linux": "https://www.whiteboxgeo.com/WBT_Linux/WhiteboxTools_linux_amd64.zip",
-        "Linux-musl": "https://www.whiteboxgeo.com/WBT_Linux/WhiteboxTools_linux_musl.zip"
+        "Linux-musl": "https://www.whiteboxgeo.com/WBT_Linux/WhiteboxTools_linux_musl.zip",
     }
 
-    if linux_musl or ('google.colab' in sys.modules) or (os.environ.get('WBT_LINUX', False) == "MUSL"):
+    if (
+        linux_musl
+        or ("google.colab" in sys.modules)
+        or (os.environ.get("WBT_LINUX", False) == "MUSL")
+    ):
         links["Linux"] = links["Linux-musl"]
 
+    if platform.system() == "Darwin" and platform.processor() == "arm":
+        links["Darwin"] = links["Darwin-arm"]
+
     # These are backup links only used to pass GitHub automated tests. WhiteboxGeo links frequently encounter timeout errors, which fail the automated tests.
     backup_links = {
         "Windows": "https://github.com/giswqs/whitebox-bin/raw/master/WhiteboxTools_win_amd64.zip",
         "Darwin": "https://github.com/giswqs/whitebox-bin/raw/master/WhiteboxTools_darwin_amd64.zip",
         "Linux": "https://github.com/giswqs/whitebox-bin/raw/master/WhiteboxTools_linux_amd64.zip",
     }
 
@@ -145,58 +153,69 @@
 
                         tar.extractall(path, members, numeric_owner=numeric_owner)
 
                     safe_extract(tar_ref, pkg_dir)
             if verbose:
                 print("WhiteboxTools package directory: {}".format(pkg_dir))
 
+            zip_dir = zip_name.split(".")[0]
+            src_dir = os.path.join(zip_dir, "WBT")
+
+            if os.path.exists(src_dir):
+                shutil.move(src_dir, pkg_dir)
+
             if os.path.exists(new_img_dir):
                 shutil.rmtree(new_img_dir)
             if os.path.exists(new_plugin_dir):
                 shutil.rmtree(new_plugin_dir)
 
+            if os.path.exists(zip_dir):
+                shutil.rmtree(zip_dir)
+
             shutil.copytree(init_img_dir, new_img_dir)
             shutil.copytree(init_plugin_dir, new_plugin_dir)
 
             exe_ext = ""  # file extension for MacOS/Linux
             if platform.system() == "Windows":
                 exe_ext = ".exe"
             exe_name = "whitebox_tools{}".format(exe_ext)
             exe_path = os.path.join(exe_dir, exe_name)
-            runner_name = "whitebox_runner{}".format(exe_ext)
-            runner_path = os.path.join(exe_dir, runner_name)
+            # runner_name = "whitebox_runner{}".format(exe_ext)
+            # runner_path = os.path.join(exe_dir, runner_name)
 
             # grant executable permission
             if platform.system() != "Windows":
                 os.system("chmod 755 " + exe_path)
-                os.system("chmod 755 " + runner_path)
+                # os.system("chmod 755 " + runner_path)
             plugins = list(
                 set(glob.glob(os.path.join(new_plugin_dir, "*")))
                 - set(glob.glob(os.path.join(new_plugin_dir, "*.json")))
             )
             if platform.system() != "Windows":
                 for plugin in plugins:
                     os.system("chmod 755 " + plugin)
 
             exe_path_new = os.path.join(pkg_dir, exe_name)
             shutil.copy(exe_path, exe_path_new)
-            runner_path_new = os.path.join(pkg_dir, runner_name)
-            shutil.copy(runner_path, runner_path_new)
+            # runner_path_new = os.path.join(pkg_dir, runner_name)
+            # shutil.copy(runner_path, runner_path_new)
 
             try:
                 os.remove(zip_name)
             except:
                 pass
 
             # # The official WhiteboxTools Linux binary from whiteboxgeo.com requires GLIBC 2.29,
             # # which is incompatible with Google Colab that uses GLIBC 2.27. The following code
             # # downloads the binary that is compatible with Google Colab.
             if "google.colab" in sys.modules:
                 # url = "https://github.com/giswqs/whitebox-bin/raw/master/WhiteboxTools_ubuntu_18.04.zip"
-                url = "https://www.whiteboxgeo.com/WBT_Linux/WhiteboxTools_linux_musl.zip"
+                url = (
+                    "https://www.whiteboxgeo.com/WBT_Linux/WhiteboxTools_linux_musl.zip"
+                )
 
                 zip_name = os.path.join(pkg_dir, os.path.basename(url))
                 try:
                     request = urllib.request.urlopen(url, timeout=500)
                     with open(zip_name, "wb") as f:
                         f.write(request.read())
                     os.remove(exe_path)
@@ -214,16 +233,16 @@
 
             webbrowser.open("https://www.whiteboxgeo.com/", new=2)
 
         if not os.path.exists(work_dir):
             if verbose:
                 print("Downloading testdata ...")
             os.mkdir(work_dir)
-            dem_url = "https://github.com/giswqs/whitebox-python/raw/master/examples/testdata/DEM.tif"
-            dep_url = "https://github.com/giswqs/whitebox-python/raw/master/examples/testdata/DEM.dep"
+            dem_url = "https://github.com/opengeos/whitebox-python/raw/master/examples/testdata/DEM.tif"
+            dep_url = "https://github.com/opengeos/whitebox-python/raw/master/examples/testdata/DEM.dep"
             urllib.request.urlretrieve(dem_url, os.path.join(work_dir, "DEM.tif"))
             urllib.request.urlretrieve(dep_url, os.path.join(work_dir, "DEM.dep"))
 
     except:
         print("Unexpected error:", sys.exc_info()[0])
         raise
 
@@ -3040,15 +3059,15 @@
     def breakline_mapping(self, dem, output, threshold=2.0, min_length=3, callback=None):
         """This tool maps breaklines from an input DEM.
 
         Keyword arguments:
 
         dem -- Name of the input raster image file. 
         output -- Name of the output vector lines file. 
-        threshold -- Threshold value (0 - infinity but typcially 1 to 5 works well). 
+        threshold -- Threshold value (0 - infinity but typically 1 to 5 works well). 
         min_length -- Minimum line length, in grid cells. 
         callback -- Custom function for handling tool text outputs.
         """
         args = []
         args.append("--dem='{}'".format(dem))
         args.append("--output='{}'".format(output))
         args.append("--threshold={}".format(threshold))
@@ -9182,19 +9201,19 @@
 
         inputs -- Name of the input raster file. 
         output -- Output shapefile. 
         samples -- Number of sample sites returned. 
         iterations -- Maximum iterations (if stopping criteria not reached). 
         seed -- Seed for RNG consistency. 
         prob -- Probability of random resample or resampling worst strata between [0,1]. 
-        threshold -- Objective function values below the theshold stop the resampling iterations. 
+        threshold -- Objective function values below the threshold stop the resampling iterations. 
         temp -- Initial annealing temperature between [0,1]. 
         temp_decay -- Annealing temperature decay proportion between [0,1]. Reduce temperature by this proportion each annealing cycle. 
         cycle -- Number of iterations before decaying annealing temperature. 
-        average -- Weight the continuous objective funtion by the 1/N contributing strata. 
+        average -- Weight the continuous objective function by the 1/N contributing strata. 
         callback -- Custom function for handling tool text outputs.
         """
         args = []
         args.append("--inputs='{}'".format(inputs))
         args.append("--output='{}'".format(output))
         args.append("--samples={}".format(samples))
         args.append("--iterations={}".format(iterations))
@@ -10889,15 +10908,15 @@
         args.append("--d8_pntr='{}'".format(d8_pntr))
         args.append("--streams='{}'".format(streams))
         args.append("--output='{}'".format(output))
         if esri_pntr: args.append("--esri_pntr")
         if zero_background: args.append("--zero_background")
         return self.run_tool('tributary_identifier', args, callback) # returns 1 if error
 
-    def vector_stream_network_analysis(self, streams, dem, output, cutting_height=10.0, snap=0.1, callback=None):
+    def vector_stream_network_analysis(self, streams, output, snap=0.1, callback=None):
         """This tool performs common stream network analysis operations on an input vector stream file.
 
         Keyword arguments:
 
         streams -- Name of the input streams vector file. 
         dem -- Name of the input DEM raster file. 
         output -- Name of the output lines shapefile.
```

### Comparing `whitebox-2.3.1/whitebox.egg-info/PKG-INFO` & `whitebox-2.3.2/whitebox.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: whitebox
-Version: 2.3.1
+Version: 2.3.2
 Summary: An advanced geospatial data analysis platform 
-Home-page: https://github.com/giswqs/whitebox
+Home-page: https://github.com/opengeos/whitebox
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: whitebox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: Click>=6.0
 
 ===============
 whitebox-python
 ===============
 
 .. image:: https://colab.research.google.com/assets/colab-badge.svg
         :target: https://gishub.org/whitebox-colab
@@ -33,45 +34,36 @@
 
 .. image:: https://pepy.tech/badge/whitebox
         :target: https://pepy.tech/project/whitebox
 
 .. image:: https://anaconda.org/conda-forge/whitebox/badges/version.svg
         :target: https://anaconda.org/conda-forge/whitebox
 
-.. image:: https://img.shields.io/travis/giswqs/whitebox-python.svg
-        :target: https://travis-ci.org/giswqs/whitebox-python
-
-.. image:: https://ci.appveyor.com/api/projects/status/a7r1hna30kjbsmk3?svg=true
-        :target: https://ci.appveyor.com/project/giswqs/whitebox-python
-
 .. image:: https://readthedocs.org/projects/whitebox/badge/?version=latest
         :target: https://whitebox.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
         :target: https://opensource.org/licenses/MIT
 
-.. image:: https://img.shields.io/twitter/follow/giswqs?style=social   
-        :target: https://twitter.com/giswqs
-
 .. image:: https://img.shields.io/badge/Donate-Buy%20me%20a%20coffee-yellowgreen.svg
-        :target: https://www.buymeacoffee.com/giswqs
+        :target: https://www.buymeacoffee.com/opengeos
 
 
 Important Note
 --------------
 .. image:: https://i.imgur.com/Ic8BA7C.png
 
 This repository is related to the WhiteboxTools Python Frontend only. You can report issues to this repo if you have problems installing this Python package. If you encounter any tool functioning specific errors, please `open an issue`_ on Dr. John Lindsay's WhiteboxTools_ repo.  
 
 **Links**
 
 * Authors: Dr. John Lindsay (https://jblindsay.github.io/ghrg/index.html)
 * Contributors: Dr. Qiusheng Wu (https://wetlands.io)
-* GitHub repo: https://github.com/giswqs/whitebox-python
+* GitHub repo: https://github.com/opengeos/whitebox-python
 * WhiteboxTools: https://github.com/jblindsay/whitebox-tools
 * User Manual: https://www.whiteboxgeo.com/manual/wbt_book/intro.html
 * PyPI: https://pypi.org/project/whitebox/
 * conda-forge: https://anaconda.org/conda-forge/whitebox
 * Documentation: https://whitebox.readthedocs.io
 * Binder: https://gishub.org/whitebox-cloud
 * Free software: `MIT license`_
@@ -223,44 +215,44 @@
 The WhiteboxTools library currently supports read/writing raster data in Whitebox GAT, GeoTIFF, ESRI (ArcGIS) ASCII and binary (.flt & .hdr), GRASS GIS, Idrisi, SAGA GIS (binary and ASCII), and Surfer 7 data formats. At present, there is limited ability in WhiteboxTools to read vector geospatial data. Support for Shapefile (and other common vector formats) will be enhanced within the library soon. 
 
 Contributing
 ------------
 
 If you would like to contribute to the project as a developer, follow these instructions to get started:
 
-1. Fork the whitebox project (https://github.com/giswqs/whitebox-python)
+1. Fork the whitebox project (https://github.com/opengeos/whitebox-python)
 2. Create your feature branch (git checkout -b my-new-feature)
 3. Commit your changes (git commit -am 'Add some feature')
 4. Push to the branch (git push origin my-new-feature)
 5. Create a new Pull Request
 
 License
 -------
 
 The **whitebox** package is distributed under the `MIT license`_, a permissive open-source (free software) license.
 
 
 Reporting Bugs
 --------------
-Report bugs at https://github.com/giswqs/whitebox-python/issues.
+Report bugs at https://github.com/opengeos/whitebox-python/issues.
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-.. _example.py: https://github.com/giswqs/whitebox/blob/master/whitebox/example.py
+.. _example.py: https://github.com/opengeos/whitebox/blob/master/whitebox/example.py
 .. _WhiteboxTools: https://github.com/jblindsay/whitebox-tools
 .. _webpage: https://jblindsay.github.io/ghrg/index.html
 .. _jblindsay: https://github.com/jblindsay
 .. _`Geomorphometry and Hydrogeomatics Research Group`: https://jblindsay.github.io/ghrg/index.html
 .. _`conda user guide`: https://conda.io/docs/user-guide/install/index.html
 .. _`managing Python environment`: https://conda.io/docs/user-guide/tasks/manage-environments.html
 .. _`WhiteboxTools Usage`: https://github.com/jblindsay/whitebox-tools#3-usage
```

### Comparing `whitebox-2.3.1/whitebox.egg-info/SOURCES.txt` & `whitebox-2.3.2/whitebox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

