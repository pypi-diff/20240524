# Comparing `tmp/pygame_phyics-1.1.1.tar.gz` & `tmp/pygame_phyics-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_phyics-1.1.1.tar", last modified: Mon Feb 26 07:31:16 2024, max compression
+gzip compressed data, was "pygame_phyics-1.1.2.tar", last modified: Fri May 24 05:34:07 2024, max compression
```

## Comparing `pygame_phyics-1.1.1.tar` & `pygame_phyics-1.1.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 07:31:16.833240 pygame_phyics-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-02-26 07:31:16.833240 pygame_phyics-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 07:31:16.829240 pygame_phyics-1.1.1/pygame_phyics/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/effect.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/game.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/instantiate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/location.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/manger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/mouse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 07:31:16.833240 pygame_phyics-1.1.1/pygame_phyics/objects/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/objects/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/objects/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/objects/gameobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/objects/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/objects/joint.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/objects/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/objects/parent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/objects/physics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/objects/tilemap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 07:31:16.833240 pygame_phyics-1.1.1/pygame_phyics/objects/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/objects/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/objects/ui/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/objects/ui/inputfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/objects/ui/text.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/objects/ui/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/timertask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/pygame_phyics/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 07:31:16.833240 pygame_phyics-1.1.1/pygame_phyics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-02-26 07:31:16.000000 pygame_phyics-1.1.1/pygame_phyics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-02-26 07:31:16.000000 pygame_phyics-1.1.1/pygame_phyics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 07:31:16.000000 pygame_phyics-1.1.1/pygame_phyics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-26 07:31:16.000000 pygame_phyics-1.1.1/pygame_phyics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-26 07:31:16.000000 pygame_phyics-1.1.1/pygame_phyics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-26 07:31:16.833240 pygame_phyics-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-26 07:31:08.000000 pygame_phyics-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:34:07.441832 pygame_phyics-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-24 05:34:07.441832 pygame_phyics-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:34:07.437832 pygame_phyics-1.1.2/pygame_phyics/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/game.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/instantiate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/manger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/mouse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:34:07.441832 pygame_phyics-1.1.2/pygame_phyics/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/objects/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/objects/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/objects/gameobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/objects/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/objects/joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/objects/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/objects/parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/objects/physics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/objects/tilemap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:34:07.441832 pygame_phyics-1.1.2/pygame_phyics/objects/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/objects/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/objects/ui/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/objects/ui/inputfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/objects/ui/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/objects/ui/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/timertask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/pygame_phyics/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:34:07.441832 pygame_phyics-1.1.2/pygame_phyics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-24 05:34:07.000000 pygame_phyics-1.1.2/pygame_phyics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-24 05:34:07.000000 pygame_phyics-1.1.2/pygame_phyics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 05:34:07.000000 pygame_phyics-1.1.2/pygame_phyics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 05:34:07.000000 pygame_phyics-1.1.2/pygame_phyics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-24 05:34:07.000000 pygame_phyics-1.1.2/pygame_phyics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-24 05:34:07.441832 pygame_phyics-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-24 05:34:03.000000 pygame_phyics-1.1.2/setup.py
```

### Comparing `pygame_phyics-1.1.1/PKG-INFO` & `pygame_phyics-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame_phyics
-Version: 1.1.1
+Version: 1.1.2
 Home-page: https://github.com/fireing123/pygame_phyics
 Author: fireing123
 Author-email: gimd82368@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 Requires-Dist: box2d
 Requires-Dist: box2d-py
```

### Comparing `pygame_phyics-1.1.1/README.md` & `pygame_phyics-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/animation.py` & `pygame_phyics-1.1.2/pygame_phyics/animation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from pygame_phyics import Manger
 from pygame_phyics.timertask import TimerTask
-import xml.etree.ElementTree as xml
 
 class Animation:
     def __init__(self, tick, image_object, **kwargs):
         self.object = image_object
-        self.period = TimerTask(tick, self.change_image)
+        self.period = TimerTask(tick)
         self.index = 0
         if  kwargs.get('sheet', None) != None:
             self.sheet = Manger.surface_sheet[kwargs['sheet']]
             if kwargs.get('range', None) != None:
                 frist, last = kwargs['range']
                 self.images = self.sheet.images[frist:last]
             else:
                 raise ValueError("범위를 설정해야함 (int, int) 튜플형식으로 재공")
         else:
             raise ValueError("키워드가 적절하지 않습니다. sheet 를 사용하면 sheet 키워드에 사용하는 시트에 이름을 작성하세요, xml 문서를 이용한 이미지의 집합을 사용하시면 \'xml\'를 작성하세요")
         self.len = len(self.images)
         
     def update(self):
-        self.period.run_periodic_task()
+        if self.period.run_periodic_task():
+            self.change_image()
 
     def change_image(self):
         self.object.og_image = self.images[self.index]
         self.index += 1
         if self.index == self.len:
             self.index = 0
```

### Comparing `pygame_phyics-1.1.1/pygame_phyics/effect.py` & `pygame_phyics-1.1.2/pygame_phyics/effect.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/error.py` & `pygame_phyics-1.1.2/pygame_phyics/error.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 
 
 class ImmutableAttributeError(Exception):
-    """불변의 값을 수정할시 raise 한다"""
+    """불변의 값을 수정하려 시도할때 (불변은 변하지 않는)"""
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
     
 class JsonSerializableError(Exception):
-    """값이 json 으로 파싱할수 없는 값일떄 raise 한다"""
+    """값이 json 으로 파싱할수 없는 값일때"""
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
     
 class FunctionError(Exception):
-    """함수가 아닐떄 raise 한다"""
+    """주어진 값이 함수가 아닐떼"""
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
     
 class GameOver(Exception):
+    """한 맵의 루프가 끝났다는 뜻"""
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
```

### Comparing `pygame_phyics-1.1.1/pygame_phyics/event.py` & `pygame_phyics-1.1.2/pygame_phyics/event.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,11 +40,14 @@
         """함수를 리스트에서 제거합니다
 
         Args:
             function (Callable): 제거할 함수 자체
         """
         self.lisners.remove(function)
     
+    def clear(self):
+        self.lisners.clear()
+
     def invoke(self, *arg):
         """lisners의 함수들을 실행합니다."""
         for function in self.lisners:
             function(*arg)
```

### Comparing `pygame_phyics-1.1.1/pygame_phyics/game.py` & `pygame_phyics-1.1.2/pygame_phyics/game.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/input.py` & `pygame_phyics-1.1.2/pygame_phyics/input.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/instantiate.py` & `pygame_phyics-1.1.2/pygame_phyics/instantiate.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/location.py` & `pygame_phyics-1.1.2/pygame_phyics/location.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/manger.py` & `pygame_phyics-1.1.2/pygame_phyics/manger.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/mouse.py` & `pygame_phyics-1.1.2/pygame_phyics/mouse.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/objects/__init__.py` & `pygame_phyics-1.1.2/pygame_phyics/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/objects/camera.py` & `pygame_phyics-1.1.2/pygame_phyics/objects/camera.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/objects/component.py` & `pygame_phyics-1.1.2/pygame_phyics/objects/component.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/objects/gameobject.py` & `pygame_phyics-1.1.2/pygame_phyics/objects/gameobject.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/objects/image.py` & `pygame_phyics-1.1.2/pygame_phyics/objects/image.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/objects/joint.py` & `pygame_phyics-1.1.2/pygame_phyics/objects/joint.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/objects/object.py` & `pygame_phyics-1.1.2/pygame_phyics/objects/object.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/objects/physics.py` & `pygame_phyics-1.1.2/pygame_phyics/objects/physics.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/objects/tilemap.py` & `pygame_phyics-1.1.2/pygame_phyics/objects/tilemap.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/objects/ui/button.py` & `pygame_phyics-1.1.2/pygame_phyics/objects/ui/button.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/objects/ui/inputfield.py` & `pygame_phyics-1.1.2/pygame_phyics/objects/ui/inputfield.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/objects/ui/text.py` & `pygame_phyics-1.1.2/pygame_phyics/objects/ui/text.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/save.py` & `pygame_phyics-1.1.2/pygame_phyics/save.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/scene.py` & `pygame_phyics-1.1.2/pygame_phyics/scene.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/sheet.py` & `pygame_phyics-1.1.2/pygame_phyics/sheet.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/timertask.py` & `pygame_phyics-1.1.2/pygame_phyics/timertask.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/util.py` & `pygame_phyics-1.1.2/pygame_phyics/util.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics/vector.py` & `pygame_phyics-1.1.2/pygame_phyics/vector.py`

 * *Files identical despite different names*

### Comparing `pygame_phyics-1.1.1/pygame_phyics.egg-info/PKG-INFO` & `pygame_phyics-1.1.2/pygame_phyics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame_phyics
-Version: 1.1.1
+Version: 1.1.2
 Home-page: https://github.com/fireing123/pygame_phyics
 Author: fireing123
 Author-email: gimd82368@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 Requires-Dist: box2d
 Requires-Dist: box2d-py
```

### Comparing `pygame_phyics-1.1.1/pygame_phyics.egg-info/SOURCES.txt` & `pygame_phyics-1.1.2/pygame_phyics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

