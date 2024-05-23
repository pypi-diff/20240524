# Comparing `tmp/spin-0.8.tar.gz` & `tmp/spin-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spin-0.8.tar", last modified: Wed Nov 15 19:02:41 2023, max compression
+gzip compressed data, was "spin-0.9.tar", last modified: Fri May  3 12:21:52 2024, max compression
```

## Comparing `spin-0.8.tar` & `spin-0.9.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:02:41.598855 spin-0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-11-15 19:02:29.000000 spin-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2023-11-15 19:02:41.598855 spin-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7420 2023-11-15 19:02:29.000000 spin-0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2023-11-15 19:02:29.000000 spin-0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 19:02:41.598855 spin-0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:02:41.594855 spin-0.8/spin/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-11-15 19:02:29.000000 spin-0.8/spin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2023-11-15 19:02:29.000000 spin-0.8/spin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:02:41.594855 spin-0.8/spin/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-11-15 19:02:29.000000 spin-0.8/spin/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-11-15 19:02:29.000000 spin-0.8/spin/cmds/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    19501 2023-11-15 19:02:29.000000 spin-0.8/spin/cmds/meson.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-11-15 19:02:29.000000 spin-0.8/spin/cmds/pip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2023-11-15 19:02:29.000000 spin-0.8/spin/cmds/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2023-11-15 19:02:29.000000 spin-0.8/spin/color_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-11-15 19:02:29.000000 spin-0.8/spin/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-11-15 19:02:29.000000 spin-0.8/spin/sectioned_help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:02:41.594855 spin-0.8/spin/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2023-11-15 19:02:29.000000 spin-0.8/spin/tests/test_meson.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:02:41.594855 spin-0.8/spin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2023-11-15 19:02:41.000000 spin-0.8/spin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-11-15 19:02:41.000000 spin-0.8/spin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 19:02:41.000000 spin-0.8/spin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-11-15 19:02:41.000000 spin-0.8/spin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-11-15 19:02:41.000000 spin-0.8/spin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-15 19:02:41.000000 spin-0.8/spin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:52.509849 spin-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-03 12:21:43.000000 spin-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-05-03 12:21:52.509849 spin-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-05-03 12:21:43.000000 spin-0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-03 12:21:43.000000 spin-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:21:52.509849 spin-0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:52.505849 spin-0.9/spin/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-03 12:21:43.000000 spin-0.9/spin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-03 12:21:43.000000 spin-0.9/spin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:52.509849 spin-0.9/spin/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-03 12:21:43.000000 spin-0.9/spin/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-03 12:21:43.000000 spin-0.9/spin/cmds/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26966 2024-05-03 12:21:43.000000 spin-0.9/spin/cmds/meson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-03 12:21:43.000000 spin-0.9/spin/cmds/pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-03 12:21:43.000000 spin-0.9/spin/cmds/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-03 12:21:43.000000 spin-0.9/spin/color_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-03 12:21:43.000000 spin-0.9/spin/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-03 12:21:43.000000 spin-0.9/spin/sectioned_help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:52.509849 spin-0.9/spin/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-03 12:21:43.000000 spin-0.9/spin/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-03 12:21:43.000000 spin-0.9/spin/tests/test_build_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-03 12:21:43.000000 spin-0.9/spin/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-03 12:21:43.000000 spin-0.9/spin/tests/test_editable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-03 12:21:43.000000 spin-0.9/spin/tests/test_meson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-03 12:21:43.000000 spin-0.9/spin/tests/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:52.509849 spin-0.9/spin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-05-03 12:21:52.000000 spin-0.9/spin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-03 12:21:52.000000 spin-0.9/spin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:21:52.000000 spin-0.9/spin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 12:21:52.000000 spin-0.9/spin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-03 12:21:52.000000 spin-0.9/spin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 12:21:52.000000 spin-0.9/spin.egg-info/top_level.txt
```

### Comparing `spin-0.8/LICENSE` & `spin-0.9/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2021--2022, Scientific Python project
+Copyright (c) 2021--2024, Scientific Python project
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `spin-0.8/PKG-INFO` & `spin-0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: spin
-Version: 0.8
+Version: 0.9
 Summary: Developer tool for scientific Python libraries
 Maintainer-email: Scientific Python <spin@discuss.scientific-python.org>
 License: BSD 3-Clause License
         
-        Copyright (c) 2021--2022, Scientific Python project
+        Copyright (c) 2021--2024, Scientific Python project
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
@@ -49,32 +49,36 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: tomli; python_version < "3.11"
 Requires-Dist: colorama; platform_system == "Windows"
+Requires-Dist: importlib_metadata>=7
 Provides-Extra: lint
-Requires-Dist: pre-commit==3.5.0; extra == "lint"
+Requires-Dist: pre-commit==3.7.0; extra == "lint"
 Provides-Extra: dev
-Requires-Dist: changelist==0.4; extra == "dev"
+Requires-Dist: changelist==0.5; extra == "dev"
 
 # 💫 Scientific Python INcantations (`spin`)
 
 ## A developer tool for scientific Python libraries
 
 Developers need to memorize a whole bunch of magic command-line incantations.
-And these incantations change from time to time!
-Typically, their lives are made simpler by a Makefile, but Makefiles can be convoluted, are not written in Python, and are hard to extend.
-The rationale behind `spin` is therefore to provide a simple interface for common development tasks.
+These incantations may also change over time.
+Often, Makefiles are used to provide aliases, but Makefiles can be convoluted, are not written in Python, and are hard to extend.
+The goal of `spin` is therefore to provide a simple, user-friendly, extendable interface for common development tasks.
 It comes with a few common build commands out the box, but can easily be customized per project.
 
 As a curiosity: the impetus behind developing the tool was the mass migration of scientific Python libraries (SciPy, scikit-image, and NumPy, etc.) to Meson, after distutils was deprecated.
 When many of the build and installation commands changed, it made sense to abstract away the nuisance of having to re-learn them.
 
+_Note:_ We now have experimental builds for editable installs.
+Most of the Meson commands listed below should work "out of the box" for those.
+
 ## Installation
 
 ```
 pip install spin
 ```
 
 ## Configuration
@@ -148,15 +152,14 @@
   python   🐍 Launch Python shell with PYTHONPATH set
   shell    💻 Launch shell with PYTHONPATH set
   test     🔧 Run pytest
   run      🏁 Run a shell command with PYTHONPATH set
   docs     📖 Build Sphinx documentation
   gdb      👾 Execute a Python snippet with GDB
   lldb     👾 Execute a Python snippet with LLDB
-  install  💽 Build and install package using pip.
 ```
 
 ### [Build](https://pypa-build.readthedocs.io/en/stable/) (PEP 517 builder)
 
 Available as `spin.cmds.build.*`:
 
 ```
@@ -203,14 +206,37 @@
 @click.command()
 def example():
     """Command that accesses `pyproject.toml` configuration"""
     config = util.get_config()
     print(config["tool.spin"])
 ```
 
+### Argument overrides
+
+Default arguments can be overridden for any command.
+The custom command above, e.g., has the following signature:
+
+```python
+@click.command()
+@click.option("-f", "--flag")
+@click.option("-t", "--test", default="not set")
+def example(flag, test, default_kwd=None):
+    """🧪 Example custom command.
+    ...
+    """
+```
+
+Use the `[tool.spin.kwargs]` section to override default values for
+click options or function keywords:
+
+```toml
+[tool.spin.kwargs]
+".spin/cmds.py:example" = {"test" = "default override", "default_kwd" = 3}
+```
+
 ### Advanced: adding arguments to built-in commands
 
 Instead of rewriting a command from scratch, a project may want to add a flag to a built-in `spin` command, or perhaps do some pre- or post-processing.
 For this, we have to use an internal Click concept called a [context](https://click.palletsprojects.com/en/8.1.x/complex/#contexts).
 Fortunately, we don't need to know anything about contexts other than that they allow us to execute commands within commands.
 
 We proceed by duplicating the function header of the existing command, and adding our own flag:
@@ -280,15 +306,15 @@
 
 ## For contributors
 
 `spin` development happens on GitHub at [scientific-python/spin](https://github.com/scientific-python/spin).
 `spin` tests are invoked using:
 
 ```
-nox -s tests
+nox -s test
 ```
 
 ## History
 
 The `dev.py` tool was [proposed for SciPy](https://github.com/scipy/scipy/issues/15489) by Ralf Gommers and [implemented](https://github.com/scipy/scipy/pull/15959) by Sayantika Banik, Eduardo Naufel Schettino, and Ralf Gommers (also see [Sayantika's blog post](https://labs.quansight.org/blog/the-evolution-of-the-scipy-developer-cli)).
 Inspired by that implementation, `spin` (this package) is a minimal rewrite by Stéfan van der Walt, that aims to be easily extendable so that it can be used across ecosystem libraries.
 We thank Danila Bredikhin and Luca Marconato who kindly donated the `spin` name on PyPi.
```

### Comparing `spin-0.8/README.md` & `spin-0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # 💫 Scientific Python INcantations (`spin`)
 
 ## A developer tool for scientific Python libraries
 
 Developers need to memorize a whole bunch of magic command-line incantations.
-And these incantations change from time to time!
-Typically, their lives are made simpler by a Makefile, but Makefiles can be convoluted, are not written in Python, and are hard to extend.
-The rationale behind `spin` is therefore to provide a simple interface for common development tasks.
+These incantations may also change over time.
+Often, Makefiles are used to provide aliases, but Makefiles can be convoluted, are not written in Python, and are hard to extend.
+The goal of `spin` is therefore to provide a simple, user-friendly, extendable interface for common development tasks.
 It comes with a few common build commands out the box, but can easily be customized per project.
 
 As a curiosity: the impetus behind developing the tool was the mass migration of scientific Python libraries (SciPy, scikit-image, and NumPy, etc.) to Meson, after distutils was deprecated.
 When many of the build and installation commands changed, it made sense to abstract away the nuisance of having to re-learn them.
 
+_Note:_ We now have experimental builds for editable installs.
+Most of the Meson commands listed below should work "out of the box" for those.
+
 ## Installation
 
 ```
 pip install spin
 ```
 
 ## Configuration
@@ -88,15 +91,14 @@
   python   🐍 Launch Python shell with PYTHONPATH set
   shell    💻 Launch shell with PYTHONPATH set
   test     🔧 Run pytest
   run      🏁 Run a shell command with PYTHONPATH set
   docs     📖 Build Sphinx documentation
   gdb      👾 Execute a Python snippet with GDB
   lldb     👾 Execute a Python snippet with LLDB
-  install  💽 Build and install package using pip.
 ```
 
 ### [Build](https://pypa-build.readthedocs.io/en/stable/) (PEP 517 builder)
 
 Available as `spin.cmds.build.*`:
 
 ```
@@ -143,14 +145,37 @@
 @click.command()
 def example():
     """Command that accesses `pyproject.toml` configuration"""
     config = util.get_config()
     print(config["tool.spin"])
 ```
 
+### Argument overrides
+
+Default arguments can be overridden for any command.
+The custom command above, e.g., has the following signature:
+
+```python
+@click.command()
+@click.option("-f", "--flag")
+@click.option("-t", "--test", default="not set")
+def example(flag, test, default_kwd=None):
+    """🧪 Example custom command.
+    ...
+    """
+```
+
+Use the `[tool.spin.kwargs]` section to override default values for
+click options or function keywords:
+
+```toml
+[tool.spin.kwargs]
+".spin/cmds.py:example" = {"test" = "default override", "default_kwd" = 3}
+```
+
 ### Advanced: adding arguments to built-in commands
 
 Instead of rewriting a command from scratch, a project may want to add a flag to a built-in `spin` command, or perhaps do some pre- or post-processing.
 For this, we have to use an internal Click concept called a [context](https://click.palletsprojects.com/en/8.1.x/complex/#contexts).
 Fortunately, we don't need to know anything about contexts other than that they allow us to execute commands within commands.
 
 We proceed by duplicating the function header of the existing command, and adding our own flag:
@@ -220,15 +245,15 @@
 
 ## For contributors
 
 `spin` development happens on GitHub at [scientific-python/spin](https://github.com/scientific-python/spin).
 `spin` tests are invoked using:
 
 ```
-nox -s tests
+nox -s test
 ```
 
 ## History
 
 The `dev.py` tool was [proposed for SciPy](https://github.com/scipy/scipy/issues/15489) by Ralf Gommers and [implemented](https://github.com/scipy/scipy/pull/15959) by Sayantika Banik, Eduardo Naufel Schettino, and Ralf Gommers (also see [Sayantika's blog post](https://labs.quansight.org/blog/the-evolution-of-the-scipy-developer-cli)).
 Inspired by that implementation, `spin` (this package) is a minimal rewrite by Stéfan van der Walt, that aims to be easily extendable so that it can be used across ecosystem libraries.
 We thank Danila Bredikhin and Luca Marconato who kindly donated the `spin` name on PyPi.
```

### Comparing `spin-0.8/pyproject.toml` & `spin-0.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -21,24 +21,25 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
   "click",
   "tomli; python_version < '3.11'",
-  "colorama; platform_system == 'Windows'"
+  "colorama; platform_system == 'Windows'",
+  "importlib_metadata >= 7"
 ]
 dynamic = ['version']
 
 [project.scripts]
 spin = "spin.__main__:main"
 
 [project.optional-dependencies]
-lint = ["pre-commit == 3.5.0"]
-dev = ["changelist == 0.4"]
+lint = ["pre-commit == 3.7.0"]
+dev = ["changelist == 0.5"]
 
 [project.urls]
 homepage = "https://github.com/scientific-python/spin"
 
 [tool.setuptools.dynamic.version]
 attr = 'spin.__version__'
```

### Comparing `spin-0.8/spin/__main__.py` & `spin-0.9/spin/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,62 +21,68 @@
 
 
 def main():
     # Alias `spin help` to `spin --help`
     if (len(sys.argv) == 2) and (sys.argv[1] == "help"):
         sys.argv[1] = "--help"
 
-    def error(message):
-        print(f"Error: {message}", file=sys.stderr)
-        sys.exit(1)
-
     def load_toml(filename):
         if not os.path.exists(filename):
             return None
         with open(filename, "rb") as f:
             try:
                 return tomllib.load(f)
             except tomllib.TOMLDecodeError:
-                error("cannot parse [{filename}]")
+                print(f"Error: cannot parse [{filename}]", file=sys.stderr)
 
     toml_config = collections.ChainMap()
     toml_config.maps.extend(
         DotDict(cfg)
         for filename in (
             ".spin.toml",
             "spin.toml",
             "pyproject.toml",
         )
         if (cfg := load_toml(filename))
     )
 
     # Basic configuration validation
-    if "tool.spin" not in toml_config:
-        error(
-            "needs valid configuration in [.spin.toml], [spin.toml] or [pyproject.toml]"
-        )
-    if "tool.spin.commands" not in toml_config:
-        error("configuration is missing section [tool.spin.commands]")
+    version_query = len(sys.argv) == 2 and (sys.argv[1] == "--version")
+
+    spin_config = {}
+    if not version_query:
+        if "tool.spin" in toml_config:
+            spin_config = toml_config["tool.spin"]
+            if "tool.spin.commands" not in toml_config:
+                print(
+                    "Error: configuration is missing section [tool.spin.commands]\n",
+                    file=sys.stderr,
+                )
+        else:
+            print(
+                "Error: need valid configuration in [.spin.toml], [spin.toml], or [pyproject.toml]\n"
+                "See https://github.com/scientific-python/spin/blob/main/README.md\n",
+                file=sys.stderr,
+            )
 
-    spin_config = toml_config["tool.spin"]
     proj_name = (
         toml_config.get("project.name")
         or spin_config.get("package")
-        or "unknown project"
+        or "[unknown project]"
     )
 
     @click.group(help=f"Developer tool for {proj_name}", cls=SectionedHelpGroup)
     @click.version_option(__version__, message="%(prog)s %(version)s")
     @click.pass_context
     def group(ctx):
         ctx.meta["config"] = toml_config
         ctx.meta["commands"] = ctx.command.section_commands
         ctx.show_default = True
 
-    config_cmds = spin_config["commands"]
+    config_cmds = spin_config.get("commands", [])
     # Commands can be provided as a list, or as a dictionary
     # so that they can be sorted into sections
     if isinstance(config_cmds, list):
         config_cmds = {"Commands": config_cmds}
 
     # Backward compatibility workaround
     # Originally, you could specify any of these commands as `spin.cmd`
@@ -84,14 +90,15 @@
     commands = {
         "spin.build": _cmds.meson.build,
         "spin.test": _cmds.meson.test,
         "spin.ipython": _cmds.meson.ipython,
         "spin.python": _cmds.meson.python,
         "spin.shell": _cmds.meson.shell,
     }
+    cmd_default_kwargs = toml_config.get("tool.spin.kwargs", {})
 
     for section, cmds in config_cmds.items():
         for cmd in cmds:
             if cmd not in commands:
                 # First, see if we can directly import the command
                 if ":" not in cmd:
                     path, func = cmd.rsplit(".", maxsplit=1)
@@ -123,19 +130,32 @@
 
                 try:
                     cmd_func = getattr(mod, func)
                 except AttributeError:
                     print(f"!! Could not load command `{func}` from file `{path}`.\n")
                     continue
 
+                default_kwargs = cmd_default_kwargs.get(cmd)
+                import functools
+
+                if default_kwargs:
+                    callback = cmd_func.callback
+                    cmd_func.callback = functools.partial(callback, **default_kwargs)
+
+                    # Also override option defaults
+                    for option in cmd_func.params:
+                        if option.name in default_kwargs:
+                            option.default = default_kwargs[option.name]
+
                 commands[cmd] = cmd_func
 
             group.add_command(commands[cmd], section=section)
 
     try:
         group()
     except Exception as e:
-        error(f"{e}; aborting.")
+        print(f"Error: {e}; aborting.", file=sys.stderr)
+        sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `spin-0.8/spin/cmds/meson.py` & `spin-0.9/spin/cmds/meson.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 import contextlib
+import copy
 import json
 import os
+import re
 import shutil
 import sys
+from enum import Enum
+from pathlib import Path
 
 import click
 
 from .util import get_commands, get_config
 from .util import run as _run
 
 install_dir = "build-install"
+build_dir = "build"
+
+
+class GcovReportFormat(str, Enum):
+    html = "html"
+    xml = "xml"
+    text = "text"
+    sonarqube = "sonarqube"
 
 
 # Allow specification of meson binary in configuration
 # This is necessary for packages like NumPy that vendor meson
 def _meson_cli():
     cfg = get_config()
     meson_cli = os.path.expanduser(cfg.get("tool.spin.meson.cli", "meson"))
@@ -21,38 +33,96 @@
     # Handle Python runner, mainly for Windows
     if meson_cli.endswith(".py"):
         return [sys.executable, meson_cli]
     else:
         return [meson_cli]
 
 
+def _editable_install_path(distname):
+    import importlib_metadata
+
+    try:
+        dist = importlib_metadata.Distribution.from_name(distname)
+    except importlib_metadata.PackageNotFoundError:
+        return None
+
+    if getattr(dist.origin.dir_info, "editable", False):
+        if sys.platform == "win32":
+            return dist.origin.url.removeprefix("file:///")
+        else:
+            return dist.origin.url.removeprefix("file://")
+    else:
+        return None
+
+
+def _is_editable_install(distname):
+    return _editable_install_path(distname) is not None
+
+
+def _is_editable_install_of_same_source(distname):
+    editable_path = _editable_install_path(distname)
+    return editable_path and os.path.samefile(_editable_install_path(distname), ".")
+
+
 def _set_pythonpath(quiet=False):
     """Set first entry of PYTHONPATH to site packages directory.
 
     Returns
     -------
     site_packages
     """
     site_packages = _get_site_packages()
     env = os.environ
 
+    cfg = get_config()
+    distname = cfg.get("project.name", None)
+    if distname:
+        if _is_editable_install(distname):
+            if _is_editable_install_of_same_source(distname):
+                if not (quiet):
+                    click.secho(
+                        "Editable install of same source directory detected; not setting PYTHONPATH",
+                        fg="bright_red",
+                    )
+                return ""
+            else:
+                # Ignoring the quiet flag, because picking up the wrong package is problematic
+                click.secho(
+                    f"Warning! Editable install of `{distname}`, from a different source location, detected.",
+                    fg="bright_red",
+                )
+                click.secho("Spin commands will pick up that version.", fg="bright_red")
+                click.secho(
+                    f"Try removing the other installation by switching to its source and running `pip uninstall {distname}`.",
+                    fg="bright_red",
+                )
+
     if "PYTHONPATH" in env:
         env["PYTHONPATH"] = f"{site_packages}{os.pathsep}{env['PYTHONPATH']}"
     else:
         env["PYTHONPATH"] = site_packages
 
     if not quiet:
         click.secho(
             f'$ export PYTHONPATH="{env["PYTHONPATH"]}"', bold=True, fg="bright_blue"
         )
 
     return site_packages
 
 
 def _get_site_packages():
+    try:
+        cfg = get_config()
+        distname = cfg.get("project.name", None)
+        if _is_editable_install_of_same_source(distname):
+            return ""
+    except RuntimeError:
+        # Probably not running in click
+        pass
+
     candidate_paths = []
     for root, dirs, _files in os.walk(install_dir):
         for subdir in dirs:
             if subdir == "site-packages" or subdir == "dist-packages":
                 candidate_paths.append(os.path.abspath(os.path.join(root, subdir)))
 
     X, Y = sys.version_info.major, sys.version_info.minor
@@ -99,22 +169,75 @@
         with open(meson_info_fn) as f:
             meson_info = json.load(f)
         return meson_info["meson_version"]["full"]
     except:
         pass
 
 
+def _meson_coverage_configured() -> bool:
+    try:
+        build_options_fn = os.path.join(
+            "build", "meson-info", "intro-buildoptions.json"
+        )
+        with open(build_options_fn) as f:
+            build_options = json.load(f)
+        for b in build_options:
+            if (b["name"] == "b_coverage") and (b["value"] is True):
+                return True
+    except:
+        pass
+
+    return False
+
+
+def _check_coverage_tool_installation(coverage_type: GcovReportFormat):
+    requirements = {  # https://github.com/mesonbuild/meson/blob/6e381714c7cb15877e2bcaa304b93c212252ada3/docs/markdown/Unit-tests.md?plain=1#L49-L62
+        GcovReportFormat.html: ["Gcovr/GenHTML", "lcov"],
+        GcovReportFormat.xml: ["Gcovr (version 3.3 or higher)"],
+        GcovReportFormat.text: ["Gcovr (version 3.3 or higher)"],
+        GcovReportFormat.sonarqube: ["Gcovr (version 4.2 or higher)"],
+    }
+
+    # First check the presence of a valid build
+    if not (os.path.exists(build_dir)):
+        raise click.ClickException(
+            f"`{build_dir}` folder not found, cannot generate coverage reports. "
+            "Generate coverage artefacts by running `spin test --gcov`"
+        )
+
+    debug_files = Path(build_dir).rglob("*.gcno")
+    if len(list(debug_files)) == 0:
+        raise click.ClickException(
+            "Debug build not found, cannot generate coverage reports.\n\n"
+            "Please rebuild using `spin build --clean --gcov` first."
+        )
+
+    # Verify the tools are installed prior to the build
+    p = _run(["ninja", "-C", build_dir, "-t", "targets", "all"], output=False)
+    if f"coverage-{coverage_type.value}" not in p.stdout.decode("ascii"):
+        raise click.ClickException(
+            f"coverage-{coverage_type.value} is not supported... "
+            f"Ensure the following are installed: {', '.join(requirements[coverage_type])} "
+            "and rerun `spin test --gcov`"
+        )
+
+
 @click.command()
 @click.option("-j", "--jobs", help="Number of parallel tasks to launch", type=int)
 @click.option("--clean", is_flag=True, help="Clean build directory before build")
 @click.option(
     "-v", "--verbose", is_flag=True, help="Print detailed build and installation output"
 )
+@click.option(
+    "--gcov",
+    is_flag=True,
+    help="Enable C code coverage using `gcov`. Use `spin test --gcov` to generate reports.",
+)
 @click.argument("meson_args", nargs=-1)
-def build(meson_args, jobs=None, clean=False, verbose=False, quiet=False):
+def build(meson_args, jobs=None, clean=False, verbose=False, gcov=False, quiet=False):
     """🔧 Build package with Meson/ninja and install
 
     MESON_ARGS are passed through e.g.:
 
       spin build -- -Dpkg_config_path=/lib64/pkgconfig
 
     The package is installed to build-install
@@ -124,16 +247,30 @@
 
       spin build -- -Dbuildtype=debug
 
     or set CFLAGS appropriately:
 
       CFLAGS="-O0 -g" spin build
     """
-    build_dir = "build"
-    setup_cmd = _meson_cli() + ["setup", build_dir, "--prefix=/usr"] + list(meson_args)
+    cfg = get_config()
+    distname = cfg.get("project.name", None)
+    if distname and _is_editable_install_of_same_source(distname):
+        if not quiet:
+            click.secho(
+                "Editable install of same source detected; skipping build",
+                fg="bright_red",
+            )
+        return
+
+    meson_args = list(meson_args)
+
+    if gcov:
+        meson_args = meson_args + ["-Db_coverage=true"]
+
+    setup_cmd = _meson_cli() + ["setup", build_dir, "--prefix=/usr"] + meson_args
 
     if clean:
         print(f"Removing `{build_dir}`")
         if os.path.isdir(build_dir):
             shutil.rmtree(build_dir)
         print(f"Removing `{install_dir}`")
         if os.path.isdir(install_dir):
@@ -145,15 +282,17 @@
             raise RuntimeError(
                 "Meson configuration failed; please try `spin build` again with the `--clean` flag."
             )
     else:
         # Build dir has been configured; check if it was configured by
         # current version of Meson
 
-        if _meson_version() != _meson_version_configured():
+        if (_meson_version() != _meson_version_configured()) or (
+            gcov and not _meson_coverage_configured()
+        ):
             _run(setup_cmd + ["--reconfigure"], output=not quiet)
 
         # Any other conditions that warrant a reconfigure?
 
     compile_flags = ["-v"] if verbose else []
     p = _run(
         _meson_cli() + ["compile"] + compile_flags + ["-C", build_dir],
@@ -209,18 +348,38 @@
     ),
 )
 @click.option("--verbose", "-v", is_flag=True, default=False)
 @click.option(
     "-c",
     "--coverage",
     is_flag=True,
-    help="Generate a coverage report of executed tests. An HTML copy of the report is written to `build/coverage`.",
+    help="Generate a Python coverage report of executed tests. An HTML copy of the report is written to `build/coverage`.",
+)
+@click.option(
+    "--gcov",
+    is_flag=True,
+    help="Generate a C coverage report in `build/meson-logs/coveragereport`.",
+)
+@click.option(
+    "--gcov-format",
+    type=click.Choice(GcovReportFormat),
+    default="html",
+    help=f"Format of the gcov report. Can be one of {', '.join(e.value for e in GcovReportFormat)}.",
 )
 @click.pass_context
-def test(ctx, pytest_args, n_jobs, tests, verbose, coverage=False):
+def test(
+    ctx,
+    pytest_args,
+    n_jobs,
+    tests,
+    verbose,
+    coverage=False,
+    gcov=None,
+    gcov_format=None,
+):
     """🔧 Run tests
 
     PYTEST_ARGS are passed through directly to pytest, e.g.:
 
       spin test -- --pdb
 
     To run tests on a directory or file:
@@ -249,35 +408,49 @@
       spin test -- -m slow
       spin test -- -m "not slow"
 
     If python-xdist is installed, you can run tests in parallel:
 
       spin test -j auto
 
+    To run a test inside of LLDB:
+
+      spin lldb -- python -mspin test ...
+
     For more, see `pytest --help`.
     """  # noqa: E501
     cfg = get_config()
+    distname = cfg.get("project.name", None)
+
+    if gcov and distname and _is_editable_install_of_same_source(distname):
+        click.secho(
+            "Error: cannot generate coverage report for editable installs",
+            fg="bright_red",
+        )
+        raise SystemExit(-1)
 
     build_cmd = _get_configured_command("build")
     if build_cmd:
         click.secho(
             "Invoking `build` prior to running tests:", bold=True, fg="bright_green"
         )
-        ctx.invoke(build_cmd)
+        ctx.invoke(build_cmd, gcov=bool(gcov))
 
     package = cfg.get("tool.spin.package", None)
     if (not pytest_args) and (not tests):
         pytest_args = (package,)
         if pytest_args == (None,):
             print(
                 "Please specify `package = packagename` under `tool.spin` section of `pyproject.toml`"
             )
             sys.exit(1)
 
     site_path = _set_pythonpath()
+    if site_path:
+        print(f'$ export PYTHONPATH="{site_path}"')
 
     # Sanity check that library built properly
     #
     # We do this because `pytest` swallows exception messages originating from `conftest.py`.
     # This can sometimes suppress useful information raised by the package on init.
     if sys.version_info[:2] >= (3, 11):
         p = _run([sys.executable, "-P", "-c", f"import {package}"], sys_exit=False)
@@ -309,20 +482,62 @@
         pytest_args = [
             *pytest_args,
             "--cov-report=term",
             f"--cov-report=html:{coverage_dir}",
             f"--cov={package}",
         ]
 
-    print(f'$ export PYTHONPATH="{site_path}"')
-    _run(
-        [sys.executable, "-m", "pytest", f"--rootdir={site_path}"] + list(pytest_args),
+    if sys.version_info[:2] >= (3, 11):
+        cmd = [sys.executable, "-P", "-m", "pytest"]
+    else:
+        cmd = ["pytest"]
+
+    cwd = os.getcwd()
+    pytest_p = _run(
+        cmd + ([f"--rootdir={site_path}"] if site_path else []) + list(pytest_args),
         cwd=site_path,
-        replace=True,
     )
+    os.chdir(cwd)
+
+    if gcov:
+        # Verify the tools are present
+        click.secho(
+            "Verifying gcov dependencies...",
+            bold=True,
+            fg="bright_yellow",
+        )
+        _check_coverage_tool_installation(gcov_format)
+
+        # Generate report
+        click.secho(
+            f"Generating {gcov_format.value} coverage report...",
+            bold=True,
+            fg="bright_yellow",
+        )
+        p = _run(
+            [
+                "ninja",
+                "-C",
+                build_dir,
+                f"coverage-{gcov_format.value.lower()}",
+            ],
+            output=False,
+        )
+        coverage_folder = click.style(
+            re.search(r"file://(.*)", p.stdout.decode("utf-8")).group(1),
+            bold=True,
+            fg="bright_yellow",
+        )
+        click.secho(
+            f"Coverage report generated successfully and written to {coverage_folder}",
+            bold=True,
+            fg="bright_green",
+        )
+
+    raise SystemExit(pytest_p.returncode)
 
 
 @click.command()
 @click.option("--code", "-c", help="Python program passed in as a string")
 @click.argument("gdb_args", nargs=-1)
 @click.pass_context
 def gdb(ctx, code, gdb_args):
@@ -388,15 +603,16 @@
     if build_cmd:
         click.secho(
             "Invoking `build` prior to invoking ipython:", bold=True, fg="bright_green"
         )
         ctx.invoke(build_cmd)
 
     p = _set_pythonpath()
-    print(f'💻 Launching IPython with PYTHONPATH="{p}"')
+    if p:
+        print(f'💻 Launching IPython with PYTHONPATH="{p}"')
     _run(["ipython", "--ignore-cwd"] + list(ipython_args), replace=True)
 
 
 @click.command()
 @click.argument("shell_args", nargs=-1)
 @click.pass_context
 def shell(ctx, shell_args=[]):
@@ -413,17 +629,19 @@
     if build_cmd:
         click.secho(
             "Invoking `build` prior to invoking shell:", bold=True, fg="bright_green"
         )
         ctx.invoke(build_cmd)
 
     p = _set_pythonpath()
+    if p:
+        print(f'💻 Launching shell with PYTHONPATH="{p}"')
+
     shell = os.environ.get("SHELL", "sh")
     cmd = [shell] + list(shell_args)
-    print(f'💻 Launching shell with PYTHONPATH="{p}"')
     print("⚠  Change directory to avoid importing source instead of built package")
     print("⚠  Ensure that your ~/.shellrc does not unset PYTHONPATH")
     _run(cmd, replace=True)
 
 
 @click.command()
 @click.argument("python_args", nargs=-1)
@@ -439,14 +657,17 @@
     if build_cmd:
         click.secho(
             "Invoking `build` prior to invoking Python:", bold=True, fg="bright_green"
         )
         ctx.invoke(build_cmd)
 
     p = _set_pythonpath()
+    if p:
+        print(f'🐍 Launching Python with PYTHONPATH="{p}"')
+
     v = sys.version_info
     if (v.major < 3) or (v.major == 3 and v.minor < 11):
         print("We're sorry, but this feature only works on Python 3.11 and greater 😢")
         print()
         print(
             "Why? Because we need the '-P' flag so the interpreter doesn't muck with PYTHONPATH"
         )
@@ -456,17 +677,15 @@
         print(f"  PYTHONPATH='{p}' python")
         print()
         print("And then call:")
         print()
         print("import sys; del(sys.path[0])")
         sys.exit(-1)
 
-    print(f'🐍 Launching Python with PYTHONPATH="{p}"')
-
-    _run(["/usr/bin/env", "python", "-P"] + list(python_args), replace=True)
+    _run([sys.executable, "-P"] + list(python_args), replace=True)
 
 
 @click.command(context_settings={"ignore_unknown_options": True})
 @click.argument("args", nargs=-1)
 @click.pass_context
 def run(ctx, args):
     """🏁 Run a shell command with PYTHONPATH set
@@ -492,23 +711,36 @@
         # Redirect spin generated output
         with contextlib.redirect_stdout(sys.stderr):
             # Also ask build to be quiet
             ctx.invoke(build_cmd, quiet=True)
 
     is_posix = sys.platform in ("linux", "darwin")
     shell = len(args) == 1
+    cmd_args = copy.copy(args)
     if shell:
-        args = args[0]
-
-    if shell and not is_posix:
-        # On Windows, we're going to try to use bash
-        args = ["bash", "-c", args]
+        cmd_args = args[0]
+        if not is_posix:
+            # On Windows, we're going to try to use bash
+            cmd_args = ["bash", "-c", cmd_args]
 
     _set_pythonpath(quiet=True)
-    _run(args, echo=False, shell=shell)
+    p = _run(cmd_args, echo=False, shell=shell, sys_exit=False)
+
+    # Is the user trying to run a Python script, without calling the Python interpreter?
+    executable = args[0]
+    if (
+        (p.returncode != 0)
+        and args[0].endswith(".py")
+        and os.path.exists(executable)
+        and (not os.access(executable, os.X_OK))
+    ):
+        click.secho(
+            f"Did you mean to call `spin run python {' '.join(args)}`?", fg="bright_red"
+        )
+    sys.exit(p.returncode)
 
 
 @click.command()
 @click.argument("sphinx_target", default="html")
 @click.option(
     "--clean",
     is_flag=True,
@@ -558,23 +790,23 @@
     if sphinx_target in ("targets", "help"):
         clean = False
         first_build = False
         sphinx_target = "help"
 
     if clean:
         doc_dirs = [
-            "./doc/build/",
-            "./doc/source/api/",
-            "./doc/source/auto_examples/",
-            "./doc/source/jupyterlite_contents/",
+            f"./{doc_dir}/build/",
+            f"./{doc_dir}/source/api/",
+            f"./{doc_dir}/source/auto_examples/",
+            f"./{doc_dir}/source/jupyterlite_contents/",
         ]
-        for doc_dir in doc_dirs:
-            if os.path.isdir(doc_dir):
-                print(f"Removing {doc_dir!r}")
-                shutil.rmtree(doc_dir)
+        for target_dir in doc_dirs:
+            if os.path.isdir(target_dir):
+                print(f"Removing {target_dir!r}")
+                shutil.rmtree(target_dir)
 
     build_cmd = _get_configured_command("build")
 
     if build_cmd and first_build:
         click.secho(
             "Invoking `build` prior to building docs:", bold=True, fg="bright_green"
         )
@@ -592,19 +824,24 @@
 
     os.environ["SPHINXOPTS"] = f"{opts} -j {jobs}"
 
     click.secho(
         f"$ export SPHINXOPTS={os.environ['SPHINXOPTS']}", bold=True, fg="bright_blue"
     )
 
-    os.environ["PYTHONPATH"] = f'{site_path}{os.sep}:{os.environ.get("PYTHONPATH", "")}'
-    click.secho(
-        f"$ export PYTHONPATH={os.environ['PYTHONPATH']}", bold=True, fg="bright_blue"
-    )
-    _run(["make", "-C", "doc", sphinx_target], replace=True)
+    if site_path:
+        os.environ["PYTHONPATH"] = (
+            f'{site_path}{os.sep}:{os.environ.get("PYTHONPATH", "")}'
+        )
+        click.secho(
+            f"$ export PYTHONPATH={os.environ['PYTHONPATH']}",
+            bold=True,
+            fg="bright_blue",
+        )
+    _run(["make", "-C", doc_dir, sphinx_target], replace=True)
 
 
 @click.command()
 @click.option("--code", "-c", help="Python program passed in as a string")
 @click.argument("lldb_args", nargs=-1)
 @click.pass_context
 def lldb(ctx, code, lldb_args):
```

### Comparing `spin-0.8/spin/cmds/pip.py` & `spin-0.9/spin/cmds/pip.py`

 * *Files identical despite different names*

### Comparing `spin-0.8/spin/cmds/util.py` & `spin-0.9/spin/cmds/util.py`

 * *Files identical despite different names*

### Comparing `spin-0.8/spin/color_format.py` & `spin-0.9/spin/color_format.py`

 * *Files identical despite different names*

### Comparing `spin-0.8/spin/containers.py` & `spin-0.9/spin/containers.py`

 * *Files identical despite different names*

### Comparing `spin-0.8/spin/sectioned_help.py` & `spin-0.9/spin/sectioned_help.py`

 * *Files identical despite different names*

### Comparing `spin-0.8/spin/tests/test_meson.py` & `spin-0.9/spin/tests/test_meson.py`

 * *Files identical despite different names*

### Comparing `spin-0.8/spin.egg-info/PKG-INFO` & `spin-0.9/spin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: spin
-Version: 0.8
+Version: 0.9
 Summary: Developer tool for scientific Python libraries
 Maintainer-email: Scientific Python <spin@discuss.scientific-python.org>
 License: BSD 3-Clause License
         
-        Copyright (c) 2021--2022, Scientific Python project
+        Copyright (c) 2021--2024, Scientific Python project
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
@@ -49,32 +49,36 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: tomli; python_version < "3.11"
 Requires-Dist: colorama; platform_system == "Windows"
+Requires-Dist: importlib_metadata>=7
 Provides-Extra: lint
-Requires-Dist: pre-commit==3.5.0; extra == "lint"
+Requires-Dist: pre-commit==3.7.0; extra == "lint"
 Provides-Extra: dev
-Requires-Dist: changelist==0.4; extra == "dev"
+Requires-Dist: changelist==0.5; extra == "dev"
 
 # 💫 Scientific Python INcantations (`spin`)
 
 ## A developer tool for scientific Python libraries
 
 Developers need to memorize a whole bunch of magic command-line incantations.
-And these incantations change from time to time!
-Typically, their lives are made simpler by a Makefile, but Makefiles can be convoluted, are not written in Python, and are hard to extend.
-The rationale behind `spin` is therefore to provide a simple interface for common development tasks.
+These incantations may also change over time.
+Often, Makefiles are used to provide aliases, but Makefiles can be convoluted, are not written in Python, and are hard to extend.
+The goal of `spin` is therefore to provide a simple, user-friendly, extendable interface for common development tasks.
 It comes with a few common build commands out the box, but can easily be customized per project.
 
 As a curiosity: the impetus behind developing the tool was the mass migration of scientific Python libraries (SciPy, scikit-image, and NumPy, etc.) to Meson, after distutils was deprecated.
 When many of the build and installation commands changed, it made sense to abstract away the nuisance of having to re-learn them.
 
+_Note:_ We now have experimental builds for editable installs.
+Most of the Meson commands listed below should work "out of the box" for those.
+
 ## Installation
 
 ```
 pip install spin
 ```
 
 ## Configuration
@@ -148,15 +152,14 @@
   python   🐍 Launch Python shell with PYTHONPATH set
   shell    💻 Launch shell with PYTHONPATH set
   test     🔧 Run pytest
   run      🏁 Run a shell command with PYTHONPATH set
   docs     📖 Build Sphinx documentation
   gdb      👾 Execute a Python snippet with GDB
   lldb     👾 Execute a Python snippet with LLDB
-  install  💽 Build and install package using pip.
 ```
 
 ### [Build](https://pypa-build.readthedocs.io/en/stable/) (PEP 517 builder)
 
 Available as `spin.cmds.build.*`:
 
 ```
@@ -203,14 +206,37 @@
 @click.command()
 def example():
     """Command that accesses `pyproject.toml` configuration"""
     config = util.get_config()
     print(config["tool.spin"])
 ```
 
+### Argument overrides
+
+Default arguments can be overridden for any command.
+The custom command above, e.g., has the following signature:
+
+```python
+@click.command()
+@click.option("-f", "--flag")
+@click.option("-t", "--test", default="not set")
+def example(flag, test, default_kwd=None):
+    """🧪 Example custom command.
+    ...
+    """
+```
+
+Use the `[tool.spin.kwargs]` section to override default values for
+click options or function keywords:
+
+```toml
+[tool.spin.kwargs]
+".spin/cmds.py:example" = {"test" = "default override", "default_kwd" = 3}
+```
+
 ### Advanced: adding arguments to built-in commands
 
 Instead of rewriting a command from scratch, a project may want to add a flag to a built-in `spin` command, or perhaps do some pre- or post-processing.
 For this, we have to use an internal Click concept called a [context](https://click.palletsprojects.com/en/8.1.x/complex/#contexts).
 Fortunately, we don't need to know anything about contexts other than that they allow us to execute commands within commands.
 
 We proceed by duplicating the function header of the existing command, and adding our own flag:
@@ -280,15 +306,15 @@
 
 ## For contributors
 
 `spin` development happens on GitHub at [scientific-python/spin](https://github.com/scientific-python/spin).
 `spin` tests are invoked using:
 
 ```
-nox -s tests
+nox -s test
 ```
 
 ## History
 
 The `dev.py` tool was [proposed for SciPy](https://github.com/scipy/scipy/issues/15489) by Ralf Gommers and [implemented](https://github.com/scipy/scipy/pull/15959) by Sayantika Banik, Eduardo Naufel Schettino, and Ralf Gommers (also see [Sayantika's blog post](https://labs.quansight.org/blog/the-evolution-of-the-scipy-developer-cli)).
 Inspired by that implementation, `spin` (this package) is a minimal rewrite by Stéfan van der Walt, that aims to be easily extendable so that it can be used across ecosystem libraries.
 We thank Danila Bredikhin and Luca Marconato who kindly donated the `spin` name on PyPi.
```

