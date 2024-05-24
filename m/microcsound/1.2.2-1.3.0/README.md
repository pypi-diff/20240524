# Comparing `tmp/microcsound-1.2.2.tar.gz` & `tmp/microcsound-1.3.0.tar.gz`

## Comparing `microcsound-1.2.2.tar` & `microcsound-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,20 @@
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 microcsound-1.2.2/.microcsound.toml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 microcsound-1.2.2/.python-version
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 microcsound-1.2.2/README.rst
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound/__init__.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound/config.py
--rw-r--r--   0        0        0     8125 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound/handlers.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound/helpers.py
--rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound/main.py
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound/parser.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound/state.py
--rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound/tests.py
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound/share/data/8bit.orc
--rw-r--r--   0        0        0    15080 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound/share/data/ciconia.mc
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound/share/doc/CHANGES
--rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound/share/doc/microcsound_tutorial.txt
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound.egg-info/PKG-INFO
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound.egg-info/entry_points.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 microcsound-1.2.2/microcsound.egg-info/top_level.txt
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 microcsound-1.2.2/LICENSE.txt
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 microcsound-1.2.2/README.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 microcsound-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 microcsound-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 microcsound-1.3.0/.microcsound.toml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 microcsound-1.3.0/.python-version
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 microcsound-1.3.0/README.rst
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 microcsound-1.3.0/pyvenv.cfg
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 microcsound-1.3.0/microcsound/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 microcsound-1.3.0/microcsound/config.py
+-rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 microcsound-1.3.0/microcsound/handlers.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 microcsound-1.3.0/microcsound/helpers.py
+-rw-r--r--   0        0        0     8347 2020-02-02 00:00:00.000000 microcsound-1.3.0/microcsound/main.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 microcsound-1.3.0/microcsound/parser.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 microcsound-1.3.0/microcsound/state.py
+-rw-r--r--   0        0        0     5983 2020-02-02 00:00:00.000000 microcsound-1.3.0/microcsound/tests.py
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 microcsound-1.3.0/microcsound/share/data/8bit.orc
+-rw-r--r--   0        0        0    15080 2020-02-02 00:00:00.000000 microcsound-1.3.0/microcsound/share/data/ciconia.mc
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 microcsound-1.3.0/microcsound/share/doc/CHANGES
+-rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 microcsound-1.3.0/microcsound/share/doc/microcsound_tutorial.txt
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 microcsound-1.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 microcsound-1.3.0/README.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 microcsound-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 microcsound-1.3.0/PKG-INFO
```

### Comparing `microcsound-1.2.2/.microcsound.toml` & `microcsound-1.3.0/.microcsound.toml`

 * *Files identical despite different names*

### Comparing `microcsound-1.2.2/README.rst` & `microcsound-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `microcsound-1.2.2/microcsound/config.py` & `microcsound-1.3.0/microcsound/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,23 @@
 try:
     with open(Path.home() / ".microcsound.toml", "rb") as config_file:
         user_config = tomllib.load(config_file)
 except:
     user_config = {}
     print("Warning: no '.microcsound.toml' config file found in your home directory!")
     print("Falling back on default values.")
-    print("To fix these, add that file from the repo to your home directory as a template, ")
+    print(
+        "To fix these, add that file from the repo to your home directory as a template, "
+    )
     print("and edit the values to your liking. Then re-run microcsound.")
 
 
 ORC_DIR = user_config.get("ORC_DIR", "/usr/local/share/microcsound")
 DEFAULT_ORC_FILE = user_config.get("DEFAULT_ORC_FILE", "8bit.orc")
-NORMAL_CSOUND_COMMAND_STUB = user_config.get("NORMAL_CSOUND_COMMAND_STUB", "csound -d --messagelevel=0 --nodisplays -W")
-RT_CSOUND_COMMAND_STUB = user_config.get("RT_CSOUND_COMMAND_STUB", "csound -b2048 -B2048 -odac")
+NORMAL_CSOUND_COMMAND_STUB = user_config.get(
+    "NORMAL_CSOUND_COMMAND_STUB", "csound -d --messagelevel=0 --nodisplays -W"
+)
+RT_CSOUND_COMMAND_STUB = user_config.get(
+    "RT_CSOUND_COMMAND_STUB", "csound -b2048 -B2048 -odac"
+)
 MIDDLE_C_HZ = user_config.get("MIDDLE_C_HZ", 261.6255653)
 MIDDLE_C_OCTAVE = user_config.get("MIDDLE_C_OCTAVE", 5)
```

### Comparing `microcsound-1.2.2/microcsound/handlers.py` & `microcsound-1.3.0/microcsound/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,27 +173,24 @@
     elif legato_end:
         state_obj.articulation = "non-legato"
 
     articulation = state_obj.articulation
 
     if pitch:
         degree = helpers.solfege2et(pitch, state_obj.div)
-        pitch = helpers.degree2hz(degree, state_obj.div)
+        state_obj.pitch = helpers.degree2hz(degree, state_obj.div)
     if length_factor:
-        length_factor = int(length_factor)
+        state_obj.length_factor = int(length_factor)
     else:
-        length_factor = 1
+        state_obj.length_factor = 1
 
     if tie_dash:
-        tie = 1
+        state_obj.tie = 1
     else:
-        tie = 0
-    state_obj.length_factor = length_factor
-
-    return pitch, length_factor, articulation, tie
+        state_obj.tie = 0
 
 
 def handle_numeric_notation(event):
     """Handle and return data from a numeric notation event."""
     mylist = re.search(
         r"(?P<articul>[.\(]?)"
         r"(?:(?P<oct>[0-9]+)[.])?"
@@ -214,39 +211,35 @@
     if articul and articul == "(":
         state_obj.articulation = "legato"
     elif articul and articul == ".":
         state_obj.articulation = "staccato"
     elif legato_end:
         state_obj.articulation = "non-legato"
 
-    articulation = state_obj.articulation
-
     if myoct:
         state_obj.octave = int(myoct)
     if deg:
         degree_raw = int(deg)
         if state_obj.div > 0:
             degree = (
                 state_obj.octave - config.MIDDLE_C_OCTAVE
             ) * state_obj.div + degree_raw
-            pitch = helpers.degree2hz(degree, state_obj.div)
+            state_obj.pitch = helpers.degree2hz(degree, state_obj.div)
         else:
             # when div=0, pitch is uninterpreted
-            pitch = degree_raw
+            state_obj.pitch = degree_raw
 
     length_factor = 1
     if tie_phrase:
         length_factor += tie_phrase.count("t")
 
     # we've already handled the ties ourselves:
-    tie = 0
+    state_obj.tie = 0
     state_obj.length_factor = length_factor
 
-    return pitch, length_factor, articulation, tie
-
 
 def handle_JI_notation(event):
     """Handle and return data from a JI note event."""
     mylist = re.search(
         r"(?P<articul>[.\(]?)"
         r"(?P<ratio>[0-9]+[:][0-9]+)"
         r"(?P<legato_end>[\)]?)"
@@ -264,22 +257,18 @@
     if articul and articul == "(":
         state_obj.articulation = "legato"
     elif articul and articul == ".":
         state_obj.articulation = "staccato"
     elif legato_end:
         state_obj.articulation = "non-legato"
 
-    articulation = state_obj.articulation
-
     ratio_text_new = ratio_text.split(":")
     ratio = float(ratio_text_new[0]) / float(ratio_text_new[1])
-    pitch = config.MIDDLE_C_HZ * ratio
+    state_obj.pitch = config.MIDDLE_C_HZ * ratio
 
     length_factor = 1
     if tie_phrase:
         length_factor += tie_phrase.count("t")
 
     # we've already handled the tie:
-    tie = 0
+    state_obj.tie = 0
     state_obj.length_factor = length_factor
-
-    return pitch, length_factor, articulation, tie
```

### Comparing `microcsound-1.2.2/microcsound/helpers.py` & `microcsound-1.3.0/microcsound/helpers.py`

 * *Files identical despite different names*

### Comparing `microcsound-1.2.2/microcsound/main.py` & `microcsound-1.3.0/microcsound/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 from readline import *
 from sys import argv, stdin, stdout
 
 from microcsound import config
 from microcsound.parser import PARSER_PATTERN, parser
 from microcsound.state import state_obj
 
-__all__ = ["process_buffer", "live_loop_in", "sanity_tests", "main"]
+__all__ = ["process_buffer", "live_input_func", "live_loop_in", "sanity_tests", "main"]
+
+
+# used for mocking
+live_input_func = input
 
 
 def process_buffer(inbuffer, rt_mode=False):
     """Split the whole string buffer into individual voice lines.
 
     Then, feed each line to the event parser.
     """
@@ -64,30 +68,30 @@
 
 # live_loop_in function here:
 def live_loop_in():
     """Handle interactive input."""
     buff = ""
     while True:
         try:
-            phrase = input("microcsound--> ")
+            phrase = live_input_func("microcsound--> ")
         except EOFError:
             print("bye!")
             exit(0)
         if phrase.strip() == "done":
             return buff
         else:
             buff += phrase + "\n"
     return buff
 
 
 def main():
     """Start the magic, of course!"""
 
     argparser = argparse.ArgumentParser(
-        epilog="This is microcsound v.1.2.2",
+        epilog="This is microcsound v.1.3.0",
     )
     argparser.usage = """microcsound [-h] [--orc orc_file] [-v]
     [-i |
           [[-o output_wav_file | -s, --score-only | -r, --realtime]
            [-t, --stdin | input_mc_filename ]
           ]
     ] """
@@ -214,44 +218,41 @@
     if args.interactive:
         rt_mode = True
         try:
             while True:
                 state_obj.__init__()
                 live_input = live_loop_in()
                 outbuf = process_buffer(live_input, rt_mode=True)
-                temp_sco_file = open("/tmp/microcsound.sco", "w")
-                temp_sco_file.write("%s\n%s" % (outbuf[0], outbuf[1]))
-                temp_sco_file.close()
+                with open("/tmp/microcsound.sco", "w") as temp_sco_file:
+                    temp_sco_file.write("%s\n%s" % (outbuf[0], outbuf[1]))
                 subprocess.call(
                     csound_command,
                     stdout=subprocess.DEVNULL,
                     stderr=subprocess.DEVNULL,
-                    shell=True
+                    shell=True,
                 )
         except KeyboardInterrupt:
             print("bye!")
             exit()
     else:
         if args.filename:
-            the_file = open(args.filename)
-            outbuf = process_buffer(the_file.read(), rt_mode=rt_mode)
-            the_file.close()
+            with open(args.filename) as input_file:
+                outbuf = process_buffer(input_file.read(), rt_mode=rt_mode)
         elif args.text_stdin:
             outbuf = process_buffer(stdin.read(), rt_mode=rt_mode)
 
         # the end result, which is either a Csound score, or audio:
         if args.score_only:
             stdout.write("%s\n%s" % (outbuf[0], outbuf[1]))
         else:
-            temp_sco_file = open("/tmp/microcsound.sco", "w")
-            temp_sco_file.write("%s\n%s" % (outbuf[0], outbuf[1]))
-            temp_sco_file.close()
+            with open("/tmp/microcsound.sco", "w") as temp_sco_file:
+                temp_sco_file.write("%s\n%s" % (outbuf[0], outbuf[1]))
             subprocess.call(
                 csound_command,
                 stdout=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
-                shell=True
+                shell=True,
             )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `microcsound-1.2.2/microcsound/parser.py` & `microcsound-1.3.0/microcsound/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,30 +100,26 @@
 
         ####################
         ## pitch events : ##
         ####################
 
         # ratio notation (JI):
         elif re.match(r"(?:[.\(])?(?:[0-9]+[:][0-9]+)", event):
-            pitch, length_factor, articulation, tie = handlers.handle_JI_notation(event)
+            handlers.handle_JI_notation(event)
 
         # [oct.]degree notation:
         elif re.match(r"(?:[.\(])?(?:[0-9]+[.])?(?:[-]?[0-9]+)", event):
-            pitch, length_factor, articulation, tie = handlers.handle_numeric_notation(
-                event
-            )
+            handlers.handle_numeric_notation(event)
 
         # symbolic diatonic notation:
         else:
-            pitch, length_factor, articulation, tie = handlers.handle_symbolic_notation(
-                event
-            )
+            handlers.handle_symbolic_notation(event)
 
         # possibly we have a JI transposition:
-        pitch = float(pitch) * float(state_obj.key)
+        pitch = float(state_obj.pitch) * float(state_obj.key)
 
         # OK, if we have finally gotten a pitch event, we know what's what
         # now. If we've gotten this far in the loop,
         # we can calculate stuff....
         on_time = state_obj.grid_time + (
             gauss(0, 0.001) * state_obj.gaussian_rhythm * state_obj.tempo * 0.01666
         )
@@ -153,15 +149,15 @@
             continue
         # or if the note was a tie, and is now not tied, that means
         # it's time actually get its endpoints and send it to the
         # output list:
         if pitch in state_obj.tie_dict[state_obj.instr]:
             tie_info = state_obj.tie_dict[state_obj.instr].pop(pitch)
             on_time = info[0]
-            length_factor = tie_info[1] + state_obj.length_factor
+            state_obj.length_factor = tie_info[1] + state_obj.length_factor
             attack = tie_info[2]
             state_obj.pan = tie_info[3]
         # calculate duration:
         if state_obj.pedal_down:
             duration = state_obj.arrival - on_time
         else:
             if state_obj.articulation == "staccato":
@@ -169,17 +165,17 @@
                     gauss(0, 0.001)
                     * state_obj.gaussian_staccato
                     * state_obj.tempo
                     * 0.01666
                 )
             elif state_obj.articulation == "legato":
                 # negative p3 for legato instruments
-                duration = (state_obj.length * length_factor) * -1
+                duration = (state_obj.length * state_obj.length_factor) * -1
             else:
-                duration = state_obj.length * length_factor
+                duration = state_obj.length * state_obj.length_factor
 
         # finally, a place to put the output text:
         state_obj.outstring = (
             state_obj.outstring
             + "i%1.1f %1.3f %1.3f  %s  %s  %s  %s  %s\n"
             % (
                 state_obj.instr,
@@ -192,8 +188,8 @@
                 " ".join(state_obj.xtra).replace('"', ""),
             )
         )
 
         # update grid_time for next event, but only if not in chord status
         # '[]' mode:
         if not state_obj.chord_status:
-            state_obj.grid_time += state_obj.length * length_factor
+            state_obj.grid_time += state_obj.length * state_obj.length_factor
```

### Comparing `microcsound-1.2.2/microcsound/state.py` & `microcsound-1.3.0/microcsound/state.py`

 * *Files identical despite different names*

### Comparing `microcsound-1.2.2/microcsound/tests.py` & `microcsound-1.3.0/microcsound/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,17 +149,16 @@
     for div in range(5, 53):
         assert solfege2et("g,", div) == solfege2et("g", div) - div
 
 
 def test_solfege2et_f_to_g_same_c_to_d():
     """Tests that step relationships work."""
     for div in range(5, 53):
-        assert (
-            (solfege2et("g", div) - solfege2et("f", div))
-            == (solfege2et("d", div) - solfege2et("c", div))
+        assert (solfege2et("g", div) - solfege2et("f", div)) == (
+            solfege2et("d", div) - solfege2et("c", div)
         )
 
 
 def test_solfege2et_31edo_7_4_ratio():
     """Test the 7/4 ratio in 31edo is the right value."""
     assert solfege2et("^a", 31) == 25
```

### Comparing `microcsound-1.2.2/microcsound/share/data/8bit.orc` & `microcsound-1.3.0/microcsound/share/data/8bit.orc`

 * *Files identical despite different names*

### Comparing `microcsound-1.2.2/microcsound/share/data/ciconia.mc` & `microcsound-1.3.0/microcsound/share/data/ciconia.mc`

 * *Files identical despite different names*

### Comparing `microcsound-1.2.2/microcsound/share/doc/CHANGES` & `microcsound-1.3.0/microcsound/share/doc/CHANGES`

 * *Files identical despite different names*

### Comparing `microcsound-1.2.2/microcsound/share/doc/microcsound_tutorial.txt` & `microcsound-1.3.0/microcsound/share/doc/microcsound_tutorial.txt`

 * *Files identical despite different names*

### Comparing `microcsound-1.2.2/LICENSE.txt` & `microcsound-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `microcsound-1.2.2/README.md` & `microcsound-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `microcsound-1.2.2/pyproject.toml` & `microcsound-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "microcsound"
-version = "1.2.2"
+version = "1.3.0"
 dependencies = ["pytest"]
 requires-python = ">=3.8"
 authors = [
   {name = "Aaron Krister Johnson", email = "akjmicro@gmail.com"}
 
 ]
 maintainers = [
```

### Comparing `microcsound-1.2.2/PKG-INFO` & `microcsound-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: microcsound
-Version: 1.2.2
+Version: 1.3.0
 Summary: A tool for writing csound scores that can make handling microtones MUCH easier.
 Project-URL: Homepage, https://untwelve.org/microcsound
 Project-URL: Repository, https://github.com/akjmicro/microcsound
 Author-email: Aaron Krister Johnson <akjmicro@gmail.com>
 Maintainer-email: Aaron Krister Johnson <akjmicro@gmail.com>
 License: Copyright 2017-2022 Aaron Krister Johnson <akjmicro@gmail.com>
```

