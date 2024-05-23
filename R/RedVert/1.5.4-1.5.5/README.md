# Comparing `tmp/redvert-1.5.4.tar.gz` & `tmp/redvert-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvert-1.5.4.tar", last modified: Thu May 23 22:04:15 2024, max compression
+gzip compressed data, was "redvert-1.5.5.tar", last modified: Thu May 23 22:19:27 2024, max compression
```

## Comparing `redvert-1.5.4.tar` & `redvert-1.5.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 22:04:15.096714 redvert-1.5.4/
--rw-rw-rw-   0        0        0    10538 2024-05-23 22:04:15.093613 redvert-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0    10439 2024-05-23 21:33:03.000000 redvert-1.5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 22:04:15.090616 redvert-1.5.4/RedVert.egg-info/
--rw-rw-rw-   0        0        0    10538 2024-05-23 22:04:14.000000 redvert-1.5.4/RedVert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-05-23 22:04:14.000000 redvert-1.5.4/RedVert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 22:04:14.000000 redvert-1.5.4/RedVert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-23 22:04:14.000000 redvert-1.5.4/RedVert.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-05-23 22:04:14.000000 redvert-1.5.4/RedVert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 22:04:15.088614 redvert-1.5.4/redvert/
--rw-rw-rw-   0        0        0       19 2024-04-24 21:45:28.000000 redvert-1.5.4/redvert/__init__.py
--rw-rw-rw-   0        0        0     9960 2024-05-23 22:04:09.000000 redvert-1.5.4/redvert/main.py
--rw-rw-rw-   0        0        0       42 2024-05-23 22:04:15.098730 redvert-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-05-23 22:04:03.000000 redvert-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 22:19:27.543435 redvert-1.5.5/
+-rw-rw-rw-   0        0        0    10538 2024-05-23 22:19:27.541023 redvert-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0    10439 2024-05-23 21:33:03.000000 redvert-1.5.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 22:19:27.538490 redvert-1.5.5/RedVert.egg-info/
+-rw-rw-rw-   0        0        0    10538 2024-05-23 22:19:27.000000 redvert-1.5.5/RedVert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-05-23 22:19:27.000000 redvert-1.5.5/RedVert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 22:19:27.000000 redvert-1.5.5/RedVert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-23 22:19:27.000000 redvert-1.5.5/RedVert.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-05-23 22:19:27.000000 redvert-1.5.5/RedVert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 22:19:27.536493 redvert-1.5.5/redvert/
+-rw-rw-rw-   0        0        0       19 2024-04-24 21:45:28.000000 redvert-1.5.5/redvert/__init__.py
+-rw-rw-rw-   0        0        0    10270 2024-05-23 22:15:40.000000 redvert-1.5.5/redvert/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 22:19:27.544760 redvert-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-05-23 22:19:12.000000 redvert-1.5.5/setup.py
```

### Comparing `redvert-1.5.4/PKG-INFO` & `redvert-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RedVert
-Version: 1.5.4
+Version: 1.5.5
 Description-Content-Type: text/markdown
 
 # @COPYRIGHT 2024 By Kyfstore
 
 # Introduction
 
 Hello! This is RedVert, the python package similar to anaconda where you can create environment folders, variables and other python scripts! These scripts may not be posted, stolen or copyrighted as your own.
```

### Comparing `redvert-1.5.4/README.md` & `redvert-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `redvert-1.5.4/RedVert.egg-info/PKG-INFO` & `redvert-1.5.5/RedVert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RedVert
-Version: 1.5.4
+Version: 1.5.5
 Description-Content-Type: text/markdown
 
 # @COPYRIGHT 2024 By Kyfstore
 
 # Introduction
 
 Hello! This is RedVert, the python package similar to anaconda where you can create environment folders, variables and other python scripts! These scripts may not be posted, stolen or copyrighted as your own.
```

### Comparing `redvert-1.5.4/redvert/main.py` & `redvert-1.5.5/redvert/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,18 +147,22 @@
         user_input = input('>>> ')
         if user_input == "Stop RedVert":
             print("Successfully Stopped RedVert\n")
             isRunning = False
             break
         elif user_input == 'Create Env':
             print("Name Environment")
-            env_name[f'env{i}'] = input('>>> ')
-            save_to_file(str(env_name), env_file)
-            print("Successfully Created Environment\n")
-            i += 1
+            env_input = input('>>> ')
+            if env_input.strip():  # Check if the input is not empty or whitespace only
+                env_name[f'env{i}'] = env_input.strip()  # Store the input without leading/trailing whitespaces
+                save_to_file(str(env_name), env_file)
+                print("Successfully Created Environment\n")
+                i += 1
+            else:
+                print("You cannot create an environment with no name\n")
         elif user_input == 'Remove All Env':
             print("Are you sure [y or n]")
             remove_input = input('>>> ')
             if remove_input == 'y':
                 print("Clearing All Data")
                 print("1% Completed")
                 delay(0.7)
@@ -257,8 +261,9 @@
                         print("Unknown Command Please Try Again\n")
                         continue
                 else:
                     print("Unknown Environment\n")
             except:
                 print("Unable To Open Environments File\n")
         else:
-            print("Unknown RedVert Command Try Again.\n")
+            print("Unknown RedVert Command Try Again.\n")
+Initalize()
```

