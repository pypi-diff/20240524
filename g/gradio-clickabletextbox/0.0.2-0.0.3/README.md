# Comparing `tmp/gradio_clickabletextbox-0.0.2.tar.gz` & `tmp/gradio_clickabletextbox-0.0.3.tar.gz`

## Comparing `gradio_clickabletextbox-0.0.2.tar` & `gradio_clickabletextbox-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/__init__.py
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/clickabletextbox.py
--rw-r--r--   0        0        0    37561 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/clickabletextbox.pyi
--rw-r--r--   0        0        0    97610 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/templates/component/index.js
--rw-r--r--   0        0        0    16404 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/templates/component/style.css
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/templates/example/index.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/demo/__init__.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/demo/app.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/demo/css.css
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/demo/requirements.txt
--rw-r--r--   0        0        0    10461 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/demo/space.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/frontend/Example.svelte
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/frontend/Index.svelte
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/frontend/gradio.config.js
--rw-r--r--   0        0        0   150164 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/frontend/package-lock.json
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/frontend/package.json
--rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/frontend/shared/Textbox.svelte
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/frontend/shared/transitions.js
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/.gitignore
--rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/README.md
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/__init__.py
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/clickabletextbox.py
+-rw-r--r--   0        0        0    37561 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/clickabletextbox.pyi
+-rw-r--r--   0        0        0    97610 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/templates/component/index.js
+-rw-r--r--   0        0        0    16404 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/templates/component/style.css
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/templates/example/index.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/demo/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/demo/app.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/demo/css.css
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/demo/requirements.txt
+-rw-r--r--   0        0        0    10461 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/demo/space.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/frontend/Example.svelte
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/frontend/Index.svelte
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/frontend/gradio.config.js
+-rw-r--r--   0        0        0   150164 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/frontend/package-lock.json
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/frontend/package.json
+-rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/frontend/shared/Textbox.svelte
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/frontend/shared/transitions.js
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/.gitignore
+-rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/README.md
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.3/PKG-INFO
```

### Comparing `gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/clickabletextbox.py` & `gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/clickabletextbox.py`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/clickabletextbox.pyi` & `gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/clickabletextbox.pyi`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/templates/component/index.js` & `gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/templates/component/index.js`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/templates/component/style.css` & `gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/templates/example/index.js` & `gradio_clickabletextbox-0.0.3/backend/gradio_clickabletextbox/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.2/demo/app.py` & `gradio_clickabletextbox-0.0.3/demo/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     lambda x: x,
     # interactive version of your component
     ClickableTextbox(suffixes=suffixes, prompts=prompts),
     ClickableTextbox(suffixes=suffixes, prompts=prompts,),
 )
 
 if __name__ == "__main__":
-    demo.launch(server_port=1235)
+    demo.launch(server_port=1236)
```

### Comparing `gradio_clickabletextbox-0.0.2/demo/css.css` & `gradio_clickabletextbox-0.0.3/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.2/demo/space.py` & `gradio_clickabletextbox-0.0.3/demo/space.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     lambda x: x,
     # interactive version of your component
     ClickableTextbox(suffixes=suffixes, prompts=prompts),
     ClickableTextbox(suffixes=suffixes, prompts=prompts,),
 )
 
 if __name__ == "__main__":
-    demo.launch(server_port=1235)
+    demo.launch(server_port=1236)
 
 ```
 """, elem_classes=["md-custom"], header_links=True)
 
 
     gr.Markdown("""
 ## `ClickableTextbox`
```

### Comparing `gradio_clickabletextbox-0.0.2/frontend/Example.svelte` & `gradio_clickabletextbox-0.0.3/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.2/frontend/Index.svelte` & `gradio_clickabletextbox-0.0.3/frontend/Index.svelte`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.2/frontend/package-lock.json` & `gradio_clickabletextbox-0.0.3/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.2/frontend/package.json` & `gradio_clickabletextbox-0.0.3/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.2/frontend/shared/Textbox.svelte` & `gradio_clickabletextbox-0.0.3/frontend/shared/Textbox.svelte`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.2/frontend/shared/transitions.js` & `gradio_clickabletextbox-0.0.3/frontend/shared/transitions.js`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.2/README.md` & `gradio_clickabletextbox-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     lambda x: x,
     # interactive version of your component
     ClickableTextbox(suffixes=suffixes, prompts=prompts),
     ClickableTextbox(suffixes=suffixes, prompts=prompts,),
 )
 
 if __name__ == "__main__":
-    demo.launch(server_port=1235)
+    demo.launch(server_port=1236)
 
 ```
 
 ## `ClickableTextbox`
 
 ### Initialization
```

### Comparing `gradio_clickabletextbox-0.0.2/pyproject.toml` & `gradio_clickabletextbox-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_clickabletextbox"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python library for easily interacting with trained machine learning models"
 readme = "README.md"
 license = "apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "YOUR NAME", email = "YOUREMAIL@domain.com" }]
 keywords = ["gradio-custom-component", "gradio-template-Textbox"]
 # Add dependencies here
```

### Comparing `gradio_clickabletextbox-0.0.2/PKG-INFO` & `gradio_clickabletextbox-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_clickabletextbox
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library for easily interacting with trained machine learning models
 Author-email: YOUR NAME <YOUREMAIL@domain.com>
 License-Expression: Apache-2.0
 Keywords: gradio-custom-component,gradio-template-Textbox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -50,15 +50,15 @@
     lambda x: x,
     # interactive version of your component
     ClickableTextbox(suffixes=suffixes, prompts=prompts),
     ClickableTextbox(suffixes=suffixes, prompts=prompts,),
 )
 
 if __name__ == "__main__":
-    demo.launch(server_port=1235)
+    demo.launch(server_port=1236)
 
 ```
 
 ## `ClickableTextbox`
 
 ### Initialization
```

