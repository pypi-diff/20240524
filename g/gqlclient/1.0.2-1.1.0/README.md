# Comparing `tmp/gqlclient-1.0.2.tar.gz` & `tmp/gqlclient-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqlclient-1.0.2.tar", last modified: Wed Oct 25 23:54:54 2023, max compression
+gzip compressed data, was "gqlclient-1.1.0.tar", last modified: Fri May 24 17:10:13 2024, max compression
```

## Comparing `gqlclient-1.0.2.tar` & `gqlclient-1.1.0.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-25 23:54:54.327973 gqlclient-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1756 2023-10-25 23:54:48.000000 gqlclient-1.0.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-10-25 23:54:48.000000 gqlclient-1.0.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1050 2023-10-25 23:54:48.000000 gqlclient-1.0.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     4839 2023-10-25 23:54:54.327973 gqlclient-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4374 2023-10-25 23:54:48.000000 gqlclient-1.0.2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      734 2023-10-25 23:54:48.000000 gqlclient-1.0.2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-25 23:54:54.327973 gqlclient-1.0.2/docs/
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-10-25 23:54:48.000000 gqlclient-1.0.2/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     3405 2023-10-25 23:54:48.000000 gqlclient-1.0.2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-10-25 23:54:48.000000 gqlclient-1.0.2/docs/index.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-25 23:54:54.327973 gqlclient-1.0.2/gqlclient/
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5548 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/async_client.py
--rw-rw-rw-   0 root         (0) root         (0)    13715 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2026 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3922 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/dataclass_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3386 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/null.py
--rw-rw-rw-   0 root         (0) root         (0)     3574 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/request_wrap.py
--rw-rw-rw-   0 root         (0) root         (0)     3240 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/response_encoders.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-25 23:54:54.327973 gqlclient-1.0.2/gqlclient/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/tests/test_async_client.py
--rw-rw-rw-   0 root         (0) root         (0)     9395 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/tests/test_dataclass_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    21422 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/tests/test_graphql_base.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/tests/test_graphql_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1880 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/tests/test_null.py
--rw-rw-rw-   0 root         (0) root         (0)     5530 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/tests/test_request_wrap.py
--rw-rw-rw-   0 root         (0) root         (0)     5784 2023-10-25 23:54:48.000000 gqlclient-1.0.2/gqlclient/tests/test_response_encoders.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-25 23:54:54.327973 gqlclient-1.0.2/gqlclient.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4839 2023-10-25 23:54:54.000000 gqlclient-1.0.2/gqlclient.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-10-25 23:54:54.000000 gqlclient-1.0.2/gqlclient.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-10-25 23:54:54.000000 gqlclient-1.0.2/gqlclient.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-10-25 23:54:54.000000 gqlclient-1.0.2/gqlclient.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       10 2023-10-25 23:54:54.000000 gqlclient-1.0.2/gqlclient.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-10-25 23:54:48.000000 gqlclient-1.0.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1001 2023-10-25 23:54:54.327973 gqlclient-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-10-25 23:54:48.000000 gqlclient-1.0.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-24 17:10:13.364003 gqlclient-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-24 17:09:58.000000 gqlclient-1.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-24 17:09:58.000000 gqlclient-1.1.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-24 17:09:58.000000 gqlclient-1.1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      464 2024-05-24 17:09:58.000000 gqlclient-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5438 2024-05-24 17:10:13.364003 gqlclient-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4453 2024-05-24 17:09:58.000000 gqlclient-1.1.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2024-05-24 17:09:58.000000 gqlclient-1.1.0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-24 17:10:13.360003 gqlclient-1.1.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      581 2024-05-24 17:09:58.000000 gqlclient-1.1.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     3404 2024-05-24 17:09:58.000000 gqlclient-1.1.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-24 17:09:58.000000 gqlclient-1.1.0/docs/index.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-24 17:10:13.360003 gqlclient-1.1.0/gqlclient/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-05-24 17:10:13.000000 gqlclient-1.1.0/gqlclient/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     5809 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/async_client.py
+-rw-rw-rw-   0 root         (0) root         (0)    13827 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2088 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/dataclass_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1932 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3376 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/null.py
+-rw-rw-rw-   0 root         (0) root         (0)     3588 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/request_wrap.py
+-rw-rw-rw-   0 root         (0) root         (0)     3276 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/response_encoders.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-24 17:10:13.364003 gqlclient-1.1.0/gqlclient/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/tests/test_async_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     9395 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/tests/test_dataclass_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    21617 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/tests/test_graphql_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      313 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/tests/test_graphql_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1880 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/tests/test_null.py
+-rw-rw-rw-   0 root         (0) root         (0)     5643 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/tests/test_request_wrap.py
+-rw-rw-rw-   0 root         (0) root         (0)     5826 2024-05-24 17:09:58.000000 gqlclient-1.1.0/gqlclient/tests/test_response_encoders.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-24 17:10:13.364003 gqlclient-1.1.0/gqlclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5438 2024-05-24 17:10:13.000000 gqlclient-1.1.0/gqlclient.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      875 2024-05-24 17:10:13.000000 gqlclient-1.1.0/gqlclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-24 17:10:13.000000 gqlclient-1.1.0/gqlclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-24 17:10:13.000000 gqlclient-1.1.0/gqlclient.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      148 2024-05-24 17:10:13.000000 gqlclient-1.1.0/gqlclient.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-05-24 17:10:13.000000 gqlclient-1.1.0/gqlclient.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1950 2024-05-24 17:09:58.000000 gqlclient-1.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-24 17:10:13.364003 gqlclient-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2024-05-24 17:09:58.000000 gqlclient-1.1.0/tox.ini
```

### Comparing `gqlclient-1.0.2/.gitignore` & `gqlclient-1.1.0/.gitignore`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -121,8 +121,8 @@
 
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
-.pyre/
+.pyre/
```

### Comparing `gqlclient-1.0.2/.pre-commit-config.yaml` & `gqlclient-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gqlclient-1.0.2/LICENSE` & `gqlclient-1.1.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+MIT License
+
 Copyright 2019 NSO / AURA
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `gqlclient-1.0.2/PKG-INFO` & `gqlclient-1.1.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: gqlclient
-Version: 1.0.2
-Summary: Client library for making graphql calls
-Home-page: https://bitbucket.org/dkistdc/graphql_client/src/master/
-Author: NSO / AURA
-Author-email: "swiant@nso.edu"
-License: MIT
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
-Provides-Extra: async
-Provides-Extra: test
-License-File: LICENSE
-
 gqlclient
 =========
 
 |codecov|
 
 .. image:: https://readthedocs.org/projects/graphql-client/badge/?version=latest
    :target: https://dkistdc.readthedocs.io/projects/graphql-client/en/latest/?badge=latest
@@ -49,14 +33,20 @@
 
 with ``asyncio`` support
 
 .. code:: bash
 
    pip install gqlclient[async]
 
+with ``pydantic`` support
+
+.. code:: bash
+
+   pip install gqlclient[pydantic]
+
 for developers
 
 .. code:: bash
 
    pip install gqlclient[test]
    pip install pre-commit
    pre-commit install
```

### Comparing `gqlclient-1.0.2/docs/Makefile` & `gqlclient-1.1.0/docs/Makefile`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `gqlclient-1.0.2/docs/conf.py` & `gqlclient-1.1.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
 #
 # Configuration file for the Sphinx documentation builder.
-
 from pkg_resources import get_distribution
 
 # -- Project information -----------------------------------------------------
 
 project = "gqlclient"
 copyright = "2019, Scott Wiant, Stuart Mumford"
 author = "Scott Wiant, Stuart Mumford"
```

### Comparing `gqlclient-1.0.2/gqlclient/async_client.py` & `gqlclient-1.1.0/gqlclient/async_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 """
 Implementation of the Base graphql client to support the asynchronous creation and
 execution of graphql queries and mutations
 """
 import logging
-from typing import Any, Callable, Optional
+from typing import Any
+from typing import Callable
+from typing import Optional
 
 import aiohttp
 
-from gqlclient.base import GraphQLClientBase, DefaultParameters
-from gqlclient.exceptions import ServerConnectionException, ClientErrorException, RedirectionResponseException, ServerErrorException, ServerResponseException
+from gqlclient.base import DefaultParameters
+from gqlclient.base import GraphQLClientBase
+from gqlclient.exceptions import ClientErrorException
+from gqlclient.exceptions import RedirectionResponseException
+from gqlclient.exceptions import ServerConnectionException
+from gqlclient.exceptions import ServerErrorException
+from gqlclient.exceptions import ServerResponseException
 
 
 __all__ = ["AsyncGraphQLClient"]
 
 
 logger = logging.getLogger(__name__)
 
@@ -37,45 +44,49 @@
         logger.debug(f"Executing graphql call: host={self.gql_uri}")
 
         async with aiohttp.ClientSession() as session:
             try:
                 async with session.post(self.gql_uri, json=query, **kwargs) as response:
                     result = await response.json()
                     if response.status > 299:
-                        exception_message = f"Server returned invalid response: " \
-                                            f"code=HTTP{response.status}, "
+                        exception_message = (
+                            f"Server returned invalid response: " f"code=HTTP{response.status}, "
+                        )
                         if response.status > 499:
                             raise ServerErrorException(exception_message)
                         if response.status > 399:
                             raise ClientErrorException(exception_message)
                         raise RedirectionResponseException(exception_message)
             except aiohttp.ClientConnectionError as e:
                 logger.error(
                     f"Error connecting to graphql server: server={self.gql_uri}, detail={e!r}"
                 )
                 raise ServerConnectionException(
                     f"Error connecting to graphql server: server={self.gql_uri}, detail={e!r}"
                 ) from e
             except aiohttp.ContentTypeError as e:
                 logger.error(
-                    f"Error decoding response from graphql server: " f"server={self.gql_uri}, " 
+                    f"Error decoding response from graphql server: "
+                    f"server={self.gql_uri}, "
                     f"detail={e}"
                 )
                 raise ServerResponseException(
-                    f"Error decoding response from graphql server: " f"server={self.gql_uri}, " f"detail={e}"
+                    f"Error decoding response from graphql server: "
+                    f"server={self.gql_uri}, "
+                    f"detail={e}"
                 )
             return result
 
     async def execute_gql_query(
         self,
         query_base: str,
         query_response_cls: type,
         query_parameters: object | None = DefaultParameters,
         response_encoder: Callable[[str, dict, type], Any] | None = None,
-        **kwargs
+        **kwargs,
     ) -> Any:
         """
         Executes a graphql query based upon input dataclass models.
 
         :param query_base: Name of the root type to be queried
 
         :param query_parameters: Optional. Instance of a dataclass model containing attributes corresponding to
@@ -96,15 +107,15 @@
 
     async def execute_gql_mutation(
         self,
         mutation_base: str,
         mutation_parameters: object,
         mutation_response_cls: type | None = None,
         response_encoder: Callable[[str, dict, type], Any] | None = None,
-        **kwargs
+        **kwargs,
     ) -> Any:
         """
         Executes a graphql mutation based upon input dataclass models.
 
         :param mutation_base: Name of the root type to be mutated
 
         :param mutation_parameters: Instance of a dataclass model containing attributes corresponding to
```

### Comparing `gqlclient-1.0.2/gqlclient/base.py` & `gqlclient-1.1.0/gqlclient/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 from requests.structures import CaseInsensitiveDict
 
 from gqlclient.dataclass_utils import extract_dataclass
 from gqlclient.dataclass_utils import yield_valid_fields
 from gqlclient.exceptions import GraphQLException
 from gqlclient.exceptions import ModelException
 from gqlclient.null import NullType
-from gqlclient.request_wrap import AbstractWrap, StaticWrap, dynamic_mutation_param_wrapper, dynamic_query_param_wrapper
+from gqlclient.request_wrap import AbstractWrap
+from gqlclient.request_wrap import dynamic_mutation_param_wrapper
+from gqlclient.request_wrap import dynamic_query_param_wrapper
+from gqlclient.request_wrap import StaticWrap
 from gqlclient.response_encoders import dataclass_encoder
 
 __all__ = ["GraphQLClientBase"]
 
 
 logger = logging.getLogger(__name__)
 
@@ -139,17 +142,17 @@
                 if getattr(model, field.name) is not None
             ]
         )
         return parameters
 
     @staticmethod
     def _get_param_wrapper(
-            model: object,
-            *,
-            mutation_base: str | None = None,
+        model: object,
+        *,
+        mutation_base: str | None = None,
     ) -> tuple[str, object]:
         """
         Return a GraphQL query param name and param values from the provided dataclass instance.
 
         :param model: Dataclass instance with the actual request parameters
         :param mutation_base: Optional mutation name.  Must be provided for mutations using a dynamic param_name.
 
@@ -223,15 +226,17 @@
         response object with attributes corresponding to the Graphql type and attribute names.
 
         :return: Dictionary that can be passed as json to the GraphQL API endpoint
         """
 
         # Construct graphql mutation
         gql_mutation = f"mutation {mutation_base} {{{mutation_base}"
-        param_wrapper, mutation_parameters = self._get_param_wrapper(mutation_parameters, mutation_base=mutation_base)
+        param_wrapper, mutation_parameters = self._get_param_wrapper(
+            mutation_parameters, mutation_base=mutation_base
+        )
         parameters = self._graphql_query_parameters_from_model(mutation_parameters)
         if param_wrapper:
             # resulting format: (params: {id: "abc"})
             gql_mutation += f"({param_wrapper}: {{{parameters}}})"
         else:
             # resulting format: (id: "abc")
             gql_mutation += f"({parameters})"
```

### Comparing `gqlclient-1.0.2/gqlclient/client.py` & `gqlclient-1.1.0/gqlclient/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 execution of graphql queries and mutations
 """
 import logging
 
 import requests
 
 from gqlclient.base import GraphQLClientBase
-from gqlclient.exceptions import ServerConnectionException, RedirectionResponseException, ClientErrorException, ServerErrorException
+from gqlclient.exceptions import ClientErrorException
+from gqlclient.exceptions import RedirectionResponseException
+from gqlclient.exceptions import ServerConnectionException
+from gqlclient.exceptions import ServerErrorException
 
 
 __all__ = ["GraphQLClient"]
 
 
 logger = logging.getLogger(__name__)
 
@@ -31,24 +34,24 @@
 
         :return: Dictionary containing the response from the GraphQL endpoint
         """
         logger.debug(f"Executing graphql call: host={self.gql_uri}")
         try:
             response = requests.post(url=self.gql_uri, json=query, **kwargs)
         except requests.ConnectionError as e:
-            logger.error(
-                f"Error connecting to graphql server: server={self.gql_uri}, detail={e!r}"
-            )
+            logger.error(f"Error connecting to graphql server: server={self.gql_uri}, detail={e!r}")
             raise ServerConnectionException(
                 f"Error connecting to graphql server: server={self.gql_uri}, detail={e!r}"
             ) from e
         # Isolating error codes due to server side exceptions
         if response.status_code > 299:
-            exception_message = f"Server returned invalid response: " \
-                                f"code=HTTP{response.status_code}, " \
-                                f"detail={response.text}"
+            exception_message = (
+                f"Server returned invalid response: "
+                f"code=HTTP{response.status_code}, "
+                f"detail={response.text}"
+            )
             if response.status_code > 499:
                 raise ServerErrorException(exception_message)
             if response.status_code > 399:
                 raise ClientErrorException(exception_message)
             raise RedirectionResponseException(exception_message)
         return response.json()
```

### Comparing `gqlclient-1.0.2/gqlclient/dataclass_utils.py` & `gqlclient-1.1.0/gqlclient/dataclass_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,10 +90,12 @@
     # noinspection PyDataclass
     for field in dc_fields(model):
         extracted_dataclass = extract_dataclass(field.type)
 
         # raise an exception if the dataclass has been seen before
         if extracted_dataclass and extracted_dataclass.__name__ in context:
             # prevent infinite loop - raise exception
-            raise ValueError(f"Circular Reference in {model.__name__!r} caused by {extracted_dataclass.__name__!r}")
+            raise ValueError(
+                f"Circular Reference in {model.__name__!r} caused by {extracted_dataclass.__name__!r}"
+            )
 
         yield field
```

### Comparing `gqlclient-1.0.2/gqlclient/exceptions.py` & `gqlclient-1.1.0/gqlclient/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "GQLClientException",
     "GraphQLException",
     "ModelException",
     "ServerConnectionException",
     "ServerResponseException",
     "RedirectionResponseException",
     "ClientErrorException",
-    "ServerErrorException"
+    "ServerErrorException",
 ]
 
 
 class GQLClientException(Exception):
     """
     Base Exception for all exceptions raised by the gql client
     """
```

### Comparing `gqlclient-1.0.2/gqlclient/null.py` & `gqlclient-1.1.0/gqlclient/null.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,44 +28,44 @@
     def __repr__(self) -> str:
         return "NULL"
 
     def __bool__(self) -> bool:
         return False
 
     @classmethod
-    def __get_pydantic_core_schema__(
-        cls, source_type: "NullType", handler
-    ):
+    def __get_pydantic_core_schema__(cls, source_type: "NullType", handler):
         """
         This validator is required to support pydantic V2 dataclass validation.
         This validator roughly equates to: `isinstance(input_value, NullType)` with attendant fluff.
         Since pydantic V2 may not be in use, no pydantic V2 imports can occur until this method gets called.
         The handler, provided by the V2 framework, is a pydantic.GetCoreSchemaHandler.
         The method returns a pydantic_core.CoreSchema to the pydantic V2 framework.
         """
         if source_type is not NullType:
             raise ValueError("This validation is only for NullType")
 
         # pydantic V2 imports
         # noinspection PyUnresolvedReferences
         from pydantic_core import core_schema
+
         # noinspection PyUnresolvedReferences
         from pydantic_core import PydanticCustomError
+
         # noinspection PyUnresolvedReferences
         from pydantic_core.core_schema import ValidationInfo
 
         def is_null_type(v: Any, info: ValidationInfo) -> Any:
             # Separate validation for json is possible if a need is identified
             if info.mode == "python":
                 if not isinstance(v, NullType):
                     raise PydanticCustomError("not_null", "Input must be NULL")
             return v
 
         null_schema = core_schema.is_instance_schema(cls)
-        return core_schema.general_before_validator_function(is_null_type, null_schema)
+        return core_schema.with_info_before_validator_function(is_null_type, null_schema)
 
     @classmethod
     def __get_validators__(cls):
         """
         This validator is required to support pydantic V1 dataclass validation.
         This validator roughly equates to: `isinstance(input_value, NullType)` with attendant fluff.
         Since pydantic V1 may not be in use, no pydantic V1 imports can occur until this method gets called.
```

### Comparing `gqlclient-1.0.2/gqlclient/request_wrap.py` & `gqlclient-1.1.0/gqlclient/request_wrap.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,22 +4,24 @@
   2.  A nested, or wrapped, request object inside a mapping, for example: (params: {id: "abc"})
   2.a.  The client dynamically assigns the `params` key
   2.b.  The caller defines the static `params` key
 This module provides tooling for wrapping requests.
 If the caller desires a direct passthrough of the request object, this module should not be used.
 """
 from abc import ABC
-from dataclasses import dataclass, is_dataclass
+from dataclasses import dataclass
+from dataclasses import is_dataclass
 
 
 @dataclass
 class AbstractWrap(ABC):
     """
     Abstract dataclass for nested request params.
     """
+
     request_params: object | None
 
     def __new__(cls, *args, **kwargs):
         if cls == AbstractWrap:
             raise TypeError("AbstractWrap cannot be instantiated because it is an abstract class")
         return super().__new__(cls)
 
@@ -30,36 +32,38 @@
 
 
 @dataclass
 class DynamicWrap(AbstractWrap):
     """
     Concrete dataclass for nested request params with a dynamic param name.
     """
+
     pass
 
     def __init__(self, request_params: object):
         super().__init__(request_params=request_params)
 
 
 @dataclass
 class StaticWrap(AbstractWrap):
     """
     Concrete dataclass for nested request params with a static param name.
     """
+
     param_name: str
 
     def __init__(self, request_params: object, param_name: str):
         super().__init__(request_params=request_params)
         self.param_name = param_name
 
 
 def wrap_request(
-        request_params: object | None = None,
-        *,
-        param_name: str = None,
+    request_params: object | None = None,
+    *,
+    param_name: str = None,
 ) -> DynamicWrap | StaticWrap:
     """
     Return a nested, or wrapped, request object.
     :param request_params: An instance of a dataclass to be nested.
     :param param_name: Optional.  If provided, this will be the mapping key.
     Otherwise the mapping key will be dynamically generated at a later point.
     :return: A nested dataclass with `request_params` matching the input.
```

### Comparing `gqlclient-1.0.2/gqlclient/response_encoders.py` & `gqlclient-1.1.0/gqlclient/response_encoders.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """
 Encoders for translating a dict graphql response into another form
 """
 import json
 import logging
-from typing import List, Optional, Union, Type
+from typing import List
+from typing import Optional
+from typing import Type
+from typing import Union
 
-from dacite import from_dict, Config
+from dacite import Config
+from dacite import from_dict
 
 from gqlclient.exceptions import EncoderResponseException
 
 __all__ = ["dataclass_encoder", "json_encoder", "dict_encoder"]
 
 
 logger = logging.getLogger(__name__)
 
 
 def dataclass_encoder(
-        call_base: str,
-        response: list[dict] | dict,
-        response_cls: type,
+    call_base: str,
+    response: list[dict] | dict,
+    response_cls: type,
 ) -> list[type] | type | None:
     """
     Response encoder that produces a list or a single instance of the response class
 
     :param call_base: The base query or mutation the response is coming from
     :param response: The dict response from the graphql server
     :param response_cls: The dataclass that was used to specify the response
@@ -48,17 +52,17 @@
     except Exception as e:
         logger.error(f"Error dataclass encoding response: detail={e}")
         raise EncoderResponseException(str(e))
     return encoded_response
 
 
 def json_encoder(
-        call_base: str,
-        response: list[dict] | dict,
-        response_cls: type,
+    call_base: str,
+    response: list[dict] | dict,
+    response_cls: type,
 ) -> str:
     """
     Response encoder that produces json string
 
     :param call_base: The base query or mutation the response is coming from
     :param response: The dict response from the graphql server
     :param response_cls: The dataclass that was used to specify the response
@@ -69,17 +73,17 @@
     except TypeError as e:
         logger.error(f"Error json encoding response: detail={e}")
         raise EncoderResponseException(str(e))
     return result
 
 
 def dict_encoder(
-        call_base: str,
-        response: list[dict] | dict,
-        response_cls: type,
+    call_base: str,
+    response: list[dict] | dict,
+    response_cls: type,
 ) -> list[dict] | dict:
     """
     Default encoder which returns the response as a dict or list of dicts
 
     :param call_base: The base query or mutation the response is coming from
     :param response: The dict response from the graphql server
     :param response_cls: The dataclass that was used to specify the response
```

### Comparing `gqlclient-1.0.2/gqlclient/tests/test_dataclass_utils.py` & `gqlclient-1.1.0/gqlclient/tests/test_dataclass_utils.py`

 * *Files identical despite different names*

### Comparing `gqlclient-1.0.2/gqlclient/tests/test_graphql_base.py` & `gqlclient-1.1.0/gqlclient/tests/test_graphql_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Tests for the graphql_client library
 """
-
+from dataclasses import dataclass
 from datetime import datetime
 from typing import List
-from dataclasses import dataclass
 
-from pydantic.dataclasses import dataclass as pydantic_dataclass
 import pytest
+from pydantic.dataclasses import dataclass as pydantic_dataclass
 
 from gqlclient import GraphQLClient
 from gqlclient.base import dynamic_mutation_param_wrapper
 from gqlclient.base import dynamic_query_param_wrapper
 from gqlclient.exceptions import ModelException
-from gqlclient.request_wrap import StaticWrap, DynamicWrap, AbstractWrap
+from gqlclient.request_wrap import AbstractWrap
+from gqlclient.request_wrap import DynamicWrap
+from gqlclient.request_wrap import StaticWrap
 
 QUERY_BASE = "query_base"
 MUTATION_BASE = "mutation_base"
 
 
 # Dataclass defined test data
 @dataclass
@@ -170,22 +171,24 @@
     Test of query string structure when request params are included for passthrough
     :param client: Graphql Client instance
     :param query_base: Name of the query endpoint
     :param request_params: Instance of a simple dataclass containing the request parameters
     :param response_cls: Dataclass containing the attributes of the graphql response
     :return: None
     """
-    assert not isinstance(request_params, AbstractWrap), "Invalid test fixture. Cannot be AbstractWrap for this test."
+    assert not isinstance(
+        request_params, AbstractWrap
+    ), "Invalid test fixture. Cannot be AbstractWrap for this test."
 
     test_query = client.get_query(
         query_base=query_base, query_parameters=request_params, query_response_cls=response_cls
     )
     assert "query" in test_query
     expected_query_str = (
-        '{query_base('
+        "{query_base("
         'str_param: "A", '
         "int_param: 1, "
         "float_param: 1.1, "
         'str_array_param: ["A", "B"], '
         "num_array_param: [1, 2], "
         "bool_param: false, "
         'date_param: "2010-03-25T14:08:00")'
@@ -209,24 +212,26 @@
     Test of query string structure when request params and `param_name` are included
     :param client: Graphql Client instance
     :param query_base: Name of the query endpoint
     :param request_object: Instance of a StaticWrap dataclass containing the `request_params` and static `param_name`
     :param response_cls: Dataclass containing the attributes of the graphql response
     :return: None
     """
-    assert isinstance(request_object, StaticWrap), "Invalid test fixture. StaticWrap required for this test."
+    assert isinstance(
+        request_object, StaticWrap
+    ), "Invalid test fixture. StaticWrap required for this test."
 
     test_query = client.get_query(
         query_base=query_base, query_parameters=request_object, query_response_cls=response_cls
     )
     param_wrapper = request_object.param_name
     assert "query" in test_query
     expected_query_str = (
-        '{query_base('
-        f'{param_wrapper}: '
+        "{query_base("
+        f"{param_wrapper}: "
         '{str_param: "A", '
         "int_param: 1, "
         "float_param: 1.1, "
         'str_array_param: ["A", "B"], '
         "num_array_param: [1, 2], "
         "bool_param: false, "
         'date_param: "2010-03-25T14:08:00"})'
@@ -242,37 +247,39 @@
     [
         (QUERY_BASE, dynamic_nested_dataclass_request, DataclassResponseParent),
         (QUERY_BASE, dynamic_nested_pydantic_dataclass_request, PydanticDataclassResponseParent),
         (QUERY_BASE, dynamic_nested_dataclass_request, DataclassResponseParentWithList),
     ],
 )
 def test_query_dynamic_nest_with_parameters(
-        client,
-        query_base: str,
-        request_object: object,
-        response_cls: type,
+    client,
+    query_base: str,
+    request_object: object,
+    response_cls: type,
 ):
     """
     Test of query string structure when request params are included and `param_name` will be determined dynamically
     :param client: Graphql Client instance
     :param query_base: Name of the query endpoint
     :param request_object: Instance of a DynamicWrap dataclass containing the `request_params`
     :param response_cls: Dataclass containing the attributes of the graphql response
     :return: None
     """
-    assert isinstance(request_object, DynamicWrap), "Invalid test fixture. DynamicWrap required for this test."
+    assert isinstance(
+        request_object, DynamicWrap
+    ), "Invalid test fixture. DynamicWrap required for this test."
 
     test_query = client.get_query(
         query_base=query_base, query_parameters=request_object, query_response_cls=response_cls
     )
     param_wrapper = dynamic_query_param_wrapper()
     assert "query" in test_query
     expected_query_str = (
-        '{query_base('
-        f'{param_wrapper}: '
+        "{query_base("
+        f"{param_wrapper}: "
         '{str_param: "A", '
         "int_param: 1, "
         "float_param: 1.1, "
         'str_array_param: ["A", "B"], '
         "num_array_param: [1, 2], "
         "bool_param: false, "
         'date_param: "2010-03-25T14:08:00"})'
@@ -281,18 +288,15 @@
         "} }"
     )
     assert test_query["query"] == expected_query_str
 
 
 @pytest.mark.parametrize(
     "query_base, response_cls",
-    [
-        (QUERY_BASE, DataclassResponseParent),
-        (QUERY_BASE, PydanticDataclassResponseParent)
-    ],
+    [(QUERY_BASE, DataclassResponseParent), (QUERY_BASE, PydanticDataclassResponseParent)],
 )
 def test_query_without_parameters(client, query_base: str, response_cls):
     """
     Test of query string structure when parameter model is NOT included
     :param client: Graphql Client instance
     :param query_base: Name of the query endpoint
     :param response_cls: Dataclass containing the attributes of the graphql response
@@ -313,35 +317,39 @@
 @pytest.mark.parametrize(
     "mutation_base, request_params, response_cls",
     [
         (MUTATION_BASE, dataclass_request, DataclassResponseParent),
         (MUTATION_BASE, pydantic_dataclass_request, PydanticDataclassResponseParent),
     ],
 )
-def test_mutation_passthrough_with_response(client, mutation_base: str, request_params, response_cls):
+def test_mutation_passthrough_with_response(
+    client, mutation_base: str, request_params, response_cls
+):
     """
     Test of mutation string structure when response model is included and request params are included for passthrough
     :param client: Graphql Client instance
     :param mutation_base: Name of the mutation endpoint
     :param request_params: Instance of a simple dataclass containing the request parameters
     :param response_cls: Dataclass containing the attributes of the graphql response
     :return: None
     """
-    assert not isinstance(request_params, AbstractWrap), "Invalid test fixture. Cannot be AbstractWrap for this test."
+    assert not isinstance(
+        request_params, AbstractWrap
+    ), "Invalid test fixture. Cannot be AbstractWrap for this test."
 
     test_mutation = client.get_mutation(
         mutation_base=mutation_base,
         mutation_response_cls=response_cls,
         mutation_parameters=request_params,
     )
     assert "query" in test_mutation
     assert "operationName" in test_mutation
     expected_query_str = (
         "mutation mutation_base "
-        '{mutation_base('
+        "{mutation_base("
         'str_param: "A", '
         "int_param: 1, "
         "float_param: 1.1, "
         'str_array_param: ["A", "B"], '
         "num_array_param: [1, 2], "
         "bool_param: false, "
         'date_param: "2010-03-25T14:08:00")'
@@ -356,37 +364,41 @@
 @pytest.mark.parametrize(
     "mutation_base, request_object, response_cls",
     [
         (MUTATION_BASE, static_nested_dataclass_request, DataclassResponseParent),
         (MUTATION_BASE, static_nested_pydantic_dataclass_request, PydanticDataclassResponseParent),
     ],
 )
-def test_mutation_static_nest_with_response(client, mutation_base: str, request_object, response_cls):
+def test_mutation_static_nest_with_response(
+    client, mutation_base: str, request_object, response_cls
+):
     """
     Test of mutation string structure when response model is included and request params and `param_name` are included
     :param client: Graphql Client instance
     :param mutation_base: Name of the mutation endpoint
     :param request_object: Instance of a StaticWrap dataclass containing the `request_params` and static `param_name`
     :param response_cls: Dataclass containing the attributes of the graphql response
     :return: None
     """
-    assert isinstance(request_object, StaticWrap), "Invalid test fixture. StaticWrap required for this test."
+    assert isinstance(
+        request_object, StaticWrap
+    ), "Invalid test fixture. StaticWrap required for this test."
 
     test_mutation = client.get_mutation(
         mutation_base=mutation_base,
         mutation_response_cls=response_cls,
         mutation_parameters=request_object,
     )
     param_wrapper = request_object.param_name  # noqa
     assert "query" in test_mutation
     assert "operationName" in test_mutation
     expected_query_str = (
         "mutation mutation_base "
-        '{mutation_base('
-        f'{param_wrapper}: '
+        "{mutation_base("
+        f"{param_wrapper}: "
         '{str_param: "A", '
         "int_param: 1, "
         "float_param: 1.1, "
         'str_array_param: ["A", "B"], '
         "num_array_param: [1, 2], "
         "bool_param: false, "
         'date_param: "2010-03-25T14:08:00"})'
@@ -401,38 +413,42 @@
 @pytest.mark.parametrize(
     "mutation_base, request_object, response_cls",
     [
         (MUTATION_BASE, dynamic_nested_dataclass_request, DataclassResponseParent),
         (MUTATION_BASE, dynamic_nested_pydantic_dataclass_request, PydanticDataclassResponseParent),
     ],
 )
-def test_mutation_dynamic_nest_with_response(client, mutation_base: str, request_object, response_cls):
+def test_mutation_dynamic_nest_with_response(
+    client, mutation_base: str, request_object, response_cls
+):
     """
     Test of mutation string structure when response model is included and request params are included
     and `param_name` will be determined dynamically.
     :param client: Graphql Client instance
     :param mutation_base: Name of the mutation endpoint
     :param request_object: Instance of a DynamicWrap dataclass containing the `request_params`
     :param response_cls: Dataclass containing the attributes of the graphql response
     :return: None
     """
-    assert isinstance(request_object, DynamicWrap), "Invalid test fixture. DynamicWrap required for this test."
+    assert isinstance(
+        request_object, DynamicWrap
+    ), "Invalid test fixture. DynamicWrap required for this test."
 
     test_mutation = client.get_mutation(
         mutation_base=mutation_base,
         mutation_response_cls=response_cls,
         mutation_parameters=request_object,
     )
     param_wrapper = dynamic_mutation_param_wrapper(mutation_base)
     assert "query" in test_mutation
     assert "operationName" in test_mutation
     expected_query_str = (
         "mutation mutation_base "
-        '{mutation_base('
-        f'{param_wrapper}: '
+        "{mutation_base("
+        f"{param_wrapper}: "
         '{str_param: "A", '
         "int_param: 1, "
         "float_param: 1.1, "
         'str_array_param: ["A", "B"], '
         "num_array_param: [1, 2], "
         "bool_param: false, "
         'date_param: "2010-03-25T14:08:00"})'
@@ -442,36 +458,37 @@
 
     assert test_mutation["query"] == expected_query_str
     assert test_mutation["operationName"] == "mutation_base"
 
 
 @pytest.mark.parametrize(
     "mutation_base, request_params",
-    [
-        (MUTATION_BASE, dataclass_request),
-        (MUTATION_BASE, pydantic_dataclass_request)
-    ],
+    [(MUTATION_BASE, dataclass_request), (MUTATION_BASE, pydantic_dataclass_request)],
 )
 def test_mutation_passthrough_without_response(client, mutation_base: str, request_params):
     """
     Test of mutation string structure when response model is NOT included
     and request params are included for passthrough
     :param client: Graphql Client instance
     :param mutation_base: Name of the mutation endpoint
     :param request_params: Instance of a simple dataclass containing the request parameters
     :return: None
     """
-    assert not isinstance(request_params, AbstractWrap), "Invalid test fixture. Cannot be AbstractWrap for this test."
+    assert not isinstance(
+        request_params, AbstractWrap
+    ), "Invalid test fixture. Cannot be AbstractWrap for this test."
 
-    test_mutation = client.get_mutation(mutation_base=mutation_base, mutation_parameters=request_params)
+    test_mutation = client.get_mutation(
+        mutation_base=mutation_base, mutation_parameters=request_params
+    )
     assert "query" in test_mutation
     assert "operationName" in test_mutation
     expected_query_str = (
         "mutation mutation_base "
-        '{mutation_base('
+        "{mutation_base("
         'str_param: "A", '
         "int_param: 1, float_param: 1.1, "
         'str_array_param: ["A", "B"], '
         "num_array_param: [1, 2], "
         "bool_param: false, "
         'date_param: "2010-03-25T14:08:00") }'
     )
@@ -480,36 +497,40 @@
     assert test_mutation["operationName"] == "mutation_base"
 
 
 @pytest.mark.parametrize(
     "mutation_base, request_object",
     [
         (MUTATION_BASE, static_nested_dataclass_request),
-        (MUTATION_BASE, static_nested_pydantic_dataclass_request)
+        (MUTATION_BASE, static_nested_pydantic_dataclass_request),
     ],
 )
 def test_mutation_static_nest_without_response(client, mutation_base: str, request_object):
     """
     Test of mutation string structure when response model is NOT included
     but request params and `param_name` are included
     :param client: Graphql Client instance
     :param mutation_base: Name of the mutation endpoint
     :param request_object: Instance of a StaticWrap dataclass containing the `request_params` and static `param_name`
     :return: None
     """
-    assert isinstance(request_object, StaticWrap), "Invalid test fixture. StaticWrap required for this test."
+    assert isinstance(
+        request_object, StaticWrap
+    ), "Invalid test fixture. StaticWrap required for this test."
 
-    test_mutation = client.get_mutation(mutation_base=mutation_base, mutation_parameters=request_object)
+    test_mutation = client.get_mutation(
+        mutation_base=mutation_base, mutation_parameters=request_object
+    )
     param_wrapper = request_object.param_name
     assert "query" in test_mutation
     assert "operationName" in test_mutation
     expected_query_str = (
         "mutation mutation_base "
-        '{mutation_base('
-        f'{param_wrapper}: '
+        "{mutation_base("
+        f"{param_wrapper}: "
         '{str_param: "A", '
         "int_param: 1, float_param: 1.1, "
         'str_array_param: ["A", "B"], '
         "num_array_param: [1, 2], "
         "bool_param: false, "
         'date_param: "2010-03-25T14:08:00"}) }'
     )
@@ -518,36 +539,40 @@
     assert test_mutation["operationName"] == "mutation_base"
 
 
 @pytest.mark.parametrize(
     "mutation_base, request_object",
     [
         (MUTATION_BASE, dynamic_nested_dataclass_request),
-        (MUTATION_BASE, dynamic_nested_pydantic_dataclass_request)
+        (MUTATION_BASE, dynamic_nested_pydantic_dataclass_request),
     ],
 )
 def test_mutation_dynamic_nest_without_response(client, mutation_base: str, request_object):
     """
     Test of mutation string structure when response model is NOT included and request params are included
     and `param_name` will be determined dynamically.
     :param client: Graphql Client instance
     :param mutation_base: Name of the mutation endpoint
     :param request_object: Instance of a DynamicWrap dataclass containing the `request_params`
     :return: None
     """
-    assert isinstance(request_object, DynamicWrap), "Invalid test fixture. DynamicWrap required for this test."
+    assert isinstance(
+        request_object, DynamicWrap
+    ), "Invalid test fixture. DynamicWrap required for this test."
 
-    test_mutation = client.get_mutation(mutation_base=mutation_base, mutation_parameters=request_object)
+    test_mutation = client.get_mutation(
+        mutation_base=mutation_base, mutation_parameters=request_object
+    )
     param_wrapper = dynamic_mutation_param_wrapper(mutation_name=mutation_base)
     assert "query" in test_mutation
     assert "operationName" in test_mutation
     expected_query_str = (
         "mutation mutation_base "
-        '{mutation_base('
-        f'{param_wrapper}: '
+        "{mutation_base("
+        f"{param_wrapper}: "
         '{str_param: "A", '
         "int_param: 1, float_param: 1.1, "
         'str_array_param: ["A", "B"], '
         "num_array_param: [1, 2], "
         "bool_param: false, "
         'date_param: "2010-03-25T14:08:00"}) }'
     )
```

### Comparing `gqlclient-1.0.2/gqlclient/tests/test_null.py` & `gqlclient-1.1.0/gqlclient/tests/test_null.py`

 * *Files identical despite different names*

### Comparing `gqlclient-1.0.2/gqlclient/tests/test_request_wrap.py` & `gqlclient-1.1.0/gqlclient/tests/test_request_wrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """
 Tests for request wrapping
 """
-from dataclasses import dataclass, asdict
+from dataclasses import asdict
+from dataclasses import dataclass
 
 import pytest
 from pydantic.dataclasses import dataclass as pydantic_dataclass
 
-from gqlclient.request_wrap import AbstractWrap, DynamicWrap, StaticWrap, wrap_request
+from gqlclient.request_wrap import AbstractWrap
+from gqlclient.request_wrap import DynamicWrap
+from gqlclient.request_wrap import StaticWrap
+from gqlclient.request_wrap import wrap_request
 
 
 @dataclass
 class BaseDataclass:
     value: str = "base dataclass"
     optInt: int | None = None
 
@@ -26,15 +30,15 @@
     [
         pytest.param(BaseDataclass(), id="base"),
         pytest.param(PydDataclass(), id="pyd"),
         pytest.param(None, id="none"),
     ],
 )
 def test_dataclasses_dynamic(request_params):
-    """ Verify proper dynamic dataclass instantiation """
+    """Verify proper dynamic dataclass instantiation"""
     result: DynamicWrap = DynamicWrap(request_params=request_params)
     assert result
     assert isinstance(result, DynamicWrap)
     result_data = asdict(result)
     # verify param_name is excluded from result
     assert "param_name" not in result_data.keys()
     assert "request_params" in result_data.keys()
@@ -51,15 +55,15 @@
     [
         pytest.param(BaseDataclass(), id="base"),
         pytest.param(PydDataclass(), id="pyd"),
         pytest.param(None, id="none"),
     ],
 )
 def test_dataclasses_static(request_params):
-    """ Verify proper static dataclass instantiation """
+    """Verify proper static dataclass instantiation"""
     result: StaticWrap = StaticWrap(request_params=request_params, param_name="whatever")
     assert result
     assert isinstance(result, StaticWrap)
     result_data = asdict(result)
     # verify param_name is included in result
     assert "param_name" in result_data.keys()
     assert result_data["param_name"] == "whatever"
@@ -76,28 +80,28 @@
     "request_params, expected_exception_type",
     [
         pytest.param(BaseDataclass(), TypeError, id="base"),
         pytest.param(PydDataclass(), TypeError, id="pyd"),
     ],
 )
 def test_dataclasses_abstract(request_params, expected_exception_type: type[Exception]):
-    """ Verify AbstractWrap cannot be instantiated """
+    """Verify AbstractWrap cannot be instantiated"""
     with pytest.raises(expected_exception_type):
         AbstractWrap(request_params=request_params)
 
 
 @pytest.mark.parametrize(
     "request_params, expected_exception_type",
     [
         pytest.param("a_string", TypeError, id="string"),
         pytest.param([], TypeError, id="list"),
     ],
 )
 def test_dataclasses_invalid(request_params, expected_exception_type: type[Exception]):
-    """ Verify request params must be a dataclass """
+    """Verify request params must be a dataclass"""
     with pytest.raises(expected_exception_type):
         DynamicWrap(request_params=request_params)
     with pytest.raises(expected_exception_type):
         StaticWrap(request_params=request_params, param_name="whatever")
 
 
 @pytest.mark.parametrize(
@@ -105,15 +109,15 @@
     [
         pytest.param(BaseDataclass(), id="baseInstance"),
         pytest.param(PydDataclass(), id="pydInstance"),
         pytest.param(None, id="none"),
     ],
 )
 def test_wrap_request(request_params):
-    """ Verify proper result from wrap_request """
+    """Verify proper result from wrap_request"""
     result: DynamicWrap = wrap_request(request_params=request_params)
     assert result
     assert isinstance(result, DynamicWrap)
     result_data = asdict(result)
     # verify param_name is excluded from result
     assert "param_name" not in result_data.keys()
     assert "request_params" in result_data.keys()
@@ -145,12 +149,12 @@
     [
         pytest.param("a_string", TypeError, id="string"),
         pytest.param(BaseDataclass, TypeError, id="baseClass"),
         pytest.param(PydDataclass, TypeError, id="pydClass"),
     ],
 )
 def test_wrap_request_invalid_inputs(request_params, expected_exception_type: type[Exception]):
-    """ Verify proper result from wrap_request for invalid input """
+    """Verify proper result from wrap_request for invalid input"""
     with pytest.raises(expected_exception_type):
         wrap_request(request_params=request_params)
     with pytest.raises(expected_exception_type):
         wrap_request(request_params=request_params, param_name="whatever")
```

### Comparing `gqlclient-1.0.2/gqlclient/tests/test_response_encoders.py` & `gqlclient-1.1.0/gqlclient/tests/test_response_encoders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Tests for the response_encoders library
 """
 from dataclasses import dataclass
-from pydantic.dataclasses import dataclass as pydantic_dataclass
 
 import pytest
+from pydantic.dataclasses import dataclass as pydantic_dataclass
 
-from gqlclient import dataclass_encoder, json_encoder, dict_encoder
+from gqlclient import dataclass_encoder
+from gqlclient import dict_encoder
+from gqlclient import json_encoder
 from gqlclient.exceptions import EncoderResponseException
 
 
 @dataclass
 class ChildResponseModel:
     s: str
     i: int
```

### Comparing `gqlclient-1.0.2/gqlclient.egg-info/SOURCES.txt` & `gqlclient-1.1.0/gqlclient.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
+MANIFEST.in
 README.rst
 bitbucket-pipelines.yml
 pyproject.toml
-setup.cfg
-setup.py
+tox.ini
 docs/Makefile
 docs/conf.py
 docs/index.rst
 gqlclient/__init__.py
+gqlclient/_version.py
 gqlclient/async_client.py
 gqlclient/base.py
 gqlclient/client.py
 gqlclient/dataclass_utils.py
 gqlclient/exceptions.py
 gqlclient/null.py
 gqlclient/request_wrap.py
 gqlclient/response_encoders.py
 gqlclient.egg-info/PKG-INFO
 gqlclient.egg-info/SOURCES.txt
 gqlclient.egg-info/dependency_links.txt
+gqlclient.egg-info/not-zip-safe
 gqlclient.egg-info/requires.txt
 gqlclient.egg-info/top_level.txt
 gqlclient/tests/__init__.py
 gqlclient/tests/test_async_client.py
 gqlclient/tests/test_dataclass_utils.py
 gqlclient/tests/test_graphql_base.py
 gqlclient/tests/test_graphql_client.py
```

