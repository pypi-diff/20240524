# Comparing `tmp/graphene_django_query_optimizer-0.5.3.tar.gz` & `tmp/graphene_django_query_optimizer-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_django_query_optimizer-0.5.3.tar", max compression
+gzip compressed data, was "graphene_django_query_optimizer-0.5.4.tar", max compression
```

## Comparing `graphene_django_query_optimizer-0.5.3.tar` & `graphene_django_query_optimizer-0.5.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1064 2024-05-10 16:32:46.895758 graphene_django_query_optimizer-0.5.3/LICENSE
--rw-r--r--   0        0        0     3151 2024-05-10 16:32:46.895758 graphene_django_query_optimizer-0.5.3/README.md
--rw-r--r--   0        0        0     6906 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      496 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/__init__.py
--rw-r--r--   0        0        0    11972 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/ast.py
--rw-r--r--   0        0        0     8683 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/compiler.py
--rw-r--r--   0        0        0     2847 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/converters.py
--rw-r--r--   0        0        0      177 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/errors.py
--rw-r--r--   0        0        0    15533 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/fields.py
--rw-r--r--   0        0        0     1686 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/filter.py
--rw-r--r--   0        0        0     5239 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/filter_info.py
--rw-r--r--   0        0        0    10870 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/optimizer.py
--rw-r--r--   0        0        0     4130 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/prefetch_hack.py
--rw-r--r--   0        0        0        0 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/py.typed
--rw-r--r--   0        0        0     3529 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/selections.py
--rw-r--r--   0        0        0     2520 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/settings.py
--rw-r--r--   0        0        0     2996 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/types.py
--rw-r--r--   0        0        0     3661 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/typing.py
--rw-r--r--   0        0        0     6141 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/utils.py
--rw-r--r--   0        0        0     3888 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/validators.py
--rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-24 15:32:13.965833 graphene_django_query_optimizer-0.5.4/LICENSE
+-rw-r--r--   0        0        0     3151 2024-05-24 15:32:13.965833 graphene_django_query_optimizer-0.5.4/README.md
+-rw-r--r--   0        0        0     6906 2024-05-24 15:32:13.965833 graphene_django_query_optimizer-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      496 2024-05-24 15:32:13.965833 graphene_django_query_optimizer-0.5.4/query_optimizer/__init__.py
+-rw-r--r--   0        0        0    11972 2024-05-24 15:32:13.965833 graphene_django_query_optimizer-0.5.4/query_optimizer/ast.py
+-rw-r--r--   0        0        0     8733 2024-05-24 15:32:13.965833 graphene_django_query_optimizer-0.5.4/query_optimizer/compiler.py
+-rw-r--r--   0        0        0     2847 2024-05-24 15:32:13.965833 graphene_django_query_optimizer-0.5.4/query_optimizer/converters.py
+-rw-r--r--   0        0        0      177 2024-05-24 15:32:13.965833 graphene_django_query_optimizer-0.5.4/query_optimizer/errors.py
+-rw-r--r--   0        0        0    15533 2024-05-24 15:32:13.965833 graphene_django_query_optimizer-0.5.4/query_optimizer/fields.py
+-rw-r--r--   0        0        0     1686 2024-05-24 15:32:13.969833 graphene_django_query_optimizer-0.5.4/query_optimizer/filter.py
+-rw-r--r--   0        0        0     5239 2024-05-24 15:32:13.969833 graphene_django_query_optimizer-0.5.4/query_optimizer/filter_info.py
+-rw-r--r--   0        0        0    10870 2024-05-24 15:32:13.969833 graphene_django_query_optimizer-0.5.4/query_optimizer/optimizer.py
+-rw-r--r--   0        0        0     4130 2024-05-24 15:32:13.969833 graphene_django_query_optimizer-0.5.4/query_optimizer/prefetch_hack.py
+-rw-r--r--   0        0        0        0 2024-05-24 15:32:13.969833 graphene_django_query_optimizer-0.5.4/query_optimizer/py.typed
+-rw-r--r--   0        0        0     3529 2024-05-24 15:32:13.969833 graphene_django_query_optimizer-0.5.4/query_optimizer/selections.py
+-rw-r--r--   0        0        0     2520 2024-05-24 15:32:13.969833 graphene_django_query_optimizer-0.5.4/query_optimizer/settings.py
+-rw-r--r--   0        0        0     2996 2024-05-24 15:32:13.969833 graphene_django_query_optimizer-0.5.4/query_optimizer/types.py
+-rw-r--r--   0        0        0     3661 2024-05-24 15:32:13.969833 graphene_django_query_optimizer-0.5.4/query_optimizer/typing.py
+-rw-r--r--   0        0        0     6141 2024-05-24 15:32:13.969833 graphene_django_query_optimizer-0.5.4/query_optimizer/utils.py
+-rw-r--r--   0        0        0     3888 2024-05-24 15:32:13.969833 graphene_django_query_optimizer-0.5.4/query_optimizer/validators.py
+-rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.5.4/PKG-INFO
```

### Comparing `graphene_django_query_optimizer-0.5.3/LICENSE` & `graphene_django_query_optimizer-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.3/README.md` & `graphene_django_query_optimizer-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.3/pyproject.toml` & `graphene_django_query_optimizer-0.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphene-django-query-optimizer"
-version = "0.5.3"
+version = "0.5.4"
 description = "Automatically optimize SQL queries in Graphene-Django schemas."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "query_optimizer" },
 ]
@@ -56,21 +56,21 @@
 typing-extensions = { version = ">=4.7.1", python = "<3.10" }
 django-settings-holder = ">=0.1.2"
 
 [tool.poetry.extras]
 filter = ["django-filter"]
 
 [tool.poetry.group.test.dependencies]
-pytest = "8.2.0"
+pytest = "8.2.1"
 coverage = "7.5.1"
 pytest-django = "4.8.0"
-pre-commit = "3.7.0"
+pre-commit = "3.7.1"
 tox = "4.15.0"
 tox-gh-actions = "3.2.0"
-faker = "25.0.1"
+faker = "25.2.0"
 factory-boy = "3.3.0"
 sqlparse = "0.5.0"
 django-graphiql-debug-toolbar = "0.2.0"
 py-spy = "0.3.14"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.6.0"
```

### Comparing `graphene_django_query_optimizer-0.5.3/query_optimizer/ast.py` & `graphene_django_query_optimizer-0.5.4/query_optimizer/ast.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.3/query_optimizer/compiler.py` & `graphene_django_query_optimizer-0.5.4/query_optimizer/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             self.run()
 
         # Allow known errors to be raised.
         except OptimizerError:  # pragma: no cover
             raise
 
         # Raise unknown errors if not allowed to skip optimization on error.
-        except Exception as error:  # noqa: BLE001  # pragma: no cover
+        except Exception as error:  # pragma: no cover
             optimizer_logger.warning("Something went wrong during the optimization process.", exc_info=error)
             if not optimizer_settings.SKIP_OPTIMIZATION_ON_ERROR:
                 raise
             return None
 
         return self.optimizer
 
@@ -133,17 +133,17 @@
         related_field: ToOneField,
         related_model: type[Model],
     ) -> None:
         name = related_field.get_cache_name() or related_field.name
         optimizer = QueryOptimizer(model=related_model, info=self.info, name=name)
 
         if isinstance(related_field, GenericForeignKey):
-            self.optimizer.prefetch_related[name] = optimizer
+            optimizer = self.optimizer.prefetch_related.setdefault(name, optimizer)
         else:
-            self.optimizer.select_related[name] = optimizer
+            optimizer = self.optimizer.select_related.setdefault(name, optimizer)
 
         if isinstance(related_field, ForeignKey):
             self.optimizer.related_fields.append(related_field.attname)
 
         if isinstance(related_field, GenericForeignKey):
             self.optimizer.related_fields.append(related_field.ct_field)
             self.optimizer.related_fields.append(related_field.fk_field)
@@ -159,15 +159,15 @@
         related_model: type[Model],
     ) -> None:
         name = related_field.get_cache_name() or related_field.name
         key = self.to_attr if self.to_attr is not None else name
         self.to_attr = None
 
         optimizer = QueryOptimizer(model=related_model, info=self.info, name=name)
-        self.optimizer.prefetch_related[key] = optimizer
+        optimizer = self.optimizer.prefetch_related.setdefault(key, optimizer)
 
         if isinstance(related_field, ManyToOneRel):
             optimizer.related_fields.append(related_field.field.attname)
 
         if isinstance(related_field, GenericRelation):
             optimizer.related_fields.append(related_field.object_id_field_name)
             optimizer.related_fields.append(related_field.content_type_field_name)
```

### Comparing `graphene_django_query_optimizer-0.5.3/query_optimizer/converters.py` & `graphene_django_query_optimizer-0.5.4/query_optimizer/converters.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.3/query_optimizer/fields.py` & `graphene_django_query_optimizer-0.5.4/query_optimizer/fields.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.3/query_optimizer/filter.py` & `graphene_django_query_optimizer-0.5.4/query_optimizer/filter.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.3/query_optimizer/filter_info.py` & `graphene_django_query_optimizer-0.5.4/query_optimizer/filter_info.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.3/query_optimizer/optimizer.py` & `graphene_django_query_optimizer-0.5.4/query_optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.3/query_optimizer/prefetch_hack.py` & `graphene_django_query_optimizer-0.5.4/query_optimizer/prefetch_hack.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.3/query_optimizer/selections.py` & `graphene_django_query_optimizer-0.5.4/query_optimizer/selections.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.3/query_optimizer/settings.py` & `graphene_django_query_optimizer-0.5.4/query_optimizer/settings.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.3/query_optimizer/types.py` & `graphene_django_query_optimizer-0.5.4/query_optimizer/types.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.3/query_optimizer/typing.py` & `graphene_django_query_optimizer-0.5.4/query_optimizer/typing.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.3/query_optimizer/utils.py` & `graphene_django_query_optimizer-0.5.4/query_optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.3/query_optimizer/validators.py` & `graphene_django_query_optimizer-0.5.4/query_optimizer/validators.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.3/PKG-INFO` & `graphene_django_query_optimizer-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-query-optimizer
-Version: 0.5.3
+Version: 0.5.4
 Summary: Automatically optimize SQL queries in Graphene-Django schemas.
 Home-page: https://mrthearman.github.io/graphene-django-query-optimizer
 License: MIT
 Keywords: django,graphene,sql,graphql,python,query,optimizer,optimization
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.9,<4
```

