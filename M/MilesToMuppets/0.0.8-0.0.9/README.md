# Comparing `tmp/milestomuppets-0.0.8.tar.gz` & `tmp/milestomuppets-0.0.9.tar.gz`

## Comparing `milestomuppets-0.0.8.tar` & `milestomuppets-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 milestomuppets-0.0.8/src/milesToMuppets/__init__.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 milestomuppets-0.0.8/src/milesToMuppets/data.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 milestomuppets-0.0.8/src/milesToMuppets/functions.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 milestomuppets-0.0.8/src/milesToMuppets/muppet.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 milestomuppets-0.0.8/src/milesToMuppets/txt/links.txt
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 milestomuppets-0.0.8/src/milesToMuppets/txt/notes.txt
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 milestomuppets-0.0.8/tests/legacy.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 milestomuppets-0.0.8/tests/tmp
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 milestomuppets-0.0.8/LICENSE
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 milestomuppets-0.0.8/README.md
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 milestomuppets-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 milestomuppets-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 milestomuppets-0.0.9/src/milesToMuppets/__init__.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 milestomuppets-0.0.9/src/milesToMuppets/data.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 milestomuppets-0.0.9/src/milesToMuppets/functions.py
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 milestomuppets-0.0.9/src/milesToMuppets/muppet.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 milestomuppets-0.0.9/src/milesToMuppets/txt/links.txt
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 milestomuppets-0.0.9/src/milesToMuppets/txt/notes.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 milestomuppets-0.0.9/tests/dimensions.py
+-rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 milestomuppets-0.0.9/tests/legacy.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 milestomuppets-0.0.9/tests/testrun.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 milestomuppets-0.0.9/tests/tmp
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 milestomuppets-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 milestomuppets-0.0.9/README.md
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 milestomuppets-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 milestomuppets-0.0.9/PKG-INFO
```

### Comparing `milestomuppets-0.0.8/src/milesToMuppets/muppet.py` & `milestomuppets-0.0.9/src/milesToMuppets/muppet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # builtins
 import sys
 import time
+import os
 
 # imports
 import requests
 
 # files
 from .data import *
 from .functions import *
 
 class MilesToMuppets:
-    def __init__(self, client_id: str, client_secret: str, output_mode: str= 'null') -> None:
+    def __init__(self, client_id: str, client_secret: str, do_print: bool = False) -> None:
         # set up internal 
         DATA = data
         CONSTANTS = DATA['constants']
         KEY_LIST = DATA['key_list']
         ALBUM_LIST = DATA['songs']
         self.data = DATA
         self.constants = CONSTANTS
@@ -26,21 +27,30 @@
         self.AUTH_HEADER = get_auth_header(self.TOKEN)
 
         # set up vals
         self.mph_speed = CONSTANTS['defMphSpeed']
         self.min_per_mile = CONSTANTS['defMinPerMile']
 
         # print DATA
-        if output_mode == 'print':
+        if do_print == True:
             print('-----------------------------')
             print("SESSION DATA:")
             print("Token:", self.TOKEN)
             print("Auth header:", self.AUTH_HEADER)
             print('-----------------------------')
 
+    def get_help(self) -> None:
+        info_help()
+
+    def get_license(self) -> None:
+        info_license()
+
+    def get_credits(self) -> None:
+        info_credits()
+        
     def get_session_data(self) -> dict:
         return {
             'token': self.TOKEN,
             'auth header': self.AUTH_HEADER
         }
     def set_mile_distance(self, distance: float) -> None:
         '''set the distance you intend to travel, in miles'''
@@ -61,32 +71,34 @@
         self.song_count = self.ALBUM_DATA['total_tracks']
         self.tracks = self.ALBUM_DATA['tracks']['items']
         return {
             "album name": self.album_name,
             "total songs": self.song_count
         }
     
-    def evaluate_album(self, print_cycle: bool = True) -> dict:
+    def evaluate_album(self, print_cycle: bool = True, do_delay: bool = True) -> dict:
         '''evaluates the album'''
         total_ms = 0
         song_amount = 0
         found_max = False
-        leng = "                                                                                      "
+        width = os.get_terminal_size()[0]
+        spacing = " " * width
         if print_cycle:
             print('-----------------------------\n')
         for track in self.tracks:
             name = track['name']
             duration_ms = track['duration_ms']
             if print_cycle:
                 sys.stdout.write("\033[F")
-                sys.stdout.write(f"{leng}\n{leng}")
+                sys.stdout.write(f"{spacing}\n{spacing}")
                 sys.stdout.write("\033[F")
                 sys.stdout.write(f"\rsong name: {name}\nduration: {duration_ms}ms")
                 sys.stdout.flush()
-                time.sleep(0.15)
+                if do_delay:
+                    time.sleep(0.15)
 
             if total_ms >= self.ms_distance:
                 found_max = True
                 break
             else:
                 total_ms += duration_ms
                 song_amount += 1
@@ -99,9 +111,10 @@
         return {
             'finished album': found_max,
             'average speed': self.mph_speed,
             'minute(s) per mile': self.min_per_mile,
             'songs listened': song_amount,
             'mile distance': self.mile_distance,
             'minute distance': self.minute_distance,
-            'ms distance': self.ms_distance
+            'ms distance': self.ms_distance,
+            'leftover minute(s)':  minute_leftover
         }
```

### Comparing `milestomuppets-0.0.8/tests/legacy.py` & `milestomuppets-0.0.9/tests/legacy.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-# builtins
-import sys
-import time
-
-# imports
-import requests
-
-# files
-from data import *
-from functions import *
-
-# set up client details (moved down from above)
-# client_id = input('Please enter your client_id: ')
-# client_secret = input('Please enter your client secret: ')
-
-# set up overrulling dict, constants
-DATA = data
-CONSTANTS = DATA['constants']
-KEY_LIST = DATA['key_list']
-ALBUM_LIST = DATA['songs']
-KEY_ITER = KEY_LIST.keys()
-ALBUM_ITER = ALBUM_LIST.keys()
-
-class MilesToMuppets:
-    def __init__(self, client_id: str, client_secret: str, output_mode: str= 'null') -> None:
-        # get token, auth_header
-        self.TOKEN = get_token(client_id, client_secret)
-        self.AUTH_HEADER = get_auth_header(self.TOKEN)
-
-        # set up vals
-        self.mph_speed = CONSTANTS['defMphSpeed']
-        self.min_per_mile = CONSTANTS['defMinPerMile']
-
-        # set up internal 
-        self.data = DATA
-        self.constants = CONSTANTS
-        self.key_list = KEY_LIST
-        self.album_list = ALBUM_LIST
-
-        # print DATA
-        if output_mode == 'print':
-            print('-----------------------------')
-            print("SESSION DATA:")
-            print("Token:", self.TOKEN)
-            print("Auth header:", self.AUTH_HEADER)
-            print('-----------------------------')
-        # else:
-        #     return {
-        #         "token": self.TOKEN,
-        #         "auth header": self.AUTH_HEADER
-        #     }
-        
-        # print('-----------------------------')
-        # if input(f'Override default speed of {mph_speed}mph? (y/n) ').lower() == 'y':
-        #     mph_speed = float(input('Enter new speed (mph) \n--> '))
-        #     min_per_mile = 60 / mph_speed
-
-    def set_mile_distance(self, speed: float) -> None:
-        '''set the distance you intend to travel, in mph'''
-        self.mile_distance = speed
-        # print('-----------------------------')
-        # mile_distance = float(input('How far is your destination, in miles? \n--> '))
-        self.minute_distance = self.min_per_mile * self.mile_distance
-        self.ms_distance = minuteToMs(self.minute_distance)
-
-    def choose_song(self, song_choice: int) -> dict:
-        '''chooses a song from the "self.key_list" dictionary'''
-        # print('-----------------------------')
-        # print('Please choose from the following albums:')
-        # for key, album in zip(KEY_ITER, ALBUM_ITER):
-        #     print(f"- {key}: {album}")
-        # song_choice = int(input('--> '))
-        album_id = ALBUM_LIST[KEY_LIST[song_choice]]
-        self.ALBUM_DATA = requests.get(f'https://api.spotify.com/v1/albums/{album_id}', headers=self.AUTH_HEADER).json()
-        self.album_name = self.ALBUM_DATA['name']
-        self.song_count = self.ALBUM_DATA['total_tracks']
-        self.tracks = self.ALBUM_DATA['tracks']['items']
-        # print('-----------------------------')
-        # print('Album name:', album_name)
-        # print('Total amount of songs:', song_count)
-        return {
-            "album name": self.album_name,
-            "total songs": self.song_count
-        }
-    
-    def evaluate_album(self) -> dict:
-        '''evaluates the album'''
-        total_ms = 0
-        song_amount = 0
-        found_max = False
-        leng = "                                                                                      "
-        print('-----------------------------\n')
-        for track in self.tracks:
-            name = track['name']
-            duration_ms = track['duration_ms']
-            # total_ms += duration_ms
-            # song_amount += 1
-            sys.stdout.write("\033[F")
-            sys.stdout.write(f"{leng}\n{leng}")
-            sys.stdout.write("\033[F")
-            sys.stdout.write(f"\rsong name: {name}\nduration: {duration_ms}ms")
-            sys.stdout.flush()
-            time.sleep(0.15)
-
-            if total_ms >= self.ms_distance:
-                found_max = True
-                break
-            else:
-                total_ms += duration_ms
-                song_amount += 1
-            
-        ms_leftover = self.ms_distance - total_ms
-        minute_leftover = round(msToMinute(ms_leftover), 2)
-        print(" ")
-        print('-----------------------------')
-        return {
-            'finished album': found_max,
-            'average speed': self.mph_speed,
-            'minute(s) per mile': self.min_per_mile,
-            'songs listened': song_amount,
-            'mile distance': self.mile_distance,
-            'minute distance': self.minute_distance,
-            'ms distance': self.ms_distance
-        }
-        # if found_max:
-        #     print(f"""Here is the results:
-        #     - average speed: {self.mph_speed}mph
-        #     - minute(s) per mile: {self.min_per_mile}
-        #     - songs listened: {song_amount}
-        #     - album name: {self.album_name}
-        #     - mile distance: {self.mile_distance}
-        #     - minute distance: {self.minute_distance}
-        #     - ms distance: {self.ms_distance}""")
-        # else:
-        #     print('Here is the results:')
-        #     print(f"""You would have finished this playlist on the drive to your destination.
-        # There would be: {minute_leftover} minute(s) left on your trip.""")
-        #     print(f"""Other data:
-        #     - average speed: {self.mph_speed}mph
-        #     - minute(s) per mile: {self.min_per_mile}
-        #     - songs listened: {song_amount}
-        #     - album name: {self.album_name}
-        #     - mile distance: {self.mile_distance}
-        #     - minute distance: {self.minute_distance}
+# builtins
+import sys
+import time
+
+# imports
+import requests
+
+# files
+from data import *
+from functions import *
+
+# set up client details (moved down from above)
+# client_id = input('Please enter your client_id: ')
+# client_secret = input('Please enter your client secret: ')
+
+# set up overrulling dict, constants
+DATA = data
+CONSTANTS = DATA['constants']
+KEY_LIST = DATA['key_list']
+ALBUM_LIST = DATA['songs']
+KEY_ITER = KEY_LIST.keys()
+ALBUM_ITER = ALBUM_LIST.keys()
+
+class MilesToMuppets:
+    def __init__(self, client_id: str, client_secret: str, output_mode: str= 'null') -> None:
+        # get token, auth_header
+        self.TOKEN = get_token(client_id, client_secret)
+        self.AUTH_HEADER = get_auth_header(self.TOKEN)
+
+        # set up vals
+        self.mph_speed = CONSTANTS['defMphSpeed']
+        self.min_per_mile = CONSTANTS['defMinPerMile']
+
+        # set up internal 
+        self.data = DATA
+        self.constants = CONSTANTS
+        self.key_list = KEY_LIST
+        self.album_list = ALBUM_LIST
+
+        # print DATA
+        if output_mode == 'print':
+            print('-----------------------------')
+            print("SESSION DATA:")
+            print("Token:", self.TOKEN)
+            print("Auth header:", self.AUTH_HEADER)
+            print('-----------------------------')
+        # else:
+        #     return {
+        #         "token": self.TOKEN,
+        #         "auth header": self.AUTH_HEADER
+        #     }
+        
+        # print('-----------------------------')
+        # if input(f'Override default speed of {mph_speed}mph? (y/n) ').lower() == 'y':
+        #     mph_speed = float(input('Enter new speed (mph) \n--> '))
+        #     min_per_mile = 60 / mph_speed
+
+    def set_mile_distance(self, speed: float) -> None:
+        '''set the distance you intend to travel, in mph'''
+        self.mile_distance = speed
+        # print('-----------------------------')
+        # mile_distance = float(input('How far is your destination, in miles? \n--> '))
+        self.minute_distance = self.min_per_mile * self.mile_distance
+        self.ms_distance = minuteToMs(self.minute_distance)
+
+    def choose_song(self, song_choice: int) -> dict:
+        '''chooses a song from the "self.key_list" dictionary'''
+        # print('-----------------------------')
+        # print('Please choose from the following albums:')
+        # for key, album in zip(KEY_ITER, ALBUM_ITER):
+        #     print(f"- {key}: {album}")
+        # song_choice = int(input('--> '))
+        album_id = ALBUM_LIST[KEY_LIST[song_choice]]
+        self.ALBUM_DATA = requests.get(f'https://api.spotify.com/v1/albums/{album_id}', headers=self.AUTH_HEADER).json()
+        self.album_name = self.ALBUM_DATA['name']
+        self.song_count = self.ALBUM_DATA['total_tracks']
+        self.tracks = self.ALBUM_DATA['tracks']['items']
+        # print('-----------------------------')
+        # print('Album name:', album_name)
+        # print('Total amount of songs:', song_count)
+        return {
+            "album name": self.album_name,
+            "total songs": self.song_count
+        }
+    
+    def evaluate_album(self) -> dict:
+        '''evaluates the album'''
+        total_ms = 0
+        song_amount = 0
+        found_max = False
+        leng = "                                                                                      "
+        print('-----------------------------\n')
+        for track in self.tracks:
+            name = track['name']
+            duration_ms = track['duration_ms']
+            # total_ms += duration_ms
+            # song_amount += 1
+            sys.stdout.write("\033[F")
+            sys.stdout.write(f"{leng}\n{leng}")
+            sys.stdout.write("\033[F")
+            sys.stdout.write(f"\rsong name: {name}\nduration: {duration_ms}ms")
+            sys.stdout.flush()
+            time.sleep(0.15)
+
+            if total_ms >= self.ms_distance:
+                found_max = True
+                break
+            else:
+                total_ms += duration_ms
+                song_amount += 1
+            
+        ms_leftover = self.ms_distance - total_ms
+        minute_leftover = round(msToMinute(ms_leftover), 2)
+        print(" ")
+        print('-----------------------------')
+        return {
+            'finished album': found_max,
+            'average speed': self.mph_speed,
+            'minute(s) per mile': self.min_per_mile,
+            'songs listened': song_amount,
+            'mile distance': self.mile_distance,
+            'minute distance': self.minute_distance,
+            'ms distance': self.ms_distance
+        }
+        # if found_max:
+        #     print(f"""Here is the results:
+        #     - average speed: {self.mph_speed}mph
+        #     - minute(s) per mile: {self.min_per_mile}
+        #     - songs listened: {song_amount}
+        #     - album name: {self.album_name}
+        #     - mile distance: {self.mile_distance}
+        #     - minute distance: {self.minute_distance}
+        #     - ms distance: {self.ms_distance}""")
+        # else:
+        #     print('Here is the results:')
+        #     print(f"""You would have finished this playlist on the drive to your destination.
+        # There would be: {minute_leftover} minute(s) left on your trip.""")
+        #     print(f"""Other data:
+        #     - average speed: {self.mph_speed}mph
+        #     - minute(s) per mile: {self.min_per_mile}
+        #     - songs listened: {song_amount}
+        #     - album name: {self.album_name}
+        #     - mile distance: {self.mile_distance}
+        #     - minute distance: {self.minute_distance}
         #     - ms distance: {self.ms_distance}""")
```

### Comparing `milestomuppets-0.0.8/LICENSE` & `milestomuppets-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.8/README.md` & `milestomuppets-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 - next, import muppet from milesToMuppets <br>
 `from milesToMuppets import muppet` <br>
 
 - in the code, set up your class object, passing in your Spotify client id and client secret (which can be obtained from Spotify for Developers for free) <br>
 `foo = muppet.MilesToMuppets(client_id = client_id, client_secret = client_secret)` <br>
 
-    - When initializing the class, if you want it to print data, initialize the class as so. <br>
-`foo = MilesToMuppets(client_id = client_id, client_secret = client_secret, output_mode = 'print')`
+    - When initializing the class, if you want it to print its session data, initialize the class as so. <br>
+`foo = MilesToMuppets(client_id = client_id, client_secret = client_secret, do_print = True)`
 
 - next, set the distance you are going, in miles. This number can be anything, but 60 is used as an example here. <br>
   `foo.set_mile_distance(60)`
 
 - set the speed at which you are traveling, in mph. This number can be anything, but 30 is used as an example here. <br>
 `foo.set_speed(30)`
 
@@ -28,12 +28,20 @@
 - then, put your selection into the following function. In this case, we are using 1. <br>
 `foo.choose_album(1)`
 
 - finally, run the function to evaluate the album and return a dictionary with the results.<br>
 `foo.evaluate_album()`
     - If you want to disable printing, set "print_cycle" to false. <br>
     `foo.evaluate_album(print_cycle = False)`
+    - If you want to disable the delay between prints, set "do_delay" to false. <br>
+    `foo.evaluate_album(do_delay = False)
 
 
 # Other functions
 
 - `foo.get_session_data()` - will return your session token, and your auth header in a dict.
+
+  `foo.get_help()` - Will print out some information to help you.
+  
+  `foo.get_license()` - Will print out what license this project is using.
+
+  `foo.get_credits()` - Will print out the credits for the development of this project.
```

### Comparing `milestomuppets-0.0.8/pyproject.toml` & `milestomuppets-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "src/milesToMuppets",
     "src/data",
     "src/functions"
 ]
 
 [project]
 name = "MilesToMuppets"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Sketched Doughnut", email="sketcheddoughnut@gmail.com" },
 ]
 description = "A conversion package to convert Miles to how many songs you can listen to from the Muppets Album"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `milestomuppets-0.0.8/PKG-INFO` & `milestomuppets-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: MilesToMuppets
-Version: 0.0.8
+Version: 0.0.9
 Summary: A conversion package to convert Miles to how many songs you can listen to from the Muppets Album
 Project-URL: Homepage, https://github.com/SketchedDoughnut/miles-to-muppets
 Project-URL: Issues, https://github.com/SketchedDoughnut/miles-to-muppets/issues
 Author-email: Sketched Doughnut <sketcheddoughnut@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -24,16 +24,16 @@
 
 - next, import muppet from milesToMuppets <br>
 `from milesToMuppets import muppet` <br>
 
 - in the code, set up your class object, passing in your Spotify client id and client secret (which can be obtained from Spotify for Developers for free) <br>
 `foo = muppet.MilesToMuppets(client_id = client_id, client_secret = client_secret)` <br>
 
-    - When initializing the class, if you want it to print data, initialize the class as so. <br>
-`foo = MilesToMuppets(client_id = client_id, client_secret = client_secret, output_mode = 'print')`
+    - When initializing the class, if you want it to print its session data, initialize the class as so. <br>
+`foo = MilesToMuppets(client_id = client_id, client_secret = client_secret, do_print = True)`
 
 - next, set the distance you are going, in miles. This number can be anything, but 60 is used as an example here. <br>
   `foo.set_mile_distance(60)`
 
 - set the speed at which you are traveling, in mph. This number can be anything, but 30 is used as an example here. <br>
 `foo.set_speed(30)`
 
@@ -43,12 +43,20 @@
 - then, put your selection into the following function. In this case, we are using 1. <br>
 `foo.choose_album(1)`
 
 - finally, run the function to evaluate the album and return a dictionary with the results.<br>
 `foo.evaluate_album()`
     - If you want to disable printing, set "print_cycle" to false. <br>
     `foo.evaluate_album(print_cycle = False)`
+    - If you want to disable the delay between prints, set "do_delay" to false. <br>
+    `foo.evaluate_album(do_delay = False)
 
 
 # Other functions
 
 - `foo.get_session_data()` - will return your session token, and your auth header in a dict.
+
+  `foo.get_help()` - Will print out some information to help you.
+  
+  `foo.get_license()` - Will print out what license this project is using.
+
+  `foo.get_credits()` - Will print out the credits for the development of this project.
```

