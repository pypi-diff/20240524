# Comparing `tmp/mypy-boto3-managedblockchain-1.34.0.tar.gz` & `tmp/mypy_boto3_managedblockchain-1.34.113.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-managedblockchain-1.34.0.tar", last modified: Wed Dec 13 21:23:10 2023, max compression
+gzip compressed data, was "mypy_boto3_managedblockchain-1.34.113.tar", last modified: Fri May 24 21:22:27 2024, max compression
```

## Comparing `mypy-boto3-managedblockchain-1.34.0.tar` & `mypy_boto3_managedblockchain-1.34.113.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:10.935279 mypy-boto3-managedblockchain-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:13:34.000000 mypy-boto3-managedblockchain-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13255 2023-12-13 21:23:10.935279 mypy-boto3-managedblockchain-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11682 2023-12-13 21:13:34.000000 mypy-boto3-managedblockchain-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:10.931279 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2023-12-13 21:13:34.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2023-12-13 21:13:34.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      945 2023-12-13 21:13:34.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20830 2023-12-13 21:13:34.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20826 2023-12-13 21:13:34.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2023-12-13 21:13:34.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9942 2023-12-13 21:13:34.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2023-12-13 21:13:34.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2023-12-13 21:13:34.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:13:34.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    24483 2023-12-13 21:13:35.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24482 2023-12-13 21:13:35.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:13:34.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:10.935279 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13255 2023-12-13 21:23:10.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 21:23:10.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:10.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:10.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:10.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 21:23:10.000000 mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:10.935279 mypy-boto3-managedblockchain-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2023-12-13 21:13:34.000000 mypy-boto3-managedblockchain-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:22:27.188438 mypy_boto3_managedblockchain-1.34.113/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-24 21:22:14.000000 mypy_boto3_managedblockchain-1.34.113/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-05-24 21:22:27.188438 mypy_boto3_managedblockchain-1.34.113/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-24 21:22:14.000000 mypy_boto3_managedblockchain-1.34.113/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:22:27.188438 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-24 21:22:14.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-24 21:22:14.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-24 21:22:14.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20850 2024-05-24 21:22:14.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20847 2024-05-24 21:22:14.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-24 21:22:14.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-24 21:22:14.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-24 21:22:14.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-24 21:22:14.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:22:14.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    24976 2024-05-24 21:22:14.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24976 2024-05-24 21:22:14.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-24 21:22:14.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:22:27.188438 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-05-24 21:22:27.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-24 21:22:27.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 21:22:27.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 21:22:27.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-24 21:22:27.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-24 21:22:27.000000 mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 21:22:27.188438 mypy_boto3_managedblockchain-1.34.113/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-24 21:22:14.000000 mypy_boto3_managedblockchain-1.34.113/setup.py
```

### Comparing `mypy-boto3-managedblockchain-1.34.0/LICENSE` & `mypy_boto3_managedblockchain-1.34.113/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-managedblockchain-1.34.0/PKG-INFO` & `mypy_boto3_managedblockchain-1.34.113/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-managedblockchain
-Version: 1.34.0
-Summary: Type annotations for boto3.ManagedBlockchain 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.113
+Summary: Type annotations for boto3.ManagedBlockchain 1.34.113 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-managedblockchain"></a>
 
 # mypy-boto3-managedblockchain
 
 [![PyPI - mypy-boto3-managedblockchain](https://img.shields.io/pypi/v/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain)](https://pepy.tech/project/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.34.113](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-managedblockchain-1.34.0/README.md` & `mypy_boto3_managedblockchain-1.34.113/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain)](https://pepy.tech/project/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.34.113](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/__init__.py` & `mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,9 +19,8 @@
 """
 
 from .client import ManagedBlockchainClient
 from .paginator import ListAccessorsPaginator
 
 Client = ManagedBlockchainClient
 
-
 __all__ = ("Client", "ListAccessorsPaginator", "ManagedBlockchainClient")
```

### Comparing `mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/__init__.pyi` & `mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/__main__.py` & `mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ManagedBlockchain 1.34.0\nVersion:         1.34.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain//\nBoto3 docs:   "
-        "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.ManagedBlockchain 1.34.113\n"
+        "Version:         1.34.113\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.113")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/client.py` & `mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,24 +48,23 @@
     ListProposalVotesOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     MemberConfigurationTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
-    ProposalActionsTypeDef,
+    ProposalActionsUnionTypeDef,
     VotingPolicyTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ManagedBlockchainClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -122,15 +121,15 @@
 
     def create_accessor(
         self,
         *,
         ClientRequestToken: str,
         AccessorType: Literal["BILLING_TOKEN"],
         Tags: Mapping[str, str] = ...,
-        NetworkType: AccessorNetworkTypeType = ...
+        NetworkType: AccessorNetworkTypeType = ...,
     ) -> CreateAccessorOutputTypeDef:
         """
         Creates a new accessor for use with Amazon Managed Blockchain service that
         supports token based
         access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_accessor)
@@ -139,15 +138,15 @@
 
     def create_member(
         self,
         *,
         ClientRequestToken: str,
         InvitationId: str,
         NetworkId: str,
-        MemberConfiguration: MemberConfigurationTypeDef
+        MemberConfiguration: MemberConfigurationTypeDef,
     ) -> CreateMemberOutputTypeDef:
         """
         Creates a member within a Managed Blockchain network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_member)
         """
@@ -159,15 +158,15 @@
         Name: str,
         Framework: FrameworkType,
         FrameworkVersion: str,
         VotingPolicy: VotingPolicyTypeDef,
         MemberConfiguration: MemberConfigurationTypeDef,
         Description: str = ...,
         FrameworkConfiguration: NetworkFrameworkConfigurationTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateNetworkOutputTypeDef:
         """
         Creates a new blockchain network using Amazon Managed Blockchain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_network)
         """
@@ -175,32 +174,32 @@
     def create_node(
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         NodeConfiguration: NodeConfigurationTypeDef,
         MemberId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateNodeOutputTypeDef:
         """
         Creates a node on the specified blockchain network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_node)
         """
 
     def create_proposal(
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         MemberId: str,
-        Actions: ProposalActionsTypeDef,
+        Actions: ProposalActionsUnionTypeDef,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateProposalOutputTypeDef:
         """
         Creates a proposal for a change to the network that other members of the
         network can vote on, for example, a proposal to add a new member to the
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_proposal)
@@ -286,15 +285,15 @@
         """
 
     def list_accessors(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        NetworkType: AccessorNetworkTypeType = ...
+        NetworkType: AccessorNetworkTypeType = ...,
     ) -> ListAccessorsOutputTypeDef:
         """
         Returns a list of the accessors and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_accessors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_accessors)
         """
@@ -313,15 +312,15 @@
         self,
         *,
         NetworkId: str,
         Name: str = ...,
         Status: MemberStatusType = ...,
         IsOwned: bool = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListMembersOutputTypeDef:
         """
         Returns a list of the members in a network and properties of their
         configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_members)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_members)
@@ -330,15 +329,15 @@
     def list_networks(
         self,
         *,
         Name: str = ...,
         Framework: FrameworkType = ...,
         Status: NetworkStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListNetworksOutputTypeDef:
         """
         Returns information about the networks in which the current Amazon Web Services
         account
         participates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_networks)
@@ -348,15 +347,15 @@
     def list_nodes(
         self,
         *,
         NetworkId: str,
         MemberId: str = ...,
         Status: NodeStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListNodesOutputTypeDef:
         """
         Returns information about the nodes within a network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_nodes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_nodes)
         """
@@ -418,30 +417,30 @@
         """
 
     def update_member(
         self,
         *,
         NetworkId: str,
         MemberId: str,
-        LogPublishingConfiguration: MemberLogPublishingConfigurationTypeDef = ...
+        LogPublishingConfiguration: MemberLogPublishingConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates a member configuration with new parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.update_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#update_member)
         """
 
     def update_node(
         self,
         *,
         NetworkId: str,
         NodeId: str,
         MemberId: str = ...,
-        LogPublishingConfiguration: NodeLogPublishingConfigurationTypeDef = ...
+        LogPublishingConfiguration: NodeLogPublishingConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates a node configuration with new parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.update_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#update_node)
         """
```

### Comparing `mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/client.pyi` & `mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     ListProposalVotesOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     MemberConfigurationTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
-    ProposalActionsTypeDef,
+    ProposalActionsUnionTypeDef,
     VotingPolicyTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -118,15 +118,15 @@
 
     def create_accessor(
         self,
         *,
         ClientRequestToken: str,
         AccessorType: Literal["BILLING_TOKEN"],
         Tags: Mapping[str, str] = ...,
-        NetworkType: AccessorNetworkTypeType = ...
+        NetworkType: AccessorNetworkTypeType = ...,
     ) -> CreateAccessorOutputTypeDef:
         """
         Creates a new accessor for use with Amazon Managed Blockchain service that
         supports token based
         access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_accessor)
@@ -135,15 +135,15 @@
 
     def create_member(
         self,
         *,
         ClientRequestToken: str,
         InvitationId: str,
         NetworkId: str,
-        MemberConfiguration: MemberConfigurationTypeDef
+        MemberConfiguration: MemberConfigurationTypeDef,
     ) -> CreateMemberOutputTypeDef:
         """
         Creates a member within a Managed Blockchain network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_member)
         """
@@ -155,15 +155,15 @@
         Name: str,
         Framework: FrameworkType,
         FrameworkVersion: str,
         VotingPolicy: VotingPolicyTypeDef,
         MemberConfiguration: MemberConfigurationTypeDef,
         Description: str = ...,
         FrameworkConfiguration: NetworkFrameworkConfigurationTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateNetworkOutputTypeDef:
         """
         Creates a new blockchain network using Amazon Managed Blockchain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_network)
         """
@@ -171,32 +171,32 @@
     def create_node(
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         NodeConfiguration: NodeConfigurationTypeDef,
         MemberId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateNodeOutputTypeDef:
         """
         Creates a node on the specified blockchain network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#create_node)
         """
 
     def create_proposal(
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         MemberId: str,
-        Actions: ProposalActionsTypeDef,
+        Actions: ProposalActionsUnionTypeDef,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateProposalOutputTypeDef:
         """
         Creates a proposal for a change to the network that other members of the
         network can vote on, for example, a proposal to add a new member to the
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_proposal)
@@ -282,15 +282,15 @@
         """
 
     def list_accessors(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        NetworkType: AccessorNetworkTypeType = ...
+        NetworkType: AccessorNetworkTypeType = ...,
     ) -> ListAccessorsOutputTypeDef:
         """
         Returns a list of the accessors and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_accessors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_accessors)
         """
@@ -309,15 +309,15 @@
         self,
         *,
         NetworkId: str,
         Name: str = ...,
         Status: MemberStatusType = ...,
         IsOwned: bool = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListMembersOutputTypeDef:
         """
         Returns a list of the members in a network and properties of their
         configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_members)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_members)
@@ -326,15 +326,15 @@
     def list_networks(
         self,
         *,
         Name: str = ...,
         Framework: FrameworkType = ...,
         Status: NetworkStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListNetworksOutputTypeDef:
         """
         Returns information about the networks in which the current Amazon Web Services
         account
         participates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_networks)
@@ -344,15 +344,15 @@
     def list_nodes(
         self,
         *,
         NetworkId: str,
         MemberId: str = ...,
         Status: NodeStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListNodesOutputTypeDef:
         """
         Returns information about the nodes within a network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_nodes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#list_nodes)
         """
@@ -414,30 +414,30 @@
         """
 
     def update_member(
         self,
         *,
         NetworkId: str,
         MemberId: str,
-        LogPublishingConfiguration: MemberLogPublishingConfigurationTypeDef = ...
+        LogPublishingConfiguration: MemberLogPublishingConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates a member configuration with new parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.update_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#update_member)
         """
 
     def update_node(
         self,
         *,
         NetworkId: str,
         NodeId: str,
         MemberId: str = ...,
-        LogPublishingConfiguration: NodeLogPublishingConfigurationTypeDef = ...
+        LogPublishingConfiguration: NodeLogPublishingConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates a node configuration with new parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.update_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/client/#update_node)
         """
```

### Comparing `mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/literals.py` & `mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AccessorNetworkTypeType",
     "AccessorStatusType",
     "AccessorTypeType",
     "EditionType",
     "FrameworkType",
     "InvitationStatusType",
@@ -38,15 +37,14 @@
     "ManagedBlockchainServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccessorNetworkTypeType = Literal[
     "ETHEREUM_GOERLI",
     "ETHEREUM_MAINNET",
     "ETHEREUM_MAINNET_AND_GOERLI",
     "POLYGON_MAINNET",
     "POLYGON_MUMBAI",
 ]
@@ -104,14 +102,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -122,14 +121,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -147,14 +147,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -167,24 +168,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -245,15 +248,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -295,14 +297,15 @@
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
+    "mailmanager",
     "managedblockchain",
     "managedblockchain-query",
     "marketplace-agreement",
     "marketplace-catalog",
     "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
@@ -325,17 +328,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -380,14 +385,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -425,19 +431,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/literals.pyi` & `mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -120,14 +121,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -145,14 +147,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -165,24 +168,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -243,15 +248,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -293,14 +297,15 @@
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
+    "mailmanager",
     "managedblockchain",
     "managedblockchain-query",
     "marketplace-agreement",
     "marketplace-catalog",
     "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
@@ -323,17 +328,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -378,14 +385,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -423,19 +431,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/paginator.py` & `mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import AccessorNetworkTypeType
 from .type_defs import ListAccessorsOutputTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListAccessorsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -46,13 +45,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/paginators/#listaccessorspaginator)
     """
 
     def paginate(
         self,
         *,
         NetworkType: AccessorNetworkTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListAccessorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Paginator.ListAccessors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/paginators/#listaccessorspaginator)
         """
```

### Comparing `mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/paginator.pyi` & `mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,13 +43,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/paginators/#listaccessorspaginator)
     """
 
     def paginate(
         self,
         *,
         NetworkType: AccessorNetworkTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListAccessorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Paginator.ListAccessors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/paginators/#listaccessorspaginator)
         """
```

### Comparing `mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/type_defs.py` & `mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AccessorSummaryTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccessorNetworkTypeType,
     AccessorStatusType,
     EditionType,
     FrameworkType,
     InvitationStatusType,
@@ -40,15 +40,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessorSummaryTypeDef",
     "AccessorTypeDef",
     "ApprovalThresholdPolicyTypeDef",
     "CreateAccessorInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteAccessorInputRequestTypeDef",
@@ -105,21 +104,23 @@
     "ListProposalsOutputTypeDef",
     "LogConfigurationsTypeDef",
     "MemberFrameworkAttributesTypeDef",
     "MemberFrameworkConfigurationTypeDef",
     "NetworkFrameworkAttributesTypeDef",
     "NetworkFrameworkConfigurationTypeDef",
     "NodeFrameworkAttributesTypeDef",
+    "ProposalActionsOutputTypeDef",
     "ProposalActionsTypeDef",
     "ListInvitationsOutputTypeDef",
     "MemberFabricLogPublishingConfigurationTypeDef",
     "NodeFabricLogPublishingConfigurationTypeDef",
     "NetworkTypeDef",
-    "CreateProposalInputRequestTypeDef",
     "ProposalTypeDef",
+    "CreateProposalInputRequestTypeDef",
+    "ProposalActionsUnionTypeDef",
     "MemberLogPublishingConfigurationTypeDef",
     "NodeLogPublishingConfigurationTypeDef",
     "GetNetworkOutputTypeDef",
     "GetProposalOutputTypeDef",
     "MemberConfigurationTypeDef",
     "MemberTypeDef",
     "UpdateMemberInputRequestTypeDef",
@@ -174,18 +175,18 @@
         "NetworkType": NotRequired[AccessorNetworkTypeType],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 DeleteAccessorInputRequestTypeDef = TypedDict(
     "DeleteAccessorInputRequestTypeDef",
     {
         "AccessorId": str,
     },
@@ -518,16 +519,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListAccessorsOutputTypeDef = TypedDict(
     "ListAccessorsOutputTypeDef",
     {
         "Accessors": List[AccessorSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -544,55 +545,55 @@
         "Arn": NotRequired[str],
     },
 )
 ListNetworksOutputTypeDef = TypedDict(
     "ListNetworksOutputTypeDef",
     {
         "Networks": List[NetworkSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListAccessorsInputListAccessorsPaginateTypeDef = TypedDict(
     "ListAccessorsInputListAccessorsPaginateTypeDef",
     {
         "NetworkType": NotRequired[AccessorNetworkTypeType],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListMembersOutputTypeDef = TypedDict(
     "ListMembersOutputTypeDef",
     {
         "Members": List[MemberSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListNodesOutputTypeDef = TypedDict(
     "ListNodesOutputTypeDef",
     {
         "Nodes": List[NodeSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListProposalVotesOutputTypeDef = TypedDict(
     "ListProposalVotesOutputTypeDef",
     {
         "ProposalVotes": List[VoteSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListProposalsOutputTypeDef = TypedDict(
     "ListProposalsOutputTypeDef",
     {
         "Proposals": List[ProposalSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 LogConfigurationsTypeDef = TypedDict(
     "LogConfigurationsTypeDef",
     {
         "Cloudwatch": NotRequired[LogConfigurationTypeDef],
     },
@@ -625,27 +626,34 @@
 NodeFrameworkAttributesTypeDef = TypedDict(
     "NodeFrameworkAttributesTypeDef",
     {
         "Fabric": NotRequired[NodeFabricAttributesTypeDef],
         "Ethereum": NotRequired[NodeEthereumAttributesTypeDef],
     },
 )
+ProposalActionsOutputTypeDef = TypedDict(
+    "ProposalActionsOutputTypeDef",
+    {
+        "Invitations": NotRequired[List[InviteActionTypeDef]],
+        "Removals": NotRequired[List[RemoveActionTypeDef]],
+    },
+)
 ProposalActionsTypeDef = TypedDict(
     "ProposalActionsTypeDef",
     {
         "Invitations": NotRequired[Sequence[InviteActionTypeDef]],
         "Removals": NotRequired[Sequence[RemoveActionTypeDef]],
     },
 )
 ListInvitationsOutputTypeDef = TypedDict(
     "ListInvitationsOutputTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 MemberFabricLogPublishingConfigurationTypeDef = TypedDict(
     "MemberFabricLogPublishingConfigurationTypeDef",
     {
         "CaLogs": NotRequired[LogConfigurationsTypeDef],
     },
@@ -670,44 +678,45 @@
         "VotingPolicy": NotRequired[VotingPolicyTypeDef],
         "Status": NotRequired[NetworkStatusType],
         "CreationDate": NotRequired[datetime],
         "Tags": NotRequired[Dict[str, str]],
         "Arn": NotRequired[str],
     },
 )
-CreateProposalInputRequestTypeDef = TypedDict(
-    "CreateProposalInputRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "NetworkId": str,
-        "MemberId": str,
-        "Actions": ProposalActionsTypeDef,
-        "Description": NotRequired[str],
-        "Tags": NotRequired[Mapping[str, str]],
-    },
-)
 ProposalTypeDef = TypedDict(
     "ProposalTypeDef",
     {
         "ProposalId": NotRequired[str],
         "NetworkId": NotRequired[str],
         "Description": NotRequired[str],
-        "Actions": NotRequired[ProposalActionsTypeDef],
+        "Actions": NotRequired[ProposalActionsOutputTypeDef],
         "ProposedByMemberId": NotRequired[str],
         "ProposedByMemberName": NotRequired[str],
         "Status": NotRequired[ProposalStatusType],
         "CreationDate": NotRequired[datetime],
         "ExpirationDate": NotRequired[datetime],
         "YesVoteCount": NotRequired[int],
         "NoVoteCount": NotRequired[int],
         "OutstandingVoteCount": NotRequired[int],
         "Tags": NotRequired[Dict[str, str]],
         "Arn": NotRequired[str],
     },
 )
+CreateProposalInputRequestTypeDef = TypedDict(
+    "CreateProposalInputRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "NetworkId": str,
+        "MemberId": str,
+        "Actions": ProposalActionsTypeDef,
+        "Description": NotRequired[str],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
+ProposalActionsUnionTypeDef = Union[ProposalActionsTypeDef, ProposalActionsOutputTypeDef]
 MemberLogPublishingConfigurationTypeDef = TypedDict(
     "MemberLogPublishingConfigurationTypeDef",
     {
         "Fabric": NotRequired[MemberFabricLogPublishingConfigurationTypeDef],
     },
 )
 NodeLogPublishingConfigurationTypeDef = TypedDict(
```

### Comparing `mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain/type_defs.pyi` & `mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AccessorSummaryTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccessorNetworkTypeType,
     AccessorStatusType,
     EditionType,
     FrameworkType,
     InvitationStatusType,
@@ -104,21 +104,23 @@
     "ListProposalsOutputTypeDef",
     "LogConfigurationsTypeDef",
     "MemberFrameworkAttributesTypeDef",
     "MemberFrameworkConfigurationTypeDef",
     "NetworkFrameworkAttributesTypeDef",
     "NetworkFrameworkConfigurationTypeDef",
     "NodeFrameworkAttributesTypeDef",
+    "ProposalActionsOutputTypeDef",
     "ProposalActionsTypeDef",
     "ListInvitationsOutputTypeDef",
     "MemberFabricLogPublishingConfigurationTypeDef",
     "NodeFabricLogPublishingConfigurationTypeDef",
     "NetworkTypeDef",
-    "CreateProposalInputRequestTypeDef",
     "ProposalTypeDef",
+    "CreateProposalInputRequestTypeDef",
+    "ProposalActionsUnionTypeDef",
     "MemberLogPublishingConfigurationTypeDef",
     "NodeLogPublishingConfigurationTypeDef",
     "GetNetworkOutputTypeDef",
     "GetProposalOutputTypeDef",
     "MemberConfigurationTypeDef",
     "MemberTypeDef",
     "UpdateMemberInputRequestTypeDef",
@@ -173,18 +175,18 @@
         "NetworkType": NotRequired[AccessorNetworkTypeType],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 DeleteAccessorInputRequestTypeDef = TypedDict(
     "DeleteAccessorInputRequestTypeDef",
     {
         "AccessorId": str,
     },
@@ -517,16 +519,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListAccessorsOutputTypeDef = TypedDict(
     "ListAccessorsOutputTypeDef",
     {
         "Accessors": List[AccessorSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -543,55 +545,55 @@
         "Arn": NotRequired[str],
     },
 )
 ListNetworksOutputTypeDef = TypedDict(
     "ListNetworksOutputTypeDef",
     {
         "Networks": List[NetworkSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListAccessorsInputListAccessorsPaginateTypeDef = TypedDict(
     "ListAccessorsInputListAccessorsPaginateTypeDef",
     {
         "NetworkType": NotRequired[AccessorNetworkTypeType],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListMembersOutputTypeDef = TypedDict(
     "ListMembersOutputTypeDef",
     {
         "Members": List[MemberSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListNodesOutputTypeDef = TypedDict(
     "ListNodesOutputTypeDef",
     {
         "Nodes": List[NodeSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListProposalVotesOutputTypeDef = TypedDict(
     "ListProposalVotesOutputTypeDef",
     {
         "ProposalVotes": List[VoteSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListProposalsOutputTypeDef = TypedDict(
     "ListProposalsOutputTypeDef",
     {
         "Proposals": List[ProposalSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 LogConfigurationsTypeDef = TypedDict(
     "LogConfigurationsTypeDef",
     {
         "Cloudwatch": NotRequired[LogConfigurationTypeDef],
     },
@@ -624,27 +626,34 @@
 NodeFrameworkAttributesTypeDef = TypedDict(
     "NodeFrameworkAttributesTypeDef",
     {
         "Fabric": NotRequired[NodeFabricAttributesTypeDef],
         "Ethereum": NotRequired[NodeEthereumAttributesTypeDef],
     },
 )
+ProposalActionsOutputTypeDef = TypedDict(
+    "ProposalActionsOutputTypeDef",
+    {
+        "Invitations": NotRequired[List[InviteActionTypeDef]],
+        "Removals": NotRequired[List[RemoveActionTypeDef]],
+    },
+)
 ProposalActionsTypeDef = TypedDict(
     "ProposalActionsTypeDef",
     {
         "Invitations": NotRequired[Sequence[InviteActionTypeDef]],
         "Removals": NotRequired[Sequence[RemoveActionTypeDef]],
     },
 )
 ListInvitationsOutputTypeDef = TypedDict(
     "ListInvitationsOutputTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 MemberFabricLogPublishingConfigurationTypeDef = TypedDict(
     "MemberFabricLogPublishingConfigurationTypeDef",
     {
         "CaLogs": NotRequired[LogConfigurationsTypeDef],
     },
@@ -669,44 +678,45 @@
         "VotingPolicy": NotRequired[VotingPolicyTypeDef],
         "Status": NotRequired[NetworkStatusType],
         "CreationDate": NotRequired[datetime],
         "Tags": NotRequired[Dict[str, str]],
         "Arn": NotRequired[str],
     },
 )
-CreateProposalInputRequestTypeDef = TypedDict(
-    "CreateProposalInputRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "NetworkId": str,
-        "MemberId": str,
-        "Actions": ProposalActionsTypeDef,
-        "Description": NotRequired[str],
-        "Tags": NotRequired[Mapping[str, str]],
-    },
-)
 ProposalTypeDef = TypedDict(
     "ProposalTypeDef",
     {
         "ProposalId": NotRequired[str],
         "NetworkId": NotRequired[str],
         "Description": NotRequired[str],
-        "Actions": NotRequired[ProposalActionsTypeDef],
+        "Actions": NotRequired[ProposalActionsOutputTypeDef],
         "ProposedByMemberId": NotRequired[str],
         "ProposedByMemberName": NotRequired[str],
         "Status": NotRequired[ProposalStatusType],
         "CreationDate": NotRequired[datetime],
         "ExpirationDate": NotRequired[datetime],
         "YesVoteCount": NotRequired[int],
         "NoVoteCount": NotRequired[int],
         "OutstandingVoteCount": NotRequired[int],
         "Tags": NotRequired[Dict[str, str]],
         "Arn": NotRequired[str],
     },
 )
+CreateProposalInputRequestTypeDef = TypedDict(
+    "CreateProposalInputRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "NetworkId": str,
+        "MemberId": str,
+        "Actions": ProposalActionsTypeDef,
+        "Description": NotRequired[str],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
+ProposalActionsUnionTypeDef = Union[ProposalActionsTypeDef, ProposalActionsOutputTypeDef]
 MemberLogPublishingConfigurationTypeDef = TypedDict(
     "MemberLogPublishingConfigurationTypeDef",
     {
         "Fabric": NotRequired[MemberFabricLogPublishingConfigurationTypeDef],
     },
 )
 NodeLogPublishingConfigurationTypeDef = TypedDict(
```

### Comparing `mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain.egg-info/PKG-INFO` & `mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-managedblockchain
-Version: 1.34.0
-Summary: Type annotations for boto3.ManagedBlockchain 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.113
+Summary: Type annotations for boto3.ManagedBlockchain 1.34.113 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-managedblockchain"></a>
 
 # mypy-boto3-managedblockchain
 
 [![PyPI - mypy-boto3-managedblockchain](https://img.shields.io/pypi/v/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain)](https://pepy.tech/project/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.34.113](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-managedblockchain-1.34.0/mypy_boto3_managedblockchain.egg-info/SOURCES.txt` & `mypy_boto3_managedblockchain-1.34.113/mypy_boto3_managedblockchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.34.0/setup.py` & `mypy_boto3_managedblockchain-1.34.113/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-managedblockchain",
-    version="1.34.0",
+    version="1.34.113",
     packages=["mypy_boto3_managedblockchain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.ManagedBlockchain 1.34.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.ManagedBlockchain 1.34.113 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 managedblockchain type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_managedblockchain": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

