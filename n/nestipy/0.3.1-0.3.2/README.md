# Comparing `tmp/nestipy-0.3.1.tar.gz` & `tmp/nestipy-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy-0.3.1.tar", max compression
+gzip compressed data, was "nestipy-0.3.2.tar", max compression
```

## Comparing `nestipy-0.3.1.tar` & `nestipy-0.3.2.tar`

### file list

```diff
@@ -1,204 +1,208 @@
--rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy-0.3.1/LICENSE
--rw-r--r--   0        0        0     1906 2024-04-29 14:09:07.000292 nestipy-0.3.1/README.md
--rw-r--r--   0        0        0      681 2024-04-30 17:15:27.258743 nestipy-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-29 12:35:05.153461 nestipy-0.3.1/src/nestipy/__init__.py
--rw-r--r--   0        0        0     1251 2024-04-30 15:54:16.415653 nestipy-0.3.1/src/nestipy/common/__init__.py
--rw-r--r--   0        0        0     1603 2024-04-30 15:55:15.203159 nestipy-0.3.1/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      652 2024-03-29 11:21:44.572810 nestipy-0.3.1/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
--rw-r--r--   0        0        0      978 2024-04-30 15:13:45.376071 nestipy-0.3.1/src/nestipy/common/config/__init__.py
--rw-r--r--   0        0        0      246 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/decorator/__init__.py
--rw-r--r--   0        0        0     2957 2024-04-30 15:13:45.376071 nestipy-0.3.1/src/nestipy/common/decorator/class_.py
--rw-r--r--   0        0        0     1204 2024-04-30 15:13:45.376071 nestipy-0.3.1/src/nestipy/common/decorator/method.py
--rw-r--r--   0        0        0      367 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/exception/__init__.py
--rw-r--r--   0        0        0      732 2024-04-30 15:13:45.376071 nestipy-0.3.1/src/nestipy/common/exception/decorator.py
--rw-r--r--   0        0        0      433 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/exception/http.py
--rw-r--r--   0        0        0      364 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/exception/interface.py
--rw-r--r--   0        0        0     2531 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/exception/message.py
--rw-r--r--   0        0        0      113 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/exception/meta.py
--rw-r--r--   0        0        0     1686 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/exception/status.py
--rw-r--r--   0        0        0      164 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/guards/__init__.py
--rw-r--r--   0        0        0      326 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/guards/can_activate.py
--rw-r--r--   0        0        0      332 2024-04-30 15:13:45.376071 nestipy-0.3.1/src/nestipy/common/guards/decorator.py
--rw-r--r--   0        0        0       45 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/guards/meta.py
--rw-r--r--   0        0        0      719 2024-04-30 15:13:45.376071 nestipy-0.3.1/src/nestipy/common/helpers/__init__.py
--rw-r--r--   0        0        0      208 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/http_/__init__.py
--rw-r--r--   0        0        0     4503 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/http_/multipart.py
--rw-r--r--   0        0        0     5299 2024-04-30 15:13:45.376071 nestipy-0.3.1/src/nestipy/common/http_/request.py
--rw-r--r--   0        0        0     5321 2024-04-30 15:13:45.376071 nestipy-0.3.1/src/nestipy/common/http_/response.py
--rw-r--r--   0        0        0      478 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/http_/test.py
--rw-r--r--   0        0        0     1403 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/http_/upload_file.py
--rw-r--r--   0        0        0      303 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/http_/websocket.py
--rw-r--r--   0        0        0      199 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/interceptor/__init__.py
--rw-r--r--   0        0        0      489 2024-04-30 15:13:45.376071 nestipy-0.3.1/src/nestipy/common/interceptor/decorator.py
--rw-r--r--   0        0        0      352 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/interceptor/interface.py
--rw-r--r--   0        0        0       52 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/interceptor/meta.py
--rw-r--r--   0        0        0       54 2024-04-30 16:50:58.507079 nestipy-0.3.1/src/nestipy/common/logger.py
--rw-r--r--   0        0        0      248 2024-04-30 15:13:45.376071 nestipy-0.3.1/src/nestipy/common/middleware/__init__.py
--rw-r--r--   0        0        0      695 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/middleware/cors.py
--rw-r--r--   0        0        0      323 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/middleware/interface.py
--rw-r--r--   0        0        0      100 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/middleware/meta.py
--rw-r--r--   0        0        0     3276 2024-04-30 15:13:45.376071 nestipy-0.3.1/src/nestipy/common/middleware/session.py
--rw-r--r--   0        0        0      167 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/template/__init__.py
--rw-r--r--   0        0        0      274 2024-04-30 15:13:45.376071 nestipy-0.3.1/src/nestipy/common/template/decorator.py
--rw-r--r--   0        0        0      627 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/template/interface.py
--rw-r--r--   0        0        0      109 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/common/template/meta.py
--rw-r--r--   0        0        0     1590 2024-04-30 16:48:07.184518 nestipy-0.3.1/src/nestipy/common/utils.py
--rw-r--r--   0        0        0      933 2024-04-29 14:09:07.020292 nestipy-0.3.1/src/nestipy/core/__init__.py
--rw-r--r--   0        0        0     1179 2024-04-29 14:53:26.309598 nestipy-0.3.1/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16492 2024-03-29 11:21:44.576810 nestipy-0.3.1/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
--rw-r--r--   0        0        0     1929 2024-03-29 11:21:44.576810 nestipy-0.3.1/src/nestipy/core/__pycache__/factory.cpython-311.pyc
--rw-r--r--   0        0        0     1567 2024-03-29 11:21:44.576810 nestipy-0.3.1/src/nestipy/core/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0      212 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/core/adapter/__init__.py
--rw-r--r--   0        0        0     4224 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/core/adapter/blacksheep_adapter.py
--rw-r--r--   0        0        0     3803 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/core/adapter/fastapi_adapter.py
--rw-r--r--   0        0        0     5666 2024-04-30 15:13:45.376071 nestipy-0.3.1/src/nestipy/core/adapter/http_adapter.py
--rw-r--r--   0        0        0      418 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/core/constant.py
--rw-r--r--   0        0        0        0 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/core/context/__init__.py
--rw-r--r--   0        0        0     1250 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/core/context/argument_host.py
--rw-r--r--   0        0        0      802 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/core/context/execution_context.py
--rw-r--r--   0        0        0      369 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/core/context/http_argument_host.py
--rw-r--r--   0        0        0      730 2024-04-29 14:09:07.020292 nestipy-0.3.1/src/nestipy/core/discover.py
--rw-r--r--   0        0        0       90 2024-04-26 12:17:55.156372 nestipy-0.3.1/src/nestipy/core/exception/__init__.py
--rw-r--r--   0        0        0     4040 2024-04-30 15:13:45.376071 nestipy-0.3.1/src/nestipy/core/exception/processor.py
--rw-r--r--   0        0        0       75 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/core/guards/__init__.py
--rw-r--r--   0        0        0     2164 2024-04-30 15:13:45.376071 nestipy-0.3.1/src/nestipy/core/guards/processor.py
--rw-r--r--   0        0        0     3847 2024-04-30 15:13:45.376071 nestipy-0.3.1/src/nestipy/core/instance_loader.py
--rw-r--r--   0        0        0       82 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/core/interceptor/__init__.py
--rw-r--r--   0        0        0     2569 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/core/interceptor/processor.py
--rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/core/meta/__init__.py
--rw-r--r--   0        0        0      380 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/core/meta/controller_metadata_creator.py
--rw-r--r--   0        0        0     4040 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/core/meta/metadata_creator.py
--rw-r--r--   0        0        0      771 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/core/meta/module_metadata_creator.py
--rw-r--r--   0        0        0      374 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/core/meta/provider_metadata_creator.py
--rw-r--r--   0        0        0      162 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/core/middleware/__init__.py
--rw-r--r--   0        0        0     3949 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/core/middleware/executor.py
--rw-r--r--   0        0        0     8889 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/core/nestipy_application.py
--rw-r--r--   0        0        0     1249 2024-04-30 16:48:01.700564 nestipy-0.3.1/src/nestipy/core/nestipy_factory.py
--rw-r--r--   0        0        0       64 2024-04-29 14:09:07.020292 nestipy-0.3.1/src/nestipy/core/on_destroy.py
--rw-r--r--   0        0        0       60 2024-04-29 14:09:07.020292 nestipy-0.3.1/src/nestipy/core/on_init.py
--rw-r--r--   0        0        0       89 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/core/platform/__init__.py
--rw-r--r--   0        0        0      608 2024-04-29 14:09:07.020292 nestipy-0.3.1/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3199 2024-03-29 11:21:44.576810 nestipy-0.3.1/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
--rw-r--r--   0        0        0     7185 2024-03-29 11:21:44.576810 nestipy-0.3.1/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
--rw-r--r--   0        0        0     7397 2024-03-29 11:21:44.576810 nestipy-0.3.1/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/core/router/__init__.py
--rw-r--r--   0        0        0     2879 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/core/router/route_explorer.py
--rw-r--r--   0        0        0      510 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/core/router/route_extractor.py
--rw-r--r--   0        0        0     8298 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/core/router/router_proxy.py
--rw-r--r--   0        0        0      184 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/core/template/__init__.py
--rw-r--r--   0        0        0     1004 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/core/template/minimal_jinja.py
--rw-r--r--   0        0        0     1457 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/core/template/processor.py
--rw-r--r--   0        0        0      231 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/dynamic_module/__init__.py
--rw-r--r--   0        0        0     3512 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/dynamic_module/builder.py
--rw-r--r--   0        0        0      139 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/dynamic_module/module/__init__.py
--rw-r--r--   0        0        0      517 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/dynamic_module/module/consumer.py
--rw-r--r--   0        0        0      251 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/dynamic_module/module/interface.py
--rw-r--r--   0        0        0      282 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/graphql/__init__.py
--rw-r--r--   0        0        0     1533 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/graphql/decorator.py
--rw-r--r--   0        0        0     2244 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/graphql/graphql_adapter.py
--rw-r--r--   0        0        0     1111 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/graphql/graphql_asgi.py
--rw-r--r--   0        0        0     1871 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/graphql/graphql_explorer.py
--rw-r--r--   0        0        0      547 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/graphql/graphql_module.py
--rw-r--r--   0        0        0     4326 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/graphql/graphql_proxy.py
--rw-r--r--   0        0        0      289 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/graphql/meta.py
--rw-r--r--   0        0        0     1531 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/graphql/playground/graphql-playground-default.html
--rw-r--r--   0        0        0     3486 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/graphql/playground/graphql-playground-graphiql.html
--rw-r--r--   0        0        0      704 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/graphql/pubsub.py
--rw-r--r--   0        0        0      648 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/graphql/strawberry/__init__.py
--rw-r--r--   0        0        0     2103 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/graphql/strawberry/strawberry_adapter.py
--rw-r--r--   0        0        0     1588 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/graphql/strawberry/strawberry_asgi.py
--rw-r--r--   0        0        0      110 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/graphql/test.py
--rw-r--r--   0        0        0      952 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/ioc/__init__.py
--rw-r--r--   0        0        0      122 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/ioc/annotation.py
--rw-r--r--   0        0        0    14115 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/ioc/container.py
--rw-r--r--   0        0        0     1485 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/ioc/context_container.py
--rw-r--r--   0        0        0     2054 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/ioc/dependency.py
--rw-r--r--   0        0        0      885 2024-04-30 15:13:45.380071 nestipy-0.3.1/src/nestipy/ioc/meta.py
--rw-r--r--   0        0        0     3013 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/ioc/middleware.py
--rw-r--r--   0        0        0      877 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/ioc/provider.py
--rw-r--r--   0        0        0       56 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/ioc/utils.py
--rw-r--r--   0        0        0      458 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/metadata/__init__.py
--rw-r--r--   0        0        0     1673 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/metadata/class_.py
--rw-r--r--   0        0        0      508 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/metadata/container.py
--rw-r--r--   0        0        0      710 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/metadata/decorator.py
--rw-r--r--   0        0        0     1004 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/metadata/dependency.py
--rw-r--r--   0        0        0      236 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/metadata/module.py
--rw-r--r--   0        0        0       88 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/metadata/provider_token.py
--rw-r--r--   0        0        0      688 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/metadata/reflect.py
--rw-r--r--   0        0        0      107 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/metadata/route.py
--rw-r--r--   0        0        0     1105 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/openapi/__init__.py
--rw-r--r--   0        0        0       49 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/openapi/constant.py
--rw-r--r--   0        0        0     3144 2024-04-30 17:05:28.231774 nestipy-0.3.1/src/nestipy/openapi/decorator.py
--rw-r--r--   0        0        0     1587 2024-04-30 17:05:35.335715 nestipy-0.3.1/src/nestipy/openapi/document_builder.py
--rw-r--r--   0        0        0      423 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/openapi/explorer.py
--rw-r--r--   0        0        0       44 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/__init__.py
--rw-r--r--   0        0        0     4684 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/common.py
--rw-r--r--   0        0        0     1325 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/__init__.py
--rw-r--r--   0        0        0     1757 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/common.py
--rw-r--r--   0        0        0     1855 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/contents.py
--rw-r--r--   0        0        0      633 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/generate.py
--rw-r--r--   0        0        0     3196 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/jinja.py
--rw-r--r--   0        0        0     1894 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/md.py
--rw-r--r--   0        0        0     3065 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/texts.py
--rw-r--r--   0        0        0    21375 2024-04-30 15:13:45.384071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py
--rw-r--r--   0        0        0     4250 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/examples.py
--rw-r--r--   0        0        0      103 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/README.md
--rw-r--r--   0        0        0        0 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/__init__.py
--rw-r--r--   0        0        0      890 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html
--rw-r--r--   0        0        0      610 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html
--rw-r--r--   0        0        0      730 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html
--rw-r--r--   0        0        0      135 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-schemas.html
--rw-r--r--   0        0        0      322 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-security-schemes.html
--rw-r--r--   0        0        0      284 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/content-examples.html
--rw-r--r--   0        0        0      207 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/external-docs.html
--rw-r--r--   0        0        0      571 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html
--rw-r--r--   0        0        0      873 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html
--rw-r--r--   0        0        0        0 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-auth.html
--rw-r--r--   0        0        0      480 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-body.html
--rw-r--r--   0        0        0      492 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-parameters.html
--rw-r--r--   0        0        0     1335 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html
--rw-r--r--   0        0        0      929 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html
--rw-r--r--   0        0        0      224 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/servers.html
--rw-r--r--   0        0        0      227 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/tags.html
--rw-r--r--   0        0        0      429 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/type.html
--rw-r--r--   0        0        0      286 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/README.md
--rw-r--r--   0        0        0        0 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/__init__.py
--rw-r--r--   0        0        0      889 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html
--rw-r--r--   0        0        0      933 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html
--rw-r--r--   0        0        0      843 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html
--rw-r--r--   0        0        0      135 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-schemas.html
--rw-r--r--   0        0        0      561 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html
--rw-r--r--   0        0        0      383 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/content-examples.html
--rw-r--r--   0        0        0      326 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/external-docs.html
--rw-r--r--   0        0        0      817 2024-04-30 15:13:45.388071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html
--rw-r--r--   0        0        0     1007 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html
--rw-r--r--   0        0        0        0 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-auth.html
--rw-r--r--   0        0        0      616 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html
--rw-r--r--   0        0        0      857 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html
--rw-r--r--   0        0        0     2250 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html
--rw-r--r--   0        0        0     1155 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html
--rw-r--r--   0        0        0      475 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/servers.html
--rw-r--r--   0        0        0      227 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/tags.html
--rw-r--r--   0        0        0      638 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html
--rw-r--r--   0        0        0      170 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/README.md
--rw-r--r--   0        0        0      548 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html
--rw-r--r--   0        0        0      670 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html
--rw-r--r--   0        0        0      156 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/README.md
--rw-r--r--   0        0        0      754 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html
--rw-r--r--   0        0        0      670 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html
--rw-r--r--   0        0        0        0 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/utils/__init__.py
--rw-r--r--   0        0        0     2844 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/utils/source.py
--rw-r--r--   0        0        0      878 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/utils/web.py
--rw-r--r--   0        0        0     9579 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/v2.py
--rw-r--r--   0        0        0     9667 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/openapi_docs/v3.py
--rw-r--r--   0        0        0     1323 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/openapi/swagger.html
--rw-r--r--   0        0        0     2653 2024-04-30 17:14:39.787142 nestipy-0.3.1/src/nestipy/openapi/swagger_module.py
--rw-r--r--   0        0        0     2676 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/openapi/test.py
--rw-r--r--   0        0        0      220 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/types_/__init__.py
--rw-r--r--   0        0        0      393 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/types_/handler.py
--rw-r--r--   0        0        0      123 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/types_/http.py
--rw-r--r--   0        0        0      254 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/websocket/__init__.py
--rw-r--r--   0        0        0     2988 2024-04-26 12:17:55.160372 nestipy-0.3.1/src/nestipy/websocket/adapter.py
--rw-r--r--   0        0        0      716 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/websocket/decorator.py
--rw-r--r--   0        0        0     4517 2024-04-30 15:13:45.392071 nestipy-0.3.1/src/nestipy/websocket/proxy.py
--rw-r--r--   0        0        0     2846 1970-01-01 00:00:00.000000 nestipy-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-05-24 11:55:00.229333 nestipy-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1906 2024-05-24 11:55:00.229333 nestipy-0.3.2/README.md
+-rw-r--r--   0        0        0      681 2024-05-24 11:55:11.617379 nestipy-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/__init__.py
+-rw-r--r--   0        0        0     1489 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      652 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
+-rw-r--r--   0        0        0     1005 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/config/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/decorator/__init__.py
+-rw-r--r--   0        0        0     2957 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/decorator/class_.py
+-rw-r--r--   0        0        0     1204 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/decorator/method.py
+-rw-r--r--   0        0        0      367 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/exception/__init__.py
+-rw-r--r--   0        0        0      732 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/exception/decorator.py
+-rw-r--r--   0        0        0      433 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/exception/http.py
+-rw-r--r--   0        0        0      364 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/exception/interface.py
+-rw-r--r--   0        0        0     2531 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/exception/message.py
+-rw-r--r--   0        0        0      113 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/exception/meta.py
+-rw-r--r--   0        0        0     1686 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/exception/status.py
+-rw-r--r--   0        0        0      164 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/guards/__init__.py
+-rw-r--r--   0        0        0      326 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/guards/can_activate.py
+-rw-r--r--   0        0        0      332 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/guards/decorator.py
+-rw-r--r--   0        0        0       45 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/guards/meta.py
+-rw-r--r--   0        0        0      719 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/helpers/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/http_/__init__.py
+-rw-r--r--   0        0        0     4503 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/http_/multipart.py
+-rw-r--r--   0        0        0     5299 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/http_/request.py
+-rw-r--r--   0        0        0     5321 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/http_/response.py
+-rw-r--r--   0        0        0      478 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/http_/test.py
+-rw-r--r--   0        0        0     1403 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/http_/upload_file.py
+-rw-r--r--   0        0        0      303 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/http_/websocket.py
+-rw-r--r--   0        0        0      199 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/interceptor/__init__.py
+-rw-r--r--   0        0        0      489 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/interceptor/decorator.py
+-rw-r--r--   0        0        0      352 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/interceptor/interface.py
+-rw-r--r--   0        0        0       52 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/interceptor/meta.py
+-rw-r--r--   0        0        0       54 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/logger.py
+-rw-r--r--   0        0        0      248 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/middleware/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/middleware/cors.py
+-rw-r--r--   0        0        0      323 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/middleware/interface.py
+-rw-r--r--   0        0        0      100 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/middleware/meta.py
+-rw-r--r--   0        0        0     3276 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/middleware/session.py
+-rw-r--r--   0        0        0      167 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/template/__init__.py
+-rw-r--r--   0        0        0      274 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/template/decorator.py
+-rw-r--r--   0        0        0      627 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/template/interface.py
+-rw-r--r--   0        0        0      109 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/template/meta.py
+-rw-r--r--   0        0        0     1590 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/common/utils.py
+-rw-r--r--   0        0        0      933 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/core/__init__.py
+-rw-r--r--   0        0        0     1179 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16492 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
+-rw-r--r--   0        0        0     1929 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/core/__pycache__/factory.cpython-311.pyc
+-rw-r--r--   0        0        0     1567 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/core/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0      212 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/core/adapter/__init__.py
+-rw-r--r--   0        0        0     4224 2024-05-24 11:55:00.257334 nestipy-0.3.2/src/nestipy/core/adapter/blacksheep_adapter.py
+-rw-r--r--   0        0        0     3803 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/adapter/fastapi_adapter.py
+-rw-r--r--   0        0        0     5666 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/adapter/http_adapter.py
+-rw-r--r--   0        0        0      418 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/constant.py
+-rw-r--r--   0        0        0        0 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/context/__init__.py
+-rw-r--r--   0        0        0     1741 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/context/argument_host.py
+-rw-r--r--   0        0        0     1613 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/context/execution_context.py
+-rw-r--r--   0        0        0      526 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/context/graphql_argument_host.py
+-rw-r--r--   0        0        0      369 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/context/http_argument_host.py
+-rw-r--r--   0        0        0      556 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/context/websocket_argument_host.py
+-rw-r--r--   0        0        0      730 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/discover.py
+-rw-r--r--   0        0        0       90 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/exception/__init__.py
+-rw-r--r--   0        0        0     4040 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/exception/processor.py
+-rw-r--r--   0        0        0       75 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/guards/__init__.py
+-rw-r--r--   0        0        0     2164 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/guards/processor.py
+-rw-r--r--   0        0        0     3847 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/instance_loader.py
+-rw-r--r--   0        0        0       82 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/interceptor/__init__.py
+-rw-r--r--   0        0        0     2569 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/interceptor/processor.py
+-rw-r--r--   0        0        0        0 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/meta/__init__.py
+-rw-r--r--   0        0        0      380 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/meta/controller_metadata_creator.py
+-rw-r--r--   0        0        0     4040 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/meta/metadata_creator.py
+-rw-r--r--   0        0        0      771 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/meta/module_metadata_creator.py
+-rw-r--r--   0        0        0      374 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/meta/provider_metadata_creator.py
+-rw-r--r--   0        0        0      162 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/middleware/__init__.py
+-rw-r--r--   0        0        0     3973 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/middleware/executor.py
+-rw-r--r--   0        0        0     8913 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/nestipy_application.py
+-rw-r--r--   0        0        0     1317 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/nestipy_factory.py
+-rw-r--r--   0        0        0       64 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/on_destroy.py
+-rw-r--r--   0        0        0       60 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/on_init.py
+-rw-r--r--   0        0        0       89 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/platform/__init__.py
+-rw-r--r--   0        0        0      608 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3199 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
+-rw-r--r--   0        0        0     7185 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
+-rw-r--r--   0        0        0     7397 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/router/__init__.py
+-rw-r--r--   0        0        0     2879 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/router/route_explorer.py
+-rw-r--r--   0        0        0      510 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/router/route_extractor.py
+-rw-r--r--   0        0        0     7343 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/router/router_proxy.py
+-rw-r--r--   0        0        0      184 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/template/__init__.py
+-rw-r--r--   0        0        0     1004 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/template/minimal_jinja.py
+-rw-r--r--   0        0        0     1457 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/core/template/processor.py
+-rw-r--r--   0        0        0      231 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/dynamic_module/__init__.py
+-rw-r--r--   0        0        0     3512 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/dynamic_module/builder.py
+-rw-r--r--   0        0        0      139 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/dynamic_module/module/__init__.py
+-rw-r--r--   0        0        0      517 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/dynamic_module/module/consumer.py
+-rw-r--r--   0        0        0      251 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/dynamic_module/module/interface.py
+-rw-r--r--   0        0        0      282 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/graphql/__init__.py
+-rw-r--r--   0        0        0     1533 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/graphql/decorator.py
+-rw-r--r--   0        0        0     2244 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/graphql/graphql_adapter.py
+-rw-r--r--   0        0        0     1111 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/graphql/graphql_asgi.py
+-rw-r--r--   0        0        0     1871 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/graphql/graphql_explorer.py
+-rw-r--r--   0        0        0      584 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/graphql/graphql_module.py
+-rw-r--r--   0        0        0     4502 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/graphql/graphql_proxy.py
+-rw-r--r--   0        0        0      289 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/graphql/meta.py
+-rw-r--r--   0        0        0     1531 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/graphql/playground/graphql-playground-default.html
+-rw-r--r--   0        0        0     3486 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/graphql/playground/graphql-playground-graphiql.html
+-rw-r--r--   0        0        0      704 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/graphql/pubsub.py
+-rw-r--r--   0        0        0      648 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/graphql/strawberry/__init__.py
+-rw-r--r--   0        0        0     2103 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/graphql/strawberry/strawberry_adapter.py
+-rw-r--r--   0        0        0     1588 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/graphql/strawberry/strawberry_asgi.py
+-rw-r--r--   0        0        0      110 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/graphql/test.py
+-rw-r--r--   0        0        0      850 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/ioc/__init__.py
+-rw-r--r--   0        0        0      444 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/ioc/annotation.py
+-rw-r--r--   0        0        0    11437 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/ioc/container.py
+-rw-r--r--   0        0        0     1047 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/ioc/context_container.py
+-rw-r--r--   0        0        0     5062 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/ioc/dependency.py
+-rw-r--r--   0        0        0      663 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/ioc/meta.py
+-rw-r--r--   0        0        0     3013 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/ioc/middleware.py
+-rw-r--r--   0        0        0      877 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/ioc/provider.py
+-rw-r--r--   0        0        0      409 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/ioc/test.py
+-rw-r--r--   0        0        0       56 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/ioc/utils.py
+-rw-r--r--   0        0        0      458 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/metadata/__init__.py
+-rw-r--r--   0        0        0     1673 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/metadata/class_.py
+-rw-r--r--   0        0        0      508 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/metadata/container.py
+-rw-r--r--   0        0        0      710 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/metadata/decorator.py
+-rw-r--r--   0        0        0     1004 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/metadata/dependency.py
+-rw-r--r--   0        0        0      236 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/metadata/module.py
+-rw-r--r--   0        0        0       88 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/metadata/provider_token.py
+-rw-r--r--   0        0        0      688 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/metadata/reflect.py
+-rw-r--r--   0        0        0      107 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/metadata/route.py
+-rw-r--r--   0        0        0     1105 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/openapi/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/openapi/constant.py
+-rw-r--r--   0        0        0     3144 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/openapi/decorator.py
+-rw-r--r--   0        0        0     1587 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/openapi/document_builder.py
+-rw-r--r--   0        0        0      423 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/openapi/explorer.py
+-rw-r--r--   0        0        0       44 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/__init__.py
+-rw-r--r--   0        0        0     4684 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/common.py
+-rw-r--r--   0        0        0     1325 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/__init__.py
+-rw-r--r--   0        0        0     1757 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/common.py
+-rw-r--r--   0        0        0     1855 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/contents.py
+-rw-r--r--   0        0        0      633 2024-05-24 11:55:00.261334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/generate.py
+-rw-r--r--   0        0        0     3196 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/jinja.py
+-rw-r--r--   0        0        0     1894 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/md.py
+-rw-r--r--   0        0        0     3065 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/texts.py
+-rw-r--r--   0        0        0    21375 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py
+-rw-r--r--   0        0        0     4250 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/examples.py
+-rw-r--r--   0        0        0      103 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/__init__.py
+-rw-r--r--   0        0        0      890 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html
+-rw-r--r--   0        0        0      610 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html
+-rw-r--r--   0        0        0      730 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html
+-rw-r--r--   0        0        0      135 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-schemas.html
+-rw-r--r--   0        0        0      322 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-security-schemes.html
+-rw-r--r--   0        0        0      284 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/content-examples.html
+-rw-r--r--   0        0        0      207 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/external-docs.html
+-rw-r--r--   0        0        0      571 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html
+-rw-r--r--   0        0        0      873 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html
+-rw-r--r--   0        0        0        0 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-auth.html
+-rw-r--r--   0        0        0      480 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-body.html
+-rw-r--r--   0        0        0      492 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-parameters.html
+-rw-r--r--   0        0        0     1335 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html
+-rw-r--r--   0        0        0      929 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html
+-rw-r--r--   0        0        0      224 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/servers.html
+-rw-r--r--   0        0        0      227 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/tags.html
+-rw-r--r--   0        0        0      429 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/type.html
+-rw-r--r--   0        0        0      286 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/__init__.py
+-rw-r--r--   0        0        0      889 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html
+-rw-r--r--   0        0        0      933 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html
+-rw-r--r--   0        0        0      843 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html
+-rw-r--r--   0        0        0      135 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-schemas.html
+-rw-r--r--   0        0        0      561 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html
+-rw-r--r--   0        0        0      383 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/content-examples.html
+-rw-r--r--   0        0        0      326 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/external-docs.html
+-rw-r--r--   0        0        0      817 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html
+-rw-r--r--   0        0        0     1007 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html
+-rw-r--r--   0        0        0        0 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-auth.html
+-rw-r--r--   0        0        0      616 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html
+-rw-r--r--   0        0        0      857 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html
+-rw-r--r--   0        0        0     2250 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html
+-rw-r--r--   0        0        0     1155 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html
+-rw-r--r--   0        0        0      475 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/servers.html
+-rw-r--r--   0        0        0      227 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/tags.html
+-rw-r--r--   0        0        0      638 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html
+-rw-r--r--   0        0        0      170 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/README.md
+-rw-r--r--   0        0        0      548 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html
+-rw-r--r--   0        0        0      670 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html
+-rw-r--r--   0        0        0      156 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/README.md
+-rw-r--r--   0        0        0      754 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html
+-rw-r--r--   0        0        0      670 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html
+-rw-r--r--   0        0        0        0 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/utils/__init__.py
+-rw-r--r--   0        0        0     2844 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/utils/source.py
+-rw-r--r--   0        0        0      878 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/utils/web.py
+-rw-r--r--   0        0        0     9579 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/v2.py
+-rw-r--r--   0        0        0     9667 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/openapi_docs/v3.py
+-rw-r--r--   0        0        0     1323 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/swagger.html
+-rw-r--r--   0        0        0     2653 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/swagger_module.py
+-rw-r--r--   0        0        0     2676 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/openapi/test.py
+-rw-r--r--   0        0        0      220 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/types_/__init__.py
+-rw-r--r--   0        0        0      393 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/types_/handler.py
+-rw-r--r--   0        0        0      123 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/types_/http.py
+-rw-r--r--   0        0        0      254 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/websocket/__init__.py
+-rw-r--r--   0        0        0     3068 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/websocket/adapter.py
+-rw-r--r--   0        0        0      716 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/websocket/decorator.py
+-rw-r--r--   0        0        0     4615 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/websocket/proxy.py
+-rw-r--r--   0        0        0      168 2024-05-24 11:55:00.265334 nestipy-0.3.2/src/nestipy/websocket/socket_request.py
+-rw-r--r--   0        0        0     2846 1970-01-01 00:00:00.000000 nestipy-0.3.2/PKG-INFO
```

### Comparing `nestipy-0.3.1/LICENSE` & `nestipy-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/README.md` & `nestipy-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/pyproject.toml` & `nestipy-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nestipy"
-version = "0.3.1"
+version = "0.3.2"
 description = "Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS"
 authors = ["tsiresymila <tsiresymila@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "nestipy", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nestipy-0.3.1/src/nestipy/common/__init__.py` & `nestipy-0.3.2/src/nestipy/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/common/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.3.2/src/nestipy/common/__pycache__/__init__.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,43 +1,43 @@
 magic:    0xa70d0d0a
-moddate:  0x28143166 (Tue Apr 30 15:54:16 2024 UTC)
-files sz: 1251
+moddate:  0x739b2b66 (Fri Apr 26 12:17:55 2024 UTC)
+files sz: 1151
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a010100640264036c026d035a036d045a0401
       00640264046c056d065a066d075a076d085a086d095a096d0a5a0a6d0b5a
       0b6d0c5a0c6d0d5a0d6d0e5a0e0100640264056c0f6d105a106d115a116d
       125a126d135a136d145a146d155a156d165a160100640264066c176d185a
       186d195a190100640264076c1a6d1b5a1b6d1c5a1c6d1d5a1d6d1e5a1e01
-      00640264086c1f6d205a206d215a210100640264096c226d225a22010064
-      02640a6c236d245a246d255a256d265a266d275a2701006402640b6c286d
-      295a296d2a5a2a01006700640ca2015a2b640d5300
+      00640264086c1f6d205a206d215a210100640264096c226d235a236d245a
+      2401006402640a6c256d265a266d275a2701006700640ba2015a28640c53
+      00
      0           0 RESUME                   0
    
      2           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('ModuleProviderDict',))
-                 6 IMPORT_NAME              0 (nestipy.ioc)
+                 6 IMPORT_NAME              0 (nestipy_ioc)
                  8 IMPORT_FROM              1 (ModuleProviderDict)
                 10 STORE_NAME               1 (ModuleProviderDict)
                 12 POP_TOP
    
-     3          14 LOAD_CONST               2 (1)
+     4          14 LOAD_CONST               2 (1)
                 16 LOAD_CONST               3 (('ConfigModule', 'ConfigService'))
                 18 IMPORT_NAME              2 (config)
                 20 IMPORT_FROM              3 (ConfigModule)
                 22 STORE_NAME               3 (ConfigModule)
                 24 IMPORT_FROM              4 (ConfigService)
                 26 STORE_NAME               4 (ConfigService)
                 28 POP_TOP
    
-     4          30 LOAD_CONST               2 (1)
+     5          30 LOAD_CONST               2 (1)
                 32 LOAD_CONST               4 (('Module', 'Controller', 'Injectable', 'Route', 'Get', 'Post', 'Patch', 'Put', 'Delete'))
                 34 IMPORT_NAME              5 (decorator)
                 36 IMPORT_FROM              6 (Module)
                 38 STORE_NAME               6 (Module)
                 40 IMPORT_FROM              7 (Controller)
                 42 STORE_NAME               7 (Controller)
                 44 IMPORT_FROM              8 (Injectable)
@@ -52,15 +52,15 @@
                 62 STORE_NAME              12 (Patch)
                 64 IMPORT_FROM             13 (Put)
                 66 STORE_NAME              13 (Put)
                 68 IMPORT_FROM             14 (Delete)
                 70 STORE_NAME              14 (Delete)
                 72 POP_TOP
    
-     5          74 LOAD_CONST               2 (1)
+     6          74 LOAD_CONST               2 (1)
                 76 LOAD_CONST               5 (('HttpException', 'HttpStatusMessages', 'HttpStatus', 'UseFilters', 'Catch', 'ExceptionKey', 'ExceptionFilter'))
                 78 IMPORT_NAME             15 (exception)
                 80 IMPORT_FROM             16 (HttpException)
                 82 STORE_NAME              16 (HttpException)
                 84 IMPORT_FROM             17 (HttpStatusMessages)
                 86 STORE_NAME              17 (HttpStatusMessages)
                 88 IMPORT_FROM             18 (HttpStatus)
@@ -71,96 +71,84 @@
                 98 STORE_NAME              20 (Catch)
                100 IMPORT_FROM             21 (ExceptionKey)
                102 STORE_NAME              21 (ExceptionKey)
                104 IMPORT_FROM             22 (ExceptionFilter)
                106 STORE_NAME              22 (ExceptionFilter)
                108 POP_TOP
    
-     6         110 LOAD_CONST               2 (1)
+     7         110 LOAD_CONST               2 (1)
                112 LOAD_CONST               6 (('CanActivate', 'UseGuards'))
                114 IMPORT_NAME             23 (guards)
                116 IMPORT_FROM             24 (CanActivate)
                118 STORE_NAME              24 (CanActivate)
                120 IMPORT_FROM             25 (UseGuards)
                122 STORE_NAME              25 (UseGuards)
                124 POP_TOP
    
-     7         126 LOAD_CONST               2 (1)
+     8         126 LOAD_CONST               2 (1)
                128 LOAD_CONST               7 (('Request', 'Response', 'Websocket', 'UploadFile'))
                130 IMPORT_NAME             26 (http_)
                132 IMPORT_FROM             27 (Request)
                134 STORE_NAME              27 (Request)
                136 IMPORT_FROM             28 (Response)
                138 STORE_NAME              28 (Response)
                140 IMPORT_FROM             29 (Websocket)
                142 STORE_NAME              29 (Websocket)
                144 IMPORT_FROM             30 (UploadFile)
                146 STORE_NAME              30 (UploadFile)
                148 POP_TOP
    
-     8         150 LOAD_CONST               2 (1)
+     9         150 LOAD_CONST               2 (1)
                152 LOAD_CONST               8 (('NestipyInterceptor', 'UseInterceptors'))
                154 IMPORT_NAME             31 (interceptor)
                156 IMPORT_FROM             32 (NestipyInterceptor)
                158 STORE_NAME              32 (NestipyInterceptor)
                160 IMPORT_FROM             33 (UseInterceptors)
                162 STORE_NAME              33 (UseInterceptors)
                164 POP_TOP
    
-     9         166 LOAD_CONST               2 (1)
-               168 LOAD_CONST               9 (('logger',))
-               170 IMPORT_NAME             34 (logger)
-               172 IMPORT_FROM             34 (logger)
-               174 STORE_NAME              34 (logger)
-               176 POP_TOP
-   
-    10         178 LOAD_CONST               2 (1)
-               180 LOAD_CONST              10 (('cors', 'NestipyMiddleware', 'session', 'SessionOption'))
-               182 IMPORT_NAME             35 (middleware)
-               184 IMPORT_FROM             36 (cors)
-               186 STORE_NAME              36 (cors)
-               188 IMPORT_FROM             37 (NestipyMiddleware)
-               190 STORE_NAME              37 (NestipyMiddleware)
-               192 IMPORT_FROM             38 (session)
-               194 STORE_NAME              38 (session)
-               196 IMPORT_FROM             39 (SessionOption)
-               198 STORE_NAME              39 (SessionOption)
-               200 POP_TOP
-   
-    11         202 LOAD_CONST               2 (1)
-               204 LOAD_CONST              11 (('Render', 'TemplateEngine'))
-               206 IMPORT_NAME             40 (template)
-               208 IMPORT_FROM             41 (Render)
-               210 STORE_NAME              41 (Render)
-               212 IMPORT_FROM             42 (TemplateEngine)
-               214 STORE_NAME              42 (TemplateEngine)
-               216 POP_TOP
-   
-    13         218 BUILD_LIST               0
-               220 LOAD_CONST              12 (('ConfigModule', 'ConfigService', 'Module', 'Controller', 'Injectable', 'Route', 'Get', 'Post', 'Put', 'Patch', 'Delete', 'HttpException', 'HttpStatusMessages', 'HttpStatus', 'UseFilters', 'Catch', 'ExceptionKey', 'ExceptionFilter', 'CanActivate', 'UseGuards', 'Response', 'Request', 'Websocket', 'UploadFile', 'NestipyInterceptor', 'UseInterceptors', 'cors', 'NestipyMiddleware', 'Render', 'TemplateEngine', 'ModuleProviderDict', 'session', 'SessionOption', 'logger'))
-               222 LIST_EXTEND              1
-               224 STORE_NAME              43 (__all__)
-               226 LOAD_CONST              13 (None)
-               228 RETURN_VALUE
+    10         166 LOAD_CONST               2 (1)
+               168 LOAD_CONST               9 (('cors', 'NestipyMiddleware'))
+               170 IMPORT_NAME             34 (middleware)
+               172 IMPORT_FROM             35 (cors)
+               174 STORE_NAME              35 (cors)
+               176 IMPORT_FROM             36 (NestipyMiddleware)
+               178 STORE_NAME              36 (NestipyMiddleware)
+               180 POP_TOP
+   
+    11         182 LOAD_CONST               2 (1)
+               184 LOAD_CONST              10 (('Render', 'TemplateEngine'))
+               186 IMPORT_NAME             37 (template)
+               188 IMPORT_FROM             38 (Render)
+               190 STORE_NAME              38 (Render)
+               192 IMPORT_FROM             39 (TemplateEngine)
+               194 STORE_NAME              39 (TemplateEngine)
+               196 POP_TOP
+   
+    13         198 BUILD_LIST               0
+               200 LOAD_CONST              11 (('ConfigModule', 'ConfigService', 'Module', 'Controller', 'Injectable', 'Route', 'Get', 'Post', 'Put', 'Patch', 'Delete', 'HttpException', 'HttpStatusMessages', 'HttpStatus', 'UseFilters', 'Catch', 'ExceptionKey', 'ExceptionFilter', 'CanActivate', 'UseGuards', 'Response', 'Request', 'Websocket', 'UploadFile', 'NestipyInterceptor', 'UseInterceptors', 'cors', 'NestipyMiddleware', 'Render', 'TemplateEngine', 'ModuleProviderDict'))
+               202 LIST_EXTEND              1
+               204 STORE_NAME              40 (__all__)
+               206 LOAD_CONST              12 (None)
+               208 RETURN_VALUE
    consts
       0
       ('ModuleProviderDict',)
       1
       ('ConfigModule', 'ConfigService')
       ('Module', 'Controller', 'Injectable', 'Route', 'Get', 'Post', 'Patch', 'Put', 'Delete')
       ('HttpException', 'HttpStatusMessages', 'HttpStatus', 'UseFilters', 'Catch', 'ExceptionKey', 'ExceptionFilter')
       ('CanActivate', 'UseGuards')
       ('Request', 'Response', 'Websocket', 'UploadFile')
       ('NestipyInterceptor', 'UseInterceptors')
-      ('logger',)
-      ('cors', 'NestipyMiddleware', 'session', 'SessionOption')
+      ('cors', 'NestipyMiddleware')
       ('Render', 'TemplateEngine')
-      ('ConfigModule', 'ConfigService', 'Module', 'Controller', 'Injectable', 'Route', 'Get', 'Post', 'Put', 'Patch', 'Delete', 'HttpException', 'HttpStatusMessages', 'HttpStatus', 'UseFilters', 'Catch', 'ExceptionKey', 'ExceptionFilter', 'CanActivate', 'UseGuards', 'Response', 'Request', 'Websocket', 'UploadFile', 'NestipyInterceptor', 'UseInterceptors', 'cors', 'NestipyMiddleware', 'Render', 'TemplateEngine', 'ModuleProviderDict', 'session', 'SessionOption', 'logger')
+      ('ConfigModule', 'ConfigService', 'Module', 'Controller', 'Injectable', 'Route', 'Get', 'Post', 'Put', 'Patch', 'Delete', 'HttpException', 'HttpStatusMessages', 'HttpStatus', 'UseFilters', 'Catch', 'ExceptionKey', 'ExceptionFilter', 'CanActivate', 'UseGuards', 'Response', 'Request', 'Websocket', 'UploadFile', 'NestipyInterceptor', 'UseInterceptors', 'cors', 'NestipyMiddleware', 'Render', 'TemplateEngine', 'ModuleProviderDict')
       None
-   names      ('nestipy.ioc', 'ModuleProviderDict', 'config', 'ConfigModule', 'ConfigService', 'decorator', 'Module', 'Controller', 'Injectable', 'Route', 'Get', 'Post', 'Patch', 'Put', 'Delete', 'exception', 'HttpException', 'HttpStatusMessages', 'HttpStatus', 'UseFilters', 'Catch', 'ExceptionKey', 'ExceptionFilter', 'guards', 'CanActivate', 'UseGuards', 'http_', 'Request', 'Response', 'Websocket', 'UploadFile', 'interceptor', 'NestipyInterceptor', 'UseInterceptors', 'logger', 'middleware', 'cors', 'NestipyMiddleware', 'session', 'SessionOption', 'template', 'Render', 'TemplateEngine', '__all__')
+   names      ('nestipy_ioc', 'ModuleProviderDict', 'config', 'ConfigModule', 'ConfigService', 'decorator', 'Module', 'Controller', 'Injectable', 'Route', 'Get', 'Post', 'Patch', 'Put', 'Delete', 'exception', 'HttpException', 'HttpStatusMessages', 'HttpStatus', 'UseFilters', 'Catch', 'ExceptionKey', 'ExceptionFilter', 'guards', 'CanActivate', 'UseGuards', 'http_', 'Request', 'Response', 'Websocket', 'UploadFile', 'interceptor', 'NestipyInterceptor', 'UseInterceptors', 'middleware', 'cors', 'NestipyMiddleware', 'template', 'Render', 'TemplateEngine', '__all__')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/tsiresy/work/python/nestipy/src/nestipy/common/__init__.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02020c0110012c0124011001180110010c0118011002
+   lnotab 0x00ff02020c0210012c01240110011801100110011002
```

### Comparing `nestipy-0.3.1/src/nestipy/common/__pycache__/http_method.cpython-311.pyc` & `nestipy-0.3.2/src/nestipy/common/__pycache__/http_method.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/common/config/__init__.py` & `nestipy-0.3.2/src/nestipy/common/config/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from dataclasses import asdict
-from typing import Literal
+from typing import Literal, Annotated
 
 from nestipy.common.decorator import Module, Injectable
 from nestipy.dynamic_module import ConfigurableModuleBuilder
 from nestipy.ioc import ModuleProviderDict, Inject
 from nestipy.metadata import Reflect
 
 Config = dict[Literal['folder'], str]
 ConfigurableModuleClass, CONFIG_MODULE_OPTION_TOKEN = ConfigurableModuleBuilder[Config]().set_method('for_root').build()
 
 
 @Injectable()
 class ConfigService:
-    token: Inject[CONFIG_MODULE_OPTION_TOKEN]
+    token: Annotated[str, Inject(CONFIG_MODULE_OPTION_TOKEN)]
 
 
 @Module(
     providers=[
         ConfigService,
         ModuleProviderDict(value='hello', token='MyProvider')
     ],
```

### Comparing `nestipy-0.3.1/src/nestipy/common/decorator/class_.py` & `nestipy-0.3.2/src/nestipy/common/decorator/class_.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/common/decorator/method.py` & `nestipy-0.3.2/src/nestipy/common/decorator/method.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/common/exception/decorator.py` & `nestipy-0.3.2/src/nestipy/common/exception/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/common/exception/message.py` & `nestipy-0.3.2/src/nestipy/common/exception/message.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/common/exception/status.py` & `nestipy-0.3.2/src/nestipy/common/exception/status.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/common/helpers/__init__.py` & `nestipy-0.3.2/src/nestipy/common/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/common/http_/multipart.py` & `nestipy-0.3.2/src/nestipy/common/http_/multipart.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/common/http_/request.py` & `nestipy-0.3.2/src/nestipy/common/http_/request.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/common/http_/response.py` & `nestipy-0.3.2/src/nestipy/common/http_/response.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/common/http_/upload_file.py` & `nestipy-0.3.2/src/nestipy/common/http_/upload_file.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/common/middleware/cors.py` & `nestipy-0.3.2/src/nestipy/common/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/common/middleware/session.py` & `nestipy-0.3.2/src/nestipy/common/middleware/session.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/common/template/interface.py` & `nestipy-0.3.2/src/nestipy/common/template/interface.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/common/utils.py` & `nestipy-0.3.2/src/nestipy/common/utils.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/__init__.py` & `nestipy-0.3.2/src/nestipy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.3.2/src/nestipy/core/__pycache__/__init__.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x03aa2f66 (Mon Apr 29 14:09:07 2024 UTC)
+moddate:  0x8d832f66 (Mon Apr 29 11:25:01 2024 UTC)
 files sz: 933
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `nestipy-0.3.1/src/nestipy/core/__pycache__/app_context.cpython-311.pyc` & `nestipy-0.3.2/src/nestipy/core/__pycache__/app_context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/__pycache__/factory.cpython-311.pyc` & `nestipy-0.3.2/src/nestipy/core/__pycache__/factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/__pycache__/utils.cpython-311.pyc` & `nestipy-0.3.2/src/nestipy/core/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/adapter/blacksheep_adapter.py` & `nestipy-0.3.2/src/nestipy/core/adapter/blacksheep_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/adapter/fastapi_adapter.py` & `nestipy-0.3.2/src/nestipy/core/adapter/fastapi_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/adapter/http_adapter.py` & `nestipy-0.3.2/src/nestipy/core/adapter/http_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/context/execution_context.py` & `nestipy-0.3.2/src/nestipy/core/context/execution_context.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Type, Callable, Union
 
 from nestipy.common.http_ import Response, Request
 from .argument_host import ArgumentHost
 from .http_argument_host import HttpArgumentHost
+from .graphql_argument_host import GraphqlArgumentHost
+from .websocket_argument_host import WebsocketArgumentHost
 
 
 class ExecutionContext(ArgumentHost):
     def get_args(self) -> tuple[Union[Type, object], Callable, Union[Request, None], Union[Response, None]]:
         return self.get_class(), self.get_handler(), self.get_request(), self.get_response()
 
     def switch_to_http(self) -> HttpArgumentHost:
@@ -16,11 +18,35 @@
             self.get_class(),
             self.get_handler(),
             self.get_request(),
             self.get_response()
         )
 
     def switch_to_graphql(self):
-        pass
+        return GraphqlArgumentHost(
+            self.get_adapter(),
+            self.get_module(),
+            self.get_class(),
+            self.get_handler(),
+            self.get_request(),
+            self.get_response(),
+            self._graphql_args,
+            self._graphql_context,
+        )
+
+    def switch_to_websocket(self):
+        return WebsocketArgumentHost(
+            self.get_adapter(),
+            self.get_module(),
+            self.get_class(),
+            self.get_handler(),
+            self.get_request(),
+            self.get_response(),
+            None,
+            None,
+            self._socket_server,
+            self._socket_client,
+            self._socket_data,
+        )
 
     def get_context(self):
         return self
```

### Comparing `nestipy-0.3.1/src/nestipy/core/discover.py` & `nestipy-0.3.2/src/nestipy/core/discover.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/exception/processor.py` & `nestipy-0.3.2/src/nestipy/core/exception/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/guards/processor.py` & `nestipy-0.3.2/src/nestipy/core/guards/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/instance_loader.py` & `nestipy-0.3.2/src/nestipy/core/instance_loader.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/interceptor/processor.py` & `nestipy-0.3.2/src/nestipy/core/interceptor/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/meta/metadata_creator.py` & `nestipy-0.3.2/src/nestipy/core/meta/metadata_creator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/meta/module_metadata_creator.py` & `nestipy-0.3.2/src/nestipy/core/meta/module_metadata_creator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/middleware/executor.py` & `nestipy-0.3.2/src/nestipy/core/middleware/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
-import logging
 import re
 import traceback
 from typing import Callable, Any
 
 from nestipy.ioc import MiddlewareContainer, MiddlewareProxy
 
+from nestipy.common.logger import logger
 from nestipy.common.http_ import Request, Response
 from nestipy.common.middleware import NestipyMiddleware
 from nestipy.types_ import HTTPMethod
 
 
 def uniq_middleware_list(data: list[MiddlewareProxy]) -> list:
     uniq_middleware = []
@@ -60,16 +60,16 @@
             try:
                 #  get instance of Middleware
                 instance = await self.container.get(proxy)
                 # get use method if it is a middleware class
                 return getattr(instance, 'use')
             except Exception as e:
                 tb = traceback.format_exc()
-                logging.error(e)
-                logging.error(tb)
+                logger.error(e)
+                logger.error(tb)
                 return None
         elif inspect.isfunction(proxy.middleware):
             return proxy.middleware
         else:
             raise Exception('Middleware must be a function or a class that extends NestipyMiddleware')
 
     async def _recursively_call_middleware(self, index: int, middlewares: list[MiddlewareProxy]) -> Any:
```

### Comparing `nestipy-0.3.1/src/nestipy/core/nestipy_application.py` & `nestipy-0.3.2/src/nestipy/core/nestipy_application.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import dataclasses
-import logging
 import os.path
 import traceback
 from typing import Type, Callable, Literal, Union, Any, TYPE_CHECKING
 
-from nestipy.dynamic_module import DynamicModule
-from nestipy.ioc import MiddlewareContainer, MiddlewareProxy, NestipyContainer, ModuleProviderDict
-from nestipy.metadata import ModuleMetadata, Reflect
 from openapidocs.v3 import PathItem
 
 from nestipy.common.http_ import Response, Request
+from nestipy.common.logger import logger
 from nestipy.common.middleware import NestipyMiddleware
 from nestipy.common.template import TemplateEngine, TemplateKey
 from nestipy.common.utils import uniq_list
 from nestipy.core.template import MinimalJinjaTemplateEngine
+from nestipy.dynamic_module import DynamicModule
 from nestipy.graphql.graphql_adapter import GraphqlAdapter
 from nestipy.graphql.strawberry.strawberry_adapter import StrawberryAdapter
+from nestipy.ioc import MiddlewareContainer, MiddlewareProxy, NestipyContainer, ModuleProviderDict
+from nestipy.metadata import ModuleMetadata, Reflect
 from .adapter.fastapi_adapter import FastApiAdapter
 from .adapter.http_adapter import HttpAdapter
 from .discover import DiscoverService
 from .instance_loader import InstanceLoader
 from .meta.controller_metadata_creator import ControllerMetadataCreator
 from .meta.module_metadata_creator import ModuleMetadataCreator
 from .meta.provider_metadata_creator import ProviderMetadataCreator
@@ -115,16 +115,16 @@
             # Register open api catch asynchronously
             from nestipy.openapi.constant import OPENAPI_HANDLER_METADATA
             openapi_register: Callable = Reflect.get_metadata(self, OPENAPI_HANDLER_METADATA, None)
             if openapi_register is not None:
                 openapi_register()
         except Exception as e:
             tb = traceback.format_exc()
-            logging.error(e)
-            logging.error(tb)
+            logger.error(e)
+            logger.error(tb)
 
     async def _destroy(self):
         await self.instance_loader.destroy()
 
     def get_adapter(self) -> HttpAdapter:
         return self._http_adapter
```

### Comparing `nestipy-0.3.1/src/nestipy/core/nestipy_factory.py` & `nestipy-0.3.2/src/nestipy/core/nestipy_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,22 +12,26 @@
         return typing.cast(NestipyFactory, self)
 
 
 class NestipyFactory(metaclass=_NestipyFactoryMeta):
 
     @classmethod
     def create(cls, module: Type, config: NestipyApplicationConfig = None) -> NestipyApplication:
-        logging.addLevelName(logging.INFO, "[NESTIPY] INFO")
-        logging.addLevelName(logging.ERROR, "[NESTIPY] ERROR")
-        logging.addLevelName(logging.WARNING, "[NESTIPY] WARNING")
-        logging.addLevelName(logging.WARN, "[NESTIPY] WARN")
-        logging.addLevelName(logging.CRITICAL, "[NESTIPY] CRITICAL")
+        cls._setup_log()
         if getattr(cls, '__generic_type__', None) == 'NestipyBlackSheepApplication':
             if not config:
                 config = NestipyApplicationConfig(adapter=BlackSheepAdapter())
         application = NestipyApplication(config=config)
         application.init(module)
         return application
 
     @classmethod
     def create_micro_service(cls):
         pass
+
+    @classmethod
+    def _setup_log(cls):
+        logging.addLevelName(logging.INFO, "[NESTIPY] INFO")
+        logging.addLevelName(logging.ERROR, "[NESTIPY] ERROR")
+        logging.addLevelName(logging.WARNING, "[NESTIPY] WARNING")
+        logging.addLevelName(logging.WARN, "[NESTIPY] WARN")
+        logging.addLevelName(logging.CRITICAL, "[NESTIPY] CRITICAL")
```

### Comparing `nestipy-0.3.1/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.3.2/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc` & `nestipy-0.3.2/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc` & `nestipy-0.3.2/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc` & `nestipy-0.3.2/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/router/route_explorer.py` & `nestipy-0.3.2/src/nestipy/core/router/route_explorer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/router/router_proxy.py` & `nestipy-0.3.2/src/nestipy/core/router/router_proxy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import dataclasses
-import logging
 import traceback
 import typing
 from typing import Type, Union
 
 from openapidocs.v3 import Operation, PathItem
 from pydantic import BaseModel
 
 from nestipy.common.exception import HttpException
 from nestipy.common.exception.message import HttpStatusMessages
 from nestipy.common.exception.status import HttpStatus
 from nestipy.common.http_ import Request, Response
+from nestipy.common.logger import logger
 from nestipy.common.utils import snakecase_to_camelcase
 from nestipy.core.exception.processor import ExceptionFilterHandler
 from nestipy.core.guards import GuardProcessor
 from nestipy.core.interceptor import RequestInterceptor
 from nestipy.core.middleware import MiddlewareExecutor
 from nestipy.core.template import TemplateRendererProcessor
 from nestipy.ioc import NestipyContainer
 from nestipy.ioc import RequestContextContainer
-from nestipy.metadata import NestipyContextProperty
 from nestipy.types_ import NextFn, CallableHandler
 from .route_explorer import RouteExplorer
 from ..adapter.http_adapter import HttpAdapter
 from ..context.execution_context import ExecutionContext
 
 
 class RouterProxy:
@@ -57,55 +56,41 @@
                     )
                     json_paths[path] = route_path
         paths = {}
         for path, op in json_paths.items():
             paths[path] = PathItem(**op)
         return paths
 
-    @classmethod
-    async def setup_context_data(cls, context_container: RequestContextContainer, req: "Request", res: "Response"):
-        context_container.set_value(NestipyContextProperty.request, req)
-        context_container.set_value(NestipyContextProperty.response, res)
-        context_container.set_value(NestipyContextProperty.params, req.path_params)
-        context_container.set_value(NestipyContextProperty.query_params, req.query_params)
-        context_container.set_value(NestipyContextProperty.headers, req.headers)
-        context_container.set_value(NestipyContextProperty.session, req.session)
-        context_container.set_value(NestipyContextProperty.cookies, req.cookies)
-        form_data = await req.form()
-        if form_data is not None:
-            context_container.set_value(NestipyContextProperty.body, form_data)
-        else:
-            json_data = await req.json()
-            context_container.set_value(NestipyContextProperty.body, json_data)
-
     def create_request_handler(
             self,
             module_ref: Type,
             controller: Union[object, Type],
             method_name: str
     ) -> CallableHandler:
 
         async def request_handler(req: "Request", res: "Response", next_fn: NextFn):
 
             context_container = RequestContextContainer.get_instance()
             # setup container for query params, route params, request, response, session, etc..
-            await self.setup_context_data(context_container, req, res)
+            # await self.setup_context_data(context_container, req, res)
+
             # TODO: req.files
 
             container = NestipyContainer.get_instance()
             controller_method_handler = getattr(controller, method_name)
             execution_context = ExecutionContext(
                 self.router,
                 module_ref,
                 controller,
                 controller_method_handler,
                 req,
                 res
             )
-            context_container.set_value(NestipyContextProperty.execution_context, execution_context)
+            context_container.set_container(container)
+            context_container.set_execution_context(execution_context)
             handler_response: Response
             try:
                 # TODO : Refactor
                 guard_processor: GuardProcessor = await NestipyContainer.get_instance().get(GuardProcessor)
                 can_activate = await guard_processor.process(execution_context)
                 if not can_activate[0]:
                     # Raise error
@@ -138,17 +123,18 @@
                 # process template rendering
                 if self._template_processor.can_process(controller_method_handler, result):
                     result = await res.html(self._template_processor.render())
                 # transform result to response
                 handler_response = await self._ensure_response(res, result)
 
             except Exception as e:
-                logging.error(e)
+                tb = traceback.format_exc()
+                logger.error(e)
+                logger.error(tb)
                 if not isinstance(e, HttpException):
-                    tb = traceback.format_exc()
                     e = HttpException(HttpStatus.INTERNAL_SERVER_ERROR, str(e), str(tb))
 
                 # Call exception catch
                 exception_handler = await container.get(ExceptionFilterHandler)
                 result = await exception_handler.catch(e, execution_context)
                 if result:
                     handler_response = await self._ensure_response(res, result)
```

### Comparing `nestipy-0.3.1/src/nestipy/core/template/minimal_jinja.py` & `nestipy-0.3.2/src/nestipy/core/template/minimal_jinja.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/core/template/processor.py` & `nestipy-0.3.2/src/nestipy/core/template/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/dynamic_module/builder.py` & `nestipy-0.3.2/src/nestipy/dynamic_module/builder.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/dynamic_module/module/consumer.py` & `nestipy-0.3.2/src/nestipy/dynamic_module/module/consumer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/graphql/decorator.py` & `nestipy-0.3.2/src/nestipy/graphql/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/graphql/graphql_adapter.py` & `nestipy-0.3.2/src/nestipy/graphql/graphql_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/graphql/graphql_asgi.py` & `nestipy-0.3.2/src/nestipy/graphql/graphql_asgi.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/graphql/graphql_explorer.py` & `nestipy-0.3.2/src/nestipy/graphql/graphql_explorer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/graphql/graphql_module.py` & `nestipy-0.3.2/src/nestipy/graphql/graphql_module.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import dataclasses
-from typing import Literal
+from typing import Literal, Annotated
 
 from nestipy.common.decorator import Module
 from nestipy.dynamic_module import ConfigurableModuleBuilder
 from nestipy.ioc import Inject
 
 
 @dataclasses.dataclass
@@ -14,8 +14,8 @@
 
 ConfigurableModuleClass, CONFIG_MODULE_OPTION_TOKEN = ConfigurableModuleBuilder[GraphqlOption]().set_method(
     'for_root').build()
 
 
 @Module()
 class GraphqlModule(ConfigurableModuleClass):
-    config: Inject[CONFIG_MODULE_OPTION_TOKEN]
+    config: Annotated[GraphqlOption, Inject(CONFIG_MODULE_OPTION_TOKEN)]
```

### Comparing `nestipy-0.3.1/src/nestipy/graphql/graphql_proxy.py` & `nestipy-0.3.2/src/nestipy/graphql/graphql_proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import traceback
 from typing import Union, Type, Callable
 
 from nestipy.core.guards import GuardProcessor
 from nestipy.graphql.graphql_adapter import GraphqlAdapter
 from nestipy.ioc import NestipyContainer
 from nestipy.ioc import RequestContextContainer
 from nestipy.metadata import NestipyContextProperty
-
 from .graphql_explorer import GraphqlExplorer
 from .graphql_module import GraphqlModule, GraphqlOption
 from ..common import Request
+from ..common.logger import logger
 from ..core.adapter.http_adapter import HttpAdapter
 from ..core.context.execution_context import ExecutionContext
 
 
 class GraphqlProxy:
 
     def __init__(self, adapter: HttpAdapter, graphql_server: GraphqlAdapter):
@@ -39,37 +40,44 @@
     def _create_graphql_query_handler(self, module_ref: Union[Type, object], meta: dict) -> tuple[str, Type, Callable]:
         resolver: Union[object, Type] = meta['class']
         method_name: str = meta['handler_name']
         method = getattr(resolver, method_name)
 
         async def graphql_handler(*_args, **kwargs):
             context_container = RequestContextContainer.get_instance()
-            context_container.set_value(NestipyContextProperty.args, kwargs)
+            execution_context = ExecutionContext(
+                self._adapter,
+                module_ref,
+                resolver,
+                getattr(resolver, method_name),
+                context_container.get_value(NestipyContextProperty.request),
+                context_container.get_value(NestipyContextProperty.response),
+                None,
+                kwargs
+            )
+            context_container.set_container(NestipyContainer.get_instance())
+            context_container.set_execution_context(execution_context)
             try:
                 # TODO: Refactor with routerProxy
                 # create execution context
-                execution_context = ExecutionContext(
-                    self._adapter,
-                    module_ref,
-                    resolver,
-                    getattr(resolver, method_name),
-                    context_container.get_value(NestipyContextProperty.request),
-                    context_container.get_value(NestipyContextProperty.response)
-                )
-                context_container.set_value(NestipyContextProperty.execution_context, execution_context)
+
                 #  apply guards
                 guard_processor: GuardProcessor = await self.container.get(GuardProcessor)
                 can_activate = await guard_processor.process(execution_context)
                 if not can_activate[0]:
                     # TODO: is this need to specify return Exception
                     raise Exception(f"Not authorized from guard {can_activate[1]}")
 
                 # perform query request
                 result = await self.container.get(resolver, method_name)
                 return result
+            except Exception as e:
+                tb = traceback.format_exc()
+                logger.error(e)
+                logger.error(tb)
             finally:
                 context_container.destroy()
 
         # mutate handle inside adapter
         return_type = self._graphql_server.mutate_handler(method, graphql_handler)
         return method_name, return_type, graphql_handler,
```

### Comparing `nestipy-0.3.1/src/nestipy/graphql/playground/graphql-playground-default.html` & `nestipy-0.3.2/src/nestipy/graphql/playground/graphql-playground-default.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/graphql/playground/graphql-playground-graphiql.html` & `nestipy-0.3.2/src/nestipy/graphql/playground/graphql-playground-graphiql.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/graphql/pubsub.py` & `nestipy-0.3.2/src/nestipy/graphql/pubsub.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/graphql/strawberry/__init__.py` & `nestipy-0.3.2/src/nestipy/graphql/strawberry/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/graphql/strawberry/strawberry_adapter.py` & `nestipy-0.3.2/src/nestipy/graphql/strawberry/strawberry_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/graphql/strawberry/strawberry_asgi.py` & `nestipy-0.3.2/src/nestipy/graphql/strawberry/strawberry_asgi.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/ioc/__init__.py` & `nestipy-0.3.2/src/nestipy/ioc/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,33 @@
-from .annotation import Annotation
+from .annotation import ParamAnnotation
 from .container import NestipyContainer
 from .context_container import RequestContextContainer
-from .dependency import Inject, Res, Req, Session, Query, Body, Args, Context, Files, SocketServer, SocketClient, \
-    SocketData, Params, Arg, Sessions, Queries, Param, Header, Headers, Cookies, Cookie
+from .dependency import Inject, Res, Req, Session, Query, Body, Arg, Context, GraphQlContext, SocketServer, \
+    SocketClient, \
+    SocketData, Params, Header, Cookie
 from .middleware import MiddlewareProxy, MiddlewareRouteConfig, MiddlewareContainer
 from .provider import ModuleProviderDict
 
 __all__ = [
-    "Annotation",
+    "ParamAnnotation",
     "NestipyContainer",
     "RequestContextContainer",
     "ModuleProviderDict",
     "Inject",
     "Res",
     "Req",
     "Session",
     "Query",
     "Body",
-    "Args",
+    "Arg",
     "Context",
-    "Files",
     "SocketServer",
     "SocketClient",
     "SocketData",
     "Params",
     "MiddlewareProxy",
     "MiddlewareRouteConfig",
     "MiddlewareContainer",
-    "Arg",
-    "Sessions",
-    "Queries",
-    "Param",
     "Header",
-    "Headers",
-    "Cookies",
-    "Cookie"
+    "Cookie",
+    "GraphQlContext"
 ]
```

### Comparing `nestipy-0.3.1/src/nestipy/ioc/container.py` & `nestipy-0.3.2/src/nestipy/ioc/container.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import dataclasses
 import inspect
 from functools import lru_cache
 from typing import Type, Union, Any, Optional, ForwardRef, Callable, Awaitable, TYPE_CHECKING
 
 from pydantic import BaseModel
 
-from nestipy.metadata import ClassMetadata, CtxDepKey, ModuleMetadata, ProviderToken, Reflect, NestipyContextProperty
+from nestipy.metadata import ClassMetadata, CtxDepKey, ModuleMetadata, ProviderToken, Reflect
 from .context_container import RequestContextContainer
+from .dependency import TypeAnnotated
 from .meta import ContainerHelper
 from .utils import uniq
 
 if TYPE_CHECKING:
     from .provider import ModuleProviderDict
 
 
@@ -82,75 +83,22 @@
     def _data_to_typed(cls, annotation: Union[Type, Any], data: Union[dict, list, str, int, tuple, set, Any]):
         if dataclasses.is_dataclass(annotation) or issubclass(annotation, BaseModel):
             return annotation(**data)
         elif annotation in (dict, list, str, int, tuple, set, Any):
             return data
         return None
 
-    def _resolve_context_service(self, name: str, dep_key: CtxDepKey, annotation: Union[Type, Any]):
+    @classmethod
+    async def _resolve_context_service(cls, dep_key: TypeAnnotated, annotation: Union[Type, Any]):
         context_container = RequestContextContainer.get_instance()
-        match dep_key:
-            case CtxDepKey.Request:
-                return context_container.get_value(NestipyContextProperty.request)
-            case CtxDepKey.Response:
-                return context_container.get_value(NestipyContextProperty.response)
-            case CtxDepKey.Body:
-                data: dict = context_container.get_value(NestipyContextProperty.body)
-                return self._data_to_typed(annotation, data)
-            case CtxDepKey.Context:
-                return context_container.get_value(NestipyContextProperty.execution_context)
-            case CtxDepKey.SocketClient:
-                return context_container.get_value(NestipyContextProperty.io_client)
-            case CtxDepKey.SocketData:
-                return self._data_to_typed(annotation, context_container.get_value(NestipyContextProperty.io_data))
-            case CtxDepKey.Session:
-                return self.helper.get_value_from_dict(
-                    context_container.get_value(NestipyContextProperty.session),
-                    name
-                )
-
-            case CtxDepKey.Sessions:
-                return self._data_to_typed(annotation, context_container.get_value(NestipyContextProperty.session))
-            case CtxDepKey.Param:
-                return self.helper.get_value_from_dict(
-                    context_container.get_value(NestipyContextProperty.params),
-                    name
-                )
-            case CtxDepKey.Params:
-                return self._data_to_typed(annotation, context_container.get_value(NestipyContextProperty.params))
-            case CtxDepKey.Query:
-                return self.helper.get_value_from_dict(
-                    context_container.get_value(NestipyContextProperty.query_params),
-                    name
-                )
-            case CtxDepKey.Queries:
-                return self._data_to_typed(annotation, context_container.get_value(NestipyContextProperty.query_params))
-            case CtxDepKey.Cookie:
-                return self.helper.get_value_from_dict(
-                    context_container.get_value(NestipyContextProperty.cookies),
-                    name
-                )
-            case CtxDepKey.Cookies:
-                return self._data_to_typed(annotation, context_container.get_value(NestipyContextProperty.cookies))
-            case CtxDepKey.Arg:
-                return self.helper.get_value_from_dict(context_container.get_value(NestipyContextProperty.args), name)
-            case CtxDepKey.Args:
-                return self._data_to_typed(annotation, context_container.get_value(NestipyContextProperty.args))
-            case CtxDepKey.Header:
-                return self.helper.get_value_from_dict(
-                    context_container.get_value(NestipyContextProperty.headers),
-                    name
-                )
-            case CtxDepKey.Headers:
-                return self._data_to_typed(annotation, context_container.get_value(NestipyContextProperty.headers))
-
-            case CtxDepKey.Files:
-                return self.helper.get_value_from_dict(context_container.get_value(NestipyContextProperty.files), name)
-            case _:
-                return None
+        callback = dep_key.metadata.callback
+        if inspect.iscoroutinefunction(callback):
+            return await callback(dep_key.metadata.token, annotation, context_container)
+        else:
+            return callback(dep_key.metadata.token, annotation, context_container)
 
     async def _resolve_module_provider_dict(self, instance: "ModuleProviderDict", search_scope: list):
         if instance.value:
             return instance.value
         elif instance.existing:
             if isinstance(instance.existing, ProviderToken):
                 return await self.get(instance.existing.key)
@@ -203,20 +151,23 @@
         annotations: dict = getattr(service, '__annotations__', {})
         for name, param_annotation in annotations.items():
             annotation, dep_key = self.helper.get_type_from_annotation(param_annotation)
             if isinstance(annotation, ForwardRef):
                 annotation = eval(annotation.__forward_arg__, globals())
                 if annotation is None:
                     raise ValueError(f"Unknown forward reference: {annotation}")
-            if dep_key.metadata in CtxDepKey.to_list():
-                if dep_key.metadata is not CtxDepKey.Service:
-                    dependency = self._resolve_context_service(name, dep_key.metadata, annotation)
+            if dep_key.metadata.key in CtxDepKey.to_list():
+                if dep_key.metadata.key is not CtxDepKey.Service:
+                    dependency = await self._resolve_context_service(dep_key, annotation)
                     setattr(service, name, dependency)
-                elif annotation in search_scope:
-                    dependency = await self.get(annotation, origin=origin)
+                elif dep_key.metadata.token in search_scope or annotation in search_scope:
+                    if dep_key.metadata.token:
+                        dependency = await self.get(dep_key.metadata.token, origin=origin)
+                    else:
+                        dependency = await self.get(annotation, origin=origin)
                     setattr(service, name, dependency)
                 elif isinstance(annotation, ProviderToken) and annotation.key in search_scope:
                     dependency = await self.get(annotation.key, origin=origin)
                     setattr(service, name, dependency)
                 else:
                     _name: str = annotation.__name__ if not isinstance(annotation, str) else annotation
                     raise ValueError(
@@ -229,16 +180,16 @@
 
     async def _get_method_dependency(self, method_to_resolve: Callable, search_scope: list, origin: list):
         params = inspect.signature(method_to_resolve).parameters
         args = {}
         for name, param in params.items():
             if name != 'self' and param.annotation is not inspect.Parameter.empty:
                 annotation, dep_key = self.helper.get_type_from_annotation(param.annotation)
-                if dep_key.metadata in CtxDepKey.to_list() and dep_key.metadata is not CtxDepKey.Service:
-                    dependency = self._resolve_context_service(name, dep_key.metadata, annotation)
+                if dep_key.metadata.key in CtxDepKey.to_list() and dep_key.metadata.key is not CtxDepKey.Service:
+                    dependency = await self._resolve_context_service(dep_key, annotation)
                     args[name] = dependency
                 elif annotation in search_scope:
                     dependency = await self.get(annotation, origin=origin)
                     args[name] = dependency
                 else:
                     _name: str = annotation.__name__ if not isinstance(annotation, str) else annotation
                     raise ValueError(f"Service {_name} not found in scope {search_scope}")
```

### Comparing `nestipy-0.3.1/src/nestipy/ioc/middleware.py` & `nestipy-0.3.2/src/nestipy/ioc/middleware.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/ioc/provider.py` & `nestipy-0.3.2/src/nestipy/ioc/provider.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/metadata/class_.py` & `nestipy-0.3.2/src/nestipy/metadata/class_.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/metadata/decorator.py` & `nestipy-0.3.2/src/nestipy/metadata/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/metadata/dependency.py` & `nestipy-0.3.2/src/nestipy/metadata/dependency.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/metadata/reflect.py` & `nestipy-0.3.2/src/nestipy/metadata/reflect.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/__init__.py` & `nestipy-0.3.2/src/nestipy/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/decorator.py` & `nestipy-0.3.2/src/nestipy/openapi/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/document_builder.py` & `nestipy-0.3.2/src/nestipy/openapi/document_builder.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/common.py` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/common.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/__init__.py` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/common.py` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/common.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/contents.py` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/contents.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/generate.py` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/generate.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/jinja.py` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/jinja.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/md.py` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/md.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/texts.py` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/texts.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/examples.py` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/examples.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/utils/source.py` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/utils/source.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/utils/web.py` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/utils/web.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/v2.py` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/v2.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/openapi_docs/v3.py` & `nestipy-0.3.2/src/nestipy/openapi/openapi_docs/v3.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/swagger.html` & `nestipy-0.3.2/src/nestipy/openapi/swagger.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/swagger_module.py` & `nestipy-0.3.2/src/nestipy/openapi/swagger_module.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/openapi/test.py` & `nestipy-0.3.2/src/nestipy/openapi/test.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/websocket/adapter.py` & `nestipy-0.3.2/src/nestipy/websocket/adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,16 +50,17 @@
         super().__init__(path=path)
         self._io = io
         self._connected = []
 
     def on(self, event: str, namespace: str = None):
         def decorator(handler: Callable):
             async def wrapper(sid: str, data: Any):
+                session = await self._io.get_session(sid, namespace)
                 #  transform data id need
-                return await handler(sid, data)
+                return await handler(event, session, data)
 
             self._io.on(event, namespace=namespace)(wrapper)
 
         return decorator
 
     async def emit(
             self,
```

### Comparing `nestipy-0.3.1/src/nestipy/websocket/decorator.py` & `nestipy-0.3.2/src/nestipy/websocket/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.1/src/nestipy/websocket/proxy.py` & `nestipy-0.3.2/src/nestipy/websocket/proxy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import inspect
+import traceback
 from typing import Type, Union, Callable, Any, TYPE_CHECKING
 
+from nestipy.common.logger import logger
 from nestipy.ioc import NestipyContainer
 from nestipy.ioc import RequestContextContainer
 from nestipy.metadata import NestipyContextProperty, Reflect, ModuleMetadata
-
 from .decorator import GATEWAY_KEY, EVENT_KEY, SUCCESS_EVENT_KEY, ERROR_EVENT_KEY
 from ..core.context.execution_context import ExecutionContext
 
 if TYPE_CHECKING:
     from ..core.adapter.http_adapter import HttpAdapter
 
 
@@ -55,51 +56,56 @@
             self,
             module_ref: Type,
             gateway: Type,
             method_name: str,
             namespace: str,
             event_name: Any
     ) -> Callable[..., Any]:
-        async def io_handler(sid: Any, data: Any):
+        async def io_handler(event: Any, session: Any, data: Any):
             io_adapter = self.adapter.get_io_adapter()
             context_container = RequestContextContainer.get_instance()
-            context_container.set_value(NestipyContextProperty.io_client, sid)
-            context_container.set_value(NestipyContextProperty.io_data, data)
-            context_container.set_value(NestipyContextProperty.io_server, io_adapter)
-
             container = NestipyContainer.get_instance()
             gateway_method = getattr(gateway, method_name)
             execution_context = ExecutionContext(
                 self.adapter,
                 module_ref,
                 gateway,
                 gateway_method,
                 None,
-                None
+                None,
+                None,
+                None,
+                io_adapter,
+                session,
+                data
             )
-            context_container.set_value(NestipyContextProperty.execution_context, execution_context)
+            context_container.set_execution_context(execution_context)
+            context_container.set_container(container)
             try:
                 result = await container.get(gateway, method_name)
                 if result is not None:
                     # get success event from handler
                     success_event = Reflect.get_metadata(gateway, SUCCESS_EVENT_KEY, None)
                     # send response to websocket
                     await self.call_handler(io_adapter.emit, {
                         'event': success_event or event_name,
                         'data': result,
                         'namespace': namespace,
-                        "to": sid
+                        "to": session.sid
                     })
             except Exception as e:
+                tb = traceback.format_exc()
+                logger.error(e)
+                logger.error(tb)
                 error_event = Reflect.get_metadata(gateway, ERROR_EVENT_KEY, None)
                 if error_event is not None:
                     await self.call_handler(io_adapter.emit, {
                         'event': error_event,
                         'data': str(e),
                         'namespace': namespace,
-                        "to": sid
+                        "to": session.sid
                     })
                 # create exception handler
             finally:
                 context_container.destroy()
 
         return io_handler
```

### Comparing `nestipy-0.3.1/PKG-INFO` & `nestipy-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestipy
-Version: 0.3.1
+Version: 0.3.2
 Summary: Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nestipy Version: 0.3.1 Summary: Nestipy is a Python
+Metadata-Version: 2.1 Name: nestipy Version: 0.3.2 Summary: Nestipy is a Python
 framework built on top of BlackSheep that follows the modular architecture of
 NestJS Author: tsiresymila Author-email: tsiresymila@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: aiofiles (>=23.2.1,<24.0.0) Requires-Dist: blacksheep (>=2.0.7,<3.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0) Requires-Dist: minijinja
```

