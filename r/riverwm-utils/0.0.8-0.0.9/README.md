# Comparing `tmp/riverwm-utils-0.0.8.tar.gz` & `tmp/riverwm-utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riverwm-utils-0.0.8.tar", last modified: Thu May  2 06:12:38 2024, max compression
+gzip compressed data, was "riverwm-utils-0.0.9.tar", last modified: Tue May  7 08:36:39 2024, max compression
```

## Comparing `riverwm-utils-0.0.8.tar` & `riverwm-utils-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hastings  (1000) hastings  (1000)        0 2024-05-02 06:12:38.853416 riverwm-utils-0.0.8/
--rw-r--r--   0 hastings  (1000) hastings  (1000)    35149 2023-07-03 09:14:06.000000 riverwm-utils-0.0.8/LICENSE
--rw-r--r--   0 hastings  (1000) hastings  (1000)     2530 2024-05-02 06:12:38.853416 riverwm-utils-0.0.8/PKG-INFO
--rw-r--r--   0 hastings  (1000) hastings  (1000)     2025 2023-07-03 09:14:06.000000 riverwm-utils-0.0.8/README.md
--rw-r--r--   0 hastings  (1000) hastings  (1000)       91 2023-07-03 09:14:06.000000 riverwm-utils-0.0.8/pyproject.toml
-drwxr-xr-x   0 hastings  (1000) hastings  (1000)        0 2024-05-02 06:12:38.849416 riverwm-utils-0.0.8/riverwm_utils/
--rw-r--r--   0 hastings  (1000) hastings  (1000)        0 2023-07-03 09:14:06.000000 riverwm-utils-0.0.8/riverwm_utils/__init__.py
--rw-r--r--   0 hastings  (1000) hastings  (1000)     3679 2023-07-03 09:14:06.000000 riverwm-utils-0.0.8/riverwm_utils/river-control-unstable-v1.xml
--rw-r--r--   0 hastings  (1000) hastings  (1000)     6147 2023-07-03 09:14:06.000000 riverwm-utils-0.0.8/riverwm_utils/river-status-unstable-v1.xml
--rw-r--r--   0 hastings  (1000) hastings  (1000)     7737 2024-05-02 05:19:51.000000 riverwm-utils-0.0.8/riverwm_utils/riverwm_utils.py
--rw-r--r--   0 hastings  (1000) hastings  (1000)   140883 2023-07-03 09:14:06.000000 riverwm-utils-0.0.8/riverwm_utils/wayland.xml
-drwxr-xr-x   0 hastings  (1000) hastings  (1000)        0 2024-05-02 06:12:38.853416 riverwm-utils-0.0.8/riverwm_utils.egg-info/
--rw-r--r--   0 hastings  (1000) hastings  (1000)     2530 2024-05-02 06:12:38.000000 riverwm-utils-0.0.8/riverwm_utils.egg-info/PKG-INFO
--rw-r--r--   0 hastings  (1000) hastings  (1000)      445 2024-05-02 06:12:38.000000 riverwm-utils-0.0.8/riverwm_utils.egg-info/SOURCES.txt
--rw-r--r--   0 hastings  (1000) hastings  (1000)        1 2024-05-02 06:12:38.000000 riverwm-utils-0.0.8/riverwm_utils.egg-info/dependency_links.txt
--rw-r--r--   0 hastings  (1000) hastings  (1000)       86 2024-05-02 06:12:38.000000 riverwm-utils-0.0.8/riverwm_utils.egg-info/entry_points.txt
--rw-r--r--   0 hastings  (1000) hastings  (1000)       17 2024-05-02 06:12:38.000000 riverwm-utils-0.0.8/riverwm_utils.egg-info/requires.txt
--rw-r--r--   0 hastings  (1000) hastings  (1000)       14 2024-05-02 06:12:38.000000 riverwm-utils-0.0.8/riverwm_utils.egg-info/top_level.txt
--rw-r--r--   0 hastings  (1000) hastings  (1000)      789 2024-05-02 06:12:38.853416 riverwm-utils-0.0.8/setup.cfg
--rw-r--r--   0 hastings  (1000) hastings  (1000)       65 2023-07-03 09:14:06.000000 riverwm-utils-0.0.8/setup.py
+drwxr-xr-x   0 hastings  (1000) hastings  (1000)        0 2024-05-07 08:36:39.510439 riverwm-utils-0.0.9/
+-rw-r--r--   0 hastings  (1000) hastings  (1000)    35149 2023-07-03 09:14:06.000000 riverwm-utils-0.0.9/LICENSE
+-rw-r--r--   0 hastings  (1000) hastings  (1000)     2530 2024-05-07 08:36:39.510439 riverwm-utils-0.0.9/PKG-INFO
+-rw-r--r--   0 hastings  (1000) hastings  (1000)     2025 2023-07-03 09:14:06.000000 riverwm-utils-0.0.9/README.md
+-rw-r--r--   0 hastings  (1000) hastings  (1000)       91 2023-07-03 09:14:06.000000 riverwm-utils-0.0.9/pyproject.toml
+drwxr-xr-x   0 hastings  (1000) hastings  (1000)        0 2024-05-07 08:36:39.506439 riverwm-utils-0.0.9/riverwm_utils/
+-rw-r--r--   0 hastings  (1000) hastings  (1000)        0 2023-07-03 09:14:06.000000 riverwm-utils-0.0.9/riverwm_utils/__init__.py
+-rw-r--r--   0 hastings  (1000) hastings  (1000)     3679 2023-07-03 09:14:06.000000 riverwm-utils-0.0.9/riverwm_utils/river-control-unstable-v1.xml
+-rw-r--r--   0 hastings  (1000) hastings  (1000)     6147 2023-07-03 09:14:06.000000 riverwm-utils-0.0.9/riverwm_utils/river-status-unstable-v1.xml
+-rw-r--r--   0 hastings  (1000) hastings  (1000)    10597 2024-05-07 08:24:11.000000 riverwm-utils-0.0.9/riverwm_utils/riverwm_utils.py
+-rw-r--r--   0 hastings  (1000) hastings  (1000)   140883 2023-07-03 09:14:06.000000 riverwm-utils-0.0.9/riverwm_utils/wayland.xml
+drwxr-xr-x   0 hastings  (1000) hastings  (1000)        0 2024-05-07 08:36:39.510439 riverwm-utils-0.0.9/riverwm_utils.egg-info/
+-rw-r--r--   0 hastings  (1000) hastings  (1000)     2530 2024-05-07 08:36:39.000000 riverwm-utils-0.0.9/riverwm_utils.egg-info/PKG-INFO
+-rw-r--r--   0 hastings  (1000) hastings  (1000)      445 2024-05-07 08:36:39.000000 riverwm-utils-0.0.9/riverwm_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 hastings  (1000) hastings  (1000)        1 2024-05-07 08:36:39.000000 riverwm-utils-0.0.9/riverwm_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 hastings  (1000) hastings  (1000)       86 2024-05-07 08:36:39.000000 riverwm-utils-0.0.9/riverwm_utils.egg-info/entry_points.txt
+-rw-r--r--   0 hastings  (1000) hastings  (1000)       17 2024-05-07 08:36:39.000000 riverwm-utils-0.0.9/riverwm_utils.egg-info/requires.txt
+-rw-r--r--   0 hastings  (1000) hastings  (1000)       14 2024-05-07 08:36:39.000000 riverwm-utils-0.0.9/riverwm_utils.egg-info/top_level.txt
+-rw-r--r--   0 hastings  (1000) hastings  (1000)      789 2024-05-07 08:36:39.510439 riverwm-utils-0.0.9/setup.cfg
+-rw-r--r--   0 hastings  (1000) hastings  (1000)       65 2023-07-03 09:14:06.000000 riverwm-utils-0.0.9/setup.py
```

### Comparing `riverwm-utils-0.0.8/LICENSE` & `riverwm-utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `riverwm-utils-0.0.8/PKG-INFO` & `riverwm-utils-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riverwm-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities for the River Wayland compositor
 Home-page: https://github.com/NickHastings/riverwm-utils
 Author: Nick Hastings
 Author-email: nicholaschastings@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `riverwm-utils-0.0.8/README.md` & `riverwm-utils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `riverwm-utils-0.0.8/riverwm_utils/river-control-unstable-v1.xml` & `riverwm-utils-0.0.9/riverwm_utils/river-control-unstable-v1.xml`

 * *Files identical despite different names*

### Comparing `riverwm-utils-0.0.8/riverwm_utils/river-status-unstable-v1.xml` & `riverwm-utils-0.0.9/riverwm_utils/river-status-unstable-v1.xml`

 * *Files identical despite different names*

### Comparing `riverwm-utils-0.0.8/riverwm_utils/riverwm_utils.py` & `riverwm-utils-0.0.9/riverwm_utils/riverwm_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 '''Utilities for river wayland compositor'''
 import sys
 import os
 import argparse
+import struct
 # pylint: disable=global-statement
 try:
     from pywayland.protocol.wayland import WlOutput
     from pywayland.protocol.wayland import WlSeat
     from pywayland.protocol.river_control_unstable_v1 import ZriverControlV1
     from pywayland.protocol.river_status_unstable_v1 import ZriverStatusManagerV1  # noqa: E501
 except ModuleNotFoundError:
@@ -63,14 +64,15 @@
 
 
 class Output:
     '''Represents a wayland output a.k.a. a display'''
     def __init__(self):
         self.wl_output = None
         self.focused_tags = None
+        self.view_tags = None
         self.tags = None
         self.status = None
 
     def destroy(self):
         '''Cleanup'''
         if self.wl_output is not None:
             self.wl_output.destroy()
@@ -78,19 +80,24 @@
             self.status.destroy()
 
     def configure(self):
         '''Setup'''
         self.status = STATUS_MANAGER.get_river_output_status(self.wl_output)
         self.status.user_data = self
         self.status.dispatcher["focused_tags"] = self.handle_focused_tags
+        self.status.dispatcher["view_tags"] = self.handle_view_tags
 
     def handle_focused_tags(self, _, tags):
         '''Handle Event'''
         self.focused_tags = tags
 
+    def handle_view_tags(self, _, tags):
+        '''Handle Event'''
+        self.view_tags = tags
+
 
 class Seat:
     '''Represtents a wayland seat'''
     def __init__(self):
         self.wl_seat = None
         self.status = None
         self.focused_output = None
@@ -133,14 +140,59 @@
     elif interface == 'wl_seat':
         # We only care about the first seat
         if SEAT is None:
             SEAT = Seat()
             SEAT.wl_seat = registry.bind(wid, WlSeat, version)
 
 
+def prepare_display(display: Display):
+    '''Prepare display global objects'''
+    display.connect()
+
+    registry = display.get_registry()
+    registry.dispatcher["global"] = registry_handle_global
+
+    display.dispatch(block=True)
+    display.roundtrip()
+
+    if STATUS_MANAGER is None:
+        print("Failed to bind river status manager")
+        sys.exit()
+
+    if CONTROL is None:
+        print("Failed to bind river control")
+        sys.exit()
+
+    # Configuring all outputs, even the ones we do not care about,
+    # should be faster than first waiting for river to advertise the
+    # focused output of the SEAT.
+    for output in OUTPUTS:
+        output.configure()
+
+    SEAT.configure()
+
+    display.dispatch(block=True)
+    display.roundtrip()
+
+
+def close_display(display):
+    '''Clean up objects'''
+    SEAT.destroy()
+    for output in OUTPUTS:
+        output.destroy()
+
+    if STATUS_MANAGER is not None:
+        STATUS_MANAGER.destroy()
+
+    if CONTROL is not None:
+        CONTROL.destroy()
+
+    display.disconnect()
+
+
 def check_direction(direction):
     '''Check validity of direction argument'''
     dir_char = direction[0].lower()
     if dir_char not in ('p', 'n'):
         raise argparse.ArgumentTypeError(f'Invalid direction: {direction}')
 
     return dir_char
@@ -169,86 +221,124 @@
     parser.add_argument(
         'n_tags', default=32, nargs='?', type=check_n_tags,
         help=('The tag number the cycling should loop back to the first tag '
               'or to the last tag from the first tag. Should be and integer '
               'between 1 and 32 inclusive.')
     )
     parser.add_argument(
+        '--all-outputs', '-a', dest='all_outputs', action='store_true',
+        help='Cycle the tags for all outputs (following the active output).'
+    )
+    parser.add_argument(
+        '--follow', '-f', dest='follow', action='store_true',
+        help='Move the active window when cycling.'
+    )
+    parser.add_argument(
+        '--skip-empty', '-s', action='store_true',
+        help='Skip empty tags.'
+    )
+    parser.add_argument(
         '--debug', '-d', action='store_true',
         help='Enable debugging output.'
     )
     return parser.parse_args()
 
 
-def cycle_focused_tags():
-    '''Shift to next or previous tags'''
-    args = parse_command_line()
-    display = Display()
-    display.connect()
+def get_occupied_tags(view_tags):
+    '''Return bitmap of occupied tags as int'''
+    occupied_tags = 0
+    nviews = int(len(view_tags) / 4)
+    for view in struct.unpack(f'{nviews}I', view_tags):
+        occupied_tags |= view
 
-    registry = display.get_registry()
-    registry.dispatcher["global"] = registry_handle_global
+    return occupied_tags
 
-    display.dispatch(block=True)
-    display.roundtrip()
 
-    if STATUS_MANAGER is None:
-        print("Failed to bind river status manager")
-        sys.exit()
+def is_occupied(tags, occupied_tags):
+    '''Return true if tags are occupied'''
+    return bool(tags & occupied_tags)
 
-    if CONTROL is None:
-        print("Failed to bind river control")
-        sys.exit()
 
-    # Configuring all outputs, even the ones we do not care about,
-    # should be faster than first waiting for river to advertise the
-    # focused output of the SEAT.
-    for output in OUTPUTS:
-        output.configure()
+def get_new_tags(cli_args, tags, last_tag, occupied_tags):
+    '''Return the new tag set'''
 
-    SEAT.configure()
+    # All tags are empty and we want to skip empty tags
+    # => return the current tags
+    if cli_args.skip_empty and occupied_tags == 0:
+        return tags
+
+    while True:
+        new_tags = 0
+        if cli_args.direction == 'n':
+            # If last tag is set => unset it and set first bit on new_tags
+            if (tags & last_tag) != 0:
+                tags ^= last_tag
+                new_tags = 1
+
+            new_tags |= (tags << 1)
+
+        else:
+            # If lowest bit is set (first tag) => unset it and set
+            # last_tag bit on new tags
+            if (tags & 1) != 0:
+                tags ^= 1
+                new_tags = last_tag
+
+            new_tags |= (tags >> 1)
+
+        if cli_args.debug:
+            print(f'new 0b{new_tags:032b}')
+
+        if not cli_args.skip_empty or is_occupied(new_tags, occupied_tags):
+            return new_tags
+
+        tags = new_tags
+
+
+def cycle_focused_tags():
+    '''Shift to next or previous tags'''
+    args = parse_command_line()
+    display = Display()
+    prepare_display(display)
 
-    display.dispatch(block=True)
-    display.roundtrip()
     used_tags = (1 << args.n_tags) - 1
     tags = SEAT.focused_output.focused_tags & used_tags
+    view_tags = SEAT.focused_output.view_tags
+    occupied_tags = get_occupied_tags(view_tags) & used_tags
+    if args.debug:
+        print(f'occ 0b{occupied_tags:032b}')
 
-    new_tags = 0
     last_tag = 1 << (args.n_tags - 1)
-    if args.direction == 'n':
-        # If last tag is set => unset it and set first bit on new_tags
-        if (tags & last_tag) != 0:
-            tags ^= last_tag
-            new_tags = 1
-
-        new_tags |= (tags << 1)
-
-    else:
-        # If lowest bit is set (first tag) => unset it and set
-        # last_tag bit on new tags
-        if (tags & 1) != 0:
-            tags ^= 1
-            new_tags = last_tag
-
-        new_tags |= (tags >> 1)
+    new_tags = get_new_tags(args, tags, last_tag, occupied_tags)
 
-    if args.debug:
-        print(f'0b{new_tags:010b} {new_tags}')
+    if args.follow:
+        CONTROL.add_argument("set-view-tags")
+        CONTROL.add_argument(str(new_tags))
+        CONTROL.run_command(SEAT.wl_seat)
 
     CONTROL.add_argument("set-focused-tags")
     CONTROL.add_argument(str(new_tags))
     CONTROL.run_command(SEAT.wl_seat)
 
+    if args.all_outputs and len(OUTPUTS) > 1:
+        # The active output has been switched, walk over all other outputs and
+        # set their tags too, wrapping back to the start (where setting can be
+        # skipped).
+        for i in range(len(OUTPUTS)):
+            CONTROL.add_argument("focus-output")
+            CONTROL.add_argument("next")
+            CONTROL.run_command(SEAT.wl_seat)
+
+            if i + 1 == len(OUTPUTS):
+                # Back to the start which has already had it's tags set.
+                # Breaking here isn't needed but the next assignment is
+                # redundant.
+                break
+
+            CONTROL.add_argument("set-focused-tags")
+            CONTROL.add_argument(str(new_tags))
+            CONTROL.run_command(SEAT.wl_seat)
+
     display.dispatch(block=True)
     display.roundtrip()
 
-    SEAT.destroy()
-    for output in OUTPUTS:
-        output.destroy()
-
-    if STATUS_MANAGER is not None:
-        STATUS_MANAGER.destroy()
-
-    if CONTROL is not None:
-        CONTROL.destroy()
-
-    display.disconnect()
+    close_display(display)
```

### Comparing `riverwm-utils-0.0.8/riverwm_utils/wayland.xml` & `riverwm-utils-0.0.9/riverwm_utils/wayland.xml`

 * *Files identical despite different names*

### Comparing `riverwm-utils-0.0.8/riverwm_utils.egg-info/PKG-INFO` & `riverwm-utils-0.0.9/riverwm_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riverwm-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities for the River Wayland compositor
 Home-page: https://github.com/NickHastings/riverwm-utils
 Author: Nick Hastings
 Author-email: nicholaschastings@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `riverwm-utils-0.0.8/setup.cfg` & `riverwm-utils-0.0.9/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = riverwm-utils
-version = 0.0.8
+version = 0.0.9
 author = Nick Hastings
 author_email = nicholaschastings@gmail.com
 description = Utilities for the River Wayland compositor
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GPLv3
 license_file = LICENSE
```

