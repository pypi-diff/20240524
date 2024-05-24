# Comparing `tmp/openai_commands-3.3.1.tar.gz` & `tmp/openai_commands-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_commands-3.3.1.tar", last modified: Fri May 24 02:27:42 2024, max compression
+gzip compressed data, was "openai_commands-3.4.1.tar", last modified: Fri May 24 02:40:49 2024, max compression
```

## Comparing `openai_commands-3.3.1.tar` & `openai_commands-3.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-24 02:27:42.947098 openai_commands-3.3.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-03-26 02:08:32.000000 openai_commands-3.3.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-24 02:13:20.000000 openai_commands-3.3.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     8371 2024-05-24 02:27:42.945783 openai_commands-3.3.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     6714 2024-03-31 21:22:29.000000 openai_commands-3.3.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-24 02:27:42.940939 openai_commands-3.3.1/openai_commands/
--rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-24 02:27:34.000000 openai_commands-3.3.1/openai_commands/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1234 2024-03-26 02:08:32.000000 openai_commands-3.3.1/openai_commands/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      461 2024-04-15 03:54:15.000000 openai_commands-3.3.1/openai_commands/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)       91 2024-03-26 02:08:32.000000 openai_commands-3.3.1/openai_commands/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-03-26 02:08:32.000000 openai_commands-3.3.1/openai_commands/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-24 02:27:42.944513 openai_commands-3.3.1/openai_commands.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     8371 2024-05-24 02:27:42.000000 openai_commands-3.3.1/openai_commands.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      393 2024-05-24 02:27:42.000000 openai_commands-3.3.1/openai_commands.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-24 02:27:42.000000 openai_commands-3.3.1/openai_commands.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      204 2024-05-24 02:27:42.000000 openai_commands-3.3.1/openai_commands.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       16 2024-05-24 02:27:42.000000 openai_commands-3.3.1/openai_commands.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-24 02:13:20.000000 openai_commands-3.3.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      264 2024-05-24 02:11:50.000000 openai_commands-3.3.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-24 02:27:42.947297 openai_commands-3.3.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      234 2024-05-24 02:20:01.000000 openai_commands-3.3.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-24 02:40:49.747569 openai_commands-3.4.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-24 02:29:00.000000 openai_commands-3.4.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-24 02:29:00.000000 openai_commands-3.4.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     8461 2024-05-24 02:40:49.746383 openai_commands-3.4.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     6744 2024-05-24 02:35:54.000000 openai_commands-3.4.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-24 02:40:49.740052 openai_commands-3.4.1/openai_commands/
+-rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-24 02:40:41.000000 openai_commands-3.4.1/openai_commands/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1249 2024-05-24 02:38:45.000000 openai_commands-3.4.1/openai_commands/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      461 2024-05-24 02:29:00.000000 openai_commands-3.4.1/openai_commands/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       96 2024-05-24 02:38:46.000000 openai_commands-3.4.1/openai_commands/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-24 02:29:00.000000 openai_commands-3.4.1/openai_commands/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-24 02:40:49.745122 openai_commands-3.4.1/openai_commands.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     8461 2024-05-24 02:40:49.000000 openai_commands-3.4.1/openai_commands.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      393 2024-05-24 02:40:49.000000 openai_commands-3.4.1/openai_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-24 02:40:49.000000 openai_commands-3.4.1/openai_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      204 2024-05-24 02:40:49.000000 openai_commands-3.4.1/openai_commands.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       16 2024-05-24 02:40:49.000000 openai_commands-3.4.1/openai_commands.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-24 02:29:00.000000 openai_commands-3.4.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      264 2024-05-24 02:29:00.000000 openai_commands-3.4.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-24 02:40:49.747840 openai_commands-3.4.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      239 2024-05-24 02:30:24.000000 openai_commands-3.4.1/setup.py
```

### Comparing `openai_commands-3.3.1/LICENSE` & `openai_commands-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_commands-3.3.1/PKG-INFO` & `openai_commands-3.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: openai_commands
-Version: 3.3.1
+Version: 3.4.1
 Summary: 🛠️ a command interface to the OpenAI API
-Home-page: https://github.com/kamangir/openai-cli
+Home-page: https://github.com/kamangir/openai-commands
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
@@ -31,72 +31,72 @@
 Requires-Dist: pylint
 Requires-Dist: pytest
 Requires-Dist: python-dotenv[cli]
 Requires-Dist: requests
 Requires-Dist: scikit-image
 Requires-Dist: tqdm
 
-# 🛠️ openai-cli (`@openai`)
+# 🛠️ openai-commands (`@openai`)
 
-`@openai` is a bash cli for the [OpenAI API](https://beta.openai.com/docs/introduction).
+`@openai` is a bash interface to the [OpenAI API](https://beta.openai.com/docs/introduction).
 
 🔷 [completion](#Completion) 🔷 [code generation](#code-generation) 🔷 [sentence -> image](#sentence---image) 🔷 [text -> mural](#text---mural) 🔷 [vision](#vision) 🔷 [images](#images) 🔷 [gpt](#gpt) 🔷 [VisuaLyze](#VisuaLyze) 🔷
 
 ## Install
 
 Install [`awesome-bash-cli`](https://github.com/kamangir/awesome-bash-cli) (`abcli`), then,
 
 ```bash
-abcli git clone openai_cli install
+abcli git clone openai-commands install
 ```
 
 ```bash
 ...
 ```
 
 ## Completion
 
 ```bash
 @openai complete "describe mathematics"
 ```
 
 > Mathematics is an abstract science that examines topics such as quantity, structure, space, change, and other topics in various ways. It involves the use of logic, algorithms, and formulas to solve problems. Mathematics can be used to study the natural world, to describe phenomena, and to make predictions about the future. It provides the foundation for the development of a wide range of disciplines in science, technology, engineering, economics, finance, and more.
 
-also works [in a notebook](https://raw.githubusercontent.com/kamangir/openai-cli/main/notebooks/completion.ipynb).
+also works [in a notebook](https://raw.githubusercontent.com/kamangir/openai-commands/main/notebooks/completion.ipynb).
 
 ## Code Generation
 
-Example notebooks to [generate a python functions](https://raw.githubusercontent.com/kamangir/openai-cli/main/notebooks/completion_ai_function_py.ipynb), special case for [image to image python functions](https://raw.githubusercontent.com/kamangir/openai-cli/main/notebooks/completion_i2i_function.ipynb), and to [write a bash script](https://raw.githubusercontent.com/kamangir/openai-cli/main/notebooks/completion_ai_function_bash.ipynb) to use a script, for example, [Vancouver-Watching](https://github.com/kamangir/Vancouver-Watching).
+Example notebooks to [generate a python functions](https://raw.githubusercontent.com/kamangir/openai-commands/main/notebooks/completion_ai_function_py.ipynb), special case for [image to image python functions](https://raw.githubusercontent.com/kamangir/openai-commands/main/notebooks/completion_i2i_function.ipynb), and to [write a bash script](https://raw.githubusercontent.com/kamangir/openai-commands/main/notebooks/completion_ai_function_bash.ipynb) to use a script, for example, [Vancouver-Watching](https://github.com/kamangir/Vancouver-Watching).
 
-![image](https://raw.githubusercontent.com/kamangir/openai-cli/main/assets/completion_i2i_function.png)
+![image](https://raw.githubusercontent.com/kamangir/openai-commands/main/assets/completion_i2i_function.png)
 
 ## Sentence -> Image
 
 ```bash
 @select - open; \
 @openai generate image \
   ~dryrun,height=1024,width=1024 \
   carrot - \
   "an orange carrot walking on Mars."
 ```
 
-![image](https://raw.githubusercontent.com/kamangir/openai-cli/main/assets/carrot.png)
+![image](https://raw.githubusercontent.com/kamangir/openai-commands/main/assets/carrot.png)
 
 ## Text -> Mural
 
 "[The Laughing Heart](https://allpoetry.com/poem/14326890-The-Laughing-Heart-by-Charles-Bukowski)" by Charles Bukowski, [more examples](http://kamangir.net/private/?object=2023-03-26-19-10-26-51814).
 
 ```bash
 @select - open; \
 DALL-E render  \
   ~dryrun,publish,url,verbose \
   https://allpoetry.com/poem/14326890-The-Laughing-Heart-by-Charles-Bukowski
 ```
 
-![image](https://raw.githubusercontent.com/kamangir/openai-cli/main/assets/DALL-E.png)
+![image](https://raw.githubusercontent.com/kamangir/openai-commands/main/assets/DALL-E.png)
 
 ## Vision
 
 Implements the [OpenAI vision API](https://platform.openai.com/docs/guides/vision).
 
 > GPT-4 with Vision ... `GPT-4V` or `gpt-4-vision-preview` in the API ... model ... take in images and answer questions about them
 > ... not stateful ... ([more](https://arash-kamangir.medium.com/%EF%B8%8F-openai-vision-1-fb3691bd095a))
@@ -131,24 +131,24 @@
 
 > The images show street scenes captured by surveillance cameras at night, and each bears a timestamp and the text "CITY OF VANCOUVER" indicating they're from Vancouver. In the first image, you see a yellow traffic light indicating caution and part of a crosswalk painted in rainbow colors, likely symbolizing support for the LGBTQ+ community. In the second image, there's a view of a city street with pedestrians crossing, some wearing reflective vests, and the storefronts illuminated with bright lights. The third image shows a different angle of a similar street scene with the same vibrant crosswalk and vehicles' headlights creating streaks of light due to the camera exposure. Finally, in the fourth image, there's a view of parked cars and a clearly visible police vehicle, suggesting the presence of law enforcement nearby. The wet pavement suggests it may have rained, and the reflections imply the street is well-lit at night.
 
 ## images
 
 Implements the [OpenAI Image Generation API](https://platform.openai.com/docs/guides/images/usage?context=python).
 
-Notebook implementation [`https://raw.githubusercontent.com/kamangir/openai-cli/main/notebooks/images.ipynb`](https://raw.githubusercontent.com/kamangir/openai-cli/main/notebooks/images.ipynb),
+Notebook implementation [`https://raw.githubusercontent.com/kamangir/openai-commands/main/notebooks/images.ipynb`](https://raw.githubusercontent.com/kamangir/openai-commands/main/notebooks/images.ipynb),
 
 ```bash
 @select - open; \
 @openai images generate - \
 	"a person flying through the streets of Vancouver." \
 	. --verbose 1
 ```
 
-![image](https://github.com/kamangir/assets/blob/main/openai_cli/2024-01-20-19-00-28-67378.png?raw=true)
+![image](https://github.com/kamangir/assets/blob/main/openai_commands/2024-01-20-19-00-28-67378.png?raw=true)
 
 ## gpt
 
 co-authored with ChapGPT.
 
 ```bash
 gpt
@@ -163,23 +163,23 @@
 gpt list_models [-] \
 	[--log 0]
  . list models.
 ```
 
 ## VisuaLyze
 
-> How about calling it "VisuaLyze"? This name combines "visualize" and "analyze," reflecting the tool's capability to generate custom data visualizations and analyze user input through AI - OpenAI, [more](https://raw.githubusercontent.com/kamangir/openai-cli/main/openai_cli/VisuaLyze/)
+> How about calling it "VisuaLyze"? This name combines "visualize" and "analyze," reflecting the tool's capability to generate custom data visualizations and analyze user input through AI - OpenAI, [more](https://raw.githubusercontent.com/kamangir/openai-commands/main/openai_commands/VisuaLyze/)
 
 ```bash
 VisuaLyze run
 ```
 
-![image](https://github.com/kamangir/openai-cli/assets/1007567/7c0ed5f7-6941-451c-a17e-504c6adab23f)
+![image](https://github.com/kamangir/openai-commands/assets/1007567/7c0ed5f7-6941-451c-a17e-504c6adab23f)
 
-sample output for [`onlinefoods`](https://raw.githubusercontent.com/kamangir/openai-cli/main/assets/VisuaLyze/onlinefoods/).
+sample output for [`onlinefoods`](https://raw.githubusercontent.com/kamangir/openai-commands/main/assets/VisuaLyze/onlinefoods/).
 
 ```python
 import pandas as pd
 import matplotlib.pyplot as plt
 
 def VisuaLyze(df: pd.DataFrame()):
     # Generate a matplotlib visualization of one aspect of the dataset
```

### Comparing `openai_commands-3.3.1/README.md` & `openai_commands-3.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# 🛠️ openai-cli (`@openai`)
+# 🛠️ openai-commands (`@openai`)
 
-`@openai` is a bash cli for the [OpenAI API](https://beta.openai.com/docs/introduction).
+`@openai` is a bash interface to the [OpenAI API](https://beta.openai.com/docs/introduction).
 
 🔷 [completion](#Completion) 🔷 [code generation](#code-generation) 🔷 [sentence -> image](#sentence---image) 🔷 [text -> mural](#text---mural) 🔷 [vision](#vision) 🔷 [images](#images) 🔷 [gpt](#gpt) 🔷 [VisuaLyze](#VisuaLyze) 🔷
 
 ## Install
 
 Install [`awesome-bash-cli`](https://github.com/kamangir/awesome-bash-cli) (`abcli`), then,
 
 ```bash
-abcli git clone openai_cli install
+abcli git clone openai-commands install
 ```
 
 ```bash
 ...
 ```
 
 ## Completion
@@ -103,15 +103,15 @@
 ```bash
 @select - open; \
 @openai images generate - \
 	"a person flying through the streets of Vancouver." \
 	. --verbose 1
 ```
 
-![image](https://github.com/kamangir/assets/blob/main/openai_cli/2024-01-20-19-00-28-67378.png?raw=true)
+![image](https://github.com/kamangir/assets/blob/main/openai_commands/2024-01-20-19-00-28-67378.png?raw=true)
 
 ## gpt
 
 co-authored with ChapGPT.
 
 ```bash
 gpt
@@ -126,21 +126,21 @@
 gpt list_models [-] \
 	[--log 0]
  . list models.
 ```
 
 ## VisuaLyze
 
-> How about calling it "VisuaLyze"? This name combines "visualize" and "analyze," reflecting the tool's capability to generate custom data visualizations and analyze user input through AI - OpenAI, [more](./openai_cli/VisuaLyze/)
+> How about calling it "VisuaLyze"? This name combines "visualize" and "analyze," reflecting the tool's capability to generate custom data visualizations and analyze user input through AI - OpenAI, [more](./openai_commands/VisuaLyze/)
 
 ```bash
 VisuaLyze run
 ```
 
-![image](https://github.com/kamangir/openai-cli/assets/1007567/7c0ed5f7-6941-451c-a17e-504c6adab23f)
+![image](https://github.com/kamangir/openai-commands/assets/1007567/7c0ed5f7-6941-451c-a17e-504c6adab23f)
 
 sample output for [`onlinefoods`](./assets/VisuaLyze/onlinefoods/).
 
 ```python
 import pandas as pd
 import matplotlib.pyplot as plt
```

### Comparing `openai_commands-3.3.1/openai_commands/__main__.py` & `openai_commands-3.4.1/openai_commands/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
-from openai_cli import NAME, VERSION, DESCRIPTION
-from openai_cli.logger import logger
+from openai_commands import NAME, VERSION, DESCRIPTION
+from openai_commands.logger import logger
 
 parser = argparse.ArgumentParser(NAME, description=f"{NAME}-{VERSION}")
 parser.add_argument(
     "task",
     type=str,
     help="complete|version",
 )
@@ -29,15 +29,15 @@
     help="0|1",
     default=0,
 )
 args = parser.parse_args()
 
 success = False
 if args.task == "complete":
-    from openai_cli.completion.api import complete_prompt
+    from openai_commands.completion.api import complete_prompt
 
     success, text, _ = complete_prompt(
         args.prompt,
         args.max_token,
         args.verbose == 1,
     )
     print(text)
```

### Comparing `openai_commands-3.3.1/openai_commands.egg-info/PKG-INFO` & `openai_commands-3.4.1/openai_commands.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: openai_commands
-Version: 3.3.1
+Version: 3.4.1
 Summary: 🛠️ a command interface to the OpenAI API
-Home-page: https://github.com/kamangir/openai-cli
+Home-page: https://github.com/kamangir/openai-commands
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
@@ -31,72 +31,72 @@
 Requires-Dist: pylint
 Requires-Dist: pytest
 Requires-Dist: python-dotenv[cli]
 Requires-Dist: requests
 Requires-Dist: scikit-image
 Requires-Dist: tqdm
 
-# 🛠️ openai-cli (`@openai`)
+# 🛠️ openai-commands (`@openai`)
 
-`@openai` is a bash cli for the [OpenAI API](https://beta.openai.com/docs/introduction).
+`@openai` is a bash interface to the [OpenAI API](https://beta.openai.com/docs/introduction).
 
 🔷 [completion](#Completion) 🔷 [code generation](#code-generation) 🔷 [sentence -> image](#sentence---image) 🔷 [text -> mural](#text---mural) 🔷 [vision](#vision) 🔷 [images](#images) 🔷 [gpt](#gpt) 🔷 [VisuaLyze](#VisuaLyze) 🔷
 
 ## Install
 
 Install [`awesome-bash-cli`](https://github.com/kamangir/awesome-bash-cli) (`abcli`), then,
 
 ```bash
-abcli git clone openai_cli install
+abcli git clone openai-commands install
 ```
 
 ```bash
 ...
 ```
 
 ## Completion
 
 ```bash
 @openai complete "describe mathematics"
 ```
 
 > Mathematics is an abstract science that examines topics such as quantity, structure, space, change, and other topics in various ways. It involves the use of logic, algorithms, and formulas to solve problems. Mathematics can be used to study the natural world, to describe phenomena, and to make predictions about the future. It provides the foundation for the development of a wide range of disciplines in science, technology, engineering, economics, finance, and more.
 
-also works [in a notebook](https://raw.githubusercontent.com/kamangir/openai-cli/main/notebooks/completion.ipynb).
+also works [in a notebook](https://raw.githubusercontent.com/kamangir/openai-commands/main/notebooks/completion.ipynb).
 
 ## Code Generation
 
-Example notebooks to [generate a python functions](https://raw.githubusercontent.com/kamangir/openai-cli/main/notebooks/completion_ai_function_py.ipynb), special case for [image to image python functions](https://raw.githubusercontent.com/kamangir/openai-cli/main/notebooks/completion_i2i_function.ipynb), and to [write a bash script](https://raw.githubusercontent.com/kamangir/openai-cli/main/notebooks/completion_ai_function_bash.ipynb) to use a script, for example, [Vancouver-Watching](https://github.com/kamangir/Vancouver-Watching).
+Example notebooks to [generate a python functions](https://raw.githubusercontent.com/kamangir/openai-commands/main/notebooks/completion_ai_function_py.ipynb), special case for [image to image python functions](https://raw.githubusercontent.com/kamangir/openai-commands/main/notebooks/completion_i2i_function.ipynb), and to [write a bash script](https://raw.githubusercontent.com/kamangir/openai-commands/main/notebooks/completion_ai_function_bash.ipynb) to use a script, for example, [Vancouver-Watching](https://github.com/kamangir/Vancouver-Watching).
 
-![image](https://raw.githubusercontent.com/kamangir/openai-cli/main/assets/completion_i2i_function.png)
+![image](https://raw.githubusercontent.com/kamangir/openai-commands/main/assets/completion_i2i_function.png)
 
 ## Sentence -> Image
 
 ```bash
 @select - open; \
 @openai generate image \
   ~dryrun,height=1024,width=1024 \
   carrot - \
   "an orange carrot walking on Mars."
 ```
 
-![image](https://raw.githubusercontent.com/kamangir/openai-cli/main/assets/carrot.png)
+![image](https://raw.githubusercontent.com/kamangir/openai-commands/main/assets/carrot.png)
 
 ## Text -> Mural
 
 "[The Laughing Heart](https://allpoetry.com/poem/14326890-The-Laughing-Heart-by-Charles-Bukowski)" by Charles Bukowski, [more examples](http://kamangir.net/private/?object=2023-03-26-19-10-26-51814).
 
 ```bash
 @select - open; \
 DALL-E render  \
   ~dryrun,publish,url,verbose \
   https://allpoetry.com/poem/14326890-The-Laughing-Heart-by-Charles-Bukowski
 ```
 
-![image](https://raw.githubusercontent.com/kamangir/openai-cli/main/assets/DALL-E.png)
+![image](https://raw.githubusercontent.com/kamangir/openai-commands/main/assets/DALL-E.png)
 
 ## Vision
 
 Implements the [OpenAI vision API](https://platform.openai.com/docs/guides/vision).
 
 > GPT-4 with Vision ... `GPT-4V` or `gpt-4-vision-preview` in the API ... model ... take in images and answer questions about them
 > ... not stateful ... ([more](https://arash-kamangir.medium.com/%EF%B8%8F-openai-vision-1-fb3691bd095a))
@@ -131,24 +131,24 @@
 
 > The images show street scenes captured by surveillance cameras at night, and each bears a timestamp and the text "CITY OF VANCOUVER" indicating they're from Vancouver. In the first image, you see a yellow traffic light indicating caution and part of a crosswalk painted in rainbow colors, likely symbolizing support for the LGBTQ+ community. In the second image, there's a view of a city street with pedestrians crossing, some wearing reflective vests, and the storefronts illuminated with bright lights. The third image shows a different angle of a similar street scene with the same vibrant crosswalk and vehicles' headlights creating streaks of light due to the camera exposure. Finally, in the fourth image, there's a view of parked cars and a clearly visible police vehicle, suggesting the presence of law enforcement nearby. The wet pavement suggests it may have rained, and the reflections imply the street is well-lit at night.
 
 ## images
 
 Implements the [OpenAI Image Generation API](https://platform.openai.com/docs/guides/images/usage?context=python).
 
-Notebook implementation [`https://raw.githubusercontent.com/kamangir/openai-cli/main/notebooks/images.ipynb`](https://raw.githubusercontent.com/kamangir/openai-cli/main/notebooks/images.ipynb),
+Notebook implementation [`https://raw.githubusercontent.com/kamangir/openai-commands/main/notebooks/images.ipynb`](https://raw.githubusercontent.com/kamangir/openai-commands/main/notebooks/images.ipynb),
 
 ```bash
 @select - open; \
 @openai images generate - \
 	"a person flying through the streets of Vancouver." \
 	. --verbose 1
 ```
 
-![image](https://github.com/kamangir/assets/blob/main/openai_cli/2024-01-20-19-00-28-67378.png?raw=true)
+![image](https://github.com/kamangir/assets/blob/main/openai_commands/2024-01-20-19-00-28-67378.png?raw=true)
 
 ## gpt
 
 co-authored with ChapGPT.
 
 ```bash
 gpt
@@ -163,23 +163,23 @@
 gpt list_models [-] \
 	[--log 0]
  . list models.
 ```
 
 ## VisuaLyze
 
-> How about calling it "VisuaLyze"? This name combines "visualize" and "analyze," reflecting the tool's capability to generate custom data visualizations and analyze user input through AI - OpenAI, [more](https://raw.githubusercontent.com/kamangir/openai-cli/main/openai_cli/VisuaLyze/)
+> How about calling it "VisuaLyze"? This name combines "visualize" and "analyze," reflecting the tool's capability to generate custom data visualizations and analyze user input through AI - OpenAI, [more](https://raw.githubusercontent.com/kamangir/openai-commands/main/openai_commands/VisuaLyze/)
 
 ```bash
 VisuaLyze run
 ```
 
-![image](https://github.com/kamangir/openai-cli/assets/1007567/7c0ed5f7-6941-451c-a17e-504c6adab23f)
+![image](https://github.com/kamangir/openai-commands/assets/1007567/7c0ed5f7-6941-451c-a17e-504c6adab23f)
 
-sample output for [`onlinefoods`](https://raw.githubusercontent.com/kamangir/openai-cli/main/assets/VisuaLyze/onlinefoods/).
+sample output for [`onlinefoods`](https://raw.githubusercontent.com/kamangir/openai-commands/main/assets/VisuaLyze/onlinefoods/).
 
 ```python
 import pandas as pd
 import matplotlib.pyplot as plt
 
 def VisuaLyze(df: pd.DataFrame()):
     # Generate a matplotlib visualization of one aspect of the dataset
```

