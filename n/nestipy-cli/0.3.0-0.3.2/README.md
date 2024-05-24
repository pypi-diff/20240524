# Comparing `tmp/nestipy_cli-0.3.0.tar.gz` & `tmp/nestipy_cli-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_cli-0.3.0.tar", max compression
+gzip compressed data, was "nestipy_cli-0.3.2.tar", max compression
```

## Comparing `nestipy_cli-0.3.0.tar` & `nestipy_cli-0.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0        0 2024-04-15 07:59:02.892079 nestipy_cli-0.3.0/README.md
--rw-r--r--   0        0        0      646 2024-04-30 15:33:38.634049 nestipy_cli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 17:11:04.969253 nestipy_cli-0.3.0/src/nestipy_cli/__init__.py
--rw-r--r--   0        0        0     2769 2024-04-26 12:11:10.721587 nestipy_cli-0.3.0/src/nestipy_cli/cli.py
--rw-r--r--   0        0        0     5054 2024-04-17 13:42:24.077471 nestipy_cli-0.3.0/src/nestipy_cli/handler.py
--rw-r--r--   0        0        0      502 2024-02-29 12:35:05.153461 nestipy_cli-0.3.0/src/nestipy_cli/style.py
--rw-r--r--   0        0        0        0 2024-04-13 17:11:04.977253 nestipy_cli-0.3.0/src/nestipy_cli/templates/__init__.py
--rw-r--r--   0        0        0      184 2024-04-17 12:09:31.875788 nestipy_cli-0.3.0/src/nestipy_cli/templates/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2906 2024-04-17 12:09:31.875788 nestipy_cli-0.3.0/src/nestipy_cli/templates/__pycache__/generator.cpython-311.pyc
--rw-r--r--   0        0        0     1068 2024-04-13 17:11:04.969253 nestipy_cli-0.3.0/src/nestipy_cli/templates/generator.py
--rw-r--r--   0        0        0       56 2024-04-29 10:08:07.445808 nestipy_cli-0.3.0/src/nestipy_cli/templates/project/.gitignore
--rw-r--r--   0        0        0      988 2024-04-26 13:46:00.142205 nestipy_cli-0.3.0/src/nestipy_cli/templates/project/README.md
--rw-r--r--   0        0        0        0 2024-04-13 17:11:04.977253 nestipy_cli-0.3.0/src/nestipy_cli/templates/project/__init__.py
--rw-r--r--   0        0        0      192 2024-04-22 08:09:23.913452 nestipy_cli-0.3.0/src/nestipy_cli/templates/project/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1301 2024-04-23 14:58:38.932547 nestipy_cli-0.3.0/src/nestipy_cli/templates/project/__pycache__/app_service.cpython-311.pyc
--rw-r--r--   0        0        0      694 2024-04-30 15:25:54.565946 nestipy_cli-0.3.0/src/nestipy_cli/templates/project/app_controller.py
--rw-r--r--   0        0        0      209 2024-04-24 10:34:01.977450 nestipy_cli-0.3.0/src/nestipy_cli/templates/project/app_module.py
--rw-r--r--   0        0        0      374 2024-04-24 10:34:09.977466 nestipy_cli-0.3.0/src/nestipy_cli/templates/project/app_service.py
--rw-r--r--   0        0        0      225 2024-04-24 10:34:14.393474 nestipy_cli-0.3.0/src/nestipy_cli/templates/project/main.py
--rw-r--r--   0        0        0        7 2024-04-30 15:25:05.082362 nestipy_cli-0.3.0/src/nestipy_cli/templates/project/requirements.txt
--rw-r--r--   0        0        0        0 2024-04-13 17:11:04.977253 nestipy_cli-0.3.0/src/nestipy_cli/templates/project/src/__init__.py
--rw-r--r--   0        0        0     1078 2024-04-30 15:26:17.357755 nestipy_cli-0.3.0/src/nestipy_cli/templates/views/controller.txt
--rw-r--r--   0        0        0      187 2024-04-13 17:11:04.969253 nestipy_cli-0.3.0/src/nestipy_cli/templates/views/dto.txt
--rw-r--r--   0        0        0      311 2024-04-13 17:11:04.969253 nestipy_cli-0.3.0/src/nestipy_cli/templates/views/graphql_module.txt
--rw-r--r--   0        0        0      294 2024-04-13 17:11:04.969253 nestipy_cli-0.3.0/src/nestipy_cli/templates/views/graphql_service.txt
--rw-r--r--   0        0        0      102 2024-04-26 08:24:54.367660 nestipy_cli-0.3.0/src/nestipy_cli/templates/views/input.txt
--rw-r--r--   0        0        0      312 2024-04-13 17:11:04.969253 nestipy_cli-0.3.0/src/nestipy_cli/templates/views/module.txt
--rw-r--r--   0        0        0      575 2024-04-30 15:26:29.405654 nestipy_cli-0.3.0/src/nestipy_cli/templates/views/resolver.txt
--rw-r--r--   0        0        0      471 2024-04-17 13:29:07.960343 nestipy_cli-0.3.0/src/nestipy_cli/templates/views/service.txt
--rw-r--r--   0        0        0      168 2024-04-13 17:11:04.969253 nestipy_cli-0.3.0/src/nestipy_cli/templates/views/single_controller.txt
--rw-r--r--   0        0        0       86 2024-04-13 17:11:04.969253 nestipy_cli-0.3.0/src/nestipy_cli/templates/views/single_module.txt
--rw-r--r--   0        0        0      303 2024-04-13 17:11:04.969253 nestipy_cli-0.3.0/src/nestipy_cli/templates/views/single_resolver.txt
--rw-r--r--   0        0        0      127 2024-04-13 17:11:04.969253 nestipy_cli-0.3.0/src/nestipy_cli/templates/views/single_service.txt
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 nestipy_cli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1906 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/README.md
+-rw-r--r--   0        0        0      646 2024-05-24 13:49:57.822062 nestipy_cli-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/__init__.py
+-rw-r--r--   0        0        0     2769 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/cli.py
+-rw-r--r--   0        0        0     5054 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/handler.py
+-rw-r--r--   0        0        0      502 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/style.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2906 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/__pycache__/generator.cpython-311.pyc
+-rw-r--r--   0        0        0     1068 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/generator.py
+-rw-r--r--   0        0        0       56 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/.gitignore
+-rw-r--r--   0        0        0      988 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/__init__.py
+-rw-r--r--   0        0        0      192 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1301 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/__pycache__/app_service.cpython-311.pyc
+-rw-r--r--   0        0        0      805 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/app_controller.py
+-rw-r--r--   0        0        0      209 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/app_module.py
+-rw-r--r--   0        0        0      376 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/app_service.py
+-rw-r--r--   0        0        0      225 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/main.py
+-rw-r--r--   0        0        0        7 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/requirements.txt
+-rw-r--r--   0        0        0        0 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/project/src/__init__.py
+-rw-r--r--   0        0        0     1210 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/controller.txt
+-rw-r--r--   0        0        0      187 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/dto.txt
+-rw-r--r--   0        0        0      311 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/graphql_module.txt
+-rw-r--r--   0        0        0      294 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/graphql_service.txt
+-rw-r--r--   0        0        0      102 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/input.txt
+-rw-r--r--   0        0        0      312 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/module.txt
+-rw-r--r--   0        0        0      618 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/resolver.txt
+-rw-r--r--   0        0        0      471 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/service.txt
+-rw-r--r--   0        0        0      168 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/single_controller.txt
+-rw-r--r--   0        0        0       86 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/single_module.txt
+-rw-r--r--   0        0        0      303 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/single_resolver.txt
+-rw-r--r--   0        0        0      127 2024-05-24 13:49:47.510107 nestipy_cli-0.3.2/src/nestipy_cli/templates/views/single_service.txt
+-rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 nestipy_cli-0.3.2/PKG-INFO
```

### Comparing `nestipy_cli-0.3.0/pyproject.toml` & `nestipy_cli-0.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nestipy-cli"
-version = "0.3.0"
+version = "0.3.2"
 description = "Nestipy is a Python framework built on top of FastAPI that follows the modular architecture of NestJS"
 authors = ["tsiresymila <tsiresymila@gmail.com>"]
 readme = "README.md"
 packages = [{include = "nestipy_cli", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nestipy_cli-0.3.0/src/nestipy_cli/cli.py` & `nestipy_cli-0.3.2/src/nestipy_cli/cli.py`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.3.0/src/nestipy_cli/handler.py` & `nestipy_cli-0.3.2/src/nestipy_cli/handler.py`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.3.0/src/nestipy_cli/templates/__pycache__/generator.cpython-311.pyc` & `nestipy_cli-0.3.2/src/nestipy_cli/templates/__pycache__/generator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.3.0/src/nestipy_cli/templates/generator.py` & `nestipy_cli-0.3.2/src/nestipy_cli/templates/generator.py`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.3.0/src/nestipy_cli/templates/project/README.md` & `nestipy_cli-0.3.2/src/nestipy_cli/templates/project/README.md`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.3.0/src/nestipy_cli/templates/project/__pycache__/app_service.cpython-311.pyc` & `nestipy_cli-0.3.2/src/nestipy_cli/templates/project/__pycache__/app_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy_cli-0.3.0/src/nestipy_cli/templates/project/app_controller.py` & `nestipy_cli-0.3.2/src/nestipy_cli/templates/project/app_controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
+from typing import Annotated
+
 from nestipy.common import Controller, Get, Post, Put, Delete
 from nestipy.ioc import Inject, Body, Params
 
 from app_service import AppService
 
 
 @Controller()
 class AppController:
-    service: Inject[AppService]
+    service: Annotated[AppService, Inject()]
 
     @Get()
     async def get(self) -> str:
         return await self.service.get()
 
     @Post()
-    async def post(self, data: Body[dict]) -> str:
+    async def post(self, data: Annotated[dict, Body()]) -> str:
         return await self.service.post(data=data)
 
     @Put('/{app_id}')
-    async def put(self, app_id: Params[int], data: Body[dict]) -> str:
+    async def put(self, app_id: Annotated[int, Params('app_id')], data: Annotated[dict, Body()]) -> str:
         return await self.service.put(id_=app_id, data=data)
 
     @Delete('/{app_id}')
-    async def delete(self, app_id: Params[int]) -> None:
+    async def delete(self, app_id: Annotated[int, Params('app_id')]) -> None:
         await self.service.delete(id_=app_id)
```

### Comparing `nestipy_cli-0.3.0/src/nestipy_cli/templates/views/controller.txt` & `nestipy_cli-0.3.2/src/nestipy_cli/templates/views/controller.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+from typing import Annotated
+
 from nestipy.common import Controller, Get, Post, Put, Delete
 from nestipy.ioc import Inject, Body, Params
 
 from .{{name|lower}}_dto import Create{{name|capitalize}}Dto, Update{{name|capitalize}}Dto
 from .{{name|lower}}_service import {{name|capitalize}}Service
 
 
 @Controller('{{name|lower}}s')
 class {{name|capitalize}}Controller:
 
-    {{name|lower}}_service:  Inject[{{name|capitalize}}Service]
+    {{name|lower}}_service:  Annotated[{{name|capitalize}}Service, Inject()]
 
     @Get()
     async def list(self) -> str:
         return await self.{{name|lower}}_service.list()
 
     @Post()
-    async def create(self, data: Body[Create{{name|capitalize}}Dto]) -> str:
+    async def create(self, data: Annotated[Create{{name|capitalize}}Dto, Body()]) -> str:
         return await self.{{name|lower}}_service.create(data)
 
     @Put('/{{'{'}}{{name|lower}}{{'_id}'}}')
-    async def update(self, {{name|lower}}_id: Params[int], data: Body[Update{{name|capitalize}}Dto]) -> str:
+    async def update(self, {{name|lower}}_id: Annotated[int, Params('{{name|lower}}_id')], data: Annotated[Update{{name|capitalize}}Dto, Body()]) -> str:
         return await self.{{name|lower}}_service.update({{name|lower}}_id, data)
 
     @Delete('/{{'{'}}{{name|lower}}{{'_id}'}}')
-    async def delete(self, {{name|lower}}_id: Params[int] ) -> None:
+    async def delete(self, {{name|lower}}_id: Annotated[int,Params('{{name|lower}}_id')] ) -> None:
         return await self.{{name|lower}}_service.delete({{name|lower}}_id)
```

### Comparing `nestipy_cli-0.3.0/src/nestipy_cli/templates/views/resolver.txt` & `nestipy_cli-0.3.2/src/nestipy_cli/templates/views/resolver.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from typing import Annotated
+
 from nestipy.graphql import Resolver, Query, Mutation
 from nestipy.ioc import Inject
 
 from .{{name|lower}}_input import {{name|capitalize}}Input
 from .{{name|lower}}_service import {{name|capitalize}}Service
 
 
 @Resolver()
 class {{name|capitalize}}Resolver:
 
-    {{name|lower}}_service: Inject[{{name|capitalize}}Service]
+    {{name|lower}}_service: Annotated[{{name|capitalize}}Service, Inject()]
 
     @Query()
     async def {{name|lower}}_test_query(self) -> str:
         return await self.{{name|lower}}_service.list()
 
     @Mutation()
     async def {{name|lower}}_test_mutation(self,data: {{name|capitalize}}Input) -> str:
```

