# Comparing `tmp/sitk-cli-0.6.0.tar.gz` & `tmp/sitk_cli-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitk-cli-0.6.0.tar", last modified: Thu Aug 10 07:56:23 2023, max compression
+gzip compressed data, was "sitk_cli-0.7.0.tar", last modified: Fri May 24 11:20:41 2024, max compression
```

## Comparing `sitk-cli-0.6.0.tar` & `sitk_cli-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 lloyd      (501) staff       (20)        0 2023-08-10 07:56:23.784360 sitk-cli-0.6.0/
--rw-r--r--   0 lloyd      (501) staff       (20)     1067 2023-06-27 06:39:35.000000 sitk-cli-0.6.0/LICENSE
--rw-r--r--   0 lloyd      (501) staff       (20)     1959 2023-08-10 07:56:23.784450 sitk-cli-0.6.0/PKG-INFO
--rw-------   0 lloyd      (501) staff       (20)     1577 2023-08-10 07:06:49.000000 sitk-cli-0.6.0/README.md
--rw-r--r--   0 lloyd      (501) staff       (20)       82 2023-06-27 06:39:35.000000 sitk-cli-0.6.0/pyproject.toml
--rw-r--r--   0 lloyd      (501) staff       (20)      837 2023-08-10 07:56:23.784751 sitk-cli-0.6.0/setup.cfg
--rw-r--r--   0 lloyd      (501) staff       (20)       83 2023-06-27 06:39:35.000000 sitk-cli-0.6.0/setup.py
-drwxr-xr-x   0 lloyd      (501) staff       (20)        0 2023-08-10 07:56:23.780932 sitk-cli-0.6.0/src/
-drwxr-xr-x   0 lloyd      (501) staff       (20)        0 2023-08-10 07:56:23.782901 sitk-cli-0.6.0/src/sitk_cli/
--rw-r--r--   0 lloyd      (501) staff       (20)       88 2023-06-27 06:39:35.000000 sitk-cli-0.6.0/src/sitk_cli/__init__.py
--rw-r--r--   0 lloyd      (501) staff       (20)     3979 2023-08-10 07:55:48.000000 sitk-cli-0.6.0/src/sitk_cli/lib.py
-drwxr-xr-x   0 lloyd      (501) staff       (20)        0 2023-08-10 07:56:23.783521 sitk-cli-0.6.0/src/sitk_cli.egg-info/
--rw-r--r--   0 lloyd      (501) staff       (20)     1959 2023-08-10 07:56:23.000000 sitk-cli-0.6.0/src/sitk_cli.egg-info/PKG-INFO
--rw-r--r--   0 lloyd      (501) staff       (20)      353 2023-08-10 07:56:23.000000 sitk-cli-0.6.0/src/sitk_cli.egg-info/SOURCES.txt
--rw-r--r--   0 lloyd      (501) staff       (20)        1 2023-08-10 07:56:23.000000 sitk-cli-0.6.0/src/sitk_cli.egg-info/dependency_links.txt
--rw-r--r--   0 lloyd      (501) staff       (20)       43 2023-08-10 07:56:23.000000 sitk-cli-0.6.0/src/sitk_cli.egg-info/requires.txt
--rw-r--r--   0 lloyd      (501) staff       (20)        9 2023-08-10 07:56:23.000000 sitk-cli-0.6.0/src/sitk_cli.egg-info/top_level.txt
-drwxr-xr-x   0 lloyd      (501) staff       (20)        0 2023-08-10 07:56:23.784093 sitk-cli-0.6.0/tests/
--rw-r--r--   0 lloyd      (501) staff       (20)     2402 2023-08-10 07:05:07.000000 sitk-cli-0.6.0/tests/test_make_cli.py
--rw-r--r--   0 lloyd      (501) staff       (20)     1440 2023-08-10 07:55:48.000000 sitk-cli-0.6.0/tests/test_optional_args.py
--rw-r--r--   0 lloyd      (501) staff       (20)      697 2023-08-09 19:07:47.000000 sitk-cli-0.6.0/tests/test_register_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:20:41.490555 sitk_cli-0.7.0/
+-rw-rw-rw-   0        0        0     1088 2024-05-24 10:03:25.000000 sitk_cli-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0     2164 2024-05-24 11:20:41.490555 sitk_cli-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1622 2024-05-24 10:03:25.000000 sitk_cli-0.7.0/README.md
+-rw-rw-rw-   0        0        0       84 2024-05-24 10:03:25.000000 sitk_cli-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0      883 2024-05-24 11:20:41.492566 sitk_cli-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0       86 2024-05-24 10:03:25.000000 sitk_cli-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:20:41.472452 sitk_cli-0.7.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-24 11:20:41.472452 sitk_cli-0.7.0/src/sitk_cli/
+-rw-rw-rw-   0        0        0       91 2024-05-24 10:03:25.000000 sitk_cli-0.7.0/src/sitk_cli/__init__.py
+-rw-rw-rw-   0        0        0     4254 2024-05-24 10:25:07.000000 sitk_cli-0.7.0/src/sitk_cli/lib.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:20:41.489554 sitk_cli-0.7.0/src/sitk_cli.egg-info/
+-rw-rw-rw-   0        0        0     2164 2024-05-24 11:20:41.000000 sitk_cli-0.7.0/src/sitk_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2024-05-24 11:20:41.000000 sitk_cli-0.7.0/src/sitk_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 11:20:41.000000 sitk_cli-0.7.0/src/sitk_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-24 11:20:41.000000 sitk_cli-0.7.0/src/sitk_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-24 11:20:41.000000 sitk_cli-0.7.0/src/sitk_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 11:20:41.488554 sitk_cli-0.7.0/tests/
+-rw-rw-rw-   0        0        0     2480 2024-05-24 10:03:25.000000 sitk_cli-0.7.0/tests/test_make_cli.py
+-rw-rw-rw-   0        0        0     1489 2024-05-24 10:03:25.000000 sitk_cli-0.7.0/tests/test_optional_args.py
+-rw-rw-rw-   0        0        0      324 2024-05-24 10:20:05.000000 sitk_cli-0.7.0/tests/test_register_cli.py
```

### Comparing `sitk-cli-0.6.0/PKG-INFO` & `sitk_cli-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,62 @@
-Metadata-Version: 2.1
-Name: sitk-cli
-Version: 0.6.0
-Summary: Wrap SimpleITK functions as command lines
-Home-page: https://github.com/dyollb/sitk-cli
-License: MIT License
-Project-URL: Bug Tracker, https://github.com/dyollb/sitk-cli/issues
-Project-URL: Source Code, https://github.com/dyollb/sitk-cli
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# Wrap SimpleITK functions as command lines
-
-[![Build Actions Status](https://github.com/dyollb/segmantic/workflows/CI/badge.svg)](https://github.com/dyollb/sitk-cli/actions)
-[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://https://opensource.org/licenses/MIT)
-[![PyPI version](https://badge.fury.io/py/sitk-cli.svg)](https://badge.fury.io/py/sitk-cli)
-<img src="https://img.shields.io/pypi/dm/sitk-cli.svg?label=pypi%20downloads&logo=python&logoColor=green"/>
-
-## Overview
-
-Create [Typer](https://github.com/tiangolo/typer) command line interface from functions that use [SimpleITK](https://github.com/SimpleITK/SimpleITK) images (and transforms) as arguments or return type.
-
-```Python
-import SimpleITK as sitk
-import typer
-
-from sitk_cli import register_command
-
-app = typer.Typer()
-
-
-@register_command(app)
-def fill_holes_slice_by_slice(mask: sitk.Image) -> sitk.Image:
-    mask = mask != 0
-    output = sitk.Image(mask.GetSize(), mask.GetPixelID())
-    output.CopyInformation(mask)
-    for k in range(mask.GetSize()[2]):
-        output[:, :, k] = sitk.BinaryFillhole(mask[:, :, k], fullyConnected=False)
-    return output
-
-
-if __name__ == "__main__":
-    app()
-```
-
-To work, sitk-cli inspects the type annotations of the function and creates a wrapper function that loads images from file and passes these to the original function. Returned images (transforms) are written to a file by the wrapper function..
-
-## Installation
-
-```sh
-pip install sitk-cli
-```
-
-## Demo
-
-![Command lind demo](https://github.com/dyollb/sitk-cli/raw/main/docs/demo.gif)
+Metadata-Version: 2.1
+Name: sitk-cli
+Version: 0.7.0
+Summary: Wrap SimpleITK functions as command lines
+Home-page: https://github.com/dyollb/sitk-cli
+License: MIT License
+Project-URL: Bug Tracker, https://github.com/dyollb/sitk-cli/issues
+Project-URL: Source Code, https://github.com/dyollb/sitk-cli
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: makefun
+Requires-Dist: SimpleITK
+Requires-Dist: typer
+Provides-Extra: dev
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+
+# Wrap SimpleITK functions as command lines
+
+[![Build Actions Status](https://github.com/dyollb/segmantic/workflows/CI/badge.svg)](https://github.com/dyollb/sitk-cli/actions)
+[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/sitk-cli.svg)](https://badge.fury.io/py/sitk-cli)
+<img src="https://img.shields.io/pypi/dm/sitk-cli.svg?label=pypi%20downloads&logo=python&logoColor=green"/>
+
+## Overview
+
+Create [Typer](https://github.com/tiangolo/typer) command line interface from functions that use [SimpleITK](https://github.com/SimpleITK/SimpleITK) images (and transforms) as arguments or return type.
+
+```Python
+import SimpleITK as sitk
+import typer
+
+from sitk_cli import register_command
+
+app = typer.Typer()
+
+
+@register_command(app)
+def fill_holes_slice_by_slice(mask: sitk.Image) -> sitk.Image:
+    mask = mask != 0
+    output = sitk.Image(mask.GetSize(), mask.GetPixelID())
+    output.CopyInformation(mask)
+    for k in range(mask.GetSize()[2]):
+        output[:, :, k] = sitk.BinaryFillhole(mask[:, :, k], fullyConnected=False)
+    return output
+
+
+if __name__ == "__main__":
+    app()
+```
+
+To work, sitk-cli inspects the type annotations of the function and creates a wrapper function that loads images from file and passes these to the original function. Returned images (transforms) are written to a file by the wrapper function..
+
+## Installation
+
+```sh
+pip install sitk-cli
+```
+
+## Demo
+
+![Command lind demo](https://github.com/dyollb/sitk-cli/raw/main/docs/demo.gif)
```

### Comparing `sitk-cli-0.6.0/README.md` & `sitk_cli-0.7.0/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-# Wrap SimpleITK functions as command lines
-
-[![Build Actions Status](https://github.com/dyollb/segmantic/workflows/CI/badge.svg)](https://github.com/dyollb/sitk-cli/actions)
-[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://https://opensource.org/licenses/MIT)
-[![PyPI version](https://badge.fury.io/py/sitk-cli.svg)](https://badge.fury.io/py/sitk-cli)
-<img src="https://img.shields.io/pypi/dm/sitk-cli.svg?label=pypi%20downloads&logo=python&logoColor=green"/>
-
-## Overview
-
-Create [Typer](https://github.com/tiangolo/typer) command line interface from functions that use [SimpleITK](https://github.com/SimpleITK/SimpleITK) images (and transforms) as arguments or return type.
-
-```Python
-import SimpleITK as sitk
-import typer
-
-from sitk_cli import register_command
-
-app = typer.Typer()
-
-
-@register_command(app)
-def fill_holes_slice_by_slice(mask: sitk.Image) -> sitk.Image:
-    mask = mask != 0
-    output = sitk.Image(mask.GetSize(), mask.GetPixelID())
-    output.CopyInformation(mask)
-    for k in range(mask.GetSize()[2]):
-        output[:, :, k] = sitk.BinaryFillhole(mask[:, :, k], fullyConnected=False)
-    return output
-
-
-if __name__ == "__main__":
-    app()
-```
-
-To work, sitk-cli inspects the type annotations of the function and creates a wrapper function that loads images from file and passes these to the original function. Returned images (transforms) are written to a file by the wrapper function..
-
-## Installation
-
-```sh
-pip install sitk-cli
-```
-
-## Demo
-
-![Command lind demo](https://github.com/dyollb/sitk-cli/raw/main/docs/demo.gif)
+# Wrap SimpleITK functions as command lines
+
+[![Build Actions Status](https://github.com/dyollb/segmantic/workflows/CI/badge.svg)](https://github.com/dyollb/sitk-cli/actions)
+[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/sitk-cli.svg)](https://badge.fury.io/py/sitk-cli)
+<img src="https://img.shields.io/pypi/dm/sitk-cli.svg?label=pypi%20downloads&logo=python&logoColor=green"/>
+
+## Overview
+
+Create [Typer](https://github.com/tiangolo/typer) command line interface from functions that use [SimpleITK](https://github.com/SimpleITK/SimpleITK) images (and transforms) as arguments or return type.
+
+```Python
+import SimpleITK as sitk
+import typer
+
+from sitk_cli import register_command
+
+app = typer.Typer()
+
+
+@register_command(app)
+def fill_holes_slice_by_slice(mask: sitk.Image) -> sitk.Image:
+    mask = mask != 0
+    output = sitk.Image(mask.GetSize(), mask.GetPixelID())
+    output.CopyInformation(mask)
+    for k in range(mask.GetSize()[2]):
+        output[:, :, k] = sitk.BinaryFillhole(mask[:, :, k], fullyConnected=False)
+    return output
+
+
+if __name__ == "__main__":
+    app()
+```
+
+To work, sitk-cli inspects the type annotations of the function and creates a wrapper function that loads images from file and passes these to the original function. Returned images (transforms) are written to a file by the wrapper function..
+
+## Installation
+
+```sh
+pip install sitk-cli
+```
+
+## Demo
+
+![Command lind demo](https://github.com/dyollb/sitk-cli/raw/main/docs/demo.gif)
```

### Comparing `sitk-cli-0.6.0/src/sitk_cli/lib.py` & `sitk_cli-0.7.0/src/sitk_cli/lib.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,125 +1,131 @@
-
-import sys
-from inspect import Parameter, isclass, signature
-from pathlib import Path
-from typing import Optional, Union, get_args, get_origin
-if sys.version_info >= (3,10):
-    from types import UnionType as UnionType
-else:
-    from typing import Union as UnionType
-
-import SimpleITK as sitk
-import typer
-from makefun import wraps
-
-
-def make_cli(func, output_arg_name="output"):
-    """Make command line interface from function with sitk.Image args"""
-    image_args = []
-    transform_args = []
-
-    def _parse_annotation(annotation):
-        """handle Optional[A], Union[A, None] and A | None, and string annotations"""
-        if isinstance(annotation, str):
-            if sys.version_info >= (3,10):
-                annotation = eval(annotation)
-            else:
-                if "|" in annotation:
-                    types = ",".join(t.strip() for t in annotation.split("|"))
-                    annotation = f"Union[{types}]"
-                annotation = eval(annotation)
-
-        origin = get_origin(annotation)
-        args = get_args(annotation)
-        if any(origin is t for t in (Union, UnionType)):
-            for a in args:
-                if not isinstance(a, type(None)):
-                    return a
-        return annotation
-
-    def _translate_param(p: Parameter):
-        """translate signature parameters"""
-        annotation = _parse_annotation(p.annotation)
-        default = p.default
-
-        if isclass(annotation) and issubclass(annotation, (sitk.Image, sitk.Transform)):
-            if issubclass(annotation, sitk.Image):
-                image_args.append(p.name)
-            else:
-                transform_args.append(p.name)
-            annotation = Path
-            default = typer.Option(None) if p.default is None else typer.Option(...)
-        elif p.default == Parameter.empty:
-            default = typer.Option(...)
-        return Parameter(
-            p.name,
-            Parameter.POSITIONAL_OR_KEYWORD,
-            annotation=annotation,
-            default=default,
-        )
-
-    func_sig = signature(func)
-
-    params = []
-    for idx, p in enumerate(func_sig.parameters.values()):
-        params.append(_translate_param(p))
-
-    return_type = _parse_annotation(func_sig.return_annotation)
-    if (
-        return_type
-        and isclass(return_type)
-        and issubclass(return_type, (sitk.Image, sitk.Transform))
-    ):
-        params.append(
-            Parameter(
-                output_arg_name,
-                kind=Parameter.POSITIONAL_OR_KEYWORD,
-                default=None,
-                annotation=Path,
-            ),
-        )
-        return_type = None
-
-    new_sig = func_sig.replace(parameters=params, return_annotation=return_type)
-
-    @wraps(func, new_sig=new_sig)
-    def func_wrapper(*args, **kwargs):
-        output_file: Optional[Path] = None
-        kwargs_inner = {}
-        for k, v in kwargs.items():
-            if k == output_arg_name:
-                output_file = v
-                continue
-            if k in image_args and issubclass(type(v), Path):
-                v = sitk.ReadImage(f"{v}")
-            if k in transform_args and issubclass(type(v), Path):
-                v = sitk.ReadTransform(f"{v}")
-            kwargs_inner[k] = v
-
-        ret = func(*args, **kwargs_inner)
-        if output_file and ret:
-            if isinstance(ret, sitk.Image):
-                return sitk.WriteImage(ret, f"{output_file}")
-            else:
-                return sitk.WriteTransform(ret, f"{output_file}")
-        return ret
-
-    return func_wrapper
-
-
-def register_command(
-    app: typer.Typer, func_name: Optional[str] = None, output_arg_name: str = "output"
-):
-    """Register function as command"""
-
-    def decorator(func):
-        func_cli = make_cli(func, output_arg_name=output_arg_name)
-
-        @app.command()
-        @wraps(func_cli, func_name=func_name)
-        def foo(*args, **kwargs):
-            return func_cli(*args, **kwargs)
-
-        return func
-
-    return decorator
+import sys
+from inspect import Parameter, isclass, signature
+from pathlib import Path
+from typing import Optional, Union, get_args, get_origin
+
+if sys.version_info >= (3, 10):
+    from types import UnionType as UnionType
+else:
+    from typing import Union as UnionType
+
+import SimpleITK as sitk
+import typer
+from makefun import wraps
+
+
+def make_cli(func, output_arg_name="output", globals=None, locals=None):
+    """Make command line interface from function with sitk.Image args"""
+    image_args = []
+    transform_args = []
+
+    def _parse_annotation(annotation):
+        """handle Optional[A], Union[A, None] and A | None, and string annotations"""
+        if isinstance(annotation, str):
+            if sys.version_info >= (3, 10):
+                annotation = eval(annotation)
+            else:
+                if "|" in annotation:
+                    types = ",".join(t.strip() for t in annotation.split("|"))
+                    annotation = f"Union[{types}]"
+                annotation = eval(annotation, globals, locals)
+
+        origin = get_origin(annotation)
+        args = get_args(annotation)
+        if any(origin is t for t in (Union, UnionType)):
+            for a in args:
+                if not isinstance(a, type(None)):
+                    return a
+        return annotation
+
+    def _translate_param(p: Parameter):
+        """translate signature parameters"""
+        annotation = _parse_annotation(p.annotation)
+        default = p.default
+
+        if isclass(annotation) and issubclass(annotation, (sitk.Image, sitk.Transform)):
+            if issubclass(annotation, sitk.Image):
+                image_args.append(p.name)
+            else:
+                transform_args.append(p.name)
+            annotation = Path
+            default = typer.Option(None) if p.default is None else typer.Option(...)
+        elif p.default == Parameter.empty:
+            default = typer.Option(...)
+        return Parameter(
+            p.name,
+            Parameter.POSITIONAL_OR_KEYWORD,
+            annotation=annotation,
+            default=default,
+        )
+
+    func_sig = signature(func)
+
+    params = []
+    for idx, p in enumerate(func_sig.parameters.values()):
+        params.append(_translate_param(p))
+
+    return_type = _parse_annotation(func_sig.return_annotation)
+    if (
+        return_type
+        and isclass(return_type)
+        and issubclass(return_type, (sitk.Image, sitk.Transform))
+    ):
+        params.append(
+            Parameter(
+                output_arg_name,
+                kind=Parameter.POSITIONAL_OR_KEYWORD,
+                default=None,
+                annotation=Path,
+            ),
+        )
+        return_type = None
+
+    new_sig = func_sig.replace(parameters=params, return_annotation=return_type)
+
+    @wraps(func, new_sig=new_sig)
+    def func_wrapper(*args, **kwargs):
+        output_file: Optional[Path] = None
+        kwargs_inner = {}
+        for k, v in kwargs.items():
+            if k == output_arg_name:
+                output_file = v
+                continue
+            if k in image_args and issubclass(type(v), Path):
+                v = sitk.ReadImage(f"{v}")
+            if k in transform_args and issubclass(type(v), Path):
+                v = sitk.ReadTransform(f"{v}")
+            kwargs_inner[k] = v
+
+        ret = func(*args, **kwargs_inner)
+        if output_file and ret:
+            if isinstance(ret, sitk.Image):
+                return sitk.WriteImage(ret, f"{output_file}")
+            else:
+                return sitk.WriteTransform(ret, f"{output_file}")
+        return ret
+
+    return func_wrapper
+
+
+def register_command(
+    app: typer.Typer,
+    func_name: Optional[str] = None,
+    output_arg_name: str = "output",
+    globals=None,
+    locals=None,
+):
+    """Register function as command"""
+
+    def decorator(func):
+        func_cli = make_cli(
+            func, output_arg_name=output_arg_name, globals=globals, locals=locals
+        )
+
+        @app.command()
+        @wraps(func_cli, func_name=func_name)
+        def foo(*args, **kwargs):
+            return func_cli(*args, **kwargs)
+
+        return func
+
+    return decorator
```

### Comparing `sitk-cli-0.6.0/src/sitk_cli.egg-info/PKG-INFO` & `sitk_cli-0.7.0/src/sitk_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,62 @@
-Metadata-Version: 2.1
-Name: sitk-cli
-Version: 0.6.0
-Summary: Wrap SimpleITK functions as command lines
-Home-page: https://github.com/dyollb/sitk-cli
-License: MIT License
-Project-URL: Bug Tracker, https://github.com/dyollb/sitk-cli/issues
-Project-URL: Source Code, https://github.com/dyollb/sitk-cli
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# Wrap SimpleITK functions as command lines
-
-[![Build Actions Status](https://github.com/dyollb/segmantic/workflows/CI/badge.svg)](https://github.com/dyollb/sitk-cli/actions)
-[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://https://opensource.org/licenses/MIT)
-[![PyPI version](https://badge.fury.io/py/sitk-cli.svg)](https://badge.fury.io/py/sitk-cli)
-<img src="https://img.shields.io/pypi/dm/sitk-cli.svg?label=pypi%20downloads&logo=python&logoColor=green"/>
-
-## Overview
-
-Create [Typer](https://github.com/tiangolo/typer) command line interface from functions that use [SimpleITK](https://github.com/SimpleITK/SimpleITK) images (and transforms) as arguments or return type.
-
-```Python
-import SimpleITK as sitk
-import typer
-
-from sitk_cli import register_command
-
-app = typer.Typer()
-
-
-@register_command(app)
-def fill_holes_slice_by_slice(mask: sitk.Image) -> sitk.Image:
-    mask = mask != 0
-    output = sitk.Image(mask.GetSize(), mask.GetPixelID())
-    output.CopyInformation(mask)
-    for k in range(mask.GetSize()[2]):
-        output[:, :, k] = sitk.BinaryFillhole(mask[:, :, k], fullyConnected=False)
-    return output
-
-
-if __name__ == "__main__":
-    app()
-```
-
-To work, sitk-cli inspects the type annotations of the function and creates a wrapper function that loads images from file and passes these to the original function. Returned images (transforms) are written to a file by the wrapper function..
-
-## Installation
-
-```sh
-pip install sitk-cli
-```
-
-## Demo
-
-![Command lind demo](https://github.com/dyollb/sitk-cli/raw/main/docs/demo.gif)
+Metadata-Version: 2.1
+Name: sitk-cli
+Version: 0.7.0
+Summary: Wrap SimpleITK functions as command lines
+Home-page: https://github.com/dyollb/sitk-cli
+License: MIT License
+Project-URL: Bug Tracker, https://github.com/dyollb/sitk-cli/issues
+Project-URL: Source Code, https://github.com/dyollb/sitk-cli
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: makefun
+Requires-Dist: SimpleITK
+Requires-Dist: typer
+Provides-Extra: dev
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+
+# Wrap SimpleITK functions as command lines
+
+[![Build Actions Status](https://github.com/dyollb/segmantic/workflows/CI/badge.svg)](https://github.com/dyollb/sitk-cli/actions)
+[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/sitk-cli.svg)](https://badge.fury.io/py/sitk-cli)
+<img src="https://img.shields.io/pypi/dm/sitk-cli.svg?label=pypi%20downloads&logo=python&logoColor=green"/>
+
+## Overview
+
+Create [Typer](https://github.com/tiangolo/typer) command line interface from functions that use [SimpleITK](https://github.com/SimpleITK/SimpleITK) images (and transforms) as arguments or return type.
+
+```Python
+import SimpleITK as sitk
+import typer
+
+from sitk_cli import register_command
+
+app = typer.Typer()
+
+
+@register_command(app)
+def fill_holes_slice_by_slice(mask: sitk.Image) -> sitk.Image:
+    mask = mask != 0
+    output = sitk.Image(mask.GetSize(), mask.GetPixelID())
+    output.CopyInformation(mask)
+    for k in range(mask.GetSize()[2]):
+        output[:, :, k] = sitk.BinaryFillhole(mask[:, :, k], fullyConnected=False)
+    return output
+
+
+if __name__ == "__main__":
+    app()
+```
+
+To work, sitk-cli inspects the type annotations of the function and creates a wrapper function that loads images from file and passes these to the original function. Returned images (transforms) are written to a file by the wrapper function..
+
+## Installation
+
+```sh
+pip install sitk-cli
+```
+
+## Demo
+
+![Command lind demo](https://github.com/dyollb/sitk-cli/raw/main/docs/demo.gif)
```

### Comparing `sitk-cli-0.6.0/tests/test_make_cli.py` & `sitk_cli-0.7.0/tests/test_make_cli.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-from inspect import signature
-from pathlib import Path
-from typing import Optional, Tuple
-
-import SimpleITK as sitk
-
-import sitk_cli
-
-
-def get_shape(input: sitk.Image) -> Tuple[int, int]:
-    return input.GetWidth(), input.GetHeight()
-
-
-def make_image(width: int, height: int) -> sitk.Image:
-    return sitk.Image(width, height, sitk.sitkInt16)
-
-
-def register_api(
-    fixed: sitk.Image, moving: sitk.Image, init_transform: sitk.Transform
-) -> sitk.Transform:
-    tx = sitk.CenteredTransformInitializer(fixed, moving)
-    return sitk.CompositeTransform([init_transform, tx])
-
-
-def select_image(input1: sitk.Image, input2: Optional[sitk.Image]) -> sitk.Image:
-    return input1 if input2 is None else input2
-
-
-def test_make_cli_image_arg():
-    cli = sitk_cli.make_cli(get_shape)
-    sig = signature(cli)
-
-    assert len(sig.parameters) == 1
-    assert issubclass(sig.parameters["input"].annotation, Path)
-
-
-def test_make_cli_image_return():
-    cli = sitk_cli.make_cli(make_image)
-    sig = signature(cli)
-
-    assert len(sig.parameters) == 3
-    assert sig.parameters["width"].annotation is int
-    assert sig.parameters["height"].annotation is int
-    assert issubclass(sig.parameters["output"].annotation, Path)
-
-
-def test_make_cli_usage(tmp_path: Path):
-    make_image_cli = sitk_cli.make_cli(make_image)
-    get_width_cli = sitk_cli.make_cli(get_shape)
-
-    tmp_file = tmp_path / "image.nii.gz"
-    make_image_cli(width=32, height=64, output=tmp_file)
-    width, height = get_width_cli(input=tmp_file)
-    assert width == 32 and height == 64
-
-    # check running without writing output file
-    make_image_cli(width=32, height=64, output=None)
-
-
-def test_make_cli_transform_arg():
-    cli = sitk_cli.make_cli(register_api, output_arg_name="output_transform")
-    sig = signature(cli)
-
-    assert len(sig.parameters) == 4
-    assert issubclass(sig.parameters["fixed"].annotation, Path)
-    assert issubclass(sig.parameters["moving"].annotation, Path)
-    assert issubclass(sig.parameters["init_transform"].annotation, Path)
-    assert issubclass(sig.parameters["output_transform"].annotation, Path)
-
-
-def test_optional_argument():
-    cli = sitk_cli.make_cli(select_image)
-    sig = signature(cli)
-
-    assert len(sig.parameters) == 3
-    assert sig.parameters["input1"].annotation is Path
-    assert sig.parameters["input2"].annotation is Path
-    assert sig.parameters["output"].annotation, Path
+from inspect import signature
+from pathlib import Path
+from typing import Optional, Tuple
+
+import SimpleITK as sitk
+
+import sitk_cli
+
+
+def get_shape(input: sitk.Image) -> Tuple[int, int]:
+    return input.GetWidth(), input.GetHeight()
+
+
+def make_image(width: int, height: int) -> sitk.Image:
+    return sitk.Image(width, height, sitk.sitkInt16)
+
+
+def register_api(
+    fixed: sitk.Image, moving: sitk.Image, init_transform: sitk.Transform
+) -> sitk.Transform:
+    tx = sitk.CenteredTransformInitializer(fixed, moving)
+    return sitk.CompositeTransform([init_transform, tx])
+
+
+def select_image(input1: sitk.Image, input2: Optional[sitk.Image]) -> sitk.Image:
+    return input1 if input2 is None else input2
+
+
+def test_make_cli_image_arg():
+    cli = sitk_cli.make_cli(get_shape)
+    sig = signature(cli)
+
+    assert len(sig.parameters) == 1
+    assert issubclass(sig.parameters["input"].annotation, Path)
+
+
+def test_make_cli_image_return():
+    cli = sitk_cli.make_cli(make_image)
+    sig = signature(cli)
+
+    assert len(sig.parameters) == 3
+    assert sig.parameters["width"].annotation is int
+    assert sig.parameters["height"].annotation is int
+    assert issubclass(sig.parameters["output"].annotation, Path)
+
+
+def test_make_cli_usage(tmp_path: Path):
+    make_image_cli = sitk_cli.make_cli(make_image)
+    get_width_cli = sitk_cli.make_cli(get_shape)
+
+    tmp_file = tmp_path / "image.nii.gz"
+    make_image_cli(width=32, height=64, output=tmp_file)
+    width, height = get_width_cli(input=tmp_file)
+    assert width == 32 and height == 64
+
+    # check running without writing output file
+    make_image_cli(width=32, height=64, output=None)
+
+
+def test_make_cli_transform_arg():
+    cli = sitk_cli.make_cli(register_api, output_arg_name="output_transform")
+    sig = signature(cli)
+
+    assert len(sig.parameters) == 4
+    assert issubclass(sig.parameters["fixed"].annotation, Path)
+    assert issubclass(sig.parameters["moving"].annotation, Path)
+    assert issubclass(sig.parameters["init_transform"].annotation, Path)
+    assert issubclass(sig.parameters["output_transform"].annotation, Path)
+
+
+def test_optional_argument():
+    cli = sitk_cli.make_cli(select_image)
+    sig = signature(cli)
+
+    assert len(sig.parameters) == 3
+    assert sig.parameters["input1"].annotation is Path
+    assert sig.parameters["input2"].annotation is Path
+    assert sig.parameters["output"].annotation, Path
```

### Comparing `sitk-cli-0.6.0/tests/test_optional_args.py` & `sitk_cli-0.7.0/tests/test_optional_args.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from __future__ import annotations
-
-from inspect import Parameter, signature
-from pathlib import Path
-
-import SimpleITK as sitk
-from typer.models import OptionInfo
-
-import sitk_cli
-
-
-def select_image(input1: sitk.Image, input2: sitk.Image | None = None) -> sitk.Image:
-    return input1 if input2 is None else input2
-
-
-def pass_image(name: str, input: sitk.Image | None = None) -> sitk.Image | None:
-    return input
-
-
-def get_option_default(p: Parameter):
-    input_default: OptionInfo = p.default
-    assert isinstance(input_default, OptionInfo)
-    return input_default.default
-
-
-def test_optional_argument():
-    cli = sitk_cli.make_cli(select_image)
-    sig = signature(cli)
-
-    assert len(sig.parameters) == 3
-    assert sig.parameters["input1"].annotation is Path
-    assert sig.parameters["input2"].annotation is Path
-    assert sig.parameters["output"].annotation, Path
-
-    assert get_option_default(sig.parameters["input1"]) is not None
-    assert get_option_default(sig.parameters["input2"]) is None
-
-
-def _test_optional_return_type():
-    cli = sitk_cli.make_cli(pass_image)
-    sig = signature(cli)
-
-    assert len(sig.parameters) == 3
-    assert sig.parameters["name"].annotation is str
-    assert sig.parameters["input"].annotation is Path
-    assert sig.parameters["output"].annotation, Path
-
-    assert get_option_default(sig.parameters["name"]) is not None
-    assert get_option_default(sig.parameters["input"]) is None
+from __future__ import annotations
+
+from inspect import Parameter, signature
+from pathlib import Path
+
+import SimpleITK as sitk
+from typer.models import OptionInfo
+
+import sitk_cli
+
+
+def select_image(input1: sitk.Image, input2: sitk.Image | None = None) -> sitk.Image:
+    return input1 if input2 is None else input2
+
+
+def pass_image(name: str, input: sitk.Image | None = None) -> sitk.Image | None:
+    return input
+
+
+def get_option_default(p: Parameter):
+    input_default: OptionInfo = p.default
+    assert isinstance(input_default, OptionInfo)
+    return input_default.default
+
+
+def test_optional_argument():
+    cli = sitk_cli.make_cli(select_image)
+    sig = signature(cli)
+
+    assert len(sig.parameters) == 3
+    assert sig.parameters["input1"].annotation is Path
+    assert sig.parameters["input2"].annotation is Path
+    assert sig.parameters["output"].annotation, Path
+
+    assert get_option_default(sig.parameters["input1"]) is not None
+    assert get_option_default(sig.parameters["input2"]) is None
+
+
+def _test_optional_return_type():
+    cli = sitk_cli.make_cli(pass_image)
+    sig = signature(cli)
+
+    assert len(sig.parameters) == 3
+    assert sig.parameters["name"].annotation is str
+    assert sig.parameters["input"].annotation is Path
+    assert sig.parameters["output"].annotation, Path
+
+    assert get_option_default(sig.parameters["name"]) is not None
+    assert get_option_default(sig.parameters["input"]) is None
```

