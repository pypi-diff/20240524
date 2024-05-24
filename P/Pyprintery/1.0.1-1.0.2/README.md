# Comparing `tmp/Pyprintery-1.0.1.tar.gz` & `tmp/Pyprintery-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Pyprintery-1.0.1.tar", last modified: Mon Apr 15 03:03:47 2024, max compression
+gzip compressed data, was "dist\Pyprintery-1.0.2.tar", last modified: Fri May 24 03:04:56 2024, max compression
```

## Comparing `Pyprintery-1.0.1.tar` & `Pyprintery-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 03:03:47.000000 Pyprintery-1.0.1/
--rw-rw-rw-   0        0        0      542 2024-04-15 03:03:47.000000 Pyprintery-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 03:03:47.000000 Pyprintery-1.0.1/Pyprinter/
--rw-rw-rw-   0        0        0     2993 2024-04-15 03:02:40.000000 Pyprintery-1.0.1/Pyprinter/Myprinter.py
--rw-rw-rw-   0        0        0        0 2024-04-14 08:14:04.000000 Pyprintery-1.0.1/Pyprinter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:03:47.000000 Pyprintery-1.0.1/Pyprintery.egg-info/
--rw-rw-rw-   0        0        0      542 2024-04-15 03:03:46.000000 Pyprintery-1.0.1/Pyprintery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-04-15 03:03:46.000000 Pyprintery-1.0.1/Pyprintery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 03:03:46.000000 Pyprintery-1.0.1/Pyprintery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-15 03:03:46.000000 Pyprintery-1.0.1/Pyprintery.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      170 2024-04-14 09:07:00.000000 Pyprintery-1.0.1/README.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 03:03:47.000000 Pyprintery-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      557 2024-04-15 03:02:38.000000 Pyprintery-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 03:04:56.000000 Pyprintery-1.0.2/
+-rw-rw-rw-   0        0        0      542 2024-05-24 03:04:56.000000 Pyprintery-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-24 03:04:56.000000 Pyprintery-1.0.2/Pyprinter/
+-rw-rw-rw-   0        0        0     4142 2024-05-24 03:01:55.000000 Pyprintery-1.0.2/Pyprinter/Myprinter.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 07:16:10.000000 Pyprintery-1.0.2/Pyprinter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 03:04:56.000000 Pyprintery-1.0.2/Pyprintery.egg-info/
+-rw-rw-rw-   0        0        0      542 2024-05-24 03:04:56.000000 Pyprintery-1.0.2/Pyprintery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-05-24 03:04:56.000000 Pyprintery-1.0.2/Pyprintery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 03:04:56.000000 Pyprintery-1.0.2/Pyprintery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-24 03:04:56.000000 Pyprintery-1.0.2/Pyprintery.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      170 2024-04-14 09:07:00.000000 Pyprintery-1.0.2/README.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 03:04:56.000000 Pyprintery-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      557 2024-05-24 03:01:47.000000 Pyprintery-1.0.2/setup.py
```

### Comparing `Pyprintery-1.0.1/Pyprinter/Myprinter.py` & `Pyprintery-1.0.2/Pyprinter/Myprinter.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,16 +23,20 @@
         
     if isinstance(Beginning, list) == False:
         raise ValueError("Pyprinter <Beginning> Must Be <List>") 
     if len(Beginning) != 2:
         raise ValueError("Pyprinter <Beginning> length Must Be <2>")
     if Going: MyWindoW_Update()
 
-    Beginning[0] = float(str(Beginning[0])[0:3])
-    Beginning[1] = float(str(Beginning[1])[0:3])
+    if Beginning[0] < 0: 
+        Beginning[0] = float(str(Beginning[0])[0:4])
+    else: Beginning[0] = float(str(Beginning[0])[0:3])
+    if Beginning[1] < 0: 
+        Beginning[1] = float(str(Beginning[1])[0:4])
+    else: Beginning[1] = float(str(Beginning[1])[0:3])
 
     if WhereMy > 15:
         raise ValueError("Pyprinter <WhereMy> Cant Get this Component")
     
     for My in range(len(WindoW[WhereMy])):
         turtle.pencolor(WindoW[WhereMy][My][1])
         Goprinting = 0
@@ -64,8 +68,26 @@
 
     turtle.onkey(My, MyWindoWKey[Mykey][Key])
     turtle.listen()
 
 def MyWindoW_InputIng(WindoW="你好  请问你要编辑哪些内容", MyWindoW="测试窗口"):
     if isinstance(WindoW, str) == False: raise ValueError("Pyprinter <WindoW> Must Be <str>")
     if isinstance(MyWindoW, str) == False: raise ValueError("Pyprinter <MyWindoW> Must Be <str>")
-    return turtle.textinput(MyWindoW, WindoW)
+    return turtle.textinput(MyWindoW, WindoW)
+
+def MyWindoW_EventDomy(Where, WhereKeyb, WhereKeyd, MyKey):
+    if isinstance(Where, list) == False or isinstance(WhereKeyb, list) == False or isinstance(WhereKeyd, list) == False: 
+        raise ValueError("Pyprinter <Where WhereKeyb WhereKeyd> Must Be <list>")      
+    if len(Where) != 2 or len(WhereKeyb) != 2 or len(WhereKeyd) != 2: 
+        raise ValueError("Pyprinter <Where WhereKeyb WhereKeyd> length Must Be <2>")
+
+    if Where[0] < 0: Where[0] = float(str(Where[0])[0:4])
+    else: Where[0] = float(str(Where[0])[0:3])
+        
+    if Where[1] < 0: Where[1] = float(str(Where[1])[0:4])
+    else: Where[1] = float(str(Where[1])[0:3])
+    
+    def InputIng(WindoWx, WindoWy):
+        if WindoWx > -(Where[0]*100)+(WhereKeyb[0]*11) and WindoWx < -(Where[0]*100)+(WhereKeyd[0]*11):
+            if WindoWy < (Where[1]*100)-(WhereKeyb[1]*21)+21 and WindoWy > (Where[1]*100)-(WhereKeyd[1]*21)+21:
+                MyKey()
+    turtle.onscreenclick(InputIng, btn=1, add=True)
```

### Comparing `Pyprintery-1.0.1/setup.py` & `Pyprintery-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name="Pyprintery",
-    version="1.0.1",
+    version="1.0.2",
     packages=find_packages(),
     description=("Simulates a game window built by the terminal console, Simple word games can be developed, "+
                 "Third-party libraries that are more entertaining than useful, Suitable for Python beginners"),
     package_data={
         "Pyprinter": [r"Pyprinter/Myprinter.py", r"Pyprinter/*"]
     },
     long_description=open("README.txt", encoding="utf-8").read(),
```

