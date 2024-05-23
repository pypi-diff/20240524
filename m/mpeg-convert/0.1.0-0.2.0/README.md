# Comparing `tmp/mpeg-convert-0.1.0.tar.gz` & `tmp/mpeg_convert-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpeg-convert-0.1.0.tar", last modified: Wed Feb 21 22:55:47 2024, max compression
+gzip compressed data, was "mpeg_convert-0.2.0.tar", last modified: Thu May 23 22:49:45 2024, max compression
```

## Comparing `mpeg-convert-0.1.0.tar` & `mpeg_convert-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-02-21 22:55:47.826725 mpeg-convert-0.1.0/
--rw-r--r--   0 Dev        (502) staff       (20)     1063 2024-02-08 19:44:52.000000 mpeg-convert-0.1.0/LICENSE
--rw-r--r--   0 Dev        (502) staff       (20)     6448 2024-02-21 22:55:47.826418 mpeg-convert-0.1.0/PKG-INFO
--rw-r--r--   0 Dev        (502) staff       (20)     5510 2024-02-21 22:53:40.000000 mpeg-convert-0.1.0/README.md
--rw-r--r--   0 Dev        (502) staff       (20)        4 2024-02-21 22:55:38.000000 mpeg-convert-0.1.0/license.txt
--rw-r--r--   0 Dev        (502) staff       (20)     1082 2024-02-21 22:55:20.000000 mpeg-convert-0.1.0/pyproject.toml
--rw-r--r--   0 Dev        (502) staff       (20)       38 2024-02-21 22:55:47.826779 mpeg-convert-0.1.0/setup.cfg
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-02-21 22:55:47.822627 mpeg-convert-0.1.0/src/
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-02-21 22:55:47.824980 mpeg-convert-0.1.0/src/mpeg_convert/
--rw-r--r--   0 Dev        (502) staff       (20)     1753 2024-02-21 22:05:30.000000 mpeg-convert-0.1.0/src/mpeg_convert/__main__.py
--rw-r--r--   0 Dev        (502) staff       (20)     3417 2024-02-21 21:48:14.000000 mpeg-convert-0.1.0/src/mpeg_convert/argparsing.py
--rw-r--r--   0 Dev        (502) staff       (20)     8441 2024-02-21 22:03:38.000000 mpeg-convert-0.1.0/src/mpeg_convert/convert.py
--rw-r--r--   0 Dev        (502) staff       (20)     2874 2024-02-21 22:38:12.000000 mpeg-convert-0.1.0/src/mpeg_convert/customization.py
--rw-r--r--   0 Dev        (502) staff       (20)     8918 2024-02-21 21:30:28.000000 mpeg-convert-0.1.0/src/mpeg_convert/metadata.py
--rw-r--r--   0 Dev        (502) staff       (20)    14352 2024-02-21 22:38:50.000000 mpeg-convert-0.1.0/src/mpeg_convert/options.py
--rw-r--r--   0 Dev        (502) staff       (20)     5521 2024-02-21 21:52:36.000000 mpeg-convert-0.1.0/src/mpeg_convert/utils.py
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-02-21 22:55:47.826120 mpeg-convert-0.1.0/src/mpeg_convert.egg-info/
--rw-r--r--   0 Dev        (502) staff       (20)     6448 2024-02-21 22:55:47.000000 mpeg-convert-0.1.0/src/mpeg_convert.egg-info/PKG-INFO
--rw-r--r--   0 Dev        (502) staff       (20)      491 2024-02-21 22:55:47.000000 mpeg-convert-0.1.0/src/mpeg_convert.egg-info/SOURCES.txt
--rw-r--r--   0 Dev        (502) staff       (20)        1 2024-02-21 22:55:47.000000 mpeg-convert-0.1.0/src/mpeg_convert.egg-info/dependency_links.txt
--rw-r--r--   0 Dev        (502) staff       (20)       60 2024-02-21 22:55:47.000000 mpeg-convert-0.1.0/src/mpeg_convert.egg-info/entry_points.txt
--rw-r--r--   0 Dev        (502) staff       (20)       35 2024-02-21 22:55:47.000000 mpeg-convert-0.1.0/src/mpeg_convert.egg-info/requires.txt
--rw-r--r--   0 Dev        (502) staff       (20)       13 2024-02-21 22:55:47.000000 mpeg-convert-0.1.0/src/mpeg_convert.egg-info/top_level.txt
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-05-23 22:49:45.456501 mpeg_convert-0.2.0/
+-rw-r--r--   0 Dev        (502) staff       (20)     1063 2024-03-28 02:00:33.000000 mpeg_convert-0.2.0/LICENSE
+-rw-r--r--   0 Dev        (502) staff       (20)       33 2024-05-23 22:18:05.000000 mpeg_convert-0.2.0/MANIFEST.in
+-rw-r--r--   0 Dev        (502) staff       (20)     6120 2024-05-23 22:49:45.456274 mpeg_convert-0.2.0/PKG-INFO
+-rw-r--r--   0 Dev        (502) staff       (20)     5222 2024-05-23 22:48:25.000000 mpeg_convert-0.2.0/README.md
+-rw-r--r--   0 Dev        (502) staff       (20)     1046 2024-05-23 22:47:29.000000 mpeg_convert-0.2.0/pyproject.toml
+-rw-r--r--   0 Dev        (502) staff       (20)       38 2024-05-23 22:49:45.456543 mpeg_convert-0.2.0/setup.cfg
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-05-23 22:49:45.451735 mpeg_convert-0.2.0/src/
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-05-23 22:49:45.454461 mpeg_convert-0.2.0/src/mpeg_convert/
+-rw-r--r--   0 Dev        (502) staff       (20)     8196 2024-05-23 22:08:54.000000 mpeg_convert-0.2.0/src/mpeg_convert/.DS_Store
+-rw-r--r--   0 Dev        (502) staff       (20)     3429 2024-05-23 22:09:54.000000 mpeg_convert-0.2.0/src/mpeg_convert/__main__.py
+-rw-r--r--   0 Dev        (502) staff       (20)     4249 2024-05-23 22:23:37.000000 mpeg_convert-0.2.0/src/mpeg_convert/arguments.py
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-05-23 22:49:45.455689 mpeg_convert-0.2.0/src/mpeg_convert/assets/
+-rw-r--r--   0 Dev        (502) staff       (20)      469 2024-05-23 22:30:17.000000 mpeg_convert-0.2.0/src/mpeg_convert/assets/default.yml
+-rw-r--r--   0 Dev        (502) staff       (20)      734 2024-05-23 22:30:57.000000 mpeg_convert-0.2.0/src/mpeg_convert/assets/help.txt
+-rw-r--r--   0 Dev        (502) staff       (20)     2389 2024-05-23 22:45:40.000000 mpeg_convert-0.2.0/src/mpeg_convert/exceptions.py
+-rw-r--r--   0 Dev        (502) staff       (20)    10934 2024-05-23 18:34:06.000000 mpeg_convert-0.2.0/src/mpeg_convert/module.py
+-rw-r--r--   0 Dev        (502) staff       (20)     4083 2024-05-23 18:17:30.000000 mpeg_convert-0.2.0/src/mpeg_convert/term.py
+-rw-r--r--   0 Dev        (502) staff       (20)     4766 2024-05-23 18:34:03.000000 mpeg_convert-0.2.0/src/mpeg_convert/utils.py
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-05-23 22:49:45.456018 mpeg_convert-0.2.0/src/mpeg_convert.egg-info/
+-rw-r--r--   0 Dev        (502) staff       (20)     6120 2024-05-23 22:49:45.000000 mpeg_convert-0.2.0/src/mpeg_convert.egg-info/PKG-INFO
+-rw-r--r--   0 Dev        (502) staff       (20)      550 2024-05-23 22:49:45.000000 mpeg_convert-0.2.0/src/mpeg_convert.egg-info/SOURCES.txt
+-rw-r--r--   0 Dev        (502) staff       (20)        1 2024-05-23 22:49:45.000000 mpeg_convert-0.2.0/src/mpeg_convert.egg-info/dependency_links.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       60 2024-05-23 22:49:45.000000 mpeg_convert-0.2.0/src/mpeg_convert.egg-info/entry_points.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       49 2024-05-23 22:49:45.000000 mpeg_convert-0.2.0/src/mpeg_convert.egg-info/requires.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       13 2024-05-23 22:49:45.000000 mpeg_convert-0.2.0/src/mpeg_convert.egg-info/top_level.txt
```

### Comparing `mpeg-convert-0.1.0/LICENSE` & `mpeg_convert-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpeg-convert-0.1.0/PKG-INFO` & `mpeg_convert-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,156 +1,108 @@
 Metadata-Version: 2.1
 Name: mpeg-convert
-Version: 0.1.0
-Summary: A python tool based on ffmpeg that makes converting between different formats/codecs a whole lot easier for the inexperienced 
-Author-email: Zichen <zichenziv@icloud.com>
+Version: 0.2.0
+Summary: A python wrapper that enhances the user experience and productivity when using ffmpeg
+Author: Zichen
 License: MIT
-        
 Project-URL: Homepage, https://github.com/SomedudeX/mpeg-convert
 Project-URL: Issues, https://github.com/SomedudeX/mpeg-convert/issues
-Keywords: ffmpeg,convert,media,mp4,mp3
+Keywords: transcode,ffmpeg,convert,media,mp4,mp3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Utilities
 Classifier: Environment :: Console
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich>=13.7.0
+Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: python-ffmpeg>=2.0.10
 
-## MPEG-Convert
-
-A highly customizable<sup>[1](#Customizing)</sup> terminal-based [Python](https://www.python.org/downloads/) wrapper for [FFmpeg](https://ffmpeg.org/download.html) that provides a humanized approach to conversions between different multimedia formats. 
-
-FFmpeg is a powerful multimedia tool, but its many options<sup>[2](https://ffmpeg.org/ffmpeg.html)</sup> can be especially overwhelming for new users. This wrapper aims to simplify the process of working with the FFmpeg engine to convert between different video/audio formats for the folks who doesn't want to memorize twenty options to use FFmpeg. This program is not, however, a complete replacement for FFmpeg in any way. For that purpose, you should look look into other software such as [Handbrake](https://handbrake.fr/) or [DaVinci Resolve](https://www.blackmagicdesign.com/products/davinciresolve). 
-
-This project is now hosted on [PyPi](https://pypi.org/project/mpeg-convert), however legacy releases can still be found on the right. 
-
-## Features
-
-* **Simplified commands**: MPEG-Convert provides a straightforward interface for commonly used FFmpeg functionalities, making it easy for both beginners and experienced users to perform tasks such as codec conversion, audio extraction, video compression, and much more.
-
-* **Configurability**: While MPEG-Convert is designed for simplicity, it also provides room for customization<sup>[1](#Customizing)</sup>. You can tweak advanced settings by specifying additional FFmpeg options in the script or during script execution, ensuring flexibility for more sophisticated multimedia processing needs.
-
-![demo](https://github.com/SomedudeX/MPEG-Convert/assets/101906945/d69c68b0-4122-4ebc-a6fb-3de50448dcd0)
+A customizable<sup>[1](#Configuring)</sup> tool that provides some quality-of-life additions for [FFmpeg](https://ffmpeg.org) such as pretty printing, progress bars, and command presets. This tool does not aim to replace FFmpeg or other transcoding software such as [Handbrake](https://handbrake.fr/). Rather, it tries to provide an easier to use interface to FFmpeg for simple operations. 
 
 ## Installation 
 
-Make sure you have Python 3 and FFmpeg installed. 
+Ensure [Python](https://www.python.org/downloads/) and [FFmpeg](https://ffmpeg.org/download.html) is installed. Then, use the [Python Packaging Index](https://pypi.org/) (PyPI) to install `mpeg-convert` and its dependencies. You may need to use `pip3` instead of `pip` in certain environments: 
 
 ```bash
-pip install --upgrade mpeg-convert
-mpeg-convert --help
+$ pip install --upgrade mpeg-convert
+$ mpeg-convert --help
 ```
 
-## Customizing
+See [usages](#Usage) and [configuring](#Configuring) for a more details. 
 
-#### Interactive
+## Usage
 
-You can customize the interactive mode of the script by changing the questions variable `VIDEO_OPTIONS` and `AUDIO_OPTIONS` in mpeg-convert to your liking. This can be achieved using the `--customize` option, which will open the correct file for you in your default text editor.
+The most basic way to use `mpeg-convert` is to specify an input file path and an output file path. `mpeg-convert` will then call FFmpeg to initiate the conversion, and display a bar indicating the progress of the conversion. No extra FFmpeg options will be added when transcoding the file. This is demonstrated with the command and screenshot below: 
 
-The two variables represents the list of questions asked during video options and audio options sections of the script respectively. The properties of each question is represented as a dictionary in python, and will be shown to the user in order. The dictionaries' format is shown below:
-
-```py
-[
-    {
-        "type": <str>,
-        "title": <str>,
-        "option": <str>,
-        "default": <int>,
-        "choices": <list[tuple]>
-    }
-]
+```bash
+$ mpeg-convert sample.mp4 output.mov
 ```
 
- * **`type`**: The type of the question
+![no_preset_nobg](https://github.com/SomedudeX/mpeg-convert/assets/101906945/f990118f-0f3c-4f0d-aabf-5afa65efdb37)
 
-   * Valid values:
-     + **`choice`**: Multiple choice
-     + **`input`**: Input field
+For conversions where you may need or want to tweak extra options (e.g. frame rate, constrast, or bitrate changes), you can add a named or unnamed preset by following the [configuration guide](#Configuring). After you have saved your custom preset to the config file, you can use it by using the `--preset` flag for named presets, or convert between matching file containers/extensions for unnamed presets. This will use the extra custom FFmpeg options you specified in the preset when transcoding. This is demonstrated below:
 
- * **`title`**: The text shown to the console when displaying the question during the execution of the program
+```bash
+$ mpeg-convert sample.mp4 output.mov --preset="custom-1080p"
+```
 
- * **`option`**: The corresponding option in FFmpeg. This option will be inserted to the list of arguments passed to FFmpeg
+![yes_preset_nobg](https://github.com/SomedudeX/mpeg-convert/assets/101906945/44503c85-5bed-441a-9f6d-c241820b8c09)
 
- * **`default`**: The default option that is used when the input field is empty. Has no effect if question type is `input`.
+As of writing, presets are the only method to use FFmpeg options while converting with `mpeg-convert`. Additionally, multiple inputs and other advanced FFmpeg features are not supported by `mpeg-convert`. Such feature is unlikely to be added to `mpeg-convert`, since it is written as a complement, not replacement, to FFmpeg; consider directly using FFmpeg or other UI based programs such as Handbrake for such tasks. 
 
- * **`choices`**: A list of choices that will be shown to the console during the execution of the program. The choices will be in tuples where the first index will be what is displayed, and the second index is what is actually entered as a value for the particular FFmpeg option. Has no effect if question type is `input`.
+## Configuring
 
-An example of a custom question is below: 
+**Presets** allows you to save FFmpeg commands for repeated use, eliminating the need to enter long and complex flag/options each time you need to convert or edit media files. You can add presets to `mpeg-convert` by editing the YAML configuration file. To open the config, use the `--config` flag as demonstrated below:
 
-```py
-[
-    {
-        "type": "choice",
-        "title": "Select an encoding preset",
-        "option": "-preset",
-        "default": 3,
-        "choices": [
-            ("Faster/lower quality", "veryfast"),
-            ("Normal/medium quality", "medium"),
-            ("Slower/best quality", "veryslow")
-        ]
-    }
-]
+```bash
+$ mpeg-convert --config
 ```
 
-<br></br>
-
-#### Presets
+There are two types of presets you can specify in the config file: named presets and unnamed presets.
 
-Presets are different predetermined flags and options of FFmpeg options that mpeg-convert uses when you specify the name of the preset. Presets can be activated by specifying the name of the preset as a positional flag. You can customize them by modifying the `PRESETS` variable also located in `customization.py`. 
+ * **Named presets** are invoked when you explicitly use the `--preset` flag. You can add a named preset under the `named` key. Each named preset must have a unique name and a string of ffmpeg options. To activate a named preset, specify its name with the `--preset` flag, and `mpeg-convert` will use the options when converting. An example of a named preset is below:
 
-The preset's format is shown below: 
-```py
-{
-    "name": {
-        "option": <str>,
-        "option": <str>,
-        "option": <str>,
-        ...
-    }
-}
+```yml
+named:
+- name: "custom-1080p"
+  options: "-vf scale=1920x1080 -r 24"
 ```
 
- * **`name`**: The name that is used to activate the preset
+ * **Unnamed presets** are applied automatically to conversions of specific file types and extensions. They are useful when you want conversions between one container type and another container type to always use certain FFmpeg options. Each unnamed preset must have an array of file extensions in `from-type` and `to-type`, and a string of FFmpeg options; and voilà, whenever you convert between any of the file extensions in `from-type` to any of the extensions in `to-type`, `mpeg-convert` will automatically use the FFmpeg options specified in the unnamed preset. An example of an unnamed preset is below:
 
- * **`option`**: A command-line option to be inserted to the list of arguments passed to FFmpeg. The option should be stripped of the dash (-) symbol at the front. If the FFmpeg option does not take any value, put `None` after the colon. There can be more than one option in each preset. 
- 
-An example of a custom preset is below:
-
-```py
-{
-    "flac-audio": {
-        "vn": None,
-        "ar": "96000",
-        "codec:a": "flac",
-        "sample_fmt": "s24",
-    }
-}
+```yml
+unnamed:
+- from-type: ["mp4", "mov"]
+  to-type: ["gif"]
+  command: "-vf scale=1280x720 -r 8"
 ```
 
+If you have an unnamed preset specified for a file type you are converting to/from, but you would like to temporarily disable it, you can use the `--plain` flag. This will remove any FFmpeg options for the current conversion.
+
+When searching for matching presets, `mpeg-convert` will check using the following order:
+ * Check if `--plain` flag is specified. If not...
+ * Check if `--preset` flag is specified. If not...
+ * Check if there is a matching unnamed preset. If not...
+ * Initiate the conversion without any FFmpeg commands
+
 ## Troubleshooting
 
 * Do you have python installed?
 * Do you have ffmpeg installed?
 * Common pitfalls:
   + Does the output file have an extension?
   + Does the extension match the codec?
     - `HEVC` with `.mp4`
     - `ALAC` with `.m4a`
   + Is the encoder installed on your system?
 
-## Resources
-
- - [Demo](https://github.com/SomedudeX/mpeg-convert/raw/main/demo.mp4)
- - [License](https://raw.githubusercontent.com/SomedudeX/mpeg-convert/main/LICENSE)
- - [Project](https://pypi.org/project/mpeg-convert/)
+## Notes
 
-Contributions are welcome! If you encounter any problems or find any bugs, please feel free to open an issue. In the meantime, happy converting! 
+This project has undergone substantial changes in `v0.2.0`. Click [here](https://github.com/SomedudeX/mpeg-convert/blob/15f4026633c5da667e6283cdeb78d82b29cd1b3d/README.md) if you are looking for documentation before `v0.2.0`
 
 --
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mpeg-convert-0.1.0/README.md` & `mpeg_convert-0.2.0/src/mpeg_convert.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,132 +1,108 @@
-## MPEG-Convert
+Metadata-Version: 2.1
+Name: mpeg-convert
+Version: 0.2.0
+Summary: A python wrapper that enhances the user experience and productivity when using ffmpeg
+Author: Zichen
+License: MIT
+Project-URL: Homepage, https://github.com/SomedudeX/mpeg-convert
+Project-URL: Issues, https://github.com/SomedudeX/mpeg-convert/issues
+Keywords: transcode,ffmpeg,convert,media,mp4,mp3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python
+Classifier: Topic :: Multimedia
+Classifier: Topic :: Utilities
+Classifier: Environment :: Console
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: rich>=13.7.0
+Requires-Dist: pyyaml>=6.0.1
+Requires-Dist: python-ffmpeg>=2.0.10
 
-A highly customizable<sup>[1](#Customizing)</sup> terminal-based [Python](https://www.python.org/downloads/) wrapper for [FFmpeg](https://ffmpeg.org/download.html) that provides a humanized approach to conversions between different multimedia formats. 
-
-FFmpeg is a powerful multimedia tool, but its many options<sup>[2](https://ffmpeg.org/ffmpeg.html)</sup> can be especially overwhelming for new users. This wrapper aims to simplify the process of working with the FFmpeg engine to convert between different video/audio formats for the folks who doesn't want to memorize twenty options to use FFmpeg. This program is not, however, a complete replacement for FFmpeg in any way. For that purpose, you should look look into other software such as [Handbrake](https://handbrake.fr/) or [DaVinci Resolve](https://www.blackmagicdesign.com/products/davinciresolve). 
-
-This project is now hosted on [PyPi](https://pypi.org/project/mpeg-convert), however legacy releases can still be found on the right. 
-
-## Features
-
-* **Simplified commands**: MPEG-Convert provides a straightforward interface for commonly used FFmpeg functionalities, making it easy for both beginners and experienced users to perform tasks such as codec conversion, audio extraction, video compression, and much more.
-
-* **Configurability**: While MPEG-Convert is designed for simplicity, it also provides room for customization<sup>[1](#Customizing)</sup>. You can tweak advanced settings by specifying additional FFmpeg options in the script or during script execution, ensuring flexibility for more sophisticated multimedia processing needs.
-
-![demo](https://github.com/SomedudeX/MPEG-Convert/assets/101906945/d69c68b0-4122-4ebc-a6fb-3de50448dcd0)
+A customizable<sup>[1](#Configuring)</sup> tool that provides some quality-of-life additions for [FFmpeg](https://ffmpeg.org) such as pretty printing, progress bars, and command presets. This tool does not aim to replace FFmpeg or other transcoding software such as [Handbrake](https://handbrake.fr/). Rather, it tries to provide an easier to use interface to FFmpeg for simple operations. 
 
 ## Installation 
 
-Make sure you have Python 3 and FFmpeg installed. 
+Ensure [Python](https://www.python.org/downloads/) and [FFmpeg](https://ffmpeg.org/download.html) is installed. Then, use the [Python Packaging Index](https://pypi.org/) (PyPI) to install `mpeg-convert` and its dependencies. You may need to use `pip3` instead of `pip` in certain environments: 
 
 ```bash
-pip install --upgrade mpeg-convert
-mpeg-convert --help
+$ pip install --upgrade mpeg-convert
+$ mpeg-convert --help
 ```
 
-## Customizing
+See [usages](#Usage) and [configuring](#Configuring) for a more details. 
 
-#### Interactive
+## Usage
 
-You can customize the interactive mode of the script by changing the questions variable `VIDEO_OPTIONS` and `AUDIO_OPTIONS` in mpeg-convert to your liking. This can be achieved using the `--customize` option, which will open the correct file for you in your default text editor.
+The most basic way to use `mpeg-convert` is to specify an input file path and an output file path. `mpeg-convert` will then call FFmpeg to initiate the conversion, and display a bar indicating the progress of the conversion. No extra FFmpeg options will be added when transcoding the file. This is demonstrated with the command and screenshot below: 
 
-The two variables represents the list of questions asked during video options and audio options sections of the script respectively. The properties of each question is represented as a dictionary in python, and will be shown to the user in order. The dictionaries' format is shown below:
-
-```py
-[
-    {
-        "type": <str>,
-        "title": <str>,
-        "option": <str>,
-        "default": <int>,
-        "choices": <list[tuple]>
-    }
-]
+```bash
+$ mpeg-convert sample.mp4 output.mov
 ```
 
- * **`type`**: The type of the question
+![no_preset_nobg](https://github.com/SomedudeX/mpeg-convert/assets/101906945/f990118f-0f3c-4f0d-aabf-5afa65efdb37)
 
-   * Valid values:
-     + **`choice`**: Multiple choice
-     + **`input`**: Input field
+For conversions where you may need or want to tweak extra options (e.g. frame rate, constrast, or bitrate changes), you can add a named or unnamed preset by following the [configuration guide](#Configuring). After you have saved your custom preset to the config file, you can use it by using the `--preset` flag for named presets, or convert between matching file containers/extensions for unnamed presets. This will use the extra custom FFmpeg options you specified in the preset when transcoding. This is demonstrated below:
 
- * **`title`**: The text shown to the console when displaying the question during the execution of the program
+```bash
+$ mpeg-convert sample.mp4 output.mov --preset="custom-1080p"
+```
 
- * **`option`**: The corresponding option in FFmpeg. This option will be inserted to the list of arguments passed to FFmpeg
+![yes_preset_nobg](https://github.com/SomedudeX/mpeg-convert/assets/101906945/44503c85-5bed-441a-9f6d-c241820b8c09)
 
- * **`default`**: The default option that is used when the input field is empty. Has no effect if question type is `input`.
+As of writing, presets are the only method to use FFmpeg options while converting with `mpeg-convert`. Additionally, multiple inputs and other advanced FFmpeg features are not supported by `mpeg-convert`. Such feature is unlikely to be added to `mpeg-convert`, since it is written as a complement, not replacement, to FFmpeg; consider directly using FFmpeg or other UI based programs such as Handbrake for such tasks. 
 
- * **`choices`**: A list of choices that will be shown to the console during the execution of the program. The choices will be in tuples where the first index will be what is displayed, and the second index is what is actually entered as a value for the particular FFmpeg option. Has no effect if question type is `input`.
+## Configuring
 
-An example of a custom question is below: 
+**Presets** allows you to save FFmpeg commands for repeated use, eliminating the need to enter long and complex flag/options each time you need to convert or edit media files. You can add presets to `mpeg-convert` by editing the YAML configuration file. To open the config, use the `--config` flag as demonstrated below:
 
-```py
-[
-    {
-        "type": "choice",
-        "title": "Select an encoding preset",
-        "option": "-preset",
-        "default": 3,
-        "choices": [
-            ("Faster/lower quality", "veryfast"),
-            ("Normal/medium quality", "medium"),
-            ("Slower/best quality", "veryslow")
-        ]
-    }
-]
+```bash
+$ mpeg-convert --config
 ```
 
-<br></br>
-
-#### Presets
+There are two types of presets you can specify in the config file: named presets and unnamed presets.
 
-Presets are different predetermined flags and options of FFmpeg options that mpeg-convert uses when you specify the name of the preset. Presets can be activated by specifying the name of the preset as a positional flag. You can customize them by modifying the `PRESETS` variable also located in `customization.py`. 
+ * **Named presets** are invoked when you explicitly use the `--preset` flag. You can add a named preset under the `named` key. Each named preset must have a unique name and a string of ffmpeg options. To activate a named preset, specify its name with the `--preset` flag, and `mpeg-convert` will use the options when converting. An example of a named preset is below:
 
-The preset's format is shown below: 
-```py
-{
-    "name": {
-        "option": <str>,
-        "option": <str>,
-        "option": <str>,
-        ...
-    }
-}
+```yml
+named:
+- name: "custom-1080p"
+  options: "-vf scale=1920x1080 -r 24"
 ```
 
- * **`name`**: The name that is used to activate the preset
+ * **Unnamed presets** are applied automatically to conversions of specific file types and extensions. They are useful when you want conversions between one container type and another container type to always use certain FFmpeg options. Each unnamed preset must have an array of file extensions in `from-type` and `to-type`, and a string of FFmpeg options; and voilà, whenever you convert between any of the file extensions in `from-type` to any of the extensions in `to-type`, `mpeg-convert` will automatically use the FFmpeg options specified in the unnamed preset. An example of an unnamed preset is below:
 
- * **`option`**: A command-line option to be inserted to the list of arguments passed to FFmpeg. The option should be stripped of the dash (-) symbol at the front. If the FFmpeg option does not take any value, put `None` after the colon. There can be more than one option in each preset. 
- 
-An example of a custom preset is below:
-
-```py
-{
-    "flac-audio": {
-        "vn": None,
-        "ar": "96000",
-        "codec:a": "flac",
-        "sample_fmt": "s24",
-    }
-}
+```yml
+unnamed:
+- from-type: ["mp4", "mov"]
+  to-type: ["gif"]
+  command: "-vf scale=1280x720 -r 8"
 ```
 
+If you have an unnamed preset specified for a file type you are converting to/from, but you would like to temporarily disable it, you can use the `--plain` flag. This will remove any FFmpeg options for the current conversion.
+
+When searching for matching presets, `mpeg-convert` will check using the following order:
+ * Check if `--plain` flag is specified. If not...
+ * Check if `--preset` flag is specified. If not...
+ * Check if there is a matching unnamed preset. If not...
+ * Initiate the conversion without any FFmpeg commands
+
 ## Troubleshooting
 
 * Do you have python installed?
 * Do you have ffmpeg installed?
 * Common pitfalls:
   + Does the output file have an extension?
   + Does the extension match the codec?
     - `HEVC` with `.mp4`
     - `ALAC` with `.m4a`
   + Is the encoder installed on your system?
 
-## Resources
-
- - [Demo](https://github.com/SomedudeX/mpeg-convert/raw/main/demo.mp4)
- - [License](https://raw.githubusercontent.com/SomedudeX/mpeg-convert/main/LICENSE)
- - [Project](https://pypi.org/project/mpeg-convert/)
+## Notes
 
-Contributions are welcome! If you encounter any problems or find any bugs, please feel free to open an issue. In the meantime, happy converting! 
+This project has undergone substantial changes in `v0.2.0`. Click [here](https://github.com/SomedudeX/mpeg-convert/blob/15f4026633c5da667e6283cdeb78d82b29cd1b3d/README.md) if you are looking for documentation before `v0.2.0`
 
 --
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mpeg-convert-0.1.0/pyproject.toml` & `mpeg_convert-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mpeg-convert"
-version = "0.1.0"
-requires-python = ">=3.9"
-description = "A python tool based on ffmpeg that makes converting between different formats/codecs a whole lot easier for the inexperienced "
-authors = [{ name = "Zichen", email = "zichenziv@icloud.com" }]
+version = "0.2.0"
+requires-python = ">=3.8"
+description = "A python wrapper that enhances the user experience and productivity when using ffmpeg"
+authors = [{ name = "Zichen" }]
 readme = "README.md"
-license = { file = "license.txt" }
-keywords = ["ffmpeg", "convert", "media", "mp4", "mp3"]
+license = { text = "MIT" }
+keywords = ["transcode", "ffmpeg", "convert", "media", "mp4", "mp3"]
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python",
     "Topic :: Multimedia",
     "Topic :: Utilities",
     "Environment :: Console",
 ]
 
-dependencies = ["rich>=13.7.0", "python-ffmpeg>=2.0.10"]
+dependencies = [
+    "rich>=13.7.0", 
+    "pyyaml>=6.0.1",
+    "python-ffmpeg>=2.0.10"
+]
 
 [project.urls]
 Homepage = "https://github.com/SomedudeX/mpeg-convert"
 Issues = "https://github.com/SomedudeX/mpeg-convert/issues"
 
 
 [project.scripts]
```

