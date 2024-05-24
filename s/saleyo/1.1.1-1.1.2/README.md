# Comparing `tmp/saleyo-1.1.1.tar.gz` & `tmp/saleyo-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saleyo-1.1.1.tar", last modified: Thu Apr 25 02:30:18 2024, max compression
+gzip compressed data, was "saleyo-1.1.2.tar", last modified: Fri May 24 06:28:50 2024, max compression
```

## Comparing `saleyo-1.1.1.tar` & `saleyo-1.1.2.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0     1063 2024-04-25 02:30:02.587123 saleyo-1.1.1/LICENSE
--rw-r--r--   0        0        0     2537 2024-04-25 02:30:02.587123 saleyo-1.1.1/README.md
--rw-r--r--   0        0        0      581 2024-04-25 02:30:18.307066 saleyo-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1359 2024-04-25 02:30:02.587123 saleyo-1.1.1/src/saleyo/__init__.py
--rw-r--r--   0        0        0      103 2024-04-25 02:30:02.587123 saleyo-1.1.1/src/saleyo/base/__init__.py
--rw-r--r--   0        0        0      872 2024-04-25 02:30:02.587123 saleyo-1.1.1/src/saleyo/base/template.py
--rw-r--r--   0        0        0     3993 2024-04-25 02:30:02.587123 saleyo-1.1.1/src/saleyo/base/toolchain.py
--rw-r--r--   0        0        0      541 2024-04-25 02:30:02.587123 saleyo-1.1.1/src/saleyo/base/typing.py
--rw-r--r--   0        0        0     4917 2024-04-25 02:30:02.587123 saleyo-1.1.1/src/saleyo/mixin.py
--rw-r--r--   0        0        0      484 2024-04-25 02:30:02.587123 saleyo-1.1.1/src/saleyo/operation/__init__.py
--rw-r--r--   0        0        0     3005 2024-04-25 02:30:02.587123 saleyo-1.1.1/src/saleyo/operation/accessor.py
--rw-r--r--   0        0        0     1154 2024-04-25 02:30:02.587123 saleyo-1.1.1/src/saleyo/operation/ancestor.py
--rw-r--r--   0        0        0     3156 2024-04-25 02:30:02.587123 saleyo-1.1.1/src/saleyo/operation/hook.py
--rw-r--r--   0        0        0     1847 2024-04-25 02:30:02.587123 saleyo-1.1.1/src/saleyo/operation/intercept.py
--rw-r--r--   0        0        0     1543 2024-04-25 02:30:02.587123 saleyo-1.1.1/src/saleyo/operation/modify.py
--rw-r--r--   0        0        0     1280 2024-04-25 02:30:02.587123 saleyo-1.1.1/src/saleyo/operation/overwrite.py
--rw-r--r--   0        0        0     2727 2024-04-25 02:30:02.587123 saleyo-1.1.1/src/saleyo/operation/processor.py
--rw-r--r--   0        0        0      100 2024-04-25 02:30:02.587123 saleyo-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0      244 2024-04-25 02:30:02.587123 saleyo-1.1.1/tests/custom.py
--rw-r--r--   0        0        0     1168 2024-04-25 02:30:02.587123 saleyo-1.1.1/tests/demo.py
--rw-r--r--   0        0        0      396 2024-04-25 02:30:02.587123 saleyo-1.1.1/tests/gc_test.py
--rw-r--r--   0        0        0      528 2024-04-25 02:30:02.587123 saleyo-1.1.1/tests/intercept.py
--rw-r--r--   0        0        0      711 2024-04-25 02:30:02.587123 saleyo-1.1.1/tests/misc_test.py
--rw-r--r--   0        0        0      216 2024-04-25 02:30:02.587123 saleyo-1.1.1/tests/modify_test.py
--rw-r--r--   0        0        0       37 2024-04-25 02:30:02.587123 saleyo-1.1.1/tests/test_module_a.py
--rw-r--r--   0        0        0      239 2024-04-25 02:30:02.587123 saleyo-1.1.1/tests/test_module_b.py
--rw-r--r--   0        0        0     2972 1970-01-01 00:00:00.000000 saleyo-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-24 06:28:35.584041 saleyo-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2537 2024-05-24 06:28:35.584041 saleyo-1.1.2/README.md
+-rw-r--r--   0        0        0      581 2024-05-24 06:28:50.523923 saleyo-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1334 2024-05-24 06:28:35.584041 saleyo-1.1.2/src/saleyo/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-24 06:28:35.584041 saleyo-1.1.2/src/saleyo/base/__init__.py
+-rw-r--r--   0        0        0      894 2024-05-24 06:28:35.584041 saleyo-1.1.2/src/saleyo/base/template.py
+-rw-r--r--   0        0        0     4076 2024-05-24 06:28:35.584041 saleyo-1.1.2/src/saleyo/base/toolchain.py
+-rw-r--r--   0        0        0      540 2024-05-24 06:28:35.584041 saleyo-1.1.2/src/saleyo/base/typing.py
+-rw-r--r--   0        0        0      138 2024-05-24 06:28:35.584041 saleyo-1.1.2/src/saleyo/decorator/__init__.py
+-rw-r--r--   0        0        0     1327 2024-05-24 06:28:35.584041 saleyo-1.1.2/src/saleyo/decorator/ancestor.py
+-rw-r--r--   0        0        0     4971 2024-05-24 06:28:35.584041 saleyo-1.1.2/src/saleyo/decorator/mixin.py
+-rw-r--r--   0        0        0      519 2024-05-24 06:28:35.584041 saleyo-1.1.2/src/saleyo/operation/__init__.py
+-rw-r--r--   0        0        0     3053 2024-05-24 06:28:35.584041 saleyo-1.1.2/src/saleyo/operation/accessor.py
+-rw-r--r--   0        0        0     3232 2024-05-24 06:28:35.584041 saleyo-1.1.2/src/saleyo/operation/hook.py
+-rw-r--r--   0        0        0     1879 2024-05-24 06:28:35.584041 saleyo-1.1.2/src/saleyo/operation/intercept.py
+-rw-r--r--   0        0        0     1581 2024-05-24 06:28:35.584041 saleyo-1.1.2/src/saleyo/operation/modify.py
+-rw-r--r--   0        0        0     1307 2024-05-24 06:28:35.584041 saleyo-1.1.2/src/saleyo/operation/overwrite.py
+-rw-r--r--   0        0        0     2762 2024-05-24 06:28:35.584041 saleyo-1.1.2/src/saleyo/operation/processor.py
+-rw-r--r--   0        0        0      100 2024-05-24 06:28:35.584041 saleyo-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      199 2024-05-24 06:28:35.588041 saleyo-1.1.2/tests/ans.py
+-rw-r--r--   0        0        0      239 2024-05-24 06:28:35.588041 saleyo-1.1.2/tests/custom.py
+-rw-r--r--   0        0        0     1176 2024-05-24 06:28:35.588041 saleyo-1.1.2/tests/demo.py
+-rw-r--r--   0        0        0      396 2024-05-24 06:28:35.588041 saleyo-1.1.2/tests/gc_test.py
+-rw-r--r--   0        0        0      528 2024-05-24 06:28:35.588041 saleyo-1.1.2/tests/intercept.py
+-rw-r--r--   0        0        0      711 2024-05-24 06:28:35.588041 saleyo-1.1.2/tests/misc_test.py
+-rw-r--r--   0        0        0      216 2024-05-24 06:28:35.588041 saleyo-1.1.2/tests/modify_test.py
+-rw-r--r--   0        0        0       37 2024-05-24 06:28:35.588041 saleyo-1.1.2/tests/test_module_a.py
+-rw-r--r--   0        0        0      249 2024-05-24 06:28:35.588041 saleyo-1.1.2/tests/test_module_b.py
+-rw-r--r--   0        0        0     2972 1970-01-01 00:00:00.000000 saleyo-1.1.2/PKG-INFO
```

### Comparing `saleyo-1.1.1/LICENSE` & `saleyo-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `saleyo-1.1.1/README.md` & `saleyo-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `saleyo-1.1.1/pyproject.toml` & `saleyo-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "saleyo"
-version = "1.1.1"
+version = "1.1.2"
 description = "Saleyo is a lightwight scalable Python AOP framework, easy to use and integrate."
 authors = [
     { name = "H2Sxxa", email = "h2sxxa0w0@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
```

### Comparing `saleyo-1.1.1/src/saleyo/__init__.py` & `saleyo-1.1.2/src/saleyo/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,28 +11,27 @@
 
 https://github.com/H2Sxxa/saleyo/blob/main/README.md
 
 https://pypi.org/project/saleyo/
 """
 
 from . import base as base
-from . import mixin as mixin
 from . import operation as operation
-from .mixin import Mixin as Mixin
+from .base.template import MixinOperation as MixinOperation
+from .base.toolchain import Arguments as Arguments
+from .base.toolchain import CPyToolChain as CPyToolChain
+from .base.toolchain import GCToolChain as GCToolChain
+from .base.toolchain import InvokeEvent as InvokeEvent
+from .base.toolchain import ToolChain as ToolChain
+from .decorator import Ancestor as Ancestor
+from .decorator import Mixin as Mixin
 from .operation import Accessor as Accessor
+from .operation import Alias as Alias
+from .operation import Del as Del
 from .operation import FunctionAccessor as FunctionAccessor
-from .operation import Processor as Processor
+from .operation import Insert as Insert
 from .operation import Intercept as Intercept
 from .operation import OverWrite as OverWrite
-from .operation import Pre as Pre
 from .operation import Post as Post
-from .operation import Del as Del
+from .operation import Pre as Pre
+from .operation import Processor as Processor
 from .operation import ReName as ReName
-from .operation import Alias as Alias
-from .operation import Ancestor as Ancestor
-from .operation import Insert as Insert
-from .base.toolchain import ToolChain as ToolChain
-from .base.toolchain import Arguments as Arguments
-from .base.toolchain import InvokeEvent as InvokeEvent
-from .base.toolchain import CPyToolChain as CPyToolChain
-from .base.toolchain import GCToolChain as GCToolChain
-from .base.template import MixinOperation as MixinOperation
```

### Comparing `saleyo-1.1.1/src/saleyo/base/template.py` & `saleyo-1.1.2/src/saleyo/base/template.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from abc import ABC
 from typing import Any, Generic
 
-from .toolchain import ToolChain
-from .typing import T, M
+from .toolchain import DefaultToolChain, ToolChain
+from .typing import M, T
 
 
 class MixinOperation(Generic[T], ABC):
     """
     The MixinOperation is the base of All Operation.
 
     The generic `MixinOperation` is the type of argument.
 
     `level` will affect to the mixin order, default `1`.
-    
-    If you call the `MixinOperation` or call the subclass of this, it will call the `MixinOperation.argument` 
+
+    If you call the `MixinOperation` or call the subclass of this,
+    it will call the `MixinOperation.argument`
     """
 
     argument: T
     level: int
 
     def __init__(self, argument: T, level=1) -> None:
         self.argument = argument
         self.level = level
 
-    def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
+    def mixin(self, target: M, toolchain: ToolChain = DefaultToolChain) -> None:
         raise NotImplementedError(
             f"Not Ready to use this Operation to modify '{target}' via '{toolchain}'"
         )
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any: ...
```

### Comparing `saleyo-1.1.1/src/saleyo/base/toolchain.py` & `saleyo-1.1.2/src/saleyo/base/toolchain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from ctypes import py_object as _py_object, POINTER as _POINTER, cast as _cast
-from types import FunctionType
+from ctypes import POINTER as _POINTER
+from ctypes import cast as _cast
+from ctypes import py_object as _py_object
 from dataclasses import dataclass
 from gc import get_referents as _get_referents
+from types import FunctionType
 from typing import Any, Callable, Dict, Generic, Optional
 
-from ..base.typing import P, T, NameSpace
+from ..base.typing import NameSpace, P, T
 
 
 @dataclass
 class ToolChain:
     """
     The tool class to do mixin.
 
@@ -17,28 +19,32 @@
 
     tool_getattr: Callable[[Any, str], Any] = getattr
     tool_setattr: Callable[[Any, str, Any], None] = setattr
     tool_hasattr: Callable[[Any, str], bool] = hasattr
     tool_delattr: Callable[[Any, str], None] = delattr
 
 
+DefaultToolChain = ToolChain()
+
 GCToolChain = ToolChain(
     tool_getattr=lambda _object, _name: _get_referents(_object.__dict__)[0][_name],
     tool_hasattr=lambda _object, _name: _name in _get_referents(_object.__dict__)[0],
     tool_setattr=lambda _object, _name, _attr: _get_referents(_object.__dict__)[
         0
     ].update({_name: _attr}),
     tool_delattr=lambda _object, _name: _get_referents(_object.__dict__)[0].__delitem__(
         _name
     ),
 )
 """
-GC ToolChain use the `get_referents` functions in `gc` and it can modify some special class.
+GC ToolChain use the `get_referents` functions in `gc` and 
+it can modify some special class.
 
-Notice: There is no guarantee that it can modify any class, and this method is rude and dangerous, avoid using it in produce environment.
+Notice: There is no guarantee that it can modify any class,
+and this method is rude and dangerous, avoid using it in produce environment.
 """
 
 
 def _cpy_get_dict(_object: Any) -> Dict[str, Any]:
     return _cast(
         id(_object) + type(_object).__dictoffset__, _POINTER(_py_object)
     ).contents.value
@@ -49,23 +55,26 @@
     tool_hasattr=lambda _object, _name: _name in _cpy_get_dict(_object),
     tool_setattr=lambda _object, _name, _attr: _cpy_get_dict(_object).update(
         {_name: _attr}
     ),
     tool_delattr=lambda _object, _name: _cpy_get_dict(_object).__delitem__(_name),
 )
 """
-`CPyToolChain` use the `ctypes` to modify class, it's dangerous than other default toolchains.
+`CPyToolChain` use the `ctypes` to modify class, 
+it's dangerous than other default toolchains.
 
-Notice: There is no guarantee that it can modify any class, and this method is rude and dangerous, avoid using it in produce environment.
+Notice: There is no guarantee that it can modify any class, 
+and this method is rude and dangerous, avoid using it in produce environment.
 """
 
 
 class Container:
     """
-    Container is A Class to keep a namespace and use this namespace to define function / variable / ...
+    Container is A Class to keep a namespace and
+    use this namespace to define function / variable / ...
     """
 
     environment: NameSpace
 
     def __init__(self, *namespace: Optional[NameSpace]) -> None:
         self.environment = {
             k: v for _ in namespace if _ is not None for k, v in _.items()
@@ -86,28 +95,30 @@
                 [line.removeprefix(" " * indent) for line in source.splitlines()]
             )
         )[function_name]
 
 
 class Arguments(Generic[P]):
     """
-    `Argument` is used to call function, the Generic `P` is the params of target function.
+    `Argument` is used to call function,
+    the Generic `P` is the params of target function.
     """
 
     def __init__(self, *args: P.args, **kwargs: P.kwargs) -> None:
         self.args = args
         self.kwargs = kwargs
 
     def __str__(self) -> str:
         return f"Arugument( positional: {self.args}, keyword: {self.kwargs} )"
 
 
 class InvokeEvent(Generic[P, T]):
     """
-    A `InvokeEvent` includes the target function and the arguments to call this functions.
+    A `InvokeEvent` includes the target function and the arguments to
+    call this functions.
     """
 
     target: Callable[P, T]
     argument: Arguments[P]
 
     def __init__(
         self,
```

### Comparing `saleyo-1.1.1/src/saleyo/base/typing.py` & `saleyo-1.1.2/src/saleyo/base/typing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from types import ModuleType
 from typing import Any, Dict, Iterable, ParamSpec, Type, TypeVar, Union
 
-
 # Generic
 
 RT = TypeVar("RT")
 """
 `RT` means `Return Type`
 """
 T = TypeVar("T")
```

### Comparing `saleyo-1.1.1/src/saleyo/mixin.py` & `saleyo-1.1.2/src/saleyo/decorator/mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 from typing import Generic, Iterable, List, Union
 
-from .base.template import MixinOperation
-from .base.toolchain import ToolChain
-from .base.typing import M, T, IterableOrSingle
+from ..base.template import MixinOperation
+from ..base.toolchain import DefaultToolChain, ToolChain
+from ..base.typing import IterableOrSingle, M, T
 
 
 class Mixin(Generic[M]):
     """
     A `Mixin` Decorator is used to invoke all the `MixinOperation` in Mixin Class.
 
     If the target is a special class, you should custom the toolchain yourself.
 
-    It is recommend to use `assert isinstance(self, <target>)` at the head of operation functions, although there may be some performance cost, but it is worth it in most conditions.
+    It is recommend to use `assert isinstance(self, <target>)` at the head of
+    operation functions, although there may be some performance cost,
+    but it is worth it in most conditions.
 
     Allow to have more than one target, but that's not recommended.
     """
 
     target: Iterable[M]
     toolchain: ToolChain
     reverse_level: bool
 
     def __init__(
         self,
         target: IterableOrSingle[M],
-        toolchain: ToolChain = ToolChain(),
+        toolchain: ToolChain = DefaultToolChain,
         reverse_level: bool = False,
     ) -> None:
         self.target = target if isinstance(target, Iterable) else [target]
         self.toolchain = toolchain
         self.reverse_level = reverse_level
 
     @staticmethod
     def from_name(
         target: IterableOrSingle[str],
-        toolchain: ToolChain = ToolChain(),
+        toolchain: ToolChain = DefaultToolChain,
         reverse_level: bool = False,
         qualname: bool = False,
     ) -> "Mixin":
         """
-        Will find target classes from `object.__subclasses__()` from class name or qualname.
+        Will find target classes via `object.__subclasses__()`.
 
-        If want to find a class named `Foo`, default use the `Foo` to match, it will use `module.to.Foo` to match when `qualname` enabled.
+        If want to find a class named `Foo`, default use the `Foo` to match,
+        it will use `module.to.Foo` to match when `qualname` enabled.
 
         Please use this after the definition of target class.
 
-        The method may takes lots of time when there are a whole lot classes, recommand to use `@Mixin()` directly if you can.
+        The method may takes lots of time when there are a whole lot classes,
+        recommand to use `@Mixin()` directly if you can.
         """
 
         target = target if isinstance(target, Iterable) else [target]
 
         return Mixin(
             filter(
                 lambda clazz: clazz.__name__ in target
@@ -60,29 +64,32 @@
             reverse_level=reverse_level,
         )
 
     @staticmethod
     def from_regex(
         pattern: str,
         pattern_flags: int = 0,
-        toolchain: ToolChain = ToolChain(),
+        toolchain: ToolChain = DefaultToolChain,
         reverse_level: bool = False,
         qualname: bool = False,
         full_match: bool = False,
     ) -> "Mixin":
         """
-        Will use regex pattern to find target classes from the `object.__subclasses__()`.
+        Will use regex pattern to find target classes from the `object.__subclasses__()`
 
-        The `pattern` will convert to a `Pattern[str]` via `re.complie` and you can provide flags in `pattern_flags`.
+        The `pattern` will convert to a `Pattern[str]` via `re.complie` and
+        you can provide flags in `pattern_flags`.
 
-        If want to find a class named `Foo`, default use the `Foo` to match, it will use `module.to.Foo` to match when `qualname` enabled.
+        If want to find a class named `Foo`, default use the `Foo` to match,
+        it will use `module.to.Foo` to match when `qualname` enabled.
 
         Please use this after the definition of target class.
 
-        The method may takes lots of time when there are a whole lot classes, recommand to use `@Mixin()` directly if you can.
+        The method may takes lots of time when there are a whole lot classes,
+        recommand to use `@Mixin()` directly if you can.
         """
         import re
 
         regex_pattern = re.compile(pattern=pattern, flags=pattern_flags)
         matcher = regex_pattern.fullmatch if full_match else regex_pattern.match
 
         return Mixin(
```

### Comparing `saleyo-1.1.1/src/saleyo/operation/accessor.py` & `saleyo-1.1.2/src/saleyo/operation/accessor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from typing import Callable, Generic, Optional
 
-from ..base.toolchain import ToolChain
-from ..base.typing import P, T, M
 from ..base.template import MixinOperation
+from ..base.toolchain import DefaultToolChain, ToolChain
+from ..base.typing import M, P, T
 
 
 class Accessor(Generic[T], MixinOperation[str]):
     """
-    The Generic `T` is the type of target varible, if you want to visit a private function, try to use the subclass `FunctionAccessor`.
+    The Generic `T` is the type of target varible,
+    if you want to visit a private function, try to use the subclass `FunctionAccessor`.
 
     Notice: The value only available after invoking the `mixin` method.
 
-    If the `private` is `True`, will add target class name (like `_Foo`) to the prefix to argument, if the target is complex, you can set `private` to `False` and provide the true name by yourself.
+    If the `private` is `True`, will add target class name (like `_Foo`) to the prefix
+    to argument, if the target is complex,
+    you can set `private` to `False` and provide the true name by yourself.
 
-    Also a variable named `argument` will add to target classes when `private` is `True`.
+    Also a variable named `argument` will add to target classes when `private` is `True`
 
-    If you use `@Mixin` and have more than one target classes, the `value` will always be the varible of latest target.
+    If you use `@Mixin` and have more than one target classes, the `value` will always
+    be the varible of latest target.
     """
 
     _inner: Optional[T]
     _private: bool
 
     def __init__(self, argument: str, level=1, private=True) -> None:
         super().__init__(argument, level)
         self._inner = None
         self._private = private
 
-    def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
+    def mixin(self, target: M, toolchain: ToolChain = DefaultToolChain) -> None:
         self._inner = toolchain.tool_getattr(
             target,
             f"_{target.__name__}{self.argument}" if self._private else self.argument,
         )
         if self._private:
             toolchain.tool_setattr(
                 target,
@@ -61,21 +65,25 @@
 
 class FunctionAccessor(Generic[P, T], Accessor[Callable[P, T]]):
     """
     `FunctionAccessor` can be call directly.
 
     It's recommend to provide the Generic `P` and `T`, it can be useful in `__call__`.
 
-    If the `private` is `True`, will add target class name (like `_Foo`) to the prefix to argument, if the target is complex, you can set `private` to `False` and provide the true name by yourself.
+    If the `private` is `True`, will add target class name (like `_Foo`) to the prefix
+    to argument, if the target is complex, you can set `private` to `False` and
+    provide the true name by yourself.
 
-    Also a variable named `argument` will add to target classes when `private` is `True`.s
+    Also a variable named `argument` will add to target classes when `private` is `True`
 
-    If you just call in operation functions, you can just use a simple variable with `Callable[P, T]` type.
-    
-    If you use `@Mixin` and have more than one target classes, the `value` will always be the varible of latest target.
+    If you just call in operation functions, you can just use a simple variable with
+    `Callable[P, T]` type.
+
+    If you use `@Mixin` and have more than one target classes, the `value` will always
+    be the varible of latest target.
 
     ```python
     something: FunctionAccessor[[str], None] = FunctionAccessor("something")
     ```
     """
 
     def __call__(self, *args: P.args, **kwargs: P.kwargs) -> T:
```

### Comparing `saleyo-1.1.1/src/saleyo/operation/ancestor.py` & `saleyo-1.1.2/src/saleyo/decorator/ancestor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-from typing import Any, Type
+from typing import Any, Generic, Type
 
-from ..base.template import MixinOperation
-from ..base.toolchain import ToolChain
-from ..base.typing import M
+from ..base.toolchain import DefaultToolChain, ToolChain
+from ..base.typing import T
 
 
-class Ancestor(MixinOperation[Type[Any]]):
+class Ancestor(Generic[T]):
     """
-    Ancestor will add the `argument` to `target.__bases__`.
+    Ancestor will add the `ancestor_class` to `target.__bases__`.
+    (Please see `__call__` method)
+
+    Please ensure the `target.__bases__` is not `(object,)`, this decorator requires
+    the target has at least one super class.
 
     If `reverse`, the `argument` will add to the head of `target.__bases__`.
 
-    Don't try to use it with external code and `module`, it may crash.
+    Don't try to use it with external code and `module`, it will crash.
     """
 
     reverse: bool
+    target: Type[Any]
+    toolchain: ToolChain
 
-    def __init__(self, argument: Type[Any], level=1, reverse=False) -> None:
-        super().__init__(argument, level)
+    def __init__(
+        self, target: Type[Any], toolchain: ToolChain = DefaultToolChain, reverse=False
+    ) -> None:
         self.reverse = reverse
+        self.target = target
+        self.toolchain = toolchain
 
-    @staticmethod
-    def configure(
-        level: int = 1,
-        reverse=False,
-    ):
-        return lambda argument: Ancestor(
-            argument,
-            level=level,
-            reverse=reverse,
-        )
+    def __call__(self, ancestor_class: Type[T]) -> Type[T]:
+        assert self.target.__bases__ != (object,)
 
-    def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
-        return toolchain.tool_setattr(
-            target,
+        self.toolchain.tool_setattr(
+            self.target,
             "__bases__",
-            (self.argument, *toolchain.tool_getattr(target, "__bases__"))
+            (ancestor_class, *self.toolchain.tool_getattr(self.target, "__bases__"))
             if self.reverse
-            else (*toolchain.tool_getattr(target, "__bases__"), self.argument),
+            else (
+                *self.toolchain.tool_getattr(self.target, "__bases__"),
+                ancestor_class,
+            ),
         )
+
+        return ancestor_class
```

### Comparing `saleyo-1.1.1/src/saleyo/operation/hook.py` & `saleyo-1.1.2/src/saleyo/operation/hook.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from typing import Any, Callable, Optional, Union
 
-from ..base.typing import M, P, RT, T
-from ..base.toolchain import ToolChain, Arguments
 from ..base.template import MixinOperation
+from ..base.toolchain import Arguments, DefaultToolChain, ToolChain
+from ..base.typing import RT, M, P, T
 
 
 class Post(MixinOperation[Callable[[T], Optional[RT]]]):
     """
-    `Post` will call after the target method, and the callable should be decorated as `@staticmethod` and have one argument to receive the result of target method.
+    `Post` will call after the target method, and the callable should be decorated as
+    `@staticmethod` and have one argument to receive the result of target method.
 
-    If the `post` function return value is not `None`, it will replace the original result.
+    If the `post` function return value is not `None`,
+    it will replace the original result.
     """
 
     target_name: Optional[str]
 
     def __init__(
         self,
         argument: Callable[[T], RT],
@@ -30,35 +32,39 @@
     ):
         return lambda argument: Post(
             argument=argument,
             target_name=target_name,
             level=level,
         )
 
-    def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
+    def mixin(self, target: M, toolchain: ToolChain = DefaultToolChain) -> None:
         target_name = (
             self.target_name if self.target_name is not None else self.argument.__name__
         )
-        native_function: Callable[..., T] = toolchain.tool_getattr(target, target_name)
+        original_function: Callable[..., T] = toolchain.tool_getattr(
+            target, target_name
+        )
 
         def post(*args, **kwargs) -> Union[T, RT]:
-            result = native_function(*args, **kwargs)
+            result = original_function(*args, **kwargs)
             post_result = self.argument(result)
             if post_result is not None:
                 return post_result
             return result
 
         return toolchain.tool_setattr(target, target_name, post)
 
 
 class Pre(MixinOperation[Callable[P, Optional[Arguments[P]]]]):
     """
-    `Pre` will call before the target method, and the callable should be decorated as `@staticmethod` and have `*args,**kwargs` to receive the arguments of target method.
+    `Pre` will call before the target method, and the callable should be decorated as
+    `@staticmethod` and have `*args,**kwargs` to receive the arguments of target method.
 
-    If the `pre` function return value is a `Aruguments`(not `None`), it will replace the original arguments.
+    If the `pre` function return value is a `Aruguments`(not `None`),
+    it will replace the original arguments.
     """
 
     target_name: Optional[str]
 
     def __init__(
         self,
         argument: Callable[P, Optional[Arguments[P]]],
@@ -75,20 +81,20 @@
     ):
         return lambda argument: Pre(
             argument=argument,
             target_name=target_name,
             level=level,
         )
 
-    def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
+    def mixin(self, target: M, toolchain: ToolChain = DefaultToolChain) -> None:
         target_name = (
             self.target_name if self.target_name is not None else self.argument.__name__
         )
-        native_function = toolchain.tool_getattr(target, target_name)
+        original_function = toolchain.tool_getattr(target, target_name)
 
         def pre(*args: P.args, **kwargs: P.kwargs) -> Any:
             arguments = self.argument(*args, **kwargs)
             if arguments is not None:
-                return native_function(*arguments.args, **arguments.kwargs)
-            return native_function(*args, **kwargs)
+                return original_function(*arguments.args, **arguments.kwargs)
+            return original_function(*args, **kwargs)
 
         return toolchain.tool_setattr(target, target_name, pre)
```

### Comparing `saleyo-1.1.1/src/saleyo/operation/intercept.py` & `saleyo-1.1.2/src/saleyo/operation/intercept.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from typing import Any, Callable, Generic, Optional, ParamSpec
 
-from ..base.typing import M
-from ..base.toolchain import InvokeEvent, ToolChain
 from ..base.template import MixinOperation
+from ..base.toolchain import DefaultToolChain, InvokeEvent, ToolChain
+from ..base.typing import M
 
 _PA = ParamSpec("_PA")
 _PB = ParamSpec("_PB")
 _A = InvokeEvent[_PA, Any]
 _B = InvokeEvent[_PB, Any]
 
 
 class Intercept(Generic[_PA, _PB], MixinOperation[Callable[[_A[_PA]], _B[_PB]]]):
     """
     The `Intercept` allow you to intercept the arguments before invoking target method.
 
-    Then, you can handle these arguments in your own function and make a redirect to another function.
+    Then, you can handle thefse arguments in your own function and make a redirect to
+    another function.
 
     If you just want to modify the arguments or the result, please see `Pre` and `Post`.
     """
 
     target_name: Optional[str]
 
     def __init__(
@@ -40,25 +41,25 @@
             level=level,
             target_name=target_name,
         )
 
     def mixin(
         self,
         target: M,
-        toolchain: ToolChain = ToolChain(),
+        toolchain: ToolChain = DefaultToolChain,
     ) -> None:
         target_name = (
             self.target_name if self.target_name is not None else self.argument.__name__
         )
 
-        native_function = toolchain.tool_getattr(
+        original_function = toolchain.tool_getattr(
             target,
             target_name,
         )
 
         return toolchain.tool_setattr(
             target,
             target_name,
             lambda *args, **kwargs: self.argument(
-                InvokeEvent(native_function, *args, **kwargs)
+                InvokeEvent(original_function, *args, **kwargs)
             ).invoke_target(),
         )
```

### Comparing `saleyo-1.1.1/src/saleyo/operation/overwrite.py` & `saleyo-1.1.2/src/saleyo/operation/overwrite.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Callable, Optional
 
-from ..base.typing import M
-from ..base.toolchain import ToolChain
 from ..base.template import MixinOperation
+from ..base.toolchain import DefaultToolChain, ToolChain
+from ..base.typing import M
 
 
 class OverWrite(MixinOperation[Callable]):
     """
     OverWrite is rude and it will cover the target method.
 
-    If the target method doesn't exist, overwrite will add overwrite method to target class.
+    If the target method doesn't exist,
+    overwrite will add overwrite method to target class.
 
     Try avoid using `OverWrite` with other `OverWrite`.
     """
 
     target_name: Optional[str]
 
     def __init__(
@@ -29,15 +30,15 @@
         target_name: Optional[str] = None,
     ) -> Callable[[Callable], "OverWrite"]:
         return lambda argument: OverWrite(
             argument=argument,
             target_name=target_name,
         )
 
-    def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
+    def mixin(self, target: M, toolchain: ToolChain = DefaultToolChain) -> None:
         target_name = (
             self.argument.__name__ if self.target_name is None else self.target_name
         )
         self.argument.__qualname__ = f"{target.__name__}.{target_name}"
         return toolchain.tool_setattr(
             target,
             target_name,
```

### Comparing `saleyo-1.1.1/src/saleyo/operation/processor.py` & `saleyo-1.1.2/src/saleyo/operation/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from inspect import getsource
 from types import ModuleType
 from typing import Callable, Optional
 
-from ..base.typing import M, NameSpace
-from ..base.toolchain import Container, ToolChain
 from ..base.template import MixinOperation
+from ..base.toolchain import Container, DefaultToolChain, ToolChain
+from ..base.typing import M, NameSpace
 
 
 class Processor(MixinOperation[Callable[[str], str]]):
     """
-    If you want to get the soure code of a method and use `split` and `replace` to modify and redefine it,Try `Processor`.
+    If you want to get the soure code of a method and use `split` and
+    `replace` to modify and redefine it,Try `Processor`.
 
-    When you try to use this, please make sure you configure the correct module of your target, or you can use `extra_namespace` to supplement the missing things.
+    When you try to use this, please make sure you configure
+    the correct module of your target, or you can use `extra_namespace` to
+    supplement the missing things.
 
     Don't try to use it with external code, like the code of cpython, it will crash.
     """
 
     module: Optional[ModuleType]
     extra_namespace: Optional[NameSpace]
     target_name: Optional[str]
@@ -52,15 +55,15 @@
             module=module,
             extra_namespace=extra_namespace,
         )
 
     def mixin(
         self,
         target: M,
-        toolchain: ToolChain = ToolChain(),
+        toolchain: ToolChain = DefaultToolChain,
     ) -> None:
         target_name = (
             self.target_name if self.target_name is not None else self.argument.__name__
         )
 
         return toolchain.tool_setattr(
             target,
```

### Comparing `saleyo-1.1.1/tests/demo.py` & `saleyo-1.1.2/tests/demo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from typing import Any
-from saleyo import Mixin, Accessor, OverWrite, Post, Pre, Intercept, InvokeEvent
+
+from saleyo import Accessor, Intercept, InvokeEvent, Mixin, OverWrite, Post, Pre
 
 
 class Foo:
     __private = "private varible"
 
     def demo(self):
         pass
 
 
 @Mixin(target=Foo)
 class MixinFoo:
-    # Will add a varible named `__private` to Foo and it has the same address with `_Foo__private`
+    # Will add a varible named `__private` to Foo and 
+    # it has the same address with `_Foo__private`
     private: Accessor[str] = Accessor("__private")
 
     # Will Add the `func` to `Foo`
     @OverWrite
     def func(self):
         print("hello saleyo")
```

### Comparing `saleyo-1.1.1/tests/intercept.py` & `saleyo-1.1.2/tests/intercept.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from saleyo import Mixin, Intercept, Post, Pre, InvokeEvent
+from saleyo import Intercept, InvokeEvent, Mixin, Post, Pre
 
 
 class Foo:
     def demo(self):
         print("goodbye~")
```

### Comparing `saleyo-1.1.1/tests/misc_test.py` & `saleyo-1.1.2/tests/misc_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from saleyo import Mixin, Insert
+from saleyo import Insert, Mixin
 from saleyo.operation.accessor import Accessor, FunctionAccessor
 
 
 class Foo:
     __value: int = 1
 
     def __increase_value(self) -> None:
```

### Comparing `saleyo-1.1.1/PKG-INFO` & `saleyo-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saleyo
-Version: 1.1.1
+Version: 1.1.2
 Summary: Saleyo is a lightwight scalable Python AOP framework, easy to use and integrate.
 Author-Email: H2Sxxa <h2sxxa0w0@gmail.com>
 License: MIT
 Project-URL: Homepage, https://pypi.org/project/saleyo/
 Project-URL: Repository, https://github.com/H2Sxxa/saleyo
 Project-URL: Issues, https://github.com/H2Sxxa/saleyo/issues
 Requires-Python: >=3.8
```

