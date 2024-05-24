# Comparing `tmp/miniogre-0.7.0.tar.gz` & `tmp/miniogre-0.8.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniogre-0.7.0.tar", max compression
+gzip compressed data, was "miniogre-0.8.0b0.tar", max compression
```

## Comparing `miniogre-0.7.0.tar` & `miniogre-0.8.0b0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-05-15 05:54:31.301456 miniogre-0.7.0/LICENSE
--rw-r--r--   0        0        0     4134 2024-05-15 05:54:31.301456 miniogre-0.7.0/README.md
--rw-r--r--   0        0        0      125 2024-05-15 05:54:31.301456 miniogre-0.7.0/miniogre/__init__.py
--rw-r--r--   0        0        0    22222 2024-05-15 05:54:31.305456 miniogre-0.7.0/miniogre/actions.py
--rw-r--r--   0        0        0     4564 2024-05-15 05:54:31.305456 miniogre-0.7.0/miniogre/config.py
--rw-r--r--   0        0        0    11469 2024-05-15 05:54:31.305456 miniogre-0.7.0/miniogre/constants.py
--rw-r--r--   0        0        0  1681126 2024-05-15 05:54:31.313456 miniogre-0.7.0/miniogre/encodings/9b5ad71b2ce5302211f9c61530b329a4922fc6a4
--rw-r--r--   0        0        0     3152 2024-05-15 05:54:31.313456 miniogre-0.7.0/miniogre/main.py
--rw-r--r--   0        0        0      902 2024-05-15 05:54:31.313456 miniogre-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5308 1970-01-01 00:00:00.000000 miniogre-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-24 04:35:03.683961 miniogre-0.8.0b0/LICENSE
+-rw-r--r--   0        0        0     4134 2024-05-24 04:35:03.683961 miniogre-0.8.0b0/README.md
+-rw-r--r--   0        0        0      125 2024-05-24 04:35:03.683961 miniogre-0.8.0b0/miniogre/__init__.py
+-rw-r--r--   0        0        0    27654 2024-05-24 04:35:03.683961 miniogre-0.8.0b0/miniogre/actions.py
+-rw-r--r--   0        0        0     4564 2024-05-24 04:35:03.683961 miniogre-0.8.0b0/miniogre/config.py
+-rw-r--r--   0        0        0    15429 2024-05-24 04:35:03.683961 miniogre-0.8.0b0/miniogre/constants.py
+-rw-r--r--   0        0        0  1681126 2024-05-24 04:35:03.695961 miniogre-0.8.0b0/miniogre/encodings/9b5ad71b2ce5302211f9c61530b329a4922fc6a4
+-rw-r--r--   0        0        0     3606 2024-05-24 04:35:03.695961 miniogre-0.8.0b0/miniogre/main.py
+-rw-r--r--   0        0        0      907 2024-05-24 04:35:03.695961 miniogre-0.8.0b0/pyproject.toml
+-rw-r--r--   0        0        0     5310 1970-01-01 00:00:00.000000 miniogre-0.8.0b0/PKG-INFO
```

### Comparing `miniogre-0.7.0/LICENSE` & `miniogre-0.8.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `miniogre-0.7.0/README.md` & `miniogre-0.8.0b0/README.md`

 * *Files identical despite different names*

### Comparing `miniogre-0.7.0/miniogre/actions.py` & `miniogre-0.8.0b0/miniogre/actions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import ast
 import os
 import platform
 import subprocess
-import tiktoken
+from string import Template
+
 import emoji
 import google.generativeai as googleai
+import tiktoken
 from groq import Groq
 # from groq.cloud.core import Completion
 from mistralai.client import MistralClient
 from mistralai.models.chat_completion import ChatMessage
 from octoai.client import Client as OctoAiClient
 from openai import OpenAI
 from pyfiglet import Figlet
@@ -46,14 +48,18 @@
     print(emoji.emojize(":magnifying_glass_tilted_left: Generating context..."))
 
 
 def readme_emoji():
     print(emoji.emojize(":notebook: Generating new README.md..."))
 
 
+def eval_emoji():
+    print(emoji.emojize(":magnifying_glass_tilted_left: Evaluating..."))
+
+
 def list_files(project_path):
     # List all files in current directory and subdirectories
     files = []
     for root, dirs, filenames in os.walk(project_path):
         if ".git" in dirs:
             dirs.remove(".git")
         if "__pycache__" in dirs:
@@ -433,17 +439,18 @@
     with open(requirements_fullpath, "w") as f:
         f.write(requirements)
     return requirements_fullpath
 
 
 def count_tokens(string) -> int:
     from importlib.resources import files
-    tiktoken_cache_dir = str(files('miniogre').joinpath('encodings'))
+
+    tiktoken_cache_dir = str(files("miniogre").joinpath("encodings"))
     os.environ["TIKTOKEN_CACHE_DIR"] = tiktoken_cache_dir
-    cache_key = "9b5ad71b2ce5302211f9c61530b329a4922fc6a4" # cl100k_base
+    cache_key = "9b5ad71b2ce5302211f9c61530b329a4922fc6a4"  # cl100k_base
     assert os.path.exists(os.path.join(tiktoken_cache_dir, cache_key))
     encoding = tiktoken.get_encoding("cl100k_base")
     num_tokens = len(encoding.encode(string))
     return num_tokens
 
 
 def rewrite_readme(provider, readme):
@@ -489,16 +496,16 @@
 
 def rewrite_readme_gemini(readme):
     model = os.getenv("GEMINI_MODEL", GEMINI_MODEL)
     prompt = os.getenv("REWRITE_README_PROMPT", REWRITE_README_PROMPT)
     full_prompt = f"{prompt}\n---\n{readme}"
     # print(f"{model=} {full_prompt=}")
     new_readme = ""
-    if "GOOGLE_API_KEY" not in os.environ:
-        raise EnvironmentError("GOOGLE_API_KEY environment variable not defined")
+    if "GEMINI_API_KEY" not in os.environ:
+        raise EnvironmentError("GEMINI_API_KEY environment variable not defined")
     try:
         client = googleai.GenerativeModel(model)
         response = client.generate_content(full_prompt)
         new_readme = response.text
     except Exception as e:
         print(e)
     return new_readme
@@ -732,7 +739,155 @@
 
 def cleanup():
     """
     Delete unnecessary files
     """
     if os.path.exists("ogre_dir/gptify_output.txt"):
         os.remove("ogre_dir/gptify_output.txt")
+
+
+def read_readme(repo_path):
+    # List of possible README file names (without specific case)
+    possible_names = ["README.md", "README.txt", "README.rst", "README.adoc", "README"]
+
+    # Get all files in the directory
+    files_in_directory = os.listdir(repo_path)
+
+    # Check for each possible README name in a case-insensitive manner
+    for name in possible_names:
+        for file in files_in_directory:
+            if file.lower() == name.lower():
+                readme_path = os.path.join(repo_path, file)
+                with open(readme_path, "r", encoding="utf-8") as file:
+                    content = file.read()
+                    return content
+
+    # If no README file is found, raise an exception
+    raise FileNotFoundError("No README file found in the repository.")
+
+
+def evaluate_readme(provider, readme, verbose):
+    eval_emoji()
+    if provider == "openai":
+        return evaluate_readme_openai(readme, verbose)
+    elif provider == "gemini":
+        return evaluate_readme_gemini(readme, verbose)
+    elif provider == "ollama":
+        return evaluate_readme_ollama(readme, verbose)
+    elif provider == "groq":
+        return evaluate_readme_groq(readme, verbose)
+    elif provider == "octoai":
+        # return evaluate_readme_octoai(readme, verbose)
+        raise NotImplementedError("This provider is not yet implemented")
+    elif provider == "mistral":
+        # res = evaluate_readme_mistral(readme, verbose)
+        raise NotImplementedError("This provider is not yet implemented")
+    else:
+        raise ValueError("Invalid provider")
+
+
+def evaluate_readme_openai(readme, verbose):
+    model = os.getenv("OPENAI_MODEL", OPENAI_MODEL)
+    system_prompt = os.getenv("README_EVAL_SYSTEM_PROMPT", README_EVAL_SYSTEM_PROMPT)
+    user_prompt_template = Template(
+        os.getenv("README_EVAL_USER_PROMPT", README_EVAL_USER_PROMPT)
+    )
+    user_prompt = user_prompt_template.substitute(README=readme)
+    if verbose:
+        print(f"\n{model=}\n{system_prompt=}\n{user_prompt=}\n")
+    score = "0"
+    if "OPENAI_API_KEY" not in os.environ:
+        raise EnvironmentError("OPENAI_API_KEY environment variable not defined")
+    try:
+        client = OpenAI()
+        completion = client.chat.completions.create(
+            model=model,
+            seed=0,
+            messages=[
+                {"role": "system", "content": system_prompt},
+                {"role": "user", "content": user_prompt},
+            ],
+        )
+        score = completion.choices[0].message.content
+        if verbose:
+            print(f"\n{score=}\n")
+    except Exception as e:
+        print(e)
+    return score
+
+
+def evaluate_readme_gemini(readme, verbose):
+    model = os.getenv("GEMINI_MODEL", GEMINI_MODEL)
+    prompt_template = Template(os.getenv("README_EVAL_PROMPT", README_EVAL_PROMPT))
+    prompt = prompt_template.substitute(README=readme)
+    if verbose:
+        print(f"\n{model=}\n{prompt=}\n")
+    score = "0"
+    if "GEMINI_API_KEY" not in os.environ:
+        raise EnvironmentError("GEMINI_API_KEY environment variable not defined")
+    try:
+        client = googleai.GenerativeModel(model)
+        response = client.generate_content(prompt)
+        score = response.text
+        if verbose:
+            print(f"\n{score=}\n")
+    except Exception as e:
+        print(e)
+    return score
+
+
+def evaluate_readme_ollama(readme, verbose):
+    model = os.getenv("OLLAMA_MODEL", OLLAMA_MODEL)
+    api_server = os.getenv("OLLAMA_API_SERVER", OLLAMA_API_SERVER)
+    system_prompt = os.getenv("README_EVAL_SYSTEM_PROMPT", README_EVAL_SYSTEM_PROMPT)
+    user_prompt_template = Template(
+        os.getenv("README_EVAL_USER_PROMPT", README_EVAL_USER_PROMPT)
+    )
+    user_prompt = user_prompt_template.substitute(README=readme)
+    if verbose:
+        print(f"\n{model=}\n{api_server=}\n{system_prompt=}\n{user_prompt=}\n")
+    score = "0"
+    try:
+        client = OpenAI(base_url=api_server, api_key="ollama")
+        completion = client.chat.completions.create(
+            model=model,
+            seed=0,
+            messages=[
+                {"role": "system", "content": system_prompt},
+                {"role": "user", "content": user_prompt},
+            ],
+        )
+        score = completion.choices[0].message.content
+        if verbose:
+            print(f"\n{score=}\n")
+    except Exception as e:
+        print(e)
+    return score
+
+
+def evaluate_readme_groq(readme, verbose):
+    model = os.getenv("GROQ_MODEL", GROQ_MODEL)
+    prompt_template = Template(os.getenv("README_EVAL_PROMPT", README_EVAL_PROMPT))
+    prompt = prompt_template.substitute(README=readme)
+    if verbose:
+        print(f"\n{model=}\n{prompt=}\n")
+    score = "0"
+    if "GROQ_API_KEY" not in os.environ:
+        raise EnvironmentError("GROQ_API_KEY environment variable not defined")
+    try:
+        client = Groq(api_key=os.environ.get("GROQ_API_KEY"))
+        chat_completion = client.chat.completions.create(
+            messages=[
+                {
+                    "role": "user",
+                    "content": prompt,
+                }
+            ],
+            model=model,
+            seed=0,
+        )
+        score = chat_completion.choices[0].message.content
+        if verbose:
+            print(f"\n{score=}\n")
+    except Exception as e:
+        print(e)
+    return score
```

### Comparing `miniogre-0.7.0/miniogre/config.py` & `miniogre-0.8.0b0/miniogre/config.py`

 * *Files identical despite different names*

### Comparing `miniogre-0.7.0/miniogre/encodings/9b5ad71b2ce5302211f9c61530b329a4922fc6a4` & `miniogre-0.8.0b0/miniogre/encodings/9b5ad71b2ce5302211f9c61530b329a4922fc6a4`

 * *Files identical despite different names*

### Comparing `miniogre-0.7.0/miniogre/main.py` & `miniogre-0.8.0b0/miniogre/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import importlib.metadata
 import os
-
 import typer
+
 from dotenv import load_dotenv
 from openai import OpenAI
 
 from .actions import *
 from .config import *
 
 app = typer.Typer()
@@ -43,14 +43,32 @@
     print("Total number of tokens: {}".format(num_tokens))
     new_readme = rewrite_readme(provider, context_contents)
     readme_path = save_readme(new_readme, ogre_dir_path)
     end_emoji()
 
     return 0
 
+@app.command()
+def eval(provider: str = "openai", verbose: bool = False):
+    """
+    Determine the reproducibility score of the repository
+    """
+
+    display_figlet()
+    starting_emoji()
+
+    # Start by evaluating the README quality
+    readme = read_readme(os.getcwd())
+    readme_score = evaluate_readme(provider, readme, verbose)
+    print(emoji.emojize(":upside-down_face: Readme score: {}".format(readme_score)))
+
+    end_emoji()
+
+    return 0
+
 
 @app.command()
 def run(
     provider: str = "openai",
     baseimage: str = "auto",
     port_map: str = "8001:8001",
     dry: bool = False,
```

### Comparing `miniogre-0.7.0/pyproject.toml` & `miniogre-0.8.0b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "miniogre"
-version = "0.7.0"
+version = "0.8.0-beta"
 description = "miniogre: from source code to reproducible environment, in seconds."
 readme = "README.md"
 authors = ["Wilder Lopes <wilder@ogre.run>"]
 include = [
     { path = "miniogre/encodings", format = ["sdist", "wheel"] }
 ]
 homepage = "https://github.com/ogre-run/miniogre"
```

### Comparing `miniogre-0.7.0/PKG-INFO` & `miniogre-0.8.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniogre
-Version: 0.7.0
+Version: 0.8.0b0
 Summary: miniogre: from source code to reproducible environment, in seconds.
 Home-page: https://github.com/ogre-run/miniogre
 Author: Wilder Lopes
 Author-email: wilder@ogre.run
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

