# Comparing `tmp/netbox_napalm_plugin-0.2.0.tar.gz` & `tmp/netbox_napalm_plugin-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_napalm_plugin-0.2.0.tar", last modified: Mon May  6 19:35:26 2024, max compression
+gzip compressed data, was "netbox_napalm_plugin-0.2.1.tar", last modified: Fri May 24 13:58:09 2024, max compression
```

## Comparing `netbox_napalm_plugin-0.2.0.tar` & `netbox_napalm_plugin-0.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.557453 netbox_napalm_plugin-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-06 19:35:26.557453 netbox_napalm_plugin-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.553453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.553453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.553453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.549453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.549453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/netbox_napalm_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.553453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/netbox_napalm_plugin/js/
--rw-r--r--   0 runner    (1001) docker     (127)   196388 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/netbox_napalm_plugin/js/config.js
--rw-r--r--   0 runner    (1001) docker     (127)   198227 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/netbox_napalm_plugin/js/lldp.js
--rw-r--r--   0 runner    (1001) docker     (127)   234145 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/netbox_napalm_plugin/js/status.js
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.549453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.557453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.557453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-06 19:35:26.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-06 19:35:26.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:35:26.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-06 19:35:26.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 19:35:26.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:35:26.557453 netbox_napalm_plugin-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.557453 netbox_napalm_plugin-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/tests/test_netbox_napalm_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:58:09.415927 netbox_napalm_plugin-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-24 13:58:09.415927 netbox_napalm_plugin-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:58:09.411927 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:58:09.411927 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:58:09.411927 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:58:09.407927 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:58:09.407927 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/static/netbox_napalm_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:58:09.415927 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/static/netbox_napalm_plugin/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   196427 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/static/netbox_napalm_plugin/js/config.js
+-rw-r--r--   0 runner    (1001) docker     (127)   198266 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/static/netbox_napalm_plugin/js/lldp.js
+-rw-r--r--   0 runner    (1001) docker     (127)   234184 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/static/netbox_napalm_plugin/js/status.js
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:58:09.407927 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:58:09.415927 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:58:09.415927 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-24 13:58:09.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-24 13:58:09.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:58:09.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-24 13:58:09.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 13:58:09.000000 netbox_napalm_plugin-0.2.1/netbox_napalm_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 13:58:09.415927 netbox_napalm_plugin-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:58:09.415927 netbox_napalm_plugin-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-24 13:58:05.000000 netbox_napalm_plugin-0.2.1/tests/test_netbox_napalm_plugin.py
```

### Comparing `netbox_napalm_plugin-0.2.0/CONTRIBUTING.md` & `netbox_napalm_plugin-0.2.1/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 You can contribute in many ways:
 
 ## Types of Contributions
 
 ### Report Bugs
 
-Report bugs at https://github.com/netbox-community/netbox-napalm/issues.
+Report bugs at https://github.com/netbox-community/netbox-napalm-plugin/issues.
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
@@ -31,32 +31,32 @@
 
 NetBox Napalm Plugin could always use more documentation, whether as part of the
 official NetBox Napalm Plugin docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 ### Submit Feedback
 
-The best way to send feedback is to file an issue at https://github.com/netbox-community/netbox-napalm/issues.
+The best way to send feedback is to file an issue at https://github.com/netbox-community/netbox-napalm-plugin/issues.
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that contributions
   are welcome :)
 
 ## Get Started!
 
-Ready to contribute? Here's how to set up `netbox-napalm` for local development.
+Ready to contribute? Here's how to set up `netbox-napalm-plugin` for local development.
 
-1. Fork the `netbox-napalm` repo on GitHub.
+1. Fork the `netbox-napalm-plugin` repo on GitHub.
 2. Clone your fork locally
 
     ```
-    $ git clone git@github.com:your_name_here/netbox-napalm.git
+    $ git clone git@github.com:your_name_here/netbox-napalm-plugin.git
     ```
 
 3. Activate the NetBox virtual environment (see the NetBox documentation under [Setting up a Development Environment](https://docs.netbox.dev/en/stable/development/getting-started/)):
 
     ```
     $ source ~/.venv/netbox/bin/activate
     ```
@@ -92,15 +92,15 @@
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.md.
 3. The pull request should work for Python 3.8, 3.9, 3.10 and 3.11. Check
-   https://github.com/netbox-community/netbox-napalm/actions
+   https://github.com/netbox-community/netbox-napalm-plugin/actions
    and make sure that the tests pass for all supported Python versions.
 
 
 ## Deploying
 
 A reminder for the maintainers on how to deploy.
 Make sure all your changes are committed (including an entry in CHANGELOG.md) and that all tests pass.
```

### Comparing `netbox_napalm_plugin-0.2.0/LICENSE` & `netbox_napalm_plugin-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.2.0/PKG-INFO` & `netbox_napalm_plugin-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-napalm-plugin
-Version: 0.2.0
+Version: 0.2.1
 Summary: NetBox plugin for Napalm.
 Author-email: Arthur Hanson <ahanson@netboxlabs.com>
 Project-URL: Documentation, https://github.com/netbox-community/netbox-napalm-plugin/blob/main/README.md
 Project-URL: Source, https://github.com/netbox-community/netbox-napalm-plugin
 Project-URL: Tracker, https://github.com/netbox-community/netbox-napalm-plugin/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -27,29 +27,30 @@
 
 # NetBox Napalm Plugin
 
 NetBox plugin for Napalm.
 
 
 * Free software: Apache-2.0
-* Documentation: https://netbox-community.github.io/netbox-napalm/.
+* Documentation: https://netbox-community.github.io/netbox-napalm-plugin/.
 
 
 ## Features
 
 The features the plugin provides should be listed here.
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |     3.5        |      0.1.0     |
 |     3.5.8      |      0.1.4     |
 |     3.6.0      |      0.1.5     |
-|     3.7.0      |      0.1.7     |
+|   < 3.7.6      |      0.1.7     |
+|   >= 4.0.2     |      0.2.1     |
 
 ## Installation
 
 For adding to a NetBox Docker setup see
 [the general instructions for using netbox-docker with plugins](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins).
 
 ```no-highlight
```

### Comparing `netbox_napalm_plugin-0.2.0/README.md` & `netbox_napalm_plugin-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # NetBox Napalm Plugin
 
 NetBox plugin for Napalm.
 
 
 * Free software: Apache-2.0
-* Documentation: https://netbox-community.github.io/netbox-napalm/.
+* Documentation: https://netbox-community.github.io/netbox-napalm-plugin/.
 
 
 ## Features
 
 The features the plugin provides should be listed here.
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |     3.5        |      0.1.0     |
 |     3.5.8      |      0.1.4     |
 |     3.6.0      |      0.1.5     |
-|     3.7.0      |      0.1.7     |
+|   < 3.7.6      |      0.1.7     |
+|   >= 4.0.2     |      0.2.1     |
 
 ## Installation
 
 For adding to a NetBox Docker setup see
 [the general instructions for using netbox-docker with plugins](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins).
 
 ```no-highlight
```

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/__init__.py` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for NetBox Napalm Plugin."""
 
 __author__ = """Arthur Hanson"""
 __email__ = "ahanson@netboxlabs.com"
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 
 from netbox.plugins import PluginConfig
 
 
 class NapalmPlatformConfig(PluginConfig):
     name = "netbox_napalm_plugin"
@@ -17,12 +17,12 @@
     author_email = __email__
     base_url = "netbox_napalm_plugin"
     required_settings = ['NAPALM_USERNAME', 'NAPALM_PASSWORD', ]
     default_settings = {
         'NAPALM_TIMEOUT': 30,
         'NAPALM_ARGS': {},
     }
-    min_version = '4.0-beta1'
+    min_version = '4.0.2'
     max_version = '4.0.99'
 
 
 config = NapalmPlatformConfig
```

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/api/serializers.py` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/api/views.py` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/filtersets.py` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/migrations/0001_initial.py` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/models.py` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/models.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/netbox_napalm_plugin/js/config.js` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/static/netbox_napalm_plugin/js/config.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5431,15 +5431,16 @@
         }
     }
 
     function getNetboxData(key) {
         if (!key.startsWith("data-")) {
             key = `data-${key}`;
         }
-        for (const element of getElements("body > div#netbox-data > *")) {
+        var parent_div = document.getElementById("netbox-data");
+        for (const element of parent_div.children) {
             const value = element.getAttribute(key);
             if (isTruthy(value)) {
                 return value;
             }
         }
         return null;
     }
```

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/netbox_napalm_plugin/js/lldp.js` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/static/netbox_napalm_plugin/js/lldp.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5431,15 +5431,16 @@
         }
     }
 
     function getNetboxData(key) {
         if (!key.startsWith("data-")) {
             key = `data-${key}`;
         }
-        for (const element of getElements("body > div#netbox-data > *")) {
+        var parent_div = document.getElementById("netbox-data");
+        for (const element of parent_div.children) {
             const value = element.getAttribute(key);
             if (isTruthy(value)) {
                 return value;
             }
         }
         return null;
     }
```

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/netbox_napalm_plugin/js/status.js` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/static/netbox_napalm_plugin/js/status.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -6270,15 +6270,16 @@
         }
     }
 
     function getNetboxData(key) {
         if (!key.startsWith("data-")) {
             key = `data-${key}`;
         }
-        for (const element of getElements("body > div#netbox-data > *")) {
+        var parent_div = document.getElementById("netbox-data");
+        for (const element of parent_div.children) {
             const value = element.getAttribute(key);
             if (isTruthy(value)) {
                 return value;
             }
         }
         return null;
     }
```

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/tables.py` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html`

 * *Files 4% similar despite different names*

```diff
@@ -34,12 +34,12 @@
                         <pre id="candidate_config"></pre>
                     </div>
                 </div>
             </div>
         </div>
     </div>
 </div>
-{% endblock %}
+<div id="netbox-data" style="display: none!important; visibility: hidden!important">
+    <span data-object-url="{% url 'plugins-api:netbox_napalm_plugin-api:napalmplatformconfig-napalm' pk=object.pk %}?method=get_config"></span>
+</div>
 
-{% block data %}
-<span data-object-url="{% url 'plugins-api:netbox_napalm_plugin-api:napalmplatformconfig-napalm' pk=object.pk %}?method=get_config"></span>
 {% endblock %}
```

#### html2text {}

```diff
@@ -2,8 +2,8 @@
 { object }} - Config{% endblock %} {% block head %}
 {% endblock %} {% block content %}
 Loading...
 **** DDeevviiccee CCoonnffiigguurraattiioonn ****
     * _R_u_n_n_i_n_g
     * _S_t_a_r_t_u_p
     * _C_a_n_d_i_d_a_t_e
-{% endblock %} {% block data %} {% endblock %}
+{% endblock %}
```

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html`

 * *Files 12% similar despite different names*

```diff
@@ -53,12 +53,13 @@
                         <td class="device"></td>
                         <td class="interface"></td>
                     </tr>
                 {% endfor %}
             </tbody>
         </table>
     </div>
+    <div id="netbox-data" style="display: none!important; visibility: hidden!important">
+        <span data-object-url="{% url 'plugins-api:netbox_napalm_plugin-api:napalmplatformconfig-napalm' pk=object.pk %}?method=get_lldp_neighbors_detail"></span>    
+    </div>
 {% endblock %}
 
-{% block data %}
-<span data-object-url="{% url 'plugins-api:netbox_napalm_plugin-api:napalmplatformconfig-napalm' pk=object.pk %}?method=get_lldp_neighbors_detail"></span>
-{% endblock %}
+
```

#### html2text {}

```diff
@@ -3,8 +3,8 @@
 {% endblock %} {% block content %}
 Loading...
 **** LLLLDDPP NNeeiigghhbboorrss ****
 IInntteerrffaaccee   CCoonnffiigguurreedd DDeevviiccee CCoonnffiigguurreedd LLLLDDPP DDeevviiccee LLLLDDPP IInntteerrffaaccee
                               IInntteerrffaaccee
 {{ iface }} _{_{_ _p_e_e_r_._d_e_v_i_c_e_ _}_} {{ peer }} _{_{_ _c_i_r_c_u_i_t_._p_r_o_v_i_d_e_r_ _}_}_ _{   None
                                          _{_ _c_i_r_c_u_i_t_ _}_}
-{% endblock %} {% block data %} {% endblock %}
+{% endblock %}
```

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html`

 * *Files 3% similar despite different names*

```diff
@@ -78,12 +78,13 @@
                     </tr>
                     <tr class="napalm-table-placeholder d-none invisible">
                     </tr>
                 </table>
             </div>
         </div>
     </div>
-{% endblock %}
+<div id="netbox-data" style="display: none!important; visibility: hidden!important">
+  <span data-object-url="{% url 'plugins-api:netbox_napalm_plugin-api:napalmplatformconfig-napalm' pk=object.pk %}?method=get_facts&method=get_environment"></span>
+</div>
 
-{% block data %}
-    <span data-object-url="{% url 'plugins-api:netbox_napalm_plugin-api:napalmplatformconfig-napalm' pk=object.pk %}?method=get_facts&method=get_environment"></span>
 {% endblock %}
+
```

#### html2text {}

```diff
@@ -13,8 +13,8 @@
 Loading...
 **** EEnnvviirroonnmmeenntt ****
 CCPPUU
 MMeemmoorryy
 TTeemmppeerraattuurree
 FFaannss
 PPoowweerr
-{% endblock %} {% block data %} {% endblock %}
+{% endblock %}
```

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/urls.py` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/views.py` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin/views.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin.egg-info/PKG-INFO` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-napalm-plugin
-Version: 0.2.0
+Version: 0.2.1
 Summary: NetBox plugin for Napalm.
 Author-email: Arthur Hanson <ahanson@netboxlabs.com>
 Project-URL: Documentation, https://github.com/netbox-community/netbox-napalm-plugin/blob/main/README.md
 Project-URL: Source, https://github.com/netbox-community/netbox-napalm-plugin
 Project-URL: Tracker, https://github.com/netbox-community/netbox-napalm-plugin/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -27,29 +27,30 @@
 
 # NetBox Napalm Plugin
 
 NetBox plugin for Napalm.
 
 
 * Free software: Apache-2.0
-* Documentation: https://netbox-community.github.io/netbox-napalm/.
+* Documentation: https://netbox-community.github.io/netbox-napalm-plugin/.
 
 
 ## Features
 
 The features the plugin provides should be listed here.
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |     3.5        |      0.1.0     |
 |     3.5.8      |      0.1.4     |
 |     3.6.0      |      0.1.5     |
-|     3.7.0      |      0.1.7     |
+|   < 3.7.6      |      0.1.7     |
+|   >= 4.0.2     |      0.2.1     |
 
 ## Installation
 
 For adding to a NetBox Docker setup see
 [the general instructions for using netbox-docker with plugins](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins).
 
 ```no-highlight
```

### Comparing `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin.egg-info/SOURCES.txt` & `netbox_napalm_plugin-0.2.1/netbox_napalm_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.2.0/pyproject.toml` & `netbox_napalm_plugin-0.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name =  "netbox-napalm-plugin"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     {name = "Arthur Hanson", email = "ahanson@netboxlabs.com"},
 ]
 description = "NetBox plugin for Napalm."
 readme = "README.md"
 
 classifiers=[
```

