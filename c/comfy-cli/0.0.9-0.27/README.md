# Comparing `tmp/comfy_cli-0.0.9.tar.gz` & `tmp/comfy_cli-0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comfy_cli-0.0.9.tar", last modified: Thu May  2 01:09:02 2024, max compression
+gzip compressed data, was "comfy_cli-0.27.tar", last modified: Mon May 20 23:36:17 2024, max compression
```

## Comparing `comfy_cli-0.0.9.tar` & `comfy_cli-0.27.tar`

### file list

```diff
@@ -1,35 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:09:02.441331 comfy_cli-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    47626 2024-05-02 01:09:02.441331 comfy_cli-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:09:02.437331 comfy_cli-0.0.9/comfy_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11977 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/cmdline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:09:02.441331 comfy_cli-0.0.9/comfy_cli/command/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:09:02.441331 comfy_cli-0.0.9/comfy_cli/command/custom_nodes/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/command/custom_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/command/custom_nodes/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/command/install.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:09:02.441331 comfy_cli-0.0.9/comfy_cli/command/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/command/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/command/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/env_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/meta_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-02 01:08:54.000000 comfy_cli-0.0.9/comfy_cli/workspace_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:09:02.441331 comfy_cli-0.0.9/comfy_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    47626 2024-05-02 01:09:02.000000 comfy_cli-0.0.9/comfy_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-02 01:09:02.000000 comfy_cli-0.0.9/comfy_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:09:02.000000 comfy_cli-0.0.9/comfy_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-02 01:09:02.000000 comfy_cli-0.0.9/comfy_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 01:09:02.000000 comfy_cli-0.0.9/comfy_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 01:09:02.000000 comfy_cli-0.0.9/comfy_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-02 01:08:59.000000 comfy_cli-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 01:09:02.441331 comfy_cli-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:36:17.802546 comfy_cli-0.27/
+-rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-20 23:36:13.000000 comfy_cli-0.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    49836 2024-05-20 23:36:17.802546 comfy_cli-0.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-20 23:36:13.000000 comfy_cli-0.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:36:17.798546 comfy_cli-0.27/comfy_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20809 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/cmdline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:36:17.802546 comfy_cli-0.27/comfy_cli/command/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:36:17.802546 comfy_cli-0.27/comfy_cli/command/custom_nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/command/custom_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23098 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/command/custom_nodes/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/command/install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:36:17.802546 comfy_cli-0.27/comfy_cli/command/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    11738 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/command/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/command/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/env_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:36:17.802546 comfy_cli-0.27/comfy_cli/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/registry/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/registry/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/registry/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12095 2024-05-20 23:36:13.000000 comfy_cli-0.27/comfy_cli/workspace_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:36:17.802546 comfy_cli-0.27/comfy_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49836 2024-05-20 23:36:17.000000 comfy_cli-0.27/comfy_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-20 23:36:17.000000 comfy_cli-0.27/comfy_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 23:36:17.000000 comfy_cli-0.27/comfy_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 23:36:17.000000 comfy_cli-0.27/comfy_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-20 23:36:17.000000 comfy_cli-0.27/comfy_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 23:36:17.000000 comfy_cli-0.27/comfy_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-20 23:36:15.000000 comfy_cli-0.27/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 23:36:17.802546 comfy_cli-0.27/setup.cfg
```

### Comparing `comfy_cli-0.0.9/LICENSE` & `comfy_cli-0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `comfy_cli-0.0.9/PKG-INFO` & `comfy_cli-0.27/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comfy-cli
-Version: 0.0.9
+Version: 0.27
 Summary: A CLI tool for installing and using ComfyUI.
 Maintainer-email: Yoland Yan <yoland@drip.art>, James Kwon <hongilkwon316@gmail.com>, Robin Huang <robin@drip.art>, "Dr.Lt.Data" <dr.lt.data@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -679,171 +679,195 @@
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Repository, https://github.com/drip-art/comfy-cli.git
 Keywords: comfyui,stable diffusion
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: typer>=0.3.0
+Requires-Dist: typer>=0.9.0
 Requires-Dist: GitPython
 Requires-Dist: rich
 Requires-Dist: requests
 Requires-Dist: pyyaml
-Requires-Dist: typing-extensions
+Requires-Dist: typing-extensions>=4.7.0
 Requires-Dist: mixpanel
 Requires-Dist: questionary
 Requires-Dist: psutil
+Requires-Dist: tomlkit
+Requires-Dist: pathspec
+Requires-Dist: httpx
+Requires-Dist: packaging
 
-# comfy-cli
+# Comfy-Cli: A Command Line Tool for ComfyUI
+[![Test ComfyUI Example Workflows](https://github.com/Comfy-Org/ComfyUI-Mirror/actions/workflows/test-workflows.yaml/badge.svg)](https://github.com/Comfy-Org/ComfyUI-Mirror/actions/workflows/test-workflows.yaml)
+[![Test ComfyUI Windows with Default Workflow](https://github.com/Comfy-Org/ComfyUI-Mirror/actions/workflows/test-workflows-windows.yaml/badge.svg)](https://github.com/Comfy-Org/ComfyUI-Mirror/actions/workflows/test-workflows-windows.yaml)
 
-comfy-cli is a command line tool that helps users easily install and manage [ComfyUI](https://github.com/comfyanonymous/ComfyUI), a powerful open-source machine learning framework. With comfy-cli, you can quickly set up ComfyUI, install packages, and manage custom nodes, all from the convenience of your terminal.
+comfy-cli is a command line tool that helps users easily install and manage
+[ComfyUI](https://github.com/comfyanonymous/ComfyUI), a powerful open-source
+machine learning framework. With comfy-cli, you can quickly set up ComfyUI,
+install packages, and manage custom nodes, all from the convenience of your
+terminal.
+
+
+
+## Demo
+
+<img src="https://github.com/yoland68/comfy-cli/raw/main/assets/comfy-demo.gif" width="400" alt="Comfy Command Demo">
 
 ## Features
 
 - 🚀 Easy installation of ComfyUI with a single command
 - 📦 Seamless package management for ComfyUI extensions and dependencies
 - 🔧 Custom node management for extending ComfyUI's functionality
+- 🗄️ Download checkpoints and save model hash
 - 💻 Cross-platform compatibility (Windows, macOS, Linux)
 - 📖 Comprehensive documentation and examples
 
 ## Installation
 
-To install comfy-cli, make sure you have Python 3.7 or higher installed on your system. Then, run the following command:
+1. (Recommended, but not necessary) Enable virtual environment ([venv](https://docs.python.org/3/library/venv.html)/[conda](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html))
+
+2. To install comfy-cli, make sure you have Python 3.9 or higher installed on your system. Then, run the following command:
+
+   `pip install comfy-cli`
 
-`pip install comfy-cli`
+### Shell Autocomplete
 
+To install autocompletion hints in your shell run:
+
+`comfy --install-completion`
+
+This enables you to type `comfy [TAP]` to autocomplete commands and options
 
 ## Usage
 
 ### Installing ComfyUI
 
 To install ComfyUI using comfy, simply run:
 
 `comfy install`
 
 This command will download and set up the latest version of ComfyUI and ComfyUI-Manager on your
 system. If you run in a ComfyUI repo that has already been setup. The command
 will simply update the comfy.yaml file to reflect the local setup
 
-  * `comfy install --skip-manager`: Install ComfyUI without ComfyUI-Manager.
-  * `comfy --workspace=<path> install`: Install ComfyUI into `<path>/ComfyUI`.
-  * For `comfy install`, if no path specification like `--workspace, --recent, or --here` is provided, it will be implicitly installed in `<HOME>/comfy`.
-
+- `comfy install --skip-manager`: Install ComfyUI without ComfyUI-Manager.
+- `comfy --workspace=<path> install`: Install ComfyUI into `<path>/ComfyUI`.
+- For `comfy install`, if no path specification like `--workspace, --recent, or --here` is provided, it will be implicitly installed in `<HOME>/comfy`.
 
 ### Specifying execution path
 
-* You can specify the path of ComfyUI where the command will be applied through path indicators as follows:
-  * `comfy --workspace=<path>`: Run from the ComfyUI installed in the specified workspace.
-  * `comfy --recent`: Run from the recently executed or installed ComfyUI.
-  * `comfy --here`: Run from the ComfyUI located in the current directory.
-* --workspace, --recent, and --here options cannot be used simultaneously.
-* If there is no path indicator, the following priority applies:
-  * Run from the default ComfyUI at the path specified by `comfy set-default <path>`.
-  * Run from the recently executed or installed ComfyUI.
-  * Run from the ComfyUI located in the current directory.
-
-* Example 1: To run the recently executed ComfyUI:
-  * `comfy --recent launch`
-* Example 2: To install a package on the ComfyUI in the current directory:
-  * `comfy --here node install ComfyUI-Impact-Pack`
-* Example 3: To update the automatically selected path of ComfyUI and custom nodes based on priority:
-  * `comfy node update all`
+- You can specify the path of ComfyUI where the command will be applied through path indicators as follows:
+  - `comfy --workspace=<path>`: Run from the ComfyUI installed in the specified workspace.
+  - `comfy --recent`: Run from the recently executed or installed ComfyUI.
+  - `comfy --here`: Run from the ComfyUI located in the current directory.
+- --workspace, --recent, and --here options cannot be used simultaneously.
+- If there is no path indicator, the following priority applies:
+
+  - Run from the default ComfyUI at the path specified by `comfy set-default <path>`.
+  - Run from the recently executed or installed ComfyUI.
+  - Run from the ComfyUI located in the current directory.
+
+- Example 1: To run the recently executed ComfyUI:
+  - `comfy --recent launch`
+- Example 2: To install a package on the ComfyUI in the current directory:
+  - `comfy --here node install ComfyUI-Impact-Pack`
+- Example 3: To update the automatically selected path of ComfyUI and custom nodes based on priority:
+
+  - `comfy node update all`
 
-* You can use the `comfy which` command to check the path of the target workspace.
-  * e.g) `comfy --recent which`, `comfy --here which`, `comfy which`, ...
+- You can use the `comfy which` command to check the path of the target workspace.
+  - e.g `comfy --recent which`, `comfy --here which`, `comfy which`, ...
+
+### Default Setup
+
+The default sets the option that will be executed by default when no specific workspace's ComfyUI has been set for the command.
+
+`comfy set-default <workspace path> ?[--launch-extras="<extra args>"]`
+
+- `--launch-extras` option specifies extra args that are applied only during launch by default. However, if extras are specified at the time of launch, this setting is ignored.
 
 ### Launch ComfyUI
 
 Comfy provides commands that allow you to easily run the installed ComfyUI.
 
-  `comfy launch`
+`comfy launch`
 
 - To run with default ComfyUI options:
 
   `comfy launch -- <extra args...>`
 
   `comfy launch -- --cpu --listen 0.0.0.0`
 
+  - When you manually configure the extra options, the extras set by set-default will be overridden.
+
 - To run background
 
   `comfy launch --background`
 
   `comfy --workspace=~/comfy launch --background -- --listen 10.0.0.10 --port 8000`
-  - Instances launched with `--background` are displayed in the "Background ComfyUI" section of `comfy env`, providing management functionalities for a single background instance only. 
+
+  - Instances launched with `--background` are displayed in the "Background ComfyUI" section of `comfy env`, providing management functionalities for a single background instance only.
   - Since "Comfy Server Running" in `comfy env` only shows the default port 8188, it doesn't display ComfyUI running on a different port.
   - Background-running ComfyUI can be stopped with `comfy stop`.
 
-
-### Managing Packages [WIP]
-
-comfy allows you to easily install, update, and remove packages for ComfyUI. Here are some examples:
-
-- Install a package:
-
-  `comfy package install package-name`
-
-- Update a package:
-
-  `comfy package update package-name`
-
-- Remove a package:
-
-  `comfy package remove package-name`
-
-- List installed packages:
-
-  `comfy package list`
-
-
 ### Managing Custom Nodes
 
 comfy provides a convenient way to manage custom nodes for extending ComfyUI's functionality. Here are some examples:
 
 - Show custom nodes' information:
- ```
-comfy node [show|simple-show] [installed|enabled|not-installed|disabled|all|snapshot|snapshot-list] 
-                              ?[--channel <channel name>] 
-                              ?[--mode [remote|local|cache]]
+
+```
+comfy node [show|simple-show] [installed|enabled|not-installed|disabled|all|snapshot|snapshot-list]
+                             ?[--channel <channel name>]
+                             ?[--mode [remote|local|cache]]
 ```
--
-  `comfy node show all --channel recent`
+
+- `comfy node show all --channel recent`
 
   `comfy node simple-show installed`
 
   `comfy node update all`
 
   `comfy node install ComfyUI-Impact-Pack`
 
-
 - Managing snapshot:
 
   `comfy node save-snapshot`
 
   `comfy node restore-snapshot <snapshot name>`
 
+- Install dependencies:
+
+  `comfy node install-deps --deps=<deps .json file>`
+
+  `comfy node install-deps --workflow=<workflow .json/.png file>`
+
+- Generate deps:
+
+  `comfy node deps-in-workflow --workflow=<workflow .json/.png file>`
 
 ### Managing Models
 
 - Model downloading
 
-  `comfy model get`
+  `comfy model download --url <URL> ?[--relative-path <PATH>] ?[--set-civitai-api-token <TOKEN>]`
 
-  *Downloading models that have already been installed will 
+  * URL: CivitAI, huggingface file url, ...
 
 - Model remove
 
-  `comfy model enable-gui`
+  `comfy model remove ?[--relative-path <PATH>] --model-names <model names>`
 
 - Model list
 
-  `comfy model list`
-
+  `comfy model list ?[--relative-path <PATH>]`
 
 ### Managing ComfyUI-Manager
 
 - disable GUI of ComfyUI-Manager (disable Manager menu and Server)
 
   `comfy manager disable-gui`
 
@@ -851,57 +875,68 @@
 
   `comfy manager enable-gui`
 
 - Clear reserved startup action:
 
   `comfy manager clear`
 
-
-## Format of comfy.yaml (WIP)
+## Beta Feature: format of comfy-lock.yaml (WIP)
 
 ```
 basic:
 
 models:
-  - model: [name of the model] 
+  - model: [name of the model]
     url: [url of the source, e.g. https://huggingface.co/...]
     paths: [list of paths to the model]
       - path: [path to the model]
       - path: [path to the model]
-    hash: [md5hash for the model]
+    hashes: [hashes for the model]
+      - hash: [hash]
+        type: [AutoV1, AutoV2, SHA256, CRC32, and Blake3]
     type: [type of the model, e.g. diffuser, lora, etc.]
 
   - model:
   ...
 
 # compatible with ComfyUI-Manager's .yaml snapshot
-custom_nodes:  
+custom_nodes:
   comfyui: [commit hash]
   file_custom_nodes:
   - disabled: [bool]
     filename: [.py filename]
     ...
   git_custom_nodes:
     [git-url]:
       disabled: [bool]
       hash: [commit hash]
     ...
 ```
 
+## Analytics
+
+We track analytics using Mixpanel to help us understand usage patterns and know where to prioritize our efforts. When you first download the cli, it will ask you to give consent. If at any point you wish to opt out:
+
+```
+comfy tracking disable
+```
+
+Check out the usage here: [Mixpanel Board](https://mixpanel.com/p/13hGfPfEPdRkjPtNaS7BYQ)
+
 ## Contributing
 
 We welcome contributions to comfy-cli! If you have any ideas, suggestions, or
 bug reports, please open an issue on our [GitHub
-repository](https://github.com/Comfy-Org/comfy-cli/issues). If you'd like to contribute code,
+repository](https://github.com/yoland68/comfy-cli/issues). If you'd like to contribute code,
 please fork the repository and submit a pull request.
 
+Check out the [Dev Guide](/DEV_README.md) for more details.
 
 ## License
 
-comfy is released under the [GNU General Public License v3.0](https://github.com/drip-art/comfy-cli/blob/master/LICENSE).
+comfy is released under the [GNU General Public License v3.0](https://github.com/yoland68/comfy-cli/blob/master/LICENSE).
 
 ## Support
 
-If you encounter any issues or have questions about comfy-cli, please [open an issue](https://github.com/comfy-cli/issues) on our GitHub repository. We'll be happy to assist you!
+If you encounter any issues or have questions about comfy-cli, please [open an issue](https://github.com/comfy-cli/issues) on our GitHub repository or contact us on [Discord](https://discord.gg/comfycontrib). We'll be happy to assist you!
 
 Happy diffusing with ComfyUI and comfy-cli! 🎉
-
```

### Comparing `comfy_cli-0.0.9/comfy_cli/logging.py` & `comfy_cli-0.27/comfy_cli/logging.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,18 +7,25 @@
 Note: we could potentially change the logging library or the way we log messages in the future.
 Therefore, it's a good idea to encapsulate logging-related code in a separate module.
 """
 
 
 def setup_logging():
     # TODO: consider supporting different ways of outputting logs
-    # Note: by default, the log level is set to INFO
-    log_level = os.getenv("LOG_LEVEL", "WARN").upper()
+    # Note: by default, the log level is set to WARN
+    log_levels = {
+        "DEBUG": logging.DEBUG,
+        "INFO": logging.INFO,
+        "WARNING": logging.WARNING,
+        "ERROR": logging.ERROR,
+        "CRITICAL": logging.CRITICAL,
+    }
+    log_level_key = os.getenv("LOG_LEVEL", "ERROR").upper()
     logging.basicConfig(
-        level=log_level,
+        level=log_levels.get(log_level_key, logging.WARNING),
         format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
 
 def debug(message):
     logging.debug(message)
```

### Comparing `comfy_cli-0.0.9/comfy_cli.egg-info/PKG-INFO` & `comfy_cli-0.27/comfy_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comfy-cli
-Version: 0.0.9
+Version: 0.27
 Summary: A CLI tool for installing and using ComfyUI.
 Maintainer-email: Yoland Yan <yoland@drip.art>, James Kwon <hongilkwon316@gmail.com>, Robin Huang <robin@drip.art>, "Dr.Lt.Data" <dr.lt.data@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -679,171 +679,195 @@
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Repository, https://github.com/drip-art/comfy-cli.git
 Keywords: comfyui,stable diffusion
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: typer>=0.3.0
+Requires-Dist: typer>=0.9.0
 Requires-Dist: GitPython
 Requires-Dist: rich
 Requires-Dist: requests
 Requires-Dist: pyyaml
-Requires-Dist: typing-extensions
+Requires-Dist: typing-extensions>=4.7.0
 Requires-Dist: mixpanel
 Requires-Dist: questionary
 Requires-Dist: psutil
+Requires-Dist: tomlkit
+Requires-Dist: pathspec
+Requires-Dist: httpx
+Requires-Dist: packaging
 
-# comfy-cli
+# Comfy-Cli: A Command Line Tool for ComfyUI
+[![Test ComfyUI Example Workflows](https://github.com/Comfy-Org/ComfyUI-Mirror/actions/workflows/test-workflows.yaml/badge.svg)](https://github.com/Comfy-Org/ComfyUI-Mirror/actions/workflows/test-workflows.yaml)
+[![Test ComfyUI Windows with Default Workflow](https://github.com/Comfy-Org/ComfyUI-Mirror/actions/workflows/test-workflows-windows.yaml/badge.svg)](https://github.com/Comfy-Org/ComfyUI-Mirror/actions/workflows/test-workflows-windows.yaml)
 
-comfy-cli is a command line tool that helps users easily install and manage [ComfyUI](https://github.com/comfyanonymous/ComfyUI), a powerful open-source machine learning framework. With comfy-cli, you can quickly set up ComfyUI, install packages, and manage custom nodes, all from the convenience of your terminal.
+comfy-cli is a command line tool that helps users easily install and manage
+[ComfyUI](https://github.com/comfyanonymous/ComfyUI), a powerful open-source
+machine learning framework. With comfy-cli, you can quickly set up ComfyUI,
+install packages, and manage custom nodes, all from the convenience of your
+terminal.
+
+
+
+## Demo
+
+<img src="https://github.com/yoland68/comfy-cli/raw/main/assets/comfy-demo.gif" width="400" alt="Comfy Command Demo">
 
 ## Features
 
 - 🚀 Easy installation of ComfyUI with a single command
 - 📦 Seamless package management for ComfyUI extensions and dependencies
 - 🔧 Custom node management for extending ComfyUI's functionality
+- 🗄️ Download checkpoints and save model hash
 - 💻 Cross-platform compatibility (Windows, macOS, Linux)
 - 📖 Comprehensive documentation and examples
 
 ## Installation
 
-To install comfy-cli, make sure you have Python 3.7 or higher installed on your system. Then, run the following command:
+1. (Recommended, but not necessary) Enable virtual environment ([venv](https://docs.python.org/3/library/venv.html)/[conda](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html))
+
+2. To install comfy-cli, make sure you have Python 3.9 or higher installed on your system. Then, run the following command:
+
+   `pip install comfy-cli`
 
-`pip install comfy-cli`
+### Shell Autocomplete
 
+To install autocompletion hints in your shell run:
+
+`comfy --install-completion`
+
+This enables you to type `comfy [TAP]` to autocomplete commands and options
 
 ## Usage
 
 ### Installing ComfyUI
 
 To install ComfyUI using comfy, simply run:
 
 `comfy install`
 
 This command will download and set up the latest version of ComfyUI and ComfyUI-Manager on your
 system. If you run in a ComfyUI repo that has already been setup. The command
 will simply update the comfy.yaml file to reflect the local setup
 
-  * `comfy install --skip-manager`: Install ComfyUI without ComfyUI-Manager.
-  * `comfy --workspace=<path> install`: Install ComfyUI into `<path>/ComfyUI`.
-  * For `comfy install`, if no path specification like `--workspace, --recent, or --here` is provided, it will be implicitly installed in `<HOME>/comfy`.
-
+- `comfy install --skip-manager`: Install ComfyUI without ComfyUI-Manager.
+- `comfy --workspace=<path> install`: Install ComfyUI into `<path>/ComfyUI`.
+- For `comfy install`, if no path specification like `--workspace, --recent, or --here` is provided, it will be implicitly installed in `<HOME>/comfy`.
 
 ### Specifying execution path
 
-* You can specify the path of ComfyUI where the command will be applied through path indicators as follows:
-  * `comfy --workspace=<path>`: Run from the ComfyUI installed in the specified workspace.
-  * `comfy --recent`: Run from the recently executed or installed ComfyUI.
-  * `comfy --here`: Run from the ComfyUI located in the current directory.
-* --workspace, --recent, and --here options cannot be used simultaneously.
-* If there is no path indicator, the following priority applies:
-  * Run from the default ComfyUI at the path specified by `comfy set-default <path>`.
-  * Run from the recently executed or installed ComfyUI.
-  * Run from the ComfyUI located in the current directory.
-
-* Example 1: To run the recently executed ComfyUI:
-  * `comfy --recent launch`
-* Example 2: To install a package on the ComfyUI in the current directory:
-  * `comfy --here node install ComfyUI-Impact-Pack`
-* Example 3: To update the automatically selected path of ComfyUI and custom nodes based on priority:
-  * `comfy node update all`
+- You can specify the path of ComfyUI where the command will be applied through path indicators as follows:
+  - `comfy --workspace=<path>`: Run from the ComfyUI installed in the specified workspace.
+  - `comfy --recent`: Run from the recently executed or installed ComfyUI.
+  - `comfy --here`: Run from the ComfyUI located in the current directory.
+- --workspace, --recent, and --here options cannot be used simultaneously.
+- If there is no path indicator, the following priority applies:
+
+  - Run from the default ComfyUI at the path specified by `comfy set-default <path>`.
+  - Run from the recently executed or installed ComfyUI.
+  - Run from the ComfyUI located in the current directory.
+
+- Example 1: To run the recently executed ComfyUI:
+  - `comfy --recent launch`
+- Example 2: To install a package on the ComfyUI in the current directory:
+  - `comfy --here node install ComfyUI-Impact-Pack`
+- Example 3: To update the automatically selected path of ComfyUI and custom nodes based on priority:
+
+  - `comfy node update all`
 
-* You can use the `comfy which` command to check the path of the target workspace.
-  * e.g) `comfy --recent which`, `comfy --here which`, `comfy which`, ...
+- You can use the `comfy which` command to check the path of the target workspace.
+  - e.g `comfy --recent which`, `comfy --here which`, `comfy which`, ...
+
+### Default Setup
+
+The default sets the option that will be executed by default when no specific workspace's ComfyUI has been set for the command.
+
+`comfy set-default <workspace path> ?[--launch-extras="<extra args>"]`
+
+- `--launch-extras` option specifies extra args that are applied only during launch by default. However, if extras are specified at the time of launch, this setting is ignored.
 
 ### Launch ComfyUI
 
 Comfy provides commands that allow you to easily run the installed ComfyUI.
 
-  `comfy launch`
+`comfy launch`
 
 - To run with default ComfyUI options:
 
   `comfy launch -- <extra args...>`
 
   `comfy launch -- --cpu --listen 0.0.0.0`
 
+  - When you manually configure the extra options, the extras set by set-default will be overridden.
+
 - To run background
 
   `comfy launch --background`
 
   `comfy --workspace=~/comfy launch --background -- --listen 10.0.0.10 --port 8000`
-  - Instances launched with `--background` are displayed in the "Background ComfyUI" section of `comfy env`, providing management functionalities for a single background instance only. 
+
+  - Instances launched with `--background` are displayed in the "Background ComfyUI" section of `comfy env`, providing management functionalities for a single background instance only.
   - Since "Comfy Server Running" in `comfy env` only shows the default port 8188, it doesn't display ComfyUI running on a different port.
   - Background-running ComfyUI can be stopped with `comfy stop`.
 
-
-### Managing Packages [WIP]
-
-comfy allows you to easily install, update, and remove packages for ComfyUI. Here are some examples:
-
-- Install a package:
-
-  `comfy package install package-name`
-
-- Update a package:
-
-  `comfy package update package-name`
-
-- Remove a package:
-
-  `comfy package remove package-name`
-
-- List installed packages:
-
-  `comfy package list`
-
-
 ### Managing Custom Nodes
 
 comfy provides a convenient way to manage custom nodes for extending ComfyUI's functionality. Here are some examples:
 
 - Show custom nodes' information:
- ```
-comfy node [show|simple-show] [installed|enabled|not-installed|disabled|all|snapshot|snapshot-list] 
-                              ?[--channel <channel name>] 
-                              ?[--mode [remote|local|cache]]
+
+```
+comfy node [show|simple-show] [installed|enabled|not-installed|disabled|all|snapshot|snapshot-list]
+                             ?[--channel <channel name>]
+                             ?[--mode [remote|local|cache]]
 ```
--
-  `comfy node show all --channel recent`
+
+- `comfy node show all --channel recent`
 
   `comfy node simple-show installed`
 
   `comfy node update all`
 
   `comfy node install ComfyUI-Impact-Pack`
 
-
 - Managing snapshot:
 
   `comfy node save-snapshot`
 
   `comfy node restore-snapshot <snapshot name>`
 
+- Install dependencies:
+
+  `comfy node install-deps --deps=<deps .json file>`
+
+  `comfy node install-deps --workflow=<workflow .json/.png file>`
+
+- Generate deps:
+
+  `comfy node deps-in-workflow --workflow=<workflow .json/.png file>`
 
 ### Managing Models
 
 - Model downloading
 
-  `comfy model get`
+  `comfy model download --url <URL> ?[--relative-path <PATH>] ?[--set-civitai-api-token <TOKEN>]`
 
-  *Downloading models that have already been installed will 
+  * URL: CivitAI, huggingface file url, ...
 
 - Model remove
 
-  `comfy model enable-gui`
+  `comfy model remove ?[--relative-path <PATH>] --model-names <model names>`
 
 - Model list
 
-  `comfy model list`
-
+  `comfy model list ?[--relative-path <PATH>]`
 
 ### Managing ComfyUI-Manager
 
 - disable GUI of ComfyUI-Manager (disable Manager menu and Server)
 
   `comfy manager disable-gui`
 
@@ -851,57 +875,68 @@
 
   `comfy manager enable-gui`
 
 - Clear reserved startup action:
 
   `comfy manager clear`
 
-
-## Format of comfy.yaml (WIP)
+## Beta Feature: format of comfy-lock.yaml (WIP)
 
 ```
 basic:
 
 models:
-  - model: [name of the model] 
+  - model: [name of the model]
     url: [url of the source, e.g. https://huggingface.co/...]
     paths: [list of paths to the model]
       - path: [path to the model]
       - path: [path to the model]
-    hash: [md5hash for the model]
+    hashes: [hashes for the model]
+      - hash: [hash]
+        type: [AutoV1, AutoV2, SHA256, CRC32, and Blake3]
     type: [type of the model, e.g. diffuser, lora, etc.]
 
   - model:
   ...
 
 # compatible with ComfyUI-Manager's .yaml snapshot
-custom_nodes:  
+custom_nodes:
   comfyui: [commit hash]
   file_custom_nodes:
   - disabled: [bool]
     filename: [.py filename]
     ...
   git_custom_nodes:
     [git-url]:
       disabled: [bool]
       hash: [commit hash]
     ...
 ```
 
+## Analytics
+
+We track analytics using Mixpanel to help us understand usage patterns and know where to prioritize our efforts. When you first download the cli, it will ask you to give consent. If at any point you wish to opt out:
+
+```
+comfy tracking disable
+```
+
+Check out the usage here: [Mixpanel Board](https://mixpanel.com/p/13hGfPfEPdRkjPtNaS7BYQ)
+
 ## Contributing
 
 We welcome contributions to comfy-cli! If you have any ideas, suggestions, or
 bug reports, please open an issue on our [GitHub
-repository](https://github.com/Comfy-Org/comfy-cli/issues). If you'd like to contribute code,
+repository](https://github.com/yoland68/comfy-cli/issues). If you'd like to contribute code,
 please fork the repository and submit a pull request.
 
+Check out the [Dev Guide](/DEV_README.md) for more details.
 
 ## License
 
-comfy is released under the [GNU General Public License v3.0](https://github.com/drip-art/comfy-cli/blob/master/LICENSE).
+comfy is released under the [GNU General Public License v3.0](https://github.com/yoland68/comfy-cli/blob/master/LICENSE).
 
 ## Support
 
-If you encounter any issues or have questions about comfy-cli, please [open an issue](https://github.com/comfy-cli/issues) on our GitHub repository. We'll be happy to assist you!
+If you encounter any issues or have questions about comfy-cli, please [open an issue](https://github.com/comfy-cli/issues) on our GitHub repository or contact us on [Discord](https://discord.gg/comfycontrib). We'll be happy to assist you!
 
 Happy diffusing with ComfyUI and comfy-cli! 🎉
-
```

### Comparing `comfy_cli-0.0.9/comfy_cli.egg-info/SOURCES.txt` & `comfy_cli-0.27/comfy_cli.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,25 +3,30 @@
 pyproject.toml
 comfy_cli/__init__.py
 comfy_cli/__main__.py
 comfy_cli/cmdline.py
 comfy_cli/config_manager.py
 comfy_cli/constants.py
 comfy_cli/env_checker.py
+comfy_cli/file_utils.py
 comfy_cli/logging.py
-comfy_cli/meta_data.py
 comfy_cli/tracking.py
 comfy_cli/ui.py
+comfy_cli/update.py
 comfy_cli/utils.py
 comfy_cli/workspace_manager.py
 comfy_cli.egg-info/PKG-INFO
 comfy_cli.egg-info/SOURCES.txt
 comfy_cli.egg-info/dependency_links.txt
 comfy_cli.egg-info/entry_points.txt
 comfy_cli.egg-info/requires.txt
 comfy_cli.egg-info/top_level.txt
 comfy_cli/command/__init__.py
 comfy_cli/command/install.py
 comfy_cli/command/run.py
 comfy_cli/command/custom_nodes/__init__.py
 comfy_cli/command/custom_nodes/command.py
-comfy_cli/command/models/models.py
+comfy_cli/command/models/models.py
+comfy_cli/registry/__init__.py
+comfy_cli/registry/api.py
+comfy_cli/registry/config_parser.py
+comfy_cli/registry/types.py
```

### Comparing `comfy_cli-0.0.9/pyproject.toml` & `comfy_cli-0.27/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "comfy-cli"
 license = {file = "LICENSE"}
-version = "v0.0.9"
-requires-python = ">= 3.8"
+version = "v0.027" # Will be filled in by the CI/CD pipeline. Check publish_package.py.
+requires-python = ">= 3.9"
 description = "A CLI tool for installing and using ComfyUI."
 readme = "README.md"
 keywords = ["comfyui", "stable diffusion"]
 
 maintainers = [
   {name = "Yoland Yan", email = "yoland@drip.art"},
   {name = "James Kwon", email = "hongilkwon316@gmail.com"},
   {name = "Robin Huang", email = "robin@drip.art"},
   {name = "Dr.Lt.Data", email = "dr.lt.data@gmail.com"}
 ]
 
 dependencies = [
-    "typer>=0.3.0",
+    "typer>=0.9.0",
     "GitPython",
     "rich",
     "requests",
     "pyyaml",
-    "typing-extensions",
+    "typing-extensions>=4.7.0",
     "mixpanel",
     "questionary",
     "psutil",
+    "tomlkit",
+    "pathspec",
+    "httpx",
+    "packaging",
 ]
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
 ]
@@ -40,9 +44,11 @@
 comfy = "comfy_cli.__main__:main"
 comfy-cli = "comfy_cli.__main__:main"
 comfycli = "comfy_cli.__main__:main"
 
 [project.urls]
 Repository = "https://github.com/drip-art/comfy-cli.git"
 
-
+[tool.setuptools.packages.find]
+where = ["."]
+include = ["comfy_cli*"]
```

