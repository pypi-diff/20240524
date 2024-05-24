# Comparing `tmp/apollo-ai-0.0.48.tar.gz` & `tmp/apollo-ai-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-ai-0.0.48.tar", last modified: Fri May 10 20:31:59 2024, max compression
+gzip compressed data, was "apollo-ai-0.0.49.tar", last modified: Fri May 24 20:12:37 2024, max compression
```

## Comparing `apollo-ai-0.0.48.tar` & `apollo-ai-0.0.49.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 20:31:59.653531 apollo-ai-0.0.48/
--rw-rw-rw-   0        0        0    35823 2023-09-19 22:57:32.000000 apollo-ai-0.0.48/LICENSE
--rw-rw-rw-   0        0        0     9511 2024-05-10 20:31:59.652490 apollo-ai-0.0.48/PKG-INFO
--rw-rw-rw-   0        0        0     8994 2023-11-08 20:42:11.000000 apollo-ai-0.0.48/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 20:31:59.361863 apollo-ai-0.0.48/apollo/
-drwxrwxrwx   0        0        0        0 2024-05-10 20:31:59.424573 apollo-ai-0.0.48/apollo/apollo_ai.egg-info/
--rw-rw-rw-   0        0        0     9511 2024-05-10 20:31:57.000000 apollo-ai-0.0.48/apollo/apollo_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2024-05-10 20:31:58.000000 apollo-ai-0.0.48/apollo/apollo_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 20:31:57.000000 apollo-ai-0.0.48/apollo/apollo_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      596 2024-05-10 20:31:57.000000 apollo-ai-0.0.48/apollo/apollo_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-10 20:31:57.000000 apollo-ai-0.0.48/apollo/apollo_ai.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-10 20:31:59.528148 apollo-ai-0.0.48/apollo/argus/
--rw-rw-rw-   0        0        0       65 2024-05-02 14:32:40.000000 apollo-ai-0.0.48/apollo/argus/__init__.py
--rw-rw-rw-   0        0        0    12485 2024-05-08 03:26:33.000000 apollo-ai-0.0.48/apollo/argus/argus.py
--rw-rw-rw-   0        0        0     6864 2024-05-08 03:20:05.000000 apollo-ai-0.0.48/apollo/argus/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 20:31:59.598050 apollo-ai-0.0.48/apollo/lyre/
--rw-rw-rw-   0        0        0      149 2024-05-06 03:28:49.000000 apollo-ai-0.0.48/apollo/lyre/__init__.py
--rw-rw-rw-   0        0        0     9151 2024-05-06 03:28:49.000000 apollo-ai-0.0.48/apollo/lyre/lyre.py
--rw-rw-rw-   0        0        0     3140 2024-05-06 03:28:49.000000 apollo-ai-0.0.48/apollo/lyre/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 20:31:59.648151 apollo-ai-0.0.48/apollo/pythia/
--rw-rw-rw-   0        0        0      201 2024-05-02 14:32:40.000000 apollo-ai-0.0.48/apollo/pythia/__init__.py
--rw-rw-rw-   0        0        0    10484 2024-05-10 20:30:38.000000 apollo-ai-0.0.48/apollo/pythia/pythia.py
--rw-rw-rw-   0        0        0     4339 2024-05-02 14:32:40.000000 apollo-ai-0.0.48/apollo/pythia/utils.py
--rw-rw-rw-   0        0        0       42 2024-05-10 20:31:59.653531 apollo-ai-0.0.48/setup.cfg
--rw-rw-rw-   0        0        0     1821 2024-05-10 20:31:51.000000 apollo-ai-0.0.48/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:12:37.223553 apollo-ai-0.0.49/
+-rw-rw-rw-   0        0        0    35823 2023-09-19 22:57:32.000000 apollo-ai-0.0.49/LICENSE
+-rw-rw-rw-   0        0        0     9511 2024-05-24 20:12:37.220552 apollo-ai-0.0.49/PKG-INFO
+-rw-rw-rw-   0        0        0     8994 2023-11-08 20:42:11.000000 apollo-ai-0.0.49/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 20:12:36.927300 apollo-ai-0.0.49/apollo/
+drwxrwxrwx   0        0        0        0 2024-05-24 20:12:36.992375 apollo-ai-0.0.49/apollo/apollo_ai.egg-info/
+-rw-rw-rw-   0        0        0     9511 2024-05-24 20:12:36.000000 apollo-ai-0.0.49/apollo/apollo_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-05-24 20:12:36.000000 apollo-ai-0.0.49/apollo/apollo_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 20:12:36.000000 apollo-ai-0.0.49/apollo/apollo_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      596 2024-05-24 20:12:36.000000 apollo-ai-0.0.49/apollo/apollo_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-24 20:12:36.000000 apollo-ai-0.0.49/apollo/apollo_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 20:12:37.010498 apollo-ai-0.0.49/apollo/argus/
+-rw-rw-rw-   0        0        0       65 2024-05-02 14:32:40.000000 apollo-ai-0.0.49/apollo/argus/__init__.py
+-rw-rw-rw-   0        0        0    12531 2024-05-16 01:28:22.000000 apollo-ai-0.0.49/apollo/argus/argus.py
+-rw-rw-rw-   0        0        0     6865 2024-05-14 22:18:09.000000 apollo-ai-0.0.49/apollo/argus/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:12:37.179206 apollo-ai-0.0.49/apollo/lyre/
+-rw-rw-rw-   0        0        0      149 2024-05-06 03:28:49.000000 apollo-ai-0.0.49/apollo/lyre/__init__.py
+-rw-rw-rw-   0        0        0     9359 2024-05-15 22:31:23.000000 apollo-ai-0.0.49/apollo/lyre/lyre.py
+-rw-rw-rw-   0        0        0     3140 2024-05-06 03:28:49.000000 apollo-ai-0.0.49/apollo/lyre/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:12:37.215442 apollo-ai-0.0.49/apollo/pythia/
+-rw-rw-rw-   0        0        0      201 2024-05-02 14:32:40.000000 apollo-ai-0.0.49/apollo/pythia/__init__.py
+-rw-rw-rw-   0        0        0     8305 2024-05-24 19:48:53.000000 apollo-ai-0.0.49/apollo/pythia/pythia.py
+-rw-rw-rw-   0        0        0     4339 2024-05-02 14:32:40.000000 apollo-ai-0.0.49/apollo/pythia/utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-24 20:12:37.223553 apollo-ai-0.0.49/setup.cfg
+-rw-rw-rw-   0        0        0     1821 2024-05-24 20:11:46.000000 apollo-ai-0.0.49/setup.py
```

### Comparing `apollo-ai-0.0.48/LICENSE` & `apollo-ai-0.0.49/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.48/PKG-INFO` & `apollo-ai-0.0.49/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-ai
-Version: 0.0.48
+Version: 0.0.49
 Summary: Framework to process 3 channels in one: Video, Audio & Text
 Home-page: https://github.com/VerbaNexAI/APOLLO.AI
 Author: VerbaNex, Riddle
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-ai-0.0.48/README.md` & `apollo-ai-0.0.49/README.md`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.48/apollo/apollo_ai.egg-info/PKG-INFO` & `apollo-ai-0.0.49/apollo/apollo_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-ai
-Version: 0.0.48
+Version: 0.0.49
 Summary: Framework to process 3 channels in one: Video, Audio & Text
 Home-page: https://github.com/VerbaNexAI/APOLLO.AI
 Author: VerbaNex, Riddle
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-ai-0.0.48/apollo/apollo_ai.egg-info/requires.txt` & `apollo-ai-0.0.49/apollo/apollo_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.48/apollo/argus/argus.py` & `apollo-ai-0.0.49/apollo/argus/argus.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,25 +14,28 @@
     plot_pose_cube,
     filter_video_data,
     plot_head_data_mov,
     plot_head_data_speed
 )
 from .utils import ensure_dir_created
 
+MILLIMETER=0.2645833333
+
 logging.basicConfig(format='APOLLO: (%(asctime)s): %(message)s', datefmt='%d/%m/%Y %I:%M:%S %p',
                     level=logging.DEBUG)
 
 
-def mouth_movement(filepath: str, focal_length_mm: int, output_dir='./output', plot=False,
+def mouth_movement(filepath: str, focal_length_mm: int, subject_distance_mm: int, output_dir='./output', plot=False,
                    normalize=False, lim: list[float, float] = None) -> str:
     """
     Generates the face data points for a given video, it currently accepts a small variety of part indices in the face
 
     :param filepath:
     :param focal_length_mm:
+    :param subject_distance_mm:
     :param output_dir:
     :param plot:
     :param normalize:
     :param lim:
     :return:
     """
     ensure_dir_created(output_dir)
@@ -103,18 +106,17 @@
 
                 source_bottom = results_facial_dots.multi_face_landmarks[0].landmark[index_bottom]
                 x_bottom = int(source_bottom.x * fw)
                 y_bottom = int(source_bottom.y * fh)
 
                 # Applying chebyshev distance
                 distance_px = int(distance.chebyshev([x_top, y_top], [x_bottom, y_bottom]))
-                distance_mm = int(
-                    (distance_px * focal_length_mm) / (focal_length_mm * 2 * math.tan(math.radians(0.5))))
+                distance_mm = (distance_px * focal_length_mm) / (focal_length_mm * 2 * math.tan(math.radians(0.5))) * subject_distance_mm
                 timestamp = video_source.get(cv2.CAP_PROP_POS_MSEC)
-                distances_data.append([(distance_mm / 100), timestamp / 1000])
+                distances_data.append([distance_px * MILLIMETER, timestamp / 1000])
 
                 cv2.circle(frame, (x, y), 2, (255, 255, 255), -1)
 
                 max_distance = max(max_distance, distance_mm / 100)
                 min_distance = min(min_distance, distance_mm / 100)
 
         out.write(frame)  # Write the frame to the output video file
@@ -329,9 +331,9 @@
             "x_head_movement": time_in_seconds,
             "y_pitch_values": pitch_vals,
             "y_yaw_values": yaw_vals,
             "y_roll_values": roll_vals,
             "threshold_speed": float(threshold_mm),
             "average_speed": float(mean_speed)}
 
-    return json.dumps(str(data))  # Does not know how it will work later
+    return json.dumps(str(data))
```

### Comparing `apollo-ai-0.0.48/apollo/argus/utils.py` & `apollo-ai-0.0.49/apollo/argus/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         # Calculate the normalization based on min and max values
         if normalize:
             max_value = df['Distance'].max()
             min_value = df['Distance'].min()
             df['Distance'] = (df['Distance'] - min_value) / (max_value - min_value)
 
-        df['Distance'] = signal.savgol_filter(df["Distance"], min(len(df["Distance"]), 51), 2)
+        df['Distance'] = signal.savgol_filter(df["Distance"], min(len(df["Distance"]), 260), 3)
 
         return df
     except Exception as e:
         raise Exception("Error normalizing the data: {0}".format(e))
 
 
 def plot_pose_cube(img, yaw, pitch, roll, tdx=None, tdy=None, size=150.):
```

### Comparing `apollo-ai-0.0.48/apollo/lyre/lyre.py` & `apollo-ai-0.0.49/apollo/lyre/lyre.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,24 +131,23 @@
     finally:
         if audio_clip is not None:
             audio_clip.close()  # Should not give an error
         if 'video_clip' in locals():
             video_clip.close()
 
 
-def voice_intensity(filepath: str, lim: list[float, float] = None, plot=False, amplitude_env=False, frame_size=1024,
+def voice_intensity(filepath: str, lim: list[float, float] = None, plot=False, frame_size=1024,
                     hop_length=512, output_dir='./output') -> str:
     """
     Generate audio data processed with librosa to create visualizations or audio processing
     if the lim is specified then the audio is cropped to that timestamp
 
     :param filepath: path to the audio file
     :param lim: list of two floats specifying start and end time for cropping (optional)
     :param plot: boolean flag to generate a plot (optional)
-    :param amplitude_env: boolean flag to calculate the amplitude envelope (optional)
     :param frame_size: size of the STFT window (default: 1024)
     :param hop_length: hop length between consecutive STFT windows (default: 512)
     :param output_dir: directory to save the plot (default: ./output)
     :return: dictionary containing processed audio data
     """
     ensure_dir_created(output_dir)
 
@@ -165,32 +164,38 @@
         # Calculate STFT and amplitude envelope
         stft = np.abs(librosa.stft(y, n_fft=frame_size, hop_length=hop_length))
         amplitude_envelope = np.array([max(y[i:i+frame_size]) for i in range(0, y.size, hop_length)])
 
         # Convert amplitude envelope to dB
         amplitude_envelope_db = librosa.amplitude_to_db(amplitude_envelope)
 
-        max_amplitude = np.max(np.abs(y))
+        std_dev_envelope = np.std(amplitude_envelope_db)
+
+        max_amplitude = np.max(amplitude_envelope_db)
+        min_amplitude = np.min(amplitude_envelope_db)
+        average_amplitude = np.mean(amplitude_envelope_db)
 
         data = {
             "duration": duration,
             "samplerate": sr,
             "max_amplitude": max_amplitude.tolist(),
+            "min_amplitude": min_amplitude.tolist(),
+            "average_amplitude": str(average_amplitude),
             "stft": stft.tolist(),
             "amplitude_envelope_db": amplitude_envelope_db.tolist(),
+            "std_dev_envelope": str(std_dev_envelope),
         }
 
         if plot:
             try:
                 frames = range(0, len(amplitude_envelope))
                 t = librosa.frames_to_time(frames, sr=sr, hop_length=hop_length)
                 plt.figure(figsize=(25, 10))
                 librosa.display.waveshow(y, sr=sr)
-                if amplitude_env:
-                    plt.plot(t, amplitude_envelope, color="r", label="Amp_env")
+                plt.plot(t, amplitude_envelope, color="r", label="Amp_env")
                 plt.xlabel('Time (seconds)')
                 plt.ylabel('Audio Time Series')
                 plt.title('Full Signal')
                 plt.legend()
                 plt.savefig(f'{file_direction}_full_signal.png')
             except Exception as e:
                 raise Exception("Error saving plot: {0}".format(e))
```

### Comparing `apollo-ai-0.0.48/apollo/lyre/utils.py` & `apollo-ai-0.0.49/apollo/lyre/utils.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.48/apollo/pythia/pythia.py` & `apollo-ai-0.0.49/apollo/pythia/pythia.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,41 @@
-import spacy
-from epitran import Epitran
-from pyphen import Pyphen
-import re
-import jiwer
+import concurrent.futures
 import difflib
-import logging
-import time
 import json
-from faster_whisper import WhisperModel
+import logging
 import multiprocessing
-import concurrent.futures
 import os
+import re
+import time
+
+import jiwer
+import spacy
+from epitran import Epitran
+from faster_whisper import WhisperModel
+from pyphen import Pyphen
 
 from .utils import (
     transcribe_file,
     split_audio_into_chunks
 )
 
-
 logging.basicConfig(format='APOLLO: (%(asctime)s): %(message)s', datefmt='%d/%m/%Y %I:%M:%S %p',
                     level=logging.DEBUG)
 
 
 def clean_text(text: str) -> str:
-    """
-    Cleans the text from all punctuation, special characters, colons and semicolons
-    it only leaves tildes and double points on top of words without changing the case
-
-    :param text:
-    :return:
-    """
     try:
         cleaned_text = re.sub(r'[^A-Za-z0-9áéíóúÁÉÍÓÚñÑüÜ]+', ' ', text)
-
-        data = {
-            "data": cleaned_text,
-        }
+        data = {"data": cleaned_text}
         return json.dumps(data)
     except Exception as e:
-        raise Exception("Error getting clean text: {0}".format(e))
+        return json.dumps({"error": f"Error getting clean text: {str(e)}"})
 
 
 def sentences(text: str) -> str:
-    """
-    Extracts all the sentences in a text string conserving inner punctuation and case
-
-    :param text:
-    :return:
-    """
     try:
         sentence_delimiters = r'[.!?]|(?:\.{3})|…|¡|¿|;|"'
         spanish_prefixes = ['Sr.', 'Sra.', 'Dr.', 'Lic.', 'Ing.']
 
         for prefix in spanish_prefixes:
             text = text.replace(prefix, prefix.replace('.', '###'))
 
@@ -59,209 +43,124 @@
 
         for prefix in spanish_prefixes:
             sentences_ = [sentence.replace(prefix.replace('.', '###'), prefix) for sentence in sentences_]
 
         processed_sentences = []
         for sentence in sentences_:
             sentence = sentence.strip()
-            if sentence and not sentence.startswith("–") and not sentence.startswith(
-                    "-"):
-                sentence = sentence.strip(":")
-                sentence = sentence.strip(", ")
+            if sentence and not sentence.startswith("–") and not sentence.startswith("-"):
+                sentence = sentence.strip(":").strip(", ")
                 processed_sentences.append(sentence)
 
-        data = {
-            "data": processed_sentences,
-        }
-
+        data = {"data": processed_sentences}
         return json.dumps(data)
-
     except Exception as e:
-        raise Exception('Error getting sentences: {0}'.format(e))
+        return json.dumps({"error": f"Error getting sentences: {str(e)}"})
 
 
 def word_checker(original_text: str, new_text: str) -> str:
-    """
-    Compares two transcriptions and returns the correct words, incorrect
-    words and omitted words
-
-    word error rate (WER)
-    match error rate (MER)
-    word information lost (WIL)
-    word information preserved (WIP)
-
-    :param original_text:
-    :param new_text:
-    :return:
-    """
-    correct_words = []
-    omitted_words = []
-
     try:
-        original_words = words(original_text, True)
-        new_words = words(new_text, True)
+        original_words = dict(json.loads(words(original_text, True)))["data"]
+        new_words = dict(json.loads(words(new_text, True)))["data"]
 
-        output = jiwer.process_words(clean_text(original_text), clean_text(new_text))
+        output = jiwer.process_words(dict(json.loads(clean_text(original_text)))["data"],
+                                     dict(json.loads(clean_text(new_text)))["data"])
 
         wer = output.wer
         mer = output.mer
         wip = output.wip
         wil = output.wil
 
-        for original_word in original_words:
-            if original_word in new_words:
-                new_words.remove(original_word)
-                correct_words.append(original_word)
-            else:
-                omitted_words.append(original_word)
-
-        incorrect_words = new_words
-
-        data = {"correct_words": correct_words, "omitted_words": omitted_words, "incorrect_words": incorrect_words,
-                "mer": mer, "wil": wil, "wip": wip, "wer": wer}
+        correct_words = [word for word in original_words if word in new_words]
+        omitted_words = [word for word in original_words if word not in new_words]
+        incorrect_words = [word for word in new_words if word not in original_words]
 
+        data = {
+            "correct_words": correct_words,
+            "omitted_words": omitted_words,
+            "incorrect_words": incorrect_words,
+            "mer": mer,
+            "wil": wil,
+            "wip": wip,
+            "wer": wer
+        }
         return json.dumps(data)
     except Exception as e:
-        raise Exception("Error comparing words: {0}".format(e))
-
+        return json.dumps({"error": f"Error comparing words: {str(e)}"})
 
-def word_alignment(original_text: str, new_text: str) -> dict:
-    """
-    Compares two transcriptions and returns word by word the difference
-    marked with "*" the length of the word and the residual words in order
-
-    Residuals are marked with "+"
-    Extras are marked with "*"
-
-    :param original_text:
-    :param new_text:
-    :return:
-    """
-    original_words = words(original_text)
-    new_words = words(new_text)
-    matcher = difflib.SequenceMatcher(None, original_words, new_words)
-    alignment = []
-    residual_words = []
-    extra_words = []
 
+def word_alignment(original_text: str, new_text: str) -> str:
     try:
+        original_words = dict(json.loads(words(original_text)))["data"]
+        new_words = dict(json.loads(words(new_text)))["data"]
+        matcher = difflib.SequenceMatcher(None, original_words, new_words)
+        alignment = []
+        residual_words = []
+        extra_words = []
+
         for opcode, a0, a1, b0, b1 in matcher.get_opcodes():
             if opcode == 'equal':
-                # If the words are the same, add them to the list
                 alignment.extend(original_words[a0:a1])
-
             elif opcode == 'delete':
-                # If the words are different, add asterisks to the list
                 alignment.extend('+' * len(word) for word in original_words[a0:a1])
                 residual_words.extend(original_words[a0:a1])
-
-            elif opcode == 'insert' or opcode == 'replace':
-                # Original transcription does not include this words
+            elif opcode in ('insert', 'replace'):
                 alignment.extend('*' * len(word) for word in new_words[b0:b1])
                 extra_words.extend(new_words[b0:b1])
 
-        data = {"alignment": alignment, "residual_words": residual_words, "extra_words": extra_words}
+        data = {
+            "alignment": alignment,
+            "residual_words": residual_words,
+            "extra_words": extra_words
+        }
         return json.dumps(data)
     except Exception as e:
-        raise Exception("Error on word alignment: {0}".format(e))
+        return json.dumps({"error": f"Error on word alignment: {str(e)}"})
 
 
 def phonetic_transcription(text: str, lang='spa-Latn') -> str:
-    """
-    Cleans text and makes the phonetic following IPA
-
-    :param text:
-    :param lang:
-    :return:
-    """
     epi = Epitran(lang)
     try:
-        data = {
-            "data": epi.transliterate(clean_text(text))
-        }
+        transcription = epi.transliterate(dict(json.loads(clean_text(text)))["data"])
+        data = {"data": transcription}
         return json.dumps(data)
     except Exception as e:
-        raise Exception("Error getting the phonetic transcription: {0}".format(e))
+        return json.dumps({"error": f"Error getting the phonetic transcription: {str(e)}"})
 
 
 def syllables(text: str, lang='es') -> str:
-    """
-    Extracts all the syllables from a text string
-
-    :param text:
-    :param lang:
-    :return:
-    """
     nlp = spacy.load('es_core_news_lg' if lang == 'es' else 'en_core_web_lg')
     py_instance = Pyphen(lang=lang)
     try:
-        text = clean_text(text)
+        text = dict(json.loads(clean_text(text)))["data"]
         doc = nlp(text)
         list_words = [token.text for token in doc]
-        list_syllables = []
-
-        for word in list_words:
-            syllables_ = py_instance.inserted(word).split('-')
-            list_syllables.extend(syllables_)
-
-        data = {
-            "data": list_syllables
-        }
+        list_syllables = [syllable for word in list_words for syllable in py_instance.inserted(word).split('-')]
 
+        data = {"data": list_syllables}
         return json.dumps(data)
     except Exception as e:
-        raise Exception('Error getting syllables: {0}'.format(e))
+        return json.dumps({"error": f"Error getting syllables: {str(e)}"})
 
 
 def words(text: str, lower=False, lang='es') -> str:
-    """
-    Extracts all the words from a corpus in lower case
-
-    :param text:
-    :param lower:
-    :param lang:
-    :return:
-    """
     nlp = spacy.load('es_core_news_lg' if lang == 'es' else 'en_core_web_lg')
     try:
-        text = clean_text(text)
-
-        if lower:
-            doc = nlp(text.lower())
-        else:
-            doc = nlp(text)
-
+        text = dict(json.loads(clean_text(text)))["data"]
+        doc = nlp(text.lower() if lower else text)
         list_words = [token.text for token in doc]
 
-        data = {
-            "data": list_words
-        }
-
+        data = {"data": list_words}
         return json.dumps(data)
     except Exception as e:
-        raise Exception("Error on getting words: {0}".format(e))
+        return json.dumps({"error": f"Error on getting words: {str(e)}"})
 
 
 def transcriber_parallel(file: str, model_name='small', device='cpu', max_processes=0, compute_type='float16',
-                lang='es', silence_threshold: str = "-20dB", silence_duration: float = 2.0) -> str:
-    """
-    Generates a transcription result from the given file
-    it simplifies the audio loading and comes out of the box
-    with all the timestamps of each word
-
-    :param file: The name of the file
-    :param model_name:
-    :param device:
-    :param max_processes:
-    :param compute_type:
-    :param lang:
-    :param silence_threshold:
-    :param silence_duration:
-    :return:
-    """
+                         lang='es', silence_threshold: str = "-20dB", silence_duration: float = 2.0) -> str:
     if max_processes > multiprocessing.cpu_count() or max_processes == 0:
         max_processes = multiprocessing.cpu_count()
 
     temp_files_array = split_audio_into_chunks(file, max_processes, silence_threshold, silence_duration)
     model = WhisperModel(model_name, device=device, compute_type=compute_type, cpu_threads=4)
     segments_output = []
     futures = []
@@ -274,62 +173,45 @@
             for file_path in temp_files_array:
                 future = executor.submit(transcribe_file, file_path, model, lang)
                 futures.append(future)
 
         transcription = ""
         for future in futures:
             segments = future.result()
-
             for segment in segments:
                 segments_output.append(
-                    {"start": segment.start, "end": segment.end, "text": segment.text, "words": segment.words})
-
+                    {"start": segment.start, "end": segment.end, "text": segment.text, "words": segment.words}
+                )
                 transcription += segment.text + " "
 
         for temp_file in temp_files_array:
             os.remove(temp_file)
 
         data = {"transcription": transcription, "segments": segments_output, "time_taken": time.time() - start_time}
-
         return json.dumps(data)
     except Exception as e:
-        raise Exception("Error transcribing: {0}".format(e))
+        return json.dumps({"error": f"Error transcribing: {str(e)}"})
 
 
-def transcriber(file: str, model_name='large-v2', device='cuda', compute_type='float16', beam_size=5,
-                lang='es') -> str:
-    """
-    Generates a transcription result from the given file
-    it simplifies the audio loading and comes out of the box
-    with all the timestamps of each word
-
-    :param file: The name of the file
-    :param model_name:
-    :param device:
-    :param compute_type:
-    :param beam_size:
-    :param lang:
-    :return:
-    """
-
+def transcriber(file: str, model_name='large-v2', device='cuda', compute_type='float16', beam_size=5, lang='es') -> str:
     model = WhisperModel(model_name, device=device, compute_type=compute_type)
     segments_output = []
 
     try:
         logging.info("Starting transcription")
         start_time = time.time()
 
         segments, info = model.transcribe(file, beam_size=beam_size, language=lang, word_timestamps=True)
 
         transcription = ""
-
         for segment in segments:
             segments_output.append(
                 {"start": segment.start, "end": segment.end, "text": segment.text, "words": segment.words,
-                 "tokens": segment.tokens})
-
+                 "tokens": segment.tokens}
+            )
             transcription += segment.text + " "
 
-        data = {"transcription": transcription, "segments": segments_output, "info": info, "time_taken": time.time() - start_time}
+        data = {"transcription": transcription, "segments": segments_output, "info": info,
+                "time_taken": time.time() - start_time}
         return json.dumps(data)
     except Exception as e:
-        raise Exception("Error transcribing: {0}".format(e))
+        return json.dumps({"error": f"Error transcribing: {str(e)}"})
```

### Comparing `apollo-ai-0.0.48/apollo/pythia/utils.py` & `apollo-ai-0.0.49/apollo/pythia/utils.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.48/setup.py` & `apollo-ai-0.0.49/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="apollo-ai",
-    version="0.0.48",
+    version="0.0.49",
     description="Framework to process 3 channels in one: Video, Audio & Text",
     package_dir={"": "apollo"},
     packages=find_packages(where="apollo"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/VerbaNexAI/APOLLO.AI",
     author="VerbaNex, Riddle",
```

