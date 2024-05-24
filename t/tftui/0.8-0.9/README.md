# Comparing `tmp/tftui-0.8.tar.gz` & `tmp/tftui-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tftui-0.8.tar", last modified: Sun Nov  5 13:11:56 2023, max compression
+gzip compressed data, was "tftui-0.9.tar", last modified: Sun Dec  3 06:19:09 2023, max compression
```

## Comparing `tftui-0.8.tar` & `tftui-0.9.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 13:11:56.083074 tftui-0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-05 13:11:38.000000 tftui-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-05 13:11:38.000000 tftui-0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16463 2023-11-05 13:11:56.079074 tftui-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2023-11-05 13:11:38.000000 tftui-0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-11-05 13:11:38.000000 tftui-0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-05 13:11:56.083074 tftui-0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 13:11:56.075074 tftui-0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 13:11:56.079074 tftui-0.8/src/tftui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-05 13:11:38.000000 tftui-0.8/src/tftui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16336 2023-11-05 13:11:38.000000 tftui-0.8/src/tftui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-11-05 13:11:38.000000 tftui-0.8/src/tftui/ui.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 13:11:56.079074 tftui-0.8/src/tftui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16463 2023-11-05 13:11:56.000000 tftui-0.8/src/tftui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-11-05 13:11:56.000000 tftui-0.8/src/tftui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-05 13:11:56.000000 tftui-0.8/src/tftui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-11-05 13:11:56.000000 tftui-0.8/src/tftui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-11-05 13:11:56.000000 tftui-0.8/src/tftui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-05 13:11:56.000000 tftui-0.8/src/tftui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 06:19:09.581199 tftui-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-03 06:18:56.000000 tftui-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-03 06:18:56.000000 tftui-0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16731 2023-12-03 06:19:09.581199 tftui-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2023-12-03 06:18:56.000000 tftui-0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2023-12-03 06:18:56.000000 tftui-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-03 06:19:09.581199 tftui-0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 06:19:09.577199 tftui-0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 06:19:09.581199 tftui-0.9/src/tftui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 06:18:56.000000 tftui-0.9/src/tftui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13266 2023-12-03 06:18:56.000000 tftui-0.9/src/tftui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-12-03 06:18:56.000000 tftui-0.9/src/tftui/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2023-12-03 06:18:56.000000 tftui-0.9/src/tftui/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2023-12-03 06:18:56.000000 tftui-0.9/src/tftui/ui.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 06:19:09.581199 tftui-0.9/src/tftui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16731 2023-12-03 06:19:09.000000 tftui-0.9/src/tftui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2023-12-03 06:19:09.000000 tftui-0.9/src/tftui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-03 06:19:09.000000 tftui-0.9/src/tftui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-03 06:19:09.000000 tftui-0.9/src/tftui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2023-12-03 06:19:09.000000 tftui-0.9/src/tftui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-03 06:19:09.000000 tftui-0.9/src/tftui.egg-info/top_level.txt
```

### Comparing `tftui-0.8/LICENSE` & `tftui-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tftui-0.8/PKG-INFO` & `tftui-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tftui
-Version: 0.8
+Version: 0.9
 Summary: Terraform Textual User Interface
 Author: Ido Avraham
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -213,27 +213,35 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: textual>=0.32.0
 Requires-Dist: textual-dev
 Requires-Dist: posthog>=3.0.2
 Requires-Dist: requests>=2.31.0
+Requires-Dist: pyperclip>=1.8.2
 
 # TFTUI - The Terraform textual UI
 
 [![PyPI version](https://badge.fury.io/py/tftui.svg?random=stuff)](https://badge.fury.io/py/tftui?)
 ![GitHub](https://img.shields.io/github/license/idoavrah/terraform-tui?random=stuff)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/tftui?random=stuff)
 
 `TFTUI` is a powerful textual GUI that empowers users to effortlessly view and interact with their Terraform state.
 
 With its latest version you can easily visualize the complete state tree, gaining deeper insights into your infrastructure's current configuration. Additionally, the ability to inspect individual resource states allows you to focus on specific details for better analysis and management. Lastly, it's now possible to select resources and perform actions such as tainting and untainting.
 
 ## Key Features
 
+### version 0.9
+
+- [x] Improved search functionality (now showing only matching resources)
+- [x] Improved the tainted resources display
+- [x] Added a copy to clipboard option (press `c` to copy)
+- [x] Major refactoring of the codebase
+
 ### version 0.8
 
 - [x] Added a delete resource option
 
 ### version 0.7
 
 - [x] Added a search option (press `/` to search)
```

### Comparing `tftui-0.8/README.md` & `tftui-0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 
 `TFTUI` is a powerful textual GUI that empowers users to effortlessly view and interact with their Terraform state.
 
 With its latest version you can easily visualize the complete state tree, gaining deeper insights into your infrastructure's current configuration. Additionally, the ability to inspect individual resource states allows you to focus on specific details for better analysis and management. Lastly, it's now possible to select resources and perform actions such as tainting and untainting.
 
 ## Key Features
 
+### version 0.9
+
+- [x] Improved search functionality (now showing only matching resources)
+- [x] Improved the tainted resources display
+- [x] Added a copy to clipboard option (press `c` to copy)
+- [x] Major refactoring of the codebase
+
 ### version 0.8
 
 - [x] Added a delete resource option
 
 ### version 0.7
 
 - [x] Added a search option (press `/` to search)
```

### Comparing `tftui-0.8/pyproject.toml` & `tftui-0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tftui"
-version = "0.8"
+version = "0.9"
 description = "Terraform Textual User Interface"
 readme = "README.md"
 authors = [{ name = "Ido Avraham" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
@@ -16,14 +16,15 @@
 ]
 keywords = ["terraform", "tui"]
 dependencies = [
     "textual>=0.32.0",
     "textual-dev",
     "posthog>=3.0.2",
     "requests>=2.31.0",
+    "pyperclip>=1.8.2",
 ]
 requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/idoavrah/terraform-tui"
 
 [project.scripts]
```

### Comparing `tftui-0.8/src/tftui/__main__.py` & `tftui-0.9/src/tftui/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,224 +1,176 @@
-import asyncio
 import argparse
-import uuid
-import importlib.metadata
-import requests
+import pyperclip
+from tftui.apis import OutboundAPIs
+from tftui.state import State, Block, execute_async
+from shutil import which
 from textual import work
-from textual.app import App, ComposeResult, Binding
+from textual.app import App, Binding
 from textual.containers import Vertical, Horizontal
-from shutil import which
-from posthog import Posthog
 from textual.widgets import (
     Header,
     Footer,
     Tree,
     Input,
     RichLog as TextLog,
     LoadingIndicator,
     ContentSwitcher,
     Static,
     Button,
 )
 
-version = importlib.metadata.version("tftui")
 global_no_init = False
 global_executable = "terraform"
 global_successful_termination = True
 
 
-class OutboundAPIs:
-    is_new_version_available = False
-    is_usage_tracking_enabled = True
-    session_id = uuid.uuid4()
-    posthog = Posthog(
-        project_api_key="phc_tjGzx7V6Y85JdNfOFWxQLXo5wtUs6MeVLvoVfybqz09",
-        host="https://app.posthog.com",
-        disable_geoip=False,
-    )
-
-    response = requests.get("https://pypi.org/pypi/tftui/json")
-    if response.status_code == 200:
-        ver = response.json()["info"]["version"]
-        if ver != version:
-            is_new_version_available = True
-
-    @staticmethod
-    def post_usage(message: str) -> None:
-        if OutboundAPIs.is_usage_tracking_enabled:
-            OutboundAPIs.posthog.capture(
-                OutboundAPIs.session_id, message, {"tftui_version": version}
-            )
-
-    @staticmethod
-    def disable_usage_tracking() -> None:
-        OutboundAPIs.is_usage_tracking_enabled = False
-
-
 class StateTree(Tree):
     current_node = None
     selected_nodes = []
+    current_state = []
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        self.current_state = State(executable=global_executable, no_init=global_no_init)
         self.guide_depth = 3
         self.root.data = ""
 
-    def on_tree_node_highlighted(self, node) -> None:
-        self.current_node = node.node
-
-    def on_tree_node_selected(self) -> None:
-        if self.current_node is None:
-            return
-        if self.current_node.data.startswith("module") or self.current_node.is_root:
-            return
-        self.app.resource.clear()
-        self.app.resource.write(self.current_node.data)
-        self.app.switcher.current = "resource"
-
-    def select_current_node(self) -> None:
-        if self.current_node is None:
-            return
-        if (
-            self.current_node.data.startswith("module")
-            or self.current_node.data.startswith("data")
-            or self.current_node.is_root
-        ):
-            return
-        if self.current_node in self.selected_nodes:
-            self.selected_nodes.remove(self.current_node)
-            self.current_node.label = self.current_node.label.plain
-        else:
-            self.selected_nodes.append(self.current_node)
-            self.current_node.label.stylize("red bold italic reverse")
-
-    @work(exclusive=True)
-    async def refresh_state(self) -> None:
-        global global_successful_termination
-
-        self.app.switcher.current = "loading"
+    def build_tree(self, search_string="") -> None:
+        self.clear()
         self.selected_nodes = []
         self.current_node = None
-        self.clear()
+        module_nodes = {}
 
-        if not global_no_init:
-            self.app.status.update(f"Executing {global_executable.capitalize()} init")
-            returncode, stdout = await execute_async(
-                global_executable, "init -no-color"
+        filtered_blocks = dict(
+            filter(
+                lambda block: search_string in block[1].contents,
+                self.current_state.state_tree.items(),
             )
-            if returncode != 0:
-                self.app.exit(message=stdout)
-                global_successful_termination = False
-                return
-
-        self.app.status.update(f"Executing {global_executable.capitalize()} show")
-
-        returncode, stdout = await execute_async(global_executable, "show -no-color")
-        if returncode != 0 or not stdout.startswith("#"):
-            self.app.exit(message=stdout)
-            global_successful_termination = False
-            return
-
-        self.app.status.update("Building state tree")
-        lines = stdout.splitlines()
-
-        # build module tree
-        modules = set()
-        module_nodes = {}
-        for line in lines:
-            if not line.startswith("# module"):
-                continue
-            parts = line[2:-1].split(".")
-            i = 0
-            module = ""
-            while parts[i] == "module":
-                module += f"{parts[i]}.{parts[i+1]}."
-                modules.add(module[:-1])
-                i += 2
+        )
+        modules = {
+            block.submodule
+            for block in filtered_blocks.values()
+            if block.submodule != ""
+        }
 
         for module_fullname in sorted(modules):
             parts = module_fullname.split(".")
-            sub_module = ""
+            submodule = ""
             i = 0
             while i < len(parts):
-                parent = sub_module
-                short_name = f"{parts[i]}.{parts[i+1]}."
-                sub_module += short_name
-                if sub_module[:-1] not in module_nodes:
-                    if module_nodes.get(parent[:-1]) is None:
+                parent = submodule
+                short_name = f"{parts[i]}.{parts[i+1]}"
+                submodule = (
+                    ".".join([submodule, short_name]) if submodule else short_name
+                )
+                if submodule not in module_nodes:
+                    if module_nodes.get(parent) is None:
                         parent_node = self.root
                     else:
-                        parent_node = module_nodes[parent[:-1]]
-                    node = parent_node.add(short_name[:-1], data=sub_module[:-1])
-                    module_nodes[sub_module[:-1]] = node
+                        parent_node = module_nodes[parent]
+                    node = parent_node.add(short_name, data=submodule)
+                    module_nodes[submodule] = node
                 i += 2
 
-        # parse objects
-        name = ""
-        for line in lines:
-            if line.startswith("#"):
-                parts = line[2:].split(".")
-                i = 0
-                qualifier = ""
-                while parts[i] == "module":
-                    qualifier += f"{parts[i]}.{parts[i+1]}."
-                    i += 2
-                name = ".".join(parts[i:]).replace(":", "")
-                data = ""
-                if qualifier[:-1] in module_nodes:
-                    module_node = module_nodes[qualifier[:-1]]
-                else:
-                    module_node = self.root
-            elif line == "}":
-                data += line + "\n"
-                module_node.add_leaf(name, data=data.strip())
+        # build resource tree
+        for block in filtered_blocks.values():
+            if block.submodule == "":
+                module_node = self.root
             else:
-                data += line + "\n"
+                module_node = module_nodes[block.submodule]
+            leaf = module_node.add_leaf(block.name, data=block)
+            if block.is_tainted:
+                leaf.label.stylize("strike")
 
         self.root.expand_all()
-        self.app.status.update("")
         self.app.switcher.current = "tree"
+
+    @work(exclusive=True)
+    async def refresh_state(self) -> None:
+        global global_successful_termination
+
+        self.app.switcher.current = "loading"
+        self.app.update_status(f"Running {global_executable.capitalize()} show")
+        self.app.search.value = ""
+        try:
+            await self.current_state.refresh_state()
+        except Exception as e:
+            self.app.exit(e)
+            global_successful_termination = False
+            return
+
+        self.build_tree()
         self.app.tree.focus()
+        self.app.update_status("")
         OutboundAPIs.post_usage("refreshed state")
 
+    def on_tree_node_highlighted(self, node) -> None:
+        self.current_node = node.node
+
+    def on_tree_node_selected(self) -> None:
+        if not self.current_node:
+            return
+        if not self.current_node.allow_expand:
+            self.app.resource.clear()
+            self.app.resource.write(self.current_node.data.contents)
+            self.app.switcher.current = "resource"
+
+    def select_current_node(self) -> None:
+        if self.current_node is None:
+            return
+        if (
+            self.current_node.allow_expand
+            or self.current_node.data.type == Block.TYPE_DATASOURCE
+        ):
+            return
+        if self.current_node in self.selected_nodes:
+            self.selected_nodes.remove(self.current_node)
+            self.current_node.label = self.current_node.label.plain
+            if self.current_node.data.is_tainted:
+                self.current_node.label.stylize("strike")
+        else:
+            self.selected_nodes.append(self.current_node)
+            self.current_node.label.stylize("red bold italic reverse")
+
 
 class TerraformTUI(App):
     status = None
     switcher = None
     tree = None
     resource = None
     question = None
     action = None
     search = None
     selected_action = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    TITLE = f"Terraform TUI v{version}"
+    TITLE = f"Terraform TUI v{OutboundAPIs.version}"
     SUB_TITLE = f"The textual UI for Terraform{' (new version available)' if OutboundAPIs.is_new_version_available else ''}"
     CSS_PATH = "ui.css"
 
     BINDINGS = [
-        ("Enter", "", "View state"),
+        ("Enter", "", "View"),
         Binding("escape", "back", "Back"),
         ("s", "select", "Select"),
         ("d", "delete", "Delete"),
         ("t", "taint", "Taint"),
         ("u", "untaint", "Untaint"),
-        ("r", "refresh", "Refresh state"),
+        ("c", "copy", "Copy"),
+        ("r", "refresh", "Refresh"),
         ("/", "search", "Search"),
-        ("1-9", "collapse", "Collapse level"),
-        ("m", "toggle_dark", "Toggle dark mode"),
+        ("1-9", "collapse", "Collapse"),
+        ("m", "toggle_dark", "Dark mode"),
         Binding("y", "yes", "Yes", show=False),
         Binding("n", "no", "No", show=False),
         ("q", "quit", "Quit"),
     ] + [Binding(f"{i}", f"collapse({i})", show=False) for i in range(10)]
 
-    def compose(self) -> ComposeResult:
+    def compose(self):
         yield Header(classes="header")
         yield Input(id="search", placeholder="Search text...")
         with ContentSwitcher(id="switcher", initial="loading"):
             yield LoadingIndicator(id="loading")
             yield StateTree("State", id="tree")
             yield TextLog(
                 id="resource",
@@ -253,83 +205,70 @@
             await self.perform_action()
         elif event.button.id == "no":
             self.action_no()
 
     def on_input_changed(self, event: Input.Changed) -> None:
         if event.input.id == "search":
             search_string = event.value.strip()
-            if search_string == "":
-                self.clear_selected_and_styling()
-                self.tree.root.expand_all()
-            else:
-                self.perform_search(search_string)
+            self.perform_search(search_string)
 
     def on_input_submitted(self, event: Input.Submitted) -> None:
         self.tree.focus()
 
     async def manipulate_resources(self, what_to_do: str) -> None:
-        resources = [
-            f"{node.parent.data}.{node.label.plain}".lstrip(".").replace(
-                " (tainted)", ""
-            )
-            for node in self.tree.selected_nodes
-        ]
-        for resource in resources:
+        for node in self.tree.selected_nodes:
             await execute_async(
                 global_executable,
                 (what_to_do if what_to_do != "delete" else "state rm"),
-                resource,
+                ".".join([node.data.submodule, node.data.name])
+                if node.data.submodule
+                else node.data.name,
             )
 
     async def perform_action(self) -> None:
         if self.switcher.current != "action":
             return
         if self.selected_action in ["taint", "untaint", "delete"]:
-            self.status.update(
+            self.update_status(
                 f"Executing {global_executable.capitalize()} {self.selected_action}"
             )
             self.switcher.current = "loading"
             await self.manipulate_resources(self.selected_action)
+            OutboundAPIs.post_usage(f"applied {self.selected_action}")
         self.tree.refresh_state()
 
+    def update_status(self, message: str) -> None:
+        self.status.update(f"\n{message}")
+
     def perform_search(self, search_string: str) -> None:
-        if search_string == "":
-            self.tree.root.expand_all()
-            return
-        if not self.switcher.current == "tree":
-            return
         self.tree.root.collapse_all()
-        for node in self.tree.root.children:
-            self.find_string_in_node(node, search_string)
+        self.tree.build_tree(search_string)
         self.tree.root.expand()
 
     async def action_yes(self) -> None:
         await self.perform_action()
 
     def action_no(self) -> None:
         self.action_back()
 
     def action_back(self) -> None:
         if (
             not self.switcher.current == "resource"
             and not self.switcher.current == "action"
+            and not self.focused.id == "search"
         ):
             return
         self.switcher.current = "tree"
         self.tree.focus()
 
     def action_select(self) -> None:
         if not self.switcher.current == "tree":
             return
         self.tree.select_current_node()
 
-    def action_destroy(self) -> None:
-        if not self.switcher.current == "tree":
-            return
-
     def action_manipulate_resources(self, what_to_do: str) -> None:
         if not self.switcher.current == "tree":
             return
         if not self.tree.selected_nodes:
             return
         self.selected_action = what_to_do
         self.question.clear()
@@ -341,23 +280,25 @@
             f"Are you sure you wish to {what_to_do} the selected resources?\n\n - "
             + "\n - ".join(resources)
         )
         self.switcher.current = "action"
 
     def action_delete(self) -> None:
         self.action_manipulate_resources("delete")
-        OutboundAPIs.post_usage("removed resources from state")
 
     def action_taint(self) -> None:
         self.action_manipulate_resources("taint")
-        OutboundAPIs.post_usage("applied taint")
 
     def action_untaint(self) -> None:
         self.action_manipulate_resources("untaint")
-        OutboundAPIs.post_usage("applied untaint")
+
+    def action_copy(self) -> None:
+        if self.switcher.current != "resource":
+            return
+        pyperclip.copy(self.app.tree.current_node.data.contents)
 
     def action_refresh(self) -> None:
         if not self.switcher.current == "tree":
             return
         self.tree.refresh_state()
         OutboundAPIs.post_usage("refreshed state")
 
@@ -382,55 +323,17 @@
             return
         self.tree.root.collapse_all()
         for node in self.tree.root.children:
             self.expand_node(level, node)
         self.tree.root.expand()
 
     def action_search(self) -> None:
-        self.clear_selected_and_styling()
+        self.switcher.current = "tree"
         self.search.focus()
 
-    def clear_selected_and_styling(self, node=None) -> None:
-        if node is None:
-            self.tree.selected_nodes = []
-            node = self.tree.root
-        else:
-            node.label = node.label.plain
-        for child in node.children:
-            self.clear_selected_and_styling(child)
-
-    def find_string_in_node(self, node, search_string: str) -> None:
-        search_string = search_string.lower()
-        if node.data.startswith("module"):
-            for child in node.children:
-                self.find_string_in_node(child, search_string)
-        elif (
-            search_string in node.data.lower()
-            or search_string in node.label.plain.lower()
-        ):
-            node.label.stylize("bold blue reverse")
-            while node.parent is not None:
-                node.expand()
-                node = node.parent
-        else:
-            node.label = node.label.plain
-
-
-async def execute_async(*command: str) -> tuple[str, str]:
-    command = [word for phrase in command for word in phrase.split()]
-
-    proc = await asyncio.create_subprocess_exec(
-        *command, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.STDOUT
-    )
-
-    stdout, strerr = await proc.communicate()
-    response = stdout.decode("utf-8")
-
-    return (proc.returncode, response)
-
 
 def parse_command_line() -> None:
     global global_no_init
     global global_executable
 
     parser = argparse.ArgumentParser(
         prog="tftui", description="TFTUI - the Terraform terminal UI", epilog="Enjoy!"
@@ -454,15 +357,15 @@
         "-v", "--version", help="show version information", action="store_true"
     )
 
     args = parser.parse_args()
 
     if args.version:
         print(
-            f"\ntftui v{version}{' (new version available)' if OutboundAPIs.is_new_version_available else ''}\n"
+            f"\ntftui v{OutboundAPIs.version}{' (new version available)' if OutboundAPIs.is_new_version_available else ''}\n"
         )
         exit(0)
     if args.no_init:
         global_no_init = True
     if args.disable_usage_tracking:
         OutboundAPIs.disable_usage_tracking()
     if args.executable:
@@ -486,14 +389,22 @@
     if result is not None:
         print(result)
     if global_successful_termination:
         OutboundAPIs.post_usage("exited successfully")
     else:
         OutboundAPIs.post_usage("exited unsuccessfully")
 
+    if OutboundAPIs.is_new_version_available:
+        print("\n*** New version available. ***")
+
     print(
-        f"\nBye!{' Also, new version available.' if OutboundAPIs.is_new_version_available else ''}\n"
+        """
+For questions and suggestions, please visit https://github.com/idoavrah/terraform-tui/discussions
+For issues and bugs, please visit https://github.com/idoavrah/terraform-tui/issues
+
+Bye!
+"""
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `tftui-0.8/src/tftui/ui.css` & `tftui-0.9/src/tftui/ui.css`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Tree {
   margin: 0 0;
   border: blue;
   height: 75vh;
 }
 
 .status {
-  height: 1;
+  height: 3;
   margin: 0;
   color: red;
   text-align: center;
 }
 
 .resource {
   border: blue;
```

### Comparing `tftui-0.8/src/tftui.egg-info/PKG-INFO` & `tftui-0.9/src/tftui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tftui
-Version: 0.8
+Version: 0.9
 Summary: Terraform Textual User Interface
 Author: Ido Avraham
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -213,27 +213,35 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: textual>=0.32.0
 Requires-Dist: textual-dev
 Requires-Dist: posthog>=3.0.2
 Requires-Dist: requests>=2.31.0
+Requires-Dist: pyperclip>=1.8.2
 
 # TFTUI - The Terraform textual UI
 
 [![PyPI version](https://badge.fury.io/py/tftui.svg?random=stuff)](https://badge.fury.io/py/tftui?)
 ![GitHub](https://img.shields.io/github/license/idoavrah/terraform-tui?random=stuff)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/tftui?random=stuff)
 
 `TFTUI` is a powerful textual GUI that empowers users to effortlessly view and interact with their Terraform state.
 
 With its latest version you can easily visualize the complete state tree, gaining deeper insights into your infrastructure's current configuration. Additionally, the ability to inspect individual resource states allows you to focus on specific details for better analysis and management. Lastly, it's now possible to select resources and perform actions such as tainting and untainting.
 
 ## Key Features
 
+### version 0.9
+
+- [x] Improved search functionality (now showing only matching resources)
+- [x] Improved the tainted resources display
+- [x] Added a copy to clipboard option (press `c` to copy)
+- [x] Major refactoring of the codebase
+
 ### version 0.8
 
 - [x] Added a delete resource option
 
 ### version 0.7
 
 - [x] Added a search option (press `/` to search)
```

