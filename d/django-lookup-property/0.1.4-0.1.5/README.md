# Comparing `tmp/django_lookup_property-0.1.4.tar.gz` & `tmp/django_lookup_property-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_lookup_property-0.1.4.tar", max compression
+gzip compressed data, was "django_lookup_property-0.1.5.tar", max compression
```

## Comparing `django_lookup_property-0.1.4.tar` & `django_lookup_property-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1064 2024-04-16 16:40:30.128764 django_lookup_property-0.1.4/LICENSE
--rw-r--r--   0        0        0     2745 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/README.md
--rw-r--r--   0        0        0      305 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/__init__.py
--rw-r--r--   0        0        0      689 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/converters/__init__.py
--rw-r--r--   0        0        0     2383 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/converters/aggregates.py
--rw-r--r--   0        0        0     4255 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/converters/cast.py
--rw-r--r--   0        0        0     1915 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/converters/conditions.py
--rw-r--r--   0        0        0    10299 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/converters/datetime.py
--rw-r--r--   0        0        0     3382 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/converters/expressions.py
--rw-r--r--   0        0        0     4311 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/converters/functions.py
--rw-r--r--   0        0        0    11160 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/converters/lookups.py
--rw-r--r--   0        0        0     2361 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/converters/main.py
--rw-r--r--   0        0        0     6043 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/converters/math.py
--rw-r--r--   0        0        0      433 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/converters/number.py
--rw-r--r--   0        0        0     9155 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/converters/string.py
--rw-r--r--   0        0        0     2081 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/converters/utils.py
--rw-r--r--   0        0        0     4052 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/decorator.py
--rw-r--r--   0        0        0     1284 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/dispatch.py
--rw-r--r--   0        0        0    14239 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/expressions.py
--rw-r--r--   0        0        0     3438 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/field.py
--rw-r--r--   0        0        0        0 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/py.typed
--rw-r--r--   0        0        0     2155 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/lookup_property/typing.py
--rw-r--r--   0        0        0     5479 2024-04-16 16:40:30.132763 django_lookup_property-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3887 1970-01-01 00:00:00.000000 django_lookup_property-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2745 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/README.md
+-rw-r--r--   0        0        0      305 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/__init__.py
+-rw-r--r--   0        0        0      689 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/__init__.py
+-rw-r--r--   0        0        0     2383 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/aggregates.py
+-rw-r--r--   0        0        0     4255 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/cast.py
+-rw-r--r--   0        0        0     1915 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/conditions.py
+-rw-r--r--   0        0        0    10299 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/datetime.py
+-rw-r--r--   0        0        0     3382 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/expressions.py
+-rw-r--r--   0        0        0     4311 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/functions.py
+-rw-r--r--   0        0        0    11293 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/lookups.py
+-rw-r--r--   0        0        0     2361 2024-05-24 10:22:11.982308 django_lookup_property-0.1.5/lookup_property/converters/main.py
+-rw-r--r--   0        0        0     6043 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/converters/math.py
+-rw-r--r--   0        0        0      433 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/converters/number.py
+-rw-r--r--   0        0        0     9155 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/converters/string.py
+-rw-r--r--   0        0        0     2081 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/converters/utils.py
+-rw-r--r--   0        0        0     4052 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/decorator.py
+-rw-r--r--   0        0        0     1284 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/dispatch.py
+-rw-r--r--   0        0        0    14501 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/expressions.py
+-rw-r--r--   0        0        0     3438 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/field.py
+-rw-r--r--   0        0        0        0 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/py.typed
+-rw-r--r--   0        0        0     2155 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/lookup_property/typing.py
+-rw-r--r--   0        0        0     5480 2024-05-24 10:22:11.986309 django_lookup_property-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3887 1970-01-01 00:00:00.000000 django_lookup_property-0.1.5/PKG-INFO
```

### Comparing `django_lookup_property-0.1.4/LICENSE` & `django_lookup_property-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/README.md` & `django_lookup_property-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/lookup_property/converters/__init__.py` & `django_lookup_property-0.1.5/lookup_property/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/lookup_property/converters/aggregates.py` & `django_lookup_property-0.1.5/lookup_property/converters/aggregates.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/lookup_property/converters/cast.py` & `django_lookup_property-0.1.5/lookup_property/converters/cast.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/lookup_property/converters/conditions.py` & `django_lookup_property-0.1.5/lookup_property/converters/conditions.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/lookup_property/converters/datetime.py` & `django_lookup_property-0.1.5/lookup_property/converters/datetime.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/lookup_property/converters/expressions.py` & `django_lookup_property-0.1.5/lookup_property/converters/expressions.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/lookup_property/converters/functions.py` & `django_lookup_property-0.1.5/lookup_property/converters/functions.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/lookup_property/converters/lookups.py` & `django_lookup_property-0.1.5/lookup_property/converters/lookups.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,22 +53,27 @@
 
     if expression.negated:
         return ast.UnaryOp(op=ast.Not(), operand=comparison)
 
     return comparison
 
 
-def and_or_comparison(children: list[tuple[str, Any]], expression: models.Q, state: State) -> ast.BoolOp:
+def and_or_comparison(children: list[tuple[str, Any] | models.Q], expression: models.Q, state: State) -> ast.BoolOp:
     """
     Q(foo=1) | Q(bar=2) -> self.foo == 1 or self.bar == 2
     Q(foo=1) & Q(bar=2) -> self.foo == 1 and self.bar == 2
     """
     return ast.BoolOp(
         op=ast.Or() if expression.connector == models.Q.OR else ast.And(),
-        values=[to_lookup_comparison(attr=attr, value=value, state=state) for attr, value in children],
+        values=[
+            expression_to_ast(item, state)
+            if isinstance(item, models.Q)
+            else to_lookup_comparison(attr=item[0], value=item[1], state=state)
+            for item in children
+        ],
     )
 
 
 def xor_comparison(children: list[tuple[str, Any]], state: State) -> ast.BinOp:
     """Q(foo__in=[...]) ^ Q(bar=1) -> (self.foo in [...]) ^ (self.bar == 1)"""
     return ast.BinOp(
         left=(
```

### Comparing `django_lookup_property-0.1.4/lookup_property/converters/main.py` & `django_lookup_property-0.1.5/lookup_property/converters/main.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/lookup_property/converters/math.py` & `django_lookup_property-0.1.5/lookup_property/converters/math.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/lookup_property/converters/string.py` & `django_lookup_property-0.1.5/lookup_property/converters/string.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/lookup_property/converters/utils.py` & `django_lookup_property-0.1.5/lookup_property/converters/utils.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/lookup_property/decorator.py` & `django_lookup_property-0.1.5/lookup_property/decorator.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/lookup_property/dispatch.py` & `django_lookup_property-0.1.5/lookup_property/dispatch.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/lookup_property/expressions.py` & `django_lookup_property-0.1.5/lookup_property/expressions.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,19 +177,29 @@
 
     def __hash__(self) -> int:
         value = getattr(self, "value", Sentinel)
         if value is not Sentinel:
             return hash((self.lookup, make_hashable(value)))
         return hash(self.lookup)
 
+    def order_by(
+        self,
+        *,
+        descending: bool = False,
+        nulls_first: bool | None = None,
+        nulls_last: bool | None = None,
+    ) -> models.OrderBy:
+        return models.OrderBy(self, descending, nulls_first, nulls_last)
+
     def asc(self, **kwargs: Any) -> models.OrderBy:
-        return models.OrderBy(self, **kwargs)
+        return self.order_by(**kwargs)
 
     def desc(self, **kwargs: Any) -> models.OrderBy:
-        return models.OrderBy(self, descending=True, **kwargs)
+        kwargs["descending"] = True
+        return self.order_by(**kwargs)
 
     def resolve_expression(  # noqa: PLR0913
         self,
         query: Query,
         allow_joins: bool,  # noqa: FBT001
         reuse: Any = None,
         summarize: bool = False,  # noqa: FBT001, FBT002
```

### Comparing `django_lookup_property-0.1.4/lookup_property/field.py` & `django_lookup_property-0.1.5/lookup_property/field.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/lookup_property/typing.py` & `django_lookup_property-0.1.5/lookup_property/typing.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.4/pyproject.toml` & `django_lookup_property-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-lookup-property"
-version = "0.1.4"
+version = "0.1.5"
 description = "Django model properties that are also lookup expressions."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "lookup_property" },
 ]
@@ -45,32 +45,32 @@
 "Bug Tracker" = "https://github.com/MrThearMan/django-lookup-property/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<4"
 Django = ">=4.2"
 
 [tool.poetry.group.test.dependencies]
-pytest = "8.1.1"
-coverage = "7.4.4"
+pytest = "8.2.1"
+coverage = "7.5.1"
 pytest-django = "4.8.0"
 freezegun = "^1.2.2"
-pre-commit = "3.7.0"
-tox = "4.14.2"
+pre-commit = "3.7.1"
+tox = "4.15.0"
 tox-gh-actions = "3.2.0"
 factory-boy = "^3.3.0"
 django-shared-property = "^0.8.0"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.5.3"
-pymdown-extensions = "10.7.1"
+mkdocs = "1.6.0"
+pymdown-extensions = "10.8.1"
 mkdocs-mermaid2-plugin = "1.1.1"
 
 [tool.poetry.group.lint.dependencies]
-mypy = "1.9.0"
-django-stubs = "4.2.7"
+mypy = "1.10.0"
+django-stubs = "5.0.0"
 
 [tool.ruff]
 fix = true
 line-length = 120
 extend-exclude = [
     "tests/*",
 ]
```

### Comparing `django_lookup_property-0.1.4/PKG-INFO` & `django_lookup_property-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lookup-property
-Version: 0.1.4
+Version: 0.1.5
 Summary: Django model properties that are also lookup expressions.
 Home-page: https://mrthearman.github.io/django-lookup-property
 License: MIT
 Keywords: django,lookup,property,orm,model,extension
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.11,<4
```

