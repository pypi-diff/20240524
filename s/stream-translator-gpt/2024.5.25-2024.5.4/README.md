# Comparing `tmp/stream_translator_gpt-2024.5.25.tar.gz` & `tmp/stream_translator_gpt-2024.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stream_translator_gpt-2024.5.25.tar", last modified: Fri May 24 19:58:12 2024, max compression
+gzip compressed data, was "stream_translator_gpt-2024.5.4.tar", last modified: Fri May  3 19:09:29 2024, max compression
```

## Comparing `stream_translator_gpt-2024.5.25.tar` & `stream_translator_gpt-2024.5.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 19:58:12.547318 stream_translator_gpt-2024.5.25/
--rw-rw-rw-   0        0        0     1089 2023-03-12 08:56:05.000000 stream_translator_gpt-2024.5.25/LICENSE
--rw-rw-rw-   0        0        0     6213 2024-05-24 19:58:12.547318 stream_translator_gpt-2024.5.25/PKG-INFO
--rw-rw-rw-   0        0        0    15693 2024-05-24 19:50:01.000000 stream_translator_gpt-2024.5.25/README.md
--rw-rw-rw-   0        0        0     4733 2024-05-24 19:50:08.000000 stream_translator_gpt-2024.5.25/README_PyPI.md
--rw-rw-rw-   0        0        0     1745 2024-05-24 19:57:40.000000 stream_translator_gpt-2024.5.25/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-24 19:58:12.548317 stream_translator_gpt-2024.5.25/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-24 19:58:12.525148 stream_translator_gpt-2024.5.25/stream_translator_gpt/
--rw-rw-rw-   0        0        0        0 2024-03-03 09:46:32.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt/__init__.py
--rw-rw-rw-   0        0        0       68 2024-03-03 10:18:23.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt/__main__.py
--rw-rw-rw-   0        0        0     5572 2024-03-26 11:43:09.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt/audio_getter.py
--rw-rw-rw-   0        0        0     4102 2024-04-25 09:10:57.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt/audio_slicer.py
--rw-rw-rw-   0        0        0     3821 2024-03-26 11:43:09.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt/audio_transcriber.py
--rw-rw-rw-   0        0        0      968 2024-04-25 17:12:13.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt/common.py
--rw-rw-rw-   0        0        0     1384 2024-03-14 15:15:25.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt/filters.py
--rw-rw-rw-   0        0        0     8980 2024-05-24 18:51:31.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt/llm_translator.py
--rw-rw-rw-   0        0        0     2731 2024-04-16 06:16:00.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt/result_exporter.py
--rw-rw-rw-   0        0        0  1439299 2024-03-05 16:52:38.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt/silero_vad.jit
--rw-rw-rw-   0        0        0    17329 2024-05-15 09:10:14.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt/translator.py
-drwxrwxrwx   0        0        0        0 2024-05-24 19:58:12.547318 stream_translator_gpt-2024.5.25/stream_translator_gpt.egg-info/
--rw-rw-rw-   0        0        0     6213 2024-05-24 19:58:12.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      725 2024-05-24 19:58:12.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 19:58:12.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-05-24 19:58:12.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      156 2024-05-24 19:58:12.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-24 19:58:12.000000 stream_translator_gpt-2024.5.25/stream_translator_gpt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 19:09:29.063574 stream_translator_gpt-2024.5.4/
+-rw-rw-rw-   0        0        0     1089 2023-03-12 08:56:05.000000 stream_translator_gpt-2024.5.4/LICENSE
+-rw-rw-rw-   0        0        0     6292 2024-05-03 19:09:29.062577 stream_translator_gpt-2024.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0    15478 2024-05-03 19:05:57.000000 stream_translator_gpt-2024.5.4/README.md
+-rw-rw-rw-   0        0        0     4813 2024-03-26 11:06:30.000000 stream_translator_gpt-2024.5.4/README_PyPI.md
+-rw-rw-rw-   0        0        0     1744 2024-05-03 19:08:52.000000 stream_translator_gpt-2024.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 19:09:29.063574 stream_translator_gpt-2024.5.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-03 19:09:29.051614 stream_translator_gpt-2024.5.4/stream_translator_gpt/
+-rw-rw-rw-   0        0        0        0 2024-03-03 09:46:32.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/__init__.py
+-rw-rw-rw-   0        0        0       68 2024-03-03 10:18:23.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/__main__.py
+-rw-rw-rw-   0        0        0     5572 2024-03-26 11:43:09.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/audio_getter.py
+-rw-rw-rw-   0        0        0     4102 2024-04-25 09:10:57.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/audio_slicer.py
+-rw-rw-rw-   0        0        0     3821 2024-03-26 11:43:09.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/audio_transcriber.py
+-rw-rw-rw-   0        0        0      968 2024-04-25 17:12:13.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/common.py
+-rw-rw-rw-   0        0        0     1384 2024-03-14 15:15:25.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/filters.py
+-rw-rw-rw-   0        0        0     8300 2024-04-25 09:26:14.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/llm_translator.py
+-rw-rw-rw-   0        0        0     2731 2024-04-16 06:16:00.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/result_exporter.py
+-rw-rw-rw-   0        0        0  1439299 2024-03-05 16:52:38.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/silero_vad.jit
+-rw-rw-rw-   0        0        0    17068 2024-05-03 19:08:00.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/translator.py
+drwxrwxrwx   0        0        0        0 2024-05-03 19:09:29.062577 stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/
+-rw-rw-rw-   0        0        0     6292 2024-05-03 19:09:29.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      725 2024-05-03 19:09:29.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 19:09:29.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-03 19:09:29.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      156 2024-05-03 19:09:29.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-03 19:09:29.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/top_level.txt
```

### Comparing `stream_translator_gpt-2024.5.25/LICENSE` & `stream_translator_gpt-2024.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.5.25/PKG-INFO` & `stream_translator_gpt-2024.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stream-translator-gpt
-Version: 2024.5.25
+Version: 2024.5.4
 Summary: Command line tool to transcribe & translate audio from livestreams in real time
 Author-email: ion <ionicbond3@gmail.com>
 Project-URL: Homepage, https://github.com/ionic-bond/stream-translator-gpt
 Project-URL: Issues, https://github.com/ionic-bond/stream-translator-gpt/issues
 Keywords: translator,translation,translate,transcribe,yt-dlp,vad,whisper,faster-whisper,whisper-api,gpt,gemini
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,15 +23,15 @@
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: yt-dlp
 Requires-Dist: ffmpeg-python<0.3,>=0.2.0
 Requires-Dist: sounddevice<1.0
 Requires-Dist: openai-whisper<=20231117
-Requires-Dist: faster-whisper<2.0.0,>=1.0.0
+Requires-Dist: faster-whisper<1.0.0,>=0.8.0
 Requires-Dist: openai<2.0,>=1.0
 Requires-Dist: google-generativeai<1.0
 
 # stream-translator-gpt
 
 Command line utility to transcribe or translate audio from livestreams in real time. Uses [yt-dlp](https://github.com/yt-dlp/yt-dlp) to 
 get livestream URLs from various services and [Whisper](https://github.com/openai/whisper) / [Faster-Whisper](https://github.com/SYSTRAN/faster-whisper) for transcription.
@@ -42,31 +42,31 @@
 Try it on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ionic-bond/stream-translator-gpt/blob/main/stream_translator.ipynb)
 
 ## Prerequisites
 
 **Linux or Windows:**
 
 1. Python >= 3.8 (Recommend >= 3.10)
-2. [**Install CUDA on your system.**](https://developer.nvidia.com/cuda-downloads).
-3. [**Install cuDNN to your CUDA dir**](https://developer.nvidia.com/cudnn-downloads) if you want to use **Faseter-Whisper**.
+2. [**Install CUDA 11 on your system.**](https://developer.nvidia.com/cuda-11-8-0-download-archive) (Faster-Whisper is not compatible with CUDA 12 for now).
+3. [**Install cuDNN to your CUDA dir**](https://developer.nvidia.com/cuda-downloads) if you want to use **Faseter-Whisper**.
 4. [**Install PyTorch (with CUDA) to your Python.**](https://pytorch.org/get-started/locally/)
-5. [**Create a Google API key**](https://aistudio.google.com/app/apikey) if you want to use **Gemini API** for translation. (Free 15 requests / minute)
+5. [**Create a Google API key**](https://aistudio.google.com/app/apikey) if you want to use **Gemini API** for translation. (Recommend, Free 60 requests / minute)
 6. [**Create a OpenAI API key**](https://platform.openai.com/api-keys) if you want to use **Whisper API** for transcription or **GPT API** for translation.
 
 **If you are in Windows, you also need to:**
 
 1. [**Install and add ffmpeg to your PATH.**](https://www.thewindowsclub.com/how-to-install-ffmpeg-on-windows-10#:~:text=Click%20New%20and%20type%20the,Click%20OK%20to%20apply%20changes.)
 2. Install [**yt-dlp**](https://github.com/yt-dlp/yt-dlp) and add it to your PATH.
 
 ## Installation
 
 **Install release version from PyPI (Recommend):**
 
 ```
-pip install stream-translator-gpt -U
+pip install stream-translator-gpt
 stream-translator-gpt
 ```
 
 or
 
 **Clone master version code from Github:**
```

### Comparing `stream_translator_gpt-2024.5.25/README.md` & `stream_translator_gpt-2024.5.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -56,31 +56,31 @@
 Try it on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ionic-bond/stream-translator-gpt/blob/main/stream_translator.ipynb)
 
 ## Prerequisites
 
 **Linux or Windows:**
 
 1. Python >= 3.8 (Recommend >= 3.10)
-2. [**Install CUDA on your system.**](https://developer.nvidia.com/cuda-downloads).
-3. [**Install cuDNN to your CUDA dir**](https://developer.nvidia.com/cudnn-downloads) if you want to use **Faseter-Whisper**.
+2. [**Install CUDA 11 on your system.**](https://developer.nvidia.com/cuda-11-8-0-download-archive) (Faster-Whisper is not compatible with CUDA 12 for now).
+3. [**Install cuDNN to your CUDA dir**](https://developer.nvidia.com/cuda-downloads) if you want to use **Faseter-Whisper**.
 4. [**Install PyTorch (with CUDA) to your Python.**](https://pytorch.org/get-started/locally/)
-5. [**Create a Google API key**](https://aistudio.google.com/app/apikey) if you want to use **Gemini API** for translation. (Free 15 requests / minute)
+5. [**Create a Google API key**](https://aistudio.google.com/app/apikey) if you want to use **Gemini API** for translation. (Recommend, Free 60 requests / minute)
 6. [**Create a OpenAI API key**](https://platform.openai.com/api-keys) if you want to use **Whisper API** for transcription or **GPT API** for translation.
 
 **If you are in Windows, you also need to:**
 
 1. [**Install and add ffmpeg to your PATH.**](https://www.thewindowsclub.com/how-to-install-ffmpeg-on-windows-10#:~:text=Click%20New%20and%20type%20the,Click%20OK%20to%20apply%20changes.)
 2. Install [**yt-dlp**](https://github.com/yt-dlp/yt-dlp) and add it to your PATH.
 
 ## Installation
 
 **Install release version from PyPI (Recommend):**
 
 ```
-pip install stream-translator-gpt -U
+pip install stream-translator-gpt
 stream-translator-gpt
 ```
 
 or
 
 **Clone master version code from Github:**
 
@@ -140,55 +140,54 @@
 
 - Saving result to a .srt subtitle file:
 
     ```stream-translator-gpt {URL} --model large --language ja --gpt_translation_prompt "Translate from Japanese to Chinese" --google_api_key {your_google_key} --hide_transcribe_result --output_timestamps --output_file_path ./result.srt```
 
 ## All options
 
-| Option                             | Default Value  | Description                                                                                                                                                                                              |
-| :--------------------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| Option                             | Default Value | Description                                                                                                                                                                                              |
+| :--------------------------------- | :------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | **Input Options**                  |
-| `URL`                              |                | The URL of the stream. If a local file path is filled in, it will be used as input. If fill in "device", the input will be obtained from your PC device.                                                 |
-| `--format`                         | wa*            | Stream format code, this parameter will be passed directly to yt-dlp.                                                                                                                                    |
-| `--cookies`                        |                | Used to open member-only stream, this parameter will be passed directly to yt-dlp.                                                                                                                       |
-| `--device_index`                   |                | The index of the device that needs to be recorded. If not set, the system default recording device will be used.                                                                                         |
+| `URL`                              |               | The URL of the stream. If a local file path is filled in, it will be used as input. If fill in "device", the input will be obtained from your PC device.                                                 |
+| `--format`                         | wa*           | Stream format code, this parameter will be passed directly to yt-dlp.                                                                                                                                    |
+| `--cookies`                        |               | Used to open member-only stream, this parameter will be passed directly to yt-dlp.                                                                                                                       |
+| `--device_index`                   |               | The index of the device that needs to be recorded. If not set, the system default recording device will be used.                                                                                         |
 | **Audio Slicing Options**          |
-| `--frame_duration`                 | 0.05           | The unit that processes live streaming data in seconds, should be >= 0.03                                                                                                                                |
-| `--continuous_no_speech_threshold` | 0.5            | Slice if there is no speech for a continuous period in second.                                                                                                                                           |
-| `--min_audio_length`               | 3.0            | Minimum slice audio length in seconds.                                                                                                                                                                   |
-| `--max_audio_length`               | 30.0           | Maximum slice audio length in seconds.                                                                                                                                                                   |
-| `--prefix_retention_length`        | 0.5            | The length of the retention prefix audio during slicing.                                                                                                                                                 |
-| `--vad_threshold`                  | 0.35           | The threshold of Voice activity detection. if the speech probability of a frame is higher than this value, then this frame is speech.                                                                    |
+| `--frame_duration`                 | 0.05          | The unit that processes live streaming data in seconds, should be >= 0.03                                                                                                                                |
+| `--continuous_no_speech_threshold` | 0.5           | Slice if there is no speech for a continuous period in second.                                                                                                                                           |
+| `--min_audio_length`               | 3.0           | Minimum slice audio length in seconds.                                                                                                                                                                   |
+| `--max_audio_length`               | 30.0          | Maximum slice audio length in seconds.                                                                                                                                                                   |
+| `--prefix_retention_length`        | 0.5           | The length of the retention prefix audio during slicing.                                                                                                                                                 |
+| `--vad_threshold`                  | 0.35          | The threshold of Voice activity detection. if the speech probability of a frame is higher than this value, then this frame is speech.                                                                    |
 | **Transcription Options**          |
-| `--model`                          | small          | Select model size. See [here](https://github.com/openai/whisper#available-models-and-languages) for available models.                                                                                    |
-| `--language`                       | auto           | Language spoken in the stream. See [here](https://github.com/openai/whisper#available-models-and-languages) for available languages.                                                                     |
-| `--beam_size`                      | 5              | Number of beams in beam search. Set to 0 to use greedy algorithm instead (faster but less accurate).                                                                                                     |
-| `--best_of`                        | 5              | Number of candidates when sampling with non-zero temperature.                                                                                                                                            |
-| `--use_faster_whisper`             |                | Set this flag to use Faster Whisper implementation instead of the original OpenAI implementation                                                                                                         |
-| `--use_whisper_api`                |                | Set this flag to use OpenAI Whisper API instead of the original local Whipser.                                                                                                                           |
-| `--whisper_filters`                | emoji_filter   | Filters apply to whisper results, separated by ",".                                                                                                                                                      |
+| `--model`                          | small         | Select model size. See [here](https://github.com/openai/whisper#available-models-and-languages) for available models.                                                                                    |
+| `--language`                       | auto          | Language spoken in the stream. See [here](https://github.com/openai/whisper#available-models-and-languages) for available languages.                                                                     |
+| `--beam_size`                      | 5             | Number of beams in beam search. Set to 0 to use greedy algorithm instead (faster but less accurate).                                                                                                     |
+| `--best_of`                        | 5             | Number of candidates when sampling with non-zero temperature.                                                                                                                                            |
+| `--use_faster_whisper`             |               | Set this flag to use Faster Whisper implementation instead of the original OpenAI implementation                                                                                                         |
+| `--use_whisper_api`                |               | Set this flag to use OpenAI Whisper API instead of the original local Whipser.                                                                                                                           |
+| `--whisper_filters`                | emoji_filter  | Filters apply to whisper results, separated by ",".                                                                                                                                                      |
 | **Translation Options**            |
-| `--openai_api_key`                 |                | OpenAI API key if using GPT translation / Whisper API.                                                                                                                                                   |
-| `--google_api_key`                 |                | Google API key if using Gemini translation.                                                                                                                                                              |
-| `--gpt_model`                      | gpt-3.5-turbo  | OpenAI's GPT model name, gpt-3.5-turbo / gpt-4 / gpt-4o.                                                                                                                                                 |
-| `--gemini_model`                   | gemini-1.0-pro | Google's Gemini model name, gemini-1.0-pro / gemini-1.5-flash-latest / gemini-1.5-pro-latest                                                                                                             |
-| `--gpt_translation_prompt`         |                | If set, will translate the result text to target language via GPT / Gemini API (According to which API key is filled in). Example: "Translate from Japanese to Chinese"                                  |
-| `--gpt_translation_history_size`   | 0              | The number of previous messages sent when calling the GPT / Gemini API. If the history size is 0, the translation will be run parallelly. If the history size > 0, the translation will be run serially. |
-| `--gpt_translation_timeout`        | 10             | If the GPT / Gemini translation exceeds this number of seconds, the translation will be discarded.                                                                                                       |
-| `--gpt_base_url`                   |                | Customize the API endpoint of GPT.                                                                                                                                                                       |
-| `--retry_if_translation_fails`     |                | Retry when translation times out/fails. Used to generate subtitles offline.                                                                                                                              |
+| `--openai_api_key`                 |               | OpenAI API key if using GPT translation / Whisper API.                                                                                                                                                   |
+| `--google_api_key`                 |               | Google API key if using Gemini translation.                                                                                                                                                              |
+| `--gpt_model`                      | gpt-3.5-turbo | GPT model name, gpt-3.5-turbo or gpt-4. (If using Gemini, not need to change this)                                                                                                                       |
+| `--gpt_translation_prompt`         |               | If set, will translate the result text to target language via GPT / Gemini API (According to which API key is filled in). Example: "Translate from Japanese to Chinese"                                  |
+| `--gpt_translation_history_size`   | 0             | The number of previous messages sent when calling the GPT / Gemini API. If the history size is 0, the translation will be run parallelly. If the history size > 0, the translation will be run serially. |
+| `--gpt_translation_timeout`        | 10            | If the GPT / Gemini translation exceeds this number of seconds, the translation will be discarded.                                                                                                       |
+| `--gpt_base_url`                   |               | Customize the API endpoint of GPT.                                                                                                                                                                       |
+| `--retry_if_translation_fails`     |               | Retry when translation times out/fails. Used to generate subtitles offline.                                                                                                                              |
 | **Output Options**                 |
-| `--output_timestamps`              |                | Output the timestamp of the text when outputting the text.                                                                                                                                               |
-| `--hide_transcribe_result`         |                | Hide the result of Whisper transcribe.                                                                                                                                                                   |
-| `--output_file_path`               |                | If set, will save the result text to this path.                                                                                                                                                          |
-| `--cqhttp_url`                     |                | If set, will send the result text to the cqhttp server.                                                                                                                                                  |
-| `--cqhttp_token`                   |                | Token of cqhttp, if it is not set on the server side, it does not need to fill in.                                                                                                                       |
-| `--discord_webhook_url`            |                | If set, will send the result text to the discord channel.                                                                                                                                                |
-| `--telegram_token`                 |                | Token of Telegram bot.                                                                                                                                                                                   |
-| `--telegram_chat_id`               |                | If set, will send the result text to this Telegram chat. Needs to be used with \"--telegram_token\".                                                                                                     |
+| `--output_timestamps`              |               | Output the timestamp of the text when outputting the text.                                                                                                                                               |
+| `--hide_transcribe_result`         |               | Hide the result of Whisper transcribe.                                                                                                                                                                   |
+| `--output_file_path`               |               | If set, will save the result text to this path.                                                                                                                                                          |
+| `--cqhttp_url`                     |               | If set, will send the result text to the cqhttp server.                                                                                                                                                  |
+| `--cqhttp_token`                   |               | Token of cqhttp, if it is not set on the server side, it does not need to fill in.                                                                                                                       |
+| `--discord_webhook_url`            |               | If set, will send the result text to the discord channel.                                                                                                                                                |
+| `--telegram_token`                 |               | Token of Telegram bot.                                                                                                                                                                                   |
+| `--telegram_chat_id`               |               | If set, will send the result text to this Telegram chat. Needs to be used with \"--telegram_token\".                                                                                                     |
 
 ## Contact me
 
 Telegram: [@ionic_bond](https://t.me/ionic_bond)
 
 ## Donate
```

### Comparing `stream_translator_gpt-2024.5.25/README_PyPI.md` & `stream_translator_gpt-2024.5.4/README_PyPI.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 Try it on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ionic-bond/stream-translator-gpt/blob/main/stream_translator.ipynb)
 
 ## Prerequisites
 
 **Linux or Windows:**
 
 1. Python >= 3.8 (Recommend >= 3.10)
-2. [**Install CUDA on your system.**](https://developer.nvidia.com/cuda-downloads).
-3. [**Install cuDNN to your CUDA dir**](https://developer.nvidia.com/cudnn-downloads) if you want to use **Faseter-Whisper**.
+2. [**Install CUDA 11 on your system.**](https://developer.nvidia.com/cuda-11-8-0-download-archive) (Faster-Whisper is not compatible with CUDA 12 for now).
+3. [**Install cuDNN to your CUDA dir**](https://developer.nvidia.com/cuda-downloads) if you want to use **Faseter-Whisper**.
 4. [**Install PyTorch (with CUDA) to your Python.**](https://pytorch.org/get-started/locally/)
-5. [**Create a Google API key**](https://aistudio.google.com/app/apikey) if you want to use **Gemini API** for translation. (Free 15 requests / minute)
+5. [**Create a Google API key**](https://aistudio.google.com/app/apikey) if you want to use **Gemini API** for translation. (Recommend, Free 60 requests / minute)
 6. [**Create a OpenAI API key**](https://platform.openai.com/api-keys) if you want to use **Whisper API** for transcription or **GPT API** for translation.
 
 **If you are in Windows, you also need to:**
 
 1. [**Install and add ffmpeg to your PATH.**](https://www.thewindowsclub.com/how-to-install-ffmpeg-on-windows-10#:~:text=Click%20New%20and%20type%20the,Click%20OK%20to%20apply%20changes.)
 2. Install [**yt-dlp**](https://github.com/yt-dlp/yt-dlp) and add it to your PATH.
 
 ## Installation
 
 **Install release version from PyPI (Recommend):**
 
 ```
-pip install stream-translator-gpt -U
+pip install stream-translator-gpt
 stream-translator-gpt
 ```
 
 or
 
 **Clone master version code from Github:**
```

### Comparing `stream_translator_gpt-2024.5.25/pyproject.toml` & `stream_translator_gpt-2024.5.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stream-translator-gpt"
-version = "2024.5.25"
+version = "2024.5.4"
 authors = [
   { name="ion", email="ionicbond3@gmail.com" },
 ]
 description = "Command line tool to transcribe & translate audio from livestreams in real time"
 readme = "README_PyPI.md"
 requires-python = ">=3.8"
 keywords = [
@@ -41,15 +41,15 @@
 dependencies = [
   "numpy",
   "scipy",
   "yt-dlp",
   "ffmpeg-python>=0.2.0,<0.3",
   "sounddevice<1.0",
   "openai-whisper<=20231117",
-  "faster-whisper>=1.0.0,<2.0.0",
+  "faster-whisper>=0.8.0,<1.0.0",
   "openai>=1.0,<2.0",
   "google-generativeai<1.0",
 ]
 
 [project.scripts]
 stream-translator-gpt = "stream_translator_gpt.translator:cli"
```

### Comparing `stream_translator_gpt-2024.5.25/stream_translator_gpt/audio_getter.py` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/audio_getter.py`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.5.25/stream_translator_gpt/audio_slicer.py` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/audio_slicer.py`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.5.25/stream_translator_gpt/audio_transcriber.py` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/audio_transcriber.py`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.5.25/stream_translator_gpt/common.py` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/common.py`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.5.25/stream_translator_gpt/filters.py` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/filters.py`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.5.25/stream_translator_gpt/llm_translator.py` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/llm_translator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,31 @@
-import json
 import queue
 import threading
 import time
-import re
 from collections import deque
 from datetime import datetime, timedelta
 
 import google.generativeai as genai
 from google.api_core.exceptions import InternalServerError
 from google.generativeai.types import HarmCategory, HarmBlockThreshold
 from openai import OpenAI, APITimeoutError, APIConnectionError
 
 from .common import TranslationTask, LoopWorkerBase
 
 
-def _parse_json_completion(completion):
-    pattern = re.compile(r'\{.*}', re.DOTALL)
-    json_match = pattern.search(completion)
-
-    if json_match:
-        try:
-            json_str = json_match.group(0)
-            json_obj = json.loads(json_str)
-            translate_text = json_obj.get('translation', None)
-            if not translate_text:
-                return completion
-            return translate_text
-        except json.JSONDecodeError:
-            return completion
-    else:
-        return completion
-
-
 class LLMClint():
 
     class LLM_TYPE:
         GPT = 'GPT'
         GEMINI = 'Gemini'
 
     def __init__(self, llm_type: str, model: str, prompt: str, history_size: int) -> None:
         if llm_type not in (self.LLM_TYPE.GPT, self.LLM_TYPE.GEMINI):
             raise ValueError('Unknow LLM type: {}'.format(llm_type))
-        print('Using {} API as translation engine.'.format(model))
+        print('Using {} API as translation engine.'.format(llm_type))
         self.llm_type = llm_type
         self.model = model
         self.prompt = prompt
         self.history_size = history_size
         self.history_messages = []
 
     def _append_history_message(self, user_content: str, assistant_content: str):
@@ -60,32 +40,30 @@
         }])
         while (len(self.history_messages) > self.history_size * 2):
             self.history_messages.pop(0)
 
     def _translate_by_gpt(self, translation_task: TranslationTask):
         # https://platform.openai.com/docs/api-reference/chat/create?lang=python
         client = OpenAI()
-        system_prompt = 'You are a translation engine. Output the answer in json format, key is translation.'
+        system_prompt = 'You are a translation engine.'
         messages = [{'role': 'system', 'content': system_prompt}]
         messages.extend(self.history_messages)
         user_content = '{}: \n{}'.format(self.prompt, translation_task.transcribed_text)
         messages.append({'role': 'user', 'content': user_content})
         try:
             completion = client.chat.completions.create(
                 model=self.model,
                 temperature=0,
                 max_tokens=1000,
                 top_p=1,
                 frequency_penalty=1,
                 presence_penalty=1,
                 messages=messages,
             )
-
-            translation_task.translated_text = _parse_json_completion(
-                completion.choices[0].message.content)
+            translation_task.translated_text = completion.choices[0].message.content
         except (APITimeoutError, APIConnectionError) as e:
             print(e)
             return
         if self.history_size:
             self._append_history_message(user_content, translation_task.translated_text)
 
     @staticmethod
@@ -96,15 +74,15 @@
             gemini_message['role'] = gpt_message['role']
             if gemini_message['role'] == 'assistant':
                 gemini_message['role'] = 'model'
             gemini_message['parts'] = [gpt_message['content']]
             gemini_messages.append(gemini_message)
         return gemini_messages
 
-    def _translate_by_gemini(self, translation_task: TranslationTask):
+    def _translate_gy_gemini(self, translation_task: TranslationTask):
         # https://ai.google.dev/tutorials/python_quickstart
         client = genai.GenerativeModel(self.model)
         messages = self._gpt_to_gemini(self.history_messages)
         user_content = '{}: \n{}'.format(self.prompt, translation_task.transcribed_text)
         messages.append({'role': 'user', 'parts': [user_content]})
         config = genai.types.GenerationConfig(candidate_count=1, temperature=0)
         safety_settings = {
@@ -113,31 +91,32 @@
             HarmCategory.HARM_CATEGORY_SEXUALLY_EXPLICIT: HarmBlockThreshold.BLOCK_NONE,
             HarmCategory.HARM_CATEGORY_DANGEROUS_CONTENT: HarmBlockThreshold.BLOCK_NONE,
         }
         try:
             response = client.generate_content(messages,
                                                generation_config=config,
                                                safety_settings=safety_settings)
-            translation_task.translated_text = _parse_json_completion(response.text)
+            translation_task.translated_text = response.text
         except (ValueError, InternalServerError) as e:
             print(e)
             return
         if self.history_size:
             self._append_history_message(user_content, translation_task.translated_text)
 
     def translate(self, translation_task: TranslationTask):
         if self.llm_type == self.LLM_TYPE.GPT:
             self._translate_by_gpt(translation_task)
         elif self.llm_type == self.LLM_TYPE.GEMINI:
-            self._translate_by_gemini(translation_task)
+            self._translate_gy_gemini(translation_task)
         else:
             raise ValueError('Unknow LLM type: {}'.format(self.llm_type))
 
 
 class ParallelTranslator(LoopWorkerBase):
+
     PARALLEL_MAX_NUMBER = 10
 
     def __init__(self, llm_client: LLMClint, timeout: int, retry_if_translation_fails: bool):
         self.llm_client = llm_client
         self.timeout = timeout
         self.retry_if_translation_fails = retry_if_translation_fails
         self.processing_queue = deque()
```

### Comparing `stream_translator_gpt-2024.5.25/stream_translator_gpt/result_exporter.py` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/result_exporter.py`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.5.25/stream_translator_gpt/silero_vad.jit` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/silero_vad.jit`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.5.25/stream_translator_gpt/translator.py` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     thread.start()
 
 
 def main(url, format, cookies, device_index, frame_duration, continuous_no_speech_threshold,
          min_audio_length, max_audio_length, prefix_retention_length, vad_threshold, model,
          language, use_faster_whisper, use_whisper_api, whisper_filters, openai_api_key,
          google_api_key, gpt_translation_prompt, gpt_translation_history_size, gpt_model,
-         gemini_model, gpt_translation_timeout, gpt_base_url, retry_if_translation_fails,
-         output_timestamps, hide_transcribe_result, output_file_path, cqhttp_url, cqhttp_token,
-         discord_webhook_url, telegram_token, telegram_chat_id, **transcribe_options):
+         gpt_translation_timeout, gpt_base_url, retry_if_translation_fails, output_timestamps,
+         hide_transcribe_result, output_file_path, cqhttp_url, cqhttp_token, discord_webhook_url,
+         telegram_token, telegram_chat_id, **transcribe_options):
 
     if openai_api_key:
         os.environ['OPENAI_API_KEY'] = openai_api_key
     if gpt_base_url:
         os.environ['OPENAI_BASE_URL'] = gpt_base_url
     if google_api_key:
         genai.configure(api_key=google_api_key)
@@ -50,15 +50,15 @@
                          discord_webhook_url=discord_webhook_url,
                          telegram_token=telegram_token,
                          telegram_chat_id=telegram_chat_id,
                          input_queue=translator_to_exporter_queue)
     if gpt_translation_prompt:
         if google_api_key:
             llm_client = LLMClint(llm_type=LLMClint.LLM_TYPE.GEMINI,
-                                  model=gemini_model,
+                                  model='gemini-pro',
                                   prompt=gpt_translation_prompt,
                                   history_size=gpt_translation_history_size)
         else:
             llm_client = LLMClint(llm_type=LLMClint.LLM_TYPE.GPT,
                                   model=gpt_model,
                                   prompt=gpt_translation_prompt,
                                   history_size=gpt_translation_history_size)
@@ -230,25 +230,19 @@
                         type=str,
                         default=None,
                         help='OpenAI API key if using GPT translation / Whisper API.')
     parser.add_argument('--google_api_key',
                         type=str,
                         default=None,
                         help='Google API key if using Gemini translation.')
-    parser.add_argument('--gpt_model',
-                        type=str,
-                        default='gpt-3.5-turbo',
-                        help='OpenAI\'s GPT model name, gpt-3.5-turbo / gpt-4 / gpt-4o.')
     parser.add_argument(
-        '--gemini_model',
+        '--gpt_model',
         type=str,
-        default='gemini-1.0-pro',
-        help=
-        'Google\'s Gemini model name, gemini-1.0-pro / gemini-1.5-flash-latest / gemini-1.5-pro-latest'
-    )
+        default='gpt-3.5-turbo',
+        help='GPT model name, gpt-3.5-turbo or gpt-4. (If using Gemini, not need to change this)')
     parser.add_argument(
         '--gpt_translation_prompt',
         type=str,
         default=None,
         help='If set, will translate result text to target language via GPT / Gemini API. '
         'Example: \"Translate from Japanese to Chinese\"')
     parser.add_argument(
```

### Comparing `stream_translator_gpt-2024.5.25/stream_translator_gpt.egg-info/PKG-INFO` & `stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stream-translator-gpt
-Version: 2024.5.25
+Version: 2024.5.4
 Summary: Command line tool to transcribe & translate audio from livestreams in real time
 Author-email: ion <ionicbond3@gmail.com>
 Project-URL: Homepage, https://github.com/ionic-bond/stream-translator-gpt
 Project-URL: Issues, https://github.com/ionic-bond/stream-translator-gpt/issues
 Keywords: translator,translation,translate,transcribe,yt-dlp,vad,whisper,faster-whisper,whisper-api,gpt,gemini
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,15 +23,15 @@
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: yt-dlp
 Requires-Dist: ffmpeg-python<0.3,>=0.2.0
 Requires-Dist: sounddevice<1.0
 Requires-Dist: openai-whisper<=20231117
-Requires-Dist: faster-whisper<2.0.0,>=1.0.0
+Requires-Dist: faster-whisper<1.0.0,>=0.8.0
 Requires-Dist: openai<2.0,>=1.0
 Requires-Dist: google-generativeai<1.0
 
 # stream-translator-gpt
 
 Command line utility to transcribe or translate audio from livestreams in real time. Uses [yt-dlp](https://github.com/yt-dlp/yt-dlp) to 
 get livestream URLs from various services and [Whisper](https://github.com/openai/whisper) / [Faster-Whisper](https://github.com/SYSTRAN/faster-whisper) for transcription.
@@ -42,31 +42,31 @@
 Try it on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ionic-bond/stream-translator-gpt/blob/main/stream_translator.ipynb)
 
 ## Prerequisites
 
 **Linux or Windows:**
 
 1. Python >= 3.8 (Recommend >= 3.10)
-2. [**Install CUDA on your system.**](https://developer.nvidia.com/cuda-downloads).
-3. [**Install cuDNN to your CUDA dir**](https://developer.nvidia.com/cudnn-downloads) if you want to use **Faseter-Whisper**.
+2. [**Install CUDA 11 on your system.**](https://developer.nvidia.com/cuda-11-8-0-download-archive) (Faster-Whisper is not compatible with CUDA 12 for now).
+3. [**Install cuDNN to your CUDA dir**](https://developer.nvidia.com/cuda-downloads) if you want to use **Faseter-Whisper**.
 4. [**Install PyTorch (with CUDA) to your Python.**](https://pytorch.org/get-started/locally/)
-5. [**Create a Google API key**](https://aistudio.google.com/app/apikey) if you want to use **Gemini API** for translation. (Free 15 requests / minute)
+5. [**Create a Google API key**](https://aistudio.google.com/app/apikey) if you want to use **Gemini API** for translation. (Recommend, Free 60 requests / minute)
 6. [**Create a OpenAI API key**](https://platform.openai.com/api-keys) if you want to use **Whisper API** for transcription or **GPT API** for translation.
 
 **If you are in Windows, you also need to:**
 
 1. [**Install and add ffmpeg to your PATH.**](https://www.thewindowsclub.com/how-to-install-ffmpeg-on-windows-10#:~:text=Click%20New%20and%20type%20the,Click%20OK%20to%20apply%20changes.)
 2. Install [**yt-dlp**](https://github.com/yt-dlp/yt-dlp) and add it to your PATH.
 
 ## Installation
 
 **Install release version from PyPI (Recommend):**
 
 ```
-pip install stream-translator-gpt -U
+pip install stream-translator-gpt
 stream-translator-gpt
 ```
 
 or
 
 **Clone master version code from Github:**
```

### Comparing `stream_translator_gpt-2024.5.25/stream_translator_gpt.egg-info/SOURCES.txt` & `stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

