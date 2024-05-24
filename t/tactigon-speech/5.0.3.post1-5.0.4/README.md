# Comparing `tmp/tactigon_speech-5.0.3.post1.tar.gz` & `tmp/tactigon_speech-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tactigon_speech-5.0.3.post1.tar", last modified: Wed Mar 27 16:09:29 2024, max compression
+gzip compressed data, was "tactigon_speech-5.0.4.tar", last modified: Fri May 24 11:02:51 2024, max compression
```

## Comparing `tactigon_speech-5.0.3.post1.tar` & `tactigon_speech-5.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 16:09:29.777384 tactigon_speech-5.0.3.post1/
--rw-rw-rw-   0        0        0        0 2023-08-28 15:35:20.000000 tactigon_speech-5.0.3.post1/LICENSE
--rw-rw-rw-   0        0        0       95 2023-11-22 17:33:33.000000 tactigon_speech-5.0.3.post1/MANIFEST.in
--rw-rw-rw-   0        0        0     2390 2024-03-27 16:09:29.776384 tactigon_speech-5.0.3.post1/PKG-INFO
--rw-rw-rw-   0        0        0     1667 2024-02-06 09:52:59.000000 tactigon_speech-5.0.3.post1/README.md
--rw-rw-rw-   0        0        0       92 2023-11-07 13:19:47.000000 tactigon_speech-5.0.3.post1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-27 16:09:29.778390 tactigon_speech-5.0.3.post1/setup.cfg
--rw-rw-rw-   0        0        0     2106 2024-03-27 15:47:18.000000 tactigon_speech-5.0.3.post1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-27 16:09:29.748384 tactigon_speech-5.0.3.post1/tactigon_speech/
--rw-rw-rw-   0        0        0     6337 2024-03-27 16:09:04.000000 tactigon_speech-5.0.3.post1/tactigon_speech/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 16:09:29.772389 tactigon_speech-5.0.3.post1/tactigon_speech/middleware/
--rw-rw-rw-   0        0        0   990256 2024-03-27 16:09:13.000000 tactigon_speech-5.0.3.post1/tactigon_speech/middleware/Tactigon_Speech.c
--rw-rw-rw-   0        0        0       89 2023-12-14 16:47:13.000000 tactigon_speech-5.0.3.post1/tactigon_speech/middleware/__init__.py
--rw-rw-rw-   0        0        0     5431 2024-03-27 13:20:32.000000 tactigon_speech-5.0.3.post1/tactigon_speech/models.py
-drwxrwxrwx   0        0        0        0 2024-03-27 16:09:29.775383 tactigon_speech-5.0.3.post1/tactigon_speech.egg-info/
--rw-rw-rw-   0        0        0     2390 2024-03-27 16:09:28.000000 tactigon_speech-5.0.3.post1/tactigon_speech.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2024-03-27 16:09:29.000000 tactigon_speech-5.0.3.post1/tactigon_speech.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 16:09:28.000000 tactigon_speech-5.0.3.post1/tactigon_speech.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-03-27 16:09:28.000000 tactigon_speech-5.0.3.post1/tactigon_speech.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-27 16:09:28.000000 tactigon_speech-5.0.3.post1/tactigon_speech.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 11:02:51.846262 tactigon_speech-5.0.4/
+-rw-rw-rw-   0        0        0        0 2023-08-28 15:35:20.000000 tactigon_speech-5.0.4/LICENSE
+-rw-rw-rw-   0        0        0       95 2023-11-22 17:33:33.000000 tactigon_speech-5.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2384 2024-05-24 11:02:51.846262 tactigon_speech-5.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1667 2024-02-06 09:52:59.000000 tactigon_speech-5.0.4/README.md
+-rw-rw-rw-   0        0        0       92 2023-11-07 13:19:47.000000 tactigon_speech-5.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 11:02:51.848273 tactigon_speech-5.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2106 2024-03-27 15:47:18.000000 tactigon_speech-5.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:02:51.804813 tactigon_speech-5.0.4/tactigon_speech/
+-rw-rw-rw-   0        0        0     6031 2024-05-24 09:26:16.000000 tactigon_speech-5.0.4/tactigon_speech/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:02:51.842263 tactigon_speech-5.0.4/tactigon_speech/middleware/
+-rw-rw-rw-   0        0        0  1001802 2024-05-24 11:02:29.000000 tactigon_speech-5.0.4/tactigon_speech/middleware/Tactigon_Speech.c
+-rw-rw-rw-   0        0        0       89 2023-12-14 16:47:13.000000 tactigon_speech-5.0.4/tactigon_speech/middleware/__init__.py
+-rw-rw-rw-   0        0        0     5541 2024-05-24 09:21:52.000000 tactigon_speech-5.0.4/tactigon_speech/models.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:02:51.845277 tactigon_speech-5.0.4/tactigon_speech.egg-info/
+-rw-rw-rw-   0        0        0     2384 2024-05-24 11:02:51.000000 tactigon_speech-5.0.4/tactigon_speech.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2024-05-24 11:02:51.000000 tactigon_speech-5.0.4/tactigon_speech.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 11:02:51.000000 tactigon_speech-5.0.4/tactigon_speech.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-05-24 11:02:51.000000 tactigon_speech-5.0.4/tactigon_speech.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-24 11:02:51.000000 tactigon_speech-5.0.4/tactigon_speech.egg-info/top_level.txt
```

### Comparing `tactigon_speech-5.0.3.post1/PKG-INFO` & `tactigon_speech-5.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tactigon_speech
-Version: 5.0.3.post1
+Version: 5.0.4
 Summary: Tactigon Speech to transcribe text into commands
 Home-page: https://nextind.eu
 Author: Next Industries s.r.l.
 Author-email: info@nextind.eu
 License: MIT
 Keywords: tactigon,wereable,voice recognition on edge,human interface
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tactigon_speech-5.0.3.post1/README.md` & `tactigon_speech-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tactigon_speech-5.0.3.post1/setup.py` & `tactigon_speech-5.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `tactigon_speech-5.0.3.post1/tactigon_speech/__init__.py` & `tactigon_speech-5.0.4/tactigon_speech/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-__version__ = "5.0.3.post1"
+__version__ = "5.0.4"
 
 __all__ = ['TSkin_Speech', 'TSkinConfig', 'AudioSource', 'HotWord', 'TSpeech', 'TSpeechObject', 'Command', 'VoiceConfig', 'Transcription',
            'Gesture', 'GestureConfig', 'Hand', 'Angle', 'Touch', 'OneFingerGesture', 'TwoFingerGesture', 'Gyro', 'Acceleration']
 
 import logging
 import time
 
 from threading import Thread, Event
 from typing import Optional
 from multiprocessing import Pipe
 from multiprocessing.connection import _ConnectionBase
 
 from tactigon_gear import TSkin, TSkinConfig, Gesture, GestureConfig, Hand, Angle, Touch, OneFingerGesture, TwoFingerGesture, Gyro, Acceleration
 from .middleware import Tactigon_Speech
-from .models import VoiceConfig, AudioSource, Command, HotWord, TSpeech, TSpeechObject, Transcription, TSkinState
+from .models import VoiceConfig, AudioSource, Command, HotWord, TSpeech, TSpeechObject, Transcription, TSkinState, InterfaceObject
 
 
 class TSkin_Speech(TSkin):
     _TICK: float = 0.02
     _audio_rx: _ConnectionBase
     source: AudioSource
 
@@ -37,50 +37,44 @@
         self._stop_interface = Event()
         self.interface = Thread(target=self.interface_thread)
 
     def interface_thread(self):
         logging.debug("Starting interface thread")
         while not self._stop_interface.is_set():
             if self.interface_pipe.poll():
-                data = self.interface_pipe.recv()
-                current_command = self.tactigon_speech.command
+                data: InterfaceObject = self.interface_pipe.recv()
+                current_command = data.command
 
-                if data is False:
+                if data.payload is False:
                     logging.error("Interface pipe: error for command %s", current_command)
-                    self.tactigon_speech.command = Command.STOP
                     self.select_sensors()
                     continue
 
                 if current_command is Command.RECORD:
-                    logging.debug("Got RECORD filename: %s", data)
-                    self.tactigon_speech.command = Command.NONE
+                    logging.debug("Got RECORD filename: %s", data.payload)
                     self.select_sensors()
                 elif current_command is Command.LISTEN:
-                    if isinstance(data, Transcription):
-                        logging.debug("Got LISTEN Transcription: %s", data)
-                        self._transcription = data
+                    if isinstance(data.payload, Transcription):
+                        logging.debug("Got LISTEN Transcription: %s", data.payload)
+                        self._transcription = data.payload
                         self.text_so_far = ""
-                        self.tactigon_speech.command = Command.NONE
                         self.select_sensors()
-                    elif isinstance(data, str):
+                    elif isinstance(data.payload, str):
                         logging.debug("Got LISTEN text_so_far: %s", data)
-                        self.text_so_far = data
+                        self.text_so_far = data.payload
                     else:
                         logging.error("Interface pipe: LISTEN error")
-                        self.tactigon_speech.command = Command.NONE
                         self.select_sensors()
                 elif current_command is Command.PLAY:
-                    if isinstance(data, str):
-                        logging.debug("Got PLAY filename: %s", data)
+                    if isinstance(data.payload, str):
+                        logging.debug("Got PLAY filename: %s", data.payload)
 
-                    self.tactigon_speech.command = Command.NONE
                     self.select_sensors()
                 elif current_command is Command.STOP:
-                    logging.debug("Got STOP: %s", data)
-                    self.tactigon_speech.command = Command.NONE
+                    logging.debug("Got STOP: %s", data.payload)
                     self.select_sensors()
             
             time.sleep(self._TICK)
 
     @property
     def initialized(self) -> bool:
         return self.tactigon_speech.initialized
@@ -140,31 +134,31 @@
 
     def listen(self, speech: TSpeechObject) -> bool:
         if self.tactigon_speech.command != Command.NONE:
             return False
         
         self.tactigon_speech.clear_audio_pipe()
         self.select_audio()
-        self.tactigon_speech.command = Command.LISTEN
         self.interface_pipe.send(speech)
+        self.tactigon_speech.command = Command.LISTEN
         return True
 
     def play(self, filename: str) -> bool:
         if self.tactigon_speech.command != Command.NONE:
             return False
         
-        self.tactigon_speech.command = Command.PLAY
         self.interface_pipe.send(filename)
+        self.tactigon_speech.command = Command.PLAY
         return True
 
     def record(self, filename: str) -> bool:
         if self.tactigon_speech.command != Command.NONE:
             return False
         
         self.tactigon_speech.clear_audio_pipe()
         self.select_audio()
-        self.tactigon_speech.command = Command.RECORD
         self.interface_pipe.send(filename)
+        self.tactigon_speech.command = Command.RECORD
         return True
 
     def stop(self):
         self.tactigon_speech.command = Command.STOP
```

### Comparing `tactigon_speech-5.0.3.post1/tactigon_speech/middleware/Tactigon_Speech.c` & `tactigon_speech-5.0.4/tactigon_speech/middleware/Tactigon_Speech.c`

 * *Files 1% similar despite different names*

```diff
@@ -1472,15 +1472,15 @@
 /* #### Code section: numeric_typedefs ### */
 /* #### Code section: complex_type_declarations ### */
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector;
 
-/* "tactigon_speech/middleware/Tactigon_Speech.py":116
+/* "tactigon_speech/middleware/Tactigon_Speech.py":115
  *         return (millis() - tick).total_seconds() > timeout
  * 
  *     def vad_collector(self) -> Generator[bytes, bytes, None]:             # <<<<<<<<<<<<<<
  *         frame_length = int(2 * self._SAMPLE_RATE * self.vad_frame / 1000)
  *         num_padding_frames: int = int(frame_length * (self.vad_padding_ms / 10000))
  */
 struct __pyx_obj_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector {
@@ -2603,15 +2603,14 @@
 static const char __pyx_k_getnchannels[] = "getnchannels";
 static const char __pyx_k_getsampwidth[] = "getsampwidth";
 static const char __pyx_k_initializing[] = "_initializing";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_is_listening[] = "is_listening";
 static const char __pyx_k_is_recording[] = "is_recording";
 static const char __pyx_k_is_timeout_2[] = "_is_timeout";
-static const char __pyx_k_last_command[] = "last_command";
 static const char __pyx_k_num_unvoiced[] = "num_unvoiced";
 static const char __pyx_k_setBeamWidth[] = "setBeamWidth";
 static const char __pyx_k_setframerate[] = "setframerate";
 static const char __pyx_k_setnchannels[] = "setnchannels";
 static const char __pyx_k_setsampwidth[] = "setsampwidth";
 static const char __pyx_k_stop_hotword[] = "stop_hotword";
 static const char __pyx_k_TSpeechObject[] = "TSpeechObject";
@@ -2626,22 +2625,23 @@
 static const char __pyx_k_vad_collector[] = "vad_collector";
 static const char __pyx_k_voice_timeout[] = "voice_timeout";
 static const char __pyx_k_ConnectionBase[] = "_ConnectionBase";
 static const char __pyx_k_Optional_float[] = "Optional[float]";
 static const char __pyx_k_current_branch[] = "current_branch";
 static const char __pyx_k_time_inference[] = "time_inference";
 static const char __pyx_k_vad_padding_ms[] = "vad_padding_ms";
+static const char __pyx_k_InterfaceObject[] = "InterfaceObject";
 static const char __pyx_k_NOT_INITIALIZED[] = "NOT_INITIALIZED";
 static const char __pyx_k_Tactigon_Speech[] = "Tactigon_Speech";
+static const char __pyx_k_current_command[] = "current_command";
 static const char __pyx_k_model_full_path[] = "model_full_path";
 static const char __pyx_k_multiprocessing[] = "multiprocessing";
 static const char __pyx_k_silence_timeout[] = "silence_timeout";
 static const char __pyx_k_Creating_PyAudio[] = "Creating PyAudio";
 static const char __pyx_k_Optional_HotWord[] = "Optional[HotWord]";
-static const char __pyx_k_SynchronizedBase[] = "SynchronizedBase";
 static const char __pyx_k_clear_audio_pipe[] = "clear_audio_pipe";
 static const char __pyx_k_deepspeech_Model[] = "deepspeech.Model";
 static const char __pyx_k_feedAudioContent[] = "feedAudioContent";
 static const char __pyx_k_scorer_full_path[] = "scorer_full_path";
 static const char __pyx_k_INTERFACE_TIMEOUT[] = "_INTERFACE_TIMEOUT";
 static const char __pyx_k_Model_initialized[] = "Model initialized";
 static const char __pyx_k_Setting_command_s[] = "Setting command %s";
@@ -2670,15 +2670,14 @@
 static const char __pyx_k_Tactigon_Speech_is_timeout[] = "Tactigon_Speech.is_timeout";
 static const char __pyx_k_multiprocessing_connection[] = "multiprocessing.connection";
 static const char __pyx_k_Tactigon_Speech_initialized[] = "Tactigon_Speech.initialized";
 static const char __pyx_k_multiprocessing_synchronize[] = "multiprocessing.synchronize";
 static const char __pyx_k_Tactigon_Speech_check_branch[] = "Tactigon_Speech.check_branch";
 static const char __pyx_k_Tactigon_Speech_is_listening[] = "Tactigon_Speech.is_listening";
 static const char __pyx_k_Tactigon_Speech_is_recording[] = "Tactigon_Speech.is_recording";
-static const char __pyx_k_multiprocessing_sharedctypes[] = "multiprocessing.sharedctypes";
 static const char __pyx_k_Tactigon_Speech_vad_collector[] = "Tactigon_Speech.vad_collector";
 static const char __pyx_k_TSpeech_Transcibed_text_s_Tree[] = "[TSpeech] Transcibed text: %s. Tree path: %s. Inference %f seconds";
 static const char __pyx_k_Clearing_audio_packet_from_pipe[] = "Clearing audio packet from pipe";
 static const char __pyx_k_Got_i_unvoiced_frames_Threshold[] = "Got %i unvoiced frames. Threshold is %f";
 static const char __pyx_k_TSpeech_Exception_while_listeni[] = "[TSpeech] Exception while listening. %s";
 static const char __pyx_k_TSpeech_Exception_while_playing[] = "[TSpeech] Exception while playing a file. %s";
 static const char __pyx_k_VAD_Frame_length_i_Frame_paddin[] = "[VAD] Frame length: %i, Frame paddings: %i, Voiced threshold: %f";
@@ -2758,14 +2757,15 @@
   PyObject *__pyx_kp_s_Generator_bytes_bytes_None;
   PyObject *__pyx_kp_s_Got_i_unvoiced_frames_Threshold;
   PyObject *__pyx_kp_s_Got_i_voiced_frames_Threshold_is;
   PyObject *__pyx_n_s_HotWord;
   PyObject *__pyx_n_s_INFO;
   PyObject *__pyx_n_s_INTERFACE_TIMEOUT;
   PyObject *__pyx_kp_s_Initializing_model;
+  PyObject *__pyx_n_s_InterfaceObject;
   PyObject *__pyx_n_s_Joined;
   PyObject *__pyx_n_s_LISTEN;
   PyObject *__pyx_n_s_List;
   PyObject *__pyx_kp_s_Listen_command_received_but_no_t;
   PyObject *__pyx_n_s_MIC;
   PyObject *__pyx_n_s_Model;
   PyObject *__pyx_kp_s_Model_initialized;
@@ -2785,15 +2785,14 @@
   PyObject *__pyx_kp_s_Running;
   PyObject *__pyx_n_s_SAMPLE_RATE;
   PyObject *__pyx_n_s_SINGLE_FRAME_LENGTH;
   PyObject *__pyx_n_s_STOP;
   PyObject *__pyx_kp_s_Setting_command_s;
   PyObject *__pyx_kp_s_Starting_Tactigon_Speech;
   PyObject *__pyx_n_s_Stopped;
-  PyObject *__pyx_n_s_SynchronizedBase;
   PyObject *__pyx_n_s_TICK;
   PyObject *__pyx_n_s_TSpeech;
   PyObject *__pyx_n_s_TSpeechObject;
   PyObject *__pyx_kp_s_TSpeech_Exception_while_listeni;
   PyObject *__pyx_kp_s_TSpeech_Exception_while_playing;
   PyObject *__pyx_kp_s_TSpeech_Transcibed_text_s_Tree;
   PyObject *__pyx_n_s_Tactigon_Speech;
@@ -2852,14 +2851,15 @@
   PyObject *__pyx_n_s_collections;
   PyObject *__pyx_n_s_command;
   PyObject *__pyx_n_s_command_2;
   PyObject *__pyx_n_s_config;
   PyObject *__pyx_n_s_createStream;
   PyObject *__pyx_n_s_ctypes;
   PyObject *__pyx_n_s_current_branch;
+  PyObject *__pyx_n_s_current_command;
   PyObject *__pyx_n_s_data;
   PyObject *__pyx_n_s_datetime;
   PyObject *__pyx_n_s_debug;
   PyObject *__pyx_n_s_deepspeech;
   PyObject *__pyx_kp_s_deepspeech_Model;
   PyObject *__pyx_n_s_delta;
   PyObject *__pyx_n_s_deque;
@@ -2911,15 +2911,14 @@
   PyObject *__pyx_n_s_is_recording;
   PyObject *__pyx_n_s_is_set;
   PyObject *__pyx_n_s_is_speech;
   PyObject *__pyx_n_s_is_timeout;
   PyObject *__pyx_n_s_is_timeout_2;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_n_s_join;
-  PyObject *__pyx_n_s_last_command;
   PyObject *__pyx_n_s_log_to_stderr;
   PyObject *__pyx_n_s_logger;
   PyObject *__pyx_n_s_logging;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_maxlen;
   PyObject *__pyx_n_s_metaclass;
   PyObject *__pyx_n_s_millis;
@@ -2927,15 +2926,14 @@
   PyObject *__pyx_n_s_model;
   PyObject *__pyx_n_s_model_full_path;
   PyObject *__pyx_n_s_models;
   PyObject *__pyx_n_s_module;
   PyObject *__pyx_n_s_mro_entries;
   PyObject *__pyx_n_s_multiprocessing;
   PyObject *__pyx_n_s_multiprocessing_connection;
-  PyObject *__pyx_n_s_multiprocessing_sharedctypes;
   PyObject *__pyx_n_s_multiprocessing_synchronize;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_name_2;
   PyObject *__pyx_n_s_now;
   PyObject *__pyx_n_s_np;
   PyObject *__pyx_n_s_num_padding_frames;
   PyObject *__pyx_n_s_num_unvoiced;
@@ -3126,14 +3124,15 @@
   Py_CLEAR(clear_module_state->__pyx_kp_s_Generator_bytes_bytes_None);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Got_i_unvoiced_frames_Threshold);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Got_i_voiced_frames_Threshold_is);
   Py_CLEAR(clear_module_state->__pyx_n_s_HotWord);
   Py_CLEAR(clear_module_state->__pyx_n_s_INFO);
   Py_CLEAR(clear_module_state->__pyx_n_s_INTERFACE_TIMEOUT);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Initializing_model);
+  Py_CLEAR(clear_module_state->__pyx_n_s_InterfaceObject);
   Py_CLEAR(clear_module_state->__pyx_n_s_Joined);
   Py_CLEAR(clear_module_state->__pyx_n_s_LISTEN);
   Py_CLEAR(clear_module_state->__pyx_n_s_List);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Listen_command_received_but_no_t);
   Py_CLEAR(clear_module_state->__pyx_n_s_MIC);
   Py_CLEAR(clear_module_state->__pyx_n_s_Model);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Model_initialized);
@@ -3153,15 +3152,14 @@
   Py_CLEAR(clear_module_state->__pyx_kp_s_Running);
   Py_CLEAR(clear_module_state->__pyx_n_s_SAMPLE_RATE);
   Py_CLEAR(clear_module_state->__pyx_n_s_SINGLE_FRAME_LENGTH);
   Py_CLEAR(clear_module_state->__pyx_n_s_STOP);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Setting_command_s);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Starting_Tactigon_Speech);
   Py_CLEAR(clear_module_state->__pyx_n_s_Stopped);
-  Py_CLEAR(clear_module_state->__pyx_n_s_SynchronizedBase);
   Py_CLEAR(clear_module_state->__pyx_n_s_TICK);
   Py_CLEAR(clear_module_state->__pyx_n_s_TSpeech);
   Py_CLEAR(clear_module_state->__pyx_n_s_TSpeechObject);
   Py_CLEAR(clear_module_state->__pyx_kp_s_TSpeech_Exception_while_listeni);
   Py_CLEAR(clear_module_state->__pyx_kp_s_TSpeech_Exception_while_playing);
   Py_CLEAR(clear_module_state->__pyx_kp_s_TSpeech_Transcibed_text_s_Tree);
   Py_CLEAR(clear_module_state->__pyx_n_s_Tactigon_Speech);
@@ -3220,14 +3218,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_collections);
   Py_CLEAR(clear_module_state->__pyx_n_s_command);
   Py_CLEAR(clear_module_state->__pyx_n_s_command_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_config);
   Py_CLEAR(clear_module_state->__pyx_n_s_createStream);
   Py_CLEAR(clear_module_state->__pyx_n_s_ctypes);
   Py_CLEAR(clear_module_state->__pyx_n_s_current_branch);
+  Py_CLEAR(clear_module_state->__pyx_n_s_current_command);
   Py_CLEAR(clear_module_state->__pyx_n_s_data);
   Py_CLEAR(clear_module_state->__pyx_n_s_datetime);
   Py_CLEAR(clear_module_state->__pyx_n_s_debug);
   Py_CLEAR(clear_module_state->__pyx_n_s_deepspeech);
   Py_CLEAR(clear_module_state->__pyx_kp_s_deepspeech_Model);
   Py_CLEAR(clear_module_state->__pyx_n_s_delta);
   Py_CLEAR(clear_module_state->__pyx_n_s_deque);
@@ -3279,15 +3278,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_is_recording);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_set);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_speech);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_timeout);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_timeout_2);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_n_s_join);
-  Py_CLEAR(clear_module_state->__pyx_n_s_last_command);
   Py_CLEAR(clear_module_state->__pyx_n_s_log_to_stderr);
   Py_CLEAR(clear_module_state->__pyx_n_s_logger);
   Py_CLEAR(clear_module_state->__pyx_n_s_logging);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_maxlen);
   Py_CLEAR(clear_module_state->__pyx_n_s_metaclass);
   Py_CLEAR(clear_module_state->__pyx_n_s_millis);
@@ -3295,15 +3293,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_model);
   Py_CLEAR(clear_module_state->__pyx_n_s_model_full_path);
   Py_CLEAR(clear_module_state->__pyx_n_s_models);
   Py_CLEAR(clear_module_state->__pyx_n_s_module);
   Py_CLEAR(clear_module_state->__pyx_n_s_mro_entries);
   Py_CLEAR(clear_module_state->__pyx_n_s_multiprocessing);
   Py_CLEAR(clear_module_state->__pyx_n_s_multiprocessing_connection);
-  Py_CLEAR(clear_module_state->__pyx_n_s_multiprocessing_sharedctypes);
   Py_CLEAR(clear_module_state->__pyx_n_s_multiprocessing_synchronize);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_name_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_now);
   Py_CLEAR(clear_module_state->__pyx_n_s_np);
   Py_CLEAR(clear_module_state->__pyx_n_s_num_padding_frames);
   Py_CLEAR(clear_module_state->__pyx_n_s_num_unvoiced);
@@ -3472,14 +3469,15 @@
   Py_VISIT(traverse_module_state->__pyx_kp_s_Generator_bytes_bytes_None);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Got_i_unvoiced_frames_Threshold);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Got_i_voiced_frames_Threshold_is);
   Py_VISIT(traverse_module_state->__pyx_n_s_HotWord);
   Py_VISIT(traverse_module_state->__pyx_n_s_INFO);
   Py_VISIT(traverse_module_state->__pyx_n_s_INTERFACE_TIMEOUT);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Initializing_model);
+  Py_VISIT(traverse_module_state->__pyx_n_s_InterfaceObject);
   Py_VISIT(traverse_module_state->__pyx_n_s_Joined);
   Py_VISIT(traverse_module_state->__pyx_n_s_LISTEN);
   Py_VISIT(traverse_module_state->__pyx_n_s_List);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Listen_command_received_but_no_t);
   Py_VISIT(traverse_module_state->__pyx_n_s_MIC);
   Py_VISIT(traverse_module_state->__pyx_n_s_Model);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Model_initialized);
@@ -3499,15 +3497,14 @@
   Py_VISIT(traverse_module_state->__pyx_kp_s_Running);
   Py_VISIT(traverse_module_state->__pyx_n_s_SAMPLE_RATE);
   Py_VISIT(traverse_module_state->__pyx_n_s_SINGLE_FRAME_LENGTH);
   Py_VISIT(traverse_module_state->__pyx_n_s_STOP);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Setting_command_s);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Starting_Tactigon_Speech);
   Py_VISIT(traverse_module_state->__pyx_n_s_Stopped);
-  Py_VISIT(traverse_module_state->__pyx_n_s_SynchronizedBase);
   Py_VISIT(traverse_module_state->__pyx_n_s_TICK);
   Py_VISIT(traverse_module_state->__pyx_n_s_TSpeech);
   Py_VISIT(traverse_module_state->__pyx_n_s_TSpeechObject);
   Py_VISIT(traverse_module_state->__pyx_kp_s_TSpeech_Exception_while_listeni);
   Py_VISIT(traverse_module_state->__pyx_kp_s_TSpeech_Exception_while_playing);
   Py_VISIT(traverse_module_state->__pyx_kp_s_TSpeech_Transcibed_text_s_Tree);
   Py_VISIT(traverse_module_state->__pyx_n_s_Tactigon_Speech);
@@ -3566,14 +3563,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_collections);
   Py_VISIT(traverse_module_state->__pyx_n_s_command);
   Py_VISIT(traverse_module_state->__pyx_n_s_command_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_config);
   Py_VISIT(traverse_module_state->__pyx_n_s_createStream);
   Py_VISIT(traverse_module_state->__pyx_n_s_ctypes);
   Py_VISIT(traverse_module_state->__pyx_n_s_current_branch);
+  Py_VISIT(traverse_module_state->__pyx_n_s_current_command);
   Py_VISIT(traverse_module_state->__pyx_n_s_data);
   Py_VISIT(traverse_module_state->__pyx_n_s_datetime);
   Py_VISIT(traverse_module_state->__pyx_n_s_debug);
   Py_VISIT(traverse_module_state->__pyx_n_s_deepspeech);
   Py_VISIT(traverse_module_state->__pyx_kp_s_deepspeech_Model);
   Py_VISIT(traverse_module_state->__pyx_n_s_delta);
   Py_VISIT(traverse_module_state->__pyx_n_s_deque);
@@ -3625,15 +3623,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_is_recording);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_set);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_speech);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_timeout);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_timeout_2);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_n_s_join);
-  Py_VISIT(traverse_module_state->__pyx_n_s_last_command);
   Py_VISIT(traverse_module_state->__pyx_n_s_log_to_stderr);
   Py_VISIT(traverse_module_state->__pyx_n_s_logger);
   Py_VISIT(traverse_module_state->__pyx_n_s_logging);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_maxlen);
   Py_VISIT(traverse_module_state->__pyx_n_s_metaclass);
   Py_VISIT(traverse_module_state->__pyx_n_s_millis);
@@ -3641,15 +3638,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_model);
   Py_VISIT(traverse_module_state->__pyx_n_s_model_full_path);
   Py_VISIT(traverse_module_state->__pyx_n_s_models);
   Py_VISIT(traverse_module_state->__pyx_n_s_module);
   Py_VISIT(traverse_module_state->__pyx_n_s_mro_entries);
   Py_VISIT(traverse_module_state->__pyx_n_s_multiprocessing);
   Py_VISIT(traverse_module_state->__pyx_n_s_multiprocessing_connection);
-  Py_VISIT(traverse_module_state->__pyx_n_s_multiprocessing_sharedctypes);
   Py_VISIT(traverse_module_state->__pyx_n_s_multiprocessing_synchronize);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_name_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_now);
   Py_VISIT(traverse_module_state->__pyx_n_s_np);
   Py_VISIT(traverse_module_state->__pyx_n_s_num_padding_frames);
   Py_VISIT(traverse_module_state->__pyx_n_s_num_unvoiced);
@@ -3828,14 +3824,15 @@
 #define __pyx_kp_s_Generator_bytes_bytes_None __pyx_mstate_global->__pyx_kp_s_Generator_bytes_bytes_None
 #define __pyx_kp_s_Got_i_unvoiced_frames_Threshold __pyx_mstate_global->__pyx_kp_s_Got_i_unvoiced_frames_Threshold
 #define __pyx_kp_s_Got_i_voiced_frames_Threshold_is __pyx_mstate_global->__pyx_kp_s_Got_i_voiced_frames_Threshold_is
 #define __pyx_n_s_HotWord __pyx_mstate_global->__pyx_n_s_HotWord
 #define __pyx_n_s_INFO __pyx_mstate_global->__pyx_n_s_INFO
 #define __pyx_n_s_INTERFACE_TIMEOUT __pyx_mstate_global->__pyx_n_s_INTERFACE_TIMEOUT
 #define __pyx_kp_s_Initializing_model __pyx_mstate_global->__pyx_kp_s_Initializing_model
+#define __pyx_n_s_InterfaceObject __pyx_mstate_global->__pyx_n_s_InterfaceObject
 #define __pyx_n_s_Joined __pyx_mstate_global->__pyx_n_s_Joined
 #define __pyx_n_s_LISTEN __pyx_mstate_global->__pyx_n_s_LISTEN
 #define __pyx_n_s_List __pyx_mstate_global->__pyx_n_s_List
 #define __pyx_kp_s_Listen_command_received_but_no_t __pyx_mstate_global->__pyx_kp_s_Listen_command_received_but_no_t
 #define __pyx_n_s_MIC __pyx_mstate_global->__pyx_n_s_MIC
 #define __pyx_n_s_Model __pyx_mstate_global->__pyx_n_s_Model
 #define __pyx_kp_s_Model_initialized __pyx_mstate_global->__pyx_kp_s_Model_initialized
@@ -3855,15 +3852,14 @@
 #define __pyx_kp_s_Running __pyx_mstate_global->__pyx_kp_s_Running
 #define __pyx_n_s_SAMPLE_RATE __pyx_mstate_global->__pyx_n_s_SAMPLE_RATE
 #define __pyx_n_s_SINGLE_FRAME_LENGTH __pyx_mstate_global->__pyx_n_s_SINGLE_FRAME_LENGTH
 #define __pyx_n_s_STOP __pyx_mstate_global->__pyx_n_s_STOP
 #define __pyx_kp_s_Setting_command_s __pyx_mstate_global->__pyx_kp_s_Setting_command_s
 #define __pyx_kp_s_Starting_Tactigon_Speech __pyx_mstate_global->__pyx_kp_s_Starting_Tactigon_Speech
 #define __pyx_n_s_Stopped __pyx_mstate_global->__pyx_n_s_Stopped
-#define __pyx_n_s_SynchronizedBase __pyx_mstate_global->__pyx_n_s_SynchronizedBase
 #define __pyx_n_s_TICK __pyx_mstate_global->__pyx_n_s_TICK
 #define __pyx_n_s_TSpeech __pyx_mstate_global->__pyx_n_s_TSpeech
 #define __pyx_n_s_TSpeechObject __pyx_mstate_global->__pyx_n_s_TSpeechObject
 #define __pyx_kp_s_TSpeech_Exception_while_listeni __pyx_mstate_global->__pyx_kp_s_TSpeech_Exception_while_listeni
 #define __pyx_kp_s_TSpeech_Exception_while_playing __pyx_mstate_global->__pyx_kp_s_TSpeech_Exception_while_playing
 #define __pyx_kp_s_TSpeech_Transcibed_text_s_Tree __pyx_mstate_global->__pyx_kp_s_TSpeech_Transcibed_text_s_Tree
 #define __pyx_n_s_Tactigon_Speech __pyx_mstate_global->__pyx_n_s_Tactigon_Speech
@@ -3922,14 +3918,15 @@
 #define __pyx_n_s_collections __pyx_mstate_global->__pyx_n_s_collections
 #define __pyx_n_s_command __pyx_mstate_global->__pyx_n_s_command
 #define __pyx_n_s_command_2 __pyx_mstate_global->__pyx_n_s_command_2
 #define __pyx_n_s_config __pyx_mstate_global->__pyx_n_s_config
 #define __pyx_n_s_createStream __pyx_mstate_global->__pyx_n_s_createStream
 #define __pyx_n_s_ctypes __pyx_mstate_global->__pyx_n_s_ctypes
 #define __pyx_n_s_current_branch __pyx_mstate_global->__pyx_n_s_current_branch
+#define __pyx_n_s_current_command __pyx_mstate_global->__pyx_n_s_current_command
 #define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
 #define __pyx_n_s_datetime __pyx_mstate_global->__pyx_n_s_datetime
 #define __pyx_n_s_debug __pyx_mstate_global->__pyx_n_s_debug
 #define __pyx_n_s_deepspeech __pyx_mstate_global->__pyx_n_s_deepspeech
 #define __pyx_kp_s_deepspeech_Model __pyx_mstate_global->__pyx_kp_s_deepspeech_Model
 #define __pyx_n_s_delta __pyx_mstate_global->__pyx_n_s_delta
 #define __pyx_n_s_deque __pyx_mstate_global->__pyx_n_s_deque
@@ -3981,15 +3978,14 @@
 #define __pyx_n_s_is_recording __pyx_mstate_global->__pyx_n_s_is_recording
 #define __pyx_n_s_is_set __pyx_mstate_global->__pyx_n_s_is_set
 #define __pyx_n_s_is_speech __pyx_mstate_global->__pyx_n_s_is_speech
 #define __pyx_n_s_is_timeout __pyx_mstate_global->__pyx_n_s_is_timeout
 #define __pyx_n_s_is_timeout_2 __pyx_mstate_global->__pyx_n_s_is_timeout_2
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_n_s_join __pyx_mstate_global->__pyx_n_s_join
-#define __pyx_n_s_last_command __pyx_mstate_global->__pyx_n_s_last_command
 #define __pyx_n_s_log_to_stderr __pyx_mstate_global->__pyx_n_s_log_to_stderr
 #define __pyx_n_s_logger __pyx_mstate_global->__pyx_n_s_logger
 #define __pyx_n_s_logging __pyx_mstate_global->__pyx_n_s_logging
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_maxlen __pyx_mstate_global->__pyx_n_s_maxlen
 #define __pyx_n_s_metaclass __pyx_mstate_global->__pyx_n_s_metaclass
 #define __pyx_n_s_millis __pyx_mstate_global->__pyx_n_s_millis
@@ -3997,15 +3993,14 @@
 #define __pyx_n_s_model __pyx_mstate_global->__pyx_n_s_model
 #define __pyx_n_s_model_full_path __pyx_mstate_global->__pyx_n_s_model_full_path
 #define __pyx_n_s_models __pyx_mstate_global->__pyx_n_s_models
 #define __pyx_n_s_module __pyx_mstate_global->__pyx_n_s_module
 #define __pyx_n_s_mro_entries __pyx_mstate_global->__pyx_n_s_mro_entries
 #define __pyx_n_s_multiprocessing __pyx_mstate_global->__pyx_n_s_multiprocessing
 #define __pyx_n_s_multiprocessing_connection __pyx_mstate_global->__pyx_n_s_multiprocessing_connection
-#define __pyx_n_s_multiprocessing_sharedctypes __pyx_mstate_global->__pyx_n_s_multiprocessing_sharedctypes
 #define __pyx_n_s_multiprocessing_synchronize __pyx_mstate_global->__pyx_n_s_multiprocessing_synchronize
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_name_2 __pyx_mstate_global->__pyx_n_s_name_2
 #define __pyx_n_s_now __pyx_mstate_global->__pyx_n_s_now
 #define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
 #define __pyx_n_s_num_padding_frames __pyx_mstate_global->__pyx_n_s_num_padding_frames
 #define __pyx_n_s_num_unvoiced __pyx_mstate_global->__pyx_n_s_num_unvoiced
@@ -4134,15 +4129,15 @@
 #define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
 #define __pyx_codeobj__31 __pyx_mstate_global->__pyx_codeobj__31
 #define __pyx_codeobj__33 __pyx_mstate_global->__pyx_codeobj__33
 #define __pyx_codeobj__35 __pyx_mstate_global->__pyx_codeobj__35
 #define __pyx_codeobj__38 __pyx_mstate_global->__pyx_codeobj__38
 /* #### Code section: module_code ### */
 
-/* "tactigon_speech/middleware/Tactigon_Speech.py":23
+/* "tactigon_speech/middleware/Tactigon_Speech.py":22
  * # from tactigon_gear.middleware import Tactigon_Audio
  * 
  * def millis():             # <<<<<<<<<<<<<<
  *     return datetime.now()
  * 
  */
 
@@ -4170,25 +4165,25 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("millis", 1);
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":24
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":23
  * 
  * def millis():
  *     return datetime.now()             # <<<<<<<<<<<<<<
  * 
  * class Tactigon_Speech(Process):
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_datetime); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_datetime); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_now); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_now); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -4201,23 +4196,23 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":23
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":22
  * # from tactigon_gear.middleware import Tactigon_Audio
  * 
  * def millis():             # <<<<<<<<<<<<<<
  *     return datetime.now()
  * 
  */
 
@@ -4230,15 +4225,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tactigon_speech/middleware/Tactigon_Speech.py":54
+/* "tactigon_speech/middleware/Tactigon_Speech.py":53
  *     stop_hotword: Optional[HotWord]
  * 
  *     def __init__(self, config: VoiceConfig, audio_source: AudioSource, audio: _ConnectionBase, interface: _ConnectionBase, debug: bool = False):             # <<<<<<<<<<<<<<
  *         Process.__init__(self)
  * 
  */
 
@@ -4307,67 +4302,67 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 54, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_config)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 54, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 5, 6, 1); __PYX_ERR(0, 54, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 5, 6, 1); __PYX_ERR(0, 53, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_audio_source)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 54, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 5, 6, 2); __PYX_ERR(0, 54, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 5, 6, 2); __PYX_ERR(0, 53, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_audio)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 54, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 5, 6, 3); __PYX_ERR(0, 54, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 5, 6, 3); __PYX_ERR(0, 53, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_interface)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 54, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 5, 6, 4); __PYX_ERR(0, 54, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 5, 6, 4); __PYX_ERR(0, 53, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_debug);
           if (value) { values[5] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 54, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 54, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 53, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
@@ -4383,15 +4378,15 @@
     __pyx_v_audio_source = values[2];
     __pyx_v_audio = values[3];
     __pyx_v_interface = values[4];
     __pyx_v_debug = values[5];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 5, 6, __pyx_nargs); __PYX_ERR(0, 54, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 5, 6, __pyx_nargs); __PYX_ERR(0, 53, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -4424,24 +4419,24 @@
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":55
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":54
  * 
  *     def __init__(self, config: VoiceConfig, audio_source: AudioSource, audio: _ConnectionBase, interface: _ConnectionBase, debug: bool = False):
  *         Process.__init__(self)             # <<<<<<<<<<<<<<
  * 
  *         self.logger = log_to_stderr()
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Process); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Process); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_init); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_init); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -4454,28 +4449,28 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_self};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":57
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":56
  *         Process.__init__(self)
  * 
  *         self.logger = log_to_stderr()             # <<<<<<<<<<<<<<
  *         if debug:
  *             self.logger.setLevel(logging.DEBUG)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_log_to_stderr); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_log_to_stderr); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -4487,46 +4482,46 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_logger, __pyx_t_1) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_logger, __pyx_t_1) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":58
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":57
  * 
  *         self.logger = log_to_stderr()
  *         if debug:             # <<<<<<<<<<<<<<
  *             self.logger.setLevel(logging.DEBUG)
  *         else:
  */
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_debug); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_debug); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 57, __pyx_L1_error)
   if (__pyx_t_5) {
 
-    /* "tactigon_speech/middleware/Tactigon_Speech.py":59
+    /* "tactigon_speech/middleware/Tactigon_Speech.py":58
  *         self.logger = log_to_stderr()
  *         if debug:
  *             self.logger.setLevel(logging.DEBUG)             # <<<<<<<<<<<<<<
  *         else:
  *             self.logger.setLevel(logging.INFO)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_setLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_setLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 58, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -4540,46 +4535,46 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_6};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "tactigon_speech/middleware/Tactigon_Speech.py":58
+    /* "tactigon_speech/middleware/Tactigon_Speech.py":57
  * 
  *         self.logger = log_to_stderr()
  *         if debug:             # <<<<<<<<<<<<<<
  *             self.logger.setLevel(logging.DEBUG)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":61
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":60
  *             self.logger.setLevel(logging.DEBUG)
  *         else:
  *             self.logger.setLevel(logging.INFO)             # <<<<<<<<<<<<<<
  * 
  *         self.logger.debug("Starting Tactigon Speech")
  */
   /*else*/ {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 61, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_setLevel); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 61, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_setLevel); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 61, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_INFO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 61, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_INFO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_6);
@@ -4593,32 +4588,32 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_3};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L3:;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":63
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":62
  *             self.logger.setLevel(logging.INFO)
  * 
  *         self.logger.debug("Starting Tactigon Speech")             # <<<<<<<<<<<<<<
  * 
  *         # self.config = config
  */
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
@@ -4631,28 +4626,28 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_kp_s_Starting_Tactigon_Speech};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":66
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":65
  * 
  *         # self.config = config
  *         self._stop_event = Event()             # <<<<<<<<<<<<<<
  *         self.audio = audio
  *         self.interface = interface
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Event); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Event); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_6 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
@@ -4664,51 +4659,51 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_stop_event, __pyx_t_1) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_stop_event, __pyx_t_1) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":67
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":66
  *         # self.config = config
  *         self._stop_event = Event()
  *         self.audio = audio             # <<<<<<<<<<<<<<
  *         self.interface = interface
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_audio, __pyx_v_audio) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_audio, __pyx_v_audio) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":68
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":67
  *         self._stop_event = Event()
  *         self.audio = audio
  *         self.interface = interface             # <<<<<<<<<<<<<<
  * 
  *         self._command = Value(ctypes.c_int)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_interface, __pyx_v_interface) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_interface, __pyx_v_interface) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":70
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":69
  *         self.interface = interface
  * 
  *         self._command = Value(ctypes.c_int)             # <<<<<<<<<<<<<<
  *         self.command = Command.NOT_INITIALIZED
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_c_int); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_c_int); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
@@ -4722,166 +4717,166 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_2};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_command, __pyx_t_1) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_command, __pyx_t_1) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":71
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":70
  * 
  *         self._command = Value(ctypes.c_int)
  *         self.command = Command.NOT_INITIALIZED             # <<<<<<<<<<<<<<
  * 
  *         self.audio_source = audio_source
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Command); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Command); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_NOT_INITIALIZED); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_NOT_INITIALIZED); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_command_2, __pyx_t_3) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_command_2, __pyx_t_3) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":73
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":72
  *         self.command = Command.NOT_INITIALIZED
  * 
  *         self.audio_source = audio_source             # <<<<<<<<<<<<<<
  *         self.vad_frame = config.vad_frame
  *         self.vad_padding_ms = config.vad_padding_ms
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_audio_source, __pyx_v_audio_source) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_audio_source, __pyx_v_audio_source) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":74
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":73
  * 
  *         self.audio_source = audio_source
  *         self.vad_frame = config.vad_frame             # <<<<<<<<<<<<<<
  *         self.vad_padding_ms = config.vad_padding_ms
  *         self.vad_ratio = config.vad_ratio
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_vad_frame); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_vad_frame); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_vad_frame, __pyx_t_3) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_vad_frame, __pyx_t_3) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":75
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":74
  *         self.audio_source = audio_source
  *         self.vad_frame = config.vad_frame
  *         self.vad_padding_ms = config.vad_padding_ms             # <<<<<<<<<<<<<<
  *         self.vad_ratio = config.vad_ratio
  *         self.silence_timeout = config.silence_timeout
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_vad_padding_ms); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_vad_padding_ms); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_vad_padding_ms, __pyx_t_3) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_vad_padding_ms, __pyx_t_3) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":76
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":75
  *         self.vad_frame = config.vad_frame
  *         self.vad_padding_ms = config.vad_padding_ms
  *         self.vad_ratio = config.vad_ratio             # <<<<<<<<<<<<<<
  *         self.silence_timeout = config.silence_timeout
  *         self.voice_timeout = config.voice_timeout
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_vad_ratio); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_vad_ratio); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_vad_ratio, __pyx_t_3) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_vad_ratio, __pyx_t_3) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":77
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":76
  *         self.vad_padding_ms = config.vad_padding_ms
  *         self.vad_ratio = config.vad_ratio
  *         self.silence_timeout = config.silence_timeout             # <<<<<<<<<<<<<<
  *         self.voice_timeout = config.voice_timeout
  *         self.vad_aggressiveness = config.vad_aggressiveness
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_silence_timeout); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_silence_timeout); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_silence_timeout, __pyx_t_3) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_silence_timeout, __pyx_t_3) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":78
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":77
  *         self.vad_ratio = config.vad_ratio
  *         self.silence_timeout = config.silence_timeout
  *         self.voice_timeout = config.voice_timeout             # <<<<<<<<<<<<<<
  *         self.vad_aggressiveness = config.vad_aggressiveness
  *         self.model_full_path = config.model_full_path
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_voice_timeout); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_voice_timeout); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_voice_timeout, __pyx_t_3) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_voice_timeout, __pyx_t_3) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":79
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":78
  *         self.silence_timeout = config.silence_timeout
  *         self.voice_timeout = config.voice_timeout
  *         self.vad_aggressiveness = config.vad_aggressiveness             # <<<<<<<<<<<<<<
  *         self.model_full_path = config.model_full_path
  *         self.scorer_full_path = config.scorer_full_path
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_vad_aggressiveness); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_vad_aggressiveness); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_vad_aggressiveness, __pyx_t_3) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_vad_aggressiveness, __pyx_t_3) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":80
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":79
  *         self.voice_timeout = config.voice_timeout
  *         self.vad_aggressiveness = config.vad_aggressiveness
  *         self.model_full_path = config.model_full_path             # <<<<<<<<<<<<<<
  *         self.scorer_full_path = config.scorer_full_path
  *         self.beam_width = config.beam_width
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_model_full_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_model_full_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_model_full_path, __pyx_t_3) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_model_full_path, __pyx_t_3) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":81
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":80
  *         self.vad_aggressiveness = config.vad_aggressiveness
  *         self.model_full_path = config.model_full_path
  *         self.scorer_full_path = config.scorer_full_path             # <<<<<<<<<<<<<<
  *         self.beam_width = config.beam_width
  *         self.stop_hotword = config.stop_hotword
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_scorer_full_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_scorer_full_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_scorer_full_path, __pyx_t_3) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_scorer_full_path, __pyx_t_3) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":82
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":81
  *         self.model_full_path = config.model_full_path
  *         self.scorer_full_path = config.scorer_full_path
  *         self.beam_width = config.beam_width             # <<<<<<<<<<<<<<
  *         self.stop_hotword = config.stop_hotword
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_beam_width); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_beam_width); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_beam_width, __pyx_t_3) < 0) __PYX_ERR(0, 82, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_beam_width, __pyx_t_3) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":83
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":82
  *         self.scorer_full_path = config.scorer_full_path
  *         self.beam_width = config.beam_width
  *         self.stop_hotword = config.stop_hotword             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_stop_hotword); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_config, __pyx_n_s_stop_hotword); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_stop_hotword, __pyx_t_3) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_stop_hotword, __pyx_t_3) < 0) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":54
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":53
  *     stop_hotword: Optional[HotWord]
  * 
  *     def __init__(self, config: VoiceConfig, audio_source: AudioSource, audio: _ConnectionBase, interface: _ConnectionBase, debug: bool = False):             # <<<<<<<<<<<<<<
  *         Process.__init__(self)
  * 
  */
 
@@ -4897,15 +4892,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tactigon_speech/middleware/Tactigon_Speech.py":85
+/* "tactigon_speech/middleware/Tactigon_Speech.py":84
  *         self.stop_hotword = config.stop_hotword
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def command(self) -> Command:
  *         with self._command.get_lock():
  */
 
@@ -4958,31 +4953,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 85, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 84, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "command") < 0)) __PYX_ERR(0, 85, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "command") < 0)) __PYX_ERR(0, 84, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("command", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 85, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("command", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 84, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -5023,25 +5018,25 @@
   int __pyx_t_12;
   int __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("command", 1);
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":87
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":86
  *     @property
  *     def command(self) -> Command:
  *         with self._command.get_lock():             # <<<<<<<<<<<<<<
  *             command = Command(self._command.get_obj().value)
  *             return command
  */
   /*with:*/ {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get_lock); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get_lock); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -5054,21 +5049,21 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __pyx_t_5 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_2 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L3_error)
+    __pyx_t_2 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_6 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_6)) {
@@ -5080,15 +5075,15 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, NULL};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L3_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     /*try:*/ {
       {
@@ -5096,26 +5091,26 @@
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_9);
         /*try:*/ {
 
-          /* "tactigon_speech/middleware/Tactigon_Speech.py":88
+          /* "tactigon_speech/middleware/Tactigon_Speech.py":87
  *     def command(self) -> Command:
  *         with self._command.get_lock():
  *             command = Command(self._command.get_obj().value)             # <<<<<<<<<<<<<<
  *             return command
  * 
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Command); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L7_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Command); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 88, __pyx_L7_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 87, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_get_obj); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 88, __pyx_L7_error)
+          __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_get_obj); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 87, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_10);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_6 = NULL;
           __pyx_t_4 = 0;
           #if CYTHON_UNPACK_METHODS
           if (likely(PyMethod_Check(__pyx_t_10))) {
             __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_10);
@@ -5128,19 +5123,19 @@
             }
           }
           #endif
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_6, NULL};
             __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
             __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-            if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L7_error)
+            if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_2);
             __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
           }
-          __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_value); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 88, __pyx_L7_error)
+          __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_value); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 87, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_10);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __pyx_t_2 = NULL;
           __pyx_t_4 = 0;
           #if CYTHON_UNPACK_METHODS
           if (unlikely(PyMethod_Check(__pyx_t_3))) {
             __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -5154,34 +5149,34 @@
           }
           #endif
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_10};
             __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
             __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L7_error)
+            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           }
           __pyx_v_command = __pyx_t_1;
           __pyx_t_1 = 0;
 
-          /* "tactigon_speech/middleware/Tactigon_Speech.py":89
+          /* "tactigon_speech/middleware/Tactigon_Speech.py":88
  *         with self._command.get_lock():
  *             command = Command(self._command.get_obj().value)
  *             return command             # <<<<<<<<<<<<<<
  * 
  *     @command.setter
  */
           __Pyx_XDECREF(__pyx_r);
           __Pyx_INCREF(__pyx_v_command);
           __pyx_r = __pyx_v_command;
           goto __pyx_L11_try_return;
 
-          /* "tactigon_speech/middleware/Tactigon_Speech.py":87
+          /* "tactigon_speech/middleware/Tactigon_Speech.py":86
  *     @property
  *     def command(self) -> Command:
  *         with self._command.get_lock():             # <<<<<<<<<<<<<<
  *             command = Command(self._command.get_obj().value)
  *             return command
  */
         }
@@ -5189,36 +5184,36 @@
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("tactigon_speech.middleware.Tactigon_Speech.Tactigon_Speech.command", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_3, &__pyx_t_10) < 0) __PYX_ERR(0, 87, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_3, &__pyx_t_10) < 0) __PYX_ERR(0, 86, __pyx_L9_except_error)
           __Pyx_XGOTREF(__pyx_t_1);
           __Pyx_XGOTREF(__pyx_t_3);
           __Pyx_XGOTREF(__pyx_t_10);
-          __pyx_t_2 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_3, __pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L9_except_error)
+          __pyx_t_2 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_3, __pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_2);
           __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, NULL);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 87, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 86, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_11);
           __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_11);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (__pyx_t_12 < 0) __PYX_ERR(0, 87, __pyx_L9_except_error)
+          if (__pyx_t_12 < 0) __PYX_ERR(0, 86, __pyx_L9_except_error)
           __pyx_t_13 = (!__pyx_t_12);
           if (unlikely(__pyx_t_13)) {
             __Pyx_GIVEREF(__pyx_t_1);
             __Pyx_GIVEREF(__pyx_t_3);
             __Pyx_XGIVEREF(__pyx_t_10);
             __Pyx_ErrRestoreWithState(__pyx_t_1, __pyx_t_3, __pyx_t_10);
             __pyx_t_1 = 0; __pyx_t_3 = 0; __pyx_t_10 = 0; 
-            __PYX_ERR(0, 87, __pyx_L9_except_error)
+            __PYX_ERR(0, 86, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -5241,27 +5236,27 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_5) {
           __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple_, NULL);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 87, __pyx_L1_error)
+          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 86, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L4_return: {
         __pyx_t_9 = __pyx_r;
         __pyx_r = 0;
         if (__pyx_t_5) {
           __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple_, NULL);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 87, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 86, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __pyx_r = __pyx_t_9;
         __pyx_t_9 = 0;
         goto __pyx_L0;
       }
@@ -5270,15 +5265,15 @@
     goto __pyx_L16;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L1_error;
     __pyx_L16:;
   }
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":85
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":84
  *         self.stop_hotword = config.stop_hotword
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def command(self) -> Command:
  *         with self._command.get_lock():
  */
 
@@ -5296,15 +5291,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_command);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tactigon_speech/middleware/Tactigon_Speech.py":91
+/* "tactigon_speech/middleware/Tactigon_Speech.py":90
  *             return command
  * 
  *     @command.setter             # <<<<<<<<<<<<<<
  *     def command(self, command: Command):
  *         self.logger.debug("Setting command %s", command.name)
  */
 
@@ -5360,43 +5355,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 91, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 90, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_command_2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 91, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 90, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("command", 1, 2, 2, 1); __PYX_ERR(0, 91, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("command", 1, 2, 2, 1); __PYX_ERR(0, 90, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "command") < 0)) __PYX_ERR(0, 91, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "command") < 0)) __PYX_ERR(0, 90, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_command = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("command", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 91, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("command", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 90, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -5435,27 +5430,27 @@
   int __pyx_t_11;
   int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("command", 1);
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":93
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":92
  *     @command.setter
  *     def command(self, command: Command):
  *         self.logger.debug("Setting command %s", command.name)             # <<<<<<<<<<<<<<
  *         with self._command.get_lock():
- *             self._command.get_obj().value = command.value
+ *             self._command.get_obj().value = command.value #type: ignore
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_command, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_command, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -5468,31 +5463,31 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_kp_s_Setting_command_s, __pyx_t_2};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":94
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":93
  *     def command(self, command: Command):
  *         self.logger.debug("Setting command %s", command.name)
  *         with self._command.get_lock():             # <<<<<<<<<<<<<<
- *             self._command.get_obj().value = command.value
+ *             self._command.get_obj().value = command.value #type: ignore
  * 
  */
   /*with:*/ {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get_lock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get_lock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -5505,21 +5500,21 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
-    __pyx_t_6 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L3_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
@@ -5531,15 +5526,15 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, NULL};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L3_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     /*try:*/ {
       {
@@ -5547,26 +5542,26 @@
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_9);
         /*try:*/ {
 
-          /* "tactigon_speech/middleware/Tactigon_Speech.py":95
+          /* "tactigon_speech/middleware/Tactigon_Speech.py":94
  *         self.logger.debug("Setting command %s", command.name)
  *         with self._command.get_lock():
- *             self._command.get_obj().value = command.value             # <<<<<<<<<<<<<<
+ *             self._command.get_obj().value = command.value #type: ignore             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_command, __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L7_error)
+          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_command, __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L7_error)
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L7_error)
+          __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __pyx_t_3 = NULL;
           __pyx_t_5 = 0;
           #if CYTHON_UNPACK_METHODS
           if (likely(PyMethod_Check(__pyx_t_4))) {
             __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
@@ -5579,63 +5574,63 @@
             }
           }
           #endif
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
             __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
             __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-            if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L7_error)
+            if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_2);
             __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           }
-          if (__Pyx_PyObject_SetAttrStr(__pyx_t_2, __pyx_n_s_value, __pyx_t_1) < 0) __PYX_ERR(0, 95, __pyx_L7_error)
+          if (__Pyx_PyObject_SetAttrStr(__pyx_t_2, __pyx_n_s_value, __pyx_t_1) < 0) __PYX_ERR(0, 94, __pyx_L7_error)
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-          /* "tactigon_speech/middleware/Tactigon_Speech.py":94
+          /* "tactigon_speech/middleware/Tactigon_Speech.py":93
  *     def command(self, command: Command):
  *         self.logger.debug("Setting command %s", command.name)
  *         with self._command.get_lock():             # <<<<<<<<<<<<<<
- *             self._command.get_obj().value = command.value
+ *             self._command.get_obj().value = command.value #type: ignore
  * 
  */
         }
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L12_try_end;
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("tactigon_speech.middleware.Tactigon_Speech.Tactigon_Speech.command", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_1, &__pyx_t_4) < 0) __PYX_ERR(0, 94, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_1, &__pyx_t_4) < 0) __PYX_ERR(0, 93, __pyx_L9_except_error)
           __Pyx_XGOTREF(__pyx_t_2);
           __Pyx_XGOTREF(__pyx_t_1);
           __Pyx_XGOTREF(__pyx_t_4);
-          __pyx_t_3 = PyTuple_Pack(3, __pyx_t_2, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L9_except_error)
+          __pyx_t_3 = PyTuple_Pack(3, __pyx_t_2, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_3);
           __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_3, NULL);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 94, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 93, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_10);
           __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_10);
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          if (__pyx_t_11 < 0) __PYX_ERR(0, 94, __pyx_L9_except_error)
+          if (__pyx_t_11 < 0) __PYX_ERR(0, 93, __pyx_L9_except_error)
           __pyx_t_12 = (!__pyx_t_11);
           if (unlikely(__pyx_t_12)) {
             __Pyx_GIVEREF(__pyx_t_2);
             __Pyx_GIVEREF(__pyx_t_1);
             __Pyx_XGIVEREF(__pyx_t_4);
             __Pyx_ErrRestoreWithState(__pyx_t_2, __pyx_t_1, __pyx_t_4);
             __pyx_t_2 = 0; __pyx_t_1 = 0; __pyx_t_4 = 0; 
-            __PYX_ERR(0, 94, __pyx_L9_except_error)
+            __PYX_ERR(0, 93, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -5653,30 +5648,30 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_6) {
           __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple_, NULL);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 94, __pyx_L1_error)
+          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 93, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
     goto __pyx_L16;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     goto __pyx_L1_error;
     __pyx_L16:;
   }
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":91
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":90
  *             return command
  * 
  *     @command.setter             # <<<<<<<<<<<<<<
  *     def command(self, command: Command):
  *         self.logger.debug("Setting command %s", command.name)
  */
 
@@ -5692,16 +5687,16 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tactigon_speech/middleware/Tactigon_Speech.py":97
- *             self._command.get_obj().value = command.value
+/* "tactigon_speech/middleware/Tactigon_Speech.py":96
+ *             self._command.get_obj().value = command.value #type: ignore
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def initialized(self):
  *         return self.command is not Command.NOT_INITIALIZED
  */
 
 /* Python wrapper */
@@ -5753,31 +5748,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 97, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 96, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "initialized") < 0)) __PYX_ERR(0, 97, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "initialized") < 0)) __PYX_ERR(0, 96, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("initialized", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 97, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("initialized", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 96, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -5808,40 +5803,40 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("initialized", 1);
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":99
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":98
  *     @property
  *     def initialized(self):
  *         return self.command is not Command.NOT_INITIALIZED             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Command); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Command); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_NOT_INITIALIZED); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_NOT_INITIALIZED); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = (__pyx_t_1 != __pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":97
- *             self._command.get_obj().value = command.value
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":96
+ *             self._command.get_obj().value = command.value #type: ignore
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def initialized(self):
  *         return self.command is not Command.NOT_INITIALIZED
  */
 
   /* function exit code */
@@ -5853,15 +5848,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tactigon_speech/middleware/Tactigon_Speech.py":101
+/* "tactigon_speech/middleware/Tactigon_Speech.py":100
  *         return self.command is not Command.NOT_INITIALIZED
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_recording(self):
  *         return self.command is Command.RECORD
  */
 
@@ -5914,31 +5909,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 100, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "is_recording") < 0)) __PYX_ERR(0, 101, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "is_recording") < 0)) __PYX_ERR(0, 100, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("is_recording", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 101, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("is_recording", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 100, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -5969,39 +5964,39 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_recording", 1);
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":103
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":102
  *     @property
  *     def is_recording(self):
  *         return self.command is Command.RECORD             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Command); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Command); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_RECORD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_RECORD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = (__pyx_t_1 == __pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":101
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":100
  *         return self.command is not Command.NOT_INITIALIZED
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_recording(self):
  *         return self.command is Command.RECORD
  */
 
@@ -6014,15 +6009,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tactigon_speech/middleware/Tactigon_Speech.py":105
+/* "tactigon_speech/middleware/Tactigon_Speech.py":104
  *         return self.command is Command.RECORD
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_listening(self):
  *         return self.command is Command.LISTEN
  */
 
@@ -6075,31 +6070,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 104, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "is_listening") < 0)) __PYX_ERR(0, 105, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "is_listening") < 0)) __PYX_ERR(0, 104, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("is_listening", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 105, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("is_listening", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 104, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -6130,39 +6125,39 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_listening", 1);
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":107
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":106
  *     @property
  *     def is_listening(self):
  *         return self.command is Command.LISTEN             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Command); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Command); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_LISTEN); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_LISTEN); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = (__pyx_t_1 == __pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":105
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":104
  *         return self.command is Command.RECORD
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_listening(self):
  *         return self.command is Command.LISTEN
  */
 
@@ -6175,15 +6170,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tactigon_speech/middleware/Tactigon_Speech.py":109
+/* "tactigon_speech/middleware/Tactigon_Speech.py":108
  *         return self.command is Command.LISTEN
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_playing(self):
  *         return self.command is Command.PLAY
  */
 
@@ -6236,31 +6231,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 109, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 108, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "is_playing") < 0)) __PYX_ERR(0, 109, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "is_playing") < 0)) __PYX_ERR(0, 108, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("is_playing", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 109, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("is_playing", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 108, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -6291,39 +6286,39 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_playing", 1);
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":111
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":110
  *     @property
  *     def is_playing(self):
  *         return self.command is Command.PLAY             # <<<<<<<<<<<<<<
  * 
  *     def is_timeout(self, tick: datetime, timeout: int):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Command); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Command); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_PLAY); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_PLAY); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = (__pyx_t_1 == __pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":109
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":108
  *         return self.command is Command.LISTEN
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_playing(self):
  *         return self.command is Command.PLAY
  */
 
@@ -6336,15 +6331,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tactigon_speech/middleware/Tactigon_Speech.py":113
+/* "tactigon_speech/middleware/Tactigon_Speech.py":112
  *         return self.command is Command.PLAY
  * 
  *     def is_timeout(self, tick: datetime, timeout: int):             # <<<<<<<<<<<<<<
  *         return (millis() - tick).total_seconds() > timeout
  * 
  */
 
@@ -6403,69 +6398,69 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 112, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_tick)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 112, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("is_timeout", 1, 3, 3, 1); __PYX_ERR(0, 113, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("is_timeout", 1, 3, 3, 1); __PYX_ERR(0, 112, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_timeout)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 112, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("is_timeout", 1, 3, 3, 2); __PYX_ERR(0, 113, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("is_timeout", 1, 3, 3, 2); __PYX_ERR(0, 112, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "is_timeout") < 0)) __PYX_ERR(0, 113, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "is_timeout") < 0)) __PYX_ERR(0, 112, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_tick = values[1];
     __pyx_v_timeout = ((PyObject*)values[2]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("is_timeout", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 113, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("is_timeout", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 112, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("tactigon_speech.middleware.Tactigon_Speech.Tactigon_Speech.is_timeout", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_timeout), (&PyInt_Type), 0, "timeout", 1))) __PYX_ERR(0, 113, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_timeout), (&PyInt_Type), 0, "timeout", 1))) __PYX_ERR(0, 112, __pyx_L1_error)
   __pyx_r = __pyx_pf_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_14is_timeout(__pyx_self, __pyx_v_self, __pyx_v_tick, __pyx_v_timeout);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -6488,23 +6483,23 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_timeout", 1);
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":114
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":113
  * 
  *     def is_timeout(self, tick: datetime, timeout: int):
  *         return (millis() - tick).total_seconds() > timeout             # <<<<<<<<<<<<<<
  * 
  *     def vad_collector(self) -> Generator[bytes, bytes, None]:
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_millis); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_millis); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -6516,22 +6511,22 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, NULL};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_3 = PyNumber_Subtract(__pyx_t_2, __pyx_v_tick); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Subtract(__pyx_t_2, __pyx_v_tick); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_total_seconds); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_total_seconds); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -6544,25 +6539,25 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_v_timeout, Py_GT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_v_timeout, Py_GT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":113
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":112
  *         return self.command is Command.PLAY
  * 
  *     def is_timeout(self, tick: datetime, timeout: int):             # <<<<<<<<<<<<<<
  *         return (millis() - tick).total_seconds() > timeout
  * 
  */
 
@@ -6577,15 +6572,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_18generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "tactigon_speech/middleware/Tactigon_Speech.py":116
+/* "tactigon_speech/middleware/Tactigon_Speech.py":115
  *         return (millis() - tick).total_seconds() > timeout
  * 
  *     def vad_collector(self) -> Generator[bytes, bytes, None]:             # <<<<<<<<<<<<<<
  *         frame_length = int(2 * self._SAMPLE_RATE * self.vad_frame / 1000)
  *         num_padding_frames: int = int(frame_length * (self.vad_padding_ms / 10000))
  */
 
@@ -6638,31 +6633,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 115, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "vad_collector") < 0)) __PYX_ERR(0, 116, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "vad_collector") < 0)) __PYX_ERR(0, 115, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("vad_collector", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 116, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("vad_collector", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 115, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -6693,23 +6688,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("vad_collector", 0);
   __pyx_cur_scope = (struct __pyx_obj_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector *)__pyx_tp_new_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector(__pyx_ptype_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 116, __pyx_L1_error)
+    __PYX_ERR(0, 115, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_self);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_18generator, __pyx_codeobj__2, (PyObject *) __pyx_cur_scope, __pyx_n_s_vad_collector, __pyx_n_s_Tactigon_Speech_vad_collector, __pyx_n_s_tactigon_speech_middleware_Tacti); if (unlikely(!gen)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_18generator, __pyx_codeobj__2, (PyObject *) __pyx_cur_scope, __pyx_n_s_vad_collector, __pyx_n_s_Tactigon_Speech_vad_collector, __pyx_n_s_tactigon_speech_middleware_Tacti); if (unlikely(!gen)) __PYX_ERR(0, 115, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6727,16 +6722,16 @@
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
-  Py_ssize_t __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  Py_ssize_t __pyx_t_8;
   int __pyx_t_9;
   PyObject *(*__pyx_t_10)(PyObject *);
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   PyObject *(*__pyx_t_13)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -6748,125 +6743,125 @@
     case 1: goto __pyx_L22_resume_from_yield;
     case 2: goto __pyx_L25_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 116, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 115, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":117
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":116
  * 
  *     def vad_collector(self) -> Generator[bytes, bytes, None]:
  *         frame_length = int(2 * self._SAMPLE_RATE * self.vad_frame / 1000)             # <<<<<<<<<<<<<<
  *         num_padding_frames: int = int(frame_length * (self.vad_padding_ms / 10000))
  *         num_voiced_threshold = self.vad_ratio * num_padding_frames
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_SAMPLE_RATE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_SAMPLE_RATE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_MultiplyCObj(__pyx_int_2, __pyx_t_1, 2, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_MultiplyCObj(__pyx_int_2, __pyx_t_1, 2, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_vad_frame); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_vad_frame); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_TrueDivideObjC(__pyx_t_3, __pyx_int_1000, 0x3E8, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_TrueDivideObjC(__pyx_t_3, __pyx_int_1000, 0x3E8, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_cur_scope->__pyx_v_frame_length = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":118
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":117
  *     def vad_collector(self) -> Generator[bytes, bytes, None]:
  *         frame_length = int(2 * self._SAMPLE_RATE * self.vad_frame / 1000)
  *         num_padding_frames: int = int(frame_length * (self.vad_padding_ms / 10000))             # <<<<<<<<<<<<<<
  *         num_voiced_threshold = self.vad_ratio * num_padding_frames
  *         triggered = False
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_vad_padding_ms); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_vad_padding_ms); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyInt_TrueDivideObjC(__pyx_t_3, __pyx_int_10000, 0x2710, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_TrueDivideObjC(__pyx_t_3, __pyx_int_10000, 0x2710, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Multiply(__pyx_cur_scope->__pyx_v_frame_length, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_cur_scope->__pyx_v_frame_length, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_cur_scope->__pyx_v_num_padding_frames = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":119
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":118
  *         frame_length = int(2 * self._SAMPLE_RATE * self.vad_frame / 1000)
  *         num_padding_frames: int = int(frame_length * (self.vad_padding_ms / 10000))
  *         num_voiced_threshold = self.vad_ratio * num_padding_frames             # <<<<<<<<<<<<<<
  *         triggered = False
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_vad_ratio); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_vad_ratio); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_cur_scope->__pyx_v_num_padding_frames); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_cur_scope->__pyx_v_num_padding_frames); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_cur_scope->__pyx_v_num_voiced_threshold = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":120
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":119
  *         num_padding_frames: int = int(frame_length * (self.vad_padding_ms / 10000))
  *         num_voiced_threshold = self.vad_ratio * num_padding_frames
  *         triggered = False             # <<<<<<<<<<<<<<
  * 
  *         ring_buffer = collections.deque(maxlen=num_padding_frames)
  */
   __pyx_cur_scope->__pyx_v_triggered = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":122
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":121
  *         triggered = False
  * 
  *         ring_buffer = collections.deque(maxlen=num_padding_frames)             # <<<<<<<<<<<<<<
  * 
  *         self.logger.debug("[VAD] Frame length: %i, Frame paddings: %i, Voiced threshold: %f", frame_length, num_padding_frames, num_voiced_threshold)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_collections); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_collections); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_deque); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_deque); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_maxlen, __pyx_cur_scope->__pyx_v_num_padding_frames) < 0) __PYX_ERR(0, 122, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_maxlen, __pyx_cur_scope->__pyx_v_num_padding_frames) < 0) __PYX_ERR(0, 121, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_cur_scope->__pyx_v_ring_buffer = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":124
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":123
  *         ring_buffer = collections.deque(maxlen=num_padding_frames)
  * 
  *         self.logger.debug("[VAD] Frame length: %i, Frame paddings: %i, Voiced threshold: %f", frame_length, num_padding_frames, num_voiced_threshold)             # <<<<<<<<<<<<<<
  * 
  *         frame = b''
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_debug); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_debug); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
@@ -6879,39 +6874,39 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[5] = {__pyx_t_3, __pyx_kp_s_VAD_Frame_length_i_Frame_paddin, __pyx_cur_scope->__pyx_v_frame_length, __pyx_cur_scope->__pyx_v_num_padding_frames, __pyx_cur_scope->__pyx_v_num_voiced_threshold};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 4+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":126
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":125
  *         self.logger.debug("[VAD] Frame length: %i, Frame paddings: %i, Voiced threshold: %f", frame_length, num_padding_frames, num_voiced_threshold)
  * 
  *         frame = b''             # <<<<<<<<<<<<<<
  *         ticks = millis()
  *         while True:
  */
   __Pyx_INCREF(__pyx_kp_b__3);
   __Pyx_GIVEREF(__pyx_kp_b__3);
   __pyx_cur_scope->__pyx_v_frame = __pyx_kp_b__3;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":127
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":126
  * 
  *         frame = b''
  *         ticks = millis()             # <<<<<<<<<<<<<<
  *         while True:
  *             if self.command == Command.STOP:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_millis); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_millis); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
@@ -6923,80 +6918,80 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_cur_scope->__pyx_v_ticks = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":128
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":127
  *         frame = b''
  *         ticks = millis()
  *         while True:             # <<<<<<<<<<<<<<
  *             if self.command == Command.STOP:
  *                 break
  */
   while (1) {
 
-    /* "tactigon_speech/middleware/Tactigon_Speech.py":129
+    /* "tactigon_speech/middleware/Tactigon_Speech.py":128
  *         ticks = millis()
  *         while True:
  *             if self.command == Command.STOP:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_command_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_command_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 128, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Command); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Command); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_STOP); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_STOP); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 128, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_5) {
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":130
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":129
  *         while True:
  *             if self.command == Command.STOP:
  *                 break             # <<<<<<<<<<<<<<
  * 
  *             if not self.audio.poll():
  */
       goto __pyx_L5_break;
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":129
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":128
  *         ticks = millis()
  *         while True:
  *             if self.command == Command.STOP:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
     }
 
-    /* "tactigon_speech/middleware/Tactigon_Speech.py":132
+    /* "tactigon_speech/middleware/Tactigon_Speech.py":131
  *                 break
  * 
  *             if not self.audio.poll():             # <<<<<<<<<<<<<<
+ *                 time.sleep(self._TICK/2)
  *                 continue
- * 
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_audio); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 132, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_audio); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_poll); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_poll); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -7009,109 +7004,151 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 132, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_6 = (!__pyx_t_5);
     if (__pyx_t_6) {
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":133
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":132
+ * 
+ *             if not self.audio.poll():
+ *                 time.sleep(self._TICK/2)             # <<<<<<<<<<<<<<
+ *                 continue
  * 
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_sleep); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 132, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_TICK); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_7 = __Pyx_PyInt_TrueDivideObjC(__pyx_t_2, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 132, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_2 = NULL;
+      __pyx_t_4 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+        if (likely(__pyx_t_2)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_2);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
+          __pyx_t_4 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_7};
+        __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      }
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":133
  *             if not self.audio.poll():
+ *                 time.sleep(self._TICK/2)
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             audio_bytes = self.audio.recv_bytes()
  */
       goto __pyx_L4_continue;
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":132
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":131
  *                 break
  * 
  *             if not self.audio.poll():             # <<<<<<<<<<<<<<
+ *                 time.sleep(self._TICK/2)
  *                 continue
- * 
  */
     }
 
     /* "tactigon_speech/middleware/Tactigon_Speech.py":135
  *                 continue
  * 
  *             audio_bytes = self.audio.recv_bytes()             # <<<<<<<<<<<<<<
  * 
  *             if len(frame) < frame_length:
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_audio); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_recv_bytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_audio); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = NULL;
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_recv_bytes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 135, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_2)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_2);
+    if (likely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_3)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+        __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
+        __Pyx_DECREF_SET(__pyx_t_7, function);
         __pyx_t_4 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
-      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
-      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+      PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_audio_bytes);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_audio_bytes, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     __pyx_t_1 = 0;
 
     /* "tactigon_speech/middleware/Tactigon_Speech.py":137
  *             audio_bytes = self.audio.recv_bytes()
  * 
  *             if len(frame) < frame_length:             # <<<<<<<<<<<<<<
  *                 frame += audio_bytes
  *                 continue
  */
-    __pyx_t_7 = PyObject_Length(__pyx_cur_scope->__pyx_v_frame); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 137, __pyx_L1_error)
-    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
+    __pyx_t_8 = PyObject_Length(__pyx_cur_scope->__pyx_v_frame); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 137, __pyx_L1_error)
+    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_cur_scope->__pyx_v_frame_length, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 137, __pyx_L1_error)
+    __pyx_t_7 = PyObject_RichCompare(__pyx_t_1, __pyx_cur_scope->__pyx_v_frame_length, Py_LT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 137, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 137, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 137, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (__pyx_t_6) {
 
       /* "tactigon_speech/middleware/Tactigon_Speech.py":138
  * 
  *             if len(frame) < frame_length:
  *                 frame += audio_bytes             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
-      __pyx_t_3 = PyNumber_InPlaceAdd(__pyx_cur_scope->__pyx_v_frame, __pyx_cur_scope->__pyx_v_audio_bytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 138, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_7 = PyNumber_InPlaceAdd(__pyx_cur_scope->__pyx_v_frame, __pyx_cur_scope->__pyx_v_audio_bytes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 138, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_frame);
-      __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_frame, __pyx_t_3);
-      __Pyx_GIVEREF(__pyx_t_3);
-      __pyx_t_3 = 0;
+      __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_frame, __pyx_t_7);
+      __Pyx_GIVEREF(__pyx_t_7);
+      __pyx_t_7 = 0;
 
       /* "tactigon_speech/middleware/Tactigon_Speech.py":139
  *             if len(frame) < frame_length:
  *                 frame += audio_bytes
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             is_speech = self.vad.is_speech(frame, self._SAMPLE_RATE)
@@ -7132,46 +7169,46 @@
  * 
  *             is_speech = self.vad.is_speech(frame, self._SAMPLE_RATE)             # <<<<<<<<<<<<<<
  *             if not triggered:
  *                 if self.is_timeout(ticks, self.silence_timeout):
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_vad); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 141, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_is_speech); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 141, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_is_speech); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 141, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_SAMPLE_RATE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 141, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = NULL;
+    __pyx_t_2 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_8)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_8);
+    if (likely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_2)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_4 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[3] = {__pyx_t_8, __pyx_cur_scope->__pyx_v_frame, __pyx_t_1};
-      __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
-      __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+      PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_cur_scope->__pyx_v_frame, __pyx_t_1};
+      __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
+      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 141, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 141, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_is_speech);
-    __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_is_speech, __pyx_t_3);
-    __Pyx_GIVEREF(__pyx_t_3);
-    __pyx_t_3 = 0;
+    __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_is_speech, __pyx_t_7);
+    __Pyx_GIVEREF(__pyx_t_7);
+    __pyx_t_7 = 0;
 
     /* "tactigon_speech/middleware/Tactigon_Speech.py":142
  * 
  *             is_speech = self.vad.is_speech(frame, self._SAMPLE_RATE)
  *             if not triggered:             # <<<<<<<<<<<<<<
  *                 if self.is_timeout(ticks, self.silence_timeout):
  *                     self._is_timeout = True
@@ -7182,43 +7219,43 @@
       /* "tactigon_speech/middleware/Tactigon_Speech.py":143
  *             is_speech = self.vad.is_speech(frame, self._SAMPLE_RATE)
  *             if not triggered:
  *                 if self.is_timeout(ticks, self.silence_timeout):             # <<<<<<<<<<<<<<
  *                     self._is_timeout = True
  *                     break
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_is_timeout); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_is_timeout); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_silence_timeout); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_8 = NULL;
+      __pyx_t_2 = NULL;
       __pyx_t_4 = 0;
       #if CYTHON_UNPACK_METHODS
-      if (likely(PyMethod_Check(__pyx_t_2))) {
-        __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
-        if (likely(__pyx_t_8)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-          __Pyx_INCREF(__pyx_t_8);
+      if (likely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+        if (likely(__pyx_t_2)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_2);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_2, function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
           __pyx_t_4 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[3] = {__pyx_t_8, __pyx_cur_scope->__pyx_v_ticks, __pyx_t_1};
-        __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
-        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+        PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_cur_scope->__pyx_v_ticks, __pyx_t_1};
+        __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
+        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 143, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 143, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 143, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       if (__pyx_t_6) {
 
         /* "tactigon_speech/middleware/Tactigon_Speech.py":144
  *             if not triggered:
  *                 if self.is_timeout(ticks, self.silence_timeout):
  *                     self._is_timeout = True             # <<<<<<<<<<<<<<
  *                     break
@@ -7247,77 +7284,77 @@
       /* "tactigon_speech/middleware/Tactigon_Speech.py":147
  *                     break
  * 
  *                 ring_buffer.append((frame, is_speech))             # <<<<<<<<<<<<<<
  * 
  *                 num_voiced = len([f for f, speech in ring_buffer if speech])
  */
-      __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 147, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_frame);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_frame);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_cur_scope->__pyx_v_frame)) __PYX_ERR(0, 147, __pyx_L1_error);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_cur_scope->__pyx_v_frame)) __PYX_ERR(0, 147, __pyx_L1_error);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_is_speech);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_is_speech);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_cur_scope->__pyx_v_is_speech)) __PYX_ERR(0, 147, __pyx_L1_error);
-      __pyx_t_9 = __Pyx_PyObject_Append(__pyx_cur_scope->__pyx_v_ring_buffer, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 147, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_cur_scope->__pyx_v_is_speech)) __PYX_ERR(0, 147, __pyx_L1_error);
+      __pyx_t_9 = __Pyx_PyObject_Append(__pyx_cur_scope->__pyx_v_ring_buffer, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 147, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
       /* "tactigon_speech/middleware/Tactigon_Speech.py":149
  *                 ring_buffer.append((frame, is_speech))
  * 
  *                 num_voiced = len([f for f, speech in ring_buffer if speech])             # <<<<<<<<<<<<<<
  *                 self.logger.debug("Got %i voiced frames. Threshold is %f", num_voiced, num_voiced_threshold)
  *                 if num_voiced >= num_voiced_threshold:
  */
       { /* enter inner scope */
-        __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
+        __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 149, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
         if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_v_ring_buffer)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_v_ring_buffer)) {
-          __pyx_t_2 = __pyx_cur_scope->__pyx_v_ring_buffer; __Pyx_INCREF(__pyx_t_2);
-          __pyx_t_7 = 0;
+          __pyx_t_3 = __pyx_cur_scope->__pyx_v_ring_buffer; __Pyx_INCREF(__pyx_t_3);
+          __pyx_t_8 = 0;
           __pyx_t_10 = NULL;
         } else {
-          __pyx_t_7 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_cur_scope->__pyx_v_ring_buffer); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_10 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 149, __pyx_L1_error)
+          __pyx_t_8 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_cur_scope->__pyx_v_ring_buffer); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_3);
+          __pyx_t_10 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 149, __pyx_L1_error)
         }
         for (;;) {
           if (likely(!__pyx_t_10)) {
-            if (likely(PyList_CheckExact(__pyx_t_2))) {
+            if (likely(PyList_CheckExact(__pyx_t_3))) {
               {
-                Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+                Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_3);
                 #if !CYTHON_ASSUME_SAFE_MACROS
                 if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 149, __pyx_L1_error)
                 #endif
-                if (__pyx_t_7 >= __pyx_temp) break;
+                if (__pyx_t_8 >= __pyx_temp) break;
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 149, __pyx_L1_error)
+              __pyx_t_1 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_8); __Pyx_INCREF(__pyx_t_1); __pyx_t_8++; if (unlikely((0 < 0))) __PYX_ERR(0, 149, __pyx_L1_error)
               #else
-              __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
+              __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
               __Pyx_GOTREF(__pyx_t_1);
               #endif
             } else {
               {
-                Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+                Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_3);
                 #if !CYTHON_ASSUME_SAFE_MACROS
                 if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 149, __pyx_L1_error)
                 #endif
-                if (__pyx_t_7 >= __pyx_temp) break;
+                if (__pyx_t_8 >= __pyx_temp) break;
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 149, __pyx_L1_error)
+              __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_8); __Pyx_INCREF(__pyx_t_1); __pyx_t_8++; if (unlikely((0 < 0))) __PYX_ERR(0, 149, __pyx_L1_error)
               #else
-              __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
+              __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
               __Pyx_GOTREF(__pyx_t_1);
               #endif
             }
           } else {
-            __pyx_t_1 = __pyx_t_10(__pyx_t_2);
+            __pyx_t_1 = __pyx_t_10(__pyx_t_3);
             if (unlikely(!__pyx_t_1)) {
               PyObject* exc_type = PyErr_Occurred();
               if (exc_type) {
                 if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
                 else __PYX_ERR(0, 149, __pyx_L1_error)
               }
               break;
@@ -7330,83 +7367,83 @@
             if (unlikely(size != 2)) {
               if (size > 2) __Pyx_RaiseTooManyValuesError(2);
               else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
               __PYX_ERR(0, 149, __pyx_L1_error)
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
             if (likely(PyTuple_CheckExact(sequence))) {
-              __pyx_t_8 = PyTuple_GET_ITEM(sequence, 0); 
+              __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
               __pyx_t_11 = PyTuple_GET_ITEM(sequence, 1); 
             } else {
-              __pyx_t_8 = PyList_GET_ITEM(sequence, 0); 
+              __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
               __pyx_t_11 = PyList_GET_ITEM(sequence, 1); 
             }
-            __Pyx_INCREF(__pyx_t_8);
+            __Pyx_INCREF(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_11);
             #else
-            __pyx_t_8 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 149, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_8);
+            __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_2);
             __pyx_t_11 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 149, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_11);
             #endif
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           } else {
             Py_ssize_t index = -1;
             __pyx_t_12 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 149, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_12);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
             __pyx_t_13 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_12);
-            index = 0; __pyx_t_8 = __pyx_t_13(__pyx_t_12); if (unlikely(!__pyx_t_8)) goto __pyx_L13_unpacking_failed;
-            __Pyx_GOTREF(__pyx_t_8);
+            index = 0; __pyx_t_2 = __pyx_t_13(__pyx_t_12); if (unlikely(!__pyx_t_2)) goto __pyx_L13_unpacking_failed;
+            __Pyx_GOTREF(__pyx_t_2);
             index = 1; __pyx_t_11 = __pyx_t_13(__pyx_t_12); if (unlikely(!__pyx_t_11)) goto __pyx_L13_unpacking_failed;
             __Pyx_GOTREF(__pyx_t_11);
             if (__Pyx_IternextUnpackEndCheck(__pyx_t_13(__pyx_t_12), 2) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
             __pyx_t_13 = NULL;
             __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
             goto __pyx_L14_unpacking_done;
             __pyx_L13_unpacking_failed:;
             __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
             __pyx_t_13 = NULL;
             if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
             __PYX_ERR(0, 149, __pyx_L1_error)
             __pyx_L14_unpacking_done:;
           }
           __Pyx_XGOTREF(__pyx_cur_scope->__pyx_7genexpr__pyx_v_f);
-          __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_7genexpr__pyx_v_f, __pyx_t_8);
-          __Pyx_GIVEREF(__pyx_t_8);
-          __pyx_t_8 = 0;
+          __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_7genexpr__pyx_v_f, __pyx_t_2);
+          __Pyx_GIVEREF(__pyx_t_2);
+          __pyx_t_2 = 0;
           __Pyx_XGOTREF(__pyx_cur_scope->__pyx_7genexpr__pyx_v_speech);
           __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_7genexpr__pyx_v_speech, __pyx_t_11);
           __Pyx_GIVEREF(__pyx_t_11);
           __pyx_t_11 = 0;
           __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_7genexpr__pyx_v_speech); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 149, __pyx_L1_error)
           if (__pyx_t_6) {
-            if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_cur_scope->__pyx_7genexpr__pyx_v_f))) __PYX_ERR(0, 149, __pyx_L1_error)
+            if (unlikely(__Pyx_ListComp_Append(__pyx_t_7, (PyObject*)__pyx_cur_scope->__pyx_7genexpr__pyx_v_f))) __PYX_ERR(0, 149, __pyx_L1_error)
           }
         }
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       } /* exit inner scope */
-      __pyx_t_7 = __Pyx_PyList_GET_SIZE(__pyx_t_3); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 149, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_cur_scope->__pyx_v_num_voiced = __pyx_t_7;
+      __pyx_t_8 = __Pyx_PyList_GET_SIZE(__pyx_t_7); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 149, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __pyx_cur_scope->__pyx_v_num_voiced = __pyx_t_8;
 
       /* "tactigon_speech/middleware/Tactigon_Speech.py":150
  * 
  *                 num_voiced = len([f for f, speech in ring_buffer if speech])
  *                 self.logger.debug("Got %i voiced frames. Threshold is %f", num_voiced, num_voiced_threshold)             # <<<<<<<<<<<<<<
  *                 if num_voiced >= num_voiced_threshold:
  *                     triggered = True
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_debug); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = PyInt_FromSsize_t(__pyx_cur_scope->__pyx_v_num_voiced); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_3 = PyInt_FromSsize_t(__pyx_cur_scope->__pyx_v_num_voiced); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_11 = NULL;
       __pyx_t_4 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_11)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -7414,35 +7451,35 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
           __pyx_t_4 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[4] = {__pyx_t_11, __pyx_kp_s_Got_i_voiced_frames_Threshold_is, __pyx_t_2, __pyx_cur_scope->__pyx_v_num_voiced_threshold};
-        __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 3+__pyx_t_4);
+        PyObject *__pyx_callargs[4] = {__pyx_t_11, __pyx_kp_s_Got_i_voiced_frames_Threshold_is, __pyx_t_3, __pyx_cur_scope->__pyx_v_num_voiced_threshold};
+        __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 3+__pyx_t_4);
         __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 150, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
       /* "tactigon_speech/middleware/Tactigon_Speech.py":151
  *                 num_voiced = len([f for f, speech in ring_buffer if speech])
  *                 self.logger.debug("Got %i voiced frames. Threshold is %f", num_voiced, num_voiced_threshold)
  *                 if num_voiced >= num_voiced_threshold:             # <<<<<<<<<<<<<<
  *                     triggered = True
  *                     ticks = millis()
  */
-      __pyx_t_3 = PyInt_FromSsize_t(__pyx_cur_scope->__pyx_v_num_voiced); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 151, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_1 = PyObject_RichCompare(__pyx_t_3, __pyx_cur_scope->__pyx_v_num_voiced_threshold, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_7 = PyInt_FromSsize_t(__pyx_cur_scope->__pyx_v_num_voiced); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 151, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_1 = PyObject_RichCompare(__pyx_t_7, __pyx_cur_scope->__pyx_v_num_voiced_threshold, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 151, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (__pyx_t_6) {
 
         /* "tactigon_speech/middleware/Tactigon_Speech.py":152
  *                 self.logger.debug("Got %i voiced frames. Threshold is %f", num_voiced, num_voiced_threshold)
  *                 if num_voiced >= num_voiced_threshold:
@@ -7455,37 +7492,37 @@
         /* "tactigon_speech/middleware/Tactigon_Speech.py":153
  *                 if num_voiced >= num_voiced_threshold:
  *                     triggered = True
  *                     ticks = millis()             # <<<<<<<<<<<<<<
  *                     for f, s in ring_buffer:
  *                         yield f
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_millis); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_2 = NULL;
+        __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_millis); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 153, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        __pyx_t_3 = NULL;
         __pyx_t_4 = 0;
         #if CYTHON_UNPACK_METHODS
-        if (unlikely(PyMethod_Check(__pyx_t_3))) {
-          __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-          if (likely(__pyx_t_2)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-            __Pyx_INCREF(__pyx_t_2);
+        if (unlikely(PyMethod_Check(__pyx_t_7))) {
+          __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
+          if (likely(__pyx_t_3)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+            __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_3, function);
+            __Pyx_DECREF_SET(__pyx_t_7, function);
             __pyx_t_4 = 1;
           }
         }
         #endif
         {
-          PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
-          __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
-          __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+          PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
+          __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+          __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+          __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         }
         __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_ticks);
         __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_ticks, __pyx_t_1);
         __Pyx_GIVEREF(__pyx_t_1);
         __pyx_t_1 = 0;
 
         /* "tactigon_speech/middleware/Tactigon_Speech.py":154
@@ -7493,114 +7530,114 @@
  *                     ticks = millis()
  *                     for f, s in ring_buffer:             # <<<<<<<<<<<<<<
  *                         yield f
  *                     ring_buffer.clear()
  */
         if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_v_ring_buffer)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_v_ring_buffer)) {
           __pyx_t_1 = __pyx_cur_scope->__pyx_v_ring_buffer; __Pyx_INCREF(__pyx_t_1);
-          __pyx_t_7 = 0;
+          __pyx_t_8 = 0;
           __pyx_t_10 = NULL;
         } else {
-          __pyx_t_7 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_v_ring_buffer); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+          __pyx_t_8 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_v_ring_buffer); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           __pyx_t_10 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 154, __pyx_L1_error)
         }
         for (;;) {
           if (likely(!__pyx_t_10)) {
             if (likely(PyList_CheckExact(__pyx_t_1))) {
               {
                 Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
                 #if !CYTHON_ASSUME_SAFE_MACROS
                 if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 154, __pyx_L1_error)
                 #endif
-                if (__pyx_t_7 >= __pyx_temp) break;
+                if (__pyx_t_8 >= __pyx_temp) break;
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 154, __pyx_L1_error)
+              __pyx_t_7 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_8); __Pyx_INCREF(__pyx_t_7); __pyx_t_8++; if (unlikely((0 < 0))) __PYX_ERR(0, 154, __pyx_L1_error)
               #else
-              __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
-              __Pyx_GOTREF(__pyx_t_3);
+              __pyx_t_7 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 154, __pyx_L1_error)
+              __Pyx_GOTREF(__pyx_t_7);
               #endif
             } else {
               {
                 Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
                 #if !CYTHON_ASSUME_SAFE_MACROS
                 if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 154, __pyx_L1_error)
                 #endif
-                if (__pyx_t_7 >= __pyx_temp) break;
+                if (__pyx_t_8 >= __pyx_temp) break;
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 154, __pyx_L1_error)
+              __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_8); __Pyx_INCREF(__pyx_t_7); __pyx_t_8++; if (unlikely((0 < 0))) __PYX_ERR(0, 154, __pyx_L1_error)
               #else
-              __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
-              __Pyx_GOTREF(__pyx_t_3);
+              __pyx_t_7 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 154, __pyx_L1_error)
+              __Pyx_GOTREF(__pyx_t_7);
               #endif
             }
           } else {
-            __pyx_t_3 = __pyx_t_10(__pyx_t_1);
-            if (unlikely(!__pyx_t_3)) {
+            __pyx_t_7 = __pyx_t_10(__pyx_t_1);
+            if (unlikely(!__pyx_t_7)) {
               PyObject* exc_type = PyErr_Occurred();
               if (exc_type) {
                 if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
                 else __PYX_ERR(0, 154, __pyx_L1_error)
               }
               break;
             }
-            __Pyx_GOTREF(__pyx_t_3);
+            __Pyx_GOTREF(__pyx_t_7);
           }
-          if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
-            PyObject* sequence = __pyx_t_3;
+          if ((likely(PyTuple_CheckExact(__pyx_t_7))) || (PyList_CheckExact(__pyx_t_7))) {
+            PyObject* sequence = __pyx_t_7;
             Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
             if (unlikely(size != 2)) {
               if (size > 2) __Pyx_RaiseTooManyValuesError(2);
               else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
               __PYX_ERR(0, 154, __pyx_L1_error)
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
             if (likely(PyTuple_CheckExact(sequence))) {
-              __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
+              __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
               __pyx_t_11 = PyTuple_GET_ITEM(sequence, 1); 
             } else {
-              __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
+              __pyx_t_3 = PyList_GET_ITEM(sequence, 0); 
               __pyx_t_11 = PyList_GET_ITEM(sequence, 1); 
             }
-            __Pyx_INCREF(__pyx_t_2);
+            __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(__pyx_t_11);
             #else
-            __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_2);
+            __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_3);
             __pyx_t_11 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 154, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_11);
             #endif
-            __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+            __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
           } else {
             Py_ssize_t index = -1;
-            __pyx_t_8 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 154, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_8);
-            __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-            __pyx_t_13 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_8);
-            index = 0; __pyx_t_2 = __pyx_t_13(__pyx_t_8); if (unlikely(!__pyx_t_2)) goto __pyx_L20_unpacking_failed;
+            __pyx_t_2 = PyObject_GetIter(__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_2);
-            index = 1; __pyx_t_11 = __pyx_t_13(__pyx_t_8); if (unlikely(!__pyx_t_11)) goto __pyx_L20_unpacking_failed;
+            __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+            __pyx_t_13 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2);
+            index = 0; __pyx_t_3 = __pyx_t_13(__pyx_t_2); if (unlikely(!__pyx_t_3)) goto __pyx_L20_unpacking_failed;
+            __Pyx_GOTREF(__pyx_t_3);
+            index = 1; __pyx_t_11 = __pyx_t_13(__pyx_t_2); if (unlikely(!__pyx_t_11)) goto __pyx_L20_unpacking_failed;
             __Pyx_GOTREF(__pyx_t_11);
-            if (__Pyx_IternextUnpackEndCheck(__pyx_t_13(__pyx_t_8), 2) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
+            if (__Pyx_IternextUnpackEndCheck(__pyx_t_13(__pyx_t_2), 2) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
             __pyx_t_13 = NULL;
-            __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             goto __pyx_L21_unpacking_done;
             __pyx_L20_unpacking_failed:;
-            __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             __pyx_t_13 = NULL;
             if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
             __PYX_ERR(0, 154, __pyx_L1_error)
             __pyx_L21_unpacking_done:;
           }
           __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_f);
-          __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_f, __pyx_t_2);
-          __Pyx_GIVEREF(__pyx_t_2);
-          __pyx_t_2 = 0;
+          __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_f, __pyx_t_3);
+          __Pyx_GIVEREF(__pyx_t_3);
+          __pyx_t_3 = 0;
           __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_s);
           __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_s, __pyx_t_11);
           __Pyx_GIVEREF(__pyx_t_11);
           __pyx_t_11 = 0;
 
           /* "tactigon_speech/middleware/Tactigon_Speech.py":155
  *                     ticks = millis()
@@ -7609,27 +7646,27 @@
  *                     ring_buffer.clear()
  * 
  */
           __Pyx_INCREF(__pyx_cur_scope->__pyx_v_f);
           __pyx_r = __pyx_cur_scope->__pyx_v_f;
           __Pyx_XGIVEREF(__pyx_t_1);
           __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
-          __pyx_cur_scope->__pyx_t_1 = __pyx_t_7;
+          __pyx_cur_scope->__pyx_t_1 = __pyx_t_8;
           __pyx_cur_scope->__pyx_t_2 = __pyx_t_10;
           __Pyx_XGIVEREF(__pyx_r);
           __Pyx_RefNannyFinishContext();
           __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
           /* return from generator, yielding value */
           __pyx_generator->resume_label = 1;
           return __pyx_r;
           __pyx_L22_resume_from_yield:;
           __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
           __pyx_cur_scope->__pyx_t_0 = 0;
           __Pyx_XGOTREF(__pyx_t_1);
-          __pyx_t_7 = __pyx_cur_scope->__pyx_t_1;
+          __pyx_t_8 = __pyx_cur_scope->__pyx_t_1;
           __pyx_t_10 = __pyx_cur_scope->__pyx_t_2;
           if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 155, __pyx_L1_error)
 
           /* "tactigon_speech/middleware/Tactigon_Speech.py":154
  *                     triggered = True
  *                     ticks = millis()
  *                     for f, s in ring_buffer:             # <<<<<<<<<<<<<<
@@ -7642,37 +7679,37 @@
         /* "tactigon_speech/middleware/Tactigon_Speech.py":156
  *                     for f, s in ring_buffer:
  *                         yield f
  *                     ring_buffer.clear()             # <<<<<<<<<<<<<<
  * 
  *             else:
  */
-        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_ring_buffer, __pyx_n_s_clear); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
+        __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_ring_buffer, __pyx_n_s_clear); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 156, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
         __pyx_t_11 = NULL;
         __pyx_t_4 = 0;
         #if CYTHON_UNPACK_METHODS
-        if (likely(PyMethod_Check(__pyx_t_3))) {
-          __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_3);
+        if (likely(PyMethod_Check(__pyx_t_7))) {
+          __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_7);
           if (likely(__pyx_t_11)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
             __Pyx_INCREF(__pyx_t_11);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_3, function);
+            __Pyx_DECREF_SET(__pyx_t_7, function);
             __pyx_t_4 = 1;
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_11, NULL};
-          __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+          __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
           __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
           if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+          __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         }
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
         /* "tactigon_speech/middleware/Tactigon_Speech.py":151
  *                 num_voiced = len([f for f, speech in ring_buffer if speech])
  *                 self.logger.debug("Got %i voiced frames. Threshold is %f", num_voiced, num_voiced_threshold)
  *                 if num_voiced >= num_voiced_threshold:             # <<<<<<<<<<<<<<
@@ -7695,40 +7732,40 @@
  * 
  *             else:
  *                 if self.is_timeout(ticks, self.voice_timeout):             # <<<<<<<<<<<<<<
  *                     self._is_timeout = True
  *                     break
  */
     /*else*/ {
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_is_timeout); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 159, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_is_timeout); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 159, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_voice_timeout); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 159, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
-      __pyx_t_2 = NULL;
+      __pyx_t_3 = NULL;
       __pyx_t_4 = 0;
       #if CYTHON_UNPACK_METHODS
-      if (likely(PyMethod_Check(__pyx_t_3))) {
-        __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-        if (likely(__pyx_t_2)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-          __Pyx_INCREF(__pyx_t_2);
+      if (likely(PyMethod_Check(__pyx_t_7))) {
+        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
+        if (likely(__pyx_t_3)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+          __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_3, function);
+          __Pyx_DECREF_SET(__pyx_t_7, function);
           __pyx_t_4 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_cur_scope->__pyx_v_ticks, __pyx_t_11};
-        __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
-        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+        PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_cur_scope->__pyx_v_ticks, __pyx_t_11};
+        __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
+        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 159, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (__pyx_t_6) {
 
         /* "tactigon_speech/middleware/Tactigon_Speech.py":160
  *             else:
@@ -7800,55 +7837,55 @@
  *                 self.logger.debug("Got %i unvoiced frames. Threshold is %f", num_unvoiced, num_voiced_threshold)
  *                 if num_unvoiced >= num_voiced_threshold:
  */
       { /* enter inner scope */
         __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_v_ring_buffer)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_v_ring_buffer)) {
-          __pyx_t_3 = __pyx_cur_scope->__pyx_v_ring_buffer; __Pyx_INCREF(__pyx_t_3);
-          __pyx_t_7 = 0;
+          __pyx_t_7 = __pyx_cur_scope->__pyx_v_ring_buffer; __Pyx_INCREF(__pyx_t_7);
+          __pyx_t_8 = 0;
           __pyx_t_10 = NULL;
         } else {
-          __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_cur_scope->__pyx_v_ring_buffer); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_10 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 165, __pyx_L1_error)
+          __pyx_t_8 = -1; __pyx_t_7 = PyObject_GetIter(__pyx_cur_scope->__pyx_v_ring_buffer); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 165, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_7);
+          __pyx_t_10 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 165, __pyx_L1_error)
         }
         for (;;) {
           if (likely(!__pyx_t_10)) {
-            if (likely(PyList_CheckExact(__pyx_t_3))) {
+            if (likely(PyList_CheckExact(__pyx_t_7))) {
               {
-                Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_3);
+                Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_7);
                 #if !CYTHON_ASSUME_SAFE_MACROS
                 if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 165, __pyx_L1_error)
                 #endif
-                if (__pyx_t_7 >= __pyx_temp) break;
+                if (__pyx_t_8 >= __pyx_temp) break;
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_11 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_11); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 165, __pyx_L1_error)
+              __pyx_t_11 = PyList_GET_ITEM(__pyx_t_7, __pyx_t_8); __Pyx_INCREF(__pyx_t_11); __pyx_t_8++; if (unlikely((0 < 0))) __PYX_ERR(0, 165, __pyx_L1_error)
               #else
-              __pyx_t_11 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 165, __pyx_L1_error)
+              __pyx_t_11 = __Pyx_PySequence_ITEM(__pyx_t_7, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 165, __pyx_L1_error)
               __Pyx_GOTREF(__pyx_t_11);
               #endif
             } else {
               {
-                Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_3);
+                Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_7);
                 #if !CYTHON_ASSUME_SAFE_MACROS
                 if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 165, __pyx_L1_error)
                 #endif
-                if (__pyx_t_7 >= __pyx_temp) break;
+                if (__pyx_t_8 >= __pyx_temp) break;
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_11 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_11); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 165, __pyx_L1_error)
+              __pyx_t_11 = PyTuple_GET_ITEM(__pyx_t_7, __pyx_t_8); __Pyx_INCREF(__pyx_t_11); __pyx_t_8++; if (unlikely((0 < 0))) __PYX_ERR(0, 165, __pyx_L1_error)
               #else
-              __pyx_t_11 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 165, __pyx_L1_error)
+              __pyx_t_11 = __Pyx_PySequence_ITEM(__pyx_t_7, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 165, __pyx_L1_error)
               __Pyx_GOTREF(__pyx_t_11);
               #endif
             }
           } else {
-            __pyx_t_11 = __pyx_t_10(__pyx_t_3);
+            __pyx_t_11 = __pyx_t_10(__pyx_t_7);
             if (unlikely(!__pyx_t_11)) {
               PyObject* exc_type = PyErr_Occurred();
               if (exc_type) {
                 if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
                 else __PYX_ERR(0, 165, __pyx_L1_error)
               }
               break;
@@ -7861,103 +7898,103 @@
             if (unlikely(size != 2)) {
               if (size > 2) __Pyx_RaiseTooManyValuesError(2);
               else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
               __PYX_ERR(0, 165, __pyx_L1_error)
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
             if (likely(PyTuple_CheckExact(sequence))) {
-              __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
-              __pyx_t_8 = PyTuple_GET_ITEM(sequence, 1); 
+              __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
+              __pyx_t_2 = PyTuple_GET_ITEM(sequence, 1); 
             } else {
-              __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
-              __pyx_t_8 = PyList_GET_ITEM(sequence, 1); 
+              __pyx_t_3 = PyList_GET_ITEM(sequence, 0); 
+              __pyx_t_2 = PyList_GET_ITEM(sequence, 1); 
             }
+            __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(__pyx_t_2);
-            __Pyx_INCREF(__pyx_t_8);
             #else
-            __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
+            __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_3);
+            __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_2);
-            __pyx_t_8 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 165, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_8);
             #endif
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
           } else {
             Py_ssize_t index = -1;
             __pyx_t_12 = PyObject_GetIter(__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 165, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_12);
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
             __pyx_t_13 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_12);
-            index = 0; __pyx_t_2 = __pyx_t_13(__pyx_t_12); if (unlikely(!__pyx_t_2)) goto __pyx_L28_unpacking_failed;
+            index = 0; __pyx_t_3 = __pyx_t_13(__pyx_t_12); if (unlikely(!__pyx_t_3)) goto __pyx_L28_unpacking_failed;
+            __Pyx_GOTREF(__pyx_t_3);
+            index = 1; __pyx_t_2 = __pyx_t_13(__pyx_t_12); if (unlikely(!__pyx_t_2)) goto __pyx_L28_unpacking_failed;
             __Pyx_GOTREF(__pyx_t_2);
-            index = 1; __pyx_t_8 = __pyx_t_13(__pyx_t_12); if (unlikely(!__pyx_t_8)) goto __pyx_L28_unpacking_failed;
-            __Pyx_GOTREF(__pyx_t_8);
             if (__Pyx_IternextUnpackEndCheck(__pyx_t_13(__pyx_t_12), 2) < 0) __PYX_ERR(0, 165, __pyx_L1_error)
             __pyx_t_13 = NULL;
             __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
             goto __pyx_L29_unpacking_done;
             __pyx_L28_unpacking_failed:;
             __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
             __pyx_t_13 = NULL;
             if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
             __PYX_ERR(0, 165, __pyx_L1_error)
             __pyx_L29_unpacking_done:;
           }
           __Pyx_XGOTREF(__pyx_cur_scope->__pyx_8genexpr1__pyx_v_f);
-          __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_8genexpr1__pyx_v_f, __pyx_t_2);
+          __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_8genexpr1__pyx_v_f, __pyx_t_3);
+          __Pyx_GIVEREF(__pyx_t_3);
+          __pyx_t_3 = 0;
+          __Pyx_XGOTREF(__pyx_cur_scope->__pyx_8genexpr1__pyx_v_speech);
+          __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_8genexpr1__pyx_v_speech, __pyx_t_2);
           __Pyx_GIVEREF(__pyx_t_2);
           __pyx_t_2 = 0;
-          __Pyx_XGOTREF(__pyx_cur_scope->__pyx_8genexpr1__pyx_v_speech);
-          __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_8genexpr1__pyx_v_speech, __pyx_t_8);
-          __Pyx_GIVEREF(__pyx_t_8);
-          __pyx_t_8 = 0;
           __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_8genexpr1__pyx_v_speech); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 165, __pyx_L1_error)
           __pyx_t_5 = (!__pyx_t_6);
           if (__pyx_t_5) {
             if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_cur_scope->__pyx_8genexpr1__pyx_v_f))) __PYX_ERR(0, 165, __pyx_L1_error)
           }
         }
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } /* exit inner scope */
-      __pyx_t_7 = __Pyx_PyList_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 165, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyList_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 165, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_cur_scope->__pyx_v_num_unvoiced = __pyx_t_7;
+      __pyx_cur_scope->__pyx_v_num_unvoiced = __pyx_t_8;
 
       /* "tactigon_speech/middleware/Tactigon_Speech.py":166
  *                 ring_buffer.append((frame, is_speech))
  *                 num_unvoiced = len([f for f, speech in ring_buffer if not speech])
  *                 self.logger.debug("Got %i unvoiced frames. Threshold is %f", num_unvoiced, num_voiced_threshold)             # <<<<<<<<<<<<<<
  *                 if num_unvoiced >= num_voiced_threshold:
  *                     break
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 166, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_debug); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 166, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 166, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_debug); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 166, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = PyInt_FromSsize_t(__pyx_cur_scope->__pyx_v_num_unvoiced); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 166, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_8 = NULL;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __pyx_t_7 = PyInt_FromSsize_t(__pyx_cur_scope->__pyx_v_num_unvoiced); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 166, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_2 = NULL;
       __pyx_t_4 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_11))) {
-        __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_11);
-        if (likely(__pyx_t_8)) {
+        __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_11);
+        if (likely(__pyx_t_2)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
-          __Pyx_INCREF(__pyx_t_8);
+          __Pyx_INCREF(__pyx_t_2);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_11, function);
           __pyx_t_4 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[4] = {__pyx_t_8, __pyx_kp_s_Got_i_unvoiced_frames_Threshold, __pyx_t_3, __pyx_cur_scope->__pyx_v_num_voiced_threshold};
+        PyObject *__pyx_callargs[4] = {__pyx_t_2, __pyx_kp_s_Got_i_unvoiced_frames_Threshold, __pyx_t_7, __pyx_cur_scope->__pyx_v_num_voiced_threshold};
         __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_11, __pyx_callargs+1-__pyx_t_4, 3+__pyx_t_4);
-        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
       /* "tactigon_speech/middleware/Tactigon_Speech.py":167
@@ -8015,32 +8052,32 @@
  * 
  *         ring_buffer.clear()             # <<<<<<<<<<<<<<
  *         return None
  * 
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_ring_buffer, __pyx_n_s_clear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = NULL;
+  __pyx_t_7 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
-    if (likely(__pyx_t_3)) {
+    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
       __pyx_t_4 = 1;
     }
   }
   #endif
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
+    PyObject *__pyx_callargs[2] = {__pyx_t_7, NULL};
     __pyx_t_11 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 172, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
   /* "tactigon_speech/middleware/Tactigon_Speech.py":173
@@ -8051,29 +8088,29 @@
  *     def run(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_r = NULL;
   goto __pyx_L0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":116
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":115
  *         return (millis() - tick).total_seconds() > timeout
  * 
  *     def vad_collector(self) -> Generator[bytes, bytes, None]:             # <<<<<<<<<<<<<<
  *         frame_length = int(2 * self._SAMPLE_RATE * self.vad_frame / 1000)
  *         num_padding_frames: int = int(frame_length * (self.vad_padding_ms / 10000))
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_Generator_Replace_StopIteration(0);
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_AddTraceback("vad_collector", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
   #if !CYTHON_USE_EXC_INFO_STACK
   __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
@@ -8185,15 +8222,15 @@
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_19run(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
-  PyObject *__pyx_v_last_command = NULL;
+  PyObject *__pyx_v_current_command = NULL;
   PyObject *__pyx_v_transcription = NULL;
   PyObject *__pyx_v_speech_tree = NULL;
   PyObject *__pyx_v_e = NULL;
   PyObject *__pyx_v_filename = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -8204,29 +8241,26 @@
   int __pyx_t_6;
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
-  PyObject *__pyx_t_13 = NULL;
-  PyObject *__pyx_t_14 = NULL;
+  int __pyx_t_13;
+  char const *__pyx_t_14;
   PyObject *__pyx_t_15 = NULL;
-  int __pyx_t_16;
-  char const *__pyx_t_17;
+  PyObject *__pyx_t_16 = NULL;
+  PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
   PyObject *__pyx_t_19 = NULL;
   PyObject *__pyx_t_20 = NULL;
-  PyObject *__pyx_t_21 = NULL;
-  PyObject *__pyx_t_22 = NULL;
-  PyObject *__pyx_t_23 = NULL;
+  char const *__pyx_t_21;
+  int __pyx_t_22;
+  char const *__pyx_t_23;
   char const *__pyx_t_24;
-  int __pyx_t_25;
-  char const *__pyx_t_26;
-  char const *__pyx_t_27;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("run", 1);
 
   /* "tactigon_speech/middleware/Tactigon_Speech.py":176
  * 
@@ -8727,48 +8761,36 @@
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "tactigon_speech/middleware/Tactigon_Speech.py":196
  *         self.logger.debug("Running!")
  * 
  *         self.command = Command.NONE             # <<<<<<<<<<<<<<
- *         last_command = self.command
  * 
+ *         while not self._stop_event.is_set():
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Command); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_NONE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_command_2, __pyx_t_3) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":197
- * 
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":198
  *         self.command = Command.NONE
- *         last_command = self.command             # <<<<<<<<<<<<<<
- * 
- *         while not self._stop_event.is_set():
- */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_v_last_command = __pyx_t_3;
-  __pyx_t_3 = 0;
-
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":199
- *         last_command = self.command
  * 
  *         while not self._stop_event.is_set():             # <<<<<<<<<<<<<<
- *             if last_command is self.command:
- *                 time.sleep(self._TICK)
+ *             current_command = self.command
+ * 
  */
   while (1) {
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_stop_event); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_stop_event); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 198, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_is_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_is_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
@@ -8781,50 +8803,65 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
-    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 198, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_7 = (!__pyx_t_6);
     if (!__pyx_t_7) break;
 
-    /* "tactigon_speech/middleware/Tactigon_Speech.py":200
+    /* "tactigon_speech/middleware/Tactigon_Speech.py":199
  * 
  *         while not self._stop_event.is_set():
- *             if last_command is self.command:             # <<<<<<<<<<<<<<
+ *             current_command = self.command             # <<<<<<<<<<<<<<
+ * 
+ *             if current_command is Command.NONE:
+ */
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_XDECREF_SET(__pyx_v_current_command, __pyx_t_3);
+    __pyx_t_3 = 0;
+
+    /* "tactigon_speech/middleware/Tactigon_Speech.py":201
+ *             current_command = self.command
+ * 
+ *             if current_command is Command.NONE:             # <<<<<<<<<<<<<<
  *                 time.sleep(self._TICK)
  *                 continue
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 200, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Command); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = (__pyx_v_last_command == __pyx_t_3);
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_NONE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_7 = (__pyx_v_current_command == __pyx_t_2);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (__pyx_t_7) {
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":201
- *         while not self._stop_event.is_set():
- *             if last_command is self.command:
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":202
+ * 
+ *             if current_command is Command.NONE:
  *                 time.sleep(self._TICK)             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_sleep); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 202, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sleep); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 202, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_TICK); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_TICK); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 202, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_5 = NULL;
       __pyx_t_4 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -8832,214 +8869,229 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
           __pyx_t_4 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_2};
-        __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+        PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_3};
+        __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 201, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 202, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":202
- *             if last_command is self.command:
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":203
+ *             if current_command is Command.NONE:
  *                 time.sleep(self._TICK)
  *                 continue             # <<<<<<<<<<<<<<
  * 
- *             last_command = self.command
+ *             if current_command == Command.LISTEN:
  */
       goto __pyx_L4_continue;
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":200
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":201
+ *             current_command = self.command
  * 
- *         while not self._stop_event.is_set():
- *             if last_command is self.command:             # <<<<<<<<<<<<<<
+ *             if current_command is Command.NONE:             # <<<<<<<<<<<<<<
  *                 time.sleep(self._TICK)
  *                 continue
  */
     }
 
-    /* "tactigon_speech/middleware/Tactigon_Speech.py":204
+    /* "tactigon_speech/middleware/Tactigon_Speech.py":205
  *                 continue
  * 
- *             last_command = self.command             # <<<<<<<<<<<<<<
- * 
- *             if last_command == Command.LISTEN:
- */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_command_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 204, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF_SET(__pyx_v_last_command, __pyx_t_3);
-    __pyx_t_3 = 0;
-
-    /* "tactigon_speech/middleware/Tactigon_Speech.py":206
- *             last_command = self.command
- * 
- *             if last_command == Command.LISTEN:             # <<<<<<<<<<<<<<
+ *             if current_command == Command.LISTEN:             # <<<<<<<<<<<<<<
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
- *                     transcription = None
+ *                     transcription = Transcription("", [], 0, False)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Command); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 206, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_LISTEN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Command); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 205, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_LISTEN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyObject_RichCompare(__pyx_v_last_command, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 206, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = PyObject_RichCompare(__pyx_v_current_command, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 206, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 205, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (__pyx_t_7) {
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":207
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":206
  * 
- *             if last_command == Command.LISTEN:
+ *             if current_command == Command.LISTEN:
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):             # <<<<<<<<<<<<<<
- *                     transcription = None
+ *                     transcription = Transcription("", [], 0, False)
  *                     try:
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_poll); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_poll); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 206, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_INTERFACE_TIMEOUT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_INTERFACE_TIMEOUT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_5 = NULL;
       __pyx_t_4 = 0;
       #if CYTHON_UNPACK_METHODS
-      if (likely(PyMethod_Check(__pyx_t_2))) {
-        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_5)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_2, function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
           __pyx_t_4 = 1;
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_1};
-        __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+        __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 207, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
-      __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 207, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 206, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_7) {
 
-        /* "tactigon_speech/middleware/Tactigon_Speech.py":208
- *             if last_command == Command.LISTEN:
+        /* "tactigon_speech/middleware/Tactigon_Speech.py":207
+ *             if current_command == Command.LISTEN:
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
- *                     transcription = None             # <<<<<<<<<<<<<<
+ *                     transcription = Transcription("", [], 0, False)             # <<<<<<<<<<<<<<
  *                     try:
  *                         speech_tree: TSpeechObject = self.interface.recv()
  */
-        __Pyx_INCREF(Py_None);
-        __Pyx_XDECREF_SET(__pyx_v_transcription, Py_None);
+        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Transcription); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 207, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_5 = NULL;
+        __pyx_t_4 = 0;
+        #if CYTHON_UNPACK_METHODS
+        if (unlikely(PyMethod_Check(__pyx_t_3))) {
+          __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+          if (likely(__pyx_t_5)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+            __Pyx_INCREF(__pyx_t_5);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_3, function);
+            __pyx_t_4 = 1;
+          }
+        }
+        #endif
+        {
+          PyObject *__pyx_callargs[5] = {__pyx_t_5, __pyx_kp_s__3, __pyx_t_1, __pyx_int_0, Py_False};
+          __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 4+__pyx_t_4);
+          __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        }
+        __Pyx_XDECREF_SET(__pyx_v_transcription, __pyx_t_2);
+        __pyx_t_2 = 0;
 
-        /* "tactigon_speech/middleware/Tactigon_Speech.py":209
+        /* "tactigon_speech/middleware/Tactigon_Speech.py":208
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
- *                     transcription = None
+ *                     transcription = Transcription("", [], 0, False)
  *                     try:             # <<<<<<<<<<<<<<
  *                         speech_tree: TSpeechObject = self.interface.recv()
  *                         transcription = self.stt(speech_tree)
  */
         /*try:*/ {
           {
             __Pyx_PyThreadState_declare
             __Pyx_PyThreadState_assign
             __Pyx_ExceptionSave(&__pyx_t_8, &__pyx_t_9, &__pyx_t_10);
             __Pyx_XGOTREF(__pyx_t_8);
             __Pyx_XGOTREF(__pyx_t_9);
             __Pyx_XGOTREF(__pyx_t_10);
             /*try:*/ {
 
-              /* "tactigon_speech/middleware/Tactigon_Speech.py":210
- *                     transcription = None
+              /* "tactigon_speech/middleware/Tactigon_Speech.py":209
+ *                     transcription = Transcription("", [], 0, False)
  *                     try:
  *                         speech_tree: TSpeechObject = self.interface.recv()             # <<<<<<<<<<<<<<
  *                         transcription = self.stt(speech_tree)
  *                     except (Exception) as e:
  */
-              __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 210, __pyx_L14_error)
-              __Pyx_GOTREF(__pyx_t_2);
-              __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_recv); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 210, __pyx_L14_error)
+              __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 209, __pyx_L14_error)
+              __Pyx_GOTREF(__pyx_t_3);
+              __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_recv); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 209, __pyx_L14_error)
               __Pyx_GOTREF(__pyx_t_1);
-              __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-              __pyx_t_2 = NULL;
+              __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+              __pyx_t_3 = NULL;
               __pyx_t_4 = 0;
               #if CYTHON_UNPACK_METHODS
               if (likely(PyMethod_Check(__pyx_t_1))) {
-                __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
-                if (likely(__pyx_t_2)) {
+                __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
+                if (likely(__pyx_t_3)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-                  __Pyx_INCREF(__pyx_t_2);
+                  __Pyx_INCREF(__pyx_t_3);
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_1, function);
                   __pyx_t_4 = 1;
                 }
               }
               #endif
               {
-                PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
-                __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
-                __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-                if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L14_error)
-                __Pyx_GOTREF(__pyx_t_3);
+                PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
+                __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+                __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+                if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 209, __pyx_L14_error)
+                __Pyx_GOTREF(__pyx_t_2);
                 __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
               }
-              __Pyx_XDECREF_SET(__pyx_v_speech_tree, __pyx_t_3);
-              __pyx_t_3 = 0;
+              __Pyx_XDECREF_SET(__pyx_v_speech_tree, __pyx_t_2);
+              __pyx_t_2 = 0;
 
-              /* "tactigon_speech/middleware/Tactigon_Speech.py":211
+              /* "tactigon_speech/middleware/Tactigon_Speech.py":210
  *                     try:
  *                         speech_tree: TSpeechObject = self.interface.recv()
  *                         transcription = self.stt(speech_tree)             # <<<<<<<<<<<<<<
  *                     except (Exception) as e:
- *                         self.interface.send(Transcription("", [], 0, False))
+ *                         self.logger.warning("[TSpeech] Exception while listening. %s", e)
  */
-              __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_stt); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L14_error)
+              __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_stt); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 210, __pyx_L14_error)
               __Pyx_GOTREF(__pyx_t_1);
-              __pyx_t_2 = NULL;
+              __pyx_t_3 = NULL;
               __pyx_t_4 = 0;
               #if CYTHON_UNPACK_METHODS
               if (likely(PyMethod_Check(__pyx_t_1))) {
-                __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
-                if (likely(__pyx_t_2)) {
+                __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
+                if (likely(__pyx_t_3)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-                  __Pyx_INCREF(__pyx_t_2);
+                  __Pyx_INCREF(__pyx_t_3);
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_1, function);
                   __pyx_t_4 = 1;
                 }
               }
               #endif
               {
-                PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_speech_tree};
-                __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-                __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-                if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 211, __pyx_L14_error)
-                __Pyx_GOTREF(__pyx_t_3);
+                PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_speech_tree};
+                __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+                __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+                if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 210, __pyx_L14_error)
+                __Pyx_GOTREF(__pyx_t_2);
                 __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
               }
-              __Pyx_DECREF_SET(__pyx_v_transcription, __pyx_t_3);
-              __pyx_t_3 = 0;
+              __Pyx_DECREF_SET(__pyx_v_transcription, __pyx_t_2);
+              __pyx_t_2 = 0;
 
-              /* "tactigon_speech/middleware/Tactigon_Speech.py":209
+              /* "tactigon_speech/middleware/Tactigon_Speech.py":208
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
- *                     transcription = None
+ *                     transcription = Transcription("", [], 0, False)
  *                     try:             # <<<<<<<<<<<<<<
  *                         speech_tree: TSpeechObject = self.interface.recv()
  *                         transcription = self.stt(speech_tree)
  */
             }
             __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
             __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
@@ -9047,194 +9099,127 @@
             goto __pyx_L21_try_end;
             __pyx_L14_error:;
             __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
             __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-            /* "tactigon_speech/middleware/Tactigon_Speech.py":212
+            /* "tactigon_speech/middleware/Tactigon_Speech.py":211
  *                         speech_tree: TSpeechObject = self.interface.recv()
  *                         transcription = self.stt(speech_tree)
  *                     except (Exception) as e:             # <<<<<<<<<<<<<<
- *                         self.interface.send(Transcription("", [], 0, False))
- *                         self.logger.info("[TSpeech] Exception while listening. %s", e)
+ *                         self.logger.warning("[TSpeech] Exception while listening. %s", e)
+ *                     finally:
  */
             __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
             if (__pyx_t_4) {
               __Pyx_AddTraceback("tactigon_speech.middleware.Tactigon_Speech.Tactigon_Speech.run", __pyx_clineno, __pyx_lineno, __pyx_filename);
-              if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_1, &__pyx_t_2) < 0) __PYX_ERR(0, 212, __pyx_L16_except_error)
-              __Pyx_XGOTREF(__pyx_t_3);
-              __Pyx_XGOTREF(__pyx_t_1);
+              if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_1, &__pyx_t_3) < 0) __PYX_ERR(0, 211, __pyx_L16_except_error)
               __Pyx_XGOTREF(__pyx_t_2);
+              __Pyx_XGOTREF(__pyx_t_1);
+              __Pyx_XGOTREF(__pyx_t_3);
               __Pyx_INCREF(__pyx_t_1);
               __pyx_v_e = __pyx_t_1;
               /*try:*/ {
 
-                /* "tactigon_speech/middleware/Tactigon_Speech.py":213
+                /* "tactigon_speech/middleware/Tactigon_Speech.py":212
  *                         transcription = self.stt(speech_tree)
  *                     except (Exception) as e:
- *                         self.interface.send(Transcription("", [], 0, False))             # <<<<<<<<<<<<<<
- *                         self.logger.info("[TSpeech] Exception while listening. %s", e)
+ *                         self.logger.warning("[TSpeech] Exception while listening. %s", e)             # <<<<<<<<<<<<<<
  *                     finally:
+ *                         self.interface.send(InterfaceObject(current_command, transcription))
  */
-                __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 213, __pyx_L27_error)
+                __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 212, __pyx_L27_error)
                 __Pyx_GOTREF(__pyx_t_11);
-                __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_send); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 213, __pyx_L27_error)
+                __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_warning); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 212, __pyx_L27_error)
                 __Pyx_GOTREF(__pyx_t_12);
                 __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-                __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_Transcription); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 213, __pyx_L27_error)
-                __Pyx_GOTREF(__pyx_t_13);
-                __pyx_t_14 = PyList_New(0); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 213, __pyx_L27_error)
-                __Pyx_GOTREF(__pyx_t_14);
-                __pyx_t_15 = NULL;
-                __pyx_t_4 = 0;
-                #if CYTHON_UNPACK_METHODS
-                if (unlikely(PyMethod_Check(__pyx_t_13))) {
-                  __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_13);
-                  if (likely(__pyx_t_15)) {
-                    PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
-                    __Pyx_INCREF(__pyx_t_15);
-                    __Pyx_INCREF(function);
-                    __Pyx_DECREF_SET(__pyx_t_13, function);
-                    __pyx_t_4 = 1;
-                  }
-                }
-                #endif
-                {
-                  PyObject *__pyx_callargs[5] = {__pyx_t_15, __pyx_kp_s__3, __pyx_t_14, __pyx_int_0, Py_False};
-                  __pyx_t_11 = __Pyx_PyObject_FastCall(__pyx_t_13, __pyx_callargs+1-__pyx_t_4, 4+__pyx_t_4);
-                  __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-                  __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-                  if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 213, __pyx_L27_error)
-                  __Pyx_GOTREF(__pyx_t_11);
-                  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-                }
-                __pyx_t_13 = NULL;
+                __pyx_t_11 = NULL;
                 __pyx_t_4 = 0;
                 #if CYTHON_UNPACK_METHODS
                 if (likely(PyMethod_Check(__pyx_t_12))) {
-                  __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_12);
-                  if (likely(__pyx_t_13)) {
+                  __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_12);
+                  if (likely(__pyx_t_11)) {
                     PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
-                    __Pyx_INCREF(__pyx_t_13);
+                    __Pyx_INCREF(__pyx_t_11);
                     __Pyx_INCREF(function);
                     __Pyx_DECREF_SET(__pyx_t_12, function);
                     __pyx_t_4 = 1;
                   }
                 }
                 #endif
                 {
-                  PyObject *__pyx_callargs[2] = {__pyx_t_13, __pyx_t_11};
-                  __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_12, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-                  __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-                  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-                  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 213, __pyx_L27_error)
+                  PyObject *__pyx_callargs[3] = {__pyx_t_11, __pyx_kp_s_TSpeech_Exception_while_listeni, __pyx_v_e};
+                  __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_12, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
+                  __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+                  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 212, __pyx_L27_error)
                   __Pyx_GOTREF(__pyx_t_5);
                   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
                 }
                 __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-
-                /* "tactigon_speech/middleware/Tactigon_Speech.py":214
- *                     except (Exception) as e:
- *                         self.interface.send(Transcription("", [], 0, False))
- *                         self.logger.info("[TSpeech] Exception while listening. %s", e)             # <<<<<<<<<<<<<<
- *                     finally:
- *                         self.interface.send(transcription)
- */
-                __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 214, __pyx_L27_error)
-                __Pyx_GOTREF(__pyx_t_12);
-                __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_info); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 214, __pyx_L27_error)
-                __Pyx_GOTREF(__pyx_t_11);
-                __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-                __pyx_t_12 = NULL;
-                __pyx_t_4 = 0;
-                #if CYTHON_UNPACK_METHODS
-                if (likely(PyMethod_Check(__pyx_t_11))) {
-                  __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
-                  if (likely(__pyx_t_12)) {
-                    PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
-                    __Pyx_INCREF(__pyx_t_12);
-                    __Pyx_INCREF(function);
-                    __Pyx_DECREF_SET(__pyx_t_11, function);
-                    __pyx_t_4 = 1;
-                  }
-                }
-                #endif
-                {
-                  PyObject *__pyx_callargs[3] = {__pyx_t_12, __pyx_kp_s_TSpeech_Exception_while_listeni, __pyx_v_e};
-                  __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_11, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
-                  __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-                  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 214, __pyx_L27_error)
-                  __Pyx_GOTREF(__pyx_t_5);
-                  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-                }
-                __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
               }
 
-              /* "tactigon_speech/middleware/Tactigon_Speech.py":212
+              /* "tactigon_speech/middleware/Tactigon_Speech.py":211
  *                         speech_tree: TSpeechObject = self.interface.recv()
  *                         transcription = self.stt(speech_tree)
  *                     except (Exception) as e:             # <<<<<<<<<<<<<<
- *                         self.interface.send(Transcription("", [], 0, False))
- *                         self.logger.info("[TSpeech] Exception while listening. %s", e)
+ *                         self.logger.warning("[TSpeech] Exception while listening. %s", e)
+ *                     finally:
  */
               /*finally:*/ {
                 /*normal exit:*/{
                   __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
                   goto __pyx_L28;
                 }
                 __pyx_L27_error:;
                 /*exception exit:*/{
                   __Pyx_PyThreadState_declare
                   __Pyx_PyThreadState_assign
-                  __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0;
+                  __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0;
                   __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
                   __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-                  __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-                  __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-                  __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
                   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-                  if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_21, &__pyx_t_22, &__pyx_t_23);
-                  if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_18, &__pyx_t_19, &__pyx_t_20) < 0)) __Pyx_ErrFetch(&__pyx_t_18, &__pyx_t_19, &__pyx_t_20);
+                  if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_18, &__pyx_t_19, &__pyx_t_20);
+                  if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_15, &__pyx_t_16, &__pyx_t_17) < 0)) __Pyx_ErrFetch(&__pyx_t_15, &__pyx_t_16, &__pyx_t_17);
+                  __Pyx_XGOTREF(__pyx_t_15);
+                  __Pyx_XGOTREF(__pyx_t_16);
+                  __Pyx_XGOTREF(__pyx_t_17);
                   __Pyx_XGOTREF(__pyx_t_18);
                   __Pyx_XGOTREF(__pyx_t_19);
                   __Pyx_XGOTREF(__pyx_t_20);
-                  __Pyx_XGOTREF(__pyx_t_21);
-                  __Pyx_XGOTREF(__pyx_t_22);
-                  __Pyx_XGOTREF(__pyx_t_23);
-                  __pyx_t_4 = __pyx_lineno; __pyx_t_16 = __pyx_clineno; __pyx_t_17 = __pyx_filename;
+                  __pyx_t_4 = __pyx_lineno; __pyx_t_13 = __pyx_clineno; __pyx_t_14 = __pyx_filename;
                   {
                     __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
                   }
                   if (PY_MAJOR_VERSION >= 3) {
-                    __Pyx_XGIVEREF(__pyx_t_21);
-                    __Pyx_XGIVEREF(__pyx_t_22);
-                    __Pyx_XGIVEREF(__pyx_t_23);
-                    __Pyx_ExceptionReset(__pyx_t_21, __pyx_t_22, __pyx_t_23);
+                    __Pyx_XGIVEREF(__pyx_t_18);
+                    __Pyx_XGIVEREF(__pyx_t_19);
+                    __Pyx_XGIVEREF(__pyx_t_20);
+                    __Pyx_ExceptionReset(__pyx_t_18, __pyx_t_19, __pyx_t_20);
                   }
-                  __Pyx_XGIVEREF(__pyx_t_18);
-                  __Pyx_XGIVEREF(__pyx_t_19);
-                  __Pyx_XGIVEREF(__pyx_t_20);
-                  __Pyx_ErrRestore(__pyx_t_18, __pyx_t_19, __pyx_t_20);
-                  __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0;
-                  __pyx_lineno = __pyx_t_4; __pyx_clineno = __pyx_t_16; __pyx_filename = __pyx_t_17;
+                  __Pyx_XGIVEREF(__pyx_t_15);
+                  __Pyx_XGIVEREF(__pyx_t_16);
+                  __Pyx_XGIVEREF(__pyx_t_17);
+                  __Pyx_ErrRestore(__pyx_t_15, __pyx_t_16, __pyx_t_17);
+                  __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0;
+                  __pyx_lineno = __pyx_t_4; __pyx_clineno = __pyx_t_13; __pyx_filename = __pyx_t_14;
                   goto __pyx_L16_except_error;
                 }
                 __pyx_L28:;
               }
-              __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-              __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
               __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+              __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+              __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
               goto __pyx_L15_exception_handled;
             }
             goto __pyx_L16_except_error;
 
-            /* "tactigon_speech/middleware/Tactigon_Speech.py":209
+            /* "tactigon_speech/middleware/Tactigon_Speech.py":208
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
- *                     transcription = None
+ *                     transcription = Transcription("", [], 0, False)
  *                     try:             # <<<<<<<<<<<<<<
  *                         speech_tree: TSpeechObject = self.interface.recv()
  *                         transcription = self.stt(speech_tree)
  */
             __pyx_L16_except_error:;
             __Pyx_XGIVEREF(__pyx_t_8);
             __Pyx_XGIVEREF(__pyx_t_9);
@@ -9246,1154 +9231,1382 @@
             __Pyx_XGIVEREF(__pyx_t_9);
             __Pyx_XGIVEREF(__pyx_t_10);
             __Pyx_ExceptionReset(__pyx_t_8, __pyx_t_9, __pyx_t_10);
             __pyx_L21_try_end:;
           }
         }
 
-        /* "tactigon_speech/middleware/Tactigon_Speech.py":216
- *                         self.logger.info("[TSpeech] Exception while listening. %s", e)
+        /* "tactigon_speech/middleware/Tactigon_Speech.py":214
+ *                         self.logger.warning("[TSpeech] Exception while listening. %s", e)
  *                     finally:
- *                         self.interface.send(transcription)             # <<<<<<<<<<<<<<
+ *                         self.interface.send(InterfaceObject(current_command, transcription))             # <<<<<<<<<<<<<<
  *                 else:
  *                     self.logger.error("Listen command received, but no tspeech from interface pipe.")
  */
         /*finally:*/ {
           /*normal exit:*/{
-            __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+            __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_1);
-            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_send); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 216, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_3);
+            __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_send); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_2);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-            __pyx_t_1 = NULL;
-            __pyx_t_16 = 0;
+            __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InterfaceObject); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 214, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_5);
+            __pyx_t_12 = NULL;
+            __pyx_t_13 = 0;
             #if CYTHON_UNPACK_METHODS
-            if (likely(PyMethod_Check(__pyx_t_3))) {
-              __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
-              if (likely(__pyx_t_1)) {
-                PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-                __Pyx_INCREF(__pyx_t_1);
+            if (unlikely(PyMethod_Check(__pyx_t_5))) {
+              __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_5);
+              if (likely(__pyx_t_12)) {
+                PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+                __Pyx_INCREF(__pyx_t_12);
                 __Pyx_INCREF(function);
-                __Pyx_DECREF_SET(__pyx_t_3, function);
-                __pyx_t_16 = 1;
+                __Pyx_DECREF_SET(__pyx_t_5, function);
+                __pyx_t_13 = 1;
               }
             }
             #endif
             {
-              PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_v_transcription};
-              __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_16, 1+__pyx_t_16);
-              __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-              if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 216, __pyx_L1_error)
-              __Pyx_GOTREF(__pyx_t_2);
-              __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+              PyObject *__pyx_callargs[3] = {__pyx_t_12, __pyx_v_current_command, __pyx_v_transcription};
+              __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_13, 2+__pyx_t_13);
+              __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+              if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L1_error)
+              __Pyx_GOTREF(__pyx_t_1);
+              __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
             }
-            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+            __pyx_t_5 = NULL;
+            __pyx_t_13 = 0;
+            #if CYTHON_UNPACK_METHODS
+            if (likely(PyMethod_Check(__pyx_t_2))) {
+              __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
+              if (likely(__pyx_t_5)) {
+                PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+                __Pyx_INCREF(__pyx_t_5);
+                __Pyx_INCREF(function);
+                __Pyx_DECREF_SET(__pyx_t_2, function);
+                __pyx_t_13 = 1;
+              }
+            }
+            #endif
+            {
+              PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_1};
+              __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_13, 1+__pyx_t_13);
+              __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+              __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+              if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 214, __pyx_L1_error)
+              __Pyx_GOTREF(__pyx_t_3);
+              __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+            }
+            __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
             goto __pyx_L13;
           }
           __pyx_L12_error:;
           /*exception exit:*/{
             __Pyx_PyThreadState_declare
             __Pyx_PyThreadState_assign
-            __pyx_t_10 = 0; __pyx_t_9 = 0; __pyx_t_8 = 0; __pyx_t_23 = 0; __pyx_t_22 = 0; __pyx_t_21 = 0;
+            __pyx_t_10 = 0; __pyx_t_9 = 0; __pyx_t_8 = 0; __pyx_t_20 = 0; __pyx_t_19 = 0; __pyx_t_18 = 0;
             __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
             __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-            __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-            __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-            __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
             __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
             __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-            if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_23, &__pyx_t_22, &__pyx_t_21);
+            if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_20, &__pyx_t_19, &__pyx_t_18);
             if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_10, &__pyx_t_9, &__pyx_t_8) < 0)) __Pyx_ErrFetch(&__pyx_t_10, &__pyx_t_9, &__pyx_t_8);
             __Pyx_XGOTREF(__pyx_t_10);
             __Pyx_XGOTREF(__pyx_t_9);
             __Pyx_XGOTREF(__pyx_t_8);
-            __Pyx_XGOTREF(__pyx_t_23);
-            __Pyx_XGOTREF(__pyx_t_22);
-            __Pyx_XGOTREF(__pyx_t_21);
-            __pyx_t_16 = __pyx_lineno; __pyx_t_4 = __pyx_clineno; __pyx_t_24 = __pyx_filename;
+            __Pyx_XGOTREF(__pyx_t_20);
+            __Pyx_XGOTREF(__pyx_t_19);
+            __Pyx_XGOTREF(__pyx_t_18);
+            __pyx_t_13 = __pyx_lineno; __pyx_t_4 = __pyx_clineno; __pyx_t_21 = __pyx_filename;
             {
-              __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 216, __pyx_L36_error)
-              __Pyx_GOTREF(__pyx_t_3);
-              __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_send); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L36_error)
+              __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L36_error)
+              __Pyx_GOTREF(__pyx_t_2);
+              __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_send); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L36_error)
               __Pyx_GOTREF(__pyx_t_1);
-              __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-              __pyx_t_3 = NULL;
-              __pyx_t_25 = 0;
+              __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+              __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InterfaceObject); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 214, __pyx_L36_error)
+              __Pyx_GOTREF(__pyx_t_5);
+              __pyx_t_12 = NULL;
+              __pyx_t_22 = 0;
+              #if CYTHON_UNPACK_METHODS
+              if (unlikely(PyMethod_Check(__pyx_t_5))) {
+                __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_5);
+                if (likely(__pyx_t_12)) {
+                  PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+                  __Pyx_INCREF(__pyx_t_12);
+                  __Pyx_INCREF(function);
+                  __Pyx_DECREF_SET(__pyx_t_5, function);
+                  __pyx_t_22 = 1;
+                }
+              }
+              #endif
+              {
+                PyObject *__pyx_callargs[3] = {__pyx_t_12, __pyx_v_current_command, __pyx_v_transcription};
+                __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_22, 2+__pyx_t_22);
+                __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+                if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L36_error)
+                __Pyx_GOTREF(__pyx_t_2);
+                __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+              }
+              __pyx_t_5 = NULL;
+              __pyx_t_22 = 0;
               #if CYTHON_UNPACK_METHODS
               if (likely(PyMethod_Check(__pyx_t_1))) {
-                __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
-                if (likely(__pyx_t_3)) {
+                __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+                if (likely(__pyx_t_5)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-                  __Pyx_INCREF(__pyx_t_3);
+                  __Pyx_INCREF(__pyx_t_5);
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_1, function);
-                  __pyx_t_25 = 1;
+                  __pyx_t_22 = 1;
                 }
               }
               #endif
               {
-                PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_transcription};
-                __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_25, 1+__pyx_t_25);
-                __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-                if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 216, __pyx_L36_error)
-                __Pyx_GOTREF(__pyx_t_2);
+                PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_2};
+                __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_22, 1+__pyx_t_22);
+                __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+                __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+                if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 214, __pyx_L36_error)
+                __Pyx_GOTREF(__pyx_t_3);
                 __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
               }
-              __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+              __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
             }
             if (PY_MAJOR_VERSION >= 3) {
-              __Pyx_XGIVEREF(__pyx_t_23);
-              __Pyx_XGIVEREF(__pyx_t_22);
-              __Pyx_XGIVEREF(__pyx_t_21);
-              __Pyx_ExceptionReset(__pyx_t_23, __pyx_t_22, __pyx_t_21);
+              __Pyx_XGIVEREF(__pyx_t_20);
+              __Pyx_XGIVEREF(__pyx_t_19);
+              __Pyx_XGIVEREF(__pyx_t_18);
+              __Pyx_ExceptionReset(__pyx_t_20, __pyx_t_19, __pyx_t_18);
             }
             __Pyx_XGIVEREF(__pyx_t_10);
             __Pyx_XGIVEREF(__pyx_t_9);
             __Pyx_XGIVEREF(__pyx_t_8);
             __Pyx_ErrRestore(__pyx_t_10, __pyx_t_9, __pyx_t_8);
-            __pyx_t_10 = 0; __pyx_t_9 = 0; __pyx_t_8 = 0; __pyx_t_23 = 0; __pyx_t_22 = 0; __pyx_t_21 = 0;
-            __pyx_lineno = __pyx_t_16; __pyx_clineno = __pyx_t_4; __pyx_filename = __pyx_t_24;
+            __pyx_t_10 = 0; __pyx_t_9 = 0; __pyx_t_8 = 0; __pyx_t_20 = 0; __pyx_t_19 = 0; __pyx_t_18 = 0;
+            __pyx_lineno = __pyx_t_13; __pyx_clineno = __pyx_t_4; __pyx_filename = __pyx_t_21;
             goto __pyx_L1_error;
             __pyx_L36_error:;
             if (PY_MAJOR_VERSION >= 3) {
-              __Pyx_XGIVEREF(__pyx_t_23);
-              __Pyx_XGIVEREF(__pyx_t_22);
-              __Pyx_XGIVEREF(__pyx_t_21);
-              __Pyx_ExceptionReset(__pyx_t_23, __pyx_t_22, __pyx_t_21);
+              __Pyx_XGIVEREF(__pyx_t_20);
+              __Pyx_XGIVEREF(__pyx_t_19);
+              __Pyx_XGIVEREF(__pyx_t_18);
+              __Pyx_ExceptionReset(__pyx_t_20, __pyx_t_19, __pyx_t_18);
             }
             __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
             __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
             __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-            __pyx_t_23 = 0; __pyx_t_22 = 0; __pyx_t_21 = 0;
+            __pyx_t_20 = 0; __pyx_t_19 = 0; __pyx_t_18 = 0;
             goto __pyx_L1_error;
           }
           __pyx_L13:;
         }
 
-        /* "tactigon_speech/middleware/Tactigon_Speech.py":207
+        /* "tactigon_speech/middleware/Tactigon_Speech.py":206
  * 
- *             if last_command == Command.LISTEN:
+ *             if current_command == Command.LISTEN:
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):             # <<<<<<<<<<<<<<
- *                     transcription = None
+ *                     transcription = Transcription("", [], 0, False)
  *                     try:
  */
         goto __pyx_L8;
       }
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":218
- *                         self.interface.send(transcription)
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":216
+ *                         self.interface.send(InterfaceObject(current_command, transcription))
  *                 else:
  *                     self.logger.error("Listen command received, but no tspeech from interface pipe.")             # <<<<<<<<<<<<<<
- *                     self.interface.send(False)
- *             elif last_command == Command.PLAY:
+ *                     self.interface.send(InterfaceObject(current_command, False))
+ *             elif current_command == Command.PLAY:
  */
       /*else*/ {
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 218, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_error); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 218, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_error); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 216, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_t_1 = NULL;
         __pyx_t_4 = 0;
         #if CYTHON_UNPACK_METHODS
-        if (likely(PyMethod_Check(__pyx_t_3))) {
-          __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
+        if (likely(PyMethod_Check(__pyx_t_2))) {
+          __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_1)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_1);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_3, function);
+            __Pyx_DECREF_SET(__pyx_t_2, function);
             __pyx_t_4 = 1;
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_kp_s_Listen_command_received_but_no_t};
-          __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+          __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 218, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 216, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_3);
+          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         }
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "tactigon_speech/middleware/Tactigon_Speech.py":219
+        /* "tactigon_speech/middleware/Tactigon_Speech.py":217
  *                 else:
  *                     self.logger.error("Listen command received, but no tspeech from interface pipe.")
- *                     self.interface.send(False)             # <<<<<<<<<<<<<<
- *             elif last_command == Command.PLAY:
+ *                     self.interface.send(InterfaceObject(current_command, False))             # <<<<<<<<<<<<<<
+ *             elif current_command == Command.PLAY:
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
  */
-        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 219, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_send); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 217, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_send); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_3 = NULL;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InterfaceObject); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 217, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __pyx_t_12 = NULL;
+        __pyx_t_4 = 0;
+        #if CYTHON_UNPACK_METHODS
+        if (unlikely(PyMethod_Check(__pyx_t_5))) {
+          __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_5);
+          if (likely(__pyx_t_12)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+            __Pyx_INCREF(__pyx_t_12);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_5, function);
+            __pyx_t_4 = 1;
+          }
+        }
+        #endif
+        {
+          PyObject *__pyx_callargs[3] = {__pyx_t_12, __pyx_v_current_command, Py_False};
+          __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
+          __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 217, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        }
+        __pyx_t_5 = NULL;
         __pyx_t_4 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_1))) {
-          __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
-          if (likely(__pyx_t_3)) {
+          __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+          if (likely(__pyx_t_5)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-            __Pyx_INCREF(__pyx_t_3);
+            __Pyx_INCREF(__pyx_t_5);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_1, function);
             __pyx_t_4 = 1;
           }
         }
         #endif
         {
-          PyObject *__pyx_callargs[2] = {__pyx_t_3, Py_False};
-          __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-          __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 219, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
+          PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_2};
+          __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+          __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 217, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         }
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
       __pyx_L8:;
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":206
- *             last_command = self.command
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":205
+ *                 continue
  * 
- *             if last_command == Command.LISTEN:             # <<<<<<<<<<<<<<
+ *             if current_command == Command.LISTEN:             # <<<<<<<<<<<<<<
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
- *                     transcription = None
+ *                     transcription = Transcription("", [], 0, False)
  */
       goto __pyx_L7;
     }
 
-    /* "tactigon_speech/middleware/Tactigon_Speech.py":220
+    /* "tactigon_speech/middleware/Tactigon_Speech.py":218
  *                     self.logger.error("Listen command received, but no tspeech from interface pipe.")
- *                     self.interface.send(False)
- *             elif last_command == Command.PLAY:             # <<<<<<<<<<<<<<
+ *                     self.interface.send(InterfaceObject(current_command, False))
+ *             elif current_command == Command.PLAY:             # <<<<<<<<<<<<<<
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
- *                     filename = None
+ *                     filename = ""
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Command); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_PLAY); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Command); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_PLAY); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyObject_RichCompare(__pyx_v_last_command, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = PyObject_RichCompare(__pyx_v_current_command, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 220, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 218, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (__pyx_t_7) {
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":221
- *                     self.interface.send(False)
- *             elif last_command == Command.PLAY:
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":219
+ *                     self.interface.send(InterfaceObject(current_command, False))
+ *             elif current_command == Command.PLAY:
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):             # <<<<<<<<<<<<<<
- *                     filename = None
+ *                     filename = ""
  *                     try:
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_poll); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 221, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_poll); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 219, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_INTERFACE_TIMEOUT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_INTERFACE_TIMEOUT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_5 = NULL;
       __pyx_t_4 = 0;
       #if CYTHON_UNPACK_METHODS
-      if (likely(PyMethod_Check(__pyx_t_3))) {
-        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(PyMethod_Check(__pyx_t_2))) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_5)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_3, function);
+          __Pyx_DECREF_SET(__pyx_t_2, function);
           __pyx_t_4 = 1;
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_1};
-        __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+        __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 221, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 219, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       }
-      __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 221, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 219, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (__pyx_t_7) {
 
-        /* "tactigon_speech/middleware/Tactigon_Speech.py":222
- *             elif last_command == Command.PLAY:
+        /* "tactigon_speech/middleware/Tactigon_Speech.py":220
+ *             elif current_command == Command.PLAY:
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
- *                     filename = None             # <<<<<<<<<<<<<<
+ *                     filename = ""             # <<<<<<<<<<<<<<
  *                     try:
- *                         filename = self.interface.recv()
+ *                         filename: str = self.interface.recv()
  */
-        __Pyx_INCREF(Py_None);
-        __Pyx_XDECREF_SET(__pyx_v_filename, Py_None);
+        __Pyx_INCREF(__pyx_kp_s__3);
+        __Pyx_XDECREF_SET(__pyx_v_filename, __pyx_kp_s__3);
 
-        /* "tactigon_speech/middleware/Tactigon_Speech.py":223
+        /* "tactigon_speech/middleware/Tactigon_Speech.py":221
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
- *                     filename = None
+ *                     filename = ""
  *                     try:             # <<<<<<<<<<<<<<
- *                         filename = self.interface.recv()
+ *                         filename: str = self.interface.recv()
  *                         self.play(filename)
  */
         /*try:*/ {
           {
             __Pyx_PyThreadState_declare
             __Pyx_PyThreadState_assign
-            __Pyx_ExceptionSave(&__pyx_t_21, &__pyx_t_22, &__pyx_t_23);
-            __Pyx_XGOTREF(__pyx_t_21);
-            __Pyx_XGOTREF(__pyx_t_22);
-            __Pyx_XGOTREF(__pyx_t_23);
+            __Pyx_ExceptionSave(&__pyx_t_18, &__pyx_t_19, &__pyx_t_20);
+            __Pyx_XGOTREF(__pyx_t_18);
+            __Pyx_XGOTREF(__pyx_t_19);
+            __Pyx_XGOTREF(__pyx_t_20);
             /*try:*/ {
 
-              /* "tactigon_speech/middleware/Tactigon_Speech.py":224
- *                     filename = None
+              /* "tactigon_speech/middleware/Tactigon_Speech.py":222
+ *                     filename = ""
  *                     try:
- *                         filename = self.interface.recv()             # <<<<<<<<<<<<<<
+ *                         filename: str = self.interface.recv()             # <<<<<<<<<<<<<<
  *                         self.play(filename)
  *                     except Exception as e:
  */
-              __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 224, __pyx_L43_error)
-              __Pyx_GOTREF(__pyx_t_3);
-              __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_recv); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L43_error)
+              __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L43_error)
+              __Pyx_GOTREF(__pyx_t_2);
+              __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_recv); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L43_error)
               __Pyx_GOTREF(__pyx_t_1);
-              __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-              __pyx_t_3 = NULL;
+              __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+              __pyx_t_2 = NULL;
               __pyx_t_4 = 0;
               #if CYTHON_UNPACK_METHODS
               if (likely(PyMethod_Check(__pyx_t_1))) {
-                __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
-                if (likely(__pyx_t_3)) {
+                __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
+                if (likely(__pyx_t_2)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-                  __Pyx_INCREF(__pyx_t_3);
+                  __Pyx_INCREF(__pyx_t_2);
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_1, function);
                   __pyx_t_4 = 1;
                 }
               }
               #endif
               {
-                PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
-                __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
-                __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-                if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L43_error)
-                __Pyx_GOTREF(__pyx_t_2);
+                PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
+                __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+                __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+                if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 222, __pyx_L43_error)
+                __Pyx_GOTREF(__pyx_t_3);
                 __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
               }
-              __Pyx_DECREF_SET(__pyx_v_filename, __pyx_t_2);
-              __pyx_t_2 = 0;
+              __Pyx_DECREF_SET(__pyx_v_filename, __pyx_t_3);
+              __pyx_t_3 = 0;
 
-              /* "tactigon_speech/middleware/Tactigon_Speech.py":225
+              /* "tactigon_speech/middleware/Tactigon_Speech.py":223
  *                     try:
- *                         filename = self.interface.recv()
+ *                         filename: str = self.interface.recv()
  *                         self.play(filename)             # <<<<<<<<<<<<<<
  *                     except Exception as e:
  *                         self.logger.warning("[TSpeech] Exception while playing a file. %s", e)
  */
-              __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_play); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L43_error)
+              __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_play); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L43_error)
               __Pyx_GOTREF(__pyx_t_1);
-              __pyx_t_3 = NULL;
+              __pyx_t_2 = NULL;
               __pyx_t_4 = 0;
               #if CYTHON_UNPACK_METHODS
               if (likely(PyMethod_Check(__pyx_t_1))) {
-                __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
-                if (likely(__pyx_t_3)) {
+                __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
+                if (likely(__pyx_t_2)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-                  __Pyx_INCREF(__pyx_t_3);
+                  __Pyx_INCREF(__pyx_t_2);
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_1, function);
                   __pyx_t_4 = 1;
                 }
               }
               #endif
               {
-                PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_filename};
-                __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-                __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-                if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L43_error)
-                __Pyx_GOTREF(__pyx_t_2);
+                PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_filename};
+                __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+                __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+                if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 223, __pyx_L43_error)
+                __Pyx_GOTREF(__pyx_t_3);
                 __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
               }
-              __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+              __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-              /* "tactigon_speech/middleware/Tactigon_Speech.py":223
+              /* "tactigon_speech/middleware/Tactigon_Speech.py":221
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
- *                     filename = None
+ *                     filename = ""
  *                     try:             # <<<<<<<<<<<<<<
- *                         filename = self.interface.recv()
+ *                         filename: str = self.interface.recv()
  *                         self.play(filename)
  */
             }
-            __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-            __Pyx_XDECREF(__pyx_t_22); __pyx_t_22 = 0;
-            __Pyx_XDECREF(__pyx_t_23); __pyx_t_23 = 0;
+            __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
+            __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
+            __Pyx_XDECREF(__pyx_t_20); __pyx_t_20 = 0;
             goto __pyx_L50_try_end;
             __pyx_L43_error:;
             __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
             __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-            __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-            __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-            __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
             __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
             __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-            /* "tactigon_speech/middleware/Tactigon_Speech.py":226
- *                         filename = self.interface.recv()
+            /* "tactigon_speech/middleware/Tactigon_Speech.py":224
+ *                         filename: str = self.interface.recv()
  *                         self.play(filename)
  *                     except Exception as e:             # <<<<<<<<<<<<<<
  *                         self.logger.warning("[TSpeech] Exception while playing a file. %s", e)
  *                     finally:
  */
             __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
             if (__pyx_t_4) {
               __Pyx_AddTraceback("tactigon_speech.middleware.Tactigon_Speech.Tactigon_Speech.run", __pyx_clineno, __pyx_lineno, __pyx_filename);
-              if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_1, &__pyx_t_3) < 0) __PYX_ERR(0, 226, __pyx_L45_except_error)
-              __Pyx_XGOTREF(__pyx_t_2);
-              __Pyx_XGOTREF(__pyx_t_1);
+              if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_1, &__pyx_t_2) < 0) __PYX_ERR(0, 224, __pyx_L45_except_error)
               __Pyx_XGOTREF(__pyx_t_3);
+              __Pyx_XGOTREF(__pyx_t_1);
+              __Pyx_XGOTREF(__pyx_t_2);
               __Pyx_INCREF(__pyx_t_1);
               __pyx_v_e = __pyx_t_1;
               /*try:*/ {
 
-                /* "tactigon_speech/middleware/Tactigon_Speech.py":227
+                /* "tactigon_speech/middleware/Tactigon_Speech.py":225
  *                         self.play(filename)
  *                     except Exception as e:
  *                         self.logger.warning("[TSpeech] Exception while playing a file. %s", e)             # <<<<<<<<<<<<<<
  *                     finally:
- *                         self.interface.send(filename)
+ *                         self.interface.send(InterfaceObject(current_command, filename))
  */
-                __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 227, __pyx_L56_error)
-                __Pyx_GOTREF(__pyx_t_11);
-                __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_warning); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 227, __pyx_L56_error)
+                __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 225, __pyx_L56_error)
                 __Pyx_GOTREF(__pyx_t_12);
-                __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-                __pyx_t_11 = NULL;
+                __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_warning); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 225, __pyx_L56_error)
+                __Pyx_GOTREF(__pyx_t_11);
+                __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+                __pyx_t_12 = NULL;
                 __pyx_t_4 = 0;
                 #if CYTHON_UNPACK_METHODS
-                if (likely(PyMethod_Check(__pyx_t_12))) {
-                  __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_12);
-                  if (likely(__pyx_t_11)) {
-                    PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
-                    __Pyx_INCREF(__pyx_t_11);
+                if (likely(PyMethod_Check(__pyx_t_11))) {
+                  __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
+                  if (likely(__pyx_t_12)) {
+                    PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
+                    __Pyx_INCREF(__pyx_t_12);
                     __Pyx_INCREF(function);
-                    __Pyx_DECREF_SET(__pyx_t_12, function);
+                    __Pyx_DECREF_SET(__pyx_t_11, function);
                     __pyx_t_4 = 1;
                   }
                 }
                 #endif
                 {
-                  PyObject *__pyx_callargs[3] = {__pyx_t_11, __pyx_kp_s_TSpeech_Exception_while_playing, __pyx_v_e};
-                  __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_12, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
-                  __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-                  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 227, __pyx_L56_error)
+                  PyObject *__pyx_callargs[3] = {__pyx_t_12, __pyx_kp_s_TSpeech_Exception_while_playing, __pyx_v_e};
+                  __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_11, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
+                  __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+                  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 225, __pyx_L56_error)
                   __Pyx_GOTREF(__pyx_t_5);
-                  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+                  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
                 }
                 __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
               }
 
-              /* "tactigon_speech/middleware/Tactigon_Speech.py":226
- *                         filename = self.interface.recv()
+              /* "tactigon_speech/middleware/Tactigon_Speech.py":224
+ *                         filename: str = self.interface.recv()
  *                         self.play(filename)
  *                     except Exception as e:             # <<<<<<<<<<<<<<
  *                         self.logger.warning("[TSpeech] Exception while playing a file. %s", e)
  *                     finally:
  */
               /*finally:*/ {
                 /*normal exit:*/{
                   __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
                   goto __pyx_L57;
                 }
                 __pyx_L56_error:;
                 /*exception exit:*/{
                   __Pyx_PyThreadState_declare
                   __Pyx_PyThreadState_assign
-                  __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_20 = 0; __pyx_t_19 = 0; __pyx_t_18 = 0;
+                  __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_17 = 0; __pyx_t_16 = 0; __pyx_t_15 = 0;
                   __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
                   __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-                  __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-                  __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-                  __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
                   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-                  if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_20, &__pyx_t_19, &__pyx_t_18);
+                  if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_17, &__pyx_t_16, &__pyx_t_15);
                   if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_8, &__pyx_t_9, &__pyx_t_10) < 0)) __Pyx_ErrFetch(&__pyx_t_8, &__pyx_t_9, &__pyx_t_10);
                   __Pyx_XGOTREF(__pyx_t_8);
                   __Pyx_XGOTREF(__pyx_t_9);
                   __Pyx_XGOTREF(__pyx_t_10);
-                  __Pyx_XGOTREF(__pyx_t_20);
-                  __Pyx_XGOTREF(__pyx_t_19);
-                  __Pyx_XGOTREF(__pyx_t_18);
-                  __pyx_t_4 = __pyx_lineno; __pyx_t_16 = __pyx_clineno; __pyx_t_26 = __pyx_filename;
+                  __Pyx_XGOTREF(__pyx_t_17);
+                  __Pyx_XGOTREF(__pyx_t_16);
+                  __Pyx_XGOTREF(__pyx_t_15);
+                  __pyx_t_4 = __pyx_lineno; __pyx_t_13 = __pyx_clineno; __pyx_t_23 = __pyx_filename;
                   {
                     __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
                   }
                   if (PY_MAJOR_VERSION >= 3) {
-                    __Pyx_XGIVEREF(__pyx_t_20);
-                    __Pyx_XGIVEREF(__pyx_t_19);
-                    __Pyx_XGIVEREF(__pyx_t_18);
-                    __Pyx_ExceptionReset(__pyx_t_20, __pyx_t_19, __pyx_t_18);
+                    __Pyx_XGIVEREF(__pyx_t_17);
+                    __Pyx_XGIVEREF(__pyx_t_16);
+                    __Pyx_XGIVEREF(__pyx_t_15);
+                    __Pyx_ExceptionReset(__pyx_t_17, __pyx_t_16, __pyx_t_15);
                   }
                   __Pyx_XGIVEREF(__pyx_t_8);
                   __Pyx_XGIVEREF(__pyx_t_9);
                   __Pyx_XGIVEREF(__pyx_t_10);
                   __Pyx_ErrRestore(__pyx_t_8, __pyx_t_9, __pyx_t_10);
-                  __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_20 = 0; __pyx_t_19 = 0; __pyx_t_18 = 0;
-                  __pyx_lineno = __pyx_t_4; __pyx_clineno = __pyx_t_16; __pyx_filename = __pyx_t_26;
+                  __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_17 = 0; __pyx_t_16 = 0; __pyx_t_15 = 0;
+                  __pyx_lineno = __pyx_t_4; __pyx_clineno = __pyx_t_13; __pyx_filename = __pyx_t_23;
                   goto __pyx_L45_except_error;
                 }
                 __pyx_L57:;
               }
-              __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-              __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
               __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+              __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+              __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
               goto __pyx_L44_exception_handled;
             }
             goto __pyx_L45_except_error;
 
-            /* "tactigon_speech/middleware/Tactigon_Speech.py":223
+            /* "tactigon_speech/middleware/Tactigon_Speech.py":221
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
- *                     filename = None
+ *                     filename = ""
  *                     try:             # <<<<<<<<<<<<<<
- *                         filename = self.interface.recv()
+ *                         filename: str = self.interface.recv()
  *                         self.play(filename)
  */
             __pyx_L45_except_error:;
-            __Pyx_XGIVEREF(__pyx_t_21);
-            __Pyx_XGIVEREF(__pyx_t_22);
-            __Pyx_XGIVEREF(__pyx_t_23);
-            __Pyx_ExceptionReset(__pyx_t_21, __pyx_t_22, __pyx_t_23);
+            __Pyx_XGIVEREF(__pyx_t_18);
+            __Pyx_XGIVEREF(__pyx_t_19);
+            __Pyx_XGIVEREF(__pyx_t_20);
+            __Pyx_ExceptionReset(__pyx_t_18, __pyx_t_19, __pyx_t_20);
             goto __pyx_L41_error;
             __pyx_L44_exception_handled:;
-            __Pyx_XGIVEREF(__pyx_t_21);
-            __Pyx_XGIVEREF(__pyx_t_22);
-            __Pyx_XGIVEREF(__pyx_t_23);
-            __Pyx_ExceptionReset(__pyx_t_21, __pyx_t_22, __pyx_t_23);
+            __Pyx_XGIVEREF(__pyx_t_18);
+            __Pyx_XGIVEREF(__pyx_t_19);
+            __Pyx_XGIVEREF(__pyx_t_20);
+            __Pyx_ExceptionReset(__pyx_t_18, __pyx_t_19, __pyx_t_20);
             __pyx_L50_try_end:;
           }
         }
 
-        /* "tactigon_speech/middleware/Tactigon_Speech.py":229
+        /* "tactigon_speech/middleware/Tactigon_Speech.py":227
  *                         self.logger.warning("[TSpeech] Exception while playing a file. %s", e)
  *                     finally:
- *                         self.interface.send(filename)             # <<<<<<<<<<<<<<
+ *                         self.interface.send(InterfaceObject(current_command, filename))             # <<<<<<<<<<<<<<
  *                 else:
  *                     self.logger.error("Play command received, but no filename from interface pipe.")
  */
         /*finally:*/ {
           /*normal exit:*/{
-            __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
+            __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_1);
-            __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_send); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 229, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_2);
+            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_send); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-            __pyx_t_1 = NULL;
-            __pyx_t_16 = 0;
+            __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InterfaceObject); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 227, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_5);
+            __pyx_t_11 = NULL;
+            __pyx_t_13 = 0;
             #if CYTHON_UNPACK_METHODS
-            if (likely(PyMethod_Check(__pyx_t_2))) {
-              __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
-              if (likely(__pyx_t_1)) {
-                PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-                __Pyx_INCREF(__pyx_t_1);
+            if (unlikely(PyMethod_Check(__pyx_t_5))) {
+              __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_5);
+              if (likely(__pyx_t_11)) {
+                PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+                __Pyx_INCREF(__pyx_t_11);
                 __Pyx_INCREF(function);
-                __Pyx_DECREF_SET(__pyx_t_2, function);
-                __pyx_t_16 = 1;
+                __Pyx_DECREF_SET(__pyx_t_5, function);
+                __pyx_t_13 = 1;
               }
             }
             #endif
             {
-              PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_v_filename};
-              __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_16, 1+__pyx_t_16);
-              __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-              if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 229, __pyx_L1_error)
-              __Pyx_GOTREF(__pyx_t_3);
-              __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+              PyObject *__pyx_callargs[3] = {__pyx_t_11, __pyx_v_current_command, __pyx_v_filename};
+              __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_13, 2+__pyx_t_13);
+              __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+              if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
+              __Pyx_GOTREF(__pyx_t_1);
+              __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
             }
-            __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+            __pyx_t_5 = NULL;
+            __pyx_t_13 = 0;
+            #if CYTHON_UNPACK_METHODS
+            if (likely(PyMethod_Check(__pyx_t_3))) {
+              __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+              if (likely(__pyx_t_5)) {
+                PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+                __Pyx_INCREF(__pyx_t_5);
+                __Pyx_INCREF(function);
+                __Pyx_DECREF_SET(__pyx_t_3, function);
+                __pyx_t_13 = 1;
+              }
+            }
+            #endif
+            {
+              PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_1};
+              __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_13, 1+__pyx_t_13);
+              __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+              __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+              if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error)
+              __Pyx_GOTREF(__pyx_t_2);
+              __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+            }
+            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             goto __pyx_L42;
           }
           __pyx_L41_error:;
           /*exception exit:*/{
             __Pyx_PyThreadState_declare
             __Pyx_PyThreadState_assign
-            __pyx_t_23 = 0; __pyx_t_22 = 0; __pyx_t_21 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0;
+            __pyx_t_20 = 0; __pyx_t_19 = 0; __pyx_t_18 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0;
             __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
             __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-            __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-            __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-            __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
             __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
             __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-            if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_18, &__pyx_t_19, &__pyx_t_20);
-            if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_23, &__pyx_t_22, &__pyx_t_21) < 0)) __Pyx_ErrFetch(&__pyx_t_23, &__pyx_t_22, &__pyx_t_21);
-            __Pyx_XGOTREF(__pyx_t_23);
-            __Pyx_XGOTREF(__pyx_t_22);
-            __Pyx_XGOTREF(__pyx_t_21);
-            __Pyx_XGOTREF(__pyx_t_18);
-            __Pyx_XGOTREF(__pyx_t_19);
+            if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_15, &__pyx_t_16, &__pyx_t_17);
+            if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_20, &__pyx_t_19, &__pyx_t_18) < 0)) __Pyx_ErrFetch(&__pyx_t_20, &__pyx_t_19, &__pyx_t_18);
             __Pyx_XGOTREF(__pyx_t_20);
-            __pyx_t_16 = __pyx_lineno; __pyx_t_4 = __pyx_clineno; __pyx_t_27 = __pyx_filename;
+            __Pyx_XGOTREF(__pyx_t_19);
+            __Pyx_XGOTREF(__pyx_t_18);
+            __Pyx_XGOTREF(__pyx_t_15);
+            __Pyx_XGOTREF(__pyx_t_16);
+            __Pyx_XGOTREF(__pyx_t_17);
+            __pyx_t_13 = __pyx_lineno; __pyx_t_4 = __pyx_clineno; __pyx_t_24 = __pyx_filename;
             {
-              __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 229, __pyx_L65_error)
-              __Pyx_GOTREF(__pyx_t_2);
-              __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_send); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L65_error)
+              __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L65_error)
+              __Pyx_GOTREF(__pyx_t_3);
+              __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_send); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L65_error)
               __Pyx_GOTREF(__pyx_t_1);
-              __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-              __pyx_t_2 = NULL;
-              __pyx_t_25 = 0;
+              __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+              __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InterfaceObject); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 227, __pyx_L65_error)
+              __Pyx_GOTREF(__pyx_t_5);
+              __pyx_t_11 = NULL;
+              __pyx_t_22 = 0;
+              #if CYTHON_UNPACK_METHODS
+              if (unlikely(PyMethod_Check(__pyx_t_5))) {
+                __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_5);
+                if (likely(__pyx_t_11)) {
+                  PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+                  __Pyx_INCREF(__pyx_t_11);
+                  __Pyx_INCREF(function);
+                  __Pyx_DECREF_SET(__pyx_t_5, function);
+                  __pyx_t_22 = 1;
+                }
+              }
+              #endif
+              {
+                PyObject *__pyx_callargs[3] = {__pyx_t_11, __pyx_v_current_command, __pyx_v_filename};
+                __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_22, 2+__pyx_t_22);
+                __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+                if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L65_error)
+                __Pyx_GOTREF(__pyx_t_3);
+                __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+              }
+              __pyx_t_5 = NULL;
+              __pyx_t_22 = 0;
               #if CYTHON_UNPACK_METHODS
               if (likely(PyMethod_Check(__pyx_t_1))) {
-                __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
-                if (likely(__pyx_t_2)) {
+                __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+                if (likely(__pyx_t_5)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-                  __Pyx_INCREF(__pyx_t_2);
+                  __Pyx_INCREF(__pyx_t_5);
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_1, function);
-                  __pyx_t_25 = 1;
+                  __pyx_t_22 = 1;
                 }
               }
               #endif
               {
-                PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_filename};
-                __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_25, 1+__pyx_t_25);
-                __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-                if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 229, __pyx_L65_error)
-                __Pyx_GOTREF(__pyx_t_3);
+                PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_3};
+                __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_22, 1+__pyx_t_22);
+                __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+                __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+                if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 227, __pyx_L65_error)
+                __Pyx_GOTREF(__pyx_t_2);
                 __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
               }
-              __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+              __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             }
             if (PY_MAJOR_VERSION >= 3) {
-              __Pyx_XGIVEREF(__pyx_t_18);
-              __Pyx_XGIVEREF(__pyx_t_19);
-              __Pyx_XGIVEREF(__pyx_t_20);
-              __Pyx_ExceptionReset(__pyx_t_18, __pyx_t_19, __pyx_t_20);
-            }
-            __Pyx_XGIVEREF(__pyx_t_23);
-            __Pyx_XGIVEREF(__pyx_t_22);
-            __Pyx_XGIVEREF(__pyx_t_21);
-            __Pyx_ErrRestore(__pyx_t_23, __pyx_t_22, __pyx_t_21);
-            __pyx_t_23 = 0; __pyx_t_22 = 0; __pyx_t_21 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0;
-            __pyx_lineno = __pyx_t_16; __pyx_clineno = __pyx_t_4; __pyx_filename = __pyx_t_27;
+              __Pyx_XGIVEREF(__pyx_t_15);
+              __Pyx_XGIVEREF(__pyx_t_16);
+              __Pyx_XGIVEREF(__pyx_t_17);
+              __Pyx_ExceptionReset(__pyx_t_15, __pyx_t_16, __pyx_t_17);
+            }
+            __Pyx_XGIVEREF(__pyx_t_20);
+            __Pyx_XGIVEREF(__pyx_t_19);
+            __Pyx_XGIVEREF(__pyx_t_18);
+            __Pyx_ErrRestore(__pyx_t_20, __pyx_t_19, __pyx_t_18);
+            __pyx_t_20 = 0; __pyx_t_19 = 0; __pyx_t_18 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0;
+            __pyx_lineno = __pyx_t_13; __pyx_clineno = __pyx_t_4; __pyx_filename = __pyx_t_24;
             goto __pyx_L1_error;
             __pyx_L65_error:;
             if (PY_MAJOR_VERSION >= 3) {
-              __Pyx_XGIVEREF(__pyx_t_18);
-              __Pyx_XGIVEREF(__pyx_t_19);
-              __Pyx_XGIVEREF(__pyx_t_20);
-              __Pyx_ExceptionReset(__pyx_t_18, __pyx_t_19, __pyx_t_20);
-            }
-            __Pyx_XDECREF(__pyx_t_23); __pyx_t_23 = 0;
-            __Pyx_XDECREF(__pyx_t_22); __pyx_t_22 = 0;
-            __Pyx_XDECREF(__pyx_t_21); __pyx_t_21 = 0;
-            __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0;
+              __Pyx_XGIVEREF(__pyx_t_15);
+              __Pyx_XGIVEREF(__pyx_t_16);
+              __Pyx_XGIVEREF(__pyx_t_17);
+              __Pyx_ExceptionReset(__pyx_t_15, __pyx_t_16, __pyx_t_17);
+            }
+            __Pyx_XDECREF(__pyx_t_20); __pyx_t_20 = 0;
+            __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
+            __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
+            __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0;
             goto __pyx_L1_error;
           }
           __pyx_L42:;
         }
 
-        /* "tactigon_speech/middleware/Tactigon_Speech.py":221
- *                     self.interface.send(False)
- *             elif last_command == Command.PLAY:
+        /* "tactigon_speech/middleware/Tactigon_Speech.py":219
+ *                     self.interface.send(InterfaceObject(current_command, False))
+ *             elif current_command == Command.PLAY:
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):             # <<<<<<<<<<<<<<
- *                     filename = None
+ *                     filename = ""
  *                     try:
  */
         goto __pyx_L37;
       }
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":231
- *                         self.interface.send(filename)
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":229
+ *                         self.interface.send(InterfaceObject(current_command, filename))
  *                 else:
  *                     self.logger.error("Play command received, but no filename from interface pipe.")             # <<<<<<<<<<<<<<
- *                     self.interface.send(False)
- *             elif last_command == Command.RECORD:
+ *                     self.interface.send(InterfaceObject(current_command, False))
+ *             elif current_command == Command.RECORD:
  */
       /*else*/ {
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_error); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_error); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 229, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_t_1 = NULL;
         __pyx_t_4 = 0;
         #if CYTHON_UNPACK_METHODS
-        if (likely(PyMethod_Check(__pyx_t_2))) {
-          __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
+        if (likely(PyMethod_Check(__pyx_t_3))) {
+          __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_1)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
             __Pyx_INCREF(__pyx_t_1);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_2, function);
+            __Pyx_DECREF_SET(__pyx_t_3, function);
             __pyx_t_4 = 1;
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_kp_s_Play_command_received_but_no_fil};
-          __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+          __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 231, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 229, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "tactigon_speech/middleware/Tactigon_Speech.py":232
+        /* "tactigon_speech/middleware/Tactigon_Speech.py":230
  *                 else:
  *                     self.logger.error("Play command received, but no filename from interface pipe.")
- *                     self.interface.send(False)             # <<<<<<<<<<<<<<
- *             elif last_command == Command.RECORD:
+ *                     self.interface.send(InterfaceObject(current_command, False))             # <<<<<<<<<<<<<<
+ *             elif current_command == Command.RECORD:
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
  */
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 232, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_send); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 230, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_send); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_2 = NULL;
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InterfaceObject); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 230, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __pyx_t_11 = NULL;
+        __pyx_t_4 = 0;
+        #if CYTHON_UNPACK_METHODS
+        if (unlikely(PyMethod_Check(__pyx_t_5))) {
+          __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_5);
+          if (likely(__pyx_t_11)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+            __Pyx_INCREF(__pyx_t_11);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_5, function);
+            __pyx_t_4 = 1;
+          }
+        }
+        #endif
+        {
+          PyObject *__pyx_callargs[3] = {__pyx_t_11, __pyx_v_current_command, Py_False};
+          __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
+          __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 230, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_3);
+          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        }
+        __pyx_t_5 = NULL;
         __pyx_t_4 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_1))) {
-          __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
-          if (likely(__pyx_t_2)) {
+          __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+          if (likely(__pyx_t_5)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-            __Pyx_INCREF(__pyx_t_2);
+            __Pyx_INCREF(__pyx_t_5);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_1, function);
             __pyx_t_4 = 1;
           }
         }
         #endif
         {
-          PyObject *__pyx_callargs[2] = {__pyx_t_2, Py_False};
-          __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-          __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 232, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_3);
+          PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_3};
+          __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+          __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 230, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         }
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       }
       __pyx_L37:;
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":220
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":218
  *                     self.logger.error("Listen command received, but no tspeech from interface pipe.")
- *                     self.interface.send(False)
- *             elif last_command == Command.PLAY:             # <<<<<<<<<<<<<<
+ *                     self.interface.send(InterfaceObject(current_command, False))
+ *             elif current_command == Command.PLAY:             # <<<<<<<<<<<<<<
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
- *                     filename = None
+ *                     filename = ""
  */
       goto __pyx_L7;
     }
 
-    /* "tactigon_speech/middleware/Tactigon_Speech.py":233
+    /* "tactigon_speech/middleware/Tactigon_Speech.py":231
  *                     self.logger.error("Play command received, but no filename from interface pipe.")
- *                     self.interface.send(False)
- *             elif last_command == Command.RECORD:             # <<<<<<<<<<<<<<
+ *                     self.interface.send(InterfaceObject(current_command, False))
+ *             elif current_command == Command.RECORD:             # <<<<<<<<<<<<<<
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
  *                     filename = self.interface.recv()
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Command); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 233, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_RECORD); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Command); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_RECORD); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyObject_RichCompare(__pyx_v_last_command, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 233, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = PyObject_RichCompare(__pyx_v_current_command, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 233, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 231, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (__pyx_t_7) {
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":234
- *                     self.interface.send(False)
- *             elif last_command == Command.RECORD:
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":232
+ *                     self.interface.send(InterfaceObject(current_command, False))
+ *             elif current_command == Command.RECORD:
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):             # <<<<<<<<<<<<<<
  *                     filename = self.interface.recv()
  *                     self.record(filename)
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_poll); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_poll); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 232, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_INTERFACE_TIMEOUT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_INTERFACE_TIMEOUT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_5 = NULL;
       __pyx_t_4 = 0;
       #if CYTHON_UNPACK_METHODS
-      if (likely(PyMethod_Check(__pyx_t_2))) {
-        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_5)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_2, function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
           __pyx_t_4 = 1;
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_1};
-        __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+        __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 232, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
-      __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 234, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 232, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_7) {
 
-        /* "tactigon_speech/middleware/Tactigon_Speech.py":235
- *             elif last_command == Command.RECORD:
+        /* "tactigon_speech/middleware/Tactigon_Speech.py":233
+ *             elif current_command == Command.RECORD:
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
  *                     filename = self.interface.recv()             # <<<<<<<<<<<<<<
  *                     self.record(filename)
- *                     self.interface.send(filename)
+ *                     self.interface.send(InterfaceObject(current_command, filename))
  */
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 235, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_recv); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 233, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_recv); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_2 = NULL;
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __pyx_t_3 = NULL;
         __pyx_t_4 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_1))) {
-          __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
-          if (likely(__pyx_t_2)) {
+          __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
+          if (likely(__pyx_t_3)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-            __Pyx_INCREF(__pyx_t_2);
+            __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_1, function);
             __pyx_t_4 = 1;
           }
         }
         #endif
         {
-          PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
-          __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
-          __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 235, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_3);
+          PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
+          __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+          __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         }
-        __Pyx_XDECREF_SET(__pyx_v_filename, __pyx_t_3);
-        __pyx_t_3 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_filename, __pyx_t_2);
+        __pyx_t_2 = 0;
 
-        /* "tactigon_speech/middleware/Tactigon_Speech.py":236
+        /* "tactigon_speech/middleware/Tactigon_Speech.py":234
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
  *                     filename = self.interface.recv()
  *                     self.record(filename)             # <<<<<<<<<<<<<<
- *                     self.interface.send(filename)
+ *                     self.interface.send(InterfaceObject(current_command, filename))
  *                 else:
  */
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_record); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_record); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_2 = NULL;
+        __pyx_t_3 = NULL;
         __pyx_t_4 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_1))) {
-          __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
-          if (likely(__pyx_t_2)) {
+          __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
+          if (likely(__pyx_t_3)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-            __Pyx_INCREF(__pyx_t_2);
+            __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_1, function);
             __pyx_t_4 = 1;
           }
         }
         #endif
         {
-          PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_filename};
-          __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-          __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_3);
+          PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_filename};
+          __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+          __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         }
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "tactigon_speech/middleware/Tactigon_Speech.py":237
+        /* "tactigon_speech/middleware/Tactigon_Speech.py":235
  *                     filename = self.interface.recv()
  *                     self.record(filename)
- *                     self.interface.send(filename)             # <<<<<<<<<<<<<<
+ *                     self.interface.send(InterfaceObject(current_command, filename))             # <<<<<<<<<<<<<<
  *                 else:
  *                     self.logger.error("Record command received, but no filename from interface pipe.")
  */
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 237, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_send); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 237, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_send); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 235, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = NULL;
+        __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InterfaceObject); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 235, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __pyx_t_11 = NULL;
         __pyx_t_4 = 0;
         #if CYTHON_UNPACK_METHODS
-        if (likely(PyMethod_Check(__pyx_t_2))) {
-          __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
-          if (likely(__pyx_t_1)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-            __Pyx_INCREF(__pyx_t_1);
+        if (unlikely(PyMethod_Check(__pyx_t_5))) {
+          __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_5);
+          if (likely(__pyx_t_11)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+            __Pyx_INCREF(__pyx_t_11);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_2, function);
+            __Pyx_DECREF_SET(__pyx_t_5, function);
             __pyx_t_4 = 1;
           }
         }
         #endif
         {
-          PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_v_filename};
-          __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-          __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 237, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          PyObject *__pyx_callargs[3] = {__pyx_t_11, __pyx_v_current_command, __pyx_v_filename};
+          __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
+          __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         }
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __pyx_t_5 = NULL;
+        __pyx_t_4 = 0;
+        #if CYTHON_UNPACK_METHODS
+        if (likely(PyMethod_Check(__pyx_t_3))) {
+          __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+          if (likely(__pyx_t_5)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+            __Pyx_INCREF(__pyx_t_5);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_3, function);
+            __pyx_t_4 = 1;
+          }
+        }
+        #endif
+        {
+          PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_1};
+          __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+          __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 235, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        }
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "tactigon_speech/middleware/Tactigon_Speech.py":234
- *                     self.interface.send(False)
- *             elif last_command == Command.RECORD:
+        /* "tactigon_speech/middleware/Tactigon_Speech.py":232
+ *                     self.interface.send(InterfaceObject(current_command, False))
+ *             elif current_command == Command.RECORD:
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):             # <<<<<<<<<<<<<<
  *                     filename = self.interface.recv()
  *                     self.record(filename)
  */
         goto __pyx_L66;
       }
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":239
- *                     self.interface.send(filename)
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":237
+ *                     self.interface.send(InterfaceObject(current_command, filename))
  *                 else:
  *                     self.logger.error("Record command received, but no filename from interface pipe.")             # <<<<<<<<<<<<<<
- *                     self.interface.send(False)
- *             elif last_command == Command.STOP:
+ *                     self.interface.send(InterfaceObject(current_command, False))
+ *             elif current_command == Command.STOP:
  */
       /*else*/ {
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 239, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 237, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 237, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_2 = NULL;
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __pyx_t_3 = NULL;
         __pyx_t_4 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_1))) {
-          __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
-          if (likely(__pyx_t_2)) {
+          __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
+          if (likely(__pyx_t_3)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-            __Pyx_INCREF(__pyx_t_2);
+            __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_1, function);
             __pyx_t_4 = 1;
           }
         }
         #endif
         {
-          PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_kp_s_Record_command_received_but_no_f};
-          __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-          __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 239, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_3);
+          PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_s_Record_command_received_but_no_f};
+          __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+          __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 237, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         }
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "tactigon_speech/middleware/Tactigon_Speech.py":240
+        /* "tactigon_speech/middleware/Tactigon_Speech.py":238
  *                 else:
  *                     self.logger.error("Record command received, but no filename from interface pipe.")
- *                     self.interface.send(False)             # <<<<<<<<<<<<<<
- *             elif last_command == Command.STOP:
- *                 self.interface.send(True)
+ *                     self.interface.send(InterfaceObject(current_command, False))             # <<<<<<<<<<<<<<
+ *             elif current_command == Command.STOP:
+ *                 self.interface.send(InterfaceObject(current_command, True))
  */
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 240, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_send); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 240, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_send); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = NULL;
+        __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InterfaceObject); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 238, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __pyx_t_11 = NULL;
         __pyx_t_4 = 0;
         #if CYTHON_UNPACK_METHODS
-        if (likely(PyMethod_Check(__pyx_t_2))) {
-          __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
-          if (likely(__pyx_t_1)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-            __Pyx_INCREF(__pyx_t_1);
+        if (unlikely(PyMethod_Check(__pyx_t_5))) {
+          __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_5);
+          if (likely(__pyx_t_11)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+            __Pyx_INCREF(__pyx_t_11);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_2, function);
+            __Pyx_DECREF_SET(__pyx_t_5, function);
             __pyx_t_4 = 1;
           }
         }
         #endif
         {
-          PyObject *__pyx_callargs[2] = {__pyx_t_1, Py_False};
-          __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-          __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          PyObject *__pyx_callargs[3] = {__pyx_t_11, __pyx_v_current_command, Py_False};
+          __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
+          __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         }
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __pyx_t_5 = NULL;
+        __pyx_t_4 = 0;
+        #if CYTHON_UNPACK_METHODS
+        if (likely(PyMethod_Check(__pyx_t_3))) {
+          __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+          if (likely(__pyx_t_5)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+            __Pyx_INCREF(__pyx_t_5);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_3, function);
+            __pyx_t_4 = 1;
+          }
+        }
+        #endif
+        {
+          PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_1};
+          __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+          __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 238, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        }
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       }
       __pyx_L66:;
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":233
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":231
  *                     self.logger.error("Play command received, but no filename from interface pipe.")
- *                     self.interface.send(False)
- *             elif last_command == Command.RECORD:             # <<<<<<<<<<<<<<
+ *                     self.interface.send(InterfaceObject(current_command, False))
+ *             elif current_command == Command.RECORD:             # <<<<<<<<<<<<<<
  *                 if self.interface.poll(self._INTERFACE_TIMEOUT):
  *                     filename = self.interface.recv()
  */
       goto __pyx_L7;
     }
 
-    /* "tactigon_speech/middleware/Tactigon_Speech.py":241
+    /* "tactigon_speech/middleware/Tactigon_Speech.py":239
  *                     self.logger.error("Record command received, but no filename from interface pipe.")
- *                     self.interface.send(False)
- *             elif last_command == Command.STOP:             # <<<<<<<<<<<<<<
- *                 self.interface.send(True)
+ *                     self.interface.send(InterfaceObject(current_command, False))
+ *             elif current_command == Command.STOP:             # <<<<<<<<<<<<<<
+ *                 self.interface.send(InterfaceObject(current_command, True))
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Command); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 241, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_STOP); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 241, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Command); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 239, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyObject_RichCompare(__pyx_v_last_command, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 241, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_STOP); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 239, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 241, __pyx_L1_error)
+    __pyx_t_2 = PyObject_RichCompare(__pyx_v_current_command, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 239, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 239, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (__pyx_t_7) {
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":242
- *                     self.interface.send(False)
- *             elif last_command == Command.STOP:
- *                 self.interface.send(True)             # <<<<<<<<<<<<<<
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":240
+ *                     self.interface.send(InterfaceObject(current_command, False))
+ *             elif current_command == Command.STOP:
+ *                 self.interface.send(InterfaceObject(current_command, True))             # <<<<<<<<<<<<<<
  * 
- *         self.clear_audio_pipe()
+ *             self.command = Command.NONE
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_send); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_send); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 240, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = NULL;
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InterfaceObject); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 240, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_11 = NULL;
+      __pyx_t_4 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_5))) {
+        __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_5);
+        if (likely(__pyx_t_11)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+          __Pyx_INCREF(__pyx_t_11);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_5, function);
+          __pyx_t_4 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[3] = {__pyx_t_11, __pyx_v_current_command, Py_True};
+        __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
+        __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      }
+      __pyx_t_5 = NULL;
       __pyx_t_4 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_1))) {
-        __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
-        if (likely(__pyx_t_2)) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+        if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-          __Pyx_INCREF(__pyx_t_2);
+          __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
           __pyx_t_4 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_2, Py_True};
-        __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 242, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
+        PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_3};
+        __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 240, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "tactigon_speech/middleware/Tactigon_Speech.py":241
+      /* "tactigon_speech/middleware/Tactigon_Speech.py":239
  *                     self.logger.error("Record command received, but no filename from interface pipe.")
- *                     self.interface.send(False)
- *             elif last_command == Command.STOP:             # <<<<<<<<<<<<<<
- *                 self.interface.send(True)
+ *                     self.interface.send(InterfaceObject(current_command, False))
+ *             elif current_command == Command.STOP:             # <<<<<<<<<<<<<<
+ *                 self.interface.send(InterfaceObject(current_command, True))
  * 
  */
     }
     __pyx_L7:;
+
+    /* "tactigon_speech/middleware/Tactigon_Speech.py":242
+ *                 self.interface.send(InterfaceObject(current_command, True))
+ * 
+ *             self.command = Command.NONE             # <<<<<<<<<<<<<<
+ * 
+ *         self.clear_audio_pipe()
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Command); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_NONE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_command_2, __pyx_t_1) < 0) __PYX_ERR(0, 242, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_L4_continue:;
   }
 
   /* "tactigon_speech/middleware/Tactigon_Speech.py":244
- *                 self.interface.send(True)
+ *             self.command = Command.NONE
  * 
  *         self.clear_audio_pipe()             # <<<<<<<<<<<<<<
  *         self.logger.debug("Stopped")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_clear_audio_pipe); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = NULL;
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_clear_audio_pipe); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
-  if (likely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-      __Pyx_INCREF(__pyx_t_2);
+  if (likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_1, function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #endif
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
-    __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 244, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "tactigon_speech/middleware/Tactigon_Speech.py":245
  * 
  *         self.clear_audio_pipe()
  *         self.logger.debug("Stopped")             # <<<<<<<<<<<<<<
  * 
  *     def join(self, timeout: Optional[float] = None):
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_debug); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = NULL;
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
-  if (likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_1)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_1);
+  if (likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_4 = 1;
     }
   }
   #endif
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_n_s_Stopped};
-    __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 245, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_n_s_Stopped};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "tactigon_speech/middleware/Tactigon_Speech.py":175
  *         return None
  * 
  *     def run(self):             # <<<<<<<<<<<<<<
  *         self.logger.debug("Creating PyAudio")
  *         self.pa = PyAudio()
@@ -10405,21 +10618,18 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
-  __Pyx_XDECREF(__pyx_t_13);
-  __Pyx_XDECREF(__pyx_t_14);
-  __Pyx_XDECREF(__pyx_t_15);
   __Pyx_AddTraceback("tactigon_speech.middleware.Tactigon_Speech.Tactigon_Speech.run", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_last_command);
+  __Pyx_XDECREF(__pyx_v_current_command);
   __Pyx_XDECREF(__pyx_v_transcription);
   __Pyx_XDECREF(__pyx_v_speech_tree);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_XDECREF(__pyx_v_filename);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -12175,77 +12385,108 @@
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
       /* "tactigon_speech/middleware/Tactigon_Speech.py":296
  *             if text != text_so_far:
  *                 self.logger.info("Transcribed: %s", text)
  *                 text_so_far = text             # <<<<<<<<<<<<<<
  *                 if text_so_far is not "":
- *                     self.interface.send(text_so_far)
+ *                     self.interface.send(InterfaceObject(Command.LISTEN, text_so_far))
  */
       __Pyx_INCREF(__pyx_v_text);
       __Pyx_DECREF_SET(__pyx_v_text_so_far, __pyx_v_text);
 
       /* "tactigon_speech/middleware/Tactigon_Speech.py":297
  *                 self.logger.info("Transcribed: %s", text)
  *                 text_so_far = text
  *                 if text_so_far is not "":             # <<<<<<<<<<<<<<
- *                     self.interface.send(text_so_far)
+ *                     self.interface.send(InterfaceObject(Command.LISTEN, text_so_far))
  *                 self.check_branch(text)
  */
       __pyx_t_7 = (__pyx_v_text_so_far != __pyx_kp_s__3);
       if (__pyx_t_7) {
 
         /* "tactigon_speech/middleware/Tactigon_Speech.py":298
  *                 text_so_far = text
  *                 if text_so_far is not "":
- *                     self.interface.send(text_so_far)             # <<<<<<<<<<<<<<
+ *                     self.interface.send(InterfaceObject(Command.LISTEN, text_so_far))             # <<<<<<<<<<<<<<
  *                 self.check_branch(text)
  * 
  */
         __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_interface); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 298, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_13);
         __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_send); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 298, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-        __pyx_t_13 = NULL;
+        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_InterfaceObject); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 298, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_Command); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 298, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_15);
+        __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_LISTEN); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 298, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
+        __pyx_t_15 = NULL;
+        __pyx_t_4 = 0;
+        #if CYTHON_UNPACK_METHODS
+        if (unlikely(PyMethod_Check(__pyx_t_3))) {
+          __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_3);
+          if (likely(__pyx_t_15)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+            __Pyx_INCREF(__pyx_t_15);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_3, function);
+            __pyx_t_4 = 1;
+          }
+        }
+        #endif
+        {
+          PyObject *__pyx_callargs[3] = {__pyx_t_15, __pyx_t_14, __pyx_v_text_so_far};
+          __pyx_t_13 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
+          __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+          if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 298, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_13);
+          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        }
+        __pyx_t_3 = NULL;
         __pyx_t_4 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_2))) {
-          __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_2);
-          if (likely(__pyx_t_13)) {
+          __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+          if (likely(__pyx_t_3)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-            __Pyx_INCREF(__pyx_t_13);
+            __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_2, function);
             __pyx_t_4 = 1;
           }
         }
         #endif
         {
-          PyObject *__pyx_callargs[2] = {__pyx_t_13, __pyx_v_text_so_far};
+          PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_13};
           __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-          __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+          __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 298, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         }
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
         /* "tactigon_speech/middleware/Tactigon_Speech.py":297
  *                 self.logger.info("Transcribed: %s", text)
  *                 text_so_far = text
  *                 if text_so_far is not "":             # <<<<<<<<<<<<<<
- *                     self.interface.send(text_so_far)
+ *                     self.interface.send(InterfaceObject(Command.LISTEN, text_so_far))
  *                 self.check_branch(text)
  */
       }
 
       /* "tactigon_speech/middleware/Tactigon_Speech.py":299
  *                 if text_so_far is not "":
- *                     self.interface.send(text_so_far)
+ *                     self.interface.send(InterfaceObject(Command.LISTEN, text_so_far))
  *                 self.check_branch(text)             # <<<<<<<<<<<<<<
  * 
  *             delta = millis() - delta
  */
       __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_check_branch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 299, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_13 = NULL;
@@ -14527,14 +14768,15 @@
     {&__pyx_kp_s_Generator_bytes_bytes_None, __pyx_k_Generator_bytes_bytes_None, sizeof(__pyx_k_Generator_bytes_bytes_None), 0, 0, 1, 0},
     {&__pyx_kp_s_Got_i_unvoiced_frames_Threshold, __pyx_k_Got_i_unvoiced_frames_Threshold, sizeof(__pyx_k_Got_i_unvoiced_frames_Threshold), 0, 0, 1, 0},
     {&__pyx_kp_s_Got_i_voiced_frames_Threshold_is, __pyx_k_Got_i_voiced_frames_Threshold_is, sizeof(__pyx_k_Got_i_voiced_frames_Threshold_is), 0, 0, 1, 0},
     {&__pyx_n_s_HotWord, __pyx_k_HotWord, sizeof(__pyx_k_HotWord), 0, 0, 1, 1},
     {&__pyx_n_s_INFO, __pyx_k_INFO, sizeof(__pyx_k_INFO), 0, 0, 1, 1},
     {&__pyx_n_s_INTERFACE_TIMEOUT, __pyx_k_INTERFACE_TIMEOUT, sizeof(__pyx_k_INTERFACE_TIMEOUT), 0, 0, 1, 1},
     {&__pyx_kp_s_Initializing_model, __pyx_k_Initializing_model, sizeof(__pyx_k_Initializing_model), 0, 0, 1, 0},
+    {&__pyx_n_s_InterfaceObject, __pyx_k_InterfaceObject, sizeof(__pyx_k_InterfaceObject), 0, 0, 1, 1},
     {&__pyx_n_s_Joined, __pyx_k_Joined, sizeof(__pyx_k_Joined), 0, 0, 1, 1},
     {&__pyx_n_s_LISTEN, __pyx_k_LISTEN, sizeof(__pyx_k_LISTEN), 0, 0, 1, 1},
     {&__pyx_n_s_List, __pyx_k_List, sizeof(__pyx_k_List), 0, 0, 1, 1},
     {&__pyx_kp_s_Listen_command_received_but_no_t, __pyx_k_Listen_command_received_but_no_t, sizeof(__pyx_k_Listen_command_received_but_no_t), 0, 0, 1, 0},
     {&__pyx_n_s_MIC, __pyx_k_MIC, sizeof(__pyx_k_MIC), 0, 0, 1, 1},
     {&__pyx_n_s_Model, __pyx_k_Model, sizeof(__pyx_k_Model), 0, 0, 1, 1},
     {&__pyx_kp_s_Model_initialized, __pyx_k_Model_initialized, sizeof(__pyx_k_Model_initialized), 0, 0, 1, 0},
@@ -14554,15 +14796,14 @@
     {&__pyx_kp_s_Running, __pyx_k_Running, sizeof(__pyx_k_Running), 0, 0, 1, 0},
     {&__pyx_n_s_SAMPLE_RATE, __pyx_k_SAMPLE_RATE, sizeof(__pyx_k_SAMPLE_RATE), 0, 0, 1, 1},
     {&__pyx_n_s_SINGLE_FRAME_LENGTH, __pyx_k_SINGLE_FRAME_LENGTH, sizeof(__pyx_k_SINGLE_FRAME_LENGTH), 0, 0, 1, 1},
     {&__pyx_n_s_STOP, __pyx_k_STOP, sizeof(__pyx_k_STOP), 0, 0, 1, 1},
     {&__pyx_kp_s_Setting_command_s, __pyx_k_Setting_command_s, sizeof(__pyx_k_Setting_command_s), 0, 0, 1, 0},
     {&__pyx_kp_s_Starting_Tactigon_Speech, __pyx_k_Starting_Tactigon_Speech, sizeof(__pyx_k_Starting_Tactigon_Speech), 0, 0, 1, 0},
     {&__pyx_n_s_Stopped, __pyx_k_Stopped, sizeof(__pyx_k_Stopped), 0, 0, 1, 1},
-    {&__pyx_n_s_SynchronizedBase, __pyx_k_SynchronizedBase, sizeof(__pyx_k_SynchronizedBase), 0, 0, 1, 1},
     {&__pyx_n_s_TICK, __pyx_k_TICK, sizeof(__pyx_k_TICK), 0, 0, 1, 1},
     {&__pyx_n_s_TSpeech, __pyx_k_TSpeech, sizeof(__pyx_k_TSpeech), 0, 0, 1, 1},
     {&__pyx_n_s_TSpeechObject, __pyx_k_TSpeechObject, sizeof(__pyx_k_TSpeechObject), 0, 0, 1, 1},
     {&__pyx_kp_s_TSpeech_Exception_while_listeni, __pyx_k_TSpeech_Exception_while_listeni, sizeof(__pyx_k_TSpeech_Exception_while_listeni), 0, 0, 1, 0},
     {&__pyx_kp_s_TSpeech_Exception_while_playing, __pyx_k_TSpeech_Exception_while_playing, sizeof(__pyx_k_TSpeech_Exception_while_playing), 0, 0, 1, 0},
     {&__pyx_kp_s_TSpeech_Transcibed_text_s_Tree, __pyx_k_TSpeech_Transcibed_text_s_Tree, sizeof(__pyx_k_TSpeech_Transcibed_text_s_Tree), 0, 0, 1, 0},
     {&__pyx_n_s_Tactigon_Speech, __pyx_k_Tactigon_Speech, sizeof(__pyx_k_Tactigon_Speech), 0, 0, 1, 1},
@@ -14621,14 +14862,15 @@
     {&__pyx_n_s_collections, __pyx_k_collections, sizeof(__pyx_k_collections), 0, 0, 1, 1},
     {&__pyx_n_s_command, __pyx_k_command, sizeof(__pyx_k_command), 0, 0, 1, 1},
     {&__pyx_n_s_command_2, __pyx_k_command_2, sizeof(__pyx_k_command_2), 0, 0, 1, 1},
     {&__pyx_n_s_config, __pyx_k_config, sizeof(__pyx_k_config), 0, 0, 1, 1},
     {&__pyx_n_s_createStream, __pyx_k_createStream, sizeof(__pyx_k_createStream), 0, 0, 1, 1},
     {&__pyx_n_s_ctypes, __pyx_k_ctypes, sizeof(__pyx_k_ctypes), 0, 0, 1, 1},
     {&__pyx_n_s_current_branch, __pyx_k_current_branch, sizeof(__pyx_k_current_branch), 0, 0, 1, 1},
+    {&__pyx_n_s_current_command, __pyx_k_current_command, sizeof(__pyx_k_current_command), 0, 0, 1, 1},
     {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
     {&__pyx_n_s_datetime, __pyx_k_datetime, sizeof(__pyx_k_datetime), 0, 0, 1, 1},
     {&__pyx_n_s_debug, __pyx_k_debug, sizeof(__pyx_k_debug), 0, 0, 1, 1},
     {&__pyx_n_s_deepspeech, __pyx_k_deepspeech, sizeof(__pyx_k_deepspeech), 0, 0, 1, 1},
     {&__pyx_kp_s_deepspeech_Model, __pyx_k_deepspeech_Model, sizeof(__pyx_k_deepspeech_Model), 0, 0, 1, 0},
     {&__pyx_n_s_delta, __pyx_k_delta, sizeof(__pyx_k_delta), 0, 0, 1, 1},
     {&__pyx_n_s_deque, __pyx_k_deque, sizeof(__pyx_k_deque), 0, 0, 1, 1},
@@ -14680,15 +14922,14 @@
     {&__pyx_n_s_is_recording, __pyx_k_is_recording, sizeof(__pyx_k_is_recording), 0, 0, 1, 1},
     {&__pyx_n_s_is_set, __pyx_k_is_set, sizeof(__pyx_k_is_set), 0, 0, 1, 1},
     {&__pyx_n_s_is_speech, __pyx_k_is_speech, sizeof(__pyx_k_is_speech), 0, 0, 1, 1},
     {&__pyx_n_s_is_timeout, __pyx_k_is_timeout, sizeof(__pyx_k_is_timeout), 0, 0, 1, 1},
     {&__pyx_n_s_is_timeout_2, __pyx_k_is_timeout_2, sizeof(__pyx_k_is_timeout_2), 0, 0, 1, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_n_s_join, __pyx_k_join, sizeof(__pyx_k_join), 0, 0, 1, 1},
-    {&__pyx_n_s_last_command, __pyx_k_last_command, sizeof(__pyx_k_last_command), 0, 0, 1, 1},
     {&__pyx_n_s_log_to_stderr, __pyx_k_log_to_stderr, sizeof(__pyx_k_log_to_stderr), 0, 0, 1, 1},
     {&__pyx_n_s_logger, __pyx_k_logger, sizeof(__pyx_k_logger), 0, 0, 1, 1},
     {&__pyx_n_s_logging, __pyx_k_logging, sizeof(__pyx_k_logging), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_maxlen, __pyx_k_maxlen, sizeof(__pyx_k_maxlen), 0, 0, 1, 1},
     {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
     {&__pyx_n_s_millis, __pyx_k_millis, sizeof(__pyx_k_millis), 0, 0, 1, 1},
@@ -14696,15 +14937,14 @@
     {&__pyx_n_s_model, __pyx_k_model, sizeof(__pyx_k_model), 0, 0, 1, 1},
     {&__pyx_n_s_model_full_path, __pyx_k_model_full_path, sizeof(__pyx_k_model_full_path), 0, 0, 1, 1},
     {&__pyx_n_s_models, __pyx_k_models, sizeof(__pyx_k_models), 0, 0, 1, 1},
     {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
     {&__pyx_n_s_mro_entries, __pyx_k_mro_entries, sizeof(__pyx_k_mro_entries), 0, 0, 1, 1},
     {&__pyx_n_s_multiprocessing, __pyx_k_multiprocessing, sizeof(__pyx_k_multiprocessing), 0, 0, 1, 1},
     {&__pyx_n_s_multiprocessing_connection, __pyx_k_multiprocessing_connection, sizeof(__pyx_k_multiprocessing_connection), 0, 0, 1, 1},
-    {&__pyx_n_s_multiprocessing_sharedctypes, __pyx_k_multiprocessing_sharedctypes, sizeof(__pyx_k_multiprocessing_sharedctypes), 0, 0, 1, 1},
     {&__pyx_n_s_multiprocessing_synchronize, __pyx_k_multiprocessing_synchronize, sizeof(__pyx_k_multiprocessing_synchronize), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
     {&__pyx_n_s_now, __pyx_k_now, sizeof(__pyx_k_now), 0, 0, 1, 1},
     {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
     {&__pyx_n_s_num_padding_frames, __pyx_k_num_padding_frames, sizeof(__pyx_k_num_padding_frames), 0, 0, 1, 1},
     {&__pyx_n_s_num_unvoiced, __pyx_k_num_unvoiced, sizeof(__pyx_k_num_unvoiced), 0, 0, 1, 1},
@@ -14792,164 +15032,164 @@
     {&__pyx_n_s_writeframes, __pyx_k_writeframes, sizeof(__pyx_k_writeframes), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_property = __Pyx_GetBuiltinName(__pyx_n_s_property); if (!__pyx_builtin_property) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_builtin_property = __Pyx_GetBuiltinName(__pyx_n_s_property); if (!__pyx_builtin_property) __PYX_ERR(0, 84, __pyx_L1_error)
   __pyx_builtin_filter = __Pyx_GetBuiltinName(__pyx_n_s_filter); if (!__pyx_builtin_filter) __PYX_ERR(0, 311, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":87
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":86
  *     @property
  *     def command(self) -> Command:
  *         with self._command.get_lock():             # <<<<<<<<<<<<<<
  *             command = Command(self._command.get_obj().value)
  *             return command
  */
-  __pyx_tuple_ = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
   /* "tactigon_speech/middleware/Tactigon_Speech.py":312
  *     def check_branch(self, text: str):
  *         word_list = list(filter(lambda t: len(t) > 1 , text.split(" ")))
  *         if self.stop_hotword and self.stop_hotword.word in word_list[-2::]:             # <<<<<<<<<<<<<<
  *             self.tree_path.append(self.stop_hotword)
  *             return
  */
   __pyx_slice__5 = PySlice_New(__pyx_int_neg_2, Py_None, Py_None); if (unlikely(!__pyx_slice__5)) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__5);
   __Pyx_GIVEREF(__pyx_slice__5);
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":23
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":22
  * # from tactigon_gear.middleware import Tactigon_Audio
  * 
  * def millis():             # <<<<<<<<<<<<<<
  *     return datetime.now()
  * 
  */
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_millis, 23, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_millis, 22, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 22, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":54
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":53
  *     stop_hotword: Optional[HotWord]
  * 
  *     def __init__(self, config: VoiceConfig, audio_source: AudioSource, audio: _ConnectionBase, interface: _ConnectionBase, debug: bool = False):             # <<<<<<<<<<<<<<
  *         Process.__init__(self)
  * 
  */
-  __pyx_tuple__9 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_config, __pyx_n_s_audio_source, __pyx_n_s_audio, __pyx_n_s_interface, __pyx_n_s_debug); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_config, __pyx_n_s_audio_source, __pyx_n_s_audio, __pyx_n_s_interface, __pyx_n_s_debug); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_init, 54, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 54, __pyx_L1_error)
-  __pyx_tuple__11 = PyTuple_Pack(1, ((PyObject *)Py_False)); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_init, 53, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(1, ((PyObject *)Py_False)); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":85
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":84
  *         self.stop_hotword = config.stop_hotword
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def command(self) -> Command:
  *         with self._command.get_lock():
  */
-  __pyx_tuple__12 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_command_2); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_command_2); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_command_2, 85, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_command_2, 84, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 84, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":91
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":90
  *             return command
  * 
  *     @command.setter             # <<<<<<<<<<<<<<
  *     def command(self, command: Command):
  *         self.logger.debug("Setting command %s", command.name)
  */
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_command_2, 91, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_command_2, 90, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 90, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":97
- *             self._command.get_obj().value = command.value
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":96
+ *             self._command.get_obj().value = command.value #type: ignore
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def initialized(self):
  *         return self.command is not Command.NOT_INITIALIZED
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_initialized, 97, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_initialized, 96, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 96, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":101
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":100
  *         return self.command is not Command.NOT_INITIALIZED
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_recording(self):
  *         return self.command is Command.RECORD
  */
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_is_recording, 101, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_is_recording, 100, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 100, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":105
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":104
  *         return self.command is Command.RECORD
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_listening(self):
  *         return self.command is Command.LISTEN
  */
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_is_listening, 105, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_is_listening, 104, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 104, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":109
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":108
  *         return self.command is Command.LISTEN
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_playing(self):
  *         return self.command is Command.PLAY
  */
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_is_playing, 109, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_is_playing, 108, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 108, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":113
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":112
  *         return self.command is Command.PLAY
  * 
  *     def is_timeout(self, tick: datetime, timeout: int):             # <<<<<<<<<<<<<<
  *         return (millis() - tick).total_seconds() > timeout
  * 
  */
-  __pyx_tuple__20 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_tick, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_tick, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_is_timeout, 113, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_is_timeout, 112, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 112, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":116
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":115
  *         return (millis() - tick).total_seconds() > timeout
  * 
  *     def vad_collector(self) -> Generator[bytes, bytes, None]:             # <<<<<<<<<<<<<<
  *         frame_length = int(2 * self._SAMPLE_RATE * self.vad_frame / 1000)
  *         num_padding_frames: int = int(frame_length * (self.vad_padding_ms / 10000))
  */
-  __pyx_tuple__22 = PyTuple_Pack(18, __pyx_n_s_self, __pyx_n_s_frame_length, __pyx_n_s_num_padding_frames, __pyx_n_s_num_voiced_threshold, __pyx_n_s_triggered, __pyx_n_s_ring_buffer, __pyx_n_s_frame, __pyx_n_s_ticks, __pyx_n_s_audio_bytes, __pyx_n_s_is_speech, __pyx_n_s_num_voiced, __pyx_n_s_f, __pyx_n_s_s, __pyx_n_s_num_unvoiced, __pyx_n_s_f, __pyx_n_s_speech, __pyx_n_s_f, __pyx_n_s_speech); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(18, __pyx_n_s_self, __pyx_n_s_frame_length, __pyx_n_s_num_padding_frames, __pyx_n_s_num_voiced_threshold, __pyx_n_s_triggered, __pyx_n_s_ring_buffer, __pyx_n_s_frame, __pyx_n_s_ticks, __pyx_n_s_audio_bytes, __pyx_n_s_is_speech, __pyx_n_s_num_voiced, __pyx_n_s_f, __pyx_n_s_s, __pyx_n_s_num_unvoiced, __pyx_n_s_f, __pyx_n_s_speech, __pyx_n_s_f, __pyx_n_s_speech); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 18, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_GENERATOR, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_vad_collector, 116, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 18, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_GENERATOR, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_vad_collector, 115, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 115, __pyx_L1_error)
 
   /* "tactigon_speech/middleware/Tactigon_Speech.py":175
  *         return None
  * 
  *     def run(self):             # <<<<<<<<<<<<<<
  *         self.logger.debug("Creating PyAudio")
  *         self.pa = PyAudio()
  */
-  __pyx_tuple__23 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_last_command, __pyx_n_s_transcription, __pyx_n_s_speech_tree, __pyx_n_s_e, __pyx_n_s_filename); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_current_command, __pyx_n_s_transcription, __pyx_n_s_speech_tree, __pyx_n_s_e, __pyx_n_s_filename); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
   __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tactigon_speech_middleware_Tacti_2, __pyx_n_s_run, 175, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 175, __pyx_L1_error)
 
   /* "tactigon_speech/middleware/Tactigon_Speech.py":247
  *         self.logger.debug("Stopped")
  * 
@@ -15095,23 +15335,23 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector_spec, NULL); if (unlikely(!__pyx_ptype_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector)) __PYX_ERR(0, 116, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector_spec, __pyx_ptype_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_ptype_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector_spec, NULL); if (unlikely(!__pyx_ptype_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector)) __PYX_ERR(0, 115, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector_spec, __pyx_ptype_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
   #else
   __pyx_ptype_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector = &__pyx_type_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector->tp_dictoffset && __pyx_ptype_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_15tactigon_speech_10middleware_15Tactigon_Speech___pyx_scope_struct__vad_collector->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
@@ -15620,15 +15860,15 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "tactigon_speech/middleware/Tactigon_Speech.py":13
  * from webrtcvad import Vad
  * from multiprocessing import Process, Value, Event, log_to_stderr
  * from multiprocessing.connection import _ConnectionBase             # <<<<<<<<<<<<<<
  * from multiprocessing.synchronize import Event as EventClass
- * from multiprocessing.sharedctypes import SynchronizedBase
+ * 
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_ConnectionBase);
   __Pyx_GIVEREF(__pyx_n_s_ConnectionBase);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_ConnectionBase)) __PYX_ERR(0, 13, __pyx_L1_error);
   __pyx_t_3 = __Pyx_Import(__pyx_n_s_multiprocessing_connection, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
@@ -15640,16 +15880,16 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "tactigon_speech/middleware/Tactigon_Speech.py":14
  * from multiprocessing import Process, Value, Event, log_to_stderr
  * from multiprocessing.connection import _ConnectionBase
  * from multiprocessing.synchronize import Event as EventClass             # <<<<<<<<<<<<<<
- * from multiprocessing.sharedctypes import SynchronizedBase
  * 
+ * from typing import Optional, List, Generator
  */
   __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_Event);
   __Pyx_GIVEREF(__pyx_n_s_Event);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_Event)) __PYX_ERR(0, 14, __pyx_L1_error);
   __pyx_t_2 = __Pyx_Import(__pyx_n_s_multiprocessing_synchronize, __pyx_t_3, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
@@ -15657,425 +15897,411 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Event); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_EventClass, __pyx_t_3) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":15
- * from multiprocessing.connection import _ConnectionBase
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":16
  * from multiprocessing.synchronize import Event as EventClass
- * from multiprocessing.sharedctypes import SynchronizedBase             # <<<<<<<<<<<<<<
- * 
- * from typing import Optional, List, Generator
- */
-  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_n_s_SynchronizedBase);
-  __Pyx_GIVEREF(__pyx_n_s_SynchronizedBase);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_SynchronizedBase)) __PYX_ERR(0, 15, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_Import(__pyx_n_s_multiprocessing_sharedctypes, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_SynchronizedBase); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SynchronizedBase, __pyx_t_2) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":17
- * from multiprocessing.sharedctypes import SynchronizedBase
  * 
  * from typing import Optional, List, Generator             # <<<<<<<<<<<<<<
  * 
- * from ..models import VoiceConfig, AudioSource, Command, HotWord, TSpeech, TSpeechObject, Transcription
+ * from ..models import VoiceConfig, AudioSource, Command, HotWord, TSpeech, TSpeechObject, Transcription, InterfaceObject
  */
-  __pyx_t_3 = PyList_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = PyList_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_Optional);
   __Pyx_GIVEREF(__pyx_n_s_Optional);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_Optional)) __PYX_ERR(0, 17, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Optional)) __PYX_ERR(0, 16, __pyx_L1_error);
   __Pyx_INCREF(__pyx_n_s_List);
   __Pyx_GIVEREF(__pyx_n_s_List);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 1, __pyx_n_s_List)) __PYX_ERR(0, 17, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_List)) __PYX_ERR(0, 16, __pyx_L1_error);
   __Pyx_INCREF(__pyx_n_s_Generator);
   __Pyx_GIVEREF(__pyx_n_s_Generator);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 2, __pyx_n_s_Generator)) __PYX_ERR(0, 17, __pyx_L1_error);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_typing, __pyx_t_3, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Optional); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Optional, __pyx_t_3) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_List); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_List, __pyx_t_3) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Generator); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 2, __pyx_n_s_Generator)) __PYX_ERR(0, 16, __pyx_L1_error);
+  __pyx_t_3 = __Pyx_Import(__pyx_n_s_typing, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Generator, __pyx_t_3) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Optional); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Optional, __pyx_t_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_List); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_List, __pyx_t_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Generator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Generator, __pyx_t_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":19
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":18
  * from typing import Optional, List, Generator
  * 
- * from ..models import VoiceConfig, AudioSource, Command, HotWord, TSpeech, TSpeechObject, Transcription             # <<<<<<<<<<<<<<
+ * from ..models import VoiceConfig, AudioSource, Command, HotWord, TSpeech, TSpeechObject, Transcription, InterfaceObject             # <<<<<<<<<<<<<<
  * 
  * # from tactigon_gear.middleware import Tactigon_Audio
  */
-  __pyx_t_2 = PyList_New(7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyList_New(8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_VoiceConfig);
   __Pyx_GIVEREF(__pyx_n_s_VoiceConfig);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_VoiceConfig)) __PYX_ERR(0, 19, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_VoiceConfig)) __PYX_ERR(0, 18, __pyx_L1_error);
   __Pyx_INCREF(__pyx_n_s_AudioSource);
   __Pyx_GIVEREF(__pyx_n_s_AudioSource);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_AudioSource)) __PYX_ERR(0, 19, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 1, __pyx_n_s_AudioSource)) __PYX_ERR(0, 18, __pyx_L1_error);
   __Pyx_INCREF(__pyx_n_s_Command);
   __Pyx_GIVEREF(__pyx_n_s_Command);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 2, __pyx_n_s_Command)) __PYX_ERR(0, 19, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 2, __pyx_n_s_Command)) __PYX_ERR(0, 18, __pyx_L1_error);
   __Pyx_INCREF(__pyx_n_s_HotWord);
   __Pyx_GIVEREF(__pyx_n_s_HotWord);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 3, __pyx_n_s_HotWord)) __PYX_ERR(0, 19, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 3, __pyx_n_s_HotWord)) __PYX_ERR(0, 18, __pyx_L1_error);
   __Pyx_INCREF(__pyx_n_s_TSpeech);
   __Pyx_GIVEREF(__pyx_n_s_TSpeech);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 4, __pyx_n_s_TSpeech)) __PYX_ERR(0, 19, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 4, __pyx_n_s_TSpeech)) __PYX_ERR(0, 18, __pyx_L1_error);
   __Pyx_INCREF(__pyx_n_s_TSpeechObject);
   __Pyx_GIVEREF(__pyx_n_s_TSpeechObject);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 5, __pyx_n_s_TSpeechObject)) __PYX_ERR(0, 19, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 5, __pyx_n_s_TSpeechObject)) __PYX_ERR(0, 18, __pyx_L1_error);
   __Pyx_INCREF(__pyx_n_s_Transcription);
   __Pyx_GIVEREF(__pyx_n_s_Transcription);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 6, __pyx_n_s_Transcription)) __PYX_ERR(0, 19, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_Import(__pyx_n_s_models, __pyx_t_2, 2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_VoiceConfig); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_VoiceConfig, __pyx_t_2) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_AudioSource); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_AudioSource, __pyx_t_2) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Command); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Command, __pyx_t_2) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_HotWord); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 6, __pyx_n_s_Transcription)) __PYX_ERR(0, 18, __pyx_L1_error);
+  __Pyx_INCREF(__pyx_n_s_InterfaceObject);
+  __Pyx_GIVEREF(__pyx_n_s_InterfaceObject);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 7, __pyx_n_s_InterfaceObject)) __PYX_ERR(0, 18, __pyx_L1_error);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_models, __pyx_t_3, 2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_HotWord, __pyx_t_2) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_TSpeech); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TSpeech, __pyx_t_2) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_TSpeechObject); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TSpeechObject, __pyx_t_2) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Transcription); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Transcription, __pyx_t_2) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_VoiceConfig); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_VoiceConfig, __pyx_t_3) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_AudioSource); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_AudioSource, __pyx_t_3) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Command); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Command, __pyx_t_3) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_HotWord); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_HotWord, __pyx_t_3) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_TSpeech); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TSpeech, __pyx_t_3) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_TSpeechObject); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TSpeechObject, __pyx_t_3) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Transcription); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Transcription, __pyx_t_3) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_InterfaceObject); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InterfaceObject, __pyx_t_3) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":23
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":22
  * # from tactigon_gear.middleware import Tactigon_Audio
  * 
  * def millis():             # <<<<<<<<<<<<<<
  *     return datetime.now()
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_1millis, 0, __pyx_n_s_millis, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_millis, __pyx_t_3) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_1millis, 0, __pyx_n_s_millis, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_millis, __pyx_t_2) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":26
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":25
  *     return datetime.now()
  * 
  * class Tactigon_Speech(Process):             # <<<<<<<<<<<<<<
  *     _TICK: float = 0.02
  *     _PIPE_TIMEOUT: float = 0.1
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Process); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Process); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error);
-  __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error);
+  __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PEP560_update_bases(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_3, __pyx_n_s_Tactigon_Speech, __pyx_n_s_Tactigon_Speech, (PyObject *) NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, (PyObject *) NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_2, __pyx_n_s_Tactigon_Speech, __pyx_n_s_Tactigon_Speech, (PyObject *) NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, (PyObject *) NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__pyx_t_3 != __pyx_t_2) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_2) < 0))) __PYX_ERR(0, 26, __pyx_L1_error)
+  if (__pyx_t_2 != __pyx_t_3) {
+    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_3) < 0))) __PYX_ERR(0, 25, __pyx_L1_error)
   }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(21); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_TICK, __pyx_n_s_float) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_PIPE_TIMEOUT, __pyx_n_s_float) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_SINGLE_FRAME_LENGTH, __pyx_n_s_int) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_SAMPLE_RATE, __pyx_n_s_int) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_INTERFACE_TIMEOUT, __pyx_n_s_float) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_stop_event, __pyx_n_s_EventClass) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_audio, __pyx_n_s_ConnectionBase) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_interface, __pyx_n_s_ConnectionBase) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_audio_source, __pyx_n_s_AudioSource) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_pa, __pyx_n_s_PyAudio) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_model, __pyx_kp_s_deepspeech_Model) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_vad_frame, __pyx_n_s_int) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_vad_padding_ms, __pyx_n_s_int) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_vad_ratio, __pyx_n_s_float) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_silence_timeout, __pyx_n_s_int) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_voice_timeout, __pyx_n_s_int) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_vad_aggressiveness, __pyx_n_s_int) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_model_full_path, __pyx_n_s_str) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_scorer_full_path, __pyx_kp_s_Optional_str) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_beam_width, __pyx_n_s_int) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_stop_hotword, __pyx_kp_s_Optional_HotWord) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_annotations, __pyx_t_2) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(21); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_TICK, __pyx_n_s_float) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_PIPE_TIMEOUT, __pyx_n_s_float) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_SINGLE_FRAME_LENGTH, __pyx_n_s_int) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_SAMPLE_RATE, __pyx_n_s_int) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_INTERFACE_TIMEOUT, __pyx_n_s_float) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_stop_event, __pyx_n_s_EventClass) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_audio, __pyx_n_s_ConnectionBase) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_interface, __pyx_n_s_ConnectionBase) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_audio_source, __pyx_n_s_AudioSource) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_pa, __pyx_n_s_PyAudio) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_model, __pyx_kp_s_deepspeech_Model) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_vad_frame, __pyx_n_s_int) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_vad_padding_ms, __pyx_n_s_int) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_vad_ratio, __pyx_n_s_float) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_silence_timeout, __pyx_n_s_int) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_voice_timeout, __pyx_n_s_int) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_vad_aggressiveness, __pyx_n_s_int) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_model_full_path, __pyx_n_s_str) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_scorer_full_path, __pyx_kp_s_Optional_str) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_beam_width, __pyx_n_s_int) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_stop_hotword, __pyx_kp_s_Optional_HotWord) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_annotations, __pyx_t_3) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":27
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":26
  * 
  * class Tactigon_Speech(Process):
  *     _TICK: float = 0.02             # <<<<<<<<<<<<<<
  *     _PIPE_TIMEOUT: float = 0.1
  *     _SINGLE_FRAME_LENGTH: int = 80
  */
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_TICK, __pyx_float_0_02) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_TICK, __pyx_float_0_02) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":28
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":27
  * class Tactigon_Speech(Process):
  *     _TICK: float = 0.02
  *     _PIPE_TIMEOUT: float = 0.1             # <<<<<<<<<<<<<<
  *     _SINGLE_FRAME_LENGTH: int = 80
  *     _SAMPLE_RATE: int = 16000
  */
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_PIPE_TIMEOUT, __pyx_float_0_1) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_PIPE_TIMEOUT, __pyx_float_0_1) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":29
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":28
  *     _TICK: float = 0.02
  *     _PIPE_TIMEOUT: float = 0.1
  *     _SINGLE_FRAME_LENGTH: int = 80             # <<<<<<<<<<<<<<
  *     _SAMPLE_RATE: int = 16000
  * 
  */
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_SINGLE_FRAME_LENGTH, __pyx_int_80) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_SINGLE_FRAME_LENGTH, __pyx_int_80) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":30
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":29
  *     _PIPE_TIMEOUT: float = 0.1
  *     _SINGLE_FRAME_LENGTH: int = 80
  *     _SAMPLE_RATE: int = 16000             # <<<<<<<<<<<<<<
  * 
  *     _INTERFACE_TIMEOUT: float = 0.2
  */
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_SAMPLE_RATE, __pyx_int_16000) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_SAMPLE_RATE, __pyx_int_16000) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":32
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":31
  *     _SAMPLE_RATE: int = 16000
  * 
  *     _INTERFACE_TIMEOUT: float = 0.2             # <<<<<<<<<<<<<<
  * 
  *     _stop_event: EventClass
  */
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_INTERFACE_TIMEOUT, __pyx_float_0_2) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_INTERFACE_TIMEOUT, __pyx_float_0_2) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":54
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":53
  *     stop_hotword: Optional[HotWord]
  * 
  *     def __init__(self, config: VoiceConfig, audio_source: AudioSource, audio: _ConnectionBase, interface: _ConnectionBase, debug: bool = False):             # <<<<<<<<<<<<<<
  *         Process.__init__(self)
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_config, __pyx_n_s_VoiceConfig) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_audio_source, __pyx_n_s_AudioSource) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_audio, __pyx_n_s_ConnectionBase) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_interface, __pyx_n_s_ConnectionBase) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_debug, __pyx_n_s_bool) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_1__init__, 0, __pyx_n_s_Tactigon_Speech___init, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_config, __pyx_n_s_VoiceConfig) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_audio_source, __pyx_n_s_AudioSource) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_audio, __pyx_n_s_ConnectionBase) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_interface, __pyx_n_s_ConnectionBase) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_debug, __pyx_n_s_bool) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_1__init__, 0, __pyx_n_s_Tactigon_Speech___init, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_6, __pyx_tuple__11);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_init, __pyx_t_6) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_3);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_init, __pyx_t_6) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":85
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":84
  *         self.stop_hotword = config.stop_hotword
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def command(self) -> Command:
  *         with self._command.get_lock():
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_return, __pyx_n_s_Command) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_3command, 0, __pyx_n_s_Tactigon_Speech_command, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_return, __pyx_n_s_Command) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_3command, 0, __pyx_n_s_Tactigon_Speech_command, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_6);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_command_2, __pyx_t_6) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_command_2, __pyx_t_6) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":91
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":90
  *             return command
  * 
  *     @command.setter             # <<<<<<<<<<<<<<
  *     def command(self, command: Command):
  *         self.logger.debug("Setting command %s", command.name)
  */
-  __pyx_t_2 = PyObject_GetItem(__pyx_t_5, __pyx_n_s_command_2);
-  if (unlikely(!__pyx_t_2)) {
+  __pyx_t_3 = PyObject_GetItem(__pyx_t_5, __pyx_n_s_command_2);
+  if (unlikely(!__pyx_t_3)) {
     PyErr_Clear();
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_command_2);
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_command_2);
   }
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_setter); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 91, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_setter); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_command_2, __pyx_n_s_Command) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_5command, 0, __pyx_n_s_Tactigon_Speech_command, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_command_2, __pyx_n_s_Command) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_5command, 0, __pyx_n_s_Tactigon_Speech_command, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_8, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = NULL;
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_8, __pyx_t_3);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = NULL;
   __pyx_t_9 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_7))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_7);
-    if (likely(__pyx_t_2)) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
+    if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
       __pyx_t_9 = 1;
     }
   }
   #endif
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_8};
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_8};
     __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_9, 1+__pyx_t_9);
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 91, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_command_2, __pyx_t_6) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_command_2, __pyx_t_6) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":97
- *             self._command.get_obj().value = command.value
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":96
+ *             self._command.get_obj().value = command.value #type: ignore
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def initialized(self):
  *         return self.command is not Command.NOT_INITIALIZED
  */
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_7initialized, 0, __pyx_n_s_Tactigon_Speech_initialized, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_7initialized, 0, __pyx_n_s_Tactigon_Speech_initialized, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_initialized, __pyx_t_7) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_initialized, __pyx_t_7) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":101
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":100
  *         return self.command is not Command.NOT_INITIALIZED
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_recording(self):
  *         return self.command is Command.RECORD
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_9is_recording, 0, __pyx_n_s_Tactigon_Speech_is_recording, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_9is_recording, 0, __pyx_n_s_Tactigon_Speech_is_recording, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_is_recording, __pyx_t_6) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_is_recording, __pyx_t_6) < 0) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":105
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":104
  *         return self.command is Command.RECORD
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_listening(self):
  *         return self.command is Command.LISTEN
  */
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_11is_listening, 0, __pyx_n_s_Tactigon_Speech_is_listening, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_11is_listening, 0, __pyx_n_s_Tactigon_Speech_is_listening, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_is_listening, __pyx_t_7) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_is_listening, __pyx_t_7) < 0) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":109
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":108
  *         return self.command is Command.LISTEN
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_playing(self):
  *         return self.command is Command.PLAY
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_13is_playing, 0, __pyx_n_s_Tactigon_Speech_is_playing, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_13is_playing, 0, __pyx_n_s_Tactigon_Speech_is_playing, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_is_playing, __pyx_t_6) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_is_playing, __pyx_t_6) < 0) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":113
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":112
  *         return self.command is Command.PLAY
  * 
  *     def is_timeout(self, tick: datetime, timeout: int):             # <<<<<<<<<<<<<<
  *         return (millis() - tick).total_seconds() > timeout
  * 
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_tick, __pyx_n_s_datetime) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_timeout, __pyx_n_s_int) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_15is_timeout, 0, __pyx_n_s_Tactigon_Speech_is_timeout, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 113, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_tick, __pyx_n_s_datetime) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_timeout, __pyx_n_s_int) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_15is_timeout, 0, __pyx_n_s_Tactigon_Speech_is_timeout, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_6);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_is_timeout, __pyx_t_7) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_is_timeout, __pyx_t_7) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":116
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":115
  *         return (millis() - tick).total_seconds() > timeout
  * 
  *     def vad_collector(self) -> Generator[bytes, bytes, None]:             # <<<<<<<<<<<<<<
  *         frame_length = int(2 * self._SAMPLE_RATE * self.vad_frame / 1000)
  *         num_padding_frames: int = int(frame_length * (self.vad_padding_ms / 10000))
  */
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_return, __pyx_kp_s_Generator_bytes_bytes_None) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_17vad_collector, 0, __pyx_n_s_Tactigon_Speech_vad_collector, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 116, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_return, __pyx_kp_s_Generator_bytes_bytes_None) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_17vad_collector, 0, __pyx_n_s_Tactigon_Speech_vad_collector, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_vad_collector, __pyx_t_6) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_vad_collector, __pyx_t_6) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   /* "tactigon_speech/middleware/Tactigon_Speech.py":175
  *         return None
  * 
  *     def run(self):             # <<<<<<<<<<<<<<
  *         self.logger.debug("Creating PyAudio")
@@ -16181,38 +16407,38 @@
  *         i = 0
  */
   __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_15tactigon_speech_10middleware_15Tactigon_Speech_15Tactigon_Speech_32clear_audio_pipe, 0, __pyx_n_s_Tactigon_Speech_clear_audio_pipe, NULL, __pyx_n_s_tactigon_speech_middleware_Tacti, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 353, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_clear_audio_pipe, __pyx_t_7) < 0) __PYX_ERR(0, 353, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "tactigon_speech/middleware/Tactigon_Speech.py":26
+  /* "tactigon_speech/middleware/Tactigon_Speech.py":25
  *     return datetime.now()
  * 
  * class Tactigon_Speech(Process):             # <<<<<<<<<<<<<<
  *     _TICK: float = 0.02
  *     _PIPE_TIMEOUT: float = 0.1
  */
-  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_Tactigon_Speech, __pyx_t_3, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_Tactigon_Speech, __pyx_t_2, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Tactigon_Speech, __pyx_t_7) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Tactigon_Speech, __pyx_t_7) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "tactigon_speech/middleware/Tactigon_Speech.py":1
  * import logging             # <<<<<<<<<<<<<<
  * import deepspeech
  * import collections
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
```

### Comparing `tactigon_speech-5.0.3.post1/tactigon_speech/models.py` & `tactigon_speech-5.0.4/tactigon_speech/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,19 @@
     def toJSON(self) -> object:
         return {
             "text": self.text,
             "path": [hw.toJSON() for hw in self.path] if self.path else None,
             "time": self.time,
             "timeout": self.timeout
         }
+    
+@dataclass
+class InterfaceObject:
+    command: Command
+    payload: Union[Transcription, str, bool]
 
 @dataclass
 class VoiceConfig:
     model: str
     scorer: Optional[str] = None
 
     vad_aggressiveness: int = 3
```

### Comparing `tactigon_speech-5.0.3.post1/tactigon_speech.egg-info/PKG-INFO` & `tactigon_speech-5.0.4/tactigon_speech.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tactigon_speech
-Version: 5.0.3.post1
+Version: 5.0.4
 Summary: Tactigon Speech to transcribe text into commands
 Home-page: https://nextind.eu
 Author: Next Industries s.r.l.
 Author-email: info@nextind.eu
 License: MIT
 Keywords: tactigon,wereable,voice recognition on edge,human interface
 Classifier: Programming Language :: Python :: 3
```

