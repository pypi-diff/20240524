# Comparing `tmp/nonebot_plugin_plus_one-0.1.0.tar.gz` & `tmp/nonebot_plugin_plus_one-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_plus_one-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_plus_one-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_plus_one-0.1.0.tar` & `nonebot_plugin_plus_one-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      489 2024-05-23 09:02:44.933514 nonebot_plugin_plus_one-0.1.0/nonebot_plugin_plus_one/__init__.py
--rw-r--r--   0        0        0      242 2024-05-23 08:30:17.093577 nonebot_plugin_plus_one-0.1.0/nonebot_plugin_plus_one/config.py
--rw-r--r--   0        0        0      931 2024-05-23 09:14:29.978513 nonebot_plugin_plus_one-0.1.0/nonebot_plugin_plus_one/handler.py
--rw-r--r--   0        0        0      580 2024-05-23 09:23:54.470707 nonebot_plugin_plus_one-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1182 2024-05-23 09:00:23.122049 nonebot_plugin_plus_one-0.1.0/README.md
--rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 nonebot_plugin_plus_one-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      489 2024-05-23 09:02:44.933514 nonebot_plugin_plus_one-0.1.1/nonebot_plugin_plus_one/__init__.py
+-rw-r--r--   0        0        0      242 2024-05-23 08:30:17.093577 nonebot_plugin_plus_one-0.1.1/nonebot_plugin_plus_one/config.py
+-rw-r--r--   0        0        0      931 2024-05-23 09:14:29.978513 nonebot_plugin_plus_one-0.1.1/nonebot_plugin_plus_one/handler.py
+-rw-r--r--   0        0        0      599 2024-05-23 09:31:04.829185 nonebot_plugin_plus_one-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1182 2024-05-23 09:00:23.122049 nonebot_plugin_plus_one-0.1.1/README.md
+-rw-r--r--   0        0        0     1995 1970-01-01 00:00:00.000000 nonebot_plugin_plus_one-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_plus_one-0.1.0/nonebot_plugin_plus_one/handler.py` & `nonebot_plugin_plus_one-0.1.1/nonebot_plugin_plus_one/handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_plus_one-0.1.0/pyproject.toml` & `nonebot_plugin_plus_one-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "nonebot-plugin-plus-one"
-version = "0.1.0"
+version = "0.1.1"
 description = "全新复读姬，任意群聊触发 +1，姬就 +1。轻巧、专注，不使用任何数据库，不使用任何文件存储"
 authors = ["yejue <1145331931@qq.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
+nonebot2 = "^2.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
```

### Comparing `nonebot_plugin_plus_one-0.1.0/README.md` & `nonebot_plugin_plus_one-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_plus_one-0.1.0/PKG-INFO` & `nonebot_plugin_plus_one-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-plus-one
-Version: 0.1.0
+Version: 0.1.1
 Summary: 全新复读姬，任意群聊触发 +1，姬就 +1。轻巧、专注，不使用任何数据库，不使用任何文件存储
 License: MIT
 Author: yejue
 Author-email: 1145331931@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: nonebot2 (>=2.0,<3.0)
 Project-URL: homepage, https://github.com/yejue/nonebot-plugin-plus-one
 Project-URL: repository, https://github.com/yejue/nonebot-plugin-plus-one
 Description-Content-Type: text/markdown
 
 
 <h1 align="center">🐣🐤只是一个复读姬 ✨</h1>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-plus-one Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-plus-one Version: 0.1.1 Summary:
 å¨æ°å¤è¯»å§¬ï¼ä»»æç¾¤èè§¦å +1ï¼å§¬å°±
 +1ãè½»å·§ãä¸æ³¨ï¼ä¸ä½¿ç¨ä»»ä½æ°æ®åºï¼ä¸ä½¿ç¨ä»»ä½æä»¶å­å¨
 License: MIT Author: yejue Author-email: 1145331931@qq.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Project-URL:
-homepage, https://github.com/yejue/nonebot-plugin-plus-one Project-URL:
-repository, https://github.com/yejue/nonebot-plugin-plus-one Description-
-Content-Type: text/markdown
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
+Dist: nonebot2 (>=2.0,<3.0) Project-URL: homepage, https://github.com/yejue/
+nonebot-plugin-plus-one Project-URL: repository, https://github.com/yejue/
+nonebot-plugin-plus-one Description-Content-Type: text/markdown
                 ************ ?ð???£?ð???¤?å??ª?æ??¯?ä?¸??ä?¸?ª?å?¤??è?¯?»?å?§?¬ ?â??¨ ************
                         _â¨ åªæ¯ä¸ä¸ªå¤è¯»å§¬ â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## å¿«éå®è£ ç¬¬ä¸æ­¥ï¼å³ä¸è§ â ç¹ä¸ªä¸è¦é±ç star
 å§ï¼è¿æ¯ä¸æ­ç»´æ¤æ´æ°çå¨åã ### nb-cli ```shell nb plugin
 install nonebot-plugin-plus-one ``` ### pip ```shell pip install nonebot-
 plugin-plus-one ``` ### git ```shell cd /your-nonebot-project-home/plugins/ git
```

