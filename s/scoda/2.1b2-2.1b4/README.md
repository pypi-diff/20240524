# Comparing `tmp/scoda-2.1b2.tar.gz` & `tmp/scoda-2.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-2.1b2.tar", last modified: Tue May 21 15:01:16 2024, max compression
+gzip compressed data, was "scoda-2.1b4.tar", last modified: Thu May 23 21:31:15 2024, max compression
```

## Comparing `scoda-2.1b2.tar` & `scoda-2.1b4.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.382685 scoda-2.1b2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-21 15:01:11.000000 scoda-2.1b2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-21 15:01:16.382685 scoda-2.1b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-21 15:01:11.000000 scoda-2.1b2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-21 15:01:11.000000 scoda-2.1b2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.374685 scoda-2.1b2/scoda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.378685 scoda-2.1b2/scoda/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/config/settings.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.378685 scoda-2.1b2/scoda/elements/
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/elements/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/elements/composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/elements/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/elements/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.378685 scoda-2.1b2/scoda/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/exceptions/bar_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/exceptions/sequence_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/exceptions/tokenisation_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/exceptions/track_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.378685 scoda-2.1b2/scoda/midi/
--rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/midi/midi_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/midi/midi_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/midi/midi_track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.378685 scoda-2.1b2/scoda/misc/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/misc/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/misc/enumerations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/misc/music_theory.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/misc/scoda_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/misc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.382685 scoda-2.1b2/scoda/sequences/
--rw-r--r--   0 runner    (1001) docker     (127)    21873 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/sequences/absolute_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/sequences/abstract_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    35040 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/sequences/relative_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    23976 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/sequences/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.382685 scoda-2.1b2/scoda/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/settings/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.382685 scoda-2.1b2/scoda/tokenisation/
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/tokenisation/base_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/tokenisation/gridlike_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/tokenisation/midilike_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    25748 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/tokenisation/notelike_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-05-21 15:01:11.000000 scoda-2.1b2/scoda/tokenisation/transposed_notelike_tokenisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:01:16.382685 scoda-2.1b2/scoda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-21 15:01:16.000000 scoda-2.1b2/scoda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-21 15:01:16.000000 scoda-2.1b2/scoda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:01:16.000000 scoda-2.1b2/scoda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-21 15:01:16.000000 scoda-2.1b2/scoda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 15:01:16.000000 scoda-2.1b2/scoda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:01:16.382685 scoda-2.1b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:31:15.928951 scoda-2.1b4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-23 21:31:11.000000 scoda-2.1b4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-23 21:31:15.928951 scoda-2.1b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-23 21:31:11.000000 scoda-2.1b4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-23 21:31:11.000000 scoda-2.1b4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:31:15.920951 scoda-2.1b4/scoda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:31:15.924951 scoda-2.1b4/scoda/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/config/settings.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:31:15.924951 scoda-2.1b4/scoda/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/elements/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/elements/composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/elements/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/elements/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:31:15.924951 scoda-2.1b4/scoda/enumerations/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/enumerations/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/enumerations/tokenisation_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/enumerations/tokeniser_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:31:15.924951 scoda-2.1b4/scoda/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/exceptions/bar_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/exceptions/sequence_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/exceptions/tokenisation_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/exceptions/track_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:31:15.924951 scoda-2.1b4/scoda/midi/
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/midi/midi_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/midi/midi_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/midi/midi_track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:31:15.924951 scoda-2.1b4/scoda/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/misc/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/misc/music_theory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/misc/scoda_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/misc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:31:15.928951 scoda-2.1b4/scoda/sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)    21887 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/sequences/absolute_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/sequences/abstract_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31799 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/sequences/relative_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23992 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/sequences/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:31:15.928951 scoda-2.1b4/scoda/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/settings/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:31:15.928951 scoda-2.1b4/scoda/tokenisation/
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/tokenisation/base_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/tokenisation/gridlike_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/tokenisation/midilike_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32209 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/tokenisation/notelike_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-05-23 21:31:11.000000 scoda-2.1b4/scoda/tokenisation/transposed_notelike_tokenisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:31:15.928951 scoda-2.1b4/scoda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-23 21:31:15.000000 scoda-2.1b4/scoda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-23 21:31:15.000000 scoda-2.1b4/scoda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:31:15.000000 scoda-2.1b4/scoda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-23 21:31:15.000000 scoda-2.1b4/scoda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 21:31:15.000000 scoda-2.1b4/scoda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:31:15.928951 scoda-2.1b4/setup.cfg
```

### Comparing `scoda-2.1b2/LICENSE.md` & `scoda-2.1b4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scoda-2.1b2/PKG-INFO` & `scoda-2.1b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda
-Version: 2.1b2
+Version: 2.1b4
 Summary: A MIDI and music data manipulation library
 Author-email: Felix Schön <schoen@kr.tuwien.ac.at>
 License: MIT License
         
         Copyright (c) 2023 Felix Schön
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -84,15 +84,15 @@
 We provide a short listing on how to use basic S-Coda functions:
 
 ```python
     # Load sequence, choose correct track (often first track contains only meta messages)
     sequence = Sequence.sequences_load(file_path=RESOURCE_BEETHOVEN)[1]
 
     # Quantise the sequence to thirty-seconds and thirty-second triplets (standard values)
-    sequence.quantise()
+    sequence.quantise_and_normalise()
 
     # Split the sequence into bars based on the occurring time signatures
     bars = Sequence.sequences_split_bars([sequence], meta_track_index=0)[0]
 
     # Prepare tokeniser and output tokens
     tokeniser = StandardNotelikeTokeniser(running_value=True, running_pitch=True, running_time_sig=True)
     tokens = []
@@ -106,10 +106,9 @@
     # (Conduct ML operations on tokens)
     tokens = tokens
 
     # Create sequence from tokens
     detokenised_sequence = tokeniser.detokenise(tokens)
 
     # Save sequence
-    Sequence.save = lambda *args: None
     detokenised_sequence.save("out/generated_sequence.mid")
 ```
```

### Comparing `scoda-2.1b2/README.md` & `scoda-2.1b4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 We provide a short listing on how to use basic S-Coda functions:
 
 ```python
     # Load sequence, choose correct track (often first track contains only meta messages)
     sequence = Sequence.sequences_load(file_path=RESOURCE_BEETHOVEN)[1]
 
     # Quantise the sequence to thirty-seconds and thirty-second triplets (standard values)
-    sequence.quantise()
+    sequence.quantise_and_normalise()
 
     # Split the sequence into bars based on the occurring time signatures
     bars = Sequence.sequences_split_bars([sequence], meta_track_index=0)[0]
 
     # Prepare tokeniser and output tokens
     tokeniser = StandardNotelikeTokeniser(running_value=True, running_pitch=True, running_time_sig=True)
     tokens = []
@@ -60,10 +60,9 @@
     # (Conduct ML operations on tokens)
     tokens = tokens
 
     # Create sequence from tokens
     detokenised_sequence = tokeniser.detokenise(tokens)
 
     # Save sequence
-    Sequence.save = lambda *args: None
     detokenised_sequence.save("out/generated_sequence.mid")
 ```
```

### Comparing `scoda-2.1b2/pyproject.toml` & `scoda-2.1b4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "scoda"
-version = "2.1-beta.2"
+version = "2.1-beta.4"
 authors = [{ name = "Felix Schön", email = "schoen@kr.tuwien.ac.at" }]
 description = "A MIDI and music data manipulation library"
 readme = "README.md"
 requires-python = ">= 3.11"
 keywords = ["midi", "music"]
 license = { file = "LICENSE.md" }
 dependencies = [
```

### Comparing `scoda-2.1b2/scoda/config/settings.json` & `scoda-2.1b4/scoda/config/settings.json`

 * *Files identical despite different names*

### Comparing `scoda-2.1b2/scoda/elements/bar.py` & `scoda-2.1b4/scoda/elements/bar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import copy
 
 from scoda.elements.message import Message
+from scoda.enumerations.message_type import MessageType
 from scoda.exceptions.bar_exception import BarException
-from scoda.misc.enumerations import MessageType
 from scoda.misc.music_theory import Key
 from scoda.sequences.sequence import Sequence
 from scoda.settings.settings import PPQN
 
 
 class Bar:
     """Class representing a single bar, its length defined by a time signature."""
@@ -21,20 +21,20 @@
         self.time_signature_denominator = denominator
         self.key_signature = key
 
         # Adjust sequence
         self.sequence.normalise()
 
         # Assert bar has correct capacity
-        if self.sequence.get_sequence_length_relation() > self.time_signature_numerator * PPQN / (
+        if self.sequence.get_sequence_duration_relation() > self.time_signature_numerator * PPQN / (
                 self.time_signature_denominator / 4):
             raise BarException("Bar capacity exceeded")
 
         # Pad bar
-        if self.sequence.get_sequence_length_relation() < self.time_signature_numerator * PPQN / (
+        if self.sequence.get_sequence_duration_relation() < self.time_signature_numerator * PPQN / (
                 self.time_signature_denominator / 4):
             self.sequence.pad(self.time_signature_numerator * PPQN / (self.time_signature_denominator / 4))
 
         # Assert time signature is consistent
         relative_sequence = self.sequence.rel
         time_signatures = [msg for msg in relative_sequence.messages if
                            msg.message_type == MessageType.TIME_SIGNATURE]
```

### Comparing `scoda-2.1b2/scoda/elements/composition.py` & `scoda-2.1b4/scoda/elements/composition.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b2/scoda/elements/message.py` & `scoda-2.1b4/scoda/elements/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from scoda.misc.enumerations import MessageType
+from scoda.enumerations.message_type import MessageType
 from scoda.misc.music_theory import Key
 
 
 class Message:
     """Class representing a musical message.
     """
```

### Comparing `scoda-2.1b2/scoda/elements/track.py` & `scoda-2.1b4/scoda/elements/track.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import copy
 
 from scoda.elements.bar import Bar
+from scoda.enumerations.message_type import MessageType
 from scoda.exceptions.track_exception import TrackException
-from scoda.misc.enumerations import MessageType
 from scoda.sequences.sequence import Sequence
 
 
 class Track:
     """Class representing a track, which is made of (multiple) bars.
     """
```

### Comparing `scoda-2.1b2/scoda/midi/midi_file.py` & `scoda-2.1b4/scoda/midi/midi_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import copy
 from typing import TYPE_CHECKING
 
 import mido
 
 from scoda.elements.message import Message
+from scoda.enumerations.message_type import MessageType
 from scoda.midi.midi_track import MidiTrack
-from scoda.misc.enumerations import MessageType
 from scoda.misc.scoda_logging import get_logger
 from scoda.settings.settings import PPQN
 
 if TYPE_CHECKING:
     from scoda.sequences.sequence import Sequence
```

### Comparing `scoda-2.1b2/scoda/midi/midi_message.py` & `scoda-2.1b4/scoda/midi/midi_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from scoda.elements.message import Message
-from scoda.misc.enumerations import MessageType
+from scoda.enumerations.message_type import MessageType
 from scoda.misc.music_theory import MusicMapping
 
 
 class MidiMessage:
 
     def __init__(self, message_type=None, control=None, denominator=None, numerator=None, key=None, note=None,
                  time=None, velocity=None, program=None) -> None:
```

### Comparing `scoda-2.1b2/scoda/midi/midi_track.py` & `scoda-2.1b4/scoda/midi/midi_track.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import mido
 
+from scoda.enumerations.message_type import MessageType
 from scoda.midi.midi_message import MidiMessage
-from scoda.misc.enumerations import MessageType
 
 
 class MidiTrack:
 
     def __init__(self) -> None:
         super().__init__()
         self.name = ""
```

### Comparing `scoda-2.1b2/scoda/misc/music_theory.py` & `scoda-2.1b4/scoda/misc/music_theory.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b2/scoda/misc/scoda_logging.py` & `scoda-2.1b4/scoda/misc/scoda_logging.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b2/scoda/misc/util.py` & `scoda-2.1b4/scoda/misc/util.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b2/scoda/sequences/absolute_sequence.py` & `scoda-2.1b4/scoda/sequences/absolute_sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import copy
 from statistics import geometric_mean
 from typing import TYPE_CHECKING
 
 from scoda.elements.message import Message
+from scoda.enumerations.message_type import MessageType
 from scoda.exceptions.sequence_exception import SequenceException
-from scoda.misc.enumerations import MessageType
 from scoda.misc.scoda_logging import get_logger
 from scoda.misc.util import binary_insort, find_minimal_distance, regress, minmax, simple_regression, \
     get_note_durations, \
     get_tuplet_durations, get_dotted_note_durations
 from scoda.sequences.abstract_sequence import AbstractSequence
 from scoda.settings.settings import PPQN, DIFF_DUAL_NOTE_VALUES_UPPER_BOUND, \
     DIFF_DUAL_NOTE_VALUES_LOWER_BOUND, NOTE_VALUE_UPPER_BOUND, NOTE_VALUE_LOWER_BOUND, VALID_TUPLETS, DOTTED_ITERATIONS, \
@@ -382,18 +382,18 @@
 
         for msg in self.messages:
             if msg.message_type in message_types:
                 timings.append((msg.time, msg))
 
         return timings
 
-    def get_sequence_length(self) -> int:
-        """Calculates the overall length of this sequence, given in ticks.
+    def get_sequence_duration(self) -> int:
+        """Calculates the overall duration of this sequence, given in ticks.
 
-        Returns: The length of this sequence.
+        Returns: The duration of this sequence.
 
         """
         return self.messages[-1].time
 
     def to_relative_sequence(self) -> RelativeSequence:
         """Converts this AbsoluteSequence to a RelativeSequence.
```

### Comparing `scoda-2.1b2/scoda/sequences/abstract_sequence.py` & `scoda-2.1b4/scoda/sequences/abstract_sequence.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b2/scoda/sequences/relative_sequence.py` & `scoda-2.1b4/scoda/sequences/relative_sequence.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import math
 import re
 import time
 from statistics import mean
 from typing import TYPE_CHECKING
 
 from scoda.elements.message import Message
+from scoda.enumerations.message_type import MessageType
 from scoda.exceptions.sequence_exception import SequenceException
 from scoda.midi.midi_message import MidiMessage
 from scoda.midi.midi_track import MidiTrack
-from scoda.misc.enumerations import MessageType
 from scoda.misc.music_theory import Note, Key, MusicMapping
 from scoda.misc.scoda_logging import get_logger
 from scoda.misc.util import minmax, simple_regression
 from scoda.sequences.abstract_sequence import AbstractSequence
 from scoda.settings.settings import NOTE_LOWER_BOUND, NOTE_UPPER_BOUND, PPQN, DIFF_DUAL_DISTANCES_UPPER_BOUND, \
     DIFF_DUAL_DISTANCES_LOWER_BOUND, DIFF_DUAL_PATTERN_COVERAGE_UPPER_BOUND, DIFF_DUAL_PATTERN_COVERAGE_LOWER_BOUND, \
     PATTERN_LENGTH_MIN, REGEX_PATTERN, REGEX_SUBPATTERN, DIFF_DUAL_NOTE_CLASSES_UPPER_BOUND, \
@@ -241,15 +241,14 @@
         # Add current sequence if it is not empty
         if len(current_sequence.messages) > 0:
             split_sequences.append(current_sequence)
 
         return split_sequences
 
     def scale(self, factor, meta_sequence=None) -> None:
-        # TODO Without normalisation inserts double time signature - check why
         """Stretches the sequence by the given factor.
 
         Args:
             factor: Factor to stretch by.
             meta_sequence: Sequence containing the time signatures to apply.
 
         """
@@ -395,96 +394,27 @@
                     best_index = i
                     best_solution = key_candidates[i]
                     best_solution_accidentals = key_note_mapping[i][1][1]
 
         guessed_key = [key for key in MusicMapping.KeyNoteMapping][best_index]
         return guessed_key
 
-    def get_sequence_length_relation(self) -> float:
-        """Calculates the length of the sequence in multiples of the `PPQN`.
+    def get_sequence_duration_relation(self) -> float:
+        """Calculates the duration of the sequence in multiples of the `PPQN`.
 
-        Returns: The length of the sequence as a multiple of the `PPQN`.
+        Returns: The duration of the sequence as a multiple of the `PPQN`.
 
         """
-        length = 0
+        duration = 0
 
         for msg in self.messages:
             if msg.message_type == MessageType.WAIT:
-                length += msg.time
+                duration += msg.time
 
-        return length / PPQN
-
-    def get_valid_next_messages(self, desired_bars, force_time_signature=True, maximum_note_length=-1) -> list[dict]:
-        """Determines, which messages are valid messages to be inserted into this sequence.
-
-        Returns: A list of valid message types
-
-        """
-        amount_bars_completed = 0
-        current_bar_capacity = 4 * PPQN
-        current_point_in_time = 0
-        current_bar_time = 0
-        at_bar_border = True
-
-        open_messages = dict()
-
-        for msg in self.messages:
-            if msg.message_type == MessageType.NOTE_ON:
-                at_bar_border = False
-                open_messages[msg.note] = current_point_in_time
-            elif msg.message_type == MessageType.NOTE_OFF:
-                open_messages.pop(msg.note, None)
-            elif msg.message_type == MessageType.WAIT:
-                at_bar_border = False
-
-                current_point_in_time += msg.time
-                current_bar_time += msg.time
-
-                if current_bar_time == current_bar_capacity:
-                    at_bar_border = True
-                    amount_bars_completed += 1
-                    current_bar_time -= current_bar_capacity
-
-                while current_bar_time > current_bar_capacity:
-                    current_bar_time -= current_bar_capacity
-                    amount_bars_completed += 1
-            elif msg.message_type == MessageType.TIME_SIGNATURE:
-                if not at_bar_border:
-                    raise SequenceException("Time signature message may only occur at border of a bar")
-                at_bar_border = False
-
-                current_bar_capacity = PPQN * (msg.numerator / (msg.denominator / 4))
-
-        valid_messages = []
-
-        if amount_bars_completed < desired_bars and not (at_bar_border and force_time_signature):
-            for wait_time in range(1, PPQN + 1):
-                if (
-                        current_bar_time + wait_time <= current_bar_capacity or
-                        current_bar_time + wait_time <= 2 * current_bar_capacity and
-                        amount_bars_completed + 1 < desired_bars) \
-                        and (maximum_note_length == -1 or all(
-                    current_point_in_time + wait_time - value <= maximum_note_length for value in
-                    open_messages.values())
-                ):
-                    valid_messages.append({"message_type": MessageType.WAIT.value, "time": wait_time})
-
-        for note in range(NOTE_LOWER_BOUND, NOTE_UPPER_BOUND + 1):
-            if note not in open_messages and amount_bars_completed < desired_bars and not (
-                    at_bar_border and force_time_signature):
-                valid_messages.append({"message_type": MessageType.NOTE_ON.value, "note": note})
-
-        for note in range(NOTE_LOWER_BOUND, NOTE_UPPER_BOUND + 1):
-            if note in open_messages and open_messages[note] != current_point_in_time:
-                valid_messages.append({"message_type": MessageType.NOTE_OFF.value, "note": note})
-
-        if at_bar_border and amount_bars_completed < desired_bars:
-            valid_messages.append({"message_type": MessageType.TIME_SIGNATURE.value})
-
-        return valid_messages
+        return duration / PPQN
 
     def to_absolute_sequence(self) -> AbsoluteSequence:
         """Converts this `RelativeSequence` to an `AbsoluteSequence`.
 
         Returns: The absolute representation of this sequence.
 
         """
@@ -538,15 +468,15 @@
         violations = 0
 
         for msg in self.messages:
             if msg.message_type == MessageType.NOTE_ON:
                 if Note(msg.note % 12) not in note_mapping[0]:
                     violations += 1
 
-        relation = violations / self.get_sequence_length_relation()
+        relation = violations / self.get_sequence_duration_relation()
         scaled_relation = simple_regression(DIFF_DUAL_ACCIDENTALS_UPPER_BOUND, 1, DIFF_DUAL_ACCIDENTALS_LOWER_BOUND, 0,
                                             relation)
 
         return minmax(0, 1, scaled_relation)
 
     def diff_concurrent_notes(self) -> float:
         """Calculates the difficulty of the sequence based on the amount of concurrent notes.
@@ -667,22 +597,22 @@
         """Calculates difficulty of the sequence based on the amount of notes played.
 
         Returns: A value from 0 (low difficulty) to 1 (high difficulty).
 
         """
         amount_notes_played = 0
 
-        if self.get_sequence_length_relation() == 0:
+        if self.get_sequence_duration_relation() == 0:
             return 0
 
         for msg in self.messages:
             if msg.message_type == MessageType.NOTE_ON:
                 amount_notes_played += 1
 
-        relation = amount_notes_played / self.get_sequence_length_relation()
+        relation = amount_notes_played / self.get_sequence_duration_relation()
 
         scaled_difficulty = simple_regression(DIFF_DUAL_NOTE_AMOUNT_UPPER_BOUND, 1, DIFF_DUAL_NOTE_AMOUNT_LOWER_BOUND,
                                               0,
                                               relation)
 
         return minmax(0, 1, scaled_difficulty)
 
@@ -699,15 +629,15 @@
             if msg.message_type == MessageType.NOTE_ON and msg.note not in note_classes:
                 note_classes.append(msg.note)
 
         # If sequence is empty, return easiest difficulty
         if len(note_classes) == 0:
             return 0
 
-        relation = len(note_classes) / self.get_sequence_length_relation()
+        relation = len(note_classes) / self.get_sequence_duration_relation()
         scaled_relation = simple_regression(DIFF_DUAL_NOTE_CLASSES_UPPER_BOUND, 1, DIFF_DUAL_NOTE_CLASSES_LOWER_BOUND,
                                             0,
                                             relation)
 
         return minmax(0, 1, scaled_relation)
 
     def diff_pattern(self) -> float:
```

### Comparing `scoda-2.1b2/scoda/sequences/sequence.py` & `scoda-2.1b4/scoda/sequences/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from typing import TYPE_CHECKING
 
 import numpy as np
 from matplotlib import pyplot as plt, pyplot
 from matplotlib.patches import Rectangle
 
 from scoda.elements.message import Message
+from scoda.enumerations.message_type import MessageType
 from scoda.midi.midi_file import MidiFile
 from scoda.midi.midi_track import MidiTrack
-from scoda.misc.enumerations import MessageType
 from scoda.misc.music_theory import Key
 from scoda.misc.util import minmax, simple_regression
 from scoda.sequences.absolute_sequence import AbsoluteSequence
 from scoda.sequences.relative_sequence import RelativeSequence
 from scoda.settings.settings import PPQN, NOTE_LOWER_BOUND, NOTE_UPPER_BOUND, VELOCITY_MAX
 
 if TYPE_CHECKING:
@@ -216,25 +216,25 @@
 
     def get_message_timings_of_type(self, message_types: [MessageType]) -> list[tuple[int, Message]]:
         """See `scoda.sequence.absolute_sequence.AbsoluteSequence.get_message_timings_of_type`.
 
         """
         return self.abs.get_message_timings_of_type(message_types)
 
-    def get_sequence_length(self) -> float:
+    def get_sequence_duration(self) -> float:
         """See `scoda.sequence.absolute_sequence.AbsoluteSequence.get_sequence_length`.
 
         """
-        return self.abs.get_sequence_length()
+        return self.abs.get_sequence_duration()
 
-    def get_sequence_length_relation(self) -> float:
+    def get_sequence_duration_relation(self) -> float:
         """See `scoda.sequence.relative_sequence.RelativeSequence.sequence_length_relation`.
 
         """
-        return self.rel.get_sequence_length_relation()
+        return self.rel.get_sequence_duration_relation()
 
     def is_empty(self) -> bool:
         """See `scoda.sequence.relative_sequence.RelativeSequence.is_empty`.
 
         """
         return self.rel.is_empty()
```

### Comparing `scoda-2.1b2/scoda/settings/settings.py` & `scoda-2.1b4/scoda/settings/settings.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b2/scoda/tokenisation/base_tokenisation.py` & `scoda-2.1b4/scoda/tokenisation/base_tokenisation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from abc import ABC, abstractmethod
 
+from scoda.enumerations.tokenisation_flags import TokenisationFlags
 from scoda.exceptions.tokenisation_exception import TokenisationException
-from scoda.misc.enumerations import Flags
 from scoda.sequences.sequence import Sequence
 from scoda.settings.settings import PPQN
 
 
 class BaseTokeniser(ABC):
 
     def __init__(self, running_time_sig: bool) -> None:
         super().__init__()
 
         self.flags = dict()
-        self.flags[Flags.RUNNING_TIME_SIG] = running_time_sig
+        self.flags[TokenisationFlags.RUNNING_TIME_SIG] = running_time_sig
 
         self.cur_time = None
         self.cur_time_target = None
         self.cur_rest_buffer = None
 
         self.prv_type = None
         self.prv_note = None
@@ -56,25 +56,25 @@
         return tokens
 
     def _notelike_tokenise_flush_rest_buffer(self, apply_target: bool, wait_token: int, value_shift: int) -> list[int]:
         tokens = []
 
         # Insert rests of length up to `set_max_rest_value`
         while self.cur_rest_buffer > self.set_max_rest_value:
-            if not (self.prv_value == self.set_max_rest_value and self.flags.get(Flags.RUNNING_VALUE, False)):
+            if not (self.prv_value == self.set_max_rest_value and self.flags.get(TokenisationFlags.RUNNING_VALUE, False)):
                 tokens.append(int(self.set_max_rest_value + value_shift))
                 self.prv_value = self.set_max_rest_value
 
             tokens.append(int(wait_token))
             self.cur_time += self.set_max_rest_value
             self.cur_rest_buffer -= self.set_max_rest_value
 
         # Insert rests smaller than `set_max_rest_value`
         if self.cur_rest_buffer > 0:
-            if not (self.prv_value == self.cur_rest_buffer and self.flags.get(Flags.RUNNING_VALUE, False)):
+            if not (self.prv_value == self.cur_rest_buffer and self.flags.get(TokenisationFlags.RUNNING_VALUE, False)):
                 tokens.append(int(self.cur_rest_buffer + value_shift))
                 self.prv_value = self.cur_rest_buffer
             tokens.append(int(wait_token))
 
         self.cur_time += self.cur_rest_buffer
         self.cur_rest_buffer = 0
```

### Comparing `scoda-2.1b2/scoda/tokenisation/gridlike_tokenisation.py` & `scoda-2.1b4/scoda/tokenisation/gridlike_tokenisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import math
 from abc import ABC
 
 from scoda.elements.message import Message
+from scoda.enumerations.message_type import MessageType
+from scoda.enumerations.tokenisation_flags import TokenisationFlags
 from scoda.exceptions.tokenisation_exception import TokenisationException
-from scoda.misc.enumerations import MessageType, Flags
 from scoda.sequences.sequence import Sequence
 from scoda.tokenisation.base_tokenisation import BaseTokeniser
 
 
 class BaseGridlikeTokeniser(BaseTokeniser, ABC):
 
     def __init__(self, running_time_sig: bool) -> None:
@@ -86,15 +87,15 @@
                 self.prv_type = MessageType.NOTE_OFF
             elif msg_type == MessageType.TIME_SIGNATURE:
                 msg_numerator = message.numerator
                 msg_denominator = message.denominator
 
                 numerator = self._time_signature_to_eights(msg_numerator, msg_denominator)
 
-                if not (self.prv_numerator == numerator and self.flags.get(Flags.RUNNING_TIME_SIG, False)):
+                if not (self.prv_numerator == numerator and self.flags.get(TokenisationFlags.RUNNING_TIME_SIG, False)):
                     tokens.extend(self._gridlike_tokenise_flush_grid_buffer(min_grid_size=min_grid_size, wait_token=3))
                     tokens.append(numerator - 2 + 204)
 
                 self.prv_type = MessageType.TIME_SIGNATURE
                 self.prv_numerator = numerator
 
         if apply_buffer and self.cur_rest_buffer > 0:
```

### Comparing `scoda-2.1b2/scoda/tokenisation/midilike_tokenisation.py` & `scoda-2.1b4/scoda/tokenisation/midilike_tokenisation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from abc import ABC
 
 from scoda.elements.message import Message
+from scoda.enumerations.message_type import MessageType
+from scoda.enumerations.tokenisation_flags import TokenisationFlags
 from scoda.exceptions.tokenisation_exception import TokenisationException
-from scoda.misc.enumerations import Flags, MessageType
 from scoda.sequences.sequence import Sequence
 from scoda.tokenisation.base_tokenisation import BaseTokeniser
 
 
 class BaseMidilikeTokeniser(BaseTokeniser, ABC):
 
     def __init__(self, running_time_sig: bool) -> None:
@@ -65,15 +66,15 @@
                 self.prv_type = MessageType.NOTE_OFF
             elif msg_type == MessageType.TIME_SIGNATURE:
                 msg_numerator = message.numerator
                 msg_denominator = message.denominator
 
                 numerator = self._time_signature_to_eights(msg_numerator, msg_denominator)
 
-                if not (self.prv_numerator == numerator and self.flags.get(Flags.RUNNING_TIME_SIG, False)):
+                if not (self.prv_numerator == numerator and self.flags.get(TokenisationFlags.RUNNING_TIME_SIG, False)):
                     tokens.extend(self._general_tokenise_flush_time_buffer(time=self.cur_rest_buffer, value_shift=3))
                     self.cur_rest_buffer = 0
 
                     tokens.append(numerator - 2 + 204)
 
                 self.prv_type = MessageType.TIME_SIGNATURE
                 self.prv_numerator = numerator
```

### Comparing `scoda-2.1b2/scoda/tokenisation/notelike_tokenisation.py` & `scoda-2.1b4/scoda/tokenisation/notelike_tokenisation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import math
 from abc import ABC
+from typing import Any
 
 from scoda.elements.message import Message
+from scoda.enumerations.message_type import MessageType
+from scoda.enumerations.tokenisation_flags import TokenisationFlags
 from scoda.exceptions.tokenisation_exception import TokenisationException
-from scoda.misc.enumerations import Flags, MessageType
 from scoda.misc.music_theory import CircleOfFifths
 from scoda.sequences.sequence import Sequence
 from scoda.settings.settings import PPQN
 from scoda.tokenisation.base_tokenisation import BaseTokeniser
 
 
 class BaseNotelikeTokeniser(BaseTokeniser, ABC):
 
     def __init__(self, running_value: bool, running_time_sig: bool) -> None:
         super().__init__(running_time_sig)
 
-        self.flags[Flags.RUNNING_VALUE] = running_value
+        self.flags[TokenisationFlags.RUNNING_VALUE] = running_value
 
 
 class StandardNotelikeTokeniser(BaseNotelikeTokeniser):
     """Tokeniser that uses note-like temporal representation.
 
     [        0] ... pad
     [        1] ... start
@@ -31,15 +33,15 @@
     [117 - 131] ... time signature numerator in eights from 2/8 to 16/8
     [      132] ... note with previous pitch (running pitch only)
     """
 
     def __init__(self, running_value: bool, running_pitch: bool, running_time_sig: bool) -> None:
         super().__init__(running_value, running_time_sig)
 
-        self.flags[Flags.RUNNING_PITCH] = running_pitch
+        self.flags[TokenisationFlags.RUNNING_PITCH] = running_pitch
 
     def tokenise(self, sequence: Sequence, apply_buffer: bool = True, reset_time: bool = True,
                  insert_trailing_separator_token: bool = True, insert_border_tokens: bool = False) -> list[int]:
         tokens = []
         event_pairings = sequence.abs.get_message_time_pairings(
             [MessageType.NOTE_ON, MessageType.NOTE_OFF, MessageType.TIME_SIGNATURE, MessageType.INTERNAL])
 
@@ -57,19 +59,19 @@
                 # Check if message occurs at current time, if not place rest messages
                 if not self.cur_time == msg_time:
                     self.cur_rest_buffer += msg_time - self.cur_time
                     tokens.extend(
                         self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=3, value_shift=4))
 
                 # Check if value of note has to be defined
-                if not (self.prv_value == msg_value and self.flags.get(Flags.RUNNING_VALUE, False)):
+                if not (self.prv_value == msg_value and self.flags.get(TokenisationFlags.RUNNING_VALUE, False)):
                     tokens.extend(self._general_tokenise_flush_time_buffer(msg_value, value_shift=4))
 
                 # Check if pitch of note has to be defined
-                if not (self.prv_note == msg_note and self.flags.get(Flags.RUNNING_PITCH, False)):
+                if not (self.prv_note == msg_note and self.flags.get(TokenisationFlags.RUNNING_PITCH, False)):
                     tokens.append(msg_note - 21 + 29)
                 else:
                     tokens.append(132)
 
                 self.cur_time_target = max(self.cur_time_target, self.cur_time + msg_value)
                 self.prv_type = MessageType.NOTE_ON
                 self.prv_note = msg_note
@@ -77,15 +79,15 @@
             elif msg_type == MessageType.TIME_SIGNATURE:
                 msg_numerator = event_pairing[0].numerator
                 msg_denominator = event_pairing[0].denominator
 
                 numerator = self._time_signature_to_eights(msg_numerator, msg_denominator)
 
                 # Check if time signature has to be defined
-                if not (self.prv_numerator == numerator and self.flags.get(Flags.RUNNING_TIME_SIG, False)):
+                if not (self.prv_numerator == numerator and self.flags.get(TokenisationFlags.RUNNING_TIME_SIG, False)):
                     self.cur_rest_buffer += msg_time - self.cur_time
                     tokens.extend(
                         self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=3, value_shift=3))
                     tokens.append(numerator - 2 + 117)
 
                 self.prv_type = MessageType.TIME_SIGNATURE
                 self.prv_numerator = numerator
@@ -153,14 +155,162 @@
                 prv_type = MessageType.NOTE_ON
             else:
                 raise TokenisationException(f"Encountered invalid token during detokenisation: {token}")
 
         return seq
 
     @staticmethod
+    def get_constraints(tokens: list[int], previous_state: dict = None, min_bars: int = -1,
+                        running_value: bool = False, running_pitch: bool = False, running_time_sig: bool = False) -> \
+            tuple[list[int], dict[str, Any]]:
+        cur_time = 0
+        cur_bar = 0
+        bar_time = 0
+        bar_tokens = []
+        bar_open_notes = []
+        bar_capacity = None
+        seq_started = False
+        seq_stopped = False
+        prv_type = None
+        prv_note = None
+        prv_value = math.nan
+
+        if previous_state is not None:
+            cur_time = previous_state["cur_time"]
+            cur_bar = previous_state["cur_bar"]
+            bar_time = previous_state["bar_time"]
+            bar_tokens = previous_state["bar_tokens"]
+            bar_open_notes = previous_state["bar_open_notes"]
+            bar_capacity = previous_state["bar_capacity"]
+            seq_started = previous_state["seq_started"]
+            seq_stopped = previous_state["seq_stopped"]
+            prv_type = previous_state["prv_type"]
+            prv_note = previous_state["prv_note"]
+            prv_value = previous_state["prv_value"]
+
+        # === Retrace sequence ===
+
+        for token in tokens:
+            if token == 0:
+                bar_tokens.append(token)
+                prv_type = MessageType.SEQUENCE_CONTROL
+            elif token == 1:
+                bar_tokens.append(token)
+                seq_started = True
+                prv_type = MessageType.SEQUENCE_CONTROL
+            elif token == 2:
+                bar_tokens.append(token)
+                seq_stopped = True
+                prv_type = MessageType.SEQUENCE_CONTROL
+            elif token == 3:
+                cur_time += prv_value
+                bar_time += prv_value
+
+                while bar_time > bar_capacity:
+                    bar_time -= bar_capacity
+                    cur_bar += 1
+
+                bar_tokens.append(token)
+                bar_open_notes = []
+                prv_type = MessageType.WAIT
+            elif token == 4:
+                cur_bar += 1
+                bar_time = 0
+                bar_tokens.append(token)
+                prv_type = MessageType.SEQUENCE_CONTROL
+            elif 5 <= token <= 28:
+                bar_tokens.append(token)
+                if prv_type != MessageType.INTERNAL:
+                    prv_value = 0
+                prv_value += token - 4
+                prv_type = MessageType.INTERNAL
+            elif 29 <= token <= 116:
+                bar_tokens.append(token)
+                bar_open_notes.append(token - 29 + 21)
+                prv_type = MessageType.NOTE_ON
+                prv_note = token - 29 + 21
+            elif 117 <= token <= 131:
+                bar_tokens.append(token)
+                bar_capacity = int(((token - 117 + 2) / 8) * 4 * PPQN)
+                prv_type = MessageType.TIME_SIGNATURE
+            elif token == 132:
+                bar_tokens.append(token)
+                bar_open_notes.append(prv_note)
+                prv_type = MessageType.NOTE_ON
+            else:
+                raise TokenisationException(f"Encountered invalid token during constraint creation: {token}")
+
+            if not running_value and not 5 <= token <= 28:
+                prv_value = None
+
+        # === Retrieve valid tokens ===
+
+        # Helper variables
+        h_started_not_stopped = seq_started and not seq_stopped
+        h_bar_contains_time_signature = any(117 <= t <= 131 for t in bar_tokens)
+        h_bar_valid_time_signature = (running_time_sig and bar_capacity is not None) or h_bar_contains_time_signature
+        h_note_not_open = lambda x: x is not None and x not in bar_open_notes
+        h_has_prv_value = prv_value is not None
+
+        valid_tokens = []
+
+        # [        0] ... pad
+        if seq_started and seq_stopped:
+            valid_tokens.append(0)
+        # [        1] ... start
+        if not seq_started:
+            valid_tokens.append(1)
+        # [        2] ... stop
+        if not seq_stopped and (min_bars == -1 or cur_bar + 1 == min_bars) and bar_time == bar_capacity:
+            valid_tokens.append(2)
+        # [        3] ... wait
+        if h_started_not_stopped and h_bar_valid_time_signature and h_has_prv_value and bar_capacity - bar_time >= prv_value:
+            valid_tokens.append(3)
+        # [        4] ... bar separator
+        if h_started_not_stopped and h_bar_valid_time_signature and bar_time == bar_capacity and 4 not in bar_tokens:
+            valid_tokens.append(4)
+        # [  5 -  28] ... value definition
+        if h_started_not_stopped and h_bar_valid_time_signature:
+            prv_value_volatile = prv_value
+            if prv_type != MessageType.INTERNAL:
+                prv_value_volatile = 0
+            for v_d in range(1, 24 + 1):
+                if bar_capacity - bar_time >= prv_value_volatile + v_d:
+                    valid_tokens.append(v_d + 4)
+        # [ 29 - 116] ... note
+        if h_started_not_stopped and h_bar_valid_time_signature and h_has_prv_value:
+            for n in range(21, 108 + 1):
+                if prv_note not in bar_open_notes:
+                    valid_tokens.append(n - 21 + 29)
+        # [117 - 131] ... time signature numerator in eights from 2/8 to 16/8
+        if h_started_not_stopped and not h_bar_contains_time_signature and bar_time == 0:
+            for t in range(117, 131 + 1):
+                valid_tokens.append(t)
+        # [      132] ... note with previous pitch (running pitch only)
+        if h_started_not_stopped and h_bar_valid_time_signature and running_pitch and h_has_prv_value and h_note_not_open(
+                prv_note):
+            valid_tokens.append(132)
+
+        # === Store and return finding ===
+
+        state = {"cur_time": cur_time,
+                 "cur_bar": cur_bar,
+                 "bar_time": bar_time,
+                 "bar_tokens": bar_tokens,
+                 "bar_open_notes": bar_open_notes,
+                 "bar_capacity": bar_capacity,
+                 "seq_started": seq_started,
+                 "seq_stopped": seq_stopped,
+                 "prv_type": prv_type,
+                 "prv_note": prv_note,
+                 "prv_value": prv_value}
+
+        return valid_tokens, state
+
+    @staticmethod
     def get_info_notes(tokens: list[int], invalid_value: int = -1) -> list[int]:
         info = []
         prv_note = None
 
         for token in tokens:
             if token == 132:
                 info.append(prv_note)
@@ -344,15 +494,15 @@
     [ 46 -  57] ... note without octave in distance on the circle of fifths
     [ 58 -  73] ... time signature numerator in eights from 2/8 to 16/8
     """
 
     def __init__(self, running_value: bool, running_octave: bool, running_time_sig: bool) -> None:
         super().__init__(running_value, running_time_sig)
 
-        self.flags[Flags.RUNNING_OCTAVE] = running_octave
+        self.flags[TokenisationFlags.RUNNING_OCTAVE] = running_octave
 
         self.prv_octave = None
 
     def reset_previous(self) -> None:
         super().reset_previous()
 
         # A4 as base note
@@ -379,20 +529,20 @@
                 # Check if message occurs at current time, if not place rest messages
                 if not self.cur_time == msg_time:
                     self.cur_rest_buffer += msg_time - self.cur_time
                     tokens.extend(
                         self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=3, value_shift=4))
 
                 # Check if value of note has to be defined
-                if not (self.prv_value == msg_value and self.flags.get(Flags.RUNNING_VALUE, False)):
+                if not (self.prv_value == msg_value and self.flags.get(TokenisationFlags.RUNNING_VALUE, False)):
                     tokens.extend(self._general_tokenise_flush_time_buffer(msg_value, value_shift=4))
 
                 # Check if octave of note hast to be defined
                 octave_tgt = msg_note // 12 - 1
-                if not (self.prv_octave == octave_tgt and self.flags.get(Flags.RUNNING_OCTAVE, False)):
+                if not (self.prv_octave == octave_tgt and self.flags.get(TokenisationFlags.RUNNING_OCTAVE, False)):
                     octave_src = self.prv_note // 12 - 1
                     octave_shift = octave_tgt - octave_src
                     assert -8 <= octave_shift <= 8
                     tokens.append((octave_shift + 8) + 29)
 
                 cof_dist = CircleOfFifths.get_distance(self.prv_note, msg_note)
 
@@ -406,15 +556,15 @@
             elif msg_type == MessageType.TIME_SIGNATURE:
                 msg_numerator = event_pairing[0].numerator
                 msg_denominator = event_pairing[0].denominator
 
                 numerator = self._time_signature_to_eights(msg_numerator, msg_denominator)
 
                 # Check if time signature has to be defined
-                if not (self.prv_numerator == numerator and self.flags.get(Flags.RUNNING_TIME_SIG, False)):
+                if not (self.prv_numerator == numerator and self.flags.get(TokenisationFlags.RUNNING_TIME_SIG, False)):
                     self.cur_rest_buffer += msg_time - self.cur_time
                     tokens.extend(
                         self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=3, value_shift=4))
                     tokens.append(numerator - 2 + 58)
 
                 self.prv_type = MessageType.TIME_SIGNATURE
                 self.prv_numerator = numerator
@@ -561,15 +711,15 @@
             elif msg_type == MessageType.TIME_SIGNATURE:
                 msg_numerator = event_pairing[0].numerator
                 msg_denominator = event_pairing[0].denominator
 
                 numerator = self._time_signature_to_eights(msg_numerator, msg_denominator)
 
                 # Check if time signature has to be defined
-                if not (self.prv_numerator == numerator and self.flags.get(Flags.RUNNING_TIME_SIG, False)):
+                if not (self.prv_numerator == numerator and self.flags.get(TokenisationFlags.RUNNING_TIME_SIG, False)):
                     self.cur_rest_buffer += msg_time - self.cur_time
                     tokens.extend(
                         self._general_tokenise_flush_time_buffer(time=self.cur_rest_buffer, value_shift=3))
                     self.cur_time += self.cur_rest_buffer
                     self.cur_rest_buffer = 0
                     tokens.append(numerator - 2 + len(LargeDictionaryNotelikeTokeniser.SUPPORTED_VALUES) * 88 + 4 + 24)
```

### Comparing `scoda-2.1b2/scoda/tokenisation/transposed_notelike_tokenisation.py` & `scoda-2.1b4/scoda/tokenisation/transposed_notelike_tokenisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import math
 from abc import ABC
 
 from scoda.elements.message import Message
+from scoda.enumerations.message_type import MessageType
+from scoda.enumerations.tokenisation_flags import TokenisationFlags
 from scoda.exceptions.tokenisation_exception import TokenisationException
-from scoda.misc.enumerations import Flags, MessageType
 from scoda.sequences.sequence import Sequence
 from scoda.settings.settings import PPQN
 from scoda.tokenisation.base_tokenisation import BaseTokeniser
 
 
 class BaseTransposedNotelikeTokeniser(BaseTokeniser, ABC):
 
@@ -30,15 +31,15 @@
     [ 30 - 117] ... note
     [118 - 132] ... time signature numerator in eights from 2/8 to 16/8
     """
 
     def __init__(self, running_value: bool, running_time_sig: bool) -> None:
         super().__init__(running_time_sig)
 
-        self.flags[Flags.RUNNING_VALUE] = running_value
+        self.flags[TokenisationFlags.RUNNING_VALUE] = running_value
 
     def tokenise(self, bar_seq: Sequence, apply_buffer: bool = True, reset_time: bool = True,
                  insert_border_tokens: bool = False) -> list[int]:
         tokens = []
         event_pairings = bar_seq.abs.get_message_time_pairings(
             [MessageType.NOTE_ON, MessageType.NOTE_OFF, MessageType.TIME_SIGNATURE, MessageType.INTERNAL])
 
@@ -98,15 +99,15 @@
                     # Check if message occurs at current time, if not place rest messages
                     if not self.cur_time == msg_time:
                         self.cur_rest_buffer += msg_time - self.cur_time
                         tokens.extend(
                             self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=4, value_shift=5))
 
                     # Check if value of note has to be defined
-                    if not (self.prv_value == msg_value and self.flags.get(Flags.RUNNING_VALUE, False)):
+                    if not (self.prv_value == msg_value and self.flags.get(TokenisationFlags.RUNNING_VALUE, False)):
                         tokens.extend(self._general_tokenise_flush_time_buffer(msg_value, value_shift=5))
 
                     # Play note
                     tokens.append(3)
 
                     self.cur_time_target = max(self.cur_time_target, self.cur_time + msg_value)
                     self.prv_type = MessageType.NOTE_ON
@@ -114,15 +115,15 @@
                 elif msg_type == MessageType.TIME_SIGNATURE:
                     msg_numerator = event_pairing[0].numerator
                     msg_denominator = event_pairing[0].denominator
 
                     numerator = self._time_signature_to_eights(msg_numerator, msg_denominator)
 
                     # Check if time signature has to be defined
-                    if not (self.prv_numerator == numerator and self.flags.get(Flags.RUNNING_TIME_SIG, False)):
+                    if not (self.prv_numerator == numerator and self.flags.get(TokenisationFlags.RUNNING_TIME_SIG, False)):
                         self.cur_rest_buffer += msg_time - self.cur_time
                         tokens.extend(
                             self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=4, value_shift=5))
                         tokens.append(numerator - 2 + 118)
 
                     self.prv_type = MessageType.TIME_SIGNATURE
                     self.prv_numerator = numerator
```

### Comparing `scoda-2.1b2/scoda.egg-info/PKG-INFO` & `scoda-2.1b4/scoda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda
-Version: 2.1b2
+Version: 2.1b4
 Summary: A MIDI and music data manipulation library
 Author-email: Felix Schön <schoen@kr.tuwien.ac.at>
 License: MIT License
         
         Copyright (c) 2023 Felix Schön
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -84,15 +84,15 @@
 We provide a short listing on how to use basic S-Coda functions:
 
 ```python
     # Load sequence, choose correct track (often first track contains only meta messages)
     sequence = Sequence.sequences_load(file_path=RESOURCE_BEETHOVEN)[1]
 
     # Quantise the sequence to thirty-seconds and thirty-second triplets (standard values)
-    sequence.quantise()
+    sequence.quantise_and_normalise()
 
     # Split the sequence into bars based on the occurring time signatures
     bars = Sequence.sequences_split_bars([sequence], meta_track_index=0)[0]
 
     # Prepare tokeniser and output tokens
     tokeniser = StandardNotelikeTokeniser(running_value=True, running_pitch=True, running_time_sig=True)
     tokens = []
@@ -106,10 +106,9 @@
     # (Conduct ML operations on tokens)
     tokens = tokens
 
     # Create sequence from tokens
     detokenised_sequence = tokeniser.detokenise(tokens)
 
     # Save sequence
-    Sequence.save = lambda *args: None
     detokenised_sequence.save("out/generated_sequence.mid")
 ```
```

### Comparing `scoda-2.1b2/scoda.egg-info/SOURCES.txt` & `scoda-2.1b4/scoda.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 scoda.egg-info/requires.txt
 scoda.egg-info/top_level.txt
 scoda/config/settings.json
 scoda/elements/bar.py
 scoda/elements/composition.py
 scoda/elements/message.py
 scoda/elements/track.py
+scoda/enumerations/message_type.py
+scoda/enumerations/tokenisation_flags.py
+scoda/enumerations/tokeniser_type.py
 scoda/exceptions/bar_exception.py
 scoda/exceptions/sequence_exception.py
 scoda/exceptions/tokenisation_exception.py
 scoda/exceptions/track_exception.py
 scoda/midi/midi_file.py
 scoda/midi/midi_message.py
 scoda/midi/midi_track.py
 scoda/misc/decorators.py
-scoda/misc/enumerations.py
 scoda/misc/music_theory.py
 scoda/misc/scoda_logging.py
 scoda/misc/util.py
 scoda/sequences/absolute_sequence.py
 scoda/sequences/abstract_sequence.py
 scoda/sequences/relative_sequence.py
 scoda/sequences/sequence.py
```

