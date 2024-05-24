# Comparing `tmp/jupyter_firefly_extensions-4.1.1.tar.gz` & `tmp/jupyter_firefly_extensions-4.2.0.tar.gz`

## Comparing `jupyter_firefly_extensions-4.1.1.tar` & `jupyter_firefly_extensions-4.2.0.tar`

### file list

```diff
@@ -1,61 +1,46 @@
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/.yarnrc.yml
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/License.txt
--rw-r--r--   0        0        0   541440 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/W4 (1).fits
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/conftest.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/install.json
--rwxr-xr-x   0        0        0     2995 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/new-release-procedure.md
--rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/setup.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/tsconfig.json
--rw-r--r--   0        0        0   188187 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/yarn.lock
--rw-r--r--   0        0        0    12786 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/examples/slate-demo-explicit.ipynb
--rw-r--r--   0        0        0    11986 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/examples/slate-demo-explicit2.ipynb
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter-config/server-config/jupyter_firefly_extensions.json
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/_version.py
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/handlers.py
--rw-r--r--   0        0        0    22079 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/build_log.json
--rw-r--r--   0        0        0     5978 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/package.json
--rw-r--r--   0        0        0    67539 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.30945f690cca6de2b14f.js
--rw-r--r--   0        0        0    33304 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.30945f690cca6de2b14f.js.map
--rw-r--r--   0        0        0    68172 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.500e363702a4f528a942.js
--rw-r--r--   0        0        0    34197 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.500e363702a4f528a942.js.map
--rw-r--r--   0        0        0    67539 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.7646a236feb88a665a4b.js
--rw-r--r--   0        0        0    34026 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.7646a236feb88a665a4b.js.map
--rw-r--r--   0        0        0    68653 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.d1c31609190d65e955f6.js
--rw-r--r--   0        0        0    34277 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.d1c31609190d65e955f6.js.map
--rw-r--r--   0        0        0    68172 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.d679203f6e645e4e72b0.js
--rw-r--r--   0        0        0    33714 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.d679203f6e645e4e72b0.js.map
--rw-r--r--   0        0        0    68653 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.eebc69299ba593b23ce5.js
--rw-r--r--   0        0        0    33794 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.eebc69299ba593b23ce5.js.map
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/node_modules_b64-to-blob_b64toBlob_js.c490fc7119beea72c47e.js
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/node_modules_b64-to-blob_b64toBlob_js.c490fc7119beea72c47e.js.map
--rw-r--r--   0        0        0    29694 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.284b55f4388674029ec0.js.map
--rw-r--r--   0        0        0    29475 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.53df49ccb005af25f721.js.map
--rw-r--r--   0        0        0    29694 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.a7d5002bd2d65a12a265.js.map
--rw-r--r--   0        0        0    29694 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.bd0f9e95d8cbaf017e34.js.map
--rw-r--r--   0        0        0    30759 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.d65ffc2462e0ee205d4e.js
--rw-r--r--   0        0        0    29694 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.d65ffc2462e0ee205d4e.js.map
--rw-r--r--   0        0        0    29475 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.f552d540a624c45383fa.js.map
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/style.js
--rw-r--r--   0        0        0    19650 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/style_index_js.1e1ab72bb82b2e804877.js
--rw-r--r--   0        0        0    15207 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/style_index_js.1e1ab72bb82b2e804877.js.map
--rw-r--r--   0        0        0    60655 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js.11d96cd25e15e62dfcc9.js
--rw-r--r--   0        0        0    85321 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js.11d96cd25e15e62dfcc9.js.map
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/tests/__init__.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/tests/test_handlers.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/src/FireflyCommonUtils.js
--rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/src/FitsViewerExt.js
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/src/SlateCommandExt.js
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/src/handler.ts
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/src/index.ts
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/src/svg.d.ts
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/style/base.css
--rw-r--r--   0        0        0    40698 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/style/fftools-logo.svg
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/style/index.js
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/.gitignore
--rwxr-xr-x   0        0        0     4954 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/README.md
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/pyproject.toml
--rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/.eslintrc
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/.yarnrc.yml
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/License.txt
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/conftest.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/install.json
+-rwxr-xr-x   0        0        0     2995 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/new-release-procedure.md
+-rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/setup.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/tsconfig.json
+-rw-r--r--   0        0        0   188187 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/yarn.lock
+-rw-r--r--   0        0        0    12786 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/examples/slate-demo-explicit.ipynb
+-rw-r--r--   0        0        0    11986 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/examples/slate-demo-explicit2.ipynb
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter-config/server-config/jupyter_firefly_extensions.json
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/_version.py
+-rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/handlers.py
+-rw-r--r--   0        0        0    20800 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/build_log.json
+-rw-r--r--   0        0        0     5978 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/package.json
+-rw-r--r--   0        0        0    68268 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/lib_index_js.e8692010c055affebbc6.js
+-rw-r--r--   0        0        0    33207 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/lib_index_js.e8692010c055affebbc6.js.map
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/node_modules_b64-to-blob_b64toBlob_js.c490fc7119beea72c47e.js
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/node_modules_b64-to-blob_b64toBlob_js.c490fc7119beea72c47e.js.map
+-rw-r--r--   0        0        0    30748 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/remoteEntry.309ab0e4582c045c93a0.js
+-rw-r--r--   0        0        0    29681 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/remoteEntry.309ab0e4582c045c93a0.js.map
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/style.js
+-rw-r--r--   0        0        0    19650 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/style_index_js.1e1ab72bb82b2e804877.js
+-rw-r--r--   0        0        0    15207 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/style_index_js.1e1ab72bb82b2e804877.js.map
+-rw-r--r--   0        0        0    60655 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js.11d96cd25e15e62dfcc9.js
+-rw-r--r--   0        0        0    85321 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js.11d96cd25e15e62dfcc9.js.map
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/tests/__init__.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/tests/test_handlers.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/src/FireflyCommonUtils.js
+-rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/src/FitsViewerExt.js
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/src/SlateCommandExt.js
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/src/handler.ts
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/src/index.ts
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/src/svg.d.ts
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/style/base.css
+-rw-r--r--   0        0        0    40698 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/style/fftools-logo.svg
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/style/index.js
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/.gitignore
+-rwxr-xr-x   0        0        0     4954 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/README.md
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.2.0/PKG-INFO
```

### Comparing `jupyter_firefly_extensions-4.1.1/License.txt` & `jupyter_firefly_extensions-4.2.0/License.txt`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/new-release-procedure.md` & `jupyter_firefly_extensions-4.2.0/new-release-procedure.md`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/package.json` & `jupyter_firefly_extensions-4.2.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'4.2.0'"}*

```diff
@@ -190,12 +190,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.1.1",
+    "version": "4.2.0",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `jupyter_firefly_extensions-4.1.1/tsconfig.json` & `jupyter_firefly_extensions-4.2.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/yarn.lock` & `jupyter_firefly_extensions-4.2.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/examples/slate-demo-explicit.ipynb` & `jupyter_firefly_extensions-4.2.0/examples/slate-demo-explicit.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/examples/slate-demo-explicit2.ipynb` & `jupyter_firefly_extensions-4.2.0/examples/slate-demo-explicit2.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/__init__.py` & `jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/handlers.py` & `jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,43 +97,51 @@
 
 
 def setup_handlers(server_app):
     """
     Called when the extension is loaded.
 
     Args:
-        nb_server_app (NotebookWebApplication): handle to the Notebook webserver instance.
+        server_app (NotebookWebApplication): handle to the Notebook webserver instance.
     """
     global firefly_config
     web_app = server_app.web_app
     config_url = server_app.config.get('Firefly', {}).get('url', 'http://localhost:8080/firefly')
     url = None
+    html_file = None
     if 'FIREFLY_URL' in os.environ:
         url = os.environ['FIREFLY_URL']
     if not url:
         url = config_url
 
+    if 'FIREFLY_HTML' in os.environ:
+        html_file = os.environ['FIREFLY_HTML']
+
     web_app.settings['fireflyURL'] = url
+    web_app.settings['fireflyHtmlFile'] = html_file
 
     # page_config = web_app.settings.setdefault('page_config_data', dict())
-    page_config = {'fireflyLabExtension': 'true', 'fireflyURL': url}
+    page_config = {'fireflyLabExtension': 'true', 'fireflyURL': url, 'fireflyHtmlFile': html_file}
     # for key,val in web_app.settings.items():
     #     print('{} => {}'.format(key,val))
 
     hostname = platform.node()
     timestamp = time.time()
     channel = 'ffChan-{}-{}-{}'.format(hostname, int(timestamp), random.randint(1, 100))
     page_config['fireflyChannel'] = channel
     logger.info('firefly URL: {}'.format(url))
+    logger.info('firefly HTML File: {}'.format('not defined' if not html_file else html_file))
     logger.info('firefly Channel: {}'.format(channel))
-    # added next two lines because logger does not seem to work JL 3.5
+    # added the next three lines because logger does not seem to work JL 3.5
     print('firefly URL: {}'.format(url))
     print('firefly Channel: {}'.format(channel))
+    print('firefly HTML File: {}'.format('not defined' if not html_file else html_file))
     os.environ['fireflyChannelLab'] = channel
     os.environ['fireflyURLLab'] = url
+    os.environ['fireflyHtmlFile'] = '' if not html_file else html_file
     os.environ['fireflyLabExtension'] = 'true'
     firefly_config = dict(page_config)
 
     # setup server endpoint: sendToFirefly: http://127.0.0.1:8888/lab/sendToFirefly?path=x.fits
     host_pattern = '.*$'
     send_pattern = url_path_join(web_app.settings['base_url'], 'lab/sendToFirefly')
     get_ff_data_pattern = url_path_join(web_app.settings['base_url'], 'lab/fireflyLocation')
```

### Comparing `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/build_log.json` & `jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/build_log.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998676818094135%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'@jupyterlab/application': {'requiredVersion': "*

 * *      "'^4.0.5'}, '@jupyterlab/application-extension': {'requiredVersion': '^4.0.5'}, "*

 * *      "'@jupyterlab/apputils-extension': {'requiredVersion': '^4.0.5'}, "*

 * *      "'@jupyterlab/cell-toolbar-extension': {'requiredVersion': '^4.0.5'}, "*

 * *      "'@jupyterlab/celltags-extension': {'requiredVersion': '^4.0.5'}, "*

 * *      "'@jupyterlab/codemirror-extension': {'requiredVersion': '^4.0.5'}, "*

 * *      "'@jupyterlab/compl […]*

```diff
@@ -129,446 +129,418 @@
                             "singleton": true
                         },
                         "@codemirror/view": {
                             "import": false,
                             "requiredVersion": "^6.9.6",
                             "singleton": true
                         },
-                        "@jupyter/react-components": {
-                            "import": false,
-                            "requiredVersion": "^0.13.3",
-                            "singleton": true
-                        },
-                        "@jupyter/web-components": {
-                            "import": false,
-                            "requiredVersion": "^0.13.3",
-                            "singleton": true
-                        },
                         "@jupyter/ydoc": {
                             "import": false,
-                            "requiredVersion": "^1.1.1",
+                            "requiredVersion": "^1.0.2",
                             "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^4.2.6",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/cell-toolbar": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/cell-toolbar-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^6.1.6",
+                            "requiredVersion": "^6.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/lsp": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/lsp-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/markedparser-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/mathjax-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
-                        },
-                        "@jupyterlab/mermaid": {
-                            "import": false,
-                            "requiredVersion": "^4.1.6",
-                            "singleton": true
-                        },
-                        "@jupyterlab/mermaid-extension": {
-                            "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/metadataform": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/metadataform-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^5.1.6"
+                            "requiredVersion": "^5.0.5"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
-                        },
-                        "@jupyterlab/pluginmanager": {
-                            "import": false,
-                            "requiredVersion": "^4.1.6",
-                            "singleton": true
-                        },
-                        "@jupyterlab/pluginmanager-extension": {
-                            "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.9.6",
+                            "requiredVersion": "^3.8.5",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^7.1.6",
+                            "requiredVersion": "^7.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^6.1.6",
+                            "requiredVersion": "^6.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^6.1.6"
+                            "requiredVersion": "^6.0.5"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^4.1.6",
+                            "requiredVersion": "^4.0.5",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.6"
+                            "requiredVersion": "^4.0.5"
                         },
                         "@lezer/common": {
                             "import": false,
                             "requiredVersion": "^1.0.0",
                             "singleton": true
                         },
                         "@lezer/highlight": {
@@ -579,30 +551,30 @@
                         "@lumino/algorithm": {
                             "import": false,
                             "requiredVersion": "^2.0.0",
                             "singleton": true
                         },
                         "@lumino/application": {
                             "import": false,
-                            "requiredVersion": "^2.3.0-alpha.0",
+                            "requiredVersion": "^2.0.1",
                             "singleton": true
                         },
                         "@lumino/commands": {
                             "import": false,
                             "requiredVersion": "^2.0.1",
                             "singleton": true
                         },
                         "@lumino/coreutils": {
                             "import": false,
                             "requiredVersion": "^2.0.0",
                             "singleton": true
                         },
                         "@lumino/datagrid": {
                             "import": false,
-                            "requiredVersion": "^2.3.0-alpha.0",
+                            "requiredVersion": "^2.0.1",
                             "singleton": true
                         },
                         "@lumino/disposable": {
                             "import": false,
                             "requiredVersion": "^2.0.0",
                             "singleton": true
                         },
@@ -644,33 +616,23 @@
                         "@lumino/virtualdom": {
                             "import": false,
                             "requiredVersion": "^2.0.0",
                             "singleton": true
                         },
                         "@lumino/widgets": {
                             "import": false,
-                            "requiredVersion": "^2.3.1-alpha.0",
-                            "singleton": true
-                        },
-                        "@microsoft/fast-element": {
-                            "import": false,
-                            "requiredVersion": "^1.12.0",
-                            "singleton": true
-                        },
-                        "@microsoft/fast-foundation": {
-                            "import": false,
-                            "requiredVersion": "^2.49.2",
+                            "requiredVersion": "^2.0.1",
                             "singleton": true
                         },
                         "b64-to-blob": {},
                         "firefly-api-access": {},
                         "jupyter_firefly_extensions": {
                             "import": "/Users/jsinghal/dev/cm/jupyter_firefly_extensions/lib/index.js",
                             "singleton": true,
-                            "version": "4.1.0"
+                            "version": "5.0.0"
                         },
                         "lodash": {},
                         "react": {
                             "import": false,
                             "requiredVersion": "^18.2.0",
                             "singleton": true
                         },
```

### Comparing `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/package.json` & `jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9795833333333333%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.309ab0e4582c045c93a0.js'}}",*

 * * "'version'": "'5.0.0'"}*

```diff
@@ -110,15 +110,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/Caltech-IPAC/jupyter_firefly_extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.d65ffc2462e0ee205d4e.js",
+            "load": "static/remoteEntry.309ab0e4582c045c93a0.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_firefly_extensions"
                 },
@@ -195,12 +195,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.1.0",
+    "version": "5.0.0",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.30945f690cca6de2b14f.js` & `jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/lib_index_js.e8692010c055affebbc6.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -21,14 +21,19 @@
                     makeLabEndpoint: () => ( /* binding */ makeLabEndpoint)
                     /* harmony export */
                 });
                 /* harmony import */
                 var firefly_api_access__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! firefly-api-access */ "webpack/sharing/consume/default/firefly-api-access/firefly-api-access");
                 /* harmony import */
                 var firefly_api_access__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(firefly_api_access__WEBPACK_IMPORTED_MODULE_0__);
+                /* harmony import */
+                var _jupyterlab_services__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! @jupyterlab/services */ "webpack/sharing/consume/default/@jupyterlab/services");
+                /* harmony import */
+                var _jupyterlab_services__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_services__WEBPACK_IMPORTED_MODULE_1__);
+
 
                 let cachedLoc;
                 let cachedFindFireflyResult;
                 const ffLocURL = makeLabEndpoint('lab/fireflyLocation');
                 const fetchOptions = {
                     method: 'get',
                     mode: 'cors',
@@ -44,41 +49,54 @@
                  * @return {Promise<{firefly: Object, channel: string, fireflyURL: string}>}
                  */
                 async function findFirefly() {
                     var _a;
                     if (cachedFindFireflyResult)
                         return cachedFindFireflyResult;
                     try {
+                        // request the config from server at /lab/fireflyLocation (see handlers.py)
+                        const settings = _jupyterlab_services__WEBPACK_IMPORTED_MODULE_1__.ServerConnection.makeSettings();
                         if (!cachedLoc)
-                            cachedLoc = await (await fetch(ffLocURL, fetchOptions)).json();
+                            cachedLoc = await (await _jupyterlab_services__WEBPACK_IMPORTED_MODULE_1__.ServerConnection.makeRequest(ffLocURL, fetchOptions, settings)).json();
+                        // make sure that response of the above request contains non-empty fireflyURL
                         const {
-                            fireflyURL = 'http://localhost:8080/firefly', fireflyChannel: channel
+                            fireflyURL,
+                            fireflyChannel: channel,
+                            fireflyHtmlFile
                         } = cachedLoc;
+                        if (!fireflyURL)
+                            throw new Error(`fireflyURL couldn't be retrieved from ${ffLocURL}`);
+                        // load firefly API from fireflyURL at /lab (window)
+                        // (CORS errors might happen here if headers aren't set up correctly, maybe due to caching)
                         if (!((_a = window.firefly) === null || _a === void 0 ? void 0 : _a.initialized))
                             window.firefly = {
                                 ...window.firefly,
                                 wsch: channel
                             };
                         if (!window.getFireflyAPI)
                             window.getFireflyAPI = (0, firefly_api_access__WEBPACK_IMPORTED_MODULE_0__.initFirefly)(fireflyURL);
                         const firefly = await window.getFireflyAPI();
+                        // resolve Promise
                         cachedFindFireflyResult = {
                             fireflyURL,
                             channel,
-                            firefly
+                            firefly,
+                            fireflyHtmlFile
                         };
+                        console.log('Firefly loaded successfully\n', cachedFindFireflyResult);
                         return cachedFindFireflyResult;
                     } catch (e) {
+                        // log information about error(s) before rejecting Promise
                         console.group('Firefly Load Failed');
                         console.log('findFirefly: Could not determine firefly location or load firefly, call failed');
-                        console.log(`find firefly url: ${ffLocURL}`);
                         if (cachedLoc)
-                            console.log(`firefly url: ${cachedLoc.fireflyURL} channel: ${cachedLoc.channel}`);
+                            console.log(`firefly url: ${cachedLoc.fireflyURL} channel: ${cachedLoc.fireflyChannel}`);
                         console.log(e);
                         console.groupEnd('Firefly Load Failed');
+                        throw e; // to let promise reject
                     }
                 }
 
                 function buildURLErrorHtml(e) {
                     const details = `<br>Set the firefly URL by setting <code>c.Firefly.url</code> in 
                     <code>jupyter_notebook_config.py</code>
                     <br>or the environment variable <code>FIREFLY_URL</code>`;
@@ -458,132 +476,112 @@
 
 
 
 
 
 
                 let widgetId;
-                let widgetCnt = 1;
-                let openWidgets = {};
                 /**
                  * Extension can be started in two ways.
                  * 1. as a jupyter command
                  * 2. firefly_client sending a 'StartLabWindow' action
                  * @param {JupyterFrontEnd} app
                  * @param {ICommandPalette} palette
                  * @param {ILauncher | null} launcher
                  */
                 function activateSlateCommandExt(app, palette, launcher) {
                     (0, _FireflyCommonUtils_js__WEBPACK_IMPORTED_MODULE_5__.findFirefly)().then((ffConfig) => {
                         const {
                             firefly
                         } = ffConfig;
-                        firefly.util.addActionListener(['StartLabWindow'], (action, state) => {
-                            openSlateMulti(app, action.payload.renderTreeId, false);
+                        firefly.util.addActionListener(['StartLabWindow'], (action) => {
+                            var _a;
+                            openSlateSingleOnly(app, undefined, (_a = action.payload) === null || _a === void 0 ? void 0 : _a.fireflyHtmlFile);
                         });
-                        firefly.util.addActionListener(['StartBrowserTab'], (action, state) => {
+                        firefly.util.addActionListener(['StartBrowserTab'], (action) => {
                             firefly.setViewerConfig(firefly.ViewerType.Grid);
                             firefly.getViewer(action.payload.channel).openViewer();
                         });
                     });
                     // for starting extension as a jupyter command -----------
                     const command = 'firefly:open-slate';
                     const category = 'Firefly';
                     const icon = new _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_4__.LabIcon({
                         name: 'jupyter_firefly_extensions:firefly-icon',
                         svgstr: _style_fftools_logo_svg__WEBPACK_IMPORTED_MODULE_6__
                     });
                     app.commands.addCommand(command, {
                         label: 'Open Firefly',
                         caption: 'Open Firefly',
-                        icon: icon,
+                        icon,
                         isEnabled: () => true,
                         execute: () => {
-                            const id = 'slate-' + widgetCnt;
-                            widgetCnt++;
-                            openSlateMulti(app, id, true);
+                            openSlateSingleOnly(app);
                         }
                     });
                     palette.addItem({
                         command,
                         category
                     });
                     if (launcher)
                         launcher.add({
                             command,
                             category
                         });
                 }
-
-                function openSlateMulti(app, id, activate) {
-                    activate = window.document.getElementById(id) || activate;
-                    if (!openWidgets[id]) {
-                        let widget = new SlateRootWidget(id);
+                /**
+                 * Open only one slate tab.  Using this keeps the tab as a singleton.
+                 * @param app
+                 * @param id
+                 * @param firelfyHtmlFile
+                 */
+                function openSlateSingleOnly(app, id, firelfyHtmlFile) {
+                    if (!widgetId) {
+                        const widget = new SlateRootWidget('slate-1', firelfyHtmlFile);
+                        widgetId = widget.id;
                         if (app.shell.addToMainArea)
                             app.shell.addToMainArea(widget); // --- pre version 1
                         else if (app.shell.add)
                             app.shell.add(widget, 'main'); // version 1
                         else
                             throw Error('Could not add firefly to tab');
                         (0, _FireflyCommonUtils_js__WEBPACK_IMPORTED_MODULE_5__.findFirefly)().then((ffConfig) => {
                             const {
                                 action
                             } = ffConfig.firefly;
                             action.dispatchChangeActivePlotView(undefined);
                         });
-                        openWidgets[id] = widget;
                     }
-                    if (activate)
-                        app.shell.activateById(id);
-                }
-                /**
-                 * Open only one slate tab.  Using this funtion keeps the slate tab as a singleton.
-                 *
-                 * Currently not used.
-                 * @param app
-                 */
-                function openSlateSingleOnly(app) {
-                    if (!widgetId) {
-                        let widget = new SlateRootWidget('slate-1');
-                        app.shell.addToMainArea(widget);
-                        widgetId = widget.id;
-                        (0, _FireflyCommonUtils_js__WEBPACK_IMPORTED_MODULE_5__.findFirefly)().then((ffConfig) => {
-                            const {
-                                action
-                            } = ffConfig.firefly;
-                            action.dispatchChangeActivePlotView(undefined);
-                        });
-                    } else {}
                     app.shell.activateById(widgetId);
                 }
                 class SlateRootWidget extends _lumino_widgets__WEBPACK_IMPORTED_MODULE_0__.Widget {
                     /**
                      * Construct a new output widget.
                      */
-                    constructor(id) {
+                    constructor(id, fireflyHtmlFile) {
                         super({
                             node: createNode(id)
                         });
                         this.id = id;
-                        this.title.label = 'Firefly: ' + id;
+                        this.title.label = 'Firefly Viewer';
                         this.title.closable = true;
                         (0, _FireflyCommonUtils_js__WEBPACK_IMPORTED_MODULE_5__.findFirefly)().then((ffConfig) => {
-                            this.startViewer(ffConfig.firefly, id, ffConfig.fireflyURL);
+                            this.startViewer(ffConfig.firefly, id, ffConfig.fireflyURL, fireflyHtmlFile !== null && fireflyHtmlFile !== void 0 ? fireflyHtmlFile : ffConfig.fireflyHtmlFile);
                         });
                     }
-                    startViewer(firefly, id, fireflyURL) {
+                    startViewer(firefly, id, fireflyURL, fireflyHtmlFile) {
                         var _a;
                         const {
                             util,
                             action
                         } = firefly;
                         const props = {
                             div: id,
                             renderTreeId: id,
-                            template: 'FireflySlate',
+                            template: fireflyHtmlFile === 'slate.html' ? 'FireflySlate' : 'FireflyViewer',
                             disableDefaultDropDown: true,
                         };
                         const fallbackMenu = [{
                             label: 'Images',
                             action: 'ImageSelectDropDownSlateCmd'
                         }, {
                             label: 'TAP Searches',
@@ -617,15 +615,14 @@
                     }
                     dispose() {
                         widgetId = undefined;
                     }
                     close() {
                         super.close();
                         widgetId = undefined;
-                        delete openWidgets[this.id];
                         if (this.controlApp)
                             this.controlApp.unrender();
                         this.controlApp = undefined;
                     }
                     activate() {
                         super.activate();
                         if (this.controlApp) {
@@ -727,8 +724,8 @@
                 module.exports = "<svg xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 128 128\">\n    <!-- base64-encoded 128x128 png image of firefly logo\n    (in future, replace it with vector paths which can scale)  -->\n    <image width=\"128\" height=\"128\" href=\"data:image/png;base64,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\"/>\n</svg>";
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.30945f690cca6de2b14f.js.map
+//# sourceMappingURL=lib_index_js.e8692010c055affebbc6.js.map
```

### Comparing `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.30945f690cca6de2b14f.js.map` & `jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/lib_index_js.e8692010c055affebbc6.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8095238095238094%*

 * *Differences: {"'file'": "'lib_index_js.e8692010c055affebbc6.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;;;AAA+C;AACS;AAGxD,IAAI,SAAS,CAAC;AACd,IAAI,uBAAuB,CAAC;AAC5B,MAAM,QAAQ,GAAE,eAAe,CAAC,qBAAqB,CAAC,CAAC;AACvD,MAAM,YAAY,GAAE;IAChB,MAAM,EAAE,KAAK;IACb,IAAI,EAAE,MAAM;IACZ,WAAW,EAAE,SAAS;IACtB,KAAK,EAAE,SAAS;IAChB,OAAO,EAAE,EAAE,kBAAkB,EAAE,gBAAgB,EAAE;CACpD,CAAC;AAEF;;;;GAIG;AACI,KAAK,UAAU,WAAW;;IAC7B,IAAI,uBAAuB;QAAE,OAAO,uBAAuB,CAAC;IAE5D,IAAI;QACA,2EAA2E;QAC3E,MAAM,QAAQ,GAAG,kEAAgB,CAAC,YAAY,EAAE,CAAC;QACjD,IAAI,CAAC,S […]*

```diff
@@ -1,19 +1,19 @@
 {
-    "file": "lib_index_js.30945f690cca6de2b14f.js",
-    "mappings": "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",
+    "file": "lib_index_js.e8692010c055affebbc6.js",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter_firefly_extensions/./src/FireflyCommonUtils.js",
         "webpack://jupyter_firefly_extensions/./src/FitsViewerExt.js",
         "webpack://jupyter_firefly_extensions/./src/SlateCommandExt.js",
         "webpack://jupyter_firefly_extensions/./src/index.ts"
     ],
     "sourcesContent": [
-        "import {initFirefly} from 'firefly-api-access';\n\n\nlet cachedLoc;\nlet cachedFindFireflyResult;\nconst ffLocURL= makeLabEndpoint('lab/fireflyLocation');\nconst fetchOptions= {\n    method: 'get',\n    mode: 'cors',\n    credentials: 'include',\n    cache: 'default',\n    headers: { 'X-Requested-With': 'XMLHttpRequest' }\n};\n\n/**\n * Determine where firefly is my calling the lab server extension then load firefly.\n * Results are cache so this function can be call many times.\n * @return {Promise<{firefly: Object, channel: string, fireflyURL: string}>}\n */\nexport async function findFirefly()  {\n    if (cachedFindFireflyResult) return cachedFindFireflyResult;\n\n    try {\n        if (!cachedLoc) cachedLoc= await (await fetch(ffLocURL, fetchOptions)).json();\n\n        const {fireflyURL='http://localhost:8080/firefly', fireflyChannel:channel}= cachedLoc;\n        if (!window.firefly?.initialized) window.firefly= {...window.firefly, wsch:channel};\n        if (!window.getFireflyAPI) window.getFireflyAPI= initFirefly(fireflyURL);\n        const firefly= await window.getFireflyAPI();\n        cachedFindFireflyResult= {fireflyURL, channel, firefly};\n        return cachedFindFireflyResult;\n    }\n    catch (e) {\n        console.group('Firefly Load Failed');\n        console.log('findFirefly: Could not determine firefly location or load firefly, call failed');\n        console.log(`find firefly url: ${ffLocURL}`);\n        if (cachedLoc) console.log(`firefly url: ${cachedLoc.fireflyURL} channel: ${cachedLoc.channel}`);\n        console.log(e);\n        console.groupEnd('Firefly Load Failed');\n    }\n\n}\n\n\n\nexport function buildURLErrorHtml(e) {\n    const details= `<br>Set the firefly URL by setting <code>c.Firefly.url</code> in \n                    <code>jupyter_notebook_config.py</code>\n                    <br>or the environment variable <code>FIREFLY_URL</code>`;\n    return `<div style='padding: 30px 0 0 30px'>${e.message}${details}</div>`;\n}\n\n\nexport function makeLabEndpoint(endPoint, searchParams) {\n    const {origin,pathname}= new URL(window.document.location.href);\n    const originURL= origin + pathname;\n    const start= originURL.substring(0, originURL.lastIndexOf('lab'))\n    const slashMaybe= start.endsWith('/') ? '' : '/';\n    return `${start}${slashMaybe}${endPoint}${searchParams?'?'+searchParams.toString():''}`\n}",
+        "import {initFirefly} from 'firefly-api-access';\nimport { ServerConnection } from '@jupyterlab/services';\n\n\nlet cachedLoc;\nlet cachedFindFireflyResult;\nconst ffLocURL= makeLabEndpoint('lab/fireflyLocation');\nconst fetchOptions= {\n    method: 'get',\n    mode: 'cors',\n    credentials: 'include',\n    cache: 'default',\n    headers: { 'X-Requested-With': 'XMLHttpRequest' }\n};\n\n/**\n * Determine where firefly is my calling the lab server extension then load firefly.\n * Results are cache so this function can be call many times.\n * @return {Promise<{firefly: Object, channel: string, fireflyURL: string}>}\n */\nexport async function findFirefly()  {\n    if (cachedFindFireflyResult) return cachedFindFireflyResult;\n\n    try {\n        // request the config from server at /lab/fireflyLocation (see handlers.py)\n        const settings = ServerConnection.makeSettings();\n        if (!cachedLoc) cachedLoc= await (await ServerConnection.makeRequest(ffLocURL, fetchOptions, settings)).json();\n\n        // make sure that response of the above request contains non-empty fireflyURL\n        const {fireflyURL, fireflyChannel:channel, fireflyHtmlFile}= cachedLoc;\n        if (!fireflyURL) throw new Error(`fireflyURL couldn't be retrieved from ${ffLocURL}`);\n\n        // load firefly API from fireflyURL at /lab (window)\n        // (CORS errors might happen here if headers aren't set up correctly, maybe due to caching)\n        if (!window.firefly?.initialized) window.firefly= {...window.firefly, wsch:channel};\n        if (!window.getFireflyAPI) window.getFireflyAPI= initFirefly(fireflyURL);\n        const firefly= await window.getFireflyAPI();\n\n        // resolve Promise\n        cachedFindFireflyResult= {fireflyURL, channel, firefly, fireflyHtmlFile};\n        console.log('Firefly loaded successfully\\n', cachedFindFireflyResult);\n        return cachedFindFireflyResult;\n    }\n    catch (e) {\n        // log information about error(s) before rejecting Promise\n        console.group('Firefly Load Failed');\n        console.log('findFirefly: Could not determine firefly location or load firefly, call failed');\n        if (cachedLoc) console.log(`firefly url: ${cachedLoc.fireflyURL} channel: ${cachedLoc.fireflyChannel}`);\n        console.log(e);\n        console.groupEnd('Firefly Load Failed');\n        throw e;  // to let promise reject\n    }\n\n}\n\n\n\nexport function buildURLErrorHtml(e) {\n    const details= `<br>Set the firefly URL by setting <code>c.Firefly.url</code> in \n                    <code>jupyter_notebook_config.py</code>\n                    <br>or the environment variable <code>FIREFLY_URL</code>`;\n    return `<div style='padding: 30px 0 0 30px'>${e.message}${details}</div>`;\n}\n\n\nexport function makeLabEndpoint(endPoint, searchParams) {\n    const {origin,pathname}= new URL(window.document.location.href);\n    const originURL= origin + pathname;\n    const start= originURL.substring(0, originURL.lastIndexOf('lab'));\n    const slashMaybe= start.endsWith('/') ? '' : '/';\n    return `${start}${slashMaybe}${endPoint}${searchParams?'?'+searchParams.toString():''}`;\n}",
         "import b64toBlob from 'b64-to-blob';\nimport {buildURLErrorHtml, findFirefly, makeLabEndpoint} from './FireflyCommonUtils.js';\nimport { Widget } from '@lumino/widgets';\nimport { ABCWidgetFactory, DocumentWidget} from '@jupyterlab/docregistry';\nimport { PageConfig} from '@jupyterlab/coreutils';\n\n\nexport const FITS_MIME_TYPE = 'application/fits';\n\n\n/**\n * The class name added to the extension.\n */\nconst CLASS_NAME = 'jp-OutputWidgetFITS';\n\nlet idCounter=0;\n\nconst FACTORY = 'FITS-IMAGE';\n\n\nconst fitsIFileType= {\n    name: 'FITS',\n    displayName: 'FITS file',\n    fileFormat: 'base64',  // TODO: try putting a null here to keep from loading file, the might be the answer\n                           // will need to check the JL version someway\n    format: 'base64',\n    mimeTypes: [FITS_MIME_TYPE],\n    extensions: ['.fits']\n};\n\n/**\n *\n * @param {JupyterLab} app\n * @param {ILayoutRestorer} restorer\n */\nexport function activateFitsViewerExt(app, restorer) {\n    const namespace = 'firefly-imageviewer-widget';\n    const jlVersion= PageConfig.getOption('appVersion');\n    const vAry= jlVersion?.split('.').map( (x) => Number(x)) ?? [0,0,0];\n\n    // if Jupyter Lab version is 3.1 or greater then clear the fileFormat so it does not load the file on the client\n    // see - https://github.com/jupyterlab/jupyterlab/pull/7596\n    if (vAry[0] >=3 && vAry[1] >= 1) fitsIFileType.fileFormat= null;\n\n    app.docRegistry.addFileType(fitsIFileType);\n    const factory = new ABCWidgetFactory({\n        name: FACTORY,\n        modelName: 'base64',\n        // modelName: 'fits-model',\n        fileTypes: ['FITS'],\n        defaultFor: ['FITS'],\n        readOnly: true\n    });\n    factory.createNewWidget= createNewFitsViewerDocumentWidget;\n    app.docRegistry.addWidgetFactory(factory);\n\n    factory.widgetCreated.connect((sender, widget) => {\n        const types = app.docRegistry.getFileTypesForPath(widget.context.path);\n\n        if (types.length) {\n            widget.title.iconClass = types[0].iconClass || '';\n            widget.title.iconLabel = types[0].iconLabel || '';\n        }\n    });\n}\n\n\n\n\n\nexport function createNewFitsViewerDocumentWidget(context) {\n    // instead of extending DocumentWidget like the example, just use it directly\n    return new DocumentWidget({ content:new FitsViewerWidget(context), context, reveal:true, toolbar:null });\n}\n\n/**\n * A widget for rendering FITS.\n */\nexport class FitsViewerWidget extends Widget {\n    /**\n     * Construct a new output widget.\n     * @param context\n     */\n    constructor(context) {\n        super({ node: createNode(context._path) });\n        const useModel= window.firefly && window.firefly.jlExtUseModel || false;\n        this.addClass(CLASS_NAME);\n        this.filename= context._path;\n        idCounter++;\n        this.plotId= `${this.filename}-${idCounter}`;\n        this.loaded= false;\n        if (this.isDisposed) return;\n        this.renderModel(context,useModel).then(() => {\n        });\n        context.model.contentChanged.connect( this.renderModel, this );\n        context.fileChanged.connect( this.renderModel, this );\n    }\n\n    /**\n     * Render FITS into this widget's node.\n     * @param context\n     * @param useModelFirst\n     * @return {Promise<{firefly: Object, channel: string, fireflyURL: string}>}\n     */\n    renderModel(context, useModelFirst) {\n\n        if (this.isDisposed) return;\n\n        if (this.loaded) {\n            return findFirefly()\n                .then( (ffConfig) => ffConfig.firefly.action.dispatchChangeActivePlotView(this.plotId) );\n        }\n\n        let firefly, fireflyURL;\n        return findFirefly()\n            .then( (ffConfig) => {\n                firefly= ffConfig.firefly;\n                fireflyURL= ffConfig.fireflyURL;\n                if (useModelFirst) {\n                    return context.ready.then(() => loadFileToServer(context.model.toString(), this.filename, firefly, fireflyURL));\n                }\n                else {\n                    return tellLabToLoadFileToServer(this.filename, firefly);\n                }\n            } )\n            .then( (response) => response.text())\n            .then( (text) => {\n                if (useModelFirst) {\n                    const [, cacheKey] = text.split('::::');\n                    showImage(cacheKey,this.plotId, this.filename, firefly);\n                }\n                else {\n                    if (text && text.length<300 && text.startsWith('${')) {\n                        showImage(text,this.plotId, this.filename, firefly);\n                    }\n                    else {\n                        console.log('Firefly FitsViewExt: Failed to upload from server, ' +\n                                          'falling back to (slower) browser upload.');\n                        context.ready.then(() => loadFileToServer(context.model.toString(), this.filename, firefly, fireflyURL))\n                            .then( (response) => response.text())\n                            .then( (text) => {\n                                const [, cacheKey] = text.split('::::');\n                                showImage(cacheKey, this.plotId, this.filename, firefly);\n                            });\n                    }\n                }\n                this.loaded= true;\n            })\n            .catch( (e) => {\n                const div= document.getElementById(this.filename);\n                if (div) div.innerHTML=buildURLErrorHtml(e);\n            });\n    }\n\n    dispose() {\n        return findFirefly()\n            .then( (ffConfig) => ffConfig.firefly.action.dispatchDeletePlotView({plotId:this.plotId, holdWcsMatch:true}) );\n\n    }\n\n    activate() {\n        super.activate();\n        if (this.loaded) {\n            return findFirefly().then( (ffConfig) => ffConfig.firefly.action.dispatchChangeActivePlotView(this.plotId) );\n        }\n    }\n}\n\n\nfunction tellLabToLoadFileToServer( path, firefly) {\n    const url= makeLabEndpoint('lab/sendToFirefly', new URLSearchParams({'path':path}));\n    return firefly.util.fetchUrl(url,{ method: 'GET' },false, false)\n        .catch( (e) => {\n            console.error('Firefly FitsViewExt: Got Error from upload request',e);\n            return 'FAILED';\n        });\n}\n\n\nfunction loadFileToServer( fileData, filename, firefly, fireflyURL) {\n    const {fetchUrl, ServerParams}= firefly.util;\n    const UL_URL = `${fireflyURL}/sticky/CmdSrv?${ServerParams.COMMAND}=${ServerParams.UPLOAD}&filename=${filename}`;\n    const fitsBlob= b64toBlob(fileData);\n    const options = { method: 'multipart', params: { filename, type:'FITS', file: fitsBlob } };\n    return fetchUrl(UL_URL, options);\n}\n\nfunction showImage(cacheKey, plotId, filename, firefly) {\n    const req= {\n        type     : 'FILE',\n        FILE     : cacheKey,\n        plotId,\n        plotGroupId: 'JUPLAB',\n        title: filename\n    };\n    firefly.action.dispatchApiToolsView(true, false);\n    firefly.setGlobalPref({imageDisplayType: 'encapusulate'});\n    firefly.showImage(filename, req, null, false);\n}\n\nfunction createNode(filename) {\n    const node = document.createElement('div');\n    node.id= filename;\n    return node;\n}\n\n//=========================================================================================================\n//============ Keep code below for reference\n//============ Keep code below for reference\n//============ Keep code below for reference\n\n\n// /**\n//  * A mime renderer factory for FITS data.\n//  */\n// export const fitsViewerRendererFactory = {\n//     safe: true,\n//     mimeTypes: [FITS_MIME_TYPE],\n//     createRenderer: options => {\n//         return new FitsViewerWidget (options);\n//     }\n// };\n\n\n\n// import { ABCWidgetFactory, DocumentRegistry, DocumentWidget, IDocumentWidget } from '@jupyterlab/docregistry';\n// import { PageConfig, URLExt } from '@jupyterlab/coreutils';\n\n\n// const ERROR_MSG_CONT= `Make sure you set the firefly URL in your jupyter_notebook_config.py.\n//                 For example- 'c.Firefly.url= http://some.firefly.url/firefly'`;\n\n// for adding a second extension for a mime type - does not work yet in Jupyter Lab\n// --- https://github.com/jupyterlab/jupyterlab/issues/5381\n// export const fitsViewerRendererFactory2 = {\n//     safe: true,\n//     mimeTypes: [FITS_MIME_TYPE],\n//     createRenderer: options => {\n//         return new FitsViewerWidget (options);\n//     }\n// };\n\n\n// export class FitsViewerDocument extends DocumentWidget {\n//\n//   constructor(context) {\n//       super({ content:new FitsViewerWidget(context), context, reveal:true, toolbar:null });\n//     // const toolbar = Private.createToolbar(content.viewer);\n//     // const reveal = content.ready;\n//   }\n// }\n\n\n// export class FitsViewerFactory extends ABCWidgetFactory {\n//\n//     constructor(options) {\n//         super(options);\n//     }\n//\n//\n//\n//     /**\n//      * Create a new widget given a context.\n//      * @param context DocumentRegistry.IContext<DocumentRegistry.IModel>\n//      * @return DocumentWidget\n//      */\n//     createNewWidget(context) {\n//         // return new FitsViewerDocument(context);\n//         return new DocumentWidget({ content:new FitsViewerWidget(context), context, reveal:true, toolbar:null });\n//     }\n// }\n\n\n// const a= {\n//     name: 'some-name',\n//     fileTypes: ['csv'],\n//     defaultFor: [],\n//     defaultRendered: [],\n//     readOnly: false,\n//     modelName: 'text',\n//     preferKernel: false,\n//     canStartKernel: false,\n//     widgetCreated: new Signal(null),\n// }\n",
-        "import { Widget } from '@lumino/widgets';\nimport { ICommandPalette, IFrame } from '@jupyterlab/apputils';\nimport { JupyterFrontEnd } from '@jupyterlab/application';\nimport { ILauncher } from '@jupyterlab/launcher';\nimport { LabIcon } from '@jupyterlab/ui-components';\n\nimport { findFirefly } from './FireflyCommonUtils.js';\nimport fireflyIconStr from '../style/fftools-logo.svg';\n\n\nlet widgetId;\nlet widgetCnt= 1;\nlet openWidgets= {};\n\n\n/**\n * Extension can be started in two ways.\n * 1. as a jupyter command\n * 2. firefly_client sending a 'StartLabWindow' action\n * @param {JupyterFrontEnd} app\n * @param {ICommandPalette} palette\n * @param {ILauncher | null} launcher\n */\nexport function activateSlateCommandExt(app, palette, launcher) {\n    findFirefly().then( (ffConfig) => {\n        const {firefly}= ffConfig;\n        firefly.util.addActionListener(['StartLabWindow'], (action,state) => {\n            openSlateMulti(app, action.payload.renderTreeId, false);\n        });\n        firefly.util.addActionListener(['StartBrowserTab'], (action,state) => {\n            firefly.setViewerConfig(firefly.ViewerType.Grid);\n            firefly.getViewer(action.payload.channel).openViewer();\n        });\n\n    });\n\n    // for starting extension as a jupyter command -----------\n    const command = 'firefly:open-slate';\n    const category = 'Firefly';\n    const icon = new LabIcon({\n        name: 'jupyter_firefly_extensions:firefly-icon',\n        svgstr: fireflyIconStr\n      }); \n\n    app.commands.addCommand(command, {\n        label: 'Open Firefly',\n        caption: 'Open Firefly',\n        icon: icon,\n        isEnabled: () => true,\n        execute: () => {\n            const id= 'slate-'+ widgetCnt;\n            widgetCnt++;\n            openSlateMulti(app, id, true);\n        }\n    });\n\n    palette.addItem({ command, category });\n    if (launcher) launcher.add({ command, category});\n}\n\nfunction openSlateMulti(app, id, activate) {\n    activate= window.document.getElementById(id) || activate;\n    if (!openWidgets[id]) {\n        let widget = new SlateRootWidget(id);\n        if (app.shell.addToMainArea) app.shell.addToMainArea(widget); // --- pre version 1\n        else if (app.shell.add) app.shell.add(widget, 'main');  // version 1\n        else throw Error('Could not add firefly to tab');\n        findFirefly().then( (ffConfig) => {\n            const {action}= ffConfig.firefly;\n            action.dispatchChangeActivePlotView(undefined);\n        });\n        openWidgets[id]= widget;\n    }\n    if (activate) app.shell.activateById(id);\n\n}\n\n\n/**\n * Open only one slate tab.  Using this funtion keeps the slate tab as a singleton.\n *\n * Currently not used.\n * @param app\n */\nfunction openSlateSingleOnly(app) {\n    if (!widgetId) {\n        let widget = new SlateRootWidget('slate-1');\n        app.shell.addToMainArea(widget);\n        widgetId= widget.id;\n        findFirefly().then( (ffConfig) => {\n            const {action}= ffConfig.firefly;\n            action.dispatchChangeActivePlotView(undefined);\n        });\n    }\n    else {\n\n    }\n    app.shell.activateById(widgetId);\n}\n\n\n\nexport class SlateRootWidget extends Widget {\n    /**\n     * Construct a new output widget.\n     */\n    constructor(id) {\n        super({node: createNode(id)});\n        this.id= id;\n        this.title.label= 'Firefly: '+ id;\n        this.title.closable= true;\n        findFirefly().then( (ffConfig) => {\n            this.startViewer(ffConfig.firefly, id, ffConfig.fireflyURL);\n        } );\n    }\n\n    startViewer(firefly, id, fireflyURL) {\n        const {util,action}= firefly;\n        const props=  {\n            div: id,\n            renderTreeId: id,\n            template: 'FireflySlate',\n            disableDefaultDropDown: true,\n        };\n        const fallbackMenu= [\n            {label:'Images', action:'ImageSelectDropDownSlateCmd'},\n            {label:'TAP Searches', action: 'TAPSearch'},\n            {label:'Catalogs', action:'IrsaCatalogDropDown'},\n            {label:'Charts', action:'ChartSelectDropDownCmd'},\n            {label:'Upload', action: 'FileUploadDropDownCmd'},\n        ];\n        if (!firefly.originalAppProps) {\n            props.menu= fallbackMenu;\n        }\n        if (fireflyURL.endsWith('irsaviewer')) {\n            // make icon file path absolute, otherwise it won't be found\n            const originalAppIconProp = firefly?.originalAppProps?.appIcon;\n            if (originalAppIconProp) props.appIcon = fireflyURL + '/' + originalAppIconProp;\n            // resize it to fit in its parent container\n            props.bannerLeftStyle = {display: 'flex', marginTop: 'unset'};\n        }\n        action.dispatchApiToolsView(true,false);\n        this.controlApp= util.startAsAppFromApi(id, props);\n    }\n\n    dispose() {\n        widgetId= undefined;\n    }\n    close() {\n        super.close();\n        widgetId= undefined;\n        delete openWidgets[this.id];\n        if (this.controlApp) this.controlApp.unrender();\n        this.controlApp= undefined;\n    }\n\n    activate() {\n        super.activate();\n        if (this.controlApp) {\n            this.controlApp.unrender();\n            this.controlApp.render();\n        }\n        findFirefly().then( (ffConfig) => {\n            const {action}= ffConfig.firefly;\n            action.dispatchChangeActivePlotView(undefined);\n        });\n    }\n}\n\n\nfunction createNode(filename) {\n    const node = document.createElement('div');\n    node.id= filename;\n    const tmpElement=  document.createElement('div');\n    tmpElement.innerHTML= '<div>Firefly Loading...</div>';\n    node.appendChild(tmpElement);\n    return node;\n}\n",
+        "import { Widget } from '@lumino/widgets';\nimport { ICommandPalette } from '@jupyterlab/apputils';\nimport { JupyterFrontEnd } from '@jupyterlab/application';\nimport { ILauncher } from '@jupyterlab/launcher';\nimport { LabIcon } from '@jupyterlab/ui-components';\n\nimport { findFirefly } from './FireflyCommonUtils.js';\nimport fireflyIconStr from '../style/fftools-logo.svg';\n\n\nlet widgetId;\n\n/**\n * Extension can be started in two ways.\n * 1. as a jupyter command\n * 2. firefly_client sending a 'StartLabWindow' action\n * @param {JupyterFrontEnd} app\n * @param {ICommandPalette} palette\n * @param {ILauncher | null} launcher\n */\nexport function activateSlateCommandExt(app, palette, launcher) {\n    findFirefly().then( (ffConfig) => {\n        const {firefly}= ffConfig;\n        firefly.util.addActionListener(['StartLabWindow'], (action) => {\n            openSlateSingleOnly(app, undefined, action.payload?.fireflyHtmlFile);\n        });\n        firefly.util.addActionListener(['StartBrowserTab'], (action) => {\n            firefly.setViewerConfig(firefly.ViewerType.Grid);\n            firefly.getViewer(action.payload.channel).openViewer();\n        });\n\n    });\n\n    // for starting extension as a jupyter command -----------\n    const command = 'firefly:open-slate';\n    const category = 'Firefly';\n    const icon = new LabIcon({\n        name: 'jupyter_firefly_extensions:firefly-icon',\n        svgstr: fireflyIconStr\n      }); \n\n    app.commands.addCommand(command, {\n        label: 'Open Firefly',\n        caption: 'Open Firefly',\n        icon,\n        isEnabled: () => true,\n        execute: () => {\n            openSlateSingleOnly(app);\n        }\n    });\n\n    palette.addItem({ command, category });\n    if (launcher) launcher.add({ command, category});\n}\n\n\n/**\n * Open only one slate tab.  Using this keeps the tab as a singleton.\n * @param app\n * @param id\n * @param firelfyHtmlFile\n */\nfunction openSlateSingleOnly(app, id, firelfyHtmlFile) {\n    if (!widgetId) {\n        const widget = new SlateRootWidget('slate-1', firelfyHtmlFile);\n        widgetId= widget.id;\n        if (app.shell.addToMainArea) app.shell.addToMainArea(widget); // --- pre version 1\n        else if (app.shell.add) app.shell.add(widget, 'main');  // version 1\n        else throw Error('Could not add firefly to tab');\n\n        findFirefly().then( (ffConfig) => {\n            const {action}= ffConfig.firefly;\n            action.dispatchChangeActivePlotView(undefined);\n        });\n    }\n    app.shell.activateById(widgetId);\n}\n\nexport class SlateRootWidget extends Widget {\n    /**\n     * Construct a new output widget.\n     */\n    constructor(id,fireflyHtmlFile) {\n        super({node: createNode(id)});\n        this.id= id;\n        this.title.label= 'Firefly Viewer';\n        this.title.closable= true;\n        findFirefly().then( (ffConfig) => {\n            this.startViewer(ffConfig.firefly, id, ffConfig.fireflyURL, fireflyHtmlFile ?? ffConfig.fireflyHtmlFile);\n        } );\n    }\n\n    startViewer(firefly, id, fireflyURL, fireflyHtmlFile) {\n        const {util,action}= firefly;\n        const props=  {\n            div: id,\n            renderTreeId: id,\n            template: fireflyHtmlFile==='slate.html' ? 'FireflySlate' : 'FireflyViewer',\n            disableDefaultDropDown: true,\n        };\n        const fallbackMenu= [\n            {label:'Images', action:'ImageSelectDropDownSlateCmd'},\n            {label:'TAP Searches', action: 'TAPSearch'},\n            {label:'Catalogs', action:'IrsaCatalogDropDown'},\n            {label:'Charts', action:'ChartSelectDropDownCmd'},\n            {label:'Upload', action: 'FileUploadDropDownCmd'},\n        ];\n        if (!firefly.originalAppProps) {\n            props.menu= fallbackMenu;\n        }\n        if (fireflyURL.endsWith('irsaviewer')) {\n            // make icon file path absolute, otherwise it won't be found\n            const originalAppIconProp = firefly?.originalAppProps?.appIcon;\n            if (originalAppIconProp) props.appIcon = fireflyURL + '/' + originalAppIconProp;\n            // resize it to fit in its parent container\n            props.bannerLeftStyle = {display: 'flex', marginTop: 'unset'};\n        }\n        action.dispatchApiToolsView(true,false);\n        this.controlApp= util.startAsAppFromApi(id, props);\n    }\n\n    dispose() {\n        widgetId= undefined;\n    }\n    close() {\n        super.close();\n        widgetId= undefined;\n        if (this.controlApp) this.controlApp.unrender();\n        this.controlApp= undefined;\n    }\n\n    activate() {\n        super.activate();\n        if (this.controlApp) {\n            this.controlApp.unrender();\n            this.controlApp.render();\n        }\n        findFirefly().then( (ffConfig) => {\n            const {action}= ffConfig.firefly;\n            action.dispatchChangeActivePlotView(undefined);\n        });\n    }\n}\n\n\nfunction createNode(filename) {\n    const node = document.createElement('div');\n    node.id= filename;\n    const tmpElement=  document.createElement('div');\n    tmpElement.innerHTML= '<div>Firefly Loading...</div>';\n    node.appendChild(tmpElement);\n    return node;\n}\n",
         "import { JupyterFrontEndPlugin, ILayoutRestorer } from '@jupyterlab/application';\nimport { ICommandPalette } from '@jupyterlab/apputils';\nimport { ILauncher } from '@jupyterlab/launcher';\n\n\nimport { activateSlateCommandExt } from './SlateCommandExt.js';\nimport { activateFitsViewerExt } from './FitsViewerExt.js';\n\n/**\n * Initialization data for each extension.\n */\nconst showSlateExt: JupyterFrontEndPlugin<void> = {\n  id: 'jupyter_firefly_extensions:showSlate',\n  description: 'Show firefly slate',\n  autoStart: true,\n  requires: [ICommandPalette],\n  optional: [ILauncher],\n  activate: activateSlateCommandExt\n};\n\nconst fitsViewerExt: JupyterFrontEndPlugin<void> = {\n  id: 'jupyter_firefly_extensions:fitsviewer',\n  description: 'View a FITS file',\n  autoStart: true,\n  requires: [ILayoutRestorer],\n  activate: activateFitsViewerExt\n};\n\n// More than one extension/plugin can be exported as a list\nexport default [showSlateExt, fitsViewerExt];\n"
     ],
     "version": 3
 }
```

### Comparing `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/node_modules_b64-to-blob_b64toBlob_js.c490fc7119beea72c47e.js` & `jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/node_modules_b64-to-blob_b64toBlob_js.c490fc7119beea72c47e.js`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/node_modules_b64-to-blob_b64toBlob_js.c490fc7119beea72c47e.js.map` & `jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/node_modules_b64-to-blob_b64toBlob_js.c490fc7119beea72c47e.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.284b55f4388674029ec0.js.map` & `jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/remoteEntry.309ab0e4582c045c93a0.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9081632653061226%*

 * *Differences: {"'file'": "'remoteEntry.309ab0e4582c045c93a0.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"lib_index_js":"e8692010c055affebbc6","style_index_js":"1e1ab72bb82b2e804877","node_modules_b64-to-blob_b64toBlob_js":"c490fc7119beea72c47e","vendors-node_modules_firefly-api-a […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.284b55f4388674029ec0.js",
+    "file": "remoteEntry.309ab0e4582c045c93a0.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,qPAAqP;WACnR;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC/CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC5LA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter_firefly_extensions/webpack/container-entry",
         "webpack://jupyter_firefly_extensions/webpack/bootstrap",
         "webpack://jupyter_firefly_extensions/webpack/runtime/compat get default export",
@@ -25,22 +25,22 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn __webpack_require__.e(\"style_index_js\").then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"500e363702a4f528a942\",\"style_index_js\":\"1e1ab72bb82b2e804877\",\"node_modules_b64-to-blob_b64toBlob_js\":\"c490fc7119beea72c47e\",\"vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js\":\"11d96cd25e15e62dfcc9\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"e8692010c055affebbc6\",\"style_index_js\":\"1e1ab72bb82b2e804877\",\"node_modules_b64-to-blob_b64toBlob_js\":\"c490fc7119beea72c47e\",\"vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js\":\"11d96cd25e15e62dfcc9\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyter_firefly_extensions:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyter_firefly_extensions\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"b64-to-blob\", \"1.2.19\", () => (__webpack_require__.e(\"node_modules_b64-to-blob_b64toBlob_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/b64-to-blob/b64toBlob.js */ \"./node_modules/b64-to-blob/b64toBlob.js\"))))));\n\t\t\tregister(\"firefly-api-access\", \"0.0.4\", () => (__webpack_require__.e(\"vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/firefly-api-access/distribution/firefly-api-access.min.js */ \"./node_modules/firefly-api-access/distribution/firefly-api-access.min.js\"))))));\n\t\t\tregister(\"jupyter_firefly_extensions\", \"4.1.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyter_firefly_extensions\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"b64-to-blob\", \"1.2.19\", () => (__webpack_require__.e(\"node_modules_b64-to-blob_b64toBlob_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/b64-to-blob/b64toBlob.js */ \"./node_modules/b64-to-blob/b64toBlob.js\"))))));\n\t\t\tregister(\"firefly-api-access\", \"0.0.4\", () => (__webpack_require__.e(\"vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/firefly-api-access/distribution/firefly-api-access.min.js */ \"./node_modules/firefly-api-access/distribution/firefly-api-access.min.js\"))))));\n\t\t\tregister(\"jupyter_firefly_extensions\", \"5.0.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,4,1,6])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,2,6])),\n\t\"webpack/sharing/consume/default/@jupyterlab/launcher\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/launcher\", [1,4,1,6])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,2,3,1,,\"alpha\",0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,4,1,6])),\n\t\"webpack/sharing/consume/default/firefly-api-access/firefly-api-access\": () => (loadStrictVersionCheckFallback(\"default\", \"firefly-api-access\", [4,0,0,4], () => (__webpack_require__.e(\"vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js\").then(() => (() => (__webpack_require__(/*! firefly-api-access */ \"./node_modules/firefly-api-access/distribution/firefly-api-access.min.js\"))))))),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,7,1,6])),\n\t\"webpack/sharing/consume/default/b64-to-blob/b64-to-blob\": () => (loadStrictVersionCheckFallback(\"default\", \"b64-to-blob\", [1,1,2,19], () => (__webpack_require__.e(\"node_modules_b64-to-blob_b64toBlob_js\").then(() => (() => (__webpack_require__(/*! b64-to-blob */ \"./node_modules/b64-to-blob/b64toBlob.js\"))))))),\n\t\"webpack/sharing/consume/default/@jupyterlab/docregistry\": () => (loadVersionCheck(\"default\", \"@jupyterlab/docregistry\", [1,4,1,6])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,6,1,6]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/launcher\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/firefly-api-access/firefly-api-access\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/b64-to-blob/b64-to-blob\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/docregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,4,0,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,1,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/launcher\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/launcher\", [1,4,0,5])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,2,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,4,0,5])),\n\t\"webpack/sharing/consume/default/firefly-api-access/firefly-api-access\": () => (loadStrictVersionCheckFallback(\"default\", \"firefly-api-access\", [4,0,0,4], () => (__webpack_require__.e(\"vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js\").then(() => (() => (__webpack_require__(/*! firefly-api-access */ \"./node_modules/firefly-api-access/distribution/firefly-api-access.min.js\"))))))),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,7,0,5])),\n\t\"webpack/sharing/consume/default/b64-to-blob/b64-to-blob\": () => (loadStrictVersionCheckFallback(\"default\", \"b64-to-blob\", [1,1,2,19], () => (__webpack_require__.e(\"node_modules_b64-to-blob_b64toBlob_js\").then(() => (() => (__webpack_require__(/*! b64-to-blob */ \"./node_modules/b64-to-blob/b64toBlob.js\"))))))),\n\t\"webpack/sharing/consume/default/@jupyterlab/docregistry\": () => (loadVersionCheck(\"default\", \"@jupyterlab/docregistry\", [1,4,0,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,6,0,5]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/launcher\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/firefly-api-access/firefly-api-access\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/b64-to-blob/b64-to-blob\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/docregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyter_firefly_extensions\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyter_firefly_extensions\"] = self[\"webpackChunkjupyter_firefly_extensions\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyter_firefly_extensions\");\n",
         ""
     ],
     "version": 3
```

### Comparing `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.d65ffc2462e0ee205d4e.js` & `jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/remoteEntry.309ab0e4582c045c93a0.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -182,15 +182,15 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_index_js": "d1c31609190d65e955f6",
+                "lib_index_js": "e8692010c055affebbc6",
                 "style_index_js": "1e1ab72bb82b2e804877",
                 "node_modules_b64-to-blob_b64toBlob_js": "c490fc7119beea72c47e",
                 "vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js": "11d96cd25e15e62dfcc9"
             } [chunkId] + ".js";
             /******/
         };
         /******/
@@ -433,15 +433,15 @@
                 /******/
                 case "default": {
                     /******/
                     register("b64-to-blob", "1.2.19", () => (__webpack_require__.e("node_modules_b64-to-blob_b64toBlob_js").then(() => (() => (__webpack_require__( /*! ./node_modules/b64-to-blob/b64toBlob.js */ "./node_modules/b64-to-blob/b64toBlob.js"))))));
                     /******/
                     register("firefly-api-access", "0.0.4", () => (__webpack_require__.e("vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js").then(() => (() => (__webpack_require__( /*! ./node_modules/firefly-api-access/distribution/firefly-api-access.min.js */ "./node_modules/firefly-api-access/distribution/firefly-api-access.min.js"))))));
                     /******/
-                    register("jupyter_firefly_extensions", "4.1.0", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyter_firefly_extensions", "5.0.0", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -834,33 +834,33 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/application": () => (loadSingletonVersionCheck("default", "@jupyterlab/application", [1, 4, 1, 6])),
+            "webpack/sharing/consume/default/@jupyterlab/application": () => (loadSingletonVersionCheck("default", "@jupyterlab/application", [1, 4, 0, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 4, 2, 6])),
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 4, 1, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/launcher": () => (loadSingletonVersionCheck("default", "@jupyterlab/launcher", [1, 4, 1, 6])),
+            "webpack/sharing/consume/default/@jupyterlab/launcher": () => (loadSingletonVersionCheck("default", "@jupyterlab/launcher", [1, 4, 0, 5])),
             /******/
-            "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0])),
+            "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 2, 0, 1])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 4, 1, 6])),
+            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 4, 0, 5])),
             /******/
             "webpack/sharing/consume/default/firefly-api-access/firefly-api-access": () => (loadStrictVersionCheckFallback("default", "firefly-api-access", [4, 0, 0, 4], () => (__webpack_require__.e("vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js").then(() => (() => (__webpack_require__( /*! firefly-api-access */ "./node_modules/firefly-api-access/distribution/firefly-api-access.min.js"))))))),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/services": () => (loadSingletonVersionCheck("default", "@jupyterlab/services", [1, 7, 1, 6])),
+            "webpack/sharing/consume/default/@jupyterlab/services": () => (loadSingletonVersionCheck("default", "@jupyterlab/services", [1, 7, 0, 5])),
             /******/
             "webpack/sharing/consume/default/b64-to-blob/b64-to-blob": () => (loadStrictVersionCheckFallback("default", "b64-to-blob", [1, 1, 2, 19], () => (__webpack_require__.e("node_modules_b64-to-blob_b64toBlob_js").then(() => (() => (__webpack_require__( /*! b64-to-blob */ "./node_modules/b64-to-blob/b64toBlob.js"))))))),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/docregistry": () => (loadVersionCheck("default", "@jupyterlab/docregistry", [1, 4, 1, 6])),
+            "webpack/sharing/consume/default/@jupyterlab/docregistry": () => (loadVersionCheck("default", "@jupyterlab/docregistry", [1, 4, 0, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 6, 1, 6]))
+            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 6, 0, 5]))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "lib_index_js": [
@@ -1114,8 +1114,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyter_firefly_extensions");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB).jupyter_firefly_extensions = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.d65ffc2462e0ee205d4e.js.map
+//# sourceMappingURL=remoteEntry.309ab0e4582c045c93a0.js.map
```

### Comparing `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/style_index_js.1e1ab72bb82b2e804877.js` & `jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/style_index_js.1e1ab72bb82b2e804877.js`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/style_index_js.1e1ab72bb82b2e804877.js.map` & `jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/style_index_js.1e1ab72bb82b2e804877.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js.11d96cd25e15e62dfcc9.js` & `jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js.11d96cd25e15e62dfcc9.js`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js.11d96cd25e15e62dfcc9.js.map` & `jupyter_firefly_extensions-4.2.0/jupyter_firefly_extensions/labextension/static/vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js.11d96cd25e15e62dfcc9.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/src/FireflyCommonUtils.js` & `jupyter_firefly_extensions-4.2.0/src/FireflyCommonUtils.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -28,18 +28,19 @@
     if (cachedFindFireflyResult) return cachedFindFireflyResult;
 
     try {
         // request the config from server at /lab/fireflyLocation (see handlers.py)
         const settings = ServerConnection.makeSettings();
         if (!cachedLoc) cachedLoc = await (await ServerConnection.makeRequest(ffLocURL, fetchOptions, settings)).json();
 
-        // make sure that response of above request contains non-empty fireflyURL
+        // make sure that response of the above request contains non-empty fireflyURL
         const {
             fireflyURL,
-            fireflyChannel: channel
+            fireflyChannel: channel,
+            fireflyHtmlFile
         } = cachedLoc;
         if (!fireflyURL) throw new Error(`fireflyURL couldn't be retrieved from ${ffLocURL}`);
 
         // load firefly API from fireflyURL at /lab (window)
         // (CORS errors might happen here if headers aren't set up correctly, maybe due to caching)
         if (!window.firefly?.initialized) window.firefly = {
             ...window.firefly,
@@ -48,15 +49,16 @@
         if (!window.getFireflyAPI) window.getFireflyAPI = initFirefly(fireflyURL);
         const firefly = await window.getFireflyAPI();
 
         // resolve Promise
         cachedFindFireflyResult = {
             fireflyURL,
             channel,
-            firefly
+            firefly,
+            fireflyHtmlFile
         };
         console.log('Firefly loaded successfully\n', cachedFindFireflyResult);
         return cachedFindFireflyResult;
     } catch (e) {
         // log information about error(s) before rejecting Promise
         console.group('Firefly Load Failed');
         console.log('findFirefly: Could not determine firefly location or load firefly, call failed');
@@ -80,11 +82,11 @@
 
 export function makeLabEndpoint(endPoint, searchParams) {
     const {
         origin,
         pathname
     } = new URL(window.document.location.href);
     const originURL = origin + pathname;
-    const start = originURL.substring(0, originURL.lastIndexOf('lab'))
+    const start = originURL.substring(0, originURL.lastIndexOf('lab'));
     const slashMaybe = start.endsWith('/') ? '' : '/';
-    return `${start}${slashMaybe}${endPoint}${searchParams?'?'+searchParams.toString():''}`
+    return `${start}${slashMaybe}${endPoint}${searchParams?'?'+searchParams.toString():''}`;
 }
```

### Comparing `jupyter_firefly_extensions-4.1.1/src/FitsViewerExt.js` & `jupyter_firefly_extensions-4.2.0/src/FitsViewerExt.js`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/src/SlateCommandExt.js` & `jupyter_firefly_extensions-4.2.0/src/SlateCommandExt.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,12 @@
 import {
     Widget
 } from '@lumino/widgets';
 import {
-    ICommandPalette,
-    IFrame
+    ICommandPalette
 } from '@jupyterlab/apputils';
 import {
     JupyterFrontEnd
 } from '@jupyterlab/application';
 import {
     ILauncher
 } from '@jupyterlab/launcher';
@@ -18,35 +17,33 @@
 import {
     findFirefly
 } from './FireflyCommonUtils.js';
 import fireflyIconStr from '../style/fftools-logo.svg';
 
 
 let widgetId;
-let widgetCnt = 1;
-let openWidgets = {};
-
+const TAB_ID = 'firefly-viewer-tab-id';
 
 /**
  * Extension can be started in two ways.
  * 1. as a jupyter command
  * 2. firefly_client sending a 'StartLabWindow' action
  * @param {JupyterFrontEnd} app
  * @param {ICommandPalette} palette
  * @param {ILauncher | null} launcher
  */
 export function activateSlateCommandExt(app, palette, launcher) {
     findFirefly().then((ffConfig) => {
         const {
             firefly
         } = ffConfig;
-        firefly.util.addActionListener(['StartLabWindow'], (action, state) => {
-            openSlateMulti(app, action.payload.renderTreeId, false);
+        firefly.util.addActionListener(['StartLabWindow'], (action) => {
+            openSlateSingleOnly(app, TAB_ID, action.payload?.fireflyHtmlFile);
         });
-        firefly.util.addActionListener(['StartBrowserTab'], (action, state) => {
+        firefly.util.addActionListener(['StartBrowserTab'], (action) => {
             firefly.setViewerConfig(firefly.ViewerType.Grid);
             firefly.getViewer(action.payload.channel).openViewer();
         });
 
     });
 
     // for starting extension as a jupyter command -----------
@@ -56,103 +53,81 @@
         name: 'jupyter_firefly_extensions:firefly-icon',
         svgstr: fireflyIconStr
     });
 
     app.commands.addCommand(command, {
         label: 'Open Firefly',
         caption: 'Open Firefly',
-        icon: icon,
+        icon,
         isEnabled: () => true,
         execute: () => {
-            const id = 'slate-' + widgetCnt;
-            widgetCnt++;
-            openSlateMulti(app, id, true);
+            openSlateSingleOnly(app, TAB_ID);
         }
     });
 
     palette.addItem({
         command,
         category
     });
     if (launcher) launcher.add({
         command,
         category
     });
 }
 
-function openSlateMulti(app, id, activate) {
-    activate = window.document.getElementById(id) || activate;
-    if (!openWidgets[id]) {
-        let widget = new SlateRootWidget(id);
-        if (app.shell.addToMainArea) app.shell.addToMainArea(widget); // --- pre version 1
-        else if (app.shell.add) app.shell.add(widget, 'main'); // version 1
-        else throw Error('Could not add firefly to tab');
-        findFirefly().then((ffConfig) => {
-            const {
-                action
-            } = ffConfig.firefly;
-            action.dispatchChangeActivePlotView(undefined);
-        });
-        openWidgets[id] = widget;
-    }
-    if (activate) app.shell.activateById(id);
-
-}
-
 
 /**
- * Open only one slate tab.  Using this funtion keeps the slate tab as a singleton.
- *
- * Currently not used.
+ * Open only one slate tab.  Using this keeps the tab as a singleton.
  * @param app
+ * @param id
+ * @param firelfyHtmlFile
  */
-function openSlateSingleOnly(app) {
+function openSlateSingleOnly(app, id, firelfyHtmlFile) {
     if (!widgetId) {
-        let widget = new SlateRootWidget('slate-1');
-        app.shell.addToMainArea(widget);
+        const widget = new SlateRootWidget(id, firelfyHtmlFile);
         widgetId = widget.id;
+        if (app.shell.addToMainArea) app.shell.addToMainArea(widget); // --- pre version 1
+        else if (app.shell.add) app.shell.add(widget, 'main'); // version 1
+        else throw Error('Could not add firefly to tab');
+
         findFirefly().then((ffConfig) => {
             const {
                 action
             } = ffConfig.firefly;
             action.dispatchChangeActivePlotView(undefined);
         });
-    } else {
-
     }
     app.shell.activateById(widgetId);
 }
 
-
-
 export class SlateRootWidget extends Widget {
     /**
      * Construct a new output widget.
      */
-    constructor(id) {
+    constructor(id, fireflyHtmlFile) {
         super({
             node: createNode(id)
         });
         this.id = id;
-        this.title.label = 'Firefly: ' + id;
+        this.title.label = 'Firefly Viewer';
         this.title.closable = true;
         findFirefly().then((ffConfig) => {
-            this.startViewer(ffConfig.firefly, id, ffConfig.fireflyURL);
+            this.startViewer(ffConfig.firefly, id, ffConfig.fireflyURL, fireflyHtmlFile ?? ffConfig.fireflyHtmlFile);
         });
     }
 
-    startViewer(firefly, id, fireflyURL) {
+    startViewer(firefly, id, fireflyURL, fireflyHtmlFile) {
         const {
             util,
             action
         } = firefly;
         const props = {
             div: id,
             renderTreeId: id,
-            template: 'FireflySlate',
+            template: fireflyHtmlFile === 'slate.html' ? 'FireflySlate' : 'FireflyViewer',
             disableDefaultDropDown: true,
         };
         const fallbackMenu = [{
             label: 'Images',
             action: 'ImageSelectDropDownSlateCmd'
         }, {
             label: 'TAP Searches',
@@ -186,15 +161,14 @@
 
     dispose() {
         widgetId = undefined;
     }
     close() {
         super.close();
         widgetId = undefined;
-        delete openWidgets[this.id];
         if (this.controlApp) this.controlApp.unrender();
         this.controlApp = undefined;
     }
 
     activate() {
         super.activate();
         if (this.controlApp) {
```

### Comparing `jupyter_firefly_extensions-4.1.1/src/handler.ts` & `jupyter_firefly_extensions-4.2.0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/src/index.ts` & `jupyter_firefly_extensions-4.2.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/style/fftools-logo.svg` & `jupyter_firefly_extensions-4.2.0/style/fftools-logo.svg`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/.gitignore` & `jupyter_firefly_extensions-4.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/README.md` & `jupyter_firefly_extensions-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/pyproject.toml` & `jupyter_firefly_extensions-4.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.1/PKG-INFO` & `jupyter_firefly_extensions-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyter_firefly_extensions
-Version: 4.1.1
+Version: 4.2.0
 Dynamic: Keywords
 Summary: Jupyterlab extensions for rendering FITS and displaying tables, images, & charts with Firefly
 Project-URL: Homepage, https://github.com/Caltech-IPAC/jupyter_firefly_extensions
 Project-URL: Bug Tracker, https://github.com/Caltech-IPAC/jupyter_firefly_extensions/issues
 Project-URL: Repository, https://github.com/Caltech-IPAC/jupyter_firefly_extensions.git
 Author-email: Trey Roby <roby@ipac.caltech.edu>
 License: BSD-3-Clause License
```

