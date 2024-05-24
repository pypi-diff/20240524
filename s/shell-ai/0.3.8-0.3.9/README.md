# Comparing `tmp/shell-ai-0.3.8.tar.gz` & `tmp/shell-ai-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell-ai-0.3.8.tar", last modified: Mon Aug 21 19:13:31 2023, max compression
+gzip compressed data, was "shell-ai-0.3.9.tar", last modified: Mon Aug 21 19:38:59 2023, max compression
```

## Comparing `shell-ai-0.3.8.tar` & `shell-ai-0.3.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-08-21 19:13:31.420935 shell-ai-0.3.8/
--rw-r--r--   0 rick      (1000) rick      (1000)     1067 2023-08-21 08:20:38.000000 shell-ai-0.3.8/LICENSE
--rw-r--r--   0 rick      (1000) rick      (1000)     3457 2023-08-21 19:13:31.420935 shell-ai-0.3.8/PKG-INFO
--rw-r--r--   0 rick      (1000) rick      (1000)     3302 2023-08-21 19:13:27.000000 shell-ai-0.3.8/README.md
--rw-r--r--   0 rick      (1000) rick      (1000)       38 2023-08-21 19:13:31.420935 shell-ai-0.3.8/setup.cfg
--rw-r--r--   0 rick      (1000) rick      (1000)      662 2023-08-21 19:13:27.000000 shell-ai-0.3.8/setup.py
-drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-08-21 19:13:31.420935 shell-ai-0.3.8/shell_ai/
--rw-r--r--   0 rick      (1000) rick      (1000)        0 2023-08-21 08:20:38.000000 shell-ai-0.3.8/shell_ai/__init__.py
--rw-r--r--   0 rick      (1000) rick      (1000)      728 2023-08-21 08:30:49.000000 shell-ai-0.3.8/shell_ai/config.py
--rw-r--r--   0 rick      (1000) rick      (1000)     3888 2023-08-21 19:13:27.000000 shell-ai-0.3.8/shell_ai/main.py
-drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-08-21 19:13:31.420935 shell-ai-0.3.8/shell_ai.egg-info/
--rw-r--r--   0 rick      (1000) rick      (1000)     3457 2023-08-21 19:13:31.000000 shell-ai-0.3.8/shell_ai.egg-info/PKG-INFO
--rw-r--r--   0 rick      (1000) rick      (1000)      277 2023-08-21 19:13:31.000000 shell-ai-0.3.8/shell_ai.egg-info/SOURCES.txt
--rw-r--r--   0 rick      (1000) rick      (1000)        1 2023-08-21 19:13:31.000000 shell-ai-0.3.8/shell_ai.egg-info/dependency_links.txt
--rw-r--r--   0 rick      (1000) rick      (1000)       44 2023-08-21 19:13:31.000000 shell-ai-0.3.8/shell_ai.egg-info/entry_points.txt
--rw-r--r--   0 rick      (1000) rick      (1000)       78 2023-08-21 19:13:31.000000 shell-ai-0.3.8/shell_ai.egg-info/requires.txt
--rw-r--r--   0 rick      (1000) rick      (1000)        9 2023-08-21 19:13:31.000000 shell-ai-0.3.8/shell_ai.egg-info/top_level.txt
+drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-08-21 19:38:59.396476 shell-ai-0.3.9/
+-rw-r--r--   0 rick      (1000) rick      (1000)     1067 2023-08-21 08:20:38.000000 shell-ai-0.3.9/LICENSE
+-rw-r--r--   0 rick      (1000) rick      (1000)     3546 2023-08-21 19:38:59.396476 shell-ai-0.3.9/PKG-INFO
+-rw-r--r--   0 rick      (1000) rick      (1000)     3391 2023-08-21 19:38:33.000000 shell-ai-0.3.9/README.md
+-rw-r--r--   0 rick      (1000) rick      (1000)       38 2023-08-21 19:38:59.396476 shell-ai-0.3.9/setup.cfg
+-rw-r--r--   0 rick      (1000) rick      (1000)      662 2023-08-21 19:37:24.000000 shell-ai-0.3.9/setup.py
+drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-08-21 19:38:59.396476 shell-ai-0.3.9/shell_ai/
+-rw-r--r--   0 rick      (1000) rick      (1000)        0 2023-08-21 08:20:38.000000 shell-ai-0.3.9/shell_ai/__init__.py
+-rw-r--r--   0 rick      (1000) rick      (1000)      728 2023-08-21 08:30:49.000000 shell-ai-0.3.9/shell_ai/config.py
+-rw-r--r--   0 rick      (1000) rick      (1000)     4098 2023-08-21 19:37:02.000000 shell-ai-0.3.9/shell_ai/main.py
+drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-08-21 19:38:59.396476 shell-ai-0.3.9/shell_ai.egg-info/
+-rw-r--r--   0 rick      (1000) rick      (1000)     3546 2023-08-21 19:38:59.000000 shell-ai-0.3.9/shell_ai.egg-info/PKG-INFO
+-rw-r--r--   0 rick      (1000) rick      (1000)      277 2023-08-21 19:38:59.000000 shell-ai-0.3.9/shell_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 rick      (1000) rick      (1000)        1 2023-08-21 19:38:59.000000 shell-ai-0.3.9/shell_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 rick      (1000) rick      (1000)       44 2023-08-21 19:38:59.000000 shell-ai-0.3.9/shell_ai.egg-info/entry_points.txt
+-rw-r--r--   0 rick      (1000) rick      (1000)       78 2023-08-21 19:38:59.000000 shell-ai-0.3.9/shell_ai.egg-info/requires.txt
+-rw-r--r--   0 rick      (1000) rick      (1000)        9 2023-08-21 19:38:59.000000 shell-ai-0.3.9/shell_ai.egg-info/top_level.txt
```

### Comparing `shell-ai-0.3.8/LICENSE` & `shell-ai-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shell-ai-0.3.8/PKG-INFO` & `shell-ai-0.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-ai
-Version: 0.3.8
+Version: 0.3.9
 Author: Rick Lamers
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Shell-AI: Your Intelligent Command-Line Companion
 
@@ -53,14 +53,16 @@
 1. **`OPENAI_API_KEY`**: Required. Set this environment variable to your OpenAI API key. You can find it on your [OpenAI Dashboard](https://beta.openai.com/account/api-keys).
 
 ### Optional Variables
 
 1. **`OPENAI_MODEL`**: Defaults to `gpt-3.5-turbo`. You can set it to another OpenAI model if desired.
 2. **`SHAI_SUGGESTION_COUNT`**: Defaults to 3. You can set it to specify the number of suggestions to generate.
 3. **`OPENAI_API_BASE`**: Defaults to `https://api.openai.com/v1`. You can set it to specify the proxy or service emulator.
+4. **`OPENAI_ORGANIZATION`**: OpenAI Organization ID
+5. **`OPENAI_PROXY`**: OpenAI proxy
 
 ### Configuration File
 
 Alternatively, you can store these variables in a JSON configuration file:
 
 - For Linux/macOS: Create a file called `config.json` under `~/.config/shell-ai/` and secure it with `chmod 600 ~/.config/shell-ai/config.json`.
 - For Windows: Create a file called `config.json` under `%APPDATA%\shell-ai\`
```

### Comparing `shell-ai-0.3.8/README.md` & `shell-ai-0.3.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 1. **`OPENAI_API_KEY`**: Required. Set this environment variable to your OpenAI API key. You can find it on your [OpenAI Dashboard](https://beta.openai.com/account/api-keys).
 
 ### Optional Variables
 
 1. **`OPENAI_MODEL`**: Defaults to `gpt-3.5-turbo`. You can set it to another OpenAI model if desired.
 2. **`SHAI_SUGGESTION_COUNT`**: Defaults to 3. You can set it to specify the number of suggestions to generate.
 3. **`OPENAI_API_BASE`**: Defaults to `https://api.openai.com/v1`. You can set it to specify the proxy or service emulator.
+4. **`OPENAI_ORGANIZATION`**: OpenAI Organization ID
+5. **`OPENAI_PROXY`**: OpenAI proxy
 
 ### Configuration File
 
 Alternatively, you can store these variables in a JSON configuration file:
 
 - For Linux/macOS: Create a file called `config.json` under `~/.config/shell-ai/` and secure it with `chmod 600 ~/.config/shell-ai/config.json`.
 - For Windows: Create a file called `config.json` under `%APPDATA%\shell-ai\`
```

### Comparing `shell-ai-0.3.8/setup.py` & `shell-ai-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read README.md
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='shell-ai',
-    version='0.3.8',
+    version='0.3.9',
     author='Rick Lamers',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=requirements,
     extras_require={
         'dev': ['setuptools', 'wheel', 'twine']
```

### Comparing `shell-ai-0.3.8/shell_ai/config.py` & `shell-ai-0.3.9/shell_ai/config.py`

 * *Files identical despite different names*

### Comparing `shell-ai-0.3.8/shell_ai/main.py` & `shell-ai-0.3.9/shell_ai/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,21 +40,25 @@
         print(
             "You can also create `config.json` under `~/.config/shell-ai/` to set the API key, see README.md for more information."
         )
         sys.exit(1)
 
     OPENAI_MODEL = os.environ.get("OPENAI_MODEL", "gpt-3.5-turbo")
     OPENAI_API_BASE = os.environ.get("OPENAI_API_BASE", None)
+    OPENAI_ORGANIZATION = os.environ.get("OPENAI_ORGANIZATION", None)
+    OPENAI_PROXY = os.environ.get("OPENAI_PROXY", None)
     SHAI_SUGGESTION_COUNT = int(os.environ.get("SHAI_SUGGESTION_COUNT", 3))
     # End loading configuration
 
     chat = ChatOpenAI(
         model_name=OPENAI_MODEL,
         n=SHAI_SUGGESTION_COUNT,
         openai_api_base=OPENAI_API_BASE,
+        openai_organization=OPENAI_ORGANIZATION,
+        openai_proxy=OPENAI_PROXY,
     )
     system_message = SystemMessage(
         content="""You are an expert at using shell commands. Only provide a single executable line of shell code as output. Never output any text before or after the shell code, as the output will be directly executed in a shell. You're allowed to chain commands like `ls | grep .txt`."""
     )
 
     def get_suggestions(prompt):
         response = chat.generate(
```

### Comparing `shell-ai-0.3.8/shell_ai.egg-info/PKG-INFO` & `shell-ai-0.3.9/shell_ai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-ai
-Version: 0.3.8
+Version: 0.3.9
 Author: Rick Lamers
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Shell-AI: Your Intelligent Command-Line Companion
 
@@ -53,14 +53,16 @@
 1. **`OPENAI_API_KEY`**: Required. Set this environment variable to your OpenAI API key. You can find it on your [OpenAI Dashboard](https://beta.openai.com/account/api-keys).
 
 ### Optional Variables
 
 1. **`OPENAI_MODEL`**: Defaults to `gpt-3.5-turbo`. You can set it to another OpenAI model if desired.
 2. **`SHAI_SUGGESTION_COUNT`**: Defaults to 3. You can set it to specify the number of suggestions to generate.
 3. **`OPENAI_API_BASE`**: Defaults to `https://api.openai.com/v1`. You can set it to specify the proxy or service emulator.
+4. **`OPENAI_ORGANIZATION`**: OpenAI Organization ID
+5. **`OPENAI_PROXY`**: OpenAI proxy
 
 ### Configuration File
 
 Alternatively, you can store these variables in a JSON configuration file:
 
 - For Linux/macOS: Create a file called `config.json` under `~/.config/shell-ai/` and secure it with `chmod 600 ~/.config/shell-ai/config.json`.
 - For Windows: Create a file called `config.json` under `%APPDATA%\shell-ai\`
```

