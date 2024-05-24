# Comparing `tmp/pysonnet-0.0.1.tar.gz` & `tmp/pysonnet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysonnet-0.0.1.tar", max compression
+gzip compressed data, was "pysonnet-0.0.2.tar", max compression
```

## Comparing `pysonnet-0.0.1.tar` & `pysonnet-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2024-02-12 14:25:07.105321 pysonnet-0.0.1/LICENSE
--rw-r--r--   0        0        0     1763 2024-02-12 14:25:07.105321 pysonnet-0.0.1/README.md
--rw-r--r--   0        0        0     1496 2024-02-12 14:25:07.105321 pysonnet-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1658 2024-02-12 14:25:07.105321 pysonnet-0.0.1/pysonnet/__init__.py
--rw-r--r--   0        0        0      180 2024-02-12 14:25:07.109320 pysonnet-0.0.1/pysonnet/__main__.py
--rw-r--r--   0        0        0     5886 2024-02-12 14:25:07.109320 pysonnet-0.0.1/pysonnet/ast.py
--rw-r--r--   0        0        0     2742 2024-02-12 14:25:07.109320 pysonnet-0.0.1/pysonnet/cli.py
--rw-r--r--   0        0        0      146 2024-02-12 14:25:07.109320 pysonnet-0.0.1/pysonnet/errors.py
--rw-r--r--   0        0        0    25580 2024-02-12 14:25:07.109320 pysonnet-0.0.1/pysonnet/evaluator.py
--rw-r--r--   0        0        0    11972 2024-02-12 14:25:07.109320 pysonnet-0.0.1/pysonnet/lexer.py
--rw-r--r--   0        0        0    10922 2024-02-12 14:25:07.109320 pysonnet-0.0.1/pysonnet/objects.py
--rw-r--r--   0        0        0    30790 2024-02-12 14:25:07.109320 pysonnet-0.0.1/pysonnet/parser.py
--rw-r--r--   0        0        0        0 2024-02-12 14:25:07.109320 pysonnet-0.0.1/pysonnet/py.typed
--rw-r--r--   0        0        0     6549 2024-02-12 14:25:07.109320 pysonnet-0.0.1/pysonnet/stdlib.py
--rw-r--r--   0        0        0     2133 2024-02-12 14:25:07.109320 pysonnet-0.0.1/pysonnet/token.py
--rw-r--r--   0        0        0       89 2024-02-12 14:25:07.109320 pysonnet-0.0.1/pysonnet/types.py
--rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 pysonnet-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-24 10:48:15.899448 pysonnet-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1763 2024-05-24 10:48:15.899448 pysonnet-0.0.2/README.md
+-rw-r--r--   0        0        0     1496 2024-05-24 10:48:15.899448 pysonnet-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2196 2024-05-24 10:48:15.899448 pysonnet-0.0.2/pysonnet/__init__.py
+-rw-r--r--   0        0        0      180 2024-05-24 10:48:15.899448 pysonnet-0.0.2/pysonnet/__main__.py
+-rw-r--r--   0        0        0     5858 2024-05-24 10:48:15.899448 pysonnet-0.0.2/pysonnet/ast.py
+-rw-r--r--   0        0        0     2751 2024-05-24 10:48:15.899448 pysonnet-0.0.2/pysonnet/cli.py
+-rw-r--r--   0        0        0      146 2024-05-24 10:48:15.899448 pysonnet-0.0.2/pysonnet/errors.py
+-rw-r--r--   0        0        0    26439 2024-05-24 10:48:15.903448 pysonnet-0.0.2/pysonnet/evaluator.py
+-rw-r--r--   0        0        0    12278 2024-05-24 10:48:15.903448 pysonnet-0.0.2/pysonnet/lexer.py
+-rw-r--r--   0        0        0    11953 2024-05-24 10:48:15.903448 pysonnet-0.0.2/pysonnet/objects.py
+-rw-r--r--   0        0        0    30790 2024-05-24 10:48:15.903448 pysonnet-0.0.2/pysonnet/parser.py
+-rw-r--r--   0        0        0        0 2024-05-24 10:48:15.903448 pysonnet-0.0.2/pysonnet/py.typed
+-rw-r--r--   0        0        0     7583 2024-05-24 10:48:15.903448 pysonnet-0.0.2/pysonnet/stdlib.py
+-rw-r--r--   0        0        0     2133 2024-05-24 10:48:15.903448 pysonnet-0.0.2/pysonnet/token.py
+-rw-r--r--   0        0        0       89 2024-05-24 10:48:15.903448 pysonnet-0.0.2/pysonnet/types.py
+-rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 pysonnet-0.0.2/PKG-INFO
```

### Comparing `pysonnet-0.0.1/LICENSE` & `pysonnet-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysonnet-0.0.1/README.md` & `pysonnet-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pysonnet-0.0.1/pyproject.toml` & `pysonnet-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysonnet"
-version = "0.0.1"
+version = "0.0.2"
 description = "📜 A pure Python implementation of the Jsonnet language"
 authors = ["altescy <altescy@fastmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/altescy/pysonnet"
 
 [tool.poetry.scripts]
@@ -15,23 +15,23 @@
 priority = "primary"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 
 [tool.poetry.group.dev.dependencies]
 python-language-server = "^0.36.2"
-pytest = "^7.4.4"
-pysen = "^0.10.5"
-black = "^23.12.1"
+pytest = "^8.2.1"
+pysen = "^0.11.0"
+black = "^24.4.2"
 isort = "^5.13.2"
 flake8 = "^5.0.4"
-mypy = "^1.8.0"
+mypy = "^1.10.0"
 
 [tool.pysen]
-version = "0.10"
+version = "0.11"
 
 [tool.pysen-cli]
 settings_dir = "."
 
 [tool.pysen.lint]
 enable_black = true
 enable_flake8 = true
```

### Comparing `pysonnet-0.0.1/pysonnet/ast.py` & `pysonnet-0.0.2/pysonnet/ast.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 _T = TypeVar("_T", bound=_PRIMITIVE)
 _S = TypeVar("_S", bound=_PRIMITIVE)
 _T_co = TypeVar("_T_co", covariant=True, bound=_PRIMITIVE)
 _S_co = TypeVar("_S_co", covariant=True, bound=_PRIMITIVE)
 
 
 @dataclasses.dataclass(frozen=True)
-class AST(abc.ABC, Generic[_T_co]):
-    ...
+class AST(abc.ABC, Generic[_T_co]): ...
 
 
 @dataclasses.dataclass(frozen=True)
 class LiteralAST(AST[_T_co]):
     value: _T_co
 
 
@@ -27,26 +26,23 @@
 
 @dataclasses.dataclass(frozen=True)
 class Null(LiteralAST[Literal[None]]):
     value: Literal[None] = None
 
 
 @dataclasses.dataclass(frozen=True)
-class Boolean(LiteralAST[bool]):
-    ...
+class Boolean(LiteralAST[bool]): ...
 
 
 @dataclasses.dataclass(frozen=True)
-class Number(LiteralAST[Union[int, float]]):
-    ...
+class Number(LiteralAST[Union[int, float]]): ...
 
 
 @dataclasses.dataclass(frozen=True)
-class String(LiteralAST[str]):
-    ...
+class String(LiteralAST[str]): ...
 
 
 @dataclasses.dataclass(frozen=True)
 class Error(Generic[_T_co], AST[_T_co]):
     expr: AST[_T_co]
 
 
@@ -133,26 +129,23 @@
 
     operator: Operator
     left: AST[Any]
     right: AST[Any]
 
 
 @dataclasses.dataclass(frozen=True)
-class Self(AST[Dict[str, Any]]):
-    ...
+class Self(AST[Dict[str, Any]]): ...
 
 
 @dataclasses.dataclass(frozen=True)
-class Dollar(AST[Dict[str, Any]]):
-    ...
+class Dollar(AST[Dict[str, Any]]): ...
 
 
 @dataclasses.dataclass(frozen=True)
-class Super(AST[Dict[str, Any]]):
-    ...
+class Super(AST[Dict[str, Any]]): ...
 
 
 @dataclasses.dataclass(frozen=True)
 class Param(Generic[_T_co]):
     ident: Identifier
     default: Optional[AST[_T_co]] = None
```

### Comparing `pysonnet-0.0.1/pysonnet/cli.py` & `pysonnet-0.0.2/pysonnet/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,14 @@
 
     if args.ast:
         print(json.dumps(asdict(ast), indent=args.indent, ensure_ascii=args.ensure_ascii))
 
     ext_vars = _parse_ext_vars(args.ext_str)
 
     try:
-        evaluator = Evaluator(ext_vars, filename)
+        evaluator = Evaluator(filename, ext_vars=ext_vars)
         value = evaluator(ast)
     except PysonnetRuntimeError as e:
         print("Runtime Error:", e.args[0], file=sys.stderr)
         sys.exit(1)
 
     print(json.dumps(value.to_json(), indent=args.indent, ensure_ascii=args.ensure_ascii))
```

### Comparing `pysonnet-0.0.1/pysonnet/evaluator.py` & `pysonnet-0.0.2/pysonnet/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import dataclasses
 from os import PathLike
 from pathlib import Path
-from typing import Dict, List, Mapping, Optional, Union, cast
+from typing import Callable, Dict, List, Mapping, Optional, Union, cast
 
 from pysonnet import ast
 from pysonnet.errors import PysonnetRuntimeError
 from pysonnet.lexer import Lexer
 from pysonnet.objects import FALSE, NULL, TRUE, Array, Boolean, Function, Lazy, Null, Number, Object, Primitive, String
 from pysonnet.parser import Parser
 from pysonnet.stdlib import StdLib
+from pysonnet.types import JsonPrimitive
 
 
 def _make_lazy(evaluator: "Evaluator", node: ast.AST, context: "Context") -> Lazy:
     # specify default args to capture the values
     return Lazy(lambda evalualtor=evaluator, node=node, context=context: evaluator(node, context))  # type: ignore[misc]
 
 
@@ -22,31 +23,38 @@
     dollar: Optional[Object] = None
     super_: Optional[Object] = None
     this: Optional[Object] = None
 
     def clone(self) -> "Context":
         return Context(
             {k: v.clone() for k, v in self.bindings.items()},
-            self.dollar.clone() if self.dollar is not None else None,
+            self.dollar,
             self.super_.clone() if self.super_ is not None else None,
-            self.this.clone() if self.this is not None else None,
+            self.this,
         )
 
 
 class Evaluator:
     def __init__(
         self,
-        ext_vars: Optional[Mapping[str, str]] = None,
         filename: Optional[Union[str, PathLike]] = None,
+        *,
+        ext_vars: Optional[Mapping[str, str]] = None,
+        native_callbacks: Optional[Mapping[str, Union[Callable[..., JsonPrimitive], Function]]] = None,
     ) -> None:
         ext_vars = ext_vars or {}
         filename = Path(filename) if filename else None
-        self._ext_vars = ext_vars
+        callbacks = {
+            name: callback if isinstance(callback, Function) else Function.from_native_function(callback)
+            for name, callback in (native_callbacks or {}).items()
+        }
         self._filename = filename
-        self._stdlib = StdLib(ext_vars)
+        self._ext_vars = ext_vars
+        self._native_callbacks = callbacks
+        self._stdlib = StdLib(ext_vars, callbacks)
         self._stdobj = self._stdlib.as_object()
         self._rootdir = self._filename.parent if self._filename else Path("")
         self._stdobj.add_field(Object.Field(String("thisFile"), String(self._filename or "")))
 
     def _evaluate_literal(self, node: ast.LiteralAST, context: Context) -> Primitive:
         del context
         if isinstance(node, ast.Null):
@@ -101,15 +109,22 @@
         obj = Object()
         context = context.clone()
         context.bindings.update(bindings)
         context.this = obj
         if context.dollar is None:
             context.dollar = obj
         for key, field in objfields.items():
-            value = _make_lazy(self, field.expr, context)
+            _context = context.clone()
+            if isinstance(field.expr, ast.Object) and _context.super_:
+                super_ = _context.super_.get(key)
+                if super_ and isinstance(super_, Lazy):
+                    super_ = super_()
+                if super_ is None or isinstance(super_, Object):
+                    _context.super_ = super_
+            value = _make_lazy(self, field.expr, _context)
             inherit = field.inherit
             visibility = Object.Visibility.VISIBLE
             if field.visibility == ast.ObjectField.Visibility.HIDDEN:
                 visibility = Object.Visibility.HIDDEN
             elif field.visibility == ast.ObjectField.Visibility.FORCE_VISIBLE:
                 visibility = Object.Visibility.FORCE_VISIBLE
             obj.add_field(Object.Field(key, value, inherit, visibility))
@@ -117,23 +132,22 @@
 
     def _evaluate_array(self, node: ast.Array, context: Context) -> Array:
         return Array([self(expr, context) for expr in node.elements])
 
     def _evaluate_binary(self, node: ast.Binary, context: Context) -> Primitive:
         operator = node.operator
         left = self(node.left, context)
+        if isinstance(left, Lazy):
+            left = left()
         if isinstance(left, Object):
             context = context.clone()
             context.super_ = left
         right = self(node.right, context)
-        if isinstance(left, Lazy):
-            left = left()
         if isinstance(right, Lazy):
             right = right()
-        del context
         if operator == ast.Binary.Operator.ADD:
             if isinstance(left, Number) and isinstance(right, Number):
                 return left + right
             if isinstance(left, Array) and isinstance(right, Array):
                 return left + right
             if isinstance(left, String) and isinstance(right, (Number, String, Array, Object)):
                 return left + right
@@ -230,27 +244,30 @@
                 return Boolean(left in right)
             if isinstance(right, dict):
                 return Boolean(left in right)
             raise PysonnetRuntimeError(
                 f"Unsupported operand types for in: {self._stdlib._type(left)} and {self._stdlib._type(right)}"
             )
         if operator == ast.Binary.Operator.INDEX:
+            value: Primitive
             if isinstance(left, Array) and isinstance(right, Number):
                 try:
-                    return cast(Primitive, left[right.value])
+                    value = cast(Primitive, left[right.value])
                 except IndexError:
                     raise PysonnetRuntimeError(f"Index out of range, not within [0, {len(left)})")
-            if isinstance(left, Object):
+            elif isinstance(left, Object):
                 if not isinstance(right, String):
                     raise PysonnetRuntimeError(f"Unsupported type for index: {type(right)}, expected string")
                 try:
-                    return left[right]
+                    value = left[right]
                 except KeyError:
                     raise PysonnetRuntimeError(f"Field does not exist: {right}")
-            raise PysonnetRuntimeError(f"Unsupported operand types for index: {type(left)} and {type(right)}")
+            else:
+                raise PysonnetRuntimeError(f"Unsupported operand types for index: {type(left)} and {type(right)}")
+            return value
         raise PysonnetRuntimeError(f"Unsupported binary operator: {operator}")
 
     def _evaluate_apply(self, node: ast.Apply, context: Context) -> Primitive:
         callee = self(node.callee, context)
         if isinstance(callee, Lazy):
             callee = callee()
         if not isinstance(callee, Function):
@@ -452,15 +469,19 @@
         if not filename.is_file():
             raise PysonnetRuntimeError(f"Not a file: {filename}")
         with filename.open() as f:
             jp = Parser(Lexer(f))
             ast = jp.parse()
         if not ast:
             raise PysonnetRuntimeError(f"Failed to parse {filename}")
-        evaluator = Evaluator(self._ext_vars, filename)
+        evaluator = Evaluator(
+            filename,
+            ext_vars=self._ext_vars,
+            native_callbacks=self._native_callbacks,
+        )
         return evaluator(ast)
 
     def _evaluate_importstr(self, node: ast.Importstr, context: Context) -> String:
         del context
         filename = self._rootdir / Path(node.filename)
         if not filename.exists():
             raise PysonnetRuntimeError(f"File not found: {filename}")
```

### Comparing `pysonnet-0.0.1/pysonnet/lexer.py` & `pysonnet-0.0.2/pysonnet/lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 from .token import Token, TokenType, lookup_hidden, lookup_ident
 
 _IDENT_START = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ_"
 _IDENT_CONT = _IDENT_START + "0123456789"
 _HEXDIGITS = "0123456789abcdefABCDEF"
 _HORIZ_WS = " \t\r"
 _INDENT_WS = " \t"
+_ESCAPED_CHARS = {
+    '"': '"',
+    "'": "'",
+    "\\": "\\",
+    "/": "/",
+    "b": "\b",
+    "f": "\f",
+    "n": "\n",
+    "r": "\r",
+    "t": "\t",
+}
 
 
 class Lexer:
     def __init__(self, textio: TextIO) -> None:
         self._textio = textio
         self._ch = self._read_char()
 
@@ -105,21 +116,24 @@
                 raise ValueError("unexpected end of file")
             if self._ch == quote:
                 self._read_char()
                 break
             elif not verbatim and self._ch == "\\":
                 next_ch = self._peek()
                 if next_ch in ('"', "'", "\\", "/", "b", "f", "n", "r", "t"):
-                    literal += self._ch + self._read_char()
-                    self._read_char()
+                    literal += _ESCAPED_CHARS[next_ch]
+                    self._read_char(2)
                 elif next_ch == "u":
                     if all(self._peek(i + 2) in _HEXDIGITS for i in range(4)):
+                        self._read_char(2)  # skip "\u"
+                        codepoint = ""
                         for ch in range(4):
-                            literal += self._ch
+                            codepoint += self._ch
                             self._read_char()
+                        literal += chr(int(codepoint, 16))
                     else:
                         raise ValueError(f"unexpected character: {self._ch}")
             else:
                 literal += self._ch
                 self._read_char()
 
         return literal
```

### Comparing `pysonnet-0.0.1/pysonnet/objects.py` & `pysonnet-0.0.2/pysonnet/objects.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,27 +23,46 @@
     def to_json(self) -> JsonPrimitive:
         """Convert the object to a JSON-serializable object."" """
         raise NotImplementedError
 
     def clone(self: _Self) -> _Self:
         return copy.deepcopy(self)
 
+    @staticmethod
+    def from_json_primitive(value: JsonPrimitive) -> Primitive:
+        if isinstance(value, bool):
+            return Boolean(value)
+        if isinstance(value, (int, float)):
+            return Number(value)
+        if isinstance(value, str):
+            return String(value)
+        if value is None:
+            return Null()
+        if isinstance(value, list):
+            return Array([Primitive.from_json_primitive(v) for v in value])
+        if isinstance(value, dict):
+            return Object(*(Object.Field(key, Primitive.from_json_primitive(val)) for key, val in value.items()))
+        raise ValueError(f"Invalid JSON primitive: {value}")
+
 
 class Lazy(Primitive):
     def __init__(self, constructor: Callable[[], Primitive]) -> None:
         self._constructor = constructor
 
     def __call__(self) -> Primitive:
         value = self._constructor()
         while isinstance(value, Lazy):
             value = value()
         return value
 
     def __str__(self) -> str:
-        return json.dumps(self.to_json())
+        value = self.to_json()
+        if isinstance(value, str):
+            return value
+        return json.dumps(value)
 
     def __repr__(self) -> str:
         return f"Lazy({self._constructor})"
 
     def to_json(self) -> JsonPrimitive:
         return self().to_json()
 
@@ -57,112 +76,91 @@
 
 
 class Number(Generic[_Real_co], Primitive):
     def __init__(self, value: _Real_co) -> None:
         self.value: _Real_co = value
 
     @overload
-    def __add__(self: Number[Union[bool, int]], other: Number[Union[bool, int]]) -> Number[int]:
-        ...
+    def __add__(self: Number[Union[bool, int]], other: Number[Union[bool, int]]) -> Number[int]: ...
 
     @overload
-    def __add__(self: Number[Union[bool, int]], other: Number[float]) -> Number[float]:
-        ...
+    def __add__(self: Number[Union[bool, int]], other: Number[float]) -> Number[float]: ...
 
     @overload
-    def __add__(self: Number[float], other: Number[Union[bool, int]]) -> Number[float]:
-        ...
+    def __add__(self: Number[float], other: Number[Union[bool, int]]) -> Number[float]: ...
 
     @overload
-    def __add__(self: Number[float], other: Number[float]) -> Number[float]:
-        ...
+    def __add__(self: Number[float], other: Number[float]) -> Number[float]: ...
 
     @overload
-    def __add__(self, other: String) -> String:
-        ...
+    def __add__(self, other: String) -> String: ...
 
     def __add__(
         self, other: Union[Number[Union[bool, int, float]], String]
     ) -> Union[Number[Union[int, float]], String]:
         if isinstance(other, String):
             return String(json.dumps(self.to_json())) + other
         return Number(self.value + other.value)
 
     @overload
-    def __sub__(self: Number[Union[bool, int]], other: Number[Union[bool, int]]) -> Number[int]:
-        ...
+    def __sub__(self: Number[Union[bool, int]], other: Number[Union[bool, int]]) -> Number[int]: ...
 
     @overload
-    def __sub__(self: Number[Union[bool, int]], other: Number[float]) -> Number[float]:
-        ...
+    def __sub__(self: Number[Union[bool, int]], other: Number[float]) -> Number[float]: ...
 
     @overload
-    def __sub__(self: Number[float], other: Number[Union[bool, int]]) -> Number[float]:
-        ...
+    def __sub__(self: Number[float], other: Number[Union[bool, int]]) -> Number[float]: ...
 
     @overload
-    def __sub__(self: Number[float], other: Number[float]) -> Number[float]:
-        ...
+    def __sub__(self: Number[float], other: Number[float]) -> Number[float]: ...
 
     def __sub__(self, other: Number[Union[bool, int, float]]) -> Number[Union[int, float]]:
         return Number(self.value - other.value)
 
     @overload
-    def __mul__(self: Number[Union[bool, int]], other: Number[Union[bool, int]]) -> Number[int]:
-        ...
+    def __mul__(self: Number[Union[bool, int]], other: Number[Union[bool, int]]) -> Number[int]: ...
 
     @overload
-    def __mul__(self: Number[Union[bool, int]], other: Number[float]) -> Number[float]:
-        ...
+    def __mul__(self: Number[Union[bool, int]], other: Number[float]) -> Number[float]: ...
 
     @overload
-    def __mul__(self: Number[float], other: Number[Union[bool, int]]) -> Number[float]:
-        ...
+    def __mul__(self: Number[float], other: Number[Union[bool, int]]) -> Number[float]: ...
 
     @overload
-    def __mul__(self: Number[float], other: Number[float]) -> Number[float]:
-        ...
+    def __mul__(self: Number[float], other: Number[float]) -> Number[float]: ...
 
     def __mul__(self, other: Number[Union[bool, int, float]]) -> Number[Union[int, float]]:
         return Number(self.value * other.value)
 
     @overload
-    def __truediv__(self: Number[Union[bool, int]], other: Number[Union[bool, int]]) -> Number[float]:
-        ...
+    def __truediv__(self: Number[Union[bool, int]], other: Number[Union[bool, int]]) -> Number[float]: ...
 
     @overload
-    def __truediv__(self: Number[Union[bool, int]], other: Number[float]) -> Number[float]:
-        ...
+    def __truediv__(self: Number[Union[bool, int]], other: Number[float]) -> Number[float]: ...
 
     @overload
-    def __truediv__(self: Number[float], other: Number[Union[bool, int]]) -> Number[float]:
-        ...
+    def __truediv__(self: Number[float], other: Number[Union[bool, int]]) -> Number[float]: ...
 
     @overload
-    def __truediv__(self: Number[float], other: Number[float]) -> Number[float]:
-        ...
+    def __truediv__(self: Number[float], other: Number[float]) -> Number[float]: ...
 
     def __truediv__(self, other: Number[Union[bool, int, float]]) -> Number[float]:
         return Number(self.value / other.value)
 
     @overload
-    def __mod__(self: Number[Union[bool, int]], other: Number[Union[bool, int]]) -> Number[int]:
-        ...
+    def __mod__(self: Number[Union[bool, int]], other: Number[Union[bool, int]]) -> Number[int]: ...
 
     @overload
-    def __mod__(self: Number[Union[bool, int]], other: Number[float]) -> Number[float]:
-        ...
+    def __mod__(self: Number[Union[bool, int]], other: Number[float]) -> Number[float]: ...
 
     @overload
-    def __mod__(self: Number[float], other: Number[Union[bool, int]]) -> Number[float]:
-        ...
+    def __mod__(self: Number[float], other: Number[Union[bool, int]]) -> Number[float]: ...
 
     @overload
-    def __mod__(self: Number[float], other: Number[float]) -> Number[float]:
-        ...
+    def __mod__(self: Number[float], other: Number[float]) -> Number[float]: ...
 
     def __mod__(self, other: Number[Union[bool, int, float]]) -> Number[Union[int, float]]:
         return Number(self.value % other.value)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Number):
             return NotImplemented
@@ -208,16 +206,15 @@
     def __float__(self) -> float:
         return float(self.value)
 
     def to_json(self) -> Union[bool, int, float]:
         return self.value
 
 
-class Boolean(Number[bool]):
-    ...
+class Boolean(Number[bool]): ...
 
 
 class String(str, Primitive):
     def __add__(self, other: Union[Number, String, Array, Object]) -> String:  # type: ignore[override]
         if not isinstance(other, String):
             other = String(json.dumps(other.to_json()))
         return String(super().__add__(other))
@@ -233,15 +230,15 @@
         if isinstance(other, Number):
             other = other.to_json()  # type: ignore[assignment]
         if isinstance(other, Array):
             other = tuple(other)  # type: ignore[assignment]
         return String(super().__mod__(other))
 
     def to_json(self) -> str:
-        return self
+        return str(self)
 
 
 class Array(Generic[_PrimitiveType], List[_PrimitiveType], Primitive):
     def __add__(self, other: Array) -> Array:  # type: ignore[override]
         return Array(super().__add__(other))
 
     def to_json(self) -> List[JsonPrimitive]:
@@ -336,12 +333,21 @@
 
     def __str__(self) -> str:
         raise NotImplementedError
 
     def to_json(self) -> None:
         raise NotImplementedError
 
+    @staticmethod
+    def from_native_function(func: Callable[..., JsonPrimitive]) -> Function[Primitive]:
+        def wrapper(*args: Primitive, **kwargs: Primitive) -> Primitive:
+            native_args = [arg.to_json() for arg in args]
+            native_kwargs = {key: value.to_json() for key, value in kwargs.items()}
+            return Primitive.from_json_primitive(func(*native_args, **native_kwargs))
+
+        return Function(wrapper)
+
 
 # Constants
 NULL = Null()
 TRUE = Boolean(True)
 FALSE = Boolean(False)
```

### Comparing `pysonnet-0.0.1/pysonnet/parser.py` & `pysonnet-0.0.2/pysonnet/parser.py`

 * *Files identical despite different names*

### Comparing `pysonnet-0.0.1/pysonnet/stdlib.py` & `pysonnet-0.0.2/pysonnet/stdlib.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+import json
 import sys
 from functools import wraps
 from typing import Any, Callable, Mapping, TypeVar, Union
 
 from pysonnet.errors import PysonnetRuntimeError
 from pysonnet.objects import NULL, TRUE, Array, Boolean, Function, Lazy, Null, Number, Object, Primitive, String
 
@@ -26,24 +27,35 @@
         evaluated_params = {k: v() if isinstance(v, Lazy) else v for k, v in params.items()}
         return func(**evaluated_params)
 
     return wrapper
 
 
 class StdLib:
-    def __init__(self, ext_vars: Mapping[str, str] = {}) -> None:
+    def __init__(
+        self,
+        ext_vars: Mapping[str, str] = {},
+        native_callbacks: Mapping[str, Callable[..., Primitive]] = {},
+    ) -> None:
         self._ext_vars = ext_vars
+        self._native_callbacks = native_callbacks
 
     @_eval_args
     def _ext_var(self, x: String) -> String:
         if x not in self._ext_vars:
             raise PysonnetRuntimeError(f"Undefined external variable: {x}")
         return String(self._ext_vars[x])
 
     @_eval_args
+    def _native(self, name: String) -> Function[Primitive]:
+        if name not in self._native_callbacks:
+            raise PysonnetRuntimeError(f"Undefined native callback: {name}")
+        return Function(self._native_callbacks[name])
+
+    @_eval_args
     def _type(self, x: Primitive) -> String:
         if isinstance(x, Null):
             return String("null")
         if isinstance(x, Boolean):
             return String("boolean")
         if isinstance(x, Number):
             return String("number")
@@ -164,17 +176,36 @@
         return str % vals
 
     @_eval_args
     def _trace(self, str: String, rest: _T) -> _T:
         print("TRACE:", str, file=sys.stderr)
         return rest
 
+    @_eval_args
+    def _manifest_json_ex(
+        self,
+        value: Primitive,
+        indent: String,
+        newline: String = String("\n"),
+        key_val_sep: String = String(": "),
+    ) -> String:
+        return String(
+            json.dumps(
+                value.to_json(),
+                indent=str(indent),
+                separators=(",", str(key_val_sep)),
+                sort_keys=True,
+                ensure_ascii=False,
+            )
+        )
+
     def as_object(self) -> Object:
         return Object(
             Object.Field(String("extVar"), Function(self._ext_var)),
+            Object.Field(String("native"), Function(self._native)),
             Object.Field(String("type"), Function(self._type)),
             Object.Field(String("length"), Function(self._length)),
             Object.Field(String("get"), Function(self._get)),
             Object.Field(String("objectHas"), Function(self._object_has)),
             Object.Field(String("slice"), Function(self._slice)),
             Object.Field(String("range"), Function(self._range)),
             Object.Field(String("map"), Function(self._map)),
@@ -184,8 +215,9 @@
             Object.Field(String("abs"), Function(self._abs)),
             Object.Field(String("max"), Function(self._max)),
             Object.Field(String("min"), Function(self._min)),
             Object.Field(String("clamp"), Function(self._clamp)),
             Object.Field(String("toString"), Function(self._to_string)),
             Object.Field(String("format"), Function(self._format)),
             Object.Field(String("trace"), Function(self._trace)),
+            Object.Field(String("manifestJsonEx"), Function(self._manifest_json_ex)),
         )
```

### Comparing `pysonnet-0.0.1/pysonnet/token.py` & `pysonnet-0.0.2/pysonnet/token.py`

 * *Files identical despite different names*

### Comparing `pysonnet-0.0.1/PKG-INFO` & `pysonnet-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysonnet
-Version: 0.0.1
+Version: 0.0.2
 Summary: 📜 A pure Python implementation of the Jsonnet language
 Home-page: https://github.com/altescy/pysonnet
 License: MIT
 Author: altescy
 Author-email: altescy@fastmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

