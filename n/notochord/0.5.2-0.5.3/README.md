# Comparing `tmp/notochord-0.5.2.tar.gz` & `tmp/notochord-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notochord-0.5.2.tar", max compression
+gzip compressed data, was "notochord-0.5.3.tar", max compression
```

## Comparing `notochord-0.5.2.tar` & `notochord-0.5.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1084 2023-11-28 17:22:02.563723 notochord-0.5.2/LICENSE
--rw-r--r--   0        0        0     4726 2024-05-17 00:10:44.090539 notochord-0.5.2/README.md
--rw-r--r--   0        0        0      833 2024-05-17 00:16:02.481173 notochord-0.5.2/pyproject.toml
--rw-r--r--   0        0        0       87 2023-11-28 17:22:02.566423 notochord-0.5.2/src/notochord/__init__.py
--rw-r--r--   0        0        0      898 2024-05-15 20:23:17.997905 notochord-0.5.2/src/notochord/__main__.py
--rw-r--r--   0        0        0      163 2023-11-28 17:22:02.566552 notochord-0.5.2/src/notochord/app/__init__.py
--rw-r--r--   0        0        0      316 2023-11-28 17:22:02.566610 notochord-0.5.2/src/notochord/app/harmonizer.css
--rw-r--r--   0        0        0    10522 2023-11-28 17:22:02.566797 notochord-0.5.2/src/notochord/app/harmonizer.py
--rw-r--r--   0        0        0     1479 2024-05-15 20:23:17.998076 notochord-0.5.2/src/notochord/app/homunculus.css
--rw-r--r--   0        0        0    45875 2024-05-17 00:10:44.091633 notochord-0.5.2/src/notochord/app/homunculus.py
--rw-r--r--   0        0        0    18983 2023-11-28 17:22:02.567055 notochord-0.5.2/src/notochord/app/improviser-txala.py
--rw-r--r--   0        0        0      385 2023-11-28 17:22:02.567122 notochord-0.5.2/src/notochord/app/improviser.css
--rw-r--r--   0        0        0    19710 2024-04-24 13:59:31.571434 notochord-0.5.2/src/notochord/app/improviser.py
--rw-r--r--   0        0        0     1558 2024-05-16 11:58:41.020109 notochord-0.5.2/src/notochord/app/preset-zeno.json
--rw-r--r--   0        0        0     4842 2024-05-16 23:35:41.902339 notochord-0.5.2/src/notochord/app/preset.json
--rw-r--r--   0        0        0     4413 2024-05-15 20:23:17.998802 notochord-0.5.2/src/notochord/app/server.py
--rw-r--r--   0        0        0     3073 2023-11-28 17:22:02.567375 notochord-0.5.2/src/notochord/app/simple_harmonizer.py
--rw-r--r--   0        0        0    10631 2024-04-24 13:59:31.572536 notochord-0.5.2/src/notochord/data.py
--rw-r--r--   0        0        0    12790 2023-11-28 17:22:02.567536 notochord-0.5.2/src/notochord/distributions.py
--rw-r--r--   0        0        0    47550 2024-05-17 00:10:44.092251 notochord-0.5.2/src/notochord/model.py
--rw-r--r--   0        0        0    12706 2024-04-24 13:59:31.573908 notochord-0.5.2/src/notochord/perform.py
--rw-r--r--   0        0        0     2528 2023-11-28 17:22:02.567874 notochord-0.5.2/src/notochord/rnn.py
--rw-r--r--   0        0        0    13940 2024-04-24 13:59:31.574327 notochord-0.5.2/src/notochord/train.py
--rw-r--r--   0        0        0     2488 2023-11-28 17:22:02.568040 notochord-0.5.2/src/notochord/util.py
--rw-r--r--   0        0        0     5519 1970-01-01 00:00:00.000000 notochord-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-11-28 17:22:02.563723 notochord-0.5.3/LICENSE
+-rw-r--r--   0        0        0     5193 2024-05-24 01:09:33.499776 notochord-0.5.3/README.md
+-rw-r--r--   0        0        0      854 2024-05-24 01:10:39.153789 notochord-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-11-28 17:22:02.566423 notochord-0.5.3/src/notochord/__init__.py
+-rw-r--r--   0        0        0     1197 2024-05-24 01:09:33.500220 notochord-0.5.3/src/notochord/__main__.py
+-rw-r--r--   0        0        0      163 2023-11-28 17:22:02.566552 notochord-0.5.3/src/notochord/app/__init__.py
+-rw-r--r--   0        0        0      316 2023-11-28 17:22:02.566610 notochord-0.5.3/src/notochord/app/harmonizer.css
+-rw-r--r--   0        0        0    10522 2023-11-28 17:22:02.566797 notochord-0.5.3/src/notochord/app/harmonizer.py
+-rw-r--r--   0        0        0     1870 2024-05-24 01:09:33.500441 notochord-0.5.3/src/notochord/app/homunculus.css
+-rw-r--r--   0        0        0    52480 2024-05-24 01:09:33.500982 notochord-0.5.3/src/notochord/app/homunculus.py
+-rw-r--r--   0        0        0     3325 2024-05-24 01:09:33.501229 notochord-0.5.3/src/notochord/app/homunculus.toml
+-rw-r--r--   0        0        0    18983 2023-11-28 17:22:02.567055 notochord-0.5.3/src/notochord/app/improviser-txala.py
+-rw-r--r--   0        0        0      385 2023-11-28 17:22:02.567122 notochord-0.5.3/src/notochord/app/improviser.css
+-rw-r--r--   0        0        0    19710 2024-04-24 13:59:31.571434 notochord-0.5.3/src/notochord/app/improviser.py
+-rw-r--r--   0        0        0      606 2024-05-24 01:02:59.965896 notochord-0.5.3/src/notochord/app/preset-zeno.toml
+-rw-r--r--   0        0        0     4413 2024-05-15 20:23:17.998802 notochord-0.5.3/src/notochord/app/server.py
+-rw-r--r--   0        0        0     3073 2023-11-28 17:22:02.567375 notochord-0.5.3/src/notochord/app/simple_harmonizer.py
+-rw-r--r--   0        0        0    10631 2024-04-24 13:59:31.572536 notochord-0.5.3/src/notochord/data.py
+-rw-r--r--   0        0        0    12790 2023-11-28 17:22:02.567536 notochord-0.5.3/src/notochord/distributions.py
+-rw-r--r--   0        0        0    47819 2024-05-24 01:09:33.501721 notochord-0.5.3/src/notochord/model.py
+-rw-r--r--   0        0        0    12706 2024-04-24 13:59:31.573908 notochord-0.5.3/src/notochord/perform.py
+-rw-r--r--   0        0        0     2528 2023-11-28 17:22:02.567874 notochord-0.5.3/src/notochord/rnn.py
+-rw-r--r--   0        0        0    13940 2024-04-24 13:59:31.574327 notochord-0.5.3/src/notochord/train.py
+-rw-r--r--   0        0        0     2488 2023-11-28 17:22:02.568040 notochord-0.5.3/src/notochord/util.py
+-rw-r--r--   0        0        0     6028 1970-01-01 00:00:00.000000 notochord-0.5.3/PKG-INFO
```

### Comparing `notochord-0.5.2/LICENSE` & `notochord-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `notochord-0.5.2/README.md` & `notochord-0.5.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,32 +22,37 @@
 
 run fluidsynth in a terminal. For example, `fluidsynth -v -o midi.portname="fluidsynth" -o synth.midi-bank-select=mma ~/'Downloads/soundfonts/Timbres of Heaven (XGM) 4.00(G).sf2'`
 
 ## Notochord MIDI Apps
 
 Notochord includes several [iipyper](https://github.com/Intelligent-Instruments-Lab/iipyper.git) apps which can be run in a terminal. They have a clickable text-mode user interface and connect directly to MIDI ports, so you can wire them up to your controllers, DAW, etc.
 
-The Notochord harmonizer adds extra concurrent notes for each MIDI note you play in. In a terminal, make sure your notochord Python environment is active and run:
-```
-notochord harmonizer
-```
-try `notochord harmonizer --help`
-to see more options.
-
-the "homunculus" gives you a UI to manage multiple input, harmonizing or autonomous notochord channels:
+The `homunculus` provides a text-based graphical interface to manage multiple input, harmonizing or autonomous notochord channels:
 ```
 notochord homunculus
 ```
 You can set the MIDI in and out ports with `--midi-in` and `--midi-out`. If you use a General MIDI synthesizer like fluidsynth, you can add `--send-pc` to also send program change messages.
 
-If you are using fluidsynth, try:
+If you are using fluidsynth as above, try:
 ```
 notochord homunculus --send-pc --midi-out fluidsynth --thru
 ```
 
+Note: on windows, there are no virtual MIDI ports and no system MIDI loopback, so you may need to attach some MIDI devices or run a loopback driver like [loopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html) before starting the app.
+
+There are also two simpler notochord apps: `improviser` and `harmonizer`. The harmonizer adds extra concurrent notes for each MIDI note you play in. In a terminal, make sure your notochord Python environment is active and run:
+```
+notochord harmonizer
+```
+try `notochord harmonizer --help`
+to see more options.
+
+Development is now focused on `homunculus`, which is intended to subsume all features of `improviser` and `harmonizer`.
+
+
 ## Python API
 
 See the docs for `Notochord.feed` and `Notochord.query` for the low-level Notochord inference API which can be used from Python code. `notochord/app/simple_harmonizer.py` provides a minimal example of how to build an interactive app.
 
 ## OSC server
 
 You can also expose the inference API over Open Sound Control:
```

### Comparing `notochord-0.5.2/pyproject.toml` & `notochord-0.5.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "notochord"
-version = "0.5.2"
+version = "0.5.3"
 description = "Notochord is a real-time neural network model for MIDI performances."
 authors = ["Victor Shepardson <victor.shepardson@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 torch = ">=1.13,<2.3"
 numpy = "^1.23"
 pandas = "^2.0"
 tqdm = "^4.64"
 sf2utils = "^0.9"
 appdirs = "^1.4.4"
-iipyper = "~0.1.3"
+iipyper = "^0.1.4"
+toml-file = "^1.0.5"
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "^1.5.3"
 mkdocstrings = {extras = ["python"], version = "^0.23.0"}
 mkdocs-gen-files = "^0.5.0"
 mkdocs-include-markdown-plugin = "^6.0.4"
 mkdocs-material = "^9.4.8"
```

### Comparing `notochord-0.5.2/src/notochord/app/harmonizer.py` & `notochord-0.5.3/src/notochord/app/harmonizer.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.2/src/notochord/app/homunculus.css` & `notochord-0.5.3/src/notochord/app/homunculus.css`

 * *Files 24% similar despite different names*

```diff
@@ -60,23 +60,48 @@
     border-bottom: none;
 }
 .cmute {
     width:7;
     height:3;
 }
 
-InstrumentSelect Grid {
-    grid-size: 8 16;
+ModalScreen {
+    align: center middle;
+}
+
+ModalScreen Grid {
+    grid-size: 4 7;
+    grid-gutter: 1 1;
+    # grid-rows: 1fr 3;
+    padding: 0 1;
+    width: 35;
+    height: 22;
+    border: thick $background 80%;
+    background: $surface;
 }
-InstrumentSelect Button {
+InstrumentGroup {
     border: none;
     min-width: 5;
     height: 2;
-
 }
+InstrumentSelect Grid {
+    grid-size: 4 5;
+}
+Instrument {
+    border: none;
+    min-width: 5;
+    min-height: 3;
+}
+
+# InstrumentSelect Button {
+#     border: none;
+#     min-width: 5;
+#     height: 2;
+
+# }
 
 /* MixerButtons Button {
     height: 5;
     border: solid purple;
 } */
 
 NotoPrediction {
```

### Comparing `notochord-0.5.2/src/notochord/app/homunculus.py` & `notochord-0.5.3/src/notochord/app/homunculus.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,34 @@
 """
 Notochord MIDI co-improviser server.
 Notochord plays different instruments along with the player.
-
-Authors:
-  Victor Shepardson
-  Intelligent Instruments Lab 2023
 """
 
+# Authors:
+#   Victor Shepardson
+#   Intelligent Instruments Lab 2023
+
+tui_doc = """Welcome to notochord homunculus.
+You have 16 channels of MIDI, laid out in two rows of eight.
+Each can be in one of three modes:
+    input (-->02)
+    follow (01->02)
+    auto (02)
+Input channels take MIDI input from the corresponding channel,
+and send it to notochord. When using --thru, input is also copied
+to the output.
+    Follow channels act like a harmonizer; they query notochord for
+a NoteOn whenever the followed channel has a NoteOn, and have the
+corresponding NoteOff when the followed channel does.
+    Auto channels are played autonomously by notochord.
+Each channel can be muted independently of the others.
+    Below the channel strips, there is a row of presets.
+These can be edited in homunculus.toml; run `notochord files` to find 
+it in your file explorer."""
+
 # TODO: move soundfont / general MIDI stuff out of script
 
 # TODO: make key bindings visibly click corresponding buttons
 # TODO: make Mute a toggle but Reset a momentary
 
 # TODO: color note by pitch class + register
 # TODO: color instrument 1-128, MEL, DRUM, ANON, ANONDRUM
@@ -21,38 +39,38 @@
 
 # TODO: controls display panel
 # TODO: held notes display panel
 # TODO: counts / weights display panel
 # TODO: MIDI learn
 
 import time
-
+import shutil
 from typing import Optional, Dict, Any
 from numbers import Number
 import math
 import functools as ft
-import json
 from pathlib import Path
 from collections import defaultdict
 from datetime import datetime
 
 import numpy as np
+import toml_file
 
 import torch
 torch.set_num_threads(1)
 
 import iipyper, notochord
 from notochord import Notochord, NotoPerformance
 from iipyper import OSC, MIDI, run, Stopwatch, repeat, cleanup, TUI, profile, lock
 
 from rich.panel import Panel
 from rich.pretty import Pretty
 from textual.reactive import reactive
 from textual.widgets import Header, Footer, Static, Button, Log, RichLog, Label
-from textual.screen import Screen
+from textual.screen import Screen, ModalScreen
 from textual.containers import Grid
 
 def main(
     checkpoint="notochord-latest.ckpt", # Notochord checkpoint
     config:Dict[int,Dict[str,Any]]=None, # map MIDI channel : GM instrument
     preset:str=None,
     preset_file:Path=None,
@@ -85,42 +103,57 @@
     estimated_latency=1e-2,
     soundfont=None,
     limit_input=None,
     thru_vel_offset=None,
     profiler=0,
     ):
     """
-    This a terminal app for using Notochord interactively with MIDI controllers and synthesizers. Arguments to main can be given on the command line as flags, for example:
+    This a terminal app for using Notochord interactively with MIDI controllers and synthesizers. It allows combining both 'harmonizer' and 'improviser' features.
+     
+    Arguments to main can be given on the command line as flags, for example:
+
+    `notochord homunculus --config "{1:{mode:auto, inst:1, mute:False}}" --initial-query --max-time 1`
+
+    This says: play the grand piano autonomously on channel 1, start automatically, allow no more than 1 second between MIDI events. A different example:
+
+    `notochord homunculus --config "{1:{mode:input, inst:1, mute:False}, 2:{mode:follow, inst:12, mute:False}}" --thru --send-pc`
 
-    `python -m notochord homunculus --initial-query --config '{1:{mode:auto, inst:1}}'`
+    This says, take grand piano input on channel 1, and harmonize it with vibraphone on channel 2. Pass input through to the output, and also send program change messages to set the instruments on the synthesizer.
+
+    You may also need to use the --midi-in or --midi-out flags to get MIDI to the right place.
     
-    16 voices correspond to the 16 MIDI channels. Each voice can be in one of three modes:
+    # MIDI Channels
+
+    In homunculus, you have 16 MIDI channels. Each channel can be in one of three modes:
+
+        * input (appearing like "-->01"), channel 1 comes from MIDI input channel 1.
+        * follow (appearing like "01->02"), channel 2 plays whenever channel 1 plays.
+        * auto (appearing like just "03"), channel 3 plays autonomously.
 
-        * input (appearing like "-->01"), voice 1 comes from MIDI input channel 1.
-        * follow (appearing like "01->02"), voice 2 plays whenever voice 1 plays.
-        * auto (appearing like just "03"), voice 3 plays autonomously.
+    Click the top section of each channel strip to cycle the mode.
 
-    Click the top section of each voice to cycle the mode.
+    Each channel is also assigned a [General MIDI instrument](https://en.wikipedia.org/wiki/General_MIDI#Program_change_events). Each 'input' and 'auto' channel should have a unique General MIDI instrument, but 'follow' channels can be duplicates of others. If you try to assign duplicate instruments, they will automatically change to "anonymous" melodic or drum instruments, but still send the right program change messages when using --send-pc.
 
-    Each voice is also assigned a [General MIDI instrument](https://en.wikipedia.org/wiki/General_MIDI#Program_change_events). Each 'input' and 'auto' voice should have a unique General MIDI instrument, but 'follow' voices can be duplicates of other voices. 
+    Click the middle section of each channel strip to choose a new instrument.
 
-    Click the middle section of each voice to choose a new instrument.
+    The bottom section of each channel strip allows muting individual voices.
 
-    The bottom section of each voice allows muting individual voices.
+    # Global controls
 
     Along the bottom, there are global query, sustain, mute and reset buttons. Query manually replaces the next pending note. Sustain stops all auto voices from playing without ending any open notes. Mute ends all open notes and stops auto voices. Reset ends all open notes, forgets all context and sets the Notochord model to its initial state.
 
     Args:
         checkpoint: path to notochord model checkpoint.
 
-        config: mapping from MIDI channels to voice specs.
+        config: 
+            mapping from MIDI channels to voice specs.
             MIDI channels and General MIDI instruments are indexed from 1.
-            see https://en.wikipedia.org/wiki/General_MIDI for instrument numbers.
-            There are 3 modes of voice: 'auto', 'follow' and 'input'.
-            Example:
+            see wikipedia.org/wiki/General_MIDI for values.
+            There are 3 modes of voice, 'auto', 'follow' and 'input'. For example,
+            ```
             {
                 1:{
                     'mode':'input', 'inst':1
                 }, # input grand piano on MIDI channel 1
                 2:{
                     'mode':'follow', 'source':1, 'inst':1, 
                     'transpose':(-12,12)
@@ -131,60 +164,82 @@
                 10:{
                     'mode':'auto', 'inst':129,
                 }, # autonomous drums voice
                 4:{
                     'mode':'follow', 'source':3, 'inst':10, 'range':(72,96)
                 }, # harmonize channel 3 within upper registers of the glockenspiel
             }
+            ```
             Notes:
-            no 'input' or 'auto' channels should use the same instrument,
-            but 'follow' channels may have the same as an 'input' or 'auto'
-        preset: preset name (in preset file) to load config from
-        preset_file: path to JSON file containing dict of name:config (as above)
-
-        initial_mute: start 'auto' voices muted so it won't play with input.
-        initial_query: query Notochord immediately,
+            when two channels use the same instrument, one will be converted
+            to an 'anonymous' instrument number (but it will still respect the 
+            chosen instrument when using --send-pc)
+
+        preset: 
+            preset name (in preset file) to load config from
+        preset_file: 
+            path to a TOML file containing channel presets
+            the default config file is `homunculus.toml`; 
+            running `notochord files` will show its location.
+
+        initial_mute: 
+            start 'auto' voices muted so it won't play with input.
+        initial_query: 
+            query Notochord immediately,
             so 'auto' voices begin playing  without input.
 
-        midi_in: MIDI ports for input. 
+        midi_in: 
+            MIDI ports for input. 
             default is to use all input ports.
             can be comma-separated list of ports.
-        midi_out: MIDI ports for output. 
+        midi_out: 
+            MIDI ports for output. 
             default is to use only virtual 'From iipyper' port.
             can be comma-separated list of ports.
-        thru: if True, copy input MIDI to output ports.
+        thru: 
+            if True, copy input MIDI to output ports.
             only makes sense if input and output ports are different.
-        send_pc: if True, send MIDI program change messages to set the General MIDI
+        send_pc: 
+            if True, send MIDI program change messages to set the General MIDI
             instrument on each channel according to player_config and noto_config.
             useful when using a General MIDI synthesizer like fluidsynth.
-        dump_midi: if True, print all incoming MIDI for debugging purposes
+        dump_midi: 
+            if True, print all incoming MIDI for debugging purposes
 
-        balance_sample choose 'auto' voices which have played less recently,
+        balance_sample:
+            choose 'auto' voices which have played less recently,
             ensures that all configured instruments will play.
-        n_recent: number of recent note-on events to consider for above
-        n_margin: amount of 'slack' in the balance_sample calculation
-
-        max_note_len: time in seconds after which to force-release sustained
-            'auto' notes.
-        max_time: maximum seconds between predicted events for 'auto' voices.
+        n_recent: 
+            number of recent note-on events to consider for above
+        n_margin: 
+            controls the amount of slack in the balance_sample calculation
+
+        max_note_len: 
+            time in seconds after which to force-release sustained 'auto' notes.
+        max_time: 
+            maximum seconds between predicted events for 'auto' voices.
             default is the Notochord model's maximum (usually 10 seconds).
-        nominal_time: if True, feed Notochord with its own predicted times
+        nominal_time: 
+            if True, feed Notochord with its own predicted times
             instead of the actual elapsed time.
             May make Notochord more likely to play chords.
 
-        osc_port: optional. if supplied, listen for OSC to set controls
-        osc_host: hostname or IP of OSC sender.
+        osc_port: 
+            optional. if supplied, listen for OSC to set controls
+        osc_host: 
+            hostname or IP of OSC sender.
             leave this as empty string to get all traffic on the port
 
-        use_tui: run textual UI.
-        predict_input: forecasted next events can be for 'input' voices.
+        use_tui: 
+            run textual UI.
+        predict_input: 
+            forecasted next events can be for 'input' voices.
             generally should be True for manual input;
             use balance_sample to force 'auto' voices to play. 
             you might want it False if you have a very busy input.
-        debug_query=False, # don't query notochord when there is no pending event.
     """
     if osc_port is not None:
         osc = OSC(osc_host, osc_port)
     midi = MIDI(midi_in, midi_out)
 
     if soundfont is not None:
         # attempt to get instrument ranges from the soundfont
@@ -222,41 +277,67 @@
             return 0,127  
 
     ### Textual UI
     tui = NotoTUI()
     print = notochord.print = iipyper.print = tui.print
     ###
 
+    # make preset file if it doesn't exist
+    cfg_dir = Notochord.user_data_dir()
+    default_preset_file = cfg_dir / 'homunculus.toml'
+    src_preset_file = Path(__file__).parent / 'homunculus.toml'
+    if not default_preset_file.exists():
+        shutil.copy(src_preset_file, default_preset_file)
+
     ### presets and config
     try:
         if preset_file is None:
-            with open(Path(__file__).parent / 'preset.json') as f:
-                presets = json.load(f)
+            presets = toml_file.Config(str(default_preset_file))['preset']
         else:
-            with open(preset_file) as f:
-                presets = json.load(f)
+            presets = toml_file.Config(str(preset_file))['preset']
     except Exception:
         print('WARNING: failed to load presets file')
         presets = {}
 
+    # defaults
+    def default_config_channel(i):
+        return {'mode':'auto', 'inst':1, 'mute':True, 'mono':False, 'source':max(1,i-1), 'note_shift':0}
+    
     # convert MIDI channels to int
-    presets = {p:{int(k):v for k,v in d.items()} for p,d in presets.items()}
+    # print(presets)
+    for p in presets:
+        p['channel'] = {int(k):{**default_config_channel(i), **v} for i,(k,v) in enumerate(p['channel'].items(),1)}
+    # presets = {p:{int(k):v for k,v in d.items()} for p,d in presets.items()}
+
+    # TODO: config from CLI > config from preset file > channel defaults
+    #       warn if preset is overridden by config
+    # TODO: what is sensible default behavior?
+    #    for quickstart, it's good if it does something as soon as possible
+    #    but for general use, it's good if it does nothing until you ask... 
 
-    if preset is None and len(presets):
-        preset = list(presets)[0]
+    config_file = {}
     if isinstance(preset, str):
-        config = presets[preset]
+        for p in presets:
+            if preset == p['name']:
+                config_file = p['channel']
+                if config is not None:
+                    print('WARNING: `--config` overrides `--preset`')
+                break
+    elif len(presets):
+        config_file = presets[0]['channel']
+        # preset = list(presets)[0]
 
-    # defaults
-    config_in = config
-    def default_config_channel():
-        return {'mode':'auto', 'inst':1, 'mute':False, 'mono':False, 'source':1}
-    config = {i:default_config_channel() for i in range(1,17)}
-    for k,v in config_in.items():
+    config_cli = {} if config is None else config
+
+    config = {i:default_config_channel(i) for i in range(1,17)}
+    for k,v in config_file.items():
         config[k].update(v)
+    for k,v in config_cli.items():
+        config[k].update(v)
+    
 
     def validate_config():
         assert all(
             v['source'] in config for v in config.values() if v['mode']=='follow'
             ), 'ERROR: no source given for follow voice'
         # TODO: check for follow cycles
     validate_config()
@@ -302,55 +383,63 @@
     def channel_followers(chan):
         # return channel of all 'follow' voices with given source
         return [
             k for k,v in config.items() 
             if v['mode']=='follow' 
             and v.get('source', None)==chan]
     
-    if len(mode_insts('input') & mode_insts('auto')):
-        print("WARNING: auto and input instruments shouldn't overlap")
-        print('setting to an anonymous instrument')
-        # TODO: set to anon insts without changing mel/drum
-        # respecting anon insts selected for player
-        raise NotImplementedError
-    # TODO:
-    # check for repeated insts/channels
+    # if len(mode_insts('input') & mode_insts('auto')):
+    #     print("WARNING: auto and input instruments shouldn't overlap")
+    #     print('setting to an anonymous instrument')
+    #     # TODO: set to anon insts without changing mel/drum
+    #     # respecting anon insts selected for player
+    #     raise NotImplementedError
     
     # load notochord model
     try:
         noto = Notochord.from_checkpoint(checkpoint)
         noto.eval()
         noto.feed(0,0,0,0)
         noto.query()
         noto.reset()
     except Exception:
         print("""error loading notochord model""")
         raise
 
-    def warn_inst(i):
-        if i > 128:
-            if i < 257:
-                print(f"WARNING: drum instrument {i} selected, be sure to select a drum bank in your synthesizer")
-            else:
-                print(f"WARNING: instrument {i} is not General MIDI")
+    # def warn_inst(i):
+    #     if i > 128:
+    #         if i < 257:
+    #             print(f"WARNING: drum instrument {i} selected, be sure to select a drum bank in your synthesizer")
+    #         else:
+    #             print(f"WARNING: instrument {i} is not General MIDI")
 
     def dedup_inst(c, i):
         # change to anon if already in use
         def in_use():
             return any(
-                c_other!=c and config[c_other]['inst']==i 
+                c_other!=c 
+                and config[c_other]['inst']==i 
+                and config[c_other]['mode']!='follow'
                 for c_other in config)
         if in_use():
             i = noto.first_anon_like(i)
         while in_use():
             i = i+1
         return i
 
     def do_send_pc(c, i):
-        warn_inst(i)
+        # warn_inst(i)
+        # assuming fluidsynth -o synth.midi-bank-select=mma
+        if noto.is_drum(i):
+            midi.control_change(channel=c-1, control=0, value=1)
+        else:
+            midi.control_change(channel=c-1, control=32, value=0)
+            midi.control_change(channel=c-1, control=0, value=0)
+        if noto.is_anon(i):
+            i = 0
         # convert to 0-index
         midi.program_change(channel=c-1, program=(i-1)%128)
 
     for c,i in channel_insts():
         if send_pc:
             do_send_pc(c, i)
         config[c]['inst'] = dedup_inst(c, i)
@@ -380,14 +469,29 @@
         now = str(datetime.now())[:-2]
         s = f'{now}   inst {inst:3d}   pitch {pitch:3d}   vel {vel:3d}   ch {channel:2d} {tag}'
         # s = f'{tag}:\t{inst=:4d}   {pitch=:4d}   {vel=:4d}   {channel=:3d}'
         if memo is not None:
             s += f' ({memo})'
         tui.defer(note=s)
 
+    def send_midi(note, velocity, channel):
+        kind = 'note_on' if velocity > 0 else 'note_off'
+        cfg = config[channel]
+        # get channel note map
+        if 'note_map' in cfg:
+            note_map = cfg['note_map']
+        else:
+            note_map = {}
+        if note in note_map:
+            note = note_map[note]
+        elif 'note_shift' in cfg:
+            note = note + cfg['note_shift']
+
+        midi.send(kind, note=note, velocity=velocity, channel=channel-1)
+
     def play_event(
             event, channel, 
             parent=None, # parent note as (channel, inst, pitch)
             feed=True, 
             send=True, 
             tag=None, memo=None):
         """realize an event as MIDI, terminal display, and Notochord update"""
@@ -396,17 +500,18 @@
         dt = stopwatch.punch()
         if 'time' not in event or not nominal_time:
             event['time'] = dt
 
         # send out as MIDI
         if send:
             with profile('\tmidi.send', print=print, enable=profiler>1):
-                midi.send(
-                    'note_on' if vel > 0 else 'note_off', 
-                    note=event['pitch'], velocity=vel, channel=channel-1)
+                send_midi(event['pitch'], vel, channel)
+                # midi.send(
+                #     'note_on' if vel > 0 else 'note_off', 
+                #     note=event['pitch'], velocity=vel, channel=channel-1)
 
         # print
         with profile('\tdisplay_event', print=print, enable=profiler>1):
             display_event(
                 tag, memo=memo, channel=channel, **event)
 
         if feed:
@@ -842,37 +947,42 @@
     def _():
         """end any remaining notes"""
         # print(f'cleanup: {notes=}')
         # for (chan,inst,pitch) in history.note_triples:
         for note in history.notes:
         # for (inst,pitch) in notes:
             if note.inst in mode_insts(('auto', 'follow')):
-                midi.note_on(note=note.pitch, velocity=0, channel=note.chan-1)
+                midi.note_off(note=note.pitch, velocity=0, channel=note.chan-1)
+                # midi.note_on(note=note.pitch, velocity=0, channel=note.chan-1)
 
     ### update_* keeps the UI in sync with the state
 
     def update_config():
         # print(config)
         for c,v in config.items():
             tui.set_channel(c, v)
 
     def update_presets():
-        for p,k in enumerate(presets):
-            tui.set_preset(p, k)
+        for k,p in enumerate(presets):
+            tui.set_preset(k, p.get('name'))
 
     @tui.on
     def mount():
         update_config()
         update_presets()
-        print('welcome to notochord homunculus')
         print('MIDI handling:')
         print(midi.get_docs())
         if osc_port is not None:
             print('OSC handling:')
             print(osc.get_docs())
+        print(tui_doc)
+        print('For more detailed documentation, see:')
+        print('https://intelligent-instruments-lab.github.io/notochord/reference/notochord/app/homunculus/')
+        print('or run `notochord homunculus --help`')
+        print('to exit, use CTRL+C')
 
     ### set_* does whatever necessary to change channel properties
     ### calls update_config() to keep the UI in sync
 
     def set_mode(c, m, update=True):
         if c in config:
             prev_m = config[c]['mode']
@@ -905,34 +1015,64 @@
                         dict(inst=note.inst, pitch=note.pitch, vel=0),
                         channel=note.chan, 
                         tag='NOTO', memo='mode change')
 
         if update:
             update_config()
 
-    class InstrumentSelect(Screen):
-        """Screen with an instrument select dialog."""
+    class Instrument(Button):
+        """button which picks an instrument"""
+        def __init__(self, c, i):
+            super().__init__(inst_label(i))
+            self.channel = c
+            self.inst = i
+        def on_button_pressed(self, event: Button.Pressed):
+            self.app.pop_screen()
+            self.app.pop_screen()
+            set_inst(self.channel, self.inst)
+
+    class InstrumentGroup(Button):
+        """button which picks an instrument group"""
+        def __init__(self, text, c, g):
+            super().__init__(text)
+            self.channel = c
+            self.group = g
+        def on_button_pressed(self, event: Button.Pressed):
+            # show inst buttons
+            tui.push_screen(InstrumentSelect(self.channel, self.group))
+
+    class InstrumentSelect(ModalScreen):
+        """Screen with instruments"""
+        def __init__(self, c, g):
+            super().__init__()
+            self.channel = c
+            self.group = g
+
+        def compose(self):
+            yield Grid(
+                *(
+                    Instrument(self.channel, i)
+                    for i in gm_groups[self.group][1]
+                ), id="dialog",
+            )
+
+    class InstrumentGroupSelect(ModalScreen):
+        """Screen with instrument groups"""
+        # TODO: add other features to this screen -- transpose, range, etc?
         def __init__(self, c):
             super().__init__()
             self.channel = c
 
         def compose(self):
             yield Grid(
                 *(
-                    Button(s, id='select_'+inst_id(i)) 
-                    for i,s in enumerate(gm_names, 1)
+                    InstrumentGroup(s, self.channel, g)
+                    for g,(s,_) in enumerate(gm_groups)
                 ), id="dialog",
             )
-        def on_button_pressed(self, event: Button.Pressed) -> None:
-            # print(event.button.id)
-            # i = 1
-            i = int(event.button.id.split('_')[-1])
-            self.app.pop_screen()
-            set_inst(self.channel, i)
-        # TODO: on key pressed esc, q: cancel
 
     def set_inst(c, i, update=True):
         print(f'SET INSTRUMENT {i}')
         if c in config:
             prev_i = config[c]['inst']
         else:
             prev_i = None
@@ -991,47 +1131,42 @@
             # TODO: source picker for follow
             set_mode(c, 'follow')
         else:
             set_mode(c, 'auto')
 
     def action_inst(c):
         print(f'inst channel {c}')
-        # TODO: instrument picker
-        tui.push_screen(InstrumentSelect(c))
-        # inst_select.channel = c
-        # tui.push_screen(inst_select)
-        # i = 1
-        # set_inst(c, i)
+        tui.push_screen(InstrumentGroupSelect(c))
 
     def action_mute(c):
         if i not in config: return
         set_mute(c, not config[c].get('mute', False))
 
     def action_preset(p):
-        ks = list(presets.keys())
-        if p >= len(ks):
+        if p >= len(presets): 
             return
-        k = ks[p]
-        preset = presets[k]
-        print(f'load preset: {k}')
+        preset = presets[p]['channel']
+        print(f'load preset: {p}')
         for c in range(1,17):    
             if c not in config:
-                config[c] = default_config_channel()
+                config[c] = default_config_channel(c)
             if c not in preset:
                 set_mute(c, True, update=False)
             else:
-                v = preset[c]
-                set_mode(c, v.get('mode', 'auto'), update=False)
-                set_inst(c, v.get('inst', 1), update=False)
-                set_mute(c, v.get('mute', False), update=False)
-                # ugly, this sets config repeatedly...
+                # note config should *not* be updated before calling set_* 
+                v = {**preset[c]}
+                # v = {**config[c]}
+                # v.update(preset[c])
+                set_mode(c, v.pop('mode'), update=False)
+                set_inst(c, v.pop('inst'), update=False)
+                set_mute(c, v.pop('mute'), update=False)
                 config[c].update(v)
         update_config()
 
-    ### set actions which have an with index argument
+    ### set actions which have an index argument
     ### TODO move this logic into @tui.set_action
 
     for i in range(1,17):
         setattr(tui, f'action_mode_{i}', ft.partial(action_mode, i))
         setattr(tui, f'action_inst_{i}', ft.partial(action_inst, i))
         setattr(tui, f'action_mute_{i}', ft.partial(action_mute, i))
 
@@ -1074,19 +1209,14 @@
         evt = self.value
         if evt is None:
             s = ''
         else:
             s = f"\tinstrument: {evt['inst']:3d}    pitch: {evt['pitch']:3d}    time: {int(evt['time']*1000):4d} ms    velocity:{int(evt['vel']):3d}"
         self.update(Panel(s, title='prediction'))
 
-# class NotoToggle(Static):
-#     def compose(self):
-#         yield Button("Mute", id="mute", variant="error")
-#         yield Switch()
-
 class Mixer(Static):
     def compose(self):
         for i in range(1,17):
             yield MixerButtons(i, id=f"mixer_{i}")
 
 def preset_id(i):
     return f"preset_{i}"
@@ -1161,32 +1291,36 @@
     CSS_PATH = 'homunculus.css'
 
     BINDINGS = [
         ("m", "mute", "Mute Notochord"),
         ("s", "sustain", "Sustain"),
         ("q", "query", "Re-query Notochord"),
         ("r", "reset", "Reset Notochord")]
+    
+
 
     def compose(self):
         """Create child widgets for the app."""
         yield Header()
         yield self.std_log
         yield NotoLog(id='note')
         yield NotoPrediction(id='prediction')
         yield Mixer()
         yield NotoPresets()
         yield NotoControl()
         yield Footer()
 
     def on_mount(self) -> None:
         self.query_one(NotoPrediction).tooltip = "displays the next predicted event"
+        print(self.screen)
 
     def set_preset(self, idx, name):
         node = self.query_one('#'+preset_id(idx))
-        node.label = name
+        node.label = str(idx) if name is None else name
+        # node.label = name
 
     def set_channel(self, chan, cfg):
         # print(f'set_channel {cfg}')
         inst_node = self.query_one('#'+inst_id(chan))
         mode_node = self.query_one('#'+mode_id(chan))
         mute_node = self.query_one('#'+mute_id(chan))
 
@@ -1217,14 +1351,15 @@
         else:
             mode_node.variant = 'primary'
             inst_node.variant = 'warning'
             mute_node.label = 'MUTE'
             mute_node.variant = 'default'
 
 gm_names = [
+    '_SEQ_\nSTART',
     'GRAND\nPIANO', 'BRGHT\nPIANO', 'EGRND\nPIANO', 'HONKY\n-TONK', 
     'RHODE\nPIANO', 'FM   \nPIANO', 'HRPSI\nCHORD', 'CLAV \n INET',
     'CEL  \n ESTA', 'GLOCN\nSPIEL', 'MUSIC\n BOX ', 'VIBRA\nPHONE', 
     'MAR  \n IMBA', 'XYLO \nPHONE', 'TUBLR\n BELL', 'DULCI\n  MER',
     'DRAWB\nORGAN', 'PERC \nORGAN', 'ROCK \nORGAN', 'CHRCH\nORGAN', 
     'REED \nORGAN', 'ACCOR\n DION', 'HARMO\n NICA', 'BANDO\n NEON',  
     'A-GTR\nNYLON', 'A-GTR\nSTEEL', 'E-GTR\nJAZZ ', 'E-GTR\nCLEAN', 
@@ -1249,18 +1384,56 @@
     'FX  5\nBRGHT', 'FX  6\nGOBLN', 'FX  7\nECHOS', 'FX  8\nSCIFI',
     'SITAR\n     ', 'BANJO\n     ', 'SHAM \n ISEN', 'KOTO \n     ',
     'KAL  \n IMBA', 'BAG  \n PIPE', 'FID  \n  DLE', 'SHA  \n  NAI',  
     'TINKL\nBELL ', 'AGO  \n   GÔ', 'STEEL\nDRUM ', 'WOOD \nBLOCK', 
     'TAIKO\nDRUM ', 'MELO \n  TOM', 'SYNTH\nDRUM ', ' REV \nCYMBL',  
     'GTR  \n FRET', 'BRE  \n  ATH', ' SEA \nSHORE', 'BIRD \nTWEET',
     'TELE \nPHONE', 'HELI \nCOPTR', 'APP  \nLAUSE', 'GUN  \n SHOT',  
-    ' STD \nDRUMS'
-] + ['DRUM \n  KIT']*127 + ['ANON \n MEL ']*32 + ['ANON \nDRUMS']*32
+] + (
+    ['STD  \n  KIT']*8 + 
+    ['ROOM \n  KIT']*8 + 
+    ['ROCK \n  KIT']*8 + 
+    ['ELCTR\n  KIT']*8 + 
+    ['JAZZ \n  KIT']*8 + 
+    ['BRUSH\n  KIT']*8 + 
+    ['ORCHS\n  KIT']*8 + 
+    ['SFX  \n  KIT']*8 + 
+    ['DRUM \n KIT?']*64 
+) + ['ANON \n MEL ']*32 + ['ANON \nDRUMS']*32
+gm_groups = [
+    ('PIANO\n     ', range(1,9)),
+    ('CHROM\nPERC ', range(9,17)),
+    ('ORGAN\n     ', range(17,25)),
+    ('GUI  \n TARS', range(25,33)),
+    ('BASS \n GTRS', range(33,41)),
+    ('STRIN\n   GS', range(41,49)),
+    ('ENSEM\n BLES', range(49,57)),
+    ('BRASS\n     ', range(57,65)),
+    ('REEDS\n     ', range(65,73)),
+    ('PIPES\n     ', range(73,81)),
+    ('SYNTH\nLEADS', range(81,89)),
+    ('SYNTH\nPADS ', range(89,97)),
+    ('SYNTH\nFX   ', range(97,105)),
+    ('MISC \n  MEL', range(105,113)),
+    ('MISC \n PERC', range(113,121)),
+    ('SOUND\nFX   ', range(121,129)),
+    ('DRUM \n KITS', [128+i for i in (1,9,17,25,33,41,49,57)]),
+    # (' STD \nDRUMS', range(129,137)),
+    # ('ROOM \nDRUMS', range(137,145)),
+    # ('ROCK \nDRUMS', range(145,153)),
+    # ('ELCTR\nDRUMS', range(153,161)),
+    # ('JAZZ \nDRUMS', range(161,169)),
+    # ('BRUSH\nDRUMS', range(169,177)),
+    # ('ORCH \nDRUMS', range(177,185)),
+    # (' SFX \nDRUMS', range(185,193)),
+    ('ANON\n  MEL', range(257,273)),
+    ('ANON\n DRUM', range(289,305)),
+]
 def inst_label(i):
     if i is None:
         return f"--- \n-----\n-----"
-    return f'{i:03d} \n{gm_names[i-1]}'
+    return f'{i:03d} \n{gm_names[i]}'
 ### end def TUI components###
 
 
 if __name__=='__main__':
     run(main)
```

### Comparing `notochord-0.5.2/src/notochord/app/improviser-txala.py` & `notochord-0.5.3/src/notochord/app/improviser-txala.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.2/src/notochord/app/improviser.py` & `notochord-0.5.3/src/notochord/app/improviser.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.2/src/notochord/app/server.py` & `notochord-0.5.3/src/notochord/app/server.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.2/src/notochord/app/simple_harmonizer.py` & `notochord-0.5.3/src/notochord/app/simple_harmonizer.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.2/src/notochord/data.py` & `notochord-0.5.3/src/notochord/data.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.2/src/notochord/distributions.py` & `notochord-0.5.3/src/notochord/distributions.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.2/src/notochord/model.py` & `notochord-0.5.3/src/notochord/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,23 +318,29 @@
                     - torch.where(time_targets - 0.03 >= 0,
                         self.time_dist.cdf(time_params, time_targets - 0.03),
                         time_targets.new_zeros([]))
                 )
         return r
 
 
+    # 0 - start token
+    # 1-128 - melodic
+    # 129-256 - drums
+    # 257-288 - anon melodic
+    # 289-320 - anon drums
     def is_drum(self, inst):
         # TODO: add a constructor argument to specify which are drums
         # hardcoded for now
         return inst > 128 and inst < 257 or inst > 288
+    def is_anon(self, inst):
+        return inst > 256
     def first_anon_like(self, inst):
         # TODO: add a constructor argument to specify how many anon
         # hardcoded for now
-        return 288 if self.is_drum(inst) else 257
-
+        return 289 if self.is_drum(inst) else 257
     
     def feed(self, inst, pitch, time, vel, **kw):
         """consume an event and advance hidden state
         
         Args:
             inst: int. instrument of current note.
                 0 is start token
@@ -1181,26 +1187,31 @@
         # for n,t in zip(self.cell_state_names(), self.initial_state):
         #     getattr(self, n)[:] = t.detach()
         # if start:
         #     self.feed(
         #         self.instrument_start_token, self.pitch_start_token, 0., 0.)
 
     @classmethod
+    def user_data_dir(cls):
+        import appdirs
+        d = Path(appdirs.user_data_dir('Notochord', 'IIL'))
+        d.mkdir(exist_ok=True, parents=True)
+        return d
+
+    @classmethod
     def from_checkpoint(cls, path):
         """
         create a Notochord from a checkpoint file containing 
         hyperparameters and model weights.
 
         Args:
             path: file path to Notochord model
         """
         if path=="notochord-latest.ckpt":
-            import appdirs
-            d = Path(appdirs.user_data_dir('Notochord', 'IIL'))
-            d.mkdir(exist_ok=True, parents=True)
+            d = Notochord.user_data_dir()
             path = d / path
             # maybe download
             if not path.is_file():
                 while True:
                     answer = input("Do you want to download a notochord model? (y/n)")
                     if answer.lower() in ["y","yes"]:
                         download_url('https://github.com/Intelligent-Instruments-Lab/iil-python-tools/releases/download/notochord-v0.4.0/notochord_lakh_50G_deep.pt', path)
```

### Comparing `notochord-0.5.2/src/notochord/perform.py` & `notochord-0.5.3/src/notochord/perform.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.2/src/notochord/rnn.py` & `notochord-0.5.3/src/notochord/rnn.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.2/src/notochord/train.py` & `notochord-0.5.3/src/notochord/train.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.2/src/notochord/util.py` & `notochord-0.5.3/src/notochord/util.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.2/PKG-INFO` & `notochord-0.5.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: notochord
-Version: 0.5.2
+Version: 0.5.3
 Summary: Notochord is a real-time neural network model for MIDI performances.
 License: MIT
 Author: Victor Shepardson
 Author-email: victor.shepardson@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
-Requires-Dist: iipyper (>=0.1.3,<0.2.0)
+Requires-Dist: iipyper (>=0.1.4,<0.2.0)
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: pandas (>=2.0,<3.0)
 Requires-Dist: sf2utils (>=0.9,<0.10)
+Requires-Dist: toml-file (>=1.0.5,<2.0.0)
 Requires-Dist: torch (>=1.13,<2.3)
 Requires-Dist: tqdm (>=4.64,<5.0)
 Description-Content-Type: text/markdown
 
 # Notochord ([Documentation](https://intelligent-instruments-lab.github.io/notochord/) | [Paper](https://zenodo.org/record/7088404 "Notochord AIMC 2022 paper") | [Video](https://www.youtube.com/watch?v=mkBKAyudL0A "Notochord AIMC 2022 video"))
  
 <div align="middle">
@@ -44,32 +45,37 @@
 
 run fluidsynth in a terminal. For example, `fluidsynth -v -o midi.portname="fluidsynth" -o synth.midi-bank-select=mma ~/'Downloads/soundfonts/Timbres of Heaven (XGM) 4.00(G).sf2'`
 
 ## Notochord MIDI Apps
 
 Notochord includes several [iipyper](https://github.com/Intelligent-Instruments-Lab/iipyper.git) apps which can be run in a terminal. They have a clickable text-mode user interface and connect directly to MIDI ports, so you can wire them up to your controllers, DAW, etc.
 
-The Notochord harmonizer adds extra concurrent notes for each MIDI note you play in. In a terminal, make sure your notochord Python environment is active and run:
-```
-notochord harmonizer
-```
-try `notochord harmonizer --help`
-to see more options.
-
-the "homunculus" gives you a UI to manage multiple input, harmonizing or autonomous notochord channels:
+The `homunculus` provides a text-based graphical interface to manage multiple input, harmonizing or autonomous notochord channels:
 ```
 notochord homunculus
 ```
 You can set the MIDI in and out ports with `--midi-in` and `--midi-out`. If you use a General MIDI synthesizer like fluidsynth, you can add `--send-pc` to also send program change messages.
 
-If you are using fluidsynth, try:
+If you are using fluidsynth as above, try:
 ```
 notochord homunculus --send-pc --midi-out fluidsynth --thru
 ```
 
+Note: on windows, there are no virtual MIDI ports and no system MIDI loopback, so you may need to attach some MIDI devices or run a loopback driver like [loopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html) before starting the app.
+
+There are also two simpler notochord apps: `improviser` and `harmonizer`. The harmonizer adds extra concurrent notes for each MIDI note you play in. In a terminal, make sure your notochord Python environment is active and run:
+```
+notochord harmonizer
+```
+try `notochord harmonizer --help`
+to see more options.
+
+Development is now focused on `homunculus`, which is intended to subsume all features of `improviser` and `harmonizer`.
+
+
 ## Python API
 
 See the docs for `Notochord.feed` and `Notochord.query` for the low-level Notochord inference API which can be used from Python code. `notochord/app/simple_harmonizer.py` provides a minimal example of how to build an interactive app.
 
 ## OSC server
 
 You can also expose the inference API over Open Sound Control:
```

