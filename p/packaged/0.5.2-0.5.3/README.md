# Comparing `tmp/packaged-0.5.2.tar.gz` & `tmp/packaged-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaged-0.5.2.tar", last modified: Tue May 21 21:28:39 2024, max compression
+gzip compressed data, was "packaged-0.5.3.tar", last modified: Fri May 24 13:49:58 2024, max compression
```

## Comparing `packaged-0.5.2.tar` & `packaged-0.5.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-21 21:28:39.452284 packaged-0.5.2/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)    18089 2024-05-14 12:10:36.000000 packaged-0.5.2/LICENSE
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     5129 2024-05-21 21:28:39.452216 packaged-0.5.2/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3849 2024-05-21 17:24:55.000000 packaged-0.5.2/README.md
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1357 2024-05-21 21:28:39.452666 packaged-0.5.2/setup.cfg
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-09 19:00:34.000000 packaged-0.5.2/setup.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-21 21:28:39.447801 packaged-0.5.2/src/
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-21 21:28:39.450467 packaged-0.5.2/src/packaged/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     7863 2024-05-21 20:19:07.000000 packaged-0.5.2/src/packaged/__init__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.5.2/src/packaged/__main__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2722 2024-05-21 20:18:41.000000 packaged-0.5.2/src/packaged/cli.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1610 2024-05-21 20:18:41.000000 packaged-0.5.2/src/packaged/config.py
--rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    19207 2024-05-14 12:16:01.000000 packaged-0.5.2/src/packaged/makeself-header.sh
--rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    21228 2024-05-13 10:09:30.000000 packaged-0.5.2/src/packaged/makeself.sh
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.5.2/src/packaged/py.typed
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-21 21:28:39.451614 packaged-0.5.2/src/packaged.egg-info/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     5129 2024-05-21 21:28:39.000000 packaged-0.5.2/src/packaged.egg-info/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      426 2024-05-21 21:28:39.000000 packaged-0.5.2/src/packaged.egg-info/SOURCES.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-21 21:28:39.000000 packaged-0.5.2/src/packaged.egg-info/dependency_links.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-21 21:28:39.000000 packaged-0.5.2/src/packaged.egg-info/entry_points.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      119 2024-05-21 21:28:39.000000 packaged-0.5.2/src/packaged.egg-info/requires.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-21 21:28:39.000000 packaged-0.5.2/src/packaged.egg-info/top_level.txt
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-24 13:49:58.772621 packaged-0.5.3/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)    18089 2024-05-14 12:10:36.000000 packaged-0.5.3/LICENSE
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     5124 2024-05-24 13:49:58.772548 packaged-0.5.3/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3844 2024-05-24 13:26:37.000000 packaged-0.5.3/README.md
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1357 2024-05-24 13:49:58.772923 packaged-0.5.3/setup.cfg
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-09 19:00:34.000000 packaged-0.5.3/setup.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-24 13:49:58.768471 packaged-0.5.3/src/
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-24 13:49:58.771117 packaged-0.5.3/src/packaged/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     8045 2024-05-23 20:53:13.000000 packaged-0.5.3/src/packaged/__init__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.5.3/src/packaged/__main__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3013 2024-05-23 20:53:13.000000 packaged-0.5.3/src/packaged/cli.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1610 2024-05-21 20:18:41.000000 packaged-0.5.3/src/packaged/config.py
+-rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    19207 2024-05-14 12:16:01.000000 packaged-0.5.3/src/packaged/makeself-header.sh
+-rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    21228 2024-05-13 10:09:30.000000 packaged-0.5.3/src/packaged/makeself.sh
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.5.3/src/packaged/py.typed
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-24 13:49:58.772024 packaged-0.5.3/src/packaged.egg-info/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     5124 2024-05-24 13:49:58.000000 packaged-0.5.3/src/packaged.egg-info/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      426 2024-05-24 13:49:58.000000 packaged-0.5.3/src/packaged.egg-info/SOURCES.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-24 13:49:58.000000 packaged-0.5.3/src/packaged.egg-info/dependency_links.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-24 13:49:58.000000 packaged-0.5.3/src/packaged.egg-info/entry_points.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      119 2024-05-24 13:49:58.000000 packaged-0.5.3/src/packaged.egg-info/requires.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-24 13:49:58.000000 packaged-0.5.3/src/packaged.egg-info/top_level.txt
```

### Comparing `packaged-0.5.2/LICENSE` & `packaged-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `packaged-0.5.2/PKG-INFO` & `packaged-0.5.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaged
-Version: 0.5.2
+Version: 0.5.3
 Summary: The easiest way to ship python applications.
 Home-page: https://github.com/tusharsadhwani/packaged
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: GPL-2.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -53,32 +53,32 @@
 ```bash
 packaged <output_path> <build_command> <startup_command> [<source_directory>]
 ```
 
 Such as:
 
 ```bash
-packaged my_project.bin 'pip install .' 'python -m your_package' path/to/project
+packaged my_project.sh 'pip install .' 'python -m your_package' path/to/project
 ```
 
 ## Examples
 
 All examples below create a self contained executable. You can send the produced
 binary file to another machine with the same OS and architecture, and it will
 run the same.
 
 You can also find the pre-built binaries on the [Releases page](https://github.com/tusharsadhwani/packaged/releases/latest).
 
 ### Mandelbrot (`numpy`, `matplotlib`, GUI)
 
 ```bash
-packaged ./mandelbrot.bin 'pip install -r requirements.txt' 'python mandelbrot.py' ./example/mandelbrot
+packaged ./mandelbrot.sh 'pip install -r requirements.txt' 'python mandelbrot.py' ./example/mandelbrot
 ```
 
-This produces a `./mandelbrot.bin` binary with:
+This produces a `./mandelbrot.sh` binary with:
 
 - Python 3.12
 - `matplotlib`
 - `numba`
 - `llvmlite`
 - `pillow`
 
@@ -94,25 +94,25 @@
 ```
 
 [This configuration](https://github.com/tusharsadhwani/packaged/blob/main/example/minesweeper/packaged.toml)
 is used for building the package. The equivalent command to build the project
 without `pyproject.toml` would be:
 
 ```bash
-packaged minesweeper.bin 'pip install .' 'python -m minesweeper' ./example/minesweeper
+packaged minesweeper.sh 'pip install .' 'python -m minesweeper' ./example/minesweeper
 ```
 
 ### Textual (TUI) Demo
 
 Since the dependencies themselves contain all the source code needed, you can
 skip the last argument. With this, no other files will be packaged other than
 what is produced in the build step.
 
 ```bash
-packaged ./textual.bin 'pip install textual' 'python -m textual'
+packaged ./textual.sh 'pip install textual' 'python -m textual'
 ```
 
 This will simply package the `textual` library's own demo into a single file.
 
 ### Aliens (pygame)
 
 Pygame ships with various games as well, `pygame.examples.aliens` is one of them:
```

### Comparing `packaged-0.5.2/README.md` & `packaged-0.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,32 +20,32 @@
 ```bash
 packaged <output_path> <build_command> <startup_command> [<source_directory>]
 ```
 
 Such as:
 
 ```bash
-packaged my_project.bin 'pip install .' 'python -m your_package' path/to/project
+packaged my_project.sh 'pip install .' 'python -m your_package' path/to/project
 ```
 
 ## Examples
 
 All examples below create a self contained executable. You can send the produced
 binary file to another machine with the same OS and architecture, and it will
 run the same.
 
 You can also find the pre-built binaries on the [Releases page](https://github.com/tusharsadhwani/packaged/releases/latest).
 
 ### Mandelbrot (`numpy`, `matplotlib`, GUI)
 
 ```bash
-packaged ./mandelbrot.bin 'pip install -r requirements.txt' 'python mandelbrot.py' ./example/mandelbrot
+packaged ./mandelbrot.sh 'pip install -r requirements.txt' 'python mandelbrot.py' ./example/mandelbrot
 ```
 
-This produces a `./mandelbrot.bin` binary with:
+This produces a `./mandelbrot.sh` binary with:
 
 - Python 3.12
 - `matplotlib`
 - `numba`
 - `llvmlite`
 - `pillow`
 
@@ -61,25 +61,25 @@
 ```
 
 [This configuration](https://github.com/tusharsadhwani/packaged/blob/main/example/minesweeper/packaged.toml)
 is used for building the package. The equivalent command to build the project
 without `pyproject.toml` would be:
 
 ```bash
-packaged minesweeper.bin 'pip install .' 'python -m minesweeper' ./example/minesweeper
+packaged minesweeper.sh 'pip install .' 'python -m minesweeper' ./example/minesweeper
 ```
 
 ### Textual (TUI) Demo
 
 Since the dependencies themselves contain all the source code needed, you can
 skip the last argument. With this, no other files will be packaged other than
 what is produced in the build step.
 
 ```bash
-packaged ./textual.bin 'pip install textual' 'python -m textual'
+packaged ./textual.sh 'pip install textual' 'python -m textual'
 ```
 
 This will simply package the `textual` library's own demo into a single file.
 
 ### Aliens (pygame)
 
 Pygame ships with various games as well, `pygame.examples.aliens` is one of them:
```

### Comparing `packaged-0.5.2/setup.cfg` & `packaged-0.5.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = packaged
-version = 0.5.2
+version = 0.5.3
 description = The easiest way to ship python applications.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tusharsadhwani/packaged
 author = Tushar Sadhwani
 author_email = tushar.sadhwani000@gmail.com
 license = GPL-2.0-or-later
```

### Comparing `packaged-0.5.2/src/packaged/__init__.py` & `packaged-0.5.3/src/packaged/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,30 @@
     """Raised when the Python version asked for is not available for download."""
 
     def __init__(self, python_version: str) -> None:
         super().__init__(python_version)
         self.python_version = python_version
 
 
+class OutputPathExists(Exception):
+    """Raised when the output path already exists."""
+
+
 def create_package(
     source_directory: str | None,
     output_path: str,
     build_command: str,
     startup_command: str,
     python_version: str,
     quiet: bool = False,
 ) -> None:
     """Create the makeself executable, with the startup script in it."""
+    if os.path.exists(output_path):
+        raise OutputPathExists
+
     if source_directory is None:
         source_directory = tempfile.mkdtemp()
 
     if not os.path.isdir(source_directory):
         raise SourceDirectoryNotFound(source_directory)
 
     startup_script_name = "_packaged_startup.sh"
@@ -181,19 +188,20 @@
         except subprocess.CalledProcessError as exc:
             spinner.stop()
             print("*** Makeself Failed:", file=sys.stderr)
             print("Stdout:\n" + exc.stdout.decode(errors="ignore"), file=sys.stderr)
             print("Stderr:\n" + exc.stdout.decode(errors="ignore"), file=sys.stderr)
             raise
 
-    finally:
         spinner.stop()
         if not quiet:
             print(f"Package {output_path!r} built successfully!")
 
+    finally:
+        spinner.stop()
         # Cleanup the packaged python and startup script from source directory
         if os.path.exists(startup_script_path):
             os.remove(startup_script_path)
         if os.path.exists(packaged_python_path):
             shutil.rmtree(packaged_python_path)
```

### Comparing `packaged-0.5.2/src/packaged/cli.py` & `packaged-0.5.3/src/packaged/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 import argparse
 import os.path
 import platform
 import sys
 
 from packaged import (
     DEFAULT_PYTHON_VERSION,
+    OutputPathExists,
     PythonNotAvailable,
     SourceDirectoryNotFound,
     create_package,
 )
 from packaged.config import (
     Config,
     ConfigValidationError,
     config_file_exists,
     parse_config,
 )
 
 
 def error(message: str) -> None:
     """Print error message"""
-    print(f"\033[1;31mError:\033[m {message}")
+    print(f"\033[1;31mError:\033[m {message}", file=sys.stderr)
 
 
 def cli(argv: list[str] | None = None) -> int:
     """CLI interface."""
     # Manually set argv from sys.argv, as we need to check its length to
     # choose to parse config instead.
     if argv is None:
@@ -87,9 +88,15 @@
         )
     except SourceDirectoryNotFound as exc:
         error(f"Folder {exc.directory_path!r} does not exist.")
         return 4
     except PythonNotAvailable as exc:
         error(f"Python {exc.python_version!r} is not available for download.")
         return 5
+    except OutputPathExists:
+        err_msg = f"output path {config.output_path!r} already exists"
+        if config.output_path == ".":
+            err_msg += "\nConsider giving a filename, like './myapp.bin'"
+        error(err_msg)
+        return 6
 
     return 0
```

### Comparing `packaged-0.5.2/src/packaged/config.py` & `packaged-0.5.3/src/packaged/config.py`

 * *Files identical despite different names*

### Comparing `packaged-0.5.2/src/packaged/makeself-header.sh` & `packaged-0.5.3/src/packaged/makeself-header.sh`

 * *Files identical despite different names*

### Comparing `packaged-0.5.2/src/packaged/makeself.sh` & `packaged-0.5.3/src/packaged/makeself.sh`

 * *Files identical despite different names*

### Comparing `packaged-0.5.2/src/packaged.egg-info/PKG-INFO` & `packaged-0.5.3/src/packaged.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaged
-Version: 0.5.2
+Version: 0.5.3
 Summary: The easiest way to ship python applications.
 Home-page: https://github.com/tusharsadhwani/packaged
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: GPL-2.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -53,32 +53,32 @@
 ```bash
 packaged <output_path> <build_command> <startup_command> [<source_directory>]
 ```
 
 Such as:
 
 ```bash
-packaged my_project.bin 'pip install .' 'python -m your_package' path/to/project
+packaged my_project.sh 'pip install .' 'python -m your_package' path/to/project
 ```
 
 ## Examples
 
 All examples below create a self contained executable. You can send the produced
 binary file to another machine with the same OS and architecture, and it will
 run the same.
 
 You can also find the pre-built binaries on the [Releases page](https://github.com/tusharsadhwani/packaged/releases/latest).
 
 ### Mandelbrot (`numpy`, `matplotlib`, GUI)
 
 ```bash
-packaged ./mandelbrot.bin 'pip install -r requirements.txt' 'python mandelbrot.py' ./example/mandelbrot
+packaged ./mandelbrot.sh 'pip install -r requirements.txt' 'python mandelbrot.py' ./example/mandelbrot
 ```
 
-This produces a `./mandelbrot.bin` binary with:
+This produces a `./mandelbrot.sh` binary with:
 
 - Python 3.12
 - `matplotlib`
 - `numba`
 - `llvmlite`
 - `pillow`
 
@@ -94,25 +94,25 @@
 ```
 
 [This configuration](https://github.com/tusharsadhwani/packaged/blob/main/example/minesweeper/packaged.toml)
 is used for building the package. The equivalent command to build the project
 without `pyproject.toml` would be:
 
 ```bash
-packaged minesweeper.bin 'pip install .' 'python -m minesweeper' ./example/minesweeper
+packaged minesweeper.sh 'pip install .' 'python -m minesweeper' ./example/minesweeper
 ```
 
 ### Textual (TUI) Demo
 
 Since the dependencies themselves contain all the source code needed, you can
 skip the last argument. With this, no other files will be packaged other than
 what is produced in the build step.
 
 ```bash
-packaged ./textual.bin 'pip install textual' 'python -m textual'
+packaged ./textual.sh 'pip install textual' 'python -m textual'
 ```
 
 This will simply package the `textual` library's own demo into a single file.
 
 ### Aliens (pygame)
 
 Pygame ships with various games as well, `pygame.examples.aliens` is one of them:
```

