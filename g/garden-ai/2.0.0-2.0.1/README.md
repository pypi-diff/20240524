# Comparing `tmp/garden_ai-2.0.0.tar.gz` & `tmp/garden_ai-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garden_ai-2.0.0.tar", max compression
+gzip compressed data, was "garden_ai-2.0.1.tar", max compression
```

## Comparing `garden_ai-2.0.0.tar` & `garden_ai-2.0.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0     1078 2024-05-03 16:58:19.319971 garden_ai-2.0.0/LICENSE
--rw-r--r--   0        0        0      797 2024-05-03 16:58:19.319971 garden_ai-2.0.0/README.md
--rw-r--r--   0        0        0      537 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/__init__.py
--rw-r--r--   0        0        0       54 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/__main__.py
--rw-r--r--   0        0        0      180 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/_version.py
--rw-r--r--   0        0        0        0 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/app/__init__.py
--rw-r--r--   0        0        0      905 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/app/completion.py
--rw-r--r--   0        0        0     2501 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/app/console.py
--rw-r--r--   0        0        0     2840 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/app/docker.py
--rw-r--r--   0        0        0     7963 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/app/entrypoint.py
--rw-r--r--   0        0        0    16504 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/app/garden.py
--rw-r--r--   0        0        0     1936 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/app/main.py
--rw-r--r--   0        0        0    22960 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/app/notebook.py
--rw-r--r--   0        0        0     3280 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/backend_client.py
--rw-r--r--   0        0        0    24960 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/client.py
--rw-r--r--   0        0        0     3970 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/constants.py
--rw-r--r--   0        0        0    18666 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/containers.py
--rw-r--r--   0        0        0     9394 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/datacite.py
--rw-r--r--   0        0        0    13997 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/entrypoints.py
--rw-r--r--   0        0        0     1068 2024-05-03 16:58:19.327971 garden_ai-2.0.0/garden_ai/garden_file_adapter.py
--rw-r--r--   0        0        0    18186 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/gardens.py
--rw-r--r--   0        0        0        0 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/globus_search/__init__.py
--rw-r--r--   0        0        0     1409 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/globus_search/garden_search.py
--rw-r--r--   0        0        0     6461 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/local_data.py
--rw-r--r--   0        0        0     3270 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/mlmodel.py
--rw-r--r--   0        0        0      107 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/model_connectors/__init__.py
--rw-r--r--   0        0        0     2449 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/model_connectors/github_conn.py
--rw-r--r--   0        0        0     1712 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/model_connectors/hugging_face.py
--rw-r--r--   0        0        0     8060 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/notebook_metadata.py
--rw-r--r--   0        0        0     2423 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/notebook_templates/debug.ipynb
--rw-r--r--   0        0        0     1200 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/notebook_templates/empty.ipynb
--rw-r--r--   0        0        0     7490 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/notebook_templates/sklearn.ipynb
--rw-r--r--   0        0        0     7405 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/notebook_templates/tensorflow.ipynb
--rw-r--r--   0        0        0     7612 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/notebook_templates/torch.ipynb
--rw-r--r--   0        0        0    10250 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/notebook_templates/tutorial.ipynb
--rw-r--r--   0        0        0     3495 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/scripts/save_session_and_metadata.py
--rw-r--r--   0        0        0        0 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/utils/__init__.py
--rw-r--r--   0        0        0     3394 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/utils/_meta.py
--rw-r--r--   0        0        0      628 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/utils/dois.py
--rw-r--r--   0        0        0     1684 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/utils/interactive_cli.py
--rw-r--r--   0        0        0     2769 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/utils/misc.py
--rw-r--r--   0        0        0     1854 2024-05-03 16:58:19.331971 garden_ai-2.0.0/garden_ai/utils/notebooks.py
--rw-r--r--   0        0        0     2545 2024-05-03 16:58:30.431993 garden_ai-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2583 1970-01-01 00:00:00.000000 garden_ai-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-24 16:05:03.079223 garden_ai-2.0.1/LICENSE
+-rw-r--r--   0        0        0      797 2024-05-24 16:05:03.079223 garden_ai-2.0.1/README.md
+-rw-r--r--   0        0        0      537 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/__init__.py
+-rw-r--r--   0        0        0       54 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/__main__.py
+-rw-r--r--   0        0        0      180 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/_version.py
+-rw-r--r--   0        0        0        0 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/app/__init__.py
+-rw-r--r--   0        0        0      905 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/app/completion.py
+-rw-r--r--   0        0        0     2501 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/app/console.py
+-rw-r--r--   0        0        0     2840 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/app/docker.py
+-rw-r--r--   0        0        0     7963 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/app/entrypoint.py
+-rw-r--r--   0        0        0    16548 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/app/garden.py
+-rw-r--r--   0        0        0     1936 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/app/main.py
+-rw-r--r--   0        0        0    24601 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/app/notebook.py
+-rw-r--r--   0        0        0     3280 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/backend_client.py
+-rw-r--r--   0        0        0    24960 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/client.py
+-rw-r--r--   0        0        0     3970 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/constants.py
+-rw-r--r--   0        0        0    18666 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/containers.py
+-rw-r--r--   0        0        0     9394 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/datacite.py
+-rw-r--r--   0        0        0    16391 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/entrypoints.py
+-rw-r--r--   0        0        0     1068 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/garden_file_adapter.py
+-rw-r--r--   0        0        0    18186 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/gardens.py
+-rw-r--r--   0        0        0        0 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/globus_search/__init__.py
+-rw-r--r--   0        0        0     1409 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/globus_search/garden_search.py
+-rw-r--r--   0        0        0     6461 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/local_data.py
+-rw-r--r--   0        0        0     3270 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/mlmodel.py
+-rw-r--r--   0        0        0      107 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/model_connectors/__init__.py
+-rw-r--r--   0        0        0      967 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/model_connectors/exceptions.py
+-rw-r--r--   0        0        0     4998 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/model_connectors/github_conn.py
+-rw-r--r--   0        0        0     2463 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/model_connectors/hugging_face.py
+-rw-r--r--   0        0        0     8445 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/notebook_metadata.py
+-rw-r--r--   0        0        0     2465 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/notebook_templates/debug.ipynb
+-rw-r--r--   0        0        0     1242 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/notebook_templates/empty.ipynb
+-rw-r--r--   0        0        0     8271 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/notebook_templates/sklearn.ipynb
+-rw-r--r--   0        0        0     8012 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/notebook_templates/tensorflow.ipynb
+-rw-r--r--   0        0        0     8219 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/notebook_templates/torch.ipynb
+-rw-r--r--   0        0        0    10668 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/notebook_templates/tutorial.ipynb
+-rw-r--r--   0        0        0     4856 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/scripts/save_session_and_metadata.py
+-rw-r--r--   0        0        0        0 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/utils/__init__.py
+-rw-r--r--   0        0        0     3394 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/utils/_meta.py
+-rw-r--r--   0        0        0      628 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/utils/dois.py
+-rw-r--r--   0        0        0     1684 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/utils/interactive_cli.py
+-rw-r--r--   0        0        0     2769 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/utils/misc.py
+-rw-r--r--   0        0        0     1854 2024-05-24 16:05:03.087223 garden_ai-2.0.1/garden_ai/utils/notebooks.py
+-rw-r--r--   0        0        0     2741 2024-05-24 16:05:12.907315 garden_ai-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2704 1970-01-01 00:00:00.000000 garden_ai-2.0.1/PKG-INFO
```

### Comparing `garden_ai-2.0.0/LICENSE` & `garden_ai-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/README.md` & `garden_ai-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/__init__.py` & `garden_ai-2.0.1/garden_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/app/completion.py` & `garden_ai-2.0.1/garden_ai/app/completion.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/app/console.py` & `garden_ai-2.0.1/garden_ai/app/console.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/app/docker.py` & `garden_ai-2.0.1/garden_ai/app/docker.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/app/entrypoint.py` & `garden_ai-2.0.1/garden_ai/app/entrypoint.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/app/garden.py` & `garden_ai-2.0.1/garden_ai/app/garden.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,16 @@
                 name = validate_name(
                     Prompt.ask("Add another contributor? (leave blank to finish)")
                 )
                 if name:
                     authors += [name]
                 else:
                     break
+        else:
+            contributors = []
 
     if not description:
         description = Prompt.ask(
             "Provide a brief description of this Garden, to aid in discovery (leave blank to skip)"
         )
 
     client = GardenClient()
```

### Comparing `garden_ai-2.0.0/garden_ai/app/main.py` & `garden_ai-2.0.1/garden_ai/app/main.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/app/notebook.py` & `garden_ai-2.0.1/garden_ai/app/notebook.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 )
 
 from garden_ai.notebook_metadata import (
     add_notebook_metadata_cell,
     set_notebook_metadata,
     get_notebook_metadata,
     read_requirements_data,
+    NotebookMetadata,
 )
 
 from garden_ai.utils.notebooks import (
     clear_cells,
     is_over_size_limit,
     generate_botanical_filename,
 )
@@ -148,14 +149,23 @@
         None,
         "--requirements",
         help=(
             "Path to a requirements.txt containing "
             "additional dependencies to install in the base image."
         ),
     ),
+    global_notebook_doi: Optional[str] = typer.Option(
+        None,
+        "--doi",
+        help=(
+            "DOI of a Garden you want to add all entrypoints in this notebook too. "
+            "To override the global notebook DOI for a specific entrypoint, "
+            "provide the garden_entrypoint decorator with the optional garden_doi argument."
+        ),
+    ),
     custom_image_uri: Optional[str] = typer.Option(
         None,
         "--custom-image",
         help=(
             "Power users only! Provide a uri of a publicly available docker image to boot the notebook in."
         ),
         hidden=True,
@@ -192,42 +202,39 @@
             need_to_create_notebook = True
 
     # Adds notebook metadata if cell is missing
     if not need_to_create_notebook:
         add_notebook_metadata_cell(notebook_path)
 
     # Figure out what base image uri we should start the notebook in
-    # base_image_uri will always be set after this point
     base_image_uri = _get_base_image_uri(
         base_image_name,
         custom_image_uri,
         None if need_to_create_notebook else notebook_path,
     )
 
     # Now we have all we need to prompt the user to proceed
     if need_to_create_notebook:
         message = f"This will create a new notebook {notebook_path.name} and open it in Docker image {base_image_uri}.\n"
+        # For a new notebook, start with all notebook_metadata values as None.
+        # Updates it with any provided values later on before the notebook starts.
+        notebook_metadata = NotebookMetadata(None, None, None, None)
     else:
         message = f"This will open existing notebook {notebook_path.name} in Docker image {base_image_uri}.\n"
+        notebook_metadata = get_notebook_metadata(notebook_path)
 
     # Validate and read requirements file.
     if requirements_path:
         message += f"Additional dependencies specified in {requirements_path.name} will also be installed in {base_image_uri}.\n"
         message += "Any dependencies previously associated with this notebook will be overwritten by the new requirements.\n"
         _validate_requirements_path(requirements_path)
         requirements_data = read_requirements_data(requirements_path)
     else:
-        # If no requirements file given, look for requirements data in notebook
-        if notebook_path.is_file():
-            requirements_data = get_notebook_metadata(
-                notebook_path
-            ).notebook_requirements
-        else:
-            # Creating new notebook, no requirements data
-            requirements_data = None
+        # If no requirements file given, look for requirements data in notebook metadata
+        requirements_data = notebook_metadata.notebook_requirements
 
     typer.confirm(message + "Do you want to proceed?", abort=True)
 
     if need_to_create_notebook:
         if tutorial:
             template_file_name = "tutorial.ipynb"
         elif base_image_name:
@@ -237,23 +244,30 @@
         else:
             template_file_name = "empty.ipynb"
 
         top_level_dir = Path(__file__).parent.parent
         source_path = top_level_dir / "notebook_templates" / template_file_name
         shutil.copy(source_path, notebook_path)
 
-    # Get base image name from notebook if user did not provide
+    # Check for base image name from notebook if user did not provide one.
     if base_image_name is None:
-        # If a user is using a custom image uri, base_image_name might be None
-        notebook_metadata = get_notebook_metadata(notebook_path)
+        # If a user is using a custom image uri, base_image_name might be None.
         base_image_name = notebook_metadata.notebook_image_name
 
+    # Check for global notebook doi from notebook if user did not provide one.
+    if global_notebook_doi is None:
+        global_notebook_doi = notebook_metadata.global_notebook_doi
+
     # Update garden metadata in notebook
     set_notebook_metadata(
-        notebook_path, base_image_name, base_image_uri, requirements_data
+        notebook_path,
+        global_notebook_doi,
+        base_image_name,
+        base_image_uri,
+        requirements_data,
     )
 
     print(
         f"Starting notebook inside base image with full name {base_image_uri}. "
         f"If you start this notebook again from the same folder, it will use this image by default."
     )
 
@@ -331,51 +345,60 @@
         base_image_uri = (
             _get_base_image_uri(
                 base_image_name=None, custom_image_uri=None, notebook_path=path
             )
             or "gardenai/base:python-3.10-base"
         )
 
+        notebook_metadata = get_notebook_metadata(path)
+
         # Validate and read requirements file.
         if requirements_path:
             _validate_requirements_path(requirements_path)
             requirements_data = read_requirements_data(requirements_path)
         else:
-            # If no requirements file given, look for requirements data in notebook
-            requirements_data = get_notebook_metadata(path).notebook_requirements
+            # If no requirements file given, look for requirements data in notebook metadata
+            requirements_data = notebook_metadata.notebook_requirements
 
-        base_image_name = get_notebook_metadata(path).notebook_image_name
+        base_image_name = notebook_metadata.notebook_image_name
         if base_image_name is None:
             base_image_name = "3.10-base"
+        global_notebook_doi = notebook_metadata.global_notebook_doi
 
         with TemporaryDirectory() as temp_dir:
             # pre-bake local image with garden-ai and additional user requirements
             local_base_image_id = build_image_with_dependencies(
                 docker_client, base_image_uri, requirements_data
             )
 
+            # pass global notebook doi to image as env_var
             image = build_notebook_session_image(
                 docker_client,
                 path,
                 local_base_image_id,
+                env_vars={"GLOBAL_NOTEBOOK_DOI": global_notebook_doi},
             )
 
             if image is None:
                 typer.echo("Failed to build image.")
                 raise typer.Exit(1)
             image_name = str(image.id)  # str used to guarantee type-check
 
             top_level_dir = Path(__file__).parent.parent
             debug_path = top_level_dir / "notebook_templates" / "debug.ipynb"
 
-            # Make tmp copy of debug notebook to add original notebook's metadata too
+            # Make tmp copy of debug notebook template to add original notebook's metadata too
             temp_debug_path = Path(temp_dir) / "debug.ipynb"
             shutil.copy(debug_path, temp_debug_path)
             set_notebook_metadata(
-                temp_debug_path, base_image_name, base_image_uri, requirements_data
+                temp_debug_path,
+                global_notebook_doi,
+                base_image_name,
+                base_image_uri,
+                requirements_data,
             )
 
             container = start_container_with_notebook(
                 docker_client, temp_debug_path, image_name, mount=False, pull=False
             )
             _register_container_sigint_handler(container)
 
@@ -429,14 +452,23 @@
         "--base-image",
         help=(
             "A Garden base image to run your notebook inside of. This will be the foundation for the image that runs your entrypoints."
             "For example, to run on top of the default Garden python 3.8 image, use --base-image 3.8-base. "
             "To see all the available Garden base images, use 'garden-ai notebook list-premade-images'"
         ),
     ),
+    global_notebook_doi: Optional[str] = typer.Option(
+        None,
+        "--doi",
+        help=(
+            "DOI of a Garden you want to publish all entrypoints in this notebook too. "
+            "To override the global notebook DOI for a specific entrypoint, "
+            "provide the garden_entrypoint decorator with the optional garden_doi argument."
+        ),
+    ),
     custom_image_uri: Optional[str] = typer.Option(
         None,
         "--custom-image",
         help=(
             "Power users only! Provide a uri of a publicly available docker image to boot the notebook in."
         ),
         hidden=True,
@@ -452,44 +484,51 @@
     client = GardenClient()
     notebook_path = path.resolve()
     if notebook_path.suffix != ".ipynb":
         raise ValueError("File must be a jupyter notebook (.ipynb)")
     if not notebook_path.exists():
         raise ValueError(f"Could not find file at {notebook_path}")
 
-    # Publish should not change the metadata of users local notebook if user provided different requirements / base image.
-    # So we use a tmpdir with a copy of the original notebook for publish.
+    # Use tmpdir and make a copy of original notebook, since publish should not modify
+    # the original notebook if provided with any new arguments.
     with TemporaryDirectory() as temp_dir:
         temp_dir_path = Path(temp_dir)
         tmp_notebook_path = temp_dir_path / notebook_path.name
         shutil.copy(notebook_path, tmp_notebook_path)
 
         base_image_uri = _get_base_image_uri(
             base_image_name, custom_image_uri, tmp_notebook_path
         )
         print(f"Using base image: {base_image_uri}")
 
+        notebook_metadata = get_notebook_metadata(tmp_notebook_path)
         # Validate and read requirements file.
         if requirements_path:
             _validate_requirements_path(requirements_path)
             requirements_data = read_requirements_data(requirements_path)
         else:
-            # If no requirements file given, look for requirements data in notebook
-            requirements_data = get_notebook_metadata(
-                tmp_notebook_path
-            ).notebook_requirements
+            # If no requirements file given, look for requirements data in notebook metadata
+            requirements_data = notebook_metadata.notebook_requirements
 
-        # Get base image name from notebook if user did not provide
+        # Check for base image name from notebook if user did not provide one.
         if base_image_name is None:
             # If a user is using a custom image uri, base_image_name might be None
-            base_image_name = get_notebook_metadata(notebook_path).notebook_image_name
+            base_image_name = notebook_metadata.notebook_image_name
+
+        # Check for global notebook doi from notebook if user did not provide one.
+        if global_notebook_doi is None:
+            global_notebook_doi = notebook_metadata.global_notebook_doi
 
-        # Update garden metadata in new tmp notebook
+        # Update the tmp notebooks metadata with any new publish args
         set_notebook_metadata(
-            tmp_notebook_path, base_image_name, base_image_uri, requirements_data
+            tmp_notebook_path,
+            global_notebook_doi,
+            base_image_name,
+            base_image_uri,
+            requirements_data,
         )
 
         # Pre-process the notebook and make sure it's not too big
         raw_notebook_contents = tmp_notebook_path.read_text()
         try:
             notebook_contents = json.loads(raw_notebook_contents)
         except json.JSONDecodeError:
@@ -517,14 +556,15 @@
             )
 
             image = build_notebook_session_image(
                 docker_client,
                 tmp_notebook_path,
                 local_base_image_id,
                 print_logs=verbose,
+                env_vars={"GLOBAL_NOTEBOOK_DOI": global_notebook_doi},
             )
 
             if image is None:
                 typer.echo("Failed to build image.")
                 raise typer.Exit(1)
             typer.echo(f"Built image: {image}")
 
@@ -551,16 +591,16 @@
     # First make sure that we have enough information to get a base image uri
     if base_image_name and custom_image_uri:
         typer.echo(
             "You specified both a base image and a custom image. Please specify only one."
         )
         raise typer.Exit(1)
 
+    # Check for saved_image_name in notebooks metadata
     if notebook_path:
-        # saved_image_name could also be None here if not set in the notebooks metadata
         saved_image_name = get_notebook_metadata(notebook_path).notebook_image_name
     else:
         saved_image_name = None
 
     if not any([base_image_name, custom_image_uri, saved_image_name]):
         typer.echo(
             f"Please specify a base image. The current Garden base images are: \n{BASE_IMAGE_NAMES}"
```

### Comparing `garden_ai-2.0.0/garden_ai/backend_client.py` & `garden_ai-2.0.1/garden_ai/backend_client.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/client.py` & `garden_ai-2.0.1/garden_ai/client.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/constants.py` & `garden_ai-2.0.1/garden_ai/constants.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/containers.py` & `garden_ai-2.0.1/garden_ai/containers.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/datacite.py` & `garden_ai-2.0.1/garden_ai/datacite.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/entrypoints.py` & `garden_ai-2.0.1/garden_ai/entrypoints.py`

 * *Files 13% similar despite different names*

```diff
@@ -144,27 +144,29 @@
             You can promote a DOI to a registered state with `garden-ai entrypoint register-doi`.
         container_uuid: ID returned from Globus Compute's register_container.
         base_image_uri: location of the base image used by this entrypoint. eg docker://index.docker.io/maxtuecke/garden-ai:python-3.9-jupyter
         full_image_uri: The name and location of the complete image used by this entrypoint.
         notebook_url: Link to the notebook used to build this entrypoint.
         steps: Ordered list of Python functions that the entrypoint author wants to highlight.
         test_functions: List of test functions that exercise the entrypoint.
+        requirements: List of Python packages required by the entrypoint.
     """
 
     doi: str = Field(
         ...
     )  # Repeating this field from base class because DOI is mandatory for RegisteredEntrypoint
     doi_is_draft: bool = Field(True)
     func_uuid: UUID = Field(...)
     container_uuid: UUID = Field(...)
     base_image_uri: Optional[str] = Field(None)
     full_image_uri: Optional[str] = Field(None)
     notebook_url: Optional[str] = Field(None)
     steps: List[Step] = Field(default_factory=list)
     test_functions: List[str] = Field(default_factory=list)
+    requirements: Optional[List[str]] = Field(default_factory=list)
 
     def __call__(
         self,
         *args: Any,
         endpoint: Union[UUID, str] = None,
         **kwargs: Any,
     ) -> Any:
@@ -270,39 +272,50 @@
         We know their DOIs. We can use this to check if a DOI is a DLHub entrypoint.
         If so, we convert the user's input into the format that DLHub models expect.
         We also just pass along the model output to the user and strip the rest.
         """
         return self.doi in GardenConstants.DLHUB_DOIS
 
 
+class EntrypointIdempotencyError(Exception):
+    """Raised when an entrypoint function is found to be non-idempotent."""
+
+    pass
+
+
 def garden_entrypoint(
     metadata: EntrypointMetadata,
     garden_doi: str = None,
     model_connectors: Optional[List] = None,
     datasets: Optional[List[DatasetConnection]] = None,
 ):
     def decorate(func):
+        # If the user is lazy and uses same EntrypointMetadata object for multiple entrypoints,
+        # garden ends up writing over the metadata of the single EntrypointMetadata object for each entrypoint.
+        # Dirty fix for this is recreating new EntrypointMetadata object.
+        entrypoint_metadata = metadata.copy(deep=True)
+
         if datasets:
             # datasets explicitly connected to entrypoint by decorator
-            metadata.datasets += datasets
+            entrypoint_metadata.datasets += datasets
         if model_connectors:
             for connector in model_connectors:
                 model_meta: ModelMetadata = connector.metadata
-                metadata.models += [model_meta]
+                entrypoint_metadata.models += [model_meta]
                 # datasets implicitly connected from model metadata
-                metadata.datasets += model_meta.datasets
+                entrypoint_metadata.datasets += model_meta.datasets
 
-        metadata._as_step = Step(
+        entrypoint_metadata._as_step = Step(
             function_text=inspect.getsource(func),
             function_name=func.__name__,
             description="Top level entrypoint function",
         )
-        metadata._target_garden_doi = garden_doi
+        entrypoint_metadata._target_garden_doi = garden_doi
         # let func carry its own metadata
-        func._garden_entrypoint = metadata
+        func._garden_entrypoint = entrypoint_metadata
         return func
 
     return decorate
 
 
 def entrypoint_test(entrypoint_func: Callable):
     """Mark a function as a 'test function' of an entrypoint.
@@ -321,14 +334,18 @@
         def test_my_entrypoint():
             ...
             results = my_entrypoint(...)
             ...
             return results
 
         ```
+
+    Raises:
+        EntrypointIdempotencyError: When entrypoint_func is found to be non-idempotent, i.e. It cannot be called twice
+            without errors.
     """
     if not entrypoint_func or not entrypoint_func._garden_entrypoint:  # type: ignore
         raise ValueError("Please pass in a valid entrypoint function")
 
     def decorate(test_func):
         test_function_text = inspect.getsource(test_func)
         entrypoint_func._garden_entrypoint._test_functions.append(test_function_text)
@@ -338,15 +355,47 @@
             import os
 
             # this flag is set during publication time in
             # containers.build_notebook_session_image
             if os.environ.get("GARDEN_SKIP_TESTS") == str(True):
                 return None
             else:
-                return test_func(*args, **kwargs)
+                import importlib.util
+
+                # call the test_func once
+                result = test_func(*args, **kwargs)
+
+                # Call the test_func again with the same args to enforce idempotency.
+                if importlib.util.find_spec("numpy") is not None:
+                    import numpy  # type: ignore
+
+                    if isinstance(result, numpy.ndarray):
+                        if numpy.array_equal(
+                            result, test_func(*args, **kwargs), equal_nan=True
+                        ):
+                            return result
+                        else:
+                            raise EntrypointIdempotencyError(
+                                "Please ensure your entrypoint can be called more than once without errors."
+                            )
+                if importlib.util.find_spec("pandas") is not None:
+                    import pandas  # type: ignore
+
+                    if isinstance(result, pandas.DataFrame):
+                        if result.equals(test_func(*args, **kwargs)):
+                            return result
+                        else:
+                            raise EntrypointIdempotencyError(
+                                "Please ensure your entrypoint can be called more than once without errors."
+                            )
+                if result != test_func(*args, **kwargs):
+                    raise EntrypointIdempotencyError(
+                        "Please ensure your entrypoint can be called more than once without errors."
+                    )
+                return result
 
         return inner
 
     return decorate
 
 
 def garden_step(description: str = None):
```

### Comparing `garden_ai-2.0.0/garden_ai/garden_file_adapter.py` & `garden_ai-2.0.1/garden_ai/garden_file_adapter.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/gardens.py` & `garden_ai-2.0.1/garden_ai/gardens.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/globus_search/garden_search.py` & `garden_ai-2.0.1/garden_ai/globus_search/garden_search.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/local_data.py` & `garden_ai-2.0.1/garden_ai/local_data.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/mlmodel.py` & `garden_ai-2.0.1/garden_ai/mlmodel.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/model_connectors/hugging_face.py` & `garden_ai-2.0.1/garden_ai/model_connectors/hugging_face.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import huggingface_hub as hfh  # type: ignore
 from garden_ai.mlmodel import ModelMetadata
 from garden_ai.utils.misc import trackcalls
 from requests.exceptions import HTTPError
 import os
 import sys
 
+from .exceptions import ConnectorInvalidRevisionError
+
 
 class HFConnector:
     def __init__(
         self, repo_id: str, revision=None, local_dir=None, enable_imports=True
     ):
         self.repo_id = repo_id
         self.revision = revision
@@ -21,19 +23,34 @@
         )
         try:
             # This fetches README.md from the repo and will raise an error if it doesn't exist
             self.model_card = hfh.ModelCard.load(repo_id)
         except HTTPError:
             self.model_card = None
 
+        # Grab the model revision from the main branch if it wasn't provided.
+        if self.revision is None:
+            try:
+                refs = hfh.list_repo_refs(self.repo_id)
+                for branch in refs.branches:
+                    if branch.name == "main":
+                        self.revision = branch.target_commit
+                        self.metadata.model_version = self.revision
+                assert self.revision is not None
+            except Exception as e:
+                # just pass along any error message, the list_repo_refs exceptions have helpful messages
+                raise ConnectorInvalidRevisionError(e)
+
     @trackcalls
     def stage(self) -> str:
         if not os.path.exists(self.local_dir):
             os.mkdir(self.local_dir)
-        hfh.snapshot_download(self.repo_id, local_dir=self.local_dir)
+        hfh.snapshot_download(
+            self.repo_id, revision=self.revision, local_dir=self.local_dir
+        )
         if self.enable_imports:
             sys.path.append(self.local_dir)
         return self.local_dir
 
     def _repr_html_(self):
         if not self.model_card:
             return ""
```

### Comparing `garden_ai-2.0.0/garden_ai/notebook_metadata.py` & `garden_ai-2.0.1/garden_ai/notebook_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 class RequirementsData(NamedTuple):
     file_format: str
     contents: Union[dict, list]
 
 
 class NotebookMetadata(NamedTuple):
+    global_notebook_doi: Optional[str]
     notebook_image_name: Optional[str]
     notebook_image_uri: Optional[str]
     notebook_requirements: Optional[RequirementsData]
 
 
 def add_notebook_metadata_cell(
     notebook_path: Path,
@@ -42,15 +43,20 @@
         if "garden_metadata_cell" in cell_tags:
             # if cell exists, exit here, don't need to add again.
             return
 
     # Was unable to find cell with garden_metadata_cell tag, add new one to top of notebook
     # notebook_image_uri can be None here since notebook start will require the user provided a base image.
     metadata_string = json.dumps(
-        {"NOTEBOOK_BASE_IMAGE_NAME": None, "NOTEBOOK_REQUIREMENTS": None}, indent=2
+        {
+            "NOTEBOOK_GLOBAL_DOI": None,
+            "NOTEBOOK_BASE_IMAGE_NAME": None,
+            "NOTEBOOK_REQUIREMENTS": None,
+        },
+        indent=2,
     )
     notebook_metadata = NOTEBOOK_METADATA_CELL_TEMPLATE.substitute(
         metadata=metadata_string
     )
 
     # Add new cell with garden_metadata_cell tag to top of notebook
     new_cell = nbformat.v4.new_code_cell(notebook_metadata)
@@ -80,24 +86,26 @@
                 "garden_metadata", {}
             )
             break
 
     # Return empty notebook metadata dict if was unable to find cell source
     if not notebook_metadata_cell_source:
         typer.echo("Unable to find garden metadata cell.")
-        return NotebookMetadata(None, None, None)
+        return NotebookMetadata(None, None, None, None)
 
     # Grab the part of cell source with the metadata dict in it
     clean_source = notebook_metadata_cell_source.replace("\n", "")
     regex_get_metadata = r"^(.*?)\"\"\"(.*?)NOTEBOOK_METADATA(.*?)=(.*?)\"\"\"(.*?)$"
 
     metadata_match = re.match(regex_get_metadata, clean_source)
     if metadata_match and len(metadata_match.groups()) == 5:
         notebook_metadata_dict = json.loads(metadata_match[4].strip())
 
+        notebook_global_doi = notebook_metadata_dict.get("NOTEBOOK_GLOBAL_DOI", None)
+
         notebook_image_name = notebook_metadata_dict.get(
             "NOTEBOOK_BASE_IMAGE_NAME", None
         )
 
         notebook_image_uri = notebook_hidden_metadata.get(
             "NOTEBOOK_BASE_IMAGE_URI", None
         )
@@ -106,23 +114,27 @@
             "NOTEBOOK_REQUIREMENTS", None
         )
         notebook_requirements = None
         if notebook_requirements_dict:
             notebook_requirements = RequirementsData(**notebook_requirements_dict)
 
         return NotebookMetadata(
-            notebook_image_name, notebook_image_uri, notebook_requirements
+            notebook_global_doi,
+            notebook_image_name,
+            notebook_image_uri,
+            notebook_requirements,
         )
     else:
         typer.echo("Unable to parse garden metadata cell.")
-        return NotebookMetadata(None, None, None)
+        return NotebookMetadata(None, None, None, None)
 
 
 def set_notebook_metadata(
     notebook_path: Path,
+    notebook_global_doi: Optional[str],
     base_image_name: Optional[str],
     base_image_uri: str,
     requirements_data: Optional[RequirementsData],
 ):
     ntbk = _read_notebook(notebook_path)
 
     # Find cell with 'garden_metadata_cell' tag
@@ -131,14 +143,15 @@
         if "garden_metadata_cell" in cell_tags:
             # Replace old cell source with new metadata
             requirements_data_dict = (
                 requirements_data._asdict() if requirements_data is not None else None
             )
             metadata_string = json.dumps(
                 {
+                    "NOTEBOOK_GLOBAL_DOI": notebook_global_doi,
                     "NOTEBOOK_BASE_IMAGE_NAME": base_image_name,
                     "NOTEBOOK_REQUIREMENTS": requirements_data_dict,
                 },
                 indent=2,
             )
 
             cell["source"] = NOTEBOOK_METADATA_CELL_TEMPLATE.substitute(
```

### Comparing `garden_ai-2.0.0/garden_ai/notebook_templates/debug.ipynb` & `garden_ai-2.0.1/garden_ai/notebook_templates/debug.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999810606060606%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(6, \'  "NOTEBOOK_GLOBAL_DOI": null,\\n\')]}}}'}*

```diff
@@ -15,14 +15,15 @@
             "source": [
                 "# This cell is auto-generated by Garden. Don't delete it. Do keep it as the first cell.\n",
                 "# It records the base image and requirements you passed to `garden-ai notebook start`.\n",
                 "# That way the next time you run this notebook Garden can start it with the same libraries.\n",
                 "\n",
                 "\"\"\"\n",
                 "NOTEBOOK_METADATA = {\n",
+                "  \"NOTEBOOK_GLOBAL_DOI\": null,\n",
                 "  \"NOTEBOOK_BASE_IMAGE_NAME\": \"3.9-base\",\n",
                 "  \"NOTEBOOK_REQUIREMENTS\": null\n",
                 "}\n",
                 "\"\"\""
             ]
         },
         {
```

### Comparing `garden_ai-2.0.0/garden_ai/notebook_templates/empty.ipynb` & `garden_ai-2.0.1/garden_ai/notebook_templates/empty.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994318181818183%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(6, \'  "NOTEBOOK_GLOBAL_DOI": null,\\n\')]}}}'}*

```diff
@@ -15,14 +15,15 @@
             "source": [
                 "# This cell is auto-generated by Garden. Don't delete it. Do keep it as the first cell.\n",
                 "# It records the base image and requirements you passed to `garden-ai notebook start`.\n",
                 "# That way the next time you run this notebook Garden can start it with the same libraries.\n",
                 "\n",
                 "\"\"\"\n",
                 "NOTEBOOK_METADATA = {\n",
+                "  \"NOTEBOOK_GLOBAL_DOI\": null,\n",
                 "  \"NOTEBOOK_BASE_IMAGE_NAME\": \"3.9-base\",\n",
                 "  \"NOTEBOOK_REQUIREMENTS\": null\n",
                 "}\n",
                 "\"\"\""
             ]
         },
         {
```

### Comparing `garden_ai-2.0.0/garden_ai/notebook_templates/sklearn.ipynb` & `garden_ai-2.0.1/garden_ai/notebook_templates/sklearn.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9968162593984963%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(6, \'  "NOTEBOOK_GLOBAL_DOI": null,\\n\'), (11, \'      '*

 * *            '"scikit-learn==1.4.1",\\n\')], delete: [10]}}, 3: {\'source\': {insert: [(2, \'import '*

 * *            "numpy as np\\n')]}}, 5: {'source': ['my_hugging_face_repo = "*

 * *            'HFConnector("garden-ai/sklearn-iris")\']}, 10: {\'source\': {insert: [(8, \'\\n\'), '*

 * *            "(9, 'You can add your entrypoint to a Garden in two different ways.\\n'), (10, "*

 * *            "'\\n'), (11, 'If you want all e […]*

```diff
@@ -15,19 +15,20 @@
             "source": [
                 "# This cell is auto-generated by Garden. Don't delete it. Do keep it as the first cell.\n",
                 "# It records the base image and requirements you passed to `garden-ai notebook start`.\n",
                 "# That way the next time you run this notebook Garden can start it with the same libraries.\n",
                 "\n",
                 "\"\"\"\n",
                 "NOTEBOOK_METADATA = {\n",
+                "  \"NOTEBOOK_GLOBAL_DOI\": null,\n",
                 "  \"NOTEBOOK_BASE_IMAGE_NAME\": \"3.9-sklearn\",\n",
                 "  \"NOTEBOOK_REQUIREMENTS\": {\n",
                 "    \"file_format\": \"pip\",\n",
                 "    \"contents\": [\n",
-                "      \"scikit-learn==1.2.2\",\n",
+                "      \"scikit-learn==1.4.1\",\n",
                 "      \"pandas\"\n",
                 "    ]\n",
                 "  }\n",
                 "}\n",
                 "\"\"\""
             ]
         },
@@ -62,14 +63,15 @@
             "metadata": {
                 "id": "b0s7Bealdp8M"
             },
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
                 "import sklearn\n",
+                "import numpy as np\n",
                 "import joblib"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "3aikfsCRdrEZ"
@@ -85,15 +87,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "H7em6SwMdvkt"
             },
             "outputs": [],
             "source": [
-                "my_hugging_face_repo = HFConnector(\"garden-ai/sample_sklearn_model\")"
+                "my_hugging_face_repo = HFConnector(\"garden-ai/sklearn-iris\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "FTziKOq7d1Qs"
             },
@@ -155,30 +157,39 @@
                 "\n",
                 "The `@garden_entrypoint` decorator makes this function available to run in your garden when you publish the notebook.\n",
                 "Download your model weights and call your model in this function.\n",
                 "\n",
                 "In the decorator be sure to include:\n",
                 "- your entrypoint metadata,\n",
                 "- connectors for any models you're using,\n",
-                "- the DOI of the garden you want this entrypoint to be found in. (Check `garden-ai garden list` for the DOIs of your gardens.)"
+                "\n",
+                "You can add your entrypoint to a Garden in two different ways.\n",
+                "\n",
+                "If you want all entrypoints in this notebook be added to one Garden, set the `NOTEBOOK_GLOBAL_DOI` in your notebooks metadata or by using the `--doi` argument for `garden-ai notebook start`\n",
+                "\n",
+                "If you want to specify different Gardens for different entrypoints, provide each decorator with the optional `garden_doi` argument.\n",
+                "\n",
+                "If you both set the `NOTEBOOK_GLOBAL_DOI` and are providing a decorator with a DOI, the entrypoint will ONLY be added to the Garden given to the decorator.\n",
+                "\n",
+                "To see all the DOIs of your gardens, use `garden-ai garden list`"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "6ls-44Wehec9"
             },
             "outputs": [],
             "source": [
                 "@garden_entrypoint(metadata=my_entrypoint_meta,  model_connectors=[my_hugging_face_repo], garden_doi=\"10.23677/my-garden-doi\")\n",
-                "def run_my_model(input_df: pd.DataFrame) -> pd.DataFrame:\n",
+                "def run_my_model(input_df: pd.DataFrame) -> np.ndarray:\n",
                 "    cleaned_df = preprocess(input_df)\n",
                 "    download_path = my_hugging_face_repo.stage()\n",
-                "    model = joblib.load(f\"{download_path}/model.pkl\")\n",
+                "    model = joblib.load(f\"{download_path}/model.joblib\")\n",
                 "    return model.predict(cleaned_df)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "dK3PHq2fhgxp"
@@ -204,19 +215,22 @@
                 "id": "A9-UTFHAmCEq"
             },
             "outputs": [],
             "source": [
                 "@entrypoint_test(run_my_model)\n",
                 "def test_run_my_model():\n",
                 "    # Replace with input that is relevant for your garden_entrypoint\n",
-                "    example_input = pd.DataFrame({\n",
-                "        'A': [1, 2, None, 4],\n",
-                "        'B': [None, 2, 3, 4],\n",
-                "        'C': [1, 2, 3, 4]\n",
-                "    })\n",
+                "    data = [\n",
+                "        [5.5, 2.4, 3.7, 1. ],\n",
+                "        [6.3, 2.8, 5.1, 1.5],\n",
+                "        [6.4, 3.1, 5.5, 1.8],\n",
+                "        [6.6, 3. , 4.4, 1.4],\n",
+                "    ]\n",
+                "\n",
+                "    example_input = pd.DataFrame(data, columns = ['sepal_length', 'sepal_width', 'petal_length', 'petal_width']) \n",
                 "    return run_my_model(example_input)\n",
                 "    \n",
                 "test_run_my_model()"
             ]
         }
     ],
     "metadata": {
```

### Comparing `garden_ai-2.0.0/garden_ai/notebook_templates/tensorflow.ipynb` & `garden_ai-2.0.1/garden_ai/notebook_templates/tensorflow.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999057302346776%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(6, \'  "NOTEBOOK_GLOBAL_DOI": null,\\n\')]}}, 10: '*

 * *            "{'source': {insert: [(8, '\\n'), (9, 'You can add your entrypoint to a Garden in two "*

 * *            "different ways.\\n'), (10, '\\n'), (11, 'If you want all entrypoints in this notebook "*

 * *            'be added to one Garden, set the `NOTEBOOK_GLOBAL_DOI` in your notebooks metadata or '*

 * *            "by using the `--doi` argument for `garden-ai notebook start`\\n'), (12, '\\n'), (13, "*

 * *            "'If yo […]*

```diff
@@ -15,14 +15,15 @@
             "source": [
                 "# This cell is auto-generated by Garden. Don't delete it. Do keep it as the first cell.\n",
                 "# It records the base image and requirements you passed to `garden-ai notebook start`.\n",
                 "# That way the next time you run this notebook Garden can start it with the same libraries.\n",
                 "\n",
                 "\"\"\"\n",
                 "NOTEBOOK_METADATA = {\n",
+                "  \"NOTEBOOK_GLOBAL_DOI\": null,\n",
                 "  \"NOTEBOOK_BASE_IMAGE_NAME\": \"3.9-tensorflow\",\n",
                 "  \"NOTEBOOK_REQUIREMENTS\": null\n",
                 "}\n",
                 "\"\"\""
             ]
         },
         {
@@ -152,15 +153,24 @@
                 "\n",
                 "The `@garden_entrypoint` decorator makes this function available to run in your garden when you publish the notebook.\n",
                 "Download your model weights and call your model in this function.\n",
                 "\n",
                 "In the decorator be sure to include:\n",
                 "- your entrypoint metadata,\n",
                 "- connectors for any models you're using,\n",
-                "- the DOI of the garden you want this entrypoint to be found in. (Check `garden-ai garden list` for the DOIs of your gardens.)"
+                "\n",
+                "You can add your entrypoint to a Garden in two different ways.\n",
+                "\n",
+                "If you want all entrypoints in this notebook be added to one Garden, set the `NOTEBOOK_GLOBAL_DOI` in your notebooks metadata or by using the `--doi` argument for `garden-ai notebook start`\n",
+                "\n",
+                "If you want to specify different Gardens for different entrypoints, provide each decorator with the optional `garden_doi` argument.\n",
+                "\n",
+                "If you both set the `NOTEBOOK_GLOBAL_DOI` and are providing a decorator with a DOI, the entrypoint will ONLY be added to the Garden given to the decorator.\n",
+                "\n",
+                "To see all the DOIs of your gardens, use `garden-ai garden list`"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "6ls-44Wehec9"
```

### Comparing `garden_ai-2.0.0/garden_ai/notebook_templates/torch.ipynb` & `garden_ai-2.0.1/garden_ai/notebook_templates/torch.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999120148856991%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(6, \'  "NOTEBOOK_GLOBAL_DOI": null,\\n\')]}}, 10: '*

 * *            "{'source': {insert: [(8, '\\n'), (9, 'You can add your entrypoint to a Garden in two "*

 * *            "different ways.\\n'), (10, '\\n'), (11, 'If you want all entrypoints in this notebook "*

 * *            'be added to one Garden, set the `NOTEBOOK_GLOBAL_DOI` in your notebooks metadata or '*

 * *            "by using the `--doi` argument for `garden-ai notebook start`\\n'), (12, '\\n'), (13, "*

 * *            "'If yo […]*

```diff
@@ -15,14 +15,15 @@
             "source": [
                 "# This cell is auto-generated by Garden. Don't delete it. Do keep it as the first cell.\n",
                 "# It records the base image and requirements you passed to `garden-ai notebook start`.\n",
                 "# That way the next time you run this notebook Garden can start it with the same libraries.\n",
                 "\n",
                 "\"\"\"\n",
                 "NOTEBOOK_METADATA = {\n",
+                "  \"NOTEBOOK_GLOBAL_DOI\": null,\n",
                 "  \"NOTEBOOK_BASE_IMAGE_NAME\": \"3.9-torch\",\n",
                 "  \"NOTEBOOK_REQUIREMENTS\": null\n",
                 "}\n",
                 "\"\"\""
             ]
         },
         {
@@ -151,15 +152,24 @@
                 "\n",
                 "The `@garden_entrypoint` decorator makes this function available to run in your garden when you publish the notebook.\n",
                 "Download your model weights and call your model in this function.\n",
                 "\n",
                 "In the decorator be sure to include:\n",
                 "- your entrypoint metadata,\n",
                 "- connectors for any models you're using,\n",
-                "- the DOI of the garden you want this entrypoint to be found in. (Check `garden-ai garden list` for the DOIs of your gardens.)"
+                "\n",
+                "You can add your entrypoint to a Garden in two different ways.\n",
+                "\n",
+                "If you want all entrypoints in this notebook be added to one Garden, set the `NOTEBOOK_GLOBAL_DOI` in your notebooks metadata or by using the `--doi` argument for `garden-ai notebook start`\n",
+                "\n",
+                "If you want to specify different Gardens for different entrypoints, provide each decorator with the optional `garden_doi` argument.\n",
+                "\n",
+                "If you both set the `NOTEBOOK_GLOBAL_DOI` and are providing a decorator with a DOI, the entrypoint will ONLY be added to the Garden given to the decorator.\n",
+                "\n",
+                "To see all the DOIs of your gardens, use `garden-ai garden list`"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "6ls-44Wehec9"
```

### Comparing `garden_ai-2.0.0/garden_ai/notebook_templates/tutorial.ipynb` & `garden_ai-2.0.1/garden_ai/notebook_templates/tutorial.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999101881914382%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(6, \'  "NOTEBOOK_GLOBAL_DOI": null,\\n\')]}}, 5: '*

 * *            "{'source': {insert: [(2, 'import numpy as np\\n')]}}, 7: {'source': {insert: [(2, "*

 * *            '\'hf_iris_connector = HFConnector("Garden-AI/sklearn-iris")\\n\')], delete: [2]}}, '*

 * *            "15: {'source': {insert: [(2, '    data = [\\n'), (3, '        [5.5, 2.4, 3.7, 1. "*

 * *            "],\\n'), (4, '        [6.3, 2.8, 5.1, 1.5],\\n'), (5, '        [6.4, 3.1, 5.5, "*

 * *            "1.8],\\n'), (6, '      […]*

```diff
@@ -15,14 +15,15 @@
             "source": [
                 "# This cell is auto-generated by Garden. Don't delete it. Do keep it as the first cell.\n",
                 "# It records the base image and requirements you passed to `garden-ai notebook start`.\n",
                 "# That way the next time you run this notebook Garden can start it with the same libraries.\n",
                 "\n",
                 "\"\"\"\n",
                 "NOTEBOOK_METADATA = {\n",
+                "  \"NOTEBOOK_GLOBAL_DOI\": null,\n",
                 "  \"NOTEBOOK_BASE_IMAGE_NAME\": \"3.10-sklearn\",\n",
                 "  \"NOTEBOOK_REQUIREMENTS\": null\n",
                 "}\n",
                 "\"\"\""
             ]
         },
         {
@@ -63,14 +64,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
                 "import sklearn\n",
+                "import numpy as np\n",
                 "import joblib"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -83,15 +85,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# The model is at https://huggingface.co/Garden-AI/sklearn-seedling.\n",
                 "# You just need to pass in the {organization}/{repo name} part to the HFConnector constructor.\n",
-                "hf_iris_connector = HFConnector(\"Garden-AI/sklearn-seedling\")\n",
+                "hf_iris_connector = HFConnector(\"Garden-AI/sklearn-iris\")\n",
                 "\n",
                 "# Check out the model card associated with this repo as a sanity check\n",
                 "hf_iris_connector"
             ]
         },
         {
             "cell_type": "markdown",
@@ -194,19 +196,27 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "@entrypoint_test(classify_irises)\n",
                 "def test_the_classifier():\n",
-                "    example_input = [[5.1, 3.5, 1.4, 0.2]]\n",
+                "    data = [\n",
+                "        [5.5, 2.4, 3.7, 1. ],\n",
+                "        [6.3, 2.8, 5.1, 1.5],\n",
+                "        [6.4, 3.1, 5.5, 1.8],\n",
+                "        [6.6, 3. , 4.4, 1.4],\n",
+                "        [5.1, 3.5, 1.4, 0.2],\n",
+                "    ]\n",
+                "\n",
+                "    example_input = pd.DataFrame(data, columns = ['sepal_length', 'sepal_width', 'petal_length', 'petal_width']) \n",
                 "    result = classify_irises(example_input)\n",
                 "    return result\n",
                 "\n",
-                "# This should return a list with one string, ['setosa']\n",
+                "# This should return the list ['versicolor', 'virginica', 'virginica', 'versicolor', 'setosa']\n",
                 "test_the_classifier()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `garden_ai-2.0.0/garden_ai/utils/_meta.py` & `garden_ai-2.0.1/garden_ai/utils/_meta.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/utils/dois.py` & `garden_ai-2.0.1/garden_ai/utils/dois.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/utils/interactive_cli.py` & `garden_ai-2.0.1/garden_ai/utils/interactive_cli.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/utils/misc.py` & `garden_ai-2.0.1/garden_ai/utils/misc.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/garden_ai/utils/notebooks.py` & `garden_ai-2.0.1/garden_ai/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `garden_ai-2.0.0/pyproject.toml` & `garden_ai-2.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "garden-ai"
-version = "2.0.0" # placeholder
+version = "2.0.1" # placeholder
 description = "Garden: tools to simplify access to scientific AI advances."
 # note to contributors: feel free to add yourselves to this list 🌱
 maintainers = [
   "Globus Labs <labs@globus.org>",
   "Owen Price Skelly",
   "Will Engler",
   "Ben Blaiszik",
@@ -48,14 +48,18 @@
 types-tabulate = "^0.9.0.3"
 nbformat = "^5.9.2"
 docker = "^6.1.3"
 nbconvert = "^7.9.2"
 ipython = "<8.13"
 boto3 = "^1.29"
 boto3-stubs = "^1.29"
+urllib3 = [
+     {version = "<2", python = "<3.10"},
+     {version = "^2.2.1", python = ">=3.10"}
+]
 python-dotenv = "^1.0.1"
 
 [tool.poetry.scripts]
 garden-ai = "garden_ai.app.main:app"
 
 [tool.poetry.group.test]
 optional = true
@@ -63,14 +67,18 @@
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
 flake8 = "^5.0.4"
 mypy = "^0.981"
 numpy = "^1.24.0"
+pandas = [
+     {version = "2.0.3", python = "<3.9"},
+     {version = "^2", python = ">=3.9"}
+]
 types-requests = "^2.20.0"
 safety = "^2.3.1"
 types-pyyaml = "^6.0.12.8"
 coverage = { extras = ["toml"], version = "^7.2.3" }
 
 [tool.poetry.group.develop.dependencies]
 pre-commit = "^3.1.1"
```

### Comparing `garden_ai-2.0.0/PKG-INFO` & `garden_ai-2.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garden-ai
-Version: 2.0.0
+Version: 2.0.1
 Summary: Garden: tools to simplify access to scientific AI advances.
 Home-page: https://thegardens.ai
 License: MIT
 Author: Garden Team
 Author-email: labs@globus.org
 Maintainer: Globus Labs
 Maintainer-email: labs@globus.org
@@ -34,14 +34,16 @@
 Requires-Dist: pydantic (>=1.10.13,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.20.0,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
 Requires-Dist: types-tabulate (>=0.9.0.3,<0.10.0.0)
+Requires-Dist: urllib3 (<2) ; python_version < "3.10"
+Requires-Dist: urllib3 (>=2.2.1,<3.0.0) ; python_version >= "3.10"
 Project-URL: Documentation, https://garden-ai.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Garden-AI/garden
 Description-Content-Type: text/markdown
 
 # Garden
 
 [![NSF-2209892](https://img.shields.io/badge/NSF-2209892-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2209892&HistoricalAwards=false)
```

