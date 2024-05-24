# Comparing `tmp/funnylog-2023.8.23.tar.gz` & `tmp/funnylog-2024.5.24.tar.gz`

## Comparing `funnylog-2023.8.23.tar` & `funnylog-2024.5.24.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    12984 2020-02-02 00:00:00.000000 funnylog-2023.8.23/funnylog/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 funnylog-2023.8.23/funnylog/__version__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 funnylog-2023.8.23/funnylog/conf.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 funnylog-2023.8.23/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 funnylog-2023.8.23/LICENSE
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 funnylog-2023.8.23/README.md
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 funnylog-2023.8.23/pyproject.toml
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 funnylog-2023.8.23/PKG-INFO
+-rw-r--r--   0        0        0    13155 2020-02-02 00:00:00.000000 funnylog-2024.5.24/funnylog/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 funnylog-2024.5.24/funnylog/__version__.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 funnylog-2024.5.24/funnylog/conf.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 funnylog-2024.5.24/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 funnylog-2024.5.24/LICENSE
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 funnylog-2024.5.24/NOTICE
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 funnylog-2024.5.24/README.md
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 funnylog-2024.5.24/pyproject.toml
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 funnylog-2024.5.24/PKG-INFO
```

### Comparing `funnylog-2023.8.23/funnylog/__init__.py` & `funnylog-2024.5.24/funnylog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#!/usr/bin/env python3
+# _*_ coding:utf-8 _*_
+
+# SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
+
+# SPDX-License-Identifier: Apache Software License
 import inspect
 import logging
 import os
 import re
 import sys
 import threading
 import time
@@ -111,15 +117,15 @@
         args = list(map(lambda x: represent(x), a))
         if func.__doc__:
             if not func.__name__.startswith("_"):
                 # 处理多行注释时候，换行空格过多
                 title = re.split(":param|@param|@return|:return", func.__doc__)[0]
                 title = "".join([ln.strip() for ln in title.split("\n")])
                 params_text = {}
-                # 获取方法的所有参数，并行程，{形参：实参} 的字典
+                # 获取方法的所有参数，并组装为 {形参：实参} 的字典
                 for index, param in enumerate(
                         inspect.signature(func).parameters.values()
                 ):
                     if param.name == "self":
                         continue
                     params_text[param.name] = param.default
                     if args:
```

### Comparing `funnylog-2023.8.23/funnylog/conf.py` & `funnylog-2024.5.24/funnylog/conf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#!/usr/bin/env python3
+# _*_ coding:utf-8 _*_
+
+# SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
+
+# SPDX-License-Identifier: Apache Software License
 import os
 from getpass import getuser
 from platform import machine
 
 
 class _Setting:
```

### Comparing `funnylog-2023.8.23/.gitignore` & `funnylog-2024.5.24/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
-
+.idea
 # PyBuilder
 .pybuilder/
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
 
@@ -88,16 +88,16 @@
 # .python-version
 
 # pipenv
 #   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
 #   However, in case of collaboration, if having platform-specific dependencies or dependencies
 #   having no cross-platform support, pipenv may install dependencies that don't work, or not
 #   install all needed dependencies.
-#Pipfile.lock
-
+Pipfile.lock
+Pipfile
 # poetry
 #   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
 #   This is especially recommended for binary packages to ensure reproducibility, and is more
 #   commonly ignored for libraries.
 #   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
 #poetry.lock
```

### Comparing `funnylog-2023.8.23/LICENSE` & `funnylog-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `funnylog-2023.8.23/README.md` & `funnylog-2024.5.24/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 一个简单易用、功能强大的日志工具。
 
 只需要加一个装饰器，就能自动日志输出类里面所有的方法的功能说明。
 
 ---
 
-**Documentation**: <a href="https://funny-dream.github.io/funnylog" target="_blank">https://funny-dream.github.io/funnylog</a>
+**Documentation**: <a href="https://linuxdeepin.github.io/funnylog" target="_blank">https://linuxdeepin.github.io/funnylog</a>
 
-**Source Code**: <a href="https://github.com/funny-dream/funnylog" target="_blank">https://github.com/funny-dream/funnylog</a>
+**Source Code**: <a href="https://github.com/linuxdeepin/funnylog" target="_blank">https://github.com/linuxdeepin/funnylog</a>
 
 ---
 
 ## 安装
 
 ```console
 pip install funnylog
```

### Comparing `funnylog-2023.8.23/pyproject.toml` & `funnylog-2024.5.24/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "funnylog"
 authors = [
   { name="mikigo", email="1964191531@qq.com" },
 ]
 description = "PaddleOCR-RPC"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
@@ -36,9 +36,9 @@
 [tool.hatch.build.targets.sdist]
 include = [
     "/funnylog",
     "/README.md",
 ]
 
 [project.urls]
-Source = "https://github.com/funny-dream/funnylog"
-Documentation = "https://funny-dream.github.io/funnylog"
+Source = "https://github.com/linuxdeepin/funnylog"
+Documentation = "https://linuxdeepin.github.io/funnylog"
```

### Comparing `funnylog-2023.8.23/PKG-INFO` & `funnylog-2024.5.24/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: funnylog
-Version: 2023.8.23
+Version: 2024.5.24
 Summary: PaddleOCR-RPC
-Project-URL: Source, https://github.com/funny-dream/funnylog
-Project-URL: Documentation, https://funny-dream.github.io/funnylog
+Project-URL: Source, https://github.com/linuxdeepin/funnylog
+Project-URL: Documentation, https://linuxdeepin.github.io/funnylog
 Author-email: mikigo <1964191531@qq.com>
 License-File: LICENSE
+License-File: NOTICE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Requires-Dist: allure-pytest
 Provides-Extra: doc
 Requires-Dist: mkdocs-material; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
@@ -21,17 +22,17 @@
 
 一个简单易用、功能强大的日志工具。
 
 只需要加一个装饰器，就能自动日志输出类里面所有的方法的功能说明。
 
 ---
 
-**Documentation**: <a href="https://funny-dream.github.io/funnylog" target="_blank">https://funny-dream.github.io/funnylog</a>
+**Documentation**: <a href="https://linuxdeepin.github.io/funnylog" target="_blank">https://linuxdeepin.github.io/funnylog</a>
 
-**Source Code**: <a href="https://github.com/funny-dream/funnylog" target="_blank">https://github.com/funny-dream/funnylog</a>
+**Source Code**: <a href="https://github.com/linuxdeepin/funnylog" target="_blank">https://github.com/linuxdeepin/funnylog</a>
 
 ---
 
 ## 安装
 
 ```console
 pip install funnylog
```

