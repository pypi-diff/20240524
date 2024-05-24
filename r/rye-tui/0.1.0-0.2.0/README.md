# Comparing `tmp/rye_tui-0.1.0.tar.gz` & `tmp/rye_tui-0.2.0.tar.gz`

## Comparing `rye_tui-0.1.0.tar` & `rye_tui-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 rye_tui-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 rye_tui-0.1.0/.python-version
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 rye_tui-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 rye_tui-0.1.0/requirements.lock
--rw-r--r--   0        0        0    56573 2020-02-02 00:00:00.000000 rye_tui-0.1.0/images/modals_screen_sketches.excalidraw
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 rye_tui-0.1.0/images/rye_favicon.svg
--rw-r--r--   0        0        0    69488 2020-02-02 00:00:00.000000 rye_tui-0.1.0/images/sketch.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/__init__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/app.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/cli_parser.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/config.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/constants.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/rye_commands.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/tooltips.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/tui.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/assets/modal_screens.css
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/assets/tui.css
--rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/components/config_tab.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/components/general_tab.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/components/helper_widgets.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/components/mainframe.py
--rw-r--r--   0        0        0    10126 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/components/modals.py
--rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/components/projects_tab.py
--rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 rye_tui-0.1.0/src/rye_tui/static/rye_image.jpg
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 rye_tui-0.1.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 rye_tui-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 rye_tui-0.1.0/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 rye_tui-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 rye_tui-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 rye_tui-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 rye_tui-0.2.0/.python-version
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 rye_tui-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 rye_tui-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 rye_tui-0.2.0/requirements.lock
+-rw-r--r--   0        0        0    61490 2020-02-02 00:00:00.000000 rye_tui-0.2.0/images/image_rye_demo_preview.png
+-rw-r--r--   0        0        0    56573 2020-02-02 00:00:00.000000 rye_tui-0.2.0/images/modals_screen_sketches.excalidraw
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 rye_tui-0.2.0/images/rye_favicon.svg
+-rw-r--r--   0        0        0    69488 2020-02-02 00:00:00.000000 rye_tui-0.2.0/images/sketch.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/__init__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/app.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/cli_parser.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/config.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/constants.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/tooltips.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/tui.py
+-rw-r--r--   0        0        0     6864 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/utils.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/assets/modal_screens.css
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/assets/tui.css
+-rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/components/config_tab.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/components/general_tab.py
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/components/helper_widgets.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/components/mainframe.py
+-rw-r--r--   0        0        0    12970 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/components/modals.py
+-rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/components/projects_tab.py
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 rye_tui-0.2.0/src/rye_tui/static/rye_image.jpg
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 rye_tui-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 rye_tui-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 rye_tui-0.2.0/README.md
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 rye_tui-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 rye_tui-0.2.0/PKG-INFO
```

### Comparing `rye_tui-0.1.0/requirements-dev.lock` & `rye_tui-0.2.0/requirements-dev.lock`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # use `rye lock` or `rye sync` to update this lockfile
 #
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: false
 #   with-sources: false
+#   generate-hashes: false
 
 -e file:.
 aiohttp==3.9.5
     # via textual-dev
 aiosignal==1.3.1
     # via aiohttp
 attrs==23.2.0
@@ -33,48 +34,48 @@
     # via yarl
 linkify-it-py==2.0.3
     # via markdown-it-py
 markdown-it-py==3.0.0
     # via mdit-py-plugins
     # via rich
     # via textual
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
 msgpack==1.0.8
     # via textual-dev
 multidict==6.0.5
     # via aiohttp
     # via yarl
 nodeenv==1.8.0
     # via pre-commit
 pillow==10.3.0
     # via rich-pixels
-platformdirs==4.2.1
+platformdirs==4.2.2
+    # via rye-tui
     # via virtualenv
-pre-commit==3.7.0
-pygments==2.17.2
+pre-commit==3.7.1
+pygments==2.18.0
     # via rich
 pyyaml==6.0.1
     # via pre-commit
 rich==13.7.1
     # via rich-pixels
     # via textual
 rich-pixels==3.0.1
     # via rye-tui
-setuptools==69.5.1
+setuptools==70.0.0
     # via nodeenv
-textual==0.58.1
+textual==0.63.0
     # via rye-tui
     # via textual-dev
 textual-dev==1.5.1
-    # via rye-tui
 typing-extensions==4.11.0
     # via textual
     # via textual-dev
 uc-micro-py==1.0.3
     # via linkify-it-py
-virtualenv==20.26.1
+virtualenv==20.26.2
     # via pre-commit
 yarl==1.9.4
     # via aiohttp
```

### Comparing `rye_tui-0.1.0/images/modals_screen_sketches.excalidraw` & `rye_tui-0.2.0/images/modals_screen_sketches.excalidraw`

 * *Files identical despite different names*

### Comparing `rye_tui-0.1.0/images/rye_favicon.svg` & `rye_tui-0.2.0/images/rye_favicon.svg`

 * *Files identical despite different names*

### Comparing `rye_tui-0.1.0/images/sketch.png` & `rye_tui-0.2.0/images/sketch.png`

 * *Files identical despite different names*

### Comparing `rye_tui-0.1.0/src/rye_tui/cli_parser.py` & `rye_tui-0.2.0/src/rye_tui/cli_parser.py`

 * *Files identical despite different names*

### Comparing `rye_tui-0.1.0/src/rye_tui/config.py` & `rye_tui-0.2.0/src/rye_tui/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import tomllib
 import configparser
-from pathlib import Path
+from rich.console import Console
 
 from rye_tui.constants import (
     CONFIG_FILE_NAME,
     CONFIG_FILE_PATH,
     CONFIG_PATH,
     PROJECT_HOME_PATH,
 )
@@ -12,37 +11,29 @@
 
 def create_init_config(conf_path=CONFIG_PATH):
     config = configparser.ConfigParser(default_section=None)
     config.optionxform = str
     config["general"] = {"project_home_path": PROJECT_HOME_PATH}
     config["projects"] = {}
 
+    console = Console(log_path=False)
+
+    console.log('Thank you for using "rye-tui".')
     with open(conf_path / CONFIG_FILE_NAME, "w") as configfile:
         config.write(configfile)
+    console.log(
+        'Since this is your first time using "rye-tui" a Configuration-File was created [green]successfully[/].'
+    )
+    console.log('You can now use "trye" again to start working with rye-tui.')
 
 
 def check_config_exists(path=CONFIG_FILE_PATH):
     return path.exists()
 
 
-def add_cwd_to_config():
-    toml_path = Path().cwd() / "pyproject.toml"
-    if toml_path.exists():
-        with open(toml_path, "rb") as tomlfile:
-            project_infos = tomllib.load(tomlfile)
-
-        project_name = project_infos["project"]["name"]
-        project_path = Path().cwd().as_posix()
-        cfg = RyeTuiConfig()
-        cfg.add_project(new_project_name=project_name, new_project_path=project_path)
-        print(f"Added {project_name} under {project_path} to rye-tui")
-    else:
-        print("error: did not find pyproject.toml")
-
-
 class RyeTuiConfig:
     def __init__(self, path=CONFIG_FILE_PATH) -> None:
         self.configpath = path
         self.config = configparser.ConfigParser(default_section=None)
         self.config.optionxform = str
         self.config.read(path)
```

### Comparing `rye_tui-0.1.0/src/rye_tui/constants.py` & `rye_tui-0.2.0/src/rye_tui/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,39 +25,47 @@
             "type": str,
             "tooltip": tt.TT_DEFAULT_TOOLCHAIN,
             "placeholder": "enter toolchain",
         },
         "build-system": {
             "default": "hatchling",
             "type": str,
-            "tooltip": tt.TT_DEFAULT_BUILD_SYSTEM,
             "placeholder": "enter build-system",
+            "tooltip": tt.TT_DEFAULT_BUILD_SYSTEM,
+        },
+        "license": {
+            "default": "MIT",
+            "type": list,
+            "options": ["MIT"],
+            "tooltip": tt.TT_DEFAULT_LICENCE,
         },
-        "license": {"default": "MIT", "type": str, "tooltip": tt.TT_DEFAULT_LICENCE},
         "author": {
             "default": "",
             "type": str,
-            "tooltip": tt.TT_DEFAULT_AUTHOR,
             "placeholder": "enter mail to override git",
+            "tooltip": tt.TT_DEFAULT_AUTHOR,
         },
         "dependency-operator": {
             "default": ">=",
-            "type": str,
+            "options": [">=", "~=", "=="],
+            "type": list,
             "tooltip": tt.TT_DEFAULT_DEPENDENCY_OPERATOR,
         },
     },
     "proxy": {
         "http": {
             "default": "",
-            "type": bool,
+            "type": str,
+            "placeholder": "enter proxy and press enter",
             "tooltip": tt.TT_PROXY_HTTP,
         },
         "https": {
             "default": "",
-            "type": bool,
+            "type": str,
+            "placeholder": "enter proxy and press enter",
             "tooltip": tt.TT_PROXY_HTTPS,
         },
     },
     "behavior": {
         "force-rye-managed": {
             "default": False,
             "type": bool,
@@ -103,13 +111,55 @@
             "username": "bla",
             "password": "blopb",
             "verify-ssl": True,
         },
     ],
 }
 
-OPT_DROPDOWN_DICT = {
-    "license": ["MIT", "TEST"],
-    "dependency-operator": [">=", "~=", "=="],
+
+SOURCES_DICT = {
+    "url": {
+        "default": "",
+        "type": str,
+        "placeholder": "enter url of package index",
+        "tooltip": "",
+    },
+    "username": {
+        "default": "",
+        "type": str,
+        "placeholder": "enter username",
+        "tooltip": "",
+    },
+    "password": {
+        "default": "",
+        "type": str,
+        "placeholder": "enter password",
+        "tooltip": "",
+    },
+    "verify-ssl": {
+        "default": True,
+        "type": bool,
+        "tooltip": "",
+    },
 }
 
 SOURCES_VALUES = ["url", "username", "password", "verify-ssl"]
+
+INIT_OPTIONS_DICT = {}
+
+ADD_OPTIONS_DICT = {
+    "--dev": bool,
+    "--git": str,
+    "--url": str,
+    "--path": str,
+    "--absolute": bool,
+    "--tag": str,
+    "--rev": str,
+    "--branch": str,
+    "--features": str,
+    "--excluded": bool,
+    "--optional": str,
+    "--pre": bool,
+    "--pin": str,
+    "--sync": bool,
+    "--no-sync": bool,
+}
```

### Comparing `rye_tui-0.1.0/src/rye_tui/tooltips.py` & `rye_tui-0.2.0/src/rye_tui/tooltips.py`

 * *Files identical despite different names*

### Comparing `rye_tui-0.1.0/src/rye_tui/components/config_tab.py` & `rye_tui-0.2.0/src/rye_tui/components/config_tab.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Iterable
 
 from textual import work, on
-from textual.widgets import Input, Static, Switch, Collapsible, Button, Select
+from textual.widgets import Input, Static, Switch, Collapsible, Button
 from textual.widget import Widget
 from textual.containers import Container, Vertical, Horizontal, VerticalScroll
 
-from rye_tui.rye_commands import get_rye_config_values, rye_config_set_command
-from rye_tui.constants import CONF_OPT_DICT, OPT_DROPDOWN_DICT, SOURCES_VALUES
+from rye_tui.utils import get_rye_config_values, rye_config_set_command
+from rye_tui.constants import CONF_OPT_DICT, SOURCES_VALUES, SOURCES_DICT
+from rye_tui.components.helper_widgets import ConfigOptionChanger
 
 
 class ConfigTab(Container):
     def compose(self) -> Iterable[Widget]:
         with Horizontal():
             with Vertical():
                 self.conf_default = ConfigDefault()
@@ -32,73 +33,55 @@
             self.conf_default.load_current(conf_dict=self.rye_config["default"])
             self.conf_behavior.load_current(conf_dict=self.rye_config["behavior"])
             self.conf_proxy.load_current(conf_dict=self.rye_config["proxy"])
 
 
 ########################################################################################
 # Default
-class ConfigDefault(Container):
+class ConfigDefault(VerticalScroll):
     category: str = "default"
+    category_dict: dict = CONF_OPT_DICT[category]
 
     def compose(self) -> Iterable[Widget]:
         self.classes = "section"
         self.border_title = self.category
-        for opt, opt_dict in CONF_OPT_DICT[self.category].items():
-            opt_name = Static(opt)
-            opt_name.tooltip = opt_dict["tooltip"]
-            if opt in OPT_DROPDOWN_DICT.keys():
-                opt_value = Select(
-                    options=[(val, val) for val in OPT_DROPDOWN_DICT[opt]],
-                    id=f"{self.category}_{opt}",
-                    value=opt_dict["default"],
-                    allow_blank=False,
-                )
-            else:
-                opt_value = Input(
-                    value=opt_dict["default"],
-                    placeholder=opt_dict.get("placeholder"),
-                    id=f"{self.category}_{opt}",
-                )
-            opt_value.loading = True
-            with Horizontal(classes=f"config-{self.category}-container"):
-                yield opt_name
-                yield opt_value
+        for opt, opt_dict in self.category_dict.items():
+            yield ConfigOptionChanger(
+                category=self.category, option=opt, opt_dict=opt_dict
+            )
         return super().compose()
 
     def load_current(self, conf_dict):
-        for opt, opt_dict in CONF_OPT_DICT[self.category].items():
-            opt_switch = self.query_one(f"#{self.category}_{opt}")
-            opt_switch.value = conf_dict.get(opt, opt_dict["default"])
-            opt_switch.loading = False
+        for opt, opt_dict in self.category_dict.items():
+            opt_widget = self.query_one(f"#{self.category}_{opt}")
+            opt_widget.value = conf_dict.get(opt, opt_dict["default"])
+            opt_widget.loading = False
 
 
 ########################################################################################
 # Behavior
-class ConfigBehavior(Container):
+class ConfigBehavior(VerticalScroll):
     category: str = "behavior"
+    category_dict: dict = CONF_OPT_DICT[category]
 
     def compose(self) -> Iterable[Widget]:
         self.classes = "section"
         self.border_title = self.category
-        for opt, opt_dict in CONF_OPT_DICT[self.category].items():
-            opt_name = Static(opt)
-            opt_name.tooltip = opt_dict["tooltip"]
-            opt_switch = Switch(value=opt_dict["default"], id=f"{self.category}_{opt}")
-            opt_switch.loading = True
-            with Horizontal(classes=f"config-{self.category}-container"):
-                yield opt_name
-                yield opt_switch
+        for opt, opt_dict in self.category_dict.items():
+            yield ConfigOptionChanger(
+                category=self.category, option=opt, opt_dict=opt_dict
+            )
 
         return super().compose()
 
     def load_current(self, conf_dict):
-        for opt, opt_dict in CONF_OPT_DICT[self.category].items():
-            opt_switch = self.query_one(f"#{self.category}_{opt}")
-            opt_switch.value = conf_dict.get(opt, opt_dict["default"])
-            opt_switch.loading = False
+        for opt, opt_dict in self.category_dict.items():
+            opt_widget = self.query_one(f"#{self.category}_{opt}")
+            opt_widget.value = conf_dict.get(opt, opt_dict["default"])
+            opt_widget.loading = False
 
     @work(thread=True, exclusive=True)
     @on(Switch.Changed)
     def update_value(event, message):
         message.switch.loading = True
         new_value = str(message.value).lower()
         category, option = message.switch.id.split("_")
@@ -111,21 +94,29 @@
         )
 
 
 ########################################################################################
 # Sources
 class ConfigSources(VerticalScroll):
     category: str = "sources"
+    # category_dict: dict = CONF_OPT_DICT[category]
 
     def compose(self) -> Iterable[Widget]:
         self.classes = "section"
         self.border_title = self.category
         for source in CONF_OPT_DICT[self.category]:
             with Collapsible(title=source["name"]):
                 # loop over url/username/pw/verify-ssl
+                for sources_val, sources_val_dict in SOURCES_DICT.items():
+                    yield ConfigOptionChanger(
+                        category=self.category,
+                        option=sources_val,
+                        opt_dict=sources_val_dict,
+                    )
+
                 for sources_val in SOURCES_VALUES:
                     if not source.get(sources_val):
                         continue
                     opt_name = Static(sources_val)
                     # opt_name.tooltip = opt_dict["tooltip"]
                     if sources_val == "verify-ssl":
                         opt_value = Switch(
@@ -144,46 +135,40 @@
 
         yield Button("Add new Source")
         return super().compose()
 
 
 ########################################################################################
 # Proxy
-class ConfigProxy(Container):
+class ConfigProxy(VerticalScroll):
     category: str = "proxy"
+    category_dict: dict = CONF_OPT_DICT[category]
 
     def compose(self) -> Iterable[Widget]:
         self.classes = "section"
         self.border_title = self.category
-        for opt, opt_dict in CONF_OPT_DICT[self.category].items():
-            opt_name = Static(opt)
-            opt_name.tooltip = opt_dict["tooltip"]
-            opt_value = Input(
-                value=opt_dict["default"],
-                placeholder="enter proxy and press enter",
-                id=f"{self.category}_{opt}",
+        for opt, opt_dict in self.category_dict.items():
+            yield ConfigOptionChanger(
+                category=self.category, option=opt, opt_dict=opt_dict
             )
-            opt_value.loading = True
-            with Horizontal(classes=f"config-{self.category}-container"):
-                yield opt_name
-                yield opt_value
         return super().compose()
 
     def load_current(self, conf_dict):
-        for opt, opt_dict in CONF_OPT_DICT[self.category].items():
-            opt_switch = self.query_one(f"#{self.category}_{opt}")
-            opt_switch.value = conf_dict.get(opt, opt_dict["default"])
-            opt_switch.loading = False
+        for opt, opt_dict in self.category_dict.items():
+            opt_widget = self.query_one(f"#{self.category}_{opt}")
+            opt_widget.value = conf_dict.get(opt, opt_dict["default"])
+            opt_widget.loading = False
 
     @work(thread=True, exclusive=True)
     @on(Input.Submitted)
     def update_value(self, event):
         event.input.loading = True
         new_value = str(event.value).lower()
         category, option = event.input.id.split("_")
         rye_config_set_command(category=category, option=option, value=new_value)
         event.input.loading = False
+
         msg_show = f"set to [green]{new_value}[/]" if new_value else "[red]removed[/]"
         self.notify(
             message=f"{category}.{option} {msg_show}",
             title="Config Updated",
         )
```

### Comparing `rye_tui-0.1.0/src/rye_tui/components/mainframe.py` & `rye_tui-0.2.0/src/rye_tui/components/mainframe.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,17 +8,35 @@
 from rye_tui.components.projects_tab import ProjectTab
 from rye_tui.components.general_tab import GeneralTab
 from rye_tui.components.config_tab import ConfigTab
 
 
 class MainFrame(Horizontal):
     BINDINGS = [
-        Binding("ctrl+j", "show_tab('Projects')", "Projects", priority=True),
-        Binding("ctrl+k", "show_tab('General')", "General", priority=True),
-        Binding("ctrl+l", "show_tab('Config')", "Config", priority=True),
+        Binding(
+            key="ctrl+j",
+            action="show_tab('Projects')",
+            description="Projects",
+            key_display="^j",
+            priority=True,
+        ),
+        Binding(
+            key="ctrl+k",
+            action="show_tab('General')",
+            description="General",
+            key_display="^k",
+            priority=True,
+        ),
+        Binding(
+            key="ctrl+l",
+            action="show_tab('Config')",
+            description="Config",
+            key_display="^l",
+            priority=True,
+        ),
     ]
 
     def compose(self) -> Iterable[Widget]:
         with TabbedContent(initial="Projects"):
             with TabPane("Projects", id="Projects", classes="tabs"):
                 yield ProjectTab()
             with TabPane("General", id="General", classes="tabs"):
```

### Comparing `rye_tui-0.1.0/src/rye_tui/components/modals.py` & `rye_tui-0.2.0/src/rye_tui/components/modals.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from typing import Iterable
 from pathlib import Path
 
 from textual import on, work
+from textual.reactive import reactive
 from textual.widget import Widget
 from textual.validation import Regex
 from textual.screen import ModalScreen
 from textual.widgets import (
     Input,
     Button,
     Collapsible,
     Static,
     Label,
     ListView,
-    RichLog,
     DataTable,
 )
 from textual.containers import Vertical, Horizontal
+from textual.worker import get_current_worker
 
-from rye_tui.rye_commands import rye_command_str_output
+from rye_tui.utils import rye_command_str_output, fill_package_add_table
 from rye_tui.components.helper_widgets import ProjectListItem
 
 
 class ModalRyeInit(ModalScreen):
     CSS_PATH: Path = Path("../assets/modal_screens.css")
     rye_command: str = ""
     project_name: str = ""
@@ -32,16 +33,15 @@
         with Vertical():
             yield Label("Create a new project")
             yield Input(placeholder="enter project name", id="input_new_project")
             with Horizontal():
                 yield Button(":house:", id="btn_home", variant="warning")
                 yield Input(placeholder="project path [default: .]", id="input_path")
             with Collapsible(title="other Options"):
-                yield Label("Test")
-                yield Label("Test2")
+                yield Label("coming soon ...")
             yield Static(self.rye_command, id="preview_rye_command")
             with Horizontal(classes="horizontal-conf-cancel"):
                 yield Button("continue", variant="success", classes="btn-continue")
                 yield Button("cancel", variant="error", classes="btn-cancel")
         return super().compose()
 
     @on(Input.Changed)
@@ -84,43 +84,43 @@
 
     @on(Button.Pressed, ".btn-continue")
     async def create_project(self):
         self.loading = True
         project_path = (Path(self.project_path) / self.project_name).as_posix()
         command = f"rye init {project_path}"
         output_str = await self.async_create_project(command=command)
-        self.notify(title="New Project created", message=output_str)
-
+        self.notify(title="New Project created", message=output_str, timeout=1)
         self.loading = False
+
         self.app.cfg.add_project(
             new_project_name=self.project_name, new_project_path=project_path
         )
         self.notify(
             f"[blue]{self.project_name}[/] was added to [b]rye-tui[/b] config",
             title="Project List Updated",
+            timeout=1,
         )
         self.app.pop_screen()
+
         project_list = self.app.query_one(ListView)
         project_list.append(item=ProjectListItem(project_title=self.project_name))
-        num_project = project_list.children.__len__()
-        project_list.index = num_project
-        self.app.log.error(num_project)
+        project_list.index = len(project_list.children)
         project_list.action_select_cursor()
 
     async def async_create_project(self, command):
         output_str = rye_command_str_output(command=command)
         return output_str
 
 
 class ModalRyePin(ModalScreen):
     CSS_PATH: Path = Path("../assets/modal_screens.css")
 
     def compose(self) -> Iterable[Widget]:
         with Vertical():
-            yield Label(f"Pin Python Version of [blue]{self.app.active_project}[/]")
+            yield Label(f"Pin Python Version of [blue]{self.app.project['name']}[/]")
             self.pin_input = Input(
                 placeholder="enter python version to pin",
                 validators=[Regex("^3\.(?:[89]|1[012])$")],
                 id="input_pin_python",
             )
             yield self.pin_input
             with Horizontal(classes="horizontal-conf-cancel"):
@@ -131,15 +131,15 @@
         return super().compose()
 
     @on(Button.Pressed, ".btn-continue")
     def pin_new_version(self):
         new_python_version = self.query_one("#input_pin_python").value
 
         rye_command_str_output(
-            command=f"rye pin {new_python_version}", cwd=self.app.active_project_path
+            command=f"rye pin {new_python_version}", cwd=self.app.project["path"]
         )
 
         self.app.pop_screen()
         self.app.query_one(ListView).action_select_cursor()
 
     @on(Button.Pressed, ".btn-cancel")
     def close_modal(self):
@@ -152,106 +152,182 @@
     @on(Input.Submitted, "#input_pin_python")
     def confirm_input(self):
         self.query_one(".btn-continue").press()
 
 
 class ModalRyeAdd(ModalScreen):
     CSS_PATH: Path = Path("../assets/modal_screens.css")
+    option_flags = reactive([])
 
     def compose(self) -> Iterable[Widget]:
         with Vertical():
             yield Label(
-                f"Add packages to your project [blue]{self.app.active_project}[/]"
+                f"Add packages to your project [blue]{self.app.project['name']}[/]",
             )
             self.pin_input = Input(
                 placeholder="enter python package to add",
                 # validators=[Regex("^3\.(?:[89]|1[012])$")],
                 id="input_add_package",
             )
-            yield self.pin_input
-            yield RichLog(markup=True, highlight=True)
+            self.pin_input.tooltip = "press enter or space to submit"
+            with Horizontal():
+                yield self.pin_input
+                yield Button("--dev", id="option_button_dev", variant="warning")
+
+            # All Dev Options
+            with Collapsible(title="Options"):
+                yield Label("coming soon")
+            #     yield VerticalScroll(*[
+            #         Horizontal(Label(flag), Input(f'{flag_type}'))
+            #         for flag, flag_type in ADD_OPTIONS_DICT.items()
+            #         ])
+
             self.package_table = DataTable(cursor_type="cell", header_height=2)
             self.package_table.add_column("package", key="package", width=16)
-            self.package_table.add_column("version", key="version", width=12)
+            self.package_table.add_column("version", key="version", width=10)
             self.package_table.add_column("added", key="added", width=6)
             self.package_table.add_column("synced", key="synced", width=6)
-            self.package_table.add_column("remove", key="remove", width=14)
+            self.package_table.add_column("--dev", key="--dev", width=6)
+            self.package_table.add_column("remove", key="remove", width=8)
+
+            # Add present packages
+            fill_package_add_table(
+                package_table=self.package_table, project_dict=self.app.project
+            )
 
-            for pkg_str in self.app.active_project_toml['project']['dependencies']:
-                pkg = pkg_str.split('=')[0][:-1]
-                version = pkg_str.lstrip(pkg)
-                
-
-                self.package_table.add_row(
-                    f"[blue]{pkg}[/]",
-                    version,
-                    ":white_check_mark:",
-                    ":white_check_mark:" if pkg in self.app.active_project_lock else ":cross_mark:",
-                    "remove package",
-                    key=pkg,
-                )
             yield self.package_table
 
             with Horizontal(classes="horizontal-conf-cancel"):
-                yield Button("continue & sync", variant="success", classes="btn-continue")
-                yield Button("cancel", variant="error", classes="btn-cancel")
+                yield Button(
+                    "continue & sync", variant="success", classes="btn-continue"
+                )
+                yield Button(
+                    "continue & dont sync", variant="error", classes="btn-cancel"
+                )
         return super().compose()
 
     @on(Input.Changed, "#input_add_package")
+    @on(Input.Submitted, "#input_add_package")
     def new_package_to_list(self, message):
         current_package = message.value.strip()
-        if message.value.endswith(" "):
+        if message.value.endswith(" ") or isinstance(message, Input.Submitted):
             message.input.value = ""
-            self.query_one(RichLog).write(f"[blue]{current_package}[/]")
+
             self.package_table.add_row(
-                f"[blue]{current_package}[/]",
+                f"[white]{current_package}[/]",
                 "00.00.00",
-                # ":white_check_mark:",
                 ":cross_mark:",
                 ":cross_mark:",
-                "remove package",
+                ":cross_mark:",
+                "remove",
                 key=current_package,
             )
             self.rye_add_package(current_package)
 
+    @on(Button.Pressed, "#option_button_dev")
+    def use_dev_flag(self, message: Button.Pressed):
+        if "--dev" in self.option_flags:
+            self.option_flags.remove("--dev")
+            message.button.variant = "warning"
+
+        else:
+            self.option_flags.append("--dev")
+            message.button.variant = "success"
+
     @work(thread=True)
     def rye_add_package(self, package):
+        flags = " ".join(self.option_flags)
+        worker = get_current_worker()
         rye_add_str = rye_command_str_output(
-            command=f"rye add {package}", cwd=self.app.active_project_path
+            command=f"rye add {package} {flags}", cwd=self.app.project["path"]
         )
-        if rye_add_str.startswith("Added"):
+        if rye_add_str.startswith("Initializing"):
+            rye_add_str = rye_add_str.split("\n")[-1]
+
+        if rye_add_str.startswith(("Added")):
             self.notify(
                 message=rye_add_str.replace(package, f"[green]{package}[/]"),
                 title="Package Added",
             )
             package_version = rye_add_str.split()[1].lstrip(package)
-            self.package_table.update_cell(
-                row_key=package, column_key="version", value=package_version
-            )
-            self.package_table.update_cell(
-                row_key=package, column_key="added", value=":white_check_mark:"
-            )
+
+            if not worker.is_cancelled:
+                self.app.call_from_thread(
+                    self.package_table.update_cell,
+                    row_key=package,
+                    column_key="version",
+                    value=package_version,
+                )
+                self.app.call_from_thread(
+                    self.package_table.update_cell,
+                    row_key=package,
+                    column_key="added",
+                    value=":white_check_mark:",
+                )
+                if "--dev" in self.option_flags:
+                    self.app.call_from_thread(
+                        self.package_table.update_cell,
+                        row_key=package,
+                        column_key="--dev",
+                        value=":white_check_mark:",
+                    )
 
     @on(DataTable.CellSelected)
-    def remove_package(self, event):
+    def remove_package(self, event: DataTable.CellSelected):
         row_key = event.cell_key.row_key.value
         col_key = event.cell_key.column_key.value
 
+        is_dev = self.package_table.get_cell(row_key=row_key, column_key="--dev")
+        dev_flag = "--dev" if is_dev == ":white_check_mark:" else ""
+
         if col_key == "remove":
             self.package_table.remove_row(row_key)
             rye_rm_str = rye_command_str_output(
-                command=f"rye remove {row_key}", cwd=self.app.active_project_path
+                command=f"rye remove {row_key} {dev_flag}", cwd=self.app.project["path"]
             )
             self.notify(
                 title="Package Removed",
                 message=rye_rm_str.replace(row_key, f"[red]{row_key}[/]"),
             )
 
     @on(Button.Pressed, ".btn-continue")
     def pin_new_version(self):
         self.app.pop_screen()
-        self.app.query_one('#btn_sync').press()
+        self.app.query_one("#btn_sync").press()
 
     @on(Button.Pressed, ".btn-cancel")
     def close_modal(self):
         self.app.pop_screen()
         self.app.query_one(ListView).action_select_cursor()
+
+
+class ModalConfirm(ModalScreen):
+    CSS_PATH: Path = Path("../assets/modal_screens.css")
+
+    def compose(self) -> Iterable[Widget]:
+        with Vertical():
+            yield Label(f"Do you want to delete [blue]{self.app.project['name']}[/]")
+            yield Label("This will [red]delete[/] all project files!")
+            with Horizontal(classes="horizontal-conf-cancel"):
+                yield Button(
+                    "delete all files", variant="success", classes="btn-continue"
+                )
+                yield Button(
+                    "remove from config", variant="error", classes="btn-cancel"
+                )
+        return super().compose()
+
+    @on(Button.Pressed, ".btn-continue")
+    def delete_all_files(self):
+        self.dismiss(True)
+        self.notify(
+            f"project [blue]{self.app.project['name']}[/] and all files were deleted",
+            title="Project List Updated",
+        )
+
+    @on(Button.Pressed, ".btn-cancel")
+    def delete_only_config_entry(self):
+        self.dismiss(False)
+        self.notify(
+            f"project [blue]{self.app.project['name']}[/] was removed from config",
+            title="Project List Updated",
+        )
```

### Comparing `rye_tui-0.1.0/src/rye_tui/components/projects_tab.py` & `rye_tui-0.2.0/src/rye_tui/components/projects_tab.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,36 @@
 from typing import Iterable
 from pathlib import Path
-import tomllib
 
-from rich.table import Table
 from textual import on, work
 from textual.events import Resize
 from textual.containers import VerticalScroll, Container, Horizontal, Vertical
 from textual.widget import Widget
 from textual.widgets import Button, ListView, RichLog
 from rich_pixels import Pixels
 
-from rye_tui.components.helper_widgets import ProjectListItem
-from rye_tui.components.modals import ModalRyeInit, ModalRyePin, ModalRyeAdd
-from rye_tui.rye_commands import rye_command_str_output
+from rye_tui.components.helper_widgets import (
+    ProjectListItem,
+    CustomLoading,
+    SyncButton,
+    BuildButton,
+)
+from rye_tui.components.modals import (
+    ModalRyeInit,
+    ModalRyePin,
+    ModalRyeAdd,
+    ModalConfirm,
+)
+from rye_tui.utils import (
+    rye_command_str_output,
+    delete_folder,
+    display_toml_project_infos,
+    display_general_project_infos,
+    display_package_project_infos,
+)
 from rye_tui.constants import IMAGE_PATH
 
 
 class ProjectTab(Container):
     def compose(self) -> Iterable[Widget]:
         with Horizontal():
             with Vertical():
@@ -24,156 +38,203 @@
                 yield ProjectInteraction()
             with Vertical():
                 yield ProjectPreview()
 
         return super().compose()
 
 
+########################################################################################
+# Project List
 class ProjectList(VerticalScroll):
     def compose(self) -> Iterable[Widget]:
         self.classes = "section"
         self.border_title = "Project List"
         self.id = "project_list"
 
         yield ListView(
             *[
                 ProjectListItem(project_title=proj)
                 for proj in self.app.cfg.project_names
             ],
-            initial_index=None,
         )
 
         return super().compose()
 
-    async def update(self):
-        self.remove()
-        self.app.mount(ProjectList(), before="#project_interaction")
+    def on_mount(self):
+        self.query_one(ListView).index = None
 
+    @work(thread=True, exclusive=True)
     @on(ListView.Selected)
     def get_project_infos(self, event: ListView.Selected):
-        self.app.active_project = event.item.project_title
-        self.app.active_project_path = self.app.cfg.config["projects"].get(
-            self.app.active_project
-        )
-        with open(Path(self.app.active_project_path) / 'pyproject.toml', 'rb') as tomlfile:
-            self.app.active_project_toml = tomllib.load(tomlfile)
+        self.app.get_project_infos(project_name=event.item.project_title)
+
+        preview_window = self.app.query_one("#project_preview")
+        preview_window.update_content()
+
+        btns = self.app.query("ProjectListItem Button")
+        for btn in btns:
+            btn.add_class("invisible")
+
+        event.item.query(Button).remove_class("invisible")
+
+    @on(Button.Pressed, ".delete-button")
+    def delete_project(self, message):
+        def check_delete(delete_files: bool) -> None:
+            if delete_files:
+                delete_folder(folder_path=self.app.project["path"])
 
-        with open(Path(self.app.active_project_path) / 'requirements.lock', 'r') as lockfile:
-            self.app.active_project_lock = [line.split('==')[0]
-                                            for line in lockfile.readlines()
-                                            if not line.startswith('#')]
+            project_list = self.app.query_one(ListView)
 
-        self.app.query_one("#project_preview").update_content()
+            for i, project in enumerate(project_list.children):
+                if project.id == self.app.project["name"]:
+                    project_list.pop(i)
 
+            self.app.cfg.remove_project(self.app.project["name"])
+            self.app.reset_project()
 
+        self.app.push_screen(ModalConfirm(), check_delete)
+
+
+########################################################################################
+# Project Interaction
 class ProjectInteraction(Container):
     def compose(self) -> Iterable[Widget]:
         self.classes = "section"
         self.border_title = "Interaction"
         self.id = "project_interaction"
 
         with Vertical():
             with Horizontal():
                 yield Button("New Project", id="btn_new")
                 yield Button("Add/Remove Packages", id="btn_pkg")
-                yield Button("Rye Sync + Update", id="btn_sync")
+                yield SyncButton()
             with Horizontal():
                 yield Button("Pin Python Version", id="btn_pin")
-                yield Button("Build", id="btn_build")
+                yield BuildButton()
+                # yield Button("Build", id="btn_build")
                 yield Button("Publish", id="btn_publish")
 
         return super().compose()
 
     @on(Button.Pressed, "#btn_publish")
-    async def rye_load_package_list(self) -> None:
+    async def rye_publish(self) -> None:
         # Open new Modal
         self.app.cfg.add_project(
             new_project_name="test2", new_project_path=Path().cwd().as_posix()
         )
 
-        # Testing
+        # for testing
         project_list = self.app.query_one(ListView)
         project_list.append(item=ProjectListItem(project_title="test2"))
         num_project = project_list.children.__len__()
         project_list.index = num_project
         project_list.action_select_cursor()
 
+    # Rye build
+    @work(thread=True)
+    @on(Button.Pressed, "#btn_build")
+    async def rye_build(self, message: Button.Pressed) -> None:
+        self.app.query_one("#project_preview").focus()
+        message.button.loading = True
+        await self.async_build_function()
+        message.button.loading = False
+
+    async def async_build_function(self):
+        output = rye_command_str_output(
+            command="rye build", cwd=self.app.project["path"]
+        )
+        self.app.query_one(ListView).action_select_cursor()
+        return output
+
     @on(Button.Pressed, "#btn_new")
     def rye_init_new_project(self) -> None:
         self.app.push_screen(ModalRyeInit())
 
     @on(Button.Pressed, "#btn_pkg")
     def rye_add_packages(self) -> None:
         self.app.push_screen(ModalRyeAdd())
 
     @on(Button.Pressed, "#btn_pin")
     def rye_pin_python_version(self) -> None:
         self.app.push_screen(ModalRyePin())
 
+    # Rye Sync
     @work(thread=True)
     @on(Button.Pressed, "#btn_sync")
-    async def rye_sync_project(self) -> None:
-        self.app.query_one("#project_preview").loading = True
+    async def rye_sync_project(self, message: Button.Pressed) -> None:
+        self.app.query_one("#project_preview").focus()
+        message.button.loading = True
         await self.async_sync_function()
-        self.app.query_one("#project_preview").loading = False
+        message.button.loading = False
 
     async def async_sync_function(self):
         output = rye_command_str_output(
-            command="rye sync -f", cwd=self.app.active_project_path
+            command="rye sync -f", cwd=self.app.project["path"]
         )
         self.app.query_one(ListView).action_select_cursor()
         return output
 
 
+########################################################################################
+# Project Preview
 class ProjectPreview(VerticalScroll):
     def compose(self) -> Iterable[Widget]:
         self.classes = "section"
         self.border_title = "Preview"
+        self.border_subtitle = "no project selected"
         self.id = "project_preview"
-        self.content_info = RichLog(wrap=False, auto_scroll=True)
+        self.content_info = RichLog(wrap=False, auto_scroll=True, markup=True)
 
         yield self.content_info
 
         return super().compose()
 
-    @work(thread=True, exclusive=True)
+    def get_loading_widget(self) -> Widget:
+        return CustomLoading(text="Loading Project Infos...")
+
+    # @work(thread=True, exclusive=True)
     def update_content(self):
+        self.loading = True
         try:
-            if self.app.active_project_path:
-                project_infos = rye_command_str_output(
-                    "rye show", cwd=self.app.active_project_path
+            if self.app.project["path"]:
+                self.content_info.clear()
+
+                general_table = display_general_project_infos(
+                    path=self.app.project["path"]
                 )
-                project_packages = rye_command_str_output(
-                    "rye list", cwd=self.app.active_project_path
+
+                toml_table = display_toml_project_infos(
+                    toml=self.app.project["toml"], header=True
                 )
-                self.content_info.clear()
-                self.content_info.write(project_infos)
-                self.content_info.write(self.app.active_project_toml)
 
-                table = Table("package", "version", expand=True)
-                for pkg in project_packages.split("\n"):
-                    if "==" in pkg:
-                        pkg_name, pkg_version = pkg.split("==")
-                        table.add_row(pkg_name, pkg_version)
+                package_table = display_package_project_infos(
+                    path=self.app.project["path"]
+                )
+
+                self.content_info.write(general_table, expand=True)
+                self.content_info.write(toml_table, expand=True)
+                self.content_info.write(package_table, expand=True)
 
-                self.content_info.write(table)
+                self.border_subtitle = self.app.project["name"]
 
             else:
                 content = "please select a project"
                 self.content_info.clear()
                 self.content_info.write(content)
             # self.content = content
         except Exception as e:
             self.app.log.error(e)
             self.content_info.clear()
             self.content_info.write("error: project path name is not valid")
 
+        self.loading = False
+
     @on(Resize)
     def keep_image_size(self, event: Resize):
-        if not self.app.active_project:
+        if not self.app.project["name"]:
             new_width, new_height = event.size
             pixels = Pixels.from_image_path(
                 IMAGE_PATH,
                 resize=(new_width, int(1.8 * new_height)),
             )
             self.content_info.clear()
             self.content_info.write(pixels)
```

### Comparing `rye_tui-0.1.0/src/rye_tui/static/rye_image.jpg` & `rye_tui-0.2.0/src/rye_tui/static/rye_image.jpg`

 * *Files identical despite different names*

### Comparing `rye_tui-0.1.0/LICENSE.txt` & `rye_tui-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

