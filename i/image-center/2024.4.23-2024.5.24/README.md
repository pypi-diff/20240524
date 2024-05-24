# Comparing `tmp/image_center-2024.4.23.tar.gz` & `tmp/image_center-2024.5.24.tar.gz`

## Comparing `image_center-2024.4.23.tar` & `image_center-2024.5.24.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    16300 2020-02-02 00:00:00.000000 image_center-2024.4.23/image_center/__init__.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 image_center-2024.4.23/image_center/__version__.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 image_center-2024.4.23/image_center/conf.py
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 image_center-2024.4.23/image_center/server.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 image_center-2024.4.23/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 image_center-2024.4.23/LICENSE
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 image_center-2024.4.23/README.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 image_center-2024.4.23/pyproject.toml
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 image_center-2024.4.23/PKG-INFO
+-rw-r--r--   0        0        0    17398 2020-02-02 00:00:00.000000 image_center-2024.5.24/image_center/__init__.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 image_center-2024.5.24/image_center/__version__.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 image_center-2024.5.24/image_center/conf.py
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 image_center-2024.5.24/image_center/server.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 image_center-2024.5.24/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 image_center-2024.5.24/LICENSE
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 image_center-2024.5.24/README.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 image_center-2024.5.24/pyproject.toml
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 image_center-2024.5.24/PKG-INFO
```

### Comparing `image_center-2024.4.23/image_center/__init__.py` & `image_center-2024.5.24/image_center/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,16 +72,16 @@
             multiple: bool = False,
             picture_abspath: str = None,
             screen_bbox: List[int] = None,
             log_level: str = "info",
             network_retry: int = 1,
     ):
         """
-         图像识别，匹配小图在屏幕中的坐标 x, y
-        :param image_path: 图像识别目标文件的存放路径
+         图像识别，匹配小图在屏幕中的坐标 x, y，当前仅支持1个主屏幕，如果存在多个屏幕只会截取主屏幕内容。
+        :param image_path: 图像识别目标文件的存放路径,仅支持英文文件名，不支持中文文件名
         :param rate: 匹配度
         :param multiple: 是否返回匹配到的多个目标
         :param picture_abspath: 大图，默认大图是截取屏幕，否则使用传入的图片；
         :param screen_bbox: 截取屏幕上指定区域图片（仅支持X11下使用）；
             [x, y, w, h]
             x: 左上角横坐标；y: 左上角纵坐标；w: 宽度；h: 高度；根据匹配度返回坐标
         :param network_retry: 连接服务器重试次数
@@ -96,19 +96,37 @@
                 screen = cls.save_temporary_picture(*screen_bbox) + ".png"
             else:
                 if setting.IS_X11:
                     try:
                         pyscreenshot.grab().save(screen)
                     except easyprocess.EasyProcessError:
                         ...
-                else:
+                elif setting.IS_WAYLAND:
                     screen = os.popen(cls.wayland_screen_dbus).read().strip("\n")
+                else:
+                    #for windows and macos
+                    pyscreenshot.grab().save(screen)
+
         else:
             screen = picture_abspath
-        template_path = os.path.expanduser(f"{image_path}.png")
+
+        # 如果传入的image_path参数不带文件后缀名，就根据文件类型判断文件是否存在，存在则将后缀类型（'.png','.jpg','.jpeg'）加上
+        if not image_path.endswith(('.png', '.jpg', '.jpeg')):
+            if os.path.exists(f"{image_path}.png"):
+                template_path = os.path.expanduser(f"{image_path}.png")
+            elif os.path.exists(f"{image_path}.jpg"):
+                template_path = os.path.expanduser(f"{image_path}.jpg")
+            elif os.path.exists(f"{image_path}.jpeg"):
+                template_path = os.path.expanduser(f"{image_path}.jpeg")
+            else:
+                logger.warning(f"The image format is not supported. Please confirm your image_path again")
+        else:
+            # image_path参数带有后缀名，不做任何添加
+            template_path = os.path.expanduser(f"{image_path}")
+
         if GET_OPENCV_FORM_RPC:
             server = ServerProxy(f"http://{setting.SERVER_IP}:{setting.PORT}", allow_none=True)
             # pylint: disable=consider-using-with
             screen_rb = open(screen, "rb")
             # pylint: disable=consider-using-with
             template_rb = open(template_path, "rb")
             for _ in range(network_retry + 1):
```

### Comparing `image_center-2024.4.23/image_center/conf.py` & `image_center-2024.5.24/image_center/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 # _*_ coding:utf-8 _*_
 
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 
 # SPDX-License-Identifier: Apache Software License
 import os
 import platform
-
+import tempfile
 
 class _Setting:
     PIC_PATH = ""
     IMAGE_RATE = 0.9
     SCREEN_CACHE = "/tmp/screen.png"
+    # Win default path——C:\\Users\\xxxx\\AppData\\Local\\Temp
+    # Linux_MacOS default path——/tmp/screen.png
+    SCREEN_CACHE = os.path.join(tempfile.gettempdir(), 'screen.png')  # /tmp/screen.png
     TMPDIR = "/tmp/tmpdir"
     # IMAGE_MATCH_NUMBER = 1
     # IMAGE_MATCH_WAIT_TIME = 1
 
     # RPC config
     SERVER_IP = ""
     PORT = 8889
@@ -34,11 +37,15 @@
 
         class DisplayServer:
             wayland = "wayland"
             x11 = "x11"
 
         IS_X11 = (DISPLAY_SERVER == DisplayServer.x11)
         IS_WAYLAND = (DISPLAY_SERVER == DisplayServer.wayland)
+    elif platform.system() == "Darwin":
+        IS_X11 = False
+        IS_WAYLAND = False
     elif platform.system() == "Windows":
-        ...
+        IS_X11 = False
+        IS_WAYLAND = False
 
 setting = _Setting()
```

### Comparing `image_center-2024.4.23/image_center/server.py` & `image_center-2024.5.24/image_center/server.py`

 * *Files identical despite different names*

### Comparing `image_center-2024.4.23/.gitignore` & `image_center-2024.5.24/.gitignore`

 * *Files identical despite different names*

### Comparing `image_center-2024.4.23/LICENSE` & `image_center-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `image_center-2024.4.23/README.md` & `image_center-2024.5.24/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,20 +21,24 @@
 
 ```shell
 sudo apt install python3-opencv
 ```
 
 ## 使用说明
 
-截取目标元素图片，将图片保存到某个路径；
+截取目标元素图片，将图片保存到某个路径,
+
+图片格式：默认使用PNG格式，支持JPG和JPEG格式；
 
 ```python
 from image_center import ImageCenter
-
+# Linux and MacOS
 ImageCenter.find_image("~/Desktop/test.png")
+# Windows
+ImageCenter.find_image("D:\\test.png")
 ```
 
 返回 `test.png` 在当前屏幕中的位置。
 
 ## RPC服务
 
 如果不想在本机安装OpenCV，或者你的机器无法安装OpenCV，可以在服务端安装OpenCV（安装方法和上面一样）；
@@ -57,9 +61,13 @@
 ```python
 from image_center import ImageCenter
 from image_center.conf import setting
 
 setting.SERCER_IP = "192.168.2.1"  # 服务端IP
 setting.PORT = 8889 # 和服务端端口保持一致
 
+# Linux and MacOS
 ImageCenter.find_image("~/Desktop/test.png") # test.png是你自己截的图，路径也修改成你自己的路径
+
+# Windows
+ImageCenter.find_image("D:\\test.png")
 ```
```

#### html2text {}

```diff
@@ -1,20 +1,24 @@
 # image-center å¾åè¯å«å®ä½æä¸ªåç´ å¨å½åå±å¹ä¸­çåæ ï¼
 å¨èªå¨åæµè¯ä¸­è·åå°åç´ åæ ä¹åï¼å¯ä»¥ä¼ å¥å°é®é¼ å·¥å·ï¼ä»èå®ç°å¯¹ç®æ åç´ çæä½ã
 --- **Documentation**: _h_t_t_p_s_:_/_/_l_i_n_u_x_d_e_e_p_i_n_._g_i_t_h_u_b_._i_o_/_i_m_a_g_e_-_c_e_n_t_e_r **Source
 Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_l_i_n_u_x_d_e_e_p_i_n_/_i_m_a_g_e_-_c_e_n_t_e_r --- ## å®è£ ```console
 pip install image-center ```
 å¦ææ³å¨æ¬æºç´æ¥ä½¿ç¨å¾åè¯å«ï¼è¿éè¦å¨æ¬æºå®è£OpenCV
 ```shell sudo apt install python3-opencv ``` ## ä½¿ç¨è¯´æ
-æªåç®æ åç´ å¾çï¼å°å¾çä¿å­å°æä¸ªè·¯å¾ï¼ ```python from
-image_center import ImageCenter ImageCenter.find_image("~/Desktop/test.png")
-``` è¿å `test.png` å¨å½åå±å¹ä¸­çä½ç½®ã ## RPCæå¡
+æªåç®æ åç´ å¾çï¼å°å¾çä¿å­å°æä¸ªè·¯å¾,
+å¾çæ ¼å¼ï¼é»è®¤ä½¿ç¨PNGæ ¼å¼ï¼æ¯æJPGåJPEGæ ¼å¼ï¼ ```python from
+image_center import ImageCenter # Linux and MacOS ImageCenter.find_image("~/
+Desktop/test.png") # Windows ImageCenter.find_image("D:\\test.png") ``` è¿å
+`test.png` å¨å½åå±å¹ä¸­çä½ç½®ã ## RPCæå¡
 å¦æä¸æ³å¨æ¬æºå®è£OpenCVï¼æèä½ çæºå¨æ æ³å®è£OpenCVï¼å¯ä»¥å¨æå¡ç«¯å®è£OpenCVï¼å®è£æ¹æ³åä¸é¢ä¸æ ·ï¼ï¼
 æå¡ç«¯å¯å¨æ¹æ³ï¼ ```python from image_center.server import server from
 image_center.conf import setting setting.PORT = 8889 #
 é»è®¤ç«¯å£æ¯8889ï¼å¯ä»¥ä¿®æ¹ä¸ºå¶ä»ç«¯å£ï¼ server() ```
 æ§è¡è¿ä¸ªä»£ç å°±å¯ä»¥å¯å¨æå¡äºï¼
 å®¢æ·ç«¯ä½¿ç¨æ¹æ³ååé¢ä¸æ ·ï¼å¯ä¸éè¦éç½®çæ¯æå¡ç«¯çIPåç«¯å£ã
 ```python from image_center import ImageCenter from image_center.conf import
 setting setting.SERCER_IP = "192.168.2.1" # æå¡ç«¯IP setting.PORT = 8889 #
-åæå¡ç«¯ç«¯å£ä¿æä¸è´ ImageCenter.find_image("~/Desktop/test.png") #
-test.pngæ¯ä½ èªå·±æªçå¾ï¼è·¯å¾ä¹ä¿®æ¹æä½ èªå·±çè·¯å¾ ```
+åæå¡ç«¯ç«¯å£ä¿æä¸è´ # Linux and MacOS ImageCenter.find_image("~/
+Desktop/test.png") #
+test.pngæ¯ä½ èªå·±æªçå¾ï¼è·¯å¾ä¹ä¿®æ¹æä½ èªå·±çè·¯å¾ # Windows
+ImageCenter.find_image("D:\\test.png") ```
```

### Comparing `image_center-2024.4.23/pyproject.toml` & `image_center-2024.5.24/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "image-center"
 authors = [
     { name = "mikigo", email = "1964191531@qq.com" },
 ]
 description = "image-center"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
```

### Comparing `image_center-2024.4.23/PKG-INFO` & `image_center-2024.5.24/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: image-center
-Version: 2024.4.23
+Version: 2024.5.24
 Summary: image-center
 Project-URL: Source, https://github.com/linuxdeepin/image-center
 Project-URL: Documentation, https://linuxdeepin.github.io/image-center
 Author-email: mikigo <1964191531@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Requires-Dist: pillow
 Requires-Dist: pyscreenshot
 Provides-Extra: doc
 Requires-Dist: mkdocs-material; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
@@ -41,20 +41,24 @@
 
 ```shell
 sudo apt install python3-opencv
 ```
 
 ## 使用说明
 
-截取目标元素图片，将图片保存到某个路径；
+截取目标元素图片，将图片保存到某个路径,
+
+图片格式：默认使用PNG格式，支持JPG和JPEG格式；
 
 ```python
 from image_center import ImageCenter
-
+# Linux and MacOS
 ImageCenter.find_image("~/Desktop/test.png")
+# Windows
+ImageCenter.find_image("D:\\test.png")
 ```
 
 返回 `test.png` 在当前屏幕中的位置。
 
 ## RPC服务
 
 如果不想在本机安装OpenCV，或者你的机器无法安装OpenCV，可以在服务端安装OpenCV（安装方法和上面一样）；
@@ -77,9 +81,13 @@
 ```python
 from image_center import ImageCenter
 from image_center.conf import setting
 
 setting.SERCER_IP = "192.168.2.1"  # 服务端IP
 setting.PORT = 8889 # 和服务端端口保持一致
 
+# Linux and MacOS
 ImageCenter.find_image("~/Desktop/test.png") # test.png是你自己截的图，路径也修改成你自己的路径
+
+# Windows
+ImageCenter.find_image("D:\\test.png")
 ```
```

#### html2text {}

```diff
@@ -1,29 +1,33 @@
-Metadata-Version: 2.1 Name: image-center Version: 2024.4.23 Summary: image-
+Metadata-Version: 2.1 Name: image-center Version: 2024.5.24 Summary: image-
 center Project-URL: Source, https://github.com/linuxdeepin/image-center
 Project-URL: Documentation, https://linuxdeepin.github.io/image-center Author-
 email: mikigo <1964191531@qq.com> License-File: LICENSE Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Requires-Python:
->=3.7 Requires-Dist: pillow Requires-Dist: pyscreenshot Provides-Extra: doc
+>=3.6 Requires-Dist: pillow Requires-Dist: pyscreenshot Provides-Extra: doc
 Requires-Dist: mkdocs-material; extra == 'doc' Provides-Extra: test Requires-
 Dist: pytest; extra == 'test' Description-Content-Type: text/markdown # image-
 center å¾åè¯å«å®ä½æä¸ªåç´ å¨å½åå±å¹ä¸­çåæ ï¼
 å¨èªå¨åæµè¯ä¸­è·åå°åç´ åæ ä¹åï¼å¯ä»¥ä¼ å¥å°é®é¼ å·¥å·ï¼ä»èå®ç°å¯¹ç®æ åç´ çæä½ã
 --- **Documentation**: _h_t_t_p_s_:_/_/_l_i_n_u_x_d_e_e_p_i_n_._g_i_t_h_u_b_._i_o_/_i_m_a_g_e_-_c_e_n_t_e_r **Source
 Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_l_i_n_u_x_d_e_e_p_i_n_/_i_m_a_g_e_-_c_e_n_t_e_r --- ## å®è£ ```console
 pip install image-center ```
 å¦ææ³å¨æ¬æºç´æ¥ä½¿ç¨å¾åè¯å«ï¼è¿éè¦å¨æ¬æºå®è£OpenCV
 ```shell sudo apt install python3-opencv ``` ## ä½¿ç¨è¯´æ
-æªåç®æ åç´ å¾çï¼å°å¾çä¿å­å°æä¸ªè·¯å¾ï¼ ```python from
-image_center import ImageCenter ImageCenter.find_image("~/Desktop/test.png")
-``` è¿å `test.png` å¨å½åå±å¹ä¸­çä½ç½®ã ## RPCæå¡
+æªåç®æ åç´ å¾çï¼å°å¾çä¿å­å°æä¸ªè·¯å¾,
+å¾çæ ¼å¼ï¼é»è®¤ä½¿ç¨PNGæ ¼å¼ï¼æ¯æJPGåJPEGæ ¼å¼ï¼ ```python from
+image_center import ImageCenter # Linux and MacOS ImageCenter.find_image("~/
+Desktop/test.png") # Windows ImageCenter.find_image("D:\\test.png") ``` è¿å
+`test.png` å¨å½åå±å¹ä¸­çä½ç½®ã ## RPCæå¡
 å¦æä¸æ³å¨æ¬æºå®è£OpenCVï¼æèä½ çæºå¨æ æ³å®è£OpenCVï¼å¯ä»¥å¨æå¡ç«¯å®è£OpenCVï¼å®è£æ¹æ³åä¸é¢ä¸æ ·ï¼ï¼
 æå¡ç«¯å¯å¨æ¹æ³ï¼ ```python from image_center.server import server from
 image_center.conf import setting setting.PORT = 8889 #
 é»è®¤ç«¯å£æ¯8889ï¼å¯ä»¥ä¿®æ¹ä¸ºå¶ä»ç«¯å£ï¼ server() ```
 æ§è¡è¿ä¸ªä»£ç å°±å¯ä»¥å¯å¨æå¡äºï¼
 å®¢æ·ç«¯ä½¿ç¨æ¹æ³ååé¢ä¸æ ·ï¼å¯ä¸éè¦éç½®çæ¯æå¡ç«¯çIPåç«¯å£ã
 ```python from image_center import ImageCenter from image_center.conf import
 setting setting.SERCER_IP = "192.168.2.1" # æå¡ç«¯IP setting.PORT = 8889 #
-åæå¡ç«¯ç«¯å£ä¿æä¸è´ ImageCenter.find_image("~/Desktop/test.png") #
-test.pngæ¯ä½ èªå·±æªçå¾ï¼è·¯å¾ä¹ä¿®æ¹æä½ èªå·±çè·¯å¾ ```
+åæå¡ç«¯ç«¯å£ä¿æä¸è´ # Linux and MacOS ImageCenter.find_image("~/
+Desktop/test.png") #
+test.pngæ¯ä½ èªå·±æªçå¾ï¼è·¯å¾ä¹ä¿®æ¹æä½ èªå·±çè·¯å¾ # Windows
+ImageCenter.find_image("D:\\test.png") ```
```

