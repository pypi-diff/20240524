# Comparing `tmp/wlkata_mirobot_Virtual-2.0.0.tar.gz` & `tmp/wlkata_mirobot_Virtual-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlkata_mirobot_Virtual-2.0.0.tar", last modified: Mon May 20 09:11:34 2024, max compression
+gzip compressed data, was "wlkata_mirobot_Virtual-2.0.1.tar", last modified: Fri May 24 10:06:23 2024, max compression
```

## Comparing `wlkata_mirobot_Virtual-2.0.0.tar` & `wlkata_mirobot_Virtual-2.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 09:11:34.216272 wlkata_mirobot_Virtual-2.0.0/
--rw-rw-rw-   0        0        0      110 2024-05-20 09:11:34.215273 wlkata_mirobot_Virtual-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      587 2024-05-13 07:29:56.000000 wlkata_mirobot_Virtual-2.0.0/license.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 09:11:34.216272 wlkata_mirobot_Virtual-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      236 2024-05-20 09:10:41.000000 wlkata_mirobot_Virtual-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 09:11:34.209289 wlkata_mirobot_Virtual-2.0.0/wlkata_mirobot_Virtual/
--rw-rw-rw-   0        0        0       83 2024-05-12 02:38:37.000000 wlkata_mirobot_Virtual-2.0.0/wlkata_mirobot_Virtual/__init__.py
--rw-rw-rw-   0        0        0    20840 2024-05-20 09:10:18.000000 wlkata_mirobot_Virtual-2.0.0/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py
-drwxrwxrwx   0        0        0        0 2024-05-20 09:11:34.214294 wlkata_mirobot_Virtual-2.0.0/wlkata_mirobot_Virtual.egg-info/
--rw-rw-rw-   0        0        0      110 2024-05-20 09:11:34.000000 wlkata_mirobot_Virtual-2.0.0/wlkata_mirobot_Virtual.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-05-20 09:11:34.000000 wlkata_mirobot_Virtual-2.0.0/wlkata_mirobot_Virtual.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 09:11:34.000000 wlkata_mirobot_Virtual-2.0.0/wlkata_mirobot_Virtual.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-20 09:11:34.000000 wlkata_mirobot_Virtual-2.0.0/wlkata_mirobot_Virtual.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 10:06:23.516526 wlkata_mirobot_Virtual-2.0.1/
+-rw-rw-rw-   0        0        0      110 2024-05-24 10:06:23.515528 wlkata_mirobot_Virtual-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2024-05-13 07:29:56.000000 wlkata_mirobot_Virtual-2.0.1/license.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 10:06:23.516526 wlkata_mirobot_Virtual-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      236 2024-05-24 10:05:56.000000 wlkata_mirobot_Virtual-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:06:23.480623 wlkata_mirobot_Virtual-2.0.1/wlkata_mirobot_Virtual/
+-rw-rw-rw-   0        0        0       83 2024-05-12 02:38:37.000000 wlkata_mirobot_Virtual-2.0.1/wlkata_mirobot_Virtual/__init__.py
+-rw-rw-rw-   0        0        0    20907 2024-05-24 10:05:46.000000 wlkata_mirobot_Virtual-2.0.1/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:06:23.514531 wlkata_mirobot_Virtual-2.0.1/wlkata_mirobot_Virtual.egg-info/
+-rw-rw-rw-   0        0        0      110 2024-05-24 10:06:23.000000 wlkata_mirobot_Virtual-2.0.1/wlkata_mirobot_Virtual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-05-24 10:06:23.000000 wlkata_mirobot_Virtual-2.0.1/wlkata_mirobot_Virtual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 10:06:23.000000 wlkata_mirobot_Virtual-2.0.1/wlkata_mirobot_Virtual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-24 10:06:23.000000 wlkata_mirobot_Virtual-2.0.1/wlkata_mirobot_Virtual.egg-info/top_level.txt
```

### Comparing `wlkata_mirobot_Virtual-2.0.0/license.txt` & `wlkata_mirobot_Virtual-2.0.1/license.txt`

 * *Files identical despite different names*

### Comparing `wlkata_mirobot_Virtual-2.0.0/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py` & `wlkata_mirobot_Virtual-2.0.1/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,18 +303,19 @@
     
     def get_Input(self, input_id):
         try:
             msg = self.client_socket.recv(1024).decode("utf-8")
             pattern = r'"IO":\[([^\]]+)\]'
             match = re.search(pattern, msg)
             input = match.group(1)
-            input_value = input[input_id]
-            if input_value == "1":
+            input_list = [int(item) for item in input.split(',')]
+            input_value = input_list[input_id]
+            if input_value == 1:
                 return True
-            elif input_value == "0":
+            elif input_value == 0:
                 return False
         except Exception as e:
             print(e)
 
     ### 机器人操作
     def home(self, has_slider=False,com1 = False, com2 = False):
         '''机械臂Homing'''
```

