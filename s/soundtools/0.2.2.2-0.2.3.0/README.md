# Comparing `tmp/soundtools-0.2.2.2.tar.gz` & `tmp/soundtools-0.2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundtools-0.2.2.2.tar", last modified: Mon May 13 12:40:42 2024, max compression
+gzip compressed data, was "soundtools-0.2.3.0.tar", last modified: Thu May 23 18:39:34 2024, max compression
```

## Comparing `soundtools-0.2.2.2.tar` & `soundtools-0.2.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 12:40:42.951738 soundtools-0.2.2.2/
--rw-rw-rw-   0        0        0      701 2024-05-13 12:40:42.950380 soundtools-0.2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 12:40:42.951738 soundtools-0.2.2.2/setup.cfg
--rw-rw-rw-   0        0        0      789 2024-05-13 12:40:14.000000 soundtools-0.2.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:40:42.947260 soundtools-0.2.2.2/soundtools/
--rw-rw-rw-   0        0        0      399 2024-05-13 12:40:09.000000 soundtools-0.2.2.2/soundtools/__init__.py
--rw-rw-rw-   0        0        0    34937 2024-05-13 12:40:07.000000 soundtools-0.2.2.2/soundtools/soundtools.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:40:42.950380 soundtools-0.2.2.2/soundtools.egg-info/
--rw-rw-rw-   0        0        0      701 2024-05-13 12:40:42.000000 soundtools-0.2.2.2/soundtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-05-13 12:40:42.000000 soundtools-0.2.2.2/soundtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 12:40:42.000000 soundtools-0.2.2.2/soundtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 12:40:42.000000 soundtools-0.2.2.2/soundtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 18:39:34.200210 soundtools-0.2.3.0/
+-rw-rw-rw-   0        0        0      701 2024-05-23 18:39:34.200210 soundtools-0.2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 18:39:34.201206 soundtools-0.2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      789 2024-05-23 18:36:40.000000 soundtools-0.2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:39:34.196223 soundtools-0.2.3.0/soundtools/
+-rw-rw-rw-   0        0        0      399 2024-05-23 18:36:08.000000 soundtools-0.2.3.0/soundtools/__init__.py
+-rw-rw-rw-   0        0        0    36223 2024-05-23 18:38:53.000000 soundtools-0.2.3.0/soundtools/soundtools.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:39:34.199213 soundtools-0.2.3.0/soundtools.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-05-23 18:39:34.000000 soundtools-0.2.3.0/soundtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-05-23 18:39:34.000000 soundtools-0.2.3.0/soundtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 18:39:34.000000 soundtools-0.2.3.0/soundtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-23 18:39:34.000000 soundtools-0.2.3.0/soundtools.egg-info/top_level.txt
```

### Comparing `soundtools-0.2.2.2/PKG-INFO` & `soundtools-0.2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: soundtools
-Version: 0.2.2.2
+Version: 0.2.3.0
 Summary: used to work with sounds waves
 Author: Mohammad Erfan Karami
 Author-email: erfan012amir016@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
 made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.2.2
+version: 0.2.3.0
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves
```

### Comparing `soundtools-0.2.2.2/setup.py` & `soundtools-0.2.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 setup(
 name='soundtools',
-version='0.2.2.2',
+version='0.2.3.0',
 description="used to work with sounds waves",
 long_description="""made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.2.2
+version: 0.2.3.0
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves""",
 author='Mohammad Erfan Karami',
```

### Comparing `soundtools-0.2.2.2/soundtools/soundtools.py` & `soundtools-0.2.3.0/soundtools/soundtools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """### made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-### version: 0.2.2.2
+### version: 0.2.3.0
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves"""
 
 
 import pyaudio
 import numpy as np
-from typing import Callable, Iterable, Literal
+from typing import Callable, Iterable, Literal, Self, Tuple, Dict, List
 import scipy.io.wavfile as wf
 import matplotlib.pyplot as plt
 import librosa.effects as effect
 from os.path import splitext
 from pydub.audio_segment import AudioSegment
 from soundfile import read as sfRead
 
@@ -25,15 +25,15 @@
 Dtype = np.dtype[np.float32|np.int16|np.uint8]
 SoundBuffer = np.ndarray[np.any, Dtype]
 Wave = Callable[[float, float, float], SoundBuffer]
 Note = str|float
 
 
 # its just a dictionary
-class Notes(dict[str, float]):
+class Notes(Dict[str, float]):
     """a dictionary used to store note names and frequencies"""
     def __init__(self):
         super().__init__()
     
     def __getitem__(self, __key: str) -> float:
         return super().__getitem__(__key.upper())
     
@@ -42,15 +42,15 @@
 
 
 #-- sound waves --#
 class Sounds:
     """has some basic sound waves and also caches the result of the functions for faster output"""
     def __init__(self, sample_rate: int=48000, dtype:Dtype=np.float32) -> None:
         self.default_sample_rate: int = sample_rate
-        self.existed_notes: dict[str, tuple] = {}
+        self.existed_notes: Dict[str, Tuple] = {}
         
         self.tau = 2*np.pi
         self.rev_pi = 1/np.pi
         self.two_oper_pi = 2/np.pi
         self.four_over_pi = 4/np.pi
         self.eight_over_pi_sqr = 8/np.pi**2
         
@@ -73,27 +73,27 @@
     # so this decorator will save a tuple of that numpy array in self.existed_notes and convert it back to a numpy array each time you want to use that wave
     def cache_wave(wave_type: str) -> SoundBuffer:
         """caches the waves so if you had to generate a note multiple times it's gonna use the cached wave. 
         you can't use the lru_cache from the functools module because waves are stored as numpy arrays and numpy arrays are not hashable, 
         so this decorator will store the numpy array as a tuple in "self.existed_notes" and convert it back to a numpy array each time you want to use that wave
         \nreturns the cached value if available, otherwise caches the returned wave"""
         def decorator(func: Wave) -> SoundBuffer:
-            def wrapper(self, freq:float, dur:float, vol: float):
+            def wrapper(self: Self, freq:float, dur:float, vol: float):
                 # Error if frequency is negative
                 if freq < 0:
                     raise f"frequency must be positive number, given frequency: {freq}"
                 
-                name = f"{wave_type}|{freq}|{dur}"
+                name = f"{wave_type}|{freq}|{dur}|{self.dtype}"
                 if name in self.existed_notes.keys():
                     wave = vol * np.array(self.existed_notes[name], dtype=self.dtype)
                     return wave
                 
                 temp = func(self, freq, dur, self.max_amp)
                 result: SoundBuffer = func(self, freq, dur, vol)
-                result = self._fix_amp(result)
+                result = self._fix_amp(result, -vol, vol)
                 self.existed_notes[name] = self.array_to_tuple(temp)
                 
                 return result
             return wrapper
         return decorator
 
     @cache_wave("sine")
@@ -116,17 +116,22 @@
         buf = np.sin(fund)
         
         n = np.ceil(20_000 / freq).astype(np.int16)
         for h in range(3, n, 2):
             #-- adding the harmonics --#
             buf += np.sin(fund*h) / h
         
-        wave = ((self.four_over_pi)*vol*buf).astype(self.dtype)
+        wave = (self.four_over_pi*vol*buf).astype(self.dtype)
         return wave
     
+    @cache_wave("fast_sqr")
+    def fast_square_wave(self, f: float, dur: float, vol: float) -> SoundBuffer:
+        """the result is same as square_wave but it's time complexity is O(1)"""
+        return vol * ((-1)**np.floor(2 * f / self.default_sample_rate * np.arange(dur * self.default_sample_rate))).astype(self.dtype)
+    
     @cache_wave("tri")
     def triangle_wave(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         """creates a triangle wave based on the given frequency, duration and amplitude or volume\n
         a triangle wave is typically generated by adding every second odd harmonic (5, 9, 13...) to a fundamental frequency\n
         each harmonic is added with a less volume which causes the amplitude to change a bit so at the end the amplitude is multiplied by '8/pi^2' to fix it\n
         returns a numpy array"""
         
@@ -139,14 +144,15 @@
             buf += (-1)**h * np.sin(fund * harmonic) / (harmonic*harmonic)
         
         wave = ((self.eight_over_pi_sqr)*vol*buf).astype(self.dtype)
         return wave
     
     @cache_wave("fast_tri")
     def fast_triangle_wave(self, freq:float, dur:float, vol: float) -> SoundBuffer:
+        """the result is same as triangle_wave but it's time complexity is O(1)"""
         return (self.two_oper_pi * vol * np.arcsin(np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate))).astype(self.dtype)
     
     @cache_wave("saw")
     def sawtooth_wave(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         """returns a numpy array,
         creates a sawtooth wave based on the given frequency, duration and amplitude or volume\n
         a sawtooth wave is typically generated by adding every harmonic to a fundamental frequency with the odd harmonics being negative (2, -3, 4, -5...)\n
@@ -156,17 +162,25 @@
         fund = self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate
         buf = np.sin(fund) * -1
         
         n = np.ceil(20_000 / freq).astype(np.int16)
         for h in range(2, n):
             buf += (-1)**h * (np.sin(fund * h) / h)
         
-        wave = (vol * ((-self.two_oper_pi)*buf)).astype(np.float32)
+        wave = (vol * ((-self.two_oper_pi)*buf)).astype(self.dtype)
         return wave
     
+    @cache_wave("fast_saw")
+    def fast_sawtooth_wave(self, freq: float, dur: float, vol: float) -> SoundBuffer:
+        """the result is same as sawtooth_wave but it's time complexity is O(1)"""
+        T = 1/freq / 2 * self.default_sample_rate
+        t = freq * np.arange(dur * self.default_sample_rate + T) / self.default_sample_rate
+        wave = (t - np.floor(t) - 0.5)[int(T):]
+        return 2 * vol * wave.astype(self.dtype)
+    
     def smooth_saw_wave(self, freq:float, dur:float, vol: float, smoothness: float=2.5) -> SoundBuffer:
         """creates a wave like saw wave but without the sharp points"""
         
         fund = self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate
         buf = np.sin(fund) * -1
         
         n = np.ceil(20_000 / freq).astype(np.int16)
@@ -216,17 +230,20 @@
         for h in range(1, 1000):
             buf += (-1)**h * (np.sin(fund * h) / h)
         
         wave = (vol * (0.5 - self.rev_pi*buf)).astype(self.dtype)
         return wave
     
     
-    def _fix_amp(self, wave: SoundBuffer) -> SoundBuffer:
-        wave[wave > self.max_amp] = self.max_amp
-        wave[wave < self.min_amp] = self.min_amp
+    def _fix_amp(self, wave: SoundBuffer, min_amp=None, max_amp=None) -> SoundBuffer:
+        if not min_amp: min_amp = self.min_amp
+        if not max_amp: max_amp = self.max_amp
+        
+        wave[wave > max_amp] = max_amp
+        wave[wave < min_amp] = min_amp
         return wave
     
     
     def _generate_fade_buffer(self, fade_len:int, start=0, stop=np.pi, dtype: Dtype|None=None) -> SoundBuffer:
         if not dtype:
             dtype = self.dtype
         
@@ -280,15 +297,15 @@
     
     def staccato(self, wave: SoundBuffer, play_time: float=0.75) -> SoundBuffer:
         playing = len(wave)*play_time
         resting = (1-play_time) * (wave.size/self.default_sample_rate)
         return np.append(wave[0:int(playing)], self.generate_note_buffer(0, self.sine_wave, resting))
     
     
-    def array_to_tuple(self, np_array: SoundBuffer) -> tuple:
+    def array_to_tuple(self, np_array: SoundBuffer) -> Tuple:
         """Iterates recursivelly."""
         try:
             return tuple(self.array_to_tuple(_) for _ in np_array)
         except TypeError:
             return np_array
 
 
@@ -453,15 +470,15 @@
     def __init__(self, middle_a=440, tempo=60, sample_rate=48000, tune=12) -> None:
         super().__init__(sample_rate)
         self.sample_rate: int = sample_rate
         self.AUDIO_OBJECT = pyaudio.PyAudio() # making an audio object that we,ll need to play sounds
         self.TUNE = tune                       # using 12 tone equal temperament
         self.MIDDLE_A = middle_a                  # middle a has a frecuency of 440 hertz
         self._NOTES: Notes = Notes()                 # a directory that has all the notes that we can use in it and R is just for rest
-        self.NOTE_NAMES: list[str] = list("ABCDEFGHIJKLMNOPQRSTUVWXYZ")
+        self.NOTE_NAMES: List[str] = list("ABCDEFGHIJKLMNOPQRSTUVWXYZ")
         self.FULL_NOTE_NAMES = []
         self.DEFAULT_DURATION = 1
         self.DEFAULT_VOLUME = self.max_amp
         self.tempo = tempo
         self.channels: int = 1
     
     
@@ -472,29 +489,31 @@
         self.generate_note_names()
         self.assign_middle_a()
         self.assign_frequencies()
         self.init_output_stream()
         self.init_input_stream()
     
     
-    def init_output_stream(self, samp_width:int|str="float32",
+    def init_output_stream(self,
+                           samp_width:int|str="float32",
                            n_channels:int|None=None,
                            sample_rate:int|None=None) -> None:
         
         if not n_channels:
             n_channels = self.channels
         if not sample_rate:
             sample_rate = self.sample_rate
         
         self.stream = self.config_stream(samp_width=samp_width,
                                          channels=n_channels,
                                          sample_rate=sample_rate)
     
     
-    def init_input_stream(self, samp_width: int|str="float32",
+    def init_input_stream(self,
+                          samp_width: int|str="float32",
                           n_channels: int=1,
                           sample_rate: int|None=None,
                           chunk:int=3200) -> None:
         if not sample_rate:
             sample_rate = self.sample_rate
         
         if type(samp_width) == str:
@@ -585,21 +604,24 @@
         else:
             duration = float(duration[:-1])
         
         return duration
     
     
     def fix_volume(self, volume:float=0) -> float:
-        if volume > self.max_amp or volume < self.min_amp:
+        if not volume:
+            volume = self.max_amp/2
+        
+        elif volume > self.max_amp or volume < self.min_amp:
             raise f"volume must be between {self.min_amp} and {self.max_amp}"
         
         return volume
     
     
-    def get_file_data(self, file_path: str) -> tuple[SoundBuffer, int]:
+    def get_file_data(self, file_path: str) -> Tuple[SoundBuffer, int]:
         """gets the file data and returns a tuple[wave, sample_rate]
         you ca access other information as shown below
         
         >>> channels = data.ndim
         >>> sample_width = data.dtype"""
         
         fformat = splitext(file_path)[1]
@@ -708,46 +730,50 @@
         
         self.input_stream.stop_stream()
         
         buf = np.frombuffer(total_frames, self.input_dtype)
         return buf
     
     
-    def add_buffers(a: SoundBuffer, b: SoundBuffer) -> SoundBuffer:
+    def add_buffers(a: SoundBuffer, b: SoundBuffer, keep_volume: bool=True) -> SoundBuffer:
         s = a.size if a.size < b.size else b.size
-        return (a[:s] + b[:s]) / 2
+        result = (a[:s] + b[:s])
+        if keep_volume: result /= 2
+        return result
     
     
-    def add_multiple_buffers(*buffers: SoundBuffer):
+    def add_multiple_buffers(*buffers: SoundBuffer, keep_volume: bool=True):
         s: int = buffers[0].size
         for buffer in buffers[1:]:
             if buffer.size < s:
                 s = buffer.size
         
         s_bufs: SoundBuffer = buffers[0][:s]
         
         for buffer in buffers[1:]:
             s_bufs += buffer[:s]
+        
+        if keep_volume: s_bufs /= len(buffers)
             
-        return s_bufs / len(buffers)
+        return s_bufs
     
     # creates a note buffer and plays it
     def play(self, note:str|float|int, wave_type: Wave, duration:str|float=0, volume:float=0) -> None:
         """generates then plays a note with the given arguments"""
         buf: bytes = self.generate_note_buffer(note, wave_type, duration, volume).tobytes()
     
         self.play_buffer(buf)
     
     
     # plays a buffer
     def play_buffer(self, wave: SoundBuffer|bytes, chunk:int=3200, dtype:Dtype|None=None) -> None:
         """plays the given wave"""
         
         if type(wave) == bytes:
-            dtype = self.dtype if not dtype else dtype
+            if not dtype: dtype = self.dtype
             wave = np.frombuffer(wave, self.dtype)
         
         n_chunks = int(wave.size / chunk)
         for i in range(n_chunks):
             b = wave[i*chunk : (i+1)*chunk].data.tobytes()
             self.stream.write(b)
         
@@ -785,15 +811,15 @@
                                              output=True)
         self.play_buffer(data)
     
     
     def visualize_sound(self, wave: SoundBuffer, sample_rate: int|None=None) -> None:
         """uses matplotlib.pyplot to visualize sound waves"""
         
-        sample_rate = self.sample_rate if not sample_rate else sample_rate
+        if not sample_rate: sample_rate = self.sample_rate
         
         times = np.linspace(0, wave.size/sample_rate, wave.size)
         duration = wave.size / sample_rate
         
         plt.figure(figsize=(15, 5))
         plt.plot(times, wave)
         plt.title('wave:')
```

### Comparing `soundtools-0.2.2.2/soundtools.egg-info/PKG-INFO` & `soundtools-0.2.3.0/soundtools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: soundtools
-Version: 0.2.2.2
+Version: 0.2.3.0
 Summary: used to work with sounds waves
 Author: Mohammad Erfan Karami
 Author-email: erfan012amir016@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
 made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.2.2
+version: 0.2.3.0
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves
```

