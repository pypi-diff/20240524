# Comparing `tmp/nonebot_plugin_plus_one-0.1.1.tar.gz` & `tmp/nonebot_plugin_plus_one-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_plus_one-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_plus_one-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_plus_one-0.1.1.tar` & `nonebot_plugin_plus_one-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      489 2024-05-23 09:02:44.933514 nonebot_plugin_plus_one-0.1.1/nonebot_plugin_plus_one/__init__.py
--rw-r--r--   0        0        0      242 2024-05-23 08:30:17.093577 nonebot_plugin_plus_one-0.1.1/nonebot_plugin_plus_one/config.py
--rw-r--r--   0        0        0      931 2024-05-23 09:14:29.978513 nonebot_plugin_plus_one-0.1.1/nonebot_plugin_plus_one/handler.py
--rw-r--r--   0        0        0      599 2024-05-23 09:31:04.829185 nonebot_plugin_plus_one-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1182 2024-05-23 09:00:23.122049 nonebot_plugin_plus_one-0.1.1/README.md
--rw-r--r--   0        0        0     1995 1970-01-01 00:00:00.000000 nonebot_plugin_plus_one-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      536 2024-05-24 04:48:27.158177 nonebot_plugin_plus_one-0.1.2/nonebot_plugin_plus_one/__init__.py
+-rw-r--r--   0        0        0      312 2024-05-24 03:08:41.722147 nonebot_plugin_plus_one-0.1.2/nonebot_plugin_plus_one/config.py
+-rw-r--r--   0        0        0     1350 2024-05-24 04:49:07.055376 nonebot_plugin_plus_one-0.1.2/nonebot_plugin_plus_one/handler.py
+-rw-r--r--   0        0        0      635 2024-05-24 04:54:06.583758 nonebot_plugin_plus_one-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1391 2024-05-24 04:52:01.673109 nonebot_plugin_plus_one-0.1.2/README.md
+-rw-r--r--   0        0        0     2236 1970-01-01 00:00:00.000000 nonebot_plugin_plus_one-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_plus_one-0.1.1/README.md` & `nonebot_plugin_plus_one-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 <h1 align="center">🐣🐤只是一个复读姬 ✨</h1>
 <p align="center">
-_✨ 只是一个复读姬 ✨_
+_✨ 只是一个复读姬：支持群聊白名单、文本复读、图片表情复读 ✨_
 </p>
 <p align="center">
   <a href="https://raw.githubusercontent.com/cscs181/QQ-Github-Bot/master/LICENSE">
     <img src="https://img.shields.io/github/license/cscs181/QQ-Github-Bot.svg" alt="license">
   </a>
   <a href="https://pypi.python.org/pypi/nonebot-plugin-analysis-bilibili">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-analysis-bilibili.svg" alt="pypi">
@@ -47,8 +47,12 @@
 [机器人]: 表情
 ```
 
 ## 配置
 ```text
 # 匹配优先级
 PLUS_ONE_PRIORITY = 10
+
+# 群聊白名单，单个或多个示例，下面任选其一
+PLUS_ONE_WHITE_LIST = ["10000000"]
+PLUS_ONE_WHITE_LIST = ["10000000", "1000000"]
 ```
```

#### html2text {}

```diff
@@ -1,11 +1,16 @@
                 ************ ?ð???£?ð???¤?å??ª?æ??¯?ä?¸??ä?¸?ª?å?¤??è?¯?»?å?§?¬ ?â??¨ ************
-                        _â¨ åªæ¯ä¸ä¸ªå¤è¯»å§¬ â¨_
+                                     _â¨
+åªæ¯ä¸ä¸ªå¤è¯»å§¬ï¼æ¯æç¾¤èç½ååãææ¬å¤è¯»ãå¾çè¡¨æå¤è¯»
+                                     â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## å¿«éå®è£ ç¬¬ä¸æ­¥ï¼å³ä¸è§ â ç¹ä¸ªä¸è¦é±ç star
 å§ï¼è¿æ¯ä¸æ­ç»´æ¤æ´æ°çå¨åã ### nb-cli ```shell nb plugin
 install nonebot-plugin-plus-one ``` ### pip ```shell pip install nonebot-
 plugin-plus-one ``` ### git ```shell cd /your-nonebot-project-home/plugins/ git
 clone https://github.com/yejue/nonebot-plugin-plus-one.git ``` ## ç¤ºä¾
 ```text [ç¾¤1]: ä½ å¥½ [ç¾¤1]: ä½ å¥½ [æºå¨äºº]: ä½ å¥½ [ç¾¤2]: è¡¨æ
 [ç¾¤2]: è¡¨æ [æºå¨äºº]: è¡¨æ ``` ## éç½® ```text # å¹éä¼åçº§
-PLUS_ONE_PRIORITY = 10 ```
+PLUS_ONE_PRIORITY = 10 #
+ç¾¤èç½ååï¼åä¸ªæå¤ä¸ªç¤ºä¾ï¼ä¸é¢ä»»éå¶ä¸
+PLUS_ONE_WHITE_LIST = ["10000000"] PLUS_ONE_WHITE_LIST = ["10000000",
+"1000000"] ```
```

### Comparing `nonebot_plugin_plus_one-0.1.1/PKG-INFO` & `nonebot_plugin_plus_one-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-plus-one
-Version: 0.1.1
-Summary: 全新复读姬，任意群聊触发 +1，姬就 +1。轻巧、专注，不使用任何数据库，不使用任何文件存储
+Version: 0.1.2
+Summary: 全新复读姬，支持文本、图片表情复读。任意群聊触发 +1，姬就 +1。轻巧、专注，不使用任何数据库，不使用任何文件存储
 License: MIT
 Author: yejue
 Author-email: 1145331931@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,15 +17,15 @@
 Project-URL: homepage, https://github.com/yejue/nonebot-plugin-plus-one
 Project-URL: repository, https://github.com/yejue/nonebot-plugin-plus-one
 Description-Content-Type: text/markdown
 
 
 <h1 align="center">🐣🐤只是一个复读姬 ✨</h1>
 <p align="center">
-_✨ 只是一个复读姬 ✨_
+_✨ 只是一个复读姬：支持群聊白名单、文本复读、图片表情复读 ✨_
 </p>
 <p align="center">
   <a href="https://raw.githubusercontent.com/cscs181/QQ-Github-Bot/master/LICENSE">
     <img src="https://img.shields.io/github/license/cscs181/QQ-Github-Bot.svg" alt="license">
   </a>
   <a href="https://pypi.python.org/pypi/nonebot-plugin-analysis-bilibili">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-analysis-bilibili.svg" alt="pypi">
@@ -67,9 +67,13 @@
 [机器人]: 表情
 ```
 
 ## 配置
 ```text
 # 匹配优先级
 PLUS_ONE_PRIORITY = 10
+
+# 群聊白名单，单个或多个示例，下面任选其一
+PLUS_ONE_WHITE_LIST = ["10000000"]
+PLUS_ONE_WHITE_LIST = ["10000000", "1000000"]
 ```
```

#### html2text {}

```diff
@@ -1,23 +1,29 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-plus-one Version: 0.1.1 Summary:
-å¨æ°å¤è¯»å§¬ï¼ä»»æç¾¤èè§¦å +1ï¼å§¬å°±
+Metadata-Version: 2.1 Name: nonebot-plugin-plus-one Version: 0.1.2 Summary:
+å¨æ°å¤è¯»å§¬ï¼æ¯æææ¬ãå¾çè¡¨æå¤è¯»ãä»»æç¾¤èè§¦å
++1ï¼å§¬å°±
 +1ãè½»å·§ãä¸æ³¨ï¼ä¸ä½¿ç¨ä»»ä½æ°æ®åºï¼ä¸ä½¿ç¨ä»»ä½æä»¶å­å¨
 License: MIT Author: yejue Author-email: 1145331931@qq.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: nonebot2 (>=2.0,<3.0) Project-URL: homepage, https://github.com/yejue/
 nonebot-plugin-plus-one Project-URL: repository, https://github.com/yejue/
 nonebot-plugin-plus-one Description-Content-Type: text/markdown
                 ************ ?ð???£?ð???¤?å??ª?æ??¯?ä?¸??ä?¸?ª?å?¤??è?¯?»?å?§?¬ ?â??¨ ************
-                        _â¨ åªæ¯ä¸ä¸ªå¤è¯»å§¬ â¨_
+                                     _â¨
+åªæ¯ä¸ä¸ªå¤è¯»å§¬ï¼æ¯æç¾¤èç½ååãææ¬å¤è¯»ãå¾çè¡¨æå¤è¯»
+                                     â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## å¿«éå®è£ ç¬¬ä¸æ­¥ï¼å³ä¸è§ â ç¹ä¸ªä¸è¦é±ç star
 å§ï¼è¿æ¯ä¸æ­ç»´æ¤æ´æ°çå¨åã ### nb-cli ```shell nb plugin
 install nonebot-plugin-plus-one ``` ### pip ```shell pip install nonebot-
 plugin-plus-one ``` ### git ```shell cd /your-nonebot-project-home/plugins/ git
 clone https://github.com/yejue/nonebot-plugin-plus-one.git ``` ## ç¤ºä¾
 ```text [ç¾¤1]: ä½ å¥½ [ç¾¤1]: ä½ å¥½ [æºå¨äºº]: ä½ å¥½ [ç¾¤2]: è¡¨æ
 [ç¾¤2]: è¡¨æ [æºå¨äºº]: è¡¨æ ``` ## éç½® ```text # å¹éä¼åçº§
-PLUS_ONE_PRIORITY = 10 ```
+PLUS_ONE_PRIORITY = 10 #
+ç¾¤èç½ååï¼åä¸ªæå¤ä¸ªç¤ºä¾ï¼ä¸é¢ä»»éå¶ä¸
+PLUS_ONE_WHITE_LIST = ["10000000"] PLUS_ONE_WHITE_LIST = ["10000000",
+"1000000"] ```
```

